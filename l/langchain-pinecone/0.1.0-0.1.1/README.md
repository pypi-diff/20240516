# Comparing `tmp/langchain_pinecone-0.1.0.tar.gz` & `tmp/langchain_pinecone-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_pinecone-0.1.0.tar", max compression
+gzip compressed data, was "langchain_pinecone-0.1.1.tar", max compression
```

## Comparing `langchain_pinecone-0.1.0.tar` & `langchain_pinecone-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1072 2024-04-08 20:07:28.340824 langchain_pinecone-0.1.0/LICENSE
--rw-r--r--   0        0        0      554 2024-04-08 20:07:28.340824 langchain_pinecone-0.1.0/README.md
--rw-r--r--   0        0        0      132 2024-04-08 20:07:28.340824 langchain_pinecone-0.1.0/langchain_pinecone/__init__.py
--rw-r--r--   0        0        0     2821 2024-04-08 20:07:28.340824 langchain_pinecone-0.1.0/langchain_pinecone/_utilities.py
--rw-r--r--   0        0        0        0 2024-04-08 20:07:28.340824 langchain_pinecone-0.1.0/langchain_pinecone/py.typed
--rw-r--r--   0        0        0    18142 2024-04-08 20:07:28.340824 langchain_pinecone-0.1.0/langchain_pinecone/vectorstores.py
--rw-r--r--   0        0        0     2616 2024-04-08 20:07:28.340824 langchain_pinecone-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1419 1970-01-01 00:00:00.000000 langchain_pinecone-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-16 02:32:11.684090 langchain_pinecone-0.1.1/LICENSE
+-rw-r--r--   0        0        0      554 2024-05-16 02:32:11.684090 langchain_pinecone-0.1.1/README.md
+-rw-r--r--   0        0        0      132 2024-05-16 02:32:11.684090 langchain_pinecone-0.1.1/langchain_pinecone/__init__.py
+-rw-r--r--   0        0        0     2821 2024-05-16 02:32:11.684090 langchain_pinecone-0.1.1/langchain_pinecone/_utilities.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:32:11.684090 langchain_pinecone-0.1.1/langchain_pinecone/py.typed
+-rw-r--r--   0        0        0    18142 2024-05-16 02:32:11.684090 langchain_pinecone-0.1.1/langchain_pinecone/vectorstores.py
+-rw-r--r--   0        0        0     2651 2024-05-16 02:32:11.684090 langchain_pinecone-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1417 1970-01-01 00:00:00.000000 langchain_pinecone-0.1.1/PKG-INFO
```

### Comparing `langchain_pinecone-0.1.0/LICENSE` & `langchain_pinecone-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_pinecone-0.1.0/README.md` & `langchain_pinecone-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_pinecone-0.1.0/langchain_pinecone/_utilities.py` & `langchain_pinecone-0.1.1/langchain_pinecone/_utilities.py`

 * *Files identical despite different names*

### Comparing `langchain_pinecone-0.1.0/langchain_pinecone/vectorstores.py` & `langchain_pinecone-0.1.1/langchain_pinecone/vectorstores.py`

 * *Files 0% similar despite different names*

```diff
@@ -490,12 +490,12 @@
             self._index.delete(filter=filter, namespace=namespace, **kwargs)
         else:
             raise ValueError("Either ids, delete_all, or filter must be provided.")
 
         return None
 
 
-@deprecated(since="0.0.3", removal="0.2.0", alternative="PineconeVectorStore")
+@deprecated(since="0.0.3", removal="0.3.0", alternative="PineconeVectorStore")
 class Pinecone(PineconeVectorStore):
     """Deprecated. Use PineconeVectorStore instead."""
 
     pass
```

### Comparing `langchain_pinecone-0.1.0/pyproject.toml` & `langchain_pinecone-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "langchain-pinecone"
-version = "0.1.0"
+version = "0.1.1"
 description = "An integration package connecting Pinecone and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/pinecone"
 
 [tool.poetry.dependencies]
 # <3.13 is due to restriction in pinecone-client package
 python = ">=3.8.1,<3.13"
-langchain-core = "^0.1.40"
+langchain-core = ">=0.1.52,<0.3"
 pinecone-client = "^3.2.2"
 numpy = "^1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
@@ -35,15 +35,15 @@
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
-langchain-openai = ">=0.0.3,<0.1"
+langchain-openai = { path = "../openai", develop = true }
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
@@ -53,15 +53,15 @@
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 langchain-core = { path = "../../core", develop = true }
 
-[tool.ruff]
+[tool.ruff.lint]
 select = [
   "E",    # pycodestyle
   "F",    # pyflakes
   "I",    # isort
   "T201", # print
 
 ]
```

### Comparing `langchain_pinecone-0.1.0/PKG-INFO` & `langchain_pinecone-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: langchain-pinecone
-Version: 0.1.0
+Version: 0.1.1
 Summary: An integration package connecting Pinecone and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain-core (>=0.1.40,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.52,<0.3)
 Requires-Dist: numpy (>=1,<2)
 Requires-Dist: pinecone-client (>=3.2.2,<4.0.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/pinecone
 Description-Content-Type: text/markdown
 
 # langchain-pinecone
```

