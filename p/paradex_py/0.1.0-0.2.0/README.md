# Comparing `tmp/paradex_py-0.1.0.tar.gz` & `tmp/paradex_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paradex_py-0.1.0.tar", max compression
+gzip compressed data, was "paradex_py-0.2.0.tar", max compression
```

## Comparing `paradex_py-0.1.0.tar` & `paradex_py-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1065 2024-03-04 21:41:21.516328 paradex_py-0.1.0/LICENSE
--rw-r--r--   0        0        0     1277 2024-03-04 21:41:21.516328 paradex_py-0.1.0/README.md
--rw-r--r--   0        0        0       37 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/account/__init__.py
--rw-r--r--   0        0        0     5218 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/account/account.py
--rw-r--r--   0        0        0     1186 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/account/starknet.py
--rw-r--r--   0        0        0     1989 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/account/typed_data.py
--rw-r--r--   0        0        0     3656 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/account/utils.py
--rw-r--r--   0        0        0        0 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/api/__init__.py
--rw-r--r--   0        0        0    12774 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/api/api_client.py
--rw-r--r--   0        0        0     2213 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/api/http_client.py
--rw-r--r--   0        0        0     1425 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/api/models.py
--rw-r--r--   0        0        0     6698 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/api/ws_client.py
--rw-r--r--   0        0        0     3638 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/common/order.py
--rw-r--r--   0        0        0      210 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/constants.py
--rw-r--r--   0        0        0      104 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/environment.py
--rw-r--r--   0        0        0        0 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/message/__init__.py
--rw-r--r--   0        0        0     1019 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/message/auth.py
--rw-r--r--   0        0        0      667 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/message/onboarding.py
--rw-r--r--   0        0        0     1611 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/message/order.py
--rw-r--r--   0        0        0      667 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/message/stark_key.py
--rw-r--r--   0        0        0     2871 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/paradex.py
--rw-r--r--   0        0        0      281 2024-03-04 21:41:21.516328 paradex_py-0.1.0/paradex_py/utils.py
--rw-r--r--   0        0        0     2091 2024-03-04 21:41:41.404554 paradex_py-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 paradex_py-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-03-20 20:56:50.439262 paradex_py-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1277 2024-03-20 20:56:50.439262 paradex_py-0.2.0/README.md
+-rw-r--r--   0        0        0       37 2024-03-20 20:56:50.439262 paradex_py-0.2.0/paradex_py/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 20:56:50.439262 paradex_py-0.2.0/paradex_py/account/__init__.py
+-rw-r--r--   0        0        0     5209 2024-03-20 20:56:50.439262 paradex_py-0.2.0/paradex_py/account/account.py
+-rw-r--r--   0        0        0     1186 2024-03-20 20:56:50.439262 paradex_py-0.2.0/paradex_py/account/starknet.py
+-rw-r--r--   0        0        0     1989 2024-03-20 20:56:50.439262 paradex_py-0.2.0/paradex_py/account/typed_data.py
+-rw-r--r--   0        0        0     3656 2024-03-20 20:56:50.439262 paradex_py-0.2.0/paradex_py/account/utils.py
+-rw-r--r--   0        0        0        0 2024-03-20 20:56:50.439262 paradex_py-0.2.0/paradex_py/api/__init__.py
+-rw-r--r--   0        0        0    16474 2024-03-20 20:56:50.439262 paradex_py-0.2.0/paradex_py/api/api_client.py
+-rw-r--r--   0        0        0     2279 2024-03-20 20:56:50.443261 paradex_py-0.2.0/paradex_py/api/http_client.py
+-rw-r--r--   0        0        0     1425 2024-03-20 20:56:50.443261 paradex_py-0.2.0/paradex_py/api/models.py
+-rw-r--r--   0        0        0    11436 2024-03-20 20:56:50.443261 paradex_py-0.2.0/paradex_py/api/ws_client.py
+-rw-r--r--   0        0        0      242 2024-03-20 20:56:50.443261 paradex_py-0.2.0/paradex_py/common/console_logging.py
+-rw-r--r--   0        0        0      452 2024-03-20 20:56:50.443261 paradex_py-0.2.0/paradex_py/common/file_logging.py
+-rw-r--r--   0        0        0     3638 2024-03-20 20:56:50.443261 paradex_py-0.2.0/paradex_py/common/order.py
+-rw-r--r--   0        0        0      231 2024-03-20 20:56:50.443261 paradex_py-0.2.0/paradex_py/constants.py
+-rw-r--r--   0        0        0      104 2024-03-20 20:56:50.443261 paradex_py-0.2.0/paradex_py/environment.py
+-rw-r--r--   0        0        0        0 2024-03-20 20:56:50.443261 paradex_py-0.2.0/paradex_py/message/__init__.py
+-rw-r--r--   0        0        0     1019 2024-03-20 20:56:50.443261 paradex_py-0.2.0/paradex_py/message/auth.py
+-rw-r--r--   0        0        0      667 2024-03-20 20:56:50.443261 paradex_py-0.2.0/paradex_py/message/onboarding.py
+-rw-r--r--   0        0        0     1611 2024-03-20 20:56:50.443261 paradex_py-0.2.0/paradex_py/message/order.py
+-rw-r--r--   0        0        0      667 2024-03-20 20:56:50.443261 paradex_py-0.2.0/paradex_py/message/stark_key.py
+-rw-r--r--   0        0        0     2759 2024-03-20 20:56:50.443261 paradex_py-0.2.0/paradex_py/paradex.py
+-rw-r--r--   0        0        0      281 2024-03-20 20:56:50.443261 paradex_py-0.2.0/paradex_py/utils.py
+-rw-r--r--   0        0        0     2091 2024-03-20 20:57:12.603180 paradex_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 paradex_py-0.2.0/PKG-INFO
```

### Comparing `paradex_py-0.1.0/LICENSE` & `paradex_py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `paradex_py-0.1.0/README.md` & `paradex_py-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `paradex_py-0.1.0/paradex_py/account/account.py` & `paradex_py-0.2.0/paradex_py/account/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 class CustomStarknetChainId(IntEnum):
     PRIVATE_SN_MAINNET = int_from_bytes(b"PRIVATE_SN_PARACLEAR_MAINNET")
     PRIVATE_SN_TESTNET_MOCK_SEPOLIA = int_from_bytes(b"PRIVATE_SN_POTC_MOCK_SEPOLIA")
     PRIVATE_SN_TESTNET_SEPOLIA = int_from_bytes(b"PRIVATE_SN_POTC_SEPOLIA")
 
 
 class ParadexAccount:
-    """ParadexAccount class to generate and manage Paradex account.
-    Initialized along with Paradex class.
+    """Class to generate and manage Paradex account.
+        Initialized along with `Paradex` class.
 
     Args:
         config (SystemConfig): SystemConfig
         l1_address (str): Ethereum address
         l1_private_key (Optional[str], optional): Ethereum private key. Defaults to None.
         l2_private_key (Optional[str], optional): Paradex private key. Defaults to None.
```

### Comparing `paradex_py-0.1.0/paradex_py/account/starknet.py` & `paradex_py-0.2.0/paradex_py/account/starknet.py`

 * *Files identical despite different names*

### Comparing `paradex_py-0.1.0/paradex_py/account/typed_data.py` & `paradex_py-0.2.0/paradex_py/account/typed_data.py`

 * *Files identical despite different names*

### Comparing `paradex_py-0.1.0/paradex_py/account/utils.py` & `paradex_py-0.2.0/paradex_py/account/utils.py`

 * *Files identical despite different names*

### Comparing `paradex_py-0.1.0/paradex_py/api/http_client.py` & `paradex_py-0.2.0/paradex_py/api/http_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,13 +67,15 @@
             headers=use_headers,
         )
 
     def delete(
         self,
         api_url: str,
         path: str,
+        params: Optional[dict] = None,
     ) -> dict:
         return self.request(
             url=f"{api_url}/{path}",
             http_method=HttpMethod.DELETE,
+            params=params,
             headers=self.client.headers,
         )
```

### Comparing `paradex_py-0.1.0/paradex_py/api/models.py` & `paradex_py-0.2.0/paradex_py/api/models.py`

 * *Files identical despite different names*

### Comparing `paradex_py-0.1.0/paradex_py/common/order.py` & `paradex_py-0.2.0/paradex_py/common/order.py`

 * *Files identical despite different names*

### Comparing `paradex_py-0.1.0/paradex_py/message/auth.py` & `paradex_py-0.2.0/paradex_py/message/auth.py`

 * *Files identical despite different names*

### Comparing `paradex_py-0.1.0/paradex_py/message/onboarding.py` & `paradex_py-0.2.0/paradex_py/message/onboarding.py`

 * *Files identical despite different names*

### Comparing `paradex_py-0.1.0/paradex_py/message/order.py` & `paradex_py-0.2.0/paradex_py/message/order.py`

 * *Files identical despite different names*

### Comparing `paradex_py-0.1.0/paradex_py/message/stark_key.py` & `paradex_py-0.2.0/paradex_py/message/stark_key.py`

 * *Files identical despite different names*

### Comparing `paradex_py-0.1.0/paradex_py/paradex.py` & `paradex_py-0.2.0/paradex_py/paradex.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,14 @@
 
     Examples:
         >>> from paradex_py import Paradex
         >>> from paradex_py.environment import Environment
         >>> paradex = Paradex(env=Environment.TESTNET)
     """
 
-    # Required for mypy to recognize the type of account
-    account: Optional[ParadexAccount] = None
-
     def __init__(
         self,
         env: Environment,
         l1_address: Optional[str] = None,
         l1_private_key: Optional[str] = None,
         l2_private_key: Optional[str] = None,
         logger: Optional[logging.Logger] = None,
@@ -37,16 +34,16 @@
         if env is None:
             raise ValueError("Paradex: Invalid environment")
         self.env = env
         self.logger: logging.Logger = logger or logging.getLogger(__name__)
         # Load api client and system config
         self.api_client = ParadexApiClient(env=env, logger=logger)
         self.ws_client = ParadexWebsocketClient(env=env, logger=logger)
-        self.config = self.api_client.load_system_config()
-        self.logger.info(f"Paradex: SystemConfig:{self.config}")
+        self.config = self.api_client.fetch_system_config()
+        self.account: Optional[ParadexAccount] = None
 
         # Initialize account if private key is provided
         if l1_address and (l2_private_key is not None or l1_private_key is not None):
             self.init_account(
                 l1_address=l1_address,
                 l1_private_key=l1_private_key,
                 l2_private_key=l2_private_key,
@@ -55,15 +52,15 @@
     def init_account(
         self,
         l1_address: str,
         l1_private_key: Optional[str] = None,
         l2_private_key: Optional[str] = None,
     ):
         """Initialize paradex account with l1 or l2 private keys.
-        Cannot be called if account is already initialized
+        Cannot be called if account is already initialized.
 
         Args:
             l1_address (str): L1 address
             l1_private_key (str): L1 private key
             l2_private_key (str): L2 private key
         """
         if self.account is not None:
```

### Comparing `paradex_py-0.1.0/pyproject.toml` & `paradex_py-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paradex_py"
-version = "v0.1.0"
+version = "v0.2.0"
 description = "Paradex Python SDK"
 authors = ["Paradex <finfo@paradex.trade>"]
 repository = "https://github.com/tradeparadex/paradex-py"
 documentation = "https://tradeparadex.github.io/paradex-py/"
 readme = "README.md"
 packages = [
   {include = "paradex_py"}
```

### Comparing `paradex_py-0.1.0/PKG-INFO` & `paradex_py-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paradex_py
-Version: 0.1.0
+Version: 0.2.0
 Summary: Paradex Python SDK
 Home-page: https://github.com/tradeparadex/paradex-py
 Author: Paradex
 Author-email: finfo@paradex.trade
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

