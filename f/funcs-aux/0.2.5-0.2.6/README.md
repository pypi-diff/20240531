# Comparing `tmp/funcs_aux-0.2.5.tar.gz` & `tmp/funcs_aux-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs_aux-0.2.5.tar", last modified: Thu May 23 14:34:56 2024, max compression
+gzip compressed data, was "funcs_aux-0.2.6.tar", last modified: Fri May 31 08:02:22 2024, max compression
```

## Comparing `funcs_aux-0.2.5.tar` & `funcs_aux-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 14:34:56.635193 funcs_aux-0.2.5/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.2.5/LICENSE
--rw-rw-rw-   0        0        0     1883 2024-05-23 14:34:56.635193 funcs_aux-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-23 14:34:15.000000 funcs_aux-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 14:34:56.625819 funcs_aux-0.2.5/funcs_aux/
--rw-rw-rw-   0        0        0     1965 2024-05-22 09:14:12.000000 funcs_aux-0.2.5/funcs_aux/__init__.py
--rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.2.5/funcs_aux/arrays.py
--rw-rw-rw-   0        0        0    10988 2024-05-23 14:33:55.000000 funcs_aux-0.2.5/funcs_aux/breeder_objects.py
--rw-rw-rw-   0        0        0     9485 2024-05-22 07:23:49.000000 funcs_aux-0.2.5/funcs_aux/breeder_str.py
--rw-rw-rw-   0        0        0     5221 2024-05-22 09:14:12.000000 funcs_aux-0.2.5/funcs_aux/iterables.py
--rw-rw-rw-   0        0        0     9678 2024-05-17 09:54:30.000000 funcs_aux-0.2.5/funcs_aux/results.py
--rw-rw-rw-   0        0        0     1918 2024-05-22 09:14:12.000000 funcs_aux-0.2.5/funcs_aux/strings.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:34:56.633860 funcs_aux-0.2.5/funcs_aux.egg-info/
--rw-rw-rw-   0        0        0     1883 2024-05-23 14:34:56.000000 funcs_aux-0.2.5/funcs_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-23 14:34:56.000000 funcs_aux-0.2.5/funcs_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 14:34:56.000000 funcs_aux-0.2.5/funcs_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 14:34:56.000000 funcs_aux-0.2.5/funcs_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 14:34:56.637272 funcs_aux-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 08:02:22.043991 funcs_aux-0.2.6/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0     1883 2024-05-31 08:02:22.043492 funcs_aux-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-31 08:01:37.000000 funcs_aux-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 08:02:22.032813 funcs_aux-0.2.6/funcs_aux/
+-rw-rw-rw-   0        0        0     2174 2024-05-31 07:59:53.000000 funcs_aux-0.2.6/funcs_aux/__init__.py
+-rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.2.6/funcs_aux/arrays.py
+-rw-rw-rw-   0        0        0    11092 2024-05-29 06:46:40.000000 funcs_aux-0.2.6/funcs_aux/breeder_objects.py
+-rw-rw-rw-   0        0        0     9485 2024-05-22 07:23:49.000000 funcs_aux-0.2.6/funcs_aux/breeder_str.py
+-rw-rw-rw-   0        0        0     5221 2024-05-22 09:14:12.000000 funcs_aux-0.2.6/funcs_aux/iterables.py
+-rw-rw-rw-   0        0        0     9678 2024-05-17 09:54:30.000000 funcs_aux-0.2.6/funcs_aux/results.py
+-rw-rw-rw-   0        0        0     1918 2024-05-22 09:14:12.000000 funcs_aux-0.2.6/funcs_aux/strings.py
+-rw-rw-rw-   0        0        0     6033 2024-05-31 07:54:42.000000 funcs_aux-0.2.6/funcs_aux/values.py
+drwxrwxrwx   0        0        0        0 2024-05-31 08:02:22.041531 funcs_aux-0.2.6/funcs_aux.egg-info/
+-rw-rw-rw-   0        0        0     1883 2024-05-31 08:02:21.000000 funcs_aux-0.2.6/funcs_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      349 2024-05-31 08:02:21.000000 funcs_aux-0.2.6/funcs_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 08:02:21.000000 funcs_aux-0.2.6/funcs_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-31 08:02:21.000000 funcs_aux-0.2.6/funcs_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 08:02:22.052961 funcs_aux-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.2.6/setup.py
```

### Comparing `funcs_aux-0.2.5/LICENSE` & `funcs_aux-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.5/PKG-INFO` & `funcs_aux-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.2.5
+Version: 0.2.6
 Summary: useful funcs in one place
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/funcs_aux
 Keywords: functions,auxiliary,auxiliary funcs,np funcs,collections funcs,strings funcs,result object
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# funcs_aux (v0.2.5)
+# funcs_aux (v0.2.6)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.2.5/README.md` & `funcs_aux-0.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# funcs_aux (v0.2.5)
+# funcs_aux (v0.2.6)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.2.5/funcs_aux/__init__.py` & `funcs_aux-0.2.6/funcs_aux/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,28 @@
     TYPE__FUNC,
     TYPE__FUNC_UNDER_VALUE,
     TYPE__ARGS,
     TYPE__KWARGS,
 
     # EXX
 )
+from .values import (
+    # BASE
+    Value_NotPassed,
+    Value_WithUnit,
+    Value_FromVariants,
+
+    # AUX
+
+    # TYPES
+
+    # EXX
+    Exx__ValueNotInVariants,
+    Exx__VariantsIncompatible,
+)
 from .strings import (
     # BASE
     Strings,
 
     # AUX
 
     # TYPES
```

### Comparing `funcs_aux-0.2.5/funcs_aux/arrays.py` & `funcs_aux-0.2.6/funcs_aux/arrays.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.5/funcs_aux/breeder_objects.py` & `funcs_aux-0.2.6/funcs_aux/breeder_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,14 +248,18 @@
                 obj_result = exx
             results = obj_result
 
         return results
 
     # -----------------------------------------------------------------------------------------------------------------
     def __getattr__(self, item: str) -> Union[None, Any, NoReturn]:
+        """
+        :param item:
+        :return: existed OBJECT from LIST or SINGLE!!!
+        """
         if self.INDEX is None:
             return
 
         # ACCESS TO OBJECT ----------------------------
         group_insts = self.group_get__insts(item)
         if group_insts is not None:
             if isinstance(group_insts, list):
```

### Comparing `funcs_aux-0.2.5/funcs_aux/breeder_str.py` & `funcs_aux-0.2.6/funcs_aux/breeder_str.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.5/funcs_aux/iterables.py` & `funcs_aux-0.2.6/funcs_aux/iterables.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.5/funcs_aux/results.py` & `funcs_aux-0.2.6/funcs_aux/results.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.5/funcs_aux/strings.py` & `funcs_aux-0.2.6/funcs_aux/strings.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.5/funcs_aux.egg-info/PKG-INFO` & `funcs_aux-0.2.6/funcs_aux.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.2.5
+Version: 0.2.6
 Summary: useful funcs in one place
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/funcs_aux
 Keywords: functions,auxiliary,auxiliary funcs,np funcs,collections funcs,strings funcs,result object
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# funcs_aux (v0.2.5)
+# funcs_aux (v0.2.6)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.2.5/setup.py` & `funcs_aux-0.2.6/setup.py`

 * *Files identical despite different names*

