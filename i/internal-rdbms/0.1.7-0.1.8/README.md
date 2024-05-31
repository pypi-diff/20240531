# Comparing `tmp/internal_rdbms-0.1.7.tar.gz` & `tmp/internal_rdbms-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internal_rdbms-0.1.7.tar", max compression
+gzip compressed data, was "internal_rdbms-0.1.8.tar", max compression
```

## Comparing `internal_rdbms-0.1.7.tar` & `internal_rdbms-0.1.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776995 internal_rdbms-0.1.7/README.md
--rw-r--r--   0        0        0      705 2024-05-24 09:37:24.882109 internal_rdbms-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776948 internal_rdbms-0.1.7/src/internal/__init__.py
--rw-r--r--   0        0        0      892 2024-05-21 10:53:42.491696 internal_rdbms-0.1.7/src/internal/base_config.py
--rw-r--r--   0        0        0     8558 2024-05-22 10:06:29.056284 internal_rdbms-0.1.7/src/internal/base_factory.py
--rw-r--r--   0        0        0        0 2024-02-13 10:57:40.969610 internal_rdbms-0.1.7/src/internal/common_enum/__init__.py
--rw-r--r--   0        0        0       90 2024-05-21 13:22:22.135464 internal_rdbms-0.1.7/src/internal/common_enum/order_type.py
--rw-r--r--   0        0        0     1604 2024-05-21 13:22:22.137838 internal_rdbms-0.1.7/src/internal/const.py
--rw-r--r--   0        0        0     2066 2024-05-22 03:53:24.284850 internal_rdbms-0.1.7/src/internal/database.py
--rw-r--r--   0        0        0        0 2023-12-15 06:58:26.332564 internal_rdbms-0.1.7/src/internal/exception/__init__.py
--rw-r--r--   0        0        0      363 2024-01-28 10:00:28.362441 internal_rdbms-0.1.7/src/internal/exception/base_exception.py
--rw-r--r--   0        0        0     1640 2024-05-21 13:23:31.968522 internal_rdbms-0.1.7/src/internal/exception/internal_exception.py
--rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564151 internal_rdbms-0.1.7/src/internal/ext/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564243 internal_rdbms-0.1.7/src/internal/ext/amazon/__init__.py
--rw-r--r--   0        0        0      834 2024-01-29 02:46:13.060361 internal_rdbms-0.1.7/src/internal/ext/amazon/aws/__init__.py
--rw-r--r--   0        0        0      109 2023-12-11 01:32:53.463567 internal_rdbms-0.1.7/src/internal/ext/amazon/aws/const.py
--rw-r--r--   0        0        0        0 2023-11-10 12:37:53.063137 internal_rdbms-0.1.7/src/internal/http/__init__.py
--rw-r--r--   0        0        0     1680 2024-05-24 09:37:24.884344 internal_rdbms-0.1.7/src/internal/http/requests.py
--rw-r--r--   0        0        0     1175 2024-05-22 08:38:49.255872 internal_rdbms-0.1.7/src/internal/http/responses.py
--rw-r--r--   0        0        0        0 2023-12-29 03:03:59.978251 internal_rdbms-0.1.7/src/internal/interface/__init__.py
--rw-r--r--   0        0        0      340 2024-01-28 03:32:05.468971 internal_rdbms-0.1.7/src/internal/interface/base_interface.py
--rw-r--r--   0        0        0        0 2023-11-29 11:18:12.218216 internal_rdbms-0.1.7/src/internal/model/__init__.py
--rw-r--r--   0        0        0      711 2024-05-22 08:38:49.254047 internal_rdbms-0.1.7/src/internal/model/base_model.py
--rw-r--r--   0        0        0        0 2024-01-03 02:21:34.411884 internal_rdbms-0.1.7/src/internal/schema/__init__.py
--rw-r--r--   0        0        0      324 2024-05-20 06:08:36.689816 internal_rdbms-0.1.7/src/internal/schema/base_schema.py
--rw-r--r--   0        0        0     2753 2024-05-22 07:29:57.723151 internal_rdbms-0.1.7/src/internal/utils.py
--rw-r--r--   0        0        0     1112 1970-01-01 00:00:00.000000 internal_rdbms-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776995 internal_rdbms-0.1.8/README.md
+-rw-r--r--   0        0        0      705 2024-05-31 02:00:14.424633 internal_rdbms-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776948 internal_rdbms-0.1.8/src/internal/__init__.py
+-rw-r--r--   0        0        0      892 2024-05-21 10:53:42.491696 internal_rdbms-0.1.8/src/internal/base_config.py
+-rw-r--r--   0        0        0     8577 2024-05-31 01:55:46.762554 internal_rdbms-0.1.8/src/internal/base_factory.py
+-rw-r--r--   0        0        0        0 2024-02-13 10:57:40.969610 internal_rdbms-0.1.8/src/internal/common_enum/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-21 13:22:22.135464 internal_rdbms-0.1.8/src/internal/common_enum/order_type.py
+-rw-r--r--   0        0        0     1604 2024-05-21 13:22:22.137838 internal_rdbms-0.1.8/src/internal/const.py
+-rw-r--r--   0        0        0     2066 2024-05-22 03:53:24.284850 internal_rdbms-0.1.8/src/internal/database.py
+-rw-r--r--   0        0        0        0 2023-12-15 06:58:26.332564 internal_rdbms-0.1.8/src/internal/exception/__init__.py
+-rw-r--r--   0        0        0      363 2024-01-28 10:00:28.362441 internal_rdbms-0.1.8/src/internal/exception/base_exception.py
+-rw-r--r--   0        0        0     1640 2024-05-21 13:23:31.968522 internal_rdbms-0.1.8/src/internal/exception/internal_exception.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564151 internal_rdbms-0.1.8/src/internal/ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564243 internal_rdbms-0.1.8/src/internal/ext/amazon/__init__.py
+-rw-r--r--   0        0        0      834 2024-01-29 02:46:13.060361 internal_rdbms-0.1.8/src/internal/ext/amazon/aws/__init__.py
+-rw-r--r--   0        0        0      109 2023-12-11 01:32:53.463567 internal_rdbms-0.1.8/src/internal/ext/amazon/aws/const.py
+-rw-r--r--   0        0        0        0 2023-11-10 12:37:53.063137 internal_rdbms-0.1.8/src/internal/http/__init__.py
+-rw-r--r--   0        0        0     1680 2024-05-24 09:37:24.884344 internal_rdbms-0.1.8/src/internal/http/requests.py
+-rw-r--r--   0        0        0     1175 2024-05-22 08:38:49.255872 internal_rdbms-0.1.8/src/internal/http/responses.py
+-rw-r--r--   0        0        0        0 2023-12-29 03:03:59.978251 internal_rdbms-0.1.8/src/internal/interface/__init__.py
+-rw-r--r--   0        0        0      340 2024-01-28 03:32:05.468971 internal_rdbms-0.1.8/src/internal/interface/base_interface.py
+-rw-r--r--   0        0        0        0 2023-11-29 11:18:12.218216 internal_rdbms-0.1.8/src/internal/model/__init__.py
+-rw-r--r--   0        0        0      711 2024-05-22 08:38:49.254047 internal_rdbms-0.1.8/src/internal/model/base_model.py
+-rw-r--r--   0        0        0        0 2024-01-03 02:21:34.411884 internal_rdbms-0.1.8/src/internal/schema/__init__.py
+-rw-r--r--   0        0        0      324 2024-05-20 06:08:36.689816 internal_rdbms-0.1.8/src/internal/schema/base_schema.py
+-rw-r--r--   0        0        0     2753 2024-05-22 07:29:57.723151 internal_rdbms-0.1.8/src/internal/utils.py
+-rw-r--r--   0        0        0     1112 1970-01-01 00:00:00.000000 internal_rdbms-0.1.8/PKG-INFO
```

### Comparing `internal_rdbms-0.1.7/pyproject.toml` & `internal_rdbms-0.1.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "internal-rdbms"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["Ray <ray@cruisys.com>"]
 readme = "README.md"
 packages = [{include = "internal", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `internal_rdbms-0.1.7/src/internal/base_config.py` & `internal_rdbms-0.1.8/src/internal/base_config.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.7/src/internal/base_factory.py` & `internal_rdbms-0.1.8/src/internal/base_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             if app.state.db._engine is not None:
                 await app.state.db.close()
 
         if title is None:
             title = self.DEFAULT_APP_NAME
 
         app = FastAPI(openapi_url=self.get_app_config().OPEN_API_URL, title=title, debug=self.get_app_config().DEBUG,
-                      version=self.API_VERSION)
+                      version=self.API_VERSION, lifespan=lifespan)
 
         origins = ["*"]
 
         app.add_middleware(
             CORSMiddleware,
             allow_origins=origins,
             allow_credentials=True,
```

### Comparing `internal_rdbms-0.1.7/src/internal/const.py` & `internal_rdbms-0.1.8/src/internal/const.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.7/src/internal/database.py` & `internal_rdbms-0.1.8/src/internal/database.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.7/src/internal/exception/internal_exception.py` & `internal_rdbms-0.1.8/src/internal/exception/internal_exception.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.7/src/internal/ext/amazon/aws/__init__.py` & `internal_rdbms-0.1.8/src/internal/ext/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.7/src/internal/http/requests.py` & `internal_rdbms-0.1.8/src/internal/http/requests.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.7/src/internal/http/responses.py` & `internal_rdbms-0.1.8/src/internal/http/responses.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.7/src/internal/model/base_model.py` & `internal_rdbms-0.1.8/src/internal/model/base_model.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.7/src/internal/utils.py` & `internal_rdbms-0.1.8/src/internal/utils.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.7/PKG-INFO` & `internal_rdbms-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internal-rdbms
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Ray
 Author-email: ray@cruisys.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

