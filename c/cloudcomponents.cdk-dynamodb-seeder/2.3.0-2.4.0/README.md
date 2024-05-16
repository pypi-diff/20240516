# Comparing `tmp/cloudcomponents.cdk-dynamodb-seeder-2.3.0.tar.gz` & `tmp/cloudcomponents.cdk-dynamodb-seeder-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-dynamodb-seeder-2.3.0.tar", last modified: Wed Apr 17 18:35:56 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-dynamodb-seeder-2.4.0.tar", last modified: Thu May 16 19:32:59 2024, max compression
```

## Comparing `cloudcomponents.cdk-dynamodb-seeder-2.3.0.tar` & `cloudcomponents.cdk-dynamodb-seeder-2.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.094277 cloudcomponents.cdk-dynamodb-seeder-2.3.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-04-17 18:35:52.000000 cloudcomponents.cdk-dynamodb-seeder-2.3.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:35:52.000000 cloudcomponents.cdk-dynamodb-seeder-2.3.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     3452 2024-04-17 18:35:56.094039 cloudcomponents.cdk-dynamodb-seeder-2.3.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     2623 2024-04-17 18:35:52.000000 cloudcomponents.cdk-dynamodb-seeder-2.3.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:35:52.000000 cloudcomponents.cdk-dynamodb-seeder-2.3.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:35:56.094316 cloudcomponents.cdk-dynamodb-seeder-2.3.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1764 2024-04-17 18:35:52.000000 cloudcomponents.cdk-dynamodb-seeder-2.3.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.090618 cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.090676 cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.092497 cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents/cdk_dynamodb_seeder/
--rw-r--r--   0 hupe       (501) staff       (20)    28907 2024-04-17 18:35:52.000000 cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents/cdk_dynamodb_seeder/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.092781 cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents/cdk_dynamodb_seeder/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      435 2024-04-17 18:35:52.000000 cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents/cdk_dynamodb_seeder/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)  1653145 2024-04-17 18:35:52.000000 cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents/cdk_dynamodb_seeder/_jsii/cdk-dynamodb-seeder@2.3.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:52.000000 cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents/cdk_dynamodb_seeder/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:56.092195 cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     3452 2024-04-17 18:35:56.000000 cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      607 2024-04-17 18:35:56.000000 cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:56.000000 cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-04-17 18:35:56.000000 cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:35:56.000000 cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.324714 cloudcomponents.cdk-dynamodb-seeder-2.4.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-05-16 19:32:55.000000 cloudcomponents.cdk-dynamodb-seeder-2.4.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-05-16 19:32:55.000000 cloudcomponents.cdk-dynamodb-seeder-2.4.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     3452 2024-05-16 19:32:59.324412 cloudcomponents.cdk-dynamodb-seeder-2.4.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     2623 2024-05-16 19:32:55.000000 cloudcomponents.cdk-dynamodb-seeder-2.4.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-05-16 19:32:55.000000 cloudcomponents.cdk-dynamodb-seeder-2.4.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-05-16 19:32:59.324799 cloudcomponents.cdk-dynamodb-seeder-2.4.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1764 2024-05-16 19:32:55.000000 cloudcomponents.cdk-dynamodb-seeder-2.4.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.320157 cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.320246 cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.323192 cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents/cdk_dynamodb_seeder/
+-rw-r--r--   0 hupe       (501) staff       (20)    28907 2024-05-16 19:32:55.000000 cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents/cdk_dynamodb_seeder/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.323720 cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents/cdk_dynamodb_seeder/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      435 2024-05-16 19:32:55.000000 cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents/cdk_dynamodb_seeder/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)   452045 2024-05-16 19:32:55.000000 cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents/cdk_dynamodb_seeder/_jsii/cdk-dynamodb-seeder@2.4.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:32:55.000000 cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents/cdk_dynamodb_seeder/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.322584 cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     3452 2024-05-16 19:32:59.000000 cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      607 2024-05-16 19:32:59.000000 cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:32:59.000000 cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-05-16 19:32:59.000000 cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-05-16 19:32:59.000000 cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-dynamodb-seeder-2.3.0/LICENSE` & `cloudcomponents.cdk-dynamodb-seeder-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-dynamodb-seeder-2.3.0/PKG-INFO` & `cloudcomponents.cdk-dynamodb-seeder-2.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-dynamodb-seeder
-Version: 2.3.0
+Version: 2.4.0
 Summary: A seeder for dynamodb tables
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-dynamodb-seeder-2.3.0/README.md` & `cloudcomponents.cdk-dynamodb-seeder-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-dynamodb-seeder-2.3.0/setup.py` & `cloudcomponents.cdk-dynamodb-seeder-2.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-dynamodb-seeder",
-    "version": "2.3.0",
+    "version": "2.4.0",
     "description": "A seeder for dynamodb tables",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cloudcomponents.cdk_dynamodb_seeder",
         "cloudcomponents.cdk_dynamodb_seeder._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_dynamodb_seeder._jsii": [
-            "cdk-dynamodb-seeder@2.3.0.jsii.tgz"
+            "cdk-dynamodb-seeder@2.4.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_dynamodb_seeder": [
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

### Comparing `cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents/cdk_dynamodb_seeder/__init__.py` & `cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents/cdk_dynamodb_seeder/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/PKG-INFO` & `cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-dynamodb-seeder
-Version: 2.3.0
+Version: 2.4.0
 Summary: A seeder for dynamodb tables
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-dynamodb-seeder-2.3.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/SOURCES.txt` & `cloudcomponents.cdk-dynamodb-seeder-2.4.0/src/cloudcomponents.cdk_dynamodb_seeder.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_dynamodb_seeder.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_dynamodb_seeder.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_dynamodb_seeder.egg-info/requires.txt
 src/cloudcomponents.cdk_dynamodb_seeder.egg-info/top_level.txt
 src/cloudcomponents/cdk_dynamodb_seeder/__init__.py
 src/cloudcomponents/cdk_dynamodb_seeder/py.typed
 src/cloudcomponents/cdk_dynamodb_seeder/_jsii/__init__.py
-src/cloudcomponents/cdk_dynamodb_seeder/_jsii/cdk-dynamodb-seeder@2.3.0.jsii.tgz
+src/cloudcomponents/cdk_dynamodb_seeder/_jsii/cdk-dynamodb-seeder@2.4.0.jsii.tgz
```

