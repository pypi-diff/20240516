# Comparing `tmp/cloudcomponents.cdk-cloudfront-authorization-2.3.0.tar.gz` & `tmp/cloudcomponents.cdk-cloudfront-authorization-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-cloudfront-authorization-2.3.0.tar", last modified: Wed Apr 17 18:36:26 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-cloudfront-authorization-2.4.0.tar", last modified: Thu May 16 19:33:27 2024, max compression
```

## Comparing `cloudcomponents.cdk-cloudfront-authorization-2.3.0.tar` & `cloudcomponents.cdk-cloudfront-authorization-2.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:26.438315 cloudcomponents.cdk-cloudfront-authorization-2.3.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1077 2024-04-17 18:36:23.000000 cloudcomponents.cdk-cloudfront-authorization-2.3.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:36:23.000000 cloudcomponents.cdk-cloudfront-authorization-2.3.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     5310 2024-04-17 18:36:26.438043 cloudcomponents.cdk-cloudfront-authorization-2.3.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     4444 2024-04-17 18:36:23.000000 cloudcomponents.cdk-cloudfront-authorization-2.3.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:36:23.000000 cloudcomponents.cdk-cloudfront-authorization-2.3.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:36:26.438359 cloudcomponents.cdk-cloudfront-authorization-2.3.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1915 2024-04-17 18:36:23.000000 cloudcomponents.cdk-cloudfront-authorization-2.3.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:26.434434 cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:26.434490 cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:26.436302 cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents/cdk_cloudfront_authorization/
--rw-r--r--   0 hupe       (501) staff       (20)   220092 2024-04-17 18:36:23.000000 cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents/cdk_cloudfront_authorization/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:26.436580 cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents/cdk_cloudfront_authorization/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      509 2024-04-17 18:36:23.000000 cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents/cdk_cloudfront_authorization/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)  2339400 2024-04-17 18:36:23.000000 cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents/cdk_cloudfront_authorization/_jsii/cdk-cloudfront-authorization@2.3.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:36:23.000000 cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents/cdk_cloudfront_authorization/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:26.435881 cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     5310 2024-04-17 18:36:26.000000 cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      697 2024-04-17 18:36:26.000000 cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:36:26.000000 cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      169 2024-04-17 18:36:26.000000 cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:36:26.000000 cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:27.815112 cloudcomponents.cdk-cloudfront-authorization-2.4.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1077 2024-05-16 19:33:24.000000 cloudcomponents.cdk-cloudfront-authorization-2.4.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-05-16 19:33:24.000000 cloudcomponents.cdk-cloudfront-authorization-2.4.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     5310 2024-05-16 19:33:27.814879 cloudcomponents.cdk-cloudfront-authorization-2.4.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     4444 2024-05-16 19:33:24.000000 cloudcomponents.cdk-cloudfront-authorization-2.4.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-05-16 19:33:24.000000 cloudcomponents.cdk-cloudfront-authorization-2.4.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-05-16 19:33:27.815167 cloudcomponents.cdk-cloudfront-authorization-2.4.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1915 2024-05-16 19:33:24.000000 cloudcomponents.cdk-cloudfront-authorization-2.4.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:27.811987 cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:27.812044 cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:27.813805 cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents/cdk_cloudfront_authorization/
+-rw-r--r--   0 hupe       (501) staff       (20)   220092 2024-05-16 19:33:24.000000 cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents/cdk_cloudfront_authorization/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:27.814072 cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents/cdk_cloudfront_authorization/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      509 2024-05-16 19:33:24.000000 cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents/cdk_cloudfront_authorization/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)  1144313 2024-05-16 19:33:24.000000 cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents/cdk_cloudfront_authorization/_jsii/cdk-cloudfront-authorization@2.4.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:33:24.000000 cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents/cdk_cloudfront_authorization/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:27.813410 cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     5310 2024-05-16 19:33:27.000000 cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      697 2024-05-16 19:33:27.000000 cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:33:27.000000 cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      169 2024-05-16 19:33:27.000000 cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-05-16 19:33:27.000000 cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-cloudfront-authorization-2.3.0/LICENSE` & `cloudcomponents.cdk-cloudfront-authorization-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-cloudfront-authorization-2.3.0/PKG-INFO` & `cloudcomponents.cdk-cloudfront-authorization-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-cloudfront-authorization
-Version: 2.3.0
+Version: 2.4.0
 Summary: CloudFront with Cognito authentication using Lambda@Edge
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-cloudfront-authorization-2.3.0/README.md` & `cloudcomponents.cdk-cloudfront-authorization-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-cloudfront-authorization-2.3.0/setup.py` & `cloudcomponents.cdk-cloudfront-authorization-2.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-cloudfront-authorization",
-    "version": "2.3.0",
+    "version": "2.4.0",
     "description": "CloudFront with Cognito authentication using Lambda@Edge",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cloudcomponents.cdk_cloudfront_authorization",
         "cloudcomponents.cdk_cloudfront_authorization._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_cloudfront_authorization._jsii": [
-            "cdk-cloudfront-authorization@2.3.0.jsii.tgz"
+            "cdk-cloudfront-authorization@2.4.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_cloudfront_authorization": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.28.0, <3.0.0",
-        "cloudcomponents.cdk-lambda-at-edge-pattern>=2.3.0, <3.0.0",
-        "constructs>=10.0.41, <11.0.0",
+        "aws-cdk-lib>=2.141.0, <3.0.0",
+        "cloudcomponents.cdk-lambda-at-edge-pattern>=2.4.0, <3.0.0",
+        "constructs>=10.3.0, <11.0.0",
         "jsii>=1.95.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents/cdk_cloudfront_authorization/__init__.py` & `cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents/cdk_cloudfront_authorization/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/PKG-INFO` & `cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-cloudfront-authorization
-Version: 2.3.0
+Version: 2.4.0
 Summary: CloudFront with Cognito authentication using Lambda@Edge
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-cloudfront-authorization-2.3.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/SOURCES.txt` & `cloudcomponents.cdk-cloudfront-authorization-2.4.0/src/cloudcomponents.cdk_cloudfront_authorization.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_cloudfront_authorization.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_cloudfront_authorization.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_cloudfront_authorization.egg-info/requires.txt
 src/cloudcomponents.cdk_cloudfront_authorization.egg-info/top_level.txt
 src/cloudcomponents/cdk_cloudfront_authorization/__init__.py
 src/cloudcomponents/cdk_cloudfront_authorization/py.typed
 src/cloudcomponents/cdk_cloudfront_authorization/_jsii/__init__.py
-src/cloudcomponents/cdk_cloudfront_authorization/_jsii/cdk-cloudfront-authorization@2.3.0.jsii.tgz
+src/cloudcomponents/cdk_cloudfront_authorization/_jsii/cdk-cloudfront-authorization@2.4.0.jsii.tgz
```

