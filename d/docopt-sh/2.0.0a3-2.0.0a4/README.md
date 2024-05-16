# Comparing `tmp/docopt_sh-2.0.0a3.tar.gz` & `tmp/docopt_sh-2.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docopt_sh-2.0.0a3.tar", max compression
+gzip compressed data, was "docopt_sh-2.0.0a4.tar", max compression
```

## Comparing `docopt_sh-2.0.0a3.tar` & `docopt_sh-2.0.0a4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1059 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/LICENSE
--rw-r--r--   0        0        0      602 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/docopt_sh/__init__.py
--rw-r--r--   0        0        0     3590 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/docopt_sh/__main__.py
--rw-r--r--   0        0        0     4011 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/docopt_sh/bash.py
--rw-r--r--   0        0        0    17767 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/docopt_sh/docopt.sh
--rw-r--r--   0        0        0    10651 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/docopt_sh/parser.py
--rw-r--r--   0        0        0     9063 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/docopt_sh/script.py
--rw-r--r--   0        0        0      221 2024-05-11 07:07:30.870042 docopt_sh-2.0.0a3/docs/README.pypi.md
--rw-r--r--   0        0        0     1218 2024-05-11 07:07:42.586063 docopt_sh-2.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 docopt_sh-2.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/LICENSE
+-rw-r--r--   0        0        0      602 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/docopt_sh/__init__.py
+-rw-r--r--   0        0        0     3590 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/docopt_sh/__main__.py
+-rw-r--r--   0        0        0     4011 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/docopt_sh/bash.py
+-rw-r--r--   0        0        0    17767 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/docopt_sh/docopt.sh
+-rw-r--r--   0        0        0    10651 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/docopt_sh/parser.py
+-rw-r--r--   0        0        0     9063 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/docopt_sh/script.py
+-rw-r--r--   0        0        0      221 2024-05-16 12:24:22.860680 docopt_sh-2.0.0a4/docs/README.pypi.md
+-rw-r--r--   0        0        0     1219 2024-05-16 12:24:36.376777 docopt_sh-2.0.0a4/pyproject.toml
+-rw-r--r--   0        0        0     1100 1970-01-01 00:00:00.000000 docopt_sh-2.0.0a4/PKG-INFO
```

### Comparing `docopt_sh-2.0.0a3/LICENSE` & `docopt_sh-2.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `docopt_sh-2.0.0a3/docopt_sh/__init__.py` & `docopt_sh-2.0.0a4/docopt_sh/__init__.py`

 * *Files identical despite different names*

### Comparing `docopt_sh-2.0.0a3/docopt_sh/__main__.py` & `docopt_sh-2.0.0a4/docopt_sh/__main__.py`

 * *Files identical despite different names*

### Comparing `docopt_sh-2.0.0a3/docopt_sh/bash.py` & `docopt_sh-2.0.0a4/docopt_sh/bash.py`

 * *Files identical despite different names*

### Comparing `docopt_sh-2.0.0a3/docopt_sh/docopt.sh` & `docopt_sh-2.0.0a4/docopt_sh/docopt.sh`

 * *Files identical despite different names*

### Comparing `docopt_sh-2.0.0a3/docopt_sh/parser.py` & `docopt_sh-2.0.0a4/docopt_sh/parser.py`

 * *Files identical despite different names*

### Comparing `docopt_sh-2.0.0a3/docopt_sh/script.py` & `docopt_sh-2.0.0a4/docopt_sh/script.py`

 * *Files identical despite different names*

### Comparing `docopt_sh-2.0.0a3/pyproject.toml` & `docopt_sh-2.0.0a4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "docopt-sh"
 description = "Command-line argument parser for bash 3.2, 4+, and 5+."
-version = "2.0.0-alpha3"
+version = "v2.0.0-alpha4"
 authors = ["Anders Ingemann <anders@ingemann.de>"]
 license = "MIT"
 readme = "docs/README.pypi.md"
 homepage = "https://github.com/andsens/docopt.sh"
 repository = "https://github.com/andsens/docopt.sh"
 classifiers = [
   "Topic :: Utilities",
```

### Comparing `docopt_sh-2.0.0a3/PKG-INFO` & `docopt_sh-2.0.0a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docopt-sh
-Version: 2.0.0a3
+Version: 2.0.0a4
 Summary: Command-line argument parser for bash 3.2, 4+, and 5+.
 Home-page: https://github.com/andsens/docopt.sh
 License: MIT
 Author: Anders Ingemann
 Author-email: anders@ingemann.de
 Requires-Python: >=3.11.0,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

