# Comparing `tmp/pytest_kookit-0.1.1.tar.gz` & `tmp/pytest_kookit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_kookit-0.1.1.tar", max compression
+gzip compressed data, was "pytest_kookit-0.1.2.tar", max compression
```

## Comparing `pytest_kookit-0.1.1.tar` & `pytest_kookit-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0       54 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/README.md
--rw-r--r--   0        0        0       49 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/__init__.py
--rw-r--r--   0        0        0     1401 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/client_side.py
--rw-r--r--   0        0        0       44 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/__init__.py
--rw-r--r--   0        0        0      823 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/interfaces.py
--rw-r--r--   0        0        0     3669 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/kookit.py
--rw-r--r--   0        0        0      214 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/models/__init__.py
--rw-r--r--   0        0        0      772 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/models/json_request.py
--rw-r--r--   0        0        0      597 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/models/json_response.py
--rw-r--r--   0        0        0     1721 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/models/request.py
--rw-r--r--   0        0        0     2747 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/models/response.py
--rw-r--r--   0        0        0      710 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/models/xml_response.py
--rw-r--r--   0        0        0     4463 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/response_group.py
--rw-r--r--   0        0        0     1695 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/server.py
--rw-r--r--   0        0        0     8096 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/http_kookit/service.py
--rw-r--r--   0        0        0     1372 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/interfaces.py
--rw-r--r--   0        0        0     2772 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/kookit.py
--rw-r--r--   0        0        0      230 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/logging.py
--rw-r--r--   0        0        0        0 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/py.typed
--rw-r--r--   0        0        0     1392 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/kookit/utils.py
--rw-r--r--   0        0        0     3416 2024-05-14 08:52:28.729402 pytest_kookit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 pytest_kookit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-05-15 08:14:21.201347 pytest_kookit-0.1.2/README.md
+-rw-r--r--   0        0        0       49 2024-05-15 08:14:21.201347 pytest_kookit-0.1.2/kookit/__init__.py
+-rw-r--r--   0        0        0     1401 2024-05-15 08:14:21.201347 pytest_kookit-0.1.2/kookit/client_side.py
+-rw-r--r--   0        0        0       44 2024-05-15 08:14:21.201347 pytest_kookit-0.1.2/kookit/http_kookit/__init__.py
+-rw-r--r--   0        0        0      823 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/http_kookit/interfaces.py
+-rw-r--r--   0        0        0     3583 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/http_kookit/kookit.py
+-rw-r--r--   0        0        0      214 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/http_kookit/models/__init__.py
+-rw-r--r--   0        0        0      772 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/http_kookit/models/json_request.py
+-rw-r--r--   0        0        0      597 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/http_kookit/models/json_response.py
+-rw-r--r--   0        0        0     1721 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/http_kookit/models/request.py
+-rw-r--r--   0        0        0     2747 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/http_kookit/models/response.py
+-rw-r--r--   0        0        0      710 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/http_kookit/models/xml_response.py
+-rw-r--r--   0        0        0     4463 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/http_kookit/response_group.py
+-rw-r--r--   0        0        0     1778 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/http_kookit/server.py
+-rw-r--r--   0        0        0     7782 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/http_kookit/service.py
+-rw-r--r--   0        0        0     1261 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/interfaces.py
+-rw-r--r--   0        0        0     2944 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/kookit.py
+-rw-r--r--   0        0        0      230 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/logging.py
+-rw-r--r--   0        0        0        0 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/py.typed
+-rw-r--r--   0        0        0     2980 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/kookit/utils.py
+-rw-r--r--   0        0        0     3416 2024-05-15 08:14:21.205347 pytest_kookit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1325 1970-01-01 00:00:00.000000 pytest_kookit-0.1.2/PKG-INFO
```

### Comparing `pytest_kookit-0.1.1/kookit/client_side.py` & `pytest_kookit-0.1.2/kookit/client_side.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.1/kookit/http_kookit/interfaces.py` & `pytest_kookit-0.1.2/kookit/http_kookit/interfaces.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.1/kookit/http_kookit/kookit.py` & `pytest_kookit-0.1.2/kookit/http_kookit/kookit.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from __future__ import annotations
 import os
-import queue
-import time
-from contextlib import suppress
 from itertools import cycle
 from typing import TYPE_CHECKING, Final, Iterable
 
 from multiprocess import Process
 from typing_extensions import Self
 
 from kookit.logging import logger
+from kookit.utils import ProcessManager
 from .server import KookitHTTPServer
 from .service import KookitHTTPService
 
 
 if TYPE_CHECKING:
     from types import TracebackType
 
@@ -30,15 +28,22 @@
 class HTTPKookit:
     server_port: Final[cycle] = cycle(i for i in range(29000, 30000))
 
     def __init__(self, mocker: MockerFixture) -> None:
         self.mocker: Final[MockerFixture] = mocker
         self.server: Final[KookitHTTPServer] = KookitHTTPServer(next(self.server_port))
         self.services: Final[list[KookitHTTPService]] = []
-        self.server_process: Process | None = None
+        self.process_manager: ProcessManager | None = None
+        self.startup_timeout: float = KookitHTTPService.DEFAULT_STARTUP_TIMEOUT
+
+    def __call__(self, startup_timeout: float) -> Self:
+        self.startup_timeout = startup_timeout
+        for service in self.services:
+            service(startup_timeout=startup_timeout)
+        return self
 
     def __str__(self) -> str:
         return "[HTTPKookit]"
 
     def new_service(
         self,
         env_var: str,
@@ -69,54 +74,45 @@
         return service
 
     def __enter__(self) -> Self:
         # 1. start global server
         # 2. start all other services' servers.
         not_unique = [s for s in self.services if not s.unique_url]
 
-        if not_unique and not self.server_process:
-            self.server_process = Process(
+        if not_unique and not self.process_manager:
+            server_process = Process(
                 target=self.server.run,
                 args=(
                     [s.router for s in not_unique],
                     [s.lifespan for s in not_unique],
                 ),
             )
-            self.server_process.start()
-            time.sleep(0.01)
 
-            with suppress(queue.Empty):
-                is_started = self.server.wait()
-                if not is_started:
-                    msg = f"{self}: bad value received from server while starting"
-                    raise ValueError(msg)
+            self.process_manager = ProcessManager(
+                server_process,
+                startup_timeout=self.startup_timeout,
+                parent=f"{self}[{self.server.url}]",
+                wait_func=self.server.wait,
+            )
+            self.process_manager.__enter__()
 
         for service in self.services:
             service.__enter__()
 
         return self
 
     def __exit__(
         self,
         typ: type[BaseException] | None,
         exc: BaseException | None,
         tb: TracebackType | None,
     ) -> None:
         # 1. stop global service
         # 2. stop all other services' servers
-        if self.server_process:
-            logger.trace(f"{self}: stop server process ({self.server.url})")
-            self.server_process.terminate()
-            time.sleep(0.01)
-
-            self.server_process = None
-
-            with suppress(queue.Empty):
-                is_started: bool = self.server.wait()
-                if is_started:
-                    msg = f"{self}: bad value received from server while stopping"
-                    raise ValueError(msg)
+        if self.process_manager:
+            self.process_manager.__exit__(typ, exc, tb)
+            self.process_manager = None
         else:
             logger.trace(f"{self}: server process already stopped")
 
         for service in self.services:
             service.__exit__(typ, exc, tb)
```

### Comparing `pytest_kookit-0.1.1/kookit/http_kookit/models/json_request.py` & `pytest_kookit-0.1.2/kookit/http_kookit/models/json_request.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.1/kookit/http_kookit/models/json_response.py` & `pytest_kookit-0.1.2/kookit/http_kookit/models/json_response.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.1/kookit/http_kookit/models/request.py` & `pytest_kookit-0.1.2/kookit/http_kookit/models/request.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.1/kookit/http_kookit/models/response.py` & `pytest_kookit-0.1.2/kookit/http_kookit/models/response.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.1/kookit/http_kookit/models/xml_response.py` & `pytest_kookit-0.1.2/kookit/http_kookit/models/xml_response.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.1/kookit/http_kookit/response_group.py` & `pytest_kookit-0.1.2/kookit/http_kookit/response_group.py`

 * *Files identical despite different names*

### Comparing `pytest_kookit-0.1.1/kookit/http_kookit/server.py` & `pytest_kookit-0.1.2/kookit/http_kookit/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+import queue
 from contextlib import asynccontextmanager
 from typing import TYPE_CHECKING, Any, Final
 
 import uvicorn
 from fastapi import APIRouter, FastAPI
 from multiprocess import Queue
 
@@ -21,15 +22,18 @@
         self.port: Final[int] = port
         self.url: Final[str] = f"http://{host}:{port}"
 
     def __str__(self) -> str:
         return "[KookitHTTPServer]"
 
     def wait(self, timeout: float | None = None) -> Any:
-        return self.queue.get(timeout=timeout)
+        try:
+            return self.queue.get(timeout=timeout)
+        except queue.Empty:
+            return False
 
     def run(
         self,
         routers: Iterable[Callable[[], APIRouter]],
         lifespans: Iterable[ILifespan],
     ) -> None:
         @asynccontextmanager
```

### Comparing `pytest_kookit-0.1.1/kookit/http_kookit/service.py` & `pytest_kookit-0.1.2/kookit/http_kookit/service.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 from __future__ import annotations
-import queue
-from contextlib import ExitStack, suppress
+from contextlib import ExitStack
 from itertools import groupby
 from threading import Thread
 from types import SimpleNamespace, TracebackType
 from typing import TYPE_CHECKING, Any, Final
 
 from fastapi import APIRouter, Request, Response
 from fastapi.responses import JSONResponse
 from multiprocess import Process
 from typing_extensions import Self
 
 from kookit.logging import logger
-from kookit.utils import ILifespan, Lifespans
+from kookit.utils import ILifespan, Lifespans, ProcessManager
 from .models import KookitHTTPRequest, KookitHTTPResponse
 from .response_group import ResponseGroup
 
 
 if TYPE_CHECKING:
     from collections.abc import Iterable, Sequence
 
     from .interfaces import IServer
 
 
 class KookitHTTPService:
+    DEFAULT_STARTUP_TIMEOUT: Final = 3
+
     def __init__(
         self,
         *,
         server: IServer,
         actions: Iterable[KookitHTTPRequest | KookitHTTPResponse] = (),
         routers: Iterable[APIRouter] = (),
         lifespans: Iterable[ILifespan] = (),
@@ -45,16 +46,23 @@
         self.add_routers(*routers)
         self.add_lifespans(*lifespans)
 
         self._unique_url: Final = unique_url
         self._name: Final = name
         self._one_off: Final = one_off
 
-        self._server_process: Process | None = None
+        self._process_manager: ProcessManager | None = None
         self._active: bool = False
+        self._startup_timeout: float = self.DEFAULT_STARTUP_TIMEOUT
+
+    def __call__(self, startup_timeout: float) -> Self:
+        if self._startup_timeout == self.DEFAULT_STARTUP_TIMEOUT:
+            self._startup_timeout = startup_timeout
+
+        return self
 
     @property
     def url(self) -> str:
         return self.server.url
 
     @property
     def name(self) -> str:
@@ -112,87 +120,73 @@
         for r in self.routers:
             router.include_router(r)
 
         for group in self._response_groups:
             if group.response:
                 router.add_api_route(
                     group.path,
-                    self.__call__,
+                    self.__endpoint__,
                     methods=[group.method],
                 )
 
         logger.trace(f"{self}: routes: {chr(10).join(str(r) for r in router.routes)}")
         return router
 
     @property
     def lifespan(self) -> ILifespan:
         return Lifespans(*self.lifespans)
 
-    def start(self, *, wait_for_start_timeout: float | None = None) -> None:
+    def start(self) -> None:
         if self._active:
             logger.trace(f"{self}: service already started")
             return
 
         logger.trace(f"{self}: starting with response groups: {self._response_groups}")
 
         with ExitStack() as stack:
             _ = [
                 stack.enter_context(group) for group in self._response_groups if not group.response
             ]
 
-        if self._unique_url and not self._server_process:
+        if self._unique_url and not self._process_manager:
             logger.trace(f"{self}: starting server process [{self.url}]")
-            self._server_process = Process(
+            server_process = Process(
                 target=self.server.run,
                 args=([self.router], [self.lifespan]),
             )
-            self._server_process.start()
-
-            logger.trace(
-                f"{self}: waiting for server process to start ({wait_for_start_timeout} seconds)",
+            self._process_manager = ProcessManager(
+                server_process,
+                startup_timeout=self._startup_timeout,
+                parent=f"{self}[{self.url}]",
+                wait_func=self.server.wait,
             )
-            with suppress(queue.Empty):
-                is_started = self.server.wait(wait_for_start_timeout)
-                if not is_started:
-                    msg = f"{self}: bad value received from server while starting"
-                    raise ValueError(msg)
-            logger.trace(f"{self}: server process successfully started")
+            self._process_manager.__enter__()
 
         self._active = True
 
     def stop(
         self,
         exc_type: type[BaseException] | None = None,
         exc_val: BaseException | None = None,
         exc_tb: TracebackType | None = None,
-        *,
-        wait_for_stop_timeout: float | None = None,
     ) -> None:
         if self._one_off:
             self.actions.clear()
             self.routers.clear()
             self.lifespans.clear()
 
-        if self._unique_url and self._server_process:
+        if self._unique_url and self._process_manager:
             logger.trace(f"{self}: stop server process")
-            self._server_process.terminate()
-            self._server_process = None
-
-            with suppress(queue.Empty):
-                is_started: bool = self.server.wait(wait_for_stop_timeout)
-                if is_started:
-                    msg = f"{self}: bad value received from server while stopping"
-                    raise ValueError(msg)
+            self._process_manager.__exit__(exc_type, exc_val, exc_tb)
+            self._process_manager = None
 
         active_groups = [group for group in self._response_groups if group.active]
         if active_groups and not any([exc_type, exc_val, exc_tb]):
             msg = f"{self}: active groups left: {', '.join(str(g) for g in active_groups)}"
-            raise RuntimeError(
-                msg,
-            )
+            raise RuntimeError(msg)
 
         self._response_groups = []
         self._active = False
 
     @staticmethod
     def create_response_groups(
         actions: Iterable[KookitHTTPRequest | KookitHTTPResponse],
@@ -209,15 +203,15 @@
                     groups.append(ResponseGroup(parent=parent))
                 groups[-1].add_requests(*group)  # type: ignore[arg-type]
             else:
                 groups.extend(ResponseGroup(response, parent=parent) for response in group)  # type: ignore[arg-type]
 
         return groups
 
-    async def __call__(self, request: Request) -> Response:
+    async def __endpoint__(self, request: Request) -> Response:
         group: ResponseGroup | None = None
         cmp_request = SimpleNamespace(
             content=await request.body(),
             headers=request.headers,
             url=request.url,
             method=request.method,
             path_params=request.path_params,
```

### Comparing `pytest_kookit-0.1.1/kookit/interfaces.py` & `pytest_kookit-0.1.2/kookit/interfaces.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,14 @@
         typ: type[BaseException] | None,
         exc: BaseException | None,
         tb: TracebackType | None,
     ) -> None: ...
     def add_actions(self, *actions: KookitHTTPResponse | KookitHTTPRequest) -> None: ...
     def add_lifespans(self, *lifespans: ILifespan) -> None: ...
     def add_routers(self, *routers: APIRouter) -> None: ...
-    def start(self, *, wait_for_start_timeout: float | None = None) -> None: ...
+    def start(self) -> None: ...
     def stop(
         self,
         exc_type: type[BaseException] | None = None,
         exc_val: BaseException | None = None,
         exc_tb: TracebackType | None = None,
-        *,
-        wait_for_stop_timeout: float | None = None,
     ) -> None: ...
```

### Comparing `pytest_kookit-0.1.1/kookit/kookit.py` & `pytest_kookit-0.1.2/kookit/kookit.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,20 @@
         self.mocker: Final[MockerFixture] = mocker
         self.http_kookit: Final = HTTPKookit(mocker)
         super().__init__()
 
     def __str__(self) -> str:
         return "[kookit]"
 
+    def __call__(self, startup_timeout: float) -> Self:
+        for kookit in [self.http_kookit]:
+            kookit(startup_timeout=startup_timeout)
+
+        return self
+
     def __enter__(self) -> Self:
         logger.trace(f"{self}: starting services")
         for kookit in [self.http_kookit]:
             kookit.__enter__()
         return self
 
     def __exit__(
```

### Comparing `pytest_kookit-0.1.1/pyproject.toml` & `pytest_kookit-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "pytest-kookit"
-version = "0.1.1"
+version = "0.1.2"
 description = "Your simple but kooky integration testing with pytest"
 readme = "README.md"
 license = "MIT"
 authors = ["Dmitry Makarov <mit.makaroff@gmail.com>"]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `pytest_kookit-0.1.1/PKG-INFO` & `pytest_kookit-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-kookit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Your simple but kooky integration testing with pytest
 License: MIT
 Keywords: Integration Testing,External Services' mocks
 Author: Dmitry Makarov
 Author-email: mit.makaroff@gmail.com
 Requires-Python: >=3.8,<3.13
 Classifier: Intended Audience :: Developers
```

