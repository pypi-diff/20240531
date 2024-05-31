# Comparing `tmp/typegraph3-0.1.2rc1.tar.gz` & `tmp/typegraph3-0.1.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typegraph3-0.1.2rc1.tar", last modified: Thu May 30 12:52:29 2024, max compression
+gzip compressed data, was "typegraph3-0.1.2rc2.tar", last modified: Fri May 31 13:08:03 2024, max compression
```

## Comparing `typegraph3-0.1.2rc1.tar` & `typegraph3-0.1.2rc2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/LICENSE
--rw-r--r--   0        0        0     6378 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/README.md
--rw-r--r--   0        0        0      515 2024-05-30 12:52:29.061537 typegraph3-0.1.2rc1/pyproject.toml
--rw-r--r--   0        0        0      165 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/src/typegraph/__init__.py
--rw-r--r--   0        0        0      146 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/src/typegraph/converter/__init__.py
--rw-r--r--   0        0        0    20373 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/src/typegraph/converter/base.py
--rw-r--r--   0        0        0     7807 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/src/typegraph/converter/typevar.py
--rw-r--r--   0        0        0     4916 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/src/typegraph/type_utils.py
--rw-r--r--   0        0        0        0 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/tests/__init__.py
--rw-r--r--   0        0        0    17209 2024-05-30 12:52:12.273436 typegraph3-0.1.2rc1/tests/test_switch.py
--rw-r--r--   0        0        0     6680 1970-01-01 00:00:00.000000 typegraph3-0.1.2rc1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-31 13:07:47.511249 typegraph3-0.1.2rc2/LICENSE
+-rw-r--r--   0        0        0     6378 2024-05-31 13:07:47.511249 typegraph3-0.1.2rc2/README.md
+-rw-r--r--   0        0        0      515 2024-05-31 13:08:03.431186 typegraph3-0.1.2rc2/pyproject.toml
+-rw-r--r--   0        0        0      165 2024-05-31 13:07:47.511249 typegraph3-0.1.2rc2/src/typegraph/__init__.py
+-rw-r--r--   0        0        0      146 2024-05-31 13:07:47.515249 typegraph3-0.1.2rc2/src/typegraph/converter/__init__.py
+-rw-r--r--   0        0        0    22791 2024-05-31 13:07:47.515249 typegraph3-0.1.2rc2/src/typegraph/converter/base.py
+-rw-r--r--   0        0        0     8854 2024-05-31 13:07:47.515249 typegraph3-0.1.2rc2/src/typegraph/converter/typevar.py
+-rw-r--r--   0        0        0     5800 2024-05-31 13:07:47.515249 typegraph3-0.1.2rc2/src/typegraph/type_utils.py
+-rw-r--r--   0        0        0        0 2024-05-31 13:07:47.515249 typegraph3-0.1.2rc2/tests/__init__.py
+-rw-r--r--   0        0        0    18972 2024-05-31 13:07:47.515249 typegraph3-0.1.2rc2/tests/test_switch.py
+-rw-r--r--   0        0        0     6680 1970-01-01 00:00:00.000000 typegraph3-0.1.2rc2/PKG-INFO
```

### Comparing `typegraph3-0.1.2rc1/LICENSE` & `typegraph3-0.1.2rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `typegraph3-0.1.2rc1/README.md` & `typegraph3-0.1.2rc2/README.md`

 * *Files identical despite different names*

### Comparing `typegraph3-0.1.2rc1/pyproject.toml` & `typegraph3-0.1.2rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "typegraph3"
-version = "0.1.2rc1"
+version = "0.1.2rc2"
 description = "Type Auto Switch"
 authors = [
     { name = "luxuncang", email = "luxuncang@qq.com" },
 ]
 dependencies = [
     "typing-inspect>=0.9.0",
     "networkx>=3.3",
```

### Comparing `typegraph3-0.1.2rc1/src/typegraph/converter/base.py` & `typegraph3-0.1.2rc2/src/typegraph/converter/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,36 +6,42 @@
     Callable,
     List,
     Tuple,
     Dict,
     Set,
     Iterable,
     Iterator,
+    Sequence,
+    MutableSequence,
     cast,
     Type,
     Awaitable,
     Any,
     Optional,
+    Mapping,
+    MutableMapping,
     get_type_hints,
-    Generic,
+    is_typeddict,
 )
 from functools import wraps, reduce
 
 import networkx as nx
 from typing_extensions import get_args, get_origin
 from typing_inspect import is_union_type, get_generic_type
-from typeguard import check_type, TypeCheckError, CollectionCheckStrategy
+from typeguard import check_type, CollectionCheckStrategy
 
 from .typevar import iter_deep_type, gen_typevar_model, extract_typevar_mapping
 from ..type_utils import (
     is_structural_type,
     deep_type,
     is_protocol_type,
     check_protocol_type,
     get_subclass_types,
+    get_connected_subgraph,
+    iter_type_args,
 )
 
 
 T = TypeVar("T")
 In = TypeVar("In", contravariant=True)
 Out = TypeVar("Out")
 P = ParamSpec("P")
@@ -46,14 +52,15 @@
 
     def __init__(self):
         self.G = nx.DiGraph()
         self.sG = nx.DiGraph()
         self.pG = nx.DiGraph()
         self.tG = nx.DiGraph()
         self.pmG = nx.DiGraph()
+        self.qG = nx.DiGraph()
         TypeConverter.instances.append(self)
 
     def get_graph(
         self,
         sub_class: bool = False,
         protocol: bool = False,
         combos: Optional[list[nx.DiGraph]] = None,
@@ -92,40 +99,62 @@
                 in_type,
                 p_type,
                 converter=lambda x: x,
                 line=False,
                 metadata={"protocol": True},
             )
         for p_type in self.get_protocol_types(out_type):
-            if out_type == str:
-                print(p_type, in_type, out_type, converter)
             self.pG.add_edge(
                 out_type,
                 p_type,
                 converter=lambda x: x,
                 line=False,
                 metadata={"protocol": True},
             )
 
     def _gen_graph(self, in_type: Type[In], out_type: Type[Out]):
         tmp_G = nx.DiGraph()
         im = gen_typevar_model(in_type)
         om = gen_typevar_model(out_type)
+
+        def _gen_sub_graph(mapping, node):
+            for su, sv, sc in get_connected_subgraph(self.tG, node).edges(data=True):
+                tmp_G.add_edge(su.get_instance(mapping), sv.get_instance(mapping), **sc)
+
         for u, v, c in self.tG.edges(data=True):
             um = gen_typevar_model(u)
             vm = gen_typevar_model(v)
             combos = [(um, im), (vm, im), (um, om), (vm, om)]
             for t, i in combos:
                 try:
                     mapping = extract_typevar_mapping(t, i)
                     tmp_G.add_edge(
                         um.get_instance(mapping), vm.get_instance(mapping), **c
                     )
+                    _gen_sub_graph(mapping, t)
                 except Exception:
                     ...
+
+            for su, sv, sc in self.G.edges(data=True):
+                su_m = gen_typevar_model(su)
+                for arg in iter_type_args(su_m):
+                    try:
+                        mapping = extract_typevar_mapping(um, arg)
+                        sub_m = su_m.replace_args(
+                            arg,
+                            gen_typevar_model(vm.get_instance(mapping)),  # type: ignore
+                        ).get_instance()
+                        tmp_G.add_edge(
+                            sub_m,
+                            sv,
+                            **sc,
+                        )
+                    except Exception:
+                        ...
+        self.qG = nx.compose(self.qG, tmp_G)
         return tmp_G
 
     def register_generic_converter(self, input_type: Type, out_type: Type):
         def decorator(func: Callable[P, T]):
             self.tG.add_edge(input_type, out_type, converter=func)
             return func
 
@@ -329,14 +358,16 @@
                     res = tuple(map(_iter_func, input_value))
                 elif in_origin == set or out_origin == Set:
                     res = set(map(_iter_func, input_value))
                 elif out_origin in (Iterable, Iterator):
                     res = map(_iter_func, input_value)
                 elif in_origin == dict or out_origin == Dict:
                     res = dict(map(__iter_func_dict, input_value.items()))
+                elif out_origin in (Mapping, MutableMapping):
+                    res = dict(map(__iter_func_dict, input_value.items()))
                 else:
                     raise ValueError(
                         f"Unsupported structural_type {input_type} to {out_type}"
                     )
                 return cast(Out, res)
 
         raise ValueError(f"No converter registered for {input_type} to {out_type}")
@@ -408,14 +439,19 @@
                 elif out_origin in (Iterable, Iterator):
                     res = await asyncio.gather(*map(_iter_func, input_value))
                 elif in_origin == dict or out_origin == Dict:
                     items = await asyncio.gather(
                         *map(__iter_func_dict, input_value.items())
                     )
                     res = dict(items)
+                elif out_origin in (Mapping, MutableMapping):
+                    items = await asyncio.gather(
+                        *map(__iter_func_dict, input_value.items())
+                    )
+                    res = dict(items)
                 else:
                     raise ValueError(
                         f"Unsupported structural_type {input_type} to {out_type}"
                     )
                 return cast(Out, res)
         raise ValueError(f"No converter registered for {input_type} to {out_type}")
 
@@ -493,25 +529,46 @@
 
     def get_edges(self, sub_class: bool = False, protocol: bool = False):
         for edge in self.get_graph(sub_class=sub_class, protocol=protocol).edges(
             data=True
         ):
             yield edge
 
-    def show_mermaid_graph(self, sub_class: bool = False, protocol: bool = False):
+    def show_mermaid_graph(
+        self, sub_class: bool = False, protocol: bool = False, full: bool = False
+    ):
         from IPython.display import display, Markdown
+        import typing
+
+        nodes = []
+
+        def get_name(cls):
+            if type(cls) in (typing._GenericAlias, typing.GenericAlias):  # type: ignore
+                return str(cls)
+            elif hasattr(cls, "__name__"):
+                return cls.__name__
+            return str(cls)
+
+        def get_node_name(cls):
+            return f"node{nodes.index(cls)}"
 
         text = "```mermaid\ngraph TD;\n"
-        for edge in self.get_edges(sub_class=sub_class, protocol=protocol):
-            line_style = "--" if edge[2]["line"] else "-.-"
-            text += f"{edge[0].__name__}{line_style}>{edge[1].__name__}\n"
+        for edge in self.get_graph(
+            sub_class=sub_class, protocol=protocol, combos=[self.qG] if full else None
+        ).edges(data=True):
+            if edge[0] not in nodes:
+                nodes.append(edge[0])
+            if edge[1] not in nodes:
+                nodes.append(edge[1])
+            line_style = "--" if edge[2].get("line", False) else "-.-"
+            text += f'{get_node_name(edge[0])}["{get_name(edge[0])}"] {line_style}> {get_node_name(edge[1])}["{get_name(edge[1])}"]\n'
         text += "```"
 
         display(Markdown(text))
-        return text
+        # return text
 
     def get_all_paths(
         self,
         in_type: Type[In],
         out_type: Type[Out],
         sub_class: bool = False,
         protocol: bool = False,
@@ -562,17 +619,25 @@
     ):
         nodes = set()
         G = self.get_graph(sub_class=sub_class, protocol=protocol)
 
         for edge in G.edges():
             if edge[0] in nodes:
                 continue
-            nodes.add(edge[0])
-            try:
-                check_type(
-                    input_value,
-                    edge[0],
-                    collection_check_strategy=CollectionCheckStrategy.ALL_ITEMS,
-                )
-            except Exception:
-                continue
-            yield edge[0]
+            if get_origin(edge[0]) in (
+                Iterable,
+                Iterator,
+                Mapping,
+                MutableMapping,
+                Sequence,
+                MutableSequence,
+            ) or is_typeddict(edge[0]):
+                nodes.add(edge[0])
+                try:
+                    check_type(
+                        input_value,
+                        edge[0],
+                        collection_check_strategy=CollectionCheckStrategy.ALL_ITEMS,
+                    )
+                except Exception:
+                    continue
+                yield edge[0]
```

### Comparing `typegraph3-0.1.2rc1/src/typegraph/converter/typevar.py` & `typegraph3-0.1.2rc2/src/typegraph/converter/typevar.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from __future__ import annotations
 from typing import (
     TypeVar,
     List,
     Type,
     Any,
     Optional,
 )
 from dataclasses import dataclass
 from collections import deque
 
 from typing_extensions import get_args
 from typing_inspect import is_typevar
 
 from ..type_utils import (
-    get_origin as get_real_origin,
+    get_real_origin,
     generate_type,
 )
 
 In = TypeVar("In", contravariant=True)
 
 
 @dataclass
@@ -50,14 +51,41 @@
                 args_list.append(arg.get_instance(instance))
             elif isinstance(arg, list):
                 args_list.append([a.get_instance(instance) for a in arg])
             else:
                 raise ValueError("Invalid TypeVarModel")
         return generate_type(generic, args_list)
 
+    def replace_args(self, source: TypeVarModel, target: TypeVarModel) -> 'TypeVarModel':
+        if self.args is None:
+            return TypeVarModel(self.origin)
+
+        new_args = []
+        for arg in self.args:
+            if isinstance(arg, TypeVarModel):
+                if arg == source:
+                    new_args.append(target)
+                else:
+                    new_args.append(arg.replace_args(source, target))
+            elif isinstance(arg, list):
+                new_list = []
+                for item in arg:
+                    if isinstance(item, TypeVarModel):
+                        if item == source:
+                            new_list.append(target)
+                        else:
+                            new_list.append(item.replace_args(source, target))
+                    else:
+                        new_list.append(item)
+                new_args.append(new_list)
+            else:
+                new_args.append(arg)
+        
+        return TypeVarModel(self.origin, new_args)
+
     def depth_first_traversal(self, parent=None, parent_arg_index=None, depth=1):
         if self.args:
             for i, arg in enumerate(self.args):
                 if isinstance(arg, TypeVarModel):
                     yield from arg.depth_first_traversal(self, i, depth + 1)
                 elif isinstance(arg, list):
                     for j, a in enumerate(arg):
```

### Comparing `typegraph3-0.1.2rc1/src/typegraph/type_utils.py` & `typegraph3-0.1.2rc2/src/typegraph/type_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 import types
 import typing
+import networkx as nx
 
-from typing import (
-    Union,
-    List,
-    Callable,
-    Any,
-    runtime_checkable,
-    Type,
-)
+from typing import Union, List, Callable, Any, runtime_checkable, Type, get_args
 from typing_extensions import get_type_hints
 from typing_inspect import get_generic_type
 
 
-def get_origin(tp):
+def get_real_origin(tp):
     """Get the unsubscripted version of a type.
 
     This supports generic types, Callable, Tuple, Union, Literal, Final, ClassVar
     and Annotated. Return None for unsupported types. Examples::
 
         get_origin(Literal[42]) is Literal
         get_origin(int) is None
@@ -33,30 +27,30 @@
     if isinstance(tp, typing._GenericAlias):  # type: ignore
         if isinstance(tp._name, str) and getattr(typing, tp._name, None):
             return getattr(typing, tp._name)
         return tp.__origin__
     if isinstance(
         tp,
         (
-            typing._BaseGenericAlias, # type: ignore
+            typing._BaseGenericAlias,  # type: ignore
             typing.GenericAlias,  # type: ignore
             typing.ParamSpecArgs,
             typing.ParamSpecKwargs,
         ),
     ):
         return tp.__origin__
     if tp is typing.Generic:
         return typing.Generic
     if isinstance(tp, types.UnionType):
         return types.UnionType
     return None
 
 
 def is_structural_type(tp):
-    if get_origin(tp):
+    if get_real_origin(tp):
         return True
     return False
 
 
 def is_protocol_type(tp):
     return hasattr(tp, "_is_protocol") and tp._is_protocol
 
@@ -151,8 +145,44 @@
     return generic[tuple(instance)]
 
 
 def get_subclass_types(cls: Type):
     if hasattr(cls, "__subclasses__"):
         for subclass in cls.__subclasses__():
             yield subclass
-            yield from get_subclass_types(subclass)
+            yield from get_subclass_types(subclass)
+
+
+def get_connected_nodes(graph, node):
+    if node not in graph:
+        return set()
+
+    # 获取正向连通的节点
+    successors = set(nx.descendants(graph, node))
+
+    # 获取逆向连通的节点
+    predecessors = set(nx.ancestors(graph, node))
+
+    # 合并所有连通的节点
+    connected_nodes = successors | predecessors | {node}
+
+    return connected_nodes
+
+
+def get_connected_subgraph(graph, node):
+    connected_nodes = get_connected_nodes(graph, node)
+    subgraph = graph.subgraph(connected_nodes).copy()
+    return subgraph
+
+
+def iter_type_args(tp):
+    args = tp.args
+    if args:
+        for arg in args:
+            if isinstance(arg, list):
+                for i in arg:
+                    yield i
+                    yield from iter_type_args(i)
+            else:
+                yield arg
+                yield from iter_type_args(arg)
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `typegraph3-0.1.2rc1/tests/test_switch.py` & `typegraph3-0.1.2rc2/tests/test_switch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import unittest
 import asyncio
-from typing import TypeVar
+from typing import TypeVar, Generic
 
 from typegraph.converter.base import TypeConverter
 
 K = TypeVar("K")
 V = TypeVar("V")
 
 
@@ -225,18 +225,14 @@
 
         class Test:
             def __init__(self, t):
                 self.t = t
 
         class Test2(int): ...
 
-        class Test3: ...
-
-        class Test4: ...
-
         @t.register_converter(str, int)
         def str_to_int(input_value):
             return int(input_value)
 
         @t.register_converter(int, str)
         def int_to_str(input_value):
             return str(input_value)
@@ -259,16 +255,16 @@
         def Test_to_float(input_value):
             return float(input_value.t)
 
         @t.register_converter(str, float)
         def str_to_float(input_value):
             return float(input_value)
 
-        @self.converter.async_register_converter(dict[K,V], dict[V,K])
-        async def reverse_dict(d: dict[K,V]) -> dict[V,K]:
+        @self.converter.async_register_converter(dict[K, V], dict[V, K])
+        async def reverse_dict(d: dict[K, V]) -> dict[V, K]:
             return {v: k for k, v in d.items()}
 
         @self.converter.auto_convert(localns=locals())
         def test_float_to_str(x: Test):
             return x.t
 
         @self.converter.auto_convert(sub_class=True)
@@ -287,18 +283,14 @@
         def test_structural(x: list[str]):
             return x
 
         @self.converter.auto_convert()
         def test_next_structural(x: list[dict[str, int]]):
             return x
 
-        @self.converter.auto_convert()
-        def test_structural_dict(x: list[dict[str, int]]):
-            return x
-
         result = test_float_to_str("10")
         self.assertEqual(result, "10")
 
         result = test_switch(Test("10.0"))
         self.assertEqual(result, "10.0")
 
         result = add_one(10)
@@ -313,16 +305,15 @@
         result = test_switch(Test2(10))
         self.assertEqual(result, "10")
 
         result = test_structural([1, 2, 3])
         self.assertEqual(result, ["1", "2", "3"])
 
         result = test_next_structural([{1: "1"}, {2: "2"}, {3: "3"}])
-        self.assertEqual(result, [{'1': 1}, {'2': 2}, {'3': 3}])
-
+        self.assertEqual(result, [{"1": 1}, {"2": 2}, {"3": 3}])
 
     def test_auto_convert_protocol(self):
         from typing import Protocol, TypedDict
         from dataclasses import dataclass
 
         t = self.converter
 
@@ -387,14 +378,43 @@
 
         result = test(d)
         self.assertEqual(result, "John 123 123")
 
         result = tests([d])
         self.assertEqual(result, ["John 123 123"])
 
+    def test_auto_convert_generic(self):
+        t = self.converter
+
+        class A: ...
+
+        class B(Generic[K, V]): ...
+
+        @t.register_converter(list[dict[str, int]], A)
+        def convert_list_dict_to_a(data: list[dict[str, int]]):
+            return A()
+
+        @t.register_generic_converter(dict[K, V], dict[V, K])  # type: ignore
+        def convert_dict(data: dict[K, V]):
+            return {v: k for k, v in data.items()}
+
+        @t.register_generic_converter(dict[V, K], B[V, K])  # type: ignore
+        def convert_dict_to_b(data: dict[V, K]):
+            return B[V, K]()
+
+        @t.auto_convert(localns=locals())
+        def test_generic(a: "B[str, int]"):
+            return a
+
+        result = test_generic({1: "1", 2: "2"})
+        self.assertIsInstance(result, B)
+
+        result = test_generic({"1": 1, "2": 2})
+        self.assertIsInstance(result, B)
+
     def test_async_auto_convert(self):
         t = self.converter
 
         class Test:
             def __init__(self, t):
                 self.t = t
 
@@ -551,10 +571,42 @@
             self.assertEqual(result, "John 123 123")
 
             result = await tests([d])
             self.assertEqual(result, ["John 123 123"])
 
         asyncio.run(test_async_conversion_protocol())
 
+    def test_async_auto_convert_generic(self):
+        t = self.converter
+
+        class A: ...
+
+        class B(Generic[K, V]): ...
+
+        @t.register_converter(list[dict[str, int]], A)
+        def convert_list_dict_to_a(data: list[dict[str, int]]):
+            return A()
+
+        @t.register_generic_converter(dict[K, V], dict[V, K])  # type: ignore
+        def convert_dict(data: dict[K, V]):
+            return {v: k for k, v in data.items()}
+
+        @t.register_generic_converter(dict[V, K], B[V, K])  # type: ignore
+        def convert_dict_to_b(data: dict[V, K]):
+            return B[V, K]()
+
+        @t.auto_convert(localns=locals())
+        async def test_generic(a: "B[str, int]"):
+            return a
+
+        async def test_async_auto_convert_generic():
+            result = await test_generic({1: "1", 2: "2"})
+            self.assertIsInstance(result, B)
+
+            result = await test_generic({"1": 1, "2": 2})
+            self.assertIsInstance(result, B)
+
+        asyncio.run(test_async_auto_convert_generic())
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `typegraph3-0.1.2rc1/PKG-INFO` & `typegraph3-0.1.2rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typegraph3
-Version: 0.1.2rc1
+Version: 0.1.2rc2
 Summary: Type Auto Switch
 Author-Email: luxuncang <luxuncang@qq.com>
 License: MIT
 Requires-Python: >=3.10
 Requires-Dist: typing-inspect>=0.9.0
 Requires-Dist: networkx>=3.3
 Requires-Dist: typeguard>=4.3.0
```

