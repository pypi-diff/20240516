# Comparing `tmp/spyder_index-0.2.1.tar.gz` & `tmp/spyder_index-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyder_index-0.2.1.tar", last modified: Mon May 13 22:06:47 2024, max compression
+gzip compressed data, was "spyder_index-0.2.2.tar", last modified: Thu May 16 15:02:01 2024, max compression
```

## Comparing `spyder_index-0.2.1.tar` & `spyder_index-0.2.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.341586 spyder_index-0.2.1/
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1071 2024-05-13 20:08:52.000000 spyder_index-0.2.1/LICENSE
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)    10265 2024-05-13 22:06:47.340342 spyder_index-0.2.1/PKG-INFO
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     9007 2024-05-13 22:04:23.000000 spyder_index-0.2.1/README.md
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1333 2024-05-13 21:02:14.000000 spyder_index-0.2.1/pyproject.toml
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)       38 2024-05-13 22:06:47.341841 spyder_index-0.2.1/setup.cfg
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.268308 spyder_index-0.2.1/spyder_index/
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)       21 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/__init__.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.254254 spyder_index-0.2.1/spyder_index/core/
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.283589 spyder_index-0.2.1/spyder_index/core/document/
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)       83 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/document/__init__.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     2168 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/document/base.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.288905 spyder_index-0.2.1/spyder_index/core/embeddings/
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)       89 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/embeddings/__init__.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      728 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/embeddings/base.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.293167 spyder_index-0.2.1/spyder_index/core/readers/
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)       86 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/readers/__init__.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      533 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/readers/base.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.298167 spyder_index-0.2.1/spyder_index/core/vector_stores/
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      116 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/vector_stores/__init__.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      256 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/core/vector_stores/base.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.304127 spyder_index-0.2.1/spyder_index/embeddings/
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      117 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/embeddings/__init__.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     2024 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/embeddings/huggingface.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.311582 spyder_index-0.2.1/spyder_index/readers/
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      165 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/readers/__init__.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     2086 2024-05-13 20:49:18.000000 spyder_index-0.2.1/spyder_index/readers/directory.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.325353 spyder_index-0.2.1/spyder_index/readers/file/
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      311 2024-05-13 20:44:59.000000 spyder_index-0.2.1/spyder_index/readers/file/__init__.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      815 2024-05-13 20:33:50.000000 spyder_index-0.2.1/spyder_index/readers/file/docx.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      831 2024-05-13 20:44:21.000000 spyder_index-0.2.1/spyder_index/readers/file/html.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1112 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/readers/file/json.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      812 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/readers/file/pdf.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      703 2024-05-13 20:59:47.000000 spyder_index-0.2.1/spyder_index/readers/file/unstructured.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1595 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/readers/s3.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.330024 spyder_index-0.2.1/spyder_index/text_splitters/
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      200 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/text_splitters/__init__.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1832 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/text_splitters/semantic.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1371 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/text_splitters/sentence.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.335156 spyder_index-0.2.1/spyder_index/vector_stores/
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      128 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/vector_stores/__init__.py
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     7619 2024-05-13 20:08:52.000000 spyder_index-0.2.1/spyder_index/vector_stores/elasticsearch.py
-drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-13 22:06:47.338239 spyder_index-0.2.1/spyder_index.egg-info/
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)    10265 2024-05-13 22:06:47.000000 spyder_index-0.2.1/spyder_index.egg-info/PKG-INFO
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1131 2024-05-13 22:06:47.000000 spyder_index-0.2.1/spyder_index.egg-info/SOURCES.txt
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)        1 2024-05-13 22:06:47.000000 spyder_index-0.2.1/spyder_index.egg-info/dependency_links.txt
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)      251 2024-05-13 22:06:47.000000 spyder_index-0.2.1/spyder_index.egg-info/requires.txt
--rw-r--r--   0 leonardofurnielis   (501) staff       (20)       13 2024-05-13 22:06:47.000000 spyder_index-0.2.1/spyder_index.egg-info/top_level.txt
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-16 15:02:01.134026 spyder_index-0.2.2/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1071 2024-05-16 14:52:03.000000 spyder_index-0.2.2/LICENSE
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1891 2024-05-16 15:02:01.132870 spyder_index-0.2.2/PKG-INFO
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      487 2024-05-16 14:52:03.000000 spyder_index-0.2.2/README.md
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1471 2024-05-16 15:00:43.000000 spyder_index-0.2.2/pyproject.toml
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       38 2024-05-16 15:02:01.134349 spyder_index-0.2.2/setup.cfg
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-16 15:02:01.097056 spyder_index-0.2.2/spyder_index/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       21 2024-05-16 14:52:52.000000 spyder_index-0.2.2/spyder_index/__init__.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-16 15:02:01.087334 spyder_index-0.2.2/spyder_index/core/
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-16 15:02:01.105776 spyder_index-0.2.2/spyder_index/core/document/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       83 2024-05-16 14:52:03.000000 spyder_index-0.2.2/spyder_index/core/document/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     2168 2024-05-16 14:52:03.000000 spyder_index-0.2.2/spyder_index/core/document/base.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-16 15:02:01.107920 spyder_index-0.2.2/spyder_index/core/embeddings/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       89 2024-05-16 14:52:03.000000 spyder_index-0.2.2/spyder_index/core/embeddings/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      728 2024-05-16 14:52:03.000000 spyder_index-0.2.2/spyder_index/core/embeddings/base.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-16 15:02:01.110711 spyder_index-0.2.2/spyder_index/core/readers/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       86 2024-05-16 14:52:03.000000 spyder_index-0.2.2/spyder_index/core/readers/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      533 2024-05-16 14:52:03.000000 spyder_index-0.2.2/spyder_index/core/readers/base.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-16 15:02:01.112696 spyder_index-0.2.2/spyder_index/core/vector_stores/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      116 2024-05-16 14:52:03.000000 spyder_index-0.2.2/spyder_index/core/vector_stores/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      256 2024-05-16 14:52:03.000000 spyder_index-0.2.2/spyder_index/core/vector_stores/base.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-16 15:02:01.114429 spyder_index-0.2.2/spyder_index/embeddings/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      117 2024-05-16 14:52:03.000000 spyder_index-0.2.2/spyder_index/embeddings/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     2024 2024-05-16 14:52:03.000000 spyder_index-0.2.2/spyder_index/embeddings/huggingface.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-16 15:02:01.117876 spyder_index-0.2.2/spyder_index/readers/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      165 2024-05-16 14:52:04.000000 spyder_index-0.2.2/spyder_index/readers/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     2086 2024-05-16 14:52:04.000000 spyder_index-0.2.2/spyder_index/readers/directory.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-16 15:02:01.124340 spyder_index-0.2.2/spyder_index/readers/file/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      311 2024-05-16 14:52:04.000000 spyder_index-0.2.2/spyder_index/readers/file/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      815 2024-05-16 14:52:04.000000 spyder_index-0.2.2/spyder_index/readers/file/docx.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      831 2024-05-16 14:52:04.000000 spyder_index-0.2.2/spyder_index/readers/file/html.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1112 2024-05-16 14:52:04.000000 spyder_index-0.2.2/spyder_index/readers/file/json.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      812 2024-05-16 14:52:04.000000 spyder_index-0.2.2/spyder_index/readers/file/pdf.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      703 2024-05-16 14:52:04.000000 spyder_index-0.2.2/spyder_index/readers/file/unstructured.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1595 2024-05-16 14:52:04.000000 spyder_index-0.2.2/spyder_index/readers/s3.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-16 15:02:01.127115 spyder_index-0.2.2/spyder_index/text_splitters/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      200 2024-05-16 14:52:04.000000 spyder_index-0.2.2/spyder_index/text_splitters/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1832 2024-05-16 14:52:04.000000 spyder_index-0.2.2/spyder_index/text_splitters/semantic.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1371 2024-05-16 14:52:04.000000 spyder_index-0.2.2/spyder_index/text_splitters/sentence.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-16 15:02:01.128770 spyder_index-0.2.2/spyder_index/vector_stores/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      128 2024-05-16 14:52:04.000000 spyder_index-0.2.2/spyder_index/vector_stores/__init__.py
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     7619 2024-05-16 14:52:04.000000 spyder_index-0.2.2/spyder_index/vector_stores/elasticsearch.py
+drwxr-xr-x   0 leonardofurnielis   (501) staff       (20)        0 2024-05-16 15:02:01.130723 spyder_index-0.2.2/spyder_index.egg-info/
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1891 2024-05-16 15:02:01.000000 spyder_index-0.2.2/spyder_index.egg-info/PKG-INFO
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)     1131 2024-05-16 15:02:01.000000 spyder_index-0.2.2/spyder_index.egg-info/SOURCES.txt
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)        1 2024-05-16 15:02:01.000000 spyder_index-0.2.2/spyder_index.egg-info/dependency_links.txt
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)      274 2024-05-16 15:02:01.000000 spyder_index-0.2.2/spyder_index.egg-info/requires.txt
+-rw-r--r--   0 leonardofurnielis   (501) staff       (20)       13 2024-05-16 15:02:01.000000 spyder_index-0.2.2/spyder_index.egg-info/top_level.txt
```

### Comparing `spyder_index-0.2.1/LICENSE` & `spyder_index-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.1/pyproject.toml` & `spyder_index-0.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0","wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spyder-index"
-version = "0.2.1"
+version = "0.2.2"
 description = "Spyder Index is an open-source framework for building LLM applications"
 readme = "README.md"
 authors = [{ name = "Leonardo Furnielis" }]
 license = {text = "MIT License"}
 keywords = ["framework", "RAG", "index", "data", "LLM", "AI", "semantic search"]
 dependencies = [
     "langchain-core ~= 0.1.48",
@@ -20,19 +20,24 @@
     "pypdf ~= 4.2.0",
     "torch == 2.1.0",
     "elasticsearch ~= 8.13.0",
     "ibm-cos-sdk ~= 2.13.2",
     "jq ~= 1.7.0",
     "docx2txt ~= 0.8"
 ]
+
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 
+[project.optional-dependencies] 
+docs = ["furo ~= 2024.5.6"]
+
 [project.urls]
 Homepage = "https://github.com/leonardofurnielis/spyder_index"
-Issues = "https://github.com/leonardofurnielis/spyder_index/issues"
+Documentation = "https://leonardofurnielis.github.io/spyder_index/"
+Issues = "https://github.com/leonardofurnielis/spyder_index/issues"
```

### Comparing `spyder_index-0.2.1/spyder_index/core/document/base.py` & `spyder_index-0.2.2/spyder_index/core/document/base.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.1/spyder_index/core/embeddings/base.py` & `spyder_index-0.2.2/spyder_index/core/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.1/spyder_index/core/readers/base.py` & `spyder_index-0.2.2/spyder_index/core/readers/base.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.1/spyder_index/embeddings/huggingface.py` & `spyder_index-0.2.2/spyder_index/embeddings/huggingface.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.1/spyder_index/readers/directory.py` & `spyder_index-0.2.2/spyder_index/readers/directory.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.1/spyder_index/readers/file/docx.py` & `spyder_index-0.2.2/spyder_index/readers/file/docx.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.1/spyder_index/readers/file/html.py` & `spyder_index-0.2.2/spyder_index/readers/file/html.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.1/spyder_index/readers/file/json.py` & `spyder_index-0.2.2/spyder_index/readers/file/json.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.1/spyder_index/readers/file/pdf.py` & `spyder_index-0.2.2/spyder_index/readers/file/pdf.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.1/spyder_index/readers/file/unstructured.py` & `spyder_index-0.2.2/spyder_index/readers/file/unstructured.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.1/spyder_index/readers/s3.py` & `spyder_index-0.2.2/spyder_index/readers/s3.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.1/spyder_index/text_splitters/semantic.py` & `spyder_index-0.2.2/spyder_index/text_splitters/semantic.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.1/spyder_index/text_splitters/sentence.py` & `spyder_index-0.2.2/spyder_index/text_splitters/sentence.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.1/spyder_index/vector_stores/elasticsearch.py` & `spyder_index-0.2.2/spyder_index/vector_stores/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `spyder_index-0.2.1/spyder_index.egg-info/SOURCES.txt` & `spyder_index-0.2.2/spyder_index.egg-info/SOURCES.txt`

 * *Files identical despite different names*

