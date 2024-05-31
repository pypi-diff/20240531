# Comparing `tmp/ctrip-helper-0.3.9.tar.gz` & `tmp/ctrip-helper-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.3.9.tar", last modified: Fri May 31 10:29:47 2024, max compression
+gzip compressed data, was "ctrip-helper-0.4.0.tar", last modified: Fri May 31 11:08:31 2024, max compression
```

## Comparing `ctrip-helper-0.3.9.tar` & `ctrip-helper-0.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 10:29:47.387035 ctrip-helper-0.3.9/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.9/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-31 10:29:47.386037 ctrip-helper-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 10:29:47.370083 ctrip-helper-0.3.9/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.9/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 10:29:47.383046 ctrip-helper-0.3.9/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.9/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    34330 2024-05-31 10:29:21.000000 ctrip-helper-0.3.9/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.9/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.9/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.9/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     7415 2024-05-31 03:29:13.000000 ctrip-helper-0.3.9/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.9/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 10:29:47.385040 ctrip-helper-0.3.9/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-31 10:29:47.000000 ctrip-helper-0.3.9/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-31 10:29:47.000000 ctrip-helper-0.3.9/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 10:29:47.000000 ctrip-helper-0.3.9/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-31 10:29:47.000000 ctrip-helper-0.3.9/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 10:29:47.000000 ctrip-helper-0.3.9/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 10:29:47.388032 ctrip-helper-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-31 10:29:42.000000 ctrip-helper-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:08:31.207524 ctrip-helper-0.4.0/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-31 11:08:31.205530 ctrip-helper-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 11:08:31.190580 ctrip-helper-0.4.0/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.4.0/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:08:31.203535 ctrip-helper-0.4.0/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.4.0/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    34330 2024-05-31 10:29:21.000000 ctrip-helper-0.4.0/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.4.0/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.4.0/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.4.0/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     9682 2024-05-31 11:07:59.000000 ctrip-helper-0.4.0/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     5954 2024-05-31 10:59:16.000000 ctrip-helper-0.4.0/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:08:31.204533 ctrip-helper-0.4.0/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-31 11:08:31.000000 ctrip-helper-0.4.0/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-31 11:08:31.000000 ctrip-helper-0.4.0/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 11:08:31.000000 ctrip-helper-0.4.0/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-31 11:08:31.000000 ctrip-helper-0.4.0/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 11:08:31.000000 ctrip-helper-0.4.0/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 11:08:31.207524 ctrip-helper-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-31 11:08:22.000000 ctrip-helper-0.4.0/setup.py
```

### Comparing `ctrip-helper-0.3.9/LICENSE` & `ctrip-helper-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.9/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.4.0/ctrip_helper/api/desktop_ui.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.9/ctrip_helper/api/http_api.py` & `ctrip-helper-0.4.0/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.9/ctrip_helper/config.py` & `ctrip-helper-0.4.0/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.9/ctrip_helper/http_client.py` & `ctrip-helper-0.4.0/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.9/ctrip_helper/libs.py` & `ctrip-helper-0.4.0/ctrip_helper/libs.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,21 +5,23 @@
 # FileName:     libs.py
 # Description:  TODO
 # Author:       mfkifhss2023
 # CreateDate:   2024/05/26
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
+import os
 import time
 import logging
 import typing as t
 from enum import Enum
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
+from utils import get_current_datetime_int_str, join_path, get_image_dir, get_log_dir
 from selenium.common.exceptions import NoSuchElementException, TimeoutException, ElementNotInteractableException
 
 logger = logging.getLogger("root")
 
 
 class EnumMetaClass(Enum):
 
@@ -191,7 +193,57 @@
     for _ in range(loop):
         current_url = driver.current_url
         if current_url.startswith(latest_page) is True:
             return True, current_url
         if sleep > 0:
             time.sleep(sleep)
     return False, current_url
+
+
+def get_screenshot(driver: webdriver, file_name: str = None, **kwargs) -> tuple:
+    """获取当前截屏"""
+    is_ignore = kwargs.get("is_ignore", True)
+    is_log_output = kwargs.get("is_log_output", True)
+    screenshot_file_name, screenshot_file_suffix = None, None
+    try:
+        if file_name is None:
+            screenshot_file_suffix = get_current_datetime_int_str()
+            iname_file_name = "screenshot_{}.png".format(screenshot_file_suffix)
+        else:
+            iname_file_name = file_name
+        image_path = get_image_dir()
+        screenshot_file_name = join_path([image_path, iname_file_name])
+        driver.save_screenshot(screenshot_file_name)
+    except Exception as e:
+        err_str = "获取当前页面截屏失败"
+        e_slice = str(e).split("Message:")
+        if len(e_slice) > 0:
+            err_str = err_str + "，原因：{}".format(e_slice[0])
+        if is_log_output is True:
+            logger.error(err_str)
+        if is_ignore is False:
+            raise OverflowError(err_str)
+    return screenshot_file_name, screenshot_file_suffix
+
+
+def exception_html_save_to_txt(driver: webdriver, file_name: str = None, **kwargs):
+    is_ignore = kwargs.get("is_ignore", True)
+    is_log_output = kwargs.get("is_log_output", True)
+    try:
+        if file_name is None:
+            exception_file_suffix = get_current_datetime_int_str()
+            exception_file_name = "exception_{}.html".format(exception_file_suffix)
+        else:
+            exception_file_name = file_name
+        log_path = get_log_dir()
+        exception_file_path = join_path([log_path, exception_file_name])
+        with open(exception_file_path, "w", encoding="utf-8") as file:
+            file.write(driver.page_source)
+    except Exception as e:
+        err_str = "页面异常内容保存至文本文件出错"
+        e_slice = str(e).split("Message:")
+        if len(e_slice) > 0:
+            err_str = err_str + "，原因：{}".format(e_slice[0])
+        if is_log_output is True:
+            logger.error(err_str)
+        if is_ignore is False:
+            raise OverflowError(err_str)
```

### Comparing `ctrip-helper-0.3.9/ctrip_helper/utils.py` & `ctrip-helper-0.4.0/ctrip_helper/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,23 +6,36 @@
 # Description:  TODO
 # Author:       mfkifhss2023
 # CreateDate:   2024/05/26
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 import re
+import os
+import sys
 import json
 import random
 import hashlib
+import typing as t
 import urllib.parse
 from datetime import datetime, timedelta
 
 standard_date_format = "%Y-%m-%d %H:%M:%S"
 
 
+def get_current_datetime_int_str() -> str:
+    current_time = datetime.now()
+    # 将当前时间格式化为字符串，精确到毫秒
+    time_string = current_time.strftime('%Y-%m-%d %H:%M:%S.%f')
+    return "{}{}{}{}{}{}{}".format(
+        time_string[0:4], time_string[5:7], time_string[8:10],
+        time_string[11:13], time_string[14:16], time_string[17:19], time_string[20:23]
+    )
+
+
 def is_later_than_current_time(time_str: str, minutes: int = 5, current_dt: str = None):
     # 将给定的时间字符串转换为 datetime 对象
     given_time = datetime.strptime(time_str, '%H:%M').time()
     if current_dt is None:
         # 获取当前日期和时间
         current_datetime = datetime.now()
     else:
@@ -112,7 +125,55 @@
     return content_length
 
 
 def to_url_str(data: str) -> str:
     # 对JSON字符串进行URL编码，确保所有特殊字符被正确编码。
     encoded_data = urllib.parse.quote(data)
     return encoded_data
+
+
+def get_project_path():
+    # 获取当前执行文件的绝对路径（兼容 Python 2 和 Python 3）
+    exec_file_path = os.path.abspath(sys.argv[0])
+    exec_file_path_slice = exec_file_path.split(os.path.sep)
+    return os.path.sep.join(exec_file_path_slice[:-1])
+
+
+def join_path(path_slice: list) -> t.LiteralString | str | bytes:
+    return os.path.join(*path_slice)
+
+
+def create_directory(dir_path):
+    """
+    创建目录，如果目录不存在则创建
+    :param dir_path: 要创建的目录路径
+    :return: True（创建成功）或 False（创建失败）
+    """
+    try:
+        os.makedirs(dir_path, exist_ok=True)
+        return True
+    except OSError:
+        return False
+
+
+def get_image_dir(is_created: bool = True) -> t.LiteralString | str | bytes:
+    """
+    获取image目录
+    :param bool is_created: 目录是否已创建
+    :return:
+    """
+    path = join_path([get_project_path(), "image"])
+    if is_created is False:
+        create_directory(dir_path=path)
+    return path
+
+
+def get_log_dir(is_created: bool = True) -> t.LiteralString | str | bytes:
+    """
+    获取日志目录
+    :param bool is_created: 目录是否已创建
+    :return:
+    """
+    path = join_path([get_project_path(), "log"])
+    if is_created is False:
+        create_directory(dir_path=path)
+    return path
```

### Comparing `ctrip-helper-0.3.9/setup.py` & `ctrip-helper-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.3.9',
+    version='0.4.0',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

