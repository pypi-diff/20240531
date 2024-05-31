# Comparing `tmp/llama_index_llms_huggingface-0.2.0.tar.gz` & `tmp/llama_index_llms_huggingface-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_huggingface-0.2.0.tar", max compression
+gzip compressed data, was "llama_index_llms_huggingface-0.2.2.tar", max compression
```

## Comparing `llama_index_llms_huggingface-0.2.0.tar` & `llama_index_llms_huggingface-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       43 2024-05-10 17:44:12.198538 llama_index_llms_huggingface-0.2.0/README.md
--rw-r--r--   0        0        0      212 2024-05-10 17:44:12.198538 llama_index_llms_huggingface-0.2.0/llama_index/llms/huggingface/__init__.py
--rw-r--r--   0        0        0    39711 2024-05-10 17:44:12.198538 llama_index_llms_huggingface-0.2.0/llama_index/llms/huggingface/base.py
--rw-r--r--   0        0        0     2082 2024-05-10 17:44:12.198538 llama_index_llms_huggingface-0.2.0/llama_index/llms/huggingface/utils.py
--rw-r--r--   0        0        0     1636 2024-05-10 17:44:12.198538 llama_index_llms_huggingface-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 llama_index_llms_huggingface-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2024-05-31 04:53:38.095158 llama_index_llms_huggingface-0.2.2/README.md
+-rw-r--r--   0        0        0      212 2024-05-31 04:53:38.095158 llama_index_llms_huggingface-0.2.2/llama_index/llms/huggingface/__init__.py
+-rw-r--r--   0        0        0    39794 2024-05-31 04:53:38.099158 llama_index_llms_huggingface-0.2.2/llama_index/llms/huggingface/base.py
+-rw-r--r--   0        0        0     2082 2024-05-31 04:53:38.099158 llama_index_llms_huggingface-0.2.2/llama_index/llms/huggingface/utils.py
+-rw-r--r--   0        0        0     1637 2024-05-31 04:53:38.099158 llama_index_llms_huggingface-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      790 1970-01-01 00:00:00.000000 llama_index_llms_huggingface-0.2.2/PKG-INFO
```

### Comparing `llama_index_llms_huggingface-0.2.0/llama_index/llms/huggingface/base.py` & `llama_index_llms_huggingface-0.2.2/llama_index/llms/huggingface/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import logging
-from threading import Thread
 from typing import Any, Callable, Dict, List, Optional, Sequence, Union
 
 import torch
 from huggingface_hub import AsyncInferenceClient, InferenceClient, model_info
 from huggingface_hub.hf_api import ModelInfo
 from huggingface_hub.inference._types import ConversationalOutput
 from llama_index.core.base.llms.types import (
@@ -38,15 +37,15 @@
     chat_to_completion_decorator,
     achat_to_completion_decorator,
     stream_chat_to_completion_decorator,
     astream_chat_to_completion_decorator,
     get_from_param_or_env,
 )
 from llama_index.core.prompts.base import PromptTemplate
-from llama_index.core.types import BaseOutputParser, PydanticProgramMode
+from llama_index.core.types import BaseOutputParser, PydanticProgramMode, Thread
 from llama_index.core.chat_engine.types import AgentChatResponse
 from llama_index.core.tools.types import BaseTool
 from llama_index.llms.huggingface.utils import (
     to_tgi_messages,
     force_single_tool_call,
     resolve_tgi_function_call,
     get_max_input_length,
@@ -866,17 +865,17 @@
         response = self._sync_client.chat(messages=messages, **all_kwargs)
         tool_calls = response.choices[0].message.tool_calls
 
         return ChatResponse(
             message=ChatMessage(
                 role=MessageRole.ASSISTANT,
                 content=response.choices[0].message.content,
-                additional_kwargs={"tool_calls": tool_calls}
-                if tool_calls is not None
-                else {},
+                additional_kwargs=(
+                    {"tool_calls": tool_calls} if tool_calls is not None else {}
+                ),
             ),
             raw=dict(response),
         )
 
     @llm_completion_callback()
     def complete(
         self, prompt: str, formatted: bool = False, **kwargs: Any
@@ -926,17 +925,17 @@
         response = await self._async_client.chat(messages=messages, **all_kwargs)
         tool_calls = response.choices[0].message.tool_calls
 
         return ChatResponse(
             message=ChatMessage(
                 role=MessageRole.ASSISTANT,
                 content=response.choices[0].message.content,
-                additional_kwargs={"tool_calls": tool_calls}
-                if tool_calls is not None
-                else {},
+                additional_kwargs=(
+                    {"tool_calls": tool_calls} if tool_calls is not None else {}
+                ),
             ),
             raw=dict(response),
         )
 
     @llm_completion_callback()
     async def acomplete(
         self, prompt: str, formatted: bool = False, **kwargs: Any
@@ -986,15 +985,17 @@
         verbose: bool = False,
         allow_parallel_tool_calls: bool = False,
         tool_choice: str = "auto",
         **kwargs: Any,
     ) -> ChatResponse:
         """Predict and call the tool."""
         # use openai tool format
-        tool_specs = [tool.metadata.to_openai_tool() for tool in tools]
+        tool_specs = [
+            tool.metadata.to_openai_tool(skip_length_check=True) for tool in tools
+        ]
 
         if isinstance(user_msg, str):
             user_msg = ChatMessage(role=MessageRole.USER, content=user_msg)
 
         messages = chat_history or []
         if user_msg:
             messages.append(user_msg)
@@ -1016,15 +1017,17 @@
         chat_history: Optional[List[ChatMessage]] = None,
         verbose: bool = False,
         allow_parallel_tool_calls: bool = False,
         tool_choice: str = "auto",
         **kwargs: Any,
     ) -> ChatResponse:
         # use openai tool format
-        tool_specs = [tool.metadata.to_openai_tool() for tool in tools]
+        tool_specs = [
+            tool.metadata.to_openai_tool(skip_length_check=True) for tool in tools
+        ]
 
         if isinstance(user_msg, str):
             user_msg = ChatMessage(role=MessageRole.USER, content=user_msg)
 
         messages = chat_history or []
         if user_msg:
             messages.append(user_msg)
```

### Comparing `llama_index_llms_huggingface-0.2.0/llama_index/llms/huggingface/utils.py` & `llama_index_llms_huggingface-0.2.2/llama_index/llms/huggingface/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_huggingface-0.2.0/pyproject.toml` & `llama_index_llms_huggingface-0.2.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms huggingface integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-huggingface"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.2"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.1"
+llama-index-core = "^0.10.41"
 huggingface-hub = "^0.23.0"
 torch = "^2.1.2"
 text-generation = "^0.7.0"
 
 [tool.poetry.dependencies.transformers]
 extras = ["torch"]
 version = "^4.37.0"
```

### Comparing `llama_index_llms_huggingface-0.2.0/PKG-INFO` & `llama_index_llms_huggingface-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-huggingface
-Version: 0.2.0
+Version: 0.2.2
 Summary: llama-index llms huggingface integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: huggingface-hub (>=0.23.0,<0.24.0)
-Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.41,<0.11.0)
 Requires-Dist: text-generation (>=0.7.0,<0.8.0)
 Requires-Dist: torch (>=2.1.2,<3.0.0)
 Requires-Dist: transformers[torch] (>=4.37.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Huggingface
```

