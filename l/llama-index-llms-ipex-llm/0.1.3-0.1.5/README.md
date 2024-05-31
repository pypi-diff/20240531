# Comparing `tmp/llama_index_llms_ipex_llm-0.1.3.tar.gz` & `tmp/llama_index_llms_ipex_llm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_ipex_llm-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_llms_ipex_llm-0.1.5.tar", max compression
```

## Comparing `llama_index_llms_ipex_llm-0.1.3.tar` & `llama_index_llms_ipex_llm-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      863 2024-05-23 15:25:44.679653 llama_index_llms_ipex_llm-0.1.3/README.md
--rw-r--r--   0        0        0       17 2024-05-23 15:25:44.679653 llama_index_llms_ipex_llm-0.1.3/llama_index/llms/ipex_llm/BUILD
--rw-r--r--   0        0        0       75 2024-05-23 15:25:44.679653 llama_index_llms_ipex_llm-0.1.3/llama_index/llms/ipex_llm/__init__.py
--rw-r--r--   0        0        0    21197 2024-05-23 15:25:44.679653 llama_index_llms_ipex_llm-0.1.3/llama_index/llms/ipex_llm/base.py
--rw-r--r--   0        0        0     2433 2024-05-23 15:25:44.679653 llama_index_llms_ipex_llm-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 llama_index_llms_ipex_llm-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      863 2024-05-31 04:53:38.099158 llama_index_llms_ipex_llm-0.1.5/README.md
+-rw-r--r--   0        0        0       17 2024-05-31 04:53:38.099158 llama_index_llms_ipex_llm-0.1.5/llama_index/llms/ipex_llm/BUILD
+-rw-r--r--   0        0        0       75 2024-05-31 04:53:38.099158 llama_index_llms_ipex_llm-0.1.5/llama_index/llms/ipex_llm/__init__.py
+-rw-r--r--   0        0        0    21176 2024-05-31 04:53:38.099158 llama_index_llms_ipex_llm-0.1.5/llama_index/llms/ipex_llm/base.py
+-rw-r--r--   0        0        0     2520 2024-05-31 04:53:38.099158 llama_index_llms_ipex_llm-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 llama_index_llms_ipex_llm-0.1.5/PKG-INFO
```

### Comparing `llama_index_llms_ipex_llm-0.1.3/README.md` & `llama_index_llms_ipex_llm-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_llms_ipex_llm-0.1.3/llama_index/llms/ipex_llm/base.py` & `llama_index_llms_ipex_llm-0.1.5/llama_index/llms/ipex_llm/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # This file is adapted from
 # https://github.com/run-llama/llama_index/blob/main/llama-index-integrations/
 # llms/llama-index-llms-huggingface/llama_index/llms/huggingface/base.py
 
 import logging
-from threading import Thread
 from typing import Any, Callable, List, Optional, Sequence, Literal
 
 import torch
 from llama_index.core.base.llms.types import (
     ChatMessage,
     ChatResponse,
     ChatResponseGen,
@@ -28,15 +27,15 @@
 from llama_index.core.llms.custom import CustomLLM
 
 from llama_index.core.base.llms.generic_utils import (
     completion_response_to_chat_response,
     stream_completion_response_to_chat_response,
     messages_to_prompt as generic_messages_to_prompt,
 )
-from llama_index.core.types import BaseOutputParser, PydanticProgramMode
+from llama_index.core.types import BaseOutputParser, PydanticProgramMode, Thread
 from transformers import (
     StoppingCriteria,
     StoppingCriteriaList,
 )
 from transformers import AutoTokenizer, LlamaTokenizer
```

### Comparing `llama_index_llms_ipex_llm-0.1.3/pyproject.toml` & `llama_index_llms_ipex_llm-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -26,28 +26,29 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms ipex-llm integration"
 license = "MIT"
 name = "llama-index-llms-ipex-llm"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-llama-index-core = "^0.10.0"
-ipex-llm = {allow-prereleases = true, extras = ["llama-index"], version = ">=2.1.0b20240514"}
+llama-index-core = "^0.10.41"
+ipex-llm = {allow-prereleases = true, extras = ["llama-index"], version = ">=2.1.0b20240529"}
 torch = {optional = true, source = "ipex-xpu-src-us", version = "2.1.0a0"}
 torchvision = {optional = true, source = "ipex-xpu-src-us", version = "0.16.0a0"}
 intel_extension_for_pytorch = {optional = true, source = "ipex-xpu-src-us", version = "2.1.10+xpu"}
 bigdl-core-xe-21 = {optional = true, version = "*"}
-bigdl-core-xe-esimd-21 = {optional = true, version = "*"}
+bigdl-core-xe-batch-21 = {optional = true, version = "*"}
+bigdl-core-xe-addons-21 = {optional = true, version = "*"}
 
 [tool.poetry.extras]
-xpu = ["bigdl-core-xe-21", "bigdl-core-xe-esimd-21", "intel_extension_for_pytorch", "torch", "torchvision"]
+xpu = ["bigdl-core-xe-21", "bigdl-core-xe-addons-21", "bigdl-core-xe-batch-21", "intel_extension_for_pytorch", "torch", "torchvision"]
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
 codespell = {extras = ["toml"], version = ">=v2.2.6"}
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
```

### Comparing `llama_index_llms_ipex_llm-0.1.3/PKG-INFO` & `llama_index_llms_ipex_llm-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-ipex-llm
-Version: 0.1.3
+Version: 0.1.5
 Summary: llama-index llms ipex-llm integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: xpu
 Requires-Dist: bigdl-core-xe-21 ; extra == "xpu"
-Requires-Dist: bigdl-core-xe-esimd-21 ; extra == "xpu"
+Requires-Dist: bigdl-core-xe-addons-21 ; extra == "xpu"
+Requires-Dist: bigdl-core-xe-batch-21 ; extra == "xpu"
 Requires-Dist: intel_extension_for_pytorch (==2.1.10+xpu) ; extra == "xpu"
-Requires-Dist: ipex-llm[llama-index] (>=2.1.0b20240514)
-Requires-Dist: llama-index-core (>=0.10.0,<0.11.0)
+Requires-Dist: ipex-llm[llama-index] (>=2.1.0b20240529)
+Requires-Dist: llama-index-core (>=0.10.41,<0.11.0)
 Requires-Dist: torch (==2.1.0a0) ; extra == "xpu"
 Requires-Dist: torchvision (==0.16.0a0) ; extra == "xpu"
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: IPEX-LLM
 
 [IPEX-LLM](https://github.com/intel-analytics/ipex-llm) is a PyTorch library for running LLM on Intel CPU and GPU (e.g., local PC with iGPU, discrete GPU such as Arc, Flex and Max) with very low latency. This module enables the use of LLMs optimized with `ipex-llm` in LlamaIndex pipelines.
```

