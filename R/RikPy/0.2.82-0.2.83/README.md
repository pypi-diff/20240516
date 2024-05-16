# Comparing `tmp/RikPy-0.2.82.tar.gz` & `tmp/RikPy-0.2.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RikPy-0.2.82.tar", last modified: Thu May 16 19:48:09 2024, max compression
+gzip compressed data, was "RikPy-0.2.83.tar", last modified: Thu May 16 19:59:01 2024, max compression
```

## Comparing `RikPy-0.2.82.tar` & `RikPy-0.2.83.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 19:48:09.265894 RikPy-0.2.82/
--rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.82/MANIFEST.in
--rw-rw-rw-   0        0        0      176 2024-05-16 19:48:09.263905 RikPy-0.2.82/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 19:48:09.241796 RikPy-0.2.82/RikPy/
--rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.82/RikPy/__init__.py
--rw-rw-rw-   0        0        0     5079 2024-02-27 11:46:00.000000 RikPy-0.2.82/RikPy/commonfunctions.py
--rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.82/RikPy/commongoogle.py
--rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.82/RikPy/commonheroku.py
--rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.82/RikPy/commonleonardo.py
--rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.82/RikPy/commonlogging.py
--rw-rw-rw-   0        0        0     4161 2024-05-16 17:44:18.000000 RikPy-0.2.82/RikPy/commonopenai.py
--rw-rw-rw-   0        0        0     8855 2024-05-16 19:47:31.000000 RikPy-0.2.82/RikPy/commons3.py
--rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.82/RikPy/commonshopify.py
--rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.82/RikPy/customresponse.py
-drwxrwxrwx   0        0        0        0 2024-05-16 19:48:09.261904 RikPy-0.2.82/RikPy.egg-info/
--rw-rw-rw-   0        0        0      176 2024-05-16 19:48:08.000000 RikPy-0.2.82/RikPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2024-05-16 19:48:09.000000 RikPy-0.2.82/RikPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 19:48:08.000000 RikPy-0.2.82/RikPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-16 19:48:08.000000 RikPy-0.2.82/RikPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.82/logfile.txt
--rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.82/readme.md
--rw-rw-rw-   0        0        0      295 2024-05-16 19:48:09.271402 RikPy-0.2.82/setup.cfg
--rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.82/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 19:59:01.766009 RikPy-0.2.83/
+-rw-rw-rw-   0        0        0      222 2024-02-01 13:41:35.000000 RikPy-0.2.83/MANIFEST.in
+-rw-rw-rw-   0        0        0      176 2024-05-16 19:59:01.763015 RikPy-0.2.83/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 19:59:01.745064 RikPy-0.2.83/RikPy/
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:28:52.000000 RikPy-0.2.83/RikPy/__init__.py
+-rw-rw-rw-   0        0        0     5079 2024-02-27 11:46:00.000000 RikPy-0.2.83/RikPy/commonfunctions.py
+-rw-rw-rw-   0        0        0     2982 2024-01-14 10:37:23.000000 RikPy-0.2.83/RikPy/commongoogle.py
+-rw-rw-rw-   0        0        0    12762 2024-02-02 12:54:14.000000 RikPy-0.2.83/RikPy/commonheroku.py
+-rw-rw-rw-   0        0        0     6672 2024-05-03 09:32:48.000000 RikPy-0.2.83/RikPy/commonleonardo.py
+-rw-rw-rw-   0        0        0      322 2024-02-02 09:53:19.000000 RikPy-0.2.83/RikPy/commonlogging.py
+-rw-rw-rw-   0        0        0     4161 2024-05-16 17:44:18.000000 RikPy-0.2.83/RikPy/commonopenai.py
+-rw-rw-rw-   0        0        0     9086 2024-05-16 19:58:37.000000 RikPy-0.2.83/RikPy/commons3.py
+-rw-rw-rw-   0        0        0    63072 2024-05-06 15:05:51.000000 RikPy-0.2.83/RikPy/commonshopify.py
+-rw-rw-rw-   0        0        0      302 2024-02-10 20:05:58.000000 RikPy-0.2.83/RikPy/customresponse.py
+drwxrwxrwx   0        0        0        0 2024-05-16 19:59:01.761022 RikPy-0.2.83/RikPy.egg-info/
+-rw-rw-rw-   0        0        0      176 2024-05-16 19:59:01.000000 RikPy-0.2.83/RikPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2024-05-16 19:59:01.000000 RikPy-0.2.83/RikPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 19:59:01.000000 RikPy-0.2.83/RikPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-16 19:59:01.000000 RikPy-0.2.83/RikPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2643 2024-02-28 23:25:52.000000 RikPy-0.2.83/logfile.txt
+-rw-rw-rw-   0        0        0        0 2024-01-13 10:22:02.000000 RikPy-0.2.83/readme.md
+-rw-rw-rw-   0        0        0      295 2024-05-16 19:59:01.771992 RikPy-0.2.83/setup.cfg
+-rw-rw-rw-   0        0        0       56 2024-01-30 10:46:18.000000 RikPy-0.2.83/setup.py
```

### Comparing `RikPy-0.2.82/RikPy/commonfunctions.py` & `RikPy-0.2.83/RikPy/commonfunctions.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.82/RikPy/commongoogle.py` & `RikPy-0.2.83/RikPy/commongoogle.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.82/RikPy/commonheroku.py` & `RikPy-0.2.83/RikPy/commonheroku.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.82/RikPy/commonleonardo.py` & `RikPy-0.2.83/RikPy/commonleonardo.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.82/RikPy/commonopenai.py` & `RikPy-0.2.83/RikPy/commonopenai.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.82/RikPy/commons3.py` & `RikPy-0.2.83/RikPy/commons3.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,17 +147,21 @@
     if folder_name is None:
         folder_name = ''
     elif not folder_name.endswith('/'):
         folder_name += '/'
 
     if bnewname:
         # Generate a new name for the file
-        file_name = generate_new_filename(file_name)
+        new_file_name = generate_new_filename(file_name)
+        new_file_path = os.path.join(os.path.dirname(file_name), new_file_name)
+        os.rename(file_name, new_file_path)
+        file_name = new_file_path
 
-    object_key = f"{folder_name}{file_name}"
+    # object_key = f"{folder_name}{file_name}"
+    object_key = f"{folder_name}{os.path.basename(file_name)}"
 
     try:
         response = s3.upload_file(file_name, bucket_name, object_key)
 
         # Set the ACL to public-read if specified
         if make_public:
             s3.put_object_acl(Bucket=bucket_name, Key=object_key, ACL='public-read')
```

### Comparing `RikPy-0.2.82/RikPy/commonshopify.py` & `RikPy-0.2.83/RikPy/commonshopify.py`

 * *Files identical despite different names*

### Comparing `RikPy-0.2.82/logfile.txt` & `RikPy-0.2.83/logfile.txt`

 * *Files identical despite different names*

