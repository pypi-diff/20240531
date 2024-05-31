# Comparing `tmp/botasaurus2-1.4.8.tar.gz` & `tmp/botasaurus2-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus2-1.4.8.tar", max compression
+gzip compressed data, was "botasaurus2-1.4.9.tar", max compression
```

## Comparing `botasaurus2-1.4.8.tar` & `botasaurus2-1.4.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.4.8/AUTHORS
--rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.4.8/LICENSE
--rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.4.8/README.md
--rw-r--r--   0        0        0      854 2024-04-15 19:45:21.210506 botasaurus2-1.4.8/botasaurus/__init__.py
--rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.4.8/botasaurus/_id.py
--rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.4.8/botasaurus/accept_google_cookies.py
--rw-r--r--   0        0        0    57750 2024-04-15 18:54:34.470840 botasaurus2-1.4.8/botasaurus/anti_detect_driver.py
--rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.4.8/botasaurus/anti_detect_requests.py
--rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.4.8/botasaurus/base_data.py
--rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.4.8/botasaurus/beep_utils.py
--rw-r--r--   0        0        0     2868 2024-04-12 14:30:05.866696 botasaurus2-1.4.8/botasaurus/botasaurus_storage.py
--rw-r--r--   0        0        0      944 2024-04-11 21:17:56.332972 botasaurus2-1.4.8/botasaurus/bt.py
--rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.4.8/botasaurus/cache.py
--rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.4.8/botasaurus/calc_max_parallel_browsers.py
--rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.4.8/botasaurus/captcha.py
--rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.4.8/botasaurus/check_and_download_driver.py
--rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.4.8/botasaurus/chrome_launcher_adapter.py
--rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.4.8/botasaurus/cl.py
--rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.4.8/botasaurus/close.py
--rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.4.8/botasaurus/constants.py
--rw-r--r--   0        0        0    15623 2024-04-20 18:10:56.213281 botasaurus2-1.4.8/botasaurus/create_driver_utils.py
--rw-r--r--   0        0        0    12501 2024-05-06 13:53:07.930494 botasaurus2-1.4.8/botasaurus/create_stealth_driver.py
--rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/creators.py
--rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/decorator_helpers.py
--rw-r--r--   0        0        0    39495 2024-04-19 09:20:51.822788 botasaurus2-1.4.8/botasaurus/decorators.py
--rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/decorators_utils.py
--rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/download_driver.py
--rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/driver_about.py
--rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/exceptions.py
--rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/formats.py
--rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/get_chrome_version.py
--rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.4.8/botasaurus/got_adapter.py
--rw-r--r--   0        0        0     2438 2024-04-12 14:30:10.786777 botasaurus2-1.4.8/botasaurus/ip_utils.py
--rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/list_utils.py
--rw-r--r--   0        0        0     3326 2024-04-11 20:48:02.911490 botasaurus2-1.4.8/botasaurus/local_storage.py
--rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/local_storage_driver.py
--rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/opponent.py
--rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.4.8/botasaurus/output.py
--rw-r--r--   0        0        0     4964 2024-04-12 14:01:33.922678 botasaurus2-1.4.8/botasaurus/profile.py
--rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.4.8/botasaurus/shortcuts.py
--rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/sitemap.py
--rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.4.8/botasaurus/str_utils.py
--rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/temp_mail.py
--rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/usage.py
--rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/user_agent.py
--rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/user_generator.py
--rw-r--r--   0        0        0     8611 2024-04-15 14:50:43.118678 botasaurus2-1.4.8/botasaurus/utils.py
--rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/wait.py
--rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.4.8/botasaurus/window_size.py
--rw-r--r--   0        0        0      848 2024-05-06 13:54:10.526135 botasaurus2-1.4.8/pyproject.toml
--rw-r--r--   0        0        0    52119 1970-01-01 00:00:00.000000 botasaurus2-1.4.8/PKG-INFO
+-rw-r--r--   0        0        0      217 2024-03-15 22:38:58.098040 botasaurus2-1.4.9/AUTHORS
+-rw-r--r--   0        0        0     1073 2024-03-15 22:38:58.098040 botasaurus2-1.4.9/LICENSE
+-rw-r--r--   0        0        0    50976 2024-03-19 13:44:59.662333 botasaurus2-1.4.9/README.md
+-rw-r--r--   0        0        0      854 2024-04-15 19:45:21.210506 botasaurus2-1.4.9/botasaurus/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-15 22:38:58.098040 botasaurus2-1.4.9/botasaurus/_id.py
+-rw-r--r--   0        0        0     1034 2024-03-15 22:38:58.098040 botasaurus2-1.4.9/botasaurus/accept_google_cookies.py
+-rw-r--r--   0        0        0    57750 2024-04-15 18:54:34.470840 botasaurus2-1.4.9/botasaurus/anti_detect_driver.py
+-rw-r--r--   0        0        0     4485 2024-04-11 15:00:22.756112 botasaurus2-1.4.9/botasaurus/anti_detect_requests.py
+-rw-r--r--   0        0        0     3549 2024-03-15 22:38:58.098040 botasaurus2-1.4.9/botasaurus/base_data.py
+-rw-r--r--   0        0        0      800 2024-03-15 22:38:58.098040 botasaurus2-1.4.9/botasaurus/beep_utils.py
+-rw-r--r--   0        0        0     2868 2024-04-12 14:30:05.866696 botasaurus2-1.4.9/botasaurus/botasaurus_storage.py
+-rw-r--r--   0        0        0      944 2024-04-11 21:17:56.332972 botasaurus2-1.4.9/botasaurus/bt.py
+-rw-r--r--   0        0        0     7486 2024-03-15 22:38:58.098040 botasaurus2-1.4.9/botasaurus/cache.py
+-rw-r--r--   0        0        0     2114 2024-03-15 22:38:58.098040 botasaurus2-1.4.9/botasaurus/calc_max_parallel_browsers.py
+-rw-r--r--   0        0        0    28154 2024-04-11 15:00:22.756112 botasaurus2-1.4.9/botasaurus/captcha.py
+-rw-r--r--   0        0        0      566 2024-03-15 22:38:58.098040 botasaurus2-1.4.9/botasaurus/check_and_download_driver.py
+-rw-r--r--   0        0        0      362 2024-03-15 22:38:58.098040 botasaurus2-1.4.9/botasaurus/chrome_launcher_adapter.py
+-rw-r--r--   0        0        0    14871 2024-03-15 22:38:58.098040 botasaurus2-1.4.9/botasaurus/cl.py
+-rw-r--r--   0        0        0      946 2024-03-15 22:38:58.098040 botasaurus2-1.4.9/botasaurus/close.py
+-rw-r--r--   0        0        0      256 2024-03-20 15:48:31.573396 botasaurus2-1.4.9/botasaurus/constants.py
+-rw-r--r--   0        0        0    15623 2024-04-20 18:10:56.213281 botasaurus2-1.4.9/botasaurus/create_driver_utils.py
+-rw-r--r--   0        0        0    12501 2024-05-06 13:53:07.930494 botasaurus2-1.4.9/botasaurus/create_stealth_driver.py
+-rw-r--r--   0        0        0     1820 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/creators.py
+-rw-r--r--   0        0        0     4130 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/decorator_helpers.py
+-rw-r--r--   0        0        0    39495 2024-04-19 09:20:51.822788 botasaurus2-1.4.9/botasaurus/decorators.py
+-rw-r--r--   0        0        0      491 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/decorators_utils.py
+-rw-r--r--   0        0        0     1617 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/download_driver.py
+-rw-r--r--   0        0        0      459 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/driver_about.py
+-rw-r--r--   0        0        0       48 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/exceptions.py
+-rw-r--r--   0        0        0       84 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/formats.py
+-rw-r--r--   0        0        0    14839 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/get_chrome_version.py
+-rw-r--r--   0        0        0     8679 2024-04-11 15:00:22.756112 botasaurus2-1.4.9/botasaurus/got_adapter.py
+-rw-r--r--   0        0        0     2438 2024-04-12 14:30:10.786777 botasaurus2-1.4.9/botasaurus/ip_utils.py
+-rw-r--r--   0        0        0     1534 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/list_utils.py
+-rw-r--r--   0        0        0     3326 2024-04-11 20:48:02.911490 botasaurus2-1.4.9/botasaurus/local_storage.py
+-rw-r--r--   0        0        0     1674 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/local_storage_driver.py
+-rw-r--r--   0        0        0       77 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/opponent.py
+-rw-r--r--   0        0        0     7343 2024-03-19 13:44:59.666333 botasaurus2-1.4.9/botasaurus/output.py
+-rw-r--r--   0        0        0     4964 2024-04-12 14:01:33.922678 botasaurus2-1.4.9/botasaurus/profile.py
+-rw-r--r--   0        0        0      352 2024-03-19 19:06:20.087339 botasaurus2-1.4.9/botasaurus/shortcuts.py
+-rw-r--r--   0        0        0    22453 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/sitemap.py
+-rw-r--r--   0        0        0     2031 2024-03-19 13:44:59.666333 botasaurus2-1.4.9/botasaurus/str_utils.py
+-rw-r--r--   0        0        0     6298 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/temp_mail.py
+-rw-r--r--   0        0        0       54 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/usage.py
+-rw-r--r--   0        0        0     7457 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/user_agent.py
+-rw-r--r--   0        0        0     4194 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/user_generator.py
+-rw-r--r--   0        0        0     8611 2024-04-15 14:50:43.118678 botasaurus2-1.4.9/botasaurus/utils.py
+-rw-r--r--   0        0        0       57 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/wait.py
+-rw-r--r--   0        0        0     1183 2024-03-15 22:38:58.102041 botasaurus2-1.4.9/botasaurus/window_size.py
+-rw-r--r--   0        0        0      849 2024-05-06 17:35:56.839067 botasaurus2-1.4.9/pyproject.toml
+-rw-r--r--   0        0        0    52112 1970-01-01 00:00:00.000000 botasaurus2-1.4.9/PKG-INFO
```

### Comparing `botasaurus2-1.4.8/LICENSE` & `botasaurus2-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/README.md` & `botasaurus2-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/__init__.py` & `botasaurus2-1.4.9/botasaurus/__init__.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/accept_google_cookies.py` & `botasaurus2-1.4.9/botasaurus/accept_google_cookies.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/anti_detect_driver.py` & `botasaurus2-1.4.9/botasaurus/anti_detect_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/anti_detect_requests.py` & `botasaurus2-1.4.9/botasaurus/anti_detect_requests.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/base_data.py` & `botasaurus2-1.4.9/botasaurus/base_data.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/beep_utils.py` & `botasaurus2-1.4.9/botasaurus/beep_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/botasaurus_storage.py` & `botasaurus2-1.4.9/botasaurus/botasaurus_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/bt.py` & `botasaurus2-1.4.9/botasaurus/bt.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/cache.py` & `botasaurus2-1.4.9/botasaurus/cache.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/calc_max_parallel_browsers.py` & `botasaurus2-1.4.9/botasaurus/calc_max_parallel_browsers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/captcha.py` & `botasaurus2-1.4.9/botasaurus/captcha.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/check_and_download_driver.py` & `botasaurus2-1.4.9/botasaurus/check_and_download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/cl.py` & `botasaurus2-1.4.9/botasaurus/cl.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/close.py` & `botasaurus2-1.4.9/botasaurus/close.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/create_driver_utils.py` & `botasaurus2-1.4.9/botasaurus/create_driver_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/create_stealth_driver.py` & `botasaurus2-1.4.9/botasaurus/create_stealth_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/creators.py` & `botasaurus2-1.4.9/botasaurus/creators.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/decorator_helpers.py` & `botasaurus2-1.4.9/botasaurus/decorator_helpers.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/decorators.py` & `botasaurus2-1.4.9/botasaurus/decorators.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/download_driver.py` & `botasaurus2-1.4.9/botasaurus/download_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/get_chrome_version.py` & `botasaurus2-1.4.9/botasaurus/get_chrome_version.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/got_adapter.py` & `botasaurus2-1.4.9/botasaurus/got_adapter.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/ip_utils.py` & `botasaurus2-1.4.9/botasaurus/ip_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/list_utils.py` & `botasaurus2-1.4.9/botasaurus/list_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/local_storage.py` & `botasaurus2-1.4.9/botasaurus/local_storage.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/local_storage_driver.py` & `botasaurus2-1.4.9/botasaurus/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/output.py` & `botasaurus2-1.4.9/botasaurus/output.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/profile.py` & `botasaurus2-1.4.9/botasaurus/profile.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/sitemap.py` & `botasaurus2-1.4.9/botasaurus/sitemap.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/str_utils.py` & `botasaurus2-1.4.9/botasaurus/str_utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/temp_mail.py` & `botasaurus2-1.4.9/botasaurus/temp_mail.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/user_agent.py` & `botasaurus2-1.4.9/botasaurus/user_agent.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/user_generator.py` & `botasaurus2-1.4.9/botasaurus/user_generator.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/utils.py` & `botasaurus2-1.4.9/botasaurus/utils.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/botasaurus/window_size.py` & `botasaurus2-1.4.9/botasaurus/window_size.py`

 * *Files identical despite different names*

### Comparing `botasaurus2-1.4.8/pyproject.toml` & `botasaurus2-1.4.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "botasaurus2"
-version = "1.4.8"
+version = "1.4.9"
 description = "Patching fork of botasaurus, The All in One Framework to build Awesome Scrapers."
 authors = ["Chetan Jain <chetan@omkar.cloud>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "botasaurus", from = "."}]
 
 [tool.poetry.dependencies]
@@ -17,15 +17,15 @@
 beautifulsoup4 = "^4.11.2"
 chromedriver-autoinstaller-fix = "^1.0.6"
 cloudscraper = "^1.2.71"
 selenium = "^4.9.0"
 botasaurus-proxy-authentication = "^1.0.12"
 capsolver-extension-python = "^1.0.1"
 lxml = "^5.1.0"
-aigents = "^0.7.1"
+aigents = ">=0.7.2"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 flake8 = "^7.0.0"
 ipykernel = "^6.29.4"
```

### Comparing `botasaurus2-1.4.8/PKG-INFO` & `botasaurus2-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: botasaurus2
-Version: 1.4.8
+Version: 1.4.9
 Summary: Patching fork of botasaurus, The All in One Framework to build Awesome Scrapers.
 License: MIT
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aigents (>=0.7.1,<0.8.0)
+Requires-Dist: aigents (>=0.7.2)
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
 Requires-Dist: botasaurus-proxy-authentication (>=1.0.12,<2.0.0)
 Requires-Dist: capsolver-extension-python (>=1.0.1,<2.0.0)
 Requires-Dist: chromedriver-autoinstaller-fix (>=1.0.6,<2.0.0)
 Requires-Dist: cloudscraper (>=1.2.71,<2.0.0)
 Requires-Dist: javascript-fixes (>=1.1.21,<2.0.0)
 Requires-Dist: joblib (>=1.3.2,<2.0.0)
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: botasaurus2 Version: 1.4.8 Summary: Patching fork
+Metadata-Version: 2.1 Name: botasaurus2 Version: 1.4.9 Summary: Patching fork
 of botasaurus, The All in One Framework to build Awesome Scrapers. License: MIT
 Author: Chetan Jain Author-email: chetan@omkar.cloud Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
-Programming Language :: Python :: 3.12 Requires-Dist: aigents (>=0.7.1,<0.8.0)
+Programming Language :: Python :: 3.12 Requires-Dist: aigents (>=0.7.2)
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0) Requires-Dist: botasaurus-
 proxy-authentication (>=1.0.12,<2.0.0) Requires-Dist: capsolver-extension-
 python (>=1.0.1,<2.0.0) Requires-Dist: chromedriver-autoinstaller-fix
 (>=1.0.6,<2.0.0) Requires-Dist: cloudscraper (>=1.2.71,<2.0.0) Requires-Dist:
 javascript-fixes (>=1.1.21,<2.0.0) Requires-Dist: joblib (>=1.3.2,<2.0.0)
 Requires-Dist: lxml (>=5.1.0,<6.0.0) Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0) Requires-Dist: requests
```

