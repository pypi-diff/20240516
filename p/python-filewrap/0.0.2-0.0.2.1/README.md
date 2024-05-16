# Comparing `tmp/python_filewrap-0.0.2.tar.gz` & `tmp/python_filewrap-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_filewrap-0.0.2.tar", max compression
+gzip compressed data, was "python_filewrap-0.0.2.1.tar", max compression
```

## Comparing `python_filewrap-0.0.2.tar` & `python_filewrap-0.0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.2/LICENSE
--rwxr-xr-x   0        0        0     7929 2024-05-16 03:47:27.870753 python_filewrap-0.0.2/filewrap/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.2/filewrap/py.typed
--rw-r--r--   0        0        0     1147 2024-05-16 03:50:40.427087 python_filewrap-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.2/readme.md
--rw-r--r--   0        0        0     1329 1970-01-01 00:00:00.000000 python_filewrap-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.2.1/LICENSE
+-rwxr-xr-x   0        0        0     7948 2024-05-16 12:31:35.118526 python_filewrap-0.0.2.1/filewrap/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.2.1/filewrap/py.typed
+-rw-r--r--   0        0        0     1149 2024-05-16 12:31:49.311113 python_filewrap-0.0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.2.1/readme.md
+-rw-r--r--   0        0        0     1331 1970-01-01 00:00:00.000000 python_filewrap-0.0.2.1/PKG-INFO
```

### Comparing `python_filewrap-0.0.2/LICENSE` & `python_filewrap-0.0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_filewrap-0.0.2/filewrap/__init__.py` & `python_filewrap-0.0.2.1/filewrap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 def ensure_async(func, /):
     if iscoroutinefunction(func):
         return func
     async def wrapper(*args, **kwds):
         ret = to_thread(func, *args, **kwds)
         if isawaitable(ret):
             ret = await ret
+        return ret
     return update_wrapper(wrapper, func)
 
 
 def bio_chunk_iter(
     bio: SupportsRead[bytes] | Callable[[int], bytes], 
     /, 
     size: int = -1,
```

### Comparing `python_filewrap-0.0.2/pyproject.toml` & `python_filewrap-0.0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-filewrap"
-version = "0.0.2"
+version = "0.0.2.1"
 description = "Python file wrappers."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 keywords = ["file", "wrapper"]
```

### Comparing `python_filewrap-0.0.2/PKG-INFO` & `python_filewrap-0.0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-filewrap
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: Python file wrappers.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap
 License: MIT
 Keywords: file,wrapper
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

