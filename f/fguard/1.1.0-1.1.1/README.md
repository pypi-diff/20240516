# Comparing `tmp/fguard-1.1.0.tar.gz` & `tmp/fguard-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fguard-1.1.0.tar", last modified: Thu May 16 17:21:04 2024, max compression
+gzip compressed data, was "fguard-1.1.1.tar", last modified: Thu May 16 17:27:36 2024, max compression
```

## Comparing `fguard-1.1.0.tar` & `fguard-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 17:21:04.682975 fguard-1.1.0/
--rw-rw-rw-   0        0        0    35823 2024-05-16 13:10:42.000000 fguard-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2824 2024-05-16 17:21:04.682975 fguard-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2274 2024-05-16 17:18:39.000000 fguard-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 17:21:04.667354 fguard-1.1.0/fguard/
--rw-rw-rw-   0        0        0        0 2024-05-16 13:14:49.000000 fguard-1.1.0/fguard/__init__.py
--rw-rw-rw-   0        0        0    13941 2024-05-16 16:32:23.000000 fguard-1.1.0/fguard/cli.py
-drwxrwxrwx   0        0        0        0 2024-05-16 17:21:04.682975 fguard-1.1.0/fguard/core/
--rw-rw-rw-   0        0        0        0 2024-05-16 17:09:53.000000 fguard-1.1.0/fguard/core/__init__.py
--rw-rw-rw-   0        0        0     8600 2024-05-15 13:38:39.000000 fguard-1.1.0/fguard/core/communication.py
--rw-rw-rw-   0        0        0     5082 2024-05-14 21:41:18.000000 fguard-1.1.0/fguard/core/handler.py
-drwxrwxrwx   0        0        0        0 2024-05-16 17:21:04.682975 fguard-1.1.0/fguard/core/unet/
--rw-rw-rw-   0        0        0        0 2024-05-16 17:10:02.000000 fguard-1.1.0/fguard/core/unet/__init__.py
--rw-rw-rw-   0        0        0     1786 2024-05-16 12:47:52.000000 fguard-1.1.0/fguard/core/unet/unet_model.py
--rw-rw-rw-   0        0        0     2679 2024-04-25 20:53:17.000000 fguard-1.1.0/fguard/core/unet/unet_parts.py
--rw-rw-rw-   0        0        0     2713 2024-05-14 21:45:33.000000 fguard-1.1.0/fguard/core/utils.py
--rw-rw-rw-   0        0        0     5225 2024-05-16 12:40:10.000000 fguard-1.1.0/fguard/core/vision.py
-drwxrwxrwx   0        0        0        0 2024-05-16 17:21:04.682975 fguard-1.1.0/fguard.egg-info/
--rw-rw-rw-   0        0        0     2824 2024-05-16 17:21:04.000000 fguard-1.1.0/fguard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2024-05-16 17:21:04.000000 fguard-1.1.0/fguard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 17:21:04.000000 fguard-1.1.0/fguard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-16 17:21:04.000000 fguard-1.1.0/fguard.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      152 2024-05-16 17:21:04.000000 fguard-1.1.0/fguard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 17:21:04.000000 fguard-1.1.0/fguard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      213 2024-05-16 13:56:19.000000 fguard-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 17:21:04.698593 fguard-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1070 2024-05-16 17:20:41.000000 fguard-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:27:36.921847 fguard-1.1.1/
+-rw-rw-rw-   0        0        0    35823 2024-05-16 13:10:42.000000 fguard-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2824 2024-05-16 17:27:36.921847 fguard-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2274 2024-05-16 17:18:39.000000 fguard-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 17:27:36.906240 fguard-1.1.1/fguard/
+-rw-rw-rw-   0        0        0        0 2024-05-16 13:14:49.000000 fguard-1.1.1/fguard/__init__.py
+-rw-rw-rw-   0        0        0    13941 2024-05-16 16:32:23.000000 fguard-1.1.1/fguard/cli.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:27:36.921847 fguard-1.1.1/fguard/core/
+-rw-rw-rw-   0        0        0        0 2024-05-16 17:09:53.000000 fguard-1.1.1/fguard/core/__init__.py
+-rw-rw-rw-   0        0        0     8600 2024-05-15 13:38:39.000000 fguard-1.1.1/fguard/core/communication.py
+-rw-rw-rw-   0        0        0     5082 2024-05-14 21:41:18.000000 fguard-1.1.1/fguard/core/handler.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:27:36.921847 fguard-1.1.1/fguard/core/unet/
+-rw-rw-rw-   0        0        0        0 2024-05-16 17:10:02.000000 fguard-1.1.1/fguard/core/unet/__init__.py
+-rw-rw-rw-   0        0        0     1786 2024-05-16 12:47:52.000000 fguard-1.1.1/fguard/core/unet/unet_model.py
+-rw-rw-rw-   0        0        0     2679 2024-04-25 20:53:17.000000 fguard-1.1.1/fguard/core/unet/unet_parts.py
+-rw-rw-rw-   0        0        0     2713 2024-05-14 21:45:33.000000 fguard-1.1.1/fguard/core/utils.py
+-rw-rw-rw-   0        0        0     5225 2024-05-16 12:40:10.000000 fguard-1.1.1/fguard/core/vision.py
+drwxrwxrwx   0        0        0        0 2024-05-16 17:27:36.921847 fguard-1.1.1/fguard.egg-info/
+-rw-rw-rw-   0        0        0     2824 2024-05-16 17:27:36.000000 fguard-1.1.1/fguard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2024-05-16 17:27:36.000000 fguard-1.1.1/fguard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 17:27:36.000000 fguard-1.1.1/fguard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-16 17:27:36.000000 fguard-1.1.1/fguard.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      185 2024-05-16 17:27:36.000000 fguard-1.1.1/fguard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 17:27:36.000000 fguard-1.1.1/fguard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      213 2024-05-16 13:56:19.000000 fguard-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 17:27:36.921847 fguard-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1127 2024-05-16 17:26:50.000000 fguard-1.1.1/setup.py
```

### Comparing `fguard-1.1.0/LICENSE` & `fguard-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fguard-1.1.0/PKG-INFO` & `fguard-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fguard
-Version: 1.1.0
+Version: 1.1.1
 Summary: Detect deforestation on area over a given period of time
 Home-page: https://forestguardian.ru/
 Author: Ivan Gronsky
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `fguard-1.1.0/README.md` & `fguard-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fguard-1.1.0/fguard/cli.py` & `fguard-1.1.1/fguard/cli.py`

 * *Files identical despite different names*

### Comparing `fguard-1.1.0/fguard/core/communication.py` & `fguard-1.1.1/fguard/core/communication.py`

 * *Files identical despite different names*

### Comparing `fguard-1.1.0/fguard/core/handler.py` & `fguard-1.1.1/fguard/core/handler.py`

 * *Files identical despite different names*

### Comparing `fguard-1.1.0/fguard/core/unet/unet_model.py` & `fguard-1.1.1/fguard/core/unet/unet_model.py`

 * *Files identical despite different names*

### Comparing `fguard-1.1.0/fguard/core/unet/unet_parts.py` & `fguard-1.1.1/fguard/core/unet/unet_parts.py`

 * *Files identical despite different names*

### Comparing `fguard-1.1.0/fguard/core/utils.py` & `fguard-1.1.1/fguard/core/utils.py`

 * *Files identical despite different names*

### Comparing `fguard-1.1.0/fguard/core/vision.py` & `fguard-1.1.1/fguard/core/vision.py`

 * *Files identical despite different names*

### Comparing `fguard-1.1.0/fguard.egg-info/PKG-INFO` & `fguard-1.1.1/fguard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fguard
-Version: 1.1.0
+Version: 1.1.1
 Summary: Detect deforestation on area over a given period of time
 Home-page: https://forestguardian.ru/
 Author: Ivan Gronsky
 License: GPL-3.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `fguard-1.1.0/setup.py` & `fguard-1.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="fguard",
-    version="1.1.0",
+    version="1.1.1",
     url="https://forestguardian.ru/",
     author="Ivan Gronsky",
     description="Detect deforestation on area over a given period of time",
     long_description=open("README.MD").read(),
     long_description_content_type='text/markdown',
     license="GPL-3.0",
     classifiers=[
@@ -23,14 +23,16 @@
         "joblib==1.3.2",
         "numpy==1.26.3",
         "opencv-python==4.8.1.78",
         "platformdirs==4.2.1",
         "python-dotenv==1.0.0",
         "requests==2.31.0",
         "tqdm==4.66.2",
+        "torch==2.3.0",
+        "torchvision==0.18.0",
     ],
     entry_points={
         "console_scripts": [
             "fguard = fguard.cli:main",
         ],
     },
 )
```

