# Comparing `tmp/BarteSDK-0.1.tar.gz` & `tmp/BarteSDK-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BarteSDK-0.1.tar", last modified: Wed May 15 19:55:37 2024, max compression
+gzip compressed data, was "BarteSDK-0.1.1.tar", last modified: Wed May 15 19:56:18 2024, max compression
```

## Comparing `BarteSDK-0.1.tar` & `BarteSDK-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 19:55:37.800179 BarteSDK-0.1/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 19:55:37.796180 BarteSDK-0.1/BarteChargesAPI/
--rw-rw-r--   0 root         (0) root         (0)       34 2024-05-15 19:54:15.000000 BarteSDK-0.1/BarteChargesAPI/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      405 2024-05-15 19:54:15.000000 BarteSDK-0.1/BarteChargesAPI/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 19:55:37.796180 BarteSDK-0.1/BarteReportAPI/
--rw-rw-r--   0 root         (0) root         (0)       33 2024-05-15 19:54:15.000000 BarteSDK-0.1/BarteReportAPI/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      718 2024-05-15 19:54:15.000000 BarteSDK-0.1/BarteReportAPI/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 19:55:37.800179 BarteSDK-0.1/BarteSDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4102 2024-05-15 19:55:37.000000 BarteSDK-0.1/BarteSDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      287 2024-05-15 19:55:37.000000 BarteSDK-0.1/BarteSDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 19:55:37.000000 BarteSDK-0.1/BarteSDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-15 19:55:37.000000 BarteSDK-0.1/BarteSDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-15 19:55:37.000000 BarteSDK-0.1/BarteSDK.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 19:54:15.000000 BarteSDK-0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4102 2024-05-15 19:55:37.800179 BarteSDK-0.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3828 2024-05-15 19:54:15.000000 BarteSDK-0.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 19:55:37.800179 BarteSDK-0.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      560 2024-05-15 19:55:23.000000 BarteSDK-0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 19:56:18.620929 BarteSDK-0.1.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 19:56:18.616929 BarteSDK-0.1.1/BarteChargesAPI/
+-rw-rw-r--   0 root         (0) root         (0)       34 2024-05-15 19:54:15.000000 BarteSDK-0.1.1/BarteChargesAPI/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      405 2024-05-15 19:54:15.000000 BarteSDK-0.1.1/BarteChargesAPI/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 19:56:18.616929 BarteSDK-0.1.1/BarteReportAPI/
+-rw-rw-r--   0 root         (0) root         (0)       33 2024-05-15 19:54:15.000000 BarteSDK-0.1.1/BarteReportAPI/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      718 2024-05-15 19:54:15.000000 BarteSDK-0.1.1/BarteReportAPI/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 19:56:18.616929 BarteSDK-0.1.1/BarteSDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4104 2024-05-15 19:56:18.000000 BarteSDK-0.1.1/BarteSDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      287 2024-05-15 19:56:18.000000 BarteSDK-0.1.1/BarteSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 19:56:18.000000 BarteSDK-0.1.1/BarteSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-15 19:56:18.000000 BarteSDK-0.1.1/BarteSDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-15 19:56:18.000000 BarteSDK-0.1.1/BarteSDK.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-05-15 19:54:15.000000 BarteSDK-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4104 2024-05-15 19:56:18.620929 BarteSDK-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3828 2024-05-15 19:54:15.000000 BarteSDK-0.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 19:56:18.620929 BarteSDK-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      562 2024-05-15 19:56:05.000000 BarteSDK-0.1.1/setup.py
```

### Comparing `BarteSDK-0.1/BarteReportAPI/main.py` & `BarteSDK-0.1.1/BarteReportAPI/main.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-0.1/BarteSDK.egg-info/PKG-INFO` & `BarteSDK-0.1.1/BarteSDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 0.1
+Version: 0.1.1
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-0.1/PKG-INFO` & `BarteSDK-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 0.1
+Version: 0.1.1
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-0.1/README.md` & `BarteSDK-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `BarteSDK-0.1/setup.py` & `BarteSDK-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='BarteSDK',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Engenharia de Plataforma da Barte',
     author_email='devops@barte.com',
     description='SDK para interação com a API da Barte.',
```

