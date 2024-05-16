# Comparing `tmp/ssec-3.0.0.tar.gz` & `tmp/ssec-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssec-3.0.0.tar", last modified: Thu May 16 10:04:25 2024, max compression
+gzip compressed data, was "ssec-3.0.1.tar", last modified: Thu May 16 10:43:18 2024, max compression
```

## Comparing `ssec-3.0.0.tar` & `ssec-3.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:04:25.381546 ssec-3.0.0/
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     1063 2024-05-06 10:30:34.000000 ssec-3.0.0/LICENSE
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     7168 2024-05-16 10:04:25.381546 ssec-3.0.0/PKG-INFO
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     5929 2024-05-15 12:02:38.000000 ssec-3.0.0/README.md
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     3651 2024-05-16 09:57:32.000000 ssec-3.0.0/pyproject.toml
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)       38 2024-05-16 10:04:25.381546 ssec-3.0.0/setup.cfg
-drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:04:25.381546 ssec-3.0.0/src/
-drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:04:25.381546 ssec-3.0.0/src/ssec/
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      117 2024-05-15 12:02:38.000000 ssec-3.0.0/src/ssec/__init__.py
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     5292 2024-05-16 09:42:47.000000 ssec-3.0.0/src/ssec/common.py
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     1187 2024-05-16 09:37:29.000000 ssec-3.0.0/src/ssec/constants.py
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      384 2024-05-16 09:40:43.000000 ssec-3.0.0/src/ssec/event.py
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)       57 2024-05-15 12:02:38.000000 ssec-3.0.0/src/ssec/py.typed
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     7115 2024-05-16 09:48:02.000000 ssec-3.0.0/src/ssec/stream.py
-drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:04:25.381546 ssec-3.0.0/src/ssec.egg-info/
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     7168 2024-05-16 10:04:25.000000 ssec-3.0.0/src/ssec.egg-info/PKG-INFO
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      308 2024-05-16 10:04:25.000000 ssec-3.0.0/src/ssec.egg-info/SOURCES.txt
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)        1 2024-05-16 10:04:25.000000 ssec-3.0.0/src/ssec.egg-info/dependency_links.txt
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      112 2024-05-16 10:04:25.000000 ssec-3.0.0/src/ssec.egg-info/requires.txt
--rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)        5 2024-05-16 10:04:25.000000 ssec-3.0.0/src/ssec.egg-info/top_level.txt
+drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:43:18.230273 ssec-3.0.1/
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     1063 2024-05-06 10:30:34.000000 ssec-3.0.1/LICENSE
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     7168 2024-05-16 10:43:18.220273 ssec-3.0.1/PKG-INFO
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     5929 2024-05-15 12:02:38.000000 ssec-3.0.1/README.md
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     3731 2024-05-16 10:42:39.000000 ssec-3.0.1/pyproject.toml
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)       38 2024-05-16 10:43:18.230273 ssec-3.0.1/setup.cfg
+drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:43:18.220273 ssec-3.0.1/src/
+drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:43:18.220273 ssec-3.0.1/src/ssec/
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      117 2024-05-15 12:02:38.000000 ssec-3.0.1/src/ssec/__init__.py
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     5416 2024-05-16 10:39:02.000000 ssec-3.0.1/src/ssec/common.py
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     1187 2024-05-16 09:37:29.000000 ssec-3.0.1/src/ssec/constants.py
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      384 2024-05-16 09:40:43.000000 ssec-3.0.1/src/ssec/event.py
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)       57 2024-05-15 12:02:38.000000 ssec-3.0.1/src/ssec/py.typed
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     7822 2024-05-16 10:41:21.000000 ssec-3.0.1/src/ssec/stream.py
+drwxr-xr-x   0 jbaudisch  (1000) jbaudisch  (1000)        0 2024-05-16 10:43:18.220273 ssec-3.0.1/src/ssec.egg-info/
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)     7168 2024-05-16 10:43:18.000000 ssec-3.0.1/src/ssec.egg-info/PKG-INFO
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      308 2024-05-16 10:43:18.000000 ssec-3.0.1/src/ssec.egg-info/SOURCES.txt
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)        1 2024-05-16 10:43:18.000000 ssec-3.0.1/src/ssec.egg-info/dependency_links.txt
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)      112 2024-05-16 10:43:18.000000 ssec-3.0.1/src/ssec.egg-info/requires.txt
+-rw-r--r--   0 jbaudisch  (1000) jbaudisch  (1000)        5 2024-05-16 10:43:18.000000 ssec-3.0.1/src/ssec.egg-info/top_level.txt
```

### Comparing `ssec-3.0.0/LICENSE` & `ssec-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ssec-3.0.0/PKG-INFO` & `ssec-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssec
-Version: 3.0.0
+Version: 3.0.1
 Summary: Synchronous and asynchronous library for server-sent events.
 Author-email: "J. Baudisch" <justin.baudisch@hsbi.de>
 Maintainer-email: "J. Baudisch" <justin.baudisch@hsbi.de>
 Project-URL: Repository, https://github.com/sharly-project/ssec
 Keywords: Network,Synchronous,Asynchronous,Server-sent events
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `ssec-3.0.0/README.md` & `ssec-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ssec-3.0.0/pyproject.toml` & `ssec-3.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools"]
 
 [project]
 name = "ssec"
-version = "3.0.0"
+version = "3.0.1"
 description = "Synchronous and asynchronous library for server-sent events."
 readme = "README.md"
 requires-python = ">=3.12"
 authors = [
   { name = "J. Baudisch", email = "justin.baudisch@hsbi.de" },
 ]
 maintainers = [{ name = "J. Baudisch", email = "justin.baudisch@hsbi.de" }]
@@ -123,14 +123,16 @@
   "ANN101",   # allow missing type annotation for `self` in method
   "ANN102",   # allow missing type annotation for `cls` in method
   "D105",     # allow missing docstring in magic method
   "TD003",    # allow missing issue link on TODO's
   "RSE102",   # allow unnecessary parentheses on raised exceptions (bug in ruff)
   "PLR1702",  # allow too many nested blocks
   "PLR0913",  # allow too many arguments
+  "PLR0912",  # allow too many branches
+  "C901",     # allow complex structure
 ]
 
 [tool.ruff.lint.extend-per-file-ignores]
 "__init__.py" = ["F401"]  # allow unused imports
 
 [tool.ruff.lint.pydocstyle]
 convention = "numpy"
```

### Comparing `ssec-3.0.0/src/ssec/common.py` & `ssec-3.0.1/src/ssec/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,31 +14,34 @@
 from .constants import DELIMITER, SSE_CONTENT_TYPE
 from .event import Event
 
 
 def create_session[T: (httpx.Client, httpx.AsyncClient)](
     session_class: type[T],
     connect_timeout: float,
+    headers: dict[str, str] | None = None,
 ) -> T:
     """Create an `httpx` session with a custom connect timeout.
 
     Parameters
     ----------
     session_class
         The `httpx` session class to create.
     connect_timeout
         The connect timeout, in seconds.
+    headers
+        Optional headers to include in the session.
     """
     timeout = httpx.Timeout(
         connect=connect_timeout,
         read=None,
         write=None,
         pool=None,
     )
-    return session_class(timeout=timeout)
+    return session_class(timeout=timeout, headers=headers)
 
 
 @dataclasses.dataclass(
     repr=False,
     eq=False,
     kw_only=True,
     slots=True,
```

### Comparing `ssec-3.0.0/src/ssec/constants.py` & `ssec-3.0.1/src/ssec/constants.py`

 * *Files identical despite different names*

### Comparing `ssec-3.0.0/src/ssec/stream.py` & `ssec-3.0.1/src/ssec/stream.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 
 def stream(
     url: str,
     *,
     session: httpx.Client | None = None,
     connect_timeout: float = DEFAULT_CONNECT_TIMEOUT,
+    headers: dict[str, str] | None = None,
     method: Literal["GET", "POST"] = "GET",
     chunk_size: int = DEFAULT_CHUNK_SIZE,
     max_connect_attempts: int = DEFAULT_MAX_CONNECT_ATTEMPTS,
     reconnect_timeout: float = DEFAULT_RECONNECT_TIMEOUT,
     backoff_delay: float = DEFAULT_BACKOFF_DELAY,
 ) -> Iterator[Event]:
     """Stream server-sent events (SSEs), synchronously.
@@ -54,31 +55,40 @@
     url
         The URL to stream server-sent events from.
     session
         An optional HTTP session to use for the request.
     connect_timeout
         The timeout for connecting to the server, in seconds.
         Only used if `session` is `None`.
+    headers
+        Optional headers to include in the session.
+        Only used if `session` is `None`.
     method
         The HTTP method to use for the request.
     chunk_size
         The size of the chunks to read from the response, in bytes.
     max_connect_attempts
         The maximum number of attempts to connect to the server.
     reconnect_timeout
         The time to wait before reconnecting to the server, in seconds.
     backoff_delay
         The additional time to wait to ease a potentially overloaded server, in seconds.
         This time is exponentiated by the number of connectioin attempts.
     """
+    session_must_be_closed = False
     if session is None:
-        session = create_session(httpx.Client, connect_timeout=connect_timeout)
+        session = create_session(
+            httpx.Client,
+            connect_timeout=connect_timeout,
+            headers=headers,
+        )
+        session_must_be_closed = True
 
     config = SSEConfig(reconnect_timeout=reconnect_timeout, last_event_id="")
-    with session:
+    try:
         connect_attempt = 0
         while True:
             headers = SSE_HEADERS.copy()
             if config.last_event_id:
                 headers["Last-Event-ID"] = config.last_event_id
 
             try:
@@ -114,21 +124,25 @@
                     f"Reconnect in {waiting_period} seconds "
                     f"[attempt {connect_attempt + 1}/{max_connect_attempts}]."
                 )
                 _logger.info(message)
 
                 connect_attempt += 1
                 time.sleep(waiting_period)
+    finally:
+        if session_must_be_closed:
+            session.close()
 
 
 async def stream_async(
     url: str,
     *,
     session: httpx.AsyncClient | None = None,
     connect_timeout: float = DEFAULT_CONNECT_TIMEOUT,
+    headers: dict[str, str] | None = None,
     method: Literal["GET", "POST"] = "GET",
     chunk_size: int = DEFAULT_CHUNK_SIZE,
     max_connect_attempts: int = DEFAULT_MAX_CONNECT_ATTEMPTS,
     reconnect_timeout: float = DEFAULT_RECONNECT_TIMEOUT,
     backoff_delay: float = DEFAULT_BACKOFF_DELAY,
 ) -> AsyncIterator[Event]:
     """Stream server-sent events (SSEs), asynchronously.
@@ -138,31 +152,40 @@
     url
         The URL to stream server-sent events from.
     session
         An optional HTTP session to use for the request.
     connect_timeout
         The timeout for connecting to the server, in seconds.
         Only used if `session` is `None`.
+    headers
+        Optional headers to include in the session.
+        Only used if `session` is `None`.
     method
         The HTTP method to use for the request.
     chunk_size
         The size of the chunks to read from the response, in bytes.
     max_connect_attempts
         The maximum number of attempts to connect to the server.
     reconnect_timeout
         The time to wait before reconnecting to the server, in seconds.
     backoff_delay
         The additional time to wait to ease a potentially overloaded server, in seconds.
         This time is exponentiated by the number of connectioin attempts.
     """
+    session_must_be_closed = False
     if session is None:
-        session = create_session(httpx.AsyncClient, connect_timeout=connect_timeout)
+        session = create_session(
+            httpx.AsyncClient,
+            connect_timeout=connect_timeout,
+            headers=headers,
+        )
+        session_must_be_closed = True
 
     config = SSEConfig(reconnect_timeout=reconnect_timeout, last_event_id="")
-    async with session:
+    try:
         connect_attempt = 0
         while True:
             headers = SSE_HEADERS.copy()
             if config.last_event_id:
                 headers["Last-Event-ID"] = config.last_event_id
 
             try:
@@ -199,7 +222,10 @@
                     f"Reconnect in {waiting_period} seconds "
                     f"[attempt {connect_attempt + 1}/{max_connect_attempts}]."
                 )
                 _logger.info(message)
 
                 connect_attempt += 1
                 await asyncio.sleep(waiting_period)
+    finally:
+        if session_must_be_closed:
+            await session.aclose()
```

### Comparing `ssec-3.0.0/src/ssec.egg-info/PKG-INFO` & `ssec-3.0.1/src/ssec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssec
-Version: 3.0.0
+Version: 3.0.1
 Summary: Synchronous and asynchronous library for server-sent events.
 Author-email: "J. Baudisch" <justin.baudisch@hsbi.de>
 Maintainer-email: "J. Baudisch" <justin.baudisch@hsbi.de>
 Project-URL: Repository, https://github.com/sharly-project/ssec
 Keywords: Network,Synchronous,Asynchronous,Server-sent events
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

