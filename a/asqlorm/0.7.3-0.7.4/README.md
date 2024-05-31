# Comparing `tmp/asqlorm-0.7.3.tar.gz` & `tmp/asqlorm-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asqlorm-0.7.3.tar", max compression
+gzip compressed data, was "asqlorm-0.7.4.tar", max compression
```

## Comparing `asqlorm-0.7.3.tar` & `asqlorm-0.7.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.7.3/README.md
--rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.7.3/asqlorm/__init__.py
--rw-r--r--   0        0        0    32029 2024-05-22 21:02:20.511620 asqlorm-0.7.3/asqlorm/generator/main.py
--rw-r--r--   0        0        0    44933 2024-05-22 20:37:43.023429 asqlorm-0.7.3/asqlorm/models.py
--rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.7.3/asqlorm/sql/sql_alchemy.py
--rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.7.3/asqlorm/utils.py
--rw-r--r--   0        0        0      649 2024-05-22 21:03:02.163917 asqlorm-0.7.3/pyproject.toml
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 asqlorm-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.7.4/README.md
+-rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.7.4/asqlorm/__init__.py
+-rw-r--r--   0        0        0    32029 2024-05-22 21:02:20.511620 asqlorm-0.7.4/asqlorm/generator/main.py
+-rw-r--r--   0        0        0    44853 2024-05-31 03:00:43.453219 asqlorm-0.7.4/asqlorm/models.py
+-rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.7.4/asqlorm/sql/sql_alchemy.py
+-rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.7.4/asqlorm/utils.py
+-rw-r--r--   0        0        0      649 2024-05-31 02:39:21.084557 asqlorm-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 asqlorm-0.7.4/PKG-INFO
```

### Comparing `asqlorm-0.7.3/asqlorm/generator/main.py` & `asqlorm-0.7.4/asqlorm/generator/main.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.7.3/asqlorm/models.py` & `asqlorm-0.7.4/asqlorm/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -545,45 +545,45 @@
             raise ResolverError("No value found.")
         return node
 
     def parse_mutation_model(
         self, model: Insert | Patch, prefix: str | None = None
     ) -> tuple[dict[str, str], dict[str, T.Any]]:
         # mode json is incorrect for date-times
-        dump_d = model.model_dump(mode="python", exclude_unset=True)
         field_names_to_value_strs: dict[str, str] = {}
         variables: dict[str, T.Any] = {}
-        for k, dump_v in dump_d.items():
+        for k in model.model_fields_set:
             model_v = getattr(model, k)
             if isinstance(model_v, raw_sql):
                 if model_v.variables:
                     for raw_k, raw_v in model_v.variables.items():
                         if raw_k in variables and raw_v != variables[raw_k]:
                             raise ResolverError(
                                 f"Variables {raw_k} is already being used."
                             )
                         variables[raw_k] = raw_v
                 field_names_to_value_value = model_v.stmt
             else:
-                v = dump_v
-                if isinstance(v, dict):
-                    v = json.dumps(v)
-                if isinstance(v, list):
-                    v = [json.dumps(i) if isinstance(i, dict) else i for i in v]
-                if computed_c := self._node.__computed_columns__.get(k):
-                    if computed_c.basemodel_type:
-                        if model_v is not None:
-                            if computed_c.cardinality == Cardinality.ONE:
-                                v = model_v.model_dump_json()
-                            else:
-                                v = (
-                                    TypeAdapter(list[computed_c.basemodel_type])
-                                    .dump_json(model_v)
-                                    .decode("utf-8")
-                                )
+                computed_c = self._node.__computed_columns__.get(k)
+                if computed_c and computed_c.basemodel_type and model_v is not None:
+                    if computed_c.cardinality == Cardinality.ONE:
+                        v = model_v.model_dump_json()
+                    else:
+                        v = (
+                            TypeAdapter(list[computed_c.basemodel_type])
+                            .dump_json(model_v)
+                            .decode("utf-8")
+                        )
+                else:
+                    v = model.model_dump(mode="python")[k]
+                    if isinstance(v, dict):
+                        v = json.dumps(v)
+                    if isinstance(v, list):
+                        v = [json.dumps(i) if isinstance(i, dict) else i for i in v]
+
                 if prefix:
                     variable_name = f"{prefix}{k}"
                 else:
                     variable_name = k
                 if variable_name in variables and v != variables[variable_name]:
                     raise ResolverError(
                         f"Variable '{variable_name}' is already being used."
```

### Comparing `asqlorm-0.7.3/asqlorm/sql/sql_alchemy.py` & `asqlorm-0.7.4/asqlorm/sql/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.7.3/asqlorm/utils.py` & `asqlorm-0.7.4/asqlorm/utils.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.7.3/pyproject.toml` & `asqlorm-0.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asqlorm"
-version = "0.7.3"
+version = "0.7.4"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = 'asqlorm' }]
 exclude = ["tests/**/*"]
```

### Comparing `asqlorm-0.7.3/PKG-INFO` & `asqlorm-0.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asqlorm
-Version: 0.7.3
+Version: 0.7.4
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
```

