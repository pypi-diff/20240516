# Comparing `tmp/prefect_docker-0.5.1.tar.gz` & `tmp/prefect_docker-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_docker-0.5.1.tar", last modified: Fri Apr 26 15:03:55 2024, max compression
+gzip compressed data, was "prefect_docker-0.5.2.tar", last modified: Thu May 16 20:58:36 2024, max compression
```

## Comparing `prefect_docker-0.5.1.tar` & `prefect_docker-0.5.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:55.648860 prefect_docker-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-26 15:03:55.648860 prefect_docker-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:55.644860 prefect_docker-0.5.1/prefect_docker/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:03:55.000000 prefect_docker-0.5.1/prefect_docker/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:55.644860 prefect_docker-0.5.1/prefect_docker/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/deployments/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/images.py
--rw-r--r--   0 runner    (1001) docker     (127)    30166 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/prefect_docker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:55.648860 prefect_docker-0.5.1/prefect_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-26 15:03:55.000000 prefect_docker-0.5.1/prefect_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-04-26 15:03:55.000000 prefect_docker-0.5.1/prefect_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:03:55.000000 prefect_docker-0.5.1/prefect_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 15:03:55.000000 prefect_docker-0.5.1/prefect_docker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-26 15:03:55.000000 prefect_docker-0.5.1/prefect_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 15:03:55.000000 prefect_docker-0.5.1/prefect_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:03:55.648860 prefect_docker-0.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:55.644860 prefect_docker-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:55.644860 prefect_docker-0.5.1/tests/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)    11631 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/deployments/test_steps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:55.648860 prefect_docker-0.5.1/tests/test-project/
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test-project/flow.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test-project/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test_host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test_images.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    46168 2024-04-26 15:03:42.000000 prefect_docker-0.5.1/tests/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.134754 prefect_docker-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-16 20:58:36.130754 prefect_docker-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.126754 prefect_docker-0.5.2/prefect_docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:35.000000 prefect_docker-0.5.2/prefect_docker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8023 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.130754 prefect_docker-0.5.2/prefect_docker/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30166 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/prefect_docker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.130754 prefect_docker-0.5.2/prefect_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-16 20:58:35.000000 prefect_docker-0.5.2/prefect_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-16 20:58:36.000000 prefect_docker-0.5.2/prefect_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:35.000000 prefect_docker-0.5.2/prefect_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 20:58:35.000000 prefect_docker-0.5.2/prefect_docker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 20:58:35.000000 prefect_docker-0.5.2/prefect_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 20:58:35.000000 prefect_docker-0.5.2/prefect_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:36.134754 prefect_docker-0.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.130754 prefect_docker-0.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.130754 prefect_docker-0.5.2/tests/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/deployments/test_steps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:36.130754 prefect_docker-0.5.2/tests/test-project/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test-project/flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test-project/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46168 2024-05-16 20:58:24.000000 prefect_docker-0.5.2/tests/test_worker.py
```

### Comparing `prefect_docker-0.5.1/LICENSE` & `prefect_docker-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.1/PKG-INFO` & `prefect_docker-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.5.1
+Version: 0.5.2
 Summary: Prefect integrations for interacting with Docker.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-docker
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
-Requires-Dist: prefect>=2.13.5
+Requires-Dist: prefect<3.0.0,>=2.13.5
 Requires-Dist: docker>=6.1.1
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
```

### Comparing `prefect_docker-0.5.1/README.md` & `prefect_docker-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.1/prefect_docker/containers.py` & `prefect_docker-0.5.2/prefect_docker/containers.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.1/prefect_docker/credentials.py` & `prefect_docker-0.5.2/prefect_docker/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.1/prefect_docker/deployments/steps.py` & `prefect_docker-0.5.2/prefect_docker/deployments/steps.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.1/prefect_docker/host.py` & `prefect_docker-0.5.2/prefect_docker/host.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.1/prefect_docker/images.py` & `prefect_docker-0.5.2/prefect_docker/images.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.1/prefect_docker/worker.py` & `prefect_docker-0.5.2/prefect_docker/worker.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.1/prefect_docker.egg-info/PKG-INFO` & `prefect_docker-0.5.2/prefect_docker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-docker
-Version: 0.5.1
+Version: 0.5.2
 Summary: Prefect integrations for interacting with Docker.
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-docker
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
-Requires-Dist: prefect>=2.13.5
+Requires-Dist: prefect<3.0.0,>=2.13.5
 Requires-Dist: docker>=6.1.1
 Provides-Extra: dev
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: mkdocs-gen-files; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs; extra == "dev"
```

### Comparing `prefect_docker-0.5.1/prefect_docker.egg-info/SOURCES.txt` & `prefect_docker-0.5.2/prefect_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.1/pyproject.toml` & `prefect_docker-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
 ]
-dependencies = ["prefect>=2.13.5", "docker>=6.1.1"]
+dependencies = ["prefect>=2.13.5, < 3.0.0", "docker>=6.1.1"]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = [
   "coverage",
   "interrogate",
   "mkdocs-gen-files",
```

### Comparing `prefect_docker-0.5.1/tests/conftest.py` & `prefect_docker-0.5.2/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,27 +46,19 @@
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

### Comparing `prefect_docker-0.5.1/tests/deployments/test_steps.py` & `prefect_docker-0.5.2/tests/deployments/test_steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,18 +229,15 @@
 
         output = docker_client_with_cleanup.containers.run(
             image=result["image"],
             command="python -c 'import pandas; print(pandas.__version__)'",
             labels=["prefect-docker-test"],
             remove=True,
         )
-        if sys.version_info >= (3, 8):
-            assert "2" in output.decode()
-        else:
-            assert "1" in output.decode()
+        assert "2" in output.decode()
 
     finally:
         docker_client_with_cleanup.containers.prune(
             filters={"label": "prefect-docker-test"}
         )
         image = docker_client_with_cleanup.images.get("local/repo:test")
         if image:
```

### Comparing `prefect_docker-0.5.1/tests/test-project/flow.py` & `prefect_docker-0.5.2/tests/test-project/flow.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.1/tests/test_containers.py` & `prefect_docker-0.5.2/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.1/tests/test_host.py` & `prefect_docker-0.5.2/tests/test_host.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.1/tests/test_images.py` & `prefect_docker-0.5.2/tests/test_images.py`

 * *Files identical despite different names*

### Comparing `prefect_docker-0.5.1/tests/test_worker.py` & `prefect_docker-0.5.2/tests/test_worker.py`

 * *Files identical despite different names*

