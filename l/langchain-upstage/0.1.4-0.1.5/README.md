# Comparing `tmp/langchain_upstage-0.1.4.tar.gz` & `tmp/langchain_upstage-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_upstage-0.1.4.tar", max compression
+gzip compressed data, was "langchain_upstage-0.1.5.tar", max compression
```

## Comparing `langchain_upstage-0.1.4.tar` & `langchain_upstage-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1072 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/LICENSE
--rw-r--r--   0        0        0      979 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/README.md
--rw-r--r--   0        0        0      567 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/langchain_upstage/__init__.py
--rw-r--r--   0        0        0     3848 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/langchain_upstage/chat_models.py
--rw-r--r--   0        0        0     9097 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/langchain_upstage/embeddings.py
--rw-r--r--   0        0        0     7105 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/langchain_upstage/layout_analysis.py
--rw-r--r--   0        0        0    12942 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/langchain_upstage/layout_analysis_parsers.py
--rw-r--r--   0        0        0        0 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/langchain_upstage/py.typed
--rw-r--r--   0        0        0     4323 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/langchain_upstage/tools/groundedness_check.py
--rw-r--r--   0        0        0     2732 2024-05-08 22:06:08.512033 langchain_upstage-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 langchain_upstage-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/LICENSE
+-rw-r--r--   0        0        0      979 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/README.md
+-rw-r--r--   0        0        0      567 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/langchain_upstage/__init__.py
+-rw-r--r--   0        0        0     3848 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/langchain_upstage/chat_models.py
+-rw-r--r--   0        0        0     9556 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/langchain_upstage/embeddings.py
+-rw-r--r--   0        0        0     8945 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/langchain_upstage/layout_analysis.py
+-rw-r--r--   0        0        0    13042 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/langchain_upstage/layout_analysis_parsers.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/langchain_upstage/py.typed
+-rw-r--r--   0        0        0     4323 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/langchain_upstage/tools/groundedness_check.py
+-rw-r--r--   0        0        0     2738 2024-05-16 02:51:35.663231 langchain_upstage-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1892 1970-01-01 00:00:00.000000 langchain_upstage-0.1.5/PKG-INFO
```

### Comparing `langchain_upstage-0.1.4/LICENSE` & `langchain_upstage-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.4/README.md` & `langchain_upstage-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.4/langchain_upstage/__init__.py` & `langchain_upstage-0.1.5/langchain_upstage/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.4/langchain_upstage/chat_models.py` & `langchain_upstage-0.1.5/langchain_upstage/chat_models.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.4/langchain_upstage/embeddings.py` & `langchain_upstage-0.1.5/langchain_upstage/embeddings.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,17 @@
     convert_to_secret_str,
     get_from_dict_or_env,
     get_pydantic_field_names,
 )
 
 logger = logging.getLogger(__name__)
 
+DEFAULT_EMBED_BATCH_SIZE = 10
+MAX_EMBED_BATCH_SIZE = 100
+
 
 class UpstageEmbeddings(BaseModel, Embeddings):
     """UpstageEmbeddings embedding model.
 
     To use, set the environment variable `UPSTAGE_API_KEY` with your API key or
     pass it as a named parameter to the constructor.
 
@@ -44,17 +47,17 @@
             from langchain_upstage import UpstageEmbeddings
 
             model = UpstageEmbeddings()
     """
 
     client: Any = Field(default=None, exclude=True)  #: :meta private:
     async_client: Any = Field(default=None, exclude=True)  #: :meta private:
-    model: str = "solar-1-mini-embedding"
+    model: str = Field(...)
     """Embeddings model name to use. Do not add suffixes like `-query` and `-passage`.
-    Instead, use 'solar-1-mini-embedding' for example.
+    Instead, use 'solar-embedding-1-large' for example.
     """
     dimensions: Optional[int] = None
     """The number of dimensions the resulting output embeddings should have.
     
     Not yet supported. 
     """
     upstage_api_key: Optional[SecretStr] = Field(default=None, alias="api_key")
@@ -64,14 +67,15 @@
     )
     """Endpoint URL to use."""
     embedding_ctx_length: int = 4096
     """The maximum number of tokens to embed at once.
     
     Not yet supported.
     """
+    embed_batch_size: int = DEFAULT_EMBED_BATCH_SIZE
     allowed_special: Union[Literal["all"], Set[str]] = set()
     """Not yet supported."""
     disallowed_special: Union[Literal["all"], Set[str], Sequence[str]] = "all"
     """Not yet supported."""
     chunk_size: int = 1000
     """Maximum number of texts to embed in each batch.
     
@@ -189,24 +193,27 @@
 
         Args:
             texts: The list of texts to embed.
 
         Returns:
             List of embeddings, one for each text.
         """
-        embeddings = []
+        assert (
+            self.embed_batch_size <= MAX_EMBED_BATCH_SIZE
+        ), f"The embed_batch_size should not be larger than {MAX_EMBED_BATCH_SIZE}."
         params = self._invocation_params
         params["model"] = params["model"] + "-passage"
+        embeddings = []
 
-        for text in texts:
-            response = self.client.create(input=text, **params)
+        batch_size = min(self.embed_batch_size, len(texts))
+        for i in range(0, len(texts), batch_size):
+            batch = texts[i : i + batch_size]
+            data = self.client.create(input=batch, **params).data
+            embeddings.extend([r.embedding for r in data])
 
-            if not isinstance(response, dict):
-                response = response.model_dump()
-                embeddings.extend([i["embedding"] for i in response["data"]])
         return embeddings
 
     def embed_query(self, text: str) -> List[float]:
         """Embed query text using query model.
 
         Args:
             text: The text to embed.
@@ -228,24 +235,26 @@
 
         Args:
             texts: The list of texts to embed.
 
         Returns:
             List of embeddings, one for each text.
         """
-        embeddings = []
+        assert (
+            self.embed_batch_size <= MAX_EMBED_BATCH_SIZE
+        ), f"The embed_batch_size should not be larger than {MAX_EMBED_BATCH_SIZE}."
         params = self._invocation_params
         params["model"] = params["model"] + "-passage"
+        embeddings = []
 
-        for text in texts:
-            response = await self.async_client.create(input=text, **params)
-
-            if not isinstance(response, dict):
-                response = response.model_dump()
-                embeddings.extend([i["embedding"] for i in response["data"]])
+        batch_size = min(self.embed_batch_size, len(texts))
+        for i in range(0, len(texts), batch_size):
+            batch = texts[i : i + batch_size]
+            response = await self.async_client.create(input=batch, **params)
+            embeddings.extend([r.embedding for r in response.data])
         return embeddings
 
     async def aembed_query(self, text: str) -> List[float]:
         """Asynchronous Embed query text using query model.
 
         Args:
             text: The text to embed.
```

### Comparing `langchain_upstage-0.1.4/langchain_upstage/layout_analysis.py` & `langchain_upstage-0.1.5/langchain_upstage/layout_analysis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import warnings
 from pathlib import Path
-from typing import Iterator, List, Literal, Optional, Union
+from typing import Any, Dict, Iterator, List, Literal, Optional, Union
 
 from langchain_core.document_loaders import BaseLoader, Blob
 from langchain_core.documents import Document
 
 from .layout_analysis_parsers import UpstageLayoutAnalysisParser
 
 DEFAULT_PAGE_BATCH_SIZE = 10
@@ -200,7 +200,49 @@
                 self.api_key,
                 split=self.split,
                 output_type=self.output_type,
                 use_ocr=self.use_ocr,
                 exclude=self.exclude,
             )
             yield from parser.lazy_parse(blob)
+
+    def merge_and_split(
+        self, documents: List[Document], splitter: Optional[object] = None
+    ) -> List[Document]:
+        """
+        Merges the page content and metadata of multiple documents into a single
+        document, or splits the documents using a custom splitter.
+
+        Args:
+            documents (list): A list of Document objects to be merged and split.
+            splitter (object, optional): An optional splitter object that implements the
+                `split_documents` method. If provided, the documents will be split using
+                this splitter. Defaults to None, in which case the documents are merged.
+
+        Returns:
+            list: A list of Document objects. If no splitter is provided, a single
+            Document object is returned with the merged content and combined metadata.
+            If a splitter is provided, the documents are split and a list of Document
+            objects is returned.
+
+        Raises:
+            AssertionError: If a splitter is provided but it does not implement the
+            `split_documents` method.
+        """
+        if splitter is None:
+            merged_content = " ".join([doc.page_content for doc in documents])
+
+            metadatas: Dict[str, Any] = dict()
+            for _meta in [doc.metadata for doc in documents]:
+                for key, value in _meta.items():
+                    if key in metadatas:
+                        metadatas[key].append(value)
+                    else:
+                        metadatas[key] = [value]
+
+            return [Document(page_content=merged_content, metadata=metadatas)]
+        else:
+            assert hasattr(
+                splitter, "split_documents"
+            ), "splitter must implement split_documents method"
+
+            return splitter.split_documents(documents)
```

### Comparing `langchain_upstage-0.1.4/langchain_upstage/layout_analysis_parsers.py` & `langchain_upstage-0.1.5/langchain_upstage/layout_analysis_parsers.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,14 +242,16 @@
         return Document(
             page_content=(parse_output(elements, self.output_type)),
             metadata={
                 "page": elements["page"],
                 "id": elements["id"],
                 "type": self.output_type,
                 "split": self.split,
+                "bbox": elements["bounding_box"],
+                "category": elements["category"],
             },
         )
 
     def _page_document(self, elements: List) -> List[Document]:
         """
         Combines elements with the same page number into a single Document object.
```

### Comparing `langchain_upstage-0.1.4/langchain_upstage/tools/groundedness_check.py` & `langchain_upstage-0.1.5/langchain_upstage/tools/groundedness_check.py`

 * *Files identical despite different names*

### Comparing `langchain_upstage-0.1.4/pyproject.toml` & `langchain_upstage-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-upstage"
-version = "0.1.4"
+version = "0.1.5"
 description = "An integration package connecting Upstage and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/upstage"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.44"
+langchain-core = ">=0.1.52,<0.3"
 langchain-openai = "^0.1.3"
 pymupdf = "^1.24.1"
 requests = "^2.31.0"
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `langchain_upstage-0.1.4/PKG-INFO` & `langchain_upstage-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: langchain-upstage
-Version: 0.1.4
+Version: 0.1.5
 Summary: An integration package connecting Upstage and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain-core (>=0.1.44,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.52,<0.3)
 Requires-Dist: langchain-openai (>=0.1.3,<0.2.0)
 Requires-Dist: pymupdf (>=1.24.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/upstage
 Description-Content-Type: text/markdown
```

