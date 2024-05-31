# Comparing `tmp/keyring_proxy_socket-0.1.4.tar.gz` & `tmp/keyring_proxy_socket-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_proxy_socket-0.1.4.tar", last modified: Thu May 30 13:29:15 2024, max compression
+gzip compressed data, was "keyring_proxy_socket-0.1.5.tar", last modified: Fri May 31 10:06:29 2024, max compression
```

## Comparing `keyring_proxy_socket-0.1.4.tar` & `keyring_proxy_socket-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       23 2024-05-29 14:09:21.218215 keyring_proxy_socket-0.1.4/README.md
--rw-r--r--   0        0        0      836 2024-05-30 13:29:15.886697 keyring_proxy_socket-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      495 2024-05-30 11:16:33.931043 keyring_proxy_socket-0.1.4/src/keyring_proxy_socket/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 14:37:23.789730 keyring_proxy_socket-0.1.4/src/keyring_proxy_socket/py.typed
--rw-r--r--   0        0        0        0 2024-05-29 14:09:21.218215 keyring_proxy_socket-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0      353 1970-01-01 00:00:00.000000 keyring_proxy_socket-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-05-29 14:09:21.218215 keyring_proxy_socket-0.1.5/README.md
+-rw-r--r--   0        0        0      837 2024-05-31 10:06:29.623390 keyring_proxy_socket-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      495 2024-05-30 11:16:33.931043 keyring_proxy_socket-0.1.5/src/keyring_proxy_socket/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:37:23.789730 keyring_proxy_socket-0.1.5/src/keyring_proxy_socket/py.typed
+-rw-r--r--   0        0        0        0 2024-05-29 14:09:21.218215 keyring_proxy_socket-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0      354 1970-01-01 00:00:00.000000 keyring_proxy_socket-0.1.5/PKG-INFO
```

### Comparing `keyring_proxy_socket-0.1.4/pyproject.toml` & `keyring_proxy_socket-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "keyring-proxy-socket"
-version = "0.1.4"
+version = "0.1.5"
 description = "Socket backend"
 authors = [
     { name = "Kalle M. Aagaard", email = "git@k-moeller.dk" },
 ]
 dependencies = [
-    "keyring-proxy>=0.1.9",
+    "keyring-proxy>=0.1.12",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

