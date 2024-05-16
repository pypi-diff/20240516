# Comparing `tmp/prefect_ray-0.3.5.tar.gz` & `tmp/prefect_ray-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_ray-0.3.5.tar", last modified: Fri Apr 26 15:04:03 2024, max compression
+gzip compressed data, was "prefect_ray-0.3.6.tar", last modified: Thu May 16 20:58:40 2024, max compression
```

## Comparing `prefect_ray-0.3.5.tar` & `prefect_ray-0.3.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:03.126844 prefect_ray-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:49.000000 prefect_ray-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:49.000000 prefect_ray-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9179 2024-04-26 15:04:03.122843 prefect_ray-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-04-26 15:03:49.000000 prefect_ray-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:03.118843 prefect_ray-0.3.5/prefect_ray/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-26 15:03:49.000000 prefect_ray-0.3.5/prefect_ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:04:02.000000 prefect_ray-0.3.5/prefect_ray/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-26 15:03:49.000000 prefect_ray-0.3.5/prefect_ray/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-04-26 15:03:49.000000 prefect_ray-0.3.5/prefect_ray/task_runners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:03.122843 prefect_ray-0.3.5/prefect_ray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9179 2024-04-26 15:04:02.000000 prefect_ray-0.3.5/prefect_ray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-26 15:04:03.000000 prefect_ray-0.3.5/prefect_ray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:04:02.000000 prefect_ray-0.3.5/prefect_ray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-26 15:04:02.000000 prefect_ray-0.3.5/prefect_ray.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-26 15:04:02.000000 prefect_ray-0.3.5/prefect_ray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 15:04:02.000000 prefect_ray-0.3.5/prefect_ray.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-26 15:03:49.000000 prefect_ray-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:04:03.126844 prefect_ray-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:04:03.122843 prefect_ray-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:49.000000 prefect_ray-0.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-26 15:03:49.000000 prefect_ray-0.3.5/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-26 15:03:49.000000 prefect_ray-0.3.5/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-26 15:03:49.000000 prefect_ray-0.3.5/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-04-26 15:03:49.000000 prefect_ray-0.3.5/tests/test_task_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-26 15:03:49.000000 prefect_ray-0.3.5/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:40.762359 prefect_ray-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-05-16 20:58:40.758359 prefect_ray-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7429 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:40.754359 prefect_ray-0.3.6/prefect_ray/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/prefect_ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:40.000000 prefect_ray-0.3.6/prefect_ray/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/prefect_ray/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/prefect_ray/task_runners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:40.758359 prefect_ray-0.3.6/prefect_ray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9186 2024-05-16 20:58:40.000000 prefect_ray-0.3.6/prefect_ray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-16 20:58:40.000000 prefect_ray-0.3.6/prefect_ray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:40.000000 prefect_ray-0.3.6/prefect_ray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 20:58:40.000000 prefect_ray-0.3.6/prefect_ray.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-16 20:58:40.000000 prefect_ray-0.3.6/prefect_ray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 20:58:40.000000 prefect_ray-0.3.6/prefect_ray.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:40.762359 prefect_ray-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:40.758359 prefect_ray-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/tests/test_task_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-16 20:58:29.000000 prefect_ray-0.3.6/tests/test_version.py
```

### Comparing `prefect_ray-0.3.5/LICENSE` & `prefect_ray-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_ray-0.3.5/PKG-INFO` & `prefect_ray-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-ray
-Version: 0.3.5
+Version: 0.3.6
 Summary: Prefect integrations with the Ray execution framework.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-ray
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prefect>=2.14.10
+Requires-Dist: prefect<3.0.0,>=2.14.10
 Requires-Dist: ray[default]>=2.0.0
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
```

### Comparing `prefect_ray-0.3.5/README.md` & `prefect_ray-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `prefect_ray-0.3.5/prefect_ray/context.py` & `prefect_ray-0.3.6/prefect_ray/context.py`

 * *Files identical despite different names*

### Comparing `prefect_ray-0.3.5/prefect_ray/task_runners.py` & `prefect_ray-0.3.6/prefect_ray/task_runners.py`

 * *Files identical despite different names*

### Comparing `prefect_ray-0.3.5/prefect_ray.egg-info/PKG-INFO` & `prefect_ray-0.3.6/prefect_ray.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-ray
-Version: 0.3.5
+Version: 0.3.6
 Summary: Prefect integrations with the Ray execution framework.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-ray
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prefect>=2.14.10
+Requires-Dist: prefect<3.0.0,>=2.14.10
 Requires-Dist: ray[default]>=2.0.0
 Provides-Extra: dev
 Requires-Dist: aiohttp; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
```

### Comparing `prefect_ray-0.3.5/pyproject.toml` & `prefect_ray-0.3.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -3,36 +3,31 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prefect-ray"
 description = "Prefect integrations with the Ray execution framework."
 readme = "README.md"
 requires-python = ">=3.8"
-license = {text = "Apache License 2.0"}
+license = { text = "Apache License 2.0" }
 keywords = ["prefect"]
-authors = [
-  {name = "Prefect Technologies, Inc.", email = "help@prefect.io"}
-]
+authors = [{ name = "Prefect Technologies, Inc.", email = "help@prefect.io" }]
 classifiers = [
   "Natural Language :: English",
   "Intended Audience :: Developers",
   "Intended Audience :: System Administrators",
   "License :: OSI Approved :: Apache Software License",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
 ]
-dependencies = [
-  "prefect>=2.14.10",
-  "ray[default]>=2.0.0"
-]
+dependencies = ["prefect>=2.14.10, < 3.0.0", "ray[default]>=2.0.0"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
   "aiohttp",
   "coverage",
   "interrogate",
@@ -74,8 +69,8 @@
 omit = ["tests/*", "prefect_ray/_version.py"]
 
 [tool.coverage.report]
 fail_under = 80
 show_missing = true
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
+asyncio_mode = "auto"
```

### Comparing `prefect_ray-0.3.5/tests/test_block_standards.py` & `prefect_ray-0.3.6/tests/test_block_standards.py`

 * *Files identical despite different names*

### Comparing `prefect_ray-0.3.5/tests/test_context.py` & `prefect_ray-0.3.6/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `prefect_ray-0.3.5/tests/test_task_runners.py` & `prefect_ray-0.3.6/tests/test_task_runners.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
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
 
     loop = policy.new_event_loop()
 
     # configure asyncio logging to capture long running tasks
```

