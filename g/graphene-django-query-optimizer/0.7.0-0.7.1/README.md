# Comparing `tmp/graphene_django_query_optimizer-0.7.0.tar.gz` & `tmp/graphene_django_query_optimizer-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_django_query_optimizer-0.7.0.tar", max compression
+gzip compressed data, was "graphene_django_query_optimizer-0.7.1.tar", max compression
```

## Comparing `graphene_django_query_optimizer-0.7.0.tar` & `graphene_django_query_optimizer-0.7.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1064 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/LICENSE
--rw-r--r--   0        0        0     3151 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/README.md
--rw-r--r--   0        0        0     6906 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      579 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/query_optimizer/__init__.py
--rw-r--r--   0        0        0    11972 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/query_optimizer/ast.py
--rw-r--r--   0        0        0     8533 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/query_optimizer/compiler.py
--rw-r--r--   0        0        0     2847 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/query_optimizer/converters.py
--rw-r--r--   0        0        0      177 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/query_optimizer/errors.py
--rw-r--r--   0        0        0    18385 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/query_optimizer/fields.py
--rw-r--r--   0        0        0     1686 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/filter.py
--rw-r--r--   0        0        0     5697 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/filter_info.py
--rw-r--r--   0        0        0    12382 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/optimizer.py
--rw-r--r--   0        0        0     4130 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/prefetch_hack.py
--rw-r--r--   0        0        0        0 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/py.typed
--rw-r--r--   0        0        0     3600 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/selections.py
--rw-r--r--   0        0        0     2520 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/settings.py
--rw-r--r--   0        0        0     3212 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/types.py
--rw-r--r--   0        0        0     4075 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/typing.py
--rw-r--r--   0        0        0     6842 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/utils.py
--rw-r--r--   0        0        0     3888 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/validators.py
--rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/LICENSE
+-rw-r--r--   0        0        0     3151 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/README.md
+-rw-r--r--   0        0        0     6906 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      579 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/__init__.py
+-rw-r--r--   0        0        0    11972 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/ast.py
+-rw-r--r--   0        0        0     8533 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/compiler.py
+-rw-r--r--   0        0        0     2847 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/converters.py
+-rw-r--r--   0        0        0      177 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/errors.py
+-rw-r--r--   0        0        0    18399 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/fields.py
+-rw-r--r--   0        0        0     1686 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/filter.py
+-rw-r--r--   0        0        0     5697 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/filter_info.py
+-rw-r--r--   0        0        0    12422 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/optimizer.py
+-rw-r--r--   0        0        0     4130 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/prefetch_hack.py
+-rw-r--r--   0        0        0        0 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/py.typed
+-rw-r--r--   0        0        0     3600 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/selections.py
+-rw-r--r--   0        0        0     2520 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/settings.py
+-rw-r--r--   0        0        0     3212 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/types.py
+-rw-r--r--   0        0        0     4075 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/typing.py
+-rw-r--r--   0        0        0     6842 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/utils.py
+-rw-r--r--   0        0        0     3888 2024-05-31 09:35:34.251037 graphene_django_query_optimizer-0.7.1/query_optimizer/validators.py
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.7.1/PKG-INFO
```

### Comparing `graphene_django_query_optimizer-0.7.0/LICENSE` & `graphene_django_query_optimizer-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.0/README.md` & `graphene_django_query_optimizer-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.0/pyproject.toml` & `graphene_django_query_optimizer-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphene-django-query-optimizer"
-version = "0.7.0"
+version = "0.7.1"
 description = "Automatically optimize SQL queries in Graphene-Django schemas."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "query_optimizer" },
 ]
```

### Comparing `graphene_django_query_optimizer-0.7.0/query_optimizer/__init__.py` & `graphene_django_query_optimizer-0.7.1/query_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.0/query_optimizer/ast.py` & `graphene_django_query_optimizer-0.7.1/query_optimizer/ast.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.0/query_optimizer/compiler.py` & `graphene_django_query_optimizer-0.7.1/query_optimizer/compiler.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.0/query_optimizer/converters.py` & `graphene_django_query_optimizer-0.7.1/query_optimizer/converters.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.0/query_optimizer/fields.py` & `graphene_django_query_optimizer-0.7.1/query_optimizer/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,15 +422,15 @@
     """
 
     def __init__(
         self,
         type_: UnmountedTypeInput,
         /,
         *,
-        args: dict[str, ArgTypeInput],
+        args: dict[str, ArgTypeInput] | None = None,
         **kwargs: Any,
     ) -> None:
         self.optimizer: ManualOptimizerMethod | None = None
         super().__init__(type_, args=args, **kwargs)
 
     def __set_name__(self, object_type: type[DjangoObjectType], name: str) -> None:
         self.name = to_camel_case(name)
```

### Comparing `graphene_django_query_optimizer-0.7.0/query_optimizer/filter.py` & `graphene_django_query_optimizer-0.7.1/query_optimizer/filter.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.0/query_optimizer/filter_info.py` & `graphene_django_query_optimizer-0.7.1/query_optimizer/filter_info.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.0/query_optimizer/optimizer.py` & `graphene_django_query_optimizer-0.7.1/query_optimizer/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,15 @@
     def process_filters(self, input_data: dict[str, Any]) -> dict[str, Any]:
         from graphene_django.filter.fields import convert_enum
 
         return {key: convert_enum(value) for key, value in input_data.items()}
 
     def run_manual_optimizers(self, queryset: QuerySet, filter_info: GraphQLFilterInfo) -> QuerySet:
         for name, func in self.manual_optimizers.items():
-            filters = filter_info["children"][name]["filters"]
+            filters: dict[str, Any] = filter_info.get("children", {}).get(name, {}).get("filters", {})
             queryset = func(queryset, self, **filters)
         return queryset
 
     def pre_compilation(self) -> None:
         object_type: Optional[DjangoObjectType] = get_global_registry().get_type_for_model(self.model)
         if callable(getattr(object_type, "pre_compilation_hook", None)):
             object_type.pre_compilation_hook(self)
```

### Comparing `graphene_django_query_optimizer-0.7.0/query_optimizer/prefetch_hack.py` & `graphene_django_query_optimizer-0.7.1/query_optimizer/prefetch_hack.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.0/query_optimizer/selections.py` & `graphene_django_query_optimizer-0.7.1/query_optimizer/selections.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.0/query_optimizer/settings.py` & `graphene_django_query_optimizer-0.7.1/query_optimizer/settings.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.0/query_optimizer/types.py` & `graphene_django_query_optimizer-0.7.1/query_optimizer/types.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.0/query_optimizer/typing.py` & `graphene_django_query_optimizer-0.7.1/query_optimizer/typing.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.0/query_optimizer/utils.py` & `graphene_django_query_optimizer-0.7.1/query_optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.0/query_optimizer/validators.py` & `graphene_django_query_optimizer-0.7.1/query_optimizer/validators.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.7.0/PKG-INFO` & `graphene_django_query_optimizer-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-query-optimizer
-Version: 0.7.0
+Version: 0.7.1
 Summary: Automatically optimize SQL queries in Graphene-Django schemas.
 Home-page: https://mrthearman.github.io/graphene-django-query-optimizer
 License: MIT
 Keywords: django,graphene,sql,graphql,python,query,optimizer,optimization
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.9,<4
```

