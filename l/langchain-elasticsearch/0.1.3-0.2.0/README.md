# Comparing `tmp/langchain_elasticsearch-0.1.3.tar.gz` & `tmp/langchain_elasticsearch-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_elasticsearch-0.1.3.tar", max compression
+gzip compressed data, was "langchain_elasticsearch-0.2.0.tar", max compression
```

## Comparing `langchain_elasticsearch-0.1.3.tar` & `langchain_elasticsearch-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-04-26 09:50:55.686820 langchain_elasticsearch-0.1.3/LICENSE
--rw-r--r--   0        0        0     5805 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/README.md
--rw-r--r--   0        0        0      705 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/__init__.py
--rw-r--r--   0        0        0     4075 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/_utilities.py
--rw-r--r--   0        0        0     7748 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/cache.py
--rw-r--r--   0        0        0     5417 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/chat_history.py
--rw-r--r--   0        0        0     1094 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/client.py
--rw-r--r--   0        0        0     7862 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/embeddings.py
--rw-r--r--   0        0        0        0 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/py.typed
--rw-r--r--   0        0        0     4764 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/retrievers.py
--rw-r--r--   0        0        0    49930 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/langchain_elasticsearch/vectorstores.py
--rw-r--r--   0        0        0     2618 2024-04-26 09:50:55.690820 langchain_elasticsearch-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6691 1970-01-01 00:00:00.000000 langchain_elasticsearch-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-16 03:06:25.616031 langchain_elasticsearch-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5805 2024-05-16 03:06:25.616031 langchain_elasticsearch-0.2.0/README.md
+-rw-r--r--   0        0        0     1185 2024-05-16 03:06:25.616031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/__init__.py
+-rw-r--r--   0        0        0     1393 2024-05-16 03:06:25.616031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/_utilities.py
+-rw-r--r--   0        0        0     7748 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/cache.py
+-rw-r--r--   0        0        0     5417 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/chat_history.py
+-rw-r--r--   0        0        0     1094 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/client.py
+-rw-r--r--   0        0        0     9253 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/embeddings.py
+-rw-r--r--   0        0        0        0 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/py.typed
+-rw-r--r--   0        0        0     4764 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/retrievers.py
+-rw-r--r--   0        0        0    44233 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/vectorstores.py
+-rw-r--r--   0        0        0     2925 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6681 1970-01-01 00:00:00.000000 langchain_elasticsearch-0.2.0/PKG-INFO
```

### Comparing `langchain_elasticsearch-0.1.3/LICENSE` & `langchain_elasticsearch-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.3/README.md` & `langchain_elasticsearch-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.3/langchain_elasticsearch/__init__.py` & `langchain_elasticsearch-0.2.0/langchain_elasticsearch/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,40 @@
+from elasticsearch.helpers.vectorstore import (
+    BM25Strategy,
+    DenseVectorScriptScoreStrategy,
+    DenseVectorStrategy,
+    DistanceMetric,
+    RetrievalStrategy,
+    SparseVectorStrategy,
+)
+
 from langchain_elasticsearch.cache import ElasticsearchCache
 from langchain_elasticsearch.chat_history import ElasticsearchChatMessageHistory
 from langchain_elasticsearch.embeddings import ElasticsearchEmbeddings
 from langchain_elasticsearch.retrievers import ElasticsearchRetriever
 from langchain_elasticsearch.vectorstores import (
     ApproxRetrievalStrategy,
+    BM25RetrievalStrategy,
     ElasticsearchStore,
     ExactRetrievalStrategy,
     SparseRetrievalStrategy,
 )
 
 __all__ = [
-    "ApproxRetrievalStrategy",
     "ElasticsearchCache",
     "ElasticsearchChatMessageHistory",
     "ElasticsearchEmbeddings",
     "ElasticsearchRetriever",
     "ElasticsearchStore",
+    # retrieval strategies
+    "BM25Strategy",
+    "DenseVectorScriptScoreStrategy",
+    "DenseVectorStrategy",
+    "DistanceMetric",
+    "RetrievalStrategy",
+    "SparseVectorStrategy",
+    # deprecated retrieval strategies
+    "ApproxRetrievalStrategy",
+    "BM25RetrievalStrategy",
     "ExactRetrievalStrategy",
     "SparseRetrievalStrategy",
 ]
```

### Comparing `langchain_elasticsearch-0.1.3/langchain_elasticsearch/cache.py` & `langchain_elasticsearch-0.2.0/langchain_elasticsearch/cache.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.3/langchain_elasticsearch/chat_history.py` & `langchain_elasticsearch-0.2.0/langchain_elasticsearch/chat_history.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.3/langchain_elasticsearch/client.py` & `langchain_elasticsearch-0.2.0/langchain_elasticsearch/client.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.3/langchain_elasticsearch/embeddings.py` & `langchain_elasticsearch-0.2.0/langchain_elasticsearch/embeddings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, List, Optional
 
 from elasticsearch import Elasticsearch
+from elasticsearch.helpers.vectorstore import EmbeddingService
 from langchain_core.embeddings import Embeddings
 from langchain_core.utils import get_from_env
 
 if TYPE_CHECKING:
     from elasticsearch.client import MlClient
 
 
@@ -202,7 +203,49 @@
         Args:
             text (str): The query text to generate an embedding for.
 
         Returns:
             List[float]: The embedding for the input query text.
         """
         return self._embedding_func([text])[0]
+
+
+class EmbeddingServiceAdapter(EmbeddingService):
+    """
+    Adapter for LangChain Embeddings to support the EmbeddingService interface from
+    elasticsearch.helpers.vectorstore.
+    """
+
+    def __init__(self, langchain_embeddings: Embeddings):
+        self._langchain_embeddings = langchain_embeddings
+
+    def __eq__(self, other):  # type: ignore[no-untyped-def]
+        if isinstance(other, self.__class__):
+            return self.__dict__ == other.__dict__
+        else:
+            return False
+
+    def embed_documents(self, texts: List[str]) -> List[List[float]]:
+        """
+        Generate embeddings for a list of documents.
+
+        Args:
+            texts (List[str]): A list of document text strings to generate embeddings
+                for.
+
+        Returns:
+            List[List[float]]: A list of embeddings, one for each document in the input
+                list.
+        """
+        return self._langchain_embeddings.embed_documents(texts)
+
+    def embed_query(self, text: str) -> List[float]:
+        """
+        Generate an embedding for a single query text.
+
+        Args:
+            text (str): The query text to generate an embedding for.
+
+        Returns:
+            List[float]: The embedding for the input query text.
+        """
+        return self._langchain_embeddings.embed_query(text)
```

### Comparing `langchain_elasticsearch-0.1.3/langchain_elasticsearch/retrievers.py` & `langchain_elasticsearch-0.2.0/langchain_elasticsearch/retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.1.3/langchain_elasticsearch/vectorstores.py` & `langchain_elasticsearch-0.2.0/langchain_elasticsearch/vectorstores.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,50 @@
 import logging
-import uuid
 from abc import ABC, abstractmethod
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
     List,
     Literal,
     Optional,
     Tuple,
     Union,
 )
 
-import numpy as np
 from elasticsearch import Elasticsearch
-from elasticsearch.helpers import BulkIndexError, bulk
+from elasticsearch.helpers.vectorstore import (
+    BM25Strategy,
+    DenseVectorScriptScoreStrategy,
+    DenseVectorStrategy,
+    DistanceMetric,
+    RetrievalStrategy,
+    SparseVectorStrategy,
+)
+from elasticsearch.helpers.vectorstore import (
+    VectorStore as EVectorStore,
+)
+from langchain_core._api.deprecation import deprecated
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.vectorstores import VectorStore
 
 from langchain_elasticsearch._utilities import (
     DistanceStrategy,
-    maximal_marginal_relevance,
     model_must_be_deployed,
-    with_user_agent_header,
+    user_agent,
 )
+from langchain_elasticsearch.client import create_elasticsearch_client
+from langchain_elasticsearch.embeddings import EmbeddingServiceAdapter
 
 logger = logging.getLogger(__name__)
 
 
+@deprecated("0.2.0", alternative="RetrievalStrategy", pending=True)
 class BaseRetrievalStrategy(ABC):
     """Base class for `Elasticsearch` retrieval strategies."""
 
     @abstractmethod
     def query(
         self,
         query_vector: Union[List[float], None],
@@ -111,14 +122,15 @@
         Returns:
             bool: Whether or not the strategy requires inference
             to be performed on the text before it is added to the index.
         """
         return True
 
 
+@deprecated("0.2.0", alternative="DenseVectorStrategy", pending=True)
 class ApproxRetrievalStrategy(BaseRetrievalStrategy):
     """Approximate retrieval strategy using the `HNSW` algorithm."""
 
     def __init__(
         self,
         query_model_id: Optional[str] = None,
         hybrid: Optional[bool] = False,
@@ -238,14 +250,15 @@
                         "similarity": similarityAlgo,
                     },
                 }
             }
         }
 
 
+@deprecated("0.2.0", alternative="DenseVectorScriptScoreStrategy", pending=True)
 class ExactRetrievalStrategy(BaseRetrievalStrategy):
     """Exact retrieval strategy using the `script_score` query."""
 
     def query(
         self,
         query_vector: Union[List[float], None],
         query: Union[str, None],
@@ -306,14 +319,15 @@
                         "index": False,
                     },
                 }
             }
         }
 
 
+@deprecated("0.2.0", alternative="SparseVectorStrategy", pending=True)
 class SparseRetrievalStrategy(BaseRetrievalStrategy):
     """Sparse retrieval strategy using the `text_expansion` processor."""
 
     def __init__(self, model_id: Optional[str] = None):
         self.model_id = model_id or ".elser_model_1"
 
     def query(
@@ -390,14 +404,15 @@
             "settings": {"default_pipeline": self._get_pipeline_name()},
         }
 
     def require_inference(self) -> bool:
         return False
 
 
+@deprecated("0.2.0", alternative="BM25Strategy", pending=True)
 class BM25RetrievalStrategy(BaseRetrievalStrategy):
     """Retrieval strategy using the native BM25 algorithm of Elasticsearch."""
 
     def __init__(self, k1: Union[float, None] = None, b: Union[float, None] = None):
         self.k1 = k1
         self.b = b
 
@@ -460,24 +475,95 @@
 
         return {"mappings": mappings, "settings": settings}
 
     def require_inference(self) -> bool:
         return False
 
 
+def _convert_retrieval_strategy(
+    langchain_strategy: BaseRetrievalStrategy,
+    distance: Optional[DistanceStrategy] = None,
+) -> RetrievalStrategy:
+    if isinstance(langchain_strategy, ApproxRetrievalStrategy):
+        if distance is None:
+            raise ValueError(
+                "ApproxRetrievalStrategy requires a distance strategy to be provided."
+            )
+        return DenseVectorStrategy(
+            distance=DistanceMetric[distance],
+            model_id=langchain_strategy.query_model_id,
+            hybrid=(
+                False
+                if langchain_strategy.hybrid is None
+                else langchain_strategy.hybrid
+            ),
+            rrf=False if langchain_strategy.rrf is None else langchain_strategy.rrf,
+        )
+    elif isinstance(langchain_strategy, ExactRetrievalStrategy):
+        if distance is None:
+            raise ValueError(
+                "ExactRetrievalStrategy requires a distance strategy to be provided."
+            )
+        return DenseVectorScriptScoreStrategy(distance=DistanceMetric[distance])
+    elif isinstance(langchain_strategy, SparseRetrievalStrategy):
+        return SparseVectorStrategy(langchain_strategy.model_id)
+    elif isinstance(langchain_strategy, BM25RetrievalStrategy):
+        return BM25Strategy(k1=langchain_strategy.k1, b=langchain_strategy.b)
+    else:
+        raise TypeError(
+            f"Strategy {langchain_strategy} not supported. To provide a "
+            f"custom strategy, please subclass {RetrievalStrategy}."
+        )
+
+
+def _hits_to_docs_scores(
+    hits: List[Dict[str, Any]],
+    content_field: str,
+    fields: Optional[List[str]] = None,
+    doc_builder: Optional[Callable[[Dict], Document]] = None,
+) -> List[Tuple[Document, float]]:
+    if fields is None:
+        fields = []
+
+    documents = []
+
+    def default_doc_builder(hit: Dict) -> Document:
+        return Document(
+            page_content=hit["_source"].get(content_field, ""),
+            metadata=hit["_source"].get("metadata", {}),
+        )
+
+    doc_builder = doc_builder or default_doc_builder
+
+    for hit in hits:
+        for field in fields:
+            if "metadata" not in hit["_source"]:
+                hit["_source"]["metadata"] = {}
+            if field in hit["_source"] and field not in [
+                "metadata",
+                content_field,
+            ]:
+                hit["_source"]["metadata"][field] = hit["_source"][field]
+
+        doc = doc_builder(hit)
+        documents.append((doc, hit["_score"]))
+
+    return documents
+
+
 class ElasticsearchStore(VectorStore):
     """`Elasticsearch` vector store.
 
     Example:
         .. code-block:: python
 
             from langchain_elasticsearch.vectorstores import ElasticsearchStore
             from langchain_openai import OpenAIEmbeddings
 
-            vectorstore = ElasticsearchStore(
+            store = ElasticsearchStore(
                 embedding=OpenAIEmbeddings(),
                 index_name="langchain-demo",
                 es_url="http://localhost:9200"
             )
 
     Args:
         index_name: Name of the Elasticsearch index to create.
@@ -504,15 +590,15 @@
 
     Example:
         .. code-block:: python
 
             from langchain_elasticsearch.vectorstores import ElasticsearchStore
             from langchain_openai import OpenAIEmbeddings
 
-            vectorstore = ElasticsearchStore(
+            store = ElasticsearchStore(
                 embedding=OpenAIEmbeddings(),
                 index_name="langchain-demo",
                 es_cloud_id="<cloud_id>"
                 es_user="elastic",
                 es_password="<password>"
             )
 
@@ -525,15 +611,15 @@
             from langchain_elasticsearch.vectorstores import ElasticsearchStore
             from langchain_openai import OpenAIEmbeddings
 
             from elasticsearch import Elasticsearch
 
             es_connection = Elasticsearch("http://localhost:9200")
 
-            vectorstore = ElasticsearchStore(
+            store = ElasticsearchStore(
                 embedding=OpenAIEmbeddings(),
                 index_name="langchain-demo",
                 es_connection=es_connection
             )
 
     ElasticsearchStore by default uses the ApproxRetrievalStrategy, which uses the
     HNSW algorithm to perform approximate nearest neighbor search. This is the
@@ -544,15 +630,15 @@
 
     Example:
         .. code-block:: python
 
             from langchain_elasticsearch.vectorstores import ElasticsearchStore
             from langchain_openai import OpenAIEmbeddings
 
-            vectorstore = ElasticsearchStore(
+            store = ElasticsearchStore(
                 embedding=OpenAIEmbeddings(),
                 index_name="langchain-demo",
                 es_url="http://localhost:9200",
                 strategy=ElasticsearchStore.ExactRetrievalStrategy()
             )
 
     Both strategies require that you know the similarity metric you want to use
@@ -562,29 +648,29 @@
     Example:
         .. code-block:: python
 
             from langchain_elasticsearch.vectorstores import ElasticsearchStore
             from langchain_openai import OpenAIEmbeddings
             from langchain_community.vectorstores.utils import DistanceStrategy
 
-            vectorstore = ElasticsearchStore(
+            store = ElasticsearchStore(
                 "langchain-demo",
                 embedding=OpenAIEmbeddings(),
                 es_url="http://localhost:9200",
                 distance_strategy="DOT_PRODUCT"
             )
 
     """
 
     def __init__(
         self,
         index_name: str,
         *,
         embedding: Optional[Embeddings] = None,
-        es_connection: Optional["Elasticsearch"] = None,
+        es_connection: Optional[Elasticsearch] = None,
         es_url: Optional[str] = None,
         es_cloud_id: Optional[str] = None,
         es_user: Optional[str] = None,
         es_api_key: Optional[str] = None,
         es_password: Optional[str] = None,
         vector_query_field: str = "vector",
         query_field: str = "text",
@@ -592,125 +678,130 @@
             Literal[
                 DistanceStrategy.COSINE,
                 DistanceStrategy.DOT_PRODUCT,
                 DistanceStrategy.EUCLIDEAN_DISTANCE,
                 DistanceStrategy.MAX_INNER_PRODUCT,
             ]
         ] = None,
-        strategy: BaseRetrievalStrategy = ApproxRetrievalStrategy(),
+        strategy: Union[
+            BaseRetrievalStrategy, RetrievalStrategy
+        ] = ApproxRetrievalStrategy(),
         es_params: Optional[Dict[str, Any]] = None,
     ):
-        self.embedding = embedding
-        self.index_name = index_name
-        self.query_field = query_field
-        self.vector_query_field = vector_query_field
-        self.distance_strategy = (
-            DistanceStrategy.COSINE
-            if distance_strategy is None
-            else DistanceStrategy[distance_strategy]
-        )
-        self.strategy = strategy
+        if isinstance(strategy, BaseRetrievalStrategy):
+            strategy = _convert_retrieval_strategy(
+                strategy, distance=distance_strategy or DistanceStrategy.COSINE
+            )
 
-        if es_connection is not None:
-            self.client = es_connection
-        elif es_url is not None or es_cloud_id is not None:
-            self.client = ElasticsearchStore.connect_to_elasticsearch(
-                es_url=es_url,
-                username=es_user,
-                password=es_password,
+        embedding_service = None
+        if embedding:
+            embedding_service = EmbeddingServiceAdapter(embedding)
+
+        if not es_connection:
+            es_connection = create_elasticsearch_client(
+                url=es_url,
                 cloud_id=es_cloud_id,
                 api_key=es_api_key,
-                es_params=es_params,
-            )
-        else:
-            raise ValueError(
-                """Either provide a pre-existing Elasticsearch connection, \
-                or valid credentials for creating a new connection."""
+                username=es_user,
+                password=es_password,
+                params=es_params,
             )
 
-        self.client = with_user_agent_header(self.client, "langchain-py-vs")
+        self._store = EVectorStore(
+            client=es_connection,
+            index=index_name,
+            retrieval_strategy=strategy,
+            embedding_service=embedding_service,
+            text_field=query_field,
+            vector_field=vector_query_field,
+            user_agent=user_agent("langchain-py-vs"),
+        )
+
+        self.embedding = embedding
+        self._embedding_service = embedding_service
+        self.query_field = query_field
+        self.vector_query_field = vector_query_field
+
+    def close(self) -> None:
+        self._store.close()
+
+    @property
+    def embeddings(self) -> Optional[Embeddings]:
+        return self.embedding
 
     @staticmethod
     def connect_to_elasticsearch(
         *,
         es_url: Optional[str] = None,
         cloud_id: Optional[str] = None,
         api_key: Optional[str] = None,
         username: Optional[str] = None,
         password: Optional[str] = None,
         es_params: Optional[Dict[str, Any]] = None,
-    ) -> "Elasticsearch":
-        if es_url and cloud_id:
-            raise ValueError(
-                "Both es_url and cloud_id are defined. Please provide only one."
-            )
-
-        connection_params: Dict[str, Any] = {}
-
-        if es_url:
-            connection_params["hosts"] = [es_url]
-        elif cloud_id:
-            connection_params["cloud_id"] = cloud_id
-        else:
-            raise ValueError("Please provide either elasticsearch_url or cloud_id.")
-
-        if api_key:
-            connection_params["api_key"] = api_key
-        elif username and password:
-            connection_params["basic_auth"] = (username, password)
-
-        if es_params is not None:
-            connection_params.update(es_params)
-
-        es_client = Elasticsearch(**connection_params)
-        try:
-            es_client.info()
-        except Exception as e:
-            logger.error(f"Error connecting to Elasticsearch: {e}")
-            raise e
-
-        return es_client
-
-    @property
-    def embeddings(self) -> Optional[Embeddings]:
-        return self.embedding
+    ) -> Elasticsearch:
+        return create_elasticsearch_client(
+            url=es_url,
+            cloud_id=cloud_id,
+            api_key=api_key,
+            username=username,
+            password=password,
+            params=es_params,
+        )
 
     def similarity_search(
         self,
         query: str,
         k: int = 4,
         fetch_k: int = 50,
         filter: Optional[List[dict]] = None,
+        *,
+        custom_query: Optional[
+            Callable[[Dict[str, Any], Optional[str]], Dict[str, Any]]
+        ] = None,
+        doc_builder: Optional[Callable[[Dict], Document]] = None,
         **kwargs: Any,
     ) -> List[Document]:
         """Return Elasticsearch documents most similar to query.
 
         Args:
             query: Text to look up documents similar to.
             k: Number of Documents to return. Defaults to 4.
             fetch_k (int): Number of Documents to fetch to pass to knn num_candidates.
             filter: Array of Elasticsearch filter clauses to apply to the query.
 
         Returns:
             List of Documents most similar to the query,
             in descending order of similarity.
         """
-
-        results = self._search(
-            query=query, k=k, fetch_k=fetch_k, filter=filter, **kwargs
+        hits = self._store.search(
+            query=query,
+            k=k,
+            num_candidates=fetch_k,
+            filter=filter,
+            custom_query=custom_query,
+        )
+        docs = _hits_to_docs_scores(
+            hits=hits,
+            content_field=self.query_field,
+            doc_builder=doc_builder,
         )
-        return [doc for doc, _ in results]
+        return [doc for doc, _score in docs]
 
     def max_marginal_relevance_search(
         self,
         query: str,
         k: int = 4,
         fetch_k: int = 20,
         lambda_mult: float = 0.5,
         fields: Optional[List[str]] = None,
+        *,
+        custom_query: Optional[
+            Callable[[Dict[str, Any], Optional[str]], Dict[str, Any]]
+        ] = None,
+        doc_builder: Optional[Callable[[Dict], Document]] = None,
         **kwargs: Any,
     ) -> List[Document]:
         """Return docs selected using the maximal marginal relevance.
 
         Maximal marginal relevance optimizes for similarity to query AND diversity
             among selected documents.
 
@@ -724,46 +815,38 @@
                 Defaults to 0.5.
             fields: Other fields to get from elasticsearch source. These fields
                 will be added to the document metadata.
 
         Returns:
             List[Document]: A list of Documents selected by maximal marginal relevance.
         """
-        if self.embedding is None:
-            raise ValueError("You must provide an embedding function to perform MMR")
-        remove_vector_query_field_from_metadata = True
-        if fields is None:
-            fields = [self.vector_query_field]
-        elif self.vector_query_field not in fields:
-            fields.append(self.vector_query_field)
-        else:
-            remove_vector_query_field_from_metadata = False
-
-        # Embed the query
-        query_embedding = self.embedding.embed_query(query)
+        if self._embedding_service is None:
+            raise ValueError(
+                "maximal marginal relevance search requires an embedding service."
+            )
 
-        # Fetch the initial documents
-        got_docs = self._search(
-            query_vector=query_embedding, k=fetch_k, fields=fields, **kwargs
+        hits = self._store.max_marginal_relevance_search(
+            embedding_service=self._embedding_service,
+            query=query,
+            vector_field=self.vector_query_field,
+            k=k,
+            num_candidates=fetch_k,
+            lambda_mult=lambda_mult,
+            fields=fields,
+            custom_query=custom_query,
         )
 
-        # Get the embeddings for the fetched documents
-        got_embeddings = [doc.metadata[self.vector_query_field] for doc, _ in got_docs]
-
-        # Select documents using maximal marginal relevance
-        selected_indices = maximal_marginal_relevance(
-            np.array(query_embedding), got_embeddings, lambda_mult=lambda_mult, k=k
+        docs_scores = _hits_to_docs_scores(
+            hits=hits,
+            content_field=self.query_field,
+            fields=fields,
+            doc_builder=doc_builder,
         )
-        selected_docs = [got_docs[i][0] for i in selected_indices]
-
-        if remove_vector_query_field_from_metadata:
-            for doc in selected_docs:
-                del doc.metadata[self.vector_query_field]
 
-        return selected_docs
+        return [doc for doc, _score in docs_scores]
 
     @staticmethod
     def _identity_fn(score: float) -> float:
         return score
 
     def _select_relevance_score_fn(self) -> Callable[[float], float]:
         """
@@ -777,372 +860,182 @@
         Vectorstores should define their own selection based method of relevance.
         """
         # All scores from Elasticsearch are already normalized similarities:
         # https://www.elastic.co/guide/en/elasticsearch/reference/current/dense-vector.html#dense-vector-params
         return self._identity_fn
 
     def similarity_search_with_score(
-        self, query: str, k: int = 4, filter: Optional[List[dict]] = None, **kwargs: Any
+        self,
+        query: str,
+        k: int = 4,
+        filter: Optional[List[dict]] = None,
+        *,
+        custom_query: Optional[
+            Callable[[Dict[str, Any], Optional[str]], Dict[str, Any]]
+        ] = None,
+        doc_builder: Optional[Callable[[Dict], Document]] = None,
+        **kwargs: Any,
     ) -> List[Tuple[Document, float]]:
         """Return Elasticsearch documents most similar to query, along with scores.
 
         Args:
             query: Text to look up documents similar to.
             k: Number of Documents to return. Defaults to 4.
             filter: Array of Elasticsearch filter clauses to apply to the query.
 
         Returns:
             List of Documents most similar to the query and score for each
         """
-        if isinstance(self.strategy, ApproxRetrievalStrategy) and self.strategy.hybrid:
+        if (
+            isinstance(self._store.retrieval_strategy, DenseVectorStrategy)
+            and self._store.retrieval_strategy.hybrid
+        ):
             raise ValueError("scores are currently not supported in hybrid mode")
 
-        return self._search(query=query, k=k, filter=filter, **kwargs)
+        hits = self._store.search(
+            query=query, k=k, filter=filter, custom_query=custom_query
+        )
+        return _hits_to_docs_scores(
+            hits=hits,
+            content_field=self.query_field,
+            doc_builder=doc_builder,
+        )
 
     def similarity_search_by_vector_with_relevance_scores(
         self,
         embedding: List[float],
         k: int = 4,
         filter: Optional[List[Dict]] = None,
+        *,
+        custom_query: Optional[
+            Callable[[Dict[str, Any], Optional[str]], Dict[str, Any]]
+        ] = None,
+        doc_builder: Optional[Callable[[Dict], Document]] = None,
         **kwargs: Any,
     ) -> List[Tuple[Document, float]]:
         """Return Elasticsearch documents most similar to query, along with scores.
 
         Args:
             embedding: Embedding to look up documents similar to.
             k: Number of Documents to return. Defaults to 4.
             filter: Array of Elasticsearch filter clauses to apply to the query.
 
         Returns:
             List of Documents most similar to the embedding and score for each
         """
-        if isinstance(self.strategy, ApproxRetrievalStrategy) and self.strategy.hybrid:
+        if (
+            isinstance(self._store.retrieval_strategy, DenseVectorStrategy)
+            and self._store.retrieval_strategy.hybrid
+        ):
             raise ValueError("scores are currently not supported in hybrid mode")
 
-        return self._search(query_vector=embedding, k=k, filter=filter, **kwargs)
-
-    def _search(
-        self,
-        query: Optional[str] = None,
-        k: int = 4,
-        query_vector: Union[List[float], None] = None,
-        fetch_k: int = 50,
-        fields: Optional[List[str]] = None,
-        filter: Optional[List[dict]] = None,
-        custom_query: Optional[Callable[[Dict, Union[str, None]], Dict]] = None,
-        doc_builder: Optional[Callable[[Dict], Document]] = None,
-        **kwargs: Any,
-    ) -> List[Tuple[Document, float]]:
-        """Return Elasticsearch documents most similar to query, along with scores.
-
-        Args:
-            query: Text to look up documents similar to.
-            k: Number of Documents to return. Defaults to 4.
-            query_vector: Embedding to look up documents similar to.
-            fetch_k: Number of candidates to fetch from each shard.
-                    Defaults to 50.
-            fields: List of fields to return from Elasticsearch.
-                    Defaults to only returning the text field.
-            filter: Array of Elasticsearch filter clauses to apply to the query.
-            custom_query: Function to modify the Elasticsearch
-                         query body before it is sent to Elasticsearch.
-
-        Returns:
-            List of Documents most similar to the query and score for each
-        """
-        if fields is None:
-            fields = []
-
-        if "metadata" not in fields:
-            fields.append("metadata")
-
-        if self.query_field not in fields:
-            fields.append(self.query_field)
-
-        if self.embedding and query is not None:
-            query_vector = self.embedding.embed_query(query)
-
-        query_body = self.strategy.query(
-            query_vector=query_vector,
-            query=query,
+        hits = self._store.search(
+            query=None,
+            query_vector=embedding,
             k=k,
-            fetch_k=fetch_k,
-            vector_query_field=self.vector_query_field,
-            text_field=self.query_field,
-            filter=filter or [],
-            similarity=self.distance_strategy,
+            filter=filter,
+            custom_query=custom_query,
         )
-
-        logger.debug(f"Query body: {query_body}")
-
-        if custom_query is not None:
-            query_body = custom_query(query_body, query)
-            logger.debug(f"Calling custom_query, Query body now: {query_body}")
-        # Perform the kNN search on the Elasticsearch index and return the results.
-        response = self.client.search(
-            index=self.index_name,
-            **query_body,
-            size=k,
-            source=True,
-            source_includes=fields,
+        return _hits_to_docs_scores(
+            hits=hits,
+            content_field=self.query_field,
+            doc_builder=doc_builder,
         )
 
-        def default_doc_builder(hit: Dict) -> Document:
-            return Document(
-                page_content=hit["_source"].get(self.query_field, ""),
-                metadata=hit["_source"].get("metadata", {}),
-            )
-
-        doc_builder = doc_builder or default_doc_builder
-
-        docs_and_scores = []
-        for hit in response["hits"]["hits"]:
-            for field in fields:
-                if "metadata" not in hit["_source"]:
-                    hit["_source"]["metadata"] = {}
-                if field in hit["_source"] and field not in [
-                    "metadata",
-                    self.query_field,
-                ]:
-                    hit["_source"]["metadata"][field] = hit["_source"][field]
-
-            docs_and_scores.append(
-                (
-                    doc_builder(hit),
-                    hit["_score"],
-                )
-            )
-        return docs_and_scores
-
     def delete(
         self,
         ids: Optional[List[str]] = None,
         refresh_indices: Optional[bool] = True,
         **kwargs: Any,
     ) -> Optional[bool]:
         """Delete documents from the Elasticsearch index.
 
         Args:
             ids: List of ids of documents to delete.
             refresh_indices: Whether to refresh the index
                             after deleting documents. Defaults to True.
         """
-        body = []
-
         if ids is None:
-            raise ValueError("ids must be provided.")
-
-        for _id in ids:
-            body.append({"_op_type": "delete", "_index": self.index_name, "_id": _id})
-
-        if len(body) > 0:
-            try:
-                bulk(self.client, body, refresh=refresh_indices, ignore_status=404)
-                logger.debug(f"Deleted {len(body)} texts from index")
-
-                return True
-            except BulkIndexError as e:
-                logger.error(f"Error deleting texts: {e}")
-                firstError = e.errors[0].get("index", {}).get("error", {})
-                logger.error(f"First error reason: {firstError.get('reason')}")
-                raise e
-
-        else:
-            logger.debug("No texts to delete from index")
-            return False
-
-    def _create_index_if_not_exists(
-        self, index_name: str, dims_length: Optional[int] = None
-    ) -> None:
-        """Create the Elasticsearch index if it doesn't already exist.
-
-        Args:
-            index_name: Name of the Elasticsearch index to create.
-            dims_length: Length of the embedding vectors.
-        """
-
-        if self.client.indices.exists(index=index_name):
-            logger.debug(f"Index {index_name} already exists. Skipping creation.")
-
-        else:
-            if dims_length is None and self.strategy.require_inference():
-                raise ValueError(
-                    "Cannot create index without specifying dims_length "
-                    "when the index doesn't already exist. We infer "
-                    "dims_length from the first embedding. Check that "
-                    "you have provided an embedding function."
-                )
-
-            self.strategy.before_index_setup(
-                client=self.client,
-                text_field=self.query_field,
-                vector_query_field=self.vector_query_field,
-            )
-
-            indexSettings = self.strategy.index(
-                vector_query_field=self.vector_query_field,
-                text_field=self.query_field,
-                dims_length=dims_length,
-                similarity=self.distance_strategy,
-            )
-            logger.debug(
-                f"Creating index {index_name} with mappings {indexSettings['mappings']}"
-            )
-            self.client.indices.create(index=index_name, **indexSettings)
-
-    def __add(
-        self,
-        texts: Iterable[str],
-        embeddings: Optional[List[List[float]]],
-        metadatas: Optional[List[Dict[Any, Any]]] = None,
-        ids: Optional[List[str]] = None,
-        refresh_indices: bool = True,
-        create_index_if_not_exists: bool = True,
-        bulk_kwargs: Optional[Dict] = None,
-        **kwargs: Any,
-    ) -> List[str]:
-        bulk_kwargs = bulk_kwargs or {}
-        ids = ids or [str(uuid.uuid4()) for _ in texts]
-        requests = []
-
-        if create_index_if_not_exists:
-            if embeddings:
-                dims_length = len(embeddings[0])
-            else:
-                dims_length = None
-
-            self._create_index_if_not_exists(
-                index_name=self.index_name, dims_length=dims_length
-            )
-
-        for i, text in enumerate(texts):
-            metadata = metadatas[i] if metadatas else {}
-
-            request = {
-                "_op_type": "index",
-                "_index": self.index_name,
-                self.query_field: text,
-                "metadata": metadata,
-                "_id": ids[i],
-            }
-            if embeddings:
-                request[self.vector_query_field] = embeddings[i]
-
-            requests.append(request)
-
-        if len(requests) > 0:
-            try:
-                success, failed = bulk(
-                    self.client,
-                    requests,
-                    stats_only=True,
-                    refresh=refresh_indices,
-                    **bulk_kwargs,
-                )
-                logger.debug(
-                    f"Added {success} and failed to add {failed} texts to index"
-                )
-
-                logger.debug(f"added texts {ids} to index")
-                return ids
-            except BulkIndexError as e:
-                logger.error(f"Error adding texts: {e}")
-                firstError = e.errors[0].get("index", {}).get("error", {})
-                logger.error(f"First error reason: {firstError.get('reason')}")
-                raise e
+            raise ValueError("please specify some IDs")
 
-        else:
-            logger.debug("No texts to add to index")
-            return []
+        return self._store.delete(ids=ids, refresh_indices=refresh_indices or False)
 
     def add_texts(
         self,
         texts: Iterable[str],
         metadatas: Optional[List[Dict[Any, Any]]] = None,
         ids: Optional[List[str]] = None,
         refresh_indices: bool = True,
         create_index_if_not_exists: bool = True,
         bulk_kwargs: Optional[Dict] = None,
         **kwargs: Any,
     ) -> List[str]:
-        """Run more texts through the embeddings and add to the vectorstore.
+        """Run more texts through the embeddings and add to the store.
 
         Args:
-            texts: Iterable of strings to add to the vectorstore.
+            texts: Iterable of strings to add to the store.
             metadatas: Optional list of metadatas associated with the texts.
             ids: Optional list of ids to associate with the texts.
             refresh_indices: Whether to refresh the Elasticsearch indices
                             after adding the texts.
             create_index_if_not_exists: Whether to create the Elasticsearch
                                         index if it doesn't already exist.
             *bulk_kwargs: Additional arguments to pass to Elasticsearch bulk.
                 - chunk_size: Optional. Number of texts to add to the
                     index at a time. Defaults to 500.
 
         Returns:
-            List of ids from adding the texts into the vectorstore.
+            List of ids from adding the texts into the store.
         """
-        if self.embedding is not None:
-            # If no search_type requires inference, we use the provided
-            # embedding function to embed the texts.
-            embeddings = self.embedding.embed_documents(list(texts))
-        else:
-            # the search_type doesn't require inference, so we don't need to
-            # embed the texts.
-            embeddings = None
-
-        return self.__add(
-            texts,
-            embeddings,
+        return self._store.add_texts(
+            texts=list(texts),
             metadatas=metadatas,
             ids=ids,
             refresh_indices=refresh_indices,
             create_index_if_not_exists=create_index_if_not_exists,
             bulk_kwargs=bulk_kwargs,
-            kwargs=kwargs,
         )
 
     def add_embeddings(
         self,
         text_embeddings: Iterable[Tuple[str, List[float]]],
         metadatas: Optional[List[dict]] = None,
         ids: Optional[List[str]] = None,
         refresh_indices: bool = True,
         create_index_if_not_exists: bool = True,
         bulk_kwargs: Optional[Dict] = None,
         **kwargs: Any,
     ) -> List[str]:
-        """Add the given texts and embeddings to the vectorstore.
+        """Add the given texts and embeddings to the store.
 
         Args:
             text_embeddings: Iterable pairs of string and embedding to
-                add to the vectorstore.
+                add to the store.
             metadatas: Optional list of metadatas associated with the texts.
             ids: Optional list of unique IDs.
             refresh_indices: Whether to refresh the Elasticsearch indices
                             after adding the texts.
             create_index_if_not_exists: Whether to create the Elasticsearch
                                         index if it doesn't already exist.
             *bulk_kwargs: Additional arguments to pass to Elasticsearch bulk.
                 - chunk_size: Optional. Number of texts to add to the
                     index at a time. Defaults to 500.
 
         Returns:
-            List of ids from adding the texts into the vectorstore.
+            List of ids from adding the texts into the store.
         """
         texts, embeddings = zip(*text_embeddings)
-        return self.__add(
-            list(texts),
-            list(embeddings),
+        return self._store.add_texts(
+            texts=list(texts),
             metadatas=metadatas,
+            vectors=list(embeddings),
             ids=ids,
             refresh_indices=refresh_indices,
             create_index_if_not_exists=create_index_if_not_exists,
             bulk_kwargs=bulk_kwargs,
-            kwargs=kwargs,
         )
 
     @classmethod
     def from_texts(
         cls,
         texts: List[str],
         embedding: Optional[Embeddings] = None,
@@ -1186,67 +1079,27 @@
                                 can be one of "COSINE",
                                 "EUCLIDEAN_DISTANCE", "DOT_PRODUCT",
                                 "MAX_INNER_PRODUCT".
             bulk_kwargs: Optional. Additional arguments to pass to
                         Elasticsearch bulk.
         """
 
-        elasticsearchStore = ElasticsearchStore._create_cls_from_kwargs(
-            embedding=embedding, **kwargs
-        )
+        index_name = kwargs.get("index_name")
+        if index_name is None:
+            raise ValueError("Please provide an index_name.")
+
+        elasticsearchStore = ElasticsearchStore(embedding=embedding, **kwargs)
 
         # Encode the provided texts and add them to the newly created index.
         elasticsearchStore.add_texts(
-            texts, metadatas=metadatas, bulk_kwargs=bulk_kwargs
+            texts=texts, metadatas=metadatas, bulk_kwargs=bulk_kwargs
         )
 
         return elasticsearchStore
 
-    @staticmethod
-    def _create_cls_from_kwargs(
-        embedding: Optional[Embeddings] = None, **kwargs: Any
-    ) -> "ElasticsearchStore":
-        index_name = kwargs.get("index_name")
-
-        if index_name is None:
-            raise ValueError("Please provide an index_name.")
-
-        es_connection = kwargs.get("es_connection")
-        es_cloud_id = kwargs.get("es_cloud_id")
-        es_url = kwargs.get("es_url")
-        es_user = kwargs.get("es_user")
-        es_password = kwargs.get("es_password")
-        es_api_key = kwargs.get("es_api_key")
-        vector_query_field = kwargs.get("vector_query_field")
-        query_field = kwargs.get("query_field")
-        distance_strategy = kwargs.get("distance_strategy")
-        strategy = kwargs.get("strategy", ElasticsearchStore.ApproxRetrievalStrategy())
-
-        optional_args = {}
-
-        if vector_query_field is not None:
-            optional_args["vector_query_field"] = vector_query_field
-
-        if query_field is not None:
-            optional_args["query_field"] = query_field
-
-        return ElasticsearchStore(
-            index_name=index_name,
-            embedding=embedding,
-            es_url=es_url,
-            es_connection=es_connection,
-            es_cloud_id=es_cloud_id,
-            es_user=es_user,
-            es_password=es_password,
-            es_api_key=es_api_key,
-            strategy=strategy,
-            distance_strategy=distance_strategy,
-            **optional_args,
-        )
-
     @classmethod
     def from_documents(
         cls,
         documents: List[Document],
         embedding: Optional[Embeddings] = None,
         bulk_kwargs: Optional[Dict] = None,
         **kwargs: Any,
@@ -1282,17 +1135,20 @@
             vector_query_field: Optional. Name of the field
                                 to store the embedding vectors in.
             query_field: Optional. Name of the field to store the texts in.
             bulk_kwargs: Optional. Additional arguments to pass to
                         Elasticsearch bulk.
         """
 
-        elasticsearchStore = ElasticsearchStore._create_cls_from_kwargs(
-            embedding=embedding, **kwargs
-        )
+        index_name = kwargs.get("index_name")
+        if index_name is None:
+            raise ValueError("Please provide an index_name.")
+
+        elasticsearchStore = ElasticsearchStore(embedding=embedding, **kwargs)
+
         # Encode the provided texts and add them to the newly created index.
         elasticsearchStore.add_documents(documents, bulk_kwargs=bulk_kwargs)
 
         return elasticsearchStore
 
     @staticmethod
     def ExactRetrievalStrategy() -> "ExactRetrievalStrategy":
```

### Comparing `langchain_elasticsearch-0.1.3/pyproject.toml` & `langchain_elasticsearch-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [tool.poetry]
 name = "langchain-elasticsearch"
-version = "0.1.3"
+version = "0.2.0"
 description = "An integration package connecting Elasticsearch and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-elastic"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain-elastic/tree/main/libs/elasticsearch"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1"
-elasticsearch = "^8.12.0"
-numpy = "^1"
+langchain-core = ">=0.1.50,<0.3"
+elasticsearch = {version = "^8.13.1", extras = ["vectorstore_mmr"]}
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
-langchain = "^0.1.13"
-langchain-text-splitters = ">=0.0.1,<0.1"
+langchain = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/langchain"}
+langchain-community = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/community"}
+langchain-text-splitters = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/text-splitters"}
 langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
```

### Comparing `langchain_elasticsearch-0.1.3/PKG-INFO` & `langchain_elasticsearch-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-elasticsearch
-Version: 0.1.3
+Version: 0.2.0
 Summary: An integration package connecting Elasticsearch and LangChain
 Home-page: https://github.com/langchain-ai/langchain-elastic
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: elasticsearch (>=8.12.0,<9.0.0)
-Requires-Dist: langchain-core (>=0.1,<0.2)
-Requires-Dist: numpy (>=1,<2)
+Requires-Dist: elasticsearch[vectorstore-mmr] (>=8.13.1,<9.0.0)
+Requires-Dist: langchain-core (>=0.1.50,<0.3)
 Project-URL: Repository, https://github.com/langchain-ai/langchain-elastic
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-elastic/tree/main/libs/elasticsearch
 Description-Content-Type: text/markdown
 
 # langchain-elasticsearch
 
 This package contains the LangChain integration with Elasticsearch.
```

