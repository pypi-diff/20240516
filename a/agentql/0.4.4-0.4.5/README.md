# Comparing `tmp/agentql-0.4.4.tar.gz` & `tmp/agentql-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentql-0.4.4.tar", max compression
+gzip compressed data, was "agentql-0.4.5.tar", max compression
```

## Comparing `agentql-0.4.4.tar` & `agentql-0.4.5.tar`

### file list

```diff
@@ -1,49 +1,61 @@
--rw-r--r--   0        0        0     1066 2024-05-08 14:57:21.100533 agentql-0.4.4/LICENSE
--rw-r--r--   0        0        0      111 2024-05-08 14:57:21.100533 agentql-0.4.4/PACKAGE_README.md
--rw-r--r--   0        0        0      771 2024-05-08 14:57:21.188532 agentql-0.4.4/pyproject.toml
--rw-r--r--   0        0        0      536 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/__init__.py
--rw-r--r--   0        0        0       78 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_api_constants.py
--rw-r--r--   0        0        0     4741 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_errors.py
--rw-r--r--   0        0        0        0 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/__init__.py
--rw-r--r--   0        0        0      322 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/add_dom_change_listener.js
--rw-r--r--   0        0        0     7207 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/generate_accessibility_tree.js
--rw-r--r--   0        0        0      147 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/get_last_dom_change.js
--rw-r--r--   0        0        0      145 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/remove_dom_change_listener.js
--rw-r--r--   0        0        0      506 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/scroll_to_bottom.js
--rw-r--r--   0        0        0      503 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/scroll_to_top.js
--rw-r--r--   0        0        0      843 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/set_iframe_path.js
--rw-r--r--   0        0        0      436 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_js_snippets/snippet_loader.py
--rw-r--r--   0        0        0        0 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/__init__.py
--rw-r--r--   0        0        0     1098 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/character_utils.py
--rw-r--r--   0        0        0     4997 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/lexer.py
--rw-r--r--   0        0        0     2431 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/node.py
--rw-r--r--   0        0        0     4686 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/parser.py
--rw-r--r--   0        0        0     1196 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/source.py
--rw-r--r--   0        0        0     1602 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/token.py
--rw-r--r--   0        0        0      213 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_syntax/token_kind.py
--rw-r--r--   0        0        0      535 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_typing.py
--rw-r--r--   0        0        0      377 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/_core/_utils.py
--rw-r--r--   0        0        0      363 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/async_api/__init__.py
--rw-r--r--   0        0        0     2893 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/async_api/_api.py
--rw-r--r--   0        0        0     1840 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/async_api/_popup.py
--rw-r--r--   0        0        0     5979 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/async_api/_response_proxy.py
--rw-r--r--   0        0        0    11329 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/async_api/_session.py
--rw-r--r--   0        0        0     5601 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/async_api/_web_driver.py
--rw-r--r--   0        0        0        0 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/__init__.py
--rw-r--r--   0        0        0      288 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/playwright/__init__.py
--rw-r--r--   0        0        0      193 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/playwright/_driver_constants.py
--rw-r--r--   0        0        0      280 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/playwright/_driver_settings.py
--rw-r--r--   0        0        0     1980 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/playwright/_html_constants.py
--rw-r--r--   0        0        0     3813 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/playwright/_network_monitor.py
--rw-r--r--   0        0        0    27588 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/playwright/playwright_driver_async.py
--rw-r--r--   0        0        0    27290 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/ext/playwright/playwright_driver_sync.py
--rw-r--r--   0        0        0      363 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/sync_api/__init__.py
--rw-r--r--   0        0        0     2847 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/sync_api/_api.py
--rw-r--r--   0        0        0     1525 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/sync_api/_popup.py
--rw-r--r--   0        0        0     5291 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/sync_api/_response_proxy.py
--rw-r--r--   0        0        0    11068 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/sync_api/_session.py
--rw-r--r--   0        0        0     5017 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/sync_api/_web_driver.py
--rw-r--r--   0        0        0      291 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/trail_logger/__init__.py
--rw-r--r--   0        0        0     5151 2024-05-08 14:57:21.188532 agentql-0.4.4/src/agentql/trail_logger/trail_logger.py
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 agentql-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-16 01:15:44.746817 agentql-0.4.5/LICENSE
+-rw-r--r--   0        0        0      111 2024-05-16 01:15:44.746817 agentql-0.4.5/PACKAGE_README.md
+-rw-r--r--   0        0        0      835 2024-05-16 01:15:44.834817 agentql-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      591 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_cli/_commands/__init__.py
+-rw-r--r--   0        0        0      261 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_cli/_commands/doctor_command.py
+-rw-r--r--   0        0        0     2681 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_cli/_commands/init_command.py
+-rw-r--r--   0        0        0      228 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_cli/_main.py
+-rw-r--r--   0        0        0        0 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/__init__.py
+-rw-r--r--   0        0        0      177 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_api_constants.py
+-rw-r--r--   0        0        0     5443 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_errors.py
+-rw-r--r--   0        0        0        0 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/__init__.py
+-rw-r--r--   0        0        0      322 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/add_dom_change_listener.js
+-rw-r--r--   0        0        0     7249 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/generate_accessibility_tree.js
+-rw-r--r--   0        0        0      147 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/get_last_dom_change.js
+-rw-r--r--   0        0        0      119 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/iframe_contains_doc_or_body.js
+-rw-r--r--   0        0        0      145 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/remove_dom_change_listener.js
+-rw-r--r--   0        0        0      506 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/scroll_to_bottom.js
+-rw-r--r--   0        0        0      503 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/scroll_to_top.js
+-rw-r--r--   0        0        0      843 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/set_iframe_path.js
+-rw-r--r--   0        0        0      436 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_js_snippets/snippet_loader.py
+-rw-r--r--   0        0        0        0 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/__init__.py
+-rw-r--r--   0        0        0     1098 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/character_utils.py
+-rw-r--r--   0        0        0     4997 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/lexer.py
+-rw-r--r--   0        0        0     2475 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/node.py
+-rw-r--r--   0        0        0     4686 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/parser.py
+-rw-r--r--   0        0        0     1196 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/source.py
+-rw-r--r--   0        0        0     1602 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/token.py
+-rw-r--r--   0        0        0      213 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_syntax/token_kind.py
+-rw-r--r--   0        0        0      297 2024-05-16 01:15:44.834817 agentql-0.4.5/src/agentql/_core/_trail_logger/__init__.py
+-rw-r--r--   0        0        0     5151 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/_core/_trail_logger/_trail_logger_impl.py
+-rw-r--r--   0        0        0      535 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/_core/_typing.py
+-rw-r--r--   0        0        0     1962 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/_core/_utils.py
+-rw-r--r--   0        0        0      363 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/async_api/__init__.py
+-rw-r--r--   0        0        0     3871 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/async_api/_agentql_service.py
+-rw-r--r--   0        0        0     2893 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/async_api/_api.py
+-rw-r--r--   0        0        0     2194 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/async_api/_popup.py
+-rw-r--r--   0        0        0     6166 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/async_api/_response_proxy.py
+-rw-r--r--   0        0        0     8409 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/async_api/_session.py
+-rw-r--r--   0        0        0     6023 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/async_api/_web_driver.py
+-rw-r--r--   0        0        0     1283 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/experimental/async_api/_protocol/_browser.py
+-rw-r--r--   0        0        0     3981 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/experimental/async_api/_protocol/_page.py
+-rw-r--r--   0        0        0     1269 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/experimental/sync_api/_protocol/_browser.py
+-rw-r--r--   0        0        0     3919 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/experimental/sync_api/_protocol/_page.py
+-rw-r--r--   0        0        0        0 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/__init__.py
+-rw-r--r--   0        0        0      440 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/playwright/__init__.py
+-rw-r--r--   0        0        0      193 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/playwright/_driver_constants.py
+-rw-r--r--   0        0        0      280 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/playwright/_driver_settings.py
+-rw-r--r--   0        0        0     1980 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/playwright/_html_constants.py
+-rw-r--r--   0        0        0     4554 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/playwright/_network_monitor.py
+-rw-r--r--   0        0        0    30022 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/playwright/playwright_driver_async.py
+-rw-r--r--   0        0        0    29657 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/ext/playwright/playwright_driver_sync.py
+-rw-r--r--   0        0        0      363 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/sync_api/__init__.py
+-rw-r--r--   0        0        0     3768 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/sync_api/_agentql_service.py
+-rw-r--r--   0        0        0     2847 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/sync_api/_api.py
+-rw-r--r--   0        0        0     1918 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/sync_api/_popup.py
+-rw-r--r--   0        0        0     5478 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/sync_api/_response_proxy.py
+-rw-r--r--   0        0        0     8199 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/sync_api/_session.py
+-rw-r--r--   0        0        0     5433 2024-05-16 01:15:44.838817 agentql-0.4.5/src/agentql/sync_api/_web_driver.py
+-rw-r--r--   0        0        0      910 1970-01-01 00:00:00.000000 agentql-0.4.5/PKG-INFO
```

### Comparing `agentql-0.4.4/LICENSE` & `agentql-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `agentql-0.4.4/pyproject.toml` & `agentql-0.4.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "agentql"
-version = "0.4.4"
+version = "0.4.5"
 description = "Tiny Fish AgentQL Python Client"
 authors = []
 license = "MIT"
 readme = "PACKAGE_README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 playwright = "^1"
 requests = "^2"
 pydantic = "^2"
-httpx = "^0.26"
-pytest-asyncio = "^0.23"
+httpx = "^0"
+pytest-asyncio = "^0"
 aiofiles = "^23"
 tf-playwright-stealth = "*"
+typer = "^0"
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
 
-
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 pytest-time = "*"
 pylint = "*"
 mockito = "*"
 pytest_env = "*"
 pytest-asyncio = "*"
@@ -38,7 +38,10 @@
 
 [tool.black]
 line-length = 100
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+agentql = "agentql._cli._main:app"
```

### Comparing `agentql-0.4.4/src/agentql/__init__.py` & `agentql-0.4.5/src/agentql/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from ._core import _trail_logger as trail_logger
 from ._core._errors import *
-from ._core._syntax.node import ContainerListNode, ContainerNode, IdListNode, IdNode
+from ._core._syntax.node import ContainerListNode, ContainerNode, IdListNode, IdNode, Node
 from ._core._syntax.parser import QueryParser
 from ._core._typing import InteractiveItemTypeT, PageTypeT
 from .async_api._api import start_async_session
 from .sync_api._api import start_session
 
 __ALL__ = [
     "start_session",
```

### Comparing `agentql-0.4.4/src/agentql/_core/_errors.py` & `agentql-0.4.5/src/agentql/_core/_errors.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import json
 import logging
+from typing import Union
+
+from agentql._core._syntax.node import Node
 
 # pylint: disable-all
 AGENTQL_1000_API_KEY_ERROR = 1000
 AGENTQL_1001_ATTRIBUTE_NOT_FOUND_ERROR = 1001
 AGENTQL_1002_NO_OPEN_BROWSER_ERROR = 1002
 AGENTQL_1003_NO_OPEN_PAGE_ERROR = 1003
 AGENTQL_1004_PAGE_TIMEOUT_ERROR = 1004
@@ -32,16 +35,38 @@
         self,
         message="Invalid or missing API key. Please set the environment variable 'AGENTQL_API_KEY' with a valid API key.",
     ):
         super().__init__(message, AGENTQL_1000_API_KEY_ERROR)
 
 
 class AttributeNotFoundError(BaseAgentQLError):
-    def __init__(self, name, response_data):
-        message = f"{name} not found in AgentQL response node: {json.dumps(response_data)[:300]}. If you are trying to perform an action on an element, make sure the element is the leaf node in your query."
+    def __init__(self, name: str, response_data: Union[dict, list], query_tree_node: Node):
+        if query_tree_node.name:
+            response_data = {query_tree_node.name: response_data}
+        message = f"""
+\"{name}\" not found in AgentQL response node:
+{json.dumps(response_data, indent=2)}
+There could be a few reasons for this:
+1. The element you are trying to access was not part of the original query. Make sure there are no typos in the name of the element you are trying to access. 
+
+Query:
+{query_tree_node.dump()}
+
+2. You may be trying to execute an action on a container node. I.e. the following would raise this error:
+Query:
+{{
+    footer {{
+        some_link
+    }}
+}}
+
+response.footer.click()
+
+In the above example, footer is a container node and you are trying to click on it. You should access the child node instead. I.e. response.footer.some_link.click()
+"""
         super().__init__(message, AGENTQL_1001_ATTRIBUTE_NOT_FOUND_ERROR)
 
 
 class NoOpenBrowserError(BaseAgentQLError):
     def __init__(
         self,
         message='No open browser if detected. Make sure you call "start_browser()" first.',
```

### Comparing `agentql-0.4.4/src/agentql/_core/_js_snippets/generate_accessibility_tree.js` & `agentql-0.4.5/src/agentql/_core/_js_snippets/generate_accessibility_tree.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -128,14 +128,17 @@
             return true;
         }
 
         return false;
     }
 
     function createNode(node, currentIframePath = "") {
+        if (!node) {
+            return null;
+        }
         const ariaHidden =
             node.getAttribute("aria-hidden") === "true" ||
             node.getAttribute("aria-hidden") === true;
         const tag = node.nodeName.toLowerCase();
         const skippedTags = [
             "script",
             "style",
```

### Comparing `agentql-0.4.4/src/agentql/_core/_js_snippets/set_iframe_path.js` & `agentql-0.4.5/src/agentql/_core/_js_snippets/set_iframe_path.js`

 * *Files identical despite different names*

### Comparing `agentql-0.4.4/src/agentql/_core/_syntax/character_utils.py` & `agentql-0.4.5/src/agentql/_core/_syntax/character_utils.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.4/src/agentql/_core/_syntax/lexer.py` & `agentql-0.4.5/src/agentql/_core/_syntax/lexer.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.4/src/agentql/_core/_syntax/node.py` & `agentql-0.4.5/src/agentql/_core/_syntax/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 from pydantic import BaseModel, ConfigDict, Field, SerializeAsAny
 from typing_extensions import Annotated
 
 DEFAULT_INDENT = 2
 
 
+class _NodeWithChildrenMixin:
+    children: Annotated[SerializeAsAny[List["Node"]], Field(default_factory=List)]
+
+
 class Node(BaseModel):
     name: str
     # Freeze the model to make it immutable
     model_config = ConfigDict(frozen=True)
 
     @property
     def query_name(self) -> str:
@@ -33,17 +37,16 @@
         return self.dump()
 
     def get_child_by_name(self, name):
         """
         Returns the child node with the specified name.
         Raises an AttributeError if no child with the specified name is found.
         """
-        if hasattr(self, "children"):
+        if isinstance(self, _NodeWithChildrenMixin):
             for child in self.children:
-                child: Node
                 if child.name == name:
                     return child
         raise AttributeError(f"Node {self.name} has no child named {name}")
 
 
 class IdNode(Node):
     """
@@ -61,26 +64,24 @@
     """
 
     @property
     def query_name(self) -> str:
         return f"{self.name}[]"
 
 
-class ContainerNode(Node):
+class ContainerNode(Node, _NodeWithChildrenMixin):
     """
     {
         container {
             child1
             child2
         }
     }
     """
 
-    children: Annotated[SerializeAsAny[List[Node]], Field(default_factory=List)]
-
     def _dump(self, level: int = 0, indent: int = DEFAULT_INDENT) -> str:
         indent_spaces = " " * indent * level
         node_name = f"{self.query_name} " if self.query_name else ""
         header = f"{indent_spaces}{node_name}{{\n"
         # pylint: disable=protected-access
         body = "\n".join([child._dump(indent=indent, level=level + 1) for child in self.children])
         footer = f"\n{indent_spaces}}}"
```

### Comparing `agentql-0.4.4/src/agentql/_core/_syntax/parser.py` & `agentql-0.4.5/src/agentql/_core/_syntax/parser.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.4/src/agentql/_core/_syntax/source.py` & `agentql-0.4.5/src/agentql/_core/_syntax/source.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.4/src/agentql/_core/_syntax/token.py` & `agentql-0.4.5/src/agentql/_core/_syntax/token.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.4/src/agentql/_core/_typing.py` & `agentql-0.4.5/src/agentql/_core/_typing.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.4/src/agentql/async_api/_api.py` & `agentql-0.4.5/src/agentql/async_api/_api.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.4/src/agentql/async_api/_popup.py` & `agentql-0.4.5/src/agentql/async_api/_popup.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 
 
 class Popup:
     """Popup objects are dispatched by session via session.on("popup") event. For each popup window detected on the page, there will be corresponding event and popup objects emitted."""
 
     def __init__(
         self,
+        page_url: str,
         popup_tree: dict,
         popup_name: str,
         on_popup_close: Coroutine[Dict[Any, Any], Any, None],
     ):
+        self._page_url = page_url
         self._tree = popup_tree
         self._name = popup_name
         self._close_popup_callback = on_popup_close
 
     def __str__(self):
-        return f"Popup {self._name}"
+        return f"Popup {self._name} on page {self._page_url}"
 
     @property
     def accessibility_tree(self) -> dict:
         """
         Returns the part of accessibility tree where the popup node as the parent.
 
         Returns:
@@ -36,18 +38,29 @@
 
         Returns:
         --------
         str: The name of the popup.
         """
         return self._name
 
+    @property
+    def page_url(self) -> str:
+        """
+        Returns the URL of the page where the popup occurred.
+
+        Returns:
+        --------
+        str: The URL of the page where the popup occurred.
+        """
+        return self._page_url
+
     async def close(self):
         """Close the popup by invoking the callback function passed into the Popup object when it is initialized."""
         if self._close_popup_callback is not None and self._tree is not None:
-            await self._close_popup_callback(self._tree)
+            await self._close_popup_callback(self._tree, self._page_url)
         else:
             raise ValueError("Popup object is not properly initialized.")
 
 
 async def close_all_popups_handler(popups: list):
     """This is a asynchronous handler function for popups. Passing it as the callback function into session.on("popup") method will close all popups.
```

### Comparing `agentql-0.4.4/src/agentql/async_api/_response_proxy.py` & `agentql-0.4.5/src/agentql/async_api/_response_proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,19 +35,21 @@
         self._query_tree_node = query_tree
 
     def __getattr__(
         self, name
     ) -> Union["AQLResponseProxy[InteractiveItemTypeT]", InteractiveItemTypeT, None]:
         if self._response_data is None:
             raise AttributeError("Response data is None")
+
         if name not in self._response_data:
-            raise AttributeNotFoundError(name, self._response_data)
+            raise AttributeNotFoundError(name, self._response_data, self._query_tree_node)
         trail_logger.add_event(f"Resolving element {name} on {self._web_driver.current_url}")
+
         return self._resolve_item(
-            self._response_data[name], self._query_tree_node.get_child_by_name(name)
+            self._response_data[name], query_tree_node=self._query_tree_node.get_child_by_name(name)
         )
 
     def __getitem__(
         self, index: int
     ) -> Union[InteractiveItemTypeT, "AQLResponseProxy[InteractiveItemTypeT]", None]:
         if not isinstance(self._response_data, list):
             raise ValueError("This node is not a list")
@@ -87,17 +89,20 @@
 
         ```py
         {
         "query_field": "text content of the corresponding web element"
         }
         ```
         """
-        return await self._to_data_node(self._response_data, self._query_tree_node)
+        res = await self._to_data_node(self._response_data, self._query_tree_node)
+        if not isinstance(res, dict):
+            raise TypeError("Root node must be a container node")
+        return res
 
-    async def _to_data_node(self, response_data, query_tree_node) -> dict:
+    async def _to_data_node(self, response_data, query_tree_node) -> Union[dict, list, str, None]:
         if isinstance(query_tree_node, ContainerListNode):
             return await self._to_data_container_list_node(response_data, query_tree_node)
         elif isinstance(query_tree_node, ContainerNode):
             return await self._to_data_container_node(response_data, query_tree_node)
         elif isinstance(query_tree_node, IdListNode):
             return await self._to_data_id_list_node(response_data)
         elif isinstance(query_tree_node, IdNode):
```

### Comparing `agentql-0.4.4/src/agentql/async_api/_session.py` & `agentql-0.4.5/src/agentql/async_api/_session.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,42 @@
 # pylint: disable=protected-access
 
 import copy
 import logging
-import os
 from typing import Callable, Generic, List, Literal, Optional, Union
 
-import httpx
-
-from agentql import (
-    AgentQLServerError,
-    AgentQLServerTimeoutError,
-    APIKeyError,
-    AttributeNotFoundError,
-    QueryParser,
-    UnableToClosePopupError,
-    trail_logger,
-)
-from agentql._core._api_constants import GET_AGENTQL_ENDPOINT, SERVICE_URL
+from agentql import QueryParser, trail_logger
 from agentql._core._utils import minify_query
+from agentql.async_api._agentql_service import query_agentql_server
 
 from ._popup import Popup
 from ._response_proxy import AQLResponseProxy
 from ._web_driver import InteractiveItemTypeT, PageTypeT, WebDriver
 
 log = logging.getLogger("agentql")
 
 RESPONSE_ERROR_KEY = "detail"
-AGENTQL_API_KEY = os.getenv("AGENTQL_API_KEY")
 
 
 class Session(Generic[InteractiveItemTypeT, PageTypeT]):
     """Session class contains core functionality of AgentQL service. It is responsible for querying elements, managing session-related state (like authentication), and handling various events."""
 
     def __init__(self, web_driver: WebDriver[InteractiveItemTypeT, PageTypeT]):
         """Initialize the session.
 
         Parameters:
         ----------
         web_driver (WebDriver): The web driver that will be used in this session.
         """
-        if AGENTQL_API_KEY:
-            self._api_key = AGENTQL_API_KEY
-        else:
-            raise APIKeyError(
-                "API key not provided. Please set the environment variable 'AGENTQL_API_KEY' with your API key."
-            )
         self._web_driver = web_driver
         self._event_listeners = {}
         self._check_popup = False
         self._last_query = None
         self._last_response = None
+        self._last_accessibility_tree = None
 
     @property
     def current_page(self) -> PageTypeT:
         """Get the current page being processed by AgentQL.
 
         Returns:
         -------
@@ -77,14 +60,19 @@
         return self._last_query
 
     @property
     def last_response(self) -> Optional[dict]:
         """Get the last response."""
         return self._last_response
 
+    @property
+    def last_accessibility_tree(self) -> Optional[dict]:
+        """Get the last captured accessibility tree"""
+        return self._last_accessibility_tree
+
     def get_last_trail(self) -> Union[trail_logger.TrailLogger, None]:
         """
         Get the last trail recorded, if enable_history_log is True when starting the session.
         """
         logger_store = trail_logger.TrailLoggerStore.get_loggers()
         return logger_store[-1] if logger_store else None
 
@@ -100,14 +88,15 @@
 
         Parameters:
         ----------
         query (str): The AgentQL query in String format.
         timeout (int) (optional): Optional timeout value for the connection with backend api service.
         lazy_load_pages_count (int) (optional): The number of pages to scroll down and up to load lazy loaded content.
         wait_for_network_idle (bool) (optional): Whether to wait for the network to be idle before querying the page.
+        include_aria_hidden (bool) (optional): Whether to include elements with aria-hidden attribute in the accessibility tree.
 
         Returns:
         -------
         AQLResponseProxy: AgentQL Response (Elements that match the query) of AQLResponseProxy type.
         """
         trail_logger.add_event(f"Querying {minify_query(query)} on {self._web_driver.current_page}")
         log.debug(f"querying {query}")
@@ -120,22 +109,26 @@
             wait_for_network_idle=wait_for_network_idle
         )
 
         accessibility_tree = await self._web_driver._prepare_accessibility_tree(
             lazy_load_pages_count=lazy_load_pages_count, include_aria_hidden=include_aria_hidden
         )
 
+        self._last_accessibility_tree = accessibility_tree
+
         # Check if there is a popup in the page before sending the agentql query
         popup_list = []
         if self._check_popup:
             popup_list = self._detect_popup(accessibility_tree, [])
             if popup_list:
                 await self._handle_popup(popup_list)
 
-        response = await self._query(query, accessibility_tree, timeout)
+        response = await query_agentql_server(
+            query, accessibility_tree, timeout, self._web_driver.current_url
+        )
         self._last_response = response
 
         # Check if there is a popup in the page after receiving the agentql response
         if self._check_popup:
             # Fetch the most up-to-date accessibility tree
             accessibility_tree = await self._web_driver.accessibility_tree
 
@@ -169,63 +162,14 @@
         """
         self._event_listeners[event] = callback
         if callback:
             self._check_popup = True
         else:
             self._check_popup = False
 
-    async def _query(self, query: str, accessibility_tree: dict, timeout: int) -> dict:
-        """Make Request to AgentQL API.
-
-        Parameters:
-        ----------
-        query (str): The query string.
-        accessibility_tree (dict): The accessibility tree.
-        timeout (int): The timeout value for the connection with backend api service
-
-        Returns:
-        -------
-        dict: AgentQL response in json format.
-        """
-        try:
-            page_url = self._web_driver.current_url
-            request_data = {
-                "query": f"{query}",
-                "accessibility_tree": accessibility_tree,
-                "metadata": {"url": page_url},
-            }
-            url = os.getenv("AGENTQL_API_HOST", SERVICE_URL) + GET_AGENTQL_ENDPOINT
-            log.debug(f"Making request to {url}")
-            headers = {"X-API-Key": self._api_key}
-            async with httpx.AsyncClient() as client:
-                response = await client.post(
-                    url, json=request_data, headers=headers, timeout=timeout, follow_redirects=True
-                )
-                response.raise_for_status()
-                return response.json()
-        except httpx.TimeoutException as e:
-            raise AgentQLServerTimeoutError() from e
-        except httpx.HTTPStatusError as e:
-            if e.response.status_code == 401:
-                raise APIKeyError(
-                    "Invalid or expired API key provided. Please set the environment variable 'AGENTQL_API_KEY' with a valid API key."
-                ) from e
-            error_code = e.response.status_code
-            server_error = e.response.text
-            if server_error:
-                try:
-                    server_error_json = e.response.json()
-                    if isinstance(server_error_json, dict):
-                        server_error = server_error_json.get(RESPONSE_ERROR_KEY)
-                except ValueError:
-                    raise AgentQLServerError(server_error, error_code) from e
-            raise AgentQLServerError(server_error, error_code) from e
-        except httpx.RequestError as e:
-            raise AgentQLServerError(str(e)) from e
-
     def _detect_popup(self, tree: dict, known_popups: List[Popup]) -> List[Popup]:
         """Detect if there is a popup in the page. If so, create a Popup object and add it to the popup dict.
 
         Parameters:
         ----------
         tree (dict): The accessibility tree.
         known_popups (list): The list of known popups.
@@ -234,15 +178,20 @@
         --------
         popups (list): The list of popups.
         """
         tree_role = tree.get("role", "")
         tree_name = tree.get("name", "")
         popup_list = []
         if tree_role == "dialog":
-            popup = Popup(copy.deepcopy(tree), tree_name, self._close_popup)
+            popup = Popup(
+                self._web_driver.current_url,
+                copy.deepcopy(tree),
+                tree_name,
+                self._web_driver._close_popup,
+            )
 
             # Avoid adding existing popup to the dict and double handle the popup
             if known_popups:
                 for popup_object in known_popups:
                     if popup_object.name != popup.name:
                         popup_list.append(popup)
             else:
@@ -260,33 +209,7 @@
         """Handle the popup. If there is a popup in the list, and there is an event listener, emit the popup event by invoking the callback function.
 
         Parameters:
         ----------
         popups (list): The list of popups to handle."""
         if popups and "popup" in self._event_listeners and self._event_listeners["popup"]:
             await self._event_listeners["popup"](popups)
-
-    async def _close_popup(self, tree: dict):
-        """Close the popup by querying AgentQL server and click the close button.
-
-        Parameters:
-        ----------
-        popup (Popup): The popup to close.
-        query (str): The query to close the popup.
-        """
-        query = """
-            {
-                popup {
-                    close_btn
-                }
-            }
-        """
-        parser = QueryParser(query)
-        query_tree = parser.parse()
-        try:
-            response = await self._query(query, tree, 500)
-            agentql_response = AQLResponseProxy[InteractiveItemTypeT](
-                response, self._web_driver, query_tree
-            )
-            await agentql_response.popup.close_btn.click()
-        except (AgentQLServerError, AttributeNotFoundError) as e:
-            raise UnableToClosePopupError() from e
```

### Comparing `agentql-0.4.4/src/agentql/async_api/_web_driver.py` & `agentql-0.4.5/src/agentql/async_api/_web_driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,14 +93,24 @@
         """Returns the page object that represents the current page. Users should be able to do more fine grained interaction using this page object, such as navigating to a different url or take screenshot of the page.
 
         Returns:
         --------
         PageTypeT: The current page object.
         """
 
+    async def _close_popup(self, popup_tree: dict, page_url: str, timeout: int = 500):
+        """Close the popup on the page.
+
+        Parameters:
+        -----------
+        popup_tree (dict): The accessibility tree that has the popup node as the parent.
+        page_url (str): The URL of the active page.
+        timeout (int) (optional): The timeout value for the connection with AgentQL server service.
+        """
+
     async def _get_user_auth_session(self) -> Any:
         """Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
 
         Returns:
         --------
         The user session state.
         """
```

### Comparing `agentql-0.4.4/src/agentql/ext/playwright/_html_constants.py` & `agentql-0.4.5/src/agentql/ext/playwright/_html_constants.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.4/src/agentql/ext/playwright/_network_monitor.py` & `agentql-0.4.5/src/agentql/ext/playwright/_network_monitor.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,39 @@
 import time
 
+from agentql import trail_logger
+
+DOM_NETWORK_QUIET_THRESHOLD_SECONDS = 0.5
+
 
 class PageActivityMonitor:
     """A class that monitors network activity and determines when a page has loaded."""
 
     def __init__(self):
         """Initialize the network monitor."""
         self._request_log = {}
         self._response_log = set()
         self._last_network_active_time = time.time()
         self._multi_request_found = False
+        self._multi_request_url = ""
         self._page_loaded = False
         self._start_time = time.time()
 
     def track_network_request(self, request):
         """Track a request and record its timestamp into the _last_network_active_time.
 
         Parameters:
         ----------
         request (requests.PreparedRequest): The request to track."""
         self._last_network_active_time = time.time()
         # Start logging duplicate urls after the first 6 seconds
         if time.time() - self._start_time > 6:
             if request.url in self._request_log:
                 self._multi_request_found = True
+                self._multi_request_url = request.url
         self._request_log[request.url] = time.time()
 
     def track_network_response(self, response):
         """Track a response and mark it in the network log.
 
         Parameters:
         ----------
@@ -44,54 +50,63 @@
         """Get the status of the page load.
 
         Returns:
         -------
         bool: True if the page has loaded, False otherwise."""
         return self._page_loaded
 
-    def check_conditions(self, last_active_dom_time=None) -> bool:
+    def is_page_ready(self, last_active_dom_time=None) -> bool:
         """Check if the conditions for Page Ready state have been met
 
         Returns:
         -------
         bool: True if the conditions for Page Ready State have been met, False otherwise."""
         dom_is_quiet = False
         network_is_quiet = False
 
         # Check if DOM has changed
         if last_active_dom_time:
             last_active_dom_time = float(last_active_dom_time) / 1000
-            if time.time() - last_active_dom_time > 0.5:
+            if time.time() - last_active_dom_time > DOM_NETWORK_QUIET_THRESHOLD_SECONDS:
                 dom_is_quiet = True
 
         # Check for inactivity
         missing_responses = []
-        if time.time() - self._last_network_active_time > 0.5:
+        if time.time() - self._last_network_active_time > DOM_NETWORK_QUIET_THRESHOLD_SECONDS:
             # Check if all requests have been resolved
             for request in self._request_log:
                 if request not in self._response_log:
                     missing_responses.append(request)
 
             # If not all requests have been resolved, check if 1.5 seconds have passed since the last request. If so, treat the request as resolved
             missing_responses_count = len(missing_responses)
             for missing_response in missing_responses:
                 time_diff = time.time() - self._request_log[missing_response]
                 if time_diff > 1.5:
                     missing_responses_count -= 1
 
             if missing_responses_count == 0:
                 if dom_is_quiet:
+                    trail_logger.add_event(
+                        f"Page ready: No network and DOM activity for {DOM_NETWORK_QUIET_THRESHOLD_SECONDS} seconds."
+                    )
                     return True
                 network_is_quiet = True
 
         # If 6 seconds has passed, only check if the network is quiet or if multiple requests to the same destination are found
         if time.time() - self._start_time > 6:
             if network_is_quiet:
+                trail_logger.add_event(
+                    f"Page ready: No network activity for {DOM_NETWORK_QUIET_THRESHOLD_SECONDS} seconds."
+                )
                 return True
             if self._multi_request_found:
+                trail_logger.add_event(
+                    f"Page ready: Multiple outgoing requests to url {self._multi_request_url} are found."
+                )
                 return True
 
         return False
 
     def reset(self):
         """Reset the network monitor."""
         self._request_log = {}
```

### Comparing `agentql-0.4.4/src/agentql/ext/playwright/playwright_driver_async.py` & `agentql-0.4.5/src/agentql/ext/playwright/playwright_driver_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,30 @@
     Locator,
     Page,
     StorageState,
     async_playwright,
 )
 from playwright_stealth import StealthConfig, stealth_async
 
-from agentql import trail_logger
+from agentql import QueryParser, trail_logger
 from agentql._core._errors import (
     AccessibilityTreeError,
+    AgentQLServerError,
+    AttributeNotFoundError,
     ElementNotFoundError,
     NoOpenBrowserError,
     NoOpenPageError,
     OpenUrlError,
+    UnableToClosePopupError,
 )
 from agentql._core._js_snippets.snippet_loader import load_js
 from agentql._core._utils import ensure_url_scheme
 from agentql.async_api import ScrollDirection, WebDriver
+from agentql.async_api._agentql_service import query_agentql_server
+from agentql.async_api._response_proxy import AQLResponseProxy
 
 from ._driver_constants import RENDERER, USER_AGENT, VENDOR
 from ._driver_settings import ProxySettings, StealthModeConfig
 from ._html_constants import HTML_ROLE_MAPPING
 from ._network_monitor import PageActivityMonitor
 
 
@@ -132,15 +137,17 @@
         new_page (bool): Whether to open the URL in a new tab in that tab. To navigate to a new url with the current tab, use Playwright Page object's [page.goto()](https://playwright.dev/python/docs/api/class-page#page-goto) method.
         """
         if not self._browser:
             raise NoOpenBrowserError()
         if new_page or self._current_page is None:
             await self._open_url(url)
         else:
-            await self._current_page.goto(url, wait_until="load")
+            url = ensure_url_scheme(url)
+            self._current_tf_id = 0
+            await self._current_page.goto(url, wait_until="domcontentloaded")
 
     @property
     def current_url(self) -> str:
         """Get the URL of the current page being processed by AgentQL.
 
         Returns:
         --------
@@ -235,15 +242,17 @@
             # Reset the network monitor to clear the logs
             self._page_monitor.reset()
 
         # Add event listeners to track DOM changes and network activities
         await self._add_page_event_listeners()
 
         # Wait for the page to reach the "Page Ready" state
-        await self._determine_load_state(self._page_monitor, wait_for_network_idle)
+        await self._determine_load_state(
+            self._page_monitor, wait_for_network_idle=wait_for_network_idle
+        )
 
         # Remove the event listeners to prevent overwhelming the async event loop
         await self._remove_page_event_listeners()
 
     async def scroll_page(self, scroll_direction: ScrollDirection, pixels: int = 720):
         """Scrolls the page up or down by given pixels. By default, it will scroll 720 pixels.
 
@@ -268,14 +277,41 @@
     async def scroll_to_top(self):
         """Scrolls to the top of the current page."""
         if not self._current_page:
             raise NoOpenPageError()
 
         await self._current_page.evaluate(load_js("scroll_to_top"))
 
+    async def _close_popup(self, popup_tree: dict, page_url: str, timeout: int = 500):
+        """Close the popup by querying AgentQL server for the close button and perform a click action with web driver.
+
+        Parameters:
+        -----------
+        popup_tree (dict): The accessibility tree that has the popup node as the parent.
+        page_url (str): The URL of the active page.
+        timeout (int) (optional): The timeout value for the connection with AgentQL server service.
+        """
+        query = """
+            {
+                popup {
+                    close_btn
+                }
+            }
+        """
+        parser = QueryParser(query)
+        query_tree = parser.parse()
+        try:
+            response = await query_agentql_server(
+                query, popup_tree, timeout=timeout, page_url=page_url
+            )
+            agentql_response = AQLResponseProxy(response, self, query_tree)
+            await agentql_response.popup.close_btn.click()
+        except (AgentQLServerError, AttributeNotFoundError) as e:
+            raise UnableToClosePopupError() from e
+
     async def _get_user_auth_session(self) -> StorageState:
         """
         Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
 
         Returns:
         --------
         dict: User auth session in Python dictionary format.
@@ -346,14 +382,16 @@
         else:
             content_frame = await frame.content_frame()
             if not content_frame:
                 return
             iframes = await content_frame.query_selector_all("iframe")
 
         for iframe in iframes:
+            if not await self._iframe_contains_doc_or_body(iframe):
+                continue
             iframe_id = await iframe.get_attribute("tf623_id")
             iframe_path_to_send = ""
             if iframe_path:
                 iframe_path_to_send = f"{iframe_path}."
             iframe_path_to_send = f"{iframe_path_to_send}{iframe_id}"
             iframe_accessibility_tree = await self._get_frame_accessibility_tree(
                 iframe, iframe_path_to_send
@@ -365,14 +403,33 @@
 
             await self._process_iframes(
                 iframe_path=iframe_path_to_send,
                 frame=iframe,
                 page_accessibility_tree=page_accessibility_tree,
             )
 
+    async def _iframe_contains_doc_or_body(self, frame: Union[Frame, ElementHandle]) -> bool:
+        """
+        Checks if an iframe contains document or body.
+
+        Parameters:
+        ----------
+        frame (Frame): The iframe to check.
+
+        Returns:
+        --------
+        bool: True if iframes contains these elements, False otherwise.
+        """
+        frame_context = await frame.content_frame()
+
+        if not frame_context:
+            return True
+
+        return await frame_context.evaluate(load_js("iframe_contains_doc_or_body"))
+
     async def _get_page_accessibility_tree(
         self, context: Union[Page, Frame], include_aria_hidden: bool = False
     ) -> dict:
         """
         Retrieves the accessibility tree for the given page.
 
         Parameters:
@@ -500,15 +557,15 @@
         url (str): The URL to navigate to.
         storgate_state_content (optional): The storage state with which user would like to initialize the browser.
         """
 
         self._current_page = None
         url = ensure_url_scheme(url)
 
-        if not self._context:
+        if not self._browser or not self._context:
             raise NoOpenBrowserError()
 
         try:
             page = await self._context.new_page()
             if self._stealth_mode_config is not None:
                 await self._apply_stealth_mode_to_page(page)
             self._current_tf_id = 0
@@ -656,15 +713,18 @@
         try:
             element_frame_context = self._get_frame_context(iframe_path)
             return element_frame_context.locator(f"[tf623_id='{tf623_id}']")
         except Exception as e:
             raise ElementNotFoundError(tf623_id) from e
 
     async def _determine_load_state(
-        self, monitor: PageActivityMonitor, timeout_seconds=14, wait_for_network_idle=True
+        self,
+        monitor: PageActivityMonitor,
+        timeout_seconds: int = 14,
+        wait_for_network_idle: bool = True,
     ):
         if not self._current_page:
             raise NoOpenPageError()
 
         if not self._page_monitor:
             raise ValueError("Page monitor is not initialized.")
 
@@ -678,23 +738,26 @@
                     )
                 # If the page is navigating, the evaluate function will raise an error. In this case, we wait for the page to load.
                 except Error:
                     while True:
                         if self._page_monitor.get_load_status() or time.time() - start_time > 6:
                             break
                         await asyncio.sleep(0.2)
-                    last_updated_timestamp = time.time()
+                    # monitor.check_conditions() is expecting milliseconds
+                    last_updated_timestamp = time.time() * 1000
 
-                if monitor.check_conditions(last_active_dom_time=last_updated_timestamp):
+                if monitor.is_page_ready(last_active_dom_time=last_updated_timestamp):
                     break
             else:
                 if self._page_monitor.get_load_status():
+                    trail_logger.add_event("Page ready: Page emitted 'load' event.")
                     break
 
             if time.time() - start_time > timeout_seconds:
+                trail_logger.add_event("Page ready: Timeout while waiting for page to settle.")
                 break
             await asyncio.sleep(0.1)
 
     async def _add_page_event_listeners(self):
         if not self._current_page:
             raise NoOpenPageError()
```

### Comparing `agentql-0.4.4/src/agentql/ext/playwright/playwright_driver_sync.py` & `agentql-0.4.5/src/agentql/ext/playwright/playwright_driver_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,25 +9,30 @@
     Locator,
     Page,
     StorageState,
     sync_playwright,
 )
 from playwright_stealth import StealthConfig, stealth_sync
 
-from agentql import trail_logger
+from agentql import QueryParser, trail_logger
 from agentql._core._errors import (
     AccessibilityTreeError,
+    AgentQLServerError,
+    AttributeNotFoundError,
     ElementNotFoundError,
     NoOpenBrowserError,
     NoOpenPageError,
     OpenUrlError,
+    UnableToClosePopupError,
 )
 from agentql._core._js_snippets.snippet_loader import load_js
 from agentql._core._utils import ensure_url_scheme
 from agentql.sync_api import ScrollDirection, WebDriver
+from agentql.sync_api._agentql_service import query_agentql_server
+from agentql.sync_api._response_proxy import AQLResponseProxy
 
 from ._driver_constants import RENDERER, USER_AGENT, VENDOR
 from ._driver_settings import ProxySettings, StealthModeConfig
 from ._html_constants import HTML_ROLE_MAPPING
 from ._network_monitor import PageActivityMonitor
 
 
@@ -147,14 +152,16 @@
         """
         if not self._browser:
             raise NoOpenBrowserError()
 
         if new_page or self._current_page is None:
             self._open_url(url)
         else:
+            url = ensure_url_scheme(url)
+            self._current_tf_id = 0
             self._current_page.goto(url, wait_until="domcontentloaded")
 
     @property
     def current_url(self) -> str:
         """Get the URL of the current page being processed by AgentQL.
 
         Returns:
@@ -213,14 +220,15 @@
         """
         if not self._current_page:
             raise NoOpenPageError()
 
         try:
             accessibility_tree = self._get_page_accessibility_tree(self._current_page)
             self._process_iframes(accessibility_tree)
+            self._post_process_accessibility_tree(accessibility_tree)
             return accessibility_tree
         except Exception as e:
             raise AccessibilityTreeError() from e
 
     def wait_for_page_ready_state(self, wait_for_network_idle: bool = True):
         """Wait for the page to reach the "Page Ready" state (i.e. page has entered a relatively stable state and most main content is loaded).
 
@@ -251,15 +259,15 @@
             # Reset the network monitor to clear the logs
             self._page_monitor.reset()
 
         # Add event listeners to track DOM changes and network activities
         self._add_page_event_listeners()
 
         # Wait for the page to reach the "Page Ready" state
-        self._determine_load_state(self._page_monitor, wait_for_network_idle)
+        self._determine_load_state(self._page_monitor, wait_for_network_idle=wait_for_network_idle)
 
         # Remove the event listeners to prevent overwhelming the async event loop
         self._remove_page_event_listeners()
 
         trail_logger.add_event(
             f"Finished waiting for {self._current_page} to reach 'Page Ready' state"
         )
@@ -288,14 +296,39 @@
     def scroll_to_top(self):
         """Scrolls to the top of the current page."""
         if not self._current_page:
             raise NoOpenPageError()
 
         self._current_page.evaluate(load_js("scroll_to_top"))
 
+    def _close_popup(self, popup_tree: dict, page_url: str, timeout: int = 500):
+        """Close the popup by querying AgentQL server for the close button and perform a click action with web driver.
+
+        Parameters:
+        -----------
+        popup_tree (dict): The accessibility tree that has the popup node as the parent.
+        page_url (str): The URL of the active page.
+        timeout (int) (optional): The timeout value for the connection with AgentQL server service.
+        """
+        query = """
+            {
+                popup {
+                    close_btn
+                }
+            }
+        """
+        parser = QueryParser(query)
+        query_tree = parser.parse()
+        try:
+            response = query_agentql_server(query, popup_tree, timeout, page_url)
+            agentql_response_proxy = AQLResponseProxy(response, self, query_tree)
+            agentql_response_proxy.popup.close_btn.click()
+        except (AgentQLServerError, ElementNotFoundError, AttributeNotFoundError) as e:
+            raise UnableToClosePopupError() from e
+
     def _get_user_auth_session(self) -> StorageState:
         """
         Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
 
         Returns:
         --------
         dict: User auth session in Python dictionary format.
@@ -393,14 +426,16 @@
         else:
             frame = frame.content_frame()
             if not frame:
                 return
             iframes = frame.query_selector_all("iframe")
 
         for iframe in iframes:
+            if not self._iframe_contains_doc_or_body(iframe):
+                continue
             iframe_id = iframe.get_attribute("tf623_id")
             iframe_path_to_send = ""
             if iframe_path:
                 iframe_path_to_send = f"{iframe_path}."
             iframe_path_to_send = f"{iframe_path_to_send}{iframe_id}"
             iframe_accessibility_tree = self._get_frame_accessibility_tree(
                 iframe, iframe_path_to_send
@@ -412,14 +447,33 @@
 
             self._process_iframes(
                 iframe_path=iframe_path_to_send,
                 frame=iframe,
                 page_accessibility_tree=page_accessibility_tree,
             )
 
+    def _iframe_contains_doc_or_body(self, frame: Union[Frame, ElementHandle]) -> bool:
+        """
+        Checks if an iframe contains document or body.
+
+        Parameters:
+        ----------
+        frame (Frame): The iframe to check.
+
+        Returns:
+        --------
+        bool: True if iframes contains these elements, False otherwise.
+        """
+        frame_context = frame.content_frame()
+
+        if not frame_context:
+            return True
+
+        return frame_context.evaluate(load_js("iframe_contains_doc_or_body"))
+
     def _get_page_accessibility_tree(
         self, context: Union[Page, Frame], include_aria_hidden: bool = False
     ) -> dict:
         """
         Retrieves the accessibility tree for the given page.
 
         Parameters:
@@ -667,16 +721,16 @@
             return element_frame_context.locator(f"[tf623_id='{tf623_id}']")
         except Exception as e:
             raise ElementNotFoundError(tf623_id) from e
 
     def _determine_load_state(
         self,
         monitor: PageActivityMonitor,
-        timeout_seconds=14,
-        wait_for_network_idle=True,
+        timeout_seconds: int = 14,
+        wait_for_network_idle: bool = True,
     ):
         if not self._current_page:
             raise NoOpenPageError()
 
         if not self._page_monitor:
             raise ValueError("Page monitor is not initialized.")
 
@@ -690,22 +744,25 @@
                     )
                 # If the page is navigating, the evaluate function will raise an error. In this case, we wait for the page to load.
                 except Error:
                     while True:
                         if self._page_monitor.get_load_status() or time.time() - start_time > 6:
                             break
                         time.sleep(0.2)
-                    last_updated_timestamp = time.time()
+                    # monitor.check_conditions() is expecting milliseconds
+                    last_updated_timestamp = time.time() * 1000
 
-                if monitor.check_conditions(last_active_dom_time=last_updated_timestamp):
+                if monitor.is_page_ready(last_active_dom_time=last_updated_timestamp):
                     break
             else:
                 if self._page_monitor.get_load_status():
+                    trail_logger.add_event("Page ready: Page emitted 'load' event.")
                     break
             if time.time() - start_time > timeout_seconds:
+                trail_logger.add_event("Page ready: Timeout while waiting for page to settle.")
                 break
             time.sleep(0.1)
 
     def _add_page_event_listeners(self):
         if not self._current_page:
             raise NoOpenPageError()
```

### Comparing `agentql-0.4.4/src/agentql/sync_api/_api.py` & `agentql-0.4.5/src/agentql/sync_api/_api.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.4/src/agentql/sync_api/_popup.py` & `agentql-0.4.5/src/agentql/sync_api/_popup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from typing import Callable
 
 
 class Popup:
     """Popup objects are dispatched by session via session.on("popup") event. For each popup window detected on the page, there will be corresponding event and popup objects emitted."""
 
-    def __init__(self, popup_tree: dict, popup_name: str, on_popup_close: Callable[[dict], None]):
+    def __init__(
+        self,
+        page_url: str,
+        popup_tree: dict,
+        popup_name: str,
+        on_popup_close: Callable[[dict], None],
+    ):
+        self._page_url = page_url
         self._tree = popup_tree
         self._name = popup_name
         self._close_popup_callback = on_popup_close
 
     def __str__(self):
-        return f"Popup {self._name}"
+        return f"Popup {self._name} on page {self._page_url}"
 
     @property
     def accessibility_tree(self) -> dict:
         """
         Returns the part of accessibility tree where the popup node as the parent.
 
         Returns:
@@ -30,17 +37,28 @@
 
         Returns:
         --------
         str: The name of the popup.
         """
         return self._name
 
+    @property
+    def page_url(self) -> str:
+        """
+        Returns the URL of the page where the popup occurred.
+
+        Returns:
+        --------
+        str: The URL of the page where the popup occurred.
+        """
+        return self._page_url
+
     def close(self):
         """Close the popup by invoking the callback function passed into the Popup object when it is initialized."""
-        self._close_popup_callback(self._tree)
+        self._close_popup_callback(self._tree, self._page_url)
 
 
 def close_all_popups_handler(popups: list):
     """This is a handler function for popups. Passing it as the callback function into session.on("popup") method will close all popups.
 
     Parameters:
     ----------
```

### Comparing `agentql-0.4.4/src/agentql/sync_api/_response_proxy.py` & `agentql-0.4.5/src/agentql/sync_api/_response_proxy.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,21 @@
         self._query_tree_node = query_tree
 
     def __getattr__(
         self, name
     ) -> Union["AQLResponseProxy[InteractiveItemTypeT]", InteractiveItemTypeT, None]:
         if self._response_data is None:
             raise AttributeError("Response data is None")
+
         if name not in self._response_data:
-            raise AttributeNotFoundError(name, self._response_data)
+            raise AttributeNotFoundError(name, self._response_data, self._query_tree_node)
         trail_logger.add_event(f"Resolving element {name} on {self._web_driver.current_url}")
+
         return self._resolve_item(
-            self._response_data[name], self._query_tree_node.get_child_by_name(name)
+            self._response_data[name], query_tree_node=self._query_tree_node.get_child_by_name(name)
         )
 
     def __getitem__(
         self, index: int
     ) -> Union[InteractiveItemTypeT, "AQLResponseProxy[InteractiveItemTypeT]", None]:
         if not isinstance(self._response_data, list):
             raise ValueError("This node is not a list")
@@ -86,17 +88,20 @@
 
         ```py
         {
         "query_field": "text content of the corresponding web element"
         }
         ```
         """
-        return self._to_data_node(self._response_data, self._query_tree_node)
+        res = self._to_data_node(self._response_data, self._query_tree_node)
+        if not isinstance(res, dict):
+            raise TypeError("Root node must be a container node")
+        return res
 
-    def _to_data_node(self, response_data, query_tree_node) -> dict:
+    def _to_data_node(self, response_data, query_tree_node) -> Union[dict, list, str, None]:
         if isinstance(query_tree_node, ContainerListNode):
             return self._to_data_container_list_node(response_data, query_tree_node)
         elif isinstance(query_tree_node, ContainerNode):
             return self._to_data_container_node(response_data, query_tree_node)
         elif isinstance(query_tree_node, IdListNode):
             return self._to_data_id_list_node(response_data)
         elif isinstance(query_tree_node, IdNode):
```

### Comparing `agentql-0.4.4/src/agentql/sync_api/_session.py` & `agentql-0.4.5/src/agentql/sync_api/_session.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,17 @@
 # pylint: disable=protected-access
 
 import copy
-import json
 import logging
-import os
 from typing import Callable, Generic, List, Literal, Optional, Union
 
-import requests
-
-from agentql import (
-    AgentQLServerError,
-    AgentQLServerTimeoutError,
-    APIKeyError,
-    AttributeNotFoundError,
-    QueryParser,
-    UnableToClosePopupError,
-    trail_logger,
-)
-from agentql._core._api_constants import GET_AGENTQL_ENDPOINT, SERVICE_URL
+from agentql import QueryParser, trail_logger
 from agentql._core._utils import minify_query
 
+from ._agentql_service import query_agentql_server
 from ._popup import Popup
 from ._response_proxy import AQLResponseProxy
 from ._web_driver import InteractiveItemTypeT, PageTypeT, WebDriver
 
 log = logging.getLogger("agentql")
 
 RESPONSE_ERROR_KEY = "detail"
@@ -36,24 +24,20 @@
         """Initialize the session.
 
         Parameters:
         ----------
         web_driver (WebDriver): The web driver that will be used in this session.
         """
 
-        self._api_key = os.getenv("AGENTQL_API_KEY")
-        if not self._api_key:
-            raise APIKeyError(
-                "API key not provided. Please set the environment variable 'AGENTQL_API_KEY' with your API key."
-            )
         self._web_driver = web_driver
         self._event_listeners = {}
         self._check_popup = False
         self._last_query = None
         self._last_response = None
+        self._last_accessibility_tree = None
 
     @property
     def current_page(self) -> PageTypeT:
         """Get the current page being processed by AgentQL.
 
         Returns:
         -------
@@ -77,14 +61,19 @@
         return self._last_query
 
     @property
     def last_response(self) -> Optional[dict]:
         """Get the last response."""
         return self._last_response
 
+    @property
+    def last_accessibility_tree(self) -> Optional[dict]:
+        """Get the last captured accessibility tree"""
+        return self._last_accessibility_tree
+
     def get_last_trail(self) -> Union[trail_logger.TrailLogger, None]:
         """
         Get the last trail recorded, if enable_history_log is True when starting the session.
         """
         logger_store = trail_logger.TrailLoggerStore.get_loggers()
         return logger_store[-1] if logger_store else None
 
@@ -109,14 +98,15 @@
 
         Parameters:
         ----------
         query (str): The AgentQL query in String format.
         timeout (int) (optional): Optional timeout value for the connection with backend api service.
         lazy_load_pages_count (int) (optional): The number of pages to scroll down and up to load lazy loaded content.
         wait_for_network_idle (bool) (optional): Whether to wait for the network to be idle before querying the page.
+        include_aria_hidden (bool) (optional): Whether to include elements with aria-hidden attribute in the accessibility tree.
 
         Returns:
         -------
         AQLResponseProxy: AgentQL Response (Elements that match the query) of AQLResponseProxy type.
         """
         trail_logger.add_event(f"Querying {minify_query(query)} on {self.current_page}")
         log.debug(f"querying {query}")
@@ -126,22 +116,26 @@
         query_tree = parser.parse()
 
         self._web_driver.wait_for_page_ready_state(wait_for_network_idle)
 
         accessibility_tree = self._web_driver._prepare_accessibility_tree(
             lazy_load_pages_count=lazy_load_pages_count, include_aria_hidden=include_aria_hidden
         )
+        self._last_accessibility_tree = accessibility_tree
 
+        popup_list = []
         # Check if there is a popup in the page before sending the agentql query
         if self._check_popup:
             popup_list = self._detect_popup(accessibility_tree, [])
             if popup_list:
                 self._handle_popup(popup_list)
 
-        response = self._query(query, accessibility_tree, timeout)
+        response = query_agentql_server(
+            query, accessibility_tree, timeout, self._web_driver.current_url
+        )
         self._last_response = response
 
         # Check if there is a popup in the page after receiving the agentql response
         if self._check_popup:
             # Fetch the most up-to-date accessibility tree
             accessibility_tree = self._web_driver.accessibility_tree
 
@@ -166,60 +160,14 @@
         """
         self._event_listeners[event] = callback
         if callback:
             self._check_popup = True
         else:
             self._check_popup = False
 
-    def _query(self, query: str, accessibility_tree: dict, timeout: int) -> dict:
-        """Make Request to AgentQL API.
-
-        Parameters:
-        ----------
-        query (str): The query string.
-        accessibility_tree (dict): The accessibility tree.
-        timeout (int): The timeout value for the connection with backend api service
-
-        Returns:
-        -------
-        dict: AgentQL response in json format.
-        """
-        try:
-            page_url = self._web_driver.current_url
-            request_data = {
-                "query": f"{query}",
-                "accessibility_tree": accessibility_tree,
-                "metadata": {"url": page_url},
-            }
-            url = os.getenv("AGENTQL_API_HOST", SERVICE_URL) + GET_AGENTQL_ENDPOINT
-            log.debug(f"Making request to {url}")
-            headers = {"X-API-Key": self._api_key}
-            response = requests.post(
-                url, json=request_data, headers=headers, timeout=timeout, allow_redirects=True
-            )
-            response.raise_for_status()
-            return response.json()
-        except requests.exceptions.RequestException as e:
-            if isinstance(e, requests.exceptions.ReadTimeout):
-                raise AgentQLServerTimeoutError() from e
-            if isinstance(e, requests.exceptions.HTTPError) and e.response.status_code == 401:
-                raise APIKeyError(
-                    "Invalid or expired API key provided. Please set the environment variable 'AGENTQL_API_KEY' with a valid API key."
-                ) from e
-            error_code = e.response.status_code if e.response is not None else None
-            server_error = e.response.content.decode("utf-8") if e.response is not None else None
-            if server_error:
-                try:
-                    server_error_json = json.loads(server_error)
-                    if isinstance(server_error_json, dict):
-                        server_error = server_error_json.get(RESPONSE_ERROR_KEY)
-                except ValueError:
-                    raise AgentQLServerError(server_error, error_code) from e
-            raise AgentQLServerError(server_error, error_code) from e
-
     def _detect_popup(self, tree: dict, known_popups: List[Popup]) -> List[Popup]:
         """Detect if there is a popup in the page. If so, create a Popup object and add it to the popup dict.
 
         Parameters:
         ----------
         tree (dict): The accessibility tree.
         known_popups (list): The list of known popups.
@@ -228,15 +176,20 @@
         --------
         popups (list): The list of popups.
         """
         tree_role = tree.get("role", "")
         tree_name = tree.get("name", "")
         popup_list = []
         if tree_role == "dialog":
-            popup = Popup(copy.deepcopy(tree), tree_name, self._close_popup)
+            popup = Popup(
+                self._web_driver.current_url,
+                copy.deepcopy(tree),
+                tree_name,
+                self._web_driver._close_popup,
+            )
 
             # Avoid adding existing popup to the dict and double handle the popup
             if known_popups:
                 for popup_object in known_popups:
                     if popup_object.name != popup.name:
                         popup_list.append(popup)
             else:
@@ -254,33 +207,7 @@
         """Handle the popup. If there is a popup in the list, and there is an event listener, emit the popup event by invoking the callback function.
 
         Parameters:
         ----------
         popups (list): The list of popups to handle."""
         if popups and "popup" in self._event_listeners and self._event_listeners["popup"]:
             self._event_listeners["popup"](popups)
-
-    def _close_popup(self, tree: dict):
-        """Close the popup by querying AgentQL server and click the close button.
-
-        Parameters:
-        ----------
-        popup (Popup): The popup to close.
-        query (str): The query to close the popup.
-        """
-        query = """
-            {
-                popup {
-                    close_btn
-                }
-            }
-        """
-        parser = QueryParser(query)
-        query_tree = parser.parse()
-        try:
-            response = self._query(query, tree, 500)
-            agentql_response = AQLResponseProxy[InteractiveItemTypeT](
-                response, self._web_driver, query_tree
-            )
-            agentql_response.popup.close_btn.click()
-        except (AgentQLServerError, AttributeNotFoundError) as e:
-            raise UnableToClosePopupError() from e
```

### Comparing `agentql-0.4.4/src/agentql/sync_api/_web_driver.py` & `agentql-0.4.5/src/agentql/sync_api/_web_driver.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,14 +83,24 @@
         """Returns the page object that represents the current page. Users should be able to do more fine grained interaction using this page object, such as navigating to a different url or take screenshot of the page.
 
         Returns:
         --------
         PageTypeT: The current page object.
         """
 
+    def _close_popup(self, popup_tree: dict, page_url: str, timeout: int = 500):
+        """Close the popup on the page.
+
+        Parameters:
+        -----------
+        popup_tree (dict): The accessibility tree that has the popup node as the parent.
+        page_url (str): The URL of the active page.
+        timeout (int) (optional): The timeout value for the connection with AgentQL server service.
+        """
+
     def _get_user_auth_session(self) -> Any:
         """Returns the user authentication session that contains the login session state of current browser. User could pass this information when starting the session to preserve previous login state.
 
         Returns:
         --------
         The user session state.
         """
```

### Comparing `agentql-0.4.4/src/agentql/trail_logger/trail_logger.py` & `agentql-0.4.5/src/agentql/_core/_trail_logger/_trail_logger_impl.py`

 * *Files identical despite different names*

### Comparing `agentql-0.4.4/PKG-INFO` & `agentql-0.4.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: agentql
-Version: 0.4.4
+Version: 0.4.5
 Summary: Tiny Fish AgentQL Python Client
 License: MIT
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23,<24)
-Requires-Dist: httpx (>=0.26,<0.27)
+Requires-Dist: httpx (>=0,<1)
 Requires-Dist: playwright (>=1,<2)
 Requires-Dist: pydantic (>=2,<3)
-Requires-Dist: pytest-asyncio (>=0.23,<0.24)
+Requires-Dist: pytest-asyncio (>=0,<1)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: tf-playwright-stealth
+Requires-Dist: typer (>=0,<1)
 Description-Content-Type: text/markdown
 
 # Tiny Fish AgentQL Python Client
 
 A Python client for Tiny Fish AgentQL - a new way to interact with the web.
```

