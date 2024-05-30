# Comparing `tmp/elasticstore-2.1.1-py3-none-any.whl.zip` & `tmp/elasticstore-2.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 12311 bytes, number of entries: 12
+Zip file size: 12338 bytes, number of entries: 12
 -rw-r--r--  2.0 unx      158 b- defN 22-Oct-28 13:29 elasticstore/__init__.py
 -rw-r--r--  2.0 unx     3964 b- defN 23-Sep-01 11:12 elasticstore/lock.py
--rw-r--r--  2.0 unx    18121 b- defN 23-Nov-28 12:41 elasticstore/store.py
+-rw-r--r--  2.0 unx    18549 b- defN 24-May-30 22:03 elasticstore/store.py
 -rw-r--r--  2.0 unx     1588 b- defN 23-Nov-27 11:32 elasticstore/utils.py
 -rw-r--r--  2.0 unx       72 b- defN 23-Nov-27 12:04 elasticstore/legacy/__init__.py
 -rw-r--r--  2.0 unx    17738 b- defN 23-Nov-28 12:41 elasticstore/legacy/store.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Nov-28 12:43 elasticstore-2.1.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1477 b- defN 23-Nov-28 12:43 elasticstore-2.1.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Nov-28 12:43 elasticstore-2.1.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Nov-28 12:43 elasticstore-2.1.1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 22-Oct-27 19:55 elasticstore-2.1.1.dist-info/zip-safe
--rw-rw-r--  2.0 unx      988 b- defN 23-Nov-28 12:43 elasticstore-2.1.1.dist-info/RECORD
-12 files, 45284 bytes uncompressed, 10645 bytes compressed:  76.5%
+-rw-r--r--  2.0 unx     1072 b- defN 24-May-30 22:07 elasticstore-2.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1476 b- defN 24-May-30 22:07 elasticstore-2.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 22:07 elasticstore-2.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 24-May-30 22:07 elasticstore-2.2.0.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 22-Oct-27 19:55 elasticstore-2.2.0.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      988 b- defN 24-May-30 22:07 elasticstore-2.2.0.dist-info/RECORD
+12 files, 45711 bytes uncompressed, 10672 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -12,26 +12,26 @@
 
 Filename: elasticstore/legacy/__init__.py
 Comment: 
 
 Filename: elasticstore/legacy/store.py
 Comment: 
 
-Filename: elasticstore-2.1.1.dist-info/LICENSE
+Filename: elasticstore-2.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: elasticstore-2.1.1.dist-info/METADATA
+Filename: elasticstore-2.2.0.dist-info/METADATA
 Comment: 
 
-Filename: elasticstore-2.1.1.dist-info/WHEEL
+Filename: elasticstore-2.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: elasticstore-2.1.1.dist-info/top_level.txt
+Filename: elasticstore-2.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: elasticstore-2.1.1.dist-info/zip-safe
+Filename: elasticstore-2.2.0.dist-info/zip-safe
 Comment: 
 
-Filename: elasticstore-2.1.1.dist-info/RECORD
+Filename: elasticstore-2.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## elasticstore/store.py

```diff
@@ -335,51 +335,54 @@
         except NotFoundError:
             raise KeyError(id) from None
 
     @ensure_index_exists()
     async def bulk_delete(
         self,
         ids: Union[Iterable[str], AsyncIterable[str]],
-        stats_only: bool = False
+        stats_only: bool = False,
+        refresh: Union[bool, Literal['wait_for']] = False
     ):
         """
         Remove documents from the index.
         """
         async def iter_actions():
             async for id in aiter(ids):
                 yield dict(_index=self._index, _id=id, _op_type='delete')
 
-        return await async_bulk(self._es, iter_actions(), raise_on_error=False, stats_only=stats_only)
+        return await async_bulk(self._es, iter_actions(), raise_on_error=False, stats_only=stats_only, refresh=refresh)
 
     @ensure_index_exists()
     async def bulk_update(
         self,
         items: AsyncIterable[Tuple[str, T]],
         retry: int = DEFAULT_RETRY,
-        stats_only: bool = False
+        stats_only: bool = False,
+        refresh: Union[bool, Literal['wait_for']] = False
     ):
         """
         Updates documents in the index.
         """
         async def iter_actions():
             async for key, item in items:
                 doc = self._to_dict(item)
                 # use _source=doc and not **doc as it allows fields with reserved names like "version"
                 yield dict(_index=self._index, _id=key, _op_type='index', retry_on_conflict=retry, _source=doc)
 
-        return await async_bulk(self._es, iter_actions(), raise_on_error=False, stats_only=stats_only)
+        return await async_bulk(self._es, iter_actions(), raise_on_error=False, stats_only=stats_only, refresh=refresh)
 
     @ensure_index_exists()
     async def bulk_upsert(
         self,
         items: AsyncIterable[Tuple[str, Union[Dict[str, Any], Any]]],
         source: Optional[str] = None,
         create: bool = False,
         retry: int = DEFAULT_RETRY,
-        stats_only: bool = False
+        stats_only: bool = False,
+        refresh: Union[bool, Literal['wait_for']] = False
     ):
         """
         Updates documents in the index with partial content.
         Interprets items as script params if a script source is given.
         """
         async def iter_actions():
             async for key, item in items:
@@ -405,42 +408,45 @@
                             _index=self._index, _id=key, _op_type='update', retry_on_conflict=retry,
                             doc=doc, doc_as_upsert=True)
                     else:
                         yield dict(
                             _index=self._index, _id=key, _op_type='update', retry_on_conflict=retry,
                             doc=doc)
 
-        return await async_bulk(self._es, iter_actions(), raise_on_error=False, stats_only=stats_only)
+        return await async_bulk(self._es, iter_actions(), raise_on_error=False, stats_only=stats_only, refresh=refresh)
 
     @ensure_index_exists()
-    async def delete_by_query(self, query: Dict):
+    async def delete_by_query(self, query: Dict, refresh: Optional[bool] = False):
         """
         Deletes documents matching the provided query.
         """
         resp = await self._es.delete_by_query(index=self._index,
                                               query=query,
-                                              conflicts='proceed')
+                                              conflicts='proceed',
+                                              refresh=refresh)
         return resp.body
 
     @ensure_index_exists()
     async def update_by_query(
         self,
         query: Dict,
         item: Union[Dict[str, Any], Any],
-        source: str = UPDATE_SCRIPT
+        source: str = UPDATE_SCRIPT,
+        refresh: Optional[bool] = False
     ):
         """
         Update documents matching the provided query.
         Interprets items as script params.
         """
         doc = self._to_dict(item)
         resp = await self._es.update_by_query(index=self._index,
                                               script=dict(source=source, params=doc),
                                               query=query,
-                                              conflicts='proceed')
+                                              conflicts='proceed',
+                                              refresh=refresh)
         return resp.body
 
     async def mget(
         self, ids: Union[Iterable[str], AsyncIterable[str]], chunk_size: int = 500, **kwargs
     ) -> AsyncGenerator[Tuple[str, Optional[T]], None]:
         async for chunk in achunked(ids, chunk_size):
             resp = await self._es.mget(index=self._index, ids=chunk, **kwargs)
```

## Comparing `elasticstore-2.1.1.dist-info/LICENSE` & `elasticstore-2.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `elasticstore-2.1.1.dist-info/METADATA` & `elasticstore-2.2.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticstore
-Version: 2.1.1
+Version: 2.2.0
 Summary: Boring storing things in Elasticsearch 🐌
 Home-page: https://github.com/exdatic/elasticstore
 Author: André Kischkel
 Author-email: andre@exdatis.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: elasticsearch[async] (>=8)
-Requires-Dist: elasticsearch-dsl (==8.9.0a1)
+Requires-Dist: elasticsearch-dsl (>=8.13.0)
 Requires-Dist: orjson
 Provides-Extra: test
 Requires-Dist: flake8 ; extra == 'test'
 Requires-Dist: pytest ; extra == 'test'
 
 # elasticstore
```

## Comparing `elasticstore-2.1.1.dist-info/RECORD` & `elasticstore-2.2.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 elasticstore/__init__.py,sha256=f88KxQ2osnik1zCwTmqmQzCZAD7eNMfrPIqKldG6VSw,158
 elasticstore/lock.py,sha256=KZFFSal6gm1YfnqTNVref391gWEpmEQ2wYo5d7kQbUQ,3964
-elasticstore/store.py,sha256=xYskSuGkZkB4VtD8lH40GfjdB8KSTvZDEVsHUdW3rPk,18121
+elasticstore/store.py,sha256=AMs9lEgZz5z3bhB51ZnugH0fQidopcXhfYr_Yqw9zHE,18549
 elasticstore/utils.py,sha256=LpNrQX2B7AFdYnD6EHDPnsphhZgSXnYOPRMhwYS7e0s,1588
 elasticstore/legacy/__init__.py,sha256=Hx35qOnv9vHe-2SyVqTG_t2lSZfx3jVGoTqAZCYn84Q,72
 elasticstore/legacy/store.py,sha256=r2k71l9Q_7eaMPASHFneoxuxCyuRrf2i3A24YSDtNMk,17738
-elasticstore-2.1.1.dist-info/LICENSE,sha256=EOgY7-EubVydG-zw1cQDYKEV9KvJw80dK-gzbfSwbzM,1072
-elasticstore-2.1.1.dist-info/METADATA,sha256=9iXOrNLX_vwWZaJml-fpoqZ7t-JWuvrfOhYDm-mX9Ko,1477
-elasticstore-2.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-elasticstore-2.1.1.dist-info/top_level.txt,sha256=sBraV7Ff-bmc9ie1j2Js7RwNTLsqWrXA6rknpZtTXYo,13
-elasticstore-2.1.1.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-elasticstore-2.1.1.dist-info/RECORD,,
+elasticstore-2.2.0.dist-info/LICENSE,sha256=EOgY7-EubVydG-zw1cQDYKEV9KvJw80dK-gzbfSwbzM,1072
+elasticstore-2.2.0.dist-info/METADATA,sha256=D7tDvb-O_Ih9YMvRsTVqV9GEw0zQASDB_i_YQrTbmj0,1476
+elasticstore-2.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+elasticstore-2.2.0.dist-info/top_level.txt,sha256=sBraV7Ff-bmc9ie1j2Js7RwNTLsqWrXA6rknpZtTXYo,13
+elasticstore-2.2.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+elasticstore-2.2.0.dist-info/RECORD,,
```

