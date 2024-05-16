# Comparing `tmp/buildgrid-0.0.94.tar.gz` & `tmp/buildgrid-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildgrid-0.0.94.tar", last modified: Mon Apr 29 15:22:12 2024, max compression
+gzip compressed data, was "buildgrid-0.0.95.tar", last modified: Thu May 16 13:10:20 2024, max compression
```

## Comparing `buildgrid-0.0.94.tar` & `buildgrid-0.0.95.tar`

### file list

```diff
@@ -1,498 +1,498 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.272567 buildgrid-0.0.94/
--rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-29 15:21:45.000000 buildgrid-0.0.94/BuildGrid.doap
--rw-rw-rw-   0 root         (0) root         (0)     9648 2024-04-29 15:21:45.000000 buildgrid-0.0.94/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    11338 2024-04-29 15:21:45.000000 buildgrid-0.0.94/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      500 2024-04-29 15:21:45.000000 buildgrid-0.0.94/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6931 2024-04-29 15:22:12.272567 buildgrid-0.0.94/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2868 2024-04-29 15:21:45.000000 buildgrid-0.0.94/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.162566 buildgrid-0.0.94/buildgrid/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.164566 buildgrid-0.0.94/buildgrid/_app/
--rw-rw-rw-   0 root         (0) root         (0)      621 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5661 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.167566 buildgrid-0.0.94/buildgrid/_app/commands/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6755 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_actioncache.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_browser_backend.py
--rw-rw-rw-   0 root         (0) root         (0)     3170 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_capabilities.py
--rw-rw-rw-   0 root         (0) root         (0)    10608 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_cas.py
--rw-rw-rw-   0 root         (0) root         (0)     8817 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_cleanup.py
--rw-rw-rw-   0 root         (0) root         (0)    12570 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_execute.py
--rw-rw-rw-   0 root         (0) root         (0)     2840 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_janitor.py
--rw-rw-rw-   0 root         (0) root         (0)     4842 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_logstream.py
--rw-rw-rw-   0 root         (0) root         (0)    11215 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_operation.py
--rw-rw-rw-   0 root         (0) root         (0)     8166 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/cmd_server.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/commands/rpc_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.168566 buildgrid-0.0.94/buildgrid/_app/settings/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   110917 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     8691 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/reference.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.168566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.169566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/caches/
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/caches/lru-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      204 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/caches/mirrored-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      676 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/caches/with-cache.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.170566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/clients/
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/clients/asset-client.yaml
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2785 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.170566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/connections/
--rw-rw-rw-   0 root         (0) root         (0)      403 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/connections/redis.yaml
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/connections/sql.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.171566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/misc/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/misc/channel.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.171566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/scheduler/
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/scheduler/memory.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3907 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/scheduler/sql.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.173566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      971 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/bots.yaml
--rw-rw-rw-   0 root         (0) root         (0)      343 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/bytestream.yaml
--rw-rw-rw-   0 root         (0) root         (0)      273 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/cas.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1557 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/execution.yaml
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/platform-queues.yml
--rw-rw-rw-   0 root         (0) root         (0)      596 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/s3-action-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/write-once-action-cache.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.177566 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/disk.yaml
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/lru.yaml
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/operations_sql_storage.yaml
--rw-rw-rw-   0 root         (0) root         (0)      207 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/redis-index.yaml
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/redis.yaml
--rw-rw-rw-   0 root         (0) root         (0)      601 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/remote.yaml
--rw-rw-rw-   0 root         (0) root         (0)      270 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/replicated.yaml
--rw-rw-rw-   0 root         (0) root         (0)      592 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/s3.yaml
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/sharded.yaml
--rw-rw-rw-   0 root         (0) root         (0)      530 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/sql-index.yaml
--rw-rw-rw-   0 root         (0) root         (0)      177 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/sql.yaml
--rw-rw-rw-   0 root         (0) root         (0)      281 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/with-cache.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4776 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_enums.py
--rw-rw-rw-   0 root         (0) root         (0)     8802 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.177566 buildgrid-0.0.94/buildgrid/_protos/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.177566 buildgrid-0.0.94/buildgrid/_protos/build/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.177566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.178566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.178566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.180566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7795 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    27103 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    16783 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    15404 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    16783 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)    15550 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.180566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.182566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    30140 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)   136470 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    59894 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)    47588 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    59894 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)    47884 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.183566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.185566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2066 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3176 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    12298 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7788 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    12298 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7844 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.186566 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1484 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     2068 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      635 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.188566 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1944 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4156 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.188566 buildgrid-0.0.94/buildgrid/_protos/buildgrid/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.193566 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3156 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    10940 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     3824 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     9955 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2881 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3433 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2872 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2872 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     1561 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.193566 buildgrid-0.0.94/buildgrid/_protos/google/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.199566 buildgrid-0.0.94/buildgrid/_protos/google/api/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     1089 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1622 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1926 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     6343 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2291 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18246 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.201566 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3246 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     7478 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10732 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     8880 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10732 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     8996 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.201566 buildgrid-0.0.94/buildgrid/_protos/google/devtools/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.201566 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.206566 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5933 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18014 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2545 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     5408 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6758 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    10427 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     5461 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     8451 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     5547 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.206566 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.212566 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7859 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    23457 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    11879 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7140 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    11879 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7256 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     6133 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    21890 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     5337 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     9321 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)     7651 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)     7651 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     4498 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2751 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    11299 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.214566 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5084 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     7984 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10950 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)     7133 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)    10950 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)     7279 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.218567 buildgrid-0.0.94/buildgrid/_protos/google/rpc/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1890 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    13407 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     4774 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)    18695 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      627 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1573 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     4889 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2_grpc.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi
--rw-rw-rw-   0 root         (0) root         (0)      159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1358 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_types.py
--rw-rw-rw-   0 root         (0) root         (0)      604 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.219566 buildgrid-0.0.94/buildgrid/browser/
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/browser/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4469 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/browser/app.py
--rw-rw-rw-   0 root         (0) root         (0)    34436 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/browser/rest_api.py
--rw-rw-rw-   0 root         (0) root         (0)     2277 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/browser/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.220566 buildgrid-0.0.94/buildgrid/cleanup/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/cleanup/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10716 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/cleanup/cleanup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.221567 buildgrid-0.0.94/buildgrid/cleanup/janitor/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/cleanup/janitor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1745 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/cleanup/janitor/config.py
--rw-rw-rw-   0 root         (0) root         (0)     3318 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/cleanup/janitor/index.py
--rw-rw-rw-   0 root         (0) root         (0)     4565 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/cleanup/janitor/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     1403 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/cleanup/janitor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.224567 buildgrid-0.0.94/buildgrid/client/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5099 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/actioncache.py
--rw-rw-rw-   0 root         (0) root         (0)     4361 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/asset.py
--rw-rw-rw-   0 root         (0) root         (0)     1631 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/auth_token_loader.py
--rw-rw-rw-   0 root         (0) root         (0)     5113 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/authentication.py
--rwxrwxrwx   0 root         (0) root         (0)     1650 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/capabilities.py
--rw-rw-rw-   0 root         (0) root         (0)    41408 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/cas.py
--rw-rw-rw-   0 root         (0) root         (0)    13926 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/channel.py
--rw-rw-rw-   0 root         (0) root         (0)     4437 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/interceptors.py
--rw-rw-rw-   0 root         (0) root         (0)     2012 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/logstream.py
--rw-rw-rw-   0 root         (0) root         (0)     3410 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/client/retrier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.227567 buildgrid-0.0.94/buildgrid/server/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.227567 buildgrid-0.0.94/buildgrid/server/actioncache/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.230567 buildgrid-0.0.94/buildgrid/server/actioncache/caches/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5564 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/action_cache_abc.py
--rw-rw-rw-   0 root         (0) root         (0)     5593 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4197 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/mirrored_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     6534 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/redis_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     6573 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/remote_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    11662 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/s3_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     4686 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/with_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3341 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/caches/write_once_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3623 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     4045 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/actioncache/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.231567 buildgrid-0.0.94/buildgrid/server/auth/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2363 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/auth/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1905 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/auth/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1599 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/auth/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    15244 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/auth/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.231567 buildgrid-0.0.94/buildgrid/server/bots/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/bots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11156 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/bots/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     7343 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/bots/job_assigner.py
--rw-rw-rw-   0 root         (0) root         (0)     5647 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/bots/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.232566 buildgrid-0.0.94/buildgrid/server/build_events/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/build_events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6045 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/build_events/service.py
--rw-rw-rw-   0 root         (0) root         (0)     7213 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/build_events/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.233567 buildgrid-0.0.94/buildgrid/server/capabilities/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/capabilities/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7113 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/capabilities/instance.py
--rwxrwxrwx   0 root         (0) root         (0)     3342 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/capabilities/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.234567 buildgrid-0.0.94/buildgrid/server/cas/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21601 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/instance.py
--rw-rw-rw-   0 root         (0) root         (0)    12330 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.237567 buildgrid-0.0.94/buildgrid/server/cas/storage/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3702 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.238566 buildgrid-0.0.94/buildgrid/server/cas/storage/index/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/index/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3335 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/index/index_abc.py
--rw-rw-rw-   0 root         (0) root         (0)    13464 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/index/redis.py
--rw-rw-rw-   0 root         (0) root         (0)    38426 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.239567 buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql_dialect_delegates/
--rw-rw-rw-   0 root         (0) root         (0)      146 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql_dialect_delegates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2136 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py
--rw-rw-rw-   0 root         (0) root         (0)     2120 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py
--rw-rw-rw-   0 root         (0) root         (0)     4436 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/lru_memory_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     5330 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/redis.py
--rw-rw-rw-   0 root         (0) root         (0)     8601 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/remote.py
--rw-rw-rw-   0 root         (0) root         (0)    11295 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/replicated.py
--rw-rw-rw-   0 root         (0) root         (0)    14426 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     6002 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/sharded.py
--rw-rw-rw-   0 root         (0) root         (0)     6985 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/size_differentiated.py
--rw-rw-rw-   0 root         (0) root         (0)     9519 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/sql.py
--rw-rw-rw-   0 root         (0) root         (0)     8154 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/storage_abc.py
--rw-rw-rw-   0 root         (0) root         (0)     7796 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/cas/storage/with_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     3029 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/context.py
--rw-rw-rw-   0 root         (0) root         (0)     2194 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.239567 buildgrid-0.0.94/buildgrid/server/execution/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/execution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9599 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/execution/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     7517 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/execution/service.py
--rw-rw-rw-   0 root         (0) root         (0)     3813 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/job_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    18608 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/metrics_names.py
--rw-rw-rw-   0 root         (0) root         (0)    14482 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/metrics_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    19548 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/monitoring.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.240567 buildgrid-0.0.94/buildgrid/server/operations/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.242567 buildgrid-0.0.94/buildgrid/server/operations/filtering/
--rw-rw-rw-   0 root         (0) root         (0)      813 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/filtering/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/filtering/filter.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/filtering/filter_grammar.lark
--rw-rw-rw-   0 root         (0) root         (0)     5769 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/filtering/interpreter.py
--rw-rw-rw-   0 root         (0) root         (0)     2510 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/filtering/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4594 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/filtering/sanitizer.py
--rw-rw-rw-   0 root         (0) root         (0)     4802 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/instance.py
--rw-rw-rw-   0 root         (0) root         (0)     6034 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/operations/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.242567 buildgrid-0.0.94/buildgrid/server/persistence/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.243567 buildgrid-0.0.94/buildgrid/server/persistence/sql/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.244567 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/README
--rw-rw-rw-   0 root         (0) root         (0)     2919 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/env.py
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.249567 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/
--rw-rw-rw-   0 root         (0) root         (0)     1127 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)     1718 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py
--rw-rw-rw-   0 root         (0) root         (0)     1250 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py
--rw-rw-rw-   0 root         (0) root         (0)     1463 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py
--rw-rw-rw-   0 root         (0) root         (0)     2422 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py
--rw-rw-rw-   0 root         (0) root         (0)     1269 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py
--rw-rw-rw-   0 root         (0) root         (0)     1155 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py
--rw-rw-rw-   0 root         (0) root         (0)     1581 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py
--rw-rw-rw-   0 root         (0) root         (0)     1793 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py
--rw-rw-rw-   0 root         (0) root         (0)     2343 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py
--rw-rw-rw-   0 root         (0) root         (0)     1191 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py
--rw-rw-rw-   0 root         (0) root         (0)     1211 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py
--rw-rw-rw-   0 root         (0) root         (0)     1418 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py
--rw-rw-rw-   0 root         (0) root         (0)     4625 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py
--rw-rw-rw-   0 root         (0) root         (0)     2072 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py
--rw-rw-rw-   0 root         (0) root         (0)    79716 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/impl.py
--rw-rw-rw-   0 root         (0) root         (0)     8915 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/models.py
--rw-rw-rw-   0 root         (0) root         (0)     6206 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/notifier.py
--rw-rw-rw-   0 root         (0) root         (0)    10298 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/persistence/sql/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.249567 buildgrid-0.0.94/buildgrid/server/redis/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/redis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6197 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/redis/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     4739 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/request_metadata_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.250567 buildgrid-0.0.94/buildgrid/server/s3/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/s3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18695 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/s3/s3utils.py
--rw-rw-rw-   0 root         (0) root         (0)    30687 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/server.py
--rw-rw-rw-   0 root         (0) root         (0)     6126 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/servicer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.251567 buildgrid-0.0.94/buildgrid/server/sql/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/sql/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    22206 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/sql/provider.py
--rw-rw-rw-   0 root         (0) root         (0)     6225 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/sql/sqlutils.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/threading.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.252567 buildgrid-0.0.94/buildgrid/server/utils/
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4484 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/utils/async_lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/utils/context.py
--rw-rw-rw-   0 root         (0) root         (0)    10885 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/server/utils/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     5450 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/settings.py
--rw-rw-rw-   0 root         (0) root         (0)    12244 2024-04-29 15:21:45.000000 buildgrid-0.0.94/buildgrid/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.265567 buildgrid-0.0.94/buildgrid.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6931 2024-04-29 15:22:12.000000 buildgrid-0.0.94/buildgrid.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    21169 2024-04-29 15:22:12.000000 buildgrid-0.0.94/buildgrid.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-29 15:22:12.000000 buildgrid-0.0.94/buildgrid.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-04-29 15:22:12.000000 buildgrid-0.0.94/buildgrid.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)     1213 2024-04-29 15:22:12.000000 buildgrid-0.0.94/buildgrid.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-29 15:22:12.000000 buildgrid-0.0.94/buildgrid.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.157566 buildgrid-0.0.94/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.256567 buildgrid-0.0.94/data/config/
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/all-in-one.yml
--rw-rw-rw-   0 root         (0) root         (0)      588 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/artifacts.yml
--rwxrwxrwx   0 root         (0) root         (0)     1351 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/basic-with-disk.yml
--rw-rw-rw-   0 root         (0) root         (0)     1159 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/bots-interface.yml
--rw-rw-rw-   0 root         (0) root         (0)      896 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/cache.yml
--rw-rw-rw-   0 root         (0) root         (0)     1302 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/controller.yml
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/default.yml
--rw-rw-rw-   0 root         (0) root         (0)      832 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/index-sqlite-no-execution.yml
--rw-rw-rw-   0 root         (0) root         (0)     1571 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/index-sqlite.yml
--rw-rw-rw-   0 root         (0) root         (0)      247 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/logstream.yml
--rw-rw-rw-   0 root         (0) root         (0)     1239 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/monitoring-controller.yml
--rw-rw-rw-   0 root         (0) root         (0)     1143 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/multi-layer-storage.yml
--rw-rw-rw-   0 root         (0) root         (0)     1474 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/redis-cache.yml
--rw-rw-rw-   0 root         (0) root         (0)     1067 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/s3-indexed-cas.yml
--rw-rw-rw-   0 root         (0) root         (0)     1270 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/storage-redis.yml
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/storage-s3.yml
--rw-rw-rw-   0 root         (0) root         (0)      900 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/storage.yml
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/with-metering.yml
--rw-rw-rw-   0 root         (0) root         (0)     1478 2024-04-29 15:21:45.000000 buildgrid-0.0.94/data/config/with-pgbouncer.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.256567 buildgrid-0.0.94/docs/
--rw-rw-rw-   0 root         (0) root         (0)      610 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.257567 buildgrid-0.0.94/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.258567 buildgrid-0.0.94/docs/source/data/
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/data/basic-disk-cas.yml
--rw-rw-rw-   0 root         (0) root         (0)      492 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/data/bazel-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      490 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/data/buildstream-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      446 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/data/cas-and-ac.yml
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/data/cas-example-server.yml
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/data/execution-and-bots.yml
--rw-rw-rw-   0 root         (0) root         (0)      531 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/data/sqlite-index-cas-only.yml
--rw-rw-rw-   0 root         (0) root         (0)     1425 2024-04-29 15:21:45.000000 buildgrid-0.0.94/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5436 2024-04-29 15:21:45.000000 buildgrid-0.0.94/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-04-29 15:22:12.272567 buildgrid-0.0.94/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      643 2024-04-29 15:21:45.000000 buildgrid-0.0.94/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.261567 buildgrid-0.0.94/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.158566 buildgrid-0.0.94/tests/auth/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-29 15:22:12.264567 buildgrid-0.0.94/tests/auth/data/
--rw-rw-rw-   0 root         (0) root         (0)      733 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/auth.yaml
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwks-valid.json
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-hs256-conflicting.secret
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-hs256-expired.token
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-hs256-matching.secret
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-hs256-unbounded.token
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-hs256-valid.token
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-rs256-conflicting.pub.key
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-rs256-expired.token
--rw-rw-rw-   0 root         (0) root         (0)      559 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-rs256-jwk-encrypted.token
--rw-rw-rw-   0 root         (0) root         (0)      886 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-rs256-matching.priv.key
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-rs256-matching.pub.key
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-rs256-unbounded.token
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/auth/data/jwt-rs256-valid.token
--rw-rw-rw-   0 root         (0) root         (0)     3829 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_async_lru_cache.py
--rw-rw-rw-   0 root         (0) root         (0)    15407 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_execution_instance.py
--rw-rw-rw-   0 root         (0) root         (0)     2199 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_job_assigner.py
--rw-rw-rw-   0 root         (0) root         (0)    12358 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_metrics_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3447 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_mirrored_cache.py
--rw-rw-rw-   0 root         (0) root         (0)     2098 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_multithreaded_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1368 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2777 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_request_metadata_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    32384 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_scheduler.py
--rw-rw-rw-   0 root         (0) root         (0)    10567 2024-04-29 15:21:45.000000 buildgrid-0.0.94/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.624997 buildgrid-0.0.95/
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-05-16 13:09:51.000000 buildgrid-0.0.95/BuildGrid.doap
+-rw-rw-rw-   0 root         (0) root         (0)     9648 2024-05-16 13:09:51.000000 buildgrid-0.0.95/CONTRIBUTING.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11338 2024-05-16 13:09:51.000000 buildgrid-0.0.95/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      500 2024-05-16 13:09:51.000000 buildgrid-0.0.95/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7030 2024-05-16 13:10:20.624997 buildgrid-0.0.95/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2024-05-16 13:09:51.000000 buildgrid-0.0.95/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.521998 buildgrid-0.0.95/buildgrid/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.523998 buildgrid-0.0.95/buildgrid/_app/
+-rw-rw-rw-   0 root         (0) root         (0)      621 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5675 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.525998 buildgrid-0.0.95/buildgrid/_app/commands/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6755 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_actioncache.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_browser_backend.py
+-rw-rw-rw-   0 root         (0) root         (0)     3170 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    10608 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_cas.py
+-rw-rw-rw-   0 root         (0) root         (0)     8817 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_cleanup.py
+-rw-rw-rw-   0 root         (0) root         (0)    12570 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     2840 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_janitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4842 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_logstream.py
+-rw-rw-rw-   0 root         (0) root         (0)    11215 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_operation.py
+-rw-rw-rw-   0 root         (0) root         (0)     8166 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/cmd_server.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/commands/rpc_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.526998 buildgrid-0.0.95/buildgrid/_app/settings/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   110867 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     8691 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/reference.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.527998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.528998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/caches/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/caches/lru-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/caches/mirrored-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      676 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/caches/with-cache.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.528998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/clients/
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/clients/asset-client.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.528998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/connections/
+-rw-rw-rw-   0 root         (0) root         (0)      403 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/connections/redis.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/connections/sql.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.529998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/misc/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/misc/channel.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.529998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/scheduler/
+-rw-rw-rw-   0 root         (0) root         (0)      155 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/scheduler/memory.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3907 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/scheduler/sql.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.531998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      971 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/bots.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      343 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/bytestream.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      273 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/cas.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1557 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/execution.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/platform-queues.yml
+-rw-rw-rw-   0 root         (0) root         (0)      596 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/s3-action-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/write-once-action-cache.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.534998 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/disk.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/lru.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      264 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/operations_sql_storage.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      207 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/redis-index.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/redis.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      601 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/remote.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      270 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/replicated.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      592 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/s3.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/sharded.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      530 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/sql-index.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      177 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/sql.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      281 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/with-cache.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4776 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     8802 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.534998 buildgrid-0.0.95/buildgrid/_protos/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.535998 buildgrid-0.0.95/buildgrid/_protos/build/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.535998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.535998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.535998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.537998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7795 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    27103 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    16783 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)    15404 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    16783 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)    15550 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.537998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.539998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    30140 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)   136470 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    59894 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)    47588 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    59894 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)    47884 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.540998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.541998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2066 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3176 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    12298 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7788 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    12298 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7844 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.543998 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      635 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.545998 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1944 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4156 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.545998 buildgrid-0.0.95/buildgrid/_protos/buildgrid/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.549998 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3156 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10940 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     3824 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     9955 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2881 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3433 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2872 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2872 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     1561 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.549998 buildgrid-0.0.95/buildgrid/_protos/google/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.555998 buildgrid-0.0.95/buildgrid/_protos/google/api/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1089 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1622 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1926 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     6343 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18246 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.556998 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3246 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7478 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10732 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     8880 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10732 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     8996 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.557998 buildgrid-0.0.95/buildgrid/_protos/google/devtools/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.557998 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.561998 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5933 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18014 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2545 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5408 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     6758 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    10427 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     8451 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5461 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     8451 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     5547 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.562998 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.568998 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7859 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    23457 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    11879 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7140 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    11879 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7256 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     6133 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    21890 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     5337 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     9321 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4382 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     4498 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2751 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    11299 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.569998 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5084 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     7984 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10950 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7133 2024-05-16 13:09:51.000000 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    10950 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)     7279 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.574998 buildgrid-0.0.95/buildgrid/_protos/google/rpc/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    13407 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     4774 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)    18695 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      627 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1573 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     4889 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2_grpc.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      159 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1358 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      604 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.575998 buildgrid-0.0.95/buildgrid/browser/
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/browser/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4469 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/browser/app.py
+-rw-rw-rw-   0 root         (0) root         (0)    34436 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/browser/rest_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/browser/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.575998 buildgrid-0.0.95/buildgrid/cleanup/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/cleanup/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10716 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/cleanup/cleanup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.576998 buildgrid-0.0.95/buildgrid/cleanup/janitor/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/cleanup/janitor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/cleanup/janitor/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3318 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/cleanup/janitor/index.py
+-rw-rw-rw-   0 root         (0) root         (0)     5829 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/cleanup/janitor/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     1403 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/cleanup/janitor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.579998 buildgrid-0.0.95/buildgrid/client/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5099 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/actioncache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4361 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/asset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1631 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/auth_token_loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/authentication.py
+-rwxrwxrwx   0 root         (0) root         (0)     1650 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/capabilities.py
+-rw-rw-rw-   0 root         (0) root         (0)    41408 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/cas.py
+-rw-rw-rw-   0 root         (0) root         (0)    13926 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/channel.py
+-rw-rw-rw-   0 root         (0) root         (0)     4437 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/interceptors.py
+-rw-rw-rw-   0 root         (0) root         (0)     2012 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/logstream.py
+-rw-rw-rw-   0 root         (0) root         (0)     3410 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/client/retrier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.582998 buildgrid-0.0.95/buildgrid/server/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.582998 buildgrid-0.0.95/buildgrid/server/actioncache/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.584998 buildgrid-0.0.95/buildgrid/server/actioncache/caches/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5564 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/action_cache_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)     5593 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4197 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/mirrored_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     6534 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/redis_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     6573 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/remote_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    11662 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/s3_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/with_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3341 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/caches/write_once_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3623 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     4045 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/actioncache/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.585998 buildgrid-0.0.95/buildgrid/server/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2363 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/auth/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1905 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/auth/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/auth/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    15244 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/auth/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.586998 buildgrid-0.0.95/buildgrid/server/bots/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/bots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11156 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/bots/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     7343 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/bots/job_assigner.py
+-rw-rw-rw-   0 root         (0) root         (0)     5647 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/bots/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.587998 buildgrid-0.0.95/buildgrid/server/build_events/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/build_events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6045 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/build_events/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     7213 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/build_events/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.588997 buildgrid-0.0.95/buildgrid/server/capabilities/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/capabilities/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7113 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/capabilities/instance.py
+-rwxrwxrwx   0 root         (0) root         (0)     3342 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/capabilities/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.588997 buildgrid-0.0.95/buildgrid/server/cas/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21766 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)    12330 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.591997 buildgrid-0.0.95/buildgrid/server/cas/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3702 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.592998 buildgrid-0.0.95/buildgrid/server/cas/storage/index/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/index/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3335 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/index/index_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)    13464 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/index/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)    38579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.593998 buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql_dialect_delegates/
+-rw-rw-rw-   0 root         (0) root         (0)      146 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql_dialect_delegates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2136 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2120 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py
+-rw-rw-rw-   0 root         (0) root         (0)     4436 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/lru_memory_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/redis.py
+-rw-rw-rw-   0 root         (0) root         (0)     8601 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/remote.py
+-rw-rw-rw-   0 root         (0) root         (0)    11295 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/replicated.py
+-rw-rw-rw-   0 root         (0) root         (0)    14426 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     6002 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/sharded.py
+-rw-rw-rw-   0 root         (0) root         (0)     6985 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/size_differentiated.py
+-rw-rw-rw-   0 root         (0) root         (0)     9519 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/sql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8154 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/storage_abc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7796 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/cas/storage/with_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     3029 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     2194 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.594998 buildgrid-0.0.95/buildgrid/server/execution/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/execution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9599 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/execution/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     7517 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/execution/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     3813 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/job_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    18608 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/metrics_names.py
+-rw-rw-rw-   0 root         (0) root         (0)    14482 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/metrics_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    19548 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/monitoring.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.594998 buildgrid-0.0.95/buildgrid/server/operations/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.596998 buildgrid-0.0.95/buildgrid/server/operations/filtering/
+-rw-rw-rw-   0 root         (0) root         (0)      813 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/filtering/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/filtering/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/filtering/filter_grammar.lark
+-rw-rw-rw-   0 root         (0) root         (0)     5769 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/filtering/interpreter.py
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/filtering/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4594 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/filtering/sanitizer.py
+-rw-rw-rw-   0 root         (0) root         (0)     4802 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     6034 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/operations/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.596998 buildgrid-0.0.95/buildgrid/server/persistence/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.597998 buildgrid-0.0.95/buildgrid/server/persistence/sql/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.598997 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/README
+-rw-rw-rw-   0 root         (0) root         (0)     2919 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/env.py
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.602998 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1718 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2422 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py
+-rw-rw-rw-   0 root         (0) root         (0)     1155 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py
+-rw-rw-rw-   0 root         (0) root         (0)     1949 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py
+-rw-rw-rw-   0 root         (0) root         (0)     1191 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py
+-rw-rw-rw-   0 root         (0) root         (0)     4625 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py
+-rw-rw-rw-   0 root         (0) root         (0)     2072 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py
+-rw-rw-rw-   0 root         (0) root         (0)    79716 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     8915 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     6206 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/notifier.py
+-rw-rw-rw-   0 root         (0) root         (0)    10298 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/persistence/sql/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.603998 buildgrid-0.0.95/buildgrid/server/redis/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/redis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6197 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/redis/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     4739 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/request_metadata_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.603998 buildgrid-0.0.95/buildgrid/server/s3/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/s3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18695 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/s3/s3utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    30687 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/server.py
+-rw-rw-rw-   0 root         (0) root         (0)     6126 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/servicer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.604997 buildgrid-0.0.95/buildgrid/server/sql/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/sql/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    22200 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/sql/provider.py
+-rw-rw-rw-   0 root         (0) root         (0)     6225 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/sql/sqlutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/threading.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.605998 buildgrid-0.0.95/buildgrid/server/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4484 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/utils/async_lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/utils/context.py
+-rw-rw-rw-   0 root         (0) root         (0)    10885 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/server/utils/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5450 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)    12244 2024-05-16 13:09:52.000000 buildgrid-0.0.95/buildgrid/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.617998 buildgrid-0.0.95/buildgrid.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7030 2024-05-16 13:10:20.000000 buildgrid-0.0.95/buildgrid.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    21169 2024-05-16 13:10:20.000000 buildgrid-0.0.95/buildgrid.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 13:10:20.000000 buildgrid-0.0.95/buildgrid.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-16 13:10:20.000000 buildgrid-0.0.95/buildgrid.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1233 2024-05-16 13:10:20.000000 buildgrid-0.0.95/buildgrid.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-16 13:10:20.000000 buildgrid-0.0.95/buildgrid.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.516998 buildgrid-0.0.95/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.609998 buildgrid-0.0.95/data/config/
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/all-in-one.yml
+-rw-rw-rw-   0 root         (0) root         (0)      588 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/artifacts.yml
+-rwxrwxrwx   0 root         (0) root         (0)     1351 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/basic-with-disk.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/bots-interface.yml
+-rw-rw-rw-   0 root         (0) root         (0)      896 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/cache.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/controller.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/default.yml
+-rw-rw-rw-   0 root         (0) root         (0)      832 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/index-sqlite-no-execution.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1571 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/index-sqlite.yml
+-rw-rw-rw-   0 root         (0) root         (0)      247 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/logstream.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/monitoring-controller.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1143 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/multi-layer-storage.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1474 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/redis-cache.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/s3-indexed-cas.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/storage-redis.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/storage-s3.yml
+-rw-rw-rw-   0 root         (0) root         (0)      900 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/storage.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/with-metering.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1478 2024-05-16 13:09:52.000000 buildgrid-0.0.95/data/config/with-pgbouncer.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.609998 buildgrid-0.0.95/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      610 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.609998 buildgrid-0.0.95/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.611997 buildgrid-0.0.95/docs/source/data/
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/data/basic-disk-cas.yml
+-rw-rw-rw-   0 root         (0) root         (0)      492 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/data/bazel-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      490 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/data/buildstream-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      446 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/data/cas-and-ac.yml
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/data/cas-example-server.yml
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/data/execution-and-bots.yml
+-rw-rw-rw-   0 root         (0) root         (0)      531 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/data/sqlite-index-cas-only.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1425 2024-05-16 13:09:52.000000 buildgrid-0.0.95/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5463 2024-05-16 13:09:52.000000 buildgrid-0.0.95/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      855 2024-05-16 13:10:20.625998 buildgrid-0.0.95/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      643 2024-05-16 13:09:52.000000 buildgrid-0.0.95/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.613998 buildgrid-0.0.95/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.517998 buildgrid-0.0.95/tests/auth/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 13:10:20.616998 buildgrid-0.0.95/tests/auth/data/
+-rw-rw-rw-   0 root         (0) root         (0)      733 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/auth.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwks-valid.json
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-hs256-conflicting.secret
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-hs256-expired.token
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-hs256-matching.secret
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-hs256-unbounded.token
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-hs256-valid.token
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-rs256-conflicting.pub.key
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-rs256-expired.token
+-rw-rw-rw-   0 root         (0) root         (0)      559 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-rs256-jwk-encrypted.token
+-rw-rw-rw-   0 root         (0) root         (0)      886 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-rs256-matching.priv.key
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-rs256-matching.pub.key
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-rs256-unbounded.token
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/auth/data/jwt-rs256-valid.token
+-rw-rw-rw-   0 root         (0) root         (0)     3829 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_async_lru_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)    15407 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_execution_instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     2199 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_job_assigner.py
+-rw-rw-rw-   0 root         (0) root         (0)    12358 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_metrics_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3447 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_mirrored_cache.py
+-rw-rw-rw-   0 root         (0) root         (0)     2098 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_multithreaded_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1368 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2777 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_request_metadata_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    32384 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_scheduler.py
+-rw-rw-rw-   0 root         (0) root         (0)    10567 2024-05-16 13:09:52.000000 buildgrid-0.0.95/tests/test_utils.py
```

### Comparing `buildgrid-0.0.94/BuildGrid.doap` & `buildgrid-0.0.95/BuildGrid.doap`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/CONTRIBUTING.rst` & `buildgrid-0.0.95/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/LICENSE` & `buildgrid-0.0.95/LICENSE`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/PKG-INFO` & `buildgrid-0.0.95/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: buildgrid
-Version: 0.0.94
+Version: 0.0.95
 Summary: A remote execution service
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://buildgrid.build
 Project-URL: Documentation, https://buildgrid.build
 Project-URL: Repository, https://gitlab.com/BuildGrid/buildgrid
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: botocore
 Requires-Dist: dnspython
 Requires-Dist: grpcio-reflection>=1.62.0
 Requires-Dist: grpcio>=1.62.0
+Requires-Dist: importlib-resources
 Requires-Dist: janus>=0.6.2
 Requires-Dist: jinja2
 Requires-Dist: protobuf
 Requires-Dist: alembic
 Requires-Dist: Click
 Requires-Dist: SQLAlchemy[mypy]<2.0,>=1.4.24
 Requires-Dist: pydantic>2.0
@@ -137,16 +138,16 @@
 the scheduling and storage. The `BuildBox`_ ecosystem provides a suite of workers and
 sandboxing tools that work with the Workers API and can be used with BuildGrid.
 
 .. _Remote Execution API: https://github.com/bazelbuild/remote-apis
 .. _Remote Workers API: https://docs.google.com/document/d/1s_AzRRD2mdyktKUj2HWBn99rMg_3tcPvdjx3MPbFidU/edit#heading=h.1u2taqr2h940
 .. _BuildStream: https://wiki.gnome.org/Projects/BuildStream
 .. _Bazel: https://bazel.build
-.. _RECC: https://gitlab.com/BuildGrid/recc
-.. _Trexe: https://gitlab.com/BuildGrid/trexe
+.. _RECC: https://gitlab.com/BuildGrid/buildbox/buildbox/-/tree/master/recc
+.. _Trexe: https://gitlab.com/BuildGrid/buildbox/buildbox/-/tree/master/trexe
 .. _BuildBox: https://buildgrid.gitlab.io/buildbox/buildbox-home/
 
 
 .. _readme-getting-started:
 
 Getting started
 ---------------
```

### Comparing `buildgrid-0.0.94/README.rst` & `buildgrid-0.0.95/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 the scheduling and storage. The `BuildBox`_ ecosystem provides a suite of workers and
 sandboxing tools that work with the Workers API and can be used with BuildGrid.
 
 .. _Remote Execution API: https://github.com/bazelbuild/remote-apis
 .. _Remote Workers API: https://docs.google.com/document/d/1s_AzRRD2mdyktKUj2HWBn99rMg_3tcPvdjx3MPbFidU/edit#heading=h.1u2taqr2h940
 .. _BuildStream: https://wiki.gnome.org/Projects/BuildStream
 .. _Bazel: https://bazel.build
-.. _RECC: https://gitlab.com/BuildGrid/recc
-.. _Trexe: https://gitlab.com/BuildGrid/trexe
+.. _RECC: https://gitlab.com/BuildGrid/buildbox/buildbox/-/tree/master/recc
+.. _Trexe: https://gitlab.com/BuildGrid/buildbox/buildbox/-/tree/master/trexe
 .. _BuildBox: https://buildgrid.gitlab.io/buildbox/buildbox-home/
 
 
 .. _readme-getting-started:
 
 Getting started
 ---------------
```

### Comparing `buildgrid-0.0.94/buildgrid/__init__.py` & `buildgrid-0.0.95/buildgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/__init__.py` & `buildgrid-0.0.95/buildgrid/_app/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/cli.py` & `buildgrid-0.0.95/buildgrid/_app/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 import logging
 import os
 import sys
 from typing import Any, Dict, Optional
 
 import click
 import grpc
+from importlib_resources import files
 
 from buildgrid.server.context import ctx_grpc_request_id
 from buildgrid.settings import LOG_RECORD_FORMAT
 
 CONTEXT_SETTINGS = {
     "auto_envvar_prefix": "BUILDGRID",
     "max_content_width": 1000,  # do not truncate option help unnecessarily
@@ -49,15 +50,15 @@
         self.logstream_channel: Optional[grpc.Channel] = None
         self.instance_name: str = ""
 
         self.user_home: str = os.getcwd()
 
 
 pass_context = click.make_pass_decorator(Context, ensure=True)
-cmd_folder = os.path.abspath(os.path.join(os.path.dirname(__file__), "commands"))
+cmd_folder = files("buildgrid._app").joinpath("commands")
 
 commands_namespace = "buildgrid._app.commands"
 
 
 class App(click.MultiCommand):
     def list_commands(self, ctx):
         """Lists available command names."""
```

### Comparing `buildgrid-0.0.94/buildgrid/_app/commands/__init__.py` & `buildgrid-0.0.95/buildgrid/_app/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/commands/cmd_actioncache.py` & `buildgrid-0.0.95/buildgrid/_app/commands/cmd_actioncache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/commands/cmd_browser_backend.py` & `buildgrid-0.0.95/buildgrid/_app/commands/cmd_browser_backend.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/commands/cmd_capabilities.py` & `buildgrid-0.0.95/buildgrid/_app/commands/cmd_capabilities.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/commands/cmd_cas.py` & `buildgrid-0.0.95/buildgrid/_app/commands/cmd_cas.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/commands/cmd_cleanup.py` & `buildgrid-0.0.95/buildgrid/_app/commands/cmd_cleanup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/commands/cmd_execute.py` & `buildgrid-0.0.95/buildgrid/_app/commands/cmd_execute.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/commands/cmd_janitor.py` & `buildgrid-0.0.95/buildgrid/_app/commands/cmd_janitor.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/commands/cmd_logstream.py` & `buildgrid-0.0.95/buildgrid/_app/commands/cmd_logstream.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/commands/cmd_operation.py` & `buildgrid-0.0.95/buildgrid/_app/commands/cmd_operation.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/commands/cmd_server.py` & `buildgrid-0.0.95/buildgrid/_app/commands/cmd_server.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/commands/rpc_utils.py` & `buildgrid-0.0.95/buildgrid/_app/commands/rpc_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/__init__.py` & `buildgrid-0.0.95/buildgrid/_app/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/parser.py` & `buildgrid-0.0.95/buildgrid/_app/settings/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 import buildgrid_metering.client as metering
 import click
 import grpc
 import requests
 import yaml
 from buildgrid_metering.client.exceptions import MeteringServiceClientError, MeteringServiceError
+from importlib_resources import files
 from jsonschema import Draft7Validator, validators
 from jsonschema.exceptions import ValidationError
 
 from buildgrid._enums import ActionCacheEntryType
 from buildgrid.client.asset import AssetClient
 from buildgrid.client.authentication import ClientCredentials
 from buildgrid.server.actioncache.caches.action_cache_abc import ActionCacheABC
@@ -77,17 +78,16 @@
     yaml_tag: Optional[str] = None
     schema: Optional[str] = None
 
     @classmethod
     def _get_schema(cls):
         schema = {}
         if cls.schema is not None:
-            path = os.path.join(os.path.dirname(__file__), "schemas", cls.schema)
-            with open(path, encoding="utf-8") as schema_file:
-                schema = yaml.safe_load(schema_file)
+            schema_text = files("buildgrid._app.settings.schemas").joinpath(cls.schema).read_text()
+            schema = yaml.safe_load(schema_text)
         return schema
 
     @classmethod
     def _validate(cls, values):
         click.echo(click.style(f"\nValidating {cls.yaml_tag}...", fg="yellow"))
         schema = cls._get_schema()
         validator = get_validator(schema=schema)
@@ -2743,17 +2743,16 @@
     yaml.SafeLoader.add_constructor(AssetClientFactory.yaml_tag, AssetClientFactory.from_yaml)
     yaml.SafeLoader.add_constructor(Replicated_Storage.yaml_tag, Replicated_Storage.from_yaml)
 
     return yaml
 
 
 def get_schema():
-    path = os.path.join(os.path.dirname(__file__), "schemas", "config.yaml")
-    with open(path, encoding="utf-8") as schema_file:
-        schema = yaml.safe_load(schema_file)
+    schema_text = files("buildgrid._app.settings.schemas").joinpath("config.yaml").read_text()
+    schema = yaml.safe_load(schema_text)
     return schema
 
 
 def check_type(*expected_types: Any) -> Callable[[Any, Any], bool]:
     def _check_type(checker: Any, instance: Any) -> bool:
         return any(isinstance(instance, t) for t in expected_types)
```

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/reference.yml` & `buildgrid-0.0.95/buildgrid/_app/settings/reference.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml` & `buildgrid-0.0.95/buildgrid/_app/settings/schemas/caches/redis-action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml` & `buildgrid-0.0.95/buildgrid/_app/settings/schemas/clients/metering-service-client.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/schemas/config.yaml` & `buildgrid-0.0.95/buildgrid/_app/settings/schemas/config.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/schemas/connections/sql.yaml` & `buildgrid-0.0.95/buildgrid/_app/settings/schemas/connections/sql.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/schemas/misc/channel.yaml` & `buildgrid-0.0.95/buildgrid/_app/settings/schemas/misc/channel.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/schemas/scheduler/sql.yaml` & `buildgrid-0.0.95/buildgrid/_app/settings/schemas/scheduler/sql.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/action-cache.yaml` & `buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/bots.yaml` & `buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/bots.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/execution.yaml` & `buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/execution.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml` & `buildgrid-0.0.95/buildgrid/_app/settings/schemas/services/remote-action-cache.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/remote.yaml` & `buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/remote.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/s3.yaml` & `buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/s3.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml` & `buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/size-differentiated.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_app/settings/schemas/storage/sql-index.yaml` & `buildgrid-0.0.95/buildgrid/_app/settings/schemas/storage/sql-index.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_enums.py` & `buildgrid-0.0.95/buildgrid/_enums.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_exceptions.py` & `buildgrid-0.0.95/buildgrid/_exceptions.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/build/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/asset/v1/remote_asset_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/execution/v2/remote_execution_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/remote/logstream/v1/remote_logstream_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/build/bazel/semver/semver_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/build/buildbox/execution_stats_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/messaging_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/monitoring_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/buildgrid/v2/query_build_events_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/google/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/api/annotations_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/api/client_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/api/field_behavior_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/api/http_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/bytestream/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/google/bytestream/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py` & `buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py` & `buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/bytestream/bytestream_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_events_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/build_status_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/build/v1/publish_build_event_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/bots_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/command_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/tasks_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/devtools/remoteworkers/v1test2/worker_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/longrunning/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/google/longrunning/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py` & `buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py` & `buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/longrunning/operations_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/rpc/__init__.py` & `buildgrid-0.0.95/buildgrid/_protos/google/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/rpc/code_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/rpc/error_details_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2.py` & `buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi` & `buildgrid-0.0.95/buildgrid/_protos/google/rpc/status_pb2_grpc_aio.pyi`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_types.py` & `buildgrid-0.0.95/buildgrid/_types.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/_version.py` & `buildgrid-0.0.95/buildgrid/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = "0.0.94"
+__version__ = "0.0.95"
```

### Comparing `buildgrid-0.0.94/buildgrid/browser/__init__.py` & `buildgrid-0.0.95/buildgrid/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/browser/app.py` & `buildgrid-0.0.95/buildgrid/browser/app.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/browser/rest_api.py` & `buildgrid-0.0.95/buildgrid/browser/rest_api.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/browser/utils.py` & `buildgrid-0.0.95/buildgrid/browser/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/cleanup/__init__.py` & `buildgrid-0.0.95/buildgrid/cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/cleanup/cleanup.py` & `buildgrid-0.0.95/buildgrid/cleanup/cleanup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/cleanup/janitor/__init__.py` & `buildgrid-0.0.95/buildgrid/cleanup/janitor/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/cleanup/janitor/config.py` & `buildgrid-0.0.95/buildgrid/cleanup/janitor/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 
 class S3Config(BaseModel):
     access_key: str
     bucket_regex: str
     endpoint: str
     path_prefix: str
+    hash_prefix_size: int = Field(default=0)
     secret_key: str
 
 
 class RedisConfig(BaseModel):
     db: Optional[int] = Field(default=None)
     dns_srv_record: Optional[str] = Field(default=None)
     index_prefix: str
```

### Comparing `buildgrid-0.0.94/buildgrid/cleanup/janitor/index.py` & `buildgrid-0.0.95/buildgrid/cleanup/janitor/index.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/cleanup/janitor/s3.py` & `buildgrid-0.0.95/buildgrid/cleanup/janitor/s3.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 import random
 import re
+from itertools import product
 from threading import Event
 from typing import Any, Iterator, List, Set, Tuple
 
 from buildgrid.cleanup.janitor.config import JanitorConfig
 from buildgrid.cleanup.janitor.index import IndexLookup
 from buildgrid.cleanup.janitor.utils import check_bucket_versioning, get_s3_client
 from buildgrid.server.threading import ContextWorker
@@ -30,29 +31,30 @@
 
     def __init__(self, config: JanitorConfig, index: IndexLookup):
         self._bucket_regex = re.compile(config.s3.bucket_regex)
         self._index = index
         self._path_prefix = config.s3.path_prefix
         self._s3 = get_s3_client(config.s3)
         self._sleep_interval = config.sleep_interval
+        self._hash_prefix_size = config.s3.hash_prefix_size
 
         self._stop_requested = Event()
         self._worker = ContextWorker(target=self.run, name="Janitor", on_shutdown_requested=self._stop_requested.set)
 
-    def enumerate_versioned_bucket(self, bucket: str) -> Iterator[Set[Tuple[str, str]]]:
-        pages = self._s3.get_paginator("list_object_versions").paginate(Bucket=bucket, Prefix=self._path_prefix)
+    def enumerate_versioned_bucket(self, bucket: str, prefix: str) -> Iterator[Set[Tuple[str, str]]]:
+        pages = self._s3.get_paginator("list_object_versions").paginate(Bucket=bucket, Prefix=prefix)
         for page in pages:
             if "Versions" not in page:
                 continue
 
             digest_version_pairs = {(item["Key"], item["VersionId"]) for item in page["Versions"]}
             yield digest_version_pairs
 
-    def enumerate_unversioned_bucket(self, bucket: str) -> Iterator[Set[Tuple[str, str]]]:
-        pages = self._s3.get_paginator("list_objects").paginate(Bucket=bucket, Prefix=self._path_prefix)
+    def enumerate_unversioned_bucket(self, bucket: str, prefix: str) -> Iterator[Set[Tuple[str, str]]]:
+        pages = self._s3.get_paginator("list_objects").paginate(Bucket=bucket, Prefix=prefix)
         for page in pages:
             if "Contents" not in page:
                 continue
 
             digest_version_pairs = {(item["Key"], "") for item in page["Contents"]}
             yield digest_version_pairs
 
@@ -69,33 +71,55 @@
 
     def get_buckets(self) -> List[str]:
         response = self._s3.list_buckets()
         return [
             bucket["Name"] for bucket in response["Buckets"] if self._bucket_regex.search(bucket["Name"]) is not None
         ]
 
+    # Generate all the hash prefixes and shuffle them to reduce the likelihood of
+    # two janitors cleaning the same hash prefix
+    def generate_prefixes(self) -> List[str]:
+        if self._hash_prefix_size:
+            prefixes = [
+                (self._path_prefix + "/" if self._path_prefix else "") + "".join(x)
+                for x in product("0123456789abcdef", repeat=self._hash_prefix_size)
+            ]
+            random.shuffle(prefixes)
+        else:
+            prefixes = [self._path_prefix]
+        return prefixes
+
     def cleanup_bucket(self, bucket: str) -> int:
         LOGGER.info(f"Cleaning up bucket: '{bucket}'")
 
         deleted_count = 0
-        enumeration = self.enumerate_unversioned_bucket
         if check_bucket_versioning(self._s3, bucket):
             enumeration = self.enumerate_versioned_bucket
+        else:
+            enumeration = self.enumerate_unversioned_bucket
 
-        for page in enumeration(bucket):
-            missing_digest_versions = set(
-                digest_version
-                for digest_version in page
-                if digest_version[0] in self._index.get_missing_digests(set(digest for digest, _ in page))
-            )
-            if missing_digest_versions:
-                self.delete_s3_entries(bucket, missing_digest_versions)
-                deleted_count += len(missing_digest_versions)
+        for prefix in self.generate_prefixes():
+            deleted_count_for_prefix = 0
+            for page in enumeration(bucket, prefix):
+                # Create a mapping between a digest as stored in S3 and a digest as stored in the index
+                # by stripping off any prefix and removing all '/' used by hash_prefix_size
+                digest_map = {digest: digest.replace(self._path_prefix, "").replace("/", "") for digest, _ in page}
+
+                missing_digest_versions = set(
+                    digest_version
+                    for digest_version in page
+                    if digest_map[digest_version[0]] in self._index.get_missing_digests(set(digest_map.values()))
+                )
+                if missing_digest_versions:
+                    self.delete_s3_entries(bucket, missing_digest_versions)
+                    deleted_count_for_prefix += len(missing_digest_versions)
+            LOGGER.info(f"Deleted {deleted_count_for_prefix} blobs from '{bucket}/{prefix}'")
+            deleted_count += deleted_count_for_prefix
 
-        LOGGER.info(f"Deleted {deleted_count} blobs from bucket '{bucket}'")
+        LOGGER.info(f"Deleted {deleted_count} blobs total from bucket '{bucket}'")
         return deleted_count
 
     def start(self) -> None:
         self._worker.start()
         self._worker.wait()
 
     def stop(self, *args: Any, **kwargs: Any) -> None:
```

### Comparing `buildgrid-0.0.94/buildgrid/cleanup/janitor/utils.py` & `buildgrid-0.0.95/buildgrid/cleanup/janitor/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/client/__init__.py` & `buildgrid-0.0.95/buildgrid/client/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/client/actioncache.py` & `buildgrid-0.0.95/buildgrid/client/actioncache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/client/asset.py` & `buildgrid-0.0.95/buildgrid/client/asset.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/client/auth_token_loader.py` & `buildgrid-0.0.95/buildgrid/client/auth_token_loader.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/client/authentication.py` & `buildgrid-0.0.95/buildgrid/client/authentication.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/client/capabilities.py` & `buildgrid-0.0.95/buildgrid/client/capabilities.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/client/cas.py` & `buildgrid-0.0.95/buildgrid/client/cas.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/client/channel.py` & `buildgrid-0.0.95/buildgrid/client/channel.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/client/interceptors.py` & `buildgrid-0.0.95/buildgrid/client/interceptors.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/client/logstream.py` & `buildgrid-0.0.95/buildgrid/client/logstream.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/client/retrier.py` & `buildgrid-0.0.95/buildgrid/client/retrier.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/__init__.py` & `buildgrid-0.0.95/buildgrid/server/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/actioncache/__init__.py` & `buildgrid-0.0.95/buildgrid/server/actioncache/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/actioncache/caches/__init__.py` & `buildgrid-0.0.95/buildgrid/server/actioncache/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/actioncache/caches/action_cache_abc.py` & `buildgrid-0.0.95/buildgrid/server/actioncache/caches/action_cache_abc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/actioncache/caches/lru_cache.py` & `buildgrid-0.0.95/buildgrid/server/actioncache/caches/lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/actioncache/caches/mirrored_cache.py` & `buildgrid-0.0.95/buildgrid/server/actioncache/caches/mirrored_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/actioncache/caches/redis_cache.py` & `buildgrid-0.0.95/buildgrid/server/actioncache/caches/redis_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/actioncache/caches/remote_cache.py` & `buildgrid-0.0.95/buildgrid/server/actioncache/caches/remote_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/actioncache/caches/s3_cache.py` & `buildgrid-0.0.95/buildgrid/server/actioncache/caches/s3_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/actioncache/caches/with_cache.py` & `buildgrid-0.0.95/buildgrid/server/actioncache/caches/with_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/actioncache/caches/write_once_cache.py` & `buildgrid-0.0.95/buildgrid/server/actioncache/caches/write_once_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/actioncache/instance.py` & `buildgrid-0.0.95/buildgrid/server/actioncache/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/actioncache/service.py` & `buildgrid-0.0.95/buildgrid/server/actioncache/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/auth/__init__.py` & `buildgrid-0.0.95/buildgrid/server/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/auth/config.py` & `buildgrid-0.0.95/buildgrid/server/auth/config.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/auth/enums.py` & `buildgrid-0.0.95/buildgrid/server/auth/enums.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/auth/exceptions.py` & `buildgrid-0.0.95/buildgrid/server/auth/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/auth/manager.py` & `buildgrid-0.0.95/buildgrid/server/auth/manager.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/bots/__init__.py` & `buildgrid-0.0.95/buildgrid/server/bots/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/bots/instance.py` & `buildgrid-0.0.95/buildgrid/server/bots/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/bots/job_assigner.py` & `buildgrid-0.0.95/buildgrid/server/bots/job_assigner.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/bots/service.py` & `buildgrid-0.0.95/buildgrid/server/bots/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/build_events/__init__.py` & `buildgrid-0.0.95/buildgrid/server/build_events/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/build_events/service.py` & `buildgrid-0.0.95/buildgrid/server/build_events/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/build_events/storage.py` & `buildgrid-0.0.95/buildgrid/server/build_events/storage.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/capabilities/__init__.py` & `buildgrid-0.0.95/buildgrid/server/capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/capabilities/instance.py` & `buildgrid-0.0.95/buildgrid/server/capabilities/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/capabilities/service.py` & `buildgrid-0.0.95/buildgrid/server/capabilities/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/__init__.py` & `buildgrid-0.0.95/buildgrid/server/cas/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/instance.py` & `buildgrid-0.0.95/buildgrid/server/cas/instance.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,14 +264,15 @@
 
                     with Distribution(
                         CAS_BATCH_READ_BLOBS_SIZE_BYTES, instance_name=self._instance_name
                     ) as metric_blob_size:
                         metric_blob_size.count = float(digest.size_bytes)
                 else:
                     status_code = code_pb2.NOT_FOUND
+                    LOGGER.info(f"Blob not found: {digest.hash}/{digest.size_bytes}, from BatchReadBlobs")
 
                 response_proto.status.CopyFrom(status_pb2.Status(code=status_code))
 
         for digest in bad_digests:
             response_proto = response.responses.add()
             response_proto.digest.CopyFrom(digest)
             status_code = code_pb2.INVALID_ARGUMENT
@@ -411,15 +412,15 @@
 
         else:
             raise InvalidArgumentError("Negative read_limit is invalid")
 
         # Read the blob from storage and send its contents to the client.
         result = self._storage.get_blob(digest)
         if result is None:
-            raise NotFoundError("Blob not found")
+            raise NotFoundError(f"Blob not found: {digest.hash}/{digest.size_bytes}, from Bytestream.Read")
 
         try:
             if read_offset > 0:
                 result.seek(read_offset)
 
             with Distribution(
                 metric_name=CAS_BYTESTREAM_READ_SIZE_BYTES, instance_name=self._instance_name
```

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/service.py` & `buildgrid-0.0.95/buildgrid/server/cas/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/__init__.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/disk.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/disk.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/index/__init__.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/index/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/index/index_abc.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/index/index_abc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/index/redis.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/index/redis.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,17 @@
                     return io.BytesIO(entry.inline_blob)
                 elif blob := self._storage.get_blob(digest):
                     # Fix any blobs that should have been inlined.
                     if digest.size_bytes <= self._max_inline_blob_size:
                         self._save_digests_to_index([(digest, read_and_rewind(blob))], session)
                         session.commit()
                     return blob
-                LOGGER.warning(f"Blob [{digest.hash}] was indexed but not in storage. Deleting from the index")
+                LOGGER.warning(
+                    f"Blob [{digest.hash}/{digest.size_bytes}] was indexed but not in storage. Deleting from the index"
+                )
                 self._bulk_delete_from_index([digest], session)
 
         # Check the storage for the blob and repair the index if found.
         if self._fallback_on_get:
             if blob := self._storage.get_blob(digest):
                 with self._sql.scoped_session() as session:
                     if digest.size_bytes <= self._max_inline_blob_size:
@@ -536,15 +538,18 @@
                     digest_pairs_to_save.append((digest, blob_data))
 
         acutal_storage_digests = set(digest_hash for (digest_hash, _) in fetched_digests.items())
         # Get a list of all the digests that were in the index but not found in storage
         digests_expected_not_in_storage: List[Digest] = []
         for expected_digest in digests_to_fetch:
             if expected_digest.hash not in acutal_storage_digests:
-                LOGGER.warning(f"Blob [{expected_digest}] was indexed but not in storage. Deleting from the index")
+                LOGGER.warning(
+                    f"Blob [{expected_digest.hash}/{expected_digest.size_bytes}] "
+                    "was indexed but not in storage. Deleting from the index"
+                )
                 digests_expected_not_in_storage.append(expected_digest)
 
         # Update any blobs which need to be inlined
         with self._sql.scoped_session() as session:
             self._save_digests_to_index(digest_pairs_to_save, session)
             if digests_expected_not_in_storage:
                 self._bulk_delete_from_index(digests_expected_not_in_storage, session)
```

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql_dialect_delegates/postgresqldelegate.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/index/sql_dialect_delegates/sqlitedelegate.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/lru_memory_cache.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/lru_memory_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/redis.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/redis.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/remote.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/remote.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/replicated.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/replicated.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/s3.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/s3.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/sharded.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/sharded.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/size_differentiated.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/size_differentiated.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/sql.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/sql.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/storage_abc.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/storage_abc.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/cas/storage/with_cache.py` & `buildgrid-0.0.95/buildgrid/server/cas/storage/with_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/context.py` & `buildgrid-0.0.95/buildgrid/server/context.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/controller.py` & `buildgrid-0.0.95/buildgrid/server/controller.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/execution/__init__.py` & `buildgrid-0.0.95/buildgrid/server/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/execution/instance.py` & `buildgrid-0.0.95/buildgrid/server/execution/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/execution/service.py` & `buildgrid-0.0.95/buildgrid/server/execution/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/job_metrics.py` & `buildgrid-0.0.95/buildgrid/server/job_metrics.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/metrics_names.py` & `buildgrid-0.0.95/buildgrid/server/metrics_names.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/metrics_utils.py` & `buildgrid-0.0.95/buildgrid/server/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/monitoring.py` & `buildgrid-0.0.95/buildgrid/server/monitoring.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/operations/__init__.py` & `buildgrid-0.0.95/buildgrid/server/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/operations/filtering/__init__.py` & `buildgrid-0.0.95/buildgrid/server/operations/filtering/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/operations/filtering/filter.py` & `buildgrid-0.0.95/buildgrid/server/operations/filtering/filter.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/operations/filtering/filter_grammar.lark` & `buildgrid-0.0.95/buildgrid/server/operations/filtering/filter_grammar.lark`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/operations/filtering/interpreter.py` & `buildgrid-0.0.95/buildgrid/server/operations/filtering/interpreter.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/operations/filtering/parser.py` & `buildgrid-0.0.95/buildgrid/server/operations/filtering/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 
 
 class FilterParser:
     """
     Utility class primarily used to parse a filter string and return a list a OperationFilters.
     """
 
-    lark_parser = Lark.open("filter_grammar.lark", rel_to=__file__, start="filter_phrase")
+    lark_parser = Lark.open_from_package(
+        "buildgrid.server.operations.filtering", "filter_grammar.lark", start="filter_phrase"
+    )
 
     @staticmethod
     def parse_listoperations_filters(filter_string: str) -> List[OperationFilter]:
         """Separate the lowercase filter string into individual components, and return a map containing
         the relevant filters to use.
 
         Filter strings take the following form: key1=value1&key2=value2,value3&key3=value4
```

### Comparing `buildgrid-0.0.94/buildgrid/server/operations/filtering/sanitizer.py` & `buildgrid-0.0.95/buildgrid/server/operations/filtering/sanitizer.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/operations/instance.py` & `buildgrid-0.0.95/buildgrid/server/operations/instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/operations/service.py` & `buildgrid-0.0.95/buildgrid/server/operations/service.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/__init__.py` & `buildgrid-0.0.95/buildgrid/server/persistence/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/__init__.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/env.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/env.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/script.py.mako` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/083f52d97bcb_add_index_on_queued_timestamp.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/1553978c6e69_add_stream_resource_names_to_jobs.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/29e88b3e0d0a_store_tool_information_for_a_job_in_the_.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/2b49634f4459_add_job_action_column.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/316ad77858af_add_blobs_table_for_sqlstorage.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/38340cc0cfb7_partial_indices.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/53e8b8b5bed6_add_inline_blob_support.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/69ceb5938c06_add_a_deleted_flag_for_indexed_cas_.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/8d910c8de8b6_use_largebinary_to_store_action_message.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/9b595964dc25_add_job_command.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/afa46425330d_add_platform_properties_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/b57c30a687fa_add_client_identities_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/bbb77b202e31_add_job_status_code.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/bc324dfd3610_add_cascades_for_job_platforms_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/c64c104b2c8b_digest_size_bytes_to_bigint.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/d4efbcc698ca_add_instance_name_to_jobs.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/e1448dca2c7a_add_expiry_time_to_bots.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/e287a533bbd7_new_database.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/alembic/versions/fcb6e8f09a1d_add_bots_table.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/impl.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/impl.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/models.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/models.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/notifier.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/notifier.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/persistence/sql/utils.py` & `buildgrid-0.0.95/buildgrid/server/persistence/sql/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/redis/__init__.py` & `buildgrid-0.0.95/buildgrid/server/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/redis/provider.py` & `buildgrid-0.0.95/buildgrid/server/redis/provider.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/request_metadata_utils.py` & `buildgrid-0.0.95/buildgrid/server/request_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/s3/__init__.py` & `buildgrid-0.0.95/buildgrid/server/s3/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/s3/s3utils.py` & `buildgrid-0.0.95/buildgrid/server/s3/s3utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/server.py` & `buildgrid-0.0.95/buildgrid/server/server.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/servicer.py` & `buildgrid-0.0.95/buildgrid/server/servicer.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/sql/__init__.py` & `buildgrid-0.0.95/buildgrid/server/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/sql/provider.py` & `buildgrid-0.0.95/buildgrid/server/sql/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
-import os
 from contextlib import contextmanager
 from datetime import timedelta
 from tempfile import NamedTemporaryFile
 from typing import Any, Dict, Generator, Iterator, List, Optional, Type, Union, cast
 
 from alembic import command
 from alembic.config import Config
+from importlib_resources import files
 from sqlalchemy import create_engine, event, text
 from sqlalchemy.engine import Engine
 from sqlalchemy.orm import Session, scoped_session, sessionmaker
 from sqlalchemy.pool import NullPool
 
 from buildgrid._exceptions import DatabaseError, RetriableDatabaseError
 from buildgrid.server.sql import sqlutils
@@ -318,17 +318,15 @@
             risk of migrations conflicting with themselves and causing at least
             one of the callers to fail.
 
         """
         LOGGER.warning("Will attempt migration to latest version if needed.")
 
         config: Config = Config()
-        config.set_main_option(
-            "script_location", os.path.join(os.path.dirname(__file__), "..", "persistence", "sql", "alembic")
-        )
+        config.set_main_option("script_location", str(files("buildgrid.server.persistence.sql").joinpath("alembic")))
 
         with self._engine.begin() as connection:
             # NOTE: pylint doesn't like this for some reason, but it is the
             # documented way to set the connection.
             # https://alembic.sqlalchemy.org/en/latest/api/config.html#alembic.config.Config
             config.attributes["connection"] = connection
             command.upgrade(config, "head")
```

### Comparing `buildgrid-0.0.94/buildgrid/server/sql/sqlutils.py` & `buildgrid-0.0.95/buildgrid/server/sql/sqlutils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/threading.py` & `buildgrid-0.0.95/buildgrid/server/threading.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/utils/__init__.py` & `buildgrid-0.0.95/buildgrid/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/utils/async_lru_cache.py` & `buildgrid-0.0.95/buildgrid/server/utils/async_lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/utils/context.py` & `buildgrid-0.0.95/buildgrid/server/utils/context.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/server/utils/decorators.py` & `buildgrid-0.0.95/buildgrid/server/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/settings.py` & `buildgrid-0.0.95/buildgrid/settings.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid/utils.py` & `buildgrid-0.0.95/buildgrid/utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid.egg-info/PKG-INFO` & `buildgrid-0.0.95/buildgrid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: buildgrid
-Version: 0.0.94
+Version: 0.0.95
 Summary: A remote execution service
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://buildgrid.build
 Project-URL: Documentation, https://buildgrid.build
 Project-URL: Repository, https://gitlab.com/BuildGrid/buildgrid
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: boto3
 Requires-Dist: botocore
 Requires-Dist: dnspython
 Requires-Dist: grpcio-reflection>=1.62.0
 Requires-Dist: grpcio>=1.62.0
+Requires-Dist: importlib-resources
 Requires-Dist: janus>=0.6.2
 Requires-Dist: jinja2
 Requires-Dist: protobuf
 Requires-Dist: alembic
 Requires-Dist: Click
 Requires-Dist: SQLAlchemy[mypy]<2.0,>=1.4.24
 Requires-Dist: pydantic>2.0
@@ -137,16 +138,16 @@
 the scheduling and storage. The `BuildBox`_ ecosystem provides a suite of workers and
 sandboxing tools that work with the Workers API and can be used with BuildGrid.
 
 .. _Remote Execution API: https://github.com/bazelbuild/remote-apis
 .. _Remote Workers API: https://docs.google.com/document/d/1s_AzRRD2mdyktKUj2HWBn99rMg_3tcPvdjx3MPbFidU/edit#heading=h.1u2taqr2h940
 .. _BuildStream: https://wiki.gnome.org/Projects/BuildStream
 .. _Bazel: https://bazel.build
-.. _RECC: https://gitlab.com/BuildGrid/recc
-.. _Trexe: https://gitlab.com/BuildGrid/trexe
+.. _RECC: https://gitlab.com/BuildGrid/buildbox/buildbox/-/tree/master/recc
+.. _Trexe: https://gitlab.com/BuildGrid/buildbox/buildbox/-/tree/master/trexe
 .. _BuildBox: https://buildgrid.gitlab.io/buildbox/buildbox-home/
 
 
 .. _readme-getting-started:
 
 Getting started
 ---------------
```

### Comparing `buildgrid-0.0.94/buildgrid.egg-info/SOURCES.txt` & `buildgrid-0.0.95/buildgrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/buildgrid.egg-info/requires.txt` & `buildgrid-0.0.95/buildgrid.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 boto3
 botocore
 dnspython
 grpcio-reflection>=1.62.0
 grpcio>=1.62.0
+importlib-resources
 janus>=0.6.2
 jinja2
 protobuf
 alembic
 Click
 SQLAlchemy[mypy]<2.0,>=1.4.24
 pydantic>2.0
```

### Comparing `buildgrid-0.0.94/data/config/all-in-one.yml` & `buildgrid-0.0.95/data/config/all-in-one.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/artifacts.yml` & `buildgrid-0.0.95/data/config/artifacts.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/basic-with-disk.yml` & `buildgrid-0.0.95/data/config/basic-with-disk.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/bots-interface.yml` & `buildgrid-0.0.95/data/config/bots-interface.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/cache.yml` & `buildgrid-0.0.95/data/config/cache.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/controller.yml` & `buildgrid-0.0.95/data/config/controller.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/default.yml` & `buildgrid-0.0.95/data/config/default.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/index-sqlite-no-execution.yml` & `buildgrid-0.0.95/data/config/index-sqlite-no-execution.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/index-sqlite.yml` & `buildgrid-0.0.95/data/config/index-sqlite.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/monitoring-controller.yml` & `buildgrid-0.0.95/data/config/monitoring-controller.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/multi-layer-storage.yml` & `buildgrid-0.0.95/data/config/multi-layer-storage.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/redis-cache.yml` & `buildgrid-0.0.95/data/config/redis-cache.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/s3-indexed-cas.yml` & `buildgrid-0.0.95/data/config/s3-indexed-cas.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/storage-redis.yml` & `buildgrid-0.0.95/data/config/storage-redis.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/storage-s3.yml` & `buildgrid-0.0.95/data/config/storage-s3.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/storage.yml` & `buildgrid-0.0.95/data/config/storage.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/with-metering.yml` & `buildgrid-0.0.95/data/config/with-metering.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/data/config/with-pgbouncer.yml` & `buildgrid-0.0.95/data/config/with-pgbouncer.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/docs/Makefile` & `buildgrid-0.0.95/docs/Makefile`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/docs/source/data/execution-and-bots.yml` & `buildgrid-0.0.95/docs/source/data/execution-and-bots.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/docs/source/data/sqlite-index-cas-only.yml` & `buildgrid-0.0.95/docs/source/data/sqlite-index-cas-only.yml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/docs/source/index.rst` & `buildgrid-0.0.95/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/pyproject.toml` & `buildgrid-0.0.95/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,28 +17,29 @@
     "setuptools >= 44",
     "wheel >= 0.35",
 ]
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "buildgrid"
-version = "0.0.94"
+version = "0.0.95"
 requires-python = ">=3.8"
 description = "A remote execution service"
 readme = "README.rst"
 license = {text = "Apache License, Version 2.0"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "boto3",
     "botocore",
     "dnspython",
     "grpcio-reflection >= 1.62.0",
     "grpcio >= 1.62.0",
+    "importlib-resources",
     "janus >= 0.6.2",
     "jinja2",
     "protobuf",
     "alembic",
     "Click",
     "SQLAlchemy[mypy] >= 1.4.24, < 2.0", # For _ConnectionFairy.dbapi_connection
     "pydantic > 2.0", # required by new models in metering-client
```

### Comparing `buildgrid-0.0.94/setup.cfg` & `buildgrid-0.0.95/setup.cfg`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/setup.py` & `buildgrid-0.0.95/setup.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/tests/auth/data/auth.yaml` & `buildgrid-0.0.95/tests/auth/data/auth.yaml`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/tests/auth/data/jwt-rs256-jwk-encrypted.token` & `buildgrid-0.0.95/tests/auth/data/jwt-rs256-jwk-encrypted.token`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/tests/auth/data/jwt-rs256-matching.priv.key` & `buildgrid-0.0.95/tests/auth/data/jwt-rs256-matching.priv.key`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/tests/test_async_lru_cache.py` & `buildgrid-0.0.95/tests/test_async_lru_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/tests/test_execution_instance.py` & `buildgrid-0.0.95/tests/test_execution_instance.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/tests/test_job_assigner.py` & `buildgrid-0.0.95/tests/test_job_assigner.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/tests/test_metrics_utils.py` & `buildgrid-0.0.95/tests/test_metrics_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/tests/test_mirrored_cache.py` & `buildgrid-0.0.95/tests/test_mirrored_cache.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/tests/test_multithreaded_metrics.py` & `buildgrid-0.0.95/tests/test_multithreaded_metrics.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/tests/test_parser.py` & `buildgrid-0.0.95/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/tests/test_request_metadata_utils.py` & `buildgrid-0.0.95/tests/test_request_metadata_utils.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/tests/test_scheduler.py` & `buildgrid-0.0.95/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `buildgrid-0.0.94/tests/test_utils.py` & `buildgrid-0.0.95/tests/test_utils.py`

 * *Files identical despite different names*

