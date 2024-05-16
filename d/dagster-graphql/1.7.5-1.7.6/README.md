# Comparing `tmp/dagster-graphql-1.7.5.tar.gz` & `tmp/dagster-graphql-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-graphql-1.7.5.tar", last modified: Thu May  9 17:48:24 2024, max compression
+gzip compressed data, was "dagster-graphql-1.7.6.tar", last modified: Thu May 16 19:28:10 2024, max compression
```

## Comparing `dagster-graphql-1.7.5.tar` & `dagster-graphql-1.7.6.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:48:24.951762 dagster-graphql-1.7.5/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       49 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      691 2024-05-09 17:48:24.951762 dagster-graphql-1.7.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:48:24.935762 dagster-graphql-1.7.5/dagster_graphql/
--rw-r--r--   0 root         (0) root         (0)      641 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7401 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:48:24.939762 dagster-graphql-1.7.5/dagster_graphql/client/
--rw-r--r--   0 root         (0) root         (0)      482 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18338 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/client/client_queries.py
--rw-r--r--   0 root         (0) root         (0)     6966 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/client/query.py
--rw-r--r--   0 root         (0) root         (0)     2917 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/client/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:48:24.939762 dagster-graphql-1.7.5/dagster_graphql/implementation/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12826 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/asset_checks_loader.py
--rw-r--r--   0 root         (0) root         (0)    20532 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/events.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:48:24.939762 dagster-graphql-1.7.5/dagster_graphql/implementation/execution/
--rw-r--r--   0 root         (0) root         (0)    14499 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/execution/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12314 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/execution/backfill.py
--rw-r--r--   0 root         (0) root         (0)     3727 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/execution/dynamic_partitions.py
--rw-r--r--   0 root         (0) root         (0)     4819 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/execution/launch_execution.py
--rw-r--r--   0 root         (0) root         (0)     4895 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/execution/run_lifecycle.py
--rw-r--r--   0 root         (0) root         (0)     7721 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/external.py
--rw-r--r--   0 root         (0) root         (0)     4251 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_asset_checks.py
--rw-r--r--   0 root         (0) root         (0)     4926 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_asset_condition_evaluations.py
--rw-r--r--   0 root         (0) root         (0)    29476 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_assets.py
--rw-r--r--   0 root         (0) root         (0)     3658 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     1237 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_backfills.py
--rw-r--r--   0 root         (0) root         (0)     1179 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_env_vars.py
--rw-r--r--   0 root         (0) root         (0)     3009 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_instigators.py
--rw-r--r--   0 root         (0) root         (0)      951 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_logs.py
--rw-r--r--   0 root         (0) root         (0)    12681 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_partition_sets.py
--rw-r--r--   0 root         (0) root         (0)     3726 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_pipelines.py
--rw-r--r--   0 root         (0) root         (0)     2438 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_resources.py
--rw-r--r--   0 root         (0) root         (0)    15161 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_runs.py
--rw-r--r--   0 root         (0) root         (0)     9069 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_schedules.py
--rw-r--r--   0 root         (0) root         (0)    10352 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_sensors.py
--rw-r--r--   0 root         (0) root         (0)     2912 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_solids.py
--rw-r--r--   0 root         (0) root         (0)     2345 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_ticks.py
--rw-r--r--   0 root         (0) root         (0)    14555 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/loader.py
--rw-r--r--   0 root         (0) root         (0)     3097 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/run_config_schema.py
--rw-r--r--   0 root         (0) root         (0)      930 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/telemetry.py
--rw-r--r--   0 root         (0) root         (0)     9774 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/implementation/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:48:24.947762 dagster-graphql-1.7.5/dagster_graphql/schema/
--rw-r--r--   0 root         (0) root         (0)     2877 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8533 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/asset_checks.py
--rw-r--r--   0 root         (0) root         (0)    11998 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/asset_condition_evaluations.py
--rw-r--r--   0 root         (0) root         (0)    55503 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/asset_graph.py
--rw-r--r--   0 root         (0) root         (0)      385 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/asset_key.py
--rw-r--r--   0 root         (0) root         (0)     2188 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/asset_selections.py
--rw-r--r--   0 root         (0) root         (0)    11078 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/auto_materialize_asset_evaluations.py
--rw-r--r--   0 root         (0) root         (0)     2592 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/auto_materialize_policy.py
--rw-r--r--   0 root         (0) root         (0)    20849 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/backfill.py
--rw-r--r--   0 root         (0) root         (0)      627 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/config_type_or_error.py
--rw-r--r--   0 root         (0) root         (0)    15855 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/config_types.py
--rw-r--r--   0 root         (0) root         (0)     4823 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/dagster_types.py
--rw-r--r--   0 root         (0) root         (0)     1743 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/env_vars.py
--rw-r--r--   0 root         (0) root         (0)    17941 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/errors.py
--rw-r--r--   0 root         (0) root         (0)     5491 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/execution.py
--rw-r--r--   0 root         (0) root         (0)    19024 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/external.py
--rw-r--r--   0 root         (0) root         (0)     1769 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/freshness_policy.py
--rw-r--r--   0 root         (0) root         (0)    13742 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/inputs.py
--rw-r--r--   0 root         (0) root         (0)    12491 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/instance.py
--rw-r--r--   0 root         (0) root         (0)    28766 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/instigation.py
--rw-r--r--   0 root         (0) root         (0)      232 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/instigators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:48:24.947762 dagster-graphql-1.7.5/dagster_graphql/schema/logs/
--rw-r--r--   0 root         (0) root         (0)     3632 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2868 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/logs/compute_logs.py
--rw-r--r--   0 root         (0) root         (0)    21701 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/logs/events.py
--rw-r--r--   0 root         (0) root         (0)      816 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/logs/log_level.py
--rw-r--r--   0 root         (0) root         (0)     5440 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/metadata.py
--rw-r--r--   0 root         (0) root         (0)      111 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/paging.py
--rw-r--r--   0 root         (0) root         (0)      529 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/partition_mappings.py
--rw-r--r--   0 root         (0) root         (0)    17797 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/partition_sets.py
--rw-r--r--   0 root         (0) root         (0)      748 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/permissions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:48:24.947762 dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/
--rw-r--r--   0 root         (0) root         (0)     3263 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11060 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/config.py
--rw-r--r--   0 root         (0) root         (0)      582 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/config_result.py
--rw-r--r--   0 root         (0) root         (0)     1369 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/logger.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/mode.py
--rw-r--r--   0 root         (0) root         (0)    39840 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/pipeline.py
--rw-r--r--   0 root         (0) root         (0)      855 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/pipeline_ref.py
--rw-r--r--   0 root         (0) root         (0)     2213 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/pipeline_run_stats.py
--rw-r--r--   0 root         (0) root         (0)     1496 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/resource.py
--rw-r--r--   0 root         (0) root         (0)     1263 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1621 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/status.py
--rw-r--r--   0 root         (0) root         (0)      993 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/subscription.py
--rw-r--r--   0 root         (0) root         (0)     1654 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/repository_origin.py
--rw-r--r--   0 root         (0) root         (0)     9025 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/resources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:48:24.951762 dagster-graphql-1.7.5/dagster_graphql/schema/roots/
--rw-r--r--   0 root         (0) root         (0)     2094 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/roots/__init__.py
--rw-r--r--   0 root         (0) root         (0)      620 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/roots/assets.py
--rw-r--r--   0 root         (0) root         (0)      564 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/roots/execution_plan.py
--rw-r--r--   0 root         (0) root         (0)    32162 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/roots/mutation.py
--rw-r--r--   0 root         (0) root         (0)      723 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/roots/pipeline.py
--rw-r--r--   0 root         (0) root         (0)    47063 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/roots/query.py
--rw-r--r--   0 root         (0) root         (0)     2905 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/roots/subscription.py
--rw-r--r--   0 root         (0) root         (0)     5092 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/run_config.py
--rw-r--r--   0 root         (0) root         (0)     6523 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/runs.py
--rw-r--r--   0 root         (0) root         (0)     1438 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/schedule_dry_run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:48:24.951762 dagster-graphql-1.7.5/dagster_graphql/schema/schedules/
--rw-r--r--   0 root         (0) root         (0)     4945 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9135 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/schedules/schedules.py
--rw-r--r--   0 root         (0) root         (0)     1833 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/schedules/ticks.py
--rw-r--r--   0 root         (0) root         (0)     1312 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/sensor_dry_run.py
--rw-r--r--   0 root         (0) root         (0)    10196 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/sensors.py
--rw-r--r--   0 root         (0) root         (0)    30059 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/solids.py
--rw-r--r--   0 root         (0) root         (0)     2390 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/table.py
--rw-r--r--   0 root         (0) root         (0)     1421 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/tags.py
--rw-r--r--   0 root         (0) root         (0)      574 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/test.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/used_solid.py
--rw-r--r--   0 root         (0) root         (0)      950 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/schema/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:48:24.951762 dagster-graphql-1.7.5/dagster_graphql/test/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7078 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/test/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/dagster_graphql/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:48:24.935762 dagster-graphql-1.7.5/dagster_graphql.egg-info/
--rw-r--r--   0 root         (0) root         (0)      691 2024-05-09 17:48:24.000000 dagster-graphql-1.7.5/dagster_graphql.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4726 2024-05-09 17:48:24.000000 dagster-graphql-1.7.5/dagster_graphql.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:48:24.000000 dagster-graphql-1.7.5/dagster_graphql.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-05-09 17:48:24.000000 dagster-graphql-1.7.5/dagster_graphql.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       69 2024-05-09 17:48:24.000000 dagster-graphql-1.7.5/dagster_graphql.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-09 17:48:24.000000 dagster-graphql-1.7.5/dagster_graphql.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      180 2024-05-09 17:48:24.951762 dagster-graphql-1.7.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1531 2024-05-09 17:47:35.000000 dagster-graphql-1.7.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.188154 dagster-graphql-1.7.6/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      691 2024-05-16 19:28:10.188154 dagster-graphql-1.7.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.176154 dagster-graphql-1.7.6/dagster_graphql/
+-rw-r--r--   0 root         (0) root         (0)      641 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7401 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.176154 dagster-graphql-1.7.6/dagster_graphql/client/
+-rw-r--r--   0 root         (0) root         (0)      482 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18338 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/client/client_queries.py
+-rw-r--r--   0 root         (0) root         (0)     6966 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/client/query.py
+-rw-r--r--   0 root         (0) root         (0)     2917 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/client/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.180154 dagster-graphql-1.7.6/dagster_graphql/implementation/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12826 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/asset_checks_loader.py
+-rw-r--r--   0 root         (0) root         (0)    21152 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/events.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.180154 dagster-graphql-1.7.6/dagster_graphql/implementation/execution/
+-rw-r--r--   0 root         (0) root         (0)    14499 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/execution/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12324 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/execution/backfill.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/execution/dynamic_partitions.py
+-rw-r--r--   0 root         (0) root         (0)     4819 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/execution/launch_execution.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/execution/run_lifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     7721 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/external.py
+-rw-r--r--   0 root         (0) root         (0)     4251 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_asset_condition_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)    29547 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_assets.py
+-rw-r--r--   0 root         (0) root         (0)     3658 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     1237 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_backfills.py
+-rw-r--r--   0 root         (0) root         (0)     1179 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_env_vars.py
+-rw-r--r--   0 root         (0) root         (0)     3009 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_instigators.py
+-rw-r--r--   0 root         (0) root         (0)      951 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_logs.py
+-rw-r--r--   0 root         (0) root         (0)    12681 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_pipelines.py
+-rw-r--r--   0 root         (0) root         (0)     2438 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_resources.py
+-rw-r--r--   0 root         (0) root         (0)    15166 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_runs.py
+-rw-r--r--   0 root         (0) root         (0)     9069 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_schedules.py
+-rw-r--r--   0 root         (0) root         (0)    10352 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_sensors.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_solids.py
+-rw-r--r--   0 root         (0) root         (0)     2345 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_ticks.py
+-rw-r--r--   0 root         (0) root         (0)    14555 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/loader.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/run_config_schema.py
+-rw-r--r--   0 root         (0) root         (0)      930 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/telemetry.py
+-rw-r--r--   0 root         (0) root         (0)     9774 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/implementation/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.184154 dagster-graphql-1.7.6/dagster_graphql/schema/
+-rw-r--r--   0 root         (0) root         (0)     2877 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8533 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/asset_checks.py
+-rw-r--r--   0 root         (0) root         (0)    11998 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/asset_condition_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)    55503 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/asset_graph.py
+-rw-r--r--   0 root         (0) root         (0)      385 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/asset_key.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/asset_selections.py
+-rw-r--r--   0 root         (0) root         (0)    11078 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/auto_materialize_asset_evaluations.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/auto_materialize_policy.py
+-rw-r--r--   0 root         (0) root         (0)    22713 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/backfill.py
+-rw-r--r--   0 root         (0) root         (0)      627 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/config_type_or_error.py
+-rw-r--r--   0 root         (0) root         (0)    15855 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/config_types.py
+-rw-r--r--   0 root         (0) root         (0)     4823 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/dagster_types.py
+-rw-r--r--   0 root         (0) root         (0)     1743 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/env_vars.py
+-rw-r--r--   0 root         (0) root         (0)    17941 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/errors.py
+-rw-r--r--   0 root         (0) root         (0)     5491 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/execution.py
+-rw-r--r--   0 root         (0) root         (0)    19024 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/external.py
+-rw-r--r--   0 root         (0) root         (0)     1769 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/freshness_policy.py
+-rw-r--r--   0 root         (0) root         (0)    13742 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/inputs.py
+-rw-r--r--   0 root         (0) root         (0)    12491 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/instance.py
+-rw-r--r--   0 root         (0) root         (0)    28766 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/instigation.py
+-rw-r--r--   0 root         (0) root         (0)      232 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/instigators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.184154 dagster-graphql-1.7.6/dagster_graphql/schema/logs/
+-rw-r--r--   0 root         (0) root         (0)     3632 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2868 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/logs/compute_logs.py
+-rw-r--r--   0 root         (0) root         (0)    21701 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/logs/events.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/logs/log_level.py
+-rw-r--r--   0 root         (0) root         (0)     6110 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      111 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/paging.py
+-rw-r--r--   0 root         (0) root         (0)      529 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/partition_mappings.py
+-rw-r--r--   0 root         (0) root         (0)    17797 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/partition_sets.py
+-rw-r--r--   0 root         (0) root         (0)      748 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/permissions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.188154 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/
+-rw-r--r--   0 root         (0) root         (0)     3263 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11060 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/config.py
+-rw-r--r--   0 root         (0) root         (0)      582 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/config_result.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/mode.py
+-rw-r--r--   0 root         (0) root         (0)    39840 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)      855 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/pipeline_ref.py
+-rw-r--r--   0 root         (0) root         (0)     2213 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/pipeline_run_stats.py
+-rw-r--r--   0 root         (0) root         (0)     1496 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1263 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1621 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/status.py
+-rw-r--r--   0 root         (0) root         (0)      993 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     1654 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/repository_origin.py
+-rw-r--r--   0 root         (0) root         (0)     9025 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/resources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.188154 dagster-graphql-1.7.6/dagster_graphql/schema/roots/
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/roots/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      620 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/roots/assets.py
+-rw-r--r--   0 root         (0) root         (0)      564 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/roots/execution_plan.py
+-rw-r--r--   0 root         (0) root         (0)    32162 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/roots/mutation.py
+-rw-r--r--   0 root         (0) root         (0)      723 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/roots/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)    47162 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/roots/query.py
+-rw-r--r--   0 root         (0) root         (0)     2905 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/roots/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     5092 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/run_config.py
+-rw-r--r--   0 root         (0) root         (0)     6523 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/runs.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/schedule_dry_run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.188154 dagster-graphql-1.7.6/dagster_graphql/schema/schedules/
+-rw-r--r--   0 root         (0) root         (0)     4945 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9135 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/schedules/schedules.py
+-rw-r--r--   0 root         (0) root         (0)     1833 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/schedules/ticks.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/sensor_dry_run.py
+-rw-r--r--   0 root         (0) root         (0)    10196 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/sensors.py
+-rw-r--r--   0 root         (0) root         (0)    30059 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/solids.py
+-rw-r--r--   0 root         (0) root         (0)     2390 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/table.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/tags.py
+-rw-r--r--   0 root         (0) root         (0)      574 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/test.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/used_solid.py
+-rw-r--r--   0 root         (0) root         (0)      950 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/schema/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.188154 dagster-graphql-1.7.6/dagster_graphql/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7078 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/test/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/dagster_graphql/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 19:28:10.176154 dagster-graphql-1.7.6/dagster_graphql.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      691 2024-05-16 19:28:10.000000 dagster-graphql-1.7.6/dagster_graphql.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4726 2024-05-16 19:28:10.000000 dagster-graphql-1.7.6/dagster_graphql.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 19:28:10.000000 dagster-graphql-1.7.6/dagster_graphql.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-05-16 19:28:10.000000 dagster-graphql-1.7.6/dagster_graphql.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2024-05-16 19:28:10.000000 dagster-graphql-1.7.6/dagster_graphql.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-16 19:28:10.000000 dagster-graphql-1.7.6/dagster_graphql.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2024-05-16 19:28:10.188154 dagster-graphql-1.7.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1531 2024-05-16 19:27:09.000000 dagster-graphql-1.7.6/setup.py
```

### Comparing `dagster-graphql-1.7.5/LICENSE` & `dagster-graphql-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/PKG-INFO` & `dagster-graphql-1.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.7.5
+Version: 1.7.6
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.7.5/dagster_graphql/__init__.py` & `dagster-graphql-1.7.6/dagster_graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/cli.py` & `dagster-graphql-1.7.6/dagster_graphql/cli.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/client/client.py` & `dagster-graphql-1.7.6/dagster_graphql/client/client.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/client/client_queries.py` & `dagster-graphql-1.7.6/dagster_graphql/client/client_queries.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/client/query.py` & `dagster-graphql-1.7.6/dagster_graphql/client/query.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/client/utils.py` & `dagster-graphql-1.7.6/dagster_graphql/client/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/asset_checks_loader.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/asset_checks_loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/events.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/events.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     TableSchemaMetadataValue,
     TextMetadataValue,
     TimestampMetadataValue,
     UrlMetadataValue,
 )
 from dagster._core.definitions.asset_check_evaluation import AssetCheckEvaluationPlanned
 from dagster._core.definitions.metadata import (
+    CodeReferencesMetadataValue,
     DagsterRunMetadataValue,
     MetadataValue,
     TableColumnLineageMetadataValue,
 )
 from dagster._core.events import (
     DagsterEventType,
     HandledOutputData,
@@ -41,18 +42,20 @@
 MIN_INT = -2147483648
 
 
 def iterate_metadata_entries(metadata: Mapping[str, MetadataValue]) -> Iterator[Any]:
     from ..schema.metadata import (
         GrapheneAssetMetadataEntry,
         GrapheneBoolMetadataEntry,
+        GrapheneCodeReferencesMetadataEntry,
         GrapheneFloatMetadataEntry,
         GrapheneIntMetadataEntry,
         GrapheneJobMetadataEntry,
         GrapheneJsonMetadataEntry,
+        GrapheneLocalFileCodeReference,
         GrapheneMarkdownMetadataEntry,
         GrapheneNotebookMetadataEntry,
         GrapheneNullMetadataEntry,
         GraphenePathMetadataEntry,
         GraphenePipelineRunMetadataEntry,
         GraphenePythonArtifactMetadataEntry,
         GrapheneTableColumnLineageEntry,
@@ -148,14 +151,26 @@
         elif isinstance(value, DagsterJobMetadataValue):
             yield GrapheneJobMetadataEntry(
                 label=key,
                 jobName=value.job_name,
                 repositoryName=value.repository_name,
                 locationName=value.location_name,
             )
+        elif isinstance(value, CodeReferencesMetadataValue):
+            yield GrapheneCodeReferencesMetadataEntry(
+                label=key,
+                code_references=[
+                    GrapheneLocalFileCodeReference(
+                        filePath=reference.file_path,
+                        lineNumber=reference.line_number,
+                        label=reference.label,
+                    )
+                    for reference in value.code_references
+                ],
+            )
         elif isinstance(value, TableMetadataValue):
             yield GrapheneTableMetadataEntry(
                 label=key,
                 table=GrapheneTable(
                     schema=value.schema,
                     records=[seven.json.dumps(record.data) for record in value.records],
                 ),
```

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/execution/__init__.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/execution/backfill.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/execution/backfill.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
                 to_submit = to_submit[BACKFILL_CHUNK_SIZE:]
                 submitted_run_ids.extend(
                     run_id
                     for run_id in submit_backfill_runs(
                         graphene_info.context.instance,
                         create_workspace=lambda: graphene_info.context,
                         backfill_job=backfill,
-                        partition_names=chunk,
+                        partition_names_or_ranges=chunk,
                     )
                     if run_id is not None
                 )
             return GrapheneLaunchBackfillSuccess(
                 backfill_id=backfill_id, launched_run_ids=submitted_run_ids
             )
     elif asset_selection is not None:  # pure asset backfill
```

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/execution/dynamic_partitions.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/execution/dynamic_partitions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/execution/launch_execution.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/execution/launch_execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/execution/run_lifecycle.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/execution/run_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/external.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_asset_checks.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_asset_condition_evaluations.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_asset_condition_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_assets.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_assets.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     AbstractSet,
     Dict,
     Iterator,
     List,
     Mapping,
     Optional,
     Sequence,
+    Set,
     Tuple,
     Union,
     cast,
 )
 
 import dagster._seven as seven
 from dagster import (
@@ -196,15 +197,15 @@
                 )
             )
 
     return results
 
 
 def get_asset_nodes_by_asset_key(
-    graphene_info: "ResolveInfo", asset_keys: Optional[Sequence[AssetKey]] = None
+    graphene_info: "ResolveInfo", asset_keys: Optional[Set[AssetKey]] = None
 ) -> Mapping[AssetKey, "GrapheneAssetNode"]:
     """If multiple repositories have asset nodes for the same asset key, chooses the asset node that
     has an op.
     """
     from ..schema.asset_graph import GrapheneAssetNode
     from .asset_checks_loader import AssetChecksLoader
 
@@ -261,40 +262,40 @@
             if base_deployment_context is not None
             else None,
         )
         for repo_loc, repo, external_asset_node in asset_nodes_by_asset_key.values()
     }
 
 
-def get_asset_nodes(graphene_info: "ResolveInfo"):
-    return get_asset_nodes_by_asset_key(graphene_info).values()
+def get_asset_nodes(graphene_info: "ResolveInfo", asset_keys: Optional[Set[AssetKey]] = None):
+    return get_asset_nodes_by_asset_key(graphene_info, asset_keys=asset_keys).values()
 
 
 def get_asset_node(
     graphene_info: "ResolveInfo", asset_key: AssetKey
 ) -> Union["GrapheneAssetNode", "GrapheneAssetNotFoundError"]:
     from ..schema.errors import GrapheneAssetNotFoundError
 
     check.inst_param(asset_key, "asset_key", AssetKey)
-    node = get_asset_nodes_by_asset_key(graphene_info, asset_keys=[asset_key]).get(asset_key, None)
+    node = get_asset_nodes_by_asset_key(graphene_info, asset_keys={asset_key}).get(asset_key, None)
     if not node:
         return GrapheneAssetNotFoundError(asset_key=asset_key)
     return node
 
 
 def get_asset(
     graphene_info: "ResolveInfo", asset_key: AssetKey
 ) -> Union["GrapheneAsset", "GrapheneAssetNotFoundError"]:
     from ..schema.errors import GrapheneAssetNotFoundError
     from ..schema.pipelines.pipeline import GrapheneAsset
 
     check.inst_param(asset_key, "asset_key", AssetKey)
     instance = graphene_info.context.instance
 
-    asset_nodes_by_asset_key = get_asset_nodes_by_asset_key(graphene_info, asset_keys=[asset_key])
+    asset_nodes_by_asset_key = get_asset_nodes_by_asset_key(graphene_info, asset_keys={asset_key})
     asset_node = asset_nodes_by_asset_key.get(asset_key)
 
     if not asset_node and not instance.has_asset_key(asset_key):
         return GrapheneAssetNotFoundError(asset_key=asset_key)
 
     return GrapheneAsset(key=asset_key, definition=asset_node)
```

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_backfills.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_backfills.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_env_vars.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_instigators.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_instigators.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_logs.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_partition_sets.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_pipelines.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_pipelines.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_resources.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_runs.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_runs.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     instance = graphene_info.context.instance
 
     asset_keys = list(step_keys_by_asset.keys())
 
     if not asset_keys:
         return []
 
-    asset_nodes = get_asset_nodes_by_asset_key(graphene_info, asset_keys)
+    asset_nodes = get_asset_nodes_by_asset_key(graphene_info, set(asset_keys))
 
     asset_records = asset_record_loader.get_asset_records(asset_keys)
 
     latest_materialization_by_asset = {
         asset_record.asset_entry.asset_key: (
             GrapheneMaterializationEvent(event=asset_record.asset_entry.last_materialization)
             if asset_record.asset_entry.last_materialization
```

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_schedules.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_sensors.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_solids.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/fetch_ticks.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/fetch_ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/loader.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/run_config_schema.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/run_config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/telemetry.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/telemetry.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/implementation/utils.py` & `dagster-graphql-1.7.6/dagster_graphql/implementation/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/__init__.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/asset_checks.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/asset_checks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/asset_condition_evaluations.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/asset_condition_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/asset_graph.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/asset_graph.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/asset_selections.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/asset_selections.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/auto_materialize_asset_evaluations.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/auto_materialize_asset_evaluations.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/auto_materialize_policy.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/auto_materialize_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/backfill.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/backfill.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 from typing import TYPE_CHECKING, Optional, Sequence
 
 import dagster._check as check
 import graphene
 from dagster import AssetKey
 from dagster._core.definitions.backfill_policy import BackfillPolicy, BackfillPolicyType
 from dagster._core.definitions.partition import PartitionsSubset
+from dagster._core.definitions.partition_key_range import PartitionKeyRange
 from dagster._core.definitions.time_window_partitions import (
     BaseTimeWindowPartitionsSubset,
 )
 from dagster._core.execution.asset_backfill import (
     AssetBackfillStatus,
     PartitionedAssetBackfillStatus,
     UnpartitionedAssetBackfillStatus,
 )
 from dagster._core.execution.backfill import (
     BulkActionStatus,
     PartitionBackfill,
 )
+from dagster._core.instance import DagsterInstance
 from dagster._core.remote_representation.external import ExternalPartitionSet
-from dagster._core.storage.dagster_run import RunPartitionData, RunRecord, RunsFilter
-from dagster._core.storage.tags import BACKFILL_ID_TAG, TagType, get_tag_type
+from dagster._core.storage.dagster_run import DagsterRun, RunPartitionData, RunRecord, RunsFilter
+from dagster._core.storage.tags import (
+    ASSET_PARTITION_RANGE_END_TAG,
+    ASSET_PARTITION_RANGE_START_TAG,
+    TagType,
+    get_tag_type,
+)
 from dagster._core.workspace.permissions import Permissions
 
 from ..implementation.fetch_partition_sets import (
     partition_status_counts_from_run_partition_data,
     partition_statuses_from_run_partition_data,
 )
 from .asset_key import GrapheneAssetKey
@@ -326,26 +333,63 @@
             filters = RunsFilter.for_backfill(self._backfill_job.backfill_id)
             self._records = graphene_info.context.instance.get_run_records(
                 filters=filters,
             )
         return self._records
 
     def _get_partition_run_data(self, graphene_info: ResolveInfo) -> Sequence[RunPartitionData]:
-        if self._partition_run_data is None:
+        if self._partition_run_data is not None:
+            return self._partition_run_data
+
+        # Storage layer not equipped to calculate partition status for ranged job backfills so
+        # we perform the calculation ad hoc here.
+        partition_set = self._get_partition_set(graphene_info)
+        if (
+            partition_set
+            and partition_set.backfill_policy
+            and partition_set.backfill_policy.max_partitions_per_run != 1
+        ):  # ranged backfills
+            self._partition_run_data = self._get_partition_run_data_for_ranged_job_backfill(
+                graphene_info.context.instance, partition_set
+            )
+        else:
             self._partition_run_data = (
                 graphene_info.context.instance.run_storage.get_run_partition_data(
                     runs_filter=RunsFilter(
-                        tags={
-                            BACKFILL_ID_TAG: self._backfill_job.backfill_id,
-                        }
+                        tags=DagsterRun.tags_for_backfill_id(self._backfill_job.backfill_id)
                     )
                 )
             )
         return self._partition_run_data
 
+    def _get_partition_run_data_for_ranged_job_backfill(
+        self, instance: DagsterInstance, partition_set: ExternalPartitionSet
+    ) -> Sequence[RunPartitionData]:
+        partitions_def = partition_set.get_partitions_definition()
+        records = instance.get_run_records(
+            RunsFilter(tags=DagsterRun.tags_for_backfill_id(self._backfill_job.backfill_id))
+        )
+        return [
+            RunPartitionData(
+                run_id=record.dagster_run.run_id,
+                partition=key,
+                status=record.dagster_run.status,
+                start_time=record.start_time,
+                end_time=record.end_time,
+            )
+            for record in records
+            for key in partitions_def.get_partition_keys_in_range(
+                PartitionKeyRange(
+                    start=record.dagster_run.tags[ASSET_PARTITION_RANGE_START_TAG],
+                    end=record.dagster_run.tags[ASSET_PARTITION_RANGE_END_TAG],
+                ),
+                instance,
+            )
+        ]
+
     def resolve_unfinishedRuns(self, graphene_info: ResolveInfo) -> Sequence["GrapheneRun"]:
         from .pipelines.pipeline import GrapheneRun
 
         records = self._get_records(graphene_info)
         return [GrapheneRun(record) for record in records if not record.dagster_run.is_finished]
 
     def resolve_runs(self, graphene_info: ResolveInfo) -> "Sequence[GrapheneRun]":
@@ -418,20 +462,20 @@
         self, graphene_info: ResolveInfo
     ) -> Sequence["GraphenePartitionStatusCounts"]:
         # This resolver is only enabled for job backfills, since it assumes a unique run per
         # partition key (which is not true for asset backfills). Asset backfills should rely on
         # the assetBackfillData resolver instead.
         if self._backfill_job.is_asset_backfill:
             return []
-
-        partition_run_data = self._get_partition_run_data(graphene_info)
-        return partition_status_counts_from_run_partition_data(
-            partition_run_data,
-            check.not_none(self._backfill_job.get_partition_names(graphene_info.context)),
-        )
+        else:
+            partition_run_data = self._get_partition_run_data(graphene_info)
+            return partition_status_counts_from_run_partition_data(
+                partition_run_data,
+                check.not_none(self._backfill_job.get_partition_names(graphene_info.context)),
+            )
 
     def resolve_isAssetBackfill(self, _graphene_info: ResolveInfo) -> bool:
         return self._backfill_job.is_asset_backfill
 
     def resolve_partitionsTargetedForAssetKey(
         self, graphene_info: ResolveInfo, asset_key
     ) -> Optional[PartitionsSubset]:
```

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/config_type_or_error.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/config_type_or_error.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/config_types.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/config_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/dagster_types.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/dagster_types.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/env_vars.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/env_vars.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/errors.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/execution.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/execution.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/external.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/external.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/freshness_policy.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/freshness_policy.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/inputs.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/inputs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/instance.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/instance.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/instigation.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/instigation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/logs/__init__.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/logs/compute_logs.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/logs/compute_logs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/logs/events.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/logs/events.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/logs/log_level.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/logs/log_level.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/metadata.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -158,14 +158,37 @@
     locationName = graphene.NonNull(graphene.String)
 
     class Meta:
         interfaces = (GrapheneMetadataEntry,)
         name = "JobMetadataEntry"
 
 
+class GrapheneLocalFileCodeReference(graphene.ObjectType):
+    filePath = graphene.NonNull(graphene.String)
+    lineNumber = graphene.NonNull(graphene.Int)
+    label = graphene.String()
+
+    class Meta:
+        name = "LocalFileCodeReference"
+
+
+class GrapheneSourceLocation(graphene.Union):
+    class Meta:
+        types = (GrapheneLocalFileCodeReference,)
+        name = "SourceLocation"
+
+
+class GrapheneCodeReferencesMetadataEntry(graphene.ObjectType):
+    code_references = non_null_list(GrapheneSourceLocation)
+
+    class Meta:
+        interfaces = (GrapheneMetadataEntry,)
+        name = "CodeReferencesMetadataEntry"
+
+
 class GrapheneNullMetadataEntry(graphene.ObjectType):
     class Meta:
         interfaces = (GrapheneMetadataEntry,)
         name = "NullMetadataEntry"
 
 
 class GrapheneTimestampMetadataEntry(graphene.ObjectType):
@@ -192,10 +215,11 @@
         GrapheneNotebookMetadataEntry,
         GraphenePythonArtifactMetadataEntry,
         GrapheneTextMetadataEntry,
         GrapheneUrlMetadataEntry,
         GraphenePipelineRunMetadataEntry,
         GrapheneAssetMetadataEntry,
         GrapheneJobMetadataEntry,
+        GrapheneCodeReferencesMetadataEntry,
         GrapheneNullMetadataEntry,
         GrapheneTimestampMetadataEntry,
     ]
```

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/partition_mappings.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/partition_mappings.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/partition_sets.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/partition_sets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/permissions.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/permissions.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/__init__.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/config.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/config_result.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/config_result.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/logger.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/logger.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/mode.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/mode.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/pipeline.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/pipeline_ref.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/pipeline_ref.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/pipeline_run_stats.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/pipeline_run_stats.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/resource.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/resource.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/snapshot.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/snapshot.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/status.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/status.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/pipelines/subscription.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/pipelines/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/repository_origin.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/repository_origin.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/resources.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/roots/__init__.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/roots/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/roots/assets.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/roots/assets.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/roots/execution_plan.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/roots/execution_plan.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/roots/mutation.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/roots/mutation.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/roots/pipeline.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/roots/pipeline.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/roots/query.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/roots/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -934,15 +934,17 @@
                     )
                     for asset_node in external_asset_nodes
                 ]
                 if external_asset_nodes
                 else []
             )
         else:
-            results = get_asset_nodes(graphene_info)
+            results = get_asset_nodes(
+                graphene_info, resolved_asset_keys if not use_all_asset_keys else None
+            )
 
         # Filter down to requested asset keys
         results = [
             node
             for node in results
             if use_all_asset_keys or node.assetKey in check.not_none(resolved_asset_keys)
         ]
@@ -1070,15 +1072,15 @@
         return graphene_info.context.has_permission(Permissions.TERMINATE_PIPELINE_EXECUTION)
 
     def resolve_assetsLatestInfo(
         self, graphene_info: ResolveInfo, assetKeys: Sequence[GrapheneAssetKeyInput]
     ):
         asset_keys = set(AssetKey.from_graphql_input(asset_key) for asset_key in assetKeys)
 
-        results = get_asset_nodes(graphene_info)
+        results = get_asset_nodes(graphene_info, asset_keys)
 
         # Filter down to requested asset keys
         # Build mapping of asset key to the step keys required to generate the asset
         step_keys_by_asset: Dict[AssetKey, Sequence[str]] = {
             node.external_asset_node.asset_key: node.external_asset_node.op_names
             for node in results
             if node.assetKey in asset_keys
```

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/roots/subscription.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/roots/subscription.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/run_config.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/run_config.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/runs.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/runs.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/schedule_dry_run.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/schedule_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/schedules/__init__.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/schedules/schedules.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/schedules/schedules.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/schedules/ticks.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/schedules/ticks.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/sensor_dry_run.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/sensor_dry_run.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/sensors.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/sensors.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/solids.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/solids.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/table.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/table.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/tags.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/tags.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/test.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/test.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/used_solid.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/used_solid.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/schema/util.py` & `dagster-graphql-1.7.6/dagster_graphql/schema/util.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql/test/utils.py` & `dagster-graphql-1.7.6/dagster_graphql/test/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/dagster_graphql.egg-info/PKG-INFO` & `dagster-graphql-1.7.6/dagster_graphql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-graphql
-Version: 1.7.5
+Version: 1.7.6
 Summary: The GraphQL frontend to python dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/dagster-graphql
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-graphql-1.7.5/dagster_graphql.egg-info/SOURCES.txt` & `dagster-graphql-1.7.6/dagster_graphql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-graphql-1.7.5/setup.py` & `dagster-graphql-1.7.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_graphql_tests*"]),
     include_package_data=True,
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.5",
+        "dagster==1.7.6",
         "graphene>=3,<4",
         "gql[requests]>=3,<4",
         "requests",
         "starlette",  # used for run_in_threadpool utility fn
     ],
     entry_points={"console_scripts": ["dagster-graphql = dagster_graphql.cli:main"]},
 )
```

