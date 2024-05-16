# Comparing `tmp/llama_index_indices_managed_zilliz-0.1.2.tar.gz` & `tmp/llama_index_indices_managed_zilliz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_indices_managed_zilliz-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_indices_managed_zilliz-0.1.3.tar", max compression
```

## Comparing `llama_index_indices_managed_zilliz-0.1.2.tar` & `llama_index_indices_managed_zilliz-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       41 2024-02-13 13:53:01.648334 llama_index_indices_managed_zilliz-0.1.2/README.md
--rw-r--r--   0        0        0      235 2024-02-13 13:53:01.648590 llama_index_indices_managed_zilliz-0.1.2/llama_index/indices/managed/zilliz/__init__.py
--rw-r--r--   0        0        0    16349 2024-02-13 13:53:01.648814 llama_index_indices_managed_zilliz-0.1.2/llama_index/indices/managed/zilliz/base.py
--rw-r--r--   0        0        0     2737 2024-02-13 13:53:01.648889 llama_index_indices_managed_zilliz-0.1.2/llama_index/indices/managed/zilliz/retriever.py
--rw-r--r--   0        0        0     1509 2024-02-21 17:18:17.177043 llama_index_indices_managed_zilliz-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      653 1970-01-01 00:00:00.000000 llama_index_indices_managed_zilliz-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-05-03 02:29:56.151647 llama_index_indices_managed_zilliz-0.1.3/README.md
+-rw-r--r--   0        0        0      235 2024-05-03 02:29:56.151647 llama_index_indices_managed_zilliz-0.1.3/llama_index/indices/managed/zilliz/__init__.py
+-rw-r--r--   0        0        0    16349 2024-05-03 02:29:56.151647 llama_index_indices_managed_zilliz-0.1.3/llama_index/indices/managed/zilliz/base.py
+-rw-r--r--   0        0        0     2737 2024-05-03 02:29:56.151647 llama_index_indices_managed_zilliz-0.1.3/llama_index/indices/managed/zilliz/retriever.py
+-rw-r--r--   0        0        0     1550 2024-05-03 02:29:56.151647 llama_index_indices_managed_zilliz-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      602 1970-01-01 00:00:00.000000 llama_index_indices_managed_zilliz-0.1.3/PKG-INFO
```

### Comparing `llama_index_indices_managed_zilliz-0.1.2/llama_index/indices/managed/zilliz/base.py` & `llama_index_indices_managed_zilliz-0.1.3/llama_index/indices/managed/zilliz/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_indices_managed_zilliz-0.1.2/llama_index/indices/managed/zilliz/retriever.py` & `llama_index_indices_managed_zilliz-0.1.3/llama_index/indices/managed/zilliz/retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index_indices_managed_zilliz-0.1.2/pyproject.toml` & `llama_index_indices_managed_zilliz-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 [tool.llamahub]
 contains_example = false
 import_path = "llama_index.indices.managed.zilliz"
 
 [tool.llamahub.class_authors]
 ZillizCloudPipelineIndex = "llama-index"
+
+[tool.llamahub.secondary_class_authors]
 ZillizCloudPipelineRetriever = "llama-index"
 
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
@@ -24,15 +26,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index managed zilliz integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-indices-managed-zilliz"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_indices_managed_zilliz-0.1.2/PKG-INFO` & `llama_index_indices_managed_zilliz-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: llama-index-indices-managed-zilliz
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index managed zilliz integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Managed Integration: Zilliz
```

