# Comparing `tmp/tuyul_sdk-0.0.1rc6.tar.gz` & `tmp/tuyul_sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuyul_sdk-0.0.1rc6.tar", max compression
+gzip compressed data, was "tuyul_sdk-0.1.0.tar", max compression
```

## Comparing `tuyul_sdk-0.0.1rc6.tar` & `tuyul_sdk-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,26 @@
--rw-r--r--   0        0        0      606 2024-05-30 08:04:19.410534 tuyul_sdk-0.0.1rc6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 00:34:07.019714 tuyul_sdk-0.0.1rc6/README.md
--rw-r--r--   0        0        0      726 2024-05-30 07:06:45.616867 tuyul_sdk-0.0.1rc6/tuyul_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 20:21:44.103798 tuyul_sdk-0.0.1rc6/tuyul_sdk/_certificate/__init__.py
--rw-r--r--   0        0        0   286252 2024-03-18 20:21:44.105798 tuyul_sdk-0.0.1rc6/tuyul_sdk/_certificate/cacert.pem
--rw-r--r--   0        0        0     8658 2024-05-30 02:19:24.831329 tuyul_sdk-0.0.1rc6/tuyul_sdk/_Cipher.py
--rw-r--r--   0        0        0      454 2024-03-30 18:29:45.577779 tuyul_sdk-0.0.1rc6/tuyul_sdk/_Color.py
--rw-r--r--   0        0        0     7153 2024-05-30 06:51:32.411276 tuyul_sdk-0.0.1rc6/tuyul_sdk/_Connection.py
--rw-r--r--   0        0        0     2654 2024-05-30 03:57:45.352001 tuyul_sdk-0.0.1rc6/tuyul_sdk/_Database.py
--rw-r--r--   0        0        0      509 2024-03-18 20:21:43.622544 tuyul_sdk-0.0.1rc6/tuyul_sdk/_input.py
--rw-r--r--   0        0        0      719 2024-03-18 20:21:43.623543 tuyul_sdk-0.0.1rc6/tuyul_sdk/_Line.py
--rw-r--r--   0        0        0      826 2024-05-26 07:36:03.091067 tuyul_sdk-0.0.1rc6/tuyul_sdk/_Log.py
--rw-r--r--   0        0        0     2373 2024-05-26 07:35:32.143357 tuyul_sdk-0.0.1rc6/tuyul_sdk/_Progress.py
--rw-r--r--   0        0        0      229 2024-05-26 07:33:25.053372 tuyul_sdk-0.0.1rc6/tuyul_sdk/_Reset.py
--rw-r--r--   0        0        0     3000 2024-05-26 07:32:31.114228 tuyul_sdk-0.0.1rc6/tuyul_sdk/_UserAgent.py
--rw-r--r--   0        0        0       93 2024-05-30 02:34:28.449126 tuyul_sdk-0.0.1rc6/tuyul_sdk/sql.py
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 tuyul_sdk-0.0.1rc6/setup.py
--rw-r--r--   0        0        0      866 1970-01-01 00:00:00.000000 tuyul_sdk-0.0.1rc6/PKG-INFO
+-rw-r--r--   0        0        0      616 2024-05-31 04:01:32.655168 tuyul_sdk-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 02:26:37.717294 tuyul_sdk-0.1.0/README.md
+-rw-r--r--   0        0        0      125 2024-05-31 03:57:46.818106 tuyul_sdk-0.1.0/tuyul_sdk/__init__.py
+-rw-r--r--   0        0        0      303 2024-05-31 03:14:55.963434 tuyul_sdk-0.1.0/tuyul_sdk/_Cipher/__init__.py
+-rw-r--r--   0        0        0     6029 2024-05-31 03:13:40.901253 tuyul_sdk-0.1.0/tuyul_sdk/_Cipher/AES.py
+-rw-r--r--   0        0        0     1559 2024-05-31 02:38:39.120584 tuyul_sdk-0.1.0/tuyul_sdk/_Cipher/Password.py
+-rw-r--r--   0        0        0      518 2024-05-31 02:45:58.639747 tuyul_sdk-0.1.0/tuyul_sdk/_Cipher/Salt.py
+-rw-r--r--   0        0        0      101 2024-05-31 03:28:50.075893 tuyul_sdk-0.1.0/tuyul_sdk/_Connection/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 20:21:44.103798 tuyul_sdk-0.1.0/tuyul_sdk/_Connection/_certificate/__init__.py
+-rw-r--r--   0        0        0   286252 2024-03-18 20:21:44.105798 tuyul_sdk-0.1.0/tuyul_sdk/_Connection/_certificate/cacert.pem
+-rw-r--r--   0        0        0     1581 2024-05-31 03:28:19.129050 tuyul_sdk-0.1.0/tuyul_sdk/_Connection/httpx.py
+-rw-r--r--   0        0        0     1294 2024-05-31 03:28:24.109127 tuyul_sdk-0.1.0/tuyul_sdk/_Connection/requests.py
+-rw-r--r--   0        0        0     4286 2024-05-31 03:18:09.960902 tuyul_sdk-0.1.0/tuyul_sdk/_Connection/utils.py
+-rw-r--r--   0        0        0     2654 2024-05-30 03:57:45.352001 tuyul_sdk-0.1.0/tuyul_sdk/_Database.py
+-rw-r--r--   0        0        0       93 2024-05-30 02:34:28.449126 tuyul_sdk-0.1.0/tuyul_sdk/sql.py
+-rw-r--r--   0        0        0      366 2024-05-31 03:59:01.720591 tuyul_sdk-0.1.0/tuyul_sdk/Utils/__init__.py
+-rw-r--r--   0        0        0      454 2024-03-30 18:29:45.577779 tuyul_sdk-0.1.0/tuyul_sdk/Utils/_Color.py
+-rw-r--r--   0        0        0     3669 2024-05-31 02:45:00.849778 tuyul_sdk-0.1.0/tuyul_sdk/Utils/_hexbytes.py
+-rw-r--r--   0        0        0      509 2024-03-18 20:21:43.622544 tuyul_sdk-0.1.0/tuyul_sdk/Utils/_input.py
+-rw-r--r--   0        0        0      719 2024-03-18 20:21:43.623543 tuyul_sdk-0.1.0/tuyul_sdk/Utils/_Line.py
+-rw-r--r--   0        0        0      826 2024-05-26 07:36:03.091067 tuyul_sdk-0.1.0/tuyul_sdk/Utils/_Log.py
+-rw-r--r--   0        0        0     2373 2024-05-26 07:35:32.143357 tuyul_sdk-0.1.0/tuyul_sdk/Utils/_Progress.py
+-rw-r--r--   0        0        0      229 2024-05-26 07:33:25.053372 tuyul_sdk-0.1.0/tuyul_sdk/Utils/_Reset.py
+-rw-r--r--   0        0        0     3000 2024-05-26 07:32:31.114228 tuyul_sdk-0.1.0/tuyul_sdk/Utils/_UserAgent.py
+-rw-r--r--   0        0        0      944 1970-01-01 00:00:00.000000 tuyul_sdk-0.1.0/setup.py
+-rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 tuyul_sdk-0.1.0/PKG-INFO
```

### Comparing `tuyul_sdk-0.0.1rc6/pyproject.toml` & `tuyul_sdk-0.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [tool.poetry]
 name = "tuyul-sdk"
-version = "0.0.1rc6"
+version = "0.1.0"
 description = ""
-authors = ["Antoni Oktha Fernandes <37358597+DesKaOne@users.noreply.github.com>"]
+authors = ["DesKaOne <DesKaOne@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "tuyul_sdk"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-pycryptodomex = "^3.20.0"
-colorama = "^0.4.6"
-sqlalchemy = "^2.0.30"
-sqlalchemy-utils = "^0.41.2"
-random-user-agent = "^1.0.1"
-base58 = "^2.1.1"
-requests = "2.31.0"
-httpx = {extras = ["http2","socks"], version = "0.27.0"}
-chardet = "^5.2.0"
+base58 = "2.1.1"
+chardet = "5.2.0"
+colorama = "0.4.6"
+httpx = {version = "0.27.0", extras = ["socks"]}
+pycryptodomex = "3.20.0"
+random-user-agent = "1.0.1"
+requests = "2.32.3"
+requests-toolbelt = "0.10.1"
+sqlalchemy = "2.0.30"
+sqlalchemy-utils = "0.41.2"
+urllib3 = "1.26.15"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tuyul_sdk-0.0.1rc6/tuyul_sdk/_certificate/cacert.pem` & `tuyul_sdk-0.1.0/tuyul_sdk/_Connection/_certificate/cacert.pem`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc6/tuyul_sdk/_Database.py` & `tuyul_sdk-0.1.0/tuyul_sdk/_Database.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc6/tuyul_sdk/_Line.py` & `tuyul_sdk-0.1.0/tuyul_sdk/Utils/_Line.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc6/tuyul_sdk/_Log.py` & `tuyul_sdk-0.1.0/tuyul_sdk/Utils/_Log.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc6/tuyul_sdk/_Progress.py` & `tuyul_sdk-0.1.0/tuyul_sdk/Utils/_Progress.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc6/tuyul_sdk/_UserAgent.py` & `tuyul_sdk-0.1.0/tuyul_sdk/Utils/_UserAgent.py`

 * *Files identical despite different names*

### Comparing `tuyul_sdk-0.0.1rc6/setup.py` & `tuyul_sdk-0.1.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['tuyul_sdk', 'tuyul_sdk._certificate']
+['tuyul_sdk',
+ 'tuyul_sdk.Utils',
+ 'tuyul_sdk._Cipher',
+ 'tuyul_sdk._Connection',
+ 'tuyul_sdk._Connection._certificate']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['base58>=2.1.1,<3.0.0',
- 'chardet>=5.2.0,<6.0.0',
- 'colorama>=0.4.6,<0.5.0',
- 'httpx[http2,socks]==0.27.0',
- 'pycryptodomex>=3.20.0,<4.0.0',
- 'random-user-agent>=1.0.1,<2.0.0',
- 'requests==2.31.0',
- 'sqlalchemy-utils>=0.41.2,<0.42.0',
- 'sqlalchemy>=2.0.30,<3.0.0']
+['base58==2.1.1',
+ 'chardet==5.2.0',
+ 'colorama==0.4.6',
+ 'httpx[socks]==0.27.0',
+ 'pycryptodomex==3.20.0',
+ 'random-user-agent==1.0.1',
+ 'requests-toolbelt==0.10.1',
+ 'requests==2.32.3',
+ 'sqlalchemy-utils==0.41.2',
+ 'sqlalchemy==2.0.30',
+ 'urllib3==1.26.15']
 
 setup_kwargs = {
     'name': 'tuyul-sdk',
-    'version': '0.0.1rc6',
+    'version': '0.1.0',
     'description': '',
     'long_description': '',
-    'author': 'Antoni Oktha Fernandes',
-    'author_email': '37358597+DesKaOne@users.noreply.github.com',
+    'author': 'DesKaOne',
+    'author_email': 'DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
```

### Comparing `tuyul_sdk-0.0.1rc6/PKG-INFO` & `tuyul_sdk-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: tuyul-sdk
-Version: 0.0.1rc6
+Version: 0.1.0
 Summary: 
-Author: Antoni Oktha Fernandes
-Author-email: 37358597+DesKaOne@users.noreply.github.com
+Author: DesKaOne
+Author-email: DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: base58 (>=2.1.1,<3.0.0)
-Requires-Dist: chardet (>=5.2.0,<6.0.0)
-Requires-Dist: colorama (>=0.4.6,<0.5.0)
-Requires-Dist: httpx[http2,socks] (==0.27.0)
-Requires-Dist: pycryptodomex (>=3.20.0,<4.0.0)
-Requires-Dist: random-user-agent (>=1.0.1,<2.0.0)
-Requires-Dist: requests (==2.31.0)
-Requires-Dist: sqlalchemy (>=2.0.30,<3.0.0)
-Requires-Dist: sqlalchemy-utils (>=0.41.2,<0.42.0)
+Requires-Dist: base58 (==2.1.1)
+Requires-Dist: chardet (==5.2.0)
+Requires-Dist: colorama (==0.4.6)
+Requires-Dist: httpx[socks] (==0.27.0)
+Requires-Dist: pycryptodomex (==3.20.0)
+Requires-Dist: random-user-agent (==1.0.1)
+Requires-Dist: requests (==2.32.3)
+Requires-Dist: requests-toolbelt (==0.10.1)
+Requires-Dist: sqlalchemy (==2.0.30)
+Requires-Dist: sqlalchemy-utils (==0.41.2)
+Requires-Dist: urllib3 (==1.26.15)
 Description-Content-Type: text/markdown
```

