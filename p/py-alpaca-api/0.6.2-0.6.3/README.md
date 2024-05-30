# Comparing `tmp/py_alpaca_api-0.6.2.tar.gz` & `tmp/py_alpaca_api-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_alpaca_api-0.6.2.tar", max compression
+gzip compressed data, was "py_alpaca_api-0.6.3.tar", max compression
```

## Comparing `py_alpaca_api-0.6.2.tar` & `py_alpaca_api-0.6.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1066 2024-05-25 20:54:28.642031 py_alpaca_api-0.6.2/LICENSE
--rw-r--r--   0        0        0    17780 2024-05-28 01:41:42.529974 py_alpaca_api-0.6.2/README.md
--rw-r--r--   0        0        0        0 2024-05-25 20:54:28.648697 py_alpaca_api-0.6.2/py_alpaca_api/__init__.py
--rw-r--r--   0        0        0     2275 2024-05-28 01:41:42.533308 py_alpaca_api-0.6.2/py_alpaca_api/alpaca.py
--rw-r--r--   0        0        0        0 2024-05-25 20:54:28.648697 py_alpaca_api-0.6.2/py_alpaca_api/src/__init__.py
--rw-r--r--   0        0        0     6777 2024-05-28 01:41:42.533308 py_alpaca_api-0.6.2/py_alpaca_api/src/account.py
--rw-r--r--   0        0        0     2898 2024-05-28 01:41:42.533308 py_alpaca_api-0.6.2/py_alpaca_api/src/asset.py
--rw-r--r--   0        0        0    11730 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.2/py_alpaca_api/src/data_classes.py
--rw-r--r--   0        0        0     7469 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.2/py_alpaca_api/src/history.py
--rw-r--r--   0        0        0     2984 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.2/py_alpaca_api/src/market.py
--rw-r--r--   0        0        0    20152 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.2/py_alpaca_api/src/order.py
--rw-r--r--   0        0        0     9323 2024-05-28 01:32:55.543711 py_alpaca_api-0.6.2/py_alpaca_api/src/position.py
--rw-r--r--   0        0        0     9587 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.2/py_alpaca_api/src/screener.py
--rw-r--r--   0        0        0    14988 2024-05-28 23:39:58.663626 py_alpaca_api-0.6.2/py_alpaca_api/src/watchlist.py
--rw-r--r--   0        0        0     1344 2024-05-28 23:39:58.663626 py_alpaca_api-0.6.2/pyproject.toml
--rw-r--r--   0        0        0    18582 1970-01-01 00:00:00.000000 py_alpaca_api-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-25 20:54:28.642031 py_alpaca_api-0.6.3/LICENSE
+-rw-r--r--   0        0        0    17780 2024-05-28 01:41:42.529974 py_alpaca_api-0.6.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-25 20:54:28.648697 py_alpaca_api-0.6.3/py_alpaca_api/__init__.py
+-rw-r--r--   0        0        0     2275 2024-05-28 01:41:42.533308 py_alpaca_api-0.6.3/py_alpaca_api/alpaca.py
+-rw-r--r--   0        0        0        0 2024-05-25 20:54:28.648697 py_alpaca_api-0.6.3/py_alpaca_api/src/__init__.py
+-rw-r--r--   0        0        0     6777 2024-05-28 01:41:42.533308 py_alpaca_api-0.6.3/py_alpaca_api/src/account.py
+-rw-r--r--   0        0        0     2898 2024-05-28 01:41:42.533308 py_alpaca_api-0.6.3/py_alpaca_api/src/asset.py
+-rw-r--r--   0        0        0    11730 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.3/py_alpaca_api/src/data_classes.py
+-rw-r--r--   0        0        0     7469 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.3/py_alpaca_api/src/history.py
+-rw-r--r--   0        0        0     2984 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.3/py_alpaca_api/src/market.py
+-rw-r--r--   0        0        0    20152 2024-05-28 01:41:42.536641 py_alpaca_api-0.6.3/py_alpaca_api/src/order.py
+-rw-r--r--   0        0        0     9323 2024-05-28 01:32:55.543711 py_alpaca_api-0.6.3/py_alpaca_api/src/position.py
+-rw-r--r--   0        0        0     9600 2024-05-30 22:46:51.399125 py_alpaca_api-0.6.3/py_alpaca_api/src/screener.py
+-rw-r--r--   0        0        0    14988 2024-05-28 23:39:58.663626 py_alpaca_api-0.6.3/py_alpaca_api/src/watchlist.py
+-rw-r--r--   0        0        0     1344 2024-05-30 22:46:51.399125 py_alpaca_api-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0    18582 1970-01-01 00:00:00.000000 py_alpaca_api-0.6.3/PKG-INFO
```

### Comparing `py_alpaca_api-0.6.2/LICENSE` & `py_alpaca_api-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.2/README.md` & `py_alpaca_api-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.2/py_alpaca_api/alpaca.py` & `py_alpaca_api-0.6.3/py_alpaca_api/alpaca.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.2/py_alpaca_api/src/account.py` & `py_alpaca_api-0.6.3/py_alpaca_api/src/account.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.2/py_alpaca_api/src/asset.py` & `py_alpaca_api-0.6.3/py_alpaca_api/src/asset.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.2/py_alpaca_api/src/data_classes.py` & `py_alpaca_api-0.6.3/py_alpaca_api/src/data_classes.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.2/py_alpaca_api/src/history.py` & `py_alpaca_api-0.6.3/py_alpaca_api/src/history.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.2/py_alpaca_api/src/market.py` & `py_alpaca_api-0.6.3/py_alpaca_api/src/market.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.2/py_alpaca_api/src/order.py` & `py_alpaca_api-0.6.3/py_alpaca_api/src/order.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.2/py_alpaca_api/src/position.py` & `py_alpaca_api-0.6.3/py_alpaca_api/src/position.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.2/py_alpaca_api/src/screener.py` & `py_alpaca_api-0.6.3/py_alpaca_api/src/screener.py`

 * *Files 2% similar despite different names*

```diff
@@ -227,15 +227,15 @@
                         "change": change,
                         "price": bar[1][1]["c"],
                         "volume": bar[1][1]["v"],
                         "trades": bar[1][1]["n"],
                     }
                     all_bars_df = pd.concat([all_bars_df, pd.DataFrame([sym_data])])
 
-                except KeyError:
+                except TypeError or KeyError:
                     pass
             all_bars_df.reset_index(drop=True, inplace=True)
             return all_bars_df
         else:
             raise ValueError(f"Failed to get assets. Response: {response.text}")
 
     ##################################################
```

### Comparing `py_alpaca_api-0.6.2/py_alpaca_api/src/watchlist.py` & `py_alpaca_api-0.6.3/py_alpaca_api/src/watchlist.py`

 * *Files identical despite different names*

### Comparing `py_alpaca_api-0.6.2/pyproject.toml` & `py_alpaca_api-0.6.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-alpaca-api"
-version = "0.6.2"
+version = "0.6.3"
 description = "Python package, for communicating with Alpaca Markets REST API."
 authors = ["TexasCoding <jeff10278@me.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/TexasCoding/py-alpaca-api"
 repository = "https://github.com/TexasCoding/py-alpaca-api"
 documentation = "https://py-alpaca-api.readthedocs.io/en/latest/"
```

### Comparing `py_alpaca_api-0.6.2/PKG-INFO` & `py_alpaca_api-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-alpaca-api
-Version: 0.6.2
+Version: 0.6.3
 Summary: Python package, for communicating with Alpaca Markets REST API.
 Home-page: https://github.com/TexasCoding/py-alpaca-api
 License: MIT
 Keywords: alpaca,python
 Author: TexasCoding
 Author-email: jeff10278@me.com
 Requires-Python: >=3.12,<4.0
```

