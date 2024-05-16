# Comparing `tmp/pyhectiqlab-3.0.5.tar.gz` & `tmp/pyhectiqlab-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhectiqlab-3.0.5.tar", last modified: Wed May 15 14:37:12 2024, max compression
+gzip compressed data, was "pyhectiqlab-3.0.7.tar", last modified: Thu May 16 18:07:05 2024, max compression
```

## Comparing `pyhectiqlab-3.0.5.tar` & `pyhectiqlab-3.0.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:12.290318 pyhectiqlab-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-15 14:37:12.290318 pyhectiqlab-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:12.286318 pyhectiqlab-3.0.5/pyhectiqlab/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5600 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:12.286318 pyhectiqlab-3.0.5/pyhectiqlab/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     9350 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    15594 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:12.290318 pyhectiqlab-3.0.5/pyhectiqlab/functional/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/block.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/functional/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    14721 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    24795 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:12.290318 pyhectiqlab-3.0.5/pyhectiqlab/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/step.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyhectiqlab/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:12.290318 pyhectiqlab-3.0.5/pyhectiqlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-15 14:37:12.000000 pyhectiqlab-3.0.5/pyhectiqlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-15 14:37:12.000000 pyhectiqlab-3.0.5/pyhectiqlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:37:12.000000 pyhectiqlab-3.0.5/pyhectiqlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-15 14:37:12.000000 pyhectiqlab-3.0.5/pyhectiqlab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-15 14:37:12.000000 pyhectiqlab-3.0.5/pyhectiqlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-15 14:37:12.000000 pyhectiqlab-3.0.5/pyhectiqlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:37:12.290318 pyhectiqlab-3.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:37:12.290318 pyhectiqlab-3.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-15 14:36:55.000000 pyhectiqlab-3.0.5/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:07:05.058126 pyhectiqlab-3.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-16 18:07:05.058126 pyhectiqlab-3.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:07:05.054126 pyhectiqlab-3.0.7/pyhectiqlab/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:07:05.054126 pyhectiqlab-3.0.7/pyhectiqlab/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:07:05.058126 pyhectiqlab-3.0.7/pyhectiqlab/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/functional/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4845 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24784 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:07:05.058126 pyhectiqlab-3.0.7/pyhectiqlab/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyhectiqlab/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:07:05.058126 pyhectiqlab-3.0.7/pyhectiqlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-16 18:07:05.000000 pyhectiqlab-3.0.7/pyhectiqlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-16 18:07:05.000000 pyhectiqlab-3.0.7/pyhectiqlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:07:05.000000 pyhectiqlab-3.0.7/pyhectiqlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 18:07:05.000000 pyhectiqlab-3.0.7/pyhectiqlab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-16 18:07:05.000000 pyhectiqlab-3.0.7/pyhectiqlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 18:07:05.000000 pyhectiqlab-3.0.7/pyhectiqlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 18:07:05.062126 pyhectiqlab-3.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:07:05.058126 pyhectiqlab-3.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-16 18:06:45.000000 pyhectiqlab-3.0.7/tests/test_run.py
```

### Comparing `pyhectiqlab-3.0.5/PKG-INFO` & `pyhectiqlab-3.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhectiqlab
-Version: 3.0.5
+Version: 3.0.7
 Summary: Python client for the Hectiq Lab plateform.
 Author-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Maintainer-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Project-URL: Repository, https://github.com/HectiqAI/hectiq-lab-revision.git
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
```

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/__init__.py` & `pyhectiqlab-3.0.7/pyhectiqlab/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-__version__ = "3.0.5"
+__version__ = "3.0.7"
 
 from pyhectiqlab.settings import getenv
 
 API_URL = getenv("HECTIQLAB_API_URL", "https://api.lab.hectiq.ai")
 
 from pyhectiqlab.config import Config
 from pyhectiqlab.dataset import Dataset
 from pyhectiqlab.model import Model
 from pyhectiqlab.run import Run
 from pyhectiqlab import functional
 
+
 def debug_mode():
     from pyhectiqlab.client import Client
+
     Client.online(False)
 
+
 __all__ = [
     "API_URL",
     "Artifact",
     "Dataset",
     "Model",
     "Run",
     "Config",
```

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/artifact.py` & `pyhectiqlab-3.0.7/pyhectiqlab/artifact.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from pyhectiqlab.decorators import online_method, functional_alias
 
 
 class Artifact:
 
     @staticmethod
     @online_method
-    @functional_alias("add_artifact")
     @clisync.include(wait_response=True)
     def create(
         local_path: str,
         run_id: str,
         project: str,
         name: Optional[str] = None,
         step: Optional[int] = None,
@@ -32,16 +31,25 @@
             step (int, optional): Step number. If None, the artifact is not considered as a step artifact. Default: None.
             group (str, optional): Group name. If None, the group is determined from the local_path. Default: None.
             wait_response (bool): Set to true to upload sync. If False, the upload is made in background. Default: False.
         """
         name = name or os.path.basename(local_path)
         group = group or os.path.basename(local_path)
         num_bytes = os.path.getsize(local_path)
+        extension = os.path.splitext(local_path)[1]
 
-        json = {"name": name, "num_bytes": num_bytes, "group": group, "step": step, "project": project, "run": run_id}
+        json = {
+            "name": name,
+            "num_bytes": num_bytes,
+            "group": group,
+            "step": step,
+            "project": project,
+            "run": run_id,
+            "extension": extension,
+        }
 
         async def composition():
             artifact = Client.post("/app/artifacts", wait_response=True, json=json)
             if not artifact:
                 return
             return await Client.upload(local_path=local_path, policy=artifact.get("upload_policy"))
```

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/auth.py` & `pyhectiqlab-3.0.7/pyhectiqlab/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 import httpx
 import toml
-import warnings
+import logging
 
 from pyhectiqlab import API_URL
 from pathlib import Path
 from typing import Optional, Union
 
 
 def load_credentials(name: Optional[str] = None) -> Union[None, str]:
@@ -78,15 +78,15 @@
     @property
     def auth_token_header(self):
         return {"Authentification": f"Bearer {self.access_token}"} if self.access_token is not None else {}
 
     def refresh_token(self):
         response = httpx.post(f"{API_URL}/app/auth/auth-api-key", headers=self.auth_header)
         if response.status_code != 200:
-            warnings.warn(f"User could not be authenticated. Continuing in offline mode.")
+            logging.error(f"User could not be authenticated. Continuing in offline mode.")
             return
         self.access_token = response.cookies["access_token"]
 
     def auth_flow(self, request: httpx.Request):
         request.headers.update(self.auth_token_header)
         response = yield request
```

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/block.py` & `pyhectiqlab-3.0.7/pyhectiqlab/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import clisync
-import warnings
+import logging
 from typing import Optional, List
 
 from pyhectiqlab.const import DISABLE_BLOCK_CREATION
 from pyhectiqlab.project import Project
 from pyhectiqlab.client import Client
 from pyhectiqlab.decorators import functional_alias, online_method
 
@@ -44,15 +44,15 @@
 
         Args:
             title (str): Block title.
             status (str, optional): Block status. Default: None.
             project (str, optional): Project name. If None, the current project is used. Default: None.
         """
         if DISABLE_BLOCK_CREATION:
-            warnings.warn("Block creation is disabled. Continuing anyway...")
+            logging.error("Block creation is disabled. Continuing anyway...")
             return
         project = project or Project.get()
         if not project:
             return None
 
         body = {"title": title, "status": status, "project": project}
         block = Client.post("/app/blocks", json=body, wait_response=wait_response)
```

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/cli/__init__.py` & `pyhectiqlab-3.0.7/pyhectiqlab/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/cli/auth.py` & `pyhectiqlab-3.0.7/pyhectiqlab/cli/auth.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/client.py` & `pyhectiqlab-3.0.7/pyhectiqlab/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,25 +38,26 @@
     response = asyncio.run(client.async_get("/app/auth/is-logged-in"))
     ```
     """
 
     _auth: Auth = None
     _client: httpx.Client = None
     _online: bool = True
+    _timeout: float = 30.0  # seconds
 
     @classproperty
     def auth(cls) -> Auth:
         if cls._auth is None:
             cls._auth = Auth()
         return cls._auth
 
     @classproperty
     def client(cls) -> httpx.Client:
         if cls._client is None:
-            cls._client = httpx.Client(auth=cls.auth)
+            cls._client = httpx.Client(auth=cls.auth, timeout=cls._timeout)
         return cls._client
 
     @staticmethod
     def is_logged():
         return Client.auth.is_logged()
 
     @staticmethod
@@ -88,15 +89,15 @@
     @staticmethod
     async def upload(local_path: str, policy: dict) -> ResponseType:
         """Upload a file."""
         upload_method = policy.get("upload_method")
         if not upload_method:
             return
 
-        async with httpx.AsyncClient() as asyncClient:
+        async with httpx.AsyncClient(timeout=Client._timeout) as asyncClient:
             if upload_method == "fragment":
                 res = await Client.upload_fragment(local_path, policy, client=asyncClient)
             elif upload_method == "single":
                 res = await Client.upload_single(
                     local_path, policy.get("policy"), bucket=policy.get("bucket_name"), client=asyncClient
                 )
         return res
@@ -148,15 +149,17 @@
         progress_bar = tqdm.tqdm(total=upload.total_bytes, unit="iB", unit_scale=True)
 
         bytes_uploaded = 0
         while upload.finished == False:
             method, url, payload, headers = upload._prepare_request()
             if headers.get("content-type") == None:
                 headers["content-type"] = "application/octet-stream"
-            result = await (client or httpx).request(method, url, data=payload, headers=headers)
+            result = await (client or httpx).request(
+                method, url, data=payload, headers=headers, timeout=Client._timeout
+            )
             upload._process_resumable_response(result, len(payload))
             progress_bar.update(upload.bytes_uploaded - bytes_uploaded)
             bytes_uploaded = upload.bytes_uploaded
         progress_bar.close()
 
     @staticmethod
     async def upload_single(
```

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/dataset.py` & `pyhectiqlab-3.0.7/pyhectiqlab/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import clisync
-from typing import Optional, List, Union
 import asyncio
-import warnings
+import shutil
+import logging
+
+from typing import Optional, List, Union
 
 from pyhectiqlab.tag import Tag
 from pyhectiqlab.project import Project
 from pyhectiqlab.block import Block
 from pyhectiqlab.block import Block
 from pyhectiqlab.client import Client
 from pyhectiqlab.decorators import functional_alias, online_method
@@ -25,15 +27,15 @@
         source: str,
         host: Optional[str] = None,
         description: Optional[str] = None,
         version: Optional[str] = None,
         block: Optional[str] = None,
         run_id: Optional[str] = None,
         project: Optional[str] = None,
-        upload: Optional[bool] = False
+        upload: Optional[bool] = False,
     ):
         """Create a dataset.
 
         Supported cloud storages:
         - Amazon S3
         - Google Cloud Storage
 
@@ -47,19 +49,20 @@
             version (str]): Version of the dataset. Default: None.
             block (str, optional): Block of the dataset. Default: None.
             run_id (str, optional): Run of the dataset. Default: None.
             project (str, optional): Project of the dataset. Default: None.
             upload (bool): If True, upload the dataset to the Lab. Default: False.
         """
         from pyhectiqlab.run import Run
+
         project = Project.get(project)
         run_id = Run.get_id(run_id)
         block = Block.get(block)
         if project is None:
-            warnings.warn("Project not found, skipping dataset creation.")
+            logging.error("Project not found, skipping dataset creation.")
             return
 
         if name is None:
             raise ValueError("The `name` parameter is required.")
 
         if source is None:
             raise ValueError("The `source` parameter is required.")
@@ -87,18 +90,17 @@
         Dataset.attach(name=name, version=version, run_id=run_id, project=project)
         return dataset
 
     @staticmethod
     @online_method
     @functional_alias("upload_dataset")
     @clisync.include()
-    def upload(id: str, 
-               source: str):
+    def upload(id: str, source: str):
         """Upload local files to a dataset hosted in the Lab.
-        
+
         Args:
             id (str): ID of the dataset.
             path (str): Path to the directory containing the files to upload.
         """
         all_files = list_all_files_in_dir(source)
         batch_size = 50
         Dataset._id = dataset_id = id
@@ -117,33 +119,28 @@
             # Upload dataset files
             asyncio.run(Dataset._client.upload_many(paths=batch, policies=sorted_files))
 
     @staticmethod
     @online_method
     @functional_alias("retrieve_dataset")
     @clisync.include()
-    def retrieve(
-        name: str,
-        version: str,
-        project: str,
-        fields: Optional[List[str]] = None
-    ):
+    def retrieve(name: str, version: str, project: str, fields: Optional[List[str]] = None):
         """Retrieve a dataset
 
         Args:
             name (str): Name of the dataset
             project (str): Project of the dataset
             version (str): Version of the dataset
             fields (list[str], optional): Fields to retrieve. Default: None.
         """
         body = Dataset._client.get(
             "/app/datasets/retrieve",
             params={
                 "name": name,
-                "project": project,
+                "project": Project.get(project),
                 "version": version,
                 "fields": fields or [],
             },
             wait_response=True,
         )
         return body
 
@@ -158,15 +155,15 @@
         block: Optional[str] = None,
         blocks: Optional[List[str]] = None,
         keep_latest_version: bool = False,
         fields: Optional[List[str]] = [],
         page: Optional[int] = 1,
         limit: Optional[int] = 100,
         order_by: Optional[str] = "created_at",
-        order_direction: Optional[str] = "desc"
+        order_direction: Optional[str] = "desc",
     ):
         """List the datasets
 
         Args:
             project (str, optional): Project of the dataset.
             block (str, optional): Block of the dataset.
             search (str, optional): Search string.
@@ -264,29 +261,44 @@
     @functional_alias("download_dataset")
     @clisync.include(wait_response=True)
     def download(
         name: str,
         version: str,
         project: Optional[str] = None,
         path: Optional[str] = "./",
-        wait_response: bool = False,
+        overwrite: bool = False,
+        wait_response: bool = True,
     ):
         """Download a dataset
 
         Args:
             name (str): Name of the dataset.
             version (str): Version of the dataset.
             project (str, optional): Project of the dataset.
             path (str): Path to download the dataset. Default: "./".
+            overwrite (bool): Overwrite the existing files. Default: False.
             wait_response (bool): Wait for the response from the server. Default: False.
         """
+        from pyhectiqlab import Run
+
         path = path or "./"
-        path = os.path.join(path, f"{name}-{version.replace('.', '-')}")
+        path = os.path.join(path, f"{name}-{version}")
+        if os.path.exists(path):
+            if not overwrite:
+                logging.warning(f"Directory {path} already exists. Set `overwrite=True` to overwrite the files.")
+                return path
+
+            shutil.rmtree(path)
+
         os.makedirs(path, exist_ok=True)
-        Dataset.attach(name=name, version=version, project=project, wait_response=True)
+        run_id = Run.get_id()
+        project = Project.get(project)
+        if run_id is not None:
+            Dataset.attach(name=name, version=version, run_id=run_id, project=project)
+
         async def composition():
             dataset = Dataset.retrieve(name=name, project=project, version=version, fields=["id"])
             if not dataset:
                 return
             dataset_id = dataset["id"]
 
             num_results = 0
@@ -306,15 +318,16 @@
                     num_bytes=[file["num_bytes"] for file in files["results"]],
                 )
                 num_results += len(files["results"])
                 page += 1
 
             Dataset._client.post(f"/app/datasets/{dataset_id}/on-download-completed", wait_response=False)
 
-        return Dataset._client.execute(composition, wait_response=wait_response, is_async_method=True)
+        Dataset._client.execute(composition, wait_response=wait_response, is_async_method=True)
+        return path
 
     @staticmethod
     @online_method
     def attach(
         name: str,
         version: str,
         run_id: Optional[str] = None,
@@ -327,14 +340,15 @@
             name (str): Name of the dataset.
             version (str): Version of the dataset.
             run_id (str): ID of the run.
             project (str, optional): Project of the dataset.
             wait_response (bool): Wait for the response from the server. Default: False.
         """
         from pyhectiqlab.run import Run
+
         run_id = Run.get_id(run_id)
         if run_id is None:
             return
         dataset = Dataset.retrieve(name=name, project=project, version=version, fields=["id"])
         if dataset is None:
             return
         return Dataset._client.post(
@@ -367,14 +381,15 @@
         dataset_id = dataset["id"]
         return Dataset._client.post(
             f"/app/datasets/{dataset_id}/detach-from-run/{run_id}", wait_response=wait_response
         )
 
     @staticmethod
     @online_method
+    @functional_alias("add_tags_to_dataset")
     def add_tags(
         tags: Union[str, List[str]],
         name: str,
         version: str,
         project: Optional[str] = None,
         wait_response: Optional[bool] = False,
     ):
@@ -392,14 +407,15 @@
         if not dataset:
             return
         dataset_id = dataset["id"]
         return Tag.attach_to_dataset(tags=tags, dataset_id=dataset_id, project=project, wait_response=wait_response)
 
     @staticmethod
     @online_method
+    @functional_alias("detach_tag_from_dataset")
     def detach_tag(
         tag: str,
         name: str,
         version: str,
         project: Optional[str] = None,
         wait_response: Optional[bool] = False,
     ):
```

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/decorators.py` & `pyhectiqlab-3.0.7/pyhectiqlab/decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from functools import wraps
 from typing import Optional, Union
 
-import warnings
 import logging
 
 logger = logging.getLogger()
 
 
 class classproperty(property):
     def __get__(self, cls, owner):
@@ -15,15 +14,15 @@
 def online_method(f):
 
     @wraps(f)
     def wrapper(*args, **kwargs):
         from pyhectiqlab.client import Client
 
         if not Client.online():
-            warnings.warn(f"`{f.__name__}` not executed. Dry (offline) mode.")
+            logging.error(f"`{f.__name__}` not executed. Dry (offline) mode.")
             return
         return f(*args, **kwargs)
 
     return wrapper
 
 
 def no_git_diff(force: bool = False):
@@ -33,36 +32,36 @@
         def wrapper(*args, **kwargs):
             from pyhectiqlab.project import Project
             from pyhectiqlab.versions import PackageVersion
 
             if force:
                 return f(*args, **kwargs)
             if Project.allow_dirty() and PackageVersion.is_dirty():
-                warnings.warn(f"`{f.__name__}` not executed. There are uncommited changes in the repository.")
+                logging.error(f"`{f.__name__}` not executed. There are uncommited changes in the repository.")
             return f(*args, **kwargs)
 
         return wrapper
 
     return _wrapper
 
 
 def beta(f):
     @wraps(f)
     def wrapper(self, *args, **kwargs):
-        warnings.warn("This method is still in development and can be unstable.")
+        logging.error("This method is still in development and can be unstable.")
         return f(self, *args, **kwargs)
 
     return wrapper
 
 
 def will_be_depreciated(suggested_method):
     def _method(f):
         @wraps(f)
         def wrapper(self, *args, **kwargs):
-            warnings.warn(
+            logging.error(
                 f"The method `{f.__name__}` will be removed in a future release. Use `{suggested_method}` instead."
             )
             return f(self, *args, **kwargs)
 
         return wrapper
 
     return _method
@@ -86,15 +85,15 @@
     Instead of returning the response, return the response.json() if the status code is 200.
     If the status code is not 200, log the error and return None.
     """
 
     def wrapper(*args, **kwargs) -> Union[dict, bytes, None]:
         response = f(*args, **kwargs)
         if response.status_code != 200:
-            warnings.warn(f"Request failed with status code {response.status_code}: {response.content}")
+            logging.error(f"Request failed with status code {response.status_code}: {response.content}")
             return None
         try:
             return response.json()
         except:
             return response.content
 
     return wrapper
```

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/logging.py` & `pyhectiqlab-3.0.7/pyhectiqlab/logging.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/metrics.py` & `pyhectiqlab-3.0.7/pyhectiqlab/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,27 +51,27 @@
     """
 
     __max_cache_quantity_per_second = 200
 
     def __init__(
         self,
         push_method: Callable[[str, List[float]], None],
-        run: Optional[str] = None,
+        run_id: Optional[str] = None,
         max_cache_timeout: int = 10,
         max_cache_length: int = 100,
         min_cache_flush_delay: int = 5,
         aggregate_metrics: str = "none",
     ):
         self.cache = defaultdict(list)
         self.cache_last_push = {}
         self._warning_is_shown = False
         self.max_cache_length = max_cache_length
         self.min_cache_flush_delay = min_cache_flush_delay
 
-        self.push_method = partial(push_method, run=run)
+        self.push_method = partial(push_method, run_id=run_id)
         self.set_aggr(aggregate_metrics)
 
         self.timer = RepeatedTimer(self.flush_cache, max_cache_timeout)
         self.timer.start()
         return
 
     def update_cache_settings(
```

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/model.py` & `pyhectiqlab-3.0.7/pyhectiqlab/model.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import clisync
 import asyncio
-import warnings
+import logging
+import shutil
 
 from typing import Optional, List, Union
 
 from pyhectiqlab.tag import Tag
 from pyhectiqlab.block import Block
 from pyhectiqlab.project import Project
 from pyhectiqlab.client import Client
@@ -24,40 +25,41 @@
         name: str,
         path: Optional[str] = None,
         version: Optional[str] = None,
         run_id: Optional[str] = None,
         project: Optional[str] = None,
         block: Optional[str] = None,
         description: Optional[str] = None,
-        upload: Optional[bool] = True
+        upload: Optional[bool] = True,
     ):
         """Create a model
 
         Args:
             name (str): Name of the model
             run_id (str, optional):  ID of the run
             project (str, optional): Project of the model
             path (str, optional): Path to the model directory
             description (str, optional): Description of the model
             version (str, optional): Version of the model
             block (str, optional): Block of the model
             upload (bool, optional): Upload the model files. Default: True
         """
         from pyhectiqlab.run import Run
+
         project = Project.get(project)
         run_id = Run.get_id(run_id)
         block = Block.get(block)
 
         if project is None:
-            warnings.warn("Project not found, skipping model creation.")
+            logging.error("Project not found, skipping model creation.")
             return
-        
+
         if name is None:
             raise ValueError("The `name` parameter is required.")
-        
+
         if block:
             if "::" not in block:
                 block = Block.format_id(block, project)
 
         json = {
             "name": name,
             "description": description,
@@ -66,27 +68,26 @@
             "project": project,
             "root_run": run_id,
         }
 
         model = Model._client.post("/app/models", wait_response=True, json=json)
         if not model or "id" not in model:
             return
-        
+
         if upload and path:
             Model.upload(id=model["id"], path=path)
 
         Model.attach(name=name, version=version, run_id=run_id, project=project, wait_response=True)
         return model
 
     @staticmethod
     @online_method
     @functional_alias("upload_model")
     @clisync.include()
-    def upload(id: str, 
-               path: str):
+    def upload(id: str, path: str):
         """Upload local files to a model hosted in the Lab.
 
         Args:
             id (str): ID of the model.
             path (str): Path to the model directory.
         """
         all_files = list_all_files_in_dir(path)
@@ -255,35 +256,42 @@
             model = Model.retrieve(name=name, project=project, version=version, fields=["id"])
             if not model:
                 return
             id = model["id"]
         return Model._client.delete(f"/app/models/{id}", wait_response=wait_response)
 
     @staticmethod
-    @online_method
     @functional_alias("download_model")
     @clisync.include(wait_response=True)
     def download(
         name: str,
         version: str,
         project: Optional[str] = None,
         path: Optional[str] = "./",
-        wait_response: bool = False,
+        overwrite: bool = False,
+        wait_response: bool = True,
     ):
         """Download a model
 
         Args:
             name (str): Name of the model
             project (str): Project of the model
             version (str): Version of the model
             path (str, optional): Path to download the model
+            overwrite (bool, optional): Overwrite the files if they already exist
             wait_response (bool, optional): Wait for the response from the server
         """
         path = path or "./"
-        path = os.path.join(path, f"{name}-{version.replace('.', '-')}")
+        path = os.path.join(path, f"{name}-{version}")
+        if os.path.exists(path):
+            if not overwrite:
+                logging.warning(f"Directory {path} already exists. Set `overwrite=True` to overwrite the files.")
+                return path
+
+            shutil.rmtree(path)
         os.makedirs(path, exist_ok=True)
         from pyhectiqlab import Run
 
         project = Project.get(project)
 
         async def composition():
             model = Model.retrieve(name=name, project=project, version=version, fields=["id"])
@@ -311,15 +319,18 @@
                     num_bytes=[file["num_bytes"] for file in files["results"]],
                 )
                 num_results += len(files["results"])
                 page += 1
 
             Model._client.post(f"/app/models/{model_id}/on-download-completed", wait_response=False)
 
-        return Model._client.execute(composition, wait_response=wait_response, is_async_method=True)
+        res = Model._client.execute(composition, wait_response=wait_response, is_async_method=True)
+        if isinstance(res, asyncio.Task):
+            return res
+        return path
 
     @staticmethod
     @online_method
     def attach(
         name: str,
         version: str,
         run_id: Optional[str] = None,
@@ -332,14 +343,15 @@
             run_id (str): ID of the run.
             name (str): Name of the model.
             version (str): Version of the model.
             project (str, optional): Project of the model. If None, the project of the current run is used. Default: None.
             wait_response (bool, optional): Wait for the response from the server. Default: False.
         """
         from pyhectiqlab.run import Run
+
         run_id = Run.get_id(run_id)
         if run_id is None:
             return
         project = Project.get(project)
         model = Model.retrieve(name=name, project=project, version=version, fields=["id"])
         if not model:
             return
@@ -369,14 +381,15 @@
         if not model:
             return
         model_id = model["id"]
         return Model._client.post(f"/app/models/{model_id}/detach-from-run/{run_id}", wait_response=wait_response)
 
     @staticmethod
     @online_method
+    @functional_alias("add_tags_to_model")
     def add_tags(
         tags: Union[str, List[str]],
         name: str,
         version: str,
         project: Optional[str] = None,
     ):
         """Add tags to a model
@@ -392,14 +405,15 @@
         if not model:
             return
         model_id = model["id"]
         return Tag.attach_to_model(tags=tags, model_id=model_id, project=project)
 
     @staticmethod
     @online_method
+    @functional_alias("detach_tag_from_model")
     def detach_tag(
         tag: str,
         name: str,
         version: str,
         project: Optional[str] = None,
     ):
         """Remove a tag from the model.
```

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/project.py` & `pyhectiqlab-3.0.7/pyhectiqlab/project.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import warnings
 import slugify
 import clisync
 import toml
 import os
 import logging
 
 from typing import Optional, List
@@ -70,26 +69,26 @@
             repo (str, optional): Repository URL. Default: None.
             force_no_git_diff (bool): Force no git diff. Default: True.
             write_config (bool): Write the config file. Default: True.
         """
         from pyhectiqlab.const import DISABLE_PROJECT_CREATION
 
         if DISABLE_PROJECT_CREATION:
-            warnings.warn("Project creation is disabled. Continuing anyway...")
+            logging.error("Project creation is disabled. Continuing anyway...")
             return
         slug = "/".join([slugify.slugify(n) for n in name.split("/")])
         body = {
             "slug": slug,
             "name": name,
             "repo": repo,
             "force_no_git_diff": force_no_git_diff,
         }
         project = Project._client.post("/app/projects", json=body, wait_response=True)
         if project is None:
-            warnings.warn("Failed to create project.")
+            logging.error(f"Failed to create project.")
             return
         if write_config:
             Project.write_config(slug)
         logger.info(f"Project `{slug}` created.")
         return slug
 
     @staticmethod
@@ -141,11 +140,11 @@
     def get(slug: Optional[str] = None):
         return slug or Project._slug
 
     @staticmethod
     @functional_alias("set_project")
     def set(slug: str):
         if not Project.exists(slug):
-            warnings.warn(f"The project `{slug}` does not exist. Continuing with the current project.")
+            logging.error(f"The project `{slug}` does not exist. Continuing with the current project.")
             Project._client.online(False)
             return
         Project._slug = slug
```

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/run.py` & `pyhectiqlab-3.0.7/pyhectiqlab/run.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 import tempfile
 import slugify
 import logging
-import warnings
 import clisync
 
 from typing import Any, List, Optional, Union, Literal, Tuple
 
 from pyhectiqlab import API_URL
 from pyhectiqlab import Config
 from pyhectiqlab.project import Project
@@ -37,30 +36,24 @@
 
     def __init__(
         self,
         rank: Optional[int] = None,
         title: Optional[str] = None,
         project: Optional[str] = None,
         block: Optional[str] = None,
-        category: Literal[None, "Develop", "Evaluation", "Test", "Training"] = None,
+        category: Literal[None, "develop", "evaluation", "test", "training"] = None,
         config: Optional[dict] = None,
     ):
-        if rank is not None:
+        if rank is not None and isinstance(rank, int):
             self.retrieve(rank, project)
-        else:
+        elif isinstance(rank, str) or rank is None:
+            title = title or rank  # support for positional argument
             self.create(title=title, project=project, block=block, category=category, config=config)
 
-    def __enter__(
-        self,
-        name: str,
-        description: Optional[str] = None,
-        metadata: Optional[dict] = None,
-        status: Optional[str] = None,
-    ):
-        self.start(name=name, description=description, metadata=metadata, status=status)
+    def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         if self._metrics:
             self._metrics.flush_cache()
         if Run.id is None:
             return
@@ -155,20 +148,17 @@
             tags (list): The tags of the run. Default: None.
             online (bool): Set to True to create the run online. Default: True.
         """
         if online:
             Run._client.online(online)
             return False
 
-        if project is not None:
-            Project.set(project)
-
         project = Project.get(project)
         if project is None:
-            warnings.warn("No project has been set. Please set a project first. Continuing in offline mode.")
+            logging.error("No project has been set. Please set a project first. Continuing in offline mode.")
             Run._client.online(False)
             return
         Project.set(project)
 
         if block is not None:
             if not "::" in block:
                 block = Block.format_id(block, project)
@@ -181,15 +171,15 @@
             category=category,
             config=config or {},
             tags=tags or [],
         )
 
         run = Run._client.post("/app/runs", json=data, wait_response=True)
         if run is None:
-            warnings.warn(f"Run failed to create.")
+            logging.error(f"Run failed to create.")
             return False
         Run.setup(**run)
         return run
 
     @staticmethod
     @functional_alias("retrieve_run")
     @no_git_diff()
@@ -207,24 +197,25 @@
         Args:
             rank (int): The rank of the run.
             project (str): The project of the run. If None, the project is taken from the context. Default: None.
             fields (List[str]): The fields to retrieve. Default: None.
         """
 
         project = Project.get(project)
-        Project.set(project)
         if project is None:
-            warnings.warn("No project has been set. Please set a project first. Continuing in offline mode.")
+            logging.error("No project has been set. Please set a project first. Continuing in offline mode.")
             Run._client.online(False)
             return
+        Project.set(project)
+
         run = Run._client.get(
             "/app/runs/retrieve", params=dict(rank=rank, project=project, fields=fields), wait_response=True
         )
         if run is None:
-            warnings.warn(f"Run {rank} not found in project {project}")
+            logging.error(f"Run {rank} not found in project {project}")
             return
         if setup_with_result:
             Run.setup(**run)
         return run
 
     @staticmethod
     @functional_alias("retrieve_run_by_id")
@@ -244,19 +235,19 @@
             project (str): The project of the run. If None, the project is taken from the context. Default: None.
             fields (List[str]): The fields to retrieve. Default: None.
             setup_with_result (bool): Set to True to setup the run with the result. Default: False.
         """
 
         run_id = run_id or Run.id
         if not run_id:
-            warnings.warn("No run to retrieve. ")
+            logging.error("No run to retrieve. ")
             return
         run_id = Run._client.get(f"/app/runs/{run_id}", params=dict(fields=fields), wait_response=True)
         if not run_id:
-            warnings.warn(f"Run not found.")
+            logging.error(f"Run not found.")
             return
         if setup_with_result:
             Run.setup(**run_id)
         return run_id
 
     @staticmethod
     @online_method
@@ -311,15 +302,15 @@
         return res is not None
 
     @staticmethod
     @online_method
     def _update(run_id: Optional[str] = None, wait_response: bool = False, **kwargs):
         run_id = run_id or Run.id
         if not (run_id):
-            warnings.warn("No run to update. Please create or retrieve a run first.")
+            logging.error("No run to update. Please create or retrieve a run first.")
             return
         return Run._client.patch(f"/app/runs/{run_id}", json=kwargs, wait_response=wait_response)
 
     @staticmethod
     @online_method
     @functional_alias("set_category")
     @clisync.include()
@@ -367,17 +358,19 @@
             path (str) : Path to the file.
             name (str, optional): Name of the artifact or the group of artifacts. If None, the name is the basename of the file. Default: None.
             step (int, optional): The optional step stamp of the artifacts. If None, the artifacts is not considered as a step artifact. Default: None.
             run_id (str, optional): ID of the run. If None, the current run ID is used. Default: None.
             project (str, optional): The project of the artifact. If None, the current project is used. Default: None.
             wait_response (bool): Set to true to upload sync. If False, the upload is made in background. Default: False.
         """
+        if Run.get_id(run_id) is None or Project.get(project) is None:
+            return
         return Artifact.create(
             path,
-            run_id or Run.id,
+            Run.get_id(run_id),
             Project.get(project),
             name=name,
             group=name,
             step=step,
             wait_response=wait_response,
         )
 
@@ -446,15 +439,15 @@
             value (float): The value of the metric.
 
         Note:
             The metrics are not pushed immediately. They are pushed when the `Run._push_metrics`
             method is called inside the MetricsManager. See `pyhectiqlab.metrics.MetricsManager`.
         """
         if Run._metrics is None:
-            Run._metrics = MetricsManager(push_method=Run._push_metrics, run=Run.id)
+            Run._metrics = MetricsManager(push_method=Run._push_metrics, run_id=Run.id)
         return Run._metrics.add(key, step, value)
 
     @staticmethod
     @online_method
     def _push_metrics(
         key: str,
         values: List[Tuple[Union[int, float], Union[int, float], Union[int, float]]],
@@ -652,14 +645,15 @@
     @functional_alias("run_is_training")
     def training(run_id: Optional[int] = None):
         """Set the run to the training status."""
         Run.set_status(run_id=run_id, status="training")
 
     @staticmethod
     @online_method
+    @functional_alias("add_tags_to_run")
     def add_tags(tags: Union[str, List[str]], run_id: Optional[str] = None, project: Optional[str] = None):
         """Add a tag to the run.
         For functional alias, use `attach_tags_to_run`.
 
         Args:
             title (str): The new title of the run.
             run_id (str): The ID of the run. If None, the current run is used. Default: None.
@@ -667,29 +661,30 @@
         """
         if isinstance(tags, str):
             tags = [tags]
         Tag.attach_to_run(tags, run_id=run_id or Run.id, project=Project.get(project))
 
     @staticmethod
     @online_method
+    @functional_alias("detach_tag_from_run")
     def detach_tag(tag: str, run_id: Optional[str] = None, project: Optional[str] = None):
         """Remove a tag from the run.
         For functional alias, use `detach_tag_from_run`.
 
         Args:
             title (str): The new title of the run.
             run_id (str): The ID of the run. If None, the current run is used. Default: None.
             project (str): The project of the run. If None, the current project is used. Default: None.
         """
         Tag.detach_from_run(tag=tag, run_id=run_id or Run.id, project=Project.get(project))
 
     def __str__(self):
         pad = 8
-        path = "/" + self.project + "/runs/" + str(self.rank)  # TBD
+        path = "/" + Project.get() + "/runs/" + str(self.rank)  # TBD
         return (
             f"<Run {self.rank}>"
-            f"\n{'Project'.ljust(pad)}: {self.project}"
-            f"\n{'Block'.ljust(pad)}: {self.block}"
-            f"\n{'author'.ljust(pad)}: {self._client._auth.user}"
-            f"\n{'online'.ljust(pad)}: {self._client._auth.online}"
+            f"\n{'Project'.ljust(pad)}: {Project.get()}"
+            f"\n{'Block'.ljust(pad)}: {Block.get()}"
+            f"\n{'author'.ljust(pad)}: {self._client.auth.user}"
+            f"\n{'online'.ljust(pad)}: {self._client.auth.online}"
             f"\n{'url'.ljust(pad)}: {API_URL+path} "
         )
```

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/settings/__init__.py` & `pyhectiqlab-3.0.7/pyhectiqlab/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/step.py` & `pyhectiqlab-3.0.7/pyhectiqlab/step.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/tag.py` & `pyhectiqlab-3.0.7/pyhectiqlab/tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             wait_response (bool): Set to true to create sync. If False, the creation is made in background. Default: False.
         """
         json = {"name": name, "color": color, "project": project}
         return Client.post("/app/tags", wait_response=wait_response, json=json)
 
     @staticmethod
     @online_method
-    @functional_alias("attach_tags_to_run")
+    # @functional_alias("attach_tags_to_run")
     @clisync.include()
     def attach_to_run(
         tags: List[str],
         run_id: str,
         project: str,
         wait_response: bool = False,
     ):
@@ -48,15 +48,15 @@
             wait_response (bool): Set to true to attach sync. If False, the attachment is made in background. Default: False.
         """
         json = {"run": run_id, "tags": tags, "project": project}
         return Client.post("/app/tags/attach-to-run", wait_response=wait_response, json=json)
 
     @staticmethod
     @online_method
-    @functional_alias("detach_tag_from_run")
+    # @functional_alias("detach_tag_from_run")
     @clisync.include()
     def detach_from_run(
         tag: str,
         run_id: str,
         project: str,
         wait_response: bool = False,
     ):
@@ -72,15 +72,15 @@
             f"/app/tags/detach-from-run",
             wait_response=wait_response,
             json={"run": run_id, "tag": tag, "project": project},
         )
 
     @staticmethod
     @online_method
-    @functional_alias("attach_tag_to_model")
+    # @functional_alias("attach_tag_to_model")
     @clisync.include()
     def attach_to_model(
         tags: List[str],
         model_id: str,
         project: str,
         wait_response: bool = False,
     ):
@@ -117,15 +117,15 @@
             f"/app/tags/detach-from-model",
             wait_response=wait_response,
             json={"model": model_id, "tag": tag, "project": project},
         )
 
     @staticmethod
     @online_method
-    @functional_alias("attach_tag_to_dataset")
+    # @functional_alias("attach_tag_to_dataset")
     @clisync.include()
     def attach_to_dataset(
         tags: List[str],
         dataset_id: str,
         project: str,
         wait_response: bool = False,
     ):
```

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/utils.py` & `pyhectiqlab-3.0.7/pyhectiqlab/utils.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab/versions.py` & `pyhectiqlab-3.0.7/pyhectiqlab/versions.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab.egg-info/PKG-INFO` & `pyhectiqlab-3.0.7/pyhectiqlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhectiqlab
-Version: 3.0.5
+Version: 3.0.7
 Summary: Python client for the Hectiq Lab plateform.
 Author-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Maintainer-email: Edward Laurence <edwardl@hectiq.ai>, Charles Murphy <cmurphy@hectiq.ai>
 Project-URL: Repository, https://github.com/HectiqAI/hectiq-lab-revision.git
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: httpx
```

### Comparing `pyhectiqlab-3.0.5/pyhectiqlab.egg-info/SOURCES.txt` & `pyhectiqlab-3.0.7/pyhectiqlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.5/pyproject.toml` & `pyhectiqlab-3.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,14 @@
 maintainers = [
   {name = "Edward Laurence", email = "edwardl@hectiq.ai"},
   {name = "Charles Murphy", email = "cmurphy@hectiq.ai"},
 ]
 name = "pyhectiqlab"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "3.0.5"
+version = "3.0.7"
 
 [project.urls]
 Repository = "https://github.com/HectiqAI/hectiq-lab-revision.git"
 
 [project.entry-points.console_scripts]
 hectiq-lab = "pyhectiqlab.cli:main"
```

### Comparing `pyhectiqlab-3.0.5/tests/test_dataset.py` & `pyhectiqlab-3.0.7/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.5/tests/test_model.py` & `pyhectiqlab-3.0.7/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.5/tests/test_project.py` & `pyhectiqlab-3.0.7/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pyhectiqlab-3.0.5/tests/test_run.py` & `pyhectiqlab-3.0.7/tests/test_run.py`

 * *Files 12% similar despite different names*

```diff
@@ -72,9 +72,19 @@
 
 def test_run_detach_tag():
     run = Run(rank=1, project="hectiq-ai/test")
     run.add_tags("some")
     run.detach_tag("some")
 
 
+def test_run_attach_dataset():
+    run = Run(rank=1, project="hectiq-ai/test")
+    print(run.attach_dataset(name="test-dataset", version="1.1", wait_response=True))
+
+
+def test_run_attach_model():
+    run = Run(rank=1, project="hectiq-ai/test")
+    print(run.attach_model(name="test-model", version="1.0", wait_response=True))
+
+
 if __name__ == "__main__":
     pass
```

