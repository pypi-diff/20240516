# Comparing `tmp/readii-1.3.0.tar.gz` & `tmp/readii-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readii-1.3.0.tar", max compression
+gzip compressed data, was "readii-1.3.1.tar", max compression
```

## Comparing `readii-1.3.0.tar` & `readii-1.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rwxr-xr-x   0        0        0     1069 2024-05-16 19:13:13.001227 readii-1.3.0/LICENSE
--rw-r--r--   0        0        0     2053 2024-05-16 19:13:13.001227 readii-1.3.0/README.md
--rw-r--r--   0        0        0     1381 2024-05-16 19:14:04.885192 readii-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      100 2024-05-16 19:13:55.605198 readii-1.3.0/src/readii/__init__.py
--rw-r--r--   0        0        0        0 2024-05-16 19:13:13.005227 readii-1.3.0/src/readii/data/__init__.py
--rw-r--r--   0        0        0      299 2024-05-16 19:13:13.005227 readii-1.3.0/src/readii/data/default_pyradiomics.yaml
--rw-r--r--   0        0        0    14813 2024-05-16 19:13:13.005227 readii-1.3.0/src/readii/feature_extraction.py
--rw-r--r--   0        0        0    12227 2024-05-16 19:13:13.005227 readii-1.3.0/src/readii/image_processing.py
--rw-r--r--   0        0        0     4192 2024-05-16 19:13:13.005227 readii-1.3.0/src/readii/loaders.py
--rw-r--r--   0        0        0     5959 2024-05-16 19:13:13.005227 readii-1.3.0/src/readii/metadata.py
--rw-r--r--   0        0        0    24474 2024-05-16 19:13:13.005227 readii-1.3.0/src/readii/negative_controls.py
--rw-r--r--   0        0        0     6126 2024-05-16 19:13:13.005227 readii-1.3.0/src/readii/pipeline.py
--rw-r--r--   0        0        0     2828 1970-01-01 00:00:00.000000 readii-1.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2024-05-16 19:40:04.791849 readii-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2096 2024-05-16 19:40:04.791849 readii-1.3.1/README.md
+-rw-r--r--   0        0        0     1381 2024-05-16 19:40:57.119829 readii-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      100 2024-05-16 19:40:48.215834 readii-1.3.1/src/readii/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 19:40:04.795848 readii-1.3.1/src/readii/data/__init__.py
+-rw-r--r--   0        0        0      299 2024-05-16 19:40:04.795848 readii-1.3.1/src/readii/data/default_pyradiomics.yaml
+-rw-r--r--   0        0        0    14813 2024-05-16 19:40:04.795848 readii-1.3.1/src/readii/feature_extraction.py
+-rw-r--r--   0        0        0    12227 2024-05-16 19:40:04.795848 readii-1.3.1/src/readii/image_processing.py
+-rw-r--r--   0        0        0     4192 2024-05-16 19:40:04.795848 readii-1.3.1/src/readii/loaders.py
+-rw-r--r--   0        0        0     5959 2024-05-16 19:40:04.795848 readii-1.3.1/src/readii/metadata.py
+-rw-r--r--   0        0        0    24474 2024-05-16 19:40:04.795848 readii-1.3.1/src/readii/negative_controls.py
+-rw-r--r--   0        0        0     6126 2024-05-16 19:40:04.795848 readii-1.3.1/src/readii/pipeline.py
+-rw-r--r--   0        0        0     2871 1970-01-01 00:00:00.000000 readii-1.3.1/PKG-INFO
```

### Comparing `readii-1.3.0/LICENSE` & `readii-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `readii-1.3.0/README.md` & `readii-1.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # READII
-![Docker Pulls](https://img.shields.io/docker/pulls/bhklab/readii)
+[![Docker Pulls](https://img.shields.io/docker/pulls/bhklab/readii)](https://hub.docker.com/r/bhklab/readii)
+
 ![GitHub Release](https://img.shields.io/github/v/release/bhklab/readii)
 
 
 **R**adiomic **E**xtraction and **A**nalysis for **DI**COM **I**mages
 
 A package to extract radiomic features from DICOM CT images.
```

### Comparing `readii-1.3.0/pyproject.toml` & `readii-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "readii"
-version = "1.3.0"
+version = "1.3.1"
 description = "A package to extract radiomic features!"
 authors = ["Katy Scott"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
```

### Comparing `readii-1.3.0/src/readii/feature_extraction.py` & `readii-1.3.1/src/readii/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `readii-1.3.0/src/readii/image_processing.py` & `readii-1.3.1/src/readii/image_processing.py`

 * *Files identical despite different names*

### Comparing `readii-1.3.0/src/readii/loaders.py` & `readii-1.3.1/src/readii/loaders.py`

 * *Files identical despite different names*

### Comparing `readii-1.3.0/src/readii/metadata.py` & `readii-1.3.1/src/readii/metadata.py`

 * *Files identical despite different names*

### Comparing `readii-1.3.0/src/readii/negative_controls.py` & `readii-1.3.1/src/readii/negative_controls.py`

 * *Files identical despite different names*

### Comparing `readii-1.3.0/src/readii/pipeline.py` & `readii-1.3.1/src/readii/pipeline.py`

 * *Files identical despite different names*

### Comparing `readii-1.3.0/PKG-INFO` & `readii-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readii
-Version: 1.3.0
+Version: 1.3.1
 Summary: A package to extract radiomic features!
 License: MIT
 Author: Katy Scott
 Requires-Python: >=3.9,<4
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -17,15 +17,16 @@
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: pydicom (>=2.3.1)
 Requires-Dist: pyradiomics (==3.0.1a3)
 Requires-Dist: simpleitk (>=2.3.1)
 Description-Content-Type: text/markdown
 
 # READII
-![Docker Pulls](https://img.shields.io/docker/pulls/bhklab/readii)
+[![Docker Pulls](https://img.shields.io/docker/pulls/bhklab/readii)](https://hub.docker.com/r/bhklab/readii)
+
 ![GitHub Release](https://img.shields.io/github/v/release/bhklab/readii)
 
 
 **R**adiomic **E**xtraction and **A**nalysis for **DI**COM **I**mages
 
 A package to extract radiomic features from DICOM CT images.
```

