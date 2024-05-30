# Comparing `tmp/social_auth_gsis-0.5.4.tar.gz` & `tmp/social_auth_gsis-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "social_auth_gsis-0.5.4.tar", max compression
+gzip compressed data, was "social_auth_gsis-0.5.5.tar", max compression
```

## Comparing `social_auth_gsis-0.5.4.tar` & `social_auth_gsis-0.5.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     4521 2024-03-01 12:27:31.225982 social_auth_gsis-0.5.4/README.md
--rw-r--r--   0        0        0      418 2024-05-30 23:33:43.982737 social_auth_gsis-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     4556 2024-05-30 23:33:40.932710 social_auth_gsis-0.5.4/social_auth_gsis/backends.py
--rw-r--r--   0        0        0     1123 2024-03-01 11:12:54.719026 social_auth_gsis-0.5.4/social_auth_gsis/pipeline/social_auth.py
--rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 social_auth_gsis-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0     4521 2024-03-01 12:27:31.225982 social_auth_gsis-0.5.5/README.md
+-rw-r--r--   0        0        0      418 2024-05-30 23:40:46.510706 social_auth_gsis-0.5.5/pyproject.toml
+-rw-r--r--   0        0        0     4556 2024-05-30 23:33:40.932710 social_auth_gsis-0.5.5/social_auth_gsis/backends.py
+-rw-r--r--   0        0        0     1115 2024-05-30 23:40:40.143849 social_auth_gsis-0.5.5/social_auth_gsis/pipeline/social_auth.py
+-rw-r--r--   0        0        0     5329 1970-01-01 00:00:00.000000 social_auth_gsis-0.5.5/PKG-INFO
```

### Comparing `social_auth_gsis-0.5.4/README.md` & `social_auth_gsis-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `social_auth_gsis-0.5.4/social_auth_gsis/backends.py` & `social_auth_gsis-0.5.5/social_auth_gsis/backends.py`

 * *Files identical despite different names*

### Comparing `social_auth_gsis-0.5.4/social_auth_gsis/pipeline/social_auth.py` & `social_auth_gsis-0.5.5/social_auth_gsis/pipeline/social_auth.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from django.contrib.auth.models import get_user_model
-from social_core.exceptions import AuthForbidden, AuthAlreadyAssociated
-
+from django.contrib.auth import get_user_model
+from social_core.exceptions import AuthAlreadyAssociated, AuthForbidden
 
 User = get_user_model()
 
 
 def social_user(backend, uid, user=None, *args, **kwargs):
     user_qs = User.objects.filter(username=kwargs["details"]["username"])
     backend_allows_new_users = getattr(backend, "allow_new_users", False)
```

### Comparing `social_auth_gsis-0.5.4/PKG-INFO` & `social_auth_gsis-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: social-auth-gsis
-Version: 0.5.4
+Version: 0.5.5
 Summary: Social Auth backend for GSIS
 License: MIT
 Author: Paris Kasidiaris
 Author-email: paris@withlogic.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

