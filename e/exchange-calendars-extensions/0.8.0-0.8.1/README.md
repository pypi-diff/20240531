# Comparing `tmp/exchange_calendars_extensions-0.8.0.tar.gz` & `tmp/exchange_calendars_extensions-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchange_calendars_extensions-0.8.0.tar", max compression
+gzip compressed data, was "exchange_calendars_extensions-0.8.1.tar", max compression
```

## Comparing `exchange_calendars_extensions-0.8.0.tar` & `exchange_calendars_extensions-0.8.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-05-10 06:32:21.327228 exchange_calendars_extensions-0.8.0/LICENSE
--rw-r--r--   0        0        0    25890 2024-05-10 06:32:21.327228 exchange_calendars_extensions-0.8.0/README.md
--rw-r--r--   0        0        0    25332 2024-05-10 06:32:21.331228 exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/__init__.py
--rw-r--r--   0        0        0     6872 2024-05-10 06:32:21.331228 exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/holiday.py
--rw-r--r--   0        0        0    45563 2024-05-10 06:32:21.331228 exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/holiday_calendar.py
--rw-r--r--   0        0        0     5787 2024-05-10 06:32:21.331228 exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/offset.py
--rw-r--r--   0        0        0     2764 2024-05-10 06:32:21.331228 exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/util.py
--rw-r--r--   0        0        0       18 2024-05-10 06:32:32.371310 exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/version.py
--rw-r--r--   0        0        0     2911 2024-05-10 06:32:32.303310 exchange_calendars_extensions-0.8.0/pyproject.toml
--rw-r--r--   0        0        0    27388 1970-01-01 00:00:00.000000 exchange_calendars_extensions-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-31 21:42:02.828643 exchange_calendars_extensions-0.8.1/LICENSE
+-rw-r--r--   0        0        0    25890 2024-05-31 21:42:02.832643 exchange_calendars_extensions-0.8.1/README.md
+-rw-r--r--   0        0        0    25332 2024-05-31 21:42:02.832643 exchange_calendars_extensions-0.8.1/exchange_calendars_extensions/core/__init__.py
+-rw-r--r--   0        0        0     6872 2024-05-31 21:42:02.832643 exchange_calendars_extensions-0.8.1/exchange_calendars_extensions/core/holiday.py
+-rw-r--r--   0        0        0    47764 2024-05-31 21:42:02.832643 exchange_calendars_extensions-0.8.1/exchange_calendars_extensions/core/holiday_calendar.py
+-rw-r--r--   0        0        0     5787 2024-05-31 21:42:02.832643 exchange_calendars_extensions-0.8.1/exchange_calendars_extensions/core/offset.py
+-rw-r--r--   0        0        0     2764 2024-05-31 21:42:02.832643 exchange_calendars_extensions-0.8.1/exchange_calendars_extensions/core/util.py
+-rw-r--r--   0        0        0       18 2024-05-31 21:42:15.492756 exchange_calendars_extensions-0.8.1/exchange_calendars_extensions/core/version.py
+-rw-r--r--   0        0        0     2911 2024-05-31 21:42:15.428756 exchange_calendars_extensions-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0    27388 1970-01-01 00:00:00.000000 exchange_calendars_extensions-0.8.1/PKG-INFO
```

### Comparing `exchange_calendars_extensions-0.8.0/LICENSE` & `exchange_calendars_extensions-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.8.0/README.md` & `exchange_calendars_extensions-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/__init__.py` & `exchange_calendars_extensions-0.8.1/exchange_calendars_extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/holiday.py` & `exchange_calendars_extensions-0.8.1/exchange_calendars_extensions/core/holiday.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/holiday_calendar.py` & `exchange_calendars_extensions-0.8.1/exchange_calendars_extensions/core/holiday_calendar.py`

 * *Files 2% similar despite different names*

```diff
@@ -953,20 +953,30 @@
 
     def __init__(self, *args, **kwargs):
         # Save adjusted properties. Initialize with copies of the original properties.
         a = AdjustedProperties(
             regular_holidays=list(copy(regular_holidays_orig(self).rules)),
             adhoc_holidays=list(copy(adhoc_holidays_orig(self))),
             special_closes=[
-                (t, d if isinstance(d, int) else list(copy(d.rules)))
+                (
+                    t,
+                    [DayOfWeekPeriodicHoliday("special close", d)]
+                    if isinstance(d, int)
+                    else list(copy(d.rules)),
+                )  # Convert day-of-week to rule, else just copy.
                 for t, d in copy(special_closes_orig(self))
             ],
             adhoc_special_closes=list(copy(adhoc_special_closes_orig(self))),
             special_opens=[
-                (t, d if isinstance(d, int) else list(copy(d.rules)))
+                (
+                    t,
+                    [DayOfWeekPeriodicHoliday("special open", d)]
+                    if isinstance(d, int)
+                    else list(copy(d.rules)),
+                )  # Convert day-of-week to rule, else just copy.
                 for t, d in copy(special_opens_orig(self))
             ],
             adhoc_special_opens=list(copy(adhoc_special_opens_orig(self))),
         )
 
         # Get changeset from provider, maybe.
         changeset: Union[ChangeSet, None] = (
@@ -1074,14 +1084,54 @@
             [
                 get_holidays_calendar(self),
                 get_special_opens_calendar(self),
                 get_special_closes_calendar(self),
             ]
         )
 
+        # Remove instances of weekly special open/close days that also coincide with a holiday.
+        all_holidays = None
+
+        def get_all_holidays() -> pd.DatetimeIndex:
+            return self._holidays_shared.holidays(
+                start=self.schedule.index[0], end=self.schedule.index[-1]
+            )
+
+        for t, rules in self._adjusted_properties.special_opens:
+            for rule in rules:
+                if isinstance(rule, DayOfWeekPeriodicHoliday):
+                    if all_holidays is None:
+                        all_holidays = get_all_holidays()
+                    for ts in all_holidays.intersection(
+                        rule.dates(
+                            start_date=self.schedule.index[0],
+                            end_date=self.schedule.index[-1],
+                        )
+                    ):
+                        a.special_opens, a.adhoc_special_opens = remove_special_session(
+                            ts, a.special_opens, a.adhoc_special_opens
+                        )
+
+        for t, rules in self._adjusted_properties.special_closes:
+            for rule in rules:
+                if isinstance(rule, DayOfWeekPeriodicHoliday):
+                    if all_holidays is None:
+                        all_holidays = get_all_holidays()
+                    for ts in all_holidays.intersection(
+                        rule.dates(
+                            start_date=self.schedule.index[0],
+                            end_date=self.schedule.index[-1],
+                        )
+                    ):
+                        a.special_closes, a.adhoc_special_closes = (
+                            remove_special_session(
+                                ts, a.special_closes, a.adhoc_special_closes
+                            )
+                        )
+
     @property
     def regular_holidays(self) -> Union[HolidayCalendar, None]:
         return HolidayCalendar(rules=self._adjusted_properties.regular_holidays)
 
     @property
     def adhoc_holidays(self) -> list[pd.Timestamp]:
         return copy(self._adjusted_properties.adhoc_holidays)
```

### Comparing `exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/offset.py` & `exchange_calendars_extensions-0.8.1/exchange_calendars_extensions/core/offset.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.8.0/exchange_calendars_extensions/core/util.py` & `exchange_calendars_extensions-0.8.1/exchange_calendars_extensions/core/util.py`

 * *Files identical despite different names*

### Comparing `exchange_calendars_extensions-0.8.0/pyproject.toml` & `exchange_calendars_extensions-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "exchange-calendars-extensions"
-version = "0.8.0"
+version = "0.8.1"
 description = "Extensions of the exchange-calendars package"
 license = "Apache-2.0"
 authors = ["Jens Keiner <jens.keiner@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/jenskeiner/exchange_calendars_extensions/"
 repository = "https://github.com/jenskeiner/exchange_calendars_extensions/"
 documentation = "https://github.com/jenskeiner/exchange_calendars_extensions/tree/main/docs/"
@@ -29,15 +29,15 @@
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 packages = [{include = "exchange_calendars_extensions"}]
 
 [tool.poetry.dependencies]
 python = "~=3.9"
-exchange-calendars-extensions-api = ">=0.4.0,<1"
+exchange-calendars-extensions-api = ">=0.4.2,<1"
 exchange-calendars = ">=4.0.1,<5"
 typing-extensions = ">=4.0,<5"
 pydantic = ">=2.0,<3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.3.1,<8.3.0"
 pytest-mock = ">=3.11.1,<3.15.0"
```

### Comparing `exchange_calendars_extensions-0.8.0/PKG-INFO` & `exchange_calendars_extensions-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exchange-calendars-extensions
-Version: 0.8.0
+Version: 0.8.1
 Summary: Extensions of the exchange-calendars package
 Home-page: https://github.com/jenskeiner/exchange_calendars_extensions/
 License: Apache-2.0
 Keywords: exchange,calendar,trading,holidays
 Author: Jens Keiner
 Author-email: jens.keiner@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: exchange-calendars (>=4.0.1,<5)
-Requires-Dist: exchange-calendars-extensions-api (>=0.4.0,<1)
+Requires-Dist: exchange-calendars-extensions-api (>=0.4.2,<1)
 Requires-Dist: pydantic (>=2.0,<3)
 Requires-Dist: typing-extensions (>=4.0,<5)
 Project-URL: Documentation, https://github.com/jenskeiner/exchange_calendars_extensions/tree/main/docs/
 Project-URL: Repository, https://github.com/jenskeiner/exchange_calendars_extensions/
 Description-Content-Type: text/markdown
 
 # exchange-calendars-extensions
```

