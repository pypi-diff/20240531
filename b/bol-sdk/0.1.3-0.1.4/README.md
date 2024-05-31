# Comparing `tmp/bol_sdk-0.1.3.tar.gz` & `tmp/bol_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bol_sdk-0.1.3.tar", max compression
+gzip compressed data, was "bol_sdk-0.1.4.tar", max compression
```

## Comparing `bol_sdk-0.1.3.tar` & `bol_sdk-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       45 2024-05-03 17:53:19.404594 bol_sdk-0.1.3/bol_SDK/__init__.py
--rw-r--r--   0        0        0      895 2024-05-06 09:27:23.359081 bol_sdk-0.1.3/bol_SDK/__main__.py
--rw-r--r--   0        0        0    15932 2024-05-06 09:27:23.357641 bol_sdk-0.1.3/bol_SDK/bol_SDK.py
--rw-r--r--   0        0        0       43 2024-05-03 17:53:19.405330 bol_sdk-0.1.3/bol_SDK/constants.py
--rw-r--r--   0        0        0      382 2024-05-06 16:06:40.296760 bol_sdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 bol_sdk-0.1.3/setup.py
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 bol_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-05-03 17:53:19.404594 bol_sdk-0.1.4/bol_SDK/__init__.py
+-rw-r--r--   0        0        0      895 2024-05-06 09:27:23.359081 bol_sdk-0.1.4/bol_SDK/__main__.py
+-rw-r--r--   0        0        0    15932 2024-05-06 09:27:23.357641 bol_sdk-0.1.4/bol_SDK/bol_SDK.py
+-rw-r--r--   0        0        0       43 2024-05-03 17:53:19.405330 bol_sdk-0.1.4/bol_SDK/constants.py
+-rw-r--r--   0        0        0      381 2024-05-31 17:04:24.904573 bol_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 bol_sdk-0.1.4/setup.py
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 bol_sdk-0.1.4/PKG-INFO
```

### Comparing `bol_sdk-0.1.3/bol_SDK/__main__.py` & `bol_sdk-0.1.4/bol_SDK/__main__.py`

 * *Files identical despite different names*

### Comparing `bol_sdk-0.1.3/bol_SDK/bol_SDK.py` & `bol_sdk-0.1.4/bol_SDK/bol_SDK.py`

 * *Files identical despite different names*

### Comparing `bol_sdk-0.1.3/setup.py` & `bol_sdk-0.1.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.23.1,<2.0.0',
  'pandas>=1.4.3,<2.0.0',
- 'python-dotenv>=0.20.0,<0.21.0',
+ 'python-dotenv>=1.0.1,<2.0.0',
  'requests>=2.28.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'bol-sdk',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': '',
     'long_description': 'None',
     'author': 'Genhao Li',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

