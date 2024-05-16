# Comparing `tmp/langchain_elasticsearch-0.2.0.tar.gz` & `tmp/langchain_elasticsearch-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_elasticsearch-0.2.0.tar", max compression
+gzip compressed data, was "langchain_elasticsearch-0.2.1.tar", max compression
```

## Comparing `langchain_elasticsearch-0.2.0.tar` & `langchain_elasticsearch-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-05-16 03:06:25.616031 langchain_elasticsearch-0.2.0/LICENSE
--rw-r--r--   0        0        0     5805 2024-05-16 03:06:25.616031 langchain_elasticsearch-0.2.0/README.md
--rw-r--r--   0        0        0     1185 2024-05-16 03:06:25.616031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/__init__.py
--rw-r--r--   0        0        0     1393 2024-05-16 03:06:25.616031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/_utilities.py
--rw-r--r--   0        0        0     7748 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/cache.py
--rw-r--r--   0        0        0     5417 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/chat_history.py
--rw-r--r--   0        0        0     1094 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/client.py
--rw-r--r--   0        0        0     9253 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/embeddings.py
--rw-r--r--   0        0        0        0 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/py.typed
--rw-r--r--   0        0        0     4764 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/retrievers.py
--rw-r--r--   0        0        0    44233 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/langchain_elasticsearch/vectorstores.py
--rw-r--r--   0        0        0     2925 2024-05-16 03:06:25.620031 langchain_elasticsearch-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6681 1970-01-01 00:00:00.000000 langchain_elasticsearch-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5805 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/README.md
+-rw-r--r--   0        0        0     1185 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/__init__.py
+-rw-r--r--   0        0        0     1393 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/_utilities.py
+-rw-r--r--   0        0        0     7748 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/cache.py
+-rw-r--r--   0        0        0     5417 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/chat_history.py
+-rw-r--r--   0        0        0     1094 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/client.py
+-rw-r--r--   0        0        0     9253 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/embeddings.py
+-rw-r--r--   0        0        0        0 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/py.typed
+-rw-r--r--   0        0        0     4764 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/retrievers.py
+-rw-r--r--   0        0        0    44274 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/vectorstores.py
+-rw-r--r--   0        0        0     2925 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6681 1970-01-01 00:00:00.000000 langchain_elasticsearch-0.2.1/PKG-INFO
```

### Comparing `langchain_elasticsearch-0.2.0/LICENSE` & `langchain_elasticsearch-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.2.0/README.md` & `langchain_elasticsearch-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.2.0/langchain_elasticsearch/__init__.py` & `langchain_elasticsearch-0.2.1/langchain_elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.2.0/langchain_elasticsearch/_utilities.py` & `langchain_elasticsearch-0.2.1/langchain_elasticsearch/_utilities.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.2.0/langchain_elasticsearch/cache.py` & `langchain_elasticsearch-0.2.1/langchain_elasticsearch/cache.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.2.0/langchain_elasticsearch/chat_history.py` & `langchain_elasticsearch-0.2.1/langchain_elasticsearch/chat_history.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.2.0/langchain_elasticsearch/client.py` & `langchain_elasticsearch-0.2.1/langchain_elasticsearch/client.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.2.0/langchain_elasticsearch/embeddings.py` & `langchain_elasticsearch-0.2.1/langchain_elasticsearch/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.2.0/langchain_elasticsearch/retrievers.py` & `langchain_elasticsearch-0.2.1/langchain_elasticsearch/retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.2.0/langchain_elasticsearch/vectorstores.py` & `langchain_elasticsearch-0.2.1/langchain_elasticsearch/vectorstores.py`

 * *Files 0% similar despite different names*

```diff
@@ -713,14 +713,15 @@
             embedding_service=embedding_service,
             text_field=query_field,
             vector_field=vector_query_field,
             user_agent=user_agent("langchain-py-vs"),
         )
 
         self.embedding = embedding
+        self.client = self._store.client
         self._embedding_service = embedding_service
         self.query_field = query_field
         self.vector_query_field = vector_query_field
 
     def close(self) -> None:
         self._store.close()
```

### Comparing `langchain_elasticsearch-0.2.0/pyproject.toml` & `langchain_elasticsearch-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-elasticsearch"
-version = "0.2.0"
+version = "0.2.1"
 description = "An integration package connecting Elasticsearch and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-elastic"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_elasticsearch-0.2.0/PKG-INFO` & `langchain_elasticsearch-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-elasticsearch
-Version: 0.2.0
+Version: 0.2.1
 Summary: An integration package connecting Elasticsearch and LangChain
 Home-page: https://github.com/langchain-ai/langchain-elastic
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

