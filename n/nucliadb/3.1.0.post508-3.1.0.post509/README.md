# Comparing `tmp/nucliadb-3.1.0.post508-py3-none-any.whl.zip` & `tmp/nucliadb-3.1.0.post509-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,462 +1,462 @@
-Zip file size: 763375 bytes, number of entries: 460
--rw-r--r--  2.0 unx     1135 b- defN 24-May-16 14:31 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-16 14:31 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-May-16 14:31 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-16 14:31 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-16 14:31 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-16 14:31 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-May-16 14:31 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-16 14:31 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-May-16 14:31 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-May-16 14:31 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-16 14:31 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-16 14:31 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-16 14:31 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-May-16 14:31 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-16 14:31 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-May-16 14:31 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-May-16 14:31 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-16 14:31 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx     3282 b- defN 24-May-16 14:31 migrations/0020_drain_nodes_from_cluster.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-16 14:31 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-May-16 14:31 nucliadb/health.py
--rw-r--r--  2.0 unx    11626 b- defN 24-May-16 14:31 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-May-16 14:31 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-May-16 14:31 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 14:31 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     5022 b- defN 24-May-16 14:31 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     4971 b- defN 24-May-16 14:31 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-May-16 14:31 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3793 b- defN 24-May-16 14:31 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-May-16 14:31 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    22097 b- defN 24-May-16 14:31 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8593 b- defN 24-May-16 14:31 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    20209 b- defN 24-May-16 14:31 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     2992 b- defN 24-May-16 14:31 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5730 b- defN 24-May-16 14:31 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-May-16 14:31 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12518 b- defN 24-May-16 14:31 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-May-16 14:31 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-16 14:31 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-May-16 14:31 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-May-16 14:31 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:31 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13707 b- defN 24-May-16 14:31 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-May-16 14:31 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-16 14:31 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3545 b- defN 24-May-16 14:31 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3440 b- defN 24-May-16 14:31 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-May-16 14:31 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1813 b- defN 24-May-16 14:31 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     1451 b- defN 24-May-16 14:31 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-May-16 14:31 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-May-16 14:31 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-May-16 14:31 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-May-16 14:31 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-16 14:31 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx     8719 b- defN 24-May-16 14:31 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5634 b- defN 24-May-16 14:31 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1631 b- defN 24-May-16 14:31 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-May-16 14:31 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-May-16 14:31 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-May-16 14:31 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-May-16 14:31 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-May-16 14:31 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-May-16 14:31 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      946 b- defN 24-May-16 14:31 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-May-16 14:31 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-May-16 14:31 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-May-16 14:31 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    14502 b- defN 24-May-16 14:31 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4109 b- defN 24-May-16 14:31 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-May-16 14:31 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-May-16 14:31 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-May-16 14:31 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-May-16 14:31 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-May-16 14:31 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-16 14:31 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-May-16 14:31 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19401 b- defN 24-May-16 14:31 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-16 14:31 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-May-16 14:31 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-May-16 14:31 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-May-16 14:31 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19541 b- defN 24-May-16 14:31 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx    20277 b- defN 24-May-16 14:31 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3183 b- defN 24-May-16 14:31 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-May-16 14:31 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx    11563 b- defN 24-May-16 14:31 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12174 b- defN 24-May-16 14:31 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3788 b- defN 24-May-16 14:31 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-May-16 14:31 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-May-16 14:31 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6935 b- defN 24-May-16 14:31 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-May-16 14:31 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-May-16 14:31 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    18433 b- defN 24-May-16 14:31 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-May-16 14:31 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-May-16 14:31 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-May-16 14:31 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     5159 b- defN 24-May-16 14:31 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-May-16 14:31 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-May-16 14:31 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-May-16 14:31 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4531 b- defN 24-May-16 14:31 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-16 14:31 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28448 b- defN 24-May-16 14:31 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-May-16 14:31 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1279 b- defN 24-May-16 14:31 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    17167 b- defN 24-May-16 14:31 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-May-16 14:31 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    60444 b- defN 24-May-16 14:31 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     1739 b- defN 24-May-16 14:31 nucliadb/ingest/orm/synonyms.py
--rw-r--r--  2.0 unx     3683 b- defN 24-May-16 14:31 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    26423 b- defN 24-May-16 14:31 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     1690 b- defN 24-May-16 14:31 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-May-16 14:31 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    33196 b- defN 24-May-16 14:31 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-May-16 14:31 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24060 b- defN 24-May-16 14:31 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-May-16 14:31 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:31 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2549 b- defN 24-May-16 14:31 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2591 b- defN 24-May-16 14:31 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4465 b- defN 24-May-16 14:31 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-May-16 14:31 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-May-16 14:31 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27336 b- defN 24-May-16 14:31 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-16 14:31 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-16 14:31 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     4004 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4140 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-May-16 14:31 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-May-16 14:31 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-May-16 14:31 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-16 14:31 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-16 14:31 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-May-16 14:31 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-May-16 14:31 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9382 b- defN 24-May-16 14:31 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-May-16 14:31 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-16 14:31 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-May-16 14:31 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-16 14:31 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-May-16 14:31 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-May-16 14:31 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-16 14:31 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-May-16 14:31 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-May-16 14:31 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-16 14:31 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx     1447 b- defN 24-May-16 14:31 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-May-16 14:31 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2434 b- defN 24-May-16 14:31 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-16 14:31 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12392 b- defN 24-May-16 14:31 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6459 b- defN 24-May-16 14:31 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3641 b- defN 24-May-16 14:31 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2099 b- defN 24-May-16 14:31 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4472 b- defN 24-May-16 14:31 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13940 b- defN 24-May-16 14:31 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-16 14:31 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    12399 b- defN 24-May-16 14:31 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     8155 b- defN 24-May-16 14:31 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-May-16 14:31 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-May-16 14:31 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-May-16 14:31 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-May-16 14:31 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-May-16 14:31 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-May-16 14:31 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-May-16 14:31 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-May-16 14:31 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-May-16 14:31 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-May-16 14:31 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    20665 b- defN 24-May-16 14:31 nucliadb/search/predict.py
--rw-r--r--  2.0 unx     1402 b- defN 24-May-16 14:31 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-May-16 14:31 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-16 14:31 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1298 b- defN 24-May-16 14:31 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     3534 b- defN 24-May-16 14:31 nucliadb/search/api/v1/ask.py
--rw-r--r--  2.0 unx     9486 b- defN 24-May-16 14:31 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2668 b- defN 24-May-16 14:31 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8810 b- defN 24-May-16 14:31 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6938 b- defN 24-May-16 14:31 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3047 b- defN 24-May-16 14:31 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-16 14:31 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    18337 b- defN 24-May-16 14:31 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5970 b- defN 24-May-16 14:31 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-16 14:31 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-16 14:31 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     4066 b- defN 24-May-16 14:31 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5821 b- defN 24-May-16 14:31 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5303 b- defN 24-May-16 14:31 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:31 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9111 b- defN 24-May-16 14:31 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-May-16 14:31 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-16 14:31 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-May-16 14:31 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-May-16 14:31 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-May-16 14:31 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-May-16 14:31 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-May-16 14:31 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-May-16 14:31 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-May-16 14:31 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-May-16 14:31 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31127 b- defN 24-May-16 14:31 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-May-16 14:31 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-May-16 14:31 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-May-16 14:31 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx    16676 b- defN 24-May-16 14:31 nucliadb/search/search/chat/ask.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-16 14:31 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-May-16 14:31 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    17543 b- defN 24-May-16 14:31 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-May-16 14:31 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-May-16 14:31 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15480 b- defN 24-May-16 14:31 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    15721 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     3759 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/api/v1/test_ask.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     5121 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-May-16 14:31 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-May-16 14:31 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-May-16 14:31 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-May-16 14:31 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5309 b- defN 24-May-16 14:31 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6930 b- defN 24-May-16 14:31 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-May-16 14:31 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1980 b- defN 24-May-16 14:31 nucliadb/standalone/migrations.py
--rw-r--r--  2.0 unx     1317 b- defN 24-May-16 14:31 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx     5415 b- defN 24-May-16 14:31 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5781 b- defN 24-May-16 14:31 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-May-16 14:31 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-May-16 14:31 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-May-16 14:31 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-May-16 14:31 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-May-16 14:31 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-16 14:31 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:31 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-May-16 14:31 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-May-16 14:31 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-16 14:31 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1845 b- defN 24-May-16 14:31 nucliadb/standalone/tests/unit/test_migrations.py
--rw-r--r--  2.0 unx     1587 b- defN 24-May-16 14:31 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-May-16 14:31 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-16 14:31 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-May-16 14:31 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-May-16 14:31 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-16 14:31 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-May-16 14:31 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-May-16 14:31 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-May-16 14:31 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-May-16 14:31 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-May-16 14:31 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-May-16 14:31 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-May-16 14:31 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-May-16 14:31 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-May-16 14:31 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-May-16 14:31 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-May-16 14:31 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-May-16 14:31 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3662 b- defN 24-May-16 14:31 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-May-16 14:31 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2780 b- defN 24-May-16 14:31 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-16 14:31 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-May-16 14:31 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-May-16 14:31 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-May-16 14:31 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3649 b- defN 24-May-16 14:31 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-May-16 14:31 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    12240 b- defN 24-May-16 14:31 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-May-16 14:31 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     9465 b- defN 24-May-16 14:31 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5627 b- defN 24-May-16 14:31 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:31 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3761 b- defN 24-May-16 14:31 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2136 b- defN 24-May-16 14:31 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:31 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-May-16 14:31 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     1869 b- defN 24-May-16 14:31 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     3093 b- defN 24-May-16 14:31 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-May-16 14:31 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-May-16 14:31 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-May-16 14:31 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-May-16 14:31 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-May-16 14:31 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-May-16 14:31 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-May-16 14:31 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-May-16 14:31 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-May-16 14:31 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-May-16 14:31 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-May-16 14:31 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-May-16 14:31 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-May-16 14:31 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-May-16 14:31 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-May-16 14:31 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-May-16 14:31 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-May-16 14:31 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-May-16 14:31 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-May-16 14:31 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-16 14:31 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-May-16 14:31 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-May-16 14:31 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-May-16 14:31 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-May-16 14:31 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-May-16 14:31 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-May-16 14:31 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-May-16 14:31 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-16 14:31 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2071 b- defN 24-May-16 14:31 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-May-16 14:31 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1908 b- defN 24-May-16 14:31 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2135 b- defN 24-May-16 14:31 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-May-16 14:31 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-May-16 14:31 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-May-16 14:31 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-May-16 14:31 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-May-16 14:31 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-May-16 14:31 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-May-16 14:31 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-May-16 14:31 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-May-16 14:31 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-May-16 14:31 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-May-16 14:31 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-May-16 14:31 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1876 b- defN 24-May-16 14:31 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-16 14:31 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2417 b- defN 24-May-16 14:31 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-May-16 14:31 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-May-16 14:31 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-May-16 14:31 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-May-16 14:31 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-May-16 14:31 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-May-16 14:31 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-May-16 14:31 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-May-16 14:31 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-May-16 14:31 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-May-16 14:31 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-May-16 14:31 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-16 14:31 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-May-16 14:31 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19495 b- defN 24-May-16 14:31 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-May-16 14:31 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-May-16 14:31 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-May-16 14:31 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx     1448 b- defN 24-May-16 14:31 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3074 b- defN 24-May-16 14:31 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-May-16 14:31 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-May-16 14:31 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-May-16 14:31 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6571 b- defN 24-May-16 14:31 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24482 b- defN 24-May-16 14:31 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5248 b- defN 24-May-16 14:31 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-16 14:31 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18893 b- defN 24-May-16 14:31 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-May-16 14:31 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10747 b- defN 24-May-16 14:31 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30857 b- defN 24-May-16 14:31 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-May-16 14:31 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-May-16 14:31 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-May-16 14:31 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-May-16 14:31 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16319 b- defN 24-May-16 14:31 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-May-16 14:31 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx     1152 b- defN 24-May-16 14:31 nucliadb/writer/resource/slug.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:31 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-May-16 14:31 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-May-16 14:31 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-May-16 14:31 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25999 b- defN 24-May-16 14:31 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-May-16 14:31 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4358 b- defN 24-May-16 14:31 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16694 b- defN 24-May-16 14:31 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-May-16 14:31 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-May-16 14:31 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-May-16 14:31 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-May-16 14:31 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-May-16 14:31 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-May-16 14:31 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-May-16 14:31 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-May-16 14:31 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-May-16 14:31 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-May-16 14:31 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-May-16 14:31 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-May-16 14:31 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4399 b- defN 24-May-16 14:32 nucliadb-3.1.0.post508.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-16 14:32 nucliadb-3.1.0.post508.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-May-16 14:32 nucliadb-3.1.0.post508.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-May-16 14:32 nucliadb-3.1.0.post508.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-16 14:32 nucliadb-3.1.0.post508.dist-info/zip-safe
--rw-rw-r--  2.0 unx    43144 b- defN 24-May-16 14:32 nucliadb-3.1.0.post508.dist-info/RECORD
-460 files, 2259472 bytes uncompressed, 694385 bytes compressed:  69.3%
+Zip file size: 763374 bytes, number of entries: 460
+-rw-r--r--  2.0 unx     1135 b- defN 24-May-16 14:43 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-16 14:43 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-May-16 14:43 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-16 14:43 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-16 14:43 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-16 14:43 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-May-16 14:43 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-16 14:43 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-May-16 14:43 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-May-16 14:43 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-May-16 14:43 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-16 14:43 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-16 14:43 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-May-16 14:43 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-16 14:43 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-May-16 14:43 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-May-16 14:43 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-16 14:43 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx     3282 b- defN 24-May-16 14:43 migrations/0020_drain_nodes_from_cluster.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-May-16 14:43 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-May-16 14:43 nucliadb/health.py
+-rw-r--r--  2.0 unx    11626 b- defN 24-May-16 14:43 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-May-16 14:43 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-May-16 14:43 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 14:43 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     5022 b- defN 24-May-16 14:43 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     4971 b- defN 24-May-16 14:43 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-May-16 14:43 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3793 b- defN 24-May-16 14:43 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-May-16 14:43 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    22091 b- defN 24-May-16 14:43 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8590 b- defN 24-May-16 14:43 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    20209 b- defN 24-May-16 14:43 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     2992 b- defN 24-May-16 14:43 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5713 b- defN 24-May-16 14:43 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-May-16 14:43 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12515 b- defN 24-May-16 14:43 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-May-16 14:43 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-16 14:43 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-May-16 14:43 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-May-16 14:43 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:43 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13707 b- defN 24-May-16 14:43 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-May-16 14:43 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-16 14:43 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3545 b- defN 24-May-16 14:43 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3440 b- defN 24-May-16 14:43 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-May-16 14:43 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1813 b- defN 24-May-16 14:43 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-May-16 14:43 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-May-16 14:43 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-May-16 14:43 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-May-16 14:43 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-May-16 14:43 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-16 14:43 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx     8719 b- defN 24-May-16 14:43 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5634 b- defN 24-May-16 14:43 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1631 b- defN 24-May-16 14:43 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-May-16 14:43 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-May-16 14:43 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-May-16 14:43 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-May-16 14:43 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-May-16 14:43 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-May-16 14:43 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      946 b- defN 24-May-16 14:43 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-May-16 14:43 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-May-16 14:43 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-May-16 14:43 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    14502 b- defN 24-May-16 14:43 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4109 b- defN 24-May-16 14:43 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-May-16 14:43 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-May-16 14:43 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-May-16 14:43 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-May-16 14:43 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-May-16 14:43 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-16 14:43 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-May-16 14:43 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19401 b- defN 24-May-16 14:43 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-16 14:43 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-16 14:43 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-May-16 14:43 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-May-16 14:43 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19541 b- defN 24-May-16 14:43 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx    20277 b- defN 24-May-16 14:43 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3183 b- defN 24-May-16 14:43 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-May-16 14:43 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx    11563 b- defN 24-May-16 14:43 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12174 b- defN 24-May-16 14:43 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3788 b- defN 24-May-16 14:43 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-May-16 14:43 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-May-16 14:43 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6935 b- defN 24-May-16 14:43 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-May-16 14:43 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-May-16 14:43 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    18433 b- defN 24-May-16 14:43 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-May-16 14:43 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-May-16 14:43 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-May-16 14:43 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     5159 b- defN 24-May-16 14:43 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-16 14:43 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-May-16 14:43 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-16 14:43 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4531 b- defN 24-May-16 14:43 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-16 14:43 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28448 b- defN 24-May-16 14:43 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-May-16 14:43 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1279 b- defN 24-May-16 14:43 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    17167 b- defN 24-May-16 14:43 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-May-16 14:43 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    60444 b- defN 24-May-16 14:43 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     1739 b- defN 24-May-16 14:43 nucliadb/ingest/orm/synonyms.py
+-rw-r--r--  2.0 unx     3683 b- defN 24-May-16 14:43 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    26420 b- defN 24-May-16 14:43 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-May-16 14:43 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-May-16 14:43 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    33193 b- defN 24-May-16 14:43 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-May-16 14:43 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24060 b- defN 24-May-16 14:43 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-May-16 14:43 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:43 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2549 b- defN 24-May-16 14:43 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2591 b- defN 24-May-16 14:43 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4465 b- defN 24-May-16 14:43 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-May-16 14:43 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-May-16 14:43 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27336 b- defN 24-May-16 14:43 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-16 14:43 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-16 14:43 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     4004 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4140 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-May-16 14:43 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-May-16 14:43 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-May-16 14:43 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-16 14:43 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-16 14:43 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-May-16 14:43 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-16 14:43 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9370 b- defN 24-May-16 14:43 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-May-16 14:43 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-16 14:43 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-May-16 14:43 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-16 14:43 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-May-16 14:43 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-May-16 14:43 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-16 14:43 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-May-16 14:43 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-16 14:43 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-16 14:43 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx     1447 b- defN 24-May-16 14:43 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-May-16 14:43 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2434 b- defN 24-May-16 14:43 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-16 14:43 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12392 b- defN 24-May-16 14:43 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6459 b- defN 24-May-16 14:43 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3641 b- defN 24-May-16 14:43 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2099 b- defN 24-May-16 14:43 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4472 b- defN 24-May-16 14:43 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13940 b- defN 24-May-16 14:43 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-16 14:43 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    12399 b- defN 24-May-16 14:43 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     8155 b- defN 24-May-16 14:43 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-May-16 14:43 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-May-16 14:43 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-May-16 14:43 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-May-16 14:43 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-May-16 14:43 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-May-16 14:43 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-May-16 14:43 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-May-16 14:43 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-16 14:43 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-May-16 14:43 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    20665 b- defN 24-May-16 14:43 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-16 14:43 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-May-16 14:43 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-16 14:43 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1298 b- defN 24-May-16 14:43 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3534 b- defN 24-May-16 14:43 nucliadb/search/api/v1/ask.py
+-rw-r--r--  2.0 unx     9486 b- defN 24-May-16 14:43 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2668 b- defN 24-May-16 14:43 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8810 b- defN 24-May-16 14:43 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6938 b- defN 24-May-16 14:43 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3047 b- defN 24-May-16 14:43 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-May-16 14:43 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    18337 b- defN 24-May-16 14:43 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5970 b- defN 24-May-16 14:43 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-16 14:43 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-16 14:43 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     4066 b- defN 24-May-16 14:43 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5821 b- defN 24-May-16 14:43 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5303 b- defN 24-May-16 14:43 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:43 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9111 b- defN 24-May-16 14:43 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-May-16 14:43 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-16 14:43 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-May-16 14:43 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-May-16 14:43 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-May-16 14:43 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-May-16 14:43 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-May-16 14:43 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-16 14:43 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-May-16 14:43 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-May-16 14:43 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31127 b- defN 24-May-16 14:43 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-May-16 14:43 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-May-16 14:43 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-16 14:43 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx    16676 b- defN 24-May-16 14:43 nucliadb/search/search/chat/ask.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-16 14:43 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-May-16 14:43 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    17543 b- defN 24-May-16 14:43 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-May-16 14:43 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-May-16 14:43 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-May-16 14:43 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    15721 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3759 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/api/v1/test_ask.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     5121 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-May-16 14:43 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-May-16 14:43 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-May-16 14:43 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-May-16 14:43 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5309 b- defN 24-May-16 14:43 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6930 b- defN 24-May-16 14:43 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-May-16 14:43 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1980 b- defN 24-May-16 14:43 nucliadb/standalone/migrations.py
+-rw-r--r--  2.0 unx     1317 b- defN 24-May-16 14:43 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx     5415 b- defN 24-May-16 14:43 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5781 b- defN 24-May-16 14:43 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-May-16 14:43 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-May-16 14:43 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-May-16 14:43 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-May-16 14:43 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-16 14:43 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-16 14:43 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:43 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-May-16 14:43 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-16 14:43 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-16 14:43 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1845 b- defN 24-May-16 14:43 nucliadb/standalone/tests/unit/test_migrations.py
+-rw-r--r--  2.0 unx     1587 b- defN 24-May-16 14:43 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-16 14:43 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-16 14:43 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-May-16 14:43 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-16 14:43 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-16 14:43 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-May-16 14:43 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-May-16 14:43 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-May-16 14:43 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-May-16 14:43 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-May-16 14:43 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-May-16 14:43 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-May-16 14:43 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-May-16 14:43 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-May-16 14:43 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-May-16 14:43 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-May-16 14:43 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-May-16 14:43 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3662 b- defN 24-May-16 14:43 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-May-16 14:43 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2780 b- defN 24-May-16 14:43 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-16 14:43 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-May-16 14:43 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-May-16 14:43 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-May-16 14:43 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3649 b- defN 24-May-16 14:43 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-16 14:43 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    12240 b- defN 24-May-16 14:43 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-May-16 14:43 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     9465 b- defN 24-May-16 14:43 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5627 b- defN 24-May-16 14:43 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:43 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3761 b- defN 24-May-16 14:43 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2136 b- defN 24-May-16 14:43 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-16 14:43 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-May-16 14:43 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-May-16 14:43 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     3093 b- defN 24-May-16 14:43 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-May-16 14:43 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-May-16 14:43 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-May-16 14:43 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-May-16 14:43 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-May-16 14:43 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-May-16 14:43 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-May-16 14:43 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-May-16 14:43 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-May-16 14:43 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-May-16 14:43 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-May-16 14:43 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-May-16 14:43 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-May-16 14:43 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-May-16 14:43 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-May-16 14:43 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-16 14:43 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-May-16 14:43 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-16 14:43 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-May-16 14:43 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-16 14:43 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-May-16 14:43 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-May-16 14:43 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-May-16 14:43 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-May-16 14:43 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-May-16 14:43 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-May-16 14:43 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-May-16 14:43 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-May-16 14:43 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-May-16 14:43 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-May-16 14:43 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1908 b- defN 24-May-16 14:43 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2135 b- defN 24-May-16 14:43 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-May-16 14:43 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-May-16 14:43 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-May-16 14:43 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-May-16 14:43 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-May-16 14:43 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-May-16 14:43 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-May-16 14:43 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-May-16 14:43 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-May-16 14:43 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-May-16 14:43 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-May-16 14:43 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-May-16 14:43 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1876 b- defN 24-May-16 14:43 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-16 14:43 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2417 b- defN 24-May-16 14:43 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-May-16 14:43 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-May-16 14:43 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-May-16 14:43 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-May-16 14:43 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-May-16 14:43 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-May-16 14:43 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-May-16 14:43 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-May-16 14:43 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-May-16 14:43 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-May-16 14:43 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-16 14:43 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-16 14:43 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-May-16 14:43 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19492 b- defN 24-May-16 14:43 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-May-16 14:43 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-May-16 14:43 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-16 14:43 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx     1448 b- defN 24-May-16 14:43 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3074 b- defN 24-May-16 14:43 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-May-16 14:43 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-May-16 14:43 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-May-16 14:43 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6571 b- defN 24-May-16 14:43 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24482 b- defN 24-May-16 14:43 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5248 b- defN 24-May-16 14:43 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-16 14:43 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18893 b- defN 24-May-16 14:43 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-16 14:43 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10747 b- defN 24-May-16 14:43 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30857 b- defN 24-May-16 14:43 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-16 14:43 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-May-16 14:43 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-May-16 14:43 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-May-16 14:43 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16319 b- defN 24-May-16 14:43 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-May-16 14:43 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx     1152 b- defN 24-May-16 14:43 nucliadb/writer/resource/slug.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-16 14:43 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-16 14:43 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-May-16 14:43 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-May-16 14:43 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25999 b- defN 24-May-16 14:43 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-May-16 14:43 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4358 b- defN 24-May-16 14:43 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16694 b- defN 24-May-16 14:43 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-May-16 14:43 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-May-16 14:43 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-16 14:43 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-May-16 14:43 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-May-16 14:43 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-May-16 14:43 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-May-16 14:43 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-May-16 14:43 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-May-16 14:43 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-May-16 14:43 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-May-16 14:43 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-May-16 14:43 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4399 b- defN 24-May-16 14:45 nucliadb-3.1.0.post509.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 14:45 nucliadb-3.1.0.post509.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-16 14:45 nucliadb-3.1.0.post509.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-May-16 14:45 nucliadb-3.1.0.post509.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-16 14:45 nucliadb-3.1.0.post509.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    43144 b- defN 24-May-16 14:45 nucliadb-3.1.0.post509.dist-info/RECORD
+460 files, 2259422 bytes uncompressed, 694384 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -1356,26 +1356,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-3.1.0.post508.dist-info/METADATA
+Filename: nucliadb-3.1.0.post509.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-3.1.0.post508.dist-info/WHEEL
+Filename: nucliadb-3.1.0.post509.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-3.1.0.post508.dist-info/entry_points.txt
+Filename: nucliadb-3.1.0.post509.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-3.1.0.post508.dist-info/top_level.txt
+Filename: nucliadb-3.1.0.post509.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-3.1.0.post508.dist-info/zip-safe
+Filename: nucliadb-3.1.0.post509.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-3.1.0.post508.dist-info/RECORD
+Filename: nucliadb-3.1.0.post509.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/common/cluster/manager.py

```diff
@@ -268,15 +268,15 @@
     async def rollback_shard(self, shard: writer_pb2.ShardObject):
         for shard_replica in shard.replicas:
             node_id = shard_replica.node
             replica_id = shard_replica.shard.id
             node = get_index_node(node_id)
             if node is not None:
                 try:
-                    logger.warning(
+                    logger.info(
                         "Deleting shard replica",
                         extra={"shard": replica_id, "node": node_id},
                     )
                     await node.delete_shard(replica_id)
                 except Exception as rollback_error:
                     errors.capture_exception(rollback_error)
                     logger.error(
@@ -373,15 +373,15 @@
         self,
         kbid: str,
         num_paragraphs: int,
     ):
         if not self.should_create_new_shard(num_paragraphs):
             return
 
-        logger.warning({"message": "Adding shard", "kbid": kbid})
+        logger.info({"message": "Adding shard", "kbid": kbid})
 
         async with datamanagers.with_transaction() as txn:
             await self.create_shard_by_kbid(txn, kbid)
             await txn.commit()
 
 
 class StandaloneKBShardManager(KBShardManager):
```

## nucliadb/common/cluster/rebalance.py

```diff
@@ -91,15 +91,15 @@
         kb_shards = await datamanagers.cluster.get_kb_shards(txn, kbid=kbid)
     if kb_shards is None:  # pragma: no cover
         logger.warning(
             "No shards found for kb. This should not happen.", extra={"kbid": kbid}
         )
         return
 
-    logger.warning(
+    logger.info(
         "Rebalancing kb shards",
         extra={"kbid": kbid, "from": from_shard_id, "to": to_shard_id, "count": count},
     )
 
     from_shard = [s for s in kb_shards.shards if s.shard == from_shard_id][0]
     to_shard = [s for s in kb_shards.shards if s.shard == to_shard_id][0]
```

## nucliadb/common/cluster/utils.py

```diff
@@ -155,16 +155,14 @@
 
 async def delete_resource_from_shard(
     app_context: ApplicationContext,
     kbid: str,
     resource_id: str,
     shard: writer_pb2.ShardObject,
 ) -> None:
-    logger.warning(
-        "Deleting resource", extra={"kbid": kbid, "resource_id": resource_id}
-    )
+    logger.info("Deleting resource", extra={"kbid": kbid, "resource_id": resource_id})
 
     sm = app_context.shard_manager
     partitioning = app_context.partitioning
     partition = partitioning.generate_partition(kbid, resource_id)
 
     await sm.delete_resource(shard, resource_id, 0, str(partition), kbid)
```

## nucliadb/common/cluster/discovery/k8s.py

```diff
@@ -133,15 +133,15 @@
                     },
                 )
                 raise
 
         if ready:
             node = manager.get_index_node(node_data.node_id)
             if node is None:
-                logger.warning(
+                logger.info(
                     "Adding node",
                     extra={
                         "node_id": node_data.node_id,
                         "pod_name": pod_name,
                         "address": node_data.address,
                     },
                 )
```

## nucliadb/ingest/orm/processor/__init__.py

```diff
@@ -238,15 +238,15 @@
     ) -> None:
         if len(messages) == 0:
             return None
 
         txn = await self.driver.begin()
         kbid = messages[0].kbid
         if not await datamanagers.kb.exists_kb(txn, kbid=kbid):
-            logger.warning(f"KB {kbid} is deleted: skiping txn")
+            logger.info(f"KB {kbid} is deleted: skiping txn")
             if transaction_check:
                 await sequence_manager.set_last_seqid(txn, partition, seqid)
             await txn.commit()
             return None
 
         try:
             multi = messages[0].multiid
```

## nucliadb/ingest/service/writer.py

```diff
@@ -150,15 +150,15 @@
     async def NewKnowledgeBox(  # type: ignore
         self, request: KnowledgeBoxNew, context=None
     ) -> NewKnowledgeBoxResponse:
         try:
             kbid = await self.create_kb(request)
             logger.info("KB created successfully", extra={"kbid": kbid})
         except KnowledgeBoxConflict:
-            logger.warning("KB already exists", extra={"slug": request.slug})
+            logger.info("KB already exists", extra={"slug": request.slug})
             return NewKnowledgeBoxResponse(status=KnowledgeBoxResponseStatus.CONFLICT)
         except Exception as exc:
             errors.capture_exception(exc)
             logger.exception(
                 "Unexpected error creating KB",
                 exc_info=True,
                 extra={"slug": request.slug},
```

## nucliadb/migrator/migrator.py

```diff
@@ -54,20 +54,20 @@
             migration_info = {
                 "from_version": kb_info.current_version,
                 "to_version": migration.version,
                 "kbid": kbid,
             }
 
             try:
-                logger.warning("Migrating KB", extra=migration_info)
+                logger.info("Migrating KB", extra=migration_info)
                 with migration_observer(
                     {"type": "kb", "target_version": str(migration.version)}
                 ):
                     await migration.module.migrate_kb(context, kbid)  # type: ignore
-                logger.warning("Finished KB Migration", extra=migration_info)
+                logger.info("Finished KB Migration", extra=migration_info)
                 await context.data_manager.update_kb_info(
                     kbid=kbid, current_version=migration.version
                 )
             except Exception as exc:
                 errors.capture_exception(exc)
                 logger.exception("Failed to migrate KB", extra=migration_info)
                 raise
@@ -149,23 +149,23 @@
     migrations = get_migrations(global_info.current_version, to_version=target_version)
     for migration in migrations:
         migration_info = {
             "from_version": global_info.current_version,
             "to_version": migration.version,
         }
         try:
-            logger.warning("Migrating", extra=migration_info)
+            logger.info("Migrating", extra=migration_info)
             with migration_observer(
                 {"type": "global", "target_version": str(migration.version)}
             ):
                 await migration.module.migrate(context)  # type: ignore
             await context.data_manager.update_global_info(
                 current_version=migration.version
             )
-            logger.warning("Finished migration", extra=migration_info)
+            logger.info("Finished migration", extra=migration_info)
         except Exception as exc:
             errors.capture_exception(exc)
             logger.exception("Failed to migrate", extra=migration_info)
             raise
 
     await context.data_manager.update_global_info(target_version=None)
```

## nucliadb/writer/back_pressure.py

```diff
@@ -111,15 +111,15 @@
     data: Optional[BackPressureData] = _cache.get(cache_key)
     if data is not None:
         try_after = data.try_after
         back_pressure_type = data.type
         RATE_LIMITED_REQUESTS_COUNTER.inc(
             {"type": back_pressure_type, "cached": "true"}
         )
-        logger.warning(
+        logger.info(
             "Back pressure applied from cache",
             extra={
                 "type": back_pressure_type,
                 "try_after": try_after,
                 "kbid": kbid,
                 "resource_uuid": resource_uuid,
             },
```

## Comparing `nucliadb-3.1.0.post508.dist-info/METADATA` & `nucliadb-3.1.0.post509.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 3.1.0.post508
+Version: 3.1.0.post509
 Home-page: https://docs.nuclia.dev/docs/guides/nucliadb/intro
 Author: NucliaDB Community
 Author-email: nucliadb@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
@@ -17,18 +17,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
-Requires-Dist: nucliadb-telemetry[all] >=3.1.0.post508
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.1.0.post508
-Requires-Dist: nucliadb-protos >=3.1.0.post508
-Requires-Dist: nucliadb-models >=3.1.0.post508
+Requires-Dist: nucliadb-telemetry[all] >=3.1.0.post509
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=3.1.0.post509
+Requires-Dist: nucliadb-protos >=3.1.0.post509
+Requires-Dist: nucliadb-models >=3.1.0.post509
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: pydantic-argparse
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-3.1.0.post508.dist-info/entry_points.txt` & `nucliadb-3.1.0.post509.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-3.1.0.post508.dist-info/RECORD` & `nucliadb-3.1.0.post509.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -27,22 +27,22 @@
 nucliadb/common/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/locking.py,sha256=M9ODhLZUfCyrtx3qaCE7282L2Nkga1mcFUsXhh0cV50,5022
 nucliadb/common/cluster/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/cluster/base.py,sha256=z_JD-xNVPB6-6O_u8YMpyOPP3fRmimwq7LbA3EGqDnE,4971
 nucliadb/common/cluster/exceptions.py,sha256=V3c_fgH00GyJ-a5CaGLhwTuhwhUNR9YAGvS5jaRuc_Y,1495
 nucliadb/common/cluster/grpc_node_dummy.py,sha256=rqco9bKGw77ssbKCakURWm5oGD4J0huEO5c30tvcA7Q,3793
 nucliadb/common/cluster/index_node.py,sha256=WafWLzU1l7EHj1VyG0w6qi2BW_Izc8rFze6ZWbYvT9g,3429
-nucliadb/common/cluster/manager.py,sha256=VnBVZk6bYxstfKDLlgwsKZVpfLw_QNVlPDcAoh1njbw,22097
-nucliadb/common/cluster/rebalance.py,sha256=o2LEvVUUHA30QW7ei4HtbXxL1RraMrrZoUB3qSYl8WI,8593
+nucliadb/common/cluster/manager.py,sha256=FgUYnPaMv2Ts9lUvzpl87wk-Otp6Hd_2Q8H7tYtPv1E,22091
+nucliadb/common/cluster/rebalance.py,sha256=BzPsMMbndal7B0DAZbET0kb27ITM6p3NogjBaKBHAR4,8590
 nucliadb/common/cluster/rollover.py,sha256=okF5Y-b-s-thk6cbTI-86wrB32jZ-NE2JwwI2D-RtRM,20209
 nucliadb/common/cluster/settings.py,sha256=JX6wgWN8A2C9nnkoEmBE5YXa6cWeE28spFKz1y7YqbE,2992
-nucliadb/common/cluster/utils.py,sha256=byi2bIHb6K2sCJfoqs0bwQHRfxSnnjVs1dowoX5Two8,5730
+nucliadb/common/cluster/utils.py,sha256=15dQBg4XKmdD5iOZsOwU7YGx01h84HRZIWv48EtaUOE,5713
 nucliadb/common/cluster/discovery/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/common/cluster/discovery/base.py,sha256=P0JwzRYqOKxOzV_K_glwPizDGFGBY-l8G7TeTId9LIA,6553
-nucliadb/common/cluster/discovery/k8s.py,sha256=pvuyIYuWWDpRz7Bv8D_LOKFMz0w8sucpJvDshmRNpe0,12518
+nucliadb/common/cluster/discovery/k8s.py,sha256=XSCxEGB_emdVgdN7ABCxth2vw8kgSNljhfFutDO0d20,12515
 nucliadb/common/cluster/discovery/manual.py,sha256=7wdcyfrR8oii2hP3AzOTAaUAGwkQu7eOj9Xl7Q49IUQ,1957
 nucliadb/common/cluster/discovery/single.py,sha256=2BhcencPKQQIfVitmTPJZm3TkBHyY9ZMcr-Clh8k2tM,1737
 nucliadb/common/cluster/discovery/types.py,sha256=vs-K790rofjZ4FWYaMkgjkZZqMvIvd_0eSw3shuiLwA,1139
 nucliadb/common/cluster/discovery/utils.py,sha256=A3DhpM3ExTSxtIo0Wh8ZIFARq2GW2OM1GPX967gyRbk,2548
 nucliadb/common/cluster/standalone/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/common/cluster/standalone/grpc_node_binding.py,sha256=52U0TCREO4CcCOC9ctrxmx6xno2M8t01QbI8MIcw3Qc,13707
 nucliadb/common/cluster/standalone/index_node.py,sha256=aKpkAEosp9qbd-77fYgE1AAnDc-6ER05cA_HJtkeBT0,4683
@@ -115,19 +115,19 @@
 nucliadb/ingest/orm/entities.py,sha256=q027LfocE-KIqRNC1ZOSrrvt6x9NGrB25TZsOe0SyVk,15758
 nucliadb/ingest/orm/exceptions.py,sha256=GKr20V5xLv-WHBBHhr8lBChpW5oa9k18Xuiw-dIF9DM,1279
 nucliadb/ingest/orm/knowledgebox.py,sha256=urKMAL8Rj0Unen5AZ4Au-Z-176Vk1mOiXTUF4PnqMMs,17167
 nucliadb/ingest/orm/metrics.py,sha256=OkwMSPKLZcKba0ZTwtTiIxwBgaLMX5ydhGieKvi2y7E,1096
 nucliadb/ingest/orm/resource.py,sha256=gmmVw8tkAcH8oYQdfuxSrRhD8KZ4mh0oPs3SML2RGtY,60444
 nucliadb/ingest/orm/synonyms.py,sha256=tyOEGPfuJwhM5iYm4uNPjc2E8oWPk70DzZeuxVZ5alQ,1739
 nucliadb/ingest/orm/utils.py,sha256=0GwmyP0CqskAUqKbp0LAInYE64kt8locVqZ0HB04zlw,3683
-nucliadb/ingest/orm/processor/__init__.py,sha256=YHtFQfYiw-VCgHoiElIGGXnuEoTwJCxehC2eTrQCeHQ,26423
+nucliadb/ingest/orm/processor/__init__.py,sha256=5B2o6MFFX3vRpLOxk2X6xWMpKZYKzudJc04Xf5D4DVI,26420
 nucliadb/ingest/orm/processor/sequence_manager.py,sha256=Mc9SA_NfzxTwovD5yGiAcdmen4pa-QNdsYcONIWeZPc,1690
 nucliadb/ingest/service/__init__.py,sha256=C_lkkjoHm0hDT2fZjEN4mpwXtU4bWthB-vM5-28-MBM,2057
 nucliadb/ingest/service/exceptions.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
-nucliadb/ingest/service/writer.py,sha256=FL44FUPdXWXrfYiRZRnW7x43o5BFB2JQaWmlCQfUT_A,33196
+nucliadb/ingest/service/writer.py,sha256=WCdV-EK4WBEbNS7RPGkj0Kp0txW7MEVRc2lSyKUg7Ls,33193
 nucliadb/ingest/tests/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/conftest.py,sha256=yTepuxodMXl5vEMTzFfgos9wdRnYfxPffZQDYm3Ej-E,1157
 nucliadb/ingest/tests/fixtures.py,sha256=L4HeWexZwgpzPl872er2sAisfrW0OdmgOvx7SzCDrWM,24060
 nucliadb/ingest/tests/vectors.py,sha256=CcNKx-E8LPpyvRyljbmb-Tn_wST9Juw2CBoogWrKiTk,62843
 nucliadb/ingest/tests/integration/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/tests/integration/consumer/__init__.py,sha256=itSI7dtTwFP55YMX4iK7JzdMHS5CQVUiB1XzQu4UBh8,833
 nucliadb/ingest/tests/integration/consumer/test_auditing.py,sha256=5VYFGUeaxd18mLtUfHCUPu9c1iAShNHNM5X_CSkIFSs,2549
@@ -159,15 +159,15 @@
 nucliadb/middleware/__init__.py,sha256=knHBrVD30vfAWxn1RdRYEloSpIqakY3Ch9-NQzqKxk4,2216
 nucliadb/middleware/transaction.py,sha256=BjLGePAUnGAtpYIfv9lXKRFI1fB6lrseVeYzY-ckiFY,3912
 nucliadb/migrator/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/migrator/command.py,sha256=MgDruKOYpLuUMoO8aAE86vPflfOt7pAbW8QZQSZTFQQ,2119
 nucliadb/migrator/context.py,sha256=3h6M_AG2HFjTYtQC2XDmKps7wywdUduT1RM3C30S_S0,1334
 nucliadb/migrator/datamanager.py,sha256=5CLt1_fA3hXCBwUr1ltfmN3o69AzbweyiP42FkOqqV0,5104
 nucliadb/migrator/exceptions.py,sha256=jTj3YhKmFwUyjjgoKUNoCAiGrpEbB64X1Um212nSNQ8,889
-nucliadb/migrator/migrator.py,sha256=4XyjqhoiG4hPoC8I3-07AlWQKYCEyo6oIx0demvAl-U,9382
+nucliadb/migrator/migrator.py,sha256=HoxeJWzRK21yzTfowS72USJDCIe2SnVRS66TV_hSvHs,9370
 nucliadb/migrator/models.py,sha256=3PJkL2PGvKgIG0KIBv4H5XCsOVmwWMlRV3m0ntDj10Q,1145
 nucliadb/migrator/settings.py,sha256=_by-e5oYmaX4ZTOIQl4dJufJDv78fuUMwIj9RTe1APs,1110
 nucliadb/migrator/utils.py,sha256=7Y2zJZWB2qM0PcmS5G20g5EEwSdRVeHyR4_1wWNbl6Q,2346
 nucliadb/models/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/models/responses.py,sha256=qnuOoc7TrVSUnpikfTwHLKez47_DE4mSFzpxrwtqijA,1599
 nucliadb/purge/__init__.py,sha256=IHnoGcbASPUQ74ewbPtHiOnUbRXfB92-aDH4sUYALTQ,6041
 nucliadb/purge/orphan_shards.py,sha256=tGFlF7-RLDHv2XPc5J_1lgBvBCM5UjUtUNUmpodGqBc,9364
@@ -402,15 +402,15 @@
 nucliadb/train/tests/test_paragraph_streaming.py,sha256=CMwGEDBQ3iwf7pldZfOBphFSYCvTLKPd1dDHgoHtslQ,4320
 nucliadb/train/tests/test_question_answer_streaming.py,sha256=URtFXd6sEy72Q1By5LtcwIPT5S_yQ0Ip8AjJPILUeDU,8751
 nucliadb/train/tests/test_sentence_classification.py,sha256=6cex9xJN1AGZhsVD1jG2JKYgZEmo09picNJkUrLjDDQ,5051
 nucliadb/train/tests/test_token_classification.py,sha256=fBS70sCKFWBjcaUDny9fg8qZgsQ5VtKBTPENFTgkHrk,5583
 nucliadb/train/tests/utils.py,sha256=J5UZoCz4Ss5b6SmZuyC7jJQlomQE8mDQ8E2OdYEV-gA,3324
 nucliadb/writer/__init__.py,sha256=HkfMuQR3CbbPU3g-A85Ibt8iwSTTADhLc0-pi3F3hvk,1328
 nucliadb/writer/app.py,sha256=Q55CmGR85wG5pjf_Ro-73QVWc7_wMpIt69xJSZ0kjCQ,4268
-nucliadb/writer/back_pressure.py,sha256=DPNeBVNQuRZzOEBMDmRIoeLDEuvRwwIGFBKNOQg3-xE,19495
+nucliadb/writer/back_pressure.py,sha256=5_9ScVZvIHj2VU4eur8_Frz4C__fst3MSj8mdZSnKXw,19492
 nucliadb/writer/exceptions.py,sha256=2dMvuoF68v3BZuyzaBEsbG6gusQqwLFcn47qm1zNdTc,972
 nucliadb/writer/lifecycle.py,sha256=gF9it0w98uBGCwzjs72e8mGi6H-qv_XAa2GGNBTOEDY,1953
 nucliadb/writer/openapi.py,sha256=thqCO1ht_RJgOkXs-aIsv8aXJrU5z8wo2n05l2_LqMs,1032
 nucliadb/writer/run.py,sha256=euVZ_rtHDXs-O1kB-Pt1Id8eft9CYVpWH3zJzEoEqls,1448
 nucliadb/writer/settings.py,sha256=A1JY7pFQzLPV0Vm0TSG6jPBR3dEMK76SknbeANTG4Hg,3074
 nucliadb/writer/utilities.py,sha256=AZ5qEny1Xm0IDsFtH13oJa2usvJZK8f0FdgF1LrnLCw,1036
 nucliadb/writer/api/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
@@ -448,13 +448,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-3.1.0.post508.dist-info/METADATA,sha256=sM5FqP3Qu1WE-xACosnuaBfSpcpPlxVcirL37iKEGTI,4399
-nucliadb-3.1.0.post508.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-3.1.0.post508.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-3.1.0.post508.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-3.1.0.post508.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-3.1.0.post508.dist-info/RECORD,,
+nucliadb-3.1.0.post509.dist-info/METADATA,sha256=gU5bPLX7hvpPVxyVQFUkDJnvVspmfsZwtGCn67rX9j4,4399
+nucliadb-3.1.0.post509.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-3.1.0.post509.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-3.1.0.post509.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-3.1.0.post509.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-3.1.0.post509.dist-info/RECORD,,
```

