# Comparing `tmp/cloudcomponents.cdk-codecommit-backup-2.1.0.tar.gz` & `tmp/cloudcomponents.cdk-codecommit-backup-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudcomponents.cdk-codecommit-backup-2.1.0.tar", last modified: Mon Mar 25 18:25:28 2024, max compression
+gzip compressed data, was "cloudcomponents.cdk-codecommit-backup-2.2.0.tar", last modified: Thu May 16 19:28:14 2024, max compression
```

## Comparing `cloudcomponents.cdk-codecommit-backup-2.1.0.tar` & `cloudcomponents.cdk-codecommit-backup-2.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.225209 cloudcomponents.cdk-codecommit-backup-2.1.0/
--rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codecommit-backup-2.1.0/LICENSE
--rw-r--r--   0 hupe       (501) staff       (20)       23 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codecommit-backup-2.1.0/MANIFEST.in
--rw-r--r--   0 hupe       (501) staff       (20)     4033 2024-03-25 18:25:28.224751 cloudcomponents.cdk-codecommit-backup-2.1.0/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)     3194 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codecommit-backup-2.1.0/README.md
--rw-r--r--   0 hupe       (501) staff       (20)      234 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codecommit-backup-2.1.0/pyproject.toml
--rw-r--r--   0 hupe       (501) staff       (20)       38 2024-03-25 18:25:28.225316 cloudcomponents.cdk-codecommit-backup-2.1.0/setup.cfg
--rw-r--r--   0 hupe       (501) staff       (20)     1784 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codecommit-backup-2.1.0/setup.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.216524 cloudcomponents.cdk-codecommit-backup-2.1.0/src/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.216622 cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents/
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.223376 cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents/cdk_codecommit_backup/
--rw-r--r--   0 hupe       (501) staff       (20)    86556 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents/cdk_codecommit_backup/__init__.py
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.223862 cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents/cdk_codecommit_backup/_jsii/
--rw-r--r--   0 hupe       (501) staff       (20)      439 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents/cdk_codecommit_backup/_jsii/__init__.py
--rw-r--r--   0 hupe       (501) staff       (20)   130260 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents/cdk_codecommit_backup/_jsii/cdk-codecommit-backup@2.1.0.jsii.tgz
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:23.000000 cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents/cdk_codecommit_backup/py.typed
-drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-03-25 18:25:28.222470 cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/
--rw-r--r--   0 hupe       (501) staff       (20)     4033 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/PKG-INFO
--rw-r--r--   0 hupe       (501) staff       (20)      627 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/SOURCES.txt
--rw-r--r--   0 hupe       (501) staff       (20)        1 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/dependency_links.txt
--rw-r--r--   0 hupe       (501) staff       (20)      112 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/requires.txt
--rw-r--r--   0 hupe       (501) staff       (20)       16 2024-03-25 18:25:28.000000 cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/top_level.txt
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.250881 cloudcomponents.cdk-codecommit-backup-2.2.0/
+-rw-r--r--   0 hupe       (501) staff       (20)     1072 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codecommit-backup-2.2.0/LICENSE
+-rw-r--r--   0 hupe       (501) staff       (20)       23 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codecommit-backup-2.2.0/MANIFEST.in
+-rw-r--r--   0 hupe       (501) staff       (20)     4033 2024-05-16 19:28:14.250587 cloudcomponents.cdk-codecommit-backup-2.2.0/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)     3194 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codecommit-backup-2.2.0/README.md
+-rw-r--r--   0 hupe       (501) staff       (20)      234 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codecommit-backup-2.2.0/pyproject.toml
+-rw-r--r--   0 hupe       (501) staff       (20)       38 2024-05-16 19:28:14.250924 cloudcomponents.cdk-codecommit-backup-2.2.0/setup.cfg
+-rw-r--r--   0 hupe       (501) staff       (20)     1784 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codecommit-backup-2.2.0/setup.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.243696 cloudcomponents.cdk-codecommit-backup-2.2.0/src/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.243779 cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents/
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.249861 cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents/cdk_codecommit_backup/
+-rw-r--r--   0 hupe       (501) staff       (20)    86556 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents/cdk_codecommit_backup/__init__.py
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.250207 cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents/cdk_codecommit_backup/_jsii/
+-rw-r--r--   0 hupe       (501) staff       (20)      439 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents/cdk_codecommit_backup/_jsii/__init__.py
+-rw-r--r--   0 hupe       (501) staff       (20)   131817 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents/cdk_codecommit_backup/_jsii/cdk-codecommit-backup@2.2.0.jsii.tgz
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:28:09.000000 cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents/cdk_codecommit_backup/py.typed
+drwxr-xr-x   0 hupe       (501) staff       (20)        0 2024-05-16 19:28:14.249443 cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/
+-rw-r--r--   0 hupe       (501) staff       (20)     4033 2024-05-16 19:28:14.000000 cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/PKG-INFO
+-rw-r--r--   0 hupe       (501) staff       (20)      627 2024-05-16 19:28:14.000000 cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 hupe       (501) staff       (20)        1 2024-05-16 19:28:14.000000 cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 hupe       (501) staff       (20)      112 2024-05-16 19:28:14.000000 cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/requires.txt
+-rw-r--r--   0 hupe       (501) staff       (20)       16 2024-05-16 19:28:14.000000 cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/top_level.txt
```

### Comparing `cloudcomponents.cdk-codecommit-backup-2.1.0/LICENSE` & `cloudcomponents.cdk-codecommit-backup-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-codecommit-backup-2.1.0/PKG-INFO` & `cloudcomponents.cdk-codecommit-backup-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-codecommit-backup
-Version: 2.1.0
+Version: 2.2.0
 Summary: Backup CodeCommit repositories to S3
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-codecommit-backup-2.1.0/README.md` & `cloudcomponents.cdk-codecommit-backup-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-codecommit-backup-2.1.0/setup.py` & `cloudcomponents.cdk-codecommit-backup-2.2.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudcomponents.cdk-codecommit-backup",
-    "version": "2.1.0",
+    "version": "2.2.0",
     "description": "Backup CodeCommit repositories to S3",
     "license": "MIT",
     "url": "https://github.com/cloudcomponents/cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "hupe1980",
     "bdist_wheel": {
         "universal": true
@@ -22,24 +22,24 @@
     },
     "packages": [
         "cloudcomponents.cdk_codecommit_backup",
         "cloudcomponents.cdk_codecommit_backup._jsii"
     ],
     "package_data": {
         "cloudcomponents.cdk_codecommit_backup._jsii": [
-            "cdk-codecommit-backup@2.1.0.jsii.tgz"
+            "cdk-codecommit-backup@2.2.0.jsii.tgz"
         ],
         "cloudcomponents.cdk_codecommit_backup": [
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

### Comparing `cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents/cdk_codecommit_backup/__init__.py` & `cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents/cdk_codecommit_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/PKG-INFO` & `cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudcomponents.cdk-codecommit-backup
-Version: 2.1.0
+Version: 2.2.0
 Summary: Backup CodeCommit repositories to S3
 Home-page: https://github.com/cloudcomponents/cdk-constructs
 Author: hupe1980
 License: MIT
 Project-URL: Source, https://github.com/cloudcomponents/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudcomponents.cdk-codecommit-backup-2.1.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/SOURCES.txt` & `cloudcomponents.cdk-codecommit-backup-2.2.0/src/cloudcomponents.cdk_codecommit_backup.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/cloudcomponents.cdk_codecommit_backup.egg-info/SOURCES.txt
 src/cloudcomponents.cdk_codecommit_backup.egg-info/dependency_links.txt
 src/cloudcomponents.cdk_codecommit_backup.egg-info/requires.txt
 src/cloudcomponents.cdk_codecommit_backup.egg-info/top_level.txt
 src/cloudcomponents/cdk_codecommit_backup/__init__.py
 src/cloudcomponents/cdk_codecommit_backup/py.typed
 src/cloudcomponents/cdk_codecommit_backup/_jsii/__init__.py
-src/cloudcomponents/cdk_codecommit_backup/_jsii/cdk-codecommit-backup@2.1.0.jsii.tgz
+src/cloudcomponents/cdk_codecommit_backup/_jsii/cdk-codecommit-backup@2.2.0.jsii.tgz
```

