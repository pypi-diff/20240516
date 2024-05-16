# Comparing `tmp/llama_index_vector_stores_azureaisearch-0.1.4.tar.gz` & `tmp/llama_index_vector_stores_azureaisearch-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_azureaisearch-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_azureaisearch-0.1.5.tar", max compression
```

## Comparing `llama_index_vector_stores_azureaisearch-0.1.4.tar` & `llama_index_vector_stores_azureaisearch-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       56 2024-02-13 13:53:01.989925 llama_index_vector_stores_azureaisearch-0.1.4/README.md
--rw-r--r--   0        0        0      306 2024-02-20 18:45:10.342718 llama_index_vector_stores_azureaisearch-0.1.4/llama_index/vector_stores/azureaisearch/__init__.py
--rw-r--r--   0        0        0    30271 2024-02-20 18:45:10.342890 llama_index_vector_stores_azureaisearch-0.1.4/llama_index/vector_stores/azureaisearch/base.py
--rw-r--r--   0        0        0     1636 2024-02-21 23:08:55.476108 llama_index_vector_stores_azureaisearch-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 llama_index_vector_stores_azureaisearch-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       56 2024-05-03 00:43:18.177806 llama_index_vector_stores_azureaisearch-0.1.5/README.md
+-rw-r--r--   0        0        0      306 2024-05-03 00:43:18.177806 llama_index_vector_stores_azureaisearch-0.1.5/llama_index/vector_stores/azureaisearch/__init__.py
+-rw-r--r--   0        0        0    32218 2024-05-03 00:43:18.177806 llama_index_vector_stores_azureaisearch-0.1.5/llama_index/vector_stores/azureaisearch/base.py
+-rw-r--r--   0        0        0     1565 2024-05-03 00:43:18.177806 llama_index_vector_stores_azureaisearch-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      692 1970-01-01 00:00:00.000000 llama_index_vector_stores_azureaisearch-0.1.5/PKG-INFO
```

### Comparing `llama_index_vector_stores_azureaisearch-0.1.4/llama_index/vector_stores/azureaisearch/base.py` & `llama_index_vector_stores_azureaisearch-0.1.5/llama_index/vector_stores/azureaisearch/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Azure AI Search vector store."""
+
 import enum
 import json
 import logging
 from enum import auto
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union, cast
 from llama_index.core.bridge.pydantic import PrivateAttr
 from llama_index.core.schema import BaseNode, MetadataMode, TextNode
@@ -46,14 +47,65 @@
 
     NO_VALIDATION = auto()
     VALIDATE_INDEX = auto()
     CREATE_IF_NOT_EXISTS = auto()
 
 
 class AzureAISearchVectorStore(BasePydanticVectorStore):
+    """Azure AI Search vector store.
+
+    Examples:
+        `pip install llama-index-vector-stores-azureaisearch`
+
+        ```python
+        from azure.core.credentials import AzureKeyCredential
+        from azure.search.documents import SearchClient
+        from azure.search.documents.indexes import SearchIndexClient
+        from llama_index.vector_stores.azureaisearch import AzureAISearchVectorStore
+        from llama_index.vector_stores.azureaisearch import IndexManagement, MetadataIndexFieldType
+
+        # Azure AI Search setup
+        search_service_api_key = "YOUR-AZURE-SEARCH-SERVICE-ADMIN-KEY"
+        search_service_endpoint = "YOUR-AZURE-SEARCH-SERVICE-ENDPOINT"
+        search_service_api_version = "2023-11-01"
+        credential = AzureKeyCredential(search_service_api_key)
+
+        # Index name to use
+        index_name = "llamaindex-vector-demo"
+
+        # Use index client to demonstrate creating an index
+        index_client = SearchIndexClient(
+            endpoint=search_service_endpoint,
+            credential=credential,
+        )
+
+        metadata_fields = {
+            "author": "author",
+            "theme": ("topic", MetadataIndexFieldType.STRING),
+            "director": "director",
+        }
+
+        # Creating an Azure AI Search Vector Store
+        vector_store = AzureAISearchVectorStore(
+            search_or_index_client=index_client,
+            filterable_metadata_field_keys=metadata_fields,
+            index_name=index_name,
+            index_management=IndexManagement.CREATE_IF_NOT_EXISTS,
+            id_field_key="id",
+            chunk_field_key="chunk",
+            embedding_field_key="embedding",
+            embedding_dimensionality=1536,
+            metadata_string_field_key="metadata",
+            doc_id_field_key="doc_id",
+            language_analyzer="en.lucene",
+            vector_algorithm_type="exhaustiveKnn",
+        )
+        ```
+    """
+
     stores_text: bool = True
     flat_metadata: bool = True
 
     _index_client: SearchIndexClient = PrivateAttr()
     _search_client: SearchClient = PrivateAttr()
     _embedding_dimensionality: int = PrivateAttr()
     _language_analyzer: str = PrivateAttr()
@@ -541,15 +593,15 @@
                     "provide entry in 'filterable_metadata_field_keys' for this "
                     "vector store"
                 )
 
             index_field = metadata_mapping[0]
 
             if len(odata_filter) > 0:
-                odata_filter.append(" and ")
+                odata_filter.append(" {metadata_filters.condition.value} ")
             if isinstance(f.value, str):
                 escaped_value = "".join([("''" if s == "'" else s) for s in f.value])
                 odata_filter.append(f"{index_field} eq '{escaped_value}'")
             else:
                 odata_filter.append(f"{index_field} eq {f.value}")
 
         odata_expr = "".join(odata_filter)
```

### Comparing `llama_index_vector_stores_azureaisearch-0.1.4/pyproject.toml` & `llama_index_vector_stores_azureaisearch-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -10,31 +10,29 @@
 [tool.llamahub]
 contains_example = false
 import_path = "llama_index.vector_stores.azureaisearch"
 
 [tool.llamahub.class_authors]
 AzureAISearchVectorStore = "llama-index"
 CognitiveSearchVectorStore = "llama-index"
-IndexManagement = "llama-index"
-MetadataIndexFieldType = "llama-index"
 
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores azureaisearch integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-azureaisearch"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 azure-search-documents = "^11.4.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_vector_stores_azureaisearch-0.1.4/PKG-INFO` & `llama_index_vector_stores_azureaisearch-0.1.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-azureaisearch
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index vector_stores azureaisearch integration
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
 Requires-Dist: azure-search-documents (>=11.4.0,<12.0.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Vector_Stores Integration: Azure AI Search
```

