# Comparing `tmp/SerialDBPy-0.1.3.2.tar.gz` & `tmp/SerialDBPy-0.1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SerialDBPy-0.1.3.2.tar", last modified: Fri May 31 02:22:54 2024, max compression
+gzip compressed data, was "SerialDBPy-0.1.3.3.tar", last modified: Fri May 31 02:27:53 2024, max compression
```

## Comparing `SerialDBPy-0.1.3.2.tar` & `SerialDBPy-0.1.3.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 02:22:54.077071 SerialDBPy-0.1.3.2/
--rw-rw-r--   0 swim      (1000) swim      (1000)     1069 2024-05-30 17:49:33.000000 SerialDBPy-0.1.3.2/LICENSE
--rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 02:22:54.077071 SerialDBPy-0.1.3.2/PKG-INFO
--rw-rw-r--   0 swim      (1000) swim      (1000)     3833 2024-05-30 18:34:21.000000 SerialDBPy-0.1.3.2/README.md
-drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 02:22:54.077071 SerialDBPy-0.1.3.2/SerialDBPy/
--rw-rw-r--   0 swim      (1000) swim      (1000)       61 2024-05-30 17:56:44.000000 SerialDBPy-0.1.3.2/SerialDBPy/__init__.py
--rw-rw-r--   0 swim      (1000) swim      (1000)     2049 2024-05-31 02:18:30.000000 SerialDBPy-0.1.3.2/SerialDBPy/query.py
--rw-rw-r--   0 swim      (1000) swim      (1000)    18356 2024-05-31 02:18:13.000000 SerialDBPy-0.1.3.2/SerialDBPy/serialization.py
-drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 02:22:54.077071 SerialDBPy-0.1.3.2/SerialDBPy.egg-info/
--rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 02:22:54.000000 SerialDBPy-0.1.3.2/SerialDBPy.egg-info/PKG-INFO
--rw-rw-r--   0 swim      (1000) swim      (1000)      243 2024-05-31 02:22:54.000000 SerialDBPy-0.1.3.2/SerialDBPy.egg-info/SOURCES.txt
--rw-rw-r--   0 swim      (1000) swim      (1000)        1 2024-05-31 02:22:54.000000 SerialDBPy-0.1.3.2/SerialDBPy.egg-info/dependency_links.txt
--rw-rw-r--   0 swim      (1000) swim      (1000)       11 2024-05-31 02:22:54.000000 SerialDBPy-0.1.3.2/SerialDBPy.egg-info/top_level.txt
--rw-rw-r--   0 swim      (1000) swim      (1000)       79 2024-05-31 02:22:54.077071 SerialDBPy-0.1.3.2/setup.cfg
--rw-rw-r--   0 swim      (1000) swim      (1000)      610 2024-05-31 02:21:32.000000 SerialDBPy-0.1.3.2/setup.py
+drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 02:27:53.335299 SerialDBPy-0.1.3.3/
+-rw-rw-r--   0 swim      (1000) swim      (1000)     1069 2024-05-30 17:49:33.000000 SerialDBPy-0.1.3.3/LICENSE
+-rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 02:27:53.335299 SerialDBPy-0.1.3.3/PKG-INFO
+-rw-rw-r--   0 swim      (1000) swim      (1000)     3833 2024-05-30 18:34:21.000000 SerialDBPy-0.1.3.3/README.md
+drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 02:27:53.335299 SerialDBPy-0.1.3.3/SerialDBPy/
+-rw-rw-r--   0 swim      (1000) swim      (1000)       83 2024-05-31 02:25:48.000000 SerialDBPy-0.1.3.3/SerialDBPy/__init__.py
+-rw-rw-r--   0 swim      (1000) swim      (1000)     2049 2024-05-31 02:18:30.000000 SerialDBPy-0.1.3.3/SerialDBPy/query.py
+-rw-rw-r--   0 swim      (1000) swim      (1000)    18356 2024-05-31 02:18:13.000000 SerialDBPy-0.1.3.3/SerialDBPy/serialization.py
+drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 02:27:53.335299 SerialDBPy-0.1.3.3/SerialDBPy.egg-info/
+-rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 02:27:53.000000 SerialDBPy-0.1.3.3/SerialDBPy.egg-info/PKG-INFO
+-rw-rw-r--   0 swim      (1000) swim      (1000)      243 2024-05-31 02:27:53.000000 SerialDBPy-0.1.3.3/SerialDBPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 swim      (1000) swim      (1000)        1 2024-05-31 02:27:53.000000 SerialDBPy-0.1.3.3/SerialDBPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 swim      (1000) swim      (1000)       11 2024-05-31 02:27:53.000000 SerialDBPy-0.1.3.3/SerialDBPy.egg-info/top_level.txt
+-rw-rw-r--   0 swim      (1000) swim      (1000)       79 2024-05-31 02:27:53.335299 SerialDBPy-0.1.3.3/setup.cfg
+-rw-rw-r--   0 swim      (1000) swim      (1000)      610 2024-05-31 02:26:28.000000 SerialDBPy-0.1.3.3/setup.py
```

### Comparing `SerialDBPy-0.1.3.2/LICENSE` & `SerialDBPy-0.1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.3.2/PKG-INFO` & `SerialDBPy-0.1.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: SerialDBPy
-Version: 0.1.3.2
+Version: 0.1.3.3
 Summary: Lightweight Python ORM for basic CRUD operations.
 Home-page: https://github.com/publicsignal
 Author: G
 Author-email: serialdbpy@swimhdr.com
 License: MIT
-Download-URL: https://github.com/publicsignal/SerialDBPy/blob/main/dist/SerialDBPy-0.1.3.2.tar.gz
+Download-URL: https://github.com/publicsignal/SerialDBPy/blob/main/dist/SerialDBPy-0.1.3.3.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `SerialDBPy-0.1.3.2/README.md` & `SerialDBPy-0.1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.3.2/SerialDBPy/query.py` & `SerialDBPy-0.1.3.3/SerialDBPy/query.py`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.3.2/SerialDBPy/serialization.py` & `SerialDBPy-0.1.3.3/SerialDBPy/serialization.py`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.3.2/SerialDBPy.egg-info/PKG-INFO` & `SerialDBPy-0.1.3.3/SerialDBPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: SerialDBPy
-Version: 0.1.3.2
+Version: 0.1.3.3
 Summary: Lightweight Python ORM for basic CRUD operations.
 Home-page: https://github.com/publicsignal
 Author: G
 Author-email: serialdbpy@swimhdr.com
 License: MIT
-Download-URL: https://github.com/publicsignal/SerialDBPy/blob/main/dist/SerialDBPy-0.1.3.2.tar.gz
+Download-URL: https://github.com/publicsignal/SerialDBPy/blob/main/dist/SerialDBPy-0.1.3.3.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `SerialDBPy-0.1.3.2/setup.py` & `SerialDBPy-0.1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 setup(
     name='SerialDBPy',
-    version='0.1.3.2',
+    version='0.1.3.3',
     author='G',
     author_email='serialdbpy@swimhdr.com',
     description='Lightweight Python ORM for basic CRUD operations.',
     license='MIT',
     url = 'https://github.com/publicsignal',
-    download_url='https://github.com/publicsignal/SerialDBPy/blob/main/dist/SerialDBPy-0.1.3.2.tar.gz',
+    download_url='https://github.com/publicsignal/SerialDBPy/blob/main/dist/SerialDBPy-0.1.3.3.tar.gz',
     packages=find_packages(),
     classifiers=[
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     ],
     python_requires='>=3.10',
```

