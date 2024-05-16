# Comparing `tmp/data_transformation_library_paula-0.1.0.tar.gz` & `tmp/data_transformation_library_paula-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_transformation_library_paula-0.1.0.tar", max compression
+gzip compressed data, was "data_transformation_library_paula-0.1.1.tar", max compression
```

## Comparing `data_transformation_library_paula-0.1.0.tar` & `data_transformation_library_paula-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-05-16 11:33:25.380607 data_transformation_library_paula-0.1.0/data_transformation_library_paula/__init__.py
--rw-r--r--   0        0        0     4925 2024-05-16 12:14:08.274181 data_transformation_library_paula-0.1.0/data_transformation_library_paula/transformation_functions.py
--rw-r--r--   0        0        0     2851 2024-05-16 12:13:56.543951 data_transformation_library_paula-0.1.0/data_transformation_library_paula/validators.py
--rw-r--r--   0        0        0      325 2024-05-16 11:37:05.355927 data_transformation_library_paula-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2604 2024-05-16 12:14:41.243043 data_transformation_library_paula-0.1.0/README.md
--rw-r--r--   0        0        0     2878 1970-01-01 00:00:00.000000 data_transformation_library_paula-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-16 11:33:25.380607 data_transformation_library_paula-0.1.1/data_transformation_library_paula/__init__.py
+-rw-r--r--   0        0        0     4925 2024-05-16 12:14:08.274181 data_transformation_library_paula-0.1.1/data_transformation_library_paula/transformation_functions.py
+-rw-r--r--   0        0        0     2851 2024-05-16 12:13:56.543951 data_transformation_library_paula-0.1.1/data_transformation_library_paula/validators.py
+-rw-r--r--   0        0        0      607 2024-05-16 12:29:20.904918 data_transformation_library_paula-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2604 2024-05-16 12:14:41.243043 data_transformation_library_paula-0.1.1/README.md
+-rw-r--r--   0        0        0     3160 1970-01-01 00:00:00.000000 data_transformation_library_paula-0.1.1/PKG-INFO
```

### Comparing `data_transformation_library_paula-0.1.0/data_transformation_library_paula/transformation_functions.py` & `data_transformation_library_paula-0.1.1/data_transformation_library_paula/transformation_functions.py`

 * *Files identical despite different names*

### Comparing `data_transformation_library_paula-0.1.0/data_transformation_library_paula/validators.py` & `data_transformation_library_paula-0.1.1/data_transformation_library_paula/validators.py`

 * *Files identical despite different names*

### Comparing `data_transformation_library_paula-0.1.0/README.md` & `data_transformation_library_paula-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `data_transformation_library_paula-0.1.0/PKG-INFO` & `data_transformation_library_paula-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: data-transformation-library-paula
-Version: 0.1.0
-Summary: 
+Version: 0.1.1
+Summary: The `data-transformation-library-paula` is a Python package focused on providing essential tools for matrix operations and data transformations. These functions are fundamental for handling and processing data in areas like machine learning, signal processing, and image processing.
 Author: Paula
 Author-email: paula.valaityte@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Description-Content-Type: text/markdown
```

