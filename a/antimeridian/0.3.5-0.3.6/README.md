# Comparing `tmp/antimeridian-0.3.5.tar.gz` & `tmp/antimeridian-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antimeridian-0.3.5.tar", last modified: Sun May  5 13:13:46 2024, max compression
+gzip compressed data, was "antimeridian-0.3.6.tar", last modified: Thu May 16 13:40:55 2024, max compression
```

## Comparing `antimeridian-0.3.5.tar` & `antimeridian-0.3.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:13:46.101095 antimeridian-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-05 13:13:42.000000 antimeridian-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-05 13:13:46.101095 antimeridian-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-05 13:13:42.000000 antimeridian-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-05 13:13:42.000000 antimeridian-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-05 13:13:46.101095 antimeridian-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:13:46.093095 antimeridian-0.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:13:46.097095 antimeridian-0.3.5/src/antimeridian/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-05 13:13:42.000000 antimeridian-0.3.5/src/antimeridian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-05 13:13:42.000000 antimeridian-0.3.5/src/antimeridian/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    25165 2024-05-05 13:13:42.000000 antimeridian-0.3.5/src/antimeridian/_implementation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-05 13:13:42.000000 antimeridian-0.3.5/src/antimeridian/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:13:46.097095 antimeridian-0.3.5/src/antimeridian.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-05 13:13:46.000000 antimeridian-0.3.5/src/antimeridian.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-05 13:13:46.000000 antimeridian-0.3.5/src/antimeridian.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-05 13:13:46.000000 antimeridian-0.3.5/src/antimeridian.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-05 13:13:46.000000 antimeridian-0.3.5/src/antimeridian.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-05 13:13:46.000000 antimeridian-0.3.5/src/antimeridian.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-05 13:13:46.000000 antimeridian-0.3.5/src/antimeridian.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-05 13:13:46.097095 antimeridian-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-05 13:13:42.000000 antimeridian-0.3.5/tests/test_bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-05 13:13:42.000000 antimeridian-0.3.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-05 13:13:42.000000 antimeridian-0.3.5/tests/test_geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-05 13:13:42.000000 antimeridian-0.3.5/tests/test_line_string.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-05 13:13:42.000000 antimeridian-0.3.5/tests/test_multi_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4992 2024-05-05 13:13:42.000000 antimeridian-0.3.5/tests/test_polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-05 13:13:42.000000 antimeridian-0.3.5/tests/test_segment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:55.768808 antimeridian-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-16 13:40:49.000000 antimeridian-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-16 13:40:55.768808 antimeridian-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-16 13:40:49.000000 antimeridian-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-16 13:40:49.000000 antimeridian-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:40:55.768808 antimeridian-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:55.760809 antimeridian-0.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:55.764809 antimeridian-0.3.6/src/antimeridian/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 13:40:49.000000 antimeridian-0.3.6/src/antimeridian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-16 13:40:49.000000 antimeridian-0.3.6/src/antimeridian/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25325 2024-05-16 13:40:49.000000 antimeridian-0.3.6/src/antimeridian/_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:49.000000 antimeridian-0.3.6/src/antimeridian/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:55.764809 antimeridian-0.3.6/src/antimeridian.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-16 13:40:55.000000 antimeridian-0.3.6/src/antimeridian.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-16 13:40:55.000000 antimeridian-0.3.6/src/antimeridian.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:40:55.000000 antimeridian-0.3.6/src/antimeridian.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 13:40:55.000000 antimeridian-0.3.6/src/antimeridian.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-16 13:40:55.000000 antimeridian-0.3.6/src/antimeridian.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 13:40:55.000000 antimeridian-0.3.6/src/antimeridian.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:40:55.764809 antimeridian-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-16 13:40:49.000000 antimeridian-0.3.6/tests/test_bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-16 13:40:49.000000 antimeridian-0.3.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-16 13:40:49.000000 antimeridian-0.3.6/tests/test_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-16 13:40:49.000000 antimeridian-0.3.6/tests/test_line_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-16 13:40:49.000000 antimeridian-0.3.6/tests/test_multi_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-16 13:40:49.000000 antimeridian-0.3.6/tests/test_polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-16 13:40:49.000000 antimeridian-0.3.6/tests/test_segment.py
```

### Comparing `antimeridian-0.3.5/LICENSE` & `antimeridian-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.5/PKG-INFO` & `antimeridian-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.3.5
+Version: 0.3.6
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Documentation, https://antimeridian.readthedocs.io
 Project-URL: Github, https://github.com/gadomski/antimeridian
 Project-URL: Changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
```

### Comparing `antimeridian-0.3.5/README.md` & `antimeridian-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.5/pyproject.toml` & `antimeridian-0.3.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "antimeridian"
-version = "0.3.5"
+version = "0.3.6"
 authors = [{ name = "Pete Gadomski", email = "pete.gadomski@gmail.com" }]
 description = "Fix GeoJSON geometries that cross the antimeridian"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["geojson", "antimeridian", "shapely"]
 license = { text = "Apache-2.0" }
 classifiers = [
```

### Comparing `antimeridian-0.3.5/src/antimeridian/__init__.py` & `antimeridian-0.3.6/src/antimeridian/__init__.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.5/src/antimeridian/_cli.py` & `antimeridian-0.3.6/src/antimeridian/_cli.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.5/src/antimeridian/_implementation.py` & `antimeridian-0.3.6/src/antimeridian/_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -448,14 +448,18 @@
             ):
                 coords[i] = (180, point[1])
             else:
                 coords[i] = (-180, point[1])
         else:
             coords[i] = (((point[0] + 180) % 360) - 180, point[1])
             all_are_on_antimeridian = False
+        if len(point) > 2:
+            point_as_list = list(coords[i])
+            point_as_list.extend(point[2:])
+            coords[i] = tuple(point_as_list)
     if all_are_on_antimeridian:
         return original
     else:
         return coords
 
 
 def segment(coords: List[XY]) -> List[List[XY]]:
```

### Comparing `antimeridian-0.3.5/src/antimeridian.egg-info/PKG-INFO` & `antimeridian-0.3.6/src/antimeridian.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antimeridian
-Version: 0.3.5
+Version: 0.3.6
 Summary: Fix GeoJSON geometries that cross the antimeridian
 Author-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Documentation, https://antimeridian.readthedocs.io
 Project-URL: Github, https://github.com/gadomski/antimeridian
 Project-URL: Changelog, https://github.com/gadomski/antimeridian/blob/main/CHANGELOG.md
 Keywords: geojson,antimeridian,shapely
```

### Comparing `antimeridian-0.3.5/src/antimeridian.egg-info/SOURCES.txt` & `antimeridian-0.3.6/src/antimeridian.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.5/tests/test_cli.py` & `antimeridian-0.3.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.5/tests/test_geojson.py` & `antimeridian-0.3.6/tests/test_geojson.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.5/tests/test_line_string.py` & `antimeridian-0.3.6/tests/test_line_string.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.5/tests/test_multi_polygon.py` & `antimeridian-0.3.6/tests/test_multi_polygon.py`

 * *Files identical despite different names*

### Comparing `antimeridian-0.3.5/tests/test_polygon.py` & `antimeridian-0.3.6/tests/test_polygon.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,7 +153,14 @@
 def test_centroid_split_with_shift(read_input: Reader) -> None:
     input = read_input("split")
     input = shapely.affinity.translate(input, xoff=+1)
     input = antimeridian.fix_polygon(input)
     centroid = cast(Point, antimeridian.centroid(input))
     assert centroid.x == -179
     assert centroid.y == 45
+
+
+def test_z_coordinates() -> None:
+    # https://github.com/gadomski/antimeridian/issues/115
+    polygon = Polygon([[0, 0, 1], [10, 0, 2], [10, 10, 3], [0, 10, 4]])
+    fixed = antimeridian.fix_polygon(polygon)
+    assert fixed.has_z
```

