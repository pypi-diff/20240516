# Comparing `tmp/galileo_observe-1.0.1.tar.gz` & `tmp/galileo_observe-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_observe-1.0.1.tar", max compression
+gzip compressed data, was "galileo_observe-1.1.0.tar", max compression
```

## Comparing `galileo_observe-1.0.1.tar` & `galileo_observe-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    11357 2024-03-25 22:02:11.304854 galileo_observe-1.0.1/LICENSE
--rw-r--r--   0        0        0      221 2024-03-25 22:02:11.304854 galileo_observe-1.0.1/README.md
--rw-r--r--   0        0        0      251 2024-03-25 22:02:11.304854 galileo_observe-1.0.1/galileo_observe/__init__.py
--rw-r--r--   0        0        0        0 2024-03-25 22:02:11.304854 galileo_observe-1.0.1/galileo_observe/constants/__init__.py
--rw-r--r--   0        0        0      889 2024-03-25 22:02:11.304854 galileo_observe-1.0.1/galileo_observe/constants/routes.py
--rw-r--r--   0        0        0    17070 2024-03-25 22:02:11.304854 galileo_observe-1.0.1/galileo_observe/handlers.py
--rw-r--r--   0        0        0     7653 2024-03-25 22:02:11.304854 galileo_observe-1.0.1/galileo_observe/monitor.py
--rw-r--r--   0        0        0        0 2024-03-25 22:02:11.304854 galileo_observe-1.0.1/galileo_observe/schema/__init__.py
--rw-r--r--   0        0        0     1330 2024-03-25 22:02:11.304854 galileo_observe-1.0.1/galileo_observe/schema/transaction.py
--rw-r--r--   0        0        0       22 2024-03-25 22:02:12.124861 galileo_observe-1.0.1/galileo_observe/utils/__init__.py
--rw-r--r--   0        0        0     5235 2024-03-25 22:02:11.304854 galileo_observe-1.0.1/galileo_observe/utils/api_client.py
--rw-r--r--   0        0        0     1738 2024-03-25 22:02:11.304854 galileo_observe-1.0.1/galileo_observe/utils/request.py
--rw-r--r--   0        0        0     2536 2024-03-25 22:02:12.120860 galileo_observe-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1200 1970-01-01 00:00:00.000000 galileo_observe-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/LICENSE
+-rw-r--r--   0        0        0      221 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/README.md
+-rw-r--r--   0        0        0      372 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/__init__.py
+-rw-r--r--   0        0        0    15663 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/async_handlers.py
+-rw-r--r--   0        0        0        0 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/constants/__init__.py
+-rw-r--r--   0        0        0      889 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/constants/routes.py
+-rw-r--r--   0        0        0    17098 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/handlers.py
+-rw-r--r--   0        0        0     7681 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/monitor.py
+-rw-r--r--   0        0        0        0 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/schema/__init__.py
+-rw-r--r--   0        0        0     1376 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/schema/transaction.py
+-rw-r--r--   0        0        0       22 2024-05-16 17:54:34.549450 galileo_observe-1.1.0/galileo_observe/utils/__init__.py
+-rw-r--r--   0        0        0     6746 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/utils/api_client.py
+-rw-r--r--   0        0        0     2255 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/utils/request.py
+-rw-r--r--   0        0        0     2554 2024-05-16 17:54:34.549450 galileo_observe-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 galileo_observe-1.1.0/PKG-INFO
```

### Comparing `galileo_observe-1.0.1/LICENSE` & `galileo_observe-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_observe-1.0.1/galileo_observe/constants/routes.py` & `galileo_observe-1.1.0/galileo_observe/constants/routes.py`

 * *Files identical despite different names*

### Comparing `galileo_observe-1.0.1/galileo_observe/handlers.py` & `galileo_observe-1.1.0/galileo_observe/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import time
 from datetime import datetime
 from http import HTTPStatus
 from json import dumps
 from typing import Any, Dict, List, Optional, Sequence, Union
 from uuid import UUID
 
@@ -105,15 +106,15 @@
                     batch_records.append(v)
                     del self.records[k]
 
             transaction_batch = TransactionRecordBatch(
                 records=batch_records,
                 logging_method=TransactionLoggingMethod.py_langchain,
             )
-            self.client.ingest_batch(transaction_batch)
+            asyncio.run(self.client.ingest_batch(transaction_batch))
 
     def on_llm_start(
         self,
         serialized: Dict[str, Any],
         prompts: List[str],
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
```

### Comparing `galileo_observe-1.0.1/galileo_observe/monitor.py` & `galileo_observe-1.1.0/galileo_observe/monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import time
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 from uuid import uuid4
 
 import pytz
 
@@ -78,15 +79,15 @@
                     batch_records.append(v)
                     del self.records[k]
 
             transaction_batch = TransactionRecordBatch(
                 records=batch_records,
                 logging_method=TransactionLoggingMethod.py_logger,
             )
-            self.client.ingest_batch(transaction_batch)
+            asyncio.run(self.client.ingest_batch(transaction_batch))
 
     def log_node_start(
         self,
         node_type: TransactionRecordType,
         input_text: str,
         model: Optional[str] = None,
         temperature: Optional[float] = None,
```

### Comparing `galileo_observe-1.0.1/galileo_observe/schema/transaction.py` & `galileo_observe-1.1.0/galileo_observe/schema/transaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     tool = "tool"
     agent = "agent"
     retriever = "retriever"
 
 
 class TransactionLoggingMethod(str, Enum):
     py_langchain = "py_langchain"
+    py_langchain_async = "py_langchain_async"
     py_logger = "py_logger"
 
 
 class TransactionRecord(BaseModel):
     latency_ms: Optional[int] = None
     status_code: Optional[int] = None
     input_text: str
```

### Comparing `galileo_observe-1.0.1/galileo_observe/utils/api_client.py` & `galileo_observe-1.1.0/galileo_observe/utils/api_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
+from asyncio import run as asyncio_run
 from os import getenv
 from time import time
-from typing import Any, Callable, Dict, Optional, Union
+from typing import Any, Dict, Optional, Union
 
 import jwt
-from requests import get, post
 
 from galileo_observe.constants.routes import Routes
 from galileo_observe.schema.transaction import TransactionRecordBatch
 from galileo_observe.utils import __version__ as client_version
 from galileo_observe.utils.request import HttpHeaders, make_request
 
 
@@ -52,50 +52,56 @@
             return self.username_login(username, password).get("access_token", "")
 
         raise Exception(
             "GALILEO_API_KEY or GALILEO_USERNAME and GALILEO_PASSWORD must be set"
         )
 
     def healthcheck(self) -> bool:
-        make_request(get, base_url=self.base_url, endpoint=Routes.healthcheck)
+        asyncio_run(
+            make_request("get", base_url=self.base_url, endpoint=Routes.healthcheck)
+        )
         return True
 
     def username_login(self, username: str, password: str) -> Dict[str, str]:
-        return make_request(
-            post,
-            base_url=self.base_url,
-            endpoint=Routes.login,
-            data={
-                "username": username,
-                "password": password,
-                "auth_method": "email",
-            },
+        return asyncio_run(
+            make_request(
+                "post",
+                base_url=self.base_url,
+                endpoint=Routes.login,
+                data={
+                    "username": username,
+                    "password": password,
+                    "auth_method": "email",
+                },
+            )
         )
 
     def api_key_login(self, api_key: str) -> Dict[str, str]:
-        return make_request(
-            post,
-            base_url=self.base_url,
-            endpoint=Routes.api_key_login,
-            body={
-                "api_key": api_key,
-            },
+        return asyncio_run(
+            make_request(
+                "post",
+                base_url=self.base_url,
+                endpoint=Routes.api_key_login,
+                body={
+                    "api_key": api_key,
+                },
+            )
         )
 
     @property
     def base_url(self) -> str:
         return self.api_url
 
     @property
     def auth_header(self) -> Dict[str, str]:
         return {"Authorization": f"Bearer {self.token}"}
 
     def _make_request(
         self,
-        request_method: Callable,
+        request_method: str,
         endpoint: str,
         body: Optional[Dict] = None,
         data: Optional[Dict] = None,
         files: Optional[Dict] = None,
         params: Optional[Dict] = None,
         timeout: Union[int, None] = None,
         json_request_only: bool = False,
@@ -108,43 +114,82 @@
                 self.token = self.get_token()
 
         if json_request_only:
             content_headers = HttpHeaders.accept_json()
         else:
             content_headers = HttpHeaders.json()
         headers = {**self.auth_header, **content_headers}
-        return make_request(
+        return asyncio_run(
+            make_request(
+                request_method=request_method,
+                base_url=self.base_url,
+                endpoint=endpoint,
+                body=body,
+                data=data,
+                files=files,
+                params=params,
+                headers=headers,
+                timeout=timeout,
+            )
+        )
+
+    async def _make_async_request(
+        self,
+        request_method: str,
+        endpoint: str,
+        body: Optional[Dict] = None,
+        data: Optional[Dict] = None,
+        files: Optional[Dict] = None,
+        params: Optional[Dict] = None,
+        timeout: Union[int, None] = None,
+        json_request_only: bool = False,
+    ) -> Any:
+        # Check to see if our token is expired before making a request
+        # and refresh token if it's expired
+        if endpoint not in [Routes.login, Routes.api_key_login] and self.token:
+            claims = jwt.decode(self.token, options={"verify_signature": False})
+            if claims.get("exp", 0) < time():
+                self.token = self.get_token()
+
+        if json_request_only:
+            content_headers = HttpHeaders.accept_json()
+        else:
+            content_headers = HttpHeaders.json()
+        headers = {**self.auth_header, **content_headers}
+        await make_request(
             request_method=request_method,
             base_url=self.base_url,
             endpoint=endpoint,
             body=body,
             data=data,
             files=files,
             params=params,
             headers=headers,
             timeout=timeout,
         )
 
-    def ingest_batch(self, transaction_batch: TransactionRecordBatch) -> Dict[str, str]:
+    async def ingest_batch(
+        self, transaction_batch: TransactionRecordBatch
+    ) -> Dict[str, str]:
         transaction_batch.client_version = client_version
-        return self._make_request(
-            post,
+        return await self._make_async_request(
+            "post",
             endpoint=Routes.ingest.format(project_id=self.project_id),
             body=transaction_batch.model_dump(),
         )
 
     def get_project_by_name(self, project_name: str) -> Any:
         projects = self._make_request(
-            get,
+            "get",
             endpoint=Routes.projects,
             params={"project_name": project_name},
         )
         if len(projects) < 1:
             raise Exception(f"Galileo project {project_name} not found")
         return projects[0]
 
     def create_project(self, project_name: str) -> Dict[str, str]:
         return self._make_request(
-            post,
+            "post",
             endpoint=Routes.projects,
             body={"name": project_name, "type": "llm_monitor"},
         )
```

### Comparing `galileo_observe-1.0.1/galileo_observe/utils/request.py` & `galileo_observe-1.1.0/galileo_observe/utils/request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,60 @@
 from enum import Enum
 from http.client import HTTPException
-from typing import Any, Callable, Dict, Optional, Union
+from typing import Any, Dict, Optional, Union
 from urllib.parse import urljoin
 
 import backoff
-from requests import RequestException, Response
+import httpx
+from requests import RequestException
 
 
-def _validate_response(response: Response) -> None:
-    if not response.ok:
+async def _validate_response(response: httpx.Response) -> None:
+    if not response.status_code < 300:
         msg = (
             "Something didn't go quite right. The api returned a non-ok status "
             f"code {response.status_code} with output: {response.text}"
         )
         # TODO: Better error handling.
         raise HTTPException(msg)
 
 
 @backoff.on_exception(backoff.expo, RequestException, max_tries=4, jitter=None)
-def make_request(
-    request_method: Callable,
+async def make_request(
+    request_method: str,
     base_url: str,
     endpoint: str,
     body: Optional[Dict] = None,
     data: Optional[Dict] = None,
     files: Optional[Dict] = None,
     params: Optional[Dict] = None,
     headers: Optional[Dict[str, str]] = None,
     timeout: Union[int, None] = None,
 ) -> Any:
-    response = request_method(
-        urljoin(base_url, endpoint),
-        json=body,
-        data=data,
-        files=files,
-        params=params,
-        headers=headers or {},
-        timeout=timeout,
-    )
-    _validate_response(response)
+    async with httpx.AsyncClient() as client:
+        if request_method == "get":
+            response = await client.get(
+                urljoin(base_url, endpoint),
+                params=params,
+                headers=headers or {},
+                timeout=timeout,
+            )
+        elif request_method == "post":
+            response = await client.post(
+                urljoin(base_url, endpoint),
+                json=body,
+                data=data,
+                files=files,
+                params=params,
+                headers=headers or {},
+                timeout=timeout,
+            )
+        else:
+            raise ValueError(f"Unsupported request method {request_method}")
+    await _validate_response(response)
     return response.json()
 
 
 class HttpHeaders(str, Enum):
     accept = "accept"
     content_type = "Content-Type"
     application_json = "application/json"
```

### Comparing `galileo_observe-1.0.1/pyproject.toml` & `galileo_observe-1.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "galileo-observe"
-version = "1.0.1"
+version = "1.1.0"
 description = "📈 Monitor your LLM integration with Galileo Observe!"
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.13"
 requests = "^2.31.0"
@@ -13,14 +13,15 @@
 pytz = "^2023.3"
 pyjwt = "^2.8.0"
 cryptography = "^42.0.0"
 backoff = "^2.2.1"
 types-pytz = "^2023.3.1.1"
 tiktoken = "^0.5.2"
 langchain = ">=0.1,<0.2"
+httpx = "^0.27.0"
 
 [tool.poetry.extras]
 langchain = ["langchain"]
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.1"
```

### Comparing `galileo_observe-1.0.1/PKG-INFO` & `galileo_observe-1.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: galileo-observe
-Version: 1.0.1
+Version: 1.1.0
 Summary: 📈 Monitor your LLM integration with Galileo Observe!
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: langchain
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: cryptography (>=42.0.0,<43.0.0)
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: langchain (>=0.1,<0.2) ; extra == "langchain"
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tiktoken (>=0.5.2,<0.6.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
```

