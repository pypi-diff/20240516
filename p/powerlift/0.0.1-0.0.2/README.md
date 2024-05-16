# Comparing `tmp/powerlift-0.0.1.tar.gz` & `tmp/powerlift-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "powerlift-0.0.1.tar", last modified: Thu Jun 30 10:22:27 2022, max compression
+gzip compressed data, was "powerlift-0.0.2.tar", last modified: Thu Jun 30 11:24:13 2022, max compression
```

## Comparing `powerlift-0.0.1.tar` & `powerlift-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 10:22:27.133878 powerlift-0.0.1/
--rw-r--r--   0 sajenkin   (501) staff       (20)     1161 2022-06-13 07:19:19.000000 powerlift-0.0.1/LICENSE
--rw-r--r--   0 sajenkin   (501) staff       (20)     4685 2022-06-30 10:22:27.133417 powerlift-0.0.1/PKG-INFO
--rw-r--r--   0 sajenkin   (501) staff       (20)     4015 2022-06-13 07:16:53.000000 powerlift-0.0.1/README.md
--rw-r--r--   0 sajenkin   (501) staff       (20)      103 2022-01-07 00:10:01.000000 powerlift-0.0.1/pyproject.toml
--rw-r--r--   0 sajenkin   (501) staff       (20)       38 2022-06-30 10:22:27.133998 powerlift-0.0.1/setup.cfg
--rw-r--r--   0 sajenkin   (501) staff       (20)     1712 2022-06-07 05:38:25.000000 powerlift-0.0.1/setup.py
-drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 10:22:27.101801 powerlift-0.0.1/src/
-drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 10:22:27.103419 powerlift-0.0.1/src/powerlift/
-drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 10:22:27.116185 powerlift-0.0.1/src/powerlift/bench/
--rw-r--r--   0 sajenkin   (501) staff       (20)      637 2022-06-13 07:07:37.000000 powerlift-0.0.1/src/powerlift/bench/__init__.py
--rw-r--r--   0 sajenkin   (501) staff       (20)    11096 2022-06-13 06:50:14.000000 powerlift-0.0.1/src/powerlift/bench/experiment.py
--rw-r--r--   0 sajenkin   (501) staff       (20)    27650 2022-06-13 07:11:19.000000 powerlift-0.0.1/src/powerlift/bench/store.py
-drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 10:22:27.119796 powerlift-0.0.1/src/powerlift/db/
--rw-r--r--   0 sajenkin   (501) staff       (20)      856 2022-06-13 06:08:05.000000 powerlift-0.0.1/src/powerlift/db/__init__.py
--rw-r--r--   0 sajenkin   (501) staff       (20)     1072 2022-06-13 06:08:44.000000 powerlift-0.0.1/src/powerlift/db/actions.py
--rw-r--r--   0 sajenkin   (501) staff       (20)     6839 2022-06-08 06:51:32.000000 powerlift-0.0.1/src/powerlift/db/schema.py
-drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 10:22:27.128834 powerlift-0.0.1/src/powerlift/executors/
--rw-r--r--   0 sajenkin   (501) staff       (20)      233 2022-06-13 06:38:29.000000 powerlift-0.0.1/src/powerlift/executors/__init__.py
--rw-r--r--   0 sajenkin   (501) staff       (20)     7639 2022-06-13 06:48:45.000000 powerlift-0.0.1/src/powerlift/executors/azure_ci.py
--rw-r--r--   0 sajenkin   (501) staff       (20)     2274 2022-06-10 06:21:05.000000 powerlift-0.0.1/src/powerlift/executors/base.py
--rw-r--r--   0 sajenkin   (501) staff       (20)     3041 2022-06-13 06:44:40.000000 powerlift-0.0.1/src/powerlift/executors/docker.py
--rw-r--r--   0 sajenkin   (501) staff       (20)     2838 2022-06-13 06:48:27.000000 powerlift-0.0.1/src/powerlift/executors/localmachine.py
-drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 10:22:27.131608 powerlift-0.0.1/src/powerlift/measures/
--rw-r--r--   0 sajenkin   (501) staff       (20)      136 2022-06-13 07:07:37.000000 powerlift-0.0.1/src/powerlift/measures/__init__.py
--rw-r--r--   0 sajenkin   (501) staff       (20)     4501 2022-06-13 07:07:37.000000 powerlift-0.0.1/src/powerlift/measures/task_measures.py
-drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 10:22:27.132588 powerlift-0.0.1/src/powerlift/run/
--rw-r--r--   0 sajenkin   (501) staff       (20)     2472 2022-06-13 06:50:57.000000 powerlift-0.0.1/src/powerlift/run/__main__.py
-drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 10:22:27.112873 powerlift-0.0.1/src/powerlift.egg-info/
--rw-r--r--   0 sajenkin   (501) staff       (20)     4685 2022-06-30 10:22:26.000000 powerlift-0.0.1/src/powerlift.egg-info/PKG-INFO
--rw-r--r--   0 sajenkin   (501) staff       (20)      687 2022-06-30 10:22:27.000000 powerlift-0.0.1/src/powerlift.egg-info/SOURCES.txt
--rw-r--r--   0 sajenkin   (501) staff       (20)        1 2022-06-30 10:22:26.000000 powerlift-0.0.1/src/powerlift.egg-info/dependency_links.txt
--rw-r--r--   0 sajenkin   (501) staff       (20)      345 2022-06-30 10:22:26.000000 powerlift-0.0.1/src/powerlift.egg-info/requires.txt
--rw-r--r--   0 sajenkin   (501) staff       (20)       10 2022-06-30 10:22:26.000000 powerlift-0.0.1/src/powerlift.egg-info/top_level.txt
+drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 11:24:13.538724 powerlift-0.0.2/
+-rw-r--r--   0 sajenkin   (501) staff       (20)     1161 2022-06-13 07:19:19.000000 powerlift-0.0.2/LICENSE
+-rw-r--r--   0 sajenkin   (501) staff       (20)     4750 2022-06-30 11:24:13.538129 powerlift-0.0.2/PKG-INFO
+-rw-r--r--   0 sajenkin   (501) staff       (20)     4081 2022-06-30 11:21:31.000000 powerlift-0.0.2/README.md
+-rw-r--r--   0 sajenkin   (501) staff       (20)      103 2022-01-07 00:10:01.000000 powerlift-0.0.2/pyproject.toml
+-rw-r--r--   0 sajenkin   (501) staff       (20)       38 2022-06-30 11:24:13.538908 powerlift-0.0.2/setup.cfg
+-rw-r--r--   0 sajenkin   (501) staff       (20)     1709 2022-06-30 11:19:53.000000 powerlift-0.0.2/setup.py
+drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 11:24:13.401805 powerlift-0.0.2/src/
+drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 11:24:13.403676 powerlift-0.0.2/src/powerlift/
+drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 11:24:13.453453 powerlift-0.0.2/src/powerlift/bench/
+-rw-r--r--   0 sajenkin   (501) staff       (20)      637 2022-06-13 07:07:37.000000 powerlift-0.0.2/src/powerlift/bench/__init__.py
+-rw-r--r--   0 sajenkin   (501) staff       (20)    11096 2022-06-13 06:50:14.000000 powerlift-0.0.2/src/powerlift/bench/experiment.py
+-rw-r--r--   0 sajenkin   (501) staff       (20)    27650 2022-06-13 07:11:19.000000 powerlift-0.0.2/src/powerlift/bench/store.py
+drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 11:24:13.470072 powerlift-0.0.2/src/powerlift/db/
+-rw-r--r--   0 sajenkin   (501) staff       (20)      856 2022-06-13 06:08:05.000000 powerlift-0.0.2/src/powerlift/db/__init__.py
+-rw-r--r--   0 sajenkin   (501) staff       (20)     1072 2022-06-13 06:08:44.000000 powerlift-0.0.2/src/powerlift/db/actions.py
+-rw-r--r--   0 sajenkin   (501) staff       (20)     6839 2022-06-08 06:51:32.000000 powerlift-0.0.2/src/powerlift/db/schema.py
+drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 11:24:13.508845 powerlift-0.0.2/src/powerlift/executors/
+-rw-r--r--   0 sajenkin   (501) staff       (20)      233 2022-06-13 06:38:29.000000 powerlift-0.0.2/src/powerlift/executors/__init__.py
+-rw-r--r--   0 sajenkin   (501) staff       (20)     7639 2022-06-13 06:48:45.000000 powerlift-0.0.2/src/powerlift/executors/azure_ci.py
+-rw-r--r--   0 sajenkin   (501) staff       (20)     2274 2022-06-10 06:21:05.000000 powerlift-0.0.2/src/powerlift/executors/base.py
+-rw-r--r--   0 sajenkin   (501) staff       (20)     3041 2022-06-13 06:44:40.000000 powerlift-0.0.2/src/powerlift/executors/docker.py
+-rw-r--r--   0 sajenkin   (501) staff       (20)     2838 2022-06-13 06:48:27.000000 powerlift-0.0.2/src/powerlift/executors/localmachine.py
+drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 11:24:13.529401 powerlift-0.0.2/src/powerlift/measures/
+-rw-r--r--   0 sajenkin   (501) staff       (20)      136 2022-06-13 07:07:37.000000 powerlift-0.0.2/src/powerlift/measures/__init__.py
+-rw-r--r--   0 sajenkin   (501) staff       (20)     4501 2022-06-13 07:07:37.000000 powerlift-0.0.2/src/powerlift/measures/task_measures.py
+drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 11:24:13.536863 powerlift-0.0.2/src/powerlift/run/
+-rw-r--r--   0 sajenkin   (501) staff       (20)     2472 2022-06-13 06:50:57.000000 powerlift-0.0.2/src/powerlift/run/__main__.py
+drwxr-xr-x   0 sajenkin   (501) staff       (20)        0 2022-06-30 11:24:13.424000 powerlift-0.0.2/src/powerlift.egg-info/
+-rw-r--r--   0 sajenkin   (501) staff       (20)     4750 2022-06-30 11:24:12.000000 powerlift-0.0.2/src/powerlift.egg-info/PKG-INFO
+-rw-r--r--   0 sajenkin   (501) staff       (20)      687 2022-06-30 11:24:13.000000 powerlift-0.0.2/src/powerlift.egg-info/SOURCES.txt
+-rw-r--r--   0 sajenkin   (501) staff       (20)        1 2022-06-30 11:24:12.000000 powerlift-0.0.2/src/powerlift.egg-info/dependency_links.txt
+-rw-r--r--   0 sajenkin   (501) staff       (20)      342 2022-06-30 11:24:13.000000 powerlift-0.0.2/src/powerlift.egg-info/requires.txt
+-rw-r--r--   0 sajenkin   (501) staff       (20)       10 2022-06-30 11:24:13.000000 powerlift-0.0.2/src/powerlift.egg-info/top_level.txt
```

### Comparing `powerlift-0.0.1/LICENSE` & `powerlift-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `powerlift-0.0.1/PKG-INFO` & `powerlift-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerlift
-Version: 0.0.1
+Version: 0.0.2
 Summary: Interactive Benchmarking for Machine Learning.
 Home-page: https://github.com/interpretml/interpret
 Author: InterpretML Team
 Author-email: interpret@microsoft.com
 Project-URL: Bug Tracker, https://github.com/interpretml/interpret/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -122,7 +122,12 @@
     mem_size_gb=2,
     raise_exception=True,
 )
 experiment = Experiment(store, "SVM vs RF")
 executor = experiment.run(benchmark, trials, timeout=10, executor=executor)
 executor.join()
 ```
+
+## Install
+`pip install powerlift`
+
+That's it, go get 'em boss.
```

### Comparing `powerlift-0.0.1/README.md` & `powerlift-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -100,8 +100,13 @@
     num_cores=1,
     mem_size_gb=2,
     raise_exception=True,
 )
 experiment = Experiment(store, "SVM vs RF")
 executor = experiment.run(benchmark, trials, timeout=10, executor=executor)
 executor.join()
-```
+```
+
+## Install
+`pip install powerlift`
+
+That's it, go get 'em boss.
```

### Comparing `powerlift-0.0.1/setup.py` & `powerlift-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="powerlift",
-    version="0.0.1",
+    version="0.0.2",
     author="InterpretML Team",
     author_email="interpret@microsoft.com",
     description="Interactive Benchmarking for Machine Learning.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/interpretml/interpret",
     project_urls={
@@ -35,15 +35,15 @@
     ],
     extras_require={
         "datasets": [
             "pmlb >=1.0",
             "openml >=0.12",
         ],
         "docker": [
-            "aiodocker",
+            "docker",
         ],
         "postgres": [
             "psycopg2 >=2.9",
         ],
         "mssql": [
             "pyodbc",
         ],
```

### Comparing `powerlift-0.0.1/src/powerlift/bench/__init__.py` & `powerlift-0.0.2/src/powerlift/bench/__init__.py`

 * *Files identical despite different names*

### Comparing `powerlift-0.0.1/src/powerlift/bench/experiment.py` & `powerlift-0.0.2/src/powerlift/bench/experiment.py`

 * *Files identical despite different names*

### Comparing `powerlift-0.0.1/src/powerlift/bench/store.py` & `powerlift-0.0.2/src/powerlift/bench/store.py`

 * *Files identical despite different names*

### Comparing `powerlift-0.0.1/src/powerlift/db/__init__.py` & `powerlift-0.0.2/src/powerlift/db/__init__.py`

 * *Files identical despite different names*

### Comparing `powerlift-0.0.1/src/powerlift/db/actions.py` & `powerlift-0.0.2/src/powerlift/db/actions.py`

 * *Files identical despite different names*

### Comparing `powerlift-0.0.1/src/powerlift/db/schema.py` & `powerlift-0.0.2/src/powerlift/db/schema.py`

 * *Files identical despite different names*

### Comparing `powerlift-0.0.1/src/powerlift/executors/azure_ci.py` & `powerlift-0.0.2/src/powerlift/executors/azure_ci.py`

 * *Files identical despite different names*

### Comparing `powerlift-0.0.1/src/powerlift/executors/base.py` & `powerlift-0.0.2/src/powerlift/executors/base.py`

 * *Files identical despite different names*

### Comparing `powerlift-0.0.1/src/powerlift/executors/docker.py` & `powerlift-0.0.2/src/powerlift/executors/docker.py`

 * *Files identical despite different names*

### Comparing `powerlift-0.0.1/src/powerlift/executors/localmachine.py` & `powerlift-0.0.2/src/powerlift/executors/localmachine.py`

 * *Files identical despite different names*

### Comparing `powerlift-0.0.1/src/powerlift/measures/task_measures.py` & `powerlift-0.0.2/src/powerlift/measures/task_measures.py`

 * *Files identical despite different names*

### Comparing `powerlift-0.0.1/src/powerlift/run/__main__.py` & `powerlift-0.0.2/src/powerlift/run/__main__.py`

 * *Files identical despite different names*

### Comparing `powerlift-0.0.1/src/powerlift.egg-info/PKG-INFO` & `powerlift-0.0.2/src/powerlift.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerlift
-Version: 0.0.1
+Version: 0.0.2
 Summary: Interactive Benchmarking for Machine Learning.
 Home-page: https://github.com/interpretml/interpret
 Author: InterpretML Team
 Author-email: interpret@microsoft.com
 Project-URL: Bug Tracker, https://github.com/interpretml/interpret/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -122,7 +122,12 @@
     mem_size_gb=2,
     raise_exception=True,
 )
 experiment = Experiment(store, "SVM vs RF")
 executor = experiment.run(benchmark, trials, timeout=10, executor=executor)
 executor.join()
 ```
+
+## Install
+`pip install powerlift`
+
+That's it, go get 'em boss.
```

### Comparing `powerlift-0.0.1/src/powerlift.egg-info/SOURCES.txt` & `powerlift-0.0.2/src/powerlift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

