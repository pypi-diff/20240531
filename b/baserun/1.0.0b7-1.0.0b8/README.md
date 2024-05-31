# Comparing `tmp/baserun-1.0.0b7.tar.gz` & `tmp/baserun-1.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baserun-1.0.0b7.tar", last modified: Wed May 29 23:36:04 2024, max compression
+gzip compressed data, was "baserun-1.0.0b8.tar", last modified: Fri May 31 18:12:57 2024, max compression
```

## Comparing `baserun-1.0.0b7.tar` & `baserun-1.0.0b8.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 23:36:04.454116 baserun-1.0.0b7/
--rw-r--r--   0 epeterson   (501) staff       (20)     1073 2023-08-04 18:23:26.000000 baserun-1.0.0b7/LICENSE
--rw-r--r--   0 epeterson   (501) staff       (20)     6568 2024-05-29 23:36:04.453928 baserun-1.0.0b7/PKG-INFO
--rw-r--r--   0 epeterson   (501) staff       (20)     4914 2024-05-29 22:46:16.000000 baserun-1.0.0b7/README.md
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 23:36:04.420094 baserun-1.0.0b7/baserun/
--rw-r--r--   0 epeterson   (501) staff       (20)     1381 2024-05-29 18:43:55.000000 baserun-1.0.0b7/baserun/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)     8879 2024-05-29 22:46:20.000000 baserun-1.0.0b7/baserun/api.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 23:36:04.449363 baserun-1.0.0b7/baserun/integrations/
--rw-r--r--   0 epeterson   (501) staff       (20)      305 2024-05-29 19:59:55.000000 baserun-1.0.0b7/baserun/integrations/integration.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2045 2024-05-29 19:59:55.000000 baserun-1.0.0b7/baserun/integrations/llamaindex.py
--rw-r--r--   0 epeterson   (501) staff       (20)     6943 2024-05-29 22:46:16.000000 baserun-1.0.0b7/baserun/mixins.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 23:36:04.450744 baserun-1.0.0b7/baserun/models/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-29 18:31:57.000000 baserun-1.0.0b7/baserun/models/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)     3292 2024-05-29 18:31:57.000000 baserun-1.0.0b7/baserun/models/evals.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2390 2024-05-29 18:31:57.000000 baserun-1.0.0b7/baserun/models/tags.py
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-29 19:59:55.000000 baserun-1.0.0b7/baserun/py.typed
--rw-r--r--   0 epeterson   (501) staff       (20)      533 2024-05-29 22:46:16.000000 baserun-1.0.0b7/baserun/pytest_plugin.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2594 2024-05-29 22:46:20.000000 baserun-1.0.0b7/baserun/utils.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 23:36:04.451647 baserun-1.0.0b7/baserun/wrappers/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-29 18:31:57.000000 baserun-1.0.0b7/baserun/wrappers/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)    17680 2024-05-29 23:14:38.000000 baserun-1.0.0b7/baserun/wrappers/openai.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 23:36:04.453206 baserun-1.0.0b7/baserun.egg-info/
--rw-r--r--   0 epeterson   (501) staff       (20)     6568 2024-05-29 23:36:04.000000 baserun-1.0.0b7/baserun.egg-info/PKG-INFO
--rw-r--r--   0 epeterson   (501) staff       (20)      570 2024-05-29 23:36:04.000000 baserun-1.0.0b7/baserun.egg-info/SOURCES.txt
--rw-r--r--   0 epeterson   (501) staff       (20)        1 2024-05-29 23:36:04.000000 baserun-1.0.0b7/baserun.egg-info/dependency_links.txt
--rw-r--r--   0 epeterson   (501) staff       (20)       44 2024-05-29 23:36:04.000000 baserun-1.0.0b7/baserun.egg-info/entry_points.txt
--rw-r--r--   0 epeterson   (501) staff       (20)       21 2024-05-29 23:36:04.000000 baserun-1.0.0b7/baserun.egg-info/requires.txt
--rw-r--r--   0 epeterson   (501) staff       (20)        8 2024-05-29 23:36:04.000000 baserun-1.0.0b7/baserun.egg-info/top_level.txt
--rw-r--r--   0 epeterson   (501) staff       (20)     1093 2024-05-29 23:35:54.000000 baserun-1.0.0b7/pyproject.toml
--rw-r--r--   0 epeterson   (501) staff       (20)       81 2024-05-29 23:36:04.454738 baserun-1.0.0b7/setup.cfg
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 23:36:04.452155 baserun-1.0.0b7/tests/
--rw-r--r--   0 epeterson   (501) staff       (20)    13673 2024-05-29 22:46:16.000000 baserun-1.0.0b7/tests/testing_functions.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-31 18:12:57.362825 baserun-1.0.0b8/
+-rw-r--r--   0 epeterson   (501) staff       (20)     1073 2023-08-04 18:23:26.000000 baserun-1.0.0b8/LICENSE
+-rw-r--r--   0 epeterson   (501) staff       (20)     6563 2024-05-31 18:12:57.362555 baserun-1.0.0b8/PKG-INFO
+-rw-r--r--   0 epeterson   (501) staff       (20)     4909 2024-05-31 18:12:40.000000 baserun-1.0.0b8/README.md
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-31 18:12:57.330805 baserun-1.0.0b8/baserun/
+-rw-r--r--   0 epeterson   (501) staff       (20)     2773 2024-05-31 18:06:41.000000 baserun-1.0.0b8/baserun/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    11020 2024-05-31 18:06:41.000000 baserun-1.0.0b8/baserun/api.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-31 18:12:57.352982 baserun-1.0.0b8/baserun/integrations/
+-rw-r--r--   0 epeterson   (501) staff       (20)      305 2024-05-29 19:59:55.000000 baserun-1.0.0b8/baserun/integrations/integration.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2045 2024-05-29 19:59:55.000000 baserun-1.0.0b8/baserun/integrations/llamaindex.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     7635 2024-05-31 18:06:41.000000 baserun-1.0.0b8/baserun/mixins.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-31 18:12:57.355139 baserun-1.0.0b8/baserun/models/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-29 18:31:57.000000 baserun-1.0.0b8/baserun/models/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     3292 2024-05-31 18:06:41.000000 baserun-1.0.0b8/baserun/models/evals.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2390 2024-05-29 18:31:57.000000 baserun-1.0.0b8/baserun/models/tags.py
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-29 19:59:55.000000 baserun-1.0.0b8/baserun/py.typed
+-rw-r--r--   0 epeterson   (501) staff       (20)      613 2024-05-31 18:06:41.000000 baserun-1.0.0b8/baserun/pytest_plugin.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2594 2024-05-29 23:36:22.000000 baserun-1.0.0b8/baserun/utils.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-31 18:12:57.358722 baserun-1.0.0b8/baserun/wrappers/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-29 18:31:57.000000 baserun-1.0.0b8/baserun/wrappers/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    19563 2024-05-31 18:06:41.000000 baserun-1.0.0b8/baserun/wrappers/anthropic.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    17699 2024-05-31 18:06:41.000000 baserun-1.0.0b8/baserun/wrappers/openai.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-31 18:12:57.361534 baserun-1.0.0b8/baserun.egg-info/
+-rw-r--r--   0 epeterson   (501) staff       (20)     6563 2024-05-31 18:12:57.000000 baserun-1.0.0b8/baserun.egg-info/PKG-INFO
+-rw-r--r--   0 epeterson   (501) staff       (20)      600 2024-05-31 18:12:57.000000 baserun-1.0.0b8/baserun.egg-info/SOURCES.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)        1 2024-05-31 18:12:57.000000 baserun-1.0.0b8/baserun.egg-info/dependency_links.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)       44 2024-05-31 18:12:57.000000 baserun-1.0.0b8/baserun.egg-info/entry_points.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)       21 2024-05-31 18:12:57.000000 baserun-1.0.0b8/baserun.egg-info/requires.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)        8 2024-05-31 18:12:57.000000 baserun-1.0.0b8/baserun.egg-info/top_level.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)     1093 2024-05-31 18:12:21.000000 baserun-1.0.0b8/pyproject.toml
+-rw-r--r--   0 epeterson   (501) staff       (20)       81 2024-05-31 18:12:57.363755 baserun-1.0.0b8/setup.cfg
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-31 18:12:57.360147 baserun-1.0.0b8/tests/
+-rw-r--r--   0 epeterson   (501) staff       (20)    13638 2024-05-31 18:06:41.000000 baserun-1.0.0b8/tests/testing_functions.py
```

### Comparing `baserun-1.0.0b7/LICENSE` & `baserun-1.0.0b8/LICENSE`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b7/PKG-INFO` & `baserun-1.0.0b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 1.0.0b7
+Version: 1.0.0b8
 Summary: tools for testing, debugging, and evaluating llm features.
 Author-email: Erik Peterson <erik@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,15 +43,15 @@
 **[Baserun](https://baserun.ai)** is the testing and observability platform for LLM apps.
 
 # Quick Start
 
 ## 1. Install Baserun
 
 ```bash
-pip install baserun==1.0.0b6
+pip install baserun==1.0.0b8
 ```
 
 ## 2. Set the Baserun API key
 Create an account at [https://baserun.ai](https://baserun.ai). Then generate an API key for your project in the [settings](https://baserun.ai/settings) tab. Set it as an environment variable:
 
 ```bash
 export BASERUN_API_KEY="your_api_key_here"
@@ -156,15 +156,15 @@
 ## Tags
 
 You can add tags either to the traced OpenAI object or to the completion. There are several different types of tags:
 
 - `log`: Any arbitrary logs you want to attach to a trace or completion
 - `feedback`: Any score-based feedback given from users (e.g. thumbs up/down, star rating)
 - `variable`: Any variables used, e.g. while rendering a template
-- `annotate`: Any arbitrary attributes you want to attach to a trace or completion
+- `tag`: Any arbitrary attributes you want to attach to a trace or completion
 
 Each tag type has functions on traced OpenAI objects and completions. Each tag function can accept a `metadata` parameter which is an arbitrary dictionary with any values you might want to capture.
 
 ```python
 from baserun import OpenAI
 
 def example():
```

### Comparing `baserun-1.0.0b7/README.md` & `baserun-1.0.0b8/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 **[Baserun](https://baserun.ai)** is the testing and observability platform for LLM apps.
 
 # Quick Start
 
 ## 1. Install Baserun
 
 ```bash
-pip install baserun==1.0.0b6
+pip install baserun==1.0.0b8
 ```
 
 ## 2. Set the Baserun API key
 Create an account at [https://baserun.ai](https://baserun.ai). Then generate an API key for your project in the [settings](https://baserun.ai/settings) tab. Set it as an environment variable:
 
 ```bash
 export BASERUN_API_KEY="your_api_key_here"
@@ -122,15 +122,15 @@
 ## Tags
 
 You can add tags either to the traced OpenAI object or to the completion. There are several different types of tags:
 
 - `log`: Any arbitrary logs you want to attach to a trace or completion
 - `feedback`: Any score-based feedback given from users (e.g. thumbs up/down, star rating)
 - `variable`: Any variables used, e.g. while rendering a template
-- `annotate`: Any arbitrary attributes you want to attach to a trace or completion
+- `tag`: Any arbitrary attributes you want to attach to a trace or completion
 
 Each tag type has functions on traced OpenAI objects and completions. Each tag function can accept a `metadata` parameter which is an arbitrary dictionary with any values you might want to capture.
 
 ```python
 from baserun import OpenAI
 
 def example():
```

### Comparing `baserun-1.0.0b7/baserun/api.py` & `baserun-1.0.0b8/baserun/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 import asyncio
 import atexit
 import json
 import logging
 import os
+from datetime import datetime
 from multiprocessing import Process, Queue
 from queue import Empty
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Optional, Union
 
 import httpx
 
 from baserun.utils import count_prompt_tokens, deep_merge
 
 if TYPE_CHECKING:
-    from baserun.wrappers.openai import (
-        WrappedAsyncStream,
-        WrappedChatCompletion,
-        WrappedOpenAIBaseClient,
-        WrappedSyncStream,
-    )
+    try:
+        from baserun.wrappers.openai import (
+            WrappedAsyncStream,
+            WrappedChatCompletion,
+            WrappedOpenAIBaseClient,
+            WrappedSyncStream,
+        )
+    except ImportError:
+        pass
+
+    try:
+        from baserun.wrappers.anthropic import WrappedAnthropicBaseClient, WrappedMessage
+    except ImportError:
+        pass
 
 logger = logging.getLogger(__name__)
 
 exporter_queue: Queue = Queue()
 tasks: List[asyncio.Task] = []  # Make tasks a global variable
 exporter_process: Union[Process, None] = None
 
@@ -118,15 +127,15 @@
         exporter_queue.close()
         exporter_queue.join_thread()
 
 
 class ApiClient:
     def __init__(
         self,
-        client: Union["WrappedOpenAIBaseClient"],
+        client: Union["WrappedOpenAIBaseClient", "WrappedAnthropicBaseClient"],
         api_key: Optional[str] = None,
         base_url: Optional[str] = None,
     ):
         self.environment = os.getenv("BASERUN_ENVIRONMENT", os.getenv("ENVIRONMENT", "production"))
         self.client = client
 
         atexit.register(self.exit_handler)
@@ -135,97 +144,143 @@
             base_url or os.getenv("BASERUN_API_URL") or "https://app.baserun.ai",
             api_key or os.getenv("BASERUN_API_KEY") or "",
         )
 
     def exit_handler(self, *args) -> None:
         stop_worker()
 
-    def submit_completion(self, completion: "WrappedChatCompletion"):
+    def submit_completion(self, completion: Union["WrappedChatCompletion", "WrappedMessage"]):
         dict_items = completion.model_dump()
         dict_items.pop("client", None)
-        start_timestamp = dict_items.pop("start_timestamp", None)
-        end_timestamp = dict_items.pop("end_timestamp", None)
-        first_token_timestamp = dict_items.pop("first_token_timestamp", None)
+
+        choices = dict_items.pop("choices", [])
+        contents = dict_items.pop("content", None)
+        if not choices and contents:
+            for content in contents:
+                choices.append({"message": {"content": content.get("text", ""), "role": "assistant"}})
+
+        usage = dict_items.pop("usage", {})
+        if usage:
+            completion_tokens = usage.get("completion_tokens", usage.get("output_tokens", 0))
+            prompt_tokens = usage.get("prompt_tokens", usage.get("input_tokens", 0))
+            dict_items["usage"] = {
+                "completion_tokens": completion_tokens,
+                "prompt_tokens": prompt_tokens,
+                "total_tokens": usage.get("total_tokens", completion_tokens + prompt_tokens),
+            }
+
+        start_timestamp = dict_items.pop("start_timestamp", datetime.now())
+        first_token_timestamp = dict_items.pop("first_token_timestamp", datetime.now())
+        end_timestamp = dict_items.pop("end_timestamp", datetime.now())
+
         input_messages = []
         for message in dict_items.pop("input_messages", []):
-            tool_calls = message.pop("tool_calls", [])
-            input_messages.append({**message, "tool_calls": [*tool_calls]})
+            message_dict = {**message}
+            if "tool_calls" in message:
+                tool_calls = message.pop("tool_calls", [])
+                message_dict["tool_calls"] = [*tool_calls]
+
+            content = message.get("content", None)
+            if isinstance(content, Iterator):
+                message_dict["content"] = json.dumps([c for c in content])
+
+            input_messages.append(message_dict)
 
-        output = {
+        data = {
             **dict_items,
+            "choices": choices,
             "name": completion.name,
             "trace_id": completion.trace_id,
             "tool_results": completion.tool_results,
             "evals": [e.model_dump() for e in completion.evals if e.score is not None],
             "tags": [tag.model_dump() for tag in completion.tags],
             "config_params": dict_items.pop("config_params", {}),
             "environment": self.environment,
             "input_messages": input_messages,
             "trace": self._trace_data(),
             "start_timestamp": start_timestamp.isoformat(),
             "end_timestamp": end_timestamp.isoformat() if end_timestamp else None,
             "first_token_timestamp": first_token_timestamp.isoformat() if first_token_timestamp else None,
             "request_id": self.client.request_ids.get(completion.id),
         }
-        logger.debug(f"Submitting completion:\n{json.dumps(output, indent=2)}")
-        self._post("completions", output)
+        logger.debug(f"Submitting completion:\n{json.dumps(data, indent=2)}")
+        self._post("completions", data)
 
     def submit_stream(self, stream: Union["WrappedAsyncStream", "WrappedSyncStream"]):
         if not stream.id:
             return
 
-        merged_choice = deep_merge([c.model_dump() for c in stream.captured_choices])
-        merged_choice.pop("delta", None)
-        merged_delta = deep_merge([c.delta.model_dump() for c in stream.captured_choices])
-        merged_choice["message"] = merged_delta
+        choices = []
+        usage = {
+            "completion_tokens": 0,
+            "prompt_tokens": 0,
+            "total_tokens": 0,
+        }
+        if hasattr(stream, "captured_choices"):
+            merged_choice = deep_merge([c.model_dump() for c in stream.captured_choices])
+            merged_choice.pop("delta", None)
+            merged_delta = deep_merge([c.delta.model_dump() for c in stream.captured_choices])
+            merged_choice["message"] = merged_delta
+            choices.append(merged_choice)
+            usage = {
+                "completion_tokens": len(stream.captured_choices) + 1,
+                "prompt_tokens": count_prompt_tokens(stream.input_messages),
+                "total_tokens": count_prompt_tokens(stream.input_messages) + len(stream.captured_choices) + 1,
+            }
+        elif hasattr(stream, "captured_messages"):
+            for message in stream.captured_messages:
+                usage["completion_tokens"] += message.usage.output_tokens
+                usage["prompt_tokens"] += message.usage.input_tokens
+                choices.append(message.model_dump())
+
+        usage["total_tokens"] = usage["completion_tokens"] + usage["prompt_tokens"]
 
-        output = {
+        config_params = stream.config_params or {}
+        config_params.pop("event_handler", None)
+
+        data = {
             "id": stream.id,
             "name": stream.name,
             "completion_id": stream.completion_id,
-            "model": stream.config_params.get("model"),
+            "model": config_params.get("model"),
             "trace_id": stream.trace_id,
             "tags": [tag.model_dump() for tag in stream.tags],
             "tool_results": stream.tool_results,
             "evals": [e.model_dump() for e in stream.evals if e.score is not None],
             "input_messages": stream.input_messages,
-            "choices": [merged_choice],
-            "usage": {
-                "completion_tokens": len(stream.captured_choices) + 1,
-                "prompt_tokens": count_prompt_tokens(stream.input_messages),
-                "total_tokens": count_prompt_tokens(stream.input_messages) + len(stream.captured_choices) + 1,
-            },
-            "config_params": stream.config_params or {},
+            "choices": choices,
+            "usage": usage,
+            "config_params": config_params,
             "start_timestamp": stream.start_timestamp.isoformat(),
             "end_timestamp": stream.end_timestamp.isoformat() if stream.end_timestamp else None,
             "first_token_timestamp": stream.first_token_timestamp.isoformat() if stream.first_token_timestamp else None,
             "request_id": self.client.request_ids.get(stream.id),
             "environment": self.environment,
             "trace": self._trace_data(),
         }
-        logger.debug(f"Submitting streamed completion:\n{json.dumps(output, indent=2)}")
-        self._post("completions", output)
+        logger.debug(f"Submitting streamed completion:\n{json.dumps(data, indent=2)}")
+        self._post("completions", data)
 
     def submit_trace(self):
-        output = self._trace_data()
+        data = self._trace_data()
 
-        logger.debug(f"Submitting trace:\n{json.dumps(output, indent=2)}")
-        self._post("traces", output)
+        logger.debug(f"Submitting trace:\n{json.dumps(data, indent=2)}")
+        self._post("traces", data)
 
     def _post(self, endpoint: str, data: Dict[str, Any]):
         exporter_queue.put({"endpoint": endpoint, "data": data})
 
     def _trace_data(self) -> Dict[str, Any]:
         return {
             "id": self.client.trace_id,
             "name": self.client.name,
             "tags": [tag.model_dump() for tag in self.client.tags],
             "evals": [e.model_dump() for e in self.client.evals if e.score is not None],
             "environment": self.environment,
-            "result": self.client.result,
+            "output": self.client.output,
             "start_timestamp": self.client.start_timestamp.isoformat(),
             "end_timestamp": self.client.end_timestamp.isoformat() if self.client.end_timestamp else None,
             "error": self.client.error,
             "end_user_identifier": self.client.user,
             "end_user_session_identifier": self.client.session,
             "metadata": self.client.metadata,
         }
```

### Comparing `baserun-1.0.0b7/baserun/integrations/llamaindex.py` & `baserun-1.0.0b8/baserun/integrations/llamaindex.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b7/baserun/mixins.py` & `baserun-1.0.0b8/baserun/mixins.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,44 @@
 
 class CompletionMixin(ABC):
     tags: List[Tag]
     evals: List[CompletionEval]
     completion_id: str
     tool_results: List[Dict[str, Any]]
 
-    def annotate(self, key: str, value: str, metadata: Optional[Dict[str, Any]] = None):
+    def _clean_kwargs(self, kwargs: Dict[str, Any]) -> Dict[str, Any]:
+        return {
+            k: v
+            for k, v in kwargs.items()
+            if k
+            not in [
+                "name",
+                "error",
+                "completion_id",
+                "trace_id",
+                "template",
+                "config_params",
+                "start_timestamp",
+                "end_timestamp",
+                "first_token_timestamp",
+                "tool_results",
+                "tags",
+                "evals",
+                "input_messages",
+            ]
+        }
+
+    def tag(
+        self, key: str, value: str, metadata: Optional[Dict[str, Any]] = None, tag_type: Optional[str] = "annotation"
+    ):
         self.tags.append(
             Tag(
                 target_type="completion",
                 target_id=self.completion_id,
-                tag_type="annotation",
+                tag_type=tag_type,
                 key=key,
                 value=value,
                 metadata=metadata or {},
             )
         )
         self.submit_to_baserun()
 
@@ -105,23 +129,25 @@
         pass
 
 
 class ClientMixin(ABC):
     tags: List[Tag]
     evals: List["TraceEval"]
     trace_id: str
-    result: Optional[str]
+    output: Optional[str]
     integrations: List[Integration]
 
-    def annotate(self, key: str, value: str, metadata: Optional[Dict[str, Any]] = None):
+    def tag(
+        self, key: str, value: str, metadata: Optional[Dict[str, Any]] = None, tag_type: Optional[str] = "annotation"
+    ):
         self.tags.append(
             Tag(
                 target_type="trace",
                 target_id=self.trace_id,
-                tag_type="annotation",
+                tag_type=tag_type,
                 key=key,
                 value=value,
                 metadata=metadata or {},
             )
         )
 
     def eval(self, name: str, score: Optional[int] = None, metadata: Optional[Dict[str, Any]] = None) -> "TraceEval":
```

### Comparing `baserun-1.0.0b7/baserun/models/evals.py` & `baserun-1.0.0b8/baserun/models/evals.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,19 +77,19 @@
     def model_dump(self, *args, **kwargs):
         dumped = super().model_dump()
         dumped["timestamp"] = dumped.pop("timestamp").isoformat()
         return dumped
 
     def not_includes(self, expected: str, actual: Optional[str] = None) -> bool:
         if not actual:
-            actual = self.target.result or ""
+            actual = self.target.output or ""
 
         result = actual not in expected
         self.score = 1 if result else 0
         self.target.submit_to_baserun()
         return result
 
     def includes(self, expected: str, actual: Optional[str] = None) -> bool:
-        result = expected in (actual or self.target.result or "")
+        result = expected in (actual or self.target.output or "")
         self.score = 1 if result else 0
         self.target.submit_to_baserun()
         return result
```

### Comparing `baserun-1.0.0b7/baserun/models/tags.py` & `baserun-1.0.0b8/baserun/models/tags.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b7/baserun/pytest_plugin.py` & `baserun-1.0.0b8/baserun/pytest_plugin.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,7 +17,11 @@
         task.cancel()
     api.tasks = []
 
 
 def pytest_sessionstart(session):
     # This will stop start_worker from starting worker threads
     api.exporter_thread = "Dummy"
+
+
+def pytest_sessionfinish(session, exitstatus):
+    api.exporter_queue.close()
```

### Comparing `baserun-1.0.0b7/baserun/utils.py` & `baserun-1.0.0b8/baserun/utils.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b7/baserun/wrappers/openai.py` & `baserun-1.0.0b8/baserun/wrappers/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     def __iter__(self) -> Iterator[ChatCompletionChunk]:  # type: ignore[override]
         for item in self._iterator:
             yield item
 
     def __stream__(self) -> Iterator[ChatCompletionChunk]:
         stream = super().__stream__()
         for item in stream:
-            # TODO? Support n > 1
+            # Assemble deltas here instead of in api
             self.captured_choices.append(item.choices[0])
             self.id = item.id
             yield item
 
         self.submit_to_baserun()
 
 
@@ -329,15 +329,15 @@
         metadata: Optional[Dict[str, Any]] = None,
     ):
         self.name = name or ".".join([v for v in [client.organization, client.__class__.__name__] if v])
         self.tags: List[Tag] = []
         self.evals: List[TraceEval] = []
         self.client = client
         self.trace_id = trace_id or str(uuid4())
-        self._result = None
+        self._output = None
         self.error: Union[str, None] = None
         self.user = user
         self.session = session
         self.start_timestamp = datetime.now(timezone.utc)
         self.end_timestamp: Union[datetime, None] = None
         self.api_client = api_client or ApiClient(self, api_key=api_key)
         self.metadata = metadata or {}
@@ -348,20 +348,20 @@
             from baserun.integrations.llamaindex import LLamaIndexInstrumentation
 
             self.integrate(LLamaIndexInstrumentation)
         except ImportError:
             pass
 
     @property
-    def result(self):
-        return self._result
+    def output(self):
+        return self._output
 
-    @result.setter
-    def result(self, value):
-        self._result = value
+    @output.setter
+    def output(self, value):
+        self._output = value
         self.submit_to_baserun()
 
     def submit_to_baserun(self):
         if self.api_client:
             self.api_client.submit_trace()
```

### Comparing `baserun-1.0.0b7/baserun.egg-info/PKG-INFO` & `baserun-1.0.0b8/baserun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 1.0.0b7
+Version: 1.0.0b8
 Summary: tools for testing, debugging, and evaluating llm features.
 Author-email: Erik Peterson <erik@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,15 +43,15 @@
 **[Baserun](https://baserun.ai)** is the testing and observability platform for LLM apps.
 
 # Quick Start
 
 ## 1. Install Baserun
 
 ```bash
-pip install baserun==1.0.0b6
+pip install baserun==1.0.0b8
 ```
 
 ## 2. Set the Baserun API key
 Create an account at [https://baserun.ai](https://baserun.ai). Then generate an API key for your project in the [settings](https://baserun.ai/settings) tab. Set it as an environment variable:
 
 ```bash
 export BASERUN_API_KEY="your_api_key_here"
@@ -156,15 +156,15 @@
 ## Tags
 
 You can add tags either to the traced OpenAI object or to the completion. There are several different types of tags:
 
 - `log`: Any arbitrary logs you want to attach to a trace or completion
 - `feedback`: Any score-based feedback given from users (e.g. thumbs up/down, star rating)
 - `variable`: Any variables used, e.g. while rendering a template
-- `annotate`: Any arbitrary attributes you want to attach to a trace or completion
+- `tag`: Any arbitrary attributes you want to attach to a trace or completion
 
 Each tag type has functions on traced OpenAI objects and completions. Each tag function can accept a `metadata` parameter which is an arbitrary dictionary with any values you might want to capture.
 
 ```python
 from baserun import OpenAI
 
 def example():
```

### Comparing `baserun-1.0.0b7/baserun.egg-info/SOURCES.txt` & `baserun-1.0.0b8/baserun.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -16,9 +16,10 @@
 baserun.egg-info/top_level.txt
 baserun/integrations/integration.py
 baserun/integrations/llamaindex.py
 baserun/models/__init__.py
 baserun/models/evals.py
 baserun/models/tags.py
 baserun/wrappers/__init__.py
+baserun/wrappers/anthropic.py
 baserun/wrappers/openai.py
 tests/testing_functions.py
```

### Comparing `baserun-1.0.0b7/pyproject.toml` & `baserun-1.0.0b8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "baserun"
-version = "1.0.0b7"
+version = "1.0.0b8"
 description = "tools for testing, debugging, and evaluating llm features."
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Erik Peterson", email = "erik@baserun.ai" }]
 requires-python = ">=3.8, <3.12"
 dependencies = ["httpx[http2]>=0.24.0"]
```

### Comparing `baserun-1.0.0b7/tests/testing_functions.py` & `baserun-1.0.0b8/tests/testing_functions.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,15 @@
         "tool_calls": [tool_call.model_dump() for tool_call in tool_calls],
     }
     messages.append(assistant_message)
     messages.append(
         {"role": "tool", "content": "wow", "tool_call_id": assistant_message.get("tool_calls")[0].get("id")}
     )
     client.chat.completions.create(
+        name="openai_chat_tools tool response",
         model="gpt-4o",
         messages=messages,
         tools=tools,
     )
 
     return tool_calls
 
@@ -211,30 +212,30 @@
     finally:
         openai.api_type = original_api_type
 
 
 def openai_chat_response_format(prompt="What is the capital of the US?") -> str:
     client = init(OpenAI())
     completion = client.chat.completions.create(
-        model="gpt-4-turbo",
+        model="gpt-4o",
         messages=[
             {"role": "system", "content": "Respond to the following question in JSON"},
             {"role": "user", "content": prompt},
         ],
         response_format={"type": "json_object"},
     )
     content = completion.choices[0].message.content
     completion.eval("openai_chat.content").includes("Washington")
     return content
 
 
 def openai_chat_seed(prompt="What is the capital of the US?") -> str:
     client = init(OpenAI())
     completion = client.chat.completions.create(
-        model="gpt-4-turbo",
+        model="gpt-4o",
         messages=[{"role": "user", "content": prompt}],
         seed=1234,
     )
     content = completion.choices[0].message.content
     completion.eval("openai_chat.content").includes("Washington")
     return content
 
@@ -252,53 +253,57 @@
     "Question & Answer": [
         {"role": "system", "content": "Respond to all messages in the form of a limerick"},
         {"role": "user", "content": "{question}"},
     ]
 }
 
 
-def use_template(question="What is the capital of the US?", template_name: str = "Question & Answer"):
-    unformatted_messages = TEMPLATES.get(template_name)
-    prompt = [
-        {"role": message["role"], "content": message["content"].format(question=question)}
-        for message in unformatted_messages
-    ]
+def use_template(
+    template="Answer this question in the form of a limerick: {question}", question="What is the capital of the US?"
+) -> str:
+    prompt = [{"role": "user", "content": template.format(question=question)}]
 
     client = init(OpenAI(), name="use_template")
     completion = client.chat.completions.create(
-        model="gpt-4-turbo", messages=prompt, template=template_name, name="use_template completion"
+        model="gpt-4o",
+        messages=prompt,
+        template=template,
+        variables={"question": question},
+        name="use_template completion",
     )
     content = completion.choices[0].message.content
     completion.eval("openai_chat.content").includes("Washington")
     return content
 
 
-async def use_template_async(question="What is the capital of the US?", template_name: str = "Question & Answer"):
-    unformatted_messages = TEMPLATES.get(template_name)
-    prompt = [
-        {"role": message["role"], "content": message["content"].format(question=question)}
-        for message in unformatted_messages
-    ]
+async def use_template_async(
+    template="Answer this question in the form of a limerick: {question}", question="What is the capital of the US?"
+) -> str:
+    prompt = [{"role": "user", "content": template.format(question=question)}]
 
-    client = init(AsyncOpenAI(), name="use_template_async")
+    client = init(AsyncOpenAI(), name="use_template async")
     completion = await client.chat.completions.create(
-        model="gpt-4-turbo", messages=prompt, template=template_name, name="use_template_async completion"
+        model="gpt-4o",
+        messages=prompt,
+        template=template,
+        variables={"question": question},
+        name="use_template async completion",
     )
     content = completion.choices[0].message.content
     completion.eval("openai_chat.content").includes("Washington")
     return content
 
 
 def use_sessions(
     prompt="What is the capital of the US?", user_identifier="example@test.com", session_identifier="session-123"
 ) -> str:
     client = init(OpenAI(), user=user_identifier, session=session_identifier, name="use_sessions")
     completion = client.chat.completions.create(
         name="use_sessions completion",
-        model="gpt-4-turbo",
+        model="gpt-4o",
         messages=[{"role": "user", "content": prompt}],
     )
     return completion.choices[0].message.content
 
 
 def create_full_trace(question="What is the capital of the US?") -> str:
     client = init(OpenAI(), name="Full Trace")
@@ -317,15 +322,15 @@
         name="question_feedback",
         score=0.8,
         metadata={"comment": "This is correct but is too concise"},
     )
     completion.eval("Contains answer").includes("Washington")
     completion.log(name="Extracted content", message=content)
     completion.submit_to_baserun()
-    client.result = content
+    client.output = content
     client.feedback("content", 0.9, metadata={"comment": "This is a great answer"})
     client.eval("Contains answer").includes(expected="Washington")
     return content
 
 
 def use_input_variables():
     client = init(OpenAI())
```

