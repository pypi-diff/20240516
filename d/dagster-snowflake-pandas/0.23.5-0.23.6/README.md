# Comparing `tmp/dagster-snowflake-pandas-0.23.5.tar.gz` & `tmp/dagster-snowflake-pandas-0.23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-snowflake-pandas-0.23.5.tar", last modified: Thu May  9 17:54:40 2024, max compression
+gzip compressed data, was "dagster-snowflake-pandas-0.23.6.tar", last modified: Thu May 16 20:16:34 2024, max compression
```

## Comparing `dagster-snowflake-pandas-0.23.5.tar` & `dagster-snowflake-pandas-0.23.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:54:40.456051 dagster-snowflake-pandas-0.23.5/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-09 17:47:35.000000 dagster-snowflake-pandas-0.23.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       76 2024-05-09 17:47:35.000000 dagster-snowflake-pandas-0.23.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      739 2024-05-09 17:54:40.456051 dagster-snowflake-pandas-0.23.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      158 2024-05-09 17:47:35.000000 dagster-snowflake-pandas-0.23.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:54:40.456051 dagster-snowflake-pandas-0.23.5/dagster_snowflake_pandas/
--rw-r--r--   0 root         (0) root         (0)      413 2024-05-09 17:47:35.000000 dagster-snowflake-pandas-0.23.5/dagster_snowflake_pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-09 17:47:35.000000 dagster-snowflake-pandas-0.23.5/dagster_snowflake_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)    12875 2024-05-09 17:47:35.000000 dagster-snowflake-pandas-0.23.5/dagster_snowflake_pandas/snowflake_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-09 17:47:35.000000 dagster-snowflake-pandas-0.23.5/dagster_snowflake_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:54:40.456051 dagster-snowflake-pandas-0.23.5/dagster_snowflake_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      739 2024-05-09 17:54:40.000000 dagster-snowflake-pandas-0.23.5/dagster_snowflake_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2024-05-09 17:54:40.000000 dagster-snowflake-pandas-0.23.5/dagster_snowflake_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:54:40.000000 dagster-snowflake-pandas-0.23.5/dagster_snowflake_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:54:40.000000 dagster-snowflake-pandas-0.23.5/dagster_snowflake_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      144 2024-05-09 17:54:40.000000 dagster-snowflake-pandas-0.23.5/dagster_snowflake_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-09 17:54:40.000000 dagster-snowflake-pandas-0.23.5/dagster_snowflake_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      171 2024-05-09 17:54:40.456051 dagster-snowflake-pandas-0.23.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1637 2024-05-09 17:47:35.000000 dagster-snowflake-pandas-0.23.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:16:34.612570 dagster-snowflake-pandas-0.23.6/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-16 20:06:23.000000 dagster-snowflake-pandas-0.23.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       76 2024-05-16 20:06:23.000000 dagster-snowflake-pandas-0.23.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      739 2024-05-16 20:16:34.612570 dagster-snowflake-pandas-0.23.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      158 2024-05-16 20:06:23.000000 dagster-snowflake-pandas-0.23.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:16:34.608570 dagster-snowflake-pandas-0.23.6/dagster_snowflake_pandas/
+-rw-r--r--   0 root         (0) root         (0)      413 2024-05-16 20:06:23.000000 dagster-snowflake-pandas-0.23.6/dagster_snowflake_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-16 20:06:23.000000 dagster-snowflake-pandas-0.23.6/dagster_snowflake_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)    13246 2024-05-16 20:06:23.000000 dagster-snowflake-pandas-0.23.6/dagster_snowflake_pandas/snowflake_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-16 20:06:23.000000 dagster-snowflake-pandas-0.23.6/dagster_snowflake_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:16:34.608570 dagster-snowflake-pandas-0.23.6/dagster_snowflake_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      739 2024-05-16 20:16:34.000000 dagster-snowflake-pandas-0.23.6/dagster_snowflake_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-16 20:16:34.000000 dagster-snowflake-pandas-0.23.6/dagster_snowflake_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:16:34.000000 dagster-snowflake-pandas-0.23.6/dagster_snowflake_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:16:34.000000 dagster-snowflake-pandas-0.23.6/dagster_snowflake_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      144 2024-05-16 20:16:34.000000 dagster-snowflake-pandas-0.23.6/dagster_snowflake_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-16 20:16:34.000000 dagster-snowflake-pandas-0.23.6/dagster_snowflake_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      171 2024-05-16 20:16:34.612570 dagster-snowflake-pandas-0.23.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1637 2024-05-16 20:06:23.000000 dagster-snowflake-pandas-0.23.6/setup.py
```

### Comparing `dagster-snowflake-pandas-0.23.5/LICENSE` & `dagster-snowflake-pandas-0.23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-snowflake-pandas-0.23.5/PKG-INFO` & `dagster-snowflake-pandas-0.23.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pandas
-Version: 0.23.5
+Version: 0.23.6
 Summary: Package for integrating Snowflake and Pandas with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-snowflake-pandas-0.23.5/dagster_snowflake_pandas/snowflake_pandas_type_handler.py` & `dagster-snowflake-pandas-0.23.6/dagster_snowflake_pandas/snowflake_pandas_type_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Mapping, Optional, Sequence, Type
 
 import numpy as np
 import pandas as pd
 from dagster import InputContext, MetadataValue, OutputContext, TableColumn, TableSchema
-from dagster._core.definitions.metadata import RawMetadataValue
+from dagster._core.definitions.metadata import RawMetadataValue, TableMetadataSet
 from dagster._core.errors import DagsterInvariantViolationError
 from dagster._core.storage.db_io_manager import DbTypeHandler, TableSlice
 from dagster_snowflake import build_snowflake_io_manager
 from dagster_snowflake.snowflake_io_manager import SnowflakeDbClient, SnowflakeIOManager
 from snowflake.connector.pandas_tools import write_pandas
 
 
@@ -125,15 +125,21 @@
             database=table_slice.database.upper() if table_slice.database else None,
             auto_create_table=True,
             use_logical_type=True,
             quote_identifiers=True,
         )
 
         return {
-            "row_count": obj.shape[0],
+            # output object may be a slice/partition, so we output different metadata keys based on
+            # whether this output represents an entire table or just a slice/partition
+            **(
+                TableMetadataSet(partition_row_count=obj.shape[0])
+                if context.has_partition_key
+                else TableMetadataSet(row_count=obj.shape[0])
+            ),
             "dataframe_columns": MetadataValue.table_schema(
                 TableSchema(
                     columns=[
                         TableColumn(name=str(name), type=str(dtype))
                         for name, dtype in obj.dtypes.items()
                     ]
                 )
```

### Comparing `dagster-snowflake-pandas-0.23.5/dagster_snowflake_pandas.egg-info/PKG-INFO` & `dagster-snowflake-pandas-0.23.6/dagster_snowflake_pandas.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-snowflake-pandas
-Version: 0.23.5
+Version: 0.23.6
 Summary: Package for integrating Snowflake and Pandas with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-snowflake-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-snowflake-pandas-0.23.5/setup.py` & `dagster-snowflake-pandas-0.23.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_snowflake_pandas_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.5",
-        "dagster-snowflake==0.23.5",
+        "dagster==1.7.6",
+        "dagster-snowflake==0.23.6",
         "pandas",
         "requests",
         "snowflake-connector-python[pandas]>=3.4.0",
         "sqlalchemy!=1.4.42",  # workaround for https://github.com/snowflakedb/snowflake-sqlalchemy/issues/350
         "snowflake-sqlalchemy>=1.2",
     ],
     zip_safe=False,
```

