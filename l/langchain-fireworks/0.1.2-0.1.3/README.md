# Comparing `tmp/langchain_fireworks-0.1.2.tar.gz` & `tmp/langchain_fireworks-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_fireworks-0.1.2.tar", max compression
+gzip compressed data, was "langchain_fireworks-0.1.3.tar", max compression
```

## Comparing `langchain_fireworks-0.1.2.tar` & `langchain_fireworks-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/LICENSE
--rw-r--r--   0        0        0     2929 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/README.md
--rw-r--r--   0        0        0      319 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/langchain_fireworks/__init__.py
--rw-r--r--   0        0        0    37383 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/langchain_fireworks/chat_models.py
--rw-r--r--   0        0        0     1788 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/langchain_fireworks/embeddings.py
--rw-r--r--   0        0        0     7962 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/langchain_fireworks/llms.py
--rw-r--r--   0        0        0        0 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/langchain_fireworks/py.typed
--rw-r--r--   0        0        0      232 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/langchain_fireworks/version.py
--rw-r--r--   0        0        0     2593 2024-04-11 16:21:10.692880 langchain_fireworks-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3870 1970-01-01 00:00:00.000000 langchain_fireworks-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-16 02:50:17.536460 langchain_fireworks-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2929 2024-05-16 02:50:17.536460 langchain_fireworks-0.1.3/README.md
+-rw-r--r--   0        0        0      319 2024-05-16 02:50:17.536460 langchain_fireworks-0.1.3/langchain_fireworks/__init__.py
+-rw-r--r--   0        0        0    37334 2024-05-16 02:50:17.536460 langchain_fireworks-0.1.3/langchain_fireworks/chat_models.py
+-rw-r--r--   0        0        0     1788 2024-05-16 02:50:17.536460 langchain_fireworks-0.1.3/langchain_fireworks/embeddings.py
+-rw-r--r--   0        0        0     7962 2024-05-16 02:50:17.536460 langchain_fireworks-0.1.3/langchain_fireworks/llms.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:50:17.536460 langchain_fireworks-0.1.3/langchain_fireworks/py.typed
+-rw-r--r--   0        0        0      232 2024-05-16 02:50:17.536460 langchain_fireworks-0.1.3/langchain_fireworks/version.py
+-rw-r--r--   0        0        0     2676 2024-05-16 02:50:17.540460 langchain_fireworks-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3868 1970-01-01 00:00:00.000000 langchain_fireworks-0.1.3/PKG-INFO
```

### Comparing `langchain_fireworks-0.1.2/LICENSE` & `langchain_fireworks-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_fireworks-0.1.2/README.md` & `langchain_fireworks-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `langchain_fireworks-0.1.2/langchain_fireworks/chat_models.py` & `langchain_fireworks-0.1.3/langchain_fireworks/chat_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     Type,
     TypedDict,
     Union,
     cast,
 )
 
 from fireworks.client import AsyncFireworks, Fireworks  # type: ignore
-from langchain_core._api import beta
 from langchain_core.callbacks import (
     AsyncCallbackManagerForLLMRun,
     CallbackManagerForLLMRun,
 )
 from langchain_core.language_models import LanguageModelInput
 from langchain_core.language_models.chat_models import (
     BaseChatModel,
@@ -667,15 +666,14 @@
                     "type": "function",
                     "function": {"name": tool_name},
                 }
 
             kwargs["tool_choice"] = tool_choice
         return super().bind(tools=formatted_tools, **kwargs)
 
-    @beta()
     def with_structured_output(
         self,
         schema: Optional[Union[Dict, Type[BaseModel]]] = None,
         *,
         method: Literal["function_calling", "json_mode"] = "function_calling",
         include_raw: bool = False,
         **kwargs: Any,
```

### Comparing `langchain_fireworks-0.1.2/langchain_fireworks/embeddings.py` & `langchain_fireworks-0.1.3/langchain_fireworks/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_fireworks-0.1.2/langchain_fireworks/llms.py` & `langchain_fireworks-0.1.3/langchain_fireworks/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_fireworks-0.1.2/pyproject.toml` & `langchain_fireworks-0.1.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-fireworks"
-version = "0.1.2"
+version = "0.1.3"
 description = "An integration package connecting Fireworks and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/fireworks"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.42"
+langchain-core = ">=0.1.52,<0.3"
 fireworks-ai = ">=0.13.0"
 openai = "^1.10.0"
 requests = "^2"
 aiohttp = "^3.9.1"
 
 [tool.poetry.group.test]
 optional = true
@@ -25,14 +25,15 @@
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
 langchain-core = { path = "../../core", develop = true }
+langchain-standard-tests = { path = "../../standard-tests", develop = true }
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
 codespell = "^2.2.0"
```

### Comparing `langchain_fireworks-0.1.2/PKG-INFO` & `langchain_fireworks-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-fireworks
-Version: 0.1.2
+Version: 0.1.3
 Summary: An integration package connecting Fireworks and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
 Requires-Dist: fireworks-ai (>=0.13.0)
-Requires-Dist: langchain-core (>=0.1.42,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.52,<0.3)
 Requires-Dist: openai (>=1.10.0,<2.0.0)
 Requires-Dist: requests (>=2,<3)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/fireworks
 Description-Content-Type: text/markdown
 
 # LangChain-Fireworks
```

