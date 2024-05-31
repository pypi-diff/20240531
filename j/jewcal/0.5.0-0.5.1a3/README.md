# Comparing `tmp/jewcal-0.5.0.tar.gz` & `tmp/jewcal-0.5.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jewcal-0.5.0.tar", last modified: Wed Nov  1 17:08:05 2023, max compression
+gzip compressed data, was "jewcal-0.5.1a3.tar", last modified: Fri May 31 15:28:28 2024, max compression
```

## Comparing `jewcal-0.5.0.tar` & `jewcal-0.5.1a3.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 17:08:05.177546 jewcal-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-11-01 17:07:55.000000 jewcal-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2023-11-01 17:08:05.177546 jewcal-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8311 2023-11-01 17:07:55.000000 jewcal-0.5.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2023-11-01 17:07:55.000000 jewcal-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-01 17:08:05.177546 jewcal-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 17:08:05.177546 jewcal-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 17:08:05.177546 jewcal-0.5.0/src/jewcal/
--rw-r--r--   0 runner    (1001) docker     (127)      770 2023-11-01 17:07:55.000000 jewcal-0.5.0/src/jewcal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2023-11-01 17:07:55.000000 jewcal-0.5.0/src/jewcal/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2023-11-01 17:07:55.000000 jewcal-0.5.0/src/jewcal/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 17:08:05.177546 jewcal-0.5.0/src/jewcal/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-01 17:07:55.000000 jewcal-0.5.0/src/jewcal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9873 2023-11-01 17:07:55.000000 jewcal-0.5.0/src/jewcal/utils/calculations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-01 17:08:05.177546 jewcal-0.5.0/src/jewcal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9066 2023-11-01 17:08:05.000000 jewcal-0.5.0/src/jewcal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-11-01 17:08:05.000000 jewcal-0.5.0/src/jewcal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-01 17:08:05.000000 jewcal-0.5.0/src/jewcal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2023-11-01 17:08:05.000000 jewcal-0.5.0/src/jewcal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-11-01 17:08:05.000000 jewcal-0.5.0/src/jewcal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:28:28.280654 jewcal-0.5.1a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-31 15:28:23.000000 jewcal-0.5.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-31 15:28:28.280654 jewcal-0.5.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-31 15:28:23.000000 jewcal-0.5.1a3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-31 15:28:23.000000 jewcal-0.5.1a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:28:28.280654 jewcal-0.5.1a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:28:28.276654 jewcal-0.5.1a3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:28:28.280654 jewcal-0.5.1a3/src/jewcal/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-31 15:28:23.000000 jewcal-0.5.1a3/src/jewcal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-31 15:28:23.000000 jewcal-0.5.1a3/src/jewcal/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-05-31 15:28:23.000000 jewcal-0.5.1a3/src/jewcal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-05-31 15:28:23.000000 jewcal-0.5.1a3/src/jewcal/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-31 15:28:23.000000 jewcal-0.5.1a3/src/jewcal/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:28:28.280654 jewcal-0.5.1a3/src/jewcal/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 15:28:23.000000 jewcal-0.5.1a3/src/jewcal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-05-31 15:28:23.000000 jewcal-0.5.1a3/src/jewcal/utils/calculations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:28:28.280654 jewcal-0.5.1a3/src/jewcal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-31 15:28:28.000000 jewcal-0.5.1a3/src/jewcal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-31 15:28:28.000000 jewcal-0.5.1a3/src/jewcal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:28:28.000000 jewcal-0.5.1a3/src/jewcal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 15:28:28.000000 jewcal-0.5.1a3/src/jewcal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-31 15:28:28.000000 jewcal-0.5.1a3/src/jewcal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 15:28:28.000000 jewcal-0.5.1a3/src/jewcal.egg-info/top_level.txt
```

### Comparing `jewcal-0.5.0/LICENSE` & `jewcal-0.5.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `jewcal-0.5.0/src/jewcal/__init__.py` & `jewcal-0.5.1a3/src/jewcal/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 """Package jewcal."""
 
+from datetime import date  # noqa: F401
 from sys import modules
 from types import ModuleType
 from typing import cast
 from warnings import warn
 
 from .core import JewCal
 
 Jewcal = JewCal
 
 
-class Wrapper:  # pylint: disable=too-few-public-methods
+class _Wrapper:  # pylint: disable=too-few-public-methods
     """Rename class `Jewcal` to `JewCal`."""
 
     def __init__(self, wrapped: ModuleType):
         self.wrapped: ModuleType = wrapped
 
     def __getattr__(self, name: str) -> ModuleType:
         if name == 'Jewcal':
             # DeprecationWarning does not alert the user if not in
             # development mode
-            warn('Class Jewcal is deprecated and renamed to JewCal')
+            warn('Jewcal is deprecated, use JewCal', stacklevel=2)
 
         return cast(ModuleType, getattr(self.wrapped, name))
 
 
-modules[__name__] = cast(ModuleType, Wrapper(modules[__name__]))
+modules[__name__] = cast(ModuleType, _Wrapper(modules[__name__]))
 
 
 __all__ = [
     'JewCal',
 ]
```

### Comparing `jewcal-0.5.0/src/jewcal/constants.py` & `jewcal-0.5.1a3/src/jewcal/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Constants."""
 
 from enum import Enum, IntEnum, unique
-from typing import NamedTuple, Optional
+from typing import NamedTuple
 
 
 @unique
 class Category(Enum):
     """Does the shabbos or yom tov start (candles) or end (havdalah)."""
 
     CANDLES = 'Candles'
@@ -31,29 +31,27 @@
     ELUL = 6
 
 
 class Event(NamedTuple):
     """Named tuple for shabbos and yom tov."""
 
     title: str
-    category: Optional[str]
+    category: str | None
 
 
 # YOMTOV[jewish_month][day]
 YOMTOV: dict[int, dict[int, Event]] = {
     6: {
         29: Event('Erev Rosh Hashana', Category.CANDLES.value),
     },
     7: {
         1: Event('Rosh Hashana 1', Category.CANDLES.value),
         2: Event('Rosh Hashana 2', Category.HAVDALAH.value),
-
         9: Event('Erev Yom Kippur', Category.CANDLES.value),
         10: Event('Yom Kippur', Category.HAVDALAH.value),
-
         14: Event('Erev Sukkos', Category.CANDLES.value),
         15: Event('Sukkos 1', Category.CANDLES.value),
         16: Event('Sukkos 2', Category.HAVDALAH.value),
         17: Event('Chol HaMoed 1 (Sukkos 3)', None),
         18: Event('Chol HaMoed 2 (Sukkos 4)', None),
         19: Event('Chol HaMoed 3 (Sukkos 5)', None),
         20: Event('Chol HaMoed 4 (Sukkos 6)', None),
@@ -82,18 +80,16 @@
 YOMTOV_ISRAEL: dict[int, dict[int, Event]] = {
     6: {
         29: Event('Erev Rosh Hashana', Category.CANDLES.value),
     },
     7: {
         1: Event('Rosh Hashana 1', Category.CANDLES.value),
         2: Event('Rosh Hashana 2', Category.HAVDALAH.value),
-
         9: Event('Erev Yom Kippur', Category.CANDLES.value),
         10: Event('Yom Kippur', Category.HAVDALAH.value),
-
         14: Event('Erev Sukkot', Category.CANDLES.value),
         15: Event('Sukkot 1', Category.HAVDALAH.value),
         16: Event('Chol HaMoed 1 (Sukkot 2)', None),
         17: Event('Chol HaMoed 2 (Sukkot 3)', None),
         18: Event('Chol HaMoed 3 (Sukkot 4)', None),
         19: Event('Chol HaMoed 4 (Sukkot 5)', None),
         20: Event('Chol HaMoed 5 (Sukkot 6)', None),
```

### Comparing `jewcal-0.5.0/src/jewcal/utils/calculations.py` & `jewcal-0.5.1a3/src/jewcal/utils/calculations.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,35 +5,40 @@
 1 BCE is 1 CE.) Thus the Gregorian date January 1, 1 CE is absolute date
 number 1.
 
 Source code Copyright © by Ulrich and David Greve (2005)
 https://www.david-greve.de/luach-code/jewish-python.html
 """
 
-from typing import Tuple
+from calendar import isleap, monthrange
+from datetime import date
+
+from jewcal.constants import Months
+
+# Calculated date of the world's creation, is equivalent to sunset on the Julian
+# proleptic calendar date 6 October 3761 BCE
+JEWISH_EPOCH = 1373429
+
+# Moon's 19 year cycle where the Moon returns to the same place
+METONIC_CYCLE = 19
 
 
 def is_gregorian_leap(year: int) -> bool:
     """Is the Gregorian year a leap year.
 
     97 leap years occur every 400 years so that every year divisible by 4 is a
     leap year, except if it is divisible by 100 and not divisible by 400.
 
     Args:
         year: The Gregorian year.
 
     Returns:
         True for leap year, False otherwise.
     """
-    return bool(all([
-        ((year % 4) == 0),
-        ((year % 400) != 100),
-        ((year % 400) != 200),
-        ((year % 400) != 300),
-    ]))
+    return isleap(year)
 
 
 def is_jewish_leap(year: int) -> bool:
     """Is the Jewish year a leap year.
 
     Jewish years have 12 months in a regular year and 13 in a leap year.
     Leap years occur on the 3rd, 6th, 8th, 11th, 14th, 17th, and 19th years of
@@ -43,48 +48,43 @@
 
     Args:
         year: The Jewish year.
 
     Returns:
         True for leap year, False otherwise.
     """
-    return bool((((year * 7) + 1) % 19) < 7)
+    return bool((((year * 7) + 1) % METONIC_CYCLE) < 7)  # noqa: PLR2004
 
 
 def days_in_gregorian_month(month: int, year: int) -> int:
     """Get the number of days in a Gregorian month.
 
     Args:
         month: The Gregorian month.
         year: The Gregorian year.
 
     Returns:
          The number of days.
     """
-    if is_gregorian_leap(year) is True and month == 2:
-        return 29
-
-    lengths = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
-    return lengths[month - 1]
+    return monthrange(year, month)[1]
 
 
 def days_in_jewish_year(year: int) -> int:
     """Get the number of days in a Jewish year.
 
     This is calculated as the difference between the elapsed days in
     successive years.
 
     Args:
         year: The Jewish year.
 
     Returns:
         The number of days.
     """
-    return (_first_day_of_jewish_year(year + 1)
-            - _first_day_of_jewish_year(year))
+    return _first_day_of_jewish_year(year + 1) - _first_day_of_jewish_year(year)
 
 
 def days_in_jewish_month(year: int, month: int) -> int:
     """Get the number of days in a Jewish month.
 
     Args:
         year: The Jewish year.
@@ -131,39 +131,15 @@
         year: The Gregorian year.
         month: The Gregorian month.
         day: The Gregorian day.
 
     Returns:
         The absolute date number.
     """
-    value = day
-    absdate = value
-
-    # days in prior months this year
-    for i in range(1, month):
-        value = days_in_gregorian_month(i, year)
-        absdate += value
-
-    # days in prior years
-    value = 365 * (year - 1)
-    absdate += value
-
-    # Julian leap days in prior years
-    value = (year - 1) // 4
-    absdate += value
-
-    # minus prior century years
-    value = (year - 1) // 100
-    absdate -= value
-
-    # plus prior years divisible by 400
-    value = (year - 1) // 400
-    absdate += value
-
-    return absdate
+    return date(year, month, day).toordinal()
 
 
 def jewish_to_absdate(year: int, month: int, day: int) -> int:
     """Convert the Jewish date to an absolute date number.
 
     Args:
         year: The Jewish year.
@@ -173,115 +149,87 @@
     Returns:
         The absolute date number.
     """
     # Days so far this month.
     value = day
     return_value = value
 
-    # If before Tishri
-    if month < 7:
+    # If before Tishrei
+    if month < Months.TISHREI:
         # add days in prior months this year before and after Nisan.
-        for i in range(7, months_in_jewish_year(year) + 1):
+        for i in range(Months.TISHREI, months_in_jewish_year(year) + 1):
             value = days_in_jewish_month(year, i)
             return_value += value
         for i in range(1, month):
             value = days_in_jewish_month(year, i)
             return_value += value
     else:
-        for i in range(7, month):
+        for i in range(Months.TISHREI, month):
             value = days_in_jewish_month(year, i)
             return_value += value
 
     # Days in prior years.
     value = _first_day_of_jewish_year(year)
     return_value += value
 
     # Days elapsed before absolute date 1.
-    value = 1373429
+    value = JEWISH_EPOCH
     return_value -= value
 
     return return_value
 
 
-def absdate_to_gregorian(absdate: int) -> Tuple[int, int, int]:
+def absdate_to_gregorian(absdate: int) -> tuple[int, int, int]:
     """Convert the absolute date number to a Gregorian date.
 
     Args:
         absdate: The absolute date number.
 
     Returns:
         A tuple with the Gregorian year, month and day.
     """
-    approx = absdate // 366
-
-    # search forward from the approximation
-    year_temp = approx
-    while 1:
-        absdate_temp = gregorian_to_absdate(year_temp + 1, 1, 1)
-        if absdate < absdate_temp:
-            break
-        year_temp += 1
-    year = year_temp
+    gregorian = date.fromordinal(absdate)
 
-    # search forward from January
-    month_temp = 1
-    while 1:
-        absdate_temp = gregorian_to_absdate(
-            year, month_temp, days_in_gregorian_month(month_temp, year))
-        if absdate <= absdate_temp:
-            break
-        month_temp += 1
-    month = month_temp
+    return (gregorian.year, gregorian.month, gregorian.day)
 
-    # calculate the day by subtraction
-    absdate_temp = gregorian_to_absdate(year, month, 1)
-    day = absdate - absdate_temp + 1
 
-    return (year, month, day)
-
-
-def absdate_to_jewish(absdate: int) -> Tuple[int, int, int]:
+def absdate_to_jewish(absdate: int) -> tuple[int, int, int]:
     """Convert the absolute date number to a Jewish date.
 
     Args:
         absdate: The absolute date number.
 
     Returns:
         A tuple with the Jewish year, month and day.
     """
-    approx = (absdate + 1373429) // 366
+    approx = (absdate + JEWISH_EPOCH) // 366
 
     year_temp = approx
     while 1:
         absdate_temp = jewish_to_absdate(year_temp + 1, 7, 1)
         if absdate < absdate_temp:
             break
         year_temp += 1
     year = year_temp
 
     absdate_temp = jewish_to_absdate(year, 1, 1)
-    if absdate < absdate_temp:
-        start = 7
-    else:
-        start = 1
+    start = 7 if absdate < absdate_temp else 1
 
     month_temp = start
     while 1:
         absdate_temp = jewish_to_absdate(
-            year,
-            month_temp,
-            days_in_jewish_month(year, month_temp)
+            year, month_temp, days_in_jewish_month(year, month_temp)
         )
         if absdate <= absdate_temp:
             break
         month_temp += 1
     month = month_temp
 
     absdate_temp = jewish_to_absdate(year, month, 1)
-    day = absdate-absdate_temp + 1
+    day = absdate - absdate_temp + 1
 
     return (year, month, day)
 
 
 def weekday_from_absdate(absdate: int) -> int:
     """Get the weekday for the absolute date number.
 
@@ -304,56 +252,64 @@
     Args:
         year: The Jewish year.
 
     Returns:
         The absolute date number.
     """
     # Months in complete cycles so far.
-    value = 235 * ((year - 1) // 19)
+    value = 235 * ((year - 1) // METONIC_CYCLE)
     months_elapsed = value
 
     # Regular months in this cycle.
-    value = 12 * ((year - 1) % 19)
+    value = 12 * ((year - 1) % METONIC_CYCLE)
     months_elapsed += value
 
     # Leap months this cycle.
-    value = ((((year - 1) % 19) * 7) + 1) // 19
+    value = ((((year - 1) % METONIC_CYCLE) * 7) + 1) // METONIC_CYCLE
 
     months_elapsed += value
 
     parts_elapsed = ((months_elapsed % 1080) * 793) + 204
 
     hours_elapsed = (
         5
         + (months_elapsed * 12)
         + ((months_elapsed // 1080) * 793)
         + (parts_elapsed // 1080)
     )
 
     # Conjunction day.
-    day = 1 + (29 * months_elapsed) + (hours_elapsed//24)
+    day = 1 + (29 * months_elapsed) + (hours_elapsed // 24)
 
     # Conjunction parts.
     parts = ((hours_elapsed % 24) * 1080) + (parts_elapsed % 1080)
 
-    if any([
-        (parts >= 19440),  # new moon is at or after midday
-
-        all([
-            ((day % 7) == 2),  # or is on a Tuesday
-            (parts >= 9924),  # and at 9 hours, 204 parts or later
-            (not is_jewish_leap(year)),  # and of a common year
-        ]),
-
-        all([
-            ((day % 7) == 1),  # or is on a Monday
-            (parts >= 16789),  # and at 15 hours, 589 parts or later
-            (is_jewish_leap(year - 1)),  # and at the end of a leap year
-        ]),
-    ]):
+    if any(
+        [
+            (parts >= 19440),  # new moon is at or after midday  # noqa: PLR2004
+            all(
+                [
+                    ((day % 7) == 2),  # or is on a Tuesday  # noqa: PLR2004
+                    (
+                        parts >= 9924  # noqa: PLR2004
+                    ),  # and at 9 hours, 204 parts or later
+                    (not is_jewish_leap(year)),  # and of a common year
+                ]
+            ),
+            all(
+                [
+                    ((day % 7) == 1),  # or is on a Monday
+                    (
+                        parts >= 16789  # noqa: PLR2004
+                    ),  # and at 15 hours, 589 parts or later
+                    (is_jewish_leap(year - 1)),  # and at the end of a leap year
+                ]
+            ),
+        ]
+    ):
         alternative_day = day + 1  # postpone Rosh Hashana one day
     else:
         alternative_day = day
 
     # if Rosh Hashana starts on Sunday, Wednesday or Friday
     if alternative_day % 7 in [0, 3, 5]:
         alternative_day += 1  # postpone it one (more) day
@@ -369,23 +325,23 @@
 
     Args:
         year: The Jewish year.
 
     Returns:
          True for long, False otherwise.
     """
-    return bool((days_in_jewish_year(year) % 10) == 5)
+    return bool((days_in_jewish_year(year) % 10) == 5)  # noqa: PLR2004
 
 
 def _is_short_kislev(year: int) -> bool:
     """Is Kislev a short month.
 
     Kislev is the ninth month of the Jewish year and the number of days can
     vary.
 
     Args:
         year: The Jewish year.
 
     Returns:
          True for short, False otherwise.
     """
-    return bool((days_in_jewish_year(year) % 10) == 3)
+    return bool((days_in_jewish_year(year) % 10) == 3)  # noqa: PLR2004
```

