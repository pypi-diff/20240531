# Comparing `tmp/salt_infisical-2.0.0.tar.gz` & `tmp/salt_infisical-2.1.0.tar.gz`

## Comparing `salt_infisical-2.0.0.tar` & `salt_infisical-2.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/src/salt_infisical/__about__.py
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/src/salt_infisical/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/LICENSE
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/README.md
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 salt_infisical-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/src/salt_infisical/__about__.py
+-rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/src/salt_infisical/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/LICENSE
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/README.md
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/PKG-INFO
```

### Comparing `salt_infisical-2.0.0/src/salt_infisical/__init__.py` & `salt_infisical-2.1.0/src/salt_infisical/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,100 @@
 # SPDX-FileCopyrightText: 2023-present Jonathan Treffler <mail@jonathan-treffler.de>
 #
 # SPDX-License-Identifier: MIT
 
 
 def get_config():
+    import logging
     import json
 
     path = "/etc/salt/infisical_config.json"
     f = open(path, "r")
     config = {}
 
     try:
         config = json.load(f)
+    except:
+        logging.exception('Invalid config')
     finally:
         f.close()
         return config
 
 def get_client():
     from infisical_client import ClientSettings, InfisicalClient, AuthenticationOptions, UniversalAuthMethod
 
     config = get_config()
 
     return InfisicalClient(
         ClientSettings(
             auth = AuthenticationOptions(
-                universal_auth = UniversalAuthMethod(**config)
+                universal_auth = UniversalAuthMethod(client_id=config["client_id"], client_secret=config["client_secret"])
             )
         )
     )
 
-def secret_bundle_to_dict(secret_bundle):
-    result = {}
-    result[getattr(secret_bundle, "secret_name")] = getattr(secret_bundle, "secret_value")
-    return result
-
-def secret_bundles_to_dict(secret_bundles):
-    result = {}
-    for secret_bundle in secret_bundles:
-        result[getattr(secret_bundle, "secret_name")] = getattr(secret_bundle, "secret_value")
-    return result
-
 def fetch_infisical_secrets(
         environment: str = "dev",
         path: str = "/",
+        project_id: str = "",
+        recursive: bool = False,
     ):
+    from infisical_client import ListSecretsOptions
+
     client = get_client()
+    config = get_config()
     subdirectories = path.strip("/").split("/")
 
+    if(project_id == "") {
+        project_id = get_config()["project_id"]
+    }
+
     secrets = {}
     for item in subdirectories[::-1]:
         if not secrets:
-            secrets[item] = secret_bundles_to_dict(client.get_all_secrets(environment=environment, path=path))
+            secrets[item] = client.listSecrets(options=ListSecretsOptions(
+                environment=environment,
+                path=path,
+                project_id=project_id,
+                recursive=recursive
+            ))
         else:
             tmp = {}
             tmp[item] = secrets.copy()
             secrets = dict(tmp)
 
     salt = { 'infisical': {} }
     salt["infisical"][environment] = secrets
 
     return salt
 
 def fetch_infisical_secret(
         secret_name: str,
         environment: str = "dev",
         path: str = "/",
+        project_id: str = "",
     ):
+    from infisical_client import GetSecretOptions
+
     client = get_client()
     subdirectories = path.strip("/").split("/")
 
+    if(project_id == "") {
+        project_id = get_config()["project_id"]
+    }
+
     secrets = {}
     for item in subdirectories[::-1]:
         if not secrets:
-            secrets[item] = secret_bundle_to_dict(client.get_secret(secret_name=secret_name, environment=environment, path=path))
+            secrets[item] = client.getSecret(options=GetSecretOptions(
+                secret_name=secret_name,
+                environment=environment,
+                path=path,
+                project_id=project_id
+            ))
         else:
             tmp = {}
             tmp[item] = secrets.copy()
             secrets = dict(tmp)
 
     salt = { 'infisical': {} }
     salt["infisical"][environment] = secrets
```

### Comparing `salt_infisical-2.0.0/LICENSE` & `salt_infisical-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `salt_infisical-2.0.0/README.md` & `salt_infisical-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `salt_infisical-2.0.0/pyproject.toml` & `salt_infisical-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `salt_infisical-2.0.0/PKG-INFO` & `salt_infisical-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: salt-infisical
-Version: 2.0.0
+Version: 2.1.0
 Project-URL: Documentation, https://github.com/unknown/salt-infisical#readme
 Project-URL: Issues, https://github.com/unknown/salt-infisical/issues
 Project-URL: Source, https://github.com/unknown/salt-infisical
 Author-email: Jonathan Treffler <mail@jonathan-treffler.de>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

