# Comparing `tmp/abstract_factories-0.2.42.tar.gz` & `tmp/abstract_factories-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abstract_factories-0.2.42.tar", last modified: Wed May 29 22:02:38 2024, max compression
+gzip compressed data, was "abstract_factories-0.3.1.tar", last modified: Fri May 31 19:33:39 2024, max compression
```

## Comparing `abstract_factories-0.2.42.tar` & `abstract_factories-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:02:38.430235 abstract_factories-0.2.42/
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-29 22:02:38.430235 abstract_factories-0.2.42/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-29 22:02:34.000000 abstract_factories-0.2.42/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:02:38.430235 abstract_factories-0.2.42/abstract_factories/
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-29 22:02:34.000000 abstract_factories-0.2.42/abstract_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-29 22:02:34.000000 abstract_factories-0.2.42/abstract_factories/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-29 22:02:34.000000 abstract_factories-0.2.42/abstract_factories/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-29 22:02:34.000000 abstract_factories-0.2.42/abstract_factories/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:02:38.430235 abstract_factories-0.2.42/abstract_factories.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-29 22:02:38.000000 abstract_factories-0.2.42/abstract_factories.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-29 22:02:38.000000 abstract_factories-0.2.42/abstract_factories.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 22:02:38.000000 abstract_factories-0.2.42/abstract_factories.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 22:02:38.000000 abstract_factories-0.2.42/abstract_factories.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-29 22:02:38.430235 abstract_factories-0.2.42/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-29 22:02:34.000000 abstract_factories-0.2.42/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 22:02:38.430235 abstract_factories-0.2.42/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-29 22:02:34.000000 abstract_factories-0.2.42/tests/test_abstract_factories_items.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:33:39.690245 abstract_factories-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-31 19:33:39.690245 abstract_factories-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-31 19:33:33.000000 abstract_factories-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:33:39.690245 abstract_factories-0.3.1/abstract_factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-31 19:33:33.000000 abstract_factories-0.3.1/abstract_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-31 19:33:33.000000 abstract_factories-0.3.1/abstract_factories/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-05-31 19:33:33.000000 abstract_factories-0.3.1/abstract_factories/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-31 19:33:33.000000 abstract_factories-0.3.1/abstract_factories/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:33:39.690245 abstract_factories-0.3.1/abstract_factories.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-31 19:33:39.000000 abstract_factories-0.3.1/abstract_factories.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-31 19:33:39.000000 abstract_factories-0.3.1/abstract_factories.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:33:39.000000 abstract_factories-0.3.1/abstract_factories.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 19:33:39.000000 abstract_factories-0.3.1/abstract_factories.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-31 19:33:39.690245 abstract_factories-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-31 19:33:33.000000 abstract_factories-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:33:39.690245 abstract_factories-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-05-31 19:33:33.000000 abstract_factories-0.3.1/tests/test_abstract_factories_items.py
```

### Comparing `abstract_factories-0.2.42/PKG-INFO` & `abstract_factories-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_factories
-Version: 0.2.42
+Version: 0.3.1
 Summary: Abstract Factory design pattern classes for scalable data in dynamic environments.
 Home-page: https://github.com/ldunham1/abstract_factories
 Author: Lee Dunham
 Author-email: leedunham@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_factories-0.2.42/README.md` & `abstract_factories-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `abstract_factories-0.2.42/abstract_factories/__init__.py` & `abstract_factories-0.3.1/abstract_factories/__init__.py`

 * *Files identical despite different names*

### Comparing `abstract_factories-0.2.42/abstract_factories/core.py` & `abstract_factories-0.3.1/abstract_factories/core.py`

 * *Files identical despite different names*

### Comparing `abstract_factories-0.2.42/abstract_factories/utils.py` & `abstract_factories-0.3.1/abstract_factories/utils.py`

 * *Files identical despite different names*

### Comparing `abstract_factories-0.2.42/abstract_factories.egg-info/PKG-INFO` & `abstract_factories-0.3.1/abstract_factories.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abstract_factories
-Version: 0.2.42
+Version: 0.3.1
 Summary: Abstract Factory design pattern classes for scalable data in dynamic environments.
 Home-page: https://github.com/ldunham1/abstract_factories
 Author: Lee Dunham
 Author-email: leedunham@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `abstract_factories-0.2.42/setup.py` & `abstract_factories-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 
 setup(
     name='abstract_factories',
     packages=['abstract_factories'],
-    version='0.2.42',
+    version='0.3.1',
     license='MIT',
     description='Abstract Factory design pattern classes for scalable data in dynamic environments.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Lee Dunham',
     author_email='leedunham@gmail.com',
     url='https://github.com/ldunham1/abstract_factories',
```

### Comparing `abstract_factories-0.2.42/tests/test_abstract_factories_items.py` & `abstract_factories-0.3.1/tests/test_abstract_factories_items.py`

 * *Files identical despite different names*

