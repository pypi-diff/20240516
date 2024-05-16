# Comparing `tmp/pathlibs3-0.2.1.tar.gz` & `tmp/pathlibs3-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathlibs3-0.2.1.tar", max compression
+gzip compressed data, was "pathlibs3-0.2.2.tar", max compression
```

## Comparing `pathlibs3-0.2.1.tar` & `pathlibs3-0.2.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.1/pathlibs3/__init__.py
--rw-r--r--   0        0        0     3305 2024-05-16 12:51:23.982420 pathlibs3-0.2.1/pathlibs3/pathlibs3.py
--rw-r--r--   0        0        0      382 2024-05-16 13:10:26.086521 pathlibs3-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 pathlibs3-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.2/pathlibs3/__init__.py
+-rw-r--r--   0        0        0     3854 2024-05-16 14:23:22.923680 pathlibs3-0.2.2/pathlibs3/pathlibs3.py
+-rw-r--r--   0        0        0      384 2024-05-16 14:26:21.653181 pathlibs3-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 pathlibs3-0.2.2/PKG-INFO
```

### Comparing `pathlibs3-0.2.1/pathlibs3/pathlibs3.py` & `pathlibs3-0.2.2/pathlibs3/pathlibs3.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,90 +6,111 @@
 
 
 class S3Path:
     def __init__(self, client: boto3.client, bucket: str, path: str):
         self.client = client
         self.bucket = bucket
         self.path = path
-    
+
+    def __repr__(self):
+        return f"S3Path(bucket={self.bucket}, path={self.path})"
+
     def __eq__(self, other) -> bool:
-        return self.path == other.path and self.client == other.client and self.bucket == other.bucket
-    
+        return (
+            self.path == other.path
+            and self.client == other.client
+            and self.bucket == other.bucket
+        )
+
     def __str__(self):
         return self.path
-    
+
     def _retrieve_folder_contents(self, results):
         contents = []
-        if 'CommonPrefixes' in results.keys():
-            contents +=  [x["Prefix"] for x in results.get('CommonPrefixes')]
-        if 'Contents' in results.keys():
-             contents += [x["Key"] for x in results.get("Contents")]
-    
+        if "CommonPrefixes" in results.keys():
+            contents += [x["Prefix"] for x in results.get("CommonPrefixes")]
+        if "Contents" in results.keys():
+            contents += [x["Key"] for x in results.get("Contents")]
+
         return contents
-    
-    def iterdir(self, recursive: bool=False, only_files: bool=False):
+
+    def iterdir(self, recursive: bool = False, only_files: bool = False):
         logging.warning("looking for folder %s", self.path)
         sub_folders = list()
 
-        result = self.client.list_objects(Bucket=self.bucket, Prefix=self.path, Delimiter='/')
+        result = self.client.list_objects(
+            Bucket=self.bucket, Prefix=self.path, Delimiter="/"
+        )
         for object in self._retrieve_folder_contents(result):
             object = S3Path(self.client, self.bucket, object)
             sub_folders.append(object)
             if object.is_dir() and recursive:
                 subfolder = object.iterdir()
                 sub_folders += subfolder
 
         if only_files:
             sub_folders = [x for x in sub_folders if not x.is_dir()]
 
         for subfolder in sub_folders:
             yield subfolder
-        
+
     def is_dir(self):
         return self.path.endswith("/")
 
     def exists(self):
         try:
             self.client.head_object(Bucket=self.bucket, Key=self.path)
             return True
         except botocore.exceptions.ClientError as e:
             if e.response["Error"]["Code"] == "404":
                 return False
             else:
                 raise
 
+    @property
+    def name(self):
+        return Path(self.path).name
+
+    def __truediv__(self, other: str) -> "S3Path":
+        return S3Path(
+            client=self.client,
+            bucket=self.bucket,
+            path=str(Path(self.path) / other),
+        )
+
     @classmethod
     def _copy_from_s3_to_s3(cls, source: "S3Path", destination: "S3Path"):
         client = source.client
-        copy_source = {
-                'Bucket': source.bucket,
-                'Key': source.path
-            }
+        copy_source = {"Bucket": source.bucket, "Key": source.path}
         client.copy(copy_source, destination.bucket, destination.path)
-    
+
     @classmethod
     def _copy_from_local_to_s3(cls, source: Path, destination: "S3Path"):
         client = destination.client
         client.upload_file(str(source), destination.bucket, destination.path)
-    
+
     @classmethod
     def _copy_from_s3_to_local(cls, source: "S3Path", destination: Path):
         client = source.client
-        with open(str(destination), 'wb') as f:
+        with open(str(destination), "wb") as f:
             client.download_fileobj(source.bucket, source.path, f)
-    
-    @classmethod
-    def copy(cls, source: Union["S3Path", Path], destination: Union["S3Path", Path]):
-        if isinstance(source, S3Path) and isinstance(destination, S3Path):
-            cls._copy_from_s3_to_s3(source, destination)
-        
-        if isinstance(source, Path) and isinstance(destination, S3Path):
-            cls._copy_from_local_to_s3(source, destination)
-        
-        if isinstance(source, S3Path) and isinstance(destination, Path):
-            cls._copy_from_s3_to_local(source, destination)
 
-            
+    @classmethod
+    def copy(cls, origin: Union["S3Path", Path], destination: Union["S3Path", Path]):
+        if origin.is_dir():
+            for path in origin.iterdir():
+                cls.copy(path, destination / path.name)
+
+        else:
+            if isinstance(origin, S3Path) and isinstance(destination, S3Path):
+                cls._copy_from_s3_to_s3(origin, destination)
+
+            if isinstance(origin, Path) and isinstance(destination, S3Path):
+                cls._copy_from_local_to_s3(origin, destination)
+
+            if isinstance(origin, S3Path) and isinstance(destination, Path):
+                destination.parent.mkdir(parents=True, exist_ok=True)
+                cls._copy_from_s3_to_local(origin, destination)
 
     @property
     def parent(self):
-        return S3Path(self.client, self.bucket, str(Path(self.path).parent))
+        return S3Path(self.client, self.bucket, str(Path(self.path).parent))
```

