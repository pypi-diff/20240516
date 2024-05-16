# Comparing `tmp/eurmlsdk-0.0.904.tar.gz` & `tmp/eurmlsdk-0.0.905.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.904.tar", last modified: Thu May 16 10:23:22 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.905.tar", last modified: Thu May 16 10:30:22 2024, max compression
```

## Comparing `eurmlsdk-0.0.904.tar` & `eurmlsdk-0.0.905.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 10:23:22.663050 eurmlsdk-0.0.904/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.904/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.904/MANIFEST.in
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 10:23:22.653050 eurmlsdk-0.0.904/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.904/README.md
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 10:23:22.653050 eurmlsdk-0.0.904/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.0.904/eurmlsdk/__init__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     6150 2024-05-16 10:22:37.000000 eurmlsdk-0.0.904/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.0.904/eurmlsdk/eur_sdk.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4036 2024-05-16 07:32:23.000000 eurmlsdk-0.0.904/eurmlsdk/pytorch.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     2032 2024-05-16 08:17:25.000000 eurmlsdk-0.0.904/eurmlsdk/yolo.py
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 10:23:22.653050 eurmlsdk-0.0.904/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 10:23:22.000000 eurmlsdk-0.0.904/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-16 10:23:22.000000 eurmlsdk-0.0.904/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-16 10:23:22.000000 eurmlsdk-0.0.904/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-16 10:23:22.000000 eurmlsdk-0.0.904/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-16 10:23:22.000000 eurmlsdk-0.0.904/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-16 10:23:22.000000 eurmlsdk-0.0.904/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-16 10:23:22.663050 eurmlsdk-0.0.904/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      847 2024-05-16 10:22:56.000000 eurmlsdk-0.0.904/setup.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 10:30:22.143050 eurmlsdk-0.0.905/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.905/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.905/MANIFEST.in
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 10:30:22.143050 eurmlsdk-0.0.905/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.905/README.md
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 10:30:22.143050 eurmlsdk-0.0.905/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.0.905/eurmlsdk/__init__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     6251 2024-05-16 10:30:06.000000 eurmlsdk-0.0.905/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.0.905/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4036 2024-05-16 07:32:23.000000 eurmlsdk-0.0.905/eurmlsdk/pytorch.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1217 2024-05-16 10:29:42.000000 eurmlsdk-0.0.905/eurmlsdk/yolo.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 10:30:22.143050 eurmlsdk-0.0.905/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 10:30:22.000000 eurmlsdk-0.0.905/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-16 10:30:22.000000 eurmlsdk-0.0.905/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-16 10:30:22.000000 eurmlsdk-0.0.905/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-16 10:30:22.000000 eurmlsdk-0.0.905/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-16 10:30:22.000000 eurmlsdk-0.0.905/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-16 10:30:22.000000 eurmlsdk-0.0.905/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-16 10:30:22.143050 eurmlsdk-0.0.905/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      847 2024-05-16 10:29:30.000000 eurmlsdk-0.0.905/setup.py
```

### Comparing `eurmlsdk-0.0.904/eurmlsdk/__main__.py` & `eurmlsdk-0.0.905/eurmlsdk/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,35 +10,35 @@
 
 def list_commands():
     print("Available commands in eurmlsdk package are:")
     print("  deploy <model type> <model path> <hostname> <username> <password> : Uploads the model file and executes remote script")
     print("  help | --h                                           : Lists all commands available in eurmlsdk package")
     print("  predict <model path> <dataset path>                  : Predicts the labels and saves the predicted result")
     print("  validate <task> <model path>                         : Validates the model and returns the metrics using default dataset")
+    print("  pt-predict <model name>                              : Predicts the labels and prints the predicted results")
+    print("  pt-list-model                                        : Lists all the pytorch models available")
+    print("  pt-validate <model name>                             : Validates the model and prints the metrics")
     print(" ")
-    print("pytorch commands")
-    print("pt-predict <modelname>                                 : Predicts the labels and prints the predicted results")
-    print("pt-list-model                                          : list all the pytorch models available")
     print("Options:")
     print(" <dataset path> : Image or Video path")
     print(" <hostname>     : Remote Server hostname")
     print(" <model path>   : Model file path")
     print(" <model type>   : Model type - 'yolo' or 'pt'")
     print(" <password>     : Remote Server password")
     print(" <task>         : Validation task - 'seg' or 'pose' or 'detect' or 'classify'")
     print(" <username>     : Remote Server username")
 
 def main():
-    commands_list = ['deploy','help','--h','predict','validate', 'pt-predict', 'pt-validate']
+    commands_list = ['deploy','help','--h','predict','validate', 'pt-predict', 'pt-validate', 'pt-list-model']
     try:
         argLen = len(argv)
         if argLen == 1:
             print("Model Zoo SDK")
             print("Package name: eurmlsdk")
-            print("Version: 0.0.902")
+            print("Version: 0.0.905")
             print("Run 'eurmlsdk help' or eurmlsdk --h to find the list of commands.")
             exit()
 
         command = argv[1]
         if command not in commands_list:
             print("Unknown command. Please find the list of commands")
             list_commands()
```

### Comparing `eurmlsdk-0.0.904/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.905/eurmlsdk/eur_sdk.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.904/eurmlsdk/pytorch.py` & `eurmlsdk-0.0.905/eurmlsdk/pytorch.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.904/setup.py` & `eurmlsdk-0.0.905/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.904',
+    version='0.0.905',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
```

