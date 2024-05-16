# Comparing `tmp/fcw_core_utils-0.8.0.tar.gz` & `tmp/fcw_core_utils-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fcw_core_utils-0.8.0.tar", max compression
+gzip compressed data, was "fcw_core_utils-0.9.0.tar", max compression
```

## Comparing `fcw_core_utils-0.8.0.tar` & `fcw_core_utils-0.9.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      419 2023-07-19 16:16:49.000000 fcw_core_utils-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-03-15 17:29:23.000000 fcw_core_utils-0.8.0/fcw_core_utils/__init__.py
--rw-r--r--   0        0        0     8767 2023-11-28 14:23:41.000000 fcw_core_utils-0.8.0/fcw_core_utils/collision.py
--rw-r--r--   0        0        0     5772 2023-11-28 14:40:23.000000 fcw_core_utils-0.8.0/fcw_core_utils/geometry.py
--rw-r--r--   0        0        0     6051 2023-06-28 11:32:52.000000 fcw_core_utils-0.8.0/fcw_core_utils/rate_timer.py
--rw-r--r--   0        0        0      627 2023-12-04 20:59:30.000000 fcw_core_utils-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 fcw_core_utils-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      419 2023-07-19 16:16:49.000000 fcw_core_utils-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-03-15 17:29:23.000000 fcw_core_utils-0.9.0/fcw_core_utils/__init__.py
+-rw-r--r--   0        0        0     8767 2023-11-28 14:23:41.000000 fcw_core_utils-0.9.0/fcw_core_utils/collision.py
+-rw-r--r--   0        0        0     5772 2023-11-28 14:40:23.000000 fcw_core_utils-0.9.0/fcw_core_utils/geometry.py
+-rw-r--r--   0        0        0     6051 2023-06-28 11:32:52.000000 fcw_core_utils-0.9.0/fcw_core_utils/rate_timer.py
+-rw-r--r--   0        0        0      627 2023-12-18 09:48:27.000000 fcw_core_utils-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 fcw_core_utils-0.9.0/PKG-INFO
```

### Comparing `fcw_core_utils-0.8.0/fcw_core_utils/collision.py` & `fcw_core_utils-0.9.0/fcw_core_utils/collision.py`

 * *Files identical despite different names*

### Comparing `fcw_core_utils-0.8.0/fcw_core_utils/geometry.py` & `fcw_core_utils-0.9.0/fcw_core_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `fcw_core_utils-0.8.0/fcw_core_utils/rate_timer.py` & `fcw_core_utils-0.9.0/fcw_core_utils/rate_timer.py`

 * *Files identical despite different names*

### Comparing `fcw_core_utils-0.8.0/pyproject.toml` & `fcw_core_utils-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "fcw-core-utils"
-version = "0.8.0"
+version = "0.9.0"
 description = "Early collision warning Network Application for Transportation use case - core utils part"
 authors = ["Petr Kleparnik <pkleparnik@cognitechna.cz>", "Roman Juranek <rjuranek@cognitechna.cz>"]
 readme = "README.md"
 repository = "https://github.com/5G-ERA/CollisionWarningService"
 packages = [{include = "fcw_core_utils"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-opencv-python = ">=4.6"
+opencv-python = ">=4.8"
 filterpy = ">=1.4.5"
 shapely = ">=2.0.2"
 matplotlib = ">=3.7.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fcw_core_utils-0.8.0/PKG-INFO` & `fcw_core_utils-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: fcw-core-utils
-Version: 0.8.0
+Version: 0.9.0
 Summary: Early collision warning Network Application for Transportation use case - core utils part
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
 Requires-Dist: filterpy (>=1.4.5)
 Requires-Dist: matplotlib (>=3.7.4)
-Requires-Dist: opencv-python (>=4.6)
+Requires-Dist: opencv-python (>=4.8)
 Requires-Dist: shapely (>=2.0.2)
 Project-URL: Repository, https://github.com/5G-ERA/CollisionWarningService
 Description-Content-Type: text/markdown
 
 # Forward Collision Warning - core utils part
 
 Early collision warning Network Application for Transportation use case - core utils part.
```

