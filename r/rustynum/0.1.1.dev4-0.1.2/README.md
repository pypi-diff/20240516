# Comparing `tmp/rustynum-0.1.1.dev4.tar.gz` & `tmp/rustynum-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rustynum-0.1.1.dev4.tar", last modified: Thu May 16 18:32:55 2024, max compression
+gzip compressed data, was "rustynum-0.1.2.tar", last modified: Thu May 16 21:16:52 2024, max compression
```

## Comparing `rustynum-0.1.1.dev4.tar` & `rustynum-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:32:55.267681 rustynum-0.1.1.dev4/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-16 18:32:55.267681 rustynum-0.1.1.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:32:43.000000 rustynum-0.1.1.dev4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-16 18:32:43.000000 rustynum-0.1.1.dev4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:32:55.263681 rustynum-0.1.1.dev4/rustynum/
--rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-05-16 18:32:43.000000 rustynum-0.1.1.dev4/rustynum/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:32:55.267681 rustynum-0.1.1.dev4/rustynum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-16 18:32:55.000000 rustynum-0.1.1.dev4/rustynum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-16 18:32:55.000000 rustynum-0.1.1.dev4/rustynum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:32:55.000000 rustynum-0.1.1.dev4/rustynum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:32:55.000000 rustynum-0.1.1.dev4/rustynum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 18:32:55.000000 rustynum-0.1.1.dev4/rustynum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 18:32:55.000000 rustynum-0.1.1.dev4/rustynum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 18:32:55.267681 rustynum-0.1.1.dev4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-16 18:32:43.000000 rustynum-0.1.1.dev4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:32:55.267681 rustynum-0.1.1.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-16 18:32:43.000000 rustynum-0.1.1.dev4/tests/test_array_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-16 18:32:43.000000 rustynum-0.1.1.dev4/tests/test_complex_flows.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-16 18:32:43.000000 rustynum-0.1.1.dev4/tests/test_dot_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-16 18:32:43.000000 rustynum-0.1.1.dev4/tests/test_mean.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-16 18:32:43.000000 rustynum-0.1.1.dev4/tests/test_min_max.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:16:52.046202 rustynum-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-16 21:16:52.046202 rustynum-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 21:16:43.000000 rustynum-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-16 21:16:43.000000 rustynum-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:16:52.042202 rustynum-0.1.2/rustynum/
+-rw-r--r--   0 runner    (1001) docker     (127)    11642 2024-05-16 21:16:43.000000 rustynum-0.1.2/rustynum/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:16:52.042202 rustynum-0.1.2/rustynum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-16 21:16:52.000000 rustynum-0.1.2/rustynum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-16 21:16:52.000000 rustynum-0.1.2/rustynum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:16:52.000000 rustynum-0.1.2/rustynum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 21:16:51.000000 rustynum-0.1.2/rustynum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 21:16:52.000000 rustynum-0.1.2/rustynum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 21:16:52.000000 rustynum-0.1.2/rustynum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 21:16:52.046202 rustynum-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-16 21:16:43.000000 rustynum-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 21:16:52.042202 rustynum-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-16 21:16:43.000000 rustynum-0.1.2/tests/test_array_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-16 21:16:43.000000 rustynum-0.1.2/tests/test_complex_flows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-16 21:16:43.000000 rustynum-0.1.2/tests/test_dot_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-16 21:16:43.000000 rustynum-0.1.2/tests/test_mean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-16 21:16:43.000000 rustynum-0.1.2/tests/test_min_max.py
```

### Comparing `rustynum-0.1.1.dev4/PKG-INFO` & `rustynum-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustynum
-Version: 0.1.1.dev4
+Version: 0.1.2
 Summary: Python wrapper for the RustyNum library bindings
 Author: IgorSusmelj
 Author-email: isusmelj@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: OS Independent
```

### Comparing `rustynum-0.1.1.dev4/rustynum/__init__.py` & `rustynum-0.1.2/rustynum/__init__.py`

 * *Files identical despite different names*

### Comparing `rustynum-0.1.1.dev4/rustynum.egg-info/PKG-INFO` & `rustynum-0.1.2/rustynum.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rustynum
-Version: 0.1.1.dev4
+Version: 0.1.2
 Summary: Python wrapper for the RustyNum library bindings
 Author: IgorSusmelj
 Author-email: isusmelj@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: OS Independent
```

### Comparing `rustynum-0.1.1.dev4/setup.py` & `rustynum-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from setuptools_rust import Binding, RustExtension
 
 setup(
     name="rustynum",
-    version="0.1.1.dev4",
+    version="0.1.2",
     description="Python wrapper for the RustyNum library bindings",
     author="IgorSusmelj",
     author_email="isusmelj@gmail.com",
     license="MIT",
     rust_extensions=[
         RustExtension(
             "rustynum._rustynum",
```

### Comparing `rustynum-0.1.1.dev4/tests/test_array_ops.py` & `rustynum-0.1.2/tests/test_array_ops.py`

 * *Files identical despite different names*

### Comparing `rustynum-0.1.1.dev4/tests/test_complex_flows.py` & `rustynum-0.1.2/tests/test_complex_flows.py`

 * *Files identical despite different names*

### Comparing `rustynum-0.1.1.dev4/tests/test_dot_product.py` & `rustynum-0.1.2/tests/test_dot_product.py`

 * *Files identical despite different names*

### Comparing `rustynum-0.1.1.dev4/tests/test_mean.py` & `rustynum-0.1.2/tests/test_mean.py`

 * *Files identical despite different names*

### Comparing `rustynum-0.1.1.dev4/tests/test_min_max.py` & `rustynum-0.1.2/tests/test_min_max.py`

 * *Files identical despite different names*

