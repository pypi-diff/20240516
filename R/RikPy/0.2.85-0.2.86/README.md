# Comparing `tmp/RikPy-0.2.85.tar.gz` & `tmp/RikPy-0.2.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RikPy-0.2.85.tar", last modified: Thu May 16 20:17:05 2024, max compression
+gzip compressed data, was "RikPy-0.2.86.tar", last modified: Thu May 16 21:08:07 2024, max compression
```

## Comparing `RikPy-0.2.85.tar` & `RikPy-0.2.86.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 20:17:05.033863 RikPy-0.2.85/
--rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.85/MANIFEST.in
--rw-rw-rw-   0        0        0      176 2024-05-16 20:17:05.031873 RikPy-0.2.85/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 20:17:05.010920 RikPy-0.2.85/RikPy/
--rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.85/RikPy/__init__.py
--rw-rw-rw-   0        0        0     5079 2024-02-27 11:46:00.000000 RikPy-0.2.85/RikPy/commonfunctions.py
--rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.85/RikPy/commongoogle.py
--rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.85/RikPy/commonheroku.py
--rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.85/RikPy/commonleonardo.py
--rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.85/RikPy/commonlogging.py
--rw-rw-rw-   0        0        0     4161 2024-05-16 17:44:18.000000 RikPy-0.2.85/RikPy/commonopenai.py
--rw-rw-rw-   0        0        0     8605 2024-05-16 20:16:37.000000 RikPy-0.2.85/RikPy/commons3.py
--rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.85/RikPy/commonshopify.py
--rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.85/RikPy/customresponse.py
-drwxrwxrwx   0        0        0        0 2024-05-16 20:17:05.029870 RikPy-0.2.85/RikPy.egg-info/
--rw-rw-rw-   0        0        0      176 2024-05-16 20:17:04.000000 RikPy-0.2.85/RikPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2024-05-16 20:17:04.000000 RikPy-0.2.85/RikPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 20:17:04.000000 RikPy-0.2.85/RikPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-16 20:17:04.000000 RikPy-0.2.85/RikPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.85/logfile.txt
--rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.85/readme.md
--rw-rw-rw-   0        0        0      295 2024-05-16 20:17:05.040841 RikPy-0.2.85/setup.cfg
--rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.85/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:08:07.783371 RikPy-0.2.86/
+-rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.86/MANIFEST.in
+-rw-rw-rw-   0        0        0      176 2024-05-16 21:08:07.781377 RikPy-0.2.86/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 21:08:07.762429 RikPy-0.2.86/RikPy/
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.86/RikPy/__init__.py
+-rw-rw-rw-   0        0        0     5079 2024-02-27 11:46:00.000000 RikPy-0.2.86/RikPy/commonfunctions.py
+-rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.86/RikPy/commongoogle.py
+-rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.86/RikPy/commonheroku.py
+-rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.86/RikPy/commonleonardo.py
+-rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.86/RikPy/commonlogging.py
+-rw-rw-rw-   0        0        0     4161 2024-05-16 17:44:18.000000 RikPy-0.2.86/RikPy/commonopenai.py
+-rw-rw-rw-   0        0        0     8854 2024-05-16 21:07:31.000000 RikPy-0.2.86/RikPy/commons3.py
+-rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.86/RikPy/commonshopify.py
+-rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.86/RikPy/customresponse.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:08:07.778384 RikPy-0.2.86/RikPy.egg-info/
+-rw-rw-rw-   0        0        0      176 2024-05-16 21:08:07.000000 RikPy-0.2.86/RikPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2024-05-16 21:08:07.000000 RikPy-0.2.86/RikPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 21:08:07.000000 RikPy-0.2.86/RikPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-16 21:08:07.000000 RikPy-0.2.86/RikPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.86/logfile.txt
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.86/readme.md
+-rw-rw-rw-   0        0        0      295 2024-05-16 21:08:07.789355 RikPy-0.2.86/setup.cfg
+-rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.86/setup.py
```

### Comparing `RikPy-0.2.85/RikPy/commonfunctions.py` & `RikPy-0.2.86/RikPy/commonfunctions.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.85/RikPy/commongoogle.py` & `RikPy-0.2.86/RikPy/commongoogle.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.85/RikPy/commonheroku.py` & `RikPy-0.2.86/RikPy/commonheroku.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.85/RikPy/commonleonardo.py` & `RikPy-0.2.86/RikPy/commonleonardo.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.85/RikPy/commonopenai.py` & `RikPy-0.2.86/RikPy/commonopenai.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.85/RikPy/commons3.py` & `RikPy-0.2.86/RikPy/commons3.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,37 +188,43 @@
         print(f"File '{object_key}' deleted successfully from bucket '{bucket_name}'.")
         return response
     except Exception as e:
         print(f"An error occurred while deleting the file: {str(e)}")
         return None
    
 def s3_upload_file_from_url(file_url="", folder_name="", s3_config_dict=None, bnewname=False, make_public=False):
-    
+       
     if s3_config_dict is None:
         raise ValueError("s3_config_dict is required for this function.")
 
+    print(f"file_url {file_url}")
     # Download the file to a local path
     file_path = download_file_local(file_url)
+    print(f"file_path {file_path}")
+
     if bnewname:
         # Generate a new filename
         new_filename = generate_new_filename(file_path)
+        print(f"new_filename {new_filename}")
 
         # Rename the local file with the new filename
         new_file_path = os.path.join(os.path.dirname(file_path), new_filename)
+        print(f"new_file_path {new_file_path}")
         os.rename(file_path, new_file_path)
 
         # Upload the file with the new filename
         object_key = s3_upload_local_file(file_name=new_file_path, folder_name=folder_name, s3_config_dict=s3_config_dict, make_public=make_public)
-
+        print(f"object_key {object_key}")
         # Delete the local file (both the original and renamed versions)
         delete_local_file(new_file_path)
     else:
         # Upload the file with its original name
         object_key = s3_upload_local_file(file_name=file_path, folder_name=folder_name, s3_config_dict=s3_config_dict)
 
         # Delete the local file
         delete_local_file(file_path)
 
     s3_url = s3_config_dict['S3_URL']
     file_url = s3_url + '/' + object_key
+    print(f"file_url {file_url}")
 
     return file_url
```

### Comparing `RikPy-0.2.85/RikPy/commonshopify.py` & `RikPy-0.2.86/RikPy/commonshopify.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.85/logfile.txt` & `RikPy-0.2.86/logfile.txt`

 * *Files identical despite different names*

