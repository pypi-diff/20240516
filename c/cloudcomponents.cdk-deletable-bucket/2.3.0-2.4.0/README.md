# Comparing `tmp/cloudcomponents.cdk-deletable-bucket-2.3.0.tar.gz` & `tmp/cloudcomponents.cdk-deletable-bucket-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-deletable-bucket-2.3.0.tar", last modified: Wed Apr 17 18:36:30 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-deletable-bucket-2.4.0.tar", last modified: Thu May 16 19:33:28 2024, max compression
```

## Comparing `cloudcomponents.cdk-deletable-bucket-2.3.0.tar` & `cloudcomponents.cdk-deletable-bucket-2.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:30.540617 cloudcomponents.cdk-deletable-bucket-2.3.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-04-17 18:36:27.000000 cloudcomponents.cdk-deletable-bucket-2.3.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:36:27.000000 cloudcomponents.cdk-deletable-bucket-2.3.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     2728 2024-04-17 18:36:30.540422 cloudcomponents.cdk-deletable-bucket-2.3.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     1841 2024-04-17 18:36:27.000000 cloudcomponents.cdk-deletable-bucket-2.3.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:36:27.000000 cloudcomponents.cdk-deletable-bucket-2.3.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:36:30.540651 cloudcomponents.cdk-deletable-bucket-2.3.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1827 2024-04-17 18:36:27.000000 cloudcomponents.cdk-deletable-bucket-2.3.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:30.537654 cloudcomponents.cdk-deletable-bucket-2.3.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:30.537711 cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:30.539355 cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents/cdk_deletable_bucket/
--rw-r--r--   0 hupe       (501) staff       (20)    57605 2024-04-17 18:36:27.000000 cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents/cdk_deletable_bucket/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:30.539620 cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents/cdk_deletable_bucket/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      437 2024-04-17 18:36:27.000000 cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents/cdk_deletable_bucket/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)  1328359 2024-04-17 18:36:27.000000 cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents/cdk_deletable_bucket/_jsii/cdk-deletable-bucket@2.3.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:36:27.000000 cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents/cdk_deletable_bucket/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:30.539066 cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     2728 2024-04-17 18:36:30.000000 cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      617 2024-04-17 18:36:30.000000 cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:36:30.000000 cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-04-17 18:36:30.000000 cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:36:30.000000 cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:28.176405 cloudcomponents.cdk-deletable-bucket-2.4.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-05-16 19:33:24.000000 cloudcomponents.cdk-deletable-bucket-2.4.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-05-16 19:33:24.000000 cloudcomponents.cdk-deletable-bucket-2.4.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     2728 2024-05-16 19:33:28.176118 cloudcomponents.cdk-deletable-bucket-2.4.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     1841 2024-05-16 19:33:24.000000 cloudcomponents.cdk-deletable-bucket-2.4.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-05-16 19:33:24.000000 cloudcomponents.cdk-deletable-bucket-2.4.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-05-16 19:33:28.176453 cloudcomponents.cdk-deletable-bucket-2.4.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1827 2024-05-16 19:33:24.000000 cloudcomponents.cdk-deletable-bucket-2.4.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:28.173480 cloudcomponents.cdk-deletable-bucket-2.4.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:28.173545 cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:28.175366 cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents/cdk_deletable_bucket/
+-rw-r--r--   0 hupe       (501) staff       (20)    57605 2024-05-16 19:33:24.000000 cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents/cdk_deletable_bucket/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:28.175655 cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents/cdk_deletable_bucket/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      437 2024-05-16 19:33:24.000000 cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents/cdk_deletable_bucket/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)   128558 2024-05-16 19:33:24.000000 cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents/cdk_deletable_bucket/_jsii/cdk-deletable-bucket@2.4.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:33:24.000000 cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents/cdk_deletable_bucket/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:28.175022 cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     2728 2024-05-16 19:33:28.000000 cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      617 2024-05-16 19:33:28.000000 cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:33:28.000000 cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-05-16 19:33:28.000000 cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-05-16 19:33:28.000000 cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-deletable-bucket-2.3.0/LICENSE` & `cloudcomponents.cdk-deletable-bucket-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-deletable-bucket-2.3.0/PKG-INFO` & `cloudcomponents.cdk-deletable-bucket-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-deletable-bucket
-Version: 2.3.0
+Version: 2.4.0
 Summary: Bucket with content cleanup to allow bucket deletion when the stack will be destroyed
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-deletable-bucket-2.3.0/README.md` & `cloudcomponents.cdk-deletable-bucket-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-deletable-bucket-2.3.0/setup.py` & `cloudcomponents.cdk-deletable-bucket-2.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-deletable-bucket",
-    "version": "2.3.0",
+    "version": "2.4.0",
     "description": "Bucket with content cleanup to allow bucket deletion when the stack will be destroyed",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cloudcomponents.cdk_deletable_bucket",
         "cloudcomponents.cdk_deletable_bucket._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_deletable_bucket._jsii": [
-            "cdk-deletable-bucket@2.3.0.jsii.tgz"
+            "cdk-deletable-bucket@2.4.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_deletable_bucket": [
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

### Comparing `cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents/cdk_deletable_bucket/__init__.py` & `cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents/cdk_deletable_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/PKG-INFO` & `cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-deletable-bucket
-Version: 2.3.0
+Version: 2.4.0
 Summary: Bucket with content cleanup to allow bucket deletion when the stack will be destroyed
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-deletable-bucket-2.3.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/SOURCES.txt` & `cloudcomponents.cdk-deletable-bucket-2.4.0/src/cloudcomponents.cdk_deletable_bucket.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_deletable_bucket.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_deletable_bucket.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_deletable_bucket.egg-info/requires.txt
 src/cloudcomponents.cdk_deletable_bucket.egg-info/top_level.txt
 src/cloudcomponents/cdk_deletable_bucket/__init__.py
 src/cloudcomponents/cdk_deletable_bucket/py.typed
 src/cloudcomponents/cdk_deletable_bucket/_jsii/__init__.py
-src/cloudcomponents/cdk_deletable_bucket/_jsii/cdk-deletable-bucket@2.3.0.jsii.tgz
+src/cloudcomponents/cdk_deletable_bucket/_jsii/cdk-deletable-bucket@2.4.0.jsii.tgz
```

