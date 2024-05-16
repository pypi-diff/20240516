# Comparing `tmp/clodo_py_tools-0.0.0.tar.gz` & `tmp/clodo_py_tools-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clodo_py_tools-0.0.0.tar", last modified: Tue Feb 27 04:31:58 2024, max compression
+gzip compressed data, was "clodo_py_tools-0.0.1.tar", last modified: Thu May 16 21:19:42 2024, max compression
```

## Comparing `clodo_py_tools-0.0.0.tar` & `clodo_py_tools-0.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-02-27 04:31:58.734354 clodo_py_tools-0.0.0/
--rw-rw-rw-   0        0        0      681 2024-02-27 04:31:58.734354 clodo_py_tools-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-02-26 21:23:49.000000 clodo_py_tools-0.0.0/README.md
--rw-rw-rw-   0        0        0      946 2024-02-27 04:30:59.000000 clodo_py_tools-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-27 04:31:58.735945 clodo_py_tools-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-02-26 19:34:56.000000 clodo_py_tools-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-27 04:31:58.727766 clodo_py_tools-0.0.0/src/
--rw-rw-rw-   0        0        0        0 2024-02-27 01:38:48.000000 clodo_py_tools-0.0.0/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-27 04:31:58.734354 clodo_py_tools-0.0.0/src/clodo_py_tools.egg-info/
--rw-rw-rw-   0        0        0      681 2024-02-27 04:31:58.000000 clodo_py_tools-0.0.0/src/clodo_py_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      362 2024-02-27 04:31:58.000000 clodo_py_tools-0.0.0/src/clodo_py_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-27 04:31:58.000000 clodo_py_tools-0.0.0/src/clodo_py_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-02-27 04:31:58.000000 clodo_py_tools-0.0.0/src/clodo_py_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       18 2024-02-27 04:31:58.000000 clodo_py_tools-0.0.0/src/clodo_py_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       44 2024-02-27 04:31:58.000000 clodo_py_tools-0.0.0/src/clodo_py_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      102 2024-02-27 03:44:07.000000 clodo_py_tools-0.0.0/src/execute_module.py
--rw-rw-rw-   0        0        0     3820 2024-02-27 03:28:13.000000 clodo_py_tools-0.0.0/src/performance_tracing.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:19:42.823211 clodo_py_tools-0.0.1/
+-rw-rw-rw-   0        0        0      681 2024-05-16 21:19:42.823211 clodo_py_tools-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       38 2024-03-11 04:48:34.000000 clodo_py_tools-0.0.1/README.md
+-rw-rw-rw-   0        0        0      947 2024-05-16 21:19:21.000000 clodo_py_tools-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 21:19:42.823211 clodo_py_tools-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-02-26 19:34:56.000000 clodo_py_tools-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:19:42.823211 clodo_py_tools-0.0.1/src/
+-rw-rw-rw-   0        0        0        0 2024-02-27 01:38:48.000000 clodo_py_tools-0.0.1/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 21:19:42.823211 clodo_py_tools-0.0.1/src/clodo_py_tools.egg-info/
+-rw-rw-rw-   0        0        0      681 2024-05-16 21:19:42.000000 clodo_py_tools-0.0.1/src/clodo_py_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2024-05-16 21:19:42.000000 clodo_py_tools-0.0.1/src/clodo_py_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 21:19:42.000000 clodo_py_tools-0.0.1/src/clodo_py_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-05-16 21:19:42.000000 clodo_py_tools-0.0.1/src/clodo_py_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       18 2024-05-16 21:19:42.000000 clodo_py_tools-0.0.1/src/clodo_py_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2024-05-16 21:19:42.000000 clodo_py_tools-0.0.1/src/clodo_py_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3918 2024-05-16 19:41:21.000000 clodo_py_tools-0.0.1/src/performance_tracing.py
+-rw-rw-rw-   0        0        0     1068 2024-05-16 20:28:20.000000 clodo_py_tools-0.0.1/src/timer.py
```

### Comparing `clodo_py_tools-0.0.0/PKG-INFO` & `clodo_py_tools-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clodo_py_tools
-Version: 0.0.0
+Version: 0.0.1
 Author-email: Clodomir Vianna <clodolinus@gmail.com>
 Project-URL: Homepage, https://example.com
 Project-URL: Documentation, https://readthedocs.org
 Project-URL: Repository, https://github.com/me/spam.git
 Project-URL: Issues, https://github.com/me/spam/issues
 Project-URL: Changelog, https://github.com/me/spam/blob/master/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clodo_py_tools-0.0.0/pyproject.toml` & `clodo_py_tools-0.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
 readme = {file = ["README.md"]}
 
 [project]
 name = "clodo_py_tools"
-version = "0.0.0"
+version = "0.0.1"
 description = ""
 authors = [
     {name = "Clodomir Vianna", email = "clodolinus@gmail.com"},
 ]
 readme = "README.rst"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -29,8 +29,8 @@
 Documentation = "https://readthedocs.org"
 Repository = "https://github.com/me/spam.git"
 Issues = "https://github.com/me/spam/issues"
 Changelog = "https://github.com/me/spam/blob/master/CHANGELOG.md"
 
 # Creation of terminal commands:
 [project.scripts]
-performance_tracing = "execute_module:performance_tracing"
+trace_performance = "performance_tracing:trace_performance"
```

### Comparing `clodo_py_tools-0.0.0/src/clodo_py_tools.egg-info/PKG-INFO` & `clodo_py_tools-0.0.1/src/clodo_py_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clodo_py_tools
-Version: 0.0.0
+Version: 0.0.1
 Author-email: Clodomir Vianna <clodolinus@gmail.com>
 Project-URL: Homepage, https://example.com
 Project-URL: Documentation, https://readthedocs.org
 Project-URL: Repository, https://github.com/me/spam.git
 Project-URL: Issues, https://github.com/me/spam/issues
 Project-URL: Changelog, https://github.com/me/spam/blob/master/CHANGELOG.md
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clodo_py_tools-0.0.0/src/performance_tracing.py` & `clodo_py_tools-0.0.1/src/performance_tracing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+def trace_performance():
+    import importlib
+    importlib.import_module("performance_tracing")
+
 import psutil
 import matplotlib.pyplot as plt
 from datetime import datetime
 import matplotlib.animation as animation
 import threading
 import queue
 import sys
```

