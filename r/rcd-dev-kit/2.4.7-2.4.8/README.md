# Comparing `tmp/rcd_dev_kit-2.4.7.tar.gz` & `tmp/rcd_dev_kit-2.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcd_dev_kit-2.4.7.tar", max compression
+gzip compressed data, was "rcd_dev_kit-2.4.8.tar", max compression
```

## Comparing `rcd_dev_kit-2.4.7.tar` & `rcd_dev_kit-2.4.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rwxr-xr-x   0        0        0     1079 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/LICENSE
--rw-r--r--   0        0        0     5662 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/README.md
--rw-r--r--   0        0        0     3990 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/pyproject.toml
--rw-r--r--   0        0        0      135 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/__init__.py
--rw-r--r--   0        0        0     7119 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/README.md
--rw-r--r--   0        0        0      840 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/__init__.py
--rw-r--r--   0        0        0    15566 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/directus_operator.py
--rw-r--r--   0        0        0    25464 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/elasticsearch_operator.py
--rw-r--r--   0        0        0     8970 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/gcloud_operator.py
--rw-r--r--   0        0        0     4039 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/mview_operator.py
--rw-r--r--   0        0        0      484 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/mysql_operator.py
--rw-r--r--   0        0        0     3120 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/oip_api_operator.py
--rw-r--r--   0        0        0    68735 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/redshift_operator.py
--rw-r--r--   0        0        0     7856 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/s3_operator.py
--rw-r--r--   0        0        0    41001 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/snowflake_operator.py
--rw-r--r--   0        0        0     1567 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/dataclass_manager/README.md
--rw-r--r--   0        0        0       73 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/dataclass_manager/__init__.py
--rw-r--r--   0        0        0     4602 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/dataclass_manager/dictionary.py
--rw-r--r--   0        0        0     2805 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/dataclass_manager/raw_data_file.py
--rw-r--r--   0        0        0      632 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/decorator_manager/README.md
--rw-r--r--   0        0        0       75 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/decorator_manager/__init__.py
--rw-r--r--   0        0        0      530 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/decorator_manager/debug_decorator.py
--rw-r--r--   0        0        0      628 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/decorator_manager/functional_decorator.py
--rw-r--r--   0        0        0     3567 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/file_manager/README.md
--rw-r--r--   0        0        0      270 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/file_manager/__init__.py
--rw-r--r--   0        0        0      334 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/file_manager/file_as_bytes.py
--rw-r--r--   0        0        0     1711 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/file_manager/file_detector.py
--rw-r--r--   0        0        0     8908 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/file_manager/file_downloader.py
--rw-r--r--   0        0        0     2118 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/file_manager/file_operator.py
--rw-r--r--   0        0        0     1390 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/file_manager/file_writer.py
--rw-r--r--   0        0        0     1386 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/pandas_manager/README.md
--rw-r--r--   0        0        0      206 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/pandas_manager/__init__.py
--rw-r--r--   0        0        0     4115 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/pandas_manager/checker.py
--rw-r--r--   0        0        0     3570 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/pandas_manager/detector.py
--rw-r--r--   0        0        0     1127 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/pandas_manager/io.py
--rw-r--r--   0        0        0      579 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/pandas_manager/manipulator.py
--rw-r--r--   0        0        0     6152 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/pandas_manager/normalizer.py
--rw-r--r--   0        0        0       85 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/sql_utils/__init__.py
--rw-r--r--   0        0        0    21107 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/sql_utils/sql2sf.py
--rw-r--r--   0        0        0     9032 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql
--rw-r--r--   0        0        0        0 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/verification_utils/__init__.py
--rw-r--r--   0        0        0     1158 2024-05-17 12:08:22.921869 rcd_dev_kit-2.4.7/src/rcd_dev_kit/verification_utils/verifification.py
--rw-r--r--   0        0        0     7965 1970-01-01 00:00:00.000000 rcd_dev_kit-2.4.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1079 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/LICENSE
+-rw-r--r--   0        0        0     5662 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/README.md
+-rw-r--r--   0        0        0     3990 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/pyproject.toml
+-rw-r--r--   0        0        0      135 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/__init__.py
+-rw-r--r--   0        0        0     7119 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/README.md
+-rw-r--r--   0        0        0      840 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/__init__.py
+-rw-r--r--   0        0        0    15566 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/directus_operator.py
+-rw-r--r--   0        0        0    25464 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/elasticsearch_operator.py
+-rw-r--r--   0        0        0     8970 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/gcloud_operator.py
+-rw-r--r--   0        0        0     4039 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/mview_operator.py
+-rw-r--r--   0        0        0      484 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/mysql_operator.py
+-rw-r--r--   0        0        0     3120 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/oip_api_operator.py
+-rw-r--r--   0        0        0    68735 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/redshift_operator.py
+-rw-r--r--   0        0        0     7856 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/s3_operator.py
+-rw-r--r--   0        0        0    41001 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/snowflake_operator.py
+-rw-r--r--   0        0        0     1567 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/dataclass_manager/README.md
+-rw-r--r--   0        0        0       73 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/dataclass_manager/__init__.py
+-rw-r--r--   0        0        0     4646 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/dataclass_manager/dictionary.py
+-rw-r--r--   0        0        0     2805 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/dataclass_manager/raw_data_file.py
+-rw-r--r--   0        0        0      632 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/decorator_manager/README.md
+-rw-r--r--   0        0        0       75 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/decorator_manager/__init__.py
+-rw-r--r--   0        0        0      530 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/decorator_manager/debug_decorator.py
+-rw-r--r--   0        0        0      628 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/decorator_manager/functional_decorator.py
+-rw-r--r--   0        0        0     3567 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/file_manager/README.md
+-rw-r--r--   0        0        0      270 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/file_manager/__init__.py
+-rw-r--r--   0        0        0      334 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/file_manager/file_as_bytes.py
+-rw-r--r--   0        0        0     1711 2024-05-31 09:49:39.428067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/file_manager/file_detector.py
+-rw-r--r--   0        0        0     8908 2024-05-31 09:49:39.432067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/file_manager/file_downloader.py
+-rw-r--r--   0        0        0     2118 2024-05-31 09:49:39.432067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/file_manager/file_operator.py
+-rw-r--r--   0        0        0     1390 2024-05-31 09:49:39.432067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/file_manager/file_writer.py
+-rw-r--r--   0        0        0     1386 2024-05-31 09:49:39.432067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/pandas_manager/README.md
+-rw-r--r--   0        0        0      206 2024-05-31 09:49:39.432067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/pandas_manager/__init__.py
+-rw-r--r--   0        0        0     4115 2024-05-31 09:49:39.432067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/pandas_manager/checker.py
+-rw-r--r--   0        0        0     3570 2024-05-31 09:49:39.432067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/pandas_manager/detector.py
+-rw-r--r--   0        0        0     1127 2024-05-31 09:49:39.432067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/pandas_manager/io.py
+-rw-r--r--   0        0        0      579 2024-05-31 09:49:39.432067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/pandas_manager/manipulator.py
+-rw-r--r--   0        0        0     6152 2024-05-31 09:49:39.432067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/pandas_manager/normalizer.py
+-rw-r--r--   0        0        0       85 2024-05-31 09:49:39.432067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/sql_utils/__init__.py
+-rw-r--r--   0        0        0    21107 2024-05-31 09:49:39.432067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/sql_utils/sql2sf.py
+-rw-r--r--   0        0        0     9032 2024-05-31 09:49:39.432067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql
+-rw-r--r--   0        0        0        0 2024-05-31 09:49:39.432067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/verification_utils/__init__.py
+-rw-r--r--   0        0        0     1158 2024-05-31 09:49:39.432067 rcd_dev_kit-2.4.8/src/rcd_dev_kit/verification_utils/verifification.py
+-rw-r--r--   0        0        0     7965 1970-01-01 00:00:00.000000 rcd_dev_kit-2.4.8/PKG-INFO
```

### Comparing `rcd_dev_kit-2.4.7/LICENSE` & `rcd_dev_kit-2.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/README.md` & `rcd_dev_kit-2.4.8/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/pyproject.toml` & `rcd_dev_kit-2.4.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rcd-dev-kit"
-version = "2.4.7"
+version = "2.4.8"
 description = "Interact with OIP ecosystem."
 authors = ["Maxime KIEFFER", "Robin Sarfati"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     'Intended Audience :: Developers',
     'Topic :: Software Development :: Build Tools',
```

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/README.md` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/__init__.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/directus_operator.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/directus_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/elasticsearch_operator.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/elasticsearch_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/gcloud_operator.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/gcloud_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/mview_operator.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/mview_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/oip_api_operator.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/oip_api_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/redshift_operator.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/redshift_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/s3_operator.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/s3_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/database_manager/snowflake_operator.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/database_manager/snowflake_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/dataclass_manager/README.md` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/dataclass_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/dataclass_manager/dictionary.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/dataclass_manager/dictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,26 +67,27 @@
         current_pk = self.ro.get_primary_keys()
         if len(column_pivot) == 0 and mode != "overwrite" and len(current_pk) > 0:
             print('Search for primary key ...')
             column_pivot = current_pk
             print('column_pivot = ', column_pivot)
         send_to_redshift(database=self.database, schema=self.schema_name, table=self.table_name,
                          df=df,
+                         primary_key=pk,
                          json_path=json_path,
                          mode=mode, column_pivot=column_pivot,
                          drop=drop,
                          check=check,
                          first_data=first_data,
                          last_data=last_data
                          )
-        if pk:
-            self.set_primary_keys(pk)
+        #if pk:
+        #   self.set_primary_keys(pk)
 
-    def set_primary_keys(self, lst_pk: list = [], drop: bool = False):
-        self.ro.set_primary_key(columns=lst_pk, drop=drop)
+    #def set_primary_keys(self, lst_pk: list = [], drop: bool = False):
+        #self.ro.set_primary_key(columns=lst_pk, drop=drop)
 
     def get(self):
         if self.ro.detect_table():
             self.df_final = read_from_redshift(database=self.database, method='auto',
                                                schema=self.schema_name, table=self.table_name)
         else:
             print(f"❌ Table {self.schema_name}.{self.table_name} does not exist")
```

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/dataclass_manager/raw_data_file.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/dataclass_manager/raw_data_file.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/decorator_manager/README.md` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/decorator_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/decorator_manager/debug_decorator.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/decorator_manager/debug_decorator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/decorator_manager/functional_decorator.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/decorator_manager/functional_decorator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/file_manager/README.md` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/file_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/file_manager/file_detector.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/file_manager/file_detector.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/file_manager/file_downloader.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/file_manager/file_downloader.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/file_manager/file_operator.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/file_manager/file_operator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/file_manager/file_writer.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/file_manager/file_writer.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/pandas_manager/README.md` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/pandas_manager/README.md`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/pandas_manager/checker.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/pandas_manager/checker.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/pandas_manager/detector.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/pandas_manager/detector.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/pandas_manager/io.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/pandas_manager/io.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/pandas_manager/manipulator.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/pandas_manager/manipulator.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/pandas_manager/normalizer.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/pandas_manager/normalizer.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/sql_utils/sql2sf.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/sql_utils/sql2sf.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/sql_utils/v_generate_tbl_ddl.sql`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/src/rcd_dev_kit/verification_utils/verifification.py` & `rcd_dev_kit-2.4.8/src/rcd_dev_kit/verification_utils/verifification.py`

 * *Files identical despite different names*

### Comparing `rcd_dev_kit-2.4.7/PKG-INFO` & `rcd_dev_kit-2.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcd-dev-kit
-Version: 2.4.7
+Version: 2.4.8
 Summary: Interact with OIP ecosystem.
 Home-page: https://github.com/Tekkare/rcd-dev-kit
 License: MIT
 Author: Maxime KIEFFER
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

