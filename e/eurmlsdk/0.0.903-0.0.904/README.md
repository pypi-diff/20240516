# Comparing `tmp/eurmlsdk-0.0.903.tar.gz` & `tmp/eurmlsdk-0.0.904.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.903.tar", last modified: Thu May 16 08:20:53 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.904.tar", last modified: Thu May 16 10:23:22 2024, max compression
```

## Comparing `eurmlsdk-0.0.903.tar` & `eurmlsdk-0.0.904.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 08:20:53.823050 eurmlsdk-0.0.903/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.903/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.903/MANIFEST.in
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 08:20:53.823050 eurmlsdk-0.0.903/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.903/README.md
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 08:20:53.823050 eurmlsdk-0.0.903/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.0.903/eurmlsdk/__init__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5498 2024-05-16 07:22:12.000000 eurmlsdk-0.0.903/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.0.903/eurmlsdk/eur_sdk.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4036 2024-05-16 07:32:23.000000 eurmlsdk-0.0.903/eurmlsdk/pytorch.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     2032 2024-05-16 08:17:25.000000 eurmlsdk-0.0.903/eurmlsdk/yolo.py
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 08:20:53.823050 eurmlsdk-0.0.903/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 08:20:53.000000 eurmlsdk-0.0.903/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-16 08:20:53.000000 eurmlsdk-0.0.903/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-16 08:20:53.000000 eurmlsdk-0.0.903/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-16 08:20:53.000000 eurmlsdk-0.0.903/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-16 08:20:53.000000 eurmlsdk-0.0.903/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-16 08:20:53.000000 eurmlsdk-0.0.903/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-16 08:20:53.823050 eurmlsdk-0.0.903/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      847 2024-05-16 08:20:20.000000 eurmlsdk-0.0.903/setup.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 10:23:22.663050 eurmlsdk-0.0.904/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.904/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.904/MANIFEST.in
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 10:23:22.653050 eurmlsdk-0.0.904/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.904/README.md
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 10:23:22.653050 eurmlsdk-0.0.904/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.0.904/eurmlsdk/__init__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     6150 2024-05-16 10:22:37.000000 eurmlsdk-0.0.904/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.0.904/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     4036 2024-05-16 07:32:23.000000 eurmlsdk-0.0.904/eurmlsdk/pytorch.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     2032 2024-05-16 08:17:25.000000 eurmlsdk-0.0.904/eurmlsdk/yolo.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-16 10:23:22.653050 eurmlsdk-0.0.904/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      384 2024-05-16 10:23:22.000000 eurmlsdk-0.0.904/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-16 10:23:22.000000 eurmlsdk-0.0.904/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-16 10:23:22.000000 eurmlsdk-0.0.904/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-16 10:23:22.000000 eurmlsdk-0.0.904/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-16 10:23:22.000000 eurmlsdk-0.0.904/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-16 10:23:22.000000 eurmlsdk-0.0.904/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-16 10:23:22.663050 eurmlsdk-0.0.904/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      847 2024-05-16 10:22:56.000000 eurmlsdk-0.0.904/setup.py
```

### Comparing `eurmlsdk-0.0.903/eurmlsdk/__main__.py` & `eurmlsdk-0.0.904/eurmlsdk/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 def list_commands():
     print("Available commands in eurmlsdk package are:")
     print("  deploy <model type> <model path> <hostname> <username> <password> : Uploads the model file and executes remote script")
     print("  help | --h                                           : Lists all commands available in eurmlsdk package")
     print("  predict <model path> <dataset path>                  : Predicts the labels and saves the predicted result")
     print("  validate <task> <model path>                         : Validates the model and returns the metrics using default dataset")
     print(" ")
+    print("pytorch commands")
+    print("pt-predict <modelname>                                 : Predicts the labels and prints the predicted results")
+    print("pt-list-model                                          : list all the pytorch models available")
     print("Options:")
     print(" <dataset path> : Image or Video path")
     print(" <hostname>     : Remote Server hostname")
     print(" <model path>   : Model file path")
     print(" <model type>   : Model type - 'yolo' or 'pt'")
     print(" <password>     : Remote Server password")
     print(" <task>         : Validation task - 'seg' or 'pose' or 'detect' or 'classify'")
@@ -39,14 +42,20 @@
         if command not in commands_list:
             print("Unknown command. Please find the list of commands")
             list_commands()
             exit()
 
         if command == "help" or command == "--h":
             list_commands()
+
+        elif command =="pt-list-model":
+            model_list = ['AlexNet','ConvNeXt','DenseNet','EfficientNet','EfficientNetV2','GoogLeNet','Inception V3','MaxVit','MNASNet','MobileNet V2', 'MobileNet V3','RegNet','ResNet','ResNeXt','ShuffleNet V2','SqueezeNet','SwinTransformer','VGG','VisionTransformer','Wide ResNet']
+            for model in model_list:
+                print(model)
+
         elif command == "validate":
             taskList = ["seg", "pose", "classify", "detect"]
             if argLen < 4:
                 print("Missing required arguments")
                 print("Usage: eurmlsdk validate <task> <model path>")
                 exit(1)
             if argLen > 4:
```

### Comparing `eurmlsdk-0.0.903/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.904/eurmlsdk/eur_sdk.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.903/eurmlsdk/pytorch.py` & `eurmlsdk-0.0.904/eurmlsdk/pytorch.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.903/eurmlsdk/yolo.py` & `eurmlsdk-0.0.904/eurmlsdk/yolo.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.903/setup.py` & `eurmlsdk-0.0.904/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.903',
+    version='0.0.904',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
```

