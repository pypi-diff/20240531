# Comparing `tmp/discovery-core-0.9.6.tar.gz` & `tmp/discovery-core-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-core-0.9.6.tar", last modified: Fri Jan 19 19:08:51 2024, max compression
+gzip compressed data, was "discovery-core-0.9.7.tar", last modified: Wed Jan 24 14:53:36 2024, max compression
```

## Comparing `discovery-core-0.9.6.tar` & `discovery-core-0.9.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-19 19:08:51.086544 discovery-core-0.9.6/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.9.6/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.9.6/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2024-01-19 19:08:51.086756 discovery-core-0.9.6/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.9.6/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-19 19:08:51.064036 discovery-core-0.9.6/discovery_core.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2024-01-19 19:08:50.000000 discovery-core-0.9.6/discovery_core.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     1208 2024-01-19 19:08:50.000000 discovery-core-0.9.6/discovery_core.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2024-01-19 19:08:50.000000 discovery-core-0.9.6/discovery_core.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       13 2024-01-19 19:08:50.000000 discovery-core-0.9.6/discovery_core.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-19 19:08:51.064476 discovery-core-0.9.6/ds_core/
--rw-r--r--   0 doatridge   (503) staff       (20)       74 2023-12-28 01:35:03.000000 discovery-core-0.9.6/ds_core/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-19 19:08:51.067117 discovery-core-0.9.6/ds_core/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.6/ds_core/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    63354 2023-10-03 22:02:38.000000 discovery-core-0.9.6/ds_core/components/abstract_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)    30913 2023-12-28 01:34:07.000000 discovery-core-0.9.6/ds_core/components/core_commons.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-19 19:08:51.069719 discovery-core-0.9.6/ds_core/handlers/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.6/ds_core/handlers/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    16254 2023-12-06 19:32:25.000000 discovery-core-0.9.6/ds_core/handlers/abstract_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5399 2023-08-30 21:48:54.000000 discovery-core-0.9.6/ds_core/handlers/event_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-19 19:08:51.070987 discovery-core-0.9.6/ds_core/intent/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.6/ds_core/intent/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.9.6/ds_core/intent/abstract_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-19 19:08:51.074183 discovery-core-0.9.6/ds_core/properties/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.6/ds_core/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    66008 2024-01-19 19:02:36.000000 discovery-core-0.9.6/ds_core/properties/abstract_properties.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.9.6/ds_core/properties/decorator_patterns.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11286 2023-10-01 18:53:31.000000 discovery-core-0.9.6/ds_core/properties/property_manager.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2024-01-19 19:08:51.087413 discovery-core-0.9.6/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.9.6/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-19 19:08:51.075183 discovery-core-0.9.6/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.9.6/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-19 19:08:51.077324 discovery-core-0.9.6/test/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.6/test/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    31386 2023-10-03 22:02:38.000000 discovery-core-0.9.6/test/components/abstract_component_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25689 2023-12-28 01:51:55.000000 discovery-core-0.9.6/test/components/commons_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     6900 2023-09-04 05:05:02.000000 discovery-core-0.9.6/test/components/pyarrow_component.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-19 19:08:51.080655 discovery-core-0.9.6/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.6/test/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11992 2023-12-06 20:33:10.000000 discovery-core-0.9.6/test/handlers/connector_contract_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4966 2023-09-27 19:55:00.000000 discovery-core-0.9.6/test/handlers/event_handlers_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2569 2023-12-01 20:09:32.000000 discovery-core-0.9.6/test/handlers/handler_factory_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-19 19:08:51.082343 discovery-core-0.9.6/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.6/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1667 2023-10-01 17:30:33.000000 discovery-core-0.9.6/test/intent/abstract_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7106 2023-09-04 04:49:36.000000 discovery-core-0.9.6/test/intent/pyarrow_intent_model.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-19 19:08:51.085764 discovery-core-0.9.6/test/properties/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.6/test/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    33733 2023-10-01 17:09:53.000000 discovery-core-0.9.6/test/properties/abstract_properties_manager_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     9064 2023-09-27 22:13:06.000000 discovery-core-0.9.6/test/properties/property_manager_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)      415 2023-09-04 04:49:36.000000 discovery-core-0.9.6/test/properties/pyarrow_property_manager.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-24 14:53:36.542489 discovery-core-0.9.7/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.9.7/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.9.7/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2024-01-24 14:53:36.542707 discovery-core-0.9.7/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.9.7/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-24 14:53:36.514998 discovery-core-0.9.7/discovery_core.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2024-01-24 14:53:36.000000 discovery-core-0.9.7/discovery_core.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1208 2024-01-24 14:53:36.000000 discovery-core-0.9.7/discovery_core.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2024-01-24 14:53:36.000000 discovery-core-0.9.7/discovery_core.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       13 2024-01-24 14:53:36.000000 discovery-core-0.9.7/discovery_core.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-24 14:53:36.515486 discovery-core-0.9.7/ds_core/
+-rw-r--r--   0 doatridge   (503) staff       (20)       74 2024-01-19 19:09:15.000000 discovery-core-0.9.7/ds_core/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-24 14:53:36.517765 discovery-core-0.9.7/ds_core/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.7/ds_core/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    63331 2024-01-24 14:51:46.000000 discovery-core-0.9.7/ds_core/components/abstract_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    30913 2023-12-28 01:34:07.000000 discovery-core-0.9.7/ds_core/components/core_commons.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-24 14:53:36.522357 discovery-core-0.9.7/ds_core/handlers/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.7/ds_core/handlers/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    16254 2023-12-06 19:32:25.000000 discovery-core-0.9.7/ds_core/handlers/abstract_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5399 2023-08-30 21:48:54.000000 discovery-core-0.9.7/ds_core/handlers/event_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-24 14:53:36.524134 discovery-core-0.9.7/ds_core/intent/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.7/ds_core/intent/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.9.7/ds_core/intent/abstract_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-24 14:53:36.528888 discovery-core-0.9.7/ds_core/properties/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.7/ds_core/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    66008 2024-01-19 19:02:36.000000 discovery-core-0.9.7/ds_core/properties/abstract_properties.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.9.7/ds_core/properties/decorator_patterns.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11286 2023-10-01 18:53:31.000000 discovery-core-0.9.7/ds_core/properties/property_manager.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2024-01-24 14:53:36.543354 discovery-core-0.9.7/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.9.7/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-24 14:53:36.529924 discovery-core-0.9.7/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.9.7/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-24 14:53:36.532906 discovery-core-0.9.7/test/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.7/test/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    31386 2023-10-03 22:02:38.000000 discovery-core-0.9.7/test/components/abstract_component_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25689 2023-12-28 01:51:55.000000 discovery-core-0.9.7/test/components/commons_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     6900 2023-09-04 05:05:02.000000 discovery-core-0.9.7/test/components/pyarrow_component.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-24 14:53:36.536278 discovery-core-0.9.7/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.7/test/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11992 2023-12-06 20:33:10.000000 discovery-core-0.9.7/test/handlers/connector_contract_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4966 2023-09-27 19:55:00.000000 discovery-core-0.9.7/test/handlers/event_handlers_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2569 2023-12-01 20:09:32.000000 discovery-core-0.9.7/test/handlers/handler_factory_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-24 14:53:36.538377 discovery-core-0.9.7/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.7/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1667 2023-10-01 17:30:33.000000 discovery-core-0.9.7/test/intent/abstract_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7106 2023-09-04 04:49:36.000000 discovery-core-0.9.7/test/intent/pyarrow_intent_model.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2024-01-24 14:53:36.541767 discovery-core-0.9.7/test/properties/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.9.7/test/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    33733 2023-10-01 17:09:53.000000 discovery-core-0.9.7/test/properties/abstract_properties_manager_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     9064 2023-09-27 22:13:06.000000 discovery-core-0.9.7/test/properties/property_manager_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      415 2023-09-04 04:49:36.000000 discovery-core-0.9.7/test/properties/pyarrow_property_manager.py
```

### Comparing `discovery-core-0.9.6/LICENSE.txt` & `discovery-core-0.9.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/PKG-INFO` & `discovery-core-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.9.6
+Version: 0.9.7
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.9.6/README.rst` & `discovery-core-0.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/discovery_core.egg-info/PKG-INFO` & `discovery-core-0.9.7/discovery_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.9.6
+Version: 0.9.7
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.9.6/discovery_core.egg-info/SOURCES.txt` & `discovery-core-0.9.7/discovery_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/ds_core/components/abstract_component.py` & `discovery-core-0.9.7/ds_core/components/abstract_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -799,22 +799,22 @@
         else:
             for intent in tuple(self.pm.get_intent().keys()):
                 self.pm.remove_intent(level=intent)
             result = True
         self.pm_persist(save)
         return result
 
-    def add_intent_level_description(self, level: [int, str], text: str, save: bool=None):
-        """ sets description to the augmented knowledge 'intent' to a level
+    def add_action_description(self, action: [int, str], text: str, save: bool=None):
+        """ sets description associated with an intent action
 
-        :param level: the intent level to add the comment to
+        :param action: the action to add the comment to
         :param text: the description text
         :param save: (optional) override of the default save action set at initialisation.
         """
-        self.pm.set_intent_description(level=level, text=text)
+        self.pm.set_intent_description(level=action, text=text)
         self.pm_persist(save)
         return
 
     """
         CANONICAL SECTION
     """
     def load_canonical(self, connector_name: str, reset_changed: bool=None, has_changed: bool=None,
```

### Comparing `discovery-core-0.9.6/ds_core/components/core_commons.py` & `discovery-core-0.9.7/ds_core/components/core_commons.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/ds_core/handlers/abstract_handlers.py` & `discovery-core-0.9.7/ds_core/handlers/abstract_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/ds_core/handlers/event_handlers.py` & `discovery-core-0.9.7/ds_core/handlers/event_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/ds_core/intent/abstract_intent.py` & `discovery-core-0.9.7/ds_core/intent/abstract_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/ds_core/properties/abstract_properties.py` & `discovery-core-0.9.7/ds_core/properties/abstract_properties.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/ds_core/properties/decorator_patterns.py` & `discovery-core-0.9.7/ds_core/properties/decorator_patterns.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/ds_core/properties/property_manager.py` & `discovery-core-0.9.7/ds_core/properties/property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/setup.py` & `discovery-core-0.9.7/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/test/components/abstract_component_test.py` & `discovery-core-0.9.7/test/components/abstract_component_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/test/components/commons_test.py` & `discovery-core-0.9.7/test/components/commons_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/test/components/pyarrow_component.py` & `discovery-core-0.9.7/test/components/pyarrow_component.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/test/handlers/connector_contract_test.py` & `discovery-core-0.9.7/test/handlers/connector_contract_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/test/handlers/event_handlers_test.py` & `discovery-core-0.9.7/test/handlers/event_handlers_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/test/handlers/handler_factory_test.py` & `discovery-core-0.9.7/test/handlers/handler_factory_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/test/intent/abstract_intent_test.py` & `discovery-core-0.9.7/test/intent/abstract_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/test/intent/pyarrow_intent_model.py` & `discovery-core-0.9.7/test/intent/pyarrow_intent_model.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/test/properties/abstract_properties_manager_test.py` & `discovery-core-0.9.7/test/properties/abstract_properties_manager_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.9.6/test/properties/property_manager_test.py` & `discovery-core-0.9.7/test/properties/property_manager_test.py`

 * *Files identical despite different names*

