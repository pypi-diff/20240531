# Comparing `tmp/pypomes_core-1.1.4.tar.gz` & `tmp/pypomes_core-1.1.5.tar.gz`

## Comparing `pypomes_core-1.1.4.tar` & `pypomes_core-1.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    29820 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    26605 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    29820 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     8434 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    26605 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.1.5/PKG-INFO
```

### Comparing `pypomes_core-1.1.4/src/pypomes_core/.ruff.toml` & `pypomes_core-1.1.5/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.4/src/pypomes_core/__init__.py` & `pypomes_core-1.1.5/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.4/src/pypomes_core/datetime_pomes.py` & `pypomes_core-1.1.5/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.4/src/pypomes_core/dict_pomes.py` & `pypomes_core-1.1.5/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.4/src/pypomes_core/email_pomes.py` & `pypomes_core-1.1.5/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.4/src/pypomes_core/encoding_pomes.py` & `pypomes_core-1.1.5/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.4/src/pypomes_core/env_pomes.py` & `pypomes_core-1.1.5/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.4/src/pypomes_core/exception_pomes.py` & `pypomes_core-1.1.5/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.4/src/pypomes_core/file_pomes.py` & `pypomes_core-1.1.5/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.4/src/pypomes_core/json_pomes.py` & `pypomes_core-1.1.5/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.4/src/pypomes_core/list_pomes.py` & `pypomes_core-1.1.5/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.4/src/pypomes_core/str_pomes.py` & `pypomes_core-1.1.5/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.4/src/pypomes_core/validation_msgs.py` & `pypomes_core-1.1.5/src/pypomes_core/validation_msgs.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 __ERR_MSGS: Final[dict] = {
     101: {
         "en": "{}",
         "pt": "{}",
     },
     102: {
         "en": "Unexpected error: {}",
-        "pt": "Error inesperado: {}",
+        "pt": "Erro inesperado: {}",
     },
     103: {
         "en": "Invalid operation {}",
         "pt": "Operação {} inválida",
     },
     104: {
         "en": "The operation {} returned the error {}",
```

### Comparing `pypomes_core-1.1.4/src/pypomes_core/validation_pomes.py` & `pypomes_core-1.1.5/src/pypomes_core/validation_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,16 +303,16 @@
     elif value is not None and not isinstance(value, str):
         # 152: Invalid value {}: must be type {}
         stat = validate_format_error(152, value, "str", f"@{attr}")
     else:
         values = default if isinstance(default, list) else None
         stat = validate_value(attr=attr,
                               val=value,
-                              max_val=min_length,
-                              min_val=max_length,
+                              min_val=min_length,
+                              max_val=max_length,
                               values=values,
                               required= required)
 
     if stat:
         __validate_log(errors=errors,
                        err_msg=stat,
                        logger=logger)
```

### Comparing `pypomes_core-1.1.4/src/pypomes_core/xml_pomes.py` & `pypomes_core-1.1.5/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.4/LICENSE` & `pypomes_core-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.4/pyproject.toml` & `pypomes_core-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-1.1.4/PKG-INFO` & `pypomes_core-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 1.1.4
+Version: 1.1.5
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

