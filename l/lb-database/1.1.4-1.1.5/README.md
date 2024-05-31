# Comparing `tmp/lb_database-1.1.4.tar.gz` & `tmp/lb_database-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lb_database-1.1.4.tar", last modified: Fri May 31 02:42:42 2024, max compression
+gzip compressed data, was "lb_database-1.1.5.tar", last modified: Fri May 31 14:59:04 2024, max compression
```

## Comparing `lb_database-1.1.4.tar` & `lb_database-1.1.5.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:42:42.250594 lb_database-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-31 02:42:42.250594 lb_database-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-31 02:42:34.000000 lb_database-1.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:42:42.246594 lb_database-1.1.4/lbConnection/
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-31 02:42:34.000000 lb_database-1.1.4/lbConnection/LbConnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-31 02:42:34.000000 lb_database-1.1.4/lbConnection/Projection.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-31 02:42:34.000000 lb_database-1.1.4/lbConnection/Query.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 02:42:34.000000 lb_database-1.1.4/lbConnection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:42:42.246594 lb_database-1.1.4/lbUser/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-31 02:42:34.000000 lb_database-1.1.4/lbUser/AddressLbUser.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-31 02:42:34.000000 lb_database-1.1.4/lbUser/EnumStatusLbUser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-31 02:42:34.000000 lb_database-1.1.4/lbUser/LbUser.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-31 02:42:34.000000 lb_database-1.1.4/lbUser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 02:42:42.246594 lb_database-1.1.4/lb_database.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-31 02:42:42.000000 lb_database-1.1.4/lb_database.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-31 02:42:42.000000 lb_database-1.1.4/lb_database.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 02:42:42.000000 lb_database-1.1.4/lb_database.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-31 02:42:42.000000 lb_database-1.1.4/lb_database.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 02:42:42.250594 lb_database-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 02:42:34.000000 lb_database-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:59:04.514870 lb_database-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-31 14:59:04.514870 lb_database-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-31 14:58:57.000000 lb_database-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:59:04.510870 lb_database-1.1.5/lbConnection/
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-05-31 14:58:57.000000 lb_database-1.1.5/lbConnection/LbConnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-31 14:58:57.000000 lb_database-1.1.5/lbConnection/Projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-31 14:58:57.000000 lb_database-1.1.5/lbConnection/Query.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 14:58:57.000000 lb_database-1.1.5/lbConnection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:59:04.510870 lb_database-1.1.5/lbUser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-31 14:58:57.000000 lb_database-1.1.5/lbUser/AddressLbUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-31 14:58:57.000000 lb_database-1.1.5/lbUser/ConfirmationCodeLbUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-31 14:58:57.000000 lb_database-1.1.5/lbUser/EnumStatusLbUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-31 14:58:57.000000 lb_database-1.1.5/lbUser/LbUser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-31 14:58:57.000000 lb_database-1.1.5/lbUser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:59:04.514870 lb_database-1.1.5/lb_database.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-31 14:59:04.000000 lb_database-1.1.5/lb_database.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-31 14:59:04.000000 lb_database-1.1.5/lb_database.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:59:04.000000 lb_database-1.1.5/lb_database.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-31 14:59:04.000000 lb_database-1.1.5/lb_database.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:59:04.514870 lb_database-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 14:58:57.000000 lb_database-1.1.5/setup.py
```

### Comparing `lb_database-1.1.4/PKG-INFO` & `lb_database-1.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lb-database
-Version: 1.1.4
+Version: 1.1.5
 Summary: Library with data models by lb services
 Author: Lucas Barros
 Author-email: lucasbarros2000@hotmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lb_database-1.1.4/README.md` & `lb_database-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `lb_database-1.1.4/lbConnection/LbConnection.py` & `lb_database-1.1.5/lbConnection/LbConnection.py`

 * *Files identical despite different names*

### Comparing `lb_database-1.1.4/lbUser/AddressLbUser.py` & `lb_database-1.1.5/lbUser/AddressLbUser.py`

 * *Files identical despite different names*

### Comparing `lb_database-1.1.4/lbUser/LbUser.py` & `lb_database-1.1.5/lbUser/LbUser.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 __version__ = 1.0
 __maintainer__ = 'Lucas Barros'
 __email__ = 'lucasbarros2000@hotmail.com'
 __status__ = 'Production'
 
 
 from bson import ObjectId
+from lbUser.ConfirmationCodeLbUser import ConfirmationCodeLbUser
 from lbUser.EnumStatusLbUser import EnumStatusLbUser
 from lbUser.AddressLbUser import AddressLbUser
 from pydantic import BaseModel
 from pydantic import Field
 
 
 class LbUser(BaseModel):
@@ -72,11 +73,16 @@
     )
 
     digest: str = Field(
         description="Digest user at mongo database",
         default=None
     )
 
+    confirmation_code: ConfirmationCodeLbUser = Field(
+        description="Confirmation code user at mongo database",
+        default=None
+    )
+
     class Config:
         allow_population_by_field_name = True
         arbitrary_types_allowed = True
         json_encoders = {ObjectId: str}
```

### Comparing `lb_database-1.1.4/lb_database.egg-info/PKG-INFO` & `lb_database-1.1.5/lb_database.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lb-database
-Version: 1.1.4
+Version: 1.1.5
 Summary: Library with data models by lb services
 Author: Lucas Barros
 Author-email: lucasbarros2000@hotmail.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lb_database-1.1.4/setup.py` & `lb_database-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="lb-database",
-    version="1.1.4",
+    version="1.1.5",
     author="Lucas Barros",
     author_email="lucasbarros2000@hotmail.com",
     description="Library with data models by lb services",
     packages=setuptools.find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     classifiers=[
```

