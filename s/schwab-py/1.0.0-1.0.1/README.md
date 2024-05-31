# Comparing `tmp/schwab_py-1.0.0.tar.gz` & `tmp/schwab_py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab_py-1.0.0.tar", last modified: Sat May 25 12:26:01 2024, max compression
+gzip compressed data, was "schwab_py-1.0.1.tar", last modified: Fri May 31 11:49:43 2024, max compression
```

## Comparing `schwab_py-1.0.0.tar` & `schwab_py-1.0.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.532307 schwab_py-1.0.0/
--rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-05-17 12:00:12.000000 schwab_py-1.0.0/LICENSE
--rw-r--r--   0 alexgolec   (501) staff       (20)     7267 2024-05-25 12:26:01.532221 schwab_py-1.0.0/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)     5750 2024-05-17 12:00:12.000000 schwab_py-1.0.0/README.rst
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.521681 schwab_py-1.0.0/bin/
--rwxr-xr-x   0 alexgolec   (501) staff       (20)      171 2024-05-17 12:00:12.000000 schwab_py-1.0.0/bin/schwab-order-codegen.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.523699 schwab_py-1.0.0/schwab/
--rw-r--r--   0 alexgolec   (501) staff       (20)      229 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    14218 2024-05-25 12:21:55.000000 schwab_py-1.0.0/schwab/auth.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.524263 schwab_py-1.0.0/schwab/client/
--rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/client/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     1942 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/client/asynchronous.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    44924 2024-05-25 12:21:55.000000 schwab_py-1.0.0/schwab/client/base.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     1809 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/client/synchronous.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.524821 schwab_py-1.0.0/schwab/contrib/
--rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/contrib/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     9608 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/contrib/orders.py
--rw-r--r--   0 alexgolec   (501) staff       (20)      885 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/contrib/util.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     4919 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/debug.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.525888 schwab_py-1.0.0/schwab/orders/
--rw-r--r--   0 alexgolec   (501) staff       (20)      811 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/orders/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    11019 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/orders/common.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5838 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/orders/equities.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    14407 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/orders/generic.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    17650 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/orders/options.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.526314 schwab_py-1.0.0/schwab/scripts/
--rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/scripts/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     4155 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/scripts/orders_codegen.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    52329 2024-05-22 03:52:54.000000 schwab_py-1.0.0/schwab/streaming.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5149 2024-05-17 12:00:12.000000 schwab_py-1.0.0/schwab/utils.py
--rw-r--r--   0 alexgolec   (501) staff       (20)       18 2024-05-25 12:23:35.000000 schwab_py-1.0.0/schwab/version.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.531543 schwab_py-1.0.0/schwab_py.egg-info/
--rw-r--r--   0 alexgolec   (501) staff       (20)     7267 2024-05-25 12:26:01.000000 schwab_py-1.0.0/schwab_py.egg-info/PKG-INFO
--rw-r--r--   0 alexgolec   (501) staff       (20)     1129 2024-05-25 12:26:01.000000 schwab_py-1.0.0/schwab_py.egg-info/SOURCES.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-05-25 12:26:01.000000 schwab_py-1.0.0/schwab_py.egg-info/dependency_links.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      152 2024-05-25 12:26:01.000000 schwab_py-1.0.0/schwab_py.egg-info/requires.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)       13 2024-05-25 12:26:01.000000 schwab_py-1.0.0/schwab_py.egg-info/top_level.txt
--rw-r--r--   0 alexgolec   (501) staff       (20)      568 2024-05-25 12:26:01.532569 schwab_py-1.0.0/setup.cfg
--rw-r--r--   0 alexgolec   (501) staff       (20)     1904 2024-05-17 12:00:12.000000 schwab_py-1.0.0/setup.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.529487 schwab_py-1.0.0/tests/
--rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    17156 2024-05-25 12:21:55.000000 schwab_py-1.0.0/tests/auth_test.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    85571 2024-05-25 12:21:55.000000 schwab_py-1.0.0/tests/client_test.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.529990 schwab_py-1.0.0/tests/contrib/
--rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/contrib/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    30599 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/contrib/orders_test.py
--rw-r--r--   0 alexgolec   (501) staff       (20)      413 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/contrib/util_test.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     5320 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/debug_test.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.531024 schwab_py-1.0.0/tests/orders/
--rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/orders/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)      989 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/orders/common_test.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    41836 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/orders/generic_test.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    17525 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/orders/options_test.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     4624 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/orders_test.py
-drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-25 12:26:01.531304 schwab_py-1.0.0/tests/scripts/
--rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/scripts/__init__.py
--rw-r--r--   0 alexgolec   (501) staff       (20)    16623 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/scripts/orders_codegen_test.py
--rw-r--r--   0 alexgolec   (501) staff       (20)   200493 2024-05-22 03:52:54.000000 schwab_py-1.0.0/tests/streaming_test.py
--rw-r--r--   0 alexgolec   (501) staff       (20)      159 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/test.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     6591 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/utils.py
--rw-r--r--   0 alexgolec   (501) staff       (20)     3300 2024-05-17 12:00:12.000000 schwab_py-1.0.0/tests/utils_test.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-31 11:49:43.695494 schwab_py-1.0.1/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1067 2024-05-17 12:00:12.000000 schwab_py-1.0.1/LICENSE
+-rw-r--r--   0 alexgolec   (501) staff       (20)     7309 2024-05-31 11:49:43.695425 schwab_py-1.0.1/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5750 2024-05-17 12:00:12.000000 schwab_py-1.0.1/README.rst
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-31 11:49:43.683896 schwab_py-1.0.1/bin/
+-rwxr-xr-x   0 alexgolec   (501) staff       (20)      171 2024-05-17 12:00:12.000000 schwab_py-1.0.1/bin/schwab-order-codegen.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-31 11:49:43.685776 schwab_py-1.0.1/schwab/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      229 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    14286 2024-05-31 11:45:20.000000 schwab_py-1.0.1/schwab/auth.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-31 11:49:43.686433 schwab_py-1.0.1/schwab/client/
+-rw-r--r--   0 alexgolec   (501) staff       (20)       70 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/client/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1942 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/client/asynchronous.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    45050 2024-05-31 11:45:20.000000 schwab_py-1.0.1/schwab/client/base.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1809 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/client/synchronous.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-31 11:49:43.686998 schwab_py-1.0.1/schwab/contrib/
+-rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/contrib/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     9608 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/contrib/orders.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)      885 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/contrib/util.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     4919 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/debug.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-31 11:49:43.688233 schwab_py-1.0.1/schwab/orders/
+-rw-r--r--   0 alexgolec   (501) staff       (20)      811 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/orders/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    11019 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/orders/common.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5838 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/orders/equities.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    14407 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/orders/generic.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    17650 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/orders/options.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-31 11:49:43.688750 schwab_py-1.0.1/schwab/scripts/
+-rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/scripts/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     4155 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/scripts/orders_codegen.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    52329 2024-05-22 03:52:54.000000 schwab_py-1.0.1/schwab/streaming.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5149 2024-05-17 12:00:12.000000 schwab_py-1.0.1/schwab/utils.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)       18 2024-05-31 11:49:43.000000 schwab_py-1.0.1/schwab/version.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-31 11:49:43.694651 schwab_py-1.0.1/schwab_py.egg-info/
+-rw-r--r--   0 alexgolec   (501) staff       (20)     7309 2024-05-31 11:49:43.000000 schwab_py-1.0.1/schwab_py.egg-info/PKG-INFO
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1129 2024-05-31 11:49:43.000000 schwab_py-1.0.1/schwab_py.egg-info/SOURCES.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)        1 2024-05-31 11:49:43.000000 schwab_py-1.0.1/schwab_py.egg-info/dependency_links.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      163 2024-05-31 11:49:43.000000 schwab_py-1.0.1/schwab_py.egg-info/requires.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)       13 2024-05-31 11:49:43.000000 schwab_py-1.0.1/schwab_py.egg-info/top_level.txt
+-rw-r--r--   0 alexgolec   (501) staff       (20)      568 2024-05-31 11:49:43.695767 schwab_py-1.0.1/setup.cfg
+-rw-r--r--   0 alexgolec   (501) staff       (20)     1930 2024-05-26 11:25:29.000000 schwab_py-1.0.1/setup.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-31 11:49:43.692401 schwab_py-1.0.1/tests/
+-rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.1/tests/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    17232 2024-05-31 11:45:20.000000 schwab_py-1.0.1/tests/auth_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    85571 2024-05-25 12:21:55.000000 schwab_py-1.0.1/tests/client_test.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-31 11:49:43.693185 schwab_py-1.0.1/tests/contrib/
+-rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.1/tests/contrib/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    30599 2024-05-17 12:00:12.000000 schwab_py-1.0.1/tests/contrib/orders_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)      413 2024-05-17 12:00:12.000000 schwab_py-1.0.1/tests/contrib/util_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     5320 2024-05-17 12:00:12.000000 schwab_py-1.0.1/tests/debug_test.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-31 11:49:43.694159 schwab_py-1.0.1/tests/orders/
+-rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.1/tests/orders/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)      989 2024-05-17 12:00:12.000000 schwab_py-1.0.1/tests/orders/common_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    41836 2024-05-17 12:00:12.000000 schwab_py-1.0.1/tests/orders/generic_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    17525 2024-05-17 12:00:12.000000 schwab_py-1.0.1/tests/orders/options_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     4624 2024-05-17 12:00:12.000000 schwab_py-1.0.1/tests/orders_test.py
+drwxr-xr-x   0 alexgolec   (501) staff       (20)        0 2024-05-31 11:49:43.694429 schwab_py-1.0.1/tests/scripts/
+-rw-r--r--   0 alexgolec   (501) staff       (20)        0 2024-05-17 12:00:12.000000 schwab_py-1.0.1/tests/scripts/__init__.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)    16623 2024-05-17 12:00:12.000000 schwab_py-1.0.1/tests/scripts/orders_codegen_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)   200493 2024-05-22 03:52:54.000000 schwab_py-1.0.1/tests/streaming_test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)      159 2024-05-17 12:00:12.000000 schwab_py-1.0.1/tests/test.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     6591 2024-05-17 12:00:12.000000 schwab_py-1.0.1/tests/utils.py
+-rw-r--r--   0 alexgolec   (501) staff       (20)     3300 2024-05-17 12:00:12.000000 schwab_py-1.0.1/tests/utils_test.py
```

### Comparing `schwab_py-1.0.0/LICENSE` & `schwab_py-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/PKG-INFO` & `schwab_py-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial API wrapper for the Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab-py
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-py
@@ -31,14 +31,15 @@
 Provides-Extra: dev
 Requires-Dist: callee; extra == "dev"
 Requires-Dist: colorama; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: nose; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytz; extra == "dev"
+Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 
 ``schwab-py``: A Charles Schwab API Wrapper
 ===========================================
```

### Comparing `schwab_py-1.0.0/README.rst` & `schwab_py-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/schwab/auth.py` & `schwab_py-1.0.1/schwab/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,16 @@
 
     # Return a new session configured to refresh credentials
     return client_class(
         api_key,
         session_class(api_key,
                       client_secret=app_secret,
                       token=token,
-                      update_token=oauth_client_update_token),
+                      update_token=oauth_client_update_token,
+                      leeway=300),
         token_metadata=metadata_manager, enforce_enums=enforce_enums)
 
 
 def client_from_token_file(token_path, api_key, app_secret, asyncio=False,
                            enforce_enums=True):
     '''
     Returns a session from an existing token file. The session will perform
@@ -319,10 +320,11 @@
 
     return client_class(
         api_key,
         session_class(api_key,
                       client_secret=app_secret,
                       token=token,
                       token_endpoint=TOKEN_ENDPOINT,
-                      update_token=oauth_client_update_token),
+                      update_token=oauth_client_update_token,
+                      leeway=300),
         token_metadata=metadata,
         enforce_enums=enforce_enums)
```

### Comparing `schwab_py-1.0.0/schwab/client/asynchronous.py` & `schwab_py-1.0.1/schwab/client/asynchronous.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/schwab/client/base.py` & `schwab_py-1.0.1/schwab/client/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,14 +440,17 @@
     ##########################################################################
     # Quotes
 
     class Quote:
         class Fields(Enum):
             QUOTE = 'quote'
             FUNDAMENTAL = 'fundamental'
+            EXTENDED = 'extended'
+            REFERENCE = 'reference'
+            REGULAR = 'regular'
 
     def get_quote(self, symbol, *, fields=None):
         '''
         Get quote for a symbol. Note due to limitations in URL encoding, this
         method is not recommended for instruments with symbols symbols
         containing non-alphanumeric characters, for example as futures like
         ``/ES``. To get quotes for those symbols, use :meth:`Client.get_quotes`.
@@ -540,14 +543,15 @@
             JUNE = 'JUN'
             JULY = 'JUL'
             AUGUST = 'AUG'
             SEPTEMBER = 'SEP'
             OCTOBER = 'OCT'
             NOVEMBER = 'NOV'
             DECEMBER = 'DEC'
+            ALL = 'ALL'
 
         class Entitlement(Enum):
             PAYING_PRO = 'PP'
             NON_PRO = 'NP'
             NON_PAYING_PRO = 'PN'
 
     def get_option_chain(
```

### Comparing `schwab_py-1.0.0/schwab/client/synchronous.py` & `schwab_py-1.0.1/schwab/client/synchronous.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/schwab/contrib/orders.py` & `schwab_py-1.0.1/schwab/contrib/orders.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/schwab/contrib/util.py` & `schwab_py-1.0.1/schwab/contrib/util.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/schwab/debug.py` & `schwab_py-1.0.1/schwab/debug.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/schwab/orders/__init__.py` & `schwab_py-1.0.1/schwab/orders/__init__.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/schwab/orders/common.py` & `schwab_py-1.0.1/schwab/orders/common.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/schwab/orders/equities.py` & `schwab_py-1.0.1/schwab/orders/equities.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/schwab/orders/generic.py` & `schwab_py-1.0.1/schwab/orders/generic.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/schwab/orders/options.py` & `schwab_py-1.0.1/schwab/orders/options.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/schwab/scripts/orders_codegen.py` & `schwab_py-1.0.1/schwab/scripts/orders_codegen.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/schwab/streaming.py` & `schwab_py-1.0.1/schwab/streaming.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/schwab/utils.py` & `schwab_py-1.0.1/schwab/utils.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/schwab_py.egg-info/PKG-INFO` & `schwab_py-1.0.1/schwab_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-py
-Version: 1.0.0
+Version: 1.0.1
 Summary: Unofficial API wrapper for the Schwab HTTP API
 Home-page: https://github.com/alexgolec/schwab-py
 Author: Alex Golec
 Author-email: bottomless.septic.tank@gmail.com
 License: MIT
 Project-URL: Documentation, https://schwab-py.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/alexgolec/schwab-py
@@ -31,14 +31,15 @@
 Provides-Extra: dev
 Requires-Dist: callee; extra == "dev"
 Requires-Dist: colorama; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: nose; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytz; extra == "dev"
+Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: sphinx_rtd_theme; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 
 ``schwab-py``: A Charles Schwab API Wrapper
 ===========================================
```

### Comparing `schwab_py-1.0.0/schwab_py.egg-info/SOURCES.txt` & `schwab_py-1.0.1/schwab_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/setup.cfg` & `schwab_py-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/setup.py` & `schwab_py-1.0.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         'dev': [
             'callee',
             'colorama',
             'coverage',
             'nose',
             'pytest',
             'pytz',
+            'setuptools',
             'sphinx_rtd_theme',
             'twine',
             'wheel',
         ]
     },
     keywords='finance trading equities bonds options research',
     project_urls={
```

### Comparing `schwab_py-1.0.0/tests/auth_test.py` & `schwab_py-1.0.1/tests/auth_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,16 @@
         client.assert_called_once_with(API_KEY, _, token_metadata=_,
                                        enforce_enums=_)
         sync_session.assert_called_once_with(
             API_KEY,
             client_secret=APP_SECRET,
             token=self.raw_token,
             token_endpoint=_,
-            update_token=_)
+            update_token=_,
+            leeway=_)
 
     @no_duplicates
     @patch('schwab.auth.Client')
     @patch('schwab.auth.OAuth2Client', new_callable=MockOAuthClient)
     @patch('schwab.auth.AsyncOAuth2Client', new_callable=MockAsyncOAuthClient)
     def test_update_token_updates_token(
             self, async_session, sync_session, client):
@@ -150,15 +151,16 @@
                              token_write_func))
 
         sync_session.assert_called_once_with(
             API_KEY,
             client_secret=APP_SECRET,
             token=self.raw_token,
             token_endpoint=_,
-            update_token=_)
+            update_token=_,
+            leeway=_)
         token_read_func.assert_called_once()
 
         # Verify that the write function is called when the updater is called
         session_call = sync_session.mock_calls[0]
         update_token = session_call[2]['update_token']
 
         update_token(self.raw_token)
@@ -190,15 +192,16 @@
                              token_write_func))
 
         sync_session.assert_called_once_with(
             API_KEY,
             client_secret=APP_SECRET,
             token=self.raw_token,
             token_endpoint=_,
-            update_token=_)
+            update_token=_,
+            leeway=_)
         token_read_func.assert_called_once()
 
         # Verify that the write function is called when the updater is called
         session_call = sync_session.mock_calls[0]
         update_token = session_call[2]['update_token']
 
         update_token(self.raw_token)
@@ -320,15 +323,15 @@
         self.assertEqual('returned client',
                          auth.client_from_manual_flow(
                              API_KEY, APP_SECRET, REDIRECT_URL,
                              self.token_path,
                              token_write_func=dummy_token_write_func))
 
         sync_session.assert_called_with(
-                _, client_secret=APP_SECRET, token=_, update_token=_)
+                _, client_secret=APP_SECRET, token=_, update_token=_, leeway=_)
 
         self.assertEqual([{
             'creation_timestamp': MOCK_NOW,
             'token': self.raw_token
         }], token_writes)
 
     @no_duplicates
```

### Comparing `schwab_py-1.0.0/tests/client_test.py` & `schwab_py-1.0.1/tests/client_test.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/tests/contrib/orders_test.py` & `schwab_py-1.0.1/tests/contrib/orders_test.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/tests/debug_test.py` & `schwab_py-1.0.1/tests/debug_test.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/tests/orders/common_test.py` & `schwab_py-1.0.1/tests/orders/common_test.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/tests/orders/generic_test.py` & `schwab_py-1.0.1/tests/orders/generic_test.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/tests/orders/options_test.py` & `schwab_py-1.0.1/tests/orders/options_test.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/tests/orders_test.py` & `schwab_py-1.0.1/tests/orders_test.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/tests/scripts/orders_codegen_test.py` & `schwab_py-1.0.1/tests/scripts/orders_codegen_test.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/tests/streaming_test.py` & `schwab_py-1.0.1/tests/streaming_test.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/tests/utils.py` & `schwab_py-1.0.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `schwab_py-1.0.0/tests/utils_test.py` & `schwab_py-1.0.1/tests/utils_test.py`

 * *Files identical despite different names*

