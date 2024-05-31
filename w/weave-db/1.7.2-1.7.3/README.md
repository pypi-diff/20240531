# Comparing `tmp/weave-db-1.7.2.tar.gz` & `tmp/weave_db-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weave-db-1.7.2.tar", last modified: Thu Apr  4 13:55:10 2024, max compression
+gzip compressed data, was "weave_db-1.7.3.tar", last modified: Fri May 31 19:01:39 2024, max compression
```

## Comparing `weave-db-1.7.2.tar` & `weave_db-1.7.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:55:10.350135 weave-db-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-04 13:55:10.350135 weave-db-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-04-04 13:55:06.000000 weave-db-1.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:55:10.350135 weave-db-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-04 13:55:06.000000 weave-db-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:55:10.346135 weave-db-1.7.2/weave/
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/basket.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:55:10.346135 weave-db-1.7.2/weave/index/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/create_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/index_abc.py
--rw-r--r--   0 runner    (1001) docker     (127)    22456 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/index_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)    31379 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/index_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    22656 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/index_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/list_baskets.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/index/validate_basket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/metadata_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/mongo_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/pantry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:55:10.346135 weave-db-1.7.2/weave/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/pytest_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    26482 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_basket.py
--rw-r--r--   0 runner    (1001) docker     (127)    65508 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_index_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_index_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_index_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_mongo_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    26212 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_pantry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_pytest.py
--rw-r--r--   0 runner    (1001) docker     (127)    44925 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)    61528 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/tests/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19221 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-04-04 13:55:06.000000 weave-db-1.7.2/weave/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:55:10.350135 weave-db-1.7.2/weave_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-04-04 13:55:10.000000 weave-db-1.7.2/weave_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-04 13:55:10.000000 weave-db-1.7.2/weave_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:55:10.000000 weave-db-1.7.2/weave_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-04 13:55:10.000000 weave-db-1.7.2/weave_db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-04 13:55:10.000000 weave-db-1.7.2/weave_db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:01:39.634607 weave_db-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-05-31 19:01:39.634607 weave_db-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-05-31 19:01:36.000000 weave_db-1.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 19:01:39.638607 weave_db-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-05-31 19:01:36.000000 weave_db-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:01:39.630607 weave_db-1.7.3/weave/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10732 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/basket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:01:39.630607 weave_db-1.7.3/weave/index/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/index/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/index/index_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22707 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/index/index_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31402 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/index/index_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22679 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/index/index_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/index/list_baskets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/index/validate_basket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/metadata_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/mongo_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10682 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/pantry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:01:39.634607 weave_db-1.7.3/weave/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/tests/pytest_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26482 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/tests/test_basket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65508 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9255 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/tests/test_index_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/tests/test_index_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7091 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/tests/test_index_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16220 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/tests/test_mongo_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26237 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/tests/test_pantry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/tests/test_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44925 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/tests/test_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61687 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19221 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14582 2024-05-31 19:01:36.000000 weave_db-1.7.3/weave/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:01:39.634607 weave_db-1.7.3/weave_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11530 2024-05-31 19:01:39.000000 weave_db-1.7.3/weave_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-31 19:01:39.000000 weave_db-1.7.3/weave_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:01:39.000000 weave_db-1.7.3/weave_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-31 19:01:39.000000 weave_db-1.7.3/weave_db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-31 19:01:39.000000 weave_db-1.7.3/weave_db.egg-info/top_level.txt
```

### Comparing `weave-db-1.7.2/PKG-INFO` & `weave_db-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weave-db
-Version: 1.7.2
+Version: 1.7.3
 Summary: Library to facilitate the creation and maintenance of complex data warehouses.
 Home-page: https://github.com/309thEDDGE/weave
 Author: 309thEDDGE
 License: GNU General Public
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `weave-db-1.7.2/README.md` & `weave_db-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/setup.py` & `weave_db-1.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/__init__.py` & `weave_db-1.7.3/weave/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from .index.index_pandas import IndexPandas
 from .index.index_sqlite import IndexSQLite
 from .index.index_sql import IndexSQL
 from .pantry import Pantry
 from .metadata_db import load_mongo
 from .mongo_db import MongoDB
 
-__version__ = "1.7.2"
+__version__ = "1.7.3"
 
 __all__ = [
     "Basket",
     "IndexPandas",
     "IndexSQLite",
     "IndexSQL",
     "Pantry",
```

### Comparing `weave-db-1.7.2/weave/basket.py` & `weave_db-1.7.3/weave/basket.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/config.py` & `weave_db-1.7.3/weave/config.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/index/create_index.py` & `weave_db-1.7.3/weave/index/create_index.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/index/index_abc.py` & `weave_db-1.7.3/weave/index/index_abc.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/index/index_pandas.py` & `weave_db-1.7.3/weave/index/index_pandas.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,14 +305,15 @@
             )
 
         # Once we have exceeded our max_gen_level, we simply want
         # to return our data
         if gen_level > max_gen_level:
             return data
 
+        current_uuid = None
         if self.file_system.exists(basket_address):
             current_uuid = self.index_df["uuid"].loc[
                 self.index_df["address"].str.endswith(basket_address)
             ].values[0]
         elif basket_address in self.index_df.uuid.values:
             current_uuid = basket_address
 
@@ -402,14 +403,15 @@
             )
 
         # Once we have exceeded our min_gen_level, we simply want
         # to return our data
         if gen_level < min_gen_level:
             return data
 
+        current_uuid = None
         if self.file_system.exists(basket_address):
             current_uuid = self.index_df["uuid"].loc[
                 self.index_df["address"].str.endswith(basket_address)
             ].values[0]
         elif basket_address in self.index_df.uuid.values:
             current_uuid = basket_address
 
@@ -449,23 +451,28 @@
         data = data.drop_duplicates(
             subset=['uuid', 'generation_level']
         ).reset_index(drop=True)
 
         return data
 
     def track_basket(self, entry_df, **kwargs):
-        """Track a basket to from the pantry referenced by the Index.
+        """Track a basket from the pantry referenced by the Index.
 
         Parameters
         ----------
         entry_df : pd.DataFrame
             The entry to be added to the index.
 
         **kwargs unused for this class.
         """
+        index_paths = self.file_system.glob(
+            os.path.join(self.index_basket_dir_path, "**", "*-index.json")
+        )
+        if len(index_paths) > 0:
+            self._sync_if_needed()
         if not self._sync_if_needed():
             self._upload_index(
                 pd.concat(
                     [df for df in [self.index_df, entry_df] if len(df) > 0],
                     ignore_index=True
                 )
             )
```

### Comparing `weave-db-1.7.2/weave/index/index_sql.py` & `weave_db-1.7.3/weave/index/index_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -759,14 +759,15 @@
             return self.to_pandas_df(max_rows=max_rows, offset=offset)
 
         pre_query = f"SELECT * FROM {self.pantry_schema}.pantry_index "
         post_query = """ORDER BY UUID
                         OFFSET (:offset) ROWS
                         FETCH FIRST (:max_rows) ROWS ONLY"""
 
+        columns = None
         if start_time and end_time:
             start_time = int(datetime.timestamp(start_time))
             end_time = int(datetime.timestamp(end_time))
             query = "WHERE upload_time >= :start_time " \
                     "AND upload_time <= :end_time "
             results, columns = self.execute_sql(
                 pre_query + query + post_query,
```

### Comparing `weave-db-1.7.2/weave/index/index_sqlite.py` & `weave_db-1.7.3/weave/index/index_sqlite.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,14 +559,15 @@
             return self.to_pandas_df(max_rows=max_rows, offset=offset)
 
         columns = (
             [info[1] for info in
              self.cur.execute("PRAGMA table_info(pantry_index)").fetchall()]
         )
 
+        results = None
         if start_time and end_time:
             start_time = int(datetime.timestamp(start_time))
             end_time = int(datetime.timestamp(end_time))
             results = self.cur.execute(
                 """SELECT * FROM pantry_index
                 WHERE upload_time >= ? AND upload_time <= ?
                 ORDER BY UUID LIMIT ? OFFSET ?
```

### Comparing `weave-db-1.7.2/weave/index/validate_basket.py` & `weave_db-1.7.3/weave/index/validate_basket.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/metadata_db.py` & `weave_db-1.7.3/weave/metadata_db.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/mongo_db.py` & `weave_db-1.7.3/weave/mongo_db.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/pantry.py` & `weave_db-1.7.3/weave/pantry.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/tests/pytest_resources.py` & `weave_db-1.7.3/weave/tests/pytest_resources.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/tests/test_basket.py` & `weave_db-1.7.3/weave/tests/test_basket.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/tests/test_index.py` & `weave_db-1.7.3/weave/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/tests/test_index_pandas.py` & `weave_db-1.7.3/weave/tests/test_index_pandas.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Pytest tests for the index directory."""
 import os
 import re
+import tempfile
 
 import pytest
 
 from weave.pantry import Pantry
 from weave.index.index_pandas import IndexPandas
 from weave.tests.pytest_resources import PantryForTest, get_file_systems
 
@@ -217,7 +218,43 @@
         pantry_path=test_pantry.pantry_path,
         file_system=test_pantry.file_system,
         sync=True,
     )
     pantry2.index.generate_index()
     assert pantry2.index.is_index_current() is True
     assert pantry.index.is_index_current() is False
+
+def test_index_updated_after_new_pantry_basket_upload(test_pantry):
+    """Tests basket_upload updates the index after creating IndexPandas pantry
+    object when another IndexPandas index exists."""
+
+    # Create first pantry
+    pantry = Pantry(
+        IndexPandas,
+        pantry_path=test_pantry.pantry_path,
+        file_system=test_pantry.file_system,
+        sync=True,
+    )
+    # Create temp directory for uploading basket
+    with tempfile.TemporaryDirectory(dir=".") as tmpdir:
+        tmp_file_path = os.path.join(tmpdir, "temp_basket.txt")
+        with open(tmp_file_path, "w", encoding="utf-8") as tmp_file:
+            pantry.upload_basket(
+                upload_items=[{"path":tmp_file.name, "stub":False}],
+                basket_type="test-1",
+            )
+    # Create second pantry
+    pantry2 = Pantry(
+        IndexPandas,
+        pantry_path=test_pantry.pantry_path,
+        file_system=test_pantry.file_system,
+        sync=True,
+    )
+    # Upload basket with new index
+    with tempfile.TemporaryDirectory(dir=".") as tmpdir:
+        tmp_file_path = os.path.join(tmpdir, "temp_basket.txt")
+        with open(tmp_file_path, "w", encoding="utf-8") as tmp_file:
+            pantry2.upload_basket(
+                upload_items=[{"path":tmp_file.name, "stub":False}],
+                basket_type="test-1",
+            )
+    assert len(pantry2.index.to_pandas_df()) == 2
```

### Comparing `weave-db-1.7.2/weave/tests/test_index_sql.py` & `weave_db-1.7.3/weave/tests/test_index_sql.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/tests/test_index_sqlite.py` & `weave_db-1.7.3/weave/tests/test_index_sqlite.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/tests/test_mongo_db.py` & `weave_db-1.7.3/weave/tests/test_mongo_db.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/tests/test_pantry.py` & `weave_db-1.7.3/weave/tests/test_pantry.py`

 * *Files 0% similar despite different names*

```diff
@@ -574,14 +574,15 @@
     pantry = Pantry(
         IndexPandas,
         pantry_path=test_pantry.pantry_path,
         file_system=test_pantry.file_system
     )
     pantry.save_metadata()
 
+    file_metadata = None
     if pantry.file_system.exists(pantry.metadata_path):
         with pantry.file_system.open(pantry.metadata_path, "rb") as file:
             file_metadata = json.load(file)
 
     assert pantry.file_system.exists(pantry.metadata_path)
     assert pantry.metadata == file_metadata
```

### Comparing `weave-db-1.7.2/weave/tests/test_pytest.py` & `weave_db-1.7.3/weave/tests/test_pytest.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/tests/test_uploader.py` & `weave_db-1.7.3/weave/tests/test_uploader.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/tests/test_validate.py` & `weave_db-1.7.3/weave/tests/test_validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,14 +364,16 @@
     # In this next section, find the supplement, which has a bad path in it,
     # pull it down, and modify it to have the proper path inside the
     # supplement's integrity data. Do this because the custom supplement
     # dictionary didn't have the correct upload path
     with test_validate.file_system.open(supplement_path, "rb",) as file:
         supplement_dict = json.load(file)
 
+    nested_supp_path = None
+    test_txt_path = None
     for integrity_data in supplement_dict["integrity_data"]:
         if integrity_data["upload_path"].endswith("basket_supplement.json"):
             nested_supp_path = integrity_data["upload_path"]
         if integrity_data["upload_path"].endswith(".txt"):
             test_txt_path = integrity_data["upload_path"]
 
     with test_validate.file_system.open(nested_supp_path, "rb",) as supp_file:
@@ -450,14 +452,16 @@
     # In this next section, find the supplement, which has a bad path in it,
     # pull it down, and modify it to have the proper path inside the
     # supplement's integrity data. Do this because the custom supplement
     # dictionary didn't have the correct upload path
     with test_validate.file_system.open(supplement_path, "rb",) as file:
         supplement_dict = json.load(file)
 
+    nested_supp_path = None
+    test_txt_path = None
     for integrity_data in supplement_dict["integrity_data"]:
         if integrity_data["upload_path"].endswith("basket_supplement.json"):
             nested_supp_path = integrity_data["upload_path"]
         if integrity_data["upload_path"].endswith(".txt"):
             test_txt_path = integrity_data["upload_path"]
 
     with test_validate.file_system.open(nested_supp_path, "rb",) as supp_file:
@@ -1061,14 +1065,16 @@
     # In this next section, find the supplement, which has a bad path in it,
     # pull it down, and modify it to have the proper path inside the
     # supplement's integrity data. Do this because the custom supplement
     # dictionary didn't have the correct upload path
     with test_validate.file_system.open(supplement_path, "rb",) as file:
         supplement_dict = json.load(file)
 
+    nested_supp_path = None
+    test_txt_path = None
     for integrity_data in supplement_dict["integrity_data"]:
         if integrity_data["upload_path"].endswith("basket_supplement.json"):
             nested_supp_path = integrity_data["upload_path"]
         if integrity_data["upload_path"].endswith(".txt"):
             test_txt_path = integrity_data["upload_path"]
 
     with test_validate.file_system.open(nested_supp_path, "rb",) as supp_file:
```

### Comparing `weave-db-1.7.2/weave/upload.py` & `weave_db-1.7.3/weave/upload.py`

 * *Files identical despite different names*

### Comparing `weave-db-1.7.2/weave/validate.py` & `weave_db-1.7.3/weave/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,14 +314,17 @@
     Parameters:
     -----------
     files_in_basket: [str]
         List of all file paths in a basket.
     pantry: weave.Pantry
         Pantry object representing the pantry to validate.
     """
+    meta_data = None
+    supp_data = None
+    man_data = None
     for file in files_in_basket:
         if file.endswith("basket_manifest.json"):
             man_data = json.load(pantry.file_system.open(file))
 
         if file.endswith("basket_supplement.json"):
             supp_data = json.load(pantry.file_system.open(file))
```

### Comparing `weave-db-1.7.2/weave_db.egg-info/PKG-INFO` & `weave_db-1.7.3/weave_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weave-db
-Version: 1.7.2
+Version: 1.7.3
 Summary: Library to facilitate the creation and maintenance of complex data warehouses.
 Home-page: https://github.com/309thEDDGE/weave
 Author: 309thEDDGE
 License: GNU General Public
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `weave-db-1.7.2/weave_db.egg-info/SOURCES.txt` & `weave_db-1.7.3/weave_db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

