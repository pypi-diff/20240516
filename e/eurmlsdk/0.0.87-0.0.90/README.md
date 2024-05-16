# Comparing `tmp/eurmlsdk-0.0.87.tar.gz` & `tmp/eurmlsdk-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eurmlsdk-0.0.87.tar", last modified: Wed May 15 13:11:30 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.90.tar", last modified: Thu May 16 05:35:19 2024, max compression
```

## Comparing `eurmlsdk-0.0.87.tar` & `eurmlsdk-0.0.90.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.87/README.md
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.87/MANIFEST.in
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      335 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      102 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      846 2024-05-15 13:11:27.000000 eurmlsdk-0.0.87/setup.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.87/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/PKG-INFO
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-15 13:11:30.000000 eurmlsdk-0.0.87/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5642 2024-05-15 13:11:22.000000 eurmlsdk-0.0.87/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     9540 2024-05-15 12:55:17.000000 eurmlsdk-0.0.87/eurmlsdk/eur_sdk.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     1217 2024-05-14 11:25:38.000000 eurmlsdk-0.0.87/eurmlsdk/yolo.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3648 2024-05-15 13:10:51.000000 eurmlsdk-0.0.87/eurmlsdk/pytorch.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       33 2024-05-14 11:25:38.000000 eurmlsdk-0.0.87/eurmlsdk/__init__.py
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-16 05:35:19.506616 eurmlsdk-0.0.90/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       16 2024-05-08 10:50:34.000000 eurmlsdk-0.0.90/LICENSE.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-05-08 10:50:34.000000 eurmlsdk-0.0.90/MANIFEST.in
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      612 2024-05-16 05:35:19.506616 eurmlsdk-0.0.90/PKG-INFO
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       10 2024-05-08 10:50:34.000000 eurmlsdk-0.0.90/README.md
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-16 05:35:19.506616 eurmlsdk-0.0.90/eurmlsdk/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       33 2024-05-16 04:56:10.000000 eurmlsdk-0.0.90/eurmlsdk/__init__.py
+-rw-r--r--   0 surajram  (1000) surajram  (1000)     5497 2024-05-16 04:56:10.000000 eurmlsdk-0.0.90/eurmlsdk/__main__.py
+-rw-r--r--   0 surajram  (1000) surajram  (1000)     9540 2024-05-16 04:56:10.000000 eurmlsdk-0.0.90/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 surajram  (1000) surajram  (1000)     4007 2024-05-16 04:56:10.000000 eurmlsdk-0.0.90/eurmlsdk/pytorch.py
+-rw-r--r--   0 surajram  (1000) surajram  (1000)     1217 2024-05-16 04:56:10.000000 eurmlsdk-0.0.90/eurmlsdk/yolo.py
+drwxr-xr-x   0 surajram  (1000) surajram  (1000)        0 2024-05-16 05:35:19.506616 eurmlsdk-0.0.90/eurmlsdk.egg-info/
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      612 2024-05-16 05:35:19.000000 eurmlsdk-0.0.90/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      335 2024-05-16 05:35:19.000000 eurmlsdk-0.0.90/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)        1 2024-05-16 05:35:19.000000 eurmlsdk-0.0.90/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       52 2024-05-16 05:35:19.000000 eurmlsdk-0.0.90/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      102 2024-05-16 05:35:19.000000 eurmlsdk-0.0.90/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)        9 2024-05-16 05:35:19.000000 eurmlsdk-0.0.90/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 surajram  (1000) surajram  (1000)       38 2024-05-16 05:35:19.506616 eurmlsdk-0.0.90/setup.cfg
+-rw-r--r--   0 surajram  (1000) surajram  (1000)      846 2024-05-16 05:35:09.000000 eurmlsdk-0.0.90/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `eurmlsdk-0.0.87/setup.py` & `eurmlsdk-0.0.90/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.87',
+    version='0.0.90',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
```

### Comparing `eurmlsdk-0.0.87/eurmlsdk/__main__.py` & `eurmlsdk-0.0.90/eurmlsdk/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 logging.getLogger('tensorflow').setLevel(logging.ERROR)  # Suppress TensorFlow warning logs
 logging.getLogger('tensorflow.compiler.tf2tensorrt').setLevel(logging.ERROR)  # Suppress TensorFlow-TRT warning logs
 
 def list_commands():
     print("Available commands in eurmlsdk package are:")
     print("  deploy <model type> <model path> <hostname> <username> <password> : Uploads the model file and executes remote script")
     print("  help | --h                                           : Lists all commands available in eurmlsdk package")
-    print("  predict <model path> <dataset path>                  : Predicts the labels and saves the predicted result using yolo model")
-    print("  validate <task> <model path>                         : Validates the model and returns the metrics using default dataset using yolo model")
-    print("  pt-predict <model path>                              : Predicts the labels and saves the predicted result using Pytorch model")
-    print("  pt-validate <model path>                             : Validates the model and returns the metrics using default dataset using Pytorch model")
+    print("  predict <model path> <dataset path>                  : Predicts the labels and saves the predicted result")
+    print("  validate <task> <model path>                         : Validates the model and returns the metrics using default dataset")
     print(" ")
     print("Options:")
     print(" <dataset path> : Image or Video path")
     print(" <hostname>     : Remote Server hostname")
     print(" <model path>   : Model file path")
     print(" <model type>   : Model type - 'yolo' or 'pt'")
     print(" <password>     : Remote Server password")
@@ -29,15 +27,15 @@
 def main():
     commands_list = ['deploy','help','--h','predict','validate', 'pt-predict', 'pt-validate']
     try:
         argLen = len(argv)
         if argLen == 1:
             print("Model Zoo SDK")
             print("Package name: eurmlsdk")
-            print("Version: 0.0.87")
+            print("Version: 0.0.84")
             print("Run 'eurmlsdk help' or eurmlsdk --h to find the list of commands.")
             exit()
 
         command = argv[1]
         if command not in commands_list:
             print("Unknown command. Please find the list of commands")
             list_commands()
@@ -75,30 +73,32 @@
             predictData = argv[3]
             yoloSDK = ModelYolo()
             yoloSDK.predict_model(modelPath, predictData)
 
         elif command == "pt-predict":
             if argLen <3 :
                 print("Missing required arguments")
-                print("<model_path>")
+                print("<model_path> <dataset_path>")
                 exit(1)
             else:
                 model_path = argv[2]
                 pyTorchSDK = ModelPytorch()
-                pyTorchSDK.predict_model(model_path)
+                class_result = pyTorchSDK.predict_model(model_path)
+                pyTorchSDK.get_predicted_results(class_result)
 
         elif command == "pt-validate":
             if argLen <3 :
                 print("Missing required arguments")
-                print("<model_path>")
+                print("<model_path> <dataset_path>")
                 exit(1)
             else:
                 model_path = argv[2]
                 pyTorchSDK = ModelPytorch()
-                pyTorchSDK.validate_model(model_path)
+                validate_result = pyTorchSDK.validate_model(model_path)
+                print("Validation result", validate_result)
 
         elif command == "deploy":
             if argLen < 7:
                 print("Missing required arguments")
                 print("Usage: eurmlsdk deploy <model type> <model path> <hostname> <username> <password>")
                 exit(1)
             if len(argv) > 7:
```

### Comparing `eurmlsdk-0.0.87/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.90/eurmlsdk/eur_sdk.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.87/eurmlsdk/yolo.py` & `eurmlsdk-0.0.90/eurmlsdk/yolo.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.87/eurmlsdk/pytorch.py` & `eurmlsdk-0.0.90/eurmlsdk/pytorch.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,23 @@
                 _, predicted = torch.max(output, 1)
                 total += labels.size(0)
                 correct += (predicted == labels).sum().item()
 
         accuracy = correct/total
         return accuracy
     
+    def get_predicted_results(self, results):
+        list_predicted_set = ['airplane', 'automobile', 'bird', 'cat', 'deer', 'dog', 'frog', 'horse', 'ship', 'truck']
+        predictied_values = list(map(int, results))
+        print(predictied_values)
+        for res in predictied_values:
+            print("Predicted_result :", list_predicted_set[res]) 
+
+
+ 
 
 
     # def loadModel(self, model_path):
     #     modelFile = self.get_model(model_path)
     #     if modelFile != "":
     #         print("model loading is yet to start")
     #         model = torch.hub.load(model_path)
```

