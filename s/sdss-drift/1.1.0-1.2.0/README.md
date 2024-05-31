# Comparing `tmp/sdss_drift-1.1.0.tar.gz` & `tmp/sdss_drift-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_drift-1.1.0.tar", max compression
+gzip compressed data, was "sdss_drift-1.2.0.tar", max compression
```

## Comparing `sdss_drift-1.1.0.tar` & `sdss_drift-1.2.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1504 2023-09-13 06:36:38.546223 sdss_drift-1.1.0/LICENSE.md
--rw-r--r--   0        0        0     1984 2023-09-13 06:36:38.546223 sdss_drift-1.1.0/README.md
--rw-r--r--   0        0        0     2529 2023-09-13 06:36:38.546223 sdss_drift-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      556 2023-09-13 06:36:38.546223 sdss_drift-1.1.0/python/drift/__init__.py
--rw-r--r--   0        0        0     2868 2023-09-13 06:36:38.546223 sdss_drift-1.1.0/python/drift/adaptors.py
--rw-r--r--   0        0        0    26480 2023-09-13 06:36:38.550223 sdss_drift-1.1.0/python/drift/drift.py
--rw-r--r--   0        0        0      614 2023-09-13 06:36:38.550223 sdss_drift-1.1.0/python/drift/exceptions.py
--rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 sdss_drift-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-05-31 05:07:49.220332 sdss_drift-1.2.0/LICENSE.md
+-rw-r--r--   0        0        0     1984 2024-05-31 05:07:49.220332 sdss_drift-1.2.0/README.md
+-rw-r--r--   0        0        0     2348 2024-05-31 05:07:49.224333 sdss_drift-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      556 2024-05-31 05:07:49.224333 sdss_drift-1.2.0/python/drift/__init__.py
+-rw-r--r--   0        0        0     2868 2024-05-31 05:07:49.224333 sdss_drift-1.2.0/python/drift/adaptors.py
+-rw-r--r--   0        0        0     3406 2024-05-31 05:07:49.224333 sdss_drift-1.2.0/python/drift/convert.py
+-rw-r--r--   0        0        0    26480 2024-05-31 05:07:49.224333 sdss_drift-1.2.0/python/drift/drift.py
+-rw-r--r--   0        0        0      614 2024-05-31 05:07:49.224333 sdss_drift-1.2.0/python/drift/exceptions.py
+-rw-r--r--   0        0        0     3155 1970-01-01 00:00:00.000000 sdss_drift-1.2.0/PKG-INFO
```

### Comparing `sdss_drift-1.1.0/LICENSE.md` & `sdss_drift-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_drift-1.1.0/README.md` & `sdss_drift-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sdss_drift-1.1.0/pyproject.toml` & `sdss_drift-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-drift"
-version = "1.1.0"
+version = "1.2.0"
 description = "Modbus PLC control library"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/drift"
 repository = "https://github.com/sdss/drift"
 documentation = "https://sdss-drift.readthedocs.org"
@@ -25,66 +25,56 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 sdsstools = "^1.0.0"
 pymodbus = "^3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = ">=7.11.0"
-flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
-isort = ">=4.3.21"
 ipdb = ">=0.12.3"
 rstcheck = ">=3.3.1"
-black = ">=20.8b1"
-ruff = ">=0.0.289"
-
-[tool.poetry.group.test]
-optional = true
-
-[tool.poetry.group.test.dependencies]
+black = ">=24.1.1"
+ruff = ">=0.4.0"
 pytest = ">=5.2.2"
 pytest-asyncio = ">=0.10.0"
 pytest-cov = ">=2.8.1"
 pytest-mock = ">=1.13.0"
 pytest-sugar = ">=0.9.2"
 coverage = {version = ">=5.0", extras = ["toml"]}
-
-[tool.poetry.group.docs]
-optional = true
-
-[tool.poetry.group.docs.dependencies]
 Sphinx = ">=3.5.2"
 myst-parser = ">=0.14.0"
 furo = ">=2021.6.18-beta.36"
 nox = ">=2021.6.12"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-copybutton = ">=0.3.3"
-sphinx-click = {version = ">=2.3.0"}
+sphinx-click = ">=2.3.0"
 sphinx-jsonschema = ">=1.16.8"
 
 [tool.black]
 line-length = 88
-target-version = ['py311']
+target-version = ['py312']
 fast = true
 
 [tool.ruff]
 line-length = 88
-target-version = 'py311'
+target-version = 'py312'
+
+[tool.ruff.lint]
 select = ["E", "F", "I"]
 unfixable = ["F841"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401", "F403", "E402"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["drift"]
 lines-after-imports = 2
 section-order = ["future", "standard-library", "typing", "third-party", "sdss", "first-party", "local-folder"]
 
-[tool.ruff.isort.sections]
+[tool.ruff.lint.isort.sections]
 typing = ["typing"]
 sdss = ["sdsstools"]
 
 [tool.pytest.ini_options]
 addopts = "--cov drift --cov-report xml --cov-report html --cov-report term -W ignore"
 asyncio_mode = "auto"
```

### Comparing `sdss_drift-1.1.0/python/drift/__init__.py` & `sdss_drift-1.2.0/python/drift/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_drift-1.1.0/python/drift/adaptors.py` & `sdss_drift-1.2.0/python/drift/adaptors.py`

 * *Files identical despite different names*

### Comparing `sdss_drift-1.1.0/python/drift/drift.py` & `sdss_drift-1.2.0/python/drift/drift.py`

 * *Files identical despite different names*

### Comparing `sdss_drift-1.1.0/python/drift/exceptions.py` & `sdss_drift-1.2.0/python/drift/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_drift-1.1.0/PKG-INFO` & `sdss_drift-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-drift
-Version: 1.1.0
+Version: 1.2.0
 Summary: Modbus PLC control library
 Home-page: https://github.com/sdss/drift
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.8,<4.0
@@ -13,14 +13,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pymodbus (>=3.0.0,<4.0.0)
 Requires-Dist: sdsstools (>=1.0.0,<2.0.0)
 Project-URL: Documentation, https://sdss-drift.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/drift
```

