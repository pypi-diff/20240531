# Comparing `tmp/llama_index_llms_openllm-0.1.4.tar.gz` & `tmp/llama_index_llms_openllm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_openllm-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_llms_openllm-0.1.5.tar", max compression
```

## Comparing `llama_index_llms_openllm-0.1.4.tar` & `llama_index_llms_openllm-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       39 2024-04-08 19:31:00.055091 llama_index_llms_openllm-0.1.4/README.md
--rw-r--r--   0        0        0       99 2024-04-08 19:31:00.059091 llama_index_llms_openllm-0.1.4/llama_index/llms/openllm/__init__.py
--rw-r--r--   0        0        0    17798 2024-04-08 19:31:00.059091 llama_index_llms_openllm-0.1.4/llama_index/llms/openllm/base.py
--rw-r--r--   0        0        0     1499 2024-04-08 19:31:00.059091 llama_index_llms_openllm-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 llama_index_llms_openllm-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-05-30 22:09:05.553634 llama_index_llms_openllm-0.1.5/README.md
+-rw-r--r--   0        0        0       99 2024-05-30 22:09:05.553634 llama_index_llms_openllm-0.1.5/llama_index/llms/openllm/__init__.py
+-rw-r--r--   0        0        0    17957 2024-05-30 22:09:05.557634 llama_index_llms_openllm-0.1.5/llama_index/llms/openllm/base.py
+-rw-r--r--   0        0        0     1494 2024-05-30 22:09:05.557634 llama_index_llms_openllm-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 llama_index_llms_openllm-0.1.5/PKG-INFO
```

### Comparing `llama_index_llms_openllm-0.1.4/llama_index/llms/openllm/base.py` & `llama_index_llms_openllm-0.1.5/llama_index/llms/openllm/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,28 +33,29 @@
 from llama_index.core.base.llms.generic_utils import (
     messages_to_prompt as generic_messages_to_prompt,
 )
 from llama_index.core.llms.llm import LLM
 from llama_index.core.types import PydanticProgramMode
 from openllm_client import AsyncHTTPClient, HTTPClient
 
-import openllm
+import openllm, openllm_core as core
 
 logger = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from typing import TypeVar
 
     M = TypeVar("M")
     T = TypeVar("T")
     Metadata = Any
 
 
 class OpenLLM(LLM):
-    """OpenLLM LLM.
+    """
+    OpenLLM LLM.
 
     Examples:
         `pip install llama-index-llms-openllm`
 
         ```python
         # If needed, set the OPENLLM_ENDPOINT environment variable to a remote server address
         # os.environ["OPENLLM_ENDPOINT"] = "remote_server_address"
@@ -69,82 +70,87 @@
         print(str(response))
         ```
     """
 
     model_id: str = Field(
         description="Given Model ID from HuggingFace Hub. This can be either a pretrained ID or local path. This is synonymous to HuggingFace's '.from_pretrained' first argument"
     )
-    model_version: Optional[str] = Field(
-        description="Optional model version to save the model as."
-    )
-    model_tag: Optional[str] = Field(
-        description="Optional tag to save to BentoML store."
-    )
-    prompt_template: Optional[str] = Field(
-        description="Optional prompt template to pass for this LLM."
-    )
-    backend: Optional[Literal["vllm", "pt"]] = Field(
-        description="Optional backend to pass for this LLM. By default, it will use vLLM if vLLM is available in local system. Otherwise, it will fallback to PyTorch."
-    )
-    quantize: Optional[Literal["awq", "gptq", "int8", "int4", "squeezellm"]] = Field(
+    quantize: Optional[Literal["awq", "gptq", "squeezellm"]] = Field(
         description="Optional quantization methods to use with this LLM. See OpenLLM's --quantize options from `openllm start` for more information."
     )
     serialization: Literal["safetensors", "legacy"] = Field(
         description="Optional serialization methods for this LLM to be save as. Default to 'safetensors', but will fallback to PyTorch pickle `.bin` on some models."
     )
     trust_remote_code: bool = Field(
         description="Optional flag to trust remote code. This is synonymous to Transformers' `trust_remote_code`. Default to False."
     )
-    _llm: openllm.LLM[Any, Any] = PrivateAttr()
+    model_version: Optional[str] = Field(
+        description="(DEPRECATED) Optional model version to save the model as."
+    )
+    model_tag: Optional[str] = Field(
+        description="(DEPRECATED) Optional tag to save to BentoML store."
+    )
+    prompt_template: Optional[str] = Field(
+        description="(DEPRECATED) Optional prompt template to pass for this LLM."
+    )
+    backend: Optional[Literal["vllm", "pt"]] = Field(
+        description="(DEPRECATED) Optional backend to pass for this LLM. Default to use vLLM."
+    )
+    _llm: openllm.LLM = PrivateAttr()
+    _engine_args: Dict[str, Any] = PrivateAttr()
 
     def __init__(
         self,
         model_id: str,
         model_version: Optional[str] = None,
         model_tag: Optional[str] = None,
         prompt_template: Optional[str] = None,
         backend: Optional[Literal["vllm", "pt"]] = None,
+        dtype: str = "auto",
         *args: Any,
-        quantize: Optional[Literal["awq", "gptq", "int8", "int4", "squeezellm"]] = None,
+        quantize: Optional[Literal["awq", "gptq", "squeezellm"]] = None,
         serialization: Literal["safetensors", "legacy"] = "safetensors",
         trust_remote_code: bool = False,
         callback_manager: Optional[CallbackManager] = None,
         system_prompt: Optional[str] = None,
         messages_to_prompt: Optional[Callable[[Sequence[ChatMessage]], str]] = None,
         completion_to_prompt: Optional[Callable[[str], str]] = None,
         pydantic_program_mode: PydanticProgramMode = PydanticProgramMode.DEFAULT,
         **attrs: Any,
     ):
-        self._llm = openllm.LLM[Any, Any](
+        if backend and backend != "vllm":
+            logger.warning(
+                "backend has been deprecated in OpenLLM 0.5 and above and will be default to vllm."
+            )
+        if model_version or model_tag or prompt_template:
+            logger.warning("This option is now deprecated and won't be used")
+        self._llm = openllm.LLM.from_model(
             model_id,
-            model_version=model_version,
-            model_tag=model_tag,
-            prompt_template=prompt_template,
-            system_message=system_prompt,
-            backend=backend,
-            quantize=quantize,
+            dtype=dtype,
+            llm_config=core.AutoConfig.from_id(
+                model_id, trust_remote_code=trust_remote_code
+            ),
+            quantise=quantize,
             serialisation=serialization,
             trust_remote_code=trust_remote_code,
-            embedded=True,
             **attrs,
         )
         if messages_to_prompt is None:
             messages_to_prompt = self._tokenizer_messages_to_prompt
 
-        # NOTE: We need to do this here to ensure model is saved and revision is set correctly.
-        assert self._llm.bentomodel
+        self._engine_args = self._llm.engine_args
 
         super().__init__(
             model_id=model_id,
-            model_version=self._llm.revision,
-            model_tag=str(self._llm.tag),
-            prompt_template=prompt_template,
-            backend=self._llm.__llm_backend__,
+            model_version="",
+            model_tag="",
+            backend="vllm",
+            prompt_template=None,
             quantize=self._llm.quantise,
-            serialization=self._llm._serialisation,
+            serialization=self._llm.serialisation,
             trust_remote_code=self._llm.trust_remote_code,
             callback_manager=callback_manager,
             system_prompt=system_prompt,
             messages_to_prompt=messages_to_prompt,
             completion_to_prompt=completion_to_prompt,
             pydantic_program_mode=pydantic_program_mode,
         )
@@ -261,18 +267,19 @@
         config = self._llm.config.model_construct_env(**kwargs)
         if config["n"] > 1:
             logger.warning("Currently only support n=1")
 
         texts: List[List[str]] = [[]] * config["n"]
 
         async for response_chunk in self._llm.generate_iterator(prompt, **kwargs):
+            print(response_chunk)
             for output in response_chunk.outputs:
                 texts[output.index].append(output.text)
             yield CompletionResponse(
-                text=response_chunk.outputs[0].text,
+                text="".join(texts[0]),
                 delta=response_chunk.outputs[0].text,
                 raw=response_chunk.model_dump(),
                 additional_kwargs={
                     "prompt_token_ids": response_chunk.prompt_token_ids,
                     "prompt_logprobs": response_chunk.prompt_logprobs,
                     "finished": response_chunk.finished,
                     "outputs": {
```

### Comparing `llama_index_llms_openllm-0.1.4/pyproject.toml` & `llama_index_llms_openllm-0.1.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -8,37 +8,37 @@
 skip = "*.csv,*.html,*.json,*.jsonl,*.pdf,*.txt,*.ipynb"
 
 [tool.llamahub]
 contains_example = false
 import_path = "llama_index.llms.openllm"
 
 [tool.llamahub.class_authors]
-OpenLLM = "llama-index"
-OpenLLMAPI = "llama-index"
+OpenLLM = "aarnphm"
+OpenLLMAPI = "aarnphm"
 
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
-authors = ["Your Name <you@example.com>"]
+authors = ["Aaron Pham <aarnphm@bentoml.com>"]
 description = "llama-index llms openllm integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-openllm"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
-openllm-client = "^0.4.41"
-openllm = "^0.4.41"
+openllm-client = "^0.5.3"
+openllm = "^0.5.3"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

