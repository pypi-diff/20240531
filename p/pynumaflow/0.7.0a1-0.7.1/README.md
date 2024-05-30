# Comparing `tmp/pynumaflow-0.7.0a1.tar.gz` & `tmp/pynumaflow-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynumaflow-0.7.0a1.tar", max compression
+gzip compressed data, was "pynumaflow-0.7.1.tar", max compression
```

## Comparing `pynumaflow-0.7.0a1.tar` & `pynumaflow-0.7.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
--rw-r--r--   0        0        0    11357 2024-04-18 03:59:38.776839 pynumaflow-0.7.0a1/LICENSE
--rw-r--r--   0        0        0     6678 2024-04-18 03:59:38.776839 pynumaflow-0.7.0a1/README.md
--rw-r--r--   0        0        0      985 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/__init__.py
--rw-r--r--   0        0        0     2310 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/_constants.py
--rw-r--r--   0        0        0      332 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/info/__init__.py
--rw-r--r--   0        0        0     1594 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/info/server.py
--rw-r--r--   0        0        0     1422 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/info/types.py
--rw-r--r--   0        0        0      404 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/__init__.py
--rw-r--r--   0        0        0     5885 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/_dtypes.py
--rw-r--r--   0        0        0     3883 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/async_server.py
--rw-r--r--   0        0        0     4292 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/multiproc_server.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/servicer/__init__.py
--rw-r--r--   0        0        0     2658 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/servicer/async_servicer.py
--rw-r--r--   0        0        0     1351 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/servicer/sync_servicer.py
--rw-r--r--   0        0        0     1310 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/servicer/utils.py
--rw-r--r--   0        0        0     3912 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapper/sync_server.py
--rw-r--r--   0        0        0      308 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapstreamer/__init__.py
--rw-r--r--   0        0        0     5595 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapstreamer/_dtypes.py
--rw-r--r--   0        0        0     4654 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapstreamer/async_server.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapstreamer/servicer/__init__.py
--rw-r--r--   0        0        0     2410 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/mapstreamer/servicer/async_servicer.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapper/__init__.py
--rw-r--r--   0        0        0      908 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapper/map.proto
--rw-r--r--   0        0        0     2731 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapper/map_pb2.py
--rw-r--r--   0        0        0     3906 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapper/map_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapstreamer/__init__.py
--rw-r--r--   0        0        0      983 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapstreamer/mapstream.proto
--rw-r--r--   0        0        0     2913 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapstreamer/mapstream_pb2.py
--rw-r--r--   0        0        0     4174 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/mapstreamer/mapstream_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/reducer/__init__.py
--rw-r--r--   0        0        0     1823 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/reducer/reduce.proto
--rw-r--r--   0        0        0     4133 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/reducer/reduce_pb2.py
--rw-r--r--   0        0        0     4055 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/reducer/reduce_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sideinput/__init__.py
--rw-r--r--   0        0        0     1482 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sideinput/sideinput.proto
--rw-r--r--   0        0        0     1699 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sideinput/sideinput_pb2.py
--rw-r--r--   0        0        0     5798 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sideinput/sideinput_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sinker/__init__.py
--rw-r--r--   0        0        0     1318 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sinker/sink.proto
--rw-r--r--   0        0        0     3037 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sinker/sink_pb2.py
--rw-r--r--   0        0        0     3970 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sinker/sink_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcer/__init__.py
--rw-r--r--   0        0        0     6480 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcer/source.proto
--rw-r--r--   0        0        0     5075 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcer/source_pb2.py
--rw-r--r--   0        0        0     9375 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcer/source_pb2_grpc.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcetransformer/__init__.py
--rw-r--r--   0        0        0     1267 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcetransformer/transform.proto
--rw-r--r--   0        0        0     3151 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcetransformer/transform_pb2.py
--rw-r--r--   0        0        0     4534 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/proto/sourcetransformer/transform_pb2_grpc.py
--rw-r--r--   0        0        0      349 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducer/__init__.py
--rw-r--r--   0        0        0    10780 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducer/_dtypes.py
--rw-r--r--   0        0        0     6797 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducer/async_server.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducer/servicer/__init__.py
--rw-r--r--   0        0        0     5959 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducer/servicer/async_servicer.py
--rw-r--r--   0        0        0     6287 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducer/servicer/task_manager.py
--rw-r--r--   0        0        0      397 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducestreamer/__init__.py
--rw-r--r--   0        0        0     9558 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducestreamer/_dtypes.py
--rw-r--r--   0        0        0     7628 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducestreamer/async_server.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducestreamer/servicer/__init__.py
--rw-r--r--   0        0        0     5447 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducestreamer/servicer/async_servicer.py
--rw-r--r--   0        0        0    12042 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/reducestreamer/servicer/task_manager.py
--rw-r--r--   0        0        0       83 2024-04-18 03:59:38.788839 pynumaflow-0.7.0a1/pynumaflow/shared/__init__.py
--rw-r--r--   0        0        0      512 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/shared/asynciter.py
--rw-r--r--   0        0        0     8131 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/shared/server.py
--rw-r--r--   0        0        0      250 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sideinput/__init__.py
--rw-r--r--   0        0        0     1826 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sideinput/_dtypes.py
--rw-r--r--   0        0        0     3484 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sideinput/server.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sideinput/servicer/__init__.py
--rw-r--r--   0        0        0     1722 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sideinput/servicer/servicer.py
--rw-r--r--   0        0        0      270 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/__init__.py
--rw-r--r--   0        0        0     6886 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/_dtypes.py
--rw-r--r--   0        0        0     4578 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/async_server.py
--rw-r--r--   0        0        0     4266 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/server.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/servicer/__init__.py
--rw-r--r--   0        0        0     2821 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/servicer/async_servicer.py
--rw-r--r--   0        0        0     2540 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/servicer/sync_servicer.py
--rw-r--r--   0        0        0      495 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sinker/servicer/utils.py
--rw-r--r--   0        0        0      520 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcer/__init__.py
--rw-r--r--   0        0        0     7957 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcer/_dtypes.py
--rw-r--r--   0        0        0     5712 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcer/async_server.py
--rw-r--r--   0        0        0     5375 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcer/server.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcer/servicer/__init__.py
--rw-r--r--   0        0        0     5138 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcer/servicer/async_servicer.py
--rw-r--r--   0        0        0     5597 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcer/servicer/sync_servicer.py
--rw-r--r--   0        0        0      446 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/__init__.py
--rw-r--r--   0        0        0     6048 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/_dtypes.py
--rw-r--r--   0        0        0     5208 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/multiproc_server.py
--rw-r--r--   0        0        0     4845 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/server.py
--rw-r--r--   0        0        0        0 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/servicer/__init__.py
--rw-r--r--   0        0        0     2996 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/servicer/server.py
--rw-r--r--   0        0        0      170 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pynumaflow/types.py
--rw-r--r--   0        0        0     1706 2024-04-18 03:59:38.792839 pynumaflow-0.7.0a1/pyproject.toml
--rw-r--r--   0        0        0     7800 1970-01-01 00:00:00.000000 pynumaflow-0.7.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-30 22:57:37.298971 pynumaflow-0.7.1/LICENSE
+-rw-r--r--   0        0        0     6678 2024-05-30 22:57:37.298971 pynumaflow-0.7.1/README.md
+-rw-r--r--   0        0        0      985 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/__init__.py
+-rw-r--r--   0        0        0     2298 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/_constants.py
+-rw-r--r--   0        0        0      332 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/info/__init__.py
+-rw-r--r--   0        0        0     1594 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/info/server.py
+-rw-r--r--   0        0        0     1422 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/info/types.py
+-rw-r--r--   0        0        0      404 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/mapper/__init__.py
+-rw-r--r--   0        0        0     5885 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/mapper/_dtypes.py
+-rw-r--r--   0        0        0     3883 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/mapper/async_server.py
+-rw-r--r--   0        0        0     4308 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/mapper/multiproc_server.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/mapper/servicer/__init__.py
+-rw-r--r--   0        0        0     2806 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/mapper/servicer/async_servicer.py
+-rw-r--r--   0        0        0     1482 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/mapper/servicer/sync_servicer.py
+-rw-r--r--   0        0        0     1380 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/mapper/servicer/utils.py
+-rw-r--r--   0        0        0     3912 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/mapper/sync_server.py
+-rw-r--r--   0        0        0      308 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/mapstreamer/__init__.py
+-rw-r--r--   0        0        0     5595 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/mapstreamer/_dtypes.py
+-rw-r--r--   0        0        0     4654 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/mapstreamer/async_server.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/mapstreamer/servicer/__init__.py
+-rw-r--r--   0        0        0     2821 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/mapstreamer/servicer/async_servicer.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/mapper/__init__.py
+-rw-r--r--   0        0        0      908 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/mapper/map.proto
+-rw-r--r--   0        0        0     2731 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/mapper/map_pb2.py
+-rw-r--r--   0        0        0     3906 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/mapper/map_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/mapstreamer/__init__.py
+-rw-r--r--   0        0        0      983 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/mapstreamer/mapstream.proto
+-rw-r--r--   0        0        0     2913 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/mapstreamer/mapstream_pb2.py
+-rw-r--r--   0        0        0     4174 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/mapstreamer/mapstream_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/reducer/__init__.py
+-rw-r--r--   0        0        0     1823 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/reducer/reduce.proto
+-rw-r--r--   0        0        0     4133 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/reducer/reduce_pb2.py
+-rw-r--r--   0        0        0     4055 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/reducer/reduce_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sideinput/__init__.py
+-rw-r--r--   0        0        0     1482 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sideinput/sideinput.proto
+-rw-r--r--   0        0        0     1699 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sideinput/sideinput_pb2.py
+-rw-r--r--   0        0        0     5798 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sideinput/sideinput_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sinker/__init__.py
+-rw-r--r--   0        0        0     1318 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sinker/sink.proto
+-rw-r--r--   0        0        0     3037 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sinker/sink_pb2.py
+-rw-r--r--   0        0        0     3970 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sinker/sink_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sourcer/__init__.py
+-rw-r--r--   0        0        0     6480 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sourcer/source.proto
+-rw-r--r--   0        0        0     5075 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sourcer/source_pb2.py
+-rw-r--r--   0        0        0     9375 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sourcer/source_pb2_grpc.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sourcetransformer/__init__.py
+-rw-r--r--   0        0        0     1267 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sourcetransformer/transform.proto
+-rw-r--r--   0        0        0     3151 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sourcetransformer/transform_pb2.py
+-rw-r--r--   0        0        0     4534 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/proto/sourcetransformer/transform_pb2_grpc.py
+-rw-r--r--   0        0        0      349 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/reducer/__init__.py
+-rw-r--r--   0        0        0    10780 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/reducer/_dtypes.py
+-rw-r--r--   0        0        0     6797 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/reducer/async_server.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/reducer/servicer/__init__.py
+-rw-r--r--   0        0        0     6656 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/reducer/servicer/async_servicer.py
+-rw-r--r--   0        0        0     6975 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/reducer/servicer/task_manager.py
+-rw-r--r--   0        0        0      397 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/reducestreamer/__init__.py
+-rw-r--r--   0        0        0     9558 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/reducestreamer/_dtypes.py
+-rw-r--r--   0        0        0     7586 2024-05-30 22:57:37.310971 pynumaflow-0.7.1/pynumaflow/reducestreamer/async_server.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/reducestreamer/servicer/__init__.py
+-rw-r--r--   0        0        0     6284 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/reducestreamer/servicer/async_servicer.py
+-rw-r--r--   0        0        0    12061 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/reducestreamer/servicer/task_manager.py
+-rw-r--r--   0        0        0       83 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/shared/__init__.py
+-rw-r--r--   0        0        0      512 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/shared/asynciter.py
+-rw-r--r--   0        0        0     9111 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/shared/server.py
+-rw-r--r--   0        0        0      250 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sideinput/__init__.py
+-rw-r--r--   0        0        0     1826 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sideinput/_dtypes.py
+-rw-r--r--   0        0        0     3484 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sideinput/server.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sideinput/servicer/__init__.py
+-rw-r--r--   0        0        0     1656 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sideinput/servicer/servicer.py
+-rw-r--r--   0        0        0      270 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sinker/__init__.py
+-rw-r--r--   0        0        0     6886 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sinker/_dtypes.py
+-rw-r--r--   0        0        0     4578 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sinker/async_server.py
+-rw-r--r--   0        0        0     4266 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sinker/server.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sinker/servicer/__init__.py
+-rw-r--r--   0        0        0     3052 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sinker/servicer/async_servicer.py
+-rw-r--r--   0        0        0     2497 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sinker/servicer/sync_servicer.py
+-rw-r--r--   0        0        0      495 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sinker/servicer/utils.py
+-rw-r--r--   0        0        0      520 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sourcer/__init__.py
+-rw-r--r--   0        0        0     7957 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sourcer/_dtypes.py
+-rw-r--r--   0        0        0     5712 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sourcer/async_server.py
+-rw-r--r--   0        0        0     5375 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sourcer/server.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sourcer/servicer/__init__.py
+-rw-r--r--   0        0        0     5713 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sourcer/servicer/async_servicer.py
+-rw-r--r--   0        0        0     6191 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sourcer/servicer/sync_servicer.py
+-rw-r--r--   0        0        0      446 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sourcetransformer/__init__.py
+-rw-r--r--   0        0        0     6048 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sourcetransformer/_dtypes.py
+-rw-r--r--   0        0        0     5224 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sourcetransformer/multiproc_server.py
+-rw-r--r--   0        0        0     4845 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sourcetransformer/server.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sourcetransformer/servicer/__init__.py
+-rw-r--r--   0        0        0     3145 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/sourcetransformer/servicer/server.py
+-rw-r--r--   0        0        0      170 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pynumaflow/types.py
+-rw-r--r--   0        0        0     1768 2024-05-30 22:57:37.314971 pynumaflow-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7888 1970-01-01 00:00:00.000000 pynumaflow-0.7.1/PKG-INFO
```

### Comparing `pynumaflow-0.7.0a1/LICENSE` & `pynumaflow-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/README.md` & `pynumaflow-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/__init__.py` & `pynumaflow-0.7.1/pynumaflow/__init__.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/_constants.py` & `pynumaflow-0.7.1/pynumaflow/_constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 MAP_STREAM_SOCK_PATH = "/var/run/numaflow/mapstream.sock"
 REDUCE_SOCK_PATH = "/var/run/numaflow/reduce.sock"
 REDUCE_STREAM_SOCK_PATH = "/var/run/numaflow/reducestream.sock"
 SOURCE_TRANSFORMER_SOCK_PATH = "/var/run/numaflow/sourcetransform.sock"
 SINK_SOCK_PATH = "/var/run/numaflow/sink.sock"
 SIDE_INPUT_SOCK_PATH = "/var/run/numaflow/sideinput.sock"
 SOURCE_SOCK_PATH = "/var/run/numaflow/source.sock"
-MULTIPROC_MAP_SOCK_PORT = 55551
-MULTIPROC_MAP_SOCK_ADDR = "0.0.0.0"
+MULTIPROC_MAP_SOCK_ADDR = "/var/run/numaflow/multiproc"
 FALLBACK_SINK_SOCK_PATH = "/var/run/numaflow/fb-sink.sock"
 
 # Server information file configs
 MAP_SERVER_INFO_FILE_PATH = "/var/run/numaflow/mapper-server-info"
 MAP_STREAM_SERVER_INFO_FILE_PATH = "/var/run/numaflow/mapstreamer-server-info"
 REDUCE_SERVER_INFO_FILE_PATH = "/var/run/numaflow/reducer-server-info"
 REDUCE_STREAM_SERVER_INFO_FILE_PATH = "/var/run/numaflow/reducestreamer-server-info"
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/info/server.py` & `pynumaflow-0.7.1/pynumaflow/info/server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/info/types.py` & `pynumaflow-0.7.1/pynumaflow/info/types.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/mapper/_dtypes.py` & `pynumaflow-0.7.1/pynumaflow/mapper/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/mapper/async_server.py` & `pynumaflow-0.7.1/pynumaflow/mapper/async_server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/mapper/multiproc_server.py` & `pynumaflow-0.7.1/pynumaflow/mapper/multiproc_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             ("grpc.so_reuseaddr", 1),
         ]
         # Set the number of processes to be spawned to the number of CPUs or
         # the value of the env var NUM_CPU_MULTIPROC defined by the user
         # Setting the max value to 2 * CPU count
         # Used for multiproc server
         self._process_count = min(server_count, 2 * _PROCESS_COUNT)
-        self.servicer = SyncMapServicer(handler=mapper_instance)
+        self.servicer = SyncMapServicer(handler=mapper_instance, multiproc=True)
 
     def start(self) -> None:
         """
         Starts the N grpc servers gRPC serves on the with
         given max threads.
         where N = The number of CPUs or the
         value of the env var NUM_CPU_MULTIPROC defined by the user. The max value
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/mapper/servicer/async_servicer.py` & `pynumaflow-0.7.1/pynumaflow/mapper/servicer/async_servicer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-import grpc
 from google.protobuf import empty_pb2 as _empty_pb2
 
 from pynumaflow.mapper._dtypes import Datum
 from pynumaflow.mapper._dtypes import MapAsyncHandlerCallable, MapSyncCallable
 from pynumaflow.proto.mapper import map_pb2, map_pb2_grpc
+from pynumaflow.shared.server import exit_on_error
 from pynumaflow.types import NumaflowServicerContext
 from pynumaflow._constants import _LOGGER
 
 
 class AsyncMapServicer(map_pb2_grpc.MapServicer):
     """
     This class is used to create a new grpc Async Map Servicer instance.
@@ -36,30 +36,32 @@
                 Datum(
                     keys=list(request.keys),
                     value=request.value,
                     event_time=request.event_time.ToDatetime(),
                     watermark=request.watermark.ToDatetime(),
                     headers=dict(request.headers),
                 ),
+                context,
             )
-        except Exception as e:
-            context.set_code(grpc.StatusCode.UNKNOWN)
-            context.set_details(str(e))
-            return map_pb2.MapResponse(results=[])
+        except BaseException as e:
+            _LOGGER.critical("UDFError, re-raising the error", exc_info=True)
+            exit_on_error(context, repr(e))
+            return
 
         return map_pb2.MapResponse(results=res)
 
-    async def __invoke_map(self, keys: list[str], req: Datum):
+    async def __invoke_map(self, keys: list[str], req: Datum, context: NumaflowServicerContext):
         """
         Invokes the user defined function.
         """
         try:
             msgs = await self.__map_handler(keys, req)
-        except Exception as err:
+        except BaseException as err:
             _LOGGER.critical("UDFError, re-raising the error", exc_info=True)
+            exit_on_error(context, repr(err))
             raise err
         datums = []
         for msg in msgs:
             datums.append(map_pb2.MapResponse.Result(keys=msg.keys, value=msg.value, tags=msg.tags))
 
         return datums
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/mapper/servicer/sync_servicer.py` & `pynumaflow-0.7.1/pynumaflow/mapper/servicer/sync_servicer.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,28 +9,27 @@
 class SyncMapServicer(map_pb2_grpc.MapServicer):
     """
     This class is used to create a new grpc Map Servicer instance.
     It implements the SyncMapServicer interface from the proto map.proto file.
     Provides the functionality for the required rpc methods.
     """
 
-    def __init__(
-        self,
-        handler: MapSyncCallable,
-    ):
+    def __init__(self, handler: MapSyncCallable, multiproc: bool = False):
         self.__map_handler: MapSyncCallable = handler
+        # This indicates whether the grpc server attached is multiproc or not
+        self.multiproc = multiproc
 
     def MapFn(
         self, request: map_pb2.MapRequest, context: NumaflowServicerContext
     ) -> map_pb2.MapResponse:
         """
         Applies a function to each datum element.
         The pascal case function name comes from the proto map_pb2_grpc.py file.
         """
-        return _map_fn_util(self.__map_handler, request, context)
+        return _map_fn_util(self.__map_handler, request, context, self.multiproc)
 
     def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> map_pb2.ReadyResponse:
         """
         IsReady is the heartbeat endpoint for gRPC.
         The pascal case function name comes from the proto map_pb2_grpc.py file.
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/mapper/sync_server.py` & `pynumaflow-0.7.1/pynumaflow/mapper/sync_server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/mapstreamer/_dtypes.py` & `pynumaflow-0.7.1/pynumaflow/mapstreamer/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/mapstreamer/async_server.py` & `pynumaflow-0.7.1/pynumaflow/mapstreamer/async_server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/mapstreamer/servicer/async_servicer.py` & `pynumaflow-0.7.1/pynumaflow/mapstreamer/servicer/async_servicer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from collections.abc import AsyncIterable
 
 from google.protobuf import empty_pb2 as _empty_pb2
 
 from pynumaflow.mapstreamer import Datum
 from pynumaflow.mapstreamer._dtypes import MapStreamCallable
 from pynumaflow.proto.mapstreamer import mapstream_pb2_grpc, mapstream_pb2
+from pynumaflow.shared.server import exit_on_error
 from pynumaflow.types import NumaflowServicerContext
 from pynumaflow._constants import _LOGGER
 
 
 class AsyncMapStreamServicer(mapstream_pb2_grpc.MapStreamServicer):
     """
     This class is used to create a new grpc Map Stream Servicer instance.
@@ -29,34 +30,43 @@
         context: NumaflowServicerContext,
     ) -> AsyncIterable[mapstream_pb2.MapStreamResponse]:
         """
         Applies a map function to a datum stream in streaming mode.
         The pascal case function name comes from the proto mapstream_pb2_grpc.py file.
         """
 
-        async for res in self.__invoke_map_stream(
-            list(request.keys),
-            Datum(
-                keys=list(request.keys),
-                value=request.value,
-                event_time=request.event_time.ToDatetime(),
-                watermark=request.watermark.ToDatetime(),
-                headers=dict(request.headers),
-            ),
-        ):
-            yield mapstream_pb2.MapStreamResponse(result=res)
+        try:
+            async for res in self.__invoke_map_stream(
+                list(request.keys),
+                Datum(
+                    keys=list(request.keys),
+                    value=request.value,
+                    event_time=request.event_time.ToDatetime(),
+                    watermark=request.watermark.ToDatetime(),
+                    headers=dict(request.headers),
+                ),
+                context,
+            ):
+                yield mapstream_pb2.MapStreamResponse(result=res)
+        except BaseException as err:
+            _LOGGER.critical("UDFError, re-raising the error", exc_info=True)
+            exit_on_error(context, repr(err))
+            return
 
-    async def __invoke_map_stream(self, keys: list[str], req: Datum):
+    async def __invoke_map_stream(
+        self, keys: list[str], req: Datum, context: NumaflowServicerContext
+    ):
         try:
             async for msg in self.__map_stream_handler(keys, req):
                 yield mapstream_pb2.MapStreamResponse.Result(
                     keys=msg.keys, value=msg.value, tags=msg.tags
                 )
-        except Exception as err:
+        except BaseException as err:
             _LOGGER.critical("UDFError, re-raising the error", exc_info=True)
+            exit_on_error(context, repr(err))
             raise err
 
     async def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> mapstream_pb2.ReadyResponse:
         """
         IsReady is the heartbeat endpoint for gRPC.
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/mapper/map.proto` & `pynumaflow-0.7.1/pynumaflow/proto/mapper/map.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/mapper/map_pb2.py` & `pynumaflow-0.7.1/pynumaflow/proto/mapper/map_pb2.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/mapper/map_pb2_grpc.py` & `pynumaflow-0.7.1/pynumaflow/proto/mapper/map_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/mapstreamer/mapstream.proto` & `pynumaflow-0.7.1/pynumaflow/proto/mapstreamer/mapstream.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/mapstreamer/mapstream_pb2.py` & `pynumaflow-0.7.1/pynumaflow/proto/mapstreamer/mapstream_pb2.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/mapstreamer/mapstream_pb2_grpc.py` & `pynumaflow-0.7.1/pynumaflow/proto/mapstreamer/mapstream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/reducer/reduce.proto` & `pynumaflow-0.7.1/pynumaflow/proto/reducer/reduce.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/reducer/reduce_pb2.py` & `pynumaflow-0.7.1/pynumaflow/proto/reducer/reduce_pb2.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/reducer/reduce_pb2_grpc.py` & `pynumaflow-0.7.1/pynumaflow/proto/reducer/reduce_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/sideinput/sideinput.proto` & `pynumaflow-0.7.1/pynumaflow/proto/sideinput/sideinput.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/sideinput/sideinput_pb2.py` & `pynumaflow-0.7.1/pynumaflow/proto/sideinput/sideinput_pb2.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/sideinput/sideinput_pb2_grpc.py` & `pynumaflow-0.7.1/pynumaflow/proto/sideinput/sideinput_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/sinker/sink.proto` & `pynumaflow-0.7.1/pynumaflow/proto/sinker/sink.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/sinker/sink_pb2.py` & `pynumaflow-0.7.1/pynumaflow/proto/sinker/sink_pb2.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/sinker/sink_pb2_grpc.py` & `pynumaflow-0.7.1/pynumaflow/proto/sinker/sink_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/sourcer/source.proto` & `pynumaflow-0.7.1/pynumaflow/proto/sourcer/source.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/sourcer/source_pb2.py` & `pynumaflow-0.7.1/pynumaflow/proto/sourcer/source_pb2.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/sourcer/source_pb2_grpc.py` & `pynumaflow-0.7.1/pynumaflow/proto/sourcer/source_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/sourcetransformer/transform.proto` & `pynumaflow-0.7.1/pynumaflow/proto/sourcetransformer/transform.proto`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/sourcetransformer/transform_pb2.py` & `pynumaflow-0.7.1/pynumaflow/proto/sourcetransformer/transform_pb2.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/proto/sourcetransformer/transform_pb2_grpc.py` & `pynumaflow-0.7.1/pynumaflow/proto/sourcetransformer/transform_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/reducer/_dtypes.py` & `pynumaflow-0.7.1/pynumaflow/reducer/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/reducer/async_server.py` & `pynumaflow-0.7.1/pynumaflow/reducer/async_server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/reducer/servicer/async_servicer.py` & `pynumaflow-0.7.1/pynumaflow/reducer/servicer/async_servicer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 from collections.abc import AsyncIterable
 from typing import Union
 
 import grpc
 from google.protobuf import empty_pb2 as _empty_pb2
 
 from pynumaflow._constants import _LOGGER
@@ -10,14 +11,15 @@
     Datum,
     ReduceAsyncCallable,
     _ReduceBuilderClass,
     ReduceRequest,
     WindowOperation,
 )
 from pynumaflow.reducer.servicer.task_manager import TaskManager
+from pynumaflow.shared.server import exit_on_error
 from pynumaflow.types import NumaflowServicerContext
 
 
 async def datum_generator(
     request_iterator: AsyncIterable[reduce_pb2.ReduceRequest],
 ) -> AsyncIterable[ReduceRequest]:
     """
@@ -82,62 +84,71 @@
         """
         # Create an async iterator from the request iterator
         datum_iterator = datum_generator(request_iterator=request_iterator)
 
         # Create a task manager instance
         # The task manager is used to manage lifecycle of the tasks
         # required for the reduce operation.
-        task_manager = TaskManager(handler=self.__reduce_handler)
+        task_manager = TaskManager(handler=self.__reduce_handler, context=context)
 
         # Start iterating through the request iterator and create tasks
         # based on the operation type received.
         try:
             async for request in datum_iterator:
                 # check whether the request is an open or append operation
                 if request.operation is int(WindowOperation.OPEN):
                     # create a new task for the open operation
                     # and inserts the request data into the task
                     await task_manager.create_task(request)
                 elif request.operation is int(WindowOperation.APPEND):
                     # append the task data to the existing task
                     # if the task does not exist, it will create a new task
                     await task_manager.append_task(request)
-        except Exception as e:
+        except BaseException as e:
             _LOGGER.critical("Reduce Error", exc_info=True)
-            context.set_code(grpc.StatusCode.UNKNOWN)
-            context.set_details(e.__str__())
-            raise e
+            # Send a context abort signal for the rpc, this is required for numa container to get
+            # the correct grpc error
+            await asyncio.gather(
+                context.abort(grpc.StatusCode.UNKNOWN, details=repr(e)), return_exceptions=True
+            )
+            exit_on_error(err=repr(e), parent=False, context=context, update_context=False)
 
         # send EOF to all the tasks once the request iterator is exhausted
         # This will signal the tasks to stop reading the data on their
         # respective iterators.
         await task_manager.stream_send_eof()
 
         # Get the list of tasks from the task manager
         res = task_manager.get_tasks()
         try:
             # iterate through the tasks and yield the response
             # from each of them once the task is completed.
             for task in res:
                 fut = task.future
                 await fut
+
                 # For each message in the task result, yield the response
-                for msg in fut.result():
-                    yield reduce_pb2.ReduceResponse(result=msg, window=task.window)
+                if fut.result():
+                    for msg in fut.result():
+                        yield reduce_pb2.ReduceResponse(result=msg, window=task.window)
 
             # For each window processed by the ReduceFn send an EOF response
             # We send one EOF per window
             current_window = task_manager.get_unique_windows()
             for window in current_window.values():
                 # yield the EOF response once the task is completed for a keyed window
                 yield reduce_pb2.ReduceResponse(window=window, EOF=True)
-        except Exception as e:
-            context.set_code(grpc.StatusCode.UNKNOWN)
-            context.set_details(e.__str__())
-            raise e
+        except BaseException as e:
+            _LOGGER.critical("Reduce Error", exc_info=True)
+            # Send a context abort signal for the rpc, this is required for numa container to get
+            # the correct grpc error
+            await asyncio.gather(
+                context.abort(grpc.StatusCode.UNKNOWN, details=repr(e)), return_exceptions=True
+            )
+            exit_on_error(err=repr(e), parent=False, context=context, update_context=False)
 
     async def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> reduce_pb2.ReadyResponse:
         """
         IsReady is the heartbeat endpoint for gRPC.
         The pascal case function name comes from the proto reduce_pb2_grpc.py file.
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/reducer/servicer/task_manager.py` & `pynumaflow-0.7.1/pynumaflow/reducer/servicer/task_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import asyncio
 from datetime import datetime, timezone
 from typing import Union
 from collections.abc import AsyncIterable
 
+import grpc
+
 from pynumaflow.exceptions import UDFError
 from pynumaflow.proto.reducer import reduce_pb2
 from pynumaflow.shared.asynciter import NonBlockingIterator
 from pynumaflow._constants import (
     STREAM_EOF,
     DELIMITER,
     _LOGGER,
@@ -16,14 +18,16 @@
     Metadata,
     ReduceResult,
     Datum,
     _ReduceBuilderClass,
     ReduceAsyncCallable,
     ReduceWindow,
 )
+from pynumaflow.shared.server import exit_on_error
+from pynumaflow.types import NumaflowServicerContext
 
 
 def build_unique_key_name(keys, window):
     """
     Builds a unique key name for the given keys and window.
     The key name is used to identify the Reduce task.
     The format is: start_time:end_time:key1:key2:...
@@ -42,23 +46,29 @@
 
 class TaskManager:
     """
     TaskManager is responsible for managing the Reduce tasks.
     It is created whenever a new reduce operation is requested.
     """
 
-    def __init__(self, handler: Union[ReduceAsyncCallable, _ReduceBuilderClass]):
+    def __init__(
+        self,
+        handler: Union[ReduceAsyncCallable, _ReduceBuilderClass],
+        context: NumaflowServicerContext,
+    ):
         # A dictionary to store the task information
         self.tasks = {}
         # Collection for storing strong references to all running tasks.
         # Event loop only keeps a weak reference, which can cause it to
         # get lost during execution.
         self.background_tasks = set()
         # Handler for the reduce operation
         self.__reduce_handler = handler
+        # Servicer context from grpc, required to abort if error occurs
+        self.context = context
 
     def get_tasks(self):
         """
         Returns the list of reduce tasks that are
         currently being processed
         """
         return self.tasks.values()
@@ -154,17 +164,24 @@
         # It is required for a new key to be processed by a
         # new instance of the reducer for a given window
         # Otherwise the function handler can be called directly
         if isinstance(self.__reduce_handler, _ReduceBuilderClass):
             new_instance = self.__reduce_handler.create()
         try:
             msgs = await new_instance(keys, request_iterator, md)
-        except Exception as err:
+        except BaseException as err:
             _LOGGER.critical("UDFError, re-raising the error", exc_info=True)
-            raise err
+            # Send a context abort signal for the rpc, this is required for numa container to get
+            # the correct grpc error
+            await asyncio.gather(
+                self.context.abort(grpc.StatusCode.UNKNOWN, details=repr(err)),
+                return_exceptions=True,
+            )
+            exit_on_error(err=repr(err), parent=False, context=self.context, update_context=False)
+            return
 
         datum_responses = []
         for msg in msgs:
             datum_responses.append(
                 reduce_pb2.ReduceResponse.Result(keys=msg.keys, value=msg.value, tags=msg.tags)
             )
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/reducestreamer/_dtypes.py` & `pynumaflow-0.7.1/pynumaflow/reducestreamer/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/reducestreamer/async_server.py` & `pynumaflow-0.7.1/pynumaflow/reducestreamer/async_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,12 +179,11 @@
         """
         # As the server is async, we need to create a new server instance in the
         # same thread as the event loop so that all the async calls are made in the
         # same context
         # Create a new async server instance and add the servicer to it
         server = grpc.aio.server()
         server.add_insecure_port(self.sock_path)
-        reduce_servicer = self.servicer
-        reduce_pb2_grpc.add_ReduceServicer_to_server(reduce_servicer, server)
+        reduce_pb2_grpc.add_ReduceServicer_to_server(self.servicer, server)
         await start_async_server(
             server, self.sock_path, self.max_threads, self._server_options, self.server_info_file
         )
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/reducestreamer/servicer/async_servicer.py` & `pynumaflow-0.7.1/pynumaflow/reducestreamer/servicer/async_servicer.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from pynumaflow.reducestreamer._dtypes import (
     Datum,
     ReduceStreamAsyncCallable,
     _ReduceStreamBuilderClass,
     ReduceRequest,
 )
 from pynumaflow.reducestreamer.servicer.task_manager import TaskManager
+from pynumaflow.shared.server import exit_on_error
 from pynumaflow.types import NumaflowServicerContext
 
 
 async def datum_generator(
     request_iterator: AsyncIterable[reduce_pb2.ReduceRequest],
 ) -> AsyncIterable[ReduceRequest]:
     """Generate a ReduceRequest from a ReduceRequest proto message."""
@@ -40,21 +41,20 @@
 
 def get_exception_traceback_str(exc) -> str:
     file = io.StringIO()
     traceback.print_exception(exc, value=exc, tb=exc.__traceback__, file=file)
     return file.getvalue().rstrip()
 
 
-async def handle_error(context: NumaflowServicerContext, e: Exception):
+def handle_error(context: NumaflowServicerContext, e: BaseException):
     trace = get_exception_traceback_str(e)
     _LOGGER.critical(trace)
     _LOGGER.critical(e.__str__())
     context.set_code(grpc.StatusCode.UNKNOWN)
     context.set_details(e.__str__())
-    return context
 
 
 class AsyncReduceStreamServicer(reduce_pb2_grpc.ReduceServicer):
     """
     This class is used to create a new grpc Reduce servicer instance.
     Provides the functionality for the required rpc methods.
     """
@@ -107,30 +107,45 @@
         #
         # 3. A reduce_pb2.ReduceResponse message with EOF=True
         # This is a special message that indicates the end of the processing for a window
         # When we get this message, we send an EOF message to the client
         try:
             async for msg in consumer:
                 # If the message is an exception, we raise the exception
-                if isinstance(msg, Exception):
-                    await handle_error(context, msg)
-                    raise msg
+                if isinstance(msg, BaseException):
+                    handle_error(context, msg)
+                    await asyncio.gather(
+                        context.abort(grpc.StatusCode.UNKNOWN, details=repr(msg)),
+                        return_exceptions=True,
+                    )
+                    exit_on_error(
+                        err=repr(msg), parent=False, context=context, update_context=False
+                    )
+                    return
                 # Send window EOF response or Window result response
                 # back to the client
                 else:
                     yield msg
-        except Exception as e:
-            await handle_error(context, e)
-            raise e
+        except BaseException as e:
+            handle_error(context, e)
+            await asyncio.gather(
+                context.abort(grpc.StatusCode.UNKNOWN, details=repr(e)), return_exceptions=True
+            )
+            exit_on_error(err=repr(e), parent=False, context=context, update_context=False)
+            return
         # Wait for the process_input_stream task to finish for a clean exit
         try:
             await producer
-        except Exception as e:
-            await handle_error(context)
-            raise e
+        except BaseException as e:
+            handle_error(context, e)
+            await asyncio.gather(
+                context.abort(grpc.StatusCode.UNKNOWN, details=repr(e)), return_exceptions=True
+            )
+            exit_on_error(err=repr(e), parent=False, context=context, update_context=False)
+            return
 
     async def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> reduce_pb2.ReadyResponse:
         """
         IsReady is the heartbeat endpoint for gRPC.
         The pascal case function name comes from the proto reduce_pb2_grpc.py file.
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/reducestreamer/servicer/task_manager.py` & `pynumaflow-0.7.1/pynumaflow/reducestreamer/servicer/task_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         # Otherwise the function handler can be called directly
         if isinstance(self.__reduce_handler, _ReduceStreamBuilderClass):
             new_instance = self.__reduce_handler.create()
         try:
             _ = await new_instance(keys, request_iterator, output, md)
         # If there is an error in the reduce operation, log and
         # then send the error to the result queue
-        except Exception as err:
+        except BaseException as err:
             _LOGGER.critical("UDFError, re-raising the error", exc_info=True)
             # Put the exception in the result queue
             await self.global_result_queue.put(err)
 
     async def process_input_stream(self, request_iterator: AsyncIterable[reduce_pb2.ReduceRequest]):
         # Start iterating through the request iterator and create tasks
         # based on the operation type received.
@@ -215,19 +215,20 @@
                     await self.create_task(request)
                 elif request.operation is int(WindowOperation.APPEND):
                     # append the task data to the existing task
                     # if the task does not exist, create a new task
                     await self.send_datum_to_task(request)
         # If there is an error in the reduce operation, log and
         # then send the error to the result queue
-        except Exception as e:
-            err_msg = "Reduce Streaming Error: %r" % e.__str__()
+        except BaseException as e:
+            err_msg = f"Reduce Streaming Error: {repr(e)}"
             _LOGGER.critical(err_msg, exc_info=True)
             # Put the exception in the global result queue
             await self.global_result_queue.put(e)
+            return
 
         try:
             # send EOF to all the tasks once the request iterator is exhausted
             # This will signal the tasks to stop reading the data on their
             # respective iterators.
             await self.stream_send_eof()
 
@@ -256,16 +257,16 @@
                 # Send an EOF message to the global result queue
                 # This will signal that window has been processed
                 eof_window_msg = create_window_eof_response(window=window)
                 await self.global_result_queue.put(eof_window_msg)
 
             # Once all tasks are completed, senf EOF the global result queue
             await self.global_result_queue.put(STREAM_EOF)
-        except Exception as e:
-            err_msg = "Reduce Streaming Error: %r" % e.__str__()
+        except BaseException as e:
+            err_msg = f"Reduce Streaming Error: {repr(e)}"
             _LOGGER.critical(err_msg, exc_info=True)
             await self.global_result_queue.put(e)
 
     async def write_to_global_queue(
         self, input_queue: NonBlockingIterator, output_queue: NonBlockingIterator, window
     ):
         """
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/shared/asynciter.py` & `pynumaflow-0.7.1/pynumaflow/shared/asynciter.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/shared/server.py` & `pynumaflow-0.7.1/pynumaflow/shared/server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import contextlib
 import multiprocessing
 import os
 import socket
 from abc import ABCMeta, abstractmethod
 from collections.abc import Iterator
 from concurrent.futures import ThreadPoolExecutor
+from typing import Optional
 
 import grpc
+import psutil
+
 from pynumaflow._constants import (
     _LOGGER,
     MULTIPROC_MAP_SOCK_ADDR,
     UDFType,
 )
 from pynumaflow.exceptions import SocketError
 from pynumaflow.info.server import get_sdk_version, write as info_server_write, get_metadata_env
@@ -22,14 +25,15 @@
     MINIMUM_NUMAFLOW_VERSION,
 )
 from pynumaflow.proto.mapper import map_pb2_grpc
 from pynumaflow.proto.sideinput import sideinput_pb2_grpc
 from pynumaflow.proto.sinker import sink_pb2_grpc
 from pynumaflow.proto.sourcer import source_pb2_grpc
 from pynumaflow.proto.sourcetransformer import transform_pb2_grpc
+from pynumaflow.types import NumaflowServicerContext
 
 
 class NumaflowServer(metaclass=ABCMeta):
     """
     Provides an interface to write a Numaflow Server
     which will be exposed over gRPC.
     """
@@ -88,16 +92,16 @@
 
 def _run_server(
     servicer,
     bind_address: str,
     threads_per_proc,
     server_options,
     udf_type: str,
-    server_info_file,
-    server_info,
+    server_info_file: Optional[str] = None,
+    server_info: Optional[ServerInfo] = None,
 ) -> None:
     """
     Starts the Synchronous server instance on the given UNIX socket
     with given max threads. Wait for the server to terminate.
     """
     server = grpc.server(
         ThreadPoolExecutor(
@@ -118,15 +122,17 @@
     elif udf_type == UDFType.SideInput:
         sideinput_pb2_grpc.add_SideInputServicer_to_server(servicer, server)
 
     # bind the server to the UDS/TCP socket
     server.add_insecure_port(bind_address)
     # start the gRPC server
     server.start()
-    info_server_write(server_info=server_info, info_file=server_info_file)
+    # Add the server information to the server info file if provided
+    if server_info and server_info_file:
+        info_server_write(server_info=server_info, info_file=server_info_file)
 
     _LOGGER.info("GRPC Server listening on: %s %d", bind_address, os.getpid())
     server.wait_for_termination()
 
 
 def start_multiproc_server(
     max_threads: int,
@@ -136,55 +142,50 @@
     server_options=None,
     udf_type: str = UDFType.Map,
 ):
     """
     Start N grpc servers in different processes where N = The number of CPUs or the
     value of the env var NUM_CPU_MULTIPROC defined by the user. The max value
     is set to 2 * CPU count.
-    Each server will be bound to a different port, and we will create equal number of
+    Each server will be bound to a different UDS socket, and we will create equal number of
     workers to handle each server.
     On the client side there will be same number of connections as the number of servers.
     """
 
     _LOGGER.info(
         "Starting new Multiproc server with num_procs: %s, num_threads per proc: %s",
         process_count,
         max_threads,
     )
     workers = []
-    server_ports = []
-    for _ in range(process_count):
-        # Find a port to bind to for each server, thus sending the port number = 0
-        # to the _reserve_port function so that kernel can find and return a free port
-        with _reserve_port(port_num=0) as port:
-            bind_address = f"{MULTIPROC_MAP_SOCK_ADDR}:{port}"
-            _LOGGER.info("Starting server on port: %s", port)
-            # NOTE: It is imperative that the worker subprocesses be forked before
-            # any gRPC servers start up. See
-            # https://github.com/grpc/grpc/issues/16001 for more details.
-            worker = multiprocessing.Process(
-                target=_run_server,
-                args=(servicer, bind_address, max_threads, server_options, udf_type),
-            )
-            worker.start()
-            workers.append(worker)
-            server_ports.append(port)
-
-    # Convert the available ports to a comma separated string
-    ports = ",".join(map(str, server_ports))
+    for idx in range(process_count):
+        # bind address is the UDS sock for each server to  bind to, it is in the format
+        # unix:///var/run/numaflow/multiproc#serv_num.sock
+        # -> unix:///var/run/numaflow/multiproc0.sock
+        bind_address = f"unix://{MULTIPROC_MAP_SOCK_ADDR}{idx}.sock"
+        _LOGGER.info("Starting server on: %s", bind_address)
+        # NOTE: It is imperative that the worker subprocesses be forked before
+        # any gRPC servers start up. See
+        # https://github.com/grpc/grpc/issues/16001 for more details.
+        worker = multiprocessing.Process(
+            target=_run_server,
+            args=(servicer, bind_address, max_threads, server_options, udf_type),
+        )
+        worker.start()
+        workers.append(worker)
 
     serv_info = ServerInfo(
-        protocol=Protocol.TCP,
+        protocol=Protocol.UDS,
         language=Language.PYTHON,
         minimum_numaflow_version=MINIMUM_NUMAFLOW_VERSION,
         version=get_sdk_version(),
         metadata=get_metadata_env(envs=METADATA_ENVS),
     )
-    # Add the PORTS metadata using the available ports
-    serv_info.metadata["SERV_PORTS"] = ports
+    # Add the MULTIPROC metadata using the number of servers to use
+    serv_info.metadata["MULTIPROC"] = str(process_count)
     info_server_write(server_info=serv_info, info_file=server_info_file)
 
     for worker in workers:
         worker.join()
 
 
 async def start_async_server(
@@ -208,15 +209,15 @@
         minimum_numaflow_version=MINIMUM_NUMAFLOW_VERSION,
         version=get_sdk_version(),
     )
     info_server_write(server_info=serv_info, info_file=server_info_file)
 
     # Log the server start
     _LOGGER.info(
-        "New Async GRPC Server listening on: %s with max threads: %s",
+        "Async GRPC Server listening on: %s with max threads: %s",
         sock_path,
         max_threads,
     )
 
     async def server_graceful_shutdown():
         """
         Shuts down the server with 5 seconds of grace period. During the
@@ -252,7 +253,34 @@
         if not isinstance(instance, callable_type):
             return False
         else:
             return True
     except Exception as e:
         _LOGGER.error(e)
         return False
+
+
+def exit_on_error(
+    context: NumaflowServicerContext, err: str, parent: bool = False, update_context=True
+):
+    """
+    Exit the current/parent process on an error.
+
+    Args:
+        context (NumaflowServicerContext): The gRPC context.
+        err (str): The error message.
+        parent (bool, optional): Whether this is the parent process.
+            Defaults to False.
+        update_context(bool, optional) : Is there a need to update
+            the context with the error codes
+    """
+    if update_context:
+        context.set_code(grpc.StatusCode.UNKNOWN)
+        context.set_details(err)
+
+    p = psutil.Process(os.getpid())
+    # If the parent flag is true, we exit from the parent process
+    # Use this for Multiproc right now to exit from the parent fork
+    if parent:
+        p = psutil.Process(os.getppid())
+    _LOGGER.info("Killing process: Got exception %s", err)
+    p.kill()
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sideinput/_dtypes.py` & `pynumaflow-0.7.1/pynumaflow/sideinput/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sideinput/server.py` & `pynumaflow-0.7.1/pynumaflow/sideinput/server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sideinput/servicer/servicer.py` & `pynumaflow-0.7.1/pynumaflow/sideinput/servicer/servicer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import grpc
 from google.protobuf import empty_pb2 as _empty_pb2
 
 from pynumaflow._constants import (
     _LOGGER,
 )
 from pynumaflow.proto.sideinput import sideinput_pb2_grpc, sideinput_pb2
+from pynumaflow.shared.server import exit_on_error
 from pynumaflow.sideinput._dtypes import RetrieverCallable
 from pynumaflow.types import NumaflowServicerContext
 
 
 class SideInputServicer(sideinput_pb2_grpc.SideInputServicer):
     def __init__(
         self,
@@ -22,20 +22,19 @@
         """
         Applies a sideinput function for a retrieval request.
         The pascal case function name comes from the proto sideinput_pb2_grpc.py file.
         """
         # if there is an exception, we will mark all the responses as a failure
         try:
             rspn = self.__retrieve_handler()
-        except Exception as err:
-            err_msg = "RetrieveSideInputErr: %r" % err
+        except BaseException as err:
+            err_msg = f"RetrieveSideInputErr: {repr(err)}"
             _LOGGER.critical(err_msg, exc_info=True)
-            context.set_code(grpc.StatusCode.UNKNOWN)
-            context.set_details(str(err))
-            return sideinput_pb2.SideInputResponse(value=None, no_broadcast=True)
+            exit_on_error(context, repr(err))
+            return
 
         return sideinput_pb2.SideInputResponse(value=rspn.value, no_broadcast=rspn.no_broadcast)
 
     def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> sideinput_pb2.ReadyResponse:
         """
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sinker/_dtypes.py` & `pynumaflow-0.7.1/pynumaflow/sinker/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sinker/async_server.py` & `pynumaflow-0.7.1/pynumaflow/sinker/async_server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sinker/server.py` & `pynumaflow-0.7.1/pynumaflow/sinker/server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sinker/servicer/async_servicer.py` & `pynumaflow-0.7.1/pynumaflow/sinker/servicer/sync_servicer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,78 +1,69 @@
-from collections.abc import AsyncIterable
+from collections.abc import Iterator, Iterable
 
 from google.protobuf import empty_pb2 as _empty_pb2
-
-from pynumaflow.sinker._dtypes import Responses, Datum, Response
+from pynumaflow._constants import _LOGGER
+from pynumaflow.shared.server import exit_on_error
+from pynumaflow.sinker._dtypes import Datum
 from pynumaflow.sinker._dtypes import SyncSinkCallable
 from pynumaflow.proto.sinker import sink_pb2_grpc, sink_pb2
 from pynumaflow.sinker.servicer.utils import build_sink_response
 from pynumaflow.types import NumaflowServicerContext
-from pynumaflow._constants import _LOGGER
 
 
-async def datum_generator(
-    request_iterator: AsyncIterable[sink_pb2.SinkRequest],
-) -> AsyncIterable[Datum]:
-    async for d in request_iterator:
+def datum_generator(request_iterator: Iterable[sink_pb2.SinkRequest]) -> Iterable[Datum]:
+    for d in request_iterator:
         datum = Datum(
             keys=list(d.keys),
             sink_msg_id=d.id,
             value=d.value,
             event_time=d.event_time.ToDatetime(),
             watermark=d.watermark.ToDatetime(),
             headers=dict(d.headers),
         )
         yield datum
 
 
-class AsyncSinkServicer(sink_pb2_grpc.SinkServicer):
+class SyncSinkServicer(sink_pb2_grpc.SinkServicer):
     """
     This class is used to create a new grpc Sink servicer instance.
     It implements the SinkServicer interface from the proto sink.proto file.
     Provides the functionality for the required rpc methods.
     """
 
     def __init__(
         self,
         handler: SyncSinkCallable,
     ):
         self.__sink_handler: SyncSinkCallable = handler
-        self.cleanup_coroutines = []
 
-    async def SinkFn(
-        self,
-        request_iterator: AsyncIterable[sink_pb2.SinkRequest],
-        context: NumaflowServicerContext,
+    def SinkFn(
+        self, request_iterator: Iterator[sink_pb2.SinkRequest], context: NumaflowServicerContext
     ) -> sink_pb2.SinkResponse:
         """
         Applies a sink function to a list of datum elements.
         The pascal case function name comes from the proto sink_pb2_grpc.py file.
         """
         # if there is an exception, we will mark all the responses as a failure
-        datum_iterator = datum_generator(request_iterator=request_iterator)
-        results = await self.__invoke_sink(datum_iterator)
-
-        return sink_pb2.SinkResponse(results=results)
-
-    async def __invoke_sink(self, datum_iterator: AsyncIterable[Datum]):
+        datum_iterator = datum_generator(request_iterator)
         try:
-            rspns = await self.__sink_handler(datum_iterator)
-        except Exception as err:
-            err_msg = "UDSinkError: %r" % err
+            rspns = self.__sink_handler(datum_iterator)
+        except BaseException as err:
+            err_msg = f"UDSinkError: {repr(err)}"
             _LOGGER.critical(err_msg, exc_info=True)
-            rspns = Responses()
-            async for _datum in datum_iterator:
-                rspns.append(Response.as_failure(_datum.id, err_msg))
+            exit_on_error(context, err_msg)
+            return
+
         responses = []
         for rspn in rspns:
             responses.append(build_sink_response(rspn))
-        return responses
 
-    async def IsReady(
+        return sink_pb2.SinkResponse(results=responses)
+
+    def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> sink_pb2.ReadyResponse:
         """
         IsReady is the heartbeat endpoint for gRPC.
         The pascal case function name comes from the proto sink_pb2_grpc.py file.
         """
         return sink_pb2.ReadyResponse(ready=True)
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sinker/servicer/sync_servicer.py` & `pynumaflow-0.7.1/pynumaflow/sinker/servicer/async_servicer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,86 @@
-from collections.abc import Iterator, Iterable
+from collections.abc import AsyncIterable
 
 from google.protobuf import empty_pb2 as _empty_pb2
-from pynumaflow._constants import _LOGGER
-from pynumaflow.sinker._dtypes import Responses, Datum, Response
+
+from pynumaflow.shared.server import exit_on_error
+from pynumaflow.sinker._dtypes import Datum
 from pynumaflow.sinker._dtypes import SyncSinkCallable
 from pynumaflow.proto.sinker import sink_pb2_grpc, sink_pb2
 from pynumaflow.sinker.servicer.utils import build_sink_response
 from pynumaflow.types import NumaflowServicerContext
+from pynumaflow._constants import _LOGGER
 
 
-def datum_generator(request_iterator: Iterable[sink_pb2.SinkRequest]) -> Iterable[Datum]:
-    for d in request_iterator:
+async def datum_generator(
+    request_iterator: AsyncIterable[sink_pb2.SinkRequest],
+) -> AsyncIterable[Datum]:
+    async for d in request_iterator:
         datum = Datum(
             keys=list(d.keys),
             sink_msg_id=d.id,
             value=d.value,
             event_time=d.event_time.ToDatetime(),
             watermark=d.watermark.ToDatetime(),
             headers=dict(d.headers),
         )
         yield datum
 
 
-class SyncSinkServicer(sink_pb2_grpc.SinkServicer):
+class AsyncSinkServicer(sink_pb2_grpc.SinkServicer):
     """
     This class is used to create a new grpc Sink servicer instance.
     It implements the SinkServicer interface from the proto sink.proto file.
     Provides the functionality for the required rpc methods.
     """
 
     def __init__(
         self,
         handler: SyncSinkCallable,
     ):
         self.__sink_handler: SyncSinkCallable = handler
+        self.cleanup_coroutines = []
 
-    def SinkFn(
-        self, request_iterator: Iterator[sink_pb2.SinkRequest], context: NumaflowServicerContext
+    async def SinkFn(
+        self,
+        request_iterator: AsyncIterable[sink_pb2.SinkRequest],
+        context: NumaflowServicerContext,
     ) -> sink_pb2.SinkResponse:
         """
         Applies a sink function to a list of datum elements.
         The pascal case function name comes from the proto sink_pb2_grpc.py file.
         """
         # if there is an exception, we will mark all the responses as a failure
-        datum_iterator = datum_generator(request_iterator)
+        datum_iterator = datum_generator(request_iterator=request_iterator)
         try:
-            rspns = self.__sink_handler(datum_iterator)
-        except Exception as err:
-            err_msg = "UDSinkError: %r" % err
+            results = await self.__invoke_sink(datum_iterator, context)
+        except BaseException as err:
+            err_msg = f"UDSinkError: {repr(err)}"
             _LOGGER.critical(err_msg, exc_info=True)
-            rspns = Responses()
-            for _datum in datum_iterator:
-                rspns.append(Response.as_failure(_datum.id, err_msg))
+            exit_on_error(context, err_msg)
+            return
+
+        return sink_pb2.SinkResponse(results=results)
 
+    async def __invoke_sink(
+        self, datum_iterator: AsyncIterable[Datum], context: NumaflowServicerContext
+    ):
+        try:
+            rspns = await self.__sink_handler(datum_iterator)
+        except BaseException as err:
+            err_msg = f"UDSinkError: {repr(err)}"
+            _LOGGER.critical(err_msg, exc_info=True)
+            exit_on_error(context, err_msg)
+            raise err
         responses = []
         for rspn in rspns:
             responses.append(build_sink_response(rspn))
+        return responses
 
-        return sink_pb2.SinkResponse(results=responses)
-
-    def IsReady(
+    async def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> sink_pb2.ReadyResponse:
         """
         IsReady is the heartbeat endpoint for gRPC.
         The pascal case function name comes from the proto sink_pb2_grpc.py file.
         """
         return sink_pb2.ReadyResponse(ready=True)
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sourcer/__init__.py` & `pynumaflow-0.7.1/pynumaflow/sourcer/__init__.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sourcer/_dtypes.py` & `pynumaflow-0.7.1/pynumaflow/sourcer/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sourcer/async_server.py` & `pynumaflow-0.7.1/pynumaflow/sourcer/async_server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sourcer/server.py` & `pynumaflow-0.7.1/pynumaflow/sourcer/server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sourcer/servicer/async_servicer.py` & `pynumaflow-0.7.1/pynumaflow/sourcer/servicer/async_servicer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from collections.abc import AsyncIterable
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
-import grpc
 from google.protobuf import empty_pb2 as _empty_pb2
 
+from pynumaflow.shared.server import exit_on_error
 from pynumaflow.sourcer._dtypes import ReadRequest
 from pynumaflow.sourcer._dtypes import Offset, AckRequest, SourceCallable
 from pynumaflow.proto.sourcer import source_pb2
 from pynumaflow.proto.sourcer import source_pb2_grpc
 from pynumaflow.types import NumaflowServicerContext
 from pynumaflow._constants import _LOGGER
 
@@ -31,67 +31,74 @@
         request: source_pb2.ReadRequest,
         context: NumaflowServicerContext,
     ) -> AsyncIterable[source_pb2.ReadResponse]:
         """
         Applies a Read function and returns a stream of datum responses.
         The pascal case function name comes from the proto source_pb2_grpc.py file.
         """
+        try:
+            async for res in self.__invoke_source_read_stream(
+                ReadRequest(
+                    num_records=request.request.num_records,
+                    timeout_in_ms=request.request.timeout_in_ms,
+                ),
+                context,
+            ):
+                yield source_pb2.ReadResponse(result=res)
+        except BaseException as err:
+            _LOGGER.critical("User-Defined Source ReadError ", exc_info=True)
+            exit_on_error(context, str(err))
+            return
 
-        async for res in self.__invoke_source_read_stream(
-            ReadRequest(
-                num_records=request.request.num_records,
-                timeout_in_ms=request.request.timeout_in_ms,
-            )
-        ):
-            yield source_pb2.ReadResponse(result=res)
-
-    async def __invoke_source_read_stream(self, req: ReadRequest):
+    async def __invoke_source_read_stream(self, req: ReadRequest, context: NumaflowServicerContext):
         try:
             async for msg in self.__source_read_handler(req):
                 event_time_timestamp = _timestamp_pb2.Timestamp()
                 event_time_timestamp.FromDatetime(dt=msg.event_time)
                 yield source_pb2.ReadResponse.Result(
                     payload=msg.payload,
                     keys=msg.keys,
                     offset=msg.offset.as_dict,
                     event_time=event_time_timestamp,
                     headers=msg.headers,
                 )
-        except Exception as err:
+        except BaseException as err:
             _LOGGER.critical("User-Defined Source ReadError ", exc_info=True)
+            exit_on_error(context, repr(err))
             raise err
 
     async def AckFn(
         self, request: source_pb2.AckRequest, context: NumaflowServicerContext
     ) -> source_pb2.AckResponse:
         """
         Applies an Ack function in User Defined Source
         """
         # proto repeated field(offsets) is of type google._upb._message.RepeatedScalarContainer
         # we need to explicitly convert it to list
         offsets = []
         for offset in request.request.offsets:
             offsets.append(Offset(offset.offset, offset.partition_id))
         try:
-            await self.__invoke_ack(ack_req=offsets)
-        except Exception as e:
-            context.set_code(grpc.StatusCode.UNKNOWN)
-            context.set_details(str(e))
-            raise e
+            await self.__invoke_ack(ack_req=offsets, context=context)
+        except BaseException as e:
+            _LOGGER.critical("AckFn Error", exc_info=True)
+            exit_on_error(context, repr(e))
+            return
 
         return source_pb2.AckResponse()
 
-    async def __invoke_ack(self, ack_req: list[Offset]):
+    async def __invoke_ack(self, ack_req: list[Offset], context: NumaflowServicerContext):
         """
         Invokes the Source Ack Function.
         """
         try:
             await self.__source_ack_handler(AckRequest(offsets=ack_req))
-        except Exception as err:
+        except BaseException as err:
             _LOGGER.critical("AckFn Error", exc_info=True)
+            exit_on_error(context, repr(err))
             raise err
         return source_pb2.AckResponse.Result()
 
     async def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> source_pb2.ReadyResponse:
         """
@@ -105,26 +112,28 @@
     ) -> source_pb2.PendingResponse:
         """
         PendingFn returns the number of pending records
         at the user defined source.
         """
         try:
             count = await self.__source_pending_handler()
-        except Exception as err:
+        except BaseException as err:
             _LOGGER.critical("PendingFn Error", exc_info=True)
-            raise err
+            exit_on_error(context, repr(err))
+            return
         resp = source_pb2.PendingResponse.Result(count=count.count)
         return source_pb2.PendingResponse(result=resp)
 
     async def PartitionsFn(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> source_pb2.PartitionsResponse:
         """
         PartitionsFn returns the partitions of the user defined source.
         """
         try:
             partitions = await self.__source_partitions_handler()
-        except Exception as err:
+        except BaseException as err:
             _LOGGER.critical("PartitionsFn Error", exc_info=True)
-            raise err
+            exit_on_error(context, repr(err))
+            return
         resp = source_pb2.PartitionsResponse.Result(partitions=partitions.partitions)
         return source_pb2.PartitionsResponse(result=resp)
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sourcer/servicer/sync_servicer.py` & `pynumaflow-0.7.1/pynumaflow/sourcer/servicer/sync_servicer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from collections.abc import Iterable
 
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
-import grpc
 from google.protobuf import empty_pb2 as _empty_pb2
 
+from pynumaflow.shared.server import exit_on_error
 from pynumaflow.sourcer._dtypes import ReadRequest
 from pynumaflow.sourcer._dtypes import (
     SourceReadCallable,
     Offset,
     AckRequest,
     SourceAckCallable,
     SourceCallable,
@@ -40,67 +40,74 @@
         request: source_pb2.ReadRequest,
         context: NumaflowServicerContext,
     ) -> Iterable[source_pb2.ReadResponse]:
         """
         Applies a Read function to a datum stream in streaming mode.
         The pascal case function name comes from the proto source_pb2_grpc.py file.
         """
+        try:
+            for res in self.__invoke_source_read_stream(
+                ReadRequest(
+                    num_records=request.request.num_records,
+                    timeout_in_ms=request.request.timeout_in_ms,
+                ),
+                context,
+            ):
+                yield source_pb2.ReadResponse(result=res)
+        except BaseException as err:
+            _LOGGER.critical("User-Defined Source ReadError ", exc_info=True)
+            exit_on_error(context, repr(err))
+            return
 
-        for res in self.__invoke_source_read_stream(
-            ReadRequest(
-                num_records=request.request.num_records,
-                timeout_in_ms=request.request.timeout_in_ms,
-            )
-        ):
-            yield source_pb2.ReadResponse(result=res)
-
-    def __invoke_source_read_stream(self, req: ReadRequest):
+    def __invoke_source_read_stream(self, req: ReadRequest, context: NumaflowServicerContext):
         try:
             for msg in self.__source_read_handler(req):
                 event_time_timestamp = _timestamp_pb2.Timestamp()
                 event_time_timestamp.FromDatetime(dt=msg.event_time)
                 yield source_pb2.ReadResponse.Result(
                     payload=msg.payload,
                     keys=msg.keys,
                     offset=msg.offset.as_dict,
                     event_time=event_time_timestamp,
                     headers=dict(msg.headers),
                 )
-        except Exception as err:
+        except BaseException as err:
             _LOGGER.critical("User-Defined Source ReadError ", exc_info=True)
+            exit_on_error(context, repr(err))
             raise err
 
     def AckFn(
         self, request: source_pb2.AckRequest, context: NumaflowServicerContext
     ) -> source_pb2.AckResponse:
         """
         Applies an Ack function in User Defined Source
         """
         # proto repeated field(offsets) is of type google._upb._message.RepeatedScalarContainer
         # we need to explicitly convert it to list
         offsets = []
         for offset in request.request.offsets:
             offsets.append(Offset(offset.offset, offset.partition_id))
         try:
-            self.__invoke_ack(ack_req=offsets)
-        except Exception as e:
-            context.set_code(grpc.StatusCode.UNKNOWN)
-            context.set_details(str(e))
-            raise e
+            self.__invoke_ack(ack_req=offsets, context=context)
+        except BaseException as e:
+            _LOGGER.critical("User-Defined Source AckError ", exc_info=True)
+            exit_on_error(context, repr(e))
+            return
 
         return source_pb2.AckResponse()
 
-    def __invoke_ack(self, ack_req: list[Offset]):
+    def __invoke_ack(self, ack_req: list[Offset], context: NumaflowServicerContext):
         """
         Invokes the Source Ack Function.
         """
         try:
             self.__source_ack_handler(AckRequest(offsets=ack_req))
-        except Exception as err:
+        except BaseException as err:
             _LOGGER.critical("AckFn Error", exc_info=True)
+            exit_on_error(context, repr(err))
             raise err
         return source_pb2.AckResponse.Result()
 
     def IsReady(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> source_pb2.ReadyResponse:
         """
@@ -114,17 +121,18 @@
     ) -> source_pb2.PendingResponse:
         """
         PendingFn returns the number of pending records
         at the user defined source.
         """
         try:
             count = self.__source_pending_handler()
-        except Exception as err:
+        except BaseException as err:
             _LOGGER.critical("PendingFn error", exc_info=True)
-            raise err
+            exit_on_error(context, repr(err))
+            return
         resp = source_pb2.PendingResponse.Result(count=count.count)
         return source_pb2.PendingResponse(result=resp)
 
     def PartitionsFn(
         self, request: _empty_pb2.Empty, context: NumaflowServicerContext
     ) -> source_pb2.PartitionsResponse:
         """
@@ -133,12 +141,13 @@
         If the source doesn't have partitions, get_default_partitions() can be used to
         return the default partitions. In most cases, the get_default_partitions()
         should be enough; the cases where we need to implement custom partitions_handler()
         is in a case like Kafka, where a reader can read from multiple Kafka partitions.
         """
         try:
             partitions = self.__source_partitions_handler()
-        except Exception as err:
+        except BaseException as err:
             _LOGGER.critical("PartitionFn error", exc_info=True)
-            raise err
+            exit_on_error(context, repr(err))
+            return
         resp = source_pb2.PartitionsResponse.Result(partitions=partitions.partitions)
         return source_pb2.PartitionsResponse(result=resp)
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/_dtypes.py` & `pynumaflow-0.7.1/pynumaflow/sourcetransformer/_dtypes.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/multiproc_server.py` & `pynumaflow-0.7.1/pynumaflow/sourcetransformer/multiproc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             ("grpc.so_reuseaddr", 1),
         ]
         # Set the number of processes to be spawned to the number of CPUs or
         # the value of the env var NUM_CPU_MULTIPROC defined by the user
         # Setting the max value to 2 * CPU count
         # Used for multiproc server
         self._process_count = min(server_count, 2 * _PROCESS_COUNT)
-        self.servicer = SourceTransformServicer(handler=source_transform_instance)
+        self.servicer = SourceTransformServicer(handler=source_transform_instance, multiproc=True)
 
     def start(self):
         """
         Starts the Multiproc gRPC server on the given TCP sockets
         with given max threads.
         """
         start_multiproc_server(
```

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/server.py` & `pynumaflow-0.7.1/pynumaflow/sourcetransformer/server.py`

 * *Files identical despite different names*

### Comparing `pynumaflow-0.7.0a1/pynumaflow/sourcetransformer/servicer/server.py` & `pynumaflow-0.7.1/pynumaflow/sourcetransformer/servicer/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import grpc
 from google.protobuf import empty_pb2 as _empty_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 
+from pynumaflow.shared.server import exit_on_error
 from pynumaflow.sourcetransformer import Datum
 from pynumaflow.sourcetransformer._dtypes import SourceTransformCallable
 from pynumaflow.proto.sourcetransformer import transform_pb2
 from pynumaflow.proto.sourcetransformer import transform_pb2_grpc
 from pynumaflow.types import NumaflowServicerContext
 from pynumaflow._constants import _LOGGER
 
@@ -13,19 +13,18 @@
 class SourceTransformServicer(transform_pb2_grpc.SourceTransformServicer):
     """
     This class is used to create a new grpc SourceTransform servicer instance.
     It implements the SourceTransformServicer interface from the proto transform.proto file.
     Provides the functionality for the required rpc methods.
     """
 
-    def __init__(
-        self,
-        handler: SourceTransformCallable,
-    ):
+    def __init__(self, handler: SourceTransformCallable, multiproc: bool = False):
         self.__transform_handler: SourceTransformCallable = handler
+        # This indicates whether the grpc server attached is multiproc or not
+        self.multiproc = multiproc
 
     def SourceTransformFn(
         self, request: transform_pb2.SourceTransformRequest, context: NumaflowServicerContext
     ) -> transform_pb2.SourceTransformResponse:
         """
         Applies a function to each datum element.
         The pascal case function name comes from the generated transform_pb2_grpc.py file.
@@ -40,19 +39,19 @@
                     keys=list(request.keys),
                     value=request.value,
                     event_time=request.event_time.ToDatetime(),
                     watermark=request.watermark.ToDatetime(),
                     headers=dict(request.headers),
                 ),
             )
-        except Exception as err:
+        except BaseException as err:
             _LOGGER.critical("UDFError, re-raising the error", exc_info=True)
-            context.set_code(grpc.StatusCode.UNKNOWN)
-            context.set_details(str(err))
-            return transform_pb2.SourceTransformResponse(results=[])
+            # Terminate the current server process due to exception
+            exit_on_error(context, repr(err), parent=self.multiproc)
+            return
 
         datums = []
         for msgt in msgts:
             event_time_timestamp = _timestamp_pb2.Timestamp()
             event_time_timestamp.FromDatetime(dt=msgt.event_time)
             datums.append(
                 transform_pb2.SourceTransformResponse.Result(
```

### Comparing `pynumaflow-0.7.0a1/pyproject.toml` & `pynumaflow-0.7.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 [tool.poetry]
 name = "pynumaflow"
-version = "0.7.0a1"
+version = "0.7.1"
 description = "Provides the interfaces of writing Python User Defined Functions and Sinks for NumaFlow."
 authors = ["NumaFlow Developers"]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Vigith Maurice <vigith@gmail.com>",
 ]
 classifiers = [
     "Topic :: Software Development :: Libraries",
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11"
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12"
 ]
 repository = "https://github.com/numaproj/numaflow-python"
 
 [tool.poetry.dependencies]
-python = ">=3.9, <3.12"
+python = ">=3.9, <3.13"
 grpcio = "^1.48.1"
 grpcio-tools = "^1.48.1"
 google-cloud = "^0.34.0"
 google-api-core = "^2.11.0"
 protobuf = ">=3.20,<5.0"
 aiorun = "^2023.7"
 uvloop = "^0.19.0"
+psutil = "^5.9.8"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^3.0"
```

### Comparing `pynumaflow-0.7.0a1/PKG-INFO` & `pynumaflow-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: pynumaflow
-Version: 0.7.0a1
+Version: 0.7.1
 Summary: Provides the interfaces of writing Python User Defined Functions and Sinks for NumaFlow.
 Home-page: https://github.com/numaproj/numaflow-python
 License: Apache-2.0
 Author: NumaFlow Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: aiorun (>=2023.7,<2024.0)
 Requires-Dist: google-api-core (>=2.11.0,<3.0.0)
 Requires-Dist: google-cloud (>=0.34.0,<0.35.0)
 Requires-Dist: grpcio (>=1.48.1,<2.0.0)
 Requires-Dist: grpcio-tools (>=1.48.1,<2.0.0)
 Requires-Dist: protobuf (>=3.20,<5.0)
+Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: uvloop (>=0.19.0,<0.20.0)
 Project-URL: Repository, https://github.com/numaproj/numaflow-python
 Description-Content-Type: text/markdown
 
 # Python SDK for Numaflow
 
 [![Build](https://github.com/numaproj/numaflow-python/actions/workflows/run-tests.yml/badge.svg)](https://github.com/numaproj/numaflow-python/actions/workflows/run-tests.yml)
```

