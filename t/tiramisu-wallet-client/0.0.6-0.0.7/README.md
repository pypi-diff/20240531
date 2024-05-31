# Comparing `tmp/tiramisu_wallet_client-0.0.6.tar.gz` & `tmp/tiramisu_wallet_client-0.0.7.tar.gz`

## Comparing `tiramisu_wallet_client-0.0.6.tar` & `tiramisu_wallet_client-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.6/.flake8
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.6/requests.txt
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.6/test.py
--rw-r--r--   0        0        0   570108 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.6/test_image.jpg
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.6/src/tiramisu_wallet_client/__init__.py
--rw-r--r--   0        0        0    90051 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.6/src/tiramisu_wallet_client/temp.png
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.6/src/tiramisu_wallet_client/test.py
--rw-r--r--   0        0        0    15014 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.6/src/tiramisu_wallet_client/tiramisu_client.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.6/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.6/LICENSE
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.6/README.md
--rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.7/.flake8
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.7/requests.txt
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.7/test.py
+-rw-r--r--   0        0        0   570108 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.7/test_image.jpg
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.7/src/tiramisu_wallet_client/__init__.py
+-rw-r--r--   0        0        0    90051 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.7/src/tiramisu_wallet_client/temp.png
+-rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.7/src/tiramisu_wallet_client/test.py
+-rw-r--r--   0        0        0    16950 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.7/src/tiramisu_wallet_client/tiramisu_client.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.7/README.md
+-rw-r--r--   0        0        0      873 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 tiramisu_wallet_client-0.0.7/PKG-INFO
```

### Comparing `tiramisu_wallet_client-0.0.6/.pre-commit-config.yaml` & `tiramisu_wallet_client-0.0.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `tiramisu_wallet_client-0.0.6/test.py` & `tiramisu_wallet_client-0.0.7/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import random
 
 # Please go to https://testnet.tarowallet.net/walletapp/ 
 # and create an account then populate your credentials 
 USER_NAME="FILL_THIS_OUT"
 PASSWORD="FILL_THIS_OUT"
 
+TiramisuClient.google_login(None)
+
 print("Create client object")
 client = TiramisuClient(username=USER_NAME,password=PASSWORD)
 
 print("List all wallet balances")
 print( client.balances() )
 
 print("List all balances of NFTs in the wallet")
```

### Comparing `tiramisu_wallet_client-0.0.6/test_image.jpg` & `tiramisu_wallet_client-0.0.7/test_image.jpg`

 * *Files identical despite different names*

### Comparing `tiramisu_wallet_client-0.0.6/src/tiramisu_wallet_client/temp.png` & `tiramisu_wallet_client-0.0.7/src/tiramisu_wallet_client/temp.png`

 * *Files identical despite different names*

### Comparing `tiramisu_wallet_client-0.0.6/src/tiramisu_wallet_client/tiramisu_client.py` & `tiramisu_wallet_client-0.0.7/src/tiramisu_wallet_client/tiramisu_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 
 import requests
 import time 
+import socket
+import sys
+import urllib.parse
 
 class TiramisuClient():
     
     def __init__(self, username:str, password:str, network:str="testnet", server_url:str=None, register_new_user:bool=False) -> None:
         
         if server_url:
             self.base_url = server_url
@@ -22,19 +25,18 @@
         if register_new_user:
             self.register_user()
             
         self.auth_token = self.get_token()
         
         self.headers = {'Authorization':f'Token {self.auth_token}'}
     
-        assets = self.assets(limit=2000)
-
-        assets_dict = {curr["acronym"]:curr for curr in assets["results"]} 
-        self.btc_asset_id = assets_dict["SAT"]["id"]
-
+        assets = self.assets(limit=10,name="Bitcoin")
+        
+        self.btc_asset_id = assets["results"][0]["id"]
+        
     def register_user(self):
         """
         Register a new user
 
         Args:
         """
         
@@ -61,18 +63,20 @@
         
         self.raise_with_text(res)
         
         return res.json()["token"]
 
         
     def raise_with_text(self, res:dict):
-        
+        print(res.url)
         try: 
             res.raise_for_status()
         except Exception as e:
+            # with open("error.txt",'w') as f:
+            #     f.write(res.text)
             raise Exception(res.text) from e
     
     def balance_create(self, asset: str):
         """
         Create a new balance in the current user account
 
         Args:
@@ -89,15 +93,15 @@
     def get_btc_balance(self):
         """
         List all asset balances in the current user account
         """
         
         balances = self.balances()
         
-        balances_dict = {bal["currency"]: bal for bal in balances["results"]}
+        balances_dict = {bal["currency"]["id"]: bal for bal in balances["results"]}
         
         return balances_dict[self.btc_asset_id]
         
     def balances(self, offset=0, limit=100):
         """
         List all asset balances in the current user account
         """
@@ -194,27 +198,41 @@
     def assets_mint_nft_wait_finished(self, acronym:str, name:str, description:str, supply:int, file_path:str):
         
         minting_transaction = self.assets_mint_nft(acronym, name, description, supply, file_path)
         minting_transaction = self.transactions_wait_status(transaction_id=minting_transaction["id"], status_wait_for='minted')
         
         return minting_transaction
 
-    def assets(self, offset=0, limit=100):
+    def assets(self, offset=0, limit=100, name=None):
+        
         url = "api/currencies/"
-    
-        res = requests.get(self.base_url + url, headers=self.headers, params = {"limit":limit, "offset":offset})
+        params = {"limit":limit, "offset":offset}
+        
+        if name:
+            params["name"]=name
+            
+        res = requests.get(self.base_url + url, headers=self.headers, params = params)
         
         self.raise_with_text(res)
         
         return res.json()
 
-    def nfts(self, offset=0, limit=100):
+    def nfts(self, offset=0, limit=100, name=None, collection_name=None):
         url = "api/nfts/"
-    
-        res = requests.get(self.base_url + url, headers=self.headers, params = {"limit":limit, "offset":offset})
+        
+        params = {"limit":limit, "offset":offset}
+        
+        if collection_name:
+            params[f"collection__name"]=collection_name
+
+        if name:
+            params[f"name"]=name
+
+
+        res = requests.get(self.base_url + url, headers=self.headers, params = params)
         
         self.raise_with_text(res)
         
         return res.json()
 
     def asset(self, id):
         url = f"api/currencies/{id}"
@@ -222,23 +240,41 @@
         res = requests.get(self.base_url + url, headers=self.headers)
         
         self.raise_with_text(res)
         
         return res.json()
     
 
-    def collections(self):
+    def collections(self, offset=0, limit=100):
         url = f"api/collections/"
     
+        res = requests.get(self.base_url + url, headers=self.headers, params = {"limit":limit, "offset":offset})
+        
+        self.raise_with_text(res)
+        
+        return res.json()
+    
+    def collection(self, id):
+        url = f"api/collection/{id}"
+    
         res = requests.get(self.base_url + url, headers=self.headers)
         
         self.raise_with_text(res)
         
         return res.json()
     
+    def notifications(self, offset=0, limit=100):
+        url = f"api/notifications/"
+    
+        res = requests.get(self.base_url + url, headers=self.headers, params = {"limit":limit, "offset":offset})
+        
+        self.raise_with_text(res)
+        
+        return res.json()
+    
     def transactions_send_taproot_asset(self, invoice_outbound):
         url = "api/transactions/send_taro/"
 
         res = requests.post(self.base_url + url,data={"invoice_outbound":invoice_outbound}, headers=self.headers)
     
         self.raise_with_text(res)
         
@@ -250,15 +286,15 @@
         res = requests.post(self.base_url + url,data={"invoice_outbound":invoice_outbound, "amount":amount}, headers=self.headers)
         
         self.raise_with_text(res)
         
         return res.json()
 
     def transactions_send_btc_lnd(self, invoice_outbound:str):
-        url = "api/transactions/send_btc_lns/"
+        url = "api/transactions/send_btc_lnd/"
         
         res = requests.post(self.base_url + url,data={"invoice_outbound":invoice_outbound}, headers=self.headers)
         
         self.raise_with_text(res)
         
         return res.json()
 
@@ -340,18 +376,42 @@
     def transactions_receive_btc_get_invoice(self, amount:int, description: str):
         
         transaction_receive = self.transactions_receive_btc(amount, description)
         transaction_receive = self.transactions_wait_status(transaction_id=transaction_receive["id"], status_wait_for='inbound_invoice_generated')
         
         return (transaction_receive)
 
-    def transactions(self, offset=0, limit=100):
+    def transactions_receive_btc_lnd(self, amount:int, description: str):
+        url = "api/transactions/receive_btc_lnd/"
+        
+        res = requests.post(self.base_url + url,data={"amount":amount,"description":description}, headers=self.headers)
+
+        self.raise_with_text(res)
+        
+        return res.json()
+
+
+
+    def transactions(self, offset=0, limit=100, destination_username=None, description=None, currency_id=None):
         url = "api/transactions/"
         
-        res = requests.get(self.base_url + url, headers=self.headers, params = {"limit":limit, "offset":offset})
+        params = {"limit":limit, "offset":offset}
+        
+        search = []
+        
+        if destination_username:
+            params["destination_user__username"] = destination_username
+            
+        if description:
+            params["description"] = description
+        
+        if currency_id:
+            params["currency_id"] = currency_id
+            
+        res = requests.get(self.base_url + url, headers=self.headers, params = params)
         
         self.raise_with_text(res)
         
         return res.json()
         
     def transaction(self, id):
         url = f"api/transactions/{id}"
@@ -376,18 +436,18 @@
         
         res = requests.post(self.base_url + url, data={"currency":asset, "price_sat":price_sat}, headers=self.headers)
         
         self.raise_with_text(res)
         
         return res.json()
         
-    def listings_my(self):
+    def listings_my(self, offset=0, limit=100):
         url = "api/listings_my/"
         
-        res = requests.get(self.base_url + url, headers=self.headers)
+        res = requests.get(self.base_url + url, headers=self.headers, params = {"limit":limit, "offset":offset})
         
         self.raise_with_text(res)
         
         return res.json()
         
     def buy_taproot_asset_asset(self, asset:int, amount:int):
         url = "api/buy_taro_asset/"
@@ -409,29 +469,36 @@
     
         res = requests.post(self.base_url + url, data={"currency":asset}, headers=self.headers)
         
         self.raise_with_text(res)
         
         return res.json()
     
-    def buy_nft_asset_wait_finished(self, asset:int, amount:int):
+    def buy_nft_asset_wait_finished(self, asset:int):
         
-        transaction_receive = self.buy_nft_asset(asset, amount)
+        transaction_receive = self.buy_nft_asset(asset)
         transaction_receive = self.transactions_wait_status(transaction_id=transaction_receive["id"], status_wait_for='exchange_finished')
         return transaction_receive
     
     def sell_taproot_asset(self, asset:int, amount:int):
         url = "api/sell_taro_asset/"
 
         res = requests.post(self.base_url + url, data={"currency":asset, "amount":amount}, headers=self.headers)
         
         self.raise_with_text(res)
         
         return res.json()
 
     def sell_taproot_asset_wait_finished(self, asset:int):
         
-        transaction_receive = self.sell_taproot_asset_asset(asset)
+        transaction_receive = self.sell_taproot_asset(asset)
         transaction_receive = self.transactions_wait_status(transaction_id=transaction_receive["id"], status_wait_for='exchange_finished')
         return transaction_receive
 
-        "api/currencies/<int:pk>",
+    def get_info(self):
+        url = "api/get_info/"
+
+        res = requests.get(self.base_url + url, headers=self.headers)
+        
+        self.raise_with_text(res)
+        
+        return res.json()
```

### Comparing `tiramisu_wallet_client-0.0.6/LICENSE` & `tiramisu_wallet_client-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tiramisu_wallet_client-0.0.6/README.md` & `tiramisu_wallet_client-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tiramisu_wallet_client-0.0.6/pyproject.toml` & `tiramisu_wallet_client-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tiramisu-wallet-client"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Adam Ivansky", email="adam.ivansky@gmail.com" },
 ]
 description = """
 A client for Tiramisu wallet platform. This client allows you to programatically mint, transfer and trade Taproot Assets Protocol that represents altcoins and NTFs on Bitcoin blackchain. 
 """
 readme = "README.md"
```

### Comparing `tiramisu_wallet_client-0.0.6/PKG-INFO` & `tiramisu_wallet_client-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tiramisu-wallet-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: A client for Tiramisu wallet platform. This client allows you to programatically mint, transfer and trade Taproot Assets Protocol that represents altcoins and NTFs on Bitcoin blackchain. 
 Project-URL: Homepage, https://github.com/snow884/tiramisu_wallet_client
 Project-URL: Bug Tracker, https://github.com/snow884/tiramisu_wallet_client/issues
 Author-email: Adam Ivansky <adam.ivansky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

