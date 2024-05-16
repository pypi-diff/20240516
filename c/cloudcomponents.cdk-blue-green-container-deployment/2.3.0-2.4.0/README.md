# Comparing `tmp/cloudcomponents.cdk-blue-green-container-deployment-2.3.0.tar.gz` & `tmp/cloudcomponents.cdk-blue-green-container-deployment-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-blue-green-container-deployment-2.3.0.tar", last modified: Wed Apr 17 18:35:46 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-blue-green-container-deployment-2.4.0.tar", last modified: Thu May 16 19:28:14 2024, max compression
```

## Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.3.0.tar` & `cloudcomponents.cdk-blue-green-container-deployment-2.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.573362 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     7023 2024-04-17 18:35:46.573039 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     6159 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:35:46.573407 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1879 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.567765 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.567833 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.570717 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/cdk_blue_green_container_deployment/
--rw-r--r--   0 hupe       (501) staff       (20)    80643 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/cdk_blue_green_container_deployment/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.571021 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      467 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)  3178833 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/cdk-blue-green-container-deployment@2.3.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:42.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/cdk_blue_green_container_deployment/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.570354 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     7023 2024-04-17 18:35:46.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      767 2024-04-17 18:35:46.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:46.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-04-17 18:35:46.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:35:46.000000 cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.365521 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-05-16 19:28:09.000000 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-05-16 19:28:09.000000 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     7023 2024-05-16 19:28:14.365231 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     6159 2024-05-16 19:28:09.000000 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-05-16 19:28:09.000000 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-05-16 19:28:14.365567 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1879 2024-05-16 19:28:09.000000 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.362096 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.362169 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.364137 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents/cdk_blue_green_container_deployment/
+-rw-r--r--   0 hupe       (501) staff       (20)    80643 2024-05-16 19:28:09.000000 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents/cdk_blue_green_container_deployment/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.364418 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      467 2024-05-16 19:28:09.000000 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)   778403 2024-05-16 19:28:09.000000 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/cdk-blue-green-container-deployment@2.4.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:28:09.000000 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents/cdk_blue_green_container_deployment/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.363783 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     7023 2024-05-16 19:28:14.000000 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      767 2024-05-16 19:28:14.000000 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:28:14.000000 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-05-16 19:28:14.000000 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-05-16 19:28:14.000000 cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.3.0/LICENSE` & `cloudcomponents.cdk-blue-green-container-deployment-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.3.0/PKG-INFO` & `cloudcomponents.cdk-blue-green-container-deployment-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-blue-green-container-deployment
-Version: 2.3.0
+Version: 2.4.0
 Summary: Blue green container deployment with CodeDeploy
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.3.0/README.md` & `cloudcomponents.cdk-blue-green-container-deployment-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.3.0/setup.py` & `cloudcomponents.cdk-blue-green-container-deployment-2.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-blue-green-container-deployment",
-    "version": "2.3.0",
+    "version": "2.4.0",
     "description": "Blue green container deployment with CodeDeploy",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cloudcomponents.cdk_blue_green_container_deployment",
         "cloudcomponents.cdk_blue_green_container_deployment._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_blue_green_container_deployment._jsii": [
-            "cdk-blue-green-container-deployment@2.3.0.jsii.tgz"
+            "cdk-blue-green-container-deployment@2.4.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_blue_green_container_deployment": [
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

### Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents/cdk_blue_green_container_deployment/__init__.py` & `cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents/cdk_blue_green_container_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/PKG-INFO` & `cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-blue-green-container-deployment
-Version: 2.3.0
+Version: 2.4.0
 Summary: Blue green container deployment with CodeDeploy
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-blue-green-container-deployment-2.3.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/SOURCES.txt` & `cloudcomponents.cdk-blue-green-container-deployment-2.4.0/src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/requires.txt
 src/cloudcomponents.cdk_blue_green_container_deployment.egg-info/top_level.txt
 src/cloudcomponents/cdk_blue_green_container_deployment/__init__.py
 src/cloudcomponents/cdk_blue_green_container_deployment/py.typed
 src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/__init__.py
-src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/cdk-blue-green-container-deployment@2.3.0.jsii.tgz
+src/cloudcomponents/cdk_blue_green_container_deployment/_jsii/cdk-blue-green-container-deployment@2.4.0.jsii.tgz
```

