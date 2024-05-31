# Comparing `tmp/eventum_core-1.0.3.tar.gz` & `tmp/eventum_core-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventum_core-1.0.3.tar", max compression
+gzip compressed data, was "eventum_core-1.0.4.tar", max compression
```

## Comparing `eventum_core-1.0.3.tar` & `eventum_core-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11345 2024-05-18 21:13:58.350025 eventum_core-1.0.3/LICENSE
--rw-r--r--   0        0        0     4969 2024-05-18 21:13:58.350025 eventum_core-1.0.3/README.md
--rw-r--r--   0        0        0        0 2024-05-18 21:13:58.350025 eventum_core-1.0.3/eventum_core/__init__.py
--rw-r--r--   0        0        0     6359 2024-05-29 11:14:23.783537 eventum_core-1.0.3/eventum_core/app.py
--rw-r--r--   0        0        0     2697 2024-05-18 21:13:58.350025 eventum_core-1.0.3/eventum_core/batcher.py
--rw-r--r--   0        0        0     3717 2024-05-27 18:43:56.363810 eventum_core-1.0.3/eventum_core/plugins_connector.py
--rw-r--r--   0        0        0        0 2024-05-26 15:45:08.775672 eventum_core-1.0.3/eventum_core/py.typed
--rw-r--r--   0        0        0     1311 2024-05-27 17:12:30.335092 eventum_core-1.0.3/eventum_core/settings.py
--rw-r--r--   0        0        0     8660 2024-05-27 18:52:49.493682 eventum_core-1.0.3/eventum_core/subprocesses.py
--rw-r--r--   0        0        0      940 2024-05-26 15:46:55.835646 eventum_core-1.0.3/eventum_core/tests/test_batcher.py
--rw-r--r--   0        0        0     3425 2024-05-29 11:16:07.933532 eventum_core-1.0.3/eventum_core/tests/test_subprocesses.py
--rw-r--r--   0        0        0     1252 2024-05-29 11:17:01.363477 eventum_core-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     6227 1970-01-01 00:00:00.000000 eventum_core-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-05-18 21:13:58.350025 eventum_core-1.0.4/LICENSE
+-rw-r--r--   0        0        0     4969 2024-05-18 21:13:58.350025 eventum_core-1.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-18 21:13:58.350025 eventum_core-1.0.4/eventum_core/__init__.py
+-rw-r--r--   0        0        0     6359 2024-05-29 11:14:23.783537 eventum_core-1.0.4/eventum_core/app.py
+-rw-r--r--   0        0        0     2697 2024-05-18 21:13:58.350025 eventum_core-1.0.4/eventum_core/batcher.py
+-rw-r--r--   0        0        0     3717 2024-05-27 18:43:56.363810 eventum_core-1.0.4/eventum_core/plugins_connector.py
+-rw-r--r--   0        0        0        0 2024-05-26 15:45:08.775672 eventum_core-1.0.4/eventum_core/py.typed
+-rw-r--r--   0        0        0     1311 2024-05-27 17:12:30.335092 eventum_core-1.0.4/eventum_core/settings.py
+-rw-r--r--   0        0        0     8660 2024-05-30 16:46:29.634429 eventum_core-1.0.4/eventum_core/subprocesses.py
+-rw-r--r--   0        0        0      940 2024-05-26 15:46:55.835646 eventum_core-1.0.4/eventum_core/tests/test_batcher.py
+-rw-r--r--   0        0        0     3425 2024-05-29 11:16:07.933532 eventum_core-1.0.4/eventum_core/tests/test_subprocesses.py
+-rw-r--r--   0        0        0     1252 2024-05-31 19:30:53.637883 eventum_core-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6227 1970-01-01 00:00:00.000000 eventum_core-1.0.4/PKG-INFO
```

### Comparing `eventum_core-1.0.3/LICENSE` & `eventum_core-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.3/README.md` & `eventum_core-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.3/eventum_core/app.py` & `eventum_core-1.0.4/eventum_core/app.py`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.3/eventum_core/batcher.py` & `eventum_core-1.0.4/eventum_core/batcher.py`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.3/eventum_core/plugins_connector.py` & `eventum_core-1.0.4/eventum_core/plugins_connector.py`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.3/eventum_core/settings.py` & `eventum_core-1.0.4/eventum_core/settings.py`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.3/eventum_core/subprocesses.py` & `eventum_core-1.0.4/eventum_core/subprocesses.py`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.3/eventum_core/tests/test_batcher.py` & `eventum_core-1.0.4/eventum_core/tests/test_batcher.py`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.3/eventum_core/tests/test_subprocesses.py` & `eventum_core-1.0.4/eventum_core/tests/test_subprocesses.py`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.3/pyproject.toml` & `eventum_core-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventum-core"
-version = "1.0.3"
+version = "1.0.4"
 description = "Flexible event generator"
 license = "Apache-2.0"
 authors = ["Nikita Reznikov <nikita.reznikov.public@mail.ru>"]
 readme = "README.md"
 repository = "https://github.com/Eventum-Generatives/EventumCore"
 documentation = "https://eventum-generatives.github.io/Website/"
 keywords = ["generator", "testing", "data", "event"]
```

### Comparing `eventum_core-1.0.3/PKG-INFO` & `eventum_core-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventum-core
-Version: 1.0.3
+Version: 1.0.4
 Summary: Flexible event generator
 Home-page: https://github.com/Eventum-Generatives/EventumCore
 License: Apache-2.0
 Keywords: generator,testing,data,event
 Author: Nikita Reznikov
 Author-email: nikita.reznikov.public@mail.ru
 Requires-Python: >=3.11,<4.0
```

