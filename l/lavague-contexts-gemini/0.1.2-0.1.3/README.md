# Comparing `tmp/lavague_contexts_gemini-0.1.2.tar.gz` & `tmp/lavague_contexts_gemini-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_contexts_gemini-0.1.2.tar", max compression
+gzip compressed data, was "lavague_contexts_gemini-0.1.3.tar", max compression
```

## Comparing `lavague_contexts_gemini-0.1.2.tar` & `lavague_contexts_gemini-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0       32 2024-05-16 06:05:44.166686 lavague_contexts_gemini-0.1.2/README.md
--rw-r--r--   0        0        0       55 2024-05-16 13:32:16.934421 lavague_contexts_gemini-0.1.2/lavague/contexts/gemini/__init__.py
--rw-r--r--   0        0        0     1779 2024-05-16 13:39:16.851328 lavague_contexts_gemini-0.1.2/lavague/contexts/gemini/base.py
--rw-r--r--   0        0        0     9165 2024-05-16 13:39:41.954150 lavague_contexts_gemini-0.1.2/lavague/contexts/gemini/base_mml.py
--rw-r--r--   0        0        0     1108 2024-05-16 13:37:37.958595 lavague_contexts_gemini-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 lavague_contexts_gemini-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       32 2024-05-16 06:05:44.166686 lavague_contexts_gemini-0.1.3/README.md
+-rw-r--r--   0        0        0       55 2024-05-16 21:10:23.639638 lavague_contexts_gemini-0.1.3/lavague/contexts/gemini/__init__.py
+-rw-r--r--   0        0        0     1738 2024-05-16 21:10:10.906372 lavague_contexts_gemini-0.1.3/lavague/contexts/gemini/base.py
+-rw-r--r--   0        0        0     1108 2024-05-16 20:09:27.326208 lavague_contexts_gemini-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 lavague_contexts_gemini-0.1.3/PKG-INFO
```

### Comparing `lavague_contexts_gemini-0.1.2/lavague/contexts/gemini/base.py` & `lavague_contexts_gemini-0.1.3/lavague/contexts/gemini/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from lavague.core import (
     OpsmSplitRetriever,
     DefaultPromptTemplate,
     PythonFromMarkdownExtractor,
     Context,
     get_default_context,
 )
-from .base_mml import GeminiMultiModal2
 from lavague.core.extractors import BaseExtractor
 from lavague.core.retrievers import BaseHtmlRetriever
 from lavague.core.context import DEFAULT_MAX_TOKENS, DEFAULT_TEMPERATURE
 
 
 class GeminiContext(Context):
     def __init__(
@@ -36,13 +35,13 @@
         return super().__init__(
             Gemini(
                 api_key=api_key,
                 model_name=llm,
                 max_tokens=DEFAULT_MAX_TOKENS,
                 temperature=DEFAULT_TEMPERATURE,
             ),
-            GeminiMultiModal2(api_key=api_key, model_name=mm_llm),
+            GeminiMultiModal(api_key=api_key, model_name=mm_llm),
             GeminiEmbedding(api_key=api_key, model_name=embedding),
             retriever,
             prompt_template,
             extractor,
         )
```

### Comparing `lavague_contexts_gemini-0.1.2/pyproject.toml` & `lavague_contexts_gemini-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-contexts-gemini"
-version = "0.1.2"
+version = "0.1.3"
 description = "gemini integration for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
@@ -18,15 +18,15 @@
 repository = "https://github.com/lavague-ai/LaVague/"
 documentation = "https://docs.lavague.ai/en/latest/"
 packages = [{include = "lavague/"}]
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
 lavague-core = "^0.1.1"
-llama-index-llms-gemini = "^0.1.7"
+llama-index-llms-gemini = "^0.1.8"
 llama-index-embeddings-gemini = "^0.1.6"
-llama-index-multi-modal-llms-gemini = "^0.1.5"
+llama-index-multi-modal-llms-gemini = "^0.1.6"
 google-generativeai = "^0.4.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `lavague_contexts_gemini-0.1.2/PKG-INFO` & `lavague_contexts_gemini-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-contexts-gemini
-Version: 0.1.2
+Version: 0.1.3
 Summary: gemini integration for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -16,14 +16,14 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: google-generativeai (>=0.4.1,<0.5.0)
 Requires-Dist: lavague-core (>=0.1.1,<0.2.0)
 Requires-Dist: llama-index-embeddings-gemini (>=0.1.6,<0.2.0)
-Requires-Dist: llama-index-llms-gemini (>=0.1.7,<0.2.0)
-Requires-Dist: llama-index-multi-modal-llms-gemini (>=0.1.5,<0.2.0)
+Requires-Dist: llama-index-llms-gemini (>=0.1.8,<0.2.0)
+Requires-Dist: llama-index-multi-modal-llms-gemini (>=0.1.6,<0.2.0)
 Project-URL: Documentation, https://docs.lavague.ai/en/latest/
 Project-URL: Repository, https://github.com/lavague-ai/LaVague/
 Description-Content-Type: text/markdown
 
 # Gemini integration for lavague
```

