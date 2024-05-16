# Comparing `tmp/pathlibs3-0.2.2.tar.gz` & `tmp/pathlibs3-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathlibs3-0.2.2.tar", max compression
+gzip compressed data, was "pathlibs3-0.2.3.tar", max compression
```

## Comparing `pathlibs3-0.2.2.tar` & `pathlibs3-0.2.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.2/pathlibs3/__init__.py
--rw-r--r--   0        0        0     3854 2024-05-16 14:23:22.923680 pathlibs3-0.2.2/pathlibs3/pathlibs3.py
--rw-r--r--   0        0        0      384 2024-05-16 14:26:21.653181 pathlibs3-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 pathlibs3-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.3/pathlibs3/__init__.py
+-rw-r--r--   0        0        0     4551 2024-05-16 15:19:27.581936 pathlibs3-0.2.3/pathlibs3/pathlibs3.py
+-rw-r--r--   0        0        0      384 2024-05-16 15:19:47.169619 pathlibs3-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 pathlibs3-0.2.3/PKG-INFO
```

### Comparing `pathlibs3-0.2.2/pathlibs3/pathlibs3.py` & `pathlibs3-0.2.3/pathlibs3/pathlibs3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,32 @@
 import boto3
 import logging
 from pathlib import Path
 import botocore
 from typing import Union
+from botocore.exceptions import ClientError
+
+
+def upload_file(
+    client, source, destination_bucket, destination_path, exists_ok: bool = False
+):
+    try:
+        exist = True
+        if not exists_ok:
+            try:
+                client.head_object(Bucket=destination_bucket, Key=destination_path)
+            except botocore.exceptions.ClientError:
+                exist = False
+        if exists_ok or exist is False:
+            client.upload_file(str(source), destination_bucket, destination_path)
+    except ClientError as e:
+        if e.response["Error"]["Code"] == "FileExists":
+            logging.error(f"File {destination_path} already exist")
+        else:
+            raise e
 
 
 class S3Path:
     def __init__(self, client: boto3.client, bucket: str, path: str):
         self.client = client
         self.bucket = bucket
         self.path = path
@@ -82,15 +102,15 @@
         client = source.client
         copy_source = {"Bucket": source.bucket, "Key": source.path}
         client.copy(copy_source, destination.bucket, destination.path)
 
     @classmethod
     def _copy_from_local_to_s3(cls, source: Path, destination: "S3Path"):
         client = destination.client
-        client.upload_file(str(source), destination.bucket, destination.path)
+        upload_file(client, str(source), destination.bucket, destination.path)
 
     @classmethod
     def _copy_from_s3_to_local(cls, source: "S3Path", destination: Path):
         client = source.client
         with open(str(destination), "wb") as f:
             client.download_fileobj(source.bucket, source.path, f)
```

