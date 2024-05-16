# Comparing `tmp/langchain_astradb-0.3.0.tar.gz` & `tmp/langchain_astradb-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_astradb-0.3.0.tar", max compression
+gzip compressed data, was "langchain_astradb-0.3.1.tar", max compression
```

## Comparing `langchain_astradb-0.3.0.tar` & `langchain_astradb-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-05-09 13:00:38.106036 langchain_astradb-0.3.0/LICENSE
--rw-r--r--   0        0        0     2058 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/README.md
--rw-r--r--   0        0        0      624 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/__init__.py
--rw-r--r--   0        0        0    20613 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/cache.py
--rw-r--r--   0        0        0     5344 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/chat_message_histories.py
--rw-r--r--   0        0        0     4549 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/document_loaders.py
--rw-r--r--   0        0        0        0 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/py.typed
--rw-r--r--   0        0        0     8833 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/storage.py
--rw-r--r--   0        0        0    14319 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/utils/astradb.py
--rw-r--r--   0        0        0     3165 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/utils/mmr.py
--rw-r--r--   0        0        0    62160 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/langchain_astradb/vectorstores.py
--rw-r--r--   0        0        0     2692 2024-05-09 13:00:38.110036 langchain_astradb-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2920 1970-01-01 00:00:00.000000 langchain_astradb-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2058 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/README.md
+-rw-r--r--   0        0        0      624 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/__init__.py
+-rw-r--r--   0        0        0    20613 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/cache.py
+-rw-r--r--   0        0        0     5344 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/chat_message_histories.py
+-rw-r--r--   0        0        0     4549 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/document_loaders.py
+-rw-r--r--   0        0        0        0 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/py.typed
+-rw-r--r--   0        0        0     8833 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/storage.py
+-rw-r--r--   0        0        0    14319 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/utils/astradb.py
+-rw-r--r--   0        0        0     3165 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/utils/mmr.py
+-rw-r--r--   0        0        0    62160 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/langchain_astradb/vectorstores.py
+-rw-r--r--   0        0        0     2888 2024-05-16 20:01:42.366827 langchain_astradb-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2918 1970-01-01 00:00:00.000000 langchain_astradb-0.3.1/PKG-INFO
```

### Comparing `langchain_astradb-0.3.0/LICENSE` & `langchain_astradb-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.0/README.md` & `langchain_astradb-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.0/langchain_astradb/__init__.py` & `langchain_astradb-0.3.1/langchain_astradb/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.0/langchain_astradb/cache.py` & `langchain_astradb-0.3.1/langchain_astradb/cache.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.0/langchain_astradb/chat_message_histories.py` & `langchain_astradb-0.3.1/langchain_astradb/chat_message_histories.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.0/langchain_astradb/document_loaders.py` & `langchain_astradb-0.3.1/langchain_astradb/document_loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.0/langchain_astradb/storage.py` & `langchain_astradb-0.3.1/langchain_astradb/storage.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.0/langchain_astradb/utils/astradb.py` & `langchain_astradb-0.3.1/langchain_astradb/utils/astradb.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.0/langchain_astradb/utils/mmr.py` & `langchain_astradb-0.3.1/langchain_astradb/utils/mmr.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.0/langchain_astradb/vectorstores.py` & `langchain_astradb-0.3.1/langchain_astradb/vectorstores.py`

 * *Files identical despite different names*

### Comparing `langchain_astradb-0.3.0/pyproject.toml` & `langchain_astradb-0.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 [tool.poetry]
 name = "langchain-astradb"
-version = "0.3.0"
+version = "0.3.1"
 description = "An integration package connecting Astra DB and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-datastax"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain-datastax/tree/main/libs/astradb"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.31"
+langchain-core = ">=0.1.31,<0.3"
 astrapy = "^1"
 numpy = "^1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 pytest-dotenv = "^0.5.2"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
-langchain = "^0.1.9"
-langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
+langchain = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/langchain" }
+langchain-text-splitters = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/text-splitters" }
+langchain-core = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core" }
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
-langchain = "^0.1.9"
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^0.991"
-langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
+langchain-core = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core" }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
+langchain-core = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core" }
 
 [tool.ruff]
 select = [
   "E", # pycodestyle
   "F", # pyflakes
   "I", # isort
 ]
```

### Comparing `langchain_astradb-0.3.0/PKG-INFO` & `langchain_astradb-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-astradb
-Version: 0.3.0
+Version: 0.3.1
 Summary: An integration package connecting Astra DB and LangChain
 Home-page: https://github.com/langchain-ai/langchain-datastax
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: astrapy (>=1,<2)
-Requires-Dist: langchain-core (>=0.1.31,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.31,<0.3)
 Requires-Dist: numpy (>=1,<2)
 Project-URL: Repository, https://github.com/langchain-ai/langchain-datastax
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-datastax/tree/main/libs/astradb
 Description-Content-Type: text/markdown
 
 # langchain-astradb
```

