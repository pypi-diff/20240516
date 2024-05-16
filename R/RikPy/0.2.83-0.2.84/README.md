# Comparing `tmp/RikPy-0.2.83.tar.gz` & `tmp/RikPy-0.2.84.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RikPy-0.2.83.tar", last modified: Thu May 16 19:59:01 2024, max compression
+gzip compressed data, was "RikPy-0.2.84.tar", last modified: Thu May 16 20:05:06 2024, max compression
```

## Comparing `RikPy-0.2.83.tar` & `RikPy-0.2.84.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 19:59:01.766009 RikPy-0.2.83/
--rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.83/MANIFEST.in
--rw-rw-rw-   0        0        0      176 2024-05-16 19:59:01.763015 RikPy-0.2.83/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 19:59:01.745064 RikPy-0.2.83/RikPy/
--rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.83/RikPy/__init__.py
--rw-rw-rw-   0        0        0     5079 2024-02-27 11:46:00.000000 RikPy-0.2.83/RikPy/commonfunctions.py
--rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.83/RikPy/commongoogle.py
--rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.83/RikPy/commonheroku.py
--rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.83/RikPy/commonleonardo.py
--rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.83/RikPy/commonlogging.py
--rw-rw-rw-   0        0        0     4161 2024-05-16 17:44:18.000000 RikPy-0.2.83/RikPy/commonopenai.py
--rw-rw-rw-   0        0        0     9086 2024-05-16 19:58:37.000000 RikPy-0.2.83/RikPy/commons3.py
--rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.83/RikPy/commonshopify.py
--rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.83/RikPy/customresponse.py
-drwxrwxrwx   0        0        0        0 2024-05-16 19:59:01.761022 RikPy-0.2.83/RikPy.egg-info/
--rw-rw-rw-   0        0        0      176 2024-05-16 19:59:01.000000 RikPy-0.2.83/RikPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2024-05-16 19:59:01.000000 RikPy-0.2.83/RikPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 19:59:01.000000 RikPy-0.2.83/RikPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-16 19:59:01.000000 RikPy-0.2.83/RikPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.83/logfile.txt
--rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.83/readme.md
--rw-rw-rw-   0        0        0      295 2024-05-16 19:59:01.771992 RikPy-0.2.83/setup.cfg
--rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.83/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:05:06.694853 RikPy-0.2.84/
+-rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.84/MANIFEST.in
+-rw-rw-rw-   0        0        0      176 2024-05-16 20:05:06.693856 RikPy-0.2.84/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 20:05:06.674909 RikPy-0.2.84/RikPy/
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.84/RikPy/__init__.py
+-rw-rw-rw-   0        0        0     5079 2024-02-27 11:46:00.000000 RikPy-0.2.84/RikPy/commonfunctions.py
+-rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.84/RikPy/commongoogle.py
+-rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.84/RikPy/commonheroku.py
+-rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.84/RikPy/commonleonardo.py
+-rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.84/RikPy/commonlogging.py
+-rw-rw-rw-   0        0        0     4161 2024-05-16 17:44:18.000000 RikPy-0.2.84/RikPy/commonopenai.py
+-rw-rw-rw-   0        0        0     8496 2024-05-16 20:04:31.000000 RikPy-0.2.84/RikPy/commons3.py
+-rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.84/RikPy/commonshopify.py
+-rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.84/RikPy/customresponse.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:05:06.690864 RikPy-0.2.84/RikPy.egg-info/
+-rw-rw-rw-   0        0        0      176 2024-05-16 20:05:06.000000 RikPy-0.2.84/RikPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2024-05-16 20:05:06.000000 RikPy-0.2.84/RikPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 20:05:06.000000 RikPy-0.2.84/RikPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-16 20:05:06.000000 RikPy-0.2.84/RikPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.84/logfile.txt
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.84/readme.md
+-rw-rw-rw-   0        0        0      295 2024-05-16 20:05:06.702831 RikPy-0.2.84/setup.cfg
+-rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.84/setup.py
```

### Comparing `RikPy-0.2.83/RikPy/commonfunctions.py` & `RikPy-0.2.84/RikPy/commonfunctions.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.83/RikPy/commongoogle.py` & `RikPy-0.2.84/RikPy/commongoogle.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.83/RikPy/commonheroku.py` & `RikPy-0.2.84/RikPy/commonheroku.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.83/RikPy/commonleonardo.py` & `RikPy-0.2.84/RikPy/commonleonardo.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.83/RikPy/commonopenai.py` & `RikPy-0.2.84/RikPy/commonopenai.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.83/RikPy/commons3.py` & `RikPy-0.2.84/RikPy/commons3.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     shortened_uuid = str(generated_uuid.hex)[:8]  # Example: Truncate to 8 characters
 
     # Create a new filename using the shortened UUID
     new_filename = f"{timestamp}_{shortened_uuid}{file_extension}"
 
     return new_filename
 
-
 #### MAIN FUNCTIONS
 
 def s3_environment():
 
     load_dotenv()  # This loads the environment variables from .env
     S3_ACCESS_KEY_ID = os.getenv("S3_ACCESS_KEY_ID")
     S3_SECRET_ACCESS_KEY = os.getenv("S3_SECRET_ACCESS_KEY")
@@ -193,29 +192,16 @@
         return None
    
 def s3_upload_file_from_url(file_url="", folder_name="", s3_config_dict=None, bnewname=False, make_public=False):
     
     # Download the file to a local path
     file_path = download_file_local(file_url)
     if bnewname:
-        # Extract the file extension from the URL
-        parsed_url = urlparse(file_url)
-        file_extension = os.path.splitext(os.path.basename(parsed_url.path))[1]
-
-        # Generate a timestamp in the format YYYYMMDDHHMMSS
-        timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
-
-        # Generate a UUID
-        generated_uuid = uuid.uuid4()
-
-        # Convert the UUID to a hexadecimal string and truncate it to the desired length
-        shortened_uuid = str(generated_uuid.hex)[:8]  # Example: Truncate to 8 characters
-
-        # Create a new filename using the shortened UUID
-        new_filename = f"{timestamp}_{shortened_uuid}{file_extension}"
+        # Generate a new filename
+        new_filename = generate_new_filename(file_path)
 
         # Rename the local file with the new filename
         new_file_path = os.path.join(os.path.dirname(file_path), new_filename)
         os.rename(file_path, new_file_path)
 
         # Upload the file with the new filename
         object_key = s3_upload_local_file(file_name=new_file_path, folder_name=folder_name, s3_config_dict=s3_config_dict, make_public=make_public)
```

### Comparing `RikPy-0.2.83/RikPy/commonshopify.py` & `RikPy-0.2.84/RikPy/commonshopify.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.83/logfile.txt` & `RikPy-0.2.84/logfile.txt`

 * *Files identical despite different names*

