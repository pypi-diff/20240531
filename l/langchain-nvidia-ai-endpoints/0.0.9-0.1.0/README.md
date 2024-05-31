# Comparing `tmp/langchain_nvidia_ai_endpoints-0.0.9.tar.gz` & `tmp/langchain_nvidia_ai_endpoints-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_nvidia_ai_endpoints-0.0.9.tar", max compression
+gzip compressed data, was "langchain_nvidia_ai_endpoints-0.1.0.tar", max compression
```

## Comparing `langchain_nvidia_ai_endpoints-0.0.9.tar` & `langchain_nvidia_ai_endpoints-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-04-23 20:25:41.432902 langchain_nvidia_ai_endpoints-0.0.9/LICENSE
--rw-r--r--   0        0        0     9661 2024-04-23 20:25:41.432902 langchain_nvidia_ai_endpoints-0.0.9/README.md
--rw-r--r--   0        0        0     2140 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/__init__.py
--rw-r--r--   0        0        0    29908 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/_common.py
--rw-r--r--   0        0        0     7292 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/_statics.py
--rw-r--r--   0        0        0    10149 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/callbacks.py
--rw-r--r--   0        0        0    16465 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/chat_models.py
--rw-r--r--   0        0        0     6644 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/embeddings.py
--rw-r--r--   0        0        0     5735 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/image_gen.py
--rw-r--r--   0        0        0     7597 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/llm.py
--rw-r--r--   0        0        0        0 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/py.typed
--rw-r--r--   0        0        0     6525 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/reranking.py
--rw-r--r--   0        0        0    10047 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/tools.py
--rw-r--r--   0        0        0     2913 2024-04-23 20:25:41.440902 langchain_nvidia_ai_endpoints-0.0.9/pyproject.toml
--rw-r--r--   0        0        0    10561 1970-01-01 00:00:00.000000 langchain_nvidia_ai_endpoints-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-31 15:19:33.969915 langchain_nvidia_ai_endpoints-0.1.0/LICENSE
+-rw-r--r--   0        0        0    10269 2024-05-31 15:19:33.969915 langchain_nvidia_ai_endpoints-0.1.0/README.md
+-rw-r--r--   0        0        0     2145 2024-05-31 15:19:33.973915 langchain_nvidia_ai_endpoints-0.1.0/langchain_nvidia_ai_endpoints/__init__.py
+-rw-r--r--   0        0        0    21535 2024-05-31 15:19:33.973915 langchain_nvidia_ai_endpoints-0.1.0/langchain_nvidia_ai_endpoints/_common.py
+-rw-r--r--   0        0        0     9649 2024-05-31 15:19:33.973915 langchain_nvidia_ai_endpoints-0.1.0/langchain_nvidia_ai_endpoints/_statics.py
+-rw-r--r--   0        0        0    10149 2024-05-31 15:19:33.973915 langchain_nvidia_ai_endpoints-0.1.0/langchain_nvidia_ai_endpoints/callbacks.py
+-rw-r--r--   0        0        0    16628 2024-05-31 15:19:33.973915 langchain_nvidia_ai_endpoints-0.1.0/langchain_nvidia_ai_endpoints/chat_models.py
+-rw-r--r--   0        0        0     7534 2024-05-31 15:19:33.973915 langchain_nvidia_ai_endpoints-0.1.0/langchain_nvidia_ai_endpoints/embeddings.py
+-rw-r--r--   0        0        0        0 2024-05-31 15:19:33.973915 langchain_nvidia_ai_endpoints-0.1.0/langchain_nvidia_ai_endpoints/py.typed
+-rw-r--r--   0        0        0     5559 2024-05-31 15:19:33.973915 langchain_nvidia_ai_endpoints-0.1.0/langchain_nvidia_ai_endpoints/reranking.py
+-rw-r--r--   0        0        0    10047 2024-05-31 15:19:33.973915 langchain_nvidia_ai_endpoints-0.1.0/langchain_nvidia_ai_endpoints/tools.py
+-rw-r--r--   0        0        0     2921 2024-05-31 15:19:33.973915 langchain_nvidia_ai_endpoints-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11170 1970-01-01 00:00:00.000000 langchain_nvidia_ai_endpoints-0.1.0/PKG-INFO
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.9/LICENSE` & `langchain_nvidia_ai_endpoints-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.9/README.md` & `langchain_nvidia_ai_endpoints-0.1.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,69 @@
-# langchain-nvidia-ai-endpoints
+# NVIDIA NIMs
 
-The `langchain-nvidia-ai-endpoints` package contains LangChain integrations for chat models and embeddings powered by the [NVIDIA AI Foundation Model](https://www.nvidia.com/en-us/ai-data-science/foundation-models/) playground environment. 
+The `langchain-nvidia-ai-endpoints` package contains LangChain integrations for chat models and embeddings powered by [NVIDIA AI Foundation Models](https://www.nvidia.com/en-us/ai-data-science/foundation-models/), and hosted on [NVIDIA API Catalog.](https://build.nvidia.com/)
 
-> [NVIDIA AI Foundation Endpoints](https://www.nvidia.com/en-us/ai-data-science/foundation-models/) give users easy access to hosted endpoints for generative AI models like Llama-2, SteerLM, Mistral, etc. Using the API, you can query live endpoints available on the [NVIDIA GPU Cloud (NGC)](https://catalog.ngc.nvidia.com/ai-foundation-models) to get quick results from a DGX-hosted cloud compute environment. All models are source-accessible and can be deployed on your own compute cluster.
+NVIDIA AI Foundation models are community and NVIDIA-built models and are NVIDIA-optimized to deliver the best performance on NVIDIA accelerated infrastructure.  Using the API, you can query live endpoints available on the NVIDIA API Catalog to get quick results from a DGX-hosted cloud compute environment. All models are source-accessible and can be deployed on your own compute cluster using NVIDIA NIM which is part of NVIDIA AI Enterprise.
 
-Below is an example on how to use some common functionality surrounding text-generative and embedding models
+Models can be exported from NVIDIA’s API catalog with NVIDIA NIM, which is included with the NVIDIA AI Enterprise license, and run them on-premises, giving Enterprises ownership of their customizations and full control of their IP and AI application. NIMs are packaged as container images on a per model/model family basis and are distributed as NGC container images through the NVIDIA NGC Catalog. At their core, NIMs are containers that provide interactive APIs for running inference on an AI Model. 
+
+Below is an example on how to use some common functionality surrounding text-generative and embedding models.
 
 ## Installation
 
 ```python
 %pip install -U --quiet langchain-nvidia-ai-endpoints
 ```
 
 ## Setup
 
 **To get started:**
-1. Create a free account with the [NVIDIA GPU Cloud](https://catalog.ngc.nvidia.com/) service, which hosts AI solution catalogs, containers, models, etc.
-2. Navigate to `Catalog > AI Foundation Models > (Model with API endpoint)`.
-3. Select the `API` option and click `Generate Key`.
-4. Save the generated key as `NVIDIA_API_KEY`. From there, you should have access to the endpoints.
+1. Create a free account with [NVIDIA](https://build.nvidia.com/), which hosts NVIDIA AI Foundation models.
+2. Click on your model of choice.
+3. Under Input select the Python tab, and click `Get API Key`. Then click `Generate Key`.
+4. Copy and save the generated key as NVIDIA_API_KEY. From there, you should have access to the endpoints.
 
 ```python
 import getpass
 import os
 
 if not os.environ.get("NVIDIA_API_KEY", "").startswith("nvapi-"):
-    nvidia_api_key = getpass.getpass("Enter your NVIDIA AIPLAY API key: ")
+    nvidia_api_key = getpass.getpass("Enter your NVIDIA API key: ")
     assert nvidia_api_key.startswith("nvapi-"), f"{nvidia_api_key[:5]}... is not a valid key"
     os.environ["NVIDIA_API_KEY"] = nvidia_api_key
 ```
 
+## Working with NVIDIA API Catalog
 ```python
 ## Core LC Chat Interface
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 
-llm = ChatNVIDIA(model="ai-llama3-70b", max_tokens=419)
+llm = ChatNVIDIA(model="meta/llama3-70b-instruct", max_tokens=419)
 result = llm.invoke("Write a ballad about LangChain.")
 print(result.content)
 ```
 
+## Working with NVIDIA NIMs
+When ready to deploy, you can self-host models with NVIDIA NIM—which is included with the NVIDIA AI Enterprise software license—and run them anywhere, giving you ownership of your customizations and full control of your intellectual property (IP) and AI applications.
+
+[Learn more about NIMs](https://developer.nvidia.com/blog/nvidia-nim-offers-optimized-inference-microservices-for-deploying-ai-models-at-scale/)
+
+```python
+from langchain_nvidia_ai_endpoints import ChatNVIDIA, NVIDIAEmbeddings, NVIDIARerank
+
+# connect to an chat NIM running at localhost:8000, specifying a specific model
+llm = ChatNVIDIA(base_url="http://localhost:8000/v1", model="meta-llama3-8b-instruct")
+
+# connect to an embedding NIM running at localhost:8080
+embedder = NVIDIAEmbeddings(base_url="http://localhost:8080/v1")
+
+# connect to a reranking NIM running at localhost:2016
+ranker = NVIDIARerank(base_url="http://localhost:2016/v1")
+```
+
 ## Stream, Batch, and Async
 
 These models natively support streaming, and as is the case with all LangChain LLMs they expose a batch method to handle concurrent requests, as well as async methods for invoke, stream, and batch. Below are a few examples.
 
 ```python
 print(llm.batch(["What's 2*3?", "What's 2*6?"]))
 # Or via the async API
@@ -63,80 +84,82 @@
 ## Supported models
 
 Querying `available_models` will still give you all of the other models offered by your API credentials.
 
 ```python
 [model.id for model in llm.available_models if model.model_type]
 
-#['ai-codegemma-7b',
-# 'ai-codellama-70b',
-# 'ai-fuyu-8b',
-# 'ai-gemma-2b',
-# 'ai-gemma-7b',
-# 'ai-google-deplot',
-# 'ai-llama2-70b',
-# 'ai-llama3-70b',
-# 'ai-llama3-8b',
-# 'ai-microsoft-kosmos-2',
-# 'ai-mistral-7b-instruct-v2',
-# 'ai-mistral-large',
-# 'ai-mixtral-8x22b-instruct',
-# 'ai-mixtral-8x7b-instruct',
-# 'ai-neva-22b',
-# 'ai-recurrentgemma-2b',
-# ]
+#[
+# ...
+# 'databricks/dbrx-instruct',
+# 'google/codegemma-7b',
+# 'google/gemma-2b',
+# 'google/gemma-7b',
+# 'google/recurrentgemma-2b',
+# 'meta/codellama-70b',
+# 'meta/llama2-70b',
+# 'meta/llama3-70b-instruct',
+# 'meta/llama3-8b-instruct',
+# 'microsoft/phi-3-mini-128k-instruct',
+# 'mistralai/mistral-7b-instruct-v0.2',
+# 'mistralai/mistral-large',
+# 'mistralai/mixtral-8x22b-instruct-v0.1',
+# 'mistralai/mixtral-8x7b-instruct-v0.1',
+# 'snowflake/arctic',
+# ...
+#]
 ```
 
 ## Model types
 
 All of these models above are supported and can be accessed via `ChatNVIDIA`.
 
 Some model types support unique prompting techniques and chat messages. We will review a few important ones below.
 
 **To find out more about a specific model, please navigate to the NVIDIA NIM section of ai.nvidia.com [as linked here](https://docs.api.nvidia.com/nim/).**
 
 ### General Chat
 
-Models such as `ai-llama3-70b` and `ai-mixtral-8x22b-instruct` are good all-around models that you can use for with any LangChain chat messages. Example below.
+Models such as `meta/llama3-8b-instruct` and `mistralai/mixtral-8x22b-instruct-v0.1` are good all-around models that you can use for with any LangChain chat messages. Example below.
 
 ```python
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.output_parsers import StrOutputParser
 
 prompt = ChatPromptTemplate.from_messages(
     [
         ("system", "You are a helpful AI assistant named Fred."),
         ("user", "{input}")
     ]
 )
 chain = (
     prompt
-    | ChatNVIDIA(model="ai-llama3-70b")
+    | ChatNVIDIA(model="meta/llama3-8b-instruct")
     | StrOutputParser()
 )
 
 for txt in chain.stream({"input": "What's your name?"}):
     print(txt, end="")
 ```
 
 ### Code Generation
 
-These models accept the same arguments and input structure as regular chat models, but they tend to perform better on code-genreation and structured code tasks. An example of this is `ai-codellama-70b` and `ai-codegemma-7b`.
+These models accept the same arguments and input structure as regular chat models, but they tend to perform better on code-genreation and structured code tasks. An example of this is `meta/codellama-70b` and `google/codegemma-7b`.
 
 ```python
 prompt = ChatPromptTemplate.from_messages(
     [
         ("system", "You are an expert coding AI. Respond only in valid python; no narration whatsoever."),
         ("user", "{input}")
     ]
 )
 chain = (
     prompt
-    | ChatNVIDIA(model="ai-codellama-70b", max_tokens=419)
+    | ChatNVIDIA(model="meta/codellama-70b", max_tokens=419)
     | StrOutputParser()
 )
 
 for txt in chain.stream({"input": "How do I solve this fizz buzz problem?"}):
     print(txt, end="")
 ```
 
@@ -194,15 +217,15 @@
     print(txt, end="")
 ```
 
 ## Multimodal
 
 NVIDIA also supports multimodal inputs, meaning you can provide both images and text for the model to reason over.
 
-An example model supporting multimodal inputs is `ai-neva-22b`.
+An example model supporting multimodal inputs is `nvidia/neva-22b`.
 
 These models accept LangChain's standard image formats. Below are examples.
 
 ```python
 import requests
 
 image_url = "https://picsum.photos/seed/kitten/300/200"
@@ -210,15 +233,15 @@
 ```
 
 Initialize the model like so:
 
 ```python
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 
-llm = ChatNVIDIA(model="ai-neva-22b")
+llm = ChatNVIDIA(model="nvidia/neva-22b")
 ```
 
 #### Passing an image as a URL
 
 ```python
 from langchain_core.messages import HumanMessage
 
@@ -252,49 +275,21 @@
 ```python
 base64_with_mime_type = f"data:image/png;base64,{b64_string}"
 llm.invoke(
     f'What\'s in this image?\n<img src="{base64_with_mime_type}" />'
 )
 ```
 
-## RAG: Context models
-
-NVIDIA also has Q&A models that support a special "context" chat message containing retrieved context (such as documents within a RAG chain). This is useful to avoid prompt-injecting the model.
-
-**Note:** Only "user" (human) and "context" chat messages are supported for these models, not system or AI messages useful in conversational flows.
-
-The `_qa_` models like `nemotron_qa_8b` support this.
-
-```python
-from langchain_nvidia_ai_endpoints import ChatNVIDIA
-from langchain_core.prompts import ChatPromptTemplate
-from langchain_core.output_parsers import StrOutputParser
-from langchain_core.messages import ChatMessage
-prompt = ChatPromptTemplate.from_messages(
-    [
-        ChatMessage(role="context", content="Parrots and Cats have signed the peace accord."),
-        ("user", "{input}")
-    ]
-)
-llm = ChatNVIDIA(model="nemotron_qa_8b")
-chain = (
-    prompt
-    | llm
-    | StrOutputParser()
-)
-chain.invoke({"input": "What was signed?"})
-```
-
 ## Embeddings
 
 You can also connect to embeddings models through this package. Below is an example:
 
 ```python
 from langchain_nvidia_ai_endpoints import NVIDIAEmbeddings
 
-embedder = NVIDIAEmbeddings(model="ai-embed-qa-4")
+embedder = NVIDIAEmbeddings(model="NV-Embed-QA")
 embedder.embed_query("What's the temperature today?")
 embedder.embed_documents([
     "The temperature is 42 degrees.",
     "Class is dismissed at 9 PM."
 ])
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/__init__.py` & `langchain_nvidia_ai_endpoints-0.1.0/langchain_nvidia_ai_endpoints/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 ## Utilizing Chat Models:
 
 After setting up the environment, interact with NVIDIA AI Foundation models:
 ```python
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 
-ai_chat_model = ChatNVIDIA(model="llama2_13b")
+ai_chat_model = ChatNVIDIA(model="meta/llama2-70b")
 response = ai_chat_model.invoke("Tell me about the LangChain integration.")
 ```
 
 # Generating Semantic Embeddings:
 
 Use NVIDIA's models for creating embeddings, useful in various NLP tasks:
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/callbacks.py` & `langchain_nvidia_ai_endpoints-0.1.0/langchain_nvidia_ai_endpoints/callbacks.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/chat_models.py` & `langchain_nvidia_ai_endpoints-0.1.0/langchain_nvidia_ai_endpoints/chat_models.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import base64
 import io
 import logging
 import os
 import sys
 import urllib.parse
-import warnings
 from typing import (
     Any,
     AsyncIterator,
     Callable,
     Dict,
     Iterator,
     List,
@@ -36,21 +35,20 @@
     ChatMessageChunk,
 )
 from langchain_core.outputs import (
     ChatGeneration,
     ChatGenerationChunk,
     ChatResult,
 )
-from langchain_core.pydantic_v1 import BaseModel, Field, validator
+from langchain_core.pydantic_v1 import BaseModel, Field, PrivateAttr
 from langchain_core.runnables import Runnable
-from langchain_core.runnables.config import run_in_executor
 from langchain_core.tools import BaseTool
 
-from langchain_nvidia_ai_endpoints import _common as nvidia_ai_endpoints
-from langchain_nvidia_ai_endpoints._statics import MODEL_SPECS
+from langchain_nvidia_ai_endpoints._common import _NVIDIAClient
+from langchain_nvidia_ai_endpoints._statics import Model, determine_model
 
 _CallbackManager = Union[AsyncCallbackManagerForLLMRun, CallbackManagerForLLMRun]
 _DictOrPydanticClass = Union[Dict[str, Any], Type[BaseModel]]
 _DictOrPydantic = Union[Dict, BaseModel]
 
 try:
     import PIL.Image
@@ -113,149 +111,154 @@
             raise ValueError(
                 "The provided string is not a valid URL, base64, or file path."
             )
     except Exception as e:
         raise ValueError(f"Unable to process the provided image source: {e}")
 
 
-class ChatNVIDIA(nvidia_ai_endpoints._NVIDIAClient, BaseChatModel):
+class ChatNVIDIA(BaseChatModel):
     """NVIDIA chat model.
 
     Example:
         .. code-block:: python
 
             from langchain_nvidia_ai_endpoints import ChatNVIDIA
 
 
-            model = ChatNVIDIA(model="llama2_13b")
+            model = ChatNVIDIA(model="meta/llama2-70b")
             response = model.invoke("Hello")
     """
 
-    _default_model: str = "ai-mixtral-8x7b-instruct"
-    infer_endpoint: str = Field("{base_url}/chat/completions")
+    _client: _NVIDIAClient = PrivateAttr(_NVIDIAClient)
+    _default_model: str = "mistralai/mixtral-8x7b-instruct-v0.1"
+    base_url: str = Field(
+        "https://integrate.api.nvidia.com/v1",
+        description="Base url for model listing an invocation",
+    )
     model: str = Field(_default_model, description="Name of the model to invoke")
     temperature: Optional[float] = Field(description="Sampling temperature in [0, 1]")
-    max_tokens: Optional[int] = Field(description="Maximum # of tokens to generate")
+    max_tokens: Optional[int] = Field(
+        1024, description="Maximum # of tokens to generate"
+    )
     top_p: Optional[float] = Field(description="Top-p for distribution sampling")
     seed: Optional[int] = Field(description="The seed for deterministic results")
-    bad: Optional[Sequence[str]] = Field(description="Bad words to avoid (cased)")
     stop: Optional[Sequence[str]] = Field(description="Stop words (cased)")
-    labels: Optional[Dict[str, float]] = Field(description="Steering parameters")
-    streaming: bool = Field(True)
 
-    @validator("model")
-    def aifm_deprecated(cls, value: str) -> str:
-        """All AI Foundataion Models are deprecate, use API Catalog models instead."""
-        for model in [value, f"playground_{value}"]:
-            if model in MODEL_SPECS and MODEL_SPECS[model].get("api_type") == "aifm":
-                alternative = MODEL_SPECS[model].get(
-                    "alternative", ChatNVIDIA._default_model
-                )
-                warnings.warn(
-                    f"{value} is deprecated. Try {alternative} instead.",
-                    DeprecationWarning,
-                )
-        return value
+    def __init__(self, **kwargs: Any):
+        """
+        Create a new NVIDIAChat chat model.
+
+        This class provides access to a NVIDIA NIM for chat. By default, it
+        connects to a hosted NIM, but can be configured to connect to a local NIM
+        using the `base_url` parameter. An API key is required to connect to the
+        hosted NIM.
+
+        Args:
+            model (str): The model to use for chat.
+            nvidia_api_key (str): The API key to use for connecting to the hosted NIM.
+            api_key (str): Alternative to nvidia_api_key.
+            base_url (str): The base URL of the NIM to connect to.
+            temperature (float): Sampling temperature in [0, 1].
+            max_tokens (int): Maximum number of tokens to generate.
+            top_p (float): Top-p for distribution sampling.
+            seed (int): A seed for deterministic results.
+            stop (list[str]): A list of cased stop words.
+
+        API Key:
+        - The recommended way to provide the API key is through the `NVIDIA_API_KEY`
+            environment variable.
+        """
+        super().__init__(**kwargs)
+        infer_path = "{base_url}/chat/completions"
+        # not all chat models are on https://integrate.api.nvidia.com/v1,
+        # those that are not are served from their own endpoints
+        if model := determine_model(self.model):
+            if model.endpoint:  # some models have custom endpoints
+                infer_path = model.endpoint
+        self._client = _NVIDIAClient(
+            base_url=self.base_url,
+            model=self.model,
+            api_key=kwargs.get("nvidia_api_key", kwargs.get("api_key", None)),
+            infer_path=infer_path,
+        )
+        # todo: only store the model in one place
+        # the model may be updated to a newer name during initialization
+        self.model = self._client.model
+
+    @property
+    def available_models(self) -> List[Model]:
+        """
+        Get a list of available models that work with ChatNVIDIA.
+        """
+        return self._client.get_available_models(self.__class__.__name__)
+
+    @classmethod
+    def get_available_models(
+        cls,
+        **kwargs: Any,
+    ) -> List[Model]:
+        """
+        Get a list of available models that work with ChatNVIDIA.
+        """
+        return cls(**kwargs).available_models
 
     @property
     def _llm_type(self) -> str:
         """Return type of NVIDIA AI Foundation Model Interface."""
         return "chat-nvidia-ai-playground"
 
     def _generate(
         self,
         messages: List[BaseMessage],
         stop: Optional[List[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> ChatResult:
-        responses = self._call(messages, stop=stop, run_manager=run_manager, **kwargs)
+        inputs = self._custom_preprocess(messages)
+        responses = self._get_generation(inputs=inputs, stop=stop, **kwargs)
         self._set_callback_out(responses, run_manager)
-        message = ChatMessage(**self.custom_postprocess(responses))
+        message = ChatMessage(**self._custom_postprocess(responses))
         generation = ChatGeneration(message=message)
         return ChatResult(generations=[generation], llm_output=responses)
 
-    async def _agenerate(
-        self,
-        messages: List[BaseMessage],
-        stop: Optional[List[str]] = None,
-        run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
-        **kwargs: Any,
-    ) -> ChatResult:
-        return await run_in_executor(
-            None,
-            self._generate,
-            messages,
-            stop=stop,
-            run_manager=run_manager.get_sync() if run_manager else None,
-            **kwargs,
-        )
-
-    def _call(
-        self,
-        messages: List[BaseMessage],
-        stop: Optional[Sequence[str]] = None,
-        run_manager: Optional[CallbackManagerForLLMRun] = None,
-        **kwargs: Any,
-    ) -> dict:
-        """Invoke on a single list of chat messages."""
-        inputs = self.custom_preprocess(messages)
-        responses = self.get_generation(inputs=inputs, stop=stop, **kwargs)
-        return responses
-
     def _get_filled_chunk(self, **kwargs: Any) -> ChatGenerationChunk:
         """Fill the generation chunk."""
         return ChatGenerationChunk(message=ChatMessageChunk(**kwargs))
 
     def _stream(
         self,
         messages: List[BaseMessage],
         stop: Optional[Sequence[str]] = None,
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> Iterator[ChatGenerationChunk]:
         """Allows streaming to model!"""
-        inputs = self.custom_preprocess(messages)
-        for response in self.get_stream(inputs=inputs, stop=stop, **kwargs):
+        inputs = self._custom_preprocess(messages)
+        for response in self._get_stream(inputs=inputs, stop=stop, **kwargs):
             self._set_callback_out(response, run_manager)
-            chunk = self._get_filled_chunk(**self.custom_postprocess(response))
+            chunk = self._get_filled_chunk(**self._custom_postprocess(response))
             if run_manager:
                 run_manager.on_llm_new_token(chunk.text, chunk=chunk)
             yield chunk
 
-    async def _astream(
-        self,
-        messages: List[BaseMessage],
-        stop: Optional[Sequence[str]] = None,
-        run_manager: Optional[AsyncCallbackManagerForLLMRun] = None,
-        **kwargs: Any,
-    ) -> AsyncIterator[ChatGenerationChunk]:
-        inputs = self.custom_preprocess(messages)
-        async for response in self.get_astream(inputs=inputs, stop=stop, **kwargs):
-            self._set_callback_out(response, run_manager)
-            chunk = self._get_filled_chunk(**self.custom_postprocess(response))
-            if run_manager:
-                await run_manager.on_llm_new_token(chunk.text, chunk=chunk)
-            yield chunk
-
     def _set_callback_out(
         self,
         result: dict,
         run_manager: Optional[_CallbackManager],
     ) -> None:
         result.update({"model_name": self.model})
         if run_manager:
             for cb in run_manager.handlers:
                 if hasattr(cb, "llm_output"):
                     cb.llm_output = result
 
-    def custom_preprocess(
+    def _custom_preprocess(  # todo: remove
         self, msg_list: Sequence[BaseMessage]
     ) -> List[Dict[str, str]]:
-        return [self.preprocess_msg(m) for m in msg_list]
+        return [self._preprocess_msg(m) for m in msg_list]
 
     def _process_content(self, content: Union[str, List[Union[dict, str]]]) -> str:
         if isinstance(content, str):
             return content
         string_array: list = []
 
         for part in content:
@@ -280,27 +283,27 @@
                         raise ValueError(
                             f"Unrecognized message part type: {part['type']}"
                         )
                 else:
                     raise ValueError(f"Unrecognized message part format: {part}")
         return "".join(string_array)
 
-    def preprocess_msg(self, msg: BaseMessage) -> Dict[str, str]:
+    def _preprocess_msg(self, msg: BaseMessage) -> Dict[str, str]:  # todo: remove
         if isinstance(msg, BaseMessage):
             role_convert = {"ai": "assistant", "human": "user"}
             if isinstance(msg, ChatMessage):
                 role = msg.role
             else:
                 role = msg.type
             role = role_convert.get(role, role)
             content = self._process_content(msg.content)
             return {"role": role, "content": content}
         raise ValueError(f"Invalid message: {repr(msg)} of type {type(msg)}")
 
-    def custom_postprocess(self, msg: dict) -> dict:
+    def _custom_postprocess(self, msg: dict) -> dict:  # todo: remove
         kw_left = msg.copy()
         out_dict = {
             "role": kw_left.pop("role", "assistant") or "assistant",
             "name": kw_left.pop("name", None),
             "id": kw_left.pop("id", None),
             "content": kw_left.pop("content", "") or "",
             "additional_kwargs": {},
@@ -311,74 +314,77 @@
                 out_dict["additional_kwargs"][k] = kw_left.pop(k)
         out_dict["response_metadata"] = kw_left
         return out_dict
 
     ######################################################################################
     ## Core client-side interfaces
 
-    def get_generation(
+    def _get_generation(
         self,
         inputs: Sequence[Dict],
         **kwargs: Any,
     ) -> dict:
         """Call to client generate method with call scope"""
-        stop = kwargs["stop"] = kwargs.get("stop") or self.stop
-        payload = self.get_payload(inputs=inputs, stream=False, **kwargs)
-        out = self.client.get_req_generation(self.model, stop=stop, payload=payload)
+        kwargs["stop"] = kwargs.get("stop", self.stop)
+        payload = self._get_payload(inputs=inputs, stream=False, **kwargs)
+        out = self._client.client.get_req_generation(payload=payload)
         return out
 
-    def get_stream(
+    def _get_stream(  # todo: remove
         self,
         inputs: Sequence[Dict],
         **kwargs: Any,
     ) -> Iterator:
         """Call to client stream method with call scope"""
-        stop = kwargs["stop"] = kwargs.get("stop") or self.stop
-        payload = self.get_payload(inputs=inputs, stream=True, **kwargs)
-        return self.client.get_req_stream(self.model, stop=stop, payload=payload)
+        kwargs["stop"] = kwargs.get("stop") or self.stop
+        payload = self._get_payload(inputs=inputs, stream=True, **kwargs)
+        return self._client.client.get_req_stream(payload=payload)
 
-    def get_astream(
+    def _get_astream(  # todo: remove
         self,
         inputs: Sequence[Dict],
         **kwargs: Any,
     ) -> AsyncIterator:
         """Call to client astream methods with call scope"""
-        stop = kwargs["stop"] = kwargs.get("stop") or self.stop
-        payload = self.get_payload(inputs=inputs, stream=True, **kwargs)
-        return self.client.get_req_astream(self.model, stop=stop, payload=payload)
-
-    def get_payload(self, inputs: Sequence[Dict], **kwargs: Any) -> dict:
+        kwargs["stop"] = kwargs.get("stop") or self.stop
+        payload = self._get_payload(inputs=inputs, stream=True, **kwargs)
+        return self._client.client.get_req_astream(payload=payload)
+
+    def _get_payload(
+        self, inputs: Sequence[Dict], **kwargs: Any
+    ) -> dict:  # todo: remove
         """Generates payload for the _NVIDIAClient API to send to service."""
         attr_kwargs = {
+            "model": self.model,
             "temperature": self.temperature,
             "max_tokens": self.max_tokens,
             "top_p": self.top_p,
             "seed": self.seed,
-            "bad": self.bad,
             "stop": self.stop,
-            "labels": self.labels,
         }
-        if model_name := self.get_binding_model():
-            attr_kwargs["model"] = model_name
+        # if model_name := self._get_binding_model():
+        #     attr_kwargs["model"] = model_name
         attr_kwargs = {k: v for k, v in attr_kwargs.items() if v is not None}
         new_kwargs = {**attr_kwargs, **kwargs}
-        return self.prep_payload(inputs=inputs, **new_kwargs)
+        return self._prep_payload(inputs=inputs, **new_kwargs)
 
-    def prep_payload(self, inputs: Sequence[Dict], **kwargs: Any) -> dict:
+    def _prep_payload(
+        self, inputs: Sequence[Dict], **kwargs: Any
+    ) -> dict:  # todo: remove
         """Prepares a message or list of messages for the payload"""
-        messages = [self.prep_msg(m) for m in inputs]
+        messages = [self._prep_msg(m) for m in inputs]
         if kwargs.get("labels"):
             # (WFH) Labels are currently (?) always passed as an assistant
             # suffix message, but this API seems less stable.
             messages += [{"labels": kwargs.pop("labels"), "role": "assistant"}]
         if kwargs.get("stop") is None:
             kwargs.pop("stop")
         return {"messages": messages, **kwargs}
 
-    def prep_msg(self, msg: Union[str, dict, BaseMessage]) -> dict:
+    def _prep_msg(self, msg: Union[str, dict, BaseMessage]) -> dict:  # todo: remove
         """Helper Method: Ensures a message is a dictionary with a role and content."""
         if isinstance(msg, str):
             # (WFH) this shouldn't ever be reached but leaving this here bcs
             # it's a Chesterton's fence I'm unwilling to touch
             return dict(role="user", content=msg)
         if isinstance(msg, dict):
             if msg.get("content", None) is None:
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/reranking.py` & `langchain_nvidia_ai_endpoints-0.1.0/langchain_nvidia_ai_endpoints/reranking.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from typing import Any, Generator, List, Optional, Sequence
 
 from langchain_core.callbacks.manager import Callbacks
 from langchain_core.documents import Document
 from langchain_core.documents.compressor import BaseDocumentCompressor
 from langchain_core.pydantic_v1 import BaseModel, Field, PrivateAttr
 
-from ._common import _MODE_TYPE, _NVIDIAClient
-from ._statics import Model
+from langchain_nvidia_ai_endpoints._common import _NVIDIAClient
+from langchain_nvidia_ai_endpoints._statics import Model, determine_model
 
 
 class Ranking(BaseModel):
     index: int
     logit: float
 
 
@@ -23,124 +23,90 @@
 
     class Config:
         validate_assignment = True
 
     _client: _NVIDIAClient = PrivateAttr(_NVIDIAClient)
 
     _default_batch_size: int = 32
+    _deprecated_model: str = "ai-rerank-qa-mistral-4b"
+    _default_model_name: str = "nv-rerank-qa-mistral-4b:1"
 
+    base_url: str = Field(
+        "https://integrate.api.nvidia.com/v1",
+        description="Base url for model listing an invocation",
+    )
     top_n: int = Field(5, ge=0, description="The number of documents to return.")
     model: str = Field(
-        "ai-rerank-qa-mistral-4b", description="The model to use for reranking."
+        _default_model_name, description="The model to use for reranking."
     )
     max_batch_size: int = Field(
         _default_batch_size, ge=1, description="The maximum batch size."
     )
 
     def __init__(self, **kwargs: Any):
         """
         Create a new NVIDIARerank document compressor.
 
-        Unless you plan to use the "nim" mode, you need to provide an API key. Your
-        options are -
-         0. Pass the key as the nvidia_api_key parameter.
-         1. Pass the key as the api_key parameter.
-         2. Set the NVIDIA_API_KEY environment variable, recommended.
-        Precedence is in the order listed above.
+        This class provides access to a NVIDIA NIM for reranking. By default, it
+        connects to a hosted NIM, but can be configured to connect to a local NIM
+        using the `base_url` parameter. An API key is required to connect to the
+        hosted NIM.
+
+        Args:
+            model (str): The model to use for reranking.
+            nvidia_api_key (str): The API key to use for connecting to the hosted NIM.
+            api_key (str): Alternative to nvidia_api_key.
+            base_url (str): The base URL of the NIM to connect to.
+
+        API Key:
+        - The recommended way to provide the API key is through the `NVIDIA_API_KEY`
+            environment variable.
         """
         super().__init__(**kwargs)
+        infer_path = "{base_url}/ranking"
+        # not all models are on https://integrate.api.nvidia.com/v1,
+        # those that are not are served from their own endpoints
+        if model := determine_model(self.model):
+            if model.endpoint:  # some models have custom endpoints
+                infer_path = model.endpoint
         self._client = _NVIDIAClient(
+            base_url=self.base_url,
             model=self.model,
             api_key=kwargs.get("nvidia_api_key", kwargs.get("api_key", None)),
+            infer_path=infer_path,
         )
+        # todo: only store the model in one place
+        # the model may be updated to a newer name during initialization
+        self.model = self._client.model
 
     @property
     def available_models(self) -> List[Model]:
         """
-        Get a list of available models that work with ChatNVIDIA.
+        Get a list of available models that work with NVIDIARerank.
         """
-        return self._client.get_available_models(
-            client=self._client,
-            filter=self.__class__.__name__,
-        )
+        return self._client.get_available_models(self.__class__.__name__)
 
     @classmethod
     def get_available_models(
         cls,
-        mode: Optional[_MODE_TYPE] = None,
-        list_all: bool = False,
         **kwargs: Any,
     ) -> List[Model]:
         """
-        Get a list of available models. These models will work with the ChatNVIDIA
-        interface.
-
-        Use the mode parameter to specify the mode to use. See the docs for mode()
-        to understand additional keyword arguments required when setting mode.
-
-        It is possible to get a list of all models, including those that are not
-        chat models, by setting the list_all parameter to True.
-        """
-        self = cls(**kwargs).mode(mode=mode, **kwargs)
-        return self._client.get_available_models(
-            mode=mode,
-            list_all=list_all,
-            client=self._client,
-            filter=cls.__name__,
-            **kwargs,
-        )
-
-    def mode(
-        self,
-        mode: Optional[_MODE_TYPE] = "nvidia",
-        base_url: Optional[str] = None,
-        model: Optional[str] = None,
-        api_key: Optional[str] = None,
-        **kwargs: Any,
-    ) -> NVIDIARerank:
+        Get a list of available models that work with NVIDIARerank.
         """
-        Change the mode.
-
-        There are two modes, "nvidia" and "nim". The "nvidia" mode is the default mode
-        and is used to interact with hosted NVIDIA AI endpoints. The "nim" mode is
-        used to interact with NVIDIA NIM endpoints, which are typically hosted
-        on-premises.
-
-        For the "nvidia" mode, the "api_key" parameter is available to specify your
-        API key. If not specified, the NVIDIA_API_KEY environment variable will be used.
-
-        For the "nim" mode, the "base_url" and "model" parameters are required. Set
-        base_url to the url of your NVIDIA NIM endpoint. For instance,
-        "https://localhost:9999/v1". Additionally, the "model" parameter must be set
-        to the name of the model inside the NIM.
-        """
-        # set a default base_url for nim mode
-        if not base_url and mode == "nim":
-            base_url = "http://localhost:1976/v1"
-        self._client = self._client.mode(
-            mode=mode,
-            base_url=base_url,
-            model=model,
-            api_key=api_key,
-            infer_path="{base_url}/ranking",
-            **kwargs,
-        )
-        self.model = self._client.model
-        return self
+        return cls(**kwargs).available_models
 
     # todo: batching when len(documents) > endpoint's max batch size
     def _rank(self, documents: List[str], query: str) -> List[Ranking]:
         response = self._client.client.get_req(
-            model_name=self.model,
             payload={
                 "model": "nv-rerank-qa-mistral-4b:1",
                 "query": {"text": query},
                 "passages": [{"text": passage} for passage in documents],
             },
-            endpoint="infer",
         )
         if response.status_code != 200:
             response.raise_for_status()
         # todo: handle errors
         rankings = response.json()["rankings"]
         # todo: callback support
         return [Ranking(**ranking) for ranking in rankings[: self.top_n]]
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.9/langchain_nvidia_ai_endpoints/tools.py` & `langchain_nvidia_ai_endpoints-0.1.0/langchain_nvidia_ai_endpoints/tools.py`

 * *Files identical despite different names*

### Comparing `langchain_nvidia_ai_endpoints-0.0.9/pyproject.toml` & `langchain_nvidia_ai_endpoints-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "langchain-nvidia-ai-endpoints"
-version = "0.0.9"
+version = "0.1.0"
 description = "An integration package connecting NVIDIA AI Endpoints and LangChain"
 authors = []
 readme = "README.md"
-repository = "https://github.com/langchain-ai/langchain"
+repository = "https://github.com/langchain-ai/langchain-nvidia"
 license = "MIT"
 
 [tool.poetry.urls]
-"Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/nvidia-ai-endpoints"
+"Source Code" = "https://github.com/langchain-ai/langchain-nvidia/tree/main/libs/ai-endpoints"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.27"
+langchain-core = ">=0.1.27,<0.3"
 aiohttp = "^3.9.1"
 pillow = ">=10.0.0,<11.0.0"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 freezegun = "^1.2.2"
 pytest-mock = "^3.10.0"
 syrupy = "^4.0.2"
 pytest-watcher = "^0.3.4"
 pytest-asyncio = "^0.21.1"
-langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
+langchain-core = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core" }
 requests-mock = "^1.11.0"
 faker = "^24.4.0"
 
 [tool.poetry.group.codespell]
 optional = true
 
 [tool.poetry.group.codespell.dependencies]
@@ -48,21 +48,21 @@
 [tool.poetry.group.lint.dependencies]
 ruff = "^0.1.5"
 
 [tool.poetry.group.typing.dependencies]
 mypy = "^0.991"
 types-requests = "^2.31.0.10"
 types-pillow = "^10.2.0.20240125"
-langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
+langchain-core = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core" }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-langchain-core = {git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core"}
+langchain-core = { git = "https://github.com/langchain-ai/langchain.git", subdirectory = "libs/core" }
 
 [tool.ruff.lint]
 select = [
   "E",    # pycodestyle
   "F",    # pyflakes
   "I",    # isort
   "T201", # print
```

### Comparing `langchain_nvidia_ai_endpoints-0.0.9/PKG-INFO` & `langchain_nvidia_ai_endpoints-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,68 +1,89 @@
 Metadata-Version: 2.1
 Name: langchain-nvidia-ai-endpoints
-Version: 0.0.9
+Version: 0.1.0
 Summary: An integration package connecting NVIDIA AI Endpoints and LangChain
-Home-page: https://github.com/langchain-ai/langchain
+Home-page: https://github.com/langchain-ai/langchain-nvidia
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
-Requires-Dist: langchain-core (>=0.1.27,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.27,<0.3)
 Requires-Dist: pillow (>=10.0.0,<11.0.0)
-Project-URL: Repository, https://github.com/langchain-ai/langchain
-Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/nvidia-ai-endpoints
+Project-URL: Repository, https://github.com/langchain-ai/langchain-nvidia
+Project-URL: Source Code, https://github.com/langchain-ai/langchain-nvidia/tree/main/libs/ai-endpoints
 Description-Content-Type: text/markdown
 
-# langchain-nvidia-ai-endpoints
+# NVIDIA NIMs
 
-The `langchain-nvidia-ai-endpoints` package contains LangChain integrations for chat models and embeddings powered by the [NVIDIA AI Foundation Model](https://www.nvidia.com/en-us/ai-data-science/foundation-models/) playground environment. 
+The `langchain-nvidia-ai-endpoints` package contains LangChain integrations for chat models and embeddings powered by [NVIDIA AI Foundation Models](https://www.nvidia.com/en-us/ai-data-science/foundation-models/), and hosted on [NVIDIA API Catalog.](https://build.nvidia.com/)
 
-> [NVIDIA AI Foundation Endpoints](https://www.nvidia.com/en-us/ai-data-science/foundation-models/) give users easy access to hosted endpoints for generative AI models like Llama-2, SteerLM, Mistral, etc. Using the API, you can query live endpoints available on the [NVIDIA GPU Cloud (NGC)](https://catalog.ngc.nvidia.com/ai-foundation-models) to get quick results from a DGX-hosted cloud compute environment. All models are source-accessible and can be deployed on your own compute cluster.
+NVIDIA AI Foundation models are community and NVIDIA-built models and are NVIDIA-optimized to deliver the best performance on NVIDIA accelerated infrastructure.  Using the API, you can query live endpoints available on the NVIDIA API Catalog to get quick results from a DGX-hosted cloud compute environment. All models are source-accessible and can be deployed on your own compute cluster using NVIDIA NIM which is part of NVIDIA AI Enterprise.
 
-Below is an example on how to use some common functionality surrounding text-generative and embedding models
+Models can be exported from NVIDIA’s API catalog with NVIDIA NIM, which is included with the NVIDIA AI Enterprise license, and run them on-premises, giving Enterprises ownership of their customizations and full control of their IP and AI application. NIMs are packaged as container images on a per model/model family basis and are distributed as NGC container images through the NVIDIA NGC Catalog. At their core, NIMs are containers that provide interactive APIs for running inference on an AI Model. 
+
+Below is an example on how to use some common functionality surrounding text-generative and embedding models.
 
 ## Installation
 
 ```python
 %pip install -U --quiet langchain-nvidia-ai-endpoints
 ```
 
 ## Setup
 
 **To get started:**
-1. Create a free account with the [NVIDIA GPU Cloud](https://catalog.ngc.nvidia.com/) service, which hosts AI solution catalogs, containers, models, etc.
-2. Navigate to `Catalog > AI Foundation Models > (Model with API endpoint)`.
-3. Select the `API` option and click `Generate Key`.
-4. Save the generated key as `NVIDIA_API_KEY`. From there, you should have access to the endpoints.
+1. Create a free account with [NVIDIA](https://build.nvidia.com/), which hosts NVIDIA AI Foundation models.
+2. Click on your model of choice.
+3. Under Input select the Python tab, and click `Get API Key`. Then click `Generate Key`.
+4. Copy and save the generated key as NVIDIA_API_KEY. From there, you should have access to the endpoints.
 
 ```python
 import getpass
 import os
 
 if not os.environ.get("NVIDIA_API_KEY", "").startswith("nvapi-"):
-    nvidia_api_key = getpass.getpass("Enter your NVIDIA AIPLAY API key: ")
+    nvidia_api_key = getpass.getpass("Enter your NVIDIA API key: ")
     assert nvidia_api_key.startswith("nvapi-"), f"{nvidia_api_key[:5]}... is not a valid key"
     os.environ["NVIDIA_API_KEY"] = nvidia_api_key
 ```
 
+## Working with NVIDIA API Catalog
 ```python
 ## Core LC Chat Interface
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 
-llm = ChatNVIDIA(model="ai-llama3-70b", max_tokens=419)
+llm = ChatNVIDIA(model="meta/llama3-70b-instruct", max_tokens=419)
 result = llm.invoke("Write a ballad about LangChain.")
 print(result.content)
 ```
 
+## Working with NVIDIA NIMs
+When ready to deploy, you can self-host models with NVIDIA NIM—which is included with the NVIDIA AI Enterprise software license—and run them anywhere, giving you ownership of your customizations and full control of your intellectual property (IP) and AI applications.
+
+[Learn more about NIMs](https://developer.nvidia.com/blog/nvidia-nim-offers-optimized-inference-microservices-for-deploying-ai-models-at-scale/)
+
+```python
+from langchain_nvidia_ai_endpoints import ChatNVIDIA, NVIDIAEmbeddings, NVIDIARerank
+
+# connect to an chat NIM running at localhost:8000, specifying a specific model
+llm = ChatNVIDIA(base_url="http://localhost:8000/v1", model="meta-llama3-8b-instruct")
+
+# connect to an embedding NIM running at localhost:8080
+embedder = NVIDIAEmbeddings(base_url="http://localhost:8080/v1")
+
+# connect to a reranking NIM running at localhost:2016
+ranker = NVIDIARerank(base_url="http://localhost:2016/v1")
+```
+
 ## Stream, Batch, and Async
 
 These models natively support streaming, and as is the case with all LangChain LLMs they expose a batch method to handle concurrent requests, as well as async methods for invoke, stream, and batch. Below are a few examples.
 
 ```python
 print(llm.batch(["What's 2*3?", "What's 2*6?"]))
 # Or via the async API
@@ -83,80 +104,82 @@
 ## Supported models
 
 Querying `available_models` will still give you all of the other models offered by your API credentials.
 
 ```python
 [model.id for model in llm.available_models if model.model_type]
 
-#['ai-codegemma-7b',
-# 'ai-codellama-70b',
-# 'ai-fuyu-8b',
-# 'ai-gemma-2b',
-# 'ai-gemma-7b',
-# 'ai-google-deplot',
-# 'ai-llama2-70b',
-# 'ai-llama3-70b',
-# 'ai-llama3-8b',
-# 'ai-microsoft-kosmos-2',
-# 'ai-mistral-7b-instruct-v2',
-# 'ai-mistral-large',
-# 'ai-mixtral-8x22b-instruct',
-# 'ai-mixtral-8x7b-instruct',
-# 'ai-neva-22b',
-# 'ai-recurrentgemma-2b',
-# ]
+#[
+# ...
+# 'databricks/dbrx-instruct',
+# 'google/codegemma-7b',
+# 'google/gemma-2b',
+# 'google/gemma-7b',
+# 'google/recurrentgemma-2b',
+# 'meta/codellama-70b',
+# 'meta/llama2-70b',
+# 'meta/llama3-70b-instruct',
+# 'meta/llama3-8b-instruct',
+# 'microsoft/phi-3-mini-128k-instruct',
+# 'mistralai/mistral-7b-instruct-v0.2',
+# 'mistralai/mistral-large',
+# 'mistralai/mixtral-8x22b-instruct-v0.1',
+# 'mistralai/mixtral-8x7b-instruct-v0.1',
+# 'snowflake/arctic',
+# ...
+#]
 ```
 
 ## Model types
 
 All of these models above are supported and can be accessed via `ChatNVIDIA`.
 
 Some model types support unique prompting techniques and chat messages. We will review a few important ones below.
 
 **To find out more about a specific model, please navigate to the NVIDIA NIM section of ai.nvidia.com [as linked here](https://docs.api.nvidia.com/nim/).**
 
 ### General Chat
 
-Models such as `ai-llama3-70b` and `ai-mixtral-8x22b-instruct` are good all-around models that you can use for with any LangChain chat messages. Example below.
+Models such as `meta/llama3-8b-instruct` and `mistralai/mixtral-8x22b-instruct-v0.1` are good all-around models that you can use for with any LangChain chat messages. Example below.
 
 ```python
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_core.output_parsers import StrOutputParser
 
 prompt = ChatPromptTemplate.from_messages(
     [
         ("system", "You are a helpful AI assistant named Fred."),
         ("user", "{input}")
     ]
 )
 chain = (
     prompt
-    | ChatNVIDIA(model="ai-llama3-70b")
+    | ChatNVIDIA(model="meta/llama3-8b-instruct")
     | StrOutputParser()
 )
 
 for txt in chain.stream({"input": "What's your name?"}):
     print(txt, end="")
 ```
 
 ### Code Generation
 
-These models accept the same arguments and input structure as regular chat models, but they tend to perform better on code-genreation and structured code tasks. An example of this is `ai-codellama-70b` and `ai-codegemma-7b`.
+These models accept the same arguments and input structure as regular chat models, but they tend to perform better on code-genreation and structured code tasks. An example of this is `meta/codellama-70b` and `google/codegemma-7b`.
 
 ```python
 prompt = ChatPromptTemplate.from_messages(
     [
         ("system", "You are an expert coding AI. Respond only in valid python; no narration whatsoever."),
         ("user", "{input}")
     ]
 )
 chain = (
     prompt
-    | ChatNVIDIA(model="ai-codellama-70b", max_tokens=419)
+    | ChatNVIDIA(model="meta/codellama-70b", max_tokens=419)
     | StrOutputParser()
 )
 
 for txt in chain.stream({"input": "How do I solve this fizz buzz problem?"}):
     print(txt, end="")
 ```
 
@@ -214,15 +237,15 @@
     print(txt, end="")
 ```
 
 ## Multimodal
 
 NVIDIA also supports multimodal inputs, meaning you can provide both images and text for the model to reason over.
 
-An example model supporting multimodal inputs is `ai-neva-22b`.
+An example model supporting multimodal inputs is `nvidia/neva-22b`.
 
 These models accept LangChain's standard image formats. Below are examples.
 
 ```python
 import requests
 
 image_url = "https://picsum.photos/seed/kitten/300/200"
@@ -230,15 +253,15 @@
 ```
 
 Initialize the model like so:
 
 ```python
 from langchain_nvidia_ai_endpoints import ChatNVIDIA
 
-llm = ChatNVIDIA(model="ai-neva-22b")
+llm = ChatNVIDIA(model="nvidia/neva-22b")
 ```
 
 #### Passing an image as a URL
 
 ```python
 from langchain_core.messages import HumanMessage
 
@@ -272,50 +295,22 @@
 ```python
 base64_with_mime_type = f"data:image/png;base64,{b64_string}"
 llm.invoke(
     f'What\'s in this image?\n<img src="{base64_with_mime_type}" />'
 )
 ```
 
-## RAG: Context models
-
-NVIDIA also has Q&A models that support a special "context" chat message containing retrieved context (such as documents within a RAG chain). This is useful to avoid prompt-injecting the model.
-
-**Note:** Only "user" (human) and "context" chat messages are supported for these models, not system or AI messages useful in conversational flows.
-
-The `_qa_` models like `nemotron_qa_8b` support this.
-
-```python
-from langchain_nvidia_ai_endpoints import ChatNVIDIA
-from langchain_core.prompts import ChatPromptTemplate
-from langchain_core.output_parsers import StrOutputParser
-from langchain_core.messages import ChatMessage
-prompt = ChatPromptTemplate.from_messages(
-    [
-        ChatMessage(role="context", content="Parrots and Cats have signed the peace accord."),
-        ("user", "{input}")
-    ]
-)
-llm = ChatNVIDIA(model="nemotron_qa_8b")
-chain = (
-    prompt
-    | llm
-    | StrOutputParser()
-)
-chain.invoke({"input": "What was signed?"})
-```
-
 ## Embeddings
 
 You can also connect to embeddings models through this package. Below is an example:
 
 ```python
 from langchain_nvidia_ai_endpoints import NVIDIAEmbeddings
 
-embedder = NVIDIAEmbeddings(model="ai-embed-qa-4")
+embedder = NVIDIAEmbeddings(model="NV-Embed-QA")
 embedder.embed_query("What's the temperature today?")
 embedder.embed_documents([
     "The temperature is 42 degrees.",
     "Class is dismissed at 9 PM."
 ])
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

