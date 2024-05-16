# Comparing `tmp/simple_threaded_tcp-1.3.tar.gz` & `tmp/simple_threaded_tcp-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_threaded_tcp-1.3.tar", last modified: Tue May 14 23:28:21 2024, max compression
+gzip compressed data, was "simple_threaded_tcp-1.3.1.tar", last modified: Thu May 16 16:35:52 2024, max compression
```

## Comparing `simple_threaded_tcp-1.3.tar` & `simple_threaded_tcp-1.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 23:28:21.841151 simple_threaded_tcp-1.3/
--rw-rw-rw-   0        0        0     6699 2024-05-14 23:28:21.840152 simple_threaded_tcp-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6184 2024-05-14 23:24:21.000000 simple_threaded_tcp-1.3/README.md
--rw-rw-rw-   0        0        0      597 2024-05-14 23:28:10.000000 simple_threaded_tcp-1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-14 23:28:21.842155 simple_threaded_tcp-1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-14 23:28:21.793122 simple_threaded_tcp-1.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-14 23:28:21.837155 simple_threaded_tcp-1.3/src/simple_threaded_tcp.egg-info/
--rw-rw-rw-   0        0        0     6699 2024-05-14 23:28:21.000000 simple_threaded_tcp-1.3/src/simple_threaded_tcp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-14 23:28:21.000000 simple_threaded_tcp-1.3/src/simple_threaded_tcp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 23:28:21.000000 simple_threaded_tcp-1.3/src/simple_threaded_tcp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-14 23:28:21.000000 simple_threaded_tcp-1.3/src/simple_threaded_tcp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-14 23:28:21.835156 simple_threaded_tcp-1.3/src/sttcp/
--rw-rw-rw-   0        0        0       64 2024-05-13 17:37:14.000000 simple_threaded_tcp-1.3/src/sttcp/__init__.py
--rw-rw-rw-   0        0        0     7135 2024-05-14 23:24:21.000000 simple_threaded_tcp-1.3/src/sttcp/client.py
--rw-rw-rw-   0        0        0     8283 2024-05-14 23:24:21.000000 simple_threaded_tcp-1.3/src/sttcp/server.py
+drwxrwxrwx   0        0        0        0 2024-05-16 16:35:52.312515 simple_threaded_tcp-1.3.1/
+-rw-rw-rw-   0        0        0     6788 2024-05-16 16:35:52.309364 simple_threaded_tcp-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6271 2024-05-16 16:32:51.000000 simple_threaded_tcp-1.3.1/README.md
+-rw-rw-rw-   0        0        0      599 2024-05-16 16:35:17.000000 simple_threaded_tcp-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 16:35:52.312515 simple_threaded_tcp-1.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 16:35:52.252871 simple_threaded_tcp-1.3.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 16:35:52.307275 simple_threaded_tcp-1.3.1/src/simple_threaded_tcp.egg-info/
+-rw-rw-rw-   0        0        0     6788 2024-05-16 16:35:52.000000 simple_threaded_tcp-1.3.1/src/simple_threaded_tcp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-16 16:35:52.000000 simple_threaded_tcp-1.3.1/src/simple_threaded_tcp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 16:35:52.000000 simple_threaded_tcp-1.3.1/src/simple_threaded_tcp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-16 16:35:52.000000 simple_threaded_tcp-1.3.1/src/simple_threaded_tcp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 16:35:52.304136 simple_threaded_tcp-1.3.1/src/sttcp/
+-rw-rw-rw-   0        0        0       64 2024-05-13 17:37:14.000000 simple_threaded_tcp-1.3.1/src/sttcp/__init__.py
+-rw-rw-rw-   0        0        0     7219 2024-05-16 16:29:28.000000 simple_threaded_tcp-1.3.1/src/sttcp/client.py
+-rw-rw-rw-   0        0        0     8432 2024-05-16 16:32:51.000000 simple_threaded_tcp-1.3.1/src/sttcp/server.py
```

### Comparing `simple_threaded_tcp-1.3/PKG-INFO` & `simple_threaded_tcp-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_threaded_tcp
-Version: 1.3
+Version: 1.3.1
 Summary: Client-Server threaded TCP connector. This project also uses socket library.
 Author-email: Emil <emilahmaboy@gmail.com>
 Project-URL: Homepage, https://github.com/EmilAhmaBoy/simple-threaded-tcp
 Project-URL: Issues, https://github.com/EmilAhmaBoy/simple-threaded-tcp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8
@@ -112,14 +112,15 @@
 # This is optional in cases of you have something like "while True" statement
 
 """
 Also there are methods like `server.close()` and `client.close()` but they only needed to close a connection.
 
 server.close() awaits for all connections to stop and stops the server
 client.close() disconnects the server with the reason of `sttcp.client.Client.DestructionException`
+server.stop() and client.stop() are alternatives to server.close() and client.close()
 """
 ```
 
 ## What's new?
 ### Version 1.0
 - Nothing :)
 ### Version 1.1
```

### Comparing `simple_threaded_tcp-1.3/README.md` & `simple_threaded_tcp-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
 # This is optional in cases of you have something like "while True" statement
 
 """
 Also there are methods like `server.close()` and `client.close()` but they only needed to close a connection.
 
 server.close() awaits for all connections to stop and stops the server
 client.close() disconnects the server with the reason of `sttcp.client.Client.DestructionException`
+server.stop() and client.stop() are alternatives to server.close() and client.close()
 """
 ```
 
 ## What's new?
 ### Version 1.0
 - Nothing :)
 ### Version 1.1
```

### Comparing `simple_threaded_tcp-1.3/pyproject.toml` & `simple_threaded_tcp-1.3.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "simple_threaded_tcp"
-version = "1.3"
+version = "1.3.1"
 authors = [
     {name = "Emil", email = "emilahmaboy@gmail.com"}
 ]
 description = "Client-Server threaded TCP connector. This project also uses socket library."
 readme = "README.md"
 requires-python = ">3.8"
 classifiers = [
```

### Comparing `simple_threaded_tcp-1.3/src/simple_threaded_tcp.egg-info/PKG-INFO` & `simple_threaded_tcp-1.3.1/src/simple_threaded_tcp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_threaded_tcp
-Version: 1.3
+Version: 1.3.1
 Summary: Client-Server threaded TCP connector. This project also uses socket library.
 Author-email: Emil <emilahmaboy@gmail.com>
 Project-URL: Homepage, https://github.com/EmilAhmaBoy/simple-threaded-tcp
 Project-URL: Issues, https://github.com/EmilAhmaBoy/simple-threaded-tcp/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >3.8
@@ -112,14 +112,15 @@
 # This is optional in cases of you have something like "while True" statement
 
 """
 Also there are methods like `server.close()` and `client.close()` but they only needed to close a connection.
 
 server.close() awaits for all connections to stop and stops the server
 client.close() disconnects the server with the reason of `sttcp.client.Client.DestructionException`
+server.stop() and client.stop() are alternatives to server.close() and client.close()
 """
 ```
 
 ## What's new?
 ### Version 1.0
 - Nothing :)
 ### Version 1.1
```

### Comparing `simple_threaded_tcp-1.3/src/sttcp/client.py` & `simple_threaded_tcp-1.3.1/src/sttcp/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,18 @@
         """Starts TCP client"""
         self._socket_thread.start()
 
     def close(self):
         """Closes TCP client"""
         self._socket_thread.shutdown = True
 
+    def stop(self):
+        """Alternative of .close()"""
+        self.close()
+
     def connection_handler(self, function) -> None:
         """
         Sets a connection handler for TCP client.
         :param function: Function handler parameter with `"address: tuple"`, `"connection: socket.socket"` parameters`
         """
         self._connection_handler = function
```

### Comparing `simple_threaded_tcp-1.3/src/sttcp/server.py` & `simple_threaded_tcp-1.3.1/src/sttcp/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import socket
 import threading
 import traceback
 import warnings
+import time
 from enum import Enum
 from typing import Union
 from . import screen_lock
 
 
 def _default_connection(addr: tuple, connection: socket.socket) -> Union[bool, None]:
     print(f'Connected by {":".join(map(str, addr))}')
@@ -142,14 +143,18 @@
         try:
             closure_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             closure_socket.connect((self.host, self.port))
             self._socket_thread.shutdown_socket = closure_socket.getsockname()
         except (ConnectionResetError, ConnectionRefusedError, ConnectionAbortedError, ConnectionError, OSError) as e:
             raise e
 
+    def stop(self):
+        """Alternative of .close()"""
+        self.close()
+
     def set_handler(self, function):
         """
         Sets a handler for TCP server. Handler format:
 
         def server_handler(addr: tuple, conn: socket.socket, data: bytes): pass
         """
         self.handler = function
@@ -189,21 +194,21 @@
         """Use it to make server stoppable only by KeyboardInterrupt exception."""
         try:
             while not self.is_listening:
                 pass
             screen_lock.acquire()
             print('Press Ctrl + C to stop server!')
             screen_lock.release()
-            while not self.closed:
-                pass
+            while self._socket_thread.is_alive():
+                self._socket_thread.join(0.1)
         except KeyboardInterrupt:
             if hasattr(self, '_socket'):
                 screen_lock.acquire()
                 print('Stopping server...')
                 screen_lock.release()
                 self.close()
                 while not self.closed:
-                    pass
+                    time.sleep(0.1)
 
     def mainloop(self):
-        warnings.warn('This method is renamed to keep_alive', DeprecationWarning)
+        warnings.warn('This method was renamed to keep_alive', DeprecationWarning)
         self.keep_alive()
```

