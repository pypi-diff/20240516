# Comparing `tmp/dagworks_sdk-0.5.3.tar.gz` & `tmp/dagworks_sdk-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagworks_sdk-0.5.3.tar", last modified: Fri Apr 26 05:50:59 2024, max compression
+gzip compressed data, was "dagworks_sdk-0.5.4.tar", last modified: Thu May 16 15:39:05 2024, max compression
```

## Comparing `dagworks_sdk-0.5.3.tar` & `dagworks_sdk-0.5.4.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.904316 dagworks_sdk-0.5.3/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2212 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/LICENSE
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4983 2024-04-26 05:50:59.903652 dagworks_sdk-0.5.3/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3655 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/README.md
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1898 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/pyproject.toml
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       18 2024-01-05 22:27:57.000000 dagworks_sdk-0.5.3/requirements-test.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       69 2024-01-05 22:27:57.000000 dagworks_sdk-0.5.3/requirements.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       38 2024-04-26 05:50:59.904463 dagworks_sdk-0.5.3/setup.cfg
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      115 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/setup.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.858364 dagworks_sdk-0.5.3/src/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.862045 dagworks_sdk-0.5.3/src/dagworks/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1092 2024-04-26 05:50:34.000000 dagworks_sdk-0.5.3/src/dagworks/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    26332 2024-03-28 06:18:44.000000 dagworks_sdk-0.5.3/src/dagworks/adapters.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.864936 dagworks_sdk-0.5.3/src/dagworks/api/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2024-04-21 23:21:37.000000 dagworks_sdk-0.5.3/src/dagworks/api/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    32935 2024-01-06 04:40:53.000000 dagworks_sdk-0.5.3/src/dagworks/api/clients.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1161 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/api/constants.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1311 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/api/projecttypes.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.866151 dagworks_sdk-0.5.3/src/dagworks/cli/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2025 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/cli.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6513 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/initialize.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.866822 dagworks_sdk-0.5.3/src/dagworks/cli/templates/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/__init__.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.869045 dagworks_sdk-0.5.3/src/dagworks/cli/templates/common/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      123 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/common/.env.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      307 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/common/README.md.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       51 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/common/requirements.txt.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2698 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/common/run.py.jinja2
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      697 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/common/run.sh.jinja2
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.869423 dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.871396 dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      351 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      520 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/components/common.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2528 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/components/data_loader.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.872198 dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/config/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       26 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/config/config.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.874309 dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      232 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/data/order_details.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      480 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/data/orders_new.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      309 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/data/orders_old.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      678 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.874891 dagworks_sdk-0.5.3/src/dagworks/cli/templates/hello_world/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.875696 dagworks_sdk-0.5.3/src/dagworks/cli/templates/hello_world/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/hello_world/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1577 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/hello_world/components/transforms.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.876460 dagworks_sdk-0.5.3/src/dagworks/cli/templates/hello_world/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      157 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/hello_world/data/signups.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      149 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/hello_world/data/spend.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      674 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/hello_world/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.876814 dagworks_sdk-0.5.3/src/dagworks/cli/templates/machine_learning/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.878879 dagworks_sdk-0.5.3/src/dagworks/cli/templates/machine_learning/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/machine_learning/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      488 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/machine_learning/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3736 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      598 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/machine_learning/components/iris_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2531 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/machine_learning/components/model_fitting.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1402 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/machine_learning/components/models.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      477 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/machine_learning/template_data.json
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.879227 dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.882385 dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/components/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        0 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/components/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1447 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      369 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/components/data_loader.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      710 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      931 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      744 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.882744 dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/data/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)   991302 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      679 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)    34017 2024-04-26 05:50:34.000000 dagworks_sdk-0.5.3/src/dagworks/driver.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.886626 dagworks_sdk-0.5.3/src/dagworks/telemetry/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/telemetry/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7465 2024-01-04 21:15:26.000000 dagworks_sdk-0.5.3/src/dagworks/telemetry/telemetry.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.896040 dagworks_sdk-0.5.3/src/dagworks/tracking/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1067 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/tracking/__init__.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3468 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/tracking/dataframe_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     1640 2024-03-28 06:09:29.000000 dagworks_sdk-0.5.3/src/dagworks/tracking/dw_pydantic.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5969 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/src/dagworks/tracking/example_tracking.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2131 2024-01-05 22:27:57.000000 dagworks_sdk-0.5.3/src/dagworks/tracking/numpy_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6505 2024-01-05 22:27:57.000000 dagworks_sdk-0.5.3/src/dagworks/tracking/pandas_col_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5892 2024-01-05 22:27:57.000000 dagworks_sdk-0.5.3/src/dagworks/tracking/pandas_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7471 2024-02-21 06:46:10.000000 dagworks_sdk-0.5.3/src/dagworks/tracking/polars_col_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     5741 2024-02-21 06:01:43.000000 dagworks_sdk-0.5.3/src/dagworks/tracking/polars_stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9615 2024-03-28 06:09:29.000000 dagworks_sdk-0.5.3/src/dagworks/tracking/runs.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)      638 2023-11-01 23:28:17.000000 dagworks_sdk-0.5.3/src/dagworks/tracking/sql_utils.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     7300 2024-01-05 22:27:57.000000 dagworks_sdk-0.5.3/src/dagworks/tracking/stats.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2496 2024-01-06 04:40:53.000000 dagworks_sdk-0.5.3/src/dagworks/tracking/trackingtypes.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     2262 2024-04-26 05:36:38.000000 dagworks_sdk-0.5.3/src/dagworks/tracking/utils.py
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.902240 dagworks_sdk-0.5.3/src/dagworks_sdk.egg-info/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     4983 2024-04-26 05:50:59.000000 dagworks_sdk-0.5.3/src/dagworks_sdk.egg-info/PKG-INFO
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3590 2024-04-26 05:50:59.000000 dagworks_sdk-0.5.3/src/dagworks_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        1 2024-04-26 05:50:59.000000 dagworks_sdk-0.5.3/src/dagworks_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       50 2024-04-26 05:50:59.000000 dagworks_sdk-0.5.3/src/dagworks_sdk.egg-info/entry_points.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)       95 2024-04-26 05:50:59.000000 dagworks_sdk-0.5.3/src/dagworks_sdk.egg-info/requires.txt
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)        9 2024-04-26 05:50:59.000000 dagworks_sdk-0.5.3/src/dagworks_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 stefankrawczyk   (501) staff       (20)        0 2024-04-26 05:50:59.901321 dagworks_sdk-0.5.3/tests/
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     6442 2024-02-21 06:46:10.000000 dagworks_sdk-0.5.3/tests/test_adapters.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3531 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/tests/test_driver.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     3343 2023-11-01 21:33:20.000000 dagworks_sdk-0.5.3/tests/test_telemetry.py
--rw-r--r--   0 stefankrawczyk   (501) staff       (20)     9584 2024-01-06 04:40:53.000000 dagworks_sdk-0.5.3/tests/test_tracking.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.766669 dagworks_sdk-0.5.4/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2212 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/LICENSE
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4983 2024-05-16 15:39:05.766416 dagworks_sdk-0.5.4/PKG-INFO
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3655 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/README.md
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1898 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/pyproject.toml
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       18 2024-02-13 04:20:57.000000 dagworks_sdk-0.5.4/requirements-test.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       69 2024-02-13 04:20:57.000000 dagworks_sdk-0.5.4/requirements.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       38 2024-05-16 15:39:05.766709 dagworks_sdk-0.5.4/setup.cfg
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      115 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/setup.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.742558 dagworks_sdk-0.5.4/src/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.744396 dagworks_sdk-0.5.4/src/dagworks/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1092 2024-05-16 15:38:55.000000 dagworks_sdk-0.5.4/src/dagworks/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)    26332 2024-05-16 15:33:17.000000 dagworks_sdk-0.5.4/src/dagworks/adapters.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.745766 dagworks_sdk-0.5.4/src/dagworks/api/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/api/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)    32935 2024-02-13 04:20:57.000000 dagworks_sdk-0.5.4/src/dagworks/api/clients.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1161 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/api/constants.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1311 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/api/projecttypes.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.746321 dagworks_sdk-0.5.4/src/dagworks/cli/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2025 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/cli.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6513 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/initialize.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.746581 dagworks_sdk-0.5.4/src/dagworks/cli/templates/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/__init__.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.747583 dagworks_sdk-0.5.4/src/dagworks/cli/templates/common/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      123 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/common/.env.jinja2
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      307 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/common/README.md.jinja2
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       51 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/common/requirements.txt.jinja2
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2698 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/common/run.py.jinja2
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      697 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/common/run.sh.jinja2
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.747750 dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.748345 dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/components/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/components/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      351 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/components/_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      520 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/components/common.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2528 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/components/data_loader.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.748502 dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/config/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       26 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/config/config.json
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.748920 dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/data/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      232 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/data/order_details.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      480 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/data/orders_new.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      309 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/data/orders_old.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      678 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/template_data.json
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.749064 dagworks_sdk-0.5.4/src/dagworks/cli/templates/hello_world/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.749300 dagworks_sdk-0.5.4/src/dagworks/cli/templates/hello_world/components/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/hello_world/components/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1577 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/hello_world/components/transforms.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.749592 dagworks_sdk-0.5.4/src/dagworks/cli/templates/hello_world/data/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      157 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/hello_world/data/signups.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      149 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/hello_world/data/spend.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      674 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/hello_world/template_data.json
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.749735 dagworks_sdk-0.5.4/src/dagworks/cli/templates/machine_learning/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.750628 dagworks_sdk-0.5.4/src/dagworks/cli/templates/machine_learning/components/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/machine_learning/components/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      488 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/machine_learning/components/_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3736 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      598 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/machine_learning/components/iris_loader.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2531 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/machine_learning/components/model_fitting.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1402 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/machine_learning/components/models.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      477 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/machine_learning/template_data.json
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.754467 dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.755762 dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/components/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        0 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/components/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1447 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      369 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/components/data_loader.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      710 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      931 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      744 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.755920 dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/data/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)   991302 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      679 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)    34591 2024-05-16 15:38:55.000000 dagworks_sdk-0.5.4/src/dagworks/driver.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.759341 dagworks_sdk-0.5.4/src/dagworks/telemetry/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/telemetry/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7465 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/telemetry/telemetry.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.764170 dagworks_sdk-0.5.4/src/dagworks/tracking/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1067 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/tracking/__init__.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3468 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/tracking/dataframe_stats.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     1640 2024-05-16 15:33:17.000000 dagworks_sdk-0.5.4/src/dagworks/tracking/dw_pydantic.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5969 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/src/dagworks/tracking/example_tracking.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2131 2024-02-13 04:20:57.000000 dagworks_sdk-0.5.4/src/dagworks/tracking/numpy_stats.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6505 2024-02-13 04:20:57.000000 dagworks_sdk-0.5.4/src/dagworks/tracking/pandas_col_stats.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5892 2024-02-13 04:20:57.000000 dagworks_sdk-0.5.4/src/dagworks/tracking/pandas_stats.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7471 2024-05-16 15:33:17.000000 dagworks_sdk-0.5.4/src/dagworks/tracking/polars_col_stats.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     5741 2024-02-13 04:20:57.000000 dagworks_sdk-0.5.4/src/dagworks/tracking/polars_stats.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     9615 2024-05-16 15:33:17.000000 dagworks_sdk-0.5.4/src/dagworks/tracking/runs.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)      638 2023-12-27 21:47:08.000000 dagworks_sdk-0.5.4/src/dagworks/tracking/sql_utils.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     7300 2024-02-13 04:20:57.000000 dagworks_sdk-0.5.4/src/dagworks/tracking/stats.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2496 2024-02-13 04:20:57.000000 dagworks_sdk-0.5.4/src/dagworks/tracking/trackingtypes.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     2262 2024-05-16 15:33:17.000000 dagworks_sdk-0.5.4/src/dagworks/tracking/utils.py
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.765914 dagworks_sdk-0.5.4/src/dagworks_sdk.egg-info/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     4983 2024-05-16 15:39:05.000000 dagworks_sdk-0.5.4/src/dagworks_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3590 2024-05-16 15:39:05.000000 dagworks_sdk-0.5.4/src/dagworks_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        1 2024-05-16 15:39:05.000000 dagworks_sdk-0.5.4/src/dagworks_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       50 2024-05-16 15:39:05.000000 dagworks_sdk-0.5.4/src/dagworks_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)       95 2024-05-16 15:39:05.000000 dagworks_sdk-0.5.4/src/dagworks_sdk.egg-info/requires.txt
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)        9 2024-05-16 15:39:05.000000 dagworks_sdk-0.5.4/src/dagworks_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 elijahbenizzy   (501) staff       (20)        0 2024-05-16 15:39:05.765612 dagworks_sdk-0.5.4/tests/
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     6442 2024-05-16 15:33:17.000000 dagworks_sdk-0.5.4/tests/test_adapters.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3531 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/tests/test_driver.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     3343 2023-10-14 00:25:16.000000 dagworks_sdk-0.5.4/tests/test_telemetry.py
+-rw-r--r--   0 elijahbenizzy   (501) staff       (20)     9584 2024-02-13 04:20:57.000000 dagworks_sdk-0.5.4/tests/test_tracking.py
```

### Comparing `dagworks_sdk-0.5.3/LICENSE` & `dagworks_sdk-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/PKG-INFO` & `dagworks_sdk-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagworks-sdk
-Version: 0.5.3
+Version: 0.5.4
 Summary: DAGWorks SDK.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://www.dagworks.io
 Project-URL: Bug Reports, https://docs.google.com/forms/d/e/1FAIpQLScS9YvcuNOTretZWXUdur8XNcJPpkJwZwzxuGfbPJKc8IRS6A/viewform
 Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/
 Project-URL: Documenation, https://docs.dagworks.io/
 Keywords: hamilton,dagworks,observability
```

### Comparing `dagworks_sdk-0.5.3/README.md` & `dagworks_sdk-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/pyproject.toml` & `dagworks_sdk-0.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/__init__.py` & `dagworks_sdk-0.5.4/src/dagworks/api/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-__version__ = (0, 5, 3)
+DAGWORKS_API_URL = "https://api.app.dagworks.io"
+DAGWORKS_UI_URL = "https://app.dagworks.io"
```

### Comparing `dagworks_sdk-0.5.3/src/dagworks/adapters.py` & `dagworks_sdk-0.5.4/src/dagworks/adapters.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/api/__init__.py` & `dagworks_sdk-0.5.4/src/dagworks/api/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/api/clients.py` & `dagworks_sdk-0.5.4/src/dagworks/api/clients.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/api/constants.py` & `dagworks_sdk-0.5.4/src/dagworks/cli/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,10 +13,7 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
-DAGWORKS_API_URL = "https://api.app.dagworks.io"
-DAGWORKS_UI_URL = "https://app.dagworks.io"
```

### Comparing `dagworks_sdk-0.5.3/src/dagworks/api/projecttypes.py` & `dagworks_sdk-0.5.4/src/dagworks/api/projecttypes.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/__init__.py` & `dagworks_sdk-0.5.4/src/dagworks/telemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/cli.py` & `dagworks_sdk-0.5.4/src/dagworks/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/initialize.py` & `dagworks_sdk-0.5.4/src/dagworks/cli/initialize.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/common/run.py.jinja2` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/common/run.py.jinja2`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/common/run.sh.jinja2` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/common/run.sh.jinja2`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/components/common.py` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/components/common.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/components/data_loader.py` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/components/data_loader.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/data_processing/template_data.json` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/data_processing/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/hello_world/components/transforms.py` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/hello_world/components/transforms.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/hello_world/template_data.json` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/hello_world/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/machine_learning/components/feature_transforms.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/machine_learning/components/iris_loader.py` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/machine_learning/components/iris_loader.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/machine_learning/components/model_fitting.py` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/machine_learning/components/model_fitting.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/machine_learning/components/models.py` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/machine_learning/components/models.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/components/_run.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_autoregression.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_calendar.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/components/ftrs_common_prep.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/data/train_sample.csv`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json` & `dagworks_sdk-0.5.4/src/dagworks/cli/templates/time_series_feature_engineering/template_data.json`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/driver.py` & `dagworks_sdk-0.5.4/src/dagworks/driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -168,16 +168,28 @@
 
     commit = repo.head.commit
     try:
         repo_url = repo.remote().url
     except ValueError:
         # TODO: change this to point to our docs on what to do.
         repo_url = "Error: No repository to link to."
+    try:
+        branch_name = repo.active_branch.name
+    except TypeError:
+        branch_name = "unknown"  # detached head
+        logger.warning(
+            "Warning: we are unable to determine the branch name. "
+            "This is likely because you are in a detached head state. "
+            "If you are in a detached head state, you can check out a "
+            "branch by running `git checkout -b <branch_name>`. "
+            "If you intend to be (if you are using some sort of CI"
+            "system that checks out a detached head) then you can ignore this."
+        )
     return GitInfo(
-        branch=repo.active_branch.name,
+        branch=branch_name,
         commit_hash=commit.hexsha,
         committed=not repo.is_dirty(),
         repository=repo_url,
         local_repo_base_path=repo.working_dir,
     )
```

### Comparing `dagworks_sdk-0.5.3/src/dagworks/telemetry/__init__.py` & `dagworks_sdk-0.5.4/src/dagworks/tracking/__init__.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/telemetry/telemetry.py` & `dagworks_sdk-0.5.4/src/dagworks/telemetry/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/tracking/__init__.py` & `dagworks_sdk-0.5.4/src/dagworks/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,7 +13,9 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
+__version__ = (0, 5, 4)
```

### Comparing `dagworks_sdk-0.5.3/src/dagworks/tracking/dataframe_stats.py` & `dagworks_sdk-0.5.4/src/dagworks/tracking/dataframe_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/tracking/dw_pydantic.py` & `dagworks_sdk-0.5.4/src/dagworks/tracking/dw_pydantic.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/tracking/example_tracking.py` & `dagworks_sdk-0.5.4/src/dagworks/tracking/example_tracking.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/tracking/numpy_stats.py` & `dagworks_sdk-0.5.4/src/dagworks/tracking/numpy_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/tracking/pandas_col_stats.py` & `dagworks_sdk-0.5.4/src/dagworks/tracking/pandas_col_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/tracking/pandas_stats.py` & `dagworks_sdk-0.5.4/src/dagworks/tracking/pandas_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/tracking/polars_col_stats.py` & `dagworks_sdk-0.5.4/src/dagworks/tracking/polars_col_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/tracking/polars_stats.py` & `dagworks_sdk-0.5.4/src/dagworks/tracking/polars_stats.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/tracking/runs.py` & `dagworks_sdk-0.5.4/src/dagworks/tracking/runs.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/tracking/sql_utils.py` & `dagworks_sdk-0.5.4/src/dagworks/tracking/sql_utils.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/tracking/stats.py` & `dagworks_sdk-0.5.4/src/dagworks/tracking/stats.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/tracking/trackingtypes.py` & `dagworks_sdk-0.5.4/src/dagworks/tracking/trackingtypes.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks/tracking/utils.py` & `dagworks_sdk-0.5.4/src/dagworks/tracking/utils.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/src/dagworks_sdk.egg-info/PKG-INFO` & `dagworks_sdk-0.5.4/src/dagworks_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagworks-sdk
-Version: 0.5.3
+Version: 0.5.4
 Summary: DAGWorks SDK.
 Author-email: Stefan Krawczyk <stefan@dagworks.io>, Elijah ben Izzy <elijah@dagworks.io>
 Project-URL: Homepage, https://www.dagworks.io
 Project-URL: Bug Reports, https://docs.google.com/forms/d/e/1FAIpQLScS9YvcuNOTretZWXUdur8XNcJPpkJwZwzxuGfbPJKc8IRS6A/viewform
 Project-URL: Source, https://github.com/dagworks-inc/dagworks-sdk/
 Project-URL: Documenation, https://docs.dagworks.io/
 Keywords: hamilton,dagworks,observability
```

### Comparing `dagworks_sdk-0.5.3/src/dagworks_sdk.egg-info/SOURCES.txt` & `dagworks_sdk-0.5.4/src/dagworks_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/tests/test_adapters.py` & `dagworks_sdk-0.5.4/tests/test_adapters.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/tests/test_driver.py` & `dagworks_sdk-0.5.4/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/tests/test_telemetry.py` & `dagworks_sdk-0.5.4/tests/test_telemetry.py`

 * *Files identical despite different names*

### Comparing `dagworks_sdk-0.5.3/tests/test_tracking.py` & `dagworks_sdk-0.5.4/tests/test_tracking.py`

 * *Files identical despite different names*

