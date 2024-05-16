# Comparing `tmp/cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0.tar.gz` & `tmp/cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0.tar", last modified: Wed Apr 17 18:35:46 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0.tar", last modified: Thu May 16 19:28:14 2024, max compression
```

## Comparing `cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0.tar` & `cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.073116 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1077 2024-04-17 18:35:41.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:35:41.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     4064 2024-04-17 18:35:46.072771 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     3205 2024-04-17 18:35:41.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:35:41.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:35:46.073160 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1829 2024-04-17 18:35:41.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.068831 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.068901 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.070987 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents/cdk_lambda_at_edge_pattern/
--rw-r--r--   0 hupe       (501) staff       (20)    32693 2024-04-17 18:35:41.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents/cdk_lambda_at_edge_pattern/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.071328 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents/cdk_lambda_at_edge_pattern/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      449 2024-04-17 18:35:41.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents/cdk_lambda_at_edge_pattern/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)  1732783 2024-04-17 18:35:41.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents/cdk_lambda_at_edge_pattern/_jsii/cdk-lambda-at-edge-pattern@2.3.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:41.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents/cdk_lambda_at_edge_pattern/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.070627 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     4064 2024-04-17 18:35:46.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      677 2024-04-17 18:35:46.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:46.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-04-17 18:35:46.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:35:46.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.290542 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1077 2024-05-16 19:28:09.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-05-16 19:28:09.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     4064 2024-05-16 19:28:14.290223 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     3205 2024-05-16 19:28:09.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-05-16 19:28:09.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-05-16 19:28:14.290616 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1829 2024-05-16 19:28:09.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.286385 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.286471 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.289224 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents/cdk_lambda_at_edge_pattern/
+-rw-r--r--   0 hupe       (501) staff       (20)    32693 2024-05-16 19:28:09.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents/cdk_lambda_at_edge_pattern/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.289534 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents/cdk_lambda_at_edge_pattern/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      449 2024-05-16 19:28:09.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents/cdk_lambda_at_edge_pattern/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)   528278 2024-05-16 19:28:09.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents/cdk_lambda_at_edge_pattern/_jsii/cdk-lambda-at-edge-pattern@2.4.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:28:09.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents/cdk_lambda_at_edge_pattern/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.288849 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     4064 2024-05-16 19:28:14.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      677 2024-05-16 19:28:14.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:28:14.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-05-16 19:28:14.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-05-16 19:28:14.000000 cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/LICENSE` & `cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/PKG-INFO` & `cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-lambda-at-edge-pattern
-Version: 2.3.0
+Version: 2.4.0
 Summary: CDK Constructs for Lambda@Edge pattern: HttpHeaders
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/README.md` & `cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/setup.py` & `cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-lambda-at-edge-pattern",
-    "version": "2.3.0",
+    "version": "2.4.0",
     "description": "CDK Constructs for Lambda@Edge pattern: HttpHeaders",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cloudcomponents.cdk_lambda_at_edge_pattern",
         "cloudcomponents.cdk_lambda_at_edge_pattern._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_lambda_at_edge_pattern._jsii": [
-            "cdk-lambda-at-edge-pattern@2.3.0.jsii.tgz"
+            "cdk-lambda-at-edge-pattern@2.4.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_lambda_at_edge_pattern": [
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

### Comparing `cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents/cdk_lambda_at_edge_pattern/__init__.py` & `cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents/cdk_lambda_at_edge_pattern/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/PKG-INFO` & `cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-lambda-at-edge-pattern
-Version: 2.3.0
+Version: 2.4.0
 Summary: CDK Constructs for Lambda@Edge pattern: HttpHeaders
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-lambda-at-edge-pattern-2.3.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/SOURCES.txt` & `cloudcomponents.cdk-lambda-at-edge-pattern-2.4.0/src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/requires.txt
 src/cloudcomponents.cdk_lambda_at_edge_pattern.egg-info/top_level.txt
 src/cloudcomponents/cdk_lambda_at_edge_pattern/__init__.py
 src/cloudcomponents/cdk_lambda_at_edge_pattern/py.typed
 src/cloudcomponents/cdk_lambda_at_edge_pattern/_jsii/__init__.py
-src/cloudcomponents/cdk_lambda_at_edge_pattern/_jsii/cdk-lambda-at-edge-pattern@2.3.0.jsii.tgz
+src/cloudcomponents/cdk_lambda_at_edge_pattern/_jsii/cdk-lambda-at-edge-pattern@2.4.0.jsii.tgz
```

