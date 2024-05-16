# Comparing `tmp/nucliadb_node_binding-3.1.0.post1299.tar.gz` & `tmp/nucliadb_node_binding-3.1.0.post1302.tar.gz`

## Comparing `nucliadb_node_binding-3.1.0.post1299.tar` & `nucliadb_node_binding-3.1.0.post1302.tar`

### file list

```diff
@@ -1,286 +1,286 @@
--rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/Cargo.toml
--rw-r--r--   0     1001      127     3409 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/src/lib.rs
--rw-r--r--   0     1001      127     2885 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/src/measure.rs
--rw-r--r--   0     1001      127     1081 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
--rw-r--r--   0     1001      127      222 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
--rw-r--r--   0     1001      127     1038 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
--rw-r--r--   0     1001      127      327 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
--rw-r--r--   0     1001      127     1086 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
--rw-r--r--   0     1001      127      249 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
--rw-r--r--   0     1001      127     1046 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
--rw-r--r--   0     1001      127     1303 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
--rw-r--r--   0     1001      127     1408 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/tests/test_measure.rs
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/Cargo.toml
--rw-r--r--   0     1001      127     2242 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/build.rs
--rw-r--r--   0     1001      127    46445 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/fdbwriter.rs
--rw-r--r--   0     1001      127        0 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/google.protobuf.rs
--rw-r--r--   0     1001      127    13228 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/knowledgebox.rs
--rw-r--r--   0     1001      127     1256 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/lib.rs
--rw-r--r--   0     1001      127    95906 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/nodereader.rs
--rw-r--r--   0     1001      127    17860 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/noderesources.rs
--rw-r--r--   0     1001      127    60791 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/nodewriter.rs
--rw-r--r--   0     1001      127    24204 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/replication.rs
--rw-r--r--   0     1001      127    50406 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/resources.rs
--rw-r--r--   0     1001      127    10160 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/utils.rs
--rw-r--r--   0        0        0     3254 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/Cargo.toml
--rw-r--r--   0     1001      127     1045 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/.rustc_info.json
--rw-r--r--   0     1001      127      877 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/Makefile
--rw-r--r--   0     1001      127     1500 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/README.md
--rw-r--r--   0     1001      127     1757 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
--rw-r--r--   0     1001      127     3957 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/app.py
--rw-r--r--   0     1001      127    19055 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
--rw-r--r--   0     1001      127      890 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
--rw-r--r--   0     1001      127     2424 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
--rw-r--r--   0     1001      127     4015 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/pull.py
--rw-r--r--   0     1001      127     1535 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/service.py
--rw-r--r--   0     1001      127     1487 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/settings.py
--rw-r--r--   0     1001      127     1133 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/signals.py
--rw-r--r--   0     1001      127      835 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
--rw-r--r--   0     1001      127     1092 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
--rw-r--r--   0     1001      127    11343 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
--rw-r--r--   0     1001      127    13965 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
--rw-r--r--   0     1001      127     2300 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
--rw-r--r--   0     1001      127     2361 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
--rw-r--r--   0     1001      127    12999 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
--rw-r--r--   0     1001      127     3394 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
--rw-r--r--   0     1001      127     2489 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/writer.py
--rw-r--r--   0     1001      127      101 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/requirements-sources.txt
--rw-r--r--   0     1001      127      332 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/requirements.txt
--rw-r--r--   0     1001      127      249 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/setup.cfg
--rw-r--r--   0     1001      127     1405 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/setup.py
--rw-r--r--   0     1001      127     2518 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/analytics/blocking.rs
--rw-r--r--   0     1001      127     1219 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/analytics/mod.rs
--rw-r--r--   0     1001      127     4931 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/analytics/payload.rs
--rw-r--r--   0     1001      127    12828 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/analytics/sender.rs
--rw-r--r--   0     1001      127     3085 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/analytics/sink.rs
--rw-r--r--   0     1001      127     1900 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/analytics/sync.rs
--rw-r--r--   0     1001      127     5045 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/bin/reader.rs
--rw-r--r--   0     1001      127     8294 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/bin/writer.rs
--rw-r--r--   0     1001      127     1345 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/cache/mod.rs
--rw-r--r--   0     1001      127     3035 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
--rw-r--r--   0     1001      127    14199 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
--rw-r--r--   0     1001      127    11358 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
--rw-r--r--   0     1001      127     1771 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/disk_structure.rs
--rw-r--r--   0     1001      127     1111 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/errors.rs
--rw-r--r--   0     1001      127     2656 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
--rw-r--r--   0     1001      127    18813 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
--rw-r--r--   0     1001      127    19080 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
--rw-r--r--   0     1001      127     3186 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
--rw-r--r--   0     1001      127     3440 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
--rw-r--r--   0     1001      127     1009 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
--rw-r--r--   0     1001      127     4158 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
--rw-r--r--   0     1001      127     1283 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/mod.rs
--rw-r--r--   0     1001      127     2581 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/update.rs
--rw-r--r--   0     1001      127     1173 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
--rw-r--r--   0     1001      127     1465 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/http_server/mod.rs
--rw-r--r--   0     1001      127     1943 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
--rw-r--r--   0     1001      127     1504 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/lib.rs
--rw-r--r--   0     1001      127     2757 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/lifecycle.rs
--rw-r--r--   0     1001      127     1778 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/merge/global.rs
--rw-r--r--   0     1001      127     1089 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/merge/mod.rs
--rw-r--r--   0     1001      127    13672 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/merge/scheduler.rs
--rw-r--r--   0     1001      127     3677 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/merge/work.rs
--rw-r--r--   0     1001      127     1935 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/node_metadata.rs
--rw-r--r--   0     1001      127     2417 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/replication/health.rs
--rw-r--r--   0     1001      127     1070 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/replication/mod.rs
--rw-r--r--   0     1001      127    14162 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/replication/replicator.rs
--rw-r--r--   0     1001      127    11803 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/replication/service.rs
--rw-r--r--   0     1001      127    15603 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/settings.rs
--rw-r--r--   0     1001      127     1111 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/shards/errors.rs
--rw-r--r--   0     1001      127    11061 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/shards/indexes.rs
--rw-r--r--   0     1001      127    11116 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/shards/metadata.rs
--rw-r--r--   0     1001      127     1144 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/shards/mod.rs
--rw-r--r--   0     1001      127    28105 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
--rw-r--r--   0     1001      127    27145 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
--rw-r--r--   0     1001      127     1890 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/shards/versioning.rs
--rw-r--r--   0     1001      127    10199 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/telemetry.rs
--rw-r--r--   0     1001      127     6396 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/utils.rs
--rw-r--r--   0     1001      127       42 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/test.sh
--rw-r--r--   0     1001      127     1115 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/common/mod.rs
--rw-r--r--   0     1001      127    12731 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/common/node_services.rs
--rw-r--r--   0     1001      127     7823 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/common/resources.rs
--rw-r--r--   0     1001      127     8386 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
--rw-r--r--   0     1001      127     4089 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_download.rs
--rw-r--r--   0     1001      127     1684 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_merge.rs
--rw-r--r--   0     1001      127     6003 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_replication.rs
--rw-r--r--   0     1001      127    22494 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_search_relations.rs
--rw-r--r--   0     1001      127     6958 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
--rw-r--r--   0     1001      127     7044 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_security_search.rs
--rw-r--r--   0     1001      127     2508 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs
--rw-r--r--   0     1001      127     6862 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_shards.rs
--rw-r--r--   0     1001      127    10698 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_suggest.rs
--rw-r--r--   0     1001      127     5401 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
--rw-r--r--   0     1001      127     5147 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_vectorsets.rs
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1009 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
--rw-r--r--   0     1001      127    43324 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/reader.rs
--rw-r--r--   0     1001      127     4808 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/schema.rs
--rw-r--r--   0     1001      127    22494 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
--rw-r--r--   0     1001      127    11391 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
--rw-r--r--   0     1001      127     4090 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
--rw-r--r--   0     1001      127    18147 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/Cargo.toml
--rw-r--r--   0     1001      127     3593 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/src/io_maps.rs
--rw-r--r--   0     1001      127      916 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/src/lib.rs
--rw-r--r--   0     1001      127    17039 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/src/reader.rs
--rw-r--r--   0     1001      127     7123 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/src/schema.rs
--rw-r--r--   0     1001      127     7990 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/src/writer.rs
--rw-r--r--   0     1001      127     1802 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/tests/common/mod.rs
--rw-r--r--   0     1001      127     9523 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/tests/test_reader.rs
--rw-r--r--   0     1001      127     3296 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/tests/test_writer.rs
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/Cargo.toml
--rw-r--r--   0     1001      127     7796 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
--rw-r--r--   0     1001      127     1024 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/lib.rs
--rw-r--r--   0     1001      127     2780 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
--rw-r--r--   0     1001      127    43269 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/reader.rs
--rw-r--r--   0     1001      127     4407 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/schema.rs
--rw-r--r--   0     1001      127    21349 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
--rw-r--r--   0     1001      127    11723 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
--rw-r--r--   0     1001      127     2846 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
--rw-r--r--   0     1001      127     4090 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
--rw-r--r--   0     1001      127    17239 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/writer.rs
--rw-r--r--   0     1001      127       88 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
--rw-r--r--   0     1001      127    19791 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
--rw-r--r--   0     1001      127     1923 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
--rw-r--r--   0     1001      127    11684 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
--rw-r--r--   0     1001      127     2513 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
--rw-r--r--   0     1001      127    12802 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
--rw-r--r--   0     1001      127      730 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
--rw-r--r--   0     1001      127     2090 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
--rw-r--r--   0     1001      127     6284 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
--rw-r--r--   0     1001      127     1473 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
--rw-r--r--   0     1001      127     3451 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
--rw-r--r--   0     1001      127     3182 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
--rw-r--r--   0     1001      127     2126 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
--rw-r--r--   0     1001      127     2748 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
--rw-r--r--   0     1001      127     1388 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
--rw-r--r--   0     1001      127     5716 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
--rw-r--r--   0     1001      127     2108 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
--rw-r--r--   0     1001      127     8721 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
--rw-r--r--   0     1001      127     2535 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
--rw-r--r--   0     1001      127    11737 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
--rw-r--r--   0     1001      127     7730 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
--rw-r--r--   0     1001      127      756 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
--rw-r--r--   0     1001      127     1447 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
--rw-r--r--   0     1001      127     2055 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
--rw-r--r--   0     1001      127     3327 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
--rw-r--r--   0     1001      127     3856 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
--rw-r--r--   0     1001      127    23032 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
--rw-r--r--   0     1001      127      993 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
--rw-r--r--   0     1001      127     5424 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
--rw-r--r--   0     1001      127      491 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/Cargo.toml
--rw-r--r--   0     1001      127      931 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/src/lib.rs
--rw-r--r--   0     1001      127     2755 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/src/query_io.rs
--rw-r--r--   0     1001      127    22721 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/src/reader.rs
--rw-r--r--   0     1001      127     3105 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/src/schema.rs
--rw-r--r--   0     1001      127     8682 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/src/search_query.rs
--rw-r--r--   0     1001      127    10092 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/src/writer.rs
--rw-r--r--   0     1001      127     3435 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/tests/common/mod.rs
--rw-r--r--   0     1001      127     2152 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/tests/test_reader.rs
--rw-r--r--   0     1001      127     9567 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/tests/test_search.rs
--rw-r--r--   0     1001      127     1249 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
--rw-r--r--   0     1001      127     3523 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/tests/test_writer.rs
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/Cargo.toml
--rw-r--r--   0     1001      127       69 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/README.md
--rw-r--r--   0     1001      127       43 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/docs/README.md
--rw-r--r--   0     1001      127    25718 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
--rw-r--r--   0     1001      127    12340 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
--rw-r--r--   0     1001      127    24470 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
--rw-r--r--   0     1001      127    11214 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point/node.rs
--rw-r--r--   0     1001      127    15068 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
--rw-r--r--   0     1001      127     1741 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point/params.rs
--rw-r--r--   0     1001      127     3952 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
--rw-r--r--   0     1001      127    14175 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
--rw-r--r--   0     1001      127     5798 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
--rw-r--r--   0     1001      127     2777 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
--rw-r--r--   0     1001      127     7917 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
--rw-r--r--   0     1001      127     2304 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
--rw-r--r--   0     1001      127     5288 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
--rw-r--r--   0     1001      127    20587 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
--rw-r--r--   0     1001      127    23710 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
--rw-r--r--   0     1001      127     6916 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
--rw-r--r--   0     1001      127     1959 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
--rw-r--r--   0     1001      127     6143 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
--rw-r--r--   0     1001      127     2904 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
--rw-r--r--   0     1001      127     4433 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
--rw-r--r--   0     1001      127    10472 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/formula/mod.rs
--rw-r--r--   0     1001      127     2165 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/lib.rs
--rw-r--r--   0     1001      127     1278 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/service/mod.rs
--rw-r--r--   0     1001      127     1897 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/service/query_io.rs
--rw-r--r--   0     1001      127    17886 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/service/reader.rs
--rw-r--r--   0     1001      127    15558 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/service/writer.rs
--rw-r--r--   0     1001      127     1668 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/utils.rs
--rw-r--r--   0     1001      127     2884 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/tests/test_merge.rs
--rw-r--r--   0        0        0      932 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/Cargo.toml
--rw-r--r--   0     1001      127     5872 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/fs_state.rs
--rw-r--r--   0     1001      127     2969 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/lib.rs
--rw-r--r--   0     1001      127     2295 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/merge.rs
--rw-r--r--   0     1001      127      906 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
--rw-r--r--   0     1001      127     5462 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
--rw-r--r--   0     1001      127     1702 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
--rw-r--r--   0     1001      127     1442 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
--rw-r--r--   0     1001      127     1950 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
--rw-r--r--   0     1001      127     2626 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
--rw-r--r--   0     1001      127     1644 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
--rw-r--r--   0     1001      127    21641 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
--rw-r--r--   0     1001      127    16736 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
--rw-r--r--   0     1001      127     3415 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
--rw-r--r--   0     1001      127     1324 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/mod.rs
--rw-r--r--   0     1001      127     3074 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
--rw-r--r--   0     1001      127     3920 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/tests.rs
--rw-r--r--   0     1001      127     2944 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/paragraphs.rs
--rw-r--r--   0     1001      127    17305 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/query_language/mod.rs
--rw-r--r--   0     1001      127    15367 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/query_planner.rs
--rw-r--r--   0     1001      127     2023 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/relations.rs
--rw-r--r--   0     1001      127     8250 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/tantivy_replica.rs
--rw-r--r--   0     1001      127     2557 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/texts.rs
--rw-r--r--   0     1001      127     3460 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/vectors.rs
--rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1299/Cargo.toml
--rw-r--r--   0     1001      127     1553 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/CHANGELOG.md
--rw-r--r--   0     1001      127      895 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/Makefile
--rw-r--r--   0     1001      127       52 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/README.md
--rwxr-xr-x   0     1001      127      978 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/cov.sh
--rw-r--r--   0     1001      127     1332 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/pyproject.toml
--rw-r--r--   0     1001      127     2195 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/src/collect_garbage.rs
--rw-r--r--   0     1001      127     1212 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/src/errors.rs
--rw-r--r--   0     1001      127     2337 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/src/lib.rs
--rw-r--r--   0     1001      127     9405 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/src/reader.rs
--rw-r--r--   0     1001      127     2154 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/src/update.rs
--rw-r--r--   0     1001      127     8996 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/src/writer.rs
--rw-r--r--   0     1001      127      835 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/tests/__init__.py
--rw-r--r--   0     1001      127      892 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/tests/conftest.py
--rw-r--r--   0     1001      127     3903 2024-05-15 08:18:39.000000 nucliadb_node_binding-3.1.0.post1299/tests/integration/test_indexing.py
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1299/PKG-INFO
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/Cargo.toml
+-rw-r--r--   0     1001      127      931 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/src/lib.rs
+-rw-r--r--   0     1001      127     2755 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/src/query_io.rs
+-rw-r--r--   0     1001      127    22721 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/src/reader.rs
+-rw-r--r--   0     1001      127     3105 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/src/schema.rs
+-rw-r--r--   0     1001      127     8682 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/src/search_query.rs
+-rw-r--r--   0     1001      127    10092 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/src/writer.rs
+-rw-r--r--   0     1001      127     3435 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     2152 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     9567 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/tests/test_search.rs
+-rw-r--r--   0     1001      127     1249 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/tests/test_streaming.rs
+-rw-r--r--   0     1001      127     3523 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/tests/test_writer.rs
+-rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/Cargo.toml
+-rw-r--r--   0     1001      127       69 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/README.md
+-rw-r--r--   0     1001      127       43 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/docs/README.md
+-rw-r--r--   0     1001      127    25718 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg
+-rw-r--r--   0     1001      127    12340 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs
+-rw-r--r--   0     1001      127    24470 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point/mod.rs
+-rw-r--r--   0     1001      127    11214 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point/node.rs
+-rw-r--r--   0     1001      127    15068 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs
+-rw-r--r--   0     1001      127     1741 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point/params.rs
+-rw-r--r--   0     1001      127     3952 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs
+-rw-r--r--   0     1001      127    14175 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point/tests.rs
+-rw-r--r--   0     1001      127     5798 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs
+-rw-r--r--   0     1001      127     2777 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs
+-rw-r--r--   0     1001      127     8373 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs
+-rw-r--r--   0     1001      127     2304 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs
+-rw-r--r--   0     1001      127     5288 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs
+-rw-r--r--   0     1001      127    20587 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs
+-rw-r--r--   0     1001      127    23710 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs
+-rw-r--r--   0     1001      127     6916 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs
+-rw-r--r--   0     1001      127     1959 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_types/mod.rs
+-rw-r--r--   0     1001      127     6143 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_types/trie.rs
+-rw-r--r--   0     1001      127     2904 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs
+-rw-r--r--   0     1001      127     4433 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_types/vector.rs
+-rw-r--r--   0     1001      127    10472 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/formula/mod.rs
+-rw-r--r--   0     1001      127     2165 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/lib.rs
+-rw-r--r--   0     1001      127     1278 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/service/mod.rs
+-rw-r--r--   0     1001      127     1897 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/service/query_io.rs
+-rw-r--r--   0     1001      127    17981 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/service/reader.rs
+-rw-r--r--   0     1001      127    15558 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/service/writer.rs
+-rw-r--r--   0     1001      127     1668 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/utils.rs
+-rw-r--r--   0     1001      127     2884 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/tests/test_merge.rs
+-rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/Cargo.toml
+-rw-r--r--   0     1001      127     2242 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/build.rs
+-rw-r--r--   0     1001      127    46445 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/fdbwriter.rs
+-rw-r--r--   0     1001      127        0 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/google.protobuf.rs
+-rw-r--r--   0     1001      127    13228 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/knowledgebox.rs
+-rw-r--r--   0     1001      127     1256 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/lib.rs
+-rw-r--r--   0     1001      127    95906 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/nodereader.rs
+-rw-r--r--   0     1001      127    17860 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/noderesources.rs
+-rw-r--r--   0     1001      127    60791 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/nodewriter.rs
+-rw-r--r--   0     1001      127    24204 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/replication.rs
+-rw-r--r--   0     1001      127    50406 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/resources.rs
+-rw-r--r--   0     1001      127    10160 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/utils.rs
+-rw-r--r--   0        0        0     3254 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/Cargo.toml
+-rw-r--r--   0     1001      127     1045 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/.rustc_info.json
+-rw-r--r--   0     1001      127      877 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/Makefile
+-rw-r--r--   0     1001      127     1500 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/README.md
+-rw-r--r--   0     1001      127     1757 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/__init__.py
+-rw-r--r--   0     1001      127     3957 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/app.py
+-rw-r--r--   0     1001      127    19055 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/indexer.py
+-rw-r--r--   0     1001      127      890 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py
+-rw-r--r--   0     1001      127     2424 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py
+-rw-r--r--   0     1001      127     4015 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/pull.py
+-rw-r--r--   0     1001      127     1535 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/service.py
+-rw-r--r--   0     1001      127     1487 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/settings.py
+-rw-r--r--   0     1001      127     1133 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/signals.py
+-rw-r--r--   0     1001      127      835 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py
+-rw-r--r--   0     1001      127     1092 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py
+-rw-r--r--   0     1001      127    11343 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py
+-rw-r--r--   0     1001      127    13965 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py
+-rw-r--r--   0     1001      127     2300 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py
+-rw-r--r--   0     1001      127     2361 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py
+-rw-r--r--   0     1001      127    12999 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py
+-rw-r--r--   0     1001      127     3394 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py
+-rw-r--r--   0     1001      127     2489 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/writer.py
+-rw-r--r--   0     1001      127      101 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/requirements-sources.txt
+-rw-r--r--   0     1001      127      332 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/requirements.txt
+-rw-r--r--   0     1001      127      249 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/setup.cfg
+-rw-r--r--   0     1001      127     1405 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/setup.py
+-rw-r--r--   0     1001      127     2518 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/analytics/blocking.rs
+-rw-r--r--   0     1001      127     1219 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/analytics/mod.rs
+-rw-r--r--   0     1001      127     4931 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/analytics/payload.rs
+-rw-r--r--   0     1001      127    12828 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/analytics/sender.rs
+-rw-r--r--   0     1001      127     3085 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/analytics/sink.rs
+-rw-r--r--   0     1001      127     1900 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/analytics/sync.rs
+-rw-r--r--   0     1001      127     5045 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/bin/reader.rs
+-rw-r--r--   0     1001      127     8294 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/bin/writer.rs
+-rw-r--r--   0     1001      127     1345 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/cache/mod.rs
+-rw-r--r--   0     1001      127     3035 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/cache/reader_cache.rs
+-rw-r--r--   0     1001      127    14199 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/cache/resource_cache.rs
+-rw-r--r--   0     1001      127    11358 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/cache/writer_cache.rs
+-rw-r--r--   0     1001      127     1771 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/disk_structure.rs
+-rw-r--r--   0     1001      127     1111 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/errors.rs
+-rw-r--r--   0     1001      127     2656 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs
+-rw-r--r--   0     1001      127    18813 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs
+-rw-r--r--   0     1001      127    19080 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs
+-rw-r--r--   0     1001      127     3186 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs
+-rw-r--r--   0     1001      127     3440 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs
+-rw-r--r--   0     1001      127     1009 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs
+-rw-r--r--   0     1001      127     4158 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs
+-rw-r--r--   0     1001      127     1283 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/mod.rs
+-rw-r--r--   0     1001      127     2581 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/update.rs
+-rw-r--r--   0     1001      127     1173 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs
+-rw-r--r--   0     1001      127     1465 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/http_server/mod.rs
+-rw-r--r--   0     1001      127     1943 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/http_server/traces_service.rs
+-rw-r--r--   0     1001      127     1504 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/lib.rs
+-rw-r--r--   0     1001      127     2757 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/lifecycle.rs
+-rw-r--r--   0     1001      127     1778 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/merge/global.rs
+-rw-r--r--   0     1001      127     1089 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/merge/mod.rs
+-rw-r--r--   0     1001      127    13672 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/merge/scheduler.rs
+-rw-r--r--   0     1001      127     3677 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/merge/work.rs
+-rw-r--r--   0     1001      127     1935 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/node_metadata.rs
+-rw-r--r--   0     1001      127     2417 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/replication/health.rs
+-rw-r--r--   0     1001      127     1070 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/replication/mod.rs
+-rw-r--r--   0     1001      127    14162 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/replication/replicator.rs
+-rw-r--r--   0     1001      127    11803 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/replication/service.rs
+-rw-r--r--   0     1001      127    15603 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/settings.rs
+-rw-r--r--   0     1001      127     1111 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/shards/errors.rs
+-rw-r--r--   0     1001      127    11061 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/shards/indexes.rs
+-rw-r--r--   0     1001      127    11116 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/shards/metadata.rs
+-rw-r--r--   0     1001      127     1144 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/shards/mod.rs
+-rw-r--r--   0     1001      127    28745 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/shards/shard_reader.rs
+-rw-r--r--   0     1001      127    27145 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/shards/shard_writer.rs
+-rw-r--r--   0     1001      127     1890 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/shards/versioning.rs
+-rw-r--r--   0     1001      127    10199 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/telemetry.rs
+-rw-r--r--   0     1001      127     6396 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/utils.rs
+-rw-r--r--   0     1001      127       42 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/test.sh
+-rw-r--r--   0     1001      127     1115 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/common/mod.rs
+-rw-r--r--   0     1001      127    12731 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/common/node_services.rs
+-rw-r--r--   0     1001      127     7823 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/common/resources.rs
+-rw-r--r--   0     1001      127     8386 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_date_range_search.rs
+-rw-r--r--   0     1001      127     4089 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_download.rs
+-rw-r--r--   0     1001      127     1684 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_merge.rs
+-rw-r--r--   0     1001      127     6003 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_replication.rs
+-rw-r--r--   0     1001      127    22494 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_search_relations.rs
+-rw-r--r--   0     1001      127     6958 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_search_sorting.rs
+-rw-r--r--   0     1001      127     7044 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_security_search.rs
+-rw-r--r--   0     1001      127     2508 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs
+-rw-r--r--   0     1001      127     6862 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_shards.rs
+-rw-r--r--   0     1001      127    10698 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_suggest.rs
+-rw-r--r--   0     1001      127     5401 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs
+-rw-r--r--   0     1001      127     5147 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_vectorsets.rs
+-rw-r--r--   0        0        0      932 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/Cargo.toml
+-rw-r--r--   0     1001      127     5872 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/fs_state.rs
+-rw-r--r--   0     1001      127     2969 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/lib.rs
+-rw-r--r--   0     1001      127     2295 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/merge.rs
+-rw-r--r--   0     1001      127      906 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs
+-rw-r--r--   0     1001      127     5462 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs
+-rw-r--r--   0     1001      127     1702 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs
+-rw-r--r--   0     1001      127     1442 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs
+-rw-r--r--   0     1001      127     1950 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs
+-rw-r--r--   0     1001      127     2626 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs
+-rw-r--r--   0     1001      127     1644 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs
+-rw-r--r--   0     1001      127    21641 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs
+-rw-r--r--   0     1001      127    16736 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs
+-rw-r--r--   0     1001      127     3415 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs
+-rw-r--r--   0     1001      127     1324 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/mod.rs
+-rw-r--r--   0     1001      127     3074 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs
+-rw-r--r--   0     1001      127     3920 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/tests.rs
+-rw-r--r--   0     1001      127     2944 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/paragraphs.rs
+-rw-r--r--   0     1001      127    17305 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/query_language/mod.rs
+-rw-r--r--   0     1001      127    15367 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/query_planner.rs
+-rw-r--r--   0     1001      127     2023 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/relations.rs
+-rw-r--r--   0     1001      127     8250 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/tantivy_replica.rs
+-rw-r--r--   0     1001      127     2557 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/texts.rs
+-rw-r--r--   0     1001      127     3508 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/vectors.rs
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1024 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/query_io.rs
+-rw-r--r--   0     1001      127    43269 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/reader.rs
+-rw-r--r--   0     1001      127     4407 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/schema.rs
+-rw-r--r--   0     1001      127    21349 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/search_query.rs
+-rw-r--r--   0     1001      127    11723 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/search_response.rs
+-rw-r--r--   0     1001      127     2846 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/set_query.rs
+-rw-r--r--   0     1001      127     4090 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs
+-rw-r--r--   0     1001      127    17239 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/tr.json
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/Cargo.toml
+-rw-r--r--   0     1001      127     3593 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/src/io_maps.rs
+-rw-r--r--   0     1001      127      916 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/src/lib.rs
+-rw-r--r--   0     1001      127    17039 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/src/reader.rs
+-rw-r--r--   0     1001      127     7123 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/src/schema.rs
+-rw-r--r--   0     1001      127     7990 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/src/writer.rs
+-rw-r--r--   0     1001      127     1802 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/tests/common/mod.rs
+-rw-r--r--   0     1001      127     9523 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/tests/test_reader.rs
+-rw-r--r--   0     1001      127     3296 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/tests/test_writer.rs
+-rw-r--r--   0        0        0      361 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/Cargo.toml
+-rw-r--r--   0     1001      127     3409 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/src/lib.rs
+-rw-r--r--   0     1001      127     2885 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/src/measure.rs
+-rw-r--r--   0     1001      127     1081 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs
+-rw-r--r--   0     1001      127      222 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.stderr
+-rw-r--r--   0     1001      127     1038 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs
+-rw-r--r--   0     1001      127      327 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.stderr
+-rw-r--r--   0     1001      127     1086 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs
+-rw-r--r--   0     1001      127      249 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.stderr
+-rw-r--r--   0     1001      127     1046 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs
+-rw-r--r--   0     1001      127     1303 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr
+-rw-r--r--   0     1001      127     1408 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/tests/test_measure.rs
+-rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/Cargo.toml
+-rw-r--r--   0     1001      127     7796 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs
+-rw-r--r--   0     1001      127     1009 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/lib.rs
+-rw-r--r--   0     1001      127     2780 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/query_io.rs
+-rw-r--r--   0     1001      127    43324 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/reader.rs
+-rw-r--r--   0     1001      127     4808 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/schema.rs
+-rw-r--r--   0     1001      127    22494 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/search_query.rs
+-rw-r--r--   0     1001      127    11391 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/search_response.rs
+-rw-r--r--   0     1001      127     4090 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs
+-rw-r--r--   0     1001      127    18147 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/writer.rs
+-rw-r--r--   0     1001      127       88 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/README.md
+-rw-r--r--   0     1001      127    19791 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json
+-rw-r--r--   0     1001      127     1923 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/az.json
+-rw-r--r--   0     1001      127    11684 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json
+-rw-r--r--   0     1001      127     2513 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json
+-rw-r--r--   0     1001      127    12802 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json
+-rw-r--r--   0     1001      127      730 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/da.json
+-rw-r--r--   0     1001      127     2090 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/de.json
+-rw-r--r--   0     1001      127     6284 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/el.json
+-rw-r--r--   0     1001      127     1473 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/en.json
+-rw-r--r--   0     1001      127     3451 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/es.json
+-rw-r--r--   0     1001      127     3182 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json
+-rw-r--r--   0     1001      127     2126 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py
+-rw-r--r--   0     1001      127     2748 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json
+-rw-r--r--   0     1001      127     1388 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json
+-rw-r--r--   0     1001      127     5716 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/he.json
+-rw-r--r--   0     1001      127     2108 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json
+-rw-r--r--   0     1001      127     8721 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/id.json
+-rw-r--r--   0     1001      127     2535 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/it.json
+-rw-r--r--   0     1001      127    11737 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json
+-rw-r--r--   0     1001      127     7730 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json
+-rw-r--r--   0     1001      127      756 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json
+-rw-r--r--   0     1001      127     1447 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/no.json
+-rw-r--r--   0     1001      127     2055 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json
+-rw-r--r--   0     1001      127     3327 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json
+-rw-r--r--   0     1001      127     3856 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json
+-rw-r--r--   0     1001      127    23032 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json
+-rw-r--r--   0     1001      127      993 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json
+-rw-r--r--   0     1001      127     5424 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json
+-rw-r--r--   0     1001      127      491 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/tr.json
+-rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1302/Cargo.toml
+-rw-r--r--   0     1001      127     1553 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/CHANGELOG.md
+-rw-r--r--   0     1001      127      895 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/Makefile
+-rw-r--r--   0     1001      127       52 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/README.md
+-rwxr-xr-x   0     1001      127      978 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/cov.sh
+-rw-r--r--   0     1001      127     1332 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/pyproject.toml
+-rw-r--r--   0     1001      127     2195 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/src/collect_garbage.rs
+-rw-r--r--   0     1001      127     1212 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/src/errors.rs
+-rw-r--r--   0     1001      127     2337 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/src/lib.rs
+-rw-r--r--   0     1001      127     9405 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/src/reader.rs
+-rw-r--r--   0     1001      127     2154 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/src/update.rs
+-rw-r--r--   0     1001      127     8996 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/src/writer.rs
+-rw-r--r--   0     1001      127      835 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/tests/__init__.py
+-rw-r--r--   0     1001      127      892 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/tests/conftest.py
+-rw-r--r--   0     1001      127     3903 2024-05-15 11:01:35.000000 nucliadb_node_binding-3.1.0.post1302/tests/integration/test_indexing.py
+-rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 nucliadb_node_binding-3.1.0.post1302/PKG-INFO
```

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/src/lib.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/src/measure.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/src/measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/tests/dont_compile/actor_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/tests/dont_compile/actor_not_defined.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/tests/dont_compile/metric_defined_twice.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/tests/dont_compile/wrong_actor.stderr`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_procs/tests/test_measure.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_procs/tests/test_measure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/Cargo.toml` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/build.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/build.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/fdbwriter.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/fdbwriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/knowledgebox.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/knowledgebox.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/lib.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/nodereader.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/nodereader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/noderesources.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/noderesources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/nodewriter.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/nodewriter.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/replication.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/resources.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_protos/src/utils.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_protos/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/Cargo.toml` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/.rustc_info.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/.rustc_info.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/Makefile` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/README.md` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/README.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/__init__.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/app.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/indexer.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/listeners/indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/pull.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/service.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/service.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/settings.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/settings.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/signals.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/signals.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/integration/test_indexing.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_app.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexed_publisher.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_indexer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/tests/unit/test_pull.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/nucliadb_node/writer.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/nucliadb_node/writer.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/setup.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/setup.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/analytics/blocking.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/analytics/blocking.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/analytics/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/analytics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/analytics/payload.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/analytics/payload.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/analytics/sender.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/analytics/sender.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/analytics/sink.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/analytics/sink.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/analytics/sync.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/analytics/sync.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/bin/reader.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/bin/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/bin/writer.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/bin/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/cache/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/cache/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/cache/reader_cache.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/cache/reader_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/cache/resource_cache.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/cache/resource_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/cache/writer_cache.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/cache/writer_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/disk_structure.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/disk_structure.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/errors.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/grpc_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/grpc_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/middleware/debug.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/middleware/metrics.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/middleware/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/middleware/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/grpc/update.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/grpc/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/http_server/metrics_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/http_server/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/http_server/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/http_server/traces_service.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/http_server/traces_service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/lib.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/lifecycle.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/lifecycle.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/merge/global.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/merge/global.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/merge/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/merge/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/merge/scheduler.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/merge/scheduler.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/merge/work.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/merge/work.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/node_metadata.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/node_metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/replication/health.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/replication/health.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/replication/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/replication/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/replication/replicator.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/replication/replicator.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/replication/service.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/replication/service.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/settings.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/settings.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/shards/errors.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/shards/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/shards/indexes.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/shards/indexes.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/shards/metadata.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/shards/metadata.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/shards/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/shards/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/shards/shard_reader.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/shards/shard_reader.rs`

 * *Files 2% similar despite different names*

```diff
@@ -641,19 +641,35 @@
     pub fn update(&self) -> NodeResult<()> {
         let shard_path = self.metadata.shard_path();
         // TODO: while we don't have all shards migrated, we still have to
         // unwrap with a default
         let indexes = ShardIndexes::load(&shard_path).unwrap_or_else(|_| ShardIndexes::new(&shard_path));
 
         let mut updated_indexes = HashMap::with_capacity(indexes.count_vectors_indexes());
+        let mut keep_indexes = vec![];
+        let vector_indexes = read_rw_lock(&self.vector_readers);
         for (vectorset, path) in indexes.iter_vectors_indexes() {
+            if let Some(existing_index) = vector_indexes.get(&vectorset) {
+                if let Ok(false) = existing_index.needs_update() {
+                    // Index already loaded and does not need update, skip
+                    keep_indexes.push(vectorset);
+                    continue;
+                }
+            }
             let new_reader = open_vectors_reader(self.versions.vectors, &path)?;
             updated_indexes.insert(vectorset, new_reader);
         }
+        drop(vector_indexes);
+
         let mut vector_indexes = write_rw_lock(&self.vector_readers);
+        for keep in keep_indexes {
+            if let Some(index) = vector_indexes.remove(&keep) {
+                updated_indexes.insert(keep, index);
+            }
+        }
         *vector_indexes = updated_indexes;
         Ok(())
     }
 
     fn vectors_index_search(
         &self,
         request: &VectorSearchRequest,
```

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/shards/shard_writer.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/shards/shard_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/shards/versioning.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/shards/versioning.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/telemetry.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/telemetry.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/src/utils.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/common/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/common/node_services.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/common/node_services.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/common/resources.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/common/resources.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_date_range_search.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_date_range_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_download.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_download.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_merge.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_replication.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_search_relations.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_search_relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_search_sorting.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_search_sorting.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_security_search.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_security_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_set_resource_from_storage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_shards.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_shards.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_suggest.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_suggest.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_vector_normalization.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_node/tests/test_vectorsets.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_node/tests/test_vectorsets.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/Cargo.toml` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/lib.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/query_io.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/reader.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/schema.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/search_query.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/search_response.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/src/writer.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/az.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/da.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/de.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/el.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/en.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/es.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/he.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/id.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/it.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/no.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/Cargo.toml` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/src/io_maps.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/src/io_maps.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/src/lib.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/src/reader.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/src/schema.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/src/writer.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/tests/common/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/tests/test_reader.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_relations2/tests/test_writer.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_relations2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/Cargo.toml` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/fuzzy_query.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/fuzzy_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/lib.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/query_io.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/reader.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/schema.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/search_query.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/search_response.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/search_response.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/set_query.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/set_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/stop_words.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/src/stop_words.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/src/writer.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs3/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/ar.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/ar.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/az.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/az.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/bn.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/bn.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/ca.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/ca.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/ch.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/ch.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/da.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/da.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/de.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/de.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/el.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/el.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/en.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/en.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/es.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/es.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/eu.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/eu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/extract.py` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/extract.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/fi.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/fi.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/fr.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/fr.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/he.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/he.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/hu.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/hu.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/id.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/id.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/it.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/it.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/kk.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/kk.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/ne.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/ne.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/nl.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/nl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/no.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/no.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/pt.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/pt.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/ro.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/ro.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/ru.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/ru.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/sl.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/sl.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/sv.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/sv.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_paragraphs3/stop_words/tg.json` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_paragraphs2/stop_words/tg.json`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/src/lib.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/src/query_io.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/src/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/src/reader.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/src/schema.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/src/schema.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/src/search_query.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/src/search_query.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/src/writer.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/tests/common/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/tests/common/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/tests/test_reader.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/tests/test_reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/tests/test_search.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/tests/test_search.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/tests/test_streaming.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/tests/test_streaming.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_texts2/tests/test_writer.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_texts2/tests/test_writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/Cargo.toml` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/docs/labels.drawio.svg`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point/disk_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point/node.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point/node.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point/ops_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point/params.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point/params.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point/ram_hnsw.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point/tests.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point_provider/garbage_collector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point_provider/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point_provider/reader.rs`

 * *Files 4% similar despite different names*

```diff
@@ -101,14 +101,19 @@
 pub struct Reader {
     metadata: IndexMetadata,
     path: PathBuf,
     open_data_points: FxHashMap<DpId, OpenDataPoint>,
     delete_log: DTrie,
     number_of_embeddings: usize,
     dimension: Option<u64>,
+    state_last_modified: SystemTime,
+}
+
+fn last_modified(path: &Path) -> std::io::Result<SystemTime> {
+    std::fs::metadata(path)?.modified()
 }
 
 impl Reader {
     pub fn open(path: &Path) -> VectorR<Reader> {
         let lock_path = path.join(OPENING_FLAG);
         let lock_file = File::create(lock_path)?;
         lock_file.lock_shared()?;
@@ -117,14 +122,15 @@
             // Old indexes may not have this file so in that case the
             // metadata file they should have is created.
             let metadata = IndexMetadata::default();
             metadata.write(path).map(|_| metadata)
         })?;
 
         let state_path = path.join(STATE);
+        let state_last_modified = last_modified(&state_path)?;
         let state_file = File::open(state_path)?;
         let state = read_state(&state_file)?;
         let data_point_list = state.data_point_list;
         let delete_log = state.delete_log;
         let mut dimension = None;
         let mut data_point_pins = Vec::new();
         let mut open_data_points = FxHashMap::default();
@@ -148,14 +154,15 @@
         Ok(Reader {
             metadata,
             open_data_points,
             delete_log,
             number_of_embeddings,
             dimension,
             path: path.to_path_buf(),
+            state_last_modified,
         })
     }
 
     pub fn search(&self, request: &dyn SearchRequest) -> VectorR<Vec<Neighbour>> {
         let Some(dimension) = self.dimension else {
             return Ok(Vec::with_capacity(0));
         };
@@ -231,8 +238,14 @@
     pub fn metadata(&self) -> &IndexMetadata {
         &self.metadata
     }
 
     pub fn embedding_dimension(&self) -> Option<u64> {
         self.dimension
     }
+
+    pub fn needs_update(&self) -> VectorR<bool> {
+        let state_path = self.path.join(STATE);
+        let state_modified = last_modified(&state_path)?;
+        Ok(self.state_last_modified < state_modified)
+    }
 }
```

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point_provider/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point_provider/state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_point_provider/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_types/data_store.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_types/dtrie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_types/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_types/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_types/trie.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_types/trie.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_types/trie_ram.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/data_types/vector.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/data_types/vector.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/formula/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/formula/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/lib.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/service/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/service/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/service/query_io.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/service/query_io.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/service/reader.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/service/reader.rs`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,18 @@
         let time = Instant::now();
         let result = self.index.keys()?;
         let v = time.elapsed().as_millis();
         debug!("Ending at {v} ms");
 
         Ok(result)
     }
+
+    fn needs_update(&self) -> NodeResult<bool> {
+        Ok(self.index.needs_update()?)
+    }
 }
 
 impl TryFrom<Neighbour> for DocumentScored {
     type Error = String;
     fn try_from(neighbour: Neighbour) -> Result<Self, Self::Error> {
         let id = std::str::from_utf8(neighbour.id());
         let metadata = neighbour.metadata().map(SentenceMetadata::decode);
```

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/service/writer.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/service/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/src/utils.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/src/utils.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_vectors/tests/test_merge.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_vectors/tests/test_merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/Cargo.toml` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/fs_state.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/fs_state.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/lib.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/merge.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/merge.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/meters/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/meters/prometheus.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/grpc_ops.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/replication.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/request_time.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/shard_cache.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/tokio_runtime.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/tokio_tasks.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/metric/vectors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/task_monitor.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/metrics/tests.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/metrics/tests.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/paragraphs.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/paragraphs.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/query_language/mod.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/query_language/mod.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/query_planner.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/query_planner.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/relations.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/relations.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/tantivy_replica.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/tantivy_replica.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/texts.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/texts.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/local_dependencies/nucliadb_core/src/vectors.rs` & `nucliadb_node_binding-3.1.0.post1302/local_dependencies/nucliadb_core/src/vectors.rs`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     fn run(&mut self) -> NodeResult<Box<dyn MergeResults>>;
 }
 
 pub trait VectorReader: std::fmt::Debug + Send + Sync {
     fn search(&self, request: &ProtosRequest, context: &VectorsContext) -> NodeResult<ProtosResponse>;
     fn stored_ids(&self) -> NodeResult<Vec<String>>;
     fn count(&self) -> NodeResult<usize>;
+    fn needs_update(&self) -> NodeResult<bool>;
 }
 
 pub trait VectorWriter: std::fmt::Debug + Send + Sync {
     fn count(&self) -> NodeResult<usize>;
     fn get_segment_ids(&self) -> NodeResult<Vec<String>>;
     fn get_index_files(&self, ignored_segment_ids: &[String]) -> NodeResult<IndexFiles>;
```

### Comparing `nucliadb_node_binding-3.1.0.post1299/Cargo.toml` & `nucliadb_node_binding-3.1.0.post1302/Cargo.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "nucliadb_node_binding"
-version = "3.1.0-post1299"
+version = "3.1.0-post1302"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nucliadb_node_binding"
 crate-type = ["cdylib"]
```

### Comparing `nucliadb_node_binding-3.1.0.post1299/CHANGELOG.md` & `nucliadb_node_binding-3.1.0.post1302/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/Makefile` & `nucliadb_node_binding-3.1.0.post1302/Makefile`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/cov.sh` & `nucliadb_node_binding-3.1.0.post1302/cov.sh`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/pyproject.toml` & `nucliadb_node_binding-3.1.0.post1302/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/src/collect_garbage.rs` & `nucliadb_node_binding-3.1.0.post1302/src/collect_garbage.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/src/errors.rs` & `nucliadb_node_binding-3.1.0.post1302/src/errors.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/src/lib.rs` & `nucliadb_node_binding-3.1.0.post1302/src/lib.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/src/reader.rs` & `nucliadb_node_binding-3.1.0.post1302/src/reader.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/src/update.rs` & `nucliadb_node_binding-3.1.0.post1302/src/update.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/src/writer.rs` & `nucliadb_node_binding-3.1.0.post1302/src/writer.rs`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/tests/__init__.py` & `nucliadb_node_binding-3.1.0.post1302/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/tests/conftest.py` & `nucliadb_node_binding-3.1.0.post1302/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nucliadb_node_binding-3.1.0.post1299/tests/integration/test_indexing.py` & `nucliadb_node_binding-3.1.0.post1302/tests/integration/test_indexing.py`

 * *Files identical despite different names*
