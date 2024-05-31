# Comparing `tmp/RnDNews-0.1.1.tar.gz` & `tmp/RnDNews-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RnDNews-0.1.1.tar", last modified: Thu May 16 14:55:58 2024, max compression
+gzip compressed data, was "RnDNews-0.1.2.tar", last modified: Fri May 31 14:21:31 2024, max compression
```

## Comparing `RnDNews-0.1.1.tar` & `RnDNews-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 hanan     (1000) hanan     (1000)        0 2024-05-16 14:55:58.871527 RnDNews-0.1.1/
--rw-r--r--   0 hanan     (1000) hanan     (1000)     1261 2024-05-16 14:55:58.867527 RnDNews-0.1.1/PKG-INFO
--rw-rw-r--   0 hanan     (1000) hanan     (1000)        0 2024-05-08 13:10:51.000000 RnDNews-0.1.1/README.md
-drwxrwxr-x   0 hanan     (1000) hanan     (1000)        0 2024-05-16 14:55:58.867527 RnDNews-0.1.1/RnDNews/
--rw-rw-r--   0 hanan     (1000) hanan     (1000)     4717 2024-05-14 15:46:53.000000 RnDNews-0.1.1/RnDNews/DuckDuckGo_Scraper.py
--rw-rw-r--   0 hanan     (1000) hanan     (1000)     4849 2024-05-14 10:46:50.000000 RnDNews-0.1.1/RnDNews/Google_Scraper.py
--rw-rw-r--   0 hanan     (1000) hanan     (1000)      404 2024-05-14 10:46:50.000000 RnDNews-0.1.1/RnDNews/Scraper.py
--rw-rw-r--   0 hanan     (1000) hanan     (1000)     4134 2024-05-16 09:52:38.000000 RnDNews-0.1.1/RnDNews/Shared_Methods.py
--rw-rw-r--   0 hanan     (1000) hanan     (1000)        0 2024-04-01 13:33:50.000000 RnDNews-0.1.1/RnDNews/__init__.py
--rw-rw-r--   0 hanan     (1000) hanan     (1000)     2110 2024-05-16 14:31:55.000000 RnDNews-0.1.1/RnDNews/config.py
-drwxrwxr-x   0 hanan     (1000) hanan     (1000)        0 2024-05-16 14:55:58.867527 RnDNews-0.1.1/RnDNews.egg-info/
--rw-r--r--   0 hanan     (1000) hanan     (1000)     1261 2024-05-16 14:55:58.000000 RnDNews-0.1.1/RnDNews.egg-info/PKG-INFO
--rw-rw-r--   0 hanan     (1000) hanan     (1000)      311 2024-05-16 14:55:58.000000 RnDNews-0.1.1/RnDNews.egg-info/SOURCES.txt
--rw-rw-r--   0 hanan     (1000) hanan     (1000)        1 2024-05-16 14:55:58.000000 RnDNews-0.1.1/RnDNews.egg-info/dependency_links.txt
--rw-rw-r--   0 hanan     (1000) hanan     (1000)      550 2024-05-16 14:55:58.000000 RnDNews-0.1.1/RnDNews.egg-info/requires.txt
--rw-rw-r--   0 hanan     (1000) hanan     (1000)        8 2024-05-16 14:55:58.000000 RnDNews-0.1.1/RnDNews.egg-info/top_level.txt
--rw-rw-r--   0 hanan     (1000) hanan     (1000)       38 2024-05-16 14:55:58.871527 RnDNews-0.1.1/setup.cfg
--rw-rw-r--   0 hanan     (1000) hanan     (1000)     1299 2024-05-16 14:36:52.000000 RnDNews-0.1.1/setup.py
+drwxrwxr-x   0 hanan     (1000) hanan     (1000)        0 2024-05-31 14:21:30.994304 RnDNews-0.1.2/
+-rw-r--r--   0 hanan     (1000) hanan     (1000)     1261 2024-05-31 14:21:30.994304 RnDNews-0.1.2/PKG-INFO
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)        0 2024-05-08 13:10:51.000000 RnDNews-0.1.2/README.md
+drwxrwxr-x   0 hanan     (1000) hanan     (1000)        0 2024-05-31 14:21:30.994304 RnDNews-0.1.2/RnDNews/
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)     4717 2024-05-14 15:46:53.000000 RnDNews-0.1.2/RnDNews/DuckDuckGo_Scraper.py
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)     4849 2024-05-14 10:46:50.000000 RnDNews-0.1.2/RnDNews/Google_Scraper.py
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)      404 2024-05-14 10:46:50.000000 RnDNews-0.1.2/RnDNews/Scraper.py
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)     4363 2024-05-31 14:18:00.000000 RnDNews-0.1.2/RnDNews/Shared_Methods.py
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)        0 2024-04-01 13:33:50.000000 RnDNews-0.1.2/RnDNews/__init__.py
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)     2110 2024-05-16 14:31:55.000000 RnDNews-0.1.2/RnDNews/config.py
+drwxrwxr-x   0 hanan     (1000) hanan     (1000)        0 2024-05-31 14:21:30.994304 RnDNews-0.1.2/RnDNews.egg-info/
+-rw-r--r--   0 hanan     (1000) hanan     (1000)     1261 2024-05-31 14:21:30.000000 RnDNews-0.1.2/RnDNews.egg-info/PKG-INFO
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)      311 2024-05-31 14:21:30.000000 RnDNews-0.1.2/RnDNews.egg-info/SOURCES.txt
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)        1 2024-05-31 14:21:30.000000 RnDNews-0.1.2/RnDNews.egg-info/dependency_links.txt
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)      550 2024-05-31 14:21:30.000000 RnDNews-0.1.2/RnDNews.egg-info/requires.txt
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)        8 2024-05-31 14:21:30.000000 RnDNews-0.1.2/RnDNews.egg-info/top_level.txt
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)       38 2024-05-31 14:21:30.994304 RnDNews-0.1.2/setup.cfg
+-rw-rw-r--   0 hanan     (1000) hanan     (1000)     1299 2024-05-31 14:20:21.000000 RnDNews-0.1.2/setup.py
```

### Comparing `RnDNews-0.1.1/PKG-INFO` & `RnDNews-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RnDNews
-Version: 0.1.1
+Version: 0.1.2
 Summary: Crawling RnDNews
 Author: Hanan Chrourou
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: argon2-cffi==23.1.0
 Requires-Dist: argon2-cffi-bindings==21.2.0
```

### Comparing `RnDNews-0.1.1/RnDNews/DuckDuckGo_Scraper.py` & `RnDNews-0.1.2/RnDNews/DuckDuckGo_Scraper.py`

 * *Files identical despite different names*

### Comparing `RnDNews-0.1.1/RnDNews/Google_Scraper.py` & `RnDNews-0.1.2/RnDNews/Google_Scraper.py`

 * *Files identical despite different names*

### Comparing `RnDNews-0.1.1/RnDNews/Shared_Methods.py` & `RnDNews-0.1.2/RnDNews/Shared_Methods.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,27 +32,33 @@
                     time.sleep(1)
         return None
 
     @staticmethod
     def retry_with_selenium(url):
         chrome_options = ChromeOptions()
         chrome_options.add_argument("--headless")
-        chrome_service = ChromeService()
+        chrome_options.add_argument("--no-sandbox")
+        chrome_options.add_argument("--disable-dev-shm-usage")
+
+        # Specify the path to the chromedriver installed in the Docker image
+        chrome_service = ChromeService(executable_path='/usr/local/bin/chromedriver')
+
         driver = webdriver.Chrome(service=chrome_service, options=chrome_options)
         try:
             driver.get(url)
             WebDriverWait(driver, 10).until(EC.presence_of_element_located((By.TAG_NAME, 'body')))
             html_content = driver.page_source
             return html_content
         except WebDriverException as e:
             print(f"Selenium WebDriverException occurred: {e}")
-            return None, url, None
+            return None
         finally:
             driver.quit()
 
+
     @staticmethod
     def save_json(company_name, status_code, url, html_content):
         if html_content is not None:
             directory_path = os.path.join("..", "data")
             os.makedirs(directory_path, exist_ok=True)
             json_file_path = os.path.join(directory_path, f"{company_name}.json")
             if not os.path.exists(json_file_path):
```

### Comparing `RnDNews-0.1.1/RnDNews/config.py` & `RnDNews-0.1.2/RnDNews/config.py`

 * *Files identical despite different names*

### Comparing `RnDNews-0.1.1/RnDNews.egg-info/PKG-INFO` & `RnDNews-0.1.2/RnDNews.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RnDNews
-Version: 0.1.1
+Version: 0.1.2
 Summary: Crawling RnDNews
 Author: Hanan Chrourou
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: argon2-cffi==23.1.0
 Requires-Dist: argon2-cffi-bindings==21.2.0
```

### Comparing `RnDNews-0.1.1/RnDNews.egg-info/requires.txt` & `RnDNews-0.1.2/RnDNews.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `RnDNews-0.1.1/setup.py` & `RnDNews-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 setup(
-    version='0.1.1',
+    version='0.1.2',
     name='RnDNews',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(include=['RnDNews']),
```

