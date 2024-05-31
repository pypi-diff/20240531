# Comparing `tmp/pulumi_tls-5.1.0a1716964117.tar.gz` & `tmp/pulumi_tls-5.1.0a1717138108.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_tls-5.1.0a1716964117.tar", last modified: Wed May 29 06:33:55 2024, max compression
+gzip compressed data, was "pulumi_tls-5.1.0a1717138108.tar", last modified: Fri May 31 06:51:44 2024, max compression
```

## Comparing `pulumi_tls-5.1.0a1716964117.tar` & `pulumi_tls-5.1.0a1717138108.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:33:55.832135 pulumi_tls-5.1.0a1716964117/
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-29 06:33:55.832135 pulumi_tls-5.1.0a1716964117/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:33:55.832135 pulumi_tls-5.1.0a1716964117/pulumi_tls/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/cert_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:33:55.832135 pulumi_tls-5.1.0a1716964117/pulumi_tls/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/get_public_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    36895 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/locally_signed_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/private_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    45979 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls/self_signed_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:33:55.832135 pulumi_tls-5.1.0a1716964117/pulumi_tls.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-29 06:33:55.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-29 06:33:55.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:33:55.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 06:33:55.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 06:33:55.000000 pulumi_tls-5.1.0a1716964117/pulumi_tls.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-29 06:33:48.000000 pulumi_tls-5.1.0a1716964117/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 06:33:55.832135 pulumi_tls-5.1.0a1716964117/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:51:44.589875 pulumi_tls-5.1.0a1717138108/
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-31 06:51:44.589875 pulumi_tls-5.1.0a1717138108/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:51:44.589875 pulumi_tls-5.1.0a1717138108/pulumi_tls/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14351 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/cert_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:51:44.589875 pulumi_tls-5.1.0a1717138108/pulumi_tls/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10349 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/get_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36895 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/locally_signed_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14909 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/private_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    45979 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls/self_signed_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 06:51:44.589875 pulumi_tls-5.1.0a1717138108/pulumi_tls.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-31 06:51:44.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-31 06:51:44.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 06:51:44.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 06:51:44.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 06:51:44.000000 pulumi_tls-5.1.0a1717138108/pulumi_tls.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-31 06:51:38.000000 pulumi_tls-5.1.0a1717138108/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 06:51:44.589875 pulumi_tls-5.1.0a1717138108/setup.cfg
```

### Comparing `pulumi_tls-5.1.0a1716964117/PKG-INFO` & `pulumi_tls-5.1.0a1717138108/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_tls
-Version: 5.1.0a1716964117
+Version: 5.1.0a1717138108
 Summary: A Pulumi package to create TLS resources in Pulumi programs.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-tls
 Keywords: pulumi,tls
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_tls-5.1.0a1716964117/README.md` & `pulumi_tls-5.1.0a1717138108/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1716964117/pulumi_tls/__init__.py` & `pulumi_tls-5.1.0a1717138108/pulumi_tls/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1716964117/pulumi_tls/_inputs.py` & `pulumi_tls-5.1.0a1717138108/pulumi_tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1716964117/pulumi_tls/_utilities.py` & `pulumi_tls-5.1.0a1717138108/pulumi_tls/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1716964117/pulumi_tls/cert_request.py` & `pulumi_tls-5.1.0a1717138108/pulumi_tls/cert_request.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1716964117/pulumi_tls/config/outputs.py` & `pulumi_tls-5.1.0a1717138108/pulumi_tls/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1716964117/pulumi_tls/config/vars.py` & `pulumi_tls-5.1.0a1717138108/pulumi_tls/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1716964117/pulumi_tls/get_certificate.py` & `pulumi_tls-5.1.0a1717138108/pulumi_tls/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1716964117/pulumi_tls/get_public_key.py` & `pulumi_tls-5.1.0a1717138108/pulumi_tls/get_public_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1716964117/pulumi_tls/locally_signed_cert.py` & `pulumi_tls-5.1.0a1717138108/pulumi_tls/locally_signed_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1716964117/pulumi_tls/outputs.py` & `pulumi_tls-5.1.0a1717138108/pulumi_tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1716964117/pulumi_tls/private_key.py` & `pulumi_tls-5.1.0a1717138108/pulumi_tls/private_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1716964117/pulumi_tls/provider.py` & `pulumi_tls-5.1.0a1717138108/pulumi_tls/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1716964117/pulumi_tls/self_signed_cert.py` & `pulumi_tls-5.1.0a1717138108/pulumi_tls/self_signed_cert.py`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1716964117/pulumi_tls.egg-info/PKG-INFO` & `pulumi_tls-5.1.0a1717138108/pulumi_tls.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_tls
-Version: 5.1.0a1716964117
+Version: 5.1.0a1717138108
 Summary: A Pulumi package to create TLS resources in Pulumi programs.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-tls
 Keywords: pulumi,tls
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_tls-5.1.0a1716964117/pulumi_tls.egg-info/SOURCES.txt` & `pulumi_tls-5.1.0a1717138108/pulumi_tls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_tls-5.1.0a1716964117/pyproject.toml` & `pulumi_tls-5.1.0a1717138108/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_tls"
   description = "A Pulumi package to create TLS resources in Pulumi programs."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "tls"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "5.1.0a1716964117"
+  version = "5.1.0a1717138108"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-tls"
 
 [build-system]
```

