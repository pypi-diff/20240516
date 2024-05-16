# Comparing `tmp/socketwrench-1.8.7.tar.gz` & `tmp/socketwrench-1.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketwrench-1.8.7.tar", last modified: Thu May 16 19:48:37 2024, max compression
+gzip compressed data, was "socketwrench-1.8.8.tar", last modified: Thu May 16 19:50:06 2024, max compression
```

## Comparing `socketwrench-1.8.7.tar` & `socketwrench-1.8.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:37.477719 socketwrench-1.8.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-16 19:48:33.000000 socketwrench-1.8.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 19:48:33.000000 socketwrench-1.8.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 19:48:37.477719 socketwrench-1.8.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-16 19:48:33.000000 socketwrench-1.8.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 19:48:33.000000 socketwrench-1.8.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:48:37.477719 socketwrench-1.8.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:37.473719 socketwrench-1.8.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:37.473719 socketwrench-1.8.7/src/socketwrench/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    26833 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:37.477719 socketwrench-1.8.7/src/socketwrench/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:37.477719 socketwrench-1.8.7/src/socketwrench/resources/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/resources/playground/panels.js
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/resources/playground/playground.html
--rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/resources/playground/playground.js
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/resources/swagger.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:37.477719 socketwrench-1.8.7/src/socketwrench/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/samples/file_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    30708 2024-05-16 19:48:33.000000 socketwrench-1.8.7/src/socketwrench/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:48:37.477719 socketwrench-1.8.7/src/socketwrench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 19:48:37.000000 socketwrench-1.8.7/src/socketwrench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 19:48:37.000000 socketwrench-1.8.7/src/socketwrench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:48:37.000000 socketwrench-1.8.7/src/socketwrench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 19:48:37.000000 socketwrench-1.8.7/src/socketwrench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:50:06.106521 socketwrench-1.8.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-16 19:50:01.000000 socketwrench-1.8.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 19:50:01.000000 socketwrench-1.8.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 19:50:06.106521 socketwrench-1.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-16 19:50:01.000000 socketwrench-1.8.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 19:50:01.000000 socketwrench-1.8.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:50:06.106521 socketwrench-1.8.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:50:06.098520 socketwrench-1.8.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:50:06.102521 socketwrench-1.8.8/src/socketwrench/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26774 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:50:06.102521 socketwrench-1.8.8/src/socketwrench/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:50:06.102521 socketwrench-1.8.8/src/socketwrench/resources/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/resources/playground/panels.js
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/resources/playground/playground.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/resources/playground/playground.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/resources/swagger.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:50:06.102521 socketwrench-1.8.8/src/socketwrench/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/samples/file_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30708 2024-05-16 19:50:01.000000 socketwrench-1.8.8/src/socketwrench/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:50:06.102521 socketwrench-1.8.8/src/socketwrench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 19:50:06.000000 socketwrench-1.8.8/src/socketwrench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 19:50:06.000000 socketwrench-1.8.8/src/socketwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:50:06.000000 socketwrench-1.8.8/src/socketwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 19:50:06.000000 socketwrench-1.8.8/src/socketwrench.egg-info/top_level.txt
```

### Comparing `socketwrench-1.8.7/LICENSE` & `socketwrench-1.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/PKG-INFO` & `socketwrench-1.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.7
+Version: 1.8.8
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.8.7/README.md` & `socketwrench-1.8.8/README.md`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/pyproject.toml` & `socketwrench-1.8.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketwrench"
-version = "1.8.7"
+version = "1.8.8"
 description = "A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger."
 readme = "README.md"
 authors = [{ name = "Torin Halsted", email = "modularizer@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `socketwrench-1.8.7/src/socketwrench/__init__.py` & `socketwrench-1.8.8/src/socketwrench/__init__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/src/socketwrench/__main__.py` & `socketwrench-1.8.8/src/socketwrench/__main__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/src/socketwrench/connection.py` & `socketwrench-1.8.8/src/socketwrench/connection.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/src/socketwrench/handlers.py` & `socketwrench-1.8.8/src/socketwrench/handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,14 @@
         else:
             args_before_collector += 1
 
 
     get_autofill_kwargs = autofill.autofill(special_params)
 
     def parser(request: Request, route_params: dict = None) -> tuple[tuple, dict, type]:
-        print("parsing args", sig.parameters, route_params)
         route_params = cast_to_types(route_params, sig.parameters) if route_params else {}
         if not sig.parameters:
             return (), {}, sig.return_annotation
         args = []
         kwargs = get_autofill_kwargs(request)
         q = request.path.query_args()
         if q:
@@ -677,8 +676,8 @@
 
     def __getattr__(self, item):
         return self.__class__(self.fallback_handler, self.routes, self.base_path + item + "/")
 
 
 if __name__ == "__main__":
     items = ["23", "3.14", "True", "False", "1", "0", "[1, 2, 3]", "(1, 2, 3)", "{1, 2, 3}", "{1: 2, 3: 4}", "hello", "world"]
-    d = {v: (cast_to_typehint(v), type(cast_to_typehint(v))) for v in items}
+    d = {v: (cast_to_typehint(v), type(cast_to_typehint(v))) for v in items}
```

### Comparing `socketwrench-1.8.7/src/socketwrench/openapi.py` & `socketwrench-1.8.8/src/socketwrench/openapi.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/src/socketwrench/resources/favicon.ico` & `socketwrench-1.8.8/src/socketwrench/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/src/socketwrench/resources/playground/panels.js` & `socketwrench-1.8.8/src/socketwrench/resources/playground/panels.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/src/socketwrench/resources/playground/playground.html` & `socketwrench-1.8.8/src/socketwrench/resources/playground/playground.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/src/socketwrench/resources/playground/playground.js` & `socketwrench-1.8.8/src/socketwrench/resources/playground/playground.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/src/socketwrench/resources/swagger.html` & `socketwrench-1.8.8/src/socketwrench/resources/swagger.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/src/socketwrench/samples/file_sample.py` & `socketwrench-1.8.8/src/socketwrench/samples/file_sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/src/socketwrench/samples/sample.py` & `socketwrench-1.8.8/src/socketwrench/samples/sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/src/socketwrench/server.py` & `socketwrench-1.8.8/src/socketwrench/server.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/src/socketwrench/tags.py` & `socketwrench-1.8.8/src/socketwrench/tags.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/src/socketwrench/types.py` & `socketwrench-1.8.8/src/socketwrench/types.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.7/src/socketwrench.egg-info/PKG-INFO` & `socketwrench-1.8.8/src/socketwrench.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.7
+Version: 1.8.8
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.8.7/src/socketwrench.egg-info/SOURCES.txt` & `socketwrench-1.8.8/src/socketwrench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

