# Comparing `tmp/fasta_reader-3.0.2.tar.gz` & `tmp/fasta_reader-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasta_reader-3.0.2.tar", max compression
+gzip compressed data, was "fasta_reader-3.0.3.tar", max compression
```

## Comparing `fasta_reader-3.0.2.tar` & `fasta_reader-3.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2022-08-26 07:28:18.000000 fasta_reader-3.0.2/LICENSE
--rw-r--r--   0        0        0      919 2023-03-02 06:06:57.377717 fasta_reader-3.0.2/README.md
--rw-r--r--   0        0        0      235 2023-03-02 05:01:40.883341 fasta_reader-3.0.2/fasta_reader/__init__.py
--rw-r--r--   0        0        0      360 2023-03-02 06:01:38.689544 fasta_reader-3.0.2/fasta_reader/anyfile.py
--rw-r--r--   0        0        0      522 2023-03-01 15:01:24.738199 fasta_reader-3.0.2/fasta_reader/errors.py
--rw-r--r--   0        0        0     1963 2023-07-07 23:21:16.775783 fasta_reader-3.0.2/fasta_reader/item.py
--rw-r--r--   0        0        0      667 2023-07-07 22:50:02.159288 fasta_reader-3.0.2/fasta_reader/read_fasta.py
--rw-r--r--   0        0        0     2044 2023-03-02 05:43:43.812105 fasta_reader-3.0.2/fasta_reader/reader.py
--rw-r--r--   0        0        0       81 2023-03-02 04:49:20.007071 fasta_reader-3.0.2/fasta_reader/uri.py
--rw-r--r--   0        0        0      679 2023-03-02 06:06:20.890334 fasta_reader-3.0.2/fasta_reader/write_fasta.py
--rw-r--r--   0        0        0      987 2023-03-02 06:03:24.398973 fasta_reader-3.0.2/fasta_reader/writer.py
--rw-r--r--   0        0        0      582 2023-07-07 22:53:53.375347 fasta_reader-3.0.2/pyproject.toml
--rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 fasta_reader-3.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-08-26 07:28:18.000000 fasta_reader-3.0.3/LICENSE
+-rw-r--r--   0        0        0      919 2023-03-02 06:06:57.377717 fasta_reader-3.0.3/README.md
+-rw-r--r--   0        0        0      235 2024-05-16 12:45:47.598994 fasta_reader-3.0.3/fasta_reader/__init__.py
+-rw-r--r--   0        0        0      360 2024-05-16 12:46:39.146256 fasta_reader-3.0.3/fasta_reader/anyfile.py
+-rw-r--r--   0        0        0      522 2024-05-16 12:47:13.209295 fasta_reader-3.0.3/fasta_reader/errors.py
+-rw-r--r--   0        0        0     1963 2024-05-16 12:47:19.907416 fasta_reader-3.0.3/fasta_reader/item.py
+-rw-r--r--   0        0        0      667 2024-05-16 12:47:22.730701 fasta_reader-3.0.3/fasta_reader/read_fasta.py
+-rw-r--r--   0        0        0     2044 2024-05-16 12:47:25.887553 fasta_reader-3.0.3/fasta_reader/reader.py
+-rw-r--r--   0        0        0       81 2024-05-16 12:47:29.363039 fasta_reader-3.0.3/fasta_reader/uri.py
+-rw-r--r--   0        0        0      679 2024-05-16 12:47:30.850421 fasta_reader-3.0.3/fasta_reader/write_fasta.py
+-rw-r--r--   0        0        0      987 2024-05-16 12:47:35.178485 fasta_reader-3.0.3/fasta_reader/writer.py
+-rw-r--r--   0        0        0      519 2024-05-16 12:51:07.214506 fasta_reader-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 fasta_reader-3.0.3/PKG-INFO
```

### Comparing `fasta_reader-3.0.2/LICENSE` & `fasta_reader-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.2/README.md` & `fasta_reader-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.2/fasta_reader/errors.py` & `fasta_reader-3.0.3/fasta_reader/errors.py`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.2/fasta_reader/item.py` & `fasta_reader-3.0.3/fasta_reader/item.py`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.2/fasta_reader/read_fasta.py` & `fasta_reader-3.0.3/fasta_reader/read_fasta.py`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.2/fasta_reader/reader.py` & `fasta_reader-3.0.3/fasta_reader/reader.py`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.2/fasta_reader/write_fasta.py` & `fasta_reader-3.0.3/fasta_reader/write_fasta.py`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.2/fasta_reader/writer.py` & `fasta_reader-3.0.3/fasta_reader/writer.py`

 * *Files identical despite different names*

### Comparing `fasta_reader-3.0.2/pyproject.toml` & `fasta_reader-3.0.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 [tool.poetry]
 name = "fasta-reader"
-version = "3.0.2"
+version = "3.0.3"
 description = "FASTA file reader/writer."
 authors = ["Danilo Horta <fdanilo.horta@pm.me>"]
 repository = "https://github.com/EBI-Metagenomics/fasta-reader"
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "fasta_reader" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-fsspec = { version = ">=2023.1.0" }
+fsspec = ">=2024.5.0"
 
 [tool.poetry.group.dev.dependencies]
-deptry = ">=0.6.4"
-pre-commit = ">=2.20.0"
-pytest = ">=7.2.0"
-pytest-datafiles = ">=3.0.0"
+pytest = "^8.2"
+pytest-datafiles = "^3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fasta_reader-3.0.2/PKG-INFO` & `fasta_reader-3.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: fasta-reader
-Version: 3.0.2
+Version: 3.0.3
 Summary: FASTA file reader/writer.
 Home-page: https://github.com/EBI-Metagenomics/fasta-reader
 License: MIT
 Author: Danilo Horta
 Author-email: fdanilo.horta@pm.me
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: fsspec (>=2023.1.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: fsspec (>=2024.5.0)
 Project-URL: Repository, https://github.com/EBI-Metagenomics/fasta-reader
 Description-Content-Type: text/markdown
 
 # Welcome to fasta-reader 👋
 
 > Read and write FASTA file
```

