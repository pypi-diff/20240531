# Comparing `tmp/django_azure_auth-1.4.1a0.tar.gz` & `tmp/django_azure_auth-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_azure_auth-1.4.1a0.tar", max compression
+gzip compressed data, was "django_azure_auth-1.4.2.tar", max compression
```

## Comparing `django_azure_auth-1.4.1a0.tar` & `django_azure_auth-1.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/LICENSE
--rw-r--r--   0        0        0     6081 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/README.md
--rw-r--r--   0        0        0        0 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/__init__.py
--rw-r--r--   0        0        0      151 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/apps.py
--rw-r--r--   0        0        0      415 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/backends.py
--rw-r--r--   0        0        0      435 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/decorators.py
--rw-r--r--   0        0        0      333 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/exceptions.py
--rw-r--r--   0        0        0     7576 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/handlers.py
--rw-r--r--   0        0        0     1233 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/middleware.py
--rw-r--r--   0        0        0        0 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/tests/__init__.py
--rw-r--r--   0        0        0     2091 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/tests/conftest.py
--rw-r--r--   0        0        0     3943 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/tests/settings.py
--rw-r--r--   0        0        0     1409 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/tests/test_decorators.py
--rw-r--r--   0        0        0     3699 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/tests/test_middleware.py
--rw-r--r--   0        0        0    13037 2024-05-29 13:17:57.990004 django_azure_auth-1.4.1a0/azure_auth/tests/test_views.py
--rw-r--r--   0        0        0     1017 2024-05-29 13:17:57.994004 django_azure_auth-1.4.1a0/azure_auth/tests/urls.py
--rw-r--r--   0        0        0      324 2024-05-29 13:17:57.994004 django_azure_auth-1.4.1a0/azure_auth/urls.py
--rw-r--r--   0        0        0     1045 2024-05-29 13:17:57.994004 django_azure_auth-1.4.1a0/azure_auth/views.py
--rw-r--r--   0        0        0     1466 2024-05-29 13:18:10.046038 django_azure_auth-1.4.1a0/pyproject.toml
--rw-r--r--   0        0        0     7064 1970-01-01 00:00:00.000000 django_azure_auth-1.4.1a0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/LICENSE
+-rw-r--r--   0        0        0     6081 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/__init__.py
+-rw-r--r--   0        0        0      151 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/apps.py
+-rw-r--r--   0        0        0      415 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/backends.py
+-rw-r--r--   0        0        0      501 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/decorators.py
+-rw-r--r--   0        0        0      333 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/exceptions.py
+-rw-r--r--   0        0        0     7693 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/handlers.py
+-rw-r--r--   0        0        0     1138 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/middleware.py
+-rw-r--r--   0        0        0        0 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/tests/__init__.py
+-rw-r--r--   0        0        0     2091 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/tests/conftest.py
+-rw-r--r--   0        0        0     3943 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/tests/settings.py
+-rw-r--r--   0        0        0     1473 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/tests/test_decorators.py
+-rw-r--r--   0        0        0     3631 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/tests/test_middleware.py
+-rw-r--r--   0        0        0    14080 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/tests/test_views.py
+-rw-r--r--   0        0        0     1017 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/tests/urls.py
+-rw-r--r--   0        0        0      324 2024-05-30 16:59:38.078190 django_azure_auth-1.4.2/azure_auth/urls.py
+-rw-r--r--   0        0        0     1116 2024-05-30 16:59:38.082190 django_azure_auth-1.4.2/azure_auth/views.py
+-rw-r--r--   0        0        0     1464 2024-05-30 16:59:38.082190 django_azure_auth-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     7062 1970-01-01 00:00:00.000000 django_azure_auth-1.4.2/PKG-INFO
```

### Comparing `django_azure_auth-1.4.1a0/LICENSE` & `django_azure_auth-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1a0/README.md` & `django_azure_auth-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1a0/azure_auth/handlers.py` & `django_azure_auth-1.4.2/azure_auth/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
 from http import HTTPStatus
-from typing import cast
+from typing import Optional, cast
 from urllib import parse
 
 import msal
 import requests
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import AbstractBaseUser, Group
@@ -30,24 +30,26 @@
         self.auth_flow_session_key = "auth_flow"
         self._cache = msal.SerializableTokenCache()
         self._msal_app = None
 
         # Eagerly load the claims from the session
         self.claims = self.request.session.get("id_token_claims", {})
 
-    def get_auth_uri(self) -> str:
+    def get_auth_uri(self, state: Optional[str] = None) -> str:
         """
         Requests the auth flow dictionary and stores it on the session to be
         queried later in the auth process.
 
+        :param state: State to persist during log in
         :return: Authentication redirect URI
         """
         flow = self.msal_app.initiate_auth_code_flow(
             scopes=settings.AZURE_AUTH["SCOPES"],
             redirect_uri=settings.AZURE_AUTH["REDIRECT_URI"],
+            state=state,
         )
         self.request.session[self.auth_flow_session_key] = flow
         return flow["auth_uri"]
 
     def get_token_from_flow(self):
         """
         Acquires the token from the auth flow on the session and the content of
```

### Comparing `django_azure_auth-1.4.1a0/azure_auth/middleware.py` & `django_azure_auth-1.4.2/azure_auth/middleware.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,10 +25,8 @@
         for path in public_paths:
             if request.path_info.startswith(path):
                 return self.get_response(request)
 
         if AuthHandler(request).user_is_authenticated:
             return self.get_response(request)
 
-        # Save the intended path on the session to be redirected there upon login
-        request.session["next"] = request.path
-        return redirect("azure_auth:login")
+        return redirect(f"{reverse('azure_auth:login')}?next={request.path}")
```

### Comparing `django_azure_auth-1.4.1a0/azure_auth/tests/conftest.py` & `django_azure_auth-1.4.2/azure_auth/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1a0/azure_auth/tests/settings.py` & `django_azure_auth-1.4.2/azure_auth/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1a0/azure_auth/tests/test_middleware.py` & `django_azure_auth-1.4.2/azure_auth/tests/test_middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,25 +12,23 @@
 @pytest.mark.usefixtures("token")
 @patch.object(msal, "ConfidentialClientApplication")
 class TestAzureAuthMiddleware(TransactionTestCase):
     def test_invalid_token(self, mocked_msal_app):
         mocked_msal_app.return_value.acquire_token_silent.return_value = None
         resp = self.client.get(reverse("middleware_protected"))
         assert resp.status_code == HTTPStatus.FOUND
-        assert resp.url == "/azure_auth/login"  # type: ignore
-        assert self.client.session.get("next") == "/middleware_protected/"
+        assert resp.url == f"{reverse('azure_auth:login')}?next=/middleware_protected/"  # type: ignore
 
     def test_valid_token_unauthenticated_user(self, mocked_msal_app):
         # Not sure how this situation could arise but test anyway...
 
         mocked_msal_app.return_value.acquire_token_silent.return_value = self.token  # type: ignore
         resp = self.client.get(reverse("middleware_protected"))
         assert resp.status_code == HTTPStatus.FOUND
-        assert resp.url == "/azure_auth/login"  # type: ignore
-        assert self.client.session.get("next") == "/middleware_protected/"
+        assert resp.url == f"{reverse('azure_auth:login')}?next=/middleware_protected/"  # type: ignore
 
     def test_valid_token_authenticated_user(self, mocked_msal_app):
         mocked_msal_app.return_value.acquire_token_silent.return_value = self.token  # type: ignore
         self.client.force_login(self.user)  # type: ignore
 
         resp = self.client.get(reverse("middleware_protected"))
         assert resp.status_code == HTTPStatus.OK
```

### Comparing `django_azure_auth-1.4.1a0/azure_auth/tests/test_views.py` & `django_azure_auth-1.4.2/azure_auth/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,39 @@
             # Don't care about the `token_cache` object so just pipe it in
             token_cache=mocked_msal_app.call_args.kwargs["token_cache"],
         )
 
         mocked_msal_app.return_value.initiate_auth_code_flow.assert_called_once_with(
             scopes=settings.AZURE_AUTH["SCOPES"],
             redirect_uri=settings.AZURE_AUTH["REDIRECT_URI"],
+            state=None,
+        )
+
+    def test_login_redirect(self, mocked_msal_app):
+        mocked_msal_app.return_value.initiate_auth_code_flow.return_value = (
+            self.auth_flow  # type: ignore
+        )
+        resp = self.client.get(f"{reverse('azure_auth:login')}?next=/dummy_next/")
+        assert resp.status_code == HTTPStatus.FOUND
+        assert resp.url == self.auth_flow["auth_uri"]  # type: ignore
+        assert self.client.session._session == {"auth_flow": self.auth_flow}  # type: ignore
+
+        # MSAL calls
+        mocked_msal_app.assert_called_once_with(
+            client_id=settings.AZURE_AUTH["CLIENT_ID"],
+            client_credential=settings.AZURE_AUTH["CLIENT_SECRET"],
+            authority=settings.AZURE_AUTH["AUTHORITY"],
+            # Don't care about the `token_cache` object so just pipe it in
+            token_cache=mocked_msal_app.call_args.kwargs["token_cache"],
+        )
+
+        mocked_msal_app.return_value.initiate_auth_code_flow.assert_called_once_with(
+            scopes=settings.AZURE_AUTH["SCOPES"],
+            redirect_uri=settings.AZURE_AUTH["REDIRECT_URI"],
+            state="/dummy_next/",
         )
 
 
 @pytest.mark.django_db
 @pytest.mark.usefixtures("token")
 @pytest.mark.usefixtures("auth_flow")
 @patch.object(AuthHandler, "cache")
@@ -249,20 +274,17 @@
 
         # Graph API response
         expected_response_json = self._get_graph_response(self.user)  # type: ignore
         mocked_requests.get.side_effect = [
             self._mocked_response(HTTPStatus.OK, expected_response_json)
         ]
 
-        # `next` should be on the session
-        session = self.client.session
-        session["next"] = "/middleware_protected/"  # type: ignore
-        session.save()
-
-        resp = self.client.get(reverse("azure_auth:callback"))
+        resp = self.client.get(
+            f"{reverse('azure_auth:callback')}?state=/middleware_protected/"
+        )
         assert resp.status_code == HTTPStatus.FOUND
         assert resp.url == reverse("middleware_protected")  # type: ignore
         assert "id_token_claims" in self.client.session
 
         self._msal_asserts(mocked_msal_app)
         self._graph_asserts(mocked_requests)
```

### Comparing `django_azure_auth-1.4.1a0/azure_auth/tests/urls.py` & `django_azure_auth-1.4.2/azure_auth/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.4.1a0/azure_auth/views.py` & `django_azure_auth-1.4.2/azure_auth/views.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,34 @@
+from urllib.parse import quote
+
 from django.conf import settings
 from django.contrib.auth import authenticate, login, logout
 from django.http import HttpRequest, HttpResponseForbidden, HttpResponseRedirect
 
 from .handlers import AuthHandler
 
 
 def azure_auth_login(request: HttpRequest):
-    return HttpResponseRedirect(AuthHandler(request).get_auth_uri())
+    return HttpResponseRedirect(
+        AuthHandler(request).get_auth_uri(state=request.GET.get("next"))
+    )
 
 
 def azure_auth_logout(request: HttpRequest):
     # Auth handler has to be initialized before `logout()` to load the claims from the session
     auth_handler = AuthHandler(request)
 
     logout(request)
     return HttpResponseRedirect(auth_handler.get_logout_uri())
 
 
 def azure_auth_callback(request: HttpRequest):
     token = AuthHandler(request).get_token_from_flow()
     user = authenticate(request, token=token)
     if user:
-        # Get the `next` URL from the anonymous session before login
-        next = request.session.get("next", "")
         login(request, user)
+
+        # Get `state` query param returned by AAD
+        next = quote(request.GET.get("state", ""), safe="/")
     else:
         return HttpResponseForbidden("Invalid email for this app.")
     return HttpResponseRedirect(next or settings.LOGIN_REDIRECT_URL)
```

### Comparing `django_azure_auth-1.4.1a0/pyproject.toml` & `django_azure_auth-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-azure-auth"
-version = "1.4.1a0"
+version = "1.4.2"
 description = "A simple Django app for user authentication with Azure Active Directory/Entra ID."
 authors = ["Weird Sheep Labs <info@weirdsheeplabs.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Weird-Sheep-Labs/django-azure-auth"
 keywords = ['django', 'azure', 'authentication', 'microsoft', 'entra']
 classifiers = [
```

### Comparing `django_azure_auth-1.4.1a0/PKG-INFO` & `django_azure_auth-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-azure-auth
-Version: 1.4.1a0
+Version: 1.4.2
 Summary: A simple Django app for user authentication with Azure Active Directory/Entra ID.
 Home-page: https://github.com/Weird-Sheep-Labs/django-azure-auth
 License: MIT
 Keywords: django,azure,authentication,microsoft,entra
 Author: Weird Sheep Labs
 Author-email: info@weirdsheeplabs.com
 Requires-Python: >=3.8,<4.0
```

