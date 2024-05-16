# Comparing `tmp/prefect_dbt-0.4.3.tar.gz` & `tmp/prefect_dbt-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect_dbt-0.4.3.tar", last modified: Fri Apr 26 15:03:58 2024, max compression
+gzip compressed data, was "prefect_dbt-0.5.0.tar", last modified: Thu May 16 20:58:35 2024, max compression
```

## Comparing `prefect_dbt-0.4.3.tar` & `prefect_dbt-0.5.0.tar`

### file list

```diff
@@ -1,56 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.745123 prefect_dbt-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-04-26 15:03:58.745123 prefect_dbt-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.733123 prefect_dbt-0.4.3/prefect_dbt/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 15:03:58.000000 prefect_dbt-0.4.3/prefect_dbt/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.733123 prefect_dbt-0.4.3/prefect_dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15255 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.733123 prefect_dbt-0.4.3/prefect_dbt/cli/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/configs/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/configs/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/configs/snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     6798 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cli/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.737123 prefect_dbt-0.4.3/prefect_dbt/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    43316 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/prefect_dbt/cloud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.741123 prefect_dbt-0.4.3/prefect_dbt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12671 2024-04-26 15:03:58.000000 prefect_dbt-0.4.3/prefect_dbt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-26 15:03:58.000000 prefect_dbt-0.4.3/prefect_dbt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 15:03:58.000000 prefect_dbt-0.4.3/prefect_dbt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-26 15:03:58.000000 prefect_dbt-0.4.3/prefect_dbt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-26 15:03:58.000000 prefect_dbt-0.4.3/prefect_dbt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-26 15:03:58.000000 prefect_dbt-0.4.3/prefect_dbt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 15:03:58.745123 prefect_dbt-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.737123 prefect_dbt-0.4.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.737123 prefect_dbt-0.4.3/tests/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.737123 prefect_dbt-0.4.3/tests/cli/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cli/configs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cli/configs/test_bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cli/configs/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cli/configs/test_snowflake.py
--rw-r--r--   0 runner    (1001) docker     (127)     9375 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cli/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cli/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cli/test_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 15:03:58.741123 prefect_dbt-0.4.3/tests/cloud/
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cloud/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cloud/test_cloud_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)    31500 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cloud/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cloud/test_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/cloud/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-26 15:03:45.000000 prefect_dbt-0.4.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.844794 prefect_dbt-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-05-16 20:58:35.840794 prefect_dbt-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.832794 prefect_dbt-0.5.0/prefect_dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 20:58:35.000000 prefect_dbt-0.5.0/prefect_dbt/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.832794 prefect_dbt-0.5.0/prefect_dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35737 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.832794 prefect_dbt-0.5.0/prefect_dbt/cli/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10508 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5768 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/configs/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/configs/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/configs/snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cli/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.836794 prefect_dbt-0.5.0/prefect_dbt/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6519 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43316 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9943 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/prefect_dbt/cloud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.836794 prefect_dbt-0.5.0/prefect_dbt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12678 2024-05-16 20:58:35.000000 prefect_dbt-0.5.0/prefect_dbt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-16 20:58:35.000000 prefect_dbt-0.5.0/prefect_dbt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:58:35.000000 prefect_dbt-0.5.0/prefect_dbt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 20:58:35.000000 prefect_dbt-0.5.0/prefect_dbt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-16 20:58:35.000000 prefect_dbt-0.5.0/prefect_dbt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 20:58:35.000000 prefect_dbt-0.5.0/prefect_dbt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:58:35.844794 prefect_dbt-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.836794 prefect_dbt-0.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.836794 prefect_dbt-0.5.0/tests/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.836794 prefect_dbt-0.5.0/tests/cli/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cli/configs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5314 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cli/configs/test_bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cli/configs/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cli/configs/test_snowflake.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17727 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cli/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cli/test_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:58:35.836794 prefect_dbt-0.5.0/tests/cloud/
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cloud/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cloud/test_cloud_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31500 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cloud/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6602 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cloud/test_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/cloud/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5840 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-16 20:58:23.000000 prefect_dbt-0.5.0/tests/test_version.py
```

### Comparing `prefect_dbt-0.4.3/LICENSE` & `prefect_dbt-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/PKG-INFO` & `prefect_dbt-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-dbt
-Version: 0.4.3
+Version: 0.5.0
 Summary: Prefect integrations for working with dbt
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dbt
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prefect>=2.16.6
-Requires-Dist: dbt_core>=1.1.1
+Requires-Dist: prefect<3.0.0,>=2.16.6
+Requires-Dist: dbt-core>=1.7.0
 Requires-Dist: prefect_shell>=0.1.4
 Requires-Dist: sgqlc>=16.0.0
 Provides-Extra: snowflake
 Requires-Dist: prefect-snowflake>=0.2.4; extra == "snowflake"
 Requires-Dist: dbt-snowflake; extra == "snowflake"
 Provides-Extra: bigquery
 Requires-Dist: prefect-gcp[bigquery]>=0.1.8; extra == "bigquery"
```

### Comparing `prefect_dbt-0.4.3/README.md` & `prefect_dbt-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/prefect_dbt/__init__.py` & `prefect_dbt-0.5.0/prefect_dbt/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/prefect_dbt/cli/__init__.py` & `prefect_dbt-0.5.0/prefect_dbt/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/prefect_dbt/cli/configs/base.py` & `prefect_dbt-0.5.0/prefect_dbt/cli/configs/base.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/prefect_dbt/cli/configs/bigquery.py` & `prefect_dbt-0.5.0/prefect_dbt/cli/configs/bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/prefect_dbt/cli/configs/postgres.py` & `prefect_dbt-0.5.0/prefect_dbt/cli/configs/postgres.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/prefect_dbt/cli/configs/snowflake.py` & `prefect_dbt-0.5.0/prefect_dbt/cli/configs/snowflake.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/prefect_dbt/cli/credentials.py` & `prefect_dbt-0.5.0/prefect_dbt/cli/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/prefect_dbt/cloud/clients.py` & `prefect_dbt-0.5.0/prefect_dbt/cloud/clients.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/prefect_dbt/cloud/credentials.py` & `prefect_dbt-0.5.0/prefect_dbt/cloud/credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/prefect_dbt/cloud/exceptions.py` & `prefect_dbt-0.5.0/prefect_dbt/cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/prefect_dbt/cloud/jobs.py` & `prefect_dbt-0.5.0/prefect_dbt/cloud/jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/prefect_dbt/cloud/models.py` & `prefect_dbt-0.5.0/prefect_dbt/cloud/models.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/prefect_dbt/cloud/runs.py` & `prefect_dbt-0.5.0/prefect_dbt/cloud/runs.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/prefect_dbt/cloud/utils.py` & `prefect_dbt-0.5.0/prefect_dbt/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/prefect_dbt.egg-info/PKG-INFO` & `prefect_dbt-0.5.0/prefect_dbt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prefect-dbt
-Version: 0.4.3
+Version: 0.5.0
 Summary: Prefect integrations for working with dbt
 Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-dbt
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
@@ -16,16 +16,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prefect>=2.16.6
-Requires-Dist: dbt_core>=1.1.1
+Requires-Dist: prefect<3.0.0,>=2.16.6
+Requires-Dist: dbt-core>=1.7.0
 Requires-Dist: prefect_shell>=0.1.4
 Requires-Dist: sgqlc>=16.0.0
 Provides-Extra: snowflake
 Requires-Dist: prefect-snowflake>=0.2.4; extra == "snowflake"
 Requires-Dist: dbt-snowflake; extra == "snowflake"
 Provides-Extra: bigquery
 Requires-Dist: prefect-gcp[bigquery]>=0.1.8; extra == "bigquery"
```

### Comparing `prefect_dbt-0.4.3/prefect_dbt.egg-info/SOURCES.txt` & `prefect_dbt-0.5.0/prefect_dbt.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 prefect_dbt.egg-info/dependency_links.txt
 prefect_dbt.egg-info/entry_points.txt
 prefect_dbt.egg-info/requires.txt
 prefect_dbt.egg-info/top_level.txt
 prefect_dbt/cli/__init__.py
 prefect_dbt/cli/commands.py
 prefect_dbt/cli/credentials.py
-prefect_dbt/cli/tasks.py
 prefect_dbt/cli/configs/__init__.py
 prefect_dbt/cli/configs/base.py
 prefect_dbt/cli/configs/bigquery.py
 prefect_dbt/cli/configs/postgres.py
 prefect_dbt/cli/configs/snowflake.py
 prefect_dbt/cloud/__init__.py
 prefect_dbt/cloud/clients.py
@@ -28,15 +27,14 @@
 prefect_dbt/cloud/runs.py
 prefect_dbt/cloud/utils.py
 tests/conftest.py
 tests/test_block_standards.py
 tests/test_version.py
 tests/cli/test_commands.py
 tests/cli/test_credentials.py
-tests/cli/test_tasks.py
 tests/cli/configs/test_base.py
 tests/cli/configs/test_bigquery.py
 tests/cli/configs/test_postgres.py
 tests/cli/configs/test_snowflake.py
 tests/cloud/test_clients.py
 tests/cloud/test_cloud_credentials.py
 tests/cloud/test_jobs.py
```

### Comparing `prefect_dbt-0.4.3/pyproject.toml` & `prefect_dbt-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Software Development :: Libraries",
 ]
 dependencies = [
-  "prefect>=2.16.6",
-  "dbt_core>=1.1.1",
+  "prefect>=2.16.6, < 3.0.0",
+  "dbt-core>=1.7.0",
   "prefect_shell>=0.1.4",
   "sgqlc>=16.0.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 snowflake = ["prefect-snowflake>=0.2.4", "dbt-snowflake"]
```

### Comparing `prefect_dbt-0.4.3/tests/cli/configs/test_base.py` & `prefect_dbt-0.5.0/tests/cli/configs/test_base.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/tests/cli/configs/test_bigquery.py` & `prefect_dbt-0.5.0/tests/cli/configs/test_bigquery.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/tests/cli/configs/test_postgres.py` & `prefect_dbt-0.5.0/tests/cli/configs/test_postgres.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/tests/cli/configs/test_snowflake.py` & `prefect_dbt-0.5.0/tests/cli/configs/test_snowflake.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/tests/cli/test_credentials.py` & `prefect_dbt-0.5.0/tests/cli/test_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/tests/cloud/test_clients.py` & `prefect_dbt-0.5.0/tests/cloud/test_clients.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/tests/cloud/test_cloud_credentials.py` & `prefect_dbt-0.5.0/tests/cloud/test_cloud_credentials.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/tests/cloud/test_jobs.py` & `prefect_dbt-0.5.0/tests/cloud/test_jobs.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/tests/cloud/test_runs.py` & `prefect_dbt-0.5.0/tests/cloud/test_runs.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/tests/cloud/test_utils.py` & `prefect_dbt-0.5.0/tests/cloud/test_utils.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/tests/conftest.py` & `prefect_dbt-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `prefect_dbt-0.4.3/tests/test_block_standards.py` & `prefect_dbt-0.5.0/tests/test_block_standards.py`

 * *Files identical despite different names*

