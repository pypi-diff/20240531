# Comparing `tmp/llama_index_llms_langchain-0.1.3.tar.gz` & `tmp/llama_index_llms_langchain-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_langchain-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_llms_langchain-0.1.4.tar", max compression
```

## Comparing `llama_index_llms_langchain-0.1.3.tar` & `llama_index_llms_langchain-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       41 2024-02-13 13:53:01.666635 llama_index_llms_langchain-0.1.3/README.md
--rw-r--r--   0        0        0       85 2024-02-13 13:53:01.666849 llama_index_llms_langchain-0.1.3/llama_index/llms/langchain/__init__.py
--rw-r--r--   0        0        0     7816 2024-02-20 22:37:41.303784 llama_index_llms_langchain-0.1.3/llama_index/llms/langchain/base.py
--rw-r--r--   0        0        0     5203 2024-02-13 13:53:01.666999 llama_index_llms_langchain-0.1.3/llama_index/llms/langchain/utils.py
--rw-r--r--   0        0        0     1529 2024-02-21 17:44:31.671034 llama_index_llms_langchain-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      801 1970-01-01 00:00:00.000000 llama_index_llms_langchain-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       41 2024-05-31 04:53:38.099158 llama_index_llms_langchain-0.1.4/README.md
+-rw-r--r--   0        0        0       85 2024-05-31 04:53:38.099158 llama_index_llms_langchain-0.1.4/llama_index/llms/langchain/__init__.py
+-rw-r--r--   0        0        0     8196 2024-05-31 04:53:38.099158 llama_index_llms_langchain-0.1.4/llama_index/llms/langchain/base.py
+-rw-r--r--   0        0        0     5593 2024-05-31 04:53:38.099158 llama_index_llms_langchain-0.1.4/llama_index/llms/langchain/utils.py
+-rw-r--r--   0        0        0     1530 2024-05-31 04:53:38.099158 llama_index_llms_langchain-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      751 1970-01-01 00:00:00.000000 llama_index_llms_langchain-0.1.4/PKG-INFO
```

### Comparing `llama_index_llms_langchain-0.1.3/llama_index/llms/langchain/base.py` & `llama_index_llms_langchain-0.1.4/llama_index/llms/langchain/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from threading import Thread
 from typing import Any, Callable, Generator, Optional, Sequence
 
 from llama_index.core.base.llms.types import (
     ChatMessage,
     ChatResponse,
     ChatResponseAsyncGen,
     ChatResponseGen,
@@ -15,21 +14,38 @@
 from llama_index.core.callbacks import CallbackManager
 from llama_index.core.llms.callbacks import llm_chat_callback, llm_completion_callback
 from llama_index.core.base.llms.generic_utils import (
     completion_response_to_chat_response,
     stream_completion_response_to_chat_response,
 )
 from llama_index.core.llms.llm import LLM
-from llama_index.core.types import BaseOutputParser, PydanticProgramMode
+from llama_index.core.types import BaseOutputParser, PydanticProgramMode, Thread
 
 from langchain.base_language import BaseLanguageModel
 
 
 class LangChainLLM(LLM):
-    """Adapter for a LangChain LLM."""
+    """Adapter for a LangChain LLM.
+
+    Examples:
+        `pip install llama-index-llms-langchain`
+
+        ```python
+        from langchain_openai import ChatOpenAI
+
+        from llama_index.llms.langchain import LangChainLLM
+
+        llm = LangChainLLM(llm=ChatOpenAI(...))
+
+        response_gen = llm.stream_complete("What is the meaning of life?")
+
+        for r in response_gen:
+            print(r.delta, end="")
+        ```
+    """
 
     _llm: Any = PrivateAttr()
 
     def __init__(
         self,
         llm: "BaseLanguageModel",
         callback_manager: Optional[CallbackManager] = None,
```

### Comparing `llama_index_llms_langchain-0.1.3/llama_index/llms/langchain/utils.py` & `llama_index_llms_langchain-0.1.4/llama_index/llms/langchain/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from typing import List, Sequence
 
 from llama_index.core.base.llms.types import ChatMessage, LLMMetadata, MessageRole
 from llama_index.core.constants import AI21_J2_CONTEXT_WINDOW, COHERE_CONTEXT_WINDOW
 from llama_index.llms.anyscale.utils import anyscale_modelname_to_contextsize
+from llama_index.llms.fireworks.utils import fireworks_modelname_to_contextsize
 from llama_index.llms.openai.utils import openai_modelname_to_contextsize
 
 
 class LC:
     from llama_index.core.bridge.langchain import (
         AI21,
         AIMessage,
         BaseChatModel,
         BaseLanguageModel,
         BaseMessage,
         ChatAnyscale,
+        ChatFireworks,
         ChatMessage,
         ChatOpenAI,
         Cohere,
         FunctionMessage,
         HumanMessage,
         OpenAI,
         SystemMessage,
@@ -106,14 +108,21 @@
     elif isinstance(llm, LC.ChatAnyscale):
         return LLMMetadata(
             context_window=anyscale_modelname_to_contextsize(llm.model_name),
             num_output=llm.max_tokens or -1,
             is_chat_model=is_chat_model_,
             model_name=llm.model_name,
         )
+    elif isinstance(llm, LC.ChatFireworks):
+        return LLMMetadata(
+            context_window=fireworks_modelname_to_contextsize(llm.model_name),
+            num_output=llm.max_tokens or -1,
+            is_chat_model=is_chat_model_,
+            model_name=llm.model_name,
+        )
     elif isinstance(llm, LC.ChatOpenAI):
         return LLMMetadata(
             context_window=openai_modelname_to_contextsize(llm.model_name),
             num_output=llm.max_tokens or -1,
             is_chat_model=is_chat_model_,
             model_name=llm.model_name,
         )
```

### Comparing `llama_index_llms_langchain-0.1.3/pyproject.toml` & `llama_index_llms_langchain-0.1.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms langchain integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-langchain"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.1"
+llama-index-core = "^0.10.41"
 llama-index-llms-anyscale = "^0.1.1"
 langchain = "^0.1.3"
 llama-index-llms-openai = "^0.1.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
```

### Comparing `llama_index_llms_langchain-0.1.3/PKG-INFO` & `llama_index_llms_langchain-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-langchain
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index llms langchain integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: langchain (>=0.1.3,<0.2.0)
-Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.41,<0.11.0)
 Requires-Dist: llama-index-llms-anyscale (>=0.1.1,<0.2.0)
 Requires-Dist: llama-index-llms-openai (>=0.1.1,<0.2.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Langchain
```

