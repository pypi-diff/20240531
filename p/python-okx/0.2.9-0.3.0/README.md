# Comparing `tmp/python-okx-0.2.9.tar.gz` & `tmp/python-okx-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-okx-0.2.9.tar", last modified: Thu May  9 08:24:47 2024, max compression
+gzip compressed data, was "python-okx-0.3.0.tar", last modified: Thu May 30 06:34:44 2024, max compression
```

## Comparing `python-okx-0.2.9.tar` & `python-okx-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-05-09 08:24:47.660338 python-okx-0.2.9/
--rw-r--r--   0 oker       (501) staff       (20)     3123 2024-05-09 08:24:47.647648 python-okx-0.2.9/PKG-INFO
--rw-r--r--   0 oker       (501) staff       (20)     2618 2023-12-07 06:04:16.000000 python-okx-0.2.9/README.md
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-05-09 08:24:47.639303 python-okx-0.2.9/okx/
--rw-r--r--   0 oker       (501) staff       (20)     9684 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/Account.py
--rw-r--r--   0 oker       (501) staff       (20)     4127 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/BlockTrading.py
--rw-r--r--   0 oker       (501) staff       (20)     1574 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/Convert.py
--rw-r--r--   0 oker       (501) staff       (20)     2750 2024-02-02 06:46:15.000000 python-okx-0.2.9/okx/CopyTrading.py
--rw-r--r--   0 oker       (501) staff       (20)     3852 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/Earning.py
--rw-r--r--   0 oker       (501) staff       (20)      787 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/FDBroker.py
--rw-r--r--   0 oker       (501) staff       (20)     6277 2024-05-09 08:21:39.000000 python-okx-0.2.9/okx/Funding.py
--rw-r--r--   0 oker       (501) staff       (20)     6690 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/Grid.py
--rw-r--r--   0 oker       (501) staff       (20)     4927 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/MarketData.py
--rw-r--r--   0 oker       (501) staff       (20)     5062 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/NDBroker.py
--rw-r--r--   0 oker       (501) staff       (20)     5135 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/PublicData.py
--rw-r--r--   0 oker       (501) staff       (20)     3226 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/SpreadTrading.py
--rw-r--r--   0 oker       (501) staff       (20)      494 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/Status.py
--rw-r--r--   0 oker       (501) staff       (20)     3527 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/SubAccount.py
--rw-r--r--   0 oker       (501) staff       (20)    10795 2024-05-09 08:21:39.000000 python-okx-0.2.9/okx/Trade.py
--rw-r--r--   0 oker       (501) staff       (20)     2330 2024-05-07 07:08:18.000000 python-okx-0.2.9/okx/TradingData.py
--rw-r--r--   0 oker       (501) staff       (20)       58 2024-05-07 07:09:18.000000 python-okx-0.2.9/okx/__init__.py
--rw-r--r--   0 oker       (501) staff       (20)    14387 2024-05-09 08:21:39.000000 python-okx-0.2.9/okx/consts.py
--rw-r--r--   0 oker       (501) staff       (20)     1182 2023-12-07 06:04:16.000000 python-okx-0.2.9/okx/exceptions.py
--rw-r--r--   0 oker       (501) staff       (20)     2510 2024-05-09 08:22:18.000000 python-okx-0.2.9/okx/okxclient.py
--rw-r--r--   0 oker       (501) staff       (20)     1826 2024-01-24 06:58:57.000000 python-okx-0.2.9/okx/utils.py
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-05-09 08:24:47.642860 python-okx-0.2.9/okx/websocket/
--rw-r--r--   0 oker       (501) staff       (20)      895 2023-12-26 08:54:41.000000 python-okx-0.2.9/okx/websocket/WebSocketFactory.py
--rw-r--r--   0 oker       (501) staff       (20)     2282 2024-01-24 08:39:57.000000 python-okx-0.2.9/okx/websocket/WsPrivateAsync.py
--rw-r--r--   0 oker       (501) staff       (20)     1561 2024-01-24 08:39:57.000000 python-okx-0.2.9/okx/websocket/WsPublicAsync.py
--rw-r--r--   0 oker       (501) staff       (20)     2199 2023-12-26 08:54:41.000000 python-okx-0.2.9/okx/websocket/WsUtils.py
--rw-r--r--   0 oker       (501) staff       (20)        0 2023-12-27 10:30:41.000000 python-okx-0.2.9/okx/websocket/__init__.py
-drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-05-09 08:24:47.646967 python-okx-0.2.9/python_okx.egg-info/
--rw-r--r--   0 oker       (501) staff       (20)     3123 2024-05-09 08:24:47.000000 python-okx-0.2.9/python_okx.egg-info/PKG-INFO
--rw-r--r--   0 oker       (501) staff       (20)      677 2024-05-09 08:24:47.000000 python-okx-0.2.9/python_okx.egg-info/SOURCES.txt
--rw-r--r--   0 oker       (501) staff       (20)        1 2024-05-09 08:24:47.000000 python-okx-0.2.9/python_okx.egg-info/dependency_links.txt
--rw-r--r--   0 oker       (501) staff       (20)       67 2024-05-09 08:24:47.000000 python-okx-0.2.9/python_okx.egg-info/requires.txt
--rw-r--r--   0 oker       (501) staff       (20)        4 2024-05-09 08:24:47.000000 python-okx-0.2.9/python_okx.egg-info/top_level.txt
--rw-r--r--   0 oker       (501) staff       (20)       38 2024-05-09 08:24:47.660500 python-okx-0.2.9/setup.cfg
--rw-r--r--   0 oker       (501) staff       (20)      775 2024-02-02 06:45:26.000000 python-okx-0.2.9/setup.py
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-05-30 06:34:44.794622 python-okx-0.3.0/
+-rw-r--r--   0 oker       (501) staff       (20)     3123 2024-05-30 06:34:44.794251 python-okx-0.3.0/PKG-INFO
+-rw-r--r--   0 oker       (501) staff       (20)     2618 2023-12-07 06:04:16.000000 python-okx-0.3.0/README.md
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-05-30 06:34:44.788894 python-okx-0.3.0/okx/
+-rw-r--r--   0 oker       (501) staff       (20)     9992 2024-05-30 06:30:57.000000 python-okx-0.3.0/okx/Account.py
+-rw-r--r--   0 oker       (501) staff       (20)     4127 2024-05-07 07:08:18.000000 python-okx-0.3.0/okx/BlockTrading.py
+-rw-r--r--   0 oker       (501) staff       (20)     1574 2024-05-07 07:08:18.000000 python-okx-0.3.0/okx/Convert.py
+-rw-r--r--   0 oker       (501) staff       (20)     2750 2024-02-02 06:46:15.000000 python-okx-0.3.0/okx/CopyTrading.py
+-rw-r--r--   0 oker       (501) staff       (20)     3852 2024-05-07 07:08:18.000000 python-okx-0.3.0/okx/Earning.py
+-rw-r--r--   0 oker       (501) staff       (20)      787 2024-05-07 07:08:18.000000 python-okx-0.3.0/okx/FDBroker.py
+-rw-r--r--   0 oker       (501) staff       (20)     6277 2024-05-09 08:21:39.000000 python-okx-0.3.0/okx/Funding.py
+-rw-r--r--   0 oker       (501) staff       (20)     6690 2024-05-07 07:08:18.000000 python-okx-0.3.0/okx/Grid.py
+-rw-r--r--   0 oker       (501) staff       (20)     4927 2024-05-07 07:08:18.000000 python-okx-0.3.0/okx/MarketData.py
+-rw-r--r--   0 oker       (501) staff       (20)     5062 2024-05-07 07:08:18.000000 python-okx-0.3.0/okx/NDBroker.py
+-rw-r--r--   0 oker       (501) staff       (20)     5135 2024-05-07 07:08:18.000000 python-okx-0.3.0/okx/PublicData.py
+-rw-r--r--   0 oker       (501) staff       (20)     3226 2024-05-07 07:08:18.000000 python-okx-0.3.0/okx/SpreadTrading.py
+-rw-r--r--   0 oker       (501) staff       (20)      494 2024-05-07 07:08:18.000000 python-okx-0.3.0/okx/Status.py
+-rw-r--r--   0 oker       (501) staff       (20)     3527 2024-05-07 07:08:18.000000 python-okx-0.3.0/okx/SubAccount.py
+-rw-r--r--   0 oker       (501) staff       (20)    10838 2024-05-30 06:24:32.000000 python-okx-0.3.0/okx/Trade.py
+-rw-r--r--   0 oker       (501) staff       (20)     2330 2024-05-07 07:08:18.000000 python-okx-0.3.0/okx/TradingData.py
+-rw-r--r--   0 oker       (501) staff       (20)       58 2024-05-30 06:34:13.000000 python-okx-0.3.0/okx/__init__.py
+-rw-r--r--   0 oker       (501) staff       (20)    14435 2024-05-29 12:34:17.000000 python-okx-0.3.0/okx/consts.py
+-rw-r--r--   0 oker       (501) staff       (20)     1182 2023-12-07 06:04:16.000000 python-okx-0.3.0/okx/exceptions.py
+-rw-r--r--   0 oker       (501) staff       (20)     2510 2024-05-09 08:22:18.000000 python-okx-0.3.0/okx/okxclient.py
+-rw-r--r--   0 oker       (501) staff       (20)     1826 2024-01-24 06:58:57.000000 python-okx-0.3.0/okx/utils.py
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-05-30 06:34:44.791638 python-okx-0.3.0/okx/websocket/
+-rw-r--r--   0 oker       (501) staff       (20)      895 2023-12-26 08:54:41.000000 python-okx-0.3.0/okx/websocket/WebSocketFactory.py
+-rw-r--r--   0 oker       (501) staff       (20)     2282 2024-01-24 08:39:57.000000 python-okx-0.3.0/okx/websocket/WsPrivateAsync.py
+-rw-r--r--   0 oker       (501) staff       (20)     1561 2024-01-24 08:39:57.000000 python-okx-0.3.0/okx/websocket/WsPublicAsync.py
+-rw-r--r--   0 oker       (501) staff       (20)     2199 2023-12-26 08:54:41.000000 python-okx-0.3.0/okx/websocket/WsUtils.py
+-rw-r--r--   0 oker       (501) staff       (20)        0 2023-12-27 10:30:41.000000 python-okx-0.3.0/okx/websocket/__init__.py
+drwxr-xr-x   0 oker       (501) staff       (20)        0 2024-05-30 06:34:44.793811 python-okx-0.3.0/python_okx.egg-info/
+-rw-r--r--   0 oker       (501) staff       (20)     3123 2024-05-30 06:34:44.000000 python-okx-0.3.0/python_okx.egg-info/PKG-INFO
+-rw-r--r--   0 oker       (501) staff       (20)      677 2024-05-30 06:34:44.000000 python-okx-0.3.0/python_okx.egg-info/SOURCES.txt
+-rw-r--r--   0 oker       (501) staff       (20)        1 2024-05-30 06:34:44.000000 python-okx-0.3.0/python_okx.egg-info/dependency_links.txt
+-rw-r--r--   0 oker       (501) staff       (20)       67 2024-05-30 06:34:44.000000 python-okx-0.3.0/python_okx.egg-info/requires.txt
+-rw-r--r--   0 oker       (501) staff       (20)        4 2024-05-30 06:34:44.000000 python-okx-0.3.0/python_okx.egg-info/top_level.txt
+-rw-r--r--   0 oker       (501) staff       (20)       38 2024-05-30 06:34:44.794677 python-okx-0.3.0/setup.cfg
+-rw-r--r--   0 oker       (501) staff       (20)      775 2024-02-02 06:45:26.000000 python-okx-0.3.0/setup.py
```

### Comparing `python-okx-0.2.9/PKG-INFO` & `python-okx-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-okx
-Version: 0.2.9
+Version: 0.3.0
 Summary: Python SDK for OKX
 Home-page: https://okx.com/docs-v5/
 Author: okxv5api
 Author-email: api@okg.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-okx-0.2.9/README.md` & `python-okx-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/Account.py` & `python-okx-0.3.0/okx/Account.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
                          limit=''):
         params = {'instType': instType, 'ccy': ccy, 'mgnMode': mgnMode, 'ctType': ctType, 'type': type,
                   'subType': subType, 'after': after, 'before': before, 'limit': limit}
         return self._request_with_params(GET, BILLS_DETAIL, params)
 
     # Get Bills Details (recent 3 months)
     def get_account_bills_archive(self, instType='', ccy='', mgnMode='', ctType='', type='', subType='', after='', before='',
-                          limit=''):
+                          limit='',begin='',end=''):
         params = {'instType': instType, 'ccy': ccy, 'mgnMode': mgnMode, 'ctType': ctType, 'type': type,
-                  'subType': subType, 'after': after, 'before': before, 'limit': limit}
+                  'subType': subType, 'after': after, 'before': before, 'limit': limit,'begin':begin,'end':end}
         return self._request_with_params(GET, BILLS_ARCHIVE, params)
 
     # Get Account Configuration
     def get_account_config(self):
         return self._request_without_params(GET, ACCOUNT_CONFIG)
 
     # Get Account Configuration
@@ -84,14 +84,18 @@
         params = {'instId': instId, 'posSide': posSide, 'type': type, 'amt': amt,'loanTrans':loanTrans}
         return self._request_with_params(POST, ADJUSTMENT_MARGIN, params)
 
     # Get Leverage
     def get_leverage(self, instId, mgnMode):
         params = {'instId': instId, 'mgnMode': mgnMode}
         return self._request_with_params(GET, GET_LEVERAGE, params)
+    # Get instruments
+    def get_instruments(self, instType='', ugly = '',instFamily='',instId=''):
+        params = {'instType': instType, 'ugly': ugly, 'instFamily': instFamily, 'instId': instId}
+        return self._request_with_params(GET,GET_INSTRUMENTS,params)
 
     # Get the maximum loan of isolated MARGIN
     def get_max_loan(self, instId, mgnMode, mgnCcy):
         params = {'instId': instId, 'mgnMode': mgnMode, 'mgnCcy': mgnCcy}
         return self._request_with_params(GET, MAX_LOAN, params)
 
     # Get Fee Rates
```

### Comparing `python-okx-0.2.9/okx/BlockTrading.py` & `python-okx-0.3.0/okx/BlockTrading.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/Convert.py` & `python-okx-0.3.0/okx/Convert.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/CopyTrading.py` & `python-okx-0.3.0/okx/CopyTrading.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/Earning.py` & `python-okx-0.3.0/okx/Earning.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/FDBroker.py` & `python-okx-0.3.0/okx/FDBroker.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/Funding.py` & `python-okx-0.3.0/okx/Funding.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/Grid.py` & `python-okx-0.3.0/okx/Grid.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/MarketData.py` & `python-okx-0.3.0/okx/MarketData.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/NDBroker.py` & `python-okx-0.3.0/okx/NDBroker.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/PublicData.py` & `python-okx-0.3.0/okx/PublicData.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/SpreadTrading.py` & `python-okx-0.3.0/okx/SpreadTrading.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/SubAccount.py` & `python-okx-0.3.0/okx/SubAccount.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/Trade.py` & `python-okx-0.3.0/okx/Trade.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,17 +82,17 @@
                                    begin='', end='', limit='', instFamily=''):
         params = {'instType': instType, 'uly': uly, 'instId': instId, 'ordType': ordType, 'state': state,
                   'after': after, 'before': before, 'begin': begin, 'end': end, 'limit': limit,
                   'instFamily': instFamily}
         return self._request_with_params(GET, ORDERS_HISTORY_ARCHIVE, params)
 
     # Get Transaction Details
-    def get_fills(self, instType='', uly='', instId='', ordId='', after='', before='', limit='', instFamily=''):
+    def get_fills(self, instType='', uly='', instId='', ordId='', after='', before='', limit='', instFamily='',begin='',end=''):
         params = {'instType': instType, 'uly': uly, 'instId': instId, 'ordId': ordId, 'after': after, 'before': before,
-                  'limit': limit, 'instFamily': instFamily}
+                  'limit': limit, 'instFamily': instFamily,'begin': begin, 'end' :end}
         return self._request_with_params(GET, ORDER_FILLS, params)
 
     # Place Algo Order
     def place_algo_order(self, instId='', tdMode='', side='', ordType='', sz='', ccy='',
                          posSide='', reduceOnly='', tpTriggerPx='',
                          tpOrdPx='', slTriggerPx='', slOrdPx='',
                          triggerPx='', orderPx='', tgtCcy='', pxVar='',
```

### Comparing `python-okx-0.2.9/okx/TradingData.py` & `python-okx-0.3.0/okx/TradingData.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/consts.py` & `python-okx-0.3.0/okx/consts.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 GET_VIP_INTEREST_DEDUCTED_DATA = '/api/v5/account/vip-interest-deducted'
 GET_VIP_LOAN_ORDER_LIST= '/api/v5/account/vip-loan-order-list'
 GET_VIP_LOAN_ORDER_DETAIL= '/api/v5/account/vip-loan-order-detail'
 SET_RISK_OFFSET_TYPE = '/api/v5/account/set-riskOffset-type'
 SET_AUTO_LOAN = '/api/v5/account/set-auto-loan'
 ACTIVSTE_OPTION = '/api/v5/account/activate-option'
 POSITION_BUILDER = '/api/v5/account/position-builder'
+GET_INSTRUMENTS = '/api/v5/account/instruments'
 
 # funding-complete-testcomplete
 NON_TRADABLE_ASSETS = '/api/v5/asset/non-tradable-assets'
 DEPOSIT_ADDRESS = '/api/v5/asset/deposit-address'
 GET_BALANCES = '/api/v5/asset/balances'
 FUNDS_TRANSFER = '/api/v5/asset/transfer'
 TRANSFER_STATE = '/api/v5/asset/transfer-state'
```

### Comparing `python-okx-0.2.9/okx/exceptions.py` & `python-okx-0.3.0/okx/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/okxclient.py` & `python-okx-0.3.0/okx/okxclient.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/utils.py` & `python-okx-0.3.0/okx/utils.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/websocket/WebSocketFactory.py` & `python-okx-0.3.0/okx/websocket/WebSocketFactory.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/websocket/WsPrivateAsync.py` & `python-okx-0.3.0/okx/websocket/WsPrivateAsync.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/websocket/WsPublicAsync.py` & `python-okx-0.3.0/okx/websocket/WsPublicAsync.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/okx/websocket/WsUtils.py` & `python-okx-0.3.0/okx/websocket/WsUtils.py`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/python_okx.egg-info/PKG-INFO` & `python-okx-0.3.0/python_okx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-okx
-Version: 0.2.9
+Version: 0.3.0
 Summary: Python SDK for OKX
 Home-page: https://okx.com/docs-v5/
 Author: okxv5api
 Author-email: api@okg.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `python-okx-0.2.9/python_okx.egg-info/SOURCES.txt` & `python-okx-0.3.0/python_okx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-okx-0.2.9/setup.py` & `python-okx-0.3.0/setup.py`

 * *Files identical despite different names*

