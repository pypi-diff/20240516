# Comparing `tmp/corebridge-0.2.1.tar.gz` & `tmp/corebridge-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corebridge-0.2.1.tar", last modified: Thu May 16 16:52:09 2024, max compression
+gzip compressed data, was "corebridge-0.2.2.tar", last modified: Thu May 16 17:52:05 2024, max compression
```

## Comparing `corebridge-0.2.1.tar` & `corebridge-0.2.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 16:52:09.658851 corebridge-0.2.1/
--rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.2.1/LICENSE
--rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.2.1/MANIFEST.in
--rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 16:52:09.658851 corebridge-0.2.1/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)     1887 2024-05-03 10:28:01.000000 corebridge-0.2.1/README.md
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 16:52:09.658851 corebridge-0.2.1/corebridge/
--rw-r--r--   0 fenke     (1000) users      (100)       22 2024-05-16 16:51:47.000000 corebridge-0.2.1/corebridge/__init__.py
--rw-r--r--   0 fenke     (1000) users      (100)     2865 2024-05-16 16:51:47.000000 corebridge-0.2.1/corebridge/_modidx.py
--rw-r--r--   0 fenke     (1000) users      (100)     4659 2024-05-16 16:51:47.000000 corebridge-0.2.1/corebridge/aicorebridge.py
--rw-r--r--   0 fenke     (1000) users      (100)     4464 2024-05-16 16:51:47.000000 corebridge-0.2.1/corebridge/core.py
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 16:52:09.658851 corebridge-0.2.1/corebridge.egg-info/
--rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 16:52:09.000000 corebridge-0.2.1/corebridge.egg-info/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      381 2024-05-16 16:52:09.000000 corebridge-0.2.1/corebridge.egg-info/SOURCES.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-05-16 16:52:09.000000 corebridge-0.2.1/corebridge.egg-info/dependency_links.txt
--rw-r--r--   0 fenke     (1000) users      (100)       42 2024-05-16 16:52:09.000000 corebridge-0.2.1/corebridge.egg-info/entry_points.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.2.1/corebridge.egg-info/not-zip-safe
--rw-r--r--   0 fenke     (1000) users      (100)      273 2024-05-16 16:52:09.000000 corebridge-0.2.1/corebridge.egg-info/requires.txt
--rw-r--r--   0 fenke     (1000) users      (100)       11 2024-05-16 16:52:09.000000 corebridge-0.2.1/corebridge.egg-info/top_level.txt
--rw-r--r--   0 fenke     (1000) users      (100)     1194 2024-05-16 16:51:37.000000 corebridge-0.2.1/settings.ini
--rw-r--r--   0 fenke     (1000) users      (100)       38 2024-05-16 16:52:09.658851 corebridge-0.2.1/setup.cfg
--rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.2.1/setup.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 17:52:05.875648 corebridge-0.2.2/
+-rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.2.2/LICENSE
+-rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.2.2/MANIFEST.in
+-rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 17:52:05.875648 corebridge-0.2.2/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)     1887 2024-05-03 10:28:01.000000 corebridge-0.2.2/README.md
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 17:52:05.875648 corebridge-0.2.2/corebridge/
+-rw-r--r--   0 fenke     (1000) users      (100)     4615 2024-05-16 17:50:44.000000 corebridge-0.2.2/corebridge/__init__.py
+-rw-r--r--   0 fenke     (1000) users      (100)     2865 2024-05-16 17:50:44.000000 corebridge-0.2.2/corebridge/_modidx.py
+-rw-r--r--   0 fenke     (1000) users      (100)     4612 2024-05-16 17:50:44.000000 corebridge-0.2.2/corebridge/aicorebridge.py
+-rw-r--r--   0 fenke     (1000) users      (100)     4464 2024-05-16 17:50:44.000000 corebridge-0.2.2/corebridge/core.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-05-16 17:52:05.875648 corebridge-0.2.2/corebridge.egg-info/
+-rw-r--r--   0 fenke     (1000) users      (100)     2655 2024-05-16 17:52:05.000000 corebridge-0.2.2/corebridge.egg-info/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      381 2024-05-16 17:52:05.000000 corebridge-0.2.2/corebridge.egg-info/SOURCES.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-05-16 17:52:05.000000 corebridge-0.2.2/corebridge.egg-info/dependency_links.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       42 2024-05-16 17:52:05.000000 corebridge-0.2.2/corebridge.egg-info/entry_points.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.2.2/corebridge.egg-info/not-zip-safe
+-rw-r--r--   0 fenke     (1000) users      (100)      273 2024-05-16 17:52:05.000000 corebridge-0.2.2/corebridge.egg-info/requires.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       11 2024-05-16 17:52:05.000000 corebridge-0.2.2/corebridge.egg-info/top_level.txt
+-rw-r--r--   0 fenke     (1000) users      (100)     1194 2024-05-16 17:50:53.000000 corebridge-0.2.2/settings.ini
+-rw-r--r--   0 fenke     (1000) users      (100)       38 2024-05-16 17:52:05.875648 corebridge-0.2.2/setup.cfg
+-rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.2.2/setup.py
```

### Comparing `corebridge-0.2.1/LICENSE` & `corebridge-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.1/PKG-INFO` & `corebridge-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.2.1
+Version: 0.2.2
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.2.1/README.md` & `corebridge-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.1/corebridge/_modidx.py` & `corebridge-0.2.2/corebridge/_modidx.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.1/corebridge/aicorebridge.py` & `corebridge-0.2.2/corebridge/aicorebridge.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import inspect
 import datetime
 import json
 import pandas as pd
 import numpy as np
 
 from fastcore.basics import patch_to, patch
-import corebridge
+from core import *
 
 
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
-            'data': corebridge.core.timeseries_dataframe_to_datadict(
+            'data': timeseries_dataframe_to_datadict(
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
 
-    df = corebridge.core.set_time_index_zone(corebridge.core.timeseries_dataframe_from_datadict(
+    df = set_time_index_zone(timeseries_dataframe_from_datadict(
         data, ['datetimemeasure', 'time'], recordformat), timezone)
 
     if reversed:
         df = df[::-1]
 
     if self.processor_params[self.data_param].annotation == pd.DataFrame:
         return df
```

### Comparing `corebridge-0.2.1/corebridge/core.py` & `corebridge-0.2.2/corebridge/core.py`

 * *Files identical despite different names*

### Comparing `corebridge-0.2.1/corebridge.egg-info/PKG-INFO` & `corebridge-0.2.2/corebridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.2.1
+Version: 0.2.2
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
 Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `corebridge-0.2.1/settings.ini` & `corebridge-0.2.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = corebridge
 lib_name = %(repo)s
-version = 0.2.1
+version = 0.2.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = corebridge
```

### Comparing `corebridge-0.2.1/setup.py` & `corebridge-0.2.2/setup.py`

 * *Files identical despite different names*

