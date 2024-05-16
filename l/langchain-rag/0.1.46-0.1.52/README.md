# Comparing `tmp/langchain_rag-0.1.46.tar.gz` & `tmp/langchain_rag-0.1.52.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_rag-0.1.46.tar", max compression
+gzip compressed data, was "langchain_rag-0.1.52.tar", max compression
```

## Comparing `langchain_rag-0.1.46.tar` & `langchain_rag-0.1.52.tar`

### file list

```diff
@@ -1,26 +1,24 @@
--rw-r--r--   0        0        0    11357 2023-10-19 05:47:38.233379 langchain_rag-0.1.46/LICENSE.txt
--rw-r--r--   0        0        0     2155 2024-02-07 08:38:30.870089 langchain_rag-0.1.46/README.md
--rw-r--r--   0        0        0        0 2023-10-23 07:07:51.650962 langchain_rag-0.1.46/langchain_rag/__init__.py
--rw-r--r--   0        0        0      698 2024-04-23 11:15:14.817186 langchain_rag-0.1.46/langchain_rag/document_transformers/__init__.py
--rw-r--r--   0        0        0     1096 2024-01-29 11:57:32.041286 langchain_rag-0.1.46/langchain_rag/document_transformers/copy_transformer.py
--rw-r--r--   0        0        0     2859 2024-04-23 11:15:14.817186 langchain_rag-0.1.46/langchain_rag/document_transformers/document_transform_pipeline.py
--rw-r--r--   0        0        0     6134 2024-04-23 11:15:14.817186 langchain_rag-0.1.46/langchain_rag/document_transformers/document_transformers.py
--rw-r--r--   0        0        0     3978 2024-01-29 11:07:27.844752 langchain_rag-0.1.46/langchain_rag/document_transformers/generate_questions.py
--rw-r--r--   0        0        0     9254 2024-04-23 11:17:36.261006 langchain_rag-0.1.46/langchain_rag/document_transformers/runnable_document_transformer.py
--rw-r--r--   0        0        0     4740 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/document_transformers/summarize_and_questions_transformer.py
--rw-r--r--   0        0        0     3257 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/document_transformers/summarize_transformer.py
--rw-r--r--   0        0        0       89 2024-01-24 09:40:10.848052 langchain_rag-0.1.46/langchain_rag/indexes/__init__.py
--rw-r--r--   0        0        0     3637 2024-01-24 07:30:49.261495 langchain_rag-0.1.46/langchain_rag/indexes/memory_recordmanager.py
--rw-r--r--   0        0        0        0 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/patch_langchain/__init__.py
--rw-r--r--   0        0        0       81 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/patch_langchain/storage/__init__.py
--rw-r--r--   0        0        0     4047 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/patch_langchain/storage/encoder_backed.py
--rw-r--r--   0        0        0        0 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/patch_langchain_community/__init__.py
--rw-r--r--   0        0        0        0 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/patch_langchain_community/indexes/__init__.py
--rw-r--r--   0        0        0    21023 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/patch_langchain_community/indexes/_sql_record_manager.py
--rw-r--r--   0        0        0       59 2023-11-02 16:16:50.944534 langchain_rag-0.1.46/langchain_rag/storage/__init__.py
--rw-r--r--   0        0        0     8277 2024-04-23 11:15:14.821186 langchain_rag-0.1.46/langchain_rag/storage/sql_docstore.py
--rw-r--r--   0        0        0      148 2023-11-02 16:16:50.948534 langchain_rag-0.1.46/langchain_rag/vectorstores/__init__.py
--rw-r--r--   0        0        0    35370 2024-04-25 08:50:07.798706 langchain_rag-0.1.46/langchain_rag/vectorstores/rag_vectorstore.py
--rw-r--r--   0        0        0     6658 2024-01-24 07:30:49.265495 langchain_rag-0.1.46/langchain_rag/vectorstores/wrapper_vectorstore.py
--rw-r--r--   0        0        0     3816 2024-04-23 11:15:14.825186 langchain_rag-0.1.46/pyproject.toml
--rw-r--r--   0        0        0     2940 1970-01-01 00:00:00.000000 langchain_rag-0.1.46/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-19 05:47:38.233379 langchain_rag-0.1.52/LICENSE.txt
+-rw-r--r--   0        0        0     2155 2024-02-07 08:38:30.870089 langchain_rag-0.1.52/README.md
+-rw-r--r--   0        0        0        0 2023-10-23 07:07:51.650962 langchain_rag-0.1.52/langchain_rag/__init__.py
+-rw-r--r--   0        0        0      698 2024-04-23 11:15:14.817186 langchain_rag-0.1.52/langchain_rag/document_transformers/__init__.py
+-rw-r--r--   0        0        0     1096 2024-01-29 11:57:32.041286 langchain_rag-0.1.52/langchain_rag/document_transformers/copy_transformer.py
+-rw-r--r--   0        0        0     2859 2024-04-23 11:15:14.817186 langchain_rag-0.1.52/langchain_rag/document_transformers/document_transform_pipeline.py
+-rw-r--r--   0        0        0     6134 2024-04-23 11:15:14.817186 langchain_rag-0.1.52/langchain_rag/document_transformers/document_transformers.py
+-rw-r--r--   0        0        0     3978 2024-01-29 11:07:27.844752 langchain_rag-0.1.52/langchain_rag/document_transformers/generate_questions.py
+-rw-r--r--   0        0        0     9254 2024-04-23 11:17:36.261006 langchain_rag-0.1.52/langchain_rag/document_transformers/runnable_document_transformer.py
+-rw-r--r--   0        0        0     4740 2024-04-23 11:15:14.821186 langchain_rag-0.1.52/langchain_rag/document_transformers/summarize_and_questions_transformer.py
+-rw-r--r--   0        0        0     3257 2024-04-23 11:15:14.821186 langchain_rag-0.1.52/langchain_rag/document_transformers/summarize_transformer.py
+-rw-r--r--   0        0        0       89 2024-01-24 09:40:10.848052 langchain_rag-0.1.52/langchain_rag/indexes/__init__.py
+-rw-r--r--   0        0        0     3637 2024-01-24 07:30:49.261495 langchain_rag-0.1.52/langchain_rag/indexes/memory_recordmanager.py
+-rw-r--r--   0        0        0        0 2024-04-23 11:15:14.821186 langchain_rag-0.1.52/langchain_rag/patch_langchain_community/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 11:15:14.821186 langchain_rag-0.1.52/langchain_rag/patch_langchain_community/indexes/__init__.py
+-rw-r--r--   0        0        0    21023 2024-05-07 08:27:10.339308 langchain_rag-0.1.52/langchain_rag/patch_langchain_community/indexes/_sql_record_manager.py
+-rw-r--r--   0        0        0       59 2023-11-02 16:16:50.944534 langchain_rag-0.1.52/langchain_rag/storage/__init__.py
+-rw-r--r--   0        0        0     8371 2024-05-16 08:17:57.407069 langchain_rag-0.1.52/langchain_rag/storage/sql_docstore.py
+-rw-r--r--   0        0        0      247 2024-05-16 08:17:55.931065 langchain_rag-0.1.52/langchain_rag/test_p.py
+-rw-r--r--   0        0        0      148 2023-11-02 16:16:50.948534 langchain_rag-0.1.52/langchain_rag/vectorstores/__init__.py
+-rw-r--r--   0        0        0    36578 2024-05-16 08:18:29.515150 langchain_rag-0.1.52/langchain_rag/vectorstores/rag_vectorstore.py
+-rw-r--r--   0        0        0     6658 2024-01-24 07:30:49.265495 langchain_rag-0.1.52/langchain_rag/vectorstores/wrapper_vectorstore.py
+-rw-r--r--   0        0        0     3816 2024-05-15 14:59:30.039235 langchain_rag-0.1.52/pyproject.toml
+-rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 langchain_rag-0.1.52/PKG-INFO
```

### Comparing `langchain_rag-0.1.46/LICENSE.txt` & `langchain_rag-0.1.52/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.46/README.md` & `langchain_rag-0.1.52/README.md`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.46/langchain_rag/document_transformers/__init__.py` & `langchain_rag-0.1.52/langchain_rag/document_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.46/langchain_rag/document_transformers/copy_transformer.py` & `langchain_rag-0.1.52/langchain_rag/document_transformers/copy_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.46/langchain_rag/document_transformers/document_transform_pipeline.py` & `langchain_rag-0.1.52/langchain_rag/document_transformers/document_transform_pipeline.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.46/langchain_rag/document_transformers/document_transformers.py` & `langchain_rag-0.1.52/langchain_rag/document_transformers/document_transformers.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.46/langchain_rag/document_transformers/generate_questions.py` & `langchain_rag-0.1.52/langchain_rag/document_transformers/generate_questions.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.46/langchain_rag/document_transformers/runnable_document_transformer.py` & `langchain_rag-0.1.52/langchain_rag/document_transformers/runnable_document_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.46/langchain_rag/document_transformers/summarize_and_questions_transformer.py` & `langchain_rag-0.1.52/langchain_rag/document_transformers/summarize_and_questions_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.46/langchain_rag/document_transformers/summarize_transformer.py` & `langchain_rag-0.1.52/langchain_rag/document_transformers/summarize_transformer.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.46/langchain_rag/indexes/memory_recordmanager.py` & `langchain_rag-0.1.52/langchain_rag/indexes/memory_recordmanager.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.46/langchain_rag/patch_langchain_community/indexes/_sql_record_manager.py` & `langchain_rag-0.1.52/langchain_rag/patch_langchain_community/indexes/_sql_record_manager.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.46/langchain_rag/storage/sql_docstore.py` & `langchain_rag-0.1.52/langchain_rag/storage/sql_docstore.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     create_engine,
     delete,
     select,
 )
 from sqlalchemy.ext.asyncio import (
     AsyncEngine,
     AsyncSession,
+    async_scoped_session,
     async_sessionmaker,
     create_async_engine,
 )
 from sqlalchemy.orm import (
     Mapped,
     Session,
     declarative_base,
@@ -236,21 +237,23 @@
                 yield str(v.key)
             await session.close()
 
     @contextlib.contextmanager
     def _make_session(self) -> Generator[Session, None, None]:
         """Create a session and close it after use."""
 
-        if isinstance(self.session_factory, async_sessionmaker):
+        if isinstance(self.session_factory, async_sessionmaker | async_scoped_session):
             raise AssertionError("This method is not supported for async engines.")
 
         yield self.session_factory()
 
     @contextlib.asynccontextmanager
     async def _amake_session(self) -> AsyncGenerator[AsyncSession, None]:
         """Create a session and close it after use."""
 
-        if not isinstance(self.session_factory, async_sessionmaker):
+        if not isinstance(
+            self.session_factory, async_sessionmaker | async_scoped_session
+        ):
             raise AssertionError("This method is not supported for sync engines.")
 
         async with self.session_factory() as session:
             yield session
```

### Comparing `langchain_rag-0.1.46/langchain_rag/vectorstores/rag_vectorstore.py` & `langchain_rag-0.1.52/langchain_rag/vectorstores/rag_vectorstore.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 import asyncio
 import concurrent
 import hashlib
 import logging
 import uuid
-from copy import copy
+from copy import copy, deepcopy
+
+# from langchain.storage import EncoderBackedStore
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Optional,
     Sequence,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
+from langchain.storage import EncoderBackedStore
 from langchain_core.documents import BaseDocumentTransformer, Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.pydantic_v1 import BaseModel, Extra, Field
 from langchain_core.stores import BaseStore
 from langchain_core.vectorstores import VectorStore, VectorStoreRetriever
 from sqlalchemy import (
-    Connection,
     Engine,
     create_engine,
 )
 from sqlalchemy.ext.asyncio import (
     AsyncEngine,
     create_async_engine,
 )
-from sqlalchemy.orm import scoped_session, sessionmaker
 
 from .wrapper_vectorstore import WrapperVectorStore
 
 logger = logging.getLogger(__name__)
 
 # %%
 VST = TypeVar("VST", bound="VectorStore")
@@ -368,14 +369,15 @@
             ids = cast(List[str], ids)
             mset_values: List[Tuple[str, List[str]]] = []
             for parent_id, doc in zip(ids, documents):
                 mset_values.append((parent_id, chunk_ids_for_doc[parent_id]))
             self.docstore.mset(mset_values)
             return ids
         else:
+            self.docstore.mset(full_chunk_docs)
             return chunk_ids
 
     async def aadd_documents(
         self,
         documents: List[Document],
         *,
         ids: Optional[List[str]] = None,
@@ -534,14 +536,15 @@
             self.docstore.mdelete(chunk_by_doc_ids)
             for chunk_doc in chunk_docs:
                 if chunk_doc:
                     transformed_ids.update(
                         chunk_doc.metadata[self.child_ids_key].split(",")
                     )
         if transformed_ids:
+            self.docstore.mdelete(ids)
             self.vectorstore.delete(ids=list(transformed_ids))
         elif self.parent_transformer:
             return self.vectorstore.delete(ids=chunk_by_doc_ids)
         elif not self.parent_transformer and self.chunk_transformer:
             return len(transformed_ids) != 0
         else:
             return self.vectorstore.delete(ids=ids)
@@ -576,14 +579,15 @@
             await self.docstore.amdelete(chunk_by_doc_ids)
             for chunk_doc in chunk_docs:
                 if chunk_doc:
                     transformed_ids.update(
                         chunk_doc.metadata[self.child_ids_key].split(",")
                     )
         if transformed_ids:
+            await self.docstore.amdelete(ids)
             await self.vectorstore.adelete(ids=list(transformed_ids))
         elif self.parent_transformer:
             return await self.vectorstore.adelete(ids=chunk_by_doc_ids)
         elif not self.parent_transformer and self.chunk_transformer:
             return len(transformed_ids) != 0
         else:
             return await self.vectorstore.adelete(ids=ids)
@@ -783,31 +787,27 @@
             {
                 "record_manager": record_manager,
                 "vector_store": vectorstore,
                 "source_id_key": source_id_key,
             },
         )
 
-    def session_maker(self, bind: Engine | Connection) -> scoped_session:
-        return scoped_session(sessionmaker(bind=bind))
-
     @staticmethod
     def from_vs_in_sql(
         vectorstore: VectorStore,
         *,
         engine: Union[None, Engine, AsyncEngine] = None,
         engine_kwargs: Optional[Dict[str, Any]] = None,
         db_url: Optional[str] = None,
         use_async: Optional[bool] = None,
         namespace: str = "rag_vectorstore",
         chunk_transformer: Optional[BaseDocumentTransformer] = None,
         parent_transformer: Optional[BaseDocumentTransformer] = None,
         **kwargs: Any,
     ) -> Tuple["RAGVectorStore", Dict[str, Any]]:
-        from langchain_rag.patch_langchain.storage import EncoderBackedStore
         from langchain_rag.patch_langchain_community.indexes._sql_record_manager import (  # noqa: E501
             SQLRecordManager,
         )
 
         if isinstance(engine, AsyncEngine):
             assert (
                 use_async is not False
@@ -873,39 +873,73 @@
             {
                 "record_manager": record_manager,
                 "vector_store": vectorstore,
                 "source_id_key": kwargs.get("source_id_key", "source"),
             },
         )
 
+    def __deepcopy__(self, memodict: Optional[dict[int, Any]] = {}) -> "RAGVectorStore":
+        new_rag_vectorstore = copy(self)
+        new_rag_vectorstore.docstore = copy(self.docstore)
+        new_rag_vectorstore.vectorstore = copy(self.vectorstore)
+        return new_rag_vectorstore
+
+    @property
+    def session_maker(self) -> Any:
+        if hasattr(self.docstore, "store"):
+            return self.docstore.store.session_factory
+        if hasattr(self.vectorstore, "session_factory"):
+            return self.vectorstore.session_factory
+        if hasattr(self.vectorstore, "session_maker"):
+            return self.vectorstore.session_maker
+        assert False, "Non session_maker detected"
+
+    def __setattr__(self, key: str, val: Any) -> None:
+        if key == "session_maker":
+            self._set_session_maker(val)
+        else:
+            super().__setattr__(key, val)
+
+    def _set_session_maker(self, session_maker: Any) -> None:
+        # Manage docstore
+        store = self.docstore
+        if hasattr(self.docstore, "store"):
+            store = self.docstore.store
+        if hasattr(store, "session_factory"):
+            store.session_factory = session_maker
+        elif hasattr(store, "session_maker"):
+            store.session_maker = session_maker
+        else:
+            logger.warning(
+                "The docstore has no session_factory or session_maker attribute"
+            )
+
+        # Manage vectorstore
+        if hasattr(self.vectorstore, "session_factory"):
+            self.vectorstore.session_factory = session_maker
+        elif hasattr(self.vectorstore, "session_maker"):
+            self.vectorstore.session_maker = session_maker
+        else:
+            logger.warning(
+                "The vectorstore has no session_factory or session_maker attribute"
+            )
+
     @staticmethod
     def copy_with_session_maker(
         session_maker: Any,
         rag_vectorstore: "RAGVectorStore",
         index_kwargs: Dict[str, Any],
     ) -> Tuple["RAGVectorStore", Dict[str, Any]]:
         """Duplicate the RAGVectorStore and index_kwargs with a new session_maker."""
         assert isinstance(rag_vectorstore, RAGVectorStore)
-        new_rag_vectorstore = copy(rag_vectorstore)
-        new_rag_vectorstore.docstore = copy(rag_vectorstore.docstore)
-        new_rag_vectorstore.vectorstore = copy(rag_vectorstore.vectorstore)
-
-        if hasattr(new_rag_vectorstore.docstore, "session_factory"):
-            new_rag_vectorstore.docstore.session_factory = session_maker
-
-        if hasattr(new_rag_vectorstore.vectorstore, "session_factory"):
-            new_rag_vectorstore.vectorstore.session_factory = session_maker
-        elif hasattr(new_rag_vectorstore.vectorstore, "session_maker"):
-            new_rag_vectorstore.vectorstore.session_maker = session_maker
-        else:
-            logger.warning(
-                "The vectorstore has no session_factory or session_maker attribute"
-            )
+        new_rag_vectorstore = deepcopy(rag_vectorstore)
+        new_rag_vectorstore.session_maker = session_maker  # type: ignore
 
         new_record_manager = copy(index_kwargs["record_manager"])
+        # new_record_manager = index_kwargs["record_manager"]
         new_record_manager.session_factory = session_maker
 
         return new_rag_vectorstore, {
             "record_manager": new_record_manager,
             "source_id_key": index_kwargs["source_id_key"],
             "vector_store": new_rag_vectorstore,
         }
```

### Comparing `langchain_rag-0.1.46/langchain_rag/vectorstores/wrapper_vectorstore.py` & `langchain_rag-0.1.52/langchain_rag/vectorstores/wrapper_vectorstore.py`

 * *Files identical despite different names*

### Comparing `langchain_rag-0.1.46/pyproject.toml` & `langchain_rag-0.1.52/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 packages = [
   { include = "langchain_rag" },
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-#langchain-core = ">=0.1.17"
-#langchain-community = ">=0.0.16"
-langchain = ">=0.1.4"
+#langchain-core = ">=0.1.52"
+#langchain-community = ">=0.0.38"
+langchain = "^0.1.20"
 
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 playwright = "^1.28.0"
```

### Comparing `langchain_rag-0.1.46/PKG-INFO` & `langchain_rag-0.1.52/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-rag
-Version: 0.1.46
+Version: 0.1.52
 Summary: This is a temporary project while I wait for my langchain [pull-request](https://github.com/langchain-ai/langchain/pull/7278) to be validated.
 Home-page: https://www.github.com/pprados/langchain-rag
 License: Apache 2.0
 Author: Philippe PRADOS
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain (>=0.1.4)
+Requires-Dist: langchain (>=0.1.20,<0.2.0)
 Project-URL: Repository, https://www.github.com/pprados/langchain-rag
 Description-Content-Type: text/markdown
 
 Langchain-RAG
 =============
 
 [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/pprados/langchain-rag?quickstart=1)
```

