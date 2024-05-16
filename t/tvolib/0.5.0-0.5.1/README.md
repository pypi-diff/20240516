# Comparing `tmp/tvolib-0.5.0.tar.gz` & `tmp/tvolib-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvolib-0.5.0.tar", max compression
+gzip compressed data, was "tvolib-0.5.1.tar", max compression
```

## Comparing `tvolib-0.5.0.tar` & `tvolib-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-10-09 18:01:36.891552 tvolib-0.5.0/LICENSE
--rw-r--r--   0        0        0      398 2023-10-09 18:01:36.891552 tvolib-0.5.0/README.md
--rw-r--r--   0        0        0      817 2023-10-31 16:27:49.261853 tvolib-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       46 2023-10-09 18:01:36.892552 tvolib-0.5.0/src/tvolib/__init__.py
--rw-r--r--   0        0        0        0 2023-10-09 18:01:36.892552 tvolib-0.5.0/src/tvolib/models/__init__.py
--rw-r--r--   0        0        0     6416 2023-10-09 18:01:36.892552 tvolib-0.5.0/src/tvolib/models/magnetopause_model.py
--rw-r--r--   0        0        0      219 2023-10-09 18:01:36.892552 tvolib-0.5.0/src/tvolib/mpl_utils/__init__.py
--rw-r--r--   0        0        0     2067 2023-10-09 18:01:36.892552 tvolib-0.5.0/src/tvolib/mpl_utils/_draw.py
--rw-r--r--   0        0        0      727 2023-10-31 16:26:39.902859 tvolib-0.5.0/src/tvolib/mpl_utils/_format.py
--rw-r--r--   0        0        0      899 2023-10-09 18:01:36.892552 tvolib-0.5.0/src/tvolib/mpl_utils/_setup.py
--rw-r--r--   0        0        0    25742 2023-10-09 18:01:36.892552 tvolib-0.5.0/src/tvolib/mpl_utils/data/mpl_utils.mplstyle
--rw-r--r--   0        0        0      174 2023-10-09 18:01:36.892552 tvolib-0.5.0/src/tvolib/numeric/__init__.py
--rw-r--r--   0        0        0     1463 2023-10-09 18:01:36.892552 tvolib-0.5.0/src/tvolib/numeric/curlometer.py
--rw-r--r--   0        0        0     2318 2023-10-09 18:01:36.892552 tvolib-0.5.0/src/tvolib/numeric/interpolate.py
--rw-r--r--   0        0        0     2455 2023-10-09 18:01:36.892552 tvolib-0.5.0/src/tvolib/numeric/moving.py
--rw-r--r--   0        0        0      572 2023-10-09 18:01:36.892552 tvolib-0.5.0/src/tvolib/numeric/timing.py
--rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 tvolib-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-10-09 18:01:36.891552 tvolib-0.5.1/LICENSE
+-rw-r--r--   0        0        0      398 2023-10-09 18:01:36.891552 tvolib-0.5.1/README.md
+-rw-r--r--   0        0        0      817 2023-10-31 16:40:19.129794 tvolib-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-10-31 16:39:14.937800 tvolib-0.5.1/src/tvolib/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-09 18:01:36.892552 tvolib-0.5.1/src/tvolib/models/__init__.py
+-rw-r--r--   0        0        0     6416 2023-10-09 18:01:36.892552 tvolib-0.5.1/src/tvolib/models/magnetopause_model.py
+-rw-r--r--   0        0        0      229 2023-10-31 16:39:31.329798 tvolib-0.5.1/src/tvolib/mpl_utils/__init__.py
+-rw-r--r--   0        0        0     2067 2023-10-09 18:01:36.892552 tvolib-0.5.1/src/tvolib/mpl_utils/_draw.py
+-rw-r--r--   0        0        0      743 2023-10-31 16:39:11.613800 tvolib-0.5.1/src/tvolib/mpl_utils/_format.py
+-rw-r--r--   0        0        0      899 2023-10-09 18:01:36.892552 tvolib-0.5.1/src/tvolib/mpl_utils/_setup.py
+-rw-r--r--   0        0        0    25742 2023-10-09 18:01:36.892552 tvolib-0.5.1/src/tvolib/mpl_utils/data/mpl_utils.mplstyle
+-rw-r--r--   0        0        0      174 2023-10-09 18:01:36.892552 tvolib-0.5.1/src/tvolib/numeric/__init__.py
+-rw-r--r--   0        0        0     1463 2023-10-09 18:01:36.892552 tvolib-0.5.1/src/tvolib/numeric/curlometer.py
+-rw-r--r--   0        0        0     2318 2023-10-09 18:01:36.892552 tvolib-0.5.1/src/tvolib/numeric/interpolate.py
+-rw-r--r--   0        0        0     2455 2023-10-09 18:01:36.892552 tvolib-0.5.1/src/tvolib/numeric/moving.py
+-rw-r--r--   0        0        0      572 2023-10-09 18:01:36.892552 tvolib-0.5.1/src/tvolib/numeric/timing.py
+-rw-r--r--   0        0        0     1292 1970-01-01 00:00:00.000000 tvolib-0.5.1/PKG-INFO
```

### Comparing `tvolib-0.5.0/LICENSE` & `tvolib-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tvolib-0.5.0/pyproject.toml` & `tvolib-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tvolib"
-version = "0.5.0"
+version = "0.5.1"
 description = "A personal collection of Python and IDL research tools in Space Plasma Physics."
 authors = ["Tien Vo <tien.a.vo@proton.me>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 packages = [
     { include = "tvolib", from = "src" }
 ]
```

### Comparing `tvolib-0.5.0/src/tvolib/models/magnetopause_model.py` & `tvolib-0.5.1/src/tvolib/models/magnetopause_model.py`

 * *Files identical despite different names*

### Comparing `tvolib-0.5.0/src/tvolib/mpl_utils/_draw.py` & `tvolib-0.5.1/src/tvolib/mpl_utils/_draw.py`

 * *Files identical despite different names*

### Comparing `tvolib-0.5.0/src/tvolib/mpl_utils/_format.py` & `tvolib-0.5.1/src/tvolib/mpl_utils/_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 __all__ = [
     "add_colorbar",
+    "add_text",
     "format_datetime_axis",
 ]
 
 import matplotlib.dates as mdates
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 
 def add_colorbar(axis, where="right", pad=0.05, size="2%"):
     r"""Adds colorbar next to an axis"""
     divider = make_axes_locatable(axis)
     return divider.append_axes(where, size=size, pad=pad)
 
 
-def format_datetime_axis(axis):
-    locator = mdates.AutoDateLocator()
-    formatter = mdates.ConciseDateFormatter(locator)
-    axis.xaxis.set_major_formatter(formatter)
-
-
 def add_text(axis, x, y, text, **kwargs):
     transform = axis.transAxes
     box_format = dict(facecolor="wheat", alpha=0.9)
     axis.text(x, y, text, transform=transform, bbox=box_format, **kwargs)
+
+
+def format_datetime_axis(axis):
+    locator = mdates.AutoDateLocator()
+    formatter = mdates.ConciseDateFormatter(locator)
+    axis.xaxis.set_major_formatter(formatter)
```

### Comparing `tvolib-0.5.0/src/tvolib/mpl_utils/_setup.py` & `tvolib-0.5.1/src/tvolib/mpl_utils/_setup.py`

 * *Files identical despite different names*

### Comparing `tvolib-0.5.0/src/tvolib/mpl_utils/data/mpl_utils.mplstyle` & `tvolib-0.5.1/src/tvolib/mpl_utils/data/mpl_utils.mplstyle`

 * *Files identical despite different names*

### Comparing `tvolib-0.5.0/src/tvolib/numeric/curlometer.py` & `tvolib-0.5.1/src/tvolib/numeric/curlometer.py`

 * *Files identical despite different names*

### Comparing `tvolib-0.5.0/src/tvolib/numeric/interpolate.py` & `tvolib-0.5.1/src/tvolib/numeric/interpolate.py`

 * *Files identical despite different names*

### Comparing `tvolib-0.5.0/src/tvolib/numeric/moving.py` & `tvolib-0.5.1/src/tvolib/numeric/moving.py`

 * *Files identical despite different names*

### Comparing `tvolib-0.5.0/src/tvolib/numeric/timing.py` & `tvolib-0.5.1/src/tvolib/numeric/timing.py`

 * *Files identical despite different names*

### Comparing `tvolib-0.5.0/PKG-INFO` & `tvolib-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvolib
-Version: 0.5.0
+Version: 0.5.1
 Summary: A personal collection of Python and IDL research tools in Space Plasma Physics.
 Home-page: https://github.com/tien-vo/tvolib
 License: GPL-3.0-or-later
 Author: Tien Vo
 Author-email: tien.a.vo@proton.me
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

