# Comparing `tmp/salt_infisical-2.1.0.tar.gz` & `tmp/salt_infisical-2.1.1.tar.gz`

## Comparing `salt_infisical-2.1.0.tar` & `salt_infisical-2.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/src/salt_infisical/__about__.py
--rw-r--r--   0        0        0     2589 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/src/salt_infisical/__init__.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/tests/__init__.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/LICENSE
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/README.md
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 salt_infisical-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/src/salt_infisical/__about__.py
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/src/salt_infisical/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/tests/__init__.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/LICENSE
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/README.md
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 salt_infisical-2.1.1/PKG-INFO
```

### Comparing `salt_infisical-2.1.0/src/salt_infisical/__init__.py` & `salt_infisical-2.1.1/src/salt_infisical/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,28 +37,23 @@
         path: str = "/",
         project_id: str = "",
         recursive: bool = False,
     ):
     from infisical_client import ListSecretsOptions
 
     client = get_client()
-    config = get_config()
     subdirectories = path.strip("/").split("/")
 
-    if(project_id == "") {
-        project_id = get_config()["project_id"]
-    }
-
     secrets = {}
     for item in subdirectories[::-1]:
         if not secrets:
             secrets[item] = client.listSecrets(options=ListSecretsOptions(
                 environment=environment,
                 path=path,
-                project_id=project_id,
+                project_id=project_id or get_config()["project_id"],
                 recursive=recursive
             ))
         else:
             tmp = {}
             tmp[item] = secrets.copy()
             secrets = dict(tmp)
 
@@ -74,26 +69,22 @@
         project_id: str = "",
     ):
     from infisical_client import GetSecretOptions
 
     client = get_client()
     subdirectories = path.strip("/").split("/")
 
-    if(project_id == "") {
-        project_id = get_config()["project_id"]
-    }
-
     secrets = {}
     for item in subdirectories[::-1]:
         if not secrets:
             secrets[item] = client.getSecret(options=GetSecretOptions(
                 secret_name=secret_name,
                 environment=environment,
                 path=path,
-                project_id=project_id
+                project_id=project_id or get_config()["project_id"]
             ))
         else:
             tmp = {}
             tmp[item] = secrets.copy()
             secrets = dict(tmp)
 
     salt = { 'infisical': {} }
```

### Comparing `salt_infisical-2.1.0/LICENSE` & `salt_infisical-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `salt_infisical-2.1.0/README.md` & `salt_infisical-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `salt_infisical-2.1.0/pyproject.toml` & `salt_infisical-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `salt_infisical-2.1.0/PKG-INFO` & `salt_infisical-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: salt-infisical
-Version: 2.1.0
+Version: 2.1.1
 Project-URL: Documentation, https://github.com/unknown/salt-infisical#readme
 Project-URL: Issues, https://github.com/unknown/salt-infisical/issues
 Project-URL: Source, https://github.com/unknown/salt-infisical
 Author-email: Jonathan Treffler <mail@jonathan-treffler.de>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

