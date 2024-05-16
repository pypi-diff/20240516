# Comparing `tmp/pep8-naming-0.9.0.tar.gz` & `tmp/pep8-naming-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pep8-naming-0.9.0.tar", last modified: Wed Nov  6 18:05:07 2019, max compression
+gzip compressed data, was "dist/pep8-naming-0.9.1.tar", last modified: Thu Nov 14 17:59:28 2019, max compression
```

## Comparing `pep8-naming-0.9.0.tar` & `pep8-naming-0.9.1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2019-11-06 18:05:07.000000 pep8-naming-0.9.0/
--rw-r--r--   0 jon        (501) staff       (20)     5215 2019-11-06 18:05:07.000000 pep8-naming-0.9.0/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)     1133 2018-01-02 16:26:01.000000 pep8-naming-0.9.0/LICENSE
--rw-r--r--   0 jon        (501) staff       (20)     3123 2019-07-17 16:28:29.000000 pep8-naming-0.9.0/run_tests.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2019-11-06 18:05:07.000000 pep8-naming-0.9.0/testsuite/
--rw-r--r--   0 jon        (501) staff       (20)      118 2019-01-24 18:23:43.000000 pep8-naming-0.9.0/testsuite/N803_py2.py
--rw-r--r--   0 jon        (501) staff       (20)      203 2019-01-24 18:23:43.000000 pep8-naming-0.9.0/testsuite/N801_py3.py
--rw-r--r--   0 jon        (501) staff       (20)      759 2019-07-17 16:28:29.000000 pep8-naming-0.9.0/testsuite/N804.py
--rw-r--r--   0 jon        (501) staff       (20)      394 2019-01-24 18:23:43.000000 pep8-naming-0.9.0/testsuite/N805_py35.py
--rw-r--r--   0 jon        (501) staff       (20)      743 2019-01-24 18:23:43.000000 pep8-naming-0.9.0/testsuite/N804_py35.py
--rw-r--r--   0 jon        (501) staff       (20)      661 2019-02-05 16:53:45.000000 pep8-naming-0.9.0/testsuite/N801.py
--rw-r--r--   0 jon        (501) staff       (20)      292 2019-02-05 16:53:45.000000 pep8-naming-0.9.0/testsuite/N815.py
--rw-r--r--   0 jon        (501) staff       (20)      437 2019-01-24 18:23:43.000000 pep8-naming-0.9.0/testsuite/N803_py3.py
--rw-r--r--   0 jon        (501) staff       (20)     2295 2019-07-17 16:28:29.000000 pep8-naming-0.9.0/testsuite/N805.py
--rw-r--r--   0 jon        (501) staff       (20)      135 2019-01-24 18:23:43.000000 pep8-naming-0.9.0/testsuite/N806_py35.py
--rw-r--r--   0 jon        (501) staff       (20)      279 2019-02-20 15:48:05.000000 pep8-naming-0.9.0/testsuite/N807_py3.py
--rw-r--r--   0 jon        (501) staff       (20)      213 2019-02-20 15:48:05.000000 pep8-naming-0.9.0/testsuite/N807_py35.py
--rw-r--r--   0 jon        (501) staff       (20)      199 2019-01-24 18:23:43.000000 pep8-naming-0.9.0/testsuite/N802_py35.py
--rw-r--r--   0 jon        (501) staff       (20)      182 2019-01-24 18:23:43.000000 pep8-naming-0.9.0/testsuite/N81x_py3.py
--rw-r--r--   0 jon        (501) staff       (20)      198 2019-01-24 18:23:43.000000 pep8-naming-0.9.0/testsuite/N816_py37.py
--rw-r--r--   0 jon        (501) staff       (20)       81 2019-01-24 18:23:43.000000 pep8-naming-0.9.0/testsuite/N802_py3.py
--rw-r--r--   0 jon        (501) staff       (20)      167 2019-11-04 14:41:34.000000 pep8-naming-0.9.0/testsuite/N805_py38.py
--rw-r--r--   0 jon        (501) staff       (20)      136 2019-01-24 18:23:43.000000 pep8-naming-0.9.0/testsuite/N803_py35.py
--rw-r--r--   0 jon        (501) staff       (20)      573 2019-01-24 18:23:43.000000 pep8-naming-0.9.0/testsuite/N806_py3.py
--rw-r--r--   0 jon        (501) staff       (20)      945 2019-02-05 16:53:45.000000 pep8-naming-0.9.0/testsuite/N802.py
--rw-r--r--   0 jon        (501) staff       (20)      245 2019-02-05 16:53:45.000000 pep8-naming-0.9.0/testsuite/N816.py
--rw-r--r--   0 jon        (501) staff       (20)     2867 2019-02-05 16:53:45.000000 pep8-naming-0.9.0/testsuite/N806.py
--rw-r--r--   0 jon        (501) staff       (20)      360 2019-01-28 19:09:31.000000 pep8-naming-0.9.0/testsuite/N81x.py
--rw-r--r--   0 jon        (501) staff       (20)      830 2019-02-20 15:48:05.000000 pep8-naming-0.9.0/testsuite/N807.py
--rw-r--r--   0 jon        (501) staff       (20)      428 2019-07-16 22:45:19.000000 pep8-naming-0.9.0/testsuite/N806_py2.py
--rw-r--r--   0 jon        (501) staff       (20)      159 2019-01-24 18:23:43.000000 pep8-naming-0.9.0/testsuite/N816_py3.py
--rw-r--r--   0 jon        (501) staff       (20)     1035 2019-07-16 22:45:19.000000 pep8-naming-0.9.0/testsuite/N803.py
--rw-r--r--   0 jon        (501) staff       (20)      103 2018-01-02 16:26:01.000000 pep8-naming-0.9.0/MANIFEST.in
--rw-r--r--   0 jon        (501) staff       (20)     2062 2018-05-07 16:34:04.000000 pep8-naming-0.9.0/setup.py
--rw-r--r--   0 jon        (501) staff       (20)       61 2019-11-06 18:05:07.000000 pep8-naming-0.9.0/setup.cfg
--rw-r--r--   0 jon        (501) staff       (20)     3603 2019-07-16 22:45:19.000000 pep8-naming-0.9.0/README.rst
--rw-r--r--   0 jon        (501) staff       (20)     3855 2019-11-06 18:04:43.000000 pep8-naming-0.9.0/CHANGELOG.rst
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2019-11-06 18:05:07.000000 pep8-naming-0.9.0/src/
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2019-11-06 18:05:07.000000 pep8-naming-0.9.0/src/pep8_naming.egg-info/
--rw-r--r--   0 jon        (501) staff       (20)     5215 2019-11-06 18:05:06.000000 pep8-naming-0.9.0/src/pep8_naming.egg-info/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)        1 2019-01-28 17:06:44.000000 pep8-naming-0.9.0/src/pep8_naming.egg-info/not-zip-safe
--rw-r--r--   0 jon        (501) staff       (20)      934 2019-11-06 18:05:07.000000 pep8-naming-0.9.0/src/pep8_naming.egg-info/SOURCES.txt
--rw-r--r--   0 jon        (501) staff       (20)       54 2019-11-06 18:05:06.000000 pep8-naming-0.9.0/src/pep8_naming.egg-info/entry_points.txt
--rw-r--r--   0 jon        (501) staff       (20)       26 2019-11-06 18:05:06.000000 pep8-naming-0.9.0/src/pep8_naming.egg-info/requires.txt
--rw-r--r--   0 jon        (501) staff       (20)       15 2019-11-06 18:05:06.000000 pep8-naming-0.9.0/src/pep8_naming.egg-info/top_level.txt
--rw-r--r--   0 jon        (501) staff       (20)        1 2019-11-06 18:05:06.000000 pep8-naming-0.9.0/src/pep8_naming.egg-info/dependency_links.txt
--rw-r--r--   0 jon        (501) staff       (20)    17993 2019-11-06 18:04:43.000000 pep8-naming-0.9.0/src/pep8ext_naming.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2019-11-14 17:59:28.000000 pep8-naming-0.9.1/
+-rw-r--r--   0 jon        (501) staff       (20)     5284 2019-11-14 17:59:28.000000 pep8-naming-0.9.1/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)     1133 2018-01-02 16:26:01.000000 pep8-naming-0.9.1/LICENSE
+-rw-r--r--   0 jon        (501) staff       (20)     3123 2019-07-17 16:28:29.000000 pep8-naming-0.9.1/run_tests.py
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2019-11-14 17:59:28.000000 pep8-naming-0.9.1/testsuite/
+-rw-r--r--   0 jon        (501) staff       (20)      118 2019-01-24 18:23:43.000000 pep8-naming-0.9.1/testsuite/N803_py2.py
+-rw-r--r--   0 jon        (501) staff       (20)      203 2019-01-24 18:23:43.000000 pep8-naming-0.9.1/testsuite/N801_py3.py
+-rw-r--r--   0 jon        (501) staff       (20)      759 2019-07-17 16:28:29.000000 pep8-naming-0.9.1/testsuite/N804.py
+-rw-r--r--   0 jon        (501) staff       (20)      394 2019-01-24 18:23:43.000000 pep8-naming-0.9.1/testsuite/N805_py35.py
+-rw-r--r--   0 jon        (501) staff       (20)      743 2019-01-24 18:23:43.000000 pep8-naming-0.9.1/testsuite/N804_py35.py
+-rw-r--r--   0 jon        (501) staff       (20)      661 2019-02-05 16:53:45.000000 pep8-naming-0.9.1/testsuite/N801.py
+-rw-r--r--   0 jon        (501) staff       (20)      292 2019-02-05 16:53:45.000000 pep8-naming-0.9.1/testsuite/N815.py
+-rw-r--r--   0 jon        (501) staff       (20)      437 2019-01-24 18:23:43.000000 pep8-naming-0.9.1/testsuite/N803_py3.py
+-rw-r--r--   0 jon        (501) staff       (20)     2295 2019-07-17 16:28:29.000000 pep8-naming-0.9.1/testsuite/N805.py
+-rw-r--r--   0 jon        (501) staff       (20)      135 2019-01-24 18:23:43.000000 pep8-naming-0.9.1/testsuite/N806_py35.py
+-rw-r--r--   0 jon        (501) staff       (20)      279 2019-02-20 15:48:05.000000 pep8-naming-0.9.1/testsuite/N807_py3.py
+-rw-r--r--   0 jon        (501) staff       (20)      213 2019-02-20 15:48:05.000000 pep8-naming-0.9.1/testsuite/N807_py35.py
+-rw-r--r--   0 jon        (501) staff       (20)      199 2019-01-24 18:23:43.000000 pep8-naming-0.9.1/testsuite/N802_py35.py
+-rw-r--r--   0 jon        (501) staff       (20)      182 2019-01-24 18:23:43.000000 pep8-naming-0.9.1/testsuite/N81x_py3.py
+-rw-r--r--   0 jon        (501) staff       (20)      198 2019-01-24 18:23:43.000000 pep8-naming-0.9.1/testsuite/N816_py37.py
+-rw-r--r--   0 jon        (501) staff       (20)       81 2019-01-24 18:23:43.000000 pep8-naming-0.9.1/testsuite/N802_py3.py
+-rw-r--r--   0 jon        (501) staff       (20)      167 2019-11-04 14:41:34.000000 pep8-naming-0.9.1/testsuite/N805_py38.py
+-rw-r--r--   0 jon        (501) staff       (20)      136 2019-01-24 18:23:43.000000 pep8-naming-0.9.1/testsuite/N803_py35.py
+-rw-r--r--   0 jon        (501) staff       (20)      573 2019-01-24 18:23:43.000000 pep8-naming-0.9.1/testsuite/N806_py3.py
+-rw-r--r--   0 jon        (501) staff       (20)      945 2019-02-05 16:53:45.000000 pep8-naming-0.9.1/testsuite/N802.py
+-rw-r--r--   0 jon        (501) staff       (20)      245 2019-02-05 16:53:45.000000 pep8-naming-0.9.1/testsuite/N816.py
+-rw-r--r--   0 jon        (501) staff       (20)     2867 2019-02-05 16:53:45.000000 pep8-naming-0.9.1/testsuite/N806.py
+-rw-r--r--   0 jon        (501) staff       (20)      360 2019-01-28 19:09:31.000000 pep8-naming-0.9.1/testsuite/N81x.py
+-rw-r--r--   0 jon        (501) staff       (20)      117 2019-11-13 17:58:40.000000 pep8-naming-0.9.1/testsuite/N80x.py
+-rw-r--r--   0 jon        (501) staff       (20)      830 2019-02-20 15:48:05.000000 pep8-naming-0.9.1/testsuite/N807.py
+-rw-r--r--   0 jon        (501) staff       (20)      428 2019-07-16 22:45:19.000000 pep8-naming-0.9.1/testsuite/N806_py2.py
+-rw-r--r--   0 jon        (501) staff       (20)      159 2019-01-24 18:23:43.000000 pep8-naming-0.9.1/testsuite/N816_py3.py
+-rw-r--r--   0 jon        (501) staff       (20)     1035 2019-07-16 22:45:19.000000 pep8-naming-0.9.1/testsuite/N803.py
+-rw-r--r--   0 jon        (501) staff       (20)      103 2018-01-02 16:26:01.000000 pep8-naming-0.9.1/MANIFEST.in
+-rw-r--r--   0 jon        (501) staff       (20)     2062 2018-05-07 16:34:04.000000 pep8-naming-0.9.1/setup.py
+-rw-r--r--   0 jon        (501) staff       (20)       61 2019-11-14 17:59:28.000000 pep8-naming-0.9.1/setup.cfg
+-rw-r--r--   0 jon        (501) staff       (20)     3664 2019-11-14 17:59:02.000000 pep8-naming-0.9.1/README.rst
+-rw-r--r--   0 jon        (501) staff       (20)     4006 2019-11-14 17:59:02.000000 pep8-naming-0.9.1/CHANGELOG.rst
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2019-11-14 17:59:28.000000 pep8-naming-0.9.1/src/
+drwxr-xr-x   0 jon        (501) staff       (20)        0 2019-11-14 17:59:28.000000 pep8-naming-0.9.1/src/pep8_naming.egg-info/
+-rw-r--r--   0 jon        (501) staff       (20)     5284 2019-11-14 17:59:28.000000 pep8-naming-0.9.1/src/pep8_naming.egg-info/PKG-INFO
+-rw-r--r--   0 jon        (501) staff       (20)        1 2019-01-28 17:06:44.000000 pep8-naming-0.9.1/src/pep8_naming.egg-info/not-zip-safe
+-rw-r--r--   0 jon        (501) staff       (20)      952 2019-11-14 17:59:28.000000 pep8-naming-0.9.1/src/pep8_naming.egg-info/SOURCES.txt
+-rw-r--r--   0 jon        (501) staff       (20)       54 2019-11-14 17:59:28.000000 pep8-naming-0.9.1/src/pep8_naming.egg-info/entry_points.txt
+-rw-r--r--   0 jon        (501) staff       (20)       26 2019-11-14 17:59:28.000000 pep8-naming-0.9.1/src/pep8_naming.egg-info/requires.txt
+-rw-r--r--   0 jon        (501) staff       (20)       15 2019-11-14 17:59:28.000000 pep8-naming-0.9.1/src/pep8_naming.egg-info/top_level.txt
+-rw-r--r--   0 jon        (501) staff       (20)        1 2019-11-14 17:59:28.000000 pep8-naming-0.9.1/src/pep8_naming.egg-info/dependency_links.txt
+-rw-r--r--   0 jon        (501) staff       (20)    18073 2019-11-14 17:59:02.000000 pep8-naming-0.9.1/src/pep8ext_naming.py
```

### Comparing `pep8-naming-0.9.0/PKG-INFO` & `pep8-naming-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 1.1
 Name: pep8-naming
-Version: 0.9.0
+Version: 0.9.1
 Summary: Check PEP-8 naming conventions, plugin for flake8
 Home-page: https://github.com/PyCQA/pep8-naming
 Author: Florent Xicluna
 Author-email: florent.xicluna@gmail.com
 License: Expat license
 Description: .. image:: https://travis-ci.org/PyCQA/pep8-naming.svg?branch=master
             :target: https://travis-ci.org/PyCQA/pep8-naming
         
-        PEP-8 Naming Conventions
+        PEP 8 Naming Conventions
         ========================
         
-        Check the PEP-8 naming conventions.
+        Check your code against `PEP 8 <https://www.python.org/dev/peps/pep-0008/>`_
+        naming conventions.
         
         This module provides a plugin for ``flake8``, the Python code checker.
         
         (It replaces the plugin ``flint-naming`` for the ``flint`` checker.)
         
         
         Installation
```

### Comparing `pep8-naming-0.9.0/LICENSE` & `pep8-naming-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pep8-naming-0.9.0/run_tests.py` & `pep8-naming-0.9.1/run_tests.py`

 * *Files identical despite different names*

### Comparing `pep8-naming-0.9.0/testsuite/N804.py` & `pep8-naming-0.9.1/testsuite/N804.py`

 * *Files identical despite different names*

### Comparing `pep8-naming-0.9.0/testsuite/N804_py35.py` & `pep8-naming-0.9.1/testsuite/N804_py35.py`

 * *Files identical despite different names*

### Comparing `pep8-naming-0.9.0/testsuite/N801.py` & `pep8-naming-0.9.1/testsuite/N801.py`

 * *Files identical despite different names*

### Comparing `pep8-naming-0.9.0/testsuite/N805.py` & `pep8-naming-0.9.1/testsuite/N805.py`

 * *Files identical despite different names*

### Comparing `pep8-naming-0.9.0/testsuite/N806_py3.py` & `pep8-naming-0.9.1/testsuite/N806_py3.py`

 * *Files identical despite different names*

### Comparing `pep8-naming-0.9.0/testsuite/N802.py` & `pep8-naming-0.9.1/testsuite/N802.py`

 * *Files identical despite different names*

### Comparing `pep8-naming-0.9.0/testsuite/N806.py` & `pep8-naming-0.9.1/testsuite/N806.py`

 * *Files identical despite different names*

### Comparing `pep8-naming-0.9.0/testsuite/N807.py` & `pep8-naming-0.9.1/testsuite/N807.py`

 * *Files identical despite different names*

### Comparing `pep8-naming-0.9.0/testsuite/N803.py` & `pep8-naming-0.9.1/testsuite/N803.py`

 * *Files identical despite different names*

### Comparing `pep8-naming-0.9.0/setup.py` & `pep8-naming-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `pep8-naming-0.9.0/README.rst` & `pep8-naming-0.9.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .. image:: https://travis-ci.org/PyCQA/pep8-naming.svg?branch=master
     :target: https://travis-ci.org/PyCQA/pep8-naming
 
-PEP-8 Naming Conventions
+PEP 8 Naming Conventions
 ========================
 
-Check the PEP-8 naming conventions.
+Check your code against `PEP 8 <https://www.python.org/dev/peps/pep-0008/>`_
+naming conventions.
 
 This module provides a plugin for ``flake8``, the Python code checker.
 
 (It replaces the plugin ``flint-naming`` for the ``flint`` checker.)
 
 
 Installation
```

### Comparing `pep8-naming-0.9.0/CHANGELOG.rst` & `pep8-naming-0.9.1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changes
 =======
 
+0.9.1 - 2019-11-14
+------------------
+
+* Fix line number offsets when reporting errors involving functions with
+  decorators in Python 3.8 and later.
+
 0.9.0 - 2019-11-06
 ------------------
 
 * Drop support for Python 3.3 and 3.4.
 
 * Support positional-only arguments in Python 3.8.
```

### Comparing `pep8-naming-0.9.0/src/pep8_naming.egg-info/PKG-INFO` & `pep8-naming-0.9.1/src/pep8_naming.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 1.1
 Name: pep8-naming
-Version: 0.9.0
+Version: 0.9.1
 Summary: Check PEP-8 naming conventions, plugin for flake8
 Home-page: https://github.com/PyCQA/pep8-naming
 Author: Florent Xicluna
 Author-email: florent.xicluna@gmail.com
 License: Expat license
 Description: .. image:: https://travis-ci.org/PyCQA/pep8-naming.svg?branch=master
             :target: https://travis-ci.org/PyCQA/pep8-naming
         
-        PEP-8 Naming Conventions
+        PEP 8 Naming Conventions
         ========================
         
-        Check the PEP-8 naming conventions.
+        Check your code against `PEP 8 <https://www.python.org/dev/peps/pep-0008/>`_
+        naming conventions.
         
         This module provides a plugin for ``flake8``, the Python code checker.
         
         (It replaces the plugin ``flint-naming`` for the ``flint`` checker.)
         
         
         Installation
```

### Comparing `pep8-naming-0.9.0/src/pep8_naming.egg-info/SOURCES.txt` & `pep8-naming-0.9.1/src/pep8_naming.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,13 +30,14 @@
 testsuite/N806.py
 testsuite/N806_py2.py
 testsuite/N806_py3.py
 testsuite/N806_py35.py
 testsuite/N807.py
 testsuite/N807_py3.py
 testsuite/N807_py35.py
+testsuite/N80x.py
 testsuite/N815.py
 testsuite/N816.py
 testsuite/N816_py3.py
 testsuite/N816_py37.py
 testsuite/N81x.py
 testsuite/N81x_py3.py
```

### Comparing `pep8-naming-0.9.0/src/pep8ext_naming.py` & `pep8-naming-0.9.1/src/pep8ext_naming.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 try:
     import ast
     from ast import iter_child_nodes
 except ImportError:
     from flake8.util import ast, iter_child_nodes
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 
 PYTHON_VERSION = sys.version_info[:3]
 PY2 = PYTHON_VERSION[0] == 2
 
 METACLASS_BASES = frozenset(('type', 'ABCMeta'))
 
 # Node types which may contain class methods
@@ -61,18 +61,20 @@
         except AttributeError:
             cls._checks = []
 
 
 def _err(self, node, code, **kwargs):
     lineno, col_offset = node.lineno, node.col_offset
     if isinstance(node, ast.ClassDef):
-        lineno += len(node.decorator_list)
+        if PYTHON_VERSION < (3, 8):
+            lineno += len(node.decorator_list)
         col_offset += 6
     elif isinstance(node, FUNC_NODES):
-        lineno += len(node.decorator_list)
+        if PYTHON_VERSION < (3, 8):
+            lineno += len(node.decorator_list)
         col_offset += 4
     code_str = getattr(self, code)
     if kwargs:
         code_str = code_str.format(**kwargs)
     return lineno, col_offset + 1, '%s %s' % (code, code_str), self
```

