# Comparing `tmp/socketwrench-1.8.3.tar.gz` & `tmp/socketwrench-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketwrench-1.8.3.tar", last modified: Thu May 16 01:05:42 2024, max compression
+gzip compressed data, was "socketwrench-1.8.4.tar", last modified: Thu May 16 05:53:53 2024, max compression
```

## Comparing `socketwrench-1.8.3.tar` & `socketwrench-1.8.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:42.492178 socketwrench-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-16 01:05:38.000000 socketwrench-1.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 01:05:38.000000 socketwrench-1.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-16 01:05:42.492178 socketwrench-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-05-16 01:05:38.000000 socketwrench-1.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 01:05:38.000000 socketwrench-1.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:05:42.492178 socketwrench-1.8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:42.484178 socketwrench-1.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:42.488178 socketwrench-1.8.3/src/socketwrench/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20976 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:42.488178 socketwrench-1.8.3/src/socketwrench/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:42.488178 socketwrench-1.8.3/src/socketwrench/resources/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/resources/playground/panels.js
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/resources/playground/playground.html
--rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/resources/playground/playground.js
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/resources/swagger.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:42.488178 socketwrench-1.8.3/src/socketwrench/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/samples/file_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    21262 2024-05-16 01:05:38.000000 socketwrench-1.8.3/src/socketwrench/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:05:42.492178 socketwrench-1.8.3/src/socketwrench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-16 01:05:42.000000 socketwrench-1.8.3/src/socketwrench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 01:05:42.000000 socketwrench-1.8.3/src/socketwrench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:05:42.000000 socketwrench-1.8.3/src/socketwrench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 01:05:42.000000 socketwrench-1.8.3/src/socketwrench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:53.859757 socketwrench-1.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-16 05:53:49.000000 socketwrench-1.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 05:53:49.000000 socketwrench-1.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-16 05:53:53.859757 socketwrench-1.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-05-16 05:53:49.000000 socketwrench-1.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 05:53:49.000000 socketwrench-1.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 05:53:53.859757 socketwrench-1.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:53.851757 socketwrench-1.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:53.855757 socketwrench-1.8.4/src/socketwrench/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26631 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:53.855757 socketwrench-1.8.4/src/socketwrench/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:53.855757 socketwrench-1.8.4/src/socketwrench/resources/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/resources/playground/panels.js
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/resources/playground/playground.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/resources/playground/playground.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/resources/swagger.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:53.855757 socketwrench-1.8.4/src/socketwrench/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/samples/file_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25554 2024-05-16 05:53:49.000000 socketwrench-1.8.4/src/socketwrench/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:53:53.859757 socketwrench-1.8.4/src/socketwrench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11855 2024-05-16 05:53:53.000000 socketwrench-1.8.4/src/socketwrench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 05:53:53.000000 socketwrench-1.8.4/src/socketwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:53:53.000000 socketwrench-1.8.4/src/socketwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 05:53:53.000000 socketwrench-1.8.4/src/socketwrench.egg-info/top_level.txt
```

### Comparing `socketwrench-1.8.3/LICENSE` & `socketwrench-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.3/PKG-INFO` & `socketwrench-1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.3
+Version: 1.8.4
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.8.3/README.md` & `socketwrench-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.3/pyproject.toml` & `socketwrench-1.8.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketwrench"
-version = "1.8.3"
+version = "1.8.4"
 description = "A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger."
 readme = "README.md"
 authors = [{ name = "Torin Halsted", email = "modularizer@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `socketwrench-1.8.3/src/socketwrench/__init__.py` & `socketwrench-1.8.4/src/socketwrench/__init__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.3/src/socketwrench/__main__.py` & `socketwrench-1.8.4/src/socketwrench/__main__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.3/src/socketwrench/connection.py` & `socketwrench-1.8.4/src/socketwrench/connection.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.3/src/socketwrench/handlers.py` & `socketwrench-1.8.4/src/socketwrench/handlers.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import traceback
 from contextlib import suppress
 from functools import wraps
 from pathlib import Path
 
 from socketwrench.tags import tag, get, gettag
 from socketwrench.types import Request, Response, Query, Body, Route, FullPath, Method, File, ClientAddr, \
-    HTTPStatusCode, ErrorResponse, Headers, ErrorModes, FileResponse, HTMLResponse
+    HTTPStatusCode, ErrorResponse, Headers, ErrorModes, FileResponse, HTMLResponse, url_decode
 
 logger = logging.getLogger("socketwrench")
 
 
 class Autofill:
     def request(self, request: Request) -> Request:
         return request
@@ -61,73 +61,96 @@
     "route": Route,
     "full_path": FullPath,
     "method": Method,
     "file": File,
     "client_addr": ClientAddr,
 }
 
+def tryissubclass(a, others):
+    try:
+        if isinstance(others, type):
+            return issubclass(a, others)
+    except:
+        pass
+    for o in others:
+        try:
+            if issubclass(a, o):
+                return True
+        except:
+            pass
+    return False
+
+def _typehint_matches(typehint, others):
+    return typehint in others or tryissubclass(typehint, others) or (hasattr(typehint, "__origin__") and typehint.__origin__ in others) or (hasattr(typehint, "__args__") and any(_typehint_matches(t, others) for t in typehint.__args__))
+
 
 def cast_to_typehint(value: str, typehint = inspect._empty):
 
     # unless specifically typed as a string, cast any numeric value to int or float
-    if typehint is not str:
-        # limited we can do here, but in general if a string is numeric it is far more likely it
-        # should be an int or float than a string
-        if value.isdigit() or (value.startswith("-") and value[1:].isdigit()):
-            if typehint is float:
-                return float(value)
+    if _typehint_matches(typehint, [int, inspect._empty]):
+        if value.isdigit() or (value.startswith("-") and value[1:].isdigit())  and not '.' in value:
             return int(value)
-        # if it's a float, it will have a decimal point
-        if "." in value:
-            v = value.replace(".", "")
-            if v.isdigit() or (v.startswith("-") and v[1:].isdigit()):
-                return float(value)
-    if typehint in [str, inspect._empty]:
-        return value
-    if typehint in [int, float]:
-        return typehint(value)
-    if typehint is bool:
-        return value.lower() in ("true", "t", "1")
-    if typehint is list:
-        try:
-            return json.loads(value)
-        except:
-            if value.startswith("[") and value.endswith("]"):
-                value = value[1:-1]
-            elif value.startswith("(") and value.endswith(")"):
-                value = value[1:-1]
-            elif value.startswith("{") and value.endswith("}"):
-                value = value[1:-1]
-            values = value.split(",")
-            values = [v.strip().strip('"') for v in values]
-            return [cast_to_typehint(v) for v in values]
-    if typehint in [tuple, set, frozenset]:
-        return typehint(cast_to_typehint(value, list))
-    if typehint is dict:
-        return json.loads(value)
-    if typehint is bytes:
+    if _typehint_matches(typehint, [float, inspect._empty]):
+        if value.isdigit() or (value.startswith("-") and value[1:].isdigit()):
+            return float(value)
+    if _typehint_matches(typehint, [bool, inspect._empty]):
+        if value.lower() in ["false", "f", "no", "n"]:
+            return False
+        if value.lower() in ["true", "t", "yes", "y"]:
+            return True
+    if _typehint_matches(typehint, [bool]):
+        if value.lower() in ["0"]:
+            return False
+        if value.lower() in ["1", "ok"]:
+            return True
+    if _typehint_matches(typehint, [list, inspect._empty]):
+        if value.startswith("[") and value.endswith("]"):
+            try:
+                return json.loads(value)
+            except:
+                pass
+    if _typehint_matches(typehint, [tuple, inspect._empty]):
+        if value.startswith("(") and value.endswith(")"):
+            try:
+                s = '[' + value[1:-1] + ']'
+                return tuple(json.loads(s))
+            except:
+                pass
+    if _typehint_matches(typehint, [dict, inspect._empty]):
+        if value.startswith("{") and value.endswith("}"):
+            try:
+                return json.loads(value)
+            except:
+                pass
+    if _typehint_matches(typehint, [frozenset]):
+        if value.startswith("{") and value.endswith("}"):
+            try:
+                return frozenset(json.loads('[' + value[1:-1] + ']'))
+            except:
+                pass
+    if _typehint_matches(typehint, [set, inspect._empty]):
+        if value.startswith("{") and value.endswith("}"):
+            try:
+                return set(json.loads('[' + value[1:-1] + ']'))
+            except:
+                pass
+    if typehint is bytes or tryissubclass(typehint, bytes):
         return value.encode()
-    if typehint is bytearray:
+    if typehint is bytearray or tryissubclass(typehint, bytearray):
         return bytearray(value.encode())
-    if typehint is memoryview:
+    if typehint is memoryview or tryissubclass(typehint, memoryview):
         return memoryview(value.encode())
     if typehint is type:
         if hasattr(builtins, value):
             return getattr(builtins, value)
         return globals().get(value, value)
     if hasattr(typehint, "__origin__"):
         if typehint.__origin__ in [list, tuple, set, frozenset]:
             return typehint([cast_to_typehint(v, typehint.__args__[0]) for v in value])
         return cast_to_typehint(value, typehint.__origin__)
-    if hasattr(typehint, "__args__"):
-        for t in typehint.__args__:
-            try:
-                return cast_to_typehint(value, t)
-            except:
-                pass
     return value
 
 
 def cast_to_types(query, signature):
     for param_name, param_value in query.items():
         if param_name in signature:
             typehint = signature[param_name].annotation
@@ -309,15 +332,14 @@
     def __init__(self, path: Path | str, route: str = None):
         self.path = path
         self.route = route or "/" + path.name
         self.allowed_methods = ["GET", "HEAD"]
 
     def match(self, route: str) -> bool:
         if not route.startswith(self.route):
-            print("route doesn't start with", self.route, route)
             return False
         added = route[len(self.route):]
         p = (self.path / added.strip("/")) if added else self.path
         if not p.exists():
             print("path doesn't exist", p, route, added)
             return False
         return True
@@ -337,14 +359,123 @@
             folder_contents = list(p.iterdir())
             contents = "<!DOCTYPE html><html><body><ul>" + "\n".join([f"<li><a href='{route}/{f.name}'>{f.name}</a></li>" for f in folder_contents]) + "</ul></body></html>"
             return Response(contents.encode(), version=request.version)
         r = FileResponse(p, version=request.version)
         print("content type", r.headers.get("Content-Type"))
         return r
 
+
+def matches_variadic_route(route: str, variadic_route: str) -> dict:
+    try:
+        route_parts = route.split("/")
+        variadic_parts = variadic_route.split("/")
+        n = len(route_parts)
+        if n != len(variadic_parts):
+            return False
+
+        found_matches = {}
+        identical_characters = 0
+        for i in range(n):
+            r = route_parts[i]
+            v = variadic_parts[i]
+            if r == v:
+                identical_characters += len(r)
+            else:
+                if not ('{' in v and '}' in v):
+                    return False
+                sections = []
+                current_section = {}
+                for c in v:
+                    if c == "{":
+                        if current_section.get("variadic", False):
+                            return False
+                        sections.append(current_section)
+                        current_section = {"variadic": True, "value": ""}
+                    elif c == "}":
+                        if not current_section.get("variadic", True):
+                            return False
+                        sections.append(current_section)
+                        current_section = {"variadic": False, "value": ""}
+                    else:
+                        if not current_section:
+                            current_section = {"variadic": False, "value": ""}
+                        current_section["value"] += c
+                sections.append(current_section)
+                sections = [s for s in sections if s]
+                sections = [s for s in sections if s["value"]]
+                if len(sections) == 1 and not sections[0]["variadic"]:
+                    found_matches[sections[0]["value"]] = r
+                    continue
+                # make sure they alternate
+                if not all([s["variadic"] != sections[i + 1]["variadic"] for i, s in enumerate(sections[:-1])]):
+                    raise ValueError("Variadic sections must alternate")
+
+                if any(s["value"] in found_matches and s["variadic"] for s in sections):
+                    raise ValueError("Variadic sections must be unique")
+
+                nonvariadic_start = 0
+                nonvariadic_end = 0
+                variadic_name = None
+                variables = {}
+                for section in sections:
+                    if section["variadic"]:
+                        variadic_name = section["value"]
+                        continue
+                    else:
+                        if section["value"] not in r[nonvariadic_end:]:
+                            return False
+                        identical_characters += len(section["value"])
+                        i = r[nonvariadic_end:].index(section["value"])
+                        nonvariadic_start = nonvariadic_end + i
+                        if variadic_name:
+                            variables[variadic_name] = r[nonvariadic_end:nonvariadic_start]
+
+                        nonvariadic_end = nonvariadic_start + len(section["value"])
+
+                        nv = r[nonvariadic_start:nonvariadic_end]
+                        if nv != section["value"]:
+                            raise ValueError(f"Expected {section['value']} but got {nv}")
+                        nonvariadic_start = nonvariadic_end
+                if sections[-1]["variadic"]:
+                    variables[variadic_name] = r[nonvariadic_end:]
+                elif nonvariadic_end < len(r):
+                    return False
+                found_matches.update(variables)
+        return found_matches
+    except Exception as e:
+        print("Error", e)
+        print(str(traceback.format_exc()))
+        return False
+
+def sort_variadic_routes(patterns):
+    q = []
+    for pattern in patterns:
+        parts = pattern.split("/")
+        part_count = len(parts)
+        variadic_part_count = len([p for p in parts if "{" in p and "}" in p])
+        nonvariadic_part_count = part_count - variadic_part_count
+        total_variadic_pattern_count = sum([1 * (c=='{') for c in pattern])
+        total_nonvariadic_chars = 0
+        in_variadic = False
+        for c in pattern:
+            if c == "{":
+                in_variadic = True
+            elif c == "}":
+                in_variadic = False
+            elif not in_variadic:
+                total_nonvariadic_chars += 1
+        q.append((part_count,
+                  nonvariadic_part_count,
+                  total_nonvariadic_chars,
+                  total_variadic_pattern_count,
+                  len(pattern),
+                  pattern))
+    sorted_patterns = [_v[-1] for _v in reversed(sorted(q))]
+    return sorted_patterns
+
 class RouteHandler:
     resources_folder = Path(__file__).parent / "resources"
     playground_folder = resources_folder / "playground"
     default_favicon = resources_folder / "favicon.ico"
 
     def __init__(self,
                  routes: dict | None = None,
@@ -442,30 +573,25 @@
             for k, v in self.matchable_routes.items():
                 if v.match(route):
                     handler = v
                     break
             else:
                 if route in self.default_routes:
                     handler = self.default_routes[route]
+                elif "{" in (x:= url_decode(route)) and x in self.variadic_routes:
+                    raise ValueError(f"Route {route} is variadic , {{}} patterns should be filled in")
                 else:
-                    # check all variadic routes
-                    route_parts = route.split("/")
-                    n = len(route_parts)
-                    for k, v in self.variadic_routes.items():
+                    # check all variadic routes in the correct order, first by number of parts, then number of variadic parts, then length of nonvariadic parts
+                    variadic_patterns = sort_variadic_routes(list(self.variadic_routes.keys()))
+
+                    for k in variadic_patterns:
                         # these are in format /a/{b}/c/{d}/e, convert to regexp groups
-                        parts = k.split("/")
-                        if n != len(parts):
-                            continue
-                        if all((route_parts[i] == parts[i]) or (parts[i].startswith("{") and parts[i].endswith("}")) for i in range(n)):
-                            handler = v
-                            route_params = {
-                                parts[i][1:-1]: route_parts[i]
-                                for i in range(n)
-                                if parts[i].startswith("{") and parts[i].endswith("}")
-                            }
+                        route_params = matches_variadic_route(route, k)
+                        if route_params:
+                            handler = self.variadic_routes[k]
                             break
                     else:
                         handler = self.fallback_handler
 
         if handler is None:
             # send a response with 404
             return Response(b'Not Found',
@@ -541,7 +667,12 @@
         return self.routes[self.base_path + item]
 
     def __setitem__(self, key, value):
         self.route(value, key)
 
     def __getattr__(self, item):
         return self.__class__(self.fallback_handler, self.routes, self.base_path + item + "/")
+
+
+if __name__ == "__main__":
+    items = ["23", "3.14", "True", "False", "1", "0", "[1, 2, 3]", "(1, 2, 3)", "{1, 2, 3}", "{1: 2, 3: 4}", "hello", "world"]
+    d = {v: (cast_to_typehint(v), type(cast_to_typehint(v))) for v in items}
```

### Comparing `socketwrench-1.8.3/src/socketwrench/openapi.py` & `socketwrench-1.8.4/src/socketwrench/openapi.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.3/src/socketwrench/resources/favicon.ico` & `socketwrench-1.8.4/src/socketwrench/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.3/src/socketwrench/resources/playground/panels.js` & `socketwrench-1.8.4/src/socketwrench/resources/playground/panels.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.3/src/socketwrench/resources/playground/playground.html` & `socketwrench-1.8.4/src/socketwrench/resources/playground/playground.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.3/src/socketwrench/resources/playground/playground.js` & `socketwrench-1.8.4/src/socketwrench/resources/playground/playground.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.3/src/socketwrench/resources/swagger.html` & `socketwrench-1.8.4/src/socketwrench/resources/swagger.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.3/src/socketwrench/samples/file_sample.py` & `socketwrench-1.8.4/src/socketwrench/samples/file_sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.3/src/socketwrench/samples/sample.py` & `socketwrench-1.8.4/src/socketwrench/samples/sample.py`

 * *Files 23% similar despite different names*

```diff
@@ -125,14 +125,35 @@
 
     @route("/a/{c}", error_mode="traceback")
     def a(self, b, c=5):
         print(f"calling a with b={b}, c={c}")
         return f"captured b={b}, c={c}"
 
 
+    @route("{misc}")
+    def misc(self, misc):
+        return f"misc={misc}"
+
+    @route("/a/{b}_is1/c/{d}_is1")
+    def a_c1(self, b, d):
+        return f"a_c1: b={b}, d={d}"
+
+    @route("/a/{b}/c/{d}")
+    def a_c(self, b, d):
+        return f"a_c: b={b}, d={d}"
+
+    @route("/a/{b}_is2/c/{d}_is2")
+    def a_c2(self, b, d):
+        return f"a_c2: b={b}, d={d}"
+
+    @route("/a/{b}_is2/c/{d}_is{e}")
+    def a_c3(self, b, d, e):
+        return f"a_c3: b={b}, d={d}, e={e}"
+
+
 if __name__ == '__main__':
     from socketwrench import serve
     s = Sample()
     serve(s)
     # OR
     # serve(Sample)
     # OR
```

### Comparing `socketwrench-1.8.3/src/socketwrench/server.py` & `socketwrench-1.8.4/src/socketwrench/server.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.3/src/socketwrench/tags.py` & `socketwrench-1.8.4/src/socketwrench/tags.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.3/src/socketwrench/types.py` & `socketwrench-1.8.4/src/socketwrench/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
     def query_args(self) -> dict[str, str]:
         """Extracts the query string from the path and parses into a dictionary."""
         q = self.query()
         if not q:
             return {}
         items = [v.split("=", 1) for v in q.split("&")]
-        d = {k: v for k, v in items}
+        d = {url_decode(k): url_decode(v) for k, v in items}
         return d
 
 
 class ClientAddr(str):
     def __new__(cls, host_port: str | tuple[str, int]):
         if isinstance(host_port, tuple):
             host = host_port[0]
@@ -284,43 +284,40 @@
 class ResponseType(type):
     def __getitem__(self, item):
         class TypedResponse(Response):
             default_content_type = item
         return TypedResponse
 
 
-
 class Response(metaclass=ResponseType):
     default_content_type = None
 
     def __new__(cls, body: bytes | ResponseBody = ResponseBody.EMPTY,
                 status_code: int | HTTPStatusCode = HTTPStatusCode.OK,
                 headers: bytes | HeaderBytes | Headers | dict = HeaderBytes.EMPTY,
                 version: str | HTTPVersion = HTTPVersion.HTTP_1_1,
                 **headers_kwargs):
         # If the body is already a Response instance, return it
         if isinstance(body, Response):
             return body
 
         # Create an instance of the appropriate subclass based on the body type
-        if isinstance(body, (bytes, memoryview)):
-            return super(Response, cls).__new__(cls)
-        elif isinstance(body, str) and issubclass(cls, RedirectResponse):
-            return super(Response, RedirectResponse).__new__(RedirectResponse)
-        elif isinstance(body, str) and issubclass(cls, HTMLResponse):
-            return super(Response, HTMLResponse).__new__(HTMLResponse)
-        elif isinstance(body, Path) and not issubclass(cls, FileResponse):
-            return super(Response, FileResponse).__new__(FileResponse)
-        elif isinstance(body, Exception) and not issubclass(cls, ErrorResponse):
-            return super(Response, ErrorResponse).__new__(ErrorResponse)
-        else:
-            if not issubclass(cls, JSONResponse):
-                return super(Response, JSONResponse).__new__(JSONResponse)
-            else:
+        if cls is Response:
+            if isinstance(body, (bytes, memoryview)):
                 return super(Response, cls).__new__(cls)
+            elif isinstance(body, str):
+                return super(Response, HTMLResponse).__new__(HTMLResponse)
+            elif isinstance(body, Path):
+                return super(Response, FileResponse).__new__(FileResponse)
+            elif isinstance(body, Exception):
+                return super(Response, ErrorResponse).__new__(ErrorResponse)
+            else:
+                return super(Response, JSONResponse).__new__(JSONResponse)
+        else:
+            return super(Response, cls).__new__(cls)
 
     def __init__(self,
                  body: bytes | ResponseBody = ResponseBody.EMPTY,
                  status_code: int | HTTPStatusCode = HTTPStatusCode.OK,
                  headers: bytes | HeaderBytes | Headers | dict = HeaderBytes.EMPTY,
                  version: str | HTTPVersion = HTTPVersion.HTTP_1_1,
                  **headers_kwargs
@@ -621,16 +618,257 @@
 
 
 class PermanentRedirect(RedirectResponse):
     def __init__(self, location: str, status_code: int = 308, headers: dict = None, version: str = "HTTP/1.1"):
         super().__init__(location, status_code, headers, version)
 
 
+url_encodings = {
+    " ": "%20",
+    "!": "%21",
+    '"': "%22",
+    "#": "%23",
+    "$": "%24",
+    "%": "%25",
+    "&": "%26",
+    "'": "%27",
+    "(": "%28",
+    ")": "%29",
+    "*": "%2A",
+    "+": "%2B",
+    ",": "%2C",
+    "-": "%2D",
+    ".": "%2E",
+    "/": "%2F",
+    "0": "%30",
+    "1": "%31",
+    "2": "%32",
+    "3": "%33",
+    "4": "%34",
+    "5": "%35",
+    "6": "%36",
+    "7": "%37",
+    "8": "%38",
+    "9": "%39",
+    ":": "%3A",
+    ";": "%3B",
+    "<": "%3C",
+    "=": "%3D",
+    ">": "%3E",
+    "?": "%3F",
+    "@": "%40",
+    "A": "%41",
+    "B": "%42",
+    "C": "%43",
+    "D": "%44",
+    "E": "%45",
+    "F": "%46",
+    "G": "%47",
+    "H": "%48",
+    "I": "%49",
+    "J": "%4A",
+    "K": "%4B",
+    "L": "%4C",
+    "M": "%4D",
+    "N": "%4E",
+    "O": "%4F",
+    "P": "%50",
+    "Q": "%51",
+    "R": "%52",
+    "S": "%53",
+    "T": "%54",
+    "U": "%55",
+    "V": "%56",
+    "W": "%57",
+    "X": "%58",
+    "Y": "%59",
+    "Z": "%5A",
+    "[": "%5B",
+    "\\": "%5C",
+    "]": "%5D",
+    "^": "%5E",
+    "_": "%5F",
+    "`": "%60",
+    "a": "%61",
+    "b": "%62",
+    "c": "%63",
+    "d": "%64",
+    "e": "%65",
+    "f": "%66",
+    "g": "%67",
+    "h": "%68",
+    "i": "%69",
+    "j": "%6A",
+    "k": "%6B",
+    "l": "%6C",
+    "m": "%6D",
+    "n": "%6E",
+    "o": "%6F",
+    "p": "%70",
+    "q": "%71",
+    "r": "%72",
+    "s": "%73",
+    "t": "%74",
+    "u": "%75",
+    "v": "%76",
+    "w": "%77",
+    "x": "%78",
+    "y": "%79",
+    "z": "%7A",
+    "{": "%7B",
+    "|": "%7C",
+    "}": "%7D",
+    "~": "%7E",
+    "\x7F": "%7F",
+    "€": "%E2%82%AC",
+    "\x81": "%81",
+    "‚": "%E2%80%9A",
+    "ƒ": "%C6%92",
+    "„": "%E2%80%9E",
+    "…": "%E2%80%A6",
+    "†": "%E2%80%A0",
+    "‡": "%E2%80%A1",
+    "ˆ": "%CB%86",
+    "‰": "%E2%80%B0",
+    "Š": "%C5%A0",
+    "‹": "%E2%80%B9",
+    "Œ": "%C5%92",
+    "\x8D": "%C5%8D",
+    "Ž": "%C5%BD",
+    "\x8F": "%8F",
+    "\x90": "%C2%90",
+    "‘": "%E2%80%98",
+    "’": "%E2%80%99",
+    "“": "%E2%80%9C",
+    "”": "%E2%80%9D",
+    "•": "%E2%80%A2",
+    "–": "%E2%80%93",
+    "—": "%E2%80%94",
+    "˜": "%CB%9C",
+    "™": "%E2%84%A2",
+    "š": "%C5%A1",
+    "›": "%E2%80%BA",
+    "œ": "%C5%93",
+    "\x9D": "%9D",
+    "ž": "%C5%BE",
+    "Ÿ": "%C5%B8",
+    "\xA0": "%C2%A0",
+    "¡": "%C2%A1",
+    "¢": "%C2%A2",
+    "£": "%C2%A3",
+    "¤": "%C2%A4",
+    "¥": "%C2%A5",
+    "¦": "%C2%A6",
+    "§": "%C2%A7",
+    "¨": "%C2%A8",
+    "©": "%C2%A9",
+    "ª": "%C2%AA",
+    "«": "%C2%AB",
+    "¬": "%C2%AC",
+    "\xAD": "%C2%AD",
+    "®": "%C2%AE",
+    "¯": "%C2%AF",
+    "°": "%C2%B0",
+    "±": "%C2%B1",
+    "²": "%C2%B2",
+    "³": "%C2%B3",
+    "´": "%C2%B4",
+    "µ": "%C2%B5",
+    "¶": "%C2%B6",
+    "·": "%C2%B7",
+    "¸": "%C2%B8",
+    "¹": "%C2%B9",
+    "º": "%C2%BA",
+    "»": "%C2%BB",
+    "¼": "%C2%BC",
+    "½": "%C2%BD",
+    "¾": "%C2%BE",
+    "¿": "%C2%BF",
+    "À": "%C3%80",
+    "Á": "%C3%81",
+    "Â": "%C3%82",
+    "Ã": "%C3%83",
+    "Ä": "%C3%84",
+    "Å": "%C3%85",
+    "Æ": "%C3%86",
+    "Ç": "%C3%87",
+    "È": "%C3%88",
+    "É": "%C3%89",
+    "Ê": "%C3%8A",
+    "Ë": "%C3%8B",
+    "Ì": "%C3%8C",
+    "Í": "%C3%8D",
+    "Î": "%C3%8E",
+    "Ï": "%C3%8F",
+    "Ð": "%C3%90",
+    "Ñ": "%C3%91",
+    "Ò": "%C3%92",
+    "Ó": "%C3%93",
+    "Ô": "%C3%94",
+    "Õ": "%C3%95",
+    "Ö": "%C3%96",
+    "×": "%C3%97",
+    "Ø": "%C3%98",
+    "Ù": "%C3%99",
+    "Ú": "%C3%9A",
+    "Û": "%C3%9B",
+    "Ü": "%C3%9C",
+    "Ý": "%C3%9D",
+    "Þ": "%C3%9E",
+    "ß": "%C3%9F",
+    "à": "%C3%A0",
+    "á": "%C3%A1",
+    "â": "%C3%A2",
+    "ã": "%C3%A3",
+    "ä": "%C3%A4",
+    "å": "%C3%A5",
+    "æ": "%C3%A6",
+    "ç": "%C3%A7",
+    "è": "%C3%A8",
+    "é": "%C3%A9",
+    "ê": "%C3%AA",
+    "ë": "%C3%AB",
+    "ì": "%C3%AC",
+    "í": "%C3%AD",
+    "î": "%C3%AE",
+    "ï": "%C3%AF",
+    "ð": "%C3%B0",
+    "ñ": "%C3%B1",
+    "ò": "%C3%B2",
+    "ó": "%C3%B3",
+    "ô": "%C3%B4",
+    "õ": "%C3%B5",
+    "ö": "%C3%B6",
+    "÷": "%C3%B7",
+    "ø": "%C3%B8",
+    "ù": "%C3%B9",
+    "ú": "%C3%BA",
+    "û": "%C3%BB",
+    "ü": "%C3%BC",
+    "ý": "%C3%BD",
+    "þ": "%C3%BE",
+    "ÿ": "%C3%BF"
+}
+
+
+def url_encode(s: str) -> str:
+    for k, e in url_encodings.items():
+        s = s.replace(k, e)
+    return s
+
+
+def url_decode(s: str) -> str:
+    for e, k in url_encodings.items():
+        s = s.replace(k, e)
+    return s
+
+
 class Query(dict):
-    pass
+    def __str__(self):
+        return "?" + "&".join([f"{url_encode(k)}={url_encode(v)}" for k, v in self.items()])
 
 
 class Route(str):
     pass
 
 
 class FullPath(str):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `socketwrench-1.8.3/src/socketwrench.egg-info/PKG-INFO` & `socketwrench-1.8.4/src/socketwrench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.3
+Version: 1.8.4
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.8.3/src/socketwrench.egg-info/SOURCES.txt` & `socketwrench-1.8.4/src/socketwrench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

