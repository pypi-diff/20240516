# Comparing `tmp/RikPy-0.2.73.tar.gz` & `tmp/RikPy-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RikPy-0.2.73.tar", last modified: Mon May  6 12:48:10 2024, max compression
+gzip compressed data, was "RikPy-0.2.8.tar", last modified: Wed Jan 17 12:45:23 2024, max compression
```

## Comparing `RikPy-0.2.73.tar` & `RikPy-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-06 12:48:10.081004 RikPy-0.2.73/
--rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.73/MANIFEST.in
--rw-rw-rw-   0        0        0      176 2024-05-06 12:48:10.077979 RikPy-0.2.73/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-06 12:48:09.916438 RikPy-0.2.73/RikPy/
--rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.73/RikPy/__init__.py
--rw-rw-rw-   0        0        0     5079 2024-02-27 11:46:00.000000 RikPy-0.2.73/RikPy/commonfunctions.py
--rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.73/RikPy/commongoogle.py
--rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.73/RikPy/commonheroku.py
--rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.73/RikPy/commonleonardo.py
--rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.73/RikPy/commonlogging.py
--rw-rw-rw-   0        0        0     2720 2024-02-10 20:06:13.000000 RikPy-0.2.73/RikPy/commonopenai.py
--rw-rw-rw-   0        0        0     7919 2024-02-07 12:06:25.000000 RikPy-0.2.73/RikPy/commons3.py
--rw-rw-rw-   0        0        0    63270 2024-05-06 12:47:01.000000 RikPy-0.2.73/RikPy/commonshopify.py
--rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.73/RikPy/customresponse.py
-drwxrwxrwx   0        0        0        0 2024-05-06 12:48:10.052894 RikPy-0.2.73/RikPy.egg-info/
--rw-rw-rw-   0        0        0      176 2024-05-06 12:48:07.000000 RikPy-0.2.73/RikPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2024-05-06 12:48:08.000000 RikPy-0.2.73/RikPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-06 12:48:07.000000 RikPy-0.2.73/RikPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-06 12:48:07.000000 RikPy-0.2.73/RikPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.73/logfile.txt
--rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.73/readme.md
--rw-rw-rw-   0        0        0      295 2024-05-06 12:48:10.093557 RikPy-0.2.73/setup.cfg
--rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.73/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-17 12:45:23.334974 RikPy-0.2.8/
+-rw-rw-rw-   0        0        0      186 2024-01-17 12:45:23.330474 RikPy-0.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-01-17 12:45:23.306435 RikPy-0.2.8/RikPy/
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.8/RikPy/__init__.py
+-rw-rw-rw-   0        0        0     1337 2024-01-17 12:14:04.000000 RikPy-0.2.8/RikPy/common.py
+-rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.8/RikPy/commongoogle.py
+-rw-rw-rw-   0        0        0    11660 2024-01-17 12:44:47.000000 RikPy-0.2.8/RikPy/commonheroku.py
+-rw-rw-rw-   0        0        0     1376 2024-01-15 20:18:24.000000 RikPy-0.2.8/RikPy/commonopenai.py
+-rw-rw-rw-   0        0        0     1760 2024-01-17 12:43:35.000000 RikPy-0.2.8/RikPy/test.py
+drwxrwxrwx   0        0        0        0 2024-01-17 12:45:23.326792 RikPy-0.2.8/RikPy.egg-info/
+-rw-rw-rw-   0        0        0      186 2024-01-17 12:45:23.000000 RikPy-0.2.8/RikPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-01-17 12:45:23.000000 RikPy-0.2.8/RikPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-17 12:45:23.000000 RikPy-0.2.8/RikPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-01-17 12:45:23.000000 RikPy-0.2.8/RikPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-01-17 12:45:23.334974 RikPy-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      320 2024-01-17 12:44:57.000000 RikPy-0.2.8/setup.py
```

### Comparing `RikPy-0.2.73/RikPy/commongoogle.py` & `RikPy-0.2.8/RikPy/commongoogle.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.73/RikPy/commonheroku.py` & `RikPy-0.2.8/RikPy/commonheroku.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,24 @@
+from common import download_file_local, delete_local_file
 from dotenv import load_dotenv
 import requests
 import os
 import uuid 
 import boto3
-from botocore.exceptions import NoCredentialsError, ClientError
+from botocore.exceptions import NoCredentialsError
 from urllib.parse import urlparse
 from datetime import datetime
-from .commonfunctions import download_file_local, delete_local_file
-from .commonlogging import configure_logger
-
-logger = configure_logger()
 
 def heroku_environment():
     load_dotenv()  # This loads the environment variables from .env
     CLOUDCUBE_ACCESS_KEY_ID = os.getenv("CLOUDCUBE_ACCESS_KEY_ID")
     CLOUDCUBE_SECRET_ACCESS_KEY = os.getenv("CLOUDCUBE_SECRET_ACCESS_KEY")
     CLOUDCUBE_URL = os.getenv("CLOUDCUBE_URL")
-    HEROKU_API_KEY  = os.getenv("HK_API_KEY")
-    HEROKU_APP_NAME = os.getenv("HK_APP_NAME")
+    HEROKU_API_KEY  = os.getenv("HEROKU_API_KEY")
+    HEROKU_APP_NAME = os.getenv("HEROKU_APP_NAME")
 
     # Extract the bucket name from the CLOUDCUBE_URL
     cube_name = CLOUDCUBE_URL.split('/')[-1]
     cube_public = f"{cube_name}/public/"
     bucket_name = CLOUDCUBE_URL.split('.')[0].split('//')[1]
 
     # Create a dictionary to store the values
@@ -48,15 +45,14 @@
 
     if heroku_config_dict is None:
         raise ValueError("heroku_config_dict is required for this function.")
     
     # Extract relevant values from heroku_config_dict
     CLOUDCUBE_ACCESS_KEY_ID = heroku_config_dict.get("CLOUDCUBE_ACCESS_KEY_ID")
     CLOUDCUBE_SECRET_ACCESS_KEY = heroku_config_dict.get("CLOUDCUBE_SECRET_ACCESS_KEY")
-    CLOUDCUBE_URL = heroku_config_dict.get("CLOUDCUBE_URL")
     CUBE_PUBLIC = heroku_config_dict.get("CUBE_PUBLIC")
     BUCKET_NAME = heroku_config_dict.get("BUCKET_NAME")
 
     # Construct the full S3 object name
     object_name = CUBE_PUBLIC + folder + file_name
 
     try:
@@ -65,23 +61,15 @@
             's3',
             aws_access_key_id=CLOUDCUBE_ACCESS_KEY_ID,
             aws_secret_access_key=CLOUDCUBE_SECRET_ACCESS_KEY
         )
 
         # Upload the file
         s3_client.upload_file(file_name, BUCKET_NAME, object_name)
-
-         # Split the object_name by '/'
-        parts = object_name.split('/')
-
-        # Exclude the first part (wwmx700brb7g) and join the rest with CLOUDCUBE_URL
-        full_url = f"{CLOUDCUBE_URL}/{'/'.join(parts[1:])}"
-        
-        return full_url
-    
+        return f"File {file_name} uploaded to {object_name} in CloudCube."
     except FileNotFoundError:
         return "The file was not found."
     except NoCredentialsError:
         return "Credentials not available."
     except Exception as e:
         return f"An error occurred: {str(e)}"
     
@@ -108,26 +96,25 @@
         new_filename = f"{timestamp}_{shortened_uuid}{file_extension}"
 
         # Rename the local file with the new filename
         new_file_path = os.path.join(os.path.dirname(file_path), new_filename)
         os.rename(file_path, new_file_path)
 
         # Upload the file with the new filename
-        object_name = heroku_upload_file(new_file_path, folder, heroku_config_dict)
+        heroku_upload_file(new_file_path, folder, heroku_config_dict)
 
         # Delete the local file (both the original and renamed versions)
         delete_local_file(new_file_path)
     else:
         # Upload the file with its original name
-        object_name = heroku_upload_file(file_path, folder, heroku_config_dict)
+        heroku_upload_file(file_path, folder, heroku_config_dict)
 
         # Delete the local file
         delete_local_file(file_path)
 
-    return object_name
 
 def heroku_list_files_in_folder(folder_name, heroku_config_dict=None):
     try:
         if heroku_config_dict is None:
             raise ValueError("heroku_config_dict is required for this function.")
 
         # Extract relevant values from heroku_config_dict
@@ -141,28 +128,24 @@
             's3',
             aws_access_key_id=CLOUDCUBE_ACCESS_KEY_ID,
             aws_secret_access_key=CLOUDCUBE_SECRET_ACCESS_KEY
         )
 
         # Set the prefix based on folder_name
         full_prefix = CUBE_PUBLIC
-        full_prefix = ""
-        print(full_prefix)
         if folder_name:
             if not folder_name.endswith('/'):
                 folder_name += '/'
             full_prefix += folder_name
-        print(full_prefix)
 
         # List objects in the specified folder
         response = s3_client.list_objects_v2(Bucket=BUCKET_NAME, Prefix=full_prefix)
-        print(f"response: {response}")
+
         # Check if the bucket has contents
         if 'Contents' in response:
-            print("Contents")
             files = [item['Key'] for item in response['Contents']]
             return files
         else:
             return []
     except ValueError as ve:
         logger.error(f"An error occurred: {ve}")
         return f"ValueError: {str(ve)}"
@@ -203,24 +186,19 @@
     except ClientError as e:
         logger.error(f"An error occurred: {e}")
         return []
     except Exception as e:
         logger.error(f"An error occurred: {e}")
         return []
     
-def heroku_download_files_in_folder(folder_name, heroku_config_dict=None, bdelete=False):
+def heroku_download_files_in_folder(folder_name, bdelete=False):
 
     user_home = os.path.expanduser("~")
     local_download_folder = os.path.join(user_home, 'Downloads', folder_name)
 
-    CLOUDCUBE_ACCESS_KEY_ID = heroku_config_dict.get("CLOUDCUBE_ACCESS_KEY_ID")
-    CLOUDCUBE_SECRET_ACCESS_KEY = heroku_config_dict.get("CLOUDCUBE_SECRET_ACCESS_KEY")
-    cube_public = heroku_config_dict.get("CUBE_PUBLIC")
-    bucket_name = heroku_config_dict.get("BUCKET_NAME")
-
     # Create an S3 client with CloudCube credentials
     s3_client = boto3.client(
         's3',
         aws_access_key_id=CLOUDCUBE_ACCESS_KEY_ID,
         aws_secret_access_key=CLOUDCUBE_SECRET_ACCESS_KEY
     )
 
@@ -244,21 +222,17 @@
         for obj in objects:
             file_key = obj['Key']
             local_file_path = os.path.join(local_download_folder, os.path.basename(file_key))
             response=s3_client.download_file(bucket_name, file_key, local_file_path)
 
             # If bdelete is True, delete the file from the S3 bucket
             if bdelete:
-                print("Deleting file:")
-                print("Bucket Name:", bucket_name)
-                print("File Key:", file_key)
                 try:
-                    heroku_delete_file(file_key=file_key, heroku_config_dict=heroku_config_dict)
-                    #s3_client.delete_object(Bucket=bucket_name, Key=file_key)
-                    #print(f"Deleted file {file_key} from bucket {bucket_name}.")
+                    s3_client.delete_object(Bucket=bucket_name, Key=file_key)
+                    print(f"Deleted file {file_key} from bucket {bucket_name}.")
                 except ClientError as e:
                     print(f"Error deleting file {file_key}: {e}")
 
         return len(objects)
     
     except NoCredentialsError:
         print("Credentials not available.")
```

