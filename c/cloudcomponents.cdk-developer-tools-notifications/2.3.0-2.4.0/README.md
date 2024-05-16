# Comparing `tmp/cloudcomponents.cdk-developer-tools-notifications-2.3.0.tar.gz` & `tmp/cloudcomponents.cdk-developer-tools-notifications-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-developer-tools-notifications-2.3.0.tar", last modified: Wed Apr 17 18:36:27 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-developer-tools-notifications-2.4.0.tar", last modified: Thu May 16 19:33:19 2024, max compression
```

## Comparing `cloudcomponents.cdk-developer-tools-notifications-2.3.0.tar` & `cloudcomponents.cdk-developer-tools-notifications-2.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:27.323520 cloudcomponents.cdk-developer-tools-notifications-2.3.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-04-17 18:36:23.000000 cloudcomponents.cdk-developer-tools-notifications-2.3.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:36:23.000000 cloudcomponents.cdk-developer-tools-notifications-2.3.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     7181 2024-04-17 18:36:27.323249 cloudcomponents.cdk-developer-tools-notifications-2.3.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     6259 2024-04-17 18:36:23.000000 cloudcomponents.cdk-developer-tools-notifications-2.3.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:36:23.000000 cloudcomponents.cdk-developer-tools-notifications-2.3.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:36:27.323566 cloudcomponents.cdk-developer-tools-notifications-2.3.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1981 2024-04-17 18:36:23.000000 cloudcomponents.cdk-developer-tools-notifications-2.3.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:27.320876 cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:27.320934 cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:27.322693 cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents/cdk_developer_tools_notifications/
--rw-r--r--   0 hupe       (501) staff       (20)    71346 2024-04-17 18:36:23.000000 cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents/cdk_developer_tools_notifications/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:27.322969 cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents/cdk_developer_tools_notifications/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      504 2024-04-17 18:36:23.000000 cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents/cdk_developer_tools_notifications/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)    79173 2024-04-17 18:36:23.000000 cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents/cdk_developer_tools_notifications/_jsii/cdk-developer-tools-notifications@2.3.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:36:23.000000 cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents/cdk_developer_tools_notifications/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:27.322378 cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     7181 2024-04-17 18:36:27.000000 cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      747 2024-04-17 18:36:27.000000 cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:36:27.000000 cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      154 2024-04-17 18:36:27.000000 cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:36:27.000000 cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:19.475899 cloudcomponents.cdk-developer-tools-notifications-2.4.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-05-16 19:33:16.000000 cloudcomponents.cdk-developer-tools-notifications-2.4.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-05-16 19:33:16.000000 cloudcomponents.cdk-developer-tools-notifications-2.4.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     7181 2024-05-16 19:33:19.475688 cloudcomponents.cdk-developer-tools-notifications-2.4.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     6259 2024-05-16 19:33:16.000000 cloudcomponents.cdk-developer-tools-notifications-2.4.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-05-16 19:33:16.000000 cloudcomponents.cdk-developer-tools-notifications-2.4.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-05-16 19:33:19.475938 cloudcomponents.cdk-developer-tools-notifications-2.4.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1981 2024-05-16 19:33:16.000000 cloudcomponents.cdk-developer-tools-notifications-2.4.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:19.473329 cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:19.473389 cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:19.475139 cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents/cdk_developer_tools_notifications/
+-rw-r--r--   0 hupe       (501) staff       (20)    71346 2024-05-16 19:33:16.000000 cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents/cdk_developer_tools_notifications/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:19.475423 cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents/cdk_developer_tools_notifications/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      504 2024-05-16 19:33:16.000000 cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents/cdk_developer_tools_notifications/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)    79529 2024-05-16 19:33:16.000000 cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents/cdk_developer_tools_notifications/_jsii/cdk-developer-tools-notifications@2.4.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:33:16.000000 cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents/cdk_developer_tools_notifications/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:19.474817 cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     7181 2024-05-16 19:33:19.000000 cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      747 2024-05-16 19:33:19.000000 cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:33:19.000000 cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      154 2024-05-16 19:33:19.000000 cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-05-16 19:33:19.000000 cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-developer-tools-notifications-2.3.0/LICENSE` & `cloudcomponents.cdk-developer-tools-notifications-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-developer-tools-notifications-2.3.0/PKG-INFO` & `cloudcomponents.cdk-developer-tools-notifications-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-developer-tools-notifications
-Version: 2.3.0
+Version: 2.4.0
 Summary: #slack / msteams / email notifications for developer tools: CodeCommit, CodeBuild, CodeDeploy, CodePipeline
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-developer-tools-notifications-2.3.0/README.md` & `cloudcomponents.cdk-developer-tools-notifications-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-developer-tools-notifications-2.3.0/setup.py` & `cloudcomponents.cdk-developer-tools-notifications-2.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-developer-tools-notifications",
-    "version": "2.3.0",
+    "version": "2.4.0",
     "description": "#slack / msteams / email notifications for developer tools: CodeCommit, CodeBuild, CodeDeploy, CodePipeline",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cloudcomponents.cdk_developer_tools_notifications",
         "cloudcomponents.cdk_developer_tools_notifications._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_developer_tools_notifications._jsii": [
-            "cdk-developer-tools-notifications@2.3.0.jsii.tgz"
+            "cdk-developer-tools-notifications@2.4.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_developer_tools_notifications": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.28.0, <3.0.0",
-        "cloudcomponents.cdk-chatops>=2.3.0, <3.0.0",
-        "constructs>=10.0.41, <11.0.0",
+        "aws-cdk-lib>=2.141.0, <3.0.0",
+        "cloudcomponents.cdk-chatops>=2.4.0, <3.0.0",
+        "constructs>=10.3.0, <11.0.0",
         "jsii>=1.95.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents/cdk_developer_tools_notifications/__init__.py` & `cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents/cdk_developer_tools_notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/PKG-INFO` & `cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-developer-tools-notifications
-Version: 2.3.0
+Version: 2.4.0
 Summary: #slack / msteams / email notifications for developer tools: CodeCommit, CodeBuild, CodeDeploy, CodePipeline
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-developer-tools-notifications-2.3.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/SOURCES.txt` & `cloudcomponents.cdk-developer-tools-notifications-2.4.0/src/cloudcomponents.cdk_developer_tools_notifications.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_developer_tools_notifications.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_developer_tools_notifications.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_developer_tools_notifications.egg-info/requires.txt
 src/cloudcomponents.cdk_developer_tools_notifications.egg-info/top_level.txt
 src/cloudcomponents/cdk_developer_tools_notifications/__init__.py
 src/cloudcomponents/cdk_developer_tools_notifications/py.typed
 src/cloudcomponents/cdk_developer_tools_notifications/_jsii/__init__.py
-src/cloudcomponents/cdk_developer_tools_notifications/_jsii/cdk-developer-tools-notifications@2.3.0.jsii.tgz
+src/cloudcomponents/cdk_developer_tools_notifications/_jsii/cdk-developer-tools-notifications@2.4.0.jsii.tgz
```

