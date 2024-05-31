# Comparing `tmp/baml_py-0.32.0-cp38-abi3-win_amd64.whl.zip` & `tmp/baml_py-0.32.1-cp38-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 4454144 bytes, number of entries: 13
--rw-r--r--  4.6 unx      354 b- defN 24-May-31 08:15 baml_py-0.32.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-May-31 08:15 baml_py-0.32.0.dist-info/WHEEL
--rw-r--r--  4.6 unx       54 b- defN 24-May-31 08:15 baml_py-0.32.0.dist-info/entry_points.txt
--rw-r--r--  4.6 unx    11556 b- defN 24-May-31 08:15 baml_py-0.32.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx    11556 b- defN 24-May-31 08:15 baml_py-0.32.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx     3406 b- defN 24-May-31 08:15 baml_py/async_context_vars.py
--rw-r--r--  4.6 unx     4297 b- defN 24-May-31 08:15 baml_py/baml_py.pyi
--rw-r--r--  4.6 unx        0 b- defN 24-May-31 08:15 baml_py/py.typed
--rw-r--r--  4.6 unx     2474 b- defN 24-May-31 08:15 baml_py/stream.py
--rw-r--r--  4.6 unx     4330 b- defN 24-May-31 08:15 baml_py/type_builder.py
--rw-r--r--  4.6 unx      506 b- defN 24-May-31 08:15 baml_py/__init__.py
--rwxr-xr-x  4.6 unx 11766272 b- defN 24-May-31 08:15 baml_py/baml_py.pyd
--rw-r--r--  4.6 unx     1053 b- defN 24-May-31 08:15 baml_py-0.32.0.dist-info/RECORD
-13 files, 11805952 bytes uncompressed, 4452396 bytes compressed:  62.3%
+Zip file size: 4454154 bytes, number of entries: 13
+-rw-r--r--  4.6 unx      354 b- defN 24-May-31 09:54 baml_py-0.32.1.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-May-31 09:54 baml_py-0.32.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx       54 b- defN 24-May-31 09:54 baml_py-0.32.1.dist-info/entry_points.txt
+-rw-r--r--  4.6 unx    11556 b- defN 24-May-31 09:54 baml_py-0.32.1.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx    11556 b- defN 24-May-31 09:54 baml_py-0.32.1.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx     3406 b- defN 24-May-31 09:54 baml_py/async_context_vars.py
+-rw-r--r--  4.6 unx     4306 b- defN 24-May-31 09:54 baml_py/baml_py.pyi
+-rw-r--r--  4.6 unx        0 b- defN 24-May-31 09:54 baml_py/py.typed
+-rw-r--r--  4.6 unx     2474 b- defN 24-May-31 09:54 baml_py/stream.py
+-rw-r--r--  4.6 unx     4330 b- defN 24-May-31 09:54 baml_py/type_builder.py
+-rw-r--r--  4.6 unx      506 b- defN 24-May-31 09:54 baml_py/__init__.py
+-rwxr-xr-x  4.6 unx 11766272 b- defN 24-May-31 09:54 baml_py/baml_py.pyd
+-rw-r--r--  4.6 unx     1053 b- defN 24-May-31 09:54 baml_py-0.32.1.dist-info/RECORD
+13 files, 11805961 bytes uncompressed, 4452406 bytes compressed:  62.3%
```

## zipnote {}

```diff
@@ -1,20 +1,20 @@
-Filename: baml_py-0.32.0.dist-info/METADATA
+Filename: baml_py-0.32.1.dist-info/METADATA
 Comment: 
 
-Filename: baml_py-0.32.0.dist-info/WHEEL
+Filename: baml_py-0.32.1.dist-info/WHEEL
 Comment: 
 
-Filename: baml_py-0.32.0.dist-info/entry_points.txt
+Filename: baml_py-0.32.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: baml_py-0.32.0.dist-info/license_files/LICENSE
+Filename: baml_py-0.32.1.dist-info/license_files/LICENSE
 Comment: 
 
-Filename: baml_py-0.32.0.dist-info/license_files/LICENSE
+Filename: baml_py-0.32.1.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: baml_py/async_context_vars.py
 Comment: 
 
 Filename: baml_py/baml_py.pyi
 Comment: 
@@ -30,11 +30,11 @@
 
 Filename: baml_py/__init__.py
 Comment: 
 
 Filename: baml_py/baml_py.pyd
 Comment: 
 
-Filename: baml_py-0.32.0.dist-info/RECORD
+Filename: baml_py-0.32.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## baml_py/baml_py.pyi

```diff
@@ -28,17 +28,16 @@
     def __str__(self) -> str: ...
     def on_event(
         self, on_event: Callable[[FunctionResult], None]
     ) -> FunctionResultStream: ...
     async def done(self, ctx: RuntimeContextManager) -> FunctionResult: ...
 
 class BamlImagePy:
-    def __init__(
-        self, url: Optional[str] = None, base64: Optional[str] = None
-    ) -> None: ...
+    def from_url(url: str) -> BamlImagePy: ...
+    def from_base64(base64: str, media_type: str) -> BamlImagePy: ...
     @property
     def url(self) -> Optional[str]: ...
     @url.setter
     def url(self, value: Optional[str]) -> None: ...
     @property
     def base64(self) -> Optional[str]: ...
     @base64.setter
```

## Comparing `baml_py-0.32.0.dist-info/license_files/LICENSE` & `baml_py-0.32.1.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `baml_py-0.32.0.dist-info/RECORD` & `baml_py-0.32.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-baml_py-0.32.0.dist-info/METADATA,sha256=QKkCcQqx_wYDtvoVM7hJnmoA8A9tB50DfxpwalUCLOs,354
-baml_py-0.32.0.dist-info/WHEEL,sha256=_-pO1V0R3bpcg5FhWC82Cl79freIhF1O9I5uv0may5k,94
-baml_py-0.32.0.dist-info/entry_points.txt,sha256=9Uu_VcUjoI2qQMjVb0PRjEgI6pQ55WqBbzNparAPJyA,54
-baml_py-0.32.0.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
-baml_py-0.32.0.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
+baml_py-0.32.1.dist-info/METADATA,sha256=_a1mYpwUxJARHfPPxpSGY1nk6JPVxBMsYRtX2J6GVs4,354
+baml_py-0.32.1.dist-info/WHEEL,sha256=_-pO1V0R3bpcg5FhWC82Cl79freIhF1O9I5uv0may5k,94
+baml_py-0.32.1.dist-info/entry_points.txt,sha256=9Uu_VcUjoI2qQMjVb0PRjEgI6pQ55WqBbzNparAPJyA,54
+baml_py-0.32.1.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
+baml_py-0.32.1.dist-info/license_files/LICENSE,sha256=WtjCEwlcVzkh1ziO35P2qfVEkLjr87Flro7xlHz3CEY,11556
 baml_py/async_context_vars.py,sha256=QfnNjQIT9MtpqbfuD4v0hWlZIdn2JmNu8U-iKpHjTrc,3406
-baml_py/baml_py.pyi,sha256=-0B710418ZSIi6QndyNnpdaQFsBs77KQgXBSK3lJols,4297
+baml_py/baml_py.pyi,sha256=mDSpyFs8B8DeGJFucD5mjgDFmptTo5LAHTXBWAM5epU,4306
 baml_py/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 baml_py/stream.py,sha256=B4mpGnqAmU7DFHJPiAAAiNIeX5wgLJhXLZp9Pqb9-AY,2474
 baml_py/type_builder.py,sha256=v3yiY2VtGuCEECr0jh7OB3ueWSiSwj-8IETXQuSIYl0,4330
 baml_py/__init__.py,sha256=-y49naDuvHdmpkmUEqZBESlBNx6W4qsPOPu9KlrMT10,506
-baml_py/baml_py.pyd,sha256=8H9yOCsnSArMWVqlypr30A5kzyeu1Yt_fJIJ6N5yOHU,11766272
-baml_py-0.32.0.dist-info/RECORD,,
+baml_py/baml_py.pyd,sha256=VA59JVBmRUa8WvisjG8goUNZsj85Vc-LHme3B4XOya4,11766272
+baml_py-0.32.1.dist-info/RECORD,,
```
