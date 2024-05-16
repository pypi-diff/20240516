# Comparing `tmp/RikPy-0.2.86.tar.gz` & `tmp/RikPy-0.2.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RikPy-0.2.86.tar", last modified: Thu May 16 21:08:07 2024, max compression
+gzip compressed data, was "RikPy-0.2.87.tar", last modified: Thu May 16 21:15:47 2024, max compression
```

## Comparing `RikPy-0.2.86.tar` & `RikPy-0.2.87.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 21:08:07.783371 RikPy-0.2.86/
--rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.86/MANIFEST.in
--rw-rw-rw-   0        0        0      176 2024-05-16 21:08:07.781377 RikPy-0.2.86/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 21:08:07.762429 RikPy-0.2.86/RikPy/
--rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.86/RikPy/__init__.py
--rw-rw-rw-   0        0        0     5079 2024-02-27 11:46:00.000000 RikPy-0.2.86/RikPy/commonfunctions.py
--rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.86/RikPy/commongoogle.py
--rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.86/RikPy/commonheroku.py
--rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.86/RikPy/commonleonardo.py
--rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.86/RikPy/commonlogging.py
--rw-rw-rw-   0        0        0     4161 2024-05-16 17:44:18.000000 RikPy-0.2.86/RikPy/commonopenai.py
--rw-rw-rw-   0        0        0     8854 2024-05-16 21:07:31.000000 RikPy-0.2.86/RikPy/commons3.py
--rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.86/RikPy/commonshopify.py
--rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.86/RikPy/customresponse.py
-drwxrwxrwx   0        0        0        0 2024-05-16 21:08:07.778384 RikPy-0.2.86/RikPy.egg-info/
--rw-rw-rw-   0        0        0      176 2024-05-16 21:08:07.000000 RikPy-0.2.86/RikPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2024-05-16 21:08:07.000000 RikPy-0.2.86/RikPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 21:08:07.000000 RikPy-0.2.86/RikPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-16 21:08:07.000000 RikPy-0.2.86/RikPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.86/logfile.txt
--rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.86/readme.md
--rw-rw-rw-   0        0        0      295 2024-05-16 21:08:07.789355 RikPy-0.2.86/setup.cfg
--rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.86/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:15:47.576833 RikPy-0.2.87/
+-rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.87/MANIFEST.in
+-rw-rw-rw-   0        0        0      176 2024-05-16 21:15:47.569208 RikPy-0.2.87/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 21:15:47.552551 RikPy-0.2.87/RikPy/
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.87/RikPy/__init__.py
+-rw-rw-rw-   0        0        0     5429 2024-05-16 21:13:28.000000 RikPy-0.2.87/RikPy/commonfunctions.py
+-rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.87/RikPy/commongoogle.py
+-rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.87/RikPy/commonheroku.py
+-rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.87/RikPy/commonleonardo.py
+-rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.87/RikPy/commonlogging.py
+-rw-rw-rw-   0        0        0     4161 2024-05-16 17:44:18.000000 RikPy-0.2.87/RikPy/commonopenai.py
+-rw-rw-rw-   0        0        0     8978 2024-05-16 21:15:17.000000 RikPy-0.2.87/RikPy/commons3.py
+-rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.87/RikPy/commonshopify.py
+-rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.87/RikPy/customresponse.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:15:47.569208 RikPy-0.2.87/RikPy.egg-info/
+-rw-rw-rw-   0        0        0      176 2024-05-16 21:15:47.000000 RikPy-0.2.87/RikPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2024-05-16 21:15:47.000000 RikPy-0.2.87/RikPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 21:15:47.000000 RikPy-0.2.87/RikPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-16 21:15:47.000000 RikPy-0.2.87/RikPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.87/logfile.txt
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.87/readme.md
+-rw-rw-rw-   0        0        0      295 2024-05-16 21:15:47.577828 RikPy-0.2.87/setup.cfg
+-rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.87/setup.py
```

### Comparing `RikPy-0.2.86/RikPy/commonfunctions.py` & `RikPy-0.2.87/RikPy/commonfunctions.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,23 @@
     with requests.get(url, stream=True) as r:
         r.raise_for_status()
         with open(local_filename, 'wb') as f:
             for chunk in r.iter_content(chunk_size=8192): 
                 f.write(chunk)
     return local_filename
 
+def download_file_local_with_query_parameters(file_url):
+    response = requests.get(file_url)
+    # Extract the path from the URL without query parameters
+    parsed_url = urlparse(file_url)
+    file_name = os.path.basename(parsed_url.path)
+    with open(file_name, 'wb') as file:
+        file.write(response.content)
+    return file_name
+
 def delete_local_file(file_name):
     try:
         # Check if file exists
         if os.path.exists(file_name):
             # Delete the file
             os.remove(file_name)
             return f"File '{file_name}' has been deleted."
```

### Comparing `RikPy-0.2.86/RikPy/commongoogle.py` & `RikPy-0.2.87/RikPy/commongoogle.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.86/RikPy/commonheroku.py` & `RikPy-0.2.87/RikPy/commonheroku.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.86/RikPy/commonleonardo.py` & `RikPy-0.2.87/RikPy/commonleonardo.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.86/RikPy/commonopenai.py` & `RikPy-0.2.87/RikPy/commonopenai.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.86/RikPy/commons3.py` & `RikPy-0.2.87/RikPy/commons3.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import uuid 
 import boto3
 from botocore.exceptions import NoCredentialsError, ClientError
 from urllib.parse import urlparse
 from dotenv import load_dotenv
 from datetime import datetime
-from .commonfunctions import download_file_local, delete_local_file
+from .commonfunctions import download_file_local, delete_local_file, download_file_local_with_query_parameters
 
 #### AUX FUNCTIONS
 def generate_new_filename(original_filename):
     """
     Generate a new filename with a timestamp and shortened UUID.
     """
     # Extract the file extension from the original filename
@@ -194,15 +194,17 @@
 def s3_upload_file_from_url(file_url="", folder_name="", s3_config_dict=None, bnewname=False, make_public=False):
        
     if s3_config_dict is None:
         raise ValueError("s3_config_dict is required for this function.")
 
     print(f"file_url {file_url}")
     # Download the file to a local path
-    file_path = download_file_local(file_url)
+    #file_path = download_file_local(file_url)
+    file_path = download_file_local_with_query_parameters(file_url=file_url)
+
     print(f"file_path {file_path}")
 
     if bnewname:
         # Generate a new filename
         new_filename = generate_new_filename(file_path)
         print(f"new_filename {new_filename}")
```

### Comparing `RikPy-0.2.86/RikPy/commonshopify.py` & `RikPy-0.2.87/RikPy/commonshopify.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.86/logfile.txt` & `RikPy-0.2.87/logfile.txt`

 * *Files identical despite different names*

