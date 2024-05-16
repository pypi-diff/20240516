# Comparing `tmp/cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0.tar.gz` & `tmp/cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0.tar", last modified: Sun Mar 20 14:48:58 2022, max compression
+gzip compressed data, was "cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0.tar", last modified: Mon Mar 25 18:25:28 2024, max compression
```

## Comparing `cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0.tar` & `cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2022-03-20 14:48:58.747680 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2022-03-20 14:48:52.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2022-03-20 14:48:52.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     4076 2022-03-20 14:48:58.747530 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     3167 2022-03-20 14:48:52.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      106 2022-03-20 14:48:52.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2022-03-20 14:48:58.747722 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1914 2022-03-20 14:48:52.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2022-03-20 14:48:58.744840 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2022-03-20 14:48:58.744902 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2022-03-20 14:48:58.746951 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/
--rw-r--r--   0 hupe       (501) staff       (20)    16672 2022-03-20 14:48:52.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2022-03-20 14:48:58.747224 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      449 2022-03-20 14:48:52.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)   109869 2022-03-20 14:48:52.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/_jsii/cdk-codepipeline-anchore-inline-scan-action@2.1.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2022-03-20 14:48:52.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2022-03-20 14:48:58.746670 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     4076 2022-03-20 14:48:58.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      847 2022-03-20 14:48:58.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2022-03-20 14:48:58.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)       93 2022-03-20 14:48:58.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2022-03-20 14:48:58.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.220366 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     4058 2024-03-25 18:25:28.220093 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     3167 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-03-25 18:25:28.220412 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1946 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.212097 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.212166 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.218445 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/
+-rw-r--r--   0 hupe       (501) staff       (20)    20265 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.219700 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      483 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)   126339 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/_jsii/cdk-codepipeline-anchore-inline-scan-action@2.2.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.216177 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     4058 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      847 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/LICENSE` & `cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/PKG-INFO` & `cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-codepipeline-anchore-inline-scan-action
-Version: 2.1.0
+Version: 2.2.0
 Summary: CodePipeline action to integrate Anchore Engine into your pipeline
 Home-page: https://github.com/cloudcomponents/cdk-components
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-components.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
-Requires-Python: >=3.6
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![cloudcomponents Logo](https://raw.githubusercontent.com/cloudcomponents/cdk-constructs/master/logo.png)](https://github.com/cloudcomponents/cdk-constructs)
 
 # @cloudcomponents/cdk-codepipeline-anchore-inline-scan-action
 
@@ -108,9 +107,7 @@
 ## Example
 
 See more complete [examples](https://github.com/cloudcomponents/cdk-constructs/tree/master/examples).
 
 ## License
 
 [MIT](https://github.com/cloudcomponents/cdk-constructs/tree/master/packages/cdk-codepipeline-anchore-inline-scan-action/LICENSE)
-
-
```

### Comparing `cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/README.md` & `cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/setup.py` & `cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-codepipeline-anchore-inline-scan-action",
-    "version": "2.1.0",
+    "version": "2.2.0",
     "description": "CodePipeline action to integrate Anchore Engine into your pipeline",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-components",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,36 +22,37 @@
     },
     "packages": [
         "cloudcomponents.cdk_codepipeline_anchore_inline_scan_action",
         "cloudcomponents.cdk_codepipeline_anchore_inline_scan_action._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_codepipeline_anchore_inline_scan_action._jsii": [
-            "cdk-codepipeline-anchore-inline-scan-action@2.1.0.jsii.tgz"
+            "cdk-codepipeline-anchore-inline-scan-action@2.2.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_codepipeline_anchore_inline_scan_action": [
             "py.typed"
         ]
     },
-    "python_requires": ">=3.6",
+    "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.8.0, <3.0.0",
+        "aws-cdk-lib>=2.28.0, <3.0.0",
         "constructs>=10.0.41, <11.0.0",
-        "jsii>=1.52.1, <2.0.0",
-        "publication>=0.0.3"
+        "jsii>=1.95.0, <2.0.0",
+        "publication>=0.0.3",
+        "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
 )
```

### Comparing `cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/PKG-INFO` & `cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-codepipeline-anchore-inline-scan-action
-Version: 2.1.0
+Version: 2.2.0
 Summary: CodePipeline action to integrate Anchore Engine into your pipeline
 Home-page: https://github.com/cloudcomponents/cdk-components
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-components.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: License :: OSI Approved
-Requires-Python: >=3.6
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![cloudcomponents Logo](https://raw.githubusercontent.com/cloudcomponents/cdk-constructs/master/logo.png)](https://github.com/cloudcomponents/cdk-constructs)
 
 # @cloudcomponents/cdk-codepipeline-anchore-inline-scan-action
 
@@ -108,9 +107,7 @@
 ## Example
 
 See more complete [examples](https://github.com/cloudcomponents/cdk-constructs/tree/master/examples).
 
 ## License
 
 [MIT](https://github.com/cloudcomponents/cdk-constructs/tree/master/packages/cdk-codepipeline-anchore-inline-scan-action/LICENSE)
-
-
```

### Comparing `cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.1.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/SOURCES.txt` & `cloudcomponents.cdk-codepipeline-anchore-inline-scan-action-2.2.0/src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/requires.txt
 src/cloudcomponents.cdk_codepipeline_anchore_inline_scan_action.egg-info/top_level.txt
 src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/__init__.py
 src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/py.typed
 src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/_jsii/__init__.py
-src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/_jsii/cdk-codepipeline-anchore-inline-scan-action@2.1.0.jsii.tgz
+src/cloudcomponents/cdk_codepipeline_anchore_inline_scan_action/_jsii/cdk-codepipeline-anchore-inline-scan-action@2.2.0.jsii.tgz
```

