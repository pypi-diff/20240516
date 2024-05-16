# Comparing `tmp/RikPy-0.2.81.tar.gz` & `tmp/RikPy-0.2.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RikPy-0.2.81.tar", last modified: Thu May 16 17:45:06 2024, max compression
+gzip compressed data, was "RikPy-0.2.82.tar", last modified: Thu May 16 19:48:09 2024, max compression
```

## Comparing `RikPy-0.2.81.tar` & `RikPy-0.2.82.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 17:45:05.998157 RikPy-0.2.81/
--rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.81/MANIFEST.in
--rw-rw-rw-   0        0        0      176 2024-05-16 17:45:05.995164 RikPy-0.2.81/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 17:45:05.974221 RikPy-0.2.81/RikPy/
--rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.81/RikPy/__init__.py
--rw-rw-rw-   0        0        0     5079 2024-02-27 11:46:00.000000 RikPy-0.2.81/RikPy/commonfunctions.py
--rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.81/RikPy/commongoogle.py
--rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.81/RikPy/commonheroku.py
--rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.81/RikPy/commonleonardo.py
--rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.81/RikPy/commonlogging.py
--rw-rw-rw-   0        0        0     4161 2024-05-16 17:44:18.000000 RikPy-0.2.81/RikPy/commonopenai.py
--rw-rw-rw-   0        0        0     7919 2024-02-07 12:06:25.000000 RikPy-0.2.81/RikPy/commons3.py
--rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.81/RikPy/commonshopify.py
--rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.81/RikPy/customresponse.py
-drwxrwxrwx   0        0        0        0 2024-05-16 17:45:05.991174 RikPy-0.2.81/RikPy.egg-info/
--rw-rw-rw-   0        0        0      176 2024-05-16 17:45:05.000000 RikPy-0.2.81/RikPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2024-05-16 17:45:05.000000 RikPy-0.2.81/RikPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 17:45:05.000000 RikPy-0.2.81/RikPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-16 17:45:05.000000 RikPy-0.2.81/RikPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.81/logfile.txt
--rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.81/readme.md
--rw-rw-rw-   0        0        0      295 2024-05-16 17:45:06.004140 RikPy-0.2.81/setup.cfg
--rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.81/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 19:48:09.265894 RikPy-0.2.82/
+-rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.82/MANIFEST.in
+-rw-rw-rw-   0        0        0      176 2024-05-16 19:48:09.263905 RikPy-0.2.82/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 19:48:09.241796 RikPy-0.2.82/RikPy/
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.82/RikPy/__init__.py
+-rw-rw-rw-   0        0        0     5079 2024-02-27 11:46:00.000000 RikPy-0.2.82/RikPy/commonfunctions.py
+-rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.82/RikPy/commongoogle.py
+-rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.82/RikPy/commonheroku.py
+-rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.82/RikPy/commonleonardo.py
+-rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.82/RikPy/commonlogging.py
+-rw-rw-rw-   0        0        0     4161 2024-05-16 17:44:18.000000 RikPy-0.2.82/RikPy/commonopenai.py
+-rw-rw-rw-   0        0        0     8855 2024-05-16 19:47:31.000000 RikPy-0.2.82/RikPy/commons3.py
+-rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.82/RikPy/commonshopify.py
+-rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.82/RikPy/customresponse.py
+drwxrwxrwx   0        0        0        0 2024-05-16 19:48:09.261904 RikPy-0.2.82/RikPy.egg-info/
+-rw-rw-rw-   0        0        0      176 2024-05-16 19:48:08.000000 RikPy-0.2.82/RikPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2024-05-16 19:48:09.000000 RikPy-0.2.82/RikPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 19:48:08.000000 RikPy-0.2.82/RikPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-16 19:48:08.000000 RikPy-0.2.82/RikPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.82/logfile.txt
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.82/readme.md
+-rw-rw-rw-   0        0        0      295 2024-05-16 19:48:09.271402 RikPy-0.2.82/setup.cfg
+-rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.82/setup.py
```

### Comparing `RikPy-0.2.81/RikPy/commonfunctions.py` & `RikPy-0.2.82/RikPy/commonfunctions.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.81/RikPy/commongoogle.py` & `RikPy-0.2.82/RikPy/commongoogle.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.81/RikPy/commonheroku.py` & `RikPy-0.2.82/RikPy/commonheroku.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.81/RikPy/commonleonardo.py` & `RikPy-0.2.82/RikPy/commonleonardo.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.81/RikPy/commonopenai.py` & `RikPy-0.2.82/RikPy/commonopenai.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.81/RikPy/commons3.py` & `RikPy-0.2.82/RikPy/commons3.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,39 @@
 import boto3
 from botocore.exceptions import NoCredentialsError, ClientError
 from urllib.parse import urlparse
 from dotenv import load_dotenv
 from datetime import datetime
 from .commonfunctions import download_file_local, delete_local_file
 
+#### AUX FUNCTIONS
+def generate_new_filename(original_filename):
+    """
+    Generate a new filename with a timestamp and shortened UUID.
+    """
+    # Extract the file extension from the original filename
+    file_extension = os.path.splitext(original_filename)[1]
+
+    # Generate a timestamp in the format YYYYMMDDHHMMSS
+    timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
+
+    # Generate a UUID
+    generated_uuid = uuid.uuid4()
+
+    # Convert the UUID to a hexadecimal string and truncate it to the desired length
+    shortened_uuid = str(generated_uuid.hex)[:8]  # Example: Truncate to 8 characters
+
+    # Create a new filename using the shortened UUID
+    new_filename = f"{timestamp}_{shortened_uuid}{file_extension}"
+
+    return new_filename
+
+
+#### MAIN FUNCTIONS
+
 def s3_environment():
 
     load_dotenv()  # This loads the environment variables from .env
     S3_ACCESS_KEY_ID = os.getenv("S3_ACCESS_KEY_ID")
     S3_SECRET_ACCESS_KEY = os.getenv("S3_SECRET_ACCESS_KEY")
     # S3_URL = os.getenv("S3_URL", 'https://eu-central-1.s3.amazonaws.com/getaiir')
     S3_URL = os.getenv("S3_URL")#, 'https://getaiir.s3.eu-central-1.amazonaws.com')
@@ -91,15 +116,15 @@
             destination_path = os.path.join(destination_folder, filename)
             s3.download_file(bucket_name, key, destination_path)
             print(f"Downloaded {key} to {destination_path}")
     else:
         print("No objects found in the bucket.")
     return
 
-def s3_upload_local_file(file_name="", folder_name=None, s3_config_dict=None, make_public=False):
+def s3_upload_local_file(file_name="", folder_name=None, s3_config_dict=None, bnewname=False, make_public=False):
     '''
     Uploads from file name to the folder_name
     file_name is local, must not be a file_path
     
     '''
 
     if s3_config_dict is None:
@@ -120,14 +145,18 @@
 
     # Ensure folder ends with a '/' if it's not empty
     if folder_name is None:
         folder_name = ''
     elif not folder_name.endswith('/'):
         folder_name += '/'
 
+    if bnewname:
+        # Generate a new name for the file
+        file_name = generate_new_filename(file_name)
+
     object_key = f"{folder_name}{file_name}"
 
     try:
         response = s3.upload_file(file_name, bucket_name, object_key)
 
         # Set the ACL to public-read if specified
         if make_public:
```

### Comparing `RikPy-0.2.81/RikPy/commonshopify.py` & `RikPy-0.2.82/RikPy/commonshopify.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.81/logfile.txt` & `RikPy-0.2.82/logfile.txt`

 * *Files identical despite different names*

