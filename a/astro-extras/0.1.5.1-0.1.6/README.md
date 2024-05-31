# Comparing `tmp/astro_extras-0.1.5.1.tar.gz` & `tmp/astro_extras-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_extras-0.1.5.1.tar", last modified: Mon May 27 10:57:08 2024, max compression
+gzip compressed data, was "astro_extras-0.1.6.tar", last modified: Thu May 30 13:06:32 2024, max compression
```

## Comparing `astro_extras-0.1.5.1.tar` & `astro_extras-0.1.6.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.480975 astro_extras-0.1.5.1/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.1.5.1/LICENSE
--rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.1.5.1/MANIFEST.in
--rw-r--r--   0 kol       (1000) kol       (1000)     7922 2024-05-27 10:57:08.480975 astro_extras-0.1.5.1/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.1.5.1/README.md
--rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.1.5.1/pyproject.toml
--rw-rw-r--   0 kol       (1000) kol       (1000)      288 2024-05-26 09:28:01.000000 astro_extras-0.1.5.1/requirements.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-05-27 10:57:08.480975 astro_extras-0.1.5.1/setup.cfg
--rw-rw-r--   0 kol       (1000) kol       (1000)     1195 2024-05-27 10:52:04.000000 astro_extras-0.1.5.1/setup.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.444975 astro_extras-0.1.5.1/src/
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.448975 astro_extras-0.1.5.1/src/astro_extras/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1208 2024-05-27 10:52:15.000000 astro_extras-0.1.5.1/src/astro_extras/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.464974 astro_extras-0.1.5.1/src/astro_extras/hooks/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.5.1/src/astro_extras/hooks/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.464974 astro_extras-0.1.5.1/src/astro_extras/operators/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.5.1/src/astro_extras/operators/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     3861 2024-04-06 11:05:12.000000 astro_extras-0.1.5.1/src/astro_extras/operators/direct.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    18221 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/operators/session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    54666 2024-05-27 10:52:47.000000 astro_extras-0.1.5.1/src/astro_extras/operators/table.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.464974 astro_extras-0.1.5.1/src/astro_extras/sensors/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.1.5.1/src/astro_extras/sensors/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)      659 2024-04-23 14:51:38.000000 astro_extras-0.1.5.1/src/astro_extras/sensors/auto.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5536 2024-04-06 11:03:48.000000 astro_extras-0.1.5.1/src/astro_extras/sensors/file.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.476975 astro_extras-0.1.5.1/src/astro_extras/templates/
--rw-rw-r--   0 kol       (1000) kol       (1000)      121 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/templates/session_close.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      269 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/templates/session_open.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      545 2024-05-22 09:04:48.000000 astro_extras-0.1.5.1/src/astro_extras/templates/table_actuals_select.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      138 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/templates/table_timed_update.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)       81 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/templates/table_transfer_nosess.sql
--rw-rw-r--   0 kol       (1000) kol       (1000)      187 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/templates/table_transfer_sess.sql
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.476975 astro_extras-0.1.5.1/src/astro_extras/utils/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.5.1/src/astro_extras/utils/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    10671 2024-05-02 14:17:47.000000 astro_extras-0.1.5.1/src/astro_extras/utils/data_compare.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.1.5.1/src/astro_extras/utils/datetime_local.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     3707 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/utils/postgres_sql.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5818 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/src/astro_extras/utils/template.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     4032 2024-05-22 07:52:50.000000 astro_extras-0.1.5.1/src/astro_extras/utils/utils.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.480975 astro_extras-0.1.5.1/src/astro_extras.egg-info/
--rw-r--r--   0 kol       (1000) kol       (1000)     7922 2024-05-27 10:57:08.000000 astro_extras-0.1.5.1/src/astro_extras.egg-info/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)     1188 2024-05-27 10:57:08.000000 astro_extras-0.1.5.1/src/astro_extras.egg-info/SOURCES.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-05-27 10:57:08.000000 astro_extras-0.1.5.1/src/astro_extras.egg-info/dependency_links.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)      139 2024-05-27 10:57:08.000000 astro_extras-0.1.5.1/src/astro_extras.egg-info/requires.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-05-27 10:57:08.000000 astro_extras-0.1.5.1/src/astro_extras.egg-info/top_level.txt
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-27 10:57:08.476975 astro_extras-0.1.5.1/tests/
--rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.1.5.1/tests/test_session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    28649 2024-05-22 07:52:04.000000 astro_extras-0.1.5.1/tests/test_table.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.1.5.1/tests/test_templates.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-05-02 14:33:06.000000 astro_extras-0.1.5.1/tests/test_utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-30 13:06:32.599997 astro_extras-0.1.6/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.1.6/LICENSE
+-rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.1.6/MANIFEST.in
+-rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-30 13:06:32.599997 astro_extras-0.1.6/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.1.6/README.md
+-rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.1.6/pyproject.toml
+-rw-rw-r--   0 kol       (1000) kol       (1000)      288 2024-05-26 09:28:01.000000 astro_extras-0.1.6/requirements.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-05-30 13:06:32.599997 astro_extras-0.1.6/setup.cfg
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1193 2024-05-30 07:09:18.000000 astro_extras-0.1.6/setup.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-30 13:06:32.535997 astro_extras-0.1.6/src/
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-30 13:06:32.539997 astro_extras-0.1.6/src/astro_extras/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1206 2024-05-30 07:09:25.000000 astro_extras-0.1.6/src/astro_extras/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-30 13:06:32.547997 astro_extras-0.1.6/src/astro_extras/hooks/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.6/src/astro_extras/hooks/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-30 13:06:32.559997 astro_extras-0.1.6/src/astro_extras/operators/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.6/src/astro_extras/operators/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3861 2024-04-06 11:05:12.000000 astro_extras-0.1.6/src/astro_extras/operators/direct.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    18221 2024-05-22 07:52:04.000000 astro_extras-0.1.6/src/astro_extras/operators/session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    55610 2024-05-30 07:08:04.000000 astro_extras-0.1.6/src/astro_extras/operators/table.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-30 13:06:32.563997 astro_extras-0.1.6/src/astro_extras/sensors/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.1.6/src/astro_extras/sensors/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)      659 2024-04-23 14:51:38.000000 astro_extras-0.1.6/src/astro_extras/sensors/auto.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5536 2024-04-06 11:03:48.000000 astro_extras-0.1.6/src/astro_extras/sensors/file.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-30 13:06:32.579997 astro_extras-0.1.6/src/astro_extras/templates/
+-rw-rw-r--   0 kol       (1000) kol       (1000)      121 2024-05-22 07:52:04.000000 astro_extras-0.1.6/src/astro_extras/templates/session_close.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      269 2024-05-22 07:52:04.000000 astro_extras-0.1.6/src/astro_extras/templates/session_open.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      495 2024-05-29 09:16:50.000000 astro_extras-0.1.6/src/astro_extras/templates/table_actuals_select.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      228 2024-05-29 10:38:10.000000 astro_extras-0.1.6/src/astro_extras/templates/table_actuals_select_all.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      485 2024-05-29 10:38:23.000000 astro_extras-0.1.6/src/astro_extras/templates/table_actuals_select_delta.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      138 2024-05-22 07:52:04.000000 astro_extras-0.1.6/src/astro_extras/templates/table_timed_update.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)       81 2024-05-22 07:52:04.000000 astro_extras-0.1.6/src/astro_extras/templates/table_transfer_nosess.sql
+-rw-rw-r--   0 kol       (1000) kol       (1000)      187 2024-05-22 07:52:04.000000 astro_extras-0.1.6/src/astro_extras/templates/table_transfer_sess.sql
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-30 13:06:32.587997 astro_extras-0.1.6/src/astro_extras/utils/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.1.6/src/astro_extras/utils/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    10699 2024-05-29 09:19:47.000000 astro_extras-0.1.6/src/astro_extras/utils/data_compare.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.1.6/src/astro_extras/utils/datetime_local.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3707 2024-05-22 07:52:04.000000 astro_extras-0.1.6/src/astro_extras/utils/postgres_sql.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5818 2024-05-22 07:52:04.000000 astro_extras-0.1.6/src/astro_extras/utils/template.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4032 2024-05-22 07:52:50.000000 astro_extras-0.1.6/src/astro_extras/utils/utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-30 13:06:32.599997 astro_extras-0.1.6/src/astro_extras.egg-info/
+-rw-r--r--   0 kol       (1000) kol       (1000)     7920 2024-05-30 13:06:32.000000 astro_extras-0.1.6/src/astro_extras.egg-info/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1302 2024-05-30 13:06:32.000000 astro_extras-0.1.6/src/astro_extras.egg-info/SOURCES.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-05-30 13:06:32.000000 astro_extras-0.1.6/src/astro_extras.egg-info/dependency_links.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)      139 2024-05-30 13:06:32.000000 astro_extras-0.1.6/src/astro_extras.egg-info/requires.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-05-30 13:06:32.000000 astro_extras-0.1.6/src/astro_extras.egg-info/top_level.txt
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-05-30 13:06:32.599997 astro_extras-0.1.6/tests/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.1.6/tests/test_session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    28649 2024-05-22 07:52:04.000000 astro_extras-0.1.6/tests/test_table.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.1.6/tests/test_templates.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-05-02 14:33:06.000000 astro_extras-0.1.6/tests/test_utils.py
```

### Comparing `astro_extras-0.1.5.1/LICENSE` & `astro_extras-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5.1/PKG-INFO` & `astro_extras-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.1.5.1
+Version: 0.1.6
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.1.5.1/README.md` & `astro_extras-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5.1/setup.py` & `astro_extras-0.1.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.readlines()
 
 setuptools.setup(
     name="astro_extras",
-    version="0.1.5.1",
+    version="0.1.6",
     author="Kol",
     author_email="skolchin@gmail.com",
     description="Additional Astro SDK operators",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/skolchin/astro-extras",
     classifiers=[
```

### Comparing `astro_extras-0.1.5.1/src/astro_extras/__init__.py` & `astro_extras-0.1.6/src/astro_extras/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Astro SDK Extras project
 # (c) kol, 2023-2024
 
-__version__ = '0.1.5.1'
+__version__ = '0.1.6'
 
 from .operators.session import (
     open_session, 
     close_session,
     ETLSession,
     get_current_session,
     get_session_period,
```

### Comparing `astro_extras-0.1.5.1/src/astro_extras/operators/direct.py` & `astro_extras-0.1.6/src/astro_extras/operators/direct.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5.1/src/astro_extras/operators/session.py` & `astro_extras-0.1.6/src/astro_extras/operators/session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5.1/src/astro_extras/operators/table.py` & `astro_extras-0.1.6/src/astro_extras/operators/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,21 +51,21 @@
     source_db: BaseDatabase
     """ Source database object """
 
     dest_db: BaseDatabase
     """ Destination database object """
 
     source: BaseTable
-    """ Source table object. See also `source_table_def` property """
+    """ Source table object as it was passed in. Property `source_table_def` reflects the same table but filled with columns structure """
 
     source_table: str
     """ Source table fully-qualified name """
 
     destination: BaseTable
-    """ Destination table object. See also `dest_table_def` property """
+    """ Destination table object as it was passed in. Property `dest_table_def` reflects the same table but filled with columns structure """
 
     destination_table: str
     """ Destination table fully-qualified name """
 
     session: ETLSession | XComArg | None
     """ ETL Session. Use `ensure_session` to cast to proper session type """
 
@@ -124,14 +124,15 @@
 
     def _get_sql(self, table: BaseTable, db: BaseDatabase, session: ETLSession | None = None, suffix: str | None = None) -> str:
         """ Internal - get a sql statement or template for given table """
 
         # Check whether a template SQL exists for given table under dags\templates\<dag_id>
         # Actual query will be loaded by Airflow templating itself
         full_name = db.get_table_qualified_name(table)
+        self.log.info(f'Looking up a template file for table {full_name}')
         if (sql_file := get_template_file(full_name, '.sql')) or (sql_file := get_template_file(table.name, '.sql')) :
             self.log.info(f'Using template file {sql_file}')
             return sql_file
 
         # Nope, load an SQL from package resources substituting template fields manually
         # SQL file names are fixed according to whether we do run under ETL session or not
         template_name = 'table_transfer_nosess.sql' if not session else 'table_transfer_sess.sql'
@@ -292,21 +293,21 @@
                     ),
                     "dataSource": DataSourceDatasetFacet(
                         name=full_name, uri=f"{ns}/{full_name}"
                     ),
                 })
 
         # Construct input dataset...
-        if self.source and self.source.openlineage_emit_temp_table_event():
+        if self.source_table_def.openlineage_emit_temp_table_event():
             source_datasets = [_make_dataset(self.source_table_def, self.source_db)]
         else:
             source_datasets = []
 
         # ... output dataset ...
-        if self.destination and self.destination.openlineage_emit_temp_table_event():
+        if self.dest_table_def.openlineage_emit_temp_table_event():
             dest_datasets = [_make_dataset(self.dest_table_def, self.dest_db)]
         else:
             dest_datasets = []
 
         # ... runtime facets ...
         run_facets: dict[str, BaseFacet] = {
             "outputStatistics": OutputStatisticsOutputDatasetFacet(
@@ -360,16 +361,19 @@
     def _compare_datasets(self, src_conn: SqlaConnection, dest_conn: SqlaConnection, stop_on_first_diff: bool, logger: logging.Logger | None = None):
         """ Internal - compare source and target dictionaries """
 
         logger = logger or self.log
 
         logger.info(f'Executing: {self.sql}')
         df_src = pd.read_sql(self.sql, src_conn)
+        logger.info(f'{len(df_src)} records selected on source')
+
         logger.info(f'Executing: {self.destination_sql}')
         df_trg  = pd.read_sql(self.destination_sql, dest_conn)
+        logger.info(f'{len(df_trg)} records selected on target')
 
         return compare_datasets(df_src, df_trg, stop_on_first_diff=stop_on_first_diff, logger=logger)
 
     def execute(self, context: Context):
         """ Execute operator """
         self._pre_execute(context)
         if not self._compare_datasets(self.source_db.connection, self.dest_db.connection, stop_on_first_diff=True):
@@ -444,32 +448,41 @@
 
     def __init__(
         self,
         *,
         source_table: BaseTable,
         destination_table: BaseTable,
         session: ETLSession | None = None,
+        transfer_delta: bool = True,
         as_ods: bool = False,
         keep_temp_table: bool = False,
         replace_data: bool = False,
         **kwargs,
     ) -> None:
-        super().__init__(source_table=source_table, destination_table=destination_table, session=session, **kwargs)
+        self.transfer_delta = transfer_delta
         self.as_ods = as_ods
         self.keep_temp_table = keep_temp_table
         self.replace_data = replace_data
+        
+        super().__init__(source_table=source_table, destination_table=destination_table, session=session, **kwargs)
 
     def _get_sql(self, table: BaseTable, db: BaseDatabase, session: ETLSession | None = None, suffix: str | None = None) -> str:
         """ Internal - get a sql statement or template for given table """
 
-        # Get template SQL from package resources
-        # The template defines `select` query which takes data from source limited 
-        # to one's loaded with successfull sessions with the same loading period as this operator has
+        # Find table-specific template
         full_name = db.get_table_qualified_name(table)
-        template = get_predefined_template('table_actuals_select.sql')
+        if (sql := get_template(full_name, '.sql', fail_if_not_found=False)):
+            # If such template exist, replace table name with subquery
+            # The subquery should contain the same subset of columns with target table, 
+            # otherwise it might be problems with dataset comparsion
+            full_name = f'({sql})'
+
+        # Get template SQL from package resources
+        # The template defines `select` query which takes data from source
+        template = get_predefined_template('table_actuals_select_delta.sql' if self.transfer_delta else 'table_actuals_select_all.sql')
         return template.render(source_table=full_name)
 
     def execute(self, context: Context):
         """ Execute operator """
 
         # All the checks
         self._pre_execute(context)
@@ -543,15 +556,15 @@
                 
                 data = self._adjust_dtypes(data, self.dest_table_def)
                 if self.session:
                     data['session_id'] = self.session.session_id
                     col_map['session_id'] = 'session_id'
 
                 # Temp table has to be created 1st, otherwise it might be column types mismatch
-                temp_sqla_table = SqlaTable(temp_table.name, temp_table.sqlalchemy_metadata, *([c.copy() for c in self.source.columns]))
+                temp_sqla_table = SqlaTable(temp_table.name, temp_table.sqlalchemy_metadata, *([c.copy() for c in self.source_table_def.columns]))
                 self.destination.sqlalchemy_metadata.create_all(bind=dest_conn, tables=[temp_sqla_table], checkfirst=False)
 
                 try:
                     # Save data to temporary table
                     data.to_sql(
                         temp_table.name,
                         con=dest_conn,
@@ -1074,26 +1087,29 @@
 
 def transfer_actuals_table(
         source: str | BaseTable,
         target: str | BaseTable | None = None,
         source_conn_id: str | None = None,
         destination_conn_id: str | None = None,
         session: XComArg | ETLSession = None,
+        transfer_delta: bool = True,
         as_ods: bool = False,
         keep_temp_table: bool = False,
         replace_data: bool = False,
         **kwargs) -> XComArg:
     
     """ Transfer table from stage to actuals.
 
     Returns:
         `XComArg` object
 
     """
     assert session is not None, 'Transfer to actuals requires ETL session'
+
+    kwargs['transfer_delta'] = transfer_delta
     kwargs['as_ods'] = as_ods
     kwargs['keep_temp_table'] = keep_temp_table
     kwargs['replace_data'] = replace_data
 
     return _do_transfer_table(
         op_cls=ActualsTableTransfer,
         source=source,
@@ -1107,22 +1123,25 @@
         source_tables: Iterable[str | Table],
         target_tables: Iterable[str | Table] | None = None,
         source_conn_id: str | None = None,
         destination_conn_id: str | None = None,
         group_id: str | None = None,
         num_parallel: int = 1,
         session: XComArg | ETLSession | None = None,
+        transfer_delta: bool = True,
         as_ods: bool = False,
         keep_temp_table: bool = False,
         replace_data: bool = False,
         **kwargs) -> TaskGroup:
 
     """ Transfer multiple tables from stage to actuals.
     """
     assert session is not None, 'Transfer to actuals requires ETL session'
+
+    kwargs['transfer_delta'] = transfer_delta
     kwargs['as_ods'] = as_ods
     kwargs['keep_temp_table'] = keep_temp_table
     kwargs['replace_data'] = replace_data
 
     return _do_transfer_tables(
         op_cls=ActualsTableTransfer,
         source_tables=source_tables,
```

### Comparing `astro_extras-0.1.5.1/src/astro_extras/sensors/auto.py` & `astro_extras-0.1.6/src/astro_extras/sensors/auto.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5.1/src/astro_extras/sensors/file.py` & `astro_extras-0.1.6/src/astro_extras/sensors/file.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5.1/src/astro_extras/utils/data_compare.py` & `astro_extras-0.1.6/src/astro_extras/utils/data_compare.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,34 +115,34 @@
         diff_cols = set(id_cols).difference(trg_cols)
         if diff_cols:
             raise AirflowFailException(f'ID columns missing from target dataset: {diff_cols}')
     logger.debug(f'ID columns: {id_cols}')
 
     diff_cols = set(src_cols).symmetric_difference(trg_cols).difference(exclude_cols)
     if diff_cols:
-        logger.warning(f'Diff in columns detected: {diff_cols}.\n' + 
+        logger.warning(f'Сolumn difference detected: {diff_cols}.\n' + 
                        'Operation will continue, but may result in incomplete data transfer or errors.\n' +
                        'Review the datasets and correct structure to avoid that.')
 
     if df_src.shape[0] != df_trg.shape[0] and stop_on_first_diff:
-        logger.info('Number of records in source and target datasets is different')
+        logger.info('Source and target datasets has different number of records, comparsion stopped')
         return False
 
     _check_timestamp_types(df_src, df_trg, exclude_cols)
 
     shared_cols = set(src_cols).intersection(trg_cols).difference(exclude_cols)
     logger.debug(f'Shared cols: {shared_cols}')
 
     df_src.index.name = '__src_idx__'
     df_trg.index.name = '__trg_idx__'
     df_deleted = None
     df_merged = pd.merge(df_src.reset_index(), df_trg.reset_index(), how='outer', on=id_cols,
                             copy=False, indicator=True, sort=False)
     if df_merged['_merge'].eq('right_only').any():
-        logger.info('Target dataset contains records not present on the source')
+        logger.info('Target dataset contains records which do not exist on the source')
         if stop_on_first_diff:
             return False
 
         idx_list = df_merged[df_merged['_merge'] == 'right_only']['__trg_idx__']
         df_deleted = df_trg.iloc[idx_list]
         df_deleted.index.name = None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `astro_extras-0.1.5.1/src/astro_extras/utils/datetime_local.py` & `astro_extras-0.1.6/src/astro_extras/utils/datetime_local.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5.1/src/astro_extras/utils/postgres_sql.py` & `astro_extras-0.1.6/src/astro_extras/utils/postgres_sql.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5.1/src/astro_extras/utils/template.py` & `astro_extras-0.1.6/src/astro_extras/utils/template.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5.1/src/astro_extras/utils/utils.py` & `astro_extras-0.1.6/src/astro_extras/utils/utils.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5.1/src/astro_extras.egg-info/PKG-INFO` & `astro_extras-0.1.6/src/astro_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.1.5.1
+Version: 0.1.6
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.1.5.1/src/astro_extras.egg-info/SOURCES.txt` & `astro_extras-0.1.6/src/astro_extras.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 src/astro_extras/operators/table.py
 src/astro_extras/sensors/__init__.py
 src/astro_extras/sensors/auto.py
 src/astro_extras/sensors/file.py
 src/astro_extras/templates/session_close.sql
 src/astro_extras/templates/session_open.sql
 src/astro_extras/templates/table_actuals_select.sql
+src/astro_extras/templates/table_actuals_select_all.sql
+src/astro_extras/templates/table_actuals_select_delta.sql
 src/astro_extras/templates/table_timed_update.sql
 src/astro_extras/templates/table_transfer_nosess.sql
 src/astro_extras/templates/table_transfer_sess.sql
 src/astro_extras/utils/__init__.py
 src/astro_extras/utils/data_compare.py
 src/astro_extras/utils/datetime_local.py
 src/astro_extras/utils/postgres_sql.py
```

### Comparing `astro_extras-0.1.5.1/tests/test_session.py` & `astro_extras-0.1.6/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5.1/tests/test_table.py` & `astro_extras-0.1.6/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5.1/tests/test_templates.py` & `astro_extras-0.1.6/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.1.5.1/tests/test_utils.py` & `astro_extras-0.1.6/tests/test_utils.py`

 * *Files identical despite different names*

