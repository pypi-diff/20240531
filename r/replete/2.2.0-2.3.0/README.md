# Comparing `tmp/replete-2.2.0.tar.gz` & `tmp/replete-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replete-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "replete-2.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `replete-2.2.0.tar` & `replete-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0       65 2024-05-27 15:27:23.915895 replete-2.2.0/.markdownlint.json
--rw-r--r--   0        0        0      569 2024-05-27 15:27:23.915895 replete-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       61 2024-05-27 15:27:23.915895 replete-2.2.0/.taplo.toml
--rw-r--r--   0        0        0       39 2024-05-27 15:27:23.915895 replete-2.2.0/.yamllint.yaml
--rw-r--r--   0        0        0    35154 2024-05-27 15:27:23.915895 replete-2.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1070 2024-05-27 15:27:23.915895 replete-2.2.0/LICENSE
--rw-r--r--   0        0        0     1853 2024-05-27 15:27:23.915895 replete-2.2.0/README.md
--rw-r--r--   0        0        0     2268 2024-05-27 15:27:23.915895 replete-2.2.0/pyproject.toml
--rw-r--r--   0        0        0      551 2024-05-27 15:27:23.915895 replete-2.2.0/replete/__init__.py
--rw-r--r--   0        0        0      593 2024-05-27 15:27:23.915895 replete-2.2.0/replete/abc.py
--rw-r--r--   0        0        0     1324 2024-05-27 15:27:23.915895 replete-2.2.0/replete/aio.py
--rw-r--r--   0        0        0    17510 2024-05-27 15:27:23.915895 replete-2.2.0/replete/cli.py
--rw-r--r--   0        0        0     3963 2024-05-27 15:27:23.915895 replete-2.2.0/replete/consistent_hash.py
--rw-r--r--   0        0        0     5253 2024-05-27 15:27:23.915895 replete-2.2.0/replete/datetime.py
--rw-r--r--   0        0        0      492 2024-05-27 15:27:23.915895 replete-2.2.0/replete/enum.py
--rw-r--r--   0        0        0     4996 2024-05-27 15:27:23.919895 replete-2.2.0/replete/funcutils.py
--rw-r--r--   0        0        0     5946 2024-05-27 15:27:23.919895 replete-2.2.0/replete/logging.py
--rw-r--r--   0        0        0     3955 2024-05-27 15:27:23.919895 replete-2.2.0/replete/register.py
--rw-r--r--   0        0        0     1291 2024-05-27 15:27:23.919895 replete-2.2.0/replete/testing.py
--rw-r--r--   0        0        0     2512 2024-05-27 15:27:23.919895 replete-2.2.0/replete/timing.py
--rw-r--r--   0        0        0     7233 2024-05-27 15:27:23.919895 replete-2.2.0/replete/utils.py
--rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 replete-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0       65 2024-05-30 22:41:27.760487 replete-2.3.0/.markdownlint.json
+-rw-r--r--   0        0        0      569 2024-05-30 22:41:27.760487 replete-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       61 2024-05-30 22:41:27.760487 replete-2.3.0/.taplo.toml
+-rw-r--r--   0        0        0       39 2024-05-30 22:41:27.760487 replete-2.3.0/.yamllint.yaml
+-rw-r--r--   0        0        0    35496 2024-05-30 22:41:27.760487 replete-2.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1070 2024-05-30 22:41:27.760487 replete-2.3.0/LICENSE
+-rw-r--r--   0        0        0     1853 2024-05-30 22:41:27.760487 replete-2.3.0/README.md
+-rw-r--r--   0        0        0     2268 2024-05-30 22:41:27.760487 replete-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      551 2024-05-30 22:41:27.760487 replete-2.3.0/replete/__init__.py
+-rw-r--r--   0        0        0      593 2024-05-30 22:41:27.760487 replete-2.3.0/replete/abc.py
+-rw-r--r--   0        0        0     1324 2024-05-30 22:41:27.760487 replete-2.3.0/replete/aio.py
+-rw-r--r--   0        0        0    17510 2024-05-30 22:41:27.760487 replete-2.3.0/replete/cli.py
+-rw-r--r--   0        0        0     3963 2024-05-30 22:41:27.764487 replete-2.3.0/replete/consistent_hash.py
+-rw-r--r--   0        0        0     5253 2024-05-30 22:41:27.764487 replete-2.3.0/replete/datetime.py
+-rw-r--r--   0        0        0      492 2024-05-30 22:41:27.764487 replete-2.3.0/replete/enum.py
+-rw-r--r--   0        0        0     2502 2024-05-30 22:41:27.764487 replete-2.3.0/replete/flock.py
+-rw-r--r--   0        0        0     4996 2024-05-30 22:41:27.764487 replete-2.3.0/replete/funcutils.py
+-rw-r--r--   0        0        0     5946 2024-05-30 22:41:27.764487 replete-2.3.0/replete/logging.py
+-rw-r--r--   0        0        0     3955 2024-05-30 22:41:27.764487 replete-2.3.0/replete/register.py
+-rw-r--r--   0        0        0     1291 2024-05-30 22:41:27.764487 replete-2.3.0/replete/testing.py
+-rw-r--r--   0        0        0     2512 2024-05-30 22:41:27.764487 replete-2.3.0/replete/timing.py
+-rw-r--r--   0        0        0     7233 2024-05-30 22:41:27.764487 replete-2.3.0/replete/utils.py
+-rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 replete-2.3.0/PKG-INFO
```

### Comparing `replete-2.2.0/.pre-commit-config.yaml` & `replete-2.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `replete-2.2.0/CHANGELOG.md` & `replete-2.3.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 # CHANGELOG
 
 
 
+## v2.3.0 (2024-05-30)
+
+### Feature
+
+* feat(flock): allow non-blocking and add re-entrant tests ([`c0a4a1f`](https://github.com/Rizhiy/replete/commit/c0a4a1f97b69c1d838e186b4f7abba5d4f5c27a6))
+
+* feat(flock): add basic filelock implementation ([`f5e88d0`](https://github.com/Rizhiy/replete/commit/f5e88d01483b0a60dab012d89d5d6b5437a3b3d9))
+
+
 ## v2.2.0 (2024-05-27)
 
 ### Chore
 
 * chore(test_and_version): add requests update to release ([`898b48a`](https://github.com/Rizhiy/replete/commit/898b48a4ef1f74bc6d608fa3e55a7d9bd65259cd))
 
 * chore: add LICENSE ([`c4ed272`](https://github.com/Rizhiy/replete/commit/c4ed272d814bf74a206ecc9ddb839e2402c463e2))
```

### Comparing `replete-2.2.0/LICENSE` & `replete-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `replete-2.2.0/README.md` & `replete-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `replete-2.2.0/pyproject.toml` & `replete-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `replete-2.2.0/replete/__init__.py` & `replete-2.3.0/replete/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 from .datetime import date_range, datetime_range, round_dt
 from .enum import ComparableEnum
 from .logging import WarnWithTraceback, assert_with_logging, setup_logging
 from .register import Register
 from .timing import RateLimiter, Timer
 from .utils import chunks, deep_update, ensure_unique_keys, grouped, split_list
 
-__version__ = "2.2.0"
+__version__ = "2.3.0"
```

### Comparing `replete-2.2.0/replete/abc.py` & `replete-2.3.0/replete/abc.py`

 * *Files identical despite different names*

### Comparing `replete-2.2.0/replete/aio.py` & `replete-2.3.0/replete/aio.py`

 * *Files identical despite different names*

### Comparing `replete-2.2.0/replete/cli.py` & `replete-2.3.0/replete/cli.py`

 * *Files identical despite different names*

### Comparing `replete-2.2.0/replete/consistent_hash.py` & `replete-2.3.0/replete/consistent_hash.py`

 * *Files identical despite different names*

### Comparing `replete-2.2.0/replete/datetime.py` & `replete-2.3.0/replete/datetime.py`

 * *Files identical despite different names*

### Comparing `replete-2.2.0/replete/funcutils.py` & `replete-2.3.0/replete/funcutils.py`

 * *Files identical despite different names*

### Comparing `replete-2.2.0/replete/logging.py` & `replete-2.3.0/replete/logging.py`

 * *Files identical despite different names*

### Comparing `replete-2.2.0/replete/register.py` & `replete-2.3.0/replete/register.py`

 * *Files identical despite different names*

### Comparing `replete-2.2.0/replete/testing.py` & `replete-2.3.0/replete/testing.py`

 * *Files identical despite different names*

### Comparing `replete-2.2.0/replete/timing.py` & `replete-2.3.0/replete/timing.py`

 * *Files identical despite different names*

### Comparing `replete-2.2.0/replete/utils.py` & `replete-2.3.0/replete/utils.py`

 * *Files identical despite different names*

### Comparing `replete-2.2.0/PKG-INFO` & `replete-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replete
-Version: 2.2.0
+Version: 2.3.0
 Summary: Assorted utilities with minimal dependencies
 Author: Anton Vasilev, Artem Vasenin
 Maintainer-email: Artem Vasenin <vasart169@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: coloredlogs
 Requires-Dist: docstring-parser
```

