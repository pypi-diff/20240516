# Comparing `tmp/cryptonets_python_sdk-1.3.0.tar.gz` & `tmp/cryptonets_python_sdk-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptonets_python_sdk-1.3.0.tar", last modified: Wed May  8 07:24:50 2024, max compression
+gzip compressed data, was "cryptonets_python_sdk-1.3.1.tar", last modified: Thu May 16 12:14:05 2024, max compression
```

## Comparing `cryptonets_python_sdk-1.3.0.tar` & `cryptonets_python_sdk-1.3.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-08 07:24:50.708243 cryptonets_python_sdk-1.3.0/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.3.0/LICENSE
--rw-rw-r--   0 azam      (1000) azam      (1000)       28 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.3.0/MANIFEST.in
--rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-05-08 07:24:50.708243 cryptonets_python_sdk-1.3.0/PKG-INFO
--rw-rw-r--   0 azam      (1000) azam      (1000)     2511 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/README.md
--rw-rw-r--   0 azam      (1000) azam      (1000)       38 2024-05-08 07:24:50.708243 cryptonets_python_sdk-1.3.0/setup.cfg
--rw-rw-r--   0 azam      (1000) azam      (1000)     3798 2024-05-08 07:24:46.000000 cryptonets_python_sdk-1.3.0/setup.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-08 07:24:50.704243 cryptonets_python_sdk-1.3.0/src/
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-08 07:24:50.704243 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)    31186 2024-04-08 11:43:05.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/factor.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-08 07:24:50.704243 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/factor_modules/
--rw-rw-r--   0 azam      (1000) azam      (1000)    19933 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/factor_modules/FaceModule.py
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/factor_modules/__init__.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-08 07:24:50.704243 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/handler/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/handler/__init__.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-08 07:24:50.704243 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/handler/lib/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/handler/lib/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)    44596 2024-05-08 07:24:46.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/handler/nativeMethods.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-08 07:24:50.704243 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     3060 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/decorators.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     3383 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/messages.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-08 07:24:50.708243 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/result_objects/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/result_objects/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     3293 2024-04-08 11:44:23.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/result_objects/compareResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      664 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     2946 2024-03-20 07:33:12.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     1575 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     1463 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     2228 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     4476 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/utils.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-08 07:24:50.708243 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/settings/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/settings/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      239 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/settings/cacheType.py
--rw-rw-r--   0 azam      (1000) azam      (1000)    17214 2024-04-30 12:01:39.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/settings/configuration.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      298 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/settings/loggingLevel.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      113 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/settings/supportedPlatforms.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-08 07:24:50.704243 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk.egg-info/
--rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-05-08 07:24:50.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 azam      (1000) azam      (1000)     1544 2024-05-08 07:24:50.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 azam      (1000) azam      (1000)        1 2024-05-08 07:24:50.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 azam      (1000) azam      (1000)       48 2024-05-08 07:24:50.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk.egg-info/requires.txt
--rw-rw-r--   0 azam      (1000) azam      (1000)       22 2024-05-08 07:24:50.000000 cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-08 07:24:50.708243 cryptonets_python_sdk-1.3.0/tests/
--rw-rw-r--   0 azam      (1000) azam      (1000)    19957 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.3.0/tests/test.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     8913 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.0/tests/test_suite.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-16 12:14:05.798820 cryptonets_python_sdk-1.3.1/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.3.1/LICENSE
+-rw-rw-r--   0 azam      (1000) azam      (1000)       28 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.3.1/MANIFEST.in
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-05-16 12:14:05.798820 cryptonets_python_sdk-1.3.1/PKG-INFO
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2511 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/README.md
+-rw-rw-r--   0 azam      (1000) azam      (1000)       38 2024-05-16 12:14:05.798820 cryptonets_python_sdk-1.3.1/setup.cfg
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3798 2024-05-16 12:12:36.000000 cryptonets_python_sdk-1.3.1/setup.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-16 12:14:05.794819 cryptonets_python_sdk-1.3.1/src/
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-16 12:14:05.798820 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)    31186 2024-04-08 11:43:05.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/factor.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-16 12:14:05.798820 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/factor_modules/
+-rw-rw-r--   0 azam      (1000) azam      (1000)    19933 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/factor_modules/FaceModule.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/factor_modules/__init__.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-16 12:14:05.798820 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/handler/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/handler/__init__.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-16 12:14:05.798820 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/handler/lib/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/handler/lib/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)    45211 2024-05-16 12:12:36.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/handler/nativeMethods.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-16 12:14:05.798820 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3060 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/decorators.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3383 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/messages.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-16 12:14:05.798820 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/result_objects/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/result_objects/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3293 2024-04-08 11:44:23.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/result_objects/compareResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      664 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2946 2024-03-20 07:33:12.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     1575 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     1463 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2228 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     4476 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/utils.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-16 12:14:05.798820 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/settings/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/settings/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      239 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/settings/cacheType.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)    17417 2024-05-16 12:12:36.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/settings/configuration.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      298 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/settings/loggingLevel.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      113 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/settings/supportedPlatforms.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-16 12:14:05.798820 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk.egg-info/
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-05-16 12:14:05.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 azam      (1000) azam      (1000)     1544 2024-05-16 12:14:05.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 azam      (1000) azam      (1000)        1 2024-05-16 12:14:05.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 azam      (1000) azam      (1000)       48 2024-05-16 12:14:05.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk.egg-info/requires.txt
+-rw-rw-r--   0 azam      (1000) azam      (1000)       22 2024-05-16 12:14:05.000000 cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-16 12:14:05.798820 cryptonets_python_sdk-1.3.1/tests/
+-rw-rw-r--   0 azam      (1000) azam      (1000)    19957 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.3.1/tests/test.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     8913 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.1/tests/test_suite.py
```

### Comparing `cryptonets_python_sdk-1.3.0/PKG-INFO` & `cryptonets_python_sdk-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptonets_python_sdk
-Version: 1.3.0
+Version: 1.3.1
 Summary: Cryptonets SDK Library for Python
 Home-page: https://privateid.com/
 Author: Private Identity
 Author-email: support@private.id
 Project-URL: Bug Reports, https://github.com/prividentity/cryptonets-python-sdk/issues
 Project-URL: Source, https://github.com/prividentity/cryptonets-python-sdk
 Project-URL: Documentation, https://docs.private.id/cryptonets-python-sdk/index.html
```

### Comparing `cryptonets_python_sdk-1.3.0/README.md` & `cryptonets_python_sdk-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.0/setup.py` & `cryptonets_python_sdk-1.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 @author: Private Identity
 """
 NAME = "cryptonets_python_sdk"
 DESCRIPTION = "Cryptonets SDK Library for Python"
 AUTHOR = "Private Identity"
 AUTHOR_EMAIL = "support@private.id"
 URL = "https://privateid.com/"
-VERSION = "1.3.0"
+VERSION = "1.3.1"
 REQUIRES = ["numpy >= 1.21.0", "pillow >= 9.1.0","boto3","tqdm","exifread"]
 
 LONG_DESCRIPTION = ""
 if os.path.exists("./README.md"):
     with open("README.md", encoding="utf-8") as fp:
         LONG_DESCRIPTION = fp.read()
 setup(
```

### Comparing `cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/factor.py` & `cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/factor.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/factor_modules/FaceModule.py` & `cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/factor_modules/FaceModule.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/handler/nativeMethods.py` & `cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/handler/nativeMethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ..settings.cacheType import CacheType
 from ..settings.configuration import ConfigObject
 from ..settings.loggingLevel import LoggingLevel
 import boto3
 import botocore
 import tqdm
 import subprocess
+import platform
 class NativeMethods(object):
     def __init__(
         self,
         api_key: str,
         server_url: str,
         local_storage_path: str,
         logging_level: LoggingLevel,
@@ -44,15 +45,18 @@
         except Exception as e:
             print("Error ", e)
             sys.exit(1)
 
     def _check_and_download_files(self, system_os):
         required_files=[]
         if system_os == "Linux":
-            required_files=["lib_fhe.so","libtensorflow-lite.so"]
+            if platform.machine() in ["aarch64","arm"]:
+                required_files=["lib_fhe_arm64.so","libtensorflow-lite-arm64.so"]
+            else:
+                required_files=["lib_fhe.so","libtensorflow-lite.so"]
         elif system_os == "Windows":
             required_files=[]
         elif system_os == "Darwin":
             required_files=["libprivid_fhe_universal.dylib"]
         
        # Create an unauthenticated session
         session = boto3.Session()
@@ -74,18 +78,24 @@
 
             with tqdm.tqdm(total=file_size, unit='B', unit_scale=True, desc=file_name) as bar:
                 for chunk in response['Body'].iter_chunks(chunk_size=1024):
                     f.write(chunk)
                     bar.update(len(chunk))
 
     def _load_linux_libraries(self):
-        self._library_path = str(self._local_lib_path.joinpath("lib_fhe.so").resolve())
-        self._library_path_2 = str(self._local_lib_path.joinpath("libtensorflow-lite.so").resolve())
-        ctypes.CDLL(self._library_path_2, mode=1)
-        self._spl_so_face = ctypes.CDLL(self._library_path)
+        if platform.machine() in ["aarch64","arm"]:
+                self._library_path = str(self._local_lib_path.joinpath("lib_fhe_arm64.so").resolve())
+                self._library_path_2 = str(self._local_lib_path.joinpath("libtensorflow-lite-arm64.so").resolve())
+                ctypes.CDLL(self._library_path_2, mode=1)
+                self._spl_so_face = ctypes.CDLL(self._library_path)
+        else:
+                self._library_path = str(self._local_lib_path.joinpath("lib_fhe.so").resolve())
+                self._library_path_2 = str(self._local_lib_path.joinpath("libtensorflow-lite.so").resolve())
+                ctypes.CDLL(self._library_path_2, mode=1)
+                self._spl_so_face = ctypes.CDLL(self._library_path)
 
     def _load_windows_libraries(self):
         self._library_path = str(self._local_lib_path.joinpath("privid_fhe.dll").resolve())
         self._library_path_2 = str(self._local_lib_path.joinpath("libssl-1_1-x64.dll").resolve())
         self._library_path_3 = str(self._local_lib_path.joinpath("libcrypto-1_1-x64.dll").resolve())
         ctypes.CDLL(self._library_path_3, mode=1)
         ctypes.CDLL(self._library_path_2, mode=1)
@@ -669,15 +679,15 @@
 
             rim_height, rim_width, _ = right_image.shape
             rim_size = (
                 right_image.shape[1] * right_image.shape[0] * right_image.shape[2]
             )
             p_buffer_result = c_char_p()
             p_buffer_result_length = c_int()
-            config_object_default = {"face_thresholds_rem_bad_emb_default": 1.275, "face_thresholds_med": 1.275,"conf_score_thr_enroll":0.2}
+            config_object_default = {"face_thresholds_rem_bad_emb_default": 1.24, "face_thresholds_med": 1.24,"conf_score_thr_enroll":0.2}
 
             if config_object and hasattr(config_object, 'get_config_param') and config_object.get_config_param():
                 config_param_str = config_object.get_config_param()
                 config_from_object = json.loads(config_param_str)
                 for key, value in config_object_default.items():
                     if key not in config_from_object:
                         config_from_object[key] = value
```

### Comparing `cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/decorators.py` & `cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/decorators.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/messages.py` & `cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/messages.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/result_objects/compareResult.py` & `cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/result_objects/compareResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py` & `cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py` & `cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py` & `cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py` & `cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py` & `cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/helper/utils.py` & `cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/helper/utils.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk/settings/configuration.py` & `cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk/settings/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,16 @@
     DOC_FRONT_RESERVATION_CALLS = "document_model"
     DOC_BACK_RESERVATION_CALLS = "document_model"
     COMPARE_RESERVATION_CALLS = "compare_files"
     FACE_RESERVATION_CALLS = "faces"
     ESTIMATE_AGE_RESERVATION_CALLS = "estimate_age"
     FACE_ISO_RESERVATION_CALLS = "face_iso"
     THRESHOLD_HIGH_VERTICAL="threshold_high_vertical_enroll"
+    DOCUMENT_AUTO_ROTATION = "document_auto_rotation"
+    
 
 
 class ParameterValidator:
     def __init__(self):
         self.__parameter = {}
         self.__populate_parameters()
         self.__billing_reservation_parameters = [
@@ -318,14 +320,17 @@
 
         self.__parameter[PARAMETERS.COLLECTION_NAME] = self.Parameter(
             name=PARAMETERS.COLLECTION_NAME, _type="ANY")
 
         self.__parameter[PARAMETERS.K] = self.Parameter(
             name=PARAMETERS.K,_type="NUMBER", min_value=1, max_value=100)
 
+        self.__parameter[PARAMETERS.DOCUMENT_AUTO_ROTATION] = self.Parameter(
+            name=PARAMETERS.DOCUMENT_AUTO_ROTATION,_type="BOOL")
+
     def validate(self, key, value):
         return self.__parameter[key].validate(value)
 
     def is_billing_parameter(self, key):
         return key in self.__billing_reservation_parameters
 
     class Parameter:
```

### Comparing `cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk.egg-info/PKG-INFO` & `cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptonets-python-sdk
-Version: 1.3.0
+Version: 1.3.1
 Summary: Cryptonets SDK Library for Python
 Home-page: https://privateid.com/
 Author: Private Identity
 Author-email: support@private.id
 Project-URL: Bug Reports, https://github.com/prividentity/cryptonets-python-sdk/issues
 Project-URL: Source, https://github.com/prividentity/cryptonets-python-sdk
 Project-URL: Documentation, https://docs.private.id/cryptonets-python-sdk/index.html
```

### Comparing `cryptonets_python_sdk-1.3.0/src/cryptonets_python_sdk.egg-info/SOURCES.txt` & `cryptonets_python_sdk-1.3.1/src/cryptonets_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.0/tests/test.py` & `cryptonets_python_sdk-1.3.1/tests/test.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.0/tests/test_suite.py` & `cryptonets_python_sdk-1.3.1/tests/test_suite.py`

 * *Files identical despite different names*

