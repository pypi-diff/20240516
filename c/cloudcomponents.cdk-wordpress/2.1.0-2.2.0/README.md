# Comparing `tmp/cloudcomponents.cdk-wordpress-2.1.0.tar.gz` & `tmp/cloudcomponents.cdk-wordpress-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-wordpress-2.1.0.tar", last modified: Mon Mar 25 18:26:12 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-wordpress-2.2.0.tar", last modified: Thu May 16 19:32:59 2024, max compression
```

## Comparing `cloudcomponents.cdk-wordpress-2.1.0.tar` & `cloudcomponents.cdk-wordpress-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:12.962673 cloudcomponents.cdk-wordpress-2.1.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-03-25 18:26:09.000000 cloudcomponents.cdk-wordpress-2.1.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-03-25 18:26:09.000000 cloudcomponents.cdk-wordpress-2.1.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     2853 2024-03-25 18:26:12.962426 cloudcomponents.cdk-wordpress-2.1.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     2025 2024-03-25 18:26:09.000000 cloudcomponents.cdk-wordpress-2.1.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-03-25 18:26:09.000000 cloudcomponents.cdk-wordpress-2.1.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-03-25 18:26:12.962715 cloudcomponents.cdk-wordpress-2.1.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1733 2024-03-25 18:26:09.000000 cloudcomponents.cdk-wordpress-2.1.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:12.959895 cloudcomponents.cdk-wordpress-2.1.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:12.959955 cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:12.961843 cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents/cdk_wordpress/
--rw-r--r--   0 hupe       (501) staff       (20)    56380 2024-03-25 18:26:09.000000 cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents/cdk_wordpress/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:12.962139 cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents/cdk_wordpress/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      423 2024-03-25 18:26:09.000000 cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents/cdk_wordpress/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)   137592 2024-03-25 18:26:09.000000 cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents/cdk_wordpress/_jsii/cdk-wordpress@2.1.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:26:09.000000 cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents/cdk_wordpress/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:12.961408 cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents.cdk_wordpress.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     2853 2024-03-25 18:26:12.000000 cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents.cdk_wordpress.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      547 2024-03-25 18:26:12.000000 cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents.cdk_wordpress.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:26:12.000000 cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents.cdk_wordpress.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-03-25 18:26:12.000000 cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents.cdk_wordpress.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-03-25 18:26:12.000000 cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents.cdk_wordpress.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.644728 cloudcomponents.cdk-wordpress-2.2.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-05-16 19:32:55.000000 cloudcomponents.cdk-wordpress-2.2.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-05-16 19:32:55.000000 cloudcomponents.cdk-wordpress-2.2.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     2853 2024-05-16 19:32:59.644404 cloudcomponents.cdk-wordpress-2.2.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     2025 2024-05-16 19:32:55.000000 cloudcomponents.cdk-wordpress-2.2.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-05-16 19:32:55.000000 cloudcomponents.cdk-wordpress-2.2.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-05-16 19:32:59.644777 cloudcomponents.cdk-wordpress-2.2.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1733 2024-05-16 19:32:55.000000 cloudcomponents.cdk-wordpress-2.2.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.641008 cloudcomponents.cdk-wordpress-2.2.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.641071 cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.643795 cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents/cdk_wordpress/
+-rw-r--r--   0 hupe       (501) staff       (20)    56380 2024-05-16 19:32:55.000000 cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents/cdk_wordpress/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.644089 cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents/cdk_wordpress/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      423 2024-05-16 19:32:55.000000 cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents/cdk_wordpress/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)   139082 2024-05-16 19:32:55.000000 cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents/cdk_wordpress/_jsii/cdk-wordpress@2.2.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:32:55.000000 cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents/cdk_wordpress/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.643402 cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents.cdk_wordpress.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     2853 2024-05-16 19:32:59.000000 cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents.cdk_wordpress.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      547 2024-05-16 19:32:59.000000 cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents.cdk_wordpress.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:32:59.000000 cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents.cdk_wordpress.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-05-16 19:32:59.000000 cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents.cdk_wordpress.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-05-16 19:32:59.000000 cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents.cdk_wordpress.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-wordpress-2.1.0/LICENSE` & `cloudcomponents.cdk-wordpress-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-wordpress-2.1.0/PKG-INFO` & `cloudcomponents.cdk-wordpress-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-wordpress
-Version: 2.1.0
+Version: 2.2.0
 Summary: CDK Construct to deploy wordpress
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-wordpress-2.1.0/README.md` & `cloudcomponents.cdk-wordpress-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-wordpress-2.1.0/setup.py` & `cloudcomponents.cdk-wordpress-2.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-wordpress",
-    "version": "2.1.0",
+    "version": "2.2.0",
     "description": "CDK Construct to deploy wordpress",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cloudcomponents.cdk_wordpress",
         "cloudcomponents.cdk_wordpress._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_wordpress._jsii": [
-            "cdk-wordpress@2.1.0.jsii.tgz"
+            "cdk-wordpress@2.2.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_wordpress": [
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

### Comparing `cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents/cdk_wordpress/__init__.py` & `cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents/cdk_wordpress/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents.cdk_wordpress.egg-info/PKG-INFO` & `cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents.cdk_wordpress.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-wordpress
-Version: 2.1.0
+Version: 2.2.0
 Summary: CDK Construct to deploy wordpress
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-wordpress-2.1.0/src/cloudcomponents.cdk_wordpress.egg-info/SOURCES.txt` & `cloudcomponents.cdk-wordpress-2.2.0/src/cloudcomponents.cdk_wordpress.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_wordpress.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_wordpress.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_wordpress.egg-info/requires.txt
 src/cloudcomponents.cdk_wordpress.egg-info/top_level.txt
 src/cloudcomponents/cdk_wordpress/__init__.py
 src/cloudcomponents/cdk_wordpress/py.typed
 src/cloudcomponents/cdk_wordpress/_jsii/__init__.py
-src/cloudcomponents/cdk_wordpress/_jsii/cdk-wordpress@2.1.0.jsii.tgz
+src/cloudcomponents/cdk_wordpress/_jsii/cdk-wordpress@2.2.0.jsii.tgz
```

