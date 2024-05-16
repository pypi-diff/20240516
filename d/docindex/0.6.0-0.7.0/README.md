# Comparing `tmp/docindex-0.6.0.tar.gz` & `tmp/docindex-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docindex-0.6.0.tar", last modified: Tue Apr 30 17:14:37 2024, max compression
+gzip compressed data, was "docindex-0.7.0.tar", last modified: Thu May 16 16:42:16 2024, max compression
```

## Comparing `docindex-0.6.0.tar` & `docindex-0.7.0.tar`

### file list

```diff
@@ -1,44 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.072249 docindex-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-30 17:14:33.000000 docindex-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-30 17:14:37.072249 docindex-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8306 2024-04-30 17:14:33.000000 docindex-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-30 17:14:33.000000 docindex-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-30 17:14:37.072249 docindex-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.068249 docindex-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.068249 docindex-0.6.0/src/_cohere/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_cohere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_cohere/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_cohere/create_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_cohere/delete_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     9250 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_cohere/doc_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_cohere/doc_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_cohere/index_documents.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.068249 docindex-0.6.0/src/_google/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_google/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_google/create_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_google/delete_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     9522 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_google/doc_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_google/index_documents.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.072249 docindex-0.6.0/src/_openai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_openai/create_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_openai/delete_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     9206 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_openai/doc_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_openai/doc_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-30 17:14:33.000000 docindex-0.6.0/src/_openai/index_documents.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.072249 docindex-0.6.0/src/docindex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-30 17:14:37.000000 docindex-0.6.0/src/docindex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-30 17:14:37.000000 docindex-0.6.0/src/docindex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 17:14:37.000000 docindex-0.6.0/src/docindex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-30 17:14:37.000000 docindex-0.6.0/src/docindex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-30 17:14:37.000000 docindex-0.6.0/src/docindex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.072249 docindex-0.6.0/src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:33.000000 docindex-0.6.0/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3542 2024-04-30 17:14:33.000000 docindex-0.6.0/src/tests/cohereindex_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-30 17:14:33.000000 docindex-0.6.0/src/tests/googleindex_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-30 17:14:33.000000 docindex-0.6.0/src/tests/openaiindex_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:37.072249 docindex-0.6.0/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 17:14:33.000000 docindex-0.6.0/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-30 17:14:33.000000 docindex-0.6.0/src/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-30 17:14:33.000000 docindex-0.6.0/src/utils/response_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:42:16.473614 docindex-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 16:42:12.000000 docindex-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-05-16 16:42:16.473614 docindex-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8604 2024-05-16 16:42:12.000000 docindex-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 16:42:12.000000 docindex-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-16 16:42:16.477614 docindex-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:42:16.469614 docindex-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:42:16.469614 docindex-0.7.0/src/_cohere/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:42:12.000000 docindex-0.7.0/src/_cohere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-05-16 16:42:12.000000 docindex-0.7.0/src/_cohere/doc_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-16 16:42:12.000000 docindex-0.7.0/src/_cohere/index_documents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:42:16.473614 docindex-0.7.0/src/_google/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:42:12.000000 docindex-0.7.0/src/_google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11177 2024-05-16 16:42:12.000000 docindex-0.7.0/src/_google/doc_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-16 16:42:12.000000 docindex-0.7.0/src/_google/index_documents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:42:16.473614 docindex-0.7.0/src/_openai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:42:12.000000 docindex-0.7.0/src/_openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10844 2024-05-16 16:42:12.000000 docindex-0.7.0/src/_openai/doc_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-16 16:42:12.000000 docindex-0.7.0/src/_openai/index_documents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:42:16.473614 docindex-0.7.0/src/docindex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9546 2024-05-16 16:42:16.000000 docindex-0.7.0/src/docindex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-16 16:42:16.000000 docindex-0.7.0/src/docindex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 16:42:16.000000 docindex-0.7.0/src/docindex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-16 16:42:16.000000 docindex-0.7.0/src/docindex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 16:42:16.000000 docindex-0.7.0/src/docindex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:42:16.473614 docindex-0.7.0/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:42:12.000000 docindex-0.7.0/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2024-05-16 16:42:12.000000 docindex-0.7.0/src/tests/cohereindex_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-16 16:42:12.000000 docindex-0.7.0/src/tests/googleindex_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-16 16:42:12.000000 docindex-0.7.0/src/tests/openaiindex_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 16:42:16.473614 docindex-0.7.0/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 16:42:12.000000 docindex-0.7.0/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-16 16:42:12.000000 docindex-0.7.0/src/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-16 16:42:12.000000 docindex-0.7.0/src/utils/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-16 16:42:12.000000 docindex-0.7.0/src/utils/delete_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-16 16:42:12.000000 docindex-0.7.0/src/utils/doc_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-16 16:42:12.000000 docindex-0.7.0/src/utils/rerank.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-16 16:42:12.000000 docindex-0.7.0/src/utils/response_model.py
```

### Comparing `docindex-0.6.0/LICENSE` & `docindex-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docindex-0.6.0/PKG-INFO` & `docindex-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docindex
-Version: 0.6.0
+Version: 0.7.0
 Summary: A package for fast persistent storage of multiple document embeddings and their metadata into Pinecone for production-level RAG.
 Home-page: https://github.com/KevKibe/docindex
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -106,15 +106,20 @@
 
 # Initialize the Vectorstore
 vectorstore = pinecone_indexer.initialize_vectorstore(index_name)
 ```
 ### Query and Retrieve Information
 ```python
 query = "what is the transformers architecture"
-response = pinecone_indexer.retrieve_and_generate(vector_store = vectorstore, query = query)
+response = pinecone_indexer.retrieve_and_generate(
+                    vector_store = vectorstore, 
+                    query = query, 
+                    top_k = "number of sources to retrieve",    # Default is 3
+                    rerank_model = "reranking model"            # Default is 'flashrank'  Other models available Docs:https://github.com/AnswerDotAI/rerankers
+                    )
 response
 ```
 
 ### Response
 ```bash
 query='what is the transformers architecture' result='The Transformer follows this overall architecture using stacked self-attention and point-wise, fully-connected layers for both the encoder and decoder, shown in the left and right halves of Figure 1, respectively.' page=1 source_documents=[Document(page_content='Figure 1: The Transformer - model architecture.\nThe Transformer follows this overall architecture using stacked self-attention and point-wise, fully\nconnected layers for both the encoder and decoder, shown in the left and right halves of Figure 1,\nrespectively.\n3.1 Encoder and Decoder Stacks\nEncoder: The encoder is composed of a stack of N= 6 identical layers. Each layer has two\nsub-layers. The first is a multi-head self-attention mechanism, and the second is a simple, position-\nwise fully connected feed-forward network. We employ a residual connection [ 11] around each of\nthe two sub-layers, followed by layer normalization [ 1]. That is, the output of each sub-layer is\nLayerNorm( x+ Sublayer( x)), where Sublayer( x)is the function implemented by the sub-layer\nitself. To facilitate these residual connections, all sub-layers in the model, as well as the embedding\nlayers, produce outputs of dimension dmodel = 512 .\nDecoder: The decoder is also composed of a stack of N= 6identical layers. In addition to the two', source=2.0, title='https://arxiv.org/pdf/1706.03762.pdf')]
 
@@ -163,15 +168,15 @@
 ```bash
 cd src
 ```
 - To create an index
 
 ```bash
 # Using OpenAI 
-python -m  _openai.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" -
+python -m  utils.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" 
 
 ```
 
 - Run the command to start indexing the documents
 
 ```bash
 # Using OpenAI
@@ -187,15 +192,15 @@
 python -m _cohere.index_documents   --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --cohere_api_key "your_google_api_key" --batch_limit "batch-limit" --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-size"
 
 ```
 - To delete an index
 
 ```bash
 # Using OpenAI 
-python -m  _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" 
+python -m  utils.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" 
 
 ```
 
 ## Contributing 
 🌟 First consider giving it a star at the top right. It means a lot!
 Contributions are welcome and encouraged.
 Before contributing, please take a moment to review our [Contribution Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for important information on how to contribute to this project.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docindex Version: 0.6.0 Summary: A package for fast
+Metadata-Version: 2.1 Name: docindex Version: 0.7.0 Summary: A package for fast
 persistent storage of multiple document embeddings and their metadata into
 Pinecone for production-level RAG. Home-page: https://github.com/KevKibe/
 docindex Author: Kevin Kibe Author-email: keviinkibe@gmail.com License: MIT
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: pinecone-client==3.2.2 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: pypdf==4.1.0 Requires-Dist: unstructured==0.12.6 Requires-Dist:
 langchain-community==0.0.31 Requires-Dist: langchain==0.1.14 Requires-Dist:
@@ -55,66 +55,69 @@
   CoherePineconeIndexer(index_name, pinecone_api_key, cohere_api_key) # Using
   Cohere # To create a new Index pinecone_indexer.create_index() # Store the
           document embeddings with the specified URLs and batch limit
 pinecone_indexer.index_documents(urls,batch_limit,chunk_size) # Initialize the
  Vectorstore vectorstore = pinecone_indexer.initialize_vectorstore(index_name)
      ``` ### Query and Retrieve Information ```python query = "what is the
  transformers architecture" response = pinecone_indexer.retrieve_and_generate
- (vector_store = vectorstore, query = query) response ``` ### Response ```bash
- query='what is the transformers architecture' result='The Transformer follows
- this overall architecture using stacked self-attention and point-wise, fully-
-connected layers for both the encoder and decoder, shown in the left and right
-     halves of Figure 1, respectively.' page=1 source_documents=[Document
-(page_content='Figure 1: The Transformer - model architecture.\nThe Transformer
-follows this overall architecture using stacked self-attention and point-wise,
-fully\nconnected layers for both the encoder and decoder, shown in the left and
-       right halves of Figure 1,\nrespectively.\n3.1 Encoder and Decoder
- Stacks\nEncoder: The encoder is composed of a stack of N= 6 identical layers.
-   Each layer has two\nsub-layers. The first is a multi-head self-attention
- mechanism, and the second is a simple, position-\nwise fully connected feed-
-forward network. We employ a residual connection [ 11] around each of\nthe two
- sub-layers, followed by layer normalization [ 1]. That is, the output of each
- sub-layer is\nLayerNorm( x+ Sublayer( x)), where Sublayer( x)is the function
-implemented by the sub-layer\nitself. To facilitate these residual connections,
-all sub-layers in the model, as well as the embedding\nlayers, produce outputs
- of dimension dmodel = 512 .\nDecoder: The decoder is also composed of a stack
- of N= 6identical layers. In addition to the two', source=2.0, title='https://
- arxiv.org/pdf/1706.03762.pdf')] ``` ### Query Response Attributes: ```python
- response.query # The query that was submitted response.result # The result of
- the query, including any retrieved information. response.source_documents # A
-list of source documents related to the query. response.sources # A list of the
- sources (page numbers) from the source documents. response.titles # A list of
- the titles from the source documents. response.page_contents # A list of the
- page contents from the source documents. ``` ### Delete Index: ```python # To
-delete the created Index pinecone_indexer.delete_index() ``` ## Using the CLI -
-  Clone the Repository: Clone or download the application code to your local
-machine. ```bash git clone https://github.com/KevKibe/docindex.git ``` - Create
- a virtual environment for the project and activate it. ```bash # Navigate to
+  ( vector_store = vectorstore, query = query, top_k = "number of sources to
+    retrieve", # Default is 3 rerank_model = "reranking model" # Default is
+    'flashrank' Other models available Docs:https://github.com/AnswerDotAI/
+ rerankers ) response ``` ### Response ```bash query='what is the transformers
+ architecture' result='The Transformer follows this overall architecture using
+  stacked self-attention and point-wise, fully-connected layers for both the
+     encoder and decoder, shown in the left and right halves of Figure 1,
+ respectively.' page=1 source_documents=[Document(page_content='Figure 1: The
+    Transformer - model architecture.\nThe Transformer follows this overall
+  architecture using stacked self-attention and point-wise, fully\nconnected
+layers for both the encoder and decoder, shown in the left and right halves of
+Figure 1,\nrespectively.\n3.1 Encoder and Decoder Stacks\nEncoder: The encoder
+   is composed of a stack of N= 6 identical layers. Each layer has two\nsub-
+layers. The first is a multi-head self-attention mechanism, and the second is a
+   simple, position-\nwise fully connected feed-forward network. We employ a
+residual connection [ 11] around each of\nthe two sub-layers, followed by layer
+  normalization [ 1]. That is, the output of each sub-layer is\nLayerNorm( x+
+   Sublayer( x)), where Sublayer( x)is the function implemented by the sub-
+layer\nitself. To facilitate these residual connections, all sub-layers in the
+model, as well as the embedding\nlayers, produce outputs of dimension dmodel =
+   512 .\nDecoder: The decoder is also composed of a stack of N= 6identical
+  layers. In addition to the two', source=2.0, title='https://arxiv.org/pdf/
+1706.03762.pdf')] ``` ### Query Response Attributes: ```python response.query #
+    The query that was submitted response.result # The result of the query,
+  including any retrieved information. response.source_documents # A list of
+source documents related to the query. response.sources # A list of the sources
+   (page numbers) from the source documents. response.titles # A list of the
+ titles from the source documents. response.page_contents # A list of the page
+contents from the source documents. ``` ### Delete Index: ```python # To delete
+the created Index pinecone_indexer.delete_index() ``` ## Using the CLI - Clone
+ the Repository: Clone or download the application code to your local machine.
+   ```bash git clone https://github.com/KevKibe/docindex.git ``` - Create a
+  virtual environment for the project and activate it. ```bash # Navigate to
 project repository cd docindex # create virtual environment python -m venv venv
      # activate virtual environment source venv/bin/activate ``` - Install
  dependencies by running this command ```bash pip install -r requirements.txt
  ``` - Navigate to src ```bash cd src ``` - To create an index ```bash # Using
-           OpenAI python -m _openai.create_index --pinecone_api_key
-"your_pinecone_api_key" --index_name "your_index_name" - ``` - Run the command
-        to start indexing the documents ```bash # Using OpenAI python -
-    m _openai.index_documents --pinecone_api_key "your_pinecone_api_key" --
-    index_name "your_index_name" --openai_api_key "your_openai_api_key" --
- batch_limit "batch-limit" --docs "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-
-    size" # Using Google Generative AI python -m _google.index_documents --
+OpenAI python -m utils.create_index --pinecone_api_key "your_pinecone_api_key"
+  --index_name "your_index_name" ``` - Run the command to start indexing the
+     documents ```bash # Using OpenAI python -m _openai.index_documents --
   pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --
- google_api_key "your_google_api_key" --batch_limit "batch-limit" --docs "doc-
-      1.pdf" "doc-2.pdf' --chunk_size "chunk-size" Using Cohere python -
-    m _cohere.index_documents --pinecone_api_key "your_pinecone_api_key" --
-    index_name "your_index_name" --cohere_api_key "your_google_api_key" --
+ openai_api_key "your_openai_api_key" --batch_limit "batch-limit" --docs "doc-
+   1.pdf" "doc-2.pdf' --chunk_size "chunk-size" # Using Google Generative AI
+python -m _google.index_documents --pinecone_api_key "your_pinecone_api_key" --
+    index_name "your_index_name" --google_api_key "your_google_api_key" --
  batch_limit "batch-limit" --docs "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-
-        size" ``` - To delete an index ```bash # Using OpenAI python -
-m _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name
- "your_index_name" ``` ## Contributing ð First consider giving it a star at
-the top right. It means a lot! Contributions are welcome and encouraged. Before
-  contributing, please take a moment to review our [Contribution Guidelines]
-  (https://github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for
- important information on how to contribute to this project. If you're unsure
-about anything or need assistance, don't hesitate to reach out to us or open an
-issue to discuss your ideas. We look forward to your contributions! ## License
-  This project is licensed under the MIT License - see the [LICENSE](https://
- github.com/KevKibe/docindex/blob/master/LICENSE) file for details. ## Contact
-    For any enquiries, please reach out to me through keviinkibe@gmail.com
+    size" Using Cohere python -m _cohere.index_documents --pinecone_api_key
+    "your_pinecone_api_key" --index_name "your_index_name" --cohere_api_key
+  "your_google_api_key" --batch_limit "batch-limit" --docs "doc-1.pdf" "doc-
+   2.pdf' --chunk_size "chunk-size" ``` - To delete an index ```bash # Using
+OpenAI python -m utils.delete_index --pinecone_api_key "your_pinecone_api_key"
+ --index_name "your_index_name" ``` ## Contributing ð First consider giving
+   it a star at the top right. It means a lot! Contributions are welcome and
+     encouraged. Before contributing, please take a moment to review our
+[Contribution Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/
+    CONTRIBUTING.md) for important information on how to contribute to this
+project. If you're unsure about anything or need assistance, don't hesitate to
+reach out to us or open an issue to discuss your ideas. We look forward to your
+contributions! ## License This project is licensed under the MIT License - see
+the [LICENSE](https://github.com/KevKibe/docindex/blob/master/LICENSE) file for
+     details. ## Contact For any enquiries, please reach out to me through
+                             keviinkibe@gmail.com
```

### Comparing `docindex-0.6.0/README.md` & `docindex-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,20 @@
 
 # Initialize the Vectorstore
 vectorstore = pinecone_indexer.initialize_vectorstore(index_name)
 ```
 ### Query and Retrieve Information
 ```python
 query = "what is the transformers architecture"
-response = pinecone_indexer.retrieve_and_generate(vector_store = vectorstore, query = query)
+response = pinecone_indexer.retrieve_and_generate(
+                    vector_store = vectorstore, 
+                    query = query, 
+                    top_k = "number of sources to retrieve",    # Default is 3
+                    rerank_model = "reranking model"            # Default is 'flashrank'  Other models available Docs:https://github.com/AnswerDotAI/rerankers
+                    )
 response
 ```
 
 ### Response
 ```bash
 query='what is the transformers architecture' result='The Transformer follows this overall architecture using stacked self-attention and point-wise, fully-connected layers for both the encoder and decoder, shown in the left and right halves of Figure 1, respectively.' page=1 source_documents=[Document(page_content='Figure 1: The Transformer - model architecture.\nThe Transformer follows this overall architecture using stacked self-attention and point-wise, fully\nconnected layers for both the encoder and decoder, shown in the left and right halves of Figure 1,\nrespectively.\n3.1 Encoder and Decoder Stacks\nEncoder: The encoder is composed of a stack of N= 6 identical layers. Each layer has two\nsub-layers. The first is a multi-head self-attention mechanism, and the second is a simple, position-\nwise fully connected feed-forward network. We employ a residual connection [ 11] around each of\nthe two sub-layers, followed by layer normalization [ 1]. That is, the output of each sub-layer is\nLayerNorm( x+ Sublayer( x)), where Sublayer( x)is the function implemented by the sub-layer\nitself. To facilitate these residual connections, all sub-layers in the model, as well as the embedding\nlayers, produce outputs of dimension dmodel = 512 .\nDecoder: The decoder is also composed of a stack of N= 6identical layers. In addition to the two', source=2.0, title='https://arxiv.org/pdf/1706.03762.pdf')]
 
@@ -136,15 +141,15 @@
 ```bash
 cd src
 ```
 - To create an index
 
 ```bash
 # Using OpenAI 
-python -m  _openai.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" -
+python -m  utils.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" 
 
 ```
 
 - Run the command to start indexing the documents
 
 ```bash
 # Using OpenAI
@@ -160,15 +165,15 @@
 python -m _cohere.index_documents   --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --cohere_api_key "your_google_api_key" --batch_limit "batch-limit" --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-size"
 
 ```
 - To delete an index
 
 ```bash
 # Using OpenAI 
-python -m  _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" 
+python -m  utils.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" 
 
 ```
 
 ## Contributing 
 🌟 First consider giving it a star at the top right. It means a lot!
 Contributions are welcome and encouraged.
 Before contributing, please take a moment to review our [Contribution Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for important information on how to contribute to this project.
```

#### html2text {}

```diff
@@ -42,66 +42,69 @@
   CoherePineconeIndexer(index_name, pinecone_api_key, cohere_api_key) # Using
   Cohere # To create a new Index pinecone_indexer.create_index() # Store the
           document embeddings with the specified URLs and batch limit
 pinecone_indexer.index_documents(urls,batch_limit,chunk_size) # Initialize the
  Vectorstore vectorstore = pinecone_indexer.initialize_vectorstore(index_name)
      ``` ### Query and Retrieve Information ```python query = "what is the
  transformers architecture" response = pinecone_indexer.retrieve_and_generate
- (vector_store = vectorstore, query = query) response ``` ### Response ```bash
- query='what is the transformers architecture' result='The Transformer follows
- this overall architecture using stacked self-attention and point-wise, fully-
-connected layers for both the encoder and decoder, shown in the left and right
-     halves of Figure 1, respectively.' page=1 source_documents=[Document
-(page_content='Figure 1: The Transformer - model architecture.\nThe Transformer
-follows this overall architecture using stacked self-attention and point-wise,
-fully\nconnected layers for both the encoder and decoder, shown in the left and
-       right halves of Figure 1,\nrespectively.\n3.1 Encoder and Decoder
- Stacks\nEncoder: The encoder is composed of a stack of N= 6 identical layers.
-   Each layer has two\nsub-layers. The first is a multi-head self-attention
- mechanism, and the second is a simple, position-\nwise fully connected feed-
-forward network. We employ a residual connection [ 11] around each of\nthe two
- sub-layers, followed by layer normalization [ 1]. That is, the output of each
- sub-layer is\nLayerNorm( x+ Sublayer( x)), where Sublayer( x)is the function
-implemented by the sub-layer\nitself. To facilitate these residual connections,
-all sub-layers in the model, as well as the embedding\nlayers, produce outputs
- of dimension dmodel = 512 .\nDecoder: The decoder is also composed of a stack
- of N= 6identical layers. In addition to the two', source=2.0, title='https://
- arxiv.org/pdf/1706.03762.pdf')] ``` ### Query Response Attributes: ```python
- response.query # The query that was submitted response.result # The result of
- the query, including any retrieved information. response.source_documents # A
-list of source documents related to the query. response.sources # A list of the
- sources (page numbers) from the source documents. response.titles # A list of
- the titles from the source documents. response.page_contents # A list of the
- page contents from the source documents. ``` ### Delete Index: ```python # To
-delete the created Index pinecone_indexer.delete_index() ``` ## Using the CLI -
-  Clone the Repository: Clone or download the application code to your local
-machine. ```bash git clone https://github.com/KevKibe/docindex.git ``` - Create
- a virtual environment for the project and activate it. ```bash # Navigate to
+  ( vector_store = vectorstore, query = query, top_k = "number of sources to
+    retrieve", # Default is 3 rerank_model = "reranking model" # Default is
+    'flashrank' Other models available Docs:https://github.com/AnswerDotAI/
+ rerankers ) response ``` ### Response ```bash query='what is the transformers
+ architecture' result='The Transformer follows this overall architecture using
+  stacked self-attention and point-wise, fully-connected layers for both the
+     encoder and decoder, shown in the left and right halves of Figure 1,
+ respectively.' page=1 source_documents=[Document(page_content='Figure 1: The
+    Transformer - model architecture.\nThe Transformer follows this overall
+  architecture using stacked self-attention and point-wise, fully\nconnected
+layers for both the encoder and decoder, shown in the left and right halves of
+Figure 1,\nrespectively.\n3.1 Encoder and Decoder Stacks\nEncoder: The encoder
+   is composed of a stack of N= 6 identical layers. Each layer has two\nsub-
+layers. The first is a multi-head self-attention mechanism, and the second is a
+   simple, position-\nwise fully connected feed-forward network. We employ a
+residual connection [ 11] around each of\nthe two sub-layers, followed by layer
+  normalization [ 1]. That is, the output of each sub-layer is\nLayerNorm( x+
+   Sublayer( x)), where Sublayer( x)is the function implemented by the sub-
+layer\nitself. To facilitate these residual connections, all sub-layers in the
+model, as well as the embedding\nlayers, produce outputs of dimension dmodel =
+   512 .\nDecoder: The decoder is also composed of a stack of N= 6identical
+  layers. In addition to the two', source=2.0, title='https://arxiv.org/pdf/
+1706.03762.pdf')] ``` ### Query Response Attributes: ```python response.query #
+    The query that was submitted response.result # The result of the query,
+  including any retrieved information. response.source_documents # A list of
+source documents related to the query. response.sources # A list of the sources
+   (page numbers) from the source documents. response.titles # A list of the
+ titles from the source documents. response.page_contents # A list of the page
+contents from the source documents. ``` ### Delete Index: ```python # To delete
+the created Index pinecone_indexer.delete_index() ``` ## Using the CLI - Clone
+ the Repository: Clone or download the application code to your local machine.
+   ```bash git clone https://github.com/KevKibe/docindex.git ``` - Create a
+  virtual environment for the project and activate it. ```bash # Navigate to
 project repository cd docindex # create virtual environment python -m venv venv
      # activate virtual environment source venv/bin/activate ``` - Install
  dependencies by running this command ```bash pip install -r requirements.txt
  ``` - Navigate to src ```bash cd src ``` - To create an index ```bash # Using
-           OpenAI python -m _openai.create_index --pinecone_api_key
-"your_pinecone_api_key" --index_name "your_index_name" - ``` - Run the command
-        to start indexing the documents ```bash # Using OpenAI python -
-    m _openai.index_documents --pinecone_api_key "your_pinecone_api_key" --
-    index_name "your_index_name" --openai_api_key "your_openai_api_key" --
- batch_limit "batch-limit" --docs "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-
-    size" # Using Google Generative AI python -m _google.index_documents --
+OpenAI python -m utils.create_index --pinecone_api_key "your_pinecone_api_key"
+  --index_name "your_index_name" ``` - Run the command to start indexing the
+     documents ```bash # Using OpenAI python -m _openai.index_documents --
   pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --
- google_api_key "your_google_api_key" --batch_limit "batch-limit" --docs "doc-
-      1.pdf" "doc-2.pdf' --chunk_size "chunk-size" Using Cohere python -
-    m _cohere.index_documents --pinecone_api_key "your_pinecone_api_key" --
-    index_name "your_index_name" --cohere_api_key "your_google_api_key" --
+ openai_api_key "your_openai_api_key" --batch_limit "batch-limit" --docs "doc-
+   1.pdf" "doc-2.pdf' --chunk_size "chunk-size" # Using Google Generative AI
+python -m _google.index_documents --pinecone_api_key "your_pinecone_api_key" --
+    index_name "your_index_name" --google_api_key "your_google_api_key" --
  batch_limit "batch-limit" --docs "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-
-        size" ``` - To delete an index ```bash # Using OpenAI python -
-m _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name
- "your_index_name" ``` ## Contributing ð First consider giving it a star at
-the top right. It means a lot! Contributions are welcome and encouraged. Before
-  contributing, please take a moment to review our [Contribution Guidelines]
-  (https://github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for
- important information on how to contribute to this project. If you're unsure
-about anything or need assistance, don't hesitate to reach out to us or open an
-issue to discuss your ideas. We look forward to your contributions! ## License
-  This project is licensed under the MIT License - see the [LICENSE](https://
- github.com/KevKibe/docindex/blob/master/LICENSE) file for details. ## Contact
-    For any enquiries, please reach out to me through keviinkibe@gmail.com
+    size" Using Cohere python -m _cohere.index_documents --pinecone_api_key
+    "your_pinecone_api_key" --index_name "your_index_name" --cohere_api_key
+  "your_google_api_key" --batch_limit "batch-limit" --docs "doc-1.pdf" "doc-
+   2.pdf' --chunk_size "chunk-size" ``` - To delete an index ```bash # Using
+OpenAI python -m utils.delete_index --pinecone_api_key "your_pinecone_api_key"
+ --index_name "your_index_name" ``` ## Contributing ð First consider giving
+   it a star at the top right. It means a lot! Contributions are welcome and
+     encouraged. Before contributing, please take a moment to review our
+[Contribution Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/
+    CONTRIBUTING.md) for important information on how to contribute to this
+project. If you're unsure about anything or need assistance, don't hesitate to
+reach out to us or open an issue to discuss your ideas. We look forward to your
+contributions! ## License This project is licensed under the MIT License - see
+the [LICENSE](https://github.com/KevKibe/docindex/blob/master/LICENSE) file for
+     details. ## Contact For any enquiries, please reach out to me through
+                             keviinkibe@gmail.com
```

### Comparing `docindex-0.6.0/setup.cfg` & `docindex-0.7.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = docindex
 author = Kevin Kibe
-version = 0.6.0
+version = 0.7.0
 author_email = keviinkibe@gmail.com
 description = A package for fast persistent storage of multiple document embeddings and their metadata into Pinecone for production-level RAG.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/KevKibe/docindex
 license = MIT
```

### Comparing `docindex-0.6.0/src/_cohere/create_index.py` & `docindex-0.7.0/src/utils/create_index.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from .doc_index import CoherePineconeIndexer
+from _openai.doc_index import OpenaiPineconeIndexer
 import argparse
 
 def parse_args():
-    parser = argparse.ArgumentParser(description="Creates an Index on Pinecone.")
+    parser = argparse.ArgumentParser(description="Create an Index on Pinecone.")
     parser.add_argument("--pinecone_api_key", type=str, help="Pinecone API key")
     parser.add_argument("--index_name", type=str, help="Name of the Pinecone index")
     return parser.parse_args()
 
 
 if __name__ == "__main__":
     args = parse_args()
-    pinecone_indexer = CoherePineconeIndexer(args.index_name, args.pinecone_api_key)
+    pinecone_indexer = OpenaiPineconeIndexer(args.index_name, args.pinecone_api_key)
     pinecone_indexer.create_index()
```

### Comparing `docindex-0.6.0/src/_cohere/delete_index.py` & `docindex-0.7.0/src/utils/delete_index.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from .doc_index import CoherePineconeIndexer
+from _openai.doc_index import OpenaiPineconeIndexer
 import argparse
 
 def parse_args():
-    parser = argparse.ArgumentParser(description="Deletes an Index on Pinecone.")
+    parser = argparse.ArgumentParser(description="Delete an existing Index on Pinecone.")
     parser.add_argument("--pinecone_api_key", type=str, help="Pinecone API key")
     parser.add_argument("--index_name", type=str, help="Name of the Pinecone index")
     return parser.parse_args()
 
 
 if __name__ == "__main__":
     args = parse_args()
-    pinecone_indexer = CoherePineconeIndexer(args.index_name, args.pinecone_api_key)
+    pinecone_indexer = OpenaiPineconeIndexer(args.index_name, args.pinecone_api_key)
     pinecone_indexer.delete_index()
```

### Comparing `docindex-0.6.0/src/_cohere/doc_index.py` & `docindex-0.7.0/src/_cohere/doc_index.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from pinecone import Pinecone, PodSpec
 from tqdm.auto import tqdm
 from uuid import uuid4
 from langchain_community.document_loaders import PyPDFLoader
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 import tiktoken
-from typing import List
-from _openai.doc_model import Page
+from typing import List, Optional
+from utils.doc_model import Page
 from langchain_pinecone import PineconeVectorStore 
 from pathlib import Path
 from langchain_community.document_loaders import UnstructuredWordDocumentLoader
 from langchain_community.document_loaders import UnstructuredMarkdownLoader
 from langchain_community.document_loaders import UnstructuredHTMLLoader
 from langchain_cohere import CohereEmbeddings
-from langchain_community.llms import Cohere
+from langchain_cohere import ChatCohere
 from langchain_core.prompts import PromptTemplate
 from operator import itemgetter
 from utils.config import Config
 from utils.response_model import QueryResult
 from langchain.output_parsers import PydanticOutputParser
+from utils.rerank import RerankerConfig
+from langchain.retrievers import ContextualCompressionRetriever
+
 
 class CoherePineconeIndexer:
     """
     Class for indexing documents to Pinecone using CohereEmbeddings embeddings.
     """
     def __init__(
         self,
@@ -208,39 +211,84 @@
             print(f"Upserting {len(pages_data)} pages to the Pinecone index...")
             self.upsert_documents(pages_data, batch_limit, chunk_size)  
             print("Finished upserting documents for this URL.")
         index = self.pc.Index(self.index_name)
         print(index.describe_index_stats())
         print("Indexing complete.")
 
-    def initialize_vectorstore(self, index_name):
+    def initialize_vectorstore(self, index_name: str) -> PineconeVectorStore:
+        """
+        Initialize a vector store with the given index name.
+
+        Args:
+            index_name (str): The name of the Pinecone index.
+
+        Returns:
+            PineconeVectorStore: Initialized vector store.
+
+        Raises:
+            ValueError: If the index_name is empty or None.
+        """
         index = self.pc.Index(index_name)
         embed = CohereEmbeddings(model="embed-multilingual-v2.0",
                                 cohere_api_key = self.cohere_api_key)
         vectorstore = PineconeVectorStore(index,embed, "text")
         return vectorstore
     
-    def retrieve_and_generate(self,query: str, vector_store: str, model_name: str = 'gpt-3.5-turbo-1106', top_k: int =5):
+    def retrieve_and_generate(
+        self,
+        query: str, 
+        vector_store: str, 
+        top_k: int =3, 
+        rerank_model: str = 'flashrank', 
+        model_type: Optional[str] = None,
+        lang: Optional[str] = None,
+        api_key: Optional[str] = None,
+        api_provider: Optional[str] = None,
+    ) -> QueryResult:
         """
         Retrieve documents from the Pinecone index and generate a response.
+
         Args:
-            query: The query from the user
-            index_name: The name of the Pinecone index
-            model_name: The name of the model to use : defaults to 'gpt-3.5-turbo-1106'
-            top_k: The number of documents to retrieve from the index : defaults to 5
+            query (str): The query from the user.
+            vector_store (str): The name of the Pinecone index.
+            top_k (int, optional): The number of documents to retrieve from the index (default is 3).
+            rerank_model (str, optional): The name or path of the model to use for ranking (default is 'flashrank').
+            model_type (str, optional): The type of the model (e.g., 'cross-encoder', 'flashrank', 't5', etc.).
+            lang (str, optional): The language for multilingual models.
+            api_key (str, optional): The API key for models accessed through an API.
+            api_provider (str, optional): The provider of the API.
+
+        Returns:
+            QueryResult: A Pydantic model representing the generated response.
+
+        Raises:
+            ValueError: If an unsupported model_type is provided.
         """
-        llm = Cohere(model="command", cohere_api_key = self.cohere_api_key)
+        llm = ChatCohere(model="command", cohere_api_key = self.cohere_api_key)
         parser = PydanticOutputParser(pydantic_object=QueryResult)
         rag_prompt = PromptTemplate(template = Config.template_str, 
                                     input_variables = ["query", "context"],
                                     partial_variables={"format_instructions": parser.get_format_instructions()})
-        retriever = vector_store.as_retriever(search_kwargs = {"k": top_k})
+        retriever = vector_store.as_retriever()
+        ranker = RerankerConfig.get_ranker(
+            rerank_model, 
+            model_type, 
+            lang, 
+            api_key, 
+            api_provider
+        )
+        compressor = ranker.as_langchain_compressor(k=top_k)
+        compression_retriever = ContextualCompressionRetriever(
+            base_compressor=compressor, 
+            base_retriever=retriever
+        )
         
         rag_chain = (
-            {"context": itemgetter("query")| retriever,
+            {"context": itemgetter("query")| compression_retriever,
             "query": itemgetter("query"),
             }
             | rag_prompt
             | llm
             | parser
         )
```

### Comparing `docindex-0.6.0/src/_cohere/index_documents.py` & `docindex-0.7.0/src/_cohere/index_documents.py`

 * *Files identical despite different names*

### Comparing `docindex-0.6.0/src/_google/doc_index.py` & `docindex-0.7.0/src/_google/doc_index.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from pinecone import Pinecone, PodSpec
 from tqdm.auto import tqdm
 from uuid import uuid4
 from langchain_community.document_loaders import PyPDFLoader
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain_google_genai import GoogleGenerativeAIEmbeddings
 import tiktoken
-from typing import List
-from _openai.doc_model import Page
+from typing import List, Optional
+from utils.doc_model import Page
 import google.generativeai as genai
 from pathlib import Path
 from langchain_community.document_loaders import UnstructuredWordDocumentLoader
 from langchain_community.document_loaders import UnstructuredMarkdownLoader
 from langchain_community.document_loaders import UnstructuredHTMLLoader
 from langchain_pinecone import PineconeVectorStore
 from langchain_core.prompts import PromptTemplate
 from operator import itemgetter
 from langchain_google_genai import ChatGoogleGenerativeAI
 from utils.config import Config
 from utils.response_model import QueryResult
 from langchain.output_parsers import PydanticOutputParser
+from utils.rerank import RerankerConfig
+from langchain.retrievers import ContextualCompressionRetriever
 
 class GooglePineconeIndexer:
     """
     Class for indexing documents to Pinecone using GoogleGenerativeAIEmbeddings embeddings.
     """
     def __init__(
         self,
         index_name: str,
-        pinecone_api_key: str,
-        google_api_key: str
+        pinecone_api_key: str = None,
+        google_api_key: str = None
     ) -> None:
         """
         Initialize the GoogleGenerativeAIEmbeddings object.
 
         Args:
             index_name (str): Name of the Pinecone index.
             pinecone_api_key (str): Pinecone API key.
@@ -219,42 +221,87 @@
             print(f"Upserting {len(pages_data)} pages to the Pinecone index...")
             self.upsert_documents(pages_data, batch_limit, chunk_size)  
             print("Finished upserting documents for this URL.")
         index = self.pc.Index(self.index_name)
         print(index.describe_index_stats())
         print("Indexing complete.")
 
-    def initialize_vectorstore(self, index_name):
+    def initialize_vectorstore(self, index_name: str) -> PineconeVectorStore:
+        """
+        Initialize a vector store with the given index name.
+
+        Args:
+            index_name (str): The name of the Pinecone index.
+
+        Returns:
+            PineconeVectorStore: Initialized vector store.
+
+        Raises:
+            ValueError: If the index_name is empty or None.
+        """
         index = self.pc.Index(index_name)
         embed = GoogleGenerativeAIEmbeddings(
                 model="models/embedding-001", 
                 google_api_key=self.google_api_key
                 )
         vectorstore = PineconeVectorStore(index, embed, "text")
         return vectorstore
 
 
-    def retrieve_and_generate(self,query: str, vector_store: str, model_name: str = 'gemini-pro', top_k: int =5):
+    def retrieve_and_generate(
+        self,
+        query: str, 
+        vector_store: str, 
+        top_k: int =3, 
+        rerank_model: str = 'flashrank', 
+        model_type: Optional[str] = None,
+        lang: Optional[str] = None,
+        api_key: Optional[str] = None,
+        api_provider: Optional[str] = None,
+    ) -> QueryResult:
         """
         Retrieve documents from the Pinecone index and generate a response.
+
         Args:
-            query: The qury from the user
-            index_name: The name of the Pinecone index
-            model_name: The name of the model to use : defaults to 'gemini-pro'
-            top_k: The number of documents to retrieve from the index : defaults to 5
+            query (str): The query from the user.
+            vector_store (str): The name of the Pinecone index.
+            top_k (int, optional): The number of documents to retrieve from the index (default is 3).
+            rerank_model (str, optional): The name or path of the model to use for ranking (default is 'flashrank').
+            model_type (str, optional): The type of the model (e.g., 'cross-encoder', 'flashrank', 't5', etc.).
+            lang (str, optional): The language for multilingual models.
+            api_key (str, optional): The API key for models accessed through an API.
+            api_provider (str, optional): The provider of the API.
+
+        Returns:
+            QueryResult: A Pydantic model representing the generated response.
+
+        Raises:
+            ValueError: If an unsupported model_type is provided.
         """
         llm = ChatGoogleGenerativeAI(model = Config.default_google_model, google_api_key=self.google_api_key)
         parser = PydanticOutputParser(pydantic_object=QueryResult)
         rag_prompt = PromptTemplate(template = Config.template_str, 
                                     input_variables = ["query", "context"],
                                     partial_variables={"format_instructions": parser.get_format_instructions()})
-        retriever = vector_store.as_retriever(search_kwargs = {"k": top_k})
+        retriever = vector_store.as_retriever()
+        ranker = RerankerConfig.get_ranker(
+            rerank_model, 
+            model_type, 
+            lang, 
+            api_key, 
+            api_provider
+        )
+        compressor = ranker.as_langchain_compressor(k=top_k)
+        compression_retriever = ContextualCompressionRetriever(
+            base_compressor=compressor, 
+            base_retriever=retriever
+        )
         
         rag_chain = (
-            {"context": itemgetter("query")| retriever,
+            {"context": itemgetter("query")| compression_retriever,
             "query": itemgetter("query"),
             }
             | rag_prompt
             | llm
             | parser
         )
```

### Comparing `docindex-0.6.0/src/_google/index_documents.py` & `docindex-0.7.0/src/_google/index_documents.py`

 * *Files identical despite different names*

### Comparing `docindex-0.6.0/src/_openai/doc_index.py` & `docindex-0.7.0/src/_openai/doc_index.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from pinecone import Pinecone, PodSpec
 from tqdm.auto import tqdm
 from uuid import uuid4
 from langchain_community.document_loaders import PyPDFLoader
 from langchain.text_splitter import RecursiveCharacterTextSplitter
 from langchain_openai import OpenAIEmbeddings
 import tiktoken
-from typing import List
-from .doc_model import Page
+from typing import List, Optional
+from utils.doc_model import Page
 from pathlib import Path
 from langchain_community.document_loaders import UnstructuredWordDocumentLoader
 from langchain_community.document_loaders import UnstructuredMarkdownLoader
 from langchain_community.document_loaders import UnstructuredHTMLLoader
 from langchain_pinecone import PineconeVectorStore
 from langchain_core.prompts import PromptTemplate
 from operator import itemgetter
 from langchain_openai import ChatOpenAI
 from utils.config import Config
 from utils.response_model import QueryResult
 from langchain.output_parsers import PydanticOutputParser
+from utils.rerank import RerankerConfig
+from langchain.retrievers import ContextualCompressionRetriever
 
 class OpenaiPineconeIndexer:
     """
     Class for indexing documents to Pinecone using OpenAI embeddings.
     """
     def __init__(
         self,
         index_name: str,
-        pinecone_api_key: str,
-        openai_api_key: str
+        pinecone_api_key: str = None ,
+        openai_api_key: str = None
     ) -> None:
         """
         Initialize the OpenAIPineconeIndexer object.
 
         Args:
             index_name (str): Name of the Pinecone index.
             pinecone_api_key (str): Pinecone API key.
@@ -218,42 +220,87 @@
             self.upsert_documents(pages_data, batch_limit, chunk_size)  
             print("Finished upserting documents for this URL.")
         index = self.pc.Index(self.index_name)
         print(index.describe_index_stats())
         print("Indexing complete.")
         return index
         
-    def initialize_vectorstore(self, index_name):
+    def initialize_vectorstore(self, index_name: str) -> PineconeVectorStore:
+        """
+        Initialize a vector store with the given index name.
+
+        Args:
+            index_name (str): The name of the Pinecone index.
+
+        Returns:
+            PineconeVectorStore: Initialized vector store.
+
+        Raises:
+            ValueError: If the index_name is empty or None.
+        """
         index = self.pc.Index(index_name)
         embed = OpenAIEmbeddings(
                 model = 'text-embedding-ada-002',
                 openai_api_key = self.openai_api_key
                 )
         vectorstore = PineconeVectorStore(index, embed, "text")
         return vectorstore
     
 
-    def retrieve_and_generate(self,query: str, vector_store: str, model_name: str = 'gpt-3.5-turbo-1106', top_k: int =5):
+    def retrieve_and_generate(
+        self,
+        query: str, 
+        vector_store: str, 
+        top_k: int =3, 
+        rerank_model: str = 'flashrank', 
+        model_type: Optional[str] = None,
+        lang: Optional[str] = None,
+        api_key: Optional[str] = None,
+        api_provider: Optional[str] = None,
+    ) -> QueryResult:
         """
         Retrieve documents from the Pinecone index and generate a response.
+
         Args:
-            query: The query from the user
-            index_name: The name of the Pinecone index
-            model_name: The name of the model to use : defaults to 'gpt-3.5-turbo-1106'
-            top_k: The number of documents to retrieve from the index : defaults to 5
+            query (str): The query from the user.
+            vector_store (str): The name of the Pinecone index.
+            top_k (int, optional): The number of documents to retrieve from the index (default is 3).
+            rerank_model (str, optional): The name or path of the model to use for ranking (default is 'flashrank').
+            model_type (str, optional): The type of the model (e.g., 'cross-encoder', 'flashrank', 't5', etc.).
+            lang (str, optional): The language for multilingual models.
+            api_key (str, optional): The API key for models accessed through an API.
+            api_provider (str, optional): The provider of the API.
+
+        Returns:
+            QueryResult: A Pydantic model representing the generated response.
+
+        Raises:
+            ValueError: If an unsupported model_type is provided.
         """
         llm = ChatOpenAI(model = Config.default_openai_model, openai_api_key = self.openai_api_key)
         parser = PydanticOutputParser(pydantic_object=QueryResult)
         rag_prompt = PromptTemplate(template = Config.template_str, 
                                     input_variables = ["query", "context"],
                                     partial_variables={"format_instructions": parser.get_format_instructions()})
-        retriever = vector_store.as_retriever(search_kwargs = {"k": top_k})
-        
+        retriever = vector_store.as_retriever()
+        ranker = RerankerConfig.get_ranker(
+            rerank_model, 
+            model_type, 
+            lang, 
+            api_key, 
+            api_provider
+        )
+        compressor = ranker.as_langchain_compressor(k=top_k)
+        compression_retriever = ContextualCompressionRetriever(
+            base_compressor=compressor, 
+            base_retriever=retriever
+        )
+
         rag_chain = (
-            {"context": itemgetter("query")| retriever,
+            {"context": itemgetter("query")| compression_retriever,
             "query": itemgetter("query"),
             }
             | rag_prompt
             | llm
             | parser
         )
```

### Comparing `docindex-0.6.0/src/_openai/index_documents.py` & `docindex-0.7.0/src/_openai/index_documents.py`

 * *Files identical despite different names*

### Comparing `docindex-0.6.0/src/docindex.egg-info/PKG-INFO` & `docindex-0.7.0/src/docindex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docindex
-Version: 0.6.0
+Version: 0.7.0
 Summary: A package for fast persistent storage of multiple document embeddings and their metadata into Pinecone for production-level RAG.
 Home-page: https://github.com/KevKibe/docindex
 Author: Kevin Kibe
 Author-email: keviinkibe@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -106,15 +106,20 @@
 
 # Initialize the Vectorstore
 vectorstore = pinecone_indexer.initialize_vectorstore(index_name)
 ```
 ### Query and Retrieve Information
 ```python
 query = "what is the transformers architecture"
-response = pinecone_indexer.retrieve_and_generate(vector_store = vectorstore, query = query)
+response = pinecone_indexer.retrieve_and_generate(
+                    vector_store = vectorstore, 
+                    query = query, 
+                    top_k = "number of sources to retrieve",    # Default is 3
+                    rerank_model = "reranking model"            # Default is 'flashrank'  Other models available Docs:https://github.com/AnswerDotAI/rerankers
+                    )
 response
 ```
 
 ### Response
 ```bash
 query='what is the transformers architecture' result='The Transformer follows this overall architecture using stacked self-attention and point-wise, fully-connected layers for both the encoder and decoder, shown in the left and right halves of Figure 1, respectively.' page=1 source_documents=[Document(page_content='Figure 1: The Transformer - model architecture.\nThe Transformer follows this overall architecture using stacked self-attention and point-wise, fully\nconnected layers for both the encoder and decoder, shown in the left and right halves of Figure 1,\nrespectively.\n3.1 Encoder and Decoder Stacks\nEncoder: The encoder is composed of a stack of N= 6 identical layers. Each layer has two\nsub-layers. The first is a multi-head self-attention mechanism, and the second is a simple, position-\nwise fully connected feed-forward network. We employ a residual connection [ 11] around each of\nthe two sub-layers, followed by layer normalization [ 1]. That is, the output of each sub-layer is\nLayerNorm( x+ Sublayer( x)), where Sublayer( x)is the function implemented by the sub-layer\nitself. To facilitate these residual connections, all sub-layers in the model, as well as the embedding\nlayers, produce outputs of dimension dmodel = 512 .\nDecoder: The decoder is also composed of a stack of N= 6identical layers. In addition to the two', source=2.0, title='https://arxiv.org/pdf/1706.03762.pdf')]
 
@@ -163,15 +168,15 @@
 ```bash
 cd src
 ```
 - To create an index
 
 ```bash
 # Using OpenAI 
-python -m  _openai.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" -
+python -m  utils.create_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" 
 
 ```
 
 - Run the command to start indexing the documents
 
 ```bash
 # Using OpenAI
@@ -187,15 +192,15 @@
 python -m _cohere.index_documents   --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --cohere_api_key "your_google_api_key" --batch_limit "batch-limit" --docs  "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-size"
 
 ```
 - To delete an index
 
 ```bash
 # Using OpenAI 
-python -m  _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" 
+python -m  utils.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" 
 
 ```
 
 ## Contributing 
 🌟 First consider giving it a star at the top right. It means a lot!
 Contributions are welcome and encouraged.
 Before contributing, please take a moment to review our [Contribution Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for important information on how to contribute to this project.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: docindex Version: 0.6.0 Summary: A package for fast
+Metadata-Version: 2.1 Name: docindex Version: 0.7.0 Summary: A package for fast
 persistent storage of multiple document embeddings and their metadata into
 Pinecone for production-level RAG. Home-page: https://github.com/KevKibe/
 docindex Author: Kevin Kibe Author-email: keviinkibe@gmail.com License: MIT
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: pinecone-client==3.2.2 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: pypdf==4.1.0 Requires-Dist: unstructured==0.12.6 Requires-Dist:
 langchain-community==0.0.31 Requires-Dist: langchain==0.1.14 Requires-Dist:
@@ -55,66 +55,69 @@
   CoherePineconeIndexer(index_name, pinecone_api_key, cohere_api_key) # Using
   Cohere # To create a new Index pinecone_indexer.create_index() # Store the
           document embeddings with the specified URLs and batch limit
 pinecone_indexer.index_documents(urls,batch_limit,chunk_size) # Initialize the
  Vectorstore vectorstore = pinecone_indexer.initialize_vectorstore(index_name)
      ``` ### Query and Retrieve Information ```python query = "what is the
  transformers architecture" response = pinecone_indexer.retrieve_and_generate
- (vector_store = vectorstore, query = query) response ``` ### Response ```bash
- query='what is the transformers architecture' result='The Transformer follows
- this overall architecture using stacked self-attention and point-wise, fully-
-connected layers for both the encoder and decoder, shown in the left and right
-     halves of Figure 1, respectively.' page=1 source_documents=[Document
-(page_content='Figure 1: The Transformer - model architecture.\nThe Transformer
-follows this overall architecture using stacked self-attention and point-wise,
-fully\nconnected layers for both the encoder and decoder, shown in the left and
-       right halves of Figure 1,\nrespectively.\n3.1 Encoder and Decoder
- Stacks\nEncoder: The encoder is composed of a stack of N= 6 identical layers.
-   Each layer has two\nsub-layers. The first is a multi-head self-attention
- mechanism, and the second is a simple, position-\nwise fully connected feed-
-forward network. We employ a residual connection [ 11] around each of\nthe two
- sub-layers, followed by layer normalization [ 1]. That is, the output of each
- sub-layer is\nLayerNorm( x+ Sublayer( x)), where Sublayer( x)is the function
-implemented by the sub-layer\nitself. To facilitate these residual connections,
-all sub-layers in the model, as well as the embedding\nlayers, produce outputs
- of dimension dmodel = 512 .\nDecoder: The decoder is also composed of a stack
- of N= 6identical layers. In addition to the two', source=2.0, title='https://
- arxiv.org/pdf/1706.03762.pdf')] ``` ### Query Response Attributes: ```python
- response.query # The query that was submitted response.result # The result of
- the query, including any retrieved information. response.source_documents # A
-list of source documents related to the query. response.sources # A list of the
- sources (page numbers) from the source documents. response.titles # A list of
- the titles from the source documents. response.page_contents # A list of the
- page contents from the source documents. ``` ### Delete Index: ```python # To
-delete the created Index pinecone_indexer.delete_index() ``` ## Using the CLI -
-  Clone the Repository: Clone or download the application code to your local
-machine. ```bash git clone https://github.com/KevKibe/docindex.git ``` - Create
- a virtual environment for the project and activate it. ```bash # Navigate to
+  ( vector_store = vectorstore, query = query, top_k = "number of sources to
+    retrieve", # Default is 3 rerank_model = "reranking model" # Default is
+    'flashrank' Other models available Docs:https://github.com/AnswerDotAI/
+ rerankers ) response ``` ### Response ```bash query='what is the transformers
+ architecture' result='The Transformer follows this overall architecture using
+  stacked self-attention and point-wise, fully-connected layers for both the
+     encoder and decoder, shown in the left and right halves of Figure 1,
+ respectively.' page=1 source_documents=[Document(page_content='Figure 1: The
+    Transformer - model architecture.\nThe Transformer follows this overall
+  architecture using stacked self-attention and point-wise, fully\nconnected
+layers for both the encoder and decoder, shown in the left and right halves of
+Figure 1,\nrespectively.\n3.1 Encoder and Decoder Stacks\nEncoder: The encoder
+   is composed of a stack of N= 6 identical layers. Each layer has two\nsub-
+layers. The first is a multi-head self-attention mechanism, and the second is a
+   simple, position-\nwise fully connected feed-forward network. We employ a
+residual connection [ 11] around each of\nthe two sub-layers, followed by layer
+  normalization [ 1]. That is, the output of each sub-layer is\nLayerNorm( x+
+   Sublayer( x)), where Sublayer( x)is the function implemented by the sub-
+layer\nitself. To facilitate these residual connections, all sub-layers in the
+model, as well as the embedding\nlayers, produce outputs of dimension dmodel =
+   512 .\nDecoder: The decoder is also composed of a stack of N= 6identical
+  layers. In addition to the two', source=2.0, title='https://arxiv.org/pdf/
+1706.03762.pdf')] ``` ### Query Response Attributes: ```python response.query #
+    The query that was submitted response.result # The result of the query,
+  including any retrieved information. response.source_documents # A list of
+source documents related to the query. response.sources # A list of the sources
+   (page numbers) from the source documents. response.titles # A list of the
+ titles from the source documents. response.page_contents # A list of the page
+contents from the source documents. ``` ### Delete Index: ```python # To delete
+the created Index pinecone_indexer.delete_index() ``` ## Using the CLI - Clone
+ the Repository: Clone or download the application code to your local machine.
+   ```bash git clone https://github.com/KevKibe/docindex.git ``` - Create a
+  virtual environment for the project and activate it. ```bash # Navigate to
 project repository cd docindex # create virtual environment python -m venv venv
      # activate virtual environment source venv/bin/activate ``` - Install
  dependencies by running this command ```bash pip install -r requirements.txt
  ``` - Navigate to src ```bash cd src ``` - To create an index ```bash # Using
-           OpenAI python -m _openai.create_index --pinecone_api_key
-"your_pinecone_api_key" --index_name "your_index_name" - ``` - Run the command
-        to start indexing the documents ```bash # Using OpenAI python -
-    m _openai.index_documents --pinecone_api_key "your_pinecone_api_key" --
-    index_name "your_index_name" --openai_api_key "your_openai_api_key" --
- batch_limit "batch-limit" --docs "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-
-    size" # Using Google Generative AI python -m _google.index_documents --
+OpenAI python -m utils.create_index --pinecone_api_key "your_pinecone_api_key"
+  --index_name "your_index_name" ``` - Run the command to start indexing the
+     documents ```bash # Using OpenAI python -m _openai.index_documents --
   pinecone_api_key "your_pinecone_api_key" --index_name "your_index_name" --
- google_api_key "your_google_api_key" --batch_limit "batch-limit" --docs "doc-
-      1.pdf" "doc-2.pdf' --chunk_size "chunk-size" Using Cohere python -
-    m _cohere.index_documents --pinecone_api_key "your_pinecone_api_key" --
-    index_name "your_index_name" --cohere_api_key "your_google_api_key" --
+ openai_api_key "your_openai_api_key" --batch_limit "batch-limit" --docs "doc-
+   1.pdf" "doc-2.pdf' --chunk_size "chunk-size" # Using Google Generative AI
+python -m _google.index_documents --pinecone_api_key "your_pinecone_api_key" --
+    index_name "your_index_name" --google_api_key "your_google_api_key" --
  batch_limit "batch-limit" --docs "doc-1.pdf" "doc-2.pdf' --chunk_size "chunk-
-        size" ``` - To delete an index ```bash # Using OpenAI python -
-m _openai.delete_index --pinecone_api_key "your_pinecone_api_key" --index_name
- "your_index_name" ``` ## Contributing ð First consider giving it a star at
-the top right. It means a lot! Contributions are welcome and encouraged. Before
-  contributing, please take a moment to review our [Contribution Guidelines]
-  (https://github.com/KevKibe/docindex/blob/master/DOCS/CONTRIBUTING.md) for
- important information on how to contribute to this project. If you're unsure
-about anything or need assistance, don't hesitate to reach out to us or open an
-issue to discuss your ideas. We look forward to your contributions! ## License
-  This project is licensed under the MIT License - see the [LICENSE](https://
- github.com/KevKibe/docindex/blob/master/LICENSE) file for details. ## Contact
-    For any enquiries, please reach out to me through keviinkibe@gmail.com
+    size" Using Cohere python -m _cohere.index_documents --pinecone_api_key
+    "your_pinecone_api_key" --index_name "your_index_name" --cohere_api_key
+  "your_google_api_key" --batch_limit "batch-limit" --docs "doc-1.pdf" "doc-
+   2.pdf' --chunk_size "chunk-size" ``` - To delete an index ```bash # Using
+OpenAI python -m utils.delete_index --pinecone_api_key "your_pinecone_api_key"
+ --index_name "your_index_name" ``` ## Contributing ð First consider giving
+   it a star at the top right. It means a lot! Contributions are welcome and
+     encouraged. Before contributing, please take a moment to review our
+[Contribution Guidelines](https://github.com/KevKibe/docindex/blob/master/DOCS/
+    CONTRIBUTING.md) for important information on how to contribute to this
+project. If you're unsure about anything or need assistance, don't hesitate to
+reach out to us or open an issue to discuss your ideas. We look forward to your
+contributions! ## License This project is licensed under the MIT License - see
+the [LICENSE](https://github.com/KevKibe/docindex/blob/master/LICENSE) file for
+     details. ## Contact For any enquiries, please reach out to me through
+                             keviinkibe@gmail.com
```

### Comparing `docindex-0.6.0/src/docindex.egg-info/SOURCES.txt` & `docindex-0.7.0/src/docindex.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/_cohere/__init__.py
-src/_cohere/config.py
-src/_cohere/create_index.py
-src/_cohere/delete_index.py
 src/_cohere/doc_index.py
-src/_cohere/doc_model.py
 src/_cohere/index_documents.py
 src/_google/__init__.py
-src/_google/config.py
-src/_google/create_index.py
-src/_google/delete_index.py
 src/_google/doc_index.py
 src/_google/index_documents.py
 src/_openai/__init__.py
-src/_openai/create_index.py
-src/_openai/delete_index.py
 src/_openai/doc_index.py
-src/_openai/doc_model.py
 src/_openai/index_documents.py
 src/docindex.egg-info/PKG-INFO
 src/docindex.egg-info/SOURCES.txt
 src/docindex.egg-info/dependency_links.txt
 src/docindex.egg-info/requires.txt
 src/docindex.egg-info/top_level.txt
 src/tests/__init__.py
 src/tests/cohereindex_test.py
 src/tests/googleindex_test.py
 src/tests/openaiindex_test.py
 src/utils/__init__.py
 src/utils/config.py
+src/utils/create_index.py
+src/utils/delete_index.py
+src/utils/doc_model.py
+src/utils/rerank.py
 src/utils/response_model.py
```

### Comparing `docindex-0.6.0/src/tests/cohereindex_test.py` & `docindex-0.7.0/src/tests/cohereindex_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,17 +54,21 @@
         vectorstore = self.indexer.initialize_vectorstore(self.index_name)
         self.assertIsInstance(vectorstore, PineconeVectorStore)
 
     # def test_04_retrieve_and_generate(self):
     #     """
     #     Test initializing the vector store and assert its type.
     #     """
-    #     response = self.indexer.retrieve_and_generate(query = "what is the title of the document",
-    #                                                   index_name= self.index_name
-    #                                                   )
+    #     vector_store = self.indexer.initialize_vectorstore(self.index_name)
+    #     response = self.indexer.retrieve_and_generate(
+    #         query = "give a short summary of the introduction",
+    #         vector_store = vector_store,
+    #         top_k = 3,
+    #         rerank_model = "t5"
+    #         )
     #     print(response)
     #     self.assertIsNotNone(response, "The retriever response should not be None.")
 
     @patch('sys.stdout', new_callable=StringIO)
     def test_05_delete_index(self, mock_stdout):
         """
         Test deleting an index and assert the output.
```

### Comparing `docindex-0.6.0/src/tests/googleindex_test.py` & `docindex-0.7.0/src/tests/openaiindex_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import unittest
-from _google.doc_index import GooglePineconeIndexer
+from _openai.doc_index import OpenaiPineconeIndexer
 import os 
 from io import StringIO
 from unittest.mock import patch
 import pinecone
 from langchain_pinecone import PineconeVectorStore 
 from dotenv import load_dotenv
 load_dotenv()
 
-
-class TestGooglePineconeIndexer(unittest.TestCase):
+class TestOpenaiPineconeIndexer(unittest.TestCase):
     """
-    Test case class for the GooglePineconeIndexer.
+    Test case class for the OpenaiPineconeIndexer.
     """
 
     def setUp(self):
         """
         Set up the test case with common attributes.
         """
         self.index_name = "new-index-1"
         self.pinecone_api_key = os.environ.get('PINECONE_API_KEY')
-        self.google_api_key = os.environ.get('GOOGLE_API_KEY')
-        self.indexer = GooglePineconeIndexer(self.index_name, self.pinecone_api_key, self.google_api_key)
+        self.openai_api_key = os.environ.get('OPENAI_API_KEY')
+        self.indexer = OpenaiPineconeIndexer(self.index_name, self.pinecone_api_key, self.openai_api_key)
         return super().setUp()
     
     @patch('sys.stdout', new_callable=StringIO)
     def test_01_create_index(self, mock_stdout):
         """
         Test creating an index and assert the output.
         """
@@ -59,19 +58,21 @@
         vectorstore = self.indexer.initialize_vectorstore(self.index_name)
         self.assertIsInstance(vectorstore, PineconeVectorStore)
 
     def test_04_retrieve_and_generate(self):
         """
         Test initializing the vector store and assert its type.
         """
-        vector_store = self.indexer.initialize_vectorstore(self.index_name)
-        response = self.indexer.retrieve_and_generate(query = "give a short summary of the introduction",
-                                                      vector_store= vector_store
-                                                      )
-        print(response)
+        vectorstore = self.indexer.initialize_vectorstore(self.index_name)
+        response = self.indexer.retrieve_and_generate(
+            query = "give a short summary of the introduction",
+            vector_store = vectorstore,
+            top_k = 3,
+            rerank_model = "t5"
+            )
         self.assertIsNotNone(response, "The retriever response should not be None.")
 
     @patch('sys.stdout', new_callable=StringIO)
     def test_05_delete_index(self, mock_stdout):
         """
         Test deleting an index and assert the output.
         """
@@ -87,9 +88,9 @@
     def sort_test_methods(cls, testCaseClass, testCaseNames):
         """
         Sort test methods for better readability.
         """
         return sorted(testCaseNames)
 
 if __name__ == "__main__":
-    unittest.TestLoader.sortTestMethodsUsing = TestGooglePineconeIndexer.sort_test_methods
+    unittest.TestLoader.sortTestMethodsUsing = TestOpenaiPineconeIndexer.sort_test_methods
     unittest.main()
```

### Comparing `docindex-0.6.0/src/tests/openaiindex_test.py` & `docindex-0.7.0/src/tests/googleindex_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import unittest
-from _openai.doc_index import OpenaiPineconeIndexer
+from _google.doc_index import GooglePineconeIndexer
 import os 
 from io import StringIO
 from unittest.mock import patch
 import pinecone
 from langchain_pinecone import PineconeVectorStore 
 from dotenv import load_dotenv
 load_dotenv()
 
-class TestOpenaiPineconeIndexer(unittest.TestCase):
+
+class TestGooglePineconeIndexer(unittest.TestCase):
     """
-    Test case class for the OpenaiPineconeIndexer.
+    Test case class for the GooglePineconeIndexer.
     """
 
     def setUp(self):
         """
         Set up the test case with common attributes.
         """
         self.index_name = "new-index-1"
         self.pinecone_api_key = os.environ.get('PINECONE_API_KEY')
-        self.openai_api_key = os.environ.get('OPENAI_API_KEY')
-        self.indexer = OpenaiPineconeIndexer(self.index_name, self.pinecone_api_key, self.openai_api_key)
+        self.google_api_key = os.environ.get('GOOGLE_API_KEY')
+        self.indexer = GooglePineconeIndexer(self.index_name, self.pinecone_api_key, self.google_api_key)
         return super().setUp()
     
     @patch('sys.stdout', new_callable=StringIO)
     def test_01_create_index(self, mock_stdout):
         """
         Test creating an index and assert the output.
         """
@@ -54,23 +55,27 @@
     def test_03_initialize_vectorstore(self):
         """
         Test initializing the vector store and assert its type.
         """
         vectorstore = self.indexer.initialize_vectorstore(self.index_name)
         self.assertIsInstance(vectorstore, PineconeVectorStore)
 
-    def test_04_retrieve_and_generate(self):
-        """
-        Test initializing the vector store and assert its type.
-        """
-        vectorstore = self.indexer.initialize_vectorstore(self.index_name)
-        response = self.indexer.retrieve_and_generate(query = "give a short summary of the introduction",
-                                                      vector_store = vectorstore
-                                                      )
-        self.assertIsNotNone(response, "The retriever response should not be None.")
+    # def test_04_retrieve_and_generate(self):
+    #     """
+    #     Test initializing the vector store and assert its type.
+    #     """
+    #     vector_store = self.indexer.initialize_vectorstore(self.index_name)
+    #     response = self.indexer.retrieve_and_generate(
+    #         query = "tell me something from the context texts",
+    #         vector_store = vector_store,
+    #         top_k = 3,
+    #         rerank_model = "t5"
+    #         )
+    #     print(response)
+    #     self.assertIsNotNone(response, "The retriever response should not be None.")
 
     @patch('sys.stdout', new_callable=StringIO)
     def test_05_delete_index(self, mock_stdout):
         """
         Test deleting an index and assert the output.
         """
         self.indexer.delete_index()
@@ -85,9 +90,9 @@
     def sort_test_methods(cls, testCaseClass, testCaseNames):
         """
         Sort test methods for better readability.
         """
         return sorted(testCaseNames)
 
 if __name__ == "__main__":
-    unittest.TestLoader.sortTestMethodsUsing = TestOpenaiPineconeIndexer.sort_test_methods
+    unittest.TestLoader.sortTestMethodsUsing = TestGooglePineconeIndexer.sort_test_methods
     unittest.main()
```

### Comparing `docindex-0.6.0/src/utils/response_model.py` & `docindex-0.7.0/src/utils/response_model.py`

 * *Files identical despite different names*

