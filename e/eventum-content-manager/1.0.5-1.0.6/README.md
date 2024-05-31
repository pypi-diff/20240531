# Comparing `tmp/eventum_content_manager-1.0.5.tar.gz` & `tmp/eventum_content_manager-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventum_content_manager-1.0.5.tar", max compression
+gzip compressed data, was "eventum_content_manager-1.0.6.tar", max compression
```

## Comparing `eventum_content_manager-1.0.5.tar` & `eventum_content_manager-1.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-05-19 07:21:56.176227 eventum_content_manager-1.0.5/LICENSE
--rw-r--r--   0        0        0       52 2024-05-19 09:04:51.174794 eventum_content_manager-1.0.5/README.md
--rw-r--r--   0        0        0        0 2024-05-19 07:22:51.766216 eventum_content_manager-1.0.5/eventum_content_manager/__init__.py
--rw-r--r--   0        0        0    10727 2024-05-21 17:34:44.577284 eventum_content_manager-1.0.5/eventum_content_manager/manage.py
--rw-r--r--   0        0        0        0 2024-05-23 17:09:42.570072 eventum_content_manager-1.0.5/eventum_content_manager/py.typed
--rw-r--r--   0        0        0     7105 2024-05-21 17:34:44.587284 eventum_content_manager-1.0.5/eventum_content_manager/tests/test_manage.py
--rw-r--r--   0        0        0     1264 2024-05-21 17:34:44.587284 eventum_content_manager-1.0.5/eventum_content_manager/tests/test_validators.py
--rw-r--r--   0        0        0     1787 2024-05-19 14:09:41.370509 eventum_content_manager-1.0.5/eventum_content_manager/validators.py
--rw-r--r--   0        0        0     1031 2024-05-23 17:12:42.880027 eventum_content_manager-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 eventum_content_manager-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-19 07:21:56.176227 eventum_content_manager-1.0.6/LICENSE
+-rw-r--r--   0        0        0       52 2024-05-19 09:04:51.174794 eventum_content_manager-1.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 07:22:51.766216 eventum_content_manager-1.0.6/eventum_content_manager/__init__.py
+-rw-r--r--   0        0        0    10735 2024-05-31 19:59:57.457464 eventum_content_manager-1.0.6/eventum_content_manager/manage.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:09:42.570072 eventum_content_manager-1.0.6/eventum_content_manager/py.typed
+-rw-r--r--   0        0        0     7105 2024-05-21 17:34:44.587284 eventum_content_manager-1.0.6/eventum_content_manager/tests/test_manage.py
+-rw-r--r--   0        0        0     1887 2024-05-25 16:41:20.427728 eventum_content_manager-1.0.6/eventum_content_manager/tests/test_validators.py
+-rw-r--r--   0        0        0     1787 2024-05-19 14:09:41.370509 eventum_content_manager-1.0.6/eventum_content_manager/validators.py
+-rw-r--r--   0        0        0     1031 2024-05-31 20:00:17.597459 eventum_content_manager-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 eventum_content_manager-1.0.6/PKG-INFO
```

### Comparing `eventum_content_manager-1.0.5/LICENSE` & `eventum_content_manager-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `eventum_content_manager-1.0.5/eventum_content_manager/manage.py` & `eventum_content_manager-1.0.6/eventum_content_manager/manage.py`

 * *Files 1% similar despite different names*

```diff
@@ -285,15 +285,15 @@
     """Load specified csv sample and return it as list of tuples. If
     path is relative then it is loaded from content directory.
     """
     def csv_loader(content: str) -> tuple[tuple[str, ...], ...]:
         return tuple(
             [
                 tuple(line.split(delimiter))
-                for line in content.split(os.linesep)
+                for line in content.strip().split(os.linesep)
             ]
         )
 
     return _load_object(    # type: ignore[return-value]
         path=path,
         root_dir=CSV_SAMPLES_DIR,
         loader=csv_loader
```

### Comparing `eventum_content_manager-1.0.5/eventum_content_manager/tests/test_manage.py` & `eventum_content_manager-1.0.6/eventum_content_manager/tests/test_manage.py`

 * *Files identical despite different names*

### Comparing `eventum_content_manager-1.0.5/eventum_content_manager/validators.py` & `eventum_content_manager-1.0.6/eventum_content_manager/validators.py`

 * *Files identical despite different names*

### Comparing `eventum_content_manager-1.0.5/pyproject.toml` & `eventum_content_manager-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventum-content-manager"
-version = "1.0.5"
+version = "1.0.6"
 description = "Content manager for Eventum"
 license = "Apache-2.0"
 authors = ["Nikita Reznikov <nikita.reznikov.public@mail.ru>"]
 readme = "README.md"
 repository = "https://github.com/Eventum-Generatives/EventumContentManager"
 documentation = "https://eventum-generatives.github.io/Website/"
 keywords = ["dependency"]
```

### Comparing `eventum_content_manager-1.0.5/PKG-INFO` & `eventum_content_manager-1.0.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventum-content-manager
-Version: 1.0.5
+Version: 1.0.6
 Summary: Content manager for Eventum
 Home-page: https://github.com/Eventum-Generatives/EventumContentManager
 License: Apache-2.0
 Keywords: dependency
 Author: Nikita Reznikov
 Author-email: nikita.reznikov.public@mail.ru
 Requires-Python: >=3.11,<4.0
```

