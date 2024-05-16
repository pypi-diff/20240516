# Comparing `tmp/pycomplexheatmap-1.7.2.tar.gz` & `tmp/pycomplexheatmap-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycomplexheatmap-1.7.2.tar", last modified: Mon Apr 15 20:36:49 2024, max compression
+gzip compressed data, was "pycomplexheatmap-1.7.3.tar", last modified: Fri Apr 26 21:18:05 2024, max compression
```

## Comparing `pycomplexheatmap-1.7.2.tar` & `pycomplexheatmap-1.7.3.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:36:49.204140 pycomplexheatmap-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:36:49.176140 pycomplexheatmap-1.7.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:36:49.176140 pycomplexheatmap-1.7.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:36:49.176140 pycomplexheatmap-1.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-15 20:36:49.204140 pycomplexheatmap-1.7.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:36:49.176140 pycomplexheatmap-1.7.2/PyComplexHeatmap/
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-15 20:36:48.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    63152 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)    80279 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/clustermap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)    21688 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/dotHeatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    19871 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/oncoPrint.py
--rw-r--r--   0 runner    (1001) docker     (127)    26848 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:36:49.204140 pycomplexheatmap-1.7.2/PyComplexHeatmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-15 20:36:48.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-15 20:36:49.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:36:48.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-15 20:36:48.000000 pycomplexheatmap-1.7.2/PyComplexHeatmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:36:49.204140 pycomplexheatmap-1.7.2/comparison/
--rw-r--r--   0 runner    (1001) docker     (127)    88559 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/ComplexHeatmap.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   319414 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/ComplexHeatmap.png
--rw-r--r--   0 runner    (1001) docker     (127)   159236 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/PyComplexHeatmap.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   669615 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/PyComplexHeatmap.png
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/README.md
--rw-r--r--   0 runner    (1001) docker     (127) 15584021 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/beta.csv
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/compare.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/df_col.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2909164 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/df_row.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/heatmap.R
--rw-r--r--   0 runner    (1001) docker     (127)   182760 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/heatmap.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-15 20:36:27.000000 pycomplexheatmap-1.7.2/comparison/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-15 20:36:28.000000 pycomplexheatmap-1.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:36:49.204140 pycomplexheatmap-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-15 20:36:28.000000 pycomplexheatmap-1.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:18:05.850218 pycomplexheatmap-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:18:05.822218 pycomplexheatmap-1.7.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:18:05.822218 pycomplexheatmap-1.7.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:18:05.822218 pycomplexheatmap-1.7.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-26 21:18:05.850218 pycomplexheatmap-1.7.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:18:05.822218 pycomplexheatmap-1.7.3/PyComplexHeatmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/PyComplexHeatmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 21:18:04.000000 pycomplexheatmap-1.7.3/PyComplexHeatmap/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65238 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/PyComplexHeatmap/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80351 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/PyComplexHeatmap/clustermap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7275 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/PyComplexHeatmap/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21688 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/PyComplexHeatmap/dotHeatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19871 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/PyComplexHeatmap/oncoPrint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27032 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/PyComplexHeatmap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:18:05.850218 pycomplexheatmap-1.7.3/PyComplexHeatmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-04-26 21:18:05.000000 pycomplexheatmap-1.7.3/PyComplexHeatmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-26 21:18:05.000000 pycomplexheatmap-1.7.3/PyComplexHeatmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:18:05.000000 pycomplexheatmap-1.7.3/PyComplexHeatmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-26 21:18:05.000000 pycomplexheatmap-1.7.3/PyComplexHeatmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8274 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:18:05.850218 pycomplexheatmap-1.7.3/comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)    88559 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/comparison/ComplexHeatmap.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   319414 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/comparison/ComplexHeatmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)   159236 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/comparison/PyComplexHeatmap.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   669615 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/comparison/PyComplexHeatmap.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/comparison/README.md
+-rw-r--r--   0 runner    (1001) docker     (127) 15584021 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/comparison/beta.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/comparison/compare.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/comparison/df_col.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2909164 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/comparison/df_row.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/comparison/heatmap.R
+-rw-r--r--   0 runner    (1001) docker     (127)   182760 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/comparison/heatmap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/comparison/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 21:18:05.850218 pycomplexheatmap-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-26 21:17:45.000000 pycomplexheatmap-1.7.3/setup.py
```

### Comparing `pycomplexheatmap-1.7.2/.github/FUNDING.yml` & `pycomplexheatmap-1.7.3/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/.github/ISSUE_TEMPLATE/bug_report.md` & `pycomplexheatmap-1.7.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/.github/ISSUE_TEMPLATE/feature_request.md` & `pycomplexheatmap-1.7.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/.github/workflows/python-publish.yml` & `pycomplexheatmap-1.7.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/CITATION.cff` & `pycomplexheatmap-1.7.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/LICENSE` & `pycomplexheatmap-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/PKG-INFO` & `pycomplexheatmap-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.7.2
+Version: 1.7.3
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Wubin Ding
```

### Comparing `pycomplexheatmap-1.7.2/PyComplexHeatmap/annotations.py` & `pycomplexheatmap-1.7.3/PyComplexHeatmap/annotations.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # -*- coding: utf-8 -*-
 # !/usr/bin/env python3
 import os, sys
 import pandas as pd
 import numpy as np
 import matplotlib
 import matplotlib.pylab as plt
-import matplotlib.image as mpimg
 from .utils import mm2inch
 from .utils import (
 	_calculate_luminance,
 	cluster_labels,
 	plot_legend_list,
 	define_cmap,
 	get_colormap,
@@ -107,14 +106,16 @@
 	def _height(self, height):
 		return 3 * self.ncols if height is None else height
 
 	def _set_default_plot_kws(self, plot_kws):
 		self.plot_kws = {} if plot_kws is None else plot_kws
 		self.plot_kws.setdefault("zorder", 10)
 
+	def set_orientation(self, orientation):
+		self.orientation = orientation
 	def update_plot_kws(self, plot_kws):
 		self.plot_kws.update(plot_kws)
 
 	def set_label(self, label):
 		self.label = label
 
 	def set_legend(self, legend):
@@ -140,26 +141,25 @@
 				subplot_ax.xaxis.tick_bottom()
 			subplot_ax.xaxis.set_label_position(self.label_side)
 			subplot_ax.xaxis.label.update(self.label_kws)
 			subplot_ax.xaxis.set_tick_params(self.ticklabels_kws)
 			# ax.yaxis.labelpad = self.labelpad
 			subplot_ax.yaxis.set_visible(False)
 			subplot_ax.xaxis.label.set_visible(False)
-			# subplot_ax.invert_yaxis()
 
 	def _check_cmap(self, cmap):
 		if cmap == "auto":
 			col = self.df.columns.tolist()[0]
 			if self.df.dtypes[col] == object:
 				if self.df[col].nunique() <= 10:
 					self.cmap = "Set1"
 				elif self.df[col].nunique() <= 20:
 					self.cmap = "tab20"
 				else:
-					self.cmap = "cmap50"
+					self.cmap = "random50"
 			elif self.df.dtypes[col] == float or self.df.dtypes[col] == int:
 				self.cmap = "jet"
 			else:
 				raise TypeError(
 					"Can not assign cmap for column %s, please specify cmap" % col
 				)
 		elif type(cmap) == str:
@@ -218,15 +218,19 @@
 		cc_list = list(self.color_dict.keys())  # column values
 		self.df[col] = self.df[col].map({v: cc_list.index(v) for v in cc_list})
 		self.cmap = matplotlib.colors.ListedColormap([self.color_dict[k] for k in cc_list])
 		self.plot_kws.setdefault("vmax", get_colormap(self.cmap).N - 1)
 		self.plot_kws.setdefault("vmin", 0)
 
 	def _type_specific_params(self):
-		pass
+		if self.ylim is None:
+			Max = np.nanmax(self.df.sum(axis=1).values)
+			Min = np.nanmin(self.df.sum(axis=1).values)
+			gap = Max - Min
+			self.ylim = [Min - 0.05 * gap, Max + 0.05 * gap]
 
 	def reorder(self, idx):
 		# Before plotting, df needs to be reordered according to the new clustered order.
 		# n_overlap = len(set(self.df.index.tolist()) & set(idx))
 		# if n_overlap == 0:
 		#     raise ValueError("The input idx is not consistent with the df.index")
 		# else:
@@ -326,14 +330,16 @@
 		col = self.df.columns.tolist()[0]
 		cc_list = list(self.color_dict.keys())  # column values
 		self.cc_list = cc_list
 		self.cmap = matplotlib.colors.ListedColormap(
 			[self.color_dict[k] for k in cc_list]
 		)
 
+	def _type_specific_params(self):
+		pass
 	def plot(self, ax=None, axis=1):
 		if hasattr(self.cmap, "N"):
 			vmax = self.cmap.N - 1
 		elif type(self.cmap) == str:
 			vmax = get_colormap(self.cmap).N - 1
 		else:
 			vmax = len(self.color_dict) - 1
@@ -344,29 +350,22 @@
 				self.plot_data.iloc[:, 0]
 				.map({v: self.cc_list.index(v) for v in self.cc_list})
 				.values
 			)
 		else:
 			mat = self.plot_data.values
 		matrix = mat.reshape(1, -1) if axis == 1 else mat.reshape(-1, 1)
-		# xlabel = None if axis == 1 else self.label
-		# ylabel = self.label if axis == 1 else None
-
-		# ax1 = heatmap(matrix, cmap=self.cmap, cbar=False, ax=ax, xlabel=xlabel, ylabel=ylabel,
-		#               xticklabels=False, yticklabels=False, **self.plot_kws)
 		ax1 = plot_heatmap(
 			matrix,
 			cmap=self.cmap,
 			ax=ax,
 			xticklabels=False,
 			yticklabels=False,
 			**self.plot_kws
-		)
-		# if axis==0:
-		#     ax1.invert_yaxis()
+		) #y will be inverted inside plot_heatmap
 		ax.tick_params(
 			axis="both",
 			which="both",
 			left=False,
 			right=False,
 			top=False,
 			bottom=False,
@@ -433,20 +432,21 @@
 	adjust_color: bool
 		When the luminance of the color is too high, use black color replace the original color. [True]
 	luminance: float
 		luminance values [0-1], used together with adjust_color, when the calculated luminance > luminance,
 		the color will be replaced with black. [0.5]
 	relpos: tuple
 		relpos passed to arrowprops in plt.annotate, tuple (x,y) means the arrow start point position relative to the
-		 label. default is (0, 0) if self.side == 'top' else (0, 1) for columns labels, (1, 1) if self.side == 'left'
+		 label. default is (0, 0) if self.orientation == 'top' else (0, 1) for columns labels, (1, 1) if self.orientation == 'left'
 		 else (0, 0) for rows labels.
 	plot_kws: dict
 		passed to plt.annotate, including annotation_clip, arrowprops and matplotlib.text.Text,
 		more information about arrowprops could be found in
-		matplotlib.patches.FancyArrowPatch
+		matplotlib.patches.FancyArrowPatch. For example, to remove arrow, just set
+		arrowprops = dict(visible=False,)
 
 	Returns
 	----------
 	Class AnnotationBase.
 
 	"""
 	def __init__(
@@ -483,32 +483,30 @@
 		self.frac = frac
 		self.relpos = relpos
 		self.annotated_texts = []
 
 	def _height(self, height):
 		return 4 if height is None else height
 
-	def set_side(self, side):
-		self.side = side
-
 	def set_plot_kws(self, axis):
 		shrink = 1  # 1 * mm2inch * 72  # 1mm -> points
 		if axis == 1:  # columns
-			relpos = (
-				(0, 0) if self.side == "top" else (0, 1)
-			)  # position to anchor, x: left -> right, y: down -> top
-			rotation = 90 if self.side == "top" else -90
+			# relpos = (
+			# 	(0, 0) if self.orientation == "up" else (0, 0)
+			# )  # position to anchor, x: left -> right, y: down -> top
+			relpos =(0,0)
+			rotation = 90 if self.orientation == "up" else -90
 			ha = "left"
 			va = "center"
 		else:
 			relpos = (
-				(1, 1) if self.side == "left" else (0, 0)
-			)  # (1, 1) if self.side == 'left' else (0, 0)
+				(1, 1) if self.orientation == "left" else (0, 0)
+			)  # (1, 1) if self.orientation == 'left' else (0, 0)
 			rotation = 0
-			ha = "right" if self.side == "left" else "left"
+			ha = "right" if self.orientation == "left" else "left"
 			va = "center"
 		# relpos: The exact starting point position of the arrow is defined by relpos. It's a tuple of relative
 		# coordinates of the text box, where (0, 0) is the lower left corner and (1, 1) is the upper right corner.
 		# Values <0 and >1 are supported and specify points outside the text box. By default (0.5, 0.5) the starting
 		# point is centered in the text box.
 		self.plot_kws.setdefault("rotation", rotation)
 		self.plot_kws.setdefault("ha", ha)
@@ -553,29 +551,32 @@
 		self.color_dict = self.colors
 		col = self.df.columns.tolist()[0]
 		cc_list = list(self.color_dict.keys())  # column values
 		self.cmap = matplotlib.colors.ListedColormap(
 			[self.color_dict[k] for k in cc_list]
 		)
 
+	def _type_specific_params(self):
+		pass
+
 	def plot(self, ax=None, axis=1):  # add self.gs,self.fig,self.ax,self.axes
 		self.axis = axis
-		if self.side is None:
+		if self.orientation is None:
 			ax_index = ax.figure.axes.index(ax)
 			ax_n = len(ax.figure.axes)
 			i = ax_index / ax_n
 			if axis == 1 and i <= 0.5:
-				side = "top"
+				orientation = "up"
 			elif axis == 1:
-				side = "bottom"
+				orientation = "down"
 			elif axis == 0 and i <= 0.5:
-				side = "left"
+				orientation = "left"
 			else:
-				side = "right"
-			self.side = side
+				orientation = "right"
+			self.orientation = orientation
 		self.set_plot_kws(axis)
 		if (
 			self.merge
 		):  # merge the adjacent ticklabels with the same text to one, return labels and mean x coordinates.
 			labels, ticks = cluster_labels(
 				self.plot_data.iloc[:, 0].values,
 				np.arange(0.5, self.nrows, 1),
@@ -583,75 +584,61 @@
 			)
 		else:
 			labels = self.plot_data.iloc[:, 0].values
 			ticks = np.arange(0.5, self.nrows, 1)
 		# labels are the merged labels, ticks are the merged mean x coordinates.
 
 		n = len(ticks)
-		text_height = (
-			self.height * mm2inch * ax.figure.dpi
-		)  # convert height (mm) to inch and to pixels.
-		# print(ax.figure.dpi,text_height)
-		text_y = text_height
-		if self.side == "bottom" or self.side == "left":
-			# when axis=0, there is an invertion for the x axes.
-			text_y = -1 * text_y
-			# bottom, y coordinate for text should be smaller than arrow start position (offset pixels)
-			# left, x coordinate for text should be smaller than arrow start pos.
-		# x,y are the coordinates where arrow starting from and x1,y1 is the end coordinates (text).
+		arrow_height = self.height * mm2inch * ax.figure.dpi # convert height (mm) to inch and to pixels.
+		text_y =  arrow_height
 		if axis == 1:
+			if self.orientation == "down":
+				# ax.invert_yaxis() # top -> bottom
+				text_y = -1 * arrow_height
 			ax.set_xticks(ticks=np.arange(0.5, self.nrows, 1))
-			x = ticks  # coordinate for the labels (text).
-			y = [0] * n if self.side == "top" else [1] * n  # position for line start on axes
+			x = ticks  # coordinate for the arrow start point
+			y = [0] * n if self.orientation == "up" else [1] * n  # position for line start on axes
 			if self.extend:
-				extend_pos = np.linspace(0, 1, n + 1)
-				x1 = [(extend_pos[i] + extend_pos[i - 1]) / 2 for i in range(1, n + 1)]
-				y1 = (
-					[1 + text_y / ax.figure.get_window_extent().height] * n
-					if self.side == "top"
-					else [text_y / ax.figure.get_window_extent().height] * n
-				)
+				extend_pos = np.linspace(0, 1, n + 1) #0,0.1,0.2,...0.9,1
+				x1 = [(extend_pos[i] + extend_pos[i - 1]) / 2 for i in range(1, n + 1)] #coordinates for text: 0.05,0.15..
+				y1 = [1] * n if self.orientation == "up" else [0] * n
 			else:
-				x1 = [0] * n
-				y1 = [text_y] * n
+				x1 = [0] * n #offset pixels
+				y1 = [text_y] * n #offset pixels
 		else:
-			# ax.invert_yaxis()
+			if self.orientation == "left":
+				# ax.invert_xaxis() # right -> left, will not affect ax.get_xaxis_transform()
+				text_y = -1 * arrow_height
 			ax.set_yticks(ticks=np.arange(0.5, self.nrows, 1))
-			labels=labels[::-1] #20231116, fix bug for right anno_label when extend=True
-			y = ticks[::-1] #Nov 16, fix bug for reverted right anno_label when extend=True
-			x = [1] * n if self.side == "left" else [0] * n #side=left, x axis <---
-			if self.extend:
-				extend_pos = np.linspace(0, 1, n + 1)
+			y=ticks
+			x = [1] * n if self.orientation == "left" else [0] * n #coordinate for start point, side=left, x axis <---
+			if self.extend: #ax.transAxes
+				# extend_pos = np.linspace(0, 1, n + 1)
+				extend_pos = np.linspace(1,0, n + 1) #y, top -> bottom
 				y1 = [(extend_pos[i] + extend_pos[i - 1]) / 2 for i in range(1, n + 1)]
-				x1 = (
-					[1 + text_y / ax.figure.get_window_extent().width] * n
-					if self.side == "right"
-					else [0 + text_y / ax.figure.get_window_extent().width] * n
-				)
-			else:
+				x1 = [1] * n if self.orientation == "right" else [0] * n
+			else: #offset pixels
 				y1 = [0] * n #vertical distance related to point (anno_simple)
 				x1 = [text_y] * n #horizonal distance related to point (anno_simple)
 		# angleA is the angle for the data point (clockwise), B is for text.
 		# https://matplotlib.org/stable/gallery/userdemo/connectionstyle_demo.html
 		xycoords = ax.get_xaxis_transform() if axis == 1 else ax.get_yaxis_transform()
-		# get_xaxis_transform: x is data coordinates,y is between [0,1]
+		# get_xaxis_transform: x is data coordinates,y is between [0,1], will not be affected by invert_xaxis()
 		if self.extend:
-			text_xycoords = (
-				ax.transAxes
-			)
+			text_xycoords = ax.transAxes #relative coordinates
 		else:
 			text_xycoords = "offset pixels"
 		if self.plot_kws["arrowprops"]["connectionstyle"] is None:
-			arm_height = text_height * self.frac
+			arm_height = arrow_height * self.frac
 			rad = 2  # arm_height / 10
-			if axis == 1 and self.side == "top":
+			if axis == 1 and self.orientation == "up":
 				angleA, angleB = (self.plot_kws["rotation"] - 180, 90)
-			elif axis == 1 and self.side == "bottom":
+			elif axis == 1 and self.orientation == "down":
 				angleA, angleB = (180 + self.plot_kws["rotation"], -90)
-			elif axis == 0 and self.side == "left":
+			elif axis == 0 and self.orientation == "left":
 				angleA, angleB = (self.plot_kws["rotation"], -180)
 			else:
 				angleA, angleB = (self.plot_kws["rotation"] - 180, 0)
 			connectionstyle = f"arc,angleA={angleA},angleB={angleB},armA={arm_height},armB={arm_height},rad={rad}"
 			self.plot_kws["arrowprops"]["connectionstyle"] = connectionstyle
 		# import pdb;
 		# pdb.set_trace()
@@ -662,36 +649,22 @@
 			if self.adjust_color:
 				lum = _calculate_luminance(color)
 				if lum > self.luminance:
 					color = "black"
 			self.plot_kws["arrowprops"]["color"] = color
 			annotated_text = ax.annotate(
 				text=t,
-				xy=(x_0, y_0),
-				xytext=(x_1, y_1),
+				xy=(x_0, y_0), #The point (x, y) to annotate
+				xytext=(x_1, y_1), #The position (x, y) to place the text at. The coordinate system is determined by textcoords.
 				xycoords=xycoords,
 				textcoords=text_xycoords,
 				color=color,
 				**self.plot_kws
 			)  # unit for shrinkA is point (1 point = 1/72 inches)
 			self.annotated_texts.append(annotated_text)
-		# _draw_figure(ax.figure)
-		# print('anno_label:',self.label_width,ax.get_window_extent().height,ax.get_window_extent().width)
-		# ax.tick_params(
-		#     axis="both",
-		#     which="both",
-		#     left=False,
-		#     right=False,
-		#     top=False,
-		#     bottom=False,
-		#     labeltop=False,
-		#     labelbottom=False,
-		#     labelleft=False,
-		#     labelright=False,
-		# )
 		ax.set_axis_off()
 		self.ax = ax
 		self.fig = self.ax.figure
 		return self.ax
 
 	def get_ticklabel_width(self):
 		hs = [text.get_window_extent().width for text in self.annotated_texts]
@@ -702,15 +675,15 @@
 
 
 # =============================================================================
 class anno_boxplot(AnnotationBase):
 	"""
 		annotate boxplots, all arguments are included in AnnotationBase,
 		plot_kws for anno_boxplot include showfliers, edgecolor, grid, medianlinecolor
-		width and other arguments passed to plt.boxplot.
+		width,zorder and other arguments passed to plt.boxplot.
 
 	Parameters
 	----------
 	"""
 
 	def _height(self, height):
 		return 10 if height is None else height
@@ -744,18 +717,14 @@
 				"Boxplot only support one string as colors now, if more colors are wanted, cmap can be specified."
 			)
 
 	def _calculate_cmap(self):
 		self.set_legend(False)
 		self.cmap = None
 
-	def _type_specific_params(self):
-		gap = self.df.max().max() - self.df.min().min()
-		self.ylim = [self.df.min().min() - 0.02 * gap, self.df.max().max() + 0.02 * gap]
-
 	def plot(self, ax=None, axis=1):  # add self.gs,self.fig,self.ax,self.axes
 		fig = ax.figure
 		if self.colors is None:  # calculate colors based on cmap
 			colors = [
 				get_colormap(self.cmap)(self.plot_data.loc[sampleID].mean())
 				for sampleID in self.plot_data.index.values
 			]
@@ -765,66 +734,67 @@
 		plot_kws = self.plot_kws.copy()
 		edgecolor = plot_kws.pop("edgecolor")
 		mlinecolor = plot_kws.pop("medianlinecolor")
 		grid = plot_kws.pop("grid")
 		# bp = ax.boxplot(self.plot_data.T.values, patch_artist=True,**self.plot_kws)
 		if axis == 1:
 			vert = True
-		else:
-			vert = False
-		if axis == 1:
 			ax.set_xticks(ticks=np.arange(0.5, self.nrows, 1))
 		else:
+			vert = False
 			ax.set_yticks(ticks=np.arange(0.5, self.nrows, 1))
 		# bp = self.plot_data.T.boxplot(ax=ax, patch_artist=True,vert=vert,return_type='dict',**self.plot_kws)
 		bp = ax.boxplot(
 			x=self.plot_data.T.values,
 			positions=np.arange(0.5, self.nrows, 1),
 			patch_artist=True,
-			vert=vert,
+			vert=vert, #If True, draws vertical boxes. If False, draw horizontal boxes
 			**plot_kws
 		)
 		if grid:
 			ax.grid(linestyle="--", zorder=-10)
 		for box, color in zip(bp["boxes"], colors):
 			box.set_facecolor(color)
 			box.set_edgecolor(edgecolor)
 		for median_line in bp["medians"]:
 			median_line.set_color(mlinecolor)
 		if axis == 1:
 			ax.set_xlim(0, self.nrows)
+			ax.set_ylim(*self.ylim)
 			ax.tick_params(
 				axis="both",
 				which="both",
 				top=False,
 				bottom=False,
 				labeltop=False,
 				labelbottom=False,
 			)
 		else:
 			ax.set_ylim(0, self.nrows)
+			ax.set_xlim(*self.ylim)
 			ax.tick_params(
 				axis="both",
 				which="both",
 				left=False,
 				right=False,
 				labelleft=False,
 				labelright=False,
 			)
-			ax.invert_xaxis()
+			# if self.orientation=='left':
+			# 	ax.invert_xaxis()
 		self.fig = fig
 		self.ax = ax
 		return self.ax
 
 
 # =============================================================================
 class anno_barplot(anno_boxplot):
 	"""
 	Annotate barplot, all arguments are included in AnnotationBase,
-		plot_kws for anno_boxplot include edgecolor, grid,
+		plot_kws for anno_boxplot include edgecolor, grid,align,zorder,
 		and other arguments passed to plt.barplot.
 	"""
 
 	def _set_default_plot_kws(self, plot_kws):
 		self.plot_kws = plot_kws if plot_kws is not None else {}
 		self.plot_kws.setdefault("edgecolor", "black")
 		self.plot_kws.setdefault("grid", False)
@@ -897,24 +867,23 @@
 		self.color_dict = color_dict
 
 	def _calculate_cmap(self):
 		self.cmap = None
 		# self.set_legend(False)
 
 	def _type_specific_params(self):
+		if self.ylim is None:
+			Max = np.nanmax(self.df.sum(axis=1).values)
+			Min = np.nanmin(self.df.sum(axis=1).values)
+			gap = Max - Min
+			self.ylim = [Min - 0.05 * gap, Max + 0.05 * gap]
 		if self.ncols > 1:
-			Max = self.df.max().max()
-			Min = self.df.min().min()
 			self.stacked = True
 		else:
-			Max = self.df.values.max()
-			Min = self.df.values.min()
 			self.stacked = False
-		gap = Max - Min
-		self.ylim = [Min - 0.02 * gap, Max + 0.02 * gap]
 
 	def plot(self, ax=None, axis=1):  # add self.gs,self.fig,self.ax,self.axes
 		if ax is None:
 			ax = plt.gca()
 		fig = ax.figure
 		plot_kws = self.plot_kws.copy()
 		grid = plot_kws.pop("grid", False)
@@ -933,36 +902,41 @@
 				ax.bar(
 					x=np.arange(0.5, self.nrows, 1),
 					height=self.plot_data[col].values,
 					bottom=base_coordinates,
 					color=color,
 					**plot_kws
 				)
+				ax.set_xlim(0, self.nrows)
+				ax.set_ylim(*self.ylim)
 			else:
 				ax.set_yticks(ticks=np.arange(0.5, self.nrows, 1))
 				ax.barh(
 					y=np.arange(0.5, self.nrows, 1),
 					width=self.plot_data[col].values,
 					left=base_coordinates,
 					color=color,
 					**plot_kws
 				)
+				ax.set_ylim(0, self.nrows)
+				ax.set_xlim(*self.ylim)
 			base_coordinates = self.plot_data[col].values + base_coordinates
 		# for patch in ax.patches:
 		#     patch.set_edgecolor(edgecolor)
 		if axis == 0:
 			ax.tick_params(
 				axis="both",
 				which="both",
 				left=False,
 				right=False,
 				labelleft=False,
 				labelright=False,
 			)
-			ax.invert_xaxis()
+			# if self.orientation == 'left':
+			# 	ax.invert_xaxis()
 		else:
 			ax.tick_params(
 				axis="both",
 				which="both",
 				top=False,
 				bottom=False,
 				labeltop=False,
@@ -973,15 +947,15 @@
 		return self.ax
 
 
 # =============================================================================
 class anno_scatterplot(anno_barplot):
 	"""
 	Annotate scatterplot, all arguments are included in AnnotationBase,
-		plot_kws for anno_boxplot include linewidths, grid, edgecolors
+		plot_kws for anno_scatterplot include linewidths, grid, edgecolors
 		and other arguments passed to plt.scatter.
 	"""
 
 	def _check_df(self, df):
 		if isinstance(df, pd.Series):
 			df = df.to_frame(name=df.name)
 		if isinstance(df, pd.DataFrame) and df.shape[1] != 1:
@@ -1019,18 +993,19 @@
 		self.colors = colors
 
 	def _calculate_cmap(self):
 		self.cmap = None
 		self.set_legend(False)
 
 	def _type_specific_params(self):
-		Max = self.df.values.max()
-		Min = self.df.values.min()
+		Max = np.nanmax(self.df.sum(axis=1).values)
+		Min = np.nanmin(self.df.sum(axis=1).values)
 		self.gap = Max - Min
-		self.ylim = [Min - 0.2 * self.gap, Max + 0.2 * self.gap]
+		if self.ylim is None:
+			self.ylim = [Min - 0.05 * self.gap, Max + 0.05 * self.gap]
 
 	def plot(self, ax=None, axis=1):  # add self.gs,self.fig,self.ax,self.axes
 		if ax is None:
 			ax = plt.gca()
 		fig = ax.figure
 		plot_kws = self.plot_kws.copy()
 		grid = plot_kws.pop("grid", False)
@@ -1058,24 +1033,29 @@
 			ax.set_yticks(ticks=np.arange(0.5, self.nrows, 1))
 			y = np.arange(0.5, self.nrows, 1)
 			x = values
 		c = self.plot_kws.get("c", colors)
 		s = self.plot_kws.get("s", self.s)
 		scatter_ax = ax.scatter(x=x, y=y, c=c, s=s, cmap=self.cmap, **plot_kws)
 		if axis == 0:
+			ax.set_xlim(0, self.nrows)
+			ax.set_ylim(*self.ylim)
 			ax.tick_params(
 				axis="both",
 				which="both",
 				left=False,
 				right=False,
 				labelleft=False,
 				labelright=False,
 			)
-			ax.invert_xaxis()
+			# if self.orientation == 'left':
+			# 	ax.invert_xaxis()
 		else:
+			ax.set_ylim(0, self.nrows)
+			ax.set_xlim(*self.ylim)
 			ax.tick_params(
 				axis="both",
 				which="both",
 				top=False,
 				bottom=False,
 				labeltop=False,
 				labelbottom=False,
@@ -1096,42 +1076,43 @@
 	border_color : int
 		color of border lines. black:0, white:255. Ignored when merge is True.
 	merge: bool
 		whether to merge the same clusters into one and show image only once.
 	merge_width: float
         width of image when merge is True
 		whether to merge the same clusters into one and show image only once.
+	rotate: int
+		Rotate the input images
+	mode: str
+		all possible mode to convert, between "L", "RGB" and "CMYK", 'RGBA', default is RGBA
 	"""
 	def __init__(
 		self,
 		df=None,
 		cmap=None,
 		colors=None,
 		border_width=1,
 		border_color=255,
         merge=False,
         merge_width=1,
-		height=None,
-		legend=True,
-		legend_kws=None,
+		rotate=None,
+		mode='RGBA',
 		**plot_kws
 	):
 		self.border_width = border_width
 		self.border_color = border_color
 		self.merge = merge
 		self.merge_width = merge_width
-
+		self.rotate=rotate
+		self.mode=mode
 		self.plot_kws = plot_kws
 		super().__init__(
 			df=df,
 			cmap=cmap,
 			colors=colors,
-			height=height,
-			legend=legend,
-			legend_kws=legend_kws,
 			**plot_kws
 		)
 
 	def _height(self, height):
 		return 10 if height is None else height
 
 	def _set_default_plot_kws(self, plot_kws):
@@ -1139,67 +1120,115 @@
 
 	def _calculate_colors(self):  # add self.color_dict (each col is a dict)
 		self.colors = None
 
 	def _check_cmap(self, cmap):
 		self.cmap = None 
 
+	def read_img(self,img_path=None,shape=None):
+		#import matplotlib.image as mpimg  # mpimg.imread
+		import PIL
+		import requests
+		from io import BytesIO
+		if pd.isna(img_path):
+			if shape is None:
+				return None
+			else:
+				new_shape=tuple([shape[1],shape[0]]+list(shape[2:]))
+				# print(shape, new_shape,type(shape), 'here')
+				return np.full(new_shape, self.border_color)
+		if os.path.exists(img_path):
+			image = PIL.Image.open(img_path) #mpimg.imread(img_path)
+		else: #remote file
+			response = requests.get(img_path)
+			# Open the image from bytes
+			image = PIL.Image.open(BytesIO(response.content))
+		if image.mode != self.mode:
+			image = image.convert(self.mode)
+		if not shape is None:
+			image=image.resize(shape[:2]) #width, height
+		if not self.rotate is None:
+			image=image.rotate(self.rotate)
+		# Convert the image to an array if needed
+		image = np.array(image)
+		return image
+
 	def _add_border(self, img, width=1, color=0, axis=1):
 		w = width
 		if axis == 1:
 			pad_width = ((0, 0), (w, w), (0, 0))
 		else:
 			pad_width = ((w, w), (0, 0), (0, 0))
 
 		bordered_img = np.pad(img, pad_width=pad_width, 
 						mode='constant', constant_values=color)
 		return bordered_img
 
-	def _check_imgfiles(self, imgfiles):
-		first_image = mpimg.imread(imgfiles[0])
-		height, width = first_image.shape[:2]
-		for imgfile in imgfiles[1:]:
-			img = mpimg.imread(imgfile)
-			assert img.shape[:2] == (height, width), \
-				f"The image size of {imgfile} differs. Reference: ({height}, {width}), Current image: {img.shape[:2]}"
-
+	def _type_specific_params(self):
+		pass
 	def plot(self, ax=None, axis=1):
 		if ax is None:
 			ax = plt.gca()
-		imgfiles = list(self.plot_data.iloc[:,0])
-		img_h = mpimg.imread(imgfiles[0]).shape[1]
+		if axis==1:
+			imgfiles = list(self.plot_data.iloc[:,0]) #[::-1] #fix bug for the inverted yaxis
+		else:
+			imgfiles = list(self.plot_data.iloc[:, 0])[::-1]
+		imgs = [self.read_img(img_path=imgfile) for imgfile in imgfiles]
+		shapes = [img.shape for img in imgs if not img is None]  # (height,width, channel)
+		if len(set(shapes)) > 1 or len(shapes) != len(imgs):  # None is in imgs
+			# resize the images to make sure all images have the same height and wdith
+			if len(shapes)>1:
+				shape = np.min(np.vstack(shapes), axis=0)  # height,width, channel; height, width,*channel
+			else:
+				shape=shapes[0]
+			new_shape = tuple([shape[1], shape[0]] + list(shape[2:]))
+			imgs = [self.read_img(img_path=imgfile, shape=new_shape) for imgfile in imgfiles]
+			shapes = [img.shape for img in imgs]
+		# for img in imgs:
+		# 	print(img.shape)
+		img_shape = shapes[0]
+		img_h = img_shape[0]  # shape: height,width, channel
+		img_w = img_shape[1]
 		if self.merge:
-			assert all(imgfile == imgfiles[0] for imgfile in imgfiles), "Not all file names in the list are identical"
-			imgs = mpimg.imread(imgfiles[0])
-			if axis==1:
+			origin = 'upper'
+			assert self.plot_data.iloc[:,0].dropna().nunique()==1, "Not all file names in the list are identical"
+			imgs = imgs[0]
+			if axis==1: #columns annotation
 				extent = [self.nrows/2-self.merge_width/2, self.nrows/2+self.merge_width/2, 0, img_h]
+				# floats (left, right, bottom, top), optional
+				# The bounding box in data coordinates that the image will fill
 			else:
-				extent = [0, img_h, self.nrows/2-self.merge_width/2, self.nrows/2+self.merge_width/2]
+				extent = [0, img_w, self.nrows/2-self.merge_width/2, self.nrows/2+self.merge_width/2]
 		else:
-			self._check_imgfiles(imgfiles)
 			if axis==1:
-				imgs = np.hstack(tuple([self._add_border(mpimg.imread(imgfile), 
-                                                width=self.border_width, color=self.border_color, axis=axis) \
-                            for imgfile in imgfiles]))
+				imgs = np.hstack(tuple([self._add_border(img,width=self.border_width,
+														 color=self.border_color, axis=axis) \
+                            for img in imgs]))
 				extent = [0, self.nrows, 0, img_h]
-			else:
-				imgs = np.vstack(tuple([self._add_border(mpimg.imread(imgfile), 
+				origin='upper'
+			else: #axis=0
+				# ax.invert_yaxis()  # y is shared, invert has no effect (only useful when anno_img on the most right side, main axes of sharey)
+				# in default, if orientation=='right', x direction is: left -> right, orient='left', right -> left
+				origin = 'lower'
+				if self.orientation=='left':
+					# ax.invert_xaxis() # no effect
+					ax.set_xlim(img_w,0)
+				# else:
+				# 	# ax.set_ylim(self.nrows,0)
+				imgs = np.vstack(tuple([self._add_border(img,
                                                 width=self.border_width, color=self.border_color, axis=axis) \
-                            for imgfile in imgfiles]))
-				extent = [0, img_h, 0, self.nrows]
-
+                            for img in imgs[::-1]])) #bottom -> up? to invert: up -> bottom
+				extent = [0,img_w, 0, self.nrows]
+		self.plot_kws.setdefault('origin',origin)
 		ax.imshow(imgs, aspect='auto', extent=extent, cmap=self.cmap, **self.plot_kws)
-
-		if axis==0:
-			ax.invert_yaxis()
-
-		ax.tick_params(labelbottom=False, labelleft=False, labelright=False, labeltop=False)
-		ax.tick_params(bottom=False, left=False, right=False, top=False)
+		ax.tick_params(axis='both',which='both',labelbottom=False, labelleft=False,
+								labelright=False, labeltop=False,
+					   			bottom=False, left=False,
+								right=False, top=False)
 		# ax.set_axis_off()
-
 		self.ax = ax
 		self.fig = self.ax.figure
 		return self.ax
 
 class anno_lineplot(anno_barplot):
 	"""
 	Annotate lineplot, all arguments are included in AnnotationBase,
@@ -1234,21 +1263,14 @@
 	def _calculate_colors(self):  # add self.color_dict (each col is a dict)
 		col_list = self.df.columns.tolist()
 		self.color_dict = {}
 		self.colors = [get_colormap(self.cmap)(col_list.index(v)) for v in col_list]
 		for v, color in zip(col_list, self.colors):
 			self.color_dict[v] = color
 
-	def _type_specific_params(self):
-		pass
-		# Max = self.df.values.max()
-		# Min = self.df.values.min()
-		# self.gap = Max - Min
-		# self.ylim = [Min - 0.2 * self.gap, Max + 0.2 * self.gap]
-
 	def plot(self, ax=None, axis=1):  # add self.gs,self.fig,self.ax,self.axes
 		if ax is None:
 			ax = plt.gca()
 		fig = ax.figure
 		plot_kws = self.plot_kws.copy()
 		grid = plot_kws.pop("grid", False)
 		if grid:
@@ -1259,41 +1281,48 @@
 				ax.set_xticks(ticks=np.arange(0.5, self.nrows, 1))
 				ax.plot(
 					np.arange(0.5, self.nrows, 1),
 					self.plot_data[col].values,
 					color=color,
 					**plot_kws
 				)
+				ax.set_xlim(0, self.nrows)
+				ax.set_ylim(*self.ylim)
 			else:
 				ax.set_yticks(ticks=np.arange(0.5, self.nrows, 1))
 				ax.plot(
 					self.plot_data[col].values,
                     np.arange(0.5, self.nrows, 1),
 					color=color,
 					**plot_kws
 				)
+				ax.set_ylim(0, self.nrows)
+				ax.set_xlim(*self.ylim)
 		if axis == 0:
 			ax.tick_params(
 				axis="both",
 				which="both",
 				left=False,
 				right=False,
 				labelleft=False,
 				labelright=False,
 			)
-			ax.invert_xaxis()
+			# if self.orientation == 'left':
+			# 	ax.invert_xaxis()
 		else:
 			ax.tick_params(
 				axis="both",
 				which="both",
 				top=False,
 				bottom=False,
 				labeltop=False,
 				labelbottom=False,
 			)
+			# if self.orientation=='down':
+			# 	ax.invert_yaxis()
 		self.fig = fig
 		self.ax = ax
 		return self.ax
 # =============================================================================
 class HeatmapAnnotation:
 	"""
 	Generate and plot heatmap annotations.
@@ -1421,20 +1450,14 @@
 		self.legend_width = legend_width
 		self.legend_hpad = legend_hpad
 		self.legend_vpad = legend_vpad
 		self.plot_legend = plot_legend
 		self.rasterized = rasterized
 		self.orientation = orientation
 		self.plot = plot
-		self.mapping_dict = {
-			"up": "top",
-			"down": "bottom",
-			"left": "left",
-			"right": "right",
-		}
 		if colors is None:
 			self._check_cmap(cmap)
 			self.colors = None
 		else:
 			self._check_colors(colors)
 		self._process_data()
 		self._heights()
@@ -1478,15 +1501,15 @@
 			for col in self.df.columns:
 				if self.df.dtypes[col] == object:
 					if self.df[col].nunique() <= 10:
 						self.cmap[col] = "Set1"
 					elif self.df[col].nunique() <= 20:
 						self.cmap[col] = "tab20"
 					else:
-						self.cmap[col] = "cmap50"
+						self.cmap[col] = "random50"
 				elif self.df.dtypes[col] == float or self.df.dtypes[col] == int:
 					self.cmap[col] = "jet"
 				else:
 					raise TypeError(
 						"Can not assign cmap for column %s, please specify cmap" % col
 					)
 		elif type(cmap) == str:
@@ -1529,14 +1552,15 @@
 					plot_kws.setdefault("cmap", self.cmap[col])  #
 				else:
 					plot_kws.setdefault("colors", self.colors[col])
 				anno1 = anno_simple(
 					self.df[col], legend=self.legend.get(col, False), **plot_kws
 				)
 				anno1.set_label(col)
+				anno1.set_orientation(self.orientation)
 				self.annotations.append(anno1)
 		elif len(self.args) > 0:
 			# print(self.args)
 			self.labels = []
 			for arg in self.args:
 				# print(arg)
 				ann = self.args[arg]
@@ -1570,17 +1594,16 @@
 							self.orientation = "up"
 						elif self.axis == 1:
 							self.orientation = "down"
 						elif self.axis == 0 and len(self.labels) == 0:
 							self.orientation = "left"
 						elif self.axis == 0:
 							self.orientation = "right"
-					if type(ann) == anno_label:
-						ann.set_side(self.mapping_dict[self.orientation])
 				self.labels.append(arg)
+				ann.set_orientation(self.orientation)
 
 	def _set_orentation(self, orientation):
 		if self.orientation is None:
 			self.orientation = orientation
 
 	def _heights(self):
 		self.heights = [ann.height for ann in self.annotations]
@@ -1641,15 +1664,15 @@
 					right=False,
 					labelright=False,
 				)
 				self.axes[i, 0].set_ylabel(self.annotations[i].label)
 				self.axes[i, 0].yaxis.set_label_position(self.label_side)
 				self.axes[i, 0].yaxis.label.update(self.label_kws)
 				# self.axes[i, -1].yaxis.tick_right()  # ticks
-				if type(self.annotations[i]) != anno_simple:
+				if type(self.annotations[i]) not in [anno_simple,anno_img]:
 					self.axes[i, -1].yaxis.set_visible(True)
 					self.axes[i, -1].tick_params(
 						axis="y", which="both", right=True, labelright=True
 					)
 					self.axes[i, -1].yaxis.set_tick_params(**self.ticklabels_kws)
 		elif self.axis == 1 and self.label_side == "right":
 			self.ax.yaxis.tick_left()
@@ -1664,39 +1687,39 @@
 					right=False,
 					labelright=False,
 				)
 				self.axes[i, -1].set_ylabel(self.annotations[i].label)
 				self.axes[i, -1].yaxis.set_label_position(self.label_side)
 				self.axes[i, -1].yaxis.label.update(self.label_kws)
 				# self.axes[i, 0].yaxis.tick_left()  # ticks
-				if type(self.annotations[i]) != anno_simple:
+				if type(self.annotations[i]) not in [anno_simple,anno_img]:
 					self.axes[i, 0].yaxis.set_visible(True)
 					self.axes[i, 0].tick_params(
 						axis="y", which="both", left=True, labelleft=True
 					)
 					self.axes[i, 0].yaxis.set_tick_params(**self.ticklabels_kws)
 		elif self.axis == 0 and self.label_side == "top":
 			self.ax.xaxis.tick_bottom()
 			for j in range(self.axes.shape[1]):
-				self.axes[0, j].xaxis.set_visible(True)
+				self.axes[0, j].xaxis.set_visible(True) #0, the top axes
 				self.axes[0, j].xaxis.label.set_visible(True)
 				self.axes[0, j].tick_params(
 					axis="x",
 					which="both",
 					top=False,
 					labeltop=False,
 					bottom=False,
 					labelbottom=False,
 				)
 				self.axes[0, j].set_xlabel(self.annotations[j].label)
 				self.axes[0, j].xaxis.set_label_position(self.label_side)
 				self.axes[0, j].xaxis.label.update(self.label_kws)
 				# self.axes[-1, j].xaxis.tick_bottom()  # ticks
-				if type(self.annotations[j]) != anno_simple:
-					self.axes[-1, j].xaxis.set_visible(True)
+				if type(self.annotations[j]) not in [anno_simple,anno_img]:
+					self.axes[-1, j].xaxis.set_visible(True) # show ticks
 					self.axes[-1, j].tick_params(
 						axis="x", which="both", bottom=True, labelbottom=True
 					)
 					self.axes[-1, j].xaxis.set_tick_params(**self.ticklabels_kws)
 		elif self.axis == 0 and self.label_side == "bottom":
 			self.ax.xaxis.tick_top()
 			for j in range(self.axes.shape[1]):
@@ -1710,15 +1733,15 @@
 					bottom=False,
 					labelbottom=False,
 				)
 				self.axes[-1, j].set_xlabel(self.annotations[j].label)
 				self.axes[-1, j].xaxis.set_label_position(self.label_side)
 				self.axes[-1, j].xaxis.label.update(self.label_kws)
 				# self.axes[0, j].xaxis.tick_top()  # ticks
-				if type(self.annotations[j]) != anno_simple:
+				if type(self.annotations[j]) not in [anno_simple,anno_img]:
 					self.axes[0, j].xaxis.set_visible(True)
 					self.axes[0, j].tick_params(
 						axis="x", which="both", top=True, labeltop=True
 					)
 					self.axes[0, j].xaxis.set_tick_params(**self.ticklabels_kws)
 
 	def collect_legends(self):
@@ -1874,25 +1897,23 @@
 				subplot_spec=subplot_spec,
 				height_ratios=height_ratios,
 				width_ratios=width_ratios,
 			)
 		self.axes = np.empty(shape=(nrows, ncols), dtype=object)
 		self.fig = self.ax.figure
 		self.ax.set_axis_off()
-		# self.ax.margins(x=0, y=0)
-		for j, idx in enumerate(idxs):
-			for i, ann in enumerate(self.annotations):
-				# print(i,j,ann.label)
+		for j, idx in enumerate(idxs): # columns if axis=1, rows if axis=0
+			for i, ann in enumerate(self.annotations): #rows for axis=1, columns if axis=0
 				# axis=1: left -> right, axis=0: bottom -> top.
-				# idx=idx[::-1] if self.axis==0 else idx #1 for cols, 0 for rows.
 				ann.reorder(idx)
 				gs = self.gs[i, j] if self.axis == 1 else self.gs[j, i]
-				sharex = self.axes[0, j] if self.axis == 1 else self.axes[0, i]
-				sharey = self.axes[i, 0] if self.axis == 1 else self.axes[j, 0]
-				# sharex,sharey=None,None
+				# sharex = self.axes[0, j] if self.axis == 1 else self.axes[0, i]
+				# sharey = self.axes[i, 0] if self.axis == 1 else self.axes[j, 0]
+				sharex = self.axes[0, j] if self.axis == 1 else None
+				sharey = None if self.axis == 1 else self.axes[j, 0]
 				ax1 = self.ax.figure.add_subplot(gs, sharex=sharex, sharey=sharey)
 				if self.axis == 1:
 					ax1.set_xlim([0, len(idx)])
 				else:
 					ax1.set_ylim([0, len(idx)])
 				ann.plot(ax=ax1, axis=self.axis) #subplot_spec=gs
 				if self.axis == 1:
@@ -1913,15 +1934,15 @@
 					ax1.xaxis.label.set_visible(False)
 					ax1.tick_params(
 						top=False, bottom=False, labeltop=False, labelbottom=False
 					)
 					self.ax.spines["left"].set_visible(False)
 					self.ax.spines["right"].set_visible(False)
 					self.axes[j, i] = ax1
-					if self.orientation == "right":
+					if self.orientation == "left":
 						ax1.invert_xaxis()
 
 		self.set_axes_kws()
 		self.legend_list = None
 		if self.plot and self.plot_legend:
 			self.plot_legends(ax=self.ax)
 		# _draw_figure(self.ax.figure)
```

### Comparing `pycomplexheatmap-1.7.2/PyComplexHeatmap/clustermap.py` & `pycomplexheatmap-1.7.3/PyComplexHeatmap/clustermap.py`

 * *Files 1% similar despite different names*

```diff
@@ -674,15 +674,15 @@
 		kwargs.setdefault("vmax", vmax)
 
 	# Draw the heatmap
 	mesh = ax.pcolormesh(plot_data, cmap=cmap, **kwargs)
 	# Set the axis limits
 	ax.set(xlim=(0, data.shape[1]), ylim=(0, data.shape[0]))
 	# Invert the y axis to show the plot in matrix form
-	ax.invert_yaxis()  # from top to bottom
+	ax.invert_yaxis()  # from top to bottom, left to right
 
 	# Add row and column labels
 	if isinstance(xticks, str) and xticks == "auto":
 		xticks, xticklabels = _auto_ticks(ax, xticklabels, 0)
 
 	if isinstance(yticks, str) and yticks == "auto":
 		yticks, yticklabels = _auto_ticks(ax, yticklabels, 1)
@@ -846,17 +846,16 @@
 				msg = (
 					"Clustering large matrix with scipy. Installing "
 					"`fastcluster` may give better performance."
 				)
 				warnings.warn(msg)
 		return self._calculate_linkage_scipy()
 
-	def calculate_dendrogram(
-		self,
-	):  # Z (linkage) shape = (n,4), then dendrogram icoord shape = (n,4)
+	def calculate_dendrogram(self,):
+		# Z (linkage) shape = (n,4), then dendrogram icoord shape = (n,4)
 		return hierarchy.dendrogram(
 			self.linkage,
 			no_plot=True,
 			labels=self.data.index.tolist(),
 			get_leaves=True,
 			**self.dendrogram_kws
 		)  # color_threshold=-np.inf,
@@ -956,24 +955,23 @@
 			colors = [colors] * len(self.dendrogram["ivl"])
 		for (x, y), color in zip(coords, colors):
 			ax.plot(x, y, color=color, **tree_kws)
 		# if self.axis==1:
 		#     ax.scatter(self.root_x, root_y,c='red',s=1)
 		# else:
 		#     ax.scatter(root_y,self.root_x, c='red', s=1)
-		if self.axis==0:
-			ax.invert_yaxis()  # 20230227 fix the bug for inverse order of row dendrogram
 
-		if self.rotate:  # horizontal; in default, no rotate
+		if self.rotate:  # if axis==0, rotate should be set to True
 			ax.yaxis.set_ticks_position("right")
 			ax.set_ylim(0, self.icoord_max)
 			ax.set_xlim(0, root_y)
-			ax.invert_xaxis()
-			ax.invert_yaxis()
-		else:  # vertical
+			# before rotate: left -> right, bottom -> top
+			ax.invert_xaxis() # right -> left, root on the left, leaf on the right.
+			ax.invert_yaxis() # top -> bottom, consistent with heatmap pcolormesh
+		else:  # vertical,  left -> right, bototom -> top. y for leaf is 0, y_root is larger.
 			ax.set_xlim(0, self.icoord_max)
 			ax.set_ylim(0, root_y)
 		despine(ax=ax, bottom=True, left=True)
 		ax.set(
 			xticks=self.xticks,
 			yticks=self.yticks,
 			xlabel=self.xlabel,
@@ -2042,16 +2040,14 @@
 					labelbottom=False,
 				)
 
 	def set_axes_labels_kws(self):
 		# ax.set_xticks(ticks=np.arange(1, self.nrows + 1, 1), labels=self.plot_data.index.tolist())
 		self.ax_heatmap.yaxis.set_tick_params(**self.yticklabels_kws)
 		self.ax_heatmap.xaxis.set_tick_params(**self.xticklabels_kws)
-		# self.ax_heatmap.tick_params(axis='both', which='both',
-		#                             left=False, right=False, top=False, bottom=False)
 		self.yticklabels = []
 		self.xticklabels = []
 		if (
 			self.show_rownames
 			and self.left_annotation is None
 			and not self.row_dendrogram
 		) and (
@@ -2217,14 +2213,15 @@
 			# 	"vmax", np.nanmax(self.data2d[self.data2d != np.inf])
 			# )
 			# vmin = self.kwargs.get(
 			# 	"vmin", np.nanmin(self.data2d[self.data2d != -np.inf])
 			# )
 			self.legend_kws.setdefault("vmin", self.kwargs.get('vmin')) #round(vmin, 2))
 			self.legend_kws.setdefault("vmax", self.kwargs.get('vmax')) #round(vmax, 2))
+			self.legend_kws.setdefault("center", self.kwargs.get('center',None))
 			self.legend_list.append([self.cmap, self.label, self.legend_kws, 4, "cmap"])
 			if len(self.yticklabels) > 0 and self.row_names_side == "right":
 				max_yticklabel_w = max(
 					[label.get_window_extent().width for label in self.yticklabels]
 				)
 			else:
 				max_yticklabel_w = 0
```

### Comparing `pycomplexheatmap-1.7.2/PyComplexHeatmap/dotHeatmap.py` & `pycomplexheatmap-1.7.3/PyComplexHeatmap/dotHeatmap.py`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/PyComplexHeatmap/oncoPrint.py` & `pycomplexheatmap-1.7.3/PyComplexHeatmap/oncoPrint.py`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/PyComplexHeatmap/utils.py` & `pycomplexheatmap-1.7.3/PyComplexHeatmap/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,18 +508,25 @@
 	cbar_kws.setdefault("fraction", 1)
 	cbar_kws.setdefault("shrink", 1)
 	cbar_kws.setdefault("pad", 0)
 	vmax = cbar_kws.pop("vmax", 1)
 	vmin = cbar_kws.pop("vmin", 0)
 	# print(vmin,vmax,'vmax,vmin')
 	cax.set_ylim([vmin, vmax])
-	cbar_kws.setdefault("ticks", [vmin, (vmax + vmin) / 2, vmax])
-	m = plt.cm.ScalarMappable(
-		norm=matplotlib.colors.Normalize(vmin=vmin, vmax=vmax), cmap=cmap
-	)
+	vcenter= (vmax + vmin) / 2
+	center=cbar_kws.pop("center",None)
+	if center is None:
+		cbar_kws.setdefault("ticks", [vmin, vcenter, vmax])
+		m = plt.cm.ScalarMappable(
+			norm=matplotlib.colors.Normalize(vmin=vmin, vmax=vmax), cmap=cmap
+		)
+	else:
+		m = plt.cm.ScalarMappable(
+			norm=matplotlib.colors.CenteredNorm(vcenter=center), cmap=cmap
+		)
 	cax.yaxis.set_label_position(label_side)
 	cax.yaxis.set_ticks_position(label_side)
 	cbar = ax.figure.colorbar(m, cax=cax, **cbar_kws)  # use_gridspec=True
 	# cbar.outline.set_color('white')
 	# cbar.outline.set_linewidth(2)
 	# cbar.dividers.set_color('red')
 	# cbar.dividers.set_linewidth(2)
```

### Comparing `pycomplexheatmap-1.7.2/PyComplexHeatmap.egg-info/PKG-INFO` & `pycomplexheatmap-1.7.3/PyComplexHeatmap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyComplexHeatmap
-Version: 1.7.2
+Version: 1.7.3
 Summary: A python package to plot complex heatmap
 Home-page: https://github.com/DingWB/PyComplexHeatmap
 Author: Wubin Ding
 Author-email: Wubin Ding <ding.wu.bin.gm@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Wubin Ding
```

### Comparing `pycomplexheatmap-1.7.2/PyComplexHeatmap.egg-info/SOURCES.txt` & `pycomplexheatmap-1.7.3/PyComplexHeatmap.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 .github/workflows/python-publish.yml
 PyComplexHeatmap/__init__.py
 PyComplexHeatmap/_version.py
 PyComplexHeatmap/annotations.py
 PyComplexHeatmap/clustermap.py
 PyComplexHeatmap/colors.py
 PyComplexHeatmap/dotHeatmap.py
-PyComplexHeatmap/example.py
 PyComplexHeatmap/oncoPrint.py
 PyComplexHeatmap/utils.py
 PyComplexHeatmap.egg-info/PKG-INFO
 PyComplexHeatmap.egg-info/SOURCES.txt
 PyComplexHeatmap.egg-info/dependency_links.txt
 PyComplexHeatmap.egg-info/top_level.txt
 comparison/ComplexHeatmap.pdf
```

### Comparing `pycomplexheatmap-1.7.2/README.md` & `pycomplexheatmap-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/comparison/ComplexHeatmap.pdf` & `pycomplexheatmap-1.7.3/comparison/ComplexHeatmap.pdf`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/comparison/ComplexHeatmap.png` & `pycomplexheatmap-1.7.3/comparison/ComplexHeatmap.png`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/comparison/PyComplexHeatmap.pdf` & `pycomplexheatmap-1.7.3/comparison/PyComplexHeatmap.pdf`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/comparison/PyComplexHeatmap.png` & `pycomplexheatmap-1.7.3/comparison/PyComplexHeatmap.png`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/comparison/README.md` & `pycomplexheatmap-1.7.3/comparison/README.md`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/comparison/beta.csv` & `pycomplexheatmap-1.7.3/comparison/beta.csv`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/comparison/df_col.csv` & `pycomplexheatmap-1.7.3/comparison/df_col.csv`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/comparison/df_row.csv` & `pycomplexheatmap-1.7.3/comparison/df_row.csv`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/comparison/heatmap.R` & `pycomplexheatmap-1.7.3/comparison/heatmap.R`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/comparison/heatmap.ipynb` & `pycomplexheatmap-1.7.3/comparison/heatmap.ipynb`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/comparison/heatmap.py` & `pycomplexheatmap-1.7.3/comparison/heatmap.py`

 * *Files identical despite different names*

### Comparing `pycomplexheatmap-1.7.2/pyproject.toml` & `pycomplexheatmap-1.7.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["setuptools>=61.0","matplotlib<3.8.0","numpy","pandas>=1.3.5", "scipy","fastcluster","wheel","setuptools_scm[toml]>=6.2"]
+requires = ["setuptools>=61.0","matplotlib<3.8.0","numpy","pandas>=1.3.5", "scipy","fastcluster","wheel","setuptools_scm[toml]>=6.2","palettable"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 version_scheme = "guess-next-dev"
 write_to = 'PyComplexHeatmap/_version.py'
 
 [project]
```

### Comparing `pycomplexheatmap-1.7.2/setup.py` & `pycomplexheatmap-1.7.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,13 +24,13 @@
     description="A Python package to plot complex heatmap",
     # long_description="#PyComplexHeatmap\n##Documentation:https://dingwb.github.io/PyComplexHeatmap/build/html/index.html",
     # long_description_content_type='text/markdown',
     author="Wubin Ding",
     author_email="ding.wu.bin.gm@gmail.com",
     url="https://github.com/DingWB/PyComplexHeatmap",
     packages=["PyComplexHeatmap"],  # src
-    install_requires=["matplotlib<3.8.0","numpy","pandas>=1.3.5", "scipy","fastcluster"],
+    install_requires=["matplotlib<3.8.0","numpy","pandas>=1.3.5", "scipy","fastcluster","palettable"],
     include_package_data=True,
 )
 # rm -rf dist && rm -rf PyComplexHeatmap/PyComplexHeatmap.egg-info/
 # python setup.py sdist bdist_wheel
 # twine upload dist/*
```

