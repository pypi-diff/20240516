# Comparing `tmp/idf_analysis-0.2.5.tar.gz` & `tmp/idf_analysis-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf_analysis-0.2.5.tar", last modified: Mon May 13 09:27:49 2024, max compression
+gzip compressed data, was "idf_analysis-0.2.6.tar", last modified: Thu May 16 16:18:30 2024, max compression
```

## Comparing `idf_analysis-0.2.5.tar` & `idf_analysis-0.2.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:27:49.554271 idf_analysis-0.2.5/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       98 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    16171 2024-05-13 09:27:49.554271 idf_analysis-0.2.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14543 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:27:49.554271 idf_analysis-0.2.5/idf_analysis/
--rw-r--r--   0 root         (0) root         (0)      624 2024-05-13 09:27:46.000000 idf_analysis-0.2.5/idf_analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      245 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/__main__.py
--rw-r--r--   0 root         (0) root         (0)      254 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/_console_script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:27:49.554271 idf_analysis-0.2.5/idf_analysis/approaches/
--rw-r--r--   0 root         (0) root         (0)      283 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/approaches/ATV-A_121.yaml
--rw-r--r--   0 root         (0) root         (0)      239 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/approaches/KOSTRA.yaml
--rw-r--r--   0 root         (0) root         (0)      241 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/approaches/convective_vs_advective.yaml
--rw-r--r--   0 root         (0) root         (0)     4309 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/arg_parser.py
--rw-r--r--   0 root         (0) root         (0)     1941 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/definitions.py
--rw-r--r--   0 root         (0) root         (0)     8024 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/event_series_analysis.py
--rw-r--r--   0 root         (0) root         (0)    24196 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/heavy_rainfall_index.py
--rw-r--r--   0 root         (0) root         (0)    12585 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/idf_backend.py
--rw-r--r--   0 root         (0) root         (0)    36166 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/idf_class.py
--rw-r--r--   0 root         (0) root         (0)     2546 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/in_out.py
--rw-r--r--   0 root         (0) root         (0)     5113 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/interim_result_plots.py
--rw-r--r--   0 root         (0) root         (0)     6920 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/little_helpers.py
--rw-r--r--   0 root         (0) root         (0)     3953 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/parameter_formulation_class.py
--rw-r--r--   0 root         (0) root         (0)     3750 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/parameter_formulations.py
--rw-r--r--   0 root         (0) root         (0)     4083 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/plot_helpers.py
--rw-r--r--   0 root         (0) root         (0)     6661 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/sww_utils.py
--rw-r--r--   0 root         (0) root         (0)     4988 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/synthetic_rainseries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:27:49.554271 idf_analysis-0.2.5/idf_analysis.egg-info/
--rw-r--r--   0 root         (0) root         (0)    16171 2024-05-13 09:27:49.000000 idf_analysis-0.2.5/idf_analysis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      931 2024-05-13 09:27:49.000000 idf_analysis-0.2.5/idf_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 09:27:49.000000 idf_analysis-0.2.5/idf_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2024-05-13 09:27:49.000000 idf_analysis-0.2.5/idf_analysis.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      147 2024-05-13 09:27:49.000000 idf_analysis-0.2.5/idf_analysis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-13 09:27:49.000000 idf_analysis-0.2.5/idf_analysis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2440 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 09:27:49.554271 idf_analysis-0.2.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:18:30.456229 idf_analysis-0.2.6/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       98 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    16171 2024-05-16 16:18:30.456229 idf_analysis-0.2.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14543 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:18:30.452229 idf_analysis-0.2.6/idf_analysis/
+-rw-r--r--   0 root         (0) root         (0)      624 2024-05-16 16:18:27.000000 idf_analysis-0.2.6/idf_analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      245 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      254 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/_console_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:18:30.456229 idf_analysis-0.2.6/idf_analysis/approaches/
+-rw-r--r--   0 root         (0) root         (0)      283 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/approaches/ATV-A_121.yaml
+-rw-r--r--   0 root         (0) root         (0)      239 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/approaches/KOSTRA.yaml
+-rw-r--r--   0 root         (0) root         (0)      241 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/approaches/convective_vs_advective.yaml
+-rw-r--r--   0 root         (0) root         (0)     4309 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/arg_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/definitions.py
+-rw-r--r--   0 root         (0) root         (0)     8024 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/event_series_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    24196 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/heavy_rainfall_index.py
+-rw-r--r--   0 root         (0) root         (0)    12585 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/idf_backend.py
+-rw-r--r--   0 root         (0) root         (0)    36166 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/idf_class.py
+-rw-r--r--   0 root         (0) root         (0)     2546 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/in_out.py
+-rw-r--r--   0 root         (0) root         (0)     5113 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/interim_result_plots.py
+-rw-r--r--   0 root         (0) root         (0)     6920 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/little_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     3953 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/parameter_formulation_class.py
+-rw-r--r--   0 root         (0) root         (0)     3750 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/parameter_formulations.py
+-rw-r--r--   0 root         (0) root         (0)     4189 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/plot_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     6835 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/sww_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4988 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/idf_analysis/synthetic_rainseries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 16:18:30.456229 idf_analysis-0.2.6/idf_analysis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16171 2024-05-16 16:18:30.000000 idf_analysis-0.2.6/idf_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      931 2024-05-16 16:18:30.000000 idf_analysis-0.2.6/idf_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 16:18:30.000000 idf_analysis-0.2.6/idf_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-16 16:18:30.000000 idf_analysis-0.2.6/idf_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      147 2024-05-16 16:18:30.000000 idf_analysis-0.2.6/idf_analysis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-16 16:18:30.000000 idf_analysis-0.2.6/idf_analysis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 16:18:30.456229 idf_analysis-0.2.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 16:18:26.000000 idf_analysis-0.2.6/setup.py
```

### Comparing `idf_analysis-0.2.5/LICENSE` & `idf_analysis-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `idf_analysis-0.2.5/PKG-INFO` & `idf_analysis-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-analysis
-Version: 0.2.5
+Version: 0.2.6
 Summary: heavy rain as a function of the duration and the return period acc. to DWA-A 531 (2012)
 Author-email: Markus Pichler <markus.pichler@tugraz.at>
 License: MIT
 Project-URL: Documentation, https://markuspic.github.io/intensity_duration_frequency_analysis/
 Project-URL: Changelog, https://github.com/MarkusPic/intensity_duration_frequency_analysis/-/blob/master/CHANGELOG.md
 Project-URL: homepage, https://github.com/MarkusPic/intensity_duration_frequency_analysis
 Keywords: duration,analysis,rainfall,dwd,idf,measurement-data,precipitation,kostra,dwa,heavy-rain,intensity-duration-frequency,design-rainfall,duration-steps,return-period,dwa-a-531
```

### Comparing `idf_analysis-0.2.5/README.md` & `idf_analysis-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `idf_analysis-0.2.5/idf_analysis/__init__.py` & `idf_analysis-0.2.6/idf_analysis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Markus Pichler"
 __credits__ = ["Markus Pichler"]
 __maintainer__ = "Markus Pichler"
 __email__ = "markus.pichler@tugraz.at"
-__version__ = '0.2.5'
+__version__ = '0.2.6'
 __license__ = "MIT"
 
 from .idf_class import IntensityDurationFrequencyAnalyse, SERIES, METHOD
 
 """
 Heavy rain as a function of the duration and the return period acc. to DWA-A 531 (2012)
```

### Comparing `idf_analysis-0.2.5/idf_analysis/arg_parser.py` & `idf_analysis-0.2.6/idf_analysis/arg_parser.py`

 * *Files identical despite different names*

### Comparing `idf_analysis-0.2.5/idf_analysis/definitions.py` & `idf_analysis-0.2.6/idf_analysis/definitions.py`

 * *Files identical despite different names*

### Comparing `idf_analysis-0.2.5/idf_analysis/event_series_analysis.py` & `idf_analysis-0.2.6/idf_analysis/event_series_analysis.py`

 * *Files identical despite different names*

### Comparing `idf_analysis-0.2.5/idf_analysis/heavy_rainfall_index.py` & `idf_analysis-0.2.6/idf_analysis/heavy_rainfall_index.py`

 * *Files identical despite different names*

### Comparing `idf_analysis-0.2.5/idf_analysis/idf_backend.py` & `idf_analysis-0.2.6/idf_analysis/idf_backend.py`

 * *Files identical despite different names*

### Comparing `idf_analysis-0.2.5/idf_analysis/idf_class.py` & `idf_analysis-0.2.6/idf_analysis/idf_class.py`

 * *Files identical despite different names*

### Comparing `idf_analysis-0.2.5/idf_analysis/in_out.py` & `idf_analysis-0.2.6/idf_analysis/in_out.py`

 * *Files identical despite different names*

### Comparing `idf_analysis-0.2.5/idf_analysis/interim_result_plots.py` & `idf_analysis-0.2.6/idf_analysis/interim_result_plots.py`

 * *Files identical despite different names*

### Comparing `idf_analysis-0.2.5/idf_analysis/little_helpers.py` & `idf_analysis-0.2.6/idf_analysis/little_helpers.py`

 * *Files identical despite different names*

### Comparing `idf_analysis-0.2.5/idf_analysis/parameter_formulation_class.py` & `idf_analysis-0.2.6/idf_analysis/parameter_formulation_class.py`

 * *Files identical despite different names*

### Comparing `idf_analysis-0.2.5/idf_analysis/parameter_formulations.py` & `idf_analysis-0.2.6/idf_analysis/parameter_formulations.py`

 * *Files identical despite different names*

### Comparing `idf_analysis-0.2.5/idf_analysis/plot_helpers.py` & `idf_analysis-0.2.6/idf_analysis/plot_helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,18 @@
 
     ax.set_yticklabels(duration_steps_readable(idf_table.columns), minor=True)
     ax.set_yticklabels([''] * duration_size, minor=False)
     ax.set_ylabel('duration of the design rainfall')
 
     # for the relative start time
     freq = guess_freq(idf_table.index)
-    start_period = idf_table.index[0].to_period(freq).ordinal
+    start_dt = idf_table.index[0]
+    if start_dt.tzinfo is not None:
+        start_dt = start_dt.tz_localize(None)
+    start_period = start_dt.to_period(freq).ordinal
 
     # idf_table.index = idf_table.index - idf_table.index[0]
 
     min_duration = pd.Timedelta(minutes=1)
 
     for hi, d in enumerate(idf_table.columns):
         tn = idf_table[d]
```

### Comparing `idf_analysis-0.2.5/idf_analysis/sww_utils.py` & `idf_analysis-0.2.6/idf_analysis/sww_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,17 @@
         color (str):
         reverse (bool):
         step (str):  'mid' 'post' pre'
 
     Returns:
         matplotlib.axes.Axes: rain plot
     """
+    if rain.size == 1:
+        freq_step = pd.Timedelta(rain.index.freq)
+        rain = rain.reindex(pd.date_range(rain.index[0]-freq_step, periods=3, freq=rain.index.freq))
     ax = rain.plot(ax=ax, drawstyle=f'steps-{step}', color=color, solid_capstyle=capstyle, solid_joinstyle=joinstyle,
                    lw=0)
     ax.fill_between(rain.index, rain.values, 0, step=step, zorder=1000, color=color, capstyle=capstyle,
                     joinstyle=joinstyle)
 
     if reverse:
         # ax.set_ylim(top=0, bottom=rain.max() * 1.1)
```

### Comparing `idf_analysis-0.2.5/idf_analysis/synthetic_rainseries.py` & `idf_analysis-0.2.6/idf_analysis/synthetic_rainseries.py`

 * *Files identical despite different names*

### Comparing `idf_analysis-0.2.5/idf_analysis.egg-info/PKG-INFO` & `idf_analysis-0.2.6/idf_analysis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-analysis
-Version: 0.2.5
+Version: 0.2.6
 Summary: heavy rain as a function of the duration and the return period acc. to DWA-A 531 (2012)
 Author-email: Markus Pichler <markus.pichler@tugraz.at>
 License: MIT
 Project-URL: Documentation, https://markuspic.github.io/intensity_duration_frequency_analysis/
 Project-URL: Changelog, https://github.com/MarkusPic/intensity_duration_frequency_analysis/-/blob/master/CHANGELOG.md
 Project-URL: homepage, https://github.com/MarkusPic/intensity_duration_frequency_analysis
 Keywords: duration,analysis,rainfall,dwd,idf,measurement-data,precipitation,kostra,dwa,heavy-rain,intensity-duration-frequency,design-rainfall,duration-steps,return-period,dwa-a-531
```

### Comparing `idf_analysis-0.2.5/idf_analysis.egg-info/SOURCES.txt` & `idf_analysis-0.2.6/idf_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idf_analysis-0.2.5/pyproject.toml` & `idf_analysis-0.2.6/pyproject.toml`

 * *Files identical despite different names*

