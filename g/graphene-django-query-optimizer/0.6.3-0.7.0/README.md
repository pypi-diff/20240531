# Comparing `tmp/graphene_django_query_optimizer-0.6.3.tar.gz` & `tmp/graphene_django_query_optimizer-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphene_django_query_optimizer-0.6.3.tar", max compression
+gzip compressed data, was "graphene_django_query_optimizer-0.7.0.tar", max compression
```

## Comparing `graphene_django_query_optimizer-0.6.3.tar` & `graphene_django_query_optimizer-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1064 2024-05-27 10:17:01.849435 graphene_django_query_optimizer-0.6.3/LICENSE
--rw-r--r--   0        0        0     3151 2024-05-27 10:17:01.849435 graphene_django_query_optimizer-0.6.3/README.md
--rw-r--r--   0        0        0     6906 2024-05-27 10:17:01.849435 graphene_django_query_optimizer-0.6.3/pyproject.toml
--rw-r--r--   0        0        0      496 2024-05-27 10:17:01.849435 graphene_django_query_optimizer-0.6.3/query_optimizer/__init__.py
--rw-r--r--   0        0        0    11972 2024-05-27 10:17:01.849435 graphene_django_query_optimizer-0.6.3/query_optimizer/ast.py
--rw-r--r--   0        0        0     9013 2024-05-27 10:17:01.849435 graphene_django_query_optimizer-0.6.3/query_optimizer/compiler.py
--rw-r--r--   0        0        0     2847 2024-05-27 10:17:01.849435 graphene_django_query_optimizer-0.6.3/query_optimizer/converters.py
--rw-r--r--   0        0        0      177 2024-05-27 10:17:01.849435 graphene_django_query_optimizer-0.6.3/query_optimizer/errors.py
--rw-r--r--   0        0        0    17282 2024-05-27 10:17:01.849435 graphene_django_query_optimizer-0.6.3/query_optimizer/fields.py
--rw-r--r--   0        0        0     1686 2024-05-27 10:17:01.849435 graphene_django_query_optimizer-0.6.3/query_optimizer/filter.py
--rw-r--r--   0        0        0     5687 2024-05-27 10:17:01.849435 graphene_django_query_optimizer-0.6.3/query_optimizer/filter_info.py
--rw-r--r--   0        0        0    12379 2024-05-27 10:17:01.849435 graphene_django_query_optimizer-0.6.3/query_optimizer/optimizer.py
--rw-r--r--   0        0        0     4130 2024-05-27 10:17:01.849435 graphene_django_query_optimizer-0.6.3/query_optimizer/prefetch_hack.py
--rw-r--r--   0        0        0        0 2024-05-27 10:17:01.849435 graphene_django_query_optimizer-0.6.3/query_optimizer/py.typed
--rw-r--r--   0        0        0     3600 2024-05-27 10:17:01.853435 graphene_django_query_optimizer-0.6.3/query_optimizer/selections.py
--rw-r--r--   0        0        0     2520 2024-05-27 10:17:01.853435 graphene_django_query_optimizer-0.6.3/query_optimizer/settings.py
--rw-r--r--   0        0        0     3212 2024-05-27 10:17:01.853435 graphene_django_query_optimizer-0.6.3/query_optimizer/types.py
--rw-r--r--   0        0        0     3845 2024-05-27 10:17:01.853435 graphene_django_query_optimizer-0.6.3/query_optimizer/typing.py
--rw-r--r--   0        0        0     6842 2024-05-27 10:17:01.853435 graphene_django_query_optimizer-0.6.3/query_optimizer/utils.py
--rw-r--r--   0        0        0     3888 2024-05-27 10:17:01.853435 graphene_django_query_optimizer-0.6.3/query_optimizer/validators.py
--rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/LICENSE
+-rw-r--r--   0        0        0     3151 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/README.md
+-rw-r--r--   0        0        0     6906 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      579 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/query_optimizer/__init__.py
+-rw-r--r--   0        0        0    11972 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/query_optimizer/ast.py
+-rw-r--r--   0        0        0     8533 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/query_optimizer/compiler.py
+-rw-r--r--   0        0        0     2847 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/query_optimizer/converters.py
+-rw-r--r--   0        0        0      177 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/query_optimizer/errors.py
+-rw-r--r--   0        0        0    18385 2024-05-31 08:40:55.656155 graphene_django_query_optimizer-0.7.0/query_optimizer/fields.py
+-rw-r--r--   0        0        0     1686 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/filter.py
+-rw-r--r--   0        0        0     5697 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/filter_info.py
+-rw-r--r--   0        0        0    12382 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/optimizer.py
+-rw-r--r--   0        0        0     4130 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/prefetch_hack.py
+-rw-r--r--   0        0        0        0 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/py.typed
+-rw-r--r--   0        0        0     3600 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/selections.py
+-rw-r--r--   0        0        0     2520 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/settings.py
+-rw-r--r--   0        0        0     3212 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/types.py
+-rw-r--r--   0        0        0     4075 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/typing.py
+-rw-r--r--   0        0        0     6842 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/utils.py
+-rw-r--r--   0        0        0     3888 2024-05-31 08:40:55.660155 graphene_django_query_optimizer-0.7.0/query_optimizer/validators.py
+-rw-r--r--   0        0        0     4694 1970-01-01 00:00:00.000000 graphene_django_query_optimizer-0.7.0/PKG-INFO
```

### Comparing `graphene_django_query_optimizer-0.6.3/LICENSE` & `graphene_django_query_optimizer-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.3/README.md` & `graphene_django_query_optimizer-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.3/pyproject.toml` & `graphene_django_query_optimizer-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphene-django-query-optimizer"
-version = "0.6.3"
+version = "0.7.0"
 description = "Automatically optimize SQL queries in Graphene-Django schemas."
 authors = [
     "Matti Lamppu <lamppu.matti.akseli@gmail.com>",
 ]
 packages = [
     { include = "query_optimizer" },
 ]
```

### Comparing `graphene_django_query_optimizer-0.6.3/query_optimizer/ast.py` & `graphene_django_query_optimizer-0.7.0/query_optimizer/ast.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.3/query_optimizer/compiler.py` & `graphene_django_query_optimizer-0.7.0/query_optimizer/compiler.py`

 * *Files 7% similar despite different names*

```diff
@@ -193,28 +193,16 @@
         # `RelatedField`, `DjangoListField` and `DjangoConnectionField` can define a
         # 'field_name' attribute to specify the actual model field name.
         actual_field_name: Optional[str] = getattr(field, "field_name", None)
         if actual_field_name is not None:
             self.to_attr = field_name
             return self.handle_model_field(field_type, field_node, actual_field_name)
 
-        from .fields import AnnotatedField, MultiField, PreResolvingField
-
-        if isinstance(field, AnnotatedField):
-            self.optimizer.annotations[to_snake_case(field.name)] = field.expression
-            if field.aliases is not None:
-                self.optimizer.aliases.update(field.aliases)
-            return None
-
-        if isinstance(field, MultiField):
-            self.optimizer.only_fields.extend(field.fields)
-            return None
-
-        if isinstance(field, PreResolvingField):
-            self.optimizer.pre_resolvers[to_snake_case(field.name)] = field.pre_resolver
+        if hasattr(field, "optimizer_hook") and callable(field.optimizer_hook):
+            field.optimizer_hook(self)
             return None
 
         return None  # pragma: no cover
 
     @contextlib.contextmanager
     def use_optimizer(self, optimizer: QueryOptimizer) -> None:
         orig_optimizer = self.optimizer
```

### Comparing `graphene_django_query_optimizer-0.6.3/query_optimizer/converters.py` & `graphene_django_query_optimizer-0.7.0/query_optimizer/converters.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.3/query_optimizer/fields.py` & `graphene_django_query_optimizer-0.7.0/query_optimizer/fields.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,38 +24,41 @@
     from django.db import models
     from django.db.models import Model, QuerySet
     from django.db.models.manager import Manager
     from graphene.relay.connection import Connection
     from graphql_relay import EdgeType
     from graphql_relay.connection.connection import ConnectionType
 
+    from .optimizer import QueryOptimizer
     from .types import DjangoObjectType
     from .typing import (
         Any,
         ArgTypeInput,
         Callable,
         ConnectionResolver,
         ExpressionKind,
         GQLInfo,
         Iterable,
+        ManualOptimizerMethod,
         ModelResolver,
         ObjectTypeInput,
         Optional,
         QuerySetResolver,
         Type,
         Union,
         UnmountedTypeInput,
     )
 
 __all__ = [
+    "AnnotatedField",
     "DjangoConnectionField",
     "DjangoListField",
-    "RelatedField",
-    "AnnotatedField",
+    "ManuallyOptimizedField",
     "MultiField",
+    "RelatedField",
 ]
 
 
 class RelatedField(graphene.Field):
     """Field for `to-one` related models with default resolvers."""
 
     def __init__(
@@ -349,32 +352,41 @@
 
     def __init__(
         self,
         type_: UnmountedTypeInput,
         /,
         expression: ExpressionKind,
         aliases: Optional[dict[str, ExpressionKind]] = None,
+        extra_annotations: Optional[dict[str, ExpressionKind]] = None,
         **kwargs: Any,
     ) -> None:
         self.expression = expression
         self.aliases = aliases
+        self.extra_annotations = extra_annotations
         super().__init__(type_, **kwargs)
 
     def __set_name__(self, owner: type[DjangoObjectType], name: str) -> None:
         self.name = to_camel_case(name)
 
     def wrap_resolve(self, parent_resolver: Callable[..., Any]) -> Callable[..., Any]:
         # `parent_resolver` is either a `resolve_{self.name}` method defined
         # on the owner class, or a partial of `dict_or_attr_resolver`.
         self.resolver = parent_resolver
         return self.annotation_resolver
 
     def annotation_resolver(self, root: Model, info: GQLInfo, **kwargs: Any) -> Any:
         return self.resolver(root, info, **kwargs)
 
+    def optimizer_hook(self, compiler: OptimizationCompiler) -> None:
+        compiler.optimizer.annotations[to_snake_case(self.name)] = self.expression
+        if self.aliases is not None:
+            compiler.optimizer.aliases.update(self.aliases)
+        if self.extra_annotations is not None:  # pragma: no cover
+            compiler.optimizer.annotations.update(self.extra_annotations)
+
 
 class MultiField(graphene.Field):
     """Field that requires multiple model fields to resolve. Does not support related lookups."""
 
     def __init__(self, type_: UnmountedTypeInput, /, fields: Iterable[str], **kwargs: Any) -> None:
         self.fields = fields
         super().__init__(type_, **kwargs)
@@ -387,50 +399,58 @@
         # on the owner class, or a partial of `dict_or_attr_resolver`.
         self.resolver = parent_resolver
         return self.multi_field_resolver
 
     def multi_field_resolver(self, root: Model, info: GQLInfo, **kwargs: Any) -> Any:
         return self.resolver(root, info, **kwargs)
 
+    def optimizer_hook(self, compiler: OptimizationCompiler) -> None:
+        compiler.optimizer.only_fields.extend(self.fields)
+
 
-class PreResolvingField(graphene.Field):
+class ManuallyOptimizedField(graphene.Field):
     """
-    Field that has a pre-resolving step.
+    Field that is manually optimized using a method defined on the object type this field is on.
 
-    Must define a `pre_resolve_{name}(queryset, info, **kwargs)` staticmethod on the object type,
-    where `{name}` is the name of the field defined on the object type, and `kwargs`
-    are the values of 'args' defined on this field.
+    Must define a `optimize_{name}` staticmethod on the object type, where `{name}` is the name
+    of the field defined on the object type. This method takes the following arguments:
 
-    The optimizer will run pre-resolving methods as the last filtering step.
+    - `queryset`: The QuerySet to optimize.
+    - `optimizer`: The QueryOptimizer instance that is performing the optimizations.
+    - `**kwargs`: Filters passed to the field (see `args` in __init__).
+
+    The optimizer will run these methods as the last filtering step.
     """
 
     def __init__(
         self,
         type_: UnmountedTypeInput,
         /,
         *,
         args: dict[str, ArgTypeInput],
         **kwargs: Any,
     ) -> None:
+        self.optimizer: ManualOptimizerMethod | None = None
         super().__init__(type_, args=args, **kwargs)
 
-    def __set_name__(self, owner: type[DjangoObjectType], name: str) -> None:
-        self.owner = owner
+    def __set_name__(self, object_type: type[DjangoObjectType], name: str) -> None:
         self.name = to_camel_case(name)
-
-    def pre_resolver(self, queryset: QuerySet, info: GQLInfo, **kwargs: Any) -> QuerySet:
-        name = to_snake_case(self.name)
-        resolver_name = f"pre_resolve_{name}"
-        resolver: Callable[..., QuerySet] | None = getattr(self.owner, resolver_name, None)
-        if resolver is None:  # pragma: no cover
-            msg = f"Pre-resolver method '{resolver_name}' missing from '{self.owner}'."
+        resolver_name = f"optimize_{name}"
+        self.optimizer = getattr(object_type, resolver_name, None)
+        if self.optimizer is None:  # pragma: no cover
+            msg = f"Optimizer method '{resolver_name}' missing from '{object_type}'."
             raise AttributeError(msg)
-        return resolver(queryset, info, **kwargs)
+
+    def optimize(self, queryset: QuerySet, optimizer: QueryOptimizer, **kwargs: Any) -> QuerySet:
+        return self.optimizer(queryset, optimizer, **kwargs)
 
     def wrap_resolve(self, parent_resolver: Callable[..., Any]) -> Callable[..., Any]:
         # `parent_resolver` is either a `resolve_{self.name}` method defined
         # on the owner class, or a partial of `dict_or_attr_resolver`.
         self.resolver = parent_resolver
         return self.field_resolver
 
     def field_resolver(self, root: Model, info: GQLInfo, **kwargs: Any) -> Any:
         return self.resolver(root, info, **kwargs)
+
+    def optimizer_hook(self, compiler: OptimizationCompiler) -> None:
+        compiler.optimizer.manual_optimizers[to_snake_case(self.name)] = self.optimize
```

### Comparing `graphene_django_query_optimizer-0.6.3/query_optimizer/filter.py` & `graphene_django_query_optimizer-0.7.0/query_optimizer/filter.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.3/query_optimizer/filter_info.py` & `graphene_django_query_optimizer-0.7.0/query_optimizer/filter_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,19 +101,19 @@
 
     def handle_query_class(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None:
         self.add_filter_info(field_type, field_node)
         with self.child_filter_info(field_node):
             super().handle_query_class(field_type, field_node)
 
     def handle_custom_field(self, field_type: GrapheneObjectType, field_node: FieldNode) -> None:
-        from .fields import PreResolvingField
+        from .fields import ManuallyOptimizedField
 
         field_name = to_snake_case(field_node.name.value)
         field = getattr(field_type.graphene_type, field_name, None)
-        if isinstance(field, PreResolvingField):
+        if isinstance(field, ManuallyOptimizedField):
             self.add_filter_info(field_type, field_node)
 
     def handle_to_one_field(
         self,
         field_type: GrapheneObjectType,
         field_node: FieldNode,
         related_field: ToOneField,
```

### Comparing `graphene_django_query_optimizer-0.6.3/query_optimizer/optimizer.py` & `graphene_django_query_optimizer-0.7.0/query_optimizer/optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.info = info
         self.only_fields: list[str] = []
         self.related_fields: list[str] = []
         self.aliases: dict[str, ExpressionKind] = {}
         self.annotations: dict[str, ExpressionKind] = {}
         self.select_related: dict[str, QueryOptimizer] = {}
         self.prefetch_related: dict[str, QueryOptimizer] = {}
-        self.pre_resolvers: dict[str, QuerySetResolver] = {}
+        self.manual_optimizers: dict[str, QuerySetResolver] = {}
         self.total_count: bool = False
         self.name = name
         self.parent: QueryOptimizer | None = parent
 
     def optimize_queryset(
         self,
         queryset: QuerySet[TModel],
@@ -103,15 +103,15 @@
             )
             if not filterset.is_valid():  # pragma: no cover
                 raise ValidationError(filterset.form.errors.as_json())
 
             queryset = filterset.qs
 
         queryset = self.get_filtered_queryset(queryset)
-        queryset = self.run_pre_resolvers(queryset, filter_info)
+        queryset = self.run_manual_optimizers(queryset, filter_info)
 
         if results.select_related:
             queryset = queryset.select_related(*results.select_related)
         if results.prefetch_related:
             queryset = queryset.prefetch_related(*results.prefetch_related)
         if not optimizer_settings.DISABLE_ONLY_FIELDS_OPTIMIZATION and (results.only_fields or results.related_fields):
             queryset = queryset.only(*results.only_fields, *results.related_fields)
@@ -273,18 +273,18 @@
         return queryset  # pragma: no cover
 
     def process_filters(self, input_data: dict[str, Any]) -> dict[str, Any]:
         from graphene_django.filter.fields import convert_enum
 
         return {key: convert_enum(value) for key, value in input_data.items()}
 
-    def run_pre_resolvers(self, queryset: QuerySet, filter_info: GraphQLFilterInfo) -> QuerySet:
-        for name, resolver in self.pre_resolvers.items():
+    def run_manual_optimizers(self, queryset: QuerySet, filter_info: GraphQLFilterInfo) -> QuerySet:
+        for name, func in self.manual_optimizers.items():
             filters = filter_info["children"][name]["filters"]
-            queryset = resolver(queryset, self.info, **filters)
+            queryset = func(queryset, self, **filters)
         return queryset
 
     def pre_compilation(self) -> None:
         object_type: Optional[DjangoObjectType] = get_global_registry().get_type_for_model(self.model)
         if callable(getattr(object_type, "pre_compilation_hook", None)):
             object_type.pre_compilation_hook(self)
```

### Comparing `graphene_django_query_optimizer-0.6.3/query_optimizer/prefetch_hack.py` & `graphene_django_query_optimizer-0.7.0/query_optimizer/prefetch_hack.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.3/query_optimizer/selections.py` & `graphene_django_query_optimizer-0.7.0/query_optimizer/selections.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.3/query_optimizer/settings.py` & `graphene_django_query_optimizer-0.7.0/query_optimizer/settings.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.3/query_optimizer/types.py` & `graphene_django_query_optimizer-0.7.0/query_optimizer/types.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.3/query_optimizer/typing.py` & `graphene_django_query_optimizer-0.7.0/query_optimizer/typing.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 
 if TYPE_CHECKING:
     from django.contrib.auth.models import AnonymousUser, User
     from django.contrib.contenttypes.fields import GenericForeignKey, GenericRelation
     from django.db.models.sql import Query
     from django_filters import FilterSet
 
+    from query_optimizer.optimizer import QueryOptimizer
+
 __all__ = [
     "Any",
     "ArgTypeInput",
     "Callable",
     "cast",
     "Collection",
     "ConnectionResolver",
@@ -73,14 +75,15 @@
     "Generic",
     "GQLInfo",
     "GRAPHQL_BUILTIN",
     "GraphQLFilterInfo",
     "Hashable",
     "Iterable",
     "Literal",
+    "ManualOptimizerMethod",
     "ModelField",
     "ModelResolver",
     "NamedTuple",
     "ObjectTypeInput",
     "OptimizedDjangoOptions",
     "Optional",
     "overload",
@@ -152,7 +155,11 @@
         self,
         query: Query,
         allow_joins: bool,  # noqa: FBT001
         reuse: set[str] | None,
         summarize: bool,  # noqa: FBT001
         for_save: bool,  # noqa: FBT001
     ) -> ExpressionKind: ...
+
+
+class ManualOptimizerMethod(Protocol):
+    def __call__(self, queryset: QuerySet, optimizer: QueryOptimizer, **kwargs: Any) -> QuerySet: ...
```

### Comparing `graphene_django_query_optimizer-0.6.3/query_optimizer/utils.py` & `graphene_django_query_optimizer-0.7.0/query_optimizer/utils.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.3/query_optimizer/validators.py` & `graphene_django_query_optimizer-0.7.0/query_optimizer/validators.py`

 * *Files identical despite different names*

### Comparing `graphene_django_query_optimizer-0.6.3/PKG-INFO` & `graphene_django_query_optimizer-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphene-django-query-optimizer
-Version: 0.6.3
+Version: 0.7.0
 Summary: Automatically optimize SQL queries in Graphene-Django schemas.
 Home-page: https://mrthearman.github.io/graphene-django-query-optimizer
 License: MIT
 Keywords: django,graphene,sql,graphql,python,query,optimizer,optimization
 Author: Matti Lamppu
 Author-email: lamppu.matti.akseli@gmail.com
 Requires-Python: >=3.9,<4
```

