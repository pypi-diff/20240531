# Comparing `tmp/ctrip-helper-0.3.5.tar.gz` & `tmp/ctrip-helper-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.3.5.tar", last modified: Fri May 31 07:43:07 2024, max compression
+gzip compressed data, was "ctrip-helper-0.3.6.tar", last modified: Fri May 31 08:35:46 2024, max compression
```

## Comparing `ctrip-helper-0.3.5.tar` & `ctrip-helper-0.3.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 07:43:07.300922 ctrip-helper-0.3.5/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.5/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-31 07:43:07.298931 ctrip-helper-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 07:43:07.284964 ctrip-helper-0.3.5/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.5/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:43:07.295935 ctrip-helper-0.3.5/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.5/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    31711 2024-05-31 07:42:47.000000 ctrip-helper-0.3.5/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.5/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.5/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.5/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     7415 2024-05-31 03:29:13.000000 ctrip-helper-0.3.5/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.5/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 07:43:07.297934 ctrip-helper-0.3.5/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-31 07:43:07.000000 ctrip-helper-0.3.5/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-31 07:43:07.000000 ctrip-helper-0.3.5/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 07:43:07.000000 ctrip-helper-0.3.5/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-31 07:43:07.000000 ctrip-helper-0.3.5/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 07:43:07.000000 ctrip-helper-0.3.5/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 07:43:07.300922 ctrip-helper-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-31 07:43:00.000000 ctrip-helper-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 08:35:46.916288 ctrip-helper-0.3.6/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.6/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-31 08:35:46.914294 ctrip-helper-0.3.6/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 08:35:46.899358 ctrip-helper-0.3.6/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.6/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 08:35:46.911302 ctrip-helper-0.3.6/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.6/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    32194 2024-05-31 08:34:43.000000 ctrip-helper-0.3.6/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.6/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.6/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.6/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     7415 2024-05-31 03:29:13.000000 ctrip-helper-0.3.6/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.6/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 08:35:46.913296 ctrip-helper-0.3.6/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-31 08:35:46.000000 ctrip-helper-0.3.6/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-31 08:35:46.000000 ctrip-helper-0.3.6/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 08:35:46.000000 ctrip-helper-0.3.6/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-31 08:35:46.000000 ctrip-helper-0.3.6/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 08:35:46.000000 ctrip-helper-0.3.6/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 08:35:46.916288 ctrip-helper-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-31 08:35:41.000000 ctrip-helper-0.3.6/setup.py
```

### Comparing `ctrip-helper-0.3.5/LICENSE` & `ctrip-helper-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.5/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.3.6/ctrip_helper/api/desktop_ui.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,18 +328,18 @@
                 order_payment_amount = order_payment_amount_element.text.strip()
                 logger.info("获取订单的支付金额为：{}".format(order_payment_amount))
         else:
             logger.warning("当前页：{} 不是订单安全支付页".format(current_url))
         return Decimal(order_payment_amount)
 
     @classmethod
-    def is_cancel_order(cls, driver: webdriver, out_total_amount: str, amount_loss_limit: str, profit_cap: str,
-                        passenger_number: int, platform: str, loop: int = 1, sleep: float = 0,
-                        discount_amount: str = None, **kwargs) -> tuple:
-        """在订单详情页，判断是否需要取消订单"""
+    def is_cancel_order_with_payment_amount(cls, driver: webdriver, out_total_amount: str, amount_loss_limit: str,
+                                            profit_cap: str, passenger_number: int, platform: str, loop: int = 1,
+                                            sleep: float = 0, discount_amount: str = None, **kwargs) -> tuple:
+        """在订单详情页，判断是否需要取消订单，检验支付金额是否满足政策要求"""
         flag = False
         remark = ""
         booking_amount_element = get_element(
             driver=driver, locator=UILocatorRegx.order_status_booking_amount.value.get("locator"),
             regx=UILocatorRegx.order_status_booking_amount.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if booking_amount_element:
@@ -380,14 +380,22 @@
                         return flag, remark
             else:
                 remark = "从订单详情页面获取订单过期时间和订单金额有异常"
                 logger.warning(remark)
         else:
             remark = "订单详情页面中未找到订单金额元素"
             logger.warning(remark)
+        return flag, remark
+
+    @classmethod
+    def is_cancel_order_with_remaining_payment_time(cls, driver: webdriver, loop: int = 1, sleep: float = 0,
+                                                    **kwargs) -> tuple:
+        """在订单详情页，判断是否需要取消订单，判断订单的剩余支付时间"""
+        flag = False
+        remark = ""
         status_sub_title_element = get_element(
             driver=driver, locator=UILocatorRegx.order_status_sub_title.value.get("locator"),
             regx=UILocatorRegx.order_status_sub_title.value.get("regx"), loop=loop, sleep=sleep, **kwargs
         )
         if status_sub_title_element:
             sub_title_text = status_sub_title_element.text.strip()
             # 使用 findall 获取所有匹配项
```

### Comparing `ctrip-helper-0.3.5/ctrip_helper/api/http_api.py` & `ctrip-helper-0.3.6/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.5/ctrip_helper/config.py` & `ctrip-helper-0.3.6/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.5/ctrip_helper/http_client.py` & `ctrip-helper-0.3.6/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.5/ctrip_helper/libs.py` & `ctrip-helper-0.3.6/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.5/ctrip_helper/utils.py` & `ctrip-helper-0.3.6/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.5/setup.py` & `ctrip-helper-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.3.5',
+    version='0.3.6',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

