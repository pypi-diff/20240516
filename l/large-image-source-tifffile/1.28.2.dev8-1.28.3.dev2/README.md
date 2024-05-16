# Comparing `tmp/large-image-source-tifffile-1.28.2.dev8.tar.gz` & `tmp/large-image-source-tifffile-1.28.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-tifffile-1.28.2.dev8.tar", last modified: Wed Apr 24 20:05:10 2024, max compression
+gzip compressed data, was "large-image-source-tifffile-1.28.3.dev2.tar", last modified: Thu May 16 16:50:36 2024, max compression
```

## Comparing `large-image-source-tifffile-1.28.2.dev8.tar` & `large-image-source-tifffile-1.28.3.dev2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:05:10.126591 large-image-source-tifffile-1.28.2.dev8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-24 20:05:09.000000 large-image-source-tifffile-1.28.2.dev8/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1058 2024-04-24 20:05:10.126591 large-image-source-tifffile-1.28.2.dev8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-24 20:05:09.000000 large-image-source-tifffile-1.28.2.dev8/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:05:10.122591 large-image-source-tifffile-1.28.2.dev8/large_image_source_tifffile/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25085 2024-04-24 19:59:45.000000 large-image-source-tifffile-1.28.2.dev8/large_image_source_tifffile/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-04-24 19:59:45.000000 large-image-source-tifffile-1.28.2.dev8/large_image_source_tifffile/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:05:10.126591 large-image-source-tifffile-1.28.2.dev8/large_image_source_tifffile.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1058 2024-04-24 20:05:10.000000 large-image-source-tifffile-1.28.2.dev8/large_image_source_tifffile.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2024-04-24 20:05:10.000000 large-image-source-tifffile-1.28.2.dev8/large_image_source_tifffile.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 20:05:10.000000 large-image-source-tifffile-1.28.2.dev8/large_image_source_tifffile.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2024-04-24 20:05:10.000000 large-image-source-tifffile-1.28.2.dev8/large_image_source_tifffile.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2024-04-24 20:05:10.000000 large-image-source-tifffile-1.28.2.dev8/large_image_source_tifffile.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-04-24 20:05:10.000000 large-image-source-tifffile-1.28.2.dev8/large_image_source_tifffile.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-24 19:59:45.000000 large-image-source-tifffile-1.28.2.dev8/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 20:05:10.126591 large-image-source-tifffile-1.28.2.dev8/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-04-24 19:59:45.000000 large-image-source-tifffile-1.28.2.dev8/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:50:36.014127 large-image-source-tifffile-1.28.3.dev2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-05-16 16:50:35.000000 large-image-source-tifffile-1.28.3.dev2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1058 2024-05-16 16:50:36.014127 large-image-source-tifffile-1.28.3.dev2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-05-16 16:50:35.000000 large-image-source-tifffile-1.28.3.dev2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:50:36.010127 large-image-source-tifffile-1.28.3.dev2/large_image_source_tifffile/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25001 2024-05-16 16:44:45.000000 large-image-source-tifffile-1.28.3.dev2/large_image_source_tifffile/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2024-05-16 16:44:45.000000 large-image-source-tifffile-1.28.3.dev2/large_image_source_tifffile/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:50:36.014127 large-image-source-tifffile-1.28.3.dev2/large_image_source_tifffile.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1058 2024-05-16 16:50:35.000000 large-image-source-tifffile-1.28.3.dev2/large_image_source_tifffile.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      435 2024-05-16 16:50:35.000000 large-image-source-tifffile-1.28.3.dev2/large_image_source_tifffile.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-16 16:50:35.000000 large-image-source-tifffile-1.28.3.dev2/large_image_source_tifffile.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2024-05-16 16:50:35.000000 large-image-source-tifffile-1.28.3.dev2/large_image_source_tifffile.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       98 2024-05-16 16:50:35.000000 large-image-source-tifffile-1.28.3.dev2/large_image_source_tifffile.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2024-05-16 16:50:35.000000 large-image-source-tifffile-1.28.3.dev2/large_image_source_tifffile.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-05-16 16:44:45.000000 large-image-source-tifffile-1.28.3.dev2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-16 16:50:36.014127 large-image-source-tifffile-1.28.3.dev2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-05-16 16:44:45.000000 large-image-source-tifffile-1.28.3.dev2/setup.py
```

### Comparing `large-image-source-tifffile-1.28.2.dev8/LICENSE` & `large-image-source-tifffile-1.28.3.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.28.2.dev8/PKG-INFO` & `large-image-source-tifffile-1.28.3.dev2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.28.2.dev8
+Version: 1.28.3.dev2
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,17 +13,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.2.dev8
+Requires-Dist: large-image>=1.28.3.dev2
 Requires-Dist: dask[array]
 Requires-Dist: tifffile[all]
 Requires-Dist: zarr
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.2.dev8; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.3.dev2; extra == "girder"
 
 A tifffile tilesource for large_image.
 
 See the large-image package for more details.
```

### Comparing `large-image-source-tifffile-1.28.2.dev8/README.rst` & `large-image-source-tifffile-1.28.3.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.28.2.dev8/large_image_source_tifffile/__init__.py` & `large-image-source-tifffile-1.28.3.dev2/large_image_source_tifffile/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -470,55 +470,54 @@
             frame = 0
         if hasattr(self, '_nonempty_levels_list') and frame in self._nonempty_levels_list:
             return self._nonempty_levels_list[frame]
         if len(self._series) > 1:
             sidx = frame // self._basis['P'][0]
         else:
             sidx = 0
-        series = self._tf.series[self._series[sidx]]
         nonempty = [None] * self.levels
         nonempty[self.levels - 1] = True
+        series = self._tf.series[self._series[sidx]]
+        za, hasgbs = self._getZarrArray(series, sidx)
         xidx = series.axes.index('X')
         yidx = series.axes.index('Y')
-        with self._zarrlock:
-            if sidx not in self._zarrcache:
-                if len(self._zarrcache) > 10:
-                    self._zarrcache = {}
-                za = zarr.open(series.aszarr(), mode='r')
-                hasgbs = hasattr(za[0], 'get_basic_selection')
-                self._zarrcache[sidx] = (za, hasgbs)
-            za, hasgbs = self._zarrcache[sidx]
         for ll in range(1, len(series.levels)):
             scale = round(math.log(max(za[0].shape[xidx] / za[ll].shape[xidx],
                                        za[0].shape[yidx] / za[ll].shape[yidx])) / math.log(2))
             if 0 < scale < self.levels:
                 nonempty[self.levels - 1 - int(scale)] = True
         if not hasattr(self, '_nonempty_levels_list'):
             self._nonempty_levels_list = {}
         self._nonempty_levels_list[frame] = nonempty
         return nonempty
 
+    def _getZarrArray(self, series, sidx):
+        with self._zarrlock:
+            if sidx not in self._zarrcache:
+                if len(self._zarrcache) > 10:
+                    self._zarrcache = {}
+                za = zarr.open(series.aszarr(), mode='r')
+                hasgbs = hasattr(za[0], 'get_basic_selection')
+                if not hasgbs and math.prod(series.shape) < 256 * 1024 ** 2:
+                    za = series.asarray()
+                self._zarrcache[sidx] = (za, hasgbs)
+            za, hasgbs = self._zarrcache[sidx]
+        return za, hasgbs
+
     @methodcache()
     def getTile(self, x, y, z, pilImageAllowed=False, numpyAllowed=False, **kwargs):
         frame = self._getFrame(**kwargs)
         self._xyzInRange(x, y, z, frame, self._framecount)
         x0, y0, x1, y1, step = self._xyzToCorners(x, y, z)
         if len(self._series) > 1:
             sidx = frame // self._basis['P'][0]
         else:
             sidx = 0
         series = self._tf.series[self._series[sidx]]
-        with self._zarrlock:
-            if sidx not in self._zarrcache:
-                if len(self._zarrcache) > 10:
-                    self._zarrcache = {}
-                za = zarr.open(series.aszarr(), mode='r')
-                hasgbs = hasattr(za[0], 'get_basic_selection')
-                self._zarrcache[sidx] = (za, hasgbs)
-            za, hasgbs = self._zarrcache[sidx]
+        za, hasgbs = self._getZarrArray(series, sidx)
         xidx = series.axes.index('X')
         yidx = series.axes.index('Y')
         if hasgbs:
             bza = za[0]
             # we could cache this
             for ll in range(len(series.levels) - 1, 0, -1):
                 scale = round(max(za[0].shape[xidx] / za[ll].shape[xidx],
```

### Comparing `large-image-source-tifffile-1.28.2.dev8/large_image_source_tifffile/girder_source.py` & `large-image-source-tifffile-1.28.3.dev2/large_image_source_tifffile/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-tifffile-1.28.2.dev8/large_image_source_tifffile.egg-info/PKG-INFO` & `large-image-source-tifffile-1.28.3.dev2/large_image_source_tifffile.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-tifffile
-Version: 1.28.2.dev8
+Version: 1.28.3.dev2
 Summary: A tifffile tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,17 +13,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 License-File: LICENSE
-Requires-Dist: large-image>=1.28.2.dev8
+Requires-Dist: large-image>=1.28.3.dev2
 Requires-Dist: dask[array]
 Requires-Dist: tifffile[all]
 Requires-Dist: zarr
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.2.dev8; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.3.dev2; extra == "girder"
 
 A tifffile tilesource for large_image.
 
 See the large-image package for more details.
```

### Comparing `large-image-source-tifffile-1.28.2.dev8/setup.py` & `large-image-source-tifffile-1.28.3.dev2/setup.py`

 * *Files identical despite different names*

