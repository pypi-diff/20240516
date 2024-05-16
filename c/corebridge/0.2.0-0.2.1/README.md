# Comparing `tmp/corebridge-0.2.0.tar.gz` & `tmp/corebridge-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corebridge-0.2.0.tar", last modified: Thu May 16 16:25:43 2024, max compression
+gzip compressed data, was "corebridge-0.2.1.tar", last modified: Thu May 16 16:52:09 2024, max compression
```

## Comparing `corebridge-0.2.0.tar` & `corebridge-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 16:25:43.544006 corebridge-0.2.0/
--rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.2.0/LICENSE
--rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.2.0/MANIFEST.in
--rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 16:25:43.544006 corebridge-0.2.0/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)     1887 2024-05-03 10:28:01.000000 corebridge-0.2.0/README.md
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 16:25:43.544006 corebridge-0.2.0/corebridge/
--rw-r--r--   0 fenke     (1000) users      (100)       22 2024-05-16 16:25:36.000000 corebridge-0.2.0/corebridge/__init__.py
--rw-r--r--   0 fenke     (1000) users      (100)     2865 2024-05-16 16:25:36.000000 corebridge-0.2.0/corebridge/_modidx.py
--rw-r--r--   0 fenke     (1000) users      (100)     4609 2024-05-16 16:25:36.000000 corebridge-0.2.0/corebridge/aicorebridge.py
--rw-r--r--   0 fenke     (1000) users      (100)     4464 2024-05-16 16:25:36.000000 corebridge-0.2.0/corebridge/core.py
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 16:25:43.544006 corebridge-0.2.0/corebridge.egg-info/
--rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 16:25:43.000000 corebridge-0.2.0/corebridge.egg-info/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      381 2024-05-16 16:25:43.000000 corebridge-0.2.0/corebridge.egg-info/SOURCES.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-05-16 16:25:43.000000 corebridge-0.2.0/corebridge.egg-info/dependency_links.txt
--rw-r--r--   0 fenke     (1000) users      (100)       42 2024-05-16 16:25:43.000000 corebridge-0.2.0/corebridge.egg-info/entry_points.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.2.0/corebridge.egg-info/not-zip-safe
--rw-r--r--   0 fenke     (1000) users      (100)      267 2024-05-16 16:25:43.000000 corebridge-0.2.0/corebridge.egg-info/requires.txt
--rw-r--r--   0 fenke     (1000) users      (100)       11 2024-05-16 16:25:43.000000 corebridge-0.2.0/corebridge.egg-info/top_level.txt
--rw-r--r--   0 fenke     (1000) users      (100)     1188 2024-05-16 16:25:18.000000 corebridge-0.2.0/settings.ini
--rw-r--r--   0 fenke     (1000) users      (100)       38 2024-05-16 16:25:43.544006 corebridge-0.2.0/setup.cfg
--rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.2.0/setup.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 16:52:09.658851 corebridge-0.2.1/
+-rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.2.1/LICENSE
+-rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.2.1/MANIFEST.in
+-rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 16:52:09.658851 corebridge-0.2.1/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)     1887 2024-05-03 10:28:01.000000 corebridge-0.2.1/README.md
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 16:52:09.658851 corebridge-0.2.1/corebridge/
+-rw-r--r--   0 fenke     (1000) users      (100)       22 2024-05-16 16:51:47.000000 corebridge-0.2.1/corebridge/__init__.py
+-rw-r--r--   0 fenke     (1000) users      (100)     2865 2024-05-16 16:51:47.000000 corebridge-0.2.1/corebridge/_modidx.py
+-rw-r--r--   0 fenke     (1000) users      (100)     4659 2024-05-16 16:51:47.000000 corebridge-0.2.1/corebridge/aicorebridge.py
+-rw-r--r--   0 fenke     (1000) users      (100)     4464 2024-05-16 16:51:47.000000 corebridge-0.2.1/corebridge/core.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 16:52:09.658851 corebridge-0.2.1/corebridge.egg-info/
+-rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 16:52:09.000000 corebridge-0.2.1/corebridge.egg-info/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      381 2024-05-16 16:52:09.000000 corebridge-0.2.1/corebridge.egg-info/SOURCES.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-05-16 16:52:09.000000 corebridge-0.2.1/corebridge.egg-info/dependency_links.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       42 2024-05-16 16:52:09.000000 corebridge-0.2.1/corebridge.egg-info/entry_points.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.2.1/corebridge.egg-info/not-zip-safe
+-rw-r--r--   0 fenke     (1000) users      (100)      273 2024-05-16 16:52:09.000000 corebridge-0.2.1/corebridge.egg-info/requires.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       11 2024-05-16 16:52:09.000000 corebridge-0.2.1/corebridge.egg-info/top_level.txt
+-rw-r--r--   0 fenke     (1000) users      (100)     1194 2024-05-16 16:51:37.000000 corebridge-0.2.1/settings.ini
+-rw-r--r--   0 fenke     (1000) users      (100)       38 2024-05-16 16:52:09.658851 corebridge-0.2.1/setup.cfg
+-rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.2.1/setup.py
```

### Comparing `corebridge-0.2.0/LICENSE` & `corebridge-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.0/PKG-INFO` & `corebridge-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.2.0
+Version: 0.2.1
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.2.0/README.md` & `corebridge-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.0/corebridge/_modidx.py` & `corebridge-0.2.1/corebridge/_modidx.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.0/corebridge/aicorebridge.py` & `corebridge-0.2.1/corebridge/aicorebridge.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import inspect
 import datetime
 import json
 import pandas as pd
 import numpy as np
 
 from fastcore.basics import patch_to, patch
-
+import corebridge
 
 
 # %% ../nbs/01_aicorebridge.ipynb 5
 syslog = logging.getLogger(__name__)
 
 # %% ../nbs/01_aicorebridge.ipynb 6
 try:
@@ -96,15 +96,15 @@
             msg.append(f"{arg}: {val}")
             
         result = self.call_processor(calldata, **callargs)
         msg.append(f"result shape: {result.shape}")
 
         return {
             'msg':msg,
-            'data': core.timeseries_dataframe_to_datadict(
+            'data': corebridge.core.timeseries_dataframe_to_datadict(
                 result if not lastSeen else result[-1:],
                 recordformat=recordformat,
                 timezone=timezone,
                 reversed=reversed)
         }
     except Exception as err:
         return {
@@ -136,15 +136,15 @@
         data:dict, 
         recordformat='records', 
         timezone='UTC', 
         reversed=False):
     
     "Convert data to the processor signature"
 
-    df = core.set_time_index_zone(core.timeseries_dataframe_from_datadict(
+    df = corebridge.core.set_time_index_zone(corebridge.core.timeseries_dataframe_from_datadict(
         data, ['datetimemeasure', 'time'], recordformat), timezone)
 
     if reversed:
         df = df[::-1]
 
     if self.processor_params[self.data_param].annotation == pd.DataFrame:
         return df
```

### Comparing `corebridge-0.2.0/corebridge/core.py` & `corebridge-0.2.1/corebridge/core.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.0/corebridge.egg-info/PKG-INFO` & `corebridge-0.2.1/corebridge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.2.0
+Version: 0.2.1
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.2.0/settings.ini` & `corebridge-0.2.1/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = corebridge
 lib_name = %(repo)s
-version = 0.2.0
+version = 0.2.1
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = corebridge
@@ -34,10 +34,10 @@
 description = Bridge for Stactics AICore
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = fenke
 
 ### Optional ###
-requirements = python-dateutil pytz numpy pandas scipy scikit-learn fastcore
+requirements = python-dateutil pytz numpy pandas scipy scikit-learn fastcore twine
 dev_requirements = python-dateutil pytz numpy pyarrow pandas scipy scikit-learn fastcore jupyter ipywidgets jupyterlab>4 jupyter_contrib_nbextensions jupyterlab-git jupyterlab-quarto nbdev aiohttp asyncpg apscheduler
 # console_scripts =
```

### Comparing `corebridge-0.2.0/setup.py` & `corebridge-0.2.1/setup.py`

 * *Files identical despite different names*
