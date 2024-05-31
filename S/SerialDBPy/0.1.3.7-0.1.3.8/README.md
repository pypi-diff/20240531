# Comparing `tmp/SerialDBPy-0.1.3.7.tar.gz` & `tmp/SerialDBPy-0.1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SerialDBPy-0.1.3.7.tar", last modified: Fri May 31 04:14:25 2024, max compression
+gzip compressed data, was "SerialDBPy-0.1.3.8.tar", last modified: Fri May 31 04:17:11 2024, max compression
```

## Comparing `SerialDBPy-0.1.3.7.tar` & `SerialDBPy-0.1.3.8.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 04:14:25.657434 SerialDBPy-0.1.3.7/
--rw-rw-r--   0 swim      (1000) swim      (1000)     1069 2024-05-30 17:49:33.000000 SerialDBPy-0.1.3.7/LICENSE
--rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 04:14:25.657434 SerialDBPy-0.1.3.7/PKG-INFO
--rw-rw-r--   0 swim      (1000) swim      (1000)     3853 2024-05-31 03:40:11.000000 SerialDBPy-0.1.3.7/README.md
-drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 04:14:25.657434 SerialDBPy-0.1.3.7/SerialDBPy/
--rw-rw-r--   0 swim      (1000) swim      (1000)        0 2024-05-31 04:13:46.000000 SerialDBPy-0.1.3.7/SerialDBPy/__init__.py
--rw-rw-r--   0 swim      (1000) swim      (1000)     2049 2024-05-31 04:12:09.000000 SerialDBPy-0.1.3.7/SerialDBPy/query.py
--rw-rw-r--   0 swim      (1000) swim      (1000)    18361 2024-05-31 04:13:48.000000 SerialDBPy-0.1.3.7/SerialDBPy/serialization.py
-drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 04:14:25.657434 SerialDBPy-0.1.3.7/SerialDBPy.egg-info/
--rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 04:14:25.000000 SerialDBPy-0.1.3.7/SerialDBPy.egg-info/PKG-INFO
--rw-rw-r--   0 swim      (1000) swim      (1000)      243 2024-05-31 04:14:25.000000 SerialDBPy-0.1.3.7/SerialDBPy.egg-info/SOURCES.txt
--rw-rw-r--   0 swim      (1000) swim      (1000)        1 2024-05-31 04:14:25.000000 SerialDBPy-0.1.3.7/SerialDBPy.egg-info/dependency_links.txt
--rw-rw-r--   0 swim      (1000) swim      (1000)       11 2024-05-31 04:14:25.000000 SerialDBPy-0.1.3.7/SerialDBPy.egg-info/top_level.txt
--rw-rw-r--   0 swim      (1000) swim      (1000)       79 2024-05-31 04:14:25.657434 SerialDBPy-0.1.3.7/setup.cfg
--rw-rw-r--   0 swim      (1000) swim      (1000)      611 2024-05-31 04:14:02.000000 SerialDBPy-0.1.3.7/setup.py
+drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 04:17:11.077570 SerialDBPy-0.1.3.8/
+-rw-rw-r--   0 swim      (1000) swim      (1000)     1069 2024-05-30 17:49:33.000000 SerialDBPy-0.1.3.8/LICENSE
+-rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 04:17:11.077570 SerialDBPy-0.1.3.8/PKG-INFO
+-rw-rw-r--   0 swim      (1000) swim      (1000)     3853 2024-05-31 03:40:11.000000 SerialDBPy-0.1.3.8/README.md
+drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 04:17:11.077570 SerialDBPy-0.1.3.8/SerialDBPy/
+-rw-rw-r--   0 swim      (1000) swim      (1000)     2049 2024-05-31 04:12:09.000000 SerialDBPy-0.1.3.8/SerialDBPy/query.py
+-rw-rw-r--   0 swim      (1000) swim      (1000)    18361 2024-05-31 04:13:48.000000 SerialDBPy-0.1.3.8/SerialDBPy/serialization.py
+drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 04:17:11.077570 SerialDBPy-0.1.3.8/SerialDBPy.egg-info/
+-rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 04:17:11.000000 SerialDBPy-0.1.3.8/SerialDBPy.egg-info/PKG-INFO
+-rw-rw-r--   0 swim      (1000) swim      (1000)      220 2024-05-31 04:17:11.000000 SerialDBPy-0.1.3.8/SerialDBPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 swim      (1000) swim      (1000)        1 2024-05-31 04:17:11.000000 SerialDBPy-0.1.3.8/SerialDBPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 swim      (1000) swim      (1000)        1 2024-05-31 04:17:11.000000 SerialDBPy-0.1.3.8/SerialDBPy.egg-info/top_level.txt
+-rw-rw-r--   0 swim      (1000) swim      (1000)       79 2024-05-31 04:17:11.077570 SerialDBPy-0.1.3.8/setup.cfg
+-rw-rw-r--   0 swim      (1000) swim      (1000)      611 2024-05-31 04:17:07.000000 SerialDBPy-0.1.3.8/setup.py
```

### Comparing `SerialDBPy-0.1.3.7/LICENSE` & `SerialDBPy-0.1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.3.7/PKG-INFO` & `SerialDBPy-0.1.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: SerialDBPy
-Version: 0.1.3.7
+Version: 0.1.3.8
 Summary: Lightweight Python ORM for basic CRUD operations.
 Home-page: https://github.com/publicsignal
 Author: G
 Author-email: serialdbpy@swimhdr.com
 License: MIT
-Download-URL: https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.3.7.tar.gz
+Download-URL: https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.3.8.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `SerialDBPy-0.1.3.7/README.md` & `SerialDBPy-0.1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.3.7/SerialDBPy/query.py` & `SerialDBPy-0.1.3.8/SerialDBPy/query.py`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.3.7/SerialDBPy/serialization.py` & `SerialDBPy-0.1.3.8/SerialDBPy/serialization.py`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.3.7/SerialDBPy.egg-info/PKG-INFO` & `SerialDBPy-0.1.3.8/SerialDBPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: SerialDBPy
-Version: 0.1.3.7
+Version: 0.1.3.8
 Summary: Lightweight Python ORM for basic CRUD operations.
 Home-page: https://github.com/publicsignal
 Author: G
 Author-email: serialdbpy@swimhdr.com
 License: MIT
-Download-URL: https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.3.7.tar.gz
+Download-URL: https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.3.8.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `SerialDBPy-0.1.3.7/setup.py` & `SerialDBPy-0.1.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='SerialDBPy',
-    version='0.1.3.7',
+    version='0.1.3.8',
     author='G',
     author_email='serialdbpy@swimhdr.com',
     description='Lightweight Python ORM for basic CRUD operations.',
     license='MIT',
     url = 'https://github.com/publicsignal',
-    download_url='https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.3.7.tar.gz',
+    download_url='https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.3.8.tar.gz',
     packages=find_packages(),
     classifiers=[
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     ],
     python_requires='>=3.10',
```

