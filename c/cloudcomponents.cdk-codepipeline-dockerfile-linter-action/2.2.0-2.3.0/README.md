# Comparing `tmp/cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0.tar.gz` & `tmp/cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0.tar", last modified: Mon Mar 25 18:25:28 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0.tar", last modified: Thu May 16 19:28:14 2024, max compression
```

## Comparing `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0.tar` & `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.225378 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     4019 2024-03-25 18:25:28.224995 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     3143 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-03-25 18:25:28.225453 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1921 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.217884 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.217977 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.223491 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/
--rw-r--r--   0 hupe       (501) staff       (20)    15699 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.223899 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      479 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)    65146 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/_jsii/cdk-codepipeline-dockerfile-linter-action@2.2.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.222752 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     4019 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      827 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.321227 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     4019 2024-05-16 19:28:14.320921 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     3143 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-05-16 19:28:14.321274 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1921 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.317972 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.318043 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.320210 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/
+-rw-r--r--   0 hupe       (501) staff       (20)    15699 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.320568 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      479 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)    65555 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/_jsii/cdk-codepipeline-dockerfile-linter-action@2.3.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.319843 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     4019 2024-05-16 19:28:14.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      827 2024-05-16 19:28:14.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:28:14.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-05-16 19:28:14.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-05-16 19:28:14.000000 cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/LICENSE` & `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/PKG-INFO` & `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-codepipeline-dockerfile-linter-action
-Version: 2.2.0
+Version: 2.3.0
 Summary: CodePipeline action to lint dockerfiles with hadolint
 Home-page: https://github.com/cloudcomponents/cdk-components
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-components.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/README.md` & `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/setup.py` & `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-codepipeline-dockerfile-linter-action",
-    "version": "2.2.0",
+    "version": "2.3.0",
     "description": "CodePipeline action to lint dockerfiles with hadolint",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-components",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cloudcomponents.cdk_codepipeline_dockerfile_linter_action",
         "cloudcomponents.cdk_codepipeline_dockerfile_linter_action._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_codepipeline_dockerfile_linter_action._jsii": [
-            "cdk-codepipeline-dockerfile-linter-action@2.2.0.jsii.tgz"
+            "cdk-codepipeline-dockerfile-linter-action@2.3.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_codepipeline_dockerfile_linter_action": [
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

### Comparing `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/__init__.py` & `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/PKG-INFO` & `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-codepipeline-dockerfile-linter-action
-Version: 2.2.0
+Version: 2.3.0
 Summary: CodePipeline action to lint dockerfiles with hadolint
 Home-page: https://github.com/cloudcomponents/cdk-components
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-components.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.2.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/SOURCES.txt` & `cloudcomponents.cdk-codepipeline-dockerfile-linter-action-2.3.0/src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/requires.txt
 src/cloudcomponents.cdk_codepipeline_dockerfile_linter_action.egg-info/top_level.txt
 src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/__init__.py
 src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/py.typed
 src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/_jsii/__init__.py
-src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/_jsii/cdk-codepipeline-dockerfile-linter-action@2.2.0.jsii.tgz
+src/cloudcomponents/cdk_codepipeline_dockerfile_linter_action/_jsii/cdk-codepipeline-dockerfile-linter-action@2.3.0.jsii.tgz
```

