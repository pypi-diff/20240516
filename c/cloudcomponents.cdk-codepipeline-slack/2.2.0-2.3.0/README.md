# Comparing `tmp/cloudcomponents.cdk-codepipeline-slack-2.2.0.tar.gz` & `tmp/cloudcomponents.cdk-codepipeline-slack-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-codepipeline-slack-2.2.0.tar", last modified: Mon Mar 25 18:25:28 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-codepipeline-slack-2.3.0.tar", last modified: Wed Apr 17 18:35:46 2024, max compression
```

## Comparing `cloudcomponents.cdk-codepipeline-slack-2.2.0.tar` & `cloudcomponents.cdk-codepipeline-slack-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.261339 cloudcomponents.cdk-codepipeline-slack-2.2.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-slack-2.2.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-slack-2.2.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     5652 2024-03-25 18:25:28.261026 cloudcomponents.cdk-codepipeline-slack-2.2.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     4736 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-slack-2.2.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-slack-2.2.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-03-25 18:25:28.261385 cloudcomponents.cdk-codepipeline-slack-2.2.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1866 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-slack-2.2.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.255696 cloudcomponents.cdk-codepipeline-slack-2.2.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.256150 cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.258985 cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents/cdk_codepipeline_slack/
--rw-r--r--   0 hupe       (501) staff       (20)    30173 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents/cdk_codepipeline_slack/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.259606 cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents/cdk_codepipeline_slack/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      441 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents/cdk_codepipeline_slack/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)  1084241 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents/cdk_codepipeline_slack/_jsii/cdk-codepipeline-slack@2.2.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents/cdk_codepipeline_slack/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.258639 cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     5652 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      637 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.878635 cloudcomponents.cdk-codepipeline-slack-2.3.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-04-17 18:35:42.000000 cloudcomponents.cdk-codepipeline-slack-2.3.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:35:42.000000 cloudcomponents.cdk-codepipeline-slack-2.3.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     5652 2024-04-17 18:35:46.878245 cloudcomponents.cdk-codepipeline-slack-2.3.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     4736 2024-04-17 18:35:42.000000 cloudcomponents.cdk-codepipeline-slack-2.3.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:35:42.000000 cloudcomponents.cdk-codepipeline-slack-2.3.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:35:46.878681 cloudcomponents.cdk-codepipeline-slack-2.3.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1866 2024-04-17 18:35:42.000000 cloudcomponents.cdk-codepipeline-slack-2.3.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.871924 cloudcomponents.cdk-codepipeline-slack-2.3.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.871983 cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.875105 cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents/cdk_codepipeline_slack/
+-rw-r--r--   0 hupe       (501) staff       (20)    30173 2024-04-17 18:35:42.000000 cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents/cdk_codepipeline_slack/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.875434 cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents/cdk_codepipeline_slack/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      441 2024-04-17 18:35:42.000000 cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents/cdk_codepipeline_slack/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)  4672439 2024-04-17 18:35:42.000000 cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents/cdk_codepipeline_slack/_jsii/cdk-codepipeline-slack@2.3.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:42.000000 cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents/cdk_codepipeline_slack/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:35:46.874633 cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     5652 2024-04-17 18:35:46.000000 cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      637 2024-04-17 18:35:46.000000 cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:35:46.000000 cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-04-17 18:35:46.000000 cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:35:46.000000 cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-codepipeline-slack-2.2.0/LICENSE` & `cloudcomponents.cdk-codepipeline-slack-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-codepipeline-slack-2.2.0/PKG-INFO` & `cloudcomponents.cdk-codepipeline-slack-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-codepipeline-slack
-Version: 2.2.0
+Version: 2.3.0
 Summary: Cdk component that provisions a #slack approval workflow and notification messages on codepipeline state changes
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-codepipeline-slack-2.2.0/README.md` & `cloudcomponents.cdk-codepipeline-slack-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-codepipeline-slack-2.2.0/setup.py` & `cloudcomponents.cdk-codepipeline-slack-2.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-codepipeline-slack",
-    "version": "2.2.0",
+    "version": "2.3.0",
     "description": "Cdk component that provisions a #slack approval workflow and notification messages on codepipeline state changes",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudcomponents.cdk_codepipeline_slack",
         "cloudcomponents.cdk_codepipeline_slack._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_codepipeline_slack._jsii": [
-            "cdk-codepipeline-slack@2.2.0.jsii.tgz"
+            "cdk-codepipeline-slack@2.3.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_codepipeline_slack": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents/cdk_codepipeline_slack/__init__.py` & `cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents/cdk_codepipeline_slack/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/PKG-INFO` & `cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-codepipeline-slack
-Version: 2.2.0
+Version: 2.3.0
 Summary: Cdk component that provisions a #slack approval workflow and notification messages on codepipeline state changes
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-codepipeline-slack-2.2.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/SOURCES.txt` & `cloudcomponents.cdk-codepipeline-slack-2.3.0/src/cloudcomponents.cdk_codepipeline_slack.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_codepipeline_slack.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_codepipeline_slack.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_codepipeline_slack.egg-info/requires.txt
 src/cloudcomponents.cdk_codepipeline_slack.egg-info/top_level.txt
 src/cloudcomponents/cdk_codepipeline_slack/__init__.py
 src/cloudcomponents/cdk_codepipeline_slack/py.typed
 src/cloudcomponents/cdk_codepipeline_slack/_jsii/__init__.py
-src/cloudcomponents/cdk_codepipeline_slack/_jsii/cdk-codepipeline-slack@2.2.0.jsii.tgz
+src/cloudcomponents/cdk_codepipeline_slack/_jsii/cdk-codepipeline-slack@2.3.0.jsii.tgz
```

