# Comparing `tmp/graphene_django_extended-1.2.1.tar.gz` & `tmp/graphene_django_extended-1.2.2.tar.gz`

## Comparing `graphene_django_extended-1.2.1.tar` & `graphene_django_extended-1.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/__init__.py
--rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/connection.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/converter.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/interface.py
--rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/mutation.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/_mutations/Pipfile
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/_mutations/__init__.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/_mutations/delete_mutation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/_mutations/fields.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/_mutations/global_id_serializer_mutation.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/_mutations/inputs.py
--rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/_mutations/model_mutation.py
--rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/_mutations/mutations.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/search/__init__.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/search/connection.py
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/search/field.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/search/node.py
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/search/types.py
--rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/graphene_django_extended/tests/test_interface.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/.gitignore
--rw-r--r--   0        0        0    17098 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/LICENSE
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/README.md
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/__init__.py
+-rw-r--r--   0        0        0     6263 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/connection.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/converter.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/interface.py
+-rw-r--r--   0        0        0     6283 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/mutation.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/_mutations/Pipfile
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/_mutations/__init__.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/_mutations/delete_mutation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/_mutations/fields.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/_mutations/global_id_serializer_mutation.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/_mutations/inputs.py
+-rw-r--r--   0        0        0     5366 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/_mutations/model_mutation.py
+-rw-r--r--   0        0        0     5667 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/_mutations/mutations.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/search/__init__.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/search/connection.py
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/search/field.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/search/node.py
+-rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/search/types.py
+-rw-r--r--   0        0        0     6849 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/graphene_django_extended/tests/test_interface.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/.gitignore
+-rw-r--r--   0        0        0    17098 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/LICENSE
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/README.md
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 graphene_django_extended-1.2.2/PKG-INFO
```

### Comparing `graphene_django_extended-1.2.1/graphene_django_extended/connection.py` & `graphene_django_extended-1.2.2/graphene_django_extended/connection.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.2.1/graphene_django_extended/converter.py` & `graphene_django_extended-1.2.2/graphene_django_extended/converter.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.2.1/graphene_django_extended/interface.py` & `graphene_django_extended-1.2.2/graphene_django_extended/interface.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.2.1/graphene_django_extended/mutation.py` & `graphene_django_extended-1.2.2/graphene_django_extended/mutation.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,16 +126,14 @@
             else:
                 raise Exception(
                     'Invalid update operation. Input parameter "{}" required.'.format(
                         lookup_field
                     )
                 )
 
-            logger.debug(f"DATA {data}")
-
             return {
                 "instance": instance,
                 "data": input,
                 "context": {"request": info.context},
                 "partial": partial,
             }
```

### Comparing `graphene_django_extended-1.2.1/graphene_django_extended/_mutations/delete_mutation.py` & `graphene_django_extended-1.2.2/graphene_django_extended/_mutations/delete_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.2.1/graphene_django_extended/_mutations/global_id_serializer_mutation.py` & `graphene_django_extended-1.2.2/graphene_django_extended/_mutations/global_id_serializer_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.2.1/graphene_django_extended/_mutations/model_mutation.py` & `graphene_django_extended-1.2.2/graphene_django_extended/_mutations/model_mutation.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.2.1/graphene_django_extended/_mutations/mutations.py` & `graphene_django_extended-1.2.2/graphene_django_extended/_mutations/mutations.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.2.1/graphene_django_extended/search/connection.py` & `graphene_django_extended-1.2.2/graphene_django_extended/search/connection.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.2.1/graphene_django_extended/search/field.py` & `graphene_django_extended-1.2.2/graphene_django_extended/search/field.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.2.1/graphene_django_extended/search/node.py` & `graphene_django_extended-1.2.2/graphene_django_extended/search/node.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.2.1/graphene_django_extended/search/types.py` & `graphene_django_extended-1.2.2/graphene_django_extended/search/types.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.2.1/graphene_django_extended/tests/test_interface.py` & `graphene_django_extended-1.2.2/graphene_django_extended/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.2.1/LICENSE` & `graphene_django_extended-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.2.1/README.md` & `graphene_django_extended-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `graphene_django_extended-1.2.1/pyproject.toml` & `graphene_django_extended-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "graphene-django-extended"
-version = "1.2.1"
+version = "1.2.2"
 #authors = [
 #  { name="Example Author", email="author@example.com" },
 #]
 description = "A collection of utility classes to extend the base functionality of graphene_django"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `graphene_django_extended-1.2.1/PKG-INFO` & `graphene_django_extended-1.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: graphene-django-extended
-Version: 1.2.1
+Version: 1.2.2
 Summary: A collection of utility classes to extend the base functionality of graphene_django
 Project-URL: Homepage, https://github.com/AztlanEngineering/graphene-django-extended
 Project-URL: Issues, https://github.com/AztlanEngineering/graphene-django-extended/issues
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

