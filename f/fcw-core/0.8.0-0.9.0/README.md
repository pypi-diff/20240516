# Comparing `tmp/fcw_core-0.8.0.tar.gz` & `tmp/fcw_core-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcw_core-0.8.0.tar", max compression
+gzip compressed data, was "fcw_core-0.9.0.tar", max compression
```

## Comparing `fcw_core-0.8.0.tar` & `fcw_core-0.9.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      320 2023-07-19 16:24:36.000000 fcw_core-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-03-15 17:29:23.000000 fcw_core-0.8.0/fcw_core/__init__.py
--rw-r--r--   0        0        0      916 2023-10-09 17:03:04.000000 fcw_core-0.8.0/fcw_core/detection.py
--rw-r--r--   0        0        0     8489 2023-10-09 15:36:03.000000 fcw_core-0.8.0/fcw_core/fcw_example.py
--rw-r--r--   0        0        0    13673 2023-11-28 14:23:41.000000 fcw_core-0.8.0/fcw_core/sort.py
--rw-r--r--   0        0        0     7626 2023-10-09 14:03:01.000000 fcw_core-0.8.0/fcw_core/vizualization.py
--rw-r--r--   0        0        0     4252 2023-11-28 14:39:53.000000 fcw_core-0.8.0/fcw_core/yolo_detector.py
--rw-r--r--   0        0        0     1106 2023-12-04 21:39:39.000000 fcw_core-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1626 1970-01-01 00:00:00.000000 fcw_core-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      320 2023-07-19 16:24:36.000000 fcw_core-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-15 17:29:23.000000 fcw_core-0.9.0/fcw_core/__init__.py
+-rw-r--r--   0        0        0      916 2023-10-09 17:03:04.000000 fcw_core-0.9.0/fcw_core/detection.py
+-rw-r--r--   0        0        0     8489 2023-10-09 15:36:03.000000 fcw_core-0.9.0/fcw_core/fcw_example.py
+-rw-r--r--   0        0        0    13673 2023-11-28 14:23:41.000000 fcw_core-0.9.0/fcw_core/sort.py
+-rw-r--r--   0        0        0     7626 2023-10-09 14:03:01.000000 fcw_core-0.9.0/fcw_core/vizualization.py
+-rw-r--r--   0        0        0     4252 2023-11-28 14:39:53.000000 fcw_core-0.9.0/fcw_core/yolo_detector.py
+-rw-r--r--   0        0        0     1106 2023-12-18 09:53:55.000000 fcw_core-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1627 1970-01-01 00:00:00.000000 fcw_core-0.9.0/PKG-INFO
```

### Comparing `fcw_core-0.8.0/fcw_core/detection.py` & `fcw_core-0.9.0/fcw_core/detection.py`

 * *Files identical despite different names*

### Comparing `fcw_core-0.8.0/fcw_core/fcw_example.py` & `fcw_core-0.9.0/fcw_core/fcw_example.py`

 * *Files identical despite different names*

### Comparing `fcw_core-0.8.0/fcw_core/sort.py` & `fcw_core-0.9.0/fcw_core/sort.py`

 * *Files identical despite different names*

### Comparing `fcw_core-0.8.0/fcw_core/vizualization.py` & `fcw_core-0.9.0/fcw_core/vizualization.py`

 * *Files identical despite different names*

### Comparing `fcw_core-0.8.0/fcw_core/yolo_detector.py` & `fcw_core-0.9.0/fcw_core/yolo_detector.py`

 * *Files identical despite different names*

### Comparing `fcw_core-0.8.0/pyproject.toml` & `fcw_core-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fcw-core"
-version = "0.8.0"
+version = "0.9.0"
 description = "Early collision warning Network Application for Transportation use case - core part"
 authors = ["Petr Kleparnik <pkleparnik@cognitechna.cz>", "Roman Juranek <rjuranek@cognitechna.cz>"]
 readme = "README.md"
 repository = "https://github.com/5G-ERA/CollisionWarningService"
 packages = [{include = "fcw_core"}]
 
 [tool.poetry.dependencies]
@@ -20,15 +20,15 @@
 more-itertools = ">=10.1.0"
 pandas = ">=2.0.3"
 requests = ">=2.31.0"
 psutil = ">=5.9.6"
 tqdm = ">=4.66.1"
 seaborn = ">=0.13.0"
 ultralytics = ">=8.0.220"
-fcw-core-utils = "^0.8.0"
+fcw-core-utils = "^0.9.0"
 matplotlib = ">=3.7.4"
 
 #pip3 install --upgrade --force-reinstall torch torchvision torchaudio --extra-index-url https://download.pytorch.org/whl/cu118
 
 [tool.poetry.scripts]
 fcw_example = "fcw_core.fcw_example:main"
```

### Comparing `fcw_core-0.8.0/PKG-INFO` & `fcw_core-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: fcw-core
-Version: 0.8.0
+Version: 0.9.0
 Summary: Early collision warning Network Application for Transportation use case - core part
 Home-page: https://github.com/5G-ERA/CollisionWarningService
 Author: Petr Kleparnik
 Author-email: pkleparnik@cognitechna.cz
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: fcw-core-utils (>=0.8.0,<0.9.0)
+Requires-Dist: fcw-core-utils (>=0.9.0,<0.10.0)
 Requires-Dist: filterpy (>=1.4.5)
 Requires-Dist: gitpython (>=3.1.40)
 Requires-Dist: matplotlib (>=3.7.4)
 Requires-Dist: more-itertools (>=10.1.0)
 Requires-Dist: opencv-python (>=4.8)
 Requires-Dist: pandas (>=2.0.3)
 Requires-Dist: psutil (>=5.9.6)
```

