# Comparing `tmp/cloudcomponents.cdk-secret-key-2.1.0.tar.gz` & `tmp/cloudcomponents.cdk-secret-key-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-secret-key-2.1.0.tar", last modified: Mon Mar 25 18:25:28 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-secret-key-2.2.0.tar", last modified: Thu May 16 19:28:14 2024, max compression
```

## Comparing `cloudcomponents.cdk-secret-key-2.1.0.tar` & `cloudcomponents.cdk-secret-key-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.241011 cloudcomponents.cdk-secret-key-2.1.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-03-25 18:25:23.000000 cloudcomponents.cdk-secret-key-2.1.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-03-25 18:25:23.000000 cloudcomponents.cdk-secret-key-2.1.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     2461 2024-03-25 18:25:28.240260 cloudcomponents.cdk-secret-key-2.1.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     1635 2024-03-25 18:25:23.000000 cloudcomponents.cdk-secret-key-2.1.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-03-25 18:25:23.000000 cloudcomponents.cdk-secret-key-2.1.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-03-25 18:25:28.241080 cloudcomponents.cdk-secret-key-2.1.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1696 2024-03-25 18:25:23.000000 cloudcomponents.cdk-secret-key-2.1.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.235505 cloudcomponents.cdk-secret-key-2.1.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.235582 cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.239586 cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents/cdk_secret_key/
--rw-r--r--   0 hupe       (501) staff       (20)    11653 2024-03-25 18:25:23.000000 cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents/cdk_secret_key/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.239932 cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents/cdk_secret_key/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      401 2024-03-25 18:25:23.000000 cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents/cdk_secret_key/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)   123715 2024-03-25 18:25:23.000000 cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents/cdk_secret_key/_jsii/cdk-secret-key@2.1.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:23.000000 cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents/cdk_secret_key/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.239123 cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents.cdk_secret_key.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     2461 2024-03-25 18:25:28.000000 cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents.cdk_secret_key.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      557 2024-03-25 18:25:28.000000 cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents.cdk_secret_key.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:28.000000 cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents.cdk_secret_key.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)       84 2024-03-25 18:25:28.000000 cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents.cdk_secret_key.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-03-25 18:25:28.000000 cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents.cdk_secret_key.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.247893 cloudcomponents.cdk-secret-key-2.2.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-05-16 19:28:09.000000 cloudcomponents.cdk-secret-key-2.2.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-05-16 19:28:09.000000 cloudcomponents.cdk-secret-key-2.2.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     2461 2024-05-16 19:28:14.247642 cloudcomponents.cdk-secret-key-2.2.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     1635 2024-05-16 19:28:09.000000 cloudcomponents.cdk-secret-key-2.2.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-05-16 19:28:09.000000 cloudcomponents.cdk-secret-key-2.2.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-05-16 19:28:14.247937 cloudcomponents.cdk-secret-key-2.2.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1697 2024-05-16 19:28:09.000000 cloudcomponents.cdk-secret-key-2.2.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.242444 cloudcomponents.cdk-secret-key-2.2.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.242505 cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.246928 cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents/cdk_secret_key/
+-rw-r--r--   0 hupe       (501) staff       (20)    11653 2024-05-16 19:28:09.000000 cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents/cdk_secret_key/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.247308 cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents/cdk_secret_key/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      401 2024-05-16 19:28:09.000000 cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents/cdk_secret_key/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)   125710 2024-05-16 19:28:09.000000 cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents/cdk_secret_key/_jsii/cdk-secret-key@2.2.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:28:09.000000 cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents/cdk_secret_key/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.246548 cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents.cdk_secret_key.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     2461 2024-05-16 19:28:14.000000 cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents.cdk_secret_key.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      557 2024-05-16 19:28:14.000000 cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents.cdk_secret_key.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:28:14.000000 cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents.cdk_secret_key.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       85 2024-05-16 19:28:14.000000 cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents.cdk_secret_key.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-05-16 19:28:14.000000 cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents.cdk_secret_key.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-secret-key-2.1.0/LICENSE` & `cloudcomponents.cdk-secret-key-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-secret-key-2.1.0/PKG-INFO` & `cloudcomponents.cdk-secret-key-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-secret-key
-Version: 2.1.0
+Version: 2.2.0
 Summary: Provide secret keys to lambdas
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-secret-key-2.1.0/README.md` & `cloudcomponents.cdk-secret-key-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-secret-key-2.1.0/setup.py` & `cloudcomponents.cdk-secret-key-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-secret-key",
-    "version": "2.1.0",
+    "version": "2.2.0",
     "description": "Provide secret keys to lambdas",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,23 @@
     },
     "packages": [
         "cloudcomponents.cdk_secret_key",
         "cloudcomponents.cdk_secret_key._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_secret_key._jsii": [
-            "cdk-secret-key@2.1.0.jsii.tgz"
+            "cdk-secret-key@2.2.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_secret_key": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.28.0, <3.0.0",
+        "aws-cdk-lib>=2.141.0, <3.0.0",
         "jsii>=1.95.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents/cdk_secret_key/__init__.py` & `cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents/cdk_secret_key/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents.cdk_secret_key.egg-info/PKG-INFO` & `cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents.cdk_secret_key.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-secret-key
-Version: 2.1.0
+Version: 2.2.0
 Summary: Provide secret keys to lambdas
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-secret-key-2.1.0/src/cloudcomponents.cdk_secret_key.egg-info/SOURCES.txt` & `cloudcomponents.cdk-secret-key-2.2.0/src/cloudcomponents.cdk_secret_key.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_secret_key.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_secret_key.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_secret_key.egg-info/requires.txt
 src/cloudcomponents.cdk_secret_key.egg-info/top_level.txt
 src/cloudcomponents/cdk_secret_key/__init__.py
 src/cloudcomponents/cdk_secret_key/py.typed
 src/cloudcomponents/cdk_secret_key/_jsii/__init__.py
-src/cloudcomponents/cdk_secret_key/_jsii/cdk-secret-key@2.1.0.jsii.tgz
+src/cloudcomponents/cdk_secret_key/_jsii/cdk-secret-key@2.2.0.jsii.tgz
```

