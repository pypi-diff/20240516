# Comparing `tmp/eurmlsdk-0.0.901.tar.gz` & `tmp/eurmlsdk-0.0.902.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eurmlsdk-0.0.901.tar", last modified: Thu May 16 06:40:16 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.902.tar", last modified: Thu May 16 07:21:14 2024, max compression
```

## Comparing `eurmlsdk-0.0.901.tar` & `eurmlsdk-0.0.902.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.901/README.md
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.901/MANIFEST.in
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      847 2024-05-16 06:32:05.000000 eurmlsdk-0.0.901/setup.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.901/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/PKG-INFO
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 06:40:16.000000 eurmlsdk-0.0.901/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5497 2024-05-16 06:11:26.000000 eurmlsdk-0.0.901/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.0.901/eurmlsdk/eur_sdk.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1320 2024-05-16 06:31:39.000000 eurmlsdk-0.0.901/eurmlsdk/yolo.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4007 2024-05-16 06:11:26.000000 eurmlsdk-0.0.901/eurmlsdk/pytorch.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.0.901/eurmlsdk/__init__.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 07:21:14.923050 eurmlsdk-0.0.902/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.902/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.902/MANIFEST.in
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 07:21:14.923050 eurmlsdk-0.0.902/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.902/README.md
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 07:21:14.923050 eurmlsdk-0.0.902/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.0.902/eurmlsdk/__init__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5497 2024-05-16 06:11:26.000000 eurmlsdk-0.0.902/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.0.902/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4010 2024-05-16 07:16:28.000000 eurmlsdk-0.0.902/eurmlsdk/pytorch.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1320 2024-05-16 06:31:39.000000 eurmlsdk-0.0.902/eurmlsdk/yolo.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 07:21:14.923050 eurmlsdk-0.0.902/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 07:21:14.000000 eurmlsdk-0.0.902/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-16 07:21:14.000000 eurmlsdk-0.0.902/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-16 07:21:14.000000 eurmlsdk-0.0.902/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-16 07:21:14.000000 eurmlsdk-0.0.902/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-16 07:21:14.000000 eurmlsdk-0.0.902/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-16 07:21:14.000000 eurmlsdk-0.0.902/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-16 07:21:14.923050 eurmlsdk-0.0.902/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      847 2024-05-16 07:20:48.000000 eurmlsdk-0.0.902/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `eurmlsdk-0.0.901/setup.py` & `eurmlsdk-0.0.902/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.901',
+    version='0.0.902',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
```

### Comparing `eurmlsdk-0.0.901/eurmlsdk/__main__.py` & `eurmlsdk-0.0.902/eurmlsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.901/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.902/eurmlsdk/eur_sdk.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.901/eurmlsdk/yolo.py` & `eurmlsdk-0.0.902/eurmlsdk/yolo.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.901/eurmlsdk/pytorch.py` & `eurmlsdk-0.0.902/eurmlsdk/pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                 correct += (predicted == labels).sum().item()
 
         accuracy = correct/total
         return accuracy
     
     def get_predicted_results(self, results):
         list_predicted_set = ['airplane', 'automobile', 'bird', 'cat', 'deer', 'dog', 'frog', 'horse', 'ship', 'truck']
-        predictied_values = list(map(int, results))
+        predictied_values = list(map(int, results[0]))
         print(predictied_values)
         for res in predictied_values:
             print("Predicted_result :", list_predicted_set[res])
```

