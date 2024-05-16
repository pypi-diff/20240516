# Comparing `tmp/worqhat-0.0.1.tar.gz` & `tmp/worqhat-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worqhat-0.0.1.tar", last modified: Thu May  9 19:04:26 2024, max compression
+gzip compressed data, was "worqhat-1.0.tar", last modified: Thu May 16 20:01:37 2024, max compression
```

## Comparing `worqhat-0.0.1.tar` & `worqhat-1.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 19:04:26.962080 worqhat-0.0.1/
--rw-rw-rw-   0        0        0    11558 2024-04-24 15:55:14.000000 worqhat-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      588 2024-05-09 19:04:26.960077 worqhat-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 19:04:26.918423 worqhat-0.0.1/app/
-drwxrwxrwx   0        0        0        0 2024-05-09 19:04:26.923597 worqhat-0.0.1/app/worqhat/
--rw-rw-rw-   0        0        0      390 2024-04-30 17:34:32.000000 worqhat-0.0.1/app/worqhat/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 19:04:26.941060 worqhat-0.0.1/app/worqhat/ai_models/
--rw-rw-rw-   0        0        0      307 2024-04-30 17:28:00.000000 worqhat-0.0.1/app/worqhat/ai_models/__init__.py
--rw-rw-rw-   0        0        0     1513 2024-05-09 18:54:18.000000 worqhat-0.0.1/app/worqhat/ai_models/ai_search.py
--rw-rw-rw-   0        0        0     1594 2024-05-09 18:54:24.000000 worqhat-0.0.1/app/worqhat/ai_models/content_mod.py
--rw-rw-rw-   0        0        0     4096 2024-05-09 18:54:34.000000 worqhat-0.0.1/app/worqhat/ai_models/image_analysis.py
--rw-rw-rw-   0        0        0    10541 2024-05-09 18:54:50.000000 worqhat-0.0.1/app/worqhat/ai_models/image_gen.py
--rw-rw-rw-   0        0        0     1805 2024-05-09 18:54:57.000000 worqhat-0.0.1/app/worqhat/ai_models/model_train.py
--rw-rw-rw-   0        0        0     3180 2024-05-09 18:55:05.000000 worqhat-0.0.1/app/worqhat/ai_models/text_extract.py
--rw-rw-rw-   0        0        0     6493 2024-05-09 18:55:31.000000 worqhat-0.0.1/app/worqhat/ai_models/text_gen.py
-drwxrwxrwx   0        0        0        0 2024-05-09 19:04:26.946064 worqhat-0.0.1/app/worqhat/database_management/
--rw-rw-rw-   0        0        0     4509 2024-05-09 18:55:41.000000 worqhat-0.0.1/app/worqhat/database_management/Edit.py
--rw-rw-rw-   0        0        0     5143 2024-05-09 18:55:46.000000 worqhat-0.0.1/app/worqhat/database_management/Read.py
--rw-rw-rw-   0        0        0      111 2024-04-30 17:28:48.000000 worqhat-0.0.1/app/worqhat/database_management/__init__.py
--rw-rw-rw-   0        0        0      815 2024-05-09 18:55:39.000000 worqhat-0.0.1/app/worqhat/database_management/collection.py
-drwxrwxrwx   0        0        0        0 2024-05-09 19:04:26.957074 worqhat-0.0.1/app/worqhat/test/
--rw-rw-rw-   0        0        0        0 2024-04-24 16:31:55.000000 worqhat-0.0.1/app/worqhat/test/__init__.py
--rw-rw-rw-   0        0        0     1406 2024-04-26 17:24:15.000000 worqhat-0.0.1/app/worqhat/test/test_ai_search.py
--rw-rw-rw-   0        0        0     1518 2024-04-26 17:27:14.000000 worqhat-0.0.1/app/worqhat/test/test_content_mod.py
--rw-rw-rw-   0        0        0     2217 2024-04-26 17:30:05.000000 worqhat-0.0.1/app/worqhat/test/test_image_analysis.py
--rw-rw-rw-   0        0        0        0 2024-04-26 17:31:39.000000 worqhat-0.0.1/app/worqhat/test/test_image_gen.py
--rw-rw-rw-   0        0        0     2158 2024-04-26 17:35:50.000000 worqhat-0.0.1/app/worqhat/test/test_model_train.py
--rw-rw-rw-   0        0        0     2693 2024-04-26 17:37:11.000000 worqhat-0.0.1/app/worqhat/test/test_text_extract.py
--rw-rw-rw-   0        0        0     2783 2024-04-26 17:41:53.000000 worqhat-0.0.1/app/worqhat/test/test_text_gen.py
-drwxrwxrwx   0        0        0        0 2024-05-09 19:04:26.959076 worqhat-0.0.1/app/worqhat.egg-info/
--rw-rw-rw-   0        0        0      588 2024-05-09 19:04:26.000000 worqhat-0.0.1/app/worqhat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      959 2024-05-09 19:04:26.000000 worqhat-0.0.1/app/worqhat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 19:04:26.000000 worqhat-0.0.1/app/worqhat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-05-09 19:04:26.000000 worqhat-0.0.1/app/worqhat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-09 19:04:26.000000 worqhat-0.0.1/app/worqhat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 19:04:26.962080 worqhat-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      860 2024-05-09 18:42:12.000000 worqhat-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:01:37.757205 worqhat-1.0/
+-rw-rw-rw-   0        0        0    11558 2024-04-24 15:55:14.000000 worqhat-1.0/LICENSE
+-rw-rw-rw-   0        0        0     3868 2024-05-16 20:01:37.755203 worqhat-1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-16 20:01:37.707159 worqhat-1.0/app/
+drwxrwxrwx   0        0        0        0 2024-05-16 20:01:37.713164 worqhat-1.0/app/worqhat/
+-rw-rw-rw-   0        0        0      390 2024-04-30 17:34:32.000000 worqhat-1.0/app/worqhat/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:01:37.735185 worqhat-1.0/app/worqhat/ai_models/
+-rw-rw-rw-   0        0        0      307 2024-04-30 17:28:00.000000 worqhat-1.0/app/worqhat/ai_models/__init__.py
+-rw-rw-rw-   0        0        0     1513 2024-05-09 18:54:18.000000 worqhat-1.0/app/worqhat/ai_models/ai_search.py
+-rw-rw-rw-   0        0        0     1594 2024-05-09 18:54:24.000000 worqhat-1.0/app/worqhat/ai_models/content_mod.py
+-rw-rw-rw-   0        0        0     4096 2024-05-09 18:54:34.000000 worqhat-1.0/app/worqhat/ai_models/image_analysis.py
+-rw-rw-rw-   0        0        0    10543 2024-05-11 18:55:08.000000 worqhat-1.0/app/worqhat/ai_models/image_gen.py
+-rw-rw-rw-   0        0        0     1805 2024-05-09 18:54:57.000000 worqhat-1.0/app/worqhat/ai_models/model_train.py
+-rw-rw-rw-   0        0        0     3180 2024-05-09 18:55:05.000000 worqhat-1.0/app/worqhat/ai_models/text_extract.py
+-rw-rw-rw-   0        0        0     6493 2024-05-09 18:55:31.000000 worqhat-1.0/app/worqhat/ai_models/text_gen.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:01:37.740189 worqhat-1.0/app/worqhat/database_management/
+-rw-rw-rw-   0        0        0     4509 2024-05-09 18:55:41.000000 worqhat-1.0/app/worqhat/database_management/Edit.py
+-rw-rw-rw-   0        0        0     5143 2024-05-09 18:55:46.000000 worqhat-1.0/app/worqhat/database_management/Read.py
+-rw-rw-rw-   0        0        0      111 2024-04-30 17:28:48.000000 worqhat-1.0/app/worqhat/database_management/__init__.py
+-rw-rw-rw-   0        0        0      815 2024-05-09 18:55:39.000000 worqhat-1.0/app/worqhat/database_management/collection.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:01:37.751199 worqhat-1.0/app/worqhat/test/
+-rw-rw-rw-   0        0        0        0 2024-04-24 16:31:55.000000 worqhat-1.0/app/worqhat/test/__init__.py
+-rw-rw-rw-   0        0        0     1406 2024-04-26 17:24:15.000000 worqhat-1.0/app/worqhat/test/test_ai_search.py
+-rw-rw-rw-   0        0        0     1518 2024-04-26 17:27:14.000000 worqhat-1.0/app/worqhat/test/test_content_mod.py
+-rw-rw-rw-   0        0        0     2217 2024-04-26 17:30:05.000000 worqhat-1.0/app/worqhat/test/test_image_analysis.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 17:31:39.000000 worqhat-1.0/app/worqhat/test/test_image_gen.py
+-rw-rw-rw-   0        0        0     2158 2024-04-26 17:35:50.000000 worqhat-1.0/app/worqhat/test/test_model_train.py
+-rw-rw-rw-   0        0        0     2693 2024-04-26 17:37:11.000000 worqhat-1.0/app/worqhat/test/test_text_extract.py
+-rw-rw-rw-   0        0        0     2783 2024-04-26 17:41:53.000000 worqhat-1.0/app/worqhat/test/test_text_gen.py
+drwxrwxrwx   0        0        0        0 2024-05-16 20:01:37.753201 worqhat-1.0/app/worqhat.egg-info/
+-rw-rw-rw-   0        0        0     3868 2024-05-16 20:01:37.000000 worqhat-1.0/app/worqhat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      959 2024-05-16 20:01:37.000000 worqhat-1.0/app/worqhat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 20:01:37.000000 worqhat-1.0/app/worqhat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-16 20:01:37.000000 worqhat-1.0/app/worqhat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 20:01:37.000000 worqhat-1.0/app/worqhat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 20:01:37.757205 worqhat-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      858 2024-05-16 19:36:49.000000 worqhat-1.0/setup.py
```

### Comparing `worqhat-0.0.1/LICENSE` & `worqhat-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat/ai_models/ai_search.py` & `worqhat-1.0/app/worqhat/ai_models/ai_search.py`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat/ai_models/content_mod.py` & `worqhat-1.0/app/worqhat/ai_models/content_mod.py`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat/ai_models/image_analysis.py` & `worqhat-1.0/app/worqhat/ai_models/image_analysis.py`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat/ai_models/image_gen.py` & `worqhat-1.0/app/worqhat/ai_models/image_gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 import os
 
 
-def generate_image_v2(prompt="", image_style="realistic", output_type="url", orientation="square", api_key=None):
+def generate_image_v2(prompt=[""], image_style="realistic", output_type="url", orientation="square", api_key=None):
     if not api_key:
         api_key = os.getenv("API_KEY")
     if not api_key:
          raise ValueError("API key is missing. Provide it as an argument or in the .env file.")
     url = "https://api.worqhat.com/api/ai/images/generate/v2"
     headers = {
         "Authorization": "Bearer " + api_key,
@@ -17,15 +17,15 @@
         "image_style": image_style,
         "output_type": output_type,
         "orientation": orientation
     }
     response = requests.post(url, json=payload, headers=headers)
     return response.text
 
-def generate_image_v3(prompt="", image_style="realistic", output_type="url", orientation="square", api_key=None):
+def generate_image_v3(prompt=[], image_style="realistic", output_type="url", orientation="square", api_key=None):
     if not api_key:
         api_key = os.getenv("API_KEY")
 
     if not api_key:
          raise ValueError("API key is missing. Provide it as an argument or in the .env file.")
     url = "https://api.worqhat.com/api/ai/images/generate/v3"
     headers = {
```

### Comparing `worqhat-0.0.1/app/worqhat/ai_models/model_train.py` & `worqhat-1.0/app/worqhat/ai_models/model_train.py`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat/ai_models/text_extract.py` & `worqhat-1.0/app/worqhat/ai_models/text_extract.py`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat/ai_models/text_gen.py` & `worqhat-1.0/app/worqhat/ai_models/text_gen.py`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat/database_management/Edit.py` & `worqhat-1.0/app/worqhat/database_management/Edit.py`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat/database_management/Read.py` & `worqhat-1.0/app/worqhat/database_management/Read.py`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat/database_management/collection.py` & `worqhat-1.0/app/worqhat/database_management/collection.py`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat/test/test_ai_search.py` & `worqhat-1.0/app/worqhat/test/test_ai_search.py`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat/test/test_content_mod.py` & `worqhat-1.0/app/worqhat/test/test_content_mod.py`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat/test/test_image_analysis.py` & `worqhat-1.0/app/worqhat/test/test_image_analysis.py`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat/test/test_model_train.py` & `worqhat-1.0/app/worqhat/test/test_model_train.py`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat/test/test_text_extract.py` & `worqhat-1.0/app/worqhat/test/test_text_extract.py`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat/test/test_text_gen.py` & `worqhat-1.0/app/worqhat/test/test_text_gen.py`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/app/worqhat.egg-info/SOURCES.txt` & `worqhat-1.0/app/worqhat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `worqhat-0.0.1/setup.py` & `worqhat-1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="worqhat",
-    version="0.0.1",
+    version="1.0",
     description="A package with all the APIs available from worqHat",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Ayush-Kul/worqhat-python",
     author="WorqHat",
```

