# Comparing `tmp/cloudcomponents.cdk-pull-request-check-2.3.0.tar.gz` & `tmp/cloudcomponents.cdk-pull-request-check-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-pull-request-check-2.3.0.tar", last modified: Wed Apr 17 18:36:03 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-pull-request-check-2.4.0.tar", last modified: Thu May 16 19:32:59 2024, max compression
```

## Comparing `cloudcomponents.cdk-pull-request-check-2.3.0.tar` & `cloudcomponents.cdk-pull-request-check-2.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:03.950043 cloudcomponents.cdk-pull-request-check-2.3.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-04-17 18:36:00.000000 cloudcomponents.cdk-pull-request-check-2.3.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:36:00.000000 cloudcomponents.cdk-pull-request-check-2.3.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     5907 2024-04-17 18:36:03.949779 cloudcomponents.cdk-pull-request-check-2.3.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     5051 2024-04-17 18:36:00.000000 cloudcomponents.cdk-pull-request-check-2.3.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:36:00.000000 cloudcomponents.cdk-pull-request-check-2.3.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:36:03.950090 cloudcomponents.cdk-pull-request-check-2.3.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1806 2024-04-17 18:36:00.000000 cloudcomponents.cdk-pull-request-check-2.3.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:03.946198 cloudcomponents.cdk-pull-request-check-2.3.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:03.946258 cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:03.948226 cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents/cdk_pull_request_check/
--rw-r--r--   0 hupe       (501) staff       (20)    38461 2024-04-17 18:36:00.000000 cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents/cdk_pull_request_check/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:03.948538 cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents/cdk_pull_request_check/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      441 2024-04-17 18:36:00.000000 cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents/cdk_pull_request_check/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)  1286450 2024-04-17 18:36:00.000000 cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents/cdk_pull_request_check/_jsii/cdk-pull-request-check@2.3.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:36:00.000000 cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents/cdk_pull_request_check/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:03.947882 cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents.cdk_pull_request_check.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     5907 2024-04-17 18:36:03.000000 cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents.cdk_pull_request_check.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      637 2024-04-17 18:36:03.000000 cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents.cdk_pull_request_check.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:36:03.000000 cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents.cdk_pull_request_check.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-04-17 18:36:03.000000 cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents.cdk_pull_request_check.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:36:03.000000 cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents.cdk_pull_request_check.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.601752 cloudcomponents.cdk-pull-request-check-2.4.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-05-16 19:32:55.000000 cloudcomponents.cdk-pull-request-check-2.4.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-05-16 19:32:55.000000 cloudcomponents.cdk-pull-request-check-2.4.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     5907 2024-05-16 19:32:59.601300 cloudcomponents.cdk-pull-request-check-2.4.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     5051 2024-05-16 19:32:55.000000 cloudcomponents.cdk-pull-request-check-2.4.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-05-16 19:32:55.000000 cloudcomponents.cdk-pull-request-check-2.4.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-05-16 19:32:59.601795 cloudcomponents.cdk-pull-request-check-2.4.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1806 2024-05-16 19:32:55.000000 cloudcomponents.cdk-pull-request-check-2.4.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.597686 cloudcomponents.cdk-pull-request-check-2.4.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.597766 cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.600625 cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents/cdk_pull_request_check/
+-rw-r--r--   0 hupe       (501) staff       (20)    38461 2024-05-16 19:32:55.000000 cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents/cdk_pull_request_check/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.600982 cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents/cdk_pull_request_check/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      441 2024-05-16 19:32:55.000000 cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents/cdk_pull_request_check/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)    84969 2024-05-16 19:32:55.000000 cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents/cdk_pull_request_check/_jsii/cdk-pull-request-check@2.4.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:32:55.000000 cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents/cdk_pull_request_check/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.600226 cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents.cdk_pull_request_check.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     5907 2024-05-16 19:32:59.000000 cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents.cdk_pull_request_check.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      637 2024-05-16 19:32:59.000000 cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents.cdk_pull_request_check.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:32:59.000000 cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents.cdk_pull_request_check.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-05-16 19:32:59.000000 cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents.cdk_pull_request_check.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-05-16 19:32:59.000000 cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents.cdk_pull_request_check.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-pull-request-check-2.3.0/LICENSE` & `cloudcomponents.cdk-pull-request-check-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-pull-request-check-2.3.0/PKG-INFO` & `cloudcomponents.cdk-pull-request-check-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-pull-request-check
-Version: 2.3.0
+Version: 2.4.0
 Summary: Cdk component that automatically check pull requests
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-pull-request-check-2.3.0/README.md` & `cloudcomponents.cdk-pull-request-check-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-pull-request-check-2.3.0/setup.py` & `cloudcomponents.cdk-pull-request-check-2.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-pull-request-check",
-    "version": "2.3.0",
+    "version": "2.4.0",
     "description": "Cdk component that automatically check pull requests",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cloudcomponents.cdk_pull_request_check",
         "cloudcomponents.cdk_pull_request_check._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_pull_request_check._jsii": [
-            "cdk-pull-request-check@2.3.0.jsii.tgz"
+            "cdk-pull-request-check@2.4.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_pull_request_check": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.28.0, <3.0.0",
-        "constructs>=10.0.41, <11.0.0",
+        "aws-cdk-lib>=2.141.0, <3.0.0",
+        "constructs>=10.3.0, <11.0.0",
         "jsii>=1.95.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents/cdk_pull_request_check/__init__.py` & `cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents/cdk_pull_request_check/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents.cdk_pull_request_check.egg-info/PKG-INFO` & `cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents.cdk_pull_request_check.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-pull-request-check
-Version: 2.3.0
+Version: 2.4.0
 Summary: Cdk component that automatically check pull requests
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-pull-request-check-2.3.0/src/cloudcomponents.cdk_pull_request_check.egg-info/SOURCES.txt` & `cloudcomponents.cdk-pull-request-check-2.4.0/src/cloudcomponents.cdk_pull_request_check.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_pull_request_check.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_pull_request_check.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_pull_request_check.egg-info/requires.txt
 src/cloudcomponents.cdk_pull_request_check.egg-info/top_level.txt
 src/cloudcomponents/cdk_pull_request_check/__init__.py
 src/cloudcomponents/cdk_pull_request_check/py.typed
 src/cloudcomponents/cdk_pull_request_check/_jsii/__init__.py
-src/cloudcomponents/cdk_pull_request_check/_jsii/cdk-pull-request-check@2.3.0.jsii.tgz
+src/cloudcomponents/cdk_pull_request_check/_jsii/cdk-pull-request-check@2.4.0.jsii.tgz
```

