# Comparing `tmp/pyqueen-1.1.2.tar.gz` & `tmp/pyqueen-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqueen-1.1.2.tar", last modified: Thu May 30 14:14:30 2024, max compression
+gzip compressed data, was "pyqueen-1.1.3.tar", last modified: Fri May 31 07:35:40 2024, max compression
```

## Comparing `pyqueen-1.1.2.tar` & `pyqueen-1.1.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.659702 pyqueen-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-30 14:14:26.000000 pyqueen-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-30 14:14:30.659702 pyqueen-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-30 14:14:26.000000 pyqueen-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.651701 pyqueen-1.1.2/pyqueen/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.655701 pyqueen-1.1.2/pyqueen/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/analysis/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.655701 pyqueen-1.1.2/pyqueen/chart/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/chart/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.655701 pyqueen-1.1.2/pyqueen/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/ds_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/kvdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/sqldb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/io/web.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.655701 pyqueen-1.1.2/pyqueen/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/remote/linux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.655701 pyqueen-1.1.2/pyqueen/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/service/pydingtalk.py
--rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/service/pyemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/service/pywechat.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/service/showdoc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.659702 pyqueen-1.1.2/pyqueen/utility/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/utility/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/utility/time_kit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-30 14:14:26.000000 pyqueen-1.1.2/pyqueen/utility/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.659702 pyqueen-1.1.2/pyqueen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-30 14:14:30.000000 pyqueen-1.1.2/pyqueen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-30 14:14:30.000000 pyqueen-1.1.2/pyqueen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 14:14:30.000000 pyqueen-1.1.2/pyqueen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 14:14:30.000000 pyqueen-1.1.2/pyqueen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 14:14:30.000000 pyqueen-1.1.2/pyqueen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 14:14:30.000000 pyqueen-1.1.2/pyqueen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 14:14:30.659702 pyqueen-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-30 14:14:26.000000 pyqueen-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:30.659702 pyqueen-1.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 14:14:26.000000 pyqueen-1.1.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-30 14:14:26.000000 pyqueen-1.1.2/test/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:40.115262 pyqueen-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-31 07:35:36.000000 pyqueen-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-31 07:35:40.115262 pyqueen-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-31 07:35:36.000000 pyqueen-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:40.111262 pyqueen-1.1.3/pyqueen/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:40.111262 pyqueen-1.1.3/pyqueen/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/analysis/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:40.111262 pyqueen-1.1.3/pyqueen/chart/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/chart/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:40.115262 pyqueen-1.1.3/pyqueen/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/io/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/io/ds_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/io/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/io/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/io/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/io/kvdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/io/sqldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/io/web.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:40.115262 pyqueen-1.1.3/pyqueen/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/remote/linux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:40.115262 pyqueen-1.1.3/pyqueen/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/service/pydingtalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3641 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/service/pyemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/service/pywechat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/service/showdoc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:40.115262 pyqueen-1.1.3/pyqueen/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/utility/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/utility/time_kit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-05-31 07:35:36.000000 pyqueen-1.1.3/pyqueen/utility/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:40.115262 pyqueen-1.1.3/pyqueen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-31 07:35:40.000000 pyqueen-1.1.3/pyqueen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-31 07:35:40.000000 pyqueen-1.1.3/pyqueen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 07:35:40.000000 pyqueen-1.1.3/pyqueen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 07:35:40.000000 pyqueen-1.1.3/pyqueen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-31 07:35:40.000000 pyqueen-1.1.3/pyqueen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 07:35:40.000000 pyqueen-1.1.3/pyqueen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 07:35:40.115262 pyqueen-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-05-31 07:35:36.000000 pyqueen-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:40.115262 pyqueen-1.1.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 07:35:36.000000 pyqueen-1.1.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-31 07:35:36.000000 pyqueen-1.1.3/test/test_main.py
```

### Comparing `pyqueen-1.1.2/LICENSE` & `pyqueen-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/PKG-INFO` & `pyqueen-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqueen
-Version: 1.1.2
+Version: 1.1.3
 Summary: Rule your Data
 Home-page: https://github.com/ts7ming/pyqueen.git
 Author: ts7ming
 Author-email: qiming.ma@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyqueen-1.1.2/README.md` & `pyqueen-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen/analysis/model.py` & `pyqueen-1.1.3/pyqueen/analysis/model.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen/chart/plot.py` & `pyqueen-1.1.3/pyqueen/chart/plot.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen/io/data_source.py` & `pyqueen-1.1.3/pyqueen/io/data_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 __support_conn_type__ = tuple(__conn_type_mapping__.keys())
 
 
 class DataSource(DsLog, DsPlugin, DsConfig, DsExt):
     def __init__(self, conn_type='excel', host=None, username=None, password=None, port=None, db_name=None, db_type=None, file_path=None, jdbc_url=None,
                  cache_dir=None, keep_conn=False, charset=None, conn_package=None, conn_params=None):
         super().__init__()
-        if conn_type is None and db_type is not None:
+        if db_type is not None and conn_type == 'excel':
             warnings.warn(message="recommend using the 'conn_type' field instead of 'db_type'", category=PendingDeprecationWarning)
             conn_type = db_type
         conn_type = str(conn_type).lower()
         self.operator_name = __conn_type_mapping__[conn_type]['class']
         self.__init_params = {k: v for k, v in locals().items()}
         self.__init_params['conn_type'] = conn_type
         self.__build_conn()
```

### Comparing `pyqueen-1.1.2/pyqueen/io/ds_plugin.py` & `pyqueen-1.1.3/pyqueen/io/ds_plugin.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen/io/excel.py` & `pyqueen-1.1.3/pyqueen/io/excel.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen/io/ftp.py` & `pyqueen-1.1.3/pyqueen/io/ftp.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen/io/image.py` & `pyqueen-1.1.3/pyqueen/io/image.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen/io/kvdb.py` & `pyqueen-1.1.3/pyqueen/io/kvdb.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,20 +19,20 @@
     def close_conn(self):
         if self.__keep_conn is False:
             if str(self.__conn_type).lower() == 'redis':
                 self.__conn.close()
             else:
                 raise Exception('Unknown conn_type: ' + str(self.__conn_type))
 
-    def get_v(self, k):
+    def get_v(self, key):
         self.create_conn()
-        v = self.__conn.get(k)
+        value = self.__conn.get(key)
         self.close_conn()
-        if v is None:
+        if value is None:
             return None
-        v = v.decode(encoding=self.__charset)
-        return v
+        value = value.decode(encoding=self.__charset)
+        return value
 
-    def set_v(self, k, v):
+    def set_v(self, key, value):
         self.create_conn()
-        self.__conn.set(k, v)
+        self.__conn.set(key, value)
         self.close_conn()
```

### Comparing `pyqueen-1.1.2/pyqueen/io/sqldb.py` & `pyqueen-1.1.3/pyqueen/io/sqldb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import os
 from sqlalchemy import create_engine, text
 import pandas as pd
 import inspect
-
+from urllib.parse import quote_plus
 
 class SqlDB:
     def __init__(self, conn_package=None, db_type=None, host=None, username=None, password=None, port=None, db_name=None, jdbc_url=None,
                  keep_conn=False, conn_params=None):
         self.__conn = None
         self.__engine = None
         self.__base_param = {
             'db_type': db_type,
             'package': str(conn_package),
             'username': str(username),
-            'password': str(password),
+            'password': quote_plus(password),
             'host': str(host),
             'port': str(port),
             'db_name': str(db_name),
         }
         self.__url = jdbc_url
         self.__ext_param = None
         self.__conn_params = conn_params
@@ -188,15 +188,15 @@
         super().__init__(**run_param)
 
 
 class Clickhouse(SqlDB):
     def __init__(self, host, username, password, port, db_name, conn_package='native', keep_conn=False, jdbc_url=None):
         self.__host = host
         self.__username = username
-        self.__password = password
+        self.__password = quote_plus(password)
         self.__port = port
         self.__db_name = db_name
         req_params = list(inspect.signature(super().__init__).parameters.keys())
         run_param = {k: v for k, v in locals().items() if k in req_params}
         run_param['db_type'] = 'clickhouse'
         super().__init__(**run_param)
```

### Comparing `pyqueen-1.1.2/pyqueen/io/web.py` & `pyqueen-1.1.3/pyqueen/io/web.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen/remote/linux.py` & `pyqueen-1.1.3/pyqueen/remote/linux.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen/service/pydingtalk.py` & `pyqueen-1.1.3/pyqueen/service/pydingtalk.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen/service/pyemail.py` & `pyqueen-1.1.3/pyqueen/service/pyemail.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen/service/pywechat.py` & `pyqueen-1.1.3/pyqueen/service/pywechat.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen/service/showdoc.py` & `pyqueen-1.1.3/pyqueen/service/showdoc.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen/utility/command.py` & `pyqueen-1.1.3/pyqueen/utility/command.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen/utility/time_kit.py` & `pyqueen-1.1.3/pyqueen/utility/time_kit.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen/utility/utils.py` & `pyqueen-1.1.3/pyqueen/utility/utils.py`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/pyqueen.egg-info/PKG-INFO` & `pyqueen-1.1.3/pyqueen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqueen
-Version: 1.1.2
+Version: 1.1.3
 Summary: Rule your Data
 Home-page: https://github.com/ts7ming/pyqueen.git
 Author: ts7ming
 Author-email: qiming.ma@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyqueen-1.1.2/pyqueen.egg-info/SOURCES.txt` & `pyqueen-1.1.3/pyqueen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyqueen-1.1.2/setup.py` & `pyqueen-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyqueen',
-    version='1.1.2',
+    version='1.1.3',
     url='https://github.com/ts7ming/pyqueen.git',
     description='Rule your Data',
     long_description=open("README.md", encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     author='ts7ming',
     author_email='qiming.ma@outlook.com',
     packages=find_packages(),
```

### Comparing `pyqueen-1.1.2/test/test_main.py` & `pyqueen-1.1.3/test/test_main.py`

 * *Files identical despite different names*

