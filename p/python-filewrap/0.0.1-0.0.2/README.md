# Comparing `tmp/python_filewrap-0.0.1.tar.gz` & `tmp/python_filewrap-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_filewrap-0.0.1.tar", max compression
+gzip compressed data, was "python_filewrap-0.0.2.tar", max compression
```

## Comparing `python_filewrap-0.0.1.tar` & `python_filewrap-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.1/LICENSE
--rw-r--r--   0        0        0     7621 2024-05-14 11:40:09.618027 python_filewrap-0.0.1/filewrap/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.1/filewrap/py.typed
--rw-r--r--   0        0        0     1147 2024-05-14 10:48:43.142334 python_filewrap-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.1/readme.md
--rw-r--r--   0        0        0     1329 1970-01-01 00:00:00.000000 python_filewrap-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.2/LICENSE
+-rwxr-xr-x   0        0        0     7929 2024-05-16 03:47:27.870753 python_filewrap-0.0.2/filewrap/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.2/filewrap/py.typed
+-rw-r--r--   0        0        0     1147 2024-05-16 03:50:40.427087 python_filewrap-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.2/readme.md
+-rw-r--r--   0        0        0     1329 1970-01-01 00:00:00.000000 python_filewrap-0.0.2/PKG-INFO
```

### Comparing `python_filewrap-0.0.1/LICENSE` & `python_filewrap-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_filewrap-0.0.1/filewrap/__init__.py` & `python_filewrap-0.0.2/filewrap/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python3
 # encoding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 1)
+__version__ = (0, 0, 2)
 __all__ = [
     "SupportsRead", "SupportsWrite", "bio_chunk_iter", "bio_chunk_async_iter", 
     "bio_skip_iter", "bio_skip_async_iter", "bio_skip_bytes", "bio_skip_bytes_async"
 ]
 
 from asyncio import to_thread
+from collections.abc import Awaitable
 from functools import update_wrapper
 from inspect import isawaitable, iscoroutinefunction
 from collections.abc import AsyncIterator, Callable, Iterator
 from shutil import COPY_BUFSIZE # type: ignore
 from typing import Any, Protocol, TypeVar
 
 
@@ -35,21 +36,24 @@
         ret = to_thread(func, *args, **kwds)
         if isawaitable(ret):
             ret = await ret
     return update_wrapper(wrapper, func)
 
 
 def bio_chunk_iter(
-    bio: SupportsRead[bytes], 
+    bio: SupportsRead[bytes] | Callable[[int], bytes], 
     /, 
     size: int = -1, 
     chunksize: int = COPY_BUFSIZE, 
     callback: None | Callable[[int], Any] = None, 
 ) -> Iterator[bytes]:
-    read = bio.read
+    if callable(bio):
+        read = bio
+    else:
+        read = bio.read
     if not callable(callback):
         callback = None
     if size > 0:
         while size:
             readsize = min(chunksize, size)
             chunk = read(readsize)
             length = len(chunk)
@@ -63,21 +67,24 @@
         while (chunk := read(chunksize)):
             if callback:
                 callback(len(chunk))
             yield chunk
 
 
 async def bio_chunk_async_iter(
-    bio: SupportsRead[bytes], 
+    bio: SupportsRead[bytes] | Callable[[int], bytes | Awaitable[bytes]], 
     /, 
     size: int = -1, 
     chunksize: int = COPY_BUFSIZE, 
     callback: None | Callable[[int], Any] = None, 
 ) -> AsyncIterator[bytes]:
-    read = ensure_async(bio.read)
+    if callable(bio):
+        read = ensure_async(bio)
+    else:
+        read = ensure_async(bio.read)
     callback = ensure_async(callback) if callable(callback) else None
     if size > 0:
         while size:
             readsize = min(chunksize, size)
             chunk = await read(readsize)
             length = len(chunk)
             if callback:
@@ -90,15 +97,15 @@
         while (chunk := (await read(chunksize))):
             if callback:
                 await callback(len(chunk))
             yield chunk
 
 
 def bio_skip_iter(
-    bio: SupportsRead[bytes], 
+    bio: SupportsRead[bytes] | Callable[[int], bytes], 
     /, 
     size: int = -1, 
     chunksize: int = COPY_BUFSIZE, 
     callback: None | Callable[[int], Any] = None, 
 ) -> Iterator[int]:
     if size == 0:
         return
@@ -110,15 +117,17 @@
         if size > 0:
             length = seek(size, 1) - curpos
         else:
             length = seek(0, 2) - curpos
     except Exception:
         if chunksize <= 0:
             chunksize = COPY_BUFSIZE
-        if hasattr(bio, "readinto"):
+        if callable(bio):
+            read = bio
+        elif hasattr(bio, "readinto"):
             readinto = bio.readinto
             buf = bytearray(chunksize)
             if size > 0:
                 while size >= chunksize:
                     length = readinto(buf)
                     if callback:
                         callback(length)
@@ -134,39 +143,40 @@
                             callback(length)
                         yield length
             else:
                 while (length := readinto(buf)):
                     if callback:
                         callback(length)
                     yield length
+            return
         else:
             read = bio.read
-            if size > 0:
-                while size:
-                    readsize = min(chunksize, size)
-                    length = len(read(readsize))
-                    if callback:
-                        callback(length)
-                    yield length
-                    if length < readsize:
-                        break
-                    size -= readsize
-            else:
-                while (length := len(read(chunksize))):
-                    if callback:
-                        callback(length)
-                    yield length
+        if size > 0:
+            while size:
+                readsize = min(chunksize, size)
+                length = len(read(readsize))
+                if callback:
+                    callback(length)
+                yield length
+                if length < readsize:
+                    break
+                size -= readsize
+        else:
+            while (length := len(read(chunksize))):
+                if callback:
+                    callback(length)
+                yield length
     else:
         if callback:
             callback(length)
         yield length
 
 
 async def bio_skip_async_iter(
-    bio: SupportsRead[bytes], 
+    bio: SupportsRead[bytes] | Callable[[int], bytes | Awaitable[bytes]], 
     /, 
     size: int = -1, 
     chunksize: int = COPY_BUFSIZE, 
     callback: None | Callable[[int], Any] = None, 
 ) -> AsyncIterator[int]:
     if size == 0:
         return
@@ -177,15 +187,17 @@
         if size > 0:
             length = (await seek(size, 1)) - curpos
         else:
             length = (await seek(0, 2)) - curpos
     except Exception:
         if chunksize <= 0:
             chunksize = COPY_BUFSIZE
-        if hasattr(bio, "readinto"):
+        if callable(bio):
+            read = ensure_async(bio)
+        elif hasattr(bio, "readinto"):
             readinto = ensure_async(bio.readinto)
             buf = bytearray(chunksize)
             if size > 0:
                 while size >= chunksize:
                     length = await readinto(buf)
                     if callback:
                         await callback(length)
@@ -203,51 +215,49 @@
             else:
                 while (length := (await readinto(buf))):
                     if callback:
                         await callback(length)
                     yield length
         else:
             read = ensure_async(bio.read)
-            if size > 0:
-                while size:
-                    readsize = min(chunksize, size)
-                    length = len(await read(readsize))
-                    if callback:
-                        await callback(length)
-                    yield length
-                    if length < readsize:
-                        break
-                    size -= readsize
-            else:
-                while (length := len(await read(chunksize))):
-                    if callback:
-                        await callback(length)
-                    yield length
+        if size > 0:
+            while size:
+                readsize = min(chunksize, size)
+                length = len(await read(readsize))
+                if callback:
+                    await callback(length)
+                yield length
+                if length < readsize:
+                    break
+                size -= readsize
+        else:
+            while (length := len(await read(chunksize))):
+                if callback:
+                    await callback(length)
+                yield length
     else:
         if callback:
             await callback(length)
         yield length
 
 
 def bio_skip_bytes(
-    bio: SupportsRead[bytes], 
+    bio: SupportsRead[bytes] | Callable[[int], bytes], 
     /, 
     size: int = -1, 
     chunksize: int = COPY_BUFSIZE, 
     callback: None | Callable[[int], Any] = None, 
-) -> SupportsRead[bytes]:
+):
     for _ in bio_skip_iter(bio, size, chunksize, callback=callback):
         pass
-    return bio
 
 
 async def bio_skip_bytes_async(
-    bio: SupportsRead[bytes], 
+    bio: SupportsRead[bytes] | Callable[[int], bytes | Awaitable[bytes]], 
     /, 
     size: int = -1, 
     chunksize: int = COPY_BUFSIZE, 
     callback: None | Callable[[int], Any] = None, 
-) -> SupportsRead[bytes]:
+):
     async for _ in bio_skip_async_iter(bio, size, chunksize, callback=callback):
         pass
-    return bio
```

### Comparing `python_filewrap-0.0.1/pyproject.toml` & `python_filewrap-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-filewrap"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python file wrappers."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 keywords = ["file", "wrapper"]
```

### Comparing `python_filewrap-0.0.1/PKG-INFO` & `python_filewrap-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-filewrap
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python file wrappers.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap
 License: MIT
 Keywords: file,wrapper
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

