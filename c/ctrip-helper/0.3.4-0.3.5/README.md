# Comparing `tmp/ctrip-helper-0.3.4.tar.gz` & `tmp/ctrip-helper-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.3.4.tar", last modified: Fri May 31 03:54:57 2024, max compression
+gzip compressed data, was "ctrip-helper-0.3.5.tar", last modified: Fri May 31 07:43:07 2024, max compression
```

## Comparing `ctrip-helper-0.3.4.tar` & `ctrip-helper-0.3.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 03:54:57.261775 ctrip-helper-0.3.4/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.4/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-31 03:54:57.259780 ctrip-helper-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 03:54:57.243822 ctrip-helper-0.3.4/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.4/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 03:54:57.257785 ctrip-helper-0.3.4/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.4/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    29364 2024-05-31 03:54:46.000000 ctrip-helper-0.3.4/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.4/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.4/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.4/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     7415 2024-05-31 03:29:13.000000 ctrip-helper-0.3.4/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.4/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 03:54:57.258794 ctrip-helper-0.3.4/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-31 03:54:57.000000 ctrip-helper-0.3.4/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-31 03:54:57.000000 ctrip-helper-0.3.4/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 03:54:57.000000 ctrip-helper-0.3.4/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-31 03:54:57.000000 ctrip-helper-0.3.4/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 03:54:57.000000 ctrip-helper-0.3.4/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 03:54:57.261775 ctrip-helper-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-31 03:54:53.000000 ctrip-helper-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:43:07.300922 ctrip-helper-0.3.5/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-31 07:43:07.298931 ctrip-helper-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 07:43:07.284964 ctrip-helper-0.3.5/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.5/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:43:07.295935 ctrip-helper-0.3.5/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.5/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    31711 2024-05-31 07:42:47.000000 ctrip-helper-0.3.5/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.5/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.5/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.5/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     7415 2024-05-31 03:29:13.000000 ctrip-helper-0.3.5/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.5/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 07:43:07.297934 ctrip-helper-0.3.5/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-31 07:43:07.000000 ctrip-helper-0.3.5/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-31 07:43:07.000000 ctrip-helper-0.3.5/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 07:43:07.000000 ctrip-helper-0.3.5/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-31 07:43:07.000000 ctrip-helper-0.3.5/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 07:43:07.000000 ctrip-helper-0.3.5/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 07:43:07.300922 ctrip-helper-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-31 07:43:00.000000 ctrip-helper-0.3.5/setup.py
```

### Comparing `ctrip-helper-0.3.4/LICENSE` & `ctrip-helper-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.4/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.3.5/ctrip_helper/api/desktop_ui.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,14 +63,18 @@
                      "regx": '//div[@data-testid="accountPanel"]//input[@data-testid="accountNameInput"]'}
     password_input = {"locator": "xpath",
                       "regx": '//div[@data-testid="accountPanel"]//input[@data-testid="passwordInput"]'}
     service_agreement = {"locator": "xpath",
                          "regx": '//div[@data-testid="agreementList"]//label[@for="checkboxAgreementInput"]'}
     login_button = {"locator": "xpath", "regx": '//div[@data-testid="accountPanel"]//input[@data-testid="loginButton"]'}
     slider_verify = {"locator": "xpath", "regx": '//div[@data-testid="captcha"]/div'}
+    more_bank_card = {"locator": "xpath", "regx": '//div[@class="payment_trip_pay_container"]//div[@class="more_card"]'}
+    bank_card = {"locator": "xpath", "regx": '//div[@class="payment_trip_pay_container"]//div[contains(text(), "{}")]'}
+    bank_card_payment = {"locator": "xpath",
+                         "regx": '//div[@class="payment_trip_pay_container"]//div[@class="trip-pay-btn-text"]'}
 
 
 class SeleniumApi(object):
 
     @classmethod
     def is_login(cls, driver: webdriver, username: str, platform: str, loop: int = 1, sleep: float = 0,
                  **kwargs) -> bool:
@@ -559,7 +563,49 @@
             return True
         else:
             return False
 
     @classmethod
     def is_yeepay2b_payment_success(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         return True
+
+    @classmethod
+    def click_more_bank_card(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
+        more_bank_card_expand = get_element(
+            driver=driver, locator=UILocatorRegx.more_bank_card.value.get("locator"),
+            regx=UILocatorRegx.more_bank_card.value.get("regx"), loop=loop, sleep=sleep, **kwargs
+        )
+        if more_bank_card_expand:
+            more_bank_card_expand.click()
+            logger.info("点击【更多银行卡】")
+            return True
+        else:
+            return False
+
+    @classmethod
+    def click_bank_card(cls, driver: webdriver, payment_card: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
+        bank_card_regx = UILocatorRegx.bank_card.value.get("regx")
+        bank_card_regx = bank_card_regx.format(payment_card)
+        bank_card_element = get_element(
+            driver=driver, locator=UILocatorRegx.more_bank_card.value.get("locator"),
+            regx=bank_card_regx, loop=loop, sleep=sleep, **kwargs
+        )
+        if bank_card_element:
+            bank_card_element.click()
+            logger.info("点击选择【{}】银行卡".format(payment_card))
+            return True
+        else:
+            return False
+
+    @classmethod
+    def click_bank_card_payment(cls, driver: webdriver, payment_card: str, loop: int = 1, sleep: float = 0,
+                                **kwargs) -> bool:
+        bank_card_payment_button = get_element(
+            driver=driver, locator=UILocatorRegx.bank_card_payment.value.get("locator"),
+            regx=UILocatorRegx.bank_card_payment.value.get("regx"), loop=loop, sleep=sleep, **kwargs
+        )
+        if bank_card_payment_button:
+            bank_card_payment_button.click()
+            logger.info("点击【银行卡支付】，接下来会出现短信验证码输入框")
+            return True
+        else:
+            return False
```

### Comparing `ctrip-helper-0.3.4/ctrip_helper/api/http_api.py` & `ctrip-helper-0.3.5/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.4/ctrip_helper/config.py` & `ctrip-helper-0.3.5/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.4/ctrip_helper/http_client.py` & `ctrip-helper-0.3.5/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.4/ctrip_helper/libs.py` & `ctrip-helper-0.3.5/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.4/ctrip_helper/utils.py` & `ctrip-helper-0.3.5/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.4/setup.py` & `ctrip-helper-0.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.3.4',
+    version='0.3.5',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

