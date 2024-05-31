# Comparing `tmp/qulab-2.0.9.tar.gz` & `tmp/qulab-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qulab-2.0.9.tar", last modified: Wed May 29 08:23:38 2024, max compression
+gzip compressed data, was "qulab-2.1.0.tar", last modified: Fri May 31 15:59:31 2024, max compression
```

## Comparing `qulab-2.0.9.tar` & `qulab-2.1.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.890203 qulab-2.0.9/
--rw-r--r--   0 runner     (501) staff       (20)     1065 2024-05-29 08:22:58.000000 qulab-2.0.9/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-29 08:22:58.000000 qulab-2.0.9/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-29 08:23:38.889917 qulab-2.0.9/PKG-INFO
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.889557 qulab-2.0.9/QuLab.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-29 08:23:38.000000 qulab-2.0.9/QuLab.egg-info/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)     2277 2024-05-29 08:23:38.000000 qulab-2.0.9/QuLab.egg-info/SOURCES.txt
--rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-29 08:23:38.000000 qulab-2.0.9/QuLab.egg-info/dependency_links.txt
--rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-29 08:23:38.000000 qulab-2.0.9/QuLab.egg-info/entry_points.txt
--rw-r--r--   0 runner     (501) staff       (20)      205 2024-05-29 08:23:38.000000 qulab-2.0.9/QuLab.egg-info/requires.txt
--rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-29 08:23:38.000000 qulab-2.0.9/QuLab.egg-info/top_level.txt
--rw-r--r--   0 runner     (501) staff       (20)     1953 2024-05-29 08:22:58.000000 qulab-2.0.9/README.md
--rw-r--r--   0 runner     (501) staff       (20)     1796 2024-05-29 08:22:58.000000 qulab-2.0.9/pyproject.toml
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.871085 qulab-2.0.9/qulab/
--rw-r--r--   0 runner     (501) staff       (20)       32 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      487 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.873479 qulab-2.0.9/qulab/monitor/
--rw-r--r--   0 runner     (501) staff       (20)       42 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)       97 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/__main__.py
--rwxr-xr-x   0 runner     (501) staff       (20)      744 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/config.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2455 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/dataset.py
--rwxr-xr-x   0 runner     (501) staff       (20)     1823 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/event_queue.py
--rwxr-xr-x   0 runner     (501) staff       (20)     7799 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/mainwindow.py
--rw-r--r--   0 runner     (501) staff       (20)     2305 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/monitor.py
--rwxr-xr-x   0 runner     (501) staff       (20)     3601 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/ploter.py
--rw-r--r--   0 runner     (501) staff       (20)      788 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/qt_compat.py
--rwxr-xr-x   0 runner     (501) staff       (20)     7948 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/monitor/toolbar.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.875719 qulab-2.0.9/qulab/scan/
--rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4518 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/curd.py
--rw-r--r--   0 runner     (501) staff       (20)    15694 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/expression.py
--rw-r--r--   0 runner     (501) staff       (20)    17117 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/models.py
--rw-r--r--   0 runner     (501) staff       (20)     2287 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/optimize.py
--rw-r--r--   0 runner     (501) staff       (20)    11493 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/query_record.py
--rw-r--r--   0 runner     (501) staff       (20)    22532 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/recorder.py
--rw-r--r--   0 runner     (501) staff       (20)    28438 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/scan.py
--rw-r--r--   0 runner     (501) staff       (20)     2844 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/server.py
--rw-r--r--   0 runner     (501) staff       (20)     2551 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/scan/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.876766 qulab-2.0.9/qulab/storage/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1692 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/__main__.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.876991 qulab-2.0.9/qulab/storage/backend/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/backend/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     5202 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/backend/redis.py
--rw-r--r--   0 runner     (501) staff       (20)    11865 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/base_dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     1701 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/chunk.py
--rw-r--r--   0 runner     (501) staff       (20)     4655 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/dataset.py
--rw-r--r--   0 runner     (501) staff       (20)     8343 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/file.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.878541 qulab-2.0.9/qulab/storage/models/
--rw-r--r--   0 runner     (501) staff       (20)      586 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/base.py
--rw-r--r--   0 runner     (501) staff       (20)      689 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/config.py
--rw-r--r--   0 runner     (501) staff       (20)     2716 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/file.py
--rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/ipy.py
--rw-r--r--   0 runner     (501) staff       (20)     2879 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/models.py
--rw-r--r--   0 runner     (501) staff       (20)     4970 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/record.py
--rw-r--r--   0 runner     (501) staff       (20)      798 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/report.py
--rw-r--r--   0 runner     (501) staff       (20)     2339 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/models/tag.py
--rw-r--r--   0 runner     (501) staff       (20)     2561 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/storage/storage.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.879326 qulab-2.0.9/qulab/sys/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    22449 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/chat.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.880799 qulab-2.0.9/qulab/sys/device/
--rw-r--r--   0 runner     (501) staff       (20)      149 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/device/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     6423 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/device/basedevice.py
--rw-r--r--   0 runner     (501) staff       (20)     2501 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/device/loader.py
--rw-r--r--   0 runner     (501) staff       (20)     1564 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/device/utils.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.881146 qulab-2.0.9/qulab/sys/drivers/
--rw-r--r--   0 runner     (501) staff       (20)     1867 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/drivers/FakeInstrument.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/drivers/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     2889 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/ipy_events.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.882844 qulab-2.0.9/qulab/sys/net/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     4959 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/bencoder.py
--rw-r--r--   0 runner     (501) staff       (20)     5690 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/cli.py
--rw-r--r--   0 runner     (501) staff       (20)    23509 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/dhcp.py
--rw-r--r--   0 runner     (501) staff       (20)     5322 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/dhcpd.py
--rw-r--r--   0 runner     (501) staff       (20)    38981 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/kad.py
--rw-r--r--   0 runner     (501) staff       (20)     5761 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/kcp.py
--rw-r--r--   0 runner     (501) staff       (20)     4964 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/net/nginx.py
--rw-r--r--   0 runner     (501) staff       (20)     5350 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/progress.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.886361 qulab-2.0.9/qulab/sys/rpc/
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/client.py
--rw-r--r--   0 runner     (501) staff       (20)     2567 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/exceptions.py
--rw-r--r--   0 runner     (501) staff       (20)    35327 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/msgpack.py
--rw-r--r--   0 runner     (501) staff       (20)     1274 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/msgpack.pyi
--rw-r--r--   0 runner     (501) staff       (20)    11979 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/rpc.py
--rw-r--r--   0 runner     (501) staff       (20)     3355 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/serialize.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/server.py
--rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/socket.py
--rw-r--r--   0 runner     (501) staff       (20)      594 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/utils.py
--rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/worker.py
--rw-r--r--   0 runner     (501) staff       (20)     7926 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/sys/rpc/zmq_socket.py
--rw-r--r--   0 runner     (501) staff       (20)       21 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/version.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.887854 qulab-2.0.9/qulab/visualization/
--rw-r--r--   0 runner     (501) staff       (20)     6129 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/visualization/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)     1639 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/visualization/__main__.py
--rw-r--r--   0 runner     (501) staff       (20)    14099 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/visualization/_autoplot.py
--rw-r--r--   0 runner     (501) staff       (20)    13533 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/visualization/plot_layout.py
--rw-r--r--   0 runner     (501) staff       (20)     2693 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/visualization/plot_seq.py
--rw-r--r--   0 runner     (501) staff       (20)     5735 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/visualization/qdat.py
--rw-r--r--   0 runner     (501) staff       (20)     3180 2024-05-29 08:22:58.000000 qulab-2.0.9/qulab/visualization/widgets.py
--rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-29 08:23:38.890242 qulab-2.0.9/setup.cfg
--rw-r--r--   0 runner     (501) staff       (20)      833 2024-05-29 08:22:58.000000 qulab-2.0.9/setup.py
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.887977 qulab-2.0.9/src/
--rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-29 08:22:58.000000 qulab-2.0.9/src/qulab.h
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-29 08:23:38.889326 qulab-2.0.9/tests/
--rw-r--r--   0 runner     (501) staff       (20)       30 2024-05-29 08:22:58.000000 qulab-2.0.9/tests/test_scan.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.375771 qulab-2.1.0/
+-rw-r--r--   0 runner     (501) staff       (20)     1065 2024-05-31 15:58:55.000000 qulab-2.1.0/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       35 2024-05-31 15:58:55.000000 qulab-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-31 15:59:31.375535 qulab-2.1.0/PKG-INFO
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.375213 qulab-2.1.0/QuLab.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)     3496 2024-05-31 15:59:31.000000 qulab-2.1.0/QuLab.egg-info/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)     2277 2024-05-31 15:59:31.000000 qulab-2.1.0/QuLab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner     (501) staff       (20)        1 2024-05-31 15:59:31.000000 qulab-2.1.0/QuLab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner     (501) staff       (20)       46 2024-05-31 15:59:31.000000 qulab-2.1.0/QuLab.egg-info/entry_points.txt
+-rw-r--r--   0 runner     (501) staff       (20)      205 2024-05-31 15:59:31.000000 qulab-2.1.0/QuLab.egg-info/requires.txt
+-rw-r--r--   0 runner     (501) staff       (20)        6 2024-05-31 15:59:31.000000 qulab-2.1.0/QuLab.egg-info/top_level.txt
+-rw-r--r--   0 runner     (501) staff       (20)     1953 2024-05-31 15:58:55.000000 qulab-2.1.0/README.md
+-rw-r--r--   0 runner     (501) staff       (20)     1796 2024-05-31 15:58:55.000000 qulab-2.1.0/pyproject.toml
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.363888 qulab-2.1.0/qulab/
+-rw-r--r--   0 runner     (501) staff       (20)       32 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      487 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.365343 qulab-2.1.0/qulab/monitor/
+-rw-r--r--   0 runner     (501) staff       (20)       42 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)       97 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/__main__.py
+-rwxr-xr-x   0 runner     (501) staff       (20)      744 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/config.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2455 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/dataset.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     1823 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/event_queue.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7799 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/mainwindow.py
+-rw-r--r--   0 runner     (501) staff       (20)     2305 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/monitor.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     3601 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/ploter.py
+-rw-r--r--   0 runner     (501) staff       (20)      788 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/qt_compat.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     7948 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/monitor/toolbar.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.367032 qulab-2.1.0/qulab/scan/
+-rw-r--r--   0 runner     (501) staff       (20)      124 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4518 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/curd.py
+-rw-r--r--   0 runner     (501) staff       (20)    15694 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/expression.py
+-rw-r--r--   0 runner     (501) staff       (20)    17117 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     2287 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/optimize.py
+-rw-r--r--   0 runner     (501) staff       (20)    11493 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/query_record.py
+-rw-r--r--   0 runner     (501) staff       (20)    25698 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/recorder.py
+-rw-r--r--   0 runner     (501) staff       (20)    29740 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/scan.py
+-rw-r--r--   0 runner     (501) staff       (20)     2844 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/server.py
+-rw-r--r--   0 runner     (501) staff       (20)     2551 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/scan/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.368025 qulab-2.1.0/qulab/storage/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1692 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/__main__.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.368271 qulab-2.1.0/qulab/storage/backend/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/backend/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     5202 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/backend/redis.py
+-rw-r--r--   0 runner     (501) staff       (20)    11865 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/base_dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     1701 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/chunk.py
+-rw-r--r--   0 runner     (501) staff       (20)     4655 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/dataset.py
+-rw-r--r--   0 runner     (501) staff       (20)     8343 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/file.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.369595 qulab-2.1.0/qulab/storage/models/
+-rw-r--r--   0 runner     (501) staff       (20)      586 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)      114 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/base.py
+-rw-r--r--   0 runner     (501) staff       (20)      689 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/config.py
+-rw-r--r--   0 runner     (501) staff       (20)     2716 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/file.py
+-rw-r--r--   0 runner     (501) staff       (20)     1574 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/ipy.py
+-rw-r--r--   0 runner     (501) staff       (20)     2879 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/models.py
+-rw-r--r--   0 runner     (501) staff       (20)     4970 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/record.py
+-rw-r--r--   0 runner     (501) staff       (20)      798 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/report.py
+-rw-r--r--   0 runner     (501) staff       (20)     2339 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/models/tag.py
+-rw-r--r--   0 runner     (501) staff       (20)     2561 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/storage/storage.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.370132 qulab-2.1.0/qulab/sys/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    22449 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/chat.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.370637 qulab-2.1.0/qulab/sys/device/
+-rw-r--r--   0 runner     (501) staff       (20)      149 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/device/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     6423 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/device/basedevice.py
+-rw-r--r--   0 runner     (501) staff       (20)     2501 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/device/loader.py
+-rw-r--r--   0 runner     (501) staff       (20)     1564 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/device/utils.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.370903 qulab-2.1.0/qulab/sys/drivers/
+-rw-r--r--   0 runner     (501) staff       (20)     1867 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/drivers/FakeInstrument.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/drivers/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     2889 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/ipy_events.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.371918 qulab-2.1.0/qulab/sys/net/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     4959 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/bencoder.py
+-rw-r--r--   0 runner     (501) staff       (20)     5690 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/cli.py
+-rw-r--r--   0 runner     (501) staff       (20)    23509 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/dhcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     5322 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/dhcpd.py
+-rw-r--r--   0 runner     (501) staff       (20)    38981 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/kad.py
+-rw-r--r--   0 runner     (501) staff       (20)     5761 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/kcp.py
+-rw-r--r--   0 runner     (501) staff       (20)     4964 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/net/nginx.py
+-rw-r--r--   0 runner     (501) staff       (20)     5350 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/progress.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.373676 qulab-2.1.0/qulab/sys/rpc/
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/client.py
+-rw-r--r--   0 runner     (501) staff       (20)     2567 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/exceptions.py
+-rw-r--r--   0 runner     (501) staff       (20)    35327 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/msgpack.py
+-rw-r--r--   0 runner     (501) staff       (20)     1274 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/msgpack.pyi
+-rw-r--r--   0 runner     (501) staff       (20)    11979 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/rpc.py
+-rw-r--r--   0 runner     (501) staff       (20)     3355 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/serialize.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/server.py
+-rw-r--r--   0 runner     (501) staff       (20)      713 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/socket.py
+-rw-r--r--   0 runner     (501) staff       (20)      594 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/utils.py
+-rw-r--r--   0 runner     (501) staff       (20)        0 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/worker.py
+-rw-r--r--   0 runner     (501) staff       (20)     7926 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/sys/rpc/zmq_socket.py
+-rw-r--r--   0 runner     (501) staff       (20)       21 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/version.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.374693 qulab-2.1.0/qulab/visualization/
+-rw-r--r--   0 runner     (501) staff       (20)     6129 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/visualization/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)     1639 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/visualization/__main__.py
+-rw-r--r--   0 runner     (501) staff       (20)    14099 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/visualization/_autoplot.py
+-rw-r--r--   0 runner     (501) staff       (20)    13533 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/visualization/plot_layout.py
+-rw-r--r--   0 runner     (501) staff       (20)     2693 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/visualization/plot_seq.py
+-rw-r--r--   0 runner     (501) staff       (20)     5735 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/visualization/qdat.py
+-rw-r--r--   0 runner     (501) staff       (20)     3180 2024-05-31 15:58:55.000000 qulab-2.1.0/qulab/visualization/widgets.py
+-rw-r--r--   0 runner     (501) staff       (20)       38 2024-05-31 15:59:31.375807 qulab-2.1.0/setup.cfg
+-rw-r--r--   0 runner     (501) staff       (20)      833 2024-05-31 15:58:55.000000 qulab-2.1.0/setup.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.374831 qulab-2.1.0/src/
+-rw-r--r--   0 runner     (501) staff       (20)       63 2024-05-31 15:58:55.000000 qulab-2.1.0/src/qulab.h
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-05-31 15:59:31.375038 qulab-2.1.0/tests/
+-rw-r--r--   0 runner     (501) staff       (20)       30 2024-05-31 15:58:55.000000 qulab-2.1.0/tests/test_scan.py
```

### Comparing `qulab-2.0.9/LICENSE` & `qulab-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/PKG-INFO` & `qulab-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.0.9
+Version: 2.1.0
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
```

### Comparing `qulab-2.0.9/QuLab.egg-info/PKG-INFO` & `qulab-2.1.0/QuLab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuLab
-Version: 2.0.9
+Version: 2.1.0
 Summary: contral instruments and manage data
 Author-email: feihoo87 <feihoo87@gmail.com>
 Maintainer-email: feihoo87 <feihoo87@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/feihoo87/QuLab
 Project-URL: Bug Reports, https://github.com/feihoo87/QuLab/issues
 Project-URL: Source, https://github.com/feihoo87/QuLab/
```

### Comparing `qulab-2.0.9/QuLab.egg-info/SOURCES.txt` & `qulab-2.1.0/QuLab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/README.md` & `qulab-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/pyproject.toml` & `qulab-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/monitor/config.py` & `qulab-2.1.0/qulab/monitor/config.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/monitor/dataset.py` & `qulab-2.1.0/qulab/monitor/dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/monitor/event_queue.py` & `qulab-2.1.0/qulab/monitor/event_queue.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/monitor/mainwindow.py` & `qulab-2.1.0/qulab/monitor/mainwindow.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/monitor/monitor.py` & `qulab-2.1.0/qulab/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/monitor/ploter.py` & `qulab-2.1.0/qulab/monitor/ploter.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/monitor/qt_compat.py` & `qulab-2.1.0/qulab/monitor/qt_compat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/monitor/toolbar.py` & `qulab-2.1.0/qulab/monitor/toolbar.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/scan/curd.py` & `qulab-2.1.0/qulab/scan/curd.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/scan/expression.py` & `qulab-2.1.0/qulab/scan/expression.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/scan/models.py` & `qulab-2.1.0/qulab/scan/models.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/scan/optimize.py` & `qulab-2.1.0/qulab/scan/optimize.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/scan/query_record.py` & `qulab-2.1.0/qulab/scan/query_record.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/scan/recorder.py` & `qulab-2.1.0/qulab/scan/recorder.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,22 +65,22 @@
 
 class BufferList():
 
     def __init__(self, file=None, slice=None):
         self._list = []
         self.lu = ()
         self.rd = ()
-        self.inner_shape = None
+        self.inner_shape = ()
         self.file = file
         self._slice = slice
         self._lock = Lock()
-        self._database = None
+        self._data_id = None
 
     def __repr__(self):
-        return f"<BufferList: lu={self.lu}, rd={self.rd}, slice={self._slice}>"
+        return f"<BufferList: shape={self.shape}, lu={self.lu}, rd={self.rd}, slice={self._slice}>"
 
     def __getstate__(self):
         self.flush()
         if isinstance(self.file, Path):
             file = '/'.join(self.file.parts[-4:])
         else:
             file = self.file
@@ -95,19 +95,20 @@
         self.file = state['file']
         self.lu = state['lu']
         self.rd = state['rd']
         self.inner_shape = state['inner_shape']
         self._list = []
         self._slice = None
         self._lock = Lock()
-        self._database = None
+        self._data_id = None
 
     @property
     def shape(self):
-        return tuple([i - j for i, j in zip(self.rd, self.lu)])
+        return tuple([i - j
+                      for i, j in zip(self.rd, self.lu)]) + self.inner_shape
 
     def flush(self):
         if not self._list:
             return
         if isinstance(self.file, Path):
             with self._lock:
                 with open(self.file, 'ab') as f:
@@ -139,19 +140,35 @@
                         try:
                             pos, value = dill.load(f)
                             yield pos, value
                         except EOFError:
                             break
 
     def iter(self):
-        for pos, value in itertools.chain(self._iter_file(), self._list):
-            if not self._slice:
-                yield pos, value
-            elif all([index_in_slice(s, i) for s, i in zip(self._slice, pos)]):
-                yield pos, value[self._slice[len(pos):]]
+        if self._data_id is None:
+            for pos, value in itertools.chain(self._iter_file(), self._list):
+                if not self._slice:
+                    yield pos, value
+                elif all(
+                    [index_in_slice(s, i) for s, i in zip(self._slice, pos)]):
+                    if self.inner_shape:
+                        yield pos, value[self._slice[len(pos):]]
+                    else:
+                        yield pos, value
+        else:
+            server, record_id, key = self._data_id
+            with ZMQContextManager(zmq.DEALER, connect=server) as socket:
+                socket.send_pyobj({
+                    'method': 'bufferlist_slice',
+                    'record_id': record_id,
+                    'key': key,
+                    'slice': self._slice
+                })
+                ret = socket.recv_pyobj()
+                yield from ret
 
     def value(self):
         d = []
         for pos, value in self.iter():
             d.append(value)
         return d
 
@@ -166,55 +183,119 @@
         for pos, value in self.iter():
             p.append(pos)
             d.append(value)
         return p, d
 
     def array(self):
         pos, data = self.items()
-        pos = np.asarray(pos) - np.asarray(self.lu)
+        if self._slice:
+            pos = np.asarray(pos)
+            lu = tuple(np.min(pos, axis=0))
+            rd = tuple(np.max(pos, axis=0) + 1)
+            pos = np.asarray(pos) - np.asarray(lu)
+            shape = []
+            for k, (s, i, j) in enumerate(zip(self._slice, rd, lu)):
+                if s.step is not None:
+                    pos[:, k] = pos[:, k] / s.step
+                    shape.append(round(np.ceil((i - j) / s.step)))
+                else:
+                    shape.append(i - j)
+            shape = tuple(shape)
+        else:
+            shape = tuple([i - j for i, j in zip(self.rd, self.lu)])
+            pos = np.asarray(pos) - np.asarray(self.lu)
         data = np.asarray(data)
         inner_shape = data.shape[1:]
-        x = np.full(self.shape + inner_shape, np.nan, dtype=data[0].dtype)
+        x = np.full(shape + inner_shape, np.nan, dtype=data[0].dtype)
         x.__setitem__(tuple(pos.T), data)
         return x
 
     def _full_slice(self, slice_tuple: slice
                     | tuple[slice | int | EllipsisType, ...]):
+        ndim = len(self.lu)
+        if self.inner_shape:
+            ndim += len(self.inner_shape)
+
         if isinstance(slice_tuple, slice):
-            slice_tuple = (slice_tuple, ) + (slice(0, sys.maxsize,
-                                                   1), ) * (len(self.lu) - 1)
+            slice_tuple = (
+                slice_tuple, ) + (slice(0, sys.maxsize, 1), ) * (ndim - 1)
         if slice_tuple is Ellipsis:
-            slice_tuple = (slice(0, sys.maxsize, 1), ) * len(self.lu)
+            slice_tuple = (slice(0, sys.maxsize, 1), ) * ndim
         else:
-            head, tail = [], []
+            head, tail = (), ()
             for i, s in enumerate(slice_tuple):
                 if s is Ellipsis:
                     head = slice_tuple[:i]
                     tail = slice_tuple[i + 1:]
                     break
-            slice_tuple = head + (slice(0, sys.maxsize, 1), ) * (
-                len(self.lu) - len(head) - len(tail)) + tail
+            else:
+                head = slice_tuple
+                tail = ()
+            slice_tuple = head + (slice(
+                0, sys.maxsize, 1), ) * (ndim - len(head) - len(tail)) + tail
         slice_list = []
-        for s in slice_tuple:
+        contract = []
+        reversed = []
+        for i, s in enumerate(slice_tuple):
             if isinstance(s, int):
-                slice_list.append(s)
+                if s >= 0:
+                    slice_list.append(slice(s, s + 1, 1))
+                elif i < len(self.lu):
+                    s = self.rd[i] + s
+                    slice_list.append(slice(s, s + 1, 1))
+                else:
+                    slice_list.append(slice(s, s - 1, -1))
+                contract.append(i)
             else:
                 start, stop, step = s.start, s.stop, s.step
+                if step is None:
+                    step = 1
+                if step < 0 and i < len(self.lu):
+                    step = -step
+                    reversed.append(i)
+                    if start is None and stop is None:
+                        start, stop = 0, sys.maxsize
+                    elif start is None:
+                        start, stop = self.lu[i], sys.maxsize
+                    elif stop is None:
+                        start, stop = 0, start + self.lu[i]
+                    else:
+                        start, stop = stop + self.lu[i] + 1, start + self.lu[
+                            i] + 1
+
                 if start is None:
                     start = 0
+                elif start < 0 and i < len(self.lu):
+                    start = self.rd[i] + start
                 if step is None:
                     step = 1
                 if stop is None:
                     stop = sys.maxsize
+                elif stop < 0 and i < len(self.lu):
+                    stop = self.rd[i] + stop
+
                 slice_list.append(slice(start, stop, step))
-        return tuple(slice_list)
+        return tuple(slice_list), contract, reversed
 
     def __getitem__(self, slice_tuple: slice | EllipsisType
                     | tuple[slice | int | EllipsisType, ...]):
-        return super().__getitem__(self._full_slice(slice_tuple))
+        self._slice, contract, reversed = self._full_slice(slice_tuple)
+        ret = self.array()
+        slices = []
+        for i, s in enumerate(self._slice):
+            if i in contract:
+                slices.append(0)
+            elif isinstance(s, slice):
+                if i in reversed:
+                    slices.append(slice(None, None, -1))
+                else:
+                    slices.append(slice(None, None, 1))
+        ret = ret.__getitem__(tuple(slices))
+        self._slice = None
+        return ret
 
 
 class Record():
 
     def __init__(self, id, database, description=None):
         from .scan import OptimizeSpace
 
@@ -306,40 +387,40 @@
         return isinstance(self.database,
                           str) and self.database.startswith("tcp://")
 
     def __del__(self):
         self.flush()
 
     def __getitem__(self, key):
-        return self.get(key)
+        return self.get(key, buffer_to_array=True)
 
-    def get(self, key, default=_notgiven, buffer_to_array=True, slice=None):
+    def get(self, key, default=_notgiven, buffer_to_array=False, slice=None):
         if self.is_remote_record():
             with ZMQContextManager(zmq.DEALER,
                                    connect=self.database) as socket:
                 socket.send_pyobj({
                     'method': 'record_getitem',
                     'record_id': self.id,
                     'key': key
                 })
                 ret = socket.recv_pyobj()
                 if isinstance(ret, BufferList):
-                    socket.send_pyobj({
-                        'method': 'bufferlist_slice',
-                        'record_id': self.id,
-                        'key': key,
-                        'slice': slice
-                    })
-                    lst = socket.recv_pyobj()
-                    ret._list = lst
-                    ret._slice = slice
                     if buffer_to_array:
+                        socket.send_pyobj({
+                            'method': 'bufferlist_slice',
+                            'record_id': self.id,
+                            'key': key,
+                            'slice': slice
+                        })
+                        lst = socket.recv_pyobj()
+                        ret._list = lst
+                        ret._slice = slice
                         return ret.array()
                     else:
-                        ret._database = self.database
+                        ret._data_id = self.database, self.id, key
                         return ret
                 else:
                     return ret
         else:
             if default is _notgiven:
                 d = self._items.get(key)
             else:
```

### Comparing `qulab-2.0.9/qulab/scan/scan.py` & `qulab-2.1.0/qulab/scan/scan.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import inspect
 import itertools
 import os
 import re
 import sys
 import uuid
 import warnings
+from concurrent.futures import ProcessPoolExecutor
 from graphlib import TopologicalSorter
 from pathlib import Path
 from types import MethodType
 from typing import Any, Awaitable, Callable, Iterable, Type
 
 import dill
 import numpy as np
@@ -153,14 +154,19 @@
     def __getitem__(self, key):
         return Promise(self.task, key, None)
 
     def __getattr__(self, attr):
         return Promise(self.task, None, attr)
 
 
+def _run_function_in_process(buf):
+    func, args, kwds = dill.loads(buf)
+    return func(*args, **kwds)
+
+
 class Scan():
 
     def __new__(cls, *args, mixin=None, **kwds):
         if mixin is None:
             return super().__new__(cls)
         for k in dir(mixin):
             if not hasattr(cls, k):
@@ -172,14 +178,16 @@
 
     def __init__(self,
                  app: str = 'task',
                  tags: tuple[str] = (),
                  database: str | Path
                  | None = f'tcp://127.0.0.1:{default_record_port}',
                  dump_globals: bool = False,
+                 max_workers: int = 4,
+                 max_promise: int = 100,
                  mixin=None):
         self.id = task_uuid()
         self.record = None
         self.namespace = {}
         self.description = {
             'app': app,
             'tags': tags,
@@ -203,65 +211,72 @@
                 'cmds': []
             },
         }
         self._current_level = 0
         self._variables = {}
         self._main_task = None
         self._sock = None
-        self._sem = asyncio.Semaphore(100)
+        self._sem = asyncio.Semaphore(max_promise + 1)
         self._bar: dict[int, tqdm] = {}
         self._hide_pattern_re = re.compile('|'.join(self.description['hiden']))
-        self._task_queue = asyncio.Queue()
-        self._task_pool = []
+        self._msg_queue = asyncio.Queue()
+        self._prm_queue = asyncio.Queue()
         self._single_step = True
+        self._max_workers = max_workers
+        self._max_promise = max_promise
+        self._executors = ProcessPoolExecutor(max_workers=max_workers)
 
     def __del__(self):
         try:
             self._main_task.cancel()
         except:
             pass
-        for task in self._task_pool:
-            try:
-                task.cancel()
-            except:
-                pass
 
     def __getstate__(self) -> dict:
         state = self.__dict__.copy()
         del state['record']
         del state['_sock']
         del state['_main_task']
         del state['_bar']
-        del state['_task_queue']
-        del state['_task_pool']
+        del state['_msg_queue']
+        del state['_prm_queue']
         del state['_sem']
+        del state['_executors']
         return state
 
     def __setstate__(self, state: dict) -> None:
         self.__dict__.update(state)
         self.record = None
         self._sock = None
         self._main_task = None
         self._bar = {}
-        self._task_queue = asyncio.Queue()
-        self._task_pool = []
-        self._sem = asyncio.Semaphore(100)
+        self._prm_queue = asyncio.Queue()
+        self._msg_queue = asyncio.Queue()
+        self._sem = asyncio.Semaphore(self._max_promise + 1)
+        self._executors = ProcessPoolExecutor(max_workers=self._max_workers)
         for opt in self.description['optimizers'].values():
             opt.scanner = self
 
+    def __del__(self):
+        try:
+            self._main_task.cancel()
+        except:
+            pass
+        self._executors.shutdown()
+
     @property
     def current_level(self):
         return self._current_level
 
     @property
     def variables(self) -> dict[str, Any]:
         return self._variables
 
-    async def emit(self, current_level, step, position, variables: dict[str,
-                                                                        Any]):
+    async def _emit(self, current_level, step, position, variables: dict[str,
+                                                                         Any]):
         for key, value in list(variables.items()):
             if inspect.isawaitable(value) and not self.hiden(key):
                 variables[key] = await value
         if self._sock is not None:
             await self._sock.send_pyobj({
                 'task': self.id,
                 'method': 'record_append',
@@ -276,28 +291,33 @@
             })
         else:
             self.record.append(current_level, step, position, {
                 k: v
                 for k, v in variables.items() if not self.hiden(k)
             })
 
+    def emit(self, current_level, step, position, variables: dict[str, Any]):
+        self._msg_queue.put_nowait(
+            asyncio.create_task(
+                self._emit(current_level, step, position, variables.copy())))
+
     def hide(self, name: str):
         self.description['hiden'].append(name)
         self._hide_pattern_re = re.compile('|'.join(self.description['hiden']))
 
     def hiden(self, name: str) -> bool:
         return bool(self._hide_pattern_re.match(name))
 
     async def _filter(self, variables: dict[str, Any], level: int = 0):
         try:
-            return all([
-                await call_function(fun, variables) for fun in itertools.chain(
+            return all(await asyncio.gather(*[
+                call_function(fun, variables) for fun in itertools.chain(
                     self.description['filters'].get(level, []),
                     self.description['filters'].get(-1, []))
-            ])
+            ]))
         except:
             return True
 
     async def create_record(self):
         if self._sock is not None:
             await self._sock.send_pyobj({
                 'task':
@@ -428,19 +448,23 @@
         self.description['optimizers'][name] = opt
         if getter:
             self.description['getters'][name] = getter
         return opt
 
     async def _update_progress(self):
         while True:
-            task = await self._task_queue.get()
-            if isinstance(task, asyncio.Event):
-                task.set()
-            elif inspect.isawaitable(task):
-                await task
+            task = await self._prm_queue.get()
+            await task
+            self._prm_queue.task_done()
+
+    async def _send_msg(self):
+        while True:
+            task = await self._msg_queue.get()
+            await task
+            self._msg_queue.task_done()
 
     async def run(self):
         assymbly(self.description)
         if isinstance(
                 self.description['database'],
                 str) and self.description['database'].startswith("tcp://"):
             async with ZMQContextManager(
@@ -448,52 +472,49 @@
                     connect=self.description['database']) as socket:
                 self._sock = socket
                 await self._run()
         else:
             await self._run()
 
     async def _run(self):
-        task = asyncio.create_task(self._update_progress())
-        self._task_pool.append(task)
+        send_msg = asyncio.create_task(self._send_msg())
+        update_progress_task = asyncio.create_task(self._update_progress())
+
         self._variables = {'self': self}
-        self._variables.update(self.description['consts'].copy())
+
+        await update_variables(self._variables, self.description['consts'],
+                               self.description['setters'])
         for level, total in self.description['total'].items():
             if total == np.inf:
                 total = None
             self._bar[level] = tqdm(total=total)
-        for group in self.description['order'].get(-1, []):
-            for name in group:
-                if name in self.description['functions']:
-                    self.variables[name] = await call_function(
-                        self.description['functions'][name], self.variables)
-                if name in self.description['setters']:
-                    coro = self.description['setters'][name](
-                        self.variables[name])
-                    if inspect.isawaitable(coro):
-                        await coro
+
+        updates = await call_many_functions(
+            self.description['order'].get(-1, []),
+            self.description['functions'], self.variables)
+        await update_variables(self.variables, updates,
+                               self.description['setters'])
+
         self.record = await self.create_record()
         await self.work()
         for level, bar in self._bar.items():
             bar.close()
 
-        while not self._task_queue.empty():
-            evt = self._task_queue.get_nowait()
-            if isinstance(evt, asyncio.Event):
-                evt.set()
-            elif inspect.isawaitable(evt):
-                await evt
         if self._single_step:
-            for group in self.description['order'].get(-1, []):
-                for name in group:
-                    if name in self.description['getters']:
-                        self.variables[name] = await call_function(
-                            self.description['getters'][name], self.variables)
-            await self.emit(0, 0, 0, self.variables.copy())
-            await self.emit(-1, 0, 0, {})
-        task.cancel()
+            self.variables.update(await call_many_functions(
+                self.description['order'].get(-1, []),
+                self.description['getters'], self.variables))
+
+            self.emit(0, 0, 0, self.variables)
+            self.emit(-1, 0, 0, {})
+
+        await self._prm_queue.join()
+        update_progress_task.cancel()
+        await self._msg_queue.join()
+        send_msg.cancel()
         return self.variables
 
     async def done(self):
         if self._main_task is not None:
             try:
                 await self._main_task
             except asyncio.CancelledError:
@@ -532,43 +553,38 @@
             self._bar[level].update(n)
 
     async def iter(self, **kwds):
         if self.current_level >= len(self.description['loops']):
             return
         step = 0
         position = 0
-        self._task_queue.put_nowait(
-            self._reset_progress_bar(self.current_level))
+        self._prm_queue.put_nowait(self._reset_progress_bar(
+            self.current_level))
         async for variables in _iter_level(
                 self.variables,
                 self.description['loops'].get(self.current_level, []),
                 self.description['order'].get(self.current_level, []),
                 self.description['functions'], self.description['optimizers'],
                 self.description['setters'], self.description['getters']):
             self._current_level += 1
             if await self._filter(variables, self.current_level - 1):
                 yield variables
                 self._single_step = False
-                asyncio.create_task(
-                    self.emit(self.current_level - 1, step, position,
-                              variables.copy()))
+                self.emit(self.current_level - 1, step, position, variables)
                 step += 1
             position += 1
             self._current_level -= 1
-            self._task_queue.put_nowait(
+            self._prm_queue.put_nowait(
                 self._update_progress_bar(self.current_level, 1))
         if self.current_level == 0:
-            await self.emit(self.current_level - 1, 0, 0, {})
+            self.emit(self.current_level - 1, 0, 0, {})
             for name, value in self.variables.items():
                 if inspect.isawaitable(value):
                     self.variables[name] = await value
-            while not self._task_queue.empty():
-                task = self._task_queue.get_nowait()
-                if inspect.isawaitable(task):
-                    await task
+            await self._prm_queue.join()
 
     async def work(self, **kwds):
         if self.current_level in self.description['actions']:
             action = self.description['actions'][self.current_level]
             coro = action(self, **kwds)
             if inspect.isawaitable(coro):
                 await coro
@@ -585,29 +601,41 @@
 
         Args:
             action: A callable object.
             level: The level of the scan to mount the action.
         """
         self.description['actions'][level] = action
 
-    async def promise(self, awaitable: Awaitable) -> Promise:
+    async def promise(self, awaitable: Awaitable | Callable, *args,
+                      **kwds) -> Promise:
         """
         Promise to calculate asynchronous function and return the result in future.
 
         Args:
             awaitable: An awaitable object.
 
         Returns:
             Promise: A promise object.
         """
         if inspect.isawaitable(awaitable):
             async with self._sem:
                 task = asyncio.create_task(self._await(awaitable))
-                self._task_queue.put_nowait(task)
+                self._prm_queue.put_nowait(task)
+                return Promise(task)
+        elif inspect.iscoroutinefunction(awaitable):
+            return await self.promise(awaitable(*args, **kwds))
+        elif callable(awaitable):
+            try:
+                buf = dill.dumps((awaitable, args, kwds))
+                task = asyncio.get_running_loop().run_in_executor(
+                    self._executors, _run_function_in_process, buf)
+                self._prm_queue.put_nowait(task)
                 return Promise(task)
+            except:
+                return awaitable(*args, **kwds)
         else:
             return awaitable
 
     async def _await(self, awaitable: Awaitable):
         async with self._sem:
             return await awaitable
 
@@ -781,21 +809,25 @@
             ready = list(keys & set(ready))
             if ready:
                 description['order'][level].append(ready)
                 keys -= set(ready)
     return description
 
 
-async def _update_variables(variables, updates, setters):
+async def update_variables(variables: dict[str, Any], updates: dict[str, Any],
+                           setters: dict[str, Callable]):
+    coros = []
     for name, value in updates.items():
         if name in setters:
             coro = setters[name](value)
             if inspect.isawaitable(coro):
-                await coro
+                coros.append(coro)
         variables[name] = value
+    if coros:
+        await asyncio.gather(*coros)
 
 
 async def _iter_level(variables,
                       iters: list[tuple[str, Iterable | Expression | Callable
                                         | OptimizeSpace]],
                       order: list[list[str]],
                       functions: dict[str, Callable | Expression],
@@ -820,39 +852,31 @@
 
     maxiter = 0xffffffff
     for name, opt in opts.items():
         opt_cfg = optimizers[name]
         maxiter = min(maxiter, opt_cfg.maxiter)
 
     async for args in async_zip(*iters_d.values(), range(maxiter)):
-        await _update_variables(variables, dict(zip(iters_d.keys(),
-                                                    args[:-1])), setters)
+        await update_variables(variables, dict(zip(iters_d.keys(), args[:-1])),
+                               setters)
         for name, opt in opts.items():
             args = opt.ask()
             opt_cfg = optimizers[name]
-            await _update_variables(variables, {
+            await update_variables(variables, {
                 n: v
                 for n, v in zip(opt_cfg.dimensions.keys(), args)
             }, setters)
 
-        for group in order:
-            for name in group:
-                if name in functions:
-                    await _update_variables(variables, {
-                        name:
-                        await call_function(functions[name], variables)
-                    }, setters)
+        await update_variables(
+            variables, await call_many_functions(order, functions, variables),
+            setters)
 
         yield variables
 
-        for group in order:
-            for name in group:
-                if name in getters:
-                    variables[name] = await call_function(
-                        getters[name], variables)
+        variables.update(await call_many_functions(order, getters, variables))
 
         for name, opt in opts.items():
             opt_cfg = optimizers[name]
             args = [variables[n] for n in opt_cfg.dimensions.keys()]
             if name not in variables:
                 raise ValueError(f'{name} not in variables.')
             fun = variables[name]
@@ -862,14 +886,32 @@
                 opt.tell(args, fun)
             else:
                 opt.tell(args, -fun)
 
     for name, opt in opts.items():
         opt_cfg = optimizers[name]
         result = opt.get_result()
-        variables.update({
-            n: v
-            for n, v in zip(opt_cfg.dimensions.keys(), result.x)
-        })
+        await update_variables(
+            variables, {
+                name: value
+                for name, value in zip(opt_cfg.dimensions.keys(), result.x)
+            }, setters)
         variables[name] = result.fun
     if opts:
         yield variables
+
+
+async def call_many_functions(order: list[list[str]],
+                              functions: dict[str, Callable],
+                              variables: dict[str, Any]) -> dict[str, Any]:
+    ret = {}
+    for group in order:
+        waited = []
+        coros = []
+        for name in group:
+            if name in functions:
+                waited.append(name)
+                coros.append(call_function(functions[name], variables | ret))
+        if coros:
+            results = await asyncio.gather(*coros)
+            ret.update(dict(zip(waited, results)))
+    return ret
```

### Comparing `qulab-2.0.9/qulab/scan/server.py` & `qulab-2.1.0/qulab/scan/server.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/scan/utils.py` & `qulab-2.1.0/qulab/scan/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/storage/__main__.py` & `qulab-2.1.0/qulab/storage/__main__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/storage/backend/redis.py` & `qulab-2.1.0/qulab/storage/backend/redis.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/storage/base_dataset.py` & `qulab-2.1.0/qulab/storage/base_dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/storage/chunk.py` & `qulab-2.1.0/qulab/storage/chunk.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/storage/dataset.py` & `qulab-2.1.0/qulab/storage/dataset.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/storage/file.py` & `qulab-2.1.0/qulab/storage/file.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/storage/models/__init__.py` & `qulab-2.1.0/qulab/storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/storage/models/config.py` & `qulab-2.1.0/qulab/storage/models/config.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/storage/models/file.py` & `qulab-2.1.0/qulab/storage/models/file.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/storage/models/ipy.py` & `qulab-2.1.0/qulab/storage/models/ipy.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/storage/models/models.py` & `qulab-2.1.0/qulab/storage/models/models.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/storage/models/record.py` & `qulab-2.1.0/qulab/storage/models/record.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/storage/models/report.py` & `qulab-2.1.0/qulab/storage/models/report.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/storage/models/tag.py` & `qulab-2.1.0/qulab/storage/models/tag.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/storage/storage.py` & `qulab-2.1.0/qulab/storage/storage.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/chat.py` & `qulab-2.1.0/qulab/sys/chat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/device/basedevice.py` & `qulab-2.1.0/qulab/sys/device/basedevice.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/device/loader.py` & `qulab-2.1.0/qulab/sys/device/loader.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/device/utils.py` & `qulab-2.1.0/qulab/sys/device/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/drivers/FakeInstrument.py` & `qulab-2.1.0/qulab/sys/drivers/FakeInstrument.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/ipy_events.py` & `qulab-2.1.0/qulab/sys/ipy_events.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/net/bencoder.py` & `qulab-2.1.0/qulab/sys/net/bencoder.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/net/cli.py` & `qulab-2.1.0/qulab/sys/net/cli.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/net/dhcp.py` & `qulab-2.1.0/qulab/sys/net/dhcp.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/net/dhcpd.py` & `qulab-2.1.0/qulab/sys/net/dhcpd.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/net/kad.py` & `qulab-2.1.0/qulab/sys/net/kad.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/net/kcp.py` & `qulab-2.1.0/qulab/sys/net/kcp.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/net/nginx.py` & `qulab-2.1.0/qulab/sys/net/nginx.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/progress.py` & `qulab-2.1.0/qulab/sys/progress.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/rpc/exceptions.py` & `qulab-2.1.0/qulab/sys/rpc/exceptions.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/rpc/msgpack.py` & `qulab-2.1.0/qulab/sys/rpc/msgpack.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/rpc/msgpack.pyi` & `qulab-2.1.0/qulab/sys/rpc/msgpack.pyi`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/rpc/rpc.py` & `qulab-2.1.0/qulab/sys/rpc/rpc.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/rpc/serialize.py` & `qulab-2.1.0/qulab/sys/rpc/serialize.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/rpc/server.py` & `qulab-2.1.0/qulab/sys/rpc/server.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/rpc/socket.py` & `qulab-2.1.0/qulab/sys/rpc/socket.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/rpc/utils.py` & `qulab-2.1.0/qulab/sys/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/sys/rpc/zmq_socket.py` & `qulab-2.1.0/qulab/sys/rpc/zmq_socket.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/visualization/__init__.py` & `qulab-2.1.0/qulab/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/visualization/__main__.py` & `qulab-2.1.0/qulab/visualization/__main__.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/visualization/_autoplot.py` & `qulab-2.1.0/qulab/visualization/_autoplot.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/visualization/plot_layout.py` & `qulab-2.1.0/qulab/visualization/plot_layout.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/visualization/plot_seq.py` & `qulab-2.1.0/qulab/visualization/plot_seq.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/visualization/qdat.py` & `qulab-2.1.0/qulab/visualization/qdat.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/qulab/visualization/widgets.py` & `qulab-2.1.0/qulab/visualization/widgets.py`

 * *Files identical despite different names*

### Comparing `qulab-2.0.9/setup.py` & `qulab-2.1.0/setup.py`

 * *Files identical despite different names*

