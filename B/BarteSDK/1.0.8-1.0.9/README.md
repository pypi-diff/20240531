# Comparing `tmp/BarteSDK-1.0.8.tar.gz` & `tmp/BarteSDK-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BarteSDK-1.0.8.tar", last modified: Thu May 30 11:58:06 2024, max compression
+gzip compressed data, was "BarteSDK-1.0.9.tar", last modified: Thu May 30 12:07:01 2024, max compression
```

## Comparing `BarteSDK-1.0.8.tar` & `BarteSDK-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:58:06.120604 BarteSDK-1.0.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:58:06.116604 BarteSDK-1.0.8/BarteSDK.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 11:58:06.000000 BarteSDK-1.0.8/BarteSDK.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      372 2024-05-30 11:58:06.000000 BarteSDK-1.0.8/BarteSDK.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 11:58:06.000000 BarteSDK-1.0.8/BarteSDK.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 11:58:06.000000 BarteSDK-1.0.8/BarteSDK.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 11:58:06.000000 BarteSDK-1.0.8/BarteSDK.egg-info/top_level.txt
--rwxrwxr-x   0 root         (0) root         (0)        0 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 11:58:06.120604 BarteSDK-1.0.8/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     9363 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 11:58:06.120604 BarteSDK-1.0.8/bartesdk/
--rwxrwxr-x   0 root         (0) root         (0)      859 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/__init__.py
--rwxrwxr-x   0 root         (0) root         (0)     2216 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/base.py
--rwxrwxr-x   0 root         (0) root         (0)      198 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/buyers.py
--rwxrwxr-x   0 root         (0) root         (0)      198 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/charges.py
--rwxrwxr-x   0 root         (0) root         (0)      196 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/orders.py
--rwxrwxr-x   0 root         (0) root         (0)      209 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/paymentlinks.py
--rwxrwxr-x   0 root         (0) root         (0)      194 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/plans.py
--rwxrwxr-x   0 root         (0) root         (0)      210 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/subscriptions.py
--rwxrwxr-x   0 root         (0) root         (0)      210 2024-05-30 11:57:42.000000 BarteSDK-1.0.8/bartesdk/subseller.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 11:58:06.120604 BarteSDK-1.0.8/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)      551 2024-05-30 11:57:51.000000 BarteSDK-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 12:07:01.960448 BarteSDK-1.0.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 12:07:01.956448 BarteSDK-1.0.9/BarteSDK.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 12:07:01.000000 BarteSDK-1.0.9/BarteSDK.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      372 2024-05-30 12:07:01.000000 BarteSDK-1.0.9/BarteSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-30 12:07:01.000000 BarteSDK-1.0.9/BarteSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 12:07:01.000000 BarteSDK-1.0.9/BarteSDK.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-30 12:07:01.000000 BarteSDK-1.0.9/BarteSDK.egg-info/top_level.txt
+-rwxrwxr-x   0 root         (0) root         (0)        0 2024-05-30 12:06:37.000000 BarteSDK-1.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9638 2024-05-30 12:07:01.956448 BarteSDK-1.0.9/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     9363 2024-05-30 12:06:37.000000 BarteSDK-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-30 12:07:01.956448 BarteSDK-1.0.9/bartesdk/
+-rwxrwxr-x   0 root         (0) root         (0)      859 2024-05-30 12:06:37.000000 BarteSDK-1.0.9/bartesdk/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     2264 2024-05-30 12:06:37.000000 BarteSDK-1.0.9/bartesdk/base.py
+-rwxrwxr-x   0 root         (0) root         (0)      196 2024-05-30 12:06:37.000000 BarteSDK-1.0.9/bartesdk/buyers.py
+-rwxrwxr-x   0 root         (0) root         (0)      198 2024-05-30 12:06:37.000000 BarteSDK-1.0.9/bartesdk/charges.py
+-rwxrwxr-x   0 root         (0) root         (0)      196 2024-05-30 12:06:37.000000 BarteSDK-1.0.9/bartesdk/orders.py
+-rwxrwxr-x   0 root         (0) root         (0)      209 2024-05-30 12:06:37.000000 BarteSDK-1.0.9/bartesdk/paymentlinks.py
+-rwxrwxr-x   0 root         (0) root         (0)      194 2024-05-30 12:06:37.000000 BarteSDK-1.0.9/bartesdk/plans.py
+-rwxrwxr-x   0 root         (0) root         (0)      210 2024-05-30 12:06:37.000000 BarteSDK-1.0.9/bartesdk/subscriptions.py
+-rwxrwxr-x   0 root         (0) root         (0)      210 2024-05-30 12:06:37.000000 BarteSDK-1.0.9/bartesdk/subseller.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-30 12:07:01.960448 BarteSDK-1.0.9/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)      551 2024-05-30 12:06:46.000000 BarteSDK-1.0.9/setup.py
```

### Comparing `BarteSDK-1.0.8/BarteSDK.egg-info/PKG-INFO` & `BarteSDK-1.0.9/BarteSDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 1.0.8
+Version: 1.0.9
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-1.0.8/PKG-INFO` & `BarteSDK-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BarteSDK
-Version: 1.0.8
+Version: 1.0.9
 Summary: SDK para interação com a API da Barte.
 Author: Engenharia de Plataforma da Barte
 Author-email: devops@barte.com
 License: MIT
 Keywords: barte pay sdk
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `BarteSDK-1.0.8/README.md` & `BarteSDK-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.8/bartesdk/__init__.py` & `BarteSDK-1.0.9/bartesdk/__init__.py`

 * *Files identical despite different names*

### Comparing `BarteSDK-1.0.8/bartesdk/base.py` & `BarteSDK-1.0.9/bartesdk/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 
 class BaseAPI:
-    def __init__(self, api_key, base_url):
+    def __init__(self, api_key, env, api_version, path):
         self.api_key = api_key
-        self.base_url = base_url
+        self.base_url = self._get_base_url(env, api_version, path)
 
     def _get_base_url(self, env, api_version, path):
         if env == "prd":
             return f'https://api.barte.com/{api_version}/{path}'
         elif env == "sandbox":
             return f'https://sandbox-api.barte.com/{api_version}/{path}'
         else:
```

### Comparing `BarteSDK-1.0.8/setup.py` & `BarteSDK-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='BarteSDK',
-    version='1.0.8',
+    version='1.0.9',
     packages=find_packages(),
     install_requires=[
         'requests',
     ],
     author='Engenharia de Plataforma da Barte',
     author_email='devops@barte.com',
     description='SDK para interação com a API da Barte.',
```

