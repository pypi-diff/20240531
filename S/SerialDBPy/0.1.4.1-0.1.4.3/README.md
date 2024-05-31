# Comparing `tmp/SerialDBPy-0.1.4.1.tar.gz` & `tmp/SerialDBPy-0.1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SerialDBPy-0.1.4.1.tar", last modified: Fri May 31 17:31:56 2024, max compression
+gzip compressed data, was "SerialDBPy-0.1.4.3.tar", last modified: Fri May 31 20:24:32 2024, max compression
```

## Comparing `SerialDBPy-0.1.4.1.tar` & `SerialDBPy-0.1.4.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 17:31:56.211452 SerialDBPy-0.1.4.1/
--rw-rw-r--   0 swim      (1000) swim      (1000)     1069 2024-05-30 17:49:33.000000 SerialDBPy-0.1.4.1/LICENSE
--rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 17:31:56.211452 SerialDBPy-0.1.4.1/PKG-INFO
--rw-rw-r--   0 swim      (1000) swim      (1000)     3853 2024-05-31 03:40:11.000000 SerialDBPy-0.1.4.1/README.md
-drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 17:31:56.211452 SerialDBPy-0.1.4.1/SerialDBPy.egg-info/
--rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 17:31:56.000000 SerialDBPy-0.1.4.1/SerialDBPy.egg-info/PKG-INFO
--rw-rw-r--   0 swim      (1000) swim      (1000)      252 2024-05-31 17:31:56.000000 SerialDBPy-0.1.4.1/SerialDBPy.egg-info/SOURCES.txt
--rw-rw-r--   0 swim      (1000) swim      (1000)        1 2024-05-31 17:31:56.000000 SerialDBPy-0.1.4.1/SerialDBPy.egg-info/dependency_links.txt
--rw-rw-r--   0 swim      (1000) swim      (1000)       14 2024-05-31 17:31:56.000000 SerialDBPy-0.1.4.1/SerialDBPy.egg-info/top_level.txt
-drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 17:31:56.211452 SerialDBPy-0.1.4.1/Serialization/
--rw-rw-r--   0 swim      (1000) swim      (1000)       91 2024-05-31 17:26:33.000000 SerialDBPy-0.1.4.1/Serialization/__init__.py
--rw-rw-r--   0 swim      (1000) swim      (1000)     2049 2024-05-31 04:22:30.000000 SerialDBPy-0.1.4.1/Serialization/query.py
--rw-rw-r--   0 swim      (1000) swim      (1000)    18426 2024-05-31 17:31:35.000000 SerialDBPy-0.1.4.1/Serialization/serialization.py
--rw-rw-r--   0 swim      (1000) swim      (1000)       79 2024-05-31 17:31:56.211452 SerialDBPy-0.1.4.1/setup.cfg
--rw-rw-r--   0 swim      (1000) swim      (1000)      611 2024-05-31 17:31:43.000000 SerialDBPy-0.1.4.1/setup.py
+drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 20:24:32.981536 SerialDBPy-0.1.4.3/
+-rw-rw-r--   0 swim      (1000) swim      (1000)     1069 2024-05-30 17:49:33.000000 SerialDBPy-0.1.4.3/LICENSE
+-rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 20:24:32.981536 SerialDBPy-0.1.4.3/PKG-INFO
+-rw-rw-r--   0 swim      (1000) swim      (1000)     3853 2024-05-31 03:40:11.000000 SerialDBPy-0.1.4.3/README.md
+drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 20:24:32.981536 SerialDBPy-0.1.4.3/SerialDBPy.egg-info/
+-rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 20:24:32.000000 SerialDBPy-0.1.4.3/SerialDBPy.egg-info/PKG-INFO
+-rw-rw-r--   0 swim      (1000) swim      (1000)      252 2024-05-31 20:24:32.000000 SerialDBPy-0.1.4.3/SerialDBPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 swim      (1000) swim      (1000)        1 2024-05-31 20:24:32.000000 SerialDBPy-0.1.4.3/SerialDBPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 swim      (1000) swim      (1000)       14 2024-05-31 20:24:32.000000 SerialDBPy-0.1.4.3/SerialDBPy.egg-info/top_level.txt
+drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 20:24:32.981536 SerialDBPy-0.1.4.3/Serialization/
+-rw-rw-r--   0 swim      (1000) swim      (1000)       91 2024-05-31 17:26:33.000000 SerialDBPy-0.1.4.3/Serialization/__init__.py
+-rw-rw-r--   0 swim      (1000) swim      (1000)     2049 2024-05-31 04:22:30.000000 SerialDBPy-0.1.4.3/Serialization/query.py
+-rw-rw-r--   0 swim      (1000) swim      (1000)    18426 2024-05-31 17:31:35.000000 SerialDBPy-0.1.4.3/Serialization/serialization.py
+-rw-rw-r--   0 swim      (1000) swim      (1000)       79 2024-05-31 20:24:32.981536 SerialDBPy-0.1.4.3/setup.cfg
+-rw-rw-r--   0 swim      (1000) swim      (1000)      611 2024-05-31 20:24:19.000000 SerialDBPy-0.1.4.3/setup.py
```

### Comparing `SerialDBPy-0.1.4.1/LICENSE` & `SerialDBPy-0.1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.4.1/PKG-INFO` & `SerialDBPy-0.1.4.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: SerialDBPy
-Version: 0.1.4.1
+Version: 0.1.4.3
 Summary: Lightweight Python ORM for basic CRUD operations.
 Home-page: https://github.com/publicsignal
 Author: G
 Author-email: serialdbpy@swimhdr.com
 License: MIT
-Download-URL: https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.4.1.tar.gz
+Download-URL: https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.4.3.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `SerialDBPy-0.1.4.1/README.md` & `SerialDBPy-0.1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.4.1/SerialDBPy.egg-info/PKG-INFO` & `SerialDBPy-0.1.4.3/SerialDBPy.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: SerialDBPy
-Version: 0.1.4.1
+Version: 0.1.4.3
 Summary: Lightweight Python ORM for basic CRUD operations.
 Home-page: https://github.com/publicsignal
 Author: G
 Author-email: serialdbpy@swimhdr.com
 License: MIT
-Download-URL: https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.4.1.tar.gz
+Download-URL: https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.4.3.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `SerialDBPy-0.1.4.1/Serialization/query.py` & `SerialDBPy-0.1.4.3/Serialization/query.py`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.4.1/Serialization/serialization.py` & `SerialDBPy-0.1.4.3/Serialization/serialization.py`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.4.1/setup.py` & `SerialDBPy-0.1.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SerialDBPy',
-    version='0.1.4.1',
+    version='0.1.4.3',
     author='G',
     author_email='serialdbpy@swimhdr.com',
     description='Lightweight Python ORM for basic CRUD operations.',
     license='MIT',
     url = 'https://github.com/publicsignal',
-    download_url='https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.4.1.tar.gz',
+    download_url='https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.4.3.tar.gz',
     packages=find_packages(),
     classifiers=[
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     ],
     python_requires='>=3.10',
```

