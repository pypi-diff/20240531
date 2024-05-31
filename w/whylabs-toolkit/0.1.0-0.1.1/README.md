# Comparing `tmp/whylabs_toolkit-0.1.0.tar.gz` & `tmp/whylabs_toolkit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylabs_toolkit-0.1.0.tar", max compression
+gzip compressed data, was "whylabs_toolkit-0.1.1.tar", max compression
```

## Comparing `whylabs_toolkit-0.1.0.tar` & `whylabs_toolkit-0.1.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    11357 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/LICENSE
--rw-r--r--   0        0        0     2056 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/README.md
--rw-r--r--   0        0        0     1288 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/cli/__init__.py
--rw-r--r--   0        0        0      559 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/container/config_types.py
--rw-r--r--   0        0        0        0 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/__init__.py
--rw-r--r--   0        0        0      362 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/client.py
--rw-r--r--   0        0        0     2029 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/config.py
--rw-r--r--   0        0        0     1257 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/cron_validators.py
--rw-r--r--   0        0        0     2488 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/dataset_profiles.py
--rw-r--r--   0        0        0     2199 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/models.py
--rw-r--r--   0        0        0     4699 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/monitor_helpers.py
--rw-r--r--   0        0        0     5922 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/schema.py
--rw-r--r--   0        0        0     1160 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/utils.py
--rw-r--r--   0        0        0      100 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 14:09:33.035840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/__init__.py
--rw-r--r--   0        0        0      113 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/constants.py
--rw-r--r--   0        0        0        0 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/converters/__init__.py
--rw-r--r--   0        0        0     1516 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/converters/granularity.py
--rw-r--r--   0        0        0        0 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/helpers/__init__.py
--rw-r--r--   0        0        0     1099 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/helpers/describe.py
--rw-r--r--   0        0        0     2192 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/helpers/utils.py
--rw-r--r--   0        0        0       62 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/models/__init__.py
--rw-r--r--   0        0        0     9555 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/models/diagnosis_report.py
--rw-r--r--   0        0        0      976 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/models/noisy_monitors.py
--rw-r--r--   0        0        0    18045 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/monitor_diagnoser.py
--rw-r--r--   0        0        0        0 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/recommendation/__init__.py
--rw-r--r--   0        0        0     7234 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/recommendation/change_recommender.py
--rw-r--r--   0        0        0      686 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/recommendation/manual_change.py
--rw-r--r--   0        0        0     2187 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/recommendation/recommended_change.py
--rw-r--r--   0        0        0     1809 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/recommendation/remove_columns.py
--rw-r--r--   0        0        0     1392 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/targeting.py
--rw-r--r--   0        0        0      178 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/manager/__init__.py
--rw-r--r--   0        0        0      557 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/manager/credentials.py
--rw-r--r--   0        0        0     5907 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/manager/manager.py
--rw-r--r--   0        0        0    14684 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/manager/monitor_setup.py
--rw-r--r--   0        0        0     1769 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/__init__.py
--rw-r--r--   0        0        0     1048 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/__init__.py
--rw-r--r--   0        0        0    15205 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/algorithms.py
--rw-r--r--   0        0        0     5693 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/analyzer.py
--rw-r--r--   0        0        0     3242 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/baseline.py
--rw-r--r--   0        0        0     2232 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/targets.py
--rw-r--r--   0        0        0     4115 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/column_schema.py
--rw-r--r--   0        0        0     3323 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/commons.py
--rw-r--r--   0        0        0     2366 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/document.py
--rw-r--r--   0        0        0     9610 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/monitor.py
--rw-r--r--   0        0        0      574 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/segments.py
--rw-r--r--   0        0        0      961 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/utils.py
--rw-r--r--   0        0        0    78578 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/schema/schema.json
--rw-r--r--   0        0        0        0 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/utils/__init__.py
--rw-r--r--   0        0        0      176 2024-05-13 14:09:33.039840 whylabs_toolkit-0.1.0/whylabs_toolkit/utils/granularity.py
--rw-r--r--   0        0        0     3661 1970-01-01 00:00:00.000000 whylabs_toolkit-0.1.0/setup.py
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 whylabs_toolkit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-31 14:56:27.240727 whylabs_toolkit-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2056 2024-05-31 14:56:27.240727 whylabs_toolkit-0.1.1/README.md
+-rw-r--r--   0        0        0     1288 2024-05-31 14:56:27.240727 whylabs_toolkit-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/cli/__init__.py
+-rw-r--r--   0        0        0      559 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/container/config_types.py
+-rw-r--r--   0        0        0        0 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/__init__.py
+-rw-r--r--   0        0        0      362 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/client.py
+-rw-r--r--   0        0        0     2029 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/config.py
+-rw-r--r--   0        0        0     1257 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/cron_validators.py
+-rw-r--r--   0        0        0     2488 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/dataset_profiles.py
+-rw-r--r--   0        0        0     2199 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/models.py
+-rw-r--r--   0        0        0     4699 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/monitor_helpers.py
+-rw-r--r--   0        0        0     5922 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/schema.py
+-rw-r--r--   0        0        0     1160 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/utils.py
+-rw-r--r--   0        0        0      100 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/constants.py
+-rw-r--r--   0        0        0        0 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/converters/__init__.py
+-rw-r--r--   0        0        0     1230 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/converters/granularity.py
+-rw-r--r--   0        0        0        0 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/helpers/__init__.py
+-rw-r--r--   0        0        0     1099 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/helpers/describe.py
+-rw-r--r--   0        0        0     2192 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/helpers/utils.py
+-rw-r--r--   0        0        0       62 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/models/__init__.py
+-rw-r--r--   0        0        0     9555 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/models/diagnosis_report.py
+-rw-r--r--   0        0        0      976 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/models/noisy_monitors.py
+-rw-r--r--   0        0        0    18045 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/monitor_diagnoser.py
+-rw-r--r--   0        0        0        0 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/recommendation/__init__.py
+-rw-r--r--   0        0        0     7234 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/recommendation/change_recommender.py
+-rw-r--r--   0        0        0      686 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/recommendation/manual_change.py
+-rw-r--r--   0        0        0     2187 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/recommendation/recommended_change.py
+-rw-r--r--   0        0        0     1809 2024-05-31 14:56:27.244727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/recommendation/remove_columns.py
+-rw-r--r--   0        0        0     1392 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/targeting.py
+-rw-r--r--   0        0        0      178 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/manager/__init__.py
+-rw-r--r--   0        0        0      557 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/manager/credentials.py
+-rw-r--r--   0        0        0     5907 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/manager/manager.py
+-rw-r--r--   0        0        0    14684 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/manager/monitor_setup.py
+-rw-r--r--   0        0        0     1769 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/__init__.py
+-rw-r--r--   0        0        0     1048 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/analyzer/__init__.py
+-rw-r--r--   0        0        0    15205 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/analyzer/algorithms.py
+-rw-r--r--   0        0        0     5693 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/analyzer/analyzer.py
+-rw-r--r--   0        0        0     3242 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/analyzer/baseline.py
+-rw-r--r--   0        0        0     2232 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/analyzer/targets.py
+-rw-r--r--   0        0        0     4115 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/column_schema.py
+-rw-r--r--   0        0        0     3323 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/commons.py
+-rw-r--r--   0        0        0     2366 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/document.py
+-rw-r--r--   0        0        0     9610 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/monitor.py
+-rw-r--r--   0        0        0      574 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/segments.py
+-rw-r--r--   0        0        0      961 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/utils.py
+-rw-r--r--   0        0        0    78578 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/schema/schema.json
+-rw-r--r--   0        0        0        0 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-31 14:56:27.248727 whylabs_toolkit-0.1.1/whylabs_toolkit/utils/granularity.py
+-rw-r--r--   0        0        0     3661 1970-01-01 00:00:00.000000 whylabs_toolkit-0.1.1/setup.py
+-rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 whylabs_toolkit-0.1.1/PKG-INFO
```

### Comparing `whylabs_toolkit-0.1.0/LICENSE` & `whylabs_toolkit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/README.md` & `whylabs_toolkit-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/pyproject.toml` & `whylabs_toolkit-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "whylabs-toolkit"
-version = "0.1.0"
+version = "0.1.1"
 description = "Whylabs Toolkit package."
 authors = ["Murilo Mendonca <murilommen@gmail.com>", "Anthony Naddeo <anthony.naddeo@gmail.com>",
     "Christine Draper <christine@whylabs.ai>"]
 license = "Apache-2.0 license"
 readme = "README.md"
 packages = [{include = "whylabs_toolkit/**/*.py"}]
 include = ["whylabs_toolkit/monitor/schema/schema.json"]
```

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/container/config_types.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/container/config_types.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/config.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/config.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/cron_validators.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/cron_validators.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/dataset_profiles.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/dataset_profiles.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/models.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/models.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/monitor_helpers.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/monitor_helpers.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/schema.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/schema.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/helpers/utils.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/converters/granularity.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/converters/granularity.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,28 @@
-from dateutil.relativedelta import relativedelta
-from whylabs_toolkit.utils.granularity import Granularity
+from math import floor
 from isodate import parse_datetime, parse_duration, parse_date
 
 
-def batches_to_timedelta(time_period: str, batches: int) -> relativedelta:
-    if time_period == "PT1H":
-        return relativedelta(hours=batches)
-
-    if time_period == "P1W":
-        return relativedelta(weeks=batches)
-
-    if time_period == "P1M":
-        return relativedelta(months=batches)
-
-    return relativedelta(days=batches)
-
-
 def calculate_num_batches(interval: str, granularity: str) -> int:
     # Parse the ISO8601 interval string into a start and end datetime
     start, end = interval.split("/")
     start_date = parse_datetime(start) if "T" in start else parse_date(start)
     try:
         end_date = parse_datetime(end) if "T" in start else parse_date(end)
     except ValueError:
         end_date = start_date + parse_duration(end)
 
-    # Calculate the difference based on the granularity
+    # Calculate the (somewhat approximate) difference based on the granularity
+    # Truncates to whole batches, ignores leap seconds
     if granularity == "hourly":
-        difference = relativedelta(end_date, start_date).days * 24 + relativedelta(end_date, start_date).hours
+        difference = (end_date - start_date).total_seconds() / 3600
     elif granularity == "daily":
-        difference = relativedelta(end_date, start_date).days
+        difference = (end_date - start_date).total_seconds() / (3600 * 24)
     elif granularity == "weekly":
-        difference = relativedelta(end_date, start_date).weeks
+        difference = (end_date - start_date).total_seconds() / (3600 * 24 * 7)
     elif granularity == "monthly":
-        difference = relativedelta(end_date, start_date).months
+        difference = (end_date.year - start_date.year) * 12 + end_date.month - start_date.month
     else:
         raise ValueError(f"Unsupported granularity: {granularity}")
 
-    return difference
+    diff_as_int: int = floor(difference)
+    return diff_as_int
```

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/helpers/describe.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/helpers/describe.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/helpers/utils.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/models/diagnosis_report.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/models/diagnosis_report.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/models/noisy_monitors.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/models/noisy_monitors.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/monitor_diagnoser.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/monitor_diagnoser.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/recommendation/change_recommender.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/recommendation/change_recommender.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/recommendation/manual_change.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/recommendation/manual_change.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/recommendation/recommended_change.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/recommendation/recommended_change.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/recommendation/remove_columns.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/recommendation/remove_columns.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/diagnoser/targeting.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/diagnoser/targeting.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/manager/credentials.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/manager/credentials.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/manager/manager.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/manager/manager.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/manager/monitor_setup.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/manager/monitor_setup.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/__init__.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/__init__.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/__init__.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/algorithms.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/analyzer/algorithms.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/analyzer.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/baseline.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/analyzer/baseline.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/analyzer/targets.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/analyzer/targets.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/column_schema.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/column_schema.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/commons.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/commons.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/document.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/document.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/monitor.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/monitor.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/segments.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/segments.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/models/utils.py` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/models/utils.py`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/whylabs_toolkit/monitor/schema/schema.json` & `whylabs_toolkit-0.1.1/whylabs_toolkit/monitor/schema/schema.json`

 * *Files identical despite different names*

### Comparing `whylabs_toolkit-0.1.0/setup.py` & `whylabs_toolkit-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                'numpy>=1.24.1,<2.0.0',
                'tabulate>=0.8.9,<0.9.0',
                'isodate>=0.6.1,<0.7.0',
                'python-dateutil>=2.8.2,<3.0.0']}
 
 setup_kwargs = {
     'name': 'whylabs-toolkit',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Whylabs Toolkit package.',
     'long_description': "# WhyLabs Toolkit\n\nThe WhyLabs Toolkit package contains helper methods to help users interact with our internal APIs. Users will benefit from using it if they want to abstract some of WhyLabs' internal logic and also automate recurring API calls.\n\n\n## Basic usage\nTo start using the `whylabs_toolkit` package, install it from PyPI with:\n```bash\npip install whylabs_toolkit\n``` \n\n## Packages\n\nThe available packages that we have enable different use-cases for the `whylabs_toolkit`. To get started, navigate to one of the following sections and find useful tutorials there.\n\n| Package                                                                                                                   | Usage                                                                  |\n|---------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------|\n| [Monitor Manager](https://github.com/whylabs/whylabs-toolkit/blob/mainline/whylabs_toolkit/monitor/manager/README.md)     | Author and modify existing WhyLabs monitor with Python.                |\n| [Monitor Diagnoser](https://github.com/whylabs/whylabs-toolkit/blob/mainline/whylabs_toolkit/monitor/diagnoser/README.md) | Diagnose problems with monitors.                                       |\n| [WhyLabs Helpers](https://github.com/whylabs/whylabs-toolkit/blob/mainline/whylabs_toolkit/helpers/README.md)             | Interact with and modify your Datasets and ML Models specs in WhyLabs. |\n\n## Development\n\nTo start contributing, you will manage dependencies with [Poetry](https://python-poetry.org/) and also a handful of `Makefile` commands. To install all necessary dependencies and activate the virtual environment, run:\n\n```bash\nmake setup && poetry shell\n```\n\n## Get in touch\nIf you want to learn more how you can benefit from this package or if there is anything missing, please [contact our support](https://whylabs.ai/contact-us), we'll be more than happy to help you!",
     'author': 'Murilo Mendonca',
     'author_email': 'murilommen@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `whylabs_toolkit-0.1.0/PKG-INFO` & `whylabs_toolkit-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whylabs-toolkit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Whylabs Toolkit package.
 License: Apache-2.0 license
 Author: Murilo Mendonca
 Author-email: murilommen@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

