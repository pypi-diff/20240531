# Comparing `tmp/nucliadb-4.0.3.post560-py3-none-any.whl.zip` & `tmp/nucliadb-4.0.3.post561-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,473 +1,473 @@
-Zip file size: 771442 bytes, number of entries: 471
--rw-r--r--  2.0 unx     1135 b- defN 24-May-30 10:07 migrations/0001_bootstrap.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-30 10:07 migrations/0002_rollover_shards.py
--rw-r--r--  2.0 unx     2436 b- defN 24-May-30 10:07 migrations/0003_allfields_key.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-30 10:07 migrations/0004_rollover_shards.py
--rw-r--r--  2.0 unx     1177 b- defN 24-May-30 10:07 migrations/0005_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-30 10:07 migrations/0006_rollover_shards.py
--rw-r--r--  2.0 unx     1301 b- defN 24-May-30 10:07 migrations/0008_cleanup_leftover_rollover_metadata.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-30 10:07 migrations/0009_upgrade_relations_and_texts_to_v2.py
--rw-r--r--  2.0 unx     1610 b- defN 24-May-30 10:07 migrations/0010_fix_corrupt_indexes.py
--rw-r--r--  2.0 unx     1843 b- defN 24-May-30 10:07 migrations/0011_materialize_labelset_ids.py
--rw-r--r--  2.0 unx     1443 b- defN 24-May-30 10:07 migrations/0012_rollover_shards.py
--rw-r--r--  2.0 unx     1024 b- defN 24-May-30 10:07 migrations/0013_rollover_shards.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-30 10:07 migrations/0014_rollover_shards.py
--rw-r--r--  2.0 unx     1462 b- defN 24-May-30 10:07 migrations/0015_targeted_rollover.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-30 10:07 migrations/0016_upgrade_to_paragraphs_v2.py
--rw-r--r--  2.0 unx     2100 b- defN 24-May-30 10:07 migrations/0017_multiple_writable_shards.py
--rw-r--r--  2.0 unx     2264 b- defN 24-May-30 10:07 migrations/0018_purge_orphan_kbslugs.py
--rw-r--r--  2.0 unx     2506 b- defN 24-May-30 10:07 migrations/0019_upgrade_to_paragraphs_v3.py
--rw-r--r--  2.0 unx     3282 b- defN 24-May-30 10:07 migrations/0020_drain_nodes_from_cluster.py
--rw-r--r--  2.0 unx     1734 b- defN 24-May-30 10:07 migrations/0021_overwrite_vectorsets_key.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 migrations/__init__.py
--rw-r--r--  2.0 unx      891 b- defN 24-May-30 10:07 nucliadb/__init__.py
--rw-r--r--  2.0 unx     3733 b- defN 24-May-30 10:07 nucliadb/health.py
--rw-r--r--  2.0 unx    11793 b- defN 24-May-30 10:07 nucliadb/learning_proxy.py
--rw-r--r--  2.0 unx     4806 b- defN 24-May-30 10:07 nucliadb/metrics_exporter.py
--rw-r--r--  2.0 unx     2272 b- defN 24-May-30 10:07 nucliadb/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-30 10:07 nucliadb/py.typed
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/common/__init__.py
--rw-r--r--  2.0 unx     5175 b- defN 24-May-30 10:07 nucliadb/common/locking.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/common/cluster/__init__.py
--rw-r--r--  2.0 unx     5134 b- defN 24-May-30 10:07 nucliadb/common/cluster/base.py
--rw-r--r--  2.0 unx     1495 b- defN 24-May-30 10:07 nucliadb/common/cluster/exceptions.py
--rw-r--r--  2.0 unx     3793 b- defN 24-May-30 10:07 nucliadb/common/cluster/grpc_node_dummy.py
--rw-r--r--  2.0 unx     3429 b- defN 24-May-30 10:07 nucliadb/common/cluster/index_node.py
--rw-r--r--  2.0 unx    24815 b- defN 24-May-30 10:07 nucliadb/common/cluster/manager.py
--rw-r--r--  2.0 unx     8853 b- defN 24-May-30 10:07 nucliadb/common/cluster/rebalance.py
--rw-r--r--  2.0 unx    20532 b- defN 24-May-30 10:07 nucliadb/common/cluster/rollover.py
--rw-r--r--  2.0 unx     3016 b- defN 24-May-30 10:07 nucliadb/common/cluster/settings.py
--rw-r--r--  2.0 unx     5713 b- defN 24-May-30 10:07 nucliadb/common/cluster/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     6553 b- defN 24-May-30 10:07 nucliadb/common/cluster/discovery/base.py
--rw-r--r--  2.0 unx    12512 b- defN 24-May-30 10:07 nucliadb/common/cluster/discovery/k8s.py
--rw-r--r--  2.0 unx     1957 b- defN 24-May-30 10:07 nucliadb/common/cluster/discovery/manual.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-30 10:07 nucliadb/common/cluster/discovery/single.py
--rw-r--r--  2.0 unx     1139 b- defN 24-May-30 10:07 nucliadb/common/cluster/discovery/types.py
--rw-r--r--  2.0 unx     2548 b- defN 24-May-30 10:07 nucliadb/common/cluster/discovery/utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-30 10:07 nucliadb/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx    13712 b- defN 24-May-30 10:07 nucliadb/common/cluster/standalone/grpc_node_binding.py
--rw-r--r--  2.0 unx     4683 b- defN 24-May-30 10:07 nucliadb/common/cluster/standalone/index_node.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-30 10:07 nucliadb/common/cluster/standalone/service.py
--rw-r--r--  2.0 unx     3545 b- defN 24-May-30 10:07 nucliadb/common/cluster/standalone/utils.py
--rw-r--r--  2.0 unx     3440 b- defN 24-May-30 10:07 nucliadb/common/context/__init__.py
--rw-r--r--  2.0 unx     1628 b- defN 24-May-30 10:07 nucliadb/common/context/fastapi.py
--rw-r--r--  2.0 unx     1940 b- defN 24-May-30 10:07 nucliadb/common/datamanagers/__init__.py
--rw-r--r--  2.0 unx     2648 b- defN 24-May-30 10:07 nucliadb/common/datamanagers/atomic.py
--rw-r--r--  2.0 unx     1451 b- defN 24-May-30 10:07 nucliadb/common/datamanagers/cluster.py
--rw-r--r--  2.0 unx     5383 b- defN 24-May-30 10:07 nucliadb/common/datamanagers/entities.py
--rw-r--r--  2.0 unx      883 b- defN 24-May-30 10:07 nucliadb/common/datamanagers/exceptions.py
--rw-r--r--  2.0 unx     3994 b- defN 24-May-30 10:07 nucliadb/common/datamanagers/kb.py
--rw-r--r--  2.0 unx     5389 b- defN 24-May-30 10:07 nucliadb/common/datamanagers/labels.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-30 10:07 nucliadb/common/datamanagers/processing.py
--rw-r--r--  2.0 unx    12177 b- defN 24-May-30 10:07 nucliadb/common/datamanagers/resources.py
--rw-r--r--  2.0 unx     5634 b- defN 24-May-30 10:07 nucliadb/common/datamanagers/rollover.py
--rw-r--r--  2.0 unx     1548 b- defN 24-May-30 10:07 nucliadb/common/datamanagers/synonyms.py
--rw-r--r--  2.0 unx     1631 b- defN 24-May-30 10:07 nucliadb/common/datamanagers/utils.py
--rw-r--r--  2.0 unx     3780 b- defN 24-May-30 10:07 nucliadb/common/datamanagers/vectorsets.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/common/http_clients/__init__.py
--rw-r--r--  2.0 unx     2146 b- defN 24-May-30 10:07 nucliadb/common/http_clients/auth.py
--rw-r--r--  2.0 unx     1100 b- defN 24-May-30 10:07 nucliadb/common/http_clients/exceptions.py
--rw-r--r--  2.0 unx     7155 b- defN 24-May-30 10:07 nucliadb/common/http_clients/processing.py
--rw-r--r--  2.0 unx     1540 b- defN 24-May-30 10:07 nucliadb/common/http_clients/pypi.py
--rw-r--r--  2.0 unx     1551 b- defN 24-May-30 10:07 nucliadb/common/http_clients/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3449 b- defN 24-May-30 10:07 nucliadb/common/maindb/driver.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-30 10:07 nucliadb/common/maindb/exceptions.py
--rw-r--r--  2.0 unx     6769 b- defN 24-May-30 10:07 nucliadb/common/maindb/local.py
--rw-r--r--  2.0 unx     8391 b- defN 24-May-30 10:07 nucliadb/common/maindb/pg.py
--rw-r--r--  2.0 unx     6053 b- defN 24-May-30 10:07 nucliadb/common/maindb/redis.py
--rw-r--r--  2.0 unx    15314 b- defN 24-May-30 10:07 nucliadb/common/maindb/tikv.py
--rw-r--r--  2.0 unx     4167 b- defN 24-May-30 10:07 nucliadb/common/maindb/utils.py
--rw-r--r--  2.0 unx      932 b- defN 24-May-30 10:07 nucliadb/export_import/__init__.py
--rw-r--r--  2.0 unx     6171 b- defN 24-May-30 10:07 nucliadb/export_import/datamanager.py
--rw-r--r--  2.0 unx     1949 b- defN 24-May-30 10:07 nucliadb/export_import/exceptions.py
--rw-r--r--  2.0 unx     7116 b- defN 24-May-30 10:07 nucliadb/export_import/exporter.py
--rw-r--r--  2.0 unx     4258 b- defN 24-May-30 10:07 nucliadb/export_import/importer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-30 10:07 nucliadb/export_import/models.py
--rw-r--r--  2.0 unx     2571 b- defN 24-May-30 10:07 nucliadb/export_import/tasks.py
--rw-r--r--  2.0 unx    19401 b- defN 24-May-30 10:07 nucliadb/export_import/utils.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-30 10:07 nucliadb/ingest/__init__.py
--rw-r--r--  2.0 unx     7277 b- defN 24-May-30 10:07 nucliadb/ingest/app.py
--rw-r--r--  2.0 unx     1005 b- defN 24-May-30 10:07 nucliadb/ingest/cache.py
--rw-r--r--  2.0 unx     2484 b- defN 24-May-30 10:07 nucliadb/ingest/partitions.py
--rw-r--r--  2.0 unx    19904 b- defN 24-May-30 10:07 nucliadb/ingest/processing.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-30 10:07 nucliadb/ingest/py.typed
--rw-r--r--  2.0 unx    20277 b- defN 24-May-30 10:07 nucliadb/ingest/serialize.py
--rw-r--r--  2.0 unx     3207 b- defN 24-May-30 10:07 nucliadb/ingest/settings.py
--rw-r--r--  2.0 unx     2314 b- defN 24-May-30 10:07 nucliadb/ingest/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/ingest/consumer/__init__.py
--rw-r--r--  2.0 unx     6918 b- defN 24-May-30 10:07 nucliadb/ingest/consumer/auditing.py
--rw-r--r--  2.0 unx    12174 b- defN 24-May-30 10:07 nucliadb/ingest/consumer/consumer.py
--rw-r--r--  2.0 unx     3945 b- defN 24-May-30 10:07 nucliadb/ingest/consumer/materializer.py
--rw-r--r--  2.0 unx     1075 b- defN 24-May-30 10:07 nucliadb/ingest/consumer/metrics.py
--rw-r--r--  2.0 unx     9543 b- defN 24-May-30 10:07 nucliadb/ingest/consumer/pull.py
--rw-r--r--  2.0 unx     6871 b- defN 24-May-30 10:07 nucliadb/ingest/consumer/service.py
--rw-r--r--  2.0 unx     4331 b- defN 24-May-30 10:07 nucliadb/ingest/consumer/shard_creator.py
--rw-r--r--  2.0 unx     2656 b- defN 24-May-30 10:07 nucliadb/ingest/consumer/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/ingest/fields/__init__.py
--rw-r--r--  2.0 unx    17461 b- defN 24-May-30 10:07 nucliadb/ingest/fields/base.py
--rw-r--r--  2.0 unx     6516 b- defN 24-May-30 10:07 nucliadb/ingest/fields/conversation.py
--rw-r--r--  2.0 unx     1223 b- defN 24-May-30 10:07 nucliadb/ingest/fields/date.py
--rw-r--r--  2.0 unx     1205 b- defN 24-May-30 10:07 nucliadb/ingest/fields/exceptions.py
--rw-r--r--  2.0 unx     4840 b- defN 24-May-30 10:07 nucliadb/ingest/fields/file.py
--rw-r--r--  2.0 unx     1547 b- defN 24-May-30 10:07 nucliadb/ingest/fields/generic.py
--rw-r--r--  2.0 unx     1235 b- defN 24-May-30 10:07 nucliadb/ingest/fields/keywordset.py
--rw-r--r--  2.0 unx     2250 b- defN 24-May-30 10:07 nucliadb/ingest/fields/layout.py
--rw-r--r--  2.0 unx     4212 b- defN 24-May-30 10:07 nucliadb/ingest/fields/link.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-30 10:07 nucliadb/ingest/fields/text.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/ingest/orm/__init__.py
--rw-r--r--  2.0 unx    28311 b- defN 24-May-30 10:07 nucliadb/ingest/orm/brain.py
--rw-r--r--  2.0 unx    15758 b- defN 24-May-30 10:07 nucliadb/ingest/orm/entities.py
--rw-r--r--  2.0 unx     1326 b- defN 24-May-30 10:07 nucliadb/ingest/orm/exceptions.py
--rw-r--r--  2.0 unx    16750 b- defN 24-May-30 10:07 nucliadb/ingest/orm/knowledgebox.py
--rw-r--r--  2.0 unx     1096 b- defN 24-May-30 10:07 nucliadb/ingest/orm/metrics.py
--rw-r--r--  2.0 unx    58955 b- defN 24-May-30 10:07 nucliadb/ingest/orm/resource.py
--rw-r--r--  2.0 unx     2685 b- defN 24-May-30 10:07 nucliadb/ingest/orm/utils.py
--rw-r--r--  2.0 unx    27092 b- defN 24-May-30 10:07 nucliadb/ingest/orm/processor/__init__.py
--rw-r--r--  2.0 unx     5090 b- defN 24-May-30 10:07 nucliadb/ingest/orm/processor/auditing.py
--rw-r--r--  2.0 unx     1690 b- defN 24-May-30 10:07 nucliadb/ingest/orm/processor/sequence_manager.py
--rw-r--r--  2.0 unx     2057 b- defN 24-May-30 10:07 nucliadb/ingest/service/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/ingest/service/exceptions.py
--rw-r--r--  2.0 unx    32813 b- defN 24-May-30 10:07 nucliadb/ingest/service/writer.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/ingest/tests/__init__.py
--rw-r--r--  2.0 unx     1157 b- defN 24-May-30 10:07 nucliadb/ingest/tests/conftest.py
--rw-r--r--  2.0 unx    24111 b- defN 24-May-30 10:07 nucliadb/ingest/tests/fixtures.py
--rw-r--r--  2.0 unx    62843 b- defN 24-May-30 10:07 nucliadb/ingest/tests/vectors.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/ingest/tests/integration/__init__.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-30 10:07 nucliadb/ingest/tests/integration/consumer/__init__.py
--rw-r--r--  2.0 unx     2500 b- defN 24-May-30 10:07 nucliadb/ingest/tests/integration/consumer/test_auditing.py
--rw-r--r--  2.0 unx     3836 b- defN 24-May-30 10:07 nucliadb/ingest/tests/integration/consumer/test_materializer.py
--rw-r--r--  2.0 unx     4470 b- defN 24-May-30 10:07 nucliadb/ingest/tests/integration/consumer/test_pull.py
--rw-r--r--  2.0 unx     2763 b- defN 24-May-30 10:07 nucliadb/ingest/tests/integration/consumer/test_service.py
--rw-r--r--  2.0 unx     2019 b- defN 24-May-30 10:07 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/ingest/tests/integration/ingest/__init__.py
--rw-r--r--  2.0 unx    27247 b- defN 24-May-30 10:07 nucliadb/ingest/tests/integration/ingest/test_ingest.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-30 10:07 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-30 10:07 nucliadb/ingest/tests/integration/ingest/test_relations.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1189 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/test_cache.py
--rw-r--r--  2.0 unx     1432 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/test_partitions.py
--rw-r--r--  2.0 unx     5807 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/test_processing.py
--rw-r--r--  2.0 unx      978 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/test_settings.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/consumer/__init__.py
--rw-r--r--  2.0 unx     3885 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/consumer/test_auditing.py
--rw-r--r--  2.0 unx     2472 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/consumer/test_consumer.py
--rw-r--r--  2.0 unx     2063 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/consumer/test_pull.py
--rw-r--r--  2.0 unx     4140 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/consumer/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/orm/__init__.py
--rw-r--r--  2.0 unx     9876 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/orm/test_brain.py
--rw-r--r--  2.0 unx     2435 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
--rw-r--r--  2.0 unx     1174 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
--rw-r--r--  2.0 unx     4045 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/orm/test_processor.py
--rw-r--r--  2.0 unx    11033 b- defN 24-May-30 10:07 nucliadb/ingest/tests/unit/orm/test_resource.py
--rw-r--r--  2.0 unx     2216 b- defN 24-May-30 10:07 nucliadb/middleware/__init__.py
--rw-r--r--  2.0 unx     3912 b- defN 24-May-30 10:07 nucliadb/middleware/transaction.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/migrator/__init__.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-30 10:07 nucliadb/migrator/command.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-30 10:07 nucliadb/migrator/context.py
--rw-r--r--  2.0 unx     5104 b- defN 24-May-30 10:07 nucliadb/migrator/datamanager.py
--rw-r--r--  2.0 unx      889 b- defN 24-May-30 10:07 nucliadb/migrator/exceptions.py
--rw-r--r--  2.0 unx     9370 b- defN 24-May-30 10:07 nucliadb/migrator/migrator.py
--rw-r--r--  2.0 unx     1145 b- defN 24-May-30 10:07 nucliadb/migrator/models.py
--rw-r--r--  2.0 unx     1144 b- defN 24-May-30 10:07 nucliadb/migrator/settings.py
--rw-r--r--  2.0 unx     2346 b- defN 24-May-30 10:07 nucliadb/migrator/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/models/__init__.py
--rw-r--r--  2.0 unx     1599 b- defN 24-May-30 10:07 nucliadb/models/responses.py
--rw-r--r--  2.0 unx     6041 b- defN 24-May-30 10:07 nucliadb/purge/__init__.py
--rw-r--r--  2.0 unx     9364 b- defN 24-May-30 10:07 nucliadb/purge/orphan_shards.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-30 10:07 nucliadb/reader/__init__.py
--rw-r--r--  2.0 unx     3709 b- defN 24-May-30 10:07 nucliadb/reader/app.py
--rw-r--r--  2.0 unx     1366 b- defN 24-May-30 10:07 nucliadb/reader/lifecycle.py
--rw-r--r--  2.0 unx     1031 b- defN 24-May-30 10:07 nucliadb/reader/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-30 10:07 nucliadb/reader/py.typed
--rw-r--r--  2.0 unx     1447 b- defN 24-May-30 10:07 nucliadb/reader/run.py
--rw-r--r--  2.0 unx      872 b- defN 24-May-30 10:07 nucliadb/reader/api/__init__.py
--rw-r--r--  2.0 unx     2458 b- defN 24-May-30 10:07 nucliadb/reader/api/models.py
--rw-r--r--  2.0 unx     1110 b- defN 24-May-30 10:07 nucliadb/reader/api/v1/__init__.py
--rw-r--r--  2.0 unx    12457 b- defN 24-May-30 10:07 nucliadb/reader/api/v1/download.py
--rw-r--r--  2.0 unx     6459 b- defN 24-May-30 10:07 nucliadb/reader/api/v1/export_import.py
--rw-r--r--  2.0 unx     3641 b- defN 24-May-30 10:07 nucliadb/reader/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2099 b- defN 24-May-30 10:07 nucliadb/reader/api/v1/learning_collector.py
--rw-r--r--  2.0 unx     4472 b- defN 24-May-30 10:07 nucliadb/reader/api/v1/learning_config.py
--rw-r--r--  2.0 unx    13951 b- defN 24-May-30 10:07 nucliadb/reader/api/v1/resource.py
--rw-r--r--  2.0 unx     1011 b- defN 24-May-30 10:07 nucliadb/reader/api/v1/router.py
--rw-r--r--  2.0 unx    12115 b- defN 24-May-30 10:07 nucliadb/reader/api/v1/services.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/reader/reader/__init__.py
--rw-r--r--  2.0 unx     7979 b- defN 24-May-30 10:07 nucliadb/reader/reader/notifications.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/reader/tests/__init__.py
--rw-r--r--  2.0 unx     1224 b- defN 24-May-30 10:07 nucliadb/reader/tests/conftest.py
--rw-r--r--  2.0 unx     4345 b- defN 24-May-30 10:07 nucliadb/reader/tests/fixtures.py
--rw-r--r--  2.0 unx     2748 b- defN 24-May-30 10:07 nucliadb/reader/tests/test_list_resources.py
--rw-r--r--  2.0 unx    10199 b- defN 24-May-30 10:07 nucliadb/reader/tests/test_reader_file_download.py
--rw-r--r--  2.0 unx    10586 b- defN 24-May-30 10:07 nucliadb/reader/tests/test_reader_resource.py
--rw-r--r--  2.0 unx     6535 b- defN 24-May-30 10:07 nucliadb/reader/tests/test_reader_resource_field.py
--rw-r--r--  2.0 unx     1535 b- defN 24-May-30 10:07 nucliadb/search/__init__.py
--rw-r--r--  2.0 unx     4905 b- defN 24-May-30 10:07 nucliadb/search/app.py
--rw-r--r--  2.0 unx     1956 b- defN 24-May-30 10:07 nucliadb/search/lifecycle.py
--rw-r--r--  2.0 unx     1016 b- defN 24-May-30 10:07 nucliadb/search/openapi.py
--rw-r--r--  2.0 unx    20665 b- defN 24-May-30 10:07 nucliadb/search/predict.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-30 10:07 nucliadb/search/py.typed
--rw-r--r--  2.0 unx     1402 b- defN 24-May-30 10:07 nucliadb/search/run.py
--rw-r--r--  2.0 unx     1193 b- defN 24-May-30 10:07 nucliadb/search/settings.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-30 10:07 nucliadb/search/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/search/api/__init__.py
--rw-r--r--  2.0 unx     1298 b- defN 24-May-30 10:07 nucliadb/search/api/v1/__init__.py
--rw-r--r--  2.0 unx     3435 b- defN 24-May-30 10:07 nucliadb/search/api/v1/ask.py
--rw-r--r--  2.0 unx     9514 b- defN 24-May-30 10:07 nucliadb/search/api/v1/chat.py
--rw-r--r--  2.0 unx     2668 b- defN 24-May-30 10:07 nucliadb/search/api/v1/feedback.py
--rw-r--r--  2.0 unx     8795 b- defN 24-May-30 10:07 nucliadb/search/api/v1/find.py
--rw-r--r--  2.0 unx     6938 b- defN 24-May-30 10:07 nucliadb/search/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     3047 b- defN 24-May-30 10:07 nucliadb/search/api/v1/predict_proxy.py
--rw-r--r--  2.0 unx      988 b- defN 24-May-30 10:07 nucliadb/search/api/v1/router.py
--rw-r--r--  2.0 unx    19262 b- defN 24-May-30 10:07 nucliadb/search/api/v1/search.py
--rw-r--r--  2.0 unx     5970 b- defN 24-May-30 10:07 nucliadb/search/api/v1/suggest.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-30 10:07 nucliadb/search/api/v1/summarize.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-30 10:07 nucliadb/search/api/v1/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/search/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3866 b- defN 24-May-30 10:07 nucliadb/search/api/v1/resource/ask.py
--rw-r--r--  2.0 unx     5863 b- defN 24-May-30 10:07 nucliadb/search/api/v1/resource/chat.py
--rw-r--r--  2.0 unx     5303 b- defN 24-May-30 10:07 nucliadb/search/api/v1/resource/search.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-30 10:07 nucliadb/search/requesters/__init__.py
--rw-r--r--  2.0 unx     9111 b- defN 24-May-30 10:07 nucliadb/search/requesters/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/search/search/__init__.py
--rw-r--r--  2.0 unx     2746 b- defN 24-May-30 10:07 nucliadb/search/search/cache.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-30 10:07 nucliadb/search/search/exceptions.py
--rw-r--r--  2.0 unx     5465 b- defN 24-May-30 10:07 nucliadb/search/search/fetch.py
--rw-r--r--  2.0 unx     6513 b- defN 24-May-30 10:07 nucliadb/search/search/filters.py
--rw-r--r--  2.0 unx     4612 b- defN 24-May-30 10:07 nucliadb/search/search/find.py
--rw-r--r--  2.0 unx    17152 b- defN 24-May-30 10:07 nucliadb/search/search/find_merge.py
--rw-r--r--  2.0 unx    21282 b- defN 24-May-30 10:07 nucliadb/search/search/merge.py
--rw-r--r--  2.0 unx     1130 b- defN 24-May-30 10:07 nucliadb/search/search/metrics.py
--rw-r--r--  2.0 unx     8698 b- defN 24-May-30 10:07 nucliadb/search/search/paragraphs.py
--rw-r--r--  2.0 unx     3026 b- defN 24-May-30 10:07 nucliadb/search/search/predict_proxy.py
--rw-r--r--  2.0 unx    31093 b- defN 24-May-30 10:07 nucliadb/search/search/query.py
--rw-r--r--  2.0 unx     3018 b- defN 24-May-30 10:07 nucliadb/search/search/shards.py
--rw-r--r--  2.0 unx     5101 b- defN 24-May-30 10:07 nucliadb/search/search/summarize.py
--rw-r--r--  2.0 unx     2438 b- defN 24-May-30 10:07 nucliadb/search/search/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/search/search/chat/__init__.py
--rw-r--r--  2.0 unx    16676 b- defN 24-May-30 10:07 nucliadb/search/search/chat/ask.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-30 10:07 nucliadb/search/search/chat/images.py
--rw-r--r--  2.0 unx    20793 b- defN 24-May-30 10:07 nucliadb/search/search/chat/prompt.py
--rw-r--r--  2.0 unx    17543 b- defN 24-May-30 10:07 nucliadb/search/search/chat/query.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/search/tests/__init__.py
--rw-r--r--  2.0 unx     1295 b- defN 24-May-30 10:07 nucliadb/search/tests/conftest.py
--rw-r--r--  2.0 unx     6578 b- defN 24-May-30 10:07 nucliadb/search/tests/fixtures.py
--rw-r--r--  2.0 unx    15480 b- defN 24-May-30 10:07 nucliadb/search/tests/node.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/test_app.py
--rw-r--r--  2.0 unx     3374 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/test_find_merge.py
--rw-r--r--  2.0 unx     1400 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/test_merge.py
--rw-r--r--  2.0 unx    15721 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/test_predict.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/test_run.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/api/__init__.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/api/v1/__init__.py
--rw-r--r--  2.0 unx     3759 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/api/v1/test_ask.py
--rw-r--r--  2.0 unx     2966 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/api/v1/test_chat.py
--rw-r--r--  2.0 unx     2865 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
--rw-r--r--  2.0 unx     2901 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/api/v1/test_summarize.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/api/v1/resource/__init__.py
--rw-r--r--  2.0 unx     3040 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/search/__init__.py
--rw-r--r--  2.0 unx     8586 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/search/test_chat_prompt.py
--rw-r--r--  2.0 unx     3736 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/search/test_fetch.py
--rw-r--r--  2.0 unx     4306 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/search/test_filters.py
--rw-r--r--  2.0 unx     4492 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/search/test_paragraphs.py
--rw-r--r--  2.0 unx     3496 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/search/test_predict_proxy.py
--rw-r--r--  2.0 unx     5121 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/search/test_query.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/search/requesters/__init__.py
--rw-r--r--  2.0 unx     6455 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/search/requesters/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/search/search/__init__.py
--rw-r--r--  2.0 unx     1759 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/search/search/test_shards.py
--rw-r--r--  2.0 unx     2511 b- defN 24-May-30 10:07 nucliadb/search/tests/unit/search/search/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/standalone/__init__.py
--rw-r--r--  2.0 unx     6746 b- defN 24-May-30 10:07 nucliadb/standalone/api_router.py
--rw-r--r--  2.0 unx     5763 b- defN 24-May-30 10:07 nucliadb/standalone/app.py
--rw-r--r--  2.0 unx     7800 b- defN 24-May-30 10:07 nucliadb/standalone/auth.py
--rw-r--r--  2.0 unx     5313 b- defN 24-May-30 10:07 nucliadb/standalone/config.py
--rw-r--r--  2.0 unx     6986 b- defN 24-May-30 10:07 nucliadb/standalone/introspect.py
--rw-r--r--  2.0 unx     2488 b- defN 24-May-30 10:07 nucliadb/standalone/lifecycle.py
--rw-r--r--  2.0 unx     1980 b- defN 24-May-30 10:07 nucliadb/standalone/migrations.py
--rw-r--r--  2.0 unx     1322 b- defN 24-May-30 10:07 nucliadb/standalone/purge.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-30 10:07 nucliadb/standalone/py.typed
--rw-r--r--  2.0 unx     5636 b- defN 24-May-30 10:07 nucliadb/standalone/run.py
--rw-r--r--  2.0 unx     5822 b- defN 24-May-30 10:07 nucliadb/standalone/settings.py
--rw-r--r--  2.0 unx     3132 b- defN 24-May-30 10:07 nucliadb/standalone/versions.py
--rw-r--r--  2.0 unx     2285 b- defN 24-May-30 10:07 nucliadb/standalone/static/favicon.ico
--rw-r--r--  2.0 unx     3833 b- defN 24-May-30 10:07 nucliadb/standalone/static/index.html
--rw-r--r--  2.0 unx     2639 b- defN 24-May-30 10:07 nucliadb/standalone/static/logo.svg
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/standalone/tests/__init__.py
--rw-r--r--  2.0 unx     1294 b- defN 24-May-30 10:07 nucliadb/standalone/tests/conftest.py
--rw-r--r--  2.0 unx     1319 b- defN 24-May-30 10:07 nucliadb/standalone/tests/fixtures.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-30 10:07 nucliadb/standalone/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 24-May-30 10:07 nucliadb/standalone/tests/unit/test_api_router.py
--rw-r--r--  2.0 unx     5509 b- defN 24-May-30 10:07 nucliadb/standalone/tests/unit/test_auth.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-30 10:07 nucliadb/standalone/tests/unit/test_introspect.py
--rw-r--r--  2.0 unx     1863 b- defN 24-May-30 10:07 nucliadb/standalone/tests/unit/test_migrations.py
--rw-r--r--  2.0 unx     1546 b- defN 24-May-30 10:07 nucliadb/standalone/tests/unit/test_run.py
--rw-r--r--  2.0 unx     1972 b- defN 24-May-30 10:07 nucliadb/standalone/tests/unit/test_versions.py
--rw-r--r--  2.0 unx     1037 b- defN 24-May-30 10:07 nucliadb/tasks/__init__.py
--rw-r--r--  2.0 unx     7655 b- defN 24-May-30 10:07 nucliadb/tasks/consumer.py
--rw-r--r--  2.0 unx      924 b- defN 24-May-30 10:07 nucliadb/tasks/logger.py
--rw-r--r--  2.0 unx     1378 b- defN 24-May-30 10:07 nucliadb/tasks/models.py
--rw-r--r--  2.0 unx     3457 b- defN 24-May-30 10:07 nucliadb/tasks/producer.py
--rw-r--r--  2.0 unx     1753 b- defN 24-May-30 10:07 nucliadb/tasks/registry.py
--rw-r--r--  2.0 unx     1360 b- defN 24-May-30 10:07 nucliadb/tasks/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/tests/__init__.py
--rw-r--r--  2.0 unx     1229 b- defN 24-May-30 10:07 nucliadb/tests/conftest.py
--rw-r--r--  2.0 unx    22365 b- defN 24-May-30 10:07 nucliadb/tests/fixtures.py
--rw-r--r--  2.0 unx     7549 b- defN 24-May-30 10:07 nucliadb/tests/tikv.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/tests/benchmarks/__init__.py
--rw-r--r--  2.0 unx     3032 b- defN 24-May-30 10:07 nucliadb/tests/benchmarks/test_search.py
--rw-r--r--  2.0 unx      919 b- defN 24-May-30 10:07 nucliadb/tests/knowledgeboxes/__init__.py
--rw-r--r--  2.0 unx     7002 b- defN 24-May-30 10:07 nucliadb/tests/knowledgeboxes/philosophy_books.py
--rw-r--r--  2.0 unx     3037 b- defN 24-May-30 10:07 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
--rw-r--r--  2.0 unx     1148 b- defN 24-May-30 10:07 nucliadb/tests/migrations/__init__.py
--rw-r--r--  2.0 unx     2726 b- defN 24-May-30 10:07 nucliadb/tests/migrations/test_migration_0017.py
--rw-r--r--  2.0 unx     3662 b- defN 24-May-30 10:07 nucliadb/tests/migrations/test_migration_0018.py
--rw-r--r--  2.0 unx     3439 b- defN 24-May-30 10:07 nucliadb/tests/migrations/test_migration_0021.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/tests/unit/__init__.py
--rw-r--r--  2.0 unx     1487 b- defN 24-May-30 10:07 nucliadb/tests/unit/test_field_ids.py
--rw-r--r--  2.0 unx     2780 b- defN 24-May-30 10:07 nucliadb/tests/unit/test_health.py
--rw-r--r--  2.0 unx     1543 b- defN 24-May-30 10:07 nucliadb/tests/unit/test_kb_slugs.py
--rw-r--r--  2.0 unx     7892 b- defN 24-May-30 10:07 nucliadb/tests/unit/test_learning_proxy.py
--rw-r--r--  2.0 unx     2642 b- defN 24-May-30 10:07 nucliadb/tests/unit/test_metrics_exporter.py
--rw-r--r--  2.0 unx     1341 b- defN 24-May-30 10:07 nucliadb/tests/unit/test_openapi.py
--rw-r--r--  2.0 unx     3649 b- defN 24-May-30 10:07 nucliadb/tests/unit/test_purge.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/__init__.py
--rw-r--r--  2.0 unx     1268 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/test_context.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/cluster/__init__.py
--rw-r--r--  2.0 unx    12240 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/cluster/test_cluster.py
--rw-r--r--  2.0 unx     5387 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
--rw-r--r--  2.0 unx     1428 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/cluster/test_rebalance.py
--rw-r--r--  2.0 unx     9465 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/cluster/test_rollover.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/cluster/discovery/__init__.py
--rw-r--r--  2.0 unx     5627 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/cluster/standalone/__init__.py
--rw-r--r--  2.0 unx     3761 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/cluster/standalone/test_service.py
--rw-r--r--  2.0 unx     2136 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
--rw-r--r--  2.0 unx      833 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/maindb/__init__.py
--rw-r--r--  2.0 unx     3579 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/maindb/test_driver.py
--rw-r--r--  2.0 unx     2119 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/maindb/test_tikv.py
--rw-r--r--  2.0 unx     3213 b- defN 24-May-30 10:07 nucliadb/tests/unit/common/maindb/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/tests/unit/export_import/__init__.py
--rw-r--r--  2.0 unx     1435 b- defN 24-May-30 10:07 nucliadb/tests/unit/export_import/test_datamanager.py
--rw-r--r--  2.0 unx     9706 b- defN 24-May-30 10:07 nucliadb/tests/unit/export_import/test_utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/tests/unit/migrator/__init__.py
--rw-r--r--  2.0 unx     3233 b- defN 24-May-30 10:07 nucliadb/tests/unit/migrator/test_migrator.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/tests/unit/tasks/__init__.py
--rw-r--r--  2.0 unx     1375 b- defN 24-May-30 10:07 nucliadb/tests/unit/tasks/conftest.py
--rw-r--r--  2.0 unx     2714 b- defN 24-May-30 10:07 nucliadb/tests/unit/tasks/test_consumer.py
--rw-r--r--  2.0 unx     3189 b- defN 24-May-30 10:07 nucliadb/tests/unit/tasks/test_producer.py
--rw-r--r--  2.0 unx     1827 b- defN 24-May-30 10:07 nucliadb/tests/unit/tasks/test_tasks.py
--rw-r--r--  2.0 unx     2507 b- defN 24-May-30 10:07 nucliadb/tests/utils/__init__.py
--rw-r--r--  2.0 unx     1797 b- defN 24-May-30 10:07 nucliadb/tests/utils/aiohttp_session.py
--rw-r--r--  2.0 unx     2533 b- defN 24-May-30 10:07 nucliadb/tests/utils/entities.py
--rw-r--r--  2.0 unx     6327 b- defN 24-May-30 10:07 nucliadb/tests/utils/broker_messages/__init__.py
--rw-r--r--  2.0 unx     7557 b- defN 24-May-30 10:07 nucliadb/tests/utils/broker_messages/fields.py
--rw-r--r--  2.0 unx     1196 b- defN 24-May-30 10:07 nucliadb/tests/utils/broker_messages/helpers.py
--rw-r--r--  2.0 unx     1325 b- defN 24-May-30 10:07 nucliadb/train/__init__.py
--rw-r--r--  2.0 unx     3530 b- defN 24-May-30 10:07 nucliadb/train/app.py
--rw-r--r--  2.0 unx     3800 b- defN 24-May-30 10:07 nucliadb/train/generator.py
--rw-r--r--  2.0 unx     1698 b- defN 24-May-30 10:07 nucliadb/train/lifecycle.py
--rw-r--r--  2.0 unx     1198 b- defN 24-May-30 10:07 nucliadb/train/models.py
--rw-r--r--  2.0 unx     5706 b- defN 24-May-30 10:07 nucliadb/train/nodes.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-30 10:07 nucliadb/train/py.typed
--rw-r--r--  2.0 unx     1400 b- defN 24-May-30 10:07 nucliadb/train/run.py
--rw-r--r--  2.0 unx     5926 b- defN 24-May-30 10:07 nucliadb/train/servicer.py
--rw-r--r--  2.0 unx     1415 b- defN 24-May-30 10:07 nucliadb/train/settings.py
--rw-r--r--  2.0 unx     1496 b- defN 24-May-30 10:07 nucliadb/train/types.py
--rw-r--r--  2.0 unx     3265 b- defN 24-May-30 10:07 nucliadb/train/upload.py
--rw-r--r--  2.0 unx     6420 b- defN 24-May-30 10:07 nucliadb/train/uploader.py
--rw-r--r--  2.0 unx     3179 b- defN 24-May-30 10:07 nucliadb/train/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/train/api/__init__.py
--rw-r--r--  2.0 unx     1479 b- defN 24-May-30 10:07 nucliadb/train/api/utils.py
--rw-r--r--  2.0 unx      928 b- defN 24-May-30 10:07 nucliadb/train/api/v1/__init__.py
--rw-r--r--  2.0 unx     2071 b- defN 24-May-30 10:07 nucliadb/train/api/v1/check.py
--rw-r--r--  2.0 unx      910 b- defN 24-May-30 10:07 nucliadb/train/api/v1/router.py
--rw-r--r--  2.0 unx     1908 b- defN 24-May-30 10:07 nucliadb/train/api/v1/shards.py
--rw-r--r--  2.0 unx     2135 b- defN 24-May-30 10:07 nucliadb/train/api/v1/trainset.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/train/generators/__init__.py
--rw-r--r--  2.0 unx     3723 b- defN 24-May-30 10:07 nucliadb/train/generators/field_classifier.py
--rw-r--r--  2.0 unx     6712 b- defN 24-May-30 10:07 nucliadb/train/generators/image_classifier.py
--rw-r--r--  2.0 unx     2789 b- defN 24-May-30 10:07 nucliadb/train/generators/paragraph_classifier.py
--rw-r--r--  2.0 unx     3590 b- defN 24-May-30 10:07 nucliadb/train/generators/paragraph_streaming.py
--rw-r--r--  2.0 unx     5372 b- defN 24-May-30 10:07 nucliadb/train/generators/question_answer_streaming.py
--rw-r--r--  2.0 unx     5160 b- defN 24-May-30 10:07 nucliadb/train/generators/sentence_classifier.py
--rw-r--r--  2.0 unx    10446 b- defN 24-May-30 10:07 nucliadb/train/generators/token_classifier.py
--rw-r--r--  2.0 unx     3877 b- defN 24-May-30 10:07 nucliadb/train/generators/utils.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/train/tests/__init__.py
--rw-r--r--  2.0 unx     1125 b- defN 24-May-30 10:07 nucliadb/train/tests/conftest.py
--rw-r--r--  2.0 unx    11053 b- defN 24-May-30 10:07 nucliadb/train/tests/fixtures.py
--rw-r--r--  2.0 unx     4598 b- defN 24-May-30 10:07 nucliadb/train/tests/test_field_classification.py
--rw-r--r--  2.0 unx     2729 b- defN 24-May-30 10:07 nucliadb/train/tests/test_get_entities.py
--rw-r--r--  2.0 unx     1660 b- defN 24-May-30 10:07 nucliadb/train/tests/test_get_info.py
--rw-r--r--  2.0 unx     1382 b- defN 24-May-30 10:07 nucliadb/train/tests/test_get_ontology.py
--rw-r--r--  2.0 unx     2201 b- defN 24-May-30 10:07 nucliadb/train/tests/test_get_ontology_count.py
--rw-r--r--  2.0 unx     7669 b- defN 24-May-30 10:07 nucliadb/train/tests/test_image_classification.py
--rw-r--r--  2.0 unx     1416 b- defN 24-May-30 10:07 nucliadb/train/tests/test_list_fields.py
--rw-r--r--  2.0 unx     2944 b- defN 24-May-30 10:07 nucliadb/train/tests/test_list_paragraphs.py
--rw-r--r--  2.0 unx     1423 b- defN 24-May-30 10:07 nucliadb/train/tests/test_list_resources.py
--rw-r--r--  2.0 unx     2947 b- defN 24-May-30 10:07 nucliadb/train/tests/test_list_sentences.py
--rw-r--r--  2.0 unx     4645 b- defN 24-May-30 10:07 nucliadb/train/tests/test_paragraph_classification.py
--rw-r--r--  2.0 unx     4320 b- defN 24-May-30 10:07 nucliadb/train/tests/test_paragraph_streaming.py
--rw-r--r--  2.0 unx     8751 b- defN 24-May-30 10:07 nucliadb/train/tests/test_question_answer_streaming.py
--rw-r--r--  2.0 unx     5051 b- defN 24-May-30 10:07 nucliadb/train/tests/test_sentence_classification.py
--rw-r--r--  2.0 unx     5583 b- defN 24-May-30 10:07 nucliadb/train/tests/test_token_classification.py
--rw-r--r--  2.0 unx     3324 b- defN 24-May-30 10:07 nucliadb/train/tests/utils.py
--rw-r--r--  2.0 unx     1328 b- defN 24-May-30 10:07 nucliadb/writer/__init__.py
--rw-r--r--  2.0 unx     4268 b- defN 24-May-30 10:07 nucliadb/writer/app.py
--rw-r--r--  2.0 unx    19483 b- defN 24-May-30 10:07 nucliadb/writer/back_pressure.py
--rw-r--r--  2.0 unx      972 b- defN 24-May-30 10:07 nucliadb/writer/exceptions.py
--rw-r--r--  2.0 unx     1953 b- defN 24-May-30 10:07 nucliadb/writer/lifecycle.py
--rw-r--r--  2.0 unx     1032 b- defN 24-May-30 10:07 nucliadb/writer/openapi.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-30 10:07 nucliadb/writer/py.typed
--rw-r--r--  2.0 unx     1448 b- defN 24-May-30 10:07 nucliadb/writer/run.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-30 10:07 nucliadb/writer/settings.py
--rw-r--r--  2.0 unx     1036 b- defN 24-May-30 10:07 nucliadb/writer/utilities.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/writer/api/__init__.py
--rw-r--r--  2.0 unx     1429 b- defN 24-May-30 10:07 nucliadb/writer/api/constants.py
--rw-r--r--  2.0 unx     1095 b- defN 24-May-30 10:07 nucliadb/writer/api/v1/__init__.py
--rw-r--r--  2.0 unx     6421 b- defN 24-May-30 10:07 nucliadb/writer/api/v1/export_import.py
--rw-r--r--  2.0 unx    24482 b- defN 24-May-30 10:07 nucliadb/writer/api/v1/field.py
--rw-r--r--  2.0 unx     5248 b- defN 24-May-30 10:07 nucliadb/writer/api/v1/knowledgebox.py
--rw-r--r--  2.0 unx     2058 b- defN 24-May-30 10:07 nucliadb/writer/api/v1/learning_config.py
--rw-r--r--  2.0 unx    18628 b- defN 24-May-30 10:07 nucliadb/writer/api/v1/resource.py
--rw-r--r--  2.0 unx     1034 b- defN 24-May-30 10:07 nucliadb/writer/api/v1/router.py
--rw-r--r--  2.0 unx    10216 b- defN 24-May-30 10:07 nucliadb/writer/api/v1/services.py
--rw-r--r--  2.0 unx    30985 b- defN 24-May-30 10:07 nucliadb/writer/api/v1/upload.py
--rw-r--r--  2.0 unx     1612 b- defN 24-May-30 10:07 nucliadb/writer/layouts/__init__.py
--rw-r--r--  2.0 unx     2115 b- defN 24-May-30 10:07 nucliadb/writer/layouts/v1.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/writer/resource/__init__.py
--rw-r--r--  2.0 unx     1425 b- defN 24-May-30 10:07 nucliadb/writer/resource/audit.py
--rw-r--r--  2.0 unx    10968 b- defN 24-May-30 10:07 nucliadb/writer/resource/basic.py
--rw-r--r--  2.0 unx    16740 b- defN 24-May-30 10:07 nucliadb/writer/resource/field.py
--rw-r--r--  2.0 unx     2022 b- defN 24-May-30 10:07 nucliadb/writer/resource/origin.py
--rw-r--r--  2.0 unx      835 b- defN 24-May-30 10:07 nucliadb/writer/tests/__init__.py
--rw-r--r--  2.0 unx     1200 b- defN 24-May-30 10:07 nucliadb/writer/tests/conftest.py
--rw-r--r--  2.0 unx     5971 b- defN 24-May-30 10:07 nucliadb/writer/tests/fixtures.py
--rw-r--r--  2.0 unx    15472 b- defN 24-May-30 10:07 nucliadb/writer/tests/test_fields.py
--rw-r--r--  2.0 unx    25999 b- defN 24-May-30 10:07 nucliadb/writer/tests/test_files.py
--rw-r--r--  2.0 unx     1729 b- defN 24-May-30 10:07 nucliadb/writer/tests/test_knowledgebox.py
--rw-r--r--  2.0 unx     4400 b- defN 24-May-30 10:07 nucliadb/writer/tests/test_reprocess_file_field.py
--rw-r--r--  2.0 unx    16857 b- defN 24-May-30 10:07 nucliadb/writer/tests/test_resources.py
--rw-r--r--  2.0 unx     5120 b- defN 24-May-30 10:07 nucliadb/writer/tests/test_service.py
--rw-r--r--  2.0 unx     6054 b- defN 24-May-30 10:07 nucliadb/writer/tests/test_tus.py
--rw-r--r--  2.0 unx     1287 b- defN 24-May-30 10:07 nucliadb/writer/tests/utils.py
--rw-r--r--  2.0 unx     5226 b- defN 24-May-30 10:07 nucliadb/writer/tus/__init__.py
--rw-r--r--  2.0 unx     5082 b- defN 24-May-30 10:07 nucliadb/writer/tus/dm.py
--rw-r--r--  2.0 unx     2186 b- defN 24-May-30 10:07 nucliadb/writer/tus/exceptions.py
--rw-r--r--  2.0 unx    14527 b- defN 24-May-30 10:07 nucliadb/writer/tus/gcs.py
--rw-r--r--  2.0 unx     5849 b- defN 24-May-30 10:07 nucliadb/writer/tus/local.py
--rw-r--r--  2.0 unx     4367 b- defN 24-May-30 10:07 nucliadb/writer/tus/pg.py
--rw-r--r--  2.0 unx     9069 b- defN 24-May-30 10:07 nucliadb/writer/tus/s3.py
--rw-r--r--  2.0 unx     4734 b- defN 24-May-30 10:07 nucliadb/writer/tus/storage.py
--rw-r--r--  2.0 unx     2556 b- defN 24-May-30 10:07 nucliadb/writer/tus/utils.py
--rw-r--r--  2.0 unx     4474 b- defN 24-May-30 10:09 nucliadb-4.0.3.post560.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-30 10:09 nucliadb-4.0.3.post560.dist-info/WHEEL
--rw-r--r--  2.0 unx     1268 b- defN 24-May-30 10:09 nucliadb-4.0.3.post560.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 24-May-30 10:09 nucliadb-4.0.3.post560.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 24-May-30 10:08 nucliadb-4.0.3.post560.dist-info/zip-safe
--rw-rw-r--  2.0 unx    44141 b- defN 24-May-30 10:09 nucliadb-4.0.3.post560.dist-info/RECORD
-471 files, 2278544 bytes uncompressed, 700840 bytes compressed:  69.3%
+Zip file size: 771455 bytes, number of entries: 471
+-rw-r--r--  2.0 unx     1135 b- defN 24-May-30 15:11 migrations/0001_bootstrap.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-30 15:11 migrations/0002_rollover_shards.py
+-rw-r--r--  2.0 unx     2436 b- defN 24-May-30 15:11 migrations/0003_allfields_key.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-30 15:11 migrations/0004_rollover_shards.py
+-rw-r--r--  2.0 unx     1177 b- defN 24-May-30 15:11 migrations/0005_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-30 15:11 migrations/0006_rollover_shards.py
+-rw-r--r--  2.0 unx     1301 b- defN 24-May-30 15:11 migrations/0008_cleanup_leftover_rollover_metadata.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-30 15:11 migrations/0009_upgrade_relations_and_texts_to_v2.py
+-rw-r--r--  2.0 unx     1610 b- defN 24-May-30 15:11 migrations/0010_fix_corrupt_indexes.py
+-rw-r--r--  2.0 unx     1843 b- defN 24-May-30 15:11 migrations/0011_materialize_labelset_ids.py
+-rw-r--r--  2.0 unx     1443 b- defN 24-May-30 15:11 migrations/0012_rollover_shards.py
+-rw-r--r--  2.0 unx     1024 b- defN 24-May-30 15:11 migrations/0013_rollover_shards.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-30 15:11 migrations/0014_rollover_shards.py
+-rw-r--r--  2.0 unx     1462 b- defN 24-May-30 15:11 migrations/0015_targeted_rollover.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-30 15:11 migrations/0016_upgrade_to_paragraphs_v2.py
+-rw-r--r--  2.0 unx     2100 b- defN 24-May-30 15:11 migrations/0017_multiple_writable_shards.py
+-rw-r--r--  2.0 unx     2264 b- defN 24-May-30 15:11 migrations/0018_purge_orphan_kbslugs.py
+-rw-r--r--  2.0 unx     2506 b- defN 24-May-30 15:11 migrations/0019_upgrade_to_paragraphs_v3.py
+-rw-r--r--  2.0 unx     3282 b- defN 24-May-30 15:11 migrations/0020_drain_nodes_from_cluster.py
+-rw-r--r--  2.0 unx     1734 b- defN 24-May-30 15:11 migrations/0021_overwrite_vectorsets_key.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 migrations/__init__.py
+-rw-r--r--  2.0 unx      891 b- defN 24-May-30 15:11 nucliadb/__init__.py
+-rw-r--r--  2.0 unx     3733 b- defN 24-May-30 15:11 nucliadb/health.py
+-rw-r--r--  2.0 unx    11793 b- defN 24-May-30 15:11 nucliadb/learning_proxy.py
+-rw-r--r--  2.0 unx     4806 b- defN 24-May-30 15:11 nucliadb/metrics_exporter.py
+-rw-r--r--  2.0 unx     2272 b- defN 24-May-30 15:11 nucliadb/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 15:11 nucliadb/py.typed
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/common/__init__.py
+-rw-r--r--  2.0 unx     5175 b- defN 24-May-30 15:11 nucliadb/common/locking.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/common/cluster/__init__.py
+-rw-r--r--  2.0 unx     5134 b- defN 24-May-30 15:11 nucliadb/common/cluster/base.py
+-rw-r--r--  2.0 unx     1495 b- defN 24-May-30 15:11 nucliadb/common/cluster/exceptions.py
+-rw-r--r--  2.0 unx     3793 b- defN 24-May-30 15:11 nucliadb/common/cluster/grpc_node_dummy.py
+-rw-r--r--  2.0 unx     3429 b- defN 24-May-30 15:11 nucliadb/common/cluster/index_node.py
+-rw-r--r--  2.0 unx    24815 b- defN 24-May-30 15:11 nucliadb/common/cluster/manager.py
+-rw-r--r--  2.0 unx     8853 b- defN 24-May-30 15:11 nucliadb/common/cluster/rebalance.py
+-rw-r--r--  2.0 unx    20532 b- defN 24-May-30 15:11 nucliadb/common/cluster/rollover.py
+-rw-r--r--  2.0 unx     3016 b- defN 24-May-30 15:11 nucliadb/common/cluster/settings.py
+-rw-r--r--  2.0 unx     5713 b- defN 24-May-30 15:11 nucliadb/common/cluster/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     6553 b- defN 24-May-30 15:11 nucliadb/common/cluster/discovery/base.py
+-rw-r--r--  2.0 unx    12512 b- defN 24-May-30 15:11 nucliadb/common/cluster/discovery/k8s.py
+-rw-r--r--  2.0 unx     1957 b- defN 24-May-30 15:11 nucliadb/common/cluster/discovery/manual.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-30 15:11 nucliadb/common/cluster/discovery/single.py
+-rw-r--r--  2.0 unx     1139 b- defN 24-May-30 15:11 nucliadb/common/cluster/discovery/types.py
+-rw-r--r--  2.0 unx     2548 b- defN 24-May-30 15:11 nucliadb/common/cluster/discovery/utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-30 15:11 nucliadb/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx    13712 b- defN 24-May-30 15:11 nucliadb/common/cluster/standalone/grpc_node_binding.py
+-rw-r--r--  2.0 unx     4683 b- defN 24-May-30 15:11 nucliadb/common/cluster/standalone/index_node.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-May-30 15:11 nucliadb/common/cluster/standalone/service.py
+-rw-r--r--  2.0 unx     3545 b- defN 24-May-30 15:11 nucliadb/common/cluster/standalone/utils.py
+-rw-r--r--  2.0 unx     3440 b- defN 24-May-30 15:11 nucliadb/common/context/__init__.py
+-rw-r--r--  2.0 unx     1628 b- defN 24-May-30 15:11 nucliadb/common/context/fastapi.py
+-rw-r--r--  2.0 unx     1940 b- defN 24-May-30 15:11 nucliadb/common/datamanagers/__init__.py
+-rw-r--r--  2.0 unx     2648 b- defN 24-May-30 15:11 nucliadb/common/datamanagers/atomic.py
+-rw-r--r--  2.0 unx     1451 b- defN 24-May-30 15:11 nucliadb/common/datamanagers/cluster.py
+-rw-r--r--  2.0 unx     5383 b- defN 24-May-30 15:11 nucliadb/common/datamanagers/entities.py
+-rw-r--r--  2.0 unx      883 b- defN 24-May-30 15:11 nucliadb/common/datamanagers/exceptions.py
+-rw-r--r--  2.0 unx     3994 b- defN 24-May-30 15:11 nucliadb/common/datamanagers/kb.py
+-rw-r--r--  2.0 unx     5389 b- defN 24-May-30 15:11 nucliadb/common/datamanagers/labels.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-30 15:11 nucliadb/common/datamanagers/processing.py
+-rw-r--r--  2.0 unx    12177 b- defN 24-May-30 15:11 nucliadb/common/datamanagers/resources.py
+-rw-r--r--  2.0 unx     5634 b- defN 24-May-30 15:11 nucliadb/common/datamanagers/rollover.py
+-rw-r--r--  2.0 unx     1548 b- defN 24-May-30 15:11 nucliadb/common/datamanagers/synonyms.py
+-rw-r--r--  2.0 unx     1631 b- defN 24-May-30 15:11 nucliadb/common/datamanagers/utils.py
+-rw-r--r--  2.0 unx     3780 b- defN 24-May-30 15:11 nucliadb/common/datamanagers/vectorsets.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/common/http_clients/__init__.py
+-rw-r--r--  2.0 unx     2146 b- defN 24-May-30 15:11 nucliadb/common/http_clients/auth.py
+-rw-r--r--  2.0 unx     1100 b- defN 24-May-30 15:11 nucliadb/common/http_clients/exceptions.py
+-rw-r--r--  2.0 unx     7155 b- defN 24-May-30 15:11 nucliadb/common/http_clients/processing.py
+-rw-r--r--  2.0 unx     1540 b- defN 24-May-30 15:11 nucliadb/common/http_clients/pypi.py
+-rw-r--r--  2.0 unx     1551 b- defN 24-May-30 15:11 nucliadb/common/http_clients/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3449 b- defN 24-May-30 15:11 nucliadb/common/maindb/driver.py
+-rw-r--r--  2.0 unx      988 b- defN 24-May-30 15:11 nucliadb/common/maindb/exceptions.py
+-rw-r--r--  2.0 unx     6769 b- defN 24-May-30 15:11 nucliadb/common/maindb/local.py
+-rw-r--r--  2.0 unx     8391 b- defN 24-May-30 15:11 nucliadb/common/maindb/pg.py
+-rw-r--r--  2.0 unx     6053 b- defN 24-May-30 15:11 nucliadb/common/maindb/redis.py
+-rw-r--r--  2.0 unx    15314 b- defN 24-May-30 15:11 nucliadb/common/maindb/tikv.py
+-rw-r--r--  2.0 unx     4167 b- defN 24-May-30 15:11 nucliadb/common/maindb/utils.py
+-rw-r--r--  2.0 unx      932 b- defN 24-May-30 15:11 nucliadb/export_import/__init__.py
+-rw-r--r--  2.0 unx     6171 b- defN 24-May-30 15:11 nucliadb/export_import/datamanager.py
+-rw-r--r--  2.0 unx     1949 b- defN 24-May-30 15:11 nucliadb/export_import/exceptions.py
+-rw-r--r--  2.0 unx     7116 b- defN 24-May-30 15:11 nucliadb/export_import/exporter.py
+-rw-r--r--  2.0 unx     4258 b- defN 24-May-30 15:11 nucliadb/export_import/importer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-30 15:11 nucliadb/export_import/models.py
+-rw-r--r--  2.0 unx     2571 b- defN 24-May-30 15:11 nucliadb/export_import/tasks.py
+-rw-r--r--  2.0 unx    19401 b- defN 24-May-30 15:11 nucliadb/export_import/utils.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-30 15:11 nucliadb/ingest/__init__.py
+-rw-r--r--  2.0 unx     7277 b- defN 24-May-30 15:11 nucliadb/ingest/app.py
+-rw-r--r--  2.0 unx     1005 b- defN 24-May-30 15:11 nucliadb/ingest/cache.py
+-rw-r--r--  2.0 unx     2484 b- defN 24-May-30 15:11 nucliadb/ingest/partitions.py
+-rw-r--r--  2.0 unx    19904 b- defN 24-May-30 15:11 nucliadb/ingest/processing.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 15:11 nucliadb/ingest/py.typed
+-rw-r--r--  2.0 unx    20277 b- defN 24-May-30 15:11 nucliadb/ingest/serialize.py
+-rw-r--r--  2.0 unx     3207 b- defN 24-May-30 15:11 nucliadb/ingest/settings.py
+-rw-r--r--  2.0 unx     2314 b- defN 24-May-30 15:11 nucliadb/ingest/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/ingest/consumer/__init__.py
+-rw-r--r--  2.0 unx     6918 b- defN 24-May-30 15:11 nucliadb/ingest/consumer/auditing.py
+-rw-r--r--  2.0 unx    12174 b- defN 24-May-30 15:11 nucliadb/ingest/consumer/consumer.py
+-rw-r--r--  2.0 unx     3945 b- defN 24-May-30 15:11 nucliadb/ingest/consumer/materializer.py
+-rw-r--r--  2.0 unx     1075 b- defN 24-May-30 15:11 nucliadb/ingest/consumer/metrics.py
+-rw-r--r--  2.0 unx     9543 b- defN 24-May-30 15:11 nucliadb/ingest/consumer/pull.py
+-rw-r--r--  2.0 unx     6871 b- defN 24-May-30 15:11 nucliadb/ingest/consumer/service.py
+-rw-r--r--  2.0 unx     4331 b- defN 24-May-30 15:11 nucliadb/ingest/consumer/shard_creator.py
+-rw-r--r--  2.0 unx     2656 b- defN 24-May-30 15:11 nucliadb/ingest/consumer/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/ingest/fields/__init__.py
+-rw-r--r--  2.0 unx    17461 b- defN 24-May-30 15:11 nucliadb/ingest/fields/base.py
+-rw-r--r--  2.0 unx     6516 b- defN 24-May-30 15:11 nucliadb/ingest/fields/conversation.py
+-rw-r--r--  2.0 unx     1223 b- defN 24-May-30 15:11 nucliadb/ingest/fields/date.py
+-rw-r--r--  2.0 unx     1205 b- defN 24-May-30 15:11 nucliadb/ingest/fields/exceptions.py
+-rw-r--r--  2.0 unx     4840 b- defN 24-May-30 15:11 nucliadb/ingest/fields/file.py
+-rw-r--r--  2.0 unx     1547 b- defN 24-May-30 15:11 nucliadb/ingest/fields/generic.py
+-rw-r--r--  2.0 unx     1235 b- defN 24-May-30 15:11 nucliadb/ingest/fields/keywordset.py
+-rw-r--r--  2.0 unx     2250 b- defN 24-May-30 15:11 nucliadb/ingest/fields/layout.py
+-rw-r--r--  2.0 unx     4212 b- defN 24-May-30 15:11 nucliadb/ingest/fields/link.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-30 15:11 nucliadb/ingest/fields/text.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/ingest/orm/__init__.py
+-rw-r--r--  2.0 unx    28311 b- defN 24-May-30 15:11 nucliadb/ingest/orm/brain.py
+-rw-r--r--  2.0 unx    15758 b- defN 24-May-30 15:11 nucliadb/ingest/orm/entities.py
+-rw-r--r--  2.0 unx     1326 b- defN 24-May-30 15:11 nucliadb/ingest/orm/exceptions.py
+-rw-r--r--  2.0 unx    16808 b- defN 24-May-30 15:11 nucliadb/ingest/orm/knowledgebox.py
+-rw-r--r--  2.0 unx     1096 b- defN 24-May-30 15:11 nucliadb/ingest/orm/metrics.py
+-rw-r--r--  2.0 unx    58955 b- defN 24-May-30 15:11 nucliadb/ingest/orm/resource.py
+-rw-r--r--  2.0 unx     2685 b- defN 24-May-30 15:11 nucliadb/ingest/orm/utils.py
+-rw-r--r--  2.0 unx    27092 b- defN 24-May-30 15:11 nucliadb/ingest/orm/processor/__init__.py
+-rw-r--r--  2.0 unx     5090 b- defN 24-May-30 15:11 nucliadb/ingest/orm/processor/auditing.py
+-rw-r--r--  2.0 unx     1690 b- defN 24-May-30 15:11 nucliadb/ingest/orm/processor/sequence_manager.py
+-rw-r--r--  2.0 unx     2057 b- defN 24-May-30 15:11 nucliadb/ingest/service/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/ingest/service/exceptions.py
+-rw-r--r--  2.0 unx    32813 b- defN 24-May-30 15:11 nucliadb/ingest/service/writer.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/ingest/tests/__init__.py
+-rw-r--r--  2.0 unx     1157 b- defN 24-May-30 15:11 nucliadb/ingest/tests/conftest.py
+-rw-r--r--  2.0 unx    24111 b- defN 24-May-30 15:11 nucliadb/ingest/tests/fixtures.py
+-rw-r--r--  2.0 unx    62843 b- defN 24-May-30 15:11 nucliadb/ingest/tests/vectors.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/ingest/tests/integration/__init__.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-30 15:11 nucliadb/ingest/tests/integration/consumer/__init__.py
+-rw-r--r--  2.0 unx     2500 b- defN 24-May-30 15:11 nucliadb/ingest/tests/integration/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     3836 b- defN 24-May-30 15:11 nucliadb/ingest/tests/integration/consumer/test_materializer.py
+-rw-r--r--  2.0 unx     4470 b- defN 24-May-30 15:11 nucliadb/ingest/tests/integration/consumer/test_pull.py
+-rw-r--r--  2.0 unx     2763 b- defN 24-May-30 15:11 nucliadb/ingest/tests/integration/consumer/test_service.py
+-rw-r--r--  2.0 unx     2019 b- defN 24-May-30 15:11 nucliadb/ingest/tests/integration/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/ingest/tests/integration/ingest/__init__.py
+-rw-r--r--  2.0 unx    27247 b- defN 24-May-30 15:11 nucliadb/ingest/tests/integration/ingest/test_ingest.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-30 15:11 nucliadb/ingest/tests/integration/ingest/test_processing_engine.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-30 15:11 nucliadb/ingest/tests/integration/ingest/test_relations.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1189 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/test_cache.py
+-rw-r--r--  2.0 unx     1432 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/test_partitions.py
+-rw-r--r--  2.0 unx     5807 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/test_processing.py
+-rw-r--r--  2.0 unx      978 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/test_settings.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/consumer/__init__.py
+-rw-r--r--  2.0 unx     3885 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/consumer/test_auditing.py
+-rw-r--r--  2.0 unx     2472 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/consumer/test_consumer.py
+-rw-r--r--  2.0 unx     2063 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/consumer/test_pull.py
+-rw-r--r--  2.0 unx     4140 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/consumer/test_shard_creator.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/consumer/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/orm/__init__.py
+-rw-r--r--  2.0 unx     9876 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/orm/test_brain.py
+-rw-r--r--  2.0 unx     2435 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/orm/test_brain_vectors.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/orm/test_orm_utils.py
+-rw-r--r--  2.0 unx     4045 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/orm/test_processor.py
+-rw-r--r--  2.0 unx    11033 b- defN 24-May-30 15:11 nucliadb/ingest/tests/unit/orm/test_resource.py
+-rw-r--r--  2.0 unx     2216 b- defN 24-May-30 15:11 nucliadb/middleware/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-May-30 15:11 nucliadb/middleware/transaction.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/migrator/__init__.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-30 15:11 nucliadb/migrator/command.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-30 15:11 nucliadb/migrator/context.py
+-rw-r--r--  2.0 unx     5104 b- defN 24-May-30 15:11 nucliadb/migrator/datamanager.py
+-rw-r--r--  2.0 unx      889 b- defN 24-May-30 15:11 nucliadb/migrator/exceptions.py
+-rw-r--r--  2.0 unx     9370 b- defN 24-May-30 15:11 nucliadb/migrator/migrator.py
+-rw-r--r--  2.0 unx     1145 b- defN 24-May-30 15:11 nucliadb/migrator/models.py
+-rw-r--r--  2.0 unx     1144 b- defN 24-May-30 15:11 nucliadb/migrator/settings.py
+-rw-r--r--  2.0 unx     2346 b- defN 24-May-30 15:11 nucliadb/migrator/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/models/__init__.py
+-rw-r--r--  2.0 unx     1599 b- defN 24-May-30 15:11 nucliadb/models/responses.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-May-30 15:11 nucliadb/purge/__init__.py
+-rw-r--r--  2.0 unx     9364 b- defN 24-May-30 15:11 nucliadb/purge/orphan_shards.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-30 15:11 nucliadb/reader/__init__.py
+-rw-r--r--  2.0 unx     3709 b- defN 24-May-30 15:11 nucliadb/reader/app.py
+-rw-r--r--  2.0 unx     1366 b- defN 24-May-30 15:11 nucliadb/reader/lifecycle.py
+-rw-r--r--  2.0 unx     1031 b- defN 24-May-30 15:11 nucliadb/reader/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 15:11 nucliadb/reader/py.typed
+-rw-r--r--  2.0 unx     1447 b- defN 24-May-30 15:11 nucliadb/reader/run.py
+-rw-r--r--  2.0 unx      872 b- defN 24-May-30 15:11 nucliadb/reader/api/__init__.py
+-rw-r--r--  2.0 unx     2458 b- defN 24-May-30 15:11 nucliadb/reader/api/models.py
+-rw-r--r--  2.0 unx     1110 b- defN 24-May-30 15:11 nucliadb/reader/api/v1/__init__.py
+-rw-r--r--  2.0 unx    12457 b- defN 24-May-30 15:11 nucliadb/reader/api/v1/download.py
+-rw-r--r--  2.0 unx     6459 b- defN 24-May-30 15:11 nucliadb/reader/api/v1/export_import.py
+-rw-r--r--  2.0 unx     3641 b- defN 24-May-30 15:11 nucliadb/reader/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2099 b- defN 24-May-30 15:11 nucliadb/reader/api/v1/learning_collector.py
+-rw-r--r--  2.0 unx     4472 b- defN 24-May-30 15:11 nucliadb/reader/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    13951 b- defN 24-May-30 15:11 nucliadb/reader/api/v1/resource.py
+-rw-r--r--  2.0 unx     1011 b- defN 24-May-30 15:11 nucliadb/reader/api/v1/router.py
+-rw-r--r--  2.0 unx    12115 b- defN 24-May-30 15:11 nucliadb/reader/api/v1/services.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/reader/reader/__init__.py
+-rw-r--r--  2.0 unx     7979 b- defN 24-May-30 15:11 nucliadb/reader/reader/notifications.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/reader/tests/__init__.py
+-rw-r--r--  2.0 unx     1224 b- defN 24-May-30 15:11 nucliadb/reader/tests/conftest.py
+-rw-r--r--  2.0 unx     4345 b- defN 24-May-30 15:11 nucliadb/reader/tests/fixtures.py
+-rw-r--r--  2.0 unx     2748 b- defN 24-May-30 15:11 nucliadb/reader/tests/test_list_resources.py
+-rw-r--r--  2.0 unx    10199 b- defN 24-May-30 15:11 nucliadb/reader/tests/test_reader_file_download.py
+-rw-r--r--  2.0 unx    10586 b- defN 24-May-30 15:11 nucliadb/reader/tests/test_reader_resource.py
+-rw-r--r--  2.0 unx     6535 b- defN 24-May-30 15:11 nucliadb/reader/tests/test_reader_resource_field.py
+-rw-r--r--  2.0 unx     1535 b- defN 24-May-30 15:11 nucliadb/search/__init__.py
+-rw-r--r--  2.0 unx     4905 b- defN 24-May-30 15:11 nucliadb/search/app.py
+-rw-r--r--  2.0 unx     1956 b- defN 24-May-30 15:11 nucliadb/search/lifecycle.py
+-rw-r--r--  2.0 unx     1016 b- defN 24-May-30 15:11 nucliadb/search/openapi.py
+-rw-r--r--  2.0 unx    20665 b- defN 24-May-30 15:11 nucliadb/search/predict.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 15:11 nucliadb/search/py.typed
+-rw-r--r--  2.0 unx     1402 b- defN 24-May-30 15:11 nucliadb/search/run.py
+-rw-r--r--  2.0 unx     1193 b- defN 24-May-30 15:11 nucliadb/search/settings.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-30 15:11 nucliadb/search/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/search/api/__init__.py
+-rw-r--r--  2.0 unx     1298 b- defN 24-May-30 15:11 nucliadb/search/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3435 b- defN 24-May-30 15:11 nucliadb/search/api/v1/ask.py
+-rw-r--r--  2.0 unx     9514 b- defN 24-May-30 15:11 nucliadb/search/api/v1/chat.py
+-rw-r--r--  2.0 unx     2668 b- defN 24-May-30 15:11 nucliadb/search/api/v1/feedback.py
+-rw-r--r--  2.0 unx     8795 b- defN 24-May-30 15:11 nucliadb/search/api/v1/find.py
+-rw-r--r--  2.0 unx     6938 b- defN 24-May-30 15:11 nucliadb/search/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     3047 b- defN 24-May-30 15:11 nucliadb/search/api/v1/predict_proxy.py
+-rw-r--r--  2.0 unx      988 b- defN 24-May-30 15:11 nucliadb/search/api/v1/router.py
+-rw-r--r--  2.0 unx    19262 b- defN 24-May-30 15:11 nucliadb/search/api/v1/search.py
+-rw-r--r--  2.0 unx     5970 b- defN 24-May-30 15:11 nucliadb/search/api/v1/suggest.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-30 15:11 nucliadb/search/api/v1/summarize.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-30 15:11 nucliadb/search/api/v1/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/search/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3866 b- defN 24-May-30 15:11 nucliadb/search/api/v1/resource/ask.py
+-rw-r--r--  2.0 unx     5863 b- defN 24-May-30 15:11 nucliadb/search/api/v1/resource/chat.py
+-rw-r--r--  2.0 unx     5303 b- defN 24-May-30 15:11 nucliadb/search/api/v1/resource/search.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-30 15:11 nucliadb/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     9111 b- defN 24-May-30 15:11 nucliadb/search/requesters/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/search/search/__init__.py
+-rw-r--r--  2.0 unx     2746 b- defN 24-May-30 15:11 nucliadb/search/search/cache.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-30 15:11 nucliadb/search/search/exceptions.py
+-rw-r--r--  2.0 unx     5465 b- defN 24-May-30 15:11 nucliadb/search/search/fetch.py
+-rw-r--r--  2.0 unx     6513 b- defN 24-May-30 15:11 nucliadb/search/search/filters.py
+-rw-r--r--  2.0 unx     4612 b- defN 24-May-30 15:11 nucliadb/search/search/find.py
+-rw-r--r--  2.0 unx    17152 b- defN 24-May-30 15:11 nucliadb/search/search/find_merge.py
+-rw-r--r--  2.0 unx    21282 b- defN 24-May-30 15:11 nucliadb/search/search/merge.py
+-rw-r--r--  2.0 unx     1130 b- defN 24-May-30 15:11 nucliadb/search/search/metrics.py
+-rw-r--r--  2.0 unx     8698 b- defN 24-May-30 15:11 nucliadb/search/search/paragraphs.py
+-rw-r--r--  2.0 unx     3026 b- defN 24-May-30 15:11 nucliadb/search/search/predict_proxy.py
+-rw-r--r--  2.0 unx    31093 b- defN 24-May-30 15:11 nucliadb/search/search/query.py
+-rw-r--r--  2.0 unx     3018 b- defN 24-May-30 15:11 nucliadb/search/search/shards.py
+-rw-r--r--  2.0 unx     5101 b- defN 24-May-30 15:11 nucliadb/search/search/summarize.py
+-rw-r--r--  2.0 unx     2438 b- defN 24-May-30 15:11 nucliadb/search/search/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/search/search/chat/__init__.py
+-rw-r--r--  2.0 unx    16676 b- defN 24-May-30 15:11 nucliadb/search/search/chat/ask.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-30 15:11 nucliadb/search/search/chat/images.py
+-rw-r--r--  2.0 unx    20793 b- defN 24-May-30 15:11 nucliadb/search/search/chat/prompt.py
+-rw-r--r--  2.0 unx    17543 b- defN 24-May-30 15:11 nucliadb/search/search/chat/query.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/search/tests/__init__.py
+-rw-r--r--  2.0 unx     1295 b- defN 24-May-30 15:11 nucliadb/search/tests/conftest.py
+-rw-r--r--  2.0 unx     6578 b- defN 24-May-30 15:11 nucliadb/search/tests/fixtures.py
+-rw-r--r--  2.0 unx    15480 b- defN 24-May-30 15:11 nucliadb/search/tests/node.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/test_app.py
+-rw-r--r--  2.0 unx     3374 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/test_find_merge.py
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/test_merge.py
+-rw-r--r--  2.0 unx    15721 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/test_predict.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/test_run.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/api/__init__.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/api/v1/__init__.py
+-rw-r--r--  2.0 unx     3759 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/api/v1/test_ask.py
+-rw-r--r--  2.0 unx     2966 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/api/v1/test_chat.py
+-rw-r--r--  2.0 unx     2865 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/api/v1/test_predict_proxy.py
+-rw-r--r--  2.0 unx     2901 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/api/v1/test_summarize.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/api/v1/resource/__init__.py
+-rw-r--r--  2.0 unx     3040 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/api/v1/resource/test_chat.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/search/__init__.py
+-rw-r--r--  2.0 unx     8586 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/search/test_chat_prompt.py
+-rw-r--r--  2.0 unx     3736 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/search/test_fetch.py
+-rw-r--r--  2.0 unx     4306 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/search/test_filters.py
+-rw-r--r--  2.0 unx     4492 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/search/test_paragraphs.py
+-rw-r--r--  2.0 unx     3496 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/search/test_predict_proxy.py
+-rw-r--r--  2.0 unx     5121 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/search/test_query.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/search/requesters/__init__.py
+-rw-r--r--  2.0 unx     6455 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/search/requesters/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/search/search/__init__.py
+-rw-r--r--  2.0 unx     1759 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/search/search/test_shards.py
+-rw-r--r--  2.0 unx     2511 b- defN 24-May-30 15:11 nucliadb/search/tests/unit/search/search/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/standalone/__init__.py
+-rw-r--r--  2.0 unx     6746 b- defN 24-May-30 15:11 nucliadb/standalone/api_router.py
+-rw-r--r--  2.0 unx     5763 b- defN 24-May-30 15:11 nucliadb/standalone/app.py
+-rw-r--r--  2.0 unx     7800 b- defN 24-May-30 15:11 nucliadb/standalone/auth.py
+-rw-r--r--  2.0 unx     5313 b- defN 24-May-30 15:11 nucliadb/standalone/config.py
+-rw-r--r--  2.0 unx     6986 b- defN 24-May-30 15:11 nucliadb/standalone/introspect.py
+-rw-r--r--  2.0 unx     2488 b- defN 24-May-30 15:11 nucliadb/standalone/lifecycle.py
+-rw-r--r--  2.0 unx     1980 b- defN 24-May-30 15:11 nucliadb/standalone/migrations.py
+-rw-r--r--  2.0 unx     1322 b- defN 24-May-30 15:11 nucliadb/standalone/purge.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 15:11 nucliadb/standalone/py.typed
+-rw-r--r--  2.0 unx     5636 b- defN 24-May-30 15:11 nucliadb/standalone/run.py
+-rw-r--r--  2.0 unx     5822 b- defN 24-May-30 15:11 nucliadb/standalone/settings.py
+-rw-r--r--  2.0 unx     3132 b- defN 24-May-30 15:11 nucliadb/standalone/versions.py
+-rw-r--r--  2.0 unx     2285 b- defN 24-May-30 15:11 nucliadb/standalone/static/favicon.ico
+-rw-r--r--  2.0 unx     3833 b- defN 24-May-30 15:11 nucliadb/standalone/static/index.html
+-rw-r--r--  2.0 unx     2639 b- defN 24-May-30 15:11 nucliadb/standalone/static/logo.svg
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/standalone/tests/__init__.py
+-rw-r--r--  2.0 unx     1294 b- defN 24-May-30 15:11 nucliadb/standalone/tests/conftest.py
+-rw-r--r--  2.0 unx     1319 b- defN 24-May-30 15:11 nucliadb/standalone/tests/fixtures.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-30 15:11 nucliadb/standalone/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1722 b- defN 24-May-30 15:11 nucliadb/standalone/tests/unit/test_api_router.py
+-rw-r--r--  2.0 unx     5509 b- defN 24-May-30 15:11 nucliadb/standalone/tests/unit/test_auth.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-30 15:11 nucliadb/standalone/tests/unit/test_introspect.py
+-rw-r--r--  2.0 unx     1863 b- defN 24-May-30 15:11 nucliadb/standalone/tests/unit/test_migrations.py
+-rw-r--r--  2.0 unx     1546 b- defN 24-May-30 15:11 nucliadb/standalone/tests/unit/test_run.py
+-rw-r--r--  2.0 unx     1972 b- defN 24-May-30 15:11 nucliadb/standalone/tests/unit/test_versions.py
+-rw-r--r--  2.0 unx     1037 b- defN 24-May-30 15:11 nucliadb/tasks/__init__.py
+-rw-r--r--  2.0 unx     7655 b- defN 24-May-30 15:11 nucliadb/tasks/consumer.py
+-rw-r--r--  2.0 unx      924 b- defN 24-May-30 15:11 nucliadb/tasks/logger.py
+-rw-r--r--  2.0 unx     1378 b- defN 24-May-30 15:11 nucliadb/tasks/models.py
+-rw-r--r--  2.0 unx     3457 b- defN 24-May-30 15:11 nucliadb/tasks/producer.py
+-rw-r--r--  2.0 unx     1753 b- defN 24-May-30 15:11 nucliadb/tasks/registry.py
+-rw-r--r--  2.0 unx     1360 b- defN 24-May-30 15:11 nucliadb/tasks/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/tests/__init__.py
+-rw-r--r--  2.0 unx     1229 b- defN 24-May-30 15:11 nucliadb/tests/conftest.py
+-rw-r--r--  2.0 unx    22365 b- defN 24-May-30 15:11 nucliadb/tests/fixtures.py
+-rw-r--r--  2.0 unx     7549 b- defN 24-May-30 15:11 nucliadb/tests/tikv.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/tests/benchmarks/__init__.py
+-rw-r--r--  2.0 unx     3032 b- defN 24-May-30 15:11 nucliadb/tests/benchmarks/test_search.py
+-rw-r--r--  2.0 unx      919 b- defN 24-May-30 15:11 nucliadb/tests/knowledgeboxes/__init__.py
+-rw-r--r--  2.0 unx     7002 b- defN 24-May-30 15:11 nucliadb/tests/knowledgeboxes/philosophy_books.py
+-rw-r--r--  2.0 unx     3037 b- defN 24-May-30 15:11 nucliadb/tests/knowledgeboxes/ten_dummy_resources.py
+-rw-r--r--  2.0 unx     1148 b- defN 24-May-30 15:11 nucliadb/tests/migrations/__init__.py
+-rw-r--r--  2.0 unx     2726 b- defN 24-May-30 15:11 nucliadb/tests/migrations/test_migration_0017.py
+-rw-r--r--  2.0 unx     3662 b- defN 24-May-30 15:11 nucliadb/tests/migrations/test_migration_0018.py
+-rw-r--r--  2.0 unx     3439 b- defN 24-May-30 15:11 nucliadb/tests/migrations/test_migration_0021.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/tests/unit/__init__.py
+-rw-r--r--  2.0 unx     1487 b- defN 24-May-30 15:11 nucliadb/tests/unit/test_field_ids.py
+-rw-r--r--  2.0 unx     2780 b- defN 24-May-30 15:11 nucliadb/tests/unit/test_health.py
+-rw-r--r--  2.0 unx     1543 b- defN 24-May-30 15:11 nucliadb/tests/unit/test_kb_slugs.py
+-rw-r--r--  2.0 unx     7892 b- defN 24-May-30 15:11 nucliadb/tests/unit/test_learning_proxy.py
+-rw-r--r--  2.0 unx     2642 b- defN 24-May-30 15:11 nucliadb/tests/unit/test_metrics_exporter.py
+-rw-r--r--  2.0 unx     1341 b- defN 24-May-30 15:11 nucliadb/tests/unit/test_openapi.py
+-rw-r--r--  2.0 unx     3649 b- defN 24-May-30 15:11 nucliadb/tests/unit/test_purge.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/__init__.py
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/test_context.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/cluster/__init__.py
+-rw-r--r--  2.0 unx    12240 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/cluster/test_cluster.py
+-rw-r--r--  2.0 unx     5387 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/cluster/test_kb_shard_manager.py
+-rw-r--r--  2.0 unx     1428 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/cluster/test_rebalance.py
+-rw-r--r--  2.0 unx     9465 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/cluster/test_rollover.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/cluster/discovery/__init__.py
+-rw-r--r--  2.0 unx     5627 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/cluster/discovery/test_k8s.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/cluster/standalone/__init__.py
+-rw-r--r--  2.0 unx     3761 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/cluster/standalone/test_service.py
+-rw-r--r--  2.0 unx     2136 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/cluster/standalone/test_utils.py
+-rw-r--r--  2.0 unx      833 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/maindb/__init__.py
+-rw-r--r--  2.0 unx     3579 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/maindb/test_driver.py
+-rw-r--r--  2.0 unx     2119 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/maindb/test_tikv.py
+-rw-r--r--  2.0 unx     3213 b- defN 24-May-30 15:11 nucliadb/tests/unit/common/maindb/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/tests/unit/export_import/__init__.py
+-rw-r--r--  2.0 unx     1435 b- defN 24-May-30 15:11 nucliadb/tests/unit/export_import/test_datamanager.py
+-rw-r--r--  2.0 unx     9706 b- defN 24-May-30 15:11 nucliadb/tests/unit/export_import/test_utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/tests/unit/migrator/__init__.py
+-rw-r--r--  2.0 unx     3233 b- defN 24-May-30 15:11 nucliadb/tests/unit/migrator/test_migrator.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/tests/unit/tasks/__init__.py
+-rw-r--r--  2.0 unx     1375 b- defN 24-May-30 15:11 nucliadb/tests/unit/tasks/conftest.py
+-rw-r--r--  2.0 unx     2714 b- defN 24-May-30 15:11 nucliadb/tests/unit/tasks/test_consumer.py
+-rw-r--r--  2.0 unx     3189 b- defN 24-May-30 15:11 nucliadb/tests/unit/tasks/test_producer.py
+-rw-r--r--  2.0 unx     1827 b- defN 24-May-30 15:11 nucliadb/tests/unit/tasks/test_tasks.py
+-rw-r--r--  2.0 unx     2507 b- defN 24-May-30 15:11 nucliadb/tests/utils/__init__.py
+-rw-r--r--  2.0 unx     1797 b- defN 24-May-30 15:11 nucliadb/tests/utils/aiohttp_session.py
+-rw-r--r--  2.0 unx     2533 b- defN 24-May-30 15:11 nucliadb/tests/utils/entities.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-May-30 15:11 nucliadb/tests/utils/broker_messages/__init__.py
+-rw-r--r--  2.0 unx     7557 b- defN 24-May-30 15:11 nucliadb/tests/utils/broker_messages/fields.py
+-rw-r--r--  2.0 unx     1196 b- defN 24-May-30 15:11 nucliadb/tests/utils/broker_messages/helpers.py
+-rw-r--r--  2.0 unx     1325 b- defN 24-May-30 15:11 nucliadb/train/__init__.py
+-rw-r--r--  2.0 unx     3530 b- defN 24-May-30 15:11 nucliadb/train/app.py
+-rw-r--r--  2.0 unx     3800 b- defN 24-May-30 15:11 nucliadb/train/generator.py
+-rw-r--r--  2.0 unx     1698 b- defN 24-May-30 15:11 nucliadb/train/lifecycle.py
+-rw-r--r--  2.0 unx     1198 b- defN 24-May-30 15:11 nucliadb/train/models.py
+-rw-r--r--  2.0 unx     5706 b- defN 24-May-30 15:11 nucliadb/train/nodes.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 15:11 nucliadb/train/py.typed
+-rw-r--r--  2.0 unx     1400 b- defN 24-May-30 15:11 nucliadb/train/run.py
+-rw-r--r--  2.0 unx     5926 b- defN 24-May-30 15:11 nucliadb/train/servicer.py
+-rw-r--r--  2.0 unx     1415 b- defN 24-May-30 15:11 nucliadb/train/settings.py
+-rw-r--r--  2.0 unx     1496 b- defN 24-May-30 15:11 nucliadb/train/types.py
+-rw-r--r--  2.0 unx     3265 b- defN 24-May-30 15:11 nucliadb/train/upload.py
+-rw-r--r--  2.0 unx     6420 b- defN 24-May-30 15:11 nucliadb/train/uploader.py
+-rw-r--r--  2.0 unx     3179 b- defN 24-May-30 15:11 nucliadb/train/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/train/api/__init__.py
+-rw-r--r--  2.0 unx     1479 b- defN 24-May-30 15:11 nucliadb/train/api/utils.py
+-rw-r--r--  2.0 unx      928 b- defN 24-May-30 15:11 nucliadb/train/api/v1/__init__.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-May-30 15:11 nucliadb/train/api/v1/check.py
+-rw-r--r--  2.0 unx      910 b- defN 24-May-30 15:11 nucliadb/train/api/v1/router.py
+-rw-r--r--  2.0 unx     1908 b- defN 24-May-30 15:11 nucliadb/train/api/v1/shards.py
+-rw-r--r--  2.0 unx     2135 b- defN 24-May-30 15:11 nucliadb/train/api/v1/trainset.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/train/generators/__init__.py
+-rw-r--r--  2.0 unx     3723 b- defN 24-May-30 15:11 nucliadb/train/generators/field_classifier.py
+-rw-r--r--  2.0 unx     6712 b- defN 24-May-30 15:11 nucliadb/train/generators/image_classifier.py
+-rw-r--r--  2.0 unx     2789 b- defN 24-May-30 15:11 nucliadb/train/generators/paragraph_classifier.py
+-rw-r--r--  2.0 unx     3590 b- defN 24-May-30 15:11 nucliadb/train/generators/paragraph_streaming.py
+-rw-r--r--  2.0 unx     5372 b- defN 24-May-30 15:11 nucliadb/train/generators/question_answer_streaming.py
+-rw-r--r--  2.0 unx     5160 b- defN 24-May-30 15:11 nucliadb/train/generators/sentence_classifier.py
+-rw-r--r--  2.0 unx    10446 b- defN 24-May-30 15:11 nucliadb/train/generators/token_classifier.py
+-rw-r--r--  2.0 unx     3877 b- defN 24-May-30 15:11 nucliadb/train/generators/utils.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/train/tests/__init__.py
+-rw-r--r--  2.0 unx     1125 b- defN 24-May-30 15:11 nucliadb/train/tests/conftest.py
+-rw-r--r--  2.0 unx    11053 b- defN 24-May-30 15:11 nucliadb/train/tests/fixtures.py
+-rw-r--r--  2.0 unx     4598 b- defN 24-May-30 15:11 nucliadb/train/tests/test_field_classification.py
+-rw-r--r--  2.0 unx     2729 b- defN 24-May-30 15:11 nucliadb/train/tests/test_get_entities.py
+-rw-r--r--  2.0 unx     1660 b- defN 24-May-30 15:11 nucliadb/train/tests/test_get_info.py
+-rw-r--r--  2.0 unx     1382 b- defN 24-May-30 15:11 nucliadb/train/tests/test_get_ontology.py
+-rw-r--r--  2.0 unx     2201 b- defN 24-May-30 15:11 nucliadb/train/tests/test_get_ontology_count.py
+-rw-r--r--  2.0 unx     7669 b- defN 24-May-30 15:11 nucliadb/train/tests/test_image_classification.py
+-rw-r--r--  2.0 unx     1416 b- defN 24-May-30 15:11 nucliadb/train/tests/test_list_fields.py
+-rw-r--r--  2.0 unx     2944 b- defN 24-May-30 15:11 nucliadb/train/tests/test_list_paragraphs.py
+-rw-r--r--  2.0 unx     1423 b- defN 24-May-30 15:11 nucliadb/train/tests/test_list_resources.py
+-rw-r--r--  2.0 unx     2947 b- defN 24-May-30 15:11 nucliadb/train/tests/test_list_sentences.py
+-rw-r--r--  2.0 unx     4645 b- defN 24-May-30 15:11 nucliadb/train/tests/test_paragraph_classification.py
+-rw-r--r--  2.0 unx     4320 b- defN 24-May-30 15:11 nucliadb/train/tests/test_paragraph_streaming.py
+-rw-r--r--  2.0 unx     8751 b- defN 24-May-30 15:11 nucliadb/train/tests/test_question_answer_streaming.py
+-rw-r--r--  2.0 unx     5051 b- defN 24-May-30 15:11 nucliadb/train/tests/test_sentence_classification.py
+-rw-r--r--  2.0 unx     5583 b- defN 24-May-30 15:11 nucliadb/train/tests/test_token_classification.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-30 15:11 nucliadb/train/tests/utils.py
+-rw-r--r--  2.0 unx     1328 b- defN 24-May-30 15:11 nucliadb/writer/__init__.py
+-rw-r--r--  2.0 unx     4268 b- defN 24-May-30 15:11 nucliadb/writer/app.py
+-rw-r--r--  2.0 unx    19483 b- defN 24-May-30 15:11 nucliadb/writer/back_pressure.py
+-rw-r--r--  2.0 unx      972 b- defN 24-May-30 15:11 nucliadb/writer/exceptions.py
+-rw-r--r--  2.0 unx     1953 b- defN 24-May-30 15:11 nucliadb/writer/lifecycle.py
+-rw-r--r--  2.0 unx     1032 b- defN 24-May-30 15:11 nucliadb/writer/openapi.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-30 15:11 nucliadb/writer/py.typed
+-rw-r--r--  2.0 unx     1448 b- defN 24-May-30 15:11 nucliadb/writer/run.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-30 15:11 nucliadb/writer/settings.py
+-rw-r--r--  2.0 unx     1036 b- defN 24-May-30 15:11 nucliadb/writer/utilities.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/writer/api/__init__.py
+-rw-r--r--  2.0 unx     1429 b- defN 24-May-30 15:11 nucliadb/writer/api/constants.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-May-30 15:11 nucliadb/writer/api/v1/__init__.py
+-rw-r--r--  2.0 unx     6421 b- defN 24-May-30 15:11 nucliadb/writer/api/v1/export_import.py
+-rw-r--r--  2.0 unx    24482 b- defN 24-May-30 15:11 nucliadb/writer/api/v1/field.py
+-rw-r--r--  2.0 unx     5248 b- defN 24-May-30 15:11 nucliadb/writer/api/v1/knowledgebox.py
+-rw-r--r--  2.0 unx     2058 b- defN 24-May-30 15:11 nucliadb/writer/api/v1/learning_config.py
+-rw-r--r--  2.0 unx    18628 b- defN 24-May-30 15:11 nucliadb/writer/api/v1/resource.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-30 15:11 nucliadb/writer/api/v1/router.py
+-rw-r--r--  2.0 unx    10216 b- defN 24-May-30 15:11 nucliadb/writer/api/v1/services.py
+-rw-r--r--  2.0 unx    30985 b- defN 24-May-30 15:11 nucliadb/writer/api/v1/upload.py
+-rw-r--r--  2.0 unx     1612 b- defN 24-May-30 15:11 nucliadb/writer/layouts/__init__.py
+-rw-r--r--  2.0 unx     2115 b- defN 24-May-30 15:11 nucliadb/writer/layouts/v1.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/writer/resource/__init__.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-May-30 15:11 nucliadb/writer/resource/audit.py
+-rw-r--r--  2.0 unx    10968 b- defN 24-May-30 15:11 nucliadb/writer/resource/basic.py
+-rw-r--r--  2.0 unx    16740 b- defN 24-May-30 15:11 nucliadb/writer/resource/field.py
+-rw-r--r--  2.0 unx     2022 b- defN 24-May-30 15:11 nucliadb/writer/resource/origin.py
+-rw-r--r--  2.0 unx      835 b- defN 24-May-30 15:11 nucliadb/writer/tests/__init__.py
+-rw-r--r--  2.0 unx     1200 b- defN 24-May-30 15:11 nucliadb/writer/tests/conftest.py
+-rw-r--r--  2.0 unx     5971 b- defN 24-May-30 15:11 nucliadb/writer/tests/fixtures.py
+-rw-r--r--  2.0 unx    15472 b- defN 24-May-30 15:11 nucliadb/writer/tests/test_fields.py
+-rw-r--r--  2.0 unx    25999 b- defN 24-May-30 15:11 nucliadb/writer/tests/test_files.py
+-rw-r--r--  2.0 unx     1729 b- defN 24-May-30 15:11 nucliadb/writer/tests/test_knowledgebox.py
+-rw-r--r--  2.0 unx     4400 b- defN 24-May-30 15:11 nucliadb/writer/tests/test_reprocess_file_field.py
+-rw-r--r--  2.0 unx    16857 b- defN 24-May-30 15:11 nucliadb/writer/tests/test_resources.py
+-rw-r--r--  2.0 unx     5120 b- defN 24-May-30 15:11 nucliadb/writer/tests/test_service.py
+-rw-r--r--  2.0 unx     6054 b- defN 24-May-30 15:11 nucliadb/writer/tests/test_tus.py
+-rw-r--r--  2.0 unx     1287 b- defN 24-May-30 15:11 nucliadb/writer/tests/utils.py
+-rw-r--r--  2.0 unx     5226 b- defN 24-May-30 15:11 nucliadb/writer/tus/__init__.py
+-rw-r--r--  2.0 unx     5082 b- defN 24-May-30 15:11 nucliadb/writer/tus/dm.py
+-rw-r--r--  2.0 unx     2186 b- defN 24-May-30 15:11 nucliadb/writer/tus/exceptions.py
+-rw-r--r--  2.0 unx    14527 b- defN 24-May-30 15:11 nucliadb/writer/tus/gcs.py
+-rw-r--r--  2.0 unx     5849 b- defN 24-May-30 15:11 nucliadb/writer/tus/local.py
+-rw-r--r--  2.0 unx     4367 b- defN 24-May-30 15:11 nucliadb/writer/tus/pg.py
+-rw-r--r--  2.0 unx     9069 b- defN 24-May-30 15:11 nucliadb/writer/tus/s3.py
+-rw-r--r--  2.0 unx     4734 b- defN 24-May-30 15:11 nucliadb/writer/tus/storage.py
+-rw-r--r--  2.0 unx     2556 b- defN 24-May-30 15:11 nucliadb/writer/tus/utils.py
+-rw-r--r--  2.0 unx     4474 b- defN 24-May-30 15:13 nucliadb-4.0.3.post561.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 15:13 nucliadb-4.0.3.post561.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1268 b- defN 24-May-30 15:13 nucliadb-4.0.3.post561.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 24-May-30 15:13 nucliadb-4.0.3.post561.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-30 15:13 nucliadb-4.0.3.post561.dist-info/zip-safe
+-rw-rw-r--  2.0 unx    44141 b- defN 24-May-30 15:13 nucliadb-4.0.3.post561.dist-info/RECORD
+471 files, 2278602 bytes uncompressed, 700853 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -1389,26 +1389,26 @@
 
 Filename: nucliadb/writer/tus/storage.py
 Comment: 
 
 Filename: nucliadb/writer/tus/utils.py
 Comment: 
 
-Filename: nucliadb-4.0.3.post560.dist-info/METADATA
+Filename: nucliadb-4.0.3.post561.dist-info/METADATA
 Comment: 
 
-Filename: nucliadb-4.0.3.post560.dist-info/WHEEL
+Filename: nucliadb-4.0.3.post561.dist-info/WHEEL
 Comment: 
 
-Filename: nucliadb-4.0.3.post560.dist-info/entry_points.txt
+Filename: nucliadb-4.0.3.post561.dist-info/entry_points.txt
 Comment: 
 
-Filename: nucliadb-4.0.3.post560.dist-info/top_level.txt
+Filename: nucliadb-4.0.3.post561.dist-info/top_level.txt
 Comment: 
 
-Filename: nucliadb-4.0.3.post560.dist-info/zip-safe
+Filename: nucliadb-4.0.3.post561.dist-info/zip-safe
 Comment: 
 
-Filename: nucliadb-4.0.3.post560.dist-info/RECORD
+Filename: nucliadb-4.0.3.post561.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nucliadb/ingest/orm/knowledgebox.py

```diff
@@ -57,16 +57,16 @@
 
 KB_TO_DELETE_BASE = "/kbtodelete/"
 KB_TO_DELETE_STORAGE_BASE = "/storagetodelete/"
 
 KB_TO_DELETE = f"{KB_TO_DELETE_BASE}{{kbid}}"
 KB_TO_DELETE_STORAGE = f"{KB_TO_DELETE_STORAGE_BASE}{{kbid}}"
 
-KB_VECTORSET_TO_DELETE_BASE = "/kbvectorsettodelete"
-KB_VECTORSET_TO_DELETE = f"{KB_VECTORSET_TO_DELETE_BASE}/{{kbid}}"
+KB_VECTORSET_TO_DELETE_BASE = "/vectorsettodelete"
+KB_VECTORSET_TO_DELETE = f"{KB_VECTORSET_TO_DELETE_BASE}/{{kbid}}/{{vectorset}}"
 
 
 class KnowledgeBox:
     def __init__(self, txn: Transaction, storage: Storage, kbid: str):
         self.txn = txn
         self.storage = storage
         self.kbid = kbid
@@ -431,15 +431,17 @@
         await shard_manager.create_vectorset(self.kbid, config)
 
     async def delete_vectorset(self, vectorset_id: str):
         await datamanagers.vectorsets.delete(
             self.txn, kbid=self.kbid, vectorset_id=vectorset_id
         )
         # mark vectorset for async deletion
-        await self.txn.set(KB_VECTORSET_TO_DELETE.format(kbid=self.kbid), b"")
+        await self.txn.set(
+            KB_VECTORSET_TO_DELETE.format(kbid=self.kbid, vectorset=vectorset_id), b""
+        )
         shard_manager = get_shard_manager()
         await shard_manager.delete_vectorset(self.kbid, vectorset_id)
 
 
 def chunker(seq: Sequence, size: int):
     return (seq[pos : pos + size] for pos in range(0, len(seq), size))
```

## Comparing `nucliadb-4.0.3.post560.dist-info/METADATA` & `nucliadb-4.0.3.post561.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nucliadb
-Version: 4.0.3.post560
+Version: 4.0.3.post561
 Home-page: https://docs.nuclia.dev/docs/guides/nucliadb/intro
 Author: NucliaDB Community
 Author-email: nucliadb@nuclia.com
 License: BSD
 Project-URL: Nuclia, https://nuclia.com
 Project-URL: Github, https://github.com/nuclia/nucliadb
 Project-URL: Discord, https://discord.gg/8EvQwmsbzf
@@ -18,18 +18,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9, <4
 Description-Content-Type: text/markdown
-Requires-Dist: nucliadb-telemetry[all] >=4.0.3.post560
-Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.3.post560
-Requires-Dist: nucliadb-protos >=4.0.3.post560
-Requires-Dist: nucliadb-models >=4.0.3.post560
+Requires-Dist: nucliadb-telemetry[all] >=4.0.3.post561
+Requires-Dist: nucliadb-utils[cache,fastapi,storages] >=4.0.3.post561
+Requires-Dist: nucliadb-protos >=4.0.3.post561
+Requires-Dist: nucliadb-models >=4.0.3.post561
 Requires-Dist: nucliadb-admin-assets >=1.0.0.post1224
 Requires-Dist: nucliadb-node-binding >=2.26.0
 Requires-Dist: uvicorn <0.19.0
 Requires-Dist: argdantic
 Requires-Dist: aiohttp >=3.9.4
 Requires-Dist: lru-dict >=1.1.7
 Requires-Dist: backoff
```

## Comparing `nucliadb-4.0.3.post560.dist-info/entry_points.txt` & `nucliadb-4.0.3.post561.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `nucliadb-4.0.3.post560.dist-info/RECORD` & `nucliadb-4.0.3.post561.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
 nucliadb/ingest/fields/layout.py,sha256=clgBVGWArtkAEawDqCAu_hB9gVu5c6UT1Cf_5yrw47s,2250
 nucliadb/ingest/fields/link.py,sha256=kwV3KxSn6bZNYBBHljMEN9qNXPlNv80guoKqQib8ivc,4212
 nucliadb/ingest/fields/text.py,sha256=qMMH76gN--Ag1fPZ1I5G9ZPAi4U0i9jbqlrpYc3cMxg,1319
 nucliadb/ingest/orm/__init__.py,sha256=cp15ZcFnHvpcu_5-aK2A4uUyvuZVV_MJn4bIXMa20ks,835
 nucliadb/ingest/orm/brain.py,sha256=qayvpXdkR_Hq7tw7UmDK8-BH-vFNuRdmkW2EWyk1lLs,28311
 nucliadb/ingest/orm/entities.py,sha256=q027LfocE-KIqRNC1ZOSrrvt6x9NGrB25TZsOe0SyVk,15758
 nucliadb/ingest/orm/exceptions.py,sha256=Wv10JwvueWrSV0ExqSTFIq_mBXWz4rAelEdc1R5w0Q0,1326
-nucliadb/ingest/orm/knowledgebox.py,sha256=RuBdnyu74sGZT0fcxwiaKUJm1jdqz4lNfvU0QVETpLw,16750
+nucliadb/ingest/orm/knowledgebox.py,sha256=LKRWdaypY5IhBVsw27Xy_rEPL04yT9kE_Ajqn-ud-Eg,16808
 nucliadb/ingest/orm/metrics.py,sha256=OkwMSPKLZcKba0ZTwtTiIxwBgaLMX5ydhGieKvi2y7E,1096
 nucliadb/ingest/orm/resource.py,sha256=vIpyFpftCgj4sBi5FfRlTLOxJnBuG57uyYH4DK0p6U4,58955
 nucliadb/ingest/orm/utils.py,sha256=A3_EsRw7Nub54qZPF08cv391caxpLQWJURR0_5qP9mU,2685
 nucliadb/ingest/orm/processor/__init__.py,sha256=SqX421XJs_g-sRNSzdv9EyWQGUUceSs6U4LllvUEzCA,27092
 nucliadb/ingest/orm/processor/auditing.py,sha256=M8YLnqEJMCvjYATqIRQS2KpJyhyxxoZvBfpxxppKGOI,5090
 nucliadb/ingest/orm/processor/sequence_manager.py,sha256=Mc9SA_NfzxTwovD5yGiAcdmen4pa-QNdsYcONIWeZPc,1690
 nucliadb/ingest/service/__init__.py,sha256=C_lkkjoHm0hDT2fZjEN4mpwXtU4bWthB-vM5-28-MBM,2057
@@ -459,13 +459,13 @@
 nucliadb/writer/tus/exceptions.py,sha256=CmxYKnHXpXug25DYV4SpVAU47SGD-NVBd7pNTRbWHyk,2186
 nucliadb/writer/tus/gcs.py,sha256=WykJZicWKRYkVB5_Fkb_1cVLovAk86IVkEn1VgEDufc,14527
 nucliadb/writer/tus/local.py,sha256=lIOoGaylnsxPBYGskcmKSHv7MsvwIYFS4soDLey_KSs,5849
 nucliadb/writer/tus/pg.py,sha256=JUK_xKsyNcKAvWOch8gUMTc_e1evI_3aC6-Y5gMk2jw,4367
 nucliadb/writer/tus/s3.py,sha256=a9mfPtjBW3QaTYY2r6P7u_Y13V6mBefZjWgV4juZzgE,9069
 nucliadb/writer/tus/storage.py,sha256=8iBOjWIcY6PawQq_rmSiBKi0Gl6J6Q5ad6L-9nLCcJ4,4734
 nucliadb/writer/tus/utils.py,sha256=MSdVbRsRSZVdkaum69_0wku7X3p5wlZf4nr6E0GMKbw,2556
-nucliadb-4.0.3.post560.dist-info/METADATA,sha256=84GF6yh_vX2OEV6JtqPmMDFNjsolRDDQ-xmFYpW8sbI,4474
-nucliadb-4.0.3.post560.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-nucliadb-4.0.3.post560.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
-nucliadb-4.0.3.post560.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
-nucliadb-4.0.3.post560.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-nucliadb-4.0.3.post560.dist-info/RECORD,,
+nucliadb-4.0.3.post561.dist-info/METADATA,sha256=5D3Ve7Y4AAQsx6zGEWWxO-jcpmqETVqaYq5xlXhp6vg,4474
+nucliadb-4.0.3.post561.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+nucliadb-4.0.3.post561.dist-info/entry_points.txt,sha256=XqGfgFDuY3zXQc8ewXM2TRVjTModIq851zOsgrmaXx4,1268
+nucliadb-4.0.3.post561.dist-info/top_level.txt,sha256=hwYhTVnX7jkQ9gJCkVrbqEG1M4lT2F_iPQND1fCzF80,20
+nucliadb-4.0.3.post561.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+nucliadb-4.0.3.post561.dist-info/RECORD,,
```

