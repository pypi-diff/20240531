# Comparing `tmp/ctrip-helper-0.4.0.tar.gz` & `tmp/ctrip-helper-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.4.0.tar", last modified: Fri May 31 11:08:31 2024, max compression
+gzip compressed data, was "ctrip-helper-0.4.1.tar", last modified: Fri May 31 11:13:32 2024, max compression
```

## Comparing `ctrip-helper-0.4.0.tar` & `ctrip-helper-0.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 11:08:31.207524 ctrip-helper-0.4.0/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.4.0/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-31 11:08:31.205530 ctrip-helper-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 11:08:31.190580 ctrip-helper-0.4.0/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.4.0/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 11:08:31.203535 ctrip-helper-0.4.0/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.4.0/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    34330 2024-05-31 10:29:21.000000 ctrip-helper-0.4.0/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.4.0/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.4.0/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.4.0/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     9682 2024-05-31 11:07:59.000000 ctrip-helper-0.4.0/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     5954 2024-05-31 10:59:16.000000 ctrip-helper-0.4.0/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 11:08:31.204533 ctrip-helper-0.4.0/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-31 11:08:31.000000 ctrip-helper-0.4.0/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-31 11:08:31.000000 ctrip-helper-0.4.0/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 11:08:31.000000 ctrip-helper-0.4.0/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-31 11:08:31.000000 ctrip-helper-0.4.0/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 11:08:31.000000 ctrip-helper-0.4.0/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 11:08:31.207524 ctrip-helper-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-31 11:08:22.000000 ctrip-helper-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:13:32.342522 ctrip-helper-0.4.1/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.4.1/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-31 11:13:32.341525 ctrip-helper-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 11:13:32.325340 ctrip-helper-0.4.1/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.4.1/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:13:32.338533 ctrip-helper-0.4.1/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.4.1/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    34330 2024-05-31 10:29:21.000000 ctrip-helper-0.4.1/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.4.1/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.4.1/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.4.1/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     9671 2024-05-31 11:13:24.000000 ctrip-helper-0.4.1/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     6305 2024-05-31 11:12:57.000000 ctrip-helper-0.4.1/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:13:32.340528 ctrip-helper-0.4.1/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-31 11:13:32.000000 ctrip-helper-0.4.1/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-31 11:13:32.000000 ctrip-helper-0.4.1/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 11:13:32.000000 ctrip-helper-0.4.1/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-31 11:13:32.000000 ctrip-helper-0.4.1/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 11:13:32.000000 ctrip-helper-0.4.1/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 11:13:32.342522 ctrip-helper-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-31 11:13:29.000000 ctrip-helper-0.4.1/setup.py
```

### Comparing `ctrip-helper-0.4.0/LICENSE` & `ctrip-helper-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.0/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.4.1/ctrip_helper/api/desktop_ui.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.0/ctrip_helper/api/http_api.py` & `ctrip-helper-0.4.1/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.0/ctrip_helper/config.py` & `ctrip-helper-0.4.1/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.0/ctrip_helper/http_client.py` & `ctrip-helper-0.4.1/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.0/ctrip_helper/libs.py` & `ctrip-helper-0.4.1/ctrip_helper/libs.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # FileName:     libs.py
 # Description:  TODO
 # Author:       mfkifhss2023
 # CreateDate:   2024/05/26
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
-import os
 import time
 import logging
 import typing as t
 from enum import Enum
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
```

### Comparing `ctrip-helper-0.4.0/ctrip_helper/utils.py` & `ctrip-helper-0.4.1/ctrip_helper/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -127,14 +127,29 @@
 
 def to_url_str(data: str) -> str:
     # 对JSON字符串进行URL编码，确保所有特殊字符被正确编码。
     encoded_data = urllib.parse.quote(data)
     return encoded_data
 
 
+def is_exists(file_name: t.LiteralString | str | bytes) -> bool:
+    if os.path.exists(file_name):
+        return True
+    else:
+        return False
+
+
+def is_file(file_path: str):
+    return os.path.exists(file_path) and os.path.isfile(file_path)
+
+
+def is_dir(file_path: str):
+    return os.path.exists(file_path) and os.path.isdir(file_path)
+
+
 def get_project_path():
     # 获取当前执行文件的绝对路径（兼容 Python 2 和 Python 3）
     exec_file_path = os.path.abspath(sys.argv[0])
     exec_file_path_slice = exec_file_path.split(os.path.sep)
     return os.path.sep.join(exec_file_path_slice[:-1])
 
 
@@ -151,29 +166,29 @@
     try:
         os.makedirs(dir_path, exist_ok=True)
         return True
     except OSError:
         return False
 
 
-def get_image_dir(is_created: bool = True) -> t.LiteralString | str | bytes:
+def get_image_dir() -> t.LiteralString | str | bytes:
     """
     获取image目录
-    :param bool is_created: 目录是否已创建
     :return:
     """
     path = join_path([get_project_path(), "image"])
-    if is_created is False:
+    path = path if isinstance(path, str) else str(path)
+    if is_dir(file_path=path) is False:
         create_directory(dir_path=path)
     return path
 
 
-def get_log_dir(is_created: bool = True) -> t.LiteralString | str | bytes:
+def get_log_dir() -> t.LiteralString | str | bytes:
     """
     获取日志目录
-    :param bool is_created: 目录是否已创建
     :return:
     """
     path = join_path([get_project_path(), "log"])
-    if is_created is False:
+    path = path if isinstance(path, str) else str(path)
+    if is_dir(file_path=path) is False:
         create_directory(dir_path=path)
     return path
```

### Comparing `ctrip-helper-0.4.0/setup.py` & `ctrip-helper-0.4.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.4.0',
+    version='0.4.1',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

