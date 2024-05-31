# Comparing `tmp/redactive-0.0.5.tar.gz` & `tmp/redactive-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redactive-0.0.5.tar", last modified: Sun Mar  3 02:47:47 2024, max compression
+gzip compressed data, was "redactive-0.1.0.tar", last modified: Fri May 31 05:46:07 2024, max compression
```

## Comparing `redactive-0.0.5.tar` & `redactive-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-03 02:47:47.154449 redactive-0.0.5/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      771 2024-03-03 02:47:47.154009 redactive-0.0.5/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      286 2023-09-13 23:34:13.000000 redactive-0.0.5/pyproject.toml
--rw-r--r--   0 vscode    (1000) vscode    (1000)      820 2024-03-03 02:47:47.155635 redactive-0.0.5/setup.cfg
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-03 02:47:47.125245 redactive-0.0.5/src/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-03 02:47:47.136459 redactive-0.0.5/src/redactive/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2024-03-03 02:42:59.000000 redactive-0.0.5/src/redactive/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-03 02:47:47.146292 redactive-0.0.5/src/redactive/client/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-02-15 04:31:11.000000 redactive-0.0.5/src/redactive/client/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      848 2024-03-03 02:47:40.000000 redactive-0.0.5/src/redactive/client/client.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-03 02:47:47.147762 redactive-0.0.5/src/redactive/client/rest/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4425 2024-03-03 02:20:24.000000 redactive-0.0.5/src/redactive/client/rest/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-03 02:47:47.149712 redactive-0.0.5/src/redactive/grpc/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2024-03-03 02:07:56.000000 redactive-0.0.5/src/redactive/grpc/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-03 02:47:47.150993 redactive-0.0.5/src/redactive/grpc/v1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     9875 2024-03-03 02:07:56.000000 redactive-0.0.5/src/redactive/grpc/v1/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2024-03-03 02:47:47.152639 redactive-0.0.5/src/redactive.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      771 2024-03-03 02:47:47.000000 redactive-0.0.5/src/redactive.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      401 2024-03-03 02:47:47.000000 redactive-0.0.5/src/redactive.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2024-03-03 02:47:47.000000 redactive-0.0.5/src/redactive.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2024-03-03 02:47:47.000000 redactive-0.0.5/src/redactive.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2024-03-03 02:47:47.000000 redactive-0.0.5/src/redactive.egg-info/top_level.txt
+drwxr-xr-x   0 kochie     (501) staff       (20)        0 2024-05-31 05:46:07.881829 redactive-0.1.0/
+-rw-r--r--   0 kochie     (501) staff       (20)      703 2024-05-31 05:46:07.881740 redactive-0.1.0/PKG-INFO
+-rw-r--r--   0 kochie     (501) staff       (20)      309 2024-05-31 05:38:34.000000 redactive-0.1.0/pyproject.toml
+-rw-r--r--   0 kochie     (501) staff       (20)      763 2024-05-31 05:46:07.882097 redactive-0.1.0/setup.cfg
+drwxr-xr-x   0 kochie     (501) staff       (20)        0 2024-05-31 05:46:07.878822 redactive-0.1.0/src/
+drwxr-xr-x   0 kochie     (501) staff       (20)        0 2024-05-31 05:46:07.879982 redactive-0.1.0/src/redactive/
+-rw-r--r--   0 kochie     (501) staff       (20)      104 2024-05-31 05:39:39.000000 redactive-0.1.0/src/redactive/__init__.py
+-rw-r--r--   0 kochie     (501) staff       (20)     3069 2024-05-31 05:41:09.000000 redactive-0.1.0/src/redactive/auth_client.py
+drwxr-xr-x   0 kochie     (501) staff       (20)        0 2024-05-31 05:46:07.878968 redactive-0.1.0/src/redactive/client/
+drwxr-xr-x   0 kochie     (501) staff       (20)        0 2024-05-31 05:46:07.880753 redactive-0.1.0/src/redactive/client/rest/
+-rw-r--r--   0 kochie     (501) staff       (20)     4425 2024-05-31 05:39:40.000000 redactive-0.1.0/src/redactive/client/rest/__init__.py
+drwxr-xr-x   0 kochie     (501) staff       (20)        0 2024-05-31 05:46:07.881004 redactive-0.1.0/src/redactive/grpc/
+-rw-r--r--   0 kochie     (501) staff       (20)        0 2024-03-03 02:07:56.000000 redactive-0.1.0/src/redactive/grpc/__init__.py
+drwxr-xr-x   0 kochie     (501) staff       (20)        0 2024-05-31 05:46:07.881102 redactive-0.1.0/src/redactive/grpc/v1/
+-rw-r--r--   0 kochie     (501) staff       (20)     6549 2024-05-31 05:39:45.000000 redactive-0.1.0/src/redactive/grpc/v1/__init__.py
+-rw-r--r--   0 kochie     (501) staff       (20)     2010 2024-05-31 05:38:34.000000 redactive-0.1.0/src/redactive/search_client.py
+drwxr-xr-x   0 kochie     (501) staff       (20)        0 2024-05-31 05:46:07.881350 redactive-0.1.0/src/redactive.egg-info/
+-rw-r--r--   0 kochie     (501) staff       (20)      703 2024-05-31 05:46:07.000000 redactive-0.1.0/src/redactive.egg-info/PKG-INFO
+-rw-r--r--   0 kochie     (501) staff       (20)      397 2024-05-31 05:46:07.000000 redactive-0.1.0/src/redactive.egg-info/SOURCES.txt
+-rw-r--r--   0 kochie     (501) staff       (20)        1 2024-05-31 05:46:07.000000 redactive-0.1.0/src/redactive.egg-info/dependency_links.txt
+-rw-r--r--   0 kochie     (501) staff       (20)      108 2024-05-31 05:46:07.000000 redactive-0.1.0/src/redactive.egg-info/requires.txt
+-rw-r--r--   0 kochie     (501) staff       (20)       10 2024-05-31 05:46:07.000000 redactive-0.1.0/src/redactive.egg-info/top_level.txt
```

### Comparing `redactive-0.0.5/PKG-INFO` & `redactive-0.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: redactive
-Version: 0.0.5
+Version: 0.1.0
 Home-page: https://github.com/redactive-ai/redactive
 Author: redactive.ai
 Project-URL: Bug Tracker, https://github.com/redactive-ai/redactive/labels/sdk:python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: cloud-mappings
+Requires-Dist: pydantic
 Requires-Dist: betterproto[compiler]==2.0.0b5
 Requires-Dist: grpclib[protobuf]
-Requires-Dist: openai==1.0.0b1
-Requires-Dist: python-dotenv
-Provides-Extra: all
-Requires-Dist: redactive-service; extra == "all"
+Requires-Dist: httpx
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-asyncio; extra == "tests"
+Requires-Dist: pytest-httpx; extra == "tests"
```

### Comparing `redactive-0.0.5/setup.cfg` & `redactive-0.1.0/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = redactive
-version = 0.0.5
+version = 0.1.0
 author = redactive.ai
 description = 
 keywords = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/redactive-ai/redactive
 project_urls = 
@@ -16,26 +16,24 @@
 
 [options]
 package_dir = 
 	= src
 packages = find_namespace:
 python_requires = >=3.10
 install_requires = 
-	cloud-mappings # placeholder
+	pydantic
 	betterproto[compiler]==2.0.0b5
 	grpclib[protobuf]
-	openai==1.0.0b1
-	python-dotenv
+	httpx
 
 [options.extras_require]
-all = 
-	redactive-service
 tests = 
 	pytest
 	pytest-asyncio
+	pytest-httpx
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `redactive-0.0.5/src/redactive/client/rest/__init__.py` & `redactive-0.1.0/src/redactive/client/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `redactive-0.0.5/src/redactive.egg-info/PKG-INFO` & `redactive-0.1.0/src/redactive.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: redactive
-Version: 0.0.5
+Version: 0.1.0
 Home-page: https://github.com/redactive-ai/redactive
 Author: redactive.ai
 Project-URL: Bug Tracker, https://github.com/redactive-ai/redactive/labels/sdk:python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: cloud-mappings
+Requires-Dist: pydantic
 Requires-Dist: betterproto[compiler]==2.0.0b5
 Requires-Dist: grpclib[protobuf]
-Requires-Dist: openai==1.0.0b1
-Requires-Dist: python-dotenv
-Provides-Extra: all
-Requires-Dist: redactive-service; extra == "all"
+Requires-Dist: httpx
 Provides-Extra: tests
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-asyncio; extra == "tests"
+Requires-Dist: pytest-httpx; extra == "tests"
```

