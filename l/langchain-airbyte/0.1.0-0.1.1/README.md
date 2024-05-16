# Comparing `tmp/langchain_airbyte-0.1.0.tar.gz` & `tmp/langchain_airbyte-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_airbyte-0.1.0.tar", max compression
+gzip compressed data, was "langchain_airbyte-0.1.1.tar", max compression
```

## Comparing `langchain_airbyte-0.1.0.tar` & `langchain_airbyte-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2024-02-28 03:55:19.644741 langchain_airbyte-0.1.0/LICENSE
--rw-r--r--   0        0        0      593 2024-02-28 03:55:19.644741 langchain_airbyte-0.1.0/README.md
--rw-r--r--   0        0        0       90 2024-02-28 03:55:19.644741 langchain_airbyte-0.1.0/langchain_airbyte/__init__.py
--rw-r--r--   0        0        0     3812 2024-02-28 03:55:19.644741 langchain_airbyte-0.1.0/langchain_airbyte/document_loaders.py
--rw-r--r--   0        0        0        0 2024-02-28 03:55:19.644741 langchain_airbyte-0.1.0/langchain_airbyte/py.typed
--rw-r--r--   0        0        0     2166 2024-02-28 03:55:19.644741 langchain_airbyte-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 langchain_airbyte-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-16 02:29:05.793868 langchain_airbyte-0.1.1/LICENSE
+-rw-r--r--   0        0        0      593 2024-05-16 02:29:05.793868 langchain_airbyte-0.1.1/README.md
+-rw-r--r--   0        0        0       90 2024-05-16 02:29:05.793868 langchain_airbyte-0.1.1/langchain_airbyte/__init__.py
+-rw-r--r--   0        0        0     4115 2024-05-16 02:29:05.793868 langchain_airbyte-0.1.1/langchain_airbyte/document_loaders.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:29:05.793868 langchain_airbyte-0.1.1/langchain_airbyte/py.typed
+-rw-r--r--   0        0        0     2309 2024-05-16 02:29:05.793868 langchain_airbyte-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 langchain_airbyte-0.1.1/PKG-INFO
```

### Comparing `langchain_airbyte-0.1.0/LICENSE` & `langchain_airbyte-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_airbyte-0.1.0/README.md` & `langchain_airbyte-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_airbyte-0.1.0/langchain_airbyte/document_loaders.py` & `langchain_airbyte-0.1.1/langchain_airbyte/document_loaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 import airbyte as ab
 from langchain_core.documents import Document
 from langchain_core.prompts import PromptTemplate
 from langchain_core.runnables import run_in_executor
 from langchain_core.vectorstores import VectorStore
 
 if TYPE_CHECKING:
-    from langchain.text_splitter import TextSplitter
-    from langchain_core.documents import Document
+    from langchain_text_splitters import TextSplitter
 
 VST = TypeVar("VST", bound=VectorStore)
 
 
 class AirbyteLoader:
     """Airbyte Document Loader.
 
@@ -68,17 +67,24 @@
         Args:
             text_splitter: TextSplitter instance to use for splitting documents.
               Defaults to RecursiveCharacterTextSplitter.
 
         Returns:
             List of Documents.
         """
-        from langchain.text_splitter import RecursiveCharacterTextSplitter
 
         if text_splitter is None:
+            try:
+                from langchain_text_splitters import RecursiveCharacterTextSplitter
+            except ImportError as e:
+                raise ImportError(
+                    "Unable to import from langchain_text_splitters. Please specify "
+                    "text_splitter or install langchain_text_splitters with "
+                    "`pip install -U langchain-text-splitters`."
+                ) from e
             _text_splitter: TextSplitter = RecursiveCharacterTextSplitter()
         else:
             _text_splitter = text_splitter
         docs = self.lazy_load()
         return _text_splitter.split_documents(docs)
 
     def lazy_load(self) -> Iterator[Document]:
```

### Comparing `langchain_airbyte-0.1.0/pyproject.toml` & `langchain_airbyte-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "langchain-airbyte"
-version = "0.1.0"
+version = "0.1.1"
 description = "An integration package connecting Airbyte and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/airbyte"
 
 [tool.poetry.dependencies]
-python = "^3.10"
-langchain-core = "^0.1.5"
-airbyte = "^0.7.0"
+python = "^3.9"
+langchain-core = ">=0.1.5,<0.3"
+airbyte = "^0.7.3"
+pydantic = ">=1.10.8,<2"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.3"
 pytest-asyncio = "^0.23.2"
@@ -39,15 +40,16 @@
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.8"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^1.7.1"
 langchain-core = { path = "../../core", develop = true }
-langchain = "^0.1.9"
+langchain-text-splitters = { path = "../../text-splitters", develop = true }
+langchain = { path = "../../langchain", develop = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 langchain-core = { path = "../../core", develop = true }
```

### Comparing `langchain_airbyte-0.1.0/PKG-INFO` & `langchain_airbyte-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-airbyte
-Version: 0.1.0
+Version: 0.1.1
 Summary: An integration package connecting Airbyte and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: airbyte (>=0.7.0,<0.8.0)
-Requires-Dist: langchain-core (>=0.1.5,<0.2.0)
+Requires-Dist: airbyte (>=0.7.3,<0.8.0)
+Requires-Dist: langchain-core (>=0.1.5,<0.3)
+Requires-Dist: pydantic (>=1.10.8,<2)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/airbyte
 Description-Content-Type: text/markdown
 
 # langchain-airbyte
 
 This package contains the LangChain integration with Airbyte
```

