# Comparing `tmp/nortech-0.2.2.tar.gz` & `tmp/nortech-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nortech-0.2.2.tar", max compression
+gzip compressed data, was "nortech-0.2.3.tar", max compression
```

## Comparing `nortech-0.2.2.tar` & `nortech-0.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11357 2023-11-28 16:36:24.114062 nortech-0.2.2/LICENSE
--rw-r--r--   0        0        0     6241 2024-05-31 10:24:25.877447 nortech-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-12-03 13:52:48.203137 nortech-0.2.2/nortech/__init__.py
--rw-r--r--   0        0        0      264 2023-12-04 16:14:37.723473 nortech-0.2.2/nortech/datatools/__init__.py
--rw-r--r--   0        0        0        0 2023-12-03 14:29:51.232877 nortech-0.2.2/nortech/datatools/handlers/__init__.py
--rw-r--r--   0        0        0     2851 2024-05-31 09:47:25.221601 nortech-0.2.2/nortech/datatools/handlers/pandas.py
--rw-r--r--   0        0        0     5969 2023-12-04 17:38:36.825041 nortech-0.2.2/nortech/datatools/handlers/polars.py
--rw-r--r--   0        0        0     5471 2024-05-31 10:11:10.216887 nortech-0.2.2/nortech/datatools/repositories/S3.py
--rw-r--r--   0        0        0        0 2023-12-03 14:29:43.016646 nortech-0.2.2/nortech/datatools/repositories/__init__.py
--rw-r--r--   0        0        0        0 2023-12-03 14:29:26.578689 nortech-0.2.2/nortech/datatools/services/__init__.py
--rw-r--r--   0        0        0      609 2023-12-04 16:16:14.399442 nortech-0.2.2/nortech/datatools/services/config.py
--rw-r--r--   0        0        0        0 2023-12-03 14:10:29.817430 nortech-0.2.2/nortech/datatools/values/__init__.py
--rw-r--r--   0        0        0      347 2023-12-03 19:51:26.287501 nortech-0.2.2/nortech/datatools/values/errors.py
--rw-r--r--   0        0        0     2239 2024-05-31 10:21:14.751804 nortech-0.2.2/nortech/datatools/values/signals.py
--rw-r--r--   0        0        0      510 2024-05-29 12:39:38.725679 nortech-0.2.2/nortech/derivers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.205309 nortech-0.2.2/nortech/derivers/gateways/__init__.py
--rw-r--r--   0        0        0     2755 2024-05-29 15:03:27.253913 nortech-0.2.2/nortech/derivers/gateways/customer_api.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.206598 nortech-0.2.2/nortech/derivers/handlers/__init__.py
--rw-r--r--   0        0        0     5637 2024-05-29 13:44:02.676884 nortech-0.2.2/nortech/derivers/handlers/deriver.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.203764 nortech-0.2.2/nortech/derivers/repositories/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.201516 nortech-0.2.2/nortech/derivers/services/__init__.py
--rw-r--r--   0        0        0      131 2024-05-29 09:45:01.201714 nortech-0.2.2/nortech/derivers/services/logger.py
--rw-r--r--   0        0        0     5431 2024-05-29 10:26:08.670198 nortech-0.2.2/nortech/derivers/services/operators.py
--rw-r--r--   0        0        0      276 2024-05-29 10:47:12.127163 nortech-0.2.2/nortech/derivers/services/physical_units.py
--rw-r--r--   0        0        0     3564 2024-05-29 12:58:49.727767 nortech-0.2.2/nortech/derivers/services/schema.py
--rw-r--r--   0        0        0     2288 2024-05-29 09:46:25.353623 nortech-0.2.2/nortech/derivers/services/visualize.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.197564 nortech-0.2.2/nortech/derivers/values/__init__.py
--rw-r--r--   0        0        0     1948 2024-05-29 11:12:50.690657 nortech-0.2.2/nortech/derivers/values/instance.py
--rw-r--r--   0        0        0     3918 2024-05-29 09:46:25.353139 nortech-0.2.2/nortech/derivers/values/physical_units.py
--rw-r--r--   0        0        0      351 2024-05-29 09:45:01.197672 nortech-0.2.2/nortech/derivers/values/physical_units_schema.py
--rw-r--r--   0        0        0     6007 2024-05-29 09:46:25.349173 nortech-0.2.2/nortech/derivers/values/schema.py
--rw-r--r--   0        0        0      825 2024-05-31 10:24:38.827259 nortech-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     7290 1970-01-01 00:00:00.000000 nortech-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-28 16:36:24.114062 nortech-0.2.3/LICENSE
+-rw-r--r--   0        0        0     6241 2024-05-31 10:24:25.877447 nortech-0.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-12-03 13:52:48.203137 nortech-0.2.3/nortech/__init__.py
+-rw-r--r--   0        0        0      264 2023-12-04 16:14:37.723473 nortech-0.2.3/nortech/datatools/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:29:51.232877 nortech-0.2.3/nortech/datatools/handlers/__init__.py
+-rw-r--r--   0        0        0     2851 2024-05-31 09:47:25.221601 nortech-0.2.3/nortech/datatools/handlers/pandas.py
+-rw-r--r--   0        0        0     5969 2023-12-04 17:38:36.825041 nortech-0.2.3/nortech/datatools/handlers/polars.py
+-rw-r--r--   0        0        0     5471 2024-05-31 10:11:10.216887 nortech-0.2.3/nortech/datatools/repositories/S3.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:29:43.016646 nortech-0.2.3/nortech/datatools/repositories/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:29:26.578689 nortech-0.2.3/nortech/datatools/services/__init__.py
+-rw-r--r--   0        0        0      609 2023-12-04 16:16:14.399442 nortech-0.2.3/nortech/datatools/services/config.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:10:29.817430 nortech-0.2.3/nortech/datatools/values/__init__.py
+-rw-r--r--   0        0        0      537 2024-05-31 10:26:38.885861 nortech-0.2.3/nortech/datatools/values/errors.py
+-rw-r--r--   0        0        0     2342 2024-05-31 10:27:03.038918 nortech-0.2.3/nortech/datatools/values/signals.py
+-rw-r--r--   0        0        0      510 2024-05-29 12:39:38.725679 nortech-0.2.3/nortech/derivers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.205309 nortech-0.2.3/nortech/derivers/gateways/__init__.py
+-rw-r--r--   0        0        0     2755 2024-05-29 15:03:27.253913 nortech-0.2.3/nortech/derivers/gateways/customer_api.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.206598 nortech-0.2.3/nortech/derivers/handlers/__init__.py
+-rw-r--r--   0        0        0     5637 2024-05-29 13:44:02.676884 nortech-0.2.3/nortech/derivers/handlers/deriver.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.203764 nortech-0.2.3/nortech/derivers/repositories/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.201516 nortech-0.2.3/nortech/derivers/services/__init__.py
+-rw-r--r--   0        0        0      131 2024-05-29 09:45:01.201714 nortech-0.2.3/nortech/derivers/services/logger.py
+-rw-r--r--   0        0        0     5431 2024-05-29 10:26:08.670198 nortech-0.2.3/nortech/derivers/services/operators.py
+-rw-r--r--   0        0        0      276 2024-05-29 10:47:12.127163 nortech-0.2.3/nortech/derivers/services/physical_units.py
+-rw-r--r--   0        0        0     3564 2024-05-29 12:58:49.727767 nortech-0.2.3/nortech/derivers/services/schema.py
+-rw-r--r--   0        0        0     2288 2024-05-29 09:46:25.353623 nortech-0.2.3/nortech/derivers/services/visualize.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.197564 nortech-0.2.3/nortech/derivers/values/__init__.py
+-rw-r--r--   0        0        0     1948 2024-05-29 11:12:50.690657 nortech-0.2.3/nortech/derivers/values/instance.py
+-rw-r--r--   0        0        0     3918 2024-05-29 09:46:25.353139 nortech-0.2.3/nortech/derivers/values/physical_units.py
+-rw-r--r--   0        0        0      351 2024-05-29 09:45:01.197672 nortech-0.2.3/nortech/derivers/values/physical_units_schema.py
+-rw-r--r--   0        0        0     6007 2024-05-29 09:46:25.349173 nortech-0.2.3/nortech/derivers/values/schema.py
+-rw-r--r--   0        0        0      825 2024-05-31 10:27:30.989485 nortech-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     7290 1970-01-01 00:00:00.000000 nortech-0.2.3/PKG-INFO
```

### Comparing `nortech-0.2.2/LICENSE` & `nortech-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nortech-0.2.2/README.md` & `nortech-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `nortech-0.2.2/nortech/datatools/handlers/pandas.py` & `nortech-0.2.3/nortech/datatools/handlers/pandas.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.2/nortech/datatools/handlers/polars.py` & `nortech-0.2.3/nortech/datatools/handlers/polars.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.2/nortech/datatools/repositories/S3.py` & `nortech-0.2.3/nortech/datatools/repositories/S3.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.2/nortech/datatools/services/config.py` & `nortech-0.2.3/nortech/datatools/services/config.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.2/nortech/datatools/values/signals.py` & `nortech-0.2.3/nortech/datatools/values/signals.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,32 @@
 from datetime import datetime
 from json import loads
 from typing import Dict, List
 
 from pydantic import BaseModel
 from tzlocal import get_localzone
 
-from nortech.datatools.values.errors import InvalidTimeWindow
+from nortech.datatools.values.errors import InvalidTimeWindow, InvalidTimeZone
 
 
 @dataclass
 class TimeWindow:
     start: datetime
     end: datetime
 
     def __post_init__(self):
         if self.start.tzinfo is None:
             self.start = self.start.replace(tzinfo=get_localzone())
 
         if self.end.tzinfo is None:
             self.end = self.end.replace(tzinfo=get_localzone())
 
+        if self.start.tzinfo != self.end.tzinfo:
+            raise InvalidTimeZone()
+
         if self.end < self.start:
             raise InvalidTimeWindow()
 
 
 @dataclass
 class SignalConfig:
     column_name: str
```

### Comparing `nortech-0.2.2/nortech/derivers/gateways/customer_api.py` & `nortech-0.2.3/nortech/derivers/gateways/customer_api.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.2/nortech/derivers/handlers/deriver.py` & `nortech-0.2.3/nortech/derivers/handlers/deriver.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.2/nortech/derivers/services/operators.py` & `nortech-0.2.3/nortech/derivers/services/operators.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.2/nortech/derivers/services/schema.py` & `nortech-0.2.3/nortech/derivers/services/schema.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.2/nortech/derivers/services/visualize.py` & `nortech-0.2.3/nortech/derivers/services/visualize.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.2/nortech/derivers/values/instance.py` & `nortech-0.2.3/nortech/derivers/values/instance.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.2/nortech/derivers/values/physical_units.py` & `nortech-0.2.3/nortech/derivers/values/physical_units.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.2/nortech/derivers/values/schema.py` & `nortech-0.2.3/nortech/derivers/values/schema.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.2/pyproject.toml` & `nortech-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nortech"
-version = "0.2.2"
+version = "0.2.3"
 description = "The official Python library for Nortech AI"
 authors = ["Nortech AI <info@nortech.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://nortech.ai/"
 repository = "https://github.com/Nortech-ai/nortech-python"
```

### Comparing `nortech-0.2.2/PKG-INFO` & `nortech-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nortech
-Version: 0.2.2
+Version: 0.2.3
 Summary: The official Python library for Nortech AI
 Home-page: https://nortech.ai/
 License: Apache-2.0
 Author: Nortech AI
 Author-email: info@nortech.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

