# Comparing `tmp/edgegap_cli-1.7.0.tar.gz` & `tmp/edgegap_cli-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgegap_cli-1.7.0.tar", max compression
+gzip compressed data, was "edgegap_cli-1.8.0.tar", max compression
```

## Comparing `edgegap_cli-1.7.0.tar` & `edgegap_cli-1.8.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1993 2024-05-06 18:04:44.759069 edgegap_cli-1.7.0/LICENSE
--rw-r--r--   0        0        0     2119 2024-05-06 18:04:44.759350 edgegap_cli-1.7.0/README.md
--rw-r--r--   0        0        0      230 2024-05-06 19:55:51.786678 edgegap_cli-1.7.0/edgegap_cli/__init__.py
--rw-r--r--   0        0        0       76 2024-05-06 18:04:44.760089 edgegap_cli-1.7.0/edgegap_cli/core/__init__.py
--rw-r--r--   0        0        0      127 2024-05-06 20:09:19.276344 edgegap_cli-1.7.0/edgegap_cli/core/builders/__init__.py
--rw-r--r--   0        0        0      333 2024-05-06 18:04:44.760508 edgegap_cli-1.7.0/edgegap_cli/core/builders/_interface.py
--rw-r--r--   0        0        0     1724 2024-05-06 20:32:49.019519 edgegap_cli-1.7.0/edgegap_cli/core/builders/_menu.py
--rw-r--r--   0        0        0     1601 2024-05-07 13:32:15.029089 edgegap_cli-1.7.0/edgegap_cli/core/builders/_terminal.py
--rw-r--r--   0        0        0      176 2024-05-06 18:04:44.761343 edgegap_cli-1.7.0/edgegap_cli/core/handlers/__init__.py
--rw-r--r--   0        0        0     1955 2024-05-06 20:32:48.931892 edgegap_cli-1.7.0/edgegap_cli/core/handlers/_cli.py
--rw-r--r--   0        0        0      128 2024-05-06 18:04:44.761804 edgegap_cli-1.7.0/edgegap_cli/core/handlers/_depends.py
--rw-r--r--   0        0        0     1527 2024-05-06 20:32:48.949450 edgegap_cli-1.7.0/edgegap_cli/core/handlers/_namespace.py
--rw-r--r--   0        0        0     4501 2024-05-06 20:32:48.967384 edgegap_cli-1.7.0/edgegap_cli/core/handlers/_view.py
--rw-r--r--   0        0        0      165 2024-05-06 18:04:44.762490 edgegap_cli-1.7.0/edgegap_cli/core/models/__init__.py
--rw-r--r--   0        0        0      197 2024-05-06 18:04:44.762636 edgegap_cli-1.7.0/edgegap_cli/core/models/_cli.py
--rw-r--r--   0        0        0      172 2024-05-06 18:04:44.762940 edgegap_cli-1.7.0/edgegap_cli/core/models/_constraint.py
--rw-r--r--   0        0        0      285 2024-05-06 18:04:44.763165 edgegap_cli-1.7.0/edgegap_cli/core/models/_namespace.py
--rw-r--r--   0        0        0      553 2024-05-06 18:04:44.763482 edgegap_cli-1.7.0/edgegap_cli/core/models/_view.py
--rw-r--r--   0        0        0       42 2024-05-06 18:04:44.763663 edgegap_cli-1.7.0/edgegap_cli/features/__init__.py
--rw-r--r--   0        0        0      255 2024-05-06 20:40:30.104404 edgegap_cli-1.7.0/edgegap_cli/features/db/__init__.py
--rw-r--r--   0        0        0      713 2024-05-06 18:04:46.733709 edgegap_cli-1.7.0/edgegap_cli/features/db/_config.py
--rw-r--r--   0        0        0      131 2024-05-06 18:04:44.764338 edgegap_cli-1.7.0/edgegap_cli/features/db/_namespace.py
--rw-r--r--   0        0        0      324 2024-05-06 18:04:44.764513 edgegap_cli-1.7.0/edgegap_cli/features/db/actions/__init__.py
--rw-r--r--   0        0        0      480 2024-05-06 20:32:49.043793 edgegap_cli-1.7.0/edgegap_cli/features/db/actions/_current.py
--rw-r--r--   0        0        0      655 2024-05-06 20:32:49.229668 edgegap_cli-1.7.0/edgegap_cli/features/db/actions/_downgrade.py
--rw-r--r--   0        0        0      509 2024-05-06 20:32:49.085303 edgegap_cli-1.7.0/edgegap_cli/features/db/actions/_history.py
--rw-r--r--   0        0        0     1607 2024-05-07 13:32:27.929141 edgegap_cli-1.7.0/edgegap_cli/features/db/actions/_initialize.py
--rw-r--r--   0        0        0      705 2024-05-06 20:32:49.070126 edgegap_cli-1.7.0/edgegap_cli/features/db/actions/_migrate.py
--rw-r--r--   0        0        0      650 2024-05-06 20:32:49.245074 edgegap_cli-1.7.0/edgegap_cli/features/db/actions/_upgrade.py
--rw-r--r--   0        0        0      368 2024-05-06 18:04:44.765641 edgegap_cli-1.7.0/edgegap_cli/main.py
--rw-r--r--   0        0        0      769 2024-05-07 13:32:46.546033 edgegap_cli-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     2969 1970-01-01 00:00:00.000000 edgegap_cli-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1993 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/LICENSE
+-rw-r--r--   0        0        0     2119 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/README.md
+-rw-r--r--   0        0        0      230 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/__init__.py
+-rw-r--r--   0        0        0       76 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/core/__init__.py
+-rw-r--r--   0        0        0      127 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/core/builders/__init__.py
+-rw-r--r--   0        0        0      333 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/core/builders/_interface.py
+-rw-r--r--   0        0        0     1724 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/core/builders/_menu.py
+-rw-r--r--   0        0        0     1601 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/core/builders/_terminal.py
+-rw-r--r--   0        0        0      176 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/core/handlers/__init__.py
+-rw-r--r--   0        0        0     1955 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/core/handlers/_cli.py
+-rw-r--r--   0        0        0      128 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/core/handlers/_depends.py
+-rw-r--r--   0        0        0     1527 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/core/handlers/_namespace.py
+-rw-r--r--   0        0        0     4501 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/core/handlers/_view.py
+-rw-r--r--   0        0        0      165 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/core/models/__init__.py
+-rw-r--r--   0        0        0      197 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/core/models/_cli.py
+-rw-r--r--   0        0        0      172 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/core/models/_constraint.py
+-rw-r--r--   0        0        0      285 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/core/models/_namespace.py
+-rw-r--r--   0        0        0      553 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/core/models/_view.py
+-rw-r--r--   0        0        0       42 2024-05-31 11:59:59.007154 edgegap_cli-1.8.0/edgegap_cli/features/__init__.py
+-rw-r--r--   0        0        0      255 2024-05-31 11:59:59.011154 edgegap_cli-1.8.0/edgegap_cli/features/db/__init__.py
+-rw-r--r--   0        0        0      713 2024-05-31 11:59:59.011154 edgegap_cli-1.8.0/edgegap_cli/features/db/_config.py
+-rw-r--r--   0        0        0      131 2024-05-31 11:59:59.011154 edgegap_cli-1.8.0/edgegap_cli/features/db/_namespace.py
+-rw-r--r--   0        0        0      324 2024-05-31 11:59:59.011154 edgegap_cli-1.8.0/edgegap_cli/features/db/actions/__init__.py
+-rw-r--r--   0        0        0      480 2024-05-31 11:59:59.011154 edgegap_cli-1.8.0/edgegap_cli/features/db/actions/_current.py
+-rw-r--r--   0        0        0      655 2024-05-31 11:59:59.011154 edgegap_cli-1.8.0/edgegap_cli/features/db/actions/_downgrade.py
+-rw-r--r--   0        0        0      509 2024-05-31 11:59:59.011154 edgegap_cli-1.8.0/edgegap_cli/features/db/actions/_history.py
+-rw-r--r--   0        0        0     1607 2024-05-31 11:59:59.011154 edgegap_cli-1.8.0/edgegap_cli/features/db/actions/_initialize.py
+-rw-r--r--   0        0        0      705 2024-05-31 11:59:59.011154 edgegap_cli-1.8.0/edgegap_cli/features/db/actions/_migrate.py
+-rw-r--r--   0        0        0      650 2024-05-31 11:59:59.011154 edgegap_cli-1.8.0/edgegap_cli/features/db/actions/_upgrade.py
+-rw-r--r--   0        0        0      368 2024-05-31 11:59:59.011154 edgegap_cli-1.8.0/edgegap_cli/main.py
+-rw-r--r--   0        0        0      769 2024-05-31 12:01:45.798176 edgegap_cli-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2969 1970-01-01 00:00:00.000000 edgegap_cli-1.8.0/PKG-INFO
```

### Comparing `edgegap_cli-1.7.0/LICENSE` & `edgegap_cli-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgegap_cli-1.7.0/README.md` & `edgegap_cli-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `edgegap_cli-1.7.0/edgegap_cli/core/builders/_menu.py` & `edgegap_cli-1.8.0/edgegap_cli/core/builders/_menu.py`

 * *Files identical despite different names*

### Comparing `edgegap_cli-1.7.0/edgegap_cli/core/builders/_terminal.py` & `edgegap_cli-1.8.0/edgegap_cli/core/builders/_terminal.py`

 * *Files identical despite different names*

### Comparing `edgegap_cli-1.7.0/edgegap_cli/core/handlers/_cli.py` & `edgegap_cli-1.8.0/edgegap_cli/core/handlers/_cli.py`

 * *Files identical despite different names*

### Comparing `edgegap_cli-1.7.0/edgegap_cli/core/handlers/_namespace.py` & `edgegap_cli-1.8.0/edgegap_cli/core/handlers/_namespace.py`

 * *Files identical despite different names*

### Comparing `edgegap_cli-1.7.0/edgegap_cli/core/handlers/_view.py` & `edgegap_cli-1.8.0/edgegap_cli/core/handlers/_view.py`

 * *Files identical despite different names*

### Comparing `edgegap_cli-1.7.0/edgegap_cli/core/models/_view.py` & `edgegap_cli-1.8.0/edgegap_cli/core/models/_view.py`

 * *Files identical despite different names*

### Comparing `edgegap_cli-1.7.0/edgegap_cli/features/db/_config.py` & `edgegap_cli-1.8.0/edgegap_cli/features/db/_config.py`

 * *Files identical despite different names*

### Comparing `edgegap_cli-1.7.0/edgegap_cli/features/db/actions/_downgrade.py` & `edgegap_cli-1.8.0/edgegap_cli/features/db/actions/_downgrade.py`

 * *Files identical despite different names*

### Comparing `edgegap_cli-1.7.0/edgegap_cli/features/db/actions/_initialize.py` & `edgegap_cli-1.8.0/edgegap_cli/features/db/actions/_initialize.py`

 * *Files identical despite different names*

### Comparing `edgegap_cli-1.7.0/edgegap_cli/features/db/actions/_migrate.py` & `edgegap_cli-1.8.0/edgegap_cli/features/db/actions/_migrate.py`

 * *Files identical despite different names*

### Comparing `edgegap_cli-1.7.0/edgegap_cli/features/db/actions/_upgrade.py` & `edgegap_cli-1.8.0/edgegap_cli/features/db/actions/_upgrade.py`

 * *Files identical despite different names*

### Comparing `edgegap_cli-1.7.0/pyproject.toml` & `edgegap_cli-1.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edgegap-cli"
-version = "1.7.0"
+version = "1.8.0"
 description = "The Edgegap CLI for operations like migrations. It is designed for use within the Edgegap organization."
 authors = ["Bastien Roy <bastien@edgegap.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 console-menu = "^0.8.0"
```

### Comparing `edgegap_cli-1.7.0/PKG-INFO` & `edgegap_cli-1.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgegap-cli
-Version: 1.7.0
+Version: 1.8.0
 Summary: The Edgegap CLI for operations like migrations. It is designed for use within the Edgegap organization.
 Author: Bastien Roy
 Author-email: bastien@edgegap.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

