# Comparing `tmp/ctrip-helper-0.3.8.tar.gz` & `tmp/ctrip-helper-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.3.8.tar", last modified: Fri May 31 09:38:41 2024, max compression
+gzip compressed data, was "ctrip-helper-0.3.9.tar", last modified: Fri May 31 10:29:47 2024, max compression
```

## Comparing `ctrip-helper-0.3.8.tar` & `ctrip-helper-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 09:38:41.000644 ctrip-helper-0.3.8/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.8/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-31 09:38:40.999647 ctrip-helper-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 09:38:40.984687 ctrip-helper-0.3.8/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.8/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:38:40.996655 ctrip-helper-0.3.8/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.8/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    33428 2024-05-31 09:38:02.000000 ctrip-helper-0.3.8/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.8/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.8/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.8/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     7415 2024-05-31 03:29:13.000000 ctrip-helper-0.3.8/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.8/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 09:38:40.997652 ctrip-helper-0.3.8/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-31 09:38:40.000000 ctrip-helper-0.3.8/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-31 09:38:40.000000 ctrip-helper-0.3.8/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 09:38:40.000000 ctrip-helper-0.3.8/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-31 09:38:40.000000 ctrip-helper-0.3.8/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 09:38:40.000000 ctrip-helper-0.3.8/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 09:38:41.000644 ctrip-helper-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-31 09:38:36.000000 ctrip-helper-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 10:29:47.387035 ctrip-helper-0.3.9/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-31 10:29:47.386037 ctrip-helper-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 10:29:47.370083 ctrip-helper-0.3.9/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.9/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 10:29:47.383046 ctrip-helper-0.3.9/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.9/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    34330 2024-05-31 10:29:21.000000 ctrip-helper-0.3.9/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.9/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.9/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.9/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     7415 2024-05-31 03:29:13.000000 ctrip-helper-0.3.9/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.9/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 10:29:47.385040 ctrip-helper-0.3.9/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-31 10:29:47.000000 ctrip-helper-0.3.9/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-31 10:29:47.000000 ctrip-helper-0.3.9/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 10:29:47.000000 ctrip-helper-0.3.9/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-31 10:29:47.000000 ctrip-helper-0.3.9/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 10:29:47.000000 ctrip-helper-0.3.9/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 10:29:47.388032 ctrip-helper-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-31 10:29:42.000000 ctrip-helper-0.3.9/setup.py
```

### Comparing `ctrip-helper-0.3.8/LICENSE` & `ctrip-helper-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.8/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.3.9/ctrip_helper/api/desktop_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,19 @@
     more_bank_card = {"locator": "xpath", "regx": '//div[@class="payment_trip_pay_container"]//div[@class="more_card"]'}
     bank_card = {"locator": "xpath", "regx": '//div[@class="payment_trip_pay_container"]//div[contains(text(), "{}")]'}
     bank_card_payment = {"locator": "xpath",
                          "regx": '//div[@class="payment_trip_pay_container"]//div[@class="trip-pay-btn-text"]'}
     yeepay2b_payment_success = {"locator": "xpath", "regx": '//div[@class="success-layout"]//p[@class="pay-success"]'}
     submit_payment_result = {"locator": "xpath",
                              "regx": '//div[contains(@class,"cds-dialog-content")]//div[contains(text(), "支付确认")]'}
+    wallet_payment_result_status = {
+        "locator": "xpath",
+        "regx": '//div[@data-testid="orderstatus_StatusWrap"]' +
+                '//div[contains(@data-testid, "orderstatus_StatusTitle_colorValue")]'
+    }
 
 
 class SeleniumApi(object):
 
     @classmethod
     def is_login(cls, driver: webdriver, username: str, platform: str, loop: int = 1, sleep: float = 0,
                  **kwargs) -> bool:
@@ -516,16 +521,29 @@
                 time.sleep(0.5)
             return True
         else:
             logger.warning("没有出现输入密码的弹框")
             return False
 
     @classmethod
-    def is_wallet_payment_success(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
-        return True
+    def is_wallet_payment_success(cls, driver: webdriver, platform: str, order_id: str, loop: int = 1, sleep: float = 0,
+                                  **kwargs) -> bool:
+        order_status_element = get_element(
+            driver=driver, locator=UILocatorRegx.wallet_payment_result_status.value.get("locator"),
+            regx=UILocatorRegx.wallet_payment_result_status.value.get("regx"), loop=loop, sleep=sleep, **kwargs
+        )
+        if order_status_element:
+            text = order_status_element.text.strip()
+            if "出票中" in text or "已出票" in text:
+                logger.info("{}订单：{}，钱包支付成功".format(platform, order_id))
+                return True
+            else:
+                return False
+        else:
+            return False
 
     @classmethod
     def enter_yeepay2b_account(cls, driver: webdriver, account: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         local_url = url_map.get("yeepay2b_cash_desk")
         is_success, current_url = is_switch_latest_page(driver=driver, latest_page=local_url, loop=loop, sleep=sleep)
         if is_success is True:
             input_box = get_element(
```

### Comparing `ctrip-helper-0.3.8/ctrip_helper/api/http_api.py` & `ctrip-helper-0.3.9/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.8/ctrip_helper/config.py` & `ctrip-helper-0.3.9/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.8/ctrip_helper/http_client.py` & `ctrip-helper-0.3.9/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.8/ctrip_helper/libs.py` & `ctrip-helper-0.3.9/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.8/ctrip_helper/utils.py` & `ctrip-helper-0.3.9/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.8/setup.py` & `ctrip-helper-0.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.3.8',
+    version='0.3.9',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

