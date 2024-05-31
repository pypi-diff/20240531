# Comparing `tmp/dinamis_sdk-0.1.8.tar.gz` & `tmp/dinamis_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinamis_sdk-0.1.8.tar", last modified: Tue May 21 18:17:20 2024, max compression
+gzip compressed data, was "dinamis_sdk-0.1.9.tar", last modified: Tue May 21 18:41:43 2024, max compression
```

## Comparing `dinamis_sdk-0.1.8.tar` & `dinamis_sdk-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:17:20.313818 dinamis_sdk-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)    11340 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      391 2024-05-21 18:17:20.313818 dinamis_sdk-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      950 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:17:20.305818 dinamis_sdk-0.1.8/dinamis_sdk/
--rw-rw-rw-   0 root         (0) root         (0)      284 2024-05-21 18:04:01.000000 dinamis_sdk-0.1.8/dinamis_sdk/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8903 2024-05-21 18:09:08.000000 dinamis_sdk-0.1.8/dinamis_sdk/auth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:17:20.309818 dinamis_sdk-0.1.8/dinamis_sdk/examples/
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/dinamis_sdk/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      920 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/dinamis_sdk/examples/pyotb_ndvi_loss.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/dinamis_sdk/examples/pyotb_toa_mosaic.py
--rw-rw-rw-   0 root         (0) root         (0)     1081 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/dinamis_sdk/examples/rio_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    17399 2024-05-21 18:04:02.000000 dinamis_sdk-0.1.8/dinamis_sdk/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     3156 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/dinamis_sdk/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:17:20.309818 dinamis_sdk-0.1.8/dinamis_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      391 2024-05-21 18:17:20.000000 dinamis_sdk-0.1.8/dinamis_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      518 2024-05-21 18:17:20.000000 dinamis_sdk-0.1.8/dinamis_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 18:17:20.000000 dinamis_sdk-0.1.8/dinamis_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 18:17:20.000000 dinamis_sdk-0.1.8/dinamis_sdk.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       80 2024-05-21 18:17:20.000000 dinamis_sdk-0.1.8/dinamis_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-05-21 18:17:20.000000 dinamis_sdk-0.1.8/dinamis_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 18:17:20.313818 dinamis_sdk-0.1.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      496 2024-05-21 17:56:59.000000 dinamis_sdk-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:17:20.309818 dinamis_sdk-0.1.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)      405 2024-05-21 18:09:08.000000 dinamis_sdk-0.1.8/tests/test_spot-6-7-drs.py
--rw-rw-rw-   0 root         (0) root         (0)      400 2024-05-21 18:09:08.000000 dinamis_sdk-0.1.8/tests/test_super-s2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:41:43.346722 dinamis_sdk-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)    11340 2024-05-21 14:43:50.000000 dinamis_sdk-0.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      367 2024-05-21 18:41:43.346722 dinamis_sdk-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      950 2024-05-21 14:43:50.000000 dinamis_sdk-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:41:43.342723 dinamis_sdk-0.1.9/dinamis_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      284 2024-05-21 18:04:28.000000 dinamis_sdk-0.1.9/dinamis_sdk/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8903 2024-05-21 18:10:07.000000 dinamis_sdk-0.1.9/dinamis_sdk/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:41:43.346722 dinamis_sdk-0.1.9/dinamis_sdk/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-05-21 14:43:50.000000 dinamis_sdk-0.1.9/dinamis_sdk/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      920 2024-05-21 14:43:50.000000 dinamis_sdk-0.1.9/dinamis_sdk/examples/pyotb_ndvi_loss.py
+-rw-rw-rw-   0 root         (0) root         (0)      595 2024-05-21 14:43:50.000000 dinamis_sdk-0.1.9/dinamis_sdk/examples/pyotb_toa_mosaic.py
+-rw-rw-rw-   0 root         (0) root         (0)     1081 2024-05-21 14:43:50.000000 dinamis_sdk-0.1.9/dinamis_sdk/examples/rio_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    17406 2024-05-21 18:20:25.000000 dinamis_sdk-0.1.9/dinamis_sdk/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2024-05-21 18:38:47.000000 dinamis_sdk-0.1.9/dinamis_sdk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:41:43.346722 dinamis_sdk-0.1.9/dinamis_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      367 2024-05-21 18:41:43.000000 dinamis_sdk-0.1.9/dinamis_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      518 2024-05-21 18:41:43.000000 dinamis_sdk-0.1.9/dinamis_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 18:41:43.000000 dinamis_sdk-0.1.9/dinamis_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 18:41:43.000000 dinamis_sdk-0.1.9/dinamis_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-21 18:41:43.000000 dinamis_sdk-0.1.9/dinamis_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-21 18:41:43.000000 dinamis_sdk-0.1.9/dinamis_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 18:41:43.346722 dinamis_sdk-0.1.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      480 2024-05-21 18:38:47.000000 dinamis_sdk-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 18:41:43.346722 dinamis_sdk-0.1.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      405 2024-05-21 18:10:07.000000 dinamis_sdk-0.1.9/tests/test_spot-6-7-drs.py
+-rw-rw-rw-   0 root         (0) root         (0)      525 2024-05-21 18:38:47.000000 dinamis_sdk-0.1.9/tests/test_super-s2.py
```

### Comparing `dinamis_sdk-0.1.8/LICENSE` & `dinamis_sdk-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dinamis_sdk-0.1.8/README.md` & `dinamis_sdk-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dinamis_sdk-0.1.8/dinamis_sdk/auth.py` & `dinamis_sdk-0.1.9/dinamis_sdk/auth.py`

 * *Files identical despite different names*

### Comparing `dinamis_sdk-0.1.8/dinamis_sdk/examples/pyotb_ndvi_loss.py` & `dinamis_sdk-0.1.9/dinamis_sdk/examples/pyotb_ndvi_loss.py`

 * *Files identical despite different names*

### Comparing `dinamis_sdk-0.1.8/dinamis_sdk/examples/pyotb_toa_mosaic.py` & `dinamis_sdk-0.1.9/dinamis_sdk/examples/pyotb_toa_mosaic.py`

 * *Files identical despite different names*

### Comparing `dinamis_sdk-0.1.8/dinamis_sdk/examples/rio_metadata.py` & `dinamis_sdk-0.1.9/dinamis_sdk/examples/rio_metadata.py`

 * *Files identical despite different names*

### Comparing `dinamis_sdk-0.1.8/dinamis_sdk/s3.py` & `dinamis_sdk-0.1.9/dinamis_sdk/s3.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
 
     """
     if copy:
         item_collection = item_collection.clone()
     urls = [
         asset.href
         for item in item_collection
-        for asset in item.values()
+        for asset in item.assets.values()
     ]
     signed_urls = sign_urls(urls=urls)
     for item in item_collection:
         for key, asset in item.assets.items():
             item.assets[key].href = signed_urls[asset.href]
     return item_collection
```

### Comparing `dinamis_sdk-0.1.8/dinamis_sdk/utils.py` & `dinamis_sdk-0.1.9/dinamis_sdk/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,34 +5,34 @@
 import appdirs
 from pydantic import BaseModel  # pylint: disable = no-name-in-module
 import requests
 
 logging.basicConfig(level=os.environ.get("LOGLEVEL") or "INFO")
 log = logging.getLogger("dinamis_sdk")
 
-def _get_seconds(env_var_name: str) -> int:
+
+def _get_seconds(env_var_name: str, default: int) -> int:
     val = os.environ.get(env_var_name)
     if val:
         if val.isdigit():
-            return int(val)
-    return None
+            log.info(
+                "Using %s = %s seconds",
+                env_var_name,
+                val
+            )           
+        return int(val)
+    return default
+
 
 # Signed TTL margin default to 1800 seconds (30 minutes), or env. var.
-if (ttl_margin_from_env := _get_seconds("DINAMIS_SDK_TTL_MARGIN")):
-    log.info(
-        "Setting TTL margin from environment variable to %s seconds",
-        ttl_margin_from_env
-    )
-SIGNED_URL_TTL_MARGIN = ttl_margin_from_env or 1800
-
-if (SIGNED_URL_DURATION_SECONDS := _get_seconds("DINAMIS_SDK_DURATION_SECONDS")):
-    log.info(
-        "Setting duration seconds from environment variable to %s seconds",
-        SIGNED_URL_DURATION_SECONDS
-    )
+SIGNED_URL_TTL_MARGIN = _get_seconds("DINAMIS_SDK_TTL_MARGIN", 1800)
+SIGNED_URL_DURATION_SECONDS = _get_seconds(
+    "DINAMIS_SDK_DURATION_SECONDS", 
+    None
+)
 
 MAX_URLS = 64
 S3_STORAGE_DOMAIN = "meso.umontpellier.fr"
 S3_SIGNING_ENDPOINT = \
     "https://s3-signing-cdos.apps.okd.crocc.meso.umontpellier.fr/"
 
 CFG_PTH = appdirs.user_config_dir(appname='dinamis_sdk_auth')
```

### Comparing `dinamis_sdk-0.1.8/dinamis_sdk.egg-info/SOURCES.txt` & `dinamis_sdk-0.1.9/dinamis_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

