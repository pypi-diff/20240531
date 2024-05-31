# Comparing `tmp/ctrip-helper-0.4.2.tar.gz` & `tmp/ctrip-helper-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.4.2.tar", last modified: Fri May 31 11:29:21 2024, max compression
+gzip compressed data, was "ctrip-helper-0.4.3.tar", last modified: Fri May 31 12:05:00 2024, max compression
```

## Comparing `ctrip-helper-0.4.2.tar` & `ctrip-helper-0.4.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 11:29:21.239165 ctrip-helper-0.4.2/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.4.2/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-31 11:29:21.238167 ctrip-helper-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 11:29:21.223208 ctrip-helper-0.4.2/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.4.2/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 11:29:21.235175 ctrip-helper-0.4.2/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.4.2/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    34330 2024-05-31 10:29:21.000000 ctrip-helper-0.4.2/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.4.2/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.4.2/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.4.2/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     9973 2024-05-31 11:29:09.000000 ctrip-helper-0.4.2/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     6305 2024-05-31 11:12:57.000000 ctrip-helper-0.4.2/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 11:29:21.237170 ctrip-helper-0.4.2/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-31 11:29:21.000000 ctrip-helper-0.4.2/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-31 11:29:21.000000 ctrip-helper-0.4.2/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 11:29:21.000000 ctrip-helper-0.4.2/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-31 11:29:21.000000 ctrip-helper-0.4.2/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 11:29:21.000000 ctrip-helper-0.4.2/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 11:29:21.240162 ctrip-helper-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-31 11:29:16.000000 ctrip-helper-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:05:00.081665 ctrip-helper-0.4.3/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.4.3/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-31 12:05:00.079655 ctrip-helper-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 12:05:00.065693 ctrip-helper-0.4.3/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.4.3/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:05:00.076664 ctrip-helper-0.4.3/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.4.3/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    34330 2024-05-31 10:29:21.000000 ctrip-helper-0.4.3/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.4.3/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.4.3/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.4.3/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     9986 2024-05-31 12:04:45.000000 ctrip-helper-0.4.3/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     6305 2024-05-31 11:12:57.000000 ctrip-helper-0.4.3/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:05:00.078667 ctrip-helper-0.4.3/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-31 12:04:59.000000 ctrip-helper-0.4.3/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-31 12:04:59.000000 ctrip-helper-0.4.3/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 12:04:59.000000 ctrip-helper-0.4.3/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-31 12:04:59.000000 ctrip-helper-0.4.3/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 12:04:59.000000 ctrip-helper-0.4.3/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 12:05:00.082649 ctrip-helper-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-31 12:04:54.000000 ctrip-helper-0.4.3/setup.py
```

### Comparing `ctrip-helper-0.4.2/LICENSE` & `ctrip-helper-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.2/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.4.3/ctrip_helper/api/desktop_ui.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.2/ctrip_helper/api/http_api.py` & `ctrip-helper-0.4.3/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.2/ctrip_helper/config.py` & `ctrip-helper-0.4.3/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.2/ctrip_helper/http_client.py` & `ctrip-helper-0.4.3/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.2/ctrip_helper/libs.py` & `ctrip-helper-0.4.3/ctrip_helper/libs.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import time
 import logging
 import typing as t
 from enum import Enum
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
-from utils import get_current_datetime_int_str, join_path, get_image_dir, get_log_dir
+from ctrip_helper.utils import get_current_datetime_int_str, join_path, get_image_dir, get_log_dir
 from selenium.common.exceptions import NoSuchElementException, TimeoutException, ElementNotInteractableException
 
 logger = logging.getLogger("root")
 
 
 class EnumMetaClass(Enum):
```

### Comparing `ctrip-helper-0.4.2/ctrip_helper/utils.py` & `ctrip-helper-0.4.3/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.2/setup.py` & `ctrip-helper-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.4.2',
+    version='0.4.3',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

