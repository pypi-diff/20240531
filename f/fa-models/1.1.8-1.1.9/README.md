# Comparing `tmp/fa-models-1.1.8.tar.gz` & `tmp/fa-models-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fa-models-1.1.8.tar", last modified: Wed Jan 10 19:44:28 2024, max compression
+gzip compressed data, was "fa-models-1.1.9.tar", last modified: Thu Jan 18 16:54:39 2024, max compression
```

## Comparing `fa-models-1.1.8.tar` & `fa-models-1.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:44:28.002564 fa-models-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-01-10 19:44:28.002564 fa-models-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-01-10 19:44:07.000000 fa-models-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:44:28.002564 fa-models-1.1.8/fa_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-01-10 19:44:27.000000 fa-models-1.1.8/fa_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-01-10 19:44:27.000000 fa-models-1.1.8/fa_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-10 19:44:27.000000 fa-models-1.1.8/fa_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-10 19:44:27.000000 fa-models-1.1.8/fa_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-10 19:44:27.000000 fa-models-1.1.8/fa_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:44:27.998564 fa-models-1.1.8/famodels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/direction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:44:27.998564 fa-models-1.1.8/famodels/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/exchange/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/exchange/connection_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/exchange/exchange_connection_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/investor.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/investor_statement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:44:27.998564 fa-models-1.1.8/famodels/market/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/market/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/market/public_trade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/order.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/order_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/person.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/qualified_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/raw_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/rejected_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/side.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/signal_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/status_of_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/trade.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-01-10 19:44:07.000000 fa-models-1.1.8/famodels/virtual_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-01-10 19:44:21.000000 fa-models-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-10 19:44:28.002564 fa-models-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-01-10 19:44:07.000000 fa-models-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-10 19:44:28.002564 fa-models-1.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-01-10 19:44:07.000000 fa-models-1.1.8/tests/test_investor.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-10 19:44:07.000000 fa-models-1.1.8/tests/test_processed_trading_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-01-10 19:44:07.000000 fa-models-1.1.8/tests/test_raw_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-01-10 19:44:07.000000 fa-models-1.1.8/tests/test_rejected_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:54:39.300178 fa-models-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-01-18 16:54:39.300178 fa-models-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-01-18 16:54:18.000000 fa-models-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:54:39.296178 fa-models-1.1.9/fa_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-01-18 16:54:39.000000 fa-models-1.1.9/fa_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-01-18 16:54:39.000000 fa-models-1.1.9/fa_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 16:54:39.000000 fa-models-1.1.9/fa_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-18 16:54:39.000000 fa-models-1.1.9/fa_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-18 16:54:39.000000 fa-models-1.1.9/fa_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:54:39.296178 fa-models-1.1.9/famodels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/direction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:54:39.296178 fa-models-1.1.9/famodels/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/exchange/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/exchange/connection_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/exchange/exchange_connection_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/investor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/investor_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:54:39.296178 fa-models-1.1.9/famodels/market/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/market/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/market/public_trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/order_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/qualified_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/raw_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/rejected_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/side.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/signal_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/status_of_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/trade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-01-18 16:54:18.000000 fa-models-1.1.9/famodels/virtual_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-01-18 16:54:32.000000 fa-models-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 16:54:39.300178 fa-models-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-01-18 16:54:18.000000 fa-models-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:54:39.296178 fa-models-1.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7110 2024-01-18 16:54:18.000000 fa-models-1.1.9/tests/test_investor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-18 16:54:18.000000 fa-models-1.1.9/tests/test_processed_trading_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-01-18 16:54:18.000000 fa-models-1.1.9/tests/test_raw_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-01-18 16:54:18.000000 fa-models-1.1.9/tests/test_rejected_signal.py
```

### Comparing `fa-models-1.1.8/PKG-INFO` & `fa-models-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.1.8
+Version: 1.1.9
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
@@ -49,14 +49,19 @@
 ```
 Start the Environment: 
 ```
 ./.venv/Scripts/activate
 ```
  (or allow VS Code to start it). Use `deactivate`to stop it.
 
+Upgrade the PIP.
+```
+python -m pip install --upgrade pip
+```
+
 All the required libraries must be listed in requirements.txt and installed by  
 ```
 python -m pip install -r .\requirements.txt
 ```
 For Dev use 
 ```
 python -m pip install -r .\requirements-dev.txt
@@ -86,15 +91,15 @@
 
 ## Releasing a new version
 
 Simply commit and push into MAIN. Make sure you have tested well.
 
 Github Actions (.github/workflows/testing_and_deployment.yml) will deploy the file to pypi.org.
 
------
+### Manual and old process
 
 Delete any old files in the /dist and build folder of your local environment.
 Update your pip: 
 ```
 python -m pip install --upgrade pip
 ```
```

### Comparing `fa-models-1.1.8/README.md` & `fa-models-1.1.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -29,14 +29,19 @@
 ```
 Start the Environment: 
 ```
 ./.venv/Scripts/activate
 ```
  (or allow VS Code to start it). Use `deactivate`to stop it.
 
+Upgrade the PIP.
+```
+python -m pip install --upgrade pip
+```
+
 All the required libraries must be listed in requirements.txt and installed by  
 ```
 python -m pip install -r .\requirements.txt
 ```
 For Dev use 
 ```
 python -m pip install -r .\requirements-dev.txt
@@ -66,15 +71,15 @@
 
 ## Releasing a new version
 
 Simply commit and push into MAIN. Make sure you have tested well.
 
 Github Actions (.github/workflows/testing_and_deployment.yml) will deploy the file to pypi.org.
 
------
+### Manual and old process
 
 Delete any old files in the /dist and build folder of your local environment.
 Update your pip: 
 ```
 python -m pip install --upgrade pip
 ```
```

### Comparing `fa-models-1.1.8/fa_models.egg-info/PKG-INFO` & `fa-models-1.1.9/fa_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fa-models
-Version: 1.1.8
+Version: 1.1.9
 Summary: A simple library of trading models.
 Author-email: Brayan Svan <brayan@freyaalpha.com>
 Project-URL: Homepage, https://github.com/svabra/fa-models
 Keywords: finance,trading,models
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
@@ -49,14 +49,19 @@
 ```
 Start the Environment: 
 ```
 ./.venv/Scripts/activate
 ```
  (or allow VS Code to start it). Use `deactivate`to stop it.
 
+Upgrade the PIP.
+```
+python -m pip install --upgrade pip
+```
+
 All the required libraries must be listed in requirements.txt and installed by  
 ```
 python -m pip install -r .\requirements.txt
 ```
 For Dev use 
 ```
 python -m pip install -r .\requirements-dev.txt
@@ -86,15 +91,15 @@
 
 ## Releasing a new version
 
 Simply commit and push into MAIN. Make sure you have tested well.
 
 Github Actions (.github/workflows/testing_and_deployment.yml) will deploy the file to pypi.org.
 
------
+### Manual and old process
 
 Delete any old files in the /dist and build folder of your local environment.
 Update your pip: 
 ```
 python -m pip install --upgrade pip
 ```
```

### Comparing `fa-models-1.1.8/fa_models.egg-info/SOURCES.txt` & `fa-models-1.1.9/fa_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/famodels/investor.py` & `fa-models-1.1.9/famodels/investor.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/famodels/investor_statement.py` & `fa-models-1.1.9/famodels/investor_statement.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/famodels/market/public_trade.py` & `fa-models-1.1.9/famodels/market/public_trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/famodels/order.py` & `fa-models-1.1.9/famodels/order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/famodels/person.py` & `fa-models-1.1.9/famodels/person.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/famodels/qualified_signal.py` & `fa-models-1.1.9/famodels/qualified_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/famodels/raw_signal.py` & `fa-models-1.1.9/famodels/raw_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/famodels/rejected_signal.py` & `fa-models-1.1.9/famodels/rejected_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/famodels/signal_provider.py` & `fa-models-1.1.9/famodels/signal_provider.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/famodels/strategy.py` & `fa-models-1.1.9/famodels/strategy.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/famodels/trade.py` & `fa-models-1.1.9/famodels/trade.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/famodels/trading_signal.py` & `fa-models-1.1.9/famodels/trading_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/famodels/virtual_order.py` & `fa-models-1.1.9/famodels/virtual_order.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/pyproject.toml` & `fa-models-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=66.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fa-models"
-version = "1.1.8"
+version = "1.1.9"
 description = "A simple library of trading models."
 readme = "README.md"
 authors = [{ name = "Brayan Svan", email = "brayan@freyaalpha.com" }]
 #license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python"
@@ -25,15 +25,15 @@
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/svabra/fa-models"
 
 [tool.bumpver]
-current_version = "1.1.8"
+current_version = "1.1.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fa-models-1.1.8/setup.py` & `fa-models-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/tests/test_investor.py` & `fa-models-1.1.9/tests/test_investor.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/tests/test_raw_signal.py` & `fa-models-1.1.9/tests/test_raw_signal.py`

 * *Files identical despite different names*

### Comparing `fa-models-1.1.8/tests/test_rejected_signal.py` & `fa-models-1.1.9/tests/test_rejected_signal.py`

 * *Files identical despite different names*

