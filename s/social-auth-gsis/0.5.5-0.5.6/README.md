# Comparing `tmp/social_auth_gsis-0.5.5.tar.gz` & `tmp/social_auth_gsis-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social_auth_gsis-0.5.5.tar", max compression
+gzip compressed data, was "social_auth_gsis-0.5.6.tar", max compression
```

## Comparing `social_auth_gsis-0.5.5.tar` & `social_auth_gsis-0.5.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4521 2024-03-01 12:27:31.225982 social_auth_gsis-0.5.5/README.md
--rw-r--r--   0        0        0      418 2024-05-30 23:40:46.510706 social_auth_gsis-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     4556 2024-05-30 23:33:40.932710 social_auth_gsis-0.5.5/social_auth_gsis/backends.py
--rw-r--r--   0        0        0     1115 2024-05-30 23:40:40.143849 social_auth_gsis-0.5.5/social_auth_gsis/pipeline/social_auth.py
--rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 social_auth_gsis-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     4521 2024-03-01 12:27:31.225982 social_auth_gsis-0.5.6/README.md
+-rw-r--r--   0        0        0      418 2024-05-30 23:52:58.783299 social_auth_gsis-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     4683 2024-05-30 23:52:52.701676 social_auth_gsis-0.5.6/social_auth_gsis/backends.py
+-rw-r--r--   0        0        0     1115 2024-05-30 23:40:40.143849 social_auth_gsis-0.5.6/social_auth_gsis/pipeline/social_auth.py
+-rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 social_auth_gsis-0.5.6/PKG-INFO
```

### Comparing `social_auth_gsis-0.5.5/README.md` & `social_auth_gsis-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `social_auth_gsis-0.5.5/social_auth_gsis/backends.py` & `social_auth_gsis-0.5.6/social_auth_gsis/backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 
     def user_data(self, access_token, *args, **kwargs):
         user_data_headers = {"Authorization": f"Bearer {access_token}"}
         user_data_response = requests.get(
             self.USER_DATA_URL,
             headers=user_data_headers,
         )
+        if settings.DEBUG and settings.SOCIAL_AUTH_GSIS_DEBUG:
+            print(f"GSIS USER DATA: {user_data_response.text}")
         user_data_response.raise_for_status()
         user_data = xmltodict.parse(user_data_response.text)
         tax_id = user_data["root"]["userinfo"]["@taxid"].strip()
         username = self.get_username_by_tax_id(tax_id)
         first_name = user_data["root"]["userinfo"]["@firstname"].strip()
         last_name = user_data["root"]["userinfo"]["@lastname"].strip()
         response = {
```

### Comparing `social_auth_gsis-0.5.5/social_auth_gsis/pipeline/social_auth.py` & `social_auth_gsis-0.5.6/social_auth_gsis/pipeline/social_auth.py`

 * *Files identical despite different names*

### Comparing `social_auth_gsis-0.5.5/PKG-INFO` & `social_auth_gsis-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: social-auth-gsis
-Version: 0.5.5
+Version: 0.5.6
 Summary: Social Auth backend for GSIS
 License: MIT
 Author: Paris Kasidiaris
 Author-email: paris@withlogic.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

