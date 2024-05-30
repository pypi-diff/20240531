# Comparing `tmp/social_auth_gsis-0.5.3.tar.gz` & `tmp/social_auth_gsis-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social_auth_gsis-0.5.3.tar", max compression
+gzip compressed data, was "social_auth_gsis-0.5.4.tar", max compression
```

## Comparing `social_auth_gsis-0.5.3.tar` & `social_auth_gsis-0.5.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4521 2024-03-01 12:27:31.225982 social_auth_gsis-0.5.3/README.md
--rw-r--r--   0        0        0      418 2024-05-30 23:14:19.772431 social_auth_gsis-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     4580 2024-03-01 12:27:31.226078 social_auth_gsis-0.5.3/social_auth_gsis/backends.py
--rw-r--r--   0        0        0     1123 2024-03-01 11:12:54.719026 social_auth_gsis-0.5.3/social_auth_gsis/pipeline/social_auth.py
--rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 social_auth_gsis-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     4521 2024-03-01 12:27:31.225982 social_auth_gsis-0.5.4/README.md
+-rw-r--r--   0        0        0      418 2024-05-30 23:33:43.982737 social_auth_gsis-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     4556 2024-05-30 23:33:40.932710 social_auth_gsis-0.5.4/social_auth_gsis/backends.py
+-rw-r--r--   0        0        0     1123 2024-03-01 11:12:54.719026 social_auth_gsis-0.5.4/social_auth_gsis/pipeline/social_auth.py
+-rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 social_auth_gsis-0.5.4/PKG-INFO
```

### Comparing `social_auth_gsis-0.5.3/README.md` & `social_auth_gsis-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `social_auth_gsis-0.5.3/social_auth_gsis/backends.py` & `social_auth_gsis-0.5.4/social_auth_gsis/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from django.conf import settings
-from social_core.backends.oauth import BaseOAuth2
 import requests
 import xmltodict
+from django.conf import settings
+from social_core.backends.oauth import BaseOAuth2
 
 
 class GSISOAuth2(BaseOAuth2):
     """GSIS OAuth 2.0 authentication backend"""
 
     name = "gsis"
     AUTHORIZATION_URL = "https://www1.gsis.gr/oauth2server/oauth/authorize"
     ACCESS_TOKEN_URL = "https://www1.gsis.gr/oauth2server/oauth/token"
-    USER_DATA_URL_URL = "https://www1.gsis.gr/oauth2server/userinfo?format=xml"
+    USER_DATA_URL = "https://www1.gsis.gr/oauth2server/userinfo?format=xml"
     ACCESS_TOKEN_METHOD = "POST"
     DEFAULT_SCOPE = ["read"]
     SCOPE_SEPARATOR = ","
     allow_new_users = True
 
     def get_redirect_uri(self, state=None):
         return settings.SOCIAL_AUTH_GSIS_REDIRECT_URL
@@ -70,45 +70,45 @@
 
 class GSISOAuth2Testing(GSISOAuth2):
     """GSIS OAuth 2.0 testing authentication backend"""
 
     name = "gsis_testing"
     AUTHORIZATION_URL = "https://test.gsis.gr/oauth2server/oauth/authorize"
     ACCESS_TOKEN_URL = "https://test.gsis.gr/oauth2server/oauth/token"
-    USER_DATA_URL_URL = "https://test.gsis.gr/oauth2server/userinfo?format=xml"
+    USER_DATA_URL = "https://test.gsis.gr/oauth2server/userinfo?format=xml"
 
 
 class GSISOTPOAuth2(GSISOAuth2):
     """GSIS OAuth 2.0 authentication backend with OTP"""
 
     name = "gsis_otp"
     AUTHORIZATION_URL = "https://www1.gsis.gr/oauth2serverotp/oauth/authorize"
     ACCESS_TOKEN_URL = "https://www1.gsis.gr/oauth2serverotp/oauth/token"
-    USER_DATA_URL_URL = "https://www1.gsis.gr/oauth2serverotp/userinfo?format=xml"
+    USER_DATA_URL = "https://www1.gsis.gr/oauth2serverotp/userinfo?format=xml"
 
     def get_redirect_uri(self, state=None):
         return settings.SOCIAL_AUTH_GSIS_OTP_REDIRECT_URL
 
 
 class GSISOTPOAuth2Testing(GSISOTPOAuth2):
     """GSIS OAuth 2.0 testing authentication backend with OTP"""
 
     name = "gsis_otp_testing"
     AUTHORIZATION_URL = "https://test.gsis.gr/oauth2serverotp/oauth/authorize"
     ACCESS_TOKEN_URL = "https://test.gsis.gr/oauth2serverotp/oauth/token"
-    USER_DATA_URL_URL = "https://test.gsis.gr/oauth2serverotp/userinfo?format=xml"
+    USER_DATA_URL = "https://test.gsis.gr/oauth2serverotp/userinfo?format=xml"
 
 
 class GSISPAOAuth2(GSISOAuth2):
     """GSIS OAuth 2.0 authentication backend for Public Administration"""
 
     name = "gsis_pa"
     AUTHORIZATION_URL = "https://www1.gsis.gr/oauth2servergov/oauth/authorize"
     ACCESS_TOKEN_URL = "https://www1.gsis.gr/oauth2servergov/oauth/token"
-    USER_DATA_URL_URL = "https://www1.gsis.gr/oauth2servergov/userinfo?format=xml"
+    USER_DATA_URL = "https://www1.gsis.gr/oauth2servergov/userinfo?format=xml"
     allow_new_users = False
 
     def get_redirect_uri(self, state=None):
         return settings.SOCIAL_AUTH_GSIS_PA_REDIRECT_URL
 
     def get_username_by_tax_id(self, tax_id):
         return f"gsis-pa-{tax_id}"
@@ -116,8 +116,8 @@
 
 class GSISPAOAuth2Testing(GSISPAOAuth2):
     """GSIS OAuth 2.0 testing authentication backend for Public Administration"""
 
     name = "gsis_pa_testing"
     AUTHORIZATION_URL = "https://test.gsis.gr/oauth2servergov/oauth/authorize"
     ACCESS_TOKEN_URL = "https://test.gsis.gr/oauth2servergov/oauth/token"
-    USER_DATA_URL_URL = "https://test.gsis.gr/oauth2servergov/userinfo?format=xml"
+    USER_DATA_URL = "https://test.gsis.gr/oauth2servergov/userinfo?format=xml"
```

### Comparing `social_auth_gsis-0.5.3/social_auth_gsis/pipeline/social_auth.py` & `social_auth_gsis-0.5.4/social_auth_gsis/pipeline/social_auth.py`

 * *Files identical despite different names*

### Comparing `social_auth_gsis-0.5.3/PKG-INFO` & `social_auth_gsis-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: social-auth-gsis
-Version: 0.5.3
+Version: 0.5.4
 Summary: Social Auth backend for GSIS
 License: MIT
 Author: Paris Kasidiaris
 Author-email: paris@withlogic.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

