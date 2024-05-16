# Comparing `tmp/RikPy-0.2.87.tar.gz` & `tmp/RikPy-0.2.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RikPy-0.2.87.tar", last modified: Thu May 16 21:15:47 2024, max compression
+gzip compressed data, was "RikPy-0.2.88.tar", last modified: Thu May 16 21:26:55 2024, max compression
```

## Comparing `RikPy-0.2.87.tar` & `RikPy-0.2.88.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 21:15:47.576833 RikPy-0.2.87/
--rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.87/MANIFEST.in
--rw-rw-rw-   0        0        0      176 2024-05-16 21:15:47.569208 RikPy-0.2.87/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 21:15:47.552551 RikPy-0.2.87/RikPy/
--rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.87/RikPy/__init__.py
--rw-rw-rw-   0        0        0     5429 2024-05-16 21:13:28.000000 RikPy-0.2.87/RikPy/commonfunctions.py
--rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.87/RikPy/commongoogle.py
--rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.87/RikPy/commonheroku.py
--rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.87/RikPy/commonleonardo.py
--rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.87/RikPy/commonlogging.py
--rw-rw-rw-   0        0        0     4161 2024-05-16 17:44:18.000000 RikPy-0.2.87/RikPy/commonopenai.py
--rw-rw-rw-   0        0        0     8978 2024-05-16 21:15:17.000000 RikPy-0.2.87/RikPy/commons3.py
--rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.87/RikPy/commonshopify.py
--rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.87/RikPy/customresponse.py
-drwxrwxrwx   0        0        0        0 2024-05-16 21:15:47.569208 RikPy-0.2.87/RikPy.egg-info/
--rw-rw-rw-   0        0        0      176 2024-05-16 21:15:47.000000 RikPy-0.2.87/RikPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2024-05-16 21:15:47.000000 RikPy-0.2.87/RikPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 21:15:47.000000 RikPy-0.2.87/RikPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-16 21:15:47.000000 RikPy-0.2.87/RikPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.87/logfile.txt
--rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.87/readme.md
--rw-rw-rw-   0        0        0      295 2024-05-16 21:15:47.577828 RikPy-0.2.87/setup.cfg
--rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.87/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:26:55.962769 RikPy-0.2.88/
+-rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.88/MANIFEST.in
+-rw-rw-rw-   0        0        0      176 2024-05-16 21:26:55.962769 RikPy-0.2.88/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 21:26:55.943771 RikPy-0.2.88/RikPy/
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.88/RikPy/__init__.py
+-rw-rw-rw-   0        0        0     5429 2024-05-16 21:13:28.000000 RikPy-0.2.88/RikPy/commonfunctions.py
+-rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.88/RikPy/commongoogle.py
+-rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.88/RikPy/commonheroku.py
+-rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.88/RikPy/commonleonardo.py
+-rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.88/RikPy/commonlogging.py
+-rw-rw-rw-   0        0        0     4161 2024-05-16 17:44:18.000000 RikPy-0.2.88/RikPy/commonopenai.py
+-rw-rw-rw-   0        0        0     9123 2024-05-16 21:26:29.000000 RikPy-0.2.88/RikPy/commons3.py
+-rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.88/RikPy/commonshopify.py
+-rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.88/RikPy/customresponse.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:26:55.960031 RikPy-0.2.88/RikPy.egg-info/
+-rw-rw-rw-   0        0        0      176 2024-05-16 21:26:55.000000 RikPy-0.2.88/RikPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2024-05-16 21:26:55.000000 RikPy-0.2.88/RikPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 21:26:55.000000 RikPy-0.2.88/RikPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-16 21:26:55.000000 RikPy-0.2.88/RikPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.88/logfile.txt
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.88/readme.md
+-rw-rw-rw-   0        0        0      295 2024-05-16 21:26:55.969037 RikPy-0.2.88/setup.cfg
+-rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.88/setup.py
```

### Comparing `RikPy-0.2.87/RikPy/commonfunctions.py` & `RikPy-0.2.88/RikPy/commonfunctions.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.87/RikPy/commongoogle.py` & `RikPy-0.2.88/RikPy/commongoogle.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.87/RikPy/commonheroku.py` & `RikPy-0.2.88/RikPy/commonheroku.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.87/RikPy/commonleonardo.py` & `RikPy-0.2.88/RikPy/commonleonardo.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.87/RikPy/commonopenai.py` & `RikPy-0.2.88/RikPy/commonopenai.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.87/RikPy/commons3.py` & `RikPy-0.2.88/RikPy/commons3.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,23 +153,28 @@
         new_file_name = generate_new_filename(file_name)
         new_file_path = os.path.join(os.path.dirname(file_name), new_file_name)
         os.rename(file_name, new_file_path)
         file_name = new_file_path
 
     # object_key = f"{folder_name}{file_name}"
     object_key = f"{folder_name}{os.path.basename(file_name)}"
+    
+    s3_url = s3_config_dict['S3_URL']
+    file_url = s3_url + '/' + object_key
+    print(f"file_url {file_url}")
 
     try:
         response = s3.upload_file(file_name, bucket_name, object_key)
 
         # Set the ACL to public-read if specified
         if make_public:
             s3.put_object_acl(Bucket=bucket_name, Key=object_key, ACL='public-read')
 
         print(f"File '{object_key}' uploaded successfully to bucket '{bucket_name}'.")
+        return s3_url
         return object_key
     except Exception as e:
         print(f"An error occurred while uploading the file: {str(e)}")
         return None
     
 def s3_delete_file(object_key, s3_config_dict):
     access_key = s3_config_dict['S3_ACCESS_KEY_ID']
```

### Comparing `RikPy-0.2.87/RikPy/commonshopify.py` & `RikPy-0.2.88/RikPy/commonshopify.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.87/logfile.txt` & `RikPy-0.2.88/logfile.txt`

 * *Files identical despite different names*

