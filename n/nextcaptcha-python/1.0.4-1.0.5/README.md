# Comparing `tmp/nextcaptcha_python-1.0.4.tar.gz` & `tmp/nextcaptcha_python-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextcaptcha_python-1.0.4.tar", last modified: Thu Apr 18 02:52:37 2024, max compression
+gzip compressed data, was "nextcaptcha_python-1.0.5.tar", last modified: Fri May 31 02:11:27 2024, max compression
```

## Comparing `nextcaptcha_python-1.0.4.tar` & `nextcaptcha_python-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:52:37.923367 nextcaptcha_python-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-18 02:52:34.000000 nextcaptcha_python-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-18 02:52:37.923367 nextcaptcha_python-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-18 02:52:34.000000 nextcaptcha_python-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:52:37.923367 nextcaptcha_python-1.0.4/nextcaptcha/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-18 02:52:34.000000 nextcaptcha_python-1.0.4/nextcaptcha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13087 2024-04-18 02:52:34.000000 nextcaptcha_python-1.0.4/nextcaptcha/next.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:52:37.923367 nextcaptcha_python-1.0.4/nextcaptcha_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-04-18 02:52:37.000000 nextcaptcha_python-1.0.4/nextcaptcha_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-04-18 02:52:37.000000 nextcaptcha_python-1.0.4/nextcaptcha_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 02:52:37.000000 nextcaptcha_python-1.0.4/nextcaptcha_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 02:52:37.000000 nextcaptcha_python-1.0.4/nextcaptcha_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-18 02:52:37.000000 nextcaptcha_python-1.0.4/nextcaptcha_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 02:52:37.923367 nextcaptcha_python-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-18 02:52:34.000000 nextcaptcha_python-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:11:27.016471 nextcaptcha_python-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-31 02:11:23.000000 nextcaptcha_python-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-31 02:11:27.016471 nextcaptcha_python-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-31 02:11:23.000000 nextcaptcha_python-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:11:27.016471 nextcaptcha_python-1.0.5/nextcaptcha/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-31 02:11:23.000000 nextcaptcha_python-1.0.5/nextcaptcha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-05-31 02:11:23.000000 nextcaptcha_python-1.0.5/nextcaptcha/next.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:11:27.016471 nextcaptcha_python-1.0.5/nextcaptcha_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-31 02:11:27.000000 nextcaptcha_python-1.0.5/nextcaptcha_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-31 02:11:27.000000 nextcaptcha_python-1.0.5/nextcaptcha_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 02:11:27.000000 nextcaptcha_python-1.0.5/nextcaptcha_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 02:11:27.000000 nextcaptcha_python-1.0.5/nextcaptcha_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 02:11:27.000000 nextcaptcha_python-1.0.5/nextcaptcha_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 02:11:27.016471 nextcaptcha_python-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-31 02:11:23.000000 nextcaptcha_python-1.0.5/setup.py
```

### Comparing `nextcaptcha_python-1.0.4/LICENSE` & `nextcaptcha_python-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nextcaptcha_python-1.0.4/PKG-INFO` & `nextcaptcha_python-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcaptcha-python
-Version: 1.0.4
+Version: 1.0.5
 Summary: NextCaptcha Captcha Solving Service Api Wrapper for Python to solving recaptcha v2, v3,recapthcha moible,hcaptcha,funcaptcha
 Home-page: https://github.com/nextcaptcha/nextcaptcha-python/
 Author: nextcaptcha
 Author-email: support@nextcaptcha.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nextcaptcha_python-1.0.4/README.md` & `nextcaptcha_python-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nextcaptcha_python-1.0.4/nextcaptcha/next.py` & `nextcaptcha_python-1.0.5/nextcaptcha/next.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 logging.basicConfig(level=logging.INFO)
 
 RECAPTCHAV2_TYPE = "RecaptchaV2TaskProxyless"
 RECAPTCHAV2_ENTERPRISE_TYPE = "RecaptchaV2EnterpriseTaskProxyless"
 RECAPTCHAV3_PROXYLESS_TYPE = "RecaptchaV3TaskProxyless"
 RECAPTCHAV3_TYPE = "RecaptchaV3Task"
-RECAPTCHA_MOBILE_TYPE = "RecaptchaMobileProxyless"
+RECAPTCHA_MOBILE_PROXYLESS_TYPE = "ReCaptchaMobileTaskProxyLess"
+RECAPTCHA_MOBILE_TYPE = "ReCaptchaMobileTask"
 HCAPTCHA_TYPE = "HCaptchaTask"
 HCAPTCHA_PROXYLESS_TYPE = "HCaptchaTaskProxyless"
 HCAPTCHA_ENTERPRISE_TYPE = "HCaptchaEnterpriseTask"
 FUNCAPTCHA_TYPE = "FunCaptchaTask"
 FUNCAPTCHA_PROXYLESS_TYPE = "FunCaptchaTaskProxyless"
 
 TIMEOUT = 45
@@ -170,29 +171,38 @@
             task["proxyType"] = proxy_type
             task["proxyAddress"] = proxy_address
             task["proxyPort"] = proxy_port
             task["proxyLogin"] = proxy_login
             task["proxyPassword"] = proxy_password
         return self.api._send(task)
 
-    def recaptcha_mobile(self, app_key: str, app_package_name: str = "", app_action: str = "") -> dict:
+    def recaptcha_mobile(self, app_key: str, app_package_name: str = "", app_action: str = "", proxy_type: str = "",
+                         proxy_address: str = "", proxy_port: int = 0, proxy_login: str = "",
+                         proxy_password: str = "") -> dict:
         """
         Solve Mobile reCAPTCHA challenge.
 
         :param app_key: The app key of the Mobile reCAPTCHA.
         :param app_package_name: Optional. The package name of the mobile app.
         :param app_action: Optional. The action parameter to use for the Mobile reCAPTCHA.
         :return: A dictionary containing the solution of the Mobile reCAPTCHA.
         """
         task = {
-            "type": RECAPTCHA_MOBILE_TYPE,
+            "type": RECAPTCHA_MOBILE_PROXYLESS_TYPE,
             "appKey": app_key,
             "appPackageName": app_package_name,
             "appAction": app_action,
         }
+        if proxy_address != "":
+            task["type"] = RECAPTCHA_MOBILE_TYPE
+            task["proxyType"] = proxy_type
+            task["proxyAddress"] = proxy_address
+            task["proxyPort"] = proxy_port
+            task["proxyLogin"] = proxy_login
+            task["proxyPassword"] = proxy_password
         return self.api._send(task)
 
     def hcaptcha(self, website_url: str, website_key: str, is_invisible: bool = False, enterprise_payload: dict = {},
                  proxy_type: str = "", proxy_address: str = "", proxy_port: int = 0, proxy_login: str = "",
                  proxy_password: str = "") -> dict:
         """
         Solve hCaptcha challenge.
```

### Comparing `nextcaptcha_python-1.0.4/nextcaptcha_python.egg-info/PKG-INFO` & `nextcaptcha_python-1.0.5/nextcaptcha_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcaptcha-python
-Version: 1.0.4
+Version: 1.0.5
 Summary: NextCaptcha Captcha Solving Service Api Wrapper for Python to solving recaptcha v2, v3,recapthcha moible,hcaptcha,funcaptcha
 Home-page: https://github.com/nextcaptcha/nextcaptcha-python/
 Author: nextcaptcha
 Author-email: support@nextcaptcha.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `nextcaptcha_python-1.0.4/setup.py` & `nextcaptcha_python-1.0.5/setup.py`

 * *Files identical despite different names*

