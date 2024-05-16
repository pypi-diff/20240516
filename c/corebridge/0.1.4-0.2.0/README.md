# Comparing `tmp/corebridge-0.1.4.tar.gz` & `tmp/corebridge-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corebridge-0.1.4.tar", last modified: Fri May  3 10:28:21 2024, max compression
+gzip compressed data, was "corebridge-0.2.0.tar", last modified: Thu May 16 16:25:43 2024, max compression
```

## Comparing `corebridge-0.1.4.tar` & `corebridge-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-03 10:28:21.469702 corebridge-0.1.4/
--rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.1.4/LICENSE
--rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.1.4/MANIFEST.in
--rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-03 10:28:21.469702 corebridge-0.1.4/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)     1887 2024-05-03 10:28:01.000000 corebridge-0.1.4/README.md
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-03 10:28:21.469702 corebridge-0.1.4/corebridge/
--rw-r--r--   0 fenke     (1000) users      (100)       22 2024-05-03 10:28:12.000000 corebridge-0.1.4/corebridge/__init__.py
--rw-r--r--   0 fenke     (1000) users      (100)     3300 2024-05-03 10:28:12.000000 corebridge-0.1.4/corebridge/_modidx.py
--rw-r--r--   0 fenke     (1000) users      (100)     8545 2024-05-03 10:28:12.000000 corebridge-0.1.4/corebridge/aicorebridge.py
--rw-r--r--   0 fenke     (1000) users      (100)     3766 2024-05-03 10:28:12.000000 corebridge-0.1.4/corebridge/core.py
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-03 10:28:21.469702 corebridge-0.1.4/corebridge.egg-info/
--rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-03 10:28:21.000000 corebridge-0.1.4/corebridge.egg-info/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      381 2024-05-03 10:28:21.000000 corebridge-0.1.4/corebridge.egg-info/SOURCES.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-05-03 10:28:21.000000 corebridge-0.1.4/corebridge.egg-info/dependency_links.txt
--rw-r--r--   0 fenke     (1000) users      (100)       42 2024-05-03 10:28:21.000000 corebridge-0.1.4/corebridge.egg-info/entry_points.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.1.4/corebridge.egg-info/not-zip-safe
--rw-r--r--   0 fenke     (1000) users      (100)      225 2024-05-03 10:28:21.000000 corebridge-0.1.4/corebridge.egg-info/requires.txt
--rw-r--r--   0 fenke     (1000) users      (100)       11 2024-05-03 10:28:21.000000 corebridge-0.1.4/corebridge.egg-info/top_level.txt
--rw-r--r--   0 fenke     (1000) users      (100)     1146 2024-04-29 12:11:53.000000 corebridge-0.1.4/settings.ini
--rw-r--r--   0 fenke     (1000) users      (100)       38 2024-05-03 10:28:21.469702 corebridge-0.1.4/setup.cfg
--rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.1.4/setup.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 16:25:43.544006 corebridge-0.2.0/
+-rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.2.0/LICENSE
+-rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.2.0/MANIFEST.in
+-rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 16:25:43.544006 corebridge-0.2.0/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)     1887 2024-05-03 10:28:01.000000 corebridge-0.2.0/README.md
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 16:25:43.544006 corebridge-0.2.0/corebridge/
+-rw-r--r--   0 fenke     (1000) users      (100)       22 2024-05-16 16:25:36.000000 corebridge-0.2.0/corebridge/__init__.py
+-rw-r--r--   0 fenke     (1000) users      (100)     2865 2024-05-16 16:25:36.000000 corebridge-0.2.0/corebridge/_modidx.py
+-rw-r--r--   0 fenke     (1000) users      (100)     4609 2024-05-16 16:25:36.000000 corebridge-0.2.0/corebridge/aicorebridge.py
+-rw-r--r--   0 fenke     (1000) users      (100)     4464 2024-05-16 16:25:36.000000 corebridge-0.2.0/corebridge/core.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 16:25:43.544006 corebridge-0.2.0/corebridge.egg-info/
+-rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 16:25:43.000000 corebridge-0.2.0/corebridge.egg-info/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      381 2024-05-16 16:25:43.000000 corebridge-0.2.0/corebridge.egg-info/SOURCES.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-05-16 16:25:43.000000 corebridge-0.2.0/corebridge.egg-info/dependency_links.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       42 2024-05-16 16:25:43.000000 corebridge-0.2.0/corebridge.egg-info/entry_points.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.2.0/corebridge.egg-info/not-zip-safe
+-rw-r--r--   0 fenke     (1000) users      (100)      267 2024-05-16 16:25:43.000000 corebridge-0.2.0/corebridge.egg-info/requires.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       11 2024-05-16 16:25:43.000000 corebridge-0.2.0/corebridge.egg-info/top_level.txt
+-rw-r--r--   0 fenke     (1000) users      (100)     1188 2024-05-16 16:25:18.000000 corebridge-0.2.0/settings.ini
+-rw-r--r--   0 fenke     (1000) users      (100)       38 2024-05-16 16:25:43.544006 corebridge-0.2.0/setup.cfg
+-rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.2.0/setup.py
```

### Comparing `corebridge-0.1.4/LICENSE` & `corebridge-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `corebridge-0.1.4/PKG-INFO` & `corebridge-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.1.4
+Version: 0.2.0
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.1.4/README.md` & `corebridge-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `corebridge-0.1.4/corebridge/_modidx.py` & `corebridge-0.2.0/corebridge/_modidx.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,22 +9,19 @@
                                                                                    'corebridge/aicorebridge.py'),
                                          'corebridge.aicorebridge.AICoreModule.__init__': ( 'aicorebridge.html#aicoremodule.__init__',
                                                                                             'corebridge/aicorebridge.py'),
                                          'corebridge.aicorebridge.AICoreModule._init_processor': ( 'aicorebridge.html#aicoremodule._init_processor',
                                                                                                    'corebridge/aicorebridge.py'),
                                          'corebridge.aicorebridge.AICoreModule.call_processor': ( 'aicorebridge.html#aicoremodule.call_processor',
                                                                                                   'corebridge/aicorebridge.py'),
-                                         'corebridge.aicorebridge.AICoreModule.convert_to_dataframe': ( 'aicorebridge.html#aicoremodule.convert_to_dataframe',
-                                                                                                        'corebridge/aicorebridge.py'),
                                          'corebridge.aicorebridge.AICoreModule.get_call_data': ( 'aicorebridge.html#aicoremodule.get_call_data',
                                                                                                  'corebridge/aicorebridge.py'),
                                          'corebridge.aicorebridge.AICoreModule.get_callargs': ( 'aicorebridge.html#aicoremodule.get_callargs',
                                                                                                 'corebridge/aicorebridge.py'),
                                          'corebridge.aicorebridge.AICoreModule.infer': ( 'aicorebridge.html#aicoremodule.infer',
-                                                                                         'corebridge/aicorebridge.py'),
-                                         'corebridge.aicorebridge.AICoreModule.rewrite_data': ( 'aicorebridge.html#aicoremodule.rewrite_data',
-                                                                                                'corebridge/aicorebridge.py')},
-            'corebridge.core': { 'corebridge.core.timeseries_dataframe': ('core.html#timeseries_dataframe', 'corebridge/core.py'),
+                                                                                         'corebridge/aicorebridge.py')},
+            'corebridge.core': { 'corebridge.core.set_time_index_zone': ('core.html#set_time_index_zone', 'corebridge/core.py'),
+                                 'corebridge.core.timeseries_dataframe': ('core.html#timeseries_dataframe', 'corebridge/core.py'),
                                  'corebridge.core.timeseries_dataframe_from_datadict': ( 'core.html#timeseries_dataframe_from_datadict',
                                                                                          'corebridge/core.py'),
                                  'corebridge.core.timeseries_dataframe_to_datadict': ( 'core.html#timeseries_dataframe_to_datadict',
                                                                                        'corebridge/core.py')}}}
```

### Comparing `corebridge-0.1.4/corebridge/core.py` & `corebridge-0.2.0/corebridge/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,108 +1,132 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/00_core.ipynb.
 
 # %% auto 0
-__all__ = ['timeseries_dataframe', 'timeseries_dataframe_from_datadict', 'timeseries_dataframe_to_datadict']
+__all__ = ['timeseries_dataframe', 'set_time_index_zone', 'timeseries_dataframe_from_datadict',
+           'timeseries_dataframe_to_datadict']
 
 # %% ../nbs/00_core.ipynb 3
 import typing
+import os
 import numpy as np
 import pandas as pd
 
 # %% ../nbs/00_core.ipynb 4
+try:
+    print(f"Loading {__name__} from {__file__}")
+except:
+    pass
+
+# %% ../nbs/00_core.ipynb 6
 def timeseries_dataframe(
-        adata:typing.Union[pd.DataFrame, pd.Series, dict, np.ndarray, np.recarray], 
+        data:typing.Union[pd.DataFrame, pd.Series, dict, np.ndarray, np.recarray], 
         timezone='UTC', 
         columnnames=None):
     
-    """Convert various data formats to standardized timeseries DataFrame"""
+    """Convert various data formats to timeseries DataFrame"""
 
-    if isinstance(adata, pd.DataFrame):
-        df = adata
+    if isinstance(data, pd.DataFrame):
+        df = data
 
-    elif isinstance(adata, pd.Series):
-        df = pd.DataFrame(adata)
+    elif isinstance(data, pd.Series):
+        df = pd.DataFrame(data)
 
-    elif isinstance(adata, dict):
+    elif isinstance(data, dict):
         # dict/mapping of individual timeseries
         df = pd.DataFrame({
             C:pd.Series(data=A[:,1], index=pd.DatetimeIndex(A[:,0]*1e9)) if isinstance(A, np.ndarray) else A
-            for C,A in adata.items()
+            for C,A in data.items()
         })
 
-    elif adata.dtype.names is not None:
-        # structured or recarray
+    elif data.dtype.names is not None:
+        # structured or recarray, we use column names from the recarray
         df = pd.DataFrame(
-            data=adata.view(dtype=np.float64).reshape(adata.shape[0],len(adata.dtype))[:,range(1,len(adata.dtype))],
-            index=pd.DatetimeIndex(adata.view(dtype=np.float64).reshape(adata.shape[0],len(adata.dtype))[:,0] * 1e9),
-            columns=adata.dtype.names[1:]
+            data=data.view(dtype=np.float64).reshape(data.shape[0],len(data.dtype))[:,range(1,len(data.dtype))],
+            index=pd.DatetimeIndex(data.view(dtype=np.float64).reshape(data.shape[0],len(data.dtype))[:,0] * 1e9),
+            columns=data.dtype.names[1:]
         )
 
     else:
-        if adata.shape[0] > 0:
-            if adata.shape[1]>2:
-                columns=[f"value_{str(i+1)}" for i in range(adata.shape[1]-1)] if not columnnames else [f"{str(i)}" for i in columnnames[1:]]
+        if data.shape[0] > 0:
+            # column names, either 'value' if there is only one column, or
+            # value_0, value_1 .... value_nn when more the one column is present
+            if data.shape[1]>2:
+                columns=[f"value_{str(i+1)}" for i in range(data.shape[1]-1)] if not columnnames else [f"{str(i)}" for i in columnnames[1:]]
             else:
                 columns=['value']
 
             df = pd.DataFrame(
-                data=adata[:, 1:],
-                index=pd.DatetimeIndex(adata[:,0]*1e9),
+                data=data[:, 1:],
+                index=pd.DatetimeIndex(data[:,0]*1e9),
                 columns=columns
             )
         else:
             return pd.DataFrame()
 
     df.index.name = 'time'
     if not df.index.tz:
         df.index = df.index.tz_localize('UTC').tz_convert(timezone)
     elif str(df.index.tz) != timezone:
         df.index = df.index.tz_convert(timezone)
 
+    return set_time_index_zone(df, timezone)
+
+# %% ../nbs/00_core.ipynb 7
+def set_time_index_zone(df:pd.DataFrame, timezone):
+
+    df.index.name = 'time'
+    if not df.index.tz:
+        df.index = df.index.tz_localize('UTC').tz_convert(timezone)
+    elif str(df.index.tz) != timezone:
+        df.index = df.index.tz_convert(timezone)
+
     return df
 
 
-# %% ../nbs/00_core.ipynb 5
+# %% ../nbs/00_core.ipynb 8
 def timeseries_dataframe_from_datadict(
         data:dict, 
-        recordformat='records',
-        timecolumns=[]):
+        timecolumns,
+        recordformat='records'):
         
     "Convert data dict to dataframe"
 
     orient = recordformat.lower()
+    assert orient in ['records', 'table']
     
     if orient == 'records':
         df = pd.DataFrame.from_records(data)
-        time_column = [C for C in df.columns if C.lower() in ['datetimemeasure', 'time']][0]
+        time_column = [C for C in df.columns if C.lower() in timecolumns][0]
 
     elif orient == 'table':
         time_column = data['schema']['primaryKey'][0]
         df = pd.DataFrame.from_dict(data['data']).set_index(data['schema']['primaryKey'])
         df.index.name = 'time'
 
     df.columns = [C.lower() for C in df.columns]
-    time_column = [C for C in df.columns if C in ['datetimemeasure', 'time']][0]
+    time_column = [C for C in df.columns if C in timecolumns][0]
     df[time_column] = pd.to_datetime(df[time_column],utc=True,format='ISO8601')
     df.set_index(time_column, inplace=True)
+    #df.index = pd.DatetimeIndex(df.index).round('ms')
     
     df.index.name = 'time'
+
     return df
 
 
-# %% ../nbs/00_core.ipynb 6
+# %% ../nbs/00_core.ipynb 9
 def timeseries_dataframe_to_datadict(
         data:typing.Union[pd.DataFrame, pd.Series, dict], 
         recordformat:str='split', 
         timezone:str='UTC', 
         reversed:bool=False):
     
     orient = recordformat.lower()
 
-    normalized_data = self.convert_to_dataframe(data, timezone=timezone)
+    normalized_data = timeseries_dataframe(data, timezone=timezone)
     normalized_data.index = normalized_data.index.map(lambda x: x.isoformat())
     
     if reversed:
         normalized_data = normalized_data[::-1]
 
     if orient == 'records':
         records = normalized_data.reset_index().to_dict(orient='records')
```

### Comparing `corebridge-0.1.4/corebridge.egg-info/PKG-INFO` & `corebridge-0.2.0/corebridge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.1.4
+Version: 0.2.0
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.1.4/settings.ini` & `corebridge-0.2.0/settings.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = corebridge
 lib_name = %(repo)s
-version = 0.1.4
+version = 0.2.0
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = corebridge
@@ -35,9 +35,9 @@
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = fenke
 
 ### Optional ###
 requirements = python-dateutil pytz numpy pandas scipy scikit-learn fastcore
-dev_requirements = python-dateutil pytz numpy pandas scipy scikit-learn fastcore jupyter ipywidgets jupyterlab>4 jupyter_contrib_nbextensions jupyterlab-git jupyterlab-quarto
+dev_requirements = python-dateutil pytz numpy pyarrow pandas scipy scikit-learn fastcore jupyter ipywidgets jupyterlab>4 jupyter_contrib_nbextensions jupyterlab-git jupyterlab-quarto nbdev aiohttp asyncpg apscheduler
 # console_scripts =
```

### Comparing `corebridge-0.1.4/setup.py` & `corebridge-0.2.0/setup.py`

 * *Files identical despite different names*

