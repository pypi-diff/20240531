# Comparing `tmp/pypomes_core-1.1.2.tar.gz` & `tmp/pypomes_core-1.1.3.tar.gz`

## Comparing `pypomes_core-1.1.2.tar` & `pypomes_core-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/src/pypomes_core/.ruff.toml
--rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    29820 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/src/pypomes_core/validation_msgs.py
--rw-r--r--   0        0        0    24903 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    29820 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4760 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6708 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/validation_msgs.py
+-rw-r--r--   0        0        0    26573 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 pypomes_core-1.1.3/PKG-INFO
```

### Comparing `pypomes_core-1.1.2/src/pypomes_core/.ruff.toml` & `pypomes_core-1.1.3/src/pypomes_core/.ruff.toml`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.2/src/pypomes_core/__init__.py` & `pypomes_core-1.1.3/src/pypomes_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.2/src/pypomes_core/datetime_pomes.py` & `pypomes_core-1.1.3/src/pypomes_core/datetime_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.2/src/pypomes_core/dict_pomes.py` & `pypomes_core-1.1.3/src/pypomes_core/dict_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.2/src/pypomes_core/email_pomes.py` & `pypomes_core-1.1.3/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.2/src/pypomes_core/encoding_pomes.py` & `pypomes_core-1.1.3/src/pypomes_core/encoding_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.2/src/pypomes_core/env_pomes.py` & `pypomes_core-1.1.3/src/pypomes_core/env_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.2/src/pypomes_core/exception_pomes.py` & `pypomes_core-1.1.3/src/pypomes_core/exception_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.2/src/pypomes_core/file_pomes.py` & `pypomes_core-1.1.3/src/pypomes_core/file_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.2/src/pypomes_core/json_pomes.py` & `pypomes_core-1.1.3/src/pypomes_core/json_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.2/src/pypomes_core/list_pomes.py` & `pypomes_core-1.1.3/src/pypomes_core/list_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.2/src/pypomes_core/str_pomes.py` & `pypomes_core-1.1.3/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.2/src/pypomes_core/validation_msgs.py` & `pypomes_core-1.1.3/src/pypomes_core/validation_msgs.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,37 +98,45 @@
         "pt": "Valor {} inválido: deve ser do tipo {}",
     },
     153: {
         "en": "Invalid value {}: date is later than the current date",
         "pt": "Valor {} inválido: data posterior à data atual",
     },
     171: {
-        "en": "Unable to receive attachment: {}",
+        "en": "Error receiving attachment: {}",
         "pt": "Erro no recebimento de documento anexado: {}",
     },
     172: {
         "en": "Invalid attachment type {}: {}",
         "pt": "Tipo de documento anexado {} inválido: {}",
     },
+    173: {
+        "en": "Unable to receive attachment {}",
+        "pt": "Não foi possível receber o documento anexado {}",
+    },
     201: {
-        "en": "Error accessing the DB {} in {}: {}",
-        "pt": "Erro na interação com o BD {} em {}: {}",
+        "en": "Error accessing the DB in {}: {}",
+        "pt": "Erro na interação com o BD em {}: {}",
     },
     202: {
         "en": "No record found on DB in {}, for {}",
         "pt": "Nenhum registro encontrado no BD, em {} para {}",
     },
     203: {
         "en": "Error accessing the object store: {}",
         "pt": "Erro na interação com o armazenador de objetos: {}",
     },
     204: {
         "en": "Unable to retrieve document {} from the object store",
         "pt": "Não foi possível recuperar o documento {} no armazenador de objetos",
     },
+    205: {
+        "en": "Error accessing the message queue manager: {}",
+        "pt": "Erro na interação com o gerenciador de mensagens: {}",
+    },
     211: {
         "en": "Error accessing the job scheduler: {}",
         "pt": "Erro na interação com o gerenciador de tarefas: {}",
     },
     212: {
         "en": "Unable to access the entry point {} for the job {}: {}",
         "pt": "Não foi possível acesso ao ponto de entrada {} para a tarefa {}: {}",
@@ -159,15 +167,15 @@
     },
     242: {
         "en": "Failed to verify the digital signature of document {}: {}",
         "pt": "Erro na verificação da assinatura digital do documento {}:{}",
     },
     243: {
         "en": "Failed to verify the digest for document {}: {}",
-        "pt": "Erro na verificação do digesto do documento {}:{}",
+        "pt": "Erro na verificação do digesto do documento {}: {}",
     },
     244: {
         "en": "Document {} is not digitally signed",
         "pt": "Documento {} não contem assinatura digital",
     },
     245: {
         "en": "Invalid digital signature in document {}: {}",
@@ -175,15 +183,15 @@
     },
     246: {
         "en": "Document {} was modified after being digitally signed",
         "pt": "Documento {} modificado após assinatura digital",
     },
     247: {
         "en": "Document {} has invalid digest",
-        "pt": "Digiesto do documento {} é inválido",
+        "pt": "Digesto do documento {} inválido",
     },
 }
 
 _ERR_MSGS_EN: dict = {}
 for key, value in __ERR_MSGS.items():
     _ERR_MSGS_EN[key] = value["en"]
```

### Comparing `pypomes_core-1.1.2/src/pypomes_core/validation_pomes.py` & `pypomes_core-1.1.3/src/pypomes_core/validation_pomes.py`

 * *Files 6% similar despite different names*

```diff
@@ -179,18 +179,25 @@
          (isinstance(value, bool) or not isinstance(value, int)):
         # 152: Invalid value {}: must be type {}
         stat = validate_format_error(152, value, "int", f"@{attr}")
     else:
         if isinstance(value, str) and value.isnumeric():
             value = int(value)
         values = default if isinstance(default, list) else None
-        stat = validate_value(attr, value, min_val, max_val, values, required)
+        stat = validate_value(attr=attr,
+                              val=value,
+                              min_val=min_val,
+                              max_val=max_val,
+                              values=values,
+                              required=required)
 
     if stat:
-        __validate_log(errors, stat, logger)
+        __validate_log(errors=errors,
+                       err_msg=stat,
+                       logger=logger)
     else:
         result = value
 
     return result
 
 
 def validate_float(errors: list[str] | None,
@@ -235,18 +242,25 @@
         # 152: Invalid value {}: must be type {}
         stat = validate_format_error(152, value, "float", f"@{attr}")
     else:
         if (isinstance(value, int) and not isinstance(value, bool)) or \
            (isinstance(value, str) and value.replace(".", "", 1).isnumeric()):
             value = float(value)
         values = default if isinstance(default, list) else None
-        stat = validate_value(attr, value, min_val, max_val, values, required)
+        stat = validate_value(attr=attr,
+                              val=value,
+                              min_val=min_val,
+                              max_val=max_val,
+                              values=values,
+                              required=required)
 
     if stat:
-        __validate_log(errors, stat, logger)
+        __validate_log(errors=errors,
+                       err_msg=stat,
+                       logger=logger)
     else:
         result = value
 
     return result
 
 
 def validate_str(errors: list[str] | None,
@@ -287,18 +301,24 @@
     if value is None and isinstance(default, str):
         value = default
     elif value is not None and not isinstance(value, str):
         # 152: Invalid value {}: must be type {}
         stat = validate_format_error(152, value, "str", f"@{attr}")
     else:
         values = default if isinstance(default, list) else None
-        stat = validate_value(attr, value, min_length, max_length, values, required)
+        stat = validate_value(attr=attr,
+                              val=value,
+                              max_val=min_length,
+                              min_val=max_length,
+                              values=values,required= required)
 
     if stat:
-        __validate_log(errors, stat, logger)
+        __validate_log(errors=errors,
+                       err_msg=stat,
+                       logger=logger)
     else:
         result = value
 
     return result
 
 
 def validate_date(errors: list[str] | None,
@@ -333,30 +353,33 @@
     suffix: str = attr[pos:]
 
     # obtain the value
     value: str = scheme.get(suffix)
 
     # validate it
     if value:
-        result = date_parse(value, dayfirst=day_first)
+        result = date_parse(dt_str=value,
+                            dayfirst=day_first)
         if not result:
             # 141: Invalid value {}
             stat = validate_format_error(141, value, f"@{attr}")
-        elif result > datetime.now(TIMEZONE_LOCAL).date():
+        elif result > datetime.now(tz=TIMEZONE_LOCAL).date():
             # 153: Invalid value {}: date is later than the current date
             stat = validate_format_error(153, value, f"@{attr}")
     elif isinstance(default, date):
         result = default
     elif isinstance(required, bool) and required:
         # 121: Required attribute
         stat = validate_format_error(121, f"@{attr}")
 
     if stat:
         result = None
-        __validate_log(errors, stat, logger)
+        __validate_log(errors=errors,
+                       err_msg=stat,
+                       logger=logger)
 
     return result
 
 
 def validate_datetime(errors: list[str] | None,
                       scheme: dict,
                       attr: str,
@@ -387,29 +410,32 @@
     stat: str | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
 
     # obtain and validate the value
     value: str = scheme[suffix]
     if value:
-        result = datetime_parse(value, dayfirst=day_first)
+        result = datetime_parse(dt_str=value,
+                                dayfirst=day_first)
         if not result:
             # 141: Invalid value {}
             stat = validate_format_error(141, value, f"@{attr}")
-        elif result > datetime.now(TIMEZONE_LOCAL):
+        elif result > datetime.now(tz=TIMEZONE_LOCAL):
             # 153: Invalid value {}: date is later than the current date
             stat = validate_format_error(153, value, f"@{attr}")
     elif isinstance(default, datetime):
         result = default
     elif isinstance(required, bool) and required:
         # 121: Required attribute
         stat = validate_format_error(121, f"@{attr}")
 
     if stat:
-        __validate_log(errors, stat, logger)
+        __validate_log(errors=errors,
+                       err_msg=stat,
+                       logger=logger)
 
     return result
 
 
 def validate_ints(errors: list[str] | None,
                   scheme: dict,
                   attr: str,
@@ -441,15 +467,18 @@
         values: list[Any] = scheme[suffix]
         if isinstance(values, list):
             result = []
             if len(values) > 0:
                 for inx, value in enumerate(values):
                     result.append(value)
                     if isinstance(value, int):
-                        stat = validate_value(f"@{attr}[{inx+1}]", value, min_val, max_val)
+                        stat = validate_value(attr=f"@{attr}[{inx+1}]",
+                                              val=value,
+                                              min_val=min_val,
+                                              max_val=max_val)
                     else:
                         # 152: Invalid value {}: must be type {}
                         stat = validate_format_error(152, value, "int", f"@{attr}[{inx+1}]")
             elif required:
                 # 121: Required attribute
                 stat = validate_format_error(121, f"@{attr}")
         else:
@@ -457,15 +486,17 @@
             stat = validate_format_error(152, result, "list", f"@{attr}")
     except (KeyError, TypeError):
         if required:
             # 121: Required attribute
             stat = validate_format_error(121, f"@{attr}")
 
     if stat:
-        __validate_log(errors, stat, logger)
+        __validate_log(errors=errors,
+                       err_msg=stat,
+                       logger=logger)
 
     return result
 
 
 def validate_strs(errors: list[str] | None,
                   scheme: dict,
                   attr: str,
@@ -497,15 +528,18 @@
         values: list[Any] = scheme[suffix]
         if isinstance(values, list):
             result = []
             if len(values) > 0:
                 for inx, value in enumerate(values):
                     result.append(value)
                     if isinstance(value, str):
-                        stat = validate_value(f"@{attr}[{inx+1}]", value, min_length, max_length)
+                        stat = validate_value(attr=f"@{attr}[{inx+1}]",
+                                              val=value,
+                                              min_val=min_length,
+                                              max_val=max_length)
                     else:
                         # 152: Invalid value {}: must be type {}
                         stat = validate_format_error(152, value, "str", f"@{attr}[{inx+1}]")
             elif required:
                 # 121: Required attribute
                 stat = validate_format_error(121, f"@{attr}")
         else:
@@ -513,15 +547,17 @@
             stat = validate_format_error(152, result, "list", f"@{attr}")
     except (KeyError, TypeError):
         if required:
             # 121: Required attribute
             stat = validate_format_error(121, f"@{attr}")
 
     if stat:
-        __validate_log(errors, stat, logger)
+        __validate_log(errors=errors,
+                       err_msg=stat,
+                       logger=logger)
 
     return result
 
 
 def validate_format_error(error_id: int,
                           *args: Any) -> str:
     """
@@ -550,15 +586,20 @@
     if VALIDATION_MSG_PREFIX:
         result += VALIDATION_MSG_PREFIX + str(error_id) + ": "
     result += err_msgs.get(error_id) or ""
 
     # apply the provided arguments
     for arg in args:
         if arg is None:
-            result = result.replace(" {}", "", 1)
+            pos1: int = result.find(": {}")
+            pos2: int = result.find(" {}")
+            if pos1 < 0 or pos2 < pos1:
+                result = result.replace(" {}", "", 1)
+            else:
+                result = result.replace(": {}", "", 1)
         elif not result or (isinstance(arg, str) and arg.startswith("@")):
             result += " " + arg
         elif isinstance(arg, str) and arg.find(" ") > 0:
             result = result.replace("{}", arg, 1)
         else:
             result = result.replace("{}", f"'{arg}'", 1)
```

### Comparing `pypomes_core-1.1.2/src/pypomes_core/xml_pomes.py` & `pypomes_core-1.1.3/src/pypomes_core/xml_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.2/LICENSE` & `pypomes_core-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-1.1.2/pyproject.toml` & `pypomes_core-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `pypomes_core-1.1.2/PKG-INFO` & `pypomes_core-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypomes_core
-Version: 1.1.2
+Version: 1.1.3
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

