# Comparing `tmp/hsfs-3.7.5.tar.gz` & `tmp/hsfs-3.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsfs-3.7.5.tar", last modified: Tue Apr 30 12:22:24 2024, max compression
+gzip compressed data, was "hsfs-3.7.6.tar", last modified: Fri May  3 09:42:15 2024, max compression
```

## Comparing `hsfs-3.7.5.tar` & `hsfs-3.7.6.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0     1006     1006        0 2024-04-30 12:22:24.546402 hsfs-3.7.5/
--rw-r--r--   0     1006     1006       40 2024-01-11 15:40:27.000000 hsfs-3.7.5/MANIFEST.in
--rw-r--r--   0     1006     1006     8377 2024-04-30 12:22:24.546402 hsfs-3.7.5/PKG-INFO
--rw-r--r--   0     1006     1006     5950 2024-04-30 12:22:23.000000 hsfs-3.7.5/README.md
-drwxr-xr-x   0     1006     1006        0 2024-04-30 12:22:24.486403 hsfs-3.7.5/hsfs/
--rw-r--r--   0     1006     1006     1421 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/__init__.py
-drwxr-xr-x   0     1006     1006        0 2024-04-30 12:22:24.490403 hsfs-3.7.5/hsfs/client/
--rw-r--r--   0     1006     1006     1694 2024-01-11 15:40:27.000000 hsfs-3.7.5/hsfs/client/__init__.py
--rw-r--r--   0     1006     1006     1401 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/client/auth.py
--rw-r--r--   0     1006     1006     9570 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/client/base.py
--rw-r--r--   0     1006     1006     3028 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/client/exceptions.py
--rw-r--r--   0     1006     1006    13155 2024-04-15 10:29:25.000000 hsfs-3.7.5/hsfs/client/external.py
--rw-r--r--   0     1006     1006     6207 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/client/hopsworks.py
--rw-r--r--   0     1006     1006    15180 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/client/online_store_rest_client.py
--rw-r--r--   0     1006     1006     1554 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/code.py
--rw-r--r--   0     1006     1006    14393 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/connection.py
-drwxr-xr-x   0     1006     1006        0 2024-04-30 12:22:24.494403 hsfs-3.7.5/hsfs/constructor/
--rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.5/hsfs/constructor/__init__.py
--rw-r--r--   0     1006     1006     1497 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/constructor/external_feature_group_alias.py
--rw-r--r--   0     1006     1006     5612 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/constructor/filter.py
--rw-r--r--   0     1006     1006     3635 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/constructor/fs_query.py
--rw-r--r--   0     1006     1006     1749 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/constructor/hudi_feature_group_alias.py
--rw-r--r--   0     1006     1006     2161 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/constructor/join.py
--rw-r--r--   0     1006     1006     1587 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/constructor/prepared_statement_parameter.py
--rw-r--r--   0     1006     1006    29552 2024-04-26 05:47:12.000000 hsfs-3.7.5/hsfs/constructor/query.py
--rw-r--r--   0     1006     1006     3349 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/constructor/serving_prepared_statement.py
-drwxr-xr-x   0     1006     1006        0 2024-04-30 12:22:24.538402 hsfs-3.7.5/hsfs/core/
--rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.5/hsfs/core/__init__.py
--rw-r--r--   0     1006     1006    24518 2024-04-26 05:47:12.000000 hsfs-3.7.5/hsfs/core/arrow_flight_client.py
--rw-r--r--   0     1006     1006     4156 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/builtin_transformation_function.py
--rw-r--r--   0     1006     1006     1853 2024-01-11 15:40:27.000000 hsfs-3.7.5/hsfs/core/code_api.py
--rw-r--r--   0     1006     1006     2032 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/code_engine.py
--rw-r--r--   0     1006     1006     3629 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/dataset_api.py
--rw-r--r--   0     1006     1006     7809 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/delta_engine.py
--rw-r--r--   0     1006     1006     1040 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/deltastreamer_jobconf.py
--rw-r--r--   0     1006     1006     1627 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/execution.py
--rw-r--r--   0     1006     1006     5396 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/expectation_api.py
--rw-r--r--   0     1006     1006     2632 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/expectation_engine.py
--rw-r--r--   0     1006     1006     6356 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/expectation_suite_api.py
--rw-r--r--   0     1006     1006     4060 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/expectation_suite_engine.py
--rw-r--r--   0     1006     1006     9810 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/explicit_provenance.py
--rw-r--r--   0     1006     1006     6198 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/external_feature_group_engine.py
--rw-r--r--   0     1006     1006    11212 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/core/feature_descriptive_statistics.py
--rw-r--r--   0     1006     1006    16823 2024-04-30 12:22:19.000000 hsfs-3.7.5/hsfs/core/feature_group_api.py
--rw-r--r--   0     1006     1006     6976 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/core/feature_group_base_engine.py
--rw-r--r--   0     1006     1006    14833 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/feature_group_engine.py
--rw-r--r--   0     1006     1006    34754 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/core/feature_monitoring_config.py
--rw-r--r--   0     1006     1006    10497 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/feature_monitoring_config_api.py
--rw-r--r--   0     1006     1006    21382 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/feature_monitoring_config_engine.py
--rw-r--r--   0     1006     1006     7864 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/feature_monitoring_result.py
--rw-r--r--   0     1006     1006     5921 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/feature_monitoring_result_api.py
--rw-r--r--   0     1006     1006    24868 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/feature_monitoring_result_engine.py
--rw-r--r--   0     1006     1006     1238 2024-01-11 15:40:27.000000 hsfs-3.7.5/hsfs/core/feature_store_api.py
--rw-r--r--   0     1006     1006    10499 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/feature_view_api.py
--rw-r--r--   0     1006     1006    32375 2024-04-26 05:47:12.000000 hsfs-3.7.5/hsfs/core/feature_view_engine.py
--rw-r--r--   0     1006     1006     5023 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/great_expectation_engine.py
--rw-r--r--   0     1006     1006      828 2024-01-11 15:40:27.000000 hsfs-3.7.5/hsfs/core/hosts_api.py
--rw-r--r--   0     1006     1006    11709 2024-04-30 07:23:58.000000 hsfs-3.7.5/hsfs/core/hudi_engine.py
--rw-r--r--   0     1006     1006     1229 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/ingestion_job.py
--rw-r--r--   0     1006     1006     2262 2024-01-11 15:40:27.000000 hsfs-3.7.5/hsfs/core/ingestion_job_conf.py
--rw-r--r--   0     1006     1006     1087 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/inode.py
--rw-r--r--   0     1006     1006     8626 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/job.py
--rw-r--r--   0     1006     1006     2814 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/job_api.py
--rw-r--r--   0     1006     1006     2065 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/job_configuration.py
--rw-r--r--   0     1006     1006     3079 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/job_schedule.py
--rw-r--r--   0     1006     1006     1205 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/kafka_api.py
--rw-r--r--   0     1006     1006    11542 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/core/monitoring_window_config.py
--rw-r--r--   0     1006     1006    16985 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/core/monitoring_window_config_engine.py
--rw-r--r--   0     1006     1006     8709 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/online_store_rest_client_api.py
--rw-r--r--   0     1006     1006    32516 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/online_store_rest_client_engine.py
--rw-r--r--   0     1006     1006     3090 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/opensearch.py
--rw-r--r--   0     1006     1006     4419 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/opensearch_api.py
--rw-r--r--   0     1006     1006      898 2024-01-11 15:40:27.000000 hsfs-3.7.5/hsfs/core/project_api.py
--rw-r--r--   0     1006     1006     1093 2024-01-11 15:40:27.000000 hsfs-3.7.5/hsfs/core/query_constructor_api.py
--rw-r--r--   0     1006     1006      875 2024-01-11 15:40:27.000000 hsfs-3.7.5/hsfs/core/services_api.py
--rw-r--r--   0     1006     1006     1981 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/spine_group_engine.py
--rw-r--r--   0     1006     1006    12655 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/statistics_api.py
--rw-r--r--   0     1006     1006    20950 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/core/statistics_engine.py
--rw-r--r--   0     1006     1006     3072 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/storage_connector_api.py
--rw-r--r--   0     1006     1006     4696 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/tags_api.py
--rw-r--r--   0     1006     1006     6685 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/training_dataset_api.py
--rw-r--r--   0     1006     1006     6210 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/training_dataset_engine.py
--rw-r--r--   0     1006     1006     2148 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/training_dataset_job_conf.py
--rw-r--r--   0     1006     1006     4161 2024-01-11 15:40:27.000000 hsfs-3.7.5/hsfs/core/transformation_function_api.py
--rw-r--r--   0     1006     1006    12712 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/transformation_function_engine.py
--rw-r--r--   0     1006     1006     4773 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/validation_report_api.py
--rw-r--r--   0     1006     1006     3640 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/validation_report_engine.py
--rw-r--r--   0     1006     1006     2158 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/validation_result_api.py
--rw-r--r--   0     1006     1006     5492 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/core/validation_result_engine.py
--rw-r--r--   0     1006     1006     2259 2024-04-26 05:47:12.000000 hsfs-3.7.5/hsfs/core/variable_api.py
--rw-r--r--   0     1006     1006    11843 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/vector_db_client.py
--rwxr-xr-x   0     1006     1006    41829 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/core/vector_server.py
--rw-r--r--   0     1006     1006     1655 2024-01-11 15:40:27.000000 hsfs-3.7.5/hsfs/decorators.py
--rw-r--r--   0     1006     1006     5552 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/embedding.py
-drwxr-xr-x   0     1006     1006        0 2024-04-30 12:22:24.542402 hsfs-3.7.5/hsfs/engine/
--rw-r--r--   0     1006     1006     2486 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/engine/__init__.py
--rw-r--r--   0     1006     1006    54331 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/engine/python.py
--rw-r--r--   0     1006     1006    47924 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/engine/spark.py
--rw-r--r--   0     1006     1006     1118 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/engine/spark_no_metastore.py
--rw-r--r--   0     1006     1006    23612 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/expectation_suite.py
--rw-r--r--   0     1006     1006     7022 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/feature.py
--rw-r--r--   0     1006     1006   157739 2024-04-30 12:22:19.000000 hsfs-3.7.5/hsfs/feature_group.py
--rw-r--r--   0     1006     1006     3955 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/feature_group_commit.py
--rw-r--r--   0     1006     1006     1992 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/feature_group_writer.py
--rw-r--r--   0     1006     1006    79282 2024-04-30 07:23:58.000000 hsfs-3.7.5/hsfs/feature_store.py
--rw-r--r--   0     1006     1006   164157 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/feature_view.py
--rw-r--r--   0     1006     1006     4822 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/ge_expectation.py
--rw-r--r--   0     1006     1006     8651 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/ge_validation_result.py
--rw-r--r--   0     1006     1006     3456 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/serving_key.py
--rw-r--r--   0     1006     1006     2081 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/split_statistics.py
--rw-r--r--   0     1006     1006     8409 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/statistics.py
--rw-r--r--   0     1006     1006     3366 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/statistics_config.py
--rw-r--r--   0     1006     1006    49774 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/storage_connector.py
--rw-r--r--   0     1006     1006     1868 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/tag.py
--rw-r--r--   0     1006     1006    39842 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/training_dataset.py
--rw-r--r--   0     1006     1006     4960 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/training_dataset_feature.py
--rw-r--r--   0     1006     1006     2816 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/training_dataset_split.py
--rw-r--r--   0     1006     1006     8982 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/transformation_function.py
--rw-r--r--   0     1006     1006     2197 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/transformation_function_attached.py
--rw-r--r--   0     1006     1006     7901 2024-04-30 12:22:19.000000 hsfs-3.7.5/hsfs/usage.py
--rw-r--r--   0     1006     1006     3323 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/user.py
--rw-r--r--   0     1006     1006    16242 2024-04-30 07:22:38.000000 hsfs-3.7.5/hsfs/util.py
--rw-r--r--   0     1006     1006     7537 2024-04-11 18:09:58.000000 hsfs-3.7.5/hsfs/validation_report.py
--rw-r--r--   0     1006     1006      628 2024-04-30 12:22:19.000000 hsfs-3.7.5/hsfs/version.py
-drwxr-xr-x   0     1006     1006        0 2024-04-30 12:22:24.486403 hsfs-3.7.5/hsfs.egg-info/
--rw-r--r--   0     1006     1006     8377 2024-04-30 12:22:24.000000 hsfs-3.7.5/hsfs.egg-info/PKG-INFO
--rw-r--r--   0     1006     1006     3650 2024-04-30 12:22:24.000000 hsfs-3.7.5/hsfs.egg-info/SOURCES.txt
--rw-r--r--   0     1006     1006        1 2024-04-30 12:22:24.000000 hsfs-3.7.5/hsfs.egg-info/dependency_links.txt
--rw-r--r--   0     1006     1006      892 2024-04-30 12:22:24.000000 hsfs-3.7.5/hsfs.egg-info/requires.txt
--rw-r--r--   0     1006     1006        5 2024-04-30 12:22:24.000000 hsfs-3.7.5/hsfs.egg-info/top_level.txt
--rw-r--r--   0     1006     1006       38 2024-04-30 12:22:24.546402 hsfs-3.7.5/setup.cfg
--rw-r--r--   0     1006     1006     3310 2024-04-11 18:09:58.000000 hsfs-3.7.5/setup.py
-drwxr-xr-x   0     1006     1006        0 2024-04-30 12:22:24.542402 hsfs-3.7.5/tests/
--rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.5/tests/__init__.py
--rw-r--r--   0     1006     1006    34202 2024-04-11 18:09:58.000000 hsfs-3.7.5/tests/test_storage_connector.py
+drwxr-xr-x   0     1006     1006        0 2024-05-03 09:42:15.769622 hsfs-3.7.6/
+-rw-r--r--   0     1006     1006       40 2024-01-11 15:40:27.000000 hsfs-3.7.6/MANIFEST.in
+-rw-r--r--   0     1006     1006     8377 2024-05-03 09:42:15.769622 hsfs-3.7.6/PKG-INFO
+-rw-r--r--   0     1006     1006     5950 2024-05-03 09:42:14.000000 hsfs-3.7.6/README.md
+drwxr-xr-x   0     1006     1006        0 2024-05-03 09:42:15.721623 hsfs-3.7.6/hsfs/
+-rw-r--r--   0     1006     1006     1421 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/__init__.py
+drwxr-xr-x   0     1006     1006        0 2024-05-03 09:42:15.725623 hsfs-3.7.6/hsfs/client/
+-rw-r--r--   0     1006     1006     1694 2024-01-11 15:40:27.000000 hsfs-3.7.6/hsfs/client/__init__.py
+-rw-r--r--   0     1006     1006     1401 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/client/auth.py
+-rw-r--r--   0     1006     1006    10372 2024-05-03 09:42:10.000000 hsfs-3.7.6/hsfs/client/base.py
+-rw-r--r--   0     1006     1006     3028 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/client/exceptions.py
+-rw-r--r--   0     1006     1006    13155 2024-04-15 10:29:25.000000 hsfs-3.7.6/hsfs/client/external.py
+-rw-r--r--   0     1006     1006     6207 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/client/hopsworks.py
+-rw-r--r--   0     1006     1006    15180 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/client/online_store_rest_client.py
+-rw-r--r--   0     1006     1006     1554 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/code.py
+-rw-r--r--   0     1006     1006    14393 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/connection.py
+drwxr-xr-x   0     1006     1006        0 2024-05-03 09:42:15.729622 hsfs-3.7.6/hsfs/constructor/
+-rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.6/hsfs/constructor/__init__.py
+-rw-r--r--   0     1006     1006     1497 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/constructor/external_feature_group_alias.py
+-rw-r--r--   0     1006     1006     5612 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/constructor/filter.py
+-rw-r--r--   0     1006     1006     3635 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/constructor/fs_query.py
+-rw-r--r--   0     1006     1006     1749 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/constructor/hudi_feature_group_alias.py
+-rw-r--r--   0     1006     1006     2161 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/constructor/join.py
+-rw-r--r--   0     1006     1006     1587 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/constructor/prepared_statement_parameter.py
+-rw-r--r--   0     1006     1006    29552 2024-04-26 05:47:12.000000 hsfs-3.7.6/hsfs/constructor/query.py
+-rw-r--r--   0     1006     1006     3349 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/constructor/serving_prepared_statement.py
+drwxr-xr-x   0     1006     1006        0 2024-05-03 09:42:15.761622 hsfs-3.7.6/hsfs/core/
+-rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.6/hsfs/core/__init__.py
+-rw-r--r--   0     1006     1006    24518 2024-04-26 05:47:12.000000 hsfs-3.7.6/hsfs/core/arrow_flight_client.py
+-rw-r--r--   0     1006     1006     4156 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/builtin_transformation_function.py
+-rw-r--r--   0     1006     1006     1853 2024-01-11 15:40:27.000000 hsfs-3.7.6/hsfs/core/code_api.py
+-rw-r--r--   0     1006     1006     2032 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/code_engine.py
+-rw-r--r--   0     1006     1006     3629 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/dataset_api.py
+-rw-r--r--   0     1006     1006     7809 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/delta_engine.py
+-rw-r--r--   0     1006     1006     1040 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/deltastreamer_jobconf.py
+-rw-r--r--   0     1006     1006     1627 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/execution.py
+-rw-r--r--   0     1006     1006     5396 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/expectation_api.py
+-rw-r--r--   0     1006     1006     2632 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/expectation_engine.py
+-rw-r--r--   0     1006     1006     6356 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/expectation_suite_api.py
+-rw-r--r--   0     1006     1006     4060 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/expectation_suite_engine.py
+-rw-r--r--   0     1006     1006     9810 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/explicit_provenance.py
+-rw-r--r--   0     1006     1006     6198 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/external_feature_group_engine.py
+-rw-r--r--   0     1006     1006    11212 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/core/feature_descriptive_statistics.py
+-rw-r--r--   0     1006     1006    16800 2024-05-03 09:42:10.000000 hsfs-3.7.6/hsfs/core/feature_group_api.py
+-rw-r--r--   0     1006     1006     6976 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/core/feature_group_base_engine.py
+-rw-r--r--   0     1006     1006    14833 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/feature_group_engine.py
+-rw-r--r--   0     1006     1006    34754 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/core/feature_monitoring_config.py
+-rw-r--r--   0     1006     1006    10497 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/feature_monitoring_config_api.py
+-rw-r--r--   0     1006     1006    21382 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/feature_monitoring_config_engine.py
+-rw-r--r--   0     1006     1006     7864 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/feature_monitoring_result.py
+-rw-r--r--   0     1006     1006     5921 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/feature_monitoring_result_api.py
+-rw-r--r--   0     1006     1006    24868 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/feature_monitoring_result_engine.py
+-rw-r--r--   0     1006     1006     1238 2024-01-11 15:40:27.000000 hsfs-3.7.6/hsfs/core/feature_store_api.py
+-rw-r--r--   0     1006     1006    10499 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/feature_view_api.py
+-rw-r--r--   0     1006     1006    32375 2024-04-26 05:47:12.000000 hsfs-3.7.6/hsfs/core/feature_view_engine.py
+-rw-r--r--   0     1006     1006     5023 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/great_expectation_engine.py
+-rw-r--r--   0     1006     1006      828 2024-01-11 15:40:27.000000 hsfs-3.7.6/hsfs/core/hosts_api.py
+-rw-r--r--   0     1006     1006    11709 2024-04-30 07:23:58.000000 hsfs-3.7.6/hsfs/core/hudi_engine.py
+-rw-r--r--   0     1006     1006     1229 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/ingestion_job.py
+-rw-r--r--   0     1006     1006     2262 2024-01-11 15:40:27.000000 hsfs-3.7.6/hsfs/core/ingestion_job_conf.py
+-rw-r--r--   0     1006     1006     1087 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/inode.py
+-rw-r--r--   0     1006     1006     8626 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/job.py
+-rw-r--r--   0     1006     1006     2814 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/job_api.py
+-rw-r--r--   0     1006     1006     2065 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/job_configuration.py
+-rw-r--r--   0     1006     1006     3079 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/job_schedule.py
+-rw-r--r--   0     1006     1006     1205 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/kafka_api.py
+-rw-r--r--   0     1006     1006    11542 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/core/monitoring_window_config.py
+-rw-r--r--   0     1006     1006    16985 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/core/monitoring_window_config_engine.py
+-rw-r--r--   0     1006     1006     8709 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/online_store_rest_client_api.py
+-rw-r--r--   0     1006     1006    32516 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/online_store_rest_client_engine.py
+-rw-r--r--   0     1006     1006     3090 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/opensearch.py
+-rw-r--r--   0     1006     1006     4419 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/opensearch_api.py
+-rw-r--r--   0     1006     1006      898 2024-01-11 15:40:27.000000 hsfs-3.7.6/hsfs/core/project_api.py
+-rw-r--r--   0     1006     1006     1093 2024-01-11 15:40:27.000000 hsfs-3.7.6/hsfs/core/query_constructor_api.py
+-rw-r--r--   0     1006     1006      875 2024-01-11 15:40:27.000000 hsfs-3.7.6/hsfs/core/services_api.py
+-rw-r--r--   0     1006     1006     1981 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/spine_group_engine.py
+-rw-r--r--   0     1006     1006    12655 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/statistics_api.py
+-rw-r--r--   0     1006     1006    20950 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/core/statistics_engine.py
+-rw-r--r--   0     1006     1006     3072 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/storage_connector_api.py
+-rw-r--r--   0     1006     1006     4696 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/tags_api.py
+-rw-r--r--   0     1006     1006     6685 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/training_dataset_api.py
+-rw-r--r--   0     1006     1006     6210 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/training_dataset_engine.py
+-rw-r--r--   0     1006     1006     2148 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/training_dataset_job_conf.py
+-rw-r--r--   0     1006     1006     4161 2024-01-11 15:40:27.000000 hsfs-3.7.6/hsfs/core/transformation_function_api.py
+-rw-r--r--   0     1006     1006    12712 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/transformation_function_engine.py
+-rw-r--r--   0     1006     1006     4773 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/validation_report_api.py
+-rw-r--r--   0     1006     1006     3640 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/validation_report_engine.py
+-rw-r--r--   0     1006     1006     2158 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/validation_result_api.py
+-rw-r--r--   0     1006     1006     5492 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/core/validation_result_engine.py
+-rw-r--r--   0     1006     1006     2259 2024-04-26 05:47:12.000000 hsfs-3.7.6/hsfs/core/variable_api.py
+-rw-r--r--   0     1006     1006    11843 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/vector_db_client.py
+-rwxr-xr-x   0     1006     1006    41829 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/core/vector_server.py
+-rw-r--r--   0     1006     1006     1655 2024-01-11 15:40:27.000000 hsfs-3.7.6/hsfs/decorators.py
+-rw-r--r--   0     1006     1006     5552 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/embedding.py
+drwxr-xr-x   0     1006     1006        0 2024-05-03 09:42:15.765622 hsfs-3.7.6/hsfs/engine/
+-rw-r--r--   0     1006     1006     2486 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/engine/__init__.py
+-rw-r--r--   0     1006     1006    54331 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/engine/python.py
+-rw-r--r--   0     1006     1006    52109 2024-05-02 06:57:50.000000 hsfs-3.7.6/hsfs/engine/spark.py
+-rw-r--r--   0     1006     1006     1118 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/engine/spark_no_metastore.py
+-rw-r--r--   0     1006     1006    23612 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/expectation_suite.py
+-rw-r--r--   0     1006     1006     7022 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/feature.py
+-rw-r--r--   0     1006     1006   157739 2024-04-30 12:22:19.000000 hsfs-3.7.6/hsfs/feature_group.py
+-rw-r--r--   0     1006     1006     3955 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/feature_group_commit.py
+-rw-r--r--   0     1006     1006     1992 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/feature_group_writer.py
+-rw-r--r--   0     1006     1006    79282 2024-04-30 07:23:58.000000 hsfs-3.7.6/hsfs/feature_store.py
+-rw-r--r--   0     1006     1006   164157 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/feature_view.py
+-rw-r--r--   0     1006     1006     4822 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/ge_expectation.py
+-rw-r--r--   0     1006     1006     8651 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/ge_validation_result.py
+-rw-r--r--   0     1006     1006     3456 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/serving_key.py
+-rw-r--r--   0     1006     1006     2081 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/split_statistics.py
+-rw-r--r--   0     1006     1006     8409 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/statistics.py
+-rw-r--r--   0     1006     1006     3366 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/statistics_config.py
+-rw-r--r--   0     1006     1006    49774 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/storage_connector.py
+-rw-r--r--   0     1006     1006     1868 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/tag.py
+-rw-r--r--   0     1006     1006    39842 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/training_dataset.py
+-rw-r--r--   0     1006     1006     4960 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/training_dataset_feature.py
+-rw-r--r--   0     1006     1006     2816 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/training_dataset_split.py
+-rw-r--r--   0     1006     1006     8982 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/transformation_function.py
+-rw-r--r--   0     1006     1006     2197 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/transformation_function_attached.py
+-rw-r--r--   0     1006     1006     7901 2024-04-30 12:22:19.000000 hsfs-3.7.6/hsfs/usage.py
+-rw-r--r--   0     1006     1006     3323 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/user.py
+-rw-r--r--   0     1006     1006    16242 2024-04-30 07:22:38.000000 hsfs-3.7.6/hsfs/util.py
+-rw-r--r--   0     1006     1006     7537 2024-04-11 18:09:58.000000 hsfs-3.7.6/hsfs/validation_report.py
+-rw-r--r--   0     1006     1006      628 2024-05-03 09:42:10.000000 hsfs-3.7.6/hsfs/version.py
+drwxr-xr-x   0     1006     1006        0 2024-05-03 09:42:15.721623 hsfs-3.7.6/hsfs.egg-info/
+-rw-r--r--   0     1006     1006     8377 2024-05-03 09:42:15.000000 hsfs-3.7.6/hsfs.egg-info/PKG-INFO
+-rw-r--r--   0     1006     1006     3650 2024-05-03 09:42:15.000000 hsfs-3.7.6/hsfs.egg-info/SOURCES.txt
+-rw-r--r--   0     1006     1006        1 2024-05-03 09:42:15.000000 hsfs-3.7.6/hsfs.egg-info/dependency_links.txt
+-rw-r--r--   0     1006     1006      892 2024-05-03 09:42:15.000000 hsfs-3.7.6/hsfs.egg-info/requires.txt
+-rw-r--r--   0     1006     1006        5 2024-05-03 09:42:15.000000 hsfs-3.7.6/hsfs.egg-info/top_level.txt
+-rw-r--r--   0     1006     1006       38 2024-05-03 09:42:15.769622 hsfs-3.7.6/setup.cfg
+-rw-r--r--   0     1006     1006     3310 2024-05-02 06:57:50.000000 hsfs-3.7.6/setup.py
+drwxr-xr-x   0     1006     1006        0 2024-05-03 09:42:15.765622 hsfs-3.7.6/tests/
+-rw-r--r--   0     1006     1006      605 2024-01-11 15:40:27.000000 hsfs-3.7.6/tests/__init__.py
+-rw-r--r--   0     1006     1006    34202 2024-04-11 18:09:58.000000 hsfs-3.7.6/tests/test_storage_connector.py
```

### Comparing `hsfs-3.7.5/PKG-INFO` & `hsfs-3.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.7.5
+Version: 3.7.6
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.5
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.6
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.7.5 Summary: HSFS: An environment
+Metadata-Version: 2.1 Name: hsfs Version: 3.7.6 Summary: HSFS: An environment
 independent client to interact with the Hopsworks Featurestore Home-page:
 https://github.com/logicalclocks/feature-store-api Author: Hopsworks AB Author-
 email: moritz@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.5
+https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.6
 Description: # Hopsworks Feature Store
 _[_H_o_p_s_w_o_r_k_s_ _C_o_m_m_u_n_i_t_y_]_[_H_o_p_s_w_o_r_k_s_ _F_e_a_t_u_r_e_ _S_t_o_r_e_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_P_y_P_i_S_t_a_t_u_s_]_[_S_c_a_l_a_/
                 _J_a_v_a_ _A_r_t_i_f_a_c_t_s_]_[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_S_t_y_l_e_][License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
```

### Comparing `hsfs-3.7.5/README.md` & `hsfs-3.7.6/README.md`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/__init__.py` & `hsfs-3.7.6/hsfs/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/client/__init__.py` & `hsfs-3.7.6/hsfs/client/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/client/auth.py` & `hsfs-3.7.6/hsfs/client/auth.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/client/base.py` & `hsfs-3.7.6/hsfs/client/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,21 +13,22 @@
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
 import base64
 import os
 import textwrap
+import time
 import furl
-from pathlib import Path
-from abc import ABC, abstractmethod
-
 import requests
 import urllib3
 
+from abc import ABC
+from pathlib import Path
+
 from hsfs.client import exceptions, auth
 from hsfs.decorators import connected
 
 try:
     import jks
 except ImportError:
     pass
@@ -35,24 +36,22 @@
 
 urllib3.disable_warnings(urllib3.exceptions.SecurityWarning)
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 class Client(ABC):
     TOKEN_FILE = "token.jwt"
+    TOKEN_EXPIRED_RETRY_INTERVAL = 0.6
+    TOKEN_EXPIRED_MAX_RETRIES = 10
+
     APIKEY_FILE = "api.key"
     REST_ENDPOINT = "REST_ENDPOINT"
     DEFAULT_DATABRICKS_ROOT_VIRTUALENV_ENV = "DEFAULT_DATABRICKS_ROOT_VIRTUALENV_ENV"
     HOPSWORKS_PUBLIC_HOST = "HOPSWORKS_PUBLIC_HOST"
 
-    @abstractmethod
-    def __init__(self):
-        """To be implemented by clients."""
-        pass
-
     def _get_verify(self, verify, trust_store_path):
         """Get verification method for sending HTTP requests to Hopsworks.
 
         Credit to https://gist.github.com/gdamjan/55a8b9eec6cf7b771f92021d93b87b2c
 
         :param verify: perform hostname verification, 'true' or 'false'
         :type verify: str
@@ -165,31 +164,50 @@
         )
 
         prepped = self._session.prepare_request(request)
         response = self._session.send(prepped, verify=self._verify, stream=stream)
 
         if response.status_code == 401 and self.REST_ENDPOINT in os.environ:
             # refresh token and retry request - only on hopsworks
-            self._auth = auth.BearerAuth(self._read_jwt())
-            # Update request with the new token
-            request.auth = self._auth
-            prepped = self._session.prepare_request(request)
-            response = self._session.send(prepped, verify=self._verify, stream=stream)
+            response = self._retry_token_expired(
+                request, stream, self.TOKEN_EXPIRED_RETRY_INTERVAL, 1
+            )
 
         if response.status_code // 100 != 2:
             raise exceptions.RestAPIError(url, response)
 
         if stream:
             return response
         else:
             # handle different success response codes
             if len(response.content) == 0:
                 return None
             return response.json()
 
+    def _retry_token_expired(self, request, stream, wait, retries):
+        """Refresh the JWT token and retry the request. Only on Hopsworks.
+        As the token might take a while to get refreshed. Keep trying
+        """
+        # Sleep the waited time before re-issuing the request
+        time.sleep(wait)
+
+        self._auth = auth.BearerAuth(self._read_jwt())
+        # Update request with the new token
+        request.auth = self._auth
+        prepped = self._session.prepare_request(request)
+        response = self._session.send(prepped, verify=self._verify, stream=stream)
+
+        if response.status_code == 401 and retries < self.TOKEN_EXPIRED_MAX_RETRIES:
+            # Try again.
+            return self._retry_token_expired(request, stream, wait * 2, retries + 1)
+        else:
+            # If the number of retries have expired, the _send_request method
+            # will throw an exception to the user as part of the status_code validation.
+            return response
+
     def _close(self):
         """Closes a client. Can be implemented for clean up purposes, not mandatory."""
         self._connected = False
 
     def _write_pem(
         self, keystore_path, keystore_pw, truststore_path, truststore_pw, prefix
     ):
```

### Comparing `hsfs-3.7.5/hsfs/client/exceptions.py` & `hsfs-3.7.6/hsfs/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/client/external.py` & `hsfs-3.7.6/hsfs/client/external.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/client/hopsworks.py` & `hsfs-3.7.6/hsfs/client/hopsworks.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/client/online_store_rest_client.py` & `hsfs-3.7.6/hsfs/client/online_store_rest_client.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/code.py` & `hsfs-3.7.6/hsfs/code.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/connection.py` & `hsfs-3.7.6/hsfs/connection.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/constructor/__init__.py` & `hsfs-3.7.6/hsfs/constructor/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/constructor/external_feature_group_alias.py` & `hsfs-3.7.6/hsfs/constructor/external_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/constructor/filter.py` & `hsfs-3.7.6/hsfs/constructor/filter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/constructor/fs_query.py` & `hsfs-3.7.6/hsfs/constructor/fs_query.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/constructor/hudi_feature_group_alias.py` & `hsfs-3.7.6/hsfs/constructor/hudi_feature_group_alias.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/constructor/join.py` & `hsfs-3.7.6/hsfs/constructor/join.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/constructor/prepared_statement_parameter.py` & `hsfs-3.7.6/hsfs/constructor/prepared_statement_parameter.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/constructor/query.py` & `hsfs-3.7.6/hsfs/constructor/query.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/constructor/serving_prepared_statement.py` & `hsfs-3.7.6/hsfs/constructor/serving_prepared_statement.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/__init__.py` & `hsfs-3.7.6/hsfs/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/arrow_flight_client.py` & `hsfs-3.7.6/hsfs/core/arrow_flight_client.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/builtin_transformation_function.py` & `hsfs-3.7.6/hsfs/core/builtin_transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/code_api.py` & `hsfs-3.7.6/hsfs/core/code_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/code_engine.py` & `hsfs-3.7.6/hsfs/core/code_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/dataset_api.py` & `hsfs-3.7.6/hsfs/core/dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/delta_engine.py` & `hsfs-3.7.6/hsfs/core/delta_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/deltastreamer_jobconf.py` & `hsfs-3.7.6/hsfs/core/deltastreamer_jobconf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/execution.py` & `hsfs-3.7.6/hsfs/core/execution.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/expectation_api.py` & `hsfs-3.7.6/hsfs/core/expectation_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/expectation_engine.py` & `hsfs-3.7.6/hsfs/core/expectation_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/expectation_suite_api.py` & `hsfs-3.7.6/hsfs/core/expectation_suite_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/expectation_suite_engine.py` & `hsfs-3.7.6/hsfs/core/expectation_suite_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/explicit_provenance.py` & `hsfs-3.7.6/hsfs/core/explicit_provenance.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/external_feature_group_engine.py` & `hsfs-3.7.6/hsfs/core/external_feature_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/feature_descriptive_statistics.py` & `hsfs-3.7.6/hsfs/core/feature_descriptive_statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/feature_group_api.py` & `hsfs-3.7.6/hsfs/core/feature_group_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,14 @@
                     FeatureGroupApi.BACKEND_FG_SPINE,
                 ]
                 raise ValueError(
                     f"Unknown feature group type: {fg_json['type']}, expected one of: "
                     + str(list_of_types)
                 )
 
-        print(fg_objs)
         if version is not None:
             return fg_objs[0]
         else:
             return fg_objs
 
     def delete_content(
         self,
```

### Comparing `hsfs-3.7.5/hsfs/core/feature_group_base_engine.py` & `hsfs-3.7.6/hsfs/core/feature_group_base_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/feature_group_engine.py` & `hsfs-3.7.6/hsfs/core/feature_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/feature_monitoring_config.py` & `hsfs-3.7.6/hsfs/core/feature_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/feature_monitoring_config_api.py` & `hsfs-3.7.6/hsfs/core/feature_monitoring_config_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/feature_monitoring_config_engine.py` & `hsfs-3.7.6/hsfs/core/feature_monitoring_config_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/feature_monitoring_result.py` & `hsfs-3.7.6/hsfs/core/feature_monitoring_result.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/feature_monitoring_result_api.py` & `hsfs-3.7.6/hsfs/core/feature_monitoring_result_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/feature_monitoring_result_engine.py` & `hsfs-3.7.6/hsfs/core/feature_monitoring_result_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/feature_store_api.py` & `hsfs-3.7.6/hsfs/core/feature_store_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/feature_view_api.py` & `hsfs-3.7.6/hsfs/core/feature_view_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/feature_view_engine.py` & `hsfs-3.7.6/hsfs/core/feature_view_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/great_expectation_engine.py` & `hsfs-3.7.6/hsfs/core/great_expectation_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/hosts_api.py` & `hsfs-3.7.6/hsfs/core/hosts_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/hudi_engine.py` & `hsfs-3.7.6/hsfs/core/hudi_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/ingestion_job.py` & `hsfs-3.7.6/hsfs/core/ingestion_job.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/ingestion_job_conf.py` & `hsfs-3.7.6/hsfs/core/ingestion_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/inode.py` & `hsfs-3.7.6/hsfs/core/inode.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/job.py` & `hsfs-3.7.6/hsfs/core/job.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/job_api.py` & `hsfs-3.7.6/hsfs/core/job_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/job_configuration.py` & `hsfs-3.7.6/hsfs/core/job_configuration.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/job_schedule.py` & `hsfs-3.7.6/hsfs/core/job_schedule.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/kafka_api.py` & `hsfs-3.7.6/hsfs/core/kafka_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/monitoring_window_config.py` & `hsfs-3.7.6/hsfs/core/monitoring_window_config.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/monitoring_window_config_engine.py` & `hsfs-3.7.6/hsfs/core/monitoring_window_config_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/online_store_rest_client_api.py` & `hsfs-3.7.6/hsfs/core/online_store_rest_client_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/online_store_rest_client_engine.py` & `hsfs-3.7.6/hsfs/core/online_store_rest_client_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/opensearch.py` & `hsfs-3.7.6/hsfs/core/opensearch.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/opensearch_api.py` & `hsfs-3.7.6/hsfs/core/opensearch_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/project_api.py` & `hsfs-3.7.6/hsfs/core/project_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/query_constructor_api.py` & `hsfs-3.7.6/hsfs/core/query_constructor_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/services_api.py` & `hsfs-3.7.6/hsfs/core/services_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/spine_group_engine.py` & `hsfs-3.7.6/hsfs/core/spine_group_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/statistics_api.py` & `hsfs-3.7.6/hsfs/core/statistics_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/statistics_engine.py` & `hsfs-3.7.6/hsfs/core/statistics_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/storage_connector_api.py` & `hsfs-3.7.6/hsfs/core/storage_connector_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/tags_api.py` & `hsfs-3.7.6/hsfs/core/tags_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/training_dataset_api.py` & `hsfs-3.7.6/hsfs/core/training_dataset_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/training_dataset_engine.py` & `hsfs-3.7.6/hsfs/core/training_dataset_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/training_dataset_job_conf.py` & `hsfs-3.7.6/hsfs/core/training_dataset_job_conf.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/transformation_function_api.py` & `hsfs-3.7.6/hsfs/core/transformation_function_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/transformation_function_engine.py` & `hsfs-3.7.6/hsfs/core/transformation_function_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/validation_report_api.py` & `hsfs-3.7.6/hsfs/core/validation_report_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/validation_report_engine.py` & `hsfs-3.7.6/hsfs/core/validation_report_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/validation_result_api.py` & `hsfs-3.7.6/hsfs/core/validation_result_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/validation_result_engine.py` & `hsfs-3.7.6/hsfs/core/validation_result_engine.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/variable_api.py` & `hsfs-3.7.6/hsfs/core/variable_api.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/vector_db_client.py` & `hsfs-3.7.6/hsfs/core/vector_db_client.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/core/vector_server.py` & `hsfs-3.7.6/hsfs/core/vector_server.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/decorators.py` & `hsfs-3.7.6/hsfs/decorators.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/embedding.py` & `hsfs-3.7.6/hsfs/embedding.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/engine/__init__.py` & `hsfs-3.7.6/hsfs/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/engine/python.py` & `hsfs-3.7.6/hsfs/engine/python.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/engine/spark.py` & `hsfs-3.7.6/hsfs/engine/spark.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import re
 import warnings
 from typing import Optional, TypeVar
 
 import numpy as np
 import pandas as pd
 import avro
-from datetime import datetime, timezone
+from datetime import datetime, date, timezone
 
 import tzlocal
 
 # in case importing in %%local
 
 try:
     import pyspark
@@ -631,17 +631,105 @@
         split_weights = [split[1] for split in splits]
         split_dataset = dataset.randomSplit(split_weights, training_dataset.seed)
         return dict([(split[0], split_dataset[i]) for i, split in enumerate(splits)])
 
     def _time_series_split(
         self, training_dataset, dataset, event_time, drop_event_time=False
     ):
+        # duplicate the code from util module to avoid udf errors on windows
+        def check_timestamp_format_from_date_string(input_date):
+            date_format_patterns = {
+                r"^([0-9]{4})([0-9]{2})([0-9]{2})$": "%Y%m%d",
+                r"^([0-9]{4})([0-9]{2})([0-9]{2})([0-9]{2})$": "%Y%m%d%H",
+                r"^([0-9]{4})([0-9]{2})([0-9]{2})([0-9]{2})([0-9]{2})$": "%Y%m%d%H%M",
+                r"^([0-9]{4})([0-9]{2})([0-9]{2})([0-9]{2})([0-9]{2})([0-9]{2})$": "%Y%m%d%H%M%S",
+                r"^([0-9]{4})([0-9]{2})([0-9]{2})([0-9]{2})([0-9]{2})([0-9]{2})([0-9]{3})$": "%Y%m%d%H%M%S%f",
+                r"^([0-9]{4})([0-9]{2})([0-9]{2})T([0-9]{2})([0-9]{2})([0-9]{2})([0-9]{6})Z$": "ISO",
+            }
+            normalized_date = (
+                input_date.replace("/", "")
+                .replace("-", "")
+                .replace(" ", "")
+                .replace(":", "")
+                .replace(".", "")
+            )
+
+            date_format = None
+            for pattern in date_format_patterns:
+                date_format_pattern = re.match(pattern, normalized_date)
+                if date_format_pattern:
+                    date_format = date_format_patterns[pattern]
+                    break
+
+            if date_format is None:
+                raise ValueError(
+                    "Unable to identify format of the provided date value : "
+                    + input_date
+                )
+
+            return normalized_date, date_format
+
+        def get_timestamp_from_date_string(input_date):
+            norm_input_date, date_format = check_timestamp_format_from_date_string(
+                input_date
+            )
+            try:
+                if date_format != "ISO":
+                    date_time = datetime.strptime(norm_input_date, date_format)
+                else:
+                    date_time = datetime.fromisoformat(input_date[:-1])
+            except ValueError as err:
+                raise ValueError(
+                    "Unable to parse the normalized input date value : "
+                    + norm_input_date
+                    + " with format "
+                    + date_format
+                ) from err
+            if date_time.tzinfo is None:
+                date_time = date_time.replace(tzinfo=timezone.utc)
+            return int(float(date_time.timestamp()) * 1000)
+
+        def convert_event_time_to_timestamp(event_time):
+            if not event_time:
+                return None
+            if isinstance(event_time, str):
+                return get_timestamp_from_date_string(event_time)
+            elif isinstance(event_time, pd._libs.tslibs.timestamps.Timestamp):
+                # convert to unix epoch time in milliseconds.
+                event_time = event_time.to_pydatetime()
+                # convert to unix epoch time in milliseconds.
+                if event_time.tzinfo is None:
+                    event_time = event_time.replace(tzinfo=timezone.utc)
+                return int(event_time.timestamp() * 1000)
+            elif isinstance(event_time, datetime):
+                # convert to unix epoch time in milliseconds.
+                if event_time.tzinfo is None:
+                    event_time = event_time.replace(tzinfo=timezone.utc)
+                return int(event_time.timestamp() * 1000)
+            elif isinstance(event_time, date):
+                # convert to unix epoch time in milliseconds.
+                event_time = datetime(*event_time.timetuple()[:7])
+                if event_time.tzinfo is None:
+                    event_time = event_time.replace(tzinfo=timezone.utc)
+                return int(event_time.timestamp() * 1000)
+            elif isinstance(event_time, int):
+                if event_time == 0:
+                    raise ValueError("Event time should be greater than 0.")
+                # jdbc supports timestamp precision up to second only.
+                if len(str(event_time)) <= 10:
+                    event_time = event_time * 1000
+                return event_time
+            else:
+                raise ValueError(
+                    "Given event time should be in `datetime`, `date`, `str` or `int` type"
+                )
+
         # registering the UDF
         _convert_event_time_to_timestamp = udf(
-            util.convert_event_time_to_timestamp, LongType()
+            convert_event_time_to_timestamp, LongType()
         )
 
         result_dfs = {}
         ts_col = _convert_event_time_to_timestamp(col(event_time))
         for split in training_dataset.splits:
             result_df = dataset.filter(ts_col >= split.start_time).filter(
                 ts_col < split.end_time
```

### Comparing `hsfs-3.7.5/hsfs/engine/spark_no_metastore.py` & `hsfs-3.7.6/hsfs/engine/spark_no_metastore.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/expectation_suite.py` & `hsfs-3.7.6/hsfs/expectation_suite.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/feature.py` & `hsfs-3.7.6/hsfs/feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/feature_group.py` & `hsfs-3.7.6/hsfs/feature_group.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/feature_group_commit.py` & `hsfs-3.7.6/hsfs/feature_group_commit.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/feature_group_writer.py` & `hsfs-3.7.6/hsfs/feature_group_writer.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/feature_store.py` & `hsfs-3.7.6/hsfs/feature_store.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/feature_view.py` & `hsfs-3.7.6/hsfs/feature_view.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/ge_expectation.py` & `hsfs-3.7.6/hsfs/ge_expectation.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/ge_validation_result.py` & `hsfs-3.7.6/hsfs/ge_validation_result.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/serving_key.py` & `hsfs-3.7.6/hsfs/serving_key.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/split_statistics.py` & `hsfs-3.7.6/hsfs/split_statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/statistics.py` & `hsfs-3.7.6/hsfs/statistics.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/statistics_config.py` & `hsfs-3.7.6/hsfs/statistics_config.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/storage_connector.py` & `hsfs-3.7.6/hsfs/storage_connector.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/tag.py` & `hsfs-3.7.6/hsfs/tag.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/training_dataset.py` & `hsfs-3.7.6/hsfs/training_dataset.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/training_dataset_feature.py` & `hsfs-3.7.6/hsfs/training_dataset_feature.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/training_dataset_split.py` & `hsfs-3.7.6/hsfs/training_dataset_split.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/transformation_function.py` & `hsfs-3.7.6/hsfs/transformation_function.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/transformation_function_attached.py` & `hsfs-3.7.6/hsfs/transformation_function_attached.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/usage.py` & `hsfs-3.7.6/hsfs/usage.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/user.py` & `hsfs-3.7.6/hsfs/user.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/util.py` & `hsfs-3.7.6/hsfs/util.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/validation_report.py` & `hsfs-3.7.6/hsfs/validation_report.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs/version.py` & `hsfs-3.7.6/hsfs/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #   Unless required by applicable law or agreed to in writing, software
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 #
 
-__version__ = "3.7.5"
+__version__ = "3.7.6"
```

### Comparing `hsfs-3.7.5/hsfs.egg-info/PKG-INFO` & `hsfs-3.7.6/hsfs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: hsfs
-Version: 3.7.5
+Version: 3.7.6
 Summary: HSFS: An environment independent client to interact with the Hopsworks Featurestore
 Home-page: https://github.com/logicalclocks/feature-store-api
 Author: Hopsworks AB
 Author-email: moritz@logicalclocks.com
 License: Apache License 2.0
-Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.5
+Download-URL: https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.6
 Description: # Hopsworks Feature Store
         
         <p align="center">
           <a href="https://community.hopsworks.ai"><img
             src="https://img.shields.io/discourse/users?label=Hopsworks%20Community&server=https%3A%2F%2Fcommunity.hopsworks.ai"
             alt="Hopsworks Community"
           /></a>
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: hsfs Version: 3.7.5 Summary: HSFS: An environment
+Metadata-Version: 2.1 Name: hsfs Version: 3.7.6 Summary: HSFS: An environment
 independent client to interact with the Hopsworks Featurestore Home-page:
 https://github.com/logicalclocks/feature-store-api Author: Hopsworks AB Author-
 email: moritz@logicalclocks.com License: Apache License 2.0 Download-URL:
-https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.5
+https://github.com/logicalclocks/feature-store-api/releases/tag/3.7.6
 Description: # Hopsworks Feature Store
 _[_H_o_p_s_w_o_r_k_s_ _C_o_m_m_u_n_i_t_y_]_[_H_o_p_s_w_o_r_k_s_ _F_e_a_t_u_r_e_ _S_t_o_r_e_ _D_o_c_u_m_e_n_t_a_t_i_o_n_]_[_P_y_P_i_S_t_a_t_u_s_]_[_S_c_a_l_a_/
                 _J_a_v_a_ _A_r_t_i_f_a_c_t_s_]_[_D_o_w_n_l_o_a_d_s_]_[_C_o_d_e_S_t_y_l_e_][License]
 HSFS is the library to interact with the Hopsworks Feature Store. The library
 makes creating new features, feature groups and training datasets easy. The
 library is environment independent and can be used in two modes: - Spark mode:
 For data engineering jobs that create and write features into the feature store
```

### Comparing `hsfs-3.7.5/hsfs.egg-info/SOURCES.txt` & `hsfs-3.7.6/hsfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/hsfs.egg-info/requires.txt` & `hsfs-3.7.6/hsfs.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 PyMySQL[rsa]
 aiomysql
 avro==1.11.3
 boto3
 fsspec
 furl
-great_expectations==0.15.12
+great_expectations==0.18.12
 mock
 numpy<2
 opensearch-py<=2.4.2,>=1.1.0
 pandas<2.2.0
 pyhumps==1.6.1
 pyjks
 requests
```

### Comparing `hsfs-3.7.5/setup.py` & `hsfs-3.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         "pandas<2.2.0",
         "numpy<2",
         "pyjks",
         "mock",
         "avro==1.11.3",
         "sqlalchemy<=1.4.48",  # aiomysql does not support v2 yet https://github.com/aio-libs/aiomysql/discussions/908
         "PyMySQL[rsa]",
-        "great_expectations==0.15.12",
+        "great_expectations==0.18.12",
         "tzlocal",
         "fsspec",
         "retrying",
         "aiomysql",
         "opensearch-py>=1.1.0,<=2.4.2",
     ],
     extras_require={
```

### Comparing `hsfs-3.7.5/tests/__init__.py` & `hsfs-3.7.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `hsfs-3.7.5/tests/test_storage_connector.py` & `hsfs-3.7.6/tests/test_storage_connector.py`

 * *Files identical despite different names*

