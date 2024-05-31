# Comparing `tmp/celery_heimdall-1.0.0.tar.gz` & `tmp/celery_heimdall-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery_heimdall-1.0.0.tar", max compression
+gzip compressed data, was "celery_heimdall-1.0.1.tar", max compression
```

## Comparing `celery_heimdall-1.0.0.tar` & `celery_heimdall-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2023-10-06 14:08:20.806296 celery_heimdall-1.0.0/LICENSE
--rw-r--r--   0        0        0     7601 2023-10-06 14:08:20.806296 celery_heimdall-1.0.0/README.md
--rw-r--r--   0        0        0      196 2023-10-06 14:08:20.806296 celery_heimdall-1.0.0/celery_heimdall/__init__.py
--rw-r--r--   0        0        0     1115 2023-10-06 14:08:20.806296 celery_heimdall-1.0.0/celery_heimdall/config.py
--rw-r--r--   0        0        0       67 2023-10-06 14:08:20.806296 celery_heimdall-1.0.0/celery_heimdall/contrib/README.md
--rw-r--r--   0        0        0        0 2023-10-06 14:08:20.806296 celery_heimdall-1.0.0/celery_heimdall/contrib/__init__.py
--rw-r--r--   0        0        0      746 2023-10-06 14:08:20.806296 celery_heimdall-1.0.0/celery_heimdall/contrib/inspector/README.md
--rw-r--r--   0        0        0        0 2023-10-06 14:08:20.806296 celery_heimdall-1.0.0/celery_heimdall/contrib/inspector/__init__.py
--rw-r--r--   0        0        0     1242 2023-10-06 14:08:20.806296 celery_heimdall-1.0.0/celery_heimdall/contrib/inspector/cli.py
--rw-r--r--   0        0        0     2224 2023-10-06 14:08:20.806296 celery_heimdall-1.0.0/celery_heimdall/contrib/inspector/models.py
--rw-r--r--   0        0        0     5196 2023-10-06 14:08:20.806296 celery_heimdall-1.0.0/celery_heimdall/contrib/inspector/monitor.py
--rw-r--r--   0        0        0      904 2023-10-06 14:08:20.806296 celery_heimdall-1.0.0/celery_heimdall/errors.py
--rw-r--r--   0        0        0    12045 2023-10-06 14:08:20.806296 celery_heimdall-1.0.0/celery_heimdall/task.py
--rw-r--r--   0        0        0      899 2023-10-06 14:08:20.806296 celery_heimdall-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8521 1970-01-01 00:00:00.000000 celery_heimdall-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-31 17:27:36.393829 celery_heimdall-1.0.1/LICENSE
+-rw-r--r--   0        0        0     7601 2024-05-31 17:27:36.393829 celery_heimdall-1.0.1/README.md
+-rw-r--r--   0        0        0      196 2024-05-31 17:27:36.393829 celery_heimdall-1.0.1/celery_heimdall/__init__.py
+-rw-r--r--   0        0        0     1115 2024-05-31 17:27:36.393829 celery_heimdall-1.0.1/celery_heimdall/config.py
+-rw-r--r--   0        0        0       67 2024-05-31 17:27:36.393829 celery_heimdall-1.0.1/celery_heimdall/contrib/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 17:27:36.393829 celery_heimdall-1.0.1/celery_heimdall/contrib/__init__.py
+-rw-r--r--   0        0        0      746 2024-05-31 17:27:36.393829 celery_heimdall-1.0.1/celery_heimdall/contrib/inspector/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 17:27:36.393829 celery_heimdall-1.0.1/celery_heimdall/contrib/inspector/__init__.py
+-rw-r--r--   0        0        0     1242 2024-05-31 17:27:36.393829 celery_heimdall-1.0.1/celery_heimdall/contrib/inspector/cli.py
+-rw-r--r--   0        0        0     2224 2024-05-31 17:27:36.393829 celery_heimdall-1.0.1/celery_heimdall/contrib/inspector/models.py
+-rw-r--r--   0        0        0     5196 2024-05-31 17:27:36.393829 celery_heimdall-1.0.1/celery_heimdall/contrib/inspector/monitor.py
+-rw-r--r--   0        0        0      904 2024-05-31 17:27:36.393829 celery_heimdall-1.0.1/celery_heimdall/errors.py
+-rw-r--r--   0        0        0    12045 2024-05-31 17:27:36.393829 celery_heimdall-1.0.1/celery_heimdall/task.py
+-rw-r--r--   0        0        0      848 2024-05-31 17:27:36.393829 celery_heimdall-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8460 1970-01-01 00:00:00.000000 celery_heimdall-1.0.1/PKG-INFO
```

### Comparing `celery_heimdall-1.0.0/LICENSE` & `celery_heimdall-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `celery_heimdall-1.0.0/README.md` & `celery_heimdall-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `celery_heimdall-1.0.0/celery_heimdall/config.py` & `celery_heimdall-1.0.1/celery_heimdall/config.py`

 * *Files identical despite different names*

### Comparing `celery_heimdall-1.0.0/celery_heimdall/contrib/inspector/README.md` & `celery_heimdall-1.0.1/celery_heimdall/contrib/inspector/README.md`

 * *Files identical despite different names*

### Comparing `celery_heimdall-1.0.0/celery_heimdall/contrib/inspector/cli.py` & `celery_heimdall-1.0.1/celery_heimdall/contrib/inspector/cli.py`

 * *Files identical despite different names*

### Comparing `celery_heimdall-1.0.0/celery_heimdall/contrib/inspector/models.py` & `celery_heimdall-1.0.1/celery_heimdall/contrib/inspector/models.py`

 * *Files identical despite different names*

### Comparing `celery_heimdall-1.0.0/celery_heimdall/contrib/inspector/monitor.py` & `celery_heimdall-1.0.1/celery_heimdall/contrib/inspector/monitor.py`

 * *Files identical despite different names*

### Comparing `celery_heimdall-1.0.0/celery_heimdall/errors.py` & `celery_heimdall-1.0.1/celery_heimdall/errors.py`

 * *Files identical despite different names*

### Comparing `celery_heimdall-1.0.0/celery_heimdall/task.py` & `celery_heimdall-1.0.1/celery_heimdall/task.py`

 * *Files identical despite different names*

### Comparing `celery_heimdall-1.0.0/pyproject.toml` & `celery_heimdall-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "celery-heimdall"
-version = "1.0.0"
+version = "1.0.1"
 description = "Helpful celery extensions."
 authors = ["Tyler Kennedy <tk@tkte.ch>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/tktech/celery-heimdall"
 repository = "https://github.com/tktech/celery-heimdall"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-celery = "^5.2.7"
-redis = "^4.3.4"
-click = {version = "^8.1.3", optional = true}
-SQLAlchemy = {version = "^1.4.40", optional = true}
-importlib-metadata = "<=4.13"
+celery = "*"
+redis = "*"
+click = {version = "*", optional = true}
+SQLAlchemy = {version = "*", optional = true}
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 bumpversion = "^0.6.0"
 coverage = "^6.4.4"
 pytest-cov = "^3.0.0"
 black = "^23.9.1"
```

### Comparing `celery_heimdall-1.0.0/PKG-INFO` & `celery_heimdall-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: celery-heimdall
-Version: 1.0.0
+Version: 1.0.1
 Summary: Helpful celery extensions.
 Home-page: https://github.com/tktech/celery-heimdall
 License: MIT
 Author: Tyler Kennedy
 Author-email: tk@tkte.ch
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: inspector
-Requires-Dist: SQLAlchemy (>=1.4.40,<2.0.0) ; extra == "inspector"
-Requires-Dist: celery (>=5.2.7,<6.0.0)
-Requires-Dist: click (>=8.1.3,<9.0.0) ; extra == "inspector"
-Requires-Dist: importlib-metadata (<=4.13)
-Requires-Dist: redis (>=4.3.4,<5.0.0)
+Requires-Dist: SQLAlchemy ; extra == "inspector"
+Requires-Dist: celery
+Requires-Dist: click ; extra == "inspector"
+Requires-Dist: redis
 Project-URL: Repository, https://github.com/tktech/celery-heimdall
 Description-Content-Type: text/markdown
 
 # celery-heimdall
 
 [![codecov](https://codecov.io/gh/TkTech/celery-heimdall/branch/main/graph/badge.svg?token=1A2CVHQ25Q)](https://codecov.io/gh/TkTech/celery-heimdall)
 ![GitHub](https://img.shields.io/github/license/tktech/celery-heimdall)
```

