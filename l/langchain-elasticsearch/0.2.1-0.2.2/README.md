# Comparing `tmp/langchain_elasticsearch-0.2.1.tar.gz` & `tmp/langchain_elasticsearch-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_elasticsearch-0.2.1.tar", max compression
+gzip compressed data, was "langchain_elasticsearch-0.2.2.tar", max compression
```

## Comparing `langchain_elasticsearch-0.2.1.tar` & `langchain_elasticsearch-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/LICENSE
--rw-r--r--   0        0        0     5805 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/README.md
--rw-r--r--   0        0        0     1185 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/__init__.py
--rw-r--r--   0        0        0     1393 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/_utilities.py
--rw-r--r--   0        0        0     7748 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/cache.py
--rw-r--r--   0        0        0     5417 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/chat_history.py
--rw-r--r--   0        0        0     1094 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/client.py
--rw-r--r--   0        0        0     9253 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/embeddings.py
--rw-r--r--   0        0        0        0 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/py.typed
--rw-r--r--   0        0        0     4764 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/retrievers.py
--rw-r--r--   0        0        0    44274 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/langchain_elasticsearch/vectorstores.py
--rw-r--r--   0        0        0     2925 2024-05-16 15:09:45.361086 langchain_elasticsearch-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     6681 1970-01-01 00:00:00.000000 langchain_elasticsearch-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-31 08:32:27.869054 langchain_elasticsearch-0.2.2/LICENSE
+-rw-r--r--   0        0        0     7386 2024-05-31 08:32:27.869054 langchain_elasticsearch-0.2.2/README.md
+-rw-r--r--   0        0        0     1264 2024-05-31 08:32:27.869054 langchain_elasticsearch-0.2.2/langchain_elasticsearch/__init__.py
+-rw-r--r--   0        0        0     1455 2024-05-31 08:32:27.869054 langchain_elasticsearch-0.2.2/langchain_elasticsearch/_utilities.py
+-rw-r--r--   0        0        0    15822 2024-05-31 08:32:27.869054 langchain_elasticsearch-0.2.2/langchain_elasticsearch/cache.py
+-rw-r--r--   0        0        0     5400 2024-05-31 08:32:27.869054 langchain_elasticsearch-0.2.2/langchain_elasticsearch/chat_history.py
+-rw-r--r--   0        0        0     1094 2024-05-31 08:32:27.869054 langchain_elasticsearch-0.2.2/langchain_elasticsearch/client.py
+-rw-r--r--   0        0        0     9253 2024-05-31 08:32:27.869054 langchain_elasticsearch-0.2.2/langchain_elasticsearch/embeddings.py
+-rw-r--r--   0        0        0        0 2024-05-31 08:32:27.869054 langchain_elasticsearch-0.2.2/langchain_elasticsearch/py.typed
+-rw-r--r--   0        0        0     4764 2024-05-31 08:32:27.869054 langchain_elasticsearch-0.2.2/langchain_elasticsearch/retrievers.py
+-rw-r--r--   0        0        0    44224 2024-05-31 08:32:27.869054 langchain_elasticsearch-0.2.2/langchain_elasticsearch/vectorstores.py
+-rw-r--r--   0        0        0     2924 2024-05-31 08:32:27.869054 langchain_elasticsearch-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     8262 1970-01-01 00:00:00.000000 langchain_elasticsearch-0.2.2/PKG-INFO
```

### Comparing `langchain_elasticsearch-0.2.1/LICENSE` & `langchain_elasticsearch-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.2.1/README.md` & `langchain_elasticsearch-0.2.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -115,23 +115,21 @@
 ### ElasticsearchCache
 
 A caching layer for LLMs that uses Elasticsearch.
 
 Simple example:
 
 ```python
-from elasticsearch import Elasticsearch
 from langchain.globals import set_llm_cache
 
 from langchain_elasticsearch import ElasticsearchCache
 
-es_client = Elasticsearch(hosts="http://localhost:9200")
 set_llm_cache(
     ElasticsearchCache(
-        es_connection=es_client,
+        es_url="http://localhost:9200",
         index_name="llm-chat-cache",
         metadata={"project": "my_chatgpt_project"},
     )
 )
 ```
 
 The `index_name` parameter can also accept aliases. This allows to use the 
@@ -149,15 +147,14 @@
 This can be done by subclassing end overriding methods.
 The new cache class can be applied also to a pre-existing cache index:
 
 ```python
 import json
 from typing import Any, Dict, List
 
-from elasticsearch import Elasticsearch
 from langchain.globals import set_llm_cache
 from langchain_core.caches import RETURN_VAL_TYPE
 
 from langchain_elasticsearch import ElasticsearchCache
 
 
 class SearchableElasticsearchCache(ElasticsearchCache):
@@ -181,15 +178,69 @@
     def _parse_output(data: List[str]) -> List[str]:
         return [
             json.loads(output)["kwargs"]["message"]["kwargs"]["content"]
             for output in data
         ]
 
 
-es_client = Elasticsearch(hosts="http://localhost:9200")
 set_llm_cache(
-    SearchableElasticsearchCache(es_connection=es_client, index_name="llm-chat-cache")
+    SearchableElasticsearchCache(
+       es_url="http://localhost:9200", 
+       index_name="llm-chat-cache"
+    )
 )
 ```
 
 When overriding the mapping and the document building, 
-please only make additive modifications, keeping the base mapping intact.
+please only make additive modifications, keeping the base mapping intact.
+
+###  ElasticsearchEmbeddingsCache
+
+Store and temporarily cache embeddings.
+
+Caching embeddings is obtained by using the [CacheBackedEmbeddings](https://python.langchain.com/docs/modules/data_connection/text_embedding/caching_embeddings), it can be instantiated using `CacheBackedEmbeddings.from_bytes_store` method.
+
+```python
+from langchain.embeddings import CacheBackedEmbeddings
+from langchain_openai import OpenAIEmbeddings
+
+from langchain_elasticsearch import ElasticsearchEmbeddingsCache
+
+underlying_embeddings = OpenAIEmbeddings(model="text-embedding-3-small")
+
+store = ElasticsearchEmbeddingsCache(
+    es_url="http://localhost:9200",
+    index_name="llm-chat-cache",
+    metadata={"project": "my_chatgpt_project"},
+    namespace="my_chatgpt_project",
+)
+
+embeddings = CacheBackedEmbeddings.from_bytes_store(
+    underlying_embeddings=OpenAIEmbeddings(),
+    document_embedding_cache=store,
+    query_embedding_cache=store,
+)
+```
+
+Similarly to the chat cache, one can subclass `ElasticsearchEmbeddingsCache` in order to index vectors for search.
+
+```python
+from typing import Any, Dict, List
+from langchain_elasticsearch import ElasticsearchEmbeddingsCache
+
+class SearchableElasticsearchStore(ElasticsearchEmbeddingsCache):
+    @property
+    def mapping(self) -> Dict[str, Any]:
+        mapping = super().mapping
+        mapping["mappings"]["properties"]["vector"] = {
+            "type": "dense_vector",
+            "dims": 1536,
+            "index": True,
+            "similarity": "dot_product",
+        }
+        return mapping
+
+    def build_document(self, llm_input: str, vector: List[float]) -> Dict[str, Any]:
+        body = super().build_document(llm_input, vector)
+        body["vector"] = vector
+        return body
+```
```

### Comparing `langchain_elasticsearch-0.2.1/langchain_elasticsearch/__init__.py` & `langchain_elasticsearch-0.2.2/langchain_elasticsearch/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,18 @@
     DenseVectorScriptScoreStrategy,
     DenseVectorStrategy,
     DistanceMetric,
     RetrievalStrategy,
     SparseVectorStrategy,
 )
 
-from langchain_elasticsearch.cache import ElasticsearchCache
+from langchain_elasticsearch.cache import (
+    ElasticsearchCache,
+    ElasticsearchEmbeddingsCache,
+)
 from langchain_elasticsearch.chat_history import ElasticsearchChatMessageHistory
 from langchain_elasticsearch.embeddings import ElasticsearchEmbeddings
 from langchain_elasticsearch.retrievers import ElasticsearchRetriever
 from langchain_elasticsearch.vectorstores import (
     ApproxRetrievalStrategy,
     BM25RetrievalStrategy,
     ElasticsearchStore,
@@ -19,14 +22,15 @@
     SparseRetrievalStrategy,
 )
 
 __all__ = [
     "ElasticsearchCache",
     "ElasticsearchChatMessageHistory",
     "ElasticsearchEmbeddings",
+    "ElasticsearchEmbeddingsCache",
     "ElasticsearchRetriever",
     "ElasticsearchStore",
     # retrieval strategies
     "BM25Strategy",
     "DenseVectorScriptScoreStrategy",
     "DenseVectorStrategy",
     "DistanceMetric",
```

### Comparing `langchain_elasticsearch-0.2.1/langchain_elasticsearch/_utilities.py` & `langchain_elasticsearch-0.2.2/langchain_elasticsearch/_utilities.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+import logging
 from enum import Enum
 
-from elasticsearch import BadRequestError, ConflictError, Elasticsearch, NotFoundError
+from elasticsearch import Elasticsearch, exceptions
 from langchain_core import __version__ as langchain_version
 
+logger = logging.getLogger(__name__)
+
 
 class DistanceStrategy(str, Enum):
     """Enumerator of the Distance strategies for calculating distances
     between vectors."""
 
     EUCLIDEAN_DISTANCE = "EUCLIDEAN_DISTANCE"
     MAX_INNER_PRODUCT = "MAX_INNER_PRODUCT"
@@ -25,19 +28,19 @@
     return client.options(headers=headers)
 
 
 def model_must_be_deployed(client: Elasticsearch, model_id: str) -> None:
     try:
         dummy = {"x": "y"}
         client.ml.infer_trained_model(model_id=model_id, docs=[dummy])
-    except NotFoundError as err:
+    except exceptions.NotFoundError as err:
         raise err
-    except ConflictError as err:
-        raise NotFoundError(
+    except exceptions.ConflictError as err:
+        raise exceptions.NotFoundError(
             f"model '{model_id}' not found, please deploy it first",
             meta=err.meta,
             body=err.body,
         ) from err
-    except BadRequestError:
+    except exceptions.BadRequestError:
         # This error is expected because we do not know the expected document
         # shape and just use a dummy doc above.
         pass
```

### Comparing `langchain_elasticsearch-0.2.1/langchain_elasticsearch/chat_history.py` & `langchain_elasticsearch-0.2.2/langchain_elasticsearch/chat_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import json
 import logging
 from time import time
 from typing import TYPE_CHECKING, List, Optional
 
 from langchain_core.chat_history import BaseChatMessageHistory
-from langchain_core.messages import (
-    BaseMessage,
-    message_to_dict,
-    messages_from_dict,
-)
+from langchain_core.messages import BaseMessage, message_to_dict, messages_from_dict
 
 from langchain_elasticsearch._utilities import with_user_agent_header
 from langchain_elasticsearch.client import create_elasticsearch_client
 
 if TYPE_CHECKING:
     from elasticsearch import Elasticsearch
```

### Comparing `langchain_elasticsearch-0.2.1/langchain_elasticsearch/client.py` & `langchain_elasticsearch-0.2.2/langchain_elasticsearch/client.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.2.1/langchain_elasticsearch/embeddings.py` & `langchain_elasticsearch-0.2.2/langchain_elasticsearch/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.2.1/langchain_elasticsearch/retrievers.py` & `langchain_elasticsearch-0.2.2/langchain_elasticsearch/retrievers.py`

 * *Files identical despite different names*

### Comparing `langchain_elasticsearch-0.2.1/langchain_elasticsearch/vectorstores.py` & `langchain_elasticsearch-0.2.2/langchain_elasticsearch/vectorstores.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,21 @@
 import logging
 from abc import ABC, abstractmethod
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Iterable,
-    List,
-    Literal,
-    Optional,
-    Tuple,
-    Union,
-)
+from typing import Any, Callable, Dict, Iterable, List, Literal, Optional, Tuple, Union
 
 from elasticsearch import Elasticsearch
 from elasticsearch.helpers.vectorstore import (
     BM25Strategy,
     DenseVectorScriptScoreStrategy,
     DenseVectorStrategy,
     DistanceMetric,
     RetrievalStrategy,
     SparseVectorStrategy,
 )
-from elasticsearch.helpers.vectorstore import (
-    VectorStore as EVectorStore,
-)
+from elasticsearch.helpers.vectorstore import VectorStore as EVectorStore
 from langchain_core._api.deprecation import deprecated
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.vectorstores import VectorStore
 
 from langchain_elasticsearch._utilities import (
     DistanceStrategy,
```

### Comparing `langchain_elasticsearch-0.2.1/pyproject.toml` & `langchain_elasticsearch-0.2.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-elasticsearch"
-version = "0.2.1"
+version = "0.2.2"
 description = "An integration package connecting Elasticsearch and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-elastic"
 license = "MIT"
 
 [tool.poetry.urls]
@@ -88,8 +88,8 @@
 addopts = "--snapshot-warn-unused --strict-markers --strict-config --durations=5"
 # Registering custom markers.
 # https://docs.pytest.org/en/7.1.x/example/markers.html#registering-markers
 markers = [
   "requires: mark tests as requiring a specific library",
   "asyncio: mark tests as requiring asyncio",
 ]
-asyncio_mode = "auto"
+asyncio_mode = "auto"
```

### Comparing `langchain_elasticsearch-0.2.1/PKG-INFO` & `langchain_elasticsearch-0.2.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-elasticsearch
-Version: 0.2.1
+Version: 0.2.2
 Summary: An integration package connecting Elasticsearch and LangChain
 Home-page: https://github.com/langchain-ai/langchain-elastic
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -134,23 +134,21 @@
 ### ElasticsearchCache
 
 A caching layer for LLMs that uses Elasticsearch.
 
 Simple example:
 
 ```python
-from elasticsearch import Elasticsearch
 from langchain.globals import set_llm_cache
 
 from langchain_elasticsearch import ElasticsearchCache
 
-es_client = Elasticsearch(hosts="http://localhost:9200")
 set_llm_cache(
     ElasticsearchCache(
-        es_connection=es_client,
+        es_url="http://localhost:9200",
         index_name="llm-chat-cache",
         metadata={"project": "my_chatgpt_project"},
     )
 )
 ```
 
 The `index_name` parameter can also accept aliases. This allows to use the 
@@ -168,15 +166,14 @@
 This can be done by subclassing end overriding methods.
 The new cache class can be applied also to a pre-existing cache index:
 
 ```python
 import json
 from typing import Any, Dict, List
 
-from elasticsearch import Elasticsearch
 from langchain.globals import set_llm_cache
 from langchain_core.caches import RETURN_VAL_TYPE
 
 from langchain_elasticsearch import ElasticsearchCache
 
 
 class SearchableElasticsearchCache(ElasticsearchCache):
@@ -200,15 +197,70 @@
     def _parse_output(data: List[str]) -> List[str]:
         return [
             json.loads(output)["kwargs"]["message"]["kwargs"]["content"]
             for output in data
         ]
 
 
-es_client = Elasticsearch(hosts="http://localhost:9200")
 set_llm_cache(
-    SearchableElasticsearchCache(es_connection=es_client, index_name="llm-chat-cache")
+    SearchableElasticsearchCache(
+       es_url="http://localhost:9200", 
+       index_name="llm-chat-cache"
+    )
 )
 ```
 
 When overriding the mapping and the document building, 
 please only make additive modifications, keeping the base mapping intact.
+
+###  ElasticsearchEmbeddingsCache
+
+Store and temporarily cache embeddings.
+
+Caching embeddings is obtained by using the [CacheBackedEmbeddings](https://python.langchain.com/docs/modules/data_connection/text_embedding/caching_embeddings), it can be instantiated using `CacheBackedEmbeddings.from_bytes_store` method.
+
+```python
+from langchain.embeddings import CacheBackedEmbeddings
+from langchain_openai import OpenAIEmbeddings
+
+from langchain_elasticsearch import ElasticsearchEmbeddingsCache
+
+underlying_embeddings = OpenAIEmbeddings(model="text-embedding-3-small")
+
+store = ElasticsearchEmbeddingsCache(
+    es_url="http://localhost:9200",
+    index_name="llm-chat-cache",
+    metadata={"project": "my_chatgpt_project"},
+    namespace="my_chatgpt_project",
+)
+
+embeddings = CacheBackedEmbeddings.from_bytes_store(
+    underlying_embeddings=OpenAIEmbeddings(),
+    document_embedding_cache=store,
+    query_embedding_cache=store,
+)
+```
+
+Similarly to the chat cache, one can subclass `ElasticsearchEmbeddingsCache` in order to index vectors for search.
+
+```python
+from typing import Any, Dict, List
+from langchain_elasticsearch import ElasticsearchEmbeddingsCache
+
+class SearchableElasticsearchStore(ElasticsearchEmbeddingsCache):
+    @property
+    def mapping(self) -> Dict[str, Any]:
+        mapping = super().mapping
+        mapping["mappings"]["properties"]["vector"] = {
+            "type": "dense_vector",
+            "dims": 1536,
+            "index": True,
+            "similarity": "dot_product",
+        }
+        return mapping
+
+    def build_document(self, llm_input: str, vector: List[float]) -> Dict[str, Any]:
+        body = super().build_document(llm_input, vector)
+        body["vector"] = vector
+        return body
+```
+
```

