# Comparing `tmp/socketwrench-1.8.2.tar.gz` & `tmp/socketwrench-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketwrench-1.8.2.tar", last modified: Wed May  8 16:00:55 2024, max compression
+gzip compressed data, was "socketwrench-1.8.3.tar", last modified: Thu May 16 01:05:42 2024, max compression
```

## Comparing `socketwrench-1.8.2.tar` & `socketwrench-1.8.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:55.440589 socketwrench-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-08 16:00:49.000000 socketwrench-1.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-08 16:00:49.000000 socketwrench-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-08 16:00:55.440589 socketwrench-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-05-08 16:00:49.000000 socketwrench-1.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-08 16:00:49.000000 socketwrench-1.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 16:00:55.440589 socketwrench-1.8.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:55.432589 socketwrench-1.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:55.436589 socketwrench-1.8.2/src/socketwrench/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20975 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:55.436589 socketwrench-1.8.2/src/socketwrench/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:55.436589 socketwrench-1.8.2/src/socketwrench/resources/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/resources/playground/panels.js
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/resources/playground/playground.html
--rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/resources/playground/playground.js
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/resources/swagger.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:55.440589 socketwrench-1.8.2/src/socketwrench/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/samples/file_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    21106 2024-05-08 16:00:49.000000 socketwrench-1.8.2/src/socketwrench/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 16:00:55.440589 socketwrench-1.8.2/src/socketwrench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-08 16:00:55.000000 socketwrench-1.8.2/src/socketwrench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-08 16:00:55.000000 socketwrench-1.8.2/src/socketwrench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 16:00:55.000000 socketwrench-1.8.2/src/socketwrench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-08 16:00:55.000000 socketwrench-1.8.2/src/socketwrench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:42.492178 socketwrench-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-16 01:05:38.000000 socketwrench-1.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 01:05:38.000000 socketwrench-1.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-16 01:05:42.492178 socketwrench-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-05-16 01:05:38.000000 socketwrench-1.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 01:05:38.000000 socketwrench-1.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:05:42.492178 socketwrench-1.8.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:42.484178 socketwrench-1.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:42.488178 socketwrench-1.8.3/src/socketwrench/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20976 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:42.488178 socketwrench-1.8.3/src/socketwrench/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:42.488178 socketwrench-1.8.3/src/socketwrench/resources/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/resources/playground/panels.js
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/resources/playground/playground.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/resources/playground/playground.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/resources/swagger.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:42.488178 socketwrench-1.8.3/src/socketwrench/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/samples/file_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21262 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:42.492178 socketwrench-1.8.3/src/socketwrench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-16 01:05:42.000000 socketwrench-1.8.3/src/socketwrench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 01:05:42.000000 socketwrench-1.8.3/src/socketwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:05:42.000000 socketwrench-1.8.3/src/socketwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 01:05:42.000000 socketwrench-1.8.3/src/socketwrench.egg-info/top_level.txt
```

### Comparing `socketwrench-1.8.2/LICENSE` & `socketwrench-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.2/PKG-INFO` & `socketwrench-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.2
+Version: 1.8.3
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.8.2/README.md` & `socketwrench-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.2/pyproject.toml` & `socketwrench-1.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketwrench"
-version = "1.8.2"
+version = "1.8.3"
 description = "A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger."
 readme = "README.md"
 authors = [{ name = "Torin Halsted", email = "modularizer@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `socketwrench-1.8.2/src/socketwrench/__init__.py` & `socketwrench-1.8.3/src/socketwrench/__init__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.2/src/socketwrench/__main__.py` & `socketwrench-1.8.3/src/socketwrench/__main__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.2/src/socketwrench/connection.py` & `socketwrench-1.8.3/src/socketwrench/connection.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.2/src/socketwrench/handlers.py` & `socketwrench-1.8.3/src/socketwrench/handlers.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -540,8 +540,8 @@
     def __getitem__(self, item):
         return self.routes[self.base_path + item]
 
     def __setitem__(self, key, value):
         self.route(value, key)
 
     def __getattr__(self, item):
-        return self.__class__(self.fallback_handler, self.routes, self.base_path + item + "/")
+        return self.__class__(self.fallback_handler, self.routes, self.base_path + item + "/")
```

### Comparing `socketwrench-1.8.2/src/socketwrench/openapi.py` & `socketwrench-1.8.3/src/socketwrench/openapi.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.2/src/socketwrench/resources/favicon.ico` & `socketwrench-1.8.3/src/socketwrench/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.2/src/socketwrench/resources/playground/panels.js` & `socketwrench-1.8.3/src/socketwrench/resources/playground/panels.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.2/src/socketwrench/resources/playground/playground.html` & `socketwrench-1.8.3/src/socketwrench/resources/playground/playground.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.2/src/socketwrench/resources/playground/playground.js` & `socketwrench-1.8.3/src/socketwrench/resources/playground/playground.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.2/src/socketwrench/resources/swagger.html` & `socketwrench-1.8.3/src/socketwrench/resources/swagger.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.2/src/socketwrench/samples/file_sample.py` & `socketwrench-1.8.3/src/socketwrench/samples/file_sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.2/src/socketwrench/samples/sample.py` & `socketwrench-1.8.3/src/socketwrench/samples/sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.2/src/socketwrench/server.py` & `socketwrench-1.8.3/src/socketwrench/server.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.2/src/socketwrench/tags.py` & `socketwrench-1.8.3/src/socketwrench/tags.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.2/src/socketwrench/types.py` & `socketwrench-1.8.3/src/socketwrench/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,15 +300,17 @@
         # If the body is already a Response instance, return it
         if isinstance(body, Response):
             return body
 
         # Create an instance of the appropriate subclass based on the body type
         if isinstance(body, (bytes, memoryview)):
             return super(Response, cls).__new__(cls)
-        elif isinstance(body, str) and not issubclass(cls, HTMLResponse):
+        elif isinstance(body, str) and issubclass(cls, RedirectResponse):
+            return super(Response, RedirectResponse).__new__(RedirectResponse)
+        elif isinstance(body, str) and issubclass(cls, HTMLResponse):
             return super(Response, HTMLResponse).__new__(HTMLResponse)
         elif isinstance(body, Path) and not issubclass(cls, FileResponse):
             return super(Response, FileResponse).__new__(FileResponse)
         elif isinstance(body, Exception) and not issubclass(cls, ErrorResponse):
             return super(Response, ErrorResponse).__new__(ErrorResponse)
         else:
             if not issubclass(cls, JSONResponse):
@@ -541,15 +543,15 @@
 
 class HTMLResponse(Response):
     def __init__(self, html: str, status_code: int = 200, headers: dict = None, version: str = "HTTP/1.1"):
         if headers is None:
             headers = {}
         if "Content-Type" not in headers:
             headers["Content-Type"] = "text/html"
-        super().__init__(html.encode(), status_code, headers, version)
+        Response.__init__(self, html.encode(), status_code, headers, version)
 
 
 class JSONResponse(Response):
     def __init__(self, data: str | dict | list | tuple | int | float, status_code: int = 200, headers: dict = None,
                  version: str = "HTTP/1.1"):
         if headers is None:
             headers = {}
```

### Comparing `socketwrench-1.8.2/src/socketwrench.egg-info/PKG-INFO` & `socketwrench-1.8.3/src/socketwrench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.2
+Version: 1.8.3
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.8.2/src/socketwrench.egg-info/SOURCES.txt` & `socketwrench-1.8.3/src/socketwrench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

