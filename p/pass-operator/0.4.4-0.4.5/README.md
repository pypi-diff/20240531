# Comparing `tmp/pass_operator-0.4.4.tar.gz` & `tmp/pass_operator-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pass_operator-0.4.4.tar", max compression
+gzip compressed data, was "pass_operator-0.4.5.tar", max compression
```

## Comparing `pass_operator-0.4.4.tar` & `pass_operator-0.4.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35140 2024-05-30 19:29:50.572975 pass_operator-0.4.4/LICENSE
--rw-r--r--   0        0        0     3727 2024-05-30 19:29:50.572975 pass_operator-0.4.4/README.md
--rw-r--r--   0        0        0     1612 2024-05-30 19:30:05.693122 pass_operator-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     1670 2024-05-30 19:29:50.580975 pass_operator-0.4.4/src/passoperator/__init__.py
--rw-r--r--   0        0        0    17134 2024-05-30 19:29:50.580975 pass_operator-0.4.4/src/passoperator/daemon.py
--rw-r--r--   0        0        0     2017 2024-05-30 19:29:50.580975 pass_operator-0.4.4/src/passoperator/git.py
--rw-r--r--   0        0        0     1213 2024-05-30 19:29:50.580975 pass_operator-0.4.4/src/passoperator/gpg.py
--rw-r--r--   0        0        0     9217 2024-05-30 19:29:50.580975 pass_operator-0.4.4/src/passoperator/secret.py
--rw-r--r--   0        0        0     1313 2024-05-30 19:29:50.580975 pass_operator-0.4.4/src/passoperator/utils.py
--rw-r--r--   0        0        0     4721 1970-01-01 00:00:00.000000 pass_operator-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    35140 2024-05-30 20:15:41.585211 pass_operator-0.4.5/LICENSE
+-rw-r--r--   0        0        0     3727 2024-05-30 20:15:41.585211 pass_operator-0.4.5/README.md
+-rw-r--r--   0        0        0     1612 2024-05-30 20:15:59.485250 pass_operator-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1670 2024-05-30 20:15:41.589211 pass_operator-0.4.5/src/passoperator/__init__.py
+-rw-r--r--   0        0        0    18470 2024-05-30 20:15:41.589211 pass_operator-0.4.5/src/passoperator/daemon.py
+-rw-r--r--   0        0        0     2017 2024-05-30 20:15:41.589211 pass_operator-0.4.5/src/passoperator/git.py
+-rw-r--r--   0        0        0     1213 2024-05-30 20:15:41.589211 pass_operator-0.4.5/src/passoperator/gpg.py
+-rw-r--r--   0        0        0     9217 2024-05-30 20:15:41.589211 pass_operator-0.4.5/src/passoperator/secret.py
+-rw-r--r--   0        0        0     1313 2024-05-30 20:15:41.589211 pass_operator-0.4.5/src/passoperator/utils.py
+-rw-r--r--   0        0        0     4721 1970-01-01 00:00:00.000000 pass_operator-0.4.5/PKG-INFO
```

### Comparing `pass_operator-0.4.4/LICENSE` & `pass_operator-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.4/README.md` & `pass_operator-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.4/pyproject.toml` & `pass_operator-0.4.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pass-operator"
-version = "v0.4.4"
+version = "v0.4.5"
 description = "A Kubernetes operator that syncs and decrypts secrets from pass store git repositories"
 authors = ["Emma Doyle <emma@premiscale.com>"]
 maintainers = ["Emma Doyle <emma@premiscale.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 packages = [
   { include = "passoperator", from = "src" }
```

### Comparing `pass_operator-0.4.4/src/passoperator/__init__.py` & `pass_operator-0.4.5/src/passoperator/__init__.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.4/src/passoperator/daemon.py` & `pass_operator-0.4.5/src/passoperator/daemon.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from pathlib import Path
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 from importlib import metadata
 from kubernetes import client, config
 from http import HTTPStatus
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
+from time import sleep
 
 from passoperator.git import pull, clone
 from passoperator.utils import LogLevel
 from passoperator.secret import PassSecret, ManagedSecret
 from passoperator import env
 
 import asyncio
@@ -34,14 +35,15 @@
     """
     Block handlers' progress on a PassSecret until it's safe to modify the managed secret.
     Decryption takes time, so we want to be sure to queue up any changes.
 
     Args:
         body [kopf.Body]: raw body of the PassSecret.
     """
+    log.debug(f'Blocking PassSecret "{body["metadata"]["name"]}" in namespace "{body["metadata"]["namespace"]}')
     __in_progress_queue.append(
         (
             body['metadata']['name'],
             body['metadata']['namespace']
         )
     )
 
@@ -58,21 +60,39 @@
     """
     return (
         body['metadata']['name'],
         body['metadata']['namespace']
     ) in __in_progress_queue
 
 
+def _block_passsecret_block(body: kopf.Body) -> None:
+    """
+    Block handlers' progress on a PassSecret until it's safe to modify the managed secret.
+    This should only ever be called by event handlers, not by the reconciliation loop.
+
+    Args:
+        body (kopf.Body): raw body of the PassSecret.
+    """
+    while True:
+        if not _is_passsecret_blocked(body):
+            _passsecret_block(body)
+            break
+        else:
+            log.debug(f'PassSecret "{body["metadata"]["name"]}" in namespace "{body["metadata"]["namespace"]}" is already blocked.')
+            sleep(0.5)
+
+
 def _lift_passsecret_block(body: kopf.Body) -> None:
     """
     Unblock handlers' progress to modify the managed secret.
 
     Args:
         body [kopf.Body]: raw body of the PassSecret.
     """
+    log.debug(f'Lifting block on PassSecret "{body["metadata"]["name"]}" in namespace "{body["metadata"]["namespace"]}"')
     __in_progress_queue.remove(
         (
             body['metadata']['name'],
             body['metadata']['namespace']
         )
     )
 
@@ -115,14 +135,15 @@
     check_gpg_id(
         path=f'{env["PASS_DIRECTORY"]}/.gpg-id'
     )
 
     v1 = client.CoreV1Api()
 
     # Create a new PassSecret object with an up-to-date managedSecret decrypted value from the pass store.
+    _passsecret_block(body)
     passSecretObj = PassSecret.from_kopf(body)
 
     log.info(
         f'Reconciling PassSecret "{passSecretObj.metadata.name}" managed Secret "{passSecretObj.spec.managedSecret.metadata.name}" in Namespace "{passSecretObj.spec.managedSecret.metadata.namespace}" against password store.'
     )
 
     try:
@@ -134,14 +155,15 @@
         log.debug(secret)
         _managedSecret = ManagedSecret.from_kopf(secret.to_dict())
 
         # If the managed secret data does not match what's in the newly-generated ManagedSecret object,
         # submit a patch request to update it.
         if not _managedSecret.data_equals(passSecretObj.spec.managedSecret):
             if _managedSecret.immutable:
+                _lift_passsecret_block(body)
                 raise kopf.TemporaryError(
                     f'PassSecret "{passSecretObj.metadata.name}" managed secret "{passSecretObj.spec.managedSecret.metadata.name}" is immutable. Ignoring data patch.'
                 )
 
             v1.patch_namespaced_secret(
                 name=passSecretObj.spec.managedSecret.metadata.name,
                 namespace=passSecretObj.spec.managedSecret.metadata.namespace,
@@ -160,15 +182,18 @@
             v1.create_namespaced_secret(
                 namespace=passSecretObj.spec.managedSecret.metadata.namespace,
                 body=client.V1Secret(
                     **passSecretObj.spec.managedSecret.to_client_dict(finalizers=False)
                 )
             )
         else:
+            _lift_passsecret_block(body)
             raise kopf.PermanentError(e)
+    finally:
+        _lift_passsecret_block(body)
 
 
 # @kopf.on.cleanup()
 # def cleanup(**kwargs) -> None:
 #     pass
 
 # @kopf.on.resume()
@@ -221,15 +246,17 @@
     metadata = {
         'metadata': {
             'name': meta['name'],
             'namespace': meta['namespace']
         }
     }
 
-    _passsecret_block(body)
+    # If a reconciliation is already in progress for the triggered PassSecret, block this event handler
+    # until it's safe to modify the managed secret.
+    _block_passsecret_block(body)
 
     # Parse the old PassSecret manifest.
     try:
         oldPassSecret = PassSecret.from_kopf(
             {
                 **metadata,
                 **old
@@ -291,18 +318,20 @@
 def create(body: kopf.Body, **_: Any) -> None:
     """
     Create a new Secret with the spec of the newly-created PassSecret.
 
     Args:
         body [kopf.Body]: raw body of the created PassSecret.
     """
-    try:
-        # Indicate to the reconciliation loop that this PassSecret is in progress.
-        _passsecret_block(body)
 
+    # If a reconciliation is already in progress for the triggered PassSecret, block this event handler
+    # until it's safe to modify the managed secret.
+    _block_passsecret_block(body)
+
+    try:
         passSecretObj = PassSecret.from_kopf(body)
     except (ValueError, KeyError) as e:
         _lift_passsecret_block(body)
         raise kopf.PermanentError(e)
 
     log.info(f'PassSecret "{passSecretObj.metadata.name}" created')
 
@@ -332,18 +361,20 @@
 def delete(body: kopf.Body, **_: Any) -> None:
     """
     Remove a managed secret, as the managing PassSecret has been deleted.
 
     Args:
         body [kopf.Body]: raw body of the deleted PassSecret.
     """
-    try:
-        # Indicate to the reconciliation loop that this PassSecret is in progress.
-        _passsecret_block(body)
 
+    # If a reconciliation is already in progress for the triggered PassSecret, block this event handler
+    # until it's safe to modify the managed secret.
+    _block_passsecret_block(body)
+
+    try:
         passSecretObj = PassSecret.from_kopf(body)
     except (ValueError, KeyError) as e:
         _lift_passsecret_block(body)
         raise kopf.PermanentError(e)
 
     log.info(f'PassSecret "{passSecretObj.metadata.name}" deleted')
```

### Comparing `pass_operator-0.4.4/src/passoperator/git.py` & `pass_operator-0.4.5/src/passoperator/git.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.4/src/passoperator/gpg.py` & `pass_operator-0.4.5/src/passoperator/gpg.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.4/src/passoperator/secret.py` & `pass_operator-0.4.5/src/passoperator/secret.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.4/src/passoperator/utils.py` & `pass_operator-0.4.5/src/passoperator/utils.py`

 * *Files identical despite different names*

### Comparing `pass_operator-0.4.4/PKG-INFO` & `pass_operator-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pass-operator
-Version: 0.4.4
+Version: 0.4.5
 Summary: A Kubernetes operator that syncs and decrypts secrets from pass store git repositories
 License: GPL-3.0-or-later
 Keywords: python,kubernetes,secrets,operator,pass
 Author: Emma Doyle
 Author-email: emma@premiscale.com
 Maintainer: Emma Doyle
 Maintainer-email: emma@premiscale.com
```

