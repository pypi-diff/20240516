# Comparing `tmp/glow-0.13.6.tar.gz` & `tmp/glow-0.13.7.tar.gz`

## Comparing `glow-0.13.6.tar` & `glow-0.13.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/__init__.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_array.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_coro.py
--rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_debug.py
--rw-r--r--   0        0        0    12097 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_ic.py
--rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_import_hook.py
--rw-r--r--   0        0        0     6833 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_more.py
--rw-r--r--   0        0        0    16339 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_parallel.py
--rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_parallel.pyi
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_patch_len.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_patch_print.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_patch_scipy.py
--rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_profile.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_profile.pyi
--rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_reduction.py
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_repr.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_sizeof.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_thread_quota.py
--rw-r--r--   0        0        0     3811 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/_uuid.py
--rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/cli.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/cli.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/py.typed
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/api/__init__.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/api/config.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/api/exporting.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/io/__init__.py
--rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/io/_sound.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/io/_svg.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/wrap/__init__.py
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/wrap/cache.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/wrap/cache.pyi
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/wrap/concurrency.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/wrap/concurrency.pyi
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/wrap/reusable.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 glow-0.13.6/src/glow/wrap/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.13.6/test/__init__.py
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_api.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_batch.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_buffered.py
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_cli.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_iter.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_shm.py
--rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_thread_pool.py
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_timed.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_timer.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 glow-0.13.6/test/test_uuid.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 glow-0.13.6/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 glow-0.13.6/LICENSE
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 glow-0.13.6/README.md
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 glow-0.13.6/pyproject.toml
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 glow-0.13.6/PKG-INFO
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/__init__.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_array.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_coro.py
+-rw-r--r--   0        0        0     3758 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_debug.py
+-rw-r--r--   0        0        0    12097 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_ic.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_import_hook.py
+-rw-r--r--   0        0        0     6833 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_more.py
+-rw-r--r--   0        0        0    16339 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_parallel.py
+-rw-r--r--   0        0        0     3645 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_parallel.pyi
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_patch_len.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_patch_print.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_patch_scipy.py
+-rw-r--r--   0        0        0     6346 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_profile.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_profile.pyi
+-rw-r--r--   0        0        0     4746 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_reduction.py
+-rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_repr.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_sizeof.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_thread_quota.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/_uuid.py
+-rw-r--r--   0        0        0     7930 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/cli.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/cli.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/py.typed
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/api/__init__.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/api/config.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/api/exporting.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/io/__init__.py
+-rw-r--r--   0        0        0     3981 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/io/_sound.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/io/_svg.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/wrap/__init__.py
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/wrap/cache.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/wrap/cache.pyi
+-rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/wrap/concurrency.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/wrap/concurrency.pyi
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/wrap/reusable.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 glow-0.13.7/src/glow/wrap/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 glow-0.13.7/test/__init__.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 glow-0.13.7/test/test_api.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 glow-0.13.7/test/test_batch.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 glow-0.13.7/test/test_buffered.py
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 glow-0.13.7/test/test_cli.py
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 glow-0.13.7/test/test_iter.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 glow-0.13.7/test/test_shm.py
+-rw-r--r--   0        0        0     4387 2020-02-02 00:00:00.000000 glow-0.13.7/test/test_thread_pool.py
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 glow-0.13.7/test/test_timed.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 glow-0.13.7/test/test_timer.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 glow-0.13.7/test/test_uuid.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 glow-0.13.7/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 glow-0.13.7/LICENSE
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 glow-0.13.7/README.md
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 glow-0.13.7/pyproject.toml
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 glow-0.13.7/PKG-INFO
```

### Comparing `glow-0.13.6/src/glow/__init__.py` & `glow-0.13.7/src/glow/__init__.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_coro.py` & `glow-0.13.7/src/glow/_coro.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_debug.py` & `glow-0.13.7/src/glow/_debug.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_ic.py` & `glow-0.13.7/src/glow/_ic.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_import_hook.py` & `glow-0.13.7/src/glow/_import_hook.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_more.py` & `glow-0.13.7/src/glow/_more.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_parallel.py` & `glow-0.13.7/src/glow/_parallel.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_parallel.pyi` & `glow-0.13.7/src/glow/_parallel.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_patch_len.py` & `glow-0.13.7/src/glow/_patch_len.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_patch_print.py` & `glow-0.13.7/src/glow/_patch_print.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_patch_scipy.py` & `glow-0.13.7/src/glow/_patch_scipy.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_profile.py` & `glow-0.13.7/src/glow/_profile.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_profile.pyi` & `glow-0.13.7/src/glow/_profile.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_reduction.py` & `glow-0.13.7/src/glow/_reduction.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_repr.py` & `glow-0.13.7/src/glow/_repr.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_sizeof.py` & `glow-0.13.7/src/glow/_sizeof.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_thread_quota.py` & `glow-0.13.7/src/glow/_thread_quota.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/_uuid.py` & `glow-0.13.7/src/glow/_uuid.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         yield cls
 
     @classmethod  # Pydantic 2.x requirement
     def __get_pydantic_core_schema__(cls, _, handler):
         from pydantic_core import core_schema
         return core_schema.no_info_after_validator_function(
             cls,
-            handler(int | str),
+            handler(SupportsInt | str),
             serialization=core_schema.plain_serializer_function_ser_schema(
                 str,
                 info_arg=False,
                 return_schema=core_schema.str_schema(),
             ),
         )
```

### Comparing `glow-0.13.6/src/glow/cli.py` & `glow-0.13.7/src/glow/cli.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/cli.pyi` & `glow-0.13.7/src/glow/cli.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/api/config.py` & `glow-0.13.7/src/glow/api/config.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/api/exporting.py` & `glow-0.13.7/src/glow/api/exporting.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/io/_sound.py` & `glow-0.13.7/src/glow/io/_sound.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/io/_svg.py` & `glow-0.13.7/src/glow/io/_svg.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/wrap/cache.py` & `glow-0.13.7/src/glow/wrap/cache.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/wrap/cache.pyi` & `glow-0.13.7/src/glow/wrap/cache.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/wrap/concurrency.py` & `glow-0.13.7/src/glow/wrap/concurrency.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/wrap/concurrency.pyi` & `glow-0.13.7/src/glow/wrap/concurrency.pyi`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/wrap/reusable.py` & `glow-0.13.7/src/glow/wrap/reusable.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/src/glow/wrap/util.py` & `glow-0.13.7/src/glow/wrap/util.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/test/test_api.py` & `glow-0.13.7/test/test_api.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/test/test_batch.py` & `glow-0.13.7/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/test/test_buffered.py` & `glow-0.13.7/test/test_buffered.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/test/test_cli.py` & `glow-0.13.7/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/test/test_iter.py` & `glow-0.13.7/test/test_iter.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/test/test_shm.py` & `glow-0.13.7/test/test_shm.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/test/test_thread_pool.py` & `glow-0.13.7/test/test_thread_pool.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/test/test_timed.py` & `glow-0.13.7/test/test_timed.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/test/test_uuid.py` & `glow-0.13.7/test/test_uuid.py`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/LICENSE` & `glow-0.13.7/LICENSE`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/README.md` & `glow-0.13.7/README.md`

 * *Files identical despite different names*

### Comparing `glow-0.13.6/pyproject.toml` & `glow-0.13.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build]
 only-packages = true
 
 [project]
 name = "glow"
-version = "0.13.6"
+version = "0.13.7"
 description = "Functional Python tools"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = []
 authors = [
     {name = "Paul Maevskikh", email = "arquolo@gmail.com"},
```

### Comparing `glow-0.13.6/PKG-INFO` & `glow-0.13.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: glow
-Version: 0.13.6
+Version: 0.13.7
 Summary: Functional Python tools
 Project-URL: homepage, https://github.com/arquolo/glow
 Author-email: Paul Maevskikh <arquolo@gmail.com>
 Maintainer-email: Paul Maevskikh <arquolo@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Paul Maevskikh
```

