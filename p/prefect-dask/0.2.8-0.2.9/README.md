# Comparing `tmp/prefect_dask-0.2.8.tar.gz` & `tmp/prefect_dask-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_dask-0.2.8.tar", last modified: Fri Apr 26 15:04:00 2024, max compression
+gzip compressed data, was "prefect_dask-0.2.9.tar", last modified: Thu May 16 20:58:35 2024, max compression
```

## Comparing `prefect_dask-0.2.8.tar` & `prefect_dask-0.2.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:00.916526 prefect_dask-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-04-26 15:04:00.916526 prefect_dask-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:00.912526 prefect_dask-0.2.8/prefect_dask/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/prefect_dask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:04:00.000000 prefect_dask-0.2.8/prefect_dask/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/prefect_dask/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/prefect_dask/task_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/prefect_dask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:00.912526 prefect_dask-0.2.8/prefect_dask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-04-26 15:04:00.000000 prefect_dask-0.2.8/prefect_dask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-26 15:04:00.000000 prefect_dask-0.2.8/prefect_dask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:04:00.000000 prefect_dask-0.2.8/prefect_dask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-26 15:04:00.000000 prefect_dask-0.2.8/prefect_dask.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-26 15:04:00.000000 prefect_dask-0.2.8/prefect_dask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 15:04:00.000000 prefect_dask-0.2.8/prefect_dask.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:04:00.916526 prefect_dask-0.2.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:00.912526 prefect_dask-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)    11490 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/tests/test_task_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-26 15:03:43.000000 prefect_dask-0.2.8/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.480780 prefect_dask-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11371 2024-05-16 20:58:35.476780 prefect_dask-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9529 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.472780 prefect_dask-0.2.9/prefect_dask/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/prefect_dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:35.000000 prefect_dask-0.2.9/prefect_dask/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/prefect_dask/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13443 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/prefect_dask/task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5756 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/prefect_dask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.476780 prefect_dask-0.2.9/prefect_dask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11371 2024-05-16 20:58:35.000000 prefect_dask-0.2.9/prefect_dask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-16 20:58:35.000000 prefect_dask-0.2.9/prefect_dask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:35.000000 prefect_dask-0.2.9/prefect_dask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 20:58:35.000000 prefect_dask-0.2.9/prefect_dask.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-16 20:58:35.000000 prefect_dask-0.2.9/prefect_dask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 20:58:35.000000 prefect_dask-0.2.9/prefect_dask.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:35.480780 prefect_dask-0.2.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.476780 prefect_dask-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11057 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/tests/test_task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 20:58:19.000000 prefect_dask-0.2.9/tests/test_version.py
```

### Comparing `prefect_dask-0.2.8/LICENSE` & `prefect_dask-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.8/PKG-INFO` & `prefect_dask-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-dask
-Version: 0.2.8
+Version: 0.2.9
 Summary: Prefect integrations with the Dask execution framework.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dask
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: anyio<4.0.0,>=3.7.1
-Requires-Dist: prefect>=2.13.5
+Requires-Dist: prefect<3.0.0,>=2.13.5
 Requires-Dist: distributed==2022.2.0; python_version < "3.8"
 Requires-Dist: distributed!=2023.3.2,!=2023.3.2.1,!=2023.4.*,!=2023.5.*,>=2022.5.0; python_version >= "3.8"
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
```

### Comparing `prefect_dask-0.2.8/README.md` & `prefect_dask-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.8/prefect_dask/task_runners.py` & `prefect_dask-0.2.9/prefect_dask/task_runners.py`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.8/prefect_dask/utils.py` & `prefect_dask-0.2.9/prefect_dask/utils.py`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.8/prefect_dask.egg-info/PKG-INFO` & `prefect_dask-0.2.9/prefect_dask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-dask
-Version: 0.2.8
+Version: 0.2.9
 Summary: Prefect integrations with the Dask execution framework.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dask
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: anyio<4.0.0,>=3.7.1
-Requires-Dist: prefect>=2.13.5
+Requires-Dist: prefect<3.0.0,>=2.13.5
 Requires-Dist: distributed==2022.2.0; python_version < "3.8"
 Requires-Dist: distributed!=2023.3.2,!=2023.3.2.1,!=2023.4.*,!=2023.5.*,>=2022.5.0; python_version >= "3.8"
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
```

### Comparing `prefect_dask-0.2.8/prefect_dask.egg-info/SOURCES.txt` & `prefect_dask-0.2.9/prefect_dask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.8/pyproject.toml` & `prefect_dask-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=45", "wheel", "setuptools_scm>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-dask"
 dependencies = [
   "anyio >= 3.7.1, < 4.0.0",
-  "prefect>=2.13.5",
+  "prefect>=2.13.5, < 3.0.0",
   "distributed==2022.2.0; python_version < '3.8'",
   "distributed>=2022.5.0,!=2023.3.2,!=2023.3.2.1,!=2023.4.*,!=2023.5.*; python_version >= '3.8'", # don't allow versions from 2023.3.2 to 2023.5 (inclusive) due to issue with get_client starting in 2023.3.2 (fixed in 2023.6.0) - https://github.com/dask/distributed/issues/7763
 ]
 dynamic = ["version"]
 description = "Prefect integrations with the Dask execution framework."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `prefect_dask-0.2.8/tests/conftest.py` & `prefect_dask-0.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.8/tests/test_block_standards.py` & `prefect_dask-0.2.9/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_dask-0.2.8/tests/test_task_runners.py` & `prefect_dask-0.2.9/tests/test_task_runners.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,27 +29,19 @@
 @pytest.fixture(scope="session")
 def event_loop(request):
     """
     Redefine the event loop to support session/module-scoped fixtures;
     see https://github.com/pytest-dev/pytest-asyncio/issues/68
     When running on Windows we need to use a non-default loop for subprocess support.
     """
-    if sys.platform == "win32" and sys.version_info >= (3, 8):
+    if sys.platform == "win32":
         asyncio.set_event_loop_policy(asyncio.WindowsProactorEventLoopPolicy())
 
     policy = asyncio.get_event_loop_policy()
 
-    if sys.version_info < (3, 8) and sys.platform != "win32":
-        from prefect.utilities.compat import ThreadedChildWatcher
-
-        # Python < 3.8 does not use a `ThreadedChildWatcher` by default which can
-        # lead to errors in tests as the previous default `SafeChildWatcher`  is not
-        # compatible with threaded event loops.
-        policy.set_child_watcher(ThreadedChildWatcher())
-
     loop = policy.new_event_loop()
 
     # configure asyncio logging to capture long running tasks
     asyncio_logger = logging.getLogger("asyncio")
     asyncio_logger.setLevel("WARNING")
     asyncio_logger.addHandler(logging.StreamHandler())
     loop.set_debug(True)
```

### Comparing `prefect_dask-0.2.8/tests/test_utils.py` & `prefect_dask-0.2.9/tests/test_utils.py`

 * *Files identical despite different names*

