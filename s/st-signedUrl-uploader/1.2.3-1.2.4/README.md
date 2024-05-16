# Comparing `tmp/st_signedurl_uploader-1.2.3.tar.gz` & `tmp/st_signedurl_uploader-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_signedurl_uploader-1.2.3.tar", last modified: Mon May 13 12:11:38 2024, max compression
+gzip compressed data, was "st_signedurl_uploader-1.2.4.tar", last modified: Thu May 16 08:00:37 2024, max compression
```

## Comparing `st_signedurl_uploader-1.2.3.tar` & `st_signedurl_uploader-1.2.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 12:11:38.804297 st_signedurl_uploader-1.2.3/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1063 2024-04-10 04:21:46.000000 st_signedurl_uploader-1.2.3/LICENSE
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)       57 2024-05-13 09:49:00.000000 st_signedurl_uploader-1.2.3/MANIFEST.in
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5021 2024-05-13 12:11:38.803773 st_signedurl_uploader-1.2.3/PKG-INFO
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     4351 2024-05-13 09:48:53.000000 st_signedurl_uploader-1.2.3/README.md
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)       38 2024-05-13 12:11:38.804378 st_signedurl_uploader-1.2.3/setup.cfg
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      927 2024-05-13 12:11:06.000000 st_signedurl_uploader-1.2.3/setup.py
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 12:11:38.798357 st_signedurl_uploader-1.2.3/st_signedUrl_uploader/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     2612 2024-05-13 08:18:08.000000 st_signedurl_uploader-1.2.3/st_signedUrl_uploader/__init__.py
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 12:11:38.797062 st_signedurl_uploader-1.2.3/st_signedUrl_uploader/frontend/
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 12:11:38.800328 st_signedurl_uploader-1.2.3/st_signedUrl_uploader/frontend/build/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      221 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.3/st_signedUrl_uploader/frontend/build/asset-manifest.json
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)   197413 2024-05-11 08:08:11.000000 st_signedurl_uploader-1.2.3/st_signedUrl_uploader/frontend/build/bootstrap.min.css
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      492 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.3/st_signedUrl_uploader/frontend/build/index.html
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 12:11:38.797317 st_signedurl_uploader-1.2.3/st_signedUrl_uploader/frontend/build/static/
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 12:11:38.801211 st_signedurl_uploader-1.2.3/st_signedUrl_uploader/frontend/build/static/js/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)   317963 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.3/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1293 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.3/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)  1248762 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.3/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.map
-drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-13 12:11:38.802931 st_signedurl_uploader-1.2.3/st_signedUrl_uploader.egg-info/
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5021 2024-05-13 12:11:38.000000 st_signedurl_uploader-1.2.3/st_signedUrl_uploader.egg-info/PKG-INFO
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      664 2024-05-13 12:11:38.000000 st_signedurl_uploader-1.2.3/st_signedUrl_uploader.egg-info/SOURCES.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)        1 2024-05-13 12:11:38.000000 st_signedurl_uploader-1.2.3/st_signedUrl_uploader.egg-info/dependency_links.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)      140 2024-05-13 12:11:38.000000 st_signedurl_uploader-1.2.3/st_signedUrl_uploader.egg-info/requires.txt
--rw-r--r--   0 meryam.assermouh   (502) staff       (20)       22 2024-05-13 12:11:38.000000 st_signedurl_uploader-1.2.3/st_signedUrl_uploader.egg-info/top_level.txt
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-16 08:00:37.971655 st_signedurl_uploader-1.2.4/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1063 2024-04-10 04:21:46.000000 st_signedurl_uploader-1.2.4/LICENSE
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)       57 2024-05-13 09:49:00.000000 st_signedurl_uploader-1.2.4/MANIFEST.in
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5156 2024-05-16 08:00:37.971362 st_signedurl_uploader-1.2.4/PKG-INFO
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     4486 2024-05-16 07:58:26.000000 st_signedurl_uploader-1.2.4/README.md
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)       38 2024-05-16 08:00:37.971731 st_signedurl_uploader-1.2.4/setup.cfg
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      927 2024-05-16 07:58:11.000000 st_signedurl_uploader-1.2.4/setup.py
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-16 08:00:37.961803 st_signedurl_uploader-1.2.4/st_signedUrl_uploader/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     2620 2024-05-16 07:58:23.000000 st_signedurl_uploader-1.2.4/st_signedUrl_uploader/__init__.py
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-16 08:00:37.960255 st_signedurl_uploader-1.2.4/st_signedUrl_uploader/frontend/
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-16 08:00:37.964614 st_signedurl_uploader-1.2.4/st_signedUrl_uploader/frontend/build/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      221 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.4/st_signedUrl_uploader/frontend/build/asset-manifest.json
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)   197413 2024-05-11 08:08:11.000000 st_signedurl_uploader-1.2.4/st_signedUrl_uploader/frontend/build/bootstrap.min.css
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      492 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.4/st_signedUrl_uploader/frontend/build/index.html
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-16 08:00:37.960452 st_signedurl_uploader-1.2.4/st_signedUrl_uploader/frontend/build/static/
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-16 08:00:37.967218 st_signedurl_uploader-1.2.4/st_signedUrl_uploader/frontend/build/static/js/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)   317963 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.4/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     1293 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.4/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)  1248762 2024-05-08 09:36:43.000000 st_signedurl_uploader-1.2.4/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.map
+drwxr-xr-x   0 meryam.assermouh   (502) staff       (20)        0 2024-05-16 08:00:37.970498 st_signedurl_uploader-1.2.4/st_signedUrl_uploader.egg-info/
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)     5156 2024-05-16 08:00:37.000000 st_signedurl_uploader-1.2.4/st_signedUrl_uploader.egg-info/PKG-INFO
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      664 2024-05-16 08:00:37.000000 st_signedurl_uploader-1.2.4/st_signedUrl_uploader.egg-info/SOURCES.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)        1 2024-05-16 08:00:37.000000 st_signedurl_uploader-1.2.4/st_signedUrl_uploader.egg-info/dependency_links.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)      140 2024-05-16 08:00:37.000000 st_signedurl_uploader-1.2.4/st_signedUrl_uploader.egg-info/requires.txt
+-rw-r--r--   0 meryam.assermouh   (502) staff       (20)       22 2024-05-16 08:00:37.000000 st_signedurl_uploader-1.2.4/st_signedUrl_uploader.egg-info/top_level.txt
```

### Comparing `st_signedurl_uploader-1.2.3/LICENSE` & `st_signedurl_uploader-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.3/PKG-INFO` & `st_signedurl_uploader-1.2.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-signedUrl-uploader
-Version: 1.2.3
+Version: 1.2.4
 Summary: Streamlit component that allows you to upload files to Google Cloud Storage via signed url
 Home-page: 
 Author: Meryam Assermouh
 Author-email: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -113,10 +113,17 @@
 
   # Use the uploader function to handle file uploads
   signedUrl_uploader(storage_client, credentials, bucket_name)
 
 if __name__ == "__main__":
     main()
 ```
+
+You can run the application using the command below and replacing `main.py` by the name of your file.
+
+```
+streamlit run main.py
+```
+
 ## Useful links
 
 [GitHub Repository](https://github.com/Meryam-A/signed-url-uploader)
```

### Comparing `st_signedurl_uploader-1.2.3/README.md` & `st_signedurl_uploader-1.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -94,10 +94,17 @@
 
   # Use the uploader function to handle file uploads
   signedUrl_uploader(storage_client, credentials, bucket_name)
 
 if __name__ == "__main__":
     main()
 ```
+
+You can run the application using the command below and replacing `main.py` by the name of your file.
+
+```
+streamlit run main.py
+```
+
 ## Useful links
 
 [GitHub Repository](https://github.com/Meryam-A/signed-url-uploader)
```

### Comparing `st_signedurl_uploader-1.2.3/setup.py` & `st_signedurl_uploader-1.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name="st-signedUrl-uploader",
-    version="1.2.3",
+    version="1.2.4",
     author="Meryam Assermouh",
     author_email="",
     description="Streamlit component that allows you to upload files to Google Cloud Storage via signed url",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st_signedurl_uploader-1.2.3/st_signedUrl_uploader/__init__.py` & `st_signedurl_uploader-1.2.4/st_signedUrl_uploader/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,17 +30,17 @@
 
 def signedUrl_uploader(storage_client, credentials, bucket_name, key='1'):
 
     bucket = storage_client.get_bucket(bucket_name)
     blob = bucket.blob("signedUrl file")
     signed_url = generate_signed_url(credentials, blob)
     files_data = _component_func(signed_url=signed_url,key=key)
-    while not blob.exists() :
-        time.sleep(1)
     if files_data:
+        while not blob.exists() :
+            time.sleep(1)
         new_blob = bucket.rename_blob(blob, files_data['filename'])
         new_blob.content_type = files_data['content_type']
         new_blob.patch()        
         st.toast('File Uploaded Successfully !', icon='🤩')
 
     return files_data
```

### Comparing `st_signedurl_uploader-1.2.3/st_signedUrl_uploader/frontend/build/bootstrap.min.css` & `st_signedurl_uploader-1.2.4/st_signedUrl_uploader/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.3/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js` & `st_signedurl_uploader-1.2.4/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.3/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt` & `st_signedurl_uploader-1.2.4/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.3/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.map` & `st_signedurl_uploader-1.2.4/st_signedUrl_uploader/frontend/build/static/js/main.022a2283.js.map`

 * *Files identical despite different names*

### Comparing `st_signedurl_uploader-1.2.3/st_signedUrl_uploader.egg-info/PKG-INFO` & `st_signedurl_uploader-1.2.4/st_signedUrl_uploader.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-signedUrl-uploader
-Version: 1.2.3
+Version: 1.2.4
 Summary: Streamlit component that allows you to upload files to Google Cloud Storage via signed url
 Home-page: 
 Author: Meryam Assermouh
 Author-email: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -113,10 +113,17 @@
 
   # Use the uploader function to handle file uploads
   signedUrl_uploader(storage_client, credentials, bucket_name)
 
 if __name__ == "__main__":
     main()
 ```
+
+You can run the application using the command below and replacing `main.py` by the name of your file.
+
+```
+streamlit run main.py
+```
+
 ## Useful links
 
 [GitHub Repository](https://github.com/Meryam-A/signed-url-uploader)
```

### Comparing `st_signedurl_uploader-1.2.3/st_signedUrl_uploader.egg-info/SOURCES.txt` & `st_signedurl_uploader-1.2.4/st_signedUrl_uploader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

