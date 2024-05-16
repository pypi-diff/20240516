# Comparing `tmp/socketwrench-1.8.5.tar.gz` & `tmp/socketwrench-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketwrench-1.8.5.tar", last modified: Thu May 16 07:13:17 2024, max compression
+gzip compressed data, was "socketwrench-1.8.6.tar", last modified: Thu May 16 07:39:48 2024, max compression
```

## Comparing `socketwrench-1.8.5.tar` & `socketwrench-1.8.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:17.561384 socketwrench-1.8.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-16 07:13:11.000000 socketwrench-1.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 07:13:11.000000 socketwrench-1.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 07:13:17.561384 socketwrench-1.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-16 07:13:11.000000 socketwrench-1.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 07:13:11.000000 socketwrench-1.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 07:13:17.561384 socketwrench-1.8.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:17.553384 socketwrench-1.8.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:17.557384 socketwrench-1.8.5/src/socketwrench/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    26833 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:17.557384 socketwrench-1.8.5/src/socketwrench/resources/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/resources/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:17.561384 socketwrench-1.8.5/src/socketwrench/resources/playground/
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/resources/playground/panels.js
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/resources/playground/playground.html
--rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/resources/playground/playground.js
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/resources/swagger.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:17.561384 socketwrench-1.8.5/src/socketwrench/samples/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/samples/file_sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/samples/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    28959 2024-05-16 07:13:11.000000 socketwrench-1.8.5/src/socketwrench/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:13:17.561384 socketwrench-1.8.5/src/socketwrench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 07:13:17.000000 socketwrench-1.8.5/src/socketwrench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 07:13:17.000000 socketwrench-1.8.5/src/socketwrench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 07:13:17.000000 socketwrench-1.8.5/src/socketwrench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 07:13:17.000000 socketwrench-1.8.5/src/socketwrench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:48.415002 socketwrench-1.8.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-16 07:39:43.000000 socketwrench-1.8.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 07:39:43.000000 socketwrench-1.8.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 07:39:48.415002 socketwrench-1.8.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-16 07:39:43.000000 socketwrench-1.8.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 07:39:43.000000 socketwrench-1.8.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 07:39:48.415002 socketwrench-1.8.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:48.411002 socketwrench-1.8.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:48.411002 socketwrench-1.8.6/src/socketwrench/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26833 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:48.415002 socketwrench-1.8.6/src/socketwrench/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/resources/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:48.415002 socketwrench-1.8.6/src/socketwrench/resources/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/resources/playground/panels.js
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/resources/playground/playground.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28435 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/resources/playground/playground.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/resources/swagger.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:48.415002 socketwrench-1.8.6/src/socketwrench/samples/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/samples/file_sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4819 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/samples/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30706 2024-05-16 07:39:43.000000 socketwrench-1.8.6/src/socketwrench/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:39:48.415002 socketwrench-1.8.6/src/socketwrench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12244 2024-05-16 07:39:48.000000 socketwrench-1.8.6/src/socketwrench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 07:39:48.000000 socketwrench-1.8.6/src/socketwrench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 07:39:48.000000 socketwrench-1.8.6/src/socketwrench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 07:39:48.000000 socketwrench-1.8.6/src/socketwrench.egg-info/top_level.txt
```

### Comparing `socketwrench-1.8.5/LICENSE` & `socketwrench-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.5/PKG-INFO` & `socketwrench-1.8.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.5
+Version: 1.8.6
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.8.5/README.md` & `socketwrench-1.8.6/README.md`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.5/pyproject.toml` & `socketwrench-1.8.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketwrench"
-version = "1.8.5"
+version = "1.8.6"
 description = "A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger."
 readme = "README.md"
 authors = [{ name = "Torin Halsted", email = "modularizer@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
```

### Comparing `socketwrench-1.8.5/src/socketwrench/__main__.py` & `socketwrench-1.8.6/src/socketwrench/__main__.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.5/src/socketwrench/connection.py` & `socketwrench-1.8.6/src/socketwrench/connection.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.5/src/socketwrench/handlers.py` & `socketwrench-1.8.6/src/socketwrench/handlers.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.5/src/socketwrench/openapi.py` & `socketwrench-1.8.6/src/socketwrench/openapi.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.5/src/socketwrench/resources/favicon.ico` & `socketwrench-1.8.6/src/socketwrench/resources/favicon.ico`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.5/src/socketwrench/resources/playground/panels.js` & `socketwrench-1.8.6/src/socketwrench/resources/playground/panels.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.5/src/socketwrench/resources/playground/playground.html` & `socketwrench-1.8.6/src/socketwrench/resources/playground/playground.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.5/src/socketwrench/resources/playground/playground.js` & `socketwrench-1.8.6/src/socketwrench/resources/playground/playground.js`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.5/src/socketwrench/resources/swagger.html` & `socketwrench-1.8.6/src/socketwrench/resources/swagger.html`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.5/src/socketwrench/samples/file_sample.py` & `socketwrench-1.8.6/src/socketwrench/samples/file_sample.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.5/src/socketwrench/samples/sample.py` & `socketwrench-1.8.6/src/socketwrench/samples/sample.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import logging
 from pathlib import Path
 
+import cv2
+import numpy as np
+
 from socketwrench.handlers import StaticFileHandler
 from socketwrench.tags import private, post, put, patch, delete, route, methods
-from socketwrench.types import TBDBResponse
+from socketwrench.types import TBDBResponse, FileTypeResponse
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 class Sample:
     src = StaticFileHandler(Path(__file__).parent.parent.parent)
 
@@ -154,14 +157,19 @@
     def tbdb_test(self) -> TBDBResponse:
         return [
             {"x": 6, "y": 7, "z": 8},
             {"x": 22, "y": 33, "z": 44},
             {"x": 55, "y": 66, "z": 77},
         ]
 
+    def random_img(self) -> FileTypeResponse("image/png", lambda x: cv2.imencode(".png", x.astype(np.uint8))[1].tobytes()):
+        x = np.random.rand(100, 100, 3) * 255
+        x = x.astype(np.uint8)
+        return x
+
 
 if __name__ == '__main__':
     from socketwrench import serve
     s = Sample()
     serve(s)
     # OR
     # serve(Sample)
```

### Comparing `socketwrench-1.8.5/src/socketwrench/server.py` & `socketwrench-1.8.6/src/socketwrench/server.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.5/src/socketwrench/tags.py` & `socketwrench-1.8.6/src/socketwrench/tags.py`

 * *Files identical despite different names*

### Comparing `socketwrench-1.8.5/src/socketwrench/types.py` & `socketwrench-1.8.6/src/socketwrench/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,55 +451,61 @@
                     else:
                         body = a[0].encode()
                 elif isinstance(a[0], Path):
                     path = a[0]
                 else:
                     body = a[0]
 
-        path = Path(path) if path else Path(".")
+        path = Path(path) if path else Path(".") if not body else None
         if filename is None:
             if path:
                 filename = path.name
             elif extension:
                 filename = "file." + extension.lstrip(".")
             elif content_type:
                 filename = "file" + self.get_extension(content_type)
             else:
                 filename = "file"
         if path and body:
-            raise ValueError("Cannot have both a path and data.")
+            raise ValueError(f"Cannot have both a path and data: {path}, {body}")
         if not path and not body:
             raise ValueError("Must have either a path or data.")
         if body:
             if isinstance(body, str):
                 body = body.encode()
             elif isinstance(body, bytes):
                 pass
             elif isinstance(a[0], (bytearray, memoryview)):
                 body = bytes(a[0])
             elif hasattr(a[0], "read"):
                 body = a[0].read()
+            elif hasattr(a[0], "tobytes"):
+                body = a[0].tobytes()
+            elif hasattr(a[0], "to_bytes"):
+                body = a[0].to_bytes()
+            elif hasattr(a[0], "dumps"):
+                body = (a[0]).dumps().encode()
             elif isinstance(a[0], dict):
                 body = json.dumps(a[0]).encode()
             else:
                 raise ValueError(f"Invalid argument: {a[0]}")
 
         if headers is None:
             headers = {}
 
         if download and "Content-Disposition" not in headers:
             headers["Content-Disposition"] = f'attachment; filename="{filename}"'
 
         # add headers related to file stats
         if "Content-Length" not in headers:
-            headers["Content-Length"] = str(path.stat().st_size)
+            headers["Content-Length"] = str(path.stat().st_size) if path else str(len(body))
         if "Last-Modified" not in headers:
-            headers["Last-Modified"] = datetime.datetime.fromtimestamp(path.stat().st_mtime).isoformat()
+            headers["Last-Modified"] = datetime.datetime.fromtimestamp(path.stat().st_mtime).isoformat() if path else datetime.datetime.now().isoformat()
 
-        if path.is_dir():
+        if path and path.is_dir():
             from tempfile import TemporaryFile
             from zipfile import ZipFile
             # zip the directory to a TemporaryFile
             with TemporaryFile() as f:
                 with ZipFile(f, "w") as z:
                     for p in path.iterdir():
                         z.write(p, p.name)
@@ -542,32 +548,64 @@
 
 
 # define a class such that FileTypeResponse[content_type] is a subclass of FileResponse
 
 
 class FileTypeResponseMeta(type):
     def __getitem__(self, content_type):
+        return self.get_class(content_type)
+
+    @classmethod
+    def get_class(cls, content_type, write_function=None):
         # Create a new subclass of FileResponse with a custom content type
         if content_type[0] == "." and content_type[1:] in FileResponse.content_types:
             content_type = FileResponse.content_types[content_type[1:]]
 
         class TypedFileResponse(FileResponse):
             default_content_type = content_type
 
+            def __init__(self,
+                         *a,
+                         body: bytes = b"",
+                         path: str | Path = None,
+                         filename: str | None = None,
+                         extension: str | None = None,
+                         status_code: int = 200,
+                         headers: dict = None,
+                         content_type: str | None = None,
+                         download: bool = False,
+                         version: str = "HTTP/1.1"):
+                if write_function:
+                    r = write_function(*a)
+                    a = (r,)
+                super().__init__(*a,
+                                    body=body,
+                                    path=path,
+                                    filename=filename,
+                                    extension=extension,
+                                    status_code=status_code,
+                                    headers=headers,
+                                    content_type=content_type,
+                                    download=download,
+                                    version=version)
+
+
         # Generate a class name based on the content type
         ct_name = content_type.split("/")[-1].replace(".", "").replace("-", "").upper()
         TypedFileResponse.__name__ = f"{ct_name}FileResponse"
 
         return TypedFileResponse
 
     def __subclasscheck__(self, subclass):
         return issubclass(subclass, FileResponse)
 
+
 class FileTypeResponse(metaclass=FileTypeResponseMeta):
-    pass
+    def __new__(cls, *args, **kwargs):
+        return FileTypeResponseMeta.get_class(*args, **kwargs)
 
 
 class HTMLResponse(Response):
     def __init__(self, html: str, status_code: int = 200, headers: dict = None, version: str = "HTTP/1.1"):
         if headers is None:
             headers = {}
         if "Content-Type" not in headers:
```

### Comparing `socketwrench-1.8.5/src/socketwrench.egg-info/PKG-INFO` & `socketwrench-1.8.6/src/socketwrench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketwrench
-Version: 1.8.5
+Version: 1.8.6
 Summary: A simple Python library for creating web servers and APIs using sockets, supporting openapi and swagger.
 Author-email: Torin Halsted <modularizer@gmail.com>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
```

### Comparing `socketwrench-1.8.5/src/socketwrench.egg-info/SOURCES.txt` & `socketwrench-1.8.6/src/socketwrench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

