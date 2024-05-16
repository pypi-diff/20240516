# Comparing `tmp/cloudcomponents.cdk-stripe-webhook-2.3.0.tar.gz` & `tmp/cloudcomponents.cdk-stripe-webhook-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-stripe-webhook-2.3.0.tar", last modified: Wed Apr 17 18:36:23 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-stripe-webhook-2.4.0.tar", last modified: Thu May 16 19:33:26 2024, max compression
```

## Comparing `cloudcomponents.cdk-stripe-webhook-2.3.0.tar` & `cloudcomponents.cdk-stripe-webhook-2.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:23.683142 cloudcomponents.cdk-stripe-webhook-2.3.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-04-17 18:36:20.000000 cloudcomponents.cdk-stripe-webhook-2.3.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-04-17 18:36:20.000000 cloudcomponents.cdk-stripe-webhook-2.3.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     4454 2024-04-17 18:36:23.682845 cloudcomponents.cdk-stripe-webhook-2.3.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     3588 2024-04-17 18:36:20.000000 cloudcomponents.cdk-stripe-webhook-2.3.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-04-17 18:36:20.000000 cloudcomponents.cdk-stripe-webhook-2.3.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-04-17 18:36:23.683186 cloudcomponents.cdk-stripe-webhook-2.3.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1853 2024-04-17 18:36:20.000000 cloudcomponents.cdk-stripe-webhook-2.3.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:23.677720 cloudcomponents.cdk-stripe-webhook-2.3.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:23.677786 cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:23.679774 cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents/cdk_stripe_webhook/
--rw-r--r--   0 hupe       (501) staff       (20)    18806 2024-04-17 18:36:20.000000 cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents/cdk_stripe_webhook/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:23.680172 cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents/cdk_stripe_webhook/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      477 2024-04-17 18:36:20.000000 cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents/cdk_stripe_webhook/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)  3097486 2024-04-17 18:36:20.000000 cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents/cdk_stripe_webhook/_jsii/cdk-stripe-webhook@2.3.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:36:20.000000 cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents/cdk_stripe_webhook/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-04-17 18:36:23.679406 cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     4454 2024-04-17 18:36:23.000000 cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      597 2024-04-17 18:36:23.000000 cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-04-17 18:36:23.000000 cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      157 2024-04-17 18:36:23.000000 cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-04-17 18:36:23.000000 cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:26.934800 cloudcomponents.cdk-stripe-webhook-2.4.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-05-16 19:33:23.000000 cloudcomponents.cdk-stripe-webhook-2.4.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-05-16 19:33:23.000000 cloudcomponents.cdk-stripe-webhook-2.4.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     4454 2024-05-16 19:33:26.934574 cloudcomponents.cdk-stripe-webhook-2.4.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     3588 2024-05-16 19:33:23.000000 cloudcomponents.cdk-stripe-webhook-2.4.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-05-16 19:33:23.000000 cloudcomponents.cdk-stripe-webhook-2.4.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-05-16 19:33:26.934840 cloudcomponents.cdk-stripe-webhook-2.4.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1853 2024-05-16 19:33:23.000000 cloudcomponents.cdk-stripe-webhook-2.4.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:26.931472 cloudcomponents.cdk-stripe-webhook-2.4.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:26.931531 cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:26.933526 cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents/cdk_stripe_webhook/
+-rw-r--r--   0 hupe       (501) staff       (20)    18806 2024-05-16 19:33:23.000000 cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents/cdk_stripe_webhook/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:26.933860 cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents/cdk_stripe_webhook/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      477 2024-05-16 19:33:23.000000 cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents/cdk_stripe_webhook/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)   694952 2024-05-16 19:33:23.000000 cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents/cdk_stripe_webhook/_jsii/cdk-stripe-webhook@2.4.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:33:23.000000 cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents/cdk_stripe_webhook/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:33:26.933215 cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     4454 2024-05-16 19:33:26.000000 cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      597 2024-05-16 19:33:26.000000 cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:33:26.000000 cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      157 2024-05-16 19:33:26.000000 cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-05-16 19:33:26.000000 cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-stripe-webhook-2.3.0/LICENSE` & `cloudcomponents.cdk-stripe-webhook-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-stripe-webhook-2.3.0/PKG-INFO` & `cloudcomponents.cdk-stripe-webhook-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-stripe-webhook
-Version: 2.3.0
+Version: 2.4.0
 Summary: Create, update and delete stripe webhooks with your app deployment
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-stripe-webhook-2.3.0/README.md` & `cloudcomponents.cdk-stripe-webhook-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-stripe-webhook-2.3.0/setup.py` & `cloudcomponents.cdk-stripe-webhook-2.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-stripe-webhook",
-    "version": "2.3.0",
+    "version": "2.4.0",
     "description": "Create, update and delete stripe webhooks with your app deployment",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "cloudcomponents.cdk_stripe_webhook",
         "cloudcomponents.cdk_stripe_webhook._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_stripe_webhook._jsii": [
-            "cdk-stripe-webhook@2.3.0.jsii.tgz"
+            "cdk-stripe-webhook@2.4.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_stripe_webhook": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
-        "aws-cdk-lib>=2.28.0, <3.0.0",
-        "cloudcomponents.cdk-secret-key>=2.1.0, <3.0.0",
-        "constructs>=10.0.41, <11.0.0",
+        "aws-cdk-lib>=2.141.0, <3.0.0",
+        "cloudcomponents.cdk-secret-key>=2.2.0, <3.0.0",
+        "constructs>=10.3.0, <11.0.0",
         "jsii>=1.95.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents/cdk_stripe_webhook/__init__.py` & `cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents/cdk_stripe_webhook/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/PKG-INFO` & `cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-stripe-webhook
-Version: 2.3.0
+Version: 2.4.0
 Summary: Create, update and delete stripe webhooks with your app deployment
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-stripe-webhook-2.3.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/SOURCES.txt` & `cloudcomponents.cdk-stripe-webhook-2.4.0/src/cloudcomponents.cdk_stripe_webhook.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_stripe_webhook.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_stripe_webhook.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_stripe_webhook.egg-info/requires.txt
 src/cloudcomponents.cdk_stripe_webhook.egg-info/top_level.txt
 src/cloudcomponents/cdk_stripe_webhook/__init__.py
 src/cloudcomponents/cdk_stripe_webhook/py.typed
 src/cloudcomponents/cdk_stripe_webhook/_jsii/__init__.py
-src/cloudcomponents/cdk_stripe_webhook/_jsii/cdk-stripe-webhook@2.3.0.jsii.tgz
+src/cloudcomponents/cdk_stripe_webhook/_jsii/cdk-stripe-webhook@2.4.0.jsii.tgz
```

