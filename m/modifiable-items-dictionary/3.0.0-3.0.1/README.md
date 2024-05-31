# Comparing `tmp/modifiable_items_dictionary-3.0.0.tar.gz` & `tmp/modifiable_items_dictionary-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modifiable_items_dictionary-3.0.0.tar", last modified: Thu May 23 19:09:28 2024, max compression
+gzip compressed data, was "modifiable_items_dictionary-3.0.1.tar", last modified: Fri May 31 15:53:34 2024, max compression
```

## Comparing `modifiable_items_dictionary-3.0.0.tar` & `modifiable_items_dictionary-3.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:09:28.951298 modifiable_items_dictionary-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-05-23 19:09:28.951298 modifiable_items_dictionary-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:09:28.947297 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary/modifiable_items_attribute_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)     9405 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary/modifiable_items_dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:09:28.951298 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-05-23 19:09:28.000000 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-23 19:09:28.000000 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:09:28.000000 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 19:09:28.000000 modifiable_items_dictionary-3.0.0/modifiable_items_dictionary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:09:28.951298 modifiable_items_dictionary-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:09:28.951298 modifiable_items_dictionary-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/tests/test_modifiable_items_attr_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    18550 2024-05-23 19:09:25.000000 modifiable_items_dictionary-3.0.0/tests/test_modifiable_items_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:53:34.767575 modifiable_items_dictionary-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 15:53:31.000000 modifiable_items_dictionary-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-05-31 15:53:34.767575 modifiable_items_dictionary-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9222 2024-05-31 15:53:31.000000 modifiable_items_dictionary-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:53:34.767575 modifiable_items_dictionary-3.0.1/modifiable_items_dictionary/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-31 15:53:31.000000 modifiable_items_dictionary-3.0.1/modifiable_items_dictionary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-31 15:53:31.000000 modifiable_items_dictionary-3.0.1/modifiable_items_dictionary/modifiable_items_attribute_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9405 2024-05-31 15:53:31.000000 modifiable_items_dictionary-3.0.1/modifiable_items_dictionary/modifiable_items_dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:53:34.767575 modifiable_items_dictionary-3.0.1/modifiable_items_dictionary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10355 2024-05-31 15:53:34.000000 modifiable_items_dictionary-3.0.1/modifiable_items_dictionary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-31 15:53:34.000000 modifiable_items_dictionary-3.0.1/modifiable_items_dictionary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:53:34.000000 modifiable_items_dictionary-3.0.1/modifiable_items_dictionary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 15:53:34.000000 modifiable_items_dictionary-3.0.1/modifiable_items_dictionary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:53:34.767575 modifiable_items_dictionary-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-31 15:53:31.000000 modifiable_items_dictionary-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:53:34.767575 modifiable_items_dictionary-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-31 15:53:31.000000 modifiable_items_dictionary-3.0.1/tests/test_modifiable_items_attr_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18550 2024-05-31 15:53:31.000000 modifiable_items_dictionary-3.0.1/tests/test_modifiable_items_dict.py
```

### Comparing `modifiable_items_dictionary-3.0.0/LICENSE` & `modifiable_items_dictionary-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modifiable_items_dictionary-3.0.0/PKG-INFO` & `modifiable_items_dictionary-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modifiable-items-dictionary
-Version: 3.0.0
+Version: 3.0.1
 Summary: Typed and Tested Modifiable Items Dict and ModifiableItemsAttrDict which allow keys and values to be modified at run time. ModifiableItemsAttrDict additionally provides attribute-style access to dictionary items.
 Home-page: https://github.com/tybruno/modifiable-items-dictionary
 Author: Tyler Bruno
 License: MIT
 Keywords: python dict attribute dictionary attrdict mapping key-mangling value-mangling
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `modifiable_items_dictionary-3.0.0/README.md` & `modifiable_items_dictionary-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `modifiable_items_dictionary-3.0.0/modifiable_items_dictionary/modifiable_items_attribute_dictionary.py` & `modifiable_items_dictionary-3.0.1/modifiable_items_dictionary/modifiable_items_attribute_dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     Dictionary class that allows attribute-style access to its items.
 
     This class extends `ModifiableItemsDict` and overrides the `__getattr__`
     and `__setattr__` methods to provide attribute-style access to dictionary
     items. This means that in addition to the standard dictionary access
     syntax (dict["key"]), you can also use attribute syntax (dict.key).
     """
+    __slots__ = ()
 
     def __getattr__(self, name: str) -> Any:
         """
         Return the value for a given attribute name.
 
         This method is called when an attribute lookup has not found the
         attribute in the usual places. It's overridden here to look for the
```

### Comparing `modifiable_items_dictionary-3.0.0/modifiable_items_dictionary/modifiable_items_dictionary.py` & `modifiable_items_dictionary-3.0.1/modifiable_items_dictionary/modifiable_items_dictionary.py`

 * *Files identical despite different names*

### Comparing `modifiable_items_dictionary-3.0.0/modifiable_items_dictionary.egg-info/PKG-INFO` & `modifiable_items_dictionary-3.0.1/modifiable_items_dictionary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modifiable-items-dictionary
-Version: 3.0.0
+Version: 3.0.1
 Summary: Typed and Tested Modifiable Items Dict and ModifiableItemsAttrDict which allow keys and values to be modified at run time. ModifiableItemsAttrDict additionally provides attribute-style access to dictionary items.
 Home-page: https://github.com/tybruno/modifiable-items-dictionary
 Author: Tyler Bruno
 License: MIT
 Keywords: python dict attribute dictionary attrdict mapping key-mangling value-mangling
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `modifiable_items_dictionary-3.0.0/setup.py` & `modifiable_items_dictionary-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Setup.py"""
 import setuptools
 
-__version__ = 'v3.0.0'
+__version__ = 'v3.0.1'
 __author__ = 'Tyler Bruno'
 _description = (
     'Typed and Tested Modifiable Items Dict and ModifiableItemsAttrDict which '
     'allow keys and values to be modified at run time. '
     'ModifiableItemsAttrDict additionally provides attribute-style access to '
     'dictionary items.'
 )
```

### Comparing `modifiable_items_dictionary-3.0.0/tests/test_modifiable_items_attr_dict.py` & `modifiable_items_dictionary-3.0.1/tests/test_modifiable_items_attr_dict.py`

 * *Files identical despite different names*

### Comparing `modifiable_items_dictionary-3.0.0/tests/test_modifiable_items_dict.py` & `modifiable_items_dictionary-3.0.1/tests/test_modifiable_items_dict.py`

 * *Files identical despite different names*

