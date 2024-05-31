# Comparing `tmp/lb_mail-1.0.0.tar.gz` & `tmp/lb_mail-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lb_mail-1.0.0.tar", last modified: Fri May 31 14:49:43 2024, max compression
+gzip compressed data, was "lb_mail-1.1.0.tar", last modified: Fri May 31 17:50:28 2024, max compression
```

## Comparing `lb_mail-1.0.0.tar` & `lb_mail-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:49:43.228869 lb_mail-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-31 14:49:43.228869 lb_mail-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-31 14:49:35.000000 lb_mail-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:49:43.224869 lb_mail-1.0.0/lbMail/
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-05-31 14:49:35.000000 lb_mail-1.0.0/lbMail/LbMail.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-31 14:49:35.000000 lb_mail-1.0.0/lbMail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:49:43.228869 lb_mail-1.0.0/lb_mail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-31 14:49:43.000000 lb_mail-1.0.0/lb_mail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 14:49:43.000000 lb_mail-1.0.0/lb_mail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:49:43.000000 lb_mail-1.0.0/lb_mail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 14:49:43.000000 lb_mail-1.0.0/lb_mail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:49:43.228869 lb_mail-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-31 14:49:35.000000 lb_mail-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:50:28.068513 lb_mail-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-31 17:50:28.068513 lb_mail-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-31 17:50:19.000000 lb_mail-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:50:28.064513 lb_mail-1.1.0/lbMail/
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-31 17:50:19.000000 lb_mail-1.1.0/lbMail/LbMail.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-31 17:50:19.000000 lb_mail-1.1.0/lbMail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 17:50:28.068513 lb_mail-1.1.0/lb_mail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-31 17:50:28.000000 lb_mail-1.1.0/lb_mail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 17:50:28.000000 lb_mail-1.1.0/lb_mail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 17:50:28.000000 lb_mail-1.1.0/lb_mail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 17:50:28.000000 lb_mail-1.1.0/lb_mail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 17:50:28.068513 lb_mail-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-31 17:50:19.000000 lb_mail-1.1.0/setup.py
```

### Comparing `lb_mail-1.0.0/PKG-INFO` & `lb_mail-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lb-mail
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library with data models by lb services
 Author: Lucas Barros
 Author-email: lucasbarros2000@hotmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lb_mail-1.0.0/README.md` & `lb_mail-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `lb_mail-1.0.0/lbMail/LbMail.py` & `lb_mail-1.1.0/lbMail/LbMail.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 __author__ = 'Lucas Barros'
 __version__ = 1.0
 __maintainer__ = 'Lucas Barros'
 __email__ = 'lucasbarros2000@hotmail.com'
 __status__ = 'Production'
 
 
+import json
 import os
 import requests
 from lbLogger.LbLogger import LbLogger
 from requests.auth import HTTPBasicAuth
 from typing import Any
+from typing import Dict
 from typing import List
 from typing import Union
 
 
 class LbMail:
 
     def __init__(self):
@@ -41,14 +43,38 @@
             if len(to_email) > 1:
                 bodyEmail['cc'] = ','.join([str(y) for y in to_email[1:]])
 
         return requests.post(self.__url_mail_gun,
                              auth=HTTPBasicAuth("api", self.__token_mail_gun),
                              data=bodyEmail)
 
+    def send_by_template(self, to_email: Union[List[str], str], template_name: str, template_variables: Dict)\
+            -> requests.Response:
+        """
+        Function for send email with html body
+        :param to_email: To email(s) for send mail
+        :param template_name: Template name
+        :param template_variables: Template variables
+        :return: Response status email sent
+        """
+
+        bodyEmail = dict()
+        if isinstance(to_email, str):
+            bodyEmail: dict = {"to": to_email, "from": self.__from_email, "template": template_name,
+                "h:X-Mailgun-Variables": json.dumps(template_variables)}
+        elif isinstance(to_email, list):
+            bodyEmail: dict = {"to": to_email[0], "from": self.__from_email, "template": template_name,
+                "h:X-Mailgun-Variables": json.dumps(template_variables)}
+            if len(to_email) > 1:
+                bodyEmail['cc'] = ','.join([str(y) for y in to_email[1:]])
+
+        return requests.post(self.__url_mail_gun,
+                             auth=HTTPBasicAuth("api", self.__token_mail_gun),
+                             data=bodyEmail)
+
     def check_and_read_environment_variables(self, variable: Any) -> Any:
         """
         Function for check and read environment variable
         :param variable: Variable for check
         :return: Environment variable
         """
```

### Comparing `lb_mail-1.0.0/lb_mail.egg-info/PKG-INFO` & `lb_mail-1.1.0/lb_mail.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lb-mail
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library with data models by lb services
 Author: Lucas Barros
 Author-email: lucasbarros2000@hotmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lb_mail-1.0.0/setup.py` & `lb_mail-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="lb-mail",
-    version="1.0.0",
+    version="1.1.0",
     author="Lucas Barros",
     author_email="lucasbarros2000@hotmail.com",
     description="Library with data models by lb services",
     packages=setuptools.find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     classifiers=[
```

