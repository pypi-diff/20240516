# Comparing `tmp/deltacat-1.1.4.tar.gz` & `tmp/deltacat-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deltacat-1.1.4.tar", last modified: Tue May  7 00:10:23 2024, max compression
+gzip compressed data, was "dist/deltacat-1.1.5.tar", last modified: Wed May 15 05:26:06 2024, max compression
```

## Comparing `deltacat-1.1.4.tar` & `deltacat-1.1.5.tar`

### file list

```diff
@@ -1,271 +1,271 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 23:58:02.000000 deltacat-1.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-07 00:10:23.000000 deltacat-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-06 23:58:02.000000 deltacat-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/aws/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/aws/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/aws/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/aws/redshift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/aws/redshift/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/aws/redshift/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/aws/redshift/model/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    24859 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/aws/s3u.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/benchmarking/benchmark_parquet_reads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/benchmarking/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/catalog/default_catalog_impl/
--rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/catalog/default_catalog_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/catalog/delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/catalog/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/catalog/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/catalog/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/catalog/model/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/catalog/model/table_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27612 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/compaction_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/compact_partition_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    30547 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/compaction_session_audit_info.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/compactor_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/dedupe_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/delta_annotated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/delta_file_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/delta_file_locator.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/hash_bucket_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/materialize_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/primary_key_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/pyarrow_write_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/repartition_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/round_completion_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/model/table_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/repartition_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor/steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/steps/dedupe.py
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/steps/hash_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/steps/materialize.py
--rw-r--r--   0 runner    (1001) docker     (127)    10960 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/steps/repartition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17303 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/utils/primary_key_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/utils/round_completion_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/utils/sort_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor/utils/system_columns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25193 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/compaction_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/delete_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/model/hash_bucket_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/model/hash_bucket_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/model/merge_file_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/model/merge_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/model/merge_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/steps/hash_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    21657 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/steps/merge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/content_type_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/dedupe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/primary_key_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    13780 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/compactor_v2/utils/task_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/daft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/model/merge_on_read_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/merge_on_read/utils/delta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/metastats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/metastats/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18731 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/meta_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/metastats/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/model/partition_stats_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/model/stats_cluster_size_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/metastats/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/metastats/utils/ray_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/stats/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/models/delta_column_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/models/delta_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/models/delta_stats_cache_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/models/manifest_entry_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/models/stats_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/compute/stats/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/utils/intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/compute/stats/utils/manifest_stats_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/io/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/io/aws/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/aws/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22599 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/aws/redshift/redshift_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/file_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/memcached_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/ray_plasma_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/read_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/redis_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/io/s3_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21649 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/storage/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/delete_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/list_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/locator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/sort_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/table_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/storage/model/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/aws/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/aws/test_s3u.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/catalog/test_default_catalog_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/compute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72082 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)    20092 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compact_partition_test_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/steps/test_repartition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor/utils/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/compute/compactor_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor_v2/test_compaction_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor_v2/test_hashlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/compute/compactor_v2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor_v2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/compactor_v2/utils/test_task_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    10271 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/test_compact_partition_incremental.py
--rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/test_compact_partition_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/test_util_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/test_util_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/compute/test_util_create_table_deltas_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/io/test_cloudpickle_bug_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/io/test_file_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/io/test_memcached_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/io/test_ray_plasma_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/io/test_redis_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/io/test_s3_object_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/local_deltacat_storage/
--rw-r--r--   0 runner    (1001) docker     (127)    35466 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/local_deltacat_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/stats/test_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/test_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/test_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/test_utils/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/test_utils/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/test_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/tests/utils/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/test_cloudpickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/test_daft.py
--rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/test_placement.py
--rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/test_pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/test_record_batch_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/tests/utils/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/types/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/types/partial_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/types/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/cloudpickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/daft.py
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/placement.py
--rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/pyarrow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat/utils/ray_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/ray_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/ray_utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/ray_utils/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/ray_utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/ray_utils/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/ray_utils/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/s3fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-06 23:58:02.000000 deltacat-1.1.4/deltacat/utils/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-07 00:10:22.000000 deltacat-1.1.4/deltacat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-07 00:10:23.000000 deltacat-1.1.4/deltacat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 00:10:22.000000 deltacat-1.1.4/deltacat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-07 00:10:22.000000 deltacat-1.1.4/deltacat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 00:10:22.000000 deltacat-1.1.4/deltacat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 00:10:23.000000 deltacat-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-06 23:58:02.000000 deltacat-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 05:12:58.000000 deltacat-1.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-15 05:26:06.000000 deltacat-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-15 05:12:58.000000 deltacat-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/aws/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/aws/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/aws/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/aws/redshift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/aws/redshift/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/aws/redshift/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/aws/redshift/model/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24859 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/aws/s3u.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/benchmarking/benchmark_parquet_reads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/benchmarking/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/catalog/default_catalog_impl/
+-rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/catalog/default_catalog_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/catalog/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/catalog/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/catalog/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/catalog/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/catalog/model/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/catalog/model/table_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/compactor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27612 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/compaction_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/compactor/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/model/compact_partition_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30547 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/model/compaction_session_audit_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/model/compactor_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/model/dedupe_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/model/delta_annotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/model/delta_file_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/model/delta_file_locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/model/hash_bucket_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/model/materialize_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/model/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/model/pyarrow_write_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/model/repartition_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/model/round_completion_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/model/table_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/repartition_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/compactor/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/steps/dedupe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/steps/hash_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/steps/materialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10960 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/steps/repartition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/compactor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17303 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/utils/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/utils/round_completion_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/utils/sort_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor/utils/system_columns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26087 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/compaction_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/deletes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/deletes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/deletes/delete_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/deletes/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/deletes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/model/hash_bucket_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/model/hash_bucket_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/model/merge_file_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/model/merge_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/model/merge_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/steps/hash_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21657 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/steps/merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/utils/content_type_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/utils/dedupe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/utils/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/utils/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/utils/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13857 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/compactor_v2/utils/task_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/merge_on_read/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/merge_on_read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/merge_on_read/daft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/merge_on_read/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/merge_on_read/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/merge_on_read/model/merge_on_read_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/merge_on_read/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/merge_on_read/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/merge_on_read/utils/delta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/metastats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/metastats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/metastats/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/metastats/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18731 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/metastats/meta_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/metastats/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/metastats/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/metastats/model/partition_stats_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/metastats/model/stats_cluster_size_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/metastats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/metastats/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/metastats/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/metastats/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/metastats/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/metastats/utils/ray_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/stats/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/stats/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/stats/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/stats/models/delta_column_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/stats/models/delta_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/stats/models/delta_stats_cache_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/stats/models/manifest_entry_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/stats/models/stats_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/stats/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/compute/stats/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/stats/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/stats/utils/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/stats/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/compute/stats/utils/manifest_stats_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/io/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/io/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/io/aws/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/io/aws/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22599 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/io/aws/redshift/redshift_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/io/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/io/file_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/io/memcached_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/io/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/io/ray_plasma_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/io/read_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/io/redis_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/io/s3_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21649 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/storage/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/storage/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/storage/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/storage/model/delete_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/storage/model/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/storage/model/list_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/storage/model/locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/storage/model/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/storage/model/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/storage/model/sort_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/storage/model/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/storage/model/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/storage/model/table_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/storage/model/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/tests/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/aws/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/aws/test_s3u.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/tests/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/catalog/test_default_catalog_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/tests/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73645 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22651 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/compact_partition_test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/tests/compute/compactor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/compactor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/tests/compute/compactor/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/compactor/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/compactor/steps/test_repartition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/tests/compute/compactor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/compactor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/compactor/utils/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/tests/compute/compactor_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/compactor_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/compactor_v2/test_compaction_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/compactor_v2/test_hashlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/tests/compute/compactor_v2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/compactor_v2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/compactor_v2/utils/test_task_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11301 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/test_compact_partition_incremental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/test_compact_partition_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14364 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/test_util_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/test_util_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/compute/test_util_create_table_deltas_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/io/test_cloudpickle_bug_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/io/test_file_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/io/test_memcached_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/io/test_ray_plasma_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/io/test_redis_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/io/test_s3_object_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/tests/local_deltacat_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)    35466 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/local_deltacat_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/tests/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/stats/test_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/test_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/test_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/test_utils/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/test_utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/test_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/tests/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/utils/test_cloudpickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/utils/test_daft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/utils/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/utils/test_placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/utils/test_pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/utils/test_record_batch_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/tests/utils/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/types/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/types/partial_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/types/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/cloudpickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/daft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/pyarrow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat/utils/ray_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/ray_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/ray_utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/ray_utils/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/ray_utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/ray_utils/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/ray_utils/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/s3fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-15 05:12:58.000000 deltacat-1.1.5/deltacat/utils/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-15 05:26:05.000000 deltacat-1.1.5/deltacat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-15 05:26:06.000000 deltacat-1.1.5/deltacat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 05:26:05.000000 deltacat-1.1.5/deltacat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-15 05:26:05.000000 deltacat-1.1.5/deltacat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-15 05:26:05.000000 deltacat-1.1.5/deltacat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 05:26:06.000000 deltacat-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-15 05:12:58.000000 deltacat-1.1.5/setup.py
```

### Comparing `deltacat-1.1.4/PKG-INFO` & `deltacat-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltacat
-Version: 1.1.4
+Version: 1.1.5
 Summary: A scalable, fast, ACID-compliant Data Catalog powered by Ray.
 Home-page: https://github.com/ray-project/deltacat
 Author: Ray Team
 License: UNKNOWN
 Description: # DeltaCAT
         
         DeltaCAT is a Pythonic Data Catalog powered by Ray.
```

### Comparing `deltacat-1.1.4/README.md` & `deltacat-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/__init__.py` & `deltacat-1.1.5/deltacat/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     SortOrder,
 )
 from deltacat.types.media import ContentEncoding, ContentType, TableType
 from deltacat.types.tables import TableWriteMode
 
 deltacat.logs.configure_deltacat_logger(logging.getLogger(__name__))
 
-__version__ = "1.1.4"
+__version__ = "1.1.5"
 
 
 __all__ = [
     "__version__",
     "all_catalogs",
     "alter_table",
     "create_table",
```

### Comparing `deltacat-1.1.4/deltacat/aws/clients.py` & `deltacat-1.1.5/deltacat/aws/clients.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/aws/redshift/model/manifest.py` & `deltacat-1.1.5/deltacat/aws/redshift/model/manifest.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/aws/s3u.py` & `deltacat-1.1.5/deltacat/aws/s3u.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/benchmarking/benchmark_parquet_reads.py` & `deltacat-1.1.5/deltacat/benchmarking/benchmark_parquet_reads.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/benchmarking/conftest.py` & `deltacat-1.1.5/deltacat/benchmarking/conftest.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/catalog/default_catalog_impl/__init__.py` & `deltacat-1.1.5/deltacat/catalog/default_catalog_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/catalog/delegate.py` & `deltacat-1.1.5/deltacat/catalog/delegate.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/catalog/interface.py` & `deltacat-1.1.5/deltacat/catalog/interface.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/catalog/model/catalog.py` & `deltacat-1.1.5/deltacat/catalog/model/catalog.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/catalog/model/table_definition.py` & `deltacat-1.1.5/deltacat/catalog/model/table_definition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/__init__.py` & `deltacat-1.1.5/deltacat/compute/compactor/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/compaction_session.py` & `deltacat-1.1.5/deltacat/compute/compactor/compaction_session.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/model/compact_partition_params.py` & `deltacat-1.1.5/deltacat/compute/compactor/model/compact_partition_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/model/compaction_session_audit_info.py` & `deltacat-1.1.5/deltacat/compute/compactor/model/compaction_session_audit_info.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/model/delta_annotated.py` & `deltacat-1.1.5/deltacat/compute/compactor/model/delta_annotated.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/model/delta_file_envelope.py` & `deltacat-1.1.5/deltacat/compute/compactor/model/delta_file_envelope.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/model/delta_file_locator.py` & `deltacat-1.1.5/deltacat/compute/compactor/model/delta_file_locator.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/model/materialize_result.py` & `deltacat-1.1.5/deltacat/compute/compactor/model/materialize_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/model/primary_key_index.py` & `deltacat-1.1.5/deltacat/compute/compactor/model/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/model/pyarrow_write_result.py` & `deltacat-1.1.5/deltacat/compute/compactor/model/pyarrow_write_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/model/round_completion_info.py` & `deltacat-1.1.5/deltacat/compute/compactor/model/round_completion_info.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/model/table_object_store.py` & `deltacat-1.1.5/deltacat/compute/compactor/model/table_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/repartition_session.py` & `deltacat-1.1.5/deltacat/compute/compactor/repartition_session.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/steps/dedupe.py` & `deltacat-1.1.5/deltacat/compute/compactor/steps/dedupe.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/steps/hash_bucket.py` & `deltacat-1.1.5/deltacat/compute/compactor/steps/hash_bucket.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/steps/materialize.py` & `deltacat-1.1.5/deltacat/compute/compactor/steps/materialize.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/steps/repartition.py` & `deltacat-1.1.5/deltacat/compute/compactor/steps/repartition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/utils/io.py` & `deltacat-1.1.5/deltacat/compute/compactor/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/utils/primary_key_index.py` & `deltacat-1.1.5/deltacat/compute/compactor/utils/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/utils/round_completion_file.py` & `deltacat-1.1.5/deltacat/compute/compactor/utils/round_completion_file.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/utils/sort_key.py` & `deltacat-1.1.5/deltacat/compute/compactor/utils/sort_key.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor/utils/system_columns.py` & `deltacat-1.1.5/deltacat/compute/compactor/utils/system_columns.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/compaction_session.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/compaction_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 from deltacat.compute.compactor_v2.model.hash_bucket_input import HashBucketInput
 
 from deltacat.compute.compactor_v2.model.merge_input import MergeInput
 
 from deltacat.aws import s3u as s3_utils
 import deltacat
 from deltacat import logs
-from deltacat.compute.compactor import PyArrowWriteResult, RoundCompletionInfo
+from deltacat.compute.compactor import (
+    HighWatermark,
+    PyArrowWriteResult,
+    RoundCompletionInfo,
+)
 from deltacat.compute.compactor_v2.model.merge_result import MergeResult
 from deltacat.compute.compactor_v2.model.hash_bucket_result import HashBucketResult
 from deltacat.compute.compactor.model.materialize_result import MaterializeResult
 from deltacat.compute.compactor_v2.utils.merge import (
     generate_local_merge_input,
 )
 from deltacat.compute.compactor import DeltaAnnotated
@@ -33,14 +37,15 @@
     DeleteFileEnvelope,
 )
 from deltacat.compute.compactor_v2.deletes.utils import prepare_deletes
 
 from deltacat.storage import (
     Delta,
     DeltaLocator,
+    Manifest,
     Partition,
 )
 from deltacat.compute.compactor.model.compact_partition_params import (
     CompactPartitionParams,
 )
 from deltacat.utils.ray_utils.concurrency import (
     invoke_parallel,
@@ -92,15 +97,15 @@
         logger.info(
             f"Partition-{params.source_partition_locator} -> "
             f"Compaction session data processing completed"
         )
         round_completion_file_s3_url = None
         if new_partition:
             logger.info(f"Committing compacted partition to: {new_partition.locator}")
-            partition = params.deltacat_storage.commit_partition(
+            partition: Partition = params.deltacat_storage.commit_partition(
                 new_partition, **params.deltacat_storage_kwargs
             )
             logger.info(f"Committed compacted partition: {partition}")
 
             round_completion_file_s3_url = rcf.write_round_completion_file(
                 params.compaction_artifact_s3_bucket,
                 new_rcf_partition_locator,
@@ -146,17 +151,17 @@
         cluster_resources = params.pg_config.resource
         cluster_cpus = cluster_resources["CPU"]
         cluster_memory = cluster_resources["memory"]
         task_max_parallelism = cluster_cpus
         compaction_audit.set_total_cluster_memory_bytes(cluster_memory)
 
     # read the results from any previously completed compaction round
-    round_completion_info = None
-    high_watermark = None
-    previous_compacted_delta_manifest = None
+    round_completion_info: Optional[RoundCompletionInfo] = None
+    high_watermark: Optional[HighWatermark] = None
+    previous_compacted_delta_manifest: Optional[Manifest] = None
 
     if not params.rebase_source_partition_locator:
         round_completion_info = rcf.read_round_completion_file(
             params.compaction_artifact_s3_bucket,
             params.source_partition_locator,
             **params.s3_client_kwargs,
         )
@@ -267,14 +272,15 @@
         memory_logs_enabled=params.memory_logs_enabled,
     )
 
     total_input_records_count = np.int64(0)
     total_hb_record_count = np.int64(0)
     telemetry_time_hb = 0
     if params.hash_bucket_count == 1:
+        logger.info("Hash bucket count set to 1. Running local merge")
         merge_start = time.monotonic()
         local_merge_input = generate_local_merge_input(
             params,
             uniform_deltas,
             compacted_partition,
             round_completion_info,
             delete_strategy,
@@ -630,12 +636,25 @@
         input_average_record_size_bytes=input_average_record_size_bytes,
     )
 
     logger.info(
         f"partition-{params.source_partition_locator.partition_values},"
         f"compacted at: {params.last_stream_position_to_compact},"
     )
+    is_inplace_compacted: bool = (
+        params.source_partition_locator.partition_values
+        == params.destination_partition_locator.partition_values
+        and params.source_partition_locator.stream_id
+        == params.destination_partition_locator.stream_id
+    )
+    if is_inplace_compacted:
+        logger.info(
+            "Overriding round completion file source partition locator as in-place compacted. "
+            + f"Got compacted partition partition_id of {compacted_partition.locator.partition_id} "
+            f"and rcf source partition_id of {rcf_source_partition_locator.partition_id}."
+        )
+        rcf_source_partition_locator = compacted_partition.locator
     return (
         compacted_partition,
         new_round_completion_info,
         rcf_source_partition_locator,
     )
```

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/constants.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/constants.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/delete_strategy.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/deletes/delete_strategy.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/model.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/deletes/model.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/deletes/utils.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/deletes/utils.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/model/hash_bucket_input.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/model/hash_bucket_input.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/model/merge_file_group.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/model/merge_file_group.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/model/merge_input.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/model/merge_input.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/steps/hash_bucket.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/steps/hash_bucket.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/steps/merge.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/steps/merge.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/utils/content_type_params.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/utils/content_type_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/utils/dedupe.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/utils/dedupe.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/utils/delta.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/utils/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/utils/io.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/utils/merge.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/utils/merge.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/utils/primary_key_index.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/utils/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/compactor_v2/utils/task_options.py` & `deltacat-1.1.5/deltacat/compute/compactor_v2/utils/task_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 from deltacat.compute.compactor_v2.utils.primary_key_index import (
     hash_group_index_to_hash_bucket_indices,
 )
 from deltacat.compute.compactor_v2.constants import (
     PARQUET_TO_PYARROW_INFLATION,
 )
 
+from daft.exceptions import DaftTransientError
+
+
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
 
 
 def _get_parquet_type_params_if_exist(
     entry: ManifestEntry,
 ) -> Optional[PartialParquetParameters]:
     if (
@@ -72,14 +75,15 @@
     # List of possible botocore exceptions are available at
     # https://github.com/boto/botocore/blob/develop/botocore/exceptions.py
     task_opts["retry_exceptions"] = [
         botocore.exceptions.ConnectionError,
         botocore.exceptions.HTTPClientError,
         ConnectionError,
         TimeoutError,
+        DaftTransientError,
     ]
 
     return task_opts
 
 
 def estimate_manifest_entry_size_bytes(
     entry: ManifestEntry, previous_inflation: float, **kwargs
```

### Comparing `deltacat-1.1.4/deltacat/compute/merge_on_read/daft.py` & `deltacat-1.1.5/deltacat/compute/merge_on_read/daft.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/merge_on_read/model/merge_on_read_params.py` & `deltacat-1.1.5/deltacat/compute/merge_on_read/model/merge_on_read_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/merge_on_read/utils/delta.py` & `deltacat-1.1.5/deltacat/compute/merge_on_read/utils/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/metastats/meta_stats.py` & `deltacat-1.1.5/deltacat/compute/metastats/meta_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/metastats/model/partition_stats_dict.py` & `deltacat-1.1.5/deltacat/compute/metastats/model/partition_stats_dict.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/metastats/model/stats_cluster_size_estimator.py` & `deltacat-1.1.5/deltacat/compute/metastats/model/stats_cluster_size_estimator.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/metastats/stats.py` & `deltacat-1.1.5/deltacat/compute/metastats/stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/metastats/utils/constants.py` & `deltacat-1.1.5/deltacat/compute/metastats/utils/constants.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/metastats/utils/io.py` & `deltacat-1.1.5/deltacat/compute/metastats/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py` & `deltacat-1.1.5/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/metastats/utils/ray_utils.py` & `deltacat-1.1.5/deltacat/compute/metastats/utils/ray_utils.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/stats/basic.py` & `deltacat-1.1.5/deltacat/compute/stats/basic.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/stats/models/delta_column_stats.py` & `deltacat-1.1.5/deltacat/compute/stats/models/delta_column_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/stats/models/delta_stats.py` & `deltacat-1.1.5/deltacat/compute/stats/models/delta_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/stats/models/delta_stats_cache_result.py` & `deltacat-1.1.5/deltacat/compute/stats/models/delta_stats_cache_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/stats/models/manifest_entry_stats.py` & `deltacat-1.1.5/deltacat/compute/stats/models/manifest_entry_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/stats/models/stats_result.py` & `deltacat-1.1.5/deltacat/compute/stats/models/stats_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/stats/utils/intervals.py` & `deltacat-1.1.5/deltacat/compute/stats/utils/intervals.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/stats/utils/io.py` & `deltacat-1.1.5/deltacat/compute/stats/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/compute/stats/utils/manifest_stats_file.py` & `deltacat-1.1.5/deltacat/compute/stats/utils/manifest_stats_file.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/constants.py` & `deltacat-1.1.5/deltacat/constants.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/io/aws/redshift/redshift_datasource.py` & `deltacat-1.1.5/deltacat/io/aws/redshift/redshift_datasource.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/io/dataset.py` & `deltacat-1.1.5/deltacat/io/dataset.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/io/file_object_store.py` & `deltacat-1.1.5/deltacat/io/file_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/io/memcached_object_store.py` & `deltacat-1.1.5/deltacat/io/memcached_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/io/object_store.py` & `deltacat-1.1.5/deltacat/io/object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/io/ray_plasma_object_store.py` & `deltacat-1.1.5/deltacat/io/ray_plasma_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/io/read_api.py` & `deltacat-1.1.5/deltacat/io/read_api.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/io/redis_object_store.py` & `deltacat-1.1.5/deltacat/io/redis_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/io/s3_object_store.py` & `deltacat-1.1.5/deltacat/io/s3_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/logs.py` & `deltacat-1.1.5/deltacat/logs.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/storage/__init__.py` & `deltacat-1.1.5/deltacat/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/storage/interface.py` & `deltacat-1.1.5/deltacat/storage/interface.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/storage/model/delete_parameters.py` & `deltacat-1.1.5/deltacat/storage/model/delete_parameters.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/storage/model/delta.py` & `deltacat-1.1.5/deltacat/storage/model/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/storage/model/list_result.py` & `deltacat-1.1.5/deltacat/storage/model/list_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/storage/model/locator.py` & `deltacat-1.1.5/deltacat/storage/model/locator.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/storage/model/namespace.py` & `deltacat-1.1.5/deltacat/storage/model/namespace.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/storage/model/partition.py` & `deltacat-1.1.5/deltacat/storage/model/partition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/storage/model/sort_key.py` & `deltacat-1.1.5/deltacat/storage/model/sort_key.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/storage/model/stream.py` & `deltacat-1.1.5/deltacat/storage/model/stream.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/storage/model/table.py` & `deltacat-1.1.5/deltacat/storage/model/table.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/storage/model/table_version.py` & `deltacat-1.1.5/deltacat/storage/model/table_version.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/storage/model/types.py` & `deltacat-1.1.5/deltacat/storage/model/types.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/aws/test_clients.py` & `deltacat-1.1.5/deltacat/tests/aws/test_clients.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/catalog/test_default_catalog_impl.py` & `deltacat-1.1.5/deltacat/tests/catalog/test_default_catalog_impl.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py` & `deltacat-1.1.5/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,14 +103,15 @@
                 pa.array([i for i in range(20, 30)]),
                 pa.array(["foo"] * 10),
                 pa.array([i / 10 for i in range(40, 50)]),
             ],
             names=["pk_col_1", "sk_col_1", "sk_col_2", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=None,
     ),
@@ -182,14 +183,15 @@
                     ]
                 ),
                 pa.array([1, 1.1, 1.2, 1.3]),
             ],
             names=["pk_col_1", "pk_col_2", "sk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=None,
     ),
@@ -230,14 +232,15 @@
             [
                 pa.array(["0", "1", "2", "3"]),
                 pa.array([18.0, 19.0, 20.0, 21.0]),
             ],
             names=["pk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=None,
     ),
@@ -278,14 +281,15 @@
             [
                 pa.array([str(i) for i in range(10)]),
                 pa.array([i / 10 for i in range(8)] + [200.0] + [100.0]),
             ],
             names=["pk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=None,
     ),
@@ -332,14 +336,15 @@
                 pa.array([0, 1, 2, 3, 4]),
                 pa.array([3.0, 4.0, 1.0, 0.0, 2.0]),
                 pa.array(["i", "a", "k", "l", "b"]),
             ],
             names=["pk_col_1", "sk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=None,
     ),
@@ -391,14 +396,15 @@
                 pa.array([i for i in range(20, 32)]),
                 pa.array(["foo"] * 12),
                 pa.array([i / 10 for i in range(40, 52)]),
             ],
             names=["pk_col_1", "sk_col_1", "sk_col_2", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=10,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT + 10,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -441,14 +447,15 @@
             [
                 pa.array([1, 1, 2, 2, 3, 3, 4, 5, 6]),
                 pa.array([1.0, 1.0, 2.0, 2.0, 3.0, 3.0, 10.0, 11.0, 12.0]),
             ],
             names=["sk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=10,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -496,14 +503,15 @@
             [
                 pa.array(["0", "1", "2", "3", "4", "5", "6", "7", "8", "9"]),
                 pa.array([1.0, 1.1, 1.2, 1.3, 1.4, 1.5, 1.6, 1.7, 1.8, 1.9]),
             ],
             names=["pk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=None,
     ),
@@ -555,14 +563,15 @@
                 pa.array([i for i in range(20, 30)]),
                 pa.array(["foo"] * 10),
                 pa.array([i / 10 for i in range(40, 50)]),
             ],
             names=["pk_col_1", "sk_col_1", "sk_col_2", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=1,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=None,
     ),
@@ -609,14 +618,15 @@
                 pa.array([0, 0, 1, 1, 1, 2, 2, 3, 3]),
                 pa.array([0, 0, 1, 0, 1, 0, 0, 1, 1]),
                 pa.array([1.4, 2, 1.5, 2.4, 2.1, 1.6, 2.2, 1.7, 2.3]),
             ],
             names=["pk_col_1", "sk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=False,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -654,14 +664,15 @@
                 pa.array([i for i in range(0, 10)]),
                 pa.array(["foo"] * 10),
                 pa.array([i / 10 for i in range(10, 20)]),
             ],
             names=["pk_col_1", "sk_col_1", "sk_col_2", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=3,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=None,
     ),
@@ -713,14 +724,15 @@
                 pa.array([i for i in range(20, 30)]),
                 pa.array(["foo"] * 10),
                 pa.array([i / 10 for i in range(40, 50)]),
             ],
             names=["pk_col_1", "sk_col_1", "sk_col_2", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=1,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=None,
     ),
@@ -758,14 +770,15 @@
                 pa.array([i for i in range(0, 10)]),
                 pa.array(["foo"] * 10),
                 pa.array([i / 10 for i in range(10, 20)]),
             ],
             names=["pk_col_1", "sk_col_1", "sk_col_2", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=1,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=None,
     ),
@@ -857,14 +870,15 @@
             [
                 pa.array([i for i in range(10)] + [13]),
                 pa.array([str(i) for i in range(0, 10)] + ["d"]),
             ],
             names=["pk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -907,14 +921,15 @@
                 pa.array([0, 1]),
                 pa.array([0.0, 3.0]),
                 pa.array(["8", "9"]),
             ],
             names=["pk_col_1", "pk_col_2", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -963,14 +978,15 @@
                     ("pk_col_1", pa.int64()),
                     ("pk_col_2", pa.float64()),
                     ("col_1", pa.string()),
                 ]
             ),
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -1015,14 +1031,15 @@
                 [
                     ("pk_col_1", pa.int64()),
                     ("col_1", pa.string()),
                 ]
             ),
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=True,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -1095,14 +1112,15 @@
             [
                 pa.array([5]),
                 pa.array(["buz"]),
             ],
             names=["pk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=True,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -1164,14 +1182,15 @@
             [
                 pa.array([0, 1, 2, 3, 4, 5]),
                 pa.array(["foo", "1", "2", "3", "4", "5"]),
             ],
             names=["pk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=True,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -1227,14 +1246,15 @@
                 [
                     ("pk_col_1", pa.int64()),
                     ("col_1", pa.string()),
                 ]
             ),
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=True,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -1317,14 +1337,15 @@
             [
                 pa.array([0, 4, 5, 7]),
                 pa.array(["0", "4", "5", "aaa"]),
             ],
             names=["pk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=True,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -1380,14 +1401,15 @@
                 [
                     ("pk_col_1", pa.int64()),
                     ("col_1", pa.string()),
                 ]
             ),
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=True,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -1449,14 +1471,15 @@
             [
                 pa.array([0]),
                 pa.array(["1"]),
             ],
             names=["pk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=True,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -1512,14 +1535,15 @@
                 [
                     ("pk_col_1", pa.int64()),
                     ("col_1", pa.string()),
                 ]
             ),
         ),
         expected_terminal_exception=AssertionError,
+        expected_terminal_exception_message="Delete type deltas are required to have delete parameters defined",
         do_create_placement_group=True,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -1576,14 +1600,15 @@
             [
                 pa.array([0, 1, 2]),
                 pa.array(["1", "1", "2"]),
             ],
             names=["pk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=True,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -1634,14 +1659,15 @@
             [
                 pa.array([3]),
                 pa.array(["3"]),
             ],
             names=["pk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=True,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -1702,14 +1728,15 @@
             [
                 pa.array([0, 3, 4]),
                 pa.array(["a", "b", "4"]),
             ],
             names=["pk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=True,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -1791,14 +1818,15 @@
                 pa.array([i for i in range(25, 30)]),
                 pa.array(["foo"] * 5),
                 pa.array([i / 10 for i in range(45, 50)]),
             ],
             names=["pk_col_1", "sk_col_1", "sk_col_2", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=1,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -1861,14 +1889,15 @@
             [
                 pa.array([1, 1, 2, 2, 4, 5]),
                 pa.array([1.0, 1.0, 2.0, 2.0, 10.0, 11.0]),
             ],
             names=["sk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=10,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
@@ -1909,14 +1938,15 @@
             [
                 pa.array([i for i in range(10)]),
                 pa.array([str(i) for i in range(0, 10)]),
             ],
             names=["pk_col_1", "col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         skip_enabled_compact_partition_drivers=None,
     ),
```

### Comparing `deltacat-1.1.4/deltacat/tests/compute/compact_partition_test_cases.py` & `deltacat-1.1.5/deltacat/tests/compute/compact_partition_test_cases.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         sort_keys: List[SortKey] - argument for the sort_keys parameter in compact_partition. Also needed for table/delta creation
         partition_keys_param: List[PartitionKey] - argument for the partition_keys parameter. Needed for table/delta creation
         partition_values_param: List[Optional[str]] - argument for the partition_valued parameter. Needed for table/delta creation
         input_deltas: List[pa.Array] - argument required for delta creation during compact_partition test setup. Actual incoming deltas expressed as a PyArrow array (https://arrow.apache.org/docs/python/generated/pyarrow.array.html)
         input_deltas_delta_type: DeltaType - enumerated argument required for delta creation during compact_partition test setup. Available values are (DeltaType.APPEND, DeltaType.UPSERT, DeltaType.DELETE). DeltaType.APPEND is not supported by compactor v1 or v2
         expected_terminal_compact_partition_result: pa.Table - expected PyArrow table after compaction (i.e,. the state of the table after applying all row UPDATES/DELETES/INSERTS)
         expected_terminal_exception: BaseException - expected exception during compaction
+        expected_terminal_exception_message: Optional[str] - expected exception message if present.
         do_create_placement_group: bool - toggles whether to create a placement group (https://docs.ray.io/en/latest/ray-core/scheduling/placement-group.html) or not
         records_per_compacted_file: int - argument for the records_per_compacted_file parameter in compact_partition
         hash_bucket_count_param: int - argument for the hash_bucket_count parameter in compact_partition
         read_kwargs_provider: Optional[ReadKwargsProvider] - argument for read_kwargs_provider parameter in compact_partition. If None then no ReadKwargsProvider is provided to compact_partition_params
         drop_duplicates: bool - argument for drop_duplicates parameter in compact_partition. Only recognized by compactor v2.
         skip_enabled_compact_partition_drivers: List[CompactorVersion] - skip whatever enabled_compact_partition_drivers are included in this list
     """
@@ -66,29 +67,35 @@
     sort_keys: List[Optional[SortKey]]
     partition_keys: Optional[List[PartitionKey]]
     partition_values: List[Optional[str]]
     input_deltas: Union[List[pa.Array], pa.Table]
     input_deltas_delta_type: DeltaType
     expected_terminal_compact_partition_result: pa.Table
     expected_terminal_exception: BaseException
+    expected_terminal_exception_message: str
     do_create_placement_group: bool
     records_per_compacted_file: int
     hash_bucket_count: int
     read_kwargs_provider: Optional[ReadKwargsProvider]
     drop_duplicates: bool
     skip_enabled_compact_partition_drivers: List[CompactorVersion]
 
     # makes CompactorTestCase iterable which is required to build the list of pytest.param values to pass to pytest.mark.parametrize
     def __iter__(self):
         return (getattr(self, field.name) for field in fields(self))
 
 
 @dataclass(frozen=True)
 class IncrementalCompactionTestCaseParams(BaseCompactorTestCase):
-    pass
+    """
+    Args:
+        is_inplace: bool - argument to indicate whether to try compacting an in-place compacted table (the source table is the destination table). Also needed to control whether the destination table is created
+    """
+
+    is_inplace: bool
 
 
 @dataclass(frozen=True)
 class NoRCFOutputCompactionTestCaseParams(BaseCompactorTestCase):
     pass
 
 
@@ -130,19 +137,21 @@
         ),
         input_deltas_delta_type=DeltaType.UPSERT,
         expected_terminal_compact_partition_result=pa.Table.from_arrays(
             [pa.array([str(i) for i in range(10)])],
             names=["pk_col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
+        is_inplace=False,
         skip_enabled_compact_partition_drivers=None,
     ),
     "2-incremental-pkstr-skstr-norcf": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=ZERO_VALUED_SORT_KEY,
         partition_keys=[PartitionKey.of("region_id", PartitionKeyType.INT)],
         partition_values=["1"],
@@ -155,19 +164,21 @@
         ),
         input_deltas_delta_type=DeltaType.UPSERT,
         expected_terminal_compact_partition_result=pa.Table.from_arrays(
             [pa.array([str(i) for i in range(10)]), pa.array(["test"] * 10)],
             names=["pk_col_1", "sk_col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
+        is_inplace=False,
         skip_enabled_compact_partition_drivers=None,
     ),
     "3-incremental-pkstr-multiskstr-norcf": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[
             SortKey.of(key_name="sk_col_1"),
             SortKey.of(key_name="sk_col_2"),
@@ -189,19 +200,21 @@
                 pa.array([str(i) for i in range(10)]),
                 pa.array(["test"] * 10),
                 pa.array(["foo"] * 10),
             ],
             names=["pk_col_1", "sk_col_1", "sk_col_2"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
+        is_inplace=False,
         skip_enabled_compact_partition_drivers=None,
     ),
     "4-incremental-duplicate-pk": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[
             SortKey.of(key_name="sk_col_1"),
             SortKey.of(key_name="sk_col_2"),
@@ -222,19 +235,21 @@
                 pa.array([str(i) for i in range(5)] + ["6"]),
                 pa.array([str(i) for i in range(5)] + ["9"]),
                 pa.array(["foo"] * 6),
             ],
             names=["pk_col_1", "sk_col_1", "sk_col_2"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
+        is_inplace=False,
         skip_enabled_compact_partition_drivers=None,
     ),
     "5-incremental-decimal-pk-simple": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=[PartitionKey.of("region_id", PartitionKeyType.INT)],
         partition_values=["1"],
@@ -250,19 +265,21 @@
             [
                 pa.array([i / 10 for i in range(0, 10)]),
                 pa.array([str(i) for i in range(10)]),
             ],
             names=["pk_col_1", "sk_col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
+        is_inplace=False,
         skip_enabled_compact_partition_drivers=None,
     ),
     "6-incremental-integer-pk-simple": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=[PartitionKey.of("region_id", PartitionKeyType.INT)],
         partition_values=["1"],
@@ -278,19 +295,21 @@
             [
                 pa.array([i for i in range(0, 10)]),
                 pa.array([str(i) for i in range(10)]),
             ],
             names=["pk_col_1", "sk_col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
+        is_inplace=False,
         skip_enabled_compact_partition_drivers=None,
     ),
     "7-incremental-timestamp-pk-simple": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=[PartitionKey.of("region_id", PartitionKeyType.INT)],
         partition_values=["1"],
@@ -306,19 +325,21 @@
             [
                 pa.array(offer_iso8601_timestamp_list(10, "minutes")),
                 pa.array([str(i) for i in range(10)]),
             ],
             names=["pk_col_1", "sk_col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
+        is_inplace=False,
         skip_enabled_compact_partition_drivers=None,
     ),
     "8-incremental-decimal-timestamp-pk-multi": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1", "pk_col_2"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=[PartitionKey.of("region_id", PartitionKeyType.INT)],
         partition_values=["1"],
@@ -336,19 +357,21 @@
                 pa.array([i / 10 for i in range(0, 20)]),
                 pa.array(offer_iso8601_timestamp_list(20, "minutes")),
                 pa.array([0.1] * 4 + [0.2] * 4 + [0.3] * 4 + [0.4] * 4 + [0.5] * 4),
             ],
             names=["pk_col_1", "pk_col_2", "sk_col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
+        is_inplace=False,
         skip_enabled_compact_partition_drivers=None,
     ),
     "9-incremental-decimal-pk-multi-dup": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=[PartitionKey.of("region_id", PartitionKeyType.INT)],
         partition_values=["1"],
@@ -364,19 +387,21 @@
             [
                 pa.array([0.1, 0.2, 0.3, 0.4, 0.5]),
                 pa.array([19, 15, 11, 7, 3]),
             ],
             names=["pk_col_1", "sk_col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
+        is_inplace=False,
         skip_enabled_compact_partition_drivers=None,
     ),
     "10-incremental-decimal-pk-partitionless": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=ZERO_VALUED_PARTITION_KEYS_PARAM,
         partition_values=ZERO_VALUED_PARTITION_VALUES_PARAM,
@@ -392,19 +417,21 @@
             [
                 pa.array([0.1, 0.2, 0.3, 0.4, 0.5]),
                 pa.array([3, 7, 11, 15, 19]),
             ],
             names=["pk_col_1", "sk_col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
+        is_inplace=False,
         skip_enabled_compact_partition_drivers=None,
     ),
     "11-incremental-decimal-hash-bucket-single": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=ZERO_VALUED_PARTITION_KEYS_PARAM,
         partition_values=ZERO_VALUED_PARTITION_VALUES_PARAM,
@@ -420,19 +447,21 @@
             [
                 pa.array([0.1, 0.2, 0.3, 0.4, 0.5]),
                 pa.array([3, 7, 11, 15, 19]),
             ],
             names=["pk_col_1", "sk_col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
+        is_inplace=False,
         skip_enabled_compact_partition_drivers=None,
     ),
     "12-incremental-decimal-single-hash-bucket": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=ZERO_VALUED_PARTITION_KEYS_PARAM,
         partition_values=ZERO_VALUED_PARTITION_VALUES_PARAM,
@@ -448,17 +477,49 @@
             [
                 pa.array([0.1, 0.2, 0.3, 0.4, 0.5]),
                 pa.array([3, 7, 11, 15, 19]),
             ],
             names=["pk_col_1", "sk_col_1"],
         ),
         expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=1,
         read_kwargs_provider=None,
         drop_duplicates=True,
+        is_inplace=False,
         skip_enabled_compact_partition_drivers=None,
     ),
+    "13-incremental-pkstr-skexists-isinplacecompacted": IncrementalCompactionTestCaseParams(
+        primary_keys={"pk_col_1"},
+        sort_keys=[SortKey.of(key_name="sk_col_1")],
+        partition_keys=[PartitionKey.of("region_id", PartitionKeyType.INT)],
+        partition_values=["1"],
+        input_deltas=pa.Table.from_arrays(
+            [
+                pa.array([str(i) for i in range(10)]),
+                pa.array([i for i in range(10)]),
+            ],
+            names=["pk_col_1", "sk_col_1"],
+        ),
+        input_deltas_delta_type=DeltaType.UPSERT,
+        expected_terminal_compact_partition_result=pa.Table.from_arrays(
+            [
+                pa.array([str(i) for i in range(10)]),
+                pa.array([i for i in range(10)]),
+            ],
+            names=["pk_col_1", "sk_col_1"],
+        ),
+        expected_terminal_exception=None,
+        expected_terminal_exception_message=None,
+        do_create_placement_group=False,
+        records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
+        hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
+        read_kwargs_provider=None,
+        drop_duplicates=True,
+        is_inplace=True,
+        skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
+    ),
 }
 
 INCREMENTAL_TEST_CASES = with_compactor_version_func_test_param(INCREMENTAL_TEST_CASES)
```

### Comparing `deltacat-1.1.4/deltacat/tests/compute/compactor/steps/test_repartition.py` & `deltacat-1.1.5/deltacat/tests/compute/compactor/steps/test_repartition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/compute/compactor/utils/test_io.py` & `deltacat-1.1.5/deltacat/tests/compute/compactor/utils/test_io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/compute/compactor_v2/test_compaction_session.py` & `deltacat-1.1.5/deltacat/tests/compute/compactor_v2/test_compaction_session.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/compute/compactor_v2/utils/test_task_options.py` & `deltacat-1.1.5/deltacat/tests/compute/compactor_v2/utils/test_task_options.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/compute/test_compact_partition_incremental.py` & `deltacat-1.1.5/deltacat/tests/compute/test_compact_partition_incremental.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     INCREMENTAL_TEST_CASES,
 )
 from deltacat.tests.compute.test_util_constant import (
     TEST_S3_RCF_BUCKET_NAME,
     DEFAULT_NUM_WORKERS,
     DEFAULT_WORKER_INSTANCE_CPUS,
 )
+from deltacat.compute.compactor import (
+    RoundCompletionInfo,
+)
 
 DATABASE_FILE_PATH_KEY, DATABASE_FILE_PATH_VALUE = (
     "db_file_path",
     "deltacat/tests/local_deltacat_storage/db_test.sqlite",
 )
 
 
@@ -97,100 +100,108 @@
         "sort_keys",
         "partition_keys_param",
         "partition_values_param",
         "input_deltas",
         "input_deltas_delta_type",
         "expected_terminal_compact_partition_result",
         "expected_terminal_exception",
+        "expected_terminal_exception_message",
         "create_placement_group_param",
         "records_per_compacted_file_param",
         "hash_bucket_count_param",
         "read_kwargs_provider_param",
         "drop_duplicates_param",
         "skip_enabled_compact_partition_drivers",
+        "is_inplace",
         "compact_partition_func",
     ],
     [
         (
             test_name,
             primary_keys,
             sort_keys,
             partition_keys_param,
             partition_values_param,
             input_deltas_param,
             input_deltas_delta_type,
             expected_terminal_compact_partition_result,
             expected_terminal_exception,
+            expected_terminal_exception_message,
             create_placement_group_param,
             records_per_compacted_file_param,
             hash_bucket_count_param,
             drop_duplicates_param,
             read_kwargs_provider,
             skip_enabled_compact_partition_drivers,
+            is_inplace,
             compact_partition_func,
         )
         for test_name, (
             primary_keys,
             sort_keys,
             partition_keys_param,
             partition_values_param,
             input_deltas_param,
             input_deltas_delta_type,
             expected_terminal_compact_partition_result,
             expected_terminal_exception,
+            expected_terminal_exception_message,
             create_placement_group_param,
             records_per_compacted_file_param,
             hash_bucket_count_param,
             drop_duplicates_param,
             read_kwargs_provider,
             skip_enabled_compact_partition_drivers,
+            is_inplace,
             compact_partition_func,
         ) in INCREMENTAL_TEST_CASES.items()
     ],
     ids=[test_name for test_name in INCREMENTAL_TEST_CASES],
-    indirect=[],
 )
 def test_compact_partition_incremental(
     setup_s3_resource: ServiceResource,
     offer_local_deltacat_storage_kwargs: Dict[str, Any],
     test_name: str,
     primary_keys: Set[str],
     sort_keys: Dict[str, str],
     partition_keys_param: Optional[Dict[str, str]],
     partition_values_param: str,
     input_deltas: pa.Table,
     input_deltas_delta_type: str,
     expected_terminal_compact_partition_result: pa.Table,
     expected_terminal_exception: BaseException,
+    expected_terminal_exception_message: Optional[str],
     create_placement_group_param: bool,
     records_per_compacted_file_param: int,
     hash_bucket_count_param: int,
     drop_duplicates_param: bool,
     read_kwargs_provider_param: Any,
     skip_enabled_compact_partition_drivers,
+    is_inplace: bool,
     compact_partition_func: Callable,
     benchmark: BenchmarkFixture,
 ):
     import deltacat.tests.local_deltacat_storage as ds
     from deltacat.types.media import ContentType
     from deltacat.storage import (
         DeltaLocator,
+        Partition,
         PartitionLocator,
     )
     from deltacat.compute.compactor.model.compaction_session_audit_info import (
         CompactionSessionAuditInfo,
     )
     from deltacat.compute.compactor.model.compact_partition_params import (
         CompactPartitionParams,
     )
     from deltacat.utils.placement import (
         PlacementGroupManager,
     )
 
-    ds_mock_kwargs = offer_local_deltacat_storage_kwargs
+    ds_mock_kwargs: Dict[str, Any] = offer_local_deltacat_storage_kwargs
 
     # setup
     partition_keys = partition_keys_param
     (
         source_table_stream,
         destination_table_stream,
         _,
@@ -198,28 +209,29 @@
         primary_keys,
         sort_keys,
         partition_keys,
         input_deltas,
         input_deltas_delta_type,
         partition_values_param,
         ds_mock_kwargs,
+        is_inplace,
     )
-    source_partition = ds.get_partition(
+    source_partition: Partition = ds.get_partition(
         source_table_stream.locator,
         partition_values_param,
         **ds_mock_kwargs,
     )
-    destination_partition_locator = PartitionLocator.of(
+    destination_partition_locator: PartitionLocator = PartitionLocator.of(
         destination_table_stream.locator,
         partition_values_param,
         None,
     )
     num_workers, worker_instance_cpu = DEFAULT_NUM_WORKERS, DEFAULT_WORKER_INSTANCE_CPUS
-    total_cpus = num_workers * worker_instance_cpu
-    pgm = None
+    total_cpus: int = num_workers * worker_instance_cpu
+    pgm: Optional[PlacementGroupManager] = None
     if create_placement_group_param:
         pgm = PlacementGroupManager(
             1, total_cpus, worker_instance_cpu, memory_per_bundle=4000000
         ).pgs[0]
     compact_partition_params = CompactPartitionParams.of(
         {
             "compaction_artifact_s3_bucket": TEST_S3_RCF_BUCKET_NAME,
@@ -256,36 +268,38 @@
         setup_s3_resource.Bucket(TEST_S3_RCF_BUCKET_NAME).objects.all().delete()
         return (compact_partition_params,), {}
 
     rcf_file_s3_uri = benchmark.pedantic(
         compact_partition_func, setup=_incremental_compaction_setup
     )
     # validate
-    round_completion_info = get_rcf(setup_s3_resource, rcf_file_s3_uri)
+    round_completion_info: RoundCompletionInfo = get_rcf(
+        setup_s3_resource, rcf_file_s3_uri
+    )
     compacted_delta_locator: DeltaLocator = (
         round_completion_info.compacted_delta_locator
     )
     audit_bucket, audit_key = round_completion_info.compaction_audit_url.replace(
         "s3://", ""
     ).split("/", 1)
-    compaction_audit_obj: dict = read_s3_contents(
+    compaction_audit_obj: Dict[str, Any] = read_s3_contents(
         setup_s3_resource, audit_bucket, audit_key
     )
     compaction_audit: CompactionSessionAuditInfo = CompactionSessionAuditInfo(
         **compaction_audit_obj
     )
 
     tables = ds.download_delta(
         compacted_delta_locator, storage_type=StorageType.LOCAL, **ds_mock_kwargs
     )
     actual_compacted_table = pa.concat_tables(tables)
     sorting_cols: List[Any] = [(val, "ascending") for val in primary_keys]
     # the compacted table may contain multiple files and chunks
     # and order of records may be incorrect due to multiple files.
-    expected_terminal_compact_partition_result = (
+    expected_terminal_compact_partition_result: pa.Table = (
         expected_terminal_compact_partition_result.combine_chunks().sort_by(
             sorting_cols
         )
     )
     actual_compacted_table = actual_compacted_table.combine_chunks().sort_by(
         sorting_cols
     )
@@ -293,8 +307,19 @@
     assert compaction_audit.input_records == len(
         input_deltas
     ), "The input_records must be equal to total records in the input"
 
     assert actual_compacted_table.equals(
         expected_terminal_compact_partition_result
     ), f"{actual_compacted_table} does not match {expected_terminal_compact_partition_result}"
+
+    if is_inplace:
+        assert (
+            source_partition.locator.partition_values
+            == destination_partition_locator.partition_values
+            and source_partition.locator.stream_id
+            == destination_partition_locator.stream_id
+        ), "The source partition should match the destination partition"
+        assert (
+            compacted_delta_locator.stream_id == source_partition.locator.stream_id
+        ), "The compacted delta should be in the same stream as the source"
     return
```

### Comparing `deltacat-1.1.4/deltacat/tests/compute/test_compact_partition_params.py` & `deltacat-1.1.5/deltacat/tests/compute/test_compact_partition_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py` & `deltacat-1.1.5/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
         "sort_keys",
         "partition_keys_param",
         "partition_values_param",
         "input_deltas_param",
         "input_deltas_delta_type",
         "expected_terminal_compact_partition_result",
         "expected_terminal_exception",
+        "expected_terminal_exception_message",
         "create_placement_group_param",
         "records_per_compacted_file_param",
         "hash_bucket_count_param",
         "read_kwargs_provider_param",
         "drop_duplicates_param",
         "skip_enabled_compact_partition_drivers",
         "incremental_deltas",
@@ -132,14 +133,15 @@
             sort_keys,
             partition_keys_param,
             partition_values_param,
             input_deltas,
             input_deltas_delta_type,
             expected_terminal_compact_partition_result,
             expected_terminal_exception,
+            expected_terminal_exception_message,
             create_placement_group_param,
             records_per_compacted_file_param,
             hash_bucket_count_param,
             drop_duplicates_param,
             read_kwargs_provider,
             skip_enabled_compact_partition_drivers,
             incremental_deltas,
@@ -151,14 +153,15 @@
             sort_keys,
             partition_keys_param,
             partition_values_param,
             input_deltas,
             input_deltas_delta_type,
             expected_terminal_compact_partition_result,
             expected_terminal_exception,
+            expected_terminal_exception_message,
             create_placement_group_param,
             records_per_compacted_file_param,
             hash_bucket_count_param,
             drop_duplicates_param,
             read_kwargs_provider,
             skip_enabled_compact_partition_drivers,
             incremental_deltas,
@@ -176,14 +179,15 @@
     sort_keys: List[Optional[Any]],
     partition_keys_param: Optional[List[Any]],
     partition_values_param: List[Optional[str]],
     input_deltas_param: List[pa.Array],
     input_deltas_delta_type: str,
     expected_terminal_compact_partition_result: pa.Table,
     expected_terminal_exception: BaseException,
+    expected_terminal_exception_message: Optional[str],
     create_placement_group_param: bool,
     records_per_compacted_file_param: int,
     hash_bucket_count_param: int,
     drop_duplicates_param: bool,
     read_kwargs_provider_param: Any,
     incremental_deltas: List[Tuple[pa.Table, DeltaType, Optional[Dict[str, str]]]],
     rebase_expected_compact_partition_result: pa.Table,
@@ -333,16 +337,17 @@
             "records_per_compacted_file": records_per_compacted_file_param,
             "s3_client_kwargs": {},
             "source_partition_locator": source_partition_locator_w_deltas,
             "sort_keys": sort_keys if sort_keys else None,
         }
     )
     if expected_terminal_exception:
-        with pytest.raises(expected_terminal_exception):
+        with pytest.raises(expected_terminal_exception) as exc_info:
             compact_partition_func(compact_partition_params)
+        assert expected_terminal_exception_message in str(exc_info.value)
         return
     rcf_file_s3_uri = compact_partition_func(compact_partition_params)
     round_completion_info = get_rcf(setup_s3_resource, rcf_file_s3_uri)
     compacted_delta_locator_incremental: DeltaLocator = (
         round_completion_info.compacted_delta_locator
     )
     audit_bucket, audit_key = round_completion_info.compaction_audit_url.replace(
```

### Comparing `deltacat-1.1.4/deltacat/tests/compute/test_util_common.py` & `deltacat-1.1.5/deltacat/tests/compute/test_util_common.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,17 @@
     BASE_TEST_DESTINATION_NAMESPACE,
     BASE_TEST_DESTINATION_TABLE_NAME,
     BASE_TEST_DESTINATION_TABLE_VERSION,
     REBASING_NAMESPACE,
     REBASING_TABLE_NAME,
     REBASING_TABLE_VERSION,
 )
+from deltacat.compute.compactor import (
+    RoundCompletionInfo,
+)
 
 
 class PartitionKeyType(str, Enum):
     INT = "int"
     STRING = "string"
     TIMESTAMP = "timestamp"
 
@@ -130,19 +133,16 @@
         primary_keys,
         sort_keys,
         partition_keys,
         ds_mock_kwargs,
     )
 
 
-def get_rcf(s3_resource, rcf_file_s3_uri: str):
+def get_rcf(s3_resource, rcf_file_s3_uri: str) -> RoundCompletionInfo:
     from deltacat.tests.test_utils.utils import read_s3_contents
-    from deltacat.compute.compactor import (
-        RoundCompletionInfo,
-    )
 
     _, rcf_object_key = rcf_file_s3_uri.rsplit("/", 1)
     rcf_file_output: Dict[str, Any] = read_s3_contents(
         s3_resource, TEST_S3_RCF_BUCKET_NAME, rcf_object_key
     )
     return RoundCompletionInfo(**rcf_file_output)
```

### Comparing `deltacat-1.1.4/deltacat/tests/compute/test_util_constant.py` & `deltacat-1.1.5/deltacat/tests/compute/test_util_constant.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/compute/test_util_create_table_deltas_repo.py` & `deltacat-1.1.5/deltacat/tests/compute/test_util_create_table_deltas_repo.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     primary_keys: Set[str],
     sort_keys: Optional[List[Any]],
     partition_keys: Optional[List[PartitionKey]],
     input_deltas: pa.Table,
     input_delta_type: DeltaType,
     partition_values: Optional[List[Any]],
     ds_mock_kwargs: Optional[Dict[str, Any]],
+    simulate_is_inplace: bool = False,
 ) -> Tuple[Stream, Stream, Optional[Stream]]:
     import deltacat.tests.local_deltacat_storage as ds
 
     source_namespace, source_table_name, source_table_version = create_src_table(
         primary_keys, sort_keys, partition_keys, ds_mock_kwargs
     )
 
@@ -109,21 +110,31 @@
     ds.commit_partition(staged_partition, **ds_mock_kwargs)
     source_table_stream_after_committed: Stream = ds.get_stream(
         namespace=source_namespace,
         table_name=source_table_name,
         table_version=source_table_version,
         **ds_mock_kwargs,
     )
-    (
-        destination_table_namespace,
-        destination_table_name,
-        destination_table_version,
-    ) = create_destination_table(
-        primary_keys, sort_keys, partition_keys, ds_mock_kwargs
-    )
+    destination_table_namespace: Optional[str] = None
+    destination_table_name: Optional[str] = None
+    destination_table_version: Optional[str] = None
+    if not simulate_is_inplace:
+        (
+            destination_table_namespace,
+            destination_table_name,
+            destination_table_version,
+        ) = create_destination_table(
+            primary_keys, sort_keys, partition_keys, ds_mock_kwargs
+        )
+    else:
+        # not creating a table as in-place
+        destination_table_namespace = source_namespace
+        destination_table_name = source_table_name
+        destination_table_version = source_table_version
+
     destination_table_stream: Stream = ds.get_stream(
         namespace=destination_table_namespace,
         table_name=destination_table_name,
         table_version=destination_table_version,
         **ds_mock_kwargs,
     )
     return source_table_stream_after_committed, destination_table_stream, None
```

### Comparing `deltacat-1.1.4/deltacat/tests/io/test_cloudpickle_bug_fix.py` & `deltacat-1.1.5/deltacat/tests/io/test_cloudpickle_bug_fix.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/io/test_file_object_store.py` & `deltacat-1.1.5/deltacat/tests/io/test_file_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/io/test_memcached_object_store.py` & `deltacat-1.1.5/deltacat/tests/io/test_memcached_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/io/test_ray_plasma_object_store.py` & `deltacat-1.1.5/deltacat/tests/io/test_ray_plasma_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/io/test_redis_object_store.py` & `deltacat-1.1.5/deltacat/tests/io/test_redis_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/io/test_s3_object_store.py` & `deltacat-1.1.5/deltacat/tests/io/test_s3_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/local_deltacat_storage/__init__.py` & `deltacat-1.1.5/deltacat/tests/local_deltacat_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/stats/test_intervals.py` & `deltacat-1.1.5/deltacat/tests/stats/test_intervals.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/test_logs.py` & `deltacat-1.1.5/deltacat/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/test_utils/pyarrow.py` & `deltacat-1.1.5/deltacat/tests/test_utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/test_utils/storage.py` & `deltacat-1.1.5/deltacat/tests/test_utils/storage.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/utils/test_cloudpickle.py` & `deltacat-1.1.5/deltacat/tests/utils/test_cloudpickle.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/utils/test_daft.py` & `deltacat-1.1.5/deltacat/tests/utils/test_daft.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/utils/test_metrics.py` & `deltacat-1.1.5/deltacat/tests/utils/test_metrics.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/utils/test_placement.py` & `deltacat-1.1.5/deltacat/tests/utils/test_placement.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/utils/test_pyarrow.py` & `deltacat-1.1.5/deltacat/tests/utils/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/utils/test_record_batch_tables.py` & `deltacat-1.1.5/deltacat/tests/utils/test_record_batch_tables.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/tests/utils/test_resources.py` & `deltacat-1.1.5/deltacat/tests/utils/test_resources.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/types/media.py` & `deltacat-1.1.5/deltacat/types/media.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/types/partial_download.py` & `deltacat-1.1.5/deltacat/types/partial_download.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/types/tables.py` & `deltacat-1.1.5/deltacat/types/tables.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/arguments.py` & `deltacat-1.1.5/deltacat/utils/arguments.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/cloudpickle.py` & `deltacat-1.1.5/deltacat/utils/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/common.py` & `deltacat-1.1.5/deltacat/utils/common.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/daft.py` & `deltacat-1.1.5/deltacat/utils/daft.py`

 * *Files 3% similar despite different names*

```diff
@@ -159,9 +159,11 @@
             key_id=s3_client_kwargs.get("aws_access_key_id"),
             access_key=s3_client_kwargs.get("aws_secret_access_key"),
             session_token=s3_client_kwargs.get("aws_session_token"),
             region_name=AWS_REGION,
             retry_mode="adaptive",
             num_tries=BOTO_MAX_RETRIES,
             max_connections=DAFT_MAX_S3_CONNECTIONS_PER_FILE,
+            connect_timeout_ms=5_000,  # Timeout to connect to server
+            read_timeout_ms=10_000,  # Timeout for first byte from server
         )
     )
```

### Comparing `deltacat-1.1.4/deltacat/utils/metrics.py` & `deltacat-1.1.5/deltacat/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/numpy.py` & `deltacat-1.1.5/deltacat/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/pandas.py` & `deltacat-1.1.5/deltacat/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/performance.py` & `deltacat-1.1.5/deltacat/utils/performance.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/placement.py` & `deltacat-1.1.5/deltacat/utils/placement.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/pyarrow.py` & `deltacat-1.1.5/deltacat/utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/ray_utils/collections.py` & `deltacat-1.1.5/deltacat/utils/ray_utils/collections.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/ray_utils/concurrency.py` & `deltacat-1.1.5/deltacat/utils/ray_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/ray_utils/dataset.py` & `deltacat-1.1.5/deltacat/utils/ray_utils/dataset.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/ray_utils/runtime.py` & `deltacat-1.1.5/deltacat/utils/ray_utils/runtime.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/resources.py` & `deltacat-1.1.5/deltacat/utils/resources.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/s3fs.py` & `deltacat-1.1.5/deltacat/utils/s3fs.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat/utils/schema.py` & `deltacat-1.1.5/deltacat/utils/schema.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/deltacat.egg-info/PKG-INFO` & `deltacat-1.1.5/deltacat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltacat
-Version: 1.1.4
+Version: 1.1.5
 Summary: A scalable, fast, ACID-compliant Data Catalog powered by Ray.
 Home-page: https://github.com/ray-project/deltacat
 Author: Ray Team
 License: UNKNOWN
 Description: # DeltaCAT
         
         DeltaCAT is a Pythonic Data Catalog powered by Ray.
```

### Comparing `deltacat-1.1.4/deltacat.egg-info/SOURCES.txt` & `deltacat-1.1.5/deltacat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.4/setup.py` & `deltacat-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         "pydantic == 1.10.4",
         "ray[default] ~= 2.0",
         "s3fs == 2022.2.0",
         "tenacity == 8.1.0",
         "typing-extensions == 4.4.0",
         "pymemcache == 4.0.0",
         "redis == 4.6.0",
-        "getdaft == 0.2.17",
+        "getdaft == 0.2.23",
         "schedule == 1.2.0",
     ],
     setup_requires=["wheel"],
     package_data={
         "compute/metastats": ["*.yaml"],
     },
     classifiers=[
```

