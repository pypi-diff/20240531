# Comparing `tmp/python_frank_energie-6.0.0.tar.gz` & `tmp/python_frank_energie-6.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_frank_energie-6.0.0.tar", max compression
+gzip compressed data, was "python_frank_energie-6.1.0b1.tar", max compression
```

## Comparing `python_frank_energie-6.0.0.tar` & `python_frank_energie-6.1.0b1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11346 2024-02-25 13:25:22.585309 python_frank_energie-6.0.0/LICENSE
--rw-r--r--   0        0        0     1442 2024-02-25 13:25:22.585309 python_frank_energie-6.0.0/README.md
--rw-r--r--   0        0        0     2367 2024-02-25 13:25:41.945431 python_frank_energie-6.0.0/pyproject.toml
--rw-r--r--   0        0        0      175 2024-02-25 13:25:22.585309 python_frank_energie-6.0.0/python_frank_energie/__init__.py
--rw-r--r--   0        0        0      378 2024-02-25 13:25:22.585309 python_frank_energie-6.0.0/python_frank_energie/exceptions.py
--rw-r--r--   0        0        0    16174 2024-02-25 13:25:22.585309 python_frank_energie-6.0.0/python_frank_energie/frank_energie.py
--rw-r--r--   0        0        0    13768 2024-02-25 13:25:22.585309 python_frank_energie-6.0.0/python_frank_energie/models.py
--rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 python_frank_energie-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2024-05-31 13:40:16.146368 python_frank_energie-6.1.0b1/LICENSE
+-rw-r--r--   0        0        0     1442 2024-05-31 13:40:16.146368 python_frank_energie-6.1.0b1/README.md
+-rw-r--r--   0        0        0     2374 2024-05-31 13:40:32.426401 python_frank_energie-6.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0      176 2024-05-31 13:40:16.146368 python_frank_energie-6.1.0b1/python_frank_energie/__init__.py
+-rw-r--r--   0        0        0      378 2024-05-31 13:40:16.146368 python_frank_energie-6.1.0b1/python_frank_energie/exceptions.py
+-rw-r--r--   0        0        0    17382 2024-05-31 13:40:16.146368 python_frank_energie-6.1.0b1/python_frank_energie/frank_energie.py
+-rw-r--r--   0        0        0    15617 2024-05-31 13:40:16.146368 python_frank_energie-6.1.0b1/python_frank_energie/models.py
+-rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 python_frank_energie-6.1.0b1/PKG-INFO
```

### Comparing `python_frank_energie-6.0.0/LICENSE` & `python_frank_energie-6.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_frank_energie-6.0.0/README.md` & `python_frank_energie-6.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `python_frank_energie-6.0.0/pyproject.toml` & `python_frank_energie-6.1.0b1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-frank-energie"
-version = "6.0.0"
+version = "6.1.0-beta-1"
 description = "Asynchronous Python client for the Frank Energie"
 authors = ["DCSBL"]
 maintainers = ["DCSBL"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://github.com/dcsbl/python-frank-energie"
 repository = "https://github.com/dcsbl/python-frank-energie"
@@ -19,40 +19,40 @@
 python = "^3.10"
 aiohttp = ">=3.8.0"
 python-dateutil = ">=2.8.0"
 PyJWT = ">=2.8.0"
 syrupy = "^4.6.1"
 
 [tool.poetry.dev-dependencies]
-aresponses = "^2.1.6"
-black = "^22.12"
+aresponses = "^3.0.0"
+black = "^24.3"
 blacken-docs = "^1.15.0"
 flake8 = "^4.0.1"
 flake8-docstrings = "^1.5.0"
 isort = "^5.13.2"
-pre-commit = "^3.6.0"
-pre-commit-hooks = "^4.4.0"
-pylint = "^3.0.3"
-pytest = "^7.4.4"
-pytest-asyncio = "^0.23.4"
-pytest-cov = "^4.1.0"
-pyupgrade = "^3.9.0"
+pre-commit = "^3.7.0"
+pre-commit-hooks = "^4.6.0"
+pylint = "^3.1.0"
+pytest = "^8.2.0"
+pytest-asyncio = "^0.23.6"
+pytest-cov = "^5.0.0"
+pyupgrade = "^3.15.2"
 flake8-simplify = "^0.21.0"
 vulture = "^2.11"
 flake8-bandit = "^3.0.0"
 flake8-bugbear = "^23.3.12"
-flake8-builtins = "^2.1.0"
+flake8-builtins = "^2.5.0"
 flake8-comprehensions = "^3.14.0"
 flake8-eradicate = "^1.2.1"
 flake8-markdown = "^0.3.0"
-freezegun = "^1.4.0"
+freezegun = "^1.5.0"
 darglint = "^1.8.1"
-safety = "^3.0.1"
+safety = "^3.2.0"
 codespell = "^2.2.5"
-bandit = "^1.7.7"
+bandit = "^1.7.8"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/dcsbl/python-frank-energie/issues"
 Changelog = "https://github.com/dcsbl/python-frank-energie/releases"
 
 [tool.black]
 target-version = ['py39']
```

### Comparing `python_frank_energie-6.0.0/python_frank_energie/frank_energie.py` & `python_frank_energie-6.1.0b1/python_frank_energie/frank_energie.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,22 @@
 import asyncio
 from datetime import date
 from typing import Any
 
 from aiohttp.client import ClientError, ClientSession
 
 from .exceptions import AuthException, AuthRequiredException
-from .models import Authentication, Invoices, MarketPrices, Me, MonthSummary
+from .models import (
+    Authentication,
+    Invoices,
+    MarketPrices,
+    Me,
+    MonthSummary,
+    SmartBatteries,
+)
 
 
 class FrankEnergie:
     """FrankEnergie API."""
 
     DATA_URL = "https://frank-graphql-prod.graphcdn.app/"
 
@@ -36,17 +43,19 @@
             self._session = ClientSession()
             self._close_session = True
 
         try:
             resp = await self._session.post(
                 self.DATA_URL,
                 json=query,
-                headers={"Authorization": f"Bearer {self._auth.authToken}"}
-                if self._auth is not None
-                else None,
+                headers=(
+                    {"Authorization": f"Bearer {self._auth.authToken}"}
+                    if self._auth is not None
+                    else None
+                ),
             )
 
             response = await resp.json()
 
         except (asyncio.TimeoutError, ClientError, KeyError) as error:
             raise ValueError(f"Request failed: {error}") from error
 
@@ -478,14 +487,57 @@
             """,
             "variables": {"date": str(start_date), "siteReference": site_reference},
             "operationName": "MarketPrices",
         }
 
         return MarketPrices.from_userprices_dict(await self._query(query_data))
 
+    async def smart_batteries(self) -> SmartBatteries:
+        """Get the users smart batteries.
+
+        Returns a list of all smart batteries.
+
+        Full query:
+        query {
+          smartBatteries {
+            brand
+            capacity
+            createdAt
+            externalReference
+            id
+            maxChargePower
+            maxDischargePower
+            provider
+            updatedAt
+          }
+        }
+        """
+        if self._auth is None:
+            raise AuthRequiredException
+
+        query = {
+            "query": """
+                    query {
+                      smartBatteries {
+                        brand
+                        capacity
+                        createdAt
+                        externalReference
+                        id
+                        maxChargePower
+                        maxDischargePower
+                        provider
+                        updatedAt
+                      }
+                """,
+            "operationName": "SmartBatteries",
+        }
+
+        return SmartBatteries.from_dict(await self._query(query))
+
     @property
     def is_authenticated(self) -> bool:
         """Return if client is authenticated.
 
         Does not actually check if the token is valid.
         """
         return self._auth is not None
```

### Comparing `python_frank_energie-6.0.0/python_frank_energie/models.py` & `python_frank_energie-6.1.0b1/python_frank_energie/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -415,7 +415,64 @@
 
         customerMarketPrices = payload.get("customerMarketPrices")
 
         return MarketPrices(
             electricity=PriceData(customerMarketPrices.get("electricityPrices")),
             gas=PriceData(customerMarketPrices.get("gasPrices")),
         )
+
+
+@dataclass
+class SmartBatteries:
+    """Collection of the users SmartBatteries."""
+
+    smart_batteries: list[SmartBattery]
+
+    @staticmethod
+    def from_dict(data: dict[str, str]) -> SmartBatteries:
+        """Parse the response from the smartBatteries query."""
+        _LOGGER.debug("SmartBatteries %s", data)
+
+        if errors := data.get("errors"):
+            raise RequestException(errors[0]["message"])
+
+        payload = data.get("data")
+        if not payload:
+            raise RequestException("Unexpected response")
+
+        return SmartBatteries(
+            smart_batteries=[
+                SmartBatteries.SmartBattery.from_dict(smart_battery)
+                for smart_battery in payload.get("smartBatteries")
+            ],
+        )
+
+    @dataclass
+    class SmartBattery:
+        """SmartBattery model."""
+
+        brand: str
+        capacity: float
+        external_reference: str
+        id: str
+        max_charge_power: float
+        max_discharge_power: float
+        provider: str
+        created_at: datetime
+        updated_at: datetime
+
+        @staticmethod
+        def from_dict(payload: dict[str, str]) -> SmartBatteries.SmartBattery:
+            """Parse the response from the SmartBatteries query."""
+            _LOGGER.debug("DeliverySites %s", payload)
+
+            return SmartBatteries.SmartBattery(
+                brand=payload.get("brand"),
+                capacity=payload.get("capacity"),
+                external_reference=payload.get("externalReference"),
+                id=payload.get("id"),
+                max_charge_power=payload.get("maxChargePower"),
+                max_discharge_power=payload.get("maxDischargePower"),
+                provider=payload.get("provider"),
+                created_at=payload.get("createdAt"),
+                updated_at=payload.get("updatedAt"),
+            )
```

### Comparing `python_frank_energie-6.0.0/PKG-INFO` & `python_frank_energie-6.1.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-frank-energie
-Version: 6.0.0
+Version: 6.1.0b1
 Summary: Asynchronous Python client for the Frank Energie
 Home-page: https://github.com/dcsbl/python-frank-energie
 License: Apache-2.0
 Author: DCSBL
 Maintainer: DCSBL
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

