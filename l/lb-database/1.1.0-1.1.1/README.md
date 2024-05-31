# Comparing `tmp/lb_database-1.1.0.tar.gz` & `tmp/lb_database-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lb_database-1.1.0.tar", last modified: Fri May 31 01:42:09 2024, max compression
+gzip compressed data, was "lb_database-1.1.1.tar", last modified: Fri May 31 02:07:31 2024, max compression
```

## Comparing `lb_database-1.1.0.tar` & `lb_database-1.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:42:09.714917 lb_database-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-31 01:42:09.714917 lb_database-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-31 01:42:01.000000 lb_database-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:42:09.714917 lb_database-1.1.0/lbConnection/
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-31 01:42:01.000000 lb_database-1.1.0/lbConnection/LbConnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-31 01:42:01.000000 lb_database-1.1.0/lbConnection/Projection.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-31 01:42:01.000000 lb_database-1.1.0/lbConnection/Query.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 01:42:01.000000 lb_database-1.1.0/lbConnection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:42:09.714917 lb_database-1.1.0/lbUser/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-31 01:42:01.000000 lb_database-1.1.0/lbUser/AddressLbUser.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-31 01:42:01.000000 lb_database-1.1.0/lbUser/EnumStatusLbUser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-31 01:42:01.000000 lb_database-1.1.0/lbUser/LbUser.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-31 01:42:01.000000 lb_database-1.1.0/lbUser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:42:09.714917 lb_database-1.1.0/lb_database.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-31 01:42:09.000000 lb_database-1.1.0/lb_database.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-31 01:42:09.000000 lb_database-1.1.0/lb_database.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 01:42:09.000000 lb_database-1.1.0/lb_database.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-31 01:42:09.000000 lb_database-1.1.0/lb_database.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 01:42:09.714917 lb_database-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 01:42:01.000000 lb_database-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:07:31.992848 lb_database-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-31 02:07:31.992848 lb_database-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-31 02:07:16.000000 lb_database-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:07:31.988848 lb_database-1.1.1/lbConnection/
+-rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-05-31 02:07:16.000000 lb_database-1.1.1/lbConnection/LbConnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-31 02:07:16.000000 lb_database-1.1.1/lbConnection/Projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-31 02:07:16.000000 lb_database-1.1.1/lbConnection/Query.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 02:07:16.000000 lb_database-1.1.1/lbConnection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:07:31.988848 lb_database-1.1.1/lbUser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-31 02:07:16.000000 lb_database-1.1.1/lbUser/AddressLbUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-31 02:07:16.000000 lb_database-1.1.1/lbUser/EnumStatusLbUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-31 02:07:16.000000 lb_database-1.1.1/lbUser/LbUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-31 02:07:16.000000 lb_database-1.1.1/lbUser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:07:31.992848 lb_database-1.1.1/lb_database.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-31 02:07:31.000000 lb_database-1.1.1/lb_database.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-31 02:07:31.000000 lb_database-1.1.1/lb_database.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 02:07:31.000000 lb_database-1.1.1/lb_database.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-31 02:07:31.000000 lb_database-1.1.1/lb_database.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 02:07:31.992848 lb_database-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 02:07:16.000000 lb_database-1.1.1/setup.py
```

### Comparing `lb_database-1.1.0/PKG-INFO` & `lb_database-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lb-database
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library with data models by lb services
 Author: Lucas Barros
 Author-email: lucasbarros2000@hotmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lb_database-1.1.0/README.md` & `lb_database-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `lb_database-1.1.0/lbConnection/LbConnection.py` & `lb_database-1.1.1/lbConnection/LbConnection.py`

 * *Files identical despite different names*

### Comparing `lb_database-1.1.0/lbUser/AddressLbUser.py` & `lb_database-1.1.1/lbUser/AddressLbUser.py`

 * *Files identical despite different names*

### Comparing `lb_database-1.1.0/lbUser/LbUser.py` & `lb_database-1.1.1/lbUser/LbUser.py`

 * *Files identical despite different names*

### Comparing `lb_database-1.1.0/lb_database.egg-info/PKG-INFO` & `lb_database-1.1.1/lb_database.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lb-database
-Version: 1.1.0
+Version: 1.1.1
 Summary: Library with data models by lb services
 Author: Lucas Barros
 Author-email: lucasbarros2000@hotmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lb_database-1.1.0/setup.py` & `lb_database-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="lb-database",
-    version="1.1.0",
+    version="1.1.1",
     author="Lucas Barros",
     author_email="lucasbarros2000@hotmail.com",
     description="Library with data models by lb services",
     packages=setuptools.find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     classifiers=[
```

