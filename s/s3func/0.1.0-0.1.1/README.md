# Comparing `tmp/s3func-0.1.0.tar.gz` & `tmp/s3func-0.1.1.tar.gz`

## Comparing `s3func-0.1.0.tar` & `s3func-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 s3func-0.1.0/s3func/__init__.py
--rw-r--r--   0        0        0    16281 2020-02-02 00:00:00.000000 s3func-0.1.0/s3func/main.py
--rw-r--r--   0        0        0     5244 2020-02-02 00:00:00.000000 s3func-0.1.0/s3func/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 s3func-0.1.0/s3func/tests/__init__.py
--rw-r--r--   0        0        0   285095 2020-02-02 00:00:00.000000 s3func-0.1.0/s3func/tests/stns_data.blt
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 s3func-0.1.0/s3func/tests/test_s3func.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 s3func-0.1.0/.gitignore
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 s3func-0.1.0/LICENSE
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 s3func-0.1.0/README.md
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 s3func-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 s3func-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 s3func-0.1.1/s3func/__init__.py
+-rw-r--r--   0        0        0    16689 2020-02-02 00:00:00.000000 s3func-0.1.1/s3func/main.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 s3func-0.1.1/s3func/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 s3func-0.1.1/s3func/tests/__init__.py
+-rw-r--r--   0        0        0   285095 2020-02-02 00:00:00.000000 s3func-0.1.1/s3func/tests/stns_data.blt
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 s3func-0.1.1/s3func/tests/test_s3func.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 s3func-0.1.1/.gitignore
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 s3func-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 s3func-0.1.1/README.md
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 s3func-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 s3func-0.1.1/PKG-INFO
```

### Comparing `s3func-0.1.0/s3func/main.py` & `s3func-0.1.1/s3func/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -159,14 +159,15 @@
     """
     if session is None:
         session = url_session(**url_session_kwargs)
 
     headers = utils.build_url_headers(range_start=range_start, range_end=range_end)
 
     response = session.request('get', url, headers=headers, preload_content=False)
+    response.content_length = int(response.headers['Content-Length'])
 
     return response
 
 
 def base_url_to_stream(obj_key: str, base_url: HttpUrl, session: urllib3.poolmanager.PoolManager=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, **url_session_kwargs):
     """
 
@@ -208,18 +209,28 @@
     """
     ## Get the object
     if s3 is None:
         s3 = s3_client(**s3_client_kwargs)
 
     params = utils.build_s3_params(bucket, obj_key=obj_key, version_id=version_id, range_start=range_start, range_end=range_end)
 
-    response = s3.get_object(**params)
-    # response['ResponseMetadata']['ETag'] = response['ResponseMetadata']['ETag'].strip('"')
+    try:
+        response = s3.get_object(**params)
+        stream = response['Body']
+        stream.status = 200
+        stream.etag = response['ETag'].strip('"')
+        stream.content_length = response['ContentLength']
+        stream.last_modified = response['LastModified']
+        stream.version_id = response['VersionId']
+        stream.metadata = response['Metadata']
+    except s3.exceptions.NoSuchKey:
+        stream = utils.S3ErrorResponse()
+        stream.status = 404
 
-    return response['Body']
+    return stream
 
 
 def get_object_combo(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, session: urllib3.poolmanager.PoolManager=None, base_url: HttpUrl=None, version_id: str=None, range_start: int=None, range_end: int=None, chunk_size: int=524288, **kwargs):
     """
     Combo function to get an object from an S3 bucket either using the S3 get_object function or the base_url_to_stream function. One of s3, connection_config, or base_url must be used. This function will return a file object of the object in the S3 (or url) location. This file object does not contain any data until data is read from it, which ensures large files are not completely read into memory.
 
     Parameters
```

### Comparing `s3func-0.1.0/s3func/utils.py` & `s3func-0.1.1/s3func/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,16 @@
 #         timeout = kwargs.get("timeout")
 #         if timeout is None and hasattr(self, 'timeout'):
 #             kwargs["timeout"] = self.timeout
 #         return super().send(request, **kwargs)
 
 
 
-
+class S3ErrorResponse:
+    pass
```

### Comparing `s3func-0.1.0/s3func/tests/stns_data.blt` & `s3func-0.1.1/s3func/tests/stns_data.blt`

 * *Files identical despite different names*

### Comparing `s3func-0.1.0/s3func/tests/test_s3func.py` & `s3func-0.1.1/s3func/tests/test_s3func.py`

 * *Files identical despite different names*

### Comparing `s3func-0.1.0/.gitignore` & `s3func-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `s3func-0.1.0/LICENSE` & `s3func-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `s3func-0.1.0/README.md` & `s3func-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `s3func-0.1.0/pyproject.toml` & `s3func-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `s3func-0.1.0/PKG-INFO` & `s3func-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: s3func
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple functions for working with S3
 Project-URL: Documentation, https://mullenkamp.github.io/s3func/
 Project-URL: Source, https://github.com/mullenkamp/s3func
 Author-email: s3func <mullenkamp1@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: s3func Version: 0.1.0 Summary: Simple functions for
+Metadata-Version: 2.3 Name: s3func Version: 0.1.1 Summary: Simple functions for
 working with S3 Project-URL: Documentation, https://mullenkamp.github.io/
 s3func/ Project-URL: Source, https://github.com/mullenkamp/s3func Author-email:
 s3func
 gmail.com> License-File: LICENSE Classifier: Programming Language :: Python ::
 3 :: Only Requires-Python: >=3.9 Requires-Dist: boto3 Requires-Dist: pydantic
 Requires-Dist: urllib3 Description-Content-Type: text/markdown # s3func
                      SSiimmppllee ffuunnccttiioonnss ffoorr wwoorrkkiinngg wwiitthh SS33
```

