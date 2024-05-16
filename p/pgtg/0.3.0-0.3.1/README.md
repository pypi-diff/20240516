# Comparing `tmp/pgtg-0.3.0.tar.gz` & `tmp/pgtg-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgtg-0.3.0.tar", max compression
+gzip compressed data, was "pgtg-0.3.1.tar", max compression
```

## Comparing `pgtg-0.3.0.tar` & `pgtg-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      181 2024-04-16 12:03:53.875555 pgtg-0.3.0/pgtg/__init__.py
--rw-r--r--   0        0        0      886 2024-04-16 10:56:00.313150 pgtg-0.3.0/pgtg/constants.py
--rw-r--r--   0        0        0    36143 2024-04-16 10:56:00.317912 pgtg-0.3.0/pgtg/environment.py
--rw-r--r--   0        0        0    12292 2024-04-16 10:56:00.317912 pgtg-0.3.0/pgtg/evaluator.py
--rw-r--r--   0        0        0     5717 2024-04-16 10:56:00.317912 pgtg-0.3.0/pgtg/example_maps/tile_map_big_with_obstacles.json
--rw-r--r--   0        0        0     4494 2024-04-16 10:56:00.317912 pgtg-0.3.0/pgtg/example_maps/tile_map_big_without_obstacles.json
--rw-r--r--   0        0        0     1422 2024-04-16 10:56:00.317912 pgtg-0.3.0/pgtg/example_maps/tile_map_medium_with_obstacles.json
--rw-r--r--   0        0        0      716 2024-04-16 10:56:00.329316 pgtg-0.3.0/pgtg/example_maps/tile_map_medium_without_obstacles.json
--rw-r--r--   0        0        0      254 2024-04-16 10:56:00.329316 pgtg-0.3.0/pgtg/example_maps/tile_map_minimal_without_obstacles.json
--rw-r--r--   0        0        0    11392 2024-04-16 10:56:00.329316 pgtg-0.3.0/pgtg/graphic.py
--rw-r--r--   0        0        0     7203 2024-04-16 10:56:00.329316 pgtg-0.3.0/pgtg/map.py
--rw-r--r--   0        0        0    10757 2024-04-16 10:56:00.337905 pgtg-0.3.0/pgtg/map_generator.py
--rw-r--r--   0        0        0    85827 2024-04-16 10:56:00.339505 pgtg-0.3.0/pgtg/map_tiles_data.py
--rw-r--r--   0        0        0    10474 2024-04-16 10:56:00.343927 pgtg-0.3.0/pgtg/parser.py
--rw-r--r--   0        0        0    12838 2024-04-16 10:56:00.346550 pgtg-0.3.0/pgtg/pics/beginning.png
--rw-r--r--   0        0        0    13575 2024-04-16 10:56:00.347808 pgtg-0.3.0/pgtg/pics/road_break.png
--rw-r--r--   0        0        0     8739 2024-04-16 10:56:00.349111 pgtg-0.3.0/pgtg/pics/road_left.png
--rw-r--r--   0        0        0      336 2024-04-16 10:56:00.349111 pgtg-0.3.0/pgtg/pics/test.png
--rw-r--r--   0        0        0     1061 2024-04-16 12:02:35.829177 pgtg-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4889 2024-04-16 10:58:57.187753 pgtg-0.3.0/README.md
--rw-r--r--   0        0        0     5685 1970-01-01 00:00:00.000000 pgtg-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      181 2024-05-16 13:41:26.099825 pgtg-0.3.1/pgtg/__init__.py
+-rw-r--r--   0        0        0      886 2024-05-16 12:34:01.263211 pgtg-0.3.1/pgtg/constants.py
+-rw-r--r--   0        0        0    36143 2024-05-16 12:34:01.267431 pgtg-0.3.1/pgtg/environment.py
+-rw-r--r--   0        0        0    12292 2024-05-16 12:34:01.268837 pgtg-0.3.1/pgtg/evaluator.py
+-rw-r--r--   0        0        0     5717 2024-05-16 12:34:01.270707 pgtg-0.3.1/pgtg/example_maps/tile_map_big_with_obstacles.json
+-rw-r--r--   0        0        0     4494 2024-05-16 12:34:01.271635 pgtg-0.3.1/pgtg/example_maps/tile_map_big_without_obstacles.json
+-rw-r--r--   0        0        0     1422 2024-05-16 12:34:01.271635 pgtg-0.3.1/pgtg/example_maps/tile_map_medium_with_obstacles.json
+-rw-r--r--   0        0        0      716 2024-05-16 12:34:01.271635 pgtg-0.3.1/pgtg/example_maps/tile_map_medium_without_obstacles.json
+-rw-r--r--   0        0        0      254 2024-05-16 12:34:01.271635 pgtg-0.3.1/pgtg/example_maps/tile_map_minimal_without_obstacles.json
+-rw-r--r--   0        0        0    11392 2024-05-16 12:34:01.271635 pgtg-0.3.1/pgtg/graphic.py
+-rw-r--r--   0        0        0     7213 2024-05-16 13:44:20.301944 pgtg-0.3.1/pgtg/map.py
+-rw-r--r--   0        0        0    11000 2024-05-16 13:43:39.691507 pgtg-0.3.1/pgtg/map_generator.py
+-rw-r--r--   0        0        0    85827 2024-05-16 12:34:01.284197 pgtg-0.3.1/pgtg/map_tiles_data.py
+-rw-r--r--   0        0        0    10474 2024-05-16 12:34:01.285398 pgtg-0.3.1/pgtg/parser.py
+-rw-r--r--   0        0        0    12838 2024-05-16 12:34:01.286970 pgtg-0.3.1/pgtg/pics/beginning.png
+-rw-r--r--   0        0        0    13575 2024-05-16 12:34:01.288023 pgtg-0.3.1/pgtg/pics/road_break.png
+-rw-r--r--   0        0        0     8739 2024-05-16 12:34:01.289095 pgtg-0.3.1/pgtg/pics/road_left.png
+-rw-r--r--   0        0        0      336 2024-05-16 12:34:01.289932 pgtg-0.3.1/pgtg/pics/test.png
+-rw-r--r--   0        0        0     1061 2024-05-16 13:40:43.353214 pgtg-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4961 2024-05-16 13:48:29.243917 pgtg-0.3.1/README.md
+-rw-r--r--   0        0        0     5755 1970-01-01 00:00:00.000000 pgtg-0.3.1/PKG-INFO
```

### Comparing `pgtg-0.3.0/pgtg/constants.py` & `pgtg-0.3.1/pgtg/constants.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.3.0/pgtg/environment.py` & `pgtg-0.3.1/pgtg/environment.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.3.0/pgtg/evaluator.py` & `pgtg-0.3.1/pgtg/evaluator.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.3.0/pgtg/example_maps/tile_map_big_with_obstacles.json` & `pgtg-0.3.1/pgtg/example_maps/tile_map_big_with_obstacles.json`

 * *Files identical despite different names*

### Comparing `pgtg-0.3.0/pgtg/example_maps/tile_map_big_without_obstacles.json` & `pgtg-0.3.1/pgtg/example_maps/tile_map_big_without_obstacles.json`

 * *Files identical despite different names*

### Comparing `pgtg-0.3.0/pgtg/example_maps/tile_map_medium_with_obstacles.json` & `pgtg-0.3.1/pgtg/example_maps/tile_map_medium_with_obstacles.json`

 * *Files identical despite different names*

### Comparing `pgtg-0.3.0/pgtg/example_maps/tile_map_medium_without_obstacles.json` & `pgtg-0.3.1/pgtg/example_maps/tile_map_medium_without_obstacles.json`

 * *Files identical despite different names*

### Comparing `pgtg-0.3.0/pgtg/graphic.py` & `pgtg-0.3.1/pgtg/graphic.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.3.0/pgtg/map.py` & `pgtg-0.3.1/pgtg/map.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,8 +174,8 @@
             path (String): path to the file the map should be saved in.
         """
 
         if not path.endswith(".json"):
             path += ".json"
 
         with open(path, "w", encoding="utf-8") as f:
-            json.dump(self.map_plan, f, ensure_ascii=False, indent=4)
+            json.dump(self.map_plan.to_dict(), f, ensure_ascii=False, indent=4)
```

### Comparing `pgtg-0.3.0/pgtg/map_generator.py` & `pgtg-0.3.1/pgtg/map_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,23 @@
 
         return cls(
             width=data["width"],
             height=data["height"],
             tiles=data["map"],
         )
 
+    def to_dict(self) -> dict[str, Any]:
+        """Returns a dictionary representation of the object."""
+
+        return {
+            "width": self.width,
+            "height": self.height,
+            "map": self.tiles,
+        }
+
 
 def generate_map(
     width: int,
     height: int,
     percentage_of_connections: float,
     rng,
     *,
```

### Comparing `pgtg-0.3.0/pgtg/map_tiles_data.py` & `pgtg-0.3.1/pgtg/map_tiles_data.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.3.0/pgtg/parser.py` & `pgtg-0.3.1/pgtg/parser.py`

 * *Files identical despite different names*

### Comparing `pgtg-0.3.0/pgtg/pics/beginning.png` & `pgtg-0.3.1/pgtg/pics/beginning.png`

 * *Files identical despite different names*

### Comparing `pgtg-0.3.0/pgtg/pics/road_break.png` & `pgtg-0.3.1/pgtg/pics/road_break.png`

 * *Files identical despite different names*

### Comparing `pgtg-0.3.0/pgtg/pics/road_left.png` & `pgtg-0.3.1/pgtg/pics/road_left.png`

 * *Files identical despite different names*

### Comparing `pgtg-0.3.0/pyproject.toml` & `pgtg-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   "Operating System :: OS Independent",
   "Intended Audience :: Science/Research",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 description = "Python simulation of a driving challange. Compatible with the Gymnasium API standard."
 name = "pgtg"
 readme = "README.md"
-version = "0.3.0"
+version = "0.3.1"
 
 [tool.poetry.dependencies]
 Pillow = "^8.4.0"
 matplotlib = "^3.4.3"
 numpy = "^1.26.3"
 python = ">=3.10,<3.11"
 jupyter = "^1.0.0"
```

### Comparing `pgtg-0.3.0/README.md` & `pgtg-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -82,8 +82,10 @@
 ### v0.2.0
 - Sand now slows down with a customizable probability (default 20%) instead of always.
 - Bump environment version to v1 because the changes impact reproducibility with earlier versions.
 ### v0.3.0
 - The x and y coordinates of observations are no longer swapped. This was the case for historical reasons but serves no use any more.
 - Adds the option to use a sliding observation window of variable size.
 - Adds the option to use the direction of the next subgoal as a additional observation.
-- Bump environment version to v2 because the changes impact reproducibility with earlier versions.
+- Bump environment version to v2 because the changes impact reproducibility with earlier versions.
+### v0.3.0
+- Fix bug that made it impossible to save a map as a file.
```

### Comparing `pgtg-0.3.0/PKG-INFO` & `pgtg-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgtg
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python simulation of a driving challange. Compatible with the Gymnasium API standard.
 Author: Timo P. Gros
 Author-email: timopgros@cs.uni-saarland.de
 Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
@@ -105,7 +105,9 @@
 - Sand now slows down with a customizable probability (default 20%) instead of always.
 - Bump environment version to v1 because the changes impact reproducibility with earlier versions.
 ### v0.3.0
 - The x and y coordinates of observations are no longer swapped. This was the case for historical reasons but serves no use any more.
 - Adds the option to use a sliding observation window of variable size.
 - Adds the option to use the direction of the next subgoal as a additional observation.
 - Bump environment version to v2 because the changes impact reproducibility with earlier versions.
+### v0.3.0
+- Fix bug that made it impossible to save a map as a file.
```

