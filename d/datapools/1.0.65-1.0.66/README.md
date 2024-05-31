# Comparing `tmp/datapools-1.0.65.tar.gz` & `tmp/datapools-1.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapools-1.0.65.tar", last modified: Thu May 30 17:36:34 2024, max compression
+gzip compressed data, was "datapools-1.0.66.tar", last modified: Fri May 31 08:38:08 2024, max compression
```

## Comparing `datapools-1.0.65.tar` & `datapools-1.0.66.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.455496 datapools-1.0.65/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-30 17:36:26.000000 datapools-1.0.65/Containerfile
--rw-r--r--   0 runner    (1001) docker     (127)    22354 2024-05-30 17:36:26.000000 datapools-1.0.65/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-30 17:36:26.000000 datapools-1.0.65/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 17:36:26.000000 datapools-1.0.65/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-30 17:36:34.455496 datapools-1.0.65/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-30 17:36:26.000000 datapools-1.0.65/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.443496 datapools-1.0.65/datapools/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.443496 datapools-1.0.65/datapools/common/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/backend_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.443496 datapools-1.0.65/datapools/common/queues/
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/queues/rabbitmq.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/stoppable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/common/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/storage/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/storage/file_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/common/tasks_db/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/tasks_db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/tasks_db/redis.py.bak
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/tasks_db/tasks_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/common/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/producer/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/producer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/producer/base_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/scheduler/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/worker/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13092 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/base_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/worker/plugins/dataphoenix_info/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/dataphoenix_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/worker/plugins/default/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/default/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.447496 datapools-1.0.65/datapools/worker/plugins/deutsche_welle/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/deutsche_welle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/freesound_org/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/freesound_org/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/freesound_org/freesound_org.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/ftp/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/ftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/ftp/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/ftp/ftp_dir_listing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/google_drive/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/google_drive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/google_drive/google_drive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/imageshack/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/imageshack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/imageshack/imageshack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/s3/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/s3/s3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/theguardian/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/theguardian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/theguardian/theguardian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/washingtonpost/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/washingtonpost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/washingtonpost/washingtonpost.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/wikipedia/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/wikipedia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/wikipedia/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.451496 datapools-1.0.65/datapools/worker/plugins/youtube_channel/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/youtube_channel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/plugins/youtube_channel/youtube_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    20285 2024-05-30 17:36:26.000000 datapools-1.0.65/datapools/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.455496 datapools-1.0.65/datapools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-30 17:36:34.000000 datapools-1.0.65/datapools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-30 17:36:34.000000 datapools-1.0.65/datapools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 17:36:34.000000 datapools-1.0.65/datapools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 17:36:34.000000 datapools-1.0.65/datapools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-30 17:36:34.000000 datapools-1.0.65/datapools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 17:36:34.000000 datapools-1.0.65/datapools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 17:36:34.455496 datapools-1.0.65/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-30 17:36:26.000000 datapools-1.0.65/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:34.455496 datapools-1.0.65/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 17:36:26.000000 datapools-1.0.65/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-30 17:36:26.000000 datapools-1.0.65/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-30 17:36:26.000000 datapools-1.0.65/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-30 17:36:26.000000 datapools-1.0.65/tests/test_session_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.544300 datapools-1.0.66/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-31 08:37:51.000000 datapools-1.0.66/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    22457 2024-05-31 08:37:51.000000 datapools-1.0.66/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-05-31 08:37:51.000000 datapools-1.0.66/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-31 08:37:51.000000 datapools-1.0.66/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-31 08:38:08.540300 datapools-1.0.66/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-31 08:37:51.000000 datapools-1.0.66/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.528300 datapools-1.0.66/datapools/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.532300 datapools-1.0.66/datapools/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/common/backend_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/common/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.532300 datapools-1.0.66/datapools/common/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/common/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12022 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/common/queues/rabbitmq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/common/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/common/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/common/stoppable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.532300 datapools-1.0.66/datapools/common/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/common/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/common/storage/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/common/storage/file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.532300 datapools-1.0.66/datapools/common/tasks_db/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/common/tasks_db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/common/tasks_db/redis.py.bak
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/common/tasks_db/tasks_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/common/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.532300 datapools-1.0.66/datapools/producer/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/producer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/producer/base_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.532300 datapools-1.0.66/datapools/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13650 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/scheduler/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.532300 datapools-1.0.66/datapools/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.536300 datapools-1.0.66/datapools/worker/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13092 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/base_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.536300 datapools-1.0.66/datapools/worker/plugins/dataphoenix_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/dataphoenix_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.536300 datapools-1.0.66/datapools/worker/plugins/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/default/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.536300 datapools-1.0.66/datapools/worker/plugins/deutsche_welle/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/deutsche_welle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/deutsche_welle/deutsche_welle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.536300 datapools-1.0.66/datapools/worker/plugins/freesound_org/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/freesound_org/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/freesound_org/freesound_org.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.536300 datapools-1.0.66/datapools/worker/plugins/ftp/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/ftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/ftp/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/ftp/ftp_dir_listing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.536300 datapools-1.0.66/datapools/worker/plugins/google_drive/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/google_drive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/google_drive/google_drive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.536300 datapools-1.0.66/datapools/worker/plugins/imageshack/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/imageshack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/imageshack/imageshack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.536300 datapools-1.0.66/datapools/worker/plugins/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/s3/s3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.540300 datapools-1.0.66/datapools/worker/plugins/theguardian/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/theguardian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/theguardian/theguardian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.540300 datapools-1.0.66/datapools/worker/plugins/washingtonpost/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/washingtonpost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/washingtonpost/washingtonpost.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.540300 datapools-1.0.66/datapools/worker/plugins/wikipedia/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/wikipedia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7619 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/wikipedia/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.540300 datapools-1.0.66/datapools/worker/plugins/youtube_channel/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/youtube_channel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10203 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/plugins/youtube_channel/youtube_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20287 2024-05-31 08:37:51.000000 datapools-1.0.66/datapools/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.540300 datapools-1.0.66/datapools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-31 08:38:08.000000 datapools-1.0.66/datapools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-31 08:38:08.000000 datapools-1.0.66/datapools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 08:38:08.000000 datapools-1.0.66/datapools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-31 08:38:08.000000 datapools-1.0.66/datapools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-31 08:38:08.000000 datapools-1.0.66/datapools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 08:38:08.000000 datapools-1.0.66/datapools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 08:38:08.544300 datapools-1.0.66/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-31 08:37:51.000000 datapools-1.0.66/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 08:38:08.540300 datapools-1.0.66/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 08:37:51.000000 datapools-1.0.66/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-31 08:37:51.000000 datapools-1.0.66/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-31 08:37:51.000000 datapools-1.0.66/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-31 08:37:51.000000 datapools-1.0.66/tests/test_session_manager.py
```

### Comparing `datapools-1.0.65/HISTORY.md` & `datapools-1.0.66/HISTORY.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 Changelog
 =========
 
 
 (unreleased)
 ------------
+- Bugfix. [sergpsu]
+
+
+1.0.65 (2024-05-30)
+-------------------
+- Release: version 1.0.65 🚀 [sergpsu]
 - Linter + demo tag. [sergpsu]
 - Linter. [sergpsu]
 - Cleanup. [sergpsu]
 - Io operations instead of memory, FTP beta. [sergpsu]
 - Merge remote-tracking branch 'origin/master' into sergpsu-io-support.
   [sergpsu]
 - Merge pull request #83 from torrentsai/sergpsu-delete-all-sessions.
```

### Comparing `datapools-1.0.65/LICENSE` & `datapools-1.0.66/LICENSE`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/PKG-INFO` & `datapools-1.0.66/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.65
+Version: 1.0.66
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.65/README.md` & `datapools-1.0.66/README.md`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/api.py` & `datapools-1.0.66/datapools/api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/cli.py` & `datapools-1.0.66/datapools/cli.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/common/backend_api.py` & `datapools-1.0.66/datapools/common/backend_api.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/common/queues/__init__.py` & `datapools-1.0.66/datapools/common/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/common/queues/rabbitmq.py` & `datapools-1.0.66/datapools/common/queues/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/common/queues/types.py` & `datapools-1.0.66/datapools/common/queues/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/common/session_manager.py` & `datapools-1.0.66/datapools/common/session_manager.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/common/stoppable.py` & `datapools-1.0.66/datapools/common/stoppable.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/common/storage/base_storage.py` & `datapools-1.0.66/datapools/common/storage/base_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/common/storage/file_storage.py` & `datapools-1.0.66/datapools/common/storage/file_storage.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/common/tasks_db/redis.py.bak` & `datapools-1.0.66/datapools/common/tasks_db/redis.py.bak`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/common/tasks_db/tasks_db.py` & `datapools-1.0.66/datapools/common/tasks_db/tasks_db.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/common/types.py` & `datapools-1.0.66/datapools/common/types.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/producer/base_producer.py` & `datapools-1.0.66/datapools/producer/base_producer.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/scheduler/scheduler.py` & `datapools-1.0.66/datapools/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/worker/plugins/base_plugin.py` & `datapools-1.0.66/datapools/worker/plugins/base_plugin.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py` & `datapools-1.0.66/datapools/worker/plugins/dataphoenix_info/dataphoenix_info.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/worker/plugins/default/default.py` & `datapools-1.0.66/datapools/worker/plugins/default/default.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/worker/plugins/deutsche_welle/deutsche_welle.py` & `datapools-1.0.66/datapools/worker/plugins/deutsche_welle/deutsche_welle.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/worker/plugins/freesound_org/freesound_org.py` & `datapools-1.0.66/datapools/worker/plugins/freesound_org/freesound_org.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/worker/plugins/ftp/ftp.py` & `datapools-1.0.66/datapools/worker/plugins/ftp/ftp.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,32 +37,34 @@
 class FTPPlugin(BasePlugin):
     host: str
     user: str
     passwd: str
     ftp: FTP
     copyright_tags: List[BaseTag]
 
-    def __init__(self, ctx, host, user="anonymous", passwd="", demo_tag: Optional[str] = None):
+    def __init__(self, ctx, host="", user="anonymous", passwd="", demo_tag: Optional[str] = None):
         super().__init__(ctx)
         self.host = host
         self.user = user
         self.passwd = passwd
         self.copyright_tags = []
         if demo_tag:
             self.copyright_tags.append(BaseTag(demo_tag))
 
     @staticmethod
-    def is_supported(__url):
-        return True
+    def is_supported(url):
+        p = BasePlugin.parse_url(url)
+        return p.scheme == "ftp"
 
     async def process(self, task: WorkerTask):
         self.ftp = FTP(self.host, self.user, self.passwd)
         pwd = self.ftp.pwd()
         async for x in self._scan_dir(pwd, 0):
             yield x
+        del self.ftp
 
     async def _scan_dir(self, path, rec):
         # logger.info(f"scanning {path}")
         lister = DirectoryListing()
         self.ftp.dir(path, lister)
 
         local_copyright_tag = await self._try_find_license(path, lister.contents)
```

### Comparing `datapools-1.0.65/datapools/worker/plugins/ftp/ftp_dir_listing.py` & `datapools-1.0.66/datapools/worker/plugins/ftp/ftp_dir_listing.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/worker/plugins/google_drive/google_drive.py` & `datapools-1.0.66/datapools/worker/plugins/google_drive/google_drive.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/worker/plugins/imageshack/imageshack.py` & `datapools-1.0.66/datapools/worker/plugins/imageshack/imageshack.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/worker/plugins/s3/s3.py` & `datapools-1.0.66/datapools/worker/plugins/s3/s3.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/worker/plugins/theguardian/theguardian.py` & `datapools-1.0.66/datapools/worker/plugins/theguardian/theguardian.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/worker/plugins/washingtonpost/washingtonpost.py` & `datapools-1.0.66/datapools/worker/plugins/washingtonpost/washingtonpost.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/worker/plugins/wikipedia/wikipedia.py` & `datapools-1.0.66/datapools/worker/plugins/wikipedia/wikipedia.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/worker/plugins/youtube_channel/youtube_channel.py` & `datapools-1.0.66/datapools/worker/plugins/youtube_channel/youtube_channel.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/datapools/worker/worker.py` & `datapools-1.0.66/datapools/worker/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,22 +386,22 @@
                     else:
                         logger.info("unknown content type")
                 else:
                     logger.info("no content")
 
             if not cc.content:
                 logger.info("no content, downloading from url")
-                with tempfile.TemporaryFile("wb") as tmp:
+                with tempfile.TemporaryFile("wb+") as tmp:
                     async for chunk in plugin.async_read_url(cc.url):
                         tmp.write(chunk)
                     cc.content = tmp
                     await process_content()
             elif isinstance(cc.content, BaseReader):
                 logger.info("content is BaseReader instance")
-                with tempfile.TemporaryFile("wb") as tmp:
+                with tempfile.TemporaryFile("wb+") as tmp:
                     cc.content.read_to(tmp)
                     cc.content = tmp
                     await process_content()
             else:
                 await process_content()
 
         else:
```

### Comparing `datapools-1.0.65/datapools.egg-info/PKG-INFO` & `datapools-1.0.66/datapools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapools
-Version: 1.0.65
+Version: 1.0.66
 Summary: Awesome datapools created by openlicenseai
 Home-page: https://github.com/openlicenseai/datapools/
 Author: openlicenseai
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.6.1
 Requires-Dist: pydantic-settings==2.2.1
```

### Comparing `datapools-1.0.65/datapools.egg-info/SOURCES.txt` & `datapools-1.0.66/datapools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/setup.py` & `datapools-1.0.66/setup.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/tests/test_base.py` & `datapools-1.0.66/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `datapools-1.0.65/tests/test_session_manager.py` & `datapools-1.0.66/tests/test_session_manager.py`

 * *Files identical despite different names*

