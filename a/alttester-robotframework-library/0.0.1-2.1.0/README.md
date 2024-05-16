# Comparing `tmp/alttester-robotframework-library-0.0.1.tar.gz` & `tmp/alttester_robotframework_library-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alttester-robotframework-library-0.0.1.tar", last modified: Thu Apr  4 09:40:12 2024, max compression
+gzip compressed data, was "alttester_robotframework_library-2.1.0.tar", last modified: Mon Apr 15 10:33:33 2024, max compression
```

## Comparing `alttester-robotframework-library-0.0.1.tar` & `alttester_robotframework_library-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-04 09:40:12.234383 alttester-robotframework-library-0.0.1/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1776 2024-04-04 09:40:12.233396 alttester-robotframework-library-0.0.1/PKG-INFO
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      373 2024-02-12 15:33:36.000000 alttester-robotframework-library-0.0.1/README.md
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       38 2024-04-04 09:40:12.234632 alttester-robotframework-library-0.0.1/setup.cfg
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     2907 2024-02-12 15:33:36.000000 alttester-robotframework-library-0.0.1/setup.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-04 09:40:12.223520 alttester-robotframework-library-0.0.1/src/
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-04 09:40:12.227038 alttester-robotframework-library-0.0.1/src/AltTesterLibrary/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)    55503 2024-04-01 07:09:49.000000 alttester-robotframework-library-0.0.1/src/AltTesterLibrary/AltTesterKeywords.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1323 2024-04-01 07:09:49.000000 alttester-robotframework-library-0.0.1/src/AltTesterLibrary/__init__.py
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      718 2024-04-04 08:40:10.000000 alttester-robotframework-library-0.0.1/src/AltTesterLibrary/version.py
-drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-04 09:40:12.232382 alttester-robotframework-library-0.0.1/src/alttester_robotframework_library.egg-info/
--rw-r--r--   0 gitlabrunner   (501) staff       (20)     1776 2024-04-04 09:40:12.000000 alttester-robotframework-library-0.0.1/src/alttester_robotframework_library.egg-info/PKG-INFO
--rw-r--r--   0 gitlabrunner   (501) staff       (20)      483 2024-04-04 09:40:12.000000 alttester-robotframework-library-0.0.1/src/alttester_robotframework_library.egg-info/SOURCES.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2024-04-04 09:40:12.000000 alttester-robotframework-library-0.0.1/src/alttester_robotframework_library.egg-info/dependency_links.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2024-04-04 07:24:26.000000 alttester-robotframework-library-0.0.1/src/alttester_robotframework_library.egg-info/not-zip-safe
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       37 2024-04-04 09:40:12.000000 alttester-robotframework-library-0.0.1/src/alttester_robotframework_library.egg-info/requires.txt
--rw-r--r--   0 gitlabrunner   (501) staff       (20)       17 2024-04-04 09:40:12.000000 alttester-robotframework-library-0.0.1/src/alttester_robotframework_library.egg-info/top_level.txt
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:33.027177 alttester_robotframework_library-2.1.0/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1776 2024-04-15 10:33:33.025931 alttester_robotframework_library-2.1.0/PKG-INFO
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      373 2024-02-12 15:33:36.000000 alttester_robotframework_library-2.1.0/README.md
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       38 2024-04-15 10:33:33.027358 alttester_robotframework_library-2.1.0/setup.cfg
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     2907 2024-02-12 15:33:36.000000 alttester_robotframework_library-2.1.0/setup.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:33.013247 alttester_robotframework_library-2.1.0/src/
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:33.018540 alttester_robotframework_library-2.1.0/src/AltTesterLibrary/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)    55503 2024-04-01 07:09:49.000000 alttester_robotframework_library-2.1.0/src/AltTesterLibrary/AltTesterKeywords.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1323 2024-04-01 07:09:49.000000 alttester_robotframework_library-2.1.0/src/AltTesterLibrary/__init__.py
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      718 2024-04-04 09:54:12.000000 alttester_robotframework_library-2.1.0/src/AltTesterLibrary/version.py
+drwxr-xr-x   0 gitlabrunner   (501) staff       (20)        0 2024-04-15 10:33:33.024754 alttester_robotframework_library-2.1.0/src/alttester_robotframework_library.egg-info/
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)     1776 2024-04-15 10:33:32.000000 alttester_robotframework_library-2.1.0/src/alttester_robotframework_library.egg-info/PKG-INFO
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)      483 2024-04-15 10:33:32.000000 alttester_robotframework_library-2.1.0/src/alttester_robotframework_library.egg-info/SOURCES.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2024-04-15 10:33:32.000000 alttester_robotframework_library-2.1.0/src/alttester_robotframework_library.egg-info/dependency_links.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)        1 2024-04-15 10:33:32.000000 alttester_robotframework_library-2.1.0/src/alttester_robotframework_library.egg-info/not-zip-safe
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       37 2024-04-15 10:33:32.000000 alttester_robotframework_library-2.1.0/src/alttester_robotframework_library.egg-info/requires.txt
+-rw-r--r--   0 gitlabrunner   (501) staff       (20)       17 2024-04-15 10:33:32.000000 alttester_robotframework_library-2.1.0/src/alttester_robotframework_library.egg-info/top_level.txt
```

### Comparing `alttester-robotframework-library-0.0.1/PKG-INFO` & `alttester_robotframework_library-2.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alttester-robotframework-library
-Version: 0.0.1
+Version: 2.1.0
 Summary: Robot Framework Library for the AltTester® framework. AltTester® is an open-source UI driven test automation tool that helps you find objects in your game and interacts with them.
 Home-page: https://alttester.com/docs/sdk/latest/
 Author: Altom Consulting
 Author-email: contact@alttester.com
 License: GNU GPLv3
 Project-URL: Issues, https://github.com/alttester/AltTester-Unity-SDK/issues
 Project-URL: Documentation, https://alttester.com/docs/sdk/latest
```

### Comparing `alttester-robotframework-library-0.0.1/setup.py` & `alttester_robotframework_library-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `alttester-robotframework-library-0.0.1/src/AltTesterLibrary/AltTesterKeywords.py` & `alttester_robotframework_library-2.1.0/src/AltTesterLibrary/AltTesterKeywords.py`

 * *Files identical despite different names*

### Comparing `alttester-robotframework-library-0.0.1/src/AltTesterLibrary/__init__.py` & `alttester_robotframework_library-2.1.0/src/AltTesterLibrary/__init__.py`

 * *Files identical despite different names*

### Comparing `alttester-robotframework-library-0.0.1/src/alttester_robotframework_library.egg-info/PKG-INFO` & `alttester_robotframework_library-2.1.0/src/alttester_robotframework_library.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alttester-robotframework-library
-Version: 0.0.1
+Version: 2.1.0
 Summary: Robot Framework Library for the AltTester® framework. AltTester® is an open-source UI driven test automation tool that helps you find objects in your game and interacts with them.
 Home-page: https://alttester.com/docs/sdk/latest/
 Author: Altom Consulting
 Author-email: contact@alttester.com
 License: GNU GPLv3
 Project-URL: Issues, https://github.com/alttester/AltTester-Unity-SDK/issues
 Project-URL: Documentation, https://alttester.com/docs/sdk/latest
```

