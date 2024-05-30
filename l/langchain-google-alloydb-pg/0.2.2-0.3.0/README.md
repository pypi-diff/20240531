# Comparing `tmp/langchain_google_alloydb_pg-0.2.2-py3-none-any.whl.zip` & `tmp/langchain_google_alloydb_pg-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 29373 bytes, number of entries: 13
--rw-r--r--  2.0 unx     1019 b- defN 24-Apr-30 23:26 langchain_google_alloydb_pg/__init__.py
--rw-r--r--  2.0 unx     4945 b- defN 24-Apr-30 23:26 langchain_google_alloydb_pg/alloydb_chat_message_history.py
--rw-r--r--  2.0 unx    13800 b- defN 24-Apr-30 23:26 langchain_google_alloydb_pg/alloydb_engine.py
--rw-r--r--  2.0 unx    16820 b- defN 24-Apr-30 23:26 langchain_google_alloydb_pg/alloydb_loader.py
--rw-r--r--  2.0 unx    29540 b- defN 24-Apr-30 23:26 langchain_google_alloydb_pg/alloydb_vectorstore.py
--rw-r--r--  2.0 unx     2580 b- defN 24-Apr-30 23:26 langchain_google_alloydb_pg/indexes.py
--rw-rw-r--  2.0 unx        0 b- defN 24-Apr-30 23:26 langchain_google_alloydb_pg/py.typed
--rw-r--r--  2.0 unx      597 b- defN 24-Apr-30 23:26 langchain_google_alloydb_pg/version.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-Apr-30 23:28 langchain_google_alloydb_pg-0.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx    20244 b- defN 24-Apr-30 23:28 langchain_google_alloydb_pg-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-30 23:28 langchain_google_alloydb_pg-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       28 b- defN 24-Apr-30 23:28 langchain_google_alloydb_pg-0.2.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1293 b- defN 24-Apr-30 23:28 langchain_google_alloydb_pg-0.2.2.dist-info/RECORD
-13 files, 102316 bytes uncompressed, 27145 bytes compressed:  73.5%
+Zip file size: 29526 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     1019 b- defN 24-May-30 22:27 langchain_google_alloydb_pg/__init__.py
+-rw-r--r--  2.0 unx     5011 b- defN 24-May-30 22:27 langchain_google_alloydb_pg/alloydb_chat_message_history.py
+-rw-r--r--  2.0 unx    14072 b- defN 24-May-30 22:27 langchain_google_alloydb_pg/alloydb_engine.py
+-rw-r--r--  2.0 unx    17328 b- defN 24-May-30 22:27 langchain_google_alloydb_pg/alloydb_loader.py
+-rw-r--r--  2.0 unx    29695 b- defN 24-May-30 22:27 langchain_google_alloydb_pg/alloydb_vectorstore.py
+-rw-r--r--  2.0 unx     2652 b- defN 24-May-30 22:27 langchain_google_alloydb_pg/indexes.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-30 22:27 langchain_google_alloydb_pg/py.typed
+-rw-r--r--  2.0 unx      597 b- defN 24-May-30 22:27 langchain_google_alloydb_pg/version.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-May-30 22:29 langchain_google_alloydb_pg-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    20295 b- defN 24-May-30 22:29 langchain_google_alloydb_pg-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 22:29 langchain_google_alloydb_pg-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 24-May-30 22:29 langchain_google_alloydb_pg-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1293 b- defN 24-May-30 22:29 langchain_google_alloydb_pg-0.3.0.dist-info/RECORD
+13 files, 103440 bytes uncompressed, 27298 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: langchain_google_alloydb_pg/py.typed
 Comment: 
 
 Filename: langchain_google_alloydb_pg/version.py
 Comment: 
 
-Filename: langchain_google_alloydb_pg-0.2.2.dist-info/LICENSE
+Filename: langchain_google_alloydb_pg-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: langchain_google_alloydb_pg-0.2.2.dist-info/METADATA
+Filename: langchain_google_alloydb_pg-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: langchain_google_alloydb_pg-0.2.2.dist-info/WHEEL
+Filename: langchain_google_alloydb_pg-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: langchain_google_alloydb_pg-0.2.2.dist-info/top_level.txt
+Filename: langchain_google_alloydb_pg-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: langchain_google_alloydb_pg-0.2.2.dist-info/RECORD
+Filename: langchain_google_alloydb_pg-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langchain_google_alloydb_pg/alloydb_chat_message_history.py

```diff
@@ -41,15 +41,15 @@
 class AlloyDBChatMessageHistory(BaseChatMessageHistory):
     """Chat message history stored in an AlloyDB."""
 
     __create_key = object()
 
     def __init__(
         self,
-        key,
+        key: object,
         engine: AlloyDBEngine,
         session_id: str,
         table_name: str,
         messages: List[BaseMessage],
     ):
         if key != AlloyDBChatMessageHistory.__create_key:
             raise Exception(
@@ -62,15 +62,15 @@
 
     @classmethod
     async def create(
         cls,
         engine: AlloyDBEngine,
         session_id: str,
         table_name: str,
-    ):
+    ) -> AlloyDBChatMessageHistory:
         table_schema = await engine._aload_table_schema(table_name)
         column_names = table_schema.columns.keys()
 
         required_columns = ["id", "session_id", "data", "type"]
 
         if not (all(x in column_names for x in required_columns)):
             raise IndexError(
@@ -89,15 +89,15 @@
 
     @classmethod
     def create_sync(
         cls,
         engine: AlloyDBEngine,
         session_id: str,
         table_name: str,
-    ):
+    ) -> AlloyDBChatMessageHistory:
         coro = cls.create(engine, session_id, table_name)
         return engine._run_as_sync(coro)
 
     async def aadd_message(self, message: BaseMessage) -> None:
         """Append the message to the record in AlloyDB"""
         query = f"""INSERT INTO "{self.table_name}"(session_id, data, type)
                     VALUES (:session_id, :data, :type);
```

## langchain_google_alloydb_pg/alloydb_engine.py

```diff
@@ -7,27 +7,37 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
 from __future__ import annotations
 
 import asyncio
 from dataclasses import dataclass
 from threading import Thread
-from typing import TYPE_CHECKING, Awaitable, Dict, List, Optional, TypeVar, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Awaitable,
+    Dict,
+    List,
+    Optional,
+    Sequence,
+    Type,
+    TypeVar,
+    Union,
+)
 
 import aiohttp
 import google.auth  # type: ignore
 import google.auth.transport.requests  # type: ignore
 from google.cloud.alloydb.connector import AsyncConnector, IPTypes
-from sqlalchemy import MetaData, Table, text
+from sqlalchemy import MetaData, RowMapping, Table, text
 from sqlalchemy.exc import InvalidRequestError
 from sqlalchemy.ext.asyncio import AsyncEngine, create_async_engine
 
 from .version import __version__
 
 if TYPE_CHECKING:
     import asyncpg  # type: ignore
@@ -77,15 +87,15 @@
 
 @dataclass
 class Column:
     name: str
     data_type: str
     nullable: bool = True
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if not isinstance(self.name, str):
             raise ValueError("Column name must be type string")
         if not isinstance(self.data_type, str):
             raise ValueError("Column data_type must be type string")
 
 
 class AlloyDBEngine:
@@ -94,22 +104,22 @@
     _connector: Optional[AsyncConnector] = None
 
     def __init__(
         self,
         engine: AsyncEngine,
         loop: Optional[asyncio.AbstractEventLoop],
         thread: Optional[Thread],
-    ):
+    ) -> None:
         self._engine = engine
         self._loop = loop
         self._thread = thread
 
     @classmethod
     def from_instance(
-        cls,
+        cls: Type[AlloyDBEngine],
         project_id: str,
         region: str,
         cluster: str,
         instance: str,
         database: str,
         user: Optional[str] = None,
         password: Optional[str] = None,
@@ -132,15 +142,15 @@
             loop=loop,
             thread=thread,
         )
         return asyncio.run_coroutine_threadsafe(coro, loop).result()
 
     @classmethod
     async def _create(
-        cls,
+        cls: Type[AlloyDBEngine],
         project_id: str,
         region: str,
         cluster: str,
         instance: str,
         database: str,
         ip_type: Union[str, IPTypes],
         user: Optional[str] = None,
@@ -189,15 +199,15 @@
             "postgresql+asyncpg://",
             async_creator=getconn,
         )
         return cls(engine, loop, thread)
 
     @classmethod
     async def afrom_instance(
-        cls,
+        cls: Type[AlloyDBEngine],
         project_id: str,
         region: str,
         cluster: str,
         instance: str,
         database: str,
         user: Optional[str] = None,
         password: Optional[str] = None,
@@ -211,42 +221,44 @@
             database,
             ip_type,
             user,
             password,
         )
 
     @classmethod
-    def from_engine(cls, engine: AsyncEngine) -> AlloyDBEngine:
+    def from_engine(cls: Type[AlloyDBEngine], engine: AsyncEngine) -> AlloyDBEngine:
         return cls(engine, None, None)
 
-    async def _aexecute(self, query: str, params: Optional[dict] = None):
+    async def _aexecute(self, query: str, params: Optional[dict] = None) -> None:
         """Execute a SQL query."""
         async with self._engine.connect() as conn:
             await conn.execute(text(query), params)
             await conn.commit()
 
-    async def _aexecute_outside_tx(self, query: str):
+    async def _aexecute_outside_tx(self, query: str) -> None:
         """Execute a SQL query."""
         async with self._engine.connect() as conn:
             await conn.execute(text("COMMIT"))
             await conn.execute(text(query))
 
-    async def _afetch(self, query: str, params: Optional[dict] = None):
+    async def _afetch(
+        self, query: str, params: Optional[dict] = None
+    ) -> Sequence[RowMapping]:
         async with self._engine.connect() as conn:
             """Fetch results from a SQL query."""
             result = await conn.execute(text(query), params)
             result_map = result.mappings()
             result_fetch = result_map.fetchall()
 
         return result_fetch
 
-    def _execute(self, query: str, params: Optional[dict] = None):
+    def _execute(self, query: str, params: Optional[dict] = None) -> None:
         return self._run_as_sync(self._aexecute(query, params))
 
-    def _fetch(self, query: str, params: Optional[dict] = None):
+    def _fetch(self, query: str, params: Optional[dict] = None) -> Sequence[RowMapping]:
         return self._run_as_sync(self._afetch(query, params))
 
     def _run_as_sync(self, coro: Awaitable[T]) -> T:
         if not self._loop:
             raise Exception("Engine was initialized async.")
         return asyncio.run_coroutine_threadsafe(coro, self._loop).result()
 
@@ -302,24 +314,24 @@
                 metadata_json_column,
                 id_column,
                 overwrite_existing,
                 store_metadata,
             )
         )
 
-    async def ainit_chat_history_table(self, table_name) -> None:
+    async def ainit_chat_history_table(self, table_name: str) -> None:
         create_table_query = f"""CREATE TABLE IF NOT EXISTS "{table_name}"(
             id SERIAL PRIMARY KEY,
             session_id TEXT NOT NULL,
             data JSONB NOT NULL,
             type TEXT NOT NULL
         );"""
         await self._aexecute(create_table_query)
 
-    def init_chat_history_table(self, table_name) -> None:
+    def init_chat_history_table(self, table_name: str) -> None:
         return self._run_as_sync(
             self.ainit_chat_history_table(
                 table_name,
             )
         )
 
     async def ainit_document_table(
@@ -336,15 +348,14 @@
         Args:
             table_name (str): The PgSQL database table name.
             metadata_columns (List[Column]): A list of Columns
                 to create for custom metadata. Optional.
             store_metadata (bool): Whether to store extra metadata in a metadata column
                 if not described in 'metadata' field list (Default: True).
         """
-
         query = f"""CREATE TABLE "{table_name}"(
             {content_column} TEXT NOT NULL
             """
         for column in metadata_columns:
             nullable = "NOT NULL" if not column.nullable else ""
             query += f',\n"{column.name}" {column.data_type} {nullable}'
         metadata_json_column = metadata_json_column or "langchain_metadata"
```

## langchain_google_alloydb_pg/alloydb_loader.py

```diff
@@ -20,54 +20,55 @@
     AsyncIterator,
     Callable,
     Dict,
     Iterable,
     Iterator,
     List,
     Optional,
+    Type,
 )
 
 import sqlalchemy
 from langchain_community.document_loaders.base import BaseLoader
 from langchain_core.documents import Document
 
 from .alloydb_engine import AlloyDBEngine
 
 DEFAULT_CONTENT_COL = "page_content"
 DEFAULT_METADATA_COL = "langchain_metadata"
 
 
-def text_formatter(row, content_columns) -> str:
+def text_formatter(row: Dict[str, Any], content_columns: Iterable[str]) -> str:
     return " ".join(str(row[column]) for column in content_columns if column in row)
 
 
-def csv_formatter(row, content_columns) -> str:
+def csv_formatter(row: Dict[str, Any], content_columns: Iterable[str]) -> str:
     return ", ".join(str(row[column]) for column in content_columns if column in row)
 
 
-def yaml_formatter(row, content_columns) -> str:
+def yaml_formatter(row: Dict[str, Any], content_columns: Iterable[str]) -> str:
     return "\n".join(
         f"{column}: {str(row[column])}" for column in content_columns if column in row
     )
 
 
-def json_formatter(row, content_columns) -> str:
-    dictionary = {}
+def json_formatter(row: Dict[str, Any], content_columns: Iterable[str]) -> str:
+    dictionary: Dict[str, Any] = {}
     for column in content_columns:
         if column in row:
             dictionary[column] = row[column]
     return json.dumps(dictionary)
 
 
 def _parse_doc_from_row(
     content_columns: Iterable[str],
     metadata_columns: Iterable[str],
-    row: dict,
+    row: Dict[str, Any],
     metadata_json_column: Optional[str] = DEFAULT_METADATA_COL,
-    formatter: Callable = text_formatter,
+    formatter: Callable[[Dict[str, Any], Iterable[str]], str] = text_formatter,
 ) -> Document:
     page_content = formatter(row, content_columns)
     metadata: Dict[str, Any] = {}
     # unnest metadata from langchain_metadata column
     if metadata_json_column and row.get(metadata_json_column):
         for k, v in row[metadata_json_column].items():
             metadata[k] = v
@@ -80,46 +81,46 @@
 
 
 def _parse_row_from_doc(
     doc: Document,
     column_names: Iterable[str],
     content_column: str = DEFAULT_CONTENT_COL,
     metadata_json_column: Optional[str] = DEFAULT_METADATA_COL,
-) -> Dict:
+) -> Dict[str, Any]:
     doc_metadata = doc.metadata.copy()
     row: Dict[str, Any] = {content_column: doc.page_content}
     for entry in doc.metadata:
         if entry in column_names:
             row[entry] = doc_metadata[entry]
             del doc_metadata[entry]
     # store extra metadata in langchain_metadata column in json format
     if metadata_json_column:
         row[metadata_json_column] = doc_metadata
     return row
 
 
 class AlloyDBLoader(BaseLoader):
-    """Load documents from Alloydb`.
+    """Load documents from AlloyDB`.
 
     Each document represents one row of the result. The `content_columns` are
-    written into the `content_columns`of the document. The `metadata_columns` are written
+    written into the `content_columns` of the document. The `metadata_columns` are written
     into the `metadata_columns` of the document. By default, first columns is written into
     the `page_content` and everything else into the `metadata`.
     """
 
     __create_key = object()
 
     def __init__(
         self,
-        key,
+        key: object,
         engine: AlloyDBEngine,
         query: str,
         content_columns: List[str],
         metadata_columns: List[str],
-        formatter: Callable,
+        formatter: Callable[[Dict[str, Any], Iterable[str]], str],
         metadata_json_column: Optional[str] = None,
     ) -> None:
         if key != AlloyDBLoader.__create_key:
             raise Exception(
                 "Only create class through 'create' or 'create_sync' methods!"
             )
 
@@ -128,24 +129,24 @@
         self.content_columns = content_columns
         self.metadata_columns = metadata_columns
         self.formatter = formatter
         self.metadata_json_column = metadata_json_column
 
     @classmethod
     async def create(
-        cls,
+        cls: Type[AlloyDBLoader],
         engine: AlloyDBEngine,
         query: Optional[str] = None,
         table_name: Optional[str] = None,
         content_columns: Optional[List[str]] = None,
         metadata_columns: Optional[List[str]] = None,
         metadata_json_column: Optional[str] = None,
         format: Optional[str] = None,
         formatter: Optional[Callable] = None,
-    ):
+    ) -> AlloyDBLoader:
         """Constructor for AlloyDBLoader
 
         Args:
             engine (AlloyDBEngine):AsyncEngine with pool connection to the postgres database
             query (Optional[str], optional): SQL query. Defaults to None.
             table_name (Optional[str], optional): Name of table to query. Defaults to None.
             content_columns (Optional[List[str]], optional): Column that represent a Document's page_content. Defaults to the first column.
@@ -221,48 +222,50 @@
             metadata_columns,
             formatter,
             metadata_json_column,
         )
 
     @classmethod
     def create_sync(
-        cls,
+        cls: Type[AlloyDBLoader],
         engine: AlloyDBEngine,
         query: Optional[str] = None,
         table_name: Optional[str] = None,
         content_columns: Optional[List[str]] = None,
         metadata_columns: Optional[List[str]] = None,
         metadata_json_column: Optional[str] = None,
         format: Optional[str] = None,
         formatter: Optional[Callable] = None,
-    ):
+    ) -> AlloyDBLoader:
         coro = cls.create(
             engine,
             query,
             table_name,
             content_columns,
             metadata_columns,
             metadata_json_column,
             format,
             formatter,
         )
         return engine._run_as_sync(coro)
 
-    async def _collect_async_items(self, docs_generator):
+    async def _collect_async_items(
+        self, docs_generator: AsyncIterator[Document]
+    ) -> List[Document]:
         return [doc async for doc in docs_generator]
 
     def load(self) -> List[Document]:
-        """Load Alloydb data into Document objects."""
+        """Load AlloyDB data into Document objects."""
         documents = self.engine._run_as_sync(
             self._collect_async_items(self.alazy_load())
         )
         return documents
 
     async def aload(self) -> List[Document]:
-        """Load Alloydb data into Document objects."""
+        """Load AlloyDB data into Document objects."""
         return [doc async for doc in self.alazy_load()]
 
     def lazy_load(self) -> Iterator[Document]:
         """Load AlloyDB data into Document objects lazily."""
         yield from self.engine._run_as_sync(
             self._collect_async_items(self.alazy_load())
         )
@@ -299,40 +302,40 @@
 class AlloyDBDocumentSaver:
     """A class for saving langchain documents into a AlloyDB database table."""
 
     __create_key = object()
 
     def __init__(
         self,
-        key,
+        key: object,
         engine: AlloyDBEngine,
         table_name: str,
         content_column: str,
         metadata_columns: List[str] = [],
         metadata_json_column: Optional[str] = None,
-    ):
+    ) -> None:
         if key != AlloyDBDocumentSaver.__create_key:
             raise Exception(
                 "Only create class through 'create' or 'create_sync' methods!"
             )
         self.engine = engine
         self.table_name = table_name
         self.content_column = content_column
         self.metadata_columns = metadata_columns
         self.metadata_json_column = metadata_json_column
 
     @classmethod
     async def create(
-        cls,
+        cls: Type[AlloyDBDocumentSaver],
         engine: AlloyDBEngine,
         table_name: str,
         content_column: str = DEFAULT_CONTENT_COL,
         metadata_columns: List[str] = [],
         metadata_json_column: Optional[str] = DEFAULT_METADATA_COL,
-    ):
+    ) -> AlloyDBDocumentSaver:
         table_schema = await engine._aload_table_schema(table_name)
         column_names = table_schema.columns.keys()
         if content_column not in column_names:
             raise ValueError(f"Content column, {content_column}, does not exist.")
 
         # Set metadata columns to all columns if not set
         if len(metadata_columns) == 0:
@@ -363,21 +366,21 @@
             content_column,
             metadata_columns,
             metadata_json_column,
         )
 
     @classmethod
     def create_sync(
-        cls,
+        cls: Type[AlloyDBDocumentSaver],
         engine: AlloyDBEngine,
         table_name: str,
         content_column: str = DEFAULT_CONTENT_COL,
         metadata_columns: List[str] = [],
         metadata_json_column: str = DEFAULT_METADATA_COL,
-    ):
+    ) -> AlloyDBDocumentSaver:
         coro = cls.create(
             engine,
             table_name,
             content_column,
             metadata_columns,
             metadata_json_column,
         )
```

## langchain_google_alloydb_pg/alloydb_vectorstore.py

```diff
@@ -12,20 +12,21 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # TODO: Remove below import when minimum supported Python version is 3.10
 from __future__ import annotations
 
 import json
-from typing import Any, Iterable, List, Optional, Tuple, Type, Union
+from typing import Any, Iterable, List, Optional, Sequence, Tuple, Type, Union
 
 import numpy as np
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.vectorstores import VectorStore
+from sqlalchemy import RowMapping
 
 from .alloydb_engine import AlloyDBEngine
 from .indexes import (
     DEFAULT_DISTANCE_STRATEGY,
     DEFAULT_INDEX_NAME,
     BaseIndex,
     DistanceStrategy,
@@ -37,15 +38,15 @@
 class AlloyDBVectorStore(VectorStore):
     """Google AlloyDB Vector Store class"""
 
     __create_key = object()
 
     def __init__(
         self,
-        key,
+        key: object,
         engine: AlloyDBEngine,
         embedding_service: Embeddings,
         table_name: str,
         content_column: str = "content",
         embedding_column: str = "embedding",
         metadata_columns: List[str] = [],
         id_column: str = "langchain_id",
@@ -73,30 +74,30 @@
         self.k = k
         self.fetch_k = fetch_k
         self.lambda_mult = lambda_mult
         self.index_query_options = index_query_options
 
     @classmethod
     async def create(
-        cls,
+        cls: Type[AlloyDBVectorStore],
         engine: AlloyDBEngine,
         embedding_service: Embeddings,
         table_name: str,
         content_column: str = "content",
         embedding_column: str = "embedding",
         metadata_columns: List[str] = [],
         ignore_metadata_columns: Optional[List[str]] = None,
         id_column: str = "langchain_id",
         metadata_json_column: Optional[str] = "langchain_metadata",
         distance_strategy: DistanceStrategy = DEFAULT_DISTANCE_STRATEGY,
         k: int = 4,
         fetch_k: int = 20,
         lambda_mult: float = 0.5,
         index_query_options: Optional[QueryOptions] = None,
-    ):
+    ) -> AlloyDBVectorStore:
         """Constructor for AlloyDBVectorStore.
         Args:
             engine (AlloyDBEngine): Connection pool engine for managing connections to AlloyDB database.
             embedding_service (Embeddings): Text embedding model to use.
             table_name (str): Name of the existing table or the table to be created.
             content_column (str): Column that represent a Document’s page_content. Defaults to "content".
             embedding_column (str): Column for embedding vectors. The embedding is generated from the document value. Defaults to "embedding".
@@ -183,15 +184,15 @@
         id_column: str = "langchain_id",
         metadata_json_column: str = "langchain_metadata",
         distance_strategy: DistanceStrategy = DEFAULT_DISTANCE_STRATEGY,
         k: int = 4,
         fetch_k: int = 20,
         lambda_mult: float = 0.5,
         index_query_options: Optional[QueryOptions] = None,
-    ):
+    ) -> AlloyDBVectorStore:
         coro = cls.create(
             engine,
             embedding_service,
             table_name,
             content_column,
             embedding_column,
             metadata_columns,
@@ -396,15 +397,15 @@
         content_column: str = "content",
         embedding_column: str = "embedding",
         metadata_columns: List[str] = [],
         ignore_metadata_columns: Optional[List[str]] = None,
         id_column: str = "langchain_id",
         metadata_json_column: str = "langchain_metadata",
         **kwargs: Any,
-    ):
+    ) -> AlloyDBVectorStore:
         coro = cls.afrom_texts(
             texts,
             embedding,
             engine,
             table_name,
             metadatas=metadatas,
             content_column=content_column,
@@ -451,15 +452,15 @@
         return engine._run_as_sync(coro)
 
     async def __query_collection(
         self,
         embedding: List[float],
         k: Optional[int] = None,
         filter: Optional[str] = None,
-    ) -> List[Any]:
+    ) -> Sequence[RowMapping]:
         k = k if k else self.k
         operator = self.distance_strategy.operator
         search_function = self.distance_strategy.search_function
 
         filter = f"WHERE {filter}" if filter else ""
         stmt = f"SELECT *, {search_function}({self.embedding_column}, '{embedding}') as distance FROM \"{self.table_name}\" {filter} ORDER BY {self.embedding_column} {operator} '{embedding}' LIMIT {k};"
         if self.index_query_options:
```

## langchain_google_alloydb_pg/indexes.py

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import enum
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
-from typing import List, Optional
+from typing import List, Optional, Type, TypeVar
 
 
 @dataclass
 class StrategyMixin:
     operator: str
     search_function: str
     index_function: str
@@ -29,16 +29,16 @@
     """Enumerator of the Distance strategies."""
 
     EUCLIDEAN = "<->", "l2_distance", "vector_l2_ops"
     COSINE_DISTANCE = "<=>", "cosine_distance", "vector_cosine_ops"
     INNER_PRODUCT = "<#>", "ip_distance", "vector_ip_ops"
 
 
-DEFAULT_DISTANCE_STRATEGY = DistanceStrategy.COSINE_DISTANCE
-DEFAULT_INDEX_NAME = "langchainvectorindex"
+DEFAULT_DISTANCE_STRATEGY: DistanceStrategy = DistanceStrategy.COSINE_DISTANCE
+DEFAULT_INDEX_NAME: str = "langchainvectorindex"
 
 
 @dataclass
 class BaseIndex(ABC):
     name: str = DEFAULT_INDEX_NAME
     index_type: str = "base"
     distance_strategy: DistanceStrategy = field(
@@ -66,23 +66,24 @@
 
     def index_options(self) -> str:
         return f"(m = {self.m}, ef_construction = {self.ef_construction})"
 
 
 @dataclass
 class QueryOptions(ABC):
+    @abstractmethod
     def to_string(self) -> str:
         raise NotImplementedError("to_string method must be implemented by subclass")
 
 
 @dataclass
 class HNSWQueryOptions(QueryOptions):
     ef_search: int = 40
 
-    def to_string(self):
+    def to_string(self) -> str:
         return f"hnsw.ef_search = {self.ef_search}"
 
 
 @dataclass
 class IVFFlatIndex(BaseIndex):
     index_type: str = "ivfflat"
     lists: int = 1
@@ -91,9 +92,9 @@
         return f"(lists = {self.lists})"
 
 
 @dataclass
 class IVFFlatQueryOptions(QueryOptions):
     probes: int = 1
 
-    def to_string(self):
-        return f"ivflfat.probes = {self.probes}"
+    def to_string(self) -> str:
+        return f"ivfflat.probes = {self.probes}"
```

## langchain_google_alloydb_pg/version.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.2"
+__version__ = "0.3.0"
```

## Comparing `langchain_google_alloydb_pg-0.2.2.dist-info/LICENSE` & `langchain_google_alloydb_pg-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langchain_google_alloydb_pg-0.2.2.dist-info/METADATA` & `langchain_google_alloydb_pg-0.3.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-alloydb-pg
-Version: 0.2.2
+Version: 0.3.0
 Summary: LangChain integrations for Google Cloud AlloyDB for PostgreSQL
 Author-email: Google LLC <googleapis-packages@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -229,28 +229,29 @@
 Requires-Dist: SQLAlchemy[asyncio] <3.0.0,>=2.0.25
 Requires-Dist: numpy ==1.24.4 ; python_version <= "3.8"
 Requires-Dist: numpy <2.0.0,>=1.24.4 ; python_version > "3.8"
 Provides-Extra: test
 Requires-Dist: black[jupyter] ==24.4.2 ; extra == 'test'
 Requires-Dist: isort ==5.13.2 ; extra == 'test'
 Requires-Dist: mypy ==1.10.0 ; extra == 'test'
-Requires-Dist: pytest-asyncio ==0.23.6 ; extra == 'test'
-Requires-Dist: pytest ==8.2.0 ; extra == 'test'
+Requires-Dist: pytest-asyncio ==0.23.7 ; extra == 'test'
+Requires-Dist: pytest ==8.2.1 ; extra == 'test'
+Requires-Dist: pytest-cov ==5.0.0 ; extra == 'test'
 
 AlloyDB for PostgreSQL for LangChain
 ==================================================
 
 |preview| |pypi| |versions|
 
 - `Client Library Documentation`_
 - `Product Documentation`_
 
 .. |preview| image:: https://img.shields.io/badge/support-preview-orange.svg
    :target: https://github.com/googleapis/google-cloud-python/blob/main/README.rst#stability-levels
-.. |pypi| image:: https://img.shields.io/pypi/v/langchain-google-alloydb-pg.svg  
+.. |pypi| image:: https://img.shields.io/pypi/v/langchain-google-alloydb-pg.svg
    :target: https://pypi.org/project/langchain-google-alloydb-pg/
 .. |versions| image:: https://img.shields.io/pypi/pyversions/langchain-google-alloydb-pg.svg
    :target: https://pypi.org/project/langchain-google-alloydb-pg/
 .. _Client Library Documentation: https://cloud.google.com/python/docs/reference/langchain-google-alloydb-pg/latest
 .. _Product Documentation: https://cloud.google.com/alloydb
 
 
@@ -328,15 +329,15 @@
 
 
    engine = AlloyDBEngine.from_instance("project-id", "region", "my-cluster", "my-instance", "my-database")
    embeddings_service = VertexAIEmbeddings(model_name="textembedding-gecko@003")
    vectorstore = AlloyDBVectorStore.create_sync(
        engine,
        table_name="my-table",
-       embedding_service=embedding_service
+       embedding_service=embeddings_service
    )
 
 See the full `Vector Store`_ tutorial.
 
 .. _`Vector Store`: https://github.com/googleapis/langchain-google-alloydb-pg-python/tree/main/docs/vector_store.ipynb
 
 Document Loader Usage
```

## Comparing `langchain_google_alloydb_pg-0.2.2.dist-info/RECORD` & `langchain_google_alloydb_pg-0.3.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 langchain_google_alloydb_pg/__init__.py,sha256=o-3xTGhj34XtT1B4mNEVaXq5ANdeFLpMvcafTm8-B_c,1019
-langchain_google_alloydb_pg/alloydb_chat_message_history.py,sha256=Uxz6VuQPxqxQp200QEa2epXKVfWEaqhp2MBHxxx8Q6o,4945
-langchain_google_alloydb_pg/alloydb_engine.py,sha256=YEhS_X0EmKlozeCXEviPEaGYA4YuHOO04HsqVt7IkEM,13800
-langchain_google_alloydb_pg/alloydb_loader.py,sha256=WC3y-APUG1X2I6xxL7lg1d9ar6RJ7xyDl1ZSNIUVxOI,16820
-langchain_google_alloydb_pg/alloydb_vectorstore.py,sha256=9yIWlDvyHQxmSMZ5763GWP-71jU4m8AFMddUUYq6mrk,29540
-langchain_google_alloydb_pg/indexes.py,sha256=UYbXMcZXBvaU7FFa7IjhXvBvCuDdxr0Tq2pgyQrKVtU,2580
+langchain_google_alloydb_pg/alloydb_chat_message_history.py,sha256=vq5w1K3U0rER_Qui-JC_V5C3rY_MaeC0iU1-iane0h0,5011
+langchain_google_alloydb_pg/alloydb_engine.py,sha256=12W2Ow2j9mJy4MTJOod_DpXaFJS34YyAL50q1FSpnzg,14072
+langchain_google_alloydb_pg/alloydb_loader.py,sha256=_trxgQtS4cpD0phSwU9Q7IdIbf2VvqhHiDuig478N9s,17328
+langchain_google_alloydb_pg/alloydb_vectorstore.py,sha256=AjVUhjqqBBEaYy5YdS7Vje-exko7SofvhRl9TTC2Cyg,29695
+langchain_google_alloydb_pg/indexes.py,sha256=hhPMXfuz28_EDT_bJIAWo4Hc1hhv4iB6Gs5HSOGuyKw,2652
 langchain_google_alloydb_pg/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-langchain_google_alloydb_pg/version.py,sha256=r_E0O4zsO8RmFXO1jNldtopOU4jjOND4dKdlCCYS1rE,597
-langchain_google_alloydb_pg-0.2.2.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-langchain_google_alloydb_pg-0.2.2.dist-info/METADATA,sha256=1idPIogU4Bww8eu65Qy8B6DJ2ihGEMdUQ1zicb4xhfA,20244
-langchain_google_alloydb_pg-0.2.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-langchain_google_alloydb_pg-0.2.2.dist-info/top_level.txt,sha256=oHZAsNgaSCO84iduMcOJROVrOYrW7BeE-c8kvmydZyo,28
-langchain_google_alloydb_pg-0.2.2.dist-info/RECORD,,
+langchain_google_alloydb_pg/version.py,sha256=Bt9xmJb_aic5hHSb19XJI5LMnotdGjBnwcYbbCI4jfo,597
+langchain_google_alloydb_pg-0.3.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+langchain_google_alloydb_pg-0.3.0.dist-info/METADATA,sha256=3xcuL2INQlmLI-EkPucBaFM9ktrjGliWLu93K5Dp5Dc,20295
+langchain_google_alloydb_pg-0.3.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+langchain_google_alloydb_pg-0.3.0.dist-info/top_level.txt,sha256=oHZAsNgaSCO84iduMcOJROVrOYrW7BeE-c8kvmydZyo,28
+langchain_google_alloydb_pg-0.3.0.dist-info/RECORD,,
```

