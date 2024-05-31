# Comparing `tmp/vana-0.1.1.tar.gz` & `tmp/vana-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vana-0.1.1.tar", max compression
+gzip compressed data, was "vana-0.1.2.tar", max compression
```

## Comparing `vana-0.1.1.tar` & `vana-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     6035 2024-05-30 21:44:10.660242 vana-0.1.1/README.md
--rw-r--r--   0        0        0      817 2024-05-30 21:44:10.660242 vana-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3944 2024-05-30 21:44:10.660242 vana-0.1.1/vana/__init__.py
--rw-r--r--   0        0        0     3432 2024-05-30 21:44:10.660242 vana-0.1.1/vana/chain_data.py
--rw-r--r--   0        0        0    19126 2024-05-30 21:44:10.660242 vana-0.1.1/vana/chain_manager.py
--rw-r--r--   0        0        0    10014 2024-05-30 21:44:10.660242 vana-0.1.1/vana/cli.py
--rw-r--r--   0        0        0     1924 2024-05-30 21:44:10.660242 vana-0.1.1/vana/commands/__init__.py
--rw-r--r--   0        0        0     5685 2024-05-30 21:44:10.660242 vana-0.1.1/vana/commands/transfer.py
--rw-r--r--   0        0        0    41105 2024-05-30 21:44:10.660242 vana-0.1.1/vana/commands/wallets.py
--rw-r--r--   0        0        0    15159 2024-05-30 21:44:10.664242 vana-0.1.1/vana/config.py
--rw-r--r--   0        0        0     3788 2024-05-30 21:44:10.664242 vana-0.1.1/vana/errors.py
--rw-r--r--   0        0        0    30954 2024-05-30 21:44:10.664242 vana-0.1.1/vana/keyfile.py
--rw-r--r--   0        0        0     1691 2024-05-30 21:44:10.664242 vana-0.1.1/vana/logging/__init__.py
--rw-r--r--   0        0        0     1474 2024-05-30 21:44:10.664242 vana-0.1.1/vana/logging/defines.py
--rw-r--r--   0        0        0     4742 2024-05-30 21:44:10.664242 vana-0.1.1/vana/logging/format.py
--rw-r--r--   0        0        0     2747 2024-05-30 21:44:10.664242 vana-0.1.1/vana/logging/helpers.py
--rw-r--r--   0        0        0    14307 2024-05-30 21:44:10.664242 vana-0.1.1/vana/logging/loggingmachine.py
--rw-r--r--   0        0        0    35119 2024-05-30 21:44:10.664242 vana-0.1.1/vana/message.py
--rw-r--r--   0        0        0        0 2024-05-30 21:44:10.664242 vana-0.1.1/vana/mock/__init__.py
--rw-r--r--   0        0        0     3266 2024-05-30 21:44:10.664242 vana-0.1.1/vana/mock/keyfile_mock.py
--rw-r--r--   0        0        0     4795 2024-05-30 21:44:10.664242 vana-0.1.1/vana/mock/wallet_mock.py
--rw-r--r--   0        0        0    19318 2024-05-30 21:44:10.664242 vana-0.1.1/vana/node_client.py
--rw-r--r--   0        0        0    13715 2024-05-30 21:44:10.664242 vana-0.1.1/vana/node_server.py
--rw-r--r--   0        0        0     6272 2024-05-30 21:44:10.664242 vana-0.1.1/vana/state.py
--rw-r--r--   0        0        0    10203 2024-05-30 21:44:10.664242 vana-0.1.1/vana/threadpool.py
--rw-r--r--   0        0        0     1399 2024-05-30 21:44:10.664242 vana-0.1.1/vana/utils/__init__.py
--rw-r--r--   0        0        0     5035 2024-05-30 21:44:10.664242 vana-0.1.1/vana/utils/fast_api_threaded_server.py
--rw-r--r--   0        0        0     1426 2024-05-30 21:44:10.664242 vana-0.1.1/vana/utils/misc.py
--rw-r--r--   0        0        0     5703 2024-05-30 21:44:10.664242 vana-0.1.1/vana/utils/networking.py
--rw-r--r--   0        0        0     5377 2024-05-30 21:44:10.664242 vana-0.1.1/vana/utils/wallet_utils.py
--rw-r--r--   0        0        0    30123 2024-05-30 21:44:10.664242 vana-0.1.1/vana/wallet.py
--rw-r--r--   0        0        0     7247 1970-01-01 00:00:00.000000 vana-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6035 2024-05-31 15:19:05.195216 vana-0.1.2/README.md
+-rw-r--r--   0        0        0      835 2024-05-31 15:19:05.195216 vana-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3944 2024-05-31 15:19:05.195216 vana-0.1.2/vana/__init__.py
+-rw-r--r--   0        0        0     3432 2024-05-31 15:19:05.195216 vana-0.1.2/vana/chain_data.py
+-rw-r--r--   0        0        0    19126 2024-05-31 15:19:05.195216 vana-0.1.2/vana/chain_manager.py
+-rw-r--r--   0        0        0    10014 2024-05-31 15:19:05.195216 vana-0.1.2/vana/cli.py
+-rw-r--r--   0        0        0     1924 2024-05-31 15:19:05.195216 vana-0.1.2/vana/commands/__init__.py
+-rw-r--r--   0        0        0     5685 2024-05-31 15:19:05.199216 vana-0.1.2/vana/commands/transfer.py
+-rw-r--r--   0        0        0    41119 2024-05-31 15:19:05.199216 vana-0.1.2/vana/commands/wallets.py
+-rw-r--r--   0        0        0    15159 2024-05-31 15:19:05.199216 vana-0.1.2/vana/config.py
+-rw-r--r--   0        0        0     3788 2024-05-31 15:19:05.199216 vana-0.1.2/vana/errors.py
+-rw-r--r--   0        0        0    30954 2024-05-31 15:19:05.199216 vana-0.1.2/vana/keyfile.py
+-rw-r--r--   0        0        0     1691 2024-05-31 15:19:05.199216 vana-0.1.2/vana/logging/__init__.py
+-rw-r--r--   0        0        0     1474 2024-05-31 15:19:05.199216 vana-0.1.2/vana/logging/defines.py
+-rw-r--r--   0        0        0     4742 2024-05-31 15:19:05.199216 vana-0.1.2/vana/logging/format.py
+-rw-r--r--   0        0        0     2747 2024-05-31 15:19:05.199216 vana-0.1.2/vana/logging/helpers.py
+-rw-r--r--   0        0        0    14307 2024-05-31 15:19:05.199216 vana-0.1.2/vana/logging/loggingmachine.py
+-rw-r--r--   0        0        0    35119 2024-05-31 15:19:05.199216 vana-0.1.2/vana/message.py
+-rw-r--r--   0        0        0        0 2024-05-31 15:19:05.199216 vana-0.1.2/vana/mock/__init__.py
+-rw-r--r--   0        0        0     3266 2024-05-31 15:19:05.199216 vana-0.1.2/vana/mock/keyfile_mock.py
+-rw-r--r--   0        0        0     4795 2024-05-31 15:19:05.199216 vana-0.1.2/vana/mock/wallet_mock.py
+-rw-r--r--   0        0        0    19318 2024-05-31 15:19:05.199216 vana-0.1.2/vana/node_client.py
+-rw-r--r--   0        0        0    13715 2024-05-31 15:19:05.199216 vana-0.1.2/vana/node_server.py
+-rw-r--r--   0        0        0     6272 2024-05-31 15:19:05.199216 vana-0.1.2/vana/state.py
+-rw-r--r--   0        0        0    10203 2024-05-31 15:19:05.199216 vana-0.1.2/vana/threadpool.py
+-rw-r--r--   0        0        0     1399 2024-05-31 15:19:05.199216 vana-0.1.2/vana/utils/__init__.py
+-rw-r--r--   0        0        0     5035 2024-05-31 15:19:05.199216 vana-0.1.2/vana/utils/fast_api_threaded_server.py
+-rw-r--r--   0        0        0     1426 2024-05-31 15:19:05.199216 vana-0.1.2/vana/utils/misc.py
+-rw-r--r--   0        0        0     5703 2024-05-31 15:19:05.199216 vana-0.1.2/vana/utils/networking.py
+-rw-r--r--   0        0        0     5377 2024-05-31 15:19:05.199216 vana-0.1.2/vana/utils/wallet_utils.py
+-rw-r--r--   0        0        0    30123 2024-05-31 15:19:05.199216 vana-0.1.2/vana/wallet.py
+-rw-r--r--   0        0        0     7286 1970-01-01 00:00:00.000000 vana-0.1.2/PKG-INFO
```

### Comparing `vana-0.1.1/README.md` & `vana-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/pyproject.toml` & `vana-0.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vana"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Tim Nunamaker <tim@vana.com>", "Volodymyr Isai <volod@vana.com>", "Kahtaf Alam <kahtaf@vana.com>"]
 readme = "README.md"
 repository = "https://github.com/vana-com/vana-framework"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.13"
@@ -22,14 +22,15 @@
 ansible-vault = "^2.1.0"
 ansible = "^9.5.1"
 password-strength = "^0.0.3.post2"
 rich = "^13.7.1"
 netaddr = "^1.2.1"
 web3 = "^6.18.0"
 shtab = "^1.7.1"
+pynacl = "^1.5.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `vana-0.1.1/vana/__init__.py` & `vana-0.1.2/vana/__init__.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/chain_data.py` & `vana-0.1.2/vana/chain_data.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/chain_manager.py` & `vana-0.1.2/vana/chain_manager.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/cli.py` & `vana-0.1.2/vana/cli.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/commands/__init__.py` & `vana-0.1.2/vana/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/commands/transfer.py` & `vana-0.1.2/vana/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/commands/wallets.py` & `vana-0.1.2/vana/commands/wallets.py`

 * *Files 0% similar despite different names*

```diff
@@ -707,15 +707,15 @@
                 vana.logging.warning(
                     f"{coldkey_path} does not exist. Excluding..."
                 )
         return coldkey_files, wallet_names
 
     coldkey_files, wallet_names = list_coldkeypub_files(path)
     addresses = [
-        vana.keyfile(coldkey_path).keypair.address
+        vana.keyfile(coldkey_path).keypair.to_checksum_address()
         for coldkey_path in coldkey_files
     ]
     return addresses, wallet_names
 
 
 class WalletBalanceCommand:
     """
```

### Comparing `vana-0.1.1/vana/config.py` & `vana-0.1.2/vana/config.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/errors.py` & `vana-0.1.2/vana/errors.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/keyfile.py` & `vana-0.1.2/vana/keyfile.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/logging/__init__.py` & `vana-0.1.2/vana/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/logging/defines.py` & `vana-0.1.2/vana/logging/defines.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/logging/format.py` & `vana-0.1.2/vana/logging/format.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/logging/helpers.py` & `vana-0.1.2/vana/logging/helpers.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/logging/loggingmachine.py` & `vana-0.1.2/vana/logging/loggingmachine.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/message.py` & `vana-0.1.2/vana/message.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/mock/keyfile_mock.py` & `vana-0.1.2/vana/mock/keyfile_mock.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/mock/wallet_mock.py` & `vana-0.1.2/vana/mock/wallet_mock.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/node_client.py` & `vana-0.1.2/vana/node_client.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/node_server.py` & `vana-0.1.2/vana/node_server.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/state.py` & `vana-0.1.2/vana/state.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/threadpool.py` & `vana-0.1.2/vana/threadpool.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/utils/__init__.py` & `vana-0.1.2/vana/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/utils/fast_api_threaded_server.py` & `vana-0.1.2/vana/utils/fast_api_threaded_server.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/utils/misc.py` & `vana-0.1.2/vana/utils/misc.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/utils/networking.py` & `vana-0.1.2/vana/utils/networking.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/utils/wallet_utils.py` & `vana-0.1.2/vana/utils/wallet_utils.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/vana/wallet.py` & `vana-0.1.2/vana/wallet.py`

 * *Files identical despite different names*

### Comparing `vana-0.1.1/PKG-INFO` & `vana-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vana
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Home-page: https://github.com/vana-com/vana-framework
 Author: Tim Nunamaker
 Author-email: tim@vana.com
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
@@ -14,14 +14,15 @@
 Requires-Dist: ansible-vault (>=2.1.0,<3.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: fastapi (>=0.111.0,<0.112.0)
 Requires-Dist: munch (>=4.0.0,<5.0.0)
 Requires-Dist: netaddr (>=1.2.1,<2.0.0)
 Requires-Dist: password-strength (>=0.0.3.post2,<0.0.4)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
+Requires-Dist: pynacl (>=1.5.0,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: python-statemachine (>=2.2.0,<3.0.0)
 Requires-Dist: redis (>=5.0.4,<6.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: shtab (>=1.7.1,<2.0.0)
```

