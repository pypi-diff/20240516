# Comparing `tmp/NJFU-0.0.5.tar.gz` & `tmp/NJFU-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NJFU-0.0.5.tar", last modified: Fri May 10 03:07:21 2024, max compression
+gzip compressed data, was "NJFU-0.0.6.tar", last modified: Thu May 16 02:57:43 2024, max compression
```

## Comparing `NJFU-0.0.5.tar` & `NJFU-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 03:07:21.870636 NJFU-0.0.5/
-drwxrwxrwx   0        0        0        0 2024-05-10 03:07:21.866650 NJFU-0.0.5/NJFU/
--rw-rw-rw-   0        0        0       87 2024-05-08 08:29:37.000000 NJFU-0.0.5/NJFU/__init__.py
--rw-rw-rw-   0        0        0       61 2024-05-07 09:27:16.000000 NJFU-0.0.5/NJFU/hello.py
--rw-rw-rw-   0        0        0    19420 2024-05-08 10:54:30.000000 NJFU-0.0.5/NJFU/utils.py
--rw-rw-rw-   0        0        0     9645 2024-05-10 03:03:13.000000 NJFU-0.0.5/NJFU/yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-10 03:07:21.869640 NJFU-0.0.5/NJFU.egg-info/
--rw-rw-rw-   0        0        0      900 2024-05-10 03:07:21.000000 NJFU-0.0.5/NJFU.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2024-05-10 03:07:21.000000 NJFU-0.0.5/NJFU.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 03:07:21.000000 NJFU-0.0.5/NJFU.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-10 03:07:21.000000 NJFU-0.0.5/NJFU.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      900 2024-05-10 03:07:21.870636 NJFU-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-10 03:07:21.870636 NJFU-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1060 2024-05-10 03:07:19.000000 NJFU-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 02:57:43.870825 NJFU-0.0.6/
+drwxrwxrwx   0        0        0        0 2024-05-16 02:57:43.865841 NJFU-0.0.6/NJFU/
+-rw-rw-rw-   0        0        0      113 2024-05-16 02:57:18.000000 NJFU-0.0.6/NJFU/__init__.py
+-rw-rw-rw-   0        0        0       61 2024-05-07 09:27:16.000000 NJFU-0.0.6/NJFU/hello.py
+-rw-rw-rw-   0        0        0      321 2024-05-16 02:56:40.000000 NJFU-0.0.6/NJFU/pcd.py
+-rw-rw-rw-   0        0        0    19420 2024-05-08 10:54:30.000000 NJFU-0.0.6/NJFU/utils.py
+-rw-rw-rw-   0        0        0     9645 2024-05-10 03:03:13.000000 NJFU-0.0.6/NJFU/yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-16 02:57:43.869828 NJFU-0.0.6/NJFU.egg-info/
+-rw-rw-rw-   0        0        0      900 2024-05-16 02:57:43.000000 NJFU-0.0.6/NJFU.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-16 02:57:43.000000 NJFU-0.0.6/NJFU.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 02:57:43.000000 NJFU-0.0.6/NJFU.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-16 02:57:43.000000 NJFU-0.0.6/NJFU.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      900 2024-05-16 02:57:43.869828 NJFU-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-16 02:57:43.870825 NJFU-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1060 2024-05-16 02:57:31.000000 NJFU-0.0.6/setup.py
```

### Comparing `NJFU-0.0.5/NJFU/utils.py` & `NJFU-0.0.6/NJFU/utils.py`

 * *Files identical despite different names*

### Comparing `NJFU-0.0.5/NJFU/yolo.py` & `NJFU-0.0.6/NJFU/yolo.py`

 * *Files identical despite different names*

### Comparing `NJFU-0.0.5/NJFU.egg-info/PKG-INFO` & `NJFU-0.0.6/NJFU.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NJFU
-Version: 0.0.5
+Version: 0.0.6
 Summary: NJFU
 Home-page: https://github.com/
 Author: XHF
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
```

### Comparing `NJFU-0.0.5/PKG-INFO` & `NJFU-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NJFU
-Version: 0.0.5
+Version: 0.0.6
 Summary: NJFU
 Home-page: https://github.com/
 Author: XHF
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
```

### Comparing `NJFU-0.0.5/setup.py` & `NJFU-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="NJFU",
-    version="0.0.5",
+    version="0.0.6",
     author="XHF",
 
     description="NJFU",
 
     Long_description_content_type="Tool for NJFU",
     url="https://github.com/",
     packages=setuptools.find_packages(),
```

