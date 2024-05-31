# Comparing `tmp/google_jetstream-0.2.1.tar.gz` & `tmp/google_jetstream-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_jetstream-0.2.1.tar", last modified: Fri May  3 21:42:43 2024, max compression
+gzip compressed data, was "google_jetstream-0.2.2.tar", last modified: Fri May 31 18:44:57 2024, max compression
```

## Comparing `google_jetstream-0.2.1.tar` & `google_jetstream-0.2.2.tar`

### file list

```diff
@@ -1,61 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.068576 google_jetstream-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/google_jetstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-05-03 21:42:43.000000 google_jetstream-0.2.1/google_jetstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-03 21:42:43.000000 google_jetstream-0.2.1/google_jetstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 21:42:43.000000 google_jetstream-0.2.1/google_jetstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-03 21:42:43.000000 google_jetstream-0.2.1/google_jetstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-03 21:42:43.000000 google_jetstream-0.2.1/google_jetstream.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.060576 google_jetstream-0.2.1/jetstream/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.060576 google_jetstream-0.2.1/jetstream/core/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/config_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.060576 google_jetstream-0.2.1/jetstream/core/implementations/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/implementations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/core/implementations/mock/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/implementations/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/implementations/mock/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/implementations/mock/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    28701 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/core/proto/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/proto/jetstream_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/proto/jetstream_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/server_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/core/utils/async_multifuture.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/engine/
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/engine_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/mock_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/mock_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12697 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/token_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/tokenizer_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/tokenizer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/engine/tokenizer_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/core/test_config_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/core/test_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/core/test_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/tests/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4613 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/engine/test_mock_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/engine/test_token_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/tests/engine/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/third_party/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/third_party/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:43.064576 google_jetstream-0.2.1/jetstream/third_party/llama3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/third_party/llama3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7279 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/jetstream/third_party/llama3/llama3_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 21:42:43.068576 google_jetstream-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-03 21:42:40.000000 google_jetstream-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.343954 google_jetstream-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-31 18:44:57.343954 google_jetstream-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.339954 google_jetstream-0.2.2/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24291 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/benchmarks/benchmark_serving.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/benchmarks/eval_accuracy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.343954 google_jetstream-0.2.2/google_jetstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-05-31 18:44:57.000000 google_jetstream-0.2.2/google_jetstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-31 18:44:57.000000 google_jetstream-0.2.2/google_jetstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:44:57.000000 google_jetstream-0.2.2/google_jetstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-31 18:44:57.000000 google_jetstream-0.2.2/google_jetstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-31 18:44:57.000000 google_jetstream-0.2.2/google_jetstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.339954 google_jetstream-0.2.2/jetstream/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.339954 google_jetstream-0.2.2/jetstream/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/config_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.339954 google_jetstream-0.2.2/jetstream/core/implementations/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/implementations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.339954 google_jetstream-0.2.2/jetstream/core/implementations/mock/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/implementations/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/implementations/mock/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/implementations/mock/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.339954 google_jetstream-0.2.2/jetstream/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/metrics/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34730 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.339954 google_jetstream-0.2.2/jetstream/core/proto/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4157 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/proto/jetstream_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/proto/jetstream_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/server_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.343954 google_jetstream-0.2.2/jetstream/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/utils/async_multifuture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/core/utils/return_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.343954 google_jetstream-0.2.2/jetstream/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7473 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/engine/engine_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/engine/mock_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/engine/mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12609 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/engine/token_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/engine/tokenizer_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/engine/tokenizer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/engine/tokenizer_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.343954 google_jetstream-0.2.2/jetstream/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.343954 google_jetstream-0.2.2/jetstream/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/tests/core/test_config_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/tests/core/test_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4998 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/tests/core/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.343954 google_jetstream-0.2.2/jetstream/tests/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/tests/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/tests/engine/test_mock_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20732 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/tests/engine/test_token_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/tests/engine/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.343954 google_jetstream-0.2.2/jetstream/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/third_party/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:57.343954 google_jetstream-0.2.2/jetstream/third_party/llama3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/third_party/llama3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7295 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/jetstream/third_party/llama3/llama3_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:44:57.343954 google_jetstream-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-31 18:44:54.000000 google_jetstream-0.2.2/setup.py
```

### Comparing `google_jetstream-0.2.1/LICENSE` & `google_jetstream-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/PKG-INFO` & `google_jetstream-0.2.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-jetstream
-Version: 0.2.1
+Version: 0.2.2
 Summary: JetStream is a throughput and memory optimized engine for LLM inference on XLA devices, starting with TPUs (and GPUs in future -- PRs welcome).
 Home-page: https://github.com/google/JetStream
 Author: Google LLC
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -15,20 +15,23 @@
 Requires-Dist: coverage
 Requires-Dist: flax
 Requires-Dist: grpcio
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: numpy
 Requires-Dist: portpicker
+Requires-Dist: prometheus-client
 Requires-Dist: pytest
 Requires-Dist: seqio
 Requires-Dist: tiktoken
 Requires-Dist: blobfile
+Requires-Dist: parameterized
+Requires-Dist: shortuuid
 
-[![Unit Tests](https://github.com/google/JetStream/actions/workflows/unit_tests.yaml/badge.svg)](https://github.com/google/JetStream/actions/workflows/unit_tests.yaml)
+[![Unit Tests](https://github.com/google/JetStream/actions/workflows/unit_tests.yaml/badge.svg?branch=main)](https://github.com/google/JetStream/actions/workflows/unit_tests.yaml?query=branch:main)
 [![PyPI version](https://badge.fury.io/py/google-jetstream.svg)](https://badge.fury.io/py/google-jetstream)
 [![PyPi downloads](https://img.shields.io/pypi/dm/google-jetstream?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/google-jetstream/)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
 
 # JetStream is a throughput and memory optimized engine for LLM inference on XLA devices.
 
 ## About
@@ -46,17 +49,19 @@
 
 ### Pytorch
 
 - Git: https://github.com/google/jetstream-pytorch 
 - README: https://github.com/google/jetstream-pytorch/blob/main/README.md 
 
 ## Documentation
-- [Online Inference with MaxText on v5e Cloud TPU VM](https://cloud.google.com/tpu/docs/tutorials/LLM/jetstream) [[README](#jetstream-maxtext-inference-on-v5e-cloud-tpu-vm-user-guide)]
+- [Online Inference with MaxText on v5e Cloud TPU VM](https://cloud.google.com/tpu/docs/tutorials/LLM/jetstream) [[README](https://github.com/google/JetStream/blob/main/docs/online-inference-with-maxtext-engine.md)]
 - [Online Inference with Pytorch on v5e Cloud TPU VM](https://cloud.google.com/tpu/docs/tutorials/LLM/jetstream-pytorch) [[README](https://github.com/google/jetstream-pytorch/tree/main?tab=readme-ov-file#jetstream-pytorch)]
 - [Serve Gemma using TPUs on GKE with JetStream](https://cloud.google.com/kubernetes-engine/docs/tutorials/serve-gemma-tpu-jetstream)
+- [Observability in JetStream Server](https://github.com/google/JetStream/blob/main/docs/observability-prometheus-metrics-in-jetstream-server.md)
+- [Profiling in JetStream Server](https://github.com/google/JetStream/blob/main/docs/profiling-with-jax-profiler-and-tensorboard.md)
 - [JetStream Standalone Local Setup](#jetstream-standalone-local-setup)
 
 
 # JetStream Standalone Local Setup
 
 ## Getting Started
 
@@ -79,19 +84,20 @@
 python -m jetstream.tools.load_tester
 
 ```
 
 ### Test core modules
 ```
 # Test JetStream core orchestrator
-python -m jetstream.tests.core.test_orchestrator
+python -m unittest -v jetstream.tests.core.test_orchestrator
 
 # Test JetStream core server library
-python -m jetstream.tests.core.test_server
+python -m unittest -v jetstream.tests.core.test_server
 
 # Test mock JetStream engine implementation
-python -m jetstream.tests.engine.test_mock_engine
+python -m unittest -v jetstream.tests.engine.test_mock_engine
 
 # Test mock JetStream token utils
-python -m jetstream.tests.engine.test_utils
+python -m unittest -v jetstream.tests.engine.test_token_utils
+python -m unittest -v jetstream.tests.engine.test_utils
 
 ```
```

### Comparing `google_jetstream-0.2.1/README.md` & `google_jetstream-0.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Unit Tests](https://github.com/google/JetStream/actions/workflows/unit_tests.yaml/badge.svg)](https://github.com/google/JetStream/actions/workflows/unit_tests.yaml)
+[![Unit Tests](https://github.com/google/JetStream/actions/workflows/unit_tests.yaml/badge.svg?branch=main)](https://github.com/google/JetStream/actions/workflows/unit_tests.yaml?query=branch:main)
 [![PyPI version](https://badge.fury.io/py/google-jetstream.svg)](https://badge.fury.io/py/google-jetstream)
 [![PyPi downloads](https://img.shields.io/pypi/dm/google-jetstream?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/google-jetstream/)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
 
 # JetStream is a throughput and memory optimized engine for LLM inference on XLA devices.
 
 ## About
@@ -20,17 +20,19 @@
 
 ### Pytorch
 
 - Git: https://github.com/google/jetstream-pytorch 
 - README: https://github.com/google/jetstream-pytorch/blob/main/README.md 
 
 ## Documentation
-- [Online Inference with MaxText on v5e Cloud TPU VM](https://cloud.google.com/tpu/docs/tutorials/LLM/jetstream) [[README](#jetstream-maxtext-inference-on-v5e-cloud-tpu-vm-user-guide)]
+- [Online Inference with MaxText on v5e Cloud TPU VM](https://cloud.google.com/tpu/docs/tutorials/LLM/jetstream) [[README](https://github.com/google/JetStream/blob/main/docs/online-inference-with-maxtext-engine.md)]
 - [Online Inference with Pytorch on v5e Cloud TPU VM](https://cloud.google.com/tpu/docs/tutorials/LLM/jetstream-pytorch) [[README](https://github.com/google/jetstream-pytorch/tree/main?tab=readme-ov-file#jetstream-pytorch)]
 - [Serve Gemma using TPUs on GKE with JetStream](https://cloud.google.com/kubernetes-engine/docs/tutorials/serve-gemma-tpu-jetstream)
+- [Observability in JetStream Server](https://github.com/google/JetStream/blob/main/docs/observability-prometheus-metrics-in-jetstream-server.md)
+- [Profiling in JetStream Server](https://github.com/google/JetStream/blob/main/docs/profiling-with-jax-profiler-and-tensorboard.md)
 - [JetStream Standalone Local Setup](#jetstream-standalone-local-setup)
 
 
 # JetStream Standalone Local Setup
 
 ## Getting Started
 
@@ -53,19 +55,20 @@
 python -m jetstream.tools.load_tester
 
 ```
 
 ### Test core modules
 ```
 # Test JetStream core orchestrator
-python -m jetstream.tests.core.test_orchestrator
+python -m unittest -v jetstream.tests.core.test_orchestrator
 
 # Test JetStream core server library
-python -m jetstream.tests.core.test_server
+python -m unittest -v jetstream.tests.core.test_server
 
 # Test mock JetStream engine implementation
-python -m jetstream.tests.engine.test_mock_engine
+python -m unittest -v jetstream.tests.engine.test_mock_engine
 
 # Test mock JetStream token utils
-python -m jetstream.tests.engine.test_utils
+python -m unittest -v jetstream.tests.engine.test_token_utils
+python -m unittest -v jetstream.tests.engine.test_utils
 
 ```
```

### Comparing `google_jetstream-0.2.1/google_jetstream.egg-info/PKG-INFO` & `google_jetstream-0.2.2/google_jetstream.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-jetstream
-Version: 0.2.1
+Version: 0.2.2
 Summary: JetStream is a throughput and memory optimized engine for LLM inference on XLA devices, starting with TPUs (and GPUs in future -- PRs welcome).
 Home-page: https://github.com/google/JetStream
 Author: Google LLC
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -15,20 +15,23 @@
 Requires-Dist: coverage
 Requires-Dist: flax
 Requires-Dist: grpcio
 Requires-Dist: jax
 Requires-Dist: jaxlib
 Requires-Dist: numpy
 Requires-Dist: portpicker
+Requires-Dist: prometheus-client
 Requires-Dist: pytest
 Requires-Dist: seqio
 Requires-Dist: tiktoken
 Requires-Dist: blobfile
+Requires-Dist: parameterized
+Requires-Dist: shortuuid
 
-[![Unit Tests](https://github.com/google/JetStream/actions/workflows/unit_tests.yaml/badge.svg)](https://github.com/google/JetStream/actions/workflows/unit_tests.yaml)
+[![Unit Tests](https://github.com/google/JetStream/actions/workflows/unit_tests.yaml/badge.svg?branch=main)](https://github.com/google/JetStream/actions/workflows/unit_tests.yaml?query=branch:main)
 [![PyPI version](https://badge.fury.io/py/google-jetstream.svg)](https://badge.fury.io/py/google-jetstream)
 [![PyPi downloads](https://img.shields.io/pypi/dm/google-jetstream?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/google-jetstream/)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
 
 # JetStream is a throughput and memory optimized engine for LLM inference on XLA devices.
 
 ## About
@@ -46,17 +49,19 @@
 
 ### Pytorch
 
 - Git: https://github.com/google/jetstream-pytorch 
 - README: https://github.com/google/jetstream-pytorch/blob/main/README.md 
 
 ## Documentation
-- [Online Inference with MaxText on v5e Cloud TPU VM](https://cloud.google.com/tpu/docs/tutorials/LLM/jetstream) [[README](#jetstream-maxtext-inference-on-v5e-cloud-tpu-vm-user-guide)]
+- [Online Inference with MaxText on v5e Cloud TPU VM](https://cloud.google.com/tpu/docs/tutorials/LLM/jetstream) [[README](https://github.com/google/JetStream/blob/main/docs/online-inference-with-maxtext-engine.md)]
 - [Online Inference with Pytorch on v5e Cloud TPU VM](https://cloud.google.com/tpu/docs/tutorials/LLM/jetstream-pytorch) [[README](https://github.com/google/jetstream-pytorch/tree/main?tab=readme-ov-file#jetstream-pytorch)]
 - [Serve Gemma using TPUs on GKE with JetStream](https://cloud.google.com/kubernetes-engine/docs/tutorials/serve-gemma-tpu-jetstream)
+- [Observability in JetStream Server](https://github.com/google/JetStream/blob/main/docs/observability-prometheus-metrics-in-jetstream-server.md)
+- [Profiling in JetStream Server](https://github.com/google/JetStream/blob/main/docs/profiling-with-jax-profiler-and-tensorboard.md)
 - [JetStream Standalone Local Setup](#jetstream-standalone-local-setup)
 
 
 # JetStream Standalone Local Setup
 
 ## Getting Started
 
@@ -79,19 +84,20 @@
 python -m jetstream.tools.load_tester
 
 ```
 
 ### Test core modules
 ```
 # Test JetStream core orchestrator
-python -m jetstream.tests.core.test_orchestrator
+python -m unittest -v jetstream.tests.core.test_orchestrator
 
 # Test JetStream core server library
-python -m jetstream.tests.core.test_server
+python -m unittest -v jetstream.tests.core.test_server
 
 # Test mock JetStream engine implementation
-python -m jetstream.tests.engine.test_mock_engine
+python -m unittest -v jetstream.tests.engine.test_mock_engine
 
 # Test mock JetStream token utils
-python -m jetstream.tests.engine.test_utils
+python -m unittest -v jetstream.tests.engine.test_token_utils
+python -m unittest -v jetstream.tests.engine.test_utils
 
 ```
```

### Comparing `google_jetstream-0.2.1/google_jetstream.egg-info/SOURCES.txt` & `google_jetstream-0.2.2/google_jetstream.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 AUTHORS
 LICENSE
 MANIFEST.in
 README.md
 requirements.in
 setup.py
+benchmarks/__init__.py
+benchmarks/benchmark_serving.py
+benchmarks/eval_accuracy.py
 google_jetstream.egg-info/PKG-INFO
 google_jetstream.egg-info/SOURCES.txt
 google_jetstream.egg-info/dependency_links.txt
 google_jetstream.egg-info/requires.txt
 google_jetstream.egg-info/top_level.txt
 jetstream/__init__.py
 jetstream/core/__init__.py
 jetstream/core/config_lib.py
 jetstream/core/orchestrator.py
 jetstream/core/server_lib.py
 jetstream/core/implementations/__init__.py
 jetstream/core/implementations/mock/__init__.py
 jetstream/core/implementations/mock/config.py
 jetstream/core/implementations/mock/server.py
+jetstream/core/metrics/__init__.py
+jetstream/core/metrics/prometheus.py
 jetstream/core/proto/__init__.py
 jetstream/core/proto/jetstream_pb2.py
 jetstream/core/proto/jetstream_pb2_grpc.py
 jetstream/core/utils/__init__.py
 jetstream/core/utils/async_multifuture.py
+jetstream/core/utils/return_sample.py
 jetstream/engine/__init__.py
 jetstream/engine/engine_api.py
 jetstream/engine/mock_engine.py
 jetstream/engine/mock_utils.py
 jetstream/engine/token_utils.py
 jetstream/engine/tokenizer_api.py
 jetstream/engine/tokenizer_pb2.py
```

### Comparing `google_jetstream-0.2.1/jetstream/__init__.py` & `google_jetstream-0.2.2/jetstream/__init__.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/core/__init__.py` & `google_jetstream-0.2.2/jetstream/core/__init__.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/core/config_lib.py` & `google_jetstream-0.2.2/jetstream/core/config_lib.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 
 """Configs of engines for the orchestrator to load."""
 
 import dataclasses
 import functools
 from typing import Any, Callable, List, Tuple, Type
+from numpy import uint16
 
 from jetstream.engine import engine_api
 from jetstream.engine import mock_engine
 
 
 Devices = Any
 
@@ -33,29 +34,29 @@
 
   prefill_slices: Tuple[str, ...] = ()
   generate_slices: Tuple[str, ...] = ()
   interleaved_slices: Tuple[str, ...] = ()
   prefill_engine_create_fns: Tuple[CreateEngineFn, ...] = ()
   generate_engine_create_fns: Tuple[CreateEngineFn, ...] = ()
   interleaved_engine_create_fns: Tuple[CreateEngineFn, ...] = ()
-
-  def get_slices_to_launch(self: "ServerConfig") -> str:
-    """Used when launching this config via xm config."""
-    return ",".join(
-        self.prefill_slices + self.generate_slices + self.interleaved_slices
-    )
+  is_ray_backend: bool = False
 
 
 @dataclasses.dataclass
 class InstantiatedEngines:
   prefill_engines: List[engine_api.Engine]
   generate_engines: List[engine_api.Engine]
   interleaved_engines: List[engine_api.Engine]
 
 
+@dataclasses.dataclass
+class MetricsServerConfig:
+  port: uint16
+
+
 # ▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼▼#
 
 
 def get_test_engine(devices: Devices, weight: int) -> engine_api.Engine:
   del devices
   return mock_engine.TestEngine(
       batch_size=8,
```

### Comparing `google_jetstream-0.2.1/jetstream/core/implementations/__init__.py` & `google_jetstream-0.2.2/jetstream/core/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/core/implementations/mock/__init__.py` & `google_jetstream-0.2.2/jetstream/core/implementations/mock/__init__.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/core/implementations/mock/config.py` & `google_jetstream-0.2.2/jetstream/core/implementations/mock/config.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/core/implementations/mock/server.py` & `google_jetstream-0.2.2/jetstream/core/implementations/mock/server.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/core/orchestrator.py` & `google_jetstream-0.2.2/jetstream/core/orchestrator.py`

 * *Files 18% similar despite different names*

```diff
@@ -81,25 +81,26 @@
 import os
 import queue
 import signal
 import sys
 import threading
 import time
 import traceback
-from typing import Any, AsyncIterator, Optional, Union
+from typing import Any, AsyncIterator, Optional, Tuple, cast
 
 import grpc
 import jax
 from jetstream.core.proto import jetstream_pb2
 from jetstream.core.proto import jetstream_pb2_grpc
 from jetstream.core.utils import async_multifuture
-from jetstream.engine import engine_api
+from jetstream.core.utils.return_sample import ReturnSample
+from jetstream.engine import engine_api, tokenizer_api, token_utils
+from jetstream.core.metrics.prometheus import JetstreamMetricsCollector
 import numpy as np
 
-
 root = logging.getLogger()
 root.setLevel(logging.DEBUG)
 
 handler = logging.StreamHandler(sys.stdout)
 handler.setLevel(logging.DEBUG)
 formatter = logging.Formatter(
     "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
@@ -122,35 +123,36 @@
   """Current state of the driver."""
 
   #################### Information relevant for generation #####################
   max_tokens: int
   # We keep prefill and decode information together in the same object so that
   # there is less indirection about where this return channel is.
   # The return channel returns a list of strings, one per sample for that query.
-  return_channel: async_multifuture.AsyncMultifuture[list[list[int]]]
+  return_channel: async_multifuture.AsyncMultifuture[list[ReturnSample]]
   # [num_samples,] which corresponds to whether each sample is complete for the
   # requests.
   complete: Optional[np.ndarray] = None
   prefill_result: Any = None
   #################### Information relevant for prefill ########################
   history_path: Optional[str] = None
-  prefill_text: Optional[str] = None
+  prefill_content: Optional[str | list[int]] = None
   ################## Information relevant for detokenization ###################
   # Which generate step this was added at.
   generate_timestep_added: Optional[int] = None
+  is_client_side_tokenization: Optional[bool] = False
 
-  def enqueue_tokens(self, generated_tokens: list[list[int]]):
-    """Records information about the step.
+  def enqueue_samples(self, generated_samples: list[ReturnSample]):
+    """Adds the generated sample(s) to return channel for current step.
 
     Args:
-      generated_tokens: One token to put into the return channel
+      generated_samples: The generated sample(s) for current step.
 
     This should be called only from within the Drivers background thread.
     """
-    self.return_channel.add_result(generated_tokens)
+    self.return_channel.add_result(generated_samples)
 
 
 class JetThread(threading.Thread):
   """Thread that kills the program if it fails.
 
   If a driver thread goes down, we can't operate.
   """
@@ -205,22 +207,27 @@
   # For interleaved_mode, only generate if all slots are full
   # or corresponding prefill queue is empty.
   _interleaved_mode: bool = False
 
   # todo: remove jax_padding after all then engine migrate to np padding
   _jax_padding = True
 
+  # All metrics we want to monitor should be collected with this
+  _metrics_collector: JetstreamMetricsCollector | None = None
+
   def __init__(
       self,
       prefill_engines: Optional[list[engine_api.Engine]] = None,
       generate_engines: Optional[list[engine_api.Engine]] = None,
       prefill_params: Optional[list[Any]] = None,
       generate_params: Optional[list[Any]] = None,
       interleaved_mode: bool = False,
       jax_padding: bool = True,
+      metrics_collector: JetstreamMetricsCollector | None = None,
+      is_ray_backend: bool = False,
   ):
     if prefill_engines is None:
       prefill_engines = []
     if generate_engines is None:
       generate_engines = []
     if prefill_params is None:
       prefill_params = []
@@ -233,19 +240,25 @@
         len(generate_engines),
     )
     self._prefill_engines = prefill_engines
     self._generate_engines = generate_engines
     self._prefill_params = prefill_params
     self._generate_params = generate_params
     self._interleaved_mode = interleaved_mode
+    self._metrics_collector = metrics_collector
 
     # Stages 1-4 represent the life cycle of a request.
     # Stage 1
     # At first, a request is placed here in order to get prefilled.
     self._prefill_backlog = queue.Queue()
+    if self._metrics_collector:
+      self._metrics_collector.get_prefill_backlog_metric().set_function(
+          lambda: float(self._prefill_backlog.qsize())
+      )
+
     # Stage 2
     # After prefilling, it is placed here in order to get transferred to
     # one of the generate backlogs.
     # Interleaved Mode: Max size is 1 to increase the HBM utilization
     # during generate.
     # Disaggregated Mode: Max size is 4 to allow for 2 prefills to be enqueued
     # while 1 transfer is enqueued while 1 is being transferred.
@@ -358,14 +371,15 @@
             self._prefill_threads,
             self._transfer_threads,
             self._generate_threads,
             self.detokenize_threads,
         )
     )
     self.live = True
+    self._is_ray_backend = is_ray_backend
     # Start all threads
     for t in self._all_threads:
       t.start()
 
   def stop(self):
     """Stops the driver and all background threads."""
     # Signal to all threads that they should stop.
@@ -418,53 +432,71 @@
     return total_max_concurrent_decodes
 
   def place_request_on_prefill_queue(self, request: ActiveRequest):
     """Used to place new requests for prefilling and generation."""
     # Don't block so we can fail and shed load when the queue is full.
     self._prefill_backlog.put(request, block=False)
 
-  def _load_cache_history(self, path: str) -> Union[None, Any]:
-    """Loads previous kv cache for a longer conversation."""
-    if path:
-      raise NotImplementedError
+  def _process_prefill_content(
+      self,
+      request: ActiveRequest,
+      tokenizer: tokenizer_api.Tokenizer,
+      is_bos: bool,
+      max_prefill_length: int,
+  ) -> Tuple[jax.Array | np.ndarray, int]:
+    content = request.prefill_content
+    if isinstance(content, str):
+      # If it's text input, tokenize and pad the input.
+      return tokenizer.encode(
+          content,
+          is_bos=is_bos,
+          max_prefill_length=max_prefill_length,
+          jax_padding=self._jax_padding,
+      )
     else:
-      return None
+      # If it's token input, pad the input.
+      return token_utils.pad_tokens(
+          content,
+          tokenizer.bos_id,
+          tokenizer.pad_id,
+          is_bos=is_bos,
+          max_prefill_length=max_prefill_length,
+          jax_padding=self._jax_padding,
+      )
 
   def _prefill_thread(self, idx: int):
     """Thread which runs in the background performing prefills."""
     logging.info("---------Spinning up prefill thread %d.---------", idx)
     prefill_engine = self._prefill_engines[idx]
     prefill_params = self._prefill_params[idx]
     metadata = prefill_engine.get_tokenizer()
     tokenizer = prefill_engine.build_tokenizer(metadata)
     logging.info("---------Prefill params %d loaded.---------", idx)
 
     while self.live:
       my_transfer_backlog = self._transfer_backlogs[idx]
       # The prefill thread can just sleep until it has work to do.
       request = self._prefill_backlog.get(block=True)
+
       if request is None:
         break
-      # Tokenize, and introduce a leading dimension
       is_bos = not bool(request.history_path)
       logging.info(
           "Prefilling on prefill engine %d : prefill queue size, %d,"
           " is_bos: %s, history: %s",
           idx,
           self._prefill_backlog.qsize(),
           is_bos,
           request.history_path,
       )
-      padded_tokens, true_length = tokenizer.encode(
-          request.prefill_text,
-          is_bos=is_bos,
-          max_prefill_length=prefill_engine.max_prefill_length,
-          jax_padding=self._jax_padding,
+      # Tokenize and padding the text or token input.
+      padded_tokens, true_length = self._process_prefill_content(
+          request, tokenizer, is_bos, prefill_engine.max_prefill_length
       )
-      # Compute new kv cache for the prefill_text.
+      # Compute new kv cache for the prefill_content.
       prefill_result = prefill_engine.prefill(
           params=prefill_params,
           padded_tokens=padded_tokens,
           true_length=true_length,
       )
       request.prefill_result = prefill_result
       # Once prefill is complete, place it on the generation queue and block if
@@ -474,43 +506,61 @@
           "Placed request on transfer queue %d, %d queued requests.",
           idx,
           my_transfer_backlog.qsize(),
       )
       del prefill_result
       del request
 
+  def _jax_transfer_prefill_result(
+      self, new_request: ActiveRequest, target_idx: int
+  ):
+    new_request.prefill_result = jax.device_put(
+        new_request.prefill_result,
+        self._generate_engines[target_idx].get_prefix_destination_sharding(),
+    )
+    # Block here so we don't block on the generate thread that steps.
+    jax.block_until_ready(new_request.prefill_result)
+
+  def _ray_transfer_prefill_result(
+      self, new_request: ActiveRequest, target_idx: int
+  ):
+    self._generate_engines[target_idx].transfer(new_request.prefill_result)
+
+  def _transfer_prefill_result(
+      self, new_request: ActiveRequest, target_idx: int
+  ):
+    if self._is_ray_backend:
+      self._ray_transfer_prefill_result(new_request, target_idx)
+    else:
+      self._jax_transfer_prefill_result(new_request, target_idx)
+
   def _transfer_thread(self, idx: int):
     """Transfers the kv cache on an active request to the least full
     generate backlog."""
     transfer_backlog = self._transfer_backlogs[idx]
 
     while self.live:
       # The transfer thread can just sleep until it has work to do.
       new_request = transfer_backlog.get(block=True)
+      if new_request is None:
+        break
       target_idx = min(
           self._generate_backlogs.items(), key=lambda q: q[1].qsize()
       )[0]
       # Only transfer the KVCache for the disaggregated serving.
       # TODO: Remove the conditional after fixing the compatibility.
       if not self._interleaved_mode:
         logging.info(
             "Transferring prefill from prefill engine %d "
             "to generate engine %d.",
             idx,
             target_idx,
         )
         # Transfer the info to the relevant generate slice.
-        new_request.prefill_result = jax.device_put(
-            new_request.prefill_result,
-            self._generate_engines[
-                target_idx
-            ].get_prefix_destination_sharding(),
-        )
-        # Block here so we don't block on the generate thread that steps.
-        jax.block_until_ready(new_request.prefill_result)
+        self._transfer_prefill_result(new_request, target_idx)
       # Place the request on the correct generate backlog and block if full.
       self._generate_backlogs[target_idx].put(new_request, block=True)
       logging.info(
           "Successfully transferred prefill "
           "from prefill engine %d to generate engine %d.",
           idx,
           target_idx,
@@ -542,14 +592,19 @@
             self._prefill_backlog.qsize(),
             my_slots.qsize(),
         )
         time_of_last_print = time.time()
 
       max_concurrent_decodes = generate_engine.max_concurrent_decodes
 
+      if self._metrics_collector:
+        self._metrics_collector.get_slots_available_percentage_metric(
+            idx
+        ).set_function(lambda: float(my_slots.qsize() / max_concurrent_decodes))
+
       # Check if there are any free my_slots. We don't want to block here since
       # we can still generate if we can't insert. We do this in a while loop to
       # insert as many sequences as possible.
       while True:
         my_slots_size = my_slots.qsize()
 
         try:
@@ -650,23 +705,25 @@
         generate_timestep_added, result_tokens = data
         # Disable attribute error because pytype doesn't know this
         # is a result tokens, and we can't annotate the tuple.
         result_tokens = result_tokens.convert_to_numpy()
 
         for slot, request in my_live_requests.items():
           if request is not None:
-            results, complete = tokenizer.decode(
+            results, complete = token_utils.process_result_tokens(
+                tokenizer=tokenizer,
                 slot=slot,
                 slot_max_length=request.max_tokens,
                 result_tokens=result_tokens,
+                is_client_side_tokenization=request.is_client_side_tokenization,
                 complete=request.complete,
             )
             request.complete = complete
-            # Return some tokens.
-            request.enqueue_tokens(results)
+            # Return some output samples.
+            request.enqueue_samples(results)
             if request.complete.all():
               request.return_channel.close()
               # Place the slot back on the free queue.
               my_live_requests[slot] = None
               my_slots.put(slot, block=False)  # This should always have space.
         logging.info(
             "Detokenizing generate step %d took %.2fms",
@@ -683,33 +740,107 @@
   """Coordinates a set of prefill and generate slices for LLM decoding."""
 
   _driver: Driver
 
   def __init__(self, driver: Driver):
     self._driver = driver
 
+  def _get_prefill_content(
+      self, request: jetstream_pb2.DecodeRequest
+  ) -> Tuple[str | list[int], bool]:
+    which_content = request.WhichOneof("content")
+    content = getattr(request, which_content)
+    if which_content == "text_content":
+      return cast(jetstream_pb2.DecodeRequest.TextContent, content).text, False
+    else:
+      return (
+          list(
+              cast(jetstream_pb2.DecodeRequest.TokenContent, content).token_ids
+          ),
+          True,
+      )
+
+  def process_client_side_tokenization_response(self, response: Any):
+    samples = []
+    for sample in response:
+      samples.append(
+          jetstream_pb2.DecodeResponse.StreamContent.Sample(
+              token_ids=sample.token_ids,
+          )
+      )
+    return jetstream_pb2.DecodeResponse(
+        stream_content=jetstream_pb2.DecodeResponse.StreamContent(
+            samples=samples
+        )
+    )
+
+  def should_buffer_response(self, response: Any) -> bool:
+    for item in response:
+      if item.text and token_utils.is_byte_token(item.text[-1]):
+        # If any sample ends in bytes, this means we might still need to
+        # decode more bytes to compose the string.
+        return True
+
+  def process_server_side_tokenization_response(
+      self, response: Any, buffered_response_list
+  ):
+    # Flush the buffered responses to each sample of current response.
+    current_response_with_flushed_buffer = list(
+        zip(*buffered_response_list, response)
+    )
+    # Empty buffer: [[s0_cur], [s1_cur], ...]
+    # Has buffer:
+    # [[s0_b0, s0_b1, ..., s0_cur], [s1_b0, s1_b1, ..., s1_cur], ...]
+    current_response_with_flushed_buffer = cast(
+        list[list[ReturnSample]], current_response_with_flushed_buffer
+    )
+    # Form correct sample(s) and return as StreamContent for this iteration.
+    samples = []
+    for sample in current_response_with_flushed_buffer:
+      text = []
+      token_ids = []
+      for resp in sample:
+        text.extend(resp.text)
+        token_ids.extend(resp.token_ids)
+      samples.append(
+          jetstream_pb2.DecodeResponse.StreamContent.Sample(
+              text=token_utils.text_tokens_to_str(text),
+              token_ids=token_ids,
+          )
+      )
+    return jetstream_pb2.DecodeResponse(
+        stream_content=jetstream_pb2.DecodeResponse.StreamContent(
+            samples=samples
+        )
+    )
+
   async def Decode(  # pylint: disable=invalid-overridden-method
       self,
       request: jetstream_pb2.DecodeRequest,
       context: Optional[grpc.aio.ServicerContext] = None,
   ) -> AsyncIterator[jetstream_pb2.DecodeResponse]:
     """Decode."""
     if context is None:
       logging.warning(
           "LLM orchestrator is being used in offline test mode, and will not"
           " respond to gRPC queries - only direct function calls."
       )
+    is_client_side_tokenization = False
     return_channel = async_multifuture.AsyncMultifuture()
     if context:
       context.add_done_callback(return_channel.cancel)
+    prefill_content, is_client_side_tokenization = self._get_prefill_content(
+        request
+    )
     # Wrap request as an ActiveRequest.
     active_request = ActiveRequest(
         max_tokens=request.max_tokens,
         history_path=request.session_cache,
-        prefill_text=request.additional_text,
+        prefill_content=prefill_content,
+        is_client_side_tokenization=is_client_side_tokenization,
         return_channel=return_channel,
     )
     # The first stage is being prefilled, all other stages are handled
     # inside the driver (transfer, generate*N, detokenize).
     try:
       self._driver.place_request_on_prefill_queue(active_request)
     except queue.Full:
@@ -721,22 +852,50 @@
               "The driver prefill queue is full and more requests cannot be"
               " handled. You may retry this request."
           ),
       )
     logging.info(
         "Placed request on the prefill queue.",
     )
+    # When an active request is created a queue is instantiated. New tokens
+    # are placed there during the decoding loop, we pop from that queue by
+    # using the .next method on the active request.
+    # Yielding allows for the response to be a streaming grpc call - which
+    # can be called via iterating over a for loop on the client side.
+    # The DecodeResponse stream should consume all generated tokens in
+    # return_channel when complete signal is received (AsyncMultifuture
+    # promises this).
+    buffered_response_list = []
     async for response in active_request.return_channel:
-      # When an active request is created a queue is instantiated. New tokens
-      # are placed there during the decoding loop, we pop from that queue by
-      # using the .next method on the active request.
-      # Yielding allows for the response to be a streaming grpc call - which
-      # can be called via iterating over a for loop on the other side.
-      # The DecodeResponse stream should consume all generated tokens in
-      # return_channel when complete signal is received. It should check if
-      # return_channel is empty to decide if it should exit the while loop.
-      repeated_token_ids = []
-      for token_ids in response:
-        repeated_token_ids.append(
-            jetstream_pb2.RepeatedTokenIds(token_ids=token_ids)
+      response = cast(list[ReturnSample], response)
+      if is_client_side_tokenization:
+        # If is_client_side_tokenization, the client should request with token
+        # ids, and the JetStream server will return token ids as response.
+        # The client should take care of tokenization and detokenization.
+        yield self.process_client_side_tokenization_response(response)
+      else:
+        # Buffer response mechanism is used to handle streaming
+        # detokenization with special character (For some edge cases with
+        # SentencePiece tokenizer, it requires to decode a complete sequence
+        # instead of a single token).
+        if self.should_buffer_response(response):
+          buffered_response_list.append(response)
+          continue
+        yield self.process_server_side_tokenization_response(
+            response, buffered_response_list
         )
-      yield jetstream_pb2.DecodeResponse(response=repeated_token_ids)
+        # Reset buffer after flushed.
+        buffered_response_list = []
+
+  async def HealthCheck(  # pylint: disable=invalid-overridden-method
+      self,
+      request: jetstream_pb2.HealthCheckRequest,
+      context: Optional[grpc.aio.ServicerContext] = None,
+  ) -> jetstream_pb2.HealthCheckResponse:
+    """HealthCheck."""
+    if context is None:
+      logging.warning(
+          "LLM orchestrator is being used in offline test mode, and will not"
+          " respond to gRPC queries - only direct function calls."
+      )
+    is_live = self._driver.live
+    return jetstream_pb2.HealthCheckResponse(is_live=is_live)
```

### Comparing `google_jetstream-0.2.1/jetstream/core/proto/__init__.py` & `google_jetstream-0.2.2/jetstream/core/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/core/proto/jetstream_pb2.py` & `google_jetstream-0.2.2/jetstream/engine/tokenizer_pb2.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,40 +10,35 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: jetstream/core/proto/jetstream.proto
+# source: jetstream/engine/tokenizer.proto
 # Protobuf Python Version: 4.25.1
 # pylint: disable=all
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n$jetstream/core/proto/jetstream.proto\x12\x0fjetstream_proto"e\n\rDecodeRequest\x12\x15\n\rsession_cache\x18\x01 \x01(\t\x12\x17\n\x0f\x61\x64\x64itional_text\x18\x02 \x01(\t\x12\x10\n\x08priority\x18\x03 \x01(\x05\x12\x12\n\nmax_tokens\x18\x04 \x01(\x05"E\n\x0e\x44\x65\x63odeResponse\x12\x33\n\x08response\x18\x01 \x03(\x0b\x32!.jetstream_proto.RepeatedTokenIds"%\n\x10RepeatedTokenIds\x12\x11\n\ttoken_ids\x18\x01 \x03(\x05\x32]\n\x0cOrchestrator\x12M\n\x06\x44\x65\x63ode\x12\x1e.jetstream_proto.DecodeRequest\x1a\x1f.jetstream_proto.DecodeResponse"\x00\x30\x01\x62\x06proto3'
+    b'\n jetstream/engine/tokenizer.proto\x12\x06\x65ngine"6\n\x13TokenizerParameters\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x11\n\textra_ids\x18\x02 \x01(\x05\x42\x02P\x01\x62\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(
-    DESCRIPTOR, "jetstream.core.proto.jetstream_pb2", _globals
+    DESCRIPTOR, "jetstream.engine.tokenizer_pb2", _globals
 )
 if _descriptor._USE_C_DESCRIPTORS == False:
-  DESCRIPTOR._options = None
-  _globals["_DECODEREQUEST"]._serialized_start = 57
-  _globals["_DECODEREQUEST"]._serialized_end = 158
-  _globals["_DECODERESPONSE"]._serialized_start = 160
-  _globals["_DECODERESPONSE"]._serialized_end = 229
-  _globals["_REPEATEDTOKENIDS"]._serialized_start = 231
-  _globals["_REPEATEDTOKENIDS"]._serialized_end = 268
-  _globals["_ORCHESTRATOR"]._serialized_start = 270
-  _globals["_ORCHESTRATOR"]._serialized_end = 363
+  _globals["DESCRIPTOR"]._options = None
+  _globals["DESCRIPTOR"]._serialized_options = b"P\001"
+  _globals["_TOKENIZERPARAMETERS"]._serialized_start = 44
+  _globals["_TOKENIZERPARAMETERS"]._serialized_end = 98
 # @@protoc_insertion_point(module_scope)
```

### Comparing `google_jetstream-0.2.1/jetstream/core/proto/jetstream_pb2_grpc.py` & `google_jetstream-0.2.2/jetstream/core/proto/jetstream_pb2_grpc.py`

 * *Files 23% similar despite different names*

```diff
@@ -30,33 +30,49 @@
         channel: A grpc.Channel.
     """
     self.Decode = channel.unary_stream(
         "/jetstream_proto.Orchestrator/Decode",
         request_serializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeRequest.SerializeToString,
         response_deserializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeResponse.FromString,
     )
+    self.HealthCheck = channel.unary_unary(
+        "/jetstream_proto.Orchestrator/HealthCheck",
+        request_serializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.HealthCheckRequest.SerializeToString,
+        response_deserializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.HealthCheckResponse.FromString,
+    )
 
 
 class OrchestratorServicer(object):
   """TODO: Merge this with main JetStream core once we settle on an API."""
 
   def Decode(self, request, context):
-    """Generate the next model tokens."""
+    """Query LLM to generate text or tokens."""
+    context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+    context.set_details("Method not implemented!")
+    raise NotImplementedError("Method not implemented!")
+
+  def HealthCheck(self, request, context):
+    """Checks if the model server is live."""
     context.set_code(grpc.StatusCode.UNIMPLEMENTED)
     context.set_details("Method not implemented!")
     raise NotImplementedError("Method not implemented!")
 
 
 def add_OrchestratorServicer_to_server(servicer, server):
   rpc_method_handlers = {
       "Decode": grpc.unary_stream_rpc_method_handler(
           servicer.Decode,
           request_deserializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeRequest.FromString,
           response_serializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.DecodeResponse.SerializeToString,
       ),
+      "HealthCheck": grpc.unary_unary_rpc_method_handler(
+          servicer.HealthCheck,
+          request_deserializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.HealthCheckRequest.FromString,
+          response_serializer=jetstream_dot_core_dot_proto_dot_jetstream__pb2.HealthCheckResponse.SerializeToString,
+      ),
   }
   generic_handler = grpc.method_handlers_generic_handler(
       "jetstream_proto.Orchestrator", rpc_method_handlers
   )
   server.add_generic_rpc_handlers((generic_handler,))
 
 
@@ -86,9 +102,38 @@
         options,
         channel_credentials,
         insecure,
         call_credentials,
         compression,
         wait_for_ready,
         timeout,
+        metadata,
+    )
+
+  @staticmethod
+  def HealthCheck(
+      request,
+      target,
+      options=(),
+      channel_credentials=None,
+      call_credentials=None,
+      insecure=False,
+      compression=None,
+      wait_for_ready=None,
+      timeout=None,
+      metadata=None,
+  ):
+    return grpc.experimental.unary_unary(
+        request,
+        target,
+        "/jetstream_proto.Orchestrator/HealthCheck",
+        jetstream_dot_core_dot_proto_dot_jetstream__pb2.HealthCheckRequest.SerializeToString,
+        jetstream_dot_core_dot_proto_dot_jetstream__pb2.HealthCheckResponse.FromString,
+        options,
+        channel_credentials,
+        insecure,
+        call_credentials,
+        compression,
+        wait_for_ready,
+        timeout,
         metadata,
     )
```

### Comparing `google_jetstream-0.2.1/jetstream/core/utils/__init__.py` & `google_jetstream-0.2.2/jetstream/core/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/core/utils/async_multifuture.py` & `google_jetstream-0.2.2/jetstream/core/utils/async_multifuture.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/engine/__init__.py` & `google_jetstream-0.2.2/jetstream/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/engine/engine_api.py` & `google_jetstream-0.2.2/jetstream/engine/engine_api.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/engine/mock_engine.py` & `google_jetstream-0.2.2/jetstream/engine/mock_engine.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/engine/mock_utils.py` & `google_jetstream-0.2.2/jetstream/engine/mock_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,15 @@
   the seqio.Vocabulary interface.
   """
 
   pad_id = 0
   eos_id = 1
   bos_id = 2
   unk_id = 3
+  stop_tokens = {pad_id, eos_id}
   _base_vocab_size = 2**16
   tokenizer: TestTokenizer = TestTokenizer()
 
   def _encode(self, s: str) -> Sequence[int]:
     """Converts a string into a integer sequenc."""
     # 'We use array methods, not python iterables so we don't
     # implement this method in the mock vocab.
@@ -72,17 +73,17 @@
 
   def _decode_tf(self, ids: np.ndarray) -> List[str]:
     """Converts a numpy array into a string."""
     # We mock using numpy to avoid propagating tf dependencies.
     results = np.split(ids, ids.shape[0])
     return ["".join([chr(r) for r in list(line[0])]) for line in results]
 
-  def decode(self, ids: np.ndarray):
+  def decode(self, ids: np.ndarray, is_streaming=True):
     """Converts a numpy array into a string."""
-    return self._decode(ids)
+    return is_streaming and self._decode(ids)
 
   def encode_tf(self, s: str) -> np.ndarray:
     """Converts a string into a numpy array."""
     return self._encode_tf(s)
 
   def decode_tf(self, ids: np.ndarray) -> List[str]:
     """Converts a numpy array into a string."""
```

### Comparing `google_jetstream-0.2.1/jetstream/engine/token_utils.py` & `google_jetstream-0.2.2/jetstream/engine/token_utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Token manipulation utilities."""
 
 from bisect import bisect_left
 import logging
-from typing import Any, List, Optional, Tuple, Union
+from typing import Any, Iterable, List, Optional, Tuple, Union
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 from seqio.vocabularies import SentencePieceVocabulary
 from seqio.vocabularies import Vocabulary
 
+from jetstream.core.utils.return_sample import ReturnSample
 from jetstream.engine import mock_utils
 from jetstream.engine import tokenizer_api
 from jetstream.engine import tokenizer_pb2
 from jetstream.third_party.llama3 import llama3_tokenizer
 
 # ResultToken class to store tokens ids.
 ResultTokens = Any
@@ -87,21 +88,22 @@
     bos_id: int,
     pad_id: int,
     is_bos: bool = True,
     prefill_lengths: Optional[List[int]] = None,
     max_prefill_length: Optional[int] = None,
     jax_padding: bool = True,
 ) -> Tuple[Union[jax.Array, np.ndarray], int]:
-  """Tokenize and pads a string.
+  """Pads tokens to the nearest prefill length that is equal to or greater
+     than the token length.
 
   Args:
-    s: String to tokenize.
-    vocab: Vocabulary to tokenize with.
-    is_bos: Whether or not this is the beginning of a sequence. Default to yes
-      as prefill is typically used when beginning sequences.
+    tokens: Tokens.
+    bos_id: Bos ID.
+    pad_id: Pad ID.
+    is_bos: Add a beginning of sequence token if this is ture.
     prefill_lengths: Buckets to pad the sequence to for static compilation.
     max_prefill_length: Maximum bucket to use.
     jax_padding: convert to JAX padded tokens if True.
 
   Returns:
     tokens: Tokenized into integers.
     true_length: Actual length of the non-padded sequence.
@@ -151,57 +153,57 @@
     padded_tokens = np.pad(tokens, (0, padding), constant_values=(pad_id,))
   if jax_padding:
     padded_tokens = jnp.array(padded_tokens)
   return padded_tokens, true_length
 
 
 def process_result_tokens(
+    tokenizer: tokenizer_api.Tokenizer,
     slot: int,
     slot_max_length: int,
     result_tokens: ResultTokens,
-    eos_id: int,
-    pad_id: int,
     complete: np.ndarray,
+    is_client_side_tokenization: bool = False,
     debug: bool = False,
-) -> Tuple[List[List[int]], np.ndarray]:
+) -> Tuple[List[ReturnSample], np.ndarray]:
   """Processes a result tokens into a list of strings, handling multiple
     samples.
 
   Args:
     slot: The slot at which to draw tokens from.
     slot_max_length: Max length for a sample in the slot.
     result_tokens: The tokens to access by slot.
-    eos_id: Id for EOS token.
-    pad_id: Id for pad token.
     complete: Array representing the completion status of each sample in the
       slot.
+    is_client_side_tokenization: Whether to detokenize on client side.
     debug: Whether to log step by step detokenisation.
 
   Returns:
-    sample_return: List of tok_id list, one list per sample.
+    return_samples: List of ReturnSample.
     complete: Updated complete.
   """
   # tokens: [samples, speculations]
   slot_data = result_tokens.get_result_at_slot(slot)
   slot_tokens = slot_data.tokens
   slot_valid = slot_data.valid
   slot_lengths = slot_data.lengths
   samples, speculations = slot_tokens.shape
-  stop_tokens = [eos_id, pad_id]
+  stop_tokens = tokenizer.stop_tokens
   # Stop anything which has reached it's max length.
   complete = complete | (slot_lengths > slot_max_length)
   if debug:
     logging.info(
         "Complete %s, slot_tokens: %s, slot_lengths: %s",
         str(complete),
         str(slot_tokens),
         str(slot_lengths),
     )
-  sample_return = []
+  return_samples = []
   for idx in range(samples):
+    text_so_far = []
     tok_id_so_far = []
     if not complete[idx].item():
       for spec_idx in range(speculations):
         tok_id = slot_tokens[idx, spec_idx].item()
         valid = slot_valid[idx, spec_idx].item()
         if debug:
           logging.info(
@@ -210,19 +212,26 @@
               spec_idx,
               tok_id,
           )
         if tok_id in stop_tokens or not valid:
           complete[idx] = True
           break
         else:
+          if not is_client_side_tokenization:
+            if isinstance(tokenizer, SentencePieceTokenizer):
+              text_so_far.append(tokenizer.decode([tok_id], is_streaming=True))
+            else:
+              text_so_far.append(tokenizer.decode([tok_id]))
           tok_id_so_far.append(tok_id)
-    sample_return.append(tok_id_so_far)
+    return_samples.append(
+        ReturnSample(text=text_so_far, token_ids=tok_id_so_far)
+    )
     if debug:
-      logging.info("Sampled return %s", str(sample_return))
-  return sample_return, complete
+      logging.info("Return samples %s", str(return_samples))
+  return return_samples, complete
 
 
 def load_vocab(path: str, extra_ids: int = 0) -> Vocabulary:
   """Eagerly loads a vocabulary.
 
   Args:
     path: Vocabulary file path.
@@ -241,27 +250,49 @@
     # SentencePieceVocabulary uses lazy loading. Request access to a property,
     # forcing the lazy loading to happen now.
     sp_model = vocab.sp_model
     del sp_model
     return vocab
 
 
+def is_byte_token(s: str) -> bool:
+  """Returns True if s is a byte string like "<0xAB>"."""
+  # Bytes look like "<0xAB>".
+  if len(s) != 6 or s[0:3] != "<0x" or s[-1] != ">":
+    return False
+  return True
+
+
+def text_tokens_to_str(text_tokens: Iterable[str]) -> str:
+  """Converts an iterable of token text to a single string, collapsing bytes.
+
+  e.g. ['你', '好', '<0xE5>', '<0x90>', '<0x97>', 'hello'] -> '你好吗hello'
+  """
+  bytes_so_far = []
+  for text_token in text_tokens:
+    if is_byte_token(text_token):
+      bytes_so_far.append(bytes([int(text_token[1:-1], 16)]))
+    else:
+      bytes_so_far.append(bytes(text_token, "utf-8"))
+  return b"".join(bytes_so_far).decode("utf-8", "replace")
+
+
 class SentencePieceTokenizer(tokenizer_api.Tokenizer):
   """Tokenizer to convert strings to token ids and vice-versa."""
 
   def __init__(self, metadata: tokenizer_pb2.TokenizerParameters):
     self.vocab = load_vocab(metadata.path, metadata.extra_ids)
 
   def encode(
       self, s: str, **kwargs
   ) -> Tuple[Union[jax.Array, np.ndarray], int]:
     """Tokenize a string.
     Args:
         s: String to tokenize.
-        **kwargs: Additional keyword arguments
+        **kwargs: Additional keyword arguments.
     Returns:
         tokens: Tokenized into integers.
         true_length: Actual length of the non-padded sequence
           if padding is used.
     """
     is_bos = kwargs.pop("is_bos", True)
     prefill_lengths = kwargs.pop("prefill_lengths", None)
@@ -277,55 +308,35 @@
         is_bos=is_bos,
         prefill_lengths=prefill_lengths,
         max_prefill_length=max_prefill_length,
         jax_padding=jax_padding,
     )
     return tokens, true_length
 
-  def decode(
-      self,
-      slot: int,
-      slot_max_length: int,
-      result_tokens: ResultTokens,
-      complete: np.ndarray,
-      **kwargs,
-  ) -> Tuple[List[List[int]], np.ndarray]:
-    """Processes a result tokens into a list of strings, handling multiple
-    samples.
-    Args:
-      slot: The slot at which to draw tokens from.
-      slot_max_length: Max length for a sample in the slot.
-      result_tokens: The tokens to access by slot.
-      complete: Array representing the completion status of each sample in the
-        slot.
-      kwargs: Additional keyword arguments.
-    Returns:
-      sample_return: List of strings, one per sample.
-      complete: Updated complete.
-    """
-    debug = kwargs.pop("debug", False)
-    results, complete = process_result_tokens(
-        slot=slot,
-        slot_max_length=slot_max_length,
-        result_tokens=result_tokens,
-        eos_id=self.eos_id,
-        pad_id=self.pad_id,
-        complete=complete,
-        debug=debug,
-    )
-    return results, complete
-
-  def decode_str(self, token_ids: list[int]) -> str:
+  def decode(self, token_ids: list[int], **kwargs) -> str:
     """Processess input token ids to generate a string.
     Args:
       token_ids: List of token ids.
+      **kwargs: Additional keyword arguments.
     Returns:
       str: String generated from the token ids.
     """
-    return self.vocab.tokenizer.decode(token_ids)
+    # If is_streaming, we need to decode a token id to a piece.
+    is_streaming = kwargs.pop("is_streaming", False)
+    if is_streaming:
+      # The piece could be a byte token or a text token. It requires further
+      # processing for the byte tokens. For JetStream, it's handled in
+      # LLMOrchestrator.
+      piece = self.vocab.tokenizer.IdToPiece(token_ids[0])
+      # SentencePiece escapes the whitespace with a meta symbol "▁" (U+2581)
+      return piece.replace("▁", " ")
+    else:
+      # If it's not streaming decoding, we can directly decode the full list
+      # of token ids to a complete sequence.
+      return self.vocab.tokenizer.decode(token_ids)
 
   @property
   def pad_id(self) -> int:
     """ID of the pad token."""
     return self.vocab.pad_id
 
   @property
@@ -371,57 +382,29 @@
         is_bos=is_bos,
         prefill_lengths=prefill_lengths,
         max_prefill_length=max_prefill_length,
         jax_padding=jax_padding,
     )
     return tokens, true_length
 
-  def decode(
-      self,
-      slot: int,
-      slot_max_length: int,
-      result_tokens: ResultTokens,
-      complete: np.ndarray,
-      **kwargs,
-  ) -> Tuple[List[List[int]], np.ndarray]:
-    """Processes a result tokens into a list of strings, handling multiple
-    samples.
-    Args:
-      slot: The slot at which to draw tokens from.
-      slot_max_length: Max length for a sample in the slot.
-      result_tokens: The tokens to access by slot.
-      complete: Array representing the completion status of each sample in the
-        slot.
-      kwargs: Additional keyword arguments.
-    Returns:
-      sample_return: List of strings, one per sample.
-      complete: Updated complete.
-    """
-    debug = kwargs.pop("debug", False)
-    results, complete = process_result_tokens(
-        slot=slot,
-        slot_max_length=slot_max_length,
-        result_tokens=result_tokens,
-        eos_id=self.eos_id,
-        pad_id=self.pad_id,
-        complete=complete,
-        debug=debug,
-    )
-    return results, complete
-
-  def decode_str(self, token_ids: list[int]) -> str:
+  def decode(self, token_ids: list[int]) -> str:
     """Processess input token ids to generate a string.
     Args:
       token_ids: List of token ids.
     Returns:
       str: String generated from the token ids.
     """
     return self.tokenizer.decode(token_ids)
 
   @property
+  def stop_tokens(self) -> set[int]:
+    """ID of the stop token."""
+    return self.tokenizer.stop_tokens
+
+  @property
   def pad_id(self) -> int:
     """ID of the pad token."""
     return self.tokenizer.pad_id
 
   @property
   def eos_id(self) -> int:
     """ID of EOS token."""
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `google_jetstream-0.2.1/jetstream/engine/tokenizer_api.py` & `google_jetstream-0.2.2/jetstream/engine/tokenizer_api.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,49 +30,27 @@
   @abc.abstractmethod
   def encode(
       self, s: str, **kwargs
   ) -> Tuple[Union[jax.Array, np.ndarray], int]:
     """Tokenize a string.
     Args:
         s: String to tokenize.
-        **kwargs: Additional keyword arguments
+        **kwargs: Additional keyword arguments.
     Returns:
         tokens: Tokenized into integers.
         true_length: Actual length of the non-padded sequence
           if padding is used.
     """
 
   @abc.abstractmethod
-  def decode(
-      self,
-      slot: int,
-      slot_max_length: int,
-      result_tokens: ResultTokens,
-      complete: np.ndarray,
-      **kwargs,
-  ) -> Tuple[list[list[int]], np.ndarray]:
-    """Processes a result tokens into a list of token ids, handling multiple
-    samples.
-    Args:
-      slot: The slot at which to draw tokens from.
-      slot_max_length: Max length for a sample in the slot.
-      result_tokens: The tokens to access by slot.
-      complete: Array representing the completion status of each sample in the
-        slot.
-      **kwards: Additional keyword arguments.
-    Returns:
-      sample_return: List of token_ids, one per sample.
-      complete: Updated complete.
-    """
-
-  @abc.abstractmethod
-  def decode_str(self, token_ids: list[int]) -> str:
+  def decode(self, token_ids: list[int], **kwargs) -> str:
     """Processess input token ids to generate a string.
     Args:
       token_ids: List of token ids.
+      **kwargs: Additional keyword arguments.
     Returns:
       str: String generated from the token ids.
     """
 
   @property
   @abc.abstractmethod
   def pad_id(self) -> int:
@@ -83,7 +61,12 @@
   def eos_id(self) -> int:
     """ID of EOS token."""
 
   @property
   @abc.abstractmethod
   def bos_id(self) -> int:
     """ID of BOS token."""
+
+  @property
+  def stop_tokens(self) -> set[int]:
+    """ID of the stop token."""
+    return {self.eos_id, self.pad_id}
```

### Comparing `google_jetstream-0.2.1/jetstream/engine/tokenizer_pb2_grpc.py` & `google_jetstream-0.2.2/jetstream/engine/tokenizer_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/tests/__init__.py` & `google_jetstream-0.2.2/jetstream/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/tests/core/__init__.py` & `google_jetstream-0.2.2/jetstream/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/tests/core/test_config_lib.py` & `google_jetstream-0.2.2/jetstream/tests/core/test_config_lib.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,26 +10,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Unit test for config_lib.py."""
 
-from absl.testing import absltest, parameterized
+import unittest
+from parameterized import parameterized
 from jetstream.core import config_lib
 
 
-class TestConfigLib(parameterized.TestCase):
+class TestConfigLib(unittest.TestCase):
 
-  @parameterized.parameters(
-      ("tpu=8", 8),
-      ("v5e-8", 8),
-      ("v5e=4", 4),
-      ("v4-8", 4),
-  )
+  @parameterized.expand([("tpu=8", 8), ("v5e-8", 8), ("v5e=4", 4), ("v4-8", 4)])
   def test_slice_to_num_chips(self, accelerator_slice, expected_num_devices):
     got = config_lib.slice_to_num_chips(accelerator_slice)
     self.assertEqual(got, expected_num_devices)
 
-
-if __name__ == "__main__":
-  absltest.main()
+  def test_get_engines_invalid(self):
+    with self.assertRaises(ValueError):
+      config_lib.get_engines(config_lib.InterleavedCPUTestServer, [])
```

### Comparing `google_jetstream-0.2.1/jetstream/tests/engine/__init__.py` & `google_jetstream-0.2.2/jetstream/tests/core/__init__.py`

 * *Files identical despite different names*

### Comparing `google_jetstream-0.2.1/jetstream/tests/engine/test_mock_engine.py` & `google_jetstream-0.2.2/jetstream/tests/engine/test_mock_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,23 +26,23 @@
 If we then insert that and run three generation steps, we should see
 266+0 / 2 = 266
 266 + [266] /2  = 399
 266 + [266, 399] /2 = 598
 I.e. ['Ċ', 'Ə', 'ɖ'] when converted back with chr()
 """
 
+import unittest
 import jax.numpy as jnp
 import numpy as np
 
 from jetstream.engine import mock_engine
 from jetstream.engine import token_utils
-from absl.testing import absltest
 
 
-class EngineTest(absltest.TestCase):
+class EngineTest(unittest.TestCase):
 
   def _setup(self):
     """Initialises a test engine."""
     engine = mock_engine.TestEngine(batch_size=32, cache_length=256, weight=2.0)
     params = engine.load_params()
     return engine, params
 
@@ -124,11 +124,7 @@
     _, sampled_tokens = engine.generate(
         params=params, decode_state=decode_state
     )
     # Char for 598
     token_data = sampled_tokens.get_result_at_slot(slot)
     tok = token_data.tokens
     assert tokenizer.IdToPiece(int(tok.item())) == "ɖ"
-
-
-if __name__ == "__main__":
-  absltest.main()
```

### Comparing `google_jetstream-0.2.1/jetstream/third_party/llama3/llama3_tokenizer.py` & `google_jetstream-0.2.2/jetstream/third_party/llama3/llama3_tokenizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,16 +103,16 @@
         self.eos_id,
     )
 
   def encode(
       self,
       s: str,
       *,
-      bos: bool,
-      eos: bool,
+      bos: bool = False,
+      eos: bool = False,
       allowed_special: Union[Literal["all"], AbstractSet[str]] | None = None,
       disallowed_special: Union[Literal["all"], Collection[str]] = (),
   ) -> List[int]:
     """
     Encodes a string into a list of token IDs.
     Args:
         s (str): The input string to be encoded.
```

### Comparing `google_jetstream-0.2.1/setup.py` & `google_jetstream-0.2.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   with open(filename) as f:
     lineiter = (line.strip() for line in f)
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 setup(
     name="google-jetstream",
-    version="0.2.1",
+    version="0.2.2",
     description=(
         "JetStream is a throughput and memory optimized engine for LLM inference on XLA devices, starting with TPUs (and GPUs in future -- PRs welcome)."
     ),
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Google LLC",
     url="https://github.com/google/JetStream",
```

