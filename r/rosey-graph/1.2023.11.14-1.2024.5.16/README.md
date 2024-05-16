# Comparing `tmp/rosey-graph-1.2023.11.14.tar.gz` & `tmp/rosey-graph-1.2024.5.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosey-graph-1.2023.11.14.tar", last modified: Tue Nov 14 14:57:25 2023, max compression
+gzip compressed data, was "rosey-graph-1.2024.5.16.tar", last modified: Thu May 16 18:29:09 2024, max compression
```

## Comparing `rosey-graph-1.2023.11.14.tar` & `rosey-graph-1.2024.5.16.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 sar       (1000) sar       (1000)        0 2023-11-14 14:57:25.309086 rosey-graph-1.2023.11.14/
--rw-r--r--   0 sar       (1000) sar       (1000)       42 2023-11-14 14:50:58.000000 rosey-graph-1.2023.11.14/MANIFEST.in
--rw-r--r--   0 sar       (1000) sar       (1000)      559 2023-11-14 14:57:25.309086 rosey-graph-1.2023.11.14/PKG-INFO
--rw-r--r--   0 sar       (1000) sar       (1000)       84 2023-11-14 14:50:58.000000 rosey-graph-1.2023.11.14/README.md
--rw-r--r--   0 sar       (1000) sar       (1000)        0 2023-11-14 14:50:58.000000 rosey-graph-1.2023.11.14/requirements.txt
-drwxr-xr-x   0 sar       (1000) sar       (1000)        0 2023-11-14 14:57:25.309086 rosey-graph-1.2023.11.14/rosey_graph/
--rw-r--r--   0 sar       (1000) sar       (1000)    16869 2023-11-14 14:55:30.000000 rosey-graph-1.2023.11.14/rosey_graph/__init__.py
-drwxr-xr-x   0 sar       (1000) sar       (1000)        0 2023-11-14 14:57:25.309086 rosey-graph-1.2023.11.14/rosey_graph.egg-info/
--rw-r--r--   0 sar       (1000) sar       (1000)      559 2023-11-14 14:57:25.000000 rosey-graph-1.2023.11.14/rosey_graph.egg-info/PKG-INFO
--rw-r--r--   0 sar       (1000) sar       (1000)      283 2023-11-14 14:57:25.000000 rosey-graph-1.2023.11.14/rosey_graph.egg-info/SOURCES.txt
--rw-r--r--   0 sar       (1000) sar       (1000)        1 2023-11-14 14:57:25.000000 rosey-graph-1.2023.11.14/rosey_graph.egg-info/dependency_links.txt
--rw-r--r--   0 sar       (1000) sar       (1000)        1 2023-11-14 14:52:06.000000 rosey-graph-1.2023.11.14/rosey_graph.egg-info/not-zip-safe
--rw-r--r--   0 sar       (1000) sar       (1000)       18 2023-11-14 14:57:25.000000 rosey-graph-1.2023.11.14/rosey_graph.egg-info/top_level.txt
--rw-r--r--   0 sar       (1000) sar       (1000)       38 2023-11-14 14:57:25.309086 rosey-graph-1.2023.11.14/setup.cfg
--rw-r--r--   0 sar       (1000) sar       (1000)     1334 2023-11-14 14:50:58.000000 rosey-graph-1.2023.11.14/setup.py
-drwxr-xr-x   0 sar       (1000) sar       (1000)        0 2023-11-14 14:57:25.309086 rosey-graph-1.2023.11.14/tests/
--rw-r--r--   0 sar       (1000) sar       (1000)       14 2023-11-14 14:50:58.000000 rosey-graph-1.2023.11.14/tests/__init__.py
--rw-r--r--   0 sar       (1000) sar       (1000)     2101 2023-11-14 14:55:30.000000 rosey-graph-1.2023.11.14/tests/test_plots.py
+drwxr-xr-x   0 srose      (502) staff       (20)        0 2024-05-16 18:29:09.077107 rosey-graph-1.2024.5.16/
+-rw-r--r--   0 srose      (502) staff       (20)       42 2024-02-01 14:47:01.000000 rosey-graph-1.2024.5.16/MANIFEST.in
+-rw-r--r--   0 srose      (502) staff       (20)      635 2024-05-16 18:29:09.076788 rosey-graph-1.2024.5.16/PKG-INFO
+-rw-r--r--   0 srose      (502) staff       (20)       84 2024-02-01 14:47:01.000000 rosey-graph-1.2024.5.16/README.md
+-rw-r--r--   0 srose      (502) staff       (20)       31 2024-05-16 17:56:52.000000 rosey-graph-1.2024.5.16/requirements.txt
+drwxr-xr-x   0 srose      (502) staff       (20)        0 2024-05-16 18:29:09.073514 rosey-graph-1.2024.5.16/rosey_graph/
+-rw-r--r--   0 srose      (502) staff       (20)    16869 2024-05-16 18:04:12.000000 rosey-graph-1.2024.5.16/rosey_graph/__init__.py
+-rw-r--r--   0 srose      (502) staff       (20)      250 2024-05-16 18:01:31.000000 rosey-graph-1.2024.5.16/rosey_graph/notebook.py
+drwxr-xr-x   0 srose      (502) staff       (20)        0 2024-05-16 18:29:09.075370 rosey-graph-1.2024.5.16/rosey_graph.egg-info/
+-rw-r--r--   0 srose      (502) staff       (20)      635 2024-05-16 18:29:09.000000 rosey-graph-1.2024.5.16/rosey_graph.egg-info/PKG-INFO
+-rw-r--r--   0 srose      (502) staff       (20)      351 2024-05-16 18:29:09.000000 rosey-graph-1.2024.5.16/rosey_graph.egg-info/SOURCES.txt
+-rw-r--r--   0 srose      (502) staff       (20)        1 2024-05-16 18:29:09.000000 rosey-graph-1.2024.5.16/rosey_graph.egg-info/dependency_links.txt
+-rw-r--r--   0 srose      (502) staff       (20)        1 2024-02-01 15:04:09.000000 rosey-graph-1.2024.5.16/rosey_graph.egg-info/not-zip-safe
+-rw-r--r--   0 srose      (502) staff       (20)       32 2024-05-16 18:29:09.000000 rosey-graph-1.2024.5.16/rosey_graph.egg-info/requires.txt
+-rw-r--r--   0 srose      (502) staff       (20)       18 2024-05-16 18:29:09.000000 rosey-graph-1.2024.5.16/rosey_graph.egg-info/top_level.txt
+-rw-r--r--   0 srose      (502) staff       (20)       38 2024-05-16 18:29:09.077175 rosey-graph-1.2024.5.16/setup.cfg
+-rw-r--r--   0 srose      (502) staff       (20)     1334 2024-02-01 14:47:01.000000 rosey-graph-1.2024.5.16/setup.py
+drwxr-xr-x   0 srose      (502) staff       (20)        0 2024-05-16 18:29:09.076050 rosey-graph-1.2024.5.16/tests/
+-rw-r--r--   0 srose      (502) staff       (20)       14 2024-02-01 14:47:01.000000 rosey-graph-1.2024.5.16/tests/__init__.py
+-rw-r--r--   0 srose      (502) staff       (20)     2101 2024-02-01 14:47:01.000000 rosey-graph-1.2024.5.16/tests/test_plots.py
```

### Comparing `rosey-graph-1.2023.11.14/PKG-INFO` & `rosey-graph-1.2024.5.16/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: rosey-graph
-Version: 1.2023.11.14
+Version: 1.2024.5.16
 Summary: Making certain routine graphs more quickly
 Home-page: https://github.com/arose13/rosey-graph
 Author: Stephen Rose
 Author-email: me@stephenro.se
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: scikit-learn
 
 # Rosey (Graphing)
 
 Uses `matplotlib`, `seaborn` and `scikit-learn` only as needed.
```

### Comparing `rosey-graph-1.2023.11.14/rosey_graph/__init__.py` & `rosey-graph-1.2024.5.16/rosey_graph/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.2023.11.14'  # Major.YYYY.MM.DD
+__version__ = '1.2024.05.16'  # Major.YYYY.MM.DD
 
 import matplotlib.pyplot as graph
 import numpy as np
 
 colors_538 = [
     '#30a2da',
     '#fc4f30',
```

### Comparing `rosey-graph-1.2023.11.14/rosey_graph.egg-info/PKG-INFO` & `rosey-graph-1.2024.5.16/rosey_graph.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.1
 Name: rosey-graph
-Version: 1.2023.11.14
+Version: 1.2024.5.16
 Summary: Making certain routine graphs more quickly
 Home-page: https://github.com/arose13/rosey-graph
 Author: Stephen Rose
 Author-email: me@stephenro.se
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: scikit-learn
 
 # Rosey (Graphing)
 
 Uses `matplotlib`, `seaborn` and `scikit-learn` only as needed.
```

### Comparing `rosey-graph-1.2023.11.14/setup.py` & `rosey-graph-1.2024.5.16/setup.py`

 * *Files identical despite different names*

### Comparing `rosey-graph-1.2023.11.14/tests/test_plots.py` & `rosey-graph-1.2024.5.16/tests/test_plots.py`

 * *Files identical despite different names*

