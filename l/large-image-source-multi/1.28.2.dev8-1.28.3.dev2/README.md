# Comparing `tmp/large-image-source-multi-1.28.2.dev8.tar.gz` & `tmp/large-image-source-multi-1.28.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-multi-1.28.2.dev8.tar", last modified: Wed Apr 24 20:03:07 2024, max compression
+gzip compressed data, was "large-image-source-multi-1.28.3.dev2.tar", last modified: Thu May 16 16:48:11 2024, max compression
```

## Comparing `large-image-source-multi-1.28.2.dev8.tar` & `large-image-source-multi-1.28.3.dev2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:03:07.486169 large-image-source-multi-1.28.2.dev8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-04-24 20:03:07.000000 large-image-source-multi-1.28.2.dev8/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2024-04-24 20:03:07.486169 large-image-source-multi-1.28.2.dev8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-04-24 20:03:07.000000 large-image-source-multi-1.28.2.dev8/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:03:07.482169 large-image-source-multi-1.28.2.dev8/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3381 2024-04-24 19:59:45.000000 large-image-source-multi-1.28.2.dev8/docs/specification.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:03:07.482169 large-image-source-multi-1.28.2.dev8/large_image_source_multi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    54069 2024-04-24 19:59:45.000000 large-image-source-multi-1.28.2.dev8/large_image_source_multi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2024-04-24 19:59:45.000000 large-image-source-multi-1.28.2.dev8/large_image_source_multi/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 20:03:07.482169 large-image-source-multi-1.28.2.dev8/large_image_source_multi.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2024-04-24 20:03:07.000000 large-image-source-multi-1.28.2.dev8/large_image_source_multi.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      434 2024-04-24 20:03:07.000000 large-image-source-multi-1.28.2.dev8/large_image_source_multi.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 20:03:07.000000 large-image-source-multi-1.28.2.dev8/large_image_source_multi.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-04-24 20:03:07.000000 large-image-source-multi-1.28.2.dev8/large_image_source_multi.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2024-04-24 20:03:07.000000 large-image-source-multi-1.28.2.dev8/large_image_source_multi.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-04-24 20:03:07.000000 large-image-source-multi-1.28.2.dev8/large_image_source_multi.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-04-24 19:59:45.000000 large-image-source-multi-1.28.2.dev8/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 20:03:07.486169 large-image-source-multi-1.28.2.dev8/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2569 2024-04-24 19:59:45.000000 large-image-source-multi-1.28.2.dev8/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:48:11.181909 large-image-source-multi-1.28.3.dev2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2024-05-16 16:48:10.000000 large-image-source-multi-1.28.3.dev2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2024-05-16 16:48:11.181909 large-image-source-multi-1.28.3.dev2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8782 2024-05-16 16:48:10.000000 large-image-source-multi-1.28.3.dev2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:48:11.177909 large-image-source-multi-1.28.3.dev2/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3381 2024-05-16 16:44:45.000000 large-image-source-multi-1.28.3.dev2/docs/specification.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:48:11.177909 large-image-source-multi-1.28.3.dev2/large_image_source_multi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    54305 2024-05-16 16:44:45.000000 large-image-source-multi-1.28.3.dev2/large_image_source_multi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2024-05-16 16:44:45.000000 large-image-source-multi-1.28.3.dev2/large_image_source_multi/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 16:48:11.181909 large-image-source-multi-1.28.3.dev2/large_image_source_multi.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1135 2024-05-16 16:48:11.000000 large-image-source-multi-1.28.3.dev2/large_image_source_multi.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      434 2024-05-16 16:48:11.000000 large-image-source-multi-1.28.3.dev2/large_image_source_multi.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-16 16:48:11.000000 large-image-source-multi-1.28.3.dev2/large_image_source_multi.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2024-05-16 16:48:11.000000 large-image-source-multi-1.28.3.dev2/large_image_source_multi.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2024-05-16 16:48:11.000000 large-image-source-multi-1.28.3.dev2/large_image_source_multi.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2024-05-16 16:48:11.000000 large-image-source-multi-1.28.3.dev2/large_image_source_multi.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       99 2024-05-16 16:44:45.000000 large-image-source-multi-1.28.3.dev2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-16 16:48:11.181909 large-image-source-multi-1.28.3.dev2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2569 2024-05-16 16:44:45.000000 large-image-source-multi-1.28.3.dev2/setup.py
```

### Comparing `large-image-source-multi-1.28.2.dev8/LICENSE` & `large-image-source-multi-1.28.3.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.28.2.dev8/PKG-INFO` & `large-image-source-multi-1.28.3.dev2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-multi
-Version: 1.28.2.dev8
+Version: 1.28.3.dev2
 Summary: A tilesource for large_image to composite other tile sources
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: jsonschema
-Requires-Dist: large-image>=1.28.2.dev8
+Requires-Dist: large-image>=1.28.3.dev2
 Requires-Dist: pyyaml
 Provides-Extra: all
 Requires-Dist: scikit-image; extra == "all"
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.2.dev8; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.3.dev2; extra == "girder"
 
 A tilesource for large_image to composite other tile sources
 
 See the large-image package for more details.
```

### Comparing `large-image-source-multi-1.28.2.dev8/README.rst` & `large-image-source-multi-1.28.3.dev2/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.28.2.dev8/docs/specification.rst` & `large-image-source-multi-1.28.3.dev2/docs/specification.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.28.2.dev8/large_image_source_multi/__init__.py` & `large-image-source-multi-1.28.3.dev2/large_image_source_multi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -824,27 +824,29 @@
         :param source: a dictionary with path, params, and possibly sourceName.
         :param params: a dictionary of parameters to pass to the open call.
         :returns: a tile source.
         """
         with self._lastOpenSourceLock:
             if (hasattr(self, '_lastOpenSource') and
                     self._lastOpenSource['source'] == source and
-                    self._lastOpenSource['params'] == params):
+                    (self._lastOpenSource['params'] == params or (
+                        params == {} and self._lastOpenSource['params'] is None))):
                 return self._lastOpenSource['ts']
         if not len(large_image.tilesource.AvailableTileSources):
             large_image.tilesource.loadTileSources()
         if ('sourceName' not in source or
                 source['sourceName'] not in large_image.tilesource.AvailableTileSources):
             openFunc = large_image.open
         else:
             openFunc = large_image.tilesource.AvailableTileSources[source['sourceName']]
         origParams = params
         if params is None:
             params = source.get('params', {})
         ts = openFunc(source['path'], **params)
+        source['sourceName'] = ts.name
         with self._lastOpenSourceLock:
             self._lastOpenSource = {
                 'source': source,
                 'params': origParams,
                 'ts': ts,
             }
         return ts
@@ -890,24 +892,24 @@
             result['bands'] = self._bands.copy()
         return result
 
     def getInternalMetadata(self, **kwargs):
         """
         Return additional known metadata about the tile source.  Data returned
         from this method is not guaranteed to be in any particular format or
-        have specific values.
+        have specific values.  Also, only the first 100 sources are used.
 
         :returns: a dictionary of data or None.
         """
         result = {
             'frames': copy.deepcopy(self._frames),
             'sources': copy.deepcopy(self._sources),
             'sourceFiles': [],
         }
-        for path in self._sourcePaths.values():
+        for path in list(self._sourcePaths.values())[:100]:
             source = self._sources[min(path['sourcenum'])]
             ts = self._openSource(source)
             result['sourceFiles'].append({
                 'path': source['path'],
                 'internal': ts.getInternalMetadata(),
             })
         return result
@@ -933,36 +935,36 @@
             base = np.zeros((0, 0, tile.shape[2]), dtype=tile.dtype)
         base, tile = _makeSameChannelDepth(base, tile)
         if base.shape[0] < tile.shape[0] + y:
             vfill = np.zeros(
                 (tile.shape[0] + y - base.shape[0], base.shape[1], base.shape[2]),
                 dtype=base.dtype)
             if base.shape[2] in {2, 4}:
-                vfill[:, :, -1] = fullAlphaValue(self.dtype)
+                vfill[:, :, -1] = fullAlphaValue(base.dtype)
             base = np.vstack((base, vfill))
         if base.shape[1] < tile.shape[1] + x:
             hfill = np.zeros(
                 (base.shape[0], tile.shape[1] + x - base.shape[1], base.shape[2]),
                 dtype=base.dtype)
             if base.shape[2] in {2, 4}:
-                hfill[:, :, -1] = fullAlphaValue(self.dtype)
+                hfill[:, :, -1] = fullAlphaValue(base.dtype)
             base = np.hstack((base, hfill))
         if base.flags.writeable is False:
             base = base.copy()
         if base.shape[2] in {2, 4}:
             baseA = base[y:y + tile.shape[0], x:x + tile.shape[1], -1].astype(
-                float) / fullAlphaValue(self.dtype)
-            tileA = tile[:, :, -1].astype(float) / fullAlphaValue(self.dtype)
+                float) / fullAlphaValue(base.dtype)
+            tileA = tile[:, :, -1].astype(float) / fullAlphaValue(tile.dtype)
             outA = tileA + baseA * (1 - tileA)
             base[y:y + tile.shape[0], x:x + tile.shape[1], :-1] = (
                 np.where(tileA[..., np.newaxis], tile[:, :, :-1], 0) +
                 base[y:y + tile.shape[0], x:x + tile.shape[1], :-1] * baseA[..., np.newaxis] *
                 (1 - tileA[..., np.newaxis])
             ) / np.where(outA[..., np.newaxis], outA[..., np.newaxis], 1)
-            base[y:y + tile.shape[0], x:x + tile.shape[1], -1] = outA * fullAlphaValue(self.dtype)
+            base[y:y + tile.shape[0], x:x + tile.shape[1], -1] = outA * fullAlphaValue(base.dtype)
         else:
             base[y:y + tile.shape[0], x:x + tile.shape[1], :] = tile
         return base
 
     def _getTransformedTile(self, ts, transform, corners, scale, frame, crop=None):
         """
         Determine where the target tile's corners are located on the source.
@@ -1094,20 +1096,20 @@
             coordinates.
         :param scale: power of 2 scale of the output; this is the number of
             pixels that are conceptually aggregated from the source for one
             output pixel.
         :returns: a numpy array of the tile.
         """
         source = self._sources[sourceEntry['sourcenum']]
-        ts = self._openSource(source, sourceEntry['kwargs'])
         # If tile is outside of bounding box, skip it
         bbox = source['bbox']
         if (corners[2][0] <= bbox['left'] or corners[0][0] >= bbox['right'] or
                 corners[2][1] <= bbox['top'] or corners[0][1] >= bbox['bottom']):
             return tile
+        ts = self._openSource(source, sourceEntry['kwargs'])
         transform = bbox.get('transform')
         x = y = 0
         # If there is no transform or the diagonals are positive and there is
         # no sheer and integer pixel alignment, use getRegion with an
         # appropriate size
         scaleX = transform[0][0] if transform is not None else 1
         scaleY = transform[1][1] if transform is not None else 1
@@ -1151,14 +1153,15 @@
                 region=region, output=output, frame=sourceEntry.get('frame', 0),
                 resample=None, format=TILE_FORMAT_NUMPY)
         else:
             sourceTile, x, y = self._getTransformedTile(
                 ts, transform, corners, scale, sourceEntry.get('frame', 0),
                 source.get('position', {}).get('crop'))
         if sourceTile is not None and all(dim > 0 for dim in sourceTile.shape):
+            sourceTile = sourceTile.astype(ts.dtype)
             tile = self._mergeTiles(tile, sourceTile, x, y)
         return tile
 
     @methodcache()
     def getTile(self, x, y, z, pilImageAllowed=False, numpyAllowed=False, **kwargs):
         frame = self._getFrame(**kwargs)
         self._xyzInRange(x, y, z, frame, len(self._frames) if hasattr(self, '_frames') else None)
```

### Comparing `large-image-source-multi-1.28.2.dev8/large_image_source_multi/girder_source.py` & `large-image-source-multi-1.28.3.dev2/large_image_source_multi/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.28.2.dev8/large_image_source_multi.egg-info/PKG-INFO` & `large-image-source-multi-1.28.3.dev2/large_image_source_multi.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-multi
-Version: 1.28.2.dev8
+Version: 1.28.3.dev2
 Summary: A tilesource for large_image to composite other tile sources
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,17 +14,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: jsonschema
-Requires-Dist: large-image>=1.28.2.dev8
+Requires-Dist: large-image>=1.28.3.dev2
 Requires-Dist: pyyaml
 Provides-Extra: all
 Requires-Dist: scikit-image; extra == "all"
 Provides-Extra: girder
-Requires-Dist: girder-large-image>=1.28.2.dev8; extra == "girder"
+Requires-Dist: girder-large-image>=1.28.3.dev2; extra == "girder"
 
 A tilesource for large_image to composite other tile sources
 
 See the large-image package for more details.
```

### Comparing `large-image-source-multi-1.28.2.dev8/setup.py` & `large-image-source-multi-1.28.3.dev2/setup.py`

 * *Files identical despite different names*

