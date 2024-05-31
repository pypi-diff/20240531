# Comparing `tmp/ctrip-helper-0.4.1.tar.gz` & `tmp/ctrip-helper-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.4.1.tar", last modified: Fri May 31 11:13:32 2024, max compression
+gzip compressed data, was "ctrip-helper-0.4.2.tar", last modified: Fri May 31 11:29:21 2024, max compression
```

## Comparing `ctrip-helper-0.4.1.tar` & `ctrip-helper-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 11:13:32.342522 ctrip-helper-0.4.1/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.4.1/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-31 11:13:32.341525 ctrip-helper-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 11:13:32.325340 ctrip-helper-0.4.1/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.4.1/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 11:13:32.338533 ctrip-helper-0.4.1/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.4.1/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    34330 2024-05-31 10:29:21.000000 ctrip-helper-0.4.1/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.4.1/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.4.1/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.4.1/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     9671 2024-05-31 11:13:24.000000 ctrip-helper-0.4.1/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     6305 2024-05-31 11:12:57.000000 ctrip-helper-0.4.1/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 11:13:32.340528 ctrip-helper-0.4.1/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-31 11:13:32.000000 ctrip-helper-0.4.1/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-31 11:13:32.000000 ctrip-helper-0.4.1/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 11:13:32.000000 ctrip-helper-0.4.1/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-31 11:13:32.000000 ctrip-helper-0.4.1/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 11:13:32.000000 ctrip-helper-0.4.1/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 11:13:32.342522 ctrip-helper-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-31 11:13:29.000000 ctrip-helper-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:29:21.239165 ctrip-helper-0.4.2/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-31 11:29:21.238167 ctrip-helper-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 11:29:21.223208 ctrip-helper-0.4.2/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.4.2/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:29:21.235175 ctrip-helper-0.4.2/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.4.2/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    34330 2024-05-31 10:29:21.000000 ctrip-helper-0.4.2/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.4.2/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.4.2/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.4.2/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     9973 2024-05-31 11:29:09.000000 ctrip-helper-0.4.2/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     6305 2024-05-31 11:12:57.000000 ctrip-helper-0.4.2/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:29:21.237170 ctrip-helper-0.4.2/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-31 11:29:21.000000 ctrip-helper-0.4.2/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-31 11:29:21.000000 ctrip-helper-0.4.2/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 11:29:21.000000 ctrip-helper-0.4.2/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-31 11:29:21.000000 ctrip-helper-0.4.2/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 11:29:21.000000 ctrip-helper-0.4.2/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 11:29:21.240162 ctrip-helper-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-31 11:29:16.000000 ctrip-helper-0.4.2/setup.py
```

### Comparing `ctrip-helper-0.4.1/LICENSE` & `ctrip-helper-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.1/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.4.2/ctrip_helper/api/desktop_ui.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.1/ctrip_helper/api/http_api.py` & `ctrip-helper-0.4.2/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.1/ctrip_helper/config.py` & `ctrip-helper-0.4.2/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.1/ctrip_helper/http_client.py` & `ctrip-helper-0.4.2/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.1/ctrip_helper/libs.py` & `ctrip-helper-0.4.2/ctrip_helper/libs.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,21 +198,23 @@
     return False, current_url
 
 
 def get_screenshot(driver: webdriver, file_name: str = None, **kwargs) -> tuple:
     """获取当前截屏"""
     is_ignore = kwargs.get("is_ignore", True)
     is_log_output = kwargs.get("is_log_output", True)
-    screenshot_file_name, screenshot_file_suffix = None, None
+    screenshot_file_name, screenshot_file_suffix = None, get_current_datetime_int_str()
     try:
         if file_name is None:
-            screenshot_file_suffix = get_current_datetime_int_str()
-            iname_file_name = "screenshot_{}.png".format(screenshot_file_suffix)
+            file_name = "screenshot"
         else:
-            iname_file_name = file_name
+            file_name_slice = file_name.split(".")
+            if len(file_name_slice) > 1:
+                file_name = file_name_slice[0]
+        iname_file_name = "{}_{}.png".format(file_name, screenshot_file_suffix)
         image_path = get_image_dir()
         screenshot_file_name = join_path([image_path, iname_file_name])
         driver.save_screenshot(screenshot_file_name)
     except Exception as e:
         err_str = "获取当前页面截屏失败"
         e_slice = str(e).split("Message:")
         if len(e_slice) > 0:
@@ -220,29 +222,33 @@
         if is_log_output is True:
             logger.error(err_str)
         if is_ignore is False:
             raise OverflowError(err_str)
     return screenshot_file_name, screenshot_file_suffix
 
 
-def exception_html_save_to_txt(driver: webdriver, file_name: str = None, **kwargs):
+def exception_html_save_to_txt(driver: webdriver, file_name: str = None, **kwargs) -> tuple:
     is_ignore = kwargs.get("is_ignore", True)
     is_log_output = kwargs.get("is_log_output", True)
+    exception_file_name, exception_file_suffix = None, get_current_datetime_int_str()
     try:
         if file_name is None:
-            exception_file_suffix = get_current_datetime_int_str()
-            exception_file_name = "exception_{}.html".format(exception_file_suffix)
+            file_name = "exception"
         else:
-            exception_file_name = file_name
+            file_name_slice = file_name.split(".")
+            if len(file_name_slice) > 1:
+                file_name = file_name_slice[0]
+        html_file_name = "{}_{}.html".format(file_name, exception_file_suffix)
         log_path = get_log_dir()
-        exception_file_path = join_path([log_path, exception_file_name])
-        with open(exception_file_path, "w", encoding="utf-8") as file:
+        exception_file_name = join_path([log_path, html_file_name])
+        with open(exception_file_name, "w", encoding="utf-8") as file:
             file.write(driver.page_source)
     except Exception as e:
         err_str = "页面异常内容保存至文本文件出错"
         e_slice = str(e).split("Message:")
         if len(e_slice) > 0:
             err_str = err_str + "，原因：{}".format(e_slice[0])
         if is_log_output is True:
             logger.error(err_str)
         if is_ignore is False:
             raise OverflowError(err_str)
+    return exception_file_name, exception_file_suffix
```

### Comparing `ctrip-helper-0.4.1/ctrip_helper/utils.py` & `ctrip-helper-0.4.2/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.4.1/setup.py` & `ctrip-helper-0.4.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.4.1',
+    version='0.4.2',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

