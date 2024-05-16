# Comparing `tmp/digitalhub-0.4.0b4.tar.gz` & `tmp/digitalhub-0.4.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub-0.4.0b4.tar", last modified: Fri May  3 12:51:47 2024, max compression
+gzip compressed data, was "digitalhub-0.4.0b8.tar", last modified: Tue May 14 09:32:59 2024, max compression
```

## Comparing `digitalhub-0.4.0b4.tar` & `digitalhub-0.4.0b8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:51:47.882927 digitalhub-0.4.0b4/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub-0.4.0b4/LICENSE.txt
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14790 2024-05-03 12:51:47.882927 digitalhub-0.4.0b4/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      510 2024-04-23 09:36:04.000000 digitalhub-0.4.0b4/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:51:47.878927 digitalhub-0.4.0b4/digitalhub/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2225 2024-05-03 12:46:16.000000 digitalhub-0.4.0b4/digitalhub/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:51:47.878927 digitalhub-0.4.0b4/digitalhub.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14790 2024-05-03 12:51:47.000000 digitalhub-0.4.0b4/digitalhub.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      421 2024-05-03 12:51:47.000000 digitalhub-0.4.0b4/digitalhub.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-03 12:51:47.000000 digitalhub-0.4.0b4/digitalhub.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      166 2024-05-03 12:51:47.000000 digitalhub-0.4.0b4/digitalhub.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       35 2024-05-03 12:51:47.000000 digitalhub-0.4.0b4/digitalhub.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1547 2024-05-03 12:31:18.000000 digitalhub-0.4.0b4/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-03 12:51:47.882927 digitalhub-0.4.0b4/setup.cfg
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-03 12:51:47.878927 digitalhub-0.4.0b4/test/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2511 2024-04-09 11:48:32.000000 digitalhub-0.4.0b4/test/test_crud_artifacts.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2504 2024-04-09 11:48:32.000000 digitalhub-0.4.0b4/test/test_crud_dataitems.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2769 2024-04-09 11:48:34.000000 digitalhub-0.4.0b4/test/test_crud_functions.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2220 2024-04-09 11:48:34.000000 digitalhub-0.4.0b4/test/test_crud_runs.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2111 2024-04-09 11:48:32.000000 digitalhub-0.4.0b4/test/test_crud_tasks.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1269 2024-03-22 13:56:51.000000 digitalhub-0.4.0b4/test/test_imports.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1086 2024-03-25 07:51:29.000000 digitalhub-0.4.0b4/test/testkfp.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      619 2024-03-25 10:18:34.000000 digitalhub-0.4.0b4/test/testkfp_pipeline.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 09:32:59.421637 digitalhub-0.4.0b8/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)    11585 2023-08-23 08:29:57.000000 digitalhub-0.4.0b8/LICENSE.txt
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14790 2024-05-14 09:32:59.421637 digitalhub-0.4.0b8/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      510 2024-04-23 09:36:04.000000 digitalhub-0.4.0b8/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 09:32:59.413637 digitalhub-0.4.0b8/digitalhub/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2218 2024-05-13 12:39:44.000000 digitalhub-0.4.0b8/digitalhub/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 09:32:59.417637 digitalhub-0.4.0b8/digitalhub.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)    14790 2024-05-14 09:32:59.000000 digitalhub-0.4.0b8/digitalhub.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      421 2024-05-14 09:32:59.000000 digitalhub-0.4.0b8/digitalhub.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-14 09:32:59.000000 digitalhub-0.4.0b8/digitalhub.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      166 2024-05-14 09:32:59.000000 digitalhub-0.4.0b8/digitalhub.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       35 2024-05-14 09:32:59.000000 digitalhub-0.4.0b8/digitalhub.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1547 2024-05-13 12:41:00.000000 digitalhub-0.4.0b8/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-14 09:32:59.421637 digitalhub-0.4.0b8/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-14 09:32:59.417637 digitalhub-0.4.0b8/test/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2511 2024-05-09 07:33:31.000000 digitalhub-0.4.0b8/test/test_crud_artifacts.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2504 2024-05-09 07:33:31.000000 digitalhub-0.4.0b8/test/test_crud_dataitems.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2769 2024-05-09 07:33:31.000000 digitalhub-0.4.0b8/test/test_crud_functions.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2220 2024-05-09 07:33:31.000000 digitalhub-0.4.0b8/test/test_crud_runs.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2111 2024-05-09 07:33:31.000000 digitalhub-0.4.0b8/test/test_crud_tasks.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1269 2024-03-22 13:56:51.000000 digitalhub-0.4.0b8/test/test_imports.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1086 2024-03-25 07:51:29.000000 digitalhub-0.4.0b8/test/testkfp.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      619 2024-03-25 10:18:34.000000 digitalhub-0.4.0b8/test/testkfp_pipeline.py
```

### Comparing `digitalhub-0.4.0b4/LICENSE.txt` & `digitalhub-0.4.0b8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b4/PKG-INFO` & `digitalhub-0.4.0b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub
-Version: 0.4.0b4
+Version: 0.4.0b8
 Summary: Python SDK for DigitalHub
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub-0.4.0b4/digitalhub/__init__.py` & `digitalhub-0.4.0b8/digitalhub/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     update_function,
     update_project,
     update_run,
     update_secret,
     update_task,
     update_workflow,
 )
-from digitalhub_core.registry.import_utils import register_layer_entities, register_runtimes_entities
+from digitalhub_core.registry.utils import register_layer_entities, register_runtimes_entities
 
 _PROJECT_IMPORTED = False
 
 if not _PROJECT_IMPORTED:
     try:
         from digitalhub_data import (
             delete_dataitem,
```

### Comparing `digitalhub-0.4.0b4/digitalhub.egg-info/PKG-INFO` & `digitalhub-0.4.0b8/digitalhub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: digitalhub
-Version: 0.4.0b4
+Version: 0.4.0b8
 Summary: Python SDK for DigitalHub
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 License:                               Apache License
                                 Version 2.0, January 2004
                              http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `digitalhub-0.4.0b4/pyproject.toml` & `digitalhub-0.4.0b8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub"
-version = "0.4.0b4"
+version = "0.4.0b8"
 description = "Python SDK for DigitalHub"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -48,15 +48,15 @@
 [tool.ruff.extend-per-file-ignores]
 "__init__.py" = ["F401"]
 
 [tool.ruff.pydocstyle]
 convention = "numpy"
 
 [tool.bumpver]
-current_version = "0.4.0b4"
+current_version = "0.4.0b8"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `digitalhub-0.4.0b4/test/test_crud_artifacts.py` & `digitalhub-0.4.0b8/test/test_crud_artifacts.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b4/test/test_crud_dataitems.py` & `digitalhub-0.4.0b8/test/test_crud_dataitems.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b4/test/test_crud_functions.py` & `digitalhub-0.4.0b8/test/test_crud_functions.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b4/test/test_crud_runs.py` & `digitalhub-0.4.0b8/test/test_crud_runs.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b4/test/test_crud_tasks.py` & `digitalhub-0.4.0b8/test/test_crud_tasks.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b4/test/test_imports.py` & `digitalhub-0.4.0b8/test/test_imports.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b4/test/testkfp.py` & `digitalhub-0.4.0b8/test/testkfp.py`

 * *Files identical despite different names*

### Comparing `digitalhub-0.4.0b4/test/testkfp_pipeline.py` & `digitalhub-0.4.0b8/test/testkfp_pipeline.py`

 * *Files identical despite different names*

