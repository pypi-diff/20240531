# Comparing `tmp/vana-0.1.0.tar.gz` & `tmp/vana-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vana-0.1.0.tar", max compression
+gzip compressed data, was "vana-0.1.1.tar", max compression
```

## Comparing `vana-0.1.0.tar` & `vana-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     6035 2024-05-30 18:49:07.454501 vana-0.1.0/README.md
--rw-r--r--   0        0        0      817 2024-05-30 18:49:07.458501 vana-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3944 2024-05-30 18:49:07.458501 vana-0.1.0/vana/__init__.py
--rw-r--r--   0        0        0     3432 2024-05-30 18:49:07.458501 vana-0.1.0/vana/chain_data.py
--rw-r--r--   0        0        0    19126 2024-05-30 18:49:07.458501 vana-0.1.0/vana/chain_manager.py
--rw-r--r--   0        0        0    10014 2024-05-30 18:49:07.458501 vana-0.1.0/vana/cli.py
--rw-r--r--   0        0        0     1924 2024-05-30 18:49:07.458501 vana-0.1.0/vana/commands/__init__.py
--rw-r--r--   0        0        0     5685 2024-05-30 18:49:07.458501 vana-0.1.0/vana/commands/transfer.py
--rw-r--r--   0        0        0    41105 2024-05-30 18:49:07.458501 vana-0.1.0/vana/commands/wallets.py
--rw-r--r--   0        0        0    15159 2024-05-30 18:49:07.458501 vana-0.1.0/vana/config.py
--rw-r--r--   0        0        0     3788 2024-05-30 18:49:07.458501 vana-0.1.0/vana/errors.py
--rw-r--r--   0        0        0    30954 2024-05-30 18:49:07.458501 vana-0.1.0/vana/keyfile.py
--rw-r--r--   0        0        0     1691 2024-05-30 18:49:07.458501 vana-0.1.0/vana/logging/__init__.py
--rw-r--r--   0        0        0     1474 2024-05-30 18:49:07.458501 vana-0.1.0/vana/logging/defines.py
--rw-r--r--   0        0        0     4742 2024-05-30 18:49:07.458501 vana-0.1.0/vana/logging/format.py
--rw-r--r--   0        0        0     2747 2024-05-30 18:49:07.458501 vana-0.1.0/vana/logging/helpers.py
--rw-r--r--   0        0        0    14307 2024-05-30 18:49:07.458501 vana-0.1.0/vana/logging/loggingmachine.py
--rw-r--r--   0        0        0    35119 2024-05-30 18:49:07.458501 vana-0.1.0/vana/message.py
--rw-r--r--   0        0        0        0 2024-05-30 18:49:07.458501 vana-0.1.0/vana/mock/__init__.py
--rw-r--r--   0        0        0     3266 2024-05-30 18:49:07.458501 vana-0.1.0/vana/mock/keyfile_mock.py
--rw-r--r--   0        0        0     4795 2024-05-30 18:49:07.458501 vana-0.1.0/vana/mock/wallet_mock.py
--rw-r--r--   0        0        0    19318 2024-05-30 18:49:07.458501 vana-0.1.0/vana/node_client.py
--rw-r--r--   0        0        0    13715 2024-05-30 18:49:07.458501 vana-0.1.0/vana/node_server.py
--rw-r--r--   0        0        0     6272 2024-05-30 18:49:07.458501 vana-0.1.0/vana/state.py
--rw-r--r--   0        0        0    10203 2024-05-30 18:49:07.458501 vana-0.1.0/vana/threadpool.py
--rw-r--r--   0        0        0     1399 2024-05-30 18:49:07.458501 vana-0.1.0/vana/utils/__init__.py
--rw-r--r--   0        0        0     5035 2024-05-30 18:49:07.458501 vana-0.1.0/vana/utils/fast_api_threaded_server.py
--rw-r--r--   0        0        0     1426 2024-05-30 18:49:07.458501 vana-0.1.0/vana/utils/misc.py
--rw-r--r--   0        0        0     5703 2024-05-30 18:49:07.458501 vana-0.1.0/vana/utils/networking.py
--rw-r--r--   0        0        0     5377 2024-05-30 18:49:07.458501 vana-0.1.0/vana/utils/wallet_utils.py
--rw-r--r--   0        0        0    30123 2024-05-30 18:49:07.458501 vana-0.1.0/vana/wallet.py
--rw-r--r--   0        0        0     7247 1970-01-01 00:00:00.000000 vana-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6035 2024-05-30 21:44:10.660242 vana-0.1.1/README.md
+-rw-r--r--   0        0        0      817 2024-05-30 21:44:10.660242 vana-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3944 2024-05-30 21:44:10.660242 vana-0.1.1/vana/__init__.py
+-rw-r--r--   0        0        0     3432 2024-05-30 21:44:10.660242 vana-0.1.1/vana/chain_data.py
+-rw-r--r--   0        0        0    19126 2024-05-30 21:44:10.660242 vana-0.1.1/vana/chain_manager.py
+-rw-r--r--   0        0        0    10014 2024-05-30 21:44:10.660242 vana-0.1.1/vana/cli.py
+-rw-r--r--   0        0        0     1924 2024-05-30 21:44:10.660242 vana-0.1.1/vana/commands/__init__.py
+-rw-r--r--   0        0        0     5685 2024-05-30 21:44:10.660242 vana-0.1.1/vana/commands/transfer.py
+-rw-r--r--   0        0        0    41105 2024-05-30 21:44:10.660242 vana-0.1.1/vana/commands/wallets.py
+-rw-r--r--   0        0        0    15159 2024-05-30 21:44:10.664242 vana-0.1.1/vana/config.py
+-rw-r--r--   0        0        0     3788 2024-05-30 21:44:10.664242 vana-0.1.1/vana/errors.py
+-rw-r--r--   0        0        0    30954 2024-05-30 21:44:10.664242 vana-0.1.1/vana/keyfile.py
+-rw-r--r--   0        0        0     1691 2024-05-30 21:44:10.664242 vana-0.1.1/vana/logging/__init__.py
+-rw-r--r--   0        0        0     1474 2024-05-30 21:44:10.664242 vana-0.1.1/vana/logging/defines.py
+-rw-r--r--   0        0        0     4742 2024-05-30 21:44:10.664242 vana-0.1.1/vana/logging/format.py
+-rw-r--r--   0        0        0     2747 2024-05-30 21:44:10.664242 vana-0.1.1/vana/logging/helpers.py
+-rw-r--r--   0        0        0    14307 2024-05-30 21:44:10.664242 vana-0.1.1/vana/logging/loggingmachine.py
+-rw-r--r--   0        0        0    35119 2024-05-30 21:44:10.664242 vana-0.1.1/vana/message.py
+-rw-r--r--   0        0        0        0 2024-05-30 21:44:10.664242 vana-0.1.1/vana/mock/__init__.py
+-rw-r--r--   0        0        0     3266 2024-05-30 21:44:10.664242 vana-0.1.1/vana/mock/keyfile_mock.py
+-rw-r--r--   0        0        0     4795 2024-05-30 21:44:10.664242 vana-0.1.1/vana/mock/wallet_mock.py
+-rw-r--r--   0        0        0    19318 2024-05-30 21:44:10.664242 vana-0.1.1/vana/node_client.py
+-rw-r--r--   0        0        0    13715 2024-05-30 21:44:10.664242 vana-0.1.1/vana/node_server.py
+-rw-r--r--   0        0        0     6272 2024-05-30 21:44:10.664242 vana-0.1.1/vana/state.py
+-rw-r--r--   0        0        0    10203 2024-05-30 21:44:10.664242 vana-0.1.1/vana/threadpool.py
+-rw-r--r--   0        0        0     1399 2024-05-30 21:44:10.664242 vana-0.1.1/vana/utils/__init__.py
+-rw-r--r--   0        0        0     5035 2024-05-30 21:44:10.664242 vana-0.1.1/vana/utils/fast_api_threaded_server.py
+-rw-r--r--   0        0        0     1426 2024-05-30 21:44:10.664242 vana-0.1.1/vana/utils/misc.py
+-rw-r--r--   0        0        0     5703 2024-05-30 21:44:10.664242 vana-0.1.1/vana/utils/networking.py
+-rw-r--r--   0        0        0     5377 2024-05-30 21:44:10.664242 vana-0.1.1/vana/utils/wallet_utils.py
+-rw-r--r--   0        0        0    30123 2024-05-30 21:44:10.664242 vana-0.1.1/vana/wallet.py
+-rw-r--r--   0        0        0     7247 1970-01-01 00:00:00.000000 vana-0.1.1/PKG-INFO
```

### Comparing `vana-0.1.0/README.md` & `vana-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/pyproject.toml` & `vana-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vana"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Tim Nunamaker <tim@vana.com>", "Volodymyr Isai <volod@vana.com>", "Kahtaf Alam <kahtaf@vana.com>"]
 readme = "README.md"
 repository = "https://github.com/vana-com/vana-framework"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
```

### Comparing `vana-0.1.0/vana/__init__.py` & `vana-0.1.1/vana/__init__.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/chain_data.py` & `vana-0.1.1/vana/chain_data.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/chain_manager.py` & `vana-0.1.1/vana/chain_manager.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/cli.py` & `vana-0.1.1/vana/cli.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/commands/__init__.py` & `vana-0.1.1/vana/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/commands/transfer.py` & `vana-0.1.1/vana/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/commands/wallets.py` & `vana-0.1.1/vana/commands/wallets.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/config.py` & `vana-0.1.1/vana/config.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/errors.py` & `vana-0.1.1/vana/errors.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/keyfile.py` & `vana-0.1.1/vana/keyfile.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/logging/__init__.py` & `vana-0.1.1/vana/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/logging/defines.py` & `vana-0.1.1/vana/logging/defines.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/logging/format.py` & `vana-0.1.1/vana/logging/format.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/logging/helpers.py` & `vana-0.1.1/vana/logging/helpers.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/logging/loggingmachine.py` & `vana-0.1.1/vana/logging/loggingmachine.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/message.py` & `vana-0.1.1/vana/message.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/mock/keyfile_mock.py` & `vana-0.1.1/vana/mock/keyfile_mock.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/mock/wallet_mock.py` & `vana-0.1.1/vana/mock/wallet_mock.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/node_client.py` & `vana-0.1.1/vana/node_client.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/node_server.py` & `vana-0.1.1/vana/node_server.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/state.py` & `vana-0.1.1/vana/state.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/threadpool.py` & `vana-0.1.1/vana/threadpool.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/utils/__init__.py` & `vana-0.1.1/vana/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/utils/fast_api_threaded_server.py` & `vana-0.1.1/vana/utils/fast_api_threaded_server.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/utils/misc.py` & `vana-0.1.1/vana/utils/misc.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/utils/networking.py` & `vana-0.1.1/vana/utils/networking.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/utils/wallet_utils.py` & `vana-0.1.1/vana/utils/wallet_utils.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/vana/wallet.py` & `vana-0.1.1/vana/wallet.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.0/PKG-INFO` & `vana-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vana
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Home-page: https://github.com/vana-com/vana-framework
 Author: Tim Nunamaker
 Author-email: tim@vana.com
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

