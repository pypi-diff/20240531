# Comparing `tmp/stac_fastapi_api-3.0.0a1.tar.gz` & `tmp/stac_fastapi_api-3.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_api-3.0.0a1.tar", last modified: Wed May 22 11:04:04 2024, max compression
+gzip compressed data, was "stac_fastapi_api-3.0.0a2.tar", last modified: Fri May 31 15:25:31 2024, max compression
```

## Comparing `stac_fastapi_api-3.0.0a1.tar` & `stac_fastapi_api-3.0.0a2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:04.536846 stac_fastapi_api-3.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-22 11:04:04.536846 stac_fastapi_api-3.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 11:04:04.536846 stac_fastapi_api-3.0.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:04.532846 stac_fastapi_api-3.0.0a1/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:04.536846 stac_fastapi_api-3.0.0a1/stac_fastapi/api/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/app.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/openapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/stac_fastapi/api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:04.536846 stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-22 11:04:04.000000 stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-22 11:04:04.000000 stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:04:04.000000 stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:04:04.000000 stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-22 11:04:04.000000 stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:04:04.000000 stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:04.536846 stac_fastapi_api-3.0.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/tests/test_app_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-22 11:03:45.000000 stac_fastapi_api-3.0.0a1/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:25:31.196750 stac_fastapi_api-3.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-31 15:25:31.196750 stac_fastapi_api-3.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-31 15:25:31.196750 stac_fastapi_api-3.0.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:25:31.188750 stac_fastapi_api-3.0.0a2/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:25:31.192750 stac_fastapi_api-3.0.0a2/stac_fastapi/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/stac_fastapi/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16978 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/stac_fastapi/api/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/stac_fastapi/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/stac_fastapi/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/stac_fastapi/api/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4563 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/stac_fastapi/api/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3134 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/stac_fastapi/api/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/stac_fastapi/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/stac_fastapi/api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:25:31.192750 stac_fastapi_api-3.0.0a2/stac_fastapi.api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-31 15:25:31.000000 stac_fastapi_api-3.0.0a2/stac_fastapi.api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-31 15:25:31.000000 stac_fastapi_api-3.0.0a2/stac_fastapi.api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:25:31.000000 stac_fastapi_api-3.0.0a2/stac_fastapi.api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:25:31.000000 stac_fastapi_api-3.0.0a2/stac_fastapi.api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-31 15:25:31.000000 stac_fastapi_api-3.0.0a2/stac_fastapi.api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 15:25:31.000000 stac_fastapi_api-3.0.0a2/stac_fastapi.api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:25:31.192750 stac_fastapi_api-3.0.0a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/tests/test_app_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-31 15:25:09.000000 stac_fastapi_api-3.0.0a2/tests/test_models.py
```

### Comparing `stac_fastapi_api-3.0.0a1/PKG-INFO` & `stac_fastapi_api-3.0.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
-Version: 3.0.0a1
+Version: 3.0.0a2
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac_fastapi_api-3.0.0a1/setup.py` & `stac_fastapi_api-3.0.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a1/stac_fastapi/api/app.py` & `stac_fastapi_api-3.0.0a2/stac_fastapi/api/app.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a1/stac_fastapi/api/config.py` & `stac_fastapi_api-3.0.0a2/stac_fastapi/api/config.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a1/stac_fastapi/api/errors.py` & `stac_fastapi_api-3.0.0a2/stac_fastapi/api/errors.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a1/stac_fastapi/api/middleware.py` & `stac_fastapi_api-3.0.0a2/stac_fastapi/api/middleware.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a1/stac_fastapi/api/models.py` & `stac_fastapi_api-3.0.0a2/stac_fastapi/api/models.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a1/stac_fastapi/api/openapi.py` & `stac_fastapi_api-3.0.0a2/stac_fastapi/api/openapi.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a1/stac_fastapi/api/routes.py` & `stac_fastapi_api-3.0.0a2/stac_fastapi/api/routes.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/PKG-INFO` & `stac_fastapi_api-3.0.0a2/stac_fastapi.api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.api
-Version: 3.0.0a1
+Version: 3.0.0a2
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac_fastapi_api-3.0.0a1/stac_fastapi.api.egg-info/SOURCES.txt` & `stac_fastapi_api-3.0.0a2/stac_fastapi.api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a1/tests/test_api.py` & `stac_fastapi_api-3.0.0a2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a1/tests/test_app.py` & `stac_fastapi_api-3.0.0a2/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a1/tests/test_app_prefix.py` & `stac_fastapi_api-3.0.0a2/tests/test_app_prefix.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a1/tests/test_middleware.py` & `stac_fastapi_api-3.0.0a2/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_api-3.0.0a1/tests/test_models.py` & `stac_fastapi_api-3.0.0a2/tests/test_models.py`

 * *Files identical despite different names*

