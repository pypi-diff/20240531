# Comparing `tmp/ctrip-helper-0.2.9.tar.gz` & `tmp/ctrip-helper-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.2.9.tar", last modified: Fri May 31 01:27:28 2024, max compression
+gzip compressed data, was "ctrip-helper-0.3.0.tar", last modified: Fri May 31 02:59:20 2024, max compression
```

## Comparing `ctrip-helper-0.2.9.tar` & `ctrip-helper-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 01:27:28.773069 ctrip-helper-0.2.9/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.9/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-31 01:27:28.772072 ctrip-helper-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 01:27:28.758108 ctrip-helper-0.2.9/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.9/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 01:27:28.769080 ctrip-helper-0.2.9/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.9/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    31043 2024-05-31 01:25:47.000000 ctrip-helper-0.2.9/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.9/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.9/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.9/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     6087 2024-05-31 01:15:27.000000 ctrip-helper-0.2.9/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.9/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 01:27:28.771073 ctrip-helper-0.2.9/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-31 01:27:28.000000 ctrip-helper-0.2.9/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-31 01:27:28.000000 ctrip-helper-0.2.9/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 01:27:28.000000 ctrip-helper-0.2.9/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-31 01:27:28.000000 ctrip-helper-0.2.9/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 01:27:28.000000 ctrip-helper-0.2.9/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 01:27:28.773069 ctrip-helper-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-31 01:27:13.000000 ctrip-helper-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:59:20.030461 ctrip-helper-0.3.0/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-31 02:59:20.029453 ctrip-helper-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 02:59:20.011501 ctrip-helper-0.3.0/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.0/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:59:20.026461 ctrip-helper-0.3.0/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.0/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    30304 2024-05-31 02:58:51.000000 ctrip-helper-0.3.0/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.0/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.0/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.0/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     7033 2024-05-31 02:57:42.000000 ctrip-helper-0.3.0/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.0/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:59:20.028456 ctrip-helper-0.3.0/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-31 02:59:19.000000 ctrip-helper-0.3.0/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-31 02:59:19.000000 ctrip-helper-0.3.0/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 02:59:19.000000 ctrip-helper-0.3.0/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-31 02:59:19.000000 ctrip-helper-0.3.0/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 02:59:19.000000 ctrip-helper-0.3.0/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 02:59:20.031452 ctrip-helper-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-31 02:59:15.000000 ctrip-helper-0.3.0/setup.py
```

### Comparing `ctrip-helper-0.2.9/LICENSE` & `ctrip-helper-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.9/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.3.0/ctrip_helper/api/desktop_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 import time
 from enum import Enum
 from decimal import Decimal
 from selenium import webdriver
 from ctrip_helper.libs import logger
 from ctrip_helper.config import url_map
 from selenium.webdriver.common.keys import Keys
-from ctrip_helper.libs import get_element, click
 from ctrip_helper.utils import is_later_than_current_time
+from ctrip_helper.libs import get_element, click, send_keys
 
 
 class UILocatorRegx(Enum):
     all_orders_select_box = {"locator": "xpath",
                              "regx": '//ul[@class="fix_myctrip_order_layer"]//div[@class="select-box"]'}
     order_id_input_box = {"locator": "xpath", "regx": '//div[@class="order_inquiry"]//input[@id="searchBookingNum"]'}
     order_query_button = {"locator": "xpath", "regx": '//div[@class="order_inquiry"]//button[@class="btn_sel"]'}
@@ -43,17 +43,16 @@
     use_wallet = {"locator": "xpath", "regx": '//div[@class="walelt-card"]//input[@class="am-switch-checkbox"]'}
     wallet_immediately_payment = {"locator": "xpath",
                                   "regx": '//div[@class="wallet_pay_button"]//button[@type="gradient"]'}
     use_yeepay2b_pyament = {"locator": "xpath",
                             "regx": '//div[@class="pay_way_container"]//div[contains(text(), "易宝会员支付")]'}
     yeepay2b_immediately_payment = {"locator": "xpath",
                                     "regx": '//div[@class="pay_btn_container"]//div[@class="trip-pay-btn-text"]'}
-    password_pop_box = {"locator": "xpath", "regx": '//div[@class="trip-pay-drawer-header-title"]'}
     password_input_box = {"locator": "xpath",
-                          "regx": '//div[@class="verify-password-box"]//div[@class="inputBox"]//div[{}]'}
+                          "regx": '//div[@class="verify-password-box"]//input[contains(@class, "ant-input")]'}
     yeepay2b_accout_input_box = {"locator": "xpath",
                                  "regx": '//div[@class="account-pay-main"]//input[@name="userAccount"]'}
     yeepay2b_password_input_box = {"locator": "xpath",
                                    "regx": '//div[@class="account-pay-main"]//input[@name="tradePassword"]'}
     yeepay2b_payment_next_button = {"locator": "xpath",
                                     "regx": '//div[@class="account-pay-main"]//button[@id="passPayButton"]'}
     is_login_button = {
@@ -508,35 +507,24 @@
             return True
         else:
             return False
 
     @classmethod
     def enter_payment_password(cls, driver: webdriver, password: str, loop: int = 1, sleep: float = 0,
                                **kwargs) -> bool:
-        is_exist_pop_box = get_element(
-            driver=driver, locator=UILocatorRegx.password_pop_box.value.get("locator"),
-            regx=UILocatorRegx.password_pop_box.value.get("regx"), sleep=sleep, loop=loop, **kwargs
+        password_input_box = get_element(
+            driver=driver, locator=UILocatorRegx.password_input_box.value.get("locator"),
+            regx=UILocatorRegx.password_input_box.value.get("regx"), sleep=sleep, loop=loop, **kwargs
         )
-        if is_exist_pop_box:
-            password_input_box_regx = UILocatorRegx.password_input_box.value.get("regx")
+        if password_input_box:
             if not isinstance(password, str):
                 password = str(password)
-            for index, char in enumerate(password):
-                password_input_box_regx_index = password_input_box_regx.format(index + 1)
-                password_inout_box_index = get_element(
-                    driver=driver, locator=UILocatorRegx.password_input_box.value.get("locator"),
-                    regx=password_input_box_regx_index, sleep=sleep, loop=loop, **kwargs
-                )
-                if password_inout_box_index:
-                    is_success = click(element=password_inout_box_index, loop=loop, sleep=sleep, **kwargs)
-                    if is_success is True:
-                        password_inout_box_index.send_keys(char)
-                    else:
-                        return False
-                else:
+            for char in password:
+                is_success = send_keys(element=password_input_box, char=char, loop=loop, sleep=sleep, **kwargs)
+                if is_success is False:
                     return False
                 # 可选：添加一个短暂的延迟，模拟更接近人类的输入速度
                 time.sleep(0.5)
             return True
         else:
             logger.warning("没有出现输入密码的弹框")
             return False
```

### Comparing `ctrip-helper-0.2.9/ctrip_helper/api/http_api.py` & `ctrip-helper-0.3.0/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.9/ctrip_helper/config.py` & `ctrip-helper-0.3.0/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.9/ctrip_helper/http_client.py` & `ctrip-helper-0.3.0/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.9/ctrip_helper/libs.py` & `ctrip-helper-0.3.0/ctrip_helper/libs.py`

 * *Files 18% similar despite different names*

```diff
@@ -145,14 +145,37 @@
             if is_ignore is False:
                 raise OverflowError("Element click failed, reason: {}".format(e_slice[0]))
         if sleep > 0:
             time.sleep(sleep)
     return False
 
 
+def send_keys(element: WebElement, value: str, loop: int, sleep: float, **kwargs) -> bool:
+    is_ignore = kwargs.get("is_ignore", True)
+    is_log_output = kwargs.get("is_log_output", True)
+    for _ in range(loop):
+        try:
+            element.send_keys(value)
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

### Comparing `ctrip-helper-0.2.9/ctrip_helper/utils.py` & `ctrip-helper-0.3.0/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.9/setup.py` & `ctrip-helper-0.3.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.2.9',
+    version='0.3.0',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

