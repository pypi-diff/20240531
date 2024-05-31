# Comparing `tmp/ctrip-helper-0.3.7.tar.gz` & `tmp/ctrip-helper-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.3.7.tar", last modified: Fri May 31 09:31:19 2024, max compression
+gzip compressed data, was "ctrip-helper-0.3.8.tar", last modified: Fri May 31 09:38:41 2024, max compression
```

## Comparing `ctrip-helper-0.3.7.tar` & `ctrip-helper-0.3.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 09:31:19.565136 ctrip-helper-0.3.7/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.7/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-31 09:31:19.563142 ctrip-helper-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 09:31:19.549180 ctrip-helper-0.3.7/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.7/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:31:19.561147 ctrip-helper-0.3.7/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.7/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    32824 2024-05-31 09:31:02.000000 ctrip-helper-0.3.7/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.7/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.7/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.7/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     7415 2024-05-31 03:29:13.000000 ctrip-helper-0.3.7/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.7/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:31:19.563142 ctrip-helper-0.3.7/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-31 09:31:19.000000 ctrip-helper-0.3.7/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-31 09:31:19.000000 ctrip-helper-0.3.7/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 09:31:19.000000 ctrip-helper-0.3.7/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-31 09:31:19.000000 ctrip-helper-0.3.7/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 09:31:19.000000 ctrip-helper-0.3.7/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 09:31:19.565136 ctrip-helper-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-31 09:31:15.000000 ctrip-helper-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:38:41.000644 ctrip-helper-0.3.8/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.8/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-31 09:38:40.999647 ctrip-helper-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 09:38:40.984687 ctrip-helper-0.3.8/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.8/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:38:40.996655 ctrip-helper-0.3.8/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.8/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    33428 2024-05-31 09:38:02.000000 ctrip-helper-0.3.8/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.8/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.8/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.8/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     7415 2024-05-31 03:29:13.000000 ctrip-helper-0.3.8/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.8/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:38:40.997652 ctrip-helper-0.3.8/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-31 09:38:40.000000 ctrip-helper-0.3.8/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-31 09:38:40.000000 ctrip-helper-0.3.8/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 09:38:40.000000 ctrip-helper-0.3.8/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-31 09:38:40.000000 ctrip-helper-0.3.8/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 09:38:40.000000 ctrip-helper-0.3.8/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 09:38:41.000644 ctrip-helper-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-31 09:38:36.000000 ctrip-helper-0.3.8/setup.py
```

### Comparing `ctrip-helper-0.3.7/LICENSE` & `ctrip-helper-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.7/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.3.8/ctrip_helper/api/desktop_ui.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,16 @@
     login_button = {"locator": "xpath", "regx": '//div[@data-testid="accountPanel"]//input[@data-testid="loginButton"]'}
     slider_verify = {"locator": "xpath", "regx": '//div[@data-testid="captcha"]/div'}
     more_bank_card = {"locator": "xpath", "regx": '//div[@class="payment_trip_pay_container"]//div[@class="more_card"]'}
     bank_card = {"locator": "xpath", "regx": '//div[@class="payment_trip_pay_container"]//div[contains(text(), "{}")]'}
     bank_card_payment = {"locator": "xpath",
                          "regx": '//div[@class="payment_trip_pay_container"]//div[@class="trip-pay-btn-text"]'}
     yeepay2b_payment_success = {"locator": "xpath", "regx": '//div[@class="success-layout"]//p[@class="pay-success"]'}
+    submit_payment_result = {"locator": "xpath",
+                             "regx": '//div[contains(@class,"cds-dialog-content")]//div[contains(text(), "支付确认")]'}
 
 
 class SeleniumApi(object):
 
     @classmethod
     def is_login(cls, driver: webdriver, username: str, platform: str, loop: int = 1, sleep: float = 0,
                  **kwargs) -> bool:
@@ -579,14 +581,21 @@
         payment_success_element = get_element(
             driver=driver, locator=UILocatorRegx.yeepay2b_payment_success.value.get("locator"),
             regx=UILocatorRegx.yeepay2b_payment_success.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if payment_success_element:
             logger.info("{}订单：{}，易宝会员支付成功".format(platform, order_id))
             return True
+        submit_payment_result_element = get_element(
+            driver=driver, locator=UILocatorRegx.submit_payment_result.value.get("locator"),
+            regx=UILocatorRegx.submit_payment_result.value.get("regx"), loop=loop, sleep=sleep, **kwargs
+        )
+        if submit_payment_result_element:
+            logger.info("{}订单：{}，易宝会员支付成功".format(platform, order_id))
+            return True
         else:
             return False
 
     @classmethod
     def click_more_bank_card(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         more_bank_card_expand = get_element(
             driver=driver, locator=UILocatorRegx.more_bank_card.value.get("locator"),
```

### Comparing `ctrip-helper-0.3.7/ctrip_helper/api/http_api.py` & `ctrip-helper-0.3.8/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.7/ctrip_helper/config.py` & `ctrip-helper-0.3.8/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.7/ctrip_helper/http_client.py` & `ctrip-helper-0.3.8/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.7/ctrip_helper/libs.py` & `ctrip-helper-0.3.8/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.7/ctrip_helper/utils.py` & `ctrip-helper-0.3.8/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.7/setup.py` & `ctrip-helper-0.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.3.7',
+    version='0.3.8',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```
