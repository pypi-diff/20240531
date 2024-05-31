# Comparing `tmp/ctrip-helper-0.3.1.tar.gz` & `tmp/ctrip-helper-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.3.1.tar", last modified: Fri May 31 03:04:56 2024, max compression
+gzip compressed data, was "ctrip-helper-0.3.2.tar", last modified: Fri May 31 03:41:45 2024, max compression
```

## Comparing `ctrip-helper-0.3.1.tar` & `ctrip-helper-0.3.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 03:04:56.260685 ctrip-helper-0.3.1/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-31 03:04:56.259687 ctrip-helper-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 03:04:56.245725 ctrip-helper-0.3.1/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.1/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 03:04:56.256695 ctrip-helper-0.3.1/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.1/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    30305 2024-05-31 03:04:41.000000 ctrip-helper-0.3.1/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.1/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.1/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.1/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     7033 2024-05-31 02:57:42.000000 ctrip-helper-0.3.1/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.1/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 03:04:56.258690 ctrip-helper-0.3.1/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-31 03:04:56.000000 ctrip-helper-0.3.1/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-31 03:04:56.000000 ctrip-helper-0.3.1/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 03:04:56.000000 ctrip-helper-0.3.1/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-31 03:04:56.000000 ctrip-helper-0.3.1/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 03:04:56.000000 ctrip-helper-0.3.1/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 03:04:56.260685 ctrip-helper-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-31 03:04:52.000000 ctrip-helper-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:41:45.135438 ctrip-helper-0.3.2/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-31 03:41:45.133442 ctrip-helper-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 03:41:45.114495 ctrip-helper-0.3.2/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.2/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:41:45.128457 ctrip-helper-0.3.2/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.2/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    30188 2024-05-31 03:41:17.000000 ctrip-helper-0.3.2/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.2/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.2/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.2/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     7415 2024-05-31 03:29:13.000000 ctrip-helper-0.3.2/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.2/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:41:45.131464 ctrip-helper-0.3.2/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-31 03:41:44.000000 ctrip-helper-0.3.2/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-31 03:41:45.000000 ctrip-helper-0.3.2/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 03:41:44.000000 ctrip-helper-0.3.2/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-31 03:41:44.000000 ctrip-helper-0.3.2/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 03:41:44.000000 ctrip-helper-0.3.2/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 03:41:45.135438 ctrip-helper-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-31 03:41:39.000000 ctrip-helper-0.3.2/setup.py
```

### Comparing `ctrip-helper-0.3.1/LICENSE` & `ctrip-helper-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.1/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.3.2/ctrip_helper/api/desktop_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from enum import Enum
 from decimal import Decimal
 from selenium import webdriver
 from ctrip_helper.libs import logger
 from ctrip_helper.config import url_map
 from selenium.webdriver.common.keys import Keys
 from ctrip_helper.utils import is_later_than_current_time
-from ctrip_helper.libs import get_element, click, send_keys
+from ctrip_helper.libs import get_element, send_keys, is_switch_latest_page
 
 
 class UILocatorRegx(Enum):
     all_orders_select_box = {"locator": "xpath",
                              "regx": '//ul[@class="fix_myctrip_order_layer"]//div[@class="select-box"]'}
     order_id_input_box = {"locator": "xpath", "regx": '//div[@class="order_inquiry"]//input[@id="searchBookingNum"]'}
     order_query_button = {"locator": "xpath", "regx": '//div[@class="order_inquiry"]//button[@class="btn_sel"]'}
@@ -165,15 +165,15 @@
     def is_exist_slider_verify(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         current_url = driver.current_url
         slider_verify = get_element(
             driver=driver, locator=UILocatorRegx.slider_verify.value.get("locator"),
             regx=UILocatorRegx.slider_verify.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if slider_verify:
-            logger.info("当前页面：{} 出现了滑块验证码".format(current_url))
+            logger.info("当前页：{} 出现了滑块验证码".format(current_url))
             return True
         else:
             return False
 
     @classmethod
     def open_order_query_home_with_flight(cls, driver: webdriver, sleep: float = 0) -> None:
         driver.get(url_map.get('order_query_home_with_flight'))
@@ -260,48 +260,48 @@
             logger.info("点击订单金额，进入订单详情界面")
             return True
         else:
             return False
 
     @classmethod
     def click_to_payment(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
-        current_url = driver.current_url
         local_url = "{}?oid={}".format(url_map.get("flight_order_details"), order_id)
-        if current_url.startswith(local_url) is True:
+        is_success, current_url = is_switch_latest_page(driver=driver, latest_page=local_url, loop=loop, sleep=sleep)
+        if is_success is True:
             to_payment_button = get_element(
                 driver=driver, locator=UILocatorRegx.order_to_payment.value.get("locator"),
                 regx=UILocatorRegx.order_to_payment.value.get("regx"), loop=loop, sleep=sleep, **kwargs
             )
             if to_payment_button:
                 to_payment_button.click()
                 logger.info("点击【去支付】，进入安全支付界面")
                 return True
             else:
                 return False
         else:
-            logger.warn("当前订单详情页面: {}，不是本次要支付的订单: {} 的详情页".format(current_url, order_id))
+            logger.warn("当前页: {}，不是本次要支付的订单: {} 的详情页".format(current_url, order_id))
             return False
 
     @classmethod
     def click_order_cancel(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
-        current_url = driver.current_url
         local_url = "{}?oid={}".format(url_map.get("flight_order_details"), order_id)
-        if current_url.startswith(local_url) is True:
+        is_success, current_url = is_switch_latest_page(driver=driver, latest_page=local_url, loop=loop, sleep=sleep)
+        if is_success is True:
             order_cancel_button = get_element(
                 driver=driver, locator=UILocatorRegx.order_to_cancel.value.get("locator"),
                 regx=UILocatorRegx.order_to_cancel.value.get("regx"), loop=loop, sleep=sleep, **kwargs
             )
             if order_cancel_button:
                 order_cancel_button.click()
                 logger.info("点击【取消订单】，接下来会出现【取消提示】小弹框")
                 return True
             else:
                 return False
         else:
-            logger.warn("当前订单详情页面: {}，不是本次要支付的订单: {} 的详情页".format(current_url, order_id))
+            logger.warn("当前页: {}，不是本次要支付的订单: {} 的详情页".format(current_url, order_id))
             return False
 
     @classmethod
     def click_order_continue_cancel(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         continue_cance_button = get_element(
             driver=driver, locator=UILocatorRegx.order_continue_cancel.value.get("locator"),
             regx=UILocatorRegx.order_continue_cancel.value.get("regx"), loop=loop, sleep=sleep, **kwargs
@@ -321,39 +321,29 @@
         )
         if got_it_button:
             return True
         else:
             return False
 
     @classmethod
-    def get_safe_payment_home_page(cls, driver: webdriver, loop: int = 1, sleep: float = 0) -> tuple:
-        current_url = ""
-        for _ in range(loop):
-            current_url = driver.current_url
-            if current_url.startswith(url_map.get("safe_payment_home")) is True:
-                return True, current_url
-            if sleep > 0:
-                time.sleep(sleep)
-        return False, current_url
-
-    @classmethod
     def get_order_amount_with_safe_payment_home(cls, driver: webdriver, loop: int = 1, sleep: float = 0,
                                                 **kwargs) -> Decimal:
         order_payment_amount = "0.00"
-        is_success, current_url = cls.get_safe_payment_home_page(driver=driver, loop=loop, sleep=sleep)
+        local_url = url_map.get("safe_payment_home")
+        is_success, current_url = is_switch_latest_page(driver=driver, latest_page=local_url, loop=loop, sleep=sleep)
         if is_success is True:
             order_payment_amount_element = get_element(
                 driver=driver, locator=UILocatorRegx.order_payment_amount.value.get("locator"),
                 regx=UILocatorRegx.order_payment_amount.value.get("regx"), loop=loop, sleep=sleep, **kwargs
             )
             if order_payment_amount_element:
                 order_payment_amount = order_payment_amount_element.text.strip()
                 logger.info("获取订单的支付金额为：{}".format(order_payment_amount))
         else:
-            logger.warning("当前的界面：{} 不是订单安全支付界面".format(current_url))
+            logger.warning("当前页：{} 不是订单安全支付页".format(current_url))
         return Decimal(order_payment_amount)
 
     @classmethod
     def is_cancel_order(cls, driver: webdriver, out_total_amount: str, amount_loss_limit: str, profit_cap: str,
                         passenger_number: int, platform: str, loop: int = 1, sleep: float = 0,
                         discount_amount: str = None, **kwargs) -> tuple:
         """在订单详情页，判断是否需要取消订单"""
@@ -531,30 +521,32 @@
 
     @classmethod
     def is_wallet_payment_success(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         return True
 
     @classmethod
     def enter_yeepay2b_account(cls, driver: webdriver, account: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
-        current_url = driver.current_url
-        if current_url.startswith(url_map.get("yeepay2b_cash_desk")) is True:
+        local_url = url_map.get("yeepay2b_cash_desk")
+        is_success, current_url = is_switch_latest_page(driver=driver, latest_page=local_url, loop=loop, sleep=sleep)
+        if is_success is True:
             input_box = get_element(
                 driver=driver, locator=UILocatorRegx.yeepay2b_accout_input_box.value.get("locator"),
                 regx=UILocatorRegx.yeepay2b_accout_input_box.value.get("regx"), loop=loop, sleep=sleep, **kwargs
             )
             if input_box:
                 # 模拟键盘操作清空输入框内容
                 input_box.send_keys(Keys.CONTROL + "a")  # 选中输入框中的所有内容
                 input_box.send_keys(Keys.BACKSPACE)  # 删除选中的内容
                 input_box.send_keys('{}'.format(account))
                 logger.info("输入的易宝会员账号：{}".format(account))
                 return True
             else:
                 return False
         else:
+            logger.warn("当前页: {}，不是易宝支付收银台页".format(current_url))
             return False
 
     @classmethod
     def enter_yeepay2b_password(cls, driver: webdriver, password: str, loop: int = 1, sleep: float = 0,
                                 **kwargs) -> bool:
         input_box = get_element(
             driver=driver, locator=UILocatorRegx.yeepay2b_password_input_box.value.get("locator"),
```

### Comparing `ctrip-helper-0.3.1/ctrip_helper/api/http_api.py` & `ctrip-helper-0.3.2/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.1/ctrip_helper/config.py` & `ctrip-helper-0.3.2/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.1/ctrip_helper/http_client.py` & `ctrip-helper-0.3.2/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.1/ctrip_helper/libs.py` & `ctrip-helper-0.3.2/ctrip_helper/libs.py`

 * *Files 4% similar despite different names*

```diff
@@ -180,7 +180,18 @@
         if len(diff) > 0:
             new_window = diff.pop()
             driver.switch_to.window(new_window)
             return True
         if sleep > 0:
             time.sleep(sleep)
     return False
+
+
+def is_switch_latest_page(driver: webdriver, latest_page: str, loop: int = 1, sleep: float = 0) -> tuple:
+    current_url = ""
+    for _ in range(loop):
+        current_url = driver.current_url
+        if current_url.startswith(latest_page) is True:
+            return True, current_url
+        if sleep > 0:
+            time.sleep(sleep)
+    return False, current_url
```

### Comparing `ctrip-helper-0.3.1/ctrip_helper/utils.py` & `ctrip-helper-0.3.2/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.1/setup.py` & `ctrip-helper-0.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.3.1',
+    version='0.3.2',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

