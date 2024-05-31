# Comparing `tmp/dex-adaptors-0.0.3.tar.gz` & `tmp/dex-adaptors-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dex-adaptors-0.0.3.tar", last modified: Thu May 16 04:08:51 2024, max compression
+gzip compressed data, was "dex-adaptors-0.0.4.tar", last modified: Fri May 31 02:34:26 2024, max compression
```

## Comparing `dex-adaptors-0.0.3.tar` & `dex-adaptors-0.0.4.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 04:08:51.035125 dex-adaptors-0.0.3/
--rw-rw-rw-   0        0        0      118 2024-05-16 04:08:51.035125 dex-adaptors-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       14 2024-05-10 08:02:18.000000 dex-adaptors-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 04:08:50.986656 dex-adaptors-0.0.3/dex_adaptors/
--rw-rw-rw-   0        0        0        0 2024-05-13 12:09:47.000000 dex-adaptors-0.0.3/dex_adaptors/__init__.py
--rw-rw-rw-   0        0        0      267 2024-05-13 11:38:21.000000 dex-adaptors-0.0.3/dex_adaptors/aave_v3.py
--rw-rw-rw-   0        0        0      358 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/balancer_v2.py
--rw-rw-rw-   0        0        0      353 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/compound_v2.py
--rw-rw-rw-   0        0        0      317 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/curve.py
-drwxrwxrwx   0        0        0        0 2024-05-16 04:08:51.014368 dex-adaptors-0.0.3/dex_adaptors/exchange/
--rw-rw-rw-   0        0        0        0 2024-05-13 12:09:47.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/__init__.py
--rw-rw-rw-   0        0        0      705 2024-05-13 11:38:21.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/aave_v3.py
--rw-rw-rw-   0        0        0      857 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/balancer_v2.py
--rw-rw-rw-   0        0        0     1980 2024-05-13 11:35:28.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/base.py
--rw-rw-rw-   0        0        0     1050 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/compound_v2.py
--rw-rw-rw-   0        0        0      329 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/curve.py
--rw-rw-rw-   0        0        0     1906 2024-05-13 01:53:02.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/morpho.py
--rw-rw-rw-   0        0        0      386 2024-05-13 11:35:28.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/pendle.py
--rw-rw-rw-   0        0        0     3746 2024-05-12 10:42:13.000000 dex-adaptors-0.0.3/dex_adaptors/exchange/uniswap_v3.py
--rw-rw-rw-   0        0        0      681 2024-05-13 01:53:02.000000 dex-adaptors-0.0.3/dex_adaptors/morpho.py
-drwxrwxrwx   0        0        0        0 2024-05-16 04:08:51.034123 dex-adaptors-0.0.3/dex_adaptors/parsers/
--rw-rw-rw-   0        0        0        0 2024-05-13 12:09:47.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/__init__.py
--rw-rw-rw-   0        0        0     1097 2024-05-13 11:38:21.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/aave_v3.py
--rw-rw-rw-   0        0        0     1057 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/balancer_v2.py
--rw-rw-rw-   0        0        0      798 2024-05-12 10:42:13.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/base.py
--rw-rw-rw-   0        0        0     1096 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/compound_v2.py
--rw-rw-rw-   0        0        0     1477 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/curve.py
--rw-rw-rw-   0        0        0     1678 2024-05-13 01:53:02.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/morpho.py
--rw-rw-rw-   0        0        0     1980 2024-05-13 11:35:28.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/pendle.py
--rw-rw-rw-   0        0        0     1808 2024-05-16 04:05:39.000000 dex-adaptors-0.0.3/dex_adaptors/parsers/uniswap_v3.py
--rw-rw-rw-   0        0        0      569 2024-05-13 11:35:28.000000 dex-adaptors-0.0.3/dex_adaptors/pendle.py
--rw-rw-rw-   0        0        0      890 2024-05-12 10:42:13.000000 dex-adaptors-0.0.3/dex_adaptors/uniswap_v3.py
-drwxrwxrwx   0        0        0        0 2024-05-16 04:08:51.000028 dex-adaptors-0.0.3/dex_adaptors.egg-info/
--rw-rw-rw-   0        0        0      118 2024-05-16 04:08:50.000000 dex-adaptors-0.0.3/dex_adaptors.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2024-05-16 04:08:50.000000 dex-adaptors-0.0.3/dex_adaptors.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 04:08:50.000000 dex-adaptors-0.0.3/dex_adaptors.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1412 2024-05-16 04:08:50.000000 dex-adaptors-0.0.3/dex_adaptors.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-16 04:08:50.000000 dex-adaptors-0.0.3/dex_adaptors.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      648 2024-05-10 08:02:18.000000 dex-adaptors-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 04:08:51.035125 dex-adaptors-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      396 2024-05-16 04:06:01.000000 dex-adaptors-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:34:26.621672 dex-adaptors-0.0.4/
+-rw-rw-rw-   0        0        0      118 2024-05-31 02:34:26.620669 dex-adaptors-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-05-10 08:02:18.000000 dex-adaptors-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 02:34:26.525967 dex-adaptors-0.0.4/dex_adaptors/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:09:47.000000 dex-adaptors-0.0.4/dex_adaptors/__init__.py
+-rw-rw-rw-   0        0        0      267 2024-05-13 11:38:21.000000 dex-adaptors-0.0.4/dex_adaptors/aave_v3.py
+-rw-rw-rw-   0        0        0      358 2024-05-16 04:05:39.000000 dex-adaptors-0.0.4/dex_adaptors/balancer_v2.py
+-rw-rw-rw-   0        0        0      353 2024-05-16 04:05:39.000000 dex-adaptors-0.0.4/dex_adaptors/compound_v2.py
+-rw-rw-rw-   0        0        0      317 2024-05-16 04:05:39.000000 dex-adaptors-0.0.4/dex_adaptors/curve.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:34:26.575786 dex-adaptors-0.0.4/dex_adaptors/exchange/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:09:47.000000 dex-adaptors-0.0.4/dex_adaptors/exchange/__init__.py
+-rw-rw-rw-   0        0        0      705 2024-05-13 11:38:21.000000 dex-adaptors-0.0.4/dex_adaptors/exchange/aave_v3.py
+-rw-rw-rw-   0        0        0      857 2024-05-16 04:05:39.000000 dex-adaptors-0.0.4/dex_adaptors/exchange/balancer_v2.py
+-rw-rw-rw-   0        0        0     2045 2024-05-24 12:35:27.000000 dex-adaptors-0.0.4/dex_adaptors/exchange/base.py
+-rw-rw-rw-   0        0        0     1050 2024-05-16 04:05:39.000000 dex-adaptors-0.0.4/dex_adaptors/exchange/compound_v2.py
+-rw-rw-rw-   0        0        0      329 2024-05-16 04:05:39.000000 dex-adaptors-0.0.4/dex_adaptors/exchange/curve.py
+-rw-rw-rw-   0        0        0     4361 2024-05-30 16:31:00.000000 dex-adaptors-0.0.4/dex_adaptors/exchange/morpho.py
+-rw-rw-rw-   0        0        0      386 2024-05-13 11:35:28.000000 dex-adaptors-0.0.4/dex_adaptors/exchange/pendle.py
+-rw-rw-rw-   0        0        0     1474 2024-05-24 12:35:27.000000 dex-adaptors-0.0.4/dex_adaptors/exchange/silo.py
+-rw-rw-rw-   0        0        0     3746 2024-05-12 10:42:13.000000 dex-adaptors-0.0.4/dex_adaptors/exchange/uniswap_v3.py
+-rw-rw-rw-   0        0        0     1177 2024-05-30 16:31:00.000000 dex-adaptors-0.0.4/dex_adaptors/morpho.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:34:26.620669 dex-adaptors-0.0.4/dex_adaptors/parsers/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:09:47.000000 dex-adaptors-0.0.4/dex_adaptors/parsers/__init__.py
+-rw-rw-rw-   0        0        0     1097 2024-05-13 11:38:21.000000 dex-adaptors-0.0.4/dex_adaptors/parsers/aave_v3.py
+-rw-rw-rw-   0        0        0     1057 2024-05-16 04:05:39.000000 dex-adaptors-0.0.4/dex_adaptors/parsers/balancer_v2.py
+-rw-rw-rw-   0        0        0      798 2024-05-12 10:42:13.000000 dex-adaptors-0.0.4/dex_adaptors/parsers/base.py
+-rw-rw-rw-   0        0        0     1096 2024-05-16 04:05:39.000000 dex-adaptors-0.0.4/dex_adaptors/parsers/compound_v2.py
+-rw-rw-rw-   0        0        0     1477 2024-05-16 04:05:39.000000 dex-adaptors-0.0.4/dex_adaptors/parsers/curve.py
+-rw-rw-rw-   0        0        0     5373 2024-05-30 16:31:00.000000 dex-adaptors-0.0.4/dex_adaptors/parsers/morpho.py
+-rw-rw-rw-   0        0        0     1980 2024-05-13 11:35:28.000000 dex-adaptors-0.0.4/dex_adaptors/parsers/pendle.py
+-rw-rw-rw-   0        0        0     1458 2024-05-24 12:35:27.000000 dex-adaptors-0.0.4/dex_adaptors/parsers/silo.py
+-rw-rw-rw-   0        0        0     1808 2024-05-16 04:05:39.000000 dex-adaptors-0.0.4/dex_adaptors/parsers/uniswap_v3.py
+-rw-rw-rw-   0        0        0      569 2024-05-13 11:35:28.000000 dex-adaptors-0.0.4/dex_adaptors/pendle.py
+-rw-rw-rw-   0        0        0      359 2024-05-24 12:46:21.000000 dex-adaptors-0.0.4/dex_adaptors/silo.py
+-rw-rw-rw-   0        0        0      890 2024-05-12 10:42:13.000000 dex-adaptors-0.0.4/dex_adaptors/uniswap_v3.py
+drwxrwxrwx   0        0        0        0 2024-05-31 02:34:26.538374 dex-adaptors-0.0.4/dex_adaptors.egg-info/
+-rw-rw-rw-   0        0        0      118 2024-05-31 02:34:26.000000 dex-adaptors-0.0.4/dex_adaptors.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1087 2024-05-31 02:34:26.000000 dex-adaptors-0.0.4/dex_adaptors.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 02:34:26.000000 dex-adaptors-0.0.4/dex_adaptors.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1534 2024-05-31 02:34:26.000000 dex-adaptors-0.0.4/dex_adaptors.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 02:34:26.000000 dex-adaptors-0.0.4/dex_adaptors.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      648 2024-05-10 08:02:18.000000 dex-adaptors-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 02:34:26.621672 dex-adaptors-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      396 2024-05-31 02:31:54.000000 dex-adaptors-0.0.4/setup.py
```

### Comparing `dex-adaptors-0.0.3/dex_adaptors/exchange/aave_v3.py` & `dex-adaptors-0.0.4/dex_adaptors/exchange/aave_v3.py`

 * *Files identical despite different names*

### Comparing `dex-adaptors-0.0.3/dex_adaptors/exchange/balancer_v2.py` & `dex-adaptors-0.0.4/dex_adaptors/exchange/balancer_v2.py`

 * *Files identical despite different names*

### Comparing `dex-adaptors-0.0.3/dex_adaptors/exchange/base.py` & `dex-adaptors-0.0.4/dex_adaptors/exchange/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 from aiohttp import ClientResponse, ClientSession
 from gql import Client, gql
 from gql.transport.aiohttp import AIOHTTPTransport
 
 
 class GqlClient:
-    def __init__(self, base_endpoint: str):
+    def __init__(self, base_endpoint: str, fetch_schema_from_transport: bool = True):
         self.base_endpoint = base_endpoint
         self.transport = AIOHTTPTransport(url=self.base_endpoint)
-        self.client = Client(transport=self.transport, fetch_schema_from_transport=True)
+        self.client = Client(transport=self.transport, fetch_schema_from_transport=fetch_schema_from_transport)
 
     async def request(self, query: str) -> dict:
         query = gql(query)
         return await self.handle_response(await self.client.execute_async(query))
 
     async def handle_response(self, response: dict) -> dict:
         return response
```

### Comparing `dex-adaptors-0.0.3/dex_adaptors/exchange/compound_v2.py` & `dex-adaptors-0.0.4/dex_adaptors/exchange/compound_v2.py`

 * *Files identical despite different names*

### Comparing `dex-adaptors-0.0.3/dex_adaptors/exchange/uniswap_v3.py` & `dex-adaptors-0.0.4/dex_adaptors/exchange/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `dex-adaptors-0.0.3/dex_adaptors/parsers/aave_v3.py` & `dex-adaptors-0.0.4/dex_adaptors/parsers/aave_v3.py`

 * *Files identical despite different names*

### Comparing `dex-adaptors-0.0.3/dex_adaptors/parsers/balancer_v2.py` & `dex-adaptors-0.0.4/dex_adaptors/parsers/balancer_v2.py`

 * *Files identical despite different names*

### Comparing `dex-adaptors-0.0.3/dex_adaptors/parsers/base.py` & `dex-adaptors-0.0.4/dex_adaptors/parsers/base.py`

 * *Files identical despite different names*

### Comparing `dex-adaptors-0.0.3/dex_adaptors/parsers/compound_v2.py` & `dex-adaptors-0.0.4/dex_adaptors/parsers/compound_v2.py`

 * *Files identical despite different names*

### Comparing `dex-adaptors-0.0.3/dex_adaptors/parsers/curve.py` & `dex-adaptors-0.0.4/dex_adaptors/parsers/curve.py`

 * *Files identical despite different names*

### Comparing `dex-adaptors-0.0.3/dex_adaptors/parsers/pendle.py` & `dex-adaptors-0.0.4/dex_adaptors/parsers/pendle.py`

 * *Files identical despite different names*

### Comparing `dex-adaptors-0.0.3/dex_adaptors/parsers/uniswap_v3.py` & `dex-adaptors-0.0.4/dex_adaptors/parsers/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `dex-adaptors-0.0.3/dex_adaptors/pendle.py` & `dex-adaptors-0.0.4/dex_adaptors/pendle.py`

 * *Files identical despite different names*

### Comparing `dex-adaptors-0.0.3/dex_adaptors/uniswap_v3.py` & `dex-adaptors-0.0.4/dex_adaptors/uniswap_v3.py`

 * *Files identical despite different names*

### Comparing `dex-adaptors-0.0.3/dex_adaptors.egg-info/SOURCES.txt` & `dex-adaptors-0.0.4/dex_adaptors.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -4,31 +4,34 @@
 dex_adaptors/__init__.py
 dex_adaptors/aave_v3.py
 dex_adaptors/balancer_v2.py
 dex_adaptors/compound_v2.py
 dex_adaptors/curve.py
 dex_adaptors/morpho.py
 dex_adaptors/pendle.py
+dex_adaptors/silo.py
 dex_adaptors/uniswap_v3.py
 dex_adaptors.egg-info/PKG-INFO
 dex_adaptors.egg-info/SOURCES.txt
 dex_adaptors.egg-info/dependency_links.txt
 dex_adaptors.egg-info/requires.txt
 dex_adaptors.egg-info/top_level.txt
 dex_adaptors/exchange/__init__.py
 dex_adaptors/exchange/aave_v3.py
 dex_adaptors/exchange/balancer_v2.py
 dex_adaptors/exchange/base.py
 dex_adaptors/exchange/compound_v2.py
 dex_adaptors/exchange/curve.py
 dex_adaptors/exchange/morpho.py
 dex_adaptors/exchange/pendle.py
+dex_adaptors/exchange/silo.py
 dex_adaptors/exchange/uniswap_v3.py
 dex_adaptors/parsers/__init__.py
 dex_adaptors/parsers/aave_v3.py
 dex_adaptors/parsers/balancer_v2.py
 dex_adaptors/parsers/base.py
 dex_adaptors/parsers/compound_v2.py
 dex_adaptors/parsers/curve.py
 dex_adaptors/parsers/morpho.py
 dex_adaptors/parsers/pendle.py
+dex_adaptors/parsers/silo.py
 dex_adaptors/parsers/uniswap_v3.py
```

### Comparing `dex-adaptors-0.0.3/dex_adaptors.egg-info/requires.txt` & `dex-adaptors-0.0.4/dex_adaptors.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -6,18 +6,21 @@
 backoff==2.2.1
 backports.tarfile==1.1.1
 cachetools==5.3.3
 certifi==2024.2.2
 cfgv==3.4.0
 charset-normalizer==3.3.2
 colorama==0.4.6
+contourpy==1.2.1
+cycler==0.12.1
 distlib==0.3.8
 docutils==0.21.2
 exceptiongroup==1.2.1
 filelock==3.14.0
+fonttools==4.52.4
 frozenlist==1.4.1
 google-api-core==2.19.0
 google-api-python-client==2.129.0
 google-auth==2.29.0
 google-auth-httplib2==0.2.0
 google-auth-oauthlib==1.2.0
 googleapis-common-protos==1.63.0
@@ -28,37 +31,41 @@
 idna==3.7
 importlib_metadata==7.1.0
 iniconfig==2.0.0
 jaraco.classes==3.4.0
 jaraco.context==5.3.0
 jaraco.functools==4.0.1
 keyring==25.2.0
+kiwisolver==1.4.5
 markdown-it-py==3.0.0
+matplotlib==3.9.0
 mdurl==0.1.2
 more-itertools==10.2.0
 multidict==6.0.5
 nh3==0.2.17
 nodeenv==1.8.0
 numpy==1.26.4
 oauthlib==3.2.2
 packaging==24.0
 pandas==2.2.2
+pillow==10.3.0
 pkginfo==1.10.0
 platformdirs==4.2.1
 pluggy==1.5.0
 pre-commit==3.7.0
 proto-plus==1.23.0
 protobuf==4.25.3
 pyasn1==0.6.0
 pyasn1_modules==0.4.0
 Pygments==2.18.0
 pygsheets==2.0.6
 pyparsing==3.1.2
 pytest==8.2.0
 python-dateutil==2.9.0.post0
+python-dotenv==1.0.1
 pytz==2024.1
 pywin32-ctypes==0.2.2
 PyYAML==6.0.1
 readme_renderer==43.0
 requests==2.31.0
 requests-oauthlib==2.0.0
 requests-toolbelt==1.0.0
```

### Comparing `dex-adaptors-0.0.3/pyproject.toml` & `dex-adaptors-0.0.4/pyproject.toml`

 * *Files identical despite different names*

