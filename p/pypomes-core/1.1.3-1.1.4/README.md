# Comparing `tmp/pypomes_core-1.1.3.tar.gz` & `tmp/pypomes_core-1.1.4.tar.gz`

## Comparing `pypomes_core-1.1.3.tar` & `pypomes_core-1.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    29820 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    26573 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    29820 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2934 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     8435 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    26605 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.1.4/PKG-INFO
```

### Comparing `pypomes_core-1.1.3/src/pypomes_core/.ruff.toml` & `pypomes_core-1.1.4/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.3/src/pypomes_core/__init__.py` & `pypomes_core-1.1.4/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.3/src/pypomes_core/datetime_pomes.py` & `pypomes_core-1.1.4/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.3/src/pypomes_core/dict_pomes.py` & `pypomes_core-1.1.4/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.3/src/pypomes_core/email_pomes.py` & `pypomes_core-1.1.4/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.3/src/pypomes_core/encoding_pomes.py` & `pypomes_core-1.1.4/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.3/src/pypomes_core/env_pomes.py` & `pypomes_core-1.1.4/src/pypomes_core/env_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
     Retrieve and return the string value defined for *key* in the current operating environment.
 
     :param key: The key the value is associated with
     :param def_value: The default value to return, if the key has not been defined
     :return: The str value associated with the key
     """
-    result: str = os.environ.get(key)
+    result: str = os.getenv(key)
     if result is None:
         result = def_value
 
     return result
 
 
 def env_get_bool(key: str,
```

### Comparing `pypomes_core-1.1.3/src/pypomes_core/exception_pomes.py` & `pypomes_core-1.1.4/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.3/src/pypomes_core/file_pomes.py` & `pypomes_core-1.1.4/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.3/src/pypomes_core/json_pomes.py` & `pypomes_core-1.1.4/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.3/src/pypomes_core/list_pomes.py` & `pypomes_core-1.1.4/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.3/src/pypomes_core/str_pomes.py` & `pypomes_core-1.1.4/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.3/src/pypomes_core/validation_msgs.py` & `pypomes_core-1.1.4/src/pypomes_core/validation_msgs.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 __ERR_MSGS: Final[dict] = {
     101: {
         "en": "{}",
         "pt": "{}",
     },
     102: {
         "en": "Unexpected error: {}",
-        "pt": "Error não previsto: {}",
+        "pt": "Error inesperado: {}",
     },
     103: {
         "en": "Invalid operation {}",
         "pt": "Operação {} inválida",
     },
     104: {
         "en": "The operation {} returned the error {}",
@@ -21,14 +21,26 @@
         "en": "Error invoking service {}: {}",
         "pt": "Erro na invocação do serviço {}: {}",
     },
     106: {
         "en": "No records matching the provided criteria found",
         "pt": "Não foram encontrados registros para os critérios fornecidos",
     },
+    107: {
+        "en": "No files matching the provided criteria found",
+        "pt": "Não foram encontrados arquivos para os critérios fornecidos",
+    },
+    111: {
+        "en": "File {} not found",
+        "pt": "Arquivo {} não encontrado",
+    },
+    112: {
+        "en": "Environment variable {} not defined",
+        "pt": "Variável de ambiente {} não definida",
+    },
     121: {
         "en": "Required attribute",
         "pt": "Atributo obrigatório",
     },
     122: {
         "en": "Attribute is unknown or invalid in this context",
         "pt": "Atributo desconhecido ou inválido para o contexto",
@@ -38,16 +50,16 @@
         "pt": "Atributo não se aplica a {}",
     },
     124: {
         "en": "Attribute applicable only for {}",
         "pt": "Atributo se aplica apenas a {}",
     },
     125: {
-        "en": "A value has not yet been assigned",
-        "pt": "Valor ainda não foi atribuído",
+        "en": "A value has not been assigned",
+        "pt": "Valor não foi atribuído",
     },
     126: {
         "en": "Value {} cannot be assigned for attributes {} at the same time",
         "pt": "Valor {} não pode ser atribuído aos atributos {} ao mesmo tempo",
     },
     141: {
         "en": "Invalid value {}",
```

### Comparing `pypomes_core-1.1.3/src/pypomes_core/validation_pomes.py` & `pypomes_core-1.1.4/src/pypomes_core/validation_pomes.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,16 @@
         stat = validate_format_error(152, value, "str", f"@{attr}")
     else:
         values = default if isinstance(default, list) else None
         stat = validate_value(attr=attr,
                               val=value,
                               max_val=min_length,
                               min_val=max_length,
-                              values=values,required= required)
+                              values=values,
+                              required= required)
 
     if stat:
         __validate_log(errors=errors,
                        err_msg=stat,
                        logger=logger)
     else:
         result = value
```

### Comparing `pypomes_core-1.1.3/src/pypomes_core/xml_pomes.py` & `pypomes_core-1.1.4/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.3/LICENSE` & `pypomes_core-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.3/pyproject.toml` & `pypomes_core-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-1.1.3/PKG-INFO` & `pypomes_core-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 1.1.3
+Version: 1.1.4
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

