# Comparing `tmp/xchainpy2_thorchain-0.0.6.tar.gz` & `tmp/xchainpy2_thorchain-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchainpy2_thorchain-0.0.6.tar", last modified: Wed Jan  3 19:12:38 2024, max compression
+gzip compressed data, was "xchainpy2_thorchain-0.0.7.tar", last modified: Fri Jan  5 17:02:38 2024, max compression
```

## Comparing `xchainpy2_thorchain-0.0.6.tar` & `xchainpy2_thorchain-0.0.7.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.483241 xchainpy2_thorchain-0.0.6/
--rw-r--r--   0 tirinox    (501) staff       (20)     2124 2023-04-22 16:09:04.000000 xchainpy2_thorchain-0.0.6/LICENSE
--rw-r--r--   0 tirinox    (501) staff       (20)     1170 2024-01-03 19:12:38.482991 xchainpy2_thorchain-0.0.6/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)       69 2023-05-27 15:54:02.000000 xchainpy2_thorchain-0.0.6/README.md
--rw-r--r--   0 tirinox    (501) staff       (20)     1353 2024-01-03 16:44:17.000000 xchainpy2_thorchain-0.0.6/pyproject.toml
--rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-01-03 19:12:38.483294 xchainpy2_thorchain-0.0.6/setup.cfg
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.475090 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/
--rw-r--r--   0 tirinox    (501) staff       (20)       86 2023-05-28 08:39:39.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)    11360 2024-01-03 16:43:19.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/client.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3192 2023-11-19 17:55:21.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/const.py
--rw-r--r--   0 tirinox    (501) staff       (20)      727 2023-11-24 19:11:50.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/models.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.475999 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/
--rw-r--r--   0 tirinox    (501) staff       (20)       75 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.476257 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/cosmos/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/cosmos/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.476377 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/cosmos/base/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/cosmos/base/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.477167 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/cosmos/base/v1beta1/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/cosmos/base/v1beta1/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2808 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/cosmos/base/v1beta1/coin_pb2.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1141 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/cosmos/base/v1beta1/coin_pb2.pyi
--rw-r--r--   0 tirinox    (501) staff       (20)      159 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/cosmos/base/v1beta1/coin_pb2_grpc.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.478155 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/gogoproto/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/gogoproto/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7721 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/gogoproto/gogo_pb2.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6847 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/gogoproto/gogo_pb2.pyi
--rw-r--r--   0 tirinox    (501) staff       (20)      159 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/gogoproto/gogo_pb2_grpc.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.478414 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.478537 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.479197 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/common/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/common/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5694 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/common/common_pb2.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2971 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/common/common_pb2.pyi
--rw-r--r--   0 tirinox    (501) staff       (20)      159 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/common/common_pb2_grpc.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.479470 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.479595 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.480726 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2050 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_deposit_pb2.py
--rw-r--r--   0 tirinox    (501) staff       (20)      902 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_deposit_pb2.pyi
--rw-r--r--   0 tirinox    (501) staff       (20)      159 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_deposit_pb2_grpc.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2304 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_send_pb2.py
--rw-r--r--   0 tirinox    (501) staff       (20)      947 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_send_pb2.pyi
--rw-r--r--   0 tirinox    (501) staff       (20)      159 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_send_pb2_grpc.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.481132 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/tests/
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.472446 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/tests/mock/
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.472510 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/tests/mock/samples/
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.482139 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/tests/mock/samples/tx/
--rw-r--r--   0 tirinox    (501) staff       (20)    12277 2023-07-20 12:35:56.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/tests/mock/samples/tx/bond-tn-8F241485970BE3CFCDE21A1F9C8E1EDD42DFF2F78B9B17358E2F81276F46173C.json
--rw-r--r--   0 tirinox    (501) staff       (20)     9297 2023-07-20 12:53:04.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/tests/mock/samples/tx/send-DBEE3FF8DC82EBB490ECE26FD761955BD6E3740BE064E8D5D27CB5F618BE6360.json
--rw-r--r--   0 tirinox    (501) staff       (20)     5105 2023-07-20 12:08:22.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/tests/mock/samples/tx/swap-1C10434D59A460FD0BE76C46A333A583B8C7761094E26C0B2548D07A5AF28356.json
--rw-r--r--   0 tirinox    (501) staff       (20)     3333 2024-01-03 16:43:19.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/tests/test_basic_tc.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2298 2024-01-03 18:28:26.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/tests/test_utils.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3516 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/utils.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:38.482494 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain.egg-info/
--rw-r--r--   0 tirinox    (501) staff       (20)     1170 2024-01-03 19:12:38.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain.egg-info/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)     2389 2024-01-03 19:12:38.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain.egg-info/SOURCES.txt
--rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-01-03 19:12:38.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain.egg-info/dependency_links.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       89 2024-01-03 19:12:38.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain.egg-info/requires.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       20 2024-01-03 19:12:38.000000 xchainpy2_thorchain-0.0.6/xchainpy2_thorchain.egg-info/top_level.txt
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.608767 xchainpy2_thorchain-0.0.7/
+-rw-r--r--   0 tirinox    (501) staff       (20)     2124 2023-04-22 16:09:04.000000 xchainpy2_thorchain-0.0.7/LICENSE
+-rw-r--r--   0 tirinox    (501) staff       (20)     1170 2024-01-05 17:02:38.608512 xchainpy2_thorchain-0.0.7/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)       69 2023-05-27 15:54:02.000000 xchainpy2_thorchain-0.0.7/README.md
+-rw-r--r--   0 tirinox    (501) staff       (20)     1353 2024-01-05 17:02:02.000000 xchainpy2_thorchain-0.0.7/pyproject.toml
+-rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-01-05 17:02:38.608825 xchainpy2_thorchain-0.0.7/setup.cfg
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.598983 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/
+-rw-r--r--   0 tirinox    (501) staff       (20)       86 2023-05-28 08:39:39.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    11361 2024-01-05 17:01:27.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/client.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3192 2023-11-19 17:55:21.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/const.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      727 2023-11-24 19:11:50.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/models.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.600290 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/
+-rw-r--r--   0 tirinox    (501) staff       (20)       75 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.600573 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/cosmos/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/cosmos/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.600703 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/cosmos/base/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/cosmos/base/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.601763 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/cosmos/base/v1beta1/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/cosmos/base/v1beta1/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2808 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/cosmos/base/v1beta1/coin_pb2.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1141 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/cosmos/base/v1beta1/coin_pb2.pyi
+-rw-r--r--   0 tirinox    (501) staff       (20)      159 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/cosmos/base/v1beta1/coin_pb2_grpc.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.602787 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/gogoproto/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/gogoproto/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7721 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/gogoproto/gogo_pb2.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6847 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/gogoproto/gogo_pb2.pyi
+-rw-r--r--   0 tirinox    (501) staff       (20)      159 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/gogoproto/gogo_pb2_grpc.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.603048 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.603177 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.604174 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/common/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/common/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5694 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/common/common_pb2.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2971 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/common/common_pb2.pyi
+-rw-r--r--   0 tirinox    (501) staff       (20)      159 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/common/common_pb2_grpc.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.604489 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.604627 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.606021 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2050 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_deposit_pb2.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      902 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_deposit_pb2.pyi
+-rw-r--r--   0 tirinox    (501) staff       (20)      159 2023-11-18 20:03:31.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_deposit_pb2_grpc.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2304 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_send_pb2.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      947 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_send_pb2.pyi
+-rw-r--r--   0 tirinox    (501) staff       (20)      159 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_send_pb2_grpc.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.606506 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/tests/
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.596793 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/tests/mock/
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.596865 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/tests/mock/samples/
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.607620 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/tests/mock/samples/tx/
+-rw-r--r--   0 tirinox    (501) staff       (20)    12277 2023-07-20 12:35:56.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/tests/mock/samples/tx/bond-tn-8F241485970BE3CFCDE21A1F9C8E1EDD42DFF2F78B9B17358E2F81276F46173C.json
+-rw-r--r--   0 tirinox    (501) staff       (20)     9297 2023-07-20 12:53:04.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/tests/mock/samples/tx/send-DBEE3FF8DC82EBB490ECE26FD761955BD6E3740BE064E8D5D27CB5F618BE6360.json
+-rw-r--r--   0 tirinox    (501) staff       (20)     5105 2023-07-20 12:08:22.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/tests/mock/samples/tx/swap-1C10434D59A460FD0BE76C46A333A583B8C7761094E26C0B2548D07A5AF28356.json
+-rw-r--r--   0 tirinox    (501) staff       (20)     4321 2024-01-05 17:00:55.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/tests/test_basic_tc.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2298 2024-01-03 18:28:26.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/tests/test_utils.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3516 2023-11-19 09:49:41.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/utils.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-05 17:02:38.607990 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain.egg-info/
+-rw-r--r--   0 tirinox    (501) staff       (20)     1170 2024-01-05 17:02:38.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain.egg-info/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)     2389 2024-01-05 17:02:38.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain.egg-info/SOURCES.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-01-05 17:02:38.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain.egg-info/dependency_links.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       89 2024-01-05 17:02:38.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain.egg-info/requires.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       20 2024-01-05 17:02:38.000000 xchainpy2_thorchain-0.0.7/xchainpy2_thorchain.egg-info/top_level.txt
```

### Comparing `xchainpy2_thorchain-0.0.6/LICENSE` & `xchainpy2_thorchain-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/PKG-INFO` & `xchainpy2_thorchain-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2_thorchain
-Version: 0.0.6
+Version: 0.0.7
 Summary: XChainPy2 THORChain Client
 Author-email: Tirinox <developer@tirinox.ru>
 License: MIT
 Project-URL: source, https://github.com/tirinox/xchainpy
 Keywords: Crypto,THORChain,Blockchain,XChain
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `xchainpy2_thorchain-0.0.6/pyproject.toml` & `xchainpy2_thorchain-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xchainpy2_thorchain"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name = "Tirinox", email = "developer@tirinox.ru" },
 ]
 description = "XChainPy2 THORChain Client"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["Crypto", "THORChain", "Blockchain", "XChain"]
```

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/client.py` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,16 +262,16 @@
     async def get_fees(self, cache=None, tc_fee_rate=None) -> Fees:
         return single_fee(FeeType.FLAT_FEE, DEFAULT_RUNE_FEE)
 
     def parse_denom_to_asset(self, denom: str) -> Asset:
         if SYNTH_DELIMITER in denom:
             # special case for synths
             return Asset.from_string(denom.upper())
-        else:
-            return super().parse_denom_to_asset(denom)
+        elif denom == DENOM_RUNE_NATIVE:
+            return AssetRUNE
 
     def get_denom(self, asset: Asset) -> str:
         if asset == AssetRUNE:
             return DENOM_RUNE_NATIVE
         else:
             return str(asset).lower()
```

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/const.py` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/const.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/models.py` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/models.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/cosmos/base/v1beta1/coin_pb2.py` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/cosmos/base/v1beta1/coin_pb2.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/cosmos/base/v1beta1/coin_pb2.pyi` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/cosmos/base/v1beta1/coin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/gogoproto/gogo_pb2.py` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/gogoproto/gogo_pb2.pyi` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/gogoproto/gogo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/common/common_pb2.py` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/common/common_pb2.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/common/common_pb2.pyi` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/common/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_deposit_pb2.py` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_deposit_pb2.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_deposit_pb2.pyi` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_deposit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_send_pb2.py` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_send_pb2.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_send_pb2.pyi` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/proto/thorchain/v1/x/thorchain/types/msg_send_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/tests/mock/samples/tx/bond-tn-8F241485970BE3CFCDE21A1F9C8E1EDD42DFF2F78B9B17358E2F81276F46173C.json` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/tests/mock/samples/tx/bond-tn-8F241485970BE3CFCDE21A1F9C8E1EDD42DFF2F78B9B17358E2F81276F46173C.json`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/tests/mock/samples/tx/send-DBEE3FF8DC82EBB490ECE26FD761955BD6E3740BE064E8D5D27CB5F618BE6360.json` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/tests/mock/samples/tx/send-DBEE3FF8DC82EBB490ECE26FD761955BD6E3740BE064E8D5D27CB5F618BE6360.json`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/tests/mock/samples/tx/swap-1C10434D59A460FD0BE76C46A333A583B8C7761094E26C0B2548D07A5AF28356.json` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/tests/mock/samples/tx/swap-1C10434D59A460FD0BE76C46A333A583B8C7761094E26C0B2548D07A5AF28356.json`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/tests/test_utils.py` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain/utils.py` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain/utils.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain.egg-info/PKG-INFO` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2_thorchain
-Version: 0.0.6
+Version: 0.0.7
 Summary: XChainPy2 THORChain Client
 Author-email: Tirinox <developer@tirinox.ru>
 License: MIT
 Project-URL: source, https://github.com/tirinox/xchainpy
 Keywords: Crypto,THORChain,Blockchain,XChain
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `xchainpy2_thorchain-0.0.6/xchainpy2_thorchain.egg-info/SOURCES.txt` & `xchainpy2_thorchain-0.0.7/xchainpy2_thorchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

