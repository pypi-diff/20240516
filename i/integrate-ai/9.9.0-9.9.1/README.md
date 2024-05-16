# Comparing `tmp/integrate-ai-9.9.0.tar.gz` & `tmp/integrate-ai-9.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integrate-ai-9.9.0.tar", last modified: Fri Apr 19 16:56:37 2024, max compression
+gzip compressed data, was "integrate-ai-9.9.1.tar", last modified: Mon Apr 29 13:27:42 2024, max compression
```

## Comparing `integrate-ai-9.9.0.tar` & `integrate-ai-9.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-19 16:56:37.369031 integrate-ai-9.9.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1075 2024-04-19 16:56:37.369031 integrate-ai-9.9.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      763 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/backend_shim.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-19 16:56:37.365031 integrate-ai-9.9.0/integrate_ai/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      657 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21141 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1081 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2692 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/sdk.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5678 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/server.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-19 16:56:37.369031 integrate-ai-9.9.0/integrate_ai/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8304 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/utils/docker_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/utils/error_handling.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/utils/logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/utils/path_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6025 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/utils/rest_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2840 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/integrate_ai/utils/typer_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-19 16:56:37.365031 integrate-ai-9.9.0/integrate_ai.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1075 2024-04-19 16:56:37.000000 integrate-ai-9.9.0/integrate_ai.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2024-04-19 16:56:37.000000 integrate-ai-9.9.0/integrate_ai.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-19 16:56:37.000000 integrate-ai-9.9.0/integrate_ai.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-04-19 16:56:37.000000 integrate-ai-9.9.0/integrate_ai.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-19 16:56:37.000000 integrate-ai-9.9.0/integrate_ai.egg-info/namespace_packages.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-19 16:56:37.000000 integrate-ai-9.9.0/integrate_ai.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-19 16:56:37.000000 integrate-ai-9.9.0/integrate_ai.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-19 16:56:37.369031 integrate-ai-9.9.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1748 2024-04-19 16:56:36.000000 integrate-ai-9.9.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 13:27:42.258869 integrate-ai-9.9.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1075 2024-04-29 13:27:42.258869 integrate-ai-9.9.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      763 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/backend_shim.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 13:27:42.258869 integrate-ai-9.9.1/integrate_ai/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/integrate_ai/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      657 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/integrate_ai/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21141 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/integrate_ai/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1081 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/integrate_ai/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2692 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/integrate_ai/sdk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5678 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/integrate_ai/server.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 13:27:42.258869 integrate-ai-9.9.1/integrate_ai/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/integrate_ai/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8304 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/integrate_ai/utils/docker_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1105 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/integrate_ai/utils/error_handling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      664 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/integrate_ai/utils/logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      859 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/integrate_ai/utils/path_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6025 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/integrate_ai/utils/rest_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2840 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/integrate_ai/utils/typer_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-29 13:27:42.258869 integrate-ai-9.9.1/integrate_ai.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1075 2024-04-29 13:27:42.000000 integrate-ai-9.9.1/integrate_ai.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2024-04-29 13:27:42.000000 integrate-ai-9.9.1/integrate_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-29 13:27:42.000000 integrate-ai-9.9.1/integrate_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-04-29 13:27:42.000000 integrate-ai-9.9.1/integrate_ai.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-29 13:27:42.000000 integrate-ai-9.9.1/integrate_ai.egg-info/namespace_packages.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-29 13:27:42.000000 integrate-ai-9.9.1/integrate_ai.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2024-04-29 13:27:42.000000 integrate-ai-9.9.1/integrate_ai.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-29 13:27:42.258869 integrate-ai-9.9.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1748 2024-04-29 13:27:41.000000 integrate-ai-9.9.1/setup.py
```

### Comparing `integrate-ai-9.9.0/PKG-INFO` & `integrate-ai-9.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integrate-ai
-Version: 9.9.0
+Version: 9.9.1
 Summary: integrate.ai
 Author: integrate.ai
 License: Copyright (C) 2022 integrate.ai, Inc. All rights reserved.
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
```

### Comparing `integrate-ai-9.9.0/backend_shim.py` & `integrate-ai-9.9.1/backend_shim.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.9.0/integrate_ai/cli.py` & `integrate-ai-9.9.1/integrate_ai/cli.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.9.0/integrate_ai/client.py` & `integrate-ai-9.9.1/integrate_ai/client.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.9.0/integrate_ai/main.py` & `integrate-ai-9.9.1/integrate_ai/main.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.9.0/integrate_ai/sdk.py` & `integrate-ai-9.9.1/integrate_ai/sdk.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.9.0/integrate_ai/server.py` & `integrate-ai-9.9.1/integrate_ai/server.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.9.0/integrate_ai/utils/docker_client.py` & `integrate-ai-9.9.1/integrate_ai/utils/docker_client.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.9.0/integrate_ai/utils/error_handling.py` & `integrate-ai-9.9.1/integrate_ai/utils/error_handling.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.9.0/integrate_ai/utils/logger.py` & `integrate-ai-9.9.1/integrate_ai/utils/logger.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.9.0/integrate_ai/utils/path_utils.py` & `integrate-ai-9.9.1/integrate_ai/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.9.0/integrate_ai/utils/rest_client.py` & `integrate-ai-9.9.1/integrate_ai/utils/rest_client.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.9.0/integrate_ai/utils/typer_utils.py` & `integrate-ai-9.9.1/integrate_ai/utils/typer_utils.py`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.9.0/integrate_ai.egg-info/PKG-INFO` & `integrate-ai-9.9.1/integrate_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: integrate-ai
-Version: 9.9.0
+Version: 9.9.1
 Summary: integrate.ai
 Author: integrate.ai
 License: Copyright (C) 2022 integrate.ai, Inc. All rights reserved.
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
```

### Comparing `integrate-ai-9.9.0/integrate_ai.egg-info/SOURCES.txt` & `integrate-ai-9.9.1/integrate_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `integrate-ai-9.9.0/setup.py` & `integrate-ai-9.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,9 +66,9 @@
     'package_data': {
     },
     'packages': (
         'integrate_ai',
         'integrate_ai.utils',
     ),
     'python_requires': '>=3.7.5',
-    'version': '9.9.0',
+    'version': '9.9.1',
 })
```

