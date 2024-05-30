# Comparing `tmp/salt_infisical-2.1.1.tar.gz` & `tmp/salt_infisical-2.1.2.tar.gz`

## Comparing `salt_infisical-2.1.1.tar` & `salt_infisical-2.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/src/salt_infisical/__about__.py
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/src/salt_infisical/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/tests/__init__.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/LICENSE
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/README.md
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 salt_infisical-2.1.2/src/salt_infisical/__about__.py
+-rw-r--r--   0        0        0     2534 2020-02-02 00:00:00.000000 salt_infisical-2.1.2/src/salt_infisical/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 salt_infisical-2.1.2/tests/__init__.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 salt_infisical-2.1.2/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 salt_infisical-2.1.2/LICENSE
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 salt_infisical-2.1.2/README.md
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 salt_infisical-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 salt_infisical-2.1.2/PKG-INFO
```

### Comparing `salt_infisical-2.1.1/src/salt_infisical/__init__.py` & `salt_infisical-2.1.2/src/salt_infisical/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,20 @@
 
     client = get_client()
     subdirectories = path.strip("/").split("/")
 
     secrets = {}
     for item in subdirectories[::-1]:
         if not secrets:
-            secrets[item] = client.listSecrets(options=ListSecretsOptions(
+            secrets[item] = {secret.secret_key:secret.secret_value for secret in client.listSecrets(options=ListSecretsOptions(
                 environment=environment,
                 path=path,
                 project_id=project_id or get_config()["project_id"],
                 recursive=recursive
-            ))
+            )).secrets}
         else:
             tmp = {}
             tmp[item] = secrets.copy()
             secrets = dict(tmp)
 
     salt = { 'infisical': {} }
     salt["infisical"][environment] = secrets
@@ -77,15 +77,15 @@
     for item in subdirectories[::-1]:
         if not secrets:
             secrets[item] = client.getSecret(options=GetSecretOptions(
                 secret_name=secret_name,
                 environment=environment,
                 path=path,
                 project_id=project_id or get_config()["project_id"]
-            ))
+            )).secret_value
         else:
             tmp = {}
             tmp[item] = secrets.copy()
             secrets = dict(tmp)
 
     salt = { 'infisical': {} }
     salt["infisical"][environment] = secrets
```

### Comparing `salt_infisical-2.1.1/LICENSE` & `salt_infisical-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `salt_infisical-2.1.1/README.md` & `salt_infisical-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `salt_infisical-2.1.1/pyproject.toml` & `salt_infisical-2.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `salt_infisical-2.1.1/PKG-INFO` & `salt_infisical-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: salt-infisical
-Version: 2.1.1
+Version: 2.1.2
 Project-URL: Documentation, https://github.com/unknown/salt-infisical#readme
 Project-URL: Issues, https://github.com/unknown/salt-infisical/issues
 Project-URL: Source, https://github.com/unknown/salt-infisical
 Author-email: Jonathan Treffler <mail@jonathan-treffler.de>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

