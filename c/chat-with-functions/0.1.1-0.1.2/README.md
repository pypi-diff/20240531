# Comparing `tmp/chat_with_functions-0.1.1.tar.gz` & `tmp/chat_with_functions-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_with_functions-0.1.1.tar", max compression
+gzip compressed data, was "chat_with_functions-0.1.2.tar", max compression
```

## Comparing `chat_with_functions-0.1.1.tar` & `chat_with_functions-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0        0 2023-11-27 05:47:16.988781 chat_with_functions-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-10-24 08:32:07.988369 chat_with_functions-0.1.1/chat_with_functions/__init__.py
--rw-r--r--   0        0        0     8850 2023-11-29 15:32:08.391354 chat_with_functions-0.1.1/chat_with_functions/cached_streaming.py
--rw-r--r--   0        0        0     1900 2023-10-24 08:42:53.293305 chat_with_functions-0.1.1/chat_with_functions/caches.py
--rw-r--r--   0        0        0     8936 2023-11-29 16:13:37.892804 chat_with_functions-0.1.1/chat_with_functions/chat.py
--rw-r--r--   0        0        0      257 2023-12-09 08:24:38.903841 chat_with_functions-0.1.1/chat_with_functions/data_structures.py
--rw-r--r--   0        0        0    11167 2023-11-29 16:06:14.374644 chat_with_functions-0.1.1/chat_with_functions/function_calling_structure.py
--rw-r--r--   0        0        0     6718 2023-11-29 16:32:37.913716 chat_with_functions-0.1.1/chat_with_functions/openai_api.py
--rw-r--r--   0        0        0    13604 2023-11-29 16:16:30.654166 chat_with_functions-0.1.1/chat_with_functions/openai_util.py
--rw-r--r--   0        0        0     4936 2023-11-29 15:54:04.409521 chat_with_functions-0.1.1/chat_with_functions/streaming.py
--rw-r--r--   0        0        0      366 2023-10-24 08:39:44.876681 chat_with_functions-0.1.1/chat_with_functions/util.py
--rw-r--r--   0        0        0      438 2024-01-22 13:32:05.857242 chat_with_functions-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 chat_with_functions-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-11-27 05:47:16.988781 chat_with_functions-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-10-24 08:32:07.988369 chat_with_functions-0.1.2/chat_with_functions/__init__.py
+-rw-r--r--   0        0        0     8874 2024-02-15 10:57:09.327202 chat_with_functions-0.1.2/chat_with_functions/cached_streaming.py
+-rw-r--r--   0        0        0     1900 2023-10-24 08:42:53.293305 chat_with_functions-0.1.2/chat_with_functions/caches.py
+-rw-r--r--   0        0        0     8936 2023-11-29 16:13:37.892804 chat_with_functions-0.1.2/chat_with_functions/chat.py
+-rw-r--r--   0        0        0      257 2023-12-09 08:24:38.903841 chat_with_functions-0.1.2/chat_with_functions/data_structures.py
+-rw-r--r--   0        0        0    11167 2023-11-29 16:06:14.374644 chat_with_functions-0.1.2/chat_with_functions/function_calling_structure.py
+-rw-r--r--   0        0        0     6718 2023-11-29 16:32:37.913716 chat_with_functions-0.1.2/chat_with_functions/openai_api.py
+-rw-r--r--   0        0        0    13604 2023-11-29 16:16:30.654166 chat_with_functions-0.1.2/chat_with_functions/openai_util.py
+-rw-r--r--   0        0        0     4952 2024-03-12 09:11:53.486811 chat_with_functions-0.1.2/chat_with_functions/streaming.py
+-rw-r--r--   0        0        0      366 2023-10-24 08:39:44.876681 chat_with_functions-0.1.2/chat_with_functions/util.py
+-rw-r--r--   0        0        0      421 2024-05-31 03:31:01.831764 chat_with_functions-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 chat_with_functions-0.1.2/PKG-INFO
```

### Comparing `chat_with_functions-0.1.1/chat_with_functions/cached_streaming.py` & `chat_with_functions-0.1.2/chat_with_functions/cached_streaming.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import asyncio
 import traceback
 from abc import ABC
 from asyncio import Future, Queue, Task, Lock
 from dataclasses import dataclass, field
 from typing import TypeVar, Generic, AsyncIterable, Callable, Awaitable, Tuple, AsyncGenerator
 
-from loguru import logger
 from returns.interfaces.unwrappable import Unwrappable
 from returns.pipeline import is_successful
 from returns.result import safe
 
 from chat_with_functions.caches import AsyncCache
 
 T = TypeVar('T')
@@ -197,14 +196,15 @@
         if self.backend is None:
             if await self.cache.exists():
                 self.backend: AsyncStream = AsyncStream.create()
 
                 async def cache_load_task():
                     try:
                         data = await self.cache.get()
+                        from loguru import logger
                         logger.debug(f"loaded {len(data)} items")
                         for item in data:
                             await self.backend.put(item)
                         await self.backend.finish()
                     except Exception as e:
                         await self.backend.raise_exception(e)
```

### Comparing `chat_with_functions-0.1.1/chat_with_functions/caches.py` & `chat_with_functions-0.1.2/chat_with_functions/caches.py`

 * *Files identical despite different names*

### Comparing `chat_with_functions-0.1.1/chat_with_functions/chat.py` & `chat_with_functions-0.1.2/chat_with_functions/chat.py`

 * *Files identical despite different names*

### Comparing `chat_with_functions-0.1.1/chat_with_functions/function_calling_structure.py` & `chat_with_functions-0.1.2/chat_with_functions/function_calling_structure.py`

 * *Files identical despite different names*

### Comparing `chat_with_functions-0.1.1/chat_with_functions/openai_api.py` & `chat_with_functions-0.1.2/chat_with_functions/openai_api.py`

 * *Files identical despite different names*

### Comparing `chat_with_functions-0.1.1/chat_with_functions/openai_util.py` & `chat_with_functions-0.1.2/chat_with_functions/openai_util.py`

 * *Files identical despite different names*

### Comparing `chat_with_functions-0.1.1/chat_with_functions/streaming.py` & `chat_with_functions-0.1.2/chat_with_functions/streaming.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,19 @@
 from chat_with_functions.cached_streaming import CachedStream, IStream
 from chat_with_functions.caches import AsyncCache, DictAsyncCacheHandle
 from chat_with_functions.data_structures import OpenAICallArgs
 from chat_with_functions.openai_api import Message, ChatCompletion
 from chat_with_functions.openai_util import OpenAIChatUtil
 from pinjected import Injected, injected, instance
 from pinjected.decoration import update_if_registered
-from pinjected.di.bindings import BindMetadata
 from pinjected.di.util import get_code_location, instances
 
+from pinjected.di.metadata.bind_metadata import BindMetadata
+
+
 @dataclass
 class StreamResponse:
     src: IStream[ChatCompletionChunk]
     msgs: IStream[str]  # stream of tokens
     fcs: IStream[ChoiceDeltaFunctionCall]
     parsed: Future[ChatCompletion]
```

