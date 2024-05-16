# Comparing `tmp/cloudcomponents.cdk-responsive-email-template-2.2.0.tar.gz` & `tmp/cloudcomponents.cdk-responsive-email-template-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-responsive-email-template-2.2.0.tar", last modified: Mon Mar 25 18:25:56 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-responsive-email-template-2.3.0.tar", last modified: Thu May 16 19:32:59 2024, max compression
```

## Comparing `cloudcomponents.cdk-responsive-email-template-2.2.0.tar` & `cloudcomponents.cdk-responsive-email-template-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:56.867516 cloudcomponents.cdk-responsive-email-template-2.2.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-03-25 18:25:53.000000 cloudcomponents.cdk-responsive-email-template-2.2.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-03-25 18:25:53.000000 cloudcomponents.cdk-responsive-email-template-2.2.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     3248 2024-03-25 18:25:56.867268 cloudcomponents.cdk-responsive-email-template-2.2.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     2400 2024-03-25 18:25:53.000000 cloudcomponents.cdk-responsive-email-template-2.2.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-03-25 18:25:53.000000 cloudcomponents.cdk-responsive-email-template-2.2.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-03-25 18:25:56.867593 cloudcomponents.cdk-responsive-email-template-2.2.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1833 2024-03-25 18:25:53.000000 cloudcomponents.cdk-responsive-email-template-2.2.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:56.864981 cloudcomponents.cdk-responsive-email-template-2.2.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:56.865046 cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:56.866758 cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents/cdk_responsive_email_template/
--rw-r--r--   0 hupe       (501) staff       (20)    18430 2024-03-25 18:25:53.000000 cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents/cdk_responsive_email_template/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:56.867032 cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents/cdk_responsive_email_template/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      455 2024-03-25 18:25:53.000000 cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents/cdk_responsive_email_template/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)    48884 2024-03-25 18:25:53.000000 cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents/cdk_responsive_email_template/_jsii/cdk-responsive-email-template@2.2.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:53.000000 cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents/cdk_responsive_email_template/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:56.866474 cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     3248 2024-03-25 18:25:56.000000 cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      707 2024-03-25 18:25:56.000000 cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:56.000000 cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-03-25 18:25:56.000000 cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-03-25 18:25:56.000000 cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.594340 cloudcomponents.cdk-responsive-email-template-2.3.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-05-16 19:32:55.000000 cloudcomponents.cdk-responsive-email-template-2.3.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-05-16 19:32:55.000000 cloudcomponents.cdk-responsive-email-template-2.3.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     3248 2024-05-16 19:32:59.594075 cloudcomponents.cdk-responsive-email-template-2.3.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     2400 2024-05-16 19:32:55.000000 cloudcomponents.cdk-responsive-email-template-2.3.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-05-16 19:32:55.000000 cloudcomponents.cdk-responsive-email-template-2.3.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-05-16 19:32:59.594389 cloudcomponents.cdk-responsive-email-template-2.3.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1833 2024-05-16 19:32:55.000000 cloudcomponents.cdk-responsive-email-template-2.3.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.591240 cloudcomponents.cdk-responsive-email-template-2.3.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.591309 cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.593450 cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents/cdk_responsive_email_template/
+-rw-r--r--   0 hupe       (501) staff       (20)    18430 2024-05-16 19:32:55.000000 cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents/cdk_responsive_email_template/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.593777 cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents/cdk_responsive_email_template/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      455 2024-05-16 19:32:55.000000 cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents/cdk_responsive_email_template/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)    49277 2024-05-16 19:32:55.000000 cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents/cdk_responsive_email_template/_jsii/cdk-responsive-email-template@2.3.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:32:55.000000 cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents/cdk_responsive_email_template/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.593087 cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     3248 2024-05-16 19:32:59.000000 cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      707 2024-05-16 19:32:59.000000 cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:32:59.000000 cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-05-16 19:32:59.000000 cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-05-16 19:32:59.000000 cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-responsive-email-template-2.2.0/LICENSE` & `cloudcomponents.cdk-responsive-email-template-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-responsive-email-template-2.2.0/PKG-INFO` & `cloudcomponents.cdk-responsive-email-template-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-responsive-email-template
-Version: 2.2.0
+Version: 2.3.0
 Summary: Responsive email template for aws ses
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-responsive-email-template-2.2.0/README.md` & `cloudcomponents.cdk-responsive-email-template-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-responsive-email-template-2.2.0/setup.py` & `cloudcomponents.cdk-responsive-email-template-2.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-responsive-email-template",
-    "version": "2.2.0",
+    "version": "2.3.0",
     "description": "Responsive email template for aws ses",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cloudcomponents.cdk_responsive_email_template",
         "cloudcomponents.cdk_responsive_email_template._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_responsive_email_template._jsii": [
-            "cdk-responsive-email-template@2.2.0.jsii.tgz"
+            "cdk-responsive-email-template@2.3.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_responsive_email_template": [
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

### Comparing `cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents/cdk_responsive_email_template/__init__.py` & `cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents/cdk_responsive_email_template/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/PKG-INFO` & `cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-responsive-email-template
-Version: 2.2.0
+Version: 2.3.0
 Summary: Responsive email template for aws ses
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-responsive-email-template-2.2.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/SOURCES.txt` & `cloudcomponents.cdk-responsive-email-template-2.3.0/src/cloudcomponents.cdk_responsive_email_template.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_responsive_email_template.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_responsive_email_template.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_responsive_email_template.egg-info/requires.txt
 src/cloudcomponents.cdk_responsive_email_template.egg-info/top_level.txt
 src/cloudcomponents/cdk_responsive_email_template/__init__.py
 src/cloudcomponents/cdk_responsive_email_template/py.typed
 src/cloudcomponents/cdk_responsive_email_template/_jsii/__init__.py
-src/cloudcomponents/cdk_responsive_email_template/_jsii/cdk-responsive-email-template@2.2.0.jsii.tgz
+src/cloudcomponents/cdk_responsive_email_template/_jsii/cdk-responsive-email-template@2.3.0.jsii.tgz
```

