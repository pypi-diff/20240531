# Comparing `tmp/armasec-2.0.0.tar.gz` & `tmp/armasec-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "armasec-2.0.0.tar", max compression
+gzip compressed data, was "armasec-2.0.1.tar", max compression
```

## Comparing `armasec-2.0.0.tar` & `armasec-2.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1078 2024-05-29 20:36:44.159150 armasec-2.0.0/LICENSE.md
--rw-r--r--   0        0        0     2646 2024-05-29 20:36:44.159150 armasec-2.0.0/README.md
--rw-r--r--   0        0        0      423 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/__init__.py
--rw-r--r--   0        0        0     4776 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/armasec.py
--rw-r--r--   0        0        0     1369 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/exceptions.py
--rw-r--r--   0        0        0     3828 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/openid_config_loader.py
--rw-r--r--   0        0        0      280 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/pluggable/__init__.py
--rw-r--r--   0        0        0     1237 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/pluggable/hookspecs.py
--rw-r--r--   0        0        0        0 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/py.typed
--rw-r--r--   0        0        0     9588 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/pytest_extension.py
--rw-r--r--   0        0        0      232 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/schemas/__init__.py
--rw-r--r--   0        0        0     2083 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/schemas/armasec_config.py
--rw-r--r--   0        0        0     1340 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/schemas/jwks.py
--rw-r--r--   0        0        0      651 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/schemas/openid_config.py
--rw-r--r--   0        0        0     6255 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/token_decoder.py
--rw-r--r--   0        0        0     3616 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/token_manager.py
--rw-r--r--   0        0        0     1266 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/token_payload.py
--rw-r--r--   0        0        0    10898 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/token_security.py
--rw-r--r--   0        0        0     1105 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/utilities.py
--rw-r--r--   0        0        0     9089 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/auth.py
--rw-r--r--   0        0        0     3050 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/cache.py
--rw-r--r--   0        0        0     8281 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/client.py
--rw-r--r--   0        0        0     2283 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/config.py
--rw-r--r--   0        0        0     1521 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/exceptions.py
--rw-r--r--   0        0        0      756 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/format.py
--rw-r--r--   0        0        0      194 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/logging.py
--rw-r--r--   0        0        0     6119 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/main.py
--rw-r--r--   0        0        0      663 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/schemas.py
--rw-r--r--   0        0        0     3057 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/time_loop.py
--rw-r--r--   0        0        0     2603 2024-05-29 20:36:44.179150 armasec-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     4457 1970-01-01 00:00:00.000000 armasec-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-30 22:32:32.398245 armasec-2.0.1/LICENSE.md
+-rw-r--r--   0        0        0     2646 2024-05-30 22:32:32.398245 armasec-2.0.1/README.md
+-rw-r--r--   0        0        0      423 2024-05-30 22:32:32.398245 armasec-2.0.1/armasec/__init__.py
+-rw-r--r--   0        0        0     4776 2024-05-30 22:32:32.398245 armasec-2.0.1/armasec/armasec.py
+-rw-r--r--   0        0        0     1369 2024-05-30 22:32:32.398245 armasec-2.0.1/armasec/exceptions.py
+-rw-r--r--   0        0        0     3828 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec/openid_config_loader.py
+-rw-r--r--   0        0        0      280 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec/pluggable/__init__.py
+-rw-r--r--   0        0        0     1237 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec/pluggable/hookspecs.py
+-rw-r--r--   0        0        0        0 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec/py.typed
+-rw-r--r--   0        0        0     9588 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec/pytest_extension.py
+-rw-r--r--   0        0        0      232 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec/schemas/__init__.py
+-rw-r--r--   0        0        0     2083 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec/schemas/armasec_config.py
+-rw-r--r--   0        0        0     1340 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec/schemas/jwks.py
+-rw-r--r--   0        0        0      651 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec/schemas/openid_config.py
+-rw-r--r--   0        0        0     6255 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec/token_decoder.py
+-rw-r--r--   0        0        0     3616 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec/token_manager.py
+-rw-r--r--   0        0        0     1286 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec/token_payload.py
+-rw-r--r--   0        0        0    10898 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec/token_security.py
+-rw-r--r--   0        0        0     1105 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec/utilities.py
+-rw-r--r--   0        0        0     9089 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec_cli/auth.py
+-rw-r--r--   0        0        0     3050 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec_cli/cache.py
+-rw-r--r--   0        0        0     8281 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec_cli/client.py
+-rw-r--r--   0        0        0     2283 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec_cli/config.py
+-rw-r--r--   0        0        0     1521 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec_cli/exceptions.py
+-rw-r--r--   0        0        0      756 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec_cli/format.py
+-rw-r--r--   0        0        0      194 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec_cli/logging.py
+-rw-r--r--   0        0        0     6119 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec_cli/main.py
+-rw-r--r--   0        0        0      663 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec_cli/schemas.py
+-rw-r--r--   0        0        0     3057 2024-05-30 22:32:32.402245 armasec-2.0.1/armasec_cli/time_loop.py
+-rw-r--r--   0        0        0     2603 2024-05-30 22:32:32.422245 armasec-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4457 1970-01-01 00:00:00.000000 armasec-2.0.1/PKG-INFO
```

### Comparing `armasec-2.0.0/LICENSE.md` & `armasec-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/README.md` & `armasec-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec/armasec.py` & `armasec-2.0.1/armasec/armasec.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec/exceptions.py` & `armasec-2.0.1/armasec/exceptions.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec/openid_config_loader.py` & `armasec-2.0.1/armasec/openid_config_loader.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec/pluggable/hookspecs.py` & `armasec-2.0.1/armasec/pluggable/hookspecs.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec/pytest_extension.py` & `armasec-2.0.1/armasec/pytest_extension.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec/schemas/armasec_config.py` & `armasec-2.0.1/armasec/schemas/armasec_config.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec/schemas/jwks.py` & `armasec-2.0.1/armasec/schemas/jwks.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec/schemas/openid_config.py` & `armasec-2.0.1/armasec/schemas/openid_config.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec/token_decoder.py` & `armasec-2.0.1/armasec/token_decoder.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec/token_manager.py` & `armasec-2.0.1/armasec/token_manager.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec/token_payload.py` & `armasec-2.0.1/armasec/token_payload.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         expire:         The "exp" claim extracted from a JWT.
         client_id:      The "azp" claim extracted from a JWT.
         original_token: The original token value
     """
 
     sub: str
     permissions: List[str] = Field(list())
-    expire: datetime = Field(None, validation_alias=AliasChoices("exp", "expire"))
-    client_id: str = Field(None, validation_alias=AliasChoices("azp", "client_id"))
+    expire: Optional[datetime] = Field(None, validation_alias=AliasChoices("exp", "expire"))
+    client_id: Optional[str] = Field(None, validation_alias=AliasChoices("azp", "client_id"))
     original_token: Optional[str] = None
     model_config = ConfigDict(extra="allow")
 
     def to_dict(self):
         """
         Convert a TokenPayload to the equivalent dictionary returned by `jwt.decode()`.
         """
```

### Comparing `armasec-2.0.0/armasec/token_security.py` & `armasec-2.0.1/armasec/token_security.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec/utilities.py` & `armasec-2.0.1/armasec/utilities.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec_cli/auth.py` & `armasec-2.0.1/armasec_cli/auth.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec_cli/cache.py` & `armasec-2.0.1/armasec_cli/cache.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec_cli/client.py` & `armasec-2.0.1/armasec_cli/client.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec_cli/config.py` & `armasec-2.0.1/armasec_cli/config.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec_cli/exceptions.py` & `armasec-2.0.1/armasec_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec_cli/format.py` & `armasec-2.0.1/armasec_cli/format.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec_cli/main.py` & `armasec-2.0.1/armasec_cli/main.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec_cli/schemas.py` & `armasec-2.0.1/armasec_cli/schemas.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/armasec_cli/time_loop.py` & `armasec-2.0.1/armasec_cli/time_loop.py`

 * *Files identical despite different names*

### Comparing `armasec-2.0.0/pyproject.toml` & `armasec-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "armasec"
-version = "2.0.0"
+version = "2.0.1"
 description = "Injectable FastAPI auth via OIDC"
 authors = ["Omnivector Engineering Team <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/omnivector-solutions/armasec"
 repository = "https://github.com/omnivector-solutions/armasec"
 documentation = "https://omnivector-solutions.github.io/armasec"
```

### Comparing `armasec-2.0.0/PKG-INFO` & `armasec-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armasec
-Version: 2.0.0
+Version: 2.0.1
 Summary: Injectable FastAPI auth via OIDC
 Home-page: https://github.com/omnivector-solutions/armasec
 License: MIT
 Author: Omnivector Engineering Team
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

