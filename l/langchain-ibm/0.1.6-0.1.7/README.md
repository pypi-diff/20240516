# Comparing `tmp/langchain_ibm-0.1.6.tar.gz` & `tmp/langchain_ibm-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_ibm-0.1.6.tar", max compression
+gzip compressed data, was "langchain_ibm-0.1.7.tar", max compression
```

## Comparing `langchain_ibm-0.1.6.tar` & `langchain_ibm-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-05-08 22:05:52.641588 langchain_ibm-0.1.6/LICENSE
--rw-r--r--   0        0        0     4395 2024-05-08 22:05:52.641588 langchain_ibm-0.1.6/README.md
--rw-r--r--   0        0        0      144 2024-05-08 22:05:52.641588 langchain_ibm-0.1.6/langchain_ibm/__init__.py
--rw-r--r--   0        0        0     6702 2024-05-08 22:05:52.641588 langchain_ibm-0.1.6/langchain_ibm/embeddings.py
--rw-r--r--   0        0        0    16171 2024-05-08 22:05:52.641588 langchain_ibm-0.1.6/langchain_ibm/llms.py
--rw-r--r--   0        0        0        0 2024-05-08 22:05:52.641588 langchain_ibm-0.1.6/langchain_ibm/py.typed
--rw-r--r--   0        0        0     2564 2024-05-08 22:05:52.641588 langchain_ibm-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 langchain_ibm-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-16 02:10:38.726112 langchain_ibm-0.1.7/LICENSE
+-rw-r--r--   0        0        0     4395 2024-05-16 02:10:38.726112 langchain_ibm-0.1.7/README.md
+-rw-r--r--   0        0        0      144 2024-05-16 02:10:38.726112 langchain_ibm-0.1.7/langchain_ibm/__init__.py
+-rw-r--r--   0        0        0     6702 2024-05-16 02:10:38.726112 langchain_ibm-0.1.7/langchain_ibm/embeddings.py
+-rw-r--r--   0        0        0    16171 2024-05-16 02:10:38.726112 langchain_ibm-0.1.7/langchain_ibm/llms.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:10:38.726112 langchain_ibm-0.1.7/langchain_ibm/py.typed
+-rw-r--r--   0        0        0     2570 2024-05-16 02:10:38.726112 langchain_ibm-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     5183 1970-01-01 00:00:00.000000 langchain_ibm-0.1.7/PKG-INFO
```

### Comparing `langchain_ibm-0.1.6/LICENSE` & `langchain_ibm-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_ibm-0.1.6/README.md` & `langchain_ibm-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `langchain_ibm-0.1.6/langchain_ibm/embeddings.py` & `langchain_ibm-0.1.7/langchain_ibm/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_ibm-0.1.6/langchain_ibm/llms.py` & `langchain_ibm-0.1.7/langchain_ibm/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_ibm-0.1.6/pyproject.toml` & `langchain_ibm-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-ibm"
-version = "0.1.6"
+version = "0.1.7"
 description = "An integration package connecting IBM watsonx.ai and LangChain"
 authors = ["IBM"]
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/ibm"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-langchain-core = "^0.1.50"
+langchain-core = ">=0.1.50,<0.3"
 ibm-watsonx-ai = "^1.0.1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
```

### Comparing `langchain_ibm-0.1.6/PKG-INFO` & `langchain_ibm-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-ibm
-Version: 0.1.6
+Version: 0.1.7
 Summary: An integration package connecting IBM watsonx.ai and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Author: IBM
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ibm-watsonx-ai (>=1.0.1,<2.0.0)
-Requires-Dist: langchain-core (>=0.1.50,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.50,<0.3)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/ibm
 Description-Content-Type: text/markdown
 
 # langchain-ibm
 
 This package provides the integration between LangChain and IBM watsonx.ai through the `ibm-watsonx-ai` SDK.
```

