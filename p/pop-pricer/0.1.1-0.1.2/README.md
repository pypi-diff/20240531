# Comparing `tmp/pop_pricer-0.1.1.tar.gz` & `tmp/pop_pricer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop_pricer-0.1.1.tar", max compression
+gzip compressed data, was "pop_pricer-0.1.2.tar", max compression
```

## Comparing `pop_pricer-0.1.1.tar` & `pop_pricer-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34522 2024-05-29 16:55:10.865652 pop_pricer-0.1.1/LICENSE.md
--rw-r--r--   0        0        0       90 2024-05-29 17:14:35.796179 pop_pricer-0.1.1/README.md
--rw-r--r--   0        0        0      138 2024-05-31 17:16:57.938928 pop_pricer-0.1.1/pop_pricer/__init__.py
--rw-r--r--   0        0        0     1524 2024-05-29 16:51:23.521880 pop_pricer-0.1.1/pop_pricer/pricer.py
--rw-r--r--   0        0        0      360 2024-05-31 19:03:47.639218 pop_pricer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 pop_pricer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    34522 2024-05-29 16:55:10.865652 pop_pricer-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0       90 2024-05-29 17:14:35.796179 pop_pricer-0.1.2/README.md
+-rw-r--r--   0        0        0      138 2024-05-31 17:16:57.938928 pop_pricer-0.1.2/pop_pricer/__init__.py
+-rw-r--r--   0        0        0     2381 2024-05-31 20:45:15.301287 pop_pricer-0.1.2/pop_pricer/pricer.py
+-rw-r--r--   0        0        0      360 2024-05-31 20:46:54.755751 pop_pricer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 pop_pricer-0.1.2/PKG-INFO
```

### Comparing `pop_pricer-0.1.1/LICENSE.md` & `pop_pricer-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pop_pricer-0.1.1/pop_pricer/pricer.py` & `pop_pricer-0.1.2/pop_pricer/pricer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from datetime import datetime, UTC
 from math import floor
+import json
 
-class PopPricer:
+class Pricer:
   def __init__(self, start_price, max_price, reset_rate=0.05, cost_weight=0.001):
     """
     """
     self._start_price = start_price
     self._max_price = max_price
     self._cost_weight = cost_weight
     self._reset_rate = reset_rate
@@ -20,14 +21,15 @@
 
   def push(self, cost):
     """
     Check current price for a given cost, to be combined with the cost weight as a multiplier of original price
     """
     return self._push_cost(cost)
 
+
   def _push_cost(self, cost):
     """
     Fetch current surge price according to sliding window, optionally incurring a new cost
     """
     if self._last_cost:
       delta = datetime.now(UTC) - self._last_cost
       self._cost = max(self._cost - delta.total_seconds() * self._reset_rate, 0)
@@ -47,9 +49,35 @@
     dec = price % 1
     if dec < 0.25:
       return round(price) - 0.01
     elif dec < 0.75:
       return floor(price) + 0.49
     else:
       return floor(price) + 0.99
+  
+  def __str__(self):
+    return self.Serializer(self).serialize()
 
-
+  class Serializer:
+    def __init__(self, pricer):
+      self._pricer = pricer
+
+    def serialize(self):
+      data = {
+        "_start_price": self._pricer._start_price,
+        "_max_price": self._pricer._max_price,
+        "_reset_rate": self._pricer._reset_rate,
+        "_cost_weight": self._pricer._cost_weight,
+        "_last_cost": self._pricer._last_cost and self._pricer._last_cost.isoformat(),
+        "_cost": self._pricer._cost
+      }
+      return json.dumps(data)
+
+    @staticmethod
+    def deserialize(str):
+      try:
+        data = json.loads(str)
+        p = Pricer(data['_start_price'], data['_max_price'], data['_reset_rate'], data['_cost_weight'])
+        p._last_cost = data['_last_cost']
+        p._cost = data['_cost']
+      except:
+        return None
```

### Comparing `pop_pricer-0.1.1/PKG-INFO` & `pop_pricer-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pop-pricer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dynamic Pricing Algorithm
 License: AGPL-3.0-only
 Author: David LoBosco
 Author-email: 5651124+dqlobo@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

