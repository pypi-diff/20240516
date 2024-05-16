# Comparing `tmp/nemosis-3.4.0.tar.gz` & `tmp/nemosis-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\nick\Documents\GitHub\NEMOSIS\dist\tmph382q9no\nemosis-3.4.0.tar", last modified: Fri Nov 11 00:12:37 2022, max compression
+gzip compressed data, was "nemosis-3.6.0.tar", last modified: Thu May 16 03:07:31 2024, max compression
```

## Comparing `nemosis-3.4.0.tar` & `nemosis-3.6.0.tar`

### file list

```diff
@@ -1,28 +1,38 @@
-drwxrwxrwx   0        0        0        0 2022-11-11 00:12:37.526651 nemosis-3.4.0/
--rw-rw-rw-   0        0        0    36649 2021-02-28 21:52:55.000000 nemosis-3.4.0/LICENSE
--rw-rw-rw-   0        0        0      494 2022-11-11 00:12:37.525655 nemosis-3.4.0/PKG-INFO
--rw-rw-rw-   0        0        0    11823 2022-11-08 05:59:15.000000 nemosis-3.4.0/README.md
-drwxrwxrwx   0        0        0        0 2022-11-11 00:12:37.494740 nemosis-3.4.0/nemosis/
--rw-rw-rw-   0        0        0      285 2022-10-18 04:36:19.000000 nemosis-3.4.0/nemosis/__init__.py
--rw-rw-rw-   0        0        0      192 2022-10-18 04:36:19.000000 nemosis-3.4.0/nemosis/custom_errors.py
--rw-rw-rw-   0        0        0    21175 2022-10-18 04:36:19.000000 nemosis-3.4.0/nemosis/custom_tables.py
--rw-rw-rw-   0        0        0    31248 2022-11-10 04:36:55.000000 nemosis-3.4.0/nemosis/data_fetch_methods.py
--rw-rw-rw-   0        0        0     5572 2022-11-08 01:08:39.000000 nemosis-3.4.0/nemosis/date_generators.py
--rw-rw-rw-   0        0        0    24706 2022-11-11 00:03:56.000000 nemosis-3.4.0/nemosis/defaults.py
--rw-rw-rw-   0        0        0     9341 2022-11-10 04:15:29.000000 nemosis-3.4.0/nemosis/downloader.py
--rw-rw-rw-   0        0        0     4195 2022-10-18 04:36:19.000000 nemosis-3.4.0/nemosis/filters.py
--rw-rw-rw-   0        0        0    23230 2022-10-18 07:52:35.000000 nemosis-3.4.0/nemosis/gui.py
--rw-rw-rw-   0        0        0       52 2022-10-18 04:36:19.000000 nemosis-3.4.0/nemosis/hook-pandas.py
--rw-rw-rw-   0        0        0     9598 2022-11-10 03:45:21.000000 nemosis-3.4.0/nemosis/processing_info_maps.py
--rw-rw-rw-   0        0        0     2909 2022-10-18 04:36:19.000000 nemosis-3.4.0/nemosis/query_wrappers.py
--rw-rw-rw-   0        0        0    43026 2022-10-18 04:36:19.000000 nemosis-3.4.0/nemosis/rows.py
--rw-rw-rw-   0        0        0     1537 2022-11-10 03:33:48.000000 nemosis-3.4.0/nemosis/write_file_names.py
-drwxrwxrwx   0        0        0        0 2022-11-11 00:12:37.524658 nemosis-3.4.0/nemosis.egg-info/
--rw-rw-rw-   0        0        0      494 2022-11-11 00:12:37.000000 nemosis-3.4.0/nemosis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      523 2022-11-11 00:12:37.000000 nemosis-3.4.0/nemosis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-11 00:12:37.000000 nemosis-3.4.0/nemosis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2022-11-11 00:12:37.000000 nemosis-3.4.0/nemosis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-11-11 00:12:37.000000 nemosis-3.4.0/nemosis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-10-19 02:21:44.000000 nemosis-3.4.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-11-11 00:12:37.526651 nemosis-3.4.0/setup.cfg
--rw-rw-rw-   0        0        0      898 2022-11-10 23:46:06.000000 nemosis-3.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 03:07:31.976484 nemosis-3.6.0/
+-rw-rw-rw-   0        0        0    36649 2021-02-28 21:52:55.000000 nemosis-3.6.0/LICENSE
+-rw-rw-rw-   0        0        0      697 2024-05-16 03:07:31.974481 nemosis-3.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11555 2023-06-28 05:44:43.000000 nemosis-3.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 03:07:31.943477 nemosis-3.6.0/nemosis/
+-rw-rw-rw-   0        0        0      335 2024-05-16 02:07:15.000000 nemosis-3.6.0/nemosis/__init__.py
+-rw-rw-rw-   0        0        0      192 2022-10-18 04:36:19.000000 nemosis-3.6.0/nemosis/custom_errors.py
+-rw-rw-rw-   0        0        0    21175 2022-10-18 04:36:19.000000 nemosis-3.6.0/nemosis/custom_tables.py
+-rw-rw-rw-   0        0        0    30717 2024-05-16 02:07:15.000000 nemosis-3.6.0/nemosis/data_fetch_methods.py
+-rw-rw-rw-   0        0        0     5572 2022-11-08 01:08:39.000000 nemosis-3.6.0/nemosis/date_generators.py
+-rw-rw-rw-   0        0        0    25796 2024-05-16 02:07:15.000000 nemosis-3.6.0/nemosis/defaults.py
+-rw-rw-rw-   0        0        0     9341 2024-04-29 03:54:05.000000 nemosis-3.6.0/nemosis/downloader.py
+-rw-rw-rw-   0        0        0     3877 2024-05-16 02:07:15.000000 nemosis-3.6.0/nemosis/filters.py
+-rw-rw-rw-   0        0        0    23230 2022-10-18 07:52:35.000000 nemosis-3.6.0/nemosis/gui.py
+-rw-rw-rw-   0        0        0       52 2022-10-18 04:36:19.000000 nemosis-3.6.0/nemosis/hook-pandas.py
+-rw-rw-rw-   0        0        0    10107 2024-04-29 04:22:29.000000 nemosis-3.6.0/nemosis/processing_info_maps.py
+-rw-rw-rw-   0        0        0     2927 2024-05-16 02:07:15.000000 nemosis-3.6.0/nemosis/query_wrappers.py
+-rw-rw-rw-   0        0        0    43026 2022-10-18 04:36:19.000000 nemosis-3.6.0/nemosis/rows.py
+-rw-rw-rw-   0        0        0     1772 2024-05-16 02:07:15.000000 nemosis-3.6.0/nemosis/value_parser.py
+-rw-rw-rw-   0        0        0     1537 2022-11-10 03:33:48.000000 nemosis-3.6.0/nemosis/write_file_names.py
+drwxrwxrwx   0        0        0        0 2024-05-16 03:07:31.973478 nemosis-3.6.0/nemosis.egg-info/
+-rw-rw-rw-   0        0        0      697 2024-05-16 03:07:31.000000 nemosis-3.6.0/nemosis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      791 2024-05-16 03:07:31.000000 nemosis-3.6.0/nemosis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 03:07:31.000000 nemosis-3.6.0/nemosis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-05-16 03:07:31.000000 nemosis-3.6.0/nemosis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-16 03:07:31.000000 nemosis-3.6.0/nemosis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-10-19 02:21:44.000000 nemosis-3.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 03:07:31.976484 nemosis-3.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      898 2024-05-16 03:07:25.000000 nemosis-3.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 03:07:31.972482 nemosis-3.6.0/tests/
+-rw-rw-rw-   0        0        0    61326 2024-04-29 05:16:46.000000 nemosis-3.6.0/tests/test_data_fetch_methods.py
+-rw-rw-rw-   0        0        0    20268 2022-11-08 04:19:14.000000 nemosis-3.6.0/tests/test_date_generators.py
+-rw-rw-rw-   0        0        0    12692 2024-05-16 02:07:15.000000 nemosis-3.6.0/tests/test_errors_and_warnings.py
+-rw-rw-rw-   0        0        0    22590 2022-10-18 04:36:19.000000 nemosis-3.6.0/tests/test_filters.py
+-rw-rw-rw-   0        0        0    17295 2022-10-18 04:36:19.000000 nemosis-3.6.0/tests/test_format_options.py
+-rw-rw-rw-   0        0        0    25912 2022-10-18 04:36:19.000000 nemosis-3.6.0/tests/test_performance_stats.py
+-rw-rw-rw-   0        0        0    10794 2024-04-29 06:38:27.000000 nemosis-3.6.0/tests/test_processing_info_maps.py
+-rw-rw-rw-   0        0        0     9569 2022-10-18 04:36:19.000000 nemosis-3.6.0/tests/test_query_wrappers.py
```

### Comparing `nemosis-3.4.0/LICENSE` & `nemosis-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nemosis-3.4.0/README.md` & `nemosis-3.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # NEMOSIS
 
-## A Python package for downloading historical data published by the Australian Energy Market Operator (AEMO)
-
-## v3.2.0 has now been released. This fixes an issue with missing bid data causing errors, now warnings are issued. Also the messages printed by NEMOSIS now use the python logging module so they can turned off if desired see [Disable logging](#disable-logging).
+A Python package for downloading historical data published by the Australian Energy Market Operator (AEMO)
 
 -----
 
 ## Table of Contents
 
 - [Download Windows Application (GUI)](#download-windows-application-gui)
 - [Documentation](#documentation)
```

### Comparing `nemosis-3.4.0/nemosis/custom_tables.py` & `nemosis-3.6.0/nemosis/custom_tables.py`

 * *Files identical despite different names*

### Comparing `nemosis-3.4.0/nemosis/data_fetch_methods.py` & `nemosis-3.6.0/nemosis/data_fetch_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import logging
 import os as _os
 import glob as _glob
 import pandas as _pd
+import warnings
 from datetime import datetime as _datetime
 from . import filters as _filters
 from . import downloader as _downloader
 from . import processing_info_maps as _processing_info_maps
 from . import defaults as _defaults
 from . import custom_tables as _custom_tables
+from . import _infer_column_data_types
 from .custom_errors import UserInputError, NoDataToReturn, DataMismatchError
 
 logger = logging.getLogger(__name__)
 
+
 def dynamic_data_compiler(
     start_time,
     end_time,
     table_name,
     raw_data_location,
     select_columns=None,
     filter_cols=None,
@@ -251,15 +254,14 @@
                                       default set of columns.
         filter_cols (list): filter on columns.
         filter_values (tuple[list]): filter index n filter col such that values are
                               equal to index n filter value.
         update_static_file (bool): If True download latest version of file
                                    even if a version already exists.
                                    Default is False.
-        **kwargs: additional arguments passed to the pd.to_{fformat}() function
 
     Returns:
         data (pd.Dataframe)
     """
     if not _os.path.isdir(raw_data_location):
         raise UserInputError("The raw_data_location provided does not exist.")
 
@@ -320,15 +322,17 @@
     if filter_cols is not None:
         if not set(filter_cols).issubset(set(table.columns)):
             missing_columns = [col for col in filter_cols if col not in table.columns]
             UserInputError(f"Filter columns {missing_columns} not in data.")
         else:
             table = _filters.filter_on_column_value(table, filter_cols, filter_values)
 
-    table = static_data_finaliser_map[table_name](table, table_name)
+    static_table_finalisers = static_data_finaliser_map[table_name]
+    for finaliser in static_table_finalisers:
+        table = finaliser(table, table_name)
 
     return table
 
 
 def _strip_if_string(x):
     if isinstance(x, str):
         x = x.strip()
@@ -401,14 +405,20 @@
         primary_keys = _defaults.table_primary_keys[table_name]
         data = data.drop_duplicates(primary_keys)
     data = data.dropna(axis=0, how="all")
     data = data.dropna(axis=1, how="all")
     return data
 
 
+def _finalise_generators_and_scheduled_loads(data, table_name):
+    data = data.replace(to_replace=['', ' '], value='-')
+    data = data.fillna('-')
+    return data
+    
+
 def _finalise_csv_data(data, table_name):
     return data
 
 
 static_downloader_map = {
     "VARIABLES_FCAS_4_SECOND": _downloader.download_csv,
     "ELEMENTS_FCAS_4_SECOND": _downloader.download_elements_file,
@@ -420,18 +430,18 @@
     "VARIABLES_FCAS_4_SECOND": _read_static_csv,
     "ELEMENTS_FCAS_4_SECOND": _read_static_csv,
     "Generators and Scheduled Loads": _read_excel,
     "FCAS Providers": _read_excel,
 }
 
 static_data_finaliser_map = {
-    "VARIABLES_FCAS_4_SECOND": _finalise_csv_data,
-    "ELEMENTS_FCAS_4_SECOND": _finalise_csv_data,
-    "Generators and Scheduled Loads": _finalise_excel_data,
-    "FCAS Providers": _finalise_excel_data,
+    "VARIABLES_FCAS_4_SECOND": [_finalise_csv_data],
+    "ELEMENTS_FCAS_4_SECOND": [_finalise_csv_data],
+    "Generators and Scheduled Loads": [_finalise_excel_data, _finalise_generators_and_scheduled_loads],
+    "FCAS Providers": [_finalise_excel_data],
 }
 
 
 def static_table_FCAS_elements_file(
     table_name,
     raw_data_location,
     select_columns=None,
@@ -758,48 +768,15 @@
         )
 
     _processing_info_maps.downloader[table_type](
         year, month, day, index, filename_stub, raw_data_location
     )
     return
 
-
-def _infer_column_data_types(data):
-    """
-    Infer datatype of DataFrame assuming inference need only be carried out
-    for any columns with dtype "object". Adapted from StackOverflow.
-
-    If the column is an object type, attempt conversions to (in order of):
-    1. datetime
-    2. numeric
-
-    Returns: Data with inferred types.
-    """
-
-    def _get_series_type(series):
-        if series.dtype == "object":
-            try:
-                col_new = _pd.to_datetime(series)
-                return col_new
-            except Exception as e:
-                try:
-                    col_new = _pd.to_numeric(series)
-                    return col_new
-                except Exception as e:
-                    return series
-        else:
-            return series
-
-    for col in data:
-        series = data[col]
-        typed = _get_series_type(series)
-        data[col] = typed
-    return data
-
-
+  
 # GUI wrappers and mappers below
 
 
 def _dynamic_data_wrapper_for_gui(
     start_time, end_time, table, raw_data_location, columns, filter_cols, filter_values
 ):
     data = dynamic_data_compiler(
@@ -836,14 +813,15 @@
     "TRADINGLOAD": _dynamic_data_wrapper_for_gui,
     "TRADINGPRICE": _dynamic_data_wrapper_for_gui,
     "TRADINGREGIONSUM": _dynamic_data_wrapper_for_gui,
     "TRADINGINTERCONNECT": _dynamic_data_wrapper_for_gui,
     "DISPATCH_UNIT_SCADA": _dynamic_data_wrapper_for_gui,
     "DISPATCHCONSTRAINT": _dynamic_data_wrapper_for_gui,
     "DUDETAILSUMMARY": _dynamic_data_wrapper_for_gui,
+    "PARTICIPANT": _dynamic_data_wrapper_for_gui,
     "DUDETAIL": _dynamic_data_wrapper_for_gui,
     "GENCONDATA": _dynamic_data_wrapper_for_gui,
     "SPDREGIONCONSTRAINT": _dynamic_data_wrapper_for_gui,
     "SPDCONNECTIONPOINTCONSTRAINT": _dynamic_data_wrapper_for_gui,
     "SPDINTERCONNECTORCONSTRAINT": _dynamic_data_wrapper_for_gui,
     "FCAS_4_SECOND": _dynamic_data_wrapper_for_gui,
     "ELEMENTS_FCAS_4_SECOND": _static_table_wrapper_for_gui,
@@ -861,9 +839,10 @@
     "MNSP_DAYOFFER": _dynamic_data_wrapper_for_gui,
     "MNSP_PEROFFER": _dynamic_data_wrapper_for_gui,
     "MNSP_INTERCONNECTOR": _dynamic_data_wrapper_for_gui,
     "INTERCONNECTOR": _dynamic_data_wrapper_for_gui,
     "INTERCONNECTORCONSTRAINT": _dynamic_data_wrapper_for_gui,
     "MARKET_PRICE_THRESHOLDS": _dynamic_data_wrapper_for_gui,
     "DAILY_REGION_SUMMARY": _dynamic_data_wrapper_for_gui,
-    "NEXT_DAY_DISPATCHLOAD": _dynamic_data_wrapper_for_gui
+    "NEXT_DAY_DISPATCHLOAD": _dynamic_data_wrapper_for_gui,
+    "ROOFTOP_PV_ACTUAL": _dynamic_data_wrapper_for_gui
 }
```

### Comparing `nemosis-3.4.0/nemosis/date_generators.py` & `nemosis-3.6.0/nemosis/date_generators.py`

 * *Files identical despite different names*

### Comparing `nemosis-3.4.0/nemosis/defaults.py` & `nemosis-3.6.0/nemosis/defaults.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 names = {
     "FCAS Providers": "NEM Registration and Exemption List.xls",
     "DISPATCHLOAD": "PUBLIC_DVD_DISPATCHLOAD",
     "NEXT_DAY_DISPATCHLOAD": "PUBLIC_NEXT_DAY_DISPATCHLOAD",
     "DUDETAILSUMMARY": "PUBLIC_DVD_DUDETAILSUMMARY",
+    "PARTICIPANT": "PUBLIC_DVD_PARTICIPANT",
     "DUDETAIL": "PUBLIC_DVD_DUDETAIL",
     "DISPATCHCONSTRAINT": "PUBLIC_DVD_DISPATCHCONSTRAINT",
     "GENCONDATA": "PUBLIC_DVD_GENCONDATA",
     "DISPATCH_UNIT_SCADA": "PUBLIC_DVD_DISPATCH_UNIT_SCADA",
     "DISPATCHPRICE": "PUBLIC_DVD_DISPATCHPRICE",
     "SPDREGIONCONSTRAINT": "PUBLIC_DVD_SPDREGIONCONSTRAINT",
     "SPDCONNECTIONPOINTCONSTRAINT": "PUBLIC_DVD_SPDCONNECTIONPOINTCONSTRAINT",
@@ -29,22 +30,24 @@
     "FCAS_4s_SCADA_MAP": "",
     "PLANTSTATS": "",
     "TRADINGLOAD": "PUBLIC_DVD_TRADINGLOAD",
     "TRADINGPRICE": "PUBLIC_DVD_TRADINGPRICE",
     "TRADINGREGIONSUM": "PUBLIC_DVD_TRADINGREGIONSUM",
     "TRADINGINTERCONNECT": "PUBLIC_DVD_TRADINGINTERCONNECT",
     "MARKET_PRICE_THRESHOLDS": "PUBLIC_DVD_MARKET_PRICE_THRESHOLDS",
-    "DAILY_REGION_SUMMARY": "PUBLIC_DAILY_REGION_SUMMARY"
+    "DAILY_REGION_SUMMARY": "PUBLIC_DAILY_REGION_SUMMARY",
+    "ROOFTOP_PV_ACTUAL": "PUBLIC_DVD_ROOFTOP_PV_ACTUAL",
 }
 
 table_types = {
     "FCAS Providers": "STATICXL",
     "DISPATCHLOAD": "MMS",
     "NEXT_DAY_DISPATCHLOAD": "NEXT_DAY_DISPATCHLOAD",
     "DUDETAILSUMMARY": "MMS",
+    "PARTICIPANT": "MMS",
     "DUDETAIL": "MMS",
     "DISPATCHCONSTRAINT": "MMS",
     "GENCONDATA": "MMS",
     "DISPATCH_UNIT_SCADA": "MMS",
     "DISPATCHPRICE": "MMS",
     "SPDREGIONCONSTRAINT": "MMS",
     "SPDCONNECTIONPOINTCONSTRAINT": "MMS",
@@ -66,15 +69,16 @@
     "LOSSFACTORMODEL": "MMS",
     "FCAS_4s_SCADA_MAP": "CUSTOM",
     "TRADINGLOAD": "MMS",
     "TRADINGPRICE": "MMS",
     "TRADINGREGIONSUM": "MMS",
     "TRADINGINTERCONNECT": "MMS",
     "MARKET_PRICE_THRESHOLDS": "MMS",
-    "DAILY_REGION_SUMMARY": "DAILY_REGION_SUMMARY"
+    "DAILY_REGION_SUMMARY": "DAILY_REGION_SUMMARY",
+    "ROOFTOP_PV_ACTUAL": "MMS",
 }
 
 dynamic_tables = [
     table
     for table, type in table_types.items()
     if type in ["MMS", "BIDDING", "DAILY_REGION_SUMMARY", "NEXT_DAY_DISPATCHLOAD", "FCAS"]
 ]
@@ -82,14 +86,15 @@
 return_tables = list(names.keys())
 
 display_as_AMEO = [
     "FCAS Providers",
     "DISPATCHLOAD",
     "NEXT_DAY_DISPATCHLOAD",
     "DUDETAILSUMMARY",
+    "PARTICIPANT",
     "DUDETAIL",
     "DISPATCHCONSTRAINT",
     "GENCONDATA",
     "DISPATCH_UNIT_SCADA",
     "DISPATCHPRICE",
     "SPDREGIONCONSTRAINT",
     "SPDCONNECTIONPOINTCONSTRAINT",
@@ -102,14 +107,15 @@
     "ELEMENTS_FCAS_4_SECOND",
     "VARIABLES_FCAS_4_SECOND",
     "Generators and Scheduled Loads",
     "TRADINGLOAD",
     "TRADINGPRICE",
     "TRADINGREGIONSUM",
     "TRADINGINTERCONNECT",
+    "ROOFTOP_PV_ACTUAL",
 ]
 
 display_as_Custom = ["FCAS_4s_SCADA_MAP", "PLANTSTATS"]
 
 static_tables = [
     "ELEMENTS_FCAS_4_SECOND",
     "VARIABLES_FCAS_4_SECOND",
@@ -137,14 +143,15 @@
 fcas_4_url = "http://www.nemweb.com.au/Reports/Current/Causer_Pays/FCAS_{}{}{}{}.zip"
 
 fcas_4_url_hist = "http://www.nemweb.com.au/Data_Archive/Wholesale_Electricity/FCAS_Causer_Pays/{}/FCAS_Causer_Pays_{}_{}/FCAS_{}{}{}{}.zip"
 
 data_url = {
     "DISPATCHLOAD": "aemo_data_url",
     "DUDETAILSUMMARY": "aemo_data_url",
+    "PARTICIPANT": "aemo_data_url",
     "DUDETAIL": "aemo_data_url",
     "DISPATCHCONSTRAINT": "aemo_data_url",
     "GENCONDATA": "aemo_data_url",
     "DISPATCH_UNIT_SCADA": "aemo_data_url",
     "DISPATCHPRICE": "aemo_data_url",
     "SPDREGIONCONSTRAINT": "aemo_data_url",
     "SPDCONNECTIONPOINTCONSTRAINT": "aemo_data_url",
@@ -163,14 +170,15 @@
     "DISPATCHCASESOLUTION": "aemo_data_url",
     "FCAS": "fcas_4_url",
     "TRADINGLOAD": "aemo_data_url",
     "TRADINGPRICE": "aemo_data_url",
     "TRADINGREGIONSUM": "aemo_data_url",
     "TRADINGINTERCONNECT": "aemo_data_url",
     "MARKET_PRICE_THRESHOLDS": "aemo_data_url",
+    "ROOFTOP_PV_ACTUAL": "aemo_data_url",
 }
 
 filterable_cols = [
     "DUID",
     "REGIONID",
     "STATIONID",
     "PARTICIPANTID",
@@ -206,14 +214,15 @@
     "Region",
     "Max Cap (MW)",
     "Min Enablement Level",
     "Max Enablement Level",
     "Max Lower Angle",
     "Max Upper Angle",
     "Bid Type",
+    "TYPE",
 ]
 
 table_columns = {
     "DISPATCHLOAD": [
         "SETTLEMENTDATE",
         "DUID",
         "INTERVENTION",
@@ -222,17 +231,19 @@
         "INITIALMW",
         "TOTALCLEARED",
         "RAMPDOWNRATE",
         "RAMPUPRATE",
         "LOWER5MIN",
         "LOWER60SEC",
         "LOWER6SEC",
+        "LOWER1SEC",
         "RAISE5MIN",
         "RAISE60SEC",
         "RAISE6SEC",
+        "RAISE1SEC",
         "LOWERREG",
         "RAISEREG",
         "SEMIDISPATCHCAP",
         "AVAILABILITY",
         "RAISEREGENABLEMENTMAX",
         "RAISEREGENABLEMENTMIN",
         "LOWERREGENABLEMENTMAX",
@@ -247,17 +258,19 @@
         "INITIALMW",
         "TOTALCLEARED",
         "RAMPDOWNRATE",
         "RAMPUPRATE",
         "LOWER5MIN",
         "LOWER60SEC",
         "LOWER6SEC",
+        "LOWER1SEC",
         "RAISE5MIN",
         "RAISE60SEC",
         "RAISE6SEC",
+        "RAISE1SEC",
         "LOWERREG",
         "RAISEREG",
         "SEMIDISPATCHCAP",
         "AVAILABILITY",
         "RAISEREGENABLEMENTMAX",
         "RAISEREGENABLEMENTMIN",
         "LOWERREGENABLEMENTMAX",
@@ -340,14 +353,20 @@
         "TRANSMISSIONLOSSFACTOR",
         "STARTTYPE",
         "DISTRIBUTIONLOSSFACTOR",
         "SCHEDULE_TYPE",
         "MAX_RAMP_RATE_UP",
         "MAX_RAMP_RATE_DOWN",
     ],
+    "PARTICIPANT": [
+        "PARTICIPANTID",
+        "PARTICIPANTCLASSID",
+        "NAME",
+        "LASTCHANGED"
+    ],
     "DISPATCHCONSTRAINT": [
         "SETTLEMENTDATE",
         "RUNNO",
         "CONSTRAINTID",
         "INTERVENTION",
         "RHS",
         "MARGINALVALUE",
@@ -370,15 +389,18 @@
         "DISPATCH",
         "PREDISPATCH",
         "STPASA",
         "MTPASA",
         "LIMITTYPE",
         "REASON",
     ],
-    "DISPATCH_UNIT_SCADA": ["SETTLEMENTDATE", "DUID", "SCADAVALUE"],
+    "DISPATCH_UNIT_SCADA": [
+        "SETTLEMENTDATE",
+        "DUID",
+        "SCADAVALUE"],
     "DUDETAIL": [
         "EFFECTIVEDATE",
         "DUID",
         "VERSIONNO",
         "CONNECTIONPOINTID",
         "REGISTEREDCAPACITY",
         "AGCCAPABILITY",
@@ -654,25 +676,34 @@
         "MARKETSUSPENDEDFLAG",
         "TOTALDEMAND",
         "DEMANDFORECAST",
         "DISPATCHABLEGENERATION",
         "DISPATCHABLELOAD",
         "NETINTERCHANGE"
     ],
+    "ROOFTOP_PV_ACTUAL": [
+        "INTERVAL_DATETIME",
+        "REGIONID",
+        "POWER",
+        "QI",
+        "TYPE",
+        "LASTCHANGED"
+    ],
 }
 
 table_primary_keys = {
     "DISPATCHCONSTRAINT": [
         "CONSTRAINTID",
         "GENCONID_EFFECTIVEDATE",
         "GENCONID_VERSIONNO",
         "SETTLEMENTDATE",
         "INTERVENTION",
     ],
     "DUDETAILSUMMARY": ["DUID", "START_DATE", "END_DATE"],
+    "PARTICIPANT": ["PARTICIPANTID", "LASTCHANGED"],
     "STATION": ["STATIONID"],
     "DUDETAIL": ["EFFECTIVEDATE", "DUID", "VERSIONNO"],
     "SPDREGIONCONSTRAINT": [
         "EFFECTIVEDATE",
         "GENCONID",
         "REGIONID",
         "VERSIONNO",
@@ -749,41 +780,48 @@
     "PLANTSTATS": ["Month", "DUID"],
     "MARKET_PRICE_THRESHOLDS": ["EFFECTIVEDATE", "VERSIONNO"],
     "DAILY_REGION_SUMMARY": [
         "SETTLEMENTDATE",
         "INTERVENTION",
         "REGIONID",
     ],
+    "ROOFTOP_PV_ACTUAL": [
+        "INTERVAL_DATETIME",
+        "REGIONID",
+        "TYPE",
+    ],
 }
 
 effective_date_group_col = {
     "SPDREGIONCONSTRAINT": ["GENCONID"],
     "SPDCONNECTIONPOINTCONSTRAINT": ["GENCONID"],
     "SPDINTERCONNECTORCONSTRAINT": ["GENCONID"],
     "GENCONDATA": ["GENCONID"],
     "MNSP_INTERCONNECTOR": ["INTERCONNECTORID"],
     "INTERCONNECTORCONSTRAINT": ["INTERCONNECTORID"],
     "INTERCONNECTOR": ["INTERCONNECTORID"],
     "LOSSMODEL": ["INTERCONNECTORID"],
     "LOSSFACTORMODEL": ["INTERCONNECTORID"],
     "DUDETAILSUMMARY": ["DUID"],
+    "PARTICIPANT": ["PARTICIPANTID"],
     "MNSP_PEROFFER": ["LINKID"],
     "MNSP_DAYOFFER": ["LINKID"],
     "DUDETAIL": ["DUID"],
     "MARKET_PRICE_THRESHOLDS": [],
 }
 
 primary_date_columns = {
     "DISPATCHLOAD": "SETTLEMENTDATE",
     "NEXT_DAY_DISPATCHLOAD": "SETTLEMENTDATE",
     "TRADINGLOAD": "SETTLEMENTDATE",
     "TRADINGPRICE": "SETTLEMENTDATE",
     "TRADINGREGIONSUM": "SETTLEMENTDATE",
     "TRADINGINTERCONNECT": "SETTLEMENTDATE",
     "DUDETAILSUMMARY": "START_DATE",
+    "PARTICIPANT": "LASTCHANGED",
     "DUDETAIL": "EFFECTIVEDATE",
     "DISPATCHCONSTRAINT": "SETTLEMENTDATE",
     "GENCONDATA": "EFFECTIVEDATE",
     "DISPATCH_UNIT_SCADA": "SETTLEMENTDATE",
     "DISPATCHPRICE": "SETTLEMENTDATE",
     "SPDREGIONCONSTRAINT": "EFFECTIVEDATE",
     "SPDCONNECTIONPOINTCONSTRAINT": "EFFECTIVEDATE",
@@ -803,23 +841,30 @@
     "INTERCONNECTORCONSTRAINT": "EFFECTIVEDATE",
     "MNSP_DAYOFFER": "SETTLEMENTDATE",
     "LOSSMODEL": "EFFECTIVEDATE",
     "LOSSFACTORMODEL": "EFFECTIVEDATE",
     "FCAS_4s_SCADA_MAP": None,
     "MARKET_PRICE_THRESHOLDS": "EFFECTIVEDATE",
     "DAILY_REGION_SUMMARY": "SETTLEMENTDATE",
+    "ROOFTOP_PV_ACTUAL": "INTERVAL_DATETIME",
 }
 
 reg_exemption_list_tabs = {
     "Generators and Scheduled Loads": "Generators and Scheduled Loads",
     "FCAS Providers": "Ancillary Services",
 }
 
 months = ["01", "02", "03", "04", "05", "06", "07", "08", "09", "10", "11", "12"]
 
+date_formats = [
+    "%Y/%m/%d %H:%M:%S",
+    '%Y/%m/%d %H:%M:%S.%f',
+    '%Y-%m-%d %H:%M:%S'
+]
+
 nem_data_model_start_time = "2009/07/01 00:00:00"
 
 
 # GUI settings.
 header_y_pad = 30
 query_y_pad = (20, 0)
 query_row_offset = 2
```

### Comparing `nemosis-3.4.0/nemosis/downloader.py` & `nemosis-3.6.0/nemosis/downloader.py`

 * *Files identical despite different names*

### Comparing `nemosis-3.4.0/nemosis/filters.py` & `nemosis-3.6.0/nemosis/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,61 @@
 import logging
 import pandas as pd
 from datetime import datetime, timedelta
 import numpy as np
 
+from .value_parser import _parse_datetime
+
 logger = logging.getLogger(__name__)
 
 def filter_on_start_and_end_date(data, start_time, end_time):
-    data["START_DATE"] = pd.to_datetime(data["START_DATE"], format="%Y/%m/%d %H:%M:%S")
+    data["START_DATE"] = _parse_datetime(data["START_DATE"])
     data["END_DATE"] = np.where(
         data["END_DATE"] == "2999/12/31 00:00:00",
         "2100/12/31 00:00:00",
         data["END_DATE"],
     )
-    data["END_DATE"] = pd.to_datetime(data["END_DATE"], format="%Y/%m/%d %H:%M:%S")
+    data["END_DATE"] = _parse_datetime(data["END_DATE"])
     data = data[(data["START_DATE"] < end_time) & (data["END_DATE"] > start_time)]
     return data
 
 
 def filter_on_effective_date(data, start_time, end_time):
-    data["EFFECTIVEDATE"] = pd.to_datetime(
-        data["EFFECTIVEDATE"], format="%Y/%m/%d %H:%M:%S"
-    )
+    data["EFFECTIVEDATE"] = _parse_datetime(data["EFFECTIVEDATE"])
     data = data[data["EFFECTIVEDATE"] < end_time]
     return data
 
 
 def filter_on_settlementdate(data, start_time, end_time):
-    data["SETTLEMENTDATE"] = pd.to_datetime(
-        data["SETTLEMENTDATE"], format="%Y/%m/%d %H:%M:%S"
-    )
+    data["SETTLEMENTDATE"] = _parse_datetime(data["SETTLEMENTDATE"])
     data = data[
         (data["SETTLEMENTDATE"] > start_time) & (data["SETTLEMENTDATE"] <= end_time)
     ]
     return data
 
 
 def filter_on_timestamp(data, start_time, end_time):
     try:
-        data["TIMESTAMP"] = pd.to_datetime(
-            data["TIMESTAMP"], format="%Y/%m/%d %H:%M:%S"
-        )
-    except Exception as e:
+        data["TIMESTAMP"] = _parse_datetime(data["TIMESTAMP"])
+    except ValueError as e:
         logger.error(e)
         # if date format is wrong, str may be too short
         med_str_len = np.median(data["TIMESTAMP"].str.len())
         not_data = data.loc[data["TIMESTAMP"].str.len() < med_str_len, :]
         data = data.loc[data["TIMESTAMP"].str.len() >= med_str_len, :]
-        data["TIMESTAMP"] = pd.to_datetime(
-            data["TIMESTAMP"], format="%Y/%m/%d %H:%M:%S"
-        )
+        data["TIMESTAMP"] = _parse_datetime(data["TIMESTAMP"])
         logger.warning("Rows with incorrect data formats omitted")
-        logger.warning(not_data)
+        logger.warning(not_data.head())
     finally:
         data = data[(data["TIMESTAMP"] > start_time) & (data["TIMESTAMP"] <= end_time)]
     return data
 
 
 def filter_on_interval_datetime(data, start_time, end_time):
-    data["INTERVAL_DATETIME"] = pd.to_datetime(
-        data["INTERVAL_DATETIME"], format="%Y/%m/%d %H:%M:%S"
-    )
+    data["INTERVAL_DATETIME"] = _parse_datetime(data["INTERVAL_DATETIME"])
     data = data[
         (data["INTERVAL_DATETIME"] > start_time)
         & (data["INTERVAL_DATETIME"] <= end_time)
     ]
     return data
 
 
@@ -75,28 +67,24 @@
         & (data["SETTLEMENTDATE"] - timedelta(minutes=30) <= end_time)
     ]
     return data
 
 
 # Not tested, just for nemlite integration.
 def filter_on_date_and_interval(data, start_time, end_time):
-    data["SETTLEMENTDATE"] = pd.to_datetime(
-        data["SETTLEMENTDATE"], format="%Y/%m/%d %H:%M:%S"
-    )
+    data["SETTLEMENTDATE"] = _parse_datetime(data["SETTLEMENTDATE"])
     data = data[
         (data["SETTLEMENTDATE"] > start_time) & (data["SETTLEMENTDATE"] <= end_time)
     ]
     return data
 
 
 # Not tested, just for nemlite integration.
 def filter_on_last_changed(data, start_time, end_time):
-    data["LASTCHANGED"] = pd.to_datetime(
-        data["LASTCHANGED"], format="%Y/%m/%d %H:%M:%S"
-    )
+    data["LASTCHANGED"] = _parse_datetime(data["LASTCHANGED"])
     data = data[data["LASTCHANGED"] < end_time]
     return data
 
 
 def filter_on_column_value(data, filter_cols, filter_values):
     for filter_col, filter_values in zip(filter_cols, filter_values):
         if filter_values is not None:
```

### Comparing `nemosis-3.4.0/nemosis/gui.py` & `nemosis-3.6.0/nemosis/gui.py`

 * *Files identical despite different names*

### Comparing `nemosis-3.4.0/nemosis/processing_info_maps.py` & `nemosis-3.6.0/nemosis/processing_info_maps.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "TRADINGPRICE": None,
     "TRADINGREGIONSUM": None,
     "TRADINGINTERCONNECT": None,
     "DISPATCHPRICE": None,
     "DISPATCH_UNIT_SCADA": None,
     "DISPATCHCONSTRAINT": None,
     "DUDETAILSUMMARY": None,
+    "PARTICIPANT": None,
     "DUDETAIL": None,
     "GENCONDATA": None,
     "SPDREGIONCONSTRAINT": None,
     "SPDCONNECTIONPOINTCONSTRAINT": None,
     "SPDINTERCONNECTORCONSTRAINT": None,
     "FCAS_4_SECOND": None,
     "ELEMENTS_FCAS_4_SECOND": None,
@@ -39,27 +40,29 @@
     "MNSP_DAYOFFER": query_wrappers.dispatch_date_setup,
     "MNSP_PEROFFER": query_wrappers.dispatch_half_hour_setup,
     "MNSP_INTERCONNECTOR": None,
     "INTERCONNECTOR": None,
     "INTERCONNECTORCONSTRAINT": None,
     "MARKET_PRICE_THRESHOLDS": None,
     "DAILY_REGION_SUMMARY": None,
+    "ROOFTOP_PV_ACTUAL": None,
 }
 
 search_type = {
     "DISPATCHLOAD": "start_to_end",
     "NEXT_DAY_DISPATCHLOAD": "start_to_end",
     "TRADINGLOAD": "start_to_end",
     "TRADINGPRICE": "start_to_end",
     "TRADINGREGIONSUM": "start_to_end",
     "TRADINGINTERCONNECT": "start_to_end",
     "DISPATCHPRICE": "start_to_end",
     "DISPATCH_UNIT_SCADA": "start_to_end",
     "DISPATCHCONSTRAINT": "start_to_end",
     "DUDETAILSUMMARY": "end",
+    "PARTICIPANT": "all",
     "DUDETAIL": "all",
     "GENCONDATA": "all",
     "SPDREGIONCONSTRAINT": "all",
     "SPDCONNECTIONPOINTCONSTRAINT": "all",
     "SPDINTERCONNECTORCONSTRAINT": "all",
     "FCAS_4_SECOND": "start_to_end",
     "ELEMENTS_FCAS_4_SECOND": None,
@@ -75,27 +78,29 @@
     "MNSP_DAYOFFER": "start_to_end",
     "MNSP_PEROFFER": "start_to_end",
     "MNSP_INTERCONNECTOR": "all",
     "INTERCONNECTOR": "all",
     "INTERCONNECTORCONSTRAINT": "all",
     "MARKET_PRICE_THRESHOLDS": "all",
     "DAILY_REGION_SUMMARY": 'start_to_end',
+    "ROOFTOP_PV_ACTUAL": "start_to_end",
 }
 
 date_cols = {
     "DISPATCHLOAD": ["SETTLEMENTDATE"],
     "NEXT_DAY_DISPATCHLOAD": ["SETTLEMENTDATE"],
     "TRADINGLOAD": ["SETTLEMENTDATE"],
     "TRADINGPRICE": ["SETTLEMENTDATE"],
     "TRADINGREGIONSUM": ["SETTLEMENTDATE"],
     "TRADINGINTERCONNECT": ["SETTLEMENTDATE"],
     "DISPATCHPRICE": ["SETTLEMENTDATE"],
     "DISPATCH_UNIT_SCADA": ["SETTLEMENTDATE"],
     "DISPATCHCONSTRAINT": ["SETTLEMENTDATE"],
     "DUDETAILSUMMARY": ["START_DATE", "END_DATE"],
+    "PARTICIPANT": ["LASTCHANGED"],
     "DUDETAIL": ["EFFECTIVEDATE"],
     "GENCONDATA": ["EFFECTIVEDATE"],
     "SPDREGIONCONSTRAINT": ["EFFECTIVEDATE"],
     "SPDCONNECTIONPOINTCONSTRAINT": ["EFFECTIVEDATE"],
     "SPDINTERCONNECTORCONSTRAINT": ["EFFECTIVEDATE"],
     "FCAS_4_SECOND": ["TIMESTAMP"],
     "ELEMENTS_FCAS_4_SECOND": None,
@@ -111,27 +116,29 @@
     "MNSP_DAYOFFER": ["SETTLEMENTDATE"],
     "MNSP_PEROFFER": ["SETTLEMENTDATE", "PERIODID"],
     "MNSP_INTERCONNECTOR": ["EFFECTIVEDATE"],
     "INTERCONNECTOR": ["LASTCHANGED"],
     "INTERCONNECTORCONSTRAINT": ["EFFECTIVEDATE"],
     "MARKET_PRICE_THRESHOLDS": ["EFFECTIVEDATE"],
     "DAILY_REGION_SUMMARY": ['SETTLEMENTDATE'],
+    "ROOFTOP_PV_ACTUAL": ["INTERVAL_DATETIME"],
 }
 
 filter = {
     "DISPATCHLOAD": filters.filter_on_settlementdate,
     "NEXT_DAY_DISPATCHLOAD": filters.filter_on_settlementdate,
     "TRADINGLOAD": filters.filter_on_settlementdate,
     "TRADINGPRICE": filters.filter_on_settlementdate,
     "TRADINGREGIONSUM": filters.filter_on_settlementdate,
     "TRADINGINTERCONNECT": filters.filter_on_settlementdate,
     "DISPATCHPRICE": filters.filter_on_settlementdate,
     "DISPATCH_UNIT_SCADA": filters.filter_on_settlementdate,
     "DISPATCHCONSTRAINT": filters.filter_on_settlementdate,
     "DUDETAILSUMMARY": filters.filter_on_start_and_end_date,
+    "PARTICIPANT": filters.filter_on_last_changed,
     "DUDETAIL": filters.filter_on_effective_date,
     "GENCONDATA": filters.filter_on_effective_date,
     "SPDREGIONCONSTRAINT": filters.filter_on_effective_date,
     "SPDCONNECTIONPOINTCONSTRAINT": filters.filter_on_effective_date,
     "SPDINTERCONNECTORCONSTRAINT": filters.filter_on_effective_date,
     "FCAS_4_SECOND": filters.filter_on_timestamp,
     "ELEMENTS_FCAS_4_SECOND": None,
@@ -147,14 +154,15 @@
     "MNSP_DAYOFFER": filters.filter_on_settlementdate,
     "MNSP_PEROFFER": filters.filter_on_date_and_peroid,
     "MNSP_INTERCONNECTOR": filters.filter_on_effective_date,
     "INTERCONNECTOR": filters.filter_on_last_changed,
     "INTERCONNECTORCONSTRAINT": filters.filter_on_effective_date,
     "MARKET_PRICE_THRESHOLDS": filters.filter_on_effective_date,
     "DAILY_REGION_SUMMARY": filters.filter_on_settlementdate,
+    "ROOFTOP_PV_ACTUAL": filters.filter_on_interval_datetime,
 }
 
 finalise = {
     "DISPATCHLOAD": None,
     "NEXT_DAY_DISPATCHLOAD": None,
     "TRADINGLOAD": None,
     "TRADINGPRICE": None,
@@ -165,14 +173,18 @@
     "DISPATCHCONSTRAINT": [
         query_wrappers.convert_genconid_effectivedate_to_datetime_format
     ],
     "DUDETAILSUMMARY": [
         query_wrappers.most_recent_records_before_start_time,
         query_wrappers.drop_duplicates_by_primary_key,
     ],
+    "PARTICIPANT": [
+        query_wrappers.most_recent_records_before_start_time,
+        query_wrappers.drop_duplicates_by_primary_key,
+    ],
     "DUDETAIL": [
         query_wrappers.most_recent_records_before_start_time,
         query_wrappers.drop_duplicates_by_primary_key,
     ],
     "GENCONDATA": [
         query_wrappers.most_recent_records_before_start_time,
         query_wrappers.drop_duplicates_by_primary_key,
@@ -221,14 +233,15 @@
     ],
     "INTERCONNECTORCONSTRAINT": [
         query_wrappers.most_recent_records_before_start_time,
         query_wrappers.drop_duplicates_by_primary_key,
     ],
     "MARKET_PRICE_THRESHOLDS": None,
     "DAILY_REGION_SUMMARY": None,
+    "ROOFTOP_PV_ACTUAL": None,
 }
 
 date_gen = {
     "MMS": date_generators.year_and_month_gen,
     "NEXT_DAY_DISPATCHLOAD": date_generators.current_gen,
     "BIDDING": date_generators.bid_table_gen,
     "DAILY_REGION_SUMMARY": date_generators.current_gen,
```

### Comparing `nemosis-3.4.0/nemosis/query_wrappers.py` & `nemosis-3.6.0/nemosis/query_wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 from datetime import datetime, timedelta
-from . import defaults
+from . import defaults, _parse_datetime
 
 
 def dispatch_date_setup(start_time, end_time):
     start_time = datetime.strptime(start_time, "%Y/%m/%d %H:%M:%S")
     start_time = start_time - timedelta(hours=4)
     start_time = start_time.replace(hour=0, minute=0)
     start_time = start_time - timedelta(seconds=1)
@@ -66,9 +66,9 @@
 def drop_duplicates_by_primary_key(data, start_time, table_name):
     data = data.drop_duplicates(defaults.table_primary_keys[table_name])
     return data
 
 
 def convert_genconid_effectivedate_to_datetime_format(data, start_time, table_name):
     if "GENCONID_EFFECTIVEDATE" in data.columns:
-        data["GENCONID_EFFECTIVEDATE"] = pd.to_datetime(data["GENCONID_EFFECTIVEDATE"])
+        data["GENCONID_EFFECTIVEDATE"] = _parse_datetime(data["GENCONID_EFFECTIVEDATE"])
     return data
```

### Comparing `nemosis-3.4.0/nemosis/rows.py` & `nemosis-3.6.0/nemosis/rows.py`

 * *Files identical despite different names*

### Comparing `nemosis-3.4.0/nemosis/write_file_names.py` & `nemosis-3.6.0/nemosis/write_file_names.py`

 * *Files identical despite different names*

### Comparing `nemosis-3.4.0/nemosis.egg-info/SOURCES.txt` & `nemosis-3.6.0/nemosis.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -11,13 +11,22 @@
 nemosis/downloader.py
 nemosis/filters.py
 nemosis/gui.py
 nemosis/hook-pandas.py
 nemosis/processing_info_maps.py
 nemosis/query_wrappers.py
 nemosis/rows.py
+nemosis/value_parser.py
 nemosis/write_file_names.py
 nemosis.egg-info/PKG-INFO
 nemosis.egg-info/SOURCES.txt
 nemosis.egg-info/dependency_links.txt
 nemosis.egg-info/requires.txt
-nemosis.egg-info/top_level.txt
+nemosis.egg-info/top_level.txt
+tests/test_data_fetch_methods.py
+tests/test_date_generators.py
+tests/test_errors_and_warnings.py
+tests/test_filters.py
+tests/test_format_options.py
+tests/test_performance_stats.py
+tests/test_processing_info_maps.py
+tests/test_query_wrappers.py
```

### Comparing `nemosis-3.4.0/setup.py` & `nemosis-3.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nemosis",
-    version="3.4.0",
+    version="3.6.0",
     author="Nicholas Gorman, Abhijith Prakash",
     author_email="n.gorman305@gmail.com",
     description="A tool for accessing AEMO data.",
     long_description="A tool for accessing AEMO data.",
     long_description_content_type="text/markdown",
     url="https://github.com/UNSW-CEEM/NEMOSIS",
     packages=setuptools.find_packages(),
```

