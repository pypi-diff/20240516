# Comparing `tmp/s3func-0.1.1.tar.gz` & `tmp/s3func-0.1.2.tar.gz`

## Comparing `s3func-0.1.1.tar` & `s3func-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 s3func-0.1.1/s3func/__init__.py
--rw-r--r--   0        0        0    16689 2020-02-02 00:00:00.000000 s3func-0.1.1/s3func/main.py
--rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 s3func-0.1.1/s3func/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 s3func-0.1.1/s3func/tests/__init__.py
--rw-r--r--   0        0        0   285095 2020-02-02 00:00:00.000000 s3func-0.1.1/s3func/tests/stns_data.blt
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 s3func-0.1.1/s3func/tests/test_s3func.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 s3func-0.1.1/.gitignore
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 s3func-0.1.1/LICENSE
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 s3func-0.1.1/README.md
--rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 s3func-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 s3func-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 s3func-0.1.2/s3func/__init__.py
+-rw-r--r--   0        0        0    19646 2020-02-02 00:00:00.000000 s3func-0.1.2/s3func/main.py
+-rw-r--r--   0        0        0     5275 2020-02-02 00:00:00.000000 s3func-0.1.2/s3func/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 s3func-0.1.2/s3func/tests/__init__.py
+-rw-r--r--   0        0        0   285095 2020-02-02 00:00:00.000000 s3func-0.1.2/s3func/tests/stns_data.blt
+-rw-r--r--   0        0        0     5591 2020-02-02 00:00:00.000000 s3func-0.1.2/s3func/tests/test_s3func.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 s3func-0.1.2/.gitignore
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 s3func-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 s3func-0.1.2/README.md
+-rw-r--r--   0        0        0     3299 2020-02-02 00:00:00.000000 s3func-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 s3func-0.1.2/PKG-INFO
```

### Comparing `s3func-0.1.1/s3func/main.py` & `s3func-0.1.2/s3func/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from typing import List, Union
 import boto3
 import botocore
 import copy
 # import requests
 import urllib.parse
 from urllib3.util import Retry, Timeout
+import datetime
 # from requests import Session
 # from requests.adapters import HTTPAdapter
 import urllib3
 
 from . import utils
 # import utils
 
@@ -215,16 +216,16 @@
 
     try:
         response = s3.get_object(**params)
         stream = response['Body']
         stream.status = 200
         stream.etag = response['ETag'].strip('"')
         stream.content_length = response['ContentLength']
-        stream.last_modified = response['LastModified']
         stream.version_id = response['VersionId']
+        stream.last_modified = datetime.datetime.fromtimestamp(int(response['VersionId'].split('_u')[1]) * 0.001, datetime.timezone.utc)
         stream.metadata = response['Metadata']
     except s3.exceptions.NoSuchKey:
         stream = utils.S3ErrorResponse()
         stream.status = 404
 
     return stream
 
@@ -267,14 +268,90 @@
 
     else:
         raise TypeError('One of s3, connection_config, or public_url needs to be correctly defined.')
 
     return stream
 
 
+def url_to_headers(url: HttpUrl, session: urllib3.poolmanager.PoolManager=None, **url_session_kwargs):
+    """
+
+    """
+    if session is None:
+        session = url_session(**url_session_kwargs)
+
+    response = session.request('head', url)
+
+    headers = dict(response.headers)
+    headers['content_length'] = int(headers['Content-Length'])
+    if 'x-bz-file-id' in headers:
+        headers['version_id'] = headers['x-bz-file-id']
+    if 'X-Bz-Upload-Timestamp' in headers:
+        headers['last_modified'] = datetime.datetime.fromtimestamp(int(headers['X-Bz-Upload-Timestamp']) * 0.001, datetime.timezone.utc)
+    elif 'x-bz-file-id' in headers:
+        headers['last_modified'] = datetime.datetime.fromtimestamp(int(headers['x-bz-file-id'].split('_u')[1]) * 0.001, datetime.timezone.utc)
+
+    return headers
+
+
+def base_url_to_headers(obj_key: str, base_url: HttpUrl, session: urllib3.poolmanager.PoolManager=None, **url_session_kwargs):
+    """
+
+    """
+    if not base_url.endswith('/'):
+        base_url += '/'
+    url = urllib.parse.urljoin(base_url, obj_key)
+    headers = url_to_headers(url, session, **url_session_kwargs)
+
+    return headers
+
+
+def head_object(obj_key: str, bucket: str, s3: botocore.client.BaseClient = None, version_id: str=None, **s3_client_kwargs):
+    """
+    Function to get an object from an S3 bucket. Either s3 or connection_config must be used. This function will return a file object of the object in the S3 location. This file object does not contain any data until data is read from it, which ensures large files are not completely read into memory.
+
+    Parameters
+    ----------
+    obj_key : str
+        The object key in the S3 bucket.
+    bucket : str
+        The bucket name.
+    s3 : botocore.client.BaseClient
+        An S3 client object created via the s3_client function.
+    version_id : str
+        The S3 version id associated with the object.
+    s3_client_kwargs:
+        kwargs to the s3_client function if the s3 parameter was not passed.
+
+    Returns
+    -------
+    read-only file obj
+    """
+    ## Get the object
+    if s3 is None:
+        s3 = s3_client(**s3_client_kwargs)
+
+    params = utils.build_s3_params(bucket, obj_key=obj_key, version_id=version_id)
+
+    try:
+        response = s3.head_object(**params)
+        response['status']= 200
+        response['etag'] = response.pop('ETag').strip('"')
+        response['content_length'] = response.pop('ContentLength')
+        response['version_id'] = response.pop('VersionId')
+        response['last_modified'] = datetime.datetime.fromtimestamp(int(response['version_id'].split('_u')[1]) * 0.001, datetime.timezone.utc)
+        response['metadata'] = response.pop('Metadata')
+        del response['LastModified']
+    except s3.exceptions.NoSuchKey:
+        response = utils.S3ErrorResponse()
+        response['status'] = 404
+
+    return response
+
+
 def put_object(s3: botocore.client.BaseClient, bucket: str, obj_key: str, obj: Union[bytes, io.BufferedIOBase], metadata: dict=None, content_type: str=None, object_legal_hold: bool=False):
     """
     Function to upload data to an S3 bucket. This function will iteratively write the input file_obj in chunks ensuring that little memory is needed writing the object.
 
     Parameters
     ----------
     s3 : boto3.client
```

### Comparing `s3func-0.1.1/s3func/utils.py` & `s3func-0.1.2/s3func/utils.py`

 * *Files identical despite different names*

### Comparing `s3func-0.1.1/s3func/tests/stns_data.blt` & `s3func-0.1.2/s3func/tests/stns_data.blt`

 * *Files identical despite different names*

### Comparing `s3func-0.1.1/s3func/tests/test_s3func.py` & `s3func-0.1.2/s3func/tests/test_s3func.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,32 @@
 
     stream2 = base_url_to_stream(obj_key, base_url)
     data2 = stream2.read()
 
     assert data1 == data2
 
 
+def test_head_object():
+    """
+
+    """
+    headers = head_object(obj_key, bucket, s3)
+
+    assert 'version_id' in headers
+
+
+def test_url_to_headers():
+    """
+
+    """
+    headers = url_to_headers(url)
+
+    assert 'version_id' in headers
+
+
 def test_legal_hold():
     """
 
     """
     hold = get_object_legal_hold(s3, bucket, obj_key)
     if hold:
         raise ValueError("There's a hold, but there shouldn't be.")
```

### Comparing `s3func-0.1.1/.gitignore` & `s3func-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `s3func-0.1.1/LICENSE` & `s3func-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `s3func-0.1.1/README.md` & `s3func-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `s3func-0.1.1/pyproject.toml` & `s3func-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `s3func-0.1.1/PKG-INFO` & `s3func-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: s3func
-Version: 0.1.1
+Version: 0.1.2
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
-Metadata-Version: 2.3 Name: s3func Version: 0.1.1 Summary: Simple functions for
+Metadata-Version: 2.3 Name: s3func Version: 0.1.2 Summary: Simple functions for
 working with S3 Project-URL: Documentation, https://mullenkamp.github.io/
 s3func/ Project-URL: Source, https://github.com/mullenkamp/s3func Author-email:
 s3func
 gmail.com> License-File: LICENSE Classifier: Programming Language :: Python ::
 3 :: Only Requires-Python: >=3.9 Requires-Dist: boto3 Requires-Dist: pydantic
 Requires-Dist: urllib3 Description-Content-Type: text/markdown # s3func
                      SSiimmppllee ffuunnccttiioonnss ffoorr wwoorrkkiinngg wwiitthh SS33
```

