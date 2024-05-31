# Comparing `tmp/exchange_calendars_extensions_api-0.4.1.tar.gz` & `tmp/exchange_calendars_extensions_api-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchange_calendars_extensions_api-0.4.1.tar", max compression
+gzip compressed data, was "exchange_calendars_extensions_api-0.4.2.tar", max compression
```

## Comparing `exchange_calendars_extensions_api-0.4.1.tar` & `exchange_calendars_extensions_api-0.4.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-05-23 14:23:50.295657 exchange_calendars_extensions_api-0.4.1/LICENSE
--rw-r--r--   0        0        0      761 2024-05-23 14:23:50.295657 exchange_calendars_extensions_api-0.4.1/README.md
--rw-r--r--   0        0        0      530 2024-05-23 14:23:50.295657 exchange_calendars_extensions_api-0.4.1/exchange_calendars_extensions/api/__init__.py
--rw-r--r--   0        0        0    18798 2024-05-23 14:23:50.295657 exchange_calendars_extensions_api-0.4.1/exchange_calendars_extensions/api/changes.py
--rw-r--r--   0        0        0       18 2024-05-23 14:24:01.583822 exchange_calendars_extensions_api-0.4.1/exchange_calendars_extensions/api/version.py
--rw-r--r--   0        0        0     2719 2024-05-23 14:24:01.515821 exchange_calendars_extensions_api-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 exchange_calendars_extensions_api-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-31 21:03:05.841771 exchange_calendars_extensions_api-0.4.2/LICENSE
+-rw-r--r--   0        0        0      761 2024-05-31 21:03:05.841771 exchange_calendars_extensions_api-0.4.2/README.md
+-rw-r--r--   0        0        0      530 2024-05-31 21:03:05.841771 exchange_calendars_extensions_api-0.4.2/exchange_calendars_extensions/api/__init__.py
+-rw-r--r--   0        0        0    18798 2024-05-31 21:03:05.841771 exchange_calendars_extensions_api-0.4.2/exchange_calendars_extensions/api/changes.py
+-rw-r--r--   0        0        0       18 2024-05-31 21:03:18.197961 exchange_calendars_extensions_api-0.4.2/exchange_calendars_extensions/api/version.py
+-rw-r--r--   0        0        0     2703 2024-05-31 21:03:18.133960 exchange_calendars_extensions_api-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 exchange_calendars_extensions_api-0.4.2/PKG-INFO
```

### Comparing `exchange_calendars_extensions_api-0.4.1/LICENSE` & `exchange_calendars_extensions_api-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions_api-0.4.1/README.md` & `exchange_calendars_extensions_api-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions_api-0.4.1/exchange_calendars_extensions/api/__init__.py` & `exchange_calendars_extensions_api-0.4.2/exchange_calendars_extensions/api/__init__.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions_api-0.4.1/exchange_calendars_extensions/api/changes.py` & `exchange_calendars_extensions_api-0.4.2/exchange_calendars_extensions/api/changes.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions_api-0.4.1/pyproject.toml` & `exchange_calendars_extensions_api-0.4.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "exchange-calendars-extensions-api"
-version = "0.4.1"
+version = "0.4.2"
 description = "A package that defines parts of the API of the exchange-calendars-extensions package."
 license = "Apache-2.0"
 authors = ["Jens Keiner <jens.keiner@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jenskeiner/exchange_calendars_extensions_api/"
 repository = "https://github.com/jenskeiner/exchange_calendars_extensions_api/"
 documentation = "https://github.com/jenskeiner/exchange_calendars_extensions_api/tree/main/docs/"
@@ -29,20 +29,20 @@
 ]
 packages = [{include = "exchange_calendars_extensions"}]
 
 [tool.poetry.dependencies]
 python = "~=3.9"
 typing-extensions = ">=4.0,<5"
 pydantic = ">=2,<3"
-pandas = "^2"
+pandas = ">=1,<3"
 
 [tool.poetry.group.dev.dependencies]
-pytest = ">=7.3.1,<8.3.0"
-pytest-cov = ">=4.1,<5.1"
-pre-commit = ">=3.3.3,<3.8.0"
+pytest = ">=8,<9"
+pytest-cov = ">=5,<6"
+pre-commit = ">=3,<4"
 
 [tool.pytest.ini_options]
 addopts = "--cov=exchange_calendars_extensions.api --cov-report=term-missing"
 
 [tool.ruff]
 # Exclude a variety of commonly ignored directories.
 exclude = [
```

### Comparing `exchange_calendars_extensions_api-0.4.1/PKG-INFO` & `exchange_calendars_extensions_api-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchange-calendars-extensions-api
-Version: 0.4.1
+Version: 0.4.2
 Summary: A package that defines parts of the API of the exchange-calendars-extensions package.
 Home-page: https://github.com/jenskeiner/exchange_calendars_extensions_api/
 License: Apache-2.0
 Keywords: keywords...
 Author: Jens Keiner
 Author-email: jens.keiner@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Dist: pandas (>=2,<3)
+Requires-Dist: pandas (>=1,<3)
 Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: typing-extensions (>=4.0,<5)
 Project-URL: Documentation, https://github.com/jenskeiner/exchange_calendars_extensions_api/tree/main/docs/
 Project-URL: Repository, https://github.com/jenskeiner/exchange_calendars_extensions_api/
 Description-Content-Type: text/markdown
 
 # exchange-calendars-extensions-api
```

