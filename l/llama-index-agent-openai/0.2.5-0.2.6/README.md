# Comparing `tmp/llama_index_agent_openai-0.2.5.tar.gz` & `tmp/llama_index_agent_openai-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_agent_openai-0.2.5.tar", max compression
+gzip compressed data, was "llama_index_agent_openai-0.2.6.tar", max compression
```

## Comparing `llama_index_agent_openai-0.2.5.tar` & `llama_index_agent_openai-0.2.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       39 2024-05-14 20:54:26.593044 llama_index_agent_openai-0.2.5/README.md
--rw-r--r--   0        0        0      342 2024-05-14 20:54:26.593044 llama_index_agent_openai-0.2.5/llama_index/agent/openai/__init__.py
--rw-r--r--   0        0        0     4745 2024-05-14 20:54:26.593044 llama_index_agent_openai-0.2.5/llama_index/agent/openai/base.py
--rw-r--r--   0        0        0    18955 2024-05-14 20:54:26.593044 llama_index_agent_openai-0.2.5/llama_index/agent/openai/openai_assistant_agent.py
--rw-r--r--   0        0        0    28597 2024-05-14 20:54:26.593044 llama_index_agent_openai-0.2.5/llama_index/agent/openai/step.py
--rw-r--r--   0        0        0      772 2024-05-14 20:54:26.593044 llama_index_agent_openai-0.2.5/llama_index/agent/openai/utils.py
--rw-r--r--   0        0        0     1522 2024-05-14 20:54:26.593044 llama_index_agent_openai-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 llama_index_agent_openai-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-05-31 04:53:38.047158 llama_index_agent_openai-0.2.6/README.md
+-rw-r--r--   0        0        0      342 2024-05-31 04:53:38.047158 llama_index_agent_openai-0.2.6/llama_index/agent/openai/__init__.py
+-rw-r--r--   0        0        0     4745 2024-05-31 04:53:38.047158 llama_index_agent_openai-0.2.6/llama_index/agent/openai/base.py
+-rw-r--r--   0        0        0    19580 2024-05-31 04:53:38.047158 llama_index_agent_openai-0.2.6/llama_index/agent/openai/openai_assistant_agent.py
+-rw-r--r--   0        0        0    28901 2024-05-31 04:53:38.047158 llama_index_agent_openai-0.2.6/llama_index/agent/openai/step.py
+-rw-r--r--   0        0        0      427 2024-05-31 04:53:38.047158 llama_index_agent_openai-0.2.6/llama_index/agent/openai/utils.py
+-rw-r--r--   0        0        0     1522 2024-05-31 04:53:38.047158 llama_index_agent_openai-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 llama_index_agent_openai-0.2.6/PKG-INFO
```

### Comparing `llama_index_agent_openai-0.2.5/llama_index/agent/openai/base.py` & `llama_index_agent_openai-0.2.6/llama_index/agent/openai/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai-0.2.5/llama_index/agent/openai/openai_assistant_agent.py` & `llama_index_agent_openai-0.2.6/llama_index/agent/openai/openai_assistant_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """OpenAI Assistant Agent."""
 
 import asyncio
 import json
 import logging
 import time
 from typing import Any, Dict, List, Optional, Tuple, Union, cast
-
-from llama_index.agent.openai.utils import get_function_by_name
+from llama_index.core.agent.function_calling.step import (
+    build_error_tool_output,
+    build_missing_tool_message,
+    get_function_by_name,
+)
 from llama_index.core.agent.types import BaseAgent
 from llama_index.core.base.llms.types import ChatMessage, MessageRole
 from llama_index.core.callbacks import (
     CallbackManager,
     CBEventType,
     EventPayload,
     trace_method,
@@ -65,23 +68,35 @@
     """Call a function and return the output as a string."""
     from openai.types.beta.threads.required_action_function_tool_call import Function
 
     fn_obj = cast(Function, fn_obj)
     # TMP: consolidate with other abstractions
     name = fn_obj.name
     arguments_str = fn_obj.arguments
+
     if verbose:
         print("=== Calling Function ===")
         print(f"Calling function: {name} with args: {arguments_str}")
+
     tool = get_function_by_name(tools, name)
-    argument_dict = json.loads(arguments_str)
-    output = tool(**argument_dict)
-    if verbose:
-        print(f"Got output: {output!s}")
-        print("========================")
+    if tool is not None:
+        argument_dict = json.loads(arguments_str)
+        output = tool(**argument_dict)
+
+        if verbose:
+            print(f"Got output: {output!s}")
+            print("========================")
+    else:
+        err_msg = build_missing_tool_message(name)
+        output = build_error_tool_output(name, arguments_str, err_msg)
+
+        if verbose:
+            print(err_msg)
+            print("========================")
+
     return (
         ChatMessage(
             content=str(output),
             role=MessageRole.FUNCTION,
             additional_kwargs={
                 "name": fn_obj.name,
             },
@@ -96,24 +111,36 @@
     """Call an async function and return the output as a string."""
     from openai.types.beta.threads.required_action_function_tool_call import Function
 
     fn_obj = cast(Function, fn_obj)
     # TMP: consolidate with other abstractions
     name = fn_obj.name
     arguments_str = fn_obj.arguments
+
     if verbose:
         print("=== Calling Function ===")
         print(f"Calling function: {name} with args: {arguments_str}")
+
     tool = get_function_by_name(tools, name)
-    argument_dict = json.loads(arguments_str)
-    async_tool = adapt_to_async_tool(tool)
-    output = await async_tool.acall(**argument_dict)
-    if verbose:
-        print(f"Got output: {output!s}")
-        print("========================")
+    if tool is not None:
+        argument_dict = json.loads(arguments_str)
+        tool = adapt_to_async_tool(tool)
+        output = await tool.acall(**argument_dict)
+
+        if verbose:
+            print(f"Got output: {output!s}")
+            print("========================")
+    else:
+        err_msg = build_missing_tool_message(name)
+        output = build_error_tool_output(name, arguments_str, err_msg)
+
+        if verbose:
+            print(err_msg)
+            print("========================")
+
     return (
         ChatMessage(
             content=str(output),
             role=MessageRole.FUNCTION,
             additional_kwargs={
                 "name": fn_obj.name,
             },
@@ -349,14 +376,15 @@
         )
 
     def _run_function_calling(self, run: Any) -> List[ToolOutput]:
         """Run function calling."""
         tool_calls = run.required_action.submit_tool_outputs.tool_calls
         tool_output_dicts = []
         tool_output_objs: List[ToolOutput] = []
+
         for tool_call in tool_calls:
             fn_obj = tool_call.function
             _, tool_output = call_function(self._tools, fn_obj, verbose=self._verbose)
             tool_output_dicts.append(
                 {"tool_call_id": tool_call.id, "output": str(tool_output)}
             )
             tool_output_objs.append(tool_output)
@@ -404,15 +432,14 @@
             instructions=instructions_prefix,
         )
         from openai.types.beta.threads import Run
 
         run = cast(Run, run)
 
         sources = []
-
         while run.status in ["queued", "in_progress", "requires_action"]:
             run = self._client.beta.threads.runs.retrieve(
                 thread_id=self._thread_id, run_id=run.id
             )
             if run.status == "requires_action":
                 cur_tool_outputs = self._run_function_calling(run)
                 sources.extend(cur_tool_outputs)
```

### Comparing `llama_index_agent_openai-0.2.5/llama_index/agent/openai/step.py` & `llama_index_agent_openai-0.2.6/llama_index/agent/openai/step.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """OpenAI agent worker."""
 
 import asyncio
 import json
 import logging
 import uuid
 from functools import partial
-from threading import Thread
-from typing import Any, Dict, List, Callable, Optional, Tuple, Union, cast, get_args
+from typing import Any, Dict, List, Callable, Optional, Union, cast, get_args
 import re
 
 from llama_index.agent.openai.utils import resolve_tool_choice
+from llama_index.core.agent.function_calling.step import (
+    build_error_tool_output,
+    build_missing_tool_message,
+    get_function_by_name,
+)
 from llama_index.core.agent.types import (
     BaseAgentWorker,
     Task,
     TaskStep,
     TaskStepOutput,
 )
 from llama_index.core.agent.utils import add_user_step_to_memory
@@ -32,31 +36,25 @@
 )
 from llama_index.core.base.llms.types import ChatMessage, ChatResponse
 from llama_index.core.llms.llm import LLM
 from llama_index.core.memory import BaseMemory, ChatMemoryBuffer
 from llama_index.core.objects.base import ObjectRetriever
 from llama_index.core.settings import Settings
 from llama_index.core.tools import BaseTool, ToolOutput, adapt_to_async_tool
+from llama_index.core.tools.types import ToolMetadata
+from llama_index.core.types import Thread
 from llama_index.llms.openai import OpenAI
 from llama_index.llms.openai.utils import OpenAIToolCall
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.WARNING)
 
 DEFAULT_MAX_FUNCTION_CALLS = 5
 
 
-def get_function_by_name(tools: List[BaseTool], name: str) -> BaseTool:
-    """Get function by name."""
-    name_to_tool = {tool.metadata.name: tool for tool in tools}
-    if name not in name_to_tool:
-        raise ValueError(f"Tool with name {name} not found")
-    return name_to_tool[name]
-
-
 def call_tool_with_error_handling(
     tool: BaseTool,
     input_dict: Dict,
     error_message: Optional[str] = None,
     raise_error: bool = False,
 ) -> ToolOutput:
     """Call tool with error handling.
@@ -117,143 +115,14 @@
             content = match.group(2)  # This is the content within the quotes
             return {variable_name: content}
         raise ValueError(
             f"Error in calling tool {tool_call.function.name}: The input json block is malformed:\n```json\n{tool_call.function.arguments}\n```"
         )
 
 
-def call_function(
-    tools: List[BaseTool],
-    tool_call: OpenAIToolCall,
-    verbose: bool = False,
-    tool_call_parser: Optional[Callable[[OpenAIToolCall], Dict]] = None,
-) -> Tuple[ChatMessage, ToolOutput]:
-    """Call a function and return the output as a string."""
-    # validations to get passed mypy
-    assert tool_call.id is not None
-    assert tool_call.function is not None
-    assert tool_call.function.name is not None
-    assert tool_call.function.arguments is not None
-    tool_call_parser = tool_call_parser or default_tool_call_parser
-
-    id_ = tool_call.id
-    _function_call = tool_call.function
-    name = tool_call.function.name
-    arguments_str = tool_call.function.arguments
-    if verbose:
-        print("=== Calling Function ===")
-        print(f"Calling function: {name} with args: {arguments_str}")
-    tool = get_function_by_name(tools, name)
-    error_message: Optional[str] = None
-    try:
-        argument_dict = tool_call_parser(tool_call)
-    except ValueError as e:
-        error_message = str(e)
-        return (
-            ChatMessage(
-                content=error_message,
-                role=MessageRole.TOOL,
-                additional_kwargs={
-                    "name": name,
-                    "tool_call_id": id_,
-                },
-            ),
-            ToolOutput(
-                content=error_message,
-                tool_name=name,
-                raw_input={"args": arguments_str},
-                raw_output=error_message,
-                is_error=True,
-            ),
-        )
-
-    # Call tool
-    # Use default error message except if json parsing fails
-    output = call_tool_with_error_handling(
-        tool, argument_dict, error_message=error_message
-    )
-    if verbose:
-        print(f"Got output: {output!s}")
-        print("========================\n")
-    return (
-        ChatMessage(
-            content=str(output),
-            role=MessageRole.TOOL,
-            additional_kwargs={
-                "name": name,
-                "tool_call_id": id_,
-            },
-        ),
-        output,
-    )
-
-
-async def acall_function(
-    tools: List[BaseTool],
-    tool_call: OpenAIToolCall,
-    verbose: bool = False,
-    tool_call_parser: Optional[Callable[[OpenAIToolCall], Dict]] = None,
-) -> Tuple[ChatMessage, ToolOutput]:
-    """Call a function and return the output as a string."""
-    # validations to get passed mypy
-    assert tool_call.id is not None
-    assert tool_call.function is not None
-    assert tool_call.function.name is not None
-    assert tool_call.function.arguments is not None
-    tool_call_parser = tool_call_parser or default_tool_call_parser
-
-    id_ = tool_call.id
-    _function_call = tool_call.function
-    name = tool_call.function.name
-    arguments_str = tool_call.function.arguments
-    if verbose:
-        print("=== Calling Function ===")
-        print(f"Calling function: {name} with args: {arguments_str}")
-    tool = get_function_by_name(tools, name)
-    async_tool = adapt_to_async_tool(tool)
-    error_message: Optional[str] = None
-    try:
-        argument_dict = tool_call_parser(tool_call)
-    except ValueError as e:
-        error_message = str(e)
-        return (
-            ChatMessage(
-                content=error_message,
-                role=MessageRole.TOOL,
-                additional_kwargs={
-                    "name": name,
-                    "tool_call_id": id_,
-                },
-            ),
-            ToolOutput(
-                content=error_message,
-                tool_name=name,
-                raw_input={"args": arguments_str},
-                raw_output=error_message,
-                is_error=True,
-            ),
-        )
-
-    output = await async_tool.acall(**argument_dict)
-    if verbose:
-        print(f"Got output: {output!s}")
-        print("========================\n")
-    return (
-        ChatMessage(
-            content=str(output),
-            role=MessageRole.TOOL,
-            additional_kwargs={
-                "name": name,
-                "tool_call_id": id_,
-            },
-        ),
-        output,
-    )
-
-
 class OpenAIAgentWorker(BaseAgentWorker):
     """OpenAI Agent agent worker."""
 
     def __init__(
         self,
         tools: List[BaseTool],
         llm: OpenAI,
@@ -444,74 +313,197 @@
     def _call_function(
         self,
         tools: List[BaseTool],
         tool_call: OpenAIToolCall,
         memory: BaseMemory,
         sources: List[ToolOutput],
     ) -> bool:
-        function_call = tool_call.function
-        # validations to get passed mypy
-        assert function_call is not None
-        assert function_call.name is not None
-        assert function_call.arguments is not None
+        # validations to get past mypy
+        assert tool_call.id is not None
+        assert tool_call.function is not None
+        assert tool_call.function.name is not None
+        assert tool_call.function.arguments is not None
+
+        function_id = tool_call.id
+        function_name = tool_call.function.name
+        function_args_str = tool_call.function.arguments
 
-        tool = get_function_by_name(tools, function_call.name)
+        tool = get_function_by_name(tools, function_name)
 
         with self.callback_manager.event(
             CBEventType.FUNCTION_CALL,
             payload={
-                EventPayload.FUNCTION_CALL: function_call.arguments,
-                EventPayload.TOOL: tool.metadata,
+                EventPayload.FUNCTION_CALL: function_args_str,
+                EventPayload.TOOL: (
+                    tool.metadata
+                    if tool is not None
+                    else ToolMetadata(description="", name=function_name)
+                ),
             },
         ) as event:
-            function_message, tool_output = call_function(
-                tools,
-                tool_call,
-                verbose=self._verbose,
-                tool_call_parser=self.tool_call_parser,
-            )
+            """Call a function and return the output as a string."""
+            tool_call_parser = self.tool_call_parser or default_tool_call_parser
+
+            if self._verbose:
+                print("=== Calling Function ===")
+                print(
+                    f"Calling function: {function_name} with args: {function_args_str}"
+                )
+
+            error_message: Optional[str] = None
+
+            # Verify that tool arguments can be parsed into dict
+            try:
+                argument_dict = tool_call_parser(tool_call)
+            except ValueError as e:
+                error_message = str(e)
+
+            # Verify that the requested tool actually exists
+            if tool is None:
+                error_message = build_missing_tool_message(function_name)
+
+            # Call tool, or wrap error into output objects
+            if error_message is not None:
+                if self._verbose:
+                    print(error_message)
+                    print("========================\n")
+
+                function_message = ChatMessage(
+                    content=error_message,
+                    role=MessageRole.TOOL,
+                    additional_kwargs={
+                        "name": function_name,
+                        "tool_call_id": function_id,
+                    },
+                )
+                tool_output = build_error_tool_output(
+                    function_name, function_args_str, error_message
+                )
+            else:
+                tool_output = call_tool_with_error_handling(
+                    tool, argument_dict, error_message=error_message
+                )
+
+                if self._verbose:
+                    print(f"Got output: {tool_output!s}")
+                    print("========================\n")
+
+                function_message = ChatMessage(
+                    content=str(tool_output),
+                    role=MessageRole.TOOL,
+                    additional_kwargs={
+                        "name": function_name,
+                        "tool_call_id": function_id,
+                    },
+                )
+
             event.on_end(payload={EventPayload.FUNCTION_OUTPUT: str(tool_output)})
         sources.append(tool_output)
         memory.put(function_message)
 
-        return tool.metadata.return_direct and not tool_output.is_error
+        return (
+            tool.metadata.return_direct and not tool_output.is_error
+            if tool is not None
+            else False
+        )
 
     async def _acall_function(
         self,
         tools: List[BaseTool],
         tool_call: OpenAIToolCall,
         memory: BaseMemory,
         sources: List[ToolOutput],
     ) -> bool:
-        function_call = tool_call.function
-        # validations to get passed mypy
-        assert function_call is not None
-        assert function_call.name is not None
-        assert function_call.arguments is not None
+        # validations to get past mypy
+        assert tool_call.id is not None
+        assert tool_call.function is not None
+        assert tool_call.function.name is not None
+        assert tool_call.function.arguments is not None
+
+        function_id = tool_call.id
+        function_name = tool_call.function.name
+        function_args_str = tool_call.function.arguments
 
-        tool = get_function_by_name(tools, function_call.name)
+        tool = get_function_by_name(tools, function_name)
 
         with self.callback_manager.event(
             CBEventType.FUNCTION_CALL,
             payload={
-                EventPayload.FUNCTION_CALL: function_call.arguments,
-                EventPayload.TOOL: tool.metadata,
+                EventPayload.FUNCTION_CALL: function_args_str,
+                EventPayload.TOOL: (
+                    tool.metadata
+                    if tool is not None
+                    else ToolMetadata(description="", name=function_name)
+                ),
             },
         ) as event:
-            function_message, tool_output = await acall_function(
-                tools,
-                tool_call,
-                verbose=self._verbose,
-                tool_call_parser=self.tool_call_parser,
-            )
+            """Call a function and return the output as a string."""
+            tool_call_parser = self.tool_call_parser or default_tool_call_parser
+
+            if self._verbose:
+                print("=== Calling Function ===")
+                print(
+                    f"Calling function: {function_name} with args: {function_args_str}"
+                )
+
+            error_message: Optional[str] = None
+
+            # Verify that tool arguments can be parsed into dict
+            try:
+                argument_dict = tool_call_parser(tool_call)
+            except ValueError as e:
+                error_message = str(e)
+
+            # Verify that the requested tool actually exists
+            if tool is None:
+                error_message = build_missing_tool_message(function_name)
+
+            # Call tool, or wrap error into output objects
+            if error_message is not None:
+                if self._verbose:
+                    print(error_message)
+                    print("========================\n")
+
+                function_message = ChatMessage(
+                    content=error_message,
+                    role=MessageRole.TOOL,
+                    additional_kwargs={
+                        "name": function_name,
+                        "tool_call_id": function_id,
+                    },
+                )
+                tool_output = build_error_tool_output(
+                    function_name, function_args_str, error_message
+                )
+            else:
+                async_tool = adapt_to_async_tool(tool)
+                tool_output = await async_tool.acall(**argument_dict)
+
+                if self._verbose:
+                    print(f"Got output: {tool_output!s}")
+                    print("========================\n")
+
+                function_message = ChatMessage(
+                    content=str(tool_output),
+                    role=MessageRole.TOOL,
+                    additional_kwargs={
+                        "name": function_name,
+                        "tool_call_id": function_id,
+                    },
+                )
+
             event.on_end(payload={EventPayload.FUNCTION_OUTPUT: str(tool_output)})
         sources.append(tool_output)
         memory.put(function_message)
 
-        return tool.metadata.return_direct and not tool_output.is_error
+        return (
+            tool.metadata.return_direct and not tool_output.is_error
+            if tool is not None
+            else False
+        )
 
     def initialize_step(self, task: Task, **kwargs: Any) -> TaskStep:
         """Initialize step from task."""
         sources: List[ToolOutput] = []
         # temporary memory for new messages
         new_memory = ChatMemoryBuffer.from_defaults()
         # initialize task state
@@ -748,17 +740,15 @@
         return await self._arun_step(
             step, task, mode=ChatResponseMode.STREAM, tool_choice=tool_choice
         )
 
     def finalize_task(self, task: Task, **kwargs: Any) -> None:
         """Finalize task, after all the steps are completed."""
         # add new messages to memory
-        task.memory.set(
-            task.memory.get_all() + task.extra_state["new_memory"].get_all()
-        )
+        task.memory.put_messages(task.extra_state["new_memory"].get_all())
         # reset new memory
         task.extra_state["new_memory"].reset()
 
     def undo_step(self, task: Task, **kwargs: Any) -> Optional[TaskStep]:
         """Undo step from task.
 
         If this cannot be implemented, return None.
```

### Comparing `llama_index_agent_openai-0.2.5/pyproject.toml` & `llama_index_agent_openai-0.2.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index agent openai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-agent-openai"
 readme = "README.md"
-version = "0.2.5"
+version = "0.2.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.35"
+llama-index-core = "^0.10.41"
 llama-index-llms-openai = "^0.1.5"
 openai = ">=1.14.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
```

### Comparing `llama_index_agent_openai-0.2.5/PKG-INFO` & `llama_index_agent_openai-0.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-agent-openai
-Version: 0.2.5
+Version: 0.2.6
 Summary: llama-index agent openai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: llama-index-core (>=0.10.35,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.41,<0.11.0)
 Requires-Dist: llama-index-llms-openai (>=0.1.5,<0.2.0)
 Requires-Dist: openai (>=1.14.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Agent Integration: Openai
```

