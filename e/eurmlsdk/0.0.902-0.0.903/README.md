# Comparing `tmp/eurmlsdk-0.0.902.tar.gz` & `tmp/eurmlsdk-0.0.903.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.902.tar", last modified: Thu May 16 07:21:14 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.903.tar", last modified: Thu May 16 08:20:53 2024, max compression
```

## Comparing `eurmlsdk-0.0.902.tar` & `eurmlsdk-0.0.903.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 07:21:14.923050 eurmlsdk-0.0.902/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.902/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.902/MANIFEST.in
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 07:21:14.923050 eurmlsdk-0.0.902/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.902/README.md
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 07:21:14.923050 eurmlsdk-0.0.902/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.0.902/eurmlsdk/__init__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5497 2024-05-16 06:11:26.000000 eurmlsdk-0.0.902/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.0.902/eurmlsdk/eur_sdk.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4010 2024-05-16 07:16:28.000000 eurmlsdk-0.0.902/eurmlsdk/pytorch.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1320 2024-05-16 06:31:39.000000 eurmlsdk-0.0.902/eurmlsdk/yolo.py
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 07:21:14.923050 eurmlsdk-0.0.902/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 07:21:14.000000 eurmlsdk-0.0.902/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-16 07:21:14.000000 eurmlsdk-0.0.902/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-16 07:21:14.000000 eurmlsdk-0.0.902/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-16 07:21:14.000000 eurmlsdk-0.0.902/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-16 07:21:14.000000 eurmlsdk-0.0.902/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-16 07:21:14.000000 eurmlsdk-0.0.902/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-16 07:21:14.923050 eurmlsdk-0.0.902/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      847 2024-05-16 07:20:48.000000 eurmlsdk-0.0.902/setup.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 08:20:53.823050 eurmlsdk-0.0.903/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.903/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.903/MANIFEST.in
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 08:20:53.823050 eurmlsdk-0.0.903/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.903/README.md
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 08:20:53.823050 eurmlsdk-0.0.903/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.0.903/eurmlsdk/__init__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5498 2024-05-16 07:22:12.000000 eurmlsdk-0.0.903/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.0.903/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4036 2024-05-16 07:32:23.000000 eurmlsdk-0.0.903/eurmlsdk/pytorch.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     2032 2024-05-16 08:17:25.000000 eurmlsdk-0.0.903/eurmlsdk/yolo.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 08:20:53.823050 eurmlsdk-0.0.903/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 08:20:53.000000 eurmlsdk-0.0.903/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-16 08:20:53.000000 eurmlsdk-0.0.903/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-16 08:20:53.000000 eurmlsdk-0.0.903/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-16 08:20:53.000000 eurmlsdk-0.0.903/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-16 08:20:53.000000 eurmlsdk-0.0.903/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-16 08:20:53.000000 eurmlsdk-0.0.903/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-16 08:20:53.823050 eurmlsdk-0.0.903/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      847 2024-05-16 08:20:20.000000 eurmlsdk-0.0.903/setup.py
```

### Comparing `eurmlsdk-0.0.902/eurmlsdk/__main__.py` & `eurmlsdk-0.0.903/eurmlsdk/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 def main():
     commands_list = ['deploy','help','--h','predict','validate', 'pt-predict', 'pt-validate']
     try:
         argLen = len(argv)
         if argLen == 1:
             print("Model Zoo SDK")
             print("Package name: eurmlsdk")
-            print("Version: 0.0.84")
+            print("Version: 0.0.902")
             print("Run 'eurmlsdk help' or eurmlsdk --h to find the list of commands.")
             exit()
 
         command = argv[1]
         if command not in commands_list:
             print("Unknown command. Please find the list of commands")
             list_commands()
```

### Comparing `eurmlsdk-0.0.902/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.903/eurmlsdk/eur_sdk.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.902/eurmlsdk/pytorch.py` & `eurmlsdk-0.0.903/eurmlsdk/pytorch.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,17 +54,17 @@
                 correct += (predicted == labels).sum().item()
 
         accuracy = correct/total
         return accuracy
     
     def get_predicted_results(self, results):
         list_predicted_set = ['airplane', 'automobile', 'bird', 'cat', 'deer', 'dog', 'frog', 'horse', 'ship', 'truck']
-        predictied_values = list(map(int, results[0]))
-        print(predictied_values)
-        for res in predictied_values:
+        predicted_results = list(map(int, results))
+        final_values = [int(d) for d in str(predicted_results[0])]
+        for res in final_values:
             print("Predicted_result :", list_predicted_set[res]) 
 
 
  
 
 
     # def loadModel(self, model_path):
```

### Comparing `eurmlsdk-0.0.902/setup.py` & `eurmlsdk-0.0.903/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.902',
+    version='0.0.903',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
```

