# Comparing `tmp/dagster-duckdb-pandas-0.23.5.tar.gz` & `tmp/dagster-duckdb-pandas-0.23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-duckdb-pandas-0.23.5.tar", last modified: Thu May  9 17:55:31 2024, max compression
+gzip compressed data, was "dagster-duckdb-pandas-0.23.6.tar", last modified: Thu May 16 20:13:24 2024, max compression
```

## Comparing `dagster-duckdb-pandas-0.23.5.tar` & `dagster-duckdb-pandas-0.23.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:31.524087 dagster-duckdb-pandas-0.23.5/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-09 17:47:35.000000 dagster-duckdb-pandas-0.23.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       55 2024-05-09 17:47:35.000000 dagster-duckdb-pandas-0.23.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      671 2024-05-09 17:55:31.524087 dagster-duckdb-pandas-0.23.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      142 2024-05-09 17:47:35.000000 dagster-duckdb-pandas-0.23.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:31.524087 dagster-duckdb-pandas-0.23.5/dagster_duckdb_pandas/
--rw-r--r--   0 root         (0) root         (0)      374 2024-05-09 17:47:35.000000 dagster-duckdb-pandas-0.23.5/dagster_duckdb_pandas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8658 2024-05-09 17:47:35.000000 dagster-duckdb-pandas-0.23.5/dagster_duckdb_pandas/duckdb_pandas_type_handler.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-09 17:47:35.000000 dagster-duckdb-pandas-0.23.5/dagster_duckdb_pandas/py.typed
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-09 17:47:35.000000 dagster-duckdb-pandas-0.23.5/dagster_duckdb_pandas/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:55:31.524087 dagster-duckdb-pandas-0.23.5/dagster_duckdb_pandas.egg-info/
--rw-r--r--   0 root         (0) root         (0)      671 2024-05-09 17:55:31.000000 dagster-duckdb-pandas-0.23.5/dagster_duckdb_pandas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      466 2024-05-09 17:55:31.000000 dagster-duckdb-pandas-0.23.5/dagster_duckdb_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:55:31.000000 dagster-duckdb-pandas-0.23.5/dagster_duckdb_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:55:31.000000 dagster-duckdb-pandas-0.23.5/dagster_duckdb_pandas.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       49 2024-05-09 17:55:31.000000 dagster-duckdb-pandas-0.23.5/dagster_duckdb_pandas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 17:55:31.000000 dagster-duckdb-pandas-0.23.5/dagster_duckdb_pandas.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      132 2024-05-09 17:55:31.528087 dagster-duckdb-pandas-0.23.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1508 2024-05-09 17:47:35.000000 dagster-duckdb-pandas-0.23.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:13:24.444036 dagster-duckdb-pandas-0.23.6/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-16 20:06:23.000000 dagster-duckdb-pandas-0.23.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       55 2024-05-16 20:06:23.000000 dagster-duckdb-pandas-0.23.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      671 2024-05-16 20:13:24.444036 dagster-duckdb-pandas-0.23.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-16 20:06:23.000000 dagster-duckdb-pandas-0.23.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:13:24.444036 dagster-duckdb-pandas-0.23.6/dagster_duckdb_pandas/
+-rw-r--r--   0 root         (0) root         (0)      374 2024-05-16 20:06:23.000000 dagster-duckdb-pandas-0.23.6/dagster_duckdb_pandas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9099 2024-05-16 20:06:23.000000 dagster-duckdb-pandas-0.23.6/dagster_duckdb_pandas/duckdb_pandas_type_handler.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-05-16 20:06:23.000000 dagster-duckdb-pandas-0.23.6/dagster_duckdb_pandas/py.typed
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-16 20:06:23.000000 dagster-duckdb-pandas-0.23.6/dagster_duckdb_pandas/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:13:24.444036 dagster-duckdb-pandas-0.23.6/dagster_duckdb_pandas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      671 2024-05-16 20:13:24.000000 dagster-duckdb-pandas-0.23.6/dagster_duckdb_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      466 2024-05-16 20:13:24.000000 dagster-duckdb-pandas-0.23.6/dagster_duckdb_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:13:24.000000 dagster-duckdb-pandas-0.23.6/dagster_duckdb_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:13:24.000000 dagster-duckdb-pandas-0.23.6/dagster_duckdb_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       45 2024-05-16 20:13:24.000000 dagster-duckdb-pandas-0.23.6/dagster_duckdb_pandas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-16 20:13:24.000000 dagster-duckdb-pandas-0.23.6/dagster_duckdb_pandas.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-16 20:13:24.444036 dagster-duckdb-pandas-0.23.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1370 2024-05-16 20:06:23.000000 dagster-duckdb-pandas-0.23.6/setup.py
```

### Comparing `dagster-duckdb-pandas-0.23.5/LICENSE` & `dagster-duckdb-pandas-0.23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-duckdb-pandas-0.23.5/PKG-INFO` & `dagster-duckdb-pandas-0.23.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pandas
-Version: 0.23.5
+Version: 0.23.6
 Summary: Package for storing Pandas DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pandas-0.23.5/dagster_duckdb_pandas/duckdb_pandas_type_handler.py` & `dagster-duckdb-pandas-0.23.6/dagster_duckdb_pandas/duckdb_pandas_type_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional, Sequence, Type
 
 import pandas as pd
 from dagster import InputContext, MetadataValue, OutputContext, TableColumn, TableSchema
+from dagster._core.definitions.metadata import TableMetadataSet
 from dagster._core.storage.db_io_manager import DbTypeHandler, TableSlice
 from dagster_duckdb.io_manager import (
     DuckDbClient,
     DuckDBIOManager,
     build_duckdb_io_manager,
 )
 
@@ -51,15 +52,21 @@
             # table was not created, therefore already exists. Insert the data
             connection.execute(
                 f"insert into {table_slice.schema}.{table_slice.table} select * from obj"
             )
 
         context.add_output_metadata(
             {
-                "row_count": obj.shape[0],
+                # output object may be a slice/partition, so we output different metadata keys based on
+                # whether this output represents an entire table or just a slice/partition
+                **(
+                    TableMetadataSet(partition_row_count=obj.shape[0])
+                    if context.has_partition_key
+                    else TableMetadataSet(row_count=obj.shape[0])
+                ),
                 "dataframe_columns": MetadataValue.table_schema(
                     TableSchema(
                         columns=[
                             TableColumn(name=name, type=str(dtype))  # type: ignore  # (bad stubs)
                             for name, dtype in obj.dtypes.items()
                         ]
                     )
```

### Comparing `dagster-duckdb-pandas-0.23.5/dagster_duckdb_pandas.egg-info/PKG-INFO` & `dagster-duckdb-pandas-0.23.6/dagster_duckdb_pandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-duckdb-pandas
-Version: 0.23.5
+Version: 0.23.6
 Summary: Package for storing Pandas DataFrames in DuckDB.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-duckb-pandas
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-duckdb-pandas-0.23.5/setup.py` & `dagster-duckdb-pandas-0.23.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,13 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_duckdb_pandas_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.5",
-        "dagster-duckdb==0.23.5",
-        # Pinned pending duckdb removal of broken pandas import. Pin can be
-        # removed as soon as it produces a working build.
-        "pandas<2.1",
+        "dagster==1.7.6",
+        "dagster-duckdb==0.23.6",
+        "pandas",
     ],
     zip_safe=False,
 )
```

