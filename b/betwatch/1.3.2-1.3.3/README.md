# Comparing `tmp/betwatch-1.3.2.tar.gz` & `tmp/betwatch-1.3.3.tar.gz`

## Comparing `betwatch-1.3.2.tar` & `betwatch-1.3.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 betwatch-1.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 betwatch-1.3.2/requirements-dev.lock
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 betwatch-1.3.2/requirements.lock
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.3.2/.github/dependabot.yml
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 betwatch-1.3.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 betwatch-1.3.2/betwatch/__about__.py
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 betwatch-1.3.2/betwatch/__init__.py
--rw-r--r--   0        0        0    13690 2020-02-02 00:00:00.000000 betwatch-1.3.2/betwatch/client.py
--rw-r--r--   0        0        0    34976 2020-02-02 00:00:00.000000 betwatch-1.3.2/betwatch/client_async.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 betwatch-1.3.2/betwatch/exceptions.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 betwatch-1.3.2/betwatch/queries.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.3.2/betwatch/types/__init__.py
--rw-r--r--   0        0        0     2809 2020-02-02 00:00:00.000000 betwatch-1.3.2/betwatch/types/bookmakers.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.3.2/betwatch/types/exceptions.py
--rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 betwatch-1.3.2/betwatch/types/filters.py
--rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 betwatch-1.3.2/betwatch/types/markets.py
--rw-r--r--   0        0        0    12424 2020-02-02 00:00:00.000000 betwatch-1.3.2/betwatch/types/race.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.3.2/betwatch/types/updates.py
--rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 betwatch-1.3.2/examples/get_race_prices.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 betwatch-1.3.2/examples/get_race_prices_async.py
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 betwatch-1.3.2/examples/get_races.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 betwatch-1.3.2/examples/get_races_async.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 betwatch-1.3.2/examples/get_races_async_lightweight.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 betwatch-1.3.2/examples/subscriptions.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 betwatch-1.3.2/examples/update_rated_prices.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.3.2/tests/__init__.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 betwatch-1.3.2/tests/test_check_last_updated.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 betwatch-1.3.2/tests/test_get_race.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 betwatch-1.3.2/tests/test_get_race_async.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 betwatch-1.3.2/tests/test_get_races.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 betwatch-1.3.2/tests/test_get_races_async.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 betwatch-1.3.2/tests/test_subscribe_race_updates.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 betwatch-1.3.2/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.3.2/LICENSE.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.3.2/README.md
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 betwatch-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 betwatch-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 betwatch-1.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 betwatch-1.3.3/requirements-dev.lock
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 betwatch-1.3.3/requirements.lock
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.3.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 betwatch-1.3.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 betwatch-1.3.3/betwatch/__about__.py
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 betwatch-1.3.3/betwatch/__init__.py
+-rw-r--r--   0        0        0    13690 2020-02-02 00:00:00.000000 betwatch-1.3.3/betwatch/client.py
+-rw-r--r--   0        0        0    34976 2020-02-02 00:00:00.000000 betwatch-1.3.3/betwatch/client_async.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 betwatch-1.3.3/betwatch/exceptions.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 betwatch-1.3.3/betwatch/queries.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.3.3/betwatch/types/__init__.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 betwatch-1.3.3/betwatch/types/bookmakers.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 betwatch-1.3.3/betwatch/types/exceptions.py
+-rw-r--r--   0        0        0     4993 2020-02-02 00:00:00.000000 betwatch-1.3.3/betwatch/types/filters.py
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 betwatch-1.3.3/betwatch/types/markets.py
+-rw-r--r--   0        0        0    12424 2020-02-02 00:00:00.000000 betwatch-1.3.3/betwatch/types/race.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.3.3/betwatch/types/updates.py
+-rw-r--r--   0        0        0     2732 2020-02-02 00:00:00.000000 betwatch-1.3.3/examples/get_race_prices.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 betwatch-1.3.3/examples/get_race_prices_async.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 betwatch-1.3.3/examples/get_races.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 betwatch-1.3.3/examples/get_races_async.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 betwatch-1.3.3/examples/get_races_async_lightweight.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 betwatch-1.3.3/examples/subscriptions.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 betwatch-1.3.3/examples/update_rated_prices.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.3.3/tests/__init__.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 betwatch-1.3.3/tests/test_check_last_updated.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 betwatch-1.3.3/tests/test_get_race.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 betwatch-1.3.3/tests/test_get_race_async.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 betwatch-1.3.3/tests/test_get_races.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 betwatch-1.3.3/tests/test_get_races_async.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 betwatch-1.3.3/tests/test_subscribe_race_updates.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 betwatch-1.3.3/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.3.3/LICENSE.txt
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.3.3/README.md
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 betwatch-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 betwatch-1.3.3/PKG-INFO
```

### Comparing `betwatch-1.3.2/requirements-dev.lock` & `betwatch-1.3.3/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/requirements.lock` & `betwatch-1.3.3/requirements.lock`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/.github/workflows/test.yml` & `betwatch-1.3.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/betwatch/__init__.py` & `betwatch-1.3.3/betwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/betwatch/client.py` & `betwatch-1.3.3/betwatch/client.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/betwatch/client_async.py` & `betwatch-1.3.3/betwatch/client_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/betwatch/queries.py` & `betwatch-1.3.3/betwatch/queries.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/betwatch/types/bookmakers.py` & `betwatch-1.3.3/betwatch/types/bookmakers.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,16 @@
     SPORTCHAMPS = "SportChamps"
     SURGE = "Surge"
     BETESTATE = "Betestate"
     CHASEBET = "Chasebet"
     BET66 = "Bet66"
     BOOKIEPRICE = "BookiePrice"
     PREMIUMBET = "PremiumBet"
+    PULSEBET = "Pulsebet"
+    NOISY = "Noisy"
 
     def __str__(self):
         return self.value
 
     def __repr__(self):
         return self.value
```

### Comparing `betwatch-1.3.2/betwatch/types/filters.py` & `betwatch-1.3.3/betwatch/types/filters.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/betwatch/types/markets.py` & `betwatch-1.3.3/betwatch/types/markets.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/betwatch/types/race.py` & `betwatch-1.3.3/betwatch/types/race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/examples/get_race_prices.py` & `betwatch-1.3.3/examples/get_race_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/examples/get_race_prices_async.py` & `betwatch-1.3.3/examples/get_race_prices_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/examples/get_races.py` & `betwatch-1.3.3/examples/get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/examples/get_races_async.py` & `betwatch-1.3.3/examples/get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/examples/get_races_async_lightweight.py` & `betwatch-1.3.3/examples/get_races_async_lightweight.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/examples/subscriptions.py` & `betwatch-1.3.3/examples/subscriptions.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/examples/update_rated_prices.py` & `betwatch-1.3.3/examples/update_rated_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/tests/test_get_race.py` & `betwatch-1.3.3/tests/test_get_race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/tests/test_get_race_async.py` & `betwatch-1.3.3/tests/test_get_race_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/tests/test_get_races.py` & `betwatch-1.3.3/tests/test_get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/tests/test_get_races_async.py` & `betwatch-1.3.3/tests/test_get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/tests/test_subscribe_race_updates.py` & `betwatch-1.3.3/tests/test_subscribe_race_updates.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/.gitignore` & `betwatch-1.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/LICENSE.txt` & `betwatch-1.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/README.md` & `betwatch-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `betwatch-1.3.2/pyproject.toml` & `betwatch-1.3.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "betwatch"
-version = "1.3.2"
+version = "1.3.3"
 description = 'A Python package for interacting with the Betwatch.com API'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["betwatch", "betting", "sports", "api", "sdk"]
 authors = [{ name = "Jamie Watts", email = "jamie@betwatch.com" }]
 classifiers = [
```

### Comparing `betwatch-1.3.2/PKG-INFO` & `betwatch-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: betwatch
-Version: 1.3.2
+Version: 1.3.3
 Summary: A Python package for interacting with the Betwatch.com API
 Project-URL: Documentation, https://github.com/betwatch/betwatch-sdk-python#readme
 Project-URL: Issues, https://github.com/betwatch/betwatch-sdk-python/issues
 Project-URL: Source, https://github.com/betwatch/betwatch-sdk-python
 Project-URL: Betwatch.com, https://betwatch.com
 Author-email: Jamie Watts <jamie@betwatch.com>
 License-Expression: MIT
```

