# Comparing `tmp/lavague_core-0.1.1.tar.gz` & `tmp/lavague_core-0.1.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_core-0.1.1.tar", max compression
+gzip compressed data, was "lavague_core-0.1.1.post1.tar", max compression
```

## Comparing `lavague_core-0.1.1.tar` & `lavague_core-0.1.1.post1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-05-15 19:17:05.210186 lavague_core-0.1.1/LICENSE
--rw-r--r--   0        0        0        0 2024-05-15 19:17:05.210186 lavague_core-0.1.1/README.md
--rw-r--r--   0        0        0      993 2024-05-15 19:20:55.646558 lavague_core-0.1.1/lavague/core/__init__.py
--rw-r--r--   0        0        0     4084 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/action_engine.py
--rw-r--r--   0        0        0     5556 2024-05-15 20:57:47.605949 lavague_core-0.1.1/lavague/core/agents.py
--rw-r--r--   0        0        0     2778 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/base_driver.py
--rw-r--r--   0        0        0     1896 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/context.py
--rw-r--r--   0        0        0     1296 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/extractors.py
--rw-r--r--   0        0        0      613 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/prompt_templates.py
--rw-r--r--   0        0        0    12118 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/retrievers.py
--rw-r--r--   0        0        0     3793 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/utilities/format_utils.py
--rw-r--r--   0        0        0     3561 2024-05-15 20:58:35.889500 lavague_core-0.1.1/lavague/core/utilities/telemetry.py
--rw-r--r--   0        0        0     1361 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/utilities/version_checker.py
--rw-r--r--   0        0        0      491 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/utilities/web_utils.py
--rw-r--r--   0        0        0     3445 2024-05-15 19:17:05.210186 lavague_core-0.1.1/lavague/core/world_model.py
--rw-r--r--   0        0        0     1080 2024-05-15 19:17:05.210186 lavague_core-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 lavague_core-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-15 19:17:05.210186 lavague_core-0.1.1.post1/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-15 19:17:05.210186 lavague_core-0.1.1.post1/README.md
+-rw-r--r--   0        0        0      993 2024-05-15 19:20:55.646558 lavague_core-0.1.1.post1/lavague/core/__init__.py
+-rw-r--r--   0        0        0     4084 2024-05-15 21:37:00.070840 lavague_core-0.1.1.post1/lavague/core/action_engine.py
+-rw-r--r--   0        0        0     5556 2024-05-15 20:57:47.605949 lavague_core-0.1.1.post1/lavague/core/agents.py
+-rw-r--r--   0        0        0     2778 2024-05-15 19:17:05.210186 lavague_core-0.1.1.post1/lavague/core/base_driver.py
+-rw-r--r--   0        0        0     1896 2024-05-15 19:17:05.210186 lavague_core-0.1.1.post1/lavague/core/context.py
+-rw-r--r--   0        0        0     1296 2024-05-15 19:17:05.210186 lavague_core-0.1.1.post1/lavague/core/extractors.py
+-rw-r--r--   0        0        0      613 2024-05-15 19:17:05.210186 lavague_core-0.1.1.post1/lavague/core/prompt_templates.py
+-rw-r--r--   0        0        0    12117 2024-05-15 21:36:55.702887 lavague_core-0.1.1.post1/lavague/core/retrievers.py
+-rw-r--r--   0        0        0     3793 2024-05-15 19:17:05.210186 lavague_core-0.1.1.post1/lavague/core/utilities/format_utils.py
+-rw-r--r--   0        0        0     3561 2024-05-15 20:58:35.889500 lavague_core-0.1.1.post1/lavague/core/utilities/telemetry.py
+-rw-r--r--   0        0        0     1361 2024-05-15 19:17:05.210186 lavague_core-0.1.1.post1/lavague/core/utilities/version_checker.py
+-rw-r--r--   0        0        0      491 2024-05-15 19:17:05.210186 lavague_core-0.1.1.post1/lavague/core/utilities/web_utils.py
+-rw-r--r--   0        0        0     3445 2024-05-15 19:17:05.210186 lavague_core-0.1.1.post1/lavague/core/world_model.py
+-rw-r--r--   0        0        0     1086 2024-05-15 21:38:39.577751 lavague_core-0.1.1.post1/pyproject.toml
+-rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 lavague_core-0.1.1.post1/PKG-INFO
```

### Comparing `lavague_core-0.1.1/LICENSE` & `lavague_core-0.1.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.1/lavague/core/__init__.py` & `lavague_core-0.1.1.post1/lavague/core/__init__.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.1/lavague/core/action_engine.py` & `lavague_core-0.1.1.post1/lavague/core/action_engine.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.1/lavague/core/agents.py` & `lavague_core-0.1.1.post1/lavague/core/agents.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.1/lavague/core/base_driver.py` & `lavague_core-0.1.1.post1/lavague/core/base_driver.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.1/lavague/core/context.py` & `lavague_core-0.1.1.post1/lavague/core/context.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.1/lavague/core/extractors.py` & `lavague_core-0.1.1.post1/lavague/core/extractors.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.1/lavague/core/prompt_templates.py` & `lavague_core-0.1.1.post1/lavague/core/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.1/lavague/core/retrievers.py` & `lavague_core-0.1.1.post1/lavague/core/retrievers.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ):
         self.html_retriever = html_retriever
         self.driver = driver
         self.embedding = embedding
         super().__init__()
 
     def _retrieve(self, query_bundle: QueryBundle) -> List[NodeWithScore]:
-        return self.html_retriever._retrieve_html(
+        return self.html_retriever.retrieve_html(
             self.driver, self.embedding, query_bundle
         )
 
 
 class BaseHtmlRetriever(ABC):
     @abstractmethod
     def retrieve_html(
```

### Comparing `lavague_core-0.1.1/lavague/core/utilities/format_utils.py` & `lavague_core-0.1.1.post1/lavague/core/utilities/format_utils.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.1/lavague/core/utilities/telemetry.py` & `lavague_core-0.1.1.post1/lavague/core/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.1/lavague/core/utilities/version_checker.py` & `lavague_core-0.1.1.post1/lavague/core/utilities/version_checker.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.1/lavague/core/world_model.py` & `lavague_core-0.1.1.post1/lavague/core/world_model.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.1/pyproject.toml` & `lavague_core-0.1.1.post1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry]
 name = "lavague-core"
-version = "0.1.1"
+version = "0.1.1-post1"
 description = "automation code generation from text instructions"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
@@ -25,10 +25,10 @@
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
 llama-index = "^0.10.19"
 llama-index-retrievers-bm25 = "^0.1.3"
 lxml = "^5.2.2"
 langchain = "^0.1.20"
-ipython = "^8.24.0"
+ipython = "^7.34.0"
 msgpack = "^1.0.8"
```

### Comparing `lavague_core-0.1.1/PKG-INFO` & `lavague_core-0.1.1.post1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-core
-Version: 0.1.1
+Version: 0.1.1.post1
 Summary: automation code generation from text instructions
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: ipython (>=8.24.0,<9.0.0)
+Requires-Dist: ipython (>=7.34.0,<8.0.0)
 Requires-Dist: langchain (>=0.1.20,<0.2.0)
 Requires-Dist: llama-index (>=0.10.19,<0.11.0)
 Requires-Dist: llama-index-retrievers-bm25 (>=0.1.3,<0.2.0)
 Requires-Dist: lxml (>=5.2.2,<6.0.0)
 Requires-Dist: msgpack (>=1.0.8,<2.0.0)
 Project-URL: Documentation, https://docs.lavague.ai/en/latest/
 Project-URL: Repository, https://github.com/lavague-ai/LaVague/
```

