# Comparing `tmp/langchain_exa-0.0.1.tar.gz` & `tmp/langchain_exa-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_exa-0.0.1.tar", max compression
+gzip compressed data, was "langchain_exa-0.1.0.tar", max compression
```

## Comparing `langchain_exa-0.0.1.tar` & `langchain_exa-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-01-25 03:59:46.667258 langchain_exa-0.0.1/LICENSE
--rw-r--r--   0        0        0       16 2024-01-25 03:59:46.667888 langchain_exa-0.0.1/README.md
--rw-r--r--   0        0        0      369 2024-01-25 03:59:46.668214 langchain_exa-0.0.1/langchain_exa/__init__.py
--rw-r--r--   0        0        0      573 2024-01-25 03:59:46.668582 langchain_exa-0.0.1/langchain_exa/_utilities.py
--rw-r--r--   0        0        0        0 2024-01-25 03:59:46.668609 langchain_exa-0.0.1/langchain_exa/py.typed
--rw-r--r--   0        0        0     3502 2024-01-25 03:59:46.669212 langchain_exa-0.0.1/langchain_exa/retrievers.py
--rw-r--r--   0        0        0     4424 2024-01-25 03:59:46.669398 langchain_exa-0.0.1/langchain_exa/tools.py
--rw-r--r--   0        0        0     2466 2024-01-25 03:59:46.670310 langchain_exa-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 langchain_exa-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-16 02:18:59.712601 langchain_exa-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1531 2024-05-16 02:18:59.712601 langchain_exa-0.1.0/README.md
+-rw-r--r--   0        0        0      369 2024-05-16 02:18:59.712601 langchain_exa-0.1.0/langchain_exa/__init__.py
+-rw-r--r--   0        0        0      573 2024-05-16 02:18:59.712601 langchain_exa-0.1.0/langchain_exa/_utilities.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:18:59.712601 langchain_exa-0.1.0/langchain_exa/py.typed
+-rw-r--r--   0        0        0     3591 2024-05-16 02:18:59.712601 langchain_exa-0.1.0/langchain_exa/retrievers.py
+-rw-r--r--   0        0        0     4615 2024-05-16 02:18:59.712601 langchain_exa-0.1.0/langchain_exa/tools.py
+-rw-r--r--   0        0        0     2495 2024-05-16 02:18:59.712601 langchain_exa-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2339 1970-01-01 00:00:00.000000 langchain_exa-0.1.0/PKG-INFO
```

### Comparing `langchain_exa-0.0.1/LICENSE` & `langchain_exa-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_exa-0.0.1/langchain_exa/_utilities.py` & `langchain_exa-0.1.0/langchain_exa/_utilities.py`

 * *Files identical despite different names*

### Comparing `langchain_exa-0.0.1/langchain_exa/retrievers.py` & `langchain_exa-0.1.0/langchain_exa/retrievers.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Dict, List, Literal, Optional, Union
 
 from exa_py import Exa  # type: ignore
 from exa_py.api import HighlightsContentsOptions, TextContentsOptions  # type: ignore
 from langchain_core.callbacks import CallbackManagerForRetrieverRun
 from langchain_core.documents import Document
-from langchain_core.pydantic_v1 import SecretStr, root_validator
+from langchain_core.pydantic_v1 import Field, SecretStr, root_validator
 from langchain_core.retrievers import BaseRetriever
 
 from langchain_exa._utilities import initialize_client
 
 
 def _get_metadata(result: Any) -> Dict[str, Any]:
     """Get the metadata from a result object."""
@@ -49,32 +49,32 @@
     type: str = "neural"
     """The type of search, 'keyword' or 'neural'. Default: neural"""
     highlights: Optional[Union[HighlightsContentsOptions, bool]] = None
     """Whether to set the page content to the highlights of the results."""
     text_contents_options: Union[TextContentsOptions, Literal[True]] = True
     """How to set the page content of the results"""
 
-    client: Exa
-    exa_api_key: SecretStr
+    client: Exa = Field(default=None)
+    exa_api_key: SecretStr = Field(default=None)
     exa_base_url: Optional[str] = None
 
     @root_validator(pre=True)
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate the environment."""
         values = initialize_client(values)
         return values
 
     def _get_relevant_documents(
         self, query: str, *, run_manager: CallbackManagerForRetrieverRun
     ) -> List[Document]:
-        response = self.client.search_and_contents(
+        response = self.client.search_and_contents(  # type: ignore[misc]
             query,
             num_results=self.k,
             text=self.text_contents_options,
-            highlights=self.highlights,
+            highlights=self.highlights,  # type: ignore
             include_domains=self.include_domains,
             exclude_domains=self.exclude_domains,
             start_crawl_date=self.start_crawl_date,
             end_crawl_date=self.end_crawl_date,
             start_published_date=self.start_published_date,
             end_published_date=self.end_published_date,
             use_autoprompt=self.use_autoprompt,
```

### Comparing `langchain_exa-0.0.1/langchain_exa/tools.py` & `langchain_exa-0.1.0/langchain_exa/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 from typing import Dict, List, Optional, Union
 
 from exa_py import Exa  # type: ignore
 from exa_py.api import HighlightsContentsOptions, TextContentsOptions  # type: ignore
 from langchain_core.callbacks import (
     CallbackManagerForToolRun,
 )
-from langchain_core.pydantic_v1 import SecretStr, root_validator
+from langchain_core.pydantic_v1 import Field, SecretStr, root_validator
 from langchain_core.tools import BaseTool
 
 from langchain_exa._utilities import initialize_client
 
 
 class ExaSearchResults(BaseTool):
     """Tool that queries the Metaphor Search API and gets back json."""
 
     name: str = "exa_search_results_json"
     description: str = (
         "A wrapper around Exa Search. "
         "Input should be an Exa-optimized query. "
         "Output is a JSON array of the query results"
     )
-    client: Exa
-    exa_api_key: SecretStr
+    client: Exa = Field(default=None)
+    exa_api_key: SecretStr = Field(default=None)
 
     @root_validator(pre=True)
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate the environment."""
         values = initialize_client(values)
         return values
 
@@ -47,39 +47,39 @@
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> Union[List[Dict], str]:
         """Use the tool."""
         try:
             return self.client.search_and_contents(
                 query,
                 num_results=num_results,
-                text=text_contents_options,
-                highlights=highlights,
+                text=text_contents_options,  # type: ignore
+                highlights=highlights,  # type: ignore
                 include_domains=include_domains,
                 exclude_domains=exclude_domains,
                 start_crawl_date=start_crawl_date,
                 end_crawl_date=end_crawl_date,
                 start_published_date=start_published_date,
                 end_published_date=end_published_date,
                 use_autoprompt=use_autoprompt,
-            )
+            )  # type: ignore
         except Exception as e:
             return repr(e)
 
 
 class ExaFindSimilarResults(BaseTool):
     """Tool that queries the Metaphor Search API and gets back json."""
 
     name: str = "exa_find_similar_results_json"
     description: str = (
         "A wrapper around Exa Find Similar. "
         "Input should be an Exa-optimized query. "
         "Output is a JSON array of the query results"
     )
-    client: Exa
-    exa_api_key: SecretStr
+    client: Exa = Field(default=None)
+    exa_api_key: SecretStr = Field(default=None)
     exa_base_url: Optional[str] = None
 
     @root_validator(pre=True)
     def validate_environment(cls, values: Dict) -> Dict:
         """Validate the environment."""
         values = initialize_client(values)
         return values
@@ -101,20 +101,20 @@
         run_manager: Optional[CallbackManagerForToolRun] = None,
     ) -> Union[List[Dict], str]:
         """Use the tool."""
         try:
             return self.client.find_similar_and_contents(
                 url,
                 num_results=num_results,
-                text=text_contents_options,
-                highlights=highlights,
+                text=text_contents_options,  # type: ignore
+                highlights=highlights,  # type: ignore
                 include_domains=include_domains,
                 exclude_domains=exclude_domains,
                 start_crawl_date=start_crawl_date,
                 end_crawl_date=end_crawl_date,
                 start_published_date=start_published_date,
                 end_published_date=end_published_date,
                 exclude_source_domain=exclude_source_domain,
                 category=category,
-            )
+            )  # type: ignore
         except Exception as e:
             return repr(e)
```

### Comparing `langchain_exa-0.0.1/pyproject.toml` & `langchain_exa-0.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,78 @@
 [tool.poetry]
 name = "langchain-exa"
-version = "0.0.1"
+version = "0.1.0"
 description = "An integration package connecting Exa and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/exa"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = ">=0.0.12"
-exa-py = "^1.0.7"
+langchain-core = ">=0.1.52,<0.3"
+exa-py = "^1.0.8"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
-pytest-mock  = "^3.10.0"
+pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
-langchain-core = {path = "../../core", develop = true}
+langchain-core = { path = "../../core", develop = true }
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
 
 [tool.poetry.group.lint]
 optional = true
 
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
 [tool.poetry.group.typing.dependencies]
-mypy = "^0.991"
-langchain-core = {path = "../../core", develop = true}
+mypy = "^1"
+langchain-core = { path = "../../core", develop = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-langchain-core = {path = "../../core", develop = true}
+langchain-core = { path = "../../core", develop = true }
 
 [tool.poetry.group.test_integration]
 optional = true
 
 [tool.poetry.group.test_integration.dependencies]
 
 
-[tool.ruff]
+[tool.ruff.lint]
 select = [
-  "E",  # pycodestyle
-  "F",  # pyflakes
-  "I",  # isort
+  "E",    # pycodestyle
+  "F",    # pyflakes
+  "I",    # isort
+  "T201", # print
+
 ]
 
 [tool.mypy]
 disallow_untyped_defs = "True"
 
 [tool.coverage.run]
-omit = [
-    "tests/*",
-]
+omit = ["tests/*"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 # --strict-markers will raise errors on unknown marks.
```

