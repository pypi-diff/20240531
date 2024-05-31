# Comparing `tmp/llama_index_agent_openai_legacy-0.1.4.tar.gz` & `tmp/llama_index_agent_openai_legacy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_agent_openai_legacy-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_agent_openai_legacy-0.1.5.tar", max compression
```

## Comparing `llama_index_agent_openai_legacy-0.1.4.tar` & `llama_index_agent_openai_legacy-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       46 2024-05-07 22:47:10.634523 llama_index_agent_openai_legacy-0.1.4/README.md
--rw-r--r--   0        0        0      412 2024-05-07 22:47:10.634523 llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/__init__.py
--rw-r--r--   0        0        0     7463 2024-05-07 22:47:10.634523 llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/context_retriever_agent.py
--rw-r--r--   0        0        0    22754 2024-05-07 22:47:10.634523 llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/openai_agent.py
--rw-r--r--   0        0        0      857 2024-05-07 22:47:10.634523 llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/retriever_openai_agent.py
--rw-r--r--   0        0        0      772 2024-05-07 22:47:10.634523 llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/utils.py
--rw-r--r--   0        0        0     1541 2024-05-07 22:47:10.634523 llama_index_agent_openai_legacy-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 llama_index_agent_openai_legacy-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-05-31 04:53:38.047158 llama_index_agent_openai_legacy-0.1.5/README.md
+-rw-r--r--   0        0        0      412 2024-05-31 04:53:38.047158 llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/__init__.py
+-rw-r--r--   0        0        0     7463 2024-05-31 04:53:38.047158 llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/context_retriever_agent.py
+-rw-r--r--   0        0        0    22767 2024-05-31 04:53:38.047158 llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/openai_agent.py
+-rw-r--r--   0        0        0      857 2024-05-31 04:53:38.047158 llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/retriever_openai_agent.py
+-rw-r--r--   0        0        0      772 2024-05-31 04:53:38.047158 llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/utils.py
+-rw-r--r--   0        0        0     1541 2024-05-31 04:53:38.047158 llama_index_agent_openai_legacy-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      666 1970-01-01 00:00:00.000000 llama_index_agent_openai_legacy-0.1.5/PKG-INFO
```

### Comparing `llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/context_retriever_agent.py` & `llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/context_retriever_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/openai_agent.py` & `llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/openai_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import asyncio
 import json
 import logging
 from abc import abstractmethod
-from threading import Thread
 from typing import Any, Dict, List, Optional, Tuple, Type, Union, cast, get_args
 
 from llama_index.agent.openai_legacy.utils import get_function_by_name
 from llama_index.core.agent.types import BaseAgent
 from llama_index.core.base.llms.types import ChatMessage, ChatResponse, MessageRole
 from llama_index.core.callbacks import (
     CallbackManager,
@@ -21,14 +20,15 @@
     StreamingAgentChatResponse,
 )
 from llama_index.core.llms.llm import LLM
 from llama_index.core.memory import BaseMemory, ChatMemoryBuffer
 from llama_index.core.objects.base import ObjectRetriever
 from llama_index.core.settings import Settings
 from llama_index.core.tools import BaseTool, ToolOutput, adapt_to_async_tool
+from llama_index.core.types import Thread
 from llama_index.llms.openai import OpenAI
 from llama_index.llms.openai.utils import OpenAIToolCall
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.WARNING)
 
 DEFAULT_MAX_FUNCTION_CALLS = 5
```

### Comparing `llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/retriever_openai_agent.py` & `llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/retriever_openai_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai_legacy-0.1.4/llama_index/agent/openai_legacy/utils.py` & `llama_index_agent_openai_legacy-0.1.5/llama_index/agent/openai_legacy/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_agent_openai_legacy-0.1.4/pyproject.toml` & `llama_index_agent_openai_legacy-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index agent openai-legacy integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-agent-openai-legacy"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.35"
+llama-index-core = "^0.10.41"
 llama-index-llms-openai = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
```

### Comparing `llama_index_agent_openai_legacy-0.1.4/PKG-INFO` & `llama_index_agent_openai_legacy-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-agent-openai-legacy
-Version: 0.1.4
+Version: 0.1.5
 Summary: llama-index agent openai-legacy integration
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
 Requires-Dist: llama-index-llms-openai (>=0.1.1,<0.2.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Agent Integration: Openai-Legacy
```

