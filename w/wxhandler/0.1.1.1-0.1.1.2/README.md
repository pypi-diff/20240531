# Comparing `tmp/wxhandler-0.1.1.1.tar.gz` & `tmp/wxhandler-0.1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxhandler-0.1.1.1.tar", last modified: Fri May 31 00:05:47 2024, max compression
+gzip compressed data, was "wxhandler-0.1.1.2.tar", last modified: Fri May 31 00:12:55 2024, max compression
```

## Comparing `wxhandler-0.1.1.1.tar` & `wxhandler-0.1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 00:05:47.809847 wxhandler-0.1.1.1/
--rw-rw-rw-   0        0        0     1055 2024-05-30 23:10:26.000000 wxhandler-0.1.1.1/LICENSE
--rw-rw-rw-   0        0        0      888 2024-05-31 00:05:47.808872 wxhandler-0.1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      400 2024-05-31 00:04:24.000000 wxhandler-0.1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-31 00:05:47.810848 wxhandler-0.1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      680 2024-05-31 00:05:36.000000 wxhandler-0.1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 00:05:47.792476 wxhandler-0.1.1.1/wxhandler/
--rw-rw-rw-   0        0        0        0 2024-05-30 23:05:42.000000 wxhandler-0.1.1.1/wxhandler/__init__.py
--rw-rw-rw-   0        0        0    23197 2024-05-30 15:38:25.000000 wxhandler-0.1.1.1/wxhandler/wxhandler.py
-drwxrwxrwx   0        0        0        0 2024-05-31 00:05:47.805848 wxhandler-0.1.1.1/wxhandler.egg-info/
--rw-rw-rw-   0        0        0      888 2024-05-31 00:05:47.000000 wxhandler-0.1.1.1/wxhandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-05-31 00:05:47.000000 wxhandler-0.1.1.1/wxhandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 00:05:47.000000 wxhandler-0.1.1.1/wxhandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 00:05:47.000000 wxhandler-0.1.1.1/wxhandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-31 00:05:47.000000 wxhandler-0.1.1.1/wxhandler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 00:12:55.667397 wxhandler-0.1.1.2/
+-rw-rw-rw-   0        0        0     1055 2024-05-30 23:10:26.000000 wxhandler-0.1.1.2/LICENSE
+-rw-rw-rw-   0        0        0      916 2024-05-31 00:12:55.665398 wxhandler-0.1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-05-31 00:07:37.000000 wxhandler-0.1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-31 00:12:55.667397 wxhandler-0.1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      680 2024-05-31 00:12:31.000000 wxhandler-0.1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:12:55.649933 wxhandler-0.1.1.2/wxhandler/
+-rw-rw-rw-   0        0        0       61 2024-05-31 00:11:00.000000 wxhandler-0.1.1.2/wxhandler/__init__.py
+-rw-rw-rw-   0        0        0    23197 2024-05-30 15:38:25.000000 wxhandler-0.1.1.2/wxhandler/wxhandler.py
+drwxrwxrwx   0        0        0        0 2024-05-31 00:12:55.664399 wxhandler-0.1.1.2/wxhandler.egg-info/
+-rw-rw-rw-   0        0        0      916 2024-05-31 00:12:55.000000 wxhandler-0.1.1.2/wxhandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-05-31 00:12:55.000000 wxhandler-0.1.1.2/wxhandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 00:12:55.000000 wxhandler-0.1.1.2/wxhandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 00:12:55.000000 wxhandler-0.1.1.2/wxhandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-31 00:12:55.000000 wxhandler-0.1.1.2/wxhandler.egg-info/top_level.txt
```

### Comparing `wxhandler-0.1.1.1/LICENSE` & `wxhandler-0.1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wxhandler-0.1.1.1/PKG-INFO` & `wxhandler-0.1.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhandler
-Version: 0.1.1.1
+Version: 0.1.1.2
 Summary: A Python package for handling wxHandler operations.
 Home-page: https://github.com/chenbifu/wxhandler
 Author: chenbifu
 Author-email: pythonaaa@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,11 +23,12 @@
 pip install wxhandler
 ```
 ## Usage
 ```python
 from wxhandler import wxHandler
 
 handler = wxHandler(base_url="http://127.0.0.1:19088")
-handler.hookSyncMsgNew(enableHttp=True, httpPort=19099)
+response = handler.hookSyncMsgNew(enableHttp=True, httpPort=19099)
+print(response)
 ```
```

### Comparing `wxhandler-0.1.1.1/setup.py` & `wxhandler-0.1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="wxhandler",
-    version="0.1.1.1",
+    version="0.1.1.2",
     packages=find_packages(),
     install_requires=[
         "requests",
     ],
     author="chenbifu",
     author_email="pythonaaa@gmail.com",
     description="A Python package for handling wxHandler operations.",
```

### Comparing `wxhandler-0.1.1.1/wxhandler/wxhandler.py` & `wxhandler-0.1.1.2/wxhandler/wxhandler.py`

 * *Files identical despite different names*

### Comparing `wxhandler-0.1.1.1/wxhandler.egg-info/PKG-INFO` & `wxhandler-0.1.1.2/wxhandler.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhandler
-Version: 0.1.1.1
+Version: 0.1.1.2
 Summary: A Python package for handling wxHandler operations.
 Home-page: https://github.com/chenbifu/wxhandler
 Author: chenbifu
 Author-email: pythonaaa@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,11 +23,12 @@
 pip install wxhandler
 ```
 ## Usage
 ```python
 from wxhandler import wxHandler
 
 handler = wxHandler(base_url="http://127.0.0.1:19088")
-handler.hookSyncMsgNew(enableHttp=True, httpPort=19099)
+response = handler.hookSyncMsgNew(enableHttp=True, httpPort=19099)
+print(response)
 ```
```

