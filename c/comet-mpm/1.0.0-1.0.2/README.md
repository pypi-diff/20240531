# Comparing `tmp/comet_mpm-1.0.0.tar.gz` & `tmp/comet_mpm-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comet_mpm-1.0.0.tar", last modified: Wed May 29 09:27:15 2024, max compression
+gzip compressed data, was "comet_mpm-1.0.2.tar", last modified: Fri May 31 13:10:29 2024, max compression
```

## Comparing `comet_mpm-1.0.0.tar` & `comet_mpm-1.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.310628 comet_mpm-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/PACKAGE.md
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-29 09:27:15.310628 comet_mpm-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:27:15.310628 comet_mpm-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.298628 comet_mpm-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.306628 comet_mpm-1.0.0/src/comet_mpm/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.306628 comet_mpm-1.0.0/src/comet_mpm/_json/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/_json/numpy_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.306628 comet_mpm-1.0.0/src/comet_mpm/api_key/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/api_key/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/api_key/base64_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/api_key/comet_api_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.306628 comet_mpm-1.0.0/src/comet_mpm/aws_lambda/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/aws_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/aws_lambda/lambda_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/batch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    20451 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/comet_mpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/connection_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/data_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/dataset_upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.306628 comet_mpm-1.0.0/src/comet_mpm/events/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/events/base_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/events/events_from_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/events/label_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/events/prediction_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/logging_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/optional_update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.306628 comet_mpm-1.0.0/src/comet_mpm/sender/
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/sender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/sender/asyncio_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/sender/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/sender/thread_sender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/server_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-29 09:27:11.000000 comet_mpm-1.0.0/src/comet_mpm/settings_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:27:15.306628 comet_mpm-1.0.0/src/comet_mpm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-29 09:27:15.000000 comet_mpm-1.0.0/src/comet_mpm.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:10:29.057069 comet_mpm-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/PACKAGE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-31 13:10:29.057069 comet_mpm-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:10:29.057069 comet_mpm-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:10:29.049069 comet_mpm-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:10:29.057069 comet_mpm-1.0.2/src/comet_mpm/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:10:29.057069 comet_mpm-1.0.2/src/comet_mpm/_json/
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/_json/numpy_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:10:29.057069 comet_mpm-1.0.2/src/comet_mpm/api_key/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/api_key/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/api_key/base64_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/api_key/comet_api_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:10:29.057069 comet_mpm-1.0.2/src/comet_mpm/aws_lambda/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/aws_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/aws_lambda/lambda_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/batch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20451 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/comet_mpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5969 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/connection_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/data_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/dataset_upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:10:29.057069 comet_mpm-1.0.2/src/comet_mpm/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/events/base_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/events/events_from_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/events/label_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/events/prediction_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/logging_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/optional_update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:10:29.057069 comet_mpm-1.0.2/src/comet_mpm/sender/
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/sender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/sender/asyncio_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/sender/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8380 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/sender/thread_sender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/server_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-31 13:10:24.000000 comet_mpm-1.0.2/src/comet_mpm/settings_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:10:29.057069 comet_mpm-1.0.2/src/comet_mpm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-31 13:10:29.000000 comet_mpm-1.0.2/src/comet_mpm.egg-info/SOURCES.txt
```

### Comparing `comet_mpm-1.0.0/MANIFEST.in` & `comet_mpm-1.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/PKG-INFO` & `comet_mpm-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet_mpm
-Version: 1.0.0
+Version: 1.0.2
 Summary: Comet MPM SDK
 Home-page: https://www.comet.ml
 Author: Comet ML Inc.
 Author-email: mail@comet.ml
 License: Proprietary
 Keywords: comet_mpm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `comet_mpm-1.0.0/setup.py` & `comet_mpm-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,11 +52,11 @@
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="comet_mpm",
     name="comet_mpm",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://www.comet.ml",
-    version="1.0.0",
+    version="1.0.2",
     zip_safe=False,
     license="Proprietary",
 )
```

### Comparing `comet_mpm-1.0.0/src/comet_mpm/__init__.py` & `comet_mpm-1.0.2/src/comet_mpm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 #  Copyright (C) 2021 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
 __author__ = """Comet ML Inc."""
 __email__ = "mail@comet.ml"
-__version__ = "1.0.0"
+__version__ = "1.0.2"
 __all__ = ["CometMPM"]
 
 from ._logging import _setup_comet_mpm_logging
 from .comet_mpm import CometMPM
 
 _setup_comet_mpm_logging()
```

### Comparing `comet_mpm-1.0.0/src/comet_mpm/_json/__init__.py` & `comet_mpm-1.0.2/src/comet_mpm/_json/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/_json/numpy_encoder.py` & `comet_mpm-1.0.2/src/comet_mpm/_json/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/_logging.py` & `comet_mpm-1.0.2/src/comet_mpm/_logging.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/api_key/__init__.py` & `comet_mpm-1.0.2/src/comet_mpm/api_key/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/api_key/base64_helper.py` & `comet_mpm-1.0.2/src/comet_mpm/api_key/base64_helper.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/api_key/comet_api_key.py` & `comet_mpm-1.0.2/src/comet_mpm/api_key/comet_api_key.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/aws_lambda/__init__.py` & `comet_mpm-1.0.2/src/comet_mpm/aws_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/aws_lambda/lambda_helpers.py` & `comet_mpm-1.0.2/src/comet_mpm/aws_lambda/lambda_helpers.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/batch_utils.py` & `comet_mpm-1.0.2/src/comet_mpm/batch_utils.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/cli.py` & `comet_mpm-1.0.2/src/comet_mpm/cli.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/comet_mpm.py` & `comet_mpm-1.0.2/src/comet_mpm/comet_mpm.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/connection.py` & `comet_mpm-1.0.2/src/comet_mpm/connection.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/connection_helpers.py` & `comet_mpm-1.0.2/src/comet_mpm/connection_helpers.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/constants.py` & `comet_mpm-1.0.2/src/comet_mpm/constants.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/data_series.py` & `comet_mpm-1.0.2/src/comet_mpm/data_series.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/dataset_upload_helpers.py` & `comet_mpm-1.0.2/src/comet_mpm/dataset_upload_helpers.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/environment.py` & `comet_mpm-1.0.2/src/comet_mpm/environment.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/events/__init__.py` & `comet_mpm-1.0.2/src/comet_mpm/events/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/events/base_event.py` & `comet_mpm-1.0.2/src/comet_mpm/events/base_event.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/events/events_from_dataframe.py` & `comet_mpm-1.0.2/src/comet_mpm/events/events_from_dataframe.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/events/label_event.py` & `comet_mpm-1.0.2/src/comet_mpm/events/label_event.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/events/prediction_event.py` & `comet_mpm-1.0.2/src/comet_mpm/events/prediction_event.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/exceptions.py` & `comet_mpm-1.0.2/src/comet_mpm/exceptions.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/logging_messages.py` & `comet_mpm-1.0.2/src/comet_mpm/logging_messages.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/optional_update.py` & `comet_mpm-1.0.2/src/comet_mpm/optional_update.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/sender/__init__.py` & `comet_mpm-1.0.2/src/comet_mpm/sender/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/sender/asyncio_sender.py` & `comet_mpm-1.0.2/src/comet_mpm/sender/asyncio_sender.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/sender/base.py` & `comet_mpm-1.0.2/src/comet_mpm/sender/base.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/sender/thread_sender.py` & `comet_mpm-1.0.2/src/comet_mpm/sender/thread_sender.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/server_address.py` & `comet_mpm-1.0.2/src/comet_mpm/server_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,11 +44,11 @@
             return NotImplemented
         return self.api_path == other.api_path
 
     def batch_endpoint_url(self) -> str:
         return urljoin(self._api_full_path, "events/batch")
 
     def labels_endpoint_url(self) -> str:
-        return urljoin(self._api_full_path, "labels")
+        return urljoin(self._api_full_path, "labels/batch")
 
     def is_alive_endpoint_url(self) -> str:
         return urljoin(self.base_url, "isAlive/ping")
```

### Comparing `comet_mpm-1.0.0/src/comet_mpm/settings.py` & `comet_mpm-1.0.2/src/comet_mpm/settings.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm/settings_helper.py` & `comet_mpm-1.0.2/src/comet_mpm/settings_helper.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-1.0.0/src/comet_mpm.egg-info/SOURCES.txt` & `comet_mpm-1.0.2/src/comet_mpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

