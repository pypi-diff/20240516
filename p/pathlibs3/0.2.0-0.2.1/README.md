# Comparing `tmp/pathlibs3-0.2.0.tar.gz` & `tmp/pathlibs3-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathlibs3-0.2.0.tar", max compression
+gzip compressed data, was "pathlibs3-0.2.1.tar", max compression
```

## Comparing `pathlibs3-0.2.0.tar` & `pathlibs3-0.2.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.0/pathlibs3/__init__.py
--rw-r--r--   0        0        0     3305 2024-05-16 12:51:23.982420 pathlibs3-0.2.0/pathlibs3/pathlibs3.py
--rw-r--r--   0        0        0      389 2024-05-16 13:06:15.026499 pathlibs3-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      435 1970-01-01 00:00:00.000000 pathlibs3-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.2.1/pathlibs3/__init__.py
+-rw-r--r--   0        0        0     3305 2024-05-16 12:51:23.982420 pathlibs3-0.2.1/pathlibs3/pathlibs3.py
+-rw-r--r--   0        0        0      382 2024-05-16 13:10:26.086521 pathlibs3-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 pathlibs3-0.2.1/PKG-INFO
```

### Comparing `pathlibs3-0.2.0/pathlibs3/pathlibs3.py` & `pathlibs3-0.2.1/pathlibs3/pathlibs3.py`

 * *Files identical despite different names*

