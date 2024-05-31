# Comparing `tmp/keyring_proxy_stdio-0.1.3.tar.gz` & `tmp/keyring_proxy_stdio-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_proxy_stdio-0.1.3.tar", last modified: Thu May 30 13:03:19 2024, max compression
+gzip compressed data, was "keyring_proxy_stdio-0.1.4.tar", last modified: Thu May 30 13:28:16 2024, max compression
```

## Comparing `keyring_proxy_stdio-0.1.3.tar` & `keyring_proxy_stdio-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       22 2024-05-30 10:47:14.521755 keyring_proxy_stdio-0.1.3/README.md
--rw-r--r--   0        0        0      849 2024-05-30 13:03:19.094445 keyring_proxy_stdio-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      484 2024-05-30 11:15:44.762803 keyring_proxy_stdio-0.1.3/src/keyring_proxy_stdio/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 10:47:14.521755 keyring_proxy_stdio-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      368 1970-01-01 00:00:00.000000 keyring_proxy_stdio-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2024-05-30 10:47:14.521755 keyring_proxy_stdio-0.1.4/README.md
+-rw-r--r--   0        0        0      849 2024-05-30 13:28:16.714098 keyring_proxy_stdio-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      484 2024-05-30 11:15:44.762803 keyring_proxy_stdio-0.1.4/src/keyring_proxy_stdio/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 10:47:14.521755 keyring_proxy_stdio-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      368 1970-01-01 00:00:00.000000 keyring_proxy_stdio-0.1.4/PKG-INFO
```

### Comparing `keyring_proxy_stdio-0.1.3/pyproject.toml` & `keyring_proxy_stdio-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "keyring-proxy-stdio"
-version = "0.1.3"
+version = "0.1.4"
 description = "Default template for PDM package"
 authors = [
     { name = "Kalle M. Aagaard", email = "git@k-moeller.dk" },
 ]
 dependencies = [
-    "keyring-proxy>=0.1.8",
+    "keyring-proxy>=0.1.9",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

