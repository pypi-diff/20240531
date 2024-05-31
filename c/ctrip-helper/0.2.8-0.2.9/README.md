# Comparing `tmp/ctrip-helper-0.2.8.tar.gz` & `tmp/ctrip-helper-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.2.8.tar", last modified: Thu May 30 18:37:29 2024, max compression
+gzip compressed data, was "ctrip-helper-0.2.9.tar", last modified: Fri May 31 01:27:28 2024, max compression
```

## Comparing `ctrip-helper-0.2.8.tar` & `ctrip-helper-0.2.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 18:37:29.725949 ctrip-helper-0.2.8/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.8/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-30 18:37:29.724951 ctrip-helper-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 18:37:29.709991 ctrip-helper-0.2.8/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.8/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 18:37:29.721960 ctrip-helper-0.2.8/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.8/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    31452 2024-05-30 18:36:52.000000 ctrip-helper-0.2.8/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.8/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.8/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.8/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     5169 2024-05-30 16:53:38.000000 ctrip-helper-0.2.8/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.8/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 18:37:29.723967 ctrip-helper-0.2.8/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-30 18:37:29.000000 ctrip-helper-0.2.8/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-30 18:37:29.000000 ctrip-helper-0.2.8/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 18:37:29.000000 ctrip-helper-0.2.8/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-30 18:37:29.000000 ctrip-helper-0.2.8/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-30 18:37:29.000000 ctrip-helper-0.2.8/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 18:37:29.726946 ctrip-helper-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-30 18:37:22.000000 ctrip-helper-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:27:28.773069 ctrip-helper-0.2.9/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-31 01:27:28.772072 ctrip-helper-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 01:27:28.758108 ctrip-helper-0.2.9/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.9/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:27:28.769080 ctrip-helper-0.2.9/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.9/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    31043 2024-05-31 01:25:47.000000 ctrip-helper-0.2.9/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.9/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.9/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.9/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     6087 2024-05-31 01:15:27.000000 ctrip-helper-0.2.9/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.9/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 01:27:28.771073 ctrip-helper-0.2.9/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-31 01:27:28.000000 ctrip-helper-0.2.9/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-31 01:27:28.000000 ctrip-helper-0.2.9/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 01:27:28.000000 ctrip-helper-0.2.9/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-31 01:27:28.000000 ctrip-helper-0.2.9/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 01:27:28.000000 ctrip-helper-0.2.9/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 01:27:28.773069 ctrip-helper-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-31 01:27:13.000000 ctrip-helper-0.2.9/setup.py
```

### Comparing `ctrip-helper-0.2.8/LICENSE` & `ctrip-helper-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.8/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.2.9/ctrip_helper/api/desktop_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import re
 import time
 from enum import Enum
 from decimal import Decimal
 from selenium import webdriver
 from ctrip_helper.libs import logger
 from ctrip_helper.config import url_map
-from ctrip_helper.libs import get_element
 from selenium.webdriver.common.keys import Keys
+from ctrip_helper.libs import get_element, click
 from ctrip_helper.utils import is_later_than_current_time
 
 
 class UILocatorRegx(Enum):
     all_orders_select_box = {"locator": "xpath",
                              "regx": '//ul[@class="fix_myctrip_order_layer"]//div[@class="select-box"]'}
     order_id_input_box = {"locator": "xpath", "regx": '//div[@class="order_inquiry"]//input[@id="searchBookingNum"]'}
@@ -514,39 +514,33 @@
                                **kwargs) -> bool:
         is_exist_pop_box = get_element(
             driver=driver, locator=UILocatorRegx.password_pop_box.value.get("locator"),
             regx=UILocatorRegx.password_pop_box.value.get("regx"), sleep=sleep, loop=loop, **kwargs
         )
         if is_exist_pop_box:
             password_input_box_regx = UILocatorRegx.password_input_box.value.get("regx")
-            first_password_input_box_regx = password_input_box_regx.format(1)
-            first_password_inout_box = get_element(
-                driver=driver, locator=UILocatorRegx.password_input_box.value.get("locator"),
-                regx=first_password_input_box_regx, sleep=sleep, loop=loop, **kwargs
-            )
-            if first_password_inout_box:
-                if not isinstance(password, str):
-                    password = str(password)
-                first_password_inout_box.click()
-                for index, char in enumerate(password):
-                    if index == 0:
-                        first_password_inout_box.send_keys(char)
+            if not isinstance(password, str):
+                password = str(password)
+            for index, char in enumerate(password):
+                password_input_box_regx_index = password_input_box_regx.format(index + 1)
+                password_inout_box_index = get_element(
+                    driver=driver, locator=UILocatorRegx.password_input_box.value.get("locator"),
+                    regx=password_input_box_regx_index, sleep=sleep, loop=loop, **kwargs
+                )
+                if password_inout_box_index:
+                    is_success = click(element=password_inout_box_index, loop=loop, sleep=sleep, **kwargs)
+                    if is_success is True:
+                        password_inout_box_index.send_keys(char)
                     else:
-                        password_input_box_regx_temp = password_input_box_regx.format(index + 1)
-                        password_inout_box_temp = get_element(
-                            driver=driver, locator=UILocatorRegx.password_input_box.value.get("locator"),
-                            regx=password_input_box_regx_temp, sleep=sleep, loop=loop, **kwargs
-                        )
-                        password_inout_box_temp.send_keys(char)
-                    # 可选：添加一个短暂的延迟，模拟更接近人类的输入速度
-                    time.sleep(0.5)
-                return True
-            else:
-                logger.warning("查找密码输入框的第一个框失败")
-                return False
+                        return False
+                else:
+                    return False
+                # 可选：添加一个短暂的延迟，模拟更接近人类的输入速度
+                time.sleep(0.5)
+            return True
         else:
             logger.warning("没有出现输入密码的弹框")
             return False
 
     @classmethod
     def is_wallet_payment_success(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         return True
```

### Comparing `ctrip-helper-0.2.8/ctrip_helper/api/http_api.py` & `ctrip-helper-0.2.9/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.8/ctrip_helper/config.py` & `ctrip-helper-0.2.9/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.8/ctrip_helper/http_client.py` & `ctrip-helper-0.2.9/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.8/ctrip_helper/libs.py` & `ctrip-helper-0.2.9/ctrip_helper/libs.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import time
 import logging
 import typing as t
 from enum import Enum
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
-from selenium.common.exceptions import NoSuchElementException, TimeoutException
+from selenium.common.exceptions import NoSuchElementException, TimeoutException, ElementNotInteractableException
 
 logger = logging.getLogger("root")
 
 
 class EnumMetaClass(Enum):
 
     @classmethod
@@ -73,15 +73,14 @@
             if is_ignore is False:
                 raise NoSuchElementException()
         except (TimeoutException,):
             if is_log_output is True:
                 logger.error("Element found timeout")
             if is_ignore is False:
                 raise TimeoutException()
-            pass
         except Exception as e:
             err_str = "通过选择器：{}，表达式: {}，判断元素是否存在失败".format(locator, regx)
             e_slice = str(e).split("Message:")
             if e_slice[0]:
                 err_str = err_str + "，error: {}".format(e_slice[0])
             if is_log_output is True:
                 logger.error(err_str)
@@ -109,29 +108,51 @@
             if is_ignore is False:
                 raise NoSuchElementException()
         except (TimeoutException,):
             if is_log_output is True:
                 logger.error("Element found timeout")
             if is_ignore is False:
                 raise TimeoutException()
-            pass
         except Exception as e:
             err_str = "通过选择器：{}，表达式: {}，获取元素失败".format(locator, regx)
             e_slice = str(e).split("Message:")
             if e_slice[0]:
                 err_str = err_str + "，error: {}".format(e_slice[0])
             if is_log_output is True:
                 logger.error(err_str)
             if is_ignore is False:
                 raise OverflowError("Element found failed, reason: {}".format(err_str))
         if sleep > 0:
             time.sleep(sleep)
     return element
 
 
+def click(element: WebElement, loop: int, sleep: float, **kwargs) -> bool:
+    is_ignore = kwargs.get("is_ignore", True)
+    is_log_output = kwargs.get("is_log_output", True)
+    for _ in range(loop):
+        try:
+            element.click()
+            return True
+        except (ElementNotInteractableException,):
+            if is_log_output is True:
+                logger.error("Waiting for element to become interactive")
+            if is_ignore is False:
+                raise RuntimeError("Waiting for element to become interactive")
+        except Exception as e:
+            e_slice = str(e).split("Message:")
+            if is_log_output is True:
+                logger.error(e_slice[0])
+            if is_ignore is False:
+                raise OverflowError("Element click failed, reason: {}".format(e_slice[0]))
+        if sleep > 0:
+            time.sleep(sleep)
+    return False
+
+
 def switch_to_window(driver: webdriver, origin_windows: list, loop: int, sleep: float) -> bool:
     for i in range(loop):
         # 获取所有的窗口句柄
         all_windows = driver.window_handles
         diff = set(all_windows).difference(set(origin_windows))
         if len(diff) > 0:
             new_window = diff.pop()
```

### Comparing `ctrip-helper-0.2.8/ctrip_helper/utils.py` & `ctrip-helper-0.2.9/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.8/setup.py` & `ctrip-helper-0.2.9/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.2.8',
+    version='0.2.9',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

