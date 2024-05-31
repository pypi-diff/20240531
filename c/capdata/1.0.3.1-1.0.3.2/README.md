# Comparing `tmp/capdata-1.0.3.1.tar.gz` & `tmp/capdata-1.0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "capdata-1.0.3.1.tar", last modified: Fri May 31 03:24:26 2024, max compression
+gzip compressed data, was "capdata-1.0.3.2.tar", last modified: Fri May 31 05:34:52 2024, max compression
```

## Comparing `capdata-1.0.3.1.tar` & `capdata-1.0.3.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 03:24:26.049296 capdata-1.0.3.1/
--rw-rw-rw-   0        0        0      132 2024-05-31 03:24:26.049296 capdata-1.0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      504 2024-05-31 03:23:46.000000 capdata-1.0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 03:24:26.038760 capdata-1.0.3.1/capdata.egg-info/
--rw-rw-rw-   0        0        0      132 2024-05-31 03:24:25.000000 capdata-1.0.3.1/capdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      418 2024-05-31 03:24:25.000000 capdata-1.0.3.1/capdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 03:24:25.000000 capdata-1.0.3.1/capdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-31 03:24:25.000000 capdata-1.0.3.1/capdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 03:24:25.000000 capdata-1.0.3.1/capdata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 03:24:26.042760 capdata-1.0.3.1/data/
--rw-rw-rw-   0        0        0       39 2022-07-29 01:19:04.000000 capdata-1.0.3.1/data/__init__.py
--rw-rw-rw-   0        0        0     1318 2024-05-31 02:50:56.000000 capdata-1.0.3.1/data/curve.py
--rw-rw-rw-   0        0        0     1309 2024-05-31 02:55:42.000000 capdata-1.0.3.1/data/market.py
--rw-rw-rw-   0        0        0     1941 2024-05-31 02:55:42.000000 capdata-1.0.3.1/data/pricing.py
--rw-rw-rw-   0        0        0      920 2024-05-31 02:51:15.000000 capdata-1.0.3.1/data/refer.py
--rw-rw-rw-   0        0        0     3541 2024-05-31 02:55:42.000000 capdata-1.0.3.1/data/risk.py
-drwxrwxrwx   0        0        0        0 2024-05-31 03:24:26.043762 capdata-1.0.3.1/request/
--rw-rw-rw-   0        0        0       80 2024-05-27 10:19:49.000000 capdata-1.0.3.1/request/__init__.py
--rw-rw-rw-   0        0        0     1916 2024-05-31 01:45:57.000000 capdata-1.0.3.1/request/request.py
--rw-rw-rw-   0        0        0       42 2024-05-31 03:24:26.050303 capdata-1.0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-05-31 03:23:46.000000 capdata-1.0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 03:24:26.048760 capdata-1.0.3.1/test/
--rw-rw-rw-   0        0        0     5712 2024-05-31 03:23:13.000000 capdata-1.0.3.1/test/test_capdata.py
--rw-rw-rw-   0        0        0     1034 2024-05-31 02:42:04.000000 capdata-1.0.3.1/test/test_curve.py
--rw-rw-rw-   0        0        0      691 2024-05-31 01:45:03.000000 capdata-1.0.3.1/test/test_market.py
--rw-rw-rw-   0        0        0      975 2024-05-31 01:45:06.000000 capdata-1.0.3.1/test/test_pricing.py
--rw-rw-rw-   0        0        0     1194 2024-05-31 01:44:25.000000 capdata-1.0.3.1/test/test_refer.py
--rw-rw-rw-   0        0        0     2098 2024-05-31 01:41:43.000000 capdata-1.0.3.1/test/test_risk.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:34:52.707434 capdata-1.0.3.2/
+-rw-rw-rw-   0        0        0      132 2024-05-31 05:34:52.706435 capdata-1.0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2024-05-31 05:34:50.000000 capdata-1.0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 05:34:52.695456 capdata-1.0.3.2/capdata.egg-info/
+-rw-rw-rw-   0        0        0      132 2024-05-31 05:34:52.000000 capdata-1.0.3.2/capdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      418 2024-05-31 05:34:52.000000 capdata-1.0.3.2/capdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 05:34:52.000000 capdata-1.0.3.2/capdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-31 05:34:52.000000 capdata-1.0.3.2/capdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 05:34:52.000000 capdata-1.0.3.2/capdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 05:34:52.699434 capdata-1.0.3.2/data/
+-rw-rw-rw-   0        0        0       39 2022-07-29 01:19:04.000000 capdata-1.0.3.2/data/__init__.py
+-rw-rw-rw-   0        0        0     1318 2024-05-31 02:50:56.000000 capdata-1.0.3.2/data/curve.py
+-rw-rw-rw-   0        0        0     1309 2024-05-31 02:55:42.000000 capdata-1.0.3.2/data/market.py
+-rw-rw-rw-   0        0        0     1941 2024-05-31 02:55:42.000000 capdata-1.0.3.2/data/pricing.py
+-rw-rw-rw-   0        0        0      920 2024-05-31 02:51:15.000000 capdata-1.0.3.2/data/refer.py
+-rw-rw-rw-   0        0        0     3541 2024-05-31 02:55:42.000000 capdata-1.0.3.2/data/risk.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:34:52.701439 capdata-1.0.3.2/request/
+-rw-rw-rw-   0        0        0       80 2024-05-27 10:19:49.000000 capdata-1.0.3.2/request/__init__.py
+-rw-rw-rw-   0        0        0     1916 2024-05-31 01:45:57.000000 capdata-1.0.3.2/request/request.py
+-rw-rw-rw-   0        0        0       42 2024-05-31 05:34:52.707434 capdata-1.0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-05-31 05:34:50.000000 capdata-1.0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:34:52.705434 capdata-1.0.3.2/test/
+-rw-rw-rw-   0        0        0     5712 2024-05-31 03:23:13.000000 capdata-1.0.3.2/test/test_capdata.py
+-rw-rw-rw-   0        0        0     1034 2024-05-31 02:42:04.000000 capdata-1.0.3.2/test/test_curve.py
+-rw-rw-rw-   0        0        0      691 2024-05-31 01:45:03.000000 capdata-1.0.3.2/test/test_market.py
+-rw-rw-rw-   0        0        0      975 2024-05-31 01:45:06.000000 capdata-1.0.3.2/test/test_pricing.py
+-rw-rw-rw-   0        0        0     1194 2024-05-31 01:44:25.000000 capdata-1.0.3.2/test/test_refer.py
+-rw-rw-rw-   0        0        0     2098 2024-05-31 01:41:43.000000 capdata-1.0.3.2/test/test_risk.py
```

### Comparing `capdata-1.0.3.1/data/curve.py` & `capdata-1.0.3.2/data/curve.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.3.1/data/market.py` & `capdata-1.0.3.2/data/market.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.3.1/data/pricing.py` & `capdata-1.0.3.2/data/pricing.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.3.1/data/refer.py` & `capdata-1.0.3.2/data/refer.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.3.1/data/risk.py` & `capdata-1.0.3.2/data/risk.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.3.1/request/request.py` & `capdata-1.0.3.2/request/request.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.3.1/setup.py` & `capdata-1.0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 from sys import version_info
 
 from setuptools import setup, find_packages
 
-__version__ = '1.0.3.1'  # 版本号
+__version__ = '1.0.3.2'  # 版本号
 requirements = open('requirements.txt').readlines()  # 依赖文件
 
 if version_info < (3, 8, 0):
     raise SystemExit('Sorry! capdata requires python 3.8.0 or later.')
 
 setup(
     name='capdata',
```

### Comparing `capdata-1.0.3.1/test/test_capdata.py` & `capdata-1.0.3.2/test/test_capdata.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.3.1/test/test_curve.py` & `capdata-1.0.3.2/test/test_curve.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.3.1/test/test_market.py` & `capdata-1.0.3.2/test/test_market.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.3.1/test/test_pricing.py` & `capdata-1.0.3.2/test/test_pricing.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.3.1/test/test_refer.py` & `capdata-1.0.3.2/test/test_refer.py`

 * *Files identical despite different names*

### Comparing `capdata-1.0.3.1/test/test_risk.py` & `capdata-1.0.3.2/test/test_risk.py`

 * *Files identical despite different names*

