# Comparing `tmp/dagster-cloud-1.7.5.tar.gz` & `tmp/dagster-cloud-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-1.7.5.tar", last modified: Thu May  9 17:58:27 2024, max compression
+gzip compressed data, was "dagster-cloud-1.7.6.tar", last modified: Thu May 16 20:18:25 2024, max compression
```

## Comparing `dagster-cloud-1.7.5.tar` & `dagster-cloud-1.7.6.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.536201 dagster-cloud-1.7.5/
--rw-r--r--   0 root         (0) root         (0)     4562 2024-05-09 17:58:27.536201 dagster-cloud-1.7.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3062 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.464201 dagster-cloud-1.7.5/dagster_cloud/
--rw-r--r--   0 root         (0) root         (0)      316 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.468201 dagster-cloud-1.7.5/dagster_cloud/agent/
--rw-r--r--   0 root         (0) root         (0)      826 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/agent/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.468201 dagster-cloud-1.7.5/dagster_cloud/agent/cli/
--rw-r--r--   0 root         (0) root         (0)     7584 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/agent/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45896 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/agent/dagster_cloud_agent.py
--rw-r--r--   0 root         (0) root         (0)     1837 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/agent/queries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.468201 dagster-cloud-1.7.5/dagster_cloud/anomaly_detection/
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/anomaly_detection/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9443 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/anomaly_detection/defs.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/anomaly_detection/mutation.py
--rw-r--r--   0 root         (0) root         (0)     2245 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/anomaly_detection/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.468201 dagster-cloud-1.7.5/dagster_cloud/api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19251 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/api/dagster_cloud_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.476201 dagster-cloud-1.7.5/dagster_cloud/artifacts/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/artifacts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.476201 dagster-cloud-1.7.5/dagster_cloud/auth/
--rw-r--r--   0 root         (0) root         (0)      248 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1242 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/auth/constants.py
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.476201 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/
--rw-r--r--   0 root         (0) root         (0)     1873 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.480201 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/__init__.py
--rw-r--r--   0 root         (0) root         (0)      816 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py
--rw-r--r--   0 root         (0) root         (0)     7964 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     3234 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py
--rw-r--r--   0 root         (0) root         (0)      138 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/errors.py
--rw-r--r--   0 root         (0) root         (0)     2524 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/insights_utils.py
--rw-r--r--   0 root         (0) root         (0)     4194 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/metrics_utils.py
--rw-r--r--   0 root         (0) root         (0)     1403 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.484201 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5611 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py
--rw-r--r--   0 root         (0) root         (0)     5185 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py
--rw-r--r--   0 root         (0) root         (0)     7254 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/definitions.py
--rw-r--r--   0 root         (0) root         (0)    10624 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py
--rw-r--r--   0 root         (0) root         (0)     3808 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.484201 dagster-cloud-1.7.5/dagster_cloud/execution/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.484201 dagster-cloud-1.7.5/dagster_cloud/execution/cloud_run_launcher/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/execution/cloud_run_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/execution/cloud_run_launcher/k8s.py
--rw-r--r--   0 root         (0) root         (0)     3215 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/execution/cloud_run_launcher/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.484201 dagster-cloud-1.7.5/dagster_cloud/execution/monitoring/
--rw-r--r--   0 root         (0) root         (0)    17294 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/execution/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.488201 dagster-cloud-1.7.5/dagster_cloud/execution/utils/
--rw-r--r--   0 root         (0) root         (0)      254 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/execution/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/execution/utils/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.488201 dagster-cloud-1.7.5/dagster_cloud/instance/
--rw-r--r--   0 root         (0) root         (0)    22345 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/instance/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.488201 dagster-cloud-1.7.5/dagster_cloud/pex/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.492201 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.496201 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/__generated__/
--rw-r--r--   0 root         (0) root         (0)      285 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/__generated__/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3907 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9301 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      327 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5251 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/client.py
--rw-r--r--   0 root         (0) root         (0)     3790 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/compile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.496201 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/
--rw-r--r--   0 root         (0) root         (0)      119 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.500201 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/cli/
--rw-r--r--   0 root         (0) root         (0)     2115 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17844 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/manager.py
--rw-r--r--   0 root         (0) root         (0)    12797 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/registry.py
--rw-r--r--   0 root         (0) root         (0)    15703 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/server.py
--rw-r--r--   0 root         (0) root         (0)     3322 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/pex/grpc/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.500201 dagster-cloud-1.7.5/dagster_cloud/secrets/
--rw-r--r--   0 root         (0) root         (0)       75 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/secrets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1620 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/secrets/loader.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.504201 dagster-cloud-1.7.5/dagster_cloud/serverless/
--rw-r--r--   0 root         (0) root         (0)       71 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/serverless/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4247 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/serverless/io_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.504201 dagster-cloud-1.7.5/dagster_cloud/storage/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1690 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.504201 dagster-cloud-1.7.5/dagster_cloud/storage/compute_logs/
--rw-r--r--   0 root         (0) root         (0)       82 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/compute_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4753 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/compute_logs/compute_log_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.508201 dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16377 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/queries.py
--rw-r--r--   0 root         (0) root         (0)    46580 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/storage.py
--rw-r--r--   0 root         (0) root         (0)      658 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.512201 dagster-cloud-1.7.5/dagster_cloud/storage/runs/
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/runs/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6446 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/runs/queries.py
--rw-r--r--   0 root         (0) root         (0)    18839 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/runs/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.512201 dagster-cloud-1.7.5/dagster_cloud/storage/schedules/
--rw-r--r--   0 root         (0) root         (0)       70 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/schedules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1930 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/schedules/queries.py
--rw-r--r--   0 root         (0) root         (0)     7585 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/schedules/storage.py
--rw-r--r--   0 root         (0) root         (0)      502 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/storage/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.516201 dagster-cloud-1.7.5/dagster_cloud/util/
--rw-r--r--   0 root         (0) root         (0)     2778 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4693 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/util/container_resources.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.516201 dagster-cloud-1.7.5/dagster_cloud/workspace/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.520201 dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/
--rw-r--r--   0 root         (0) root         (0)    10918 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/__init__.py
--rw-r--r--   0 root         (0) root         (0)      967 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/docker.py
--rw-r--r--   0 root         (0) root         (0)     6575 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/ecs.py
--rw-r--r--   0 root         (0) root         (0)     5319 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/kubernetes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.524201 dagster-cloud-1.7.5/dagster_cloud/workspace/docker/
--rw-r--r--   0 root         (0) root         (0)    12977 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      352 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/docker/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.528201 dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28818 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/client.py
--rw-r--r--   0 root         (0) root         (0)    28623 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/launcher.py
--rw-r--r--   0 root         (0) root         (0)      534 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/run_launcher.py
--rw-r--r--   0 root         (0) root         (0)     4126 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/service.py
--rw-r--r--   0 root         (0) root         (0)     2746 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.528201 dagster-cloud-1.7.5/dagster_cloud/workspace/kubernetes/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/kubernetes/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26248 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/kubernetes/launcher.py
--rw-r--r--   0 root         (0) root         (0)     9825 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/kubernetes/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.536201 dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/
--rw-r--r--   0 root         (0) root         (0)      745 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14248 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/process.py
--rw-r--r--   0 root         (0) root         (0)    83997 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
--rw-r--r--   0 root         (0) root         (0)     1209 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:27.464201 dagster-cloud-1.7.5/dagster_cloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4562 2024-05-09 17:58:27.000000 dagster-cloud-1.7.5/dagster_cloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4240 2024-05-09 17:58:27.000000 dagster-cloud-1.7.5/dagster_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:58:27.000000 dagster-cloud-1.7.5/dagster_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      509 2024-05-09 17:58:27.000000 dagster-cloud-1.7.5/dagster_cloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-09 17:58:27.000000 dagster-cloud-1.7.5/dagster_cloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 17:58:27.536201 dagster-cloud-1.7.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3078 2024-05-09 17:47:54.000000 dagster-cloud-1.7.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.552893 dagster-cloud-1.7.6/
+-rw-r--r--   0 root         (0) root         (0)     4562 2024-05-16 20:18:25.552893 dagster-cloud-1.7.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3062 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.464893 dagster-cloud-1.7.6/dagster_cloud/
+-rw-r--r--   0 root         (0) root         (0)      316 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.468893 dagster-cloud-1.7.6/dagster_cloud/agent/
+-rw-r--r--   0 root         (0) root         (0)      826 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/agent/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.468893 dagster-cloud-1.7.6/dagster_cloud/agent/cli/
+-rw-r--r--   0 root         (0) root         (0)     7584 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/agent/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45896 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/agent/dagster_cloud_agent.py
+-rw-r--r--   0 root         (0) root         (0)     1837 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/agent/queries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.468893 dagster-cloud-1.7.6/dagster_cloud/anomaly_detection/
+-rw-r--r--   0 root         (0) root         (0)      279 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/anomaly_detection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9443 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/anomaly_detection/defs.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/anomaly_detection/mutation.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/anomaly_detection/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.468893 dagster-cloud-1.7.6/dagster_cloud/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19251 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/api/dagster_cloud_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.468893 dagster-cloud-1.7.6/dagster_cloud/artifacts/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/artifacts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.476893 dagster-cloud-1.7.6/dagster_cloud/auth/
+-rw-r--r--   0 root         (0) root         (0)      248 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/auth/constants.py
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.476893 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/
+-rw-r--r--   0 root         (0) root         (0)     1873 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.476893 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      816 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py
+-rw-r--r--   0 root         (0) root         (0)     7964 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     3234 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py
+-rw-r--r--   0 root         (0) root         (0)      138 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/errors.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/insights_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4194 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/metrics_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1403 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.476893 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5611 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py
+-rw-r--r--   0 root         (0) root         (0)     5185 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py
+-rw-r--r--   0 root         (0) root         (0)     7254 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/definitions.py
+-rw-r--r--   0 root         (0) root         (0)    10624 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.480893 dagster-cloud-1.7.6/dagster_cloud/execution/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.480893 dagster-cloud-1.7.6/dagster_cloud/execution/cloud_run_launcher/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/execution/cloud_run_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/execution/cloud_run_launcher/k8s.py
+-rw-r--r--   0 root         (0) root         (0)     3215 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/execution/cloud_run_launcher/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.480893 dagster-cloud-1.7.6/dagster_cloud/execution/monitoring/
+-rw-r--r--   0 root         (0) root         (0)    17294 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/execution/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.484893 dagster-cloud-1.7.6/dagster_cloud/execution/utils/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/execution/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/execution/utils/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.484893 dagster-cloud-1.7.6/dagster_cloud/instance/
+-rw-r--r--   0 root         (0) root         (0)    22345 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/instance/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.484893 dagster-cloud-1.7.6/dagster_cloud/pex/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.488893 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.488893 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/__generated__/
+-rw-r--r--   0 root         (0) root         (0)      285 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/__generated__/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3907 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9301 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5251 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/client.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/compile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.492893 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/
+-rw-r--r--   0 root         (0) root         (0)      119 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.492893 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/cli/
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17844 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/manager.py
+-rw-r--r--   0 root         (0) root         (0)    12797 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/registry.py
+-rw-r--r--   0 root         (0) root         (0)    15703 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     3322 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/pex/grpc/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.496893 dagster-cloud-1.7.6/dagster_cloud/secrets/
+-rw-r--r--   0 root         (0) root         (0)       75 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/secrets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/secrets/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.496893 dagster-cloud-1.7.6/dagster_cloud/serverless/
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/serverless/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4247 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/serverless/io_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.500893 dagster-cloud-1.7.6/dagster_cloud/storage/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.500893 dagster-cloud-1.7.6/dagster_cloud/storage/compute_logs/
+-rw-r--r--   0 root         (0) root         (0)       82 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/compute_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4753 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/compute_logs/compute_log_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.516893 dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16377 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    46580 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/storage.py
+-rw-r--r--   0 root         (0) root         (0)      640 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.524893 dagster-cloud-1.7.6/dagster_cloud/storage/runs/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/runs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6742 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/runs/queries.py
+-rw-r--r--   0 root         (0) root         (0)    19554 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/runs/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.524893 dagster-cloud-1.7.6/dagster_cloud/storage/schedules/
+-rw-r--r--   0 root         (0) root         (0)       70 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/schedules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/schedules/queries.py
+-rw-r--r--   0 root         (0) root         (0)     7585 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/schedules/storage.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/storage/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.528893 dagster-cloud-1.7.6/dagster_cloud/util/
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/util/container_resources.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.528893 dagster-cloud-1.7.6/dagster_cloud/workspace/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.532893 dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/
+-rw-r--r--   0 root         (0) root         (0)    10918 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      967 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/docker.py
+-rw-r--r--   0 root         (0) root         (0)     6575 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/ecs.py
+-rw-r--r--   0 root         (0) root         (0)     5319 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/kubernetes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.532893 dagster-cloud-1.7.6/dagster_cloud/workspace/docker/
+-rw-r--r--   0 root         (0) root         (0)    12989 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      352 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/docker/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.540893 dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28867 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/client.py
+-rw-r--r--   0 root         (0) root         (0)    28823 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/launcher.py
+-rw-r--r--   0 root         (0) root         (0)      534 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/run_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     4126 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/service.py
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.544893 dagster-cloud-1.7.6/dagster_cloud/workspace/kubernetes/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/kubernetes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26266 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/kubernetes/launcher.py
+-rw-r--r--   0 root         (0) root         (0)     9855 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/kubernetes/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.552893 dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/
+-rw-r--r--   0 root         (0) root         (0)      745 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14260 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/process.py
+-rw-r--r--   0 root         (0) root         (0)    85944 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-05-16 20:06:42.000000 dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:25.468893 dagster-cloud-1.7.6/dagster_cloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4562 2024-05-16 20:18:25.000000 dagster-cloud-1.7.6/dagster_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4240 2024-05-16 20:18:25.000000 dagster-cloud-1.7.6/dagster_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:18:25.000000 dagster-cloud-1.7.6/dagster_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      504 2024-05-16 20:18:25.000000 dagster-cloud-1.7.6/dagster_cloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-16 20:18:25.000000 dagster-cloud-1.7.6/dagster_cloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 20:18:25.552893 dagster-cloud-1.7.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3073 2024-05-16 20:06:43.000000 dagster-cloud-1.7.6/setup.py
```

### Comparing `dagster-cloud-1.7.5/PKG-INFO` & `dagster-cloud-1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.7.5
+Version: 1.7.6
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster-cloud-1.7.5/README.md` & `dagster-cloud-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/agent/__init__.py` & `dagster-cloud-1.7.6/dagster_cloud/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/agent/cli/__init__.py` & `dagster-cloud-1.7.6/dagster_cloud/agent/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/agent/dagster_cloud_agent.py` & `dagster-cloud-1.7.6/dagster_cloud/agent/dagster_cloud_agent.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/agent/queries.py` & `dagster-cloud-1.7.6/dagster_cloud/agent/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/anomaly_detection/defs.py` & `dagster-cloud-1.7.6/dagster_cloud/anomaly_detection/defs.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/anomaly_detection/types.py` & `dagster-cloud-1.7.6/dagster_cloud/anomaly_detection/types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/api/dagster_cloud_api.py` & `dagster-cloud-1.7.6/dagster_cloud/api/dagster_cloud_api.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/auth/constants.py` & `dagster-cloud-1.7.6/dagster_cloud/auth/constants.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/__init__.py` & `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py` & `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/bigquery_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py` & `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/dbt_wrapper.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py` & `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/bigquery/insights_bigquery_resource.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/insights_utils.py` & `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/insights_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/metrics_utils.py` & `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/query.py` & `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/query.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py` & `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/dagster_snowflake_insights.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py` & `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/dbt_wrapper.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/definitions.py` & `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/definitions.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py` & `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/insights_snowflake_resource.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py` & `dagster-cloud-1.7.6/dagster_cloud/dagster_insights/snowflake/snowflake_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/execution/cloud_run_launcher/process.py` & `dagster-cloud-1.7.6/dagster_cloud/execution/cloud_run_launcher/process.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/execution/monitoring/__init__.py` & `dagster-cloud-1.7.6/dagster_cloud/execution/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/execution/utils/process.py` & `dagster-cloud-1.7.6/dagster_cloud/execution/utils/process.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/instance/__init__.py` & `dagster-cloud-1.7.6/dagster_cloud/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py` & `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py` & `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/__generated__/multi_pex_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/client.py` & `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/compile.py` & `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/compile.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/cli/__init__.py` & `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/manager.py` & `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/manager.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/registry.py` & `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/registry.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/server/server.py` & `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/server/server.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/pex/grpc/types.py` & `dagster-cloud-1.7.6/dagster_cloud/pex/grpc/types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/secrets/loader.py` & `dagster-cloud-1.7.6/dagster_cloud/secrets/loader.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/serverless/io_manager.py` & `dagster-cloud-1.7.6/dagster_cloud/serverless/io_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/storage/client.py` & `dagster-cloud-1.7.6/dagster_cloud/storage/client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/storage/compute_logs/compute_log_manager.py` & `dagster-cloud-1.7.6/dagster_cloud/storage/compute_logs/compute_log_manager.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/queries.py` & `dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/storage.py` & `dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/storage/event_logs/utils.py` & `dagster-cloud-1.7.6/dagster_cloud/storage/event_logs/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 def truncate_event(
     event: EventLogEntry, maximum_length=MAXIMUM_EVENT_MESSAGE_CHARACTERS
 ) -> EventLogEntry:
     if len(event.user_message) > maximum_length:
         return event._replace(
             user_message=(
                 f"[TRUNCATED from {len(event.user_message)} characters to"
-                f" {MAXIMUM_EVENT_MESSAGE_CHARACTERS}]"
+                f" {maximum_length}]"
                 f" {event.user_message[:maximum_length]} [TRUNCATED]"
             ),
         )
 
     return event
```

### Comparing `dagster-cloud-1.7.5/dagster_cloud/storage/runs/queries.py` & `dagster-cloud-1.7.6/dagster_cloud/storage/runs/queries.py`

 * *Files 3% similar despite different names*

```diff
@@ -211,14 +211,24 @@
     query getDaemonHeartbeatsQuery {
         runs {
             getDaemonHeartbeats
         }
     }
 """
 
+ADD_RUN_TELEMETRY_MUTATION = """
+    mutation addRunTelemetry($serializedTelemetry: String!, $serializedTags: String!) {
+        runs {
+            addRunTelemetry(serializedTelemetry: $serializedTelemetry, serializedTags: $serializedTags) {
+                ok
+            }
+        }
+    }
+"""
+
 GET_BACKFILLS_QUERY = """
     query getBackfillsQuery($status: String, $cursor: String, $limit: Int) {
         runs {
             getBackfills(status: $status, cursor: $cursor, limit: $limit)
         }
     }
 """
```

### Comparing `dagster-cloud-1.7.5/dagster_cloud/storage/runs/storage.py` & `dagster-cloud-1.7.6/dagster_cloud/storage/runs/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     DagsterInvariantViolationError,
     DagsterRunAlreadyExists,
     DagsterRunNotFoundError,
     DagsterSnapshotDoesNotExist,
 )
 from dagster._core.events import DagsterEvent
 from dagster._core.execution.backfill import BulkActionStatus, PartitionBackfill
+from dagster._core.execution.types import RunTelemetryData
 from dagster._core.remote_representation.origin import RemoteJobOrigin
 from dagster._core.snap import (
     ExecutionPlanSnapshot,
     JobSnapshot,
     create_execution_plan_snapshot_id,
     create_job_snapshot_id,
 )
@@ -53,14 +54,15 @@
 from .queries import (
     ADD_BACKFILL_MUTATION,
     ADD_DAEMON_HEARTBEAT_MUTATION,
     ADD_EXECUTION_PLAN_SNAPSHOT_MUTATION,
     ADD_PIPELINE_SNAPSHOT_MUTATION,
     ADD_RUN_MUTATION,
     ADD_RUN_TAGS_MUTATION,
+    ADD_RUN_TELEMETRY_MUTATION,
     GET_BACKFILL_QUERY,
     GET_BACKFILLS_QUERY,
     GET_DAEMON_HEARTBEATS_QUERY,
     GET_EXECUTION_PLAN_SNAPSHOT_QUERY,
     GET_PIPELINE_SNAPSHOT_QUERY,
     GET_RUN_BY_ID_QUERY,
     GET_RUN_GROUP_QUERY,
@@ -435,14 +437,34 @@
             variables={
                 "serializedDaemonHeartbeat": serialize_value(
                     check.inst_param(daemon_heartbeat, "daemon_heartbeat", DaemonHeartbeat)
                 )
             },
         )
 
+    def add_run_telemetry(
+        self,
+        run_telemetry: RunTelemetryData,
+        tags: Optional[Dict[str, str]] = None,
+    ) -> None:
+        if tags is None:
+            tags = {}
+
+        self._execute_query(
+            ADD_RUN_TELEMETRY_MUTATION,
+            variables={
+                "serializedTelemetry": serialize_value(
+                    check.inst_param(run_telemetry, "run_telemetry", RunTelemetryData)
+                ),
+                "serializedTags": serialize_value(
+                    check.dict_param(tags, "tags", key_type=str, value_type=str)
+                ),
+            },
+        )
+
     def build_missing_indexes(
         self, print_fn: Callable = lambda _: None, force_rebuild_all: bool = False
     ):
         raise Exception("Not allowed to build indexes from user cloud")
 
     def get_daemon_heartbeats(self) -> Dict[str, DaemonHeartbeat]:
         res = self._execute_query(GET_DAEMON_HEARTBEATS_QUERY)
```

### Comparing `dagster-cloud-1.7.5/dagster_cloud/storage/schedules/queries.py` & `dagster-cloud-1.7.6/dagster_cloud/storage/schedules/queries.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/storage/schedules/storage.py` & `dagster-cloud-1.7.6/dagster_cloud/storage/schedules/storage.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/util/__init__.py` & `dagster-cloud-1.7.6/dagster_cloud/util/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/util/container_resources.py` & `dagster-cloud-1.7.6/dagster_cloud/util/container_resources.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/__init__.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/docker.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/docker.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/ecs.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/ecs.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/config_schema/kubernetes.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/config_schema/kubernetes.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/docker/__init__.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/docker/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,23 +327,23 @@
             labels=labels,
         )
 
         return DagsterCloudGrpcServer(
             DagsterDockerContainer(container=container), server_endpoint, metadata
         )
 
-    def _wait_for_new_server_ready(
+    async def _wait_for_new_server_ready(
         self,
         deployment_name: str,
         location_name: str,
         user_code_launcher_entry: UserCodeLauncherEntry,
         server_handle: DagsterDockerContainer,
         server_endpoint: ServerEndpoint,
     ) -> None:
-        self._wait_for_dagster_server_process(
+        await self._wait_for_dagster_server_process(
             client=server_endpoint.create_client(),
             timeout=self._server_process_startup_timeout,
         )
 
     def _remove_server_handle(self, server_handle: DagsterDockerContainer) -> None:
         container = server_handle.container
         try:
```

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/client.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import json
 import logging
 import time
 from typing import List, Optional
 
 import boto3
 import botocore
@@ -515,25 +516,25 @@
                 for key, value in tags.items()
             ]
 
         arn = self.ecs.create_service(**params).get("service").get("serviceArn")
 
         return Service(client=self, arn=arn)
 
-    def wait_for_new_service(self, service, container_name, logger=None) -> dict:
+    async def wait_for_new_service(self, service, container_name, logger=None) -> str:
         logger = logger or logging.getLogger("dagster_cloud.EcsClient")
         service_name = service.name
         start_time = time.time()
         while True:
             response = self.ecs.describe_services(
                 cluster=self.cluster_name,
                 services=[service_name],
             )
             if response.get("services"):
-                running_tasks = self.check_service_has_running_tasks(
+                running_tasks = await self.check_service_has_running_tasks(
                     service_name, container_name, logger=logger
                 )
                 return running_tasks[0]
 
             failures = response.get("failures")
 
             if not failures:
@@ -548,15 +549,15 @@
             # Even if we fail, check a few more times in case it's just the ECS API
             # being eventually consistent
             if time.time() - start_time >= self.grace_period:
                 raise Exception(
                     f"ECS DescribeServices API returned failures: {json.dumps(failures)}"
                 )
 
-            time.sleep(10)
+            await asyncio.sleep(10)
 
     def _raise_failed_task(self, task, container_name, logger):
         task_arn = task["taskArn"]
         stopped_reason = task["stoppedReason"]
 
         logs = None
 
@@ -576,17 +577,17 @@
     def assert_task_not_stopped(self, task_arn, container_name, logger=None):
         logger = logger or logging.getLogger("dagster_cloud.EcsClient")
 
         task = self.ecs.describe_tasks(cluster=self.cluster_name, tasks=[task_arn]).get("tasks")[0]
         if task.get("lastStatus") == "STOPPED":
             self._raise_failed_task(task, container_name, logger)
 
-    def check_service_has_running_tasks(
+    async def check_service_has_running_tasks(
         self, service_name, container_name, logger=None
-    ) -> List[dict]:
+    ) -> List[str]:
         # return the ARN of the task if it starts
         logger = logger or logging.getLogger("dagster_cloud.EcsClient")
         start_time = time.time()
 
         tasks_to_track = None
 
         while start_time + self.timeout > time.time():
@@ -638,15 +639,15 @@
                             all_tasks_running = False
                     elif task.get("lastStatus") == "STOPPED":
                         self._raise_failed_task(task, container_name, logger)
 
                 if all_tasks_running:
                     return tasks_to_track
 
-            time.sleep(20)
+            await asyncio.sleep(20)
 
         # Fetch the service event logs to try to get some clue about why the service never spun
         # up any tasks
         service_events_str = ""
         try:
             response = self.ecs.describe_services(
                 cluster=self.cluster_name,
```

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/launcher.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import os
 from pathlib import Path
 from typing import Any, Collection, Dict, List, Mapping, Optional, Sequence, cast
 
 import boto3
 import grpc
 from dagster import (
@@ -39,15 +40,18 @@
 from dagster_cloud.workspace.user_code_launcher import (
     DEFAULT_SERVER_PROCESS_STARTUP_TIMEOUT,
     SHARED_USER_CODE_LAUNCHER_CONFIG,
     DagsterCloudGrpcServer,
     DagsterCloudUserCodeLauncher,
     ServerEndpoint,
 )
-from dagster_cloud.workspace.user_code_launcher.user_code_launcher import UserCodeLauncherEntry
+from dagster_cloud.workspace.user_code_launcher.user_code_launcher import (
+    UserCodeLauncherEntry,
+    async_serialize_exceptions,
+)
 from dagster_cloud.workspace.user_code_launcher.utils import deterministic_label_for_location
 
 from .client import get_debug_ecs_prompt
 from .run_launcher import CloudEcsRunLauncher
 from .utils import get_server_task_definition_family
 
 EcsServerHandleType = Service
@@ -478,33 +482,38 @@
         return DagsterCloudGrpcServer(service, endpoint, metadata)
 
     def _check_running_multipex_server(self, multipex_server: DagsterCloudGrpcServer):
         self._logger.info(
             f"Checking whether service {multipex_server.server_handle.name} is ready for existing"
             " multipex server..."
         )
-        self.client.check_service_has_running_tasks(
-            multipex_server.server_handle.name, container_name=CONTAINER_NAME, logger=self._logger
+        asyncio.run(
+            self.client.check_service_has_running_tasks(
+                multipex_server.server_handle.name,
+                container_name=CONTAINER_NAME,
+                logger=self._logger,
+            )
         )
         super()._check_running_multipex_server(multipex_server)
 
-    def _wait_for_new_multipex_server(
+    @async_serialize_exceptions
+    async def _wait_for_new_multipex_server(
         self,
         _deployment_name: str,
         _location_name: str,
         server_handle: Service,
         multipex_endpoint: ServerEndpoint,
     ):
         self._logger.info(
             f"Waiting for service {server_handle.name} to be ready for multipex server..."
         )
-        task_arn = self.client.wait_for_new_service(
+        task_arn = await self.client.wait_for_new_service(
             server_handle, container_name=CONTAINER_NAME, logger=self._logger
         )
-        self._wait_for_server_process(
+        await self._wait_for_server_process(
             multipex_endpoint.create_multipex_client(),
             timeout=self._server_process_startup_timeout,
             additional_check=lambda: self.client.assert_task_not_stopped(
                 task_arn, CONTAINER_NAME, self._logger
             ),
         )
 
@@ -522,27 +531,27 @@
             self._logger.exception("Error trying to get logs for failed task", task_arn=task_arn)
 
         if self.show_debug_cluster_info:
             sections.append(get_debug_ecs_prompt(self.cluster, task_arn))
 
         return "\n\n".join(sections)
 
-    def _wait_for_new_server_ready(
+    async def _wait_for_new_server_ready(
         self,
         deployment_name: str,
         location_name: str,
         user_code_launcher_entry: UserCodeLauncherEntry,
         server_handle: Service,
         server_endpoint: ServerEndpoint,
     ) -> None:
         metadata = user_code_launcher_entry.code_deployment_metadata
         self._logger.info(
             f"Waiting for service {server_handle.name} to be ready for gRPC server..."
         )
-        task_arn = self.client.wait_for_new_service(
+        task_arn = await self.client.wait_for_new_service(
             server_handle, container_name=CONTAINER_NAME, logger=self._logger
         )
 
         multipex_client = None
 
         if metadata.pex_metadata:
             multipex_server = check.not_none(
@@ -591,15 +600,15 @@
         if metadata.pex_metadata:
             additional_check = lambda: _assert_new_pex_server_did_not_crash()
         else:
             additional_check = lambda: self.client.assert_task_not_stopped(
                 task_arn, CONTAINER_NAME, self._logger
             )
 
-        self._wait_for_dagster_server_process(
+        await self._wait_for_dagster_server_process(
             client=server_endpoint.create_client(),
             timeout=self._server_process_startup_timeout,
             additional_check=additional_check,
             get_timeout_debug_info=lambda: self._get_update_failure_debug_info(task_arn),
         )
 
     def _remove_server_handle(self, server_handle: EcsServerHandleType) -> None:
```

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/run_launcher.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/run_launcher.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/service.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/service.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/ecs/utils.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/ecs/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/kubernetes/launcher.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/kubernetes/launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,36 +506,36 @@
         # reconciliation - this is used to indicate that we're ready to
         # serve requests
         Path("/tmp/finished_initial_reconciliation_sentinel.txt").touch(exist_ok=True)
         self._logger.info(
             "Wrote liveness sentinel: indicating that agent is ready to serve requests"
         )
 
-    def _wait_for_new_server_ready(
+    async def _wait_for_new_server_ready(
         self,
         deployment_name: str,
         location_name: str,
         user_code_launcher_entry: UserCodeLauncherEntry,
         server_handle: K8sHandle,
         server_endpoint: ServerEndpoint,
     ) -> None:
         metadata = user_code_launcher_entry.code_deployment_metadata
 
-        wait_for_deployment_complete(
+        await wait_for_deployment_complete(
             server_handle.name,
             server_handle.namespace,
             self._logger,
             location_name,
             metadata,
             timeout=self._deployment_startup_timeout,
             image_pull_grace_period=self._image_pull_grace_period,
             core_api=self._get_core_api_client(),
         )
 
-        self._wait_for_dagster_server_process(
+        await self._wait_for_dagster_server_process(
             client=server_endpoint.create_client(),
             timeout=self._server_process_startup_timeout,
             get_timeout_debug_info=lambda: self._get_timeout_debug_info(server_handle),
         )
 
     def _get_standalone_dagster_server_handles_for_location(
         self,
```

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/kubernetes/utils.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/kubernetes/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import copy
 import re
 import time
 from typing import Mapping, Optional
 
 import kubernetes
 from dagster_k8s.client import DagsterKubernetesClient
@@ -213,15 +214,15 @@
         pod_debug_info = api_client.get_pod_debug_info(pod_name, namespace)
     except Exception:
         logger.exception(f"Error trying to get debug information for failed k8s pod {pod_name}")
 
     return f"{pod_debug_info}\n\n{kubectl_prompt}" if pod_debug_info else kubectl_prompt
 
 
-def wait_for_deployment_complete(
+async def wait_for_deployment_complete(
     k8s_deployment_name,
     namespace,
     logger,
     location_name,
     metadata,
     timeout,
     image_pull_grace_period,
@@ -233,15 +234,15 @@
     api = client.AppsV1Api(client.ApiClient())
 
     start = time.time()
 
     pod_list = []
 
     while True:
-        time.sleep(2)
+        await asyncio.sleep(2)
 
         time_elapsed = time.time() - start
 
         if time_elapsed >= timeout:
             timeout_message: str = f"Timed out waiting for deployment {k8s_deployment_name}."
             debug_info = get_deployment_failure_debug_info(
                 k8s_deployment_name, namespace, core_api, pod_list, logger
```

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/__init__.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/process.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/process.py`

 * *Files 0% similar despite different names*

```diff
@@ -313,23 +313,23 @@
             host="localhost",
             port=port,
             socket=socket,
         )
 
         return DagsterCloudGrpcServer(pid, endpoint, metadata)
 
-    def _wait_for_new_server_ready(
+    async def _wait_for_new_server_ready(
         self,
         deployment_name: str,
         location_name: str,
         desired_entry: UserCodeLauncherEntry,
         server_handle: int,
         server_endpoint: ServerEndpoint,
     ) -> None:
-        self._wait_for_dagster_server_process(
+        await self._wait_for_dagster_server_process(
             client=server_endpoint.create_client(),
             timeout=self._server_process_startup_timeout,
         )
 
     def _get_standalone_dagster_server_handles_for_location(
         self, deployment_name: str, location_name: str
     ) -> Collection[int]:
```

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/user_code_launcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # The following allows logging calls with extra arguments
 # ruff: noqa: PLE1205
+import asyncio
+import functools
 import json
 import logging
 import os
 import sys
 import tempfile
 import threading
 import time
@@ -119,14 +121,26 @@
         }
     }
 """
 
 DEFAULT_SERVER_TTL_SECONDS = 60 * 60 * 24
 
 
+def async_serialize_exceptions(func):
+    @functools.wraps(func)
+    async def wrapper(*args, **kwargs):
+        try:
+            return await func(*args, **kwargs)
+        except Exception:
+            # Capture and return exception details and stack trace
+            return serializable_error_info_from_exc_info(sys.exc_info())
+
+    return wrapper
+
+
 @whitelist_for_serdes
 class UserCodeLauncherEntry(
     NamedTuple(
         "_UserCodeLauncherEntry",
         [
             ("code_deployment_metadata", CodeDeploymentMetadata),
             ("update_timestamp", float),
@@ -817,28 +831,89 @@
         desired_entry: UserCodeLauncherEntry,
     ) -> DagsterCloudGrpcServer:
         """Create a new server for the given location using the given metadata as configuration
         and return a ServerHandle indicating where it can be found. Any waiting for the server
         to happen should happen in _wait_for_new_server_ready.
         """
 
-    def _wait_for_new_multipex_server(
+    @async_serialize_exceptions
+    async def _wait_for_new_multipex_server(
         self,
         _deployment_name: str,
         _location_name: str,
         _server_handle: ServerHandle,
         multipex_endpoint: ServerEndpoint,
     ):
-        self._wait_for_server_process(
+        await self._wait_for_server_process(
             multipex_endpoint.create_multipex_client(),
             timeout=self._server_process_startup_timeout,
         )
 
+    @async_serialize_exceptions
+    async def _wait_for_new_server_ready_and_possibly_upload(
+        self,
+        to_update_key: DeploymentAndLocation,
+        server_or_error: Union[DagsterCloudGrpcServer, SerializableErrorInfo],
+        desired_entry: UserCodeLauncherEntry,
+        should_upload: bool,
+    ):
+        deployment_name, location_name = to_update_key
+
+        code_deployment_metadata = desired_entry.code_deployment_metadata
+        pex_metadata = code_deployment_metadata.pex_metadata
+        deployment_info = (
+            f"(pex_tag={pex_metadata.pex_tag}, python_version={pex_metadata.python_version})"
+            if pex_metadata
+            else f"(image={code_deployment_metadata})"
+        )
+        if not isinstance(server_or_error, SerializableErrorInfo):
+            try:
+                self._logger.info(
+                    f"Waiting for new grpc server for {deployment_name}:{location_name} for {deployment_info} to be ready..."
+                )
+                await self._wait_for_new_server_ready(
+                    deployment_name,
+                    location_name,
+                    desired_entry,
+                    server_or_error.server_handle,
+                    server_or_error.server_endpoint,
+                )
+            except Exception:
+                error_info = serializable_error_info_from_exc_info(sys.exc_info())
+                self._logger.error(
+                    f"Error while waiting for server for {deployment_name}:{location_name} for {deployment_info} to be"
+                    f" ready: {error_info}"
+                )
+                server_or_error = error_info
+
+        if should_upload:
+            try:
+                self._update_location_data(
+                    deployment_name,
+                    location_name,
+                    server_or_error,
+                    desired_entry.code_deployment_metadata,
+                )
+            except Exception:
+                # If there was a failure uploading snapshots, log it but don't block other code locations
+                # from updating (and still use the new server to serve new requests)
+                error_info = serializable_error_info_from_exc_info(sys.exc_info())
+                self._logger.error(
+                    f"Error while writing location data for {deployment_name}:{location_name}:"
+                    f" {error_info}"
+                )
+
+        # Once we've verified that the new server has uploaded its data successfully, swap in
+        # the server to start serving new requests
+        with self._grpc_servers_lock:
+            self._grpc_servers[to_update_key] = server_or_error
+            self._first_unavailable_times.pop(to_update_key, None)
+
     @abstractmethod
-    def _wait_for_new_server_ready(
+    async def _wait_for_new_server_ready(
         self,
         deployment_name: str,
         location_name: str,
         desired_entry: UserCodeLauncherEntry,
         server_handle: ServerHandle,
         server_endpoint: ServerEndpoint,
     ) -> None:
@@ -1323,14 +1398,18 @@
             )
             + "}"
         )
 
     def _check_running_multipex_server(self, multipex_server: DagsterCloudGrpcServer):
         multipex_server.server_endpoint.create_multipex_client().ping("")
 
+    async def _gather_tasks(self, tasks):
+        # Single async function that can be passed into asyncio.run
+        return await asyncio.gather(*tasks)
+
     def _reconcile(
         self,
         desired_entries: Dict[DeploymentAndLocation, UserCodeLauncherEntry],
         upload_locations: Set[DeploymentAndLocation],
         check_on_pending_delete_servers: bool,
     ):
         if check_on_pending_delete_servers:
@@ -1456,30 +1535,41 @@
                     new_dagster_servers[to_update_key] = error_info
             elif to_update_key in self._multipex_servers:
                 # This key is no longer a multipex server
                 del self._multipex_servers[to_update_key]
 
         # For each new multi-pex server, wait for it to be ready. If it fails, put
         # the location that was planned to use it into an error state
+
+        tasks = {}
+
         for to_update_key, multipex_server in new_multipex_servers.items():
             deployment_name, location_name = to_update_key
 
-            try:
-                self._logger.info(
-                    f"Waiting for new multipex server for {deployment_name}:{location_name} to be"
-                    " ready"
-                )
-                self._wait_for_new_multipex_server(
-                    deployment_name,
-                    location_name,
-                    multipex_server.server_handle,
-                    multipex_server.server_endpoint,
-                )
-            except Exception:
-                error_info = serializable_error_info_from_exc_info(sys.exc_info())
+            self._logger.info(
+                f"Waiting for new multipex server for {deployment_name}:{location_name} to be"
+                " ready"
+            )
+            tasks[to_update_key] = self._wait_for_new_multipex_server(
+                deployment_name,
+                location_name,
+                multipex_server.server_handle,
+                multipex_server.server_endpoint,
+            )
+
+        # Wait for each new multipex server concurrently
+        results = asyncio.run(self._gather_tasks(tasks.values()))
+
+        results_with_keys = dict(zip(tasks.keys(), results))
+
+        for to_update_key, result in results_with_keys.items():
+            deployment_name, location_name = to_update_key
+
+            if isinstance(result, SerializableErrorInfo):
+                error_info = result
 
                 self._logger.error(
                     f"Error while waiting for multipex server for {deployment_name}:{location_name}:"
                     f" {error_info}"
                 )
                 new_dagster_servers[to_update_key] = error_info
                 # Clear out this multipex server so we don't try to use it again
@@ -1521,70 +1611,41 @@
                 error_info = serializable_error_info_from_exc_info(sys.exc_info())
                 self._logger.error(
                     f"Error while updating server for {deployment_name}:{location_name}:"
                     f" {error_info}"
                 )
                 new_dagster_servers[to_update_key] = error_info
 
+        tasks = {}
+
         # Wait for all new dagster servers (standalone or within a multipex server) to be ready
+        # concurrently, possibly uploading the results to Dagster servers if requested
         for to_update_key in to_update_keys:
-            deployment_name, location_name = to_update_key
-            code_deployment_metadata = desired_entries[to_update_key].code_deployment_metadata
             server_or_error = new_dagster_servers[to_update_key]
-
-            pex_metadata = code_deployment_metadata.pex_metadata
-            deployment_info = (
-                f"(pex_tag={pex_metadata.pex_tag}, python_version={pex_metadata.python_version})"
-                if pex_metadata
-                else f"(image={code_deployment_metadata})"
+            tasks[to_update_key] = self._wait_for_new_server_ready_and_possibly_upload(
+                to_update_key,
+                server_or_error,
+                desired_entries[to_update_key],
+                should_upload=to_update_key in upload_locations,
             )
-            if not isinstance(server_or_error, SerializableErrorInfo):
-                try:
-                    self._logger.info(
-                        f"Waiting for new grpc server for {to_update_key} for {deployment_info} to be ready..."
-                    )
-                    self._wait_for_new_server_ready(
-                        deployment_name,
-                        location_name,
-                        desired_entries[to_update_key],
-                        server_or_error.server_handle,
-                        server_or_error.server_endpoint,
-                    )
-                except Exception:
-                    error_info = serializable_error_info_from_exc_info(sys.exc_info())
-                    self._logger.error(
-                        f"Error while waiting for server for {deployment_name}:{location_name} for {deployment_info} to be"
-                        f" ready: {error_info}"
-                    )
-                    server_or_error = error_info
 
-            # If needed, upload snapshot information to Dagster Cloud
-            if to_update_key in upload_locations:
-                upload_locations.remove(to_update_key)
-                try:
-                    self._update_location_data(
-                        deployment_name,
-                        location_name,
-                        server_or_error,
-                        desired_entries[to_update_key].code_deployment_metadata,
-                    )
-                except Exception:
-                    # If there was a failure uploading snapshots, log it but don't block other code locations
-                    # from updating (and still use the new server to serve new requests)
-                    error_info = serializable_error_info_from_exc_info(sys.exc_info())
-                    self._logger.error(
-                        f"Error while writing location data for {deployment_name}:{location_name}:"
-                        f" {error_info}"
-                    )
+        results = asyncio.run(self._gather_tasks(tasks.values()))
+        results_with_keys = dict(zip(tasks.keys(), results))
+        for to_update_key, result in results_with_keys.items():
+            deployment_name, location_name = to_update_key
 
-            # Once we've verified that the new server has uploaded its data successfully, swap in
-            # the server to start serving new requests
-            with self._grpc_servers_lock:
-                self._grpc_servers[to_update_key] = server_or_error
-                self._first_unavailable_times.pop(to_update_key, None)
+            # Don't expect any uncaught exceptions here, but can't hurt
+            if isinstance(result, SerializableErrorInfo):
+                error_info = serializable_error_info_from_exc_info(sys.exc_info())
+                self._logger.error(
+                    f"Error while waiting for new server for {deployment_name}:{location_name}:"
+                    f" {error_info}"
+                )
+
+        upload_locations.difference_update(to_update_keys)
 
         for to_update_key in to_update_keys:
             deployment_name, location_name = to_update_key
 
             # Remove any old standalone grpc server containers
             server_handles = existing_standalone_dagster_server_handles.get(to_update_key, [])
             removed_any_servers = False
@@ -1904,28 +1965,28 @@
 
         existing_multipex_server_handles = self._get_multipex_server_handles_for_location(
             deployment_name, location_name
         )
         for server_handle in existing_multipex_server_handles:
             self._graceful_remove_server_handle(server_handle)
 
-    def _wait_for_dagster_server_process(
+    async def _wait_for_dagster_server_process(
         self,
         client: DagsterGrpcClient,
         timeout,
         additional_check: Optional[Callable[[], None]] = None,
         get_timeout_debug_info: Optional[Callable[[], Any]] = None,
     ) -> None:
-        self._wait_for_server_process(
+        await self._wait_for_server_process(
             client, timeout, additional_check, get_timeout_debug_info=get_timeout_debug_info
         )
         # Call a method that raises an exception if there was an error importing the code
         sync_list_repositories_grpc(client)
 
-    def _wait_for_server_process(
+    async def _wait_for_server_process(
         self,
         client: Union[DagsterGrpcClient, MultiPexGrpcClient],
         timeout,
         additional_check: Optional[Callable[[], None]] = None,
         additional_check_interval: int = 5,
         get_timeout_debug_info: Optional[Callable[[], None]] = None,
     ) -> None:
@@ -1953,15 +2014,15 @@
                 raise Exception(
                     f"Timed out after waiting {timeout}s for server"
                     f" {client.host}:{client.port or client.socket}."
                     + (f"\n\n{timeout_debug_info}" if timeout_debug_info else "")
                     + f"\n\nMost recent connection error: {last_error}"
                 )
 
-            time.sleep(1)
+            await asyncio.sleep(1)
 
             if additional_check and (
                 not last_additional_check_time
                 or time.time() - last_additional_check_time > additional_check_interval
             ):
                 last_additional_check_time = time.time()
                 additional_check()
```

### Comparing `dagster-cloud-1.7.5/dagster_cloud/workspace/user_code_launcher/utils.py` & `dagster-cloud-1.7.6/dagster_cloud/workspace/user_code_launcher/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/dagster_cloud.egg-info/PKG-INFO` & `dagster-cloud-1.7.6/dagster_cloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-cloud
-Version: 1.7.5
+Version: 1.7.6
 Author: Elementl
 Author-email: support@elementl.com
 License: Apache-2.0
 Project-URL: Homepage, https://dagster.io/cloud
 Project-URL: GitHub, https://github.com/dagster-io/dagster-cloud
 Project-URL: Changelog, https://github.com/dagster-io/dagster-cloud/blob/main/CHANGES.md
 Project-URL: Issue Tracker, https://github.com/dagster-io/dagster-cloud/issues
```

### Comparing `dagster-cloud-1.7.5/dagster_cloud.egg-info/SOURCES.txt` & `dagster-cloud-1.7.6/dagster_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-cloud-1.7.5/setup.py` & `dagster-cloud-1.7.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,20 +36,20 @@
         "Slack": "https://dagster.io/slack",
         "Blog": "https://dagster.io/blog",
         "Newsletter": "https://dagster.io/newsletter-signup",
     },
     packages=find_packages(exclude=["dagster_cloud_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.7.5",
-        "dagster-cloud-cli==1.7.5",
+        "dagster==1.7.6",
+        "dagster-cloud-cli==1.7.6",
         "pex>=2.1.132,<3",
         "questionary",
         "requests",
-        "typer[all]",
+        "typer",
     ],
     extras_require={
         "tests": [
             "docker",
             "httpretty",
             "isort",
             "kubernetes",
@@ -62,21 +62,21 @@
             "types-PyYAML",
             "types-requests",
             "dagster-cloud-test-infra",
             "dbt-core",
             "dbt-snowflake",
             "dbt-postgres",
             "dbt-duckdb",
-            "dagster-dbt==0.23.5",
-            "dagster_k8s==0.23.5",
+            "dagster-dbt==0.23.6",
+            "dagster_k8s==0.23.6",
         ],
         "insights": ["pyarrow"],
-        "docker": ["docker", "dagster_docker==0.23.5"],
-        "kubernetes": ["kubernetes", "dagster_k8s==0.23.5"],
-        "ecs": ["dagster_aws==0.23.5", "boto3"],
+        "docker": ["docker", "dagster_docker==0.23.6"],
+        "kubernetes": ["kubernetes", "dagster_k8s==0.23.6"],
+        "ecs": ["dagster_aws==0.23.6", "boto3"],
         "sandbox": ["supervisor"],
         "pex": ["boto3"],
         "serverless": ["boto3"],
     },
     author="Elementl",
     license="Apache-2.0",
     classifiers=[
```

