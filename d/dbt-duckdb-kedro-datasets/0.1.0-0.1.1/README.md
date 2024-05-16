# Comparing `tmp/dbt_duckdb_kedro_datasets-0.1.0.tar.gz` & `tmp/dbt_duckdb_kedro_datasets-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_duckdb_kedro_datasets-0.1.0.tar", max compression
+gzip compressed data, was "dbt_duckdb_kedro_datasets-0.1.1.tar", max compression
```

## Comparing `dbt_duckdb_kedro_datasets-0.1.0.tar` & `dbt_duckdb_kedro_datasets-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      944 2024-05-16 08:56:04.870042 dbt_duckdb_kedro_datasets-0.1.0/README.md
--rw-r--r--   0        0        0       33 2024-05-16 08:56:56.088091 dbt_duckdb_kedro_datasets-0.1.0/dbt_duckdb_kedro_datasets/__init__.py
--rw-r--r--   0        0        0     1729 2024-05-16 08:56:50.679312 dbt_duckdb_kedro_datasets-0.1.0/dbt_duckdb_kedro_datasets/ddkd.py
--rw-r--r--   0        0        0      641 2024-05-16 08:18:59.670071 dbt_duckdb_kedro_datasets-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 dbt_duckdb_kedro_datasets-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-16 09:38:24.174729 dbt_duckdb_kedro_datasets-0.1.1/README.md
+-rw-r--r--   0        0        0       33 2024-05-16 09:38:24.174729 dbt_duckdb_kedro_datasets-0.1.1/dbt_duckdb_kedro_datasets/__init__.py
+-rw-r--r--   0        0        0     1729 2024-05-16 09:38:24.174729 dbt_duckdb_kedro_datasets-0.1.1/dbt_duckdb_kedro_datasets/ddkd.py
+-rw-r--r--   0        0        0      676 2024-05-16 09:38:24.178729 dbt_duckdb_kedro_datasets-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1740 1970-01-01 00:00:00.000000 dbt_duckdb_kedro_datasets-0.1.1/PKG-INFO
```

### Comparing `dbt_duckdb_kedro_datasets-0.1.0/dbt_duckdb_kedro_datasets/ddkd.py` & `dbt_duckdb_kedro_datasets-0.1.1/dbt_duckdb_kedro_datasets/ddkd.py`

 * *Files identical despite different names*

### Comparing `dbt_duckdb_kedro_datasets-0.1.0/pyproject.toml` & `dbt_duckdb_kedro_datasets-0.1.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbt_duckdb_kedro_datasets"
-version = "0.1.0"
+version = "0.1.1"
 description = "Combine duckdb-dbt and Kedro Dataset to easily read Kedro Dataset configs (yaml), enabling conversion of Kedro projects to dbt."
 authors = ["Conrad <conradbez1@gmail.com>"]
 readme = "README.md"
 packages = [{include = "dbt_duckdb_kedro_datasets"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
@@ -12,11 +12,13 @@
 kedro-datasets = {extras = ["pandas"], version = "^3.0.0"}
 pandas = "^2.2.2"
 fastparquet = "^2024.2.0"
 
 
 [tool.poetry.group.dev.dependencies]
 ipdb = "^0.13.13"
+twine = "^5.0.0"
+pytest = "^8.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dbt_duckdb_kedro_datasets-0.1.0/PKG-INFO` & `dbt_duckdb_kedro_datasets-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: dbt_duckdb_kedro_datasets
-Version: 0.1.0
+Version: 0.1.1
 Summary: Combine duckdb-dbt and Kedro Dataset to easily read Kedro Dataset configs (yaml), enabling conversion of Kedro projects to dbt.
 Author: Conrad
 Author-email: conradbez1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dbt-duckdb (>=1.8.0,<2.0.0)
 Requires-Dist: fastparquet (>=2024.2.0,<2025.0.0)
 Requires-Dist: kedro-datasets[pandas] (>=3.0.0,<4.0.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Description-Content-Type: text/markdown
 
-Combine duckdb-dbt and Kedro Dataset to easily read Kedro Dataset configs (yaml), enabling conversion of Kedro projects to dbt.
+Combine [duckdb-dbt](https://github.com/duckdb/dbt-duckdb/tree/master) and [Kedro](https://docs.kedro.org/en/stable/) [Datases](https://docs.kedro.org/projects/kedro-datasets/en/kedro-datasets-3.0.0/) to enable:
+
+- extension of dbt to ingest wide array of data, and;
+- conversion of Kedro projects to dbt by easily reading your Kedro data catalog configs (yaml files)
 
 ## Demo
 
 You can add your existing Kedro definitions to your dbt sources like so:
 
 `pip install dbt_duckdb_kedro_datasets`
 
@@ -45,14 +48,7 @@
 ```
 select *
 from {{ source('my_source', 'my_table') }}
 ```
 
 For a more complete example look at [this](example/example_dbt)
 
-## Todo
-
--[x] plugin backbone
--[x] initial install
--[x] initial execution
--[x] one config passed from yaml
-
```

