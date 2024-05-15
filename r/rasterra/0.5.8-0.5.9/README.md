# Comparing `tmp/rasterra-0.5.8.tar.gz` & `tmp/rasterra-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasterra-0.5.8.tar", max compression
+gzip compressed data, was "rasterra-0.5.9.tar", max compression
```

## Comparing `rasterra-0.5.8.tar` & `rasterra-0.5.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1521 2024-05-10 17:15:11.334050 rasterra-0.5.8/LICENSE
--rw-r--r--   0        0        0     2687 2024-05-10 17:15:11.334050 rasterra-0.5.8/README.md
--rw-r--r--   0        0        0     3546 2024-05-10 17:15:11.334050 rasterra-0.5.8/pyproject.toml
--rw-r--r--   0        0        0      152 2024-05-10 17:15:11.334050 rasterra-0.5.8/src/rasterra/__init__.py
--rw-r--r--   0        0        0    19196 2024-05-10 17:15:11.338050 rasterra-0.5.8/src/rasterra/_array.py
--rw-r--r--   0        0        0     3267 2024-05-10 17:15:11.338050 rasterra-0.5.8/src/rasterra/_features.py
--rw-r--r--   0        0        0     1657 2024-05-10 17:15:11.338050 rasterra-0.5.8/src/rasterra/_io.py
--rw-r--r--   0        0        0     3795 2024-05-10 17:15:11.338050 rasterra-0.5.8/src/rasterra/_plotting.py
--rw-r--r--   0        0        0      828 2024-05-10 17:15:11.338050 rasterra-0.5.8/src/rasterra/_typing.py
--rw-r--r--   0        0        0        0 2024-05-10 17:15:11.338050 rasterra-0.5.8/src/rasterra/py.typed
--rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 rasterra-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1521 2024-05-10 21:23:38.084601 rasterra-0.5.9/LICENSE
+-rw-r--r--   0        0        0     2687 2024-05-10 21:23:38.088601 rasterra-0.5.9/README.md
+-rw-r--r--   0        0        0     3546 2024-05-10 21:23:38.088601 rasterra-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0      152 2024-05-10 21:23:38.088601 rasterra-0.5.9/src/rasterra/__init__.py
+-rw-r--r--   0        0        0    19228 2024-05-10 21:23:38.088601 rasterra-0.5.9/src/rasterra/_array.py
+-rw-r--r--   0        0        0     3267 2024-05-10 21:23:38.088601 rasterra-0.5.9/src/rasterra/_features.py
+-rw-r--r--   0        0        0     1717 2024-05-10 21:23:38.088601 rasterra-0.5.9/src/rasterra/_io.py
+-rw-r--r--   0        0        0     3795 2024-05-10 21:23:38.088601 rasterra-0.5.9/src/rasterra/_plotting.py
+-rw-r--r--   0        0        0      828 2024-05-10 21:23:38.088601 rasterra-0.5.9/src/rasterra/_typing.py
+-rw-r--r--   0        0        0        0 2024-05-10 21:23:38.088601 rasterra-0.5.9/src/rasterra/py.typed
+-rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 rasterra-0.5.9/PKG-INFO
```

### Comparing `rasterra-0.5.8/LICENSE` & `rasterra-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rasterra-0.5.8/README.md` & `rasterra-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `rasterra-0.5.8/pyproject.toml` & `rasterra-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rasterra"
-version = "0.5.8"
+version = "0.5.9"
 description = "A sleek, object-oriented interface designed for intuitive raster data manipulation in Python."
 authors = [
     "James Collins <collijk1@gmail.com>",
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `rasterra-0.5.8/src/rasterra/_array.py` & `rasterra-0.5.9/src/rasterra/_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -541,19 +541,19 @@
         out += f"extent        : {bounds} (xmin, xmax, ymin, ymax)\n"
         out += f"crs           : {self.crs}\n"
         out += f"no_data_value : {self._no_data_value}\n"
         out += f"size          : {self.nbytes / 1024 ** 2:.2f} MB\n"
         out += f"dtype         : {self._ndarray.dtype}\n"
         return out
 
-    def to_file(self, path: FilePath) -> None:
+    def to_file(self, path: FilePath, **kwargs: typing.Any) -> None:
         """Write the raster to a file."""
         from rasterra._io import write_raster
 
-        write_raster(self, path)
+        write_raster(self, path, **kwargs)
 
     def to_gdf(self) -> gpd.GeoDataFrame:
         return to_gdf(self)
 
     @property
     def plot(self) -> Plotter:
         return Plotter(self._ndarray, self.no_data_mask, self.transform)
```

### Comparing `rasterra-0.5.8/src/rasterra/_features.py` & `rasterra-0.5.9/src/rasterra/_features.py`

 * *Files identical despite different names*

### Comparing `rasterra-0.5.8/src/rasterra/_io.py` & `rasterra-0.5.9/src/rasterra/_io.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections.abc import Sequence
+from typing import Any
 
 import rasterio
 from rasterio.merge import merge
 
 from rasterra._array import RasterArray
 from rasterra._typing import FilePath
 
@@ -23,25 +24,27 @@
             msg = "Only single-band rasters are supported"
             raise NotImplementedError(msg)
 
 
 def write_raster(
     raster: RasterArray,
     path: FilePath,
+    **kwargs: Any,
 ) -> None:
     """Write a raster to a file."""
     meta = {
         "driver": "GTiff",
         "height": raster.shape[0],
         "width": raster.shape[1],
         "count": 1,
         "dtype": raster.dtype,
         "crs": raster.crs,
         "transform": raster.transform,
         "nodata": raster.no_data_value,
+        **kwargs,
     }
 
     with rasterio.open(path, "w", **meta) as f:
         f.write(raster.to_numpy(), 1)
 
 
 def load_mf_raster(paths: Sequence[FilePath]) -> RasterArray:
```

### Comparing `rasterra-0.5.8/src/rasterra/_plotting.py` & `rasterra-0.5.9/src/rasterra/_plotting.py`

 * *Files identical despite different names*

### Comparing `rasterra-0.5.8/src/rasterra/_typing.py` & `rasterra-0.5.9/src/rasterra/_typing.py`

 * *Files identical despite different names*

### Comparing `rasterra-0.5.8/PKG-INFO` & `rasterra-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasterra
-Version: 0.5.8
+Version: 0.5.9
 Summary: A sleek, object-oriented interface designed for intuitive raster data manipulation in Python.
 Home-page: https://collijk.github.io/rasterra
 License: BSD-3-Clause
 Author: James Collins
 Author-email: collijk1@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
```

