# Comparing `tmp/delaunay_triangulation_and_its_dual_2d-0.1.4.tar.gz` & `tmp/delaunay_triangulation_and_its_dual_2d-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delaunay_triangulation_and_its_dual_2d-0.1.4.tar", last modified: Thu May  9 14:54:50 2024, max compression
+gzip compressed data, was "delaunay_triangulation_and_its_dual_2d-0.1.5.tar", last modified: Thu May 16 11:26:35 2024, max compression
```

## Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4.tar` & `delaunay_triangulation_and_its_dual_2d-0.1.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 14:54:50.834186 delaunay_triangulation_and_its_dual_2d-0.1.4/
--rw-rw-rw-   0        0        0     3318 2024-05-05 03:33:40.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/.gitignore
--rw-rw-rw-   0        0        0     1086 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     6089 2024-05-09 14:54:50.833281 delaunay_triangulation_and_its_dual_2d-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4084 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 14:54:50.815259 delaunay_triangulation_and_its_dual_2d-0.1.4/assets/
--rw-rw-rw-   0        0        0    66443 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/assets/time_to_compute_voronoi_tessellation.png
-drwxrwxrwx   0        0        0        0 2024-05-09 14:54:50.821259 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/
--rw-rw-rw-   0        0        0       32 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/__init__.py
--rw-rw-rw-   0        0        0      427 2024-05-09 14:54:50.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/_version.py
--rw-rw-rw-   0        0        0    22442 2024-05-09 14:53:59.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/delaunay.py
--rw-rw-rw-   0        0        0       58 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:54:50.827258 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/geometry/
--rw-rw-rw-   0        0        0      142 2024-05-09 13:57:34.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/geometry/__init__.py
--rw-rw-rw-   0        0        0     3932 2024-05-09 14:43:59.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/geometry/bounding_box_2d.py
--rw-rw-rw-   0        0        0      220 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/geometry/centroid.py
--rw-rw-rw-   0        0        0     2758 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:54:50.828259 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/util/
--rw-rw-rw-   0        0        0       65 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/util/__init__.py
--rw-rw-rw-   0        0        0      865 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:54:50.832282 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d.egg-info/
--rw-rw-rw-   0        0        0     6089 2024-05-09 14:54:50.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1142 2024-05-09 14:54:50.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 14:54:50.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-05-09 14:54:50.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d.egg-info/requires.txt
--rw-rw-rw-   0        0        0       39 2024-05-09 14:54:50.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1319 2024-05-05 04:11:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 14:54:50.834186 delaunay_triangulation_and_its_dual_2d-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-09 14:54:50.811256 delaunay_triangulation_and_its_dual_2d-0.1.4/tests/
-drwxrwxrwx   0        0        0        0 2024-05-09 14:54:50.831282 delaunay_triangulation_and_its_dual_2d-0.1.4/tests/delaunay/
--rw-rw-rw-   0        0        0        0 2024-05-09 14:43:59.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/tests/delaunay/__init__.py
--rw-rw-rw-   0        0        0     2484 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/tests/delaunay/performance.py
--rw-rw-rw-   0        0        0      481 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/tests/delaunay/profiling.py
--rw-rw-rw-   0        0        0     6180 2024-05-05 03:48:22.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/tests/delaunay/test_all.py
--rw-rw-rw-   0        0        0     2650 2024-05-09 14:53:58.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/tests/delaunay/try.py
-drwxrwxrwx   0        0        0        0 2024-05-09 14:54:50.831282 delaunay_triangulation_and_its_dual_2d-0.1.4/tests/geometry/
--rw-rw-rw-   0        0        0        0 2024-05-09 14:43:59.000000 delaunay_triangulation_and_its_dual_2d-0.1.4/tests/geometry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.464269 delaunay_triangulation_and_its_dual_2d-0.1.5/
+-rw-rw-rw-   0        0        0     3318 2024-05-05 03:33:40.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/.gitignore
+-rw-rw-rw-   0        0        0     1086 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     6089 2024-05-16 11:26:35.464269 delaunay_triangulation_and_its_dual_2d-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4084 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.437375 delaunay_triangulation_and_its_dual_2d-0.1.5/assets/
+-rw-rw-rw-   0        0        0    66443 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/assets/time_to_compute_voronoi_tessellation.png
+drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.446690 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/
+-rw-rw-rw-   0        0        0       32 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/__init__.py
+-rw-rw-rw-   0        0        0      427 2024-05-16 11:26:35.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/_version.py
+-rw-rw-rw-   0        0        0    22218 2024-05-16 11:01:21.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/delaunay.py
+-rw-rw-rw-   0        0        0       58 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.457695 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/geometry/
+-rw-rw-rw-   0        0        0      142 2024-05-09 13:57:34.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/geometry/__init__.py
+-rw-rw-rw-   0        0        0     3912 2024-05-16 11:23:28.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/geometry/bounding_box_2d.py
+-rw-rw-rw-   0        0        0      220 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/geometry/centroid.py
+-rw-rw-rw-   0        0        0     2758 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.458263 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/util/
+-rw-rw-rw-   0        0        0       65 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/util/__init__.py
+-rw-rw-rw-   0        0        0      865 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.463267 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/
+-rw-rw-rw-   0        0        0     6089 2024-05-16 11:26:35.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1142 2024-05-16 11:26:35.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:26:35.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-05-16 11:26:35.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       39 2024-05-16 11:26:35.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1319 2024-05-05 04:11:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:26:35.465267 delaunay_triangulation_and_its_dual_2d-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.434376 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/
+drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.462268 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/
+-rw-rw-rw-   0        0        0        0 2024-05-09 14:43:59.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/__init__.py
+-rw-rw-rw-   0        0        0     2484 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/performance.py
+-rw-rw-rw-   0        0        0      481 2024-05-05 03:29:42.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/profiling.py
+-rw-rw-rw-   0        0        0     6180 2024-05-05 03:48:22.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/test_all.py
+-rw-rw-rw-   0        0        0     3478 2024-05-16 11:22:58.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/try.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:26:35.462268 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/geometry/
+-rw-rw-rw-   0        0        0        0 2024-05-09 14:43:59.000000 delaunay_triangulation_and_its_dual_2d-0.1.5/tests/geometry/__init__.py
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4/.gitignore` & `delaunay_triangulation_and_its_dual_2d-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4/LICENSE` & `delaunay_triangulation_and_its_dual_2d-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4/PKG-INFO` & `delaunay_triangulation_and_its_dual_2d-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay-triangulation-and-its-dual-2d
-Version: 0.1.4
+Version: 0.1.5
 License: MIT License
         
         Copyright (c) 2024 M.H. Luk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4/README.md` & `delaunay_triangulation_and_its_dual_2d-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4/assets/time_to_compute_voronoi_tessellation.png` & `delaunay_triangulation_and_its_dual_2d-0.1.5/assets/time_to_compute_voronoi_tessellation.png`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/delaunay.py` & `delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/delaunay.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,55 @@
 from abc import ABC, abstractmethod
 from collections import defaultdict, deque
 import logging
 from typing import Literal
 
-import matplotlib.pyplot as plt
 import numpy as np
 from numpy.typing import NDArray
 import scipy
-from scipy.spatial import voronoi_plot_2d
 
 from . import exceptions, util
 from .geometry import BoundingBox2d, CentroidHelper, CircumcircleHelper
 
 
 logger = logging.getLogger(__name__)
 
 
 class Base(ABC):
-    def __init__(self, *, points: NDArray[np.float_]) -> None:
+    def __init__(
+        self, *, points: NDArray[np.float_], bounding_box: BoundingBox2d | None
+    ) -> None:
         """
 
         Args:
             points:
                 A collection of "n" 2D points arranged in the Cartesian
                 coordinate system with the axis order (x, y) and having a shape
                 of (n, 2).
+            bounding_box:
+                An optional bounding box specifying the boundary of points
         """
         assert self._check_points_validity(points=points)
 
         self._points: NDArray[np.float_] = points
         self._delaunay_triangulation_computed: bool = False
         self._ridges_and_regions_computed: bool = False
         self._voronoi_tessellation_computed: bool = False
         self._barycentric_dual_computed: bool = False
 
-        self._bounding_box: BoundingBox2d = self._compute_bounding_box(
-            points=points
+        if bounding_box is not None and (
+            np.any(np.min(points, axis=0) < bounding_box.min_)
+            or np.any(np.max(points, axis=0) > bounding_box.max_)
+        ):
+            raise ValueError("The points are not within the bounding box")
+
+        self._bounding_box: BoundingBox2d = (
+            self._compute_bounding_box(points=points)
+            if bounding_box is None
+            else bounding_box
         )
 
         self._triangles: NDArray[np.intc]
         self._ridge_points: NDArray[np.int32]
         self._ridge_vertices: list[list[int]]
         self._regions: list[list[int]]
         self._voronoi_vertices: NDArray[np.float_]
@@ -110,34 +120,14 @@
         )
 
     @staticmethod
     def _duplicated_points_exist(points: NDArray[np.float32]) -> bool:
         _, count = np.unique(points, axis=0, return_counts=True)
         return np.any(count > 1).item()
 
-    @staticmethod
-    def _plot_voronoi_diagram(
-        voronoi_diagram: scipy.spatial._qhull.Voronoi,
-        bounding_box: BoundingBox2d,
-    ):
-        fig = voronoi_plot_2d(
-            voronoi_diagram,
-            show_vertices=False,
-            line_colors="orange",
-            line_alpha=0.6,
-            point_size=2,
-        )
-        ax = fig.axes[0]
-        lower_lim, upper_lim = np.min(bounding_box.min_), np.max(
-            bounding_box.max_
-        )
-        ax.set_xlim(lower_lim, upper_lim)
-        ax.set_ylim(lower_lim, upper_lim)
-        plt.show()
-
     @classmethod
     def _jitter_points_on_overlap(
         cls,
         points: NDArray[np.float_],
         rng: np.random.Generator,
         scale: float | None = None,
     ) -> NDArray[np.float_]:
@@ -392,31 +382,30 @@
             axis=0,
         )
         # NOTE: Not sure whether qhull_options should be changed
         voronoi_diagram = scipy.spatial.Voronoi(
             points_with_dilated_bounding_box_vertices,
             # qhull_options="Qbb Qc Qx",
         )
-        if __debug__:
-            if debug:
-                cls._plot_voronoi_diagram(voronoi_diagram=voronoi_diagram)
 
         new_points = cls._compute_centroids_of_voronoi_diagram(
             voronoi_diagram=voronoi_diagram,
             target_regions_indices=voronoi_diagram.point_region[:-4],
         )
         new_points = np.clip(
             new_points, a_min=bounding_box.min_, a_max=bounding_box.max_
         )
         return new_points
 
 
 class Delaunay(Base):
-    def __init__(self, *, points: NDArray[np.float_]) -> None:
-        super().__init__(points=points)
+    def __init__(
+        self, *, points: NDArray[np.float_], bounding_box: BoundingBox2d | None
+    ) -> None:
+        super().__init__(points=points, bounding_box=bounding_box)
 
         self.compute_delaunay_triangulation()
 
     def _compute_ridges_and_regions(self) -> None:
         if self._ridges_and_regions_computed:
             return
         self.compute_delaunay_triangulation()
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/geometry/bounding_box_2d.py` & `delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/geometry/bounding_box_2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,29 +87,26 @@
             ],
             dtype=np.float_,
         )
         t_enter = np.zeros_like(x1)
         t_exit = np.ones_like(x1)
 
         for i in range(4):
-            is_parallel = p[i] == 0
+            is_parallel = np.isclose(p[i], 0)
             outside_parallel = np.logical_and(is_parallel, q[i] < 0)
-            # t = np.where(p[i] != 0, q[i] / p[i], np.inf)
+            t_enter[outside_parallel] = np.nan
+            t_exit[outside_parallel] = np.nan
             # To avoid RuntimeWarning: divide by zero encountered in divide
             t = np.divide(
-                q[i], p[i], out=np.full_like(q[i], np.inf), where=p[i] != 0
-            )
-            t_enter = np.where(
-                np.logical_and(p[i] < 0, ~outside_parallel),
-                np.maximum(t_enter, t),
-                t_enter,
+                q[i], p[i], out=np.full_like(q[i], np.inf), where=~is_parallel
             )
+            t_enter = np.where(p[i] < 0, np.maximum(t_enter, t), t_enter)
             t_exit = np.where(p[i] > 0, np.minimum(t_exit, t), t_exit)
 
-        outside = t_enter > t_exit
+        outside = np.logical_or(np.isnan(t_enter), t_enter > t_exit)
         x1_clip = np.where(~outside, x1 + t_enter * dx, np.nan)
         y1_clip = np.where(~outside, y1 + t_enter * dy, np.nan)
         x2_clip = np.where(~outside, x1 + t_exit * dx, np.nan)
         y2_clip = np.where(~outside, y1 + t_exit * dy, np.nan)
 
         result = np.stack(
             [
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py` & `delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/geometry/circumcircle.py`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py` & `delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d/util/scipy_spatial_mocked.py`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO` & `delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delaunay-triangulation-and-its-dual-2d
-Version: 0.1.4
+Version: 0.1.5
 License: MIT License
         
         Copyright (c) 2024 M.H. Luk
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt` & `delaunay_triangulation_and_its_dual_2d-0.1.5/delaunay_triangulation_and_its_dual_2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4/pyproject.toml` & `delaunay_triangulation_and_its_dual_2d-0.1.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4/tests/delaunay/performance.py` & `delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/performance.py`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4/tests/delaunay/test_all.py` & `delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/test_all.py`

 * *Files identical despite different names*

### Comparing `delaunay_triangulation_and_its_dual_2d-0.1.4/tests/delaunay/try.py` & `delaunay_triangulation_and_its_dual_2d-0.1.5/tests/delaunay/try.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import matplotlib.collections
 import matplotlib.pyplot as plt
 import numpy as np
 import scipy.spatial
 
 import delaunay_triangulation_and_its_dual_2d
 import delaunay_triangulation_and_its_dual_2d.exceptions
+import delaunay_triangulation_and_its_dual_2d.geometry
 
 
 def visualize_mocked_scipy_spatial_delaunay_and_voronoi():
     points = np.array(
         [[0, 0], [3, 0], [1, 1], [3, 2], [4, 2], [1, 3], [2, 4], [4, 4]],
         dtype=np.float32,
     )
@@ -54,22 +55,40 @@
 #         matplotlib.collections.LineCollection(rectangle, colors="blue")
 #     )
 #     ax.autoscale()
 #     ax.grid()
 #     plt.show()
 
 
-def try_compute_bounded_line_segments_of_dual():
+def try_compute_bounded_line_segments_of_dual_from_predefined_points():
     points = np.array(
         [[0, 0], [3, 0], [1, 1], [3, 2], [4, 2], [1, 3], [2, 4], [4, 4]],
         dtype=np.float32,
     )
     delaunay = delaunay_triangulation_and_its_dual_2d.Delaunay(points=points)
     bounded_line_segments = delaunay.compute_bounded_line_segments_of_dual(
         dual="voronoi"
     )
     print("bounded_line_segments.shape: ", bounded_line_segments.shape)
 
 
+def try_compute_bounded_line_segments_of_dual_from_random_points():
+    lower_bound = 0.0
+    upper_bound = 1.0
+    rng = np.random.default_rng()
+    points = rng.uniform(low=lower_bound, high=upper_bound, size=(10, 2))
+    delaunay = delaunay_triangulation_and_its_dual_2d.Delaunay(
+        points=points,
+        bounding_box=delaunay_triangulation_and_its_dual_2d.geometry.BoundingBox2d(
+            min_=np.array([lower_bound, lower_bound], dtype=np.float_),
+            max_=np.array([upper_bound, upper_bound], dtype=np.float_),
+        ),
+    )
+    bounded_line_segments = delaunay.compute_bounded_line_segments_of_dual(
+        dual="voronoi"
+    )
+    print("bounded_line_segments.shape: ", bounded_line_segments.shape)
+
+
 if __name__ == "__main__":
     # Reference: https://stackoverflow.com/a/52837375
     globals()[sys.argv[1]]()
```

