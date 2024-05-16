# Comparing `tmp/cpimerge-0.0.6.tar.gz` & `tmp/cpimerge-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpimerge-0.0.6.tar", max compression
+gzip compressed data, was "cpimerge-0.0.7.tar", max compression
```

## Comparing `cpimerge-0.0.6.tar` & `cpimerge-0.0.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1073 2024-05-16 14:41:39.767562 cpimerge-0.0.6/LICENSE
--rw-r--r--   0        0        0      418 2024-05-16 19:04:13.533355 cpimerge-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 14:41:37.832006 cpimerge-0.0.6/src/cpimerge/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 15:31:06.257693 cpimerge-0.0.6/src/cpimerge/__main__.py
--rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 cpimerge-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-16 14:41:39.767562 cpimerge-0.0.7/LICENSE
+-rw-r--r--   0        0        0      422 2024-05-16 19:06:01.897858 cpimerge-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 14:41:37.832006 cpimerge-0.0.7/src/cpimerge/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 15:31:06.257693 cpimerge-0.0.7/src/cpimerge/__main__.py
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 cpimerge-0.0.7/PKG-INFO
```

### Comparing `cpimerge-0.0.6/LICENSE` & `cpimerge-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cpimerge-0.0.6/PKG-INFO` & `cpimerge-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpimerge
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool to merge iCalendar files with exclusions.
 Author: Kirk Coombs
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```
