# Comparing `tmp/xchainpy2_cosmos-0.0.5.tar.gz` & `tmp/xchainpy2_cosmos-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchainpy2_cosmos-0.0.5.tar", last modified: Wed Jan  3 16:33:56 2024, max compression
+gzip compressed data, was "xchainpy2_cosmos-0.0.6.tar", last modified: Fri May 31 14:25:06 2024, max compression
```

## Comparing `xchainpy2_cosmos-0.0.5.tar` & `xchainpy2_cosmos-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 16:33:56.575513 xchainpy2_cosmos-0.0.5/
--rw-r--r--   0 tirinox    (501) staff       (20)     1086 2023-04-22 16:09:04.000000 xchainpy2_cosmos-0.0.5/LICENSE
--rw-r--r--   0 tirinox    (501) staff       (20)     1218 2024-01-03 16:33:56.575264 xchainpy2_cosmos-0.0.5/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)       40 2023-10-11 12:18:22.000000 xchainpy2_cosmos-0.0.5/README.md
--rw-r--r--   0 tirinox    (501) staff       (20)     1362 2023-10-10 07:07:24.000000 xchainpy2_cosmos-0.0.5/pyproject.toml
--rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-01-03 16:33:56.575562 xchainpy2_cosmos-0.0.5/setup.cfg
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 16:33:56.572631 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/
--rw-r--r--   0 tirinox    (501) staff       (20)       85 2023-06-17 18:34:47.000000 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3441 2023-11-16 12:27:48.000000 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/const.py
--rw-r--r--   0 tirinox    (501) staff       (20)    21660 2023-12-08 20:12:43.000000 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/cosm_client.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3034 2023-11-16 12:27:48.000000 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/models.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 16:33:56.574271 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/tests/
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 16:33:56.574512 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/tests/samples/
--rw-r--r--   0 tirinox    (501) staff       (20)     9625 2023-07-10 15:57:37.000000 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/tests/samples/40BD2FCF41252AD7EAEE313989DC9CB10A120CD384804DD0E9D87F1B388243BB.json
--rw-r--r--   0 tirinox    (501) staff       (20)     2771 2023-12-07 17:12:43.000000 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/tests/test_cosm_client.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1385 2023-12-05 13:48:52.000000 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/tests/test_cosm_util.py
--rw-r--r--   0 tirinox    (501) staff       (20)      743 2023-11-25 10:54:33.000000 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/tests/test_models.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6646 2023-12-07 17:51:56.000000 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/utils.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-01-03 16:33:56.574809 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos.egg-info/
--rw-r--r--   0 tirinox    (501) staff       (20)     1218 2024-01-03 16:33:56.000000 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos.egg-info/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)      594 2024-01-03 16:33:56.000000 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos.egg-info/SOURCES.txt
--rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-01-03 16:33:56.000000 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos.egg-info/dependency_links.txt
--rw-r--r--   0 tirinox    (501) staff       (20)      135 2024-01-03 16:33:56.000000 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos.egg-info/requires.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       17 2024-01-03 16:33:56.000000 xchainpy2_cosmos-0.0.5/xchainpy2_cosmos.egg-info/top_level.txt
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:25:06.275281 xchainpy2_cosmos-0.0.6/
+-rw-r--r--   0 tirinox    (501) staff       (20)     1086 2024-03-07 10:37:31.000000 xchainpy2_cosmos-0.0.6/LICENSE
+-rw-r--r--   0 tirinox    (501) staff       (20)     1218 2024-05-31 14:25:06.275048 xchainpy2_cosmos-0.0.6/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)       40 2024-03-07 10:37:31.000000 xchainpy2_cosmos-0.0.6/README.md
+-rw-r--r--   0 tirinox    (501) staff       (20)     1362 2024-03-07 10:37:31.000000 xchainpy2_cosmos-0.0.6/pyproject.toml
+-rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-05-31 14:25:06.275313 xchainpy2_cosmos-0.0.6/setup.cfg
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:25:06.272685 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/
+-rw-r--r--   0 tirinox    (501) staff       (20)       85 2024-03-07 10:37:31.000000 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3512 2024-03-07 10:37:31.000000 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/const.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    21319 2024-03-07 10:37:31.000000 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/cosm_client.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3034 2024-03-07 10:37:31.000000 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/models.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:25:06.274109 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/tests/
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:25:06.274282 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/tests/samples/
+-rw-r--r--   0 tirinox    (501) staff       (20)     9625 2024-03-07 10:37:31.000000 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/tests/samples/40BD2FCF41252AD7EAEE313989DC9CB10A120CD384804DD0E9D87F1B388243BB.json
+-rw-r--r--   0 tirinox    (501) staff       (20)     2771 2024-03-07 10:37:31.000000 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/tests/test_cosm_client.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1385 2024-03-07 10:37:31.000000 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/tests/test_cosm_util.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      743 2024-03-07 10:37:31.000000 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/tests/test_models.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6647 2024-05-31 12:48:06.000000 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/utils.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-05-31 14:25:06.274651 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos.egg-info/
+-rw-r--r--   0 tirinox    (501) staff       (20)     1218 2024-05-31 14:25:06.000000 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos.egg-info/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)      594 2024-05-31 14:25:06.000000 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos.egg-info/SOURCES.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-05-31 14:25:06.000000 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos.egg-info/dependency_links.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)      135 2024-05-31 14:25:06.000000 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos.egg-info/requires.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       17 2024-05-31 14:25:06.000000 xchainpy2_cosmos-0.0.6/xchainpy2_cosmos.egg-info/top_level.txt
```

### Comparing `xchainpy2_cosmos-0.0.5/LICENSE` & `xchainpy2_cosmos-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xchainpy2_cosmos-0.0.5/PKG-INFO` & `xchainpy2_cosmos-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2_cosmos
-Version: 0.0.5
+Version: 0.0.6
 Summary: XChainPy2 Cosmos Client
 Author-email: Tirinox <developer@tirinox.ru>
 License: MIT
 Project-URL: source, https://github.com/tirinox/xchainpy
 Keywords: Crypto,THORChain,Blockchain,XChain,Cosmos
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `xchainpy2_cosmos-0.0.5/pyproject.toml` & `xchainpy2_cosmos-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xchainpy2_cosmos"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
     { name = "Tirinox", email = "developer@tirinox.ru" },
 ]
 description = "XChainPy2 Cosmos Client"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["Crypto", "THORChain", "Blockchain", "XChain", "Cosmos"]
```

### Comparing `xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/const.py` & `xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,21 @@
 from xchainpy2_client import Fees, FeeType, FeeOption, ExplorerProvider
 from xchainpy2_utils import Amount, NetworkType
 
 COSMOS_DECIMAL = 6
 
 # Default gas limit
 # As same as definition in Cosmosstation's web wallet
-DEFAULT_GAS_LIMIT = '200000'
+DEFAULT_GAS_LIMIT = 90_000
+
+FEE_MINIMUM_GAS_PRICE = 0.006
 
 # Default fee
 # As same as definition in Cosmosstation's web wallet
-DEFAULT_FEE = Amount.from_base(5000, COSMOS_DECIMAL)
+DEFAULT_FEE = Amount.from_base(int(DEFAULT_GAS_LIMIT * FEE_MINIMUM_GAS_PRICE), COSMOS_DECIMAL)
 
 # Chain identifier for Cosmos chain
 GAIA_CHAIN_KEY = 'GAIA'
 
 # Cosmos denomination
 COSMOS_DENOM = 'uatom'
```

### Comparing `xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/cosm_client.py` & `xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/cosm_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import asyncio
 import logging
 from datetime import datetime
+from math import ceil
 from operator import itemgetter
 from typing import Optional, List, Union
 from urllib.parse import urlencode
 
 from aiohttp import ClientSession
-from cosmpy.aerial.client import LedgerClient, Account, create_bank_send_msg, prepare_and_broadcast_basic_transaction
+from cosmpy.aerial.client import LedgerClient, Account, create_bank_send_msg, prepare_and_broadcast_basic_transaction, \
+    Coin
 from cosmpy.aerial.config import NetworkConfig
 from cosmpy.aerial.tx import Transaction
 from cosmpy.aerial.wallet import LocalWallet
 from cosmpy.crypto.address import Address
 from cosmpy.crypto.keypairs import PrivateKey, PublicKey
 from cosmpy.protos.cosmos.tx.v1beta1.service_pb2 import BroadcastTxRequest, BroadcastMode
-from math import ceil
 
 from xchainpy2_client import XChainClient, RootDerivationPaths, FeeBounds, XcTx, \
-    Fees, TxPage, AssetInfo, FeeType, FeeOption
+    Fees, TxPage, FeeType, FeeOption
 from xchainpy2_client.fees import single_fee
 from xchainpy2_crypto import derive_private_key, create_address
-from xchainpy2_utils import Chain, NetworkType, CryptoAmount, RUNE_DECIMAL, Asset, Amount, AssetATOM, \
+from xchainpy2_utils import Chain, NetworkType, CryptoAmount, Asset, Amount, AssetATOM, \
     unique_by_key, batched, NINE_REALMS_CLIENT_HEADER, XCHAINPY_IDENTIFIER, flatten
 from .const import DEFAULT_CLIENT_URLS, DEFAULT_EXPLORER_PROVIDER, COSMOS_ROOT_DERIVATION_PATHS, COSMOS_ADDR_PREFIX, \
     COSMOS_CHAIN_IDS, COSMOS_DECIMAL, TxFilterFunc, MAX_PAGES_PER_FUNCTION_CALL, MAX_TX_COUNT_PER_PAGE, \
-    MAX_TX_COUNT_PER_FUNCTION_CALL, COSMOS_DENOM, DEFAULT_FEE, DEFAULT_GAS_LIMIT, DEFAULT_REST_USER_AGENT
+    MAX_TX_COUNT_PER_FUNCTION_CALL, COSMOS_DENOM, DEFAULT_FEE, DEFAULT_GAS_LIMIT, DEFAULT_REST_USER_AGENT, \
+    FEE_MINIMUM_GAS_PRICE
 from .models import TxHistoryResponse, TxLoadException
 from .utils import parse_tx_response_json
 
 logger = logging.getLogger(__name__)
 
 
 class CosmosGaiaClient(XChainClient):
@@ -59,46 +61,56 @@
         super().__init__(Chain.Cosmos, network, phrase, private_key, fee_bound, root_derivation_paths, wallet_index)
 
         self.explorers = explorer_providers
 
         if isinstance(client_urls, str):
             client_urls = {NetworkType.MAINNET: client_urls}
 
-        self.client_urls = client_urls.copy() if client_urls else DEFAULT_CLIENT_URLS.copy()
+        self._client_urls = client_urls.copy() if client_urls else DEFAULT_CLIENT_URLS.copy()
         self.chain_ids = chain_ids.copy() if chain_ids else COSMOS_CHAIN_IDS.copy()
 
         self._gas_asset = AssetATOM
         self._prefix = COSMOS_ADDR_PREFIX
 
         self._denom = COSMOS_DENOM
         self._decimal = COSMOS_DECIMAL
         self._gas_limit = DEFAULT_GAS_LIMIT
 
+        self._fee_minimum_gas_price = FEE_MINIMUM_GAS_PRICE
+
         self._client: Optional[LedgerClient] = None
         self._recreate_client()
 
         self._wallet: Optional[LocalWallet] = None
         self._make_wallet()
 
         self.cache = None
         self.tx_responses = {}
 
+        self.standard_tx_fee = DEFAULT_FEE
+
+        self.cache_fee_period = 600  # sec = 10 min
+
+    @property
+    def get_client_urls(self):
+        return self._client_urls
+
     def get_client(self) -> LedgerClient:
         """
         Please use this getter to obtain LedgerClient for specific Cosmos calls like delegation, staking etc.
         Underlying library is cosmpy (https://github.com/fetchai/cosmpy)
         :return: LedgerClient
         """
         if not self._client:
             self._recreate_client()
         return self._client
 
     @property
     def server_url(self):
-        return self.client_urls[self.network]
+        return self._client_urls[self.network]
 
     @property
     def rpc_url(self):
         return self.server_url
 
     @property
     def rest_session(self) -> ClientSession:
@@ -117,15 +129,15 @@
 
         rest_url = f'rest+{self.server_url}'
         self._client = LedgerClient(NetworkConfig(
             chain_id=self.chain_ids[self.network],
             url=rest_url,
             fee_denomination=self._denom,
             staking_denomination=self._denom,
-            fee_minimum_gas_price=0,
+            fee_minimum_gas_price=self._fee_minimum_gas_price,
         ))
 
     def set_chain_id(self, chain_id: str):
         """
         Set/update the current chain id.
         :param chain_id:
         :return: None
@@ -224,24 +236,25 @@
 
         balances = await asyncio.get_event_loop().run_in_executor(
             None,
             self._client.query_bank_all_balances,
             address
         )
 
-        our_balances = [
-            CryptoAmount(
-                Amount.from_base(balance.amount, self._decimal),
-                self.parse_denom_to_asset(balance.denom)
-            )
-            for balance in balances
-        ]
+        our_balances = [self.convert_coin_to_amount(balance) for balance in balances]
 
         return our_balances
 
+    def convert_coin_to_amount(self, c: Coin):
+        asset = self.parse_denom_to_asset(c.denom)
+        return CryptoAmount(
+            Amount.from_base(c.amount, self._decimal),
+            asset
+        )
+
     def parse_denom_to_asset(self, denom: str) -> Asset:
         if denom == self._denom:
             return self._gas_asset
         else:
             return Asset(self.chain.value, denom.upper())
 
     async def get_account(self, address: str = None) -> Optional[Account]:
@@ -443,32 +456,16 @@
             j, tx_id, our_address, self._decimal, self._denom, self._gas_asset
         )
 
     async def get_transaction_data_raw(self, tx_id: str) -> dict:
         url = self.url_to_fetch_tx_data(tx_id)
         return await self._get_json(url)
 
-    async def get_fees(self, cache=None, tc_fee_rate=None) -> Fees:
-        """
-        Returns fees.
-        It tries to get chain fees from THORChain `inbound_addresses` first
-        :param cache: THORChainCache from the query module
-        :param tc_fee_rate: You can externally pass the fee rate having 8 decimals. (optional)
-        :return:
-        """
-        if tc_fee_rate is not None:
-            return single_fee(FeeType.FLAT_FEE, DEFAULT_FEE)
-
-        tc_fee_rate = await cache.get_fee_rates(self.chain)
-
-        # convert decimal: 1e8 (THORChain) to 1e6 (COSMOS)
-        # Similar to `fromCosmosToThorchain` in THORNode
-        decimal_diff = self._decimal - RUNE_DECIMAL
-        fee_rate = Amount.from_base(tc_fee_rate * 10 ** decimal_diff, self._decimal)
-        return single_fee(FeeType.FLAT_FEE, fee_rate)
+    async def get_fees(self) -> Fees:
+        return single_fee(FeeType.FLAT_FEE, self.standard_tx_fee)
 
     async def transfer(self, what: CryptoAmount,
                        recipient: str,
                        memo: Optional[str] = None,
                        fee_rate: Optional[int] = None,
                        check_balance: bool = True) -> str:
         """
@@ -490,15 +487,15 @@
         response = await asyncio.get_event_loop().run_in_executor(
             None,
             prepare_and_broadcast_basic_transaction,
             self._client,
             tx,
             self._wallet,
             None,  # account
-            int(self._gas_limit),
+            self._gas_limit,
             memo
         )
 
         self._save_last_response(response.tx_hash, response)
 
         return response.tx_hash
 
@@ -556,15 +553,15 @@
         return self._client
 
     @property
     def prefix(self) -> str:
         return self._prefix
 
     async def check_balance(self, address, amount: CryptoAmount):
-        fees = await self.get_fees(self.cache)
+        fees = await self.get_fees()
         fee = fees.fees[FeeOption.AVERAGE]
 
         balances = await self.get_balance(address)
 
         asset_balance = None
         native_balance = None
 
@@ -573,16 +570,17 @@
                 asset_balance = balance
             if balance.asset == self._gas_asset:
                 native_balance = balance
 
         is_native = amount.asset == self._gas_asset
         extra_fee = fee if is_native else Amount.from_base(0, self._decimal)
 
-        if asset_balance is None or asset_balance.amount.as_base < amount.amount.as_base + extra_fee.as_base:
-            raise ValueError(f"Insufficient funds: {amount.amount} {amount.asset}")
+        if (asset_balance is None
+                or asset_balance.amount.as_base < (required := amount.amount.as_base + extra_fee.as_base)):
+            raise ValueError(f"Insufficient funds: {required} is required. Balance is {asset_balance}")
 
         if native_balance is None or native_balance.amount < fee:
             raise ValueError(f"Insufficient funds to pay fee: {fee.amount} {self._gas_asset}")
 
     def _make_wallet(self) -> LocalWallet:
         if self.phrase or self._private_key:
             pk = PrivateKey(bytes.fromhex(self.get_private_key()))
```

### Comparing `xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/models.py` & `xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/models.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/tests/samples/40BD2FCF41252AD7EAEE313989DC9CB10A120CD384804DD0E9D87F1B388243BB.json` & `xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/tests/samples/40BD2FCF41252AD7EAEE313989DC9CB10A120CD384804DD0E9D87F1B388243BB.json`

 * *Files identical despite different names*

### Comparing `xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/tests/test_cosm_client.py` & `xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/tests/test_cosm_client.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/tests/test_cosm_util.py` & `xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/tests/test_cosm_util.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/tests/test_models.py` & `xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `xchainpy2_cosmos-0.0.5/xchainpy2_cosmos/utils.py` & `xchainpy2_cosmos-0.0.6/xchainpy2_cosmos/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Optional, List, Tuple
 
+
 from cosmpy.crypto.address import Address
 
 from xchainpy2_client import XcTx, TxType, TokenTransfer
 from xchainpy2_utils import Asset, AssetATOM, Chain, Amount, key_attr_getter, parse_iso_date
 from .const import COSMOS_DENOM
 from .models import TxLoadException, load_logs, TxLog
```

### Comparing `xchainpy2_cosmos-0.0.5/xchainpy2_cosmos.egg-info/PKG-INFO` & `xchainpy2_cosmos-0.0.6/xchainpy2_cosmos.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2_cosmos
-Version: 0.0.5
+Version: 0.0.6
 Summary: XChainPy2 Cosmos Client
 Author-email: Tirinox <developer@tirinox.ru>
 License: MIT
 Project-URL: source, https://github.com/tirinox/xchainpy
 Keywords: Crypto,THORChain,Blockchain,XChain,Cosmos
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `xchainpy2_cosmos-0.0.5/xchainpy2_cosmos.egg-info/SOURCES.txt` & `xchainpy2_cosmos-0.0.6/xchainpy2_cosmos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

