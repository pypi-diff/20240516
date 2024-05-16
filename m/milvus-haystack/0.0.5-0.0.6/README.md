# Comparing `tmp/milvus_haystack-0.0.5.tar.gz` & `tmp/milvus_haystack-0.0.6.tar.gz`

## Comparing `milvus_haystack-0.0.5.tar` & `milvus_haystack-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/OWNERS
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/.github/mergify.yml
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/.github/workflows/main.yml
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/.github/workflows/test.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/src/milvus_haystack/__about__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/src/milvus_haystack/__init__.py
--rw-r--r--   0        0        0    25580 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/src/milvus_haystack/document_store.py
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/src/milvus_haystack/filters.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/src/milvus_haystack/milvus_embedding_retriever.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/tests/test_document_store.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/tests/test_embedding_retriever.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/tests/test_filters.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/.gitignore
--rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/README.md
--rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 milvus_haystack-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/OWNERS
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/.github/mergify.yml
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/.github/workflows/test.yml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/src/milvus_haystack/__about__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/src/milvus_haystack/__init__.py
+-rw-r--r--   0        0        0    25495 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/src/milvus_haystack/document_store.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/src/milvus_haystack/filters.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/src/milvus_haystack/milvus_embedding_retriever.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     3386 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/tests/test_document_store.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/tests/test_embedding_retriever.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/tests/test_filters.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/.gitignore
+-rw-r--r--   0        0        0    10279 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/README.md
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6644 2020-02-02 00:00:00.000000 milvus_haystack-0.0.6/PKG-INFO
```

### Comparing `milvus_haystack-0.0.5/.github/mergify.yml` & `milvus_haystack-0.0.6/.github/mergify.yml`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.5/.github/workflows/test.yml` & `milvus_haystack-0.0.6/.github/workflows/test.yml`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 on:
   pull_request:
     paths:
       - "src/**"
       - "tests/**"
       - pyproject.toml
+      - .github/workflows/test.yml
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.event.pull_request.number || github.ref }}
   cancel-in-progress: ${{ github.event_name == 'pull_request' }}
 
 jobs:
   build:
@@ -32,19 +33,19 @@
         run: pip install --upgrade hatch
 
       - name: Lint
         run: hatch run lint:all
 
       - name: Run Milvus
         run: |
-          wget https://github.com/milvus-io/milvus/releases/download/v2.4.0-rc.1/milvus-standalone-docker-compose.yml -O docker-compose.yml
-          sudo docker compose up -d
+          wget https://raw.githubusercontent.com/milvus-io/milvus/master/scripts/standalone_embed.sh
+          bash standalone_embed.sh start
           sleep 5
           echo "\nMilvus server started!"
 
       - name: Run tests
         run: hatch run cov
 
       - name: Stop and Remove Milvus
         run: |
-          sudo docker compose down
+          bash standalone_embed.sh stop
           echo "\nMilvus server stopped and removed!"
```

### Comparing `milvus_haystack-0.0.5/src/milvus_haystack/document_store.py` & `milvus_haystack-0.0.6/src/milvus_haystack/document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -405,17 +405,15 @@
             given_address = str(host) + ":" + str(port)
         elif uri is not None:
             if uri.startswith("https://"):
                 given_address = uri.split("https://")[1]
             elif uri.startswith("http://"):
                 given_address = uri.split("http://")[1]
             else:
-                err_msg = "Invalid Milvus URI: %s", uri
-                logger.error(err_msg)
-                raise ValueError(err_msg)
+                given_address = uri  # Milvus lite
         elif address is not None:
             given_address = address
         else:
             given_address = None
             logger.debug("Missing standard address type for reuse attempt")
 
         # User defaults to empty string when getting connection info
```

### Comparing `milvus_haystack-0.0.5/src/milvus_haystack/filters.py` & `milvus_haystack-0.0.6/src/milvus_haystack/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 
 def _assert_comparison_filter(filters: Dict[str, Any]):
     assert "operator" in filters, "operator must be specified in filters"  # noqa: S101
     assert "field" in filters, "field must be specified in filters"  # noqa: S101
     assert "value" in filters, "value must be specified in filters"  # noqa: S101
     assert filters["operator"] in COMPARISON_OPERATORS, FilterError(  # noqa: S101
-        "operator must be one of: %s" % LOGIC_OPERATORS
+        f"operator must be one of: {LOGIC_OPERATORS}"
     )
 
 
 def _parse_logic(filters: Dict[str, Any]) -> str:
     try:
         _assert_logic_filter(filters)
     except AssertionError as assert_e:
@@ -81,9 +81,9 @@
         expr = operator.join([parse_filters(condition) for condition in filters["conditions"]])
     return f"({expr})"
 
 
 def _assert_logic_filter(filters: Dict[str, Any]):
     assert "operator" in filters, "operator must be specified in filters"  # noqa: S101
     assert "conditions" in filters, "conditions must be specified in filters"  # noqa: S101
-    assert filters["operator"] in LOGIC_OPERATORS, "operator must be one of: %s" % LOGIC_OPERATORS  # noqa: S101
+    assert filters["operator"] in LOGIC_OPERATORS, f"operator must be one of: {LOGIC_OPERATORS}"  # noqa: S101
     assert isinstance(filters["conditions"], list), "conditions must be a list"  # noqa: S101
```

### Comparing `milvus_haystack-0.0.5/src/milvus_haystack/milvus_embedding_retriever.py` & `milvus_haystack-0.0.6/src/milvus_haystack/milvus_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.5/tests/test_document_store.py` & `milvus_haystack-0.0.6/tests/test_document_store.py`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.5/tests/test_embedding_retriever.py` & `milvus_haystack-0.0.6/tests/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.5/tests/test_filters.py` & `milvus_haystack-0.0.6/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.5/.gitignore` & `milvus_haystack-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.5/LICENSE.txt` & `milvus_haystack-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.5/pyproject.toml` & `milvus_haystack-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `milvus_haystack-0.0.5/PKG-INFO` & `milvus_haystack-0.0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: milvus-haystack
-Version: 0.0.5
+Version: 0.0.6
 Project-URL: Documentation, https://github.com/milvus-io/milvus-haystack#readme
 Project-URL: Issues, https://github.com/milvus-io/milvus-haystack/issues
 Project-URL: Source, https://github.com/milvus-io/milvus-haystack
 Author-email: Zilliz <support@zilliz.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -25,121 +25,134 @@
 # Milvus Document Store for Haystack
 
 [![PyPI - Version](https://img.shields.io/pypi/v/milvus-haystack.svg)](https://pypi.org/project/milvus-haystack)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/milvus-haystack.svg)](https://pypi.org/project/milvus-haystack)
 
 ## Installation
 
-```console
-pip install milvus-haystack
+```shell
+pip install --upgrade pymilvus milvus-haystack
 ```
 
 ## Usage
 
-First, to start up a Milvus service, follow
-the ['Start Milvus'](https://milvus.io/docs/install_standalone-docker.md#Start-Milvus) instructions in the
-documentation.
+By default, if you install the latest version of pymilvus, you don't need to start the milvus service manually.
+Optionally, you
+can [start the Milvus service by docker](https://milvus.io/docs/install_standalone-docker.md#Start-Milvus).
 
-Then, to use the `MilvusDocumentStore` in a Haystack pipeline"
+Use the `MilvusDocumentStore` in a Haystack pipeline as a quick start.
 
 ```python
 from haystack import Document
 from milvus_haystack import MilvusDocumentStore
 
-document_store = MilvusDocumentStore()
+document_store = MilvusDocumentStore(
+    # If you have installed the latest version of pymilvus with milvus lite, you can use a local path as the uri without starting the milvus service.
+    connection_args={"uri": "./milvus.db"},
+    # Or, if you have started the milvus standalone service by docker, you can use the specified uri to connect to the service.
+    # connection_args={"uri": "http://localhost:19530"},
+    drop_old=True,
+)
 documents = [Document(
     content="A Foo Document",
     meta={"page": "100", "chapter": "intro"},
     embedding=[-10.0] * 128,
 )]
 document_store.write_documents(documents)
-document_store.count_documents()  # 1
+print(document_store.count_documents())  # 1
 ```
 
 ## Dive deep usage
 
-Here are the ways to build index, retrieval, and build rag pipeline respectively.
+Prepare an OpenAI API key and set it as an environment variable:
+
+```shell
+export OPENAI_API_KEY=<your_api_key>
+```
+
+Here are the ways to
+
+- Create the indexing Pipeline
+- Create the retrieval pipeline
+- Create the RAG pipeline
 
 ### Create the indexing Pipeline and index some documents
 
 ```python
 import glob
 import os
 
 from haystack import Pipeline
 from haystack.components.converters import MarkdownToDocument
-from haystack.components.embedders import SentenceTransformersDocumentEmbedder, SentenceTransformersTextEmbedder
+from haystack.components.embedders import OpenAIDocumentEmbedder, OpenAITextEmbedder
 from haystack.components.preprocessors import DocumentSplitter
 from haystack.components.writers import DocumentWriter
 
 from milvus_haystack import MilvusDocumentStore
 from milvus_haystack.milvus_embedding_retriever import MilvusEmbeddingRetriever
 
-file_paths = glob.glob("./your_docs.md")
+current_file_path = os.path.abspath(__file__)
+file_paths = [current_file_path]  # You can replace it with your own file paths.
 
 document_store = MilvusDocumentStore(
-    connection_args={
-        "host": "localhost",
-        "port": "19530",
-        "user": "",
-        "password": "",
-        "secure": False,
-    },
+    # If you have installed the latest version of pymilvus with milvus lite, you can use a local path as the uri without starting the milvus service.
+    connection_args={"uri": "./milvus.db"},
+    # Or, if you have started the milvus standalone service by docker, you can use the specified uri to connect to the service.
+    # connection_args={"uri": "http://localhost:19530"},
     drop_old=True,
 )
 indexing_pipeline = Pipeline()
 indexing_pipeline.add_component("converter", MarkdownToDocument())
 indexing_pipeline.add_component("splitter", DocumentSplitter(split_by="sentence", split_length=2))
-indexing_pipeline.add_component("embedder", SentenceTransformersDocumentEmbedder())
+indexing_pipeline.add_component("embedder", OpenAIDocumentEmbedder())
 indexing_pipeline.add_component("writer", DocumentWriter(document_store))
 indexing_pipeline.connect("converter", "splitter")
 indexing_pipeline.connect("splitter", "embedder")
 indexing_pipeline.connect("embedder", "writer")
 indexing_pipeline.run({"converter": {"sources": file_paths}})
 
 print("Number of documents:", document_store.count_documents())
 ```
 
 ### Create the retrieval pipeline and try a query
 
 ```python
-question = "What is Milvus?"
+question = "How to set the service uri with milvus lite?"  # You can replace it with your own question. 
 
 retrieval_pipeline = Pipeline()
-retrieval_pipeline.add_component("embedder", SentenceTransformersTextEmbedder())
+retrieval_pipeline.add_component("embedder", OpenAITextEmbedder())
 retrieval_pipeline.add_component("retriever", MilvusEmbeddingRetriever(document_store=document_store, top_k=3))
 retrieval_pipeline.connect("embedder", "retriever")
 
 retrieval_results = retrieval_pipeline.run({"embedder": {"text": question}})
 
 for doc in retrieval_results["retriever"]["documents"]:
     print(doc.content)
     print("-" * 10)
 ```
 
 ### Create the RAG pipeline and try a query
 
 ```python
 from haystack.utils import Secret
-from haystack.components.embedders import SentenceTransformersTextEmbedder
 from haystack.components.builders import PromptBuilder
 from haystack.components.generators import OpenAIGenerator
 
 prompt_template = """Answer the following query based on the provided context. If the context does
                      not include an answer, reply with 'I don't know'.\n
                      Query: {{query}}
                      Documents:
                      {% for doc in documents %}
                         {{ doc.content }}
                      {% endfor %}
                      Answer: 
                   """
 
 rag_pipeline = Pipeline()
-rag_pipeline.add_component("text_embedder", SentenceTransformersTextEmbedder())
+rag_pipeline.add_component("text_embedder", OpenAITextEmbedder())
 rag_pipeline.add_component("retriever", MilvusEmbeddingRetriever(document_store=document_store, top_k=3))
 rag_pipeline.add_component("prompt_builder", PromptBuilder(template=prompt_template))
 rag_pipeline.add_component("generator", OpenAIGenerator(api_key=Secret.from_token(os.getenv("OPENAI_API_KEY")),
                                                         generation_kwargs={"temperature": 0}))
 rag_pipeline.connect("text_embedder.embedding", "retriever.query_embedding")
 rag_pipeline.connect("retriever.documents", "prompt_builder.documents")
 rag_pipeline.connect("prompt_builder", "generator")
```

