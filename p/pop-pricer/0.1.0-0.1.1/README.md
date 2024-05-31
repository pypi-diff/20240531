# Comparing `tmp/pop_pricer-0.1.0.tar.gz` & `tmp/pop_pricer-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pop_pricer-0.1.0.tar", max compression
+gzip compressed data, was "pop_pricer-0.1.1.tar", max compression
```

## Comparing `pop_pricer-0.1.0.tar` & `pop_pricer-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34522 2024-05-29 16:55:10.865652 pop_pricer-0.1.0/LICENSE.md
--rw-r--r--   0        0        0       90 2024-05-29 17:14:35.796179 pop_pricer-0.1.0/README.md
--rw-r--r--   0        0        0      138 2024-05-31 17:16:57.938928 pop_pricer-0.1.0/pop_pricer/__init__.py
--rw-r--r--   0        0        0     1524 2024-05-29 16:51:23.521880 pop_pricer-0.1.0/pop_pricer/pricer.py
--rw-r--r--   0        0        0      360 2024-05-31 18:29:51.902250 pop_pricer-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      665 1970-01-01 00:00:00.000000 pop_pricer-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    34522 2024-05-29 16:55:10.865652 pop_pricer-0.1.1/LICENSE.md
+-rw-r--r--   0        0        0       90 2024-05-29 17:14:35.796179 pop_pricer-0.1.1/README.md
+-rw-r--r--   0        0        0      138 2024-05-31 17:16:57.938928 pop_pricer-0.1.1/pop_pricer/__init__.py
+-rw-r--r--   0        0        0     1524 2024-05-29 16:51:23.521880 pop_pricer-0.1.1/pop_pricer/pricer.py
+-rw-r--r--   0        0        0      360 2024-05-31 19:03:47.639218 pop_pricer-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 pop_pricer-0.1.1/PKG-INFO
```

### Comparing `pop_pricer-0.1.0/LICENSE.md` & `pop_pricer-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pop_pricer-0.1.0/pop_pricer/pricer.py` & `pop_pricer-0.1.1/pop_pricer/pricer.py`

 * *Files identical despite different names*

### Comparing `pop_pricer-0.1.0/PKG-INFO` & `pop_pricer-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: pop-pricer
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dynamic Pricing Algorithm
 License: AGPL-3.0-only
 Author: David LoBosco
 Author-email: 5651124+dqlobo@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pytest (>=8.2.1,<9.0.0)
 Description-Content-Type: text/markdown
 
 Popcorn icon courtesy of [Kate Maldjian](https://thenounproject.com/creator/katemaldjian/)
```

