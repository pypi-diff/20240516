# Comparing `tmp/python_filewrap-0.0.2.1.tar.gz` & `tmp/python_filewrap-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_filewrap-0.0.2.1.tar", max compression
+gzip compressed data, was "python_filewrap-0.0.3.tar", max compression
```

## Comparing `python_filewrap-0.0.2.1.tar` & `python_filewrap-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.2.1/LICENSE
--rwxr-xr-x   0        0        0     7948 2024-05-16 12:31:35.118526 python_filewrap-0.0.2.1/filewrap/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.2.1/filewrap/py.typed
--rw-r--r--   0        0        0     1149 2024-05-16 12:31:49.311113 python_filewrap-0.0.2.1/pyproject.toml
--rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.2.1/readme.md
--rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 python_filewrap-0.0.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.3/LICENSE
+-rwxr-xr-x   0        0        0     9765 2024-05-16 15:59:19.428444 python_filewrap-0.0.3/filewrap/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.3/filewrap/py.typed
+-rw-r--r--   0        0        0     1147 2024-05-16 15:59:32.162427 python_filewrap-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.3/readme.md
+-rw-r--r--   0        0        0     1329 1970-01-01 00:00:00.000000 python_filewrap-0.0.3/PKG-INFO
```

### Comparing `python_filewrap-0.0.2.1/LICENSE` & `python_filewrap-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_filewrap-0.0.2.1/pyproject.toml` & `python_filewrap-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-filewrap"
-version = "0.0.2.1"
+version = "0.0.3"
 description = "Python file wrappers."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 keywords = ["file", "wrapper"]
```

### Comparing `python_filewrap-0.0.2.1/PKG-INFO` & `python_filewrap-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-filewrap
-Version: 0.0.2.1
+Version: 0.0.3
 Summary: Python file wrappers.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap
 License: MIT
 Keywords: file,wrapper
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

