# Comparing `tmp/pathlibs3-0.1.2.tar.gz` & `tmp/pathlibs3-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pathlibs3-0.1.2.tar", max compression
+gzip compressed data, was "pathlibs3-0.1.3.tar", max compression
```

## Comparing `pathlibs3-0.1.2.tar` & `pathlibs3-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.1.2/pathlibs3/__init__.py
--rw-r--r--   0        0        0     3305 2024-05-16 12:51:23.982420 pathlibs3-0.1.2/pathlibs3/pathlibs3.py
--rw-r--r--   0        0        0      389 2024-05-16 13:02:11.886477 pathlibs3-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      435 1970-01-01 00:00:00.000000 pathlibs3-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-05-16 12:51:23.982420 pathlibs3-0.1.3/pathlibs3/__init__.py
+-rw-r--r--   0        0        0     3305 2024-05-16 12:51:23.982420 pathlibs3-0.1.3/pathlibs3/pathlibs3.py
+-rw-r--r--   0        0        0      389 2024-05-16 13:03:15.573420 pathlibs3-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      435 1970-01-01 00:00:00.000000 pathlibs3-0.1.3/PKG-INFO
```

### Comparing `pathlibs3-0.1.2/pathlibs3/pathlibs3.py` & `pathlibs3-0.1.3/pathlibs3/pathlibs3.py`

 * *Files identical despite different names*

