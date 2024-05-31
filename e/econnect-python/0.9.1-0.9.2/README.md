# Comparing `tmp/econnect_python-0.9.1.tar.gz` & `tmp/econnect_python-0.9.2.tar.gz`

## Comparing `econnect_python-0.9.1.tar` & `econnect_python-0.9.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 econnect_python-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 econnect_python-0.9.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 econnect_python-0.9.1/tox.ini
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 econnect_python-0.9.1/.github/pull_request_template.md
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 econnect_python-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 econnect_python-0.9.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 econnect_python-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 econnect_python-0.9.1/.github/workflows/building.yaml
--rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 econnect_python-0.9.1/.github/workflows/linting.yaml
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 econnect_python-0.9.1/.github/workflows/testing.yaml
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 econnect_python-0.9.1/src/elmo/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 econnect_python-0.9.1/src/elmo/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 econnect_python-0.9.1/src/elmo/query.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 econnect_python-0.9.1/src/elmo/systems.py
--rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 econnect_python-0.9.1/src/elmo/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 econnect_python-0.9.1/src/elmo/api/__init__.py
--rw-r--r--   0        0        0    28974 2020-02-02 00:00:00.000000 econnect_python-0.9.1/src/elmo/api/client.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 econnect_python-0.9.1/src/elmo/api/decorators.py
--rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 econnect_python-0.9.1/src/elmo/api/exceptions.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 econnect_python-0.9.1/src/elmo/api/router.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 econnect_python-0.9.1/tests/conftest.py
--rw-r--r--   0        0        0    74420 2020-02-02 00:00:00.000000 econnect_python-0.9.1/tests/test_client.py
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 econnect_python-0.9.1/tests/test_decorators.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 econnect_python-0.9.1/tests/test_router.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 econnect_python-0.9.1/tests/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 econnect_python-0.9.1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     7580 2020-02-02 00:00:00.000000 econnect_python-0.9.1/tests/fixtures/responses.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 econnect_python-0.9.1/.gitignore
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 econnect_python-0.9.1/LICENSE
--rw-r--r--   0        0        0     6834 2020-02-02 00:00:00.000000 econnect_python-0.9.1/README.md
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 econnect_python-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     8350 2020-02-02 00:00:00.000000 econnect_python-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 econnect_python-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 econnect_python-0.9.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 econnect_python-0.9.2/tox.ini
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 econnect_python-0.9.2/.github/pull_request_template.md
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 econnect_python-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 econnect_python-0.9.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 econnect_python-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 econnect_python-0.9.2/.github/workflows/building.yaml
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 econnect_python-0.9.2/.github/workflows/linting.yaml
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 econnect_python-0.9.2/.github/workflows/testing.yaml
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 econnect_python-0.9.2/src/elmo/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 econnect_python-0.9.2/src/elmo/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 econnect_python-0.9.2/src/elmo/query.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 econnect_python-0.9.2/src/elmo/systems.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 econnect_python-0.9.2/src/elmo/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 econnect_python-0.9.2/src/elmo/api/__init__.py
+-rw-r--r--   0        0        0    29072 2020-02-02 00:00:00.000000 econnect_python-0.9.2/src/elmo/api/client.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 econnect_python-0.9.2/src/elmo/api/decorators.py
+-rw-r--r--   0        0        0     2273 2020-02-02 00:00:00.000000 econnect_python-0.9.2/src/elmo/api/exceptions.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 econnect_python-0.9.2/src/elmo/api/router.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 econnect_python-0.9.2/tests/conftest.py
+-rw-r--r--   0        0        0    74922 2020-02-02 00:00:00.000000 econnect_python-0.9.2/tests/test_client.py
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 econnect_python-0.9.2/tests/test_decorators.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 econnect_python-0.9.2/tests/test_router.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 econnect_python-0.9.2/tests/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 econnect_python-0.9.2/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     7580 2020-02-02 00:00:00.000000 econnect_python-0.9.2/tests/fixtures/responses.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 econnect_python-0.9.2/.gitignore
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 econnect_python-0.9.2/LICENSE
+-rw-r--r--   0        0        0     6834 2020-02-02 00:00:00.000000 econnect_python-0.9.2/README.md
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 econnect_python-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     8350 2020-02-02 00:00:00.000000 econnect_python-0.9.2/PKG-INFO
```

### Comparing `econnect_python-0.9.1/.pre-commit-config.yaml` & `econnect_python-0.9.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/CONTRIBUTING.md` & `econnect_python-0.9.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/.github/pull_request_template.md` & `econnect_python-0.9.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/.github/ISSUE_TEMPLATE/bug_report.md` & `econnect_python-0.9.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/.github/ISSUE_TEMPLATE/feature_request.md` & `econnect_python-0.9.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/.github/workflows/building.yaml` & `econnect_python-0.9.2/.github/workflows/building.yaml`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/.github/workflows/linting.yaml` & `econnect_python-0.9.2/.github/workflows/linting.yaml`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/.github/workflows/testing.yaml` & `econnect_python-0.9.2/.github/workflows/testing.yaml`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/src/elmo/utils.py` & `econnect_python-0.9.2/src/elmo/utils.py`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/src/elmo/api/client.py` & `econnect_python-0.9.2/src/elmo/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from ..utils import _camel_to_snake_case, _sanitize_session_id
 from .decorators import require_lock, require_session
 from .exceptions import (
     CodeError,
     CredentialError,
     InvalidInput,
     InvalidSector,
+    InvalidToken,
     LockError,
     ParseError,
     QueryNotValid,
 )
 from .router import Router
 
 _LOGGER = logging.getLogger(__name__)
@@ -168,18 +169,20 @@
         """
         payload = {"userId": 1, "password": code, "sessionId": self._session_id}
         response = self._session.post(self._router.lock, data=payload)
 
         try:
             response.raise_for_status()
         except HTTPError as err:
-            # 403: Not possible to obtain the lock, probably because of a race condition
-            # with another application
+            # 403: Unable obtain the lock (race condition with another application)
             if err.response.status_code == 403:
                 raise LockError
+            # 401: The token has expired
+            if err.response.status_code == 401:
+                raise InvalidToken
             raise err
 
         # A wrong code returns 200 with a fail state
         body = response.json()
         if not body[0]["Successful"]:
             raise CodeError
```

### Comparing `econnect_python-0.9.1/src/elmo/api/decorators.py` & `econnect_python-0.9.2/src/elmo/api/decorators.py`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/src/elmo/api/exceptions.py` & `econnect_python-0.9.2/src/elmo/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/src/elmo/api/router.py` & `econnect_python-0.9.2/src/elmo/api/router.py`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/tests/conftest.py` & `econnect_python-0.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/tests/test_client.py` & `econnect_python-0.9.2/tests/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -597,14 +597,27 @@
     # Test
     with pytest.raises(LockError):
         with client.lock("test"):
             pass
     assert len(server.calls) == 1
 
 
+def test_client_lock_invalid_token(server, mocker):
+    """Should raise a CodeError if the token is expired while calling Lock()."""
+    server.add(responses.POST, "https://example.com/api/panel/syncLogin", status=401)
+    client = ElmoClient(base_url="https://example.com", domain="domain")
+    client._session_id = "test"
+    mocker.patch.object(client, "unlock")
+    # Test
+    with pytest.raises(InvalidToken):
+        with client.lock("test"):
+            pass
+    assert len(server.calls) == 1
+
+
 def test_client_lock_unknown_error(server, mocker):
     """Should raise an Exception for unknown status code."""
     server.add(
         responses.POST,
         "https://example.com/api/panel/syncLogin",
         body="Server Error",
         status=500,
```

### Comparing `econnect_python-0.9.1/tests/test_decorators.py` & `econnect_python-0.9.2/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/tests/test_utils.py` & `econnect_python-0.9.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/tests/fixtures/responses.py` & `econnect_python-0.9.2/tests/fixtures/responses.py`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/.gitignore` & `econnect_python-0.9.2/.gitignore`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/LICENSE` & `econnect_python-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/README.md` & `econnect_python-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/pyproject.toml` & `econnect_python-0.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `econnect_python-0.9.1/PKG-INFO` & `econnect_python-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: econnect-python
-Version: 0.9.1
+Version: 0.9.2
 Summary: API adapter used to control programmatically an Elmo alarm system
 Project-URL: Documentation, https://github.com/palazzem/econnect-python#readme
 Project-URL: Issues, https://github.com/palazzem/econnect-python/issues
 Project-URL: Source, https://github.com/palazzem/econnect-python
 Author-email: Emanuele Palazzetti <emanuele.palazzetti@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

