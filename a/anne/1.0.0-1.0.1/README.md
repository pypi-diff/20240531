# Comparing `tmp/anne-1.0.0.tar.gz` & `tmp/anne-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anne-1.0.0.tar", last modified: Tue May 28 15:37:06 2024, max compression
+gzip compressed data, was "anne-1.0.1.tar", last modified: Fri May 31 00:29:35 2024, max compression
```

## Comparing `anne-1.0.0.tar` & `anne-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 15:37:06.786958 anne-1.0.0/
--rw-rw-rw-   0        0        0     1090 2024-05-28 14:49:46.000000 anne-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1504 2024-05-28 15:37:06.786958 anne-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       45 2024-05-28 15:27:28.000000 anne-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 15:37:06.777988 anne-1.0.0/app/
-drwxrwxrwx   0        0        0        0 2024-05-28 15:37:06.780978 anne-1.0.0/app/anne/
--rw-rw-rw-   0        0        0       64 2024-05-28 15:29:15.000000 anne-1.0.0/app/anne/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 15:37:06.783967 anne-1.0.0/app/anne/browser/
--rw-rw-rw-   0        0        0       42 2024-05-28 14:58:15.000000 anne-1.0.0/app/anne/browser/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 15:37:06.783967 anne-1.0.0/app/anne/browser/src/
--rw-rw-rw-   0        0        0    16592 2024-05-28 15:23:51.000000 anne-1.0.0/app/anne/browser/src/AnneBrowser.py
--rw-rw-rw-   0        0        0        0 2024-05-28 14:55:35.000000 anne-1.0.0/app/anne/browser/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 15:37:06.784965 anne-1.0.0/app/anne/browser/test/
--rw-rw-rw-   0        0        0        0 2024-05-28 14:55:35.000000 anne-1.0.0/app/anne/browser/test/__init__.py
--rw-rw-rw-   0        0        0      875 2024-05-28 15:22:57.000000 anne-1.0.0/app/anne/browser/test/test_AnneBrowser.py
-drwxrwxrwx   0        0        0        0 2024-05-28 15:37:06.786958 anne-1.0.0/app/anne/proxy/
--rw-rw-rw-   0        0        0       83 2024-05-28 10:16:05.000000 anne-1.0.0/app/anne/proxy/AnneProxy.py
--rw-rw-rw-   0        0        0       26 2024-05-28 05:22:43.000000 anne-1.0.0/app/anne/proxy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 15:37:06.782971 anne-1.0.0/app/anne.egg-info/
--rw-rw-rw-   0        0        0     1504 2024-05-28 15:37:06.000000 anne-1.0.0/app/anne.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      435 2024-05-28 15:37:06.000000 anne-1.0.0/app/anne.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 15:37:06.000000 anne-1.0.0/app/anne.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-28 15:37:06.000000 anne-1.0.0/app/anne.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-28 15:37:06.000000 anne-1.0.0/app/anne.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 15:37:06.786958 anne-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-05-28 15:35:06.000000 anne-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:29:35.267022 anne-1.0.1/
+-rw-rw-rw-   0        0        0     1090 2024-05-28 14:49:46.000000 anne-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1504 2024-05-31 00:29:35.267022 anne-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2024-05-28 15:27:28.000000 anne-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 00:29:35.261042 anne-1.0.1/app/
+drwxrwxrwx   0        0        0        0 2024-05-31 00:29:35.263035 anne-1.0.1/app/anne/
+-rw-rw-rw-   0        0        0       64 2024-05-31 00:19:07.000000 anne-1.0.1/app/anne/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:29:35.266025 anne-1.0.1/app/anne/browser/
+-rw-rw-rw-   0        0        0    18824 2024-05-28 16:14:25.000000 anne-1.0.1/app/anne/browser/AnneBrowser.py
+-rw-rw-rw-   0        0        0       38 2024-05-31 00:17:53.000000 anne-1.0.1/app/anne/browser/__init__.py
+-rw-rw-rw-   0        0        0      692 2024-05-28 16:07:51.000000 anne-1.0.1/app/anne/browser/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:29:35.267022 anne-1.0.1/app/anne/proxy/
+-rw-rw-rw-   0        0        0      882 2024-05-31 00:03:51.000000 anne-1.0.1/app/anne/proxy/AnneProxy.py
+-rw-rw-rw-   0        0        0       32 2024-05-31 00:19:01.000000 anne-1.0.1/app/anne/proxy/__init__.py
+-rw-rw-rw-   0        0        0       16 2024-05-31 00:09:11.000000 anne-1.0.1/app/anne/proxy/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:29:35.265029 anne-1.0.1/app/anne.egg-info/
+-rw-rw-rw-   0        0        0     1504 2024-05-31 00:29:35.000000 anne-1.0.1/app/anne.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-05-31 00:29:35.000000 anne-1.0.1/app/anne.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 00:29:35.000000 anne-1.0.1/app/anne.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-31 00:29:35.000000 anne-1.0.1/app/anne.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-31 00:29:35.000000 anne-1.0.1/app/anne.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 00:29:35.267022 anne-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-05-31 00:19:14.000000 anne-1.0.1/setup.py
```

### Comparing `anne-1.0.0/LICENSE` & `anne-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anne-1.0.0/PKG-INFO` & `anne-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anne
-Version: 1.0.0
+Version: 1.0.1
 Summary: Lib for lazy dev
 Home-page: https://github.com/mrship666/anne-lib
 Author: AnneHouman
 Author-email: annehouman01@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `anne-1.0.0/app/anne/browser/src/AnneBrowser.py` & `anne-1.0.1/app/anne/browser/AnneBrowser.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,31 +5,77 @@
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.common.exceptions import TimeoutException, NoSuchElementException, WebDriverException, NoSuchWindowException
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.by import By
 
 import time, random
+from utils import *
+
 
 
 """
     
 Version: 28/05/2024
 Developer: AnneHouman
 
 """
 
 
 class AnneBrowser:
     # DEBUG = True
     
-    def __init__(self, driver, debug=False):
+    def __init__(self, driver=None, debug=False):
         self.driver = driver
         self.DEBUG = debug
+    
+    def createDriver(self, browser='chrome', data=None): # Tạo driver
+        """ Giá trị của các tham số:
+        
+        browser: 'chrome', 'firefox'
+        
+        data: {
+            "headless": True,  # True hoặc False
+            "proxy": {
+                "mode": 0,  # 0: Không sử dụng proxy, 1: Sử dụng proxy
+                "host": None,  # None hoặc str
+                "port": None,  # None hoặc int
+                "username": None,  # None hoặc str
+                "password": None  # None hoặc str
+            },
+            "user_agent": 0,  # 0: Không sử dụng user agent, 1: Sử dụng user agent ngẫu nhiên, 2: Sử dụng user agent cố định
+            "window_size": None,  # None hoặc (width, height) - tuple | Ví dụ: (1920, 1080)
+            "antibot": False,  # True hoặc False
+        """
+        if browser == 'chrome': return self._chrome_driver(data)
+     
+    def _chrome_driver(self, data=None): # Tạo driver cho Chrome
+        if not data: return webdriver.Chrome(ChromeDriverManager().install())
+        chrome_options = webdriver.ChromeOptions()
+        
+        if data.get('headless', False) is True: chrome_options.add_argument("--headless")
         
+        if data.get('proxy', None) is not None:
+            proxy = data['proxy']
+            if proxy['mode'] == 1:
+                chrome_options.add_argument(f"--proxy-server={proxy['host']}:{proxy['port']}")
+                if proxy['username'] and proxy['password']:
+                    chrome_options.add_argument(f"--proxy-auth={proxy['username']}:{proxy['password']}")
+            else: pass
+        
+        if data.get('user_agent', 0) == 0: pass
+        elif data['user_agent'] == 1: chrome_options.add_argument(f"user-agent={get_ua()}")
+        else: chrome_options.add_argument(f"user-agent={data['user_agent']}")
+        
+        if data.get('window_size', None) is not None: chrome_options.add_argument(f"--window-size={data['window_size'][0]},{data['window_size'][1]}")
+        
+        driver = webdriver.Chrome(ChromeDriverManager().install(), options=chrome_options)
+        return driver
+         
+    
     def _locator_type(self, locator): # Định dạng loại locator
         """Định dạng loại locator
 
         Args:
             locator (str): 'xpath', 'css', 'id', 'name', 'linktext1', 'linktext2', 'class', 'tag'
 
         Raises:
```

### Comparing `anne-1.0.0/app/anne.egg-info/PKG-INFO` & `anne-1.0.1/app/anne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anne
-Version: 1.0.0
+Version: 1.0.1
 Summary: Lib for lazy dev
 Home-page: https://github.com/mrship666/anne-lib
 Author: AnneHouman
 Author-email: annehouman01@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `anne-1.0.0/setup.py` & `anne-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="anne",
-    version="1.0.0",
+    version="1.0.1",
     description="Lib for lazy dev",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrship666/anne-lib",
     author="AnneHouman",
```

