# Comparing `tmp/socketwrench-1.8.6.tar.gz` & `tmp/socketwrench-1.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketwrench-1.8.6.tar", last modified: Thu May 16 07:39:48 2024, max compression
+gzip compressed data, was "socketwrench-1.8.7.tar", last modified: Thu May 16 19:48:37 2024, max compression
```

## Comparing `socketwrench-1.8.6.tar` & `socketwrench-1.8.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:48.415002 socketwrench-1.8.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-16 07:39:43.000000 socketwrench-1.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 07:39:43.000000 socketwrench-1.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 07:39:48.415002 socketwrench-1.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-16 07:39:43.000000 socketwrench-1.8.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 07:39:43.000000 socketwrench-1.8.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 07:39:48.415002 socketwrench-1.8.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:48.411002 socketwrench-1.8.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:48.411002 socketwrench-1.8.6/src/socketwrench/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    26833 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:48.415002 socketwrench-1.8.6/src/socketwrench/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:48.415002 socketwrench-1.8.6/src/socketwrench/resources/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/resources/playground/panels.js
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/resources/playground/playground.html
--rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/resources/playground/playground.js
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/resources/swagger.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:48.415002 socketwrench-1.8.6/src/socketwrench/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/samples/file_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    30706 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:48.415002 socketwrench-1.8.6/src/socketwrench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 07:39:48.000000 socketwrench-1.8.6/src/socketwrench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 07:39:48.000000 socketwrench-1.8.6/src/socketwrench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 07:39:48.000000 socketwrench-1.8.6/src/socketwrench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 07:39:48.000000 socketwrench-1.8.6/src/socketwrench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:37.477719 socketwrench-1.8.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-16 19:48:33.000000 socketwrench-1.8.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 19:48:33.000000 socketwrench-1.8.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 19:48:37.477719 socketwrench-1.8.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-16 19:48:33.000000 socketwrench-1.8.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 19:48:33.000000 socketwrench-1.8.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:48:37.477719 socketwrench-1.8.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:37.473719 socketwrench-1.8.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:37.473719 socketwrench-1.8.7/src/socketwrench/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26833 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:37.477719 socketwrench-1.8.7/src/socketwrench/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:37.477719 socketwrench-1.8.7/src/socketwrench/resources/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/resources/playground/panels.js
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/resources/playground/playground.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/resources/playground/playground.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/resources/swagger.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:37.477719 socketwrench-1.8.7/src/socketwrench/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/samples/file_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30708 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:37.477719 socketwrench-1.8.7/src/socketwrench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 19:48:37.000000 socketwrench-1.8.7/src/socketwrench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 19:48:37.000000 socketwrench-1.8.7/src/socketwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:48:37.000000 socketwrench-1.8.7/src/socketwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 19:48:37.000000 socketwrench-1.8.7/src/socketwrench.egg-info/top_level.txt
```

### Comparing `socketwrench-1.8.6/LICENSE` & `socketwrench-1.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.6/PKG-INFO` & `socketwrench-1.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.6
+Version: 1.8.7
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.8.6/README.md` & `socketwrench-1.8.7/README.md`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.6/pyproject.toml` & `socketwrench-1.8.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketwrench"
-version = "1.8.6"
+version = "1.8.7"
 description = "A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger."
 readme = "README.md"
 authors = [{ name = "Torin Halsted", email = "modularizer@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `socketwrench-1.8.6/src/socketwrench/__init__.py` & `socketwrench-1.8.7/src/socketwrench/__init__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.6/src/socketwrench/__main__.py` & `socketwrench-1.8.7/src/socketwrench/__main__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.6/src/socketwrench/connection.py` & `socketwrench-1.8.7/src/socketwrench/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from socketwrench.types import Request, Response
 
 logger = logging.getLogger("socketwrench")
 
 
 class Connection:
     default_chunk_size: int = 1024
+    timeout = 5
 
     def __init__(self,
                  handler,
                  connection_socket: socket.socket,
                  client_address: tuple,
                  cleanup_event,
                  chunk_size: int = default_chunk_size):
@@ -20,24 +21,29 @@
         self.chunk_size = chunk_size
         self.cleanup_event = cleanup_event
         self.handler = handler
 
         self._rep = None
 
     def handle(self):
-        request = self.receive_request(self.socket)
-        if self.check_cleanup():
-            return request, None, False
-        response = self.handler(request)
-        if self.check_cleanup():
-            return request, response, False
-        self.send_response(self.socket, response)
-        return request, response, True
+                try:
+            request = self.receive_request(self.socket)
+            if self.check_cleanup():
+                return request, None, False
+            response = self.handler(request)
+            if self.check_cleanup():
+                return request, response, False
+            self.send_response(self.socket, response)
+            return request, response, True
+        except Exception as e
+            self.close()
+            raise e
 
     def receive_request(self, connection_socket: socket.socket, chunk_size: int = None) -> Request:
+        connection_socket.settimeout(self.timeout)
         if chunk_size is None:
             chunk_size = self.chunk_size
 
         new_line = b'\r\n'
         end_of_header = 2 * new_line
 
         request_data = b''
@@ -60,24 +66,26 @@
         else:
             body = b''
 
         r = Request.from_components(pre_body_bytes, body, self.client_addr, self.socket)
         return r
 
     def send_response(self, connection_socket: socket.socket, response: Response):
-        connection_socket.send(bytes(response))
+        connection_socket.sendall(bytes(response))
+        connection_socket.shutdown(socket.SHUT_WR) # seems to be needed for linux?
         connection_socket.close()
 
     def check_cleanup(self):
         if self.cleanup_event and self.cleanup_event.is_set():
             self.close()
             return True
         return False
 
     def close(self):
+        self.socket.shutdown(socket.SHUT_WR) # seems to be needed for linux?
         self.socket.close()
 
     def __repr__(self):
         if self._rep is None:
             r = ""
             if self.chunk_size != self.default_chunk_size:
                 r += f", chunk_size={self.chunk_size}"
```

### Comparing `socketwrench-1.8.6/src/socketwrench/handlers.py` & `socketwrench-1.8.7/src/socketwrench/handlers.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.6/src/socketwrench/openapi.py` & `socketwrench-1.8.7/src/socketwrench/openapi.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.6/src/socketwrench/resources/favicon.ico` & `socketwrench-1.8.7/src/socketwrench/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.6/src/socketwrench/resources/playground/panels.js` & `socketwrench-1.8.7/src/socketwrench/resources/playground/panels.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.6/src/socketwrench/resources/playground/playground.html` & `socketwrench-1.8.7/src/socketwrench/resources/playground/playground.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.6/src/socketwrench/resources/playground/playground.js` & `socketwrench-1.8.7/src/socketwrench/resources/playground/playground.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.6/src/socketwrench/resources/swagger.html` & `socketwrench-1.8.7/src/socketwrench/resources/swagger.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.6/src/socketwrench/samples/file_sample.py` & `socketwrench-1.8.7/src/socketwrench/samples/file_sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.6/src/socketwrench/samples/sample.py` & `socketwrench-1.8.7/src/socketwrench/samples/sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.6/src/socketwrench/server.py` & `socketwrench-1.8.7/src/socketwrench/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,20 @@
 class Server(socket.socket):
     """A simple HTTP server built directly on top of socket.socket."""
     default_port = 8080
     default_host = ''
     default_backlog = 1
     default_chunk_size = Connection.default_chunk_size
     default_num_connection_threads = 1
-    default_socket_options = None
+    default_socket_options = {
+        socket.SOL_SOCKET: {
+            socket.SO_REUSEADDR: 1,
+            socket.SO_REUSEPORT: 1
+        }
+    }
     default_pause_sleep = 0.1
     default_accept_sleep = 0
     default_favicon = RouteHandler.default_favicon
 
     def __init__(self,
                  routes: dict | None = None,
                  port: int = default_port,
```

### Comparing `socketwrench-1.8.6/src/socketwrench/tags.py` & `socketwrench-1.8.7/src/socketwrench/tags.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.6/src/socketwrench/types.py` & `socketwrench-1.8.7/src/socketwrench/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 class Headers(dict):
     EMPTY = {}
 
     def to_string(self) -> str:
         s = ""
         for k, v in self.items():
-            s += f"{k}: {v}\n"
+            s += f"{k}: {v}\r\n"
         return s
 
     def __str__(self):
         return self.to_string()
 
     def to_bytes(self) -> bytes:
         return self.to_string().encode()
```

### Comparing `socketwrench-1.8.6/src/socketwrench.egg-info/PKG-INFO` & `socketwrench-1.8.7/src/socketwrench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.6
+Version: 1.8.7
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.8.6/src/socketwrench.egg-info/SOURCES.txt` & `socketwrench-1.8.7/src/socketwrench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

