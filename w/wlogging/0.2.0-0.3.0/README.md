# Comparing `tmp/wlogging-0.2.0.tar.gz` & `tmp/wlogging-0.3.0.tar.gz`

## Comparing `wlogging-0.2.0.tar` & `wlogging-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 wlogging-0.2.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 wlogging-0.2.0/src/wlogging/__init__.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 wlogging-0.2.0/src/wlogging/formatters.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 wlogging-0.2.0/src/wlogging/loggers.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 wlogging-0.2.0/.gitignore
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 wlogging-0.2.0/README.md
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 wlogging-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 wlogging-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 wlogging-0.3.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 wlogging-0.3.0/src/wlogging/__init__.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 wlogging-0.3.0/src/wlogging/formatters.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 wlogging-0.3.0/src/wlogging/loggers.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 wlogging-0.3.0/.gitignore
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 wlogging-0.3.0/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 wlogging-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 wlogging-0.3.0/PKG-INFO
```

### Comparing `wlogging-0.2.0/.github/workflows/publish-to-pypi.yml` & `wlogging-0.3.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `wlogging-0.2.0/src/wlogging/__init__.py` & `wlogging-0.3.0/src/wlogging/__init__.py`

 * *Files identical despite different names*

### Comparing `wlogging-0.2.0/src/wlogging/formatters.py` & `wlogging-0.3.0/src/wlogging/formatters.py`

 * *Files identical despite different names*

### Comparing `wlogging-0.2.0/src/wlogging/loggers.py` & `wlogging-0.3.0/src/wlogging/loggers.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import logging
 from . import formatters as _formatters
 #]
 
 
 __all__ = (
     "get_colored_logger",
+    "get_short_logger",
     "get_colored_two_liner",
 )
 
 
 def get_colored_logger(
     name: str | None = None,
     level: int = logging.WARNING,
@@ -38,17 +39,23 @@
     handler.set_formatter(formatter, )
     logger.addHandler(handler, )
     logger.setLevel(level, )
     logger._decorated = True
     return logger
 
 
+get_short_logger = _ft.partial(
+    get_colored_logger,
+    format="%(name)s | %(message)s",
+)
+
+
 get_colored_two_liner = _ft.partial(
     get_colored_logger,
-    format="%(asctime)s | %(levelname)s | %(name)s:\n••• %(message)s",
+    format="%(asctime)s | %(levelname)s | %(name)s:\n::: %(message)s",
 )
 
 
 def _clear_handlers(logger: Logger, ) -> None:
     for handler in logger.handlers:
         logger.remove_handler(handler, )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `wlogging-0.2.0/pyproject.toml` & `wlogging-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
     requires = ["hatchling"]
     build-backend = "hatchling.build"
 
 [project]
     name = "wlogging"
-    version = "0.2.0"
+    version = "0.3.0"
     authors = [
       { name="Jaromir Benes", email="jaromir.benes@gmail.com" },
     ]
     description = "Pythonic wrapper for the standard logging module"
     readme = "README.md"
     requires-python = ">=3.11"
     classifiers = [
```

### Comparing `wlogging-0.2.0/PKG-INFO` & `wlogging-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: wlogging
-Version: 0.2.0
+Version: 0.3.0
 Summary: Pythonic wrapper for the standard logging module
 Project-URL: Homepage, https://github.com/iris-solutions-team/wlogging
 Project-URL: Bug Tracker, https://github.com/iris-solutions-team/wlogging/issues
 Author-email: Jaromir Benes <jaromir.benes@gmail.com>
 Keywords: logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

