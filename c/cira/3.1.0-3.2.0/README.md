# Comparing `tmp/cira-3.1.0.tar.gz` & `tmp/cira-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cira-3.1.0.tar", last modified: Tue May  7 08:43:45 2024, max compression
+gzip compressed data, was "cira-3.2.0.tar", last modified: Fri May 31 09:26:53 2024, max compression
```

## Comparing `cira-3.1.0.tar` & `cira-3.2.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:43:45.469777 cira-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-07 08:43:27.000000 cira-3.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-07 08:43:27.000000 cira-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-05-07 08:43:45.469777 cira-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-07 08:43:27.000000 cira-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:43:45.465777 cira-3.1.0/cira/
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-07 08:43:27.000000 cira-3.1.0/cira/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-07 08:43:27.000000 cira-3.1.0/cira/alpaca_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10627 2024-05-07 08:43:27.000000 cira-3.1.0/cira/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-07 08:43:27.000000 cira-3.1.0/cira/asset_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-07 08:43:27.000000 cira-3.1.0/cira/asset_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-07 08:43:27.000000 cira-3.1.0/cira/assset_cryptocurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-07 08:43:27.000000 cira-3.1.0/cira/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-07 08:43:27.000000 cira-3.1.0/cira/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-07 08:43:27.000000 cira-3.1.0/cira/exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-07 08:43:27.000000 cira-3.1.0/cira/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-07 08:43:27.000000 cira-3.1.0/cira/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-07 08:43:27.000000 cira-3.1.0/cira/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-07 08:43:27.000000 cira-3.1.0/cira/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 08:43:45.469777 cira-3.1.0/cira.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-05-07 08:43:45.000000 cira-3.1.0/cira.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-07 08:43:45.000000 cira-3.1.0/cira.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 08:43:45.000000 cira-3.1.0/cira.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-07 08:43:45.000000 cira-3.1.0/cira.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-07 08:43:45.000000 cira-3.1.0/cira.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 08:43:45.469777 cira-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-07 08:43:27.000000 cira-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:26:53.858521 cira-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-31 09:26:36.000000 cira-3.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-31 09:26:36.000000 cira-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-05-31 09:26:53.858521 cira-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8426 2024-05-31 09:26:36.000000 cira-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:26:53.854521 cira-3.2.0/cira/
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-31 09:26:36.000000 cira-3.2.0/cira/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-31 09:26:36.000000 cira-3.2.0/cira/alpaca_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10873 2024-05-31 09:26:36.000000 cira-3.2.0/cira/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-31 09:26:36.000000 cira-3.2.0/cira/asset_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-31 09:26:36.000000 cira-3.2.0/cira/asset_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-05-31 09:26:36.000000 cira-3.2.0/cira/assset_cryptocurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-31 09:26:36.000000 cira-3.2.0/cira/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-31 09:26:36.000000 cira-3.2.0/cira/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-05-31 09:26:36.000000 cira-3.2.0/cira/exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-31 09:26:36.000000 cira-3.2.0/cira/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-31 09:26:36.000000 cira-3.2.0/cira/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-31 09:26:36.000000 cira-3.2.0/cira/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-31 09:26:36.000000 cira-3.2.0/cira/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:26:53.854521 cira-3.2.0/cira.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-05-31 09:26:53.000000 cira-3.2.0/cira.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-31 09:26:53.000000 cira-3.2.0/cira.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 09:26:53.000000 cira-3.2.0/cira.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-31 09:26:53.000000 cira-3.2.0/cira.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-31 09:26:53.000000 cira-3.2.0/cira.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 09:26:53.858521 cira-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-31 09:26:37.000000 cira-3.2.0/setup.py
```

### Comparing `cira-3.1.0/LICENSE.txt` & `cira-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cira-3.1.0/PKG-INFO` & `cira-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cira
-Version: 3.1.0
+Version: 3.2.0
 Summary: A simpler library for the alapaca trade api
 Home-page: https://github.com/AxelGard/cira
 Author: Axel Gard
 Author-email: axel.gard@tutanota.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Office/Business :: Financial
```

### Comparing `cira-3.1.0/README.md` & `cira-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cira-3.1.0/cira/__init__.py` & `cira-3.2.0/cira/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 from .asset_option import OptionContract
 
 from .portfolio import Portfolio, Position
 from .exchange import Exchange, DemoExchange
 
 import alpaca
 
-__version__ = "3.1.0"
+__version__ = "3.2.0"
 __author__ = "Axel Gard"
 __credits__ = "alpaca.markets"
```

### Comparing `cira-3.1.0/cira/asset.py` & `cira-3.2.0/cira/asset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import List
 from datetime import datetime
 import logging
 import warnings
 
 # Alpaca
 import alpaca
+import alpaca.trading
+import alpaca.trading.models
 from alpaca.trading.requests import GetAssetsRequest
 from alpaca.trading.enums import AssetClass, OrderType, AssetStatus
 from alpaca.data.models import Bar
 from alpaca.trading.enums import OrderSide, TimeInForce
 from alpaca.data.timeframe import TimeFrame
 from alpaca.trading.requests import LimitOrderRequest, StopLimitOrderRequest
 from alpaca.trading.client import TradingClient
@@ -170,60 +172,67 @@
         else:
             self._value = bars[0].c  # get stock at close
         return self._value
 
     def order(self, qty: int, beh: str) -> float:
         """submit order and is a template for order"""
 
-        warnings.warn(f"Warning: function is deprecated ({self.order})")
-
-        if not self.is_tradable():
-            raise Exception(
-                f"Sorry, {self.symbol} is currantly not tradable on https://alpaca.markets/"
-            )
-        order = auth.api().submit_order(
-            symbol=self.symbol, qty=qty, side=beh, type="market", time_in_force="gtc"
+        warnings.warn(
+            f"Warning: function is deprecated ({self.order}), will return {None}"
         )
-        return order
+
+        return None
 
     def is_sortable(self) -> bool:
         """checks if asset can be shorted"""
-        return bool(auth.api().get_asset(self.symbol).shortable)
+        return self.trade.get_asset(self.symbol).shortable
 
     def can_borrow(self) -> bool:
         """check whether the name is currently
         available to short at Alpaca"""
-        return auth.api().get_asset(self.symbol).easy_to_borrow
+        return self.trade.get_asset(self.symbol).easy_to_borrow
 
     def barset(self, limit: int):
         """returns barset for asset for time period lim"""
         return alpaca.api().get_bars(self.symbol, TimeFrame.Minute, limit=int(limit))
 
     def is_tradable(self) -> bool:
         """return if the asset can be traded"""
-        return bool(auth.api().get_asset(self.symbol).tradable)
+        return self.trade.get_asset(self.symbol).tradable
 
     def position(self):
-        """returns position of asset"""
-
-        warnings.warn(f"Warning: function is deprecated ({self.position})")
+        """returns position of asset,
+        if symbols is not in all your positions then it will return None"""
 
-        pos = auth.api().get_position(self.symbol)
-        self._position = util.reformat_position(pos)
-        return self._position
+        def reformat_position(position):
+            """reformat position to be float values"""
+            for key, value in position.items():
+                try:
+                    if isinstance(value, str):
+                        if "." in value:
+                            position[key] = float(value)
+                        else:
+                            position[key] = int(value)
+                except ValueError:
+                    continue
+            return position
+
+        all_pos = self.trade.get_all_positions()
+        for pos in all_pos:
+            if pos.symbol == self.symbol:
+                return reformat_position(dict(pos))
+        return None
 
     def today_plpc(self) -> float:
         """asset today's profit/loss percent"""
-        self._today_plpc = self.position()["unrealized_intraday_plpc"]
-        return self._today_plpc
+        return float(self.position().unrealized_intraday_plpc)
 
     def plpc(self) -> float:
         """asset sym (str) Unrealized profit/loss percentage"""
-        self._plpc = self.position()["unrealized_plpc"]
-        return self._plpc
+        return float(self.position().unrealized_plpc)
 
     # Operators
 
     def __eq__(self, other):
         if isinstance(other, (int, float)):
             return self.price() == other
         return self.price() == other.price()
```

### Comparing `cira-3.1.0/cira/asset_stock.py` & `cira-3.2.0/cira/asset_stock.py`

 * *Files identical despite different names*

### Comparing `cira-3.1.0/cira/assset_cryptocurrency.py` & `cira-3.2.0/cira/assset_cryptocurrency.py`

 * *Files identical despite different names*

### Comparing `cira-3.1.0/cira/auth.py` & `cira-3.2.0/cira/auth.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-import alpaca_trade_api as tradeapi
+import warnings
 import os
 
 from alpaca.data import StockHistoricalDataClient, StockLatestQuoteRequest
 
 from .portfolio import Portfolio
 
 
@@ -57,13 +57,9 @@
     with open(KEY_FILE, "r") as file:
         header = json.load(file)
     return header
 
 
 def api(version="v2"):
     """returns object for api"""
-    APCA_ID, APCA_KEY = get_api_keys()
-    # Open the API connection
-    api = tradeapi.REST(APCA_ID, APCA_KEY, "https://paper-api.alpaca.markets", version)
-    # Get account info
-    api.get_account()
-    return api
+    warnings.warn("This function has been deepracted by Alpaca Markets")
+    return None
```

### Comparing `cira-3.1.0/cira/portfolio.py` & `cira-3.2.0/cira/portfolio.py`

 * *Files identical despite different names*

### Comparing `cira-3.1.0/cira/strategy.py` & `cira-3.2.0/cira/strategy.py`

 * *Files identical despite different names*

### Comparing `cira-3.1.0/cira.egg-info/PKG-INFO` & `cira-3.2.0/cira.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cira
-Version: 3.1.0
+Version: 3.2.0
 Summary: A simpler library for the alapaca trade api
 Home-page: https://github.com/AxelGard/cira
 Author: Axel Gard
 Author-email: axel.gard@tutanota.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Office/Business :: Financial
```

### Comparing `cira-3.1.0/setup.py` & `cira-3.2.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="cira",
-    version="3.1.0",
+    version="3.2.0",
     description="A simpler library for the alapaca trade api",
     url="https://github.com/AxelGard/cira",
     author="Axel Gard",
     author_email="axel.gard@tutanota.com",
     license="MIT",
     packages=["cira"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "alpaca-py==0.21.0",
-        "alpaca-trade-api==2.3.0",
         "schedule==1.2.0",
     ],
     extras_requires={"dev": ["pytest"]},
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Topic :: Office/Business :: Financial",
         "Programming Language :: Python :: 3.8",
```

