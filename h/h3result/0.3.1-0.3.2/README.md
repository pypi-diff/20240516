# Comparing `tmp/h3result-0.3.1.tar.gz` & `tmp/h3result-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h3result-0.3.1.tar", max compression
+gzip compressed data, was "h3result-0.3.2.tar", max compression
```

## Comparing `h3result-0.3.1.tar` & `h3result-0.3.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       34 2023-06-15 20:47:23.576073 h3result-0.3.1/README.md
--rw-r--r--   0        0        0     4297 2023-10-31 16:05:55.369509 h3result-0.3.1/build_ext.py
--rw-r--r--   0        0        0        0 2023-06-15 20:47:23.719071 h3result-0.3.1/h3result/__init__.py
--rw-r--r--   0        0        0      242 2023-06-15 21:23:57.265652 h3result-0.3.1/h3result/error.py
--rw-r--r--   0        0        0     1513 2023-06-21 11:21:21.364139 h3result-0.3.1/h3result/h3result.py
--rw-r--r--   0        0        0      970 2023-06-15 21:24:22.759664 h3result-0.3.1/h3result/interface.h
--rw-r--r--   0        0        0       72 2023-06-15 20:47:23.718229 h3result-0.3.1/h3result/path_like.py
--rw-r--r--   0        0        0      645 2023-06-21 11:22:35.090117 h3result-0.3.1/h3result/read_h3result.py
--rw-r--r--   0        0        0      895 2023-10-31 16:02:42.027874 h3result-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      548 1970-01-01 00:00:00.000000 h3result-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       34 2024-05-16 10:01:09.019245 h3result-0.3.2/README.md
+-rw-r--r--   0        0        0     4297 2024-05-16 10:01:09.019245 h3result-0.3.2/build_ext.py
+-rw-r--r--   0        0        0        0 2024-05-16 10:01:09.019245 h3result-0.3.2/h3result/__init__.py
+-rw-r--r--   0        0        0      242 2024-05-16 10:01:09.019245 h3result-0.3.2/h3result/error.py
+-rw-r--r--   0        0        0     1513 2024-05-16 10:01:09.019245 h3result-0.3.2/h3result/h3result.py
+-rw-r--r--   0        0        0      970 2024-05-16 10:01:09.019245 h3result-0.3.2/h3result/interface.h
+-rw-r--r--   0        0        0       72 2024-05-16 10:01:09.019245 h3result-0.3.2/h3result/path_like.py
+-rw-r--r--   0        0        0      645 2024-05-16 10:01:09.019245 h3result-0.3.2/h3result/read_h3result.py
+-rw-r--r--   0        0        0      898 2024-05-16 10:01:09.019245 h3result-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 h3result-0.3.2/PKG-INFO
```

### Comparing `h3result-0.3.1/build_ext.py` & `h3result-0.3.2/build_ext.py`

 * *Files identical despite different names*

### Comparing `h3result-0.3.1/h3result/h3result.py` & `h3result-0.3.2/h3result/h3result.py`

 * *Files identical despite different names*

### Comparing `h3result-0.3.1/h3result/interface.h` & `h3result-0.3.2/h3result/interface.h`

 * *Files identical despite different names*

### Comparing `h3result-0.3.1/h3result/read_h3result.py` & `h3result-0.3.2/h3result/read_h3result.py`

 * *Files identical despite different names*

