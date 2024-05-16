# Comparing `tmp/dominodatalab-1.4.0.tar.gz` & `tmp/dominodatalab-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dominodatalab-1.4.0.tar", last modified: Tue Apr 30 14:03:10 2024, max compression
+gzip compressed data, was "dominodatalab-1.4.1.tar", last modified: Thu May 16 17:17:36 2024, max compression
```

## Comparing `dominodatalab-1.4.0.tar` & `dominodatalab-1.4.1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.223392 dominodatalab-1.4.0/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    11358 2022-06-06 14:00:07.000000 dominodatalab-1.4.0/LICENSE.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)       14 2022-06-21 20:35:17.000000 dominodatalab-1.4.0/MANIFEST.in
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    30459 2024-04-30 14:03:10.221122 dominodatalab-1.4.0/PKG-INFO
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    28944 2024-04-30 12:48:57.000000 dominodatalab-1.4.0/README.md
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.014395 dominodatalab-1.4.0/domino/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      105 2022-06-21 20:35:17.000000 dominodatalab-1.4.0/domino/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9576 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_custom_metrics.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.016384 dominodatalab-1.4.0/domino/_impl/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)        0 2022-10-18 20:07:39.000000 dominodatalab-1.4.0/domino/_impl/__init__.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.033306 dominodatalab-1.4.0/domino/_impl/custommetrics/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      821 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    58419 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/api_client.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.044702 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      214 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      972 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/path_to_api.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.052424 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/paths/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      253 2022-10-18 20:07:39.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/paths/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      137 2022-10-18 20:07:39.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/paths/api_metric_alerts_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      137 2022-10-18 20:07:39.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/paths/api_metric_values_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      184 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/paths/api_metric_values_v1_model_monitoring_id_metric.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      383 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/tag_to_api.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.056223 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/tags/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      336 2022-10-18 20:07:39.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/tags/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      750 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/apis/tags/custom_metrics_api.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    15937 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/configuration.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4416 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/exceptions.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.100222 dominodatalab-1.4.0/domino/_impl/custommetrics/model/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      360 2022-10-18 20:07:39.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3798 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/failure_envelope_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3798 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/failure_envelope_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2463 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/invalid_body_envelope_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2463 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/invalid_body_envelope_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3801 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metadata_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3801 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metadata_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4856 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_alert_request_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4888 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_alert_request_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2871 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_tag_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2871 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_tag_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4529 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_value_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4561 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_value_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4054 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_values_envelope_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4118 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_values_envelope_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     5730 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_value_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     5762 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_value_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3557 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3589 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4848 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/target_range_v1.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     4449 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/model/target_range_v1.pyi
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.102229 dominodatalab-1.4.0/domino/_impl/custommetrics/models/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     1236 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/models/__init__.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.104818 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      508 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/__init__.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.109647 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      351 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    15351 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    15120 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.pyi
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.114092 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      351 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    15377 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1/post.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    15146 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1/post.pyi
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.145291 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      405 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    16879 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    16648 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.pyi
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    10493 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/rest.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    96843 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/_impl/custommetrics/schemas.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)       22 2024-04-30 12:33:26.000000 dominodatalab-1.4.0/domino/_version.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.164659 dominodatalab-1.4.0/domino/airflow/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      259 2022-06-21 20:35:17.000000 dominodatalab-1.4.0/domino/airflow/__init__.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    11462 2023-01-05 19:13:36.000000 dominodatalab-1.4.0/domino/airflow/_operator.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3612 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/domino/authentication.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     1513 2024-04-24 12:43:48.000000 dominodatalab-1.4.0/domino/constants.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      723 2022-07-27 14:46:07.000000 dominodatalab-1.4.0/domino/data_sources.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9038 2024-01-19 15:58:01.000000 dominodatalab-1.4.0/domino/datasets.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    69419 2024-04-30 12:15:28.000000 dominodatalab-1.4.0/domino/domino.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      437 2024-04-30 12:15:28.000000 dominodatalab-1.4.0/domino/domino_enums.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     1626 2022-07-06 17:07:45.000000 dominodatalab-1.4.0/domino/exceptions.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2426 2022-08-22 21:15:27.000000 dominodatalab-1.4.0/domino/helpers.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3408 2024-04-29 13:03:50.000000 dominodatalab-1.4.0/domino/http_request_manager.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    10594 2024-04-30 12:15:28.000000 dominodatalab-1.4.0/domino/routes.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      787 2022-06-21 20:35:17.000000 dominodatalab-1.4.0/domino/training_sets.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.214326 dominodatalab-1.4.0/dominodatalab.egg-info/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)    30459 2024-04-30 14:03:09.000000 dominodatalab-1.4.0/dominodatalab.egg-info/PKG-INFO
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3584 2024-04-30 14:03:09.000000 dominodatalab-1.4.0/dominodatalab.egg-info/SOURCES.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)        1 2024-04-30 14:03:09.000000 dominodatalab-1.4.0/dominodatalab.egg-info/dependency_links.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      424 2024-04-30 14:03:09.000000 dominodatalab-1.4.0/dominodatalab.egg-info/requires.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)        7 2024-04-30 14:03:09.000000 dominodatalab-1.4.0/dominodatalab.egg-info/top_level.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      879 2024-04-30 14:02:11.000000 dominodatalab-1.4.0/requirements.txt
--rw-r--r--   0 olson.dimanche   (503) staff       (20)       38 2024-04-30 14:03:10.223650 dominodatalab-1.4.0/setup.cfg
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2184 2024-04-19 14:44:50.000000 dominodatalab-1.4.0/setup.py
-drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-04-30 14:03:10.212525 dominodatalab-1.4.0/tests/
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9973 2024-04-30 12:15:28.000000 dominodatalab-1.4.0/tests/test_basic_auth.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      675 2022-08-22 21:15:27.000000 dominodatalab-1.4.0/tests/test_data_sources.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     5183 2024-04-19 12:44:33.000000 dominodatalab-1.4.0/tests/test_datasets.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     1321 2024-04-30 12:15:28.000000 dominodatalab-1.4.0/tests/test_domino.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2015 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/tests/test_environments.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9013 2024-04-30 12:15:28.000000 dominodatalab-1.4.0/tests/test_finops.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9142 2024-04-19 12:44:33.000000 dominodatalab-1.4.0/tests/test_jobs.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     1969 2022-06-21 20:35:17.000000 dominodatalab-1.4.0/tests/test_models.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)      505 2022-08-22 21:15:27.000000 dominodatalab-1.4.0/tests/test_no_data_sources.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     2280 2023-03-20 13:24:47.000000 dominodatalab-1.4.0/tests/test_operator.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     9614 2023-12-14 22:20:12.000000 dominodatalab-1.4.0/tests/test_projects.py
--rw-r--r--   0 olson.dimanche   (503) staff       (20)     3472 2024-04-19 12:44:33.000000 dominodatalab-1.4.0/tests/test_spark_operator.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.356902 dominodatalab-1.4.1/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    11358 2022-06-06 14:00:07.000000 dominodatalab-1.4.1/LICENSE.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)       14 2022-06-21 20:35:17.000000 dominodatalab-1.4.1/MANIFEST.in
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    30521 2024-05-16 17:17:36.356128 dominodatalab-1.4.1/PKG-INFO
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    29006 2024-05-16 16:55:17.000000 dominodatalab-1.4.1/README.md
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.218465 dominodatalab-1.4.1/domino/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      105 2022-06-21 20:35:17.000000 dominodatalab-1.4.1/domino/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9576 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_custom_metrics.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.219363 dominodatalab-1.4.1/domino/_impl/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)        0 2022-10-18 20:07:39.000000 dominodatalab-1.4.1/domino/_impl/__init__.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.234245 dominodatalab-1.4.1/domino/_impl/custommetrics/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      821 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    58419 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/api_client.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.242575 dominodatalab-1.4.1/domino/_impl/custommetrics/apis/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      214 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/apis/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      972 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/apis/path_to_api.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.254783 dominodatalab-1.4.1/domino/_impl/custommetrics/apis/paths/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      253 2022-10-18 20:07:39.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/apis/paths/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      137 2022-10-18 20:07:39.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/apis/paths/api_metric_alerts_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      137 2022-10-18 20:07:39.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/apis/paths/api_metric_values_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      184 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/apis/paths/api_metric_values_v1_model_monitoring_id_metric.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      383 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/apis/tag_to_api.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.258876 dominodatalab-1.4.1/domino/_impl/custommetrics/apis/tags/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      336 2022-10-18 20:07:39.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/apis/tags/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      750 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/apis/tags/custom_metrics_api.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    15937 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/configuration.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4416 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/exceptions.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.312455 dominodatalab-1.4.1/domino/_impl/custommetrics/model/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      360 2022-10-18 20:07:39.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3798 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/failure_envelope_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3798 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/failure_envelope_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2463 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/invalid_body_envelope_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2463 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/invalid_body_envelope_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3801 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/metadata_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3801 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/metadata_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4856 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_alert_request_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4888 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_alert_request_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2871 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_tag_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2871 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_tag_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4529 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_value_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4561 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_value_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4054 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_values_envelope_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4118 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_values_envelope_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     5730 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/new_metric_value_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     5762 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/new_metric_value_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3557 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3589 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4848 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/target_range_v1.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     4449 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/model/target_range_v1.pyi
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.314327 dominodatalab-1.4.1/domino/_impl/custommetrics/models/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     1236 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/models/__init__.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.315886 dominodatalab-1.4.1/domino/_impl/custommetrics/paths/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      508 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/paths/__init__.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.320523 dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      351 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    15351 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    15120 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.pyi
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.325567 dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_values_v1/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      351 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_values_v1/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    15377 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_values_v1/post.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    15146 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_values_v1/post.pyi
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.330917 dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      405 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    16879 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    16648 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.pyi
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    10493 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/rest.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    96843 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/_impl/custommetrics/schemas.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)       22 2024-05-16 16:21:53.000000 dominodatalab-1.4.1/domino/_version.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.334706 dominodatalab-1.4.1/domino/airflow/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      259 2022-06-21 20:35:17.000000 dominodatalab-1.4.1/domino/airflow/__init__.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    11462 2023-01-05 19:13:36.000000 dominodatalab-1.4.1/domino/airflow/_operator.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3612 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/domino/authentication.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     1513 2024-04-24 12:43:48.000000 dominodatalab-1.4.1/domino/constants.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      723 2022-07-27 14:46:07.000000 dominodatalab-1.4.1/domino/data_sources.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9038 2024-01-19 15:58:01.000000 dominodatalab-1.4.1/domino/datasets.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    69419 2024-04-30 12:15:28.000000 dominodatalab-1.4.1/domino/domino.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      437 2024-04-30 12:15:28.000000 dominodatalab-1.4.1/domino/domino_enums.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     1626 2022-07-06 17:07:45.000000 dominodatalab-1.4.1/domino/exceptions.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2426 2022-08-22 21:15:27.000000 dominodatalab-1.4.1/domino/helpers.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3408 2024-04-29 13:03:50.000000 dominodatalab-1.4.1/domino/http_request_manager.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    10594 2024-04-30 12:15:28.000000 dominodatalab-1.4.1/domino/routes.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      787 2022-06-21 20:35:17.000000 dominodatalab-1.4.1/domino/training_sets.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.352294 dominodatalab-1.4.1/dominodatalab.egg-info/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)    30521 2024-05-16 17:17:36.000000 dominodatalab-1.4.1/dominodatalab.egg-info/PKG-INFO
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3584 2024-05-16 17:17:36.000000 dominodatalab-1.4.1/dominodatalab.egg-info/SOURCES.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)        1 2024-05-16 17:17:36.000000 dominodatalab-1.4.1/dominodatalab.egg-info/dependency_links.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      424 2024-05-16 17:17:36.000000 dominodatalab-1.4.1/dominodatalab.egg-info/requires.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)        7 2024-05-16 17:17:36.000000 dominodatalab-1.4.1/dominodatalab.egg-info/top_level.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      879 2024-05-16 17:16:48.000000 dominodatalab-1.4.1/requirements.txt
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)       38 2024-05-16 17:17:36.357058 dominodatalab-1.4.1/setup.cfg
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2184 2024-05-16 16:09:23.000000 dominodatalab-1.4.1/setup.py
+drwxr-xr-x   0 olson.dimanche   (503) staff       (20)        0 2024-05-16 17:17:36.351281 dominodatalab-1.4.1/tests/
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9973 2024-04-30 12:15:28.000000 dominodatalab-1.4.1/tests/test_basic_auth.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      675 2022-08-22 21:15:27.000000 dominodatalab-1.4.1/tests/test_data_sources.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     5183 2024-04-19 12:44:33.000000 dominodatalab-1.4.1/tests/test_datasets.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     1321 2024-04-30 12:15:28.000000 dominodatalab-1.4.1/tests/test_domino.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2015 2023-03-20 13:24:47.000000 dominodatalab-1.4.1/tests/test_environments.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9013 2024-04-30 12:15:28.000000 dominodatalab-1.4.1/tests/test_finops.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9142 2024-04-19 12:44:33.000000 dominodatalab-1.4.1/tests/test_jobs.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     1969 2022-06-21 20:35:17.000000 dominodatalab-1.4.1/tests/test_models.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)      505 2022-08-22 21:15:27.000000 dominodatalab-1.4.1/tests/test_no_data_sources.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     2280 2024-05-16 15:58:04.000000 dominodatalab-1.4.1/tests/test_operator.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     9614 2023-12-14 22:20:12.000000 dominodatalab-1.4.1/tests/test_projects.py
+-rw-r--r--   0 olson.dimanche   (503) staff       (20)     3472 2024-04-19 12:44:33.000000 dominodatalab-1.4.1/tests/test_spark_operator.py
```

### Comparing `dominodatalab-1.4.0/LICENSE.txt` & `dominodatalab-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/PKG-INFO` & `dominodatalab-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: dominodatalab
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python bindings for the Domino API
 Home-page: https://github.com/dominodatalab/python-domino
-Download-URL: https://github.com/dominodatalab/python-domino/archive/release-1.4.0.zip
+Download-URL: https://github.com/dominodatalab/python-domino/archive/release-1.4.1.zip
 Author: Domino Data Lab
 Author-email: support@dominodatalab.com
 License: Apache Software License (Apache 2.0)
 Keywords: Domino Data Lab,API
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: packaging
 Requires-Dist: requests>=2.4.2
 Requires-Dist: beautifulsoup4~=4.11
 Requires-Dist: polling2~=0.5.0
 Requires-Dist: urllib3~=1.26.12
-Requires-Dist: typing-extensions~=4.4.0
+Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: frozendict~=2.3.4
 Requires-Dist: python-dateutil~=2.8.2
 Requires-Dist: retry==0.9.2
 Provides-Extra: airflow
 Requires-Dist: apache-airflow==2.2.4; extra == "airflow"
 Provides-Extra: data
 Requires-Dist: dominodatalab-data>=0.1.0; extra == "data"
@@ -43,29 +43,29 @@
 See this documentation for details about the APIs:
 
 -   [Latest public Domino
     APIs](https://docs.dominodatalab.com/en/latest/api_guide/8c929e/domino-public-apis/)
 
 -   [Legacy APIs](https://dominodatalab.github.io/api-docs/)
 
-The latest released version of `python-domino` is `1.4.0`.
+The latest released version of `python-domino` is `1.4.1`.
 
 # Version compatibility matrix
 
 The `python-domino` library is compatible with different versions of
 Domino:
 
-| Domino Versions |                                    Python-Domino                                    |
-|-----------------|:-----------------------------------------------------------------------------------:|
-| 3.6.x or lower  |      [0.3.5](https://github.com/dominodatalab/python-domino/archive/0.3.5.zip)       |
-| 4.1.0 or higher | [1.0.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/1.0.0.zip) or Higher |
-| 5.3.0 or higher | [1.2.0]https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.0.zip) or Higher |
+| Domino Versions |                                             Python-Domino                                             |
+|-----------------|:-----------------------------------------------------------------------------------------------------:|
+| 3.6.x or lower  |               [0.3.5](https://github.com/dominodatalab/python-domino/archive/0.3.5.zip)               |
+| 4.1.0 or higher |     [1.0.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/1.0.0.zip) or Higher     |
+| 5.3.0 or higher | [1.2.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.0.zip) or Higher |
 | 5.5.0 or higher | [1.2.2](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.2.zip) or Higher |
 | 5.10.0 or higher | [1.3.1](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.3.1.zip) or Higher |
-| 5.11.0 or higher | [1.4.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.4.0.zip) or Higher |
+| 5.11.0 or higher | [1.4.1](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.4.1.zip) or Higher |
 
 # Development
 
 The current `python-domino` is based on Python 3.9, which is therefore recommended for development. `Pipenv` is also recommended to manage the dependencies.
 
 To use the Python binding in a Domino workbook session, include `dominodatalab` in your project's requirements.txt file.
 This makes the Python binding available for each new workbook session (or batch run) started within the project.
```

### Comparing `dominodatalab-1.4.0/README.md` & `dominodatalab-1.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 See this documentation for details about the APIs:
 
 -   [Latest public Domino
     APIs](https://docs.dominodatalab.com/en/latest/api_guide/8c929e/domino-public-apis/)
 
 -   [Legacy APIs](https://dominodatalab.github.io/api-docs/)
 
-The latest released version of `python-domino` is `1.4.0`.
+The latest released version of `python-domino` is `1.4.1`.
 
 # Version compatibility matrix
 
 The `python-domino` library is compatible with different versions of
 Domino:
 
-| Domino Versions |                                    Python-Domino                                    |
-|-----------------|:-----------------------------------------------------------------------------------:|
-| 3.6.x or lower  |      [0.3.5](https://github.com/dominodatalab/python-domino/archive/0.3.5.zip)       |
-| 4.1.0 or higher | [1.0.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/1.0.0.zip) or Higher |
-| 5.3.0 or higher | [1.2.0]https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.0.zip) or Higher |
+| Domino Versions |                                             Python-Domino                                             |
+|-----------------|:-----------------------------------------------------------------------------------------------------:|
+| 3.6.x or lower  |               [0.3.5](https://github.com/dominodatalab/python-domino/archive/0.3.5.zip)               |
+| 4.1.0 or higher |     [1.0.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/1.0.0.zip) or Higher     |
+| 5.3.0 or higher | [1.2.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.0.zip) or Higher |
 | 5.5.0 or higher | [1.2.2](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.2.zip) or Higher |
 | 5.10.0 or higher | [1.3.1](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.3.1.zip) or Higher |
-| 5.11.0 or higher | [1.4.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.4.0.zip) or Higher |
+| 5.11.0 or higher | [1.4.1](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.4.1.zip) or Higher |
 
 # Development
 
 The current `python-domino` is based on Python 3.9, which is therefore recommended for development. `Pipenv` is also recommended to manage the dependencies.
 
 To use the Python binding in a Domino workbook session, include `dominodatalab` in your project's requirements.txt file.
 This makes the Python binding available for each new workbook session (or batch run) started within the project.
```

### Comparing `dominodatalab-1.4.0/domino/_custom_metrics.py` & `dominodatalab-1.4.1/domino/_custom_metrics.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/__init__.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/api_client.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/api_client.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/apis/path_to_api.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/apis/path_to_api.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/apis/tags/custom_metrics_api.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/apis/tags/custom_metrics_api.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/configuration.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/configuration.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/exceptions.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/exceptions.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/failure_envelope_v1.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/failure_envelope_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/failure_envelope_v1.pyi` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/failure_envelope_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/invalid_body_envelope_v1.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/invalid_body_envelope_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/invalid_body_envelope_v1.pyi` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/invalid_body_envelope_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metadata_v1.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/metadata_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metadata_v1.pyi` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/metadata_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_alert_request_v1.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_alert_request_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_alert_request_v1.pyi` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_alert_request_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_tag_v1.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_tag_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_tag_v1.pyi` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_tag_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_value_v1.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_value_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_value_v1.pyi` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_value_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_values_envelope_v1.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_values_envelope_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/metric_values_envelope_v1.pyi` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/metric_values_envelope_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_value_v1.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/new_metric_value_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_value_v1.pyi` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/new_metric_value_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.pyi` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/new_metric_values_envelope_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/target_range_v1.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/target_range_v1.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/model/target_range_v1.pyi` & `dominodatalab-1.4.1/domino/_impl/custommetrics/model/target_range_v1.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/models/__init__.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.pyi` & `dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_alerts_v1/post.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1/post.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_values_v1/post.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1/post.pyi` & `dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_values_v1/post.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.pyi` & `dominodatalab-1.4.1/domino/_impl/custommetrics/paths/api_metric_values_v1_model_monitoring_id_metric/get.pyi`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/rest.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/rest.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/_impl/custommetrics/schemas.py` & `dominodatalab-1.4.1/domino/_impl/custommetrics/schemas.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/airflow/_operator.py` & `dominodatalab-1.4.1/domino/airflow/_operator.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/authentication.py` & `dominodatalab-1.4.1/domino/authentication.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/constants.py` & `dominodatalab-1.4.1/domino/constants.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/data_sources.py` & `dominodatalab-1.4.1/domino/data_sources.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/datasets.py` & `dominodatalab-1.4.1/domino/datasets.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/domino.py` & `dominodatalab-1.4.1/domino/domino.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/exceptions.py` & `dominodatalab-1.4.1/domino/exceptions.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/helpers.py` & `dominodatalab-1.4.1/domino/helpers.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/http_request_manager.py` & `dominodatalab-1.4.1/domino/http_request_manager.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/routes.py` & `dominodatalab-1.4.1/domino/routes.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/domino/training_sets.py` & `dominodatalab-1.4.1/domino/training_sets.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/dominodatalab.egg-info/PKG-INFO` & `dominodatalab-1.4.1/dominodatalab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: dominodatalab
-Version: 1.4.0
+Version: 1.4.1
 Summary: Python bindings for the Domino API
 Home-page: https://github.com/dominodatalab/python-domino
-Download-URL: https://github.com/dominodatalab/python-domino/archive/release-1.4.0.zip
+Download-URL: https://github.com/dominodatalab/python-domino/archive/release-1.4.1.zip
 Author: Domino Data Lab
 Author-email: support@dominodatalab.com
 License: Apache Software License (Apache 2.0)
 Keywords: Domino Data Lab,API
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: packaging
 Requires-Dist: requests>=2.4.2
 Requires-Dist: beautifulsoup4~=4.11
 Requires-Dist: polling2~=0.5.0
 Requires-Dist: urllib3~=1.26.12
-Requires-Dist: typing-extensions~=4.4.0
+Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: frozendict~=2.3.4
 Requires-Dist: python-dateutil~=2.8.2
 Requires-Dist: retry==0.9.2
 Provides-Extra: airflow
 Requires-Dist: apache-airflow==2.2.4; extra == "airflow"
 Provides-Extra: data
 Requires-Dist: dominodatalab-data>=0.1.0; extra == "data"
@@ -43,29 +43,29 @@
 See this documentation for details about the APIs:
 
 -   [Latest public Domino
     APIs](https://docs.dominodatalab.com/en/latest/api_guide/8c929e/domino-public-apis/)
 
 -   [Legacy APIs](https://dominodatalab.github.io/api-docs/)
 
-The latest released version of `python-domino` is `1.4.0`.
+The latest released version of `python-domino` is `1.4.1`.
 
 # Version compatibility matrix
 
 The `python-domino` library is compatible with different versions of
 Domino:
 
-| Domino Versions |                                    Python-Domino                                    |
-|-----------------|:-----------------------------------------------------------------------------------:|
-| 3.6.x or lower  |      [0.3.5](https://github.com/dominodatalab/python-domino/archive/0.3.5.zip)       |
-| 4.1.0 or higher | [1.0.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/1.0.0.zip) or Higher |
-| 5.3.0 or higher | [1.2.0]https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.0.zip) or Higher |
+| Domino Versions |                                             Python-Domino                                             |
+|-----------------|:-----------------------------------------------------------------------------------------------------:|
+| 3.6.x or lower  |               [0.3.5](https://github.com/dominodatalab/python-domino/archive/0.3.5.zip)               |
+| 4.1.0 or higher |     [1.0.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/1.0.0.zip) or Higher     |
+| 5.3.0 or higher | [1.2.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.0.zip) or Higher |
 | 5.5.0 or higher | [1.2.2](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.2.2.zip) or Higher |
 | 5.10.0 or higher | [1.3.1](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.3.1.zip) or Higher |
-| 5.11.0 or higher | [1.4.0](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.4.0.zip) or Higher |
+| 5.11.0 or higher | [1.4.1](https://github.com/dominodatalab/python-domino/archive/refs/tags/Release-1.4.1.zip) or Higher |
 
 # Development
 
 The current `python-domino` is based on Python 3.9, which is therefore recommended for development. `Pipenv` is also recommended to manage the dependencies.
 
 To use the Python binding in a Domino workbook session, include `dominodatalab` in your project's requirements.txt file.
 This makes the Python binding available for each new workbook session (or batch run) started within the project.
```

### Comparing `dominodatalab-1.4.0/dominodatalab.egg-info/SOURCES.txt` & `dominodatalab-1.4.1/dominodatalab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/requirements.txt` & `dominodatalab-1.4.1/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile setup.py
 #
 beautifulsoup4==4.12.3
     # via dominodatalab (setup.py)
 certifi==2024.2.2
@@ -28,13 +28,13 @@
     # via dominodatalab (setup.py)
 retry==0.9.2
     # via dominodatalab (setup.py)
 six==1.16.0
     # via python-dateutil
 soupsieve==2.5
     # via beautifulsoup4
-typing-extensions==4.4.0
+typing-extensions==4.11.0
     # via dominodatalab (setup.py)
 urllib3==1.26.18
     # via
     #   dominodatalab (setup.py)
     #   requests
```

### Comparing `dominodatalab-1.4.0/setup.py` & `dominodatalab-1.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     license="Apache Software License (Apache 2.0)",
     description="Python bindings for the Domino API",
     long_description=README,
     long_description_content_type="text/markdown",
     keywords=["Domino Data Lab", "API"],
     python_requires='>=3.9.0',
     install_requires=["packaging", "requests>=2.4.2", "beautifulsoup4~=4.11", "polling2~=0.5.0",
-                      "urllib3~=1.26.12", "typing-extensions~=4.4.0", "frozendict~=2.3.4", "python-dateutil~=2.8.2",
+                      "urllib3~=1.26.12", "typing-extensions>=4.5.0", "frozendict~=2.3.4", "python-dateutil~=2.8.2",
                       "retry==0.9.2"],
     extras_require={
         "airflow": ["apache-airflow==2.2.4"],
         "data": ["dominodatalab-data>=0.1.0"],
         "dev": [
             "black==22.3.0",
             "flake8==4.0.1",
```

### Comparing `dominodatalab-1.4.0/tests/test_basic_auth.py` & `dominodatalab-1.4.1/tests/test_basic_auth.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/tests/test_data_sources.py` & `dominodatalab-1.4.1/tests/test_data_sources.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/tests/test_datasets.py` & `dominodatalab-1.4.1/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/tests/test_domino.py` & `dominodatalab-1.4.1/tests/test_domino.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/tests/test_environments.py` & `dominodatalab-1.4.1/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/tests/test_finops.py` & `dominodatalab-1.4.1/tests/test_finops.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/tests/test_jobs.py` & `dominodatalab-1.4.1/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/tests/test_models.py` & `dominodatalab-1.4.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/tests/test_operator.py` & `dominodatalab-1.4.1/tests/test_operator.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/tests/test_projects.py` & `dominodatalab-1.4.1/tests/test_projects.py`

 * *Files identical despite different names*

### Comparing `dominodatalab-1.4.0/tests/test_spark_operator.py` & `dominodatalab-1.4.1/tests/test_spark_operator.py`

 * *Files identical despite different names*

