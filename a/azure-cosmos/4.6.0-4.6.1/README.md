# Comparing `tmp/azure-cosmos-4.6.0.tar.gz` & `tmp/azure-cosmos-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-cosmos-4.6.0.tar", last modified: Thu Mar 14 22:17:06 2024, max compression
+gzip compressed data, was "azure-cosmos-4.6.1.tar", last modified: Wed May 15 22:23:21 2024, max compression
```

## Comparing `azure-cosmos-4.6.0.tar` & `azure-cosmos-4.6.1.tar`

### file list

```diff
@@ -1,186 +1,194 @@
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-14 22:17:06.992251 azure-cosmos-4.6.0/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24344 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/CHANGELOG.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      147 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/Contributing.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/LICENSE
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      149 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/MANIFEST.in
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    63518 2024-03-14 22:17:06.992251 azure-cosmos-4.6.0/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    38026 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/README.md
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-14 22:17:06.960251 azure-cosmos-4.6.0/azure/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-14 22:17:06.968251 azure-cosmos-4.6.0/azure/cosmos/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2200 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2439 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_auth_policy.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34487 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_base.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2968 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_constants.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   118906 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_cosmos_client_connection.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4034 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_cosmos_http_logging_policy.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6437 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_cosmos_integers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5157 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_cosmos_murmurhash3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2308 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_default_retry_policy.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4756 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_endpoint_discovery_retry_policy.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-14 22:17:06.968251 azure-cosmos-4.6.0/azure/cosmos/_execution_context/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1121 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_execution_context/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2258 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_execution_context/aggregators.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-14 22:17:06.972252 azure-cosmos-4.6.0/azure/cosmos/_execution_context/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1121 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_execution_context/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3590 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_execution_context/aio/_queue_async_helper.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6184 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_execution_context/aio/base_execution_context.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9198 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_execution_context/aio/document_producer.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7516 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_execution_context/aio/endpoint_component.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8955 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_execution_context/aio/execution_dispatcher.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8507 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6100 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_execution_context/base_execution_context.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9248 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_execution_context/document_producer.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7671 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_execution_context/endpoint_component.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9096 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_execution_context/execution_dispatcher.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8092 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_execution_context/multi_execution_aggregator.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5153 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_execution_context/query_execution_info.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8127 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_global_endpoint_manager.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2385 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_gone_retry_policy.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14980 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_location_cache.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2904 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_partition.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4021 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_query_iterable.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3230 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_range.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5079 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_range_partition_resolver.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2508 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_request_object.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3064 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_resource_throttle_retry_policy.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2538 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_retry_options.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10779 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_retry_utility.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-14 22:17:06.972252 azure-cosmos-4.6.0/azure/cosmos/_routing/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1121 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_routing/__init__.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-14 22:17:06.972252 azure-cosmos-4.6.0/azure/cosmos/_routing/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1121 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_routing/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8085 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_routing/aio/routing_map_provider.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7528 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_routing/collection_routing_map.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7964 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_routing/routing_map_provider.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4520 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_routing/routing_range.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1696 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_runtime_constants.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9700 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_session.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5844 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_session_retry_policy.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8132 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_synchronized_request.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2729 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_timeout_failover_retry_policy.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2652 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_utils.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6575 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_vector_session_token.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1140 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/_version.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-14 22:17:06.976251 azure-cosmos-4.6.0/azure/cosmos/aio/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1417 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/aio/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7197 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/aio/_asynchronous_request.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2571 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/aio/_auth_policy_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    56238 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/aio/_container.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24188 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/aio/_cosmos_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   117853 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/aio/_cosmos_client_connection_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    41863 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/aio/_database.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8111 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/aio/_global_endpoint_manager_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4240 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/aio/_query_iterable_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10184 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/aio/_retry_utility_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22161 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/aio/_scripts.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13180 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/aio/_user.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6049 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/auth.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    59552 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/container.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26760 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/cosmos_client.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    42482 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/database.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3629 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/diagnostics.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16441 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/documents.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1509 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/errors.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5220 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/exceptions.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15509 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/http_constants.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2674 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/offer.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12584 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/partition_key.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1894 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/permission.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/py.typed
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    21250 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/scripts.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12252 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/azure/cosmos/user.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-14 22:17:06.992251 azure-cosmos-4.6.0/azure_cosmos.egg-info/
--rw-r--r--   0 cloudtest  (1000) cloudtest  (1000)    63518 2024-03-14 22:17:06.000000 azure-cosmos-4.6.0/azure_cosmos.egg-info/PKG-INFO
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5680 2024-03-14 22:17:06.000000 azure-cosmos-4.6.0/azure_cosmos.egg-info/SOURCES.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-14 22:17:06.000000 azure-cosmos-4.6.0/azure_cosmos.egg-info/dependency_links.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-03-14 22:17:06.000000 azure-cosmos-4.6.0/azure_cosmos.egg-info/not-zip-safe
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       44 2024-03-14 22:17:06.000000 azure-cosmos-4.6.0/azure_cosmos.egg-info/requires.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-03-14 22:17:06.000000 azure-cosmos-4.6.0/azure_cosmos.egg-info/top_level.txt
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      111 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/pyproject.toml
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-14 22:17:06.980251 azure-cosmos-4.6.0/samples/
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-14 22:17:06.980251 azure-cosmos-4.6.0/samples/MultiMasterOperations/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      402 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/MultiMasterOperations/Configurations.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35390 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/MultiMasterOperations/ConflictWorker.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4083 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/MultiMasterOperations/MultiMasterScenario.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      318 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/MultiMasterOperations/Program.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2843 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/MultiMasterOperations/Worker.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3581 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/README.md
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4484 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/access_cosmos_with_aad.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5234 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/access_cosmos_with_aad_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9407 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/access_cosmos_with_resource_token.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10642 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/access_cosmos_with_resource_token_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3794 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/change_feed_management.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4258 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/change_feed_management_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2538 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/client_user_configs.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2571 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/client_user_configs_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5480 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/concurrency_sample.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      905 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/config.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11296 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/container_management.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13996 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/container_management_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4291 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/database_management.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6418 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/database_management_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25279 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/document_management.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27644 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/document_management_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8733 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/examples.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10936 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/examples_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    29702 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/index_management.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    30359 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/index_management_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2640 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/samples/tracing_open_telemetry.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-03-14 22:17:06.992251 azure-cosmos-4.6.0/setup.cfg
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2544 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/setup.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-14 22:17:06.992251 azure-cosmos-4.6.0/test/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1269 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/conftest.py
-drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-03-14 22:17:06.992251 azure-cosmos-4.6.0/test/routing/
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1103 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/routing/__init__.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9052 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/routing/test_collection_routing_map.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9526 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/routing/test_routing_map_provider.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5881 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_aad.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8941 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_aggregate.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12642 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_analytical_ttl.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12912 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_analytical_ttl_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6568 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_auto_scale.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6762 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_auto_scale_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3211 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_backwards_compatibility.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      500 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_base_unit.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      970 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_client_user_agent.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6929 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_config.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5695 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_cosmos_http_logging_policy.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   118715 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_crud.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   113629 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_crud_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35651 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_crud_subpartition.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36221 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_crud_subpartition_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1486 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_diagnostics.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3226 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_encoding.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22878 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_globaldb.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8481 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_globaldb_mock.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3435 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_headers.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3725 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_integrated_cache.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25447 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_location_cache.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11186 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_multi_orderby.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4667 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_multimaster.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1401 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_murmurhash3.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19359 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_orderby.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2521 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_partition_key.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3562 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_partition_split_query.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3118 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_proxy.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    40042 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_query.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    41064 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_query_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5211 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_query_computed_properties.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5832 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_query_computed_properties_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22990 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_query_cross_partition.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26530 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_query_cross_partition_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7207 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_query_execution_context.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4729 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_resource_id.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5006 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_resource_id_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14635 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_retry_policy.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2462 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_routing_map.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5503 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_session.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3006 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_session_container.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4132 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_session_token_unit.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10581 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_streaming_failover.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20449 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_transactional_batch.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    21116 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_transactional_batch_async.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3978 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_ttl.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5549 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_user_configs.py
--rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1164 2024-03-14 22:15:36.000000 azure-cosmos-4.6.0/test/test_utils.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-15 22:23:21.630666 azure-cosmos-4.6.1/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25218 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/CHANGELOG.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      147 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/Contributing.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1073 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/LICENSE
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      149 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/MANIFEST.in
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    70168 2024-05-15 22:23:21.630666 azure-cosmos-4.6.1/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    43876 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/README.md
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-15 22:23:21.602666 azure-cosmos-4.6.1/azure/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       81 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-15 22:23:21.610666 azure-cosmos-4.6.1/azure/cosmos/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2200 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2439 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_auth_policy.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    34655 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_base.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2968 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_constants.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   119671 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_cosmos_client_connection.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4034 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_cosmos_http_logging_policy.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6437 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_cosmos_integers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5157 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_cosmos_murmurhash3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2308 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_default_retry_policy.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4756 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_endpoint_discovery_retry_policy.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-15 22:23:21.614666 azure-cosmos-4.6.1/azure/cosmos/_execution_context/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1121 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2258 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/aggregators.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-15 22:23:21.614666 azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1121 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3590 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/_queue_async_helper.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6456 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/base_execution_context.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11259 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/document_producer.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7896 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/endpoint_component.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10843 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/execution_dispatcher.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8507 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7250 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/non_streaming_order_by_aggregator.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6403 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/base_execution_context.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9948 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/document_producer.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8044 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/endpoint_component.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10833 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/execution_dispatcher.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8092 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/multi_execution_aggregator.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6982 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/non_streaming_order_by_aggregator.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5518 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_execution_context/query_execution_info.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8127 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_global_endpoint_manager.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2385 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_gone_retry_policy.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14980 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_location_cache.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2904 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_partition.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4021 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_query_iterable.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3230 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_range.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5079 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_range_partition_resolver.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2508 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_request_object.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3064 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_resource_throttle_retry_policy.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2538 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_retry_options.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10779 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_retry_utility.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-15 22:23:21.614666 azure-cosmos-4.6.1/azure/cosmos/_routing/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1121 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_routing/__init__.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-15 22:23:21.614666 azure-cosmos-4.6.1/azure/cosmos/_routing/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1121 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_routing/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8085 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_routing/aio/routing_map_provider.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7528 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_routing/collection_routing_map.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7964 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_routing/routing_map_provider.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4520 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_routing/routing_range.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1696 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_runtime_constants.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9700 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_session.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5844 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_session_retry_policy.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8148 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_synchronized_request.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2729 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_timeout_failover_retry_policy.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2652 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_utils.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6575 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_vector_session_token.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1140 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/_version.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-15 22:23:21.618666 azure-cosmos-4.6.1/azure/cosmos/aio/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1417 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/aio/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7213 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/aio/_asynchronous_request.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2571 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/aio/_auth_policy_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    56735 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/aio/_container.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    24189 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/aio/_cosmos_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   118618 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/aio/_cosmos_client_connection_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    42778 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/aio/_database.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8111 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/aio/_global_endpoint_manager_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4240 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/aio/_query_iterable_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10184 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/aio/_retry_utility_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22167 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/aio/_scripts.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13182 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/aio/_user.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6049 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/auth.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    60049 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/container.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26759 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/cosmos_client.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    43488 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/database.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3629 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/diagnostics.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16521 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/documents.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1509 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/errors.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5220 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/exceptions.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    15509 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/http_constants.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2674 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/offer.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12584 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/partition_key.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1894 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/permission.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/py.typed
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    21256 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/scripts.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12254 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/azure/cosmos/user.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-15 22:23:21.618666 azure-cosmos-4.6.1/azure_cosmos.egg-info/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    70168 2024-05-15 22:23:21.000000 azure-cosmos-4.6.1/azure_cosmos.egg-info/PKG-INFO
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6015 2024-05-15 22:23:21.000000 azure-cosmos-4.6.1/azure_cosmos.egg-info/SOURCES.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-15 22:23:21.000000 azure-cosmos-4.6.1/azure_cosmos.egg-info/dependency_links.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        1 2024-05-15 22:23:21.000000 azure-cosmos-4.6.1/azure_cosmos.egg-info/not-zip-safe
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       44 2024-05-15 22:23:21.000000 azure-cosmos-4.6.1/azure_cosmos.egg-info/requires.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)        6 2024-05-15 22:23:21.000000 azure-cosmos-4.6.1/azure_cosmos.egg-info/top_level.txt
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      111 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/pyproject.toml
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-15 22:23:21.622666 azure-cosmos-4.6.1/samples/
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-15 22:23:21.622666 azure-cosmos-4.6.1/samples/MultiMasterOperations/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      402 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/MultiMasterOperations/Configurations.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35390 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/MultiMasterOperations/ConflictWorker.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4083 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/MultiMasterOperations/MultiMasterScenario.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      318 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/MultiMasterOperations/Program.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2843 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/MultiMasterOperations/Worker.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3581 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/README.md
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4484 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/access_cosmos_with_aad.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5234 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/access_cosmos_with_aad_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9407 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/access_cosmos_with_resource_token.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10642 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/access_cosmos_with_resource_token_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4685 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/change_feed_management.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5205 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/change_feed_management_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2538 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/client_user_configs.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2571 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/client_user_configs_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5480 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/concurrency_sample.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      905 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/config.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11296 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/container_management.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    13996 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/container_management_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4291 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/database_management.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6418 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/database_management_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25279 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/document_management.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    27644 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/document_management_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8733 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/examples.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10936 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/examples_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    32737 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/index_management.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    33298 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/index_management_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2640 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/tracing_open_telemetry.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19781 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/samples/vector_test_data.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)       38 2024-05-15 22:23:21.630666 azure-cosmos-4.6.1/setup.cfg
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2544 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/setup.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-15 22:23:21.630666 azure-cosmos-4.6.1/test/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1269 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/conftest.py
+drwxrwxr-x   0 cloudtest  (1000) cloudtest  (1000)        0 2024-05-15 22:23:21.630666 azure-cosmos-4.6.1/test/routing/
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1103 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/routing/__init__.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9052 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/routing/test_collection_routing_map.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9526 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/routing/test_routing_map_provider.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5881 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_aad.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9084 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_aggregate.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12642 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_analytical_ttl.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    12912 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_analytical_ttl_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6568 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_auto_scale.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     6762 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_auto_scale_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3211 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_backwards_compatibility.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      500 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_base_unit.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)      970 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_client_user_agent.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7577 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_config.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5695 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_cosmos_http_logging_policy.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   118715 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_crud.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)   113629 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_crud_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    35651 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_crud_subpartition.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    36221 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_crud_subpartition_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1486 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_diagnostics.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3226 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_encoding.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    22878 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_globaldb.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     8481 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_globaldb_mock.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3435 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_headers.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3725 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_integrated_cache.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    25447 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_location_cache.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    11325 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_multi_orderby.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4667 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_multimaster.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1401 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_murmurhash3.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19359 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_orderby.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2521 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_partition_key.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3701 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_partition_split_query.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3118 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_proxy.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    43172 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_query.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    47305 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_query_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5211 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_query_computed_properties.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5832 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_query_computed_properties_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    23129 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_query_cross_partition.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    26670 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_query_cross_partition_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     7207 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_query_execution_context.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    17386 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_query_vector_similarity.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    16115 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_query_vector_similarity_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4729 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_resource_id.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5006 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_resource_id_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    14635 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_retry_policy.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     2462 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_routing_map.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5503 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_session.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3006 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_session_container.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     4132 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_session_token_unit.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10581 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_streaming_failover.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    20449 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_transactional_batch.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    21116 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_transactional_batch_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     3978 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_ttl.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     5549 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_user_configs.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     1164 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_utils.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)     9924 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_vector_policy.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    10372 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/test_vector_policy_async.py
+-rw-rw-r--   0 cloudtest  (1000) cloudtest  (1000)    19781 2024-05-15 22:22:03.000000 azure-cosmos-4.6.1/test/vector_test_data.py
```

### Comparing `azure-cosmos-4.6.0/CHANGELOG.md` & `azure-cosmos-4.6.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,20 @@
 ## Release History
 
+### 4.6.1 (2024-05-15)
+
+#### Features Added
+* Adds vector embedding policy and vector indexing policy. See [PR 34882](https://github.com/Azure/azure-sdk-for-python/pull/34882).
+* Adds support for vector search non-streaming order by queries. See [PR 35468](https://github.com/Azure/azure-sdk-for-python/pull/35468).
+* Adds support for using the start time option for change feed query API. See [PR 35090](https://github.com/Azure/azure-sdk-for-python/pull/35090).
+
+#### Bugs Fixed
+* Fixed a bug where change feed query in Async client was not returning all pages due to case-sensitive response headers. See [PR 35090](https://github.com/Azure/azure-sdk-for-python/pull/35090).
+* Fixed a bug when a retryable exception occurs in the first page of a query execution causing query to return 0 results. See [PR 35090](https://github.com/Azure/azure-sdk-for-python/pull/35090).
+
 ### 4.6.0 (2024-03-14)
 
 #### Features Added
 * GA release of hierarchical partitioning, index metrics and transactional batch.
 
 #### Bugs Fixed
 * Keyword arguments were not being passed down for `create_container_if_not_exists()` methods. See [PR 34286](https://github.com/Azure/azure-sdk-for-python/pull/34286).
```

### Comparing `azure-cosmos-4.6.0/LICENSE` & `azure-cosmos-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/PKG-INFO` & `azure-cosmos-4.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-cosmos
-Version: 4.6.0
+Version: 4.6.1
 Summary: Microsoft Azure Cosmos Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: askdocdb@microsoft.com
 Maintainer: Microsoft
 Maintainer-email: askdocdb@microsoft.com
 License: MIT License
@@ -21,16 +21,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: azure-core>=1.25.1
-Requires-Dist: typing-extensions>=4.6.0
 
 ## _Disclaimer_
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
 # Azure Cosmos DB SQL API client library for Python
 
 Azure Cosmos DB is a globally distributed, multi-model database service that supports document, key-value, wide-column, and graph databases.
@@ -184,15 +182,14 @@
 * Group By queries
 * Queries with COUNT from a DISTINCT subquery: SELECT COUNT (1) FROM (SELECT DISTINCT C.ID FROM C)
 * Direct TCP Mode access
 * Continuation token support for aggregate cross-partition queries like sorting, counting, and distinct.
 Streamable queries like `SELECT * FROM WHERE` *do* support continuation tokens.
 * Change Feed: Processor
 * Change Feed: Read multiple partitions key values
-* Change Feed: Read specific time
 * Cross-partition ORDER BY for mixed types
 * Enabling diagnostics for async query-type methods
 
 ### Control Plane Limitations:
 
 * Get CollectionSizeUsage, DatabaseUsage, and DocumentUsage metrics
 * Create Geospatial Index
@@ -202,15 +199,15 @@
 ## Workarounds
 
 ### Control Plane Limitations Workaround
 
 Typically, you can use [Azure Portal](https://portal.azure.com/), [Azure Cosmos DB Resource Provider REST API](https://docs.microsoft.com/rest/api/cosmos-db-resource-provider), [Azure CLI](https://docs.microsoft.com/cli/azure/azure-cli-reference-for-cosmos-db) or [PowerShell](https://docs.microsoft.com/azure/cosmos-db/manage-with-powershell) for the control plane unsupported limitations.
 
 ### Using The Async Client as a Workaround to Bulk
-While the SDK supports transactional batch, support for bulk requests is not yet implemented in the Python SDK. You can use the async client along with this [concurrency sample][concurrency_sample] we have developed as a reference for a possible workaround. 
+While the SDK supports transactional batch, support for bulk requests is not yet implemented in the Python SDK. You can use the async client along with this [concurrency sample][cosmos_concurrency_sample] we have developed as a reference for a possible workaround. 
 >[WARNING]
 > Using the asynchronous client for concurrent operations like shown in this sample will consume a lot of RUs very fast. We **strongly recommend** testing this out against the cosmos emulator first to verify your code works well and avoid incurring charges.
 
 
 
 ## Boolean Data Type
 
@@ -655,14 +652,115 @@
 and [async][sample_document_mgmt_async] clients.
 
 If there is a failure for an operation within the batch, the SDK will raise a `CosmosBatchOperationError` letting you know which operation failed,
 as well as containing the list of failed responses for the failed request.
 
 For more information on Transactional Batch, see [Azure Cosmos DB Transactional Batch][cosmos_transactional_batch].
 
+### Public Preview - Vector Embeddings and Vector Indexes
+We have added new capabilities to utilize vector embeddings and vector indexing for users to leverage vector
+search utilizing our Cosmos SDK. These two container-level configurations have to be turned on at the account-level
+before you can use them.
+
+Each vector embedding should have a path to the relevant vector field in your items being stored, a supported data type
+(float32, int8, uint8), the vector's dimensions, and the distance function being used for that embedding. Vectors indexed 
+with the flat index type can be at most 505 dimensions. Vectors indexed with the quantizedFlat index type can be at most 4,096 dimensions.
+A sample vector embedding policy would look like this:
+```python
+vector_embedding_policy = {
+    "vectorEmbeddings": [
+        {
+            "path": "/vector1",
+            "dataType": "float32",
+            "dimensions": 256,
+            "distanceFunction": "euclidean"
+        },
+        {
+            "path": "/vector2",
+            "dataType": "int8",
+            "dimensions": 200,
+            "distanceFunction": "dotproduct"
+        },
+        {
+            "path": "/vector3",
+            "dataType": "uint8",
+            "dimensions": 400,
+            "distanceFunction": "cosine"
+        }
+    ]
+}
+```
+
+Separately, vector indexes have been added to the already existing indexing_policy and only require two fields per index:
+the path to the relevant field to be used, and the type of index from the possible options (flat or quantizedFlat).
+A sample indexing policy with vector indexes would look like this:
+```python
+indexing_policy = {
+        "automatic": True,
+        "indexingMode": "consistent",
+        "compositeIndexes": [
+            [
+                {"path": "/numberField", "order": "ascending"},
+                {"path": "/stringField", "order": "descending"}
+            ]
+        ],
+        "spatialIndexes": [
+            {"path": "/location/*", "types": [
+                "Point",
+                "Polygon"]}
+        ],
+        "vectorIndexes": [
+            {"path": "/vector1", "type": "flat"},
+            {"path": "/vector2", "type": "quantizedFlat"}
+        ]
+    }
+```
+You would then pass in the relevant policies to your container creation method to ensure these configurations are used by it.
+The operation will fail if you pass new vector indexes to your indexing policy but forget to pass in an embedding policy.
+```python
+database.create_container(id=container_id, partition_key=PartitionKey(path="/id"),
+                          indexing_policy=indexing_policy, vector_embedding_policy=vector_embedding_policy)
+```
+***Note: vector embeddings and vector indexes CANNOT be edited by container replace operations. They are only available directly through creation.***
+
+### Public Preview - Vector Search
+
+With the addition of the vector indexing and vector embedding capabilities, the SDK can now perform order by vector search queries.
+These queries specify the VectorDistance to use as a metric within the query text. These must always use a TOP or LIMIT clause within the query though,
+since vector search queries have to look through a lot of data otherwise and may become too expensive or long-running.
+Since these queries are relatively expensive, the SDK sets a default limit of 50000 max items per query - if you'd like to raise that further, you
+can use the `AZURE_COSMOS_MAX_ITEM_BUFFER_VECTOR_SEARCH` environment variable to do so. However, be advised that queries with too many vector results
+may have additional latencies associated with searching in the service.
+The query syntax for these operations looks like this:
+```python
+VectorDistance(<embedding1>, <embedding2>, [,<exact_search>], [,<specification>])
+```
+Embeddings 1 and 2 are the arrays of values for the relevant embeddings, `exact_search` is an optional boolean indicating whether
+to do an exact search vs. an approximate one (default value of false), and `specification` is an optional Json snippet with embedding
+specs that can include `dataType`, `dimensions` and `distanceFunction`. The specifications within the query will take precedence
+to any configurations previously set by a vector embedding policy.
+A sample vector search query would look something like this:
+```python
+    query = "SELECT TOP 10 c.title,VectorDistance(c.embedding, [{}]) AS " \
+            "SimilarityScore FROM c ORDER BY VectorDistance(c.embedding, [{}])".format(embeddings_string, embeddings_string)
+```
+Or if you'd like to add the optional parameters to the vector distance, you could do this:
+```python
+    query = "SELECT TOP 10 c.title,VectorDistance(c.embedding, [{}], true, {{'dataType': 'float32' , 'distanceFunction': 'cosine'}}) AS " \
+            "SimilarityScore FROM c ORDER BY VectorDistance(c.embedding, [{}], true, {{'dataType': " \
+            "'float32', 'distanceFunction': 'cosine'}})".format(embeddings_string, embeddings_string)
+```
+The `embeddings_string` above would be your string made from your vector embeddings.
+You can find our sync samples [here][cosmos_index_sample] and our async samples [here][cosmos_index_sample_async] as well to help yourself out.
+
+*Note: For a limited time, if your query operates against a region or emulator that has not yet been updated the client might run into some issues
+not being able to recognize the new NonStreamingOrderBy capability that makes vector search possible.
+If this happens, you can set the `AZURE_COSMOS_DISABLE_NON_STREAMING_ORDER_BY` environment variable to `"True"` to opt out of this
+functionality and continue operating as usual.*
+
 ## Troubleshooting
 
 ### General
 
 When you interact with Cosmos DB using the Python SDK, exceptions returned by the service correspond to the same HTTP status codes returned for REST API requests:
 
 [HTTP Status Codes for Azure Cosmos DB][cosmos_http_status_codes]
@@ -789,14 +887,16 @@
 [source_code]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos
 [venv]: https://docs.python.org/3/library/venv.html
 [virtualenv]: https://virtualenv.pypa.io
 [telemetry_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/tracing_open_telemetry.py
 [timeouts_document]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/docs/TimeoutAndRetriesConfig.md
 [cosmos_transactional_batch]: https://learn.microsoft.com/azure/cosmos-db/nosql/transactional-batch
 [cosmos_concurrency_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/concurrency_sample.py
+[cosmos_index_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/index_management.py
+[cosmos_index_sample_async]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/index_management_async.py
 
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.microsoft.com.
 
@@ -806,14 +906,25 @@
 
 This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
 For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
 contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
 ## Release History
 
+### 4.6.1 (2024-05-15)
+
+#### Features Added
+* Adds vector embedding policy and vector indexing policy. See [PR 34882](https://github.com/Azure/azure-sdk-for-python/pull/34882).
+* Adds support for vector search non-streaming order by queries. See [PR 35468](https://github.com/Azure/azure-sdk-for-python/pull/35468).
+* Adds support for using the start time option for change feed query API. See [PR 35090](https://github.com/Azure/azure-sdk-for-python/pull/35090).
+
+#### Bugs Fixed
+* Fixed a bug where change feed query in Async client was not returning all pages due to case-sensitive response headers. See [PR 35090](https://github.com/Azure/azure-sdk-for-python/pull/35090).
+* Fixed a bug when a retryable exception occurs in the first page of a query execution causing query to return 0 results. See [PR 35090](https://github.com/Azure/azure-sdk-for-python/pull/35090).
+
 ### 4.6.0 (2024-03-14)
 
 #### Features Added
 * GA release of hierarchical partitioning, index metrics and transactional batch.
 
 #### Bugs Fixed
 * Keyword arguments were not being passed down for `create_container_if_not_exists()` methods. See [PR 34286](https://github.com/Azure/azure-sdk-for-python/pull/34286).
```

### Comparing `azure-cosmos-4.6.0/README.md` & `azure-cosmos-4.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -154,15 +154,14 @@
 * Group By queries
 * Queries with COUNT from a DISTINCT subquery: SELECT COUNT (1) FROM (SELECT DISTINCT C.ID FROM C)
 * Direct TCP Mode access
 * Continuation token support for aggregate cross-partition queries like sorting, counting, and distinct.
 Streamable queries like `SELECT * FROM WHERE` *do* support continuation tokens.
 * Change Feed: Processor
 * Change Feed: Read multiple partitions key values
-* Change Feed: Read specific time
 * Cross-partition ORDER BY for mixed types
 * Enabling diagnostics for async query-type methods
 
 ### Control Plane Limitations:
 
 * Get CollectionSizeUsage, DatabaseUsage, and DocumentUsage metrics
 * Create Geospatial Index
@@ -172,15 +171,15 @@
 ## Workarounds
 
 ### Control Plane Limitations Workaround
 
 Typically, you can use [Azure Portal](https://portal.azure.com/), [Azure Cosmos DB Resource Provider REST API](https://docs.microsoft.com/rest/api/cosmos-db-resource-provider), [Azure CLI](https://docs.microsoft.com/cli/azure/azure-cli-reference-for-cosmos-db) or [PowerShell](https://docs.microsoft.com/azure/cosmos-db/manage-with-powershell) for the control plane unsupported limitations.
 
 ### Using The Async Client as a Workaround to Bulk
-While the SDK supports transactional batch, support for bulk requests is not yet implemented in the Python SDK. You can use the async client along with this [concurrency sample][concurrency_sample] we have developed as a reference for a possible workaround. 
+While the SDK supports transactional batch, support for bulk requests is not yet implemented in the Python SDK. You can use the async client along with this [concurrency sample][cosmos_concurrency_sample] we have developed as a reference for a possible workaround. 
 >[WARNING]
 > Using the asynchronous client for concurrent operations like shown in this sample will consume a lot of RUs very fast. We **strongly recommend** testing this out against the cosmos emulator first to verify your code works well and avoid incurring charges.
 
 
 
 ## Boolean Data Type
 
@@ -625,14 +624,115 @@
 and [async][sample_document_mgmt_async] clients.
 
 If there is a failure for an operation within the batch, the SDK will raise a `CosmosBatchOperationError` letting you know which operation failed,
 as well as containing the list of failed responses for the failed request.
 
 For more information on Transactional Batch, see [Azure Cosmos DB Transactional Batch][cosmos_transactional_batch].
 
+### Public Preview - Vector Embeddings and Vector Indexes
+We have added new capabilities to utilize vector embeddings and vector indexing for users to leverage vector
+search utilizing our Cosmos SDK. These two container-level configurations have to be turned on at the account-level
+before you can use them.
+
+Each vector embedding should have a path to the relevant vector field in your items being stored, a supported data type
+(float32, int8, uint8), the vector's dimensions, and the distance function being used for that embedding. Vectors indexed 
+with the flat index type can be at most 505 dimensions. Vectors indexed with the quantizedFlat index type can be at most 4,096 dimensions.
+A sample vector embedding policy would look like this:
+```python
+vector_embedding_policy = {
+    "vectorEmbeddings": [
+        {
+            "path": "/vector1",
+            "dataType": "float32",
+            "dimensions": 256,
+            "distanceFunction": "euclidean"
+        },
+        {
+            "path": "/vector2",
+            "dataType": "int8",
+            "dimensions": 200,
+            "distanceFunction": "dotproduct"
+        },
+        {
+            "path": "/vector3",
+            "dataType": "uint8",
+            "dimensions": 400,
+            "distanceFunction": "cosine"
+        }
+    ]
+}
+```
+
+Separately, vector indexes have been added to the already existing indexing_policy and only require two fields per index:
+the path to the relevant field to be used, and the type of index from the possible options (flat or quantizedFlat).
+A sample indexing policy with vector indexes would look like this:
+```python
+indexing_policy = {
+        "automatic": True,
+        "indexingMode": "consistent",
+        "compositeIndexes": [
+            [
+                {"path": "/numberField", "order": "ascending"},
+                {"path": "/stringField", "order": "descending"}
+            ]
+        ],
+        "spatialIndexes": [
+            {"path": "/location/*", "types": [
+                "Point",
+                "Polygon"]}
+        ],
+        "vectorIndexes": [
+            {"path": "/vector1", "type": "flat"},
+            {"path": "/vector2", "type": "quantizedFlat"}
+        ]
+    }
+```
+You would then pass in the relevant policies to your container creation method to ensure these configurations are used by it.
+The operation will fail if you pass new vector indexes to your indexing policy but forget to pass in an embedding policy.
+```python
+database.create_container(id=container_id, partition_key=PartitionKey(path="/id"),
+                          indexing_policy=indexing_policy, vector_embedding_policy=vector_embedding_policy)
+```
+***Note: vector embeddings and vector indexes CANNOT be edited by container replace operations. They are only available directly through creation.***
+
+### Public Preview - Vector Search
+
+With the addition of the vector indexing and vector embedding capabilities, the SDK can now perform order by vector search queries.
+These queries specify the VectorDistance to use as a metric within the query text. These must always use a TOP or LIMIT clause within the query though,
+since vector search queries have to look through a lot of data otherwise and may become too expensive or long-running.
+Since these queries are relatively expensive, the SDK sets a default limit of 50000 max items per query - if you'd like to raise that further, you
+can use the `AZURE_COSMOS_MAX_ITEM_BUFFER_VECTOR_SEARCH` environment variable to do so. However, be advised that queries with too many vector results
+may have additional latencies associated with searching in the service.
+The query syntax for these operations looks like this:
+```python
+VectorDistance(<embedding1>, <embedding2>, [,<exact_search>], [,<specification>])
+```
+Embeddings 1 and 2 are the arrays of values for the relevant embeddings, `exact_search` is an optional boolean indicating whether
+to do an exact search vs. an approximate one (default value of false), and `specification` is an optional Json snippet with embedding
+specs that can include `dataType`, `dimensions` and `distanceFunction`. The specifications within the query will take precedence
+to any configurations previously set by a vector embedding policy.
+A sample vector search query would look something like this:
+```python
+    query = "SELECT TOP 10 c.title,VectorDistance(c.embedding, [{}]) AS " \
+            "SimilarityScore FROM c ORDER BY VectorDistance(c.embedding, [{}])".format(embeddings_string, embeddings_string)
+```
+Or if you'd like to add the optional parameters to the vector distance, you could do this:
+```python
+    query = "SELECT TOP 10 c.title,VectorDistance(c.embedding, [{}], true, {{'dataType': 'float32' , 'distanceFunction': 'cosine'}}) AS " \
+            "SimilarityScore FROM c ORDER BY VectorDistance(c.embedding, [{}], true, {{'dataType': " \
+            "'float32', 'distanceFunction': 'cosine'}})".format(embeddings_string, embeddings_string)
+```
+The `embeddings_string` above would be your string made from your vector embeddings.
+You can find our sync samples [here][cosmos_index_sample] and our async samples [here][cosmos_index_sample_async] as well to help yourself out.
+
+*Note: For a limited time, if your query operates against a region or emulator that has not yet been updated the client might run into some issues
+not being able to recognize the new NonStreamingOrderBy capability that makes vector search possible.
+If this happens, you can set the `AZURE_COSMOS_DISABLE_NON_STREAMING_ORDER_BY` environment variable to `"True"` to opt out of this
+functionality and continue operating as usual.*
+
 ## Troubleshooting
 
 ### General
 
 When you interact with Cosmos DB using the Python SDK, exceptions returned by the service correspond to the same HTTP status codes returned for REST API requests:
 
 [HTTP Status Codes for Azure Cosmos DB][cosmos_http_status_codes]
@@ -759,14 +859,16 @@
 [source_code]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos
 [venv]: https://docs.python.org/3/library/venv.html
 [virtualenv]: https://virtualenv.pypa.io
 [telemetry_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/tracing_open_telemetry.py
 [timeouts_document]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/docs/TimeoutAndRetriesConfig.md
 [cosmos_transactional_batch]: https://learn.microsoft.com/azure/cosmos-db/nosql/transactional-batch
 [cosmos_concurrency_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/concurrency_sample.py
+[cosmos_index_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/index_management.py
+[cosmos_index_sample_async]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/index_management_async.py
 
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.microsoft.com.
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/__init__.py` & `azure-cosmos-4.6.1/azure/cosmos/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_auth_policy.py` & `azure-cosmos-4.6.1/azure/cosmos/_auth_policy.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_base.py` & `azure-cosmos-4.6.1/azure/cosmos/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,16 +287,20 @@
     if options.get("changeFeed") is True:
         # On REST level, change feed is using IfNoneMatch/ETag instead of continuation.
         if_none_match_value = None
         if options.get("continuation"):
             if_none_match_value = options["continuation"]
         elif options.get("isStartFromBeginning") and not options["isStartFromBeginning"]:
             if_none_match_value = "*"
+        elif options.get("startTime"):
+            start_time = options.get("startTime")
+            headers[http_constants.HttpHeaders.IfModified_since] = start_time
         if if_none_match_value:
             headers[http_constants.HttpHeaders.IfNoneMatch] = if_none_match_value
+
         headers[http_constants.HttpHeaders.AIM] = http_constants.HttpHeaders.IncrementalFeedHeaderValue
     else:
         if options.get("continuation"):
             headers[http_constants.HttpHeaders.Continuation] = options["continuation"]
 
     if options.get("populatePartitionKeyRangeStatistics"):
         headers[http_constants.HttpHeaders.PopulatePartitionKeyRangeStatistics] = options[
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_constants.py` & `azure-cosmos-4.6.1/azure/cosmos/_constants.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_cosmos_client_connection.py` & `azure-cosmos-4.6.1/azure/cosmos/_cosmos_client_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # pylint: disable=too-many-lines, protected-access
 
 """Document client class for the Azure Cosmos database service.
 """
+import os
 import urllib.parse
 from typing import Callable, Dict, Any, Iterable, List, Mapping, Optional, Sequence, Tuple, Union, cast, Type
 from typing_extensions import TypedDict
 
 from urllib3.util.retry import Retry
 from azure.core.credentials import TokenCredential
 from azure.core.paging import ItemPaged
@@ -653,17 +654,17 @@
         self,
         database_link: str,
         options: Optional[Mapping[str, Any]] = None,
         **kwargs: Any
     ) -> ItemPaged[Dict[str, Any]]:
         """Reads all users in a database.
 
-        :params str database_link:
+        :param str database_link:
             The link to the database.
-        :params dict options:
+        :param dict[str, Any] options:
             The request options for the request.
         :return:
             Query iterable of Users.
         :rtype:
             query_iterable.QueryIterable
 
         """
@@ -3103,15 +3104,24 @@
     def _GetQueryPlanThroughGateway(self, query: str, resource_link: str, **kwargs: Any) -> List[Dict[str, Any]]:
         supported_query_features = (documents._QueryFeature.Aggregate + "," +
                                     documents._QueryFeature.CompositeAggregate + "," +
                                     documents._QueryFeature.Distinct + "," +
                                     documents._QueryFeature.MultipleOrderBy + "," +
                                     documents._QueryFeature.OffsetAndLimit + "," +
                                     documents._QueryFeature.OrderBy + "," +
-                                    documents._QueryFeature.Top)
+                                    documents._QueryFeature.Top + "," +
+                                    documents._QueryFeature.NonStreamingOrderBy)
+        if os.environ.get('AZURE_COSMOS_DISABLE_NON_STREAMING_ORDER_BY', False):
+            supported_query_features = (documents._QueryFeature.Aggregate + "," +
+                                        documents._QueryFeature.CompositeAggregate + "," +
+                                        documents._QueryFeature.Distinct + "," +
+                                        documents._QueryFeature.MultipleOrderBy + "," +
+                                        documents._QueryFeature.OffsetAndLimit + "," +
+                                        documents._QueryFeature.OrderBy + "," +
+                                        documents._QueryFeature.Top)
 
         options = {
             "contentType": runtime_constants.MediaTypes.Json,
             "isQueryPlanRequest": True,
             "supportedQueryFeatures": supported_query_features,
             "queryVersion": http_constants.Versions.QueryVersion
         }
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_cosmos_http_logging_policy.py` & `azure-cosmos-4.6.1/azure/cosmos/_cosmos_http_logging_policy.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_cosmos_integers.py` & `azure-cosmos-4.6.1/azure/cosmos/_cosmos_integers.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_cosmos_murmurhash3.py` & `azure-cosmos-4.6.1/azure/cosmos/_cosmos_murmurhash3.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_default_retry_policy.py` & `azure-cosmos-4.6.1/azure/cosmos/_default_retry_policy.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_endpoint_discovery_retry_policy.py` & `azure-cosmos-4.6.1/azure/cosmos/_endpoint_discovery_retry_policy.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_execution_context/__init__.py` & `azure-cosmos-4.6.1/azure/cosmos/_execution_context/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_execution_context/aggregators.py` & `azure-cosmos-4.6.1/azure/cosmos/_execution_context/aggregators.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_execution_context/aio/__init__.py` & `azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_execution_context/aio/_queue_async_helper.py` & `azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/_queue_async_helper.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_execution_context/aio/base_execution_context.py` & `azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/base_execution_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,36 +52,40 @@
 
     def _get_initial_continuation(self):
         if "continuation" in self._options:
             return self._options["continuation"]
         return None
 
     def _has_more_pages(self):
-        return not self._has_started or self._continuation
+        return not self._has_finished
+
+    async def _ensure(self):
+        if not self._has_more_pages():
+            return
+
+        if not self._buffer:
+            results = await self._fetch_next_block()
+            self._buffer.extend(results)
+
+        if not self._buffer:
+            self._has_finished = True
 
     async def fetch_next_block(self):
         """Returns a block of results with respecting retry policy.
 
         This method only exists for backward compatibility reasons. (Because
         QueryIterable has exposed fetch_next_block api).
 
         :return: List of results.
         :rtype: list
         """
-        if not self._has_more_pages():
-            return []
-
-        if self._buffer:
-            # if there is anything in the buffer returns that
-            res = list(self._buffer)
-            self._buffer.clear()
-            return res
-
-        # fetches the next block
-        return await self._fetch_next_block()
+        await self._ensure()
+        res = list(self._buffer)
+        self._buffer.clear()
+        return res
 
     async def _fetch_next_block(self):
         raise NotImplementedError
 
     def __aiter__(self):
         """Returns itself as an iterator
         :returns: Query as an iterator.
@@ -92,50 +96,50 @@
     async def __anext__(self):
         """Return the next query result.
 
         :return: The next query result.
         :rtype: dict
         :raises StopAsyncIteration: If no more result is left.
         """
-        if self._has_finished:
-            raise StopAsyncIteration
-
-        if not self._buffer:
-
-            results = await self.fetch_next_block()
-            self._buffer.extend(results)
+        await self._ensure()
 
         if not self._buffer:
             raise StopAsyncIteration
 
         return self._buffer.popleft()
 
     async def _fetch_items_helper_no_retries(self, fetch_function):
         """Fetches more items and doesn't retry on failure
 
         :param Callable fetch_function: The function that fetches the items.
         :return: List of fetched items.
         :rtype: list
         """
         fetched_items = []
-        # Continues pages till finds a non-empty page or all results are exhausted
+        new_options = copy.deepcopy(self._options)
         while self._continuation or not self._has_started:
-            if not self._has_started:
-                self._has_started = True
-            new_options = copy.deepcopy(self._options)
+            # Check if this is first fetch for read from specific time change feed.
+            # For read specific time the first fetch will return empty even if we have more pages.
+            is_s_time_first_fetch = self._is_change_feed and self._options.get("startTime") and not self._has_started
+
             new_options["continuation"] = self._continuation
 
+            response_headers = {}
             (fetched_items, response_headers) = await fetch_function(new_options)
+            if not self._has_started:
+                self._has_started = True
+
             continuation_key = http_constants.HttpHeaders.Continuation
             # Use Etag as continuation token for change feed queries.
             if self._is_change_feed:
                 continuation_key = http_constants.HttpHeaders.ETag
             # In change feed queries, the continuation token is always populated. The hasNext() test is whether
             # there is any items in the response or not.
-            if not self._is_change_feed or fetched_items:
+            # No initial fetch for start time change feed, so we need to pass continuation token for first fetch
+            if not self._is_change_feed or fetched_items or is_s_time_first_fetch:
                 self._continuation = response_headers.get(continuation_key)
             else:
                 self._continuation = None
             if fetched_items:
                 break
         return fetched_items
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_execution_context/aio/document_producer.py` & `azure-cosmos-4.6.1/azure/cosmos/_execution_context/document_producer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2021 Microsoft Corporation
+# Copyright (c) 2014 Microsoft Corporation
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -23,15 +23,15 @@
 database service.
 """
 
 import numbers
 from collections import deque
 
 from azure.cosmos import _base
-from azure.cosmos._execution_context.aio.base_execution_context import _DefaultQueryExecutionContext
+from azure.cosmos._execution_context.base_execution_context import _DefaultQueryExecutionContext
 
 
 class _DocumentProducer(object):
     """This class takes care of handling of the results for one single partition
     key range.
 
     When handling an orderby query, MultiExecutionContextAggregator instantiates
@@ -53,57 +53,62 @@
         self._has_started = False
         self._cur_item = None
         # initiate execution context
 
         path = _base.GetPathFromLink(collection_link, "docs")
         collection_id = _base.GetResourceIdOrFullNameFromLink(collection_link)
 
-        async def fetch_fn(options):
-            return await self._client.QueryFeed(path, collection_id, query, options, partition_key_target_range["id"])
+        def fetch_fn(options):
+            return self._client.QueryFeed(path, collection_id, query, options, partition_key_target_range["id"])
 
         self._ex_context = _DefaultQueryExecutionContext(client, self._options, fetch_fn)
 
-    def __aiter__(self):
+    def __lt__(self, other):
+        return self._doc_producer_comp.compare(self, other) < 0
+
+    def __iter__(self):
         return self
 
-    async def __anext__(self):
+    def __next__(self):
         """
         :return: The next result item.
         :rtype: dict
         :raises StopIteration: If there is no more result.
 
         """
         if self._cur_item is not None:
             res = self._cur_item
             self._cur_item = None
             return res
 
-        return await self._ex_context.__anext__()
+        return next(self._ex_context)
 
     def get_target_range(self):
         """Returns the target partition key range.
             :return:
                 Target partition key range.
             :rtype: dict
         """
         return self._partition_key_target_range
 
-    async def peek(self):
+    def peek(self):
         """
         TODO: use more_itertools.peekable instead
         :return: The current result item.
         :rtype: dict.
         :raises StopIteration: If there is no current item.
 
         """
         if self._cur_item is None:
-            self._cur_item = await self._ex_context.__anext__()
+            self._cur_item = next(self._ex_context)
 
         return self._cur_item
 
+    next = __next__  # Python 2 compatibility.
+
 
 def _compare_helper(a, b):
     if a is None and b is None:
         return 0
     return (a > b) - (a < b)
 
 
@@ -112,15 +117,15 @@
     Provides a Comparator for document producers using the min value of the
     corresponding target partition.
     """
 
     def __init__(self):
         pass
 
-    async def compare(self, doc_producer1, doc_producer2):
+    def compare(self, doc_producer1, doc_producer2):
         return _compare_helper(
             doc_producer1.get_target_range()["minInclusive"], doc_producer2.get_target_range()["minInclusive"]
         )
 
 
 class _OrderByHelper(object):
 
@@ -171,15 +176,15 @@
             return "Number"
         if isinstance(val, str):
             return "String"
 
         raise TypeError("unknown type" + str(val))
 
     @staticmethod
-    async def compare(orderby_item1, orderby_item2):
+    def compare(orderby_item1, orderby_item2):
         """Compare two orderby item pairs.
 
         :param dict orderby_item1:
         :param dict orderby_item2:
         :return: Integer comparison result.
             The comparator acts such that
             - if the types are different we get:
@@ -213,53 +218,49 @@
     """
 
     def __init__(self, sort_order):  # pylint: disable=super-init-not-called
         """Instantiates this class
 
         :param list sort_order:
             List of sort orders (i.e., Ascending, Descending)
-
-        :ivar list sort_order:
-            List of sort orders (i.e., Ascending, Descending)
-
         """
         self._sort_order = sort_order
 
-    async def compare(self, doc_producer1, doc_producer2):
+    def compare(self, doc_producer1, doc_producer2):
         """Compares the given two instances of DocumentProducers.
 
         Based on the orderby query items and whether the sort order is Ascending
         or Descending compares the peek result of the two DocumentProducers.
 
         If the peek results are equal based on the sort order, this comparator
         compares the target partition key range of the two DocumentProducers.
 
         :param _DocumentProducer doc_producer1: first instance to be compared
         :param _DocumentProducer doc_producer2: second instance to be compared
         :return:
             Integer value of compare result.
-                positive integer if doc_producer1 > doc_producer2
-                negative integer if doc_producer1 < doc_producer2
+                positive integer if doc_producers1 > doc_producers2
+                negative integer if doc_producers1 < doc_producers2
         :rtype: int
         """
 
-        res1 = _peek_order_by_items(await doc_producer1.peek())
-        res2 = _peek_order_by_items(await doc_producer2.peek())
+        res1 = _peek_order_by_items(doc_producer1.peek())
+        res2 = _peek_order_by_items(doc_producer2.peek())
 
         self._validate_orderby_items(res1, res2)
 
         for i, (elt1, elt2) in enumerate(zip(res1, res2)):
-            res = await _OrderByHelper.compare(elt1, elt2)
+            res = _OrderByHelper.compare(elt1, elt2)
             if res != 0:
                 if self._sort_order[i] == "Ascending":
                     return res
                 if self._sort_order[i] == "Descending":
                     return -res
 
-        return await _PartitionKeyRangeDocumentProducerComparator.compare(self, doc_producer1, doc_producer2)
+        return _PartitionKeyRangeDocumentProducerComparator.compare(self, doc_producer1, doc_producer2)
 
     def _validate_orderby_items(self, res1, res2):
         if len(res1) != len(res2):
             # error
             raise ValueError("orderByItems cannot have different size")
 
         if len(res1) != len(self._sort_order):
@@ -267,7 +268,30 @@
             raise ValueError("orderByItems cannot have a different size than sort orders.")
 
         for elt1, elt2 in zip(res1, res2):
             type1 = _OrderByHelper.getTypeStr(elt1)
             type2 = _OrderByHelper.getTypeStr(elt2)
             if type1 != type2:
                 raise ValueError("Expected {}, but got {}.".format(type1, type2))
+
+
+class _NonStreamingItemResultProducer:
+    """This class takes care of handling of the items to be sorted in a non-streaming context.
+
+    One instance of this document producer goes attached to every item coming in for the priority queue to be able
+    to properly sort items as they get inserted.
+    """
+
+    def __init__(self, item_result, sort_order):
+        """
+        Constructor
+        """
+        self._item_result = item_result
+        self._sort_order = sort_order
+
+    def __lt__(self, other):
+        res = _OrderByHelper.compare(self._item_result["orderByItems"][0],
+                                               other._item_result["orderByItems"][0])
+        if res != 0:
+            if self._sort_order[0] == "Descending":
+                res = -res
+        return res < 0
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_execution_context/aio/endpoint_component.py` & `azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/endpoint_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,21 @@
 
     For each processed orderby result it returns 'payload' item of the result.
     """
     async def __anext__(self):
         payload = await self._execution_context.__anext__()
         return payload["payload"]
 
+class _QueryExecutionNonStreamingEndpointComponent(_QueryExecutionEndpointComponent):
+    """Represents an endpoint in handling a non-streaming order by query results.
+    For each processed orderby result it returns the item result.
+    """
+    async def __anext__(self):
+        payload = await self._execution_context.__anext__()
+        return payload._item_result["payload"]
 
 class _QueryExecutionTopEndpointComponent(_QueryExecutionEndpointComponent):
     """Represents an endpoint in handling top query.
 
     It only returns as many results as top arg specified.
     """
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_execution_context/aio/execution_dispatcher.py` & `azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/execution_dispatcher.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Internal class for proxy query execution context implementation in the Azure
 Cosmos database service.
 """
 
-from azure.cosmos._execution_context.aio import endpoint_component
-from azure.cosmos._execution_context.aio import multi_execution_aggregator
+import os
+from azure.cosmos._execution_context.aio import endpoint_component, multi_execution_aggregator
+from azure.cosmos._execution_context.aio import non_streaming_order_by_aggregator
 from azure.cosmos._execution_context.aio.base_execution_context import _QueryExecutionContextBase
 from azure.cosmos._execution_context.aio.base_execution_context import _DefaultQueryExecutionContext
 from azure.cosmos._execution_context.execution_dispatcher import _is_partitioned_execution_info
 from azure.cosmos._execution_context.query_execution_info import _PartitionedQueryExecutionInfo
 from azure.cosmos.documents import _DistinctType
 from azure.cosmos.exceptions import CosmosHttpResponseError
 from azure.cosmos.http_constants import StatusCodes
@@ -103,20 +104,39 @@
         assert self._resource_link, "code bug, resource_link is required."
         if query_execution_info.has_aggregates() and not query_execution_info.has_select_value():
             if self._options and ("enableCrossPartitionQuery" in self._options
                                   and self._options["enableCrossPartitionQuery"]):
                 raise CosmosHttpResponseError(StatusCodes.BAD_REQUEST,
                                   "Cross partition query only supports 'VALUE <AggregateFunc>' for aggregates")
 
-        execution_context_aggregator = multi_execution_aggregator._MultiExecutionContextAggregator(self._client,
+        # throw exception here for vector search query without limit filter or limit > max_limit
+        if query_execution_info.get_non_streaming_order_by():
+            total_item_buffer = query_execution_info.get_top() or\
+                                query_execution_info.get_limit() + query_execution_info.get_offset()
+            if total_item_buffer is None:
+                raise ValueError("Executing a vector search query without TOP or LIMIT can consume many" +
+                                 " RUs very fast and have long runtimes. Please ensure you are using one" +
+                                 " of the two filters with your vector search query.")
+            if total_item_buffer > os.environ.get('AZURE_COSMOS_MAX_ITEM_BUFFER_VECTOR_SEARCH', 50000):
+                raise ValueError("Executing a vector search query with more items than the max is not allowed." +
+                                 "Please ensure you are using a limit smaller than the max, or change the max.")
+            execution_context_aggregator =\
+                non_streaming_order_by_aggregator._NonStreamingOrderByContextAggregator(self._client,
+                                                                                        self._resource_link,
+                                                                                        self._query,
+                                                                                        self._options,
+                                                                                        query_execution_info)
+            await execution_context_aggregator._configure_partition_ranges()
+        else:
+            execution_context_aggregator = multi_execution_aggregator._MultiExecutionContextAggregator(self._client,
                                                                                                    self._resource_link,
                                                                                                    self._query,
                                                                                                    self._options,
                                                                                                    query_execution_info)
-        await execution_context_aggregator._configure_partition_ranges()
+            await execution_context_aggregator._configure_partition_ranges()
         return _PipelineExecutionContext(self._client, self._options, execution_context_aggregator,
                                          query_execution_info)
 
 
 class _PipelineExecutionContext(_QueryExecutionContextBase):  # pylint: disable=abstract-method
 
     DEFAULT_PAGE_SIZE = 1000
@@ -130,15 +150,17 @@
             self._page_size = _PipelineExecutionContext.DEFAULT_PAGE_SIZE
 
         self._execution_context = execution_context
 
         self._endpoint = endpoint_component._QueryExecutionEndpointComponent(execution_context)
 
         order_by = query_execution_info.get_order_by()
-        if order_by:
+        if query_execution_info.get_non_streaming_order_by():
+            self._endpoint = endpoint_component._QueryExecutionNonStreamingEndpointComponent(self._endpoint)
+        elif order_by:
             self._endpoint = endpoint_component._QueryExecutionOrderByEndpointComponent(self._endpoint)
 
         aggregates = query_execution_info.get_aggregates()
         if aggregates:
             self._endpoint = endpoint_component._QueryExecutionAggregateEndpointComponent(self._endpoint, aggregates)
 
         distinct_type = query_execution_info.get_distinct_type()
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py` & `azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/multi_execution_aggregator.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_execution_context/base_execution_context.py` & `azure-cosmos-4.6.1/azure/cosmos/_execution_context/base_execution_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,36 +50,40 @@
 
     def _get_initial_continuation(self):
         if "continuation" in self._options:
             return self._options["continuation"]
         return None
 
     def _has_more_pages(self):
-        return not self._has_started or self._continuation
+        return not self._has_finished
+
+    def _ensure(self):
+        if not self._has_more_pages():
+            return
+
+        if not self._buffer:
+            results = self._fetch_next_block()
+            self._buffer.extend(results)
+
+        if not self._buffer:
+            self._has_finished = True
 
     def fetch_next_block(self):
         """Returns a block of results with respecting retry policy.
 
         This method only exists for backward compatibility reasons. (Because
         QueryIterable has exposed fetch_next_block api).
 
         :return: List of results.
         :rtype: list
         """
-        if not self._has_more_pages():
-            return []
-
-        if self._buffer:
-            # if there is anything in the buffer returns that
-            res = list(self._buffer)
-            self._buffer.clear()
-            return res
-
-        # fetches the next block
-        return self._fetch_next_block()
+        self._ensure()
+        res = list(self._buffer)
+        self._buffer.clear()
+        return res
 
     def _fetch_next_block(self):
         raise NotImplementedError
 
     def __iter__(self):
         """Returns itself as an iterator
         :returns: Query as an iterator.
@@ -90,50 +94,49 @@
     def __next__(self):
         """Return the next query result.
 
         :return: The next query result.
         :rtype: dict
         :raises StopIteration: If no more result is left.
         """
-        if self._has_finished:
-            raise StopIteration
-
-        if not self._buffer:
-
-            results = self.fetch_next_block()
-            self._buffer.extend(results)
+        self._ensure()
 
         if not self._buffer:
             raise StopIteration
 
         return self._buffer.popleft()
 
     def _fetch_items_helper_no_retries(self, fetch_function):
         """Fetches more items and doesn't retry on failure
 
         :param Callable fetch_function: The function that fetches the items.
         :return: List of fetched items.
         :rtype: list
         """
         fetched_items = []
-        # Continues pages till finds a non-empty page or all results are exhausted
+        new_options = copy.deepcopy(self._options)
         while self._continuation or not self._has_started:
+            # Check if this is first fetch for read from specific time change feed.
+            # For read specific time the first fetch will return empty even if we have more pages.
+            is_s_time_first_fetch = self._is_change_feed and self._options.get("startTime") and not self._has_started
             if not self._has_started:
                 self._has_started = True
-            new_options = copy.deepcopy(self._options)
             new_options["continuation"] = self._continuation
 
+            response_headers = {}
             (fetched_items, response_headers) = fetch_function(new_options)
+
             continuation_key = http_constants.HttpHeaders.Continuation
             # Use Etag as continuation token for change feed queries.
             if self._is_change_feed:
                 continuation_key = http_constants.HttpHeaders.ETag
             # In change feed queries, the continuation token is always populated. The hasNext() test is whether
             # there is any items in the response or not.
-            if not self._is_change_feed or fetched_items:
+            # For start time however we get no initial results, so we need to pass continuation token
+            if not self._is_change_feed or fetched_items or is_s_time_first_fetch:
                 self._continuation = response_headers.get(continuation_key)
             else:
                 self._continuation = None
             if fetched_items:
                 break
         return fetched_items
 
@@ -163,10 +166,10 @@
             >>> def result_fn(result):
             >>>     return result['Databases']
 
         """
         super(_DefaultQueryExecutionContext, self).__init__(client, options)
         self._fetch_function = fetch_function
 
-    def _fetch_next_block(self):
+    def _fetch_next_block(self):  # pylint: disable=inconsistent-return-statements
         while super(_DefaultQueryExecutionContext, self)._has_more_pages() and not self._buffer:
             return self._fetch_items_helper_with_retries(self._fetch_function)
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_execution_context/document_producer.py` & `azure-cosmos-4.6.1/azure/cosmos/_execution_context/aio/document_producer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # The MIT License (MIT)
-# Copyright (c) 2014 Microsoft Corporation
+# Copyright (c) 2021 Microsoft Corporation
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -23,16 +23,17 @@
 database service.
 """
 
 import numbers
 from collections import deque
 
 from azure.cosmos import _base
-from azure.cosmos._execution_context.base_execution_context import _DefaultQueryExecutionContext
+from azure.cosmos._execution_context.aio.base_execution_context import _DefaultQueryExecutionContext
 
+# pylint: disable=protected-access
 
 class _DocumentProducer(object):
     """This class takes care of handling of the results for one single partition
     key range.
 
     When handling an orderby query, MultiExecutionContextAggregator instantiates
     one instance of this class per target partition key range and aggregates the
@@ -53,62 +54,57 @@
         self._has_started = False
         self._cur_item = None
         # initiate execution context
 
         path = _base.GetPathFromLink(collection_link, "docs")
         collection_id = _base.GetResourceIdOrFullNameFromLink(collection_link)
 
-        def fetch_fn(options):
-            return self._client.QueryFeed(path, collection_id, query, options, partition_key_target_range["id"])
+        async def fetch_fn(options):
+            return await self._client.QueryFeed(path, collection_id, query, options, partition_key_target_range["id"])
 
         self._ex_context = _DefaultQueryExecutionContext(client, self._options, fetch_fn)
 
-    def __lt__(self, other):
-        return self._doc_producer_comp.compare(self, other) < 0
-
-    def __iter__(self):
+    def __aiter__(self):
         return self
 
-    def __next__(self):
+    async def __anext__(self):
         """
         :return: The next result item.
         :rtype: dict
         :raises StopIteration: If there is no more result.
 
         """
         if self._cur_item is not None:
             res = self._cur_item
             self._cur_item = None
             return res
 
-        return next(self._ex_context)
+        return await self._ex_context.__anext__()
 
     def get_target_range(self):
         """Returns the target partition key range.
             :return:
                 Target partition key range.
             :rtype: dict
         """
         return self._partition_key_target_range
 
-    def peek(self):
+    async def peek(self):
         """
         TODO: use more_itertools.peekable instead
         :return: The current result item.
         :rtype: dict.
         :raises StopIteration: If there is no current item.
 
         """
         if self._cur_item is None:
-            self._cur_item = next(self._ex_context)
+            self._cur_item = await self._ex_context.__anext__()
 
         return self._cur_item
 
-    next = __next__  # Python 2 compatibility.
-
 
 def _compare_helper(a, b):
     if a is None and b is None:
         return 0
     return (a > b) - (a < b)
 
 
@@ -117,15 +113,15 @@
     Provides a Comparator for document producers using the min value of the
     corresponding target partition.
     """
 
     def __init__(self):
         pass
 
-    def compare(self, doc_producer1, doc_producer2):
+    async def compare(self, doc_producer1, doc_producer2):
         return _compare_helper(
             doc_producer1.get_target_range()["minInclusive"], doc_producer2.get_target_range()["minInclusive"]
         )
 
 
 class _OrderByHelper(object):
 
@@ -176,15 +172,15 @@
             return "Number"
         if isinstance(val, str):
             return "String"
 
         raise TypeError("unknown type" + str(val))
 
     @staticmethod
-    def compare(orderby_item1, orderby_item2):
+    async def compare(orderby_item1, orderby_item2):
         """Compare two orderby item pairs.
 
         :param dict orderby_item1:
         :param dict orderby_item2:
         :return: Integer comparison result.
             The comparator acts such that
             - if the types are different we get:
@@ -225,46 +221,46 @@
 
         :ivar list sort_order:
             List of sort orders (i.e., Ascending, Descending)
 
         """
         self._sort_order = sort_order
 
-    def compare(self, doc_producer1, doc_producer2):
+    async def compare(self, doc_producer1, doc_producer2):
         """Compares the given two instances of DocumentProducers.
 
         Based on the orderby query items and whether the sort order is Ascending
         or Descending compares the peek result of the two DocumentProducers.
 
         If the peek results are equal based on the sort order, this comparator
         compares the target partition key range of the two DocumentProducers.
 
         :param _DocumentProducer doc_producer1: first instance to be compared
         :param _DocumentProducer doc_producer2: second instance to be compared
         :return:
             Integer value of compare result.
-                positive integer if doc_producers1 > doc_producers2
-                negative integer if doc_producers1 < doc_producers2
+                positive integer if doc_producer1 > doc_producer2
+                negative integer if doc_producer1 < doc_producer2
         :rtype: int
         """
 
-        res1 = _peek_order_by_items(doc_producer1.peek())
-        res2 = _peek_order_by_items(doc_producer2.peek())
+        res1 = _peek_order_by_items(await doc_producer1.peek())
+        res2 = _peek_order_by_items(await doc_producer2.peek())
 
         self._validate_orderby_items(res1, res2)
 
         for i, (elt1, elt2) in enumerate(zip(res1, res2)):
-            res = _OrderByHelper.compare(elt1, elt2)
+            res = await _OrderByHelper.compare(elt1, elt2)
             if res != 0:
                 if self._sort_order[i] == "Ascending":
                     return res
                 if self._sort_order[i] == "Descending":
                     return -res
 
-        return _PartitionKeyRangeDocumentProducerComparator.compare(self, doc_producer1, doc_producer2)
+        return await _PartitionKeyRangeDocumentProducerComparator.compare(self, doc_producer1, doc_producer2)
 
     def _validate_orderby_items(self, res1, res2):
         if len(res1) != len(res2):
             # error
             raise ValueError("orderByItems cannot have different size")
 
         if len(res1) != len(self._sort_order):
@@ -272,7 +268,55 @@
             raise ValueError("orderByItems cannot have a different size than sort orders.")
 
         for elt1, elt2 in zip(res1, res2):
             type1 = _OrderByHelper.getTypeStr(elt1)
             type2 = _OrderByHelper.getTypeStr(elt2)
             if type1 != type2:
                 raise ValueError("Expected {}, but got {}.".format(type1, type2))
+
+class _NonStreamingItemResultProducer:
+    """This class takes care of handling of the items to be sorted in a non-streaming context.
+    One instance of this document producer goes attached to every item coming in for the priority queue to be able
+    to properly sort items as they get inserted.
+    """
+
+    def __init__(self, item_result, sort_order):
+        """
+        Constructor
+        :param dict[str, Any] item_result: The item result extracted from the document producer
+        :param list[str] sort_order: List of sort orders (i.e., Ascending, Descending)
+        """
+        self._item_result = item_result
+        self._doc_producer_comp = _NonStreamingOrderByComparator(sort_order)
+
+
+
+class _NonStreamingOrderByComparator(object):
+    """Provide a Comparator for item results which respects orderby sort order.
+    """
+
+    def __init__(self, sort_order):
+        """Instantiates this class
+        :param list sort_order:
+            List of sort orders (i.e., Ascending, Descending)
+        """
+        self._sort_order = sort_order
+
+    async def compare(self, doc_producer1, doc_producer2):
+        """Compares the given two instances of DocumentProducers.
+        Based on the orderby query items and whether the sort order is Ascending
+        or Descending compares the peek result of the two DocumentProducers.
+        :param _DocumentProducer doc_producer1: first instance to be compared
+        :param _DocumentProducer doc_producer2: second instance to be compared
+        :return:
+            Integer value of compare result.
+                positive integer if doc_producers1 > doc_producers2
+                negative integer if doc_producers1 < doc_producers2
+        :rtype: int
+        """
+        rank1 = doc_producer1._item_result["orderByItems"][0]
+        rank2 = doc_producer2._item_result["orderByItems"][0]
+        res = await _OrderByHelper.compare(rank1, rank2)
+        if res != 0:
+            if self._sort_order[0] == "Descending":
+                return -res
+        return res
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_execution_context/endpoint_component.py` & `azure-cosmos-4.6.1/azure/cosmos/_execution_context/endpoint_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,22 @@
     For each processed orderby result it returns 'payload' item of the result.
     """
     def __next__(self):
         return next(self._execution_context)["payload"]
 
     next = __next__  # Python 2 compatibility.
 
+class _QueryExecutionNonStreamingEndpointComponent(_QueryExecutionEndpointComponent):
+    """Represents an endpoint in handling a non-streaming order by query results.
+
+    For each processed orderby result it returns the item result.
+    """
+    def __next__(self):
+        return next(self._execution_context)._item_result["payload"]  # pylint: disable=protected-access
+
 
 class _QueryExecutionTopEndpointComponent(_QueryExecutionEndpointComponent):
     """Represents an endpoint in handling top query.
 
     It only returns as many results as top arg specified.
     """
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_execution_context/execution_dispatcher.py` & `azure-cosmos-4.6.1/azure/cosmos/_execution_context/execution_dispatcher.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,20 +20,21 @@
 # SOFTWARE.
 
 """Internal class for proxy query execution context implementation in the Azure
 Cosmos database service.
 """
 
 import json
+import os
 from azure.cosmos.exceptions import CosmosHttpResponseError
-from azure.cosmos._execution_context import multi_execution_aggregator
+from azure.cosmos._execution_context import endpoint_component, multi_execution_aggregator
+from azure.cosmos._execution_context import non_streaming_order_by_aggregator
 from azure.cosmos._execution_context.base_execution_context import _QueryExecutionContextBase
 from azure.cosmos._execution_context.base_execution_context import _DefaultQueryExecutionContext
 from azure.cosmos._execution_context.query_execution_info import _PartitionedQueryExecutionInfo
-from azure.cosmos._execution_context import endpoint_component
 from azure.cosmos.documents import _DistinctType
 from azure.cosmos.http_constants import StatusCodes, SubStatusCodes
 
 # pylint: disable=protected-access
 
 
 def _is_partitioned_execution_info(e):
@@ -107,23 +108,39 @@
                 self._execution_context = self._create_pipelined_execution_context(query_execution_info)
             else:
                 raise e
 
         return self._execution_context.fetch_next_block()
 
     def _create_pipelined_execution_context(self, query_execution_info):
-
         assert self._resource_link, "code bug, resource_link is required."
         if query_execution_info.has_aggregates() and not query_execution_info.has_select_value():
             if self._options and ("enableCrossPartitionQuery" in self._options
                                   and self._options["enableCrossPartitionQuery"]):
                 raise CosmosHttpResponseError(StatusCodes.BAD_REQUEST,
                                   "Cross partition query only supports 'VALUE <AggregateFunc>' for aggregates")
 
-        execution_context_aggregator = multi_execution_aggregator._MultiExecutionContextAggregator(self._client,
+        # throw exception here for vector search query without limit filter or limit > max_limit
+        if query_execution_info.get_non_streaming_order_by():
+            total_item_number = query_execution_info.get_top() or query_execution_info.get_limit()
+            if total_item_number is None:
+                raise ValueError("Executing a vector search query without TOP or LIMIT can consume many" +
+                                 " RUs very fast and have long runtimes. Please ensure you are using one" +
+                                 " of the two filters with your vector search query.")
+            if total_item_number > os.environ.get('AZURE_COSMOS_MAX_ITEM_BUFFER_VECTOR_SEARCH', 50000):
+                raise ValueError("Executing a vector search query with more items than the max is not allowed." +
+                                 "Please ensure you are using a limit smaller than the max, or change the max.")
+            execution_context_aggregator =\
+                non_streaming_order_by_aggregator._NonStreamingOrderByContextAggregator(self._client,
+                                                                                        self._resource_link,
+                                                                                        self._query,
+                                                                                        self._options,
+                                                                                        query_execution_info)
+        else:
+            execution_context_aggregator = multi_execution_aggregator._MultiExecutionContextAggregator(self._client,
                                                                                                    self._resource_link,
                                                                                                    self._query,
                                                                                                    self._options,
                                                                                                    query_execution_info)
         return _PipelineExecutionContext(self._client, self._options, execution_context_aggregator,
                                          query_execution_info)
 
@@ -143,15 +160,17 @@
             self._page_size = _PipelineExecutionContext.DEFAULT_PAGE_SIZE
 
         self._execution_context = execution_context
 
         self._endpoint = endpoint_component._QueryExecutionEndpointComponent(execution_context)
 
         order_by = query_execution_info.get_order_by()
-        if order_by:
+        if query_execution_info.get_non_streaming_order_by():
+            self._endpoint = endpoint_component._QueryExecutionNonStreamingEndpointComponent(self._endpoint)
+        elif order_by:
             self._endpoint = endpoint_component._QueryExecutionOrderByEndpointComponent(self._endpoint)
 
         aggregates = query_execution_info.get_aggregates()
         if aggregates:
             self._endpoint = endpoint_component._QueryExecutionAggregateEndpointComponent(self._endpoint, aggregates)
 
         distinct_type = query_execution_info.get_distinct_type()
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_execution_context/multi_execution_aggregator.py` & `azure-cosmos-4.6.1/azure/cosmos/_execution_context/multi_execution_aggregator.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_execution_context/query_execution_info.py` & `azure-cosmos-4.6.1/azure/cosmos/_execution_context/query_execution_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     OffsetPath = [QueryInfoPath, "offset"]
     LimitPath = [QueryInfoPath, "limit"]
     DistinctTypePath = [QueryInfoPath, "distinctType"]
     OrderByPath = [QueryInfoPath, "orderBy"]
     AggregatesPath = [QueryInfoPath, "aggregates"]
     QueryRangesPath = "queryRanges"
     RewrittenQueryPath = [QueryInfoPath, "rewrittenQuery"]
+    HasNonStreamingOrderByPath = [QueryInfoPath, "hasNonStreamingOrderBy"]
 
     def __init__(self, query_execution_info):
         """
         :param dict query_execution_info:
         """
         self._query_execution_info = query_execution_info
 
@@ -103,14 +104,21 @@
         """
         rewrittenQuery = self._extract(_PartitionedQueryExecutionInfo.RewrittenQueryPath)
         if rewrittenQuery is not None:
             # Hardcode formattable filter to true for now
             rewrittenQuery = rewrittenQuery.replace("{documentdb-formattableorderbyquery-filter}", "true")
         return rewrittenQuery
 
+    def get_non_streaming_order_by(self):
+        """Returns if the query is a non-streaming order by query.
+        :returns: Query is a non-streaming order by query.
+        :rtype: bool
+        """
+        return self._extract(_PartitionedQueryExecutionInfo.HasNonStreamingOrderByPath)
+
     def has_select_value(self):
         return self._extract(self.HasSelectValue)
 
     def has_top(self):
         return self.get_top() is not None
 
     def has_limit(self):
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_global_endpoint_manager.py` & `azure-cosmos-4.6.1/azure/cosmos/_global_endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_gone_retry_policy.py` & `azure-cosmos-4.6.1/azure/cosmos/_gone_retry_policy.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_location_cache.py` & `azure-cosmos-4.6.1/azure/cosmos/_location_cache.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_partition.py` & `azure-cosmos-4.6.1/azure/cosmos/_partition.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_query_iterable.py` & `azure-cosmos-4.6.1/azure/cosmos/_query_iterable.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_range.py` & `azure-cosmos-4.6.1/azure/cosmos/_range.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_range_partition_resolver.py` & `azure-cosmos-4.6.1/azure/cosmos/_range_partition_resolver.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_request_object.py` & `azure-cosmos-4.6.1/azure/cosmos/_request_object.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_resource_throttle_retry_policy.py` & `azure-cosmos-4.6.1/azure/cosmos/_resource_throttle_retry_policy.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_retry_options.py` & `azure-cosmos-4.6.1/azure/cosmos/_retry_options.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_retry_utility.py` & `azure-cosmos-4.6.1/azure/cosmos/_retry_utility.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_routing/__init__.py` & `azure-cosmos-4.6.1/azure/cosmos/_routing/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_routing/aio/__init__.py` & `azure-cosmos-4.6.1/azure/cosmos/_routing/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_routing/aio/routing_map_provider.py` & `azure-cosmos-4.6.1/azure/cosmos/_routing/aio/routing_map_provider.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_routing/collection_routing_map.py` & `azure-cosmos-4.6.1/azure/cosmos/_routing/collection_routing_map.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_routing/routing_map_provider.py` & `azure-cosmos-4.6.1/azure/cosmos/_routing/routing_map_provider.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_routing/routing_range.py` & `azure-cosmos-4.6.1/azure/cosmos/_routing/routing_range.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_runtime_constants.py` & `azure-cosmos-4.6.1/azure/cosmos/_runtime_constants.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_session.py` & `azure-cosmos-4.6.1/azure/cosmos/_session.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_session_retry_policy.py` & `azure-cosmos-4.6.1/azure/cosmos/_session_retry_policy.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_synchronized_request.py` & `azure-cosmos-4.6.1/azure/cosmos/_synchronized_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Synchronized request in the Azure Cosmos database service.
 """
-
+import copy
 import json
 import time
 
 from urllib.parse import urlparse
 from azure.core.exceptions import DecodeError  # type: ignore
 
 from . import exceptions
@@ -135,15 +135,15 @@
             connection_timeout=connection_timeout,
             # If SSL is disabled, verify = false
             connection_verify=kwargs.pop("connection_verify", is_ssl_enabled),
             **kwargs
         )
 
     response = response.http_response
-    headers = dict(response.headers)
+    headers = copy.copy(response.headers)
 
     data = response.body()
     if data:
         data = data.decode("utf-8")
 
     if response.status_code == 404:
         raise exceptions.CosmosResourceNotFoundError(message=data, response=response)
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_timeout_failover_retry_policy.py` & `azure-cosmos-4.6.1/azure/cosmos/_timeout_failover_retry_policy.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_utils.py` & `azure-cosmos-4.6.1/azure/cosmos/_utils.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_vector_session_token.py` & `azure-cosmos-4.6.1/azure/cosmos/_vector_session_token.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/_version.py` & `azure-cosmos-4.6.1/azure/cosmos/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-VERSION = "4.6.0"
+VERSION = "4.6.1"
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/aio/__init__.py` & `azure-cosmos-4.6.1/azure/cosmos/aio/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/aio/_asynchronous_request.py` & `azure-cosmos-4.6.1/azure/cosmos/aio/_asynchronous_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Asynchronous request in the Azure Cosmos database service.
 """
-
+import copy
 import json
 import time
 
 from urllib.parse import urlparse
 from azure.core.exceptions import DecodeError  # type: ignore
 
 from .. import exceptions
@@ -103,15 +103,15 @@
             connection_timeout=connection_timeout,
             # If SSL is disabled, verify = false
             connection_verify=kwargs.pop("connection_verify", is_ssl_enabled),
             **kwargs
         )
 
     response = response.http_response
-    headers = dict(response.headers)
+    headers = copy.copy(response.headers)
 
     data = response.body()
     if data:
         data = data.decode("utf-8")
 
     if response.status_code == 404:
         raise exceptions.CosmosResourceNotFoundError(message=data, response=response)
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/aio/_auth_policy_async.py` & `azure-cosmos-4.6.1/azure/cosmos/aio/_auth_policy_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/aio/_container.py` & `azure-cosmos-4.6.1/azure/cosmos/aio/_container.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Create, read, update and delete items in the Azure Cosmos DB SQL API service.
 """
-
+from datetime import datetime, timezone
 from typing import Any, Dict, Mapping, Optional, Sequence, Type, Union, List, Tuple, cast
 from typing_extensions import Literal
 
 from azure.core import MatchConditions
 from azure.core.async_paging import AsyncItemPaged
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.tracing.decorator_async import distributed_trace_async  # type: ignore
@@ -456,15 +456,15 @@
         if continuation_token_limit is not None:
             feed_options["responseContinuationTokenLimitInKb"] = continuation_token_limit
         if hasattr(response_hook, "clear"):
             response_hook.clear()
 
         items = self.client_connection.QueryItems(
             database_or_container_link=self.container_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             partition_key=partition_key,
             response_hook=response_hook,
             **kwargs
         )
         if response_hook:
             response_hook(self.client_connection.last_response_headers, items)
@@ -472,24 +472,27 @@
 
     @distributed_trace
     def query_items_change_feed(
         self,
         *,
         partition_key_range_id: Optional[str] = None,
         is_start_from_beginning: bool = False,
+        start_time: Optional[datetime] = None,
         continuation: Optional[str] = None,
         max_item_count: Optional[int] = None,
         partition_key: Optional[PartitionKeyType] = None,
         priority: Optional[Literal["High", "Low"]] = None,
         **kwargs: Any
     ) -> AsyncItemPaged[Dict[str, Any]]:
         """Get a sorted list of items that were changed, in the order in which they were modified.
 
         :keyword bool is_start_from_beginning: Get whether change feed should start from
             beginning (true) or from current (false). By default, it's start from current (false).
+        :keyword ~datetime.datetime start_time: Specifies a point of time to start change feed. Provided value will be
+            converted to UTC. This value will be ignored if `is_start_from_beginning` is set to true.
         :keyword str partition_key_range_id: ChangeFeed requests can be executed against specific partition key
             ranges. This is used to process the change feed in parallel across multiple consumers.
         :keyword str continuation: e_tag value to be used as continuation for reading change feed.
         :keyword int max_item_count: Max number of items to be returned in the enumeration operation.
         :keyword partition_key: partition key at which ChangeFeed requests are targeted.
         :paramtype partition_key: Union[str, int, float, bool, List[Union[str, int, float, bool]]]
         :keyword response_hook: A callable invoked with the response metadata.
@@ -501,14 +504,16 @@
         :rtype: AsyncItemPaged[Dict[str, Any]]
         """
         response_hook = kwargs.pop('response_hook', None)
         if priority is not None:
             kwargs['priority'] = priority
         feed_options = _build_options(kwargs)
         feed_options["isStartFromBeginning"] = is_start_from_beginning
+        if start_time is not None and is_start_from_beginning is False:
+            feed_options["startTime"] = start_time.astimezone(timezone.utc).strftime('%a, %d %b %Y %H:%M:%S GMT')
         if partition_key_range_id is not None:
             feed_options["partitionKeyRangeId"] = partition_key_range_id
         if partition_key is not None:
             feed_options["partitionKey"] = self._set_partition_key(partition_key)
         if max_item_count is not None:
             feed_options["maxItemCount"] = max_item_count
         if continuation is not None:
@@ -902,15 +907,15 @@
         if partition_key is not None:
             feed_options["partitionKey"] = self._set_partition_key(partition_key)
         else:
             feed_options["enableCrossPartitionQuery"] = True
 
         result = self.client_connection.QueryConflicts(
             collection_link=self.container_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             **kwargs
         )
         if response_hook:
             response_hook(self.client_connection.last_response_headers, result)
         return result
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/aio/_cosmos_client.py` & `azure-cosmos-4.6.1/azure/cosmos/aio/_cosmos_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
         if etag is not None:
             kwargs["etag"] = etag
         if match_condition is not None:
             kwargs["match_condition"] = match_condition
         request_options = _build_options(kwargs)
         _set_throughput_options(offer=offer_throughput, request_options=request_options)
 
-        result = await self.client_connection.CreateDatabase(database=dict(id=id), options=request_options, **kwargs)
+        result = await self.client_connection.CreateDatabase(database={"id": id}, options=request_options, **kwargs)
         return DatabaseProxy(self.client_connection, id=result["id"], properties=result)
 
     @distributed_trace_async
     async def create_database_if_not_exists(  # pylint: disable=redefined-builtin
         self,
         id: str,
         *,
@@ -422,15 +422,15 @@
         if initial_headers is not None:
             kwargs["initial_headers"] = initial_headers
         feed_options = _build_options(kwargs)
         if max_item_count is not None:
             feed_options["maxItemCount"] = max_item_count
 
         result = self.client_connection.QueryDatabases(
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             **kwargs)
         if response_hook:
             response_hook(self.client_connection.last_response_headers)
         return result
 
     @distributed_trace_async
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/aio/_cosmos_client_connection_async.py` & `azure-cosmos-4.6.1/azure/cosmos/aio/_cosmos_client_connection_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 # pylint: disable=protected-access,too-many-lines
 
 """Document client class for the Azure Cosmos database service.
 """
+import os
 from urllib.parse import urlparse
 from typing import (
     Callable, Dict, Any, Iterable, Mapping, Optional, List,
     Sequence, Tuple, Type, Union, cast
 )
 
 from typing_extensions import TypedDict
@@ -2331,17 +2332,17 @@
         self,
         database_link: str,
         options: Optional[Mapping[str, Any]] = None,
         **kwargs: Any
     ) -> AsyncItemPaged[Dict[str, Any]]:
         """Reads all users in a database.
 
-        :params str database_link:
+        :param str database_link:
             The link to the database.
-        :params dict options:
+        :param dict[str, Any] options:
             The request options for the request.
         :return:
             Query iterable of Users.
         :rtype:
             query_iterable.QueryIterable
 
         """
@@ -3108,15 +3109,24 @@
     async def _GetQueryPlanThroughGateway(self, query: str, resource_link: str, **kwargs) -> List[Dict[str, Any]]:
         supported_query_features = (documents._QueryFeature.Aggregate + "," +
                                     documents._QueryFeature.CompositeAggregate + "," +
                                     documents._QueryFeature.Distinct + "," +
                                     documents._QueryFeature.MultipleOrderBy + "," +
                                     documents._QueryFeature.OffsetAndLimit + "," +
                                     documents._QueryFeature.OrderBy + "," +
-                                    documents._QueryFeature.Top)
+                                    documents._QueryFeature.Top + "," +
+                                    documents._QueryFeature.NonStreamingOrderBy)
+        if os.environ.get('AZURE_COSMOS_DISABLE_NON_STREAMING_ORDER_BY', False):
+            supported_query_features = (documents._QueryFeature.Aggregate + "," +
+                                        documents._QueryFeature.CompositeAggregate + "," +
+                                        documents._QueryFeature.Distinct + "," +
+                                        documents._QueryFeature.MultipleOrderBy + "," +
+                                        documents._QueryFeature.OffsetAndLimit + "," +
+                                        documents._QueryFeature.OrderBy + "," +
+                                        documents._QueryFeature.Top)
 
         options = {
             "contentType": runtime_constants.MediaTypes.Json,
             "isQueryPlanRequest": True,
             "supportedQueryFeatures": supported_query_features,
             "queryVersion": http_constants.Versions.QueryVersion
         }
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/aio/_database.py` & `azure-cosmos-4.6.1/azure/cosmos/aio/_database.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,15 @@
         unique_key_policy: Optional[Dict[str, str]] = None,
         conflict_resolution_policy: Optional[Dict[str, str]] = None,
         session_token: Optional[str] = None,
         initial_headers: Optional[Dict[str, str]] = None,
         etag: Optional[str] = None,
         match_condition: Optional[MatchConditions] = None,
         analytical_storage_ttl: Optional[int] = None,
+        vector_embedding_policy: Optional[Dict[str, Any]] = None,
         **kwargs: Any
     ) -> ContainerProxy:
         """Create a new container with the given ID (name).
 
         If a container with the given ID already exists, a CosmosResourceExistsError is raised.
 
         :param str id: ID (name) of container to create.
@@ -198,14 +199,17 @@
             container in the Azure Cosmos DB Service. For more Information on how to use computed properties visit
             `here: https://learn.microsoft.com/en-us/azure/cosmos-db/nosql/query/computed-properties?tabs=dotnet`
         :keyword response_hook: A callable invoked with the response metadata.
         :paramtype response_hook: Callable[[Dict[str, str], Dict[str, Any]], None]
         :keyword int analytical_storage_ttl: Analytical store time to live (TTL) for items in the container.  A value of
             None leaves analytical storage off and a value of -1 turns analytical storage on with no TTL. Please
             note that analytical storage can only be enabled on Synapse Link enabled accounts.
+        :keyword Dict[str, Any] vector_embedding_policy: The vector embedding policy for the container. Each vector
+            embedding possesses a predetermined number of dimensions, is associated with an underlying data type, and
+            is generated for a particular distance function.
         :raises ~azure.cosmos.exceptions.CosmosHttpResponseError: The container creation failed.
         :returns: A `ContainerProxy` instance representing the new container.
         :rtype: ~azure.cosmos.aio.ContainerProxy
 
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/examples_async.py
@@ -220,15 +224,15 @@
                 :start-after: [START create_container_with_settings]
                 :end-before: [END create_container_with_settings]
                 :language: python
                 :dedent: 0
                 :caption: Create a container with specific settings; in this case, a custom partition key:
                 :name: create_container_with_settings
         """
-        definition: Dict[str, Any] = dict(id=id)
+        definition: Dict[str, Any] = {"id": id}
         if partition_key is not None:
             definition["partitionKey"] = partition_key
         if indexing_policy is not None:
             if indexing_policy.get("indexingMode") is IndexingMode.Lazy:
                 warnings.warn(
                     "Lazy indexing mode has been deprecated. Mode will be set to consistent indexing by the backend.",
                     DeprecationWarning
@@ -239,16 +243,18 @@
         if unique_key_policy is not None:
             definition["uniqueKeyPolicy"] = unique_key_policy
         if conflict_resolution_policy is not None:
             definition["conflictResolutionPolicy"] = conflict_resolution_policy
         if analytical_storage_ttl is not None:
             definition["analyticalStorageTtl"] = analytical_storage_ttl
         computed_properties = kwargs.pop('computed_properties', None)
-        if computed_properties:
+        if computed_properties is not None:
             definition["computedProperties"] = computed_properties
+        if vector_embedding_policy is not None:
+            definition["vectorEmbeddingPolicy"] = vector_embedding_policy
 
         if session_token is not None:
             kwargs['session_token'] = session_token
         if initial_headers is not None:
             kwargs['initial_headers'] = initial_headers
         if etag is not None:
             kwargs['etag'] = etag
@@ -274,14 +280,15 @@
         unique_key_policy: Optional[Dict[str, str]] = None,
         conflict_resolution_policy: Optional[Dict[str, str]] = None,
         session_token: Optional[str] = None,
         initial_headers: Optional[Dict[str, str]] = None,
         etag: Optional[str] = None,
         match_condition: Optional[MatchConditions] = None,
         analytical_storage_ttl: Optional[int] = None,
+        vector_embedding_policy: Optional[Dict[str, Any]] = None,
         **kwargs: Any
     ) -> ContainerProxy:
         """Create a container if it does not exist already.
 
         If the container already exists, the existing settings are returned.
         Note: it does not check or update the existing container settings or offer throughput
         if they differ from what was passed into the method.
@@ -306,14 +313,17 @@
             container in the Azure Cosmos DB Service. For more Information on how to use computed properties visit
             `here: https://learn.microsoft.com/en-us/azure/cosmos-db/nosql/query/computed-properties?tabs=dotnet`
         :keyword response_hook: A callable invoked with the response metadata.
         :paramtype response_hook: Callable[[Dict[str, str], Dict[str, Any]], None]
         :keyword int analytical_storage_ttl: Analytical store time to live (TTL) for items in the container.  A value of
             None leaves analytical storage off and a value of -1 turns analytical storage on with no TTL. Please
             note that analytical storage can only be enabled on Synapse Link enabled accounts.
+        :keyword Dict[str, Any] vector_embedding_policy: **provisional** The vector embedding policy for the container.
+            Each vector embedding possesses a predetermined number of dimensions, is associated with an underlying
+            data type, and is generated for a particular distance function.
         :raises ~azure.cosmos.exceptions.CosmosHttpResponseError: The container creation failed.
         :returns: A `ContainerProxy` instance representing the new container.
         :rtype: ~azure.cosmos.aio.ContainerProxy
         """
         computed_properties = kwargs.pop("computed_properties", None)
         try:
             container_proxy = self.get_container_client(id)
@@ -334,14 +344,15 @@
                 conflict_resolution_policy=conflict_resolution_policy,
                 analytical_storage_ttl=analytical_storage_ttl,
                 computed_properties=computed_properties,
                 etag=etag,
                 match_condition=match_condition,
                 session_token=session_token,
                 initial_headers=initial_headers,
+                vector_embedding_policy=vector_embedding_policy,
                 **kwargs
             )
 
     def get_container_client(self, container: Union[str, ContainerProxy, Dict[str, Any]]) -> ContainerProxy:
         """Get a `ContainerProxy` for a container with specified ID (name).
 
         :param container: The ID (name), dict representing the properties, or :class:`ContainerProxy`
@@ -422,15 +433,15 @@
         session_token: Optional[str] = None,
         max_item_count: Optional[int] = None,
         initial_headers: Optional[Dict[str, str]] = None,
         **kwargs: Any
     ) -> AsyncItemPaged[Dict[str, Any]]:
         """List the properties for containers in the current database.
 
-        :keyword Union[str, Dict[str, Any]] query: The Azure Cosmos DB SQL query to execute.
+        :param str query: The Azure Cosmos DB SQL query to execute.
         :keyword parameters: Optional array of parameters to the query.
             Each parameter is a dict() with 'name' and 'value' keys.
         :paramtype parameters: Optional[List[Dict[str, Any]]]
         :keyword int max_item_count: Max number of items to be returned in the enumeration operation.
         :keyword str session_token: Token for use with Session consistency.
         :keyword dict[str, str] initial_headers: Initial headers to be sent as part of the request.
         :keyword response_hook: A callable invoked with the response metadata.
@@ -445,15 +456,15 @@
             kwargs['initial_headers'] = initial_headers
         feed_options = _build_options(kwargs)
         if max_item_count is not None:
             feed_options["maxItemCount"] = max_item_count
 
         result = self.client_connection.QueryContainers(
             database_link=self.database_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             **kwargs
         )
         if response_hook:
             response_hook(self.client_connection.last_response_headers, result)
         return result
 
@@ -696,15 +707,15 @@
         feed_options = _build_options(kwargs)
         response_hook = kwargs.pop('response_hook', None)
         if max_item_count is not None:
             feed_options["maxItemCount"] = max_item_count
 
         result = self.client_connection.QueryUsers(
             database_link=self.database_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             **kwargs
         )
         if response_hook:
             response_hook(self.client_connection.last_response_headers, result)
         return result
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/aio/_global_endpoint_manager_async.py` & `azure-cosmos-4.6.1/azure/cosmos/aio/_global_endpoint_manager_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/aio/_query_iterable_async.py` & `azure-cosmos-4.6.1/azure/cosmos/aio/_query_iterable_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/aio/_retry_utility_async.py` & `azure-cosmos-4.6.1/azure/cosmos/aio/_retry_utility_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/aio/_scripts.py` & `azure-cosmos-4.6.1/azure/cosmos/aio/_scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         """
         feed_options = _build_options(kwargs)
         if max_item_count is not None:
             feed_options["maxItemCount"] = max_item_count
 
         return self.client_connection.QueryStoredProcedures(
             collection_link=self.container_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             **kwargs
         )
 
     @distributed_trace_async
     async def get_stored_procedure(self, sproc: Union[str, Mapping[str, Any]], **kwargs: Any) -> Dict[str, Any]:
         """Get the stored procedure identified by `sproc`.
@@ -278,15 +278,15 @@
         :rtype: AsyncItemPaged[Dict[str, Any]]
         """
         feed_options = _build_options(kwargs)
         if max_item_count is not None:
             feed_options["maxItemCount"] = max_item_count
         return self.client_connection.QueryTriggers(
             collection_link=self.container_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             **kwargs
         )
 
     @distributed_trace_async
     async def get_trigger(self, trigger: Union[str, Mapping[str, Any]], **kwargs: Any) -> Dict[str, Any]:
         """Get a trigger identified by `id`.
@@ -404,15 +404,15 @@
         """
         feed_options = _build_options(kwargs)
         if max_item_count is not None:
             feed_options["maxItemCount"] = max_item_count
 
         return self.client_connection.QueryUserDefinedFunctions(
             collection_link=self.container_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             **kwargs
         )
 
     @distributed_trace_async
     async def get_user_defined_function(self, udf: Union[str, Mapping[str, Any]], **kwargs: Any) -> Dict[str, Any]:
         """Get a user-defined function identified by `id`.
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/aio/_user.py` & `azure-cosmos-4.6.1/azure/cosmos/aio/_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         feed_options = build_options(kwargs)
         response_hook = kwargs.pop('response_hook', None)
         if max_item_count is not None:
             feed_options["maxItemCount"] = max_item_count
 
         result = self.client_connection.QueryPermissions(
             user_link=self.user_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             **kwargs
         )
 
         if response_hook:
             response_hook(self.client_connection.last_response_headers, result)
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/auth.py` & `azure-cosmos-4.6.1/azure/cosmos/auth.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/container.py` & `azure-cosmos-4.6.1/azure/cosmos/container.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 """Create, read, update and delete items in the Azure Cosmos DB SQL API service.
 """
-
+from datetime import datetime, timezone
 import warnings
 from typing import Any, Dict, List, Optional, Sequence, Union, Tuple, Mapping, Type, cast
 from typing_extensions import Literal
 
 from azure.core import MatchConditions
 from azure.core.tracing.decorator import distributed_trace
 from azure.core.paging import ItemPaged
@@ -306,27 +306,30 @@
     def query_items_change_feed(
         self,
         partition_key_range_id: Optional[str] = None,
         is_start_from_beginning: bool = False,
         continuation: Optional[str] = None,
         max_item_count: Optional[int] = None,
         *,
+        start_time: Optional[datetime] = None,
         partition_key: Optional[PartitionKeyType] = None,
         priority: Optional[Literal["High", "Low"]] = None,
         **kwargs: Any
     ) -> ItemPaged[Dict[str, Any]]:
         """Get a sorted list of items that were changed, in the order in which they were modified.
 
         :param str partition_key_range_id: ChangeFeed requests can be executed against specific partition key ranges.
             This is used to process the change feed in parallel across multiple consumers.
         :param bool is_start_from_beginning: Get whether change feed should start from
             beginning (true) or from current (false). By default, it's start from current (false).
         :param max_item_count: Max number of items to be returned in the enumeration operation.
         :param str continuation: e_tag value to be used as continuation for reading change feed.
         :param int max_item_count: Max number of items to be returned in the enumeration operation.
+        :keyword ~datetime.datetime start_time: Specifies a point of time to start change feed. Provided value will be
+            converted to UTC. This value will be ignored if `is_start_from_beginning` is set to true.
         :keyword partition_key: partition key at which ChangeFeed requests are targeted.
         :paramtype partition_key: Union[str, int, float, bool, List[Union[str, int, float, bool]]]
         :keyword Callable response_hook: A callable invoked with the response metadata.
         :keyword Literal["High", "Low"] priority: Priority based execution allows users to set a priority for each
             request. Once the user has reached their provisioned throughput, low priority requests are throttled
             before high priority requests start getting throttled. Feature must first be enabled at the account level.
         :returns: An Iterable of items (dicts).
@@ -338,14 +341,16 @@
         response_hook = kwargs.pop('response_hook', None)
         if partition_key_range_id is not None:
             feed_options["partitionKeyRangeId"] = partition_key_range_id
         if partition_key is not None:
             feed_options["partitionKey"] = self._set_partition_key(partition_key)
         if is_start_from_beginning is not None:
             feed_options["isStartFromBeginning"] = is_start_from_beginning
+        if start_time is not None and is_start_from_beginning is False:
+            feed_options["startTime"] = start_time.astimezone(timezone.utc).strftime('%a, %d %b %Y %H:%M:%S GMT')
         if max_item_count is not None:
             feed_options["maxItemCount"] = max_item_count
         if continuation is not None:
             feed_options["continuation"] = continuation
 
         if hasattr(response_hook, "clear"):
             response_hook.clear()
@@ -467,15 +472,15 @@
         if continuation_token_limit is not None:
             feed_options["responseContinuationTokenLimitInKb"] = continuation_token_limit
         if hasattr(response_hook, "clear"):
             response_hook.clear()
 
         items = self.client_connection.QueryItems(
             database_or_container_link=self.container_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             partition_key=partition_key,
             response_hook=response_hook,
             **kwargs
         )
         if response_hook:
             response_hook(self.client_connection.last_response_headers, items)
@@ -1024,15 +1029,15 @@
         if enable_cross_partition_query is not None:
             feed_options["enableCrossPartitionQuery"] = enable_cross_partition_query
         if partition_key is not None:
             feed_options["partitionKey"] = self._set_partition_key(partition_key)
 
         result = self.client_connection.QueryConflicts(
             collection_link=self.container_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             **kwargs
         )
         if response_hook:
             response_hook(self.client_connection.last_response_headers, result)
         return result
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/cosmos_client.py` & `azure-cosmos-4.6.1/azure/cosmos/cosmos_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
             warnings.warn(
                 "the populate_query_metrics flag does not apply to this method and will be removed in the future",
                 UserWarning,
             )
             request_options["populateQueryMetrics"] = populate_query_metrics
 
         _set_throughput_options(offer=offer_throughput, request_options=request_options)
-        result = self.client_connection.CreateDatabase(database=dict(id=id), options=request_options, **kwargs)
+        result = self.client_connection.CreateDatabase(database={"id": id}, options=request_options, **kwargs)
         if response_hook:
             response_hook(self.client_connection.last_response_headers)
         return DatabaseProxy(self.client_connection, id=result["id"], properties=result)
 
     @distributed_trace
     def create_database_if_not_exists(  # pylint:disable=docstring-missing-param
         self,
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/database.py` & `azure-cosmos-4.6.1/azure/cosmos/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,15 @@
         conflict_resolution_policy: Optional[Dict[str, Any]] = None,
         *,
         session_token: Optional[str] = None,
         initial_headers: Optional[Dict[str, str]] = None,
         etag: Optional[str] = None,
         match_condition: Optional[MatchConditions] = None,
         analytical_storage_ttl: Optional[int] = None,
+        vector_embedding_policy: Optional[Dict[str, Any]] = None,
         **kwargs: Any
     ) -> ContainerProxy:
         """Create a new container with the given ID (name).
 
         If a container with the given ID already exists, a CosmosResourceExistsError is raised.
 
         :param str id: ID (name) of container to create.
@@ -195,14 +196,17 @@
         :keyword Callable response_hook: A callable invoked with the response metadata.
         :keyword int analytical_storage_ttl: Analytical store time to live (TTL) for items in the container.  A value of
             None leaves analytical storage off and a value of -1 turns analytical storage on with no TTL. Please
             note that analytical storage can only be enabled on Synapse Link enabled accounts.
         :keyword List[Dict[str, str]] computed_properties: **provisional** Sets The computed properties for this
             container in the Azure Cosmos DB Service. For more Information on how to use computed properties visit
             `here: https://learn.microsoft.com/en-us/azure/cosmos-db/nosql/query/computed-properties?tabs=dotnet`
+        :keyword Dict[str, Any] vector_embedding_policy: **provisional** The vector embedding policy for the container.
+            Each vector embedding possesses a predetermined number of dimensions, is associated with an underlying
+            data type, and is generated for a particular distance function.
         :returns: A `ContainerProxy` instance representing the new container.
         :raises ~azure.cosmos.exceptions.CosmosHttpResponseError: The container creation failed.
         :rtype: ~azure.cosmos.ContainerProxy
         .. admonition:: Example:
 
             .. literalinclude:: ../samples/examples.py
                 :start-after: [START create_container]
@@ -216,15 +220,15 @@
                 :start-after: [START create_container_with_settings]
                 :end-before: [END create_container_with_settings]
                 :language: python
                 :dedent: 0
                 :caption: Create a container with specific settings; in this case, a custom partition key:
                 :name: create_container_with_settings
         """
-        definition: Dict[str, Any] = dict(id=id)
+        definition: Dict[str, Any] = {"id": id}
         if partition_key is not None:
             definition["partitionKey"] = partition_key
         if indexing_policy is not None:
             if indexing_policy.get("indexingMode") is IndexingMode.Lazy:
                 warnings.warn(
                     "Lazy indexing mode has been deprecated. Mode will be set to consistent indexing by the backend.",
                     DeprecationWarning
@@ -235,16 +239,18 @@
         if unique_key_policy is not None:
             definition["uniqueKeyPolicy"] = unique_key_policy
         if conflict_resolution_policy is not None:
             definition["conflictResolutionPolicy"] = conflict_resolution_policy
         if analytical_storage_ttl is not None:
             definition["analyticalStorageTtl"] = analytical_storage_ttl
         computed_properties = kwargs.pop('computed_properties', None)
-        if computed_properties:
+        if computed_properties is not None:
             definition["computedProperties"] = computed_properties
+        if vector_embedding_policy is not None:
+            definition["vectorEmbeddingPolicy"] = vector_embedding_policy
 
         if session_token is not None:
             kwargs['session_token'] = session_token
         if initial_headers is not None:
             kwargs['initial_headers'] = initial_headers
         if etag is not None:
             kwargs['etag'] = etag
@@ -277,42 +283,46 @@
         conflict_resolution_policy: Optional[Dict[str, Any]] = None,
         *,
         session_token: Optional[str] = None,
         initial_headers: Optional[Dict[str, str]] = None,
         etag: Optional[str] = None,
         match_condition: Optional[MatchConditions] = None,
         analytical_storage_ttl: Optional[int] = None,
+        vector_embedding_policy: Optional[Dict[str, Any]] = None,
         **kwargs: Any
     ) -> ContainerProxy:
         """Create a container if it does not exist already.
 
         If the container already exists, the existing settings are returned.
         Note: it does not check or update the existing container settings or offer throughput
         if they differ from what was passed into the method.
 
-        :param id: ID (name) of container to read or create.
-        :param partition_key: The partition key to use for the container.
-        :param indexing_policy: The indexing policy to apply to the container.
-        :param default_ttl: Default time to live (TTL) for items in the container. If unspecified, items do not expire.
+        :param str id: ID (name) of container to create.
+        :param ~azure.cosmos.PartitionKey partition_key: The partition key to use for the container.
+        :param Dict[str, Any] indexing_policy: The indexing policy to apply to the container.
+        :param int default_ttl: Default time to live (TTL) for items in the container. If unused, items do not expire.
         :param offer_throughput: The provisioned throughput for this offer.
-        :paramtype offer_throughput: int or ~azure.cosmos.ThroughputProperties.
-        :param unique_key_policy: The unique key policy to apply to the container.
-        :param conflict_resolution_policy: The conflict resolution policy to apply to the container.
+        :type offer_throughput: Union[int, ~azure.cosmos.ThroughputProperties]
+        :param Dict[str, Any] unique_key_policy: The unique key policy to apply to the container.
+        :param Dict[str, Any] conflict_resolution_policy: The conflict resolution policy to apply to the container.
         :keyword str session_token: Token for use with Session consistency.
         :keyword Dict[str, str] initial_headers: Initial headers to be sent as part of the request.
         :keyword str etag: An ETag value, or the wildcard character (*). Used to check if the resource
             has changed, and act according to the condition specified by the `match_condition` parameter.
         :keyword ~azure.core.MatchConditions match_condition: The match condition to use upon the etag.
         :keyword Callable response_hook: A callable invoked with the response metadata.
         :keyword int analytical_storage_ttl: Analytical store time to live (TTL) for items in the container.  A value of
             None leaves analytical storage off and a value of -1 turns analytical storage on with no TTL.  Please
             note that analytical storage can only be enabled on Synapse Link enabled accounts.
         :keyword List[Dict[str, str]] computed_properties: **provisional** Sets The computed properties for this
             container in the Azure Cosmos DB Service. For more Information on how to use computed properties visit
             `here: https://learn.microsoft.com/en-us/azure/cosmos-db/nosql/query/computed-properties?tabs=dotnet`
+        :keyword Dict[str, Any] vector_embedding_policy: The vector embedding policy for the container. Each vector
+            embedding possesses a predetermined number of dimensions, is associated with an underlying data type, and
+            is generated for a particular distance function.
         :returns: A `ContainerProxy` instance representing the container.
         :raises ~azure.cosmos.exceptions.CosmosHttpResponseError: The container read or creation failed.
         :rtype: ~azure.cosmos.ContainerProxy
         """
         computed_properties = kwargs.pop("computed_properties", None)
         try:
             container_proxy = self.get_container_client(id)
@@ -335,14 +345,15 @@
                 conflict_resolution_policy=conflict_resolution_policy,
                 analytical_storage_ttl=analytical_storage_ttl,
                 computed_properties=computed_properties,
                 etag=etag,
                 match_condition=match_condition,
                 session_token=session_token,
                 initial_headers=initial_headers,
+                vector_embedding_policy=vector_embedding_policy,
                 **kwargs
             )
 
     @distributed_trace
     def delete_container(  # pylint:disable=docstring-missing-param
         self,
         container: Union[str, ContainerProxy, Mapping[str, Any]],
@@ -503,15 +514,15 @@
                 "the populate_query_metrics flag does not apply to this method and will be removed in the future",
                 UserWarning,
             )
             feed_options["populateQueryMetrics"] = populate_query_metrics
 
         result = self.client_connection.QueryContainers(
             database_link=self.database_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             **kwargs
         )
         if response_hook:
             response_hook(self.client_connection.last_response_headers, result)
         return result
 
@@ -647,15 +658,15 @@
         feed_options = build_options(kwargs)
         response_hook = kwargs.pop('response_hook', None)
         if max_item_count is not None:
             feed_options["maxItemCount"] = max_item_count
 
         result = self.client_connection.QueryUsers(
             database_link=self.database_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             **kwargs
         )
         if response_hook:
             response_hook(self.client_connection.last_response_headers, result)
         return result
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/diagnostics.py` & `azure-cosmos-4.6.1/azure/cosmos/diagnostics.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/documents.py` & `azure-cosmos-4.6.1/azure/cosmos/documents.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,13 +403,14 @@
     Distinct: Literal["Distinct"] = "Distinct"
     GroupBy: Literal["GroupBy"] = "GroupBy"
     MultipleAggregates: Literal["MultipleAggregates"] = "MultipleAggregates"
     MultipleOrderBy: Literal["MultipleOrderBy"] = "MultipleOrderBy"
     OffsetAndLimit: Literal["OffsetAndLimit"] = "OffsetAndLimit"
     OrderBy: Literal["OrderBy"] = "OrderBy"
     Top: Literal["Top"] = "Top"
+    NonStreamingOrderBy: Literal["NonStreamingOrderBy"] = "NonStreamingOrderBy"
 
 
 class _DistinctType:
     NoneType: Literal["None"] = "None"
     Ordered: Literal["Ordered"] = "Ordered"
     Unordered: Literal["Unordered"] = "Unordered"
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/errors.py` & `azure-cosmos-4.6.1/azure/cosmos/errors.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/exceptions.py` & `azure-cosmos-4.6.1/azure/cosmos/exceptions.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/http_constants.py` & `azure-cosmos-4.6.1/azure/cosmos/http_constants.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/offer.py` & `azure-cosmos-4.6.1/azure/cosmos/offer.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/partition_key.py` & `azure-cosmos-4.6.1/azure/cosmos/partition_key.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/permission.py` & `azure-cosmos-4.6.1/azure/cosmos/permission.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/azure/cosmos/scripts.py` & `azure-cosmos-4.6.1/azure/cosmos/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         :rtype: Iterable[Dict[str, Any]]
         """
         feed_options = build_options(kwargs)
         if max_item_count is not None:
             feed_options["maxItemCount"] = max_item_count
         return self.client_connection.QueryStoredProcedures(
             collection_link=self.container_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             **kwargs
         )
 
     @distributed_trace
     def get_stored_procedure(self, sproc: Union[str, Mapping[str, Any]], **kwargs: Any) -> Dict[str, Any]:
         """Get the stored procedure identified by `id`.
@@ -266,15 +266,15 @@
         """
         feed_options = build_options(kwargs)
         if max_item_count is not None:
             feed_options["maxItemCount"] = max_item_count
 
         return self.client_connection.QueryTriggers(
             collection_link=self.container_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             **kwargs
         )
 
     @distributed_trace
     def get_trigger(self, trigger: Union[str, Mapping[str, Any]], **kwargs: Any) -> Dict[str, Any]:
         """Get a trigger identified by `id`.
@@ -391,15 +391,15 @@
         """
         feed_options = build_options(kwargs)
         if max_item_count is not None:
             feed_options["maxItemCount"] = max_item_count
 
         return self.client_connection.QueryUserDefinedFunctions(
             collection_link=self.container_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             **kwargs
         )
 
     @distributed_trace
     def get_user_defined_function(self, udf: Union[str, Mapping[str, Any]], **kwargs: Any) -> Dict[str, Any]:
         """Get a user-defined functions identified by `id`.
```

### Comparing `azure-cosmos-4.6.0/azure/cosmos/user.py` & `azure-cosmos-4.6.1/azure/cosmos/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,15 +133,15 @@
         feed_options = build_options(kwargs)
         response_hook = kwargs.pop('response_hook', None)
         if max_item_count is not None:
             feed_options["maxItemCount"] = max_item_count
 
         result = self.client_connection.QueryPermissions(
             user_link=self.user_link,
-            query=query if parameters is None else dict(query=query, parameters=parameters),
+            query=query if parameters is None else {"query": query, "parameters": parameters},
             options=feed_options,
             response_hook=response_hook,
             **kwargs
         )
 
         if response_hook:
             response_hook(self.client_connection.last_response_headers, result)
```

### Comparing `azure-cosmos-4.6.0/azure_cosmos.egg-info/PKG-INFO` & `azure-cosmos-4.6.1/azure_cosmos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-cosmos
-Version: 4.6.0
+Version: 4.6.1
 Summary: Microsoft Azure Cosmos Client Library for Python
 Home-page: https://github.com/Azure/azure-sdk-for-python
 Author: Microsoft Corporation
 Author-email: askdocdb@microsoft.com
 Maintainer: Microsoft
 Maintainer-email: askdocdb@microsoft.com
 License: MIT License
@@ -21,16 +21,14 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: azure-core>=1.25.1
-Requires-Dist: typing-extensions>=4.6.0
 
 ## _Disclaimer_
 _Azure SDK Python packages support for Python 2.7 has ended 01 January 2022. For more information and questions, please refer to https://github.com/Azure/azure-sdk-for-python/issues/20691_
 
 # Azure Cosmos DB SQL API client library for Python
 
 Azure Cosmos DB is a globally distributed, multi-model database service that supports document, key-value, wide-column, and graph databases.
@@ -184,15 +182,14 @@
 * Group By queries
 * Queries with COUNT from a DISTINCT subquery: SELECT COUNT (1) FROM (SELECT DISTINCT C.ID FROM C)
 * Direct TCP Mode access
 * Continuation token support for aggregate cross-partition queries like sorting, counting, and distinct.
 Streamable queries like `SELECT * FROM WHERE` *do* support continuation tokens.
 * Change Feed: Processor
 * Change Feed: Read multiple partitions key values
-* Change Feed: Read specific time
 * Cross-partition ORDER BY for mixed types
 * Enabling diagnostics for async query-type methods
 
 ### Control Plane Limitations:
 
 * Get CollectionSizeUsage, DatabaseUsage, and DocumentUsage metrics
 * Create Geospatial Index
@@ -202,15 +199,15 @@
 ## Workarounds
 
 ### Control Plane Limitations Workaround
 
 Typically, you can use [Azure Portal](https://portal.azure.com/), [Azure Cosmos DB Resource Provider REST API](https://docs.microsoft.com/rest/api/cosmos-db-resource-provider), [Azure CLI](https://docs.microsoft.com/cli/azure/azure-cli-reference-for-cosmos-db) or [PowerShell](https://docs.microsoft.com/azure/cosmos-db/manage-with-powershell) for the control plane unsupported limitations.
 
 ### Using The Async Client as a Workaround to Bulk
-While the SDK supports transactional batch, support for bulk requests is not yet implemented in the Python SDK. You can use the async client along with this [concurrency sample][concurrency_sample] we have developed as a reference for a possible workaround. 
+While the SDK supports transactional batch, support for bulk requests is not yet implemented in the Python SDK. You can use the async client along with this [concurrency sample][cosmos_concurrency_sample] we have developed as a reference for a possible workaround. 
 >[WARNING]
 > Using the asynchronous client for concurrent operations like shown in this sample will consume a lot of RUs very fast. We **strongly recommend** testing this out against the cosmos emulator first to verify your code works well and avoid incurring charges.
 
 
 
 ## Boolean Data Type
 
@@ -655,14 +652,115 @@
 and [async][sample_document_mgmt_async] clients.
 
 If there is a failure for an operation within the batch, the SDK will raise a `CosmosBatchOperationError` letting you know which operation failed,
 as well as containing the list of failed responses for the failed request.
 
 For more information on Transactional Batch, see [Azure Cosmos DB Transactional Batch][cosmos_transactional_batch].
 
+### Public Preview - Vector Embeddings and Vector Indexes
+We have added new capabilities to utilize vector embeddings and vector indexing for users to leverage vector
+search utilizing our Cosmos SDK. These two container-level configurations have to be turned on at the account-level
+before you can use them.
+
+Each vector embedding should have a path to the relevant vector field in your items being stored, a supported data type
+(float32, int8, uint8), the vector's dimensions, and the distance function being used for that embedding. Vectors indexed 
+with the flat index type can be at most 505 dimensions. Vectors indexed with the quantizedFlat index type can be at most 4,096 dimensions.
+A sample vector embedding policy would look like this:
+```python
+vector_embedding_policy = {
+    "vectorEmbeddings": [
+        {
+            "path": "/vector1",
+            "dataType": "float32",
+            "dimensions": 256,
+            "distanceFunction": "euclidean"
+        },
+        {
+            "path": "/vector2",
+            "dataType": "int8",
+            "dimensions": 200,
+            "distanceFunction": "dotproduct"
+        },
+        {
+            "path": "/vector3",
+            "dataType": "uint8",
+            "dimensions": 400,
+            "distanceFunction": "cosine"
+        }
+    ]
+}
+```
+
+Separately, vector indexes have been added to the already existing indexing_policy and only require two fields per index:
+the path to the relevant field to be used, and the type of index from the possible options (flat or quantizedFlat).
+A sample indexing policy with vector indexes would look like this:
+```python
+indexing_policy = {
+        "automatic": True,
+        "indexingMode": "consistent",
+        "compositeIndexes": [
+            [
+                {"path": "/numberField", "order": "ascending"},
+                {"path": "/stringField", "order": "descending"}
+            ]
+        ],
+        "spatialIndexes": [
+            {"path": "/location/*", "types": [
+                "Point",
+                "Polygon"]}
+        ],
+        "vectorIndexes": [
+            {"path": "/vector1", "type": "flat"},
+            {"path": "/vector2", "type": "quantizedFlat"}
+        ]
+    }
+```
+You would then pass in the relevant policies to your container creation method to ensure these configurations are used by it.
+The operation will fail if you pass new vector indexes to your indexing policy but forget to pass in an embedding policy.
+```python
+database.create_container(id=container_id, partition_key=PartitionKey(path="/id"),
+                          indexing_policy=indexing_policy, vector_embedding_policy=vector_embedding_policy)
+```
+***Note: vector embeddings and vector indexes CANNOT be edited by container replace operations. They are only available directly through creation.***
+
+### Public Preview - Vector Search
+
+With the addition of the vector indexing and vector embedding capabilities, the SDK can now perform order by vector search queries.
+These queries specify the VectorDistance to use as a metric within the query text. These must always use a TOP or LIMIT clause within the query though,
+since vector search queries have to look through a lot of data otherwise and may become too expensive or long-running.
+Since these queries are relatively expensive, the SDK sets a default limit of 50000 max items per query - if you'd like to raise that further, you
+can use the `AZURE_COSMOS_MAX_ITEM_BUFFER_VECTOR_SEARCH` environment variable to do so. However, be advised that queries with too many vector results
+may have additional latencies associated with searching in the service.
+The query syntax for these operations looks like this:
+```python
+VectorDistance(<embedding1>, <embedding2>, [,<exact_search>], [,<specification>])
+```
+Embeddings 1 and 2 are the arrays of values for the relevant embeddings, `exact_search` is an optional boolean indicating whether
+to do an exact search vs. an approximate one (default value of false), and `specification` is an optional Json snippet with embedding
+specs that can include `dataType`, `dimensions` and `distanceFunction`. The specifications within the query will take precedence
+to any configurations previously set by a vector embedding policy.
+A sample vector search query would look something like this:
+```python
+    query = "SELECT TOP 10 c.title,VectorDistance(c.embedding, [{}]) AS " \
+            "SimilarityScore FROM c ORDER BY VectorDistance(c.embedding, [{}])".format(embeddings_string, embeddings_string)
+```
+Or if you'd like to add the optional parameters to the vector distance, you could do this:
+```python
+    query = "SELECT TOP 10 c.title,VectorDistance(c.embedding, [{}], true, {{'dataType': 'float32' , 'distanceFunction': 'cosine'}}) AS " \
+            "SimilarityScore FROM c ORDER BY VectorDistance(c.embedding, [{}], true, {{'dataType': " \
+            "'float32', 'distanceFunction': 'cosine'}})".format(embeddings_string, embeddings_string)
+```
+The `embeddings_string` above would be your string made from your vector embeddings.
+You can find our sync samples [here][cosmos_index_sample] and our async samples [here][cosmos_index_sample_async] as well to help yourself out.
+
+*Note: For a limited time, if your query operates against a region or emulator that has not yet been updated the client might run into some issues
+not being able to recognize the new NonStreamingOrderBy capability that makes vector search possible.
+If this happens, you can set the `AZURE_COSMOS_DISABLE_NON_STREAMING_ORDER_BY` environment variable to `"True"` to opt out of this
+functionality and continue operating as usual.*
+
 ## Troubleshooting
 
 ### General
 
 When you interact with Cosmos DB using the Python SDK, exceptions returned by the service correspond to the same HTTP status codes returned for REST API requests:
 
 [HTTP Status Codes for Azure Cosmos DB][cosmos_http_status_codes]
@@ -789,14 +887,16 @@
 [source_code]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos
 [venv]: https://docs.python.org/3/library/venv.html
 [virtualenv]: https://virtualenv.pypa.io
 [telemetry_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/tracing_open_telemetry.py
 [timeouts_document]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/docs/TimeoutAndRetriesConfig.md
 [cosmos_transactional_batch]: https://learn.microsoft.com/azure/cosmos-db/nosql/transactional-batch
 [cosmos_concurrency_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/concurrency_sample.py
+[cosmos_index_sample]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/index_management.py
+[cosmos_index_sample_async]: https://github.com/Azure/azure-sdk-for-python/tree/main/sdk/cosmos/azure-cosmos/samples/index_management_async.py
 
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.microsoft.com.
 
@@ -806,14 +906,25 @@
 
 This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
 For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
 contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
 
 ## Release History
 
+### 4.6.1 (2024-05-15)
+
+#### Features Added
+* Adds vector embedding policy and vector indexing policy. See [PR 34882](https://github.com/Azure/azure-sdk-for-python/pull/34882).
+* Adds support for vector search non-streaming order by queries. See [PR 35468](https://github.com/Azure/azure-sdk-for-python/pull/35468).
+* Adds support for using the start time option for change feed query API. See [PR 35090](https://github.com/Azure/azure-sdk-for-python/pull/35090).
+
+#### Bugs Fixed
+* Fixed a bug where change feed query in Async client was not returning all pages due to case-sensitive response headers. See [PR 35090](https://github.com/Azure/azure-sdk-for-python/pull/35090).
+* Fixed a bug when a retryable exception occurs in the first page of a query execution causing query to return 0 results. See [PR 35090](https://github.com/Azure/azure-sdk-for-python/pull/35090).
+
 ### 4.6.0 (2024-03-14)
 
 #### Features Added
 * GA release of hierarchical partitioning, index metrics and transactional batch.
 
 #### Bugs Fixed
 * Keyword arguments were not being passed down for `create_container_if_not_exists()` methods. See [PR 34286](https://github.com/Azure/azure-sdk-for-python/pull/34286).
```

### Comparing `azure-cosmos-4.6.0/azure_cosmos.egg-info/SOURCES.txt` & `azure-cosmos-4.6.1/azure_cosmos.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -53,22 +53,24 @@
 azure/cosmos/_execution_context/__init__.py
 azure/cosmos/_execution_context/aggregators.py
 azure/cosmos/_execution_context/base_execution_context.py
 azure/cosmos/_execution_context/document_producer.py
 azure/cosmos/_execution_context/endpoint_component.py
 azure/cosmos/_execution_context/execution_dispatcher.py
 azure/cosmos/_execution_context/multi_execution_aggregator.py
+azure/cosmos/_execution_context/non_streaming_order_by_aggregator.py
 azure/cosmos/_execution_context/query_execution_info.py
 azure/cosmos/_execution_context/aio/__init__.py
 azure/cosmos/_execution_context/aio/_queue_async_helper.py
 azure/cosmos/_execution_context/aio/base_execution_context.py
 azure/cosmos/_execution_context/aio/document_producer.py
 azure/cosmos/_execution_context/aio/endpoint_component.py
 azure/cosmos/_execution_context/aio/execution_dispatcher.py
 azure/cosmos/_execution_context/aio/multi_execution_aggregator.py
+azure/cosmos/_execution_context/aio/non_streaming_order_by_aggregator.py
 azure/cosmos/_routing/__init__.py
 azure/cosmos/_routing/collection_routing_map.py
 azure/cosmos/_routing/routing_map_provider.py
 azure/cosmos/_routing/routing_range.py
 azure/cosmos/_routing/aio/__init__.py
 azure/cosmos/_routing/aio/routing_map_provider.py
 azure/cosmos/aio/__init__.py
@@ -107,14 +109,15 @@
 samples/document_management.py
 samples/document_management_async.py
 samples/examples.py
 samples/examples_async.py
 samples/index_management.py
 samples/index_management_async.py
 samples/tracing_open_telemetry.py
+samples/vector_test_data.py
 samples/MultiMasterOperations/Configurations.py
 samples/MultiMasterOperations/ConflictWorker.py
 samples/MultiMasterOperations/MultiMasterScenario.py
 samples/MultiMasterOperations/Program.py
 samples/MultiMasterOperations/Worker.py
 test/conftest.py
 test/test_aad.py
@@ -149,23 +152,28 @@
 test/test_query.py
 test/test_query_async.py
 test/test_query_computed_properties.py
 test/test_query_computed_properties_async.py
 test/test_query_cross_partition.py
 test/test_query_cross_partition_async.py
 test/test_query_execution_context.py
+test/test_query_vector_similarity.py
+test/test_query_vector_similarity_async.py
 test/test_resource_id.py
 test/test_resource_id_async.py
 test/test_retry_policy.py
 test/test_routing_map.py
 test/test_session.py
 test/test_session_container.py
 test/test_session_token_unit.py
 test/test_streaming_failover.py
 test/test_transactional_batch.py
 test/test_transactional_batch_async.py
 test/test_ttl.py
 test/test_user_configs.py
 test/test_utils.py
+test/test_vector_policy.py
+test/test_vector_policy_async.py
+test/vector_test_data.py
 test/routing/__init__.py
 test/routing/test_collection_routing_map.py
 test/routing/test_routing_map_provider.py
```

### Comparing `azure-cosmos-4.6.0/samples/MultiMasterOperations/ConflictWorker.py` & `azure-cosmos-4.6.1/samples/MultiMasterOperations/ConflictWorker.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/MultiMasterOperations/MultiMasterScenario.py` & `azure-cosmos-4.6.1/samples/MultiMasterOperations/MultiMasterScenario.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/MultiMasterOperations/Worker.py` & `azure-cosmos-4.6.1/samples/MultiMasterOperations/Worker.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/README.md` & `azure-cosmos-4.6.1/samples/README.md`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/access_cosmos_with_aad.py` & `azure-cosmos-4.6.1/samples/access_cosmos_with_aad.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/access_cosmos_with_aad_async.py` & `azure-cosmos-4.6.1/samples/access_cosmos_with_aad_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/access_cosmos_with_resource_token.py` & `azure-cosmos-4.6.1/samples/access_cosmos_with_resource_token.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/access_cosmos_with_resource_token_async.py` & `azure-cosmos-4.6.1/samples/access_cosmos_with_resource_token_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/change_feed_management.py` & `azure-cosmos-4.6.1/test/test_partition_split_query.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,100 @@
-# -------------------------------------------------------------------------
+# The MIT License (MIT)
 # Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See LICENSE.txt in the project root for
-# license information.
-# -------------------------------------------------------------------------
-import azure.cosmos.documents as documents
-import azure.cosmos.cosmos_client as cosmos_client
-import azure.cosmos.exceptions as exceptions
-import azure.cosmos.partition_key as partition_key
-import uuid
-
-import config
-
-# ----------------------------------------------------------------------------------------------------------
-# Prerequisites -
-#
-# 1. An Azure Cosmos account -
-#    https:#azure.microsoft.com/en-us/documentation/articles/documentdb-create-account/
-#
-# 2. Microsoft Azure Cosmos PyPi package -
-#    https://pypi.python.org/pypi/azure-cosmos/
-# ----------------------------------------------------------------------------------------------------------
-# Sample - demonstrates how to consume the Change Feed and iterate on the results.
-# ----------------------------------------------------------------------------------------------------------
-
-HOST = config.settings['host']
-MASTER_KEY = config.settings['master_key']
-DATABASE_ID = config.settings['database_id']
-CONTAINER_ID = config.settings['container_id']
-
-
-def create_items(container, size):
-    print('Creating Items')
-
-    for i in range(1, size):
-        c = str(uuid.uuid4())
-        item_definition = {'id': 'item' + c,
-                                'address': {'street': '1 Microsoft Way'+c,
-                                        'city': 'Redmond'+c,
-                                        'state': 'WA',
-                                        'zip code': 98052
-                                        }
-                                }
-
-        created_item = container.create_item(body=item_definition)
-
-
-def read_change_feed(container):
-    print('\nReading Change Feed from the beginning\n')
-
-    # For a particular Partition Key Range we can use partition_key_range_id]
-    # 'is_start_from_beginning = True' will read from the beginning of the history of the container
-    # If no is_start_from_beginning is specified, the read change feed loop will pickup the items that happen while the loop / process is active
-    response = container.query_items_change_feed(is_start_from_beginning=True)
-    for doc in response:
-        print(doc)
-
-    print('\nFinished reading all the change feed\n')
-
-
-def run_sample():
-    client = cosmos_client.CosmosClient(HOST, {'masterKey': MASTER_KEY})
-    try:
-        # setup database for this sample
-        try:
-            db = client.create_database(id=DATABASE_ID)
-        except exceptions.CosmosResourceExistsError:
-            raise RuntimeError("Database with id '{}' already exists".format(DATABASE_ID))
 
-        # setup container for this sample
-        try:
-            container = db.create_container(
-                id=CONTAINER_ID,
-                partition_key=partition_key.PartitionKey(path='/address/state', kind=documents.PartitionKind.Hash)
-            )
-            print('Container with id \'{0}\' created'.format(CONTAINER_ID))
-
-        except exceptions.CosmosResourceExistsError:
-            raise RuntimeError("Container with id '{}' already exists".format(CONTAINER_ID))
+import random
+import time
+import unittest
+import uuid
+import os
 
-        create_items(container, 100)
-        read_change_feed(container)
+import azure.cosmos.cosmos_client as cosmos_client
+import test_config
+from azure.cosmos import DatabaseProxy, PartitionKey, ContainerProxy
+from azure.cosmos.exceptions import CosmosClientTimeoutError, CosmosHttpResponseError
+
+
+def get_test_item():
+    test_item = {
+        'id': 'Item_' + str(uuid.uuid4()),
+        'test_object': True,
+        'lastName': 'Smith',
+        'attr1': random.randint(0, 10)
+    }
+    return test_item
+
+
+def run_queries(container, iterations):
+    ret_list = list()
+    for i in range(iterations):
+        curr = str(random.randint(0, 10))
+        query = 'SELECT * FROM c WHERE c.attr1=' + curr + ' order by c.attr1'
+        qlist = list(container.query_items(query=query, enable_cross_partition_query=True))
+        ret_list.append((curr, qlist))
+    for ret in ret_list:
+        curr = ret[0]
+        if len(ret[1]) != 0:
+            for results in ret[1]:
+                attr_number = results['attr1']
+                assert str(attr_number) == curr  # verify that all results match their randomly generated attributes
+        print("validation succeeded for all query results")
+
+
+class TestPartitionSplitQuery(unittest.TestCase):
+    database: DatabaseProxy = None
+    container: ContainerProxy = None
+    client: cosmos_client.CosmosClient = None
+    configs = test_config.TestConfig
+    host = configs.host
+    masterKey = configs.masterKey
+    throughput = 400
+    TEST_DATABASE_ID = configs.TEST_DATABASE_ID
+    TEST_CONTAINER_ID = "Single-partition-container-without-throughput"
+
+    @classmethod
+    def setUpClass(cls):
+        cls.client = cosmos_client.CosmosClient(cls.host, cls.masterKey)
+        cls.database = cls.client.get_database_client(cls.TEST_DATABASE_ID)
+        cls.container = cls.database.create_container(
+            id=cls.TEST_CONTAINER_ID,
+            partition_key=PartitionKey(path="/id"))
+        if cls.host == "https://localhost:8081/":
+            os.environ["AZURE_COSMOS_DISABLE_NON_STREAMING_ORDER_BY"] = "True"
 
-        # cleanup database after sample
+    @classmethod
+    def tearDownClass(cls) -> None:
         try:
-            client.delete_database(db)
-        except exceptions.CosmosResourceNotFoundError:
+            cls.database.delete_container(cls.container.id)
+        except CosmosHttpResponseError:
             pass
 
-    except exceptions.CosmosHttpResponseError as e:
-        print('\nrun_sample has caught an error. {0}'.format(e.message))
-
-    finally:
-        print("\nrun_sample done")
+    def test_partition_split_query(self):
+        for i in range(100):
+            body = get_test_item()
+            self.container.create_item(body=body)
+
+        start_time = time.time()
+        print("created items, changing offer to 11k and starting queries")
+        self.database.replace_throughput(11000)
+        offer_time = time.time()
+        print("changed offer to 11k")
+        print("--------------------------------")
+        print("now starting queries")
+
+        run_queries(self.container, 100)  # initial check for queries before partition split
+        print("initial check succeeded, now reading offer until replacing is done")
+        offer = self.database.get_throughput()
+        while True:
+            if time.time() - start_time > 60 * 25:  # timeout test at 25 minutes
+                raise CosmosClientTimeoutError()
+            if offer.properties['content'].get('isOfferReplacePending', False):
+                time.sleep(10)
+                offer = self.database.get_throughput()
+            else:
+                print("offer replaced successfully, took around {} seconds".format(time.time() - offer_time))
+                run_queries(self.container, 100)  # check queries work post partition split
+                self.assertTrue(offer.offer_throughput > self.throughput)
+                return
 
 
-if __name__ == '__main__':
-    run_sample()
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `azure-cosmos-4.6.0/samples/change_feed_management_async.py` & `azure-cosmos-4.6.1/samples/change_feed_management.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License. See LICENSE.txt in the project root for
 # license information.
 # -------------------------------------------------------------------------
-from azure.cosmos.aio import CosmosClient
-import azure.cosmos.exceptions as exceptions
+from datetime import datetime, timezone
+
 import azure.cosmos.documents as documents
+import azure.cosmos.cosmos_client as cosmos_client
+import azure.cosmos.exceptions as exceptions
 import azure.cosmos.partition_key as partition_key
 import uuid
 
-import asyncio
 import config
 
 # ----------------------------------------------------------------------------------------------------------
 # Prerequisites -
 #
 # 1. An Azure Cosmos account -
 #    https:#azure.microsoft.com/en-us/documentation/articles/documentdb-create-account/
@@ -26,78 +27,95 @@
 
 HOST = config.settings['host']
 MASTER_KEY = config.settings['master_key']
 DATABASE_ID = config.settings['database_id']
 CONTAINER_ID = config.settings['container_id']
 
 
-async def create_items(container, size):
+def create_items(container, size):
     print('Creating Items')
 
     for i in range(1, size):
         c = str(uuid.uuid4())
         item_definition = {'id': 'item' + c,
-                                'address': {'street': '1 Microsoft Way'+c,
-                                        'city': 'Redmond'+c,
-                                        'state': 'WA',
-                                        'zip code': 98052
-                                        }
-                                }
+                           'address': {'street': '1 Microsoft Way' + c,
+                                       'city': 'Redmond' + c,
+                                       'state': 'WA',
+                                       'zip code': 98052
+                                       }
+                           }
 
-        await container.create_item(body=item_definition)
+        created_item = container.create_item(body=item_definition)
 
 
-async def read_change_feed(container):
+def read_change_feed(container):
     print('\nReading Change Feed from the beginning\n')
 
     # For a particular Partition Key Range we can use partition_key_range_id]
     # 'is_start_from_beginning = True' will read from the beginning of the history of the container
     # If no is_start_from_beginning is specified, the read change feed loop will pickup the items that happen while the loop / process is active
     response = container.query_items_change_feed(is_start_from_beginning=True)
-
-    # Because the asynchronous client returns an asynchronous iterator object for methods using queries,
-    # we do not need to await the function. However, attempting to cast this object into a list directly 
-    # will throw an error; instead, iterate over the result using an async for loop like shown here
-    async for doc in response:
+    for doc in response:
         print(doc)
 
     print('\nFinished reading all the change feed\n')
 
 
-async def run_sample():
-    async with CosmosClient(HOST, MASTER_KEY) as client:
+def read_change_feed_with_start_time(container, start_time):
+    time = start_time.strftime('%a, %d %b %Y %H:%M:%S GMT')
+    print('\nReading Change Feed from start time of {}\n'.format(time))
+
+    # You can read change feed from a specific time.
+    # You must pass in a datetime object for the start_time field.
+    response = container.query_items_change_feed(start_time=start_time)
+    for doc in response:
+        print(doc)
+
+    print('\nFinished reading all the change feed from start time of {}\n'.format(time))
+
+
+def run_sample():
+    client = cosmos_client.CosmosClient(HOST, {'masterKey': MASTER_KEY})
+    try:
+        # setup database for this sample
+        try:
+            db = client.create_database(id=DATABASE_ID)
+        except exceptions.CosmosResourceExistsError:
+            raise RuntimeError("Database with id '{}' already exists".format(DATABASE_ID))
+
+        # setup container for this sample
+        try:
+            container = db.create_container(
+                id=CONTAINER_ID,
+                partition_key=partition_key.PartitionKey(path='/address/state', kind=documents.PartitionKind.Hash)
+            )
+            print('Container with id \'{0}\' created'.format(CONTAINER_ID))
+
+        except exceptions.CosmosResourceExistsError:
+            raise RuntimeError("Container with id '{}' already exists".format(CONTAINER_ID))
+
+        # Create items
+        create_items(container, 100)
+        # Timestamp post item creations
+        timestamp = datetime.now(timezone.utc)
+        # Create more items after time stamp
+        create_items(container, 50)
+        # Read change feed from beginning
+        read_change_feed(container)
+        # Read Change Feed from timestamp
+        read_change_feed_with_start_time(container, timestamp)
+
+        # cleanup database after sample
         try:
-            # setup database for this sample
-            try:
-                db = await client.create_database(id=DATABASE_ID)
-            except exceptions.CosmosResourceExistsError:
-                raise RuntimeError("Database with id '{}' already exists".format(DATABASE_ID))
-
-            # setup container for this sample
-            try:
-                container = await db.create_container(
-                    id=CONTAINER_ID,
-                    partition_key=partition_key.PartitionKey(path='/address/state', kind=documents.PartitionKind.Hash)
-                )
-                print('Container with id \'{0}\' created'.format(CONTAINER_ID))
-
-            except exceptions.CosmosResourceExistsError:
-                raise RuntimeError("Container with id '{}' already exists".format(CONTAINER_ID))
-
-            await create_items(container, 100)
-            await read_change_feed(container)
-
-            # cleanup database after sample
-            try:
-                await client.delete_database(db)
-            except exceptions.CosmosResourceNotFoundError:
-                pass
+            client.delete_database(db)
+        except exceptions.CosmosResourceNotFoundError:
+            pass
 
-        except exceptions.CosmosHttpResponseError as e:
-            print('\nrun_sample has caught an error. {0}'.format(e.message))
+    except exceptions.CosmosHttpResponseError as e:
+        print('\nrun_sample has caught an error. {0}'.format(e.message))
 
-        finally:
-            print("\nrun_sample done")
+    finally:
+        print("\nrun_sample done")
 
 
 if __name__ == '__main__':
-    asyncio.run(run_sample())
+    run_sample()
```

### Comparing `azure-cosmos-4.6.0/samples/client_user_configs.py` & `azure-cosmos-4.6.1/samples/client_user_configs.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/client_user_configs_async.py` & `azure-cosmos-4.6.1/samples/client_user_configs_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/concurrency_sample.py` & `azure-cosmos-4.6.1/samples/concurrency_sample.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/config.py` & `azure-cosmos-4.6.1/samples/config.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/container_management.py` & `azure-cosmos-4.6.1/samples/container_management.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/container_management_async.py` & `azure-cosmos-4.6.1/samples/container_management_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/database_management.py` & `azure-cosmos-4.6.1/samples/database_management.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/database_management_async.py` & `azure-cosmos-4.6.1/samples/database_management_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/document_management.py` & `azure-cosmos-4.6.1/samples/document_management.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/document_management_async.py` & `azure-cosmos-4.6.1/samples/document_management_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/examples.py` & `azure-cosmos-4.6.1/samples/examples.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/examples_async.py` & `azure-cosmos-4.6.1/samples/examples_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/samples/index_management.py` & `azure-cosmos-4.6.1/samples/index_management.py`

 * *Files 3% similar despite different names*

```diff
@@ -629,14 +629,79 @@
         print("\n")
     except exceptions.CosmosResourceExistsError:
         print("Entity already exists")
     except exceptions.CosmosResourceNotFoundError:
         print("Entity doesn't exist")
 
 
+def use_vector_embedding_policy(db):
+    try:
+        delete_container_if_exists(db, CONTAINER_ID)
+
+        # Create a container with vector embedding policy and vector indexes
+        indexing_policy = {
+            "vectorIndexes": [
+                {"path": "/embeddings", "type": "quantizedFlat"},
+            ]
+        }
+        vector_embedding_policy = {
+            "vectorEmbeddings": [
+                {
+                    "path": "/embeddings",
+                    "dataType": "float32",
+                    "dimensions": 1000,
+                    "distanceFunction": "cosine"
+                }
+            ]
+        }
+
+        created_container = db.create_container(
+            id=CONTAINER_ID,
+            partition_key=PARTITION_KEY,
+            indexing_policy=indexing_policy,
+            vector_embedding_policy=vector_embedding_policy
+        )
+        properties = created_container.read()
+        print(created_container)
+
+        print("\n" + "-" * 25 + "\n9. Container created with vector embedding policy and vector indexes")
+        print_dictionary_items(properties["indexingPolicy"])
+        print_dictionary_items(properties["vectorEmbeddingPolicy"])
+
+        # We define our own get_embeddings() function for the sake of the sample, but you should be using a third
+        # party service to generate these properly
+        def get_embeddings(num):
+            return f"{str(num)}, {str(num)}, {str(num)}"
+
+        # Create some items with vector embeddings
+        for i in range(10):
+            created_container.create_item({"id": "vector_item" + str(i), "embeddings": get_embeddings(i)})
+
+        # Run vector similarity search queries using VectorDistance
+        query = "SELECT TOP 5 c.id,VectorDistance(c.embeddings, [{}]) AS " \
+                "SimilarityScore FROM c ORDER BY VectorDistance(c.embeddings, [{}])".format(get_embeddings(1),
+                                                                                            get_embeddings(1))
+        query_documents_with_custom_query(created_container, query)
+
+        # Run vector similarity search queries using VectorDistance with specifications
+        query = "SELECT TOP 5 c.id,VectorDistance(c.embeddings, [{}], true, {{'dataType': 'float32' ," \
+                " 'distanceFunction': 'cosine'}}) AS SimilarityScore FROM c ORDER BY VectorDistance(c.embeddings," \
+                " [{}], true, {{'dataType': 'float32', 'distanceFunction': 'cosine'}})".format(get_embeddings(1),
+                                                                                               get_embeddings(1))
+        query_documents_with_custom_query(created_container, query)
+
+        # Cleanup
+        db.delete_container(created_container)
+        print("\n")
+    except exceptions.CosmosResourceExistsError:
+        print("Entity already exists")
+    except exceptions.CosmosResourceNotFoundError:
+        print("Entity doesn't exist")
+
+
 def run_sample():
     try:
         client = obtain_client()
         fetch_all_databases(client)
 
         # Create database if doesn't exist already.
         created_db = create_database_if_not_exists(client, DATABASE_ID)
@@ -659,12 +724,15 @@
 
         # 7. Perform an index transform
         perform_index_transformations(created_db)
 
         # 8. Perform Multi Orderby queries using composite indexes
         perform_multi_orderby_query(created_db)
 
+        # 9. Create and use a vector embedding policy
+        use_vector_embedding_policy(created_db)
+
     except exceptions.AzureError as e:
         raise e
 
 if __name__ == '__main__':
     run_sample()
```

### Comparing `azure-cosmos-4.6.0/samples/index_management_async.py` & `azure-cosmos-4.6.1/samples/index_management_async.py`

 * *Files 6% similar despite different names*

```diff
@@ -624,14 +624,79 @@
         print("\n")
     except exceptions.CosmosResourceExistsError:
         print("Entity already exists")
     except exceptions.CosmosResourceNotFoundError:
         print("Entity doesn't exist")
 
 
+async def use_vector_embedding_policy(db):
+    try:
+        await delete_container_if_exists(db, CONTAINER_ID)
+
+        # Create a container with vector embedding policy and vector indexes
+        indexing_policy = {
+            "vectorIndexes": [
+                {"path": "/vector", "type": "quantizedFlat"},
+            ]
+        }
+        vector_embedding_policy = {
+            "vectorEmbeddings": [
+                {
+                    "path": "/vector",
+                    "dataType": "float32",
+                    "dimensions": 1000,
+                    "distanceFunction": "cosine"
+                }
+            ]
+        }
+
+        created_container = await db.create_container(
+            id=CONTAINER_ID,
+            partition_key=PARTITION_KEY,
+            indexing_policy=indexing_policy,
+            vector_embedding_policy=vector_embedding_policy
+        )
+        properties = await created_container.read()
+        print(created_container)
+
+        print("\n" + "-" * 25 + "\n9. Container created with vector embedding policy and vector indexes")
+        print_dictionary_items(properties["indexingPolicy"])
+        print_dictionary_items(properties["vectorEmbeddingPolicy"])
+
+        # We define our own get_embeddings() function for the sake of the sample, but you should be using a third
+        # party service to generate these properly.
+        def get_embeddings(num):
+            return [num, num, num]
+
+        # Create some items with vector embeddings
+        for i in range(10):
+            created_container.create_item({"id": "vector_item" + str(i), "embeddings": get_embeddings(i)})
+
+        # Run vector similarity search queries using VectorDistance
+        query = "SELECT TOP 5 c.id,VectorDistance(c.embeddings, [{}]) AS " \
+                "SimilarityScore FROM c ORDER BY VectorDistance(c.embeddings, [{}])".format(get_embeddings(1),
+                                                                                            get_embeddings(1))
+        await query_documents_with_custom_query(created_container, query)
+
+        # Run vector similarity search queries using VectorDistance with specifications
+        query = "SELECT TOP 5 c.id,VectorDistance(c.embeddings, [{}], true, {{'dataType': 'float32' ," \
+                " 'distanceFunction': 'cosine'}}) AS SimilarityScore FROM c ORDER BY VectorDistance(c.embeddings," \
+                " [{}], true, {{'dataType': 'float32', 'distanceFunction': 'cosine'}})".format(get_embeddings(1),
+                                                                                               get_embeddings(1))
+        await query_documents_with_custom_query(created_container, query)
+
+        # Cleanup
+        await db.delete_container(created_container)
+        print("\n")
+    except exceptions.CosmosResourceExistsError:
+        print("Entity already exists")
+    except exceptions.CosmosResourceNotFoundError:
+        print("Entity doesn't exist")
+
+
 async def run_sample():
     try:
         async with obtain_client() as client:
             await fetch_all_databases(client)
 
             # Create database if doesn't exist already.
             created_db = await client.create_database_if_not_exists(DATABASE_ID)
@@ -654,15 +719,15 @@
 
             # 7. Perform an index transform
             await perform_index_transformations(created_db)
 
             # 8. Perform Multi Orderby queries using composite indexes
             await perform_multi_orderby_query(created_db)
 
-            print('Sample done, cleaning up sample-generated data')
-            await client.delete_database(DATABASE_ID)
+            # 9. Create and use a vector embedding policy
+            await use_vector_embedding_policy(created_db)
 
     except exceptions.AzureError as e:
         raise e
 
 if __name__ == '__main__':
     asyncio.run(run_sample())
```

### Comparing `azure-cosmos-4.6.0/samples/tracing_open_telemetry.py` & `azure-cosmos-4.6.1/samples/tracing_open_telemetry.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/setup.py` & `azure-cosmos-4.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/conftest.py` & `azure-cosmos-4.6.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/routing/__init__.py` & `azure-cosmos-4.6.1/test/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/routing/test_collection_routing_map.py` & `azure-cosmos-4.6.1/test/routing/test_collection_routing_map.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/routing/test_routing_map_provider.py` & `azure-cosmos-4.6.1/test/routing/test_routing_map_provider.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_aad.py` & `azure-cosmos-4.6.1/test/test_aad.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_aggregate.py` & `azure-cosmos-4.6.1/test/test_aggregate.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # The MIT License (MIT)
 # Copyright (c) Microsoft Corporation. All rights reserved.
 
 from __future__ import print_function
 
+import os
 import unittest
 import uuid
 
 import pytest
 
 import azure.cosmos.cosmos_client as cosmos_client
 import azure.cosmos.documents as documents
@@ -52,14 +53,16 @@
                 "You must specify your Azure Cosmos account values for "
                 "'masterKey' and 'host' at the top of this class to run the "
                 "tests.")
 
         cls.client = cosmos_client.CosmosClient(_config.host, _config.master_key)
         cls.created_db = cls.client.get_database_client(test_config.TestConfig.TEST_DATABASE_ID)
         cls.created_collection = cls._create_collection(cls.created_db)
+        if _config.host == "https://localhost:8081/":
+            os.environ["AZURE_COSMOS_DISABLE_NON_STREAMING_ORDER_BY"] = "True"
 
         # test documents
         document_definitions = []
 
         values = [None, False, True, "abc", "cdfg", "opqrs", "ttttttt", "xyz", "oo", "ppp"]
         for value in values:
             d = {_config.PARTITION_KEY: value, 'id': str(uuid.uuid4())}
```

### Comparing `azure-cosmos-4.6.0/test/test_analytical_ttl.py` & `azure-cosmos-4.6.1/test/test_analytical_ttl.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_analytical_ttl_async.py` & `azure-cosmos-4.6.1/test/test_analytical_ttl_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_auto_scale.py` & `azure-cosmos-4.6.1/test/test_auto_scale.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_auto_scale_async.py` & `azure-cosmos-4.6.1/test/test_auto_scale_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_backwards_compatibility.py` & `azure-cosmos-4.6.1/test/test_backwards_compatibility.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_client_user_agent.py` & `azure-cosmos-4.6.1/test/test_client_user_agent.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_config.py` & `azure-cosmos-4.6.1/test/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,12 +152,35 @@
 
     @classmethod
     async def _validate_offset_limit(cls, created_collection, query, results):
         query_iterable = created_collection.query_items(query=query)
         assert list(map(lambda doc: doc['pk'], [item async for item in query_iterable])) == results
 
 
+def get_vector_indexing_policy(embedding_type):
+    return {
+        "indexingMode": "consistent",
+        "includedPaths": [{"path": "/*"}],
+        'excludedPaths': [{'path': '/"_etag"/?'}],
+        "vectorIndexes": [
+            {"path": "/embedding", "type": f"{embedding_type}"}
+        ]
+    }
+
+
+def get_vector_embedding_policy(distance_function, data_type, dimensions):
+    return {
+        "vectorEmbeddings": [
+            {
+                "path": "/embedding",
+                "dataType": f"{data_type}",
+                "dimensions": dimensions,
+                "distanceFunction": f"{distance_function}"
+            }
+        ]
+    }
+
 class FakeResponse:
     def __init__(self, headers):
         self.headers = headers
         self.reason = "foo"
         self.status_code = "bar"
```

### Comparing `azure-cosmos-4.6.0/test/test_cosmos_http_logging_policy.py` & `azure-cosmos-4.6.1/test/test_cosmos_http_logging_policy.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_crud.py` & `azure-cosmos-4.6.1/test/test_crud.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_crud_async.py` & `azure-cosmos-4.6.1/test/test_crud_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_crud_subpartition.py` & `azure-cosmos-4.6.1/test/test_crud_subpartition.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_crud_subpartition_async.py` & `azure-cosmos-4.6.1/test/test_crud_subpartition_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_diagnostics.py` & `azure-cosmos-4.6.1/test/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_encoding.py` & `azure-cosmos-4.6.1/test/test_encoding.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_globaldb.py` & `azure-cosmos-4.6.1/test/test_globaldb.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_globaldb_mock.py` & `azure-cosmos-4.6.1/test/test_globaldb_mock.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_headers.py` & `azure-cosmos-4.6.1/test/test_headers.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_integrated_cache.py` & `azure-cosmos-4.6.1/test/test_integrated_cache.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_location_cache.py` & `azure-cosmos-4.6.1/test/test_location_cache.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_multi_orderby.py` & `azure-cosmos-4.6.1/test/test_multi_orderby.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # The MIT License (MIT)
 # Copyright (c) Microsoft Corporation. All rights reserved.
 
 import random
 import unittest
 import uuid
+import os
 
 import pytest
 
 import azure.cosmos.cosmos_client as cosmos_client
 import test_config
 from azure.cosmos import DatabaseProxy
 from azure.cosmos.partition_key import PartitionKey
@@ -39,14 +40,16 @@
     client: cosmos_client.CosmosClient = None
     database: DatabaseProxy = None
 
     @classmethod
     def setUpClass(cls):
         cls.client = cosmos_client.CosmosClient(cls.host, cls.masterKey)
         cls.database = cls.client.get_database_client(cls.configs.TEST_DATABASE_ID)
+        if cls.host == "https://localhost:8081/":
+            os.environ["AZURE_COSMOS_DISABLE_NON_STREAMING_ORDER_BY"] = "True"
 
     def generate_multi_orderby_item(self):
         item = {'id': str(uuid.uuid4()), self.NUMBER_FIELD: random.randint(0, 5),
                 self.NUMBER_FIELD_2: random.randint(0, 5), self.BOOL_FIELD: random.randint(0, 2) % 2 == 0,
                 self.STRING_FIELD: str(random.randint(0, 5)), self.STRING_FIELD_2: str(random.randint(0, 5)),
                 self.NULL_FIELD: None, self.OBJECT_FIELD: "", self.ARRAY_FIELD: [],
                 self.SHORT_STRING_FIELD: "a" + str(random.randint(0, 100)),
```

### Comparing `azure-cosmos-4.6.0/test/test_multimaster.py` & `azure-cosmos-4.6.1/test/test_multimaster.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_murmurhash3.py` & `azure-cosmos-4.6.1/test/test_murmurhash3.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_orderby.py` & `azure-cosmos-4.6.1/test/test_orderby.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_partition_key.py` & `azure-cosmos-4.6.1/test/test_partition_key.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_proxy.py` & `azure-cosmos-4.6.1/test/test_proxy.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_query.py` & `azure-cosmos-4.6.1/test/test_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # The MIT License (MIT)
 # Copyright (c) Microsoft Corporation. All rights reserved.
 
+import os
 import unittest
 import uuid
-
+from datetime import datetime, timedelta, timezone
+from time import sleep
 import pytest
 
 import azure.cosmos._retry_utility as retry_utility
 import azure.cosmos.cosmos_client as cosmos_client
 import azure.cosmos.exceptions as exceptions
 import test_config
 from azure.cosmos import http_constants, DatabaseProxy
@@ -36,14 +38,16 @@
             raise Exception(
                 "You must specify your Azure Cosmos account values for "
                 "'masterKey' and 'host' at the top of this class to run the "
                 "tests.")
 
         cls.client = cosmos_client.CosmosClient(cls.host, cls.masterKey)
         cls.created_db = cls.client.get_database_client(cls.TEST_DATABASE_ID)
+        if cls.host == "https://localhost:8081/":
+            os.environ["AZURE_COSMOS_DISABLE_NON_STREAMING_ORDER_BY"] = "True"
 
     def test_first_and_last_slashes_trimmed_for_query_string(self):
         created_collection = self.created_db.create_container(
             "test_trimmed_slashes", PartitionKey(path="/pk"))
         doc_id = 'myId' + str(uuid.uuid4())
         document_definition = {'pk': 'pk', 'id': doc_id}
         created_collection.create_item(body=document_definition)
@@ -274,14 +278,80 @@
             is_start_from_beginning=True,
             **partitionParam
         )
         iter_list = list(query_iterable)
         self.assertEqual(len(iter_list), 0)
         self.created_db.delete_container(created_collection.id)
 
+    def test_query_change_feed_with_start_time(self):
+        created_collection = self.created_db.create_container_if_not_exists("query_change_feed_start_time_test",
+                                                                            PartitionKey(path="/pk"))
+        batchSize = 50
+
+        def round_time():
+            utc_now = datetime.now(timezone.utc)
+            return utc_now - timedelta(microseconds=utc_now.microsecond)
+        def create_random_items(container, batch_size):
+            for _ in range(batch_size):
+                # Generate a Random partition key
+                partition_key = 'pk' + str(uuid.uuid4())
+
+                # Generate a random item
+                item = {
+                    'id': 'item' + str(uuid.uuid4()),
+                    'partitionKey': partition_key,
+                    'content': 'This is some random content',
+                }
+
+                try:
+                    # Create the item in the container
+                    container.upsert_item(item)
+                except exceptions.CosmosHttpResponseError as e:
+                    self.fail(e)
+
+        # Create first batch of random items
+        create_random_items(created_collection, batchSize)
+
+        # wait for 1 second and record the time, then wait another second
+        sleep(1)
+        start_time = round_time()
+        not_utc_time = datetime.now()
+        sleep(1)
+
+        # now create another batch of items
+        create_random_items(created_collection, batchSize)
+
+        # now query change feed based on start time
+        change_feed_iter = list(created_collection.query_items_change_feed(start_time=start_time))
+        totalCount = len(change_feed_iter)
+
+        # now check if the number of items that were changed match the batch size
+        self.assertEqual(totalCount, batchSize)
+
+        # negative test: pass in a valid time in the future
+        future_time = start_time + timedelta(hours=1)
+        change_feed_iter = list(created_collection.query_items_change_feed(start_time=future_time))
+        totalCount = len(change_feed_iter)
+        # A future time should return 0
+        self.assertEqual(totalCount, 0)
+
+        # test a date that is not utc, will be converted to utc by sdk
+        change_feed_iter = list(created_collection.query_items_change_feed(start_time=not_utc_time))
+        totalCount = len(change_feed_iter)
+        # Should equal batch size
+        self.assertEqual(totalCount, batchSize)
+
+        # test an invalid value, Attribute error will be raised for passing non datetime object
+        invalid_time = "Invalid value"
+        try:
+            change_feed_iter = list(created_collection.query_items_change_feed(start_time=invalid_time))
+            self.fail("Cannot format date on a non datetime object.")
+        except AttributeError as e:
+            self.assertTrue("'str' object has no attribute 'astimezone'" == e.args[0])
+
     def test_populate_query_metrics(self):
         created_collection = self.created_db.create_container("query_metrics_test",
                                                               PartitionKey(path="/pk"))
         doc_id = 'MyId' + str(uuid.uuid4())
         document_definition = {'pk': 'pk', 'id': doc_id}
         created_collection.create_item(body=document_definition)
```

### Comparing `azure-cosmos-4.6.0/test/test_query_async.py` & `azure-cosmos-4.6.1/test/test_query_async.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # The MIT License (MIT)
 # Copyright (c) Microsoft Corporation. All rights reserved.
 
+import os
 import unittest
 import uuid
+from asyncio import sleep, gather
+from datetime import datetime, timedelta, timezone
 
 import pytest
 
 import azure.cosmos.aio._retry_utility_async as retry_utility
 import azure.cosmos.exceptions as exceptions
 import test_config
 from azure.cosmos import http_constants
 from azure.cosmos._execution_context.query_execution_info import _PartitionedQueryExecutionInfo
 from azure.cosmos.aio import CosmosClient, DatabaseProxy, ContainerProxy
 from azure.cosmos.documents import _DistinctType
 from azure.cosmos.partition_key import PartitionKey
+from azure.cosmos._retry_options import RetryOptions
 
 
 @pytest.mark.cosmosEmulator
 class TestQueryAsync(unittest.IsolatedAsyncioTestCase):
     """Test to ensure escaping of non-ascii characters from partition key"""
 
     created_db: DatabaseProxy = None
@@ -38,14 +42,16 @@
                 "You must specify your Azure Cosmos account values for "
                 "'masterKey' and 'host' at the top of this class to run the "
                 "tests.")
 
     async def asyncSetUp(self):
         self.client = CosmosClient(self.host, self.masterKey)
         self.created_db = self.client.get_database_client(self.TEST_DATABASE_ID)
+        if self.host == "https://localhost:8081/":
+            os.environ["AZURE_COSMOS_DISABLE_NON_STREAMING_ORDER_BY"] = "True"
 
     async def asyncTearDown(self):
         await self.client.close()
 
     async def test_first_and_last_slashes_trimmed_for_query_string_async(self):
         created_collection = await self.created_db.create_container(
             str(uuid.uuid4()), PartitionKey(path="/pk"))
@@ -312,16 +318,85 @@
             continuation=continuation3,
             is_start_from_beginning=True,
             **partition_param
         )
         iter_list = [item async for item in query_iterable]
         assert len(iter_list) == 0
 
+    @pytest.mark.asyncio
+    async def test_query_change_feed_with_start_time(self):
+        created_collection = await self.created_db.create_container_if_not_exists("query_change_feed_start_time_test",
+                                                                                  PartitionKey(path="/pk"))
+        batchSize = 50
+
+        def round_time():
+            utc_now = datetime.now(timezone.utc)
+            return utc_now - timedelta(microseconds=utc_now.microsecond)
+
+        async def create_random_items(container, batch_size):
+            for _ in range(batch_size):
+                # Generate a Random partition key
+                partition_key = 'pk' + str(uuid.uuid4())
+
+                # Generate a random item
+                item = {
+                    'id': 'item' + str(uuid.uuid4()),
+                    'partitionKey': partition_key,
+                    'content': 'This is some random content',
+                }
+
+                try:
+                    # Create the item in the container
+                    await container.upsert_item(item)
+                except exceptions.CosmosHttpResponseError as e:
+                    pytest.fail(e)
+
+        # Create first batch of random items
+        await create_random_items(created_collection, batchSize)
+
+        # wait for 1 second and record the time, then wait another second
+        await sleep(1)
+        start_time = round_time()
+        not_utc_time = datetime.now()
+        await sleep(1)
+
+        # now create another batch of items
+        await create_random_items(created_collection, batchSize)
+
+        # now query change feed based on start time
+        change_feed_iter = [i async for i in created_collection.query_items_change_feed(start_time=start_time)]
+        totalCount = len(change_feed_iter)
+
+        # now check if the number of items that were changed match the batch size
+        assert totalCount == batchSize
+
+        # negative test: pass in a valid time in the future
+        future_time = start_time + timedelta(hours=1)
+        change_feed_iter = [i async for i in created_collection.query_items_change_feed(start_time=future_time)]
+        totalCount = len(change_feed_iter)
+        # A future time should return 0
+        assert totalCount == 0
+
+        # test a date that is not utc, will be converted to utc by sdk
+        change_feed_iter = [i async for i in created_collection.query_items_change_feed(start_time=not_utc_time)]
+        totalCount = len(change_feed_iter)
+        # Should equal batch size
+        assert totalCount == batchSize
+
+        # test an invalid value, Attribute error will be raised for passing non datetime object
+        invalid_time = "Invalid value"
+        try:
+            change_feed_iter = [i async for i in created_collection.query_items_change_feed(start_time=invalid_time)]
+            self.fail("Cannot format date on a non datetime object.")
+        except AttributeError as e:
+            assert ("'str' object has no attribute 'astimezone'" == e.args[0])
+
         await self.created_db.delete_container(created_collection.id)
 
+    @pytest.mark.asyncio
     async def test_populate_query_metrics_async(self):
         created_collection = await self.created_db.create_container(
             "query_metrics_test" + str(uuid.uuid4()),
             PartitionKey(path="/pk"))
         doc_id = 'MyId' + str(uuid.uuid4())
         document_definition = {'pk': 'pk', 'id': doc_id}
         await created_collection.create_item(body=document_definition)
@@ -805,10 +880,62 @@
         assert len(queried_items) == 2
 
         # Test 3 Negative: Test Str length that isn't there
         queried_items = [q async for q in created_collection.query_items(query='Select * from c Where c.cp_str_len = 3',
                                                                          partition_key="test")]
         assert len(queried_items) == 0
 
+    async def test_cosmos_query_retryable_error_async(self):
+        async def query_items(database):
+            # Tests to make sure 429 exception is surfaced when retries run out in the first page of a query.
+            try:
+                container = await database.create_container(
+                    id="query_retryable_error_test", partition_key=PartitionKey(path="/pk"), offer_throughput=400
+                )
+            except exceptions.CosmosResourceExistsError:
+                container = database.get_container_client("query_retryable_error_test")
+            query = "SELECT * FROM c"
+            try:
+                query_iterable = [d async for d in container.query_items(query, max_item_count=10)]
+                if len(query_iterable) == 0:
+                    # Query should not return empty if it has items to query on a retryable exception is raised
+                    pytest.fail("Expected 429 Exception.")
+            except exceptions.CosmosHttpResponseError as ex:
+                # A retryable exception should be surfaced when retries run out
+                assert ex.status_code == 429
+
+        created_collection = await self.created_db.create_container_if_not_exists("query_retryable_error_test",
+                                                                                  PartitionKey(path="/pk"))
+        # Created items to query
+        for _ in range(150):
+            # Generate a Random partition key
+            partition_key = 'pk' + str(uuid.uuid4())
+
+            # Generate a random item
+            item = {
+                'id': 'item' + str(uuid.uuid4()),
+                'partitionKey': partition_key,
+                'content': 'This is some random content',
+            }
+
+            try:
+                # Create the item in the container
+                await created_collection.upsert_item(item)
+            except exceptions.CosmosHttpResponseError as e:
+                pytest.fail(e)
+        # Set retry options to fail much more easily to avoid too much concurrency
+        retry_options = RetryOptions(max_retry_attempt_count=1,
+                                     fixed_retry_interval_in_milliseconds=1, max_wait_time_in_seconds=1)
+        old_retry = self.client.client_connection.connection_policy.RetryOptions
+        self.client.client_connection.connection_policy.RetryOptions = retry_options
+        created_collection = await self.created_db.create_container_if_not_exists("query_retryable_error_test",
+                                                                                  PartitionKey(path="/pk"))
+        # Force a 429 exception by having multiple concurrent queries.
+        num_queries = 4
+        await gather(*[query_items(self.created_db) for _ in range(num_queries)])
+
+        self.client.client_connection.connection_policy.RetryOptions = old_retry
+        await self.created_db.delete_container(created_collection.id)
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `azure-cosmos-4.6.0/test/test_query_computed_properties.py` & `azure-cosmos-4.6.1/test/test_query_computed_properties.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_query_computed_properties_async.py` & `azure-cosmos-4.6.1/test/test_query_computed_properties_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_query_cross_partition.py` & `azure-cosmos-4.6.1/test/test_query_cross_partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # The MIT License (MIT)
 # Copyright (c) Microsoft Corporation. All rights reserved.
 
+import os
 import unittest
 import uuid
 
 import pytest
 
 import azure.cosmos.cosmos_client as cosmos_client
 import azure.cosmos.exceptions as exceptions
@@ -36,14 +37,16 @@
             raise Exception(
                 "You must specify your Azure Cosmos account values for "
                 "'masterKey' and 'host' at the top of this class to run the "
                 "tests.")
 
         cls.client = cosmos_client.CosmosClient(cls.host, cls.masterKey)
         cls.created_db = cls.client.get_database_client(cls.TEST_DATABASE_ID)
+        if cls.host == "https://localhost:8081/":
+            os.environ["AZURE_COSMOS_DISABLE_NON_STREAMING_ORDER_BY"] = "True"
 
     def setUp(self):
         self.created_container = self.created_db.create_container(
             id=self.TEST_CONTAINER_ID,
             partition_key=PartitionKey(path="/pk"),
             offer_throughput=test_config.TestConfig.THROUGHPUT_FOR_5_PARTITIONS)
```

### Comparing `azure-cosmos-4.6.0/test/test_query_cross_partition_async.py` & `azure-cosmos-4.6.1/test/test_query_cross_partition_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # The MIT License (MIT)
 # Copyright (c) Microsoft Corporation. All rights reserved.
 
+import os
 import unittest
 import uuid
 
 import pytest
 
 import azure.cosmos.aio._retry_utility_async as retry_utility
 import azure.cosmos.exceptions as exceptions
@@ -42,14 +43,16 @@
     async def asyncSetUp(self):
         self.client = CosmosClient(self.host, self.masterKey)
         self.created_db = self.client.get_database_client(self.TEST_DATABASE_ID)
         self.created_container = await self.created_db.create_container(
             self.TEST_CONTAINER_ID,
             PartitionKey(path="/pk"),
             offer_throughput=test_config.TestConfig.THROUGHPUT_FOR_5_PARTITIONS)
+        if self.host == "https://localhost:8081/":
+            os.environ["AZURE_COSMOS_DISABLE_NON_STREAMING_ORDER_BY"] = "True"
 
     async def asyncTearDown(self):
         try:
             await self.created_db.delete_container(self.TEST_CONTAINER_ID)
         except CosmosHttpResponseError:
             pass
         finally:
```

### Comparing `azure-cosmos-4.6.0/test/test_query_execution_context.py` & `azure-cosmos-4.6.1/test/test_query_execution_context.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_resource_id.py` & `azure-cosmos-4.6.1/test/test_resource_id.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_resource_id_async.py` & `azure-cosmos-4.6.1/test/test_resource_id_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_retry_policy.py` & `azure-cosmos-4.6.1/test/test_retry_policy.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_routing_map.py` & `azure-cosmos-4.6.1/test/test_routing_map.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_session.py` & `azure-cosmos-4.6.1/test/test_session.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_session_container.py` & `azure-cosmos-4.6.1/test/test_session_container.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_session_token_unit.py` & `azure-cosmos-4.6.1/test/test_session_token_unit.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_streaming_failover.py` & `azure-cosmos-4.6.1/test/test_streaming_failover.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_transactional_batch.py` & `azure-cosmos-4.6.1/test/test_transactional_batch.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_transactional_batch_async.py` & `azure-cosmos-4.6.1/test/test_transactional_batch_async.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_ttl.py` & `azure-cosmos-4.6.1/test/test_ttl.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_user_configs.py` & `azure-cosmos-4.6.1/test/test_user_configs.py`

 * *Files identical despite different names*

### Comparing `azure-cosmos-4.6.0/test/test_utils.py` & `azure-cosmos-4.6.1/test/test_utils.py`

 * *Files identical despite different names*

