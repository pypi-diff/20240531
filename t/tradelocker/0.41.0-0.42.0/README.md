# Comparing `tmp/tradelocker-0.41.0.tar.gz` & `tmp/tradelocker-0.42.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradelocker-0.41.0.tar", max compression
+gzip compressed data, was "tradelocker-0.42.0.tar", max compression
```

## Comparing `tradelocker-0.41.0.tar` & `tradelocker-0.42.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1069 2024-04-28 19:44:48.930398 tradelocker-0.41.0/LICENSE.txt
--rw-r--r--   0        0        0     2829 2024-04-28 19:44:48.931056 tradelocker-0.41.0/README.md
--rw-r--r--   0        0        0     1476 2024-04-30 07:42:37.704738 tradelocker-0.41.0/pyproject.toml
--rw-r--r--   0        0        0       23 2024-04-28 19:44:48.950787 tradelocker-0.41.0/src/tradelocker/__about__.py
--rw-r--r--   0        0        0       85 2024-04-28 19:44:48.941751 tradelocker-0.41.0/src/tradelocker/__init__.py
--rw-r--r--   0        0        0        0 2024-04-28 19:44:48.950881 tradelocker-0.41.0/src/tradelocker/py.typed
--rw-r--r--   0        0        0    55793 2024-04-30 07:42:37.705156 tradelocker-0.41.0/src/tradelocker/tradelocker_api.py
--rw-r--r--   0        0        0     5350 2024-04-30 07:42:37.705578 tradelocker-0.41.0/src/tradelocker/types.py
--rw-r--r--   0        0        0     9168 2024-04-29 12:27:29.894587 tradelocker-0.41.0/src/tradelocker/utils.py
--rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 tradelocker-0.41.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-31 04:31:45.532192 tradelocker-0.42.0/LICENSE.txt
+-rw-r--r--   0        0        0     2829 2024-05-31 04:31:45.532863 tradelocker-0.42.0/README.md
+-rw-r--r--   0        0        0     1454 2024-05-31 05:53:22.315574 tradelocker-0.42.0/pyproject.toml
+-rw-r--r--   0        0        0       23 2024-05-31 04:31:45.565981 tradelocker-0.42.0/src/tradelocker/__about__.py
+-rw-r--r--   0        0        0       85 2024-05-31 05:09:13.572381 tradelocker-0.42.0/src/tradelocker/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 04:31:45.566082 tradelocker-0.42.0/src/tradelocker/py.typed
+-rw-r--r--   0        0        0    57744 2024-05-31 05:53:22.315946 tradelocker-0.42.0/src/tradelocker/tradelocker_api.py
+-rw-r--r--   0        0        0     5939 2024-05-31 05:53:22.316816 tradelocker-0.42.0/src/tradelocker/types.py
+-rw-r--r--   0        0        0     7885 2024-05-31 05:53:22.317098 tradelocker-0.42.0/src/tradelocker/utils.py
+-rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 tradelocker-0.42.0/PKG-INFO
```

### Comparing `tradelocker-0.41.0/LICENSE.txt` & `tradelocker-0.42.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tradelocker-0.41.0/README.md` & `tradelocker-0.42.0/README.md`

 * *Files identical despite different names*

### Comparing `tradelocker-0.41.0/pyproject.toml` & `tradelocker-0.42.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,43 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "tradelocker"
-version = "0.41.0"
-description = "TradeLocker Trading API support for Python"
+version = "0.42.0"
+description = "Python client for TradeLocker's Trading API"
 authors = ["TradeLocker <admin@tradelocker.com>"]
 license = "MIT"
 readme = "README.md"
-keywords=["tradelocker","api", "rest", "trading", "exchange", "algotrading", "algo", "bots", "strategies"]
+keywords=["tradelocker","api", "rest", "trading", "algotrading", "algo", "bots", "strategies"]
 urls.Source = "https://github.com/tradelocker/tradelocker-python/"
 urls.Issues = "https://github.com/tradelocker/tradelocker-python/issues"
 
 
 [tool.poetry.dependencies]
 python = ">=3.11"
 
 pandas = "2.1.1"
 PyJWT = "2.8.0"
-Requests = "2.31.0"
-# typeguard is removed as being a dependency that is installed by since it causes problems with pyinstaller and nuitka -- add it manually if you prefer to use it.
-# typeguard = "4.1.5"
-colorlog = "6.6.0"
+requests = "2.32.2"
 python-dotenv = "1.0.0"
+# typeguard is removed as being a dependency since it causes problems with pyinstaller and nuitka -- add it manually if you prefer to use it or if you want to run tests
+# typeguard = "4.1.5"
 
 [tool.poetry.dev-dependencies]
+poethepoet = "0.26.1"
 pytest = "7.4.2"
 pytest-cov = "4.1.0"
 mypy = "1.5.1"
 mypy-extensions = "1.0.0"
-types-requests = "2.31.0"
+types-requests = "2.32.0.*"
 pandas-stubs = "2.0.3.*"
 pylint = "2.17.7"
-poethepoet = "0.24.2"
-black = "23.9.1"
+black = "24.4.2"
 
 
 [tool.poe.tasks]
 test = "poetry run pytest -v --cov=tradelocker --cov-report term-missing"
 test_typing = "poetry run mypy src/tradelocker --strict"
 test_pylint = "poetry run pylint tradelocker"
 test_all = ["test", "test_typing", "test_pylint"]
```

### Comparing `tradelocker-0.41.0/src/tradelocker/tradelocker_api.py` & `tradelocker-0.42.0/src/tradelocker/tradelocker_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 import requests
 import pandas as pd
 
 import logging
 
 from tradelocker.utils import (
-    color_logger,
     log_func,
     get_nested_key,
     resolve_lookback_and_timestamps,
     retry,
     tl_typechecked,
     tl_check_type,
     estimate_history_size,
@@ -31,14 +30,16 @@
     InstrumentDetailsType,
     LimitsType,
     LocaleType,
     LogLevelType,
     MarketDepthlistType,
     ModificationParamsType,
     OrderTypeType,
+    RouteNamesType,
+    RateLimitType,
     StopLossType,
     TakeProfitType,
     RequestsMappingType,
     ResolutionType,
     RouteType,
     RouteTypeType,
     SessionDetailsType,
@@ -55,34 +56,33 @@
     OrdersColumns,
     PositionsColumns,
     PriceHistoryColumns,
     InstrumentsColumns,
     int64,
 )
 
-from time import sleep
-
 # More information about the API: https://tradelocker.com/api
 
-# Constants
-_TIMEOUT: Tuple[int, int] = (10, 30)  # (connection_timeout, read_timeout
-_EPS: float = 0.00001
-_MIN_LOT_SIZE: float = (
-    0.01  ## TODO: this should probably be fetched per-instrument from BE
-)
-
-
 class TLAPI:
     """TradeLocker API Client
 
     Implements a REST connection to the TradeLocker REST API.
 
     See https://tradelocker.com/api/ for more information.
     """
 
+    # Constants
+    _TIMEOUT: Tuple[int, int] = (10, 30)  # (connection_timeout, read_timeout
+    _EPS: float = 0.00001
+    _MIN_LOT_SIZE: float = (
+        0.01  ## TODO: this should probably be fetched per-instrument from BE
+    )
+    _LOGGING_FORMAT = "[%(levelname)s %(asctime)s %(module)s.%(funcName)s:%(lineno)d]: %(message)s"
+    _MAX_STRATEGY_ID_LEN = 31
+
     _instances = {}
 
     # This is here to ensure that users don't accidentally create multiple instances
     # of the same TLAPI object, which would lead to multiple connections to the API for no reason.
     # However, different instances can be created with different parameters,
     # or a new instance will be created in case the access token has expired.
     def __new__(cls, *args, **kwargs):
@@ -132,15 +132,15 @@
         if username and password and server:
             self._credentials = {
                 "username": username,
                 "password": password,
                 "server": server,
             }
 
-        self.log = color_logger
+        logging.basicConfig(level=log_level.upper(), format=self._LOGGING_FORMAT)
 
         if self._credentials:
             self._auth_with_password(
                 username=self._credentials["username"],
                 password=self._credentials["password"],
                 server=self._credentials["server"],
             )
@@ -163,15 +163,15 @@
     def get_access_token(self) -> str:
         """Returns the access token. If the token is about to expire, it will be refreshed."""
 
         # If auth token is not set, or refresh token has expired, try fetching a completely new one
         if not self._access_token or time_to_token_expiry(self._refresh_token) < 0:
             if not self._credentials:
                 error_msg = "Cannot fetch or refresh authentication tokens"
-                self.log.critical(error_msg)
+                logging.critical(error_msg)
                 raise Exception(error_msg)
             else:
                 self._auth_with_password(
                     self._credentials["username"],
                     self._credentials["password"],
                     self._credentials["server"],
                 )
@@ -192,23 +192,23 @@
                 self._auth_with_password(
                     self._credentials["username"],
                     self._credentials["password"],
                     self._credentials["server"],
                 )
             else:
                 error_msg = "No refresh token found or token expired"
-                self.log.critical(error_msg)
+                logging.critical(error_msg)
                 raise Exception(error_msg)
         return self._refresh_token
 
     def _set_account_id_and_acc_num(self, account_id: int, acc_num: int) -> None:
         all_accounts: pd.DataFrame = self.get_all_accounts()
 
         if all_accounts.empty:
-            self.log.critical("No accounts found")
+            logging.critical("No accounts found")
             raise Exception("No accounts found")
 
         # Pick the correct account, either by having account_id, or acc_num specified
         if account_id != 0:
             if account_id not in all_accounts["id"].values:
                 raise ValueError(
                     f"account_id '{account_id}' not found in all_accounts:\n{all_accounts} "
@@ -219,15 +219,15 @@
             self.acc_num = int(
                 all_accounts[all_accounts["id"] == account_id]["accNum"].iloc[0]
             )
             self.account_name = all_accounts[all_accounts["id"] == account_id][
                 "name"
             ].iloc[0]
 
-            self.log.debug(
+            logging.debug(
                 f"Logging in using the specified account_id: {account_id}, using acc_num: {self.acc_num}"
             )
 
         elif acc_num != 0:
             if acc_num not in all_accounts["accNum"].values:
                 raise ValueError(
                     f"acc_num '{acc_num}' not found in all_accounts:\n{all_accounts}"
@@ -238,27 +238,27 @@
             self.account_id = int(
                 all_accounts[all_accounts["accNum"] == acc_num]["id"].iloc[0]
             )
             self.account_name = all_accounts[all_accounts["accNum"] == acc_num][
                 "name"
             ].iloc[0]
 
-            self.log.debug(
+            logging.debug(
                 f"Logging in using the specified acc_num: {acc_num}, using account_id: {self.account_id}"
             )
         else:
-            self.log.debug(
+            logging.debug(
                 "Neither account_id nor acc_num specified, using the first account"
             )
             # use the last account in the list
             self.account_id = int(all_accounts["id"].iloc[0])
             self.acc_num = int(all_accounts["accNum"].iloc[0])
             self.account_name = all_accounts["name"].iloc[0]
 
-            self.log.debug(
+            logging.debug(
                 f"Logging in using the first account, account_id: {self.account_id}, acc_num: {self.acc_num}"
             )
 
     def _auth_with_tokens(self, access_token: str, refresh_token: str) -> None:
         """Stores the access and refresh tokens."""
         self._access_token = access_token
         self._refresh_token = refresh_token
@@ -298,24 +298,40 @@
 
     @lru_cache
     def _get_info_route_id(self, instrument_id: int) -> str:
         """Returns the "INFO" route_id for the specified instrument_id"""
         return self._get_route_id(instrument_id, "INFO")
 
     @lru_cache
-    def _get_max_history_rows(self) -> int:
+    def max_price_history_rows(self) -> int:
         config_dict: ConfigType = self.get_config()
         limits: list[LimitsType] = get_nested_key(
             config_dict, ["limits"], list[LimitsType]
         )
         for limit in limits:
             if limit["limitType"] == "QUOTES_HISTORY_BARS":
                 return limit["limit"]
         raise Exception("Failed to fetch max history rows")
 
+    @lru_cache
+    def get_route_rate_limit(self, route_name: RouteNamesType) -> RateLimitType:
+        config_dict: ConfigType = self.get_config()
+        limits: list[LimitsType] = get_nested_key(
+            config_dict, ["rateLimits"], list[RateLimitType]
+        )
+
+        for limit in limits:
+            if limit["rateLimitType"] == route_name:
+                return limit
+
+        raise Exception("Failed to fetch trade rate limit")
+
+    def get_price_history_rate_limit(self) -> RateLimitType:
+        return self.get_route_rate_limit("QUOTES_HISTORY")
+
     @tl_typechecked
     def _get_route_id(self, instrument_id: int, route_type: RouteTypeType) -> str:
         """Returns the route_id for the specified instrument_id and route_type (TRADE/INFO)"""
         all_instruments: pd.DataFrame = self.get_all_instruments()
         matching_instruments: pd.DataFrame = all_instruments[
             all_instruments["tradableInstrumentId"] == instrument_id
         ]
@@ -389,15 +405,15 @@
         if response.text == "":
             raise Exception(f"Empty response received from the API for {response.url}")
 
         try:
             response_json: JSONType = response.json()
             return response_json
         except json.decoder.JSONDecodeError as err:
-            self.log.error(
+            logging.error(
                 f"Failed to decode JSON response from {response.url}. Received response:\n'{response.text}'\n{err}"
             )
             raise err
 
     @retry
     @tl_typechecked
     def _request_get(
@@ -422,15 +438,15 @@
             HTTPError: Will be raised if the request fails
         """
 
         headers = self._get_headers(additional_headers, include_acc_num=include_acc_num)
         params = self._get_params(additional_params)
 
         response = requests.get(
-            url=url, headers=headers, params=params, timeout=_TIMEOUT
+            url=url, headers=headers, params=params, timeout=self._TIMEOUT
         )
         response_json = self._get_response_json(response)
         return response_json
 
     def _apply_typing(
         self, df: pd.DataFrame, column_types: dict[str, type]
     ) -> pd.DataFrame:
@@ -440,33 +456,33 @@
             columns_types (dict[str, type]): The column types to apply
 
         Returns:
             pd.DataFrame: The DataFrame with the types applied
         """
         for column in df.columns:
             if column not in column_types:
-                self.log.error(
+                logging.error(
                     f"Missing type specification for column {column} in {column_types}"
                 )
             else:
                 try:
                     # Only convert the ints and floats after replacing "None" values with 0
                     if column_types[column] in [int64, float]:
                         df[column] = df[column].fillna(0).astype(column_types[column])
 
                 except Exception as err:
-                    self.log.warning(
+                    logging.warning(
                         f"Failed to apply type {column_types[column]} to column {column}: {err}"
                     )
 
     ############################## PUBLIC UTILS #######################
 
-    @tl_typechecked
     @lru_cache
     @log_func
+    @tl_typechecked
     def get_instrument_id_from_symbol_name(self, symbol_name: str) -> int:
         """Returns the instrument Id from the given symol's name.
 
         Args:
             symbol_name (str): Name of the symbol, for example `BTCUSD`
 
         Raises:
@@ -476,15 +492,15 @@
             int: On success the instrument Id will be returned
         """
         all_instruments: pd.DataFrame = self.get_all_instruments()
         matching_instruments = all_instruments[all_instruments["name"] == symbol_name]
         if len(matching_instruments) == 0:
             raise ValueError(f"No instrument found with {symbol_name=}")
         if len(matching_instruments) > 1:
-            self.log.warning(
+            logging.warning(
                 f"Multiple instruments found with {symbol_name=}. Using the first one."
             )
 
         return int(matching_instruments["tradableInstrumentId"].iloc[0])
 
     @log_func
     @tl_typechecked
@@ -501,15 +517,15 @@
             int: On success the instrument Id will be returned
         """
         all_instruments: pd.DataFrame = self.get_all_instruments()
         matching_instruments = all_instruments[all_instruments["id"] == symbol_id]
         if len(matching_instruments) == 0:
             raise ValueError(f"No instrument found with {symbol_id=}")
         if len(matching_instruments) > 1:
-            self.log.warning(
+            logging.warning(
                 f"Multiple instruments found with {symbol_id=}. Using the first one."
             )
 
         return int(matching_instruments["tradableInstrumentId"].iloc[0])
 
     @log_func
     @tl_typechecked
@@ -525,18 +541,18 @@
         all_instruments: pd.DataFrame = self.get_all_instruments()
         matching_instruments = all_instruments[
             all_instruments["tradableInstrumentId"] == instrument_id
         ]
         if len(matching_instruments) == 0:
             raise ValueError(f"No instrument found with id = {instrument_id}")
 
-        self.log.debug(
+        logging.debug(
             f"(get_symbol_name_from_instrument_id) instrument_id: {instrument_id}"
         )
-        self.log.debug(f"matching_instruments:\n{matching_instruments}")
+        logging.debug(f"matching_instruments:\n{matching_instruments}")
         return matching_instruments["name"].iloc[0]
 
     @log_func
     @tl_typechecked
     def close_all_positions(self, instrument_id_filter: int = 0) -> bool:
         """Places an order to close all open positions.
 
@@ -557,44 +573,43 @@
         if instrument_id_filter != 0:
             additional_params = {"tradableInstrumentId": str(instrument_id_filter)}
 
         response = requests.delete(
             route_url,
             headers=self._get_headers(),
             params=self._get_params(additional_params=additional_params),
-            timeout=_TIMEOUT,
+            timeout=self._TIMEOUT,
         )
         response.raise_for_status()
         response_json = self._get_response_json(response)
         response_status: str = get_nested_key(response_json, ["s"], str)
         return response_status == "ok"
 
     @log_func
     @tl_typechecked
     def delete_all_orders_manual(self, instrument_id_filter: int = 0) -> bool:
-        """Deletes all pending orders.
+        """DEPRECATED -- Use delete_all_orders instead -- Deletes all pending orders, one by one.
 
         If instrument_id is provided, only pending orders in this instrument will be closed
 
         Args:
             instrument_id_filter (int, optional): The instrument id to use. Defaults to 0.
 
         Returns:
             bool: True if executed successfully False otherwise
         """
-        route_url = f"{self._base_url}/trade/accounts/{self.account_id}/orders"
+        logging.warning(f"delete_all_orders_manual is deprecated and will be removed in the future. Use delete_all_orders instead.")
 
         orders = self.get_all_orders(
             history=False, instrument_id_filter=instrument_id_filter
         )
         # iterate over all rows of the orders dataframe
         for index, row in orders.iterrows():
             order_id = row["id"]
             self.delete_order(order_id)
-            sleep(1)
 
         return True
 
     @log_func
     @tl_typechecked
     def delete_all_orders(self, instrument_id_filter: int = 0) -> bool:
         """Deletes all pending orders.
@@ -613,15 +628,15 @@
         if instrument_id_filter != 0:
             additional_params = {"tradableInstrumentId": str(instrument_id_filter)}
 
         response = requests.delete(
             route_url,
             headers=self._get_headers(),
             params=self._get_params(additional_params=additional_params),
-            timeout=_TIMEOUT,
+            timeout=self._TIMEOUT,
         )
         response.raise_for_status()
         response_json = self._get_response_json(response)
         response_status: str = get_nested_key(response_json, ["s"], str)
         return response_status == "ok"
 
     @log_func
@@ -634,15 +649,15 @@
         data = {"qty": str(quantity)}
 
         response = requests.delete(
             url=route_url,
             json=data,
             headers=self._get_headers(),
             params=self._get_params(),
-            timeout=_TIMEOUT,
+            timeout=self._TIMEOUT,
         )
         response.raise_for_status()
         response_json = self._get_response_json(response)
         response_status: str = get_nested_key(response_json, ["s"], str)
 
         return response_status == "ok"
 
@@ -666,15 +681,15 @@
 
         Raises:
             ValueError: Will be raised if no order_id or position_id was provided
         """
         if order_id == 0 and position_id == 0:
             raise ValueError("Either order_id or position_id must be provided!")
         if order_id != 0 and position_id != 0:
-            self.log.warning(
+            logging.warning(
                 "Both order_id and position_id provided. position_id will be ignored."
             )
 
         # Important: make sure to use ordersHistory since some orders might have been from previous sessions
         all_orders = self.get_all_orders(history=True)
 
         selection_criteria: str = ""
@@ -685,36 +700,36 @@
             matching_orders = all_orders[all_orders["positionId"] == position_id]
             selection_criteria = f"position_id: {position_id}"
 
         rejected_matching_orders = matching_orders[
             matching_orders["status"] == "Rejected"
         ]
         if len(rejected_matching_orders.index) > 0:
-            self.log.warning(f"Rejected orders found for {selection_criteria}!")
+            logging.warning(f"Rejected orders found for {selection_criteria}!")
 
         # leave only filled orders
         matching_orders = matching_orders[matching_orders["status"] == "Filled"]
 
         if len(matching_orders.index) == 0:
-            self.log.error(f"No matching position found for {selection_criteria}!")
+            logging.error(f"No matching position found for {selection_criteria}!")
 
         if len(matching_orders.index) > 1:
-            self.log.warning(
+            logging.warning(
                 f"Multiple positions found for {selection_criteria}! Attempting to close all: \n{matching_orders}"
             )
 
         for _, row in matching_orders.iterrows():
             quantity_to_close: float = float(row["qty"])
             if close_quantity:
                 quantity_to_close = min(quantity_to_close, close_quantity)
                 close_quantity -= quantity_to_close
 
-            if quantity_to_close < _MIN_LOT_SIZE:
-                self.log.warning(
-                    f"Quantity to close ({quantity_to_close}) is less than minimum lot size ({_MIN_LOT_SIZE}). Skipping."
+            if quantity_to_close < self._MIN_LOT_SIZE:
+                logging.warning(
+                    f"Quantity to close ({quantity_to_close}) is less than minimum lot size ({self._MIN_LOT_SIZE}). Skipping."
                 )
                 continue
 
             self._place_close_position_order(
                 position_id=int(row["positionId"]), quantity=quantity_to_close
             )
 
@@ -732,38 +747,38 @@
         Raises:
             Exception: Will be raised on authentication errors
         """
         route_url = f"{self._base_url}/auth/jwt/token"
 
         data = {"email": username, "password": password, "server": server}
 
-        response = requests.post(url=route_url, json=data, timeout=_TIMEOUT)
+        response = requests.post(url=route_url, json=data, timeout=self._TIMEOUT)
         try:
             response_json = self._get_response_json(response)
             self._access_token = get_nested_key(response_json, ["accessToken"], str)
             self._refresh_token = get_nested_key(response_json, ["refreshToken"], str)
             assert self._access_token and self._refresh_token
-            self.log.info("Successfully fetched authentication tokens")
+            logging.info("Successfully fetched authentication tokens")
         except Exception as err:
-            self.log.critical(f"Failed to fetch authentication tokens: {err}")
+            logging.critical(f"Failed to fetch authentication tokens: {err}")
             # Explicitly re-raise from err
             raise Exception(f"Failed to fetch authentication tokens: {err}") from err
             # raise Exception(f"Failed to fetch authentication tokens: {err}")
 
     @tl_typechecked
     def refresh_access_tokens(self) -> None:
         """Refreshes authentication tokens."""
         route_url = f"{self._base_url}/auth/jwt/refresh"
 
         data = {"refreshToken": self._refresh_token}
 
-        response = requests.post(url=route_url, json=data, timeout=_TIMEOUT)
+        response = requests.post(url=route_url, json=data, timeout=self._TIMEOUT)
         response_json = self._get_response_json(response)
 
-        self.log.info("Successfully refreshed authentication tokens")
+        logging.info("Successfully refreshed authentication tokens")
 
         self._access_token = get_nested_key(response_json, ["accessToken"], str)
         self._refresh_token = get_nested_key(response_json, ["refreshToken"], str)
 
     @lru_cache(maxsize=1)
     @log_func
     @tl_typechecked
@@ -782,27 +797,29 @@
         response_json = self._request_get(route_url, include_acc_num=False)
         accounts_json = get_nested_key(response_json, ["accounts"])
 
         accounts = pd.DataFrame(accounts_json)
         self._apply_typing(accounts, AccountsColumns)
 
         if not accounts_json or accounts.empty:
-            self.log.critical("Failed to fetch user's accounts")
+            logging.critical("Failed to fetch user's accounts")
             raise Exception("Failed to fetch user's accounts")
 
         return accounts
 
     ############################## CONFIG ROUTES ##########################
 
     @lru_cache(maxsize=1)
     @log_func
     @tl_typechecked
     def get_config(self) -> ConfigType:
         """Returns the user's configuration.
 
+        Route Name: GET_CONFIG
+
         Returns:
             ConfigType: The configuration
         """
         route_url = f"{self._base_url}/trade/config"
         response_json = self._request_get(route_url)
         config_dict: ConfigType = get_nested_key(response_json, ["d"], ConfigType)
         return config_dict
@@ -812,14 +829,16 @@
     @log_func
     @tl_typechecked
     def get_trade_accounts(self) -> TradeAccountsType:
         """Returns the account information.
 
         The account is defined by the acc_num used in constructor.
 
+        Route Name: GET_ACCOUNTS
+
         Returns:
             TradeAccountsType: The account details
         """
         route_url = f"{self._base_url}/trade/accounts"
 
         response_json = self._request_get(route_url)
 
@@ -829,14 +848,16 @@
         return trade_accounts
 
     @log_func
     @tl_typechecked
     def get_all_executions(self) -> pd.DataFrame:
         """Returns a list of orders executed in account in current session.
 
+        Route Name: GET_EXECUTIONS
+
         Returns:
             pd.DataFrame[ExecutionsColumnTypes]: DataFrame containing all executed orders
         """
         route_url = f"{self._base_url}/trade/accounts/{self.account_id}/executions"
 
         response_json = self._request_get(route_url)
 
@@ -850,14 +871,16 @@
         return all_executions
 
     @lru_cache(maxsize=1)
     @log_func
     def get_all_instruments(self) -> pd.DataFrame:
         """Returns all available instruments for account.
 
+        route_name = GET_INSTRUMENTS
+
         Returns:
             pd.DataFrame[InstrumentsColumnsTypes]: DataFrame with all available instruments
         """
         route_url = f"{self._base_url}/trade/accounts/{self.account_id}/instruments"
 
         response_json = self._request_get(route_url)
 
@@ -880,14 +903,17 @@
     ) -> pd.DataFrame:
         """Returns all orders associated with the account.
         If history is set to True, it will return all orders from the beginning of the session.
         If history is set to False, it will return only orders that have not been executed yet.
         The default value is False.
         If the account has no orders, an empty DataFrame is returned.
 
+        Route Name: GET_ORDERS
+        Route Name: GET_ORDERS_HISTORY
+
         Args:
             history (bool, optional): Should historical orders be returned. Defaults to False.
 
         Returns:
             pd.DataFrame[OrdersColumnsTypes]: DataFrame containing all orders
         """
         endpoint = "orders" + ("History" if history else "")
@@ -922,14 +948,16 @@
         return all_orders
 
     @log_func
     @tl_typechecked
     def get_all_positions(self) -> pd.DataFrame:
         """Returns all open positions for account.
 
+        Route Name: GET_POSITIONS
+
         Returns:
             pd.DataFrame[PositionsColumnsTypes]: DataFrame containing all positions
         """
         route_url = f"{self._base_url}/trade/accounts/{self.account_id}/positions"
 
         response_json = self._request_get(route_url)
         all_positions_raw = get_nested_key(response_json, ["d", "positions"])
@@ -939,14 +967,21 @@
         self._apply_typing(all_positions, PositionsColumns)
 
         return all_positions
 
     @log_func
     @tl_typechecked
     def get_account_state(self) -> DictValuesType:
+        """Returns the account state.
+
+        Route Name: GET_ACCOUNT_STATE
+
+        Returns:
+            DictValuesType: The account state
+        """
         route_url = f"{self._base_url}/trade/accounts/{self.account_id}/state"
 
         response_json = self._request_get(route_url)
         account_state_values = get_nested_key(
             response_json, ["d", "accountDetailsData"]
         )
         account_state = dict(
@@ -959,14 +994,16 @@
     @log_func
     @tl_typechecked
     def get_instrument_details(
         self, instrument_id: int, locale: LocaleType = "en"
     ) -> InstrumentDetailsType:
         """Returns instrument details for a given instrument Id.
 
+        Route Name: GET_INSTRUMENT_DETAILS
+
         Args:
             instrument_id (int): The instrument Id
             locale (LocaleType, optional): Locale (language) id. Defaults to "en".
 
         Returns:
             InstrumentDetailsType: The instrument details
         """
@@ -983,14 +1020,16 @@
         return instrument_details
 
     @log_func
     @tl_typechecked
     def get_session_details(self, session_id: int) -> SessionDetailsType:
         """Returns details about the session defined by session_id.
 
+        Route Name: GET_SESSION_DETAILS
+
         Args:
             session_id (int): Session id
 
         Returns:
             SessionDetailsType: Session details
         """
         route_url = f"{self._base_url}/trade/sessions/{session_id}"
@@ -1004,14 +1043,16 @@
     @log_func
     @tl_typechecked
     def get_session_status_details(
         self, session_status_id: int
     ) -> SessionStatusDetailsType:
         """Returns details about the session status.
 
+        Route Name: GET_SESSION_STATUSES
+
         Args:
             session_status_id (int): Session id
 
         Returns:
             SessionStatusDetailsType: Session details
         """
         route_url = f"{self._base_url}/trade/sessionStatuses/{session_status_id}"
@@ -1027,14 +1068,16 @@
     @log_func
     @tl_typechecked
     def get_daily_bar(
         self, instrument_id: int, bar_type: Literal["BID", "ASK", "TRADE"] = "ASK"
     ) -> DailyBarType:
         """Returns daily candle data for requested instrument.
 
+        Route Name: DAILY_BAR
+
         Args:
             instrument_id (int): Instrument Id
             bar_type (Literal[BID, ASK, TRADE], optional): The type of candle data to return. Defaults to "ASK".
 
         Returns:
             DailyBarType: Daily candle data
         """
@@ -1054,14 +1097,16 @@
 
     # Returns asks and bids
     @log_func
     @tl_typechecked
     def get_market_depth(self, instrument_id: int) -> MarketDepthlistType:
         """Returns market depth information for the requested instrument.
 
+        Route Name: DEPTH
+
         Args:
             instrument_id (int): Instrument Id
 
         Returns:
             MarketDepthlistType: Market depth data
         """
         route_url = f"{self._base_url}/trade/depth"
@@ -1087,14 +1132,16 @@
         resolution: ResolutionType = "15m",
         lookback_period: str = "",
         start_timestamp: int = 0,  # timestamps are in miliseconds!
         end_timestamp: int = 0,
     ) -> pd.DataFrame:
         """Returns price history data for the requested instrument.
 
+        Route Name: QUOTES_HISTORY
+
         Args:
             instrument_id (int): Instrument Id
             resolution (ResolutionType, optional): Data resolution. Defaults to "15m".
             lookback_period (str, optional): Lookback period (for example "5m"). Defaults to "".
             start_timestamp (int, optional): Start timestamp (in ms). Defaults to 0.
             end_timestamp: (int, optional): End timestamp (in ms). Defaults to 0.
 
@@ -1107,17 +1154,17 @@
         route_url = f"{self._base_url}/trade/history"
 
         start_timestamp, end_timestamp = resolve_lookback_and_timestamps(
             lookback_period, start_timestamp, end_timestamp
         )
 
         history_size = estimate_history_size(start_timestamp, end_timestamp, resolution)
-        if history_size > self._get_max_history_rows():
+        if history_size > self.max_price_history_rows():
             raise ValueError(
-                f"No. of requested rows ({history_size}) larger than max allowed ({self._get_max_history_rows()})."
+                f"No. of requested rows ({history_size}) larger than max allowed ({self.max_price_history_rows()})."
                 "Try splitting your request in smaller chunks."
             )
 
         params: RequestsMappingType = self._get_params(
             {
                 "tradableInstrumentId": instrument_id,
                 "routeId": self._get_info_route_id(instrument_id),
@@ -1131,15 +1178,15 @@
 
         try:
             bar_details = pd.DataFrame(
                 get_nested_key(response_json, ["d", "barDetails"])
             )
         except KeyError as err:
             if response_json["s"] == "no_data":
-                self.log.warning("No data returned from the API for the given period")
+                logging.warning("No data returned from the API for the given period")
                 # Specify column names to make sure they exist even for empty returns
                 bar_details = pd.DataFrame(columns=["t", "o", "h", "l", "c", "v"])
             else:
                 raise err
 
         self._apply_typing(bar_details, PriceHistoryColumns)
 
@@ -1180,14 +1227,16 @@
         return current_bp
 
     @log_func
     @tl_typechecked
     def get_quotes(self, instrument_id: int) -> QuotesType:
         """Returns price quotes for requested instrument.
 
+        Route Name: QUOTES
+
         Args:
             instrument_id (int): Instrument Id
 
         Returns:
             QuotesType: Price quotes for instrument
         """
         route_url = f"{self._base_url}/trade/quotes"
@@ -1237,25 +1286,25 @@
 
         total_netted: float = 0
         for _, position in opposite_positions.iterrows():
             if not position["stopLossId"] and not position["takeProfitId"]:
                 # Compute how much to close in case a partial close would be needed
                 quantity_to_close = min(position["qty"], float(quantity) - total_netted)
 
-                self.log.info(
+                logging.info(
                     "Closing position {position_id}, {quantity_to_close} due to position_netting order {order}"
                 )
                 self.close_position(
                     position_id=position["id"], close_quantity=quantity_to_close
                 )
                 total_netted += quantity_to_close
 
                 # If sufficient orders have been placed, return
-                if abs(total_netted - float(quantity)) < _EPS:
-                    self.log.debug(
+                if abs(total_netted - float(quantity)) < self._EPS:
+                    logging.debug(
                         "New position completely netted from opposite positions."
                     )
                     break
 
         return total_netted
 
     # TODO: add tests for sl/tp
@@ -1271,17 +1320,20 @@
         validity: Optional[ValidityType] = None,
         position_netting: bool = False,
         take_profit: Optional[float] = None,
         take_profit_type: Optional[TakeProfitType] = None,
         stop_loss: Optional[float] = None,
         stop_loss_type: Optional[StopLossType] = None,
         stop_price: Optional[float] = None,
+        strategy_id: Optional[str] = None,
     ) -> Optional[int]:
         """Creates an order.
 
+        Route Name: PLACE_ORDER
+
         Args:
             instrument_id (int): Instrument Id
             quantity (float): Order size
             side (SideType): Order side
             price (float, optional): Price for non-market orders. Defaults to 0.
             type_ (OrderTypeType, optional): Order type. Defaults to "market".
             validity (ValidityType, optional): Validity type of order. Defaults to "IOC".
@@ -1293,210 +1345,221 @@
 
         Returns:
             Optional[int]: Order Id if order created, otherwise None
         """
         route_url = f"{self._base_url}/trade/accounts/{self.account_id}/orders"
 
         if type_ == "market" and price:
-            self.log.warning("Price specified for a market order. Ignoring the price.")
+            logging.warning("Price specified for a market order. Ignoring the price.")
             price = None
 
         if type_ == "market":
             if validity and validity != "IOC":
                 error_msg = (
                     f"Market orders must use IOC as validity. Not placing the order."
                 )
-                self.log.error(error_msg)
+                logging.error(error_msg)
                 raise ValueError(error_msg)
             else:
                 validity = "IOC"
         elif validity and validity != "GTC":
             error_msg = (
                 f"{type_} orders must use GTC as validity. Not placing the order."
             )
-            self.log.error(error_msg)
+            logging.error(error_msg)
             raise ValueError(error_msg)
 
         if stop_loss and not stop_loss_type:
             warning_msg = "Stop loss value specified, but no stop loss type. Continuing with 'absolute'"
-            self.log.warning(warning_msg)
+            logging.warning(warning_msg)
             stop_loss_type = "absolute"
 
         if take_profit and not take_profit_type:
             warning_msg = "Take profit value specified, but no take profit type. Continuing with 'absolute'"
-            self.log.warning(warning_msg)
+            logging.warning(warning_msg)
             take_profit_type = "absolute"
 
         if type == "stop" and stop_price == None:
             if not price:
-                self.log.error(
+                logging.error(
                     "Stop orders must have a stop price set. Not placing the order."
                 )
                 return None
 
             stop_price = price
             price = None
-            self.log.warning(
+            logging.warning(
                 f"Order of {type_ = } specified, but no stop_price set. Using price as stop price."
             )
 
         # Make sure that quantity is positive. If not, switch the side of the order
         if quantity < 0:
             quantity = abs(quantity)
             side = "sell" if (side == "buy") else "buy"
-            self.log.warning(
+            logging.warning(
                 "Quantity was negative, Continuing by changing the side of the order."
             )
 
         # Make sure that quantity is a multiple of 0.01
         floored_quantity = floor(quantity * 100) / 100
-        if abs(quantity - floored_quantity) > _EPS:
+        if abs(quantity - floored_quantity) > self._EPS:
             old_quantity = quantity
             quantity = floored_quantity
-            self.log.warning(
+            logging.warning(
                 f"Quantity {old_quantity} was not a multiple of 0.01."
                 f"Continuing by rounding down the quantity to {quantity}."
             )
 
         # If the quantity is smaller than the minimum lot size, return
-        if quantity < _MIN_LOT_SIZE:
-            self.log.warning(
-                "Unable to place an order with quantity smaller than min lot size of {_MIN_LOT_SIZE}"
+        if quantity < self._MIN_LOT_SIZE:
+            logging.warning(
+                "Unable to place an order with quantity smaller than min lot size of {self._MIN_LOT_SIZE}"
             )
             return None
 
+        if strategy_id and len(strategy_id) > self._MAX_STRATEGY_ID_LEN:
+            raise ValueError(
+                f"Strategy ID {strategy_id} is too long. Max length is {self._MAX_STRATEGY_ID_LEN}"
+            )
+
         request_body = {
             "price": price,
             "stopPrice": stop_price,
             "qty": str(quantity),
             "routeId": self._get_trade_route_id(instrument_id),
             "side": side,
             "validity": validity,
             "tradableInstrumentId": str(instrument_id),
             "type": type_,
             "takeProfit": take_profit,
             "takeProfitType": take_profit_type,
             "stopLoss": stop_loss,
             "stopLossType": stop_loss_type,
             "stopPrice": stop_price,
+            "strategyId": strategy_id,
         }
 
         if position_netting:
             # Try finding opposite orders to net against
             if type_ == "market":
                 total_netted = self._perform_order_netting(
                     instrument_id, side, quantity
                 )
                 # Reduce the necessary quantity by the total_amount that was netted
                 request_body["qty"] = str(float(request_body["qty"]) - total_netted)
-                if float(request_body["qty"]) < _MIN_LOT_SIZE:
-                    self.log.info(
+                if float(request_body["qty"]) < self._MIN_LOT_SIZE:
+                    logging.info(
                         "Not placing a new order after closing sufficient opposite orders due to netting."
                     )
                     return None
             else:
-                self.log.warning(
+                logging.warning(
                     "Order netting is only supported for market orders. Continuing without netting."
                 )
 
         # Place the order
         response = requests.post(
             url=route_url,
             headers=self._get_headers({"Content-type": "application/json"}),
             json=request_body,
-            timeout=_TIMEOUT,
+            timeout=self._TIMEOUT,
         )
         response_json = self._get_response_json(response)
         try:
             order_id: int = int(get_nested_key(response_json, ["d", "orderId"], str))
-            self.log.info(f"Order {request_body} placed with order_id: {order_id}")
+            logging.info(f"Order {request_body} placed with order_id: {order_id}")
             return order_id
         except KeyError as err:
-            self.log.error(f"Unable to place order {request_body}. Error: {err}")
+            logging.error(f"Unable to place order {request_body}. Error: {err}")
             return None
 
     @log_func
     @tl_typechecked
     def delete_order(self, order_id: int) -> bool:
         """Deletes a pending order.
 
+
         Args:
             order_id (int): Order Id
 
         Returns:
             bool: True on success, False on error
         """
         route_url = f"{self._base_url}/trade/orders/{order_id}"
 
-        self.log.info(f"Deleting order with id {order_id}")
+        logging.info(f"Deleting order with id {order_id}")
 
         response = requests.delete(
             url=route_url,
             headers=self._get_headers(),
             params=self._get_params(),
-            timeout=_TIMEOUT,
+            timeout=self._TIMEOUT,
         )
         response_json = self._get_response_json(response)
 
-        self.log.info(f"Order deletion response: {response.json()}")
+        logging.info(f"Order deletion response: {response.json()}")
         response_status: str = get_nested_key(response_json, ["s"], str)
 
         return response_status == "ok"
 
     @log_func
     @tl_typechecked
     def modify_order(
         self, order_id: int, modification_params: ModificationParamsType
     ) -> bool:
         """Modifies a pending order -- a thin wrapper around PATCH /trade/orders/{order_id}.
 
+        Route Name: MODIFY_ORDER
+
         Args:
             order_id (int): Order Id
             modification_params (ModificationParamsType): Order modification details
 
         Returns:
             bool: True on success, False on error
         """
         route_url = f"{self._base_url}/trade/orders/{order_id}"
 
-        self.log.info(f"Modifying the order with id {order_id}")
+        logging.info(f"Modifying the order with id {order_id}")
 
         response = requests.patch(
             url=route_url,
             headers=self._get_headers({"Content-type": "application/json"}),
             json=modification_params,
-            timeout=_TIMEOUT,
+            timeout=self._TIMEOUT,
         )
         response_json = self._get_response_json(response)
         response_status: str = get_nested_key(response_json, ["s"], str)
         return response_status == "ok"
 
     @log_func
     @tl_typechecked
     def modify_position(
         self, position_id: int, modification_params: ModificationParamsType
     ) -> bool:
         """Modifies an open position.
 
+        Route Name: MODIFY_POSITION
+
         Args:
             position_id (int): Position Id
             modification_params (_ModificationParamsType): Position modification details
 
         Returns:
             bool: True on success, False on error
         """
         route_url = f"{self._base_url}/trade/positions/{position_id}"
 
-        self.log.info(f"Modifying the position with id {position_id}")
+        logging.info(f"Modifying the position with id {position_id}")
 
         response = requests.patch(
             url=route_url,
             headers=self._get_headers({"Content-type": "application/json"}),
             json=modification_params,
-            timeout=_TIMEOUT,
+            timeout=self._TIMEOUT,
         )
         response_json = self._get_response_json(response)
         response_status: str = get_nested_key(response_json, ["s"], str)
         return response_status == "ok"
 
     @log_func
     @tl_typechecked
@@ -1505,17 +1568,17 @@
 
         Args:
             order_id (int): An order id
 
         Returns:
             Optional[int]: position_id or None
         """
-        self.log.info(f"Getting execution id from orders history")
+        logging.info(f"Getting execution id from orders history")
         orders_history = self.get_all_orders(history=True)
 
         matching_orders = orders_history[orders_history["id"] == order_id]
         if len(matching_orders) == 0:
-            self.log.info(f"No matching order found for order_id: {order_id}")
+            logging.info(f"No matching order found for order_id: {order_id}")
             return None
 
         position_id = int(matching_orders["positionId"].iloc[0])
         return position_id
```

### Comparing `tradelocker-0.41.0/src/tradelocker/types.py` & `tradelocker-0.42.0/src/tradelocker/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,27 +31,51 @@
     "accountDetailsConfig",
 ]
 ConfigColumnType: TA = list[dict[Literal["id", "description"], str]]
 ColumnConfigValuesType: TA = (
     dict[Literal["id", "title"], str] | dict[Literal["columns"], ConfigColumnType]
 )
 
+
+RouteNamesType: TA = Literal[
+    "GET_ACCOUNTS",
+    "GET_EXECUTIONS",
+    "GET_INSTRUMENTS",
+    "GET_ORDERS",
+    "GET_ORDERS_HISTORY",
+    "GET_POSITIONS",
+    "GET_ACCOUNTS_STATE",
+    "GET_INSTRUMENT_DETAILS",
+    "GET_TRADE_SESSIONS",
+    "GET_SESSION_STATUSES",
+    "PLACE_ORDER",
+    "MODIFY_ORDER",
+    "MODIFY_POSITION",
+    "DAILY_BAR",
+    "QUOTES",
+    "DEPTH",
+    "TRADES",
+    "QUOTES_HISTORY",
+]
+
+RateLimitMeasureTypes: TA = Literal["SECONDS", "MINUTES"]
+
 LimitsType: TA = dict[Literal["limitType", "limit"], str | int | float]
-RateLimitsType: TA = dict[
+RateLimitType: TA = dict[
     Literal["rateLimitType", "measure", "intervalNum", "limit"],
-    str | int | float,
+    int | float | RateLimitMeasureTypes | RouteNamesType,
 ]
 
 ConfigType: TA = (
     dict[Literal["customerAccess"], dict[str, bool]]
     | dict[ColumnConfigKeysType, ColumnConfigValuesType]
     | dict[Literal["limits"], list[LimitsType]]
     | dict[
         Literal["rateLimits"],
-        list[RateLimitsType],
+        list[RateLimitType],
     ]
 )
 
 ResolutionType: TA = Literal["1M", "1W", "1D", "4H", "1H", "30m", "15m", "5m", "1m"]
 ModificationParamsType: TA = dict[
     str, str | float | StopLossType | TakeProfitType | ValidityType
 ]
@@ -81,14 +105,15 @@
     "id": int64,
     "price": float,
     "side": SideType,
     "createdDate": int64,
     "qty": float,
     "orderId": int64,
     "positionId": int64,
+    "tradableInstrumentId": int64,
 }
 
 OrdersColumns: dict[str, type] = {
     "id": int64,
     "tradableInstrumentId": int64,
     "routeId": int64,
     "qty": float,
@@ -105,27 +130,29 @@
     "lastModified": int64,
     "isOpen": bool,
     "positionId": int64,
     "stopLoss": float,
     "stopLossType": StopLossType,
     "takeProfit": float,
     "takeProfitType": TakeProfitType,
+    "strategyId": str,
 }
 
 PositionsColumns: dict[str, type] = {
     "id": int64,
     "tradableInstrumentId": int64,
     "routeId": int64,
     "side": SideType,
     "qty": float,
     "avgPrice": float,
     "stopLossId": int64,
     "takeProfitId": int64,
     "openDate": int64,
     "unrealizedPl": float,
+    "strategyId": str,
 }
 
 PriceHistoryColumns: dict[str, type] = {
     "t": int64,
     "o": float,
     "h": float,
     "l": float,
```

### Comparing `tradelocker-0.41.0/src/tradelocker/utils.py` & `tradelocker-0.42.0/src/tradelocker/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from typing import Any, Callable, Tuple, TypeVar, cast
 import datetime
 import time
 import logging
 import os
 
 from dotenv import dotenv_values
-import colorlog
 import jwt
 
 from .types import ResolutionType, LogLevelType
 
 # This will allow us to keep track of the return type of the functions
 # being decorated.
 RT = TypeVar("RT")  # Return Type
@@ -48,87 +47,35 @@
     "D": 24 * 60 * 60 * MS_COEFF,
     "W": 7 * 24 * 60 * 60 * MS_COEFF,
     "M": 30 * 24 * 60 * 60 * MS_COEFF,
     "Y": 365 * 24 * 60 * 60 * MS_COEFF,
 }
 
 
-class ColorLogger:
-    LOG_LEVELS = {
-        "debug": logging.DEBUG,
-        "info": logging.INFO,
-        "warning": logging.WARNING,
-        "error": logging.ERROR,
-        "critical": logging.CRITICAL,
-    }
-
-    def __init__(self, log_level: LogLevelType = "debug"):
-        self.logger = logging.getLogger()
-
-        # remove all handlers from the new logger
-        for handler in self.logger.handlers[:]:
-            self.logger.removeHandler(handler)
-
-        handler = logging.StreamHandler()
-        handler.setFormatter(
-            colorlog.ColoredFormatter(
-                f"%(log_color)s [%(levelname)s %(asctime)s %(name)s.%(module)s.%(funcName)s:%(lineno)d]: %(message)s",
-                datefmt=None,
-                reset=True,
-                log_colors={
-                    "DEBUG": "thin_white",
-                    "INFO": "green",
-                    "WARNING": "yellow",
-                    "ERROR": "red",
-                    "CRITICAL": "red,bg_white",
-                },
-                secondary_log_colors={},
-                style="%",
-            )
-        )
-
-        self.logger.addHandler(handler)
-        self.set_log_level(log_level)
-
-    def get_logger(self) -> logging.Logger:
-        return self.logger
-
-    def set_log_level(self, log_level: LogLevelType) -> None:
-        if log_level not in self.LOG_LEVELS.keys():
-            raise ValueError(
-                f"log_level ({log_level}) not among {list(self.LOG_LEVELS.keys())}"
-            )
-
-        self.logger.setLevel(self.LOG_LEVELS[log_level])
-
-
-color_logger = ColorLogger(log_level="debug").get_logger()
-
 
 # This decorator logs the function call and its arguments
 def log_func(func: Callable[..., RT]) -> Callable[..., RT]:
     @wraps(func)
     def wrapper(*args: Any, **kwargs: Any) -> RT:
         args_repr = [repr(a) for a in args]
         kwargs_repr = [f"{k}={v!r}" for k, v in kwargs.items()]
         signature = ", ".join(args_repr + kwargs_repr)
 
-        log = args[0].log
-        log.debug(f"**** CALLING {func.__name__}({signature})")
+        logging.debug(f"**** CALLING {func.__name__}({signature})")
 
         return_value = func(*args, **kwargs)
 
         max_return_string_length = 1000
         return_string = repr(return_value)
         if len(return_string) > max_return_string_length:
             return_string = (
                 return_string[:max_return_string_length]
                 + "    ...   ===<< TRUNCATED DUE TO LENGTH >>===   "
             )
-        log.debug(f"**** RETURN from {func.__name__}({signature}):\n{return_string}")
+        logging.debug(f"**** RETURN from {func.__name__}({signature}):\n{return_string}")
 
         return return_value
 
     return cast(Callable[..., RT], wrapper)
 
 
 def retry(func: Callable[..., RT], delay: float = 1) -> Callable[..., RT]:
@@ -216,23 +163,22 @@
         )
 
     if start_timestamp != 0 and end_timestamp != 0 and start_timestamp <= end_timestamp:
         return start_timestamp, end_timestamp
 
     try:
         start_timestamp, end_timestamp = timestamps_from_lookback(lookback_period)
-        # color_logger.warning(
-        #     "Both valid lookback_period and start_timestamp/end_timestamp were provided.\n"
-        #     "Continuing with only the start_timestamp/end_timestamp"
-        # )
+        logging.warning(
+            "Both valid lookback_period and start_timestamp/end_timestamp were provided.\n"
+            "Continuing with only the start_timestamp/end_timestamp"
+        )
     except Exception as err:
-        pass
-        # color_logger.warning(
-        #     f"Invalid lookback_period provided: {err}\nContinuing with only the start_timestamp/end_timestamp"
-        # )
+        logging.warning(
+            f"Invalid lookback_period provided: {err}\nContinuing with only the start_timestamp/end_timestamp"
+        )
 
     return start_timestamp, end_timestamp
 
 
 @tl_typechecked
 def estimate_history_size(
     start_timestamp: int, end_timestamp: int, resolution: ResolutionType
@@ -257,21 +203,30 @@
     remaining_time: float = expiration_time - datetime.datetime.now().timestamp()
     return remaining_time
 
 
 @tl_typechecked
 # Should be called with callers_file = __file__
 def load_env_config(callers_file: str, backup_env_file=".env") -> dict[str, str | int]:
+    """Load the .env file from the path defined in ENV_FILE_PATH or the backup_env_file, relative to current dir
+    """
+
     # Get the current script's directory
-    basedir = os.path.abspath(os.path.dirname(callers_file))
+    script_dir = os.path.abspath(os.path.dirname(callers_file))
 
     env_var_name = "ENV_FILE_PATH"
 
     # read the "$(env_var_name)" environment variable if it exists, otherwise use .env or .env-test
-    env_path = os.environ.get(env_var_name, os.path.join(basedir, backup_env_file))
+    env_path = os.environ.get(env_var_name, os.path.join(script_dir, backup_env_file))
 
     # Load the .env file from that directory
     config: dict[str, str] = dotenv_values(env_path)
     if "tl_acc_num" not in config:
         config["tl_acc_num"] = 0
 
     return config
+
+
+@tl_typechecked
+def is_more_frequent(resolution1: ResolutionType, resolution2: ResolutionType) -> bool:
+    all_resolutions = ["1m", "5m", "15m", "30m", "1H", "4H", "1D", "1W", "1M"]
+    return all_resolutions.index(resolution1) < all_resolutions.index(resolution2)
```

### Comparing `tradelocker-0.41.0/PKG-INFO` & `tradelocker-0.42.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: tradelocker
-Version: 0.41.0
-Summary: TradeLocker Trading API support for Python
+Version: 0.42.0
+Summary: Python client for TradeLocker's Trading API
 License: MIT
-Keywords: tradelocker,api,rest,trading,exchange,algotrading,algo,bots,strategies
+Keywords: tradelocker,api,rest,trading,algotrading,algo,bots,strategies
 Author: TradeLocker
 Author-email: admin@tradelocker.com
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyJWT (==2.8.0)
-Requires-Dist: Requests (==2.31.0)
-Requires-Dist: colorlog (==6.6.0)
 Requires-Dist: pandas (==2.1.1)
 Requires-Dist: python-dotenv (==1.0.0)
+Requires-Dist: requests (==2.32.2)
 Project-URL: Issues, https://github.com/tradelocker/tradelocker-python/issues
 Project-URL: Source, https://github.com/tradelocker/tradelocker-python/
 Description-Content-Type: text/markdown
 
 # TradeLocker Python API Wrapper
 
 This project provides a Python wrapper for TradeLocker's public API. It simplifies the process of making requests to the API by providing Pythonic interfaces.
```

