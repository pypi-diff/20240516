# Comparing `tmp/NJFU-0.0.8.tar.gz` & `tmp/NJFU-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NJFU-0.0.8.tar", last modified: Thu May 16 03:02:04 2024, max compression
+gzip compressed data, was "NJFU-0.0.9.tar", last modified: Thu May 16 03:03:08 2024, max compression
```

## Comparing `NJFU-0.0.8.tar` & `NJFU-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 03:02:04.034297 NJFU-0.0.8/
-drwxrwxrwx   0        0        0        0 2024-05-16 03:02:04.029314 NJFU-0.0.8/NJFU/
--rw-rw-rw-   0        0        0      113 2024-05-16 03:01:57.000000 NJFU-0.0.8/NJFU/__init__.py
--rw-rw-rw-   0        0        0       61 2024-05-07 09:27:16.000000 NJFU-0.0.8/NJFU/hello.py
--rw-rw-rw-   0        0        0      321 2024-05-16 02:56:40.000000 NJFU-0.0.8/NJFU/pcd.py
--rw-rw-rw-   0        0        0    19420 2024-05-08 10:54:30.000000 NJFU-0.0.8/NJFU/utils.py
--rw-rw-rw-   0        0        0     9646 2024-05-16 03:01:57.000000 NJFU-0.0.8/NJFU/yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-16 03:02:04.033301 NJFU-0.0.8/NJFU.egg-info/
--rw-rw-rw-   0        0        0      900 2024-05-16 03:02:03.000000 NJFU-0.0.8/NJFU.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-16 03:02:03.000000 NJFU-0.0.8/NJFU.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 03:02:03.000000 NJFU-0.0.8/NJFU.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-16 03:02:03.000000 NJFU-0.0.8/NJFU.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      900 2024-05-16 03:02:04.033301 NJFU-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-16 03:02:04.034297 NJFU-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1060 2024-05-16 03:02:01.000000 NJFU-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 03:03:08.862478 NJFU-0.0.9/
+drwxrwxrwx   0        0        0        0 2024-05-16 03:03:08.858492 NJFU-0.0.9/NJFU/
+-rw-rw-rw-   0        0        0      113 2024-05-16 03:01:57.000000 NJFU-0.0.9/NJFU/__init__.py
+-rw-rw-rw-   0        0        0       61 2024-05-07 09:27:16.000000 NJFU-0.0.9/NJFU/hello.py
+-rw-rw-rw-   0        0        0      322 2024-05-16 03:02:57.000000 NJFU-0.0.9/NJFU/pcd.py
+-rw-rw-rw-   0        0        0    19420 2024-05-08 10:54:30.000000 NJFU-0.0.9/NJFU/utils.py
+-rw-rw-rw-   0        0        0     9646 2024-05-16 03:01:57.000000 NJFU-0.0.9/NJFU/yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-16 03:03:08.861482 NJFU-0.0.9/NJFU.egg-info/
+-rw-rw-rw-   0        0        0      900 2024-05-16 03:03:08.000000 NJFU-0.0.9/NJFU.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-16 03:03:08.000000 NJFU-0.0.9/NJFU.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 03:03:08.000000 NJFU-0.0.9/NJFU.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-16 03:03:08.000000 NJFU-0.0.9/NJFU.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      900 2024-05-16 03:03:08.862478 NJFU-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-16 03:03:08.862478 NJFU-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1060 2024-05-16 03:03:07.000000 NJFU-0.0.9/setup.py
```

### Comparing `NJFU-0.0.8/NJFU/utils.py` & `NJFU-0.0.9/NJFU/utils.py`

 * *Files identical despite different names*

### Comparing `NJFU-0.0.8/NJFU/yolo.py` & `NJFU-0.0.9/NJFU/yolo.py`

 * *Files identical despite different names*

### Comparing `NJFU-0.0.8/NJFU.egg-info/PKG-INFO` & `NJFU-0.0.9/NJFU.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NJFU
-Version: 0.0.8
+Version: 0.0.9
 Summary: NJFU
 Home-page: https://github.com/
 Author: XHF
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
```

### Comparing `NJFU-0.0.8/PKG-INFO` & `NJFU-0.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NJFU
-Version: 0.0.8
+Version: 0.0.9
 Summary: NJFU
 Home-page: https://github.com/
 Author: XHF
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 2
```

### Comparing `NJFU-0.0.8/setup.py` & `NJFU-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="NJFU",
-    version="0.0.8",
+    version="0.0.9",
     author="XHF",
 
     description="NJFU",
 
     Long_description_content_type="Tool for NJFU",
     url="https://github.com/",
     packages=setuptools.find_packages(),
```

