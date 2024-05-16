# Comparing `tmp/fastapi_namespace_vet1ments-0.1.0.tar.gz` & `tmp/fastapi_namespace_vet1ments-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_namespace_vet1ments-0.1.0.tar", last modified: Thu May 16 15:41:29 2024, max compression
+gzip compressed data, was "fastapi_namespace_vet1ments-0.1.1.tar", last modified: Thu May 16 17:53:38 2024, max compression
```

## Comparing `fastapi_namespace_vet1ments-0.1.0.tar` & `fastapi_namespace_vet1ments-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:29.195336 fastapi_namespace_vet1ments-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 15:41:20.000000 fastapi_namespace_vet1ments-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-16 15:41:29.195336 fastapi_namespace_vet1ments-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-16 15:41:20.000000 fastapi_namespace_vet1ments-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:29.195336 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 15:41:20.000000 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-05-16 15:41:20.000000 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 15:41:20.000000 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:29.195336 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:20.000000 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-16 15:41:20.000000 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:20.000000 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace/tests/test2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-16 15:41:20.000000 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace/types.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-16 15:41:20.000000 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:41:29.195336 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace_vet1ments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-16 15:41:29.000000 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace_vet1ments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-16 15:41:29.000000 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace_vet1ments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:41:29.000000 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace_vet1ments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 15:41:29.000000 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace_vet1ments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 15:41:29.000000 fastapi_namespace_vet1ments-0.1.0/fastapi_namespace_vet1ments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:41:29.195336 fastapi_namespace_vet1ments-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-16 15:41:27.000000 fastapi_namespace_vet1ments-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:53:38.161330 fastapi_namespace_vet1ments-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 17:53:26.000000 fastapi_namespace_vet1ments-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-16 17:53:38.161330 fastapi_namespace_vet1ments-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-16 17:53:26.000000 fastapi_namespace_vet1ments-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:53:38.161330 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 17:53:26.000000 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12545 2024-05-16 17:53:26.000000 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 17:53:26.000000 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:53:38.161330 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:53:26.000000 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-16 17:53:26.000000 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:53:26.000000 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace/tests/test2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-16 17:53:26.000000 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-16 17:53:26.000000 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:53:38.161330 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace_vet1ments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-16 17:53:38.000000 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace_vet1ments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-16 17:53:38.000000 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace_vet1ments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 17:53:38.000000 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace_vet1ments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 17:53:38.000000 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace_vet1ments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 17:53:38.000000 fastapi_namespace_vet1ments-0.1.1/fastapi_namespace_vet1ments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 17:53:38.161330 fastapi_namespace_vet1ments-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-16 17:53:35.000000 fastapi_namespace_vet1ments-0.1.1/setup.py
```

### Comparing `fastapi_namespace_vet1ments-0.1.0/LICENSE` & `fastapi_namespace_vet1ments-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.0/PKG-INFO` & `fastapi_namespace_vet1ments-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_namespace_vet1ments
-Version: 0.1.0
+Version: 0.1.1
 Summary: For FastAPI Routing Class
 Author: no hong seok
 Author-email: vet1ments@naver.com
 Maintainer: no hong seok
 Maintainer-email: vet1ments@naver.com
 License: MIT
 Project-URL: Repository, https://github.com/vet1ments/fastapi_namespace
```

### Comparing `fastapi_namespace_vet1ments-0.1.0/README.md` & `fastapi_namespace_vet1ments-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.0/fastapi_namespace/namespace.py` & `fastapi_namespace_vet1ments-0.1.1/fastapi_namespace/namespace.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     Lifespan
 )
 from starlette.routing import BaseRoute
 from fastapi import APIRouter
 from fastapi.types import (
     IncEx,
 )
-from fastapi.responses import ORJSONResponse
+from fastapi.responses import JSONResponse as ORJSONResponse
 from fastapi.routing import APIRoute
 from fastapi.utils import generate_unique_id
 from fastapi import Depends, Response
 
 from .resource import Resource
 from .types import (
     MethodDocument,
@@ -22,16 +22,16 @@
     Optional,
     Callable,
     Sequence,
     Type,
     Any,
     Literal,
 )
+from utils import delete_none
 from enum import Enum
-
 """
     실행순서
     route out
     doc out
     doc in
     route in 
     resource set doc
@@ -221,15 +221,15 @@
             include_in_schema=include_in_schema,
             response_class=response_class,
             name=name,
             callbacks=callbacks,
             openapi_extra=openapi_extra,
             generate_unique_id_function=generate_unique_id_function
         )
-
+        #
         if hasattr(func.__func__, "__meth_doc__"):
             doc: MethodDocument = func.__func__.__meth_doc__
             if doc.get("dependencies") is not None and dependencies is not None:
                 doc["dependencies"] = [*dependencies, *doc["dependencies"]]
             if doc.get("callbacks") is not None and callbacks is not None:
                 doc["callbacks"] = [*callbacks, *doc["callbacks"]]
             if doc.get("tags") is not None and tags is not None:
@@ -237,21 +237,21 @@
             kwargs.update({
                 **doc,
             })
         default_summary = f"{func.__self__.__class__.__name__}_{func.__name__}"
         kwargs.update({
             "summary": default_summary if (summary := kwargs.get("summary", None)) is None else f"{summary} {default_summary}"
         })
-        func.__func__.__meth_doc__ = kwargs
+        func.__func__.__meth_doc__ = delete_none(kwargs)
 
         self.add_api_route(
-            path,
-            func,
-            methods=[method],
-            **kwargs
+            path=path,
+            endpoint=func,
+            methods=[method.upper()],
+            **func.__func__.__meth_doc__
         )
 
     def doc(
             self,
             summary: str | None = None,
             description: str | None = None,
             name: str | None = None,
```

### Comparing `fastapi_namespace_vet1ments-0.1.0/fastapi_namespace/tests/test.py` & `fastapi_namespace_vet1ments-0.1.1/fastapi_namespace/tests/test.py`

 * *Files 27% similar despite different names*

```diff
@@ -13,40 +13,50 @@
 
 def depends1():
     print("depends1")
 
 def depends2():
     print("depends2")
 
+from fastapi import FastAPI
+from pydantic import BaseModel
+from uvicorn import run
+
+
+class ItemResponse(BaseModel):
+    id: str
+
+
 @namespace.route(
     "/",
-    dependencies=[Depends(depends0)]
 )
 class TestResource(Resource):
-    @namespace.doc(
-        summary="1234",
-        dependencies=[Depends(depends0)]
-    )
+    # @namespace.doc(
+    #     summary="1234",
+    #     dependencies=[Depends(depends0)]
+    # )
     def get(
             self,
-            a: None = Depends(depends2)
-    ):
+            a: str = Depends(depends2)
+    ) -> ItemResponse:
         pass
 
-    @namespace.doc(
-        summary="qor"
-    )
     def post(self):
         ...
 
     async def put(self):
         ...
 
 
 app = FastAPI()
+
+@app.get("/items")
+def test() -> ItemResponse:
+    return ItemResponse()
+
 app.include_router(namespace)
 
 
 if __name__ == "__main__":
     from uvicorn import run
     run(
         app=app,
```

### Comparing `fastapi_namespace_vet1ments-0.1.0/fastapi_namespace/types.py` & `fastapi_namespace_vet1ments-0.1.1/fastapi_namespace/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.0/fastapi_namespace_vet1ments.egg-info/PKG-INFO` & `fastapi_namespace_vet1ments-0.1.1/fastapi_namespace_vet1ments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-namespace-vet1ments
-Version: 0.1.0
+Version: 0.1.1
 Summary: For FastAPI Routing Class
 Author: no hong seok
 Author-email: vet1ments@naver.com
 Maintainer: no hong seok
 Maintainer-email: vet1ments@naver.com
 License: MIT
 Project-URL: Repository, https://github.com/vet1ments/fastapi_namespace
```

### Comparing `fastapi_namespace_vet1ments-0.1.0/fastapi_namespace_vet1ments.egg-info/SOURCES.txt` & `fastapi_namespace_vet1ments-0.1.1/fastapi_namespace_vet1ments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.0/setup.py` & `fastapi_namespace_vet1ments-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from glob import glob
-from os.path import basename, splitext
 from setuptools import find_packages, setup
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='fastapi_namespace_vet1ments',
     description="For FastAPI Routing Class",
-    version='0.1.0',
+    version='0.1.1',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.11.0',
     author="no hong seok",
     author_email="vet1ments@naver.com",
     maintainer="no hong seok",
     maintainer_email="vet1ments@naver.com",
```

