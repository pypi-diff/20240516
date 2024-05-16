# Comparing `tmp/socketwrench-1.8.4.tar.gz` & `tmp/socketwrench-1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketwrench-1.8.4.tar", last modified: Thu May 16 05:53:53 2024, max compression
+gzip compressed data, was "socketwrench-1.8.5.tar", last modified: Thu May 16 07:13:17 2024, max compression
```

## Comparing `socketwrench-1.8.4.tar` & `socketwrench-1.8.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:53.859757 socketwrench-1.8.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-16 05:53:49.000000 socketwrench-1.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 05:53:49.000000 socketwrench-1.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-16 05:53:53.859757 socketwrench-1.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-05-16 05:53:49.000000 socketwrench-1.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 05:53:49.000000 socketwrench-1.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 05:53:53.859757 socketwrench-1.8.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:53.851757 socketwrench-1.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:53.855757 socketwrench-1.8.4/src/socketwrench/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    26631 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:53.855757 socketwrench-1.8.4/src/socketwrench/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:53.855757 socketwrench-1.8.4/src/socketwrench/resources/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/resources/playground/panels.js
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/resources/playground/playground.html
--rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/resources/playground/playground.js
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/resources/swagger.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:53.855757 socketwrench-1.8.4/src/socketwrench/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/samples/file_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    25554 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:53.859757 socketwrench-1.8.4/src/socketwrench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-16 05:53:53.000000 socketwrench-1.8.4/src/socketwrench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 05:53:53.000000 socketwrench-1.8.4/src/socketwrench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:53:53.000000 socketwrench-1.8.4/src/socketwrench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 05:53:53.000000 socketwrench-1.8.4/src/socketwrench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:17.561384 socketwrench-1.8.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-16 07:13:11.000000 socketwrench-1.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 07:13:11.000000 socketwrench-1.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 07:13:17.561384 socketwrench-1.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-16 07:13:11.000000 socketwrench-1.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 07:13:11.000000 socketwrench-1.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 07:13:17.561384 socketwrench-1.8.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:17.553384 socketwrench-1.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:17.557384 socketwrench-1.8.5/src/socketwrench/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26833 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:17.557384 socketwrench-1.8.5/src/socketwrench/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:17.561384 socketwrench-1.8.5/src/socketwrench/resources/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/resources/playground/panels.js
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/resources/playground/playground.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/resources/playground/playground.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/resources/swagger.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:17.561384 socketwrench-1.8.5/src/socketwrench/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/samples/file_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28959 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:17.561384 socketwrench-1.8.5/src/socketwrench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 07:13:17.000000 socketwrench-1.8.5/src/socketwrench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 07:13:17.000000 socketwrench-1.8.5/src/socketwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 07:13:17.000000 socketwrench-1.8.5/src/socketwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 07:13:17.000000 socketwrench-1.8.5/src/socketwrench.egg-info/top_level.txt
```

### Comparing `socketwrench-1.8.4/LICENSE` & `socketwrench-1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.4/PKG-INFO` & `socketwrench-1.8.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.4
+Version: 1.8.5
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -91,14 +91,15 @@
     "body": Body, # request body bytes
     "headers": Headers, # request headers dict[str, str]
     "route": Route, # route string (without query string)
     "full_path": FullPath, # full path string (with query string)
     "method": Method, # request method str (GET, POST, etc.)
     "file": File, # file bytes (essentially the same as body)
     "client_addr": ClientAddr, # client ip address string (also contains host and port attributes)
+    "socket": socket.socket, # the socket object for the client
 }
 ```
 
 ### Decorators
 ```python
 from socketwrench import route, methods, get, post, put, patch, delete, private
 ```
@@ -147,14 +148,24 @@
 Add a custom function to handle any requests that don't match any other routes.
 
 # Planned Features
 * [ ] Implement nesting / recursion to serve deeper routes and/or multiple classes
 * [ ] Enforce OpenAPI spec with better error responses
 * [x] Serve static folders
 * [x] Make a better playground for testing endpoints
+  * [ ] better preview of variadic routes
+* [ ] improve docs
+  * [ ] document variadic routes
+  * [ ] document autofilled parameters
+  * [ ] document decorators
+  * [ ] document error modes
+  * [ ] document static file serving
+  * [ ] document favicon
+  * [ ] document fallback handler
+  * [ ] document regexp / match routes
 * [ ] Make a client-side python proxy object to make API requests from python
 * [ ] Test on ESP32 and other microcontrollers
 * [ ] Ideas? Let me know!
 
 # Other Usage Modes
 ### Serve a module
 Using commandline, just specify a filepath or file import path to a module.
```

### Comparing `socketwrench-1.8.4/README.md` & `socketwrench-1.8.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     "body": Body, # request body bytes
     "headers": Headers, # request headers dict[str, str]
     "route": Route, # route string (without query string)
     "full_path": FullPath, # full path string (with query string)
     "method": Method, # request method str (GET, POST, etc.)
     "file": File, # file bytes (essentially the same as body)
     "client_addr": ClientAddr, # client ip address string (also contains host and port attributes)
+    "socket": socket.socket, # the socket object for the client
 }
 ```
 
 ### Decorators
 ```python
 from socketwrench import route, methods, get, post, put, patch, delete, private
 ```
@@ -111,14 +112,24 @@
 Add a custom function to handle any requests that don't match any other routes.
 
 # Planned Features
 * [ ] Implement nesting / recursion to serve deeper routes and/or multiple classes
 * [ ] Enforce OpenAPI spec with better error responses
 * [x] Serve static folders
 * [x] Make a better playground for testing endpoints
+  * [ ] better preview of variadic routes
+* [ ] improve docs
+  * [ ] document variadic routes
+  * [ ] document autofilled parameters
+  * [ ] document decorators
+  * [ ] document error modes
+  * [ ] document static file serving
+  * [ ] document favicon
+  * [ ] document fallback handler
+  * [ ] document regexp / match routes
 * [ ] Make a client-side python proxy object to make API requests from python
 * [ ] Test on ESP32 and other microcontrollers
 * [ ] Ideas? Let me know!
 
 # Other Usage Modes
 ### Serve a module
 Using commandline, just specify a filepath or file import path to a module.
```

### Comparing `socketwrench-1.8.4/pyproject.toml` & `socketwrench-1.8.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketwrench"
-version = "1.8.4"
+version = "1.8.5"
 description = "A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger."
 readme = "README.md"
 authors = [{ name = "Torin Halsted", email = "modularizer@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `socketwrench-1.8.4/src/socketwrench/__init__.py` & `socketwrench-1.8.5/src/socketwrench/__init__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.4/src/socketwrench/__main__.py` & `socketwrench-1.8.5/src/socketwrench/__main__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.4/src/socketwrench/connection.py` & `socketwrench-1.8.5/src/socketwrench/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,16 +56,15 @@
         if b'Content-Length:' in pre_body_bytes:
             length = int(pre_body_bytes.split(b'Content-Length: ')[1].split(new_line)[0])
             while len(body) < length and not self.cleanup_event or not self.cleanup_event.is_set():
                 body += connection_socket.recv(chunk_size)
         else:
             body = b''
 
-        r = Request.from_components(pre_body_bytes, body, self.client_addr)
-        logger.info(f"{r}")
+        r = Request.from_components(pre_body_bytes, body, self.client_addr, self.socket)
         return r
 
     def send_response(self, connection_socket: socket.socket, response: Response):
         connection_socket.send(bytes(response))
         connection_socket.close()
 
     def check_cleanup(self):
```

### Comparing `socketwrench-1.8.4/src/socketwrench/handlers.py` & `socketwrench-1.8.5/src/socketwrench/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,30 @@
 import json
 import builtins
 import logging
 import traceback
 from contextlib import suppress
 from functools import wraps
 from pathlib import Path
+import socket
 
 from socketwrench.tags import tag, get, gettag
 from socketwrench.types import Request, Response, Query, Body, Route, FullPath, Method, File, ClientAddr, \
     HTTPStatusCode, ErrorResponse, Headers, ErrorModes, FileResponse, HTMLResponse, url_decode
 
 logger = logging.getLogger("socketwrench")
 
 
 class Autofill:
     def request(self, request: Request) -> Request:
         return request
 
+    def socket(self, request: Request) -> socket.socket:
+        return request.connection_socket
+
     def query(self, request: Request) -> Query:
         return Query(request.path.query_args())
 
     def body(self, request: Request) -> Body:
         return request.body
 
     def headers(self, request: Request) -> Headers:
@@ -59,14 +63,15 @@
     "body": Body,
     "headers": Headers,
     "route": Route,
     "full_path": FullPath,
     "method": Method,
     "file": File,
     "client_addr": ClientAddr,
+    "socket": socket.socket,
 }
 
 def tryissubclass(a, others):
     try:
         if isinstance(others, type):
             return issubclass(a, others)
     except:
@@ -210,14 +215,15 @@
         else:
             args_before_collector += 1
 
 
     get_autofill_kwargs = autofill.autofill(special_params)
 
     def parser(request: Request, route_params: dict = None) -> tuple[tuple, dict, type]:
+        print("parsing args", sig.parameters, route_params)
         route_params = cast_to_types(route_params, sig.parameters) if route_params else {}
         if not sig.parameters:
             return (), {}, sig.return_annotation
         args = []
         kwargs = get_autofill_kwargs(request)
         q = request.path.query_args()
         if q:
```

### Comparing `socketwrench-1.8.4/src/socketwrench/openapi.py` & `socketwrench-1.8.5/src/socketwrench/openapi.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.4/src/socketwrench/resources/favicon.ico` & `socketwrench-1.8.5/src/socketwrench/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.4/src/socketwrench/resources/playground/panels.js` & `socketwrench-1.8.5/src/socketwrench/resources/playground/panels.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.4/src/socketwrench/resources/playground/playground.html` & `socketwrench-1.8.5/src/socketwrench/resources/playground/playground.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.4/src/socketwrench/resources/playground/playground.js` & `socketwrench-1.8.5/src/socketwrench/resources/playground/playground.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.4/src/socketwrench/resources/swagger.html` & `socketwrench-1.8.5/src/socketwrench/resources/swagger.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.4/src/socketwrench/samples/file_sample.py` & `socketwrench-1.8.5/src/socketwrench/samples/file_sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.4/src/socketwrench/samples/sample.py` & `socketwrench-1.8.5/src/socketwrench/samples/sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from pathlib import Path
 
 from socketwrench.handlers import StaticFileHandler
 from socketwrench.tags import private, post, put, patch, delete, route, methods
+from socketwrench.types import TBDBResponse
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 class Sample:
     src = StaticFileHandler(Path(__file__).parent.parent.parent)
 
@@ -134,25 +135,33 @@
         return f"misc={misc}"
 
     @route("/a/{b}_is1/c/{d}_is1")
     def a_c1(self, b, d):
         return f"a_c1: b={b}, d={d}"
 
     @route("/a/{b}/c/{d}")
-    def a_c(self, b, d):
-        return f"a_c: b={b}, d={d}"
+    def a_c(self, b, d, socket=None):
+        s = f"a_c: b={b}, d={d}, socket={str(socket)}".replace("<", "&lt").replace(">", "&gt")
+        return s
 
     @route("/a/{b}_is2/c/{d}_is2")
     def a_c2(self, b, d):
         return f"a_c2: b={b}, d={d}"
 
     @route("/a/{b}_is2/c/{d}_is{e}")
     def a_c3(self, b, d, e):
         return f"a_c3: b={b}, d={d}, e={e}"
 
+    def tbdb_test(self) -> TBDBResponse:
+        return [
+            {"x": 6, "y": 7, "z": 8},
+            {"x": 22, "y": 33, "z": 44},
+            {"x": 55, "y": 66, "z": 77},
+        ]
+
 
 if __name__ == '__main__':
     from socketwrench import serve
     s = Sample()
     serve(s)
     # OR
     # serve(Sample)
```

### Comparing `socketwrench-1.8.4/src/socketwrench/server.py` & `socketwrench-1.8.5/src/socketwrench/server.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.4/src/socketwrench/tags.py` & `socketwrench-1.8.5/src/socketwrench/tags.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.4/src/socketwrench/types.py` & `socketwrench-1.8.5/src/socketwrench/types.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import dataclasses
 import datetime
 import json
+import socket
 from pathlib import Path
 
 
 class HTTPVersion(str):
     """Represents an HTTP version string."""
     HTTP_0_9 = "HTTP/0.9"
     HTTP_1_0 = "HTTP/1.0"
@@ -109,37 +110,39 @@
         self.host = host
         self.port = port
         return self
 
 
 class Request:
     @classmethod
-    def from_components(cls, pre_body_bytes: bytes, body: bytes, client_addr: str | tuple[str, int]) -> "Request":
+    def from_components(cls, pre_body_bytes: bytes, body: bytes, client_addr: str | tuple[str, int], connection_socket: socket.socket = None) -> "Request":
         """Create a Request object from a header string and a body bytes object."""
         i = pre_body_bytes.index(b"\r\n")
         first_line = pre_body_bytes[:i].decode()
         method, path, version = first_line.split(" ")
         header_bytes = pre_body_bytes[i + 2:]
-        return cls(method, path, version, header_bytes, body, client_addr)
+        return cls(method, path, version, header_bytes, body, client_addr, connection_socket)
 
     def __init__(self,
                  method: str | HTTPMethod = HTTPMethod.GET,
                  path: str | RequestPath = RequestPath.BASE,
                  version: str | HTTPVersion = HTTPVersion.HTTP_1_1,
                  header: bytes | HeaderBytes | Headers | dict[str, str] = HeaderBytes.EMPTY,
                  body: bytes | RequestBody = RequestBody.EMPTY,
                  client_addr: str | tuple[str, int] | None = None,
+                 connection_socket: socket.socket | None = None
                  ):
         self.method = HTTPMethod(method)
         self.path = RequestPath(path)
         self.version = HTTPVersion(version)
         self.header_bytes = HeaderBytes(header)
         self._headers = None
         self.body = RequestBody(body)
         self.client_addr = ClientAddr(client_addr) if client_addr else None
+        self.connection_socket = connection_socket
 
     @property
     def headers(self) -> Headers:
         if self._headers is None:
             self._headers = Headers(self.header_bytes.to_dict())
         return self._headers
 
@@ -534,23 +537,96 @@
     def get_extension(self, content_type: str):
         for k, v in self.content_types.items():
             if v == content_type:
                 return "." + k
         return ""
 
 
+# define a class such that FileTypeResponse[content_type] is a subclass of FileResponse
+
+
+class FileTypeResponseMeta(type):
+    def __getitem__(self, content_type):
+        # Create a new subclass of FileResponse with a custom content type
+        if content_type[0] == "." and content_type[1:] in FileResponse.content_types:
+            content_type = FileResponse.content_types[content_type[1:]]
+
+        class TypedFileResponse(FileResponse):
+            default_content_type = content_type
+
+        # Generate a class name based on the content type
+        ct_name = content_type.split("/")[-1].replace(".", "").replace("-", "").upper()
+        TypedFileResponse.__name__ = f"{ct_name}FileResponse"
+
+        return TypedFileResponse
+
+    def __subclasscheck__(self, subclass):
+        return issubclass(subclass, FileResponse)
+
+class FileTypeResponse(metaclass=FileTypeResponseMeta):
+    pass
+
+
 class HTMLResponse(Response):
     def __init__(self, html: str, status_code: int = 200, headers: dict = None, version: str = "HTTP/1.1"):
         if headers is None:
             headers = {}
         if "Content-Type" not in headers:
             headers["Content-Type"] = "text/html"
         Response.__init__(self, html.encode(), status_code, headers, version)
 
 
+class StandardHTMLResponse(HTMLResponse):
+    def __init__(self, body: str, title = "", favicon=None,  scripts: list = None, stylesheets = None, status_code: int = 200, headers: dict = None, version: str = "HTTP/1.1"):
+        favicon = f'<link rel="icon" href="{favicon}">' if favicon else ""
+        scripts = "\n".join([f'<script src="{i}"></script>' for i in scripts]) if scripts else ""
+        stylesheets = "\n".join([f'<link rel="stylesheet" href="{i}">' for i in stylesheets]) if stylesheets else ""
+        html = f"""<!DOCTYPE html>
+<html>
+<head>
+    <title>{title}</title>
+    {favicon}
+    {scripts}
+    {stylesheets}
+</head>
+<body>
+    {body}
+</body>
+</html>"""
+        super().__init__(html, status_code, headers, version)
+
+
+class HTMLTextResponse(StandardHTMLResponse): # this is easier to implement than escaping the text
+    def __init__(self, body: str, title="", favicon=None,  scripts: list = None, stylesheets = None, status_code: int = 200, headers: dict = None, version: str = "HTTP/1.1"):
+        super().__init__(f"<pre>{body}</pre>",
+                            title=title,
+                            favicon=favicon,
+                            scripts=scripts,
+                            stylesheets=stylesheets,
+                            status_code=status_code,
+                            headers=headers,
+                            version=version)
+
+
+class TBDBResponse(StandardHTMLResponse):
+    """Displays tabular json data in a table using https://github.com/modularizer/teebydeeby"""
+    def __init__(self, data, title="", favicon=None,  scripts: list = None, stylesheets = None, status_code: int = 200, headers: dict = None, version: str = "HTTP/1.1"):
+        if not isinstance(data, str):
+            data = json.dumps(data, indent=4)
+        super().__init__(f"<teeby-deeby>{data}</teeby-deeby>",
+                            title=title,
+                            favicon=favicon,
+                            scripts=["https://cdnjs.cloudflare.com/ajax/libs/lz-string/1.4.4/lz-string.min.js", "https://modularizer.github.io/teebydeeby/tbdb.js"] + list(scripts or []),
+                            stylesheets=stylesheets,
+                            status_code=status_code,
+                            headers=headers,
+                            version=version)
+
+
+
 class JSONResponse(Response):
     def __init__(self, data: str | dict | list | tuple | int | float, status_code: int = 200, headers: dict = None,
                  version: str = "HTTP/1.1"):
         if headers is None:
             headers = {}
         if "Content-Type" not in headers:
             headers["Content-Type"] = "application/json"
```

### Comparing `socketwrench-1.8.4/src/socketwrench.egg-info/PKG-INFO` & `socketwrench-1.8.5/src/socketwrench.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.4
+Version: 1.8.5
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -91,14 +91,15 @@
     "body": Body, # request body bytes
     "headers": Headers, # request headers dict[str, str]
     "route": Route, # route string (without query string)
     "full_path": FullPath, # full path string (with query string)
     "method": Method, # request method str (GET, POST, etc.)
     "file": File, # file bytes (essentially the same as body)
     "client_addr": ClientAddr, # client ip address string (also contains host and port attributes)
+    "socket": socket.socket, # the socket object for the client
 }
 ```
 
 ### Decorators
 ```python
 from socketwrench import route, methods, get, post, put, patch, delete, private
 ```
@@ -147,14 +148,24 @@
 Add a custom function to handle any requests that don't match any other routes.
 
 # Planned Features
 * [ ] Implement nesting / recursion to serve deeper routes and/or multiple classes
 * [ ] Enforce OpenAPI spec with better error responses
 * [x] Serve static folders
 * [x] Make a better playground for testing endpoints
+  * [ ] better preview of variadic routes
+* [ ] improve docs
+  * [ ] document variadic routes
+  * [ ] document autofilled parameters
+  * [ ] document decorators
+  * [ ] document error modes
+  * [ ] document static file serving
+  * [ ] document favicon
+  * [ ] document fallback handler
+  * [ ] document regexp / match routes
 * [ ] Make a client-side python proxy object to make API requests from python
 * [ ] Test on ESP32 and other microcontrollers
 * [ ] Ideas? Let me know!
 
 # Other Usage Modes
 ### Serve a module
 Using commandline, just specify a filepath or file import path to a module.
```

### Comparing `socketwrench-1.8.4/src/socketwrench.egg-info/SOURCES.txt` & `socketwrench-1.8.5/src/socketwrench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

