# Comparing `tmp/glue_utils-0.3.1.tar.gz` & `tmp/glue_utils-0.4.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_utils-0.3.1.tar", max compression
+gzip compressed data, was "glue_utils-0.4.0rc0.tar", max compression
```

## Comparing `glue_utils-0.3.1.tar` & `glue_utils-0.4.0rc0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.3.1/LICENSE
--rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.3.1/README.md
--rw-r--r--   0        0        0     3822 2024-05-13 03:18:52.496013 glue_utils-0.3.1/pyproject.toml
--rw-r--r--   0        0        0       89 2024-05-13 03:18:52.496772 glue_utils-0.3.1/src/glue_utils/__init__.py
--rw-r--r--   0        0        0     1050 2024-05-10 09:44:26.756369 glue_utils-0.3.1/src/glue_utils/options.py
--rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.3.1/src/glue_utils/py.typed
--rw-r--r--   0        0        0      577 2024-05-12 10:26:39.523202 glue_utils-0.3.1/src/glue_utils/pyspark/__init__.py
--rw-r--r--   0        0        0      674 2024-05-10 12:17:39.961510 glue_utils-0.3.1/src/glue_utils/pyspark/context.py
--rw-r--r--   0        0        0     2652 2024-05-10 12:17:39.961783 glue_utils-0.3.1/src/glue_utils/pyspark/job.py
--rw-r--r--   0        0        0      466 2024-05-12 10:26:39.523784 glue_utils-0.3.1/src/glue_utils/pyspark/mixins/__init__.py
--rw-r--r--   0        0        0      849 2024-05-10 12:17:39.962157 glue_utils-0.3.1/src/glue_utils/pyspark/mixins/connection_types.py
--rw-r--r--   0        0        0     8981 2024-05-12 10:26:39.524433 glue_utils-0.3.1/src/glue_utils/pyspark/mixins/jdbc.py
--rw-r--r--   0        0        0    13057 2024-05-12 10:26:39.525070 glue_utils-0.3.1/src/glue_utils/pyspark/mixins/s3.py
--rw-r--r--   0        0        0     2250 1970-01-01 00:00:00.000000 glue_utils-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.4.0rc0/LICENSE
+-rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.4.0rc0/README.md
+-rw-r--r--   0        0        0     3828 2024-05-12 10:27:19.294331 glue_utils-0.4.0rc0/pyproject.toml
+-rw-r--r--   0        0        0       92 2024-05-12 10:27:19.294679 glue_utils-0.4.0rc0/src/glue_utils/__init__.py
+-rw-r--r--   0        0        0     1050 2024-05-10 09:44:26.756369 glue_utils-0.4.0rc0/src/glue_utils/options.py
+-rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.4.0rc0/src/glue_utils/py.typed
+-rw-r--r--   0        0        0      577 2024-05-12 10:26:39.523202 glue_utils-0.4.0rc0/src/glue_utils/pyspark/__init__.py
+-rw-r--r--   0        0        0      674 2024-05-10 12:17:39.961510 glue_utils-0.4.0rc0/src/glue_utils/pyspark/context.py
+-rw-r--r--   0        0        0     2652 2024-05-10 12:17:39.961783 glue_utils-0.4.0rc0/src/glue_utils/pyspark/job.py
+-rw-r--r--   0        0        0      466 2024-05-12 10:26:39.523784 glue_utils-0.4.0rc0/src/glue_utils/pyspark/mixins/__init__.py
+-rw-r--r--   0        0        0      849 2024-05-10 12:17:39.962157 glue_utils-0.4.0rc0/src/glue_utils/pyspark/mixins/connection_types.py
+-rw-r--r--   0        0        0     8981 2024-05-12 10:26:39.524433 glue_utils-0.4.0rc0/src/glue_utils/pyspark/mixins/jdbc.py
+-rw-r--r--   0        0        0    13057 2024-05-12 10:26:39.525070 glue_utils-0.4.0rc0/src/glue_utils/pyspark/mixins/s3.py
+-rw-r--r--   0        0        0     2253 1970-01-01 00:00:00.000000 glue_utils-0.4.0rc0/PKG-INFO
```

### Comparing `glue_utils-0.3.1/LICENSE` & `glue_utils-0.4.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.1/README.md` & `glue_utils-0.4.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.1/pyproject.toml` & `glue_utils-0.4.0rc0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glue-utils"
-version = "0.3.1"
+version = "0.4.0rc0"
 package-mode = true
 description = "Reusable utilities for working with Glue PySpark jobs"
 authors = ["Noel Llevares <dashmug@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dashmug/glue-utils"
 repository = "https://github.com/dashmug/glue-utils/issues"
@@ -126,15 +126,15 @@
     "if TYPE_CHECKING:",
     "class .*\\bProtocol\\):",
     "@(abc\\.)?abstractmethod",
     "@overload",
 ]
 
 [tool.bumpver]
-current_version = "0.3.1"
+current_version = "0.4.0rc0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "release: Bump version {old_version} -> {new_version}"
 commit = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
```

### Comparing `glue_utils-0.3.1/src/glue_utils/options.py` & `glue_utils-0.4.0rc0/src/glue_utils/options.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.1/src/glue_utils/pyspark/__init__.py` & `glue_utils-0.4.0rc0/src/glue_utils/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.1/src/glue_utils/pyspark/context.py` & `glue_utils-0.4.0rc0/src/glue_utils/pyspark/context.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.1/src/glue_utils/pyspark/job.py` & `glue_utils-0.4.0rc0/src/glue_utils/pyspark/job.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.1/src/glue_utils/pyspark/mixins/connection_types.py` & `glue_utils-0.4.0rc0/src/glue_utils/pyspark/mixins/connection_types.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.1/src/glue_utils/pyspark/mixins/jdbc.py` & `glue_utils-0.4.0rc0/src/glue_utils/pyspark/mixins/jdbc.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.1/src/glue_utils/pyspark/mixins/s3.py` & `glue_utils-0.4.0rc0/src/glue_utils/pyspark/mixins/s3.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.3.1/PKG-INFO` & `glue_utils-0.4.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-utils
-Version: 0.3.1
+Version: 0.4.0rc0
 Summary: Reusable utilities for working with Glue PySpark jobs
 Home-page: https://github.com/dashmug/glue-utils
 License: MIT
 Keywords: aws,glue,pyspark,spark,etl,data,data-engineering
 Author: Noel Llevares
 Author-email: dashmug@gmail.com
 Requires-Python: >=3.9,<4.0
```

