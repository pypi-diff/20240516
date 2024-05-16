# Comparing `tmp/eurmlsdk-0.0.90.tar.gz` & `tmp/eurmlsdk-0.0.901.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.90.tar", last modified: Thu May 16 05:35:19 2024, max compression
+gzip compressed data, was "dist/eurmlsdk-0.0.901.tar", last modified: Thu May 16 06:40:16 2024, max compression
```

## Comparing `eurmlsdk-0.0.90.tar` & `eurmlsdk-0.0.901.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-16 05:35:19.506616 eurmlsdk-0.0.90/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       16 2024-05-08 10:50:34.000000 eurmlsdk-0.0.90/LICENSE.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-05-08 10:50:34.000000 eurmlsdk-0.0.90/MANIFEST.in
--rw-r--r--   0 surajram  (1000) surajram  (1000)      612 2024-05-16 05:35:19.506616 eurmlsdk-0.0.90/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)       10 2024-05-08 10:50:34.000000 eurmlsdk-0.0.90/README.md
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-16 05:35:19.506616 eurmlsdk-0.0.90/eurmlsdk/
--rw-r--r--   0 surajram  (1000) surajram  (1000)       33 2024-05-16 04:56:10.000000 eurmlsdk-0.0.90/eurmlsdk/__init__.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)     5497 2024-05-16 04:56:10.000000 eurmlsdk-0.0.90/eurmlsdk/__main__.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)     9540 2024-05-16 04:56:10.000000 eurmlsdk-0.0.90/eurmlsdk/eur_sdk.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)     4007 2024-05-16 04:56:10.000000 eurmlsdk-0.0.90/eurmlsdk/pytorch.py
--rw-r--r--   0 surajram  (1000) surajram  (1000)     1217 2024-05-16 04:56:10.000000 eurmlsdk-0.0.90/eurmlsdk/yolo.py
-drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-16 05:35:19.506616 eurmlsdk-0.0.90/eurmlsdk.egg-info/
--rw-r--r--   0 surajram  (1000) surajram  (1000)      612 2024-05-16 05:35:19.000000 eurmlsdk-0.0.90/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 surajram  (1000) surajram  (1000)      335 2024-05-16 05:35:19.000000 eurmlsdk-0.0.90/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-05-16 05:35:19.000000 eurmlsdk-0.0.90/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       52 2024-05-16 05:35:19.000000 eurmlsdk-0.0.90/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)      102 2024-05-16 05:35:19.000000 eurmlsdk-0.0.90/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)        9 2024-05-16 05:35:19.000000 eurmlsdk-0.0.90/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-05-16 05:35:19.506616 eurmlsdk-0.0.90/setup.cfg
--rw-r--r--   0 surajram  (1000) surajram  (1000)      846 2024-05-16 05:35:09.000000 eurmlsdk-0.0.90/setup.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.901/README.md
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.901/MANIFEST.in
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      847 2024-05-16 06:32:05.000000 eurmlsdk-0.0.901/setup.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.901/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/PKG-INFO
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5497 2024-05-16 06:11:26.000000 eurmlsdk-0.0.901/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.0.901/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1320 2024-05-16 06:31:39.000000 eurmlsdk-0.0.901/eurmlsdk/yolo.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4007 2024-05-16 06:11:26.000000 eurmlsdk-0.0.901/eurmlsdk/pytorch.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.0.901/eurmlsdk/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `eurmlsdk-0.0.90/eurmlsdk/__main__.py` & `eurmlsdk-0.0.901/eurmlsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.90/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.901/eurmlsdk/eur_sdk.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.90/eurmlsdk/pytorch.py` & `eurmlsdk-0.0.901/eurmlsdk/pytorch.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.90/eurmlsdk/yolo.py` & `eurmlsdk-0.0.901/eurmlsdk/yolo.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,17 @@
         else:
             raise ModelNotFound()
         
     def predict_model(self, pathArg, dataSet):
         try:
             model = self.load_model(pathArg)
             print("Prediction started.....")
-            model.predict(dataSet, save=True)
+            results = model(dataSet,stream=True)
+            print(f"Prediction results: {results}")
+            # model.predict(dataSet, save=True)
         except ModelNotFound as err:
             print("Error :", err)
             exit(1)
         except Exception as err:
             print("Error in Prediction :", err)
             exit(1)
```

### Comparing `eurmlsdk-0.0.90/setup.py` & `eurmlsdk-0.0.901/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.90',
+    version='0.0.901',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
```

