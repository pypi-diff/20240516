# Comparing `tmp/dataclasses_struct-0.8.1.tar.gz` & `tmp/dataclasses_struct-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclasses_struct-0.8.1.tar", max compression
+gzip compressed data, was "dataclasses_struct-0.8.2.tar", max compression
```

## Comparing `dataclasses_struct-0.8.1.tar` & `dataclasses_struct-0.8.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1079 2023-07-25 23:44:26.259255 dataclasses_struct-0.8.1/LICENSE
--rw-r--r--   0        0        0     6346 2023-08-07 01:02:05.413876 dataclasses_struct-0.8.1/README.md
--rw-r--r--   0        0        0     1425 2023-08-07 00:46:51.784399 dataclasses_struct-0.8.1/dataclasses_struct/__init__.py
--rw-r--r--   0        0        0     9432 2024-03-17 21:14:31.077959 dataclasses_struct-0.8.1/dataclasses_struct/dataclass.py
--rw-r--r--   0        0        0        0 2023-07-25 23:44:26.259255 dataclasses_struct-0.8.1/dataclasses_struct/ext/__init__.py
--rw-r--r--   0        0        0     1856 2023-08-07 00:46:51.784399 dataclasses_struct-0.8.1/dataclasses_struct/ext/mypy_plugin.py
--rw-r--r--   0        0        0     4429 2023-08-25 03:10:46.115543 dataclasses_struct-0.8.1/dataclasses_struct/field.py
--rw-r--r--   0        0        0      313 2023-07-27 22:18:30.718550 dataclasses_struct-0.8.1/dataclasses_struct/intsizes.py
--rw-r--r--   0        0        0        0 2023-07-25 23:44:26.259255 dataclasses_struct-0.8.1/dataclasses_struct/py.typed
--rw-r--r--   0        0        0     1340 2023-08-03 02:47:39.912029 dataclasses_struct-0.8.1/dataclasses_struct/types.py
--rw-r--r--   0        0        0     2078 2024-03-17 21:28:24.530520 dataclasses_struct-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     7846 1970-01-01 00:00:00.000000 dataclasses_struct-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-25 23:44:26.259255 dataclasses_struct-0.8.2/LICENSE
+-rw-r--r--   0        0        0     6346 2024-03-26 19:27:44.477487 dataclasses_struct-0.8.2/README.md
+-rw-r--r--   0        0        0     1425 2024-05-16 08:02:14.107463 dataclasses_struct-0.8.2/dataclasses_struct/__init__.py
+-rw-r--r--   0        0        0     9432 2024-05-16 08:02:14.107463 dataclasses_struct-0.8.2/dataclasses_struct/dataclass.py
+-rw-r--r--   0        0        0        0 2023-07-25 23:44:26.259255 dataclasses_struct-0.8.2/dataclasses_struct/ext/__init__.py
+-rw-r--r--   0        0        0     1856 2023-08-07 00:46:51.784399 dataclasses_struct-0.8.2/dataclasses_struct/ext/mypy_plugin.py
+-rw-r--r--   0        0        0     4429 2024-05-16 08:02:14.107463 dataclasses_struct-0.8.2/dataclasses_struct/field.py
+-rw-r--r--   0        0        0      313 2024-05-16 08:02:14.107463 dataclasses_struct-0.8.2/dataclasses_struct/intsizes.py
+-rw-r--r--   0        0        0        0 2023-07-25 23:44:26.259255 dataclasses_struct-0.8.2/dataclasses_struct/py.typed
+-rw-r--r--   0        0        0     1340 2024-05-16 08:02:14.111463 dataclasses_struct-0.8.2/dataclasses_struct/types.py
+-rw-r--r--   0        0        0     2062 2024-05-16 08:03:30.215449 dataclasses_struct-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     7809 1970-01-01 00:00:00.000000 dataclasses_struct-0.8.2/PKG-INFO
```

### Comparing `dataclasses_struct-0.8.1/LICENSE` & `dataclasses_struct-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.8.1/README.md` & `dataclasses_struct-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.8.1/dataclasses_struct/__init__.py` & `dataclasses_struct-0.8.2/dataclasses_struct/__init__.py`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.8.1/dataclasses_struct/dataclass.py` & `dataclasses_struct-0.8.2/dataclasses_struct/dataclass.py`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.8.1/dataclasses_struct/ext/mypy_plugin.py` & `dataclasses_struct-0.8.2/dataclasses_struct/ext/mypy_plugin.py`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.8.1/dataclasses_struct/field.py` & `dataclasses_struct-0.8.2/dataclasses_struct/field.py`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.8.1/dataclasses_struct/types.py` & `dataclasses_struct-0.8.2/dataclasses_struct/types.py`

 * *Files identical despite different names*

### Comparing `dataclasses_struct-0.8.1/pyproject.toml` & `dataclasses_struct-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataclasses-struct"
-version = "0.8.1"
+version = "0.8.2"
 description = "Converting dataclasses to and from fixed-length binary data using struct"
 authors = ["Harry Mander <harrymander96@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/harrymander/dataclasses-struct"
 repository = "https://github.com/harrymander/dataclasses-struct"
 documentation = "https://github.com/harrymander/dataclasses-struct/blob/main/README.md#usage"
@@ -28,15 +28,14 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 typing-extensions = "^4.5.0"
-mypy = "^1.9.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.1.1"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-mypy-plugins = "^1.10.1"
 ruff = "^0.2.2"
```

### Comparing `dataclasses_struct-0.8.1/PKG-INFO` & `dataclasses_struct-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclasses-struct
-Version: 0.8.1
+Version: 0.8.2
 Summary: Converting dataclasses to and from fixed-length binary data using struct
 Home-page: https://github.com/harrymander/dataclasses-struct
 License: MIT
 Author: Harry Mander
 Author-email: harrymander96@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
@@ -20,15 +20,14 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Dist: mypy (>=1.9.0,<2.0.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Documentation, https://github.com/harrymander/dataclasses-struct/blob/main/README.md#usage
 Project-URL: Repository, https://github.com/harrymander/dataclasses-struct
 Description-Content-Type: text/markdown
 
 # dataclasses-struct
```

