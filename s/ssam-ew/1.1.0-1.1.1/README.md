# Comparing `tmp/ssam_ew-1.1.0.tar.gz` & `tmp/ssam_ew-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssam_ew-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ssam_ew-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ssam_ew-1.1.0.tar` & `ssam_ew-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1085 2024-05-01 09:50:24.775826 ssam_ew-1.1.0/LICENSE
--rw-r--r--   0        0        0       45 2024-05-01 09:50:24.733137 ssam_ew-1.1.0/README.md
--rw-r--r--   0        0        0     1001 2024-05-13 15:39:34.805605 ssam_ew-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      366 2024-05-13 15:39:08.706041 ssam_ew-1.1.0/src/ssam_ew/__init__.py
--rw-r--r--   0        0        0    14055 2024-05-13 15:28:42.530201 ssam_ew-1.1.0/src/ssam_ew/magma.py
--rw-r--r--   0        0        0    11295 2024-05-13 15:24:09.805076 ssam_ew-1.1.0/src/ssam_ew/ssam.py
--rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 ssam_ew-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-05-01 09:50:24.775826 ssam_ew-1.1.1/LICENSE
+-rw-r--r--   0        0        0       45 2024-05-01 09:50:24.733137 ssam_ew-1.1.1/README.md
+-rw-r--r--   0        0        0     1001 2024-05-16 05:26:24.830975 ssam_ew-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      366 2024-05-13 15:39:08.706041 ssam_ew-1.1.1/src/ssam_ew/__init__.py
+-rw-r--r--   0        0        0    14055 2024-05-13 15:28:42.530201 ssam_ew-1.1.1/src/ssam_ew/magma.py
+-rw-r--r--   0        0        0    11303 2024-05-16 05:25:39.257114 ssam_ew-1.1.1/src/ssam_ew/ssam.py
+-rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 ssam_ew-1.1.1/PKG-INFO
```

### Comparing `ssam_ew-1.1.0/LICENSE` & `ssam_ew-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ssam_ew-1.1.0/pyproject.toml` & `ssam_ew-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name =  "ssam-ew"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
     {name = "Martanto", email = "martanto@live.com"},
 ]
 description = "Plot SSAM from earthworm files"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["seismic", "volcano", "seiscomp", "volcanology", "seismology", "magma indonesia"]
```

### Comparing `ssam_ew-1.1.0/src/ssam_ew/magma.py` & `ssam_ew-1.1.1/src/ssam_ew/magma.py`

 * *Files identical despite different names*

### Comparing `ssam_ew-1.1.0/src/ssam_ew/ssam.py` & `ssam_ew-1.1.1/src/ssam_ew/ssam.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,17 +220,17 @@
             resample = '1min'
 
         dates: DatetimeIndex = pd.date_range(start_date, end_date, freq="D")
 
         df = self.get_df(dates, resample)
 
         fig, ax = plt.subplots(figsize=(width, height), layout='constrained')
-        fig.colorbar(
-            plt.cm.ScalarMappable(norm=plt.Normalize(vmin=value_min, vmax=value_max), cmap=color_map),
-            ax=ax, pad=0.02)
+        # fig.colorbar(
+        #     plt.cm.ScalarMappable(norm=plt.Normalize(vmin=value_min, vmax=value_max), cmap=color_map),
+        #     ax=ax, pad=0.02)
 
         ax = self.plot_ax(ax, df=df, interval=interval, color_map=color_map, value_min=0.0,
                           value_max=value_max, frequencies=frequencies)
 
         if title is None:
             title = f'SSAM {self.nslc}'
 
@@ -248,15 +248,15 @@
 
     def plot_with_magma(self, token: str, volcano_code: str,  start_date: str, end_date: str,
                         resample: str = None, interval: int = 1, color_map: str = 'jet_r',
                         value_min: float = 0.0, value_max: float = 50.0, frequencies: list[float] = None,
                         earthquake_events: str | list[str] = None, width: int = 14, height: int = 12, height_ratios=None):
 
         if height_ratios is None:
-            height_ratios = [2, 1]
+            height_ratios = [1, 0.2]
 
         magma_plot = Plot(
             token=token,
             volcano_code=volcano_code,
             start_date=start_date,
             end_date=end_date,
             earthquake_events=earthquake_events,
```

### Comparing `ssam_ew-1.1.0/PKG-INFO` & `ssam_ew-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssam-ew
-Version: 1.1.0
+Version: 1.1.1
 Summary: Plot SSAM from earthworm files
 Keywords: seismic,volcano,seiscomp,volcanology,seismology,magma indonesia
 Author-email: Martanto <martanto@live.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

