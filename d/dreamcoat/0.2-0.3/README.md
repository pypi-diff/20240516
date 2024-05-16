# Comparing `tmp/dreamcoat-0.2.tar.gz` & `tmp/dreamcoat-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamcoat-0.2.tar", last modified: Wed Oct 25 14:20:08 2023, max compression
+gzip compressed data, was "dreamcoat-0.3.tar", last modified: Thu May 16 09:21:32 2024, max compression
```

## Comparing `dreamcoat-0.2.tar` & `dreamcoat-0.3.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-10-25 14:20:08.046021 dreamcoat-0.2/
--rw-r--r--   0 matthew    (501) staff       (20)    35149 2023-07-20 06:28:58.000000 dreamcoat-0.2/LICENSE
--rw-r--r--   0 matthew    (501) staff       (20)      851 2023-10-25 14:20:08.045841 dreamcoat-0.2/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)      214 2023-10-25 13:24:04.000000 dreamcoat-0.2/README.md
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-10-25 14:20:08.044516 dreamcoat-0.2/dreamcoat/
--rw-r--r--   0 matthew    (501) staff       (20)     2097 2023-10-25 13:47:10.000000 dreamcoat-0.2/dreamcoat/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)    35118 2023-07-20 06:28:58.000000 dreamcoat-0.2/dreamcoat/cmems.py
--rw-r--r--   0 matthew    (501) staff       (20)     4102 2023-07-20 06:28:58.000000 dreamcoat-0.2/dreamcoat/convert.py
--rw-r--r--   0 matthew    (501) staff       (20)     5449 2023-10-25 13:25:53.000000 dreamcoat-0.2/dreamcoat/ctd.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-10-25 14:20:08.045607 dreamcoat-0.2/dreamcoat/maps/
--rw-r--r--   0 matthew    (501) staff       (20)    21015 2023-10-25 13:52:06.000000 dreamcoat-0.2/dreamcoat/maps/__init__.py
--rw-r--r--   0 matthew    (501) staff       (20)     3459 2023-07-20 06:28:58.000000 dreamcoat-0.2/dreamcoat/maps/degrees_decimal_minutes.py
--rw-r--r--   0 matthew    (501) staff       (20)     1827 2023-10-25 13:24:04.000000 dreamcoat-0.2/dreamcoat/meta.py
--rw-r--r--   0 matthew    (501) staff       (20)     9378 2023-07-20 06:28:58.000000 dreamcoat-0.2/dreamcoat/modis.py
--rw-r--r--   0 matthew    (501) staff       (20)    32266 2023-10-25 13:51:10.000000 dreamcoat-0.2/dreamcoat/plot.py
--rw-r--r--   0 matthew    (501) staff       (20)     4818 2023-07-20 06:28:58.000000 dreamcoat-0.2/dreamcoat/send.py
--rw-r--r--   0 matthew    (501) staff       (20)     5774 2023-07-20 06:28:58.000000 dreamcoat-0.2/dreamcoat/style.py
-drwxr-xr-x   0 matthew    (501) staff       (20)        0 2023-10-25 14:20:08.045177 dreamcoat-0.2/dreamcoat.egg-info/
--rw-r--r--   0 matthew    (501) staff       (20)      851 2023-10-25 14:20:08.000000 dreamcoat-0.2/dreamcoat.egg-info/PKG-INFO
--rw-r--r--   0 matthew    (501) staff       (20)      436 2023-10-25 14:20:08.000000 dreamcoat-0.2/dreamcoat.egg-info/SOURCES.txt
--rw-r--r--   0 matthew    (501) staff       (20)        1 2023-10-25 14:20:08.000000 dreamcoat-0.2/dreamcoat.egg-info/dependency_links.txt
--rw-r--r--   0 matthew    (501) staff       (20)      168 2023-10-25 14:20:08.000000 dreamcoat-0.2/dreamcoat.egg-info/requires.txt
--rw-r--r--   0 matthew    (501) staff       (20)       10 2023-10-25 14:20:08.000000 dreamcoat-0.2/dreamcoat.egg-info/top_level.txt
--rw-r--r--   0 matthew    (501) staff       (20)      938 2023-10-25 13:48:59.000000 dreamcoat-0.2/pyproject.toml
--rw-r--r--   0 matthew    (501) staff       (20)       38 2023-10-25 14:20:08.046058 dreamcoat-0.2/setup.cfg
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-05-16 09:21:32.846904 dreamcoat-0.3/
+-rw-r--r--   0 matthew    (501) staff       (20)    35149 2023-07-20 06:28:58.000000 dreamcoat-0.3/LICENSE
+-rw-r--r--   0 matthew    (501) staff       (20)      601 2024-05-16 09:21:32.846441 dreamcoat-0.3/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)      214 2023-10-30 11:51:49.000000 dreamcoat-0.3/README.md
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-05-16 09:21:32.840595 dreamcoat-0.3/dreamcoat/
+-rw-r--r--   0 matthew    (501) staff       (20)     1548 2024-05-04 14:14:39.000000 dreamcoat-0.3/dreamcoat/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)     5432 2024-05-16 09:15:32.000000 dreamcoat-0.3/dreamcoat/convert.py
+-rw-r--r--   0 matthew    (501) staff       (20)    14504 2024-05-12 16:52:53.000000 dreamcoat-0.3/dreamcoat/ctd.py
+-rw-r--r--   0 matthew    (501) staff       (20)     1459 2024-04-30 05:27:14.000000 dreamcoat-0.3/dreamcoat/glider.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-05-16 09:21:32.843787 dreamcoat-0.3/dreamcoat/maps/
+-rw-r--r--   0 matthew    (501) staff       (20)    26929 2024-05-12 05:06:39.000000 dreamcoat-0.3/dreamcoat/maps/__init__.py
+-rw-r--r--   0 matthew    (501) staff       (20)     6559 2024-05-12 04:48:46.000000 dreamcoat-0.3/dreamcoat/maps/degrees_decimal_minutes.py
+-rw-r--r--   0 matthew    (501) staff       (20)     1826 2023-10-31 15:05:47.000000 dreamcoat-0.3/dreamcoat/meta.py
+-rw-r--r--   0 matthew    (501) staff       (20)     5319 2024-05-05 11:10:49.000000 dreamcoat-0.3/dreamcoat/plot.py
+-rw-r--r--   0 matthew    (501) staff       (20)     2359 2024-05-05 12:37:22.000000 dreamcoat-0.3/dreamcoat/stats.py
+-rw-r--r--   0 matthew    (501) staff       (20)     2643 2024-04-28 10:28:28.000000 dreamcoat-0.3/dreamcoat/underway.py
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-05-16 09:21:32.846169 dreamcoat-0.3/dreamcoat.egg-info/
+-rw-r--r--   0 matthew    (501) staff       (20)      601 2024-05-16 09:21:32.000000 dreamcoat-0.3/dreamcoat.egg-info/PKG-INFO
+-rw-r--r--   0 matthew    (501) staff       (20)      484 2024-05-16 09:21:32.000000 dreamcoat-0.3/dreamcoat.egg-info/SOURCES.txt
+-rw-r--r--   0 matthew    (501) staff       (20)        1 2024-05-16 09:21:32.000000 dreamcoat-0.3/dreamcoat.egg-info/dependency_links.txt
+-rw-r--r--   0 matthew    (501) staff       (20)       83 2024-05-16 09:21:32.000000 dreamcoat-0.3/dreamcoat.egg-info/requires.txt
+-rw-r--r--   0 matthew    (501) staff       (20)       10 2024-05-16 09:21:32.000000 dreamcoat-0.3/dreamcoat.egg-info/top_level.txt
+-rw-r--r--   0 matthew    (501) staff       (20)      475 2024-04-17 16:37:15.000000 dreamcoat-0.3/pyproject.toml
+-rw-r--r--   0 matthew    (501) staff       (20)       38 2024-05-16 09:21:32.846957 dreamcoat-0.3/setup.cfg
+drwxr-xr-x   0 matthew    (501) staff       (20)        0 2024-05-16 09:21:32.845918 dreamcoat-0.3/tests/
+-rw-r--r--   0 matthew    (501) staff       (20)      689 2024-04-18 04:59:57.000000 dreamcoat-0.3/tests/test_LatLon.py
+-rw-r--r--   0 matthew    (501) staff       (20)     1083 2024-05-05 07:01:44.000000 dreamcoat-0.3/tests/test_stats.py
+-rw-r--r--   0 matthew    (501) staff       (20)     1516 2024-04-17 16:56:00.000000 dreamcoat-0.3/tests/test_vptree.py
```

### Comparing `dreamcoat-0.2/LICENSE` & `dreamcoat-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamcoat-0.2/PKG-INFO` & `dreamcoat-0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 Metadata-Version: 2.1
 Name: dreamcoat
-Version: 0.2
+Version: 0.3
 Summary: The joyful oceanographic seagoing expedition planning helper
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: calkulate
-Requires-Dist: cartopy
 Requires-Dist: fsspec
 Requires-Dist: geographiclib
 Requires-Dist: great_circle_calculator
-Requires-Dist: gsw
-Requires-Dist: keyring
-Requires-Dist: koolstof
 Requires-Dist: matplotlib
-Requires-Dist: motuclient
-Requires-Dist: napari
-Requires-Dist: netcdf4
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: shapely
 Requires-Dist: vptree
-Requires-Dist: xarray
-Requires-Dist: yagmail
-Requires-Dist: zarr
 
 # dreamcoat
 
 The joyful oceanographic seagoing expedition planning helper
 
 ## Version list
```

### Comparing `dreamcoat-0.2/dreamcoat/__init__.py` & `dreamcoat-0.3/dreamcoat/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,54 @@
-"""Dreamcoat
+"""
+Dreamcoat
 =========
 
 > The joyful oceanographic seagoing expedition planning helper
 
-Dreamcoat is a set of tools to help work with live oceanographic data of the sort that
-might be needed during a research expedition.  At sea, internet bandwidth is usually
-restricted, so dreamcoat is designed to be remotely usable: it can be left to run on a
-server on land, which does the heavy lifting in terms of downloading files, producing
-smaller figures or data subsets that can be automatically sent by email or uploaded to
-an online repo.
+Dreamcoat is a set of tools to help work with oceanographic data of the sort that might
+be needed or generated during a research expedition.
 
 Dreamcoat is being developed by Dr Matthew Humphreys (https://seaco2.group) at the NIOZ
 Royal Netherlands Institute for Sea Research, Texel.  You're very welcome to give it a
 go and suggestions and contributions are welcome, but please be aware that it is
-primarily designed as a personal tool so I probably won't be able to help out if you get
+primarily designed as a personal tool so there probably won't be much help if you get
 stuck; nothing is guaranteed not to break between versions, and the documentation
 (https://mvdh.xyz/dreamcoat) may be incomplete or out of date.
 
 The docstring examples assume that `dreamcoat` has been imported as ``dc``:
 
   >>> import dreamcoat as dc
 
-Available subpackages
----------------------
-cmems
-    Tools to import and open CMEMS data files
-    (https://data.marine.copernicus.eu/products).
+Modules
+-------
 convert
-    Functions to convert between different units and formats.
+    Convert between different units and formats.
 ctd
     Dealing with CTD data files.
+glider
+    Working with Slocum gliders.
 maps
     Working with data in (longitude, latitude) space.
 meta
-    Metadata for `dreamcoat`.
-modis
-    Tools to import and open data from the MODIS satellites
-    (https://oceancolor.gsfc.nasa.gov/).
+    Metadata for dreamcoat.
 plot
     Shortcuts for data visualisations.
-send
-    Send files by email.
-style
-    Get colour schemes and nicely formatted labels based on variable names.
-"""
+underway
+    Working with underway data files.
 
-from . import convert, cmems, ctd, maps, meta, modis, plot, send, style
-from .maps import (
-    Route,
-    get_route_distance,
-    linspace_gc,
-    linspace_gc_waypoints,
-    build_vptree,
-)
-from .maps.degrees_decimal_minutes import DegreesDecimalMinutes
+Classes
+-------
+LatLon
+    A tool to convert between decimal degrees and degrees decimal minutes.
+Route
+    A set of waypoints defining a route.
+
+Functions
+---------
+hello
+    Report the version number.
+"""
 
-DDM = DegreesDecimalMinutes
+from . import convert, ctd, glider, maps, meta, plot, stats, underway
+from .maps import Route
+from .maps.degrees_decimal_minutes import LatLon
 from .meta import __version__, hello
-from .style import styles
```

### Comparing `dreamcoat-0.2/dreamcoat/maps/__init__.py` & `dreamcoat-0.3/dreamcoat/maps/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-"""dreamcoat.maps
-=================
-A set of tools for helping with geographic mapping and routing.
+"""
+dreamcoat.maps
+==============
+Geographic mapping and route planning.
 
 Functions
 ---------
+build_vptree
+    Build vantage-point tree for Natural Earth Data coastline.
+get_distance
+    Calculate distance between a pair of points.
+get_distance_gcc
+    Calculate distance between a pair of points in km using great_circle_calculator.
+get_distance_geodesic
+    Calculate geodesic distance between a single pair of points in km.
+get_route_distance
+    Calculate distance from point to point along a route.
 linspace_gc
     Return evenly spaced points along a great circle.
 linspace_gc_waypoints
     Apply `linspace_gc` across a series of waypoints, aiming for evenly spaced points.
 linspace_gc_waypoints_cs
     Apply `linspace_gc` across a series of waypoints, with a constant number of points
     between each pair.
-get_distance_geodesic
-    Calculate geodesic distance between a single pair of points in km.
-get_distance_gcc
-    Calculate distance between a pair of points in km using great_circle_calculator.
-get_distance
-    Calculate distance between a pair of points.
-get_route_distance
-    Calculate distance from point to point along a route.
-map_point_to_section
-    Find the closest point on a single line section to a given point.
 map_point_to_route
     Find the closest point on a route to a new point.
+map_point_to_section
+    Find the closest point on a single line section to a given point.
 """
 
 import itertools
 from collections import namedtuple
 import numpy as np
 from geographiclib.geodesic import Geodesic
 import great_circle_calculator.great_circle_calculator as gcc
@@ -185,40 +188,71 @@
     if method == "gcc":
         return get_distance_gcc
     elif method == "geodesic":
         return get_distance_geodesic
 
 
 def get_distance(lon_lat_1, lon_lat_2, method="gcc"):
-    """Calculate distance between a pair of points in km using either great_circle_calculator.
-    (default) or geographiclib (more accurate but ~50 times slower).
+    """Calculate distance between a pair of points in km using either
+    great_circle_calculator (default) or geographiclib (more accurate but ~50 times
+    slower).
+
     Parameters
     ----------
     lon_lat_1 : array_like
         (longitude, latitude) of the first point in decimal degrees.
     lon_lat_2 : array_like
         (longitude, latitude) of the second point in decimal degrees.
     method : str, optional
         Which method to use: 'gcc' (default) or 'geodesic'.
 
     Returns
     -------
     float
         Distance between the two points in km.
     """
+    if isinstance(lon_lat_1, degrees_decimal_minutes.LatLon):
+        lon_lat_1 = (lon_lat_1.longitude_dd, lon_lat_1.latitude_dd)
+    if isinstance(lon_lat_2, degrees_decimal_minutes.LatLon):
+        lon_lat_2 = (lon_lat_2.longitude_dd, lon_lat_2.latitude_dd)
     return _get_distance_func(method)(lon_lat_1, lon_lat_2)
 
 
+def get_heading(lon_lat_1, lon_lat_2):
+    """Calculate heading from lon_lat_1 to lon_lat_2.
+
+    Parameters
+    ----------
+    lon_lat_1 : array_like
+        (longitude, latitude) of the first point in decimal degrees.
+    lon_lat_2 : array_like
+        (longitude, latitude) of the second point in decimal degrees.
+
+    Returns
+    -------
+    float
+        Heading in ° (with N as 0, E as 90, ...).
+    """
+    if isinstance(lon_lat_1, degrees_decimal_minutes.LatLon):
+        lon_lat_1 = (lon_lat_1.longitude_dd, lon_lat_1.latitude_dd)
+    if isinstance(lon_lat_2, degrees_decimal_minutes.LatLon):
+        lon_lat_2 = (lon_lat_2.longitude_dd, lon_lat_2.latitude_dd)
+    heading = gcc.bearing_at_p1(lon_lat_1, lon_lat_2)
+    if heading < 0:
+        heading += 360
+    return heading
+
+
 def get_route_distance(waypoints, method="gcc"):
     """Calculate distance from point to point along a route.
 
     Parameters
     ----------
-    waypoints : (array_like, array_like)
-        The route (longitude, latitude) waypoints.
+    waypoints : array_like
+        The route (longitude, latitude) waypoints as a size (2, n) np.array.
     method : str, optional
         Which method to use: 'gcc' (default) or 'geodesic'.
 
     Returns
     -------
     array_like
         Distance from the start of the route in km.
@@ -292,16 +326,16 @@
 
 
 def map_point_to_route(route, lon_lat, extrapolate=False, verbose=False):
     """Find the closest point on a `route` to a new `lon_lat` point.
 
     Parameters
     ----------
-    route : array_like
-        (longitude, latitude) of the route waypoints.
+    route : Route
+        A Route object containing the route's waypoints.
     lon_lat : array_like
         (longitude, latitude) of the new off-route point.
     extrapolate : bool, optional
         Whether to extrapolate beyond the ends of the route, by default False.
     verbose : bool, optional
         Whether to report on progress, by default False.
 
@@ -411,15 +445,63 @@
         section.in_section,
         nearest,
     )
     return route_point
 
 
 class Route:
-    """ """
+    """A set of waypoints defining a route, which is assumed to travel in straight lines
+    (i.e., along great circles) between the waypoints.
+
+    Parameters
+    ----------
+    waypoints : np.ndarray
+        A (2, n) NumPy array of the (longitude, latitude) values of the waypoints.
+    distance_method : str, optional
+        Which method is used to calculate distances, either
+          "gcc" (default) - uses great_circle_calculator
+          "geodesic" - uses geographiclib.geodesic.Geodesic.WGS84
+        The first is an order of magnitude faster but a bit less accurate.
+
+    Attributes
+    ----------
+    waypoints : np.ndarray
+        The (2, n) NumPy array of the (longitude, latitude) values of the waypoints.
+    size : int
+        The number of waypoints (i.e., n).
+    distance_method : str
+        The method being used to calculate distances ("gcc" or "geodesic").
+    distance : np.ndarray
+        The distance of each waypoint along the route in km.
+    vpt : vptree.VPTree
+        A vantage-point tree for the route.
+    wp_interp : np.ndarray
+        A (2, n) NumPy array of the (longitude, latitude) values of a higher-resolution
+        set of points interpolated between the waypoints.  Appears after running the
+        interp method.
+    wp_distance : np.ndarray
+        The distance of each interpolated point in wp_interp along the route in km.
+        Appears after running the interp method.
+
+    Methods
+    -------
+    build_vpt
+        Create a vantage-point tree for the route.
+    find_nearest_waypoint
+        Find the index of the waypoint closest to a given new point.
+    get_distance
+        Find the distance along the route corresponding to the closest point on the
+        route to a new point.
+    get_lon_lat
+        Calculate the longitude and latitude of a given distance along the route.
+    interp
+        Interpolate the route to a higher resolution.
+    map_point_to_route
+        Find the closest point on the route to a new point.
+    """
 
     def __init__(self, waypoints, distance_method="gcc"):
         assert (
             isinstance(waypoints, np.ndarray)
             and waypoints.shape[0] == 2
             and waypoints.ndim == 2
         ), "`waypoints` must be a numpy array of shape (2, n)."
@@ -429,43 +511,108 @@
         assert np.all(
             (waypoints[1] >= -90) & (waypoints[1] <= 90)
         ), "All latitudes must be from -90 to 90."
         self.waypoints = waypoints
         self.size = waypoints.shape[1]
         self.distance_method = distance_method
         self.distance = get_route_distance(waypoints, method=distance_method)
-        self.build_vpt(distance_method=distance_method)
+        self.build_vpt()
 
-    def build_vpt(self, distance_method="gcc"):
+    def build_vpt(self):
         """Create a vantage-point tree that can be used to find nearest neighbours."""
-        self.vpt = VPTree(self.waypoints.T, _get_distance_func(distance_method))
+        self.vpt = VPTree(self.waypoints.T, _get_distance_func(self.distance_method))
 
     def find_nearest_waypoint(self, lon_lat):
-        """Find the index of the waypoint closest to `lon_lat`."""
+        """Find the index of the waypoint closest to a new point.
+
+        Parameters
+        ----------
+        lon_lat : array-like
+            A two-element list or array containing the (longitude, latitude) of a new
+            point, not necessarily on the route.
+
+        Returns
+        -------
+        int
+            The index of the waypoint closest to the new point.
+        """
         nearest = self.vpt.get_nearest_neighbor(lon_lat)[1]
         return (
             (self.waypoints[0] == nearest[0]) & (self.waypoints[1] == nearest[1])
         ).argmax()
 
-    map_point_to_route = map_point_to_route
+    def map_point_to_route(self, lon_lat, extrapolate=False, verbose=False):
+        """Find the closest point on the route to a new point.
+
+        Parameters
+        ----------
+        lon_lat : array-like
+            (longitude, latitude) of the new off-route point.
+        extrapolate : bool, optional
+            Whether to extrapolate beyond the ends of the route, by default False.
+        verbose : bool, optional
+            Whether to report on progress, by default False.
+
+        Results
+        -------
+        namedtuple (RoutePoint) containing fields
+            distance_on_route : float
+                Distance along the route up to the mapping of `lon_lat` onto the route
+                in km.
+            lon_lat : (float, float)
+                (longitude, latitude) of the mapping of `lon_lat` onto the route in
+                decimal degrees.
+            in_route : bool
+                Whether the mapping of `lon_lat` falls within the route.
+            waypoint_nearest : int
+                The index of the nearest waypoint.
+        """
+        return map_point_to_route(
+            self, lon_lat, extrapolate=extrapolate, verbose=verbose
+        )
 
     def interp(self, num_approx=100, endpoint=True):
         """Interpolate the route to a higher resolution, with the interpolated route
         stored in the attribute `wp_interp` and corresponding route distances in
         `wp_distance`.
+
+        The interpolation runs such that the exact positions of the original waypoints
+        are still included and the interpolated points are distributed as evenly as
+        possible between the waypoints.
+
+        Parameters
+        ----------
+        num_approx : int, optional
+            Approximate total number of interpolated points, by default 100.
+        endpoint : bool, optional
+            Whether to include the very final waypoint in the interpolated set, by
+            default True.
         """
         self.wp_interp = linspace_gc_waypoints(
             self.waypoints, num_approx=num_approx, endpoint=endpoint
         )
         self.wp_distance = get_route_distance(
             self.wp_interp, method=self.distance_method
         )
 
     def get_lon_lat(self, distance, extrapolate=False):
-        """Get the longitude and latitude of a given distance along the route."""
+        """Get the longitude and latitude of a given distance along the route.
+
+        Parameters
+        ----------
+        distance : float
+            A distance along the route in km.
+        extrapolate : bool, optional
+            Whether to extrapolate beyond the ends of the route, if necessary; by
+            default False.
+
+        array-like
+            (longitude, latitude) of the point along the route at the specified
+            distance.
+        """
         out_of_range = False
         if distance in self.distance:
             nearest = (self.distance == distance).argmax()
             lon_lat = self.waypoints[:, nearest]
         else:
             if distance < 0:
                 after = 1
@@ -492,15 +639,30 @@
                     self.waypoints[:, before],
                     self.waypoints[:, after],
                     fraction=section_fraction,
                 )
         return lon_lat
 
     def get_distance(self, lon_lat, extrapolate=False, verbose=False):
-        """Get the route distance corresponding to a given longitude and latitude."""
+        """Get the route distance corresponding to a given longitude and latitude.
+
+        Parameters
+        ----------
+        lon_lat : array-like
+            (longitude, latitude) of the new off-route point.
+        extrapolate : bool, optional
+            Whether to extrapolate beyond the ends of the route, by default False.
+        verbose : bool, optional
+            Whether to report on progress, by default False.
+
+        Returns
+        -------
+        float
+            Distance along the route in km.
+        """
         rp = self.map_point_to_route(lon_lat, extrapolate=extrapolate, verbose=verbose)
         return rp.distance_on_route
 
 
 def geodesic_distance(lon_lat_1, lon_lat_2):
     """Calculate geodesic distance between a single pair of points in km, based on
     https://stackoverflow.com/a/45480555
@@ -532,15 +694,16 @@
     Parameters
     ----------
     lat_range : array_like
         (min, max) latitude in decimal degrees.
     lon_range : array_like
         (min, max) longitude in decimal degrees.
     resolution : str, optional
-        Natural Earth Data resolution, by default "10m".
+        Natural Earth Data resolution, by default "10m" (can also be "50m" or "110m";
+        default "10m" is the most detailed).
 
     Returns
     -------
     list
         Coordinates of the matching coastlines.
     """
     assert resolution in ["10m", "50m", "110m"]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dreamcoat-0.2/dreamcoat/meta.py` & `dreamcoat-0.3/dreamcoat/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
-version_number = "0.2"
-version_colour = "yellow"
+version_number = "0.3"
+version_colour = "green"
 __version__ = "{}-{}".format(version_number, version_colour)
 
 
 def hello():
     print(
         r"""
     ____    ____    U _____ u    _      __  __     ____   U  ___ u    _       _____
```

### Comparing `dreamcoat-0.2/dreamcoat.egg-info/PKG-INFO` & `dreamcoat-0.3/dreamcoat.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 Metadata-Version: 2.1
 Name: dreamcoat
-Version: 0.2
+Version: 0.3
 Summary: The joyful oceanographic seagoing expedition planning helper
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: calkulate
-Requires-Dist: cartopy
 Requires-Dist: fsspec
 Requires-Dist: geographiclib
 Requires-Dist: great_circle_calculator
-Requires-Dist: gsw
-Requires-Dist: keyring
-Requires-Dist: koolstof
 Requires-Dist: matplotlib
-Requires-Dist: motuclient
-Requires-Dist: napari
-Requires-Dist: netcdf4
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: shapely
 Requires-Dist: vptree
-Requires-Dist: xarray
-Requires-Dist: yagmail
-Requires-Dist: zarr
 
 # dreamcoat
 
 The joyful oceanographic seagoing expedition planning helper
 
 ## Version list
```

