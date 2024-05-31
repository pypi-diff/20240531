# Comparing `tmp/django_azure_auth-1.4.2.tar.gz` & `tmp/django_azure_auth-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_azure_auth-1.4.2.tar", max compression
+gzip compressed data, was "django_azure_auth-1.4.3.tar", max compression
```

## Comparing `django_azure_auth-1.4.2.tar` & `django_azure_auth-1.4.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1064 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/LICENSE
--rw-r--r--   0        0        0     6081 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/README.md
--rw-r--r--   0        0        0        0 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/__init__.py
--rw-r--r--   0        0        0      151 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/apps.py
--rw-r--r--   0        0        0      415 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/backends.py
--rw-r--r--   0        0        0      501 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/decorators.py
--rw-r--r--   0        0        0      333 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/exceptions.py
--rw-r--r--   0        0        0     7693 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/handlers.py
--rw-r--r--   0        0        0     1138 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/middleware.py
--rw-r--r--   0        0        0        0 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/tests/__init__.py
--rw-r--r--   0        0        0     2091 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/tests/conftest.py
--rw-r--r--   0        0        0     3943 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/tests/settings.py
--rw-r--r--   0        0        0     1473 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/tests/test_decorators.py
--rw-r--r--   0        0        0     3631 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/tests/test_middleware.py
--rw-r--r--   0        0        0    14080 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/tests/test_views.py
--rw-r--r--   0        0        0     1017 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/tests/urls.py
--rw-r--r--   0        0        0      324 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/urls.py
--rw-r--r--   0        0        0     1116 2024-05-30 16:59:38.082190 django_azure_auth-1.4.2/azure_auth/views.py
--rw-r--r--   0        0        0     1464 2024-05-30 16:59:38.082190 django_azure_auth-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     7062 1970-01-01 00:00:00.000000 django_azure_auth-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-31 13:50:52.375330 django_azure_auth-1.4.3/LICENSE
+-rw-r--r--   0        0        0     6081 2024-05-31 13:50:52.375330 django_azure_auth-1.4.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-31 13:50:52.375330 django_azure_auth-1.4.3/azure_auth/__init__.py
+-rw-r--r--   0        0        0      151 2024-05-31 13:50:52.375330 django_azure_auth-1.4.3/azure_auth/apps.py
+-rw-r--r--   0        0        0      415 2024-05-31 13:50:52.375330 django_azure_auth-1.4.3/azure_auth/backends.py
+-rw-r--r--   0        0        0      501 2024-05-31 13:50:52.375330 django_azure_auth-1.4.3/azure_auth/decorators.py
+-rw-r--r--   0        0        0      333 2024-05-31 13:50:52.379330 django_azure_auth-1.4.3/azure_auth/exceptions.py
+-rw-r--r--   0        0        0     7693 2024-05-31 13:50:52.379330 django_azure_auth-1.4.3/azure_auth/handlers.py
+-rw-r--r--   0        0        0     1138 2024-05-31 13:50:52.379330 django_azure_auth-1.4.3/azure_auth/middleware.py
+-rw-r--r--   0        0        0        0 2024-05-31 13:50:52.379330 django_azure_auth-1.4.3/azure_auth/tests/__init__.py
+-rw-r--r--   0        0        0     2091 2024-05-31 13:50:52.379330 django_azure_auth-1.4.3/azure_auth/tests/conftest.py
+-rw-r--r--   0        0        0     3943 2024-05-31 13:50:52.379330 django_azure_auth-1.4.3/azure_auth/tests/settings.py
+-rw-r--r--   0        0        0     1473 2024-05-31 13:50:52.379330 django_azure_auth-1.4.3/azure_auth/tests/test_decorators.py
+-rw-r--r--   0        0        0     3631 2024-05-31 13:50:52.379330 django_azure_auth-1.4.3/azure_auth/tests/test_middleware.py
+-rw-r--r--   0        0        0    14245 2024-05-31 13:50:52.379330 django_azure_auth-1.4.3/azure_auth/tests/test_views.py
+-rw-r--r--   0        0        0     1017 2024-05-31 13:50:52.379330 django_azure_auth-1.4.3/azure_auth/tests/urls.py
+-rw-r--r--   0        0        0      324 2024-05-31 13:50:52.379330 django_azure_auth-1.4.3/azure_auth/urls.py
+-rw-r--r--   0        0        0      260 2024-05-31 13:50:52.379330 django_azure_auth-1.4.3/azure_auth/utils.py
+-rw-r--r--   0        0        0     1283 2024-05-31 13:50:52.379330 django_azure_auth-1.4.3/azure_auth/views.py
+-rw-r--r--   0        0        0     1464 2024-05-31 13:50:52.379330 django_azure_auth-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     7062 1970-01-01 00:00:00.000000 django_azure_auth-1.4.3/PKG-INFO
```

### Comparing `django_azure_auth-1.4.2/LICENSE` & `django_azure_auth-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.2/README.md` & `django_azure_auth-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.2/azure_auth/handlers.py` & `django_azure_auth-1.4.3/azure_auth/handlers.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.2/azure_auth/middleware.py` & `django_azure_auth-1.4.3/azure_auth/middleware.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.2/azure_auth/tests/conftest.py` & `django_azure_auth-1.4.3/azure_auth/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.2/azure_auth/tests/settings.py` & `django_azure_auth-1.4.3/azure_auth/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.2/azure_auth/tests/test_decorators.py` & `django_azure_auth-1.4.3/azure_auth/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.2/azure_auth/tests/test_middleware.py` & `django_azure_auth-1.4.3/azure_auth/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.2/azure_auth/tests/test_views.py` & `django_azure_auth-1.4.3/azure_auth/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import copy
 from http import HTTPStatus
 from typing import cast
 from unittest.mock import patch
+from urllib.parse import quote
 
 import msal
 import pytest
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import AbstractUser, Group
 from django.test import TestCase, TransactionTestCase, override_settings
 from django.urls import reverse
 from mixer.backend.django import Mixer
 
 from azure_auth.exceptions import TokenError
 from azure_auth.handlers import AuthHandler
+from azure_auth.utils import EntraStateSerializer
 
 UserModel = get_user_model()
 
 
 @pytest.mark.django_db
 @pytest.mark.usefixtures("auth_flow")
 @patch.object(msal, "ConfidentialClientApplication")
@@ -41,15 +43,15 @@
             # Don't care about the `token_cache` object so just pipe it in
             token_cache=mocked_msal_app.call_args.kwargs["token_cache"],
         )
 
         mocked_msal_app.return_value.initiate_auth_code_flow.assert_called_once_with(
             scopes=settings.AZURE_AUTH["SCOPES"],
             redirect_uri=settings.AZURE_AUTH["REDIRECT_URI"],
-            state=None,
+            state='{"next": null}',
         )
 
     def test_login_redirect(self, mocked_msal_app):
         mocked_msal_app.return_value.initiate_auth_code_flow.return_value = (
             self.auth_flow  # type: ignore
         )
         resp = self.client.get(f"{reverse('azure_auth:login')}?next=/dummy_next/")
@@ -65,15 +67,15 @@
             # Don't care about the `token_cache` object so just pipe it in
             token_cache=mocked_msal_app.call_args.kwargs["token_cache"],
         )
 
         mocked_msal_app.return_value.initiate_auth_code_flow.assert_called_once_with(
             scopes=settings.AZURE_AUTH["SCOPES"],
             redirect_uri=settings.AZURE_AUTH["REDIRECT_URI"],
-            state="/dummy_next/",
+            state='{"next": "/dummy_next/"}',
         )
 
 
 @pytest.mark.django_db
 @pytest.mark.usefixtures("token")
 @pytest.mark.usefixtures("auth_flow")
 @patch.object(AuthHandler, "cache")
@@ -275,15 +277,15 @@
         # Graph API response
         expected_response_json = self._get_graph_response(self.user)  # type: ignore
         mocked_requests.get.side_effect = [
             self._mocked_response(HTTPStatus.OK, expected_response_json)
         ]
 
         resp = self.client.get(
-            f"{reverse('azure_auth:callback')}?state=/middleware_protected/"
+            f"{reverse('azure_auth:callback')}?state={quote(EntraStateSerializer().serialize(next='/middleware_protected/'), safe='/')}"
         )
         assert resp.status_code == HTTPStatus.FOUND
         assert resp.url == reverse("middleware_protected")  # type: ignore
         assert "id_token_claims" in self.client.session
 
         self._msal_asserts(mocked_msal_app)
         self._graph_asserts(mocked_requests)
```

### Comparing `django_azure_auth-1.4.2/azure_auth/tests/urls.py` & `django_azure_auth-1.4.3/azure_auth/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.2/azure_auth/views.py` & `django_azure_auth-1.4.3/azure_auth/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-from urllib.parse import quote
+from urllib.parse import unquote
 
 from django.conf import settings
 from django.contrib.auth import authenticate, login, logout
 from django.http import HttpRequest, HttpResponseForbidden, HttpResponseRedirect
 
+from azure_auth.utils import EntraStateSerializer
+
 from .handlers import AuthHandler
 
+serializer = EntraStateSerializer()
+
 
 def azure_auth_login(request: HttpRequest):
     return HttpResponseRedirect(
-        AuthHandler(request).get_auth_uri(state=request.GET.get("next"))
+        AuthHandler(request).get_auth_uri(
+            state=serializer.serialize(next=request.GET.get("next"))
+        )
     )
 
 
 def azure_auth_logout(request: HttpRequest):
     # Auth handler has to be initialized before `logout()` to load the claims from the session
     auth_handler = AuthHandler(request)
 
@@ -24,11 +30,11 @@
 def azure_auth_callback(request: HttpRequest):
     token = AuthHandler(request).get_token_from_flow()
     user = authenticate(request, token=token)
     if user:
         login(request, user)
 
         # Get `state` query param returned by AAD
-        next = quote(request.GET.get("state", ""), safe="/")
+        next = serializer.deserialize(unquote(request.GET.get("state", ""))).get("next")
     else:
         return HttpResponseForbidden("Invalid email for this app.")
     return HttpResponseRedirect(next or settings.LOGIN_REDIRECT_URL)
```

### Comparing `django_azure_auth-1.4.2/pyproject.toml` & `django_azure_auth-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-azure-auth"
-version = "1.4.2"
+version = "1.4.3"
 description = "A simple Django app for user authentication with Azure Active Directory/Entra ID."
 authors = ["Weird Sheep Labs <info@weirdsheeplabs.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Weird-Sheep-Labs/django-azure-auth"
 keywords = ['django', 'azure', 'authentication', 'microsoft', 'entra']
 classifiers = [
```

### Comparing `django_azure_auth-1.4.2/PKG-INFO` & `django_azure_auth-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-azure-auth
-Version: 1.4.2
+Version: 1.4.3
 Summary: A simple Django app for user authentication with Azure Active Directory/Entra ID.
 Home-page: https://github.com/Weird-Sheep-Labs/django-azure-auth
 License: MIT
 Keywords: django,azure,authentication,microsoft,entra
 Author: Weird Sheep Labs
 Author-email: info@weirdsheeplabs.com
 Requires-Python: >=3.8,<4.0
```

