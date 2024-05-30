# Comparing `tmp/ziptimezone-1.1.6.tar.gz` & `tmp/ziptimezone-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziptimezone-1.1.6.tar", max compression
+gzip compressed data, was "ziptimezone-1.1.7.tar", max compression
```

## Comparing `ziptimezone-1.1.6.tar` & `ziptimezone-1.1.7.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-1.1.6/LICENSE
--rw-r--r--   0        0        0      859 2024-05-28 10:19:03.496065 ziptimezone-1.1.6/pyproject.toml
--rw-r--r--   0        0        0     2010 2024-05-28 10:18:22.986628 ziptimezone-1.1.6/README.rst
--rw-r--r--   0        0        0     1395 2024-05-13 11:45:23.443070 ziptimezone-1.1.6/ziptimezone/__init__.py
--rw-r--r--   0        0        0     3598 2024-04-24 12:28:21.581939 ziptimezone-1.1.6/ziptimezone/batch_processor.py
--rw-r--r--   0        0        0     4325 2024-05-19 09:28:26.628819 ziptimezone-1.1.6/ziptimezone/core.py
--rw-r--r--   0        0        0     2780 2024-04-21 13:54:36.749759 ziptimezone-1.1.6/ziptimezone/data_manager.py
--rw-r--r--   0        0        0     1101 2024-04-21 13:54:36.749759 ziptimezone-1.1.6/ziptimezone/geocode.py
--rw-r--r--   0        0        0     1645 2024-04-21 13:54:36.749759 ziptimezone-1.1.6/ziptimezone/globals.py
--rw-r--r--   0        0        0     1874 2024-04-21 13:54:36.749759 ziptimezone-1.1.6/ziptimezone/mappings.py
--rw-r--r--   0        0        0     2722 1970-01-01 00:00:00.000000 ziptimezone-1.1.6/PKG-INFO
+-rw-r--r--   0        0        0        2 2024-04-20 11:29:25.216037 ziptimezone-1.1.7/LICENSE
+-rw-r--r--   0        0        0      874 2024-05-30 11:33:54.050795 ziptimezone-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2383 2024-05-30 22:03:54.865550 ziptimezone-1.1.7/README.rst
+-rw-r--r--   0        0        0     1560 2024-05-30 22:11:50.060549 ziptimezone-1.1.7/ziptimezone/__init__.py
+-rw-r--r--   0        0        0     1921 2024-05-30 22:11:50.061666 ziptimezone-1.1.7/ziptimezone/addon.py
+-rw-r--r--   0        0        0     3598 2024-04-24 12:28:21.581939 ziptimezone-1.1.7/ziptimezone/batch_processor.py
+-rw-r--r--   0        0        0     4325 2024-05-19 09:28:26.628819 ziptimezone-1.1.7/ziptimezone/core.py
+-rw-r--r--   0        0        0     2780 2024-04-21 13:54:36.749759 ziptimezone-1.1.7/ziptimezone/data_manager.py
+-rw-r--r--   0        0        0     1101 2024-04-21 13:54:36.749759 ziptimezone-1.1.7/ziptimezone/geocode.py
+-rw-r--r--   0        0        0     1645 2024-04-21 13:54:36.749759 ziptimezone-1.1.7/ziptimezone/globals.py
+-rw-r--r--   0        0        0     1874 2024-04-21 13:54:36.749759 ziptimezone-1.1.7/ziptimezone/mappings.py
+-rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 ziptimezone-1.1.7/PKG-INFO
```

### Comparing `ziptimezone-1.1.6/pyproject.toml` & `ziptimezone-1.1.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [tool.poetry]
 name = "ziptimezone"
-version = "1.1.6"
+version = "1.1.7"
 description = "A package to convert ZIP codes to time zones and get geographic coordinates."
 readme = "README.rst"
 authors = ["Manjunath Bettadapura <manjunathbettadapura412@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.9, <4.0"
 requests = "^2.31.0"
 timezonefinder = ">=6.1.5, <=6.5.0"
 python-dateutil = "^2.8"
 pytz="^2024.1"
+astral="^3.2"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `ziptimezone-1.1.6/ziptimezone/__init__.py` & `ziptimezone-1.1.7/ziptimezone/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,22 +15,30 @@
 # Get the timezone of a ZIP code
 timezone = get_timezone_by_zip('85260')
 
 # Get the latitude and longitude of a ZIP code
 latitude, longitude = get_lat_long_for_zip('02138')
 """
 
-from .core import get_timezone_by_zip, get_lat_long_for_zip, calculate_time_difference
+from .core import (
+    get_timezone_by_zip,
+    get_lat_long_for_zip,
+    calculate_time_difference,
+    get_timezone_without_map_by_zip,
+)
 from .data_manager import refresh_data_if_needed
 from .batch_processor import get_timezone_for_many_zips, get_lat_long_for_many_zips
+from .addon import get_sunrise_sunset
 
 ##from .mappings import map_timezone_to_region
 # from .geocode import get_lat_long_for_zip
 
 __all__ = [
     "get_lat_long_for_zip",
     "get_timezone_by_zip",
+    "get_timezone_without_map_by_zip",
     "calculate_time_difference",
     "refresh_data_if_needed",
     "get_timezone_for_many_zips",
     "get_lat_long_for_many_zips",
+    "get_sunrise_sunset",
 ]
```

### Comparing `ziptimezone-1.1.6/ziptimezone/batch_processor.py` & `ziptimezone-1.1.7/ziptimezone/batch_processor.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.6/ziptimezone/core.py` & `ziptimezone-1.1.7/ziptimezone/core.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.6/ziptimezone/data_manager.py` & `ziptimezone-1.1.7/ziptimezone/data_manager.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.6/ziptimezone/geocode.py` & `ziptimezone-1.1.7/ziptimezone/geocode.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.6/ziptimezone/globals.py` & `ziptimezone-1.1.7/ziptimezone/globals.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.6/ziptimezone/mappings.py` & `ziptimezone-1.1.7/ziptimezone/mappings.py`

 * *Files identical despite different names*

### Comparing `ziptimezone-1.1.6/PKG-INFO` & `ziptimezone-1.1.7/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: ziptimezone
-Version: 1.1.6
+Version: 1.1.7
 Summary: A package to convert ZIP codes to time zones and get geographic coordinates.
 License: MIT
 Author: Manjunath Bettadapura
 Author-email: manjunathbettadapura412@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: astral (>=3.2,<4.0)
 Requires-Dist: python-dateutil (>=2.8,<3.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: timezonefinder (>=6.1.5,<=6.5.0)
 Description-Content-Type: text/x-rst
 
 ==============
-timezonefinder
+ziptimezone
 ==============
 
 
 ..
     Note: can't include the badges file from the docs here, as it won't render on PyPI -> sync manually
 
 .. image:: https://readthedocs.org/projects/ziptimezone/badge/?version=latest
@@ -68,16 +69,23 @@
     # returns 'Eastern' the timezone has been reduced to the more popular zones 
     # for United States Regions
     zpt.get_timezone_by_zip('02138') 
 
     # returns a dictionary, {'02138': 'Eastern', '85260': 'Mountain'}
     zpt.get_timezone_for_many_zips(['02138', '85260']) 
 
-    # returns a a string, '02138 is ahead of 72201 by 1.00 hours."}
+    # returns a string, '02138 is ahead of 72201 by 1.00 hours."}
     zpt.calculate_time_difference(['02138', '72201']) 
 
+    # returns a dictionary, for 5/30/24 {'sunrise_time': '05:11:13', 'sunset_time': '20:13:31'}
+    today_sun_times = get_sunrise_sunset("02138")
+
+    # Get sunrise and sunset times for ZIP code 02138 on July 4, 2024
+    # will return {'sunrise_time': '05:13:42', 'sunset_time': '20:24:10'}
+    july4_sun_times = get_sunrise_sunset("02138", datetime(2024, 7, 4).date())
+
 For more refer to the `Documentation <https://ziptimezone.readthedocs.io/en/latest/>`__.
 
 Also check:
 
 `PyPI <https://pypi.python.org/pypi/ziptimezone/>`__
```

