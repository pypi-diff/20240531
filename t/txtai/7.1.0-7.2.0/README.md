# Comparing `tmp/txtai-7.1.0.tar.gz` & `tmp/txtai-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txtai-7.1.0.tar", last modified: Fri Apr 19 13:07:55 2024, max compression
+gzip compressed data, was "txtai-7.2.0.tar", last modified: Fri May 31 14:50:58 2024, max compression
```

## Comparing `txtai-7.1.0.tar` & `txtai-7.2.0.tar`

### file list

```diff
@@ -1,235 +1,241 @@
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.488750 txtai-7.1.0/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)    10754 2021-01-12 02:31:22.000000 txtai-7.1.0/LICENSE
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    26266 2024-04-19 13:07:55.488750 txtai-7.1.0/PKG-INFO
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    18444 2024-04-18 17:11:10.000000 txtai-7.1.0/README.md
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)       31 2021-01-23 16:25:29.000000 txtai-7.1.0/pyproject.toml
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       38 2024-04-19 13:07:55.488750 txtai-7.1.0/setup.cfg
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3932 2024-04-19 10:24:30.000000 txtai-7.1.0/setup.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.470749 txtai-7.1.0/src/
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.470749 txtai-7.1.0/src/python/
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.472750 txtai-7.1.0/src/python/txtai/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      291 2024-01-29 15:16:27.000000 txtai-7.1.0/src/python/txtai/__init__.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.472750 txtai-7.1.0/src/python/txtai/ann/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      198 2023-05-02 19:52:58.000000 txtai-7.1.0/src/python/txtai/ann/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1886 2023-09-08 13:19:22.000000 txtai-7.1.0/src/python/txtai/ann/annoy.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3205 2023-09-08 13:19:37.000000 txtai-7.1.0/src/python/txtai/ann/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1467 2023-06-14 16:28:58.000000 txtai-7.1.0/src/python/txtai/ann/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6526 2023-11-04 13:45:52.000000 txtai-7.1.0/src/python/txtai/ann/faiss.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3207 2023-10-27 17:13:57.000000 txtai-7.1.0/src/python/txtai/ann/hnsw.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4085 2023-10-27 19:09:06.000000 txtai-7.1.0/src/python/txtai/ann/numpy.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      894 2023-10-27 19:03:54.000000 txtai-7.1.0/src/python/txtai/ann/torch.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.473749 txtai-7.1.0/src/python/txtai/api/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      510 2024-03-30 12:38:43.000000 txtai-7.1.0/src/python/txtai/api/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2931 2024-02-05 22:48:18.000000 txtai-7.1.0/src/python/txtai/api/application.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1312 2023-12-26 16:31:07.000000 txtai-7.1.0/src/python/txtai/api/authorization.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4736 2024-02-20 16:43:38.000000 txtai-7.1.0/src/python/txtai/api/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8500 2024-02-20 16:44:37.000000 txtai-7.1.0/src/python/txtai/api/cluster.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      369 2021-04-09 22:58:59.000000 txtai-7.1.0/src/python/txtai/api/extension.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      640 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/factory.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.473749 txtai-7.1.0/src/python/txtai/api/responses/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      153 2024-02-06 01:16:00.000000 txtai-7.1.0/src/python/txtai/api/responses/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      608 2024-02-05 22:28:09.000000 txtai-7.1.0/src/python/txtai/api/responses/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1318 2024-02-06 16:38:51.000000 txtai-7.1.0/src/python/txtai/api/responses/json.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1007 2024-02-06 16:39:02.000000 txtai-7.1.0/src/python/txtai/api/responses/messagepack.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1375 2024-02-06 16:39:23.000000 txtai-7.1.0/src/python/txtai/api/route.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.473749 txtai-7.1.0/src/python/txtai/api/routers/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      357 2024-02-04 12:33:23.000000 txtai-7.1.0/src/python/txtai/api/routers/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      741 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/caption.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7615 2024-02-20 16:53:10.000000 txtai-7.1.0/src/python/txtai/api/routers/embeddings.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      807 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/entity.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      658 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/extractor.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1212 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/labels.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      843 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/objects.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      769 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/segmentation.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1210 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/similarity.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1188 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/summary.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      803 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/tabular.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      782 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/textractor.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      795 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/transcription.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1272 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/translation.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      593 2024-02-06 16:31:35.000000 txtai-7.1.0/src/python/txtai/api/routers/workflow.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.473749 txtai-7.1.0/src/python/txtai/app/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       66 2022-03-01 18:21:41.000000 txtai-7.1.0/src/python/txtai/app/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    24345 2024-02-20 16:53:11.000000 txtai-7.1.0/src/python/txtai/app/base.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.474749 txtai-7.1.0/src/python/txtai/archive/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      160 2023-02-19 13:31:37.000000 txtai-7.1.0/src/python/txtai/archive/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2840 2023-02-19 18:17:59.000000 txtai-7.1.0/src/python/txtai/archive/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1029 2023-12-04 17:41:19.000000 txtai-7.1.0/src/python/txtai/archive/compress.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      429 2023-02-19 18:15:28.000000 txtai-7.1.0/src/python/txtai/archive/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1272 2023-12-04 14:24:11.000000 txtai-7.1.0/src/python/txtai/archive/tar.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1027 2023-12-04 17:56:46.000000 txtai-7.1.0/src/python/txtai/archive/zip.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.474749 txtai-7.1.0/src/python/txtai/cloud/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      148 2023-02-17 13:35:20.000000 txtai-7.1.0/src/python/txtai/cloud/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2424 2023-02-19 18:45:23.000000 txtai-7.1.0/src/python/txtai/cloud/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1544 2023-02-19 13:30:19.000000 txtai-7.1.0/src/python/txtai/cloud/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3649 2023-03-03 17:46:20.000000 txtai-7.1.0/src/python/txtai/cloud/hub.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3741 2024-03-05 16:14:02.000000 txtai-7.1.0/src/python/txtai/cloud/storage.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.474749 txtai-7.1.0/src/python/txtai/console/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       51 2022-03-29 00:05:18.000000 txtai-7.1.0/src/python/txtai/console/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      274 2022-03-29 16:55:55.000000 txtai-7.1.0/src/python/txtai/console/__main__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6590 2023-02-19 19:08:09.000000 txtai-7.1.0/src/python/txtai/console/base.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.474749 txtai-7.1.0/src/python/txtai/data/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      190 2023-01-01 14:12:39.000000 txtai-7.1.0/src/python/txtai/data/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3958 2023-01-09 14:39:56.000000 txtai-7.1.0/src/python/txtai/data/base.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1198 2022-11-26 00:37:43.000000 txtai-7.1.0/src/python/txtai/data/labels.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4599 2022-04-16 12:34:51.000000 txtai-7.1.0/src/python/txtai/data/questions.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1336 2022-04-11 19:50:27.000000 txtai-7.1.0/src/python/txtai/data/sequences.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1883 2023-01-09 15:33:33.000000 txtai-7.1.0/src/python/txtai/data/texts.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      579 2022-12-04 18:56:16.000000 txtai-7.1.0/src/python/txtai/data/tokens.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.475750 txtai-7.1.0/src/python/txtai/database/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      291 2023-08-22 13:28:05.000000 txtai-7.1.0/src/python/txtai/database/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9739 2024-01-23 18:09:29.000000 txtai-7.1.0/src/python/txtai/database/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5308 2024-04-17 12:20:59.000000 txtai-7.1.0/src/python/txtai/database/client.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4381 2023-11-07 15:54:54.000000 txtai-7.1.0/src/python/txtai/database/duckdb.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1801 2024-04-17 12:20:59.000000 txtai-7.1.0/src/python/txtai/database/embedded.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.475750 txtai-7.1.0/src/python/txtai/database/encoder/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      153 2021-12-22 11:16:40.000000 txtai-7.1.0/src/python/txtai/database/encoder/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      719 2022-05-27 12:13:14.000000 txtai-7.1.0/src/python/txtai/database/encoder/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1001 2022-09-20 17:06:23.000000 txtai-7.1.0/src/python/txtai/database/encoder/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      904 2023-04-21 14:52:54.000000 txtai-7.1.0/src/python/txtai/database/encoder/image.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      435 2023-08-07 00:41:39.000000 txtai-7.1.0/src/python/txtai/database/encoder/pickle.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1790 2023-09-07 14:18:38.000000 txtai-7.1.0/src/python/txtai/database/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    16441 2024-04-17 12:20:59.000000 txtai-7.1.0/src/python/txtai/database/rdbms.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.475750 txtai-7.1.0/src/python/txtai/database/schema/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       76 2023-08-22 09:49:40.000000 txtai-7.1.0/src/python/txtai/database/schema/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2321 2023-08-26 00:47:23.000000 txtai-7.1.0/src/python/txtai/database/schema/orm.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3110 2023-09-19 13:47:26.000000 txtai-7.1.0/src/python/txtai/database/schema/statement.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.475750 txtai-7.1.0/src/python/txtai/database/sql/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      146 2022-03-01 13:12:16.000000 txtai-7.1.0/src/python/txtai/database/sql/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5315 2021-12-26 16:01:02.000000 txtai-7.1.0/src/python/txtai/database/sql/aggregate.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6198 2023-10-26 16:22:14.000000 txtai-7.1.0/src/python/txtai/database/sql/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    13855 2023-11-07 01:06:06.000000 txtai-7.1.0/src/python/txtai/database/sql/expression.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8869 2022-11-19 15:44:37.000000 txtai-7.1.0/src/python/txtai/database/sql/token.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1588 2023-08-22 13:25:25.000000 txtai-7.1.0/src/python/txtai/database/sqlite.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.475750 txtai-7.1.0/src/python/txtai/embeddings/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      100 2023-08-09 11:18:31.000000 txtai-7.1.0/src/python/txtai/embeddings/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    33434 2024-04-17 11:52:42.000000 txtai-7.1.0/src/python/txtai/embeddings/base.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.476750 txtai-7.1.0/src/python/txtai/embeddings/index/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      293 2024-02-02 12:33:35.000000 txtai-7.1.0/src/python/txtai/embeddings/index/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      152 2023-07-09 19:17:44.000000 txtai-7.1.0/src/python/txtai/embeddings/index/action.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2154 2023-07-10 16:44:09.000000 txtai-7.1.0/src/python/txtai/embeddings/index/autoid.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1890 2023-08-09 09:52:25.000000 txtai-7.1.0/src/python/txtai/embeddings/index/documents.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4329 2023-08-08 10:14:35.000000 txtai-7.1.0/src/python/txtai/embeddings/index/functions.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4568 2024-02-28 15:34:15.000000 txtai-7.1.0/src/python/txtai/embeddings/index/indexes.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1286 2024-01-30 20:32:31.000000 txtai-7.1.0/src/python/txtai/embeddings/index/indexids.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2717 2023-08-09 10:05:10.000000 txtai-7.1.0/src/python/txtai/embeddings/index/reducer.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2109 2023-08-23 14:12:53.000000 txtai-7.1.0/src/python/txtai/embeddings/index/stream.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7192 2024-01-19 01:38:26.000000 txtai-7.1.0/src/python/txtai/embeddings/index/transform.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.476750 txtai-7.1.0/src/python/txtai/embeddings/search/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      194 2024-01-21 13:37:35.000000 txtai-7.1.0/src/python/txtai/embeddings/search/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9490 2024-03-31 16:05:43.000000 txtai-7.1.0/src/python/txtai/embeddings/search/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      138 2023-08-08 13:42:50.000000 txtai-7.1.0/src/python/txtai/embeddings/search/errors.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4132 2023-07-25 21:39:08.000000 txtai-7.1.0/src/python/txtai/embeddings/search/explain.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1305 2024-01-30 16:48:28.000000 txtai-7.1.0/src/python/txtai/embeddings/search/ids.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1783 2022-04-18 19:57:38.000000 txtai-7.1.0/src/python/txtai/embeddings/search/query.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6023 2023-11-07 15:38:49.000000 txtai-7.1.0/src/python/txtai/embeddings/search/scan.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1145 2023-03-02 22:24:02.000000 txtai-7.1.0/src/python/txtai/embeddings/search/terms.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.476750 txtai-7.1.0/src/python/txtai/graph/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      139 2022-09-03 13:13:44.000000 txtai-7.1.0/src/python/txtai/graph/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    21990 2024-04-17 12:28:46.000000 txtai-7.1.0/src/python/txtai/graph/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1133 2023-06-14 16:29:08.000000 txtai-7.1.0/src/python/txtai/graph/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6543 2024-04-17 12:28:46.000000 txtai-7.1.0/src/python/txtai/graph/networkx.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4549 2024-01-22 22:57:23.000000 txtai-7.1.0/src/python/txtai/graph/topics.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.476750 txtai-7.1.0/src/python/txtai/models/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      176 2023-10-06 15:17:23.000000 txtai-7.1.0/src/python/txtai/models/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7543 2024-02-28 00:08:15.000000 txtai-7.1.0/src/python/txtai/models/models.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3508 2023-02-19 19:01:48.000000 txtai-7.1.0/src/python/txtai/models/onnx.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.476750 txtai-7.1.0/src/python/txtai/models/pooling/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      146 2023-10-09 16:17:44.000000 txtai-7.1.0/src/python/txtai/models/pooling/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3112 2024-02-28 00:07:11.000000 txtai-7.1.0/src/python/txtai/models/pooling/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      563 2023-10-09 16:01:10.000000 txtai-7.1.0/src/python/txtai/models/pooling/cls.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2351 2024-02-28 00:04:26.000000 txtai-7.1.0/src/python/txtai/models/pooling/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      801 2023-10-06 16:10:02.000000 txtai-7.1.0/src/python/txtai/models/pooling/mean.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1384 2022-10-27 19:39:43.000000 txtai-7.1.0/src/python/txtai/models/registry.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4659 2023-04-14 21:23:31.000000 txtai-7.1.0/src/python/txtai/models/tokendetection.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.477749 txtai-7.1.0/src/python/txtai/pipeline/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      326 2023-12-09 16:19:47.000000 txtai-7.1.0/src/python/txtai/pipeline/__init__.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.477749 txtai-7.1.0/src/python/txtai/pipeline/audio/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      103 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/audio/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3823 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/audio/texttospeech.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6568 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/audio/transcription.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      536 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/base.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.477749 txtai-7.1.0/src/python/txtai/pipeline/data/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      161 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/data/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3765 2023-11-29 13:00:51.000000 txtai-7.1.0/src/python/txtai/pipeline/data/segmentation.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4093 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/data/tabular.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7455 2024-03-05 18:21:46.000000 txtai-7.1.0/src/python/txtai/pipeline/data/textractor.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4236 2023-12-03 15:18:53.000000 txtai-7.1.0/src/python/txtai/pipeline/data/tokenizer.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1782 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3684 2023-09-26 13:45:56.000000 txtai-7.1.0/src/python/txtai/pipeline/hfmodel.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3530 2023-09-26 13:33:11.000000 txtai-7.1.0/src/python/txtai/pipeline/hfpipeline.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.477749 txtai-7.1.0/src/python/txtai/pipeline/image/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      114 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/image/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1523 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/image/caption.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2546 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/image/imagehash.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2726 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/image/objects.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.477749 txtai-7.1.0/src/python/txtai/pipeline/llm/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      200 2023-12-09 16:43:34.000000 txtai-7.1.0/src/python/txtai/pipeline/llm/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1998 2023-12-09 11:31:56.000000 txtai-7.1.0/src/python/txtai/pipeline/llm/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2154 2023-12-09 03:15:53.000000 txtai-7.1.0/src/python/txtai/pipeline/llm/generation.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3710 2023-12-09 01:27:30.000000 txtai-7.1.0/src/python/txtai/pipeline/llm/huggingface.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1868 2023-12-26 16:19:57.000000 txtai-7.1.0/src/python/txtai/pipeline/llm/litellm.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1841 2023-12-09 17:55:52.000000 txtai-7.1.0/src/python/txtai/pipeline/llm/llama.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1267 2023-12-09 16:40:59.000000 txtai-7.1.0/src/python/txtai/pipeline/llm/llm.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      189 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/nop.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1058 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/tensors.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.478750 txtai-7.1.0/src/python/txtai/pipeline/text/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      282 2023-12-09 16:19:47.000000 txtai-7.1.0/src/python/txtai/pipeline/text/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2619 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/text/crossencoder.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2539 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/text/entity.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    17142 2023-12-16 17:56:03.000000 txtai-7.1.0/src/python/txtai/pipeline/text/extractor.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5328 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/text/labels.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1417 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/text/questions.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2257 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/text/similarity.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2836 2023-07-08 20:26:24.000000 txtai-7.1.0/src/python/txtai/pipeline/text/summary.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9333 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/text/translation.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.478750 txtai-7.1.0/src/python/txtai/pipeline/train/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      110 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/train/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5998 2023-10-09 15:52:01.000000 txtai-7.1.0/src/python/txtai/pipeline/train/hfonnx.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    13634 2024-01-31 20:03:20.000000 txtai-7.1.0/src/python/txtai/pipeline/train/hftrainer.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1991 2023-07-07 22:15:31.000000 txtai-7.1.0/src/python/txtai/pipeline/train/mlonnx.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.478750 txtai-7.1.0/src/python/txtai/scoring/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      156 2023-07-18 19:36:05.000000 txtai-7.1.0/src/python/txtai/scoring/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    12600 2023-09-02 13:44:59.000000 txtai-7.1.0/src/python/txtai/scoring/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      673 2023-07-27 01:21:09.000000 txtai-7.1.0/src/python/txtai/scoring/bm25.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1603 2023-09-06 21:23:10.000000 txtai-7.1.0/src/python/txtai/scoring/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      846 2023-07-20 01:44:25.000000 txtai-7.1.0/src/python/txtai/scoring/sif.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    14471 2023-08-08 10:55:46.000000 txtai-7.1.0/src/python/txtai/scoring/terms.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.478750 txtai-7.1.0/src/python/txtai/util/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       96 2023-10-03 17:56:55.000000 txtai-7.1.0/src/python/txtai/util/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      565 2023-07-10 16:06:01.000000 txtai-7.1.0/src/python/txtai/util/resolver.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      349 2023-10-03 18:38:54.000000 txtai-7.1.0/src/python/txtai/util/template.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.479750 txtai-7.1.0/src/python/txtai/vectors/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      201 2022-05-12 15:49:17.000000 txtai-7.1.0/src/python/txtai/vectors/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9070 2024-03-11 01:48:40.000000 txtai-7.1.0/src/python/txtai/vectors/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1569 2024-02-27 23:36:17.000000 txtai-7.1.0/src/python/txtai/vectors/external.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1945 2024-02-27 22:21:09.000000 txtai-7.1.0/src/python/txtai/vectors/factory.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2115 2024-02-28 02:20:24.000000 txtai-7.1.0/src/python/txtai/vectors/transformers.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6590 2024-02-27 23:36:29.000000 txtai-7.1.0/src/python/txtai/vectors/words.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      111 2024-02-22 01:16:23.000000 txtai-7.1.0/src/python/txtai/version.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.479750 txtai-7.1.0/src/python/txtai/workflow/
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      139 2023-03-21 22:13:38.000000 txtai-7.1.0/src/python/txtai/workflow/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5486 2023-04-14 21:51:47.000000 txtai-7.1.0/src/python/txtai/workflow/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2845 2021-12-05 00:26:44.000000 txtai-7.1.0/src/python/txtai/workflow/execute.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      965 2023-04-14 21:51:47.000000 txtai-7.1.0/src/python/txtai/workflow/factory.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.479750 txtai-7.1.0/src/python/txtai/workflow/task/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      440 2023-04-14 21:51:47.000000 txtai-7.1.0/src/python/txtai/workflow/task/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    14712 2023-03-11 17:31:41.000000 txtai-7.1.0/src/python/txtai/workflow/task/base.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      492 2022-02-01 02:31:47.000000 txtai-7.1.0/src/python/txtai/workflow/task/console.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1567 2022-02-01 21:55:52.000000 txtai-7.1.0/src/python/txtai/workflow/task/export.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2200 2023-03-02 22:27:53.000000 txtai-7.1.0/src/python/txtai/workflow/task/factory.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      560 2022-01-10 15:07:33.000000 txtai-7.1.0/src/python/txtai/workflow/task/file.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      732 2022-09-11 23:47:05.000000 txtai-7.1.0/src/python/txtai/workflow/task/image.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1711 2023-10-03 16:41:51.000000 txtai-7.1.0/src/python/txtai/workflow/task/retrieve.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3038 2022-02-09 21:00:35.000000 txtai-7.1.0/src/python/txtai/workflow/task/service.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3295 2024-03-05 16:14:02.000000 txtai-7.1.0/src/python/txtai/workflow/task/storage.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      935 2023-04-17 14:31:28.000000 txtai-7.1.0/src/python/txtai/workflow/task/stream.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3453 2023-10-14 10:26:45.000000 txtai-7.1.0/src/python/txtai/workflow/task/template.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      346 2022-01-21 00:01:04.000000 txtai-7.1.0/src/python/txtai/workflow/task/url.py
--rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      232 2021-11-26 17:08:18.000000 txtai-7.1.0/src/python/txtai/workflow/task/workflow.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 13:07:55.472750 txtai-7.1.0/src/python/txtai.egg-info/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    26266 2024-04-19 13:07:55.000000 txtai-7.1.0/src/python/txtai.egg-info/PKG-INFO
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7552 2024-04-19 13:07:55.000000 txtai-7.1.0/src/python/txtai.egg-info/SOURCES.txt
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        1 2024-04-19 13:07:55.000000 txtai-7.1.0/src/python/txtai.egg-info/dependency_links.txt
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2438 2024-04-19 13:07:55.000000 txtai-7.1.0/src/python/txtai.egg-info/requires.txt
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        6 2024-04-19 13:07:55.000000 txtai-7.1.0/src/python/txtai.egg-info/top_level.txt
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.574871 txtai-7.2.0/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)    10754 2021-01-12 02:31:22.000000 txtai-7.2.0/LICENSE
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    28083 2024-05-31 14:50:58.574871 txtai-7.2.0/PKG-INFO
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    18921 2024-05-30 18:53:07.000000 txtai-7.2.0/README.md
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)       31 2021-01-23 16:25:29.000000 txtai-7.2.0/pyproject.toml
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       38 2024-05-31 14:50:58.574871 txtai-7.2.0/setup.cfg
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4286 2024-05-31 11:50:10.000000 txtai-7.2.0/setup.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.554871 txtai-7.2.0/src/
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.554871 txtai-7.2.0/src/python/
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.555871 txtai-7.2.0/src/python/txtai/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      291 2024-01-29 15:16:27.000000 txtai-7.2.0/src/python/txtai/__init__.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.556871 txtai-7.2.0/src/python/txtai/ann/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      229 2024-04-24 15:05:47.000000 txtai-7.2.0/src/python/txtai/ann/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1879 2024-04-23 12:57:16.000000 txtai-7.2.0/src/python/txtai/ann/annoy.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3305 2024-05-08 21:22:30.000000 txtai-7.2.0/src/python/txtai/ann/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1569 2024-04-24 15:05:47.000000 txtai-7.2.0/src/python/txtai/ann/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6526 2023-11-04 13:45:52.000000 txtai-7.2.0/src/python/txtai/ann/faiss.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3200 2024-04-23 12:57:09.000000 txtai-7.2.0/src/python/txtai/ann/hnsw.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4085 2023-10-27 19:09:06.000000 txtai-7.2.0/src/python/txtai/ann/numpy.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3987 2024-05-08 20:51:34.000000 txtai-7.2.0/src/python/txtai/ann/pgvector.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      894 2023-10-27 19:03:54.000000 txtai-7.2.0/src/python/txtai/ann/torch.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.556871 txtai-7.2.0/src/python/txtai/api/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      510 2024-03-30 12:38:43.000000 txtai-7.2.0/src/python/txtai/api/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2931 2024-02-05 22:48:18.000000 txtai-7.2.0/src/python/txtai/api/application.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1312 2023-12-26 16:31:07.000000 txtai-7.2.0/src/python/txtai/api/authorization.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4736 2024-02-20 16:43:38.000000 txtai-7.2.0/src/python/txtai/api/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8500 2024-02-20 16:44:37.000000 txtai-7.2.0/src/python/txtai/api/cluster.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      369 2021-04-09 22:58:59.000000 txtai-7.2.0/src/python/txtai/api/extension.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      640 2024-02-06 16:31:35.000000 txtai-7.2.0/src/python/txtai/api/factory.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.556871 txtai-7.2.0/src/python/txtai/api/responses/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      153 2024-02-06 01:16:00.000000 txtai-7.2.0/src/python/txtai/api/responses/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      608 2024-02-05 22:28:09.000000 txtai-7.2.0/src/python/txtai/api/responses/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1318 2024-02-06 16:38:51.000000 txtai-7.2.0/src/python/txtai/api/responses/json.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1007 2024-02-06 16:39:02.000000 txtai-7.2.0/src/python/txtai/api/responses/messagepack.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1375 2024-02-06 16:39:23.000000 txtai-7.2.0/src/python/txtai/api/route.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.557871 txtai-7.2.0/src/python/txtai/api/routers/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      357 2024-02-04 12:33:23.000000 txtai-7.2.0/src/python/txtai/api/routers/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      741 2024-02-06 16:31:35.000000 txtai-7.2.0/src/python/txtai/api/routers/caption.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7615 2024-02-20 16:53:10.000000 txtai-7.2.0/src/python/txtai/api/routers/embeddings.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      807 2024-02-06 16:31:35.000000 txtai-7.2.0/src/python/txtai/api/routers/entity.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      658 2024-02-06 16:31:35.000000 txtai-7.2.0/src/python/txtai/api/routers/extractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1212 2024-02-06 16:31:35.000000 txtai-7.2.0/src/python/txtai/api/routers/labels.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      843 2024-02-06 16:31:35.000000 txtai-7.2.0/src/python/txtai/api/routers/objects.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      769 2024-02-06 16:31:35.000000 txtai-7.2.0/src/python/txtai/api/routers/segmentation.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1210 2024-02-06 16:31:35.000000 txtai-7.2.0/src/python/txtai/api/routers/similarity.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1188 2024-02-06 16:31:35.000000 txtai-7.2.0/src/python/txtai/api/routers/summary.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      803 2024-02-06 16:31:35.000000 txtai-7.2.0/src/python/txtai/api/routers/tabular.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      782 2024-02-06 16:31:35.000000 txtai-7.2.0/src/python/txtai/api/routers/textractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      795 2024-02-06 16:31:35.000000 txtai-7.2.0/src/python/txtai/api/routers/transcription.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1272 2024-02-06 16:31:35.000000 txtai-7.2.0/src/python/txtai/api/routers/translation.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      593 2024-02-06 16:31:35.000000 txtai-7.2.0/src/python/txtai/api/routers/workflow.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.557871 txtai-7.2.0/src/python/txtai/app/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       66 2022-03-01 18:21:41.000000 txtai-7.2.0/src/python/txtai/app/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    24371 2024-05-25 10:27:07.000000 txtai-7.2.0/src/python/txtai/app/base.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.557871 txtai-7.2.0/src/python/txtai/archive/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      160 2023-02-19 13:31:37.000000 txtai-7.2.0/src/python/txtai/archive/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2840 2023-02-19 18:17:59.000000 txtai-7.2.0/src/python/txtai/archive/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1029 2023-12-04 17:41:19.000000 txtai-7.2.0/src/python/txtai/archive/compress.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      429 2023-02-19 18:15:28.000000 txtai-7.2.0/src/python/txtai/archive/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1272 2023-12-04 14:24:11.000000 txtai-7.2.0/src/python/txtai/archive/tar.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1027 2023-12-04 17:56:46.000000 txtai-7.2.0/src/python/txtai/archive/zip.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.557871 txtai-7.2.0/src/python/txtai/cloud/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      148 2023-02-17 13:35:20.000000 txtai-7.2.0/src/python/txtai/cloud/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2424 2023-02-19 18:45:23.000000 txtai-7.2.0/src/python/txtai/cloud/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1544 2023-02-19 13:30:19.000000 txtai-7.2.0/src/python/txtai/cloud/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3649 2023-03-03 17:46:20.000000 txtai-7.2.0/src/python/txtai/cloud/hub.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3741 2024-03-05 16:14:02.000000 txtai-7.2.0/src/python/txtai/cloud/storage.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.557871 txtai-7.2.0/src/python/txtai/console/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       51 2022-03-29 00:05:18.000000 txtai-7.2.0/src/python/txtai/console/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      274 2022-03-29 16:55:55.000000 txtai-7.2.0/src/python/txtai/console/__main__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6590 2023-02-19 19:08:09.000000 txtai-7.2.0/src/python/txtai/console/base.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.558871 txtai-7.2.0/src/python/txtai/data/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      190 2023-01-01 14:12:39.000000 txtai-7.2.0/src/python/txtai/data/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3958 2023-01-09 14:39:56.000000 txtai-7.2.0/src/python/txtai/data/base.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1198 2022-11-26 00:37:43.000000 txtai-7.2.0/src/python/txtai/data/labels.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     4599 2022-04-16 12:34:51.000000 txtai-7.2.0/src/python/txtai/data/questions.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1336 2022-04-11 19:50:27.000000 txtai-7.2.0/src/python/txtai/data/sequences.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1883 2023-01-09 15:33:33.000000 txtai-7.2.0/src/python/txtai/data/texts.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      579 2022-12-04 18:56:16.000000 txtai-7.2.0/src/python/txtai/data/tokens.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.558871 txtai-7.2.0/src/python/txtai/database/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      291 2023-08-22 13:28:05.000000 txtai-7.2.0/src/python/txtai/database/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9740 2024-05-09 19:16:12.000000 txtai-7.2.0/src/python/txtai/database/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5335 2024-05-09 19:16:12.000000 txtai-7.2.0/src/python/txtai/database/client.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4381 2023-11-07 15:54:54.000000 txtai-7.2.0/src/python/txtai/database/duckdb.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1801 2024-04-17 12:20:59.000000 txtai-7.2.0/src/python/txtai/database/embedded.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.558871 txtai-7.2.0/src/python/txtai/database/encoder/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      153 2021-12-22 11:16:40.000000 txtai-7.2.0/src/python/txtai/database/encoder/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      719 2022-05-27 12:13:14.000000 txtai-7.2.0/src/python/txtai/database/encoder/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1001 2022-09-20 17:06:23.000000 txtai-7.2.0/src/python/txtai/database/encoder/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      904 2023-04-21 14:52:54.000000 txtai-7.2.0/src/python/txtai/database/encoder/image.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      435 2023-08-07 00:41:39.000000 txtai-7.2.0/src/python/txtai/database/encoder/pickle.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1790 2024-04-24 00:32:39.000000 txtai-7.2.0/src/python/txtai/database/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    16462 2024-05-09 19:16:12.000000 txtai-7.2.0/src/python/txtai/database/rdbms.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.558871 txtai-7.2.0/src/python/txtai/database/schema/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       76 2023-08-22 09:49:40.000000 txtai-7.2.0/src/python/txtai/database/schema/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2321 2023-08-26 00:47:23.000000 txtai-7.2.0/src/python/txtai/database/schema/orm.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3110 2023-09-19 13:47:26.000000 txtai-7.2.0/src/python/txtai/database/schema/statement.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.559871 txtai-7.2.0/src/python/txtai/database/sql/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      146 2022-03-01 13:12:16.000000 txtai-7.2.0/src/python/txtai/database/sql/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5315 2021-12-26 16:01:02.000000 txtai-7.2.0/src/python/txtai/database/sql/aggregate.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6198 2023-10-26 16:22:14.000000 txtai-7.2.0/src/python/txtai/database/sql/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    13855 2023-11-07 01:06:06.000000 txtai-7.2.0/src/python/txtai/database/sql/expression.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     8869 2022-11-19 15:44:37.000000 txtai-7.2.0/src/python/txtai/database/sql/token.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1588 2023-08-22 13:25:25.000000 txtai-7.2.0/src/python/txtai/database/sqlite.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.559871 txtai-7.2.0/src/python/txtai/embeddings/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      100 2023-08-09 11:18:31.000000 txtai-7.2.0/src/python/txtai/embeddings/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    33422 2024-05-27 23:58:54.000000 txtai-7.2.0/src/python/txtai/embeddings/base.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.559871 txtai-7.2.0/src/python/txtai/embeddings/index/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      293 2024-02-02 12:33:35.000000 txtai-7.2.0/src/python/txtai/embeddings/index/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      152 2023-07-09 19:17:44.000000 txtai-7.2.0/src/python/txtai/embeddings/index/action.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2154 2023-07-10 16:44:09.000000 txtai-7.2.0/src/python/txtai/embeddings/index/autoid.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1890 2023-08-09 09:52:25.000000 txtai-7.2.0/src/python/txtai/embeddings/index/documents.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4329 2023-08-08 10:14:35.000000 txtai-7.2.0/src/python/txtai/embeddings/index/functions.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4568 2024-02-28 15:34:15.000000 txtai-7.2.0/src/python/txtai/embeddings/index/indexes.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1286 2024-01-30 20:32:31.000000 txtai-7.2.0/src/python/txtai/embeddings/index/indexids.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     2714 2024-04-23 13:03:11.000000 txtai-7.2.0/src/python/txtai/embeddings/index/reducer.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2109 2023-08-23 14:12:53.000000 txtai-7.2.0/src/python/txtai/embeddings/index/stream.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7192 2024-01-19 01:38:26.000000 txtai-7.2.0/src/python/txtai/embeddings/index/transform.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.559871 txtai-7.2.0/src/python/txtai/embeddings/search/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      194 2024-01-21 13:37:35.000000 txtai-7.2.0/src/python/txtai/embeddings/search/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9490 2024-03-31 16:05:43.000000 txtai-7.2.0/src/python/txtai/embeddings/search/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      138 2023-08-08 13:42:50.000000 txtai-7.2.0/src/python/txtai/embeddings/search/errors.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4132 2023-07-25 21:39:08.000000 txtai-7.2.0/src/python/txtai/embeddings/search/explain.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1305 2024-01-30 16:48:28.000000 txtai-7.2.0/src/python/txtai/embeddings/search/ids.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1783 2022-04-18 19:57:38.000000 txtai-7.2.0/src/python/txtai/embeddings/search/query.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6023 2023-11-07 15:38:49.000000 txtai-7.2.0/src/python/txtai/embeddings/search/scan.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1145 2023-03-02 22:24:02.000000 txtai-7.2.0/src/python/txtai/embeddings/search/terms.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.560871 txtai-7.2.0/src/python/txtai/graph/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      164 2024-04-24 15:19:27.000000 txtai-7.2.0/src/python/txtai/graph/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    22156 2024-05-08 21:22:14.000000 txtai-7.2.0/src/python/txtai/graph/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1225 2024-04-24 15:20:11.000000 txtai-7.2.0/src/python/txtai/graph/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6550 2024-04-24 15:19:27.000000 txtai-7.2.0/src/python/txtai/graph/networkx.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2577 2024-05-25 10:27:07.000000 txtai-7.2.0/src/python/txtai/graph/rdbms.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4549 2024-01-22 22:57:23.000000 txtai-7.2.0/src/python/txtai/graph/topics.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.560871 txtai-7.2.0/src/python/txtai/models/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      176 2023-10-06 15:17:23.000000 txtai-7.2.0/src/python/txtai/models/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7543 2024-02-28 00:08:15.000000 txtai-7.2.0/src/python/txtai/models/models.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3667 2024-05-20 21:10:40.000000 txtai-7.2.0/src/python/txtai/models/onnx.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.560871 txtai-7.2.0/src/python/txtai/models/pooling/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      146 2023-10-09 16:17:44.000000 txtai-7.2.0/src/python/txtai/models/pooling/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3112 2024-02-28 00:07:11.000000 txtai-7.2.0/src/python/txtai/models/pooling/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      563 2023-10-09 16:01:10.000000 txtai-7.2.0/src/python/txtai/models/pooling/cls.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2351 2024-02-28 00:04:26.000000 txtai-7.2.0/src/python/txtai/models/pooling/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      801 2023-10-06 16:10:02.000000 txtai-7.2.0/src/python/txtai/models/pooling/mean.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     1384 2022-10-27 19:39:43.000000 txtai-7.2.0/src/python/txtai/models/registry.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4659 2023-04-14 21:23:31.000000 txtai-7.2.0/src/python/txtai/models/tokendetection.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.560871 txtai-7.2.0/src/python/txtai/pipeline/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      326 2023-12-09 16:19:47.000000 txtai-7.2.0/src/python/txtai/pipeline/__init__.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.561871 txtai-7.2.0/src/python/txtai/pipeline/audio/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      103 2023-07-07 22:15:31.000000 txtai-7.2.0/src/python/txtai/pipeline/audio/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3823 2023-07-07 22:15:31.000000 txtai-7.2.0/src/python/txtai/pipeline/audio/texttospeech.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6568 2023-07-08 20:26:24.000000 txtai-7.2.0/src/python/txtai/pipeline/audio/transcription.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      536 2023-07-07 22:15:31.000000 txtai-7.2.0/src/python/txtai/pipeline/base.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.561871 txtai-7.2.0/src/python/txtai/pipeline/data/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      161 2023-07-07 22:15:31.000000 txtai-7.2.0/src/python/txtai/pipeline/data/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3765 2023-11-29 13:00:51.000000 txtai-7.2.0/src/python/txtai/pipeline/data/segmentation.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4093 2023-07-07 22:15:31.000000 txtai-7.2.0/src/python/txtai/pipeline/data/tabular.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7455 2024-03-05 18:21:46.000000 txtai-7.2.0/src/python/txtai/pipeline/data/textractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4236 2023-12-03 15:18:53.000000 txtai-7.2.0/src/python/txtai/pipeline/data/tokenizer.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1782 2023-07-07 22:15:31.000000 txtai-7.2.0/src/python/txtai/pipeline/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3684 2023-09-26 13:45:56.000000 txtai-7.2.0/src/python/txtai/pipeline/hfmodel.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3530 2024-05-20 20:24:48.000000 txtai-7.2.0/src/python/txtai/pipeline/hfpipeline.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.561871 txtai-7.2.0/src/python/txtai/pipeline/image/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      114 2023-07-07 22:15:31.000000 txtai-7.2.0/src/python/txtai/pipeline/image/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1523 2023-07-08 20:26:24.000000 txtai-7.2.0/src/python/txtai/pipeline/image/caption.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2546 2023-07-07 22:15:31.000000 txtai-7.2.0/src/python/txtai/pipeline/image/imagehash.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2726 2023-07-08 20:26:24.000000 txtai-7.2.0/src/python/txtai/pipeline/image/objects.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.561871 txtai-7.2.0/src/python/txtai/pipeline/llm/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      200 2023-12-09 16:43:34.000000 txtai-7.2.0/src/python/txtai/pipeline/llm/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1998 2023-12-09 11:31:56.000000 txtai-7.2.0/src/python/txtai/pipeline/llm/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2441 2024-05-18 17:57:21.000000 txtai-7.2.0/src/python/txtai/pipeline/llm/generation.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3930 2024-05-18 17:57:26.000000 txtai-7.2.0/src/python/txtai/pipeline/llm/huggingface.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1660 2024-05-18 11:34:59.000000 txtai-7.2.0/src/python/txtai/pipeline/llm/litellm.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2923 2024-05-28 17:53:46.000000 txtai-7.2.0/src/python/txtai/pipeline/llm/llama.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1416 2024-05-18 17:57:14.000000 txtai-7.2.0/src/python/txtai/pipeline/llm/llm.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      189 2023-07-07 22:15:31.000000 txtai-7.2.0/src/python/txtai/pipeline/nop.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1058 2023-07-07 22:15:31.000000 txtai-7.2.0/src/python/txtai/pipeline/tensors.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.562871 txtai-7.2.0/src/python/txtai/pipeline/text/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      282 2023-12-09 16:19:47.000000 txtai-7.2.0/src/python/txtai/pipeline/text/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2619 2023-07-08 20:26:24.000000 txtai-7.2.0/src/python/txtai/pipeline/text/crossencoder.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2539 2023-07-08 20:26:24.000000 txtai-7.2.0/src/python/txtai/pipeline/text/entity.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    17142 2023-12-16 17:56:03.000000 txtai-7.2.0/src/python/txtai/pipeline/text/extractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5328 2023-07-08 20:26:24.000000 txtai-7.2.0/src/python/txtai/pipeline/text/labels.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1417 2023-07-08 20:26:24.000000 txtai-7.2.0/src/python/txtai/pipeline/text/questions.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2257 2023-07-08 20:26:24.000000 txtai-7.2.0/src/python/txtai/pipeline/text/similarity.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2836 2023-07-08 20:26:24.000000 txtai-7.2.0/src/python/txtai/pipeline/text/summary.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9333 2023-07-07 22:15:31.000000 txtai-7.2.0/src/python/txtai/pipeline/text/translation.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.562871 txtai-7.2.0/src/python/txtai/pipeline/train/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      110 2023-07-07 22:15:31.000000 txtai-7.2.0/src/python/txtai/pipeline/train/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5998 2024-05-18 19:15:37.000000 txtai-7.2.0/src/python/txtai/pipeline/train/hfonnx.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    13634 2024-01-31 20:03:20.000000 txtai-7.2.0/src/python/txtai/pipeline/train/hftrainer.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2047 2024-05-31 11:54:32.000000 txtai-7.2.0/src/python/txtai/pipeline/train/mlonnx.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.562871 txtai-7.2.0/src/python/txtai/scoring/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      208 2024-05-09 19:21:49.000000 txtai-7.2.0/src/python/txtai/scoring/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3560 2024-05-09 19:21:49.000000 txtai-7.2.0/src/python/txtai/scoring/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      670 2024-05-09 19:21:49.000000 txtai-7.2.0/src/python/txtai/scoring/bm25.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1643 2024-05-09 19:21:49.000000 txtai-7.2.0/src/python/txtai/scoring/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4628 2024-05-09 20:40:20.000000 txtai-7.2.0/src/python/txtai/scoring/pgtext.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      843 2024-05-09 19:21:49.000000 txtai-7.2.0/src/python/txtai/scoring/sif.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    14471 2024-05-08 20:59:40.000000 txtai-7.2.0/src/python/txtai/scoring/terms.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    10135 2024-05-07 16:20:55.000000 txtai-7.2.0/src/python/txtai/scoring/tfidf.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.562871 txtai-7.2.0/src/python/txtai/util/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       96 2023-10-03 17:56:55.000000 txtai-7.2.0/src/python/txtai/util/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      565 2023-07-10 16:06:01.000000 txtai-7.2.0/src/python/txtai/util/resolver.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      349 2023-10-03 18:38:54.000000 txtai-7.2.0/src/python/txtai/util/template.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.563871 txtai-7.2.0/src/python/txtai/vectors/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      240 2024-05-28 12:24:49.000000 txtai-7.2.0/src/python/txtai/vectors/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     9050 2024-05-29 17:43:16.000000 txtai-7.2.0/src/python/txtai/vectors/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1455 2024-05-28 12:24:49.000000 txtai-7.2.0/src/python/txtai/vectors/external.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3192 2024-05-28 12:24:49.000000 txtai-7.2.0/src/python/txtai/vectors/factory.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2533 2024-05-27 21:40:34.000000 txtai-7.2.0/src/python/txtai/vectors/huggingface.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1606 2024-05-28 12:26:18.000000 txtai-7.2.0/src/python/txtai/vectors/litellm.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2147 2024-05-28 17:53:46.000000 txtai-7.2.0/src/python/txtai/vectors/llama.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     6570 2024-05-01 11:06:24.000000 txtai-7.2.0/src/python/txtai/vectors/words.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      111 2024-04-19 19:31:59.000000 txtai-7.2.0/src/python/txtai/version.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.563871 txtai-7.2.0/src/python/txtai/workflow/
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      139 2023-03-21 22:13:38.000000 txtai-7.2.0/src/python/txtai/workflow/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     5486 2023-04-14 21:51:47.000000 txtai-7.2.0/src/python/txtai/workflow/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2902 2024-05-25 10:27:07.000000 txtai-7.2.0/src/python/txtai/workflow/execute.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      965 2023-04-14 21:51:47.000000 txtai-7.2.0/src/python/txtai/workflow/factory.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.563871 txtai-7.2.0/src/python/txtai/workflow/task/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      440 2023-04-14 21:51:47.000000 txtai-7.2.0/src/python/txtai/workflow/task/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    14712 2023-03-11 17:31:41.000000 txtai-7.2.0/src/python/txtai/workflow/task/base.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      492 2022-02-01 02:31:47.000000 txtai-7.2.0/src/python/txtai/workflow/task/console.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1567 2022-02-01 21:55:52.000000 txtai-7.2.0/src/python/txtai/workflow/task/export.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2200 2023-03-02 22:27:53.000000 txtai-7.2.0/src/python/txtai/workflow/task/factory.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      560 2022-01-10 15:07:33.000000 txtai-7.2.0/src/python/txtai/workflow/task/file.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      732 2022-09-11 23:47:05.000000 txtai-7.2.0/src/python/txtai/workflow/task/image.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1711 2023-10-03 16:41:51.000000 txtai-7.2.0/src/python/txtai/workflow/task/retrieve.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)     3038 2022-02-09 21:00:35.000000 txtai-7.2.0/src/python/txtai/workflow/task/service.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3295 2024-03-05 16:14:02.000000 txtai-7.2.0/src/python/txtai/workflow/task/storage.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      935 2023-04-17 14:31:28.000000 txtai-7.2.0/src/python/txtai/workflow/task/stream.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3453 2023-10-14 10:26:45.000000 txtai-7.2.0/src/python/txtai/workflow/task/template.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      346 2022-01-21 00:01:04.000000 txtai-7.2.0/src/python/txtai/workflow/task/url.py
+-rw-rw-r--   0 dmezzett  (1000) dmezzett  (1000)      232 2021-11-26 17:08:18.000000 txtai-7.2.0/src/python/txtai/workflow/task/workflow.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 14:50:58.555871 txtai-7.2.0/src/python/txtai.egg-info/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    28083 2024-05-31 14:50:58.000000 txtai-7.2.0/src/python/txtai.egg-info/PKG-INFO
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     7755 2024-05-31 14:50:58.000000 txtai-7.2.0/src/python/txtai.egg-info/SOURCES.txt
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        1 2024-05-31 14:50:58.000000 txtai-7.2.0/src/python/txtai.egg-info/dependency_links.txt
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2836 2024-05-31 14:50:58.000000 txtai-7.2.0/src/python/txtai.egg-info/requires.txt
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        6 2024-05-31 14:50:58.000000 txtai-7.2.0/src/python/txtai.egg-info/top_level.txt
```

### Comparing `txtai-7.1.0/LICENSE` & `txtai-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/PKG-INFO` & `txtai-7.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txtai
-Version: 7.1.0
+Version: 7.2.0
 Summary: All-in-one open-source embeddings database for semantic search, LLM orchestration and language model workflows
 Home-page: https://github.com/neuml/txtai
 Author: NeuML
 License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/neuml/txtai
 Project-URL: Issue Tracker, https://github.com/neuml/txtai/issues
 Project-URL: Source Code, https://github.com/neuml/txtai
@@ -32,14 +32,19 @@
 Requires-Dist: coveralls; extra == "dev"
 Requires-Dist: httpx; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs-redirects; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
+Provides-Extra: ann
+Requires-Dist: annoy>=1.16.3; extra == "ann"
+Requires-Dist: hnswlib>=0.5.0; extra == "ann"
+Requires-Dist: pgvector>=0.2.5; extra == "ann"
+Requires-Dist: sqlalchemy>=2.0.20; extra == "ann"
 Provides-Extra: api
 Requires-Dist: aiohttp>=3.8.1; extra == "api"
 Requires-Dist: fastapi>=0.94.0; extra == "api"
 Requires-Dist: msgpack>=1.0.7; extra == "api"
 Requires-Dist: pillow>=7.1.2; extra == "api"
 Requires-Dist: python-multipart>=0.0.7; extra == "api"
 Requires-Dist: uvicorn>=0.12.1; extra == "api"
@@ -49,16 +54,18 @@
 Requires-Dist: rich>=12.0.1; extra == "console"
 Provides-Extra: database
 Requires-Dist: duckdb>=0.7.1; extra == "database"
 Requires-Dist: pillow>=7.1.2; extra == "database"
 Requires-Dist: sqlalchemy>=2.0.20; extra == "database"
 Provides-Extra: graph
 Requires-Dist: grand-cypher>=0.6.0; extra == "graph"
+Requires-Dist: grand-graph>=0.5.0; extra == "graph"
 Requires-Dist: networkx>=2.6.3; extra == "graph"
 Requires-Dist: python-louvain>=0.16; extra == "graph"
+Requires-Dist: sqlalchemy>=2.0.20; extra == "graph"
 Provides-Extra: model
 Requires-Dist: onnx>=1.11.0; extra == "model"
 Requires-Dist: onnxruntime>=1.11.0; extra == "model"
 Provides-Extra: pipeline-audio
 Requires-Dist: onnx>=1.11.0; extra == "pipeline-audio"
 Requires-Dist: onnxruntime>=1.11.0; extra == "pipeline-audio"
 Requires-Dist: soundfile>=0.10.3.post1; extra == "pipeline-audio"
@@ -70,16 +77,16 @@
 Requires-Dist: pandas>=1.1.0; extra == "pipeline-data"
 Requires-Dist: tika>=1.24; extra == "pipeline-data"
 Provides-Extra: pipeline-image
 Requires-Dist: imagehash>=4.2.1; extra == "pipeline-image"
 Requires-Dist: pillow>=7.1.2; extra == "pipeline-image"
 Requires-Dist: timm>=0.4.12; extra == "pipeline-image"
 Provides-Extra: pipeline-llm
-Requires-Dist: litellm>=1.31.2; extra == "pipeline-llm"
-Requires-Dist: llama-cpp-python>=0.2.20; extra == "pipeline-llm"
+Requires-Dist: litellm>=1.37.16; extra == "pipeline-llm"
+Requires-Dist: llama-cpp-python>=0.2.75; extra == "pipeline-llm"
 Provides-Extra: pipeline-text
 Requires-Dist: fasttext>=0.9.2; extra == "pipeline-text"
 Requires-Dist: sentencepiece>=0.1.91; extra == "pipeline-text"
 Provides-Extra: pipeline-train
 Requires-Dist: accelerate>=0.26.0; extra == "pipeline-train"
 Requires-Dist: bitsandbytes>=0.42.0; extra == "pipeline-train"
 Requires-Dist: onnx>=1.11.0; extra == "pipeline-train"
@@ -96,83 +103,103 @@
 Requires-Dist: beautifulsoup4>=4.9.3; extra == "pipeline"
 Requires-Dist: nltk>=3.5; extra == "pipeline"
 Requires-Dist: pandas>=1.1.0; extra == "pipeline"
 Requires-Dist: tika>=1.24; extra == "pipeline"
 Requires-Dist: imagehash>=4.2.1; extra == "pipeline"
 Requires-Dist: pillow>=7.1.2; extra == "pipeline"
 Requires-Dist: timm>=0.4.12; extra == "pipeline"
-Requires-Dist: litellm>=1.31.2; extra == "pipeline"
-Requires-Dist: llama-cpp-python>=0.2.20; extra == "pipeline"
+Requires-Dist: litellm>=1.37.16; extra == "pipeline"
+Requires-Dist: llama-cpp-python>=0.2.75; extra == "pipeline"
 Requires-Dist: fasttext>=0.9.2; extra == "pipeline"
 Requires-Dist: sentencepiece>=0.1.91; extra == "pipeline"
 Requires-Dist: accelerate>=0.26.0; extra == "pipeline"
 Requires-Dist: bitsandbytes>=0.42.0; extra == "pipeline"
 Requires-Dist: onnx>=1.11.0; extra == "pipeline"
 Requires-Dist: onnxmltools>=1.9.1; extra == "pipeline"
 Requires-Dist: onnxruntime>=1.11.0; extra == "pipeline"
 Requires-Dist: peft>=0.8.1; extra == "pipeline"
 Requires-Dist: skl2onnx>=1.9.1; extra == "pipeline"
-Provides-Extra: similarity
-Requires-Dist: annoy>=1.16.3; extra == "similarity"
-Requires-Dist: fasttext>=0.9.2; extra == "similarity"
-Requires-Dist: hnswlib>=0.5.0; extra == "similarity"
-Requires-Dist: pymagnitude-lite>=0.1.43; extra == "similarity"
-Requires-Dist: scikit-learn>=0.23.1; extra == "similarity"
-Requires-Dist: sentence-transformers>=2.2.0; extra == "similarity"
+Provides-Extra: scoring
+Requires-Dist: sqlalchemy>=2.0.20; extra == "scoring"
+Provides-Extra: vectors
+Requires-Dist: fasttext>=0.9.2; extra == "vectors"
+Requires-Dist: litellm>=1.37.16; extra == "vectors"
+Requires-Dist: llama-cpp-python>=0.2.75; extra == "vectors"
+Requires-Dist: pymagnitude-lite>=0.1.43; extra == "vectors"
+Requires-Dist: scikit-learn>=0.23.1; extra == "vectors"
+Requires-Dist: sentence-transformers>=2.2.0; extra == "vectors"
 Provides-Extra: workflow
 Requires-Dist: apache-libcloud>=3.3.1; extra == "workflow"
 Requires-Dist: croniter>=1.2.0; extra == "workflow"
 Requires-Dist: openpyxl>=3.0.9; extra == "workflow"
 Requires-Dist: pandas>=1.1.0; extra == "workflow"
 Requires-Dist: pillow>=7.1.2; extra == "workflow"
 Requires-Dist: requests>=2.26.0; extra == "workflow"
 Requires-Dist: xmltodict>=0.12.0; extra == "workflow"
+Provides-Extra: similarity
+Requires-Dist: annoy>=1.16.3; extra == "similarity"
+Requires-Dist: hnswlib>=0.5.0; extra == "similarity"
+Requires-Dist: pgvector>=0.2.5; extra == "similarity"
+Requires-Dist: sqlalchemy>=2.0.20; extra == "similarity"
+Requires-Dist: fasttext>=0.9.2; extra == "similarity"
+Requires-Dist: litellm>=1.37.16; extra == "similarity"
+Requires-Dist: llama-cpp-python>=0.2.75; extra == "similarity"
+Requires-Dist: pymagnitude-lite>=0.1.43; extra == "similarity"
+Requires-Dist: scikit-learn>=0.23.1; extra == "similarity"
+Requires-Dist: sentence-transformers>=2.2.0; extra == "similarity"
 Provides-Extra: all
 Requires-Dist: aiohttp>=3.8.1; extra == "all"
 Requires-Dist: fastapi>=0.94.0; extra == "all"
 Requires-Dist: msgpack>=1.0.7; extra == "all"
 Requires-Dist: pillow>=7.1.2; extra == "all"
 Requires-Dist: python-multipart>=0.0.7; extra == "all"
 Requires-Dist: uvicorn>=0.12.1; extra == "all"
 Requires-Dist: apache-libcloud>=3.3.1; extra == "all"
 Requires-Dist: rich>=12.0.1; extra == "all"
 Requires-Dist: duckdb>=0.7.1; extra == "all"
 Requires-Dist: pillow>=7.1.2; extra == "all"
 Requires-Dist: sqlalchemy>=2.0.20; extra == "all"
 Requires-Dist: grand-cypher>=0.6.0; extra == "all"
+Requires-Dist: grand-graph>=0.5.0; extra == "all"
 Requires-Dist: networkx>=2.6.3; extra == "all"
 Requires-Dist: python-louvain>=0.16; extra == "all"
+Requires-Dist: sqlalchemy>=2.0.20; extra == "all"
 Requires-Dist: onnx>=1.11.0; extra == "all"
 Requires-Dist: onnxruntime>=1.11.0; extra == "all"
 Requires-Dist: onnx>=1.11.0; extra == "all"
 Requires-Dist: onnxruntime>=1.11.0; extra == "all"
 Requires-Dist: soundfile>=0.10.3.post1; extra == "all"
 Requires-Dist: scipy>=1.4.1; extra == "all"
 Requires-Dist: ttstokenizer>=1.0.0; extra == "all"
 Requires-Dist: beautifulsoup4>=4.9.3; extra == "all"
 Requires-Dist: nltk>=3.5; extra == "all"
 Requires-Dist: pandas>=1.1.0; extra == "all"
 Requires-Dist: tika>=1.24; extra == "all"
 Requires-Dist: imagehash>=4.2.1; extra == "all"
 Requires-Dist: pillow>=7.1.2; extra == "all"
 Requires-Dist: timm>=0.4.12; extra == "all"
-Requires-Dist: litellm>=1.31.2; extra == "all"
-Requires-Dist: llama-cpp-python>=0.2.20; extra == "all"
+Requires-Dist: litellm>=1.37.16; extra == "all"
+Requires-Dist: llama-cpp-python>=0.2.75; extra == "all"
 Requires-Dist: fasttext>=0.9.2; extra == "all"
 Requires-Dist: sentencepiece>=0.1.91; extra == "all"
 Requires-Dist: accelerate>=0.26.0; extra == "all"
 Requires-Dist: bitsandbytes>=0.42.0; extra == "all"
 Requires-Dist: onnx>=1.11.0; extra == "all"
 Requires-Dist: onnxmltools>=1.9.1; extra == "all"
 Requires-Dist: onnxruntime>=1.11.0; extra == "all"
 Requires-Dist: peft>=0.8.1; extra == "all"
 Requires-Dist: skl2onnx>=1.9.1; extra == "all"
+Requires-Dist: sqlalchemy>=2.0.20; extra == "all"
 Requires-Dist: annoy>=1.16.3; extra == "all"
-Requires-Dist: fasttext>=0.9.2; extra == "all"
 Requires-Dist: hnswlib>=0.5.0; extra == "all"
+Requires-Dist: pgvector>=0.2.5; extra == "all"
+Requires-Dist: sqlalchemy>=2.0.20; extra == "all"
+Requires-Dist: fasttext>=0.9.2; extra == "all"
+Requires-Dist: litellm>=1.37.16; extra == "all"
+Requires-Dist: llama-cpp-python>=0.2.75; extra == "all"
 Requires-Dist: pymagnitude-lite>=0.1.43; extra == "all"
 Requires-Dist: scikit-learn>=0.23.1; extra == "all"
 Requires-Dist: sentence-transformers>=2.2.0; extra == "all"
 Requires-Dist: apache-libcloud>=3.3.1; extra == "all"
 Requires-Dist: croniter>=1.2.0; extra == "all"
 Requires-Dist: openpyxl>=3.0.9; extra == "all"
 Requires-Dist: pandas>=1.1.0; extra == "all"
@@ -311,14 +338,15 @@
 A novel feature of txtai is that it can provide both an answer and source citation.
 
 | Notebook  | Description  |       |
 |:----------|:-------------|------:|
 | [Build RAG pipelines with txtai](https://github.com/neuml/txtai/blob/master/examples/52_Build_RAG_pipelines_with_txtai.ipynb) | Guide on retrieval augmented generation including how to create citations | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/52_Build_RAG_pipelines_with_txtai.ipynb) |
 | [Advanced RAG with graph path traversal](https://github.com/neuml/txtai/blob/master/examples/58_Advanced_RAG_with_graph_path_traversal.ipynb) | Graph path traversal to collect complex sets of data for advanced RAG | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/58_Advanced_RAG_with_graph_path_traversal.ipynb) |
 | [Advanced RAG with guided generation](https://github.com/neuml/txtai/blob/master/examples/60_Advanced_RAG_with_guided_generation.ipynb) | Retrieval Augmented and Guided Generation | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/60_Advanced_RAG_with_guided_generation.ipynb) |
+| [RAG with llama.cpp and external API services](https://github.com/neuml/txtai/blob/master/examples/62_RAG_with_llama_cpp_and_external_API_services.ipynb) | RAG with additional vector and LLM frameworks | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/62_RAG_with_llama_cpp_and_external_API_services.ipynb) |
 
 ### Language Model Workflows
 
 Language model workflows, also known as semantic workflows, connect language models together to build intelligent applications.
 
 ![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-light-mode-only)
 
@@ -366,14 +394,15 @@
 Models can be loaded as either a path from the Hugging Face Hub or a local directory. Model paths are optional, defaults are loaded when not specified. For tasks with no recommended model, txtai uses the default models as shown in the Hugging Face Tasks guide.
 
 See the following links to learn more.
 
 - [Hugging Face Tasks](https://hf.co/tasks)
 - [Hugging Face Model Hub](https://hf.co/models)
 - [MTEB Leaderboard](https://hf.co/spaces/mteb/leaderboard)
+- [LMSYS LLM Leaderboard](https://chat.lmsys.org/?leaderboard)
 - [Open LLM Leaderboard](https://hf.co/spaces/HuggingFaceH4/open_llm_leaderboard)
 
 ## Powered by txtai
 
 The following applications are powered by txtai.
 
 ![apps](https://raw.githubusercontent.com/neuml/txtai/master/apps.jpg)
```

### Comparing `txtai-7.1.0/README.md` & `txtai-7.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 A novel feature of txtai is that it can provide both an answer and source citation.
 
 | Notebook  | Description  |       |
 |:----------|:-------------|------:|
 | [Build RAG pipelines with txtai](https://github.com/neuml/txtai/blob/master/examples/52_Build_RAG_pipelines_with_txtai.ipynb) | Guide on retrieval augmented generation including how to create citations | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/52_Build_RAG_pipelines_with_txtai.ipynb) |
 | [Advanced RAG with graph path traversal](https://github.com/neuml/txtai/blob/master/examples/58_Advanced_RAG_with_graph_path_traversal.ipynb) | Graph path traversal to collect complex sets of data for advanced RAG | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/58_Advanced_RAG_with_graph_path_traversal.ipynb) |
 | [Advanced RAG with guided generation](https://github.com/neuml/txtai/blob/master/examples/60_Advanced_RAG_with_guided_generation.ipynb) | Retrieval Augmented and Guided Generation | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/60_Advanced_RAG_with_guided_generation.ipynb) |
+| [RAG with llama.cpp and external API services](https://github.com/neuml/txtai/blob/master/examples/62_RAG_with_llama_cpp_and_external_API_services.ipynb) | RAG with additional vector and LLM frameworks | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/62_RAG_with_llama_cpp_and_external_API_services.ipynb) |
 
 ### Language Model Workflows
 
 Language model workflows, also known as semantic workflows, connect language models together to build intelligent applications.
 
 ![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-light-mode-only)
 ![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows-dark.png#gh-dark-mode-only)
@@ -190,14 +191,15 @@
 Models can be loaded as either a path from the Hugging Face Hub or a local directory. Model paths are optional, defaults are loaded when not specified. For tasks with no recommended model, txtai uses the default models as shown in the Hugging Face Tasks guide.
 
 See the following links to learn more.
 
 - [Hugging Face Tasks](https://hf.co/tasks)
 - [Hugging Face Model Hub](https://hf.co/models)
 - [MTEB Leaderboard](https://hf.co/spaces/mteb/leaderboard)
+- [LMSYS LLM Leaderboard](https://chat.lmsys.org/?leaderboard)
 - [Open LLM Leaderboard](https://hf.co/spaces/HuggingFaceH4/open_llm_leaderboard)
 
 ## Powered by txtai
 
 The following applications are powered by txtai.
 
 ![apps](https://raw.githubusercontent.com/neuml/txtai/master/apps.jpg)
```

#### html2text {}

```diff
@@ -119,15 +119,21 @@
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/neuml/txtai/blob/master/examples/
 58_Advanced_RAG_with_graph_path_traversal.ipynb) | | [Advanced RAG with guided
 generation](https://github.com/neuml/txtai/blob/master/examples/
 60_Advanced_RAG_with_guided_generation.ipynb) | Retrieval Augmented and Guided
 Generation | [![Open In Colab](https://colab.research.google.com/assets/colab-
 badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/
-examples/60_Advanced_RAG_with_guided_generation.ipynb) | ### Language Model
+examples/60_Advanced_RAG_with_guided_generation.ipynb) | | [RAG with llama.cpp
+and external API services](https://github.com/neuml/txtai/blob/master/examples/
+62_RAG_with_llama_cpp_and_external_API_services.ipynb) | RAG with additional
+vector and LLM frameworks | [![Open In Colab](https://
+colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/neuml/txtai/blob/master/examples/
+62_RAG_with_llama_cpp_and_external_API_services.ipynb) | ### Language Model
 Workflows Language model workflows, also known as semantic workflows, connect
 language models together to build intelligent applications. ![flows](https://
 raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-light-
 mode-only) ![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/
 images/flows-dark.png#gh-dark-mode-only) While LLMs are powerful, there are
 plenty of smaller, more specialized models that work better and faster for
 specific tasks. This includes models for extractive question-answering,
@@ -190,15 +196,16 @@
 [Translation](https://neuml.github.io/txtai/pipeline/text/translation) | [OPUS
 Model Series](https://hf.co/Helsinki-NLP) | Models can be loaded as either a
 path from the Hugging Face Hub or a local directory. Model paths are optional,
 defaults are loaded when not specified. For tasks with no recommended model,
 txtai uses the default models as shown in the Hugging Face Tasks guide. See the
 following links to learn more. - [Hugging Face Tasks](https://hf.co/tasks) -
 [Hugging Face Model Hub](https://hf.co/models) - [MTEB Leaderboard](https://
-hf.co/spaces/mteb/leaderboard) - [Open LLM Leaderboard](https://hf.co/spaces/
+hf.co/spaces/mteb/leaderboard) - [LMSYS LLM Leaderboard](https://
+chat.lmsys.org/?leaderboard) - [Open LLM Leaderboard](https://hf.co/spaces/
 HuggingFaceH4/open_llm_leaderboard) ## Powered by txtai The following
 applications are powered by txtai. ![apps](https://raw.githubusercontent.com/
 neuml/txtai/master/apps.jpg) | Application | Description | |:------------ |:---
 ----------| | [txtchat](https://github.com/neuml/txtchat) | Retrieval Augmented
 Generation (RAG) powered search | | [paperai](https://github.com/neuml/paperai)
 | Semantic search and workflows for medical/scientific papers | |
 [codequestion](https://github.com/neuml/codequestion) | Semantic search for
```

### Comparing `txtai-7.1.0/setup.py` & `txtai-7.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,21 @@
     "mkdocs-material",
     "mkdocs-redirects",
     "mkdocstrings[python]",
     "pre-commit",
     "pylint",
 ]
 
+extras["ann"] = [
+    "annoy>=1.16.3",
+    "hnswlib>=0.5.0",
+    "pgvector>=0.2.5",
+    "sqlalchemy>=2.0.20",
+]
+
 extras["api"] = [
     "aiohttp>=3.8.1",
     "fastapi>=0.94.0",
     "msgpack>=1.0.7",
     "pillow>=7.1.2",
     "python-multipart>=0.0.7",
     "uvicorn>=0.12.1",
@@ -38,25 +45,25 @@
 
 extras["cloud"] = ["apache-libcloud>=3.3.1"]
 
 extras["console"] = ["rich>=12.0.1"]
 
 extras["database"] = ["duckdb>=0.7.1", "pillow>=7.1.2", "sqlalchemy>=2.0.20"]
 
-extras["graph"] = ["grand-cypher>=0.6.0", "networkx>=2.6.3", "python-louvain>=0.16"]
+extras["graph"] = ["grand-cypher>=0.6.0", "grand-graph>=0.5.0", "networkx>=2.6.3", "python-louvain>=0.16", "sqlalchemy>=2.0.20"]
 
 extras["model"] = ["onnx>=1.11.0", "onnxruntime>=1.11.0"]
 
 extras["pipeline-audio"] = ["onnx>=1.11.0", "onnxruntime>=1.11.0", "soundfile>=0.10.3.post1", "scipy>=1.4.1", "ttstokenizer>=1.0.0"]
 
 extras["pipeline-data"] = ["beautifulsoup4>=4.9.3", "nltk>=3.5", "pandas>=1.1.0", "tika>=1.24"]
 
 extras["pipeline-image"] = ["imagehash>=4.2.1", "pillow>=7.1.2", "timm>=0.4.12"]
 
-extras["pipeline-llm"] = ["litellm>=1.31.2", "llama-cpp-python>=0.2.20"]
+extras["pipeline-llm"] = ["litellm>=1.37.16", "llama-cpp-python>=0.2.75"]
 
 extras["pipeline-text"] = ["fasttext>=0.9.2", "sentencepiece>=0.1.91"]
 
 extras["pipeline-train"] = [
     "accelerate>=0.26.0",
     "bitsandbytes>=0.42.0",
     "onnx>=1.11.0",
@@ -71,18 +78,20 @@
     + extras["pipeline-data"]
     + extras["pipeline-image"]
     + extras["pipeline-llm"]
     + extras["pipeline-text"]
     + extras["pipeline-train"]
 )
 
-extras["similarity"] = [
-    "annoy>=1.16.3",
+extras["scoring"] = ["sqlalchemy>=2.0.20"]
+
+extras["vectors"] = [
     "fasttext>=0.9.2",
-    "hnswlib>=0.5.0",
+    "litellm>=1.37.16",
+    "llama-cpp-python>=0.2.75",
     "pymagnitude-lite>=0.1.43",
     "scikit-learn>=0.23.1",
     "sentence-transformers>=2.2.0",
 ]
 
 extras["workflow"] = [
     "apache-libcloud>=3.3.1",
@@ -90,29 +99,33 @@
     "openpyxl>=3.0.9",
     "pandas>=1.1.0",
     "pillow>=7.1.2",
     "requests>=2.26.0",
     "xmltodict>=0.12.0",
 ]
 
+# Backwards-compatible combination of ann and vectors extra
+extras["similarity"] = extras["ann"] + extras["vectors"]
+
 extras["all"] = (
     extras["api"]
     + extras["cloud"]
     + extras["console"]
     + extras["database"]
     + extras["graph"]
     + extras["model"]
     + extras["pipeline"]
+    + extras["scoring"]
     + extras["similarity"]
     + extras["workflow"]
 )
 
 setup(
     name="txtai",
-    version="7.1.0",
+    version="7.2.0",
     author="NeuML",
     description="All-in-one open-source embeddings database for semantic search, LLM orchestration and language model workflows",
     long_description=DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/neuml/txtai",
     project_urls={
         "Documentation": "https://github.com/neuml/txtai",
```

### Comparing `txtai-7.1.0/src/python/txtai/ann/annoy.py` & `txtai-7.2.0/src/python/txtai/ann/annoy.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Builds an ANN index using the Annoy library.
     """
 
     def __init__(self, config):
         super().__init__(config)
 
         if not ANNOY:
-            raise ImportError('Annoy is not available - install "similarity" extra to enable')
+            raise ImportError('Annoy is not available - install "ann" extra to enable')
 
     def load(self, path):
         # Load index
         self.backend = AnnoyIndex(self.config["dimensions"], self.config["metric"])
         self.backend.load(path)
 
     def index(self, embeddings):
```

### Comparing `txtai-7.1.0/src/python/txtai/ann/base.py` & `txtai-7.2.0/src/python/txtai/ann/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,14 +98,21 @@
 
         Args:
             path: path to save ann index
         """
 
         raise NotImplementedError
 
+    def close(self):
+        """
+        Closes this ANN.
+        """
+
+        self.backend = None
+
     def setting(self, name, default=None):
         """
         Looks up backend specific setting.
 
         Args:
             name: setting name
             default: default value when setting not found
```

### Comparing `txtai-7.1.0/src/python/txtai/ann/factory.py` & `txtai-7.2.0/src/python/txtai/ann/factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from ..util import Resolver
 
 from .annoy import Annoy
 from .faiss import Faiss
 from .hnsw import HNSW
 from .numpy import NumPy
+from .pgvector import PGVector
 from .torch import Torch
 
 
 class ANNFactory:
     """
     Methods to create ANN indexes.
     """
@@ -37,14 +38,16 @@
             ann = Annoy(config)
         elif backend == "faiss":
             ann = Faiss(config)
         elif backend == "hnsw":
             ann = HNSW(config)
         elif backend == "numpy":
             ann = NumPy(config)
+        elif backend == "pgvector":
+            ann = PGVector(config)
         elif backend == "torch":
             ann = Torch(config)
         else:
             ann = ANNFactory.resolve(backend, config)
 
         # Store config back
         config["backend"] = backend
```

### Comparing `txtai-7.1.0/src/python/txtai/ann/faiss.py` & `txtai-7.2.0/src/python/txtai/ann/faiss.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/ann/hnsw.py` & `txtai-7.2.0/src/python/txtai/ann/hnsw.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Builds an ANN index using the hnswlib library.
     """
 
     def __init__(self, config):
         super().__init__(config)
 
         if not HNSWLIB:
-            raise ImportError('HNSW is not available - install "similarity" extra to enable')
+            raise ImportError('HNSW is not available - install "ann" extra to enable')
 
     def load(self, path):
         # Load index
         self.backend = Index(dim=self.config["dimensions"], space=self.config["metric"])
         self.backend.load_index(path)
 
     def index(self, embeddings):
```

### Comparing `txtai-7.1.0/src/python/txtai/ann/numpy.py` & `txtai-7.2.0/src/python/txtai/ann/numpy.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/ann/torch.py` & `txtai-7.2.0/src/python/txtai/ann/torch.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/application.py` & `txtai-7.2.0/src/python/txtai/api/application.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/authorization.py` & `txtai-7.2.0/src/python/txtai/api/authorization.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/base.py` & `txtai-7.2.0/src/python/txtai/api/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/cluster.py` & `txtai-7.2.0/src/python/txtai/api/cluster.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/factory.py` & `txtai-7.2.0/src/python/txtai/api/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/responses/factory.py` & `txtai-7.2.0/src/python/txtai/api/responses/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/responses/json.py` & `txtai-7.2.0/src/python/txtai/api/responses/json.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/responses/messagepack.py` & `txtai-7.2.0/src/python/txtai/api/responses/messagepack.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/route.py` & `txtai-7.2.0/src/python/txtai/api/route.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/routers/caption.py` & `txtai-7.2.0/src/python/txtai/api/routers/caption.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/routers/embeddings.py` & `txtai-7.2.0/src/python/txtai/api/routers/embeddings.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/routers/entity.py` & `txtai-7.2.0/src/python/txtai/api/routers/entity.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/routers/extractor.py` & `txtai-7.2.0/src/python/txtai/api/routers/extractor.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/routers/labels.py` & `txtai-7.2.0/src/python/txtai/api/routers/labels.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/routers/objects.py` & `txtai-7.2.0/src/python/txtai/api/routers/objects.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/routers/segmentation.py` & `txtai-7.2.0/src/python/txtai/api/routers/segmentation.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/routers/similarity.py` & `txtai-7.2.0/src/python/txtai/api/routers/similarity.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/routers/summary.py` & `txtai-7.2.0/src/python/txtai/api/routers/summary.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/routers/tabular.py` & `txtai-7.2.0/src/python/txtai/api/routers/tabular.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/routers/textractor.py` & `txtai-7.2.0/src/python/txtai/api/routers/textractor.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/routers/transcription.py` & `txtai-7.2.0/src/python/txtai/api/routers/transcription.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/routers/translation.py` & `txtai-7.2.0/src/python/txtai/api/routers/translation.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/api/routers/workflow.py` & `txtai-7.2.0/src/python/txtai/api/routers/workflow.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/app/base.py` & `txtai-7.2.0/src/python/txtai/app/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         self.indexes(loaddata)
 
     def __del__(self):
         """
         Close threadpool when this object is garbage collected.
         """
 
-        if self.pool:
+        if hasattr(self, "pool") and self.pool:
             self.pool.close()
             self.pool = None
 
     def pipes(self):
         """
         Initialize pipelines.
         """
```

### Comparing `txtai-7.1.0/src/python/txtai/archive/base.py` & `txtai-7.2.0/src/python/txtai/archive/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/archive/compress.py` & `txtai-7.2.0/src/python/txtai/archive/compress.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/archive/tar.py` & `txtai-7.2.0/src/python/txtai/archive/tar.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/archive/zip.py` & `txtai-7.2.0/src/python/txtai/archive/zip.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/cloud/base.py` & `txtai-7.2.0/src/python/txtai/cloud/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/cloud/factory.py` & `txtai-7.2.0/src/python/txtai/cloud/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/cloud/hub.py` & `txtai-7.2.0/src/python/txtai/cloud/hub.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/cloud/storage.py` & `txtai-7.2.0/src/python/txtai/cloud/storage.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/console/base.py` & `txtai-7.2.0/src/python/txtai/console/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/data/base.py` & `txtai-7.2.0/src/python/txtai/data/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/data/labels.py` & `txtai-7.2.0/src/python/txtai/data/labels.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/data/questions.py` & `txtai-7.2.0/src/python/txtai/data/questions.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/data/sequences.py` & `txtai-7.2.0/src/python/txtai/data/sequences.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/data/texts.py` & `txtai-7.2.0/src/python/txtai/data/texts.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/data/tokens.py` & `txtai-7.2.0/src/python/txtai/data/tokens.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/database/base.py` & `txtai-7.2.0/src/python/txtai/database/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             path: path to write database
         """
 
         raise NotImplementedError
 
     def close(self):
         """
-        Closes the database.
+        Closes this database.
         """
 
         raise NotImplementedError
 
     def ids(self, ids):
         """
         Retrieves the internal indexids for a list of ids. Multiple indexids may be present for an id in cases
```

### Comparing `txtai-7.1.0/src/python/txtai/database/client.py` & `txtai-7.2.0/src/python/txtai/database/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,19 +97,20 @@
 
     def createscores(self):
         # Create temporary scores table, if necessary
         Base.metadata.tables["scores"].create(self.connection.bind, checkfirst=True)
 
     def insertscores(self, scores):
         # Average scores by id
-        self.connection.execute(insert(Score), [{"indexid": i, "score": sum(s) / len(s)} for i, s in scores.items()])
+        if scores:
+            self.connection.execute(insert(Score), [{"indexid": i, "score": sum(s) / len(s)} for i, s in scores.items()])
 
     def connect(self, path=None):
         # Connection URL
-        content = self.config["content"]
+        content = self.config.get("content")
 
         # Read ENV variable, if necessary
         content = os.environ.get("CLIENT_URL") if content == "client" else content
 
         # Create engine using database URL
         engine = create_engine(content, poolclass=StaticPool, echo=False, json_serializer=lambda x: x)
```

### Comparing `txtai-7.1.0/src/python/txtai/database/duckdb.py` & `txtai-7.2.0/src/python/txtai/database/duckdb.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/database/embedded.py` & `txtai-7.2.0/src/python/txtai/database/embedded.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/database/encoder/base.py` & `txtai-7.2.0/src/python/txtai/database/encoder/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/database/encoder/factory.py` & `txtai-7.2.0/src/python/txtai/database/encoder/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/database/encoder/image.py` & `txtai-7.2.0/src/python/txtai/database/encoder/image.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/database/factory.py` & `txtai-7.2.0/src/python/txtai/database/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/database/rdbms.py` & `txtai-7.2.0/src/python/txtai/database/rdbms.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
 
     def initialize(self):
         """
         Creates connection and initial database schema if no connection exists.
         """
 
         if not self.connection:
-            # Create temporary database. Thread locking must be handled externally.
+            # Create database session. Thread locking must be handled externally.
             self.session()
 
             # Create initial table schema
             self.createtables()
 
     def session(self, path=None, connection=None):
         """
@@ -485,15 +485,16 @@
         Inserts a batch of scores.
 
         Args:
             scores: scores to add
         """
 
         # Average scores by id
-        self.cursor.executemany(Statement.INSERT_SCORE, [(i, sum(s) / len(s)) for i, s in scores.items()])
+        if scores:
+            self.cursor.executemany(Statement.INSERT_SCORE, [(i, sum(s) / len(s)) for i, s in scores.items()])
 
     def defaults(self):
         """
         Returns a list of default columns when there is no select clause.
 
         Returns:
             list of default columns
```

### Comparing `txtai-7.1.0/src/python/txtai/database/schema/orm.py` & `txtai-7.2.0/src/python/txtai/database/schema/orm.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/database/schema/statement.py` & `txtai-7.2.0/src/python/txtai/database/schema/statement.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/database/sql/aggregate.py` & `txtai-7.2.0/src/python/txtai/database/sql/aggregate.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/database/sql/base.py` & `txtai-7.2.0/src/python/txtai/database/sql/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/database/sql/expression.py` & `txtai-7.2.0/src/python/txtai/database/sql/expression.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/database/sql/token.py` & `txtai-7.2.0/src/python/txtai/database/sql/token.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/database/sqlite.py` & `txtai-7.2.0/src/python/txtai/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/embeddings/base.py` & `txtai-7.2.0/src/python/txtai/embeddings/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,21 +83,14 @@
 
         # Merge configuration into single dictionary
         config = {**config, **kwargs} if config and kwargs else kwargs if kwargs else config
 
         # Set initial configuration
         self.configure(config)
 
-    def __del__(self):
-        """
-        Clean resources when embeddings is deleted.
-        """
-
-        self.close()
-
     def score(self, documents):
         """
         Builds a term weighting scoring index. Only used by word vectors models.
 
         Args:
             documents: iterable of (id, data, tags), (id, data) or data
         """
@@ -320,15 +313,15 @@
 
         # Initialize default parameters, if necessary
         self.defaults()
 
         # Default vector model, if necessary
         model = self.model if self.model else self.indexes.model()
 
-        # Convert documents into sentence embeddings
+        # Convert documents into embeddings
         embeddings = model.batchtransform(Stream(self)(documents), category)
 
         # Reduce the dimensionality of the embeddings. Scale the embeddings using this
         # model to reduce the noise of common but less relevant terms.
         if self.reducer:
             self.reducer(embeddings)
 
@@ -609,15 +602,15 @@
         if self.config:
             # Check if this is an archive file
             path, apath = self.checkarchive(path)
 
             # Create output directory, if necessary
             os.makedirs(path, exist_ok=True)
 
-            # Copy sentence vectors model
+            # Copy vectors model
             if self.config.get("storevectors"):
                 shutil.copyfile(self.config["path"], os.path.join(path, os.path.basename(self.config["path"])))
 
                 self.config["path"] = os.path.basename(self.config["path"])
 
             # Save index configuration
             self.saveconfig(path)
@@ -660,29 +653,39 @@
                 cloud.save(apath if apath else path)
 
     def close(self):
         """
         Closes this embeddings index and frees all resources.
         """
 
-        self.ann, self.config, self.graph, self.archive = None, None, None, None
+        self.config, self.archive = None, None
         self.reducer, self.query, self.model, self.models = None, None, None, None
         self.ids = None
 
-        # Close database connection if open
+        # Close ANN
+        if self.ann:
+            self.ann.close()
+            self.ann = None
+
+        # Close database
         if self.database:
             self.database.close()
             self.database, self.functions = None, None
 
-        # Close scoring instance if open
+        # Close scoring
         if self.scoring:
             self.scoring.close()
             self.scoring = None
 
-        # Close indexes if open
+        # Close graph
+        if self.graph:
+            self.graph.close()
+            self.graph = None
+
+        # Close indexes
         if self.indexes:
             self.indexes.close()
             self.indexes = None
 
     def info(self):
         """
         Prints the current embeddings index configuration.
```

### Comparing `txtai-7.1.0/src/python/txtai/embeddings/index/autoid.py` & `txtai-7.2.0/src/python/txtai/embeddings/index/autoid.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/embeddings/index/documents.py` & `txtai-7.2.0/src/python/txtai/embeddings/index/documents.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/embeddings/index/functions.py` & `txtai-7.2.0/src/python/txtai/embeddings/index/functions.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/embeddings/index/indexes.py` & `txtai-7.2.0/src/python/txtai/embeddings/index/indexes.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/embeddings/index/indexids.py` & `txtai-7.2.0/src/python/txtai/embeddings/index/indexids.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/embeddings/index/reducer.py` & `txtai-7.2.0/src/python/txtai/embeddings/index/reducer.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
         Args:
             embeddings: input embeddings matrix
             components: number of model components
         """
 
         if not REDUCER:
-            raise ImportError('Dimensionality reduction is not available - install "similarity" extra to enable')
+            raise ImportError('Dimensionality reduction is not available - install "vectors" extra to enable')
 
         self.model = self.build(embeddings, components) if embeddings is not None and components else None
 
     def __call__(self, embeddings):
         """
         Applies a dimensionality reduction model to embeddings, removed the top n principal components. Operation applied
         directly on array.
```

### Comparing `txtai-7.1.0/src/python/txtai/embeddings/index/stream.py` & `txtai-7.2.0/src/python/txtai/embeddings/index/stream.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/embeddings/index/transform.py` & `txtai-7.2.0/src/python/txtai/embeddings/index/transform.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/embeddings/search/base.py` & `txtai-7.2.0/src/python/txtai/embeddings/search/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/embeddings/search/explain.py` & `txtai-7.2.0/src/python/txtai/embeddings/search/explain.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/embeddings/search/ids.py` & `txtai-7.2.0/src/python/txtai/embeddings/search/ids.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/embeddings/search/query.py` & `txtai-7.2.0/src/python/txtai/embeddings/search/query.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/embeddings/search/scan.py` & `txtai-7.2.0/src/python/txtai/embeddings/search/scan.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/embeddings/search/terms.py` & `txtai-7.2.0/src/python/txtai/embeddings/search/terms.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/graph/base.py` & `txtai-7.2.0/src/python/txtai/graph/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,14 +413,21 @@
                 with open(f"{directory}/topics", "wb") as handle:
                     pickle.dump(self.topics, handle, protocol=__pickle__)
 
             # Pack files
             archive = ArchiveFactory.create(directory)
             archive.save(path, "tar")
 
+    def close(self):
+        """
+        Closes this graph.
+        """
+
+        self.backend, self.categories, self.topics = None, None, None
+
     def insert(self, documents, index=0):
         """
         Insert graph nodes for each document.
 
         Args:
             documents: list of (id, data, tags)
             index: indexid offset, used for node ids
@@ -633,15 +640,16 @@
                         # Add weight, if not provided
                         relation["weight"] = relation.get("weight", 1.0)
 
                         # Add edge and all other attributes
                         edges.append((node, target, relation))
 
         # Add relationships
-        self.addedges(edges)
+        if edges:
+            self.addedges(edges)
 
         # Clear temporary relationship storage
         self.relations = {}
 
     def inferedges(self, nodes, search, attributes=None):
         """
         Infers edges for a list of nodes using a score-based search function.
```

### Comparing `txtai-7.1.0/src/python/txtai/graph/factory.py` & `txtai-7.2.0/src/python/txtai/graph/factory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Factory module
 """
 
 from ..util import Resolver
 
 from .networkx import NetworkX
+from .rdbms import RDBMS
 
 
 class GraphFactory:
     """
     Methods to create graphs.
     """
 
@@ -27,14 +28,16 @@
         # Graph instance
         graph = None
         backend = config.get("backend", "networkx")
 
         # Create graph instance
         if backend == "networkx":
             graph = NetworkX(config)
+        elif backend == "rdbms":
+            graph = RDBMS(config)
         else:
             graph = GraphFactory.resolve(backend, config)
 
         # Store config back
         config["backend"] = backend
 
         return graph
```

### Comparing `txtai-7.1.0/src/python/txtai/graph/networkx.py` & `txtai-7.2.0/src/python/txtai/graph/networkx.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
     def edgecount(self):
         return self.backend.number_of_edges()
 
     def edges(self, node):
         edges = self.backend.adj.get(node)
         if edges:
-            return dict(sorted(edges.items(), key=lambda x: x[1]["weight"], reverse=True))
+            return dict(sorted(edges.items(), key=lambda x: x[1].get("weight", 0), reverse=True))
 
         return None
 
     def addedge(self, source, target, **attrs):
         self.backend.add_edge(source, target, **attrs)
 
     def addedges(self, edges):
```

### Comparing `txtai-7.1.0/src/python/txtai/graph/topics.py` & `txtai-7.2.0/src/python/txtai/graph/topics.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/models/models.py` & `txtai-7.2.0/src/python/txtai/models/models.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/models/onnx.py` & `txtai-7.2.0/src/python/txtai/models/onnx.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,14 +44,25 @@
 
         # Create ONNX session
         self.model = ort.InferenceSession(model, ort.SessionOptions(), self.providers())
 
         # Add references for this class to supported AutoModel classes
         Registry.register(self)
 
+    @property
+    def device(self):
+        """
+        Returns model device id.
+
+        Returns:
+            model device id
+        """
+
+        return -1
+
     def providers(self):
         """
         Returns a list of available and usable providers.
 
         Returns:
             list of available and usable providers
         """
```

### Comparing `txtai-7.1.0/src/python/txtai/models/pooling/base.py` & `txtai-7.2.0/src/python/txtai/models/pooling/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/models/pooling/cls.py` & `txtai-7.2.0/src/python/txtai/models/pooling/cls.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/models/pooling/factory.py` & `txtai-7.2.0/src/python/txtai/models/pooling/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/models/pooling/mean.py` & `txtai-7.2.0/src/python/txtai/models/pooling/mean.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/models/registry.py` & `txtai-7.2.0/src/python/txtai/models/registry.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/models/tokendetection.py` & `txtai-7.2.0/src/python/txtai/models/tokendetection.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/audio/texttospeech.py` & `txtai-7.2.0/src/python/txtai/pipeline/audio/texttospeech.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/audio/transcription.py` & `txtai-7.2.0/src/python/txtai/pipeline/audio/transcription.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/base.py` & `txtai-7.2.0/src/python/txtai/pipeline/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/data/segmentation.py` & `txtai-7.2.0/src/python/txtai/pipeline/data/segmentation.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/data/tabular.py` & `txtai-7.2.0/src/python/txtai/pipeline/data/tabular.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/data/textractor.py` & `txtai-7.2.0/src/python/txtai/pipeline/data/textractor.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/data/tokenizer.py` & `txtai-7.2.0/src/python/txtai/pipeline/data/tokenizer.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/factory.py` & `txtai-7.2.0/src/python/txtai/pipeline/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/hfmodel.py` & `txtai-7.2.0/src/python/txtai/pipeline/hfmodel.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/hfpipeline.py` & `txtai-7.2.0/src/python/txtai/pipeline/hfpipeline.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/image/caption.py` & `txtai-7.2.0/src/python/txtai/pipeline/image/caption.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/image/imagehash.py` & `txtai-7.2.0/src/python/txtai/pipeline/image/imagehash.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/image/objects.py` & `txtai-7.2.0/src/python/txtai/pipeline/image/objects.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/llm/factory.py` & `txtai-7.2.0/src/python/txtai/pipeline/llm/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/llm/generation.py` & `txtai-7.2.0/src/python/txtai/pipeline/llm/generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,40 +22,44 @@
 
         self.path = path
         self.template = template
         self.kwargs = kwargs
 
     def __call__(self, text, maxlength, **kwargs):
         """
-        Generates text using input text
+        Generates text. Supports the following input formats:
+
+          - String or list of strings
+          - List of dictionaries with `role` and `content` key-values or lists of lists
 
         Args:
             text: text|list
             maxlength: maximum sequence length
             kwargs: additional generation keyword arguments
 
         Returns:
             generated text
         """
 
-        # List of texts
-        texts = text if isinstance(text, list) else [text]
+        # Format inputs
+        texts = [text] if isinstance(text, str) or isinstance(text[0], dict) else text
 
         # Apply template, if necessary
         if self.template:
             formatter = TemplateFormatter()
             texts = [formatter.format(self.template, text=x) for x in texts]
 
         # Run pipeline
         results = self.execute(texts, maxlength, **kwargs)
 
         # Clean generated text
         results = [self.clean(texts[x], result) for x, result in enumerate(results)]
 
-        return results[0] if isinstance(text, str) else results
+        # Extract results based on inputs
+        return results[0] if isinstance(text, str) or isinstance(text[0], dict) else results
 
     def execute(self, texts, maxlength, **kwargs):
         """
         Runs a list of prompts through a generative model.
 
         Args:
             texts: list of prompts to run
@@ -74,11 +78,11 @@
             result: result text
 
         Returns:
             clean text
         """
 
         # Replace input prompt
-        text = result.replace(prompt, "")
+        text = result.replace(prompt, "") if isinstance(prompt, str) else result
 
         # Apply text cleaning rules
         return text.replace("$=", "<=").strip()
```

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/llm/huggingface.py` & `txtai-7.2.0/src/python/txtai/pipeline/llm/huggingface.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,18 @@
         super().__init__(self.task(path, task, **kwargs), path, quantize, gpu, model, **kwargs)
 
         # Load tokenizer, if necessary
         self.pipeline.tokenizer = self.pipeline.tokenizer if self.pipeline.tokenizer else Models.tokenizer(path, **kwargs)
 
     def __call__(self, text, prefix=None, maxlength=512, workers=0, **kwargs):
         """
-        Generates text using input text
+        Generates text. Supports the following input formats:
+
+          - String or list of strings
+          - List of dictionaries with `role` and `content` key-values or lists of lists
 
         Args:
             text: text|list
             prefix: optional prefix to prepend to text elements
             maxlength: maximum sequence length
             workers: number of concurrent workers to use for processing data, defaults to None
             kwargs: additional generation keyword arguments
@@ -76,15 +79,16 @@
 
         Returns:
             generated text
         """
 
         # Extract output from list, if necessary
         result = result[0] if isinstance(result, list) else result
-        return result["generated_text"]
+        text = result["generated_text"]
+        return text[-1]["content"] if isinstance(text, list) else text
 
     def task(self, path, task, **kwargs):
         """
         Get the pipeline task name.
 
         Args:
             path: model path input
```

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/llm/litellm.py` & `txtai-7.2.0/src/python/txtai/pipeline/llm/litellm.py`

 * *Files 17% similar despite different names*

```diff
@@ -47,27 +47,19 @@
 
     def __init__(self, path, template=None, **kwargs):
         super().__init__(path, template, **kwargs)
 
         if not LITELLM:
             raise ImportError('LiteLLM is not available - install "pipeline" extra to enable')
 
-        # Register prompt template
-        self.register(path)
-
     def execute(self, texts, maxlength, **kwargs):
         results = []
         for text in texts:
-            result = api.completion(model=self.path, messages=[{"content": text, "role": "user"}], max_tokens=maxlength, **{**kwargs, **self.kwargs})
+            result = api.completion(
+                model=self.path,
+                messages=[{"content": text, "role": "prompt"}] if isinstance(text, str) else text,
+                max_tokens=maxlength,
+                **{**kwargs, **self.kwargs}
+            )
             results.append(result["choices"][0]["message"]["content"])
 
         return results
-
-    def register(self, path):
-        """
-        Registers a custom prompt template for path.
-
-        Args:
-            path: model path
-        """
-
-        api.register_prompt_template(model=path, roles={"user": {"pre_message": "", "post_message": ""}})
```

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/llm/llama.py` & `txtai-7.2.0/src/python/txtai/vectors/llama.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """
 Llama module
 """
 
 import os
 
+import numpy as np
+
 from huggingface_hub import hf_hub_download
 
 # Conditional import
 try:
     from llama_cpp import Llama
 
     LLAMA_CPP = True
 except ImportError:
     LLAMA_CPP = False
 
-from .generation import Generation
+from .base import Vectors
 
 
-class LlamaCpp(Generation):
+class LlamaCpp(Vectors):
     """
-    llama.cpp generative model.
+    Builds vectors using llama.cpp.
     """
 
     @staticmethod
     def ismodel(path):
         """
         Checks if path is a llama.cpp model.
 
@@ -32,33 +34,37 @@
 
         Returns:
             True if this is a llama.cpp model, False otherwise
         """
 
         return isinstance(path, str) and path.lower().endswith(".gguf")
 
-    def __init__(self, path, template=None, **kwargs):
-        super().__init__(path, template, **kwargs)
-
+    def __init__(self, config, scoring, models):
+        # Check before parent constructor since it calls loadmodel
         if not LLAMA_CPP:
-            raise ImportError('llama.cpp is not available - install "pipeline" extra to enable')
+            raise ImportError('llama.cpp is not available - install "vectors" extra to enable')
+
+        super().__init__(config, scoring, models)
 
+    def loadmodel(self, path):
         # Check if this is a local path, otherwise download from the HF Hub
         path = path if os.path.exists(path) else self.download(path)
 
-        # Create llama.cpp instance
-        self.llm = Llama(path, verbose=kwargs.pop("verbose", False), **kwargs)
+        # Additional model arguments
+        modelargs = self.config.get("vectors", {})
+
+        # Default GPU layers if not already set
+        modelargs["n_gpu_layers"] = modelargs.get("n_gpu_layers", -1 if self.config.get("gpu", os.environ.get("LLAMA_NO_METAL") != "1") else 0)
 
-    def execute(self, texts, maxlength, **kwargs):
-        results = []
-        for text in texts:
-            result = self.llm(text, max_tokens=maxlength, **kwargs)
-            results.append(result["choices"][0]["text"])
+        # Create llama.cpp instance
+        return Llama(path, verbose=modelargs.pop("verbose", False), embedding=True, **modelargs)
 
-        return results
+    def encode(self, data):
+        # Generate embeddings and return as a NumPy array
+        return np.array(self.model.embed(data), dtype=np.float32)
 
     def download(self, path):
         """
         Downloads path from the Hugging Face Hub.
 
         Args:
             path: full model path
```

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/llm/llm.py` & `txtai-7.2.0/src/python/txtai/pipeline/llm/llm.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,15 +31,18 @@
         path = path if path else "google/flan-t5-base"
 
         # Generation instance
         self.generator = GenerationFactory.create(path, method, **kwargs)
 
     def __call__(self, text, maxlength=512, **kwargs):
         """
-        Generates text using input text
+        Generates text. Supports the following input formats:
+
+          - String or list of strings
+          - List of dictionaries with `role` and `content` key-values or lists of lists
 
         Args:
             text: text|list
             maxlength: maximum sequence length
             kwargs: additional generation keyword arguments
 
         Returns:
```

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/tensors.py` & `txtai-7.2.0/src/python/txtai/pipeline/tensors.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/text/crossencoder.py` & `txtai-7.2.0/src/python/txtai/pipeline/text/crossencoder.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/text/entity.py` & `txtai-7.2.0/src/python/txtai/pipeline/text/entity.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/text/extractor.py` & `txtai-7.2.0/src/python/txtai/pipeline/text/extractor.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/text/labels.py` & `txtai-7.2.0/src/python/txtai/pipeline/text/labels.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/text/questions.py` & `txtai-7.2.0/src/python/txtai/pipeline/text/questions.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/text/similarity.py` & `txtai-7.2.0/src/python/txtai/pipeline/text/similarity.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/text/summary.py` & `txtai-7.2.0/src/python/txtai/pipeline/text/summary.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/text/translation.py` & `txtai-7.2.0/src/python/txtai/pipeline/text/translation.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/train/hfonnx.py` & `txtai-7.2.0/src/python/txtai/pipeline/train/hfonnx.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 
 
 class HFOnnx(Tensors):
     """
     Exports a Hugging Face Transformer model to ONNX.
     """
 
-    def __call__(self, path, task="default", output=None, quantize=False, opset=12):
+    def __call__(self, path, task="default", output=None, quantize=False, opset=14):
         """
         Exports a Hugging Face Transformer model to ONNX.
 
         Args:
             path: path to model, accepts Hugging Face model hub id, local path or (model, tokenizer) tuple
             task: optional model task or category, determines the model type and outputs, defaults to export hidden state
             output: optional output model path, defaults to return byte array if None
             quantize: if model should be quantized (requires onnx to be installed), defaults to False
-            opset: onnx opset, defaults to 12
+            opset: onnx opset, defaults to 14
 
         Returns:
             path to model output or model as bytes depending on output parameter
         """
 
         inputs, outputs, model = self.parameters(task)
```

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/train/hftrainer.py` & `txtai-7.2.0/src/python/txtai/pipeline/train/hftrainer.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/pipeline/train/mlonnx.py` & `txtai-7.2.0/src/python/txtai/pipeline/train/mlonnx.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,13 +50,14 @@
 
         # pylint: disable=E1101
         # Rename output to logits for consistency with other models
         model.graph.output[0].name = "logits"
 
         # Find probabilities output node and rename to logits
         for node in model.graph.node:
-            if node.output[0] == "probabilities":
-                node.output[0] = "logits"
+            for x, _ in enumerate(node.output):
+                if node.output[x] == "probabilities":
+                    node.output[x] = "logits"
 
         # Save model to specified output path or return bytes
         model = save_onnx_model(model, output)
         return output if output else model
```

### Comparing `txtai-7.1.0/src/python/txtai/scoring/base.py` & `txtai-7.2.0/src/python/txtai/scoring/tfidf.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 """
-Scoring module
+TFIDF module
 """
 
 import math
 import os
 import pickle
 
 from collections import Counter
 from multiprocessing.pool import ThreadPool
 
 import numpy as np
 
 from ..pipeline import Tokenizer
 from ..version import __pickle__
 
+from .base import Scoring
 from .terms import Terms
 
 
-class Scoring:
+class TFIDF(Scoring):
     """
-    Base scoring. Uses term frequency-inverse document frequency (TF-IDF).
+    Term frequency-inverse document frequency (TF-IDF) scoring.
     """
 
     def __init__(self, config=None):
-        """
-        Initializes backing statistic objects.
-
-        Args:
-            config: input configuration
-        """
-
-        # Scoring configuration
-        self.config = config if config else {}
+        super().__init__(config)
 
         # Document stats
         self.total = 0
         self.tokens = 0
         self.avgdl = 0
 
         # Word frequency
@@ -49,38 +42,25 @@
 
         # Tag boosting
         self.tags = Counter()
 
         # Tokenizer, lazily loaded as needed
         self.tokenizer = None
 
-        # Transform columns
-        columns = config.get("columns", {})
-        self.text = columns.get("text", "text")
-        self.object = columns.get("object", "object")
-
         # Term index
         self.terms = Terms(self.config["terms"], self.score, self.idf) if self.config.get("terms") else None
 
         # Document data
         self.documents = {} if self.config.get("content") else None
 
         # Normalize scores
         self.normalize = self.config.get("normalize")
         self.avgscore = None
 
     def insert(self, documents, index=None):
-        """
-        Inserts documents into the scoring index.
-
-        Args:
-            documents: list of (id, dict|text|tokens, tags)
-            index: indexid offset
-        """
-
         # Insert documents, calculate word frequency, total tokens and total documents
         for uid, document, tags in documents:
             # Extract text, if necessary
             if isinstance(document, dict):
                 document = document.get(self.text, document.get(self.object))
 
             if document is not None:
@@ -103,41 +83,26 @@
                     # Add tokens and tags to stats
                     self.addstats(tokens, tags)
 
                 # Increment index
                 index = index + 1 if index is not None else None
 
     def delete(self, ids):
-        """
-        Deletes documents from scoring index.
-
-        Args:
-            ids: list of ids to delete
-        """
-
         # Delete from terms index
         if self.terms:
             self.terms.delete(ids)
 
         # Delete content
         if self.documents:
             for uid in ids:
                 self.documents.pop(uid)
 
     def index(self, documents=None):
-        """
-        Indexes a collection of documents using a scoring method.
-
-        Args:
-            documents: list of (id, dict|text|tokens, tags)
-        """
-
-        # Insert documents
-        if documents:
-            self.insert(documents)
+        # Call base method
+        super().index(documents)
 
         # Build index if tokens parsed
         if self.wordfreq:
             # Calculate total token frequency
             self.tokens = sum(self.wordfreq.values())
 
             # Calculate average frequency per token
@@ -160,35 +125,15 @@
             # Filter for tags that appear in at least 1% of the documents
             self.tags = Counter({tag: number for tag, number in self.tags.items() if number >= self.total * 0.005})
 
         # Index terms, if available
         if self.terms:
             self.terms.index()
 
-    def upsert(self, documents=None):
-        """
-        Convience method for API clarity. Calls index method.
-
-        Args:
-            documents: list of (id, dict|text|tokens, tags)
-        """
-
-        self.index(documents)
-
     def weights(self, tokens):
-        """
-        Builds a weights vector for each token in input tokens.
-
-        Args:
-            tokens: input tokens
-
-        Returns:
-            list of weights for each token
-        """
-
         # Document length
         length = len(tokens)
 
         # Calculate token counts
         freq = self.computefreq(tokens)
         freq = np.array([freq[token] for token in tokens])
 
@@ -206,25 +151,14 @@
                 maxTag = max(tags.values())
 
                 weights = [max(maxWeight * (tags[tokens[x]] / maxTag), weight) if tokens[x] in tags else weight for x, weight in enumerate(weights)]
 
         return weights
 
     def search(self, query, limit=3):
-        """
-        Search index for documents matching query.
-
-        Args:
-            query: input query
-            limit: maximum results
-
-        Returns:
-            list of (id, score) or (data, score) if content is enabled
-        """
-
         # Check if term index available
         if self.terms:
             # Parse query into terms
             query = self.tokenize(query) if isinstance(query, str) else query
 
             # Get topn term query matches
             scores = self.terms.search(query, limit)
@@ -240,104 +174,60 @@
 
             # Add content, if available
             return self.results(scores)
 
         return None
 
     def batchsearch(self, queries, limit=3, threads=True):
-        """
-        Search index for documents matching queries. This method is able to run as multiple threads due to
-        a number of regex and numpy method calls that drop the GIL.
-        """
-
         # Calculate number of threads using a thread per 25k records in index
         threads = math.ceil(self.count() / 25000) if isinstance(threads, bool) and threads else int(threads)
         threads = min(max(threads, 1), os.cpu_count())
 
-        # Run threaded queries
+        # This method is able to run as multiple threads due to a number of regex and numpy method calls that drop the GIL.
         results = []
         with ThreadPool(threads) as pool:
             for result in pool.starmap(self.search, [(x, limit) for x in queries]):
                 results.append(result)
 
         return results
 
     def count(self):
-        """
-        Returns the total number of documents indexed.
-
-        Returns:
-            total number of documents indexed
-        """
-
         return self.terms.count() if self.terms else self.total
 
     def load(self, path):
-        """
-        Loads a saved Scoring object from path.
-
-        Args:
-            path: directory path to load scoring index
-        """
-
         with open(path, "rb") as handle:
             # Load scoring
             self.__dict__.update(pickle.load(handle))
 
             # Load terms
             if self.config.get("terms"):
                 self.terms = Terms(self.config["terms"], self.score, self.idf)
                 self.terms.load(path + ".terms")
 
     def save(self, path):
-        """
-        Saves a Scoring object to path.
-
-        Args:
-            path: directory path to save scoring index
-        """
-
         with open(path, "wb") as handle:
             # Don't serialize following fields
             skipfields = ("config", "terms", "tokenizer")
 
             # Save scoring
             state = {key: value for key, value in self.__dict__.items() if key not in skipfields}
             pickle.dump(state, handle, protocol=__pickle__)
 
             # Save terms
             if self.terms:
                 self.terms.save(path + ".terms")
 
     def close(self):
-        """
-        Close and free resources used by this instance.
-        """
-
         if self.terms:
             self.terms.close()
 
     def hasterms(self):
-        """
-        Check if this scoring instance has an associated terms index.
-
-        Returns:
-            True if this scoring instance has an associated terms index.
-        """
-
         return self.terms is not None
 
     def isnormalized(self):
-        """
-        Check if this scoring instance returns normalized scores.
-
-        Returns:
-            True if normalize is enabled, False otherwise
-        """
-
         return self.normalize
 
     def computefreq(self, tokens):
         """
         Computes token frequency. Used for token weighting.
 
         Args:
```

### Comparing `txtai-7.1.0/src/python/txtai/scoring/bm25.py` & `txtai-7.2.0/src/python/txtai/scoring/bm25.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 BM25 module
 """
 
 import numpy as np
 
-from .base import Scoring
+from .tfidf import TFIDF
 
 
-class BM25(Scoring):
+class BM25(TFIDF):
     """
     Best matching (BM25) scoring.
     """
 
     def __init__(self, config=None):
         super().__init__(config)
```

### Comparing `txtai-7.1.0/src/python/txtai/scoring/factory.py` & `txtai-7.2.0/src/python/txtai/scoring/factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 Factory module
 """
 
 from ..util import Resolver
 
-from .base import Scoring
 from .bm25 import BM25
 from .sif import SIF
+from .pgtext import PGText
+from .tfidf import TFIDF
 
 
 class ScoringFactory:
     """
     Methods to create Scoring indexes.
     """
 
@@ -36,17 +37,18 @@
         # Get scoring method
         method = config.get("method", "bm25")
 
         if method == "bm25":
             scoring = BM25(config)
         elif method == "sif":
             scoring = SIF(config)
+        elif method == "pgtext":
+            scoring = PGText(config)
         elif method == "tfidf":
-            # Default scoring class implements tf-idf
-            scoring = Scoring(config)
+            scoring = TFIDF(config)
         else:
             # Resolve custom method
             scoring = ScoringFactory.resolve(method, config)
 
         # Store config back
         config["method"] = method
```

### Comparing `txtai-7.1.0/src/python/txtai/scoring/sif.py` & `txtai-7.2.0/src/python/txtai/scoring/sif.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
 SIF module
 """
 
 import numpy as np
 
-from .base import Scoring
+from .tfidf import TFIDF
 
 
-class SIF(Scoring):
+class SIF(TFIDF):
     """
     Smooth Inverse Frequency (SIF) scoring.
     """
 
     def __init__(self, config=None):
         super().__init__(config)
```

### Comparing `txtai-7.1.0/src/python/txtai/scoring/terms.py` & `txtai-7.2.0/src/python/txtai/scoring/terms.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/util/resolver.py` & `txtai-7.2.0/src/python/txtai/util/resolver.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/vectors/base.py` & `txtai-7.2.0/src/python/txtai/vectors/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import numpy as np
 
 from ..version import __pickle__
 
 
 class Vectors:
     """
-    Base class for sentence embeddings/vector models. Vector models transform input content into numeric vectors.
+    Base class for vector models. Vector models transform input content into numeric vectors.
     """
 
     def __init__(self, config, scoring, models):
         """
         Creates a new vectors instance.
 
         Args:
```

### Comparing `txtai-7.1.0/src/python/txtai/vectors/external.py` & `txtai-7.2.0/src/python/txtai/vectors/external.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 import numpy as np
 
 from ..util import Resolver
 
 from .base import Vectors
 
 
-class ExternalVectors(Vectors):
+class External(Vectors):
     """
-    Loads pre-computed vectors. Pre-computed vectors allow integrating other vector models. They can also be used to efficiently
-    test different model configurations without having to recompute vectors.
+    Builds vectors using an external method. This can be a local function or an external API call.
     """
 
     def __init__(self, config, scoring, models):
         super().__init__(config, scoring, models)
 
         # Lookup and resolve transform function
         self.transform = self.resolve(config.get("transform"))
```

### Comparing `txtai-7.1.0/src/python/txtai/vectors/factory.py` & `txtai-7.2.0/src/python/txtai/vectors/factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 """
 Factory module
 """
 
-from .external import ExternalVectors
-from .transformers import TransformersVectors
+from ..util import Resolver
+
+from .external import External
+from .huggingface import HFVectors
+from .litellm import LiteLLM
+from .llama import LlamaCpp
 from .words import WordVectors, WORDS
 
 
 class VectorsFactory:
     """
     Methods to create Vectors models.
     """
@@ -24,47 +28,89 @@
 
         Returns:
             Vectors
         """
 
         # Determine vector method
         method = VectorsFactory.method(config)
+
+        # External vectors
         if method == "external":
-            return ExternalVectors(config, scoring, models)
+            return External(config, scoring, models)
+
+        # LiteLLM vectors
+        if method == "litellm":
+            return LiteLLM(config, scoring, models)
 
+        # llama.cpp vectors
+        if method == "llama.cpp":
+            return LlamaCpp(config, scoring, models)
+
+        # Word vectors
         if method == "words":
             if not WORDS:
-                # Raise error if trying to create Word Vectors without similarity extra
+                # Raise error if trying to create Word Vectors without vectors extra
                 raise ImportError(
-                    'Word vector models are not available - install "similarity" extra to enable. Otherwise, specify '
+                    'Word vector models are not available - install "vectors" extra to enable. Otherwise, specify '
                     + 'method="transformers" to use transformer backed models'
                 )
 
             return WordVectors(config, scoring, models)
 
-        # Default to TransformersVectors when configuration available
-        return TransformersVectors(config, scoring, models) if config and "path" in config else None
+        # Transformers vectors
+        if HFVectors.ismethod(method):
+            return HFVectors(config, scoring, models) if config and config.get("path") else None
+
+        # Resolve custom method
+        return VectorsFactory.resolve(method, config, scoring, models) if method else None
 
     @staticmethod
     def method(config):
         """
         Get or derive the vector method.
 
         Args:
             config: vector configuration
 
         Returns:
             vector method
         """
 
-        # Determine vector type (external, transformers or words)
+        # Determine vector method (external, litellm, llama.cpp, transformers or words)
         method = config.get("method")
         path = config.get("path")
 
         # Infer method from path, if blank
         if not method:
             if path:
-                method = "words" if WordVectors.isdatabase(path) else "transformers"
+                if LiteLLM.ismodel(path):
+                    method = "litellm"
+                elif LlamaCpp.ismodel(path):
+                    method = "llama.cpp"
+                elif WordVectors.isdatabase(path):
+                    method = "words"
+                else:
+                    method = "transformers"
             elif config.get("transform"):
                 method = "external"
 
         return method
+
+    @staticmethod
+    def resolve(backend, config, scoring, models):
+        """
+        Attempt to resolve a custom backend.
+
+        Args:
+            backend: backend class
+            config: vector configuration
+            scoring: scoring instance
+            models: models cache
+
+        Returns:
+            Vectors
+        """
+
+        try:
+            return Resolver()(backend)(config, scoring, models)
+        except Exception as e:
+            raise ImportError(f"Unable to resolve vectors backend: '{backend}'") from e
```

### Comparing `txtai-7.1.0/src/python/txtai/vectors/transformers.py` & `txtai-7.2.0/src/python/txtai/vectors/huggingface.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Transformers module
+Hugging Face module
 """
 
 # Conditional import
 try:
     from sentence_transformers import SentenceTransformer
 
     SENTENCE_TRANSFORMERS = True
@@ -11,19 +11,33 @@
     SENTENCE_TRANSFORMERS = False
 
 from .base import Vectors
 from ..models import Models, PoolingFactory
 from ..pipeline import Tokenizer
 
 
-class TransformersVectors(Vectors):
+class HFVectors(Vectors):
     """
-    Builds sentence embeddings/vectors using the transformers library.
+    Builds vectors using the Hugging Face transformers library. Also supports the sentence-transformers library.
     """
 
+    @staticmethod
+    def ismethod(method):
+        """
+        Checks if this method uses local transformers-based models.
+
+        Args:
+            method: input method
+
+        Returns:
+            True if this is a local transformers-based model, False otherwise
+        """
+
+        return method in ("transformers", "sentence-transformers", "pooling", "clspooling", "meanpooling")
+
     def loadmodel(self, path):
         # Flag that determines if transformers or sentence-transformers should be used to build embeddings
         method = self.config.get("method")
         transformers = method != "sentence-transformers"
 
         # Tensor device id
         deviceid = Models.deviceid(self.config.get("gpu", True))
@@ -35,15 +49,15 @@
         if transformers:
             return PoolingFactory.create(
                 {"path": path, "device": deviceid, "tokenizer": self.config.get("tokenizer"), "method": method, "modelargs": modelargs}
             )
 
         # Otherwise, use sentence-transformers library
         if not SENTENCE_TRANSFORMERS:
-            raise ImportError('sentence-transformers is not available - install "similarity" extra to enable')
+            raise ImportError('sentence-transformers is not available - install "vectors" extra to enable')
 
         # Build embeddings with sentence-transformers
         return SentenceTransformer(path, device=Models.device(deviceid), **modelargs)
 
     def encode(self, data):
         # Get batch parameter name
         param = "batch_size" if self.config.get("method") == "sentence-transformers" else "batch"
```

### Comparing `txtai-7.1.0/src/python/txtai/vectors/words.py` & `txtai-7.2.0/src/python/txtai/vectors/words.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     """
 
     return (document[0], VECTORS.transform(document))
 
 
 class WordVectors(Vectors):
     """
-    Builds sentence embeddings/vectors using weighted word embeddings.
+    Builds vectors using weighted word embeddings.
     """
 
     def loadmodel(self, path):
         # Ensure that vector path exists
         if not path or not os.path.isfile(path):
             raise IOError(ENOENT, "Vector model file not found", path)
```

### Comparing `txtai-7.1.0/src/python/txtai/workflow/base.py` & `txtai-7.2.0/src/python/txtai/workflow/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/workflow/execute.py` & `txtai-7.2.0/src/python/txtai/workflow/execute.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,16 +84,16 @@
         return None
 
     def close(self):
         """
         Closes concurrent processing pools.
         """
 
-        if self.thread:
+        if hasattr(self, "thread") and self.thread:
             self.thread.close()
             self.thread.join()
             self.thread = None
 
-        if self.process:
+        if hasattr(self, "process") and self.process:
             self.process.close()
             self.process.join()
             self.process = None
```

### Comparing `txtai-7.1.0/src/python/txtai/workflow/factory.py` & `txtai-7.2.0/src/python/txtai/workflow/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/workflow/task/base.py` & `txtai-7.2.0/src/python/txtai/workflow/task/base.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/workflow/task/export.py` & `txtai-7.2.0/src/python/txtai/workflow/task/export.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/workflow/task/factory.py` & `txtai-7.2.0/src/python/txtai/workflow/task/factory.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/workflow/task/file.py` & `txtai-7.2.0/src/python/txtai/workflow/task/file.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/workflow/task/image.py` & `txtai-7.2.0/src/python/txtai/workflow/task/image.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/workflow/task/retrieve.py` & `txtai-7.2.0/src/python/txtai/workflow/task/retrieve.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/workflow/task/service.py` & `txtai-7.2.0/src/python/txtai/workflow/task/service.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/workflow/task/storage.py` & `txtai-7.2.0/src/python/txtai/workflow/task/storage.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/workflow/task/stream.py` & `txtai-7.2.0/src/python/txtai/workflow/task/stream.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai/workflow/task/template.py` & `txtai-7.2.0/src/python/txtai/workflow/task/template.py`

 * *Files identical despite different names*

### Comparing `txtai-7.1.0/src/python/txtai.egg-info/PKG-INFO` & `txtai-7.2.0/src/python/txtai.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txtai
-Version: 7.1.0
+Version: 7.2.0
 Summary: All-in-one open-source embeddings database for semantic search, LLM orchestration and language model workflows
 Home-page: https://github.com/neuml/txtai
 Author: NeuML
 License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/neuml/txtai
 Project-URL: Issue Tracker, https://github.com/neuml/txtai/issues
 Project-URL: Source Code, https://github.com/neuml/txtai
@@ -32,14 +32,19 @@
 Requires-Dist: coveralls; extra == "dev"
 Requires-Dist: httpx; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs-redirects; extra == "dev"
 Requires-Dist: mkdocstrings[python]; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pylint; extra == "dev"
+Provides-Extra: ann
+Requires-Dist: annoy>=1.16.3; extra == "ann"
+Requires-Dist: hnswlib>=0.5.0; extra == "ann"
+Requires-Dist: pgvector>=0.2.5; extra == "ann"
+Requires-Dist: sqlalchemy>=2.0.20; extra == "ann"
 Provides-Extra: api
 Requires-Dist: aiohttp>=3.8.1; extra == "api"
 Requires-Dist: fastapi>=0.94.0; extra == "api"
 Requires-Dist: msgpack>=1.0.7; extra == "api"
 Requires-Dist: pillow>=7.1.2; extra == "api"
 Requires-Dist: python-multipart>=0.0.7; extra == "api"
 Requires-Dist: uvicorn>=0.12.1; extra == "api"
@@ -49,16 +54,18 @@
 Requires-Dist: rich>=12.0.1; extra == "console"
 Provides-Extra: database
 Requires-Dist: duckdb>=0.7.1; extra == "database"
 Requires-Dist: pillow>=7.1.2; extra == "database"
 Requires-Dist: sqlalchemy>=2.0.20; extra == "database"
 Provides-Extra: graph
 Requires-Dist: grand-cypher>=0.6.0; extra == "graph"
+Requires-Dist: grand-graph>=0.5.0; extra == "graph"
 Requires-Dist: networkx>=2.6.3; extra == "graph"
 Requires-Dist: python-louvain>=0.16; extra == "graph"
+Requires-Dist: sqlalchemy>=2.0.20; extra == "graph"
 Provides-Extra: model
 Requires-Dist: onnx>=1.11.0; extra == "model"
 Requires-Dist: onnxruntime>=1.11.0; extra == "model"
 Provides-Extra: pipeline-audio
 Requires-Dist: onnx>=1.11.0; extra == "pipeline-audio"
 Requires-Dist: onnxruntime>=1.11.0; extra == "pipeline-audio"
 Requires-Dist: soundfile>=0.10.3.post1; extra == "pipeline-audio"
@@ -70,16 +77,16 @@
 Requires-Dist: pandas>=1.1.0; extra == "pipeline-data"
 Requires-Dist: tika>=1.24; extra == "pipeline-data"
 Provides-Extra: pipeline-image
 Requires-Dist: imagehash>=4.2.1; extra == "pipeline-image"
 Requires-Dist: pillow>=7.1.2; extra == "pipeline-image"
 Requires-Dist: timm>=0.4.12; extra == "pipeline-image"
 Provides-Extra: pipeline-llm
-Requires-Dist: litellm>=1.31.2; extra == "pipeline-llm"
-Requires-Dist: llama-cpp-python>=0.2.20; extra == "pipeline-llm"
+Requires-Dist: litellm>=1.37.16; extra == "pipeline-llm"
+Requires-Dist: llama-cpp-python>=0.2.75; extra == "pipeline-llm"
 Provides-Extra: pipeline-text
 Requires-Dist: fasttext>=0.9.2; extra == "pipeline-text"
 Requires-Dist: sentencepiece>=0.1.91; extra == "pipeline-text"
 Provides-Extra: pipeline-train
 Requires-Dist: accelerate>=0.26.0; extra == "pipeline-train"
 Requires-Dist: bitsandbytes>=0.42.0; extra == "pipeline-train"
 Requires-Dist: onnx>=1.11.0; extra == "pipeline-train"
@@ -96,83 +103,103 @@
 Requires-Dist: beautifulsoup4>=4.9.3; extra == "pipeline"
 Requires-Dist: nltk>=3.5; extra == "pipeline"
 Requires-Dist: pandas>=1.1.0; extra == "pipeline"
 Requires-Dist: tika>=1.24; extra == "pipeline"
 Requires-Dist: imagehash>=4.2.1; extra == "pipeline"
 Requires-Dist: pillow>=7.1.2; extra == "pipeline"
 Requires-Dist: timm>=0.4.12; extra == "pipeline"
-Requires-Dist: litellm>=1.31.2; extra == "pipeline"
-Requires-Dist: llama-cpp-python>=0.2.20; extra == "pipeline"
+Requires-Dist: litellm>=1.37.16; extra == "pipeline"
+Requires-Dist: llama-cpp-python>=0.2.75; extra == "pipeline"
 Requires-Dist: fasttext>=0.9.2; extra == "pipeline"
 Requires-Dist: sentencepiece>=0.1.91; extra == "pipeline"
 Requires-Dist: accelerate>=0.26.0; extra == "pipeline"
 Requires-Dist: bitsandbytes>=0.42.0; extra == "pipeline"
 Requires-Dist: onnx>=1.11.0; extra == "pipeline"
 Requires-Dist: onnxmltools>=1.9.1; extra == "pipeline"
 Requires-Dist: onnxruntime>=1.11.0; extra == "pipeline"
 Requires-Dist: peft>=0.8.1; extra == "pipeline"
 Requires-Dist: skl2onnx>=1.9.1; extra == "pipeline"
-Provides-Extra: similarity
-Requires-Dist: annoy>=1.16.3; extra == "similarity"
-Requires-Dist: fasttext>=0.9.2; extra == "similarity"
-Requires-Dist: hnswlib>=0.5.0; extra == "similarity"
-Requires-Dist: pymagnitude-lite>=0.1.43; extra == "similarity"
-Requires-Dist: scikit-learn>=0.23.1; extra == "similarity"
-Requires-Dist: sentence-transformers>=2.2.0; extra == "similarity"
+Provides-Extra: scoring
+Requires-Dist: sqlalchemy>=2.0.20; extra == "scoring"
+Provides-Extra: vectors
+Requires-Dist: fasttext>=0.9.2; extra == "vectors"
+Requires-Dist: litellm>=1.37.16; extra == "vectors"
+Requires-Dist: llama-cpp-python>=0.2.75; extra == "vectors"
+Requires-Dist: pymagnitude-lite>=0.1.43; extra == "vectors"
+Requires-Dist: scikit-learn>=0.23.1; extra == "vectors"
+Requires-Dist: sentence-transformers>=2.2.0; extra == "vectors"
 Provides-Extra: workflow
 Requires-Dist: apache-libcloud>=3.3.1; extra == "workflow"
 Requires-Dist: croniter>=1.2.0; extra == "workflow"
 Requires-Dist: openpyxl>=3.0.9; extra == "workflow"
 Requires-Dist: pandas>=1.1.0; extra == "workflow"
 Requires-Dist: pillow>=7.1.2; extra == "workflow"
 Requires-Dist: requests>=2.26.0; extra == "workflow"
 Requires-Dist: xmltodict>=0.12.0; extra == "workflow"
+Provides-Extra: similarity
+Requires-Dist: annoy>=1.16.3; extra == "similarity"
+Requires-Dist: hnswlib>=0.5.0; extra == "similarity"
+Requires-Dist: pgvector>=0.2.5; extra == "similarity"
+Requires-Dist: sqlalchemy>=2.0.20; extra == "similarity"
+Requires-Dist: fasttext>=0.9.2; extra == "similarity"
+Requires-Dist: litellm>=1.37.16; extra == "similarity"
+Requires-Dist: llama-cpp-python>=0.2.75; extra == "similarity"
+Requires-Dist: pymagnitude-lite>=0.1.43; extra == "similarity"
+Requires-Dist: scikit-learn>=0.23.1; extra == "similarity"
+Requires-Dist: sentence-transformers>=2.2.0; extra == "similarity"
 Provides-Extra: all
 Requires-Dist: aiohttp>=3.8.1; extra == "all"
 Requires-Dist: fastapi>=0.94.0; extra == "all"
 Requires-Dist: msgpack>=1.0.7; extra == "all"
 Requires-Dist: pillow>=7.1.2; extra == "all"
 Requires-Dist: python-multipart>=0.0.7; extra == "all"
 Requires-Dist: uvicorn>=0.12.1; extra == "all"
 Requires-Dist: apache-libcloud>=3.3.1; extra == "all"
 Requires-Dist: rich>=12.0.1; extra == "all"
 Requires-Dist: duckdb>=0.7.1; extra == "all"
 Requires-Dist: pillow>=7.1.2; extra == "all"
 Requires-Dist: sqlalchemy>=2.0.20; extra == "all"
 Requires-Dist: grand-cypher>=0.6.0; extra == "all"
+Requires-Dist: grand-graph>=0.5.0; extra == "all"
 Requires-Dist: networkx>=2.6.3; extra == "all"
 Requires-Dist: python-louvain>=0.16; extra == "all"
+Requires-Dist: sqlalchemy>=2.0.20; extra == "all"
 Requires-Dist: onnx>=1.11.0; extra == "all"
 Requires-Dist: onnxruntime>=1.11.0; extra == "all"
 Requires-Dist: onnx>=1.11.0; extra == "all"
 Requires-Dist: onnxruntime>=1.11.0; extra == "all"
 Requires-Dist: soundfile>=0.10.3.post1; extra == "all"
 Requires-Dist: scipy>=1.4.1; extra == "all"
 Requires-Dist: ttstokenizer>=1.0.0; extra == "all"
 Requires-Dist: beautifulsoup4>=4.9.3; extra == "all"
 Requires-Dist: nltk>=3.5; extra == "all"
 Requires-Dist: pandas>=1.1.0; extra == "all"
 Requires-Dist: tika>=1.24; extra == "all"
 Requires-Dist: imagehash>=4.2.1; extra == "all"
 Requires-Dist: pillow>=7.1.2; extra == "all"
 Requires-Dist: timm>=0.4.12; extra == "all"
-Requires-Dist: litellm>=1.31.2; extra == "all"
-Requires-Dist: llama-cpp-python>=0.2.20; extra == "all"
+Requires-Dist: litellm>=1.37.16; extra == "all"
+Requires-Dist: llama-cpp-python>=0.2.75; extra == "all"
 Requires-Dist: fasttext>=0.9.2; extra == "all"
 Requires-Dist: sentencepiece>=0.1.91; extra == "all"
 Requires-Dist: accelerate>=0.26.0; extra == "all"
 Requires-Dist: bitsandbytes>=0.42.0; extra == "all"
 Requires-Dist: onnx>=1.11.0; extra == "all"
 Requires-Dist: onnxmltools>=1.9.1; extra == "all"
 Requires-Dist: onnxruntime>=1.11.0; extra == "all"
 Requires-Dist: peft>=0.8.1; extra == "all"
 Requires-Dist: skl2onnx>=1.9.1; extra == "all"
+Requires-Dist: sqlalchemy>=2.0.20; extra == "all"
 Requires-Dist: annoy>=1.16.3; extra == "all"
-Requires-Dist: fasttext>=0.9.2; extra == "all"
 Requires-Dist: hnswlib>=0.5.0; extra == "all"
+Requires-Dist: pgvector>=0.2.5; extra == "all"
+Requires-Dist: sqlalchemy>=2.0.20; extra == "all"
+Requires-Dist: fasttext>=0.9.2; extra == "all"
+Requires-Dist: litellm>=1.37.16; extra == "all"
+Requires-Dist: llama-cpp-python>=0.2.75; extra == "all"
 Requires-Dist: pymagnitude-lite>=0.1.43; extra == "all"
 Requires-Dist: scikit-learn>=0.23.1; extra == "all"
 Requires-Dist: sentence-transformers>=2.2.0; extra == "all"
 Requires-Dist: apache-libcloud>=3.3.1; extra == "all"
 Requires-Dist: croniter>=1.2.0; extra == "all"
 Requires-Dist: openpyxl>=3.0.9; extra == "all"
 Requires-Dist: pandas>=1.1.0; extra == "all"
@@ -311,14 +338,15 @@
 A novel feature of txtai is that it can provide both an answer and source citation.
 
 | Notebook  | Description  |       |
 |:----------|:-------------|------:|
 | [Build RAG pipelines with txtai](https://github.com/neuml/txtai/blob/master/examples/52_Build_RAG_pipelines_with_txtai.ipynb) | Guide on retrieval augmented generation including how to create citations | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/52_Build_RAG_pipelines_with_txtai.ipynb) |
 | [Advanced RAG with graph path traversal](https://github.com/neuml/txtai/blob/master/examples/58_Advanced_RAG_with_graph_path_traversal.ipynb) | Graph path traversal to collect complex sets of data for advanced RAG | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/58_Advanced_RAG_with_graph_path_traversal.ipynb) |
 | [Advanced RAG with guided generation](https://github.com/neuml/txtai/blob/master/examples/60_Advanced_RAG_with_guided_generation.ipynb) | Retrieval Augmented and Guided Generation | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/60_Advanced_RAG_with_guided_generation.ipynb) |
+| [RAG with llama.cpp and external API services](https://github.com/neuml/txtai/blob/master/examples/62_RAG_with_llama_cpp_and_external_API_services.ipynb) | RAG with additional vector and LLM frameworks | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neuml/txtai/blob/master/examples/62_RAG_with_llama_cpp_and_external_API_services.ipynb) |
 
 ### Language Model Workflows
 
 Language model workflows, also known as semantic workflows, connect language models together to build intelligent applications.
 
 ![flows](https://raw.githubusercontent.com/neuml/txtai/master/docs/images/flows.png#gh-light-mode-only)
 
@@ -366,14 +394,15 @@
 Models can be loaded as either a path from the Hugging Face Hub or a local directory. Model paths are optional, defaults are loaded when not specified. For tasks with no recommended model, txtai uses the default models as shown in the Hugging Face Tasks guide.
 
 See the following links to learn more.
 
 - [Hugging Face Tasks](https://hf.co/tasks)
 - [Hugging Face Model Hub](https://hf.co/models)
 - [MTEB Leaderboard](https://hf.co/spaces/mteb/leaderboard)
+- [LMSYS LLM Leaderboard](https://chat.lmsys.org/?leaderboard)
 - [Open LLM Leaderboard](https://hf.co/spaces/HuggingFaceH4/open_llm_leaderboard)
 
 ## Powered by txtai
 
 The following applications are powered by txtai.
 
 ![apps](https://raw.githubusercontent.com/neuml/txtai/master/apps.jpg)
```

### Comparing `txtai-7.1.0/src/python/txtai.egg-info/SOURCES.txt` & `txtai-7.2.0/src/python/txtai.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/python/txtai/ann/__init__.py
 src/python/txtai/ann/annoy.py
 src/python/txtai/ann/base.py
 src/python/txtai/ann/factory.py
 src/python/txtai/ann/faiss.py
 src/python/txtai/ann/hnsw.py
 src/python/txtai/ann/numpy.py
+src/python/txtai/ann/pgvector.py
 src/python/txtai/ann/torch.py
 src/python/txtai/api/__init__.py
 src/python/txtai/api/application.py
 src/python/txtai/api/authorization.py
 src/python/txtai/api/base.py
 src/python/txtai/api/cluster.py
 src/python/txtai/api/extension.py
@@ -108,14 +109,15 @@
 src/python/txtai/embeddings/search/query.py
 src/python/txtai/embeddings/search/scan.py
 src/python/txtai/embeddings/search/terms.py
 src/python/txtai/graph/__init__.py
 src/python/txtai/graph/base.py
 src/python/txtai/graph/factory.py
 src/python/txtai/graph/networkx.py
+src/python/txtai/graph/rdbms.py
 src/python/txtai/graph/topics.py
 src/python/txtai/models/__init__.py
 src/python/txtai/models/models.py
 src/python/txtai/models/onnx.py
 src/python/txtai/models/registry.py
 src/python/txtai/models/tokendetection.py
 src/python/txtai/models/pooling/__init__.py
@@ -162,24 +164,28 @@
 src/python/txtai/pipeline/train/hfonnx.py
 src/python/txtai/pipeline/train/hftrainer.py
 src/python/txtai/pipeline/train/mlonnx.py
 src/python/txtai/scoring/__init__.py
 src/python/txtai/scoring/base.py
 src/python/txtai/scoring/bm25.py
 src/python/txtai/scoring/factory.py
+src/python/txtai/scoring/pgtext.py
 src/python/txtai/scoring/sif.py
 src/python/txtai/scoring/terms.py
+src/python/txtai/scoring/tfidf.py
 src/python/txtai/util/__init__.py
 src/python/txtai/util/resolver.py
 src/python/txtai/util/template.py
 src/python/txtai/vectors/__init__.py
 src/python/txtai/vectors/base.py
 src/python/txtai/vectors/external.py
 src/python/txtai/vectors/factory.py
-src/python/txtai/vectors/transformers.py
+src/python/txtai/vectors/huggingface.py
+src/python/txtai/vectors/litellm.py
+src/python/txtai/vectors/llama.py
 src/python/txtai/vectors/words.py
 src/python/txtai/workflow/__init__.py
 src/python/txtai/workflow/base.py
 src/python/txtai/workflow/execute.py
 src/python/txtai/workflow/factory.py
 src/python/txtai/workflow/task/__init__.py
 src/python/txtai/workflow/task/base.py
```

### Comparing `txtai-7.1.0/src/python/txtai.egg-info/requires.txt` & `txtai-7.2.0/src/python/txtai.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -14,46 +14,54 @@
 python-multipart>=0.0.7
 uvicorn>=0.12.1
 apache-libcloud>=3.3.1
 rich>=12.0.1
 duckdb>=0.7.1
 sqlalchemy>=2.0.20
 grand-cypher>=0.6.0
+grand-graph>=0.5.0
 networkx>=2.6.3
 python-louvain>=0.16
 onnx>=1.11.0
 onnxruntime>=1.11.0
 soundfile>=0.10.3.post1
 scipy>=1.4.1
 ttstokenizer>=1.0.0
 beautifulsoup4>=4.9.3
 nltk>=3.5
 pandas>=1.1.0
 tika>=1.24
 imagehash>=4.2.1
 timm>=0.4.12
-litellm>=1.31.2
-llama-cpp-python>=0.2.20
+litellm>=1.37.16
+llama-cpp-python>=0.2.75
 fasttext>=0.9.2
 sentencepiece>=0.1.91
 accelerate>=0.26.0
 bitsandbytes>=0.42.0
 onnxmltools>=1.9.1
 peft>=0.8.1
 skl2onnx>=1.9.1
 annoy>=1.16.3
 hnswlib>=0.5.0
+pgvector>=0.2.5
 pymagnitude-lite>=0.1.43
 scikit-learn>=0.23.1
 sentence-transformers>=2.2.0
 croniter>=1.2.0
 openpyxl>=3.0.9
 requests>=2.26.0
 xmltodict>=0.12.0
 
+[ann]
+annoy>=1.16.3
+hnswlib>=0.5.0
+pgvector>=0.2.5
+sqlalchemy>=2.0.20
+
 [api]
 aiohttp>=3.8.1
 fastapi>=0.94.0
 msgpack>=1.0.7
 pillow>=7.1.2
 python-multipart>=0.0.7
 uvicorn>=0.12.1
@@ -78,16 +86,18 @@
 mkdocs-redirects
 mkdocstrings[python]
 pre-commit
 pylint
 
 [graph]
 grand-cypher>=0.6.0
+grand-graph>=0.5.0
 networkx>=2.6.3
 python-louvain>=0.16
+sqlalchemy>=2.0.20
 
 [model]
 onnx>=1.11.0
 onnxruntime>=1.11.0
 
 [pipeline]
 onnx>=1.11.0
@@ -98,16 +108,16 @@
 beautifulsoup4>=4.9.3
 nltk>=3.5
 pandas>=1.1.0
 tika>=1.24
 imagehash>=4.2.1
 pillow>=7.1.2
 timm>=0.4.12
-litellm>=1.31.2
-llama-cpp-python>=0.2.20
+litellm>=1.37.16
+llama-cpp-python>=0.2.75
 fasttext>=0.9.2
 sentencepiece>=0.1.91
 accelerate>=0.26.0
 bitsandbytes>=0.42.0
 onnxmltools>=1.9.1
 peft>=0.8.1
 skl2onnx>=1.9.1
@@ -127,34 +137,49 @@
 
 [pipeline-image]
 imagehash>=4.2.1
 pillow>=7.1.2
 timm>=0.4.12
 
 [pipeline-llm]
-litellm>=1.31.2
-llama-cpp-python>=0.2.20
+litellm>=1.37.16
+llama-cpp-python>=0.2.75
 
 [pipeline-text]
 fasttext>=0.9.2
 sentencepiece>=0.1.91
 
 [pipeline-train]
 accelerate>=0.26.0
 bitsandbytes>=0.42.0
 onnx>=1.11.0
 onnxmltools>=1.9.1
 onnxruntime>=1.11.0
 peft>=0.8.1
 skl2onnx>=1.9.1
 
+[scoring]
+sqlalchemy>=2.0.20
+
 [similarity]
 annoy>=1.16.3
-fasttext>=0.9.2
 hnswlib>=0.5.0
+pgvector>=0.2.5
+sqlalchemy>=2.0.20
+fasttext>=0.9.2
+litellm>=1.37.16
+llama-cpp-python>=0.2.75
+pymagnitude-lite>=0.1.43
+scikit-learn>=0.23.1
+sentence-transformers>=2.2.0
+
+[vectors]
+fasttext>=0.9.2
+litellm>=1.37.16
+llama-cpp-python>=0.2.75
 pymagnitude-lite>=0.1.43
 scikit-learn>=0.23.1
 sentence-transformers>=2.2.0
 
 [workflow]
 apache-libcloud>=3.3.1
 croniter>=1.2.0
```

