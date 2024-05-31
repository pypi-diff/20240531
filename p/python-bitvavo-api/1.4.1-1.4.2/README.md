# Comparing `tmp/python_bitvavo_api-1.4.1.tar.gz` & `tmp/python_bitvavo_api-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_bitvavo_api-1.4.1.tar", last modified: Mon Feb 26 12:38:36 2024, max compression
+gzip compressed data, was "python_bitvavo_api-1.4.2.tar", last modified: Fri May 31 11:41:08 2024, max compression
```

## Comparing `python_bitvavo_api-1.4.1.tar` & `python_bitvavo_api-1.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:38:36.711177 python_bitvavo_api-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-26 12:38:29.000000 python_bitvavo_api-1.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-02-26 12:38:36.711177 python_bitvavo_api-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-02-26 12:38:29.000000 python_bitvavo_api-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:38:36.707177 python_bitvavo_api-1.4.1/python_bitvavo_api/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-26 12:38:29.000000 python_bitvavo_api-1.4.1/python_bitvavo_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31333 2024-02-26 12:38:29.000000 python_bitvavo_api-1.4.1/python_bitvavo_api/bitvavo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-02-26 12:38:29.000000 python_bitvavo_api-1.4.1/python_bitvavo_api/testApi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 12:38:36.711177 python_bitvavo_api-1.4.1/python_bitvavo_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-02-26 12:38:36.000000 python_bitvavo_api-1.4.1/python_bitvavo_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-26 12:38:36.000000 python_bitvavo_api-1.4.1/python_bitvavo_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 12:38:36.000000 python_bitvavo_api-1.4.1/python_bitvavo_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-26 12:38:36.000000 python_bitvavo_api-1.4.1/python_bitvavo_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-26 12:38:36.000000 python_bitvavo_api-1.4.1/python_bitvavo_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 12:38:36.711177 python_bitvavo_api-1.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      964 2024-02-26 12:38:29.000000 python_bitvavo_api-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:41:08.044220 python_bitvavo_api-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-31 11:41:00.000000 python_bitvavo_api-1.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8850 2024-05-31 11:41:08.044220 python_bitvavo_api-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8244 2024-05-31 11:41:00.000000 python_bitvavo_api-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:41:08.044220 python_bitvavo_api-1.4.2/python_bitvavo_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 11:41:00.000000 python_bitvavo_api-1.4.2/python_bitvavo_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31333 2024-05-31 11:41:00.000000 python_bitvavo_api-1.4.2/python_bitvavo_api/bitvavo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-31 11:41:00.000000 python_bitvavo_api-1.4.2/python_bitvavo_api/testApi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 11:41:08.044220 python_bitvavo_api-1.4.2/python_bitvavo_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8850 2024-05-31 11:41:08.000000 python_bitvavo_api-1.4.2/python_bitvavo_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-31 11:41:08.000000 python_bitvavo_api-1.4.2/python_bitvavo_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 11:41:08.000000 python_bitvavo_api-1.4.2/python_bitvavo_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 11:41:08.000000 python_bitvavo_api-1.4.2/python_bitvavo_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 11:41:08.000000 python_bitvavo_api-1.4.2/python_bitvavo_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 11:41:08.044220 python_bitvavo_api-1.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      986 2024-05-31 11:41:00.000000 python_bitvavo_api-1.4.2/setup.py
```

### Comparing `python_bitvavo_api-1.4.1/LICENSE.txt` & `python_bitvavo_api-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_bitvavo_api-1.4.1/PKG-INFO` & `python_bitvavo_api-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: python_bitvavo_api
-Version: 1.4.1
+Version: 1.4.2
 Summary: Use Bitvavo SDK for Python to buy, sell, and store over 200 digital assets on Bitvavo from inside your app.
 Home-page: https://github.com/bitvavo/python-bitvavo-api
 Author: Bitvavo
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: websocket-client
-Requires-Dist: requests==2.31.0
+Requires-Dist: websocket-client<2.0.0,>=1.6.0
+Requires-Dist: requests<3.0.0,>=2.31.0
 Requires-Dist: setuptools
 
 
 # Bitvavo SDK for Python
 
 Crypto starts with Bitvavo. 
 You use Bitvavo SDK for Python to buy, sell, and store over 200 digital assets on Bitvavo from inside your app.
```

### Comparing `python_bitvavo_api-1.4.1/README.md` & `python_bitvavo_api-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `python_bitvavo_api-1.4.1/python_bitvavo_api/bitvavo.py` & `python_bitvavo_api-1.4.2/python_bitvavo_api/bitvavo.py`

 * *Files identical despite different names*

### Comparing `python_bitvavo_api-1.4.1/python_bitvavo_api/testApi.py` & `python_bitvavo_api-1.4.2/python_bitvavo_api/testApi.py`

 * *Files identical despite different names*

### Comparing `python_bitvavo_api-1.4.1/python_bitvavo_api.egg-info/PKG-INFO` & `python_bitvavo_api-1.4.2/python_bitvavo_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: python_bitvavo_api
-Version: 1.4.1
+Version: 1.4.2
 Summary: Use Bitvavo SDK for Python to buy, sell, and store over 200 digital assets on Bitvavo from inside your app.
 Home-page: https://github.com/bitvavo/python-bitvavo-api
 Author: Bitvavo
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
-Requires-Dist: websocket-client
-Requires-Dist: requests==2.31.0
+Requires-Dist: websocket-client<2.0.0,>=1.6.0
+Requires-Dist: requests<3.0.0,>=2.31.0
 Requires-Dist: setuptools
 
 
 # Bitvavo SDK for Python
 
 Crypto starts with Bitvavo. 
 You use Bitvavo SDK for Python to buy, sell, and store over 200 digital assets on Bitvavo from inside your app.
```

### Comparing `python_bitvavo_api-1.4.1/setup.py` & `python_bitvavo_api-1.4.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="python_bitvavo_api",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version="1.4.1",
+    version="v1.4.2",
     author="Bitvavo",
     description="Use Bitvavo SDK for Python to buy, sell, and store over 200 digital assets on Bitvavo from inside your app.",
     url="https://github.com/bitvavo/python-bitvavo-api",
     packages=find_packages(),
     install_requires=[
-        'websocket-client',
-        'requests==2.31.0',
+        'websocket-client>=1.6.0,<2.0.0',
+        'requests>=2.31.0,<3.0.0',
         'setuptools'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: ISC License (ISCL)",
         "Operating System :: OS Independent",
     ],
```

