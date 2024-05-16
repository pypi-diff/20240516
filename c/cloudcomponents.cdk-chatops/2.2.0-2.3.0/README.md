# Comparing `tmp/cloudcomponents.cdk-chatops-2.2.0.tar.gz` & `tmp/cloudcomponents.cdk-chatops-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-chatops-2.2.0.tar", last modified: Mon Mar 25 18:25:28 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-chatops-2.3.0.tar", last modified: Wed Apr 17 18:35:46 2024, max compression
```

## Comparing `cloudcomponents.cdk-chatops-2.2.0.tar` & `cloudcomponents.cdk-chatops-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.290583 cloudcomponents.cdk-chatops-2.2.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-03-25 18:25:23.000000 cloudcomponents.cdk-chatops-2.2.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-03-25 18:25:23.000000 cloudcomponents.cdk-chatops-2.2.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     6178 2024-03-25 18:25:28.290289 cloudcomponents.cdk-chatops-2.2.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     5332 2024-03-25 18:25:23.000000 cloudcomponents.cdk-chatops-2.2.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-03-25 18:25:23.000000 cloudcomponents.cdk-chatops-2.2.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-03-25 18:25:28.290627 cloudcomponents.cdk-chatops-2.2.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1741 2024-03-25 18:25:23.000000 cloudcomponents.cdk-chatops-2.2.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.286745 cloudcomponents.cdk-chatops-2.2.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.286810 cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.289559 cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents/cdk_chatops/
--rw-r--r--   0 hupe       (501) staff       (20)    27989 2024-03-25 18:25:23.000000 cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents/cdk_chatops/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.289923 cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents/cdk_chatops/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      419 2024-03-25 18:25:23.000000 cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents/cdk_chatops/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)   144701 2024-03-25 18:25:23.000000 cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents/cdk_chatops/_jsii/cdk-chatops@2.2.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:23.000000 cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents/cdk_chatops/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.289198 cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents.cdk_chatops.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     6178 2024-03-25 18:25:28.000000 cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents.cdk_chatops.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      527 2024-03-25 18:25:28.000000 cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents.cdk_chatops.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:28.000000 cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents.cdk_chatops.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-03-25 18:25:28.000000 cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents.cdk_chatops.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-03-25 18:25:28.000000 cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents.cdk_chatops.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.423362 cloudcomponents.cdk-chatops-2.3.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-04-17 18:35:41.000000 cloudcomponents.cdk-chatops-2.3.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:35:41.000000 cloudcomponents.cdk-chatops-2.3.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     6178 2024-04-17 18:35:46.422948 cloudcomponents.cdk-chatops-2.3.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     5332 2024-04-17 18:35:41.000000 cloudcomponents.cdk-chatops-2.3.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:35:41.000000 cloudcomponents.cdk-chatops-2.3.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:35:46.423455 cloudcomponents.cdk-chatops-2.3.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1741 2024-04-17 18:35:41.000000 cloudcomponents.cdk-chatops-2.3.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.418905 cloudcomponents.cdk-chatops-2.3.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.418976 cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.420964 cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents/cdk_chatops/
+-rw-r--r--   0 hupe       (501) staff       (20)    27989 2024-04-17 18:35:41.000000 cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents/cdk_chatops/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.421732 cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents/cdk_chatops/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      419 2024-04-17 18:35:41.000000 cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents/cdk_chatops/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)  1346363 2024-04-17 18:35:41.000000 cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents/cdk_chatops/_jsii/cdk-chatops@2.3.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:41.000000 cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents/cdk_chatops/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.420633 cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents.cdk_chatops.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     6178 2024-04-17 18:35:46.000000 cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents.cdk_chatops.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      527 2024-04-17 18:35:46.000000 cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents.cdk_chatops.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:46.000000 cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents.cdk_chatops.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-04-17 18:35:46.000000 cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents.cdk_chatops.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:35:46.000000 cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents.cdk_chatops.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-chatops-2.2.0/LICENSE` & `cloudcomponents.cdk-chatops-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-chatops-2.2.0/PKG-INFO` & `cloudcomponents.cdk-chatops-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-chatops
-Version: 2.2.0
+Version: 2.3.0
 Summary: Constructs for chattool integration: #slack / msteams
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-chatops-2.2.0/README.md` & `cloudcomponents.cdk-chatops-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-chatops-2.2.0/setup.py` & `cloudcomponents.cdk-chatops-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-chatops",
-    "version": "2.2.0",
+    "version": "2.3.0",
     "description": "Constructs for chattool integration: #slack / msteams",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudcomponents.cdk_chatops",
         "cloudcomponents.cdk_chatops._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_chatops._jsii": [
-            "cdk-chatops@2.2.0.jsii.tgz"
+            "cdk-chatops@2.3.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_chatops": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents/cdk_chatops/__init__.py` & `cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents/cdk_chatops/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents.cdk_chatops.egg-info/PKG-INFO` & `cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents.cdk_chatops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-chatops
-Version: 2.2.0
+Version: 2.3.0
 Summary: Constructs for chattool integration: #slack / msteams
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-chatops-2.2.0/src/cloudcomponents.cdk_chatops.egg-info/SOURCES.txt` & `cloudcomponents.cdk-chatops-2.3.0/src/cloudcomponents.cdk_chatops.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_chatops.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_chatops.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_chatops.egg-info/requires.txt
 src/cloudcomponents.cdk_chatops.egg-info/top_level.txt
 src/cloudcomponents/cdk_chatops/__init__.py
 src/cloudcomponents/cdk_chatops/py.typed
 src/cloudcomponents/cdk_chatops/_jsii/__init__.py
-src/cloudcomponents/cdk_chatops/_jsii/cdk-chatops@2.2.0.jsii.tgz
+src/cloudcomponents/cdk_chatops/_jsii/cdk-chatops@2.3.0.jsii.tgz
```

