# Comparing `tmp/ctrip-helper-0.3.0.tar.gz` & `tmp/ctrip-helper-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctrip-helper-0.3.0.tar", last modified: Fri May 31 02:59:20 2024, max compression
+gzip compressed data, was "ctrip-helper-0.3.1.tar", last modified: Fri May 31 03:04:56 2024, max compression
```

## Comparing `ctrip-helper-0.3.0.tar` & `ctrip-helper-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 02:59:20.030461 ctrip-helper-0.3.0/
--rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      474 2024-05-31 02:59:20.029453 ctrip-helper-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 02:59:20.011501 ctrip-helper-0.3.0/ctrip_helper/
--rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.0/ctrip_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 02:59:20.026461 ctrip-helper-0.3.0/ctrip_helper/api/
--rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.0/ctrip_helper/api/__init__.py
--rw-rw-rw-   0        0        0    30304 2024-05-31 02:58:51.000000 ctrip-helper-0.3.0/ctrip_helper/api/desktop_ui.py
--rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.0/ctrip_helper/api/http_api.py
--rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.0/ctrip_helper/config.py
--rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.0/ctrip_helper/http_client.py
--rw-rw-rw-   0        0        0     7033 2024-05-31 02:57:42.000000 ctrip-helper-0.3.0/ctrip_helper/libs.py
--rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.0/ctrip_helper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 02:59:20.028456 ctrip-helper-0.3.0/ctrip_helper.egg-info/
--rw-rw-rw-   0        0        0      474 2024-05-31 02:59:19.000000 ctrip-helper-0.3.0/ctrip_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2024-05-31 02:59:19.000000 ctrip-helper-0.3.0/ctrip_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 02:59:19.000000 ctrip-helper-0.3.0/ctrip_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-05-31 02:59:19.000000 ctrip-helper-0.3.0/ctrip_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 02:59:19.000000 ctrip-helper-0.3.0/ctrip_helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 02:59:20.031452 ctrip-helper-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1087 2024-05-31 02:59:15.000000 ctrip-helper-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:04:56.260685 ctrip-helper-0.3.1/
+-rw-rw-rw-   0        0        0    11558 2024-05-25 17:09:13.000000 ctrip-helper-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      474 2024-05-31 03:04:56.259687 ctrip-helper-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2024-05-25 17:09:13.000000 ctrip-helper-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 03:04:56.245725 ctrip-helper-0.3.1/ctrip_helper/
+-rw-rw-rw-   0        0        0      470 2024-05-25 17:13:06.000000 ctrip-helper-0.3.1/ctrip_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:04:56.256695 ctrip-helper-0.3.1/ctrip_helper/api/
+-rw-rw-rw-   0        0        0      470 2024-05-29 02:43:24.000000 ctrip-helper-0.3.1/ctrip_helper/api/__init__.py
+-rw-rw-rw-   0        0        0    30305 2024-05-31 03:04:41.000000 ctrip-helper-0.3.1/ctrip_helper/api/desktop_ui.py
+-rw-rw-rw-   0        0        0    10771 2024-05-29 16:47:31.000000 ctrip-helper-0.3.1/ctrip_helper/api/http_api.py
+-rw-rw-rw-   0        0        0     3741 2024-05-30 02:36:46.000000 ctrip-helper-0.3.1/ctrip_helper/config.py
+-rw-rw-rw-   0        0        0     4517 2024-05-28 03:12:53.000000 ctrip-helper-0.3.1/ctrip_helper/http_client.py
+-rw-rw-rw-   0        0        0     7033 2024-05-31 02:57:42.000000 ctrip-helper-0.3.1/ctrip_helper/libs.py
+-rw-rw-rw-   0        0        0     4127 2024-05-29 12:27:06.000000 ctrip-helper-0.3.1/ctrip_helper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:04:56.258690 ctrip-helper-0.3.1/ctrip_helper.egg-info/
+-rw-rw-rw-   0        0        0      474 2024-05-31 03:04:56.000000 ctrip-helper-0.3.1/ctrip_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2024-05-31 03:04:56.000000 ctrip-helper-0.3.1/ctrip_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 03:04:56.000000 ctrip-helper-0.3.1/ctrip_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-05-31 03:04:56.000000 ctrip-helper-0.3.1/ctrip_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 03:04:56.000000 ctrip-helper-0.3.1/ctrip_helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 03:04:56.260685 ctrip-helper-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1087 2024-05-31 03:04:52.000000 ctrip-helper-0.3.1/setup.py
```

### Comparing `ctrip-helper-0.3.0/LICENSE` & `ctrip-helper-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.0/ctrip_helper/api/desktop_ui.py` & `ctrip-helper-0.3.1/ctrip_helper/api/desktop_ui.py`

 * *Files 0% similar despite different names*

```diff
@@ -515,15 +515,15 @@
             driver=driver, locator=UILocatorRegx.password_input_box.value.get("locator"),
             regx=UILocatorRegx.password_input_box.value.get("regx"), sleep=sleep, loop=loop, **kwargs
         )
         if password_input_box:
             if not isinstance(password, str):
                 password = str(password)
             for char in password:
-                is_success = send_keys(element=password_input_box, char=char, loop=loop, sleep=sleep, **kwargs)
+                is_success = send_keys(element=password_input_box, value=char, loop=loop, sleep=sleep, **kwargs)
                 if is_success is False:
                     return False
                 # 可选：添加一个短暂的延迟，模拟更接近人类的输入速度
                 time.sleep(0.5)
             return True
         else:
             logger.warning("没有出现输入密码的弹框")
```

### Comparing `ctrip-helper-0.3.0/ctrip_helper/api/http_api.py` & `ctrip-helper-0.3.1/ctrip_helper/api/http_api.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.0/ctrip_helper/config.py` & `ctrip-helper-0.3.1/ctrip_helper/config.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.0/ctrip_helper/http_client.py` & `ctrip-helper-0.3.1/ctrip_helper/http_client.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.0/ctrip_helper/libs.py` & `ctrip-helper-0.3.1/ctrip_helper/libs.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.0/ctrip_helper/utils.py` & `ctrip-helper-0.3.1/ctrip_helper/utils.py`

 * *Files identical despite different names*

### Comparing `ctrip-helper-0.3.0/setup.py` & `ctrip-helper-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='ctrip-helper',
-    version='0.3.0',
+    version='0.3.1',
     description='This is my ctrip help package',
     long_description='This is my ctrip help package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/ctrip-helper',
     packages=find_packages(),
     install_requires=[
```

