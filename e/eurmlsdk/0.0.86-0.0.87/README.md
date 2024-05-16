# Comparing `tmp/eurmlsdk-0.0.86.tar.gz` & `tmp/eurmlsdk-0.0.87.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eurmlsdk-0.0.86.tar", last modified: Wed May 15 13:04:23 2024, max compression
+gzip compressed data, was "dist/eurmlsdk-0.0.87.tar", last modified: Wed May 15 13:11:30 2024, max compression
```

## Comparing `eurmlsdk-0.0.86.tar` & `eurmlsdk-0.0.87.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.86/README.md
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.86/MANIFEST.in
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      846 2024-05-15 13:04:04.000000 eurmlsdk-0.0.86/setup.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.86/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/PKG-INFO
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 13:04:23.000000 eurmlsdk-0.0.86/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5642 2024-05-15 13:04:09.000000 eurmlsdk-0.0.86/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.0.86/eurmlsdk/eur_sdk.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1217 2024-05-14 11:25:38.000000 eurmlsdk-0.0.86/eurmlsdk/yolo.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3648 2024-05-15 12:55:17.000000 eurmlsdk-0.0.86/eurmlsdk/pytorch.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.0.86/eurmlsdk/__init__.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.87/README.md
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.87/MANIFEST.in
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      846 2024-05-15 13:11:27.000000 eurmlsdk-0.0.87/setup.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.87/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/PKG-INFO
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5642 2024-05-15 13:11:22.000000 eurmlsdk-0.0.87/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.0.87/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1217 2024-05-14 11:25:38.000000 eurmlsdk-0.0.87/eurmlsdk/yolo.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3648 2024-05-15 13:10:51.000000 eurmlsdk-0.0.87/eurmlsdk/pytorch.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.0.87/eurmlsdk/__init__.py
```

### Comparing `eurmlsdk-0.0.86/setup.py` & `eurmlsdk-0.0.87/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.86',
+    version='0.0.87',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
```

### Comparing `eurmlsdk-0.0.86/eurmlsdk/__main__.py` & `eurmlsdk-0.0.87/eurmlsdk/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def main():
     commands_list = ['deploy','help','--h','predict','validate', 'pt-predict', 'pt-validate']
     try:
         argLen = len(argv)
         if argLen == 1:
             print("Model Zoo SDK")
             print("Package name: eurmlsdk")
-            print("Version: 0.0.86")
+            print("Version: 0.0.87")
             print("Run 'eurmlsdk help' or eurmlsdk --h to find the list of commands.")
             exit()
 
         command = argv[1]
         if command not in commands_list:
             print("Unknown command. Please find the list of commands")
             list_commands()
```

### Comparing `eurmlsdk-0.0.86/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.87/eurmlsdk/eur_sdk.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.86/eurmlsdk/yolo.py` & `eurmlsdk-0.0.87/eurmlsdk/yolo.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.86/eurmlsdk/pytorch.py` & `eurmlsdk-0.0.87/eurmlsdk/pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from torchvision.utils import make_grid
 import matplotlib.pyplot as plt
 import numpy as np
 from .eur_sdk import EurBaseSDK
 
 class ModelPytorch(EurBaseSDK):
     def load_model(self, model_path):
-        device = torch.device("cuda" if torch.cuba.is_available() else "cpu")
+        device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         model = timm.create_model(model_path, pretrained=True)
         save_path = 'resnet50.pth'
         torch.save(model.state_dict(), save_path)
         num_ftrs = model.fc.in_features
         model.fc = nn.Linear(num_ftrs, 1000)
         model.load_state_dict(torch.load(save_path, map_location=device))
         model.to(device)
```

