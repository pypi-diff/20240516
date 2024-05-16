# Comparing `tmp/cloudcomponents.cdk-static-website-2.1.0.tar.gz` & `tmp/cloudcomponents.cdk-static-website-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-static-website-2.1.0.tar", last modified: Mon Mar 25 18:26:09 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-static-website-2.2.0.tar", last modified: Thu May 16 19:32:59 2024, max compression
```

## Comparing `cloudcomponents.cdk-static-website-2.1.0.tar` & `cloudcomponents.cdk-static-website-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:09.183105 cloudcomponents.cdk-static-website-2.1.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-03-25 18:26:05.000000 cloudcomponents.cdk-static-website-2.1.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-03-25 18:26:05.000000 cloudcomponents.cdk-static-website-2.1.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     4910 2024-03-25 18:26:09.182842 cloudcomponents.cdk-static-website-2.1.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     3986 2024-03-25 18:26:05.000000 cloudcomponents.cdk-static-website-2.1.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-03-25 18:26:05.000000 cloudcomponents.cdk-static-website-2.1.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-03-25 18:26:09.183151 cloudcomponents.cdk-static-website-2.1.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1854 2024-03-25 18:26:05.000000 cloudcomponents.cdk-static-website-2.1.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:09.180169 cloudcomponents.cdk-static-website-2.1.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:09.180229 cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:09.182260 cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents/cdk_static_website/
--rw-r--r--   0 hupe       (501) staff       (20)    51256 2024-03-25 18:26:05.000000 cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents/cdk_static_website/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:09.182536 cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents/cdk_static_website/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      433 2024-03-25 18:26:05.000000 cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents/cdk_static_website/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)   135757 2024-03-25 18:26:05.000000 cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents/cdk_static_website/_jsii/cdk-static-website@2.1.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:26:05.000000 cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents/cdk_static_website/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:26:09.181905 cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents.cdk_static_website.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     4910 2024-03-25 18:26:09.000000 cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents.cdk_static_website.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      597 2024-03-25 18:26:09.000000 cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents.cdk_static_website.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:26:09.000000 cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents.cdk_static_website.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-03-25 18:26:09.000000 cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents.cdk_static_website.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-03-25 18:26:09.000000 cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents.cdk_static_website.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.530455 cloudcomponents.cdk-static-website-2.2.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-05-16 19:32:55.000000 cloudcomponents.cdk-static-website-2.2.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-05-16 19:32:55.000000 cloudcomponents.cdk-static-website-2.2.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     4910 2024-05-16 19:32:59.530122 cloudcomponents.cdk-static-website-2.2.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     3986 2024-05-16 19:32:55.000000 cloudcomponents.cdk-static-website-2.2.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-05-16 19:32:55.000000 cloudcomponents.cdk-static-website-2.2.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-05-16 19:32:59.530511 cloudcomponents.cdk-static-website-2.2.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1854 2024-05-16 19:32:55.000000 cloudcomponents.cdk-static-website-2.2.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.526826 cloudcomponents.cdk-static-website-2.2.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.526902 cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.529145 cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents/cdk_static_website/
+-rw-r--r--   0 hupe       (501) staff       (20)    51256 2024-05-16 19:32:55.000000 cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents/cdk_static_website/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.529613 cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents/cdk_static_website/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      433 2024-05-16 19:32:55.000000 cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents/cdk_static_website/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)   137507 2024-05-16 19:32:55.000000 cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents/cdk_static_website/_jsii/cdk-static-website@2.2.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:32:55.000000 cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents/cdk_static_website/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:32:59.528751 cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents.cdk_static_website.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     4910 2024-05-16 19:32:59.000000 cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents.cdk_static_website.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      597 2024-05-16 19:32:59.000000 cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents.cdk_static_website.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:32:59.000000 cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents.cdk_static_website.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-05-16 19:32:59.000000 cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents.cdk_static_website.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-05-16 19:32:59.000000 cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents.cdk_static_website.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-static-website-2.1.0/LICENSE` & `cloudcomponents.cdk-static-website-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-static-website-2.1.0/PKG-INFO` & `cloudcomponents.cdk-static-website-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-static-website
-Version: 2.1.0
+Version: 2.2.0
 Summary: Cdk component that creates a static website using S3, configures CloudFront (CDN) and maps a custom domain via Route53 (DNS)
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-static-website-2.1.0/README.md` & `cloudcomponents.cdk-static-website-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-static-website-2.1.0/setup.py` & `cloudcomponents.cdk-static-website-2.2.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-static-website",
-    "version": "2.1.0",
+    "version": "2.2.0",
     "description": "Cdk component that creates a static website using S3, configures CloudFront (CDN) and maps a custom domain via Route53 (DNS)",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cloudcomponents.cdk_static_website",
         "cloudcomponents.cdk_static_website._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_static_website._jsii": [
-            "cdk-static-website@2.1.0.jsii.tgz"
+            "cdk-static-website@2.2.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_static_website": [
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

### Comparing `cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents/cdk_static_website/__init__.py` & `cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents/cdk_static_website/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents.cdk_static_website.egg-info/PKG-INFO` & `cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents.cdk_static_website.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-static-website
-Version: 2.1.0
+Version: 2.2.0
 Summary: Cdk component that creates a static website using S3, configures CloudFront (CDN) and maps a custom domain via Route53 (DNS)
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-static-website-2.1.0/src/cloudcomponents.cdk_static_website.egg-info/SOURCES.txt` & `cloudcomponents.cdk-static-website-2.2.0/src/cloudcomponents.cdk_static_website.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_static_website.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_static_website.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_static_website.egg-info/requires.txt
 src/cloudcomponents.cdk_static_website.egg-info/top_level.txt
 src/cloudcomponents/cdk_static_website/__init__.py
 src/cloudcomponents/cdk_static_website/py.typed
 src/cloudcomponents/cdk_static_website/_jsii/__init__.py
-src/cloudcomponents/cdk_static_website/_jsii/cdk-static-website@2.1.0.jsii.tgz
+src/cloudcomponents/cdk_static_website/_jsii/cdk-static-website@2.2.0.jsii.tgz
```

