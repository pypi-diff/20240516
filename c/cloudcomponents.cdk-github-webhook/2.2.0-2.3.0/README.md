# Comparing `tmp/cloudcomponents.cdk-github-webhook-2.2.0.tar.gz` & `tmp/cloudcomponents.cdk-github-webhook-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-github-webhook-2.2.0.tar", last modified: Mon Mar 25 18:26:22 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-github-webhook-2.3.0.tar", last modified: Wed Apr 17 18:36:23 2024, max compression
```

## Comparing `cloudcomponents.cdk-github-webhook-2.2.0.tar` & `cloudcomponents.cdk-github-webhook-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:22.896209 cloudcomponents.cdk-github-webhook-2.2.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-03-25 18:26:19.000000 cloudcomponents.cdk-github-webhook-2.2.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-03-25 18:26:19.000000 cloudcomponents.cdk-github-webhook-2.2.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     3543 2024-03-25 18:26:22.896015 cloudcomponents.cdk-github-webhook-2.2.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     2677 2024-03-25 18:26:19.000000 cloudcomponents.cdk-github-webhook-2.2.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-03-25 18:26:19.000000 cloudcomponents.cdk-github-webhook-2.2.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-03-25 18:26:22.896246 cloudcomponents.cdk-github-webhook-2.2.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1853 2024-03-25 18:26:19.000000 cloudcomponents.cdk-github-webhook-2.2.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:22.893477 cloudcomponents.cdk-github-webhook-2.2.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:22.893533 cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:22.895186 cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents/cdk_github_webhook/
--rw-r--r--   0 hupe       (501) staff       (20)     9629 2024-03-25 18:26:19.000000 cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents/cdk_github_webhook/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:22.895455 cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents/cdk_github_webhook/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      477 2024-03-25 18:26:19.000000 cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents/cdk_github_webhook/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)   622921 2024-03-25 18:26:19.000000 cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents/cdk_github_webhook/_jsii/cdk-github-webhook@2.2.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:26:19.000000 cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents/cdk_github_webhook/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:22.894925 cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents.cdk_github_webhook.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     3543 2024-03-25 18:26:22.000000 cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents.cdk_github_webhook.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      597 2024-03-25 18:26:22.000000 cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents.cdk_github_webhook.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:26:22.000000 cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents.cdk_github_webhook.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      157 2024-03-25 18:26:22.000000 cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents.cdk_github_webhook.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-03-25 18:26:22.000000 cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents.cdk_github_webhook.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:23.013466 cloudcomponents.cdk-github-webhook-2.3.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-04-17 18:36:19.000000 cloudcomponents.cdk-github-webhook-2.3.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:36:19.000000 cloudcomponents.cdk-github-webhook-2.3.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     3543 2024-04-17 18:36:23.013126 cloudcomponents.cdk-github-webhook-2.3.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     2677 2024-04-17 18:36:19.000000 cloudcomponents.cdk-github-webhook-2.3.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:36:19.000000 cloudcomponents.cdk-github-webhook-2.3.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:36:23.013529 cloudcomponents.cdk-github-webhook-2.3.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1853 2024-04-17 18:36:19.000000 cloudcomponents.cdk-github-webhook-2.3.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:23.009024 cloudcomponents.cdk-github-webhook-2.3.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:23.009186 cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:23.011415 cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents/cdk_github_webhook/
+-rw-r--r--   0 hupe       (501) staff       (20)     9629 2024-04-17 18:36:19.000000 cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents/cdk_github_webhook/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:23.011711 cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents/cdk_github_webhook/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      477 2024-04-17 18:36:19.000000 cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents/cdk_github_webhook/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)  1827958 2024-04-17 18:36:19.000000 cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents/cdk_github_webhook/_jsii/cdk-github-webhook@2.3.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:36:19.000000 cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents/cdk_github_webhook/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:23.011055 cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents.cdk_github_webhook.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     3543 2024-04-17 18:36:22.000000 cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents.cdk_github_webhook.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      597 2024-04-17 18:36:22.000000 cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents.cdk_github_webhook.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:36:22.000000 cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents.cdk_github_webhook.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      157 2024-04-17 18:36:22.000000 cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents.cdk_github_webhook.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:36:22.000000 cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents.cdk_github_webhook.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-github-webhook-2.2.0/LICENSE` & `cloudcomponents.cdk-github-webhook-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-github-webhook-2.2.0/PKG-INFO` & `cloudcomponents.cdk-github-webhook-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-github-webhook
-Version: 2.2.0
+Version: 2.3.0
 Summary: Create, update and delete github webhooks with your app deployment
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-github-webhook-2.2.0/README.md` & `cloudcomponents.cdk-github-webhook-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-github-webhook-2.2.0/setup.py` & `cloudcomponents.cdk-github-webhook-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-github-webhook",
-    "version": "2.2.0",
+    "version": "2.3.0",
     "description": "Create, update and delete github webhooks with your app deployment",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudcomponents.cdk_github_webhook",
         "cloudcomponents.cdk_github_webhook._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_github_webhook._jsii": [
-            "cdk-github-webhook@2.2.0.jsii.tgz"
+            "cdk-github-webhook@2.3.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_github_webhook": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents/cdk_github_webhook/__init__.py` & `cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents/cdk_github_webhook/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents.cdk_github_webhook.egg-info/PKG-INFO` & `cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents.cdk_github_webhook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-github-webhook
-Version: 2.2.0
+Version: 2.3.0
 Summary: Create, update and delete github webhooks with your app deployment
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-github-webhook-2.2.0/src/cloudcomponents.cdk_github_webhook.egg-info/SOURCES.txt` & `cloudcomponents.cdk-github-webhook-2.3.0/src/cloudcomponents.cdk_github_webhook.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_github_webhook.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_github_webhook.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_github_webhook.egg-info/requires.txt
 src/cloudcomponents.cdk_github_webhook.egg-info/top_level.txt
 src/cloudcomponents/cdk_github_webhook/__init__.py
 src/cloudcomponents/cdk_github_webhook/py.typed
 src/cloudcomponents/cdk_github_webhook/_jsii/__init__.py
-src/cloudcomponents/cdk_github_webhook/_jsii/cdk-github-webhook@2.2.0.jsii.tgz
+src/cloudcomponents/cdk_github_webhook/_jsii/cdk-github-webhook@2.3.0.jsii.tgz
```

