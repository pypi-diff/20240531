# Comparing `tmp/ctrip-helper-0.2.7.tar.gz` & `tmp/ctrip-helper-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.2.7.tar", last modified: Thu May 30 18:17:06 2024, max compression
+gzip compressed data, was "ctrip-helper-0.2.8.tar", last modified: Thu May 30 18:37:29 2024, max compression
```

## Comparing `ctrip-helper-0.2.7.tar` & `ctrip-helper-0.2.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 18:17:06.315632 ctrip-helper-0.2.7/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.7/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-30 18:17:06.313638 ctrip-helper-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 18:17:06.299675 ctrip-helper-0.2.7/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.7/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 18:17:06.310660 ctrip-helper-0.2.7/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.7/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    30760 2024-05-30 18:16:43.000000 ctrip-helper-0.2.7/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.7/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.7/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.7/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     5169 2024-05-30 16:53:38.000000 ctrip-helper-0.2.7/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.7/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-30 18:17:06.312641 ctrip-helper-0.2.7/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-30 18:17:06.000000 ctrip-helper-0.2.7/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-30 18:17:06.000000 ctrip-helper-0.2.7/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 18:17:06.000000 ctrip-helper-0.2.7/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-30 18:17:06.000000 ctrip-helper-0.2.7/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-30 18:17:06.000000 ctrip-helper-0.2.7/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-30 18:17:06.315632 ctrip-helper-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-30 18:17:02.000000 ctrip-helper-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:37:29.725949 ctrip-helper-0.2.8/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-30 18:37:29.724951 ctrip-helper-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-30 18:37:29.709991 ctrip-helper-0.2.8/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.2.8/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:37:29.721960 ctrip-helper-0.2.8/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.2.8/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    31452 2024-05-30 18:36:52.000000 ctrip-helper-0.2.8/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.2.8/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.2.8/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.2.8/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     5169 2024-05-30 16:53:38.000000 ctrip-helper-0.2.8/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.2.8/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 18:37:29.723967 ctrip-helper-0.2.8/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-30 18:37:29.000000 ctrip-helper-0.2.8/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-30 18:37:29.000000 ctrip-helper-0.2.8/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 18:37:29.000000 ctrip-helper-0.2.8/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-30 18:37:29.000000 ctrip-helper-0.2.8/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-30 18:37:29.000000 ctrip-helper-0.2.8/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-30 18:37:29.726946 ctrip-helper-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-30 18:37:22.000000 ctrip-helper-0.2.8/setup.py
```

### Comparing `ctrip-helper-0.2.7/LICENSE` & `ctrip-helper-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.7/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.2.8/ctrip_helper/api/desktop_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
     wallet_immediately_payment = {"locator": "xpath",
                                   "regx": '//div[@class="wallet_pay_button"]//button[@type="gradient"]'}
     use_yeepay2b_pyament = {"locator": "xpath",
                             "regx": '//div[@class="pay_way_container"]//div[contains(text(), "易宝会员支付")]'}
     yeepay2b_immediately_payment = {"locator": "xpath",
                                     "regx": '//div[@class="pay_btn_container"]//div[@class="trip-pay-btn-text"]'}
     password_pop_box = {"locator": "xpath", "regx": '//div[@class="trip-pay-drawer-header-title"]'}
-    first_password_input_box = {"locator": "xpath",
-                                "regx": '//div[@class="verify-password-box"]//div[@class="inputBox"]//div[1]'}
+    password_input_box = {"locator": "xpath",
+                          "regx": '//div[@class="verify-password-box"]//div[@class="inputBox"]//div[{}]'}
     yeepay2b_accout_input_box = {"locator": "xpath",
                                  "regx": '//div[@class="account-pay-main"]//input[@name="userAccount"]'}
     yeepay2b_password_input_box = {"locator": "xpath",
                                    "regx": '//div[@class="account-pay-main"]//input[@name="tradePassword"]'}
     yeepay2b_payment_next_button = {"locator": "xpath",
                                     "regx": '//div[@class="account-pay-main"]//button[@id="passPayButton"]'}
     is_login_button = {
@@ -513,24 +513,34 @@
     def enter_payment_password(cls, driver: webdriver, password: str, loop: int = 1, sleep: float = 0,
                                **kwargs) -> bool:
         is_exist_pop_box = get_element(
             driver=driver, locator=UILocatorRegx.password_pop_box.value.get("locator"),
             regx=UILocatorRegx.password_pop_box.value.get("regx"), sleep=sleep, loop=loop, **kwargs
         )
         if is_exist_pop_box:
+            password_input_box_regx = UILocatorRegx.password_input_box.value.get("regx")
+            first_password_input_box_regx = password_input_box_regx.format(1)
             first_password_inout_box = get_element(
-                driver=driver, locator=UILocatorRegx.first_password_input_box.value.get("locator"),
-                regx=UILocatorRegx.first_password_input_box.value.get("regx"), sleep=sleep, loop=loop, **kwargs
+                driver=driver, locator=UILocatorRegx.password_input_box.value.get("locator"),
+                regx=first_password_input_box_regx, sleep=sleep, loop=loop, **kwargs
             )
             if first_password_inout_box:
                 if not isinstance(password, str):
                     password = str(password)
                 first_password_inout_box.click()
-                for i in password:
-                    driver.send_keys(i)
+                for index, char in enumerate(password):
+                    if index == 0:
+                        first_password_inout_box.send_keys(char)
+                    else:
+                        password_input_box_regx_temp = password_input_box_regx.format(index + 1)
+                        password_inout_box_temp = get_element(
+                            driver=driver, locator=UILocatorRegx.password_input_box.value.get("locator"),
+                            regx=password_input_box_regx_temp, sleep=sleep, loop=loop, **kwargs
+                        )
+                        password_inout_box_temp.send_keys(char)
                     # 可选：添加一个短暂的延迟，模拟更接近人类的输入速度
                     time.sleep(0.5)
                 return True
             else:
                 logger.warning("查找密码输入框的第一个框失败")
                 return False
         else:
```

### Comparing `ctrip-helper-0.2.7/ctrip_helper/api/http_api.py` & `ctrip-helper-0.2.8/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.7/ctrip_helper/config.py` & `ctrip-helper-0.2.8/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.7/ctrip_helper/http_client.py` & `ctrip-helper-0.2.8/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.7/ctrip_helper/libs.py` & `ctrip-helper-0.2.8/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.7/ctrip_helper/utils.py` & `ctrip-helper-0.2.8/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.2.7/setup.py` & `ctrip-helper-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.2.7',
+    version='0.2.8',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

