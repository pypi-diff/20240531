# Comparing `tmp/llama_index_embeddings_cohere-0.1.8.tar.gz` & `tmp/llama_index_embeddings_cohere-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_cohere-0.1.8.tar", max compression
+gzip compressed data, was "llama_index_embeddings_cohere-0.1.9.tar", max compression
```

## Comparing `llama_index_embeddings_cohere-0.1.8.tar` & `llama_index_embeddings_cohere-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       44 2024-04-17 19:23:24.482014 llama_index_embeddings_cohere-0.1.8/README.md
--rw-r--r--   0        0        0       94 2024-04-17 19:23:24.482014 llama_index_embeddings_cohere-0.1.8/llama_index/embeddings/cohere/__init__.py
--rw-r--r--   0        0        0     9459 2024-04-17 19:23:24.482014 llama_index_embeddings_cohere-0.1.8/llama_index/embeddings/cohere/base.py
--rw-r--r--   0        0        0     1493 2024-04-17 19:23:24.482014 llama_index_embeddings_cohere-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 llama_index_embeddings_cohere-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-05-31 18:59:53.837239 llama_index_embeddings_cohere-0.1.9/README.md
+-rw-r--r--   0        0        0       94 2024-05-31 18:59:53.837239 llama_index_embeddings_cohere-0.1.9/llama_index/embeddings/cohere/__init__.py
+-rw-r--r--   0        0        0    10312 2024-05-31 18:59:53.837239 llama_index_embeddings_cohere-0.1.9/llama_index/embeddings/cohere/base.py
+-rw-r--r--   0        0        0     1493 2024-05-31 18:59:53.837239 llama_index_embeddings_cohere-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 llama_index_embeddings_cohere-0.1.9/PKG-INFO
```

### Comparing `llama_index_embeddings_cohere-0.1.8/llama_index/embeddings/cohere/base.py` & `llama_index_embeddings_cohere-0.1.9/llama_index/embeddings/cohere/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
-from typing import List, Optional
+from typing import Any, List, Optional
 
 from llama_index.core.base.embeddings.base import (
     DEFAULT_EMBED_BATCH_SIZE,
     BaseEmbedding,
 )
-from llama_index.core.bridge.pydantic import Field
+from llama_index.core.bridge.pydantic import Field, PrivateAttr
 from llama_index.core.callbacks import CallbackManager
 import cohere
 import httpx
 
 
 # Enums for validation and type safety
 class CohereAIModelName(str, Enum):
@@ -101,43 +101,52 @@
 
 
 # Assuming BaseEmbedding is a Pydantic model and handles its own initializations
 class CohereEmbedding(BaseEmbedding):
     """CohereEmbedding uses the Cohere API to generate embeddings for text."""
 
     # Instance variables initialized via Pydantic's mechanism
-    cohere_client: cohere.Client = Field(description="CohereAI client")
-    cohere_async_client: cohere.AsyncClient = Field(description="CohereAI Async client")
+    api_key: str = Field(description="The Cohere API key.")
     truncate: str = Field(description="Truncation type - START/ END/ NONE")
     input_type: Optional[str] = Field(
         description="Model Input type. If not provided, search_document and search_query are used when needed."
     )
     embedding_type: str = Field(
         description="Embedding type. If not provided float embedding_type is used when needed."
     )
 
+    _client: cohere.Client = PrivateAttr()
+    _async_client: cohere.AsyncClient = PrivateAttr()
+    _base_url: Optional[str] = PrivateAttr()
+    _timeout: Optional[float] = PrivateAttr()
+    _httpx_client: Optional[httpx.Client] = PrivateAttr()
+    _httpx_async_client: Optional[httpx.AsyncClient] = PrivateAttr()
+
     def __init__(
         self,
+        # deprecated
         cohere_api_key: Optional[str] = None,
+        api_key: Optional[str] = None,
         model_name: str = "embed-english-v3.0",
         truncate: str = "END",
         input_type: Optional[str] = None,
         embedding_type: str = "float",
         embed_batch_size: int = DEFAULT_EMBED_BATCH_SIZE,
         callback_manager: Optional[CallbackManager] = None,
         base_url: Optional[str] = None,
         timeout: Optional[float] = None,
         httpx_client: Optional[httpx.Client] = None,
         httpx_async_client: Optional[httpx.AsyncClient] = None,
+        num_workers: Optional[int] = None,
+        **kwargs: Any,
     ):
         """
         A class representation for generating embeddings using the Cohere API.
 
         Args:
-            cohere_client (Any): An instance of the Cohere client, which is used to communicate with the Cohere API.
             truncate (str): A string indicating the truncation strategy to be applied to input text. Possible values
                         are 'START', 'END', or 'NONE'.
             input_type (Optional[str]): An optional string that specifies the type of input provided to the model.
                                     This is model-dependent and could be one of the following: 'search_query',
                                     'search_document', 'classification', or 'clustering'.
             model_name (str): The name of the model to be used for generating embeddings. The class ensures that
                           this model is supported and that the input type provided is compatible with the model.
@@ -155,75 +164,98 @@
                 f"{embedding_type} is not a embedding type for the provided model."
             )
 
         if truncate not in VALID_TRUNCATE_OPTIONS:
             raise ValueError(f"truncate must be one of {VALID_TRUNCATE_OPTIONS}")
 
         super().__init__(
-            cohere_client=cohere.Client(
-                cohere_api_key,
-                client_name="llama_index",
-                base_url=base_url,
-                timeout=timeout,
-                httpx_client=httpx_client,
-            ),
-            cohere_async_client=cohere.AsyncClient(
-                cohere_api_key,
-                client_name="llama_index",
-                base_url=base_url,
-                timeout=timeout,
-                httpx_client=httpx_async_client,
-            ),
-            cohere_api_key=cohere_api_key,
+            api_key=api_key or cohere_api_key,
             model_name=model_name,
             input_type=input_type,
             embedding_type=embedding_type,
             truncate=truncate,
             embed_batch_size=embed_batch_size,
             callback_manager=callback_manager,
+            num_workers=num_workers,
+            **kwargs,
         )
 
+        self._client = None
+        self._async_client = None
+        self._base_url = base_url
+        self._timeout = timeout
+        self._httpx_client = httpx_client
+        self._httpx_async_client = httpx_async_client
+
+    def _get_client(self) -> cohere.Client:
+        if self._client is None:
+            self._client = cohere.Client(
+                api_key=self.api_key,
+                client_name="llama_index",
+                base_url=self._base_url,
+                timeout=self._timeout,
+                httpx_client=self._httpx_client,
+            )
+
+        return self._client
+
+    def _get_async_client(self) -> cohere.AsyncClient:
+        if self._async_client is None:
+            self._async_client = cohere.AsyncClient(
+                api_key=self.api_key,
+                client_name="llama_index",
+                base_url=self._base_url,
+                timeout=self._timeout,
+                httpx_client=self._httpx_async_client,
+            )
+
+        return self._async_client
+
     @classmethod
     def class_name(cls) -> str:
         return "CohereEmbedding"
 
     def _embed(self, texts: List[str], input_type: str) -> List[List[float]]:
         """Embed sentences using Cohere."""
+        client = self._get_client()
+
         if self.model_name in V3_MODELS:
-            result = self.cohere_client.embed(
+            result = client.embed(
                 texts=texts,
                 input_type=self.input_type or input_type,
                 embedding_types=[self.embedding_type],
                 model=self.model_name,
                 truncate=self.truncate,
             ).embeddings
         else:
-            result = self.cohere_client.embed(
+            result = client.embed(
                 texts=texts,
                 model=self.model_name,
                 embedding_types=[self.embedding_type],
                 truncate=self.truncate,
             ).embeddings
         return getattr(result, self.embedding_type, None)
 
     async def _aembed(self, texts: List[str], input_type: str) -> List[List[float]]:
         """Embed sentences using Cohere."""
+        async_client = self._get_async_client()
+
         if self.model_name in V3_MODELS:
             result = (
-                await self.cohere_async_client.embed(
+                await async_client.embed(
                     texts=texts,
                     input_type=self.input_type or input_type,
                     embedding_types=[self.embedding_type],
                     model=self.model_name,
                     truncate=self.truncate,
                 )
             ).embeddings
         else:
             result = (
-                await self.cohere_async_client.embed(
+                await async_client.embed(
                     texts=texts,
                     model=self.model_name,
                     embedding_types=[self.embedding_type],
                     truncate=self.truncate,
                 )
             ).embeddings
         return getattr(result, self.embedding_type, None)
```

### Comparing `llama_index_embeddings_cohere-0.1.8/pyproject.toml` & `llama_index_embeddings_cohere-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings cohere integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-cohere"
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 cohere = "^5.2.5"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_embeddings_cohere-0.1.8/PKG-INFO` & `llama_index_embeddings_cohere-0.1.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-cohere
-Version: 0.1.8
+Version: 0.1.9
 Summary: llama-index embeddings cohere integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

