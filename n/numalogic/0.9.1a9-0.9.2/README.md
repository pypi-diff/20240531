# Comparing `tmp/numalogic-0.9.1a9.tar.gz` & `tmp/numalogic-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic-0.9.1a9.tar", max compression
+gzip compressed data, was "numalogic-0.9.2.tar", max compression
```

## Comparing `numalogic-0.9.1a9.tar` & `numalogic-0.9.2.tar`

### file list

```diff
@@ -1,106 +1,106 @@
--rw-r--r--   0        0        0    11357 2024-05-03 22:36:58.388312 numalogic-0.9.1a9/LICENSE
--rw-r--r--   0        0        0     5244 2024-05-03 22:36:58.388312 numalogic-0.9.1a9/README.md
--rw-r--r--   0        0        0      676 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/__init__.py
--rw-r--r--   0        0        0     1016 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/_constants.py
--rw-r--r--   0        0        0      413 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/backtest/__init__.py
--rw-r--r--   0        0        0      248 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/backtest/_constants.py
--rw-r--r--   0        0        0    16031 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/backtest/_prom.py
--rw-r--r--   0        0        0     1636 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/base.py
--rw-r--r--   0        0        0     1102 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/blocks/__init__.py
--rw-r--r--   0        0        0     4672 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/blocks/_base.py
--rw-r--r--   0        0        0     3229 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/blocks/_nn.py
--rw-r--r--   0        0        0     3906 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/blocks/_transform.py
--rw-r--r--   0        0        0     5776 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/blocks/pipeline.py
--rw-r--r--   0        0        0     1271 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/config/__init__.py
--rw-r--r--   0        0        0     4828 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/config/_config.py
--rw-r--r--   0        0        0     7543 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/config/factory.py
--rw-r--r--   0        0        0      550 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/connectors/__init__.py
--rw-r--r--   0        0        0      689 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/connectors/_base.py
--rw-r--r--   0        0        0     1890 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/connectors/_config.py
--rw-r--r--   0        0        0      157 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/connectors/druid/__init__.py
--rw-r--r--   0        0        0    11185 2024-05-03 22:36:58.408312 numalogic-0.9.1a9/numalogic/connectors/druid/_druid.py
--rw-r--r--   0        0        0      765 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/druid/aggregators.py
--rw-r--r--   0        0        0      696 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/druid/postaggregator.py
--rw-r--r--   0        0        0    10150 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/prometheus.py
--rw-r--r--   0        0        0       79 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/rds/__init__.py
--rw-r--r--   0        0        0     5022 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/rds/_base.py
--rw-r--r--   0        0        0     2608 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/rds/_rds.py
--rw-r--r--   0        0        0        0 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/rds/db/__init__.py
--rw-r--r--   0        0        0     1061 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/rds/db/factory.py
--rw-r--r--   0        0        0     4193 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/rds/db/mysql_fetcher.py
--rw-r--r--   0        0        0     2734 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/redis.py
--rw-r--r--   0        0        0        0 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/utils/aws/__init__.py
--rw-r--r--   0        0        0     5637 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/utils/aws/boto3_client_manager.py
--rw-r--r--   0        0        0     4636 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/utils/aws/config.py
--rw-r--r--   0        0        0     1265 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/utils/aws/db_configurations.py
--rw-r--r--   0        0        0     1738 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/utils/aws/exceptions.py
--rw-r--r--   0        0        0     3346 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/utils/aws/sts_client_manager.py
--rw-r--r--   0        0        0     2181 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/connectors/utils/enum.py
--rw-r--r--   0        0        0        0 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/__init__.py
--rw-r--r--   0        0        0      668 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/autoencoder/__init__.py
--rw-r--r--   0        0        0     3419 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/autoencoder/base.py
--rw-r--r--   0        0        0      581 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/autoencoder/variants/__init__.py
--rw-r--r--   0        0        0    11705 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/autoencoder/variants/conv.py
--rw-r--r--   0        0        0     6599 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/autoencoder/variants/lstm.py
--rw-r--r--   0        0        0    14335 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/autoencoder/variants/transformer.py
--rw-r--r--   0        0        0     8562 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/autoencoder/variants/vanilla.py
--rw-r--r--   0        0        0        0 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/forecast/__init__.py
--rw-r--r--   0        0        0      158 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/forecast/variants/__init__.py
--rw-r--r--   0        0        0     4289 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/forecast/variants/naive.py
--rw-r--r--   0        0        0      489 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/threshold/__init__.py
--rw-r--r--   0        0        0     7531 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/threshold/_mahalanobis.py
--rw-r--r--   0        0        0     2943 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/threshold/_median.py
--rw-r--r--   0        0        0     4720 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/threshold/_static.py
--rw-r--r--   0        0        0     2462 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/threshold/_std.py
--rw-r--r--   0        0        0       77 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/vae/__init__.py
--rw-r--r--   0        0        0     2046 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/vae/base.py
--rw-r--r--   0        0        0     1536 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/vae/layer.py
--rw-r--r--   0        0        0       82 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/vae/variants/__init__.py
--rw-r--r--   0        0        0     7916 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/models/vae/variants/conv.py
--rw-r--r--   0        0        0      975 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/monitoring/__init__.py
--rw-r--r--   0        0        0     3906 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/monitoring/metrics.py
--rw-r--r--   0        0        0     1282 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/registry/__init__.py
--rw-r--r--   0        0        0      651 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/registry/_serialize.py
--rw-r--r--   0        0        0     6734 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/registry/artifact.py
--rw-r--r--   0        0        0    15564 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/registry/dynamodb_registry.py
--rw-r--r--   0        0        0     3334 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/registry/localcache.py
--rw-r--r--   0        0        0    13536 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/registry/mlflow_registry.py
--rw-r--r--   0        0        0    16600 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/registry/redis_registry.py
--rw-r--r--   0        0        0      841 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/synthetic/__init__.py
--rw-r--r--   0        0        0    12457 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/synthetic/anomalies.py
--rw-r--r--   0        0        0     1637 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/synthetic/sparsity.py
--rw-r--r--   0        0        0     4739 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/synthetic/timeseries.py
--rw-r--r--   0        0        0        0 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/tools/__init__.py
--rw-r--r--   0        0        0      631 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/tools/aggregators.py
--rw-r--r--   0        0        0     3615 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/tools/callbacks.py
--rw-r--r--   0        0        0    10279 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/tools/data.py
--rw-r--r--   0        0        0     2545 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/tools/exceptions.py
--rw-r--r--   0        0        0     3168 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/tools/trainer.py
--rw-r--r--   0        0        0     2237 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/tools/types.py
--rw-r--r--   0        0        0     1418 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/transforms/__init__.py
--rw-r--r--   0        0        0     4006 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/transforms/_movavg.py
--rw-r--r--   0        0        0     2252 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/transforms/_postprocess.py
--rw-r--r--   0        0        0     4772 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/transforms/_scaler.py
--rw-r--r--   0        0        0     5178 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/transforms/_stateless.py
--rw-r--r--   0        0        0     3560 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/udfs/README.md
--rw-r--r--   0        0        0     1232 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/udfs/__init__.py
--rw-r--r--   0        0        0     1937 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/udfs/__main__.py
--rw-r--r--   0        0        0     5192 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/udfs/_base.py
--rw-r--r--   0        0        0     3711 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/udfs/_config.py
--rw-r--r--   0        0        0     1060 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/udfs/_logger.py
--rw-r--r--   0        0        0     4923 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/udfs/_metrics.py
--rw-r--r--   0        0        0     3376 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/udfs/entities.py
--rw-r--r--   0        0        0     4298 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/udfs/factory.py
--rw-r--r--   0        0        0     7317 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/udfs/inference.py
--rw-r--r--   0        0        0     2196 2024-05-03 22:36:58.412313 numalogic-0.9.1a9/numalogic/udfs/payloadtx.py
--rw-r--r--   0        0        0    15964 2024-05-03 22:36:58.416313 numalogic-0.9.1a9/numalogic/udfs/postprocess.py
--rw-r--r--   0        0        0     9286 2024-05-03 22:36:58.416313 numalogic-0.9.1a9/numalogic/udfs/preprocess.py
--rw-r--r--   0        0        0     5581 2024-05-03 22:36:58.416313 numalogic-0.9.1a9/numalogic/udfs/staticthresh.py
--rw-r--r--   0        0        0    14920 2024-05-03 22:36:58.416313 numalogic-0.9.1a9/numalogic/udfs/tools.py
--rw-r--r--   0        0        0      229 2024-05-03 22:36:58.416313 numalogic-0.9.1a9/numalogic/udfs/trainer/__init__.py
--rw-r--r--   0        0        0    14056 2024-05-03 22:36:58.416313 numalogic-0.9.1a9/numalogic/udfs/trainer/_base.py
--rw-r--r--   0        0        0     5248 2024-05-03 22:36:58.416313 numalogic-0.9.1a9/numalogic/udfs/trainer/_druid.py
--rw-r--r--   0        0        0     3816 2024-05-03 22:36:58.416313 numalogic-0.9.1a9/numalogic/udfs/trainer/_prom.py
--rw-r--r--   0        0        0     3032 2024-05-03 22:36:58.416313 numalogic-0.9.1a9/pyproject.toml
--rw-r--r--   0        0        0     6954 1970-01-01 00:00:00.000000 numalogic-0.9.1a9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-06 21:28:57.544693 numalogic-0.9.2/LICENSE
+-rw-r--r--   0        0        0     5244 2024-05-06 21:28:57.544693 numalogic-0.9.2/README.md
+-rw-r--r--   0        0        0      676 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/__init__.py
+-rw-r--r--   0        0        0     1016 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/_constants.py
+-rw-r--r--   0        0        0      413 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/backtest/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/backtest/_constants.py
+-rw-r--r--   0        0        0    15499 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/backtest/_prom.py
+-rw-r--r--   0        0        0     1636 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/base.py
+-rw-r--r--   0        0        0     1102 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/blocks/__init__.py
+-rw-r--r--   0        0        0     4672 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/blocks/_base.py
+-rw-r--r--   0        0        0     3229 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/blocks/_nn.py
+-rw-r--r--   0        0        0     3906 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/blocks/_transform.py
+-rw-r--r--   0        0        0     5776 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/blocks/pipeline.py
+-rw-r--r--   0        0        0     1271 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/config/__init__.py
+-rw-r--r--   0        0        0     4818 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/config/_config.py
+-rw-r--r--   0        0        0     7327 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/config/factory.py
+-rw-r--r--   0        0        0      550 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/__init__.py
+-rw-r--r--   0        0        0      689 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/_base.py
+-rw-r--r--   0        0        0     1709 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/_config.py
+-rw-r--r--   0        0        0      157 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/druid/__init__.py
+-rw-r--r--   0        0        0     9647 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/druid/_druid.py
+-rw-r--r--   0        0        0      765 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/druid/aggregators.py
+-rw-r--r--   0        0        0      696 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/druid/postaggregator.py
+-rw-r--r--   0        0        0    10150 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/prometheus.py
+-rw-r--r--   0        0        0       79 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/rds/__init__.py
+-rw-r--r--   0        0        0     5022 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/rds/_base.py
+-rw-r--r--   0        0        0     2608 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/rds/_rds.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/rds/db/__init__.py
+-rw-r--r--   0        0        0     1061 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/rds/db/factory.py
+-rw-r--r--   0        0        0     4193 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/rds/db/mysql_fetcher.py
+-rw-r--r--   0        0        0     2734 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/redis.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/utils/aws/__init__.py
+-rw-r--r--   0        0        0     5637 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/utils/aws/boto3_client_manager.py
+-rw-r--r--   0        0        0     4636 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/utils/aws/config.py
+-rw-r--r--   0        0        0     1265 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/utils/aws/db_configurations.py
+-rw-r--r--   0        0        0     1738 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/utils/aws/exceptions.py
+-rw-r--r--   0        0        0     3346 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/utils/aws/sts_client_manager.py
+-rw-r--r--   0        0        0     2181 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/connectors/utils/enum.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/models/__init__.py
+-rw-r--r--   0        0        0      668 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/models/autoencoder/__init__.py
+-rw-r--r--   0        0        0     3419 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/models/autoencoder/base.py
+-rw-r--r--   0        0        0      581 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/models/autoencoder/variants/__init__.py
+-rw-r--r--   0        0        0    11705 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/models/autoencoder/variants/conv.py
+-rw-r--r--   0        0        0     6599 2024-05-06 21:28:57.564693 numalogic-0.9.2/numalogic/models/autoencoder/variants/lstm.py
+-rw-r--r--   0        0        0    14335 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/models/autoencoder/variants/transformer.py
+-rw-r--r--   0        0        0     8420 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/models/autoencoder/variants/vanilla.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/models/forecast/__init__.py
+-rw-r--r--   0        0        0      158 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/models/forecast/variants/__init__.py
+-rw-r--r--   0        0        0     4289 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/models/forecast/variants/naive.py
+-rw-r--r--   0        0        0      489 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/models/threshold/__init__.py
+-rw-r--r--   0        0        0     7531 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/models/threshold/_mahalanobis.py
+-rw-r--r--   0        0        0     2119 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/models/threshold/_median.py
+-rw-r--r--   0        0        0     4720 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/models/threshold/_static.py
+-rw-r--r--   0        0        0     2462 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/models/threshold/_std.py
+-rw-r--r--   0        0        0       77 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/models/vae/__init__.py
+-rw-r--r--   0        0        0     2046 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/models/vae/base.py
+-rw-r--r--   0        0        0     1536 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/models/vae/layer.py
+-rw-r--r--   0        0        0       82 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/models/vae/variants/__init__.py
+-rw-r--r--   0        0        0     7916 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/models/vae/variants/conv.py
+-rw-r--r--   0        0        0      975 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/monitoring/__init__.py
+-rw-r--r--   0        0        0     3906 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/monitoring/metrics.py
+-rw-r--r--   0        0        0     1282 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/registry/__init__.py
+-rw-r--r--   0        0        0      651 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/registry/_serialize.py
+-rw-r--r--   0        0        0     6734 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/registry/artifact.py
+-rw-r--r--   0        0        0    15564 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/registry/dynamodb_registry.py
+-rw-r--r--   0        0        0     3334 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/registry/localcache.py
+-rw-r--r--   0        0        0    13536 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/registry/mlflow_registry.py
+-rw-r--r--   0        0        0    16600 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/registry/redis_registry.py
+-rw-r--r--   0        0        0      841 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/synthetic/__init__.py
+-rw-r--r--   0        0        0    12457 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/synthetic/anomalies.py
+-rw-r--r--   0        0        0     1637 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/synthetic/sparsity.py
+-rw-r--r--   0        0        0     4739 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/synthetic/timeseries.py
+-rw-r--r--   0        0        0        0 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/tools/__init__.py
+-rw-r--r--   0        0        0      631 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/tools/aggregators.py
+-rw-r--r--   0        0        0     3615 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/tools/callbacks.py
+-rw-r--r--   0        0        0    10245 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/tools/data.py
+-rw-r--r--   0        0        0     2545 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/tools/exceptions.py
+-rw-r--r--   0        0        0     3168 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/tools/trainer.py
+-rw-r--r--   0        0        0     2237 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/tools/types.py
+-rw-r--r--   0        0        0     1344 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/transforms/__init__.py
+-rw-r--r--   0        0        0     5090 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/transforms/_movavg.py
+-rw-r--r--   0        0        0     1861 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/transforms/_postprocess.py
+-rw-r--r--   0        0        0     2600 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/transforms/_scaler.py
+-rw-r--r--   0        0        0     5178 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/transforms/_stateless.py
+-rw-r--r--   0        0        0     3560 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/README.md
+-rw-r--r--   0        0        0     1232 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/__init__.py
+-rw-r--r--   0        0        0     1937 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/__main__.py
+-rw-r--r--   0        0        0     5192 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/_base.py
+-rw-r--r--   0        0        0     3711 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/_config.py
+-rw-r--r--   0        0        0     1060 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/_logger.py
+-rw-r--r--   0        0        0     4923 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/_metrics.py
+-rw-r--r--   0        0        0     3376 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/entities.py
+-rw-r--r--   0        0        0     4298 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/factory.py
+-rw-r--r--   0        0        0     7349 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/inference.py
+-rw-r--r--   0        0        0     2196 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/payloadtx.py
+-rw-r--r--   0        0        0    15383 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/postprocess.py
+-rw-r--r--   0        0        0     9222 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/preprocess.py
+-rw-r--r--   0        0        0     5581 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/staticthresh.py
+-rw-r--r--   0        0        0    14920 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/tools.py
+-rw-r--r--   0        0        0      229 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/trainer/__init__.py
+-rw-r--r--   0        0        0    13891 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/trainer/_base.py
+-rw-r--r--   0        0        0     5187 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/trainer/_druid.py
+-rw-r--r--   0        0        0     3816 2024-05-06 21:28:57.568693 numalogic-0.9.2/numalogic/udfs/trainer/_prom.py
+-rw-r--r--   0        0        0     3031 2024-05-06 21:28:57.572693 numalogic-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     6952 1970-01-01 00:00:00.000000 numalogic-0.9.2/PKG-INFO
```

### Comparing `numalogic-0.9.1a9/LICENSE` & `numalogic-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/README.md` & `numalogic-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/__init__.py` & `numalogic-0.9.2/numalogic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/_constants.py` & `numalogic-0.9.2/numalogic/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/backtest/_prom.py` & `numalogic-0.9.2/numalogic/backtest/_prom.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,17 +26,15 @@
 from numalogic.backtest._constants import DEFAULT_SEQUENCE_LEN
 from numalogic.config import (
     NumalogicConf,
     ModelFactory,
     PreprocessFactory,
     PostprocessFactory,
     ThresholdFactory,
-    AggregatorConf,
 )
-from numalogic.config._config import AggMethod
 from numalogic.connectors import ConnectorType
 from numalogic.connectors.prometheus import PrometheusFetcher
 from numalogic.tools.data import StreamingDataset, inverse_window
 from numalogic.tools.types import artifact_t
 from numalogic.udfs import UDFFactory, StreamConf, MLPipelineConf
 
 DEFAULT_OUTPUT_DIR = os.path.join(BASE_DIR, ".btoutput")
@@ -133,22 +131,17 @@
             df = df[self.metrics]
 
         df_train, _ = self._split_data(df)
 
         x_train = df_train.to_numpy(dtype=np.float32)
         LOGGER.info("Training data shape: %s", x_train.shape)
 
-        if self.nlconf.trainer.transforms:
-            train_txs = PreprocessFactory().get_pipeline_instance(self.nlconf.trainer.transforms)
-        else:
-            train_txs = None
         artifacts = UDFFactory.get_udf_cls("promtrainer").compute(
             model=ModelFactory().get_instance(self.nlconf.model),
             input_=x_train,
-            trainer_transform=train_txs,
             preproc_clf=PreprocessFactory().get_pipeline_instance(self.nlconf.preprocess),
             threshold_clf=ThresholdFactory().get_instance(self.nlconf.threshold),
             numalogic_cfg=self.nlconf,
         )
         artifacts_dict = {
             "model": artifacts["inference"].artifact,
             "preproc_clf": artifacts["preproc_clf"].artifact,
@@ -241,16 +234,14 @@
 
         n_feat = x_scaled.shape[1]
 
         ds = StreamingDataset(x_scaled, seq_len=self.seq_len, stride=self.nlconf.trainer.ds_stride)
 
         x_recon = np.zeros((len(ds), self.seq_len, n_feat), dtype=np.float32)
         raw_scores = np.zeros((len(ds), self.seq_len, n_feat), dtype=np.float32)
-        unified_raw_scores = np.zeros((len(ds), 1), dtype=np.float32)
-
         feature_scores = np.zeros((len(ds), n_feat), dtype=np.float32)
         unified_scores = np.zeros((len(ds), 1), dtype=np.float32)
 
         postproc_func = PostprocessFactory().get_instance(self.nlconf.postprocess)
 
         # Model Inference
         for idx, arr in enumerate(ds):
@@ -258,25 +249,20 @@
 
             # TODO support for multivariate thresholding functions
             thresh_out = postproc_udf.compute_threshold(artifacts["threshold_clf"], x_recon[idx])
             raw_scores[idx] = thresh_out
 
             winscores = postproc_udf.compute_feature_scores(
                 raw_scores[idx], self.nlconf.score.window_agg
-            )  # (nfeat,)
-
-            unified_raw_scores[idx] = postproc_udf.compute_unified_score(
-                winscores,
-                AggregatorConf(method=AggMethod.MEAN),
             )
 
             feature_scores[idx] = postproc_udf.compute_postprocess(postproc_func, winscores)
 
-            unified_scores[idx] = postproc_udf.compute_postprocess(
-                postproc_func, unified_raw_scores[idx]
+            unified_scores[idx] = postproc_udf.compute_unified_score(
+                feature_scores[idx], self.nlconf.score.feature_agg
             )
 
         x_recon = self.window_inverse(x_recon)
         raw_scores = self.window_inverse(raw_scores)
 
         feature_scores = np.vstack(
             [
```

### Comparing `numalogic-0.9.1a9/numalogic/base.py` & `numalogic-0.9.2/numalogic/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/blocks/__init__.py` & `numalogic-0.9.2/numalogic/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/blocks/_base.py` & `numalogic-0.9.2/numalogic/blocks/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/blocks/_nn.py` & `numalogic-0.9.2/numalogic/blocks/_nn.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/blocks/_transform.py` & `numalogic-0.9.2/numalogic/blocks/_transform.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/blocks/pipeline.py` & `numalogic-0.9.2/numalogic/blocks/pipeline.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/config/__init__.py` & `numalogic-0.9.2/numalogic/config/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/config/_config.py` & `numalogic-0.9.2/numalogic/config/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 class NumalogicConf:
     """Top level config schema for numalogic."""
 
     model: ModelInfo = field(default_factory=ModelInfo)
     trainer: TrainerConf = field(default_factory=TrainerConf)
     preprocess: list[ModelInfo] = field(default_factory=list)
     threshold: ModelInfo = field(default_factory=lambda: ModelInfo(name="StdDevThreshold"))
-    postprocess: Optional[ModelInfo] = field(
+    postprocess: ModelInfo = field(
         default_factory=lambda: ModelInfo(name="TanhNorm", stateful=False)
     )
     score: ScoreConf = field(default_factory=lambda: ScoreConf())
 
 
 @dataclass
 class DataConnectorConf:
```

### Comparing `numalogic-0.9.1a9/numalogic/config/factory.py` & `numalogic-0.9.2/numalogic/config/factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,32 +47,28 @@
         LogTransformer,
         StaticPowerTransformer,
         TanhScaler,
         DataClipper,
         GaussianNoiseAdder,
         DifferenceTransform,
         FlattenVector,
-        PercentileScaler,
-        ExpMovingAverage,
     )
 
     _CLS_MAP: ClassVar[dict] = {
         "StandardScaler": StandardScaler,
         "MinMaxScaler": MinMaxScaler,
         "MaxAbsScaler": MaxAbsScaler,
         "RobustScaler": RobustScaler,
         "LogTransformer": LogTransformer,
         "StaticPowerTransformer": StaticPowerTransformer,
         "TanhScaler": TanhScaler,
         "DataClipper": DataClipper,
         "GaussianNoiseAdder": GaussianNoiseAdder,
         "DifferenceTransform": DifferenceTransform,
         "FlattenVector": FlattenVector,
-        "PercentileScaler": PercentileScaler,
-        "ExpMovingAverage": ExpMovingAverage,
     }
 
     def get_pipeline_instance(self, objs_info: list[ModelInfo]):
         preproc_clfs = []
         for obj_info in objs_info:
             _clf = self.get_instance(obj_info)
             preproc_clfs.append(_clf)
@@ -82,21 +78,17 @@
             return preproc_clfs[0]
         return make_pipeline(*preproc_clfs)
 
 
 class PostprocessFactory(_ObjectFactory):
     """Factory class to create postprocess instances."""
 
-    from numalogic.transforms import TanhNorm, ExpMovingAverage, SigmoidNorm
+    from numalogic.transforms import TanhNorm, ExpMovingAverage
 
-    _CLS_MAP: ClassVar[dict] = {
-        "TanhNorm": TanhNorm,
-        "ExpMovingAverage": ExpMovingAverage,
-        "SigmoidNorm": SigmoidNorm,
-    }
+    _CLS_MAP: ClassVar[dict] = {"TanhNorm": TanhNorm, "ExpMovingAverage": ExpMovingAverage}
 
 
 class ThresholdFactory(_ObjectFactory):
     """Factory class to create threshold instances."""
 
     from numalogic.models.threshold import (
         StdDevThreshold,
```

### Comparing `numalogic-0.9.1a9/numalogic/connectors/__init__.py` & `numalogic-0.9.2/numalogic/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/connectors/_base.py` & `numalogic-0.9.2/numalogic/connectors/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/connectors/_config.py` & `numalogic-0.9.2/numalogic/connectors/_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,23 +33,16 @@
 class Pivot:
     index: str = "timestamp"
     columns: list[str] = field(default_factory=list)
     value: list[str] = field(default_factory=lambda: ["count"])
 
 
 @dataclass
-class FilterConf:
-    inclusion_filters: Optional[list[dict]] = None
-    exclusion_filters: Optional[list[dict]] = None
-
-
-@dataclass
 class DruidFetcherConf:
     datasource: str
-    static_filters: Optional[FilterConf] = None
     dimensions: list[str] = field(default_factory=list)
     aggregations: dict = field(default_factory=dict)
     group_by: list[str] = field(default_factory=list)
     pivot: Pivot = field(default_factory=lambda: Pivot())
     granularity: str = "minute"
 
     def __post_init__(self):
```

### Comparing `numalogic-0.9.1a9/numalogic/connectors/druid/_druid.py` & `numalogic-0.9.2/numalogic/connectors/druid/_druid.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import pandas as pd
 import pytz
 from pydruid.client import PyDruid
 from pydruid.utils.dimensions import DimensionSpec
 from pydruid.utils.filters import Filter
 
 from numalogic.connectors._base import DataFetcher
-from numalogic.connectors._config import Pivot, FilterConf
+from numalogic.connectors._config import Pivot
 from typing import Optional, Final
 
 from numalogic.tools.exceptions import DruidFetcherError
 
 _LOGGER = logging.getLogger(__name__)
 TIMEOUT: Final[int] = 10000
 _MAX_CONCURRENCY: Final[int] = 16
@@ -30,50 +30,32 @@
 
     Returns: a dict of key value pairs
 
     """
     return dict(zip(filter_keys, filter_values))
 
 
-def _combine_in_filters(filters_list) -> Filter:
-    return Filter(type="and", fields=[Filter(**item) for item in filters_list])
-
-
-def _combine_ex_filters(filters_list) -> Filter:
-    filters = _combine_in_filters(filters_list)
-    return Filter(type="not", field=filters)
-
-
-def _make_static_filters(filters: FilterConf) -> Filter:
-    in_filters, ex_filters = _combine_in_filters(filters.inclusion_filters), _combine_ex_filters(
-        filters.exclusion_filters
-    )
-    return Filter(type="and", fields=[in_filters, ex_filters])
-
-
 def build_params(
     datasource: str,
     dimensions: list[str],
     filter_pairs: dict,
     granularity: str,
     hours: float,
     delay: float,
-    static_filters: Optional[FilterConf] = None,
     aggregations: Optional[list[str]] = None,
     post_aggregations: Optional[list[str]] = None,
     reference_dt: Optional[datetime] = None,
 ) -> dict:
     """
 
     Args:
         datasource: Data source to query
         dimensions: The dimensions to group by
         filter_pairs: Indicates which rows of
           data to include in the query
-        static_filters: Static filters passed from config
         granularity: Time bucket to aggregate data by hour, day, minute, etc.,
         hours: Hours from now to skip training.
         delay: Added delay to the fetch query from current time.
         aggregations: A map from aggregator name to one of the
           ``pydruid.utils.aggregators`` e.g., ``doublesum``
         post_aggregations: A map from post aggregator name to one of the
           ``pydruid.utils.postaggregator`` e.g., ``QuantilesDoublesSketchToQuantile``.
@@ -83,19 +65,14 @@
     Returns: a dict of parameters
 
     """
     _filter = Filter(
         type="and",
         fields=[Filter(type="selector", dimension=k, value=v) for k, v in filter_pairs.items()],
     )
-    if static_filters:
-        _LOGGER.debug("Static Filters are present!")
-        _static_filters = _make_static_filters(static_filters)
-        _filter = Filter(type="and", fields=[_static_filters, _filter])
-
     reference_dt = reference_dt or datetime.now(pytz.utc)
     end_dt = reference_dt - timedelta(hours=delay)
     _LOGGER.debug("Querying with end_dt: %s, that is with delay of %s hrs", end_dt, delay)
 
     start_dt = end_dt - timedelta(hours=hours)
 
     intervals = [f"{start_dt.isoformat()}/{end_dt.isoformat()}"]
@@ -137,15 +114,14 @@
         self,
         datasource: str,
         filter_keys: list[str],
         filter_values: list[str],
         dimensions: list[str],
         delay: float = 3.0,
         granularity: str = "minute",
-        static_filters: Optional[FilterConf] = None,
         aggregations: Optional[dict] = None,
         post_aggregations: Optional[dict] = None,
         group_by: Optional[list[str]] = None,
         pivot: Optional[Pivot] = None,
         hours: float = 24,
     ) -> pd.DataFrame:
         """
@@ -155,15 +131,14 @@
         ------
             datasource: Data source to query
             filter_keys: keys
             filter_values: values
             dimensions: The dimensions to group by
             delay: Added delay to the fetch query from current time.
             granularity: Time bucket to aggregate data by hour, day, minute, etc.
-            static_filters: user defined filters
             aggregations: A map from aggregator name to one of the
                 ``pydruid.utils.aggregators`` e.g., ``doublesum``
             post_aggregations: postaggregations map
             group_by: List of columns to group by
             pivot: Pivot configuration
             hours: Hours from now to fetch.
 
@@ -173,15 +148,14 @@
         """
         _start_time = time.perf_counter()
         filter_pairs = make_filter_pairs(filter_keys, filter_values)
         query_params = build_params(
             datasource=datasource,
             dimensions=dimensions,
             filter_pairs=filter_pairs,
-            static_filters=static_filters,
             granularity=granularity,
             hours=hours,
             delay=delay,
             aggregations=aggregations,
             post_aggregations=post_aggregations,
         )
         df = self._fetch(**query_params)
@@ -191,26 +165,20 @@
             return pd.DataFrame()
 
         df["timestamp"] = pd.to_datetime(df["timestamp"]).astype("int64") // 10**6
 
         if group_by:
             df = df.groupby(by=group_by).sum().reset_index()
 
-        # TODO: performance review
-        if pivot:
-            pivoted_frames = []
-            for column in pivot.columns:
-                _df = df.pivot(
-                    index=pivot.index,
-                    columns=[column],
-                    values=pivot.value,
-                )
-                pivoted_frames.append(_df)
-
-            df = pd.concat(pivoted_frames, axis=1, join="outer")
+        if pivot and pivot.columns:
+            df = df.pivot(
+                index=pivot.index,
+                columns=pivot.columns,
+                values=pivot.value,
+            )
             df.columns = df.columns.map("{0[1]}".format)
             df.reset_index(inplace=True)
 
         _end_time = time.perf_counter() - _start_time
         _LOGGER.debug("Druid params: %s, fetch time: %.4fs", query_params, _end_time)
         return df
 
@@ -221,15 +189,14 @@
         self,
         datasource: str,
         filter_keys: list[str],
         filter_values: list[str],
         dimensions: list[str],
         delay: float = 3.0,
         granularity: str = "minute",
-        static_filter: Optional[FilterConf] = None,
         aggregations: Optional[dict] = None,
         post_aggregations: Optional[dict] = None,
         group_by: Optional[list[str]] = None,
         pivot: Optional[Pivot] = None,
         hours: int = 24,
         chunked_hours: int = 6,
     ) -> pd.DataFrame:
@@ -242,15 +209,14 @@
             filter_keys: keys
             filter_values: values
             dimensions: The dimensions to group by
             delay: Added delay to the fetch query from current time.
             granularity: Time bucket to aggregate data by hour, day, minute, etc.
             aggregations: A map from aggregator name to one of the
                 ``pydruid.utils.aggregators`` e.g., ``doublesum``
-            static_filter: user defined filters
             post_aggregations: postaggregations map
             group_by: List of columns to group by
             pivot: Pivot configuration
             hours: Hours from now to skip training.
             chunked_hours: Hours to fetch in each chunk
 
         Returns
@@ -275,47 +241,43 @@
         while hours_elapsed < hours:
             ref_dt = curr_time - timedelta(hours=hours_elapsed)
             qparams.append(
                 build_params(
                     datasource=datasource,
                     dimensions=dimensions,
                     filter_pairs=filter_pairs,
-                    static_filters=static_filter,
                     granularity=granularity,
                     hours=min(chunked_hours, hours - hours_elapsed),
                     delay=delay,
                     aggregations=aggregations,
                     post_aggregations=post_aggregations,
                     reference_dt=ref_dt,
                 )
             )
             hours_elapsed += chunked_hours
 
         max_threads = min(_MAX_CONCURRENCY, len(qparams))
         _LOGGER.debug("Fetching data concurrently with %s threads", max_threads)
         with ThreadPoolExecutor(max_workers=max_threads) as executor:
             futures = [executor.submit(self._fetch, **params) for params in qparams]
-            chunked_dfs.extend(future.result() for future in futures)
+            for future in futures:
+                chunked_dfs.append(future.result())
+
         df = pd.concat(chunked_dfs, axis=0, ignore_index=True)
         df["timestamp"] = pd.to_datetime(df["timestamp"]).astype("int64") // 10**6
 
         if group_by:
             df = df.groupby(by=group_by).sum().reset_index()
 
-        if pivot:
-            pivoted_frames = []
-            for column in pivot.columns:
-                _df = df.pivot(
-                    index=pivot.index,
-                    columns=[column],
-                    values=pivot.value,
-                )
-                pivoted_frames.append(_df)
-
-            df = pd.concat(pivoted_frames, axis=1, join="outer")
+        if pivot and pivot.columns:
+            df = df.pivot(
+                index=pivot.index,
+                columns=pivot.columns,
+                values=pivot.value,
+            )
             df.columns = df.columns.map("{0[1]}".format)
             df.reset_index(inplace=True)
 
         _LOGGER.debug("Fetch time: %.4fs", time.perf_counter() - _start_time)
         return df
 
     def _fetch(self, **query_params) -> pd.DataFrame:
```

### Comparing `numalogic-0.9.1a9/numalogic/connectors/druid/aggregators.py` & `numalogic-0.9.2/numalogic/connectors/druid/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/connectors/druid/postaggregator.py` & `numalogic-0.9.2/numalogic/connectors/druid/postaggregator.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/connectors/prometheus.py` & `numalogic-0.9.2/numalogic/connectors/prometheus.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/connectors/rds/_base.py` & `numalogic-0.9.2/numalogic/connectors/rds/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/connectors/rds/_rds.py` & `numalogic-0.9.2/numalogic/connectors/rds/_rds.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/connectors/rds/db/factory.py` & `numalogic-0.9.2/numalogic/connectors/rds/db/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/connectors/rds/db/mysql_fetcher.py` & `numalogic-0.9.2/numalogic/connectors/rds/db/mysql_fetcher.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/connectors/redis.py` & `numalogic-0.9.2/numalogic/connectors/redis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/connectors/utils/aws/boto3_client_manager.py` & `numalogic-0.9.2/numalogic/connectors/utils/aws/boto3_client_manager.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/connectors/utils/aws/config.py` & `numalogic-0.9.2/numalogic/connectors/utils/aws/config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/connectors/utils/aws/db_configurations.py` & `numalogic-0.9.2/numalogic/connectors/utils/aws/db_configurations.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/connectors/utils/aws/exceptions.py` & `numalogic-0.9.2/numalogic/connectors/utils/aws/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/connectors/utils/aws/sts_client_manager.py` & `numalogic-0.9.2/numalogic/connectors/utils/aws/sts_client_manager.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/connectors/utils/enum.py` & `numalogic-0.9.2/numalogic/connectors/utils/enum.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/models/autoencoder/__init__.py` & `numalogic-0.9.2/numalogic/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/models/autoencoder/base.py` & `numalogic-0.9.2/numalogic/models/autoencoder/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/models/autoencoder/variants/__init__.py` & `numalogic-0.9.2/numalogic/models/autoencoder/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/models/autoencoder/variants/conv.py` & `numalogic-0.9.2/numalogic/models/autoencoder/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/models/autoencoder/variants/lstm.py` & `numalogic-0.9.2/numalogic/models/autoencoder/variants/lstm.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/models/autoencoder/variants/transformer.py` & `numalogic-0.9.2/numalogic/models/autoencoder/variants/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/models/autoencoder/variants/vanilla.py` & `numalogic-0.9.2/numalogic/models/autoencoder/variants/vanilla.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,28 +55,26 @@
         layers = nn.ModuleList()
         start_layersize = self.seq_len
 
         for lsize in layersizes[:-1]:
             layers.extend(
                 [
                     nn.Linear(start_layersize, lsize),
-                    # nn.BatchNorm1d(self.n_features),
+                    nn.BatchNorm1d(self.n_features),
                     nn.Tanh(),
                     nn.Dropout(p=self.dropout_p),
                 ]
             )
             start_layersize = lsize
 
         layers.extend(
             [
                 nn.Linear(start_layersize, layersizes[-1]),
-                # nn.BatchNorm1d(self.n_features),
-                # nn.ReLU(),
-                nn.Tanh(),
-                nn.Dropout(p=self.dropout_p),
+                nn.BatchNorm1d(self.n_features),
+                nn.ReLU(),
             ]
         )
         return layers
 
     def forward(self, x: Tensor) -> Tensor:
         return self.encoder(x)
 
@@ -118,15 +116,15 @@
         """
         layers = nn.ModuleList()
 
         for idx, _ in enumerate(layersizes[:-1]):
             layers.extend(
                 [
                     nn.Linear(layersizes[idx], layersizes[idx + 1]),
-                    # nn.BatchNorm1d(self.n_features),
+                    nn.BatchNorm1d(self.n_features),
                     nn.Tanh(),
                     nn.Dropout(p=self.dropout_p),
                 ]
             )
 
         layers.append(nn.Linear(layersizes[-1], self.seq_len))
         return layers
@@ -188,22 +186,22 @@
 
     def forward(self, batch: Tensor) -> tuple[Tensor, Tensor]:
         batch = torch.swapdims(batch, 1, 2)
         encoded = self.encoder(batch)
         decoded = self.decoder(encoded)
         return encoded, torch.swapdims(decoded, 1, 2)
 
-    def _get_reconstruction_loss(self, batch: Tensor, reduction="mean") -> Tensor:
+    def _get_reconstruction_loss(self, batch: Tensor):
         _, recon = self.forward(batch)
-        return 0.5 * self.criterion(batch, recon, reduction=reduction)
+        return self.criterion(batch, recon)
 
     def predict_step(self, batch: Tensor, batch_idx: int, dataloader_idx: int = 0):
         """Returns reconstruction for streaming input."""
         recon = self.reconstruction(batch)
-        return 0.5 * self.criterion(batch, recon, reduction="none")
+        return self.criterion(batch, recon, reduction="none")
 
 
 class SparseVanillaAE(VanillaAE):
     r"""Sparse Autoencoder for a fully connected network.
     It inherits from VanillaAE class and serves as a wrapper around base network models.
     Sparse Autoencoder is a type of autoencoder that applies sparsity constraint.
     This helps in achieving information bottleneck even when the number of hidden units is huge.
```

### Comparing `numalogic-0.9.1a9/numalogic/models/forecast/variants/naive.py` & `numalogic-0.9.2/numalogic/models/forecast/variants/naive.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/models/threshold/_mahalanobis.py` & `numalogic-0.9.2/numalogic/models/threshold/_mahalanobis.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/models/threshold/_median.py` & `numalogic-0.9.2/numalogic/models/threshold/_median.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,54 @@
 import numpy as np
 import numpy.typing as npt
 from typing_extensions import Self, Final
 
 from numalogic.base import BaseThresholdModel
 from numalogic.tools.exceptions import InvalidDataShapeError, ModelInitializationError
 
-import logging
-
-LOGGER = logging.getLogger(__name__)
 _INLIER: Final[int] = 0
 _OUTLIER: Final[int] = 1
 _INPUT_DIMS: Final[int] = 2
 
 
 class MaxPercentileThreshold(BaseThresholdModel):
     """
     Percentile based Thresholding estimator.
 
     Args:
         max_inlier_percentile: Max percentile greater than which will be treated as outlier
         min_threshold:  Value to be used if threshold is less than this
     """
 
-    __slots__ = (
-        "_max_percentile",
-        "_min_thresh",
-        "_thresh",
-        "_is_fitted",
-        "_adjust_threshold",
-        "_adjust_factor",
-    )
+    __slots__ = ("_max_percentile", "_min_thresh", "_thresh", "_is_fitted")
 
     def __init__(
         self,
         max_inlier_percentile: float = 96.0,
         min_threshold: float = 1e-4,
-        adjust_threshold: bool = False,
-        adjust_factor: float = 3.0,
     ):
         super().__init__()
         self._max_percentile = max_inlier_percentile
         self._min_thresh = min_threshold
         self._thresh = None
         self._is_fitted = False
-        self._adjust_threshold = adjust_threshold
-        self._adjust_factor = adjust_factor
 
     @property
     def threshold(self):
         return self._thresh
 
     @staticmethod
     def _validate_input(x: npt.NDArray[float]) -> None:
         """Validate the input matrix shape."""
         if x.ndim != _INPUT_DIMS:
             raise InvalidDataShapeError(f"Input matrix should have 2 dims, given shape: {x.shape}.")
 
     def fit(self, x: npt.NDArray[float]) -> Self:
         self._validate_input(x)
         self._thresh = np.percentile(x, self._max_percentile, axis=0)
-
-        if self._adjust_threshold:
-            for idx, _ in enumerate(self._thresh):
-                ratio = self._thresh[idx] / self._min_thresh
-                if ratio < 1e-2:
-                    LOGGER.info(
-                        "Min threshold ratio: %s is less than 1e-2 times the "
-                        "threshold for column %s;",
-                        ratio,
-                        idx,
-                    )
-                    self._thresh[idx] = self._min_thresh * self._adjust_factor
-
         self._thresh[self._thresh < self._min_thresh] = self._min_thresh
         self._is_fitted = True
         return self
 
     def predict(self, x: npt.NDArray[float]) -> npt.NDArray[int]:
         if not self._is_fitted:
             raise ModelInitializationError("Model not fitted yet.")
```

### Comparing `numalogic-0.9.1a9/numalogic/models/threshold/_static.py` & `numalogic-0.9.2/numalogic/models/threshold/_static.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/models/threshold/_std.py` & `numalogic-0.9.2/numalogic/models/threshold/_std.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/models/vae/base.py` & `numalogic-0.9.2/numalogic/models/vae/base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/models/vae/layer.py` & `numalogic-0.9.2/numalogic/models/vae/layer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/models/vae/variants/conv.py` & `numalogic-0.9.2/numalogic/models/vae/variants/conv.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/monitoring/__init__.py` & `numalogic-0.9.2/numalogic/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/monitoring/metrics.py` & `numalogic-0.9.2/numalogic/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/registry/__init__.py` & `numalogic-0.9.2/numalogic/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/registry/_serialize.py` & `numalogic-0.9.2/numalogic/registry/_serialize.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/registry/artifact.py` & `numalogic-0.9.2/numalogic/registry/artifact.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/registry/dynamodb_registry.py` & `numalogic-0.9.2/numalogic/registry/dynamodb_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/registry/localcache.py` & `numalogic-0.9.2/numalogic/registry/localcache.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/registry/mlflow_registry.py` & `numalogic-0.9.2/numalogic/registry/mlflow_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/registry/redis_registry.py` & `numalogic-0.9.2/numalogic/registry/redis_registry.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/synthetic/__init__.py` & `numalogic-0.9.2/numalogic/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/synthetic/anomalies.py` & `numalogic-0.9.2/numalogic/synthetic/anomalies.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/synthetic/sparsity.py` & `numalogic-0.9.2/numalogic/synthetic/sparsity.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/synthetic/timeseries.py` & `numalogic-0.9.2/numalogic/synthetic/timeseries.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/tools/aggregators.py` & `numalogic-0.9.2/numalogic/tools/aggregators.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/tools/callbacks.py` & `numalogic-0.9.2/numalogic/tools/callbacks.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/tools/data.py` & `numalogic-0.9.2/numalogic/tools/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,15 @@
             start = idx.start or 0
             stop = min(idx.stop, raw_data_size) if idx.stop else raw_data_size
             for i in range(start, stop - self._seq_len + 1, self._stride):
                 output.append(self._data[i : (i + self._seq_len)])
             return np.stack(output)
         if idx >= len(self):
             raise IndexError(f"{idx} out of bound!")
-        return self._data[(idx * self._stride) : (idx * self._stride) + self._seq_len]
+        return self._data[idx : idx + self._seq_len]
 
 
 class StreamingDataLoader(DataLoader):
     """
     A DataLoader for convenience that uses StreamingDataset for handling time series data.
 
     Args:
```

### Comparing `numalogic-0.9.1a9/numalogic/tools/exceptions.py` & `numalogic-0.9.2/numalogic/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/tools/trainer.py` & `numalogic-0.9.2/numalogic/tools/trainer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/tools/types.py` & `numalogic-0.9.2/numalogic/tools/types.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/transforms/__init__.py` & `numalogic-0.9.2/numalogic/transforms/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,34 +10,32 @@
 # limitations under the License.
 
 """
 Module to provide timeseries transformations needed for preprocessing,
 feature engineering and postprocessing.
 """
 
-from numalogic.transforms._scaler import TanhScaler, PercentileScaler
+from numalogic.transforms._scaler import TanhScaler
 from numalogic.transforms._stateless import (
     LogTransformer,
     StaticPowerTransformer,
     DataClipper,
     GaussianNoiseAdder,
     DifferenceTransform,
     FlattenVector,
 )
 from numalogic.transforms._movavg import ExpMovingAverage, expmov_avg_aggregator
-from numalogic.transforms._postprocess import TanhNorm, tanh_norm, SigmoidNorm
+from numalogic.transforms._postprocess import TanhNorm, tanh_norm
 
 __all__ = [
     "TanhScaler",
     "LogTransformer",
     "StaticPowerTransformer",
     "DataClipper",
     "ExpMovingAverage",
     "expmov_avg_aggregator",
     "TanhNorm",
     "tanh_norm",
     "GaussianNoiseAdder",
     "DifferenceTransform",
     "FlattenVector",
-    "PercentileScaler",
-    "SigmoidNorm",
 ]
```

### Comparing `numalogic-0.9.1a9/numalogic/transforms/_postprocess.py` & `numalogic-0.9.2/numalogic/transforms/_postprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,17 +44,7 @@
 
     def __init__(self, scale_factor=10, smooth_factor=10):
         self.scale_factor = scale_factor
         self.smooth_factor = smooth_factor
 
     def transform(self, input_: npt.NDArray[float], **__) -> npt.NDArray[float]:
         return tanh_norm(input_, scale_factor=self.scale_factor, smooth_factor=self.smooth_factor)
-
-
-class SigmoidNorm(StatelessTransformer):
-    def __init__(self, scale_factor: float = 10.0, smooth_factor: float = 0.5):
-        super().__init__()
-        self.scale_factor = scale_factor
-        self.smooth_factor = smooth_factor
-
-    def transform(self, x: npt.NDArray[float], **__) -> npt.NDArray[float]:
-        return self.scale_factor / (1.0 + np.exp(5 - (self.smooth_factor * x)))
```

### Comparing `numalogic-0.9.1a9/numalogic/transforms/_scaler.py` & `numalogic-0.9.2/numalogic/transforms/_stateless.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,137 +5,154 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
-import logging
-from typing import Optional
+from collections.abc import Sequence
+from typing import Optional, Union
 
 import numpy as np
 import numpy.typing as npt
-from sklearn.preprocessing import MinMaxScaler
-from typing_extensions import Self
+import pandas as pd
 
-from numalogic.base import BaseTransformer
-from numalogic.transforms._stateless import DataClipper
+from numalogic.base import StatelessTransformer
 
-LOGGER = logging.getLogger(__name__)
 
+class LogTransformer(StatelessTransformer):
+    """
+    Applies column-wise log normalization.
 
-class TanhScaler(BaseTransformer):
-    r"""Tanh Estimator applies column-wise tanh normalization to the Z-score,
-    and scales the values between 0 and 1.
+    Args:
+    ----
+        add_factor: float value to be added to the feature before taking log.
+    """
 
-    After scaling, the data has a mean of 0.5.
+    __slots__ = ("add_factor",)
 
-    The coeff parameter determines the spread of the scores.
-    Higher the value, the linear portion of the curve will have a higher slope
-    but will reach the asymptote (flatten out) earlier.
+    def __init__(self, add_factor=2):
+        self.add_factor = add_factor
 
-    Args:
-    ----
-        coeff: float value determining the spread of the scores
-        eps: minimum value below which the feature will be treated as constant.
-             In order to avoid division by zero or a very small number,
-             standard deviation will be set as 1 for that feature.
+    def transform(self, x: npt.NDArray[float], **__) -> npt.NDArray[float]:
+        return np.log(x + self.add_factor)
 
-    References
-    ----------
-        Nandakumar, Jain, Ross. 2005. Score Normalization in
-        Multimodal Biometric Systems, Pattern Recognition 38, 2270-2285.
-        https://web.cse.msu.edu/~rossarun/pubs/RossScoreNormalization_PR05.pdf
-    """
+    def inverse_transform(self, x: npt.NDArray[float]) -> npt.NDArray[float]:
+        return np.exp(x) - self.add_factor
 
-    __slots__ = ("_coeff", "_std", "_mean", "_eps")
 
-    def __init__(self, coeff: float = 0.2, eps: float = 1e-10):
-        self._coeff = coeff
-        self._std = None
-        self._mean = None
-        self._eps = eps
+class StaticPowerTransformer(StatelessTransformer):
+    """
+    Applies column-wise power transformation.
 
-    def fit(self, x: npt.NDArray[float]) -> Self:
-        self._mean = np.mean(x, axis=0)
-        self._std = np.std(x, axis=0)
-        self._check_if_constant(x)
-        return self
+    Args:
+    ----
+        n: float value to be used as the power.
+        add_factor: float value to be added to the feature before taking power.
+    """
 
-    def transform(self, x: npt.NDArray[float]) -> npt.NDArray[float]:
-        x_std_scaled = (x - self._mean) / self._std
-        return 0.5 * (np.tanh(self._coeff * x_std_scaled) + 1)
+    def __init__(self, n: float, add_factor=0):
+        self.add_factor = add_factor
+        self.n = n
 
-    def fit_transform(self, x: npt.NDArray[float], y=None, **_) -> npt.NDArray[float]:
-        return self.fit(x).transform(x)
+    def transform(self, X, **__):
+        return np.power(X + self.add_factor, self.n)
 
-    def _check_if_constant(self, x: npt.NDArray[float]) -> None:
-        delta = np.max(x, axis=0) - np.min(x, axis=0)
-        self._std[delta < self._eps] = 1.0
+    def inverse_transform(self, X) -> npt.NDArray[float]:
+        return np.power(X, 1.0 / self.n) - self.add_factor
 
 
-class PercentileScaler(BaseTransformer):
+class DataClipper(StatelessTransformer):
     """
-    Scales the data based on the percentiles of the data.
+    Applies column-wise ceiling transformation.
 
     Args:
-    -----
-        max_percentile: float, optional
-            The upper percentile to clip the data.
-            Default is 99.
-        min_percentile: float, optional
-            The lower percentile to clip the data.
-            If None, minimum value of the data is used.
-            Default is None.
+    ----
+        lower: lower bound for clipping.
+        upper: upper bound for clipping.
     """
 
+    __slots__ = ("lower", "upper")
+
     def __init__(
-        self, max_percentile: float = 99, min_percentile: Optional[float] = None, eps: float = 1e-2
+        self,
+        lower: Optional[Union[float, Sequence[float]]] = None,
+        upper: Optional[Union[float, Sequence[float]]] = None,
     ):
-        self._max_px = max_percentile
-        self._min_px = min_percentile
-        self.tx = MinMaxScaler()
-
-        self._data_pth_max = None
-        self._data_pth_min = None
-        self._eps = eps
-
-    @property
-    def data_pth_max(self) -> float:
-        return self._data_pth_max
-
-    @property
-    def data_pth_min(self) -> float:
-        return self._data_pth_min
-
-    def fit(self, x: npt.NDArray[float]) -> Self:
-        data_max_px = np.percentile(x, self._max_px, axis=0)
-        data_max = np.max(x, axis=0)
-
-        if self._min_px is None:
-            data_min_px = np.min(x, axis=0)
-        else:
-            data_min_px = np.percentile(x, self._min_px, axis=0)
-
-        p_ranges = data_max_px - data_min_px
-
-        for idx, _range in enumerate(p_ranges):
-            if _range <= self._eps:
-                LOGGER.warning(
-                    "Max and Min percentile difference is less than " "epsilon: %s for column %s",
-                    self._eps,
-                    idx,
-                )
-                data_max_px[idx] = data_max[idx]
-
-        self._data_pth_max = data_max_px
-        self._data_pth_min = data_min_px
+        self.lower, self.upper = self._validate_args(lower, upper)
+
+    @staticmethod
+    def _validate_args(
+        lower: Optional[Union[float, Sequence[float]]],
+        upper: Optional[Union[float, Sequence[float]]],
+    ) -> Optional[tuple[Optional[Union[float, npt.NDArray]], Optional[Union[float, npt.NDArray]]]]:
+        if lower is None and upper is None:
+            raise ValueError("At least one of lower or upper should be provided.")
+        if isinstance(lower, Sequence) and isinstance(upper, Sequence):
+            if len(lower) != len(upper):
+                raise ValueError("lower and upper should have the same length.")
+            lower, upper = np.asarray(lower, dtype=np.float32), np.asarray(upper, dtype=np.float32)
+        if upper is not None and lower is not None and np.any(lower > upper):
+            raise ValueError("lower value should be less than or equal to upper value")
+        return lower, upper
+
+    def transform(self, x: npt.NDArray[float], **__) -> npt.NDArray[float]:
+        _df = pd.DataFrame(x, dtype=np.float32)
+        _df = _df.clip(upper=self.upper, lower=self.lower, axis=1)
+        return _df.to_numpy(dtype=np.float32)
+
+
+class GaussianNoiseAdder(StatelessTransformer):
+    """
+    Applies Gaussian noise to data.
+
+    Args:
+    ----
+        scale: small float value to be used as the noise factor (default: 1e-8).
+        positive_only: bool value to indicate whether
+            to use absolute value of the noise (default: True).
+        seed: int value to be used as the random seed (default: 42).
+    """
+
+    __slots__ = ("_rng", "_is_abs", "_scale")
+
+    def __init__(self, scale: float = 1e-8, positive_only: bool = True, seed: int = 42):
+        self._rng = np.random.default_rng(seed)
+        self._is_abs = positive_only
+        self._scale = scale
+
+    def transform(self, x: npt.NDArray[float], **__) -> npt.NDArray[float]:
+        noise = self._rng.normal(loc=0.0, scale=self._scale, size=x.shape)
+        if self._is_abs:
+            noise = np.abs(noise)
+        return x + noise
+
+
+class DifferenceTransform(StatelessTransformer):
+    """
+    Apply feature wise differencing.
+
+    Note: First value is backfilled with the first non-NAN value.
+    """
+
+    def transform(self, input_: npt.NDArray, **__):
+        diff_df = pd.DataFrame(input_).diff().bfill()
+        return diff_df.to_numpy(dtype=np.float32)
+
+
+class FlattenVector(StatelessTransformer):
+    """A stateless transformer that flattens a vector.
+
+    Args:
+    ____
+        n_features: number of features
+
+    """
 
-        x_clipped = DataClipper(lower=data_min_px, upper=data_max_px).transform(x)
-        return self.tx.fit(x_clipped)
+    def __init__(self, n_features: int):
+        self.n_features = n_features
 
-    def fit_transform(self, x: npt.NDArray[float], y=None, **_):
-        return self.fit(x).transform(x)
+    def transform(self, X: npt.NDArray[float], **__) -> npt.NDArray[float]:
+        return X.flatten().reshape(-1, 1)
 
-    def transform(self, x: npt.NDArray[float]) -> npt.NDArray[float]:
-        return self.tx.transform(x)
+    def inverse_transform(self, X: npt.NDArray[float]) -> npt.NDArray[float]:
+        return X.reshape(-1, self.n_features)
```

### Comparing `numalogic-0.9.1a9/numalogic/udfs/README.md` & `numalogic-0.9.2/numalogic/udfs/README.md`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/udfs/__init__.py` & `numalogic-0.9.2/numalogic/udfs/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/udfs/__main__.py` & `numalogic-0.9.2/numalogic/udfs/__main__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/udfs/_base.py` & `numalogic-0.9.2/numalogic/udfs/_base.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/udfs/_config.py` & `numalogic-0.9.2/numalogic/udfs/_config.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/udfs/_logger.py` & `numalogic-0.9.2/numalogic/udfs/_logger.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/udfs/_metrics.py` & `numalogic-0.9.2/numalogic/udfs/_metrics.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/udfs/entities.py` & `numalogic-0.9.2/numalogic/udfs/entities.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/udfs/factory.py` & `numalogic-0.9.2/numalogic/udfs/factory.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/udfs/inference.py` & `numalogic-0.9.2/numalogic/udfs/inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,16 @@
         ------
             RuntimeError: If model forward pass fails
         """
         x = torch.from_numpy(input_).unsqueeze(0)
         model.eval()
         try:
             with torch.no_grad():
-                recon_err = model._get_reconstruction_loss(x, reduction="none")
+                _, out = model.forward(x)
+                recon_err = model.criterion(out, x, reduction="none")
         except Exception as err:
             raise RuntimeError("Model forward pass failed!") from err
         return np.ascontiguousarray(recon_err).squeeze(0)
 
     @UDF_TIME.time()
     def exec(self, keys: list[str], datum: Datum) -> Messages:
         """
```

### Comparing `numalogic-0.9.1a9/numalogic/udfs/payloadtx.py` & `numalogic-0.9.2/numalogic/udfs/payloadtx.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/udfs/postprocess.py` & `numalogic-0.9.2/numalogic/udfs/postprocess.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,19 +118,15 @@
             skeys=[_ckey for _, _ckey in zip(_stream_conf.composite_keys, payload.composite_keys)],
             dkeys=[payload.pipeline_id, thresh_cfg.name],
             payload=payload,
             model_registry=self.model_registry,
             load_latest=LOAD_LATEST,
             vertex=self._vtx,
         )
-        postproc_tx = (
-            self.postproc_factory.get_instance(postprocess_cfg) if postprocess_cfg else None
-        )
-        if not postproc_tx:
-            logger.info("Postprocess model is absent!")
+        postproc_tx = self.postproc_factory.get_instance(postprocess_cfg)
 
         if thresh_artifact is None:
             payload = replace(
                 payload, status=Status.ARTIFACT_NOT_FOUND, header=Header.TRAIN_REQUEST
             )
             # Send training request if artifact loading is not successful
             msgs = Messages(get_trainer_message(keys, _stream_conf, payload))
@@ -139,27 +135,25 @@
             return msgs
 
         if payload.header == Header.STATIC_INFERENCE:
             logger.warning("Static inference not supported in postprocess yet")
 
         #  Postprocess payload
         try:
-            # Compute anomaly scores
-            a_unified, a_features = self.compute(
+            # Compute anomaly scores per feature
+            a_features = self.compute(
                 model=thresh_artifact.artifact,
                 input_=payload.get_data(),
                 score_conf=_conf.numalogic_conf.score,
                 postproc_tx=postproc_tx,
             )  # (nfeat,)
-            payload = replace(
-                payload,
-                metadata={
-                    "threshold": float(thresh_artifact.artifact.threshold),
-                    **payload.metadata,
-                },
+
+            # Compute unified score
+            a_unified = self.compute_unified_score(
+                a_features, feat_agg_conf=_conf.numalogic_conf.score.feature_agg
             )
 
             # Calculate adjusted unified score
             a_adjusted, y_unified, y_features = self._adjust_score(_conf, a_unified, payload)
 
         except RuntimeError:
             _increment_counter(RUNTIME_ERROR_COUNTER, _metric_label_values)
@@ -209,14 +203,15 @@
             "Successfully post-processed!",
             composite_keys=out_payload.composite_keys,
             unified_anomaly=out_payload.unified_anomaly,
             a_unified=a_unified,
             y_features=y_features,
             y_unified=y_unified,
             a_features=a_features.tolist(),
+            artifact_versions=payload.artifact_versions,
             execution_time_secs=round(time.perf_counter() - _start_time, 4),
         )
 
         return Messages(Message(keys=keys, value=out_payload.to_json(), tags=["output"]))
 
     def _adjust_score(
         self, mlpl_conf: MLPipelineConf, a_unified: float, payload: StreamPayload
@@ -304,54 +299,44 @@
     def compute(
         cls,
         model: artifact_t,
         input_: NDArray[float],
         postproc_tx=None,
         score_conf: Optional[ScoreConf] = None,
         **_,
-    ) -> tuple[float, NDArray[float]]:
+    ) -> NDArray[float]:
         """
         Compute thresholding, window aggregation followed by postprocess.
 
         Args:
         -------
         model: Threshold model instance
         input_: Input data (Shape: seq_len x n_features)
         postproc_tx: Postprocess transform
         score_conf: Score Config
 
         Returns
         -------
-        Tuple of combined/unified score (float), and feature scores of shape (n_features,)
+        Output data of shape (n_features, )
 
         Raises
         ------
             RuntimeError: If threshold model or postproc function fails
         """
         if score_conf is None:
             _struct_log.warning("Score config not provided, using default values")
             score_conf = ScoreConf()
 
-        thresh_scores = cls.compute_threshold(model, input_)  # (seqlen x nfeat)
-
-        # Aggregate over the sequence length
-        raw_scores = cls.compute_feature_scores(
-            thresh_scores, win_agg_conf=score_conf.window_agg
+        scores = cls.compute_threshold(model, input_)  # (seqlen x nfeat)
+        win_scores = cls.compute_feature_scores(
+            scores, win_agg_conf=score_conf.window_agg
         )  # (nfeat,)
-
-        # Aggregate over the features
-        unified_raw_score = cls.compute_unified_score(raw_scores, score_conf.feature_agg)  # float
-
         if postproc_tx:
-            # Postprocess the raw scores
-            feature_scores = cls.compute_postprocess(postproc_tx, raw_scores)  # (nfeat,)
-            unified_score = cls.compute_postprocess(postproc_tx, unified_raw_score)  # float
-            return unified_score, feature_scores
-
-        return unified_raw_score, raw_scores
+            win_scores = cls.compute_postprocess(postproc_tx, win_scores)  # (nfeat,)
+        return win_scores  # (nfeat, )
 
     @classmethod
     def compute_threshold(cls, model: artifact_t, input_: NDArray[float]) -> NDArray[float]:
         """
         Compute raw anomaly scores using the threshold model.
 
         Args:
```

### Comparing `numalogic-0.9.1a9/numalogic/udfs/preprocess.py` & `numalogic-0.9.2/numalogic/udfs/preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,14 @@
                 return msgs
         # Model will not be in registry
         else:
             # Load configuration for the config_id
             _increment_counter(SOURCE_COUNTER, labels=("config", *_metric_label_values))
             preproc_clf = self._load_model_from_config(_conf.numalogic_conf.preprocess)
             payload = replace(payload, status=Status.ARTIFACT_FOUND)
-            logger = logger.bind(model_from_config=preproc_clf)
         try:
             x_scaled = self.compute(model=preproc_clf, input_=payload.get_data())
 
             # make metrics list matching same shape as data
             payload = replace(
                 payload, metrics=_get_updated_metrics(payload.metrics, x_scaled.shape)
             )
```

### Comparing `numalogic-0.9.1a9/numalogic/udfs/staticthresh.py` & `numalogic-0.9.2/numalogic/udfs/staticthresh.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/udfs/tools.py` & `numalogic-0.9.2/numalogic/udfs/tools.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/numalogic/udfs/trainer/_base.py` & `numalogic-0.9.2/numalogic/udfs/trainer/_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     MSG_PROCESSED_COUNTER,
     UDF_TIME,
     _increment_counter,
     _add_summary,
 )
 from numalogic.udfs.entities import TrainerPayload
 from numalogic.udfs.tools import TrainMsgDeduplicator
-import torch
 
 _struct_log = configure_logger()
 
 
 class TrainerUDF(NumalogicUDF):
     """
     Trainer UDF for Numalogic.
@@ -76,14 +75,15 @@
         cls,
         model: artifact_t,
         input_: npt.NDArray[float],
         preproc_clf: Optional[artifact_t] = None,
         trainer_transform: Optional[artifact_t] = None,
         threshold_clf: Optional[artifact_t] = None,
         numalogic_cfg: Optional[NumalogicConf] = None,
+        logger=None,
     ) -> dict[str, KeyedArtifact]:
         """
         Train the model on the given input data.
 
         Args:
             model: Model artifact
             input_: Input data
@@ -117,27 +117,24 @@
 
         train_ds = StreamingDataset(input_, model.seq_len, stride=trainer_cfg.ds_stride)
         trainer = TimeseriesTrainer(**asdict(trainer_cfg.pltrainer_conf))
         trainer.fit(
             model, train_dataloaders=DataLoader(train_ds, batch_size=trainer_cfg.batch_size)
         )
         train_reconerr = trainer.predict(
-            model,
-            dataloaders=DataLoader(train_ds, batch_size=trainer_cfg.batch_size),
-            unbatch=False,
-        )
-        train_reconerr = torch.mean(train_reconerr, dim=1).numpy()
-
+            model, dataloaders=DataLoader(train_ds, batch_size=trainer_cfg.batch_size)
+        ).numpy()
         dict_artifacts["inference"] = KeyedArtifact(
             dkeys=[numalogic_cfg.model.name], artifact=model, stateful=numalogic_cfg.model.stateful
         )
 
         if threshold_clf:
             threshold_clf.fit(train_reconerr)
-            _struct_log.debug("Fit data using threshold model")
+            if logger:
+                logger.debug("Fit data using threshold model")
             dict_artifacts["threshold_clf"] = KeyedArtifact(
                 dkeys=[numalogic_cfg.threshold.name],
                 artifact=threshold_clf,
                 stateful=numalogic_cfg.threshold.stateful,
             )
 
         return dict_artifacts
@@ -234,20 +231,20 @@
         logger.debug("Data fetched", uuid=payload.uuid, shape=df.shape)
 
         # Construct feature array
         x_train, nan_counter, inf_counter = self.get_feature_arr(df, _conf.metrics)
         _add_summary(
             summary=NAN_SUMMARY,
             labels=_metric_label_values,
-            data=np.sum(nan_counter),
+            data=nan_counter,
         )
         _add_summary(
             summary=INF_SUMMARY,
             labels=_metric_label_values,
-            data=np.sum(inf_counter),
+            data=inf_counter,
         )
 
         # Initialize artifacts
         preproc_clf = self._construct_clf(_conf.numalogic_conf.preprocess)
         trainer_transform = self._construct_clf(_conf.numalogic_conf.trainer.transforms)
         model = self._model_factory.get_instance(_conf.numalogic_conf.model)
         thresh_clf = self._thresh_factory.get_instance(_conf.numalogic_conf.threshold)
@@ -256,14 +253,15 @@
         dict_artifacts = self.compute(
             model=model,
             input_=x_train,
             preproc_clf=preproc_clf,
             trainer_transform=trainer_transform,
             threshold_clf=thresh_clf,
             numalogic_cfg=_conf.numalogic_conf,
+            logger=logger,
         )
         # Save artifacts
 
         self.artifacts_to_save(
             skeys=payload.composite_keys,
             dict_artifacts=dict_artifacts,
             model_registry=self.model_registry,
@@ -364,38 +362,37 @@
 
     # TODO: Use a custom impute in transforms module
     @staticmethod
     def get_feature_arr(
         raw_df: pd.DataFrame,
         metrics: list[str],
         fill_value: float = 0.0,
-    ) -> tuple[npt.NDArray[float], pd.Series, pd.Series]:
+    ) -> tuple[npt.NDArray[float], float, float]:
         """
         Get feature array from the raw dataframe.
 
         Args:
             raw_df: Raw dataframe
             metrics: List of metrics
             fill_value: Value to fill missing values with
 
         Returns
         -------
             Numpy array
             nan_counter: Number of nan values
             inf_counter: Number of inf values
         """
-        nan_counter = np.zeros(len(metrics), dtype=int)
-        inf_counter = np.zeros(len(metrics), dtype=int)
-        for idx, col in enumerate(metrics):
+        nan_counter = 0
+        for col in metrics:
             if col not in raw_df.columns:
                 raw_df[col] = fill_value
-                nan_counter[idx] += len(raw_df)
+                nan_counter += len(raw_df)
         feat_df = raw_df[metrics]
-        nan_counter += feat_df.isna().sum()
-        inf_counter = np.isinf(feat_df).sum()
+        nan_counter += raw_df.isna().sum().all()
+        inf_counter = np.isinf(feat_df).sum().all()
         feat_df = feat_df.fillna(fill_value).replace([np.inf, -np.inf], fill_value)
         return feat_df.to_numpy(dtype=np.float32), nan_counter, inf_counter
 
     def fetch_data(self, payload: TrainerPayload) -> Optional[pd.DataFrame]:
         """
         Fetch data from a data connector.
```

### Comparing `numalogic-0.9.1a9/numalogic/udfs/trainer/_druid.py` & `numalogic-0.9.2/numalogic/udfs/trainer/_druid.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,14 @@
             )
 
         try:
             _df = self.data_fetcher.fetch(
                 datasource=_fetcher_conf.datasource,
                 filter_keys=_stream_conf.composite_keys,
                 filter_values=payload.composite_keys,
-                static_filters=_fetcher_conf.static_filters,
                 dimensions=list(_fetcher_conf.dimensions),
                 delay=self.dataconn_conf.delay_hrs,
                 granularity=_fetcher_conf.granularity,
                 aggregations=dict(_fetcher_conf.aggregations),
                 group_by=list(_fetcher_conf.group_by),
                 pivot=_fetcher_conf.pivot,
                 hours=_conf.numalogic_conf.trainer.train_hours,
```

### Comparing `numalogic-0.9.1a9/numalogic/udfs/trainer/_prom.py` & `numalogic-0.9.2/numalogic/udfs/trainer/_prom.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.9.1a9/pyproject.toml` & `numalogic-0.9.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "numalogic"
-version = "0.9.1a9"
+version = "0.9.2"
 description = "Collection of operational Machine Learning models and tools."
 authors = ["Numalogic Developers"]
 packages = [{ include = "numalogic" }]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
@@ -35,14 +35,15 @@
 prometheus_client = "^0.18.0"
 structlog = "^24.1.0"
 
 # extras
 mlflow-skinny = { version = "^2.0", optional = true }
 redis = { extras = ["hiredis"], version = "^5.0", optional = true }
 boto3 = { version = "^1.24.64", optional = true }
+
 pydruid = { version = "^0.6", optional = true }
 PyMySQL = { version = "^1.1.0", optional = true }
 
 
 [tool.poetry.extras]
 mlflow = ["mlflow-skinny"]
 redis = ["redis"]
```

### Comparing `numalogic-0.9.1a9/PKG-INFO` & `numalogic-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numalogic
-Version: 0.9.1a9
+Version: 0.9.2
 Summary: Collection of operational Machine Learning models and tools.
 Home-page: https://numalogic.numaproj.io/
 License: Apache-2.0
 Author: Numalogic Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
 Requires-Python: >=3.9,<3.12
```

