# Comparing `tmp/flake8_commas-4.0.0.tar.gz` & `tmp/flake8_commas-4.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_commas-4.0.0.tar", last modified: Thu May 16 19:52:49 2024, max compression
+gzip compressed data, was "flake8_commas-4.0.0.dev0.tar", last modified: Sun May  5 16:51:25 2024, max compression
```

## Comparing `flake8_commas-4.0.0.tar` & `flake8_commas-4.0.0.dev0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:52:49.391101 flake8_commas-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4465 2024-05-16 19:52:34.000000 flake8_commas-4.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-16 19:52:34.000000 flake8_commas-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-16 19:52:34.000000 flake8_commas-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-05-16 19:52:49.391101 flake8_commas-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-16 19:52:34.000000 flake8_commas-4.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:52:49.387100 flake8_commas-4.0.0/flake8_commas/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-16 19:52:34.000000 flake8_commas-4.0.0/flake8_commas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-05-16 19:52:34.000000 flake8_commas-4.0.0/flake8_commas/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:52:49.391101 flake8_commas-4.0.0/flake8_commas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-05-16 19:52:49.000000 flake8_commas-4.0.0/flake8_commas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-16 19:52:49.000000 flake8_commas-4.0.0/flake8_commas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:52:49.000000 flake8_commas-4.0.0/flake8_commas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 19:52:49.000000 flake8_commas-4.0.0/flake8_commas.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 19:52:49.000000 flake8_commas-4.0.0/flake8_commas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 19:52:49.000000 flake8_commas-4.0.0/flake8_commas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:52:49.391101 flake8_commas-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-16 19:52:34.000000 flake8_commas-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:52:49.391101 flake8_commas-4.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-05-16 19:52:34.000000 flake8_commas-4.0.0/test/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-16 19:52:34.000000 flake8_commas-4.0.0/test/test_flake8.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:51:25.185836 flake8_commas-4.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-05 16:51:15.000000 flake8_commas-4.0.0.dev0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-05 16:51:15.000000 flake8_commas-4.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-05 16:51:15.000000 flake8_commas-4.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-05-05 16:51:25.185836 flake8_commas-4.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-05 16:51:15.000000 flake8_commas-4.0.0.dev0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:51:25.185836 flake8_commas-4.0.0.dev0/flake8_commas/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-05 16:51:15.000000 flake8_commas-4.0.0.dev0/flake8_commas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10027 2024-05-05 16:51:15.000000 flake8_commas-4.0.0.dev0/flake8_commas/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:51:25.185836 flake8_commas-4.0.0.dev0/flake8_commas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-05-05 16:51:25.000000 flake8_commas-4.0.0.dev0/flake8_commas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-05 16:51:25.000000 flake8_commas-4.0.0.dev0/flake8_commas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 16:51:25.000000 flake8_commas-4.0.0.dev0/flake8_commas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-05 16:51:25.000000 flake8_commas-4.0.0.dev0/flake8_commas.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-05 16:51:25.000000 flake8_commas-4.0.0.dev0/flake8_commas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-05 16:51:25.000000 flake8_commas-4.0.0.dev0/flake8_commas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 16:51:25.185836 flake8_commas-4.0.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-05 16:51:15.000000 flake8_commas-4.0.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 16:51:25.185836 flake8_commas-4.0.0.dev0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-05-05 16:51:15.000000 flake8_commas-4.0.0.dev0/test/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-05 16:51:15.000000 flake8_commas-4.0.0.dev0/test/test_flake8.py
```

### Comparing `flake8_commas-4.0.0/CHANGES.rst` & `flake8_commas-4.0.0.dev0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
-4.0.0 (2024-05-16)
+4.0.0
 ------------------
 
-- Project renamed back to ``flake8-commas``. If upgrading from
-  ``flake8-commas-x`` you should uninstall that package before
-  installing this one as both packages install the same modules.
+- Project renamed back to ``flake8-commas``
 
 3.0.0 (2024-03-12)
 ------------------
 
 - Project renamed to ``flake8-commas-x`` to continue maintenance.
 - Support dropped for Python <3.8.
 - Support added for Python 3.12.
```

### Comparing `flake8_commas-4.0.0/LICENSE` & `flake8_commas-4.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_commas-4.0.0/PKG-INFO` & `flake8_commas-4.0.0.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-commas
-Version: 4.0.0
+Version: 4.0.0.dev0
 Summary: Flake8 lint for trailing commas.
 Home-page: https://github.com/PyCQA/flake8-commas/
 Author: Trevor Creech
 Author-email: trevor@trevorcreech.com
 Maintainer: Peter Law
 Maintainer-email: PeterJCLaw@gmail.com
 Classifier: Environment :: Console
@@ -94,20 +94,18 @@
 .. |Build Status| image:: https://github.com/PyCQA/flake8-commas/actions/workflows/.github/workflows/tests.yml/badge.svg?branch=main
    :target: https://github.com/PyCQA/flake8-commas/actions?query=branch%3Amain
 
 .. |PyPI - Version| image:: https://img.shields.io/pypi/v/flake8-commas
    :target: https://pypi.org/project/flake8-commas/
 
 
-4.0.0 (2024-05-16)
+4.0.0
 ------------------
 
-- Project renamed back to ``flake8-commas``. If upgrading from
-  ``flake8-commas-x`` you should uninstall that package before
-  installing this one as both packages install the same modules.
+- Project renamed back to ``flake8-commas``
 
 3.0.0 (2024-03-12)
 ------------------
 
 - Project renamed to ``flake8-commas-x`` to continue maintenance.
 - Support dropped for Python <3.8.
 - Support added for Python 3.12.
```

### Comparing `flake8_commas-4.0.0/README.rst` & `flake8_commas-4.0.0.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `flake8_commas-4.0.0/flake8_commas/_base.py` & `flake8_commas-4.0.0.dev0/flake8_commas/_base.py`

 * *Files identical despite different names*

### Comparing `flake8_commas-4.0.0/flake8_commas.egg-info/PKG-INFO` & `flake8_commas-4.0.0.dev0/flake8_commas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-commas
-Version: 4.0.0
+Version: 4.0.0.dev0
 Summary: Flake8 lint for trailing commas.
 Home-page: https://github.com/PyCQA/flake8-commas/
 Author: Trevor Creech
 Author-email: trevor@trevorcreech.com
 Maintainer: Peter Law
 Maintainer-email: PeterJCLaw@gmail.com
 Classifier: Environment :: Console
@@ -94,20 +94,18 @@
 .. |Build Status| image:: https://github.com/PyCQA/flake8-commas/actions/workflows/.github/workflows/tests.yml/badge.svg?branch=main
    :target: https://github.com/PyCQA/flake8-commas/actions?query=branch%3Amain
 
 .. |PyPI - Version| image:: https://img.shields.io/pypi/v/flake8-commas
    :target: https://pypi.org/project/flake8-commas/
 
 
-4.0.0 (2024-05-16)
+4.0.0
 ------------------
 
-- Project renamed back to ``flake8-commas``. If upgrading from
-  ``flake8-commas-x`` you should uninstall that package before
-  installing this one as both packages install the same modules.
+- Project renamed back to ``flake8-commas``
 
 3.0.0 (2024-03-12)
 ------------------
 
 - Project renamed to ``flake8-commas-x`` to continue maintenance.
 - Support dropped for Python <3.8.
 - Support added for Python 3.12.
```

### Comparing `flake8_commas-4.0.0/setup.py` & `flake8_commas-4.0.0.dev0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 setup(
     name='flake8-commas',
     author="Trevor Creech",
     author_email="trevor@trevorcreech.com",
     maintainer="Peter Law",
     maintainer_email="PeterJCLaw@gmail.com",
-    version='4.0.0',
+    version='4.0.0.dev0',
     install_requires=['flake8>=5'],
     python_requires='>=3.8',
     url='https://github.com/PyCQA/flake8-commas/',
     long_description=readme + '\n\n' + history,
     long_description_content_type='text/x-rst',
     description='Flake8 lint for trailing commas.',
     packages=['flake8_commas'],
```

### Comparing `flake8_commas-4.0.0/test/test_checks.py` & `flake8_commas-4.0.0.dev0/test/test_checks.py`

 * *Files identical despite different names*

