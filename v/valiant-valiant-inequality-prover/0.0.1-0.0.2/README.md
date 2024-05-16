# Comparing `tmp/valiant_valiant_inequality_prover-0.0.1.tar.gz` & `tmp/valiant_valiant_inequality_prover-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valiant_valiant_inequality_prover-0.0.1.tar", last modified: Mon May 13 02:34:12 2024, max compression
+gzip compressed data, was "valiant_valiant_inequality_prover-0.0.2.tar", last modified: Thu May 16 13:19:11 2024, max compression
```

## Comparing `valiant_valiant_inequality_prover-0.0.1.tar` & `valiant_valiant_inequality_prover-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 02:34:12.124905 valiant_valiant_inequality_prover-0.0.1/
--rw-rw-rw-   0        0        0     1089 2024-05-12 11:28:41.000000 valiant_valiant_inequality_prover-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      900 2024-05-13 02:34:12.120577 valiant_valiant_inequality_prover-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      124 2024-05-13 02:08:29.000000 valiant_valiant_inequality_prover-0.0.1/README.md
--rw-rw-rw-   0        0        0      755 2024-05-13 02:06:17.000000 valiant_valiant_inequality_prover-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 02:34:12.124905 valiant_valiant_inequality_prover-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      523 2024-05-13 02:34:03.000000 valiant_valiant_inequality_prover-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 02:34:12.070777 valiant_valiant_inequality_prover-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 02:34:12.093310 valiant_valiant_inequality_prover-0.0.1/src/valiant_valiant_inequality_prover/
--rw-rw-rw-   0        0        0        0 2024-05-13 02:01:56.000000 valiant_valiant_inequality_prover-0.0.1/src/valiant_valiant_inequality_prover/__init__.py
--rw-rw-rw-   0        0        0    13558 2024-05-13 02:01:56.000000 valiant_valiant_inequality_prover-0.0.1/src/valiant_valiant_inequality_prover/valiant_valiant_inequality_prover.py
-drwxrwxrwx   0        0        0        0 2024-05-13 02:34:12.117546 valiant_valiant_inequality_prover-0.0.1/valiant_valiant_inequality_prover.egg-info/
--rw-rw-rw-   0        0        0      900 2024-05-13 02:34:12.000000 valiant_valiant_inequality_prover-0.0.1/valiant_valiant_inequality_prover.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-05-13 02:34:12.000000 valiant_valiant_inequality_prover-0.0.1/valiant_valiant_inequality_prover.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 02:34:12.000000 valiant_valiant_inequality_prover-0.0.1/valiant_valiant_inequality_prover.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-13 02:34:12.000000 valiant_valiant_inequality_prover-0.0.1/valiant_valiant_inequality_prover.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 13:19:11.768226 valiant_valiant_inequality_prover-0.0.2/
+-rw-rw-rw-   0        0        0     1089 2024-05-12 11:28:41.000000 valiant_valiant_inequality_prover-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      900 2024-05-16 13:19:11.763062 valiant_valiant_inequality_prover-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2024-05-13 02:08:29.000000 valiant_valiant_inequality_prover-0.0.2/README.md
+-rw-rw-rw-   0        0        0      755 2024-05-16 13:17:34.000000 valiant_valiant_inequality_prover-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 13:19:11.769328 valiant_valiant_inequality_prover-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      422 2024-05-16 13:17:47.000000 valiant_valiant_inequality_prover-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:19:11.694799 valiant_valiant_inequality_prover-0.0.2/valiant_valiant_inequality_prover/
+-rw-rw-rw-   0        0        0        0 2024-05-13 02:01:56.000000 valiant_valiant_inequality_prover-0.0.2/valiant_valiant_inequality_prover/__init__.py
+-rw-rw-rw-   0        0        0    13558 2024-05-13 02:01:56.000000 valiant_valiant_inequality_prover-0.0.2/valiant_valiant_inequality_prover/valiant_valiant_inequality_prover.py
+drwxrwxrwx   0        0        0        0 2024-05-16 13:19:11.758804 valiant_valiant_inequality_prover-0.0.2/valiant_valiant_inequality_prover.egg-info/
+-rw-rw-rw-   0        0        0      900 2024-05-16 13:19:11.000000 valiant_valiant_inequality_prover-0.0.2/valiant_valiant_inequality_prover.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2024-05-16 13:19:11.000000 valiant_valiant_inequality_prover-0.0.2/valiant_valiant_inequality_prover.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 13:19:11.000000 valiant_valiant_inequality_prover-0.0.2/valiant_valiant_inequality_prover.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-16 13:19:11.000000 valiant_valiant_inequality_prover-0.0.2/valiant_valiant_inequality_prover.egg-info/top_level.txt
```

### Comparing `valiant_valiant_inequality_prover-0.0.1/LICENSE` & `valiant_valiant_inequality_prover-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `valiant_valiant_inequality_prover-0.0.1/PKG-INFO` & `valiant_valiant_inequality_prover-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valiant_valiant_inequality_prover
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python implementation of the automatic inequality prover proposed by Valiant & Valiant (https://doi.org/10.1137/151002526)
 Home-page: http://packages.python.org/valiant_valiant_inequality_prover
 Author: Richard Riis
 Author-email: Richard Riis <richardpriis@gmail.com>
 Project-URL: Homepage, https://github.com/rpriis/valiant_valiant_inequality_prover
 Project-URL: Issues, https://github.com/rpriis/valiant_valiant_inequality_prover/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `valiant_valiant_inequality_prover-0.0.1/pyproject.toml` & `valiant_valiant_inequality_prover-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "valiant_valiant_inequality_prover"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Richard Riis", email="richardpriis@gmail.com" },
 ]
 description = "Python implementation of the automatic inequality prover proposed by Valiant & Valiant (https://doi.org/10.1137/151002526)"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
```

### Comparing `valiant_valiant_inequality_prover-0.0.1/src/valiant_valiant_inequality_prover/valiant_valiant_inequality_prover.py` & `valiant_valiant_inequality_prover-0.0.2/valiant_valiant_inequality_prover/valiant_valiant_inequality_prover.py`

 * *Files identical despite different names*

### Comparing `valiant_valiant_inequality_prover-0.0.1/valiant_valiant_inequality_prover.egg-info/PKG-INFO` & `valiant_valiant_inequality_prover-0.0.2/valiant_valiant_inequality_prover.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valiant_valiant_inequality_prover
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python implementation of the automatic inequality prover proposed by Valiant & Valiant (https://doi.org/10.1137/151002526)
 Home-page: http://packages.python.org/valiant_valiant_inequality_prover
 Author: Richard Riis
 Author-email: Richard Riis <richardpriis@gmail.com>
 Project-URL: Homepage, https://github.com/rpriis/valiant_valiant_inequality_prover
 Project-URL: Issues, https://github.com/rpriis/valiant_valiant_inequality_prover/issues
 Classifier: Programming Language :: Python :: 3
```

