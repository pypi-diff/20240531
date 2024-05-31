# Comparing `tmp/nortech-0.2.1.tar.gz` & `tmp/nortech-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nortech-0.2.1.tar", max compression
+gzip compressed data, was "nortech-0.2.2.tar", max compression
```

## Comparing `nortech-0.2.1.tar` & `nortech-0.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11357 2023-11-28 16:36:24.114062 nortech-0.2.1/LICENSE
--rw-r--r--   0        0        0     6228 2023-12-04 14:04:21.033886 nortech-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-12-03 13:52:48.203137 nortech-0.2.1/nortech/__init__.py
--rw-r--r--   0        0        0      264 2023-12-04 16:14:37.723473 nortech-0.2.1/nortech/datatools/__init__.py
--rw-r--r--   0        0        0        0 2023-12-03 14:29:51.232877 nortech-0.2.1/nortech/datatools/handlers/__init__.py
--rw-r--r--   0        0        0     2828 2023-12-04 17:38:39.495516 nortech-0.2.1/nortech/datatools/handlers/pandas.py
--rw-r--r--   0        0        0     5969 2023-12-04 17:38:36.825041 nortech-0.2.1/nortech/datatools/handlers/polars.py
--rw-r--r--   0        0        0     5200 2023-12-04 16:16:06.875409 nortech-0.2.1/nortech/datatools/repositories/S3.py
--rw-r--r--   0        0        0        0 2023-12-03 14:29:43.016646 nortech-0.2.1/nortech/datatools/repositories/__init__.py
--rw-r--r--   0        0        0        0 2023-12-03 14:29:26.578689 nortech-0.2.1/nortech/datatools/services/__init__.py
--rw-r--r--   0        0        0      609 2023-12-04 16:16:14.399442 nortech-0.2.1/nortech/datatools/services/config.py
--rw-r--r--   0        0        0        0 2023-12-03 14:10:29.817430 nortech-0.2.1/nortech/datatools/values/__init__.py
--rw-r--r--   0        0        0      347 2023-12-03 19:51:26.287501 nortech-0.2.1/nortech/datatools/values/errors.py
--rw-r--r--   0        0        0     2159 2023-12-03 19:51:44.164402 nortech-0.2.1/nortech/datatools/values/signals.py
--rw-r--r--   0        0        0      510 2024-05-29 12:39:38.725679 nortech-0.2.1/nortech/derivers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.205309 nortech-0.2.1/nortech/derivers/gateways/__init__.py
--rw-r--r--   0        0        0     2755 2024-05-29 14:21:14.243508 nortech-0.2.1/nortech/derivers/gateways/customer_api.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.206598 nortech-0.2.1/nortech/derivers/handlers/__init__.py
--rw-r--r--   0        0        0     5637 2024-05-29 13:44:02.676884 nortech-0.2.1/nortech/derivers/handlers/deriver.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.203764 nortech-0.2.1/nortech/derivers/repositories/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.201516 nortech-0.2.1/nortech/derivers/services/__init__.py
--rw-r--r--   0        0        0      131 2024-05-29 09:45:01.201714 nortech-0.2.1/nortech/derivers/services/logger.py
--rw-r--r--   0        0        0     5431 2024-05-29 10:26:08.670198 nortech-0.2.1/nortech/derivers/services/operators.py
--rw-r--r--   0        0        0      276 2024-05-29 10:47:12.127163 nortech-0.2.1/nortech/derivers/services/physical_units.py
--rw-r--r--   0        0        0     3564 2024-05-29 12:58:49.727767 nortech-0.2.1/nortech/derivers/services/schema.py
--rw-r--r--   0        0        0     2288 2024-05-29 09:46:25.353623 nortech-0.2.1/nortech/derivers/services/visualize.py
--rw-r--r--   0        0        0        0 2024-05-29 09:45:01.197564 nortech-0.2.1/nortech/derivers/values/__init__.py
--rw-r--r--   0        0        0     1948 2024-05-29 11:12:50.690657 nortech-0.2.1/nortech/derivers/values/instance.py
--rw-r--r--   0        0        0     3918 2024-05-29 09:46:25.353139 nortech-0.2.1/nortech/derivers/values/physical_units.py
--rw-r--r--   0        0        0      351 2024-05-29 09:45:01.197672 nortech-0.2.1/nortech/derivers/values/physical_units_schema.py
--rw-r--r--   0        0        0     6007 2024-05-29 09:46:25.349173 nortech-0.2.1/nortech/derivers/values/schema.py
--rw-r--r--   0        0        0      789 2024-05-29 14:21:38.335624 nortech-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     7241 1970-01-01 00:00:00.000000 nortech-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-28 16:36:24.114062 nortech-0.2.2/LICENSE
+-rw-r--r--   0        0        0     6241 2024-05-31 10:24:25.877447 nortech-0.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-12-03 13:52:48.203137 nortech-0.2.2/nortech/__init__.py
+-rw-r--r--   0        0        0      264 2023-12-04 16:14:37.723473 nortech-0.2.2/nortech/datatools/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:29:51.232877 nortech-0.2.2/nortech/datatools/handlers/__init__.py
+-rw-r--r--   0        0        0     2851 2024-05-31 09:47:25.221601 nortech-0.2.2/nortech/datatools/handlers/pandas.py
+-rw-r--r--   0        0        0     5969 2023-12-04 17:38:36.825041 nortech-0.2.2/nortech/datatools/handlers/polars.py
+-rw-r--r--   0        0        0     5471 2024-05-31 10:11:10.216887 nortech-0.2.2/nortech/datatools/repositories/S3.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:29:43.016646 nortech-0.2.2/nortech/datatools/repositories/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:29:26.578689 nortech-0.2.2/nortech/datatools/services/__init__.py
+-rw-r--r--   0        0        0      609 2023-12-04 16:16:14.399442 nortech-0.2.2/nortech/datatools/services/config.py
+-rw-r--r--   0        0        0        0 2023-12-03 14:10:29.817430 nortech-0.2.2/nortech/datatools/values/__init__.py
+-rw-r--r--   0        0        0      347 2023-12-03 19:51:26.287501 nortech-0.2.2/nortech/datatools/values/errors.py
+-rw-r--r--   0        0        0     2239 2024-05-31 10:21:14.751804 nortech-0.2.2/nortech/datatools/values/signals.py
+-rw-r--r--   0        0        0      510 2024-05-29 12:39:38.725679 nortech-0.2.2/nortech/derivers/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.205309 nortech-0.2.2/nortech/derivers/gateways/__init__.py
+-rw-r--r--   0        0        0     2755 2024-05-29 15:03:27.253913 nortech-0.2.2/nortech/derivers/gateways/customer_api.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.206598 nortech-0.2.2/nortech/derivers/handlers/__init__.py
+-rw-r--r--   0        0        0     5637 2024-05-29 13:44:02.676884 nortech-0.2.2/nortech/derivers/handlers/deriver.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.203764 nortech-0.2.2/nortech/derivers/repositories/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.201516 nortech-0.2.2/nortech/derivers/services/__init__.py
+-rw-r--r--   0        0        0      131 2024-05-29 09:45:01.201714 nortech-0.2.2/nortech/derivers/services/logger.py
+-rw-r--r--   0        0        0     5431 2024-05-29 10:26:08.670198 nortech-0.2.2/nortech/derivers/services/operators.py
+-rw-r--r--   0        0        0      276 2024-05-29 10:47:12.127163 nortech-0.2.2/nortech/derivers/services/physical_units.py
+-rw-r--r--   0        0        0     3564 2024-05-29 12:58:49.727767 nortech-0.2.2/nortech/derivers/services/schema.py
+-rw-r--r--   0        0        0     2288 2024-05-29 09:46:25.353623 nortech-0.2.2/nortech/derivers/services/visualize.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:45:01.197564 nortech-0.2.2/nortech/derivers/values/__init__.py
+-rw-r--r--   0        0        0     1948 2024-05-29 11:12:50.690657 nortech-0.2.2/nortech/derivers/values/instance.py
+-rw-r--r--   0        0        0     3918 2024-05-29 09:46:25.353139 nortech-0.2.2/nortech/derivers/values/physical_units.py
+-rw-r--r--   0        0        0      351 2024-05-29 09:45:01.197672 nortech-0.2.2/nortech/derivers/values/physical_units_schema.py
+-rw-r--r--   0        0        0     6007 2024-05-29 09:46:25.349173 nortech-0.2.2/nortech/derivers/values/schema.py
+-rw-r--r--   0        0        0      825 2024-05-31 10:24:38.827259 nortech-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7290 1970-01-01 00:00:00.000000 nortech-0.2.2/PKG-INFO
```

### Comparing `nortech-0.2.1/LICENSE` & `nortech-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nortech-0.2.1/README.md` & `nortech-0.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,21 @@
 
 Or if you are using poetry:
 
 ```bash
 poetry add nortech
 ```
 
-## S3
+## nortech.datatools
 
-### Config
+
+
+### S3
+
+#### Config
 
 Setup your environment variables with the `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` provided to you:
 
 ```bash
 export AWS_ACCESS_KEY_ID="<AWS_ACCESS_KEY_ID>"
 export AWS_SECRET_ACCESS_KEY="<AWS_SECRET_ACCESS_KEY>"
 ```
@@ -35,24 +39,24 @@
 
 As an alternative you can use the [AWS CLI](https://aws.amazon.com/cli/):
 
 ```bash
 aws configure
 ```
 
-### Examples
+#### Examples
 
 To get a DataFrame with the requested signals:
 
 1. Go to your `Signal Search` interface.
 2. Select the desired signals.
 3. Select the `DataTools` exported columns and copy the resulting `search_json`.
 4. Use the `search_json` and speficy a `TimeWindow` as in the examples bellow.
 
-#### Pandas DataFrame
+##### Pandas DataFrame
 
 In order to get a [pandas](https://pandas.pydata.org/docs/) DataFrame use the `get_df`:
 
 ```python
 from datetime import datetime
 
 from nortech.datatools import get_df, TimeWindow
@@ -117,22 +121,21 @@
 time_window = TimeWindow(
             start=datetime(2020, 1, 1),
             end=datetime(2020, 1, 5),
 )
 df = get_df(search_json=search_json, time_window=time_window)
 
 assert list(df.columns) == [
-    'timestamp',
     'asset_1/division_1/unit_1/signal_1',
     'asset_1/division_1/unit_1/signal_2',
     'asset_2/division_2/unit_2/signal_3'
 ]
 ```
 
-#### Polars DataFrame
+##### Polars DataFrame
 
 In order to get a [polars](https://pola-rs.github.io/polars/py-polars/html/reference/) DataFrame use the `get_polars_df`:
 
 ```python
 from datetime import datetime
 
 from nortech.datatools import get_polars_df, TimeWindow
@@ -204,15 +207,15 @@
     'timestamp',
     'asset_1/division_1/unit_1/signal_1',
     'asset_1/division_1/unit_1/signal_2',
     'asset_2/division_2/unit_2/signal_3'
 ]
 ```
 
-#### Polars LazyFrame
+##### Polars LazyFrame
 
 In order to get a [polars](https://pola-rs.github.io/polars/py-polars/html/reference/) LazyFrame use the `get_lazy_polars_df`:
 
 ```python
 from datetime import datetime
 
 from nortech.datatools import get_lazy_polars_df, TimeWindow
```

### Comparing `nortech-0.2.1/nortech/datatools/handlers/pandas.py` & `nortech-0.2.2/nortech/datatools/handlers/pandas.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,10 +98,10 @@
             'asset_1/division_1/unit_1/signal_1',
             'asset_1/division_1/unit_1/signal_2',
             'asset_2/division_2/unit_2/signal_3'
         ]
     """
     polars_df = get_polars_df(search_json=search_json, time_window=time_window)
 
-    df = polars_df.to_pandas()
+    df = polars_df.to_pandas().set_index("timestamp")
 
     return df
```

### Comparing `nortech-0.2.1/nortech/datatools/handlers/polars.py` & `nortech-0.2.2/nortech/datatools/handlers/polars.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.1/nortech/datatools/repositories/S3.py` & `nortech-0.2.2/nortech/datatools/repositories/S3.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from os import getenv
 from typing import List, Tuple
 
 import pyarrow as pa
 from polars import Expr, LazyFrame, col, from_epoch, scan_pyarrow_dataset
 from pyarrow import DataType, Schema, schema
 from pyarrow.dataset import dataset, partitioning
@@ -126,14 +126,17 @@
     Raises
     ------
     NoSignalsRequestedError
         Raised when no signals are requested.
     InvalidTimeWindow
         Raised when the start date is after the end date.
     """
+    start = time_window.start.astimezone(timezone.utc)
+    end = time_window.end.astimezone(timezone.utc)
+
     s3_file_system = S3FileSystem(endpoint_url=getenv("AWS_ENDPOINT_URL"))
 
     lazy_dfs = None
     for location, columns in parquet_paths.items():
         pyarrow_ds = dataset(
             location,
             format="parquet",
@@ -149,29 +152,33 @@
         )
 
         lazy_df = scan_pyarrow_dataset(pyarrow_ds)
 
         select_columns = get_select_columns(columns=columns)
         lazy_df_select = lazy_df.select(select_columns)
 
-        lazy_df_partition = lazy_df_select.filter(
-            generate_date_filter(time_window.start, time_window.end)
-        )
+        lazy_df_partition = lazy_df_select.filter(generate_date_filter(start, end))
 
         lazy_df_without_partition_columns = lazy_df_partition.drop(
             ["year", "month", "day"]
         )
 
-        lazy_df_window = lazy_df_without_partition_columns.with_columns(
-            from_epoch("timestamp", "ms")
-        ).filter(
-            col("timestamp").is_between(
-                lower_bound=time_window.start,
-                upper_bound=time_window.end,
-                closed="right",
+        lazy_df_window = (
+            lazy_df_without_partition_columns.with_columns(
+                from_epoch("timestamp", "ms").dt.replace_time_zone("UTC"),
+            )
+            .filter(
+                col("timestamp").is_between(
+                    lower_bound=start,
+                    upper_bound=end,
+                    closed="right",
+                )
+            )
+            .with_columns(
+                col("timestamp").dt.convert_time_zone(str(time_window.start.tzinfo))
             )
         )
 
         if lazy_dfs is not None:
             lazy_dfs = lazy_dfs.join(lazy_df_window, on="timestamp", how="outer")
         else:
             lazy_dfs = lazy_df_window
```

### Comparing `nortech-0.2.1/nortech/datatools/services/config.py` & `nortech-0.2.2/nortech/datatools/services/config.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.1/nortech/datatools/values/signals.py` & `nortech-0.2.2/nortech/datatools/values/signals.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from dataclasses import dataclass
-from datetime import datetime, timezone
+from datetime import datetime
 from json import loads
 from typing import Dict, List
 
 from pydantic import BaseModel
+from tzlocal import get_localzone
 
 from nortech.datatools.values.errors import InvalidTimeWindow
 
 
 @dataclass
 class TimeWindow:
     start: datetime
     end: datetime
 
     def __post_init__(self):
-        self.start = self.start.astimezone(timezone.utc).replace(tzinfo=None)
-        self.end = self.end.astimezone(timezone.utc).replace(tzinfo=None)
+        if self.start.tzinfo is None:
+            self.start = self.start.replace(tzinfo=get_localzone())
+
+        if self.end.tzinfo is None:
+            self.end = self.end.replace(tzinfo=get_localzone())
+
         if self.end < self.start:
             raise InvalidTimeWindow()
 
 
 @dataclass
 class SignalConfig:
     column_name: str
```

### Comparing `nortech-0.2.1/nortech/derivers/gateways/customer_api.py` & `nortech-0.2.2/nortech/derivers/gateways/customer_api.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.1/nortech/derivers/handlers/deriver.py` & `nortech-0.2.2/nortech/derivers/handlers/deriver.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.1/nortech/derivers/services/operators.py` & `nortech-0.2.2/nortech/derivers/services/operators.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.1/nortech/derivers/services/schema.py` & `nortech-0.2.2/nortech/derivers/services/schema.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.1/nortech/derivers/services/visualize.py` & `nortech-0.2.2/nortech/derivers/services/visualize.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.1/nortech/derivers/values/instance.py` & `nortech-0.2.2/nortech/derivers/values/instance.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.1/nortech/derivers/values/physical_units.py` & `nortech-0.2.2/nortech/derivers/values/physical_units.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.1/nortech/derivers/values/schema.py` & `nortech-0.2.2/nortech/derivers/values/schema.py`

 * *Files identical despite different names*

### Comparing `nortech-0.2.1/pyproject.toml` & `nortech-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nortech"
-version = "0.2.1"
+version = "0.2.2"
 description = "The official Python library for Nortech AI"
 authors = ["Nortech AI <info@nortech.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://nortech.ai/"
 repository = "https://github.com/Nortech-ai/nortech-python"
 
@@ -16,18 +16,20 @@
 s3fs = "2023.6.0"
 aiobotocore = "2.5.2"
 pydantic = "^2.5.2"
 bytewax = "^0.20.0"
 pydantic-settings = "^2.2.1"
 pint = "^0.23"
 python-dotenv = "^1.0.1"
+tzlocal = "^5.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 ipykernel = "^6.27.1"
 black = "^23.11.0"
 flake8 = "^6.1.0"
 moto = {extras = ["server"], version = "^4.2.11"}
+plotly = "^5.22.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nortech-0.2.1/PKG-INFO` & `nortech-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nortech
-Version: 0.2.1
+Version: 0.2.2
 Summary: The official Python library for Nortech AI
 Home-page: https://nortech.ai/
 License: Apache-2.0
 Author: Nortech AI
 Author-email: info@nortech.ai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -18,14 +18,15 @@
 Requires-Dist: pint (>=0.23,<0.24)
 Requires-Dist: polars (>=0.19.19,<0.20.0)
 Requires-Dist: pyarrow (>=13.0.0,<14.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: s3fs (==2023.6.0)
+Requires-Dist: tzlocal (>=5.2,<6.0)
 Project-URL: Repository, https://github.com/Nortech-ai/nortech-python
 Description-Content-Type: text/markdown
 
 # nortech-python
 
 The official Python library for Nortech AI.
 
@@ -39,17 +40,21 @@
 
 Or if you are using poetry:
 
 ```bash
 poetry add nortech
 ```
 
-## S3
+## nortech.datatools
 
-### Config
+
+
+### S3
+
+#### Config
 
 Setup your environment variables with the `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` provided to you:
 
 ```bash
 export AWS_ACCESS_KEY_ID="<AWS_ACCESS_KEY_ID>"
 export AWS_SECRET_ACCESS_KEY="<AWS_SECRET_ACCESS_KEY>"
 ```
@@ -62,24 +67,24 @@
 
 As an alternative you can use the [AWS CLI](https://aws.amazon.com/cli/):
 
 ```bash
 aws configure
 ```
 
-### Examples
+#### Examples
 
 To get a DataFrame with the requested signals:
 
 1. Go to your `Signal Search` interface.
 2. Select the desired signals.
 3. Select the `DataTools` exported columns and copy the resulting `search_json`.
 4. Use the `search_json` and speficy a `TimeWindow` as in the examples bellow.
 
-#### Pandas DataFrame
+##### Pandas DataFrame
 
 In order to get a [pandas](https://pandas.pydata.org/docs/) DataFrame use the `get_df`:
 
 ```python
 from datetime import datetime
 
 from nortech.datatools import get_df, TimeWindow
@@ -144,22 +149,21 @@
 time_window = TimeWindow(
             start=datetime(2020, 1, 1),
             end=datetime(2020, 1, 5),
 )
 df = get_df(search_json=search_json, time_window=time_window)
 
 assert list(df.columns) == [
-    'timestamp',
     'asset_1/division_1/unit_1/signal_1',
     'asset_1/division_1/unit_1/signal_2',
     'asset_2/division_2/unit_2/signal_3'
 ]
 ```
 
-#### Polars DataFrame
+##### Polars DataFrame
 
 In order to get a [polars](https://pola-rs.github.io/polars/py-polars/html/reference/) DataFrame use the `get_polars_df`:
 
 ```python
 from datetime import datetime
 
 from nortech.datatools import get_polars_df, TimeWindow
@@ -231,15 +235,15 @@
     'timestamp',
     'asset_1/division_1/unit_1/signal_1',
     'asset_1/division_1/unit_1/signal_2',
     'asset_2/division_2/unit_2/signal_3'
 ]
 ```
 
-#### Polars LazyFrame
+##### Polars LazyFrame
 
 In order to get a [polars](https://pola-rs.github.io/polars/py-polars/html/reference/) LazyFrame use the `get_lazy_polars_df`:
 
 ```python
 from datetime import datetime
 
 from nortech.datatools import get_lazy_polars_df, TimeWindow
```

