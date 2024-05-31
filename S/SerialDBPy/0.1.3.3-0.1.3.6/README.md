# Comparing `tmp/SerialDBPy-0.1.3.3.tar.gz` & `tmp/SerialDBPy-0.1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SerialDBPy-0.1.3.3.tar", last modified: Fri May 31 02:27:53 2024, max compression
+gzip compressed data, was "SerialDBPy-0.1.3.6.tar", last modified: Fri May 31 03:49:44 2024, max compression
```

## Comparing `SerialDBPy-0.1.3.3.tar` & `SerialDBPy-0.1.3.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 02:27:53.335299 SerialDBPy-0.1.3.3/
--rw-rw-r--   0 swim      (1000) swim      (1000)     1069 2024-05-30 17:49:33.000000 SerialDBPy-0.1.3.3/LICENSE
--rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 02:27:53.335299 SerialDBPy-0.1.3.3/PKG-INFO
--rw-rw-r--   0 swim      (1000) swim      (1000)     3833 2024-05-30 18:34:21.000000 SerialDBPy-0.1.3.3/README.md
-drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 02:27:53.335299 SerialDBPy-0.1.3.3/SerialDBPy/
--rw-rw-r--   0 swim      (1000) swim      (1000)       83 2024-05-31 02:25:48.000000 SerialDBPy-0.1.3.3/SerialDBPy/__init__.py
--rw-rw-r--   0 swim      (1000) swim      (1000)     2049 2024-05-31 02:18:30.000000 SerialDBPy-0.1.3.3/SerialDBPy/query.py
--rw-rw-r--   0 swim      (1000) swim      (1000)    18356 2024-05-31 02:18:13.000000 SerialDBPy-0.1.3.3/SerialDBPy/serialization.py
-drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 02:27:53.335299 SerialDBPy-0.1.3.3/SerialDBPy.egg-info/
--rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 02:27:53.000000 SerialDBPy-0.1.3.3/SerialDBPy.egg-info/PKG-INFO
--rw-rw-r--   0 swim      (1000) swim      (1000)      243 2024-05-31 02:27:53.000000 SerialDBPy-0.1.3.3/SerialDBPy.egg-info/SOURCES.txt
--rw-rw-r--   0 swim      (1000) swim      (1000)        1 2024-05-31 02:27:53.000000 SerialDBPy-0.1.3.3/SerialDBPy.egg-info/dependency_links.txt
--rw-rw-r--   0 swim      (1000) swim      (1000)       11 2024-05-31 02:27:53.000000 SerialDBPy-0.1.3.3/SerialDBPy.egg-info/top_level.txt
--rw-rw-r--   0 swim      (1000) swim      (1000)       79 2024-05-31 02:27:53.335299 SerialDBPy-0.1.3.3/setup.cfg
--rw-rw-r--   0 swim      (1000) swim      (1000)      610 2024-05-31 02:26:28.000000 SerialDBPy-0.1.3.3/setup.py
+drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 03:49:44.464355 SerialDBPy-0.1.3.6/
+-rw-rw-r--   0 swim      (1000) swim      (1000)     1069 2024-05-30 17:49:33.000000 SerialDBPy-0.1.3.6/LICENSE
+-rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 03:49:44.464355 SerialDBPy-0.1.3.6/PKG-INFO
+-rw-rw-r--   0 swim      (1000) swim      (1000)     3853 2024-05-31 03:40:11.000000 SerialDBPy-0.1.3.6/README.md
+drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 03:49:44.464355 SerialDBPy-0.1.3.6/SerialDBPy/
+-rw-rw-r--   0 swim      (1000) swim      (1000)       36 2024-05-31 03:49:18.000000 SerialDBPy-0.1.3.6/SerialDBPy/__init__.py
+-rw-rw-r--   0 swim      (1000) swim      (1000)     2049 2024-05-31 02:18:30.000000 SerialDBPy-0.1.3.6/SerialDBPy/query.py
+-rw-rw-r--   0 swim      (1000) swim      (1000)    18356 2024-05-31 02:18:13.000000 SerialDBPy-0.1.3.6/SerialDBPy/serialization.py
+drwxrwxr-x   0 swim      (1000) swim      (1000)        0 2024-05-31 03:49:44.464355 SerialDBPy-0.1.3.6/SerialDBPy.egg-info/
+-rw-rw-r--   0 swim      (1000) swim      (1000)      536 2024-05-31 03:49:44.000000 SerialDBPy-0.1.3.6/SerialDBPy.egg-info/PKG-INFO
+-rw-rw-r--   0 swim      (1000) swim      (1000)      243 2024-05-31 03:49:44.000000 SerialDBPy-0.1.3.6/SerialDBPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 swim      (1000) swim      (1000)        1 2024-05-31 03:49:44.000000 SerialDBPy-0.1.3.6/SerialDBPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 swim      (1000) swim      (1000)       11 2024-05-31 03:49:44.000000 SerialDBPy-0.1.3.6/SerialDBPy.egg-info/top_level.txt
+-rw-rw-r--   0 swim      (1000) swim      (1000)       79 2024-05-31 03:49:44.464355 SerialDBPy-0.1.3.6/setup.cfg
+-rw-rw-r--   0 swim      (1000) swim      (1000)      611 2024-05-31 03:49:36.000000 SerialDBPy-0.1.3.6/setup.py
```

### Comparing `SerialDBPy-0.1.3.3/LICENSE` & `SerialDBPy-0.1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.3.3/PKG-INFO` & `SerialDBPy-0.1.3.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: SerialDBPy
-Version: 0.1.3.3
+Version: 0.1.3.6
 Summary: Lightweight Python ORM for basic CRUD operations.
 Home-page: https://github.com/publicsignal
 Author: G
 Author-email: serialdbpy@swimhdr.com
 License: MIT
-Download-URL: https://github.com/publicsignal/SerialDBPy/blob/main/dist/SerialDBPy-0.1.3.3.tar.gz
+Download-URL: https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.3.6.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `SerialDBPy-0.1.3.3/README.md` & `SerialDBPy-0.1.3.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 - SQL injection prevention through query sanitization
 - Flexible configuration through environment variables
 
 ## Usage
 # Basic Usage
 To use SerialDBPy, simply inherit it in your class and call the relevant methods for serialization and deserialization.
 
-```sh
+```python
 from serialdbpy import SerialDBPy
 
 os.environ['default_server'] = 'server_containing_databases'
 os.environ['default_middleware'] = 'default_schema' # Example: SELECT TOP 100 * FROM [db_name].[default_schema].[table];
 os.environ['SerialDBPy_ACCOUNT'] = 'SNOWFLAKE_ACCOUNT'
 os.environ['SerialDBPy_PSWD'] = 'SNOWFLAKE_ACCOUNT_PSWD'
 os.environ['SerialDBPy_user'] = 'SNOWFLAKE_USER'
@@ -41,42 +41,42 @@
         
         self.id = None
         self.name = name
         self.age = age
         self.height = height
 ```
 
-```sh
+```python
 # Create and insert a new person
 person = Person(name="John Doe", age=30, height=200)
 person.id = person._uuid()
 person.insert()
 
 # Updates the person's row in our DB
 person.name = 'Jane Doe'
 person.age = 27
 person.height = 150
 person.update()
 
 # Converts the instance of Person into JSON format
 print( person.serialize_to_json() )
 ```
-```sh
+```python
 # Retrieve a person from the database
 # Gets John Doe from our database (I always recommend getting by the Primary Key, but either way works)
 # the kwargs on a .get() are akin to a SQL where clause
 person = Person()
 person.get(name="John Doe") 
 ```
-```sh
+```python
 # Deletes a person from the database
 person = Person().get(name="John Doe", age=30, height=200)
 person.delete()
 ```
-```sh
+```python
 # Truncates the table associated with the Person class
 Person.truncate()
 ```
 # Configuration
 ## SerialDBPy allows configuration through environment variables:
 
 - IGNORE_UNDERSCORE_VARS: Ignore variables starting with an underscore (default: True)
```

### Comparing `SerialDBPy-0.1.3.3/SerialDBPy/query.py` & `SerialDBPy-0.1.3.6/SerialDBPy/query.py`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.3.3/SerialDBPy/serialization.py` & `SerialDBPy-0.1.3.6/SerialDBPy/serialization.py`

 * *Files identical despite different names*

### Comparing `SerialDBPy-0.1.3.3/SerialDBPy.egg-info/PKG-INFO` & `SerialDBPy-0.1.3.6/SerialDBPy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: SerialDBPy
-Version: 0.1.3.3
+Version: 0.1.3.6
 Summary: Lightweight Python ORM for basic CRUD operations.
 Home-page: https://github.com/publicsignal
 Author: G
 Author-email: serialdbpy@swimhdr.com
 License: MIT
-Download-URL: https://github.com/publicsignal/SerialDBPy/blob/main/dist/SerialDBPy-0.1.3.3.tar.gz
+Download-URL: https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.3.6.tar.gz
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `SerialDBPy-0.1.3.3/setup.py` & `SerialDBPy-0.1.3.6/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import setup, find_packages
+
 setup(
     name='SerialDBPy',
-    version='0.1.3.3',
+    version='0.1.3.6',
     author='G',
     author_email='serialdbpy@swimhdr.com',
     description='Lightweight Python ORM for basic CRUD operations.',
     license='MIT',
     url = 'https://github.com/publicsignal',
-    download_url='https://github.com/publicsignal/SerialDBPy/blob/main/dist/SerialDBPy-0.1.3.3.tar.gz',
+    download_url='https://github.com/publicsignal/SerialDBPy/tree/main/dist/SerialDBPy-0.1.3.6.tar.gz',
     packages=find_packages(),
     classifiers=[
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     ],
     python_requires='>=3.10',
```

