# Comparing `tmp/cloudcomponents.cdk-temp-stack-2.2.0.tar.gz` & `tmp/cloudcomponents.cdk-temp-stack-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-temp-stack-2.2.0.tar", last modified: Mon Mar 25 18:26:12 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-temp-stack-2.3.0.tar", last modified: Wed Apr 17 18:36:15 2024, max compression
```

## Comparing `cloudcomponents.cdk-temp-stack-2.2.0.tar` & `cloudcomponents.cdk-temp-stack-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:12.362122 cloudcomponents.cdk-temp-stack-2.2.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-03-25 18:26:09.000000 cloudcomponents.cdk-temp-stack-2.2.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-03-25 18:26:09.000000 cloudcomponents.cdk-temp-stack-2.2.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     3440 2024-03-25 18:26:12.361834 cloudcomponents.cdk-temp-stack-2.2.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     2591 2024-03-25 18:26:09.000000 cloudcomponents.cdk-temp-stack-2.2.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-03-25 18:26:09.000000 cloudcomponents.cdk-temp-stack-2.2.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-03-25 18:26:12.362176 cloudcomponents.cdk-temp-stack-2.2.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1759 2024-03-25 18:26:09.000000 cloudcomponents.cdk-temp-stack-2.2.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:12.358805 cloudcomponents.cdk-temp-stack-2.2.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:12.358861 cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:12.361005 cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents/cdk_temp_stack/
--rw-r--r--   0 hupe       (501) staff       (20)    29632 2024-03-25 18:26:09.000000 cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents/cdk_temp_stack/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:12.361426 cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents/cdk_temp_stack/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      425 2024-03-25 18:26:09.000000 cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents/cdk_temp_stack/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)   126940 2024-03-25 18:26:09.000000 cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents/cdk_temp_stack/_jsii/cdk-temp-stack@2.2.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:26:09.000000 cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents/cdk_temp_stack/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:12.360568 cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents.cdk_temp_stack.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     3440 2024-03-25 18:26:12.000000 cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents.cdk_temp_stack.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      557 2024-03-25 18:26:12.000000 cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents.cdk_temp_stack.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:26:12.000000 cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents.cdk_temp_stack.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-03-25 18:26:12.000000 cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents.cdk_temp_stack.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-03-25 18:26:12.000000 cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents.cdk_temp_stack.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:15.490718 cloudcomponents.cdk-temp-stack-2.3.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-04-17 18:36:12.000000 cloudcomponents.cdk-temp-stack-2.3.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:36:12.000000 cloudcomponents.cdk-temp-stack-2.3.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     3440 2024-04-17 18:36:15.490500 cloudcomponents.cdk-temp-stack-2.3.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     2591 2024-04-17 18:36:12.000000 cloudcomponents.cdk-temp-stack-2.3.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:36:12.000000 cloudcomponents.cdk-temp-stack-2.3.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:36:15.490754 cloudcomponents.cdk-temp-stack-2.3.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1759 2024-04-17 18:36:12.000000 cloudcomponents.cdk-temp-stack-2.3.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:15.487512 cloudcomponents.cdk-temp-stack-2.3.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:15.487574 cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:15.489313 cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents/cdk_temp_stack/
+-rw-r--r--   0 hupe       (501) staff       (20)    29632 2024-04-17 18:36:12.000000 cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents/cdk_temp_stack/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:15.489581 cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents/cdk_temp_stack/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      425 2024-04-17 18:36:12.000000 cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents/cdk_temp_stack/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)  1328839 2024-04-17 18:36:12.000000 cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents/cdk_temp_stack/_jsii/cdk-temp-stack@2.3.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:36:12.000000 cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents/cdk_temp_stack/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:15.488997 cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents.cdk_temp_stack.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     3440 2024-04-17 18:36:15.000000 cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents.cdk_temp_stack.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      557 2024-04-17 18:36:15.000000 cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents.cdk_temp_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:36:15.000000 cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents.cdk_temp_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-04-17 18:36:15.000000 cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents.cdk_temp_stack.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:36:15.000000 cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents.cdk_temp_stack.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-temp-stack-2.2.0/LICENSE` & `cloudcomponents.cdk-temp-stack-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-temp-stack-2.2.0/PKG-INFO` & `cloudcomponents.cdk-temp-stack-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-temp-stack
-Version: 2.2.0
+Version: 2.3.0
 Summary: A stack that destroys itself after a given time (ttl)
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-temp-stack-2.2.0/README.md` & `cloudcomponents.cdk-temp-stack-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-temp-stack-2.2.0/setup.py` & `cloudcomponents.cdk-temp-stack-2.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-temp-stack",
-    "version": "2.2.0",
+    "version": "2.3.0",
     "description": "A stack that destroys itself after a given time (ttl)",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudcomponents.cdk_temp_stack",
         "cloudcomponents.cdk_temp_stack._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_temp_stack._jsii": [
-            "cdk-temp-stack@2.2.0.jsii.tgz"
+            "cdk-temp-stack@2.3.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_temp_stack": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents/cdk_temp_stack/__init__.py` & `cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents/cdk_temp_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents.cdk_temp_stack.egg-info/PKG-INFO` & `cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents.cdk_temp_stack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-temp-stack
-Version: 2.2.0
+Version: 2.3.0
 Summary: A stack that destroys itself after a given time (ttl)
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-temp-stack-2.2.0/src/cloudcomponents.cdk_temp_stack.egg-info/SOURCES.txt` & `cloudcomponents.cdk-temp-stack-2.3.0/src/cloudcomponents.cdk_temp_stack.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_temp_stack.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_temp_stack.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_temp_stack.egg-info/requires.txt
 src/cloudcomponents.cdk_temp_stack.egg-info/top_level.txt
 src/cloudcomponents/cdk_temp_stack/__init__.py
 src/cloudcomponents/cdk_temp_stack/py.typed
 src/cloudcomponents/cdk_temp_stack/_jsii/__init__.py
-src/cloudcomponents/cdk_temp_stack/_jsii/cdk-temp-stack@2.2.0.jsii.tgz
+src/cloudcomponents/cdk_temp_stack/_jsii/cdk-temp-stack@2.3.0.jsii.tgz
```

