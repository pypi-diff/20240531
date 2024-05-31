# Comparing `tmp/ctrip-helper-0.3.2.tar.gz` & `tmp/ctrip-helper-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.3.2.tar", last modified: Fri May 31 03:41:45 2024, max compression
+gzip compressed data, was "ctrip-helper-0.3.3.tar", last modified: Fri May 31 03:53:28 2024, max compression
```

## Comparing `ctrip-helper-0.3.2.tar` & `ctrip-helper-0.3.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 03:41:45.135438 ctrip-helper-0.3.2/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.2/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-31 03:41:45.133442 ctrip-helper-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 03:41:45.114495 ctrip-helper-0.3.2/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.2/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 03:41:45.128457 ctrip-helper-0.3.2/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.2/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    30188 2024-05-31 03:41:17.000000 ctrip-helper-0.3.2/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.2/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.2/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.2/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     7415 2024-05-31 03:29:13.000000 ctrip-helper-0.3.2/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.2/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 03:41:45.131464 ctrip-helper-0.3.2/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-31 03:41:44.000000 ctrip-helper-0.3.2/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-31 03:41:45.000000 ctrip-helper-0.3.2/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 03:41:44.000000 ctrip-helper-0.3.2/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-31 03:41:44.000000 ctrip-helper-0.3.2/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 03:41:44.000000 ctrip-helper-0.3.2/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 03:41:45.135438 ctrip-helper-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-31 03:41:39.000000 ctrip-helper-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:53:28.545987 ctrip-helper-0.3.3/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-31 03:53:28.544990 ctrip-helper-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 03:53:28.528034 ctrip-helper-0.3.3/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.3/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:53:28.540999 ctrip-helper-0.3.3/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.3/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    29364 2024-05-31 03:53:09.000000 ctrip-helper-0.3.3/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.3/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.3/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.3/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     7415 2024-05-31 03:29:13.000000 ctrip-helper-0.3.3/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.3/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:53:28.542994 ctrip-helper-0.3.3/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-31 03:53:28.000000 ctrip-helper-0.3.3/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-31 03:53:28.000000 ctrip-helper-0.3.3/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 03:53:28.000000 ctrip-helper-0.3.3/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-31 03:53:28.000000 ctrip-helper-0.3.3/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 03:53:28.000000 ctrip-helper-0.3.3/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 03:53:28.545987 ctrip-helper-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-31 03:53:20.000000 ctrip-helper-0.3.3/setup.py
```

### Comparing `ctrip-helper-0.3.2/LICENSE` & `ctrip-helper-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.2/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.3.3/ctrip_helper/api/desktop_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 class UILocatorRegx(Enum):
     all_orders_select_box = {"locator": "xpath",
                              "regx": '//ul[@class="fix_myctrip_order_layer"]//div[@class="select-box"]'}
     order_id_input_box = {"locator": "xpath", "regx": '//div[@class="order_inquiry"]//input[@id="searchBookingNum"]'}
     order_query_button = {"locator": "xpath", "regx": '//div[@class="order_inquiry"]//button[@class="btn_sel"]'}
     order_status_with_list = {"locator": "xpath",
                               "regx": '//ul[@class="t_body"]//span[@class="order-price-status-title"]'}
-    order_price = {"locator": "xpath", "regx": '//li[@class="item"]//div[@class="order-price-detail"]'}
     order_status_sub_title = {"locator": "xpath",
                               "regx": '//div[contains(@data-testid, "orderstatus_StatusSubTitleWrap")]'}
     order_status_booking_amount = {"locator": "xpath",
                                    "regx": '//div[@data-testid="fbu_PaymentWrapper"]//span[@data-testid="false"]'}
     order_to_payment = {"locator": "xpath", "regx": '//div[@id="button-group"]//a[@data-ubt-v="主订单支付"]'}
     order_to_cancel = {"locator": "xpath", "regx": '//div[@id="button-group"]//a[@data-ubt-v="取消订单"]'}
     order_continue_cancel = {"locator": "xpath", "regx": '//div[@class="ant-modal"]//div[@data-testid="继续取消"]'}
@@ -232,36 +231,22 @@
         )
         if order_status_element:
             order_status = order_status_element.text.strip()
             logger.info("获取订单的状态为：{}".format(order_status))
         return order_status
 
     @classmethod
-    def get_order_amonut_with_query_list(cls, driver: webdriver, order_id: str, loop: int = 1,
-                                         sleep: float = 0, **kwargs) -> Decimal:
-        order_amonut = "0.00"
-        order_amonut_element = get_element(
-            driver=driver, locator=UILocatorRegx.order_price.value.get("locator"),
-            regx=UILocatorRegx.order_price.value.get("regx"), loop=loop, sleep=sleep, **kwargs
-        )
-        if order_amonut_element:
-            text = order_amonut_element.text.strip()
-            logger.info("从查询列表中获取订单: {} 的金额：{}".format(order_id, text))
-            order_amonut = text.split("¥")[-1]
-        return Decimal(order_amonut)
-
-    @classmethod
     def click_order_amonut_with_query_list(cls, driver: webdriver, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
-        order_amonut_element = get_element(
-            driver=driver, locator=UILocatorRegx.order_price.value.get("locator"),
-            regx=UILocatorRegx.order_price.value.get("regx"), loop=loop, sleep=sleep, **kwargs
-        )
-        if order_amonut_element:
-            order_amonut_element.click()
-            logger.info("点击订单金额，进入订单详情界面")
+        order_status_element = get_element(
+            driver=driver, locator=UILocatorRegx.order_status_with_list.value.get("locator"),
+            regx=UILocatorRegx.order_status_with_list.value.get("regx"), loop=loop, sleep=sleep, **kwargs
+        )
+        if order_status_element:
+            order_status_element.click()
+            logger.info("点击订单状态，进入订单详情界面")
             return True
         else:
             return False
 
     @classmethod
     def click_to_payment(cls, driver: webdriver, order_id: str, loop: int = 1, sleep: float = 0, **kwargs) -> bool:
         local_url = "{}?oid={}".format(url_map.get("flight_order_details"), order_id)
```

### Comparing `ctrip-helper-0.3.2/ctrip_helper/api/http_api.py` & `ctrip-helper-0.3.3/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.2/ctrip_helper/config.py` & `ctrip-helper-0.3.3/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.2/ctrip_helper/http_client.py` & `ctrip-helper-0.3.3/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.2/ctrip_helper/libs.py` & `ctrip-helper-0.3.3/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.2/ctrip_helper/utils.py` & `ctrip-helper-0.3.3/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.2/setup.py` & `ctrip-helper-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.3.2',
+    version='0.3.3',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

