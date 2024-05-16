# Comparing `tmp/gedhtml-0.0.1.tar.gz` & `tmp/gedhtml-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gedhtml-0.0.1.tar", max compression
+gzip compressed data, was "gedhtml-0.0.2.tar", max compression
```

## Comparing `gedhtml-0.0.1.tar` & `gedhtml-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2024-05-15 20:30:56.134940 gedhtml-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/__init__.py
--rw-r--r--   0        0        0      977 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/__main__.py
--rw-r--r--   0        0        0     3017 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/describe.py
--rw-r--r--   0        0        0     5089 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/family_tree.py
--rw-r--r--   0        0        0     2537 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/file.py
--rw-r--r--   0        0        0     1826 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/html_template.py
--rw-r--r--   0        0        0     3163 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/language.py
--rw-r--r--   0        0        0     3277 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/pedigree.py
--rw-r--r--   0        0        0      146 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/utils.py
--rw-r--r--   0        0        0    10100 2024-05-15 20:30:56.134940 gedhtml-0.0.1/gedhtml/webpage.py
--rw-r--r--   0        0        0      618 2024-05-15 20:31:05.282926 gedhtml-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 gedhtml-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-05-16 06:55:14.475798 gedhtml-0.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-16 06:55:14.475798 gedhtml-0.0.2/gedhtml/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-16 06:55:14.475798 gedhtml-0.0.2/gedhtml/__main__.py
+-rw-r--r--   0        0        0     3017 2024-05-16 06:55:14.475798 gedhtml-0.0.2/gedhtml/describe.py
+-rw-r--r--   0        0        0     5089 2024-05-16 06:55:14.475798 gedhtml-0.0.2/gedhtml/family_tree.py
+-rw-r--r--   0        0        0     2537 2024-05-16 06:55:14.475798 gedhtml-0.0.2/gedhtml/file.py
+-rw-r--r--   0        0        0     1826 2024-05-16 06:55:14.475798 gedhtml-0.0.2/gedhtml/html_template.py
+-rw-r--r--   0        0        0     3163 2024-05-16 06:55:14.475798 gedhtml-0.0.2/gedhtml/language.py
+-rw-r--r--   0        0        0     3277 2024-05-16 06:55:14.475798 gedhtml-0.0.2/gedhtml/pedigree.py
+-rw-r--r--   0        0        0      146 2024-05-16 06:55:14.475798 gedhtml-0.0.2/gedhtml/utils.py
+-rw-r--r--   0        0        0    10100 2024-05-16 06:55:14.475798 gedhtml-0.0.2/gedhtml/webpage.py
+-rw-r--r--   0        0        0      618 2024-05-16 06:55:24.091782 gedhtml-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      553 1970-01-01 00:00:00.000000 gedhtml-0.0.2/PKG-INFO
```

### Comparing `gedhtml-0.0.1/LICENSE` & `gedhtml-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gedhtml-0.0.1/gedhtml/__main__.py` & `gedhtml-0.0.2/gedhtml/__main__.py`

 * *Files identical despite different names*

### Comparing `gedhtml-0.0.1/gedhtml/describe.py` & `gedhtml-0.0.2/gedhtml/describe.py`

 * *Files identical despite different names*

### Comparing `gedhtml-0.0.1/gedhtml/family_tree.py` & `gedhtml-0.0.2/gedhtml/family_tree.py`

 * *Files identical despite different names*

### Comparing `gedhtml-0.0.1/gedhtml/file.py` & `gedhtml-0.0.2/gedhtml/file.py`

 * *Files identical despite different names*

### Comparing `gedhtml-0.0.1/gedhtml/html_template.py` & `gedhtml-0.0.2/gedhtml/html_template.py`

 * *Files identical despite different names*

### Comparing `gedhtml-0.0.1/gedhtml/language.py` & `gedhtml-0.0.2/gedhtml/language.py`

 * *Files identical despite different names*

### Comparing `gedhtml-0.0.1/gedhtml/pedigree.py` & `gedhtml-0.0.2/gedhtml/pedigree.py`

 * *Files identical despite different names*

### Comparing `gedhtml-0.0.1/gedhtml/webpage.py` & `gedhtml-0.0.2/gedhtml/webpage.py`

 * *Files identical despite different names*

### Comparing `gedhtml-0.0.1/pyproject.toml` & `gedhtml-0.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gedhtml"
-version = "v0.0.1"
+version = "v0.0.2"
 description = "Converting GED files to static web pages."
 authors = ["Edo van Veen <edo@vanveen.io>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 matplotlib = "^3.8.4"
 yattag = "^1.15.2"
```

### Comparing `gedhtml-0.0.1/PKG-INFO` & `gedhtml-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gedhtml
-Version: 0.0.1
+Version: 0.0.2
 Summary: Converting GED files to static web pages.
 Author: Edo van Veen
 Author-email: edo@vanveen.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

