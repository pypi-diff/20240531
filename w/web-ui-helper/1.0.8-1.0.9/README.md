# Comparing `tmp/web-ui-helper-1.0.8.tar.gz` & `tmp/web-ui-helper-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web-ui-helper-1.0.8.tar", last modified: Wed May 29 02:15:37 2024, max compression
+gzip compressed data, was "web-ui-helper-1.0.9.tar", last modified: Fri May 31 12:23:50 2024, max compression
```

## Comparing `web-ui-helper-1.0.8.tar` & `web-ui-helper-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 02:15:37.100210 web-ui-helper-1.0.8/
--rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      747 2024-05-29 02:15:37.098216 web-ui-helper-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-29 02:15:37.100210 web-ui-helper-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1325 2024-05-29 02:15:28.000000 web-ui-helper-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:15:37.053337 web-ui-helper-1.0.8/web_ui_helper/
--rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-1.0.8/web_ui_helper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:15:37.075278 web-ui-helper-1.0.8/web_ui_helper/common/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.8/web_ui_helper/common/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-1.0.8/web_ui_helper/common/date_extend.py
--rw-rw-rw-   0        0        0     5309 2024-05-25 01:33:22.000000 web-ui-helper-1.0.8/web_ui_helper/common/dir.py
--rw-rw-rw-   0        0        0     1704 2024-05-24 09:36:39.000000 web-ui-helper-1.0.8/web_ui_helper/common/http_proxy.py
--rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-1.0.8/web_ui_helper/common/log.py
--rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-1.0.8/web_ui_helper/common/metaclass.py
--rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-1.0.8/web_ui_helper/common/platforms.py
--rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-1.0.8/web_ui_helper/common/webdriver.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:15:37.080264 web-ui-helper-1.0.8/web_ui_helper/decorators/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.8/web_ui_helper/decorators/__init__.py
--rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-1.0.8/web_ui_helper/decorators/airtest_exception.py
--rw-rw-rw-   0        0        0     4104 2024-05-22 11:26:11.000000 web-ui-helper-1.0.8/web_ui_helper/decorators/selenium_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:15:37.081272 web-ui-helper-1.0.8/web_ui_helper/selenium/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-1.0.8/web_ui_helper/selenium/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:15:37.084253 web-ui-helper-1.0.8/web_ui_helper/selenium/frame/
--rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-1.0.8/web_ui_helper/selenium/frame/__init__.py
--rw-rw-rw-   0        0        0    38888 2024-05-29 02:15:01.000000 web-ui-helper-1.0.8/web_ui_helper/selenium/frame/browser.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:15:37.087245 web-ui-helper-1.0.8/web_ui_helper/selenium/parse/
--rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-1.0.8/web_ui_helper/selenium/parse/__init__.py
--rw-rw-rw-   0        0        0    23304 2024-05-24 07:34:39.000000 web-ui-helper-1.0.8/web_ui_helper/selenium/parse/ctrip_flight.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:15:37.091237 web-ui-helper-1.0.8/web_ui_helper/selenium/ui/
--rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.8/web_ui_helper/selenium/ui/__init__.py
--rw-rw-rw-   0        0        0     9680 2024-05-24 07:37:00.000000 web-ui-helper-1.0.8/web_ui_helper/selenium/ui/frame.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:15:37.094227 web-ui-helper-1.0.8/web_ui_helper/terminal/
--rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-1.0.8/web_ui_helper/terminal/__init__.py
--rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-1.0.8/web_ui_helper/terminal/device.py
-drwxrwxrwx   0        0        0        0 2024-05-29 02:15:37.097231 web-ui-helper-1.0.8/web_ui_helper.egg-info/
--rw-rw-rw-   0        0        0      747 2024-05-29 02:15:36.000000 web-ui-helper-1.0.8/web_ui_helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      971 2024-05-29 02:15:36.000000 web-ui-helper-1.0.8/web_ui_helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 02:15:36.000000 web-ui-helper-1.0.8/web_ui_helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      171 2024-05-29 02:15:36.000000 web-ui-helper-1.0.8/web_ui_helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-29 02:15:36.000000 web-ui-helper-1.0.8/web_ui_helper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 12:23:50.965028 web-ui-helper-1.0.9/
+-rw-rw-rw-   0        0        0    11558 2024-04-28 17:21:26.000000 web-ui-helper-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      747 2024-05-31 12:23:50.964030 web-ui-helper-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-04-28 17:21:26.000000 web-ui-helper-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-31 12:23:50.966026 web-ui-helper-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1325 2024-05-31 12:23:38.000000 web-ui-helper-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:23:50.917156 web-ui-helper-1.0.9/web_ui_helper/
+-rw-rw-rw-   0        0        0      467 2024-04-28 18:08:46.000000 web-ui-helper-1.0.9/web_ui_helper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:23:50.940094 web-ui-helper-1.0.9/web_ui_helper/common/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.9/web_ui_helper/common/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-04-28 18:51:41.000000 web-ui-helper-1.0.9/web_ui_helper/common/date_extend.py
+-rw-rw-rw-   0        0        0     5309 2024-05-25 01:33:22.000000 web-ui-helper-1.0.9/web_ui_helper/common/dir.py
+-rw-rw-rw-   0        0        0     1704 2024-05-24 09:36:39.000000 web-ui-helper-1.0.9/web_ui_helper/common/http_proxy.py
+-rw-rw-rw-   0        0        0      866 2024-04-28 17:21:26.000000 web-ui-helper-1.0.9/web_ui_helper/common/log.py
+-rw-rw-rw-   0        0        0     1104 2024-04-28 17:21:26.000000 web-ui-helper-1.0.9/web_ui_helper/common/metaclass.py
+-rw-rw-rw-   0        0        0      552 2024-04-28 17:21:26.000000 web-ui-helper-1.0.9/web_ui_helper/common/platforms.py
+-rw-rw-rw-   0        0        0      836 2024-04-28 17:21:26.000000 web-ui-helper-1.0.9/web_ui_helper/common/webdriver.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:23:50.946078 web-ui-helper-1.0.9/web_ui_helper/decorators/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.9/web_ui_helper/decorators/__init__.py
+-rw-rw-rw-   0        0        0     2449 2024-04-28 17:21:26.000000 web-ui-helper-1.0.9/web_ui_helper/decorators/airtest_exception.py
+-rw-rw-rw-   0        0        0     4104 2024-05-22 11:26:11.000000 web-ui-helper-1.0.9/web_ui_helper/decorators/selenium_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:23:50.948073 web-ui-helper-1.0.9/web_ui_helper/selenium/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:56:27.000000 web-ui-helper-1.0.9/web_ui_helper/selenium/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:23:50.950068 web-ui-helper-1.0.9/web_ui_helper/selenium/frame/
+-rw-rw-rw-   0        0        0      471 2024-04-28 17:46:47.000000 web-ui-helper-1.0.9/web_ui_helper/selenium/frame/__init__.py
+-rw-rw-rw-   0        0        0    39014 2024-05-31 12:23:29.000000 web-ui-helper-1.0.9/web_ui_helper/selenium/frame/browser.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:23:50.954058 web-ui-helper-1.0.9/web_ui_helper/selenium/parse/
+-rw-rw-rw-   0        0        0      471 2024-05-05 09:55:38.000000 web-ui-helper-1.0.9/web_ui_helper/selenium/parse/__init__.py
+-rw-rw-rw-   0        0        0    23304 2024-05-24 07:34:39.000000 web-ui-helper-1.0.9/web_ui_helper/selenium/parse/ctrip_flight.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:23:50.958047 web-ui-helper-1.0.9/web_ui_helper/selenium/ui/
+-rw-rw-rw-   0        0        0      467 2024-04-28 17:21:26.000000 web-ui-helper-1.0.9/web_ui_helper/selenium/ui/__init__.py
+-rw-rw-rw-   0        0        0     9680 2024-05-24 07:37:00.000000 web-ui-helper-1.0.9/web_ui_helper/selenium/ui/frame.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:23:50.961038 web-ui-helper-1.0.9/web_ui_helper/terminal/
+-rw-rw-rw-   0        0        0      470 2024-04-28 17:21:26.000000 web-ui-helper-1.0.9/web_ui_helper/terminal/__init__.py
+-rw-rw-rw-   0        0        0    27491 2024-04-28 17:21:26.000000 web-ui-helper-1.0.9/web_ui_helper/terminal/device.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:23:50.963034 web-ui-helper-1.0.9/web_ui_helper.egg-info/
+-rw-rw-rw-   0        0        0      747 2024-05-31 12:23:50.000000 web-ui-helper-1.0.9/web_ui_helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      971 2024-05-31 12:23:50.000000 web-ui-helper-1.0.9/web_ui_helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 12:23:50.000000 web-ui-helper-1.0.9/web_ui_helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      171 2024-05-31 12:23:50.000000 web-ui-helper-1.0.9/web_ui_helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-31 12:23:50.000000 web-ui-helper-1.0.9/web_ui_helper.egg-info/top_level.txt
```

### Comparing `web-ui-helper-1.0.8/LICENSE` & `web-ui-helper-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.8/PKG-INFO` & `web-ui-helper-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 1.0.8
+Version: 1.0.9
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-1.0.8/setup.py` & `web-ui-helper-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # Copyright ©2011-2024. Hunan xxxxxxx Company limited. All rights reserved.
 # ---------------------------------------------------------------------------------------------------------
 """
 from setuptools import setup, find_packages
 
 setup(
     name='web-ui-helper',
-    version='1.0.8',
+    version='1.0.9',
     description='This is my web ui helper package',
     long_description='This is my web ui helper package',
     author='ckf10000',
     author_email='ckf10000@sina.com',
     url='https://github.com/ckf10000/web-ui-helper',
     packages=find_packages(),
     install_requires=[
```

### Comparing `web-ui-helper-1.0.8/web_ui_helper/common/date_extend.py` & `web-ui-helper-1.0.9/web_ui_helper/common/date_extend.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.8/web_ui_helper/common/dir.py` & `web-ui-helper-1.0.9/web_ui_helper/common/dir.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.8/web_ui_helper/common/http_proxy.py` & `web-ui-helper-1.0.9/web_ui_helper/common/http_proxy.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.8/web_ui_helper/common/log.py` & `web-ui-helper-1.0.9/web_ui_helper/common/log.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.8/web_ui_helper/common/metaclass.py` & `web-ui-helper-1.0.9/web_ui_helper/common/metaclass.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.8/web_ui_helper/common/platforms.py` & `web-ui-helper-1.0.9/web_ui_helper/common/platforms.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.8/web_ui_helper/common/webdriver.py` & `web-ui-helper-1.0.9/web_ui_helper/common/webdriver.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.8/web_ui_helper/decorators/airtest_exception.py` & `web-ui-helper-1.0.9/web_ui_helper/decorators/airtest_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.8/web_ui_helper/decorators/selenium_exception.py` & `web-ui-helper-1.0.9/web_ui_helper/decorators/selenium_exception.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.8/web_ui_helper/selenium/frame/browser.py` & `web-ui-helper-1.0.9/web_ui_helper/selenium/frame/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,14 +383,17 @@
             if is_single_instance is True:
                 if self.browser_proxy.is_running() is True:
                     raise ValueError("Firefox browser is already running.")
             self.browser, self.wait, self.browser_name = self.browser_proxy.get_browser()
         else:
             raise ValueError("Browser name must be Chrome or Firefox.")
 
+    def new_instance(self) -> None:
+        self.browser, self.wait, self.browser_name = self.browser_proxy.get_browser()
+
     def input_text(self, locator: str, regx: str, value: str) -> bool:
         """
         locator 选择器
         regx 选择器所要匹配的表达式
         value 文本框输入值
         """
         flag = False
```

### Comparing `web-ui-helper-1.0.8/web_ui_helper/selenium/parse/ctrip_flight.py` & `web-ui-helper-1.0.9/web_ui_helper/selenium/parse/ctrip_flight.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.8/web_ui_helper/selenium/ui/frame.py` & `web-ui-helper-1.0.9/web_ui_helper/selenium/ui/frame.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.8/web_ui_helper/terminal/device.py` & `web-ui-helper-1.0.9/web_ui_helper/terminal/device.py`

 * *Files identical despite different names*

### Comparing `web-ui-helper-1.0.8/web_ui_helper.egg-info/PKG-INFO` & `web-ui-helper-1.0.9/web_ui_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web-ui-helper
-Version: 1.0.8
+Version: 1.0.9
 Summary: This is my web ui helper package
 Home-page: https://github.com/ckf10000/web-ui-helper
 Author: ckf10000
 Author-email: ckf10000@sina.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `web-ui-helper-1.0.8/web_ui_helper.egg-info/SOURCES.txt` & `web-ui-helper-1.0.9/web_ui_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

