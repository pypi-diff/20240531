# Comparing `tmp/mozci-2.4.0.tar.gz` & `tmp/mozci-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mozci-2.4.0.tar", max compression
+gzip compressed data, was "mozci-2.4.1.tar", max compression
```

## Comparing `mozci-2.4.0.tar` & `mozci-2.4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    16725 2019-12-03 23:09:31.000000 mozci-2.4.0/LICENSE
--rw-r--r--   0        0        0      133 2020-09-01 14:24:53.000000 mozci-2.4.0/mozci/__init__.py
--rw-r--r--   0        0        0     6851 2023-05-19 09:55:23.916343 mozci-2.4.0/mozci/configuration.py
--rw-r--r--   0        0        0      925 2023-05-19 18:27:35.108952 mozci-2.4.0/mozci/console/application.py
--rw-r--r--   0        0        0    12528 2023-06-21 17:03:10.128250 mozci-2.4.0/mozci/console/commands/batch_execution.py
--rw-r--r--   0        0        0    10054 2023-07-28 14:52:07.682119 mozci-2.4.0/mozci/console/commands/check_backfills.py
--rw-r--r--   0        0        0     5549 2023-09-21 17:54:35.643850 mozci-2.4.0/mozci/console/commands/decision.py
--rw-r--r--   0        0        0    56101 2024-01-22 19:19:02.851165 mozci-2.4.0/mozci/console/commands/push.py
--rw-r--r--   0        0        0      172 2020-09-01 14:24:53.000000 mozci-2.4.0/mozci/data/__init__.py
--rw-r--r--   0        0        0     3253 2024-01-22 19:19:02.851165 mozci-2.4.0/mozci/data/base.py
--rw-r--r--   0        0        0     7307 2024-01-22 19:19:02.851165 mozci-2.4.0/mozci/data/contract.py
--rw-r--r--   0        0        0        0 2020-09-01 14:24:53.000000 mozci-2.4.0/mozci/data/sources/__init__.py
--rw-r--r--   0        0        0     4354 2023-10-01 13:48:23.201772 mozci-2.4.0/mozci/data/sources/artifact/__init__.py
--rw-r--r--   0        0        0     1884 2022-01-13 21:51:04.000000 mozci-2.4.0/mozci/data/sources/bugbug/__init__.py
--rw-r--r--   0        0        0      652 2022-01-13 21:50:58.000000 mozci-2.4.0/mozci/data/sources/hgmo/__init__.py
--rw-r--r--   0        0        0     6496 2024-01-22 19:19:02.851165 mozci-2.4.0/mozci/data/sources/taskcluster/__init__.py
--rw-r--r--   0        0        0     3419 2024-01-22 19:19:02.851165 mozci-2.4.0/mozci/data/sources/treeherder/__init__.py
--rw-r--r--   0        0        0     3135 2022-01-13 21:50:58.000000 mozci-2.4.0/mozci/errors.py
--rw-r--r--   0        0        0    61990 2024-01-22 19:19:02.851165 mozci-2.4.0/mozci/push.py
--rw-r--r--   0        0        0    25620 2024-01-22 19:19:02.851165 mozci-2.4.0/mozci/task.py
--rw-r--r--   0        0        0        0 2019-12-13 09:52:36.000000 mozci-2.4.0/mozci/util/__init__.py
--rw-r--r--   0        0        0     7772 2023-12-11 15:25:08.334847 mozci-2.4.0/mozci/util/cache_stores.py
--rw-r--r--   0        0        0      239 2023-05-19 09:55:23.926343 mozci-2.4.0/mozci/util/defs.py
--rw-r--r--   0        0        0     7168 2022-06-24 14:12:09.000000 mozci-2.4.0/mozci/util/hgmo.py
--rw-r--r--   0        0        0     1093 2020-09-01 14:24:53.000000 mozci-2.4.0/mozci/util/logging.py
--rw-r--r--   0        0        0     1585 2022-01-13 21:50:44.000000 mozci-2.4.0/mozci/util/memoize.py
--rw-r--r--   0        0        0     1023 2023-10-10 14:05:58.868523 mozci-2.4.0/mozci/util/req.py
--rw-r--r--   0        0        0     7139 2022-05-10 10:03:58.000000 mozci-2.4.0/mozci/util/taskcluster.py
--rw-r--r--   0        0        0     1087 2020-02-26 16:06:17.000000 mozci-2.4.0/mozci/util/yaml.py
--rw-r--r--   0        0        0     1174 2024-01-22 19:19:35.281160 mozci-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 mozci-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2019-12-03 23:09:31.000000 mozci-2.4.1/LICENSE
+-rw-r--r--   0        0        0      133 2020-09-01 14:24:53.000000 mozci-2.4.1/mozci/__init__.py
+-rw-r--r--   0        0        0     6851 2023-05-19 09:55:23.916343 mozci-2.4.1/mozci/configuration.py
+-rw-r--r--   0        0        0      925 2023-05-19 18:27:35.108952 mozci-2.4.1/mozci/console/application.py
+-rw-r--r--   0        0        0    12528 2023-06-21 17:03:10.128250 mozci-2.4.1/mozci/console/commands/batch_execution.py
+-rw-r--r--   0        0        0    10054 2023-07-28 14:52:07.682119 mozci-2.4.1/mozci/console/commands/check_backfills.py
+-rw-r--r--   0        0        0     5549 2023-09-21 17:54:35.643850 mozci-2.4.1/mozci/console/commands/decision.py
+-rw-r--r--   0        0        0    56101 2024-01-22 19:19:02.851165 mozci-2.4.1/mozci/console/commands/push.py
+-rw-r--r--   0        0        0      172 2020-09-01 14:24:53.000000 mozci-2.4.1/mozci/data/__init__.py
+-rw-r--r--   0        0        0     3253 2024-01-22 19:19:02.851165 mozci-2.4.1/mozci/data/base.py
+-rw-r--r--   0        0        0     7307 2024-01-22 19:19:02.851165 mozci-2.4.1/mozci/data/contract.py
+-rw-r--r--   0        0        0        0 2020-09-01 14:24:53.000000 mozci-2.4.1/mozci/data/sources/__init__.py
+-rw-r--r--   0        0        0     4354 2023-10-01 13:48:23.201772 mozci-2.4.1/mozci/data/sources/artifact/__init__.py
+-rw-r--r--   0        0        0     1884 2022-01-13 21:51:04.000000 mozci-2.4.1/mozci/data/sources/bugbug/__init__.py
+-rw-r--r--   0        0        0      652 2022-01-13 21:50:58.000000 mozci-2.4.1/mozci/data/sources/hgmo/__init__.py
+-rw-r--r--   0        0        0     6496 2024-01-22 19:19:02.851165 mozci-2.4.1/mozci/data/sources/taskcluster/__init__.py
+-rw-r--r--   0        0        0     3419 2024-01-22 19:19:02.851165 mozci-2.4.1/mozci/data/sources/treeherder/__init__.py
+-rw-r--r--   0        0        0     3135 2022-01-13 21:50:58.000000 mozci-2.4.1/mozci/errors.py
+-rw-r--r--   0        0        0    61990 2024-01-22 19:19:02.851165 mozci-2.4.1/mozci/push.py
+-rw-r--r--   0        0        0    25677 2024-05-31 08:19:11.073633 mozci-2.4.1/mozci/task.py
+-rw-r--r--   0        0        0        0 2019-12-13 09:52:36.000000 mozci-2.4.1/mozci/util/__init__.py
+-rw-r--r--   0        0        0     7772 2023-12-11 15:25:08.334847 mozci-2.4.1/mozci/util/cache_stores.py
+-rw-r--r--   0        0        0      239 2023-05-19 09:55:23.926343 mozci-2.4.1/mozci/util/defs.py
+-rw-r--r--   0        0        0     7168 2022-06-24 14:12:09.000000 mozci-2.4.1/mozci/util/hgmo.py
+-rw-r--r--   0        0        0     1093 2020-09-01 14:24:53.000000 mozci-2.4.1/mozci/util/logging.py
+-rw-r--r--   0        0        0     1585 2022-01-13 21:50:44.000000 mozci-2.4.1/mozci/util/memoize.py
+-rw-r--r--   0        0        0     1023 2023-10-10 14:05:58.868523 mozci-2.4.1/mozci/util/req.py
+-rw-r--r--   0        0        0     7139 2022-05-10 10:03:58.000000 mozci-2.4.1/mozci/util/taskcluster.py
+-rw-r--r--   0        0        0     1087 2020-02-26 16:06:17.000000 mozci-2.4.1/mozci/util/yaml.py
+-rw-r--r--   0        0        0     1174 2024-05-31 08:20:51.273616 mozci-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 mozci-2.4.1/PKG-INFO
```

### Comparing `mozci-2.4.0/LICENSE` & `mozci-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/configuration.py` & `mozci-2.4.1/mozci/configuration.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/console/application.py` & `mozci-2.4.1/mozci/console/application.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/console/commands/batch_execution.py` & `mozci-2.4.1/mozci/console/commands/batch_execution.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/console/commands/check_backfills.py` & `mozci-2.4.1/mozci/console/commands/check_backfills.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/console/commands/decision.py` & `mozci-2.4.1/mozci/console/commands/decision.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/console/commands/push.py` & `mozci-2.4.1/mozci/console/commands/push.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/data/base.py` & `mozci-2.4.1/mozci/data/base.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/data/contract.py` & `mozci-2.4.1/mozci/data/contract.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/data/sources/artifact/__init__.py` & `mozci-2.4.1/mozci/data/sources/artifact/__init__.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/data/sources/bugbug/__init__.py` & `mozci-2.4.1/mozci/data/sources/bugbug/__init__.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/data/sources/hgmo/__init__.py` & `mozci-2.4.1/mozci/data/sources/hgmo/__init__.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/data/sources/taskcluster/__init__.py` & `mozci-2.4.1/mozci/data/sources/taskcluster/__init__.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/data/sources/treeherder/__init__.py` & `mozci-2.4.1/mozci/data/sources/treeherder/__init__.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/errors.py` & `mozci-2.4.1/mozci/errors.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/push.py` & `mozci-2.4.1/mozci/push.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/task.py` & `mozci-2.4.1/mozci/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 @memoize
 def fetch_test_variant_yaml() -> Dict:
     # load variants.yml from mozilla-central
     test_variants = {}
     try:
         r = requests.get(
-            "https://hg.mozilla.org/mozilla-central/raw-file/tip/taskcluster/ci/test/variants.yml"
+            "https://hg.mozilla.org/mozilla-central/raw-file/tip/taskcluster/kinds/test/variants.yml"
         )
         tv = yaml.load(r.text, yaml.BaseLoader)
         for v in tv:
             test_variants[v] = tv[v]["suffix"]
     except requests.ConnectionError:
         raise
     return test_variants
@@ -173,14 +173,16 @@
     assert platform is not None
     retVal = f"test-{platform}"
 
     # Hack #1: Android platform names do not match
     if "android" in platform:
         platform = platform.replace("7-0", "7.0")
         retVal = f"test-{platform}"
+        if suite is None:
+            suite = "junit"
         if "junit" not in suite:
             retVal += "-geckoview"
 
     # account for the suite being replaced
     retVal += "-*"
 
     # Hack #2: wpt tasks using tag=<X> have no attributes in test-settings
```

### Comparing `mozci-2.4.0/mozci/util/cache_stores.py` & `mozci-2.4.1/mozci/util/cache_stores.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/util/hgmo.py` & `mozci-2.4.1/mozci/util/hgmo.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/util/logging.py` & `mozci-2.4.1/mozci/util/logging.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/util/memoize.py` & `mozci-2.4.1/mozci/util/memoize.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/util/req.py` & `mozci-2.4.1/mozci/util/req.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/util/taskcluster.py` & `mozci-2.4.1/mozci/util/taskcluster.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/mozci/util/yaml.py` & `mozci-2.4.1/mozci/util/yaml.py`

 * *Files identical despite different names*

### Comparing `mozci-2.4.0/pyproject.toml` & `mozci-2.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mozci"
-version = "2.4.0"
+version = "2.4.1"
 description = ""
 authors = [
   "Andrew Halberstadt <ahal@mozilla.com>",
   "Marco Castelluccio <marco@mozilla.com>",
 ]
 
 [tool.poetry.scripts]
```

### Comparing `mozci-2.4.0/PKG-INFO` & `mozci-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mozci
-Version: 2.4.0
+Version: 2.4.1
 Summary: 
 Author: Andrew Halberstadt
 Author-email: ahal@mozilla.com
 Requires-Python: >=3.7,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

