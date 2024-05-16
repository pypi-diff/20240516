# Comparing `tmp/pathlibs3-0.2.3.tar.gz` & `tmp/pathlibs3-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathlibs3-0.2.3.tar", max compression
+gzip compressed data, was "pathlibs3-0.2.4.tar", max compression
```

## Comparing `pathlibs3-0.2.3.tar` & `pathlibs3-0.2.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.3/pathlibs3/__init__.py
--rw-r--r--   0        0        0     4551 2024-05-16 15:19:27.581936 pathlibs3-0.2.3/pathlibs3/pathlibs3.py
--rw-r--r--   0        0        0      384 2024-05-16 15:19:47.169619 pathlibs3-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 pathlibs3-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.4/pathlibs3/__init__.py
+-rw-r--r--   0        0        0     4636 2024-05-16 16:55:44.797522 pathlibs3-0.2.4/pathlibs3/pathlibs3.py
+-rw-r--r--   0        0        0      384 2024-05-16 16:56:30.064900 pathlibs3-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 pathlibs3-0.2.4/PKG-INFO
```

### Comparing `pathlibs3-0.2.3/pathlibs3/pathlibs3.py` & `pathlibs3-0.2.4/pathlibs3/pathlibs3.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,17 +58,19 @@
         sub_folders = list()
 
         result = self.client.list_objects(
             Bucket=self.bucket, Prefix=self.path, Delimiter="/"
         )
         for object in self._retrieve_folder_contents(result):
             object = S3Path(self.client, self.bucket, object)
+            if object.path == self.path:
+                continue
             sub_folders.append(object)
             if object.is_dir() and recursive:
-                subfolder = object.iterdir()
+                subfolder = object.iterdir(recursive=recursive)
                 sub_folders += subfolder
 
         if only_files:
             sub_folders = [x for x in sub_folders if not x.is_dir()]
 
         for subfolder in sub_folders:
             yield subfolder
```

