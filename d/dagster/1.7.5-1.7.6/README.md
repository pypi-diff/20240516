# Comparing `tmp/dagster-1.7.5.tar.gz` & `tmp/dagster-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-1.7.5.tar", last modified: Thu May  9 17:47:59 2024, max compression
+gzip compressed data, was "dagster-1.7.6.tar", last modified: Thu May 16 19:27:38 2024, max compression
```

## Comparing `dagster-1.7.5.tar` & `dagster-1.7.6.tar`

### file list

```diff
@@ -1,714 +1,721 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.447741 dagster-1.7.5/
--rw-r--r--   0 root         (0) root         (0)      553 2024-05-09 17:47:35.000000 dagster-1.7.5/COPYING
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-09 17:47:35.000000 dagster-1.7.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)      533 2024-05-09 17:47:35.000000 dagster-1.7.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     8928 2024-05-09 17:47:59.447741 dagster-1.7.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7214 2024-05-09 17:47:35.000000 dagster-1.7.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.367741 dagster-1.7.5/dagster/
--rw-r--r--   0 root         (0) root         (0)    30128 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/__init__.py
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/__main__.py
--rw-r--r--   0 root         (0) root         (0)    20744 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_annotations.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.371741 dagster-1.7.5/dagster/_api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      731 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/get_server_id.py
--rw-r--r--   0 root         (0) root         (0)     2147 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/list_repositories.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/notebook_data.py
--rw-r--r--   0 root         (0) root         (0)     3224 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/snapshot_execution_plan.py
--rw-r--r--   0 root         (0) root         (0)     1964 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/snapshot_job.py
--rw-r--r--   0 root         (0) root         (0)     5483 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/snapshot_partition.py
--rw-r--r--   0 root         (0) root         (0)     1670 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/snapshot_repository.py
--rw-r--r--   0 root         (0) root         (0)     3021 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/snapshot_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3370 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_api/snapshot_sensor.py
--rw-r--r--   0 root         (0) root         (0)      478 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_builtins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.371741 dagster-1.7.5/dagster/_check/
--rw-r--r--   0 root         (0) root         (0)     1352 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_check/README.md
--rw-r--r--   0 root         (0) root         (0)    52040 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_check/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.371741 dagster-1.7.5/dagster/_cli/
--rw-r--r--   0 root         (0) root         (0)     1182 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26898 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/api.py
--rw-r--r--   0 root         (0) root         (0)     8271 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/asset.py
--rw-r--r--   0 root         (0) root         (0)     8302 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/code_server.py
--rw-r--r--   0 root         (0) root         (0)     2374 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/config_scaffolder.py
--rw-r--r--   0 root         (0) root         (0)     3513 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/debug.py
--rw-r--r--   0 root         (0) root         (0)     8134 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/dev.py
--rw-r--r--   0 root         (0) root         (0)     6651 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/instance.py
--rw-r--r--   0 root         (0) root         (0)    30542 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/job.py
--rw-r--r--   0 root         (0) root         (0)     1695 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/load_handle.py
--rw-r--r--   0 root         (0) root         (0)     9114 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/project.py
--rw-r--r--   0 root         (0) root         (0)     5120 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/run.py
--rw-r--r--   0 root         (0) root         (0)    19351 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/schedule.py
--rw-r--r--   0 root         (0) root         (0)    15461 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/sensor.py
--rw-r--r--   0 root         (0) root         (0)     4259 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.371741 dagster-1.7.5/dagster/_cli/workspace/
--rw-r--r--   0 root         (0) root         (0)      180 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27910 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_cli/workspace/cli_target.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.375741 dagster-1.7.5/dagster/_config/
--rw-r--r--   0 root         (0) root         (0)     3186 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3403 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    15830 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/config_type.py
--rw-r--r--   0 root         (0) root         (0)    18787 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/errors.py
--rw-r--r--   0 root         (0) root         (0)     1783 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/evaluate_value_result.py
--rw-r--r--   0 root         (0) root         (0)    14918 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/field.py
--rw-r--r--   0 root         (0) root         (0)    19728 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/field_utils.py
--rw-r--r--   0 root         (0) root         (0)     9536 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/post_process.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/primitive_mapping.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.375741 dagster-1.7.5/dagster/_config/pythonic_config/
--rw-r--r--   0 root         (0) root         (0)     1394 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1641 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/attach_other_object_to_context.py
--rw-r--r--   0 root         (0) root         (0)    18114 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/config.py
--rw-r--r--   0 root         (0) root         (0)    11510 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)    11583 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    41265 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/resource.py
--rw-r--r--   0 root         (0) root         (0)     1996 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/type_check_utils.py
--rw-r--r--   0 root         (0) root         (0)     8375 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/pythonic_config/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)    12532 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/snap.py
--rw-r--r--   0 root         (0) root         (0)     3087 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/source.py
--rw-r--r--   0 root         (0) root         (0)     3528 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/stack.py
--rw-r--r--   0 root         (0) root         (0)     7772 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/traversal_context.py
--rw-r--r--   0 root         (0) root         (0)     4167 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/type_printer.py
--rw-r--r--   0 root         (0) root         (0)    17137 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_config/validate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.379741 dagster-1.7.5/dagster/_core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.379741 dagster-1.7.5/dagster/_core/asset_graph_view/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/asset_graph_view/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22976 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/asset_graph_view/asset_graph_view.py
--rw-r--r--   0 root         (0) root         (0)      994 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/assets.py
--rw-r--r--   0 root         (0) root         (0)    13427 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/code_pointer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.379741 dagster-1.7.5/dagster/_core/container_context/
--rw-r--r--   0 root         (0) root         (0)      184 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/container_context/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/container_context/config.py
--rw-r--r--   0 root         (0) root         (0)     2310 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/debug.py
--rw-r--r--   0 root         (0) root         (0)     9665 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/decorator_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.391741 dagster-1.7.5/dagster/_core/definitions/
--rw-r--r--   0 root         (0) root         (0)     7873 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4506 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_evaluation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.391741 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.391741 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/freshness_checks/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/freshness_checks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12253 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/freshness_checks/last_update.py
--rw-r--r--   0 root         (0) root         (0)     7692 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py
--rw-r--r--   0 root         (0) root         (0)     9763 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py
--rw-r--r--   0 root         (0) root         (0)     6122 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/schema_change_checks.py
--rw-r--r--   0 root         (0) root         (0)    11378 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_factories/utils.py
--rw-r--r--   0 root         (0) root         (0)     7090 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_result.py
--rw-r--r--   0 root         (0) root         (0)     5628 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_check_spec.py
--rw-r--r--   0 root         (0) root         (0)     6113 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_checks.py
--rw-r--r--   0 root         (0) root         (0)    28490 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_daemon_context.py
--rw-r--r--   0 root         (0) root         (0)    10831 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)     4628 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_dep.py
--rw-r--r--   0 root         (0) root         (0)    10133 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)     7696 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_graph_differ.py
--rw-r--r--   0 root         (0) root         (0)    16636 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_graph_subset.py
--rw-r--r--   0 root         (0) root         (0)     3644 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_in.py
--rw-r--r--   0 root         (0) root         (0)    30136 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_job.py
--rw-r--r--   0 root         (0) root         (0)     5897 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_key.py
--rw-r--r--   0 root         (0) root         (0)    30355 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_layer.py
--rw-r--r--   0 root         (0) root         (0)     6937 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_out.py
--rw-r--r--   0 root         (0) root         (0)    39535 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_selection.py
--rw-r--r--   0 root         (0) root         (0)     7444 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     6756 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_spec.py
--rw-r--r--   0 root         (0) root         (0)    10965 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/asset_subset.py
--rw-r--r--   0 root         (0) root         (0)    79051 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/assets.py
--rw-r--r--   0 root         (0) root         (0)    13969 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    11580 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/auto_materialize_rule.py
--rw-r--r--   0 root         (0) root         (0)    21722 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/auto_materialize_rule_evaluation.py
--rw-r--r--   0 root         (0) root         (0)    50726 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/auto_materialize_rule_impls.py
--rw-r--r--   0 root         (0) root         (0)     2768 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/auto_materialize_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)     2939 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/backfill_policy.py
--rw-r--r--   0 root         (0) root         (0)    34599 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/base_asset_graph.py
--rw-r--r--   0 root         (0) root         (0)    16772 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/cacheable_assets.py
--rw-r--r--   0 root         (0) root         (0)    40623 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/composition.py
--rw-r--r--   0 root         (0) root         (0)     4278 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/config.py
--rw-r--r--   0 root         (0) root         (0)    14811 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/configurable.py
--rw-r--r--   0 root         (0) root         (0)    22990 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/data_time.py
--rw-r--r--   0 root         (0) root         (0)    30236 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/data_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.395741 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/
--rw-r--r--   0 root         (0) root         (0)     1348 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/README.md
--rw-r--r--   0 root         (0) root         (0)      956 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.395741 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/legacy/
--rw-r--r--   0 root         (0) root         (0)       59 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/legacy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2771 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py
--rw-r--r--   0 root         (0) root         (0)    16841 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/legacy/rule_condition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.395741 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operands/
--rw-r--r--   0 root         (0) root         (0)      325 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2450 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operands/slice_conditions.py
--rw-r--r--   0 root         (0) root         (0)     2196 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operands/updated_since_cron_condition.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.395741 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operators/
--rw-r--r--   0 root         (0) root         (0)      280 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3163 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operators/boolean_operators.py
--rw-r--r--   0 root         (0) root         (0)     3592 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operators/dep_operators.py
--rw-r--r--   0 root         (0) root         (0)     7206 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/scheduling_condition.py
--rw-r--r--   0 root         (0) root         (0)     6430 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/scheduling_context.py
--rw-r--r--   0 root         (0) root         (0)     3620 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/scheduling_evaluation_info.py
--rw-r--r--   0 root         (0) root         (0)    10067 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/serialized_objects.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.395741 dagster-1.7.5/dagster/_core/definitions/decorators/
--rw-r--r--   0 root         (0) root         (0)      620 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16572 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/asset_check_decorator.py
--rw-r--r--   0 root         (0) root         (0)    70075 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4907 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/config_mapping_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9077 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/graph_decorator.py
--rw-r--r--   0 root         (0) root         (0)     9353 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/hook_decorator.py
--rw-r--r--   0 root         (0) root         (0)    10815 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/job_decorator.py
--rw-r--r--   0 root         (0) root         (0)    19011 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/op_decorator.py
--rw-r--r--   0 root         (0) root         (0)    15668 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/repository_decorator.py
--rw-r--r--   0 root         (0) root         (0)     8718 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/schedule_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12463 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/sensor_decorator.py
--rw-r--r--   0 root         (0) root         (0)    12656 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/decorators/source_asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     5267 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/definition_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    23545 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/definitions_class.py
--rw-r--r--   0 root         (0) root         (0)    42243 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/dependency.py
--rw-r--r--   0 root         (0) root         (0)    27649 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/events.py
--rw-r--r--   0 root         (0) root         (0)    21182 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/executor_definition.py
--rw-r--r--   0 root         (0) root         (0)     9379 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/external_asset.py
--rw-r--r--   0 root         (0) root         (0)     9808 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/freshness_based_auto_materialize.py
--rw-r--r--   0 root         (0) root         (0)     8801 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    16401 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/freshness_policy_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    47569 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/graph_definition.py
--rw-r--r--   0 root         (0) root         (0)     6546 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/hook_definition.py
--rw-r--r--   0 root         (0) root         (0)     1524 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/hook_invocation.py
--rw-r--r--   0 root         (0) root         (0)     3537 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/inference.py
--rw-r--r--   0 root         (0) root         (0)    21027 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/input.py
--rw-r--r--   0 root         (0) root         (0)     6410 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/instigation_logger.py
--rw-r--r--   0 root         (0) root         (0)     2991 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/job_base.py
--rw-r--r--   0 root         (0) root         (0)    53689 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/job_definition.py
--rw-r--r--   0 root         (0) root         (0)     5693 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/load_asset_checks_from_modules.py
--rw-r--r--   0 root         (0) root         (0)    22306 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/load_assets_from_modules.py
--rw-r--r--   0 root         (0) root         (0)     7171 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/logger_definition.py
--rw-r--r--   0 root         (0) root         (0)      636 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/logger_invocation.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/materialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.395741 dagster-1.7.5/dagster/_core/definitions/metadata/
--rw-r--r--   0 root         (0) root         (0)     9602 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/metadata/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5591 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/metadata/metadata_set.py
--rw-r--r--   0 root         (0) root         (0)    31381 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/metadata/metadata_value.py
--rw-r--r--   0 root         (0) root         (0)    12452 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/metadata/table.py
--rw-r--r--   0 root         (0) root         (0)    57203 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/multi_asset_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    22029 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/multi_dimensional_partitions.py
--rw-r--r--   0 root         (0) root         (0)      197 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/no_step_launcher.py
--rw-r--r--   0 root         (0) root         (0)    11892 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/node_container.py
--rw-r--r--   0 root         (0) root         (0)     8016 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/node_definition.py
--rw-r--r--   0 root         (0) root         (0)     2892 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/observe.py
--rw-r--r--   0 root         (0) root         (0)    23078 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/op_definition.py
--rw-r--r--   0 root         (0) root         (0)    23141 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/op_invocation.py
--rw-r--r--   0 root         (0) root         (0)     7551 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/op_selection.py
--rw-r--r--   0 root         (0) root         (0)    19237 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/output.py
--rw-r--r--   0 root         (0) root         (0)    50520 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/partition.py
--rw-r--r--   0 root         (0) root         (0)      630 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/partition_key_range.py
--rw-r--r--   0 root         (0) root         (0)    47665 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)    11087 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/partitioned_schedule.py
--rw-r--r--   0 root         (0) root         (0)     3779 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/policy.py
--rw-r--r--   0 root         (0) root         (0)    27690 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/reconstruct.py
--rw-r--r--   0 root         (0) root         (0)    21602 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/remote_asset_graph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.399741 dagster-1.7.5/dagster/_core/definitions/repository_definition/
--rw-r--r--   0 root         (0) root         (0)      654 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/repository_definition/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6024 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/repository_definition/caching_index.py
--rw-r--r--   0 root         (0) root         (0)    21698 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/repository_definition/repository_data.py
--rw-r--r--   0 root         (0) root         (0)    20892 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/repository_definition/repository_data_builder.py
--rw-r--r--   0 root         (0) root         (0)    20432 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/repository_definition/repository_definition.py
--rw-r--r--   0 root         (0) root         (0)     1479 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/repository_definition/valid_definitions.py
--rw-r--r--   0 root         (0) root         (0)     8858 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/resolved_asset_deps.py
--rw-r--r--   0 root         (0) root         (0)     1465 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/resource_annotation.py
--rw-r--r--   0 root         (0) root         (0)    17900 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     5382 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/resource_invocation.py
--rw-r--r--   0 root         (0) root         (0)    10320 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/resource_requirement.py
--rw-r--r--   0 root         (0) root         (0)     3875 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/result.py
--rw-r--r--   0 root         (0) root         (0)    23076 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/run_config.py
--rw-r--r--   0 root         (0) root         (0)     1445 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)    19555 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/run_request.py
--rw-r--r--   0 root         (0) root         (0)    45639 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/run_status_sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    39363 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/schedule_definition.py
--rw-r--r--   0 root         (0) root         (0)     5134 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/scoped_resources_builder.py
--rw-r--r--   0 root         (0) root         (0)    14134 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/selector.py
--rw-r--r--   0 root         (0) root         (0)    53797 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/sensor_definition.py
--rw-r--r--   0 root         (0) root         (0)    19236 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/source_asset.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/step_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/target.py
--rw-r--r--   0 root         (0) root         (0)    22389 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/time_window_partition_mapping.py
--rw-r--r--   0 root         (0) root         (0)   102377 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/time_window_partitions.py
--rw-r--r--   0 root         (0) root         (0)    15160 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/unresolved_asset_job_definition.py
--rw-r--r--   0 root         (0) root         (0)    11027 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/utils.py
--rw-r--r--   0 root         (0) root         (0)     3982 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/definitions/version_strategy.py
--rw-r--r--   0 root         (0) root         (0)    26986 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/errors.py
--rw-r--r--   0 root         (0) root         (0)    17452 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/event_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.399741 dagster-1.7.5/dagster/_core/events/
--rw-r--r--   0 root         (0) root         (0)    71913 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/events/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8142 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/events/log.py
--rw-r--r--   0 root         (0) root         (0)     1614 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/events/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.403741 dagster-1.7.5/dagster/_core/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38363 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/api.py
--rw-r--r--   0 root         (0) root         (0)    65474 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/asset_backfill.py
--rw-r--r--   0 root         (0) root         (0)    17100 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     6296 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/build_resources.py
--rw-r--r--   0 root         (0) root         (0)      224 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/bulk_actions.py
--rw-r--r--   0 root         (0) root         (0)     5587 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/compute_logs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.403741 dagster-1.7.5/dagster/_core/execution/context/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79687 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/compute.py
--rw-r--r--   0 root         (0) root         (0)     8657 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/data_version_cache.py
--rw-r--r--   0 root         (0) root         (0)    17598 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/hook.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/init.py
--rw-r--r--   0 root         (0) root         (0)    29167 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/input.py
--rw-r--r--   0 root         (0) root         (0)    40124 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/invocation.py
--rw-r--r--   0 root         (0) root         (0)     3164 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/logger.py
--rw-r--r--   0 root         (0) root         (0)    37256 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/output.py
--rw-r--r--   0 root         (0) root         (0)    49252 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context/system.py
--rw-r--r--   0 root         (0) root         (0)    18837 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/context_creation_job.py
--rw-r--r--   0 root         (0) root         (0)     5135 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/execute_in_process.py
--rw-r--r--   0 root         (0) root         (0)     5897 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/execute_in_process_result.py
--rw-r--r--   0 root         (0) root         (0)     9633 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/execution_result.py
--rw-r--r--   0 root         (0) root         (0)     8602 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/host_mode.py
--rw-r--r--   0 root         (0) root         (0)    14247 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/job_backfill.py
--rw-r--r--   0 root         (0) root         (0)     6723 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/job_execution_result.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/memoization.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.407741 dagster-1.7.5/dagster/_core/execution/plan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26460 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/active.py
--rw-r--r--   0 root         (0) root         (0)     9850 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/compute.py
--rw-r--r--   0 root         (0) root         (0)    17062 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/compute_generator.py
--rw-r--r--   0 root         (0) root         (0)    16974 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/execute_plan.py
--rw-r--r--   0 root         (0) root         (0)    40877 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/execute_step.py
--rw-r--r--   0 root         (0) root         (0)    11032 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/external_step.py
--rw-r--r--   0 root         (0) root         (0)     3664 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/handle.py
--rw-r--r--   0 root         (0) root         (0)    39260 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/inputs.py
--rw-r--r--   0 root         (0) root         (0)     6251 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/instance_concurrency_context.py
--rw-r--r--   0 root         (0) root         (0)     1197 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/local_external_step_main.py
--rw-r--r--   0 root         (0) root         (0)     5706 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/objects.py
--rw-r--r--   0 root         (0) root         (0)     7326 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/outputs.py
--rw-r--r--   0 root         (0) root         (0)    61075 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/plan.py
--rw-r--r--   0 root         (0) root         (0)      114 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/resume_retry.py
--rw-r--r--   0 root         (0) root         (0)    17174 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/state.py
--rw-r--r--   0 root         (0) root         (0)    15985 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/step.py
--rw-r--r--   0 root         (0) root         (0)     3796 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/plan/utils.py
--rw-r--r--   0 root         (0) root         (0)     1762 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/poll_compute_logs.py
--rw-r--r--   0 root         (0) root         (0)     8230 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/resolve_versions.py
--rw-r--r--   0 root         (0) root         (0)    19141 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/resources_init.py
--rw-r--r--   0 root         (0) root         (0)     2100 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/retries.py
--rw-r--r--   0 root         (0) root         (0)     1564 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/run_cancellation_thread.py
--rw-r--r--   0 root         (0) root         (0)     9950 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/stats.py
--rw-r--r--   0 root         (0) root         (0)    15211 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/submit_asset_runs.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/tags.py
--rw-r--r--   0 root         (0) root         (0)     1172 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/validate_run_config.py
--rw-r--r--   0 root         (0) root         (0)     1282 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/watch_orphans.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/execution/with_resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.407741 dagster-1.7.5/dagster/_core/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/base.py
--rw-r--r--   0 root         (0) root         (0)     5989 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/child_process_executor.py
--rw-r--r--   0 root         (0) root         (0)     3366 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/in_process.py
--rw-r--r--   0 root         (0) root         (0)     1509 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/init.py
--rw-r--r--   0 root         (0) root         (0)    15497 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/multiprocess.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.407741 dagster-1.7.5/dagster/_core/executor/step_delegating/
--rw-r--r--   0 root         (0) root         (0)      247 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/step_delegating/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16894 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/step_delegating/step_delegating_executor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.407741 dagster-1.7.5/dagster/_core/executor/step_delegating/step_handler/
--rw-r--r--   0 root         (0) root         (0)      152 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/step_delegating/step_handler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3078 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/executor/step_delegating/step_handler/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/instance/
--rw-r--r--   0 root         (0) root         (0)   132334 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/instance/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15788 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/instance/config.py
--rw-r--r--   0 root         (0) root         (0)    24141 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/instance/ref.py
--rw-r--r--   0 root         (0) root         (0)     3899 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/instance_for_test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/launcher/
--rw-r--r--   0 root         (0) root         (0)      297 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3819 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/launcher/base.py
--rw-r--r--   0 root         (0) root         (0)     6645 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/launcher/default_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1566 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/launcher/sync_in_memory_run_launcher.py
--rw-r--r--   0 root         (0) root         (0)      473 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/libraries.py
--rw-r--r--   0 root         (0) root         (0)    18041 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/nux.py
--rw-r--r--   0 root         (0) root         (0)     6656 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/op_concurrency_limits_counter.py
--rw-r--r--   0 root         (0) root         (0)     3691 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/origin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/pipes/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/pipes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8974 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/pipes/client.py
--rw-r--r--   0 root         (0) root         (0)    18318 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/pipes/context.py
--rw-r--r--   0 root         (0) root         (0)     5648 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/pipes/subprocess.py
--rw-r--r--   0 root         (0) root         (0)    25661 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/pipes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/remote_representation/
--rw-r--r--   0 root         (0) root         (0)     2793 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36695 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/code_location.py
--rw-r--r--   0 root         (0) root         (0)    37482 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/external.py
--rw-r--r--   0 root         (0) root         (0)    83582 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/external_data.py
--rw-r--r--   0 root         (0) root         (0)     1450 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/feature_flags.py
--rw-r--r--   0 root         (0) root         (0)    12429 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/grpc_server_registry.py
--rw-r--r--   0 root         (0) root         (0)     1487 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/grpc_server_state_subscriber.py
--rw-r--r--   0 root         (0) root         (0)     4356 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/handle.py
--rw-r--r--   0 root         (0) root         (0)     1581 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/historical.py
--rw-r--r--   0 root         (0) root         (0)     4850 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/job_index.py
--rw-r--r--   0 root         (0) root         (0)    19669 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/origin.py
--rw-r--r--   0 root         (0) root         (0)     3602 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/remote_representation/represented.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      267 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2005 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/run_coordinator/base.py
--rw-r--r--   0 root         (0) root         (0)     1922 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/run_coordinator/default_run_coordinator.py
--rw-r--r--   0 root         (0) root         (0)    13364 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/run_coordinator/queued_run_coordinator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/scheduler/
--rw-r--r--   0 root         (0) root         (0)      534 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1241 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/scheduler/execution.py
--rw-r--r--   0 root         (0) root         (0)    28819 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/scheduler/instigation.py
--rw-r--r--   0 root         (0) root         (0)    10917 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/scheduler/scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/secrets/
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1801 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/secrets/env_file.py
--rw-r--r--   0 root         (0) root         (0)      388 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.411741 dagster-1.7.5/dagster/_core/selector/
--rw-r--r--   0 root         (0) root         (0)      295 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/selector/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18109 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/selector/subset_selector.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.415741 dagster-1.7.5/dagster/_core/snap/
--rw-r--r--   0 root         (0) root         (0)     2842 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/__init__.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/config_types.py
--rw-r--r--   0 root         (0) root         (0)     3999 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     9302 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/dep_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    12155 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/execution_plan_snapshot.py
--rw-r--r--   0 root         (0) root         (0)    16934 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/job_snapshot.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/mode.py
--rw-r--r--   0 root         (0) root         (0)    14185 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/node.py
--rw-r--r--   0 root         (0) root         (0)     3183 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/snap/snap_to_yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.419741 dagster-1.7.5/dagster/_core/storage/
--rw-r--r--   0 root         (0) root         (0)     3058 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/DEVELOPING.md
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.419741 dagster-1.7.5/dagster/_core/storage/alembic/
--rw-r--r--   0 root         (0) root         (0)     6686 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/README.md
--rw-r--r--   0 root         (0) root         (0)      687 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      494 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     3150 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/001_initial_1.py
--rw-r--r--   0 root         (0) root         (0)      312 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/001_initial_schedule.py
--rw-r--r--   0 root         (0) root         (0)     1486 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
--rw-r--r--   0 root         (0) root         (0)      599 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
--rw-r--r--   0 root         (0) root         (0)      973 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     2729 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1406 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      953 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      956 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1171 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1730 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1147 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1125 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
--rw-r--r--   0 root         (0) root         (0)     1143 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      435 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
--rw-r--r--   0 root         (0) root         (0)      432 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
--rw-r--r--   0 root         (0) root         (0)     3927 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      409 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      936 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      325 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/017_initial_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1570 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1034 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      531 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
--rw-r--r--   0 root         (0) root         (0)     1275 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      404 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      635 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      434 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
--rw-r--r--   0 root         (0) root         (0)      416 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
--rw-r--r--   0 root         (0) root         (0)     1893 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
--rw-r--r--   0 root         (0) root         (0)      958 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
--rw-r--r--   0 root         (0) root         (0)      499 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
--rw-r--r--   0 root         (0) root         (0)     1951 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
--rw-r--r--   0 root         (0) root         (0)      428 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
--rw-r--r--   0 root         (0) root         (0)      427 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
--rw-r--r--   0 root         (0) root         (0)     1537 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
--rw-r--r--   0 root         (0) root         (0)     2481 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
--rw-r--r--   0 root         (0) root         (0)     1177 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
--rw-r--r--   0 root         (0) root         (0)     2062 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
--rw-r--r--   0 root         (0) root         (0)     2359 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
--rw-r--r--   0 root         (0) root         (0)     2898 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
--rw-r--r--   0 root         (0) root         (0)     1322 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3872 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/asset_check_execution_record.py
--rw-r--r--   0 root         (0) root         (0)     7301 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/asset_value_loader.py
--rw-r--r--   0 root         (0) root         (0)     1227 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/base_storage.py
--rw-r--r--   0 root         (0) root         (0)     3320 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/batch_asset_record_loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/branching/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/branching/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/branching/branching_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8725 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/captured_log_manager.py
--rw-r--r--   0 root         (0) root         (0)    16223 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/cloud_storage_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     9557 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1863 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/config.py
--rw-r--r--   0 root         (0) root         (0)      417 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/daemon_cursor.py
--rw-r--r--   0 root         (0) root         (0)    25652 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/dagster_run.py
--rw-r--r--   0 root         (0) root         (0)    11187 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/db_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/event_log/
--rw-r--r--   0 root         (0) root         (0)      742 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20210 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/base.py
--rw-r--r--   0 root         (0) root         (0)     3801 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     7289 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/migration.py
--rw-r--r--   0 root         (0) root         (0)     8037 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/polling_event_watcher.py
--rw-r--r--   0 root         (0) root         (0)     9250 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/schema.py
--rw-r--r--   0 root         (0) root         (0)   121797 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/sql_event_log.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/event_log/sqlite/
--rw-r--r--   0 root         (0) root         (0)      200 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/event_log/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     7508 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    22497 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
--rw-r--r--   0 root         (0) root         (0)    10983 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/file_manager.py
--rw-r--r--   0 root         (0) root         (0)    13492 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/fs_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     8819 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/input_manager.py
--rw-r--r--   0 root         (0) root         (0)    10882 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/io_manager.py
--rw-r--r--   0 root         (0) root         (0)    32639 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/legacy_storage.py
--rw-r--r--   0 root         (0) root         (0)    17558 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/local_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     1167 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/mem_io_manager.py
--rw-r--r--   0 root         (0) root         (0)     4355 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/memoizable_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/migration/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/migration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5964 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/migration/bigint_migration.py
--rw-r--r--   0 root         (0) root         (0)    15491 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/migration/utils.py
--rw-r--r--   0 root         (0) root         (0)     3270 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/noop_compute_log_manager.py
--rw-r--r--   0 root         (0) root         (0)     2361 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/output_manager.py
--rw-r--r--   0 root         (0) root         (0)    18101 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/partition_status_cache.py
--rw-r--r--   0 root         (0) root         (0)     2121 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/root.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/runs/
--rw-r--r--   0 root         (0) root         (0)      386 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13903 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/base.py
--rw-r--r--   0 root         (0) root         (0)     2452 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/in_memory.py
--rw-r--r--   0 root         (0) root         (0)     8716 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/migration.py
--rw-r--r--   0 root         (0) root         (0)     6391 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/schema.py
--rw-r--r--   0 root         (0) root         (0)    37611 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/sql_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/runs/sqlite/
--rw-r--r--   0 root         (0) root         (0)       69 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/runs/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     6310 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.427741 dagster-1.7.5/dagster/_core/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)      272 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7246 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/base.py
--rw-r--r--   0 root         (0) root         (0)     4133 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/migration.py
--rw-r--r--   0 root         (0) root         (0)     4086 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/schema.py
--rw-r--r--   0 root         (0) root         (0)    25156 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/sql_schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_core/storage/schedules/sqlite/
--rw-r--r--   0 root         (0) root         (0)       84 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/sqlite/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_core/storage/schedules/sqlite/alembic/
--rw-r--r--   0 root         (0) root         (0)      986 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
--rw-r--r--   0 root         (0) root         (0)     3684 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
--rw-r--r--   0 root         (0) root         (0)     7691 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/sql.py
--rw-r--r--   0 root         (0) root         (0)     1391 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/sqlalchemy_compat.py
--rw-r--r--   0 root         (0) root         (0)      926 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/sqlite.py
--rw-r--r--   0 root         (0) root         (0)     4875 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/sqlite_storage.py
--rw-r--r--   0 root         (0) root         (0)     3546 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/tags.py
--rw-r--r--   0 root         (0) root         (0)     1186 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/temp_file_manager.py
--rw-r--r--   0 root         (0) root         (0)    19138 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/storage/upath_io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_core/system_config/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/system_config/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13962 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/system_config/composite_descent.py
--rw-r--r--   0 root         (0) root         (0)    15178 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/system_config/objects.py
--rw-r--r--   0 root         (0) root         (0)    29921 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     4824 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/telemetry_upload.py
--rw-r--r--   0 root         (0) root         (0)    22361 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/test_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_core/types/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3084 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/builtin_config_schemas.py
--rw-r--r--   0 root         (0) root         (0)     7042 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    36504 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)     3571 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/decorator.py
--rw-r--r--   0 root         (0) root         (0)     1846 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/loadable_target_origin.py
--rw-r--r--   0 root         (0) root         (0)     1027 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/primitive_mapping.py
--rw-r--r--   0 root         (0) root         (0)     4764 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/python_dict.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/python_set.py
--rw-r--r--   0 root         (0) root         (0)     3620 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/python_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1772 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/types/transform_typing.py
--rw-r--r--   0 root         (0) root         (0)     1441 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/utility_ops.py
--rw-r--r--   0 root         (0) root         (0)     6652 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_core/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4457 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/autodiscovery.py
--rw-r--r--   0 root         (0) root         (0)     3422 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/config_schema.py
--rw-r--r--   0 root         (0) root         (0)    29231 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/context.py
--rw-r--r--   0 root         (0) root         (0)    11852 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/load.py
--rw-r--r--   0 root         (0) root         (0)     4721 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/load_target.py
--rw-r--r--   0 root         (0) root         (0)     4311 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/permissions.py
--rw-r--r--   0 root         (0) root         (0)     3463 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_core/workspace/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_daemon/
--rw-r--r--   0 root         (0) root         (0)     1971 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/__init__.py
--rw-r--r--   0 root         (0) root         (0)       30 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/__main__.py
--rw-r--r--   0 root         (0) root         (0)    42160 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/asset_daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_daemon/auto_run_reexecution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/auto_run_reexecution/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7402 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
--rw-r--r--   0 root         (0) root         (0)     9036 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
--rw-r--r--   0 root         (0) root         (0)     2665 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/backfill.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.431741 dagster-1.7.5/dagster/_daemon/cli/
--rw-r--r--   0 root         (0) root         (0)     5118 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19590 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/controller.py
--rw-r--r--   0 root         (0) root         (0)    12656 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/daemon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_daemon/monitoring/
--rw-r--r--   0 root         (0) root         (0)      320 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/monitoring/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1792 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/monitoring/concurrency.py
--rw-r--r--   0 root         (0) root         (0)     9904 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/monitoring/run_monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_daemon/run_coordinator/
--rw-r--r--   0 root         (0) root         (0)      100 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/run_coordinator/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18725 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
--rw-r--r--   0 root         (0) root         (0)    39411 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/sensor.py
--rw-r--r--   0 root         (0) root         (0)     2860 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/types.py
--rw-r--r--   0 root         (0) root         (0)      678 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/utils.py
--rw-r--r--   0 root         (0) root         (0)     4114 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_daemon/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_experimental/
--rw-r--r--   0 root         (0) root         (0)      300 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_experimental/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/
--rw-r--r--   0 root         (0) root         (0)      253 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2997 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/download.py
--rw-r--r--   0 root         (0) root         (0)     4805 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/generate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.363741 dagster-1.7.5/dagster/_generate/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)      175 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)      137 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      297 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)     1753 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
--rw-r--r--   0 root         (0) root         (0)      164 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.435741 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
--rw-r--r--   0 root         (0) root         (0)       80 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       34 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      178 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13462 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/__generated__/api_pb2.py
--rw-r--r--   0 root         (0) root         (0)    27262 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/__generated__/api_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    43164 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/__generated__/api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2060 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)       89 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/__main__.py
--rw-r--r--   0 root         (0) root         (0)    22739 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     3584 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/compile.py
--rw-r--r--   0 root         (0) root         (0)    23173 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_grpc/protos/
--rw-r--r--   0 root         (0) root         (0)     5993 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/protos/api.proto
--rw-r--r--   0 root         (0) root         (0)    13431 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/proxy_server.py
--rw-r--r--   0 root         (0) root         (0)    60914 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/server.py
--rw-r--r--   0 root         (0) root         (0)     5297 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/server_watcher.py
--rw-r--r--   0 root         (0) root         (0)    29291 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/types.py
--rw-r--r--   0 root         (0) root         (0)     3693 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_grpc/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_legacy/
--rw-r--r--   0 root         (0) root         (0)      180 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_legacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_loggers/
--rw-r--r--   0 root         (0) root         (0)     4748 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_loggers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_model/
--rw-r--r--   0 root         (0) root         (0)     1491 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_model/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4295 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_model/pydantic_compat_layer.py
--rw-r--r--   0 root         (0) root         (0)     3269 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_module_alias_map.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_scheduler/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_scheduler/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42035 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_scheduler/scheduler.py
--rw-r--r--   0 root         (0) root         (0)     1262 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_scheduler/stale.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_serdes/
--rw-r--r--   0 root         (0) root         (0)      701 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_serdes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8978 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_serdes/config_class.py
--rw-r--r--   0 root         (0) root         (0)      142 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_serdes/errors.py
--rw-r--r--   0 root         (0) root         (0)     7292 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_serdes/ipc.py
--rw-r--r--   0 root         (0) root         (0)    46494 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_serdes/serdes.py
--rw-r--r--   0 root         (0) root         (0)      674 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_serdes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_seven/
--rw-r--r--   0 root         (0) root         (0)     5455 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_seven/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_seven/abc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.439741 dagster-1.7.5/dagster/_seven/compat/
--rw-r--r--   0 root         (0) root         (0)      105 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_seven/compat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_seven/compat/pendulum.py
--rw-r--r--   0 root         (0) root         (0)      383 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_seven/json.py
--rw-r--r--   0 root         (0) root         (0)      354 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_seven/temp_dir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.443741 dagster-1.7.5/dagster/_utils/
--rw-r--r--   0 root         (0) root         (0)    26539 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9314 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/alert.py
--rw-r--r--   0 root         (0) root         (0)     2250 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/backoff.py
--rw-r--r--   0 root         (0) root         (0)     5536 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/cached_method.py
--rw-r--r--   0 root         (0) root         (0)    44181 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/caching_instance_queryer.py
--rw-r--r--   0 root         (0) root         (0)     5865 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/concurrency.py
--rw-r--r--   0 root         (0) root         (0)    12887 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/container.py
--rw-r--r--   0 root         (0) root         (0)     2412 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/dagster_type.py
--rw-r--r--   0 root         (0) root         (0)      799 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/env.py
--rw-r--r--   0 root         (0) root         (0)     5477 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/error.py
--rw-r--r--   0 root         (0) root         (0)     1255 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/external.py
--rw-r--r--   0 root         (0) root         (0)      891 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/forked_pdb.py
--rw-r--r--   0 root         (0) root         (0)     1870 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/hosted_user_process.py
--rw-r--r--   0 root         (0) root         (0)     2796 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/indenting_printer.py
--rw-r--r--   0 root         (0) root         (0)      745 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/internal_init.py
--rw-r--r--   0 root         (0) root         (0)     3227 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/interrupts.py
--rw-r--r--   0 root         (0) root         (0)    11214 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/log.py
--rw-r--r--   0 root         (0) root         (0)     2313 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/merger.py
--rw-r--r--   0 root         (0) root         (0)     1507 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/net.py
--rw-r--r--   0 root         (0) root         (0)      208 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/partitions.py
--rw-r--r--   0 root         (0) root         (0)    33445 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/schedules.py
--rw-r--r--   0 root         (0) root         (0)      477 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/security.py
--rw-r--r--   0 root         (0) root         (0)     3289 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/tags.py
--rw-r--r--   0 root         (0) root         (0)     1820 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.447741 dagster-1.7.5/dagster/_utils/test/
--rw-r--r--   0 root         (0) root         (0)    13678 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7790 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/data_versions.py
--rw-r--r--   0 root         (0) root         (0)      119 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/hello_world_defs.py
--rw-r--r--   0 root         (0) root         (0)      214 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8622 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/mysql_instance.py
--rw-r--r--   0 root         (0) root         (0)      256 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/named_hello_world_repository.py
--rw-r--r--   0 root         (0) root         (0)     8959 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/postgres_instance.py
--rw-r--r--   0 root         (0) root         (0)    36148 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/schedule_storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.447741 dagster-1.7.5/dagster/_utils/test/toys/
--rw-r--r--   0 root         (0) root         (0)       83 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/toys/__init__.py
--rw-r--r--   0 root         (0) root         (0)       84 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/test/toys/single_repository.py
--rw-r--r--   0 root         (0) root         (0)     2004 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/timing.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/typed_dict.py
--rw-r--r--   0 root         (0) root         (0)      170 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/types.py
--rw-r--r--   0 root         (0) root         (0)     4009 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/typing_api.py
--rw-r--r--   0 root         (0) root         (0)     4740 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/warnings.py
--rw-r--r--   0 root         (0) root         (0)     4902 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/_utils/yaml_utils.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/py.typed
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 17:47:35.000000 dagster-1.7.5/dagster/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:47:59.367741 dagster-1.7.5/dagster.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8928 2024-05-09 17:47:59.000000 dagster-1.7.5/dagster.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    29326 2024-05-09 17:47:59.000000 dagster-1.7.5/dagster.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:47:59.000000 dagster-1.7.5/dagster.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       86 2024-05-09 17:47:59.000000 dagster-1.7.5/dagster.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1467 2024-05-09 17:47:59.000000 dagster-1.7.5/dagster.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-09 17:47:59.000000 dagster-1.7.5/dagster.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      154 2024-05-09 17:47:59.447741 dagster-1.7.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     6847 2024-05-09 17:47:35.000000 dagster-1.7.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.256053 dagster-1.7.6/
+-rw-r--r--   0 root         (0) root         (0)      553 2024-05-16 19:27:09.000000 dagster-1.7.6/COPYING
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-16 19:27:09.000000 dagster-1.7.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      533 2024-05-16 19:27:09.000000 dagster-1.7.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8928 2024-05-16 19:27:38.256053 dagster-1.7.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7214 2024-05-16 19:27:09.000000 dagster-1.7.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.132053 dagster-1.7.6/dagster/
+-rw-r--r--   0 root         (0) root         (0)    30192 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    20744 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_annotations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.136053 dagster-1.7.6/dagster/_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      731 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/get_server_id.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/list_repositories.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/notebook_data.py
+-rw-r--r--   0 root         (0) root         (0)     3224 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/snapshot_execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)     1964 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/snapshot_job.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/snapshot_partition.py
+-rw-r--r--   0 root         (0) root         (0)     1670 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/snapshot_repository.py
+-rw-r--r--   0 root         (0) root         (0)     3021 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/snapshot_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3370 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_api/snapshot_sensor.py
+-rw-r--r--   0 root         (0) root         (0)      478 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_builtins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.136053 dagster-1.7.6/dagster/_check/
+-rw-r--r--   0 root         (0) root         (0)     1352 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_check/README.md
+-rw-r--r--   0 root         (0) root         (0)    52040 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_check/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.140053 dagster-1.7.6/dagster/_cli/
+-rw-r--r--   0 root         (0) root         (0)     1182 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30233 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     8271 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/asset.py
+-rw-r--r--   0 root         (0) root         (0)     8302 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/code_server.py
+-rw-r--r--   0 root         (0) root         (0)     2374 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/config_scaffolder.py
+-rw-r--r--   0 root         (0) root         (0)     3513 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/debug.py
+-rw-r--r--   0 root         (0) root         (0)     8134 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/dev.py
+-rw-r--r--   0 root         (0) root         (0)     6651 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/instance.py
+-rw-r--r--   0 root         (0) root         (0)    30627 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/job.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/load_handle.py
+-rw-r--r--   0 root         (0) root         (0)     9114 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/project.py
+-rw-r--r--   0 root         (0) root         (0)     5120 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/run.py
+-rw-r--r--   0 root         (0) root         (0)    19351 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/schedule.py
+-rw-r--r--   0 root         (0) root         (0)    15461 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     4259 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.140053 dagster-1.7.6/dagster/_cli/workspace/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27910 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_cli/workspace/cli_target.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.144053 dagster-1.7.6/dagster/_config/
+-rw-r--r--   0 root         (0) root         (0)     3186 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3403 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    15830 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/config_type.py
+-rw-r--r--   0 root         (0) root         (0)    18787 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1783 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/evaluate_value_result.py
+-rw-r--r--   0 root         (0) root         (0)    14918 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/field.py
+-rw-r--r--   0 root         (0) root         (0)    19728 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/field_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9536 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/post_process.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/primitive_mapping.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.144053 dagster-1.7.6/dagster/_config/pythonic_config/
+-rw-r--r--   0 root         (0) root         (0)     1394 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1641 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/attach_other_object_to_context.py
+-rw-r--r--   0 root         (0) root         (0)    18114 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/config.py
+-rw-r--r--   0 root         (0) root         (0)    11510 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)    11583 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    41265 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/type_check_utils.py
+-rw-r--r--   0 root         (0) root         (0)     8375 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/pythonic_config/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)    12532 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/snap.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/source.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/stack.py
+-rw-r--r--   0 root         (0) root         (0)     7772 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/traversal_context.py
+-rw-r--r--   0 root         (0) root         (0)     4167 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/type_printer.py
+-rw-r--r--   0 root         (0) root         (0)    17137 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_config/validate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.148053 dagster-1.7.6/dagster/_core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.148053 dagster-1.7.6/dagster/_core/asset_graph_view/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/asset_graph_view/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25057 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/asset_graph_view/asset_graph_view.py
+-rw-r--r--   0 root         (0) root         (0)      994 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/assets.py
+-rw-r--r--   0 root         (0) root         (0)    13427 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/code_pointer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.148053 dagster-1.7.6/dagster/_core/container_context/
+-rw-r--r--   0 root         (0) root         (0)      184 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/container_context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/container_context/config.py
+-rw-r--r--   0 root         (0) root         (0)     2310 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/debug.py
+-rw-r--r--   0 root         (0) root         (0)     9665 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/decorator_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.168053 dagster-1.7.6/dagster/_core/definitions/
+-rw-r--r--   0 root         (0) root         (0)     7873 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4506 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_evaluation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.168053 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.172053 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12253 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/last_update.py
+-rw-r--r--   0 root         (0) root         (0)     7692 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     9763 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py
+-rw-r--r--   0 root         (0) root         (0)     6122 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/schema_change_checks.py
+-rw-r--r--   0 root         (0) root         (0)    11378 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_factories/utils.py
+-rw-r--r--   0 root         (0) root         (0)     7090 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_result.py
+-rw-r--r--   0 root         (0) root         (0)     5628 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_check_spec.py
+-rw-r--r--   0 root         (0) root         (0)     6113 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)    28490 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_daemon_context.py
+-rw-r--r--   0 root         (0) root         (0)     5790 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)     4628 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_dep.py
+-rw-r--r--   0 root         (0) root         (0)    10133 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)     7696 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_graph_differ.py
+-rw-r--r--   0 root         (0) root         (0)    16636 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_graph_subset.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_in.py
+-rw-r--r--   0 root         (0) root         (0)    30136 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_job.py
+-rw-r--r--   0 root         (0) root         (0)     5897 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)    30355 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_layer.py
+-rw-r--r--   0 root         (0) root         (0)     6937 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_out.py
+-rw-r--r--   0 root         (0) root         (0)    39535 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_selection.py
+-rw-r--r--   0 root         (0) root         (0)     7444 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6756 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_spec.py
+-rw-r--r--   0 root         (0) root         (0)    11171 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/asset_subset.py
+-rw-r--r--   0 root         (0) root         (0)    79051 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/assets.py
+-rw-r--r--   0 root         (0) root         (0)    14208 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    11580 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/auto_materialize_rule.py
+-rw-r--r--   0 root         (0) root         (0)    21722 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/auto_materialize_rule_evaluation.py
+-rw-r--r--   0 root         (0) root         (0)    50974 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/auto_materialize_rule_impls.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/auto_materialize_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2939 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/backfill_policy.py
+-rw-r--r--   0 root         (0) root         (0)    35401 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/base_asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)    16772 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/cacheable_assets.py
+-rw-r--r--   0 root         (0) root         (0)    40623 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/composition.py
+-rw-r--r--   0 root         (0) root         (0)     4278 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/config.py
+-rw-r--r--   0 root         (0) root         (0)    14811 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/configurable.py
+-rw-r--r--   0 root         (0) root         (0)    22990 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/data_time.py
+-rw-r--r--   0 root         (0) root         (0)    30236 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/data_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.172053 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/
+-rw-r--r--   0 root         (0) root         (0)     1348 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/README.md
+-rw-r--r--   0 root         (0) root         (0)     1244 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.172053 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/
+-rw-r--r--   0 root         (0) root         (0)       59 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2771 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py
+-rw-r--r--   0 root         (0) root         (0)    16847 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py
+-rw-r--r--   0 root         (0) root         (0)     1642 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/rule_condition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.172053 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4995 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/parent_newer_condition.py
+-rw-r--r--   0 root         (0) root         (0)     4918 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/scheduled_since_condition.py
+-rw-r--r--   0 root         (0) root         (0)     4335 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/slice_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/updated_since_cron_condition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.172053 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operators/
+-rw-r--r--   0 root         (0) root         (0)      280 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operators/boolean_operators.py
+-rw-r--r--   0 root         (0) root         (0)     3710 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operators/dep_operators.py
+-rw-r--r--   0 root         (0) root         (0)    14325 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/scheduling_condition.py
+-rw-r--r--   0 root         (0) root         (0)     7344 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/scheduling_context.py
+-rw-r--r--   0 root         (0) root         (0)     5132 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/scheduling_evaluation_info.py
+-rw-r--r--   0 root         (0) root         (0)    10067 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/serialized_objects.py
+-rw-r--r--   0 root         (0) root         (0)      912 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.176053 dagster-1.7.6/dagster/_core/definitions/decorators/
+-rw-r--r--   0 root         (0) root         (0)      620 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16572 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/asset_check_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    70075 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4907 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/config_mapping_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9077 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/graph_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     9353 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/hook_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    10815 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/job_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    19011 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/op_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    15668 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/repository_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     8718 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/schedule_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12463 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/sensor_decorator.py
+-rw-r--r--   0 root         (0) root         (0)    12656 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/decorators/source_asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     5267 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/definition_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    23545 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/definitions_class.py
+-rw-r--r--   0 root         (0) root         (0)    42243 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/dependency.py
+-rw-r--r--   0 root         (0) root         (0)    28072 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/events.py
+-rw-r--r--   0 root         (0) root         (0)    21182 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/executor_definition.py
+-rw-r--r--   0 root         (0) root         (0)     9379 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/external_asset.py
+-rw-r--r--   0 root         (0) root         (0)     9808 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/freshness_based_auto_materialize.py
+-rw-r--r--   0 root         (0) root         (0)     8801 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    16401 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/freshness_policy_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    47569 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/graph_definition.py
+-rw-r--r--   0 root         (0) root         (0)     6546 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/hook_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1524 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/hook_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3537 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/inference.py
+-rw-r--r--   0 root         (0) root         (0)    21027 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/input.py
+-rw-r--r--   0 root         (0) root         (0)     6410 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/instigation_logger.py
+-rw-r--r--   0 root         (0) root         (0)     2991 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/job_base.py
+-rw-r--r--   0 root         (0) root         (0)    54423 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/job_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5693 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/load_asset_checks_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)    22306 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/load_assets_from_modules.py
+-rw-r--r--   0 root         (0) root         (0)     7171 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/logger_definition.py
+-rw-r--r--   0 root         (0) root         (0)      636 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/logger_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     8703 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/materialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.176053 dagster-1.7.6/dagster/_core/definitions/metadata/
+-rw-r--r--   0 root         (0) root         (0)     9922 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5848 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/metadata/metadata_set.py
+-rw-r--r--   0 root         (0) root         (0)    31381 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/metadata/metadata_value.py
+-rw-r--r--   0 root         (0) root         (0)     4795 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/metadata/source_code.py
+-rw-r--r--   0 root         (0) root         (0)    12486 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/metadata/table.py
+-rw-r--r--   0 root         (0) root         (0)    57203 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/multi_asset_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    22029 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/multi_dimensional_partitions.py
+-rw-r--r--   0 root         (0) root         (0)      197 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/no_step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    11892 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/node_container.py
+-rw-r--r--   0 root         (0) root         (0)     8016 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/node_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2892 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/observe.py
+-rw-r--r--   0 root         (0) root         (0)    23078 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/op_definition.py
+-rw-r--r--   0 root         (0) root         (0)    23141 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/op_invocation.py
+-rw-r--r--   0 root         (0) root         (0)     7551 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/op_selection.py
+-rw-r--r--   0 root         (0) root         (0)    19237 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/output.py
+-rw-r--r--   0 root         (0) root         (0)    50520 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/partition.py
+-rw-r--r--   0 root         (0) root         (0)      630 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/partition_key_range.py
+-rw-r--r--   0 root         (0) root         (0)    47665 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)    11087 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/partitioned_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/policy.py
+-rw-r--r--   0 root         (0) root         (0)    27690 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/reconstruct.py
+-rw-r--r--   0 root         (0) root         (0)    21602 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/remote_asset_graph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.180053 dagster-1.7.6/dagster/_core/definitions/repository_definition/
+-rw-r--r--   0 root         (0) root         (0)      654 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/repository_definition/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6024 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/repository_definition/caching_index.py
+-rw-r--r--   0 root         (0) root         (0)    21698 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/repository_definition/repository_data.py
+-rw-r--r--   0 root         (0) root         (0)    20892 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/repository_definition/repository_data_builder.py
+-rw-r--r--   0 root         (0) root         (0)    20432 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/repository_definition/repository_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/repository_definition/valid_definitions.py
+-rw-r--r--   0 root         (0) root         (0)     8858 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/resolved_asset_deps.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/resource_annotation.py
+-rw-r--r--   0 root         (0) root         (0)    17900 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/resource_invocation.py
+-rw-r--r--   0 root         (0) root         (0)    10320 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/resource_requirement.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/result.py
+-rw-r--r--   0 root         (0) root         (0)    23076 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1445 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    19555 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/run_request.py
+-rw-r--r--   0 root         (0) root         (0)    45639 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/run_status_sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    39363 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/schedule_definition.py
+-rw-r--r--   0 root         (0) root         (0)     5134 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/scoped_resources_builder.py
+-rw-r--r--   0 root         (0) root         (0)    14134 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/selector.py
+-rw-r--r--   0 root         (0) root         (0)    53797 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/sensor_definition.py
+-rw-r--r--   0 root         (0) root         (0)    19236 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/source_asset.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/step_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/target.py
+-rw-r--r--   0 root         (0) root         (0)    22389 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/time_window_partition_mapping.py
+-rw-r--r--   0 root         (0) root         (0)   102817 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/time_window_partitions.py
+-rw-r--r--   0 root         (0) root         (0)    16727 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/unresolved_asset_job_definition.py
+-rw-r--r--   0 root         (0) root         (0)    11027 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3982 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/definitions/version_strategy.py
+-rw-r--r--   0 root         (0) root         (0)    26986 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    17452 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/event_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.180053 dagster-1.7.6/dagster/_core/events/
+-rw-r--r--   0 root         (0) root         (0)    71913 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/events/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8142 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/events/log.py
+-rw-r--r--   0 root         (0) root         (0)     1614 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/events/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.184053 dagster-1.7.6/dagster/_core/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38363 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/api.py
+-rw-r--r--   0 root         (0) root         (0)    67853 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/asset_backfill.py
+-rw-r--r--   0 root         (0) root         (0)    17100 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6296 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/build_resources.py
+-rw-r--r--   0 root         (0) root         (0)      224 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/bulk_actions.py
+-rw-r--r--   0 root         (0) root         (0)     5587 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/compute_logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.184053 dagster-1.7.6/dagster/_core/execution/context/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79687 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/compute.py
+-rw-r--r--   0 root         (0) root         (0)    10226 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/data_version_cache.py
+-rw-r--r--   0 root         (0) root         (0)    17598 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/hook.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/init.py
+-rw-r--r--   0 root         (0) root         (0)    29167 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/input.py
+-rw-r--r--   0 root         (0) root         (0)    40124 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/invocation.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/logger.py
+-rw-r--r--   0 root         (0) root         (0)    37256 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/output.py
+-rw-r--r--   0 root         (0) root         (0)    49252 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context/system.py
+-rw-r--r--   0 root         (0) root         (0)    18837 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/context_creation_job.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/execute_in_process.py
+-rw-r--r--   0 root         (0) root         (0)     5897 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/execute_in_process_result.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/execution_result.py
+-rw-r--r--   0 root         (0) root         (0)     8602 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/host_mode.py
+-rw-r--r--   0 root         (0) root         (0)    18608 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/job_backfill.py
+-rw-r--r--   0 root         (0) root         (0)     6723 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/job_execution_result.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/memoization.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.188053 dagster-1.7.6/dagster/_core/execution/plan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26460 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/active.py
+-rw-r--r--   0 root         (0) root         (0)     9850 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/compute.py
+-rw-r--r--   0 root         (0) root         (0)    17062 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/compute_generator.py
+-rw-r--r--   0 root         (0) root         (0)    16974 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/execute_plan.py
+-rw-r--r--   0 root         (0) root         (0)    40877 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/execute_step.py
+-rw-r--r--   0 root         (0) root         (0)    11032 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/external_step.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/handle.py
+-rw-r--r--   0 root         (0) root         (0)    39260 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/inputs.py
+-rw-r--r--   0 root         (0) root         (0)     6251 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/instance_concurrency_context.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/local_external_step_main.py
+-rw-r--r--   0 root         (0) root         (0)     5706 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/objects.py
+-rw-r--r--   0 root         (0) root         (0)     7326 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/outputs.py
+-rw-r--r--   0 root         (0) root         (0)    61075 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/plan.py
+-rw-r--r--   0 root         (0) root         (0)      114 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/resume_retry.py
+-rw-r--r--   0 root         (0) root         (0)    17174 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/state.py
+-rw-r--r--   0 root         (0) root         (0)    15985 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/step.py
+-rw-r--r--   0 root         (0) root         (0)     3796 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/plan/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/poll_compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)     8230 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/resolve_versions.py
+-rw-r--r--   0 root         (0) root         (0)    19141 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/resources_init.py
+-rw-r--r--   0 root         (0) root         (0)     2100 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/retries.py
+-rw-r--r--   0 root         (0) root         (0)     1564 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/run_cancellation_thread.py
+-rw-r--r--   0 root         (0) root         (0)     9764 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/run_metrics_thread.py
+-rw-r--r--   0 root         (0) root         (0)     9950 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/stats.py
+-rw-r--r--   0 root         (0) root         (0)    15211 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/submit_asset_runs.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/tags.py
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/types.py
+-rw-r--r--   0 root         (0) root         (0)     1172 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/validate_run_config.py
+-rw-r--r--   0 root         (0) root         (0)     1282 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/watch_orphans.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/execution/with_resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.192053 dagster-1.7.6/dagster/_core/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/base.py
+-rw-r--r--   0 root         (0) root         (0)     5989 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/child_process_executor.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/in_process.py
+-rw-r--r--   0 root         (0) root         (0)     1509 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/init.py
+-rw-r--r--   0 root         (0) root         (0)    15497 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/multiprocess.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.192053 dagster-1.7.6/dagster/_core/executor/step_delegating/
+-rw-r--r--   0 root         (0) root         (0)      247 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/step_delegating/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16894 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/step_delegating/step_delegating_executor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.192053 dagster-1.7.6/dagster/_core/executor/step_delegating/step_handler/
+-rw-r--r--   0 root         (0) root         (0)      152 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/step_delegating/step_handler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3078 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/executor/step_delegating/step_handler/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.192053 dagster-1.7.6/dagster/_core/instance/
+-rw-r--r--   0 root         (0) root         (0)   132126 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/instance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15788 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/instance/config.py
+-rw-r--r--   0 root         (0) root         (0)    24141 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/instance/ref.py
+-rw-r--r--   0 root         (0) root         (0)     3899 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/instance_for_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.192053 dagster-1.7.6/dagster/_core/launcher/
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3819 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/launcher/base.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/launcher/default_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1566 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/launcher/sync_in_memory_run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)      473 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/libraries.py
+-rw-r--r--   0 root         (0) root         (0)    18041 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/nux.py
+-rw-r--r--   0 root         (0) root         (0)     6656 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/op_concurrency_limits_counter.py
+-rw-r--r--   0 root         (0) root         (0)     3691 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/origin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.192053 dagster-1.7.6/dagster/_core/pipes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/pipes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8974 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/pipes/client.py
+-rw-r--r--   0 root         (0) root         (0)    18318 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/pipes/context.py
+-rw-r--r--   0 root         (0) root         (0)     5624 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/pipes/subprocess.py
+-rw-r--r--   0 root         (0) root         (0)    25661 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/pipes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.196053 dagster-1.7.6/dagster/_core/remote_representation/
+-rw-r--r--   0 root         (0) root         (0)     2793 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36695 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/code_location.py
+-rw-r--r--   0 root         (0) root         (0)    37860 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/external.py
+-rw-r--r--   0 root         (0) root         (0)    83881 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/external_data.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/feature_flags.py
+-rw-r--r--   0 root         (0) root         (0)    12429 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/grpc_server_registry.py
+-rw-r--r--   0 root         (0) root         (0)     1487 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/grpc_server_state_subscriber.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/handle.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/historical.py
+-rw-r--r--   0 root         (0) root         (0)     4850 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/job_index.py
+-rw-r--r--   0 root         (0) root         (0)    19669 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/origin.py
+-rw-r--r--   0 root         (0) root         (0)     3602 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/remote_representation/represented.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.196053 dagster-1.7.6/dagster/_core/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      267 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/run_coordinator/base.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/run_coordinator/default_run_coordinator.py
+-rw-r--r--   0 root         (0) root         (0)    13364 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/run_coordinator/queued_run_coordinator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.196053 dagster-1.7.6/dagster/_core/scheduler/
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1241 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/scheduler/execution.py
+-rw-r--r--   0 root         (0) root         (0)    28819 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/scheduler/instigation.py
+-rw-r--r--   0 root         (0) root         (0)    10917 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/scheduler/scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.200053 dagster-1.7.6/dagster/_core/secrets/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1801 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/secrets/env_file.py
+-rw-r--r--   0 root         (0) root         (0)      388 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.200053 dagster-1.7.6/dagster/_core/selector/
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/selector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18109 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/selector/subset_selector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.200053 dagster-1.7.6/dagster/_core/snap/
+-rw-r--r--   0 root         (0) root         (0)     2842 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     9302 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/dep_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    12155 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/execution_plan_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)    16934 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/job_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/mode.py
+-rw-r--r--   0 root         (0) root         (0)    14185 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/node.py
+-rw-r--r--   0 root         (0) root         (0)     3183 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/snap/snap_to_yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.208053 dagster-1.7.6/dagster/_core/storage/
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/DEVELOPING.md
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.208053 dagster-1.7.6/dagster/_core/storage/alembic/
+-rw-r--r--   0 root         (0) root         (0)     6686 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/README.md
+-rw-r--r--   0 root         (0) root         (0)      687 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      494 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.224053 dagster-1.7.6/dagster/_core/storage/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     3150 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/001_initial_1.py
+-rw-r--r--   0 root         (0) root         (0)      312 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/001_initial_schedule.py
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      599 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      973 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1406 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      953 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      956 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1730 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1147 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py
+-rw-r--r--   0 root         (0) root         (0)     1143 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/012_0_10_0_create_new_run_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      435 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/013_0_10_0_create_new_event_log_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      432 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/014_0_10_0_create_new_schedule_tables_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      409 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/016_add_bulk_actions_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      936 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      325 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/017_initial_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/018_add_asset_tags_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/018_add_asset_tags_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/018_add_asset_tags_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/020_add_column_asset_body_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/020_add_column_asset_body_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/020_add_column_asset_body_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1034 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/022_extract_asset_keys_index_columns_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/023_add_event_log_event_type_idx_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      531 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py
+-rw-r--r--   0 root         (0) root         (0)     1275 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/025_add_range_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/025_add_range_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      404 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/025_add_range_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      635 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/027_add_migration_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/027_add_migration_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      434 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/027_add_migration_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/028_add_instigators_table_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/028_add_instigators_table_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/028_add_instigators_table_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_mysql.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_postgres.py
+-rw-r--r--   0 root         (0) root         (0)      416 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/029_add_tick_selector_index_sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py
+-rw-r--r--   0 root         (0) root         (0)      958 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/031_add_kvs_table.py
+-rw-r--r--   0 root         (0) root         (0)      499 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/032_rebuild_event_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     1951 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/034_add_cached_status_data_column.py
+-rw-r--r--   0 root         (0) root         (0)      427 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/035_add_run_job_index.py
+-rw-r--r--   0 root         (0) root         (0)     1537 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py
+-rw-r--r--   0 root         (0) root         (0)     1177 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py
+-rw-r--r--   0 root         (0) root         (0)     2062 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py
+-rw-r--r--   0 root         (0) root         (0)     2359 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py
+-rw-r--r--   0 root         (0) root         (0)     1322 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3872 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/asset_check_execution_record.py
+-rw-r--r--   0 root         (0) root         (0)     7301 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/asset_value_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/base_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3320 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/batch_asset_record_loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.224053 dagster-1.7.6/dagster/_core/storage/branching/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/branching/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/branching/branching_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8725 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/captured_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)    16223 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/cloud_storage_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     9557 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/config.py
+-rw-r--r--   0 root         (0) root         (0)      417 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/daemon_cursor.py
+-rw-r--r--   0 root         (0) root         (0)    25652 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/dagster_run.py
+-rw-r--r--   0 root         (0) root         (0)    11187 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/db_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.224053 dagster-1.7.6/dagster/_core/storage/event_log/
+-rw-r--r--   0 root         (0) root         (0)      742 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20682 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/base.py
+-rw-r--r--   0 root         (0) root         (0)     3801 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     7289 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/migration.py
+-rw-r--r--   0 root         (0) root         (0)     8037 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/polling_event_watcher.py
+-rw-r--r--   0 root         (0) root         (0)     9250 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/schema.py
+-rw-r--r--   0 root         (0) root         (0)   122186 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/sql_event_log.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.224053 dagster-1.7.6/dagster/_core/storage/event_log/sqlite/
+-rw-r--r--   0 root         (0) root         (0)      200 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.224053 dagster-1.7.6/dagster/_core/storage/event_log/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     7508 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    22497 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py
+-rw-r--r--   0 root         (0) root         (0)    10983 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13492 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/fs_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     8819 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/input_manager.py
+-rw-r--r--   0 root         (0) root         (0)    10882 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/io_manager.py
+-rw-r--r--   0 root         (0) root         (0)    32639 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/legacy_storage.py
+-rw-r--r--   0 root         (0) root         (0)    17558 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/local_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/mem_io_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4355 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/memoizable_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.228053 dagster-1.7.6/dagster/_core/storage/migration/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/migration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/migration/bigint_migration.py
+-rw-r--r--   0 root         (0) root         (0)    15491 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/migration/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3270 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/noop_compute_log_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/output_manager.py
+-rw-r--r--   0 root         (0) root         (0)    18101 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/partition_status_cache.py
+-rw-r--r--   0 root         (0) root         (0)     2121 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/root.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.228053 dagster-1.7.6/dagster/_core/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)      386 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14231 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/base.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/in_memory.py
+-rw-r--r--   0 root         (0) root         (0)     8716 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/migration.py
+-rw-r--r--   0 root         (0) root         (0)     6391 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/schema.py
+-rw-r--r--   0 root         (0) root         (0)    37611 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/sql_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.228053 dagster-1.7.6/dagster/_core/storage/runs/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.228053 dagster-1.7.6/dagster/_core/storage/runs/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     6310 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.232053 dagster-1.7.6/dagster/_core/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)      272 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7246 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/base.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/migration.py
+-rw-r--r--   0 root         (0) root         (0)     4086 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/schema.py
+-rw-r--r--   0 root         (0) root         (0)    25156 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/sql_schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.232053 dagster-1.7.6/dagster/_core/storage/schedules/sqlite/
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/sqlite/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.232053 dagster-1.7.6/dagster/_core/storage/schedules/sqlite/alembic/
+-rw-r--r--   0 root         (0) root         (0)      986 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini
+-rw-r--r--   0 root         (0) root         (0)     3684 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py
+-rw-r--r--   0 root         (0) root         (0)     7691 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/sql.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/sqlalchemy_compat.py
+-rw-r--r--   0 root         (0) root         (0)      926 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/sqlite.py
+-rw-r--r--   0 root         (0) root         (0)     4875 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/sqlite_storage.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/temp_file_manager.py
+-rw-r--r--   0 root         (0) root         (0)    19736 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/storage/upath_io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.232053 dagster-1.7.6/dagster/_core/system_config/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/system_config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13962 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/system_config/composite_descent.py
+-rw-r--r--   0 root         (0) root         (0)    15178 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/system_config/objects.py
+-rw-r--r--   0 root         (0) root         (0)    29921 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     4824 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/telemetry_upload.py
+-rw-r--r--   0 root         (0) root         (0)    22361 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.232053 dagster-1.7.6/dagster/_core/types/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3084 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/builtin_config_schemas.py
+-rw-r--r--   0 root         (0) root         (0)     7042 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    36504 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/decorator.py
+-rw-r--r--   0 root         (0) root         (0)     1846 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/loadable_target_origin.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/primitive_mapping.py
+-rw-r--r--   0 root         (0) root         (0)     4764 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/python_dict.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/python_set.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/python_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/types/transform_typing.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/utility_ops.py
+-rw-r--r--   0 root         (0) root         (0)     6652 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.236053 dagster-1.7.6/dagster/_core/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4457 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/autodiscovery.py
+-rw-r--r--   0 root         (0) root         (0)     3422 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/config_schema.py
+-rw-r--r--   0 root         (0) root         (0)    29231 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/context.py
+-rw-r--r--   0 root         (0) root         (0)    11852 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/load.py
+-rw-r--r--   0 root         (0) root         (0)     4721 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/load_target.py
+-rw-r--r--   0 root         (0) root         (0)     4311 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/permissions.py
+-rw-r--r--   0 root         (0) root         (0)     3463 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_core/workspace/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.236053 dagster-1.7.6/dagster/_daemon/
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    42160 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/asset_daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.236053 dagster-1.7.6/dagster/_daemon/auto_run_reexecution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/auto_run_reexecution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7402 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py
+-rw-r--r--   0 root         (0) root         (0)     9036 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/auto_run_reexecution/event_log_consumer.py
+-rw-r--r--   0 root         (0) root         (0)     3014 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/backfill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.236053 dagster-1.7.6/dagster/_daemon/cli/
+-rw-r--r--   0 root         (0) root         (0)     5118 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19590 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/controller.py
+-rw-r--r--   0 root         (0) root         (0)    12656 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_daemon/monitoring/
+-rw-r--r--   0 root         (0) root         (0)      320 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/monitoring/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/monitoring/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)     9904 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/monitoring/run_monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_daemon/run_coordinator/
+-rw-r--r--   0 root         (0) root         (0)      100 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/run_coordinator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18725 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py
+-rw-r--r--   0 root         (0) root         (0)    39411 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/sensor.py
+-rw-r--r--   0 root         (0) root         (0)     2860 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/types.py
+-rw-r--r--   0 root         (0) root         (0)      678 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_daemon/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_experimental/
+-rw-r--r--   0 root         (0) root         (0)      300 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_experimental/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_generate/
+-rw-r--r--   0 root         (0) root         (0)      253 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/download.py
+-rw-r--r--   0 root         (0) root         (0)     4805 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/generate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.128053 dagster-1.7.6/dagster/_generate/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)      175 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER/assets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/CODE_LOCATION_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)      137 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/pyproject.toml.tmpl
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      297 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/CODE_LOCATION_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)     1753 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.240053 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.244053 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/__init__.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/assets.py
+-rw-r--r--   0 root         (0) root         (0)      164 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER/repository.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.244053 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/REPO_NAME_PLACEHOLDER_tests/test_assets.py.tmpl
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.cfg.tmpl
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_generate/templates/REPO_NAME_PLACEHOLDER/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.244053 dagster-1.7.6/dagster/_grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.244053 dagster-1.7.6/dagster/_grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      178 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13462 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/__generated__/api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    27262 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/__generated__/api_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    43164 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/__generated__/api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2060 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       89 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    22739 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3584 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/compile.py
+-rw-r--r--   0 root         (0) root         (0)    23173 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.244053 dagster-1.7.6/dagster/_grpc/protos/
+-rw-r--r--   0 root         (0) root         (0)     5993 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/protos/api.proto
+-rw-r--r--   0 root         (0) root         (0)    13431 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/proxy_server.py
+-rw-r--r--   0 root         (0) root         (0)    60914 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/server.py
+-rw-r--r--   0 root         (0) root         (0)     5297 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/server_watcher.py
+-rw-r--r--   0 root         (0) root         (0)    29291 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/types.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_grpc/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.248053 dagster-1.7.6/dagster/_legacy/
+-rw-r--r--   0 root         (0) root         (0)      180 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_legacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.248053 dagster-1.7.6/dagster/_loggers/
+-rw-r--r--   0 root         (0) root         (0)     4748 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_loggers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.248053 dagster-1.7.6/dagster/_model/
+-rw-r--r--   0 root         (0) root         (0)     2306 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4295 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_model/pydantic_compat_layer.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_module_alias_map.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.248053 dagster-1.7.6/dagster/_scheduler/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_scheduler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42035 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_scheduler/scheduler.py
+-rw-r--r--   0 root         (0) root         (0)     1262 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_scheduler/stale.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.248053 dagster-1.7.6/dagster/_serdes/
+-rw-r--r--   0 root         (0) root         (0)      701 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_serdes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8978 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_serdes/config_class.py
+-rw-r--r--   0 root         (0) root         (0)      142 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_serdes/errors.py
+-rw-r--r--   0 root         (0) root         (0)     7292 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_serdes/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    46494 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_serdes/serdes.py
+-rw-r--r--   0 root         (0) root         (0)      674 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_serdes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.248053 dagster-1.7.6/dagster/_seven/
+-rw-r--r--   0 root         (0) root         (0)     5455 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_seven/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_seven/abc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.248053 dagster-1.7.6/dagster/_seven/compat/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_seven/compat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      603 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_seven/compat/datetime.py
+-rw-r--r--   0 root         (0) root         (0)     4114 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_seven/compat/pendulum.py
+-rw-r--r--   0 root         (0) root         (0)      383 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_seven/json.py
+-rw-r--r--   0 root         (0) root         (0)      354 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_seven/temp_dir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.256053 dagster-1.7.6/dagster/_utils/
+-rw-r--r--   0 root         (0) root         (0)    26652 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9314 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/alert.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/backoff.py
+-rw-r--r--   0 root         (0) root         (0)     5536 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/cached_method.py
+-rw-r--r--   0 root         (0) root         (0)    45456 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/caching_instance_queryer.py
+-rw-r--r--   0 root         (0) root         (0)     5865 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/concurrency.py
+-rw-r--r--   0 root         (0) root         (0)    13054 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/container.py
+-rw-r--r--   0 root         (0) root         (0)     2412 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/dagster_type.py
+-rw-r--r--   0 root         (0) root         (0)      799 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/env.py
+-rw-r--r--   0 root         (0) root         (0)     5477 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/error.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/external.py
+-rw-r--r--   0 root         (0) root         (0)      891 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/forked_pdb.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/hosted_user_process.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/indenting_printer.py
+-rw-r--r--   0 root         (0) root         (0)      745 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/internal_init.py
+-rw-r--r--   0 root         (0) root         (0)     3227 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/interrupts.py
+-rw-r--r--   0 root         (0) root         (0)    11253 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/merger.py
+-rw-r--r--   0 root         (0) root         (0)     1507 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/net.py
+-rw-r--r--   0 root         (0) root         (0)      208 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/partitions.py
+-rw-r--r--   0 root         (0) root         (0)    32783 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/schedules.py
+-rw-r--r--   0 root         (0) root         (0)      477 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/security.py
+-rw-r--r--   0 root         (0) root         (0)     3289 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/tags.py
+-rw-r--r--   0 root         (0) root         (0)     1820 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/temp_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.256053 dagster-1.7.6/dagster/_utils/test/
+-rw-r--r--   0 root         (0) root         (0)    13678 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7790 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/data_versions.py
+-rw-r--r--   0 root         (0) root         (0)      119 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/hello_world_defs.py
+-rw-r--r--   0 root         (0) root         (0)      214 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/mysql_instance.py
+-rw-r--r--   0 root         (0) root         (0)      256 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/named_hello_world_repository.py
+-rw-r--r--   0 root         (0) root         (0)     8959 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/postgres_instance.py
+-rw-r--r--   0 root         (0) root         (0)    36148 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/schedule_storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.256053 dagster-1.7.6/dagster/_utils/test/toys/
+-rw-r--r--   0 root         (0) root         (0)       83 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/toys/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       84 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/test/toys/single_repository.py
+-rw-r--r--   0 root         (0) root         (0)     2004 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/timing.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/typed_dict.py
+-rw-r--r--   0 root         (0) root         (0)      170 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/types.py
+-rw-r--r--   0 root         (0) root         (0)     4009 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/typing_api.py
+-rw-r--r--   0 root         (0) root         (0)     4740 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/warnings.py
+-rw-r--r--   0 root         (0) root         (0)     4902 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/_utils/yaml_utils.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/py.typed
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-16 19:27:09.000000 dagster-1.7.6/dagster/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:27:38.136053 dagster-1.7.6/dagster.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8928 2024-05-16 19:27:37.000000 dagster-1.7.6/dagster.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    29718 2024-05-16 19:27:37.000000 dagster-1.7.6/dagster.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 19:27:37.000000 dagster-1.7.6/dagster.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2024-05-16 19:27:37.000000 dagster-1.7.6/dagster.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1483 2024-05-16 19:27:37.000000 dagster-1.7.6/dagster.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-16 19:27:37.000000 dagster-1.7.6/dagster.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      154 2024-05-16 19:27:38.260053 dagster-1.7.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     6901 2024-05-16 19:27:10.000000 dagster-1.7.6/setup.py
```

### Comparing `dagster-1.7.5/COPYING` & `dagster-1.7.6/COPYING`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/LICENSE` & `dagster-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/MANIFEST.in` & `dagster-1.7.6/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/PKG-INFO` & `dagster-1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.5
+Version: 1.7.6
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
```

### Comparing `dagster-1.7.5/README.md` & `dagster-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/__init__.py` & `dagster-1.7.6/dagster/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,14 +281,15 @@
     PythonArtifactMetadataValue as PythonArtifactMetadataValue,
     TableColumnLineageMetadataValue as TableColumnLineageMetadataValue,
     TableMetadataValue as TableMetadataValue,
     TableSchemaMetadataValue as TableSchemaMetadataValue,
     TextMetadataValue as TextMetadataValue,
     TimestampMetadataValue as TimestampMetadataValue,
     UrlMetadataValue as UrlMetadataValue,
+    with_source_code_references as with_source_code_references,
 )
 from dagster._core.definitions.metadata.table import (
     TableColumn as TableColumn,
     TableColumnConstraints as TableColumnConstraints,
     TableColumnDep as TableColumnDep,
     TableColumnLineage as TableColumnLineage,
     TableConstraints as TableConstraints,
```

### Comparing `dagster-1.7.5/dagster/_annotations.py` & `dagster-1.7.6/dagster/_annotations.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_api/get_server_id.py` & `dagster-1.7.6/dagster/_api/get_server_id.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_api/list_repositories.py` & `dagster-1.7.6/dagster/_api/list_repositories.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_api/notebook_data.py` & `dagster-1.7.6/dagster/_api/notebook_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_api/snapshot_execution_plan.py` & `dagster-1.7.6/dagster/_api/snapshot_execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_api/snapshot_job.py` & `dagster-1.7.6/dagster/_api/snapshot_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_api/snapshot_partition.py` & `dagster-1.7.6/dagster/_api/snapshot_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_api/snapshot_repository.py` & `dagster-1.7.6/dagster/_api/snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_api/snapshot_schedule.py` & `dagster-1.7.6/dagster/_api/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_api/snapshot_sensor.py` & `dagster-1.7.6/dagster/_api/snapshot_sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_check/README.md` & `dagster-1.7.6/dagster/_check/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_check/__init__.py` & `dagster-1.7.6/dagster/_check/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_cli/__init__.py` & `dagster-1.7.6/dagster/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_cli/api.py` & `dagster-1.7.6/dagster/_cli/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -36,14 +36,19 @@
 from dagster._grpc.types import ExecuteRunArgs, ExecuteStepArgs, ResumeRunArgs
 from dagster._serdes import deserialize_value, serialize_value
 from dagster._utils.error import serializable_error_info_from_exc_info
 from dagster._utils.hosted_user_process import recon_job_from_origin
 from dagster._utils.interrupts import capture_interrupts, setup_interrupt_handlers
 from dagster._utils.log import configure_loggers
 
+from .._core.execution.run_metrics_thread import (
+    DEFAULT_RUN_METRICS_POLL_INTERVAL_SECONDS,
+    start_run_metrics_thread,
+    stop_run_metrics_thread,
+)
 from .utils import get_instance_for_cli
 
 
 @click.group(name="api", hidden=True)
 def api_cli():
     """[INTERNAL] These commands are intended to support internal use cases. Users should generally
     not invoke these commands interactively.
@@ -75,14 +80,51 @@
                 set_exit_code_on_failure=args.set_exit_code_on_failure or False,
             )
 
             if return_code != 0:
                 sys.exit(return_code)
 
 
+def _truthy_tag_value(dagster_run: DagsterRun, tag: str, default: str = "false") -> bool:
+    return dagster_run.tags.get(tag, default).casefold() not in ["false", "0", "off", "no", ""]
+
+
+def _should_start_metrics_thread(dagster_run: DagsterRun) -> bool:
+    return _truthy_tag_value(dagster_run, "dagster/run_metrics")
+
+
+def _enable_python_runtime_metrics(dagster_run: DagsterRun) -> bool:
+    return _truthy_tag_value(dagster_run, "dagster/python_runtime_metrics")
+
+
+def _report_container_metrics_as_engine_events(dagster_run: DagsterRun) -> bool:
+    return _truthy_tag_value(dagster_run, "dagster/container_metrics_engine_events")
+
+
+def _metrics_polling_interval(
+    dagster_run: DagsterRun, logger: Optional[logging.Logger] = None
+) -> float:
+    try:
+        return float(
+            dagster_run.tags.get(
+                "dagster/run_metrics_polling_interval_seconds",
+                DEFAULT_RUN_METRICS_POLL_INTERVAL_SECONDS,
+            )
+        )
+    except ValueError:
+        if logger:
+            logger.warning(
+                (
+                    "Invalid value for dagster/run_metrics_polling_interval_seconds tag."
+                    f"Setting metric polling interval to default value: {DEFAULT_RUN_METRICS_POLL_INTERVAL_SECONDS}."
+                )
+            )
+        return DEFAULT_RUN_METRICS_POLL_INTERVAL_SECONDS
+
+
 def _execute_run_command_body(
     run_id: str,
     instance: DagsterInstance,
     write_stream_fn: Callable[[DagsterEvent], Any],
     set_exit_code_on_failure: bool,
 ) -> int:
     if instance.should_start_background_run_thread:
@@ -98,14 +140,29 @@
     )
 
     check.not_none(
         dagster_run.job_code_origin,
         f"Run with id '{run_id}' does not include an origin.",
     )
 
+    start_metric_thread = _should_start_metrics_thread(dagster_run)
+    if start_metric_thread:
+        logger = logging.getLogger("run_metrics")
+        polling_interval = _metrics_polling_interval(dagster_run, logger=logger)
+        metrics_thread, metrics_thread_shutdown_event = start_run_metrics_thread(
+            instance,
+            dagster_run,
+            container_metrics_enabled=True,
+            python_metrics_enabled=_enable_python_runtime_metrics(dagster_run),
+            polling_interval=polling_interval,
+            logger=logger,
+        )
+    else:
+        metrics_thread, metrics_thread_shutdown_event = None, None
+
     recon_job = recon_job_from_origin(cast(JobPythonOrigin, dagster_run.job_code_origin))
 
     pid = os.getpid()
     instance.report_engine_event(
         f"Started process for run (pid: {pid}).",
         dagster_run,
         EngineEventData.in_process(pid),
@@ -123,14 +180,19 @@
             write_stream_fn(event)
             if event.event_type == DagsterEventType.PIPELINE_FAILURE:
                 run_worker_failed = True
     except:
         # relies on core_execute_run writing failures to the event log before raising
         run_worker_failed = True
     finally:
+        if metrics_thread and metrics_thread_shutdown_event:
+            stopped = stop_run_metrics_thread(metrics_thread, metrics_thread_shutdown_event)
+            if not stopped:
+                instance.report_engine_event("Metrics thread did not shutdown properly")
+
         if instance.should_start_background_run_thread:
             cancellation_thread_shutdown_event = check.not_none(cancellation_thread_shutdown_event)
             cancellation_thread = check.not_none(cancellation_thread)
             cancellation_thread_shutdown_event.set()
             if cancellation_thread.is_alive():
                 cancellation_thread.join(timeout=15)
                 if cancellation_thread.is_alive():
@@ -193,14 +255,29 @@
         f"Run with id '{run_id}' not found for run execution.",
     )
     check.not_none(
         dagster_run.job_code_origin,
         f"Run with id '{run_id}' does not include an origin.",
     )
 
+    start_metric_thread = _should_start_metrics_thread(dagster_run)
+    if start_metric_thread:
+        logger = logging.getLogger("run_metrics")
+        polling_interval = _metrics_polling_interval(dagster_run, logger=logger)
+        metrics_thread, metrics_thread_shutdown_event = start_run_metrics_thread(
+            instance,
+            dagster_run,
+            container_metrics_enabled=True,
+            python_metrics_enabled=_enable_python_runtime_metrics(dagster_run),
+            polling_interval=polling_interval,
+            logger=logger,
+        )
+    else:
+        metrics_thread, metrics_thread_shutdown_event = None, None
+
     recon_job = recon_job_from_origin(cast(JobPythonOrigin, dagster_run.job_code_origin))
 
     pid = os.getpid()
     instance.report_engine_event(
         f"Started process for resuming job (pid: {pid}).",
         dagster_run,
         EngineEventData.in_process(pid),
@@ -220,14 +297,19 @@
             if event.event_type == DagsterEventType.PIPELINE_FAILURE:
                 run_worker_failed = True
 
     except:
         # relies on core_execute_run writing failures to the event log before raising
         run_worker_failed = True
     finally:
+        if metrics_thread and metrics_thread_shutdown_event:
+            stopped = stop_run_metrics_thread(metrics_thread, metrics_thread_shutdown_event)
+            if not stopped:
+                instance.report_engine_event("Metrics thread did not shutdown properly")
+
         if instance.should_start_background_run_thread:
             cancellation_thread_shutdown_event = check.not_none(cancellation_thread_shutdown_event)
             cancellation_thread = check.not_none(cancellation_thread)
             cancellation_thread_shutdown_event.set()
             if cancellation_thread.is_alive():
                 cancellation_thread.join(timeout=15)
                 if cancellation_thread.is_alive():
```

### Comparing `dagster-1.7.5/dagster/_cli/asset.py` & `dagster-1.7.6/dagster/_cli/asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_cli/code_server.py` & `dagster-1.7.6/dagster/_cli/code_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_cli/config_scaffolder.py` & `dagster-1.7.6/dagster/_cli/config_scaffolder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_cli/debug.py` & `dagster-1.7.6/dagster/_cli/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_cli/dev.py` & `dagster-1.7.6/dagster/_cli/dev.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_cli/instance.py` & `dagster-1.7.6/dagster/_cli/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_cli/job.py` & `dagster-1.7.6/dagster/_cli/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -767,15 +767,17 @@
         for partition_data in partition_execution_data.partition_data:
             dagster_run = create_backfill_run(
                 instance,
                 code_location,
                 external_job,
                 job_partition_set,
                 backfill_job,
-                partition_data,
+                partition_data.name,
+                partition_data.tags,
+                partition_data.run_config,
             )
             if dagster_run:
                 instance.submit_run(dagster_run.run_id, workspace)
 
         instance.add_backfill(backfill_job.with_status(BulkActionStatus.COMPLETED))
 
         print_fn(f"Launched backfill job `{backfill_id}`")
```

### Comparing `dagster-1.7.5/dagster/_cli/load_handle.py` & `dagster-1.7.6/dagster/_cli/load_handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_cli/project.py` & `dagster-1.7.6/dagster/_cli/project.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_cli/run.py` & `dagster-1.7.6/dagster/_cli/run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_cli/schedule.py` & `dagster-1.7.6/dagster/_cli/schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_cli/sensor.py` & `dagster-1.7.6/dagster/_cli/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_cli/utils.py` & `dagster-1.7.6/dagster/_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_cli/workspace/cli_target.py` & `dagster-1.7.6/dagster/_cli/workspace/cli_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/__init__.py` & `dagster-1.7.6/dagster/_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/config_schema.py` & `dagster-1.7.6/dagster/_config/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/config_type.py` & `dagster-1.7.6/dagster/_config/config_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/errors.py` & `dagster-1.7.6/dagster/_config/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/evaluate_value_result.py` & `dagster-1.7.6/dagster/_config/evaluate_value_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/field.py` & `dagster-1.7.6/dagster/_config/field.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/field_utils.py` & `dagster-1.7.6/dagster/_config/field_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/post_process.py` & `dagster-1.7.6/dagster/_config/post_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/primitive_mapping.py` & `dagster-1.7.6/dagster/_config/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/pythonic_config/__init__.py` & `dagster-1.7.6/dagster/_config/pythonic_config/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/pythonic_config/attach_other_object_to_context.py` & `dagster-1.7.6/dagster/_config/pythonic_config/attach_other_object_to_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/pythonic_config/config.py` & `dagster-1.7.6/dagster/_config/pythonic_config/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/pythonic_config/conversion_utils.py` & `dagster-1.7.6/dagster/_config/pythonic_config/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/pythonic_config/io_manager.py` & `dagster-1.7.6/dagster/_config/pythonic_config/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/pythonic_config/resource.py` & `dagster-1.7.6/dagster/_config/pythonic_config/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/pythonic_config/type_check_utils.py` & `dagster-1.7.6/dagster/_config/pythonic_config/type_check_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/pythonic_config/typing_utils.py` & `dagster-1.7.6/dagster/_config/pythonic_config/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/snap.py` & `dagster-1.7.6/dagster/_config/snap.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/source.py` & `dagster-1.7.6/dagster/_config/source.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/stack.py` & `dagster-1.7.6/dagster/_config/stack.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/traversal_context.py` & `dagster-1.7.6/dagster/_config/traversal_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/type_printer.py` & `dagster-1.7.6/dagster/_config/type_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_config/validate.py` & `dagster-1.7.6/dagster/_config/validate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/asset_graph_view/asset_graph_view.py` & `dagster-1.7.6/dagster/_core/asset_graph_view/asset_graph_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     NewType,
     Optional,
     Sequence,
 )
 
 from dagster import _check as check
 from dagster._core.definitions.asset_subset import AssetSubset, ValidAssetSubset
-from dagster._core.definitions.events import AssetKey
+from dagster._core.definitions.events import AssetKey, AssetKeyPartitionKey
 from dagster._core.definitions.multi_dimensional_partitions import (
     MultiPartitionKey,
     MultiPartitionsDefinition,
     PartitionDimensionDefinition,
 )
 from dagster._core.definitions.partition import (
     AllPartitionsSubset,
@@ -123,14 +123,19 @@
     # only works for partitioned assets for now
     def compute_partition_keys(self) -> AbstractSet[str]:
         return {
             check.not_none(akpk.partition_key, "No None partition keys")
             for akpk in self._compatible_subset.asset_partitions
         }
 
+    def expensively_compute_asset_partitions(self) -> AbstractSet[AssetKeyPartitionKey]:
+        # this method requires computing all partition keys of the definition, which
+        # may be expensive
+        return self._compatible_subset.asset_partitions
+
     @property
     def asset_key(self) -> AssetKey:
         return self._compatible_subset.asset_key
 
     @property
     def parent_keys(self) -> AbstractSet[AssetKey]:
         return self._asset_graph_view.asset_graph.get(self.asset_key).parent_keys
@@ -333,43 +338,43 @@
                 asset_key=asset_key,
                 partitions_def=self._get_partitions_def(asset_key),
                 dynamic_partitions_store=self._queryer,
                 current_time=self.effective_dt,
             ),
         )
 
-    def get_asset_slice_from_subset(self, subset: AssetSubset) -> "AssetSlice":
+    def get_asset_slice_from_subset(self, subset: AssetSubset) -> Optional["AssetSlice"]:
+        if subset.is_compatible_with_partitions_def(self._get_partitions_def(subset.asset_key)):
+            return _slice_from_subset(self, subset)
+        else:
+            return None
+
+    def get_asset_slice_from_valid_subset(self, subset: ValidAssetSubset) -> "AssetSlice":
         return _slice_from_subset(self, subset)
 
-    def compute_missing_subslice(
-        self, asset_key: "AssetKey", from_slice: "AssetSlice"
+    def get_asset_slice_from_asset_partitions(
+        self, asset_partitions: AbstractSet[AssetKeyPartitionKey]
     ) -> "AssetSlice":
-        """Returns a slice which is the subset of the input slice that has never been materialized
-        (if it is a materializable asset) or observered (if it is an observable asset).
-        """
-        # TODO: this logic should be simplified once we have a unified way of detecting both
-        # materializations and observations through the parittion status cache. at that point, the
-        # definition will slightly change to search for materializations and observations regardless
-        # of the materializability of the asset
-        if self.asset_graph.get(asset_key).is_materializable:
-            # cheap call which takes advantage of the partition status cache
-            materialized_subset = self._queryer.get_materialized_asset_subset(asset_key=asset_key)
-            materialized_slice = self.get_asset_slice_from_subset(materialized_subset)
-            return from_slice.compute_difference(materialized_slice)
-        else:
-            # more expensive call
-            missing_asset_partitions = {
-                ap
-                for ap in from_slice.convert_to_valid_asset_subset().asset_partitions
-                if not self._queryer.asset_partition_has_materialization_or_observation(ap)
-            }
-            missing_subset = ValidAssetSubset.from_asset_partitions_set(
-                asset_key, self._get_partitions_def(asset_key), missing_asset_partitions
-            )
-            return self.get_asset_slice_from_subset(missing_subset)
+        asset_keys = {akpk.asset_key for akpk in asset_partitions}
+        check.invariant(len(asset_keys) == 1, "Must have exactly one asset key")
+        asset_key = asset_keys.pop()
+        return _slice_from_subset(
+            self,
+            ValidAssetSubset.from_asset_partitions_set(
+                asset_key=asset_key,
+                partitions_def=self._get_partitions_def(asset_key),
+                asset_partitions_set=asset_partitions,
+            ),
+        )
+
+    def create_empty_slice(self, asset_key: AssetKey) -> AssetSlice:
+        return _slice_from_subset(
+            self,
+            AssetSubset.empty(asset_key, self._get_partitions_def(asset_key)),
+        )
 
     def compute_parent_asset_slice(
         self, parent_asset_key: AssetKey, asset_slice: AssetSlice
     ) -> AssetSlice:
         return _slice_from_subset(
             self,
             self.asset_graph.get_parent_asset_subset(
@@ -389,19 +394,14 @@
                 dynamic_partitions_store=self._queryer,
                 child_asset_key=child_asset_key,
                 current_time=self.effective_dt,
                 parent_asset_subset=asset_slice.convert_to_valid_asset_subset(),
             ),
         )
 
-    def compute_in_progress_asset_slice(self, asset_key: "AssetKey") -> "AssetSlice":
-        return _slice_from_subset(
-            self, self._queryer.get_in_progress_asset_subset(asset_key=asset_key)
-        )
-
     def compute_intersection_with_partition_keys(
         self, partition_keys: AbstractSet[str], asset_slice: AssetSlice
     ) -> "AssetSlice":
         """Return a new AssetSlice with only the given partition keys if they are in the slice."""
         partitions_def = check.not_none(
             self._get_partitions_def(asset_slice.asset_key), "Must have partitions def"
         )
@@ -460,20 +460,73 @@
         elif isinstance(partitions_def, MultiPartitionsDefinition):
             return self._build_multi_partition_slice(
                 asset_key, self._get_multi_dim_info(asset_key), time_window
             )
         else:
             check.failed(f"Unsupported partitions_def: {partitions_def}")
 
-    def create_empty_slice(self, asset_key: AssetKey) -> AssetSlice:
+    def compute_missing_subslice(
+        self, asset_key: "AssetKey", from_slice: "AssetSlice"
+    ) -> "AssetSlice":
+        """Returns a slice which is the subset of the input slice that has never been materialized
+        (if it is a materializable asset) or observered (if it is an observable asset).
+        """
+        # TODO: this logic should be simplified once we have a unified way of detecting both
+        # materializations and observations through the parittion status cache. at that point, the
+        # definition will slightly change to search for materializations and observations regardless
+        # of the materializability of the asset
+        if self.asset_graph.get(asset_key).is_materializable:
+            # cheap call which takes advantage of the partition status cache
+            materialized_subset = self._queryer.get_materialized_asset_subset(asset_key=asset_key)
+            materialized_slice = self.get_asset_slice_from_valid_subset(materialized_subset)
+            return from_slice.compute_difference(materialized_slice)
+        else:
+            # more expensive call
+            missing_asset_partitions = {
+                ap
+                for ap in from_slice.convert_to_valid_asset_subset().asset_partitions
+                if not self._queryer.asset_partition_has_materialization_or_observation(ap)
+            }
+            missing_subset = ValidAssetSubset.from_asset_partitions_set(
+                asset_key, self._get_partitions_def(asset_key), missing_asset_partitions
+            )
+            return self.get_asset_slice_from_valid_subset(missing_subset)
+
+    @cached_method
+    def compute_in_progress_asset_slice(self, *, asset_key: "AssetKey") -> "AssetSlice":
         return _slice_from_subset(
-            self,
-            AssetSubset.empty(asset_key, self._get_partitions_def(asset_key)),
+            self, self._queryer.get_in_progress_asset_subset(asset_key=asset_key)
         )
 
+    @cached_method
+    def compute_failed_asset_slice(self, *, asset_key: "AssetKey") -> "AssetSlice":
+        return _slice_from_subset(self, self._queryer.get_failed_asset_subset(asset_key=asset_key))
+
+    @cached_method
+    def compute_updated_since_cursor_slice(
+        self, *, asset_key: AssetKey, cursor: Optional[int]
+    ) -> AssetSlice:
+        subset = self._queryer.get_asset_subset_updated_after_cursor(
+            asset_key=asset_key, after_cursor=cursor
+        )
+        return self.get_asset_slice_from_valid_subset(subset)
+
+    @cached_method
+    def compute_parent_updated_since_cursor_slice(
+        self, *, asset_key: AssetKey, cursor: Optional[int]
+    ) -> AssetSlice:
+        result_slice = self.create_empty_slice(asset_key)
+        for parent_key in self.asset_graph.get(asset_key).parent_keys:
+            result_slice = result_slice.compute_union(
+                self.compute_updated_since_cursor_slice(
+                    asset_key=parent_key, cursor=cursor
+                ).compute_child_slice(asset_key)
+            )
+        return result_slice
+
     class MultiDimInfo(NamedTuple):
         tw_dim: PartitionDimensionDefinition
         secondary_dim: PartitionDimensionDefinition
 
         @property
         def tw_partition_def(self) -> TimeWindowPartitionsDefinition:
             return check.inst(
@@ -525,13 +578,7 @@
                 )
                 for secondary_pk in multi_dim_info.secondary_partition_def.get_partition_keys(
                     current_time=self.effective_dt,
                     dynamic_partitions_store=self._queryer,
                 )
             }
         )
-
-
-def _required_tw_partitions_def(
-    partitions_def: Optional["PartitionsDefinition"],
-) -> TimeWindowPartitionsDefinition:
-    return check.inst(partitions_def, TimeWindowPartitionsDefinition, "Must be time windowed.")
```

### Comparing `dagster-1.7.5/dagster/_core/assets.py` & `dagster-1.7.6/dagster/_core/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/code_pointer.py` & `dagster-1.7.6/dagster/_core/code_pointer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/container_context/config.py` & `dagster-1.7.6/dagster/_core/container_context/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/debug.py` & `dagster-1.7.6/dagster/_core/debug.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/decorator_utils.py` & `dagster-1.7.6/dagster/_core/decorator_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/__init__.py` & `dagster-1.7.6/dagster/_core/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_check_evaluation.py` & `dagster-1.7.6/dagster/_core/definitions/asset_check_evaluation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_check_factories/freshness_checks/last_update.py` & `dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/last_update.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py` & `dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py` & `dagster-1.7.6/dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_check_factories/schema_change_checks.py` & `dagster-1.7.6/dagster/_core/definitions/asset_check_factories/schema_change_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_check_factories/utils.py` & `dagster-1.7.6/dagster/_core/definitions/asset_check_factories/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_check_result.py` & `dagster-1.7.6/dagster/_core/definitions/asset_check_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_check_spec.py` & `dagster-1.7.6/dagster/_core/definitions/asset_check_spec.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_checks.py` & `dagster-1.7.6/dagster/_core/definitions/asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_daemon_context.py` & `dagster-1.7.6/dagster/_core/definitions/asset_daemon_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_daemon_cursor.py` & `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/serialized_objects.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,286 +1,257 @@
-import dataclasses
-import json
 from dataclasses import dataclass
-from functools import cached_property
 from typing import (
     TYPE_CHECKING,
+    AbstractSet,
+    Dict,
+    FrozenSet,
     Mapping,
-    NamedTuple,
     Optional,
     Sequence,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
 )
 
-from dagster._core.definitions.asset_graph_subset import AssetGraphSubset
-from dagster._core.definitions.asset_subset import AssetSubset
+from dagster._core.definitions.asset_subset import AssetSubset, ValidAssetSubset
 from dagster._core.definitions.events import AssetKey
-from dagster._serdes.serdes import (
-    FieldSerializer,
-    JsonSerializableValue,
-    PackableValue,
-    SerializableNonScalarKeyMapping,
-    UnpackContext,
-    WhitelistMap,
-    pack_value,
-    unpack_value,
-    whitelist_for_serdes,
-)
-
-from .base_asset_graph import BaseAssetGraph
-from .declarative_scheduling.serialized_objects import (
-    AssetConditionEvaluation,
-    AssetConditionEvaluationState,
-)
+from dagster._core.definitions.metadata import MetadataMapping, MetadataValue
+from dagster._core.definitions.partition import AllPartitionsSubset
+from dagster._model import DagsterModel
+from dagster._serdes.serdes import whitelist_for_serdes
 
 if TYPE_CHECKING:
-    from .declarative_scheduling.serialized_objects import (
-        AssetConditionSnapshot,
+    from dagster._core.definitions.declarative_scheduling.scheduling_condition import (
+        SchedulingResult,
     )
+    from dagster._core.definitions.declarative_scheduling.scheduling_context import (
+        SchedulingContext,
+    )
+
+T = TypeVar("T")
 
 
 @whitelist_for_serdes
-class AssetConditionCursorExtras(NamedTuple):
-    """Represents additional state that may be optionally saved by an AssetCondition between
-    evaluations.
+class HistoricalAllPartitionsSubsetSentinel(DagsterModel):
+    """Serializable indicator that this value was an AllPartitionsSubset at serialization time, but
+    the partitions may have changed since that time.
     """
 
-    condition_snapshot: "AssetConditionSnapshot"
-    extras: Mapping[str, PackableValue]
 
+def get_serializable_candidate_subset(
+    candidate_subset: Union[AssetSubset, HistoricalAllPartitionsSubsetSentinel],
+) -> Union[AssetSubset, HistoricalAllPartitionsSubsetSentinel]:
+    """Do not serialize the candidate subset directly if it is an AllPartitionsSubset."""
+    if isinstance(candidate_subset, AssetSubset) and isinstance(
+        candidate_subset.value, AllPartitionsSubset
+    ):
+        return HistoricalAllPartitionsSubsetSentinel()
+    return candidate_subset
 
-class ObserveRequestTimestampSerializer(FieldSerializer):
-    def pack(
-        self,
-        mapping: Mapping[str, float],
-        whitelist_map: WhitelistMap,
-        descent_path: str,
-    ) -> JsonSerializableValue:
-        return pack_value(SerializableNonScalarKeyMapping(mapping), whitelist_map, descent_path)
-
-    def unpack(
-        self,
-        unpacked_value: JsonSerializableValue,
-        whitelist_map: WhitelistMap,
-        context: UnpackContext,
-    ) -> PackableValue:
-        return unpack_value(unpacked_value, dict, whitelist_map, context)
-
-
-@whitelist_for_serdes(
-    field_serializers={
-        "last_observe_request_timestamp_by_asset_key": ObserveRequestTimestampSerializer
-    }
-)
-@dataclass(frozen=True)
-class AssetDaemonCursor:
-    """State that's stored between daemon evaluations.
 
-    Attributes:
-        evaluation_id (int): The ID of the evaluation that produced this cursor.
-        previous_evaluation_state (Sequence[AssetConditionEvaluationInfo]): The evaluation info
-            recorded for each asset on the previous tick.
-    """
+@whitelist_for_serdes
+class AssetConditionSnapshot(DagsterModel):
+    """A serializable snapshot of a node in the AutomationCondition tree."""
 
-    evaluation_id: int
-    previous_evaluation_state: Sequence["AssetConditionEvaluationState"]
+    class_name: str
+    description: str
+    unique_id: str
 
-    last_observe_request_timestamp_by_asset_key: Mapping[AssetKey, float]
 
-    @staticmethod
-    def empty(evaluation_id: int = 0) -> "AssetDaemonCursor":
-        return AssetDaemonCursor(
-            evaluation_id=evaluation_id,
-            previous_evaluation_state=[],
-            last_observe_request_timestamp_by_asset_key={},
-        )
+@whitelist_for_serdes
+class AssetSubsetWithMetadata(DagsterModel):
+    """An asset subset with metadata that corresponds to it."""
 
-    @cached_property
-    def previous_evaluation_state_by_key(
-        self,
-    ) -> Mapping[AssetKey, "AssetConditionEvaluationState"]:
-        """Efficient lookup of previous evaluation info by asset key."""
-        return {
-            evaluation_state.asset_key: evaluation_state
-            for evaluation_state in self.previous_evaluation_state
-        }
-
-    def get_previous_evaluation_state(
-        self, asset_key: AssetKey
-    ) -> Optional["AssetConditionEvaluationState"]:
-        """Returns the AssetConditionCursor associated with the given asset key. If no stored
-        cursor exists, returns an empty cursor.
-        """
-        return self.previous_evaluation_state_by_key.get(asset_key)
+    subset: AssetSubset
+    metadata: MetadataMapping
 
-    def get_previous_evaluation(self, asset_key: AssetKey) -> Optional["AssetConditionEvaluation"]:
-        """Returns the previous AssetConditionEvaluation for a given asset key, if it exists."""
-        previous_evaluation_state = self.get_previous_evaluation_state(asset_key)
-        return previous_evaluation_state.previous_evaluation if previous_evaluation_state else None
-
-    def with_updates(
-        self,
-        evaluation_id: int,
-        evaluation_timestamp: float,
-        newly_observe_requested_asset_keys: Sequence[AssetKey],
-        evaluation_state: Sequence["AssetConditionEvaluationState"],
-    ) -> "AssetDaemonCursor":
-        return dataclasses.replace(
-            self,
-            evaluation_id=evaluation_id,
-            previous_evaluation_state=evaluation_state,
-            last_observe_request_timestamp_by_asset_key={
-                **self.last_observe_request_timestamp_by_asset_key,
-                **{
-                    asset_key: evaluation_timestamp
-                    for asset_key in newly_observe_requested_asset_keys
-                },
-            },
-        )
+    @property
+    def frozen_metadata(self) -> FrozenSet[Tuple[str, MetadataValue]]:
+        return frozenset(self.metadata.items())
 
-    def __hash__(self) -> int:
-        return hash(id(self))
 
+@whitelist_for_serdes
+class AssetConditionEvaluation(DagsterModel):
+    """Serializable representation of the results of evaluating a node in the evaluation tree."""
 
-# BACKCOMPAT
+    condition_snapshot: AssetConditionSnapshot
+    start_timestamp: Optional[float]
+    end_timestamp: Optional[float]
+
+    true_subset: AssetSubset
+    candidate_subset: Union[AssetSubset, HistoricalAllPartitionsSubsetSentinel]
+    subsets_with_metadata: Sequence[AssetSubsetWithMetadata]
+
+    child_evaluations: Sequence["AssetConditionEvaluation"]
+
+    @property
+    def asset_key(self) -> AssetKey:
+        return self.true_subset.asset_key
 
+    @staticmethod
+    def from_result(result: "SchedulingResult") -> "AssetConditionEvaluation":
+        return AssetConditionEvaluation(
+            condition_snapshot=result.condition.get_snapshot(result.condition_unique_id),
+            start_timestamp=result.start_timestamp,
+            end_timestamp=result.end_timestamp,
+            true_subset=result.true_subset,
+            candidate_subset=get_serializable_candidate_subset(result.candidate_subset),
+            subsets_with_metadata=result.subsets_with_metadata,
+            child_evaluations=[
+                AssetConditionEvaluation.from_result(child_result)
+                for child_result in result.child_results
+            ],
+        )
 
-def get_backcompat_asset_condition_evaluation_state(
-    latest_evaluation: "AssetConditionEvaluation",
-    latest_storage_id: Optional[int],
-    latest_timestamp: Optional[float],
-    handled_root_subset: Optional[AssetSubset],
-) -> "AssetConditionEvaluationState":
-    """Generates an AssetDaemonCursor from information available on the old cursor format."""
-    from dagster._core.definitions.auto_materialize_rule_impls import MaterializeOnMissingRule
-    from dagster._core.definitions.declarative_scheduling.legacy.rule_condition import (
-        RuleCondition,
-    )
-    from dagster._core.definitions.declarative_scheduling.serialized_objects import (
-        AssetConditionEvaluationState,
-    )
+    def equivalent_to_stored_evaluation(self, other: Optional["AssetConditionEvaluation"]) -> bool:
+        """Returns if this evaluation is functionally equivalent to the given stored evaluation.
+        This is used to determine if it is necessary to store this new evaluation in the database.
+        Noteably, the timestamps on successive evaluations will always be different, so a simple
+        equality check would be too strict.
+        """
+        return (
+            other is not None
+            and self.condition_snapshot == other.condition_snapshot
+            and self.true_subset == other.true_subset
+            # the candidate subset gets modified during serialization
+            and get_serializable_candidate_subset(self.candidate_subset)
+            == get_serializable_candidate_subset(other.candidate_subset)
+            and self.subsets_with_metadata == other.subsets_with_metadata
+            and len(self.child_evaluations) == len(other.child_evaluations)
+            and all(
+                self_child.equivalent_to_stored_evaluation(other_child)
+                for self_child, other_child in zip(self.child_evaluations, other.child_evaluations)
+            )
+        )
 
-    return AssetConditionEvaluationState(
-        previous_evaluation=latest_evaluation,
-        previous_tick_evaluation_timestamp=latest_timestamp,
-        max_storage_id=latest_storage_id,
-        # the only information we need to preserve from the previous cursor is the handled subset
-        extra_state_by_unique_id={
-            RuleCondition(rule=MaterializeOnMissingRule()).get_unique_id(None): handled_root_subset,
-        }
-        if handled_root_subset and handled_root_subset.size > 0
-        else {},
-    )
+    def discarded_subset(self) -> Optional[AssetSubset]:
+        """Returns the AssetSubset representing asset partitions that were discarded during this
+        evaluation. Note that 'discarding' is a deprecated concept that is only used for backwards
+        compatibility.
+        """
+        if len(self.child_evaluations) != 3:
+            return None
+        not_discard_evaluation = self.child_evaluations[-1]
+        discard_evaluation = not_discard_evaluation.child_evaluations[0]
+        return discard_evaluation.true_subset
+
+    def get_requested_or_discarded_subset(self) -> AssetSubset:
+        discarded_subset = self.discarded_subset()
+        if discarded_subset is None:
+            return self.true_subset
+        else:
+            # the true_subset and discarded_subset were created on the same tick, so they are
+            # guaranteed to be compatible with each other
+            return (
+                ValidAssetSubset(asset_key=self.asset_key, value=self.true_subset.value)
+                | discarded_subset
+            )
+
+    def for_child(self, child_unique_id: str) -> Optional["AssetConditionEvaluation"]:
+        """Returns the evaluation of a given child condition by finding the child evaluation that
+        has an identical hash to the given condition.
+        """
+        for child_evaluation in self.child_evaluations:
+            if child_evaluation.condition_snapshot.unique_id == child_unique_id:
+                return child_evaluation
+
+        return None
+
+    def with_run_ids(self, run_ids: AbstractSet[str]) -> "AssetConditionEvaluationWithRunIds":
+        return AssetConditionEvaluationWithRunIds(evaluation=self, run_ids=frozenset(run_ids))
+
+    def legacy_num_skipped(self) -> int:
+        if len(self.child_evaluations) < 2:
+            return 0
+
+        not_skip_evaluation = self.child_evaluations[-1]
+        skip_evaluation = not_skip_evaluation.child_evaluations[0]
+        return skip_evaluation.true_subset.size - self.legacy_num_discarded()
+
+    def legacy_num_discarded(self) -> int:
+        discarded_subset = self.discarded_subset()
+        if discarded_subset is None:
+            return 0
+        return discarded_subset.size
 
 
-def backcompat_deserialize_asset_daemon_cursor_str(
-    cursor_str: str, asset_graph: Optional[BaseAssetGraph], default_evaluation_id: int
-) -> AssetDaemonCursor:
-    """This serves as a backcompat layer for deserializing the old cursor format. Some information
-    is impossible to fully recover, this will recover enough to continue operating as normal.
+@whitelist_for_serdes
+class AssetConditionEvaluationWithRunIds(DagsterModel):
+    """A union of an AssetConditionEvaluation and the set of run IDs that have been launched in
+    response to it.
     """
-    from .auto_materialize_rule_evaluation import (
-        deserialize_auto_materialize_asset_evaluation_to_asset_condition_evaluation_with_run_ids,
-    )
-    from .declarative_scheduling.serialized_objects import (
-        AssetConditionSnapshot,
-    )
 
-    data = json.loads(cursor_str)
+    evaluation: AssetConditionEvaluation
+    run_ids: FrozenSet[str]
 
-    if isinstance(data, list):
-        evaluation_id = data[0] if isinstance(data[0], int) else default_evaluation_id
-        return AssetDaemonCursor.empty(evaluation_id)
-    elif not isinstance(data, dict):
-        return AssetDaemonCursor.empty(default_evaluation_id)
-    elif asset_graph is None:
-        return AssetDaemonCursor.empty(data.get("evaluation_id", default_evaluation_id))
+    @property
+    def asset_key(self) -> AssetKey:
+        return self.evaluation.asset_key
+
+    @property
+    def num_requested(self) -> int:
+        return self.evaluation.true_subset.size
 
-    serialized_last_observe_request_timestamp_by_asset_key = data.get(
-        "last_observe_request_timestamp_by_asset_key", {}
-    )
-    last_observe_request_timestamp_by_asset_key = {
-        AssetKey.from_user_string(key_str): timestamp
-        for key_str, timestamp in serialized_last_observe_request_timestamp_by_asset_key.items()
-    }
-
-    partition_subsets_by_asset_key = {}
-    for key_str, serialized_str in data.get("handled_root_partitions_by_asset_key", {}).items():
-        asset_key = AssetKey.from_user_string(key_str)
-        partitions_def = asset_graph.get(asset_key).partitions_def if asset_graph else None
-        if not partitions_def:
-            continue
-        try:
-            partition_subsets_by_asset_key[asset_key] = partitions_def.deserialize_subset(
-                serialized_str
-            )
-        except:
-            continue
 
-    handled_root_asset_graph_subset = AssetGraphSubset(
-        non_partitioned_asset_keys={
-            AssetKey.from_user_string(key_str)
-            for key_str in data.get("handled_root_asset_keys", set())
-        },
-        partitions_subsets_by_asset_key=partition_subsets_by_asset_key,
-    )
+@whitelist_for_serdes
+@dataclass(frozen=True)
+class AssetConditionEvaluationState:
+    """Incremental state calculated during the evaluation of an AssetCondition. This may be used
+    on the subsequent evaluation to make the computation more efficient.
 
-    serialized_latest_evaluation_by_asset_key = data.get("latest_evaluation_by_asset_key", {})
-    latest_evaluation_by_asset_key = {}
-    for key_str, serialized_evaluation in serialized_latest_evaluation_by_asset_key.items():
-        key = AssetKey.from_user_string(key_str)
-        partitions_def = asset_graph.get(key).partitions_def if asset_graph else None
-
-        evaluation = deserialize_auto_materialize_asset_evaluation_to_asset_condition_evaluation_with_run_ids(
-            serialized_evaluation, partitions_def
-        ).evaluation
-
-        latest_evaluation_by_asset_key[key] = evaluation
-
-    previous_evaluation_state = []
-    cursor_keys = (
-        asset_graph.materializable_asset_keys
-        if asset_graph
-        else latest_evaluation_by_asset_key.keys()
-    )
-    for asset_key in cursor_keys:
-        latest_evaluation_result = latest_evaluation_by_asset_key.get(asset_key)
-        # create a placeholder evaluation result if we don't have one
-        if not latest_evaluation_result:
-            partitions_def = asset_graph.get(asset_key).partitions_def if asset_graph else None
-            latest_evaluation_result = AssetConditionEvaluation(
-                condition_snapshot=AssetConditionSnapshot(
-                    class_name="", description="", unique_id=""
-                ),
-                true_subset=AssetSubset.empty(asset_key, partitions_def),
-                candidate_subset=AssetSubset.empty(asset_key, partitions_def),
-                start_timestamp=None,
-                end_timestamp=None,
-                subsets_with_metadata=[],
-                child_evaluations=[],
-            )
-        backcompat_evaluation_state = get_backcompat_asset_condition_evaluation_state(
-            latest_evaluation_result,
-            data.get("latest_storage_id"),
-            data.get("latest_evaluation_timestamp"),
-            handled_root_asset_graph_subset.get_asset_subset(asset_key, asset_graph)
-            if asset_graph
-            else None,
-        )
-        previous_evaluation_state.append(backcompat_evaluation_state)
+    Attributes:
+        previous_evaluation: The computed AssetConditionEvaluation.
+        previous_tick_evaluation_timestamp: The evaluation_timestamp at which the evaluation was performed.
+        max_storage_id: The maximum storage ID over all events used in this computation.
+        extra_state_by_unique_id: A mapping from the unique ID of each condition in the evaluation
+            tree to the extra state that was calculated for it, if any.
+    """
 
-    return AssetDaemonCursor(
-        evaluation_id=data.get("evaluation_id") or default_evaluation_id,
-        previous_evaluation_state=previous_evaluation_state,
-        last_observe_request_timestamp_by_asset_key=last_observe_request_timestamp_by_asset_key,
-    )
+    previous_evaluation: AssetConditionEvaluation
+    previous_tick_evaluation_timestamp: Optional[float]
 
+    max_storage_id: Optional[int]
+    extra_state_by_unique_id: Mapping[str, Optional[Union[AssetSubset, Sequence[AssetSubset]]]]
 
-@whitelist_for_serdes
-class LegacyAssetDaemonCursorWrapper(NamedTuple):
-    """Wrapper class for the legacy AssetDaemonCursor object, which is not a serializable NamedTuple."""
+    @property
+    def asset_key(self) -> AssetKey:
+        return self.previous_evaluation.asset_key
+
+    @property
+    def true_subset(self) -> AssetSubset:
+        return self.previous_evaluation.true_subset
 
-    serialized_cursor: str
+    @staticmethod
+    def create(
+        context: "SchedulingContext", root_result: "SchedulingResult"
+    ) -> "AssetConditionEvaluationState":
+        """Convenience constructor to generate an AssetConditionEvaluationState from the root result
+        and the context in which it was evaluated.
+        """
 
-    def get_asset_daemon_cursor(self, asset_graph: Optional[BaseAssetGraph]) -> AssetDaemonCursor:
-        return backcompat_deserialize_asset_daemon_cursor_str(
-            self.serialized_cursor, asset_graph, 0
+        # flatten the extra state into a single dict
+        def _flatten_extra_state(
+            r: "SchedulingResult",
+        ) -> Mapping[str, Optional[Union[AssetSubset, Sequence[AssetSubset]]]]:
+            extra_state: Dict[str, Optional[Union[AssetSubset, Sequence[AssetSubset]]]] = (
+                {r.condition_unique_id: r.extra_state} if r.extra_state else {}
+            )
+            for child in r.child_results:
+                extra_state.update(_flatten_extra_state(child))
+            return extra_state
+
+        return AssetConditionEvaluationState(
+            previous_evaluation=AssetConditionEvaluation.from_result(root_result),
+            previous_tick_evaluation_timestamp=context.asset_graph_view.effective_dt.timestamp(),
+            max_storage_id=context.new_max_storage_id,
+            extra_state_by_unique_id=_flatten_extra_state(root_result),
         )
+
+    def get_extra_state(self, unique_id: str, as_type: Type[T]) -> Optional[T]:
+        """Returns the value from the extras dict for the given condition, if it exists and is of
+        the expected type. Otherwise, returns None.
+        """
+        extra_state = self.extra_state_by_unique_id.get(unique_id)
+        if isinstance(extra_state, as_type):
+            return extra_state
+        return None
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_dep.py` & `dagster-1.7.6/dagster/_core/definitions/asset_dep.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_graph.py` & `dagster-1.7.6/dagster/_core/definitions/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_graph_differ.py` & `dagster-1.7.6/dagster/_core/definitions/asset_graph_differ.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_graph_subset.py` & `dagster-1.7.6/dagster/_core/definitions/asset_graph_subset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_in.py` & `dagster-1.7.6/dagster/_core/definitions/asset_in.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_job.py` & `dagster-1.7.6/dagster/_core/definitions/asset_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_key.py` & `dagster-1.7.6/dagster/_core/definitions/asset_key.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_layer.py` & `dagster-1.7.6/dagster/_core/definitions/asset_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_out.py` & `dagster-1.7.6/dagster/_core/definitions/asset_out.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_selection.py` & `dagster-1.7.6/dagster/_core/definitions/asset_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_sensor_definition.py` & `dagster-1.7.6/dagster/_core/definitions/asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_spec.py` & `dagster-1.7.6/dagster/_core/definitions/asset_spec.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/asset_subset.py` & `dagster-1.7.6/dagster/_core/definitions/asset_subset.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     AllPartitionsSubset,
     PartitionsDefinition,
     PartitionsSubset,
 )
 from dagster._core.definitions.time_window_partitions import (
     BaseTimeWindowPartitionsSubset,
 )
-from dagster._model import DagsterModel
+from dagster._model import DagsterModel, InstanceOf
 from dagster._serdes.serdes import (
     PydanticModelSerializer,
     whitelist_for_serdes,
 )
 
 if TYPE_CHECKING:
     from dagster._core.instance import DynamicPartitionsStore
@@ -35,27 +35,29 @@
 
     def get_storage_name(self) -> str:
         # override this method so all ValidAssetSubsets are serialzied as AssetSubsets
         return "AssetSubset"
 
     def before_pack(self, value: "AssetSubset") -> "AssetSubset":
         if value.is_partitioned:
-            return value.copy(update={"value": value.subset_value.to_serializable_subset()})
+            return value.model_copy(update={"value": value.subset_value.to_serializable_subset()})
         return value
 
 
 @whitelist_for_serdes(serializer=AssetSubsetSerializer)
 class AssetSubset(DagsterModel):
     """Represents a set of AssetKeyPartitionKeys for a given AssetKey. For partitioned assets, this
     class uses a PartitionsSubset to represent the set of partitions, enabling lazy evaluation of the
     underlying partition keys. For unpartitioned assets, this class uses a bool to represent whether
     the asset is present or not.
     """
 
-    asset_key: AssetKey
+    # use InstanceOf to tell pydantic to just do an instanceof check instead of the default
+    # costly NamedTuple validation and reconstruction
+    asset_key: InstanceOf[AssetKey]
     value: Union[bool, PartitionsSubset]
 
     @property
     def is_partitioned(self) -> bool:
         return not isinstance(self.value, bool)
 
     @property
@@ -215,34 +217,34 @@
         self,
         partitions_def: Optional[PartitionsDefinition],
         current_time: Optional[datetime.datetime] = None,
         dynamic_partitions_store: Optional["DynamicPartitionsStore"] = None,
     ) -> "ValidAssetSubset":
         """Returns the AssetSubset containing all asset partitions which are not in this AssetSubset."""
         if partitions_def is None:
-            return self.copy(update={"value": not self.bool_value})
+            return self.model_copy(update={"value": not self.bool_value})
         else:
             value = partitions_def.subset_with_partition_keys(
                 self.subset_value.get_partition_keys_not_in_subset(
                     partitions_def,
                     current_time=current_time,
                     dynamic_partitions_store=dynamic_partitions_store,
                 )
             )
-            return self.copy(update={"value": value})
+            return self.model_copy(update={"value": value})
 
     def _oper(self, other: "ValidAssetSubset", oper: Callable[..., Any]) -> "ValidAssetSubset":
         value = oper(self.value, other.value)
-        return self.copy(update={"value": value})
+        return self.model_copy(update={"value": value})
 
     def __sub__(self, other: AssetSubset) -> "ValidAssetSubset":
         """Returns an AssetSubset representing self.asset_partitions - other.asset_partitions."""
         valid_other = self.get_valid(other)
         if not self.is_partitioned:
-            return self.copy(update={"value": self.bool_value and not valid_other.bool_value})
+            return self.model_copy(update={"value": self.bool_value and not valid_other.bool_value})
         return self._oper(valid_other, operator.sub)
 
     def __and__(self, other: AssetSubset) -> "ValidAssetSubset":
         """Returns an AssetSubset representing self.asset_partitions & other.asset_partitions."""
         return self._oper(self.get_valid(other), operator.and_)
 
     def __or__(self, other: AssetSubset) -> "ValidAssetSubset":
@@ -252,15 +254,15 @@
     def get_valid(self, other: AssetSubset) -> "ValidAssetSubset":
         """Creates a ValidAssetSubset from the given AssetSubset by returning a copy of the given
         AssetSubset if it is compatible with this AssetSubset, otherwise returns an empty subset.
         """
         if self._is_compatible_with_subset(other):
             return ValidAssetSubset(asset_key=other.asset_key, value=other.value)
         else:
-            return self.copy(
+            return self.model_copy(
                 # unfortunately, this is the best way to get an empty partitions subset of an unknown
                 # type if you don't have access to the partitions definition
                 update={
                     "value": (self.subset_value - self.subset_value)
                     if self.is_partitioned
                     else False
                 }
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/assets.py` & `dagster-1.7.6/dagster/_core/definitions/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/auto_materialize_policy.py` & `dagster-1.7.6/dagster/_core/definitions/auto_materialize_policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -172,23 +172,29 @@
 
         return {
             rule for rule in self.rules if rule.decision_type == AutoMaterializeDecisionType.SKIP
         }
 
     @staticmethod
     def from_asset_condition(asset_condition: SchedulingCondition) -> "AutoMaterializePolicy":
+        return AutoMaterializePolicy.from_scheduling_condition(asset_condition)
+
+    @staticmethod
+    def from_scheduling_condition(
+        scheduling_condition: SchedulingCondition,
+    ) -> "AutoMaterializePolicy":
         """Constructs an AutoMaterializePolicy which will materialize an asset partition whenever
-        the provided asset_condition evaluates to True.
+        the provided scheduling_condition evaluates to True.
 
         Args:
-            asset_condition (AssetCondition): The condition which determines whether an asset
+            scheduling_condition (SchedulingCondition): The condition which determines whether an asset
                 partition should be materialized.
         """
         return AutoMaterializePolicy(
-            rules=set(), max_materializations_per_minute=None, asset_condition=asset_condition
+            rules=set(), max_materializations_per_minute=None, asset_condition=scheduling_condition
         )
 
     @public
     @staticmethod
     def eager(max_materializations_per_minute: Optional[int] = 1) -> "AutoMaterializePolicy":
         """Constructs an eager AutoMaterializePolicy.
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/auto_materialize_rule.py` & `dagster-1.7.6/dagster/_core/definitions/auto_materialize_rule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/auto_materialize_rule_evaluation.py` & `dagster-1.7.6/dagster/_core/definitions/auto_materialize_rule_evaluation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/auto_materialize_rule_impls.py` & `dagster-1.7.6/dagster/_core/definitions/auto_materialize_rule_impls.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     def evaluate_for_asset(self, context: "SchedulingContext") -> "SchedulingResult":
         from .declarative_scheduling.scheduling_condition import SchedulingResult
 
         true_subset, subsets_with_metadata = freshness_evaluation_results_for_asset_key(
             context.legacy_context.root_context
         )
-        true_slice = context.asset_graph_view.get_asset_slice_from_subset(true_subset)
+        true_slice = context.asset_graph_view.get_asset_slice_from_valid_subset(true_subset)
         return SchedulingResult.create(context, true_slice, subsets_with_metadata)
 
 
 @whitelist_for_serdes
 class MaterializeOnCronRule(
     AutoMaterializeRule,
     NamedTuple(
@@ -213,15 +213,17 @@
         ) | (
             context.legacy_context.previous_true_subset.as_valid(
                 context.legacy_context.partitions_def
             )
             - context.legacy_context.materialized_requested_or_discarded_since_previous_tick_subset
         )
 
-        true_slice = context.asset_graph_view.get_asset_slice_from_subset(asset_subset_to_request)
+        true_slice = context.asset_graph_view.get_asset_slice_from_valid_subset(
+            asset_subset_to_request
+        )
         return SchedulingResult.create(context, true_slice=true_slice)
 
 
 @whitelist_for_serdes
 @experimental
 class AutoMaterializeAssetPartitionsFilter(
     NamedTuple(
@@ -362,16 +364,16 @@
                 dynamic_partitions_store=context.legacy_context.instance_queryer,
                 current_time=context.legacy_context.instance_queryer.evaluation_time,
                 asset_key=asset_partition.asset_key,
                 partition_key=asset_partition.partition_key,
             ).parent_partitions
 
             updated_parent_asset_partitions = context.legacy_context.instance_queryer.get_parent_asset_partitions_updated_after_child(
-                asset_partition,
-                parent_asset_partitions,
+                asset_partition=asset_partition,
+                parent_asset_partitions=parent_asset_partitions,
                 # do a precise check for updated parents, factoring in data versions, as long as
                 # we're within reasonable limits on the number of partitions to check
                 respect_materialization_data_versions=context.legacy_context.daemon_context.respect_materialization_data_versions
                 and len(parent_asset_partitions) + subset_to_evaluate.size < 100,
                 # ignore self-dependencies when checking for updated parents, to avoid historical
                 # rematerializations from causing a chain of materializations to be kicked off
                 ignored_parent_keys={context.legacy_context.asset_key},
@@ -431,15 +433,15 @@
 
         true_subset, subsets_with_metadata = (
             context.legacy_context.add_evaluation_data_from_previous_tick(
                 asset_partitions_by_evaluation_data,
                 ignore_subset=context.legacy_context.materialized_requested_or_discarded_since_previous_tick_subset,
             )
         )
-        true_slice = context.asset_graph_view.get_asset_slice_from_subset(true_subset)
+        true_slice = context.asset_graph_view.get_asset_slice_from_valid_subset(true_subset)
         return SchedulingResult.create(context, true_slice, subsets_with_metadata)
 
 
 @whitelist_for_serdes
 class MaterializeOnMissingRule(AutoMaterializeRule, NamedTuple("_MaterializeOnMissingRule", [])):
     @property
     def decision_type(self) -> AutoMaterializeDecisionType:
@@ -530,15 +532,17 @@
                     },
                 )
                 | context.legacy_context.previous_true_subset
             ) - context.legacy_context.previous_tick_requested_subset
 
         return SchedulingResult.create(
             context,
-            true_slice=context.asset_graph_view.get_asset_slice_from_subset(unhandled_candidates),
+            true_slice=context.asset_graph_view.get_asset_slice_from_valid_subset(
+                unhandled_candidates
+            ),
             # we keep track of the handled subset instead of the unhandled subset because new
             # partitions may spontaneously jump into existence at any time
             extra_state=handled_subset,
         )
 
 
 @whitelist_for_serdes
@@ -584,15 +588,15 @@
                 ].add(candidate)
 
         true_subset, subsets_with_metadata = (
             context.legacy_context.add_evaluation_data_from_previous_tick(
                 asset_partitions_by_evaluation_data, ignore_subset=subset_to_evaluate
             )
         )
-        true_slice = context.asset_graph_view.get_asset_slice_from_subset(true_subset)
+        true_slice = context.asset_graph_view.get_asset_slice_from_valid_subset(true_subset)
         return SchedulingResult.create(context, true_slice, subsets_with_metadata)
 
 
 @whitelist_for_serdes
 class SkipOnParentMissingRule(AutoMaterializeRule, NamedTuple("_SkipOnParentMissingRule", [])):
     @property
     def decision_type(self) -> AutoMaterializeDecisionType:
@@ -641,15 +645,15 @@
                 ].add(candidate)
 
         true_subset, subsets_with_metadata = (
             context.legacy_context.add_evaluation_data_from_previous_tick(
                 asset_partitions_by_evaluation_data, ignore_subset=subset_to_evaluate
             )
         )
-        true_slice = context.asset_graph_view.get_asset_slice_from_subset(true_subset)
+        true_slice = context.asset_graph_view.get_asset_slice_from_valid_subset(true_subset)
         return SchedulingResult.create(context, true_slice, subsets_with_metadata)
 
 
 @whitelist_for_serdes
 class SkipOnNotAllParentsUpdatedRule(
     AutoMaterializeRule,
     NamedTuple(
@@ -698,17 +702,17 @@
                 context.legacy_context.instance_queryer.evaluation_time,
                 context.legacy_context.asset_key,
                 candidate.partition_key,
             ).parent_partitions
 
             updated_parent_partitions = (
                 context.legacy_context.instance_queryer.get_parent_asset_partitions_updated_after_child(
-                    candidate,
-                    parent_partitions,
-                    context.legacy_context.daemon_context.respect_materialization_data_versions,
+                    asset_partition=candidate,
+                    parent_asset_partitions=parent_partitions,
+                    respect_materialization_data_versions=context.legacy_context.daemon_context.respect_materialization_data_versions,
                     ignored_parent_keys=set(),
                 )
                 | context.legacy_context.parent_will_update_subset.asset_partitions
             )
 
             if self.require_update_for_all_parent_partitions:
                 # All upstream partitions must be updated in order for the candidate to be updated
@@ -735,15 +739,15 @@
                 ].add(candidate)
 
         true_subset, subsets_with_metadata = (
             context.legacy_context.add_evaluation_data_from_previous_tick(
                 asset_partitions_by_evaluation_data, ignore_subset=subset_to_evaluate
             )
         )
-        true_slice = context.asset_graph_view.get_asset_slice_from_subset(true_subset)
+        true_slice = context.asset_graph_view.get_asset_slice_from_valid_subset(true_subset)
         return SchedulingResult.create(context, true_slice, subsets_with_metadata)
 
 
 @whitelist_for_serdes
 class SkipOnNotAllParentsUpdatedSinceCronRule(
     AutoMaterializeRule,
     NamedTuple(
@@ -961,15 +965,15 @@
                     context.legacy_context.partitions_def
                 )
                 - context.legacy_context.previous_true_subset
             ) | all_parents_updated_subset
 
         return SchedulingResult.create(
             context,
-            true_slice=context.asset_graph_view.get_asset_slice_from_subset(
+            true_slice=context.asset_graph_view.get_asset_slice_from_valid_subset(
                 context.legacy_context.candidate_subset - all_parents_updated_subset
             ),
             extra_state=list(updated_subsets_by_key.values()),
         )
 
 
 @whitelist_for_serdes
@@ -1012,15 +1016,15 @@
                 ].add(candidate)
 
         true_subset, subsets_with_metadata = (
             context.legacy_context.add_evaluation_data_from_previous_tick(
                 asset_partitions_by_evaluation_data, ignore_subset=subset_to_evaluate
             )
         )
-        true_slice = context.asset_graph_view.get_asset_slice_from_subset(true_subset)
+        true_slice = context.asset_graph_view.get_asset_slice_from_valid_subset(true_subset)
         return SchedulingResult.create(context, true_slice, subsets_with_metadata)
 
 
 @whitelist_for_serdes
 class SkipOnBackfillInProgressRule(
     AutoMaterializeRule,
     NamedTuple("_SkipOnBackfillInProgressRule", [("all_partitions", bool)]),
@@ -1052,15 +1056,15 @@
         if backfilling_subset.size == 0:
             true_subset = context.legacy_context.empty_subset()
         elif self.all_partitions:
             true_subset = context.legacy_context.candidate_subset
         else:
             true_subset = context.legacy_context.candidate_subset & backfilling_subset
 
-        true_slice = context.asset_graph_view.get_asset_slice_from_subset(true_subset)
+        true_slice = context.asset_graph_view.get_asset_slice_from_valid_subset(true_subset)
         return SchedulingResult.create(context, true_slice)
 
 
 @whitelist_for_serdes
 class DiscardOnMaxMaterializationsExceededRule(
     AutoMaterializeRule, NamedTuple("_DiscardOnMaxMaterializationsExceededRule", [("limit", int)])
 ):
@@ -1081,15 +1085,15 @@
                 context.legacy_context.candidate_subset.asset_partitions,
                 key=lambda x: sort_key_for_asset_partition(context.legacy_context.asset_graph, x),
             )[self.limit :]
         )
 
         return SchedulingResult.create(
             context,
-            context.asset_graph_view.get_asset_slice_from_subset(
+            context.asset_graph_view.get_asset_slice_from_valid_subset(
                 AssetSubset.from_asset_partitions_set(
                     context.legacy_context.asset_key,
                     context.legacy_context.partitions_def,
                     rate_limited_asset_partitions,
                 )
             ),
         )
@@ -1119,17 +1123,17 @@
             )
         )
         if planned_materialization_info:
             dagster_run = instance.get_run_by_id(planned_materialization_info.run_id)
             if dagster_run and dagster_run.status in IN_PROGRESS_RUN_STATUSES:
                 return SchedulingResult.create(
                     context,
-                    context.asset_graph_view.get_asset_slice_from_subset(
+                    context.asset_graph_view.get_asset_slice_from_valid_subset(
                         context.legacy_context.candidate_subset
                     ),
                 )
         return SchedulingResult.create(
             context,
-            context.asset_graph_view.get_asset_slice_from_subset(
+            context.asset_graph_view.get_asset_slice_from_valid_subset(
                 context.legacy_context.empty_subset()
             ),
         )
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/auto_materialize_sensor_definition.py` & `dagster-1.7.6/dagster/_core/definitions/auto_materialize_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/backfill_policy.py` & `dagster-1.7.6/dagster/_core/definitions/backfill_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/base_asset_graph.py` & `dagster-1.7.6/dagster/_core/definitions/base_asset_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,19 +7,21 @@
     TYPE_CHECKING,
     AbstractSet,
     Callable,
     Dict,
     Generic,
     Iterable,
     Iterator,
+    List,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Set,
+    Tuple,
     TypeVar,
     Union,
     cast,
 )
 
 import toposort
 
@@ -710,55 +712,68 @@
 
         return result
 
     def bfs_filter_asset_partitions(
         self,
         dynamic_partitions_store: DynamicPartitionsStore,
         condition_fn: Callable[
-            [Iterable[AssetKeyPartitionKey], AbstractSet[AssetKeyPartitionKey]], bool
+            [Iterable[AssetKeyPartitionKey], AbstractSet[AssetKeyPartitionKey]], Tuple[bool, str]
         ],
         initial_asset_partitions: Iterable[AssetKeyPartitionKey],
         evaluation_time: datetime,
-    ) -> AbstractSet[AssetKeyPartitionKey]:
+    ) -> Tuple[
+        AbstractSet[AssetKeyPartitionKey], Sequence[Tuple[Iterable[AssetKeyPartitionKey], str]]
+    ]:
         """Returns asset partitions within the graph that satisfy supplied criteria.
 
         - Are >= initial_asset_partitions
         - Match the condition_fn
         - Any of their ancestors >= initial_asset_partitions match the condition_fn
 
+        Also returns a list of tuples, where each tuple is a candidated_unit (list of
+        AssetKeyPartitionKeys that must be materialized together - ie multi_asset) that do not
+        satisfy the criteria and the reason they were filtered out.
+
+        The condition_fn should return a tuple of a boolean indicating whether the asset partition meets
+        the condition and a string explaining why it does not meet the condition, if applicable.
+
         Visits parents before children.
 
         When asset partitions are part of the same execution set (non-subsettable multi-asset),
         they're provided all at once to the condition_fn.
         """
         all_nodes = set(initial_asset_partitions)
 
         # invariant: we never consider an asset partition before considering its ancestors
         queue = ToposortedPriorityQueue(self, all_nodes, include_full_execution_set=True)
 
         result: Set[AssetKeyPartitionKey] = set()
+        failed_reasons: List[Tuple[Iterable[AssetKeyPartitionKey], str]] = []
 
         while len(queue) > 0:
             candidates_unit = queue.dequeue()
 
-            if condition_fn(candidates_unit, result):
+            meets_condition, fail_reason = condition_fn(candidates_unit, result)
+            if meets_condition:
                 result.update(candidates_unit)
 
                 for candidate in candidates_unit:
                     for child in self.get_children_partitions(
                         dynamic_partitions_store,
                         evaluation_time,
                         candidate.asset_key,
                         candidate.partition_key,
                     ):
                         if child not in all_nodes:
                             queue.enqueue(child)
                             all_nodes.add(child)
+            else:
+                failed_reasons.append((candidates_unit, fail_reason))
 
-        return result
+        return result, failed_reasons
 
     def split_asset_keys_by_repository(
         self, asset_keys: AbstractSet[AssetKey]
     ) -> Sequence[AbstractSet[AssetKey]]:
         return [asset_keys]
 
     def __hash__(self) -> int:
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/cacheable_assets.py` & `dagster-1.7.6/dagster/_core/definitions/cacheable_assets.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/composition.py` & `dagster-1.7.6/dagster/_core/definitions/composition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/config.py` & `dagster-1.7.6/dagster/_core/definitions/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/configurable.py` & `dagster-1.7.6/dagster/_core/definitions/configurable.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/data_time.py` & `dagster-1.7.6/dagster/_core/definitions/data_time.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/data_version.py` & `dagster-1.7.6/dagster/_core/definitions/data_version.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/README.md` & `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/__init__.py` & `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from .legacy import RuleCondition as RuleCondition
 from .legacy.asset_condition import AssetCondition as AssetCondition
 from .operands import (
+    FailedSchedulingCondition as FailedSchedulingCondition,
     InLatestTimeWindowCondition as InLatestTimeWindowCondition,
     InProgressSchedulingCondition as InProgressSchedulingCondition,
     MissingSchedulingCondition as MissingSchedulingCondition,
+    ParentNewerCondition as ParentNewerCondition,
+    RequestedThisTickCondition as RequestedThisTickCondition,
+    ScheduledSinceCondition as ScheduledSinceCondition,
+    UpdatedSinceCronCondition as UpdatedSinceCronCondition,
 )
 from .operators import (
     AllDepsCondition as AllDepsCondition,
     AndAssetCondition as AndAssetCondition,
     AnyDepsCondition as AnyDepsCondition,
     NotAssetCondition as NotAssetCondition,
     OrAssetCondition as OrAssetCondition,
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py` & `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py` & `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
         for parent_key in self.asset_graph.get(self.asset_key).parent_keys:
             if not self.materializable_in_same_run(self.asset_key, parent_key):
                 continue
             parent_info = self.evaluation_state_by_key.get(parent_key)
             if not parent_info:
                 continue
             parent_subset = parent_info.true_subset.as_valid(self.partitions_def)
-            subset |= parent_subset.copy(update={"asset_key": self.asset_key})
+            subset |= parent_subset.model_copy(update={"asset_key": self.asset_key})
         return subset
 
     @functools.cached_property
     @root_property
     def materialized_since_previous_tick_subset(self) -> ValidAssetSubset:
         """Returns the set of asset partitions that were materialized since the previous tick."""
         return AssetSubset.from_asset_partitions_set(
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/legacy/rule_condition.py` & `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/legacy/rule_condition.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 @experimental
 @whitelist_for_serdes
 class RuleCondition(AssetCondition):
     """This class represents the condition that a particular AutoMaterializeRule is satisfied."""
 
     rule: AutoMaterializeRule
 
-    def get_unique_id(self, parent_unique_id: Optional[str]) -> str:
+    def get_unique_id(self, *, parent_unique_id: Optional[str], index: Optional[str]) -> str:
         # preserves old (bad) behavior of not including the parent_unique_id to avoid inavlidating
         # old serialized information
         parts = [self.rule.__class__.__name__, self.description]
         return non_secure_md5_hash_str("".join(parts).encode())
 
     @property
     def description(self) -> str:
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operands/updated_since_cron_condition.py` & `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operands/updated_since_cron_condition.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,60 @@
 import datetime
 
+from dagster._serdes.serdes import whitelist_for_serdes
 from dagster._utils.schedules import reverse_cron_string_iterator
 
-from ..legacy.asset_condition import AssetCondition
-from ..scheduling_condition import SchedulingResult
+from ..scheduling_condition import SchedulingCondition, SchedulingResult
 from ..scheduling_context import SchedulingContext
 
 
-class UpdatedSinceCronCondition(AssetCondition):
+@whitelist_for_serdes
+class UpdatedSinceCronCondition(SchedulingCondition):
     cron_schedule: str
     cron_timezone: str
 
     @property
-    def condition_description(self) -> str:
+    def description(self) -> str:
         return f"Updated since latest tick of {self.cron_schedule} ({self.cron_timezone})"
 
     def _get_previous_cron_tick(self, context: SchedulingContext) -> datetime.datetime:
         previous_ticks = reverse_cron_string_iterator(
             end_timestamp=context.effective_dt.timestamp(),
             cron_string=self.cron_schedule,
             execution_timezone=self.cron_timezone,
         )
         return next(previous_ticks)
 
     def evaluate(self, context: SchedulingContext) -> SchedulingResult:
         previous_cron_tick = self._get_previous_cron_tick(context)
 
         if (
-            # never evaluated
+            # never evaluated or evaluation info is no longer valid
             context.previous_evaluation_info is None
             or context.previous_evaluation_node is None
+            or context.previous_evaluation_node.true_slice is None
             # not evaluated since latest schedule tick
             or context.previous_evaluation_info.temporal_context.effective_dt < previous_cron_tick
             # has new set of candidates
             or context.previous_evaluation_node.candidate_slice != context.candidate_slice
-            # asset updated since latest evaluation
-            or context.asset_updated_since_previous_tick()
         ):
             # do a full recomputation
             updated_subset = (
                 context.legacy_context.instance_queryer.get_asset_subset_updated_after_time(
                     asset_key=context.asset_key,
                     after_time=previous_cron_tick,
                 )
             )
             # TODO: implement this on the AssetGraphView
-            true_slice = context.candidate_slice.compute_intersection(
-                context.asset_graph_view.get_asset_slice_from_subset(updated_subset)
-            )
+            true_slice = context.asset_graph_view.get_asset_slice_from_valid_subset(updated_subset)
         else:
-            true_slice = context.previous_evaluation_node.true_slice
+            # do an incremental updated, adding in any asset partitions that have been materialized
+            # since the previous evaluation
+            true_slice = context.previous_evaluation_node.true_slice.compute_union(
+                context.asset_graph_view.compute_updated_since_cursor_slice(
+                    asset_key=context.asset_key, cursor=context.previous_evaluation_max_storage_id
+                )
+            )
 
-        return SchedulingResult.create(context, true_slice)
+        return SchedulingResult.create(
+            context, context.candidate_slice.compute_intersection(true_slice)
+        )
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operators/boolean_operators.py` & `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operators/boolean_operators.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     @property
     def description(self) -> str:
         return "All of"
 
     def evaluate(self, context: SchedulingContext) -> SchedulingResult:
         child_results: List[SchedulingResult] = []
         true_slice = context.candidate_slice
-        for child in self.children:
+        for i, child in enumerate(self.children):
             child_context = context.for_child_condition(
-                child_condition=child, candidate_slice=true_slice
+                child_condition=child, child_index=i, candidate_slice=true_slice
             )
             child_result = child.evaluate(child_context)
             child_results.append(child_result)
             true_slice = true_slice.compute_intersection(child_result.true_slice)
         return SchedulingResult.create_from_children(context, true_slice, child_results)
 
 
@@ -49,17 +49,17 @@
     @property
     def description(self) -> str:
         return "Any of"
 
     def evaluate(self, context: SchedulingContext) -> SchedulingResult:
         child_results: List[SchedulingResult] = []
         true_slice = context.asset_graph_view.create_empty_slice(context.asset_key)
-        for child in self.children:
+        for i, child in enumerate(self.children):
             child_context = context.for_child_condition(
-                child_condition=child, candidate_slice=context.candidate_slice
+                child_condition=child, child_index=i, candidate_slice=context.candidate_slice
             )
             child_result = child.evaluate(child_context)
             child_results.append(child_result)
             true_slice = true_slice.compute_union(child_result.true_slice)
 
         return SchedulingResult.create_from_children(context, true_slice, child_results)
 
@@ -77,13 +77,13 @@
 
     @property
     def children(self) -> Sequence[SchedulingCondition]:
         return [self.operand]
 
     def evaluate(self, context: SchedulingContext) -> SchedulingResult:
         child_context = context.for_child_condition(
-            child_condition=self.operand, candidate_slice=context.candidate_slice
+            child_condition=self.operand, child_index=0, candidate_slice=context.candidate_slice
         )
         child_result = self.operand.evaluate(child_context)
         true_slice = context.candidate_slice.compute_difference(child_result.true_slice)
 
         return SchedulingResult.create_from_children(context, true_slice, [child_result])
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/operators/dep_operators.py` & `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/operators/dep_operators.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from dagster._core.definitions.asset_key import AssetKey
 from dagster._serdes.serdes import whitelist_for_serdes
 
-from ..legacy.asset_condition import AssetCondition
 from ..scheduling_condition import SchedulingCondition, SchedulingResult
 from ..scheduling_context import SchedulingContext
 
 
 class DepConditionWrapperCondition(SchedulingCondition):
     """Wrapper object which evaluates a condition against a dependency and returns a subset
     representing the subset of downstream asset which has at least one parent which evaluated to
@@ -19,74 +18,78 @@
     def description(self) -> str:
         return f"{self.dep_key.to_user_string()}"
 
     def evaluate(self, context: SchedulingContext) -> SchedulingResult:
         # only evaluate parents of the current candidates
         dep_candidate_slice = context.candidate_slice.compute_parent_slice(self.dep_key)
         dep_context = context.for_child_condition(
-            child_condition=self.operand, candidate_slice=dep_candidate_slice
+            child_condition=self.operand, child_index=0, candidate_slice=dep_candidate_slice
         )
 
         # evaluate condition against the dependency
         dep_result = self.operand.evaluate(dep_context)
 
         # find all children of the true dep slice
         true_slice = dep_result.true_slice.compute_child_slice(context.asset_key)
         return SchedulingResult.create_from_children(
             context=context, true_slice=true_slice, child_results=[dep_result]
         )
 
 
-@whitelist_for_serdes
-class AnyDepsCondition(AssetCondition):
+class DepCondition(SchedulingCondition):
     operand: SchedulingCondition
 
+
+@whitelist_for_serdes
+class AnyDepsCondition(DepCondition):
     @property
     def description(self) -> str:
         return "Any deps"
 
     def evaluate(self, context: SchedulingContext) -> SchedulingResult:
         dep_results = []
         true_slice = context.asset_graph_view.create_empty_slice(context.asset_key)
 
         dep_keys = context.asset_graph_view.asset_graph.get(context.asset_key).parent_keys
-        for dep_key in dep_keys:
+        for i, dep_key in enumerate(sorted(dep_keys)):
             dep_condition = DepConditionWrapperCondition(dep_key=dep_key, operand=self.operand)
             dep_result = dep_condition.evaluate(
                 context.for_child_condition(
-                    child_condition=dep_condition, candidate_slice=context.candidate_slice
+                    child_condition=dep_condition,
+                    child_index=i,
+                    candidate_slice=context.candidate_slice,
                 )
             )
             dep_results.append(dep_result)
             true_slice = true_slice.compute_union(dep_result.true_slice)
 
         true_slice = context.candidate_slice.compute_intersection(true_slice)
         return SchedulingResult.create_from_children(
             context, true_slice=true_slice, child_results=dep_results
         )
 
 
 @whitelist_for_serdes
-class AllDepsCondition(SchedulingCondition):
-    operand: SchedulingCondition
-
+class AllDepsCondition(DepCondition):
     @property
     def description(self) -> str:
         return "All deps"
 
     def evaluate(self, context: SchedulingContext) -> SchedulingResult:
         dep_results = []
         true_slice = context.candidate_slice
 
         dep_keys = context.asset_graph_view.asset_graph.get(context.asset_key).parent_keys
-        for dep_key in dep_keys:
+        for i, dep_key in enumerate(sorted(dep_keys)):
             dep_condition = DepConditionWrapperCondition(dep_key=dep_key, operand=self.operand)
             dep_result = dep_condition.evaluate(
                 context.for_child_condition(
-                    child_condition=dep_condition, candidate_slice=context.candidate_slice
+                    child_condition=dep_condition,
+                    child_index=i,
+                    candidate_slice=context.candidate_slice,
                 )
             )
             dep_results.append(dep_result)
             true_slice = true_slice.compute_intersection(dep_result.true_slice)
 
         return SchedulingResult.create_from_children(
             context, true_slice=true_slice, child_results=dep_results
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/declarative_scheduling/scheduling_context.py` & `dagster-1.7.6/dagster/_core/definitions/declarative_scheduling/scheduling_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 from dagster._core.definitions.declarative_scheduling.scheduling_condition import (
     SchedulingCondition,
 )
 from dagster._core.definitions.declarative_scheduling.scheduling_evaluation_info import (
     SchedulingEvaluationInfo,
     SchedulingEvaluationResultNode,
 )
-from dagster._core.definitions.events import AssetKeyPartitionKey
 from dagster._core.definitions.partition import PartitionsDefinition
 from dagster._model import DagsterModel
 
 from .legacy.legacy_context import LegacyRuleEvaluationContext
 
 if TYPE_CHECKING:
+    from dagster._core.definitions.base_asset_graph import BaseAssetGraph
     from dagster._utils.caching_instance_queryer import CachingInstanceQueryer
 
 
 class SchedulingContext(DagsterModel):
     # the slice over which the condition is being evaluated
     candidate_slice: AssetSlice
 
@@ -65,59 +65,67 @@
         legacy_context: "LegacyRuleEvaluationContext",
     ) -> "SchedulingContext":
         asset_graph = asset_graph_view.asset_graph
         auto_materialize_policy = check.not_none(asset_graph.get(asset_key).auto_materialize_policy)
         scheduling_condition = auto_materialize_policy.to_scheduling_condition()
 
         # construct is used here for performance
-        return SchedulingContext.construct(
+        return SchedulingContext.model_construct(
             candidate_slice=asset_graph_view.get_asset_slice(asset_key),
             condition=scheduling_condition,
-            condition_unique_id=scheduling_condition.get_unique_id(None),
+            condition_unique_id=scheduling_condition.get_unique_id(
+                parent_unique_id=None, index=None
+            ),
             asset_graph_view=asset_graph_view,
             parent_context=None,
             create_time=pendulum.now("UTC"),
             logger=logger,
             previous_evaluation_info=previous_evaluation_info,
             current_tick_evaluation_info_by_key=current_tick_evaluation_info_by_key,
             inner_legacy_context=legacy_context,
         )
 
     def for_child_condition(
-        self, child_condition: SchedulingCondition, candidate_slice: AssetSlice
+        self, child_condition: SchedulingCondition, child_index: int, candidate_slice: AssetSlice
     ) -> "SchedulingContext":
         # construct is used here for performance
-        return SchedulingContext.construct(
+        return SchedulingContext.model_construct(
             candidate_slice=candidate_slice,
             condition=child_condition,
             condition_unique_id=child_condition.get_unique_id(
-                parent_unique_id=self.condition_unique_id
+                parent_unique_id=self.condition_unique_id, index=child_index
             ),
             asset_graph_view=self.asset_graph_view,
             parent_context=self,
             create_time=pendulum.now("UTC"),
             logger=self.logger,
             previous_evaluation_info=self.previous_evaluation_info,
             current_tick_evaluation_info_by_key=self.current_tick_evaluation_info_by_key,
             inner_legacy_context=self.legacy_context.for_child(
                 child_condition,
-                child_condition.get_unique_id(self.condition_unique_id),
+                child_condition.get_unique_id(
+                    parent_unique_id=self.condition_unique_id, index=child_index
+                ),
                 candidate_slice.convert_to_valid_asset_subset(),
             ),
         )
 
     @property
+    def asset_graph(self) -> "BaseAssetGraph":
+        return self.asset_graph_view.asset_graph
+
+    @property
     def asset_key(self) -> AssetKey:
         """The asset key over which this condition is being evaluated."""
         return self.candidate_slice.asset_key
 
     @property
     def partitions_def(self) -> Optional[PartitionsDefinition]:
         """The partitions definition for the asset being evaluated, if it exists."""
-        return self.asset_graph_view.asset_graph.get(self.asset_key).partitions_def
+        return self.asset_graph.get(self.asset_key).partitions_def
 
     @property
     def root_context(self) -> "SchedulingContext":
         """Returns the context object at the root of the condition evaluation tree."""
         return self.parent_context.root_context if self.parent_context is not None else self
 
     @property
@@ -139,22 +147,39 @@
         return self.inner_legacy_context
 
     @property
     def _queryer(self) -> "CachingInstanceQueryer":
         return self.asset_graph_view._queryer  # noqa
 
     @property
-    def new_max_storage_id(self) -> Optional[int]:
-        # TODO: pull this from the AssetGraphView instead
-        return self.legacy_context.new_max_storage_id
+    def previous_requested_slice(self) -> Optional[AssetSlice]:
+        """Returns the requested slice for the previous evaluation. If this asset has never been
+        evaluated, returns None.
+        """
+        return (
+            self.previous_evaluation_info.requested_slice if self.previous_evaluation_info else None
+        )
+
+    @property
+    def previous_candidate_slice(self) -> Optional[AssetSlice]:
+        """Returns the candidate slice for the previous evaluation. If this node has never been
+        evaluated, returns None.
+        """
+        return (
+            self.previous_evaluation_node.candidate_slice if self.previous_evaluation_node else None
+        )
 
-    def asset_updated_since_previous_tick(self) -> bool:
-        """Returns True if the target asset has been updated since the previous evaluation."""
-        cursor = (
+    @property
+    def previous_evaluation_max_storage_id(self) -> Optional[int]:
+        """Returns the maximum storage ID for the previous time this node was evaluated. If this
+        node has never been evaluated, returns None.
+        """
+        return (
             self.previous_evaluation_info.temporal_context.last_event_id
-            if self.previous_evaluation_info
+            if self.previous_evaluation_info and self.previous_evaluation_node
             else None
         )
-        return self._queryer.asset_partition_has_materialization_or_observation(
-            asset_partition=AssetKeyPartitionKey(self.asset_key),
-            after_cursor=cursor,
-        )
+
+    @property
+    def new_max_storage_id(self) -> Optional[int]:
+        # TODO: pull this from the AssetGraphView instead
+        return self.legacy_context.new_max_storage_id
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/decorators/__init__.py` & `dagster-1.7.6/dagster/_core/definitions/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/decorators/asset_check_decorator.py` & `dagster-1.7.6/dagster/_core/definitions/decorators/asset_check_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/decorators/asset_decorator.py` & `dagster-1.7.6/dagster/_core/definitions/decorators/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/decorators/config_mapping_decorator.py` & `dagster-1.7.6/dagster/_core/definitions/decorators/config_mapping_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/decorators/graph_decorator.py` & `dagster-1.7.6/dagster/_core/definitions/decorators/graph_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/decorators/hook_decorator.py` & `dagster-1.7.6/dagster/_core/definitions/decorators/hook_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/decorators/job_decorator.py` & `dagster-1.7.6/dagster/_core/definitions/decorators/job_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/decorators/op_decorator.py` & `dagster-1.7.6/dagster/_core/definitions/decorators/op_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/decorators/repository_decorator.py` & `dagster-1.7.6/dagster/_core/definitions/decorators/repository_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/decorators/schedule_decorator.py` & `dagster-1.7.6/dagster/_core/definitions/decorators/schedule_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/decorators/sensor_decorator.py` & `dagster-1.7.6/dagster/_core/definitions/decorators/sensor_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/decorators/source_asset_decorator.py` & `dagster-1.7.6/dagster/_core/definitions/decorators/source_asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/definition_config_schema.py` & `dagster-1.7.6/dagster/_core/definitions/definition_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/definitions_class.py` & `dagster-1.7.6/dagster/_core/definitions/definitions_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/dependency.py` & `dagster-1.7.6/dagster/_core/definitions/dependency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/events.py` & `dagster-1.7.6/dagster/_core/definitions/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,26 @@
             isinstance(other, Output)
             and self.value == other.value
             and self.output_name == other.output_name
             and self.metadata == other.metadata
             and self.tags == other.tags
         )
 
+    def with_metadata(self, metadata: Optional[Mapping[str, RawMetadataValue]]) -> "Output":
+        """Returns a new Output with the same value and output_name,
+        but with the provided metadata.
+        """
+        return Output(
+            value=self.value,
+            output_name=self.output_name,
+            metadata=metadata,
+            data_version=self.data_version,
+            tags=self.tags,
+        )
+
 
 class DynamicOutput(Generic[T]):
     """Variant of :py:class:`Output <dagster.Output>` used to support
     dynamic mapping & collect. Each ``DynamicOutput`` produced by an op represents
     one item in a set that can be processed individually with ``map`` or gathered
     with ``collect``.
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/executor_definition.py` & `dagster-1.7.6/dagster/_core/definitions/executor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/external_asset.py` & `dagster-1.7.6/dagster/_core/definitions/external_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/freshness_based_auto_materialize.py` & `dagster-1.7.6/dagster/_core/definitions/freshness_based_auto_materialize.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/freshness_policy.py` & `dagster-1.7.6/dagster/_core/definitions/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/freshness_policy_sensor_definition.py` & `dagster-1.7.6/dagster/_core/definitions/freshness_policy_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/graph_definition.py` & `dagster-1.7.6/dagster/_core/definitions/graph_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/hook_definition.py` & `dagster-1.7.6/dagster/_core/definitions/hook_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/hook_invocation.py` & `dagster-1.7.6/dagster/_core/definitions/hook_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/inference.py` & `dagster-1.7.6/dagster/_core/definitions/inference.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/input.py` & `dagster-1.7.6/dagster/_core/definitions/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/instigation_logger.py` & `dagster-1.7.6/dagster/_core/definitions/instigation_logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/job_base.py` & `dagster-1.7.6/dagster/_core/definitions/job_base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/job_definition.py` & `dagster-1.7.6/dagster/_core/definitions/job_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import importlib
 import os
 import warnings
 from datetime import datetime
-from functools import update_wrapper
+from functools import cached_property, update_wrapper
 from typing import (
     TYPE_CHECKING,
     AbstractSet,
     Any,
     Dict,
     Iterable,
     List,
@@ -22,14 +22,15 @@
 import dagster._check as check
 from dagster._annotations import deprecated, experimental_param, public
 from dagster._config import Field, Shape, StringSource
 from dagster._config.config_type import ConfigType
 from dagster._config.validate import validate_config
 from dagster._core.definitions.asset_check_spec import AssetCheckKey
 from dagster._core.definitions.asset_selection import AssetSelection
+from dagster._core.definitions.backfill_policy import BackfillPolicy
 from dagster._core.definitions.dependency import (
     Node,
     NodeHandle,
     NodeInputHandle,
     NodeInvocation,
 )
 from dagster._core.definitions.events import AssetKey
@@ -412,14 +413,27 @@
     def partitions_def(self) -> Optional[PartitionsDefinition]:
         """Returns the :py:class:`PartitionsDefinition` for the job, if it has one.
 
         A partitions definition defines the set of partition keys the job operates on.
         """
         return None if not self.partitioned_config else self.partitioned_config.partitions_def
 
+    @cached_property
+    def backfill_policy(self) -> Optional[BackfillPolicy]:
+        from dagster._core.definitions.asset_job import ASSET_BASE_JOB_PREFIX
+
+        executable_nodes = {self.asset_layer.get(k) for k in self.asset_layer.executable_asset_keys}
+        backfill_policies = {n.backfill_policy for n in executable_nodes if n.is_partitioned}
+        if not self.name.startswith(ASSET_BASE_JOB_PREFIX):
+            check.invariant(
+                len(backfill_policies) <= 1,
+                "All assets in non-asset base job a job must have the same backfill policy.",
+            )
+        return next(iter(backfill_policies), None)
+
     @property
     def hook_defs(self) -> AbstractSet[HookDefinition]:
         return self._hook_defs
 
     @property
     def asset_layer(self) -> AssetLayer:
         return self._asset_layer
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/load_asset_checks_from_modules.py` & `dagster-1.7.6/dagster/_core/definitions/load_asset_checks_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/load_assets_from_modules.py` & `dagster-1.7.6/dagster/_core/definitions/load_assets_from_modules.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/logger_definition.py` & `dagster-1.7.6/dagster/_core/definitions/logger_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/logger_invocation.py` & `dagster-1.7.6/dagster/_core/definitions/logger_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/materialize.py` & `dagster-1.7.6/dagster/_core/definitions/materialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from ..storage.io_manager import IOManagerDefinition
 from ..storage.mem_io_manager import mem_io_manager
 from .assets import AssetsDefinition
 from .source_asset import SourceAsset
 
 if TYPE_CHECKING:
     from dagster._core.definitions.asset_selection import CoercibleToAssetSelection
-    from dagster._core.definitions.events import AssetKey
 
     from ..execution.execute_in_process_result import ExecuteInProcessResult
 
 EPHEMERAL_JOB_NAME = "__ephemeral_asset_job__"
 
 
 def materialize(
@@ -86,19 +85,14 @@
     from dagster._core.definitions.definitions_class import Definitions
 
     assets = check.sequence_param(assets, "assets", of_type=(AssetsDefinition, SourceAsset))
     instance = check.opt_inst_param(instance, "instance", DagsterInstance)
     partition_key = check.opt_str_param(partition_key, "partition_key")
     resources = check.opt_mapping_param(resources, "resources", key_type=str)
 
-    all_executable_keys: Set[AssetKey] = set()
-    for asset in assets:
-        if isinstance(asset, AssetsDefinition):
-            all_executable_keys = all_executable_keys.union(set(asset.keys))
-
     defs = Definitions(
         jobs=[define_asset_job(name=EPHEMERAL_JOB_NAME, selection=selection)],
         assets=assets,
         resources=resources,
     )
 
     # validate input asset graph and resources
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/metadata/__init__.py` & `dagster-1.7.6/dagster/_core/definitions/metadata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,55 +53,61 @@
     TableColumnLineageMetadataValue as TableColumnLineageMetadataValue,
     TableMetadataValue as TableMetadataValue,
     TableSchemaMetadataValue as TableSchemaMetadataValue,
     TextMetadataValue as TextMetadataValue,
     TimestampMetadataValue as TimestampMetadataValue,
     UrlMetadataValue as UrlMetadataValue,
 )
+from .source_code import (
+    DEFAULT_SOURCE_FILE_KEY as DEFAULT_SOURCE_FILE_KEY,
+    CodeReferencesMetadataSet as CodeReferencesMetadataSet,
+    CodeReferencesMetadataValue as CodeReferencesMetadataValue,
+    LocalFileCodeReference as LocalFileCodeReference,
+    with_source_code_references as with_source_code_references,
+)
 from .table import (  # re-exported
     TableColumn as TableColumn,
     TableColumnConstraints as TableColumnConstraints,
     TableColumnDep as TableColumnDep,
     TableColumnLineage as TableColumnLineage,
     TableConstraints as TableConstraints,
     TableRecord as TableRecord,
     TableSchema as TableSchema,
 )
 
 ArbitraryMetadataMapping: TypeAlias = Mapping[str, Any]
 
 RawMetadataValue = Union[
-    "MetadataValue",
+    MetadataValue,
     TableSchema,
     AssetKey,
     os.PathLike,
     Dict[Any, Any],
     float,
     int,
     List[Any],
     str,
     datetime,
     None,
 ]
 
-MetadataMapping: TypeAlias = Mapping[str, "MetadataValue"]
+MetadataMapping: TypeAlias = Mapping[str, MetadataValue]
 RawMetadataMapping: TypeAlias = Mapping[str, RawMetadataValue]
 
 T_Packable = TypeVar("T_Packable", bound=PackableValue, default=PackableValue, covariant=True)
 
-
 # ########################
 # ##### NORMALIZATION
 # ########################
 
 
 def normalize_metadata(
     metadata: Mapping[str, RawMetadataValue],
     allow_invalid: bool = False,
-) -> Mapping[str, "MetadataValue"]:
+) -> Mapping[str, MetadataValue]:
     # This is a stopgap measure to deal with unsupported metadata values, which occur when we try
     # to convert arbitrary metadata (on e.g. OutputDefinition) to a MetadataValue, which is required
     # for serialization. This will cause unsupported values to be silently replaced with a
     # string placeholder.
     normalized_metadata: Dict[str, MetadataValue] = {}
     for k, v in metadata.items():
         try:
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/metadata/metadata_set.py` & `dagster-1.7.6/dagster/_core/definitions/metadata/metadata_set.py`

 * *Files 7% similar despite different names*

```diff
@@ -145,15 +145,19 @@
     """Metadata entries that apply to definitions, observations, or materializations of assets that
     are tables.
 
     Args:
         column_schema (Optional[TableSchema]): The schema of the columns in the table.
         column_lineage (Optional[TableColumnLineage]): The lineage of column inputs to column
             outputs for the table.
+        row_count (Optional[int]): The number of rows in the table.
+        partition_row_count (Optional[int]): The number of rows in the materialized or observed partition.
     """
 
     column_schema: Optional[TableSchema] = None
     column_lineage: Optional[TableColumnLineage] = None
+    row_count: Optional[int] = None
+    partition_row_count: Optional[int] = None
 
     @classmethod
     def namespace(cls) -> str:
         return "dagster"
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/metadata/metadata_value.py` & `dagster-1.7.6/dagster/_core/definitions/metadata/metadata_value.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/metadata/table.py` & `dagster-1.7.6/dagster/_core/definitions/metadata/table.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 # ##### TABLE RECORD
 # ########################
 
 
 @experimental
 @whitelist_for_serdes
 class TableRecord(
-    NamedTuple("TableRecord", [("data", PublicAttr[Mapping[str, Union[str, int, float, bool]]])])
+    NamedTuple(
+        "TableRecord", [("data", PublicAttr[Mapping[str, Optional[Union[str, int, float, bool]]]])]
+    )
 ):
     """Represents one record in a table. Field keys are arbitrary strings-- field values must be
     strings, integers, floats, or bools.
     """
 
-    def __new__(cls, data: Mapping[str, Union[str, int, float, bool]]):
+    def __new__(cls, data: Mapping[str, Optional[Union[str, int, float, bool]]]):
         check.dict_param(
             data,
             "data",
             value_type=(str, float, int, bool, type(None)),
             additional_message="Record fields must be one of types: (str, float, int, bool)",
         )
         return super(TableRecord, cls).__new__(cls, data=data)
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/multi_asset_sensor_definition.py` & `dagster-1.7.6/dagster/_core/definitions/multi_asset_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/multi_dimensional_partitions.py` & `dagster-1.7.6/dagster/_core/definitions/multi_dimensional_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/node_container.py` & `dagster-1.7.6/dagster/_core/definitions/node_container.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/node_definition.py` & `dagster-1.7.6/dagster/_core/definitions/node_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/observe.py` & `dagster-1.7.6/dagster/_core/definitions/observe.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/op_definition.py` & `dagster-1.7.6/dagster/_core/definitions/op_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/op_invocation.py` & `dagster-1.7.6/dagster/_core/definitions/op_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/op_selection.py` & `dagster-1.7.6/dagster/_core/definitions/op_selection.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/output.py` & `dagster-1.7.6/dagster/_core/definitions/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/partition.py` & `dagster-1.7.6/dagster/_core/definitions/partition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/partition_key_range.py` & `dagster-1.7.6/dagster/_core/definitions/partition_key_range.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/partition_mapping.py` & `dagster-1.7.6/dagster/_core/definitions/partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/partitioned_schedule.py` & `dagster-1.7.6/dagster/_core/definitions/partitioned_schedule.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/policy.py` & `dagster-1.7.6/dagster/_core/definitions/policy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/reconstruct.py` & `dagster-1.7.6/dagster/_core/definitions/reconstruct.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/remote_asset_graph.py` & `dagster-1.7.6/dagster/_core/definitions/remote_asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/repository_definition/__init__.py` & `dagster-1.7.6/dagster/_core/definitions/repository_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/repository_definition/caching_index.py` & `dagster-1.7.6/dagster/_core/definitions/repository_definition/caching_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/repository_definition/repository_data.py` & `dagster-1.7.6/dagster/_core/definitions/repository_definition/repository_data.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/repository_definition/repository_data_builder.py` & `dagster-1.7.6/dagster/_core/definitions/repository_definition/repository_data_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/repository_definition/repository_definition.py` & `dagster-1.7.6/dagster/_core/definitions/repository_definition/repository_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/repository_definition/valid_definitions.py` & `dagster-1.7.6/dagster/_core/definitions/repository_definition/valid_definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/resolved_asset_deps.py` & `dagster-1.7.6/dagster/_core/definitions/resolved_asset_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/resource_annotation.py` & `dagster-1.7.6/dagster/_core/definitions/resource_annotation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,55 @@
+from abc import ABC
 from inspect import Parameter
 from typing import Any, Optional, Sequence, Type, TypeVar
 
 from typing_extensions import Annotated
 
 from dagster._core.decorator_utils import get_function_params, get_type_hints
 from dagster._core.definitions.resource_definition import ResourceDefinition
+from dagster._seven import is_subclass
 
 
 def get_resource_args(fn) -> Sequence[Parameter]:
     type_annotations = get_type_hints(fn)
     return [
         param
         for param in get_function_params(fn)
         if _is_resource_annotation(type_annotations.get(param.name))
     ]
 
 
 RESOURCE_PARAM_METADATA = "resource_param"
 
 
+class TreatAsResourceParam(ABC):
+    """Marker class for types that can be used as a parameter on an annotated
+    function like `@asset`. Any type marked with this class does not require
+    a ResourceParam when used on an asset.
+
+    Example:
+        class YourClass(TreatAsResourceParam):
+            ...
+
+        @asset
+        def an_asset(your_class: YourClass):
+            ...
+    """
+
+
 def _is_resource_annotation(annotation: Optional[Type[Any]]) -> bool:
     from dagster._config.pythonic_config import ConfigurableResourceFactory
 
-    extends_resource_definition = False
-    try:
-        extends_resource_definition = isinstance(annotation, type) and issubclass(
-            annotation, (ResourceDefinition, ConfigurableResourceFactory)
-        )
-    except TypeError:
-        # Using builtin Python types in python 3.9+ will raise a TypeError when using issubclass
-        # even though the isinstance check will succeed (as will inspect.isclass), for example
-        # list[dict[str, str]] will raise a TypeError
-        pass
-
-    return (extends_resource_definition) or (
-        hasattr(annotation, "__metadata__")
-        and getattr(annotation, "__metadata__") == (RESOURCE_PARAM_METADATA,)
+    if isinstance(annotation, type) and (
+        is_subclass(annotation, ResourceDefinition)
+        or is_subclass(annotation, ConfigurableResourceFactory)
+        or is_subclass(annotation, TreatAsResourceParam)
+    ):
+        return True
+
+    return hasattr(annotation, "__metadata__") and getattr(annotation, "__metadata__") == (
+        RESOURCE_PARAM_METADATA,
     )
 
 
 T = TypeVar("T")
 ResourceParam = Annotated[T, RESOURCE_PARAM_METADATA]
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/resource_definition.py` & `dagster-1.7.6/dagster/_core/definitions/resource_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/resource_invocation.py` & `dagster-1.7.6/dagster/_core/definitions/resource_invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/resource_requirement.py` & `dagster-1.7.6/dagster/_core/definitions/resource_requirement.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/result.py` & `dagster-1.7.6/dagster/_core/definitions/result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/run_config.py` & `dagster-1.7.6/dagster/_core/definitions/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/run_config_schema.py` & `dagster-1.7.6/dagster/_core/definitions/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/run_request.py` & `dagster-1.7.6/dagster/_core/definitions/run_request.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/run_status_sensor_definition.py` & `dagster-1.7.6/dagster/_core/definitions/run_status_sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/schedule_definition.py` & `dagster-1.7.6/dagster/_core/definitions/schedule_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/scoped_resources_builder.py` & `dagster-1.7.6/dagster/_core/definitions/scoped_resources_builder.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/selector.py` & `dagster-1.7.6/dagster/_core/definitions/selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/sensor_definition.py` & `dagster-1.7.6/dagster/_core/definitions/sensor_definition.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/source_asset.py` & `dagster-1.7.6/dagster/_core/definitions/source_asset.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/step_launcher.py` & `dagster-1.7.6/dagster/_core/definitions/step_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/target.py` & `dagster-1.7.6/dagster/_core/definitions/target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/time_window_partition_mapping.py` & `dagster-1.7.6/dagster/_core/definitions/time_window_partition_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/time_window_partitions.py` & `dagster-1.7.6/dagster/_core/definitions/time_window_partitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,25 +67,28 @@
     PartitionsSubset,
     ScheduleType,
     cron_schedule_from_schedule_type_and_offsets,
 )
 from .partition_key_range import PartitionKeyRange
 
 
-def is_second_ambiguous_time(dt: datetime, tz: str):
+def is_second_ambiguous_time(dt: datetime, tz: Optional[str]):
     """Returns if a datetime is the second instance of an ambiguous time in the given timezone due
     to DST transitions.
     """
     # UTC is never ambiguous
-    if tz.upper() == "UTC":
+    if tz is not None and tz.upper() == "UTC":
         return False
 
     # Ensure that the datetime is in the correct timezone
     tzinfo = check.not_none(dt.tzinfo)
-    if tzinfo.tzname(None) != tz:
+
+    # pendulum has the non-standard "name" attribute on it's tzinfo, check for it
+    # otherwise there is no standard way of getting the IANA timezone name from datetime/tzinfo
+    if tz is not None and getattr(tzinfo, "name", None) != tz:
         dt = to_timezone(dt, tz)
         tzinfo = check.not_none(dt.tzinfo)
 
     # Only interested in the second instance of an ambiguous time
     if dt.fold == 0:
         return False
 
@@ -105,32 +108,32 @@
     transitions.
     """
     if "%z" in fmt:
         return fmt
     return fmt + "%z"
 
 
-def dst_safe_strftime(dt: datetime, tz: str, fmt: str, cron_schedule: str) -> str:
+def dst_safe_strftime(dt: datetime, tz: Optional[str], fmt: str, cron_schedule: str) -> str:
     """A method for converting a datetime to a string which will append a suffix in cases where
     the resulting timestamp would be ambiguous due to DST transitions.
-    """
-    time_str = dt.strftime(fmt)
 
+    tz is Optional. None means use the timezone on the datetime object
+    """
     # if the format already includes a UTC offset, then we don't need to do anything
-    if fmt == dst_safe_fmt(fmt):
-        return time_str
+    if "%z" in fmt:
+        return dt.strftime(fmt)
 
     # only need to handle ambiguous times for cron schedules which repeat every hour
     if not cron_string_repeats_every_hour(cron_schedule):
-        return time_str
+        return dt.strftime(fmt)
 
     # if the datetime is the second instance of an ambiguous time, then we append the UTC offset
     if is_second_ambiguous_time(dt, tz):
         return dt.strftime(dst_safe_fmt(fmt))
-    return time_str
+    return dt.strftime(fmt)
 
 
 def dst_safe_strptime(date_string: str, tz: str, fmt: str) -> PendulumDateTime:
     """A method for parsing a datetime created with the dst_safe_strftime() method."""
     try:
         # first, try to parse the datetime in the normal format
         dt = datetime.strptime(date_string, fmt)
@@ -418,18 +421,17 @@
             if self.end and time_window.end.timestamp() > self.end.timestamp():
                 reached_end = True
             if (
                 time_window.end.timestamp() <= current_timestamp
                 or partitions_past_current_time < self.end_offset
             ):
                 if idx >= start_idx and idx < end_idx:
+                    # datetimes from _iterate_time_windows have the correct tz so use None as a optimization
                     partition_keys.append(
-                        dst_safe_strftime(
-                            time_window.start, self.timezone, self.fmt, self.cron_schedule
-                        )
+                        dst_safe_strftime(time_window.start, None, self.fmt, self.cron_schedule)
                     )
                 if time_window.end.timestamp() > current_timestamp:
                     partitions_past_current_time += 1
             else:
                 break
             if len(partition_keys) >= end_idx - start_idx:
                 break
@@ -451,18 +453,17 @@
         for time_window in self._iterate_time_windows(self.start):
             if self.end and time_window.end.timestamp() > self.end.timestamp():
                 break
             if (
                 time_window.end.timestamp() <= current_timestamp
                 or partitions_past_current_time < self.end_offset
             ):
+                # datetimes from _iterate_time_windows have the correct tz so use None as a optimization
                 partition_keys.append(
-                    dst_safe_strftime(
-                        time_window.start, self.timezone, self.fmt, self.cron_schedule
-                    )
+                    dst_safe_strftime(time_window.start, None, self.fmt, self.cron_schedule)
                 )
 
                 if time_window.end.timestamp() > current_timestamp:
                     partitions_past_current_time += 1
             else:
                 break
 
@@ -525,15 +526,15 @@
         cur_windows_iterator = iter(
             self._iterate_time_windows(dst_safe_strptime(sorted_pks[0], self.timezone, self.fmt))
         )
         partition_key_time_windows: List[TimeWindow] = []
         for partition_key in sorted_pks:
             next_window = next(cur_windows_iterator)
             if (
-                dst_safe_strftime(next_window.start, self.timezone, self.fmt, self.cron_schedule)
+                dst_safe_strftime(next_window.start, None, self.fmt, self.cron_schedule)
                 == partition_key
             ):
                 partition_key_time_windows.append(next_window)
             else:
                 cur_windows_iterator = iter(
                     self._iterate_time_windows(
                         dst_safe_strptime(partition_key, self.timezone, self.fmt)
@@ -581,15 +582,15 @@
         )
         windows_iter = iter(self._iterate_time_windows(partition_key_dt))
         next(windows_iter)
         start_time = next(windows_iter).start
         if start_time.timestamp() >= last_partition_window.end.timestamp():
             return None
         else:
-            return dst_safe_strftime(start_time, self.timezone, self.fmt, self.cron_schedule)
+            return dst_safe_strftime(start_time, None, self.fmt, self.cron_schedule)
 
     def get_next_partition_window(
         self, end_dt: datetime, current_time: Optional[datetime] = None, respect_bounds: bool = True
     ) -> Optional[TimeWindow]:
         windows_iter = iter(self._iterate_time_windows(end_dt))
         next_window = next(windows_iter)
 
@@ -1885,17 +1886,19 @@
         return self.num_partitions
 
     def __contains__(self, partition_key: str) -> bool:
         time_window = cast(
             TimeWindowPartitionsDefinition, self.partitions_def
         ).time_window_for_partition_key(partition_key)
 
+        time_window_start_timestamp = time_window.start.timestamp()
+
         return any(
-            time_window.start.timestamp() >= included_time_window.start.timestamp()
-            and time_window.start.timestamp() < included_time_window.end.timestamp()
+            time_window_start_timestamp >= included_time_window.start.timestamp()
+            and time_window_start_timestamp < included_time_window.end.timestamp()
             for included_time_window in self.included_time_windows
         )
 
     def __eq__(self, other):
         return (
             isinstance(other, BaseTimeWindowPartitionsSubset)
             and self.partitions_def == other.partitions_def
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/unresolved_asset_job_definition.py` & `dagster-1.7.6/dagster/_core/definitions/unresolved_asset_job_definition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,78 +1,74 @@
 from datetime import datetime
 from typing import TYPE_CHECKING, AbstractSet, Any, Mapping, NamedTuple, Optional, Sequence, Union
 
 import dagster._check as check
 from dagster._annotations import deprecated
 from dagster._core.definitions import AssetKey
-from dagster._core.definitions.asset_job import build_asset_job, get_asset_graph_for_job
+from dagster._core.definitions.asset_job import (
+    build_asset_job,
+    get_asset_graph_for_job,
+)
+from dagster._core.definitions.asset_selection import AssetSelection
+from dagster._core.definitions.executor_definition import ExecutorDefinition
+from dagster._core.definitions.hook_definition import HookDefinition
+from dagster._core.definitions.partition import PartitionsDefinition
+from dagster._core.definitions.resource_definition import ResourceDefinition
 from dagster._core.definitions.run_request import RunRequest
 from dagster._core.errors import DagsterInvalidDefinitionError
 from dagster._core.instance import DynamicPartitionsStore
 
 from .config import ConfigMapping
 from .metadata import RawMetadataValue
+from .partition import PartitionedConfig
 from .policy import RetryPolicy
 
 if TYPE_CHECKING:
-    from dagster._core.definitions import (
-        AssetSelection,
-        ExecutorDefinition,
-        HookDefinition,
-        JobDefinition,
-        PartitionedConfig,
-        PartitionsDefinition,
-        ResourceDefinition,
-    )
+    from dagster._core.definitions import JobDefinition
     from dagster._core.definitions.asset_graph import AssetGraph
     from dagster._core.definitions.asset_selection import CoercibleToAssetSelection
     from dagster._core.definitions.run_config import RunConfig
 
 
 class UnresolvedAssetJobDefinition(
     NamedTuple(
         "_UnresolvedAssetJobDefinition",
         [
             ("name", str),
-            ("selection", "AssetSelection"),
+            ("selection", AssetSelection),
             (
                 "config",
                 Optional[Union[ConfigMapping, Mapping[str, Any], "PartitionedConfig"]],
             ),
             ("description", Optional[str]),
             ("tags", Optional[Mapping[str, Any]]),
             ("metadata", Optional[Mapping[str, RawMetadataValue]]),
-            ("partitions_def", Optional["PartitionsDefinition"]),
-            ("executor_def", Optional["ExecutorDefinition"]),
-            ("hooks", Optional[AbstractSet["HookDefinition"]]),
+            ("partitions_def", Optional[PartitionsDefinition]),
+            ("executor_def", Optional[ExecutorDefinition]),
+            ("hooks", Optional[AbstractSet[HookDefinition]]),
             ("op_retry_policy", Optional["RetryPolicy"]),
         ],
     )
 ):
     def __new__(
         cls,
         name: str,
-        selection: "AssetSelection",
+        selection: AssetSelection,
         config: Optional[
             Union[ConfigMapping, Mapping[str, Any], "PartitionedConfig", "RunConfig"]
         ] = None,
         description: Optional[str] = None,
         tags: Optional[Mapping[str, Any]] = None,
         metadata: Optional[Mapping[str, RawMetadataValue]] = None,
-        partitions_def: Optional["PartitionsDefinition"] = None,
-        executor_def: Optional["ExecutorDefinition"] = None,
-        hooks: Optional[AbstractSet["HookDefinition"]] = None,
+        partitions_def: Optional[PartitionsDefinition] = None,
+        executor_def: Optional[ExecutorDefinition] = None,
+        hooks: Optional[AbstractSet[HookDefinition]] = None,
         op_retry_policy: Optional["RetryPolicy"] = None,
     ):
-        from dagster._core.definitions import (
-            AssetSelection,
-            ExecutorDefinition,
-            HookDefinition,
-            PartitionsDefinition,
-        )
+        from dagster._core.definitions import ExecutorDefinition
         from dagster._core.definitions.run_config import convert_config_input
 
         return super(UnresolvedAssetJobDefinition, cls).__new__(
             cls,
             name=check.str_param(name, "name"),
             selection=check.inst_param(selection, "selection", AssetSelection),
             config=convert_config_input(config),
@@ -172,25 +168,50 @@
             asset_selection=asset_selection,
             partition_key=partition_key,
         )
 
     def resolve(
         self,
         asset_graph: "AssetGraph",
-        default_executor_def: Optional["ExecutorDefinition"] = None,
-        resource_defs: Optional[Mapping[str, "ResourceDefinition"]] = None,
+        default_executor_def: Optional[ExecutorDefinition] = None,
+        resource_defs: Optional[Mapping[str, ResourceDefinition]] = None,
     ) -> "JobDefinition":
         """Resolve this UnresolvedAssetJobDefinition into a JobDefinition."""
         try:
             job_asset_graph = get_asset_graph_for_job(asset_graph, self.selection)
         except DagsterInvalidDefinitionError as e:
             raise DagsterInvalidDefinitionError(
                 f'Error resolving selection for asset job "{self.name}": {e}'
             ) from e
 
+        # Require that all assets in the job have the same backfill policy
+        executable_nodes = {job_asset_graph.get(k) for k in job_asset_graph.executable_asset_keys}
+        backfill_policies = {n.backfill_policy for n in executable_nodes if n.is_partitioned}
+        if len(backfill_policies) > 1:
+            raise DagsterInvalidDefinitionError(
+                f"Asset job {self.name} materializes assets with varying BackfillPolicies. All assets"
+                " in a job must share the same BackfillPolicy."
+            )
+
+        # Error if a PartitionedConfig is defined and any target asset has a backfill policy that
+        # materializes anything other than a single partition per run. This is because
+        # PartitionedConfig is a function that maps single partition keys to run config, so it's
+        # behavior is undefined for multiple-partition runs.
+        backfill_policy = next(iter(backfill_policies), None)
+        if (
+            backfill_policy
+            and backfill_policy.max_partitions_per_run != 1
+            and isinstance(self.config, PartitionedConfig)
+        ):
+            raise DagsterInvalidDefinitionError(
+                f"Asset job {self.name} materializes an asset with a BackfillPolicy targeting multiple partitions per run,"
+                "but a PartitionedConfig was provided. PartitionedConfigs are not supported for "
+                "jobs with multi-partition-per-run backfill policies."
+            )
+
         return build_asset_job(
             self.name,
             asset_graph=job_asset_graph,
             config=self.config,
             description=self.description,
             tags=self.tags,
             metadata=self.metadata,
@@ -207,17 +228,17 @@
     selection: Optional["CoercibleToAssetSelection"] = None,
     config: Optional[
         Union[ConfigMapping, Mapping[str, Any], "PartitionedConfig", "RunConfig"]
     ] = None,
     description: Optional[str] = None,
     tags: Optional[Mapping[str, Any]] = None,
     metadata: Optional[Mapping[str, RawMetadataValue]] = None,
-    partitions_def: Optional["PartitionsDefinition"] = None,
-    executor_def: Optional["ExecutorDefinition"] = None,
-    hooks: Optional[AbstractSet["HookDefinition"]] = None,
+    partitions_def: Optional[PartitionsDefinition] = None,
+    executor_def: Optional[ExecutorDefinition] = None,
+    hooks: Optional[AbstractSet[HookDefinition]] = None,
     op_retry_policy: Optional["RetryPolicy"] = None,
 ) -> UnresolvedAssetJobDefinition:
     """Creates a definition of a job which will either materialize a selection of assets or observe
     a selection of source assets. This will only be resolved to a JobDefinition once placed in a
     code location.
 
     Args:
```

### Comparing `dagster-1.7.5/dagster/_core/definitions/utils.py` & `dagster-1.7.6/dagster/_core/definitions/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/definitions/version_strategy.py` & `dagster-1.7.6/dagster/_core/definitions/version_strategy.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/errors.py` & `dagster-1.7.6/dagster/_core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/event_api.py` & `dagster-1.7.6/dagster/_core/event_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/events/__init__.py` & `dagster-1.7.6/dagster/_core/events/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/events/log.py` & `dagster-1.7.6/dagster/_core/events/log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/events/utils.py` & `dagster-1.7.6/dagster/_core/events/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/api.py` & `dagster-1.7.6/dagster/_core/execution/api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/asset_backfill.py` & `dagster-1.7.6/dagster/_core/execution/asset_backfill.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     Iterable,
     List,
     Mapping,
     NamedTuple,
     Optional,
     Sequence,
     Set,
+    Tuple,
     Union,
     cast,
 )
 
 import pendulum
 
 import dagster._check as check
@@ -918,14 +919,15 @@
         for result in execute_asset_backfill_iteration_inner(
             backfill_id=backfill.backfill_id,
             asset_backfill_data=previous_asset_backfill_data,
             instance_queryer=instance_queryer,
             asset_graph=asset_graph,
             run_tags=backfill.tags,
             backfill_start_time=backfill_start_time,
+            logger=logger,
         ):
             yield None
 
         if not isinstance(result, AssetBackfillIterationResult):
             check.failed(
                 "Expected execute_asset_backfill_iteration_inner to return an"
                 " AssetBackfillIterationResult"
@@ -1147,21 +1149,24 @@
     asset_graph: RemoteAssetGraph,
     instance_queryer: CachingInstanceQueryer,
     backfill_start_time: datetime,
 ) -> AssetGraphSubset:
     failed_and_downstream_subset = AssetGraphSubset.from_asset_partition_set(
         asset_graph.bfs_filter_asset_partitions(
             instance_queryer,
-            lambda asset_partitions, _: any(
-                asset_partition in asset_backfill_data.target_subset
-                for asset_partition in asset_partitions
+            lambda asset_partitions, _: (
+                any(
+                    asset_partition in asset_backfill_data.target_subset
+                    for asset_partition in asset_partitions
+                ),
+                "",
             ),
             _get_failed_asset_partitions(instance_queryer, backfill_id, asset_graph),
             evaluation_time=backfill_start_time,
-        ),
+        )[0],
         asset_graph,
     )
     return failed_and_downstream_subset
 
 
 def _get_next_latest_storage_id(instance_queryer: CachingInstanceQueryer) -> int:
     # Events are not always guaranteed to be written to the event log in monotonically increasing
@@ -1180,33 +1185,36 @@
 def execute_asset_backfill_iteration_inner(
     backfill_id: str,
     asset_backfill_data: AssetBackfillData,
     asset_graph: RemoteAssetGraph,
     instance_queryer: CachingInstanceQueryer,
     run_tags: Mapping[str, str],
     backfill_start_time: datetime,
+    logger: logging.Logger,
 ) -> Iterable[Optional[AssetBackfillIterationResult]]:
     """Core logic of a backfill iteration. Has no side effects.
 
     Computes which runs should be requested, if any, as well as updated bookkeeping about the status
     of asset partitions targeted by the backfill.
 
     This is a generator so that we can return control to the daemon and let it heartbeat during
     expensive operations.
     """
     initial_candidates: Set[AssetKeyPartitionKey] = set()
     request_roots = not asset_backfill_data.requested_runs_for_target_roots
     if request_roots:
+        logger.info("Not all root assets have been requested, finding root assets.")
         target_roots = asset_backfill_data.get_target_root_asset_partitions(instance_queryer)
         # Because the code server may have failed while requesting roots, some roots may have
         # already been requested. Checking here will reduce the amount of BFS work later in the iteration.
         not_yet_requested = [
             root for root in target_roots if root not in asset_backfill_data.requested_subset
         ]
         initial_candidates.update(not_yet_requested)
+        logger.info(f"Root assets that have not yet been requested: {initial_candidates}")
 
         yield None
 
         updated_materialized_subset = AssetGraphSubset()
         failed_and_downstream_subset = AssetGraphSubset()
         next_latest_storage_id = _get_next_latest_storage_id(instance_queryer)
     else:
@@ -1226,14 +1234,18 @@
 
         if not isinstance(updated_materialized_subset, AssetGraphSubset):
             check.failed(
                 "Expected get_asset_backfill_iteration_materialized_partitions to return an"
                 " AssetGraphSubset"
             )
 
+        logger.info(
+            f"Assets materialized since last tick {updated_materialized_subset - asset_backfill_data.materialized_subset}"
+        )
+
         parent_materialized_asset_partitions = set().union(
             *(
                 instance_queryer.asset_partitions_with_newly_updated_parents_and_new_cursor(
                     latest_storage_id=asset_backfill_data.latest_storage_id,
                     child_asset_key=asset_key,
                 )[0]
                 for asset_key in asset_backfill_data.target_subset.asset_keys
@@ -1245,29 +1257,44 @@
 
         failed_and_downstream_subset = _get_failed_and_downstream_asset_partitions(
             backfill_id, asset_backfill_data, asset_graph, instance_queryer, backfill_start_time
         )
 
         yield None
 
-    asset_partitions_to_request = asset_graph.bfs_filter_asset_partitions(
-        instance_queryer,
-        lambda unit, visited: should_backfill_atomic_asset_partitions_unit(
-            candidates_unit=unit,
-            asset_partitions_to_request=visited,
-            asset_graph=asset_graph,
-            materialized_subset=updated_materialized_subset,
-            requested_subset=asset_backfill_data.requested_subset,
-            target_subset=asset_backfill_data.target_subset,
-            failed_and_downstream_subset=failed_and_downstream_subset,
-            dynamic_partitions_store=instance_queryer,
-            current_time=backfill_start_time,
-        ),
-        initial_asset_partitions=initial_candidates,
-        evaluation_time=backfill_start_time,
+    asset_partitions_to_request, not_requested_and_reasons = (
+        asset_graph.bfs_filter_asset_partitions(
+            instance_queryer,
+            lambda unit, visited: should_backfill_atomic_asset_partitions_unit(
+                candidates_unit=unit,
+                asset_partitions_to_request=visited,
+                asset_graph=asset_graph,
+                materialized_subset=updated_materialized_subset,
+                requested_subset=asset_backfill_data.requested_subset,
+                target_subset=asset_backfill_data.target_subset,
+                failed_and_downstream_subset=failed_and_downstream_subset,
+                dynamic_partitions_store=instance_queryer,
+                current_time=backfill_start_time,
+            ),
+            initial_asset_partitions=initial_candidates,
+            evaluation_time=backfill_start_time,
+        )
+    )
+
+    logger.info(
+        f"After BFS-should-backfill filter, asset partitions to request: {asset_partitions_to_request}"
+    )
+    not_requested_str = (
+        "\n"
+        + "\n".join([f"{keys} - Reason: {reason}." for keys, reason in not_requested_and_reasons])
+        if len(not_requested_and_reasons) > 0
+        else "None"
+    )
+    logger.info(
+        f"The following assets were considered for materialization but not requested:  {not_requested_str}"
     )
 
     # check if all assets have backfill policies if any of them do, otherwise, raise error
     asset_backfill_policies = [
         asset_graph.get(asset_key).backfill_policy
         for asset_key in {
             asset_partition.asset_key for asset_partition in asset_partitions_to_request
@@ -1322,17 +1349,17 @@
 def can_run_with_parent(
     parent: AssetKeyPartitionKey,
     candidate: AssetKeyPartitionKey,
     candidates_unit: Iterable[AssetKeyPartitionKey],
     asset_graph: RemoteAssetGraph,
     target_subset: AssetGraphSubset,
     asset_partitions_to_request_map: Mapping[AssetKey, AbstractSet[Optional[str]]],
-) -> bool:
+) -> Tuple[bool, str]:
     """Returns if a given candidate can be materialized in the same run as a given parent on
-    this tick.
+    this tick, and the reason it cannot be materialized, if applicable.
     """
     parent_target_subset = target_subset.get_asset_subset(parent.asset_key, asset_graph)
     candidate_target_subset = target_subset.get_asset_subset(candidate.asset_key, asset_graph)
     partition_mapping = asset_graph.get_partition_mapping(
         candidate.asset_key, parent_asset_key=parent.asset_key
     )
 
@@ -1349,73 +1376,98 @@
         # mapping functions as an identity partition mapping
         or (
             isinstance(partition_mapping, TimeWindowPartitionMapping)
             and partition_mapping.start_offset == 0
             and partition_mapping.end_offset == 0
         )
     )
-    return (
-        parent_node.backfill_policy == candidate_node.backfill_policy
-        and parent_node.priority_repository_handle is candidate_node.priority_repository_handle
-        and parent_node.partitions_def == candidate_node.partitions_def
-        and (
-            parent.partition_key in asset_partitions_to_request_map[parent.asset_key]
-            or parent in candidates_unit
-        )
-        and (
-            # if there is a simple mapping between the parent and the child, then
-            # with the parent
-            has_identity_partition_mapping
-            # if there is not a simple mapping, we can only materialize this asset with its
-            # parent if...
-            or (
-                # there is a backfill policy for the parent
-                parent_node.backfill_policy is not None
-                # the same subset of parents is targeted as the child
-                and parent_target_subset.value == candidate_target_subset.value
-                and (
-                    # there is no limit on the size of a single run or...
-                    parent_node.backfill_policy.max_partitions_per_run is None
-                    # a single run can materialize all requested parent partitions
-                    or parent_node.backfill_policy.max_partitions_per_run
-                    > len(asset_partitions_to_request_map[parent.asset_key])
-                )
-                # all targeted parents are being requested this tick
-                and len(asset_partitions_to_request_map[parent.asset_key])
-                == parent_target_subset.size
+    if parent_node.backfill_policy != candidate_node.backfill_policy:
+        return (
+            False,
+            f"parent {parent_node.key} and {candidate_node.key} have different backfill policies",
+        )
+    if parent_node.priority_repository_handle is not candidate_node.priority_repository_handle:
+        return (
+            False,
+            f"parent {parent_node.key} and {candidate_node.key} are in different code locations",
+        )
+    if parent_node.partitions_def != candidate_node.partitions_def:
+        return (
+            False,
+            f"parent {parent_node.key} and {candidate_node.key} have different partitions definitions",
+        )
+    if (
+        parent.partition_key not in asset_partitions_to_request_map[parent.asset_key]
+        and parent not in candidates_unit
+    ):
+        return (
+            False,
+            f"parent {parent.asset_key} with partition key {parent.partition_key} is not requested in this iteration",
+        )
+    if (
+        # if there is a simple mapping between the parent and the child, then
+        # with the parent
+        has_identity_partition_mapping
+        # if there is not a simple mapping, we can only materialize this asset with its
+        # parent if...
+        or (
+            # there is a backfill policy for the parent
+            parent_node.backfill_policy is not None
+            # the same subset of parents is targeted as the child
+            and parent_target_subset.value == candidate_target_subset.value
+            and (
+                # there is no limit on the size of a single run or...
+                parent_node.backfill_policy.max_partitions_per_run is None
+                # a single run can materialize all requested parent partitions
+                or parent_node.backfill_policy.max_partitions_per_run
+                > len(asset_partitions_to_request_map[parent.asset_key])
             )
-            # if all the above are true, then a single run can be launched this tick which
-            # will materialize all requested partitions
+            # all targeted parents are being requested this tick
+            and len(asset_partitions_to_request_map[parent.asset_key]) == parent_target_subset.size
         )
-    )
+    ):
+        return True, ""
+    else:
+        failed_reason = (
+            f"partition mapping between {parent_node.key} and {candidate_node.key} is not simple and "
+            f"{parent_node.key} does not meet requirements of: targeting the same partitions as "
+            f"{candidate_node.key}, have all of its partitions requested in this iteration, having "
+            "a backfill policy, and that backfill policy size limit is not exceeded by adding "
+            f"{candidate_node.key} to the run."
+        )
+        return False, failed_reason
 
 
 def should_backfill_atomic_asset_partitions_unit(
     asset_graph: RemoteAssetGraph,
     candidates_unit: Iterable[AssetKeyPartitionKey],
     asset_partitions_to_request: AbstractSet[AssetKeyPartitionKey],
     target_subset: AssetGraphSubset,
     requested_subset: AssetGraphSubset,
     materialized_subset: AssetGraphSubset,
     failed_and_downstream_subset: AssetGraphSubset,
     dynamic_partitions_store: DynamicPartitionsStore,
     current_time: datetime,
-) -> bool:
+) -> Tuple[bool, str]:
     """Args:
     candidates_unit: A set of asset partitions that must all be materialized if any is
         materialized.
+
+    returns if the candidates_unit can be materialized in this tick of the backfill, and the reason
+    it cannot, if applicable
     """
     for candidate in candidates_unit:
-        if (
-            candidate not in target_subset
-            or candidate in failed_and_downstream_subset
-            or candidate in materialized_subset
-            or candidate in requested_subset
-        ):
-            return False
+        if candidate not in target_subset:
+            return False, f"{candidate} not targeted by backfill"
+        elif candidate in failed_and_downstream_subset:
+            return False, f"{candidate} in failed and downstream subset"
+        elif candidate in materialized_subset:
+            return False, f"{candidate} already materialized by backfill"
+        elif candidate in requested_subset:
+            return False, f"{candidate} already requested by backfill"
 
         parent_partitions_result = asset_graph.get_parents_partitions(
             dynamic_partitions_store, current_time, *candidate
         )
         if parent_partitions_result.required_but_nonexistent_parents_partitions:
             raise DagsterInvariantViolationError(
                 f"Asset partition {candidate}"
@@ -1426,29 +1478,27 @@
         asset_partitions_to_request_map: Dict[AssetKey, Set[Optional[str]]] = defaultdict(set)
         for asset_partition in asset_partitions_to_request:
             asset_partitions_to_request_map[asset_partition.asset_key].add(
                 asset_partition.partition_key
             )
 
         for parent in parent_partitions_result.parent_partitions:
-            if (
-                parent in target_subset
-                and parent not in materialized_subset
-                and not can_run_with_parent(
+            if parent in target_subset and parent not in materialized_subset:
+                can_run, failed_reason = can_run_with_parent(
                     parent,
                     candidate,
                     candidates_unit,
                     asset_graph,
                     target_subset,
                     asset_partitions_to_request_map,
                 )
-            ):
-                return False
+                if not can_run:
+                    return False, failed_reason
 
-    return True
+    return True, ""
 
 
 def _get_failed_asset_partitions(
     instance_queryer: CachingInstanceQueryer, backfill_id: str, asset_graph: RemoteAssetGraph
 ) -> Sequence[AssetKeyPartitionKey]:
     """Returns asset partitions that materializations were requested for as part of the backfill, but
     will not be materialized.
```

### Comparing `dagster-1.7.5/dagster/_core/execution/backfill.py` & `dagster-1.7.6/dagster/_core/execution/backfill.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/build_resources.py` & `dagster-1.7.6/dagster/_core/execution/build_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/compute_logs.py` & `dagster-1.7.6/dagster/_core/execution/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/context/compute.py` & `dagster-1.7.6/dagster/_core/execution/context/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/context/data_version_cache.py` & `dagster-1.7.6/dagster/_core/execution/context/data_version_cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from typing import TYPE_CHECKING
 
 """This module contains the execution context objects that are internal to the system.
 Not every property on these should be exposed to random Jane or Joe dagster user
 so we have a different layer of objects that encode the explicit public API
 in the user_context module.
 """
@@ -25,14 +26,15 @@
 
 if TYPE_CHECKING:
     from dagster._core.definitions.data_version import (
         DataVersion,
     )
     from dagster._core.event_api import EventLogRecord
     from dagster._core.events import DagsterEventType
+    from dagster._core.storage.event_log.base import AssetRecord
 
 
 if TYPE_CHECKING:
     from dagster._core.execution.context.compute import StepExecutionContext
 
 
 @dataclass
@@ -72,15 +74,15 @@
     def get_data_version(self, asset_key: AssetKey) -> "DataVersion":
         return self.values[asset_key]
 
     def maybe_fetch_and_get_input_asset_version_info(
         self, key: AssetKey
     ) -> Optional["InputAssetVersionInfo"]:
         if key not in self.input_asset_version_info:
-            self._fetch_input_asset_version_info(key)
+            self._fetch_input_asset_version_info([key])
         return self.input_asset_version_info[key]
 
     # "external" refers to records for inputs generated outside of this step
     def fetch_external_input_asset_version_info(self) -> None:
         output_keys = self._context.get_output_asset_keys()
 
         all_dep_keys: List[AssetKey] = []
@@ -89,65 +91,96 @@
                 continue
             dep_keys = self._context.job_def.asset_layer.get(output_key).parent_keys
             for key in dep_keys:
                 if key not in all_dep_keys and key not in output_keys:
                     all_dep_keys.append(key)
 
         self.input_asset_version_info = {}
-        for key in all_dep_keys:
-            self._fetch_input_asset_version_info(key)
+        self._fetch_input_asset_version_info(all_dep_keys)
         self.is_external_input_asset_version_info_loaded = True
 
-    def _fetch_input_asset_version_info(self, key: AssetKey) -> None:
+    def _fetch_input_asset_version_info(self, asset_keys: Sequence[AssetKey]) -> None:
         from dagster._core.definitions.data_version import (
             extract_data_version_from_entry,
         )
 
-        event = self._get_input_asset_event(key)
-        if event is None:
-            self.input_asset_version_info[key] = None
-        else:
-            storage_id = event.storage_id
-            # Input name will be none if this is an internal dep
-            input_name = self._context.job_def.asset_layer.input_for_asset_key(
-                self._context.node_handle, key
-            )
-            # Exclude AllPartitionMapping for now to avoid huge queries
-            if input_name and self._context.has_asset_partitions_for_input(input_name):
-                subset = self._context.asset_partitions_subset_for_input(
-                    input_name, require_valid_partitions=False
+        asset_records_by_key = self._fetch_asset_records(asset_keys)
+        for key in asset_keys:
+            asset_record = asset_records_by_key.get(key)
+            event = self._get_input_asset_event(key, asset_record)
+            if event is None:
+                self.input_asset_version_info[key] = None
+            else:
+                storage_id = event.storage_id
+                # Input name will be none if this is an internal dep
+                input_name = self._context.job_def.asset_layer.input_for_asset_key(
+                    self._context.node_handle, key
                 )
-                input_keys = list(subset.get_partition_keys())
-
-                # This check represents a temporary constraint that prevents huge query results for upstream
-                # partition data versions from timing out runs. If a partitioned dependency (a) uses an
-                # AllPartitionMapping; and (b) has greater than or equal to
-                # SKIP_PARTITION_DATA_VERSION_DEPENDENCY_THRESHOLD dependency partitions, then we
-                # process it as a non-partitioned dependency (note that this was the behavior for
-                # all partition dependencies prior to 2023-08).  This means that stale status
-                # results cannot be accurately computed for the dependency, and there is thus
-                # corresponding logic in the CachingStaleStatusResolver to account for this. This
-                # constraint should be removed when we have thoroughly examined the performance of
-                # the data version retrieval query and can guarantee decent performance.
-                if len(input_keys) < SKIP_PARTITION_DATA_VERSION_DEPENDENCY_THRESHOLD:
-                    data_version = self._get_partitions_data_version_from_keys(key, input_keys)
+                # Exclude AllPartitionMapping for now to avoid huge queries
+                if input_name and self._context.has_asset_partitions_for_input(input_name):
+                    subset = self._context.asset_partitions_subset_for_input(
+                        input_name, require_valid_partitions=False
+                    )
+                    input_keys = list(subset.get_partition_keys())
+
+                    # This check represents a temporary constraint that prevents huge query results for upstream
+                    # partition data versions from timing out runs. If a partitioned dependency (a) uses an
+                    # AllPartitionMapping; and (b) has greater than or equal to
+                    # SKIP_PARTITION_DATA_VERSION_DEPENDENCY_THRESHOLD dependency partitions, then we
+                    # process it as a non-partitioned dependency (note that this was the behavior for
+                    # all partition dependencies prior to 2023-08).  This means that stale status
+                    # results cannot be accurately computed for the dependency, and there is thus
+                    # corresponding logic in the CachingStaleStatusResolver to account for this. This
+                    # constraint should be removed when we have thoroughly examined the performance of
+                    # the data version retrieval query and can guarantee decent performance.
+                    if len(input_keys) < SKIP_PARTITION_DATA_VERSION_DEPENDENCY_THRESHOLD:
+                        data_version = self._get_partitions_data_version_from_keys(key, input_keys)
+                    else:
+                        data_version = extract_data_version_from_entry(event.event_log_entry)
                 else:
                     data_version = extract_data_version_from_entry(event.event_log_entry)
-            else:
-                data_version = extract_data_version_from_entry(event.event_log_entry)
-            self.input_asset_version_info[key] = InputAssetVersionInfo(
-                storage_id,
-                check.not_none(event.event_log_entry.dagster_event).event_type,
-                data_version,
-                event.run_id,
-                event.timestamp,
+                self.input_asset_version_info[key] = InputAssetVersionInfo(
+                    storage_id,
+                    check.not_none(event.event_log_entry.dagster_event).event_type,
+                    data_version,
+                    event.run_id,
+                    event.timestamp,
+                )
+
+    def _fetch_asset_records(self, asset_keys: Sequence[AssetKey]) -> Dict[AssetKey, "AssetRecord"]:
+        batch_size = int(os.getenv("GET_ASSET_RECORDS_FOR_DATA_VERSION_BATCH_SIZE", "100"))
+        asset_records_by_key = {}
+        to_fetch = asset_keys
+        while len(to_fetch):
+            for record in self._context.instance.get_asset_records(to_fetch[:batch_size]):
+                asset_records_by_key[record.asset_entry.asset_key] = record
+            to_fetch = to_fetch[batch_size:]
+
+        return asset_records_by_key
+
+    def _get_input_asset_event(
+        self, key: AssetKey, asset_record: Optional["AssetRecord"]
+    ) -> Optional["EventLogRecord"]:
+        event = None
+        if asset_record and asset_record.asset_entry.last_materialization_record:
+            event = asset_record.asset_entry.last_materialization_record
+        elif (
+            asset_record
+            and self._context.instance.event_log_storage.asset_records_have_last_observation
+        ):
+            event = asset_record.asset_entry.last_observation_record
+
+        if (
+            not event
+            and not self._context.instance.event_log_storage.asset_records_have_last_observation
+        ):
+            event = next(
+                iter(self._context.instance.fetch_observations(key, limit=1).records), None
             )
 
-    def _get_input_asset_event(self, key: AssetKey) -> Optional["EventLogRecord"]:
-        event = self._context.instance.get_latest_data_version_record(key)
         if event:
             self._check_input_asset_event(key, event)
         return event
 
     def _check_input_asset_event(self, key: AssetKey, event: "EventLogRecord") -> None:
         assert event.event_log_entry
         event_data_version = extract_data_version_from_entry(event.event_log_entry)
```

### Comparing `dagster-1.7.5/dagster/_core/execution/context/hook.py` & `dagster-1.7.6/dagster/_core/execution/context/hook.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/context/init.py` & `dagster-1.7.6/dagster/_core/execution/context/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/context/input.py` & `dagster-1.7.6/dagster/_core/execution/context/input.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/context/invocation.py` & `dagster-1.7.6/dagster/_core/execution/context/invocation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/context/logger.py` & `dagster-1.7.6/dagster/_core/execution/context/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/context/output.py` & `dagster-1.7.6/dagster/_core/execution/context/output.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/context/system.py` & `dagster-1.7.6/dagster/_core/execution/context/system.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/context_creation_job.py` & `dagster-1.7.6/dagster/_core/execution/context_creation_job.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/execute_in_process.py` & `dagster-1.7.6/dagster/_core/execution/execute_in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/execute_in_process_result.py` & `dagster-1.7.6/dagster/_core/execution/execute_in_process_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/execution_result.py` & `dagster-1.7.6/dagster/_core/execution/execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/host_mode.py` & `dagster-1.7.6/dagster/_core/execution/host_mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/job_backfill.py` & `dagster-1.7.6/dagster/_core/execution/job_backfill.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import logging
 import time
-from typing import Callable, Iterable, Mapping, Optional, Sequence, Tuple, cast
+from typing import Any, Callable, Iterable, Mapping, Optional, Sequence, Tuple, Union, cast
 
 import dagster._check as check
+from dagster._core.definitions.partition import PartitionsDefinition
+from dagster._core.definitions.partition_key_range import PartitionKeyRange
 from dagster._core.definitions.selector import JobSubsetSelector
 from dagster._core.errors import DagsterBackfillFailedError
 from dagster._core.execution.plan.resume_retry import ReexecutionStrategy
 from dagster._core.execution.plan.state import KnownExecutionState
 from dagster._core.instance import DagsterInstance
 from dagster._core.remote_representation import (
     CodeLocation,
     ExternalJob,
     ExternalPartitionSet,
 )
 from dagster._core.remote_representation.external_data import (
-    ExternalPartitionExecutionParamData,
     ExternalPartitionSetExecutionParamData,
 )
 from dagster._core.remote_representation.origin import RemotePartitionSetOrigin
 from dagster._core.storage.dagster_run import DagsterRun, DagsterRunStatus, RunsFilter
 from dagster._core.storage.tags import (
+    ASSET_PARTITION_RANGE_END_TAG,
+    ASSET_PARTITION_RANGE_START_TAG,
     PARENT_RUN_ID_TAG,
     PARTITION_NAME_TAG,
     PARTITION_SET_TAG,
     ROOT_RUN_ID_TAG,
 )
 from dagster._core.telemetry import BACKFILL_RUN_CREATED, hash_name, log_action
 from dagster._core.utils import make_new_run_id
@@ -47,30 +50,34 @@
     backfill: PartitionBackfill,
     logger: logging.Logger,
     workspace_process_context: IWorkspaceProcessContext,
     debug_crash_flags: Optional[Mapping[str, int]],
     instance: DagsterInstance,
 ) -> Iterable[Optional[SerializableErrorInfo]]:
     if not backfill.last_submitted_partition_name:
-        logger.info(f"Starting backfill for {backfill.backfill_id}")
+        logger.info(f"Starting job backfill for {backfill.backfill_id}")
     else:
         logger.info(
-            f"Resuming backfill for {backfill.backfill_id} from"
+            f"Resuming job backfill for {backfill.backfill_id} from"
             f" {backfill.last_submitted_partition_name}"
         )
 
-    _check_repo_has_partition_set(workspace_process_context, backfill)
+    partition_set = _get_partition_set(workspace_process_context, backfill)
 
     has_more = True
     while has_more:
         if backfill.status != BulkActionStatus.REQUESTED:
             break
 
         chunk, checkpoint, has_more = _get_partitions_chunk(
-            instance, logger, backfill, CHECKPOINT_COUNT
+            instance,
+            logger,
+            backfill,
+            CHECKPOINT_COUNT,
+            partition_set,
         )
         check_for_debug_crash(debug_crash_flags, "BEFORE_SUBMIT")
 
         if chunk:
             for _run_id in submit_backfill_runs(
                 instance,
                 lambda: workspace_process_context.create_request_context(),
@@ -97,17 +104,17 @@
                 f"Backfill completed for {backfill.backfill_id} for"
                 f" {len(partition_names)} partitions"
             )
             instance.update_backfill(backfill.with_status(BulkActionStatus.COMPLETED))
             yield None
 
 
-def _check_repo_has_partition_set(
+def _get_partition_set(
     workspace_process_context: IWorkspaceProcessContext, backfill_job: PartitionBackfill
-) -> None:
+) -> ExternalPartitionSet:
     origin = cast(RemotePartitionSetOrigin, backfill_job.partition_set_origin)
 
     location_name = origin.repository_origin.code_location_origin.location_name
 
     workspace = workspace_process_context.create_request_context()
     code_location = workspace.get_code_location(location_name)
 
@@ -120,22 +127,44 @@
 
     partition_set_name = origin.partition_set_name
     external_repo = code_location.get_repository(repo_name)
     if not external_repo.has_external_partition_set(partition_set_name):
         raise DagsterBackfillFailedError(
             f"Could not find partition set {partition_set_name} in repository {repo_name}. "
         )
+    return external_repo.get_external_partition_set(partition_set_name)
+
+
+def _subdivide_partition_key_range(
+    partitions_def: PartitionsDefinition,
+    partition_key_range: PartitionKeyRange,
+    instance: DagsterInstance,
+    max_range_size: Optional[int],
+) -> Sequence[PartitionKeyRange]:
+    """Take a partition key range and subdivide it into smaller ranges of size max_range_size. This
+    is done to satisfy backfill policies that limit the maximum number of partitions that can be
+    materialized in a run.
+    """
+    if max_range_size is None:
+        return [partition_key_range]
+    else:
+        keys = partitions_def.get_partition_keys_in_range(
+            partition_key_range, dynamic_partitions_store=instance
+        )
+        chunks = [keys[i : i + max_range_size] for i in range(0, len(keys), max_range_size)]
+        return [PartitionKeyRange(start=chunk[0], end=chunk[-1]) for chunk in chunks]
 
 
 def _get_partitions_chunk(
     instance: DagsterInstance,
     logger: logging.Logger,
     backfill_job: PartitionBackfill,
     chunk_size: int,
-) -> Tuple[Sequence[str], str, bool]:
+    partition_set: ExternalPartitionSet,
+) -> Tuple[Sequence[Union[str, PartitionKeyRange]], str, bool]:
     partition_names = cast(Sequence[str], backfill_job.partition_names)
     checkpoint = backfill_job.last_submitted_partition_name
 
     if (
         backfill_job.last_submitted_partition_name
         and backfill_job.last_submitted_partition_name in partition_names
     ):
@@ -147,87 +176,148 @@
         RunsFilter(tags=DagsterRun.tags_for_backfill_id(backfill_job.backfill_id))
     )
     completed_partitions = set([run.tags.get(PARTITION_NAME_TAG) for run in backfill_runs])
     initial_checkpoint = (
         partition_names.index(checkpoint) + 1 if checkpoint and checkpoint in partition_names else 0
     )
     partition_names = partition_names[initial_checkpoint:]
-    has_more = chunk_size < len(partition_names)
-    partitions_chunk = partition_names[:chunk_size]
-    next_checkpoint = partitions_chunk[-1]
 
-    to_skip = set(partitions_chunk).intersection(completed_partitions)
-    if to_skip:
-        logger.info(
-            f"Found {len(to_skip)} existing runs for backfill {backfill_job.backfill_id}, skipping"
+    partitions_def = partition_set.get_partitions_definition()
+    backfill_policy = partition_set.backfill_policy
+    if backfill_policy and backfill_policy.max_partitions_per_run != 1:
+        partitions_subset = partitions_def.subset_with_partition_keys(partition_names)
+        partition_key_ranges = partitions_subset.get_partition_key_ranges(
+            partitions_def, dynamic_partitions_store=instance
         )
-    to_submit = [
-        partition_name
-        for partition_name in partitions_chunk
-        if partition_name not in completed_partitions
-    ]
+        subdivided_ranges = [
+            sr
+            for r in partition_key_ranges
+            for sr in _subdivide_partition_key_range(
+                partitions_def, r, instance, backfill_policy.max_partitions_per_run
+            )
+        ]
+        ranges_to_launch = subdivided_ranges[:chunk_size]
+        has_more = chunk_size < len(subdivided_ranges)
+        next_checkpoint = ranges_to_launch[-1].end
+        to_submit = ranges_to_launch
+    else:
+        has_more = chunk_size < len(partition_names)
+        partitions_chunk = partition_names[:chunk_size]
+        next_checkpoint = partitions_chunk[-1]
+        to_skip = set(partitions_chunk).intersection(completed_partitions)
+        if to_skip:
+            logger.info(
+                f"Found {len(to_skip)} existing runs for backfill {backfill_job.backfill_id}, skipping"
+            )
+        to_submit = [
+            partition_name
+            for partition_name in partitions_chunk
+            if partition_name not in completed_partitions
+        ]
+
     return to_submit, next_checkpoint, has_more
 
 
 def submit_backfill_runs(
     instance: DagsterInstance,
     create_workspace: Callable[[], BaseWorkspaceRequestContext],
     backfill_job: PartitionBackfill,
-    partition_names: Optional[Sequence[str]] = None,
+    partition_names_or_ranges: Optional[Sequence[Union[str, PartitionKeyRange]]] = None,
 ) -> Iterable[Optional[str]]:
     """Returns the run IDs of the submitted runs."""
     origin = cast(RemotePartitionSetOrigin, backfill_job.partition_set_origin)
 
     repository_origin = origin.repository_origin
     repo_name = repository_origin.repository_name
     location_name = repository_origin.code_location_origin.location_name
 
-    if not partition_names:
-        partition_names = cast(Sequence[str], backfill_job.partition_names)
+    if not partition_names_or_ranges:
+        partition_names_or_ranges = cast(Sequence[str], backfill_job.partition_names)
 
     workspace = create_workspace()
     code_location = workspace.get_code_location(location_name)
-
     check.invariant(
         code_location.has_repository(repo_name),
         f"Could not find repository {repo_name} in location {code_location.name}",
     )
     external_repo = code_location.get_repository(repo_name)
     partition_set_name = origin.partition_set_name
     external_partition_set = external_repo.get_external_partition_set(partition_set_name)
-    result = code_location.get_external_partition_set_execution_param_data(
-        external_repo.handle, partition_set_name, partition_names, instance
-    )
 
-    assert isinstance(result, ExternalPartitionSetExecutionParamData)
     if backfill_job.asset_selection:
         # need to make another call to the user code location to properly subset
         # for an asset selection
         pipeline_selector = JobSubsetSelector(
             location_name=code_location.name,
             repository_name=repo_name,
             job_name=external_partition_set.job_name,
             op_selection=None,
             asset_selection=backfill_job.asset_selection,
         )
         external_job = code_location.get_external_job(pipeline_selector)
     else:
         external_job = external_repo.get_full_external_job(external_partition_set.job_name)
-    for partition_data in result.partition_data:
+
+    partition_data_target = check.is_list(
+        [partition_names_or_ranges[0].start]
+        if isinstance(partition_names_or_ranges[0], PartitionKeyRange)
+        else partition_names_or_ranges,
+        of_type=str,
+    )
+    partition_set_execution_data = code_location.get_external_partition_set_execution_param_data(
+        external_repo.handle,
+        partition_set_name,
+        partition_data_target,
+        instance,
+    )
+    assert isinstance(partition_set_execution_data, ExternalPartitionSetExecutionParamData)
+
+    # Partition-scoped run config is prohibited at the definitions level for a jobs that materialize
+    # ranges, so we can assume that all partition data will have the same run config and tags as the
+    # first partition.
+    tags_by_key_or_range: Mapping[Union[str, PartitionKeyRange], Mapping[str, str]]
+    run_config_by_key_or_range: Mapping[Union[str, PartitionKeyRange], Mapping[str, Any]]
+    if isinstance(partition_names_or_ranges[0], PartitionKeyRange):
+        run_config = partition_set_execution_data.partition_data[0].run_config
+        tags = {
+            k: v
+            for k, v in partition_set_execution_data.partition_data[0].tags.items()
+            if k != PARTITION_NAME_TAG
+        }
+        run_config_by_key_or_range = {r: run_config for r in partition_names_or_ranges}
+        tags_by_key_or_range = {
+            r: {
+                **tags,
+                ASSET_PARTITION_RANGE_START_TAG: r.start,
+                ASSET_PARTITION_RANGE_END_TAG: r.end,
+            }
+            for r in check.is_list(partition_names_or_ranges, of_type=PartitionKeyRange)
+        }
+    else:
+        run_config_by_key_or_range = {
+            pd.name: pd.run_config for pd in partition_set_execution_data.partition_data
+        }
+        tags_by_key_or_range = {
+            pd.name: pd.tags for pd in partition_set_execution_data.partition_data
+        }
+
+    for key_or_range in partition_names_or_ranges:
         # Refresh the code location in case the workspace has reloaded mid-backfill
         workspace = create_workspace()
         code_location = workspace.get_code_location(location_name)
 
         dagster_run = create_backfill_run(
             instance,
             code_location,
             external_job,
             external_partition_set,
             backfill_job,
-            partition_data,
+            key_or_range,
+            run_tags=tags_by_key_or_range[key_or_range],
+            run_config=run_config_by_key_or_range[key_or_range],
         )
         if dagster_run:
             # we skip runs in certain cases, e.g. we are running a `from_failure` backfill job
             # and the partition has had a successful run since the time the backfill was
             # scheduled
             instance.submit_run(dagster_run.run_id, workspace)
             yield dagster_run.run_id
@@ -236,15 +326,17 @@
 
 def create_backfill_run(
     instance: DagsterInstance,
     code_location: CodeLocation,
     external_pipeline: ExternalJob,
     external_partition_set: ExternalPartitionSet,
     backfill_job: PartitionBackfill,
-    partition_data: ExternalPartitionExecutionParamData,
+    partition_key_or_range: Union[str, PartitionKeyRange],
+    run_tags: Mapping[str, str],
+    run_config: Mapping[str, Any],
 ) -> Optional[DagsterRun]:
     from dagster._daemon.daemon import get_telemetry_daemon_session_id
 
     log_action(
         instance,
         BACKFILL_RUN_CREATED,
         metadata={
@@ -252,15 +344,15 @@
             "repo_hash": hash_name(code_location.name),
             "pipeline_name_hash": hash_name(external_pipeline.name),
         },
     )
 
     tags = merge_dicts(
         external_pipeline.tags,
-        partition_data.tags,
+        run_tags,
         DagsterRun.tags_for_backfill_id(backfill_job.backfill_id),
         backfill_job.tags,
     )
 
     resolved_op_selection = None
     op_selection = None
     if not backfill_job.from_failure and not backfill_job.reexecution_steps:
@@ -269,29 +361,29 @@
         root_run_id = None
         known_state = None
         if external_partition_set.op_selection:
             resolved_op_selection = frozenset(external_partition_set.op_selection)
             op_selection = external_partition_set.op_selection
 
     elif backfill_job.from_failure:
-        last_run = _fetch_last_run(instance, external_partition_set, partition_data.name)
+        last_run = _fetch_last_run(instance, external_partition_set, partition_key_or_range)
         if not last_run or last_run.status != DagsterRunStatus.FAILURE:
             return None
         return instance.create_reexecuted_run(
             parent_run=last_run,
             code_location=code_location,
             external_job=external_pipeline,
             strategy=ReexecutionStrategy.FROM_FAILURE,
             extra_tags=tags,
-            run_config=partition_data.run_config,
+            run_config=run_config,
             use_parent_run_tags=False,  # don't inherit tags from the previous run
         )
 
     else:  # backfill_job.reexecution_steps
-        last_run = _fetch_last_run(instance, external_partition_set, partition_data.name)
+        last_run = _fetch_last_run(instance, external_partition_set, partition_key_or_range)
         parent_run_id = last_run.run_id if last_run else None
         root_run_id = (last_run.root_run_id or last_run.run_id) if last_run else None
         if parent_run_id and root_run_id:
             tags = merge_dicts(
                 tags, {PARENT_RUN_ID_TAG: parent_run_id, ROOT_RUN_ID_TAG: root_run_id}
             )
         step_keys_to_execute = backfill_job.reexecution_steps
@@ -305,28 +397,28 @@
 
         if external_partition_set.op_selection:
             resolved_op_selection = frozenset(external_partition_set.op_selection)
             op_selection = external_partition_set.op_selection
 
     external_execution_plan = code_location.get_external_execution_plan(
         external_pipeline,
-        partition_data.run_config,
+        run_config,
         step_keys_to_execute=step_keys_to_execute,
         known_state=known_state,
         instance=instance,
     )
 
     return instance.create_run(
         job_snapshot=external_pipeline.job_snapshot,
         execution_plan_snapshot=external_execution_plan.execution_plan_snapshot,
         parent_job_snapshot=external_pipeline.parent_job_snapshot,
         job_name=external_pipeline.name,
         run_id=make_new_run_id(),
         resolved_op_selection=resolved_op_selection,
-        run_config=partition_data.run_config,
+        run_config=run_config,
         step_keys_to_execute=step_keys_to_execute,
         tags=tags,
         root_run_id=root_run_id,
         parent_run_id=parent_run_id,
         status=DagsterRunStatus.NOT_STARTED,
         external_job_origin=external_pipeline.get_external_origin(),
         job_code_origin=external_pipeline.get_python_origin(),
@@ -336,25 +428,35 @@
         ),
         asset_check_selection=None,
         asset_job_partitions_def=code_location.get_asset_job_partitions_def(external_pipeline),
     )
 
 
 def _fetch_last_run(
-    instance: DagsterInstance, external_partition_set: ExternalPartitionSet, partition_name: str
+    instance: DagsterInstance,
+    external_partition_set: ExternalPartitionSet,
+    partition_key_or_range: Union[str, PartitionKeyRange],
 ) -> Optional[DagsterRun]:
     check.inst_param(instance, "instance", DagsterInstance)
     check.inst_param(external_partition_set, "external_partition_set", ExternalPartitionSet)
-    check.str_param(partition_name, "partition_name")
+    check.str_param(partition_key_or_range, "partition_name")
+
+    tags = (
+        {
+            PARTITION_NAME_TAG: partition_key_or_range,
+        }
+        if isinstance(partition_key_or_range, str)
+        else {
+            ASSET_PARTITION_RANGE_START_TAG: partition_key_or_range.start,
+            ASSET_PARTITION_RANGE_END_TAG: partition_key_or_range.end,
+        }
+    )
 
     runs = instance.get_runs(
         RunsFilter(
             job_name=external_partition_set.job_name,
-            tags={
-                PARTITION_SET_TAG: external_partition_set.name,
-                PARTITION_NAME_TAG: partition_name,
-            },
+            tags={PARTITION_SET_TAG: external_partition_set.name, **tags},
         ),
         limit=1,
     )
 
     return runs[0] if runs else None
```

### Comparing `dagster-1.7.5/dagster/_core/execution/job_execution_result.py` & `dagster-1.7.6/dagster/_core/execution/job_execution_result.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/memoization.py` & `dagster-1.7.6/dagster/_core/execution/memoization.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/active.py` & `dagster-1.7.6/dagster/_core/execution/plan/active.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/compute.py` & `dagster-1.7.6/dagster/_core/execution/plan/compute.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/compute_generator.py` & `dagster-1.7.6/dagster/_core/execution/plan/compute_generator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/execute_plan.py` & `dagster-1.7.6/dagster/_core/execution/plan/execute_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/execute_step.py` & `dagster-1.7.6/dagster/_core/execution/plan/execute_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/external_step.py` & `dagster-1.7.6/dagster/_core/execution/plan/external_step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/handle.py` & `dagster-1.7.6/dagster/_core/execution/plan/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/inputs.py` & `dagster-1.7.6/dagster/_core/execution/plan/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/instance_concurrency_context.py` & `dagster-1.7.6/dagster/_core/execution/plan/instance_concurrency_context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/local_external_step_main.py` & `dagster-1.7.6/dagster/_core/execution/plan/local_external_step_main.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/objects.py` & `dagster-1.7.6/dagster/_core/execution/plan/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/outputs.py` & `dagster-1.7.6/dagster/_core/execution/plan/outputs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/plan.py` & `dagster-1.7.6/dagster/_core/execution/plan/plan.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/state.py` & `dagster-1.7.6/dagster/_core/execution/plan/state.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/step.py` & `dagster-1.7.6/dagster/_core/execution/plan/step.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/plan/utils.py` & `dagster-1.7.6/dagster/_core/execution/plan/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/poll_compute_logs.py` & `dagster-1.7.6/dagster/_core/execution/poll_compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/resolve_versions.py` & `dagster-1.7.6/dagster/_core/execution/resolve_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/resources_init.py` & `dagster-1.7.6/dagster/_core/execution/resources_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/retries.py` & `dagster-1.7.6/dagster/_core/execution/retries.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/run_cancellation_thread.py` & `dagster-1.7.6/dagster/_core/execution/run_cancellation_thread.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/stats.py` & `dagster-1.7.6/dagster/_core/execution/stats.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/submit_asset_runs.py` & `dagster-1.7.6/dagster/_core/execution/submit_asset_runs.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/tags.py` & `dagster-1.7.6/dagster/_core/execution/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/validate_run_config.py` & `dagster-1.7.6/dagster/_core/execution/validate_run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/watch_orphans.py` & `dagster-1.7.6/dagster/_core/execution/watch_orphans.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/execution/with_resources.py` & `dagster-1.7.6/dagster/_core/execution/with_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/executor/base.py` & `dagster-1.7.6/dagster/_core/executor/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/executor/child_process_executor.py` & `dagster-1.7.6/dagster/_core/executor/child_process_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/executor/in_process.py` & `dagster-1.7.6/dagster/_core/executor/in_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/executor/init.py` & `dagster-1.7.6/dagster/_core/executor/init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/executor/multiprocess.py` & `dagster-1.7.6/dagster/_core/executor/multiprocess.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/executor/step_delegating/step_delegating_executor.py` & `dagster-1.7.6/dagster/_core/executor/step_delegating/step_delegating_executor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/executor/step_delegating/step_handler/base.py` & `dagster-1.7.6/dagster/_core/executor/step_delegating/step_handler/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/instance/__init__.py` & `dagster-1.7.6/dagster/_core/instance/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3135,50 +3135,44 @@
         self,
         key: AssetKey,
         is_source: Optional[bool] = None,
         partition_key: Optional[str] = None,
         before_cursor: Optional[int] = None,
         after_cursor: Optional[int] = None,
     ) -> Optional["EventLogRecord"]:
-        from dagster._core.events import DagsterEventType
-        from dagster._core.storage.event_log.base import EventRecordsFilter
+        from dagster._core.storage.event_log.base import AssetRecordsFilter
 
-        # When we cant don't know whether the requested key corresponds to a source or regular
-        # asset, we need to retrieve both the latest observation and materialization for all assets.
-        # If there is a materialization, it's a regular asset and we can ignore the observation.
-
-        observation: Optional[EventLogRecord] = None
-        if is_source or is_source is None:
-            observations = self.get_event_records(
-                EventRecordsFilter(
-                    event_type=DagsterEventType.ASSET_OBSERVATION,
-                    asset_key=key,
-                    asset_partitions=[partition_key] if partition_key else None,
-                    before_cursor=before_cursor,
-                    after_cursor=after_cursor,
-                ),
-                limit=1,
-            )
-            observation = next(iter(observations), None)
+        records_filter = AssetRecordsFilter(
+            asset_key=key,
+            asset_partitions=[partition_key] if partition_key else None,
+            before_storage_id=before_cursor,
+            after_storage_id=after_cursor,
+        )
 
-        materialization: Optional[EventLogRecord] = None
-        if not is_source:
-            materializations = self.get_event_records(
-                EventRecordsFilter(
-                    event_type=DagsterEventType.ASSET_MATERIALIZATION,
-                    asset_key=key,
-                    asset_partitions=[partition_key] if partition_key else None,
-                    before_cursor=before_cursor,
-                    after_cursor=after_cursor,
-                ),
-                limit=1,
-            )
-            materialization = next(iter(materializations), None)
+        if is_source is True:
+            # this is a source asset, fetch latest observation record
+            return next(iter(self.fetch_observations(records_filter, limit=1).records), None)
+
+        elif is_source is False:
+            # this is not a source asset, fetch latest materialization record
+            return next(iter(self.fetch_materializations(records_filter, limit=1).records), None)
 
-        return materialization or observation
+        else:
+            assert is_source is None
+            # if is_source is None, the requested key could correspond to either a source asset or
+            # materializable asset. If there is a non-null materialization, we are dealing with a
+            # materializable asset and should just return that.  If not, we should check for any
+            # observation records that may match.
+
+            materialization = next(
+                iter(self.fetch_materializations(records_filter, limit=1).records), None
+            )
+            if materialization:
+                return materialization
+            return next(iter(self.fetch_observations(records_filter, limit=1).records), None)
 
     @public
     def get_latest_materialization_code_versions(
         self, asset_keys: Iterable[AssetKey]
     ) -> Mapping[AssetKey, Optional[str]]:
         """Returns the code version used for the latest materialization of each of the provided
         assets.
```

### Comparing `dagster-1.7.5/dagster/_core/instance/config.py` & `dagster-1.7.6/dagster/_core/instance/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/instance/ref.py` & `dagster-1.7.6/dagster/_core/instance/ref.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/instance_for_test.py` & `dagster-1.7.6/dagster/_core/instance_for_test.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/launcher/base.py` & `dagster-1.7.6/dagster/_core/launcher/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/launcher/default_run_launcher.py` & `dagster-1.7.6/dagster/_core/launcher/default_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/launcher/sync_in_memory_run_launcher.py` & `dagster-1.7.6/dagster/_core/launcher/sync_in_memory_run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/log_manager.py` & `dagster-1.7.6/dagster/_core/log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/nux.py` & `dagster-1.7.6/dagster/_core/nux.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/op_concurrency_limits_counter.py` & `dagster-1.7.6/dagster/_core/op_concurrency_limits_counter.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/origin.py` & `dagster-1.7.6/dagster/_core/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/pipes/client.py` & `dagster-1.7.6/dagster/_core/pipes/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/pipes/context.py` & `dagster-1.7.6/dagster/_core/pipes/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/pipes/subprocess.py` & `dagster-1.7.6/dagster/_core/pipes/subprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from subprocess import Popen
 from typing import Mapping, Optional, Sequence, Union
 
 from dagster_pipes import PipesExtras
 
 from dagster import _check as check
 from dagster._annotations import experimental, public
-from dagster._core.definitions.resource_annotation import ResourceParam
+from dagster._core.definitions.resource_annotation import TreatAsResourceParam
 from dagster._core.errors import DagsterExecutionInterruptedError, DagsterPipesExecutionError
 from dagster._core.execution.context.compute import OpExecutionContext
 from dagster._core.pipes.client import (
     PipesClient,
     PipesClientCompletedInvocation,
     PipesContextInjector,
     PipesMessageReader,
@@ -20,15 +20,15 @@
     PipesTempFileContextInjector,
     PipesTempFileMessageReader,
     open_pipes_session,
 )
 
 
 @experimental
-class _PipesSubprocess(PipesClient):
+class PipesSubprocessClient(PipesClient, TreatAsResourceParam):
     """A pipes client that runs a subprocess with the given command and environment.
 
     By default parameters are injected via environment variables. Context is passed via
     a temp file, and structured messages are read from from a temp file.
 
     Args:
         env (Optional[Mapping[str, str]]): An optional dict of environment variables to pass to the
@@ -130,10 +130,7 @@
                     context.log.info("[pipes] execution interrupted, sending SIGINT to subprocess.")
                     # send sigint to give external process chance to exit gracefully
                     process.send_signal(signal.SIGINT)
                     process.wait(timeout=self.termination_timeout_seconds)
                 raise
 
         return PipesClientCompletedInvocation(pipes_session)
-
-
-PipesSubprocessClient = ResourceParam[_PipesSubprocess]
```

### Comparing `dagster-1.7.5/dagster/_core/pipes/utils.py` & `dagster-1.7.6/dagster/_core/pipes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/remote_representation/__init__.py` & `dagster-1.7.6/dagster/_core/remote_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/remote_representation/code_location.py` & `dagster-1.7.6/dagster/_core/remote_representation/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/remote_representation/external.py` & `dagster-1.7.6/dagster/_core/remote_representation/external.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,18 +15,20 @@
     Union,
 )
 
 import dagster._check as check
 from dagster import AssetSelection
 from dagster._config.snap import ConfigFieldSnap, ConfigSchemaSnapshot
 from dagster._core.definitions.asset_check_spec import AssetCheckKey
+from dagster._core.definitions.backfill_policy import BackfillPolicy
 from dagster._core.definitions.events import AssetKey
 from dagster._core.definitions.metadata import (
     MetadataValue,
 )
+from dagster._core.definitions.partition import PartitionsDefinition
 from dagster._core.definitions.run_request import InstigatorType
 from dagster._core.definitions.schedule_definition import DefaultScheduleStatus
 from dagster._core.definitions.selector import (
     InstigatorSelector,
     RepositorySelector,
     ScheduleSelector,
     SensorSelector,
@@ -516,15 +518,15 @@
         return self._active_preset_dict[preset_name]
 
     @property
     def root_config_key(self) -> Optional[str]:
         return self.get_mode_def_snap(DEFAULT_MODE_NAME).root_config_key
 
     @property
-    def tags(self) -> Mapping[str, object]:
+    def tags(self) -> Mapping[str, str]:
         return self._job_index.job_snapshot.tags
 
     @property
     def metadata(self) -> Mapping[str, MetadataValue]:
         return self._job_index.job_snapshot.metadata
 
     @property
@@ -1007,14 +1009,18 @@
         return self._external_partition_set_data.mode
 
     @property
     def job_name(self) -> str:
         return self._external_partition_set_data.job_name
 
     @property
+    def backfill_policy(self) -> Optional[BackfillPolicy]:
+        return self._external_partition_set_data.backfill_policy
+
+    @property
     def repository_handle(self) -> RepositoryHandle:
         return self._handle.repository_handle
 
     def get_external_origin(self) -> RemotePartitionSetOrigin:
         return self._handle.get_external_origin()
 
     def get_external_origin_id(self) -> str:
@@ -1022,13 +1028,17 @@
 
     def has_partition_name_data(self) -> bool:
         # Partition sets from older versions of Dagster as well as partition sets using
         # a DynamicPartitionsDefinition require calling out to user code to compute the partition
         # names
         return self._external_partition_set_data.external_partitions_data is not None
 
+    def get_partitions_definition(self) -> PartitionsDefinition:
+        return (
+            self._external_partition_set_data.external_partitions_data.get_partitions_definition()  # type: ignore
+        )
+
     def get_partition_names(self, instance: DagsterInstance) -> Sequence[str]:
         check.invariant(self.has_partition_name_data())
-        partitions = (
-            self._external_partition_set_data.external_partitions_data.get_partitions_definition()  # type: ignore
+        return self.get_partitions_definition().get_partition_keys(
+            dynamic_partitions_store=instance
         )
-        return partitions.get_partition_keys(dynamic_partitions_store=instance)
```

### Comparing `dagster-1.7.5/dagster/_core/remote_representation/external_data.py` & `dagster-1.7.6/dagster/_core/remote_representation/external_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -899,36 +899,41 @@
         "_PartitionSetSnap",
         [
             ("name", str),
             ("job_name", str),
             ("op_selection", Optional[Sequence[str]]),
             ("mode", Optional[str]),
             ("external_partitions_data", Optional[ExternalPartitionsDefinitionData]),
+            ("backfill_policy", Optional[BackfillPolicy]),
         ],
     )
 ):
     def __new__(
         cls,
         name: str,
         job_name: str,
         op_selection: Optional[Sequence[str]],
         mode: Optional[str],
         external_partitions_data: Optional[ExternalPartitionsDefinitionData] = None,
+        backfill_policy: Optional[BackfillPolicy] = None,
     ):
         return super(PartitionSetSnap, cls).__new__(
             cls,
             name=check.str_param(name, "name"),
             job_name=check.str_param(job_name, "job_name"),
             op_selection=check.opt_nullable_sequence_param(op_selection, "op_selection", str),
             mode=check.opt_str_param(mode, "mode"),
             external_partitions_data=check.opt_inst_param(
                 external_partitions_data,
                 "external_partitions_data",
                 ExternalPartitionsDefinitionData,
             ),
+            backfill_policy=check.opt_inst_param(
+                backfill_policy, "backfill_policy", BackfillPolicy
+            ),
         )
 
     @classmethod
     def from_job_def(cls, job_def: JobDefinition) -> Self:
         check.inst_param(job_def, "job_def", JobDefinition)
         partitions_def = check.not_none(job_def.partitions_def)
 
@@ -951,14 +956,15 @@
 
         return cls(
             name=external_partition_set_name_for_job_name(job_def.name),
             job_name=job_def.name,
             op_selection=None,
             mode=DEFAULT_MODE_NAME,
             external_partitions_data=partitions_def_data,
+            backfill_policy=job_def.backfill_policy,
         )
 
 
 @whitelist_for_serdes
 class ExternalPartitionNamesData(
     NamedTuple("_ExternalPartitionNamesData", [("partition_names", Sequence[str])])
 ):
@@ -995,15 +1001,15 @@
         )
 
 
 @whitelist_for_serdes
 class ExternalPartitionExecutionParamData(
     NamedTuple(
         "_ExternalPartitionExecutionParamData",
-        [("name", str), ("tags", Mapping[str, object]), ("run_config", Mapping[str, object])],
+        [("name", str), ("tags", Mapping[str, str]), ("run_config", Mapping[str, object])],
     )
 ):
     def __new__(cls, name: str, tags: Mapping[str, str], run_config: Mapping[str, object]):
         return super(ExternalPartitionExecutionParamData, cls).__new__(
             cls,
             name=check.str_param(name, "name"),
             tags=check.mapping_param(tags, "tags"),
```

### Comparing `dagster-1.7.5/dagster/_core/remote_representation/feature_flags.py` & `dagster-1.7.6/dagster/_core/remote_representation/feature_flags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/remote_representation/grpc_server_registry.py` & `dagster-1.7.6/dagster/_core/remote_representation/grpc_server_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/remote_representation/grpc_server_state_subscriber.py` & `dagster-1.7.6/dagster/_core/remote_representation/grpc_server_state_subscriber.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/remote_representation/handle.py` & `dagster-1.7.6/dagster/_core/remote_representation/handle.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/remote_representation/historical.py` & `dagster-1.7.6/dagster/_core/remote_representation/historical.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/remote_representation/job_index.py` & `dagster-1.7.6/dagster/_core/remote_representation/job_index.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/remote_representation/origin.py` & `dagster-1.7.6/dagster/_core/remote_representation/origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/remote_representation/represented.py` & `dagster-1.7.6/dagster/_core/remote_representation/represented.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/run_coordinator/base.py` & `dagster-1.7.6/dagster/_core/run_coordinator/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/run_coordinator/default_run_coordinator.py` & `dagster-1.7.6/dagster/_core/run_coordinator/default_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/run_coordinator/queued_run_coordinator.py` & `dagster-1.7.6/dagster/_core/run_coordinator/queued_run_coordinator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/scheduler/__init__.py` & `dagster-1.7.6/dagster/_core/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/scheduler/execution.py` & `dagster-1.7.6/dagster/_core/scheduler/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/scheduler/instigation.py` & `dagster-1.7.6/dagster/_core/scheduler/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/scheduler/scheduler.py` & `dagster-1.7.6/dagster/_core/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/secrets/env_file.py` & `dagster-1.7.6/dagster/_core/secrets/env_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/selector/subset_selector.py` & `dagster-1.7.6/dagster/_core/selector/subset_selector.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/snap/__init__.py` & `dagster-1.7.6/dagster/_core/snap/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/snap/dagster_types.py` & `dagster-1.7.6/dagster/_core/snap/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/snap/dep_snapshot.py` & `dagster-1.7.6/dagster/_core/snap/dep_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/snap/execution_plan_snapshot.py` & `dagster-1.7.6/dagster/_core/snap/execution_plan_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/snap/job_snapshot.py` & `dagster-1.7.6/dagster/_core/snap/job_snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/snap/mode.py` & `dagster-1.7.6/dagster/_core/snap/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/snap/node.py` & `dagster-1.7.6/dagster/_core/snap/node.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/snap/snap_to_yaml.py` & `dagster-1.7.6/dagster/_core/snap/snap_to_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/DEVELOPING.md` & `dagster-1.7.6/dagster/_core/storage/DEVELOPING.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/README.md` & `dagster-1.7.6/dagster/_core/storage/alembic/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/env.py` & `dagster-1.7.6/dagster/_core/storage/alembic/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/001_initial_1.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/001_initial_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/002_cascade_run_deletion_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/003_add_step_key_pipeline_name_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/004_add_snapshots_to_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/005_add_asset_key_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/005_add_asset_key_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/006_scheduler_update_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/007_create_run_id_idx_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/008_add_run_tags_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/009_add_partition_column_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/009_add_partition_column_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/010_add_run_partition_columns_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_1.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/011_wipe_schedules_table_for_0_10_0_sqlite_2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/015_change_varchar_to_text_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/017_add_run_status_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/019_0_11_0_db_text_to_db_string_unique_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/021_add_column_mode_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/021_add_column_mode_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/021_add_column_mode_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_postgres.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/024_add_columns_start_time_and_end_time_sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/026_convert_start_end_times_format_mysql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/030_add_columns_action_type_and_selector_id_.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/031_add_kvs_table.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/031_add_kvs_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/033_add_asset_event_tags_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/036_add_dynamic_partitions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/037_d9092588866f_add_primary_key_cols.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/038_701913684cb4_add_postgres_pks.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/039_d3a4c9e87af3_add_asset_daemon_asset_evaluations_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/040_add_in_progress_step_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/041_add_asset_check_executions_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py` & `dagster-1.7.6/dagster/_core/storage/alembic/versions/042_46b412388816_add_concurrency_limits_table.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/asset_check_execution_record.py` & `dagster-1.7.6/dagster/_core/storage/asset_check_execution_record.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/asset_value_loader.py` & `dagster-1.7.6/dagster/_core/storage/asset_value_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/base_storage.py` & `dagster-1.7.6/dagster/_core/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/batch_asset_record_loader.py` & `dagster-1.7.6/dagster/_core/storage/batch_asset_record_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/branching/branching_io_manager.py` & `dagster-1.7.6/dagster/_core/storage/branching/branching_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/captured_log_manager.py` & `dagster-1.7.6/dagster/_core/storage/captured_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/cloud_storage_compute_log_manager.py` & `dagster-1.7.6/dagster/_core/storage/cloud_storage_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/compute_log_manager.py` & `dagster-1.7.6/dagster/_core/storage/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/config.py` & `dagster-1.7.6/dagster/_core/storage/config.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/dagster_run.py` & `dagster-1.7.6/dagster/_core/storage/dagster_run.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/db_io_manager.py` & `dagster-1.7.6/dagster/_core/storage/db_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/event_log/__init__.py` & `dagster-1.7.6/dagster/_core/storage/event_log/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/event_log/base.py` & `dagster-1.7.6/dagster/_core/storage/event_log/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Tuple,
     Union,
 )
 
 import dagster._check as check
 from dagster._core.assets import AssetDetails
 from dagster._core.definitions.asset_check_spec import AssetCheckKey
+from dagster._core.definitions.data_version import DATA_VERSION_TAG
 from dagster._core.definitions.events import AssetKey
 from dagster._core.event_api import (
     AssetRecordsFilter,
     EventHandlerFn,
     EventLogCursor,
     EventLogRecord,
     EventRecordsFilter,
@@ -30,14 +31,15 @@
     build_run_stats_from_events,
     build_run_step_stats_from_events,
 )
 from dagster._core.instance import MayHaveInstanceWeakref, T_DagsterInstance
 from dagster._core.storage.asset_check_execution_record import AssetCheckExecutionRecord
 from dagster._core.storage.dagster_run import DagsterRunStatsSnapshot
 from dagster._core.storage.sql import AlembicVersion
+from dagster._core.storage.tags import MULTIDIMENSIONAL_PARTITION_PREFIX
 from dagster._utils import PrintFn
 from dagster._utils.concurrency import ConcurrencyClaimStatus, ConcurrencyKeyInfo
 from dagster._utils.warnings import deprecation_warning
 
 if TYPE_CHECKING:
     from dagster._core.events.log import EventLogEntry
     from dagster._core.storage.partition_status_cache import AssetStatusCacheValue
@@ -374,14 +376,22 @@
         self,
         asset_key: AssetKey,
         filter_tags: Optional[Mapping[str, str]] = None,
         filter_event_id: Optional[int] = None,
     ) -> Sequence[Mapping[str, str]]:
         pass
 
+    def get_asset_tags_to_index(self, tag_keys: Set[str]) -> Set[str]:
+        # make sure we update the list of tested tags in test_asset_tags_to_insert to match
+        return {
+            key
+            for key in tag_keys
+            if key == DATA_VERSION_TAG or key.startswith(MULTIDIMENSIONAL_PARTITION_PREFIX)
+        }
+
     @abstractmethod
     def wipe_asset(self, asset_key: AssetKey) -> None:
         """Remove asset index history from event log for given asset_key."""
 
     @abstractmethod
     def get_materialized_partitions(
         self,
```

### Comparing `dagster-1.7.5/dagster/_core/storage/event_log/in_memory.py` & `dagster-1.7.6/dagster/_core/storage/event_log/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/event_log/migration.py` & `dagster-1.7.6/dagster/_core/storage/event_log/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/event_log/polling_event_watcher.py` & `dagster-1.7.6/dagster/_core/storage/event_log/polling_event_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/event_log/schema.py` & `dagster-1.7.6/dagster/_core/storage/event_log/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/event_log/sql_event_log.py` & `dagster-1.7.6/dagster/_core/storage/event_log/sql_event_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -422,22 +422,24 @@
         # migration to create the table. On read, we will throw an error if the table does not
         # exist.
         if len(all_values) > 0 and self.has_table(AssetEventTagsTable.name):
             with self.index_connection() as conn:
                 conn.execute(AssetEventTagsTable.insert(), all_values)
 
     def _tags_for_asset_event(self, event: EventLogEntry) -> Mapping[str, str]:
+        tags = {}
         if event.dagster_event and event.dagster_event.asset_key:
             if event.dagster_event.is_step_materialization:
-                return (
+                tags = (
                     event.get_dagster_event().step_materialization_data.materialization.tags or {}
                 )
             elif event.dagster_event.is_asset_observation:
-                return event.get_dagster_event().asset_observation_data.asset_observation.tags
-        return {}
+                tags = event.get_dagster_event().asset_observation_data.asset_observation.tags
+        keys_to_index = self.get_asset_tags_to_index(set(tags.keys()))
+        return {k: v for k, v in tags.items() if k in keys_to_index}
 
     def store_event(self, event: EventLogEntry) -> None:
         """Store an event corresponding to a pipeline run.
 
         Args:
             event (EventLogEntry): The event to store.
         """
@@ -1878,14 +1880,19 @@
         check.inst_param(asset_key, "asset_key", AssetKey)
         check.inst_param(event_type, "event_type", DagsterEventType)
         check.sequence_param(tag_keys, "tag_keys", of_type=str)
         check.opt_nullable_sequence_param(asset_partitions, "asset_partitions", of_type=str)
         check.opt_int_param(before_cursor, "before_cursor")
         check.opt_int_param(after_cursor, "after_cursor")
 
+        if not tag_keys or len(tag_keys) != len(self.get_asset_tags_to_index(set(tag_keys))):
+            check.failed(
+                "Only a limited set of tag keys are whitelisted for querying the latest tag values by partition."
+            )
+
         latest_event_ids_subquery = self._latest_event_ids_by_partition_subquery(
             asset_key=asset_key,
             event_types=[event_type],
             asset_partitions=asset_partitions,
             before_cursor=before_cursor,
             after_cursor=after_cursor,
         )
```

### Comparing `dagster-1.7.5/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini` & `dagster-1.7.6/dagster/_core/storage/event_log/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py` & `dagster-1.7.6/dagster/_core/storage/event_log/sqlite/consolidated_sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py` & `dagster-1.7.6/dagster/_core/storage/event_log/sqlite/sqlite_event_log.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/file_manager.py` & `dagster-1.7.6/dagster/_core/storage/file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/fs_io_manager.py` & `dagster-1.7.6/dagster/_core/storage/fs_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/input_manager.py` & `dagster-1.7.6/dagster/_core/storage/input_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/io_manager.py` & `dagster-1.7.6/dagster/_core/storage/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/legacy_storage.py` & `dagster-1.7.6/dagster/_core/storage/legacy_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/local_compute_log_manager.py` & `dagster-1.7.6/dagster/_core/storage/local_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/mem_io_manager.py` & `dagster-1.7.6/dagster/_core/storage/mem_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/memoizable_io_manager.py` & `dagster-1.7.6/dagster/_core/storage/memoizable_io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/migration/bigint_migration.py` & `dagster-1.7.6/dagster/_core/storage/migration/bigint_migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/migration/utils.py` & `dagster-1.7.6/dagster/_core/storage/migration/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/noop_compute_log_manager.py` & `dagster-1.7.6/dagster/_core/storage/noop_compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/output_manager.py` & `dagster-1.7.6/dagster/_core/storage/output_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/partition_status_cache.py` & `dagster-1.7.6/dagster/_core/storage/partition_status_cache.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/root.py` & `dagster-1.7.6/dagster/_core/storage/root.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/runs/base.py` & `dagster-1.7.6/dagster/_core/storage/runs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Mapping, Optional, Sequence, Set, Tuple, Union
+from typing import TYPE_CHECKING, Dict, Mapping, Optional, Sequence, Set, Tuple, Union
 
 from typing_extensions import TypedDict
 
 from dagster._core.events import DagsterEvent
 from dagster._core.execution.backfill import BulkActionStatus, PartitionBackfill
+from dagster._core.execution.types import RunTelemetryData
 from dagster._core.instance import MayHaveInstanceWeakref, T_DagsterInstance
 from dagster._core.snap import ExecutionPlanSnapshot, JobSnapshot
 from dagster._core.storage.dagster_run import (
     DagsterRun,
     JobBucket,
     RunPartitionData,
     RunRecord,
@@ -349,14 +350,22 @@
     def add_daemon_heartbeat(self, daemon_heartbeat: DaemonHeartbeat) -> None:
         """Called on a regular interval by the daemon."""
 
     @abstractmethod
     def get_daemon_heartbeats(self) -> Mapping[str, DaemonHeartbeat]:
         """Latest heartbeats of all daemon types."""
 
+    def add_run_telemetry(
+        self,
+        run_telemetry: RunTelemetryData,
+        tags: Optional[Dict[str, str]] = None,
+    ) -> None:
+        """Not implemented in base class. Should be implemented in subclasses that support telemetry."""
+        pass
+
     @abstractmethod
     def wipe_daemon_heartbeats(self) -> None:
         """Wipe all daemon heartbeats."""
 
     # Backfill storage
     @abstractmethod
     def get_backfills(
```

### Comparing `dagster-1.7.5/dagster/_core/storage/runs/in_memory.py` & `dagster-1.7.6/dagster/_core/storage/runs/in_memory.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/runs/migration.py` & `dagster-1.7.6/dagster/_core/storage/runs/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/runs/schema.py` & `dagster-1.7.6/dagster/_core/storage/runs/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/runs/sql_run_storage.py` & `dagster-1.7.6/dagster/_core/storage/runs/sql_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/runs/sqlite/alembic/alembic.ini` & `dagster-1.7.6/dagster/_core/storage/runs/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py` & `dagster-1.7.6/dagster/_core/storage/runs/sqlite/sqlite_run_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/schedules/base.py` & `dagster-1.7.6/dagster/_core/storage/schedules/base.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/schedules/migration.py` & `dagster-1.7.6/dagster/_core/storage/schedules/migration.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/schedules/schema.py` & `dagster-1.7.6/dagster/_core/storage/schedules/schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/schedules/sql_schedule_storage.py` & `dagster-1.7.6/dagster/_core/storage/schedules/sql_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini` & `dagster-1.7.6/dagster/_core/storage/schedules/sqlite/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py` & `dagster-1.7.6/dagster/_core/storage/schedules/sqlite/sqlite_schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/sql.py` & `dagster-1.7.6/dagster/_core/storage/sql.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/sqlalchemy_compat.py` & `dagster-1.7.6/dagster/_core/storage/sqlalchemy_compat.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/sqlite.py` & `dagster-1.7.6/dagster/_core/storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/sqlite_storage.py` & `dagster-1.7.6/dagster/_core/storage/sqlite_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/tags.py` & `dagster-1.7.6/dagster/_core/storage/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/temp_file_manager.py` & `dagster-1.7.6/dagster/_core/storage/temp_file_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/storage/upath_io_manager.py` & `dagster-1.7.6/dagster/_core/storage/upath_io_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,15 +441,21 @@
             self._handle_transition_to_partitioned_asset(context, path.parent)
         else:
             path = self._get_path(context)
         self.make_directory(path.parent)
         context.log.debug(self.get_writing_output_log_message(path))
         self.dump_to_path(context=context, obj=obj, path=path)
 
-        metadata = {"path": MetadataValue.path(str(path))}
+        # Usually, when the value is None, it means that the user didn't intend to use an IO manager
+        # at all, but ended up with one because they didn't set None as their return type
+        # annotation. In these cases, seeing a "path" metadata value can be very confusing, because
+        # often they're actually writing data to a different location within their op. We omit
+        # the metadata when "obj is None", in order to avoid this confusion in the common case.
+        # This comes at the cost of this metadata not being present in these edge cases.
+        metadata = {"path": MetadataValue.path(str(path))} if obj is not None else {}
         custom_metadata = self.get_metadata(context=context, obj=obj)
         metadata.update(custom_metadata)  # type: ignore
 
         context.add_output_metadata(metadata)
 
 
 def is_dict_type(type_obj) -> bool:
```

### Comparing `dagster-1.7.5/dagster/_core/system_config/composite_descent.py` & `dagster-1.7.6/dagster/_core/system_config/composite_descent.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/system_config/objects.py` & `dagster-1.7.6/dagster/_core/system_config/objects.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/telemetry.py` & `dagster-1.7.6/dagster/_core/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/telemetry_upload.py` & `dagster-1.7.6/dagster/_core/telemetry_upload.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/test_utils.py` & `dagster-1.7.6/dagster/_core/test_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/types/builtin_config_schemas.py` & `dagster-1.7.6/dagster/_core/types/builtin_config_schemas.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/types/config_schema.py` & `dagster-1.7.6/dagster/_core/types/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/types/dagster_type.py` & `dagster-1.7.6/dagster/_core/types/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/types/decorator.py` & `dagster-1.7.6/dagster/_core/types/decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/types/loadable_target_origin.py` & `dagster-1.7.6/dagster/_core/types/loadable_target_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/types/primitive_mapping.py` & `dagster-1.7.6/dagster/_core/types/primitive_mapping.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/types/python_dict.py` & `dagster-1.7.6/dagster/_core/types/python_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/types/python_set.py` & `dagster-1.7.6/dagster/_core/types/python_set.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/types/python_tuple.py` & `dagster-1.7.6/dagster/_core/types/python_tuple.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/types/transform_typing.py` & `dagster-1.7.6/dagster/_core/types/transform_typing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/utility_ops.py` & `dagster-1.7.6/dagster/_core/utility_ops.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/utils.py` & `dagster-1.7.6/dagster/_core/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/workspace/autodiscovery.py` & `dagster-1.7.6/dagster/_core/workspace/autodiscovery.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/workspace/config_schema.py` & `dagster-1.7.6/dagster/_core/workspace/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/workspace/context.py` & `dagster-1.7.6/dagster/_core/workspace/context.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/workspace/load.py` & `dagster-1.7.6/dagster/_core/workspace/load.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/workspace/load_target.py` & `dagster-1.7.6/dagster/_core/workspace/load_target.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/workspace/permissions.py` & `dagster-1.7.6/dagster/_core/workspace/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_core/workspace/workspace.py` & `dagster-1.7.6/dagster/_core/workspace/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_daemon/__init__.py` & `dagster-1.7.6/dagster/_daemon/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_daemon/asset_daemon.py` & `dagster-1.7.6/dagster/_daemon/asset_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py` & `dagster-1.7.6/dagster/_daemon/auto_run_reexecution/auto_run_reexecution.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_daemon/auto_run_reexecution/event_log_consumer.py` & `dagster-1.7.6/dagster/_daemon/auto_run_reexecution/event_log_consumer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_daemon/backfill.py` & `dagster-1.7.6/dagster/_daemon/backfill.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,26 +41,37 @@
     instance = workspace_process_context.instance
 
     for backfill_job in backfill_jobs:
         backfill_id = backfill_job.backfill_id
 
         # refetch, in case the backfill was updated in the meantime
         backfill = cast(PartitionBackfill, instance.get_backfill(backfill_id))
+        # create a logger that will always include the backfill_id as an `extra`
+
+        backfill_logger = cast(
+            logging.Logger,
+            logging.LoggerAdapter(logger, extra={"backfill_id": backfill.backfill_id}),
+        )
+
         try:
             if backfill.is_asset_backfill:
                 yield from execute_asset_backfill_iteration(
-                    backfill, logger, workspace_process_context, instance
+                    backfill, backfill_logger, workspace_process_context, instance
                 )
             else:
                 yield from execute_job_backfill_iteration(
-                    backfill, logger, workspace_process_context, debug_crash_flags, instance
+                    backfill,
+                    backfill_logger,
+                    workspace_process_context,
+                    debug_crash_flags,
+                    instance,
                 )
         except Exception:
             error_info = DaemonErrorCapture.on_exception(
                 sys.exc_info(),
-                logger=logger,
+                logger=backfill_logger,
                 log_message=f"Backfill failed for {backfill.backfill_id}",
             )
             instance.update_backfill(
                 backfill.with_status(BulkActionStatus.FAILED).with_error(error_info)
             )
             yield error_info
```

### Comparing `dagster-1.7.5/dagster/_daemon/cli/__init__.py` & `dagster-1.7.6/dagster/_daemon/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_daemon/controller.py` & `dagster-1.7.6/dagster/_daemon/controller.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_daemon/daemon.py` & `dagster-1.7.6/dagster/_daemon/daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_daemon/monitoring/concurrency.py` & `dagster-1.7.6/dagster/_daemon/monitoring/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_daemon/monitoring/run_monitoring.py` & `dagster-1.7.6/dagster/_daemon/monitoring/run_monitoring.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py` & `dagster-1.7.6/dagster/_daemon/run_coordinator/queued_run_coordinator_daemon.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_daemon/sensor.py` & `dagster-1.7.6/dagster/_daemon/sensor.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_daemon/types.py` & `dagster-1.7.6/dagster/_daemon/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_daemon/utils.py` & `dagster-1.7.6/dagster/_daemon/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_daemon/workspace.py` & `dagster-1.7.6/dagster/_daemon/workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_generate/download.py` & `dagster-1.7.6/dagster/_generate/download.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_generate/generate.py` & `dagster-1.7.6/dagster/_generate/generate.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md` & `dagster-1.7.6/dagster/_generate/templates/PROJECT_NAME_PLACEHOLDER/README.md`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_grpc/__generated__/api_pb2.py` & `dagster-1.7.6/dagster/_grpc/__generated__/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_grpc/__generated__/api_pb2.pyi` & `dagster-1.7.6/dagster/_grpc/__generated__/api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_grpc/__generated__/api_pb2_grpc.py` & `dagster-1.7.6/dagster/_grpc/__generated__/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_grpc/__init__.py` & `dagster-1.7.6/dagster/_grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_grpc/client.py` & `dagster-1.7.6/dagster/_grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_grpc/compile.py` & `dagster-1.7.6/dagster/_grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_grpc/impl.py` & `dagster-1.7.6/dagster/_grpc/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_grpc/protos/api.proto` & `dagster-1.7.6/dagster/_grpc/protos/api.proto`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_grpc/proxy_server.py` & `dagster-1.7.6/dagster/_grpc/proxy_server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_grpc/server.py` & `dagster-1.7.6/dagster/_grpc/server.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_grpc/server_watcher.py` & `dagster-1.7.6/dagster/_grpc/server_watcher.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_grpc/types.py` & `dagster-1.7.6/dagster/_grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_grpc/utils.py` & `dagster-1.7.6/dagster/_grpc/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_loggers/__init__.py` & `dagster-1.7.6/dagster/_loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_model/__init__.py` & `dagster-1.7.6/dagster/_model/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 from functools import cached_property
-from typing import Any, Dict, Hashable, Optional
+from typing import TYPE_CHECKING, Any, Dict, Hashable, Optional
 
 from pydantic import BaseModel, ConfigDict, PrivateAttr
-from typing_extensions import Self
+from typing_extensions import Annotated, Self, TypeAlias, TypeVar
 
 from .pydantic_compat_layer import USING_PYDANTIC_2
 
+if USING_PYDANTIC_2:
+    from pydantic import InstanceOf as InstanceOf  # type: ignore
+else:
+    # fallback to a no-op on pydantic 1 as there is no equivalent
+    AnyType = TypeVar("AnyType")
+    InstanceOf: TypeAlias = Annotated[AnyType, ...]
+
 
 class DagsterModel(BaseModel):
     """Standardizes on Pydantic settings that are stricter than the default.
     - Frozen, to avoid complexity caused by mutation.
     - extra=forbid, to avoid bugs caused by accidentally constructing with the wrong arguments.
     - arbitrary_types_allowed, to allow non-model class params to be validated with isinstance.
     - Avoid pydantic reading a cached property class as part of the schema.
     """
 
-    _cached_method_cache__internal__: Dict[Hashable, Any] = PrivateAttr(default_factory=dict)
-
-    def __init__(self, **data: Any) -> None:
-        super().__init__(**data)
+    if not USING_PYDANTIC_2:
+        # the setattr approach for cached_method works in pydantic 2 so only declare the PrivateAttr
+        # in pydantic 1 as it has non trivial performance impact
+        _cached_method_cache__internal__: Dict[Hashable, Any] = PrivateAttr(default_factory=dict)
+
+    if TYPE_CHECKING:
+        # without this, the type checker does not understand the constructor kwargs on subclasses
+        def __init__(self, **data: Any) -> None: ...
 
     if USING_PYDANTIC_2:
         model_config = ConfigDict(  # type: ignore
             extra="forbid",
             frozen=True,
             arbitrary_types_allowed=True,
             ignored_types=(cached_property,),
@@ -36,7 +47,14 @@
             keep_untouched = (cached_property,)
 
     def model_copy(self, *, update: Optional[Dict[str, Any]] = None) -> Self:
         if USING_PYDANTIC_2:
             return super().model_copy(update=update)  # type: ignore
         else:
             return super().copy(update=update)
+
+    @classmethod
+    def model_construct(cls, **kwargs: Any) -> Self:
+        if USING_PYDANTIC_2:
+            return super().model_construct(**kwargs)  # type: ignore
+        else:
+            return super().construct(**kwargs)
```

### Comparing `dagster-1.7.5/dagster/_model/pydantic_compat_layer.py` & `dagster-1.7.6/dagster/_model/pydantic_compat_layer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_module_alias_map.py` & `dagster-1.7.6/dagster/_module_alias_map.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_scheduler/scheduler.py` & `dagster-1.7.6/dagster/_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_scheduler/stale.py` & `dagster-1.7.6/dagster/_scheduler/stale.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_serdes/__init__.py` & `dagster-1.7.6/dagster/_serdes/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_serdes/config_class.py` & `dagster-1.7.6/dagster/_serdes/config_class.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_serdes/ipc.py` & `dagster-1.7.6/dagster/_serdes/ipc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_serdes/serdes.py` & `dagster-1.7.6/dagster/_serdes/serdes.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_serdes/utils.py` & `dagster-1.7.6/dagster/_serdes/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_seven/__init__.py` & `dagster-1.7.6/dagster/_seven/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_seven/abc.py` & `dagster-1.7.6/dagster/_seven/abc.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_seven/compat/pendulum.py` & `dagster-1.7.6/dagster/_seven/compat/pendulum.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,20 @@
     else:
         with pendulum.tz.test_local_timezone(pendulum.tz.timezone(override_timezone)):
             yield
 
 
 def create_pendulum_time(year, month, day, *args, **kwargs):
     if "tz" in kwargs and "dst_rule" in kwargs and _IS_PENDULUM_1:
-        tz = pendulum.timezone(kwargs.pop("tz"))
+        tz_name_or_info = kwargs.pop("tz")
+        tz = (
+            pendulum.timezone(tz_name_or_info)
+            if isinstance(tz_name_or_info, str)
+            else tz_name_or_info
+        )
         dst_rule = kwargs.pop("dst_rule")
 
         return pendulum.instance(
             tz.convert(
                 datetime.datetime(
                     year,
                     month,
```

### Comparing `dagster-1.7.5/dagster/_utils/__init__.py` & `dagster-1.7.6/dagster/_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     Union,
     cast,
     overload,
 )
 
 import packaging.version
 from filelock import FileLock
+from pydantic import BaseModel
 from typing_extensions import Literal, TypeAlias, TypeGuard
 
 import dagster._check as check
 import dagster._seven as seven
 
 from .internal_init import IHasInternalInit as IHasInternalInit
 
@@ -283,14 +284,16 @@
 
 
 def make_hashable(value: Any) -> Any:
     if isinstance(value, dict):
         return tuple(sorted((key, make_hashable(value)) for key, value in value.items()))
     elif isinstance(value, (list, tuple, set)):
         return tuple([make_hashable(x) for x in value])
+    elif isinstance(value, BaseModel):
+        return make_hashable(value.dict())
     else:
         return value
 
 
 def get_prop_or_key(elem, key):
     if isinstance(elem, Mapping):
         return elem.get(key)
```

### Comparing `dagster-1.7.5/dagster/_utils/alert.py` & `dagster-1.7.6/dagster/_utils/alert.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/backoff.py` & `dagster-1.7.6/dagster/_utils/backoff.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/cached_method.py` & `dagster-1.7.6/dagster/_utils/cached_method.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/caching_instance_queryer.py` & `dagster-1.7.6/dagster/_utils/caching_instance_queryer.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 from dagster._core.event_api import AssetRecordsFilter, EventRecordsFilter
 from dagster._core.events import DagsterEventType
 from dagster._core.instance import DagsterInstance, DynamicPartitionsStore
 from dagster._core.storage.batch_asset_record_loader import BatchAssetRecordLoader
 from dagster._core.storage.dagster_run import (
     IN_PROGRESS_RUN_STATUSES,
     DagsterRun,
+    DagsterRunStatus,
     RunRecord,
 )
 from dagster._core.storage.tags import PARTITION_NAME_TAG
 from dagster._utils.cached_method import cached_method
 
 if TYPE_CHECKING:
     from dagster._core.storage.event_log import EventLogRecord
@@ -189,14 +190,40 @@
                 value = False
             else:
                 dagster_run = self.instance.get_run_by_id(planned_materialization_info.run_id)
                 value = dagster_run is not None and dagster_run.status in IN_PROGRESS_RUN_STATUSES
 
         return ValidAssetSubset(asset_key=asset_key, value=value)
 
+    @cached_method
+    def get_failed_asset_subset(self, *, asset_key: AssetKey) -> ValidAssetSubset:
+        """Returns an AssetSubset representing the subset of the asset that failed to be
+        materialized its most recent run.
+        """
+        partitions_def = self.asset_graph.get(asset_key).partitions_def
+        if partitions_def:
+            cache_value = self._get_updated_cache_value(asset_key=asset_key)
+            if cache_value is None:
+                value = partitions_def.empty_subset()
+            else:
+                value = cache_value.deserialize_failed_partition_subsets(partitions_def)
+        else:
+            # ideally, unpartitioned assets would also be handled by the asset status cache
+            planned_materialization_info = (
+                self.instance.event_log_storage.get_latest_planned_materialization_info(asset_key)
+            )
+            if not planned_materialization_info:
+                value = False
+            else:
+                dagster_run = self.instance.get_run_by_id(planned_materialization_info.run_id)
+
+                value = dagster_run is not None and dagster_run.status == DagsterRunStatus.FAILURE
+
+        return ValidAssetSubset(asset_key=asset_key, value=value)
+
     ####################
     # ASSET RECORDS / STORAGE IDS
     ####################
 
     def has_cached_asset_record(self, asset_key: AssetKey) -> bool:
         return self._batch_asset_record_loader.has_cached_asset_record(asset_key)
 
@@ -907,14 +934,15 @@
         else:
             return self.get_asset_subset_updated_after_cursor(
                 asset_key=asset_key, after_cursor=first_event_after_time.storage_id - 1
             )
 
     def get_parent_asset_partitions_updated_after_child(
         self,
+        *,
         asset_partition: AssetKeyPartitionKey,
         parent_asset_partitions: AbstractSet[AssetKeyPartitionKey],
         respect_materialization_data_versions: bool,
         ignored_parent_keys: AbstractSet[AssetKey],
     ) -> AbstractSet[AssetKeyPartitionKey]:
         """Returns values inside parent_asset_partitions that correspond to asset partitions that
         have been updated since the latest materialization of asset_partition.
```

### Comparing `dagster-1.7.5/dagster/_utils/concurrency.py` & `dagster-1.7.6/dagster/_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/container.py` & `dagster-1.7.6/dagster/_utils/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,16 +107,16 @@
     previous_cpu_usage: Optional[float]
     previous_measurement_timestamp: Optional[float]
     cgroup_version: Optional[str]
 
 
 def retrieve_containerized_utilization_metrics(
     logger: Optional[logging.Logger],
-    previous_measurement_timestamp: Optional[float],
-    previous_cpu_usage: Optional[float],
+    previous_measurement_timestamp: Optional[float] = None,
+    previous_cpu_usage: Optional[float] = None,
 ) -> ContainerUtilizationMetrics:
     """Retrieve the CPU and memory utilization metrics from cgroup and proc files."""
     cgroup_version = _retrieve_cgroup_version(logger)
     return {
         "num_allocated_cores": _retrieve_containerized_num_allocated_cores(logger),
         "cpu_usage": _retrieve_containerized_cpu_usage(logger, cgroup_version),
         "previous_cpu_usage": previous_cpu_usage,
@@ -249,15 +249,17 @@
 
 def _retrieve_containerized_memory_limit_v2(logger: Optional[logging.Logger]) -> Optional[int]:
     try:
         with open(memory_limit_path_cgroup_v2()) as f:
             return int(f.read())
     except:
         if logger:
-            logger.exception("Failed to retrieve memory limit from cgroup")
+            logger.exception(
+                "Failed to retrieve memory limit from cgroup. There may be no limit set on the container."
+            )
         return None
 
 
 def _retrieve_containerized_cpu_cfs_period_us(
     logger: Optional[logging.Logger], cgroup_version: Optional[CGroupVersion]
 ) -> Optional[float]:
     """Retrieve the CPU period in microseconds from the cgroup file."""
@@ -325,9 +327,11 @@
     # We can retrieve quota information from the cpu.max file. The file is in the format $MAX $PERIOD .
     try:
         with open(cpu_max_path_cgroup_v2()) as f:
             line = f.readline()
             return float(line.split()[0])
     except:
         if logger:
-            logger.exception("Failed to retrieve CPU quota from cgroup")
+            logger.exception(
+                "Failed to retrieve CPU quota from cgroup. There might be not limit set on the container."
+            )
         return None
```

### Comparing `dagster-1.7.5/dagster/_utils/dagster_type.py` & `dagster-1.7.6/dagster/_utils/dagster_type.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/env.py` & `dagster-1.7.6/dagster/_utils/env.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/error.py` & `dagster-1.7.6/dagster/_utils/error.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/external.py` & `dagster-1.7.6/dagster/_utils/external.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/forked_pdb.py` & `dagster-1.7.6/dagster/_utils/forked_pdb.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/hosted_user_process.py` & `dagster-1.7.6/dagster/_utils/hosted_user_process.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/indenting_printer.py` & `dagster-1.7.6/dagster/_utils/indenting_printer.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/internal_init.py` & `dagster-1.7.6/dagster/_utils/internal_init.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/interrupts.py` & `dagster-1.7.6/dagster/_utils/interrupts.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/log.py` & `dagster-1.7.6/dagster/_utils/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,15 @@
     timestamper = structlog.processors.TimeStamper(fmt="iso", utc=True)
 
     shared_processors = [
         structlog.stdlib.add_logger_name,
         structlog.stdlib.add_log_level,
         timestamper,
         structlog.processors.StackInfoRenderer(),
+        structlog.stdlib.ExtraAdder(),
     ]
 
     return shared_processors
 
 
 def get_structlog_json_formatter() -> structlog.stdlib.ProcessorFormatter:
     return structlog.stdlib.ProcessorFormatter(
```

### Comparing `dagster-1.7.5/dagster/_utils/merger.py` & `dagster-1.7.6/dagster/_utils/merger.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/net.py` & `dagster-1.7.6/dagster/_utils/net.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/schedules.py` & `dagster-1.7.6/dagster/_utils/schedules.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,24 +3,22 @@
 import functools
 import math
 import re
 from typing import Iterator, Optional, Sequence, Union
 
 import pendulum
 from croniter import croniter as _croniter
+from dateutil.relativedelta import relativedelta
+from dateutil.tz import datetime_ambiguous, datetime_exists
 
 import dagster._check as check
 from dagster._core.definitions.partition import ScheduleType
+from dagster._seven.compat.datetime import timezone_from_string
 from dagster._seven.compat.pendulum import (
-    POST_TRANSITION,
-    PRE_TRANSITION,
-    TRANSITION_ERROR,
-    PendulumDateTime,
-    create_pendulum_time,
-    get_crontab_day_of_week,
+    pendulum_create_timezone,
 )
 
 # Monthly schedules with 29-31 won't reliably run every month
 MAX_DAY_OF_MONTH_WITH_GUARANTEED_MONTHLY_INTERVAL = 28
 
 CRON_RANGES = ((0, 59), (0, 23), (1, 31), (1, 12), (0, 7), (0, 59))
 CRON_STEP_SEARCH_REGEX = re.compile(r"^([^-]+)-([^-/]+)(/(\d+))?$")
@@ -32,46 +30,29 @@
 
     @classmethod
     @functools.lru_cache(maxsize=128)
     def expand(cls, *args, **kwargs):
         return super().expand(*args, **kwargs)
 
 
-def _exact_match(
+def _is_simple_cron(
     cron_expression: str,
-    schedule_type: ScheduleType,
-    minutes: Optional[Sequence[int]],
-    hour: Optional[int],
-    day: Optional[int],
-    day_of_week: Optional[int],
-    dt: PendulumDateTime,
+    dt: datetime.datetime,
 ) -> bool:
-    """The default croniter match function only checks that the given datetime is within 60 seconds
-    of a cron schedule tick. This function checks that the given datetime is exactly on a cron tick.
+    """This function is purely an optimization to see if the provided datetime is already on an obvious boundary
+    of the common and easy to detect (daily at midnight and on the hour). The optimization is to avoid calling
+    _find_schedule_time to find the next cron boundary.
     """
     if cron_expression == "0 0 * * *":
         return dt.hour == 0 and dt.minute == 0 and dt.second == 0 and dt.microsecond == 0
 
     if cron_expression == "0 * * * *":
         return dt.minute == 0 and dt.second == 0 and dt.microsecond == 0
 
-    return (
-        dt.timestamp()
-        == _find_schedule_time(
-            cron_expression,
-            minutes,
-            hour,
-            day,
-            day_of_week,
-            schedule_type,
-            dt.add(seconds=1),
-            ascending=False,
-            already_on_boundary=False,
-        ).timestamp()
-    )
+    return False
 
 
 def is_valid_cron_string(cron_string: str) -> bool:
     if not CroniterShim.is_valid(cron_string):
         return False
     # Croniter < 1.4 returns 2 items
     # Croniter >= 1.4 returns 3 items
@@ -91,90 +72,90 @@
 
 def cron_string_repeats_every_hour(cron_string: str) -> bool:
     """Returns if the given cron schedule repeats every hour."""
     cron_parts, nth_weekday_of_month, *_ = CroniterShim.expand(cron_string)
     return len(cron_parts[1]) == 1 and cron_parts[1][0] == "*"
 
 
+def apply_fold_and_post_transition(date: datetime.datetime) -> datetime.datetime:
+    date = apply_post_transition(date)
+    return _apply_fold(date)
+
+
+def _apply_fold(date: datetime.datetime) -> datetime.datetime:
+    """For consistency, always choose the latter of the two possible times during a fall DST
+    transition when there are two possibilities - match behavior described in the docs:
+    https://docs.dagster.io/concepts/partitions-schedules-sensors/schedules#execution-time-and-daylight-savings-time)
+
+    Never call this with datetimes that could be non-existant. datetime_ambiguous will return true
+    but folding them will leave them non-existant.
+    """  # noqa: D415
+    if date.fold == 0 and datetime_ambiguous(date):
+        return date.replace(fold=1)
+    return date
+
+
+def apply_post_transition(
+    date: datetime.datetime,
+) -> datetime.datetime:
+    if not datetime_exists(date):
+        # If we fall on a non-existant time (e.g. between 2 and 3AM during a DST transition)
+        # advance to the end of the window, which does exist - match behavior described in the docs:
+        # https://docs.dagster.io/concepts/partitions-schedules-sensors/schedules#execution-time-and-daylight-savings-time)
+
+        # This assumes that all dst offsets are <= to an hour, which is true at time of writing.
+        # The date passed to dst needs to be in DST to get the offset for the timezone.
+        dst_offset = check.not_none(date.tzinfo).dst(date + datetime.timedelta(hours=1))
+
+        # This assumes that all dst transitions happen on the hour, which is true at time of writing.
+        # Rewind time to the start of the transition and then add the offset to get the first time out of the transition.
+        start_dst = date.replace(minute=0, second=0, microsecond=0)
+        return start_dst + check.not_none(dst_offset)
+    return date
+
+
 def _replace_date_fields(
-    pendulum_date: PendulumDateTime,
+    date: datetime.datetime,
     hour: int,
     minute: int,
     day: int,
 ):
-    try:
-        new_time = create_pendulum_time(
-            pendulum_date.year,
-            pendulum_date.month,
-            day,
-            hour,
-            minute,
-            0,
-            0,
-            tz=pendulum_date.timezone_name,
-            dst_rule=TRANSITION_ERROR,
-        )
-    except pendulum.tz.exceptions.NonExistingTime:  # type: ignore
-        # If we fall on a non-existant time (e.g. between 2 and 3AM during a DST transition)
-        # advance to the end of the window, which does exist - match behavior described in the docs:
-        # https://docs.dagster.io/concepts/partitions-schedules-sensors/schedules#execution-time-and-daylight-savings-time)
-        new_time = create_pendulum_time(
-            pendulum_date.year,
-            pendulum_date.month,
-            day,
-            hour + 1,
-            0,
-            0,
-            0,
-            tz=pendulum_date.timezone_name,
-            dst_rule=TRANSITION_ERROR,
-        )
-    except pendulum.tz.exceptions.AmbiguousTime:  # type: ignore
-        # For consistency, always choose the latter of the two possible times during a fall DST
-        # transition when there are two possibilities - match behavior described in the docs:
-        # https://docs.dagster.io/concepts/partitions-schedules-sensors/schedules#execution-time-and-daylight-savings-time)
-        new_time = create_pendulum_time(
-            pendulum_date.year,
-            pendulum_date.month,
-            day,
-            hour,
-            minute,
-            0,
-            0,
-            tz=pendulum_date.timezone_name,
-            dst_rule=POST_TRANSITION,
-        )
-
-    return new_time
+    new_date = date.replace(
+        day=day,
+        hour=hour,
+        minute=minute,
+        second=0,
+        microsecond=0,
+    )
+    return apply_fold_and_post_transition(new_date)
 
 
 SECONDS_PER_MINUTE = 60
 MINUTES_PER_HOUR = 60
 
 
 def _find_hourly_schedule_time(
     minutes: Sequence[int],
-    pendulum_date: PendulumDateTime,
+    date: datetime.datetime,
     ascending: bool,
     already_on_boundary: bool,
-) -> PendulumDateTime:
+) -> datetime.datetime:
     if ascending:
         # short-circuit if minutes and seconds are already correct
         if len(minutes) == 1 and (
             already_on_boundary
-            or (
-                pendulum_date.minute == minutes[0]
-                and pendulum_date.second == 0
-                and pendulum_date.microsecond == 0
-            )
+            or (date.minute == minutes[0] and date.second == 0 and date.microsecond == 0)
         ):
-            return pendulum_date.add(hours=1)
+            # switch to utc so that timedelta behaves as expected instead of doing walltime math
+            new_date = date.astimezone(datetime.timezone.utc) + datetime.timedelta(hours=1)
+            new_date = new_date.astimezone(date.tzinfo)
+            return new_date
 
         # clear microseconds
-        new_timestamp = math.ceil(pendulum_date.timestamp())
+        new_timestamp = math.ceil(date.timestamp())
         # clear seconds
         new_timestamp = (
             new_timestamp
             + (SECONDS_PER_MINUTE - new_timestamp % SECONDS_PER_MINUTE) % SECONDS_PER_MINUTE
         )
 
         current_minute = (new_timestamp // SECONDS_PER_MINUTE) % SECONDS_PER_MINUTE
@@ -183,302 +164,268 @@
 
         for minute in minutes:
             new_timestamp_cand = new_timestamp + SECONDS_PER_MINUTE * (
                 (minute - current_minute) % MINUTES_PER_HOUR
             )
 
             # move forward an hour if we haven't moved forwards yet
-            if new_timestamp_cand <= pendulum_date.timestamp():
+            if new_timestamp_cand <= date.timestamp():
                 new_timestamp_cand = new_timestamp_cand + SECONDS_PER_MINUTE * MINUTES_PER_HOUR
 
             final_timestamp = (
                 new_timestamp_cand
                 if not final_timestamp
                 else min(final_timestamp, new_timestamp_cand)
             )
-
     else:
         if len(minutes) == 1 and (
             already_on_boundary
-            or (
-                pendulum_date.minute == minutes[0]
-                and pendulum_date.second == 0
-                and pendulum_date.microsecond == 0
-            )
+            or (date.minute == minutes[0] and date.second == 0 and date.microsecond == 0)
         ):
-            return pendulum_date.subtract(hours=1)
+            # switch to utc so that timedelta behaves as expected instead of doing walltime math
+            new_date = date.astimezone(datetime.timezone.utc) - datetime.timedelta(hours=1)
+            new_date = new_date.astimezone(date.tzinfo)
+            return new_date
 
         # clear microseconds
-        new_timestamp = math.floor(pendulum_date.timestamp())
+        new_timestamp = math.floor(date.timestamp())
         # clear seconds
         new_timestamp = new_timestamp - new_timestamp % SECONDS_PER_MINUTE
 
         # move minutes back to correct place
         current_minute = (new_timestamp // SECONDS_PER_MINUTE) % SECONDS_PER_MINUTE
 
         final_timestamp = None
 
         for minute in minutes:
             new_timestamp_cand = new_timestamp - SECONDS_PER_MINUTE * (
                 (current_minute - minute) % MINUTES_PER_HOUR
             )
 
             # move back an hour if we haven't moved backwards yet
-            if new_timestamp_cand >= pendulum_date.timestamp():
+            if new_timestamp_cand >= date.timestamp():
                 new_timestamp_cand = new_timestamp_cand - SECONDS_PER_MINUTE * MINUTES_PER_HOUR
 
             final_timestamp = (
                 new_timestamp_cand
                 if not final_timestamp
                 else max(final_timestamp, new_timestamp_cand)
             )
 
-    return pendulum.from_timestamp(final_timestamp, tz=pendulum_date.timezone_name)
+    return datetime.datetime.fromtimestamp(check.not_none(final_timestamp), tz=date.tzinfo)
 
 
 def _find_daily_schedule_time(
     minute: int,
     hour: int,
-    pendulum_date: PendulumDateTime,
+    date: datetime.datetime,
     ascending: bool,
     already_on_boundary: bool,
-) -> PendulumDateTime:
+) -> datetime.datetime:
     # First move to the correct time of day today (ignoring whether it is the correct day)
-
-    if not already_on_boundary and (
-        pendulum_date.hour != hour
-        or pendulum_date.minute != minute
-        or pendulum_date.second != 0
-        or pendulum_date.microsecond != 0
+    if not already_on_boundary or (
+        date.hour != hour or date.minute != minute or date.second != 0 or date.microsecond != 0
     ):
         new_time = _replace_date_fields(
-            pendulum_date,
+            date,
             hour,
             minute,
-            pendulum_date.day,
+            date.day,
         )
     else:
-        new_time = pendulum_date
-
-    new_hour = new_time.hour
+        new_time = date
 
     if ascending:
-        if already_on_boundary or new_time.timestamp() <= pendulum_date.timestamp():
-            new_time = new_time.add(days=1)
+        if already_on_boundary or new_time.timestamp() <= date.timestamp():
+            new_time = new_time + datetime.timedelta(days=1)
     else:
-        if already_on_boundary or new_time.timestamp() >= pendulum_date.timestamp():
-            # Move back a day if needed
-            new_time = new_time.subtract(days=1)
+        if already_on_boundary or new_time.timestamp() >= date.timestamp():
+            new_time = new_time - datetime.timedelta(days=1)
 
-    # If the hour has changed from either what it was before or the hour on the cronstring,
+    # If the hour or minute has changed the schedule in cronstring,
     # double-check that it's still correct in case we crossed a DST boundary
-    if new_time.hour != new_hour or new_time.hour != hour:
+    if new_time.hour != hour or new_time.minute != minute:
         new_time = _replace_date_fields(
             new_time,
             hour,
             minute,
             new_time.day,
         )
+    return apply_fold_and_post_transition(new_time)
+
 
-    return new_time
+def _get_crontab_day_of_week(dt: datetime.datetime) -> int:
+    weekday = dt.isoweekday()
+    # crontab has 0-6, sunday - saturday
+    # isoweekday is 1-7 monday - sunday
+    return weekday if weekday <= 6 else 0
 
 
 def _find_weekly_schedule_time(
     minute: int,
     hour: int,
     day_of_week: int,
-    pendulum_date: PendulumDateTime,
+    date: datetime.datetime,
     ascending: bool,
     already_on_boundary: bool,
-) -> PendulumDateTime:
+) -> datetime.datetime:
     # first move to the correct time of day
     if not already_on_boundary:
         new_time = _replace_date_fields(
-            pendulum_date,
+            date,
             hour,
             minute,
-            pendulum_date.day,
+            date.day,
         )
         # Move to the correct day of the week
-        current_day_of_week = get_crontab_day_of_week(new_time)
+        current_day_of_week = _get_crontab_day_of_week(new_time)
 
         if day_of_week != current_day_of_week:
             if ascending:
-                new_time = new_time.add(days=(day_of_week - current_day_of_week) % 7)
+                new_time = new_time + relativedelta(days=(day_of_week - current_day_of_week) % 7)
             else:
-                new_time = new_time.subtract(days=(current_day_of_week - day_of_week) % 7)
-
+                new_time = new_time - relativedelta(days=(current_day_of_week - day_of_week) % 7)
     else:
-        new_time = pendulum_date
-
-    new_hour = new_time.hour
+        new_time = date
 
     # Make sure that we've actually moved in the correct direction, advance if we haven't
     if ascending:
-        if already_on_boundary or new_time.timestamp() <= pendulum_date.timestamp():
-            new_time = new_time.add(weeks=1)
+        if already_on_boundary or new_time.timestamp() <= date.timestamp():
+            new_time = new_time + relativedelta(weeks=1)
     else:
-        if already_on_boundary or new_time.timestamp() >= pendulum_date.timestamp():
-            new_time = new_time.subtract(weeks=1)
+        if already_on_boundary or new_time.timestamp() >= date.timestamp():
+            new_time = new_time - relativedelta(weeks=1)
 
-    # If the hour has changed from either what it was before or the hour on the cronstring,
+    # If the hour or minute has from the schedule in cronstring,
     # double-check that it's still correct in case we crossed a DST boundary
-    if new_time.hour != new_hour or new_time.hour != hour:
+    if new_time.hour != hour or new_time.minute != minute:
         new_time = _replace_date_fields(
             new_time,
             hour,
             minute,
             new_time.day,
         )
-
-    return new_time
+    return apply_fold_and_post_transition(new_time)
 
 
 def _find_monthly_schedule_time(
     minute: int,
     hour: int,
     day: int,
-    pendulum_date: PendulumDateTime,
+    date: datetime.datetime,
     ascending: bool,
     already_on_boundary: bool,
-) -> PendulumDateTime:
+) -> datetime.datetime:
     # First move to the correct day and time of day
     if not already_on_boundary:
         new_time = _replace_date_fields(
-            pendulum_date,
+            date,
             check.not_none(hour),
             check.not_none(minute),
             check.not_none(day),
         )
     else:
-        new_time = pendulum_date
-
-    new_hour = new_time.hour
+        new_time = date
 
     if ascending:
-        if already_on_boundary or new_time.timestamp() <= pendulum_date.timestamp():
-            new_time = new_time.add(months=1)
+        if already_on_boundary or new_time.timestamp() <= date.timestamp():
+            new_time = new_time + relativedelta(months=1)
     else:
-        if already_on_boundary or new_time.timestamp() >= pendulum_date.timestamp():
+        if already_on_boundary or new_time.timestamp() >= date.timestamp():
             # Move back a month if needed
-            new_time = new_time.subtract(months=1)
+            new_time = new_time - relativedelta(months=1)
 
-    if new_time.hour != new_hour or new_time.hour != hour:
-        # Doing so may have adjusted the hour again if we crossed a DST boundary,
-        # so make sure it's still correct
+    # If the hour or minute has changed from the schedule in cronstring,
+    # double-check that it's still correct in case we crossed a DST boundary
+    if new_time.hour != hour or new_time.minute != minute:
         new_time = _replace_date_fields(
             new_time,
             check.not_none(hour),
             check.not_none(minute),
             check.not_none(day),
         )
 
-    return new_time
+    return apply_fold_and_post_transition(new_time)
 
 
 def _find_schedule_time(
-    cron_string: str,
     minutes: Optional[Sequence[int]],
     hour: Optional[int],
     day_of_month: Optional[int],
     day_of_week: Optional[int],
     schedule_type: ScheduleType,
-    pendulum_date: PendulumDateTime,
+    date: datetime.datetime,
     ascending: bool,
     # lets us skip slow work to find the starting point if we know that
     # we are already on the boundary of the cron interval
     already_on_boundary: bool,
-) -> PendulumDateTime:
+) -> datetime.datetime:
     if schedule_type == ScheduleType.HOURLY:
         return _find_hourly_schedule_time(
-            check.not_none(minutes), pendulum_date, ascending, already_on_boundary
+            check.not_none(minutes), date, ascending, already_on_boundary
         )
     elif schedule_type == ScheduleType.DAILY:
         minutes = check.not_none(minutes)
         check.invariant(len(minutes) == 1)
         return _find_daily_schedule_time(
             minutes[0],
             check.not_none(hour),
-            pendulum_date,
+            date,
             ascending,
             already_on_boundary,
         )
     elif schedule_type == ScheduleType.WEEKLY:
         minutes = check.not_none(minutes)
         check.invariant(len(minutes) == 1)
         return _find_weekly_schedule_time(
             minutes[0],
             check.not_none(hour),
             check.not_none(day_of_week),
-            pendulum_date,
+            date,
             ascending,
             already_on_boundary,
         )
     elif schedule_type == ScheduleType.MONTHLY:
         minutes = check.not_none(minutes)
         check.invariant(len(minutes) == 1)
         return _find_monthly_schedule_time(
             minutes[0],
             check.not_none(hour),
             check.not_none(day_of_month),
-            pendulum_date,
+            date,
             ascending,
             already_on_boundary,
         )
     else:
         raise Exception(f"Unexpected schedule type {schedule_type}")
 
 
 def _get_dates_to_consider_after_ambigious_time(
     cron_iter: CroniterShim,
     next_date: datetime.datetime,
-    timezone_str: str,
     repeats_every_hour: bool,
     ascending: bool,
 ):
     # Return a list of all times that need to be considered when the next date returned by
     # croniter is ambigious (e.g. 2:30 AM during a fall DST transition). This is tricky because
     # we need to make sure that we are emitting times in the correct order, so we return a sorted
     # contiguous sequence of times that include all potentially ambigious times.
-    post_transition_time = create_pendulum_time(
-        next_date.year,
-        next_date.month,
-        next_date.day,
-        next_date.hour,
-        next_date.minute,
-        next_date.second,
-        next_date.microsecond,
-        tz=timezone_str,
-        dst_rule=POST_TRANSITION,
-    )
-
-    dates_to_consider = [post_transition_time]
+    post_transition_time = next_date.replace(fold=1)
 
     # Most schedules only need to consider the POST_TRANSITION time and can return here.
     if not repeats_every_hour:
         return [post_transition_time]
 
     # hourly schedules are more complicated - they'll continue firing once an hour no
     # matter what, including both PRE_TRANSITION and POST_TRANSITION times. So we need
     # to make sure that every time in the ambigious timerange has both its PRE_TRANSITION
     # and POST_TRANSITION times considered and returned.
-    pre_transition_time = create_pendulum_time(
-        next_date.year,
-        next_date.month,
-        next_date.day,
-        next_date.hour,
-        next_date.minute,
-        next_date.second,
-        next_date.microsecond,
-        tz=timezone_str,
-        dst_rule=PRE_TRANSITION,
-    )
-    dates_to_consider.append(pre_transition_time)
+    pre_transition_time = next_date.replace(fold=0)
+    dates_to_consider = [post_transition_time, pre_transition_time]
 
-    # fill in any gaps between pre-transition time and post-transition time
     curr_pre_transition_time = pre_transition_time
     curr_post_transition_time = post_transition_time
     while True:
         if ascending:
             # Time always advances because get_next() is called, so we will eventually break
             # Stop once the current PRE_TRANSITION time exceeds the original POST_TRANSITION time
             # (so we know we have moved forward across the whole range)
@@ -492,55 +439,52 @@
             if curr_post_transition_time.timestamp() <= pre_transition_time.timestamp():
                 break
             next_date = cron_iter.get_prev(datetime.datetime)
 
         # Make sure we add both the PRE_TRANSITION and POST_TRANSITION times to the
         # list of dates to consider so every time emitted by the
         # croniter instance is considered and returned from the calling iterator
-        curr_pre_transition_time = create_pendulum_time(
-            next_date.year,
-            next_date.month,
-            next_date.day,
-            next_date.hour,
-            next_date.minute,
-            next_date.second,
-            next_date.microsecond,
-            tz=timezone_str,
-            dst_rule=PRE_TRANSITION,
+        curr_pre_transition_time = datetime.datetime(
+            year=next_date.year,
+            month=next_date.month,
+            day=next_date.day,
+            hour=next_date.hour,
+            minute=next_date.minute,
+            second=next_date.second,
+            microsecond=next_date.microsecond,
+            fold=0,
+            tzinfo=post_transition_time.tzinfo,
         )
         dates_to_consider.append(curr_pre_transition_time)
-
-        curr_post_transition_time = create_pendulum_time(
-            next_date.year,
-            next_date.month,
-            next_date.day,
-            next_date.hour,
-            next_date.minute,
-            next_date.second,
-            next_date.microsecond,
-            tz=timezone_str,
-            dst_rule=POST_TRANSITION,
+        curr_post_transition_time = datetime.datetime(
+            year=next_date.year,
+            month=next_date.month,
+            day=next_date.day,
+            hour=next_date.hour,
+            minute=next_date.minute,
+            second=next_date.second,
+            microsecond=next_date.microsecond,
+            fold=1,
+            tzinfo=post_transition_time.tzinfo,
         )
         dates_to_consider.append(curr_post_transition_time)
 
     return sorted(dates_to_consider, key=lambda d: d.timestamp())
 
 
 def _timezone_aware_cron_iter(
-    cron_string, timezone_str: str, start_timestamp: float, ascending: bool
-) -> Iterator[PendulumDateTime]:
+    cron_string, start_datetime: datetime.datetime, ascending: bool
+) -> Iterator[datetime.datetime]:
     """Use croniter to determine the next timestamp matching the passed in cron string
     that is past the passed in UTC timestamp. croniter can only be trusted to compute
     non-timezone aware cron intervals, so we first figure out the time corresponding to the
     passed in timestamp without taking any timezones into account, use croniter to
     determine the next time that matches the cron string, translate that back into the passed in
     timezone, and repeat, returning the first time that is later than the passed in timestamp.
     """
-    start_datetime = pendulum.from_timestamp(start_timestamp, tz=timezone_str)
-
     # Create a naive (timezone-free) datetime to pass into croniter
     naive_time = datetime.datetime(
         year=start_datetime.year,
         month=start_datetime.month,
         day=start_datetime.day,
         hour=start_datetime.hour,
         minute=start_datetime.minute,
@@ -563,15 +507,15 @@
     # entirely and just move on to the next matching time (instead of returning
     # the end time of the non-existant interval), and when there are two times that match the cron
     # string, they return both instead of picking the latter time.
     repeats_every_hour = cron_string_repeats_every_hour(cron_string)
 
     # Chronological order of dates to return
     dates_to_consider = []
-
+    start_timestamp = start_datetime.timestamp()
     while True:
         # Work through everything currently in dates_to_consider
         if ascending:
             for next_date_with_tz in dates_to_consider:
                 next_timestamp = next_date_with_tz.timestamp()
                 if next_timestamp > start_timestamp:
                     start_timestamp = next_timestamp
@@ -586,54 +530,38 @@
         # Clear the list and generate new candidates using croniter
         dates_to_consider = []
 
         if ascending:
             next_date = cron_iter.get_next(datetime.datetime)
         else:
             next_date = cron_iter.get_prev(datetime.datetime)
+        next_date_with_tz = datetime.datetime(
+            year=next_date.year,
+            month=next_date.month,
+            day=next_date.day,
+            hour=next_date.hour,
+            minute=next_date.minute,
+            second=next_date.second,
+            microsecond=next_date.microsecond,
+            tzinfo=start_datetime.tzinfo,
+        )
 
-        try:
-            dates_to_consider = [
-                create_pendulum_time(
-                    next_date.year,
-                    next_date.month,
-                    next_date.day,
-                    next_date.hour,
-                    next_date.minute,
-                    next_date.second,
-                    next_date.microsecond,
-                    tz=timezone_str,
-                    dst_rule=TRANSITION_ERROR,
-                )
-            ]
-        except pendulum.tz.exceptions.NonExistingTime:  # type:ignore
+        dates_to_consider = [next_date_with_tz]
+        if not datetime_exists(next_date_with_tz):
             if repeats_every_hour:
                 # hourly schedules just move on to the next time
                 dates_to_consider = []
             else:
                 # other schedules advance to the time at the end of the interval (so that e.g.
                 # a daily schedule doesn't miss an entire day)
-                dates_to_consider = [
-                    create_pendulum_time(
-                        next_date.year,
-                        next_date.month,
-                        next_date.day,
-                        next_date.hour + 1,
-                        0,
-                        0,
-                        0,
-                        tz=timezone_str,
-                        dst_rule=TRANSITION_ERROR,
-                    )
-                ]
-        except pendulum.tz.exceptions.AmbiguousTime:  # type: ignore
+                dates_to_consider = [apply_post_transition(next_date_with_tz)]
+        elif datetime_ambiguous(next_date_with_tz):
             dates_to_consider = _get_dates_to_consider_after_ambigious_time(
                 cron_iter=cron_iter,
-                next_date=next_date,
-                timezone_str=timezone_str,
+                next_date=next_date_with_tz,
                 repeats_every_hour=repeats_every_hour,
                 ascending=ascending,
             )
 
 
 def _has_out_of_range_cron_interval_str(cron_string: str):
     assert CroniterShim.is_valid(cron_string)
@@ -700,16 +628,16 @@
         ):
             # only return on leap years
             if calendar.isleap(dt.year):
                 # shift 28th back to 29th
                 shifted_dt = dt + datetime.timedelta(days=1)
                 yield shifted_dt
         return
-
-    timezone_str = execution_timezone if execution_timezone else "UTC"
+    execution_timezone = execution_timezone or "UTC"
+    timezone = pendulum_create_timezone(execution_timezone)
 
     # Croniter < 1.4 returns 2 items
     # Croniter >= 1.4 returns 3 items
     cron_parts, nth_weekday_of_month, *_ = CroniterShim.expand(cron_string)
 
     is_numeric = [len(part) == 1 and part[0] != "*" for part in cron_parts]
     is_wildcard = [len(part) == 1 and part[0] == "*" for part in cron_parts]
@@ -750,59 +678,50 @@
     if is_numeric[2]:
         expected_day = int(cron_parts[2][0])
 
     if is_numeric[4]:
         expected_day_of_week = int(cron_parts[4][0])
 
     if known_schedule_type:
-        start_datetime = pendulum.from_timestamp(start_timestamp, tz=timezone_str)
+        start_datetime = datetime.datetime.fromtimestamp(
+            start_timestamp, tz=timezone_from_string(execution_timezone)
+        )
 
-        if start_offset == 0 and _exact_match(
-            cron_string,
-            known_schedule_type,
-            expected_minutes,
-            expected_hour,
-            expected_day,
-            expected_day_of_week,
-            start_datetime,
-        ):
+        if start_offset == 0 and _is_simple_cron(cron_string, start_datetime):
             # In simple cases, where you're already on a cron boundary, the below logic is unnecessary
             # and slow
             next_date = start_datetime
             # This is already on a cron boundary, so yield it
-            yield start_datetime
+            yield pendulum.from_timestamp(next_date.timestamp(), tz=timezone)
         else:
             next_date = _find_schedule_time(
-                cron_string,
                 expected_minutes,
                 expected_hour,
                 expected_day,
                 expected_day_of_week,
                 known_schedule_type,
                 start_datetime,
                 ascending=not ascending,  # Going in the reverse direction
                 already_on_boundary=False,
             )
             check.invariant(start_offset <= 0)
             for _ in range(-start_offset):
                 next_date = _find_schedule_time(
-                    cron_string,
                     expected_minutes,
                     expected_hour,
                     expected_day,
                     expected_day_of_week,
                     known_schedule_type,
                     next_date,
                     ascending=not ascending,  # Going in the reverse direction
                     already_on_boundary=True,
                 )
 
         while True:
             next_date = _find_schedule_time(
-                cron_string,
                 expected_minutes,
                 expected_hour,
                 expected_day,
                 expected_day_of_week,
                 known_schedule_type,
                 next_date,
                 ascending=ascending,
@@ -812,54 +731,56 @@
             if start_offset == 0:
                 if ascending:
                     # Guard against _find_schedule_time returning unexpected results
                     check.invariant(next_date.timestamp() >= start_timestamp)
                 else:
                     check.invariant(next_date.timestamp() <= start_timestamp)
 
-            yield next_date
+            yield pendulum.from_timestamp(next_date.timestamp(), tz=timezone)
     else:
         yield from _croniter_string_iterator(
-            start_timestamp, cron_string, timezone_str, ascending, start_offset
+            start_timestamp, cron_string, execution_timezone, ascending, start_offset
         )
 
 
 def _croniter_string_iterator(
     start_timestamp: float,
     cron_string: str,
     timezone_str: str,
     ascending: bool = True,
     start_offset: int = 0,
 ):
-    reverse_cron = _timezone_aware_cron_iter(
-        cron_string, timezone_str, start_timestamp, ascending=not ascending
+    timezone = pendulum_create_timezone(timezone_str)
+    start_datetime = datetime.datetime.fromtimestamp(
+        start_timestamp, timezone_from_string(timezone_str)
     )
+    reverse_cron = _timezone_aware_cron_iter(cron_string, start_datetime, ascending=not ascending)
     next_date = None
     check.invariant(start_offset <= 0)
     for _ in range(-start_offset + 1):
         next_date = next(reverse_cron)
-
-    forward_cron = _timezone_aware_cron_iter(
-        cron_string, timezone_str, check.not_none(next_date).timestamp(), ascending=ascending
-    )
+    next_date = check.not_none(next_date).astimezone(start_datetime.tzinfo)
+    forward_cron = _timezone_aware_cron_iter(cron_string, next_date, ascending=ascending)
     while True:
         next_date = next(forward_cron)
 
         if start_offset == 0:
             if ascending:
                 # Guard against _find_schedule_time returning unexpected results
                 check.invariant(next_date.timestamp() >= start_timestamp)
             else:
                 check.invariant(next_date.timestamp() <= start_timestamp)
 
-        yield next_date
+        yield pendulum.from_timestamp(next_date.timestamp(), tz=timezone)
 
 
 def reverse_cron_string_iterator(
-    end_timestamp: float, cron_string: str, execution_timezone: Optional[str]
+    end_timestamp: float,
+    cron_string: str,
+    execution_timezone: Optional[str],
 ) -> Iterator[datetime.datetime]:
     yield from cron_string_iterator(end_timestamp, cron_string, execution_timezone, ascending=False)
 
 
 def schedule_execution_time_iterator(
     start_timestamp: float,
     cron_schedule: Union[str, Sequence[str]],
@@ -900,26 +821,30 @@
             # Increment all iterators that generated the earliest subsequent datetime.
             for i, next_date in enumerate(next_dates):
                 if next_date == earliest_next_date:
                     next_dates[i] = next(iterators[i])
 
 
 def get_latest_completed_cron_tick(
-    cron_string: str, current_time: datetime.datetime, timezone: Optional[str]
+    cron_string: str,
+    current_time: datetime.datetime,
+    timezone: Optional[str],
 ) -> datetime.datetime:
     cron_iter = reverse_cron_string_iterator(
         end_timestamp=current_time.timestamp(),
         cron_string=cron_string,
         execution_timezone=timezone,
     )
-    return pendulum.instance(next(cron_iter))
+    return next(cron_iter)
 
 
 def get_next_cron_tick(
-    cron_string: str, current_time: datetime.datetime, timezone: Optional[str]
+    cron_string: str,
+    current_time: datetime.datetime,
+    timezone: Optional[str],
 ) -> datetime.datetime:
     cron_iter = cron_string_iterator(
         start_timestamp=current_time.timestamp(),
         cron_string=cron_string,
         execution_timezone=timezone,
     )
-    return pendulum.instance(next(cron_iter))
+    return next(cron_iter)
```

### Comparing `dagster-1.7.5/dagster/_utils/tags.py` & `dagster-1.7.6/dagster/_utils/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/temp_file.py` & `dagster-1.7.6/dagster/_utils/temp_file.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/test/__init__.py` & `dagster-1.7.6/dagster/_utils/test/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/test/data_versions.py` & `dagster-1.7.6/dagster/_utils/test/data_versions.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/test/mysql_instance.py` & `dagster-1.7.6/dagster/_utils/test/mysql_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/test/postgres_instance.py` & `dagster-1.7.6/dagster/_utils/test/postgres_instance.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/test/schedule_storage.py` & `dagster-1.7.6/dagster/_utils/test/schedule_storage.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/timing.py` & `dagster-1.7.6/dagster/_utils/timing.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/typed_dict.py` & `dagster-1.7.6/dagster/_utils/typed_dict.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/typing_api.py` & `dagster-1.7.6/dagster/_utils/typing_api.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/warnings.py` & `dagster-1.7.6/dagster/_utils/warnings.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster/_utils/yaml_utils.py` & `dagster-1.7.6/dagster/_utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-1.7.5/dagster.egg-info/PKG-INFO` & `dagster-1.7.6/dagster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster
-Version: 1.7.5
+Version: 1.7.6
 Summary: Dagster is an orchestration platform for the development, production, and observation of data assets.
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io
 Project-URL: GitHub, https://github.com/dagster-io/dagster
 Project-URL: Documentation, https://docs.dagster.io
```

### Comparing `dagster-1.7.5/dagster.egg-info/SOURCES.txt` & `dagster-1.7.6/dagster.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -195,19 +195,22 @@
 dagster/_core/definitions/asset_check_factories/freshness_checks/time_partition.py
 dagster/_core/definitions/declarative_scheduling/README.md
 dagster/_core/definitions/declarative_scheduling/__init__.py
 dagster/_core/definitions/declarative_scheduling/scheduling_condition.py
 dagster/_core/definitions/declarative_scheduling/scheduling_context.py
 dagster/_core/definitions/declarative_scheduling/scheduling_evaluation_info.py
 dagster/_core/definitions/declarative_scheduling/serialized_objects.py
+dagster/_core/definitions/declarative_scheduling/utils.py
 dagster/_core/definitions/declarative_scheduling/legacy/__init__.py
 dagster/_core/definitions/declarative_scheduling/legacy/asset_condition.py
 dagster/_core/definitions/declarative_scheduling/legacy/legacy_context.py
 dagster/_core/definitions/declarative_scheduling/legacy/rule_condition.py
 dagster/_core/definitions/declarative_scheduling/operands/__init__.py
+dagster/_core/definitions/declarative_scheduling/operands/parent_newer_condition.py
+dagster/_core/definitions/declarative_scheduling/operands/scheduled_since_condition.py
 dagster/_core/definitions/declarative_scheduling/operands/slice_conditions.py
 dagster/_core/definitions/declarative_scheduling/operands/updated_since_cron_condition.py
 dagster/_core/definitions/declarative_scheduling/operators/__init__.py
 dagster/_core/definitions/declarative_scheduling/operators/boolean_operators.py
 dagster/_core/definitions/declarative_scheduling/operators/dep_operators.py
 dagster/_core/definitions/decorators/__init__.py
 dagster/_core/definitions/decorators/asset_check_decorator.py
@@ -220,14 +223,15 @@
 dagster/_core/definitions/decorators/repository_decorator.py
 dagster/_core/definitions/decorators/schedule_decorator.py
 dagster/_core/definitions/decorators/sensor_decorator.py
 dagster/_core/definitions/decorators/source_asset_decorator.py
 dagster/_core/definitions/metadata/__init__.py
 dagster/_core/definitions/metadata/metadata_set.py
 dagster/_core/definitions/metadata/metadata_value.py
+dagster/_core/definitions/metadata/source_code.py
 dagster/_core/definitions/metadata/table.py
 dagster/_core/definitions/repository_definition/__init__.py
 dagster/_core/definitions/repository_definition/caching_index.py
 dagster/_core/definitions/repository_definition/repository_data.py
 dagster/_core/definitions/repository_definition/repository_data_builder.py
 dagster/_core/definitions/repository_definition/repository_definition.py
 dagster/_core/definitions/repository_definition/valid_definitions.py
@@ -250,17 +254,19 @@
 dagster/_core/execution/job_execution_result.py
 dagster/_core/execution/memoization.py
 dagster/_core/execution/poll_compute_logs.py
 dagster/_core/execution/resolve_versions.py
 dagster/_core/execution/resources_init.py
 dagster/_core/execution/retries.py
 dagster/_core/execution/run_cancellation_thread.py
+dagster/_core/execution/run_metrics_thread.py
 dagster/_core/execution/stats.py
 dagster/_core/execution/submit_asset_runs.py
 dagster/_core/execution/tags.py
+dagster/_core/execution/types.py
 dagster/_core/execution/validate_run_config.py
 dagster/_core/execution/watch_orphans.py
 dagster/_core/execution/with_resources.py
 dagster/_core/execution/context/__init__.py
 dagster/_core/execution/context/compute.py
 dagster/_core/execution/context/data_version_cache.py
 dagster/_core/execution/context/hook.py
@@ -583,14 +589,15 @@
 dagster/_serdes/serdes.py
 dagster/_serdes/utils.py
 dagster/_seven/__init__.py
 dagster/_seven/abc.py
 dagster/_seven/json.py
 dagster/_seven/temp_dir.py
 dagster/_seven/compat/__init__.py
+dagster/_seven/compat/datetime.py
 dagster/_seven/compat/pendulum.py
 dagster/_utils/__init__.py
 dagster/_utils/alert.py
 dagster/_utils/backoff.py
 dagster/_utils/cached_method.py
 dagster/_utils/caching_instance_queryer.py
 dagster/_utils/concurrency.py
```

### Comparing `dagster-1.7.5/dagster.egg-info/requires.txt` & `dagster-1.7.6/dagster.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 sqlalchemy<3,>=1.0
 toposort>=1.0
 watchdog>=0.8.3
 docstring-parser
 pydantic!=1.10.7,<3,>1.10.0
 rich
 filelock
-dagster-pipes==1.7.5
+dagster-pipes==1.7.6
 
 [:platform_system == "Windows"]
 psutil>=1.0
 pywin32!=226
 
 [:python_version < "3.11"]
 protobuf<5,>=3.20.0
@@ -93,8 +93,9 @@
 pytest-rerunfailures==10.0
 pytest-xdist==3.5.0
 pytest>=7.0.1
 responses<=0.23.1
 syrupy>=4.0.0
 tox==3.25.0
 morefs[asynclocal]
+fsspec<2024.5.0
 rapidfuzz
```

### Comparing `dagster-1.7.5/setup.py` & `dagster-1.7.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         "docstring-parser",
         "universal_pathlib; python_version<'3.12'",
         "universal_pathlib>=0.2.0; python_version>='3.12'",
         # https://github.com/pydantic/pydantic/issues/5821
         "pydantic>1.10.0,!= 1.10.7,<3",
         "rich",
         "filelock",
-        "dagster-pipes==1.7.5",
+        "dagster-pipes==1.7.6",
     ],
     extras_require={
         "docker": ["docker"],
         "test": [
             "buildkite-test-collector",
             "docker",
             f"grpcio-tools>={GRPC_VERSION_FLOOR}",
@@ -132,14 +132,15 @@
             "pytest-rerunfailures==10.0",
             "pytest-xdist==3.5.0",
             "pytest>=7.0.1",
             "responses<=0.23.1",  # https://github.com/getsentry/responses/issues/654
             "syrupy>=4.0.0",
             "tox==3.25.0",
             "morefs[asynclocal]",
+            "fsspec<2024.5.0",  # morefs incompatibly
             "rapidfuzz",
         ],
         "mypy": ["mypy==1.8.0"],
         "pyright": [
             "pyright==1.1.356",
             ### Stub packages
             "pandas-stubs",  # version will be resolved against pandas
```

