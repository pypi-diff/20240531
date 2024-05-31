# Comparing `tmp/xchainpy2_mayachain-0.0.14.tar.gz` & `tmp/xchainpy2_mayachain-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchainpy2_mayachain-0.0.14.tar", last modified: Fri May 31 14:24:12 2024, max compression
+gzip compressed data, was "xchainpy2_mayachain-0.0.6.tar", last modified: Wed Jan  3 19:12:21 2024, max compression
```

## Comparing `xchainpy2_mayachain-0.0.14.tar` & `xchainpy2_mayachain-0.0.6.tar`

### file list

```diff
@@ -1,68 +1,58 @@
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.919183 xchainpy2_mayachain-0.0.14/
--rw-r--r--   0 tirinox    (501) staff       (20)     2124 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/LICENSE
--rw-r--r--   0 tirinox    (501) staff       (20)     1177 2024-05-31 14:24:12.918990 xchainpy2_mayachain-0.0.14/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)       75 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/README.md
--rw-r--r--   0 tirinox    (501) staff       (20)     1354 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/pyproject.toml
--rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-05-31 14:24:12.919219 xchainpy2_mayachain-0.0.14/setup.cfg
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.912161 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/
--rw-r--r--   0 tirinox    (501) staff       (20)      107 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)    18281 2024-05-31 12:48:06.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/client.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3173 2024-05-31 12:48:06.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/const.py
--rw-r--r--   0 tirinox    (501) staff       (20)      727 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/models.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.914416 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/mrc20/
--rw-r--r--   0 tirinox    (501) staff       (20)       40 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/mrc20/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5799 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/mrc20/api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      605 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/mrc20/const.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6584 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/mrc20/memo.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7541 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/mrc20/model.py
--rw-r--r--   0 tirinox    (501) staff       (20)      515 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/mrc20/utils.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.914532 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/
--rw-r--r--   0 tirinox    (501) staff       (20)      863 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.914649 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/cosmos/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/cosmos/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.914731 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/cosmos/base/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/cosmos/base/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.915132 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/cosmos/base/v1beta1/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/cosmos/base/v1beta1/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2808 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/cosmos/base/v1beta1/coin_pb2.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1141 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/cosmos/base/v1beta1/coin_pb2.pyi
--rw-r--r--   0 tirinox    (501) staff       (20)      159 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/cosmos/base/v1beta1/coin_pb2_grpc.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.915756 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/gogoproto/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/gogoproto/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7721 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/gogoproto/gogo_pb2.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6847 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/gogoproto/gogo_pb2.pyi
--rw-r--r--   0 tirinox    (501) staff       (20)      159 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/gogoproto/gogo_pb2_grpc.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.915880 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.915958 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.916459 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/common/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/common/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5694 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/common/common_pb2.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2971 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/common/common_pb2.pyi
--rw-r--r--   0 tirinox    (501) staff       (20)      159 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/common/common_pb2_grpc.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.916592 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.916685 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.917744 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/
--rw-r--r--   0 tirinox    (501) staff       (20)        0 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2050 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_deposit_pb2.py
--rw-r--r--   0 tirinox    (501) staff       (20)      902 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_deposit_pb2.pyi
--rw-r--r--   0 tirinox    (501) staff       (20)      159 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_deposit_pb2_grpc.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2304 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_send_pb2.py
--rw-r--r--   0 tirinox    (501) staff       (20)      947 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_send_pb2.pyi
--rw-r--r--   0 tirinox    (501) staff       (20)      159 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_send_pb2_grpc.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.918164 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/tests/
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.918427 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/tests/mock/
--rw-r--r--   0 tirinox    (501) staff       (20)     1323 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/tests/mock/mimir.json
--rw-r--r--   0 tirinox    (501) staff       (20)     3773 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/tests/test_basic_mc.py
--rw-r--r--   0 tirinox    (501) staff       (20)      932 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/tests/test_fee.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2433 2024-05-31 12:48:06.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/tests/test_utils.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3346 2024-03-07 10:37:31.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/utils.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:24:12.918646 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain.egg-info/
--rw-r--r--   0 tirinox    (501) staff       (20)     1177 2024-05-31 14:24:12.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain.egg-info/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)     2325 2024-05-31 14:24:12.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain.egg-info/SOURCES.txt
--rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-05-31 14:24:12.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain.egg-info/dependency_links.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       89 2024-05-31 14:24:12.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain.egg-info/requires.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       20 2024-05-31 14:24:12.000000 xchainpy2_mayachain-0.0.14/xchainpy2_mayachain.egg-info/top_level.txt
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:21.395813 xchainpy2_mayachain-0.0.6/
+-rw-r--r--   0 tirinox    (501) staff       (20)     2124 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/LICENSE
+-rw-r--r--   0 tirinox    (501) staff       (20)     1176 2024-01-03 19:12:21.395552 xchainpy2_mayachain-0.0.6/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)       75 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/README.md
+-rw-r--r--   0 tirinox    (501) staff       (20)     1353 2024-01-03 16:44:16.000000 xchainpy2_mayachain-0.0.6/pyproject.toml
+-rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-01-03 19:12:21.395866 xchainpy2_mayachain-0.0.6/setup.cfg
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:21.388588 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/
+-rw-r--r--   0 tirinox    (501) staff       (20)       86 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    11399 2024-01-03 16:43:19.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/client.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2822 2023-11-23 11:22:19.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/const.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      727 2023-11-24 19:11:50.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/models.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:21.389855 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/
+-rw-r--r--   0 tirinox    (501) staff       (20)       75 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:21.390089 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/cosmos/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/cosmos/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:21.390215 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/cosmos/base/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/cosmos/base/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:21.390878 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/cosmos/base/v1beta1/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/cosmos/base/v1beta1/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2808 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/cosmos/base/v1beta1/coin_pb2.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1141 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/cosmos/base/v1beta1/coin_pb2.pyi
+-rw-r--r--   0 tirinox    (501) staff       (20)      159 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/cosmos/base/v1beta1/coin_pb2_grpc.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:21.391619 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/gogoproto/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/gogoproto/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7721 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/gogoproto/gogo_pb2.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6847 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/gogoproto/gogo_pb2.pyi
+-rw-r--r--   0 tirinox    (501) staff       (20)      159 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/gogoproto/gogo_pb2_grpc.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:21.391831 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:21.391964 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:21.392673 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/common/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/common/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5694 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/common/common_pb2.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2971 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/common/common_pb2.pyi
+-rw-r--r--   0 tirinox    (501) staff       (20)      159 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/common/common_pb2_grpc.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:21.392866 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:21.393005 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:21.394192 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/
+-rw-r--r--   0 tirinox    (501) staff       (20)        0 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2050 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_deposit_pb2.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      902 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_deposit_pb2.pyi
+-rw-r--r--   0 tirinox    (501) staff       (20)      159 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_deposit_pb2_grpc.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2304 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_send_pb2.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      947 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_send_pb2.pyi
+-rw-r--r--   0 tirinox    (501) staff       (20)      159 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_send_pb2_grpc.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:21.394694 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/tests/
+-rw-r--r--   0 tirinox    (501) staff       (20)     2625 2024-01-03 18:27:29.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/tests/test_basic_mc.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4930 2023-11-19 09:49:41.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/tests/test_utils.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3521 2023-12-17 17:49:01.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/utils.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 19:12:21.394977 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain.egg-info/
+-rw-r--r--   0 tirinox    (501) staff       (20)     1176 2024-01-03 19:12:21.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain.egg-info/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)     2035 2024-01-03 19:12:21.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain.egg-info/SOURCES.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-01-03 19:12:21.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain.egg-info/dependency_links.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       89 2024-01-03 19:12:21.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain.egg-info/requires.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       20 2024-01-03 19:12:21.000000 xchainpy2_mayachain-0.0.6/xchainpy2_mayachain.egg-info/top_level.txt
```

### Comparing `xchainpy2_mayachain-0.0.14/LICENSE` & `xchainpy2_mayachain-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xchainpy2_mayachain-0.0.14/PKG-INFO` & `xchainpy2_mayachain-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2_mayachain
-Version: 0.0.14
+Version: 0.0.6
 Summary: XChainPy2 MayaChain Client
 Author-email: Tirinox <developer@tirinox.ru>
 License: MIT
 Project-URL: source, https://github.com/tirinox/xchainpy
 Keywords: Crypto,MayaChain,Blockchain,XChain
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `xchainpy2_mayachain-0.0.14/pyproject.toml` & `xchainpy2_mayachain-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xchainpy2_mayachain"
-version = "0.0.14"
+version = "0.0.6"
 authors = [
     { name = "Tirinox", email = "developer@tirinox.ru" },
 ]
 description = "XChainPy2 MayaChain Client"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["Crypto", "MayaChain", "Blockchain", "XChain"]
```

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/client.py` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 import asyncio
-from typing import Optional, Union, List
+from typing import Optional, Union
 
 from bip_utils import Bech32ChecksumError
-from cosmpy.aerial.client import Coin
 from cosmpy.aerial.tx import Transaction
 from cosmpy.aerial.tx_helpers import SubmittedTx
 
+from xchainpy2_client import AssetInfo, XcTx, TxType, Fees, FeeType, TokenTransfer
 from xchainpy2_client import RootDerivationPaths, FeeBounds
-from xchainpy2_client import XcTx, TxType, Fees, FeeType, TokenTransfer
 from xchainpy2_client.fees import single_fee
 from xchainpy2_cosmos import CosmosGaiaClient, TxLoadException, TxInternalException
 from xchainpy2_cosmos.utils import parse_tx_response_json
 from xchainpy2_crypto import decode_address
-from xchainpy2_mayanode import MimirApi, ApiClient
 from xchainpy2_utils import Chain, NetworkType, CryptoAmount, Amount, remove_0x_prefix, \
     Asset, SYNTH_DELIMITER, CACAO_DECIMAL, AssetCACAO
 from .const import NodeURL, DEFAULT_CHAIN_IDS, DEFAULT_CLIENT_URLS, DENOM_CACAO_NATIVE, ROOT_DERIVATION_PATHS, \
     DEFAULT_GAS_LIMIT_VALUE, DEPOSIT_GAS_LIMIT_VALUE, FALLBACK_CLIENT_URLS, DEFAULT_CACAO_FEE, \
-    make_client_urls_from_ip_address, DEFAULT_MAYA_EXPLORERS, AssetMAYA, DENOM_MAYA, MAYA_DECIMAL, CACAO_DUST
-from .mrc20.api import MayaScanClient, MayaScanException
-from .mrc20.const import is_mrc20, make_mrc20_asset, MRC20_DECIMALS
-from .mrc20.memo import MRC20Memo, MNFTMemo
+    make_client_urls_from_ip_address, DEFAULT_MAYA_EXPLORERS
 from .utils import build_deposit_tx_unsigned, get_maya_address_prefix, build_transfer_tx_draft
 
 
 class MayaChainClient(CosmosGaiaClient):
     @classmethod
     def from_node_ip(cls, ip: str):
         """
-        Initialize MayaChainClient from node IP address.
+        Initialize THORChainClient from node IP address.
         :param ip: IP address of the node
-        :return: MayaChainClient
+        :return: THORChainClient
         """
         return cls(client_urls=make_client_urls_from_ip_address(ip))
 
     def __init__(self,
                  network=NetworkType.MAINNET,
                  phrase: Optional[str] = None,
                  private_key: Union[str, bytes, callable, None] = None,
@@ -54,56 +49,50 @@
         :param fee_bound: Fee bound structure. See: FeeBounds
         :param root_derivation_paths: Dictionary of derivation paths for each network type. See: ROOT_DERIVATION_PATHS
         :param client_urls: Dictionary of client urls for each network type. See: DEFAULT_CLIENT_URLS
         :param chain_ids: Dictionary of chain ids for each network type. See: DEFAULT_CHAIN_IDS
         :param explorer_providers: Dictionary of explorer providers for each network type. See: THOR_EXPLORERS
         :param wallet_index: int (wallet index, default 0) We can derive any number of addresses from a single seed
         """
-        self.mayanode_api_client = ApiClient()
 
         if isinstance(client_urls, NodeURL):
             client_urls = {network: client_urls}
 
-        self._client_urls = client_urls.copy() if client_urls else DEFAULT_CLIENT_URLS.copy()
+        self.client_urls = client_urls.copy() if client_urls else DEFAULT_CLIENT_URLS.copy()
         self.fallback_client_urls = fallback_client_urls.copy() if fallback_client_urls else None
 
         self.chain_ids = chain_ids.copy() if chain_ids else DEFAULT_CHAIN_IDS.copy()
 
         self.explorers = explorer_providers
 
         root_derivation_paths = root_derivation_paths.copy() if root_derivation_paths else ROOT_DERIVATION_PATHS.copy()
         super().__init__(
             network, phrase, private_key, fee_bound, root_derivation_paths,
-            self._client_urls, self.chain_ids, self.explorers, wallet_index
+            self.client_urls, self.chain_ids, self.explorers, wallet_index
         )
-        self._fee_minimum_gas_price = 0
 
         # Tune for MayaChain
         self.chain = Chain.Maya
         self._prefix = get_maya_address_prefix(network)
         self._gas_asset = AssetCACAO
         self._denom = DENOM_CACAO_NATIVE
         self._decimal = CACAO_DECIMAL
         self._gas_limit = DEFAULT_GAS_LIMIT_VALUE
         self._deposit_gas_limit = DEPOSIT_GAS_LIMIT_VALUE
-        self.standard_tx_fee = DEFAULT_CACAO_FEE
 
         self._recreate_client()
         self._make_wallet()
 
-        self.maya_scan = MayaScanClient()
-        self.mayanode_api_client.configuration.host = self._client_urls[self.network].node
-
     @property
     def server_url(self) -> str:
-        return self._client_urls[self.network].node
+        return self.client_urls[self.network].node
 
     @property
     def rpc_url(self) -> str:
-        return self._client_urls[self.network].rpc
+        return self.client_urls[self.network].rpc
 
     def validate_address(self, address: str) -> bool:
         if not super().validate_address(address):
             return False
         try:
             decode_address(address, self._prefix)
             return True
@@ -180,20 +169,20 @@
             tx
         )
 
         return result if return_full_response else result.tx_hash
 
     async def fetch_transaction_from_mayanode_raw(self, tx_hash: str) -> dict:
         """
-        Fetch transaction from MayaNode, try to use fallback client if main client is not available
+        Fetch transaction from THORNode, try to use fallback client if main client is not available
         Url: https://node/mayachain/tx/{tx_hash}
         :param tx_hash: Tx Hash
         :return: Transaction data (raw, unparsed)
         """
-        clients = [self._client_urls[self.network]]
+        clients = [self.client_urls[self.network]]
         if self.fallback_client_urls:
             clients.extend(self.fallback_client_urls[self.network])
 
         exc = None
         for client in clients:
             try:
                 url = f"{client.node}/mayachain/tx/{tx_hash}"
@@ -204,15 +193,15 @@
                 continue
         if exc:
             raise exc
 
     async def get_transaction_data_mayanode(self, tx_id: str) -> XcTx:
         """
         Fetch transaction data from MayaNode (parsed to XcTx instance)
-        This function is used when inbound or outbound tx is not of MayaChain.
+        This function is used when inbound or outbound tx is not of THORChain.
         It is called "getTransactionDataThornode" in xchainjs
         Parsing "observed_tx" object.
         Url: https://node/mayachain/tx/{tx_hash}
         :param tx_id: Tx Hash
         :return: XcTx result
         """
         if not tx_id:
@@ -266,198 +255,32 @@
         """
         try:
             j = await self.get_transaction_data_cosmos(tx_id)
             return parse_tx_response_json(j, tx_id, address, self._decimal, self._denom, self._gas_asset)
         except TxLoadException:
             return await self.get_transaction_data_mayanode(tx_id)
 
-    async def get_fees(self) -> Fees:
-        mimir_api = MimirApi(self.mayanode_api_client)
-        mimir_params = await mimir_api.mimir()
-
-        fee_param = mimir_params.get('NATIVETRANSACTIONFEE')
-        try:
-            fee_param = int(fee_param)
-            if fee_param < 0:
-                raise ValueError
-        except ValueError:
-            raise ValueError(f"Invalid native TX fee in Mimir: {fee_param}")
-
-        return single_fee(FeeType.FLAT_FEE, Amount.from_base(fee_param, self._decimal))
+    async def get_fees(self, cache=None, tc_fee_rate=None) -> Fees:
+        return single_fee(FeeType.FLAT_FEE, DEFAULT_CACAO_FEE)
 
     def parse_denom_to_asset(self, denom: str) -> Asset:
         if SYNTH_DELIMITER in denom:
             # special case for synths
             return Asset.from_string(denom.upper())
-        elif denom == DENOM_MAYA:
-            return AssetMAYA
-        elif denom == DENOM_CACAO_NATIVE:
-            return AssetCACAO
-
-    def convert_coin_to_amount(self, c: Coin) -> CryptoAmount:
-        if c.denom == DENOM_MAYA:
-            decimal = MAYA_DECIMAL
-        elif c.denom == DENOM_CACAO_NATIVE:
-            decimal = CACAO_DECIMAL
         else:
-            decimal = 8
-
-        return CryptoAmount(
-            Amount.from_base(c.amount, decimal),
-            asset=self.parse_denom_to_asset(c.denom)
-        )
+            return super().parse_denom_to_asset(denom)
 
     def get_denom(self, asset: Asset) -> str:
         if asset == AssetCACAO:
             return DENOM_CACAO_NATIVE
-        elif asset == AssetMAYA:
-            return DENOM_MAYA
         else:
             return str(asset).lower()
 
     def build_transfer_tx(self, what: CryptoAmount, recipient: str) -> Transaction:
         self._make_wallet()
         tx = build_transfer_tx_draft(
             what, denom=self.get_denom(what.asset),
             sender=str(self._wallet.address()),
             recipient=recipient,
             prefix=self.prefix,
         )
         return tx
-
-    def _maya_scan_tx_value_cacao(self):
-        return self.gas_amount(CACAO_DUST)
-
-    async def transfer_mrc20(self, what: CryptoAmount, recipient: str):
-        """
-        Transfer MRC20 token
-        Example: await maya.transfer_mrc20(CryptoAmount.automatic(100, 'MRC20.GLD'), 'maya1f4f2a4b24')
-        :param what: CryptoAmount
-        :param recipient: maya1Address
-        :return: TX hash string
-        """
-        if not self.validate_address(recipient):
-            raise ValueError(f"Invalid recipient address: {recipient}")
-
-        if not is_mrc20(what.asset):
-            raise ValueError(f"Asset {what.asset} is not MRC20")
-
-        memo = MRC20Memo.transfer(what.asset.symbol, what.amount)
-
-        return await self._mrc20_submit_tx(memo, recipient)
-
-    async def transfer_mnft(self, symbol: str, ident: int, recipient: str):
-        """
-        Transfer MNFT token
-        Example: await maya.transfer_mnft('PEPE', 25, 'maya1f4f2a4b24')
-        :param symbol: MNFT ticker
-        :param ident: MNFT token ID
-        :param recipient: maya1Address
-        :return: TX hash string
-        """
-        if not self.validate_address(recipient):
-            raise ValueError(f"Invalid recipient address: {recipient}")
-
-        memo = MNFTMemo.transfer(symbol, ident)
-
-        return await self.transfer(
-            self._maya_scan_tx_value_cacao(),
-            recipient, memo=memo,
-            check_balance=False,
-        )
-
-    @staticmethod
-    def amount_of_mrc20(amount, asset_name: str):
-        return CryptoAmount.automatic(amount, make_mrc20_asset(asset_name))
-
-    async def close(self):
-        if self.maya_scan:
-            await self.maya_scan.close()
-
-    async def transfer(self, what: CryptoAmount, recipient: str, memo: Optional[str] = None,
-                       fee_rate: Optional[int] = None, check_balance: bool = True) -> str:
-        if is_mrc20(what.asset):
-            return await self.transfer_mrc20(what, recipient)
-        else:
-            return await super().transfer(what, recipient, memo, fee_rate, check_balance)
-
-    transfer.__doc__ = CosmosGaiaClient.transfer.__doc__
-
-    async def get_balance(self, address: str = '', include_mrc20=True) -> List[CryptoAmount]:
-        if not address:
-            address = self.get_address()
-
-        on_chain_balances = await super().get_balance(address)
-        if include_mrc20:
-            try:
-                mrc20_balances = await self.maya_scan.get_balance(address)
-                mrc20_balances = [
-                    CryptoAmount(Amount.from_base(b.balance, b.decimals), make_mrc20_asset(b.ticker))
-                    for b in mrc20_balances
-                ]
-                on_chain_balances.extend(mrc20_balances)
-            except MayaScanException as e:
-                # "not found" means zero balances, that is OK
-                if not e.is_not_found:
-                    raise
-
-        return on_chain_balances
-
-    get_balance.__doc__ = CosmosGaiaClient.get_balance.__doc__
-
-    async def _mrc20_submit_tx(self, memo: str, recipient=''):
-        if not recipient:
-            recipient = self.get_address()
-        return await self.transfer(
-            self._maya_scan_tx_value_cacao(),
-            recipient, memo=memo,
-            check_balance=False,
-        )
-
-    async def mrc20_cancel_order(self, ticker: Union[str, Asset], tx_hash: str):
-        """
-        Cancel MRC20 sell order
-        :param ticker: ticker of MRC20 token (e.g. GLD)
-        :param tx_hash: exact hash of the transaction that created the order
-        :return: txid of the cancel transaction
-        """
-        memo = MRC20Memo.cancel(ticker, tx_hash)
-        return await self._mrc20_submit_tx(memo)
-
-    async def mrc20_sell(self, ticker: Union[str, Asset], amount: Union[CryptoAmount, Amount, int, float],
-                         price: float):
-        """
-        Post an order to sell MRC20 token
-        :param ticker: ticker of MRC20 token (e.g. GLD)
-        :param amount: amount of MRC20 token to sell
-        :param price: price of MRC20 token in CACAO
-        :return: txid of the sell transaction
-        """
-        amount = Amount.automatic(amount, MRC20_DECIMALS)
-        price = Amount.automatic(price, MRC20_DECIMALS)
-
-        memo = MRC20Memo.sell(ticker, int(amount), int(price))
-        return await self._mrc20_submit_tx(memo)
-
-    async def mrc20_buy(self, ticker: Union[str, Asset],
-                        amount: Union[CryptoAmount, Amount, int, float],
-                        seller_address: str,
-                        tx_hash: str):
-        """
-        Buy MRC20 token from the seller
-        :param ticker: ticker of MRC20 token (e.g. GLD)
-        :param amount: amount of MRC20 token to buy
-        :param seller_address: seller address
-        :param tx_hash: exact hash of the transaction that created the order
-        :return: txid of the buy transaction
-        """
-        if not tx_hash:
-            raise ValueError("tx_hash of the selling tx is not specified")
-
-        if not self.validate_address(seller_address):
-            raise ValueError(f"Invalid seller address: {seller_address}")
-        amount = Amount.automatic(amount, MRC20_DECIMALS)
-        memo = MRC20Memo.buy(ticker, amount, tx_hash)
-        return await self._mrc20_submit_tx(memo, recipient=seller_address)
-
-    async def wait_for_transaction(self, tx_id: str):
-        raise NotImplemented
```

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/const.py` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/const.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-from decimal import Decimal
-
 from xchainpy2_client import ExplorerProvider
-from xchainpy2_utils import Asset, Amount, CryptoAmount, AssetCACAO
+from xchainpy2_utils import Asset, Amount
 from xchainpy2_utils.consts import NetworkType, CACAO_DECIMAL
 from .models import NodeURL
 
 DEFAULT_GAS_ADJUSTMENT = 2
-DEFAULT_GAS_LIMIT_VALUE = 4_000_000
-DEPOSIT_GAS_LIMIT_VALUE = 600_000_000
+DEFAULT_GAS_LIMIT_VALUE = '4000000'
+DEPOSIT_GAS_LIMIT_VALUE = '600000000'
 
 MAX_TX_COUNT_PER_PAGE = 100
 
 MAX_TX_COUNT_PER_FUNCTION_CALL = 500
 
 MAX_PAGES_PER_FUNCTION_CALL = 15
 
 RUNE_SYMBOL = 'C'
 CACAO_TICKER = 'CACAO'
 DENOM_CACAO_NATIVE = 'cacao'
 
 MAYA_DECIMAL = 4
 DENOM_MAYA = 'maya'
 
-AssetMAYA = Asset.from_string('MAYA.MAYA')
-
-DEFAULT_CACAO_NETWORK_FEE = CryptoAmount(Amount.from_asset(Decimal("0.5"), CACAO_DECIMAL), AssetCACAO)
+AssetMAYA = Asset.from_string('MAYA.CACAO')
 
-DEFAULT_CACAO_FEE = Amount.from_asset(0.5, CACAO_DECIMAL)
+DEFAULT_CACAO_FEE = Amount.from_asset(0.02, CACAO_DECIMAL)
 
 DEFAULT_EXPLORER_URL = 'https://explorer.mayachain.info{path}{network_tag}'
 MAYASCAN_EXPLORER_URL = 'https://mayascan.org{path}'
 
 
 def make_explorer_object(network_tag: str, base_url=MAYASCAN_EXPLORER_URL):
     return ExplorerProvider(
@@ -90,23 +86,14 @@
     NetworkType.STAGENET: NodeURL(
         'https://stagenet.mayanode.mayachain.info',
         'https://stagenet.mayachain.info/'
     ),
     NetworkType.TESTNET: NodeURL('deprecated', 'deprecated'),
 }
 
-MAYA_LIQUIFY_NODE_URL = NodeURL(
-    "https://api-maya.liquify.com/",
-    "https://rpc-maya.liquify.com/"
-)
-
-MAYA_LIQUIFY_MIDGARD_URL = "https://midgard-maya.liquify.com"
-
 FALLBACK_CLIENT_URLS = {
     NetworkType.MAINNET: [],
     NetworkType.STAGENET: [],
     NetworkType.TESTNET: []
 }
 
-MAYA_BLOCK_TIME_SEC = 6.0
-
-CACAO_DUST = 0.0001
+MAYA_BLOCK_TIME_SEC = 6.0
```

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/models.py` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/models.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/cosmos/base/v1beta1/coin_pb2.py` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/cosmos/base/v1beta1/coin_pb2.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/cosmos/base/v1beta1/coin_pb2.pyi` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/cosmos/base/v1beta1/coin_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/gogoproto/gogo_pb2.py` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/gogoproto/gogo_pb2.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/gogoproto/gogo_pb2.pyi` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/gogoproto/gogo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/common/common_pb2.py` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/common/common_pb2.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/common/common_pb2.pyi` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/common/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_deposit_pb2.py` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_deposit_pb2.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_deposit_pb2.pyi` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_deposit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_send_pb2.py` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_send_pb2.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_send_pb2.pyi` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_send_pb2.pyi`

 * *Files identical despite different names*

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain/utils.py` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from cosmpy.aerial.tx import Transaction, SigningCfg
 from cosmpy.crypto.keypairs import PublicKey
 
 from xchainpy2_cosmos.utils import convert_address_for_msg
 from xchainpy2_utils import NetworkType, CryptoAmount, Amount, Asset, CACAO_DECIMAL, AssetCACAO
 from .const import DEPOSIT_GAS_LIMIT_VALUE, DENOM_CACAO_NATIVE
 from .proto.cosmos.base.v1beta1.coin_pb2 import Coin
-from .proto import THORCoin, THORAsset, MsgSend, MsgDeposit
+from .proto.mayachain.v1.common.common_pb2 import Coin as THORCoin, Asset as THORAsset
+from .proto.mayachain.v1.x.mayachain.types.msg_deposit_pb2 import MsgDeposit
+from .proto.mayachain.v1.x.mayachain.types.msg_send_pb2 import MsgSend
 
 
 def get_maya_address_prefix(network: NetworkType) -> str:
     """
     Get address prefix based on the network.
     :param network:
     :return: string address prefix
```

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain.egg-info/PKG-INFO` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2_mayachain
-Version: 0.0.14
+Version: 0.0.6
 Summary: XChainPy2 MayaChain Client
 Author-email: Tirinox <developer@tirinox.ru>
 License: MIT
 Project-URL: source, https://github.com/tirinox/xchainpy
 Keywords: Crypto,MayaChain,Blockchain,XChain
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `xchainpy2_mayachain-0.0.14/xchainpy2_mayachain.egg-info/SOURCES.txt` & `xchainpy2_mayachain-0.0.6/xchainpy2_mayachain.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,20 +7,14 @@
 xchainpy2_mayachain/models.py
 xchainpy2_mayachain/utils.py
 xchainpy2_mayachain.egg-info/PKG-INFO
 xchainpy2_mayachain.egg-info/SOURCES.txt
 xchainpy2_mayachain.egg-info/dependency_links.txt
 xchainpy2_mayachain.egg-info/requires.txt
 xchainpy2_mayachain.egg-info/top_level.txt
-xchainpy2_mayachain/mrc20/__init__.py
-xchainpy2_mayachain/mrc20/api.py
-xchainpy2_mayachain/mrc20/const.py
-xchainpy2_mayachain/mrc20/memo.py
-xchainpy2_mayachain/mrc20/model.py
-xchainpy2_mayachain/mrc20/utils.py
 xchainpy2_mayachain/proto/__init__.py
 xchainpy2_mayachain/proto/cosmos/__init__.py
 xchainpy2_mayachain/proto/cosmos/base/__init__.py
 xchainpy2_mayachain/proto/cosmos/base/v1beta1/__init__.py
 xchainpy2_mayachain/proto/cosmos/base/v1beta1/coin_pb2.py
 xchainpy2_mayachain/proto/cosmos/base/v1beta1/coin_pb2.pyi
 xchainpy2_mayachain/proto/cosmos/base/v1beta1/coin_pb2_grpc.py
@@ -40,10 +34,8 @@
 xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_deposit_pb2.py
 xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_deposit_pb2.pyi
 xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_deposit_pb2_grpc.py
 xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_send_pb2.py
 xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_send_pb2.pyi
 xchainpy2_mayachain/proto/mayachain/v1/x/mayachain/types/msg_send_pb2_grpc.py
 xchainpy2_mayachain/tests/test_basic_mc.py
-xchainpy2_mayachain/tests/test_fee.py
-xchainpy2_mayachain/tests/test_utils.py
-xchainpy2_mayachain/tests/mock/mimir.json
+xchainpy2_mayachain/tests/test_utils.py
```

