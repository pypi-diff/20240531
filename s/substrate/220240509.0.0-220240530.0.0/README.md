# Comparing `tmp/substrate-220240509.0.0.tar.gz` & `tmp/substrate-220240530.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "substrate-220240509.0.0.tar", max compression
+gzip compressed data, was "substrate-220240530.0.0.tar", max compression
```

## Comparing `substrate-220240509.0.0.tar` & `substrate-220240530.0.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-220240509.0.0/LICENSE
--rw-r--r--   0        0        0     2715 2024-05-01 20:59:44.017862 substrate-220240509.0.0/README.md
--rw-r--r--   0        0        0     2079 2024-05-24 10:50:42.952002 substrate-220240509.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-220240509.0.0/substrate/.keep
--rw-r--r--   0        0        0       17 2024-05-24 10:31:07.000000 substrate-220240509.0.0/substrate/GEN_VERSION
--rw-r--r--   0        0        0     2189 2024-05-24 10:31:09.000000 substrate-220240509.0.0/substrate/__init__.py
--rw-r--r--   0        0        0     5885 2024-05-23 08:32:49.033293 substrate-220240509.0.0/substrate/_client.py
--rw-r--r--   0        0        0       30 2024-05-24 10:56:53.972716 substrate-220240509.0.0/substrate/_version.py
--rw-r--r--   0        0        0        1 2024-05-24 10:50:43.510765 substrate-220240509.0.0/substrate/core/__init__.py
--rw-r--r--   0        0        0       27 2024-05-24 10:50:43.510522 substrate-220240509.0.0/substrate/core/_version.py
--rw-r--r--   0        0        0     1535 2024-05-24 10:50:43.511260 substrate-220240509.0.0/substrate/core/base_future.py
--rw-r--r--   0        0        0        0 2024-05-24 10:50:43.512621 substrate-220240509.0.0/substrate/core/client/__init__.py
--rw-r--r--   0        0        0     1750 2024-05-24 10:50:43.512882 substrate-220240509.0.0/substrate/core/client/find_futures_client.py
--rw-r--r--   0        0        0     2697 2024-05-24 10:50:43.513384 substrate-220240509.0.0/substrate/core/client/future.py
--rw-r--r--   0        0        0     1212 2024-05-24 10:50:43.512440 substrate-220240509.0.0/substrate/core/client/graph.py
--rw-r--r--   0        0        0     1149 2024-05-24 10:50:43.511082 substrate-220240509.0.0/substrate/core/coregraph.py
--rw-r--r--   0        0        0     2212 2024-05-24 10:50:43.508719 substrate-220240509.0.0/substrate/core/corenode.py
--rw-r--r--   0        0        0     1587 2024-05-24 10:50:43.511587 substrate-220240509.0.0/substrate/core/future_directive.py
--rw-r--r--   0        0        0     1095 2024-05-24 10:50:43.508248 substrate-220240509.0.0/substrate/core/id_generator.py
--rw-r--r--   0        0        0    37376 2024-05-24 10:50:43.509677 substrate-220240509.0.0/substrate/core/models.py
--rw-r--r--   0        0        0     3798 2024-05-24 10:50:43.507773 substrate-220240509.0.0/substrate/core/sb.py
--rw-r--r--   0        0        0    32553 2024-04-19 00:53:25.000000 substrate-220240509.0.0/substrate/dataclass_models.py
--rw-r--r--   0        0        0    50559 2024-05-24 10:31:06.000000 substrate-220240509.0.0/substrate/future_dataclass_models.py
--rw-r--r--   0        0        0    59454 2024-05-24 10:46:13.000000 substrate-220240509.0.0/substrate/nodes.py
--rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-220240509.0.0/substrate/py.typed
--rw-r--r--   0        0        0     2196 2024-05-06 18:16:14.492293 substrate-220240509.0.0/substrate/substrate.py
--rw-r--r--   0        0        0     1015 2024-04-30 17:24:23.842724 substrate-220240509.0.0/substrate/substrate_response.py
--rw-r--r--   0        0        0    37780 2024-05-24 10:31:03.000000 substrate-220240509.0.0/substrate/typeddict_models.py
--rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 substrate-220240509.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-19 21:46:08.735767 substrate-220240530.0.0/LICENSE
+-rw-r--r--   0        0        0     2715 2024-05-01 20:59:44.017862 substrate-220240530.0.0/README.md
+-rw-r--r--   0        0        0     2079 2024-05-31 21:43:05.887526 substrate-220240530.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 19:17:25.000000 substrate-220240530.0.0/substrate/.keep
+-rw-r--r--   0        0        0       17 2024-05-31 21:42:04.000000 substrate-220240530.0.0/substrate/GEN_VERSION
+-rw-r--r--   0        0        0     2231 2024-05-31 21:42:05.000000 substrate-220240530.0.0/substrate/__init__.py
+-rw-r--r--   0        0        0     5885 2024-05-23 08:32:49.033293 substrate-220240530.0.0/substrate/_client.py
+-rw-r--r--   0        0        0       29 2024-05-31 21:43:05.887704 substrate-220240530.0.0/substrate/_version.py
+-rw-r--r--   0        0        0        1 2024-05-31 21:43:06.140547 substrate-220240530.0.0/substrate/core/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-31 21:43:06.140358 substrate-220240530.0.0/substrate/core/_version.py
+-rw-r--r--   0        0        0     1535 2024-05-31 21:43:06.140912 substrate-220240530.0.0/substrate/core/base_future.py
+-rw-r--r--   0        0        0        0 2024-05-31 21:43:06.141685 substrate-220240530.0.0/substrate/core/client/__init__.py
+-rw-r--r--   0        0        0     1750 2024-05-31 21:43:06.141851 substrate-220240530.0.0/substrate/core/client/find_futures_client.py
+-rw-r--r--   0        0        0     2697 2024-05-31 21:43:06.142061 substrate-220240530.0.0/substrate/core/client/future.py
+-rw-r--r--   0        0        0     1212 2024-05-31 21:43:06.141572 substrate-220240530.0.0/substrate/core/client/graph.py
+-rw-r--r--   0        0        0     1149 2024-05-31 21:43:06.140739 substrate-220240530.0.0/substrate/core/coregraph.py
+-rw-r--r--   0        0        0     2212 2024-05-31 21:43:06.139377 substrate-220240530.0.0/substrate/core/corenode.py
+-rw-r--r--   0        0        0     1587 2024-05-31 21:43:06.141104 substrate-220240530.0.0/substrate/core/future_directive.py
+-rw-r--r--   0        0        0     1095 2024-05-31 21:43:06.139156 substrate-220240530.0.0/substrate/core/id_generator.py
+-rw-r--r--   0        0        0    38289 2024-05-31 21:43:06.139654 substrate-220240530.0.0/substrate/core/models.py
+-rw-r--r--   0        0        0     3798 2024-05-31 21:43:06.138965 substrate-220240530.0.0/substrate/core/sb.py
+-rw-r--r--   0        0        0    32553 2024-04-19 00:53:25.000000 substrate-220240530.0.0/substrate/dataclass_models.py
+-rw-r--r--   0        0        0    51597 2024-05-31 21:42:03.000000 substrate-220240530.0.0/substrate/future_dataclass_models.py
+-rw-r--r--   0        0        0    60981 2024-05-31 21:42:53.000000 substrate-220240530.0.0/substrate/nodes.py
+-rw-r--r--   0        0        0        0 2024-02-07 23:39:17.000078 substrate-220240530.0.0/substrate/py.typed
+-rw-r--r--   0        0        0     2196 2024-05-06 18:16:14.492293 substrate-220240530.0.0/substrate/substrate.py
+-rw-r--r--   0        0        0     1015 2024-04-30 17:24:23.842724 substrate-220240530.0.0/substrate/substrate_response.py
+-rw-r--r--   0        0        0    38601 2024-05-31 21:42:02.000000 substrate-220240530.0.0/substrate/typeddict_models.py
+-rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 substrate-220240530.0.0/PKG-INFO
```

### Comparing `substrate-220240509.0.0/LICENSE` & `substrate-220240530.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `substrate-220240509.0.0/README.md` & `substrate-220240530.0.0/README.md`

 * *Files identical despite different names*

### Comparing `substrate-220240509.0.0/pyproject.toml` & `substrate-220240530.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "substrate"
-version = "220240509.0.0"
+version = "220240530.0.0"
 description = "Substrate Python SDK"
 readme = "README.md"
 authors = [ "vprtwn <ben@substrate.run>", "liamgriffiths <liam@substrate.run>",]
 [[tool.poetry.packages]]
 include = "substrate"
 
 [tool.pyright]
```

### Comparing `substrate-220240509.0.0/substrate/__init__.py` & `substrate-220240530.0.0/substrate/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 """
 𐃏 Substrate Python SDK
 
-20240509.20240524
+20240530.20240531
 """
 
 from .nodes import (
-    CLIP,
-    XTTSV2,
-    JinaV2,
-    RunCode,
-    FillMask,
-    EmbedText,
-    EmbedImage,
-    FetchVectors,
-    Firellava13B,
-    GenerateJSON,
+    Experimental,
+    RunPython,
     GenerateText,
-    UpscaleImage,
-    DeleteVectors,
-    GenerateImage,
-    UpdateVectors,
-    GenerateSpeech,
-    MultiEmbedText,
-    MultiEmbedImage,
-    SegmentAnything,
-    TranscribeMedia,
-    ListVectorStores,
-    Llama3Instruct8B,
-    QueryVectorStore,
-    RemoveBackground,
-    BatchGenerateJSON,
+    MultiGenerateText,
     BatchGenerateText,
-    CreateVectorStore,
-    DeleteVectorStore,
-    Llama3Instruct70B,
-    Mistral7BInstruct,
+    BatchGenerateJSON,
+    GenerateJSON,
     MultiGenerateJSON,
-    MultiGenerateText,
-    SegmentUnderPoint,
-    StableDiffusionXL,
     GenerateTextVision,
+    Mistral7BInstruct,
+    Mixtral8x7BInstruct,
+    Llama3Instruct8B,
+    Llama3Instruct70B,
+    Firellava13B,
+    GenerateImage,
     MultiGenerateImage,
     GenerativeEditImage,
-    Mixtral8x7BInstruct,
     MultiGenerativeEditImage,
-    StableDiffusionXLInpaint,
-    StableDiffusionXLIPAdapter,
+    StableDiffusionXL,
     StableDiffusionXLLightning,
+    StableDiffusionXLInpaint,
     StableDiffusionXLControlNet,
+    StableDiffusionXLIPAdapter,
+    TranscribeMedia,
+    GenerateSpeech,
+    XTTSV2,
+    RemoveBackground,
+    FillMask,
+    UpscaleImage,
+    SegmentUnderPoint,
+    SegmentAnything,
+    EmbedText,
+    MultiEmbedText,
+    EmbedImage,
+    MultiEmbedImage,
+    JinaV2,
+    CLIP,
+    CreateVectorStore,
+    ListVectorStores,
+    DeleteVectorStore,
+    QueryVectorStore,
+    FetchVectors,
+    UpdateVectors,
+    DeleteVectors,
 )
 from .core.sb import sb
 from ._version import __version__
 from .substrate import Substrate, SubstrateResponse
 
 __all__ = [
     "__version__",
     "SubstrateResponse",
     "sb",
     "Substrate",
-    "RunCode",
+    "Experimental",
+    "RunPython",
     "GenerateText",
     "MultiGenerateText",
     "BatchGenerateText",
     "BatchGenerateJSON",
     "GenerateJSON",
     "MultiGenerateJSON",
     "GenerateTextVision",
```

### Comparing `substrate-220240509.0.0/substrate/_client.py` & `substrate-220240530.0.0/substrate/_client.py`

 * *Files identical despite different names*

### Comparing `substrate-220240509.0.0/substrate/core/base_future.py` & `substrate-220240530.0.0/substrate/core/base_future.py`

 * *Files identical despite different names*

### Comparing `substrate-220240509.0.0/substrate/core/client/find_futures_client.py` & `substrate-220240530.0.0/substrate/core/client/find_futures_client.py`

 * *Files identical despite different names*

### Comparing `substrate-220240509.0.0/substrate/core/client/future.py` & `substrate-220240530.0.0/substrate/core/client/future.py`

 * *Files identical despite different names*

### Comparing `substrate-220240509.0.0/substrate/core/client/graph.py` & `substrate-220240530.0.0/substrate/core/client/graph.py`

 * *Files identical despite different names*

### Comparing `substrate-220240509.0.0/substrate/core/coregraph.py` & `substrate-220240530.0.0/substrate/core/coregraph.py`

 * *Files identical despite different names*

### Comparing `substrate-220240509.0.0/substrate/core/corenode.py` & `substrate-220240530.0.0/substrate/core/corenode.py`

 * *Files identical despite different names*

### Comparing `substrate-220240509.0.0/substrate/core/future_directive.py` & `substrate-220240530.0.0/substrate/core/future_directive.py`

 * *Files identical despite different names*

### Comparing `substrate-220240509.0.0/substrate/core/id_generator.py` & `substrate-220240530.0.0/substrate/core/id_generator.py`

 * *Files identical despite different names*

### Comparing `substrate-220240509.0.0/substrate/core/models.py` & `substrate-220240530.0.0/substrate/core/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,61 +4,87 @@
 (using datamodel-codegen)
 """
 
 
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional
-from typing_extensions import Literal, Annotated
 
-from pydantic import Field, BaseModel
+import os
+
+use_pydantic_v1 = os.getenv("USE_PYDANTIC_V1", "0").lower() == "1"
+
+if use_pydantic_v1:
+    from pydantic.v1 import BaseModel, Field
+else:
+    from pydantic import BaseModel, Field
+
+from typing_extensions import Annotated, Literal
 
 
 class ErrorOut(BaseModel):
     type: Literal["api_error", "invalid_request_error"]
     """
     The type of error returned.
     """
     message: str
     """
     A message providing more details about the error.
     """
-    request_id: Optional[str] = None
+
+
+class ExperimentalIn(BaseModel):
+    name: str
+    """
+    Identifier.
+    """
+    args: Dict[str, Any]
+    """
+    Arguments.
+    """
+    timeout: int = 60
+    """
+    Timeout in seconds.
+    """
+
+
+class ExperimentalOut(BaseModel):
+    output: Dict[str, Any]
     """
-    A unique identifier for the request.
+    Response.
     """
 
 
-class RunCodeIn(BaseModel):
+class RunPythonIn(BaseModel):
     code: str
     """
-    Code to execute.
+    Python code to execute. In your code, access values from the `input` parameter using the `SB_IN` variable. Update the `SB_OUT` variable with results you want returned in `output`.
     """
-    args: Optional[List[str]] = None
+    input: Optional[Dict[str, Any]] = None
     """
-    List of command line arguments.
+    Input to your code, accessible using the preloaded `SB_IN` variable.
     """
-    language: Literal["python", "typescript", "javascript"] = "python"
+    pip_install: Optional[List[str]] = None
     """
-    Interpreter to use.
+    Python packages to install. You must import them in your code.
     """
 
 
-class RunCodeOut(BaseModel):
-    output: Optional[str] = None
+class RunPythonOut(BaseModel):
+    stdout: str
     """
-    Contents of `stdout` after executing the code.
+    Everything printed to stdout while running your code.
     """
-    json_output: Dict[str, Any]
+    output: Dict[str, Any]
     """
-    `output` as parsed JSON. Print serialized json to `stdout` to receive JSON.
+    Contents of the `SB_OUT` variable after running your code.
     """
-    error: Optional[str] = None
+    stderr: str
     """
-    Contents of `stderr` after executing the code.
+    Contents of stderr if your code did not run successfully.
     """
 
 
 class GenerateTextIn(BaseModel):
     prompt: str
     """
     Input prompt.
@@ -102,15 +128,15 @@
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct", "Llama3Instruct8B"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 class GenerateJSONOut(BaseModel):
     json_object: Optional[Dict[str, Any]] = None
@@ -197,28 +223,32 @@
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct", "Llama3Instruct8B"] = "Mistral7BInstruct"
     """
     Selected node.
     """
 
 
 class MultiGenerateJSONOut(BaseModel):
     choices: List[GenerateJSONOut]
     """
     Response choices.
     """
 
 
 class BatchGenerateJSONIn(BaseModel):
+    node: Literal["Mistral7BInstruct", "Llama3Instruct8B"] = "Mistral7BInstruct"
+    """
+    Selected node.
+    """
     prompts: List[str]
     """
     Batch input prompts.
     """
     json_schema: Dict[str, Any]
     """
     JSON schema to guide `json_object` response.
@@ -335,21 +365,29 @@
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     Maximum number of tokens to generate.
     """
+    json_schema: Optional[Dict[str, Any]] = None
+    """
+    JSON schema to guide response.
+    """
 
 
 class Llama3Instruct8BChoice(BaseModel):
     text: Optional[str] = None
     """
     Text response.
     """
+    json_object: Optional[Dict[str, Any]] = None
+    """
+    JSON response, if `json_schema` was provided.
+    """
 
 
 class Llama3Instruct8BOut(BaseModel):
     choices: List[Llama3Instruct8BChoice]
     """
     Response choices.
     """
```

### Comparing `substrate-220240509.0.0/substrate/core/sb.py` & `substrate-220240530.0.0/substrate/core/sb.py`

 * *Files identical despite different names*

### Comparing `substrate-220240509.0.0/substrate/dataclass_models.py` & `substrate-220240530.0.0/substrate/dataclass_models.py`

 * *Files identical despite different names*

### Comparing `substrate-220240509.0.0/substrate/future_dataclass_models.py` & `substrate-220240530.0.0/substrate/future_dataclass_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 @generated file
 (using datamodel-codegen)
 """
 
 
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional
 from dataclasses import dataclass
+from typing import Any, Dict, List, Optional
+
 from typing_extensions import Literal
 
 
 @dataclass
 class ErrorOut:
     """
     Future reference to ErrorOut
@@ -24,64 +25,95 @@
     The type of error returned.
     """
     message: str
     """
     (Future reference)
     A message providing more details about the error.
     """
-    request_id: Optional[str] = None
+
+
+@dataclass
+class FutureExperimentalIn:
+    """
+    Future reference to FutureExperimentalIn
+    """
+
+    name: str
+    """
+    (Future reference)
+    Identifier.
+    """
+    args: Dict[str, Any]
+    """
+    (Future reference)
+    Arguments.
+    """
+    timeout: int = 60
+    """
+    (Future reference)
+    Timeout in seconds.
+    """
+
+
+@dataclass
+class FutureExperimentalOut:
+    """
+    Future reference to FutureExperimentalOut
+    """
+
+    output: Dict[str, Any]
     """
     (Future reference)
-    A unique identifier for the request.
+    Response.
     """
 
 
 @dataclass
-class FutureRunCodeIn:
+class FutureRunPythonIn:
     """
-    Future reference to FutureRunCodeIn
+    Future reference to FutureRunPythonIn
     """
 
     code: str
     """
     (Future reference)
-    Code to execute.
+    Python code to execute. In your code, access values from the `input` parameter using the `SB_IN` variable. Update the `SB_OUT` variable with results you want returned in `output`.
     """
-    args: Optional[List[str]] = None
+    input: Optional[Dict[str, Any]] = None
     """
     (Future reference)
-    List of command line arguments.
+    Input to your code, accessible using the preloaded `SB_IN` variable.
     """
-    language: Literal["python", "typescript", "javascript"] = "python"
+    pip_install: Optional[List[str]] = None
     """
     (Future reference)
-    Interpreter to use.
+    Python packages to install. You must import them in your code.
     """
 
 
 @dataclass
-class FutureRunCodeOut:
+class FutureRunPythonOut:
     """
-    Future reference to FutureRunCodeOut
+    Future reference to FutureRunPythonOut
     """
 
-    json_output: Dict[str, Any]
+    stdout: str
     """
     (Future reference)
-    `output` as parsed JSON. Print serialized json to `stdout` to receive JSON.
+    Everything printed to stdout while running your code.
     """
-    output: Optional[str] = None
+    output: Dict[str, Any]
     """
     (Future reference)
-    Contents of `stdout` after executing the code.
+    Contents of the `SB_OUT` variable after running your code.
     """
-    error: Optional[str] = None
+    stderr: str
     """
     (Future reference)
-    Contents of `stderr` after executing the code.
+    Contents of stderr if your code did not run successfully.
     """
 
 
 @dataclass
 class FutureGenerateTextIn:
     """
     Future reference to FutureGenerateTextIn
@@ -149,15 +181,15 @@
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct", "Llama3Instruct8B"] = "Mistral7BInstruct"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -292,15 +324,15 @@
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
-    node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"] = "Mistral7BInstruct"
+    node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct", "Llama3Instruct8B"] = "Mistral7BInstruct"
     """
     (Future reference)
     Selected node.
     """
 
 
 @dataclass
@@ -328,14 +360,19 @@
     Batch input prompts.
     """
     json_schema: Dict[str, Any]
     """
     (Future reference)
     JSON schema to guide `json_object` response.
     """
+    node: Literal["Mistral7BInstruct", "Llama3Instruct8B"] = "Mistral7BInstruct"
+    """
+    (Future reference)
+    Selected node.
+    """
     temperature: float = 0.4
     """
     (Future reference)
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
@@ -507,27 +544,37 @@
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: Optional[int] = None
     """
     (Future reference)
     Maximum number of tokens to generate.
     """
+    json_schema: Optional[Dict[str, Any]] = None
+    """
+    (Future reference)
+    JSON schema to guide response.
+    """
 
 
 @dataclass
 class Llama3Instruct8BChoice:
     """
     Future reference to Llama3Instruct8BChoice
     """
 
     text: Optional[str] = None
     """
     (Future reference)
     Text response.
     """
+    json_object: Optional[Dict[str, Any]] = None
+    """
+    (Future reference)
+    JSON response, if `json_schema` was provided.
+    """
 
 
 @dataclass
 class FutureLlama3Instruct8BOut:
     """
     Future reference to FutureLlama3Instruct8BOut
     """
```

### Comparing `substrate-220240509.0.0/substrate/nodes.py` & `substrate-220240530.0.0/substrate/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,137 +1,172 @@
 """
 𐃏 Substrate
 @GENERATED FILE
-20240509.20240524
 """
 from __future__ import annotations
-
-from typing import Any, Dict, List, Optional
-from typing_extensions import Literal
-
+from .substrate import SubstrateResponse
+from .core.corenode import CoreNode
 from .core.models import (
-    CLIPOut,
-    JinaV2Out,
-    XTTSV2Out,
-    RunCodeOut,
-    FillMaskOut,
-    EmbedTextOut,
-    EmbedImageOut,
-    FetchVectorsOut,
-    Firellava13BOut,
-    GenerateJSONOut,
+    ExperimentalOut,
+    RunPythonOut,
     GenerateTextOut,
-    UpscaleImageOut,
-    DeleteVectorsOut,
-    GenerateImageOut,
-    UpdateVectorsOut,
-    GenerateSpeechOut,
-    MultiEmbedTextOut,
-    MultiEmbedImageOut,
-    SegmentAnythingOut,
-    TranscribeMediaOut,
-    ListVectorStoresOut,
-    Llama3Instruct8BOut,
-    QueryVectorStoreOut,
-    RemoveBackgroundOut,
-    BatchGenerateJSONOut,
+    MultiGenerateTextOut,
     BatchGenerateTextOut,
-    CreateVectorStoreOut,
-    DeleteVectorStoreOut,
-    Llama3Instruct70BOut,
-    Mistral7BInstructOut,
+    BatchGenerateJSONOut,
+    GenerateJSONOut,
     MultiGenerateJSONOut,
-    MultiGenerateTextOut,
-    SegmentUnderPointOut,
-    StableDiffusionXLOut,
     GenerateTextVisionOut,
+    Mistral7BInstructOut,
+    Mixtral8x7BInstructOut,
+    Llama3Instruct8BOut,
+    Llama3Instruct70BOut,
+    Firellava13BOut,
+    GenerateImageOut,
     MultiGenerateImageOut,
     GenerativeEditImageOut,
-    Mixtral8x7BInstructOut,
     MultiGenerativeEditImageOut,
-    StableDiffusionXLInpaintOut,
-    StableDiffusionXLIPAdapterOut,
+    StableDiffusionXLOut,
     StableDiffusionXLLightningOut,
+    StableDiffusionXLInpaintOut,
     StableDiffusionXLControlNetOut,
+    StableDiffusionXLIPAdapterOut,
+    TranscribeMediaOut,
+    GenerateSpeechOut,
+    XTTSV2Out,
+    RemoveBackgroundOut,
+    FillMaskOut,
+    UpscaleImageOut,
+    SegmentUnderPointOut,
+    SegmentAnythingOut,
+    EmbedTextOut,
+    MultiEmbedTextOut,
+    EmbedImageOut,
+    MultiEmbedImageOut,
+    JinaV2Out,
+    CLIPOut,
+    CreateVectorStoreOut,
+    ListVectorStoresOut,
+    DeleteVectorStoreOut,
+    QueryVectorStoreOut,
+    FetchVectorsOut,
+    UpdateVectorsOut,
+    DeleteVectorsOut,
 )
-from .core.corenode import CoreNode
 from .future_dataclass_models import (
-    FutureCLIPOut,
-    FutureJinaV2Out,
-    FutureXTTSV2Out,
-    FutureRunCodeOut,
-    FutureFillMaskOut,
-    FutureEmbedTextOut,
-    FutureEmbedImageOut,
-    FutureFetchVectorsOut,
-    FutureFirellava13BOut,
-    FutureGenerateJSONOut,
+    FutureExperimentalOut,
+    FutureRunPythonOut,
     FutureGenerateTextOut,
-    FutureUpscaleImageOut,
-    FutureDeleteVectorsOut,
-    FutureGenerateImageOut,
-    FutureUpdateVectorsOut,
-    FutureGenerateSpeechOut,
-    FutureMultiEmbedTextOut,
-    FutureMultiEmbedImageOut,
-    FutureSegmentAnythingOut,
-    FutureTranscribeMediaOut,
-    FutureListVectorStoresOut,
-    FutureLlama3Instruct8BOut,
-    FutureQueryVectorStoreOut,
-    FutureRemoveBackgroundOut,
-    FutureBatchGenerateJSONOut,
+    FutureMultiGenerateTextOut,
     FutureBatchGenerateTextOut,
-    FutureCreateVectorStoreOut,
-    FutureDeleteVectorStoreOut,
-    FutureLlama3Instruct70BOut,
-    FutureMistral7BInstructOut,
+    FutureBatchGenerateJSONOut,
+    FutureGenerateJSONOut,
     FutureMultiGenerateJSONOut,
-    FutureMultiGenerateTextOut,
-    FutureSegmentUnderPointOut,
-    FutureStableDiffusionXLOut,
     FutureGenerateTextVisionOut,
+    FutureMistral7BInstructOut,
+    FutureMixtral8x7BInstructOut,
+    FutureLlama3Instruct8BOut,
+    FutureLlama3Instruct70BOut,
+    FutureFirellava13BOut,
+    FutureGenerateImageOut,
     FutureMultiGenerateImageOut,
     FutureGenerativeEditImageOut,
-    FutureMixtral8x7BInstructOut,
     FutureMultiGenerativeEditImageOut,
-    FutureStableDiffusionXLInpaintOut,
-    FutureStableDiffusionXLIPAdapterOut,
+    FutureStableDiffusionXLOut,
     FutureStableDiffusionXLLightningOut,
+    FutureStableDiffusionXLInpaintOut,
     FutureStableDiffusionXLControlNetOut,
+    FutureStableDiffusionXLIPAdapterOut,
+    FutureTranscribeMediaOut,
+    FutureGenerateSpeechOut,
+    FutureXTTSV2Out,
+    FutureRemoveBackgroundOut,
+    FutureFillMaskOut,
+    FutureUpscaleImageOut,
+    FutureSegmentUnderPointOut,
+    FutureSegmentAnythingOut,
+    FutureEmbedTextOut,
+    FutureMultiEmbedTextOut,
+    FutureEmbedImageOut,
+    FutureMultiEmbedImageOut,
+    FutureJinaV2Out,
+    FutureCLIPOut,
+    FutureCreateVectorStoreOut,
+    FutureListVectorStoresOut,
+    FutureDeleteVectorStoreOut,
+    FutureQueryVectorStoreOut,
+    FutureFetchVectorsOut,
+    FutureUpdateVectorsOut,
+    FutureDeleteVectorsOut,
 )
 
 
-class RunCode(CoreNode[RunCodeOut]):
-    """https://substrate.run/nodes#RunCode"""
+from dataclasses import dataclass
+from typing import Any, Dict, List, Optional
+
+from typing_extensions import Literal
+
+
+class Experimental(CoreNode[ExperimentalOut]):
+    """https://substrate.run/nodes#Experimental"""
+
+    def __init__(self, name: str, args: Dict[str, Any], timeout: int = 60, hide: bool = False):
+        """
+        Args:
+            name: Identifier.
+            args: Arguments.
+            timeout: Timeout in seconds.
+
+        https://substrate.run/nodes#Experimental
+        """
+        super().__init__(name=name, args=args, timeout=timeout, hide=hide, out_type=ExperimentalOut)
+        self.node = "Experimental"
+
+    @property
+    def future(self) -> FutureExperimentalOut:  # type: ignore
+        """
+        Future reference to this node's output.
+
+        https://substrate.run/nodes#Experimental
+        """
+        return super().future  # type: ignore
+
+
+class RunPython(CoreNode[RunPythonOut]):
+    """https://substrate.run/nodes#RunPython"""
 
     def __init__(
         self,
         code: str,
-        args: Optional[List[str]] = None,
-        language: Literal["python", "typescript", "javascript"] = "python",
+        input: Optional[Dict[str, Any]] = None,
+        pip_install: Optional[List[str]] = None,
         hide: bool = False,
     ):
         """
         Args:
-            code: Code to execute.
-            args: List of command line arguments.
-            language: Interpreter to use.
+            code: Python code to execute. In your code, access values from the `input` parameter using the `SB_IN` variable. Update the `SB_OUT` variable with results you want returned in `output`.
+            input: Input to your code, accessible using the preloaded `SB_IN` variable.
+            pip_install: Python packages to install. You must import them in your code.
 
-        https://substrate.run/nodes#RunCode
+        https://substrate.run/nodes#RunPython
         """
-        super().__init__(code=code, args=args, language=language, hide=hide, out_type=RunCodeOut)
-        self.node = "RunCode"
+        super().__init__(
+            code=code,
+            input=input,
+            pip_install=pip_install,
+            hide=hide,
+            out_type=RunPythonOut,
+        )
+        self.node = "RunPython"
 
     @property
-    def future(self) -> FutureRunCodeOut:  # type: ignore
+    def future(self) -> FutureRunPythonOut:  # type: ignore
         """
         Future reference to this node's output.
 
-        https://substrate.run/nodes#RunCode
+        https://substrate.run/nodes#RunPython
         """
         return super().future  # type: ignore
 
 
 class GenerateText(CoreNode[GenerateTextOut]):
     """https://substrate.run/nodes#GenerateText"""
 
@@ -182,15 +217,15 @@
 
     def __init__(
         self,
         prompt: str,
         json_schema: Dict[str, Any],
         temperature: float = 0.4,
         max_tokens: Optional[int] = None,
-        node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"] = "Mistral7BInstruct",
+        node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct", "Llama3Instruct8B"] = "Mistral7BInstruct",
         hide: bool = False,
     ):
         """
         Args:
             prompt: Input prompt.
             json_schema: JSON schema to guide `json_object` response.
             temperature: Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
@@ -311,15 +346,15 @@
     def __init__(
         self,
         prompt: str,
         json_schema: Dict[str, Any],
         num_choices: int,
         temperature: float = 0.4,
         max_tokens: Optional[int] = None,
-        node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"] = "Mistral7BInstruct",
+        node: Literal["Mistral7BInstruct", "Mixtral8x7BInstruct", "Llama3Instruct8B"] = "Mistral7BInstruct",
         hide: bool = False,
     ):
         """
         Args:
             prompt: Input prompt.
             json_schema: JSON schema to guide `json_object` response.
             num_choices: Number of choices to generate.
@@ -354,30 +389,33 @@
 class BatchGenerateJSON(CoreNode[BatchGenerateJSONOut]):
     """https://substrate.run/nodes#BatchGenerateJSON"""
 
     def __init__(
         self,
         prompts: List[str],
         json_schema: Dict[str, Any],
+        node: Literal["Mistral7BInstruct", "Llama3Instruct8B"] = "Mistral7BInstruct",
         temperature: float = 0.4,
         max_tokens: Optional[int] = None,
         hide: bool = False,
     ):
         """
         Args:
             prompts: Batch input prompts.
             json_schema: JSON schema to guide `json_object` response.
+            node: Selected node.
             temperature: Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
             max_tokens: Maximum number of tokens to generate.
 
         https://substrate.run/nodes#BatchGenerateJSON
         """
         super().__init__(
             prompts=prompts,
             json_schema=json_schema,
+            node=node,
             temperature=temperature,
             max_tokens=max_tokens,
             hide=hide,
             out_type=BatchGenerateJSONOut,
         )
         self.node = "BatchGenerateJSON"
 
@@ -482,30 +520,33 @@
 
     def __init__(
         self,
         prompt: str,
         num_choices: int = 1,
         temperature: Optional[float] = None,
         max_tokens: Optional[int] = None,
+        json_schema: Optional[Dict[str, Any]] = None,
         hide: bool = False,
     ):
         """
         Args:
             prompt: Input prompt.
             num_choices: Number of choices to generate.
             temperature: Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
             max_tokens: Maximum number of tokens to generate.
+            json_schema: JSON schema to guide response.
 
         https://substrate.run/nodes#Llama3Instruct8B
         """
         super().__init__(
             prompt=prompt,
             num_choices=num_choices,
             temperature=temperature,
             max_tokens=max_tokens,
+            json_schema=json_schema,
             hide=hide,
             out_type=Llama3Instruct8BOut,
         )
         self.node = "Llama3Instruct8B"
 
     @property
     def future(self) -> FutureLlama3Instruct8BOut:  # type: ignore
```

### Comparing `substrate-220240509.0.0/substrate/substrate.py` & `substrate-220240530.0.0/substrate/substrate.py`

 * *Files identical despite different names*

### Comparing `substrate-220240509.0.0/substrate/substrate_response.py` & `substrate-220240530.0.0/substrate/substrate_response.py`

 * *Files identical despite different names*

### Comparing `substrate-220240509.0.0/substrate/typeddict_models.py` & `substrate-220240530.0.0/substrate/typeddict_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,59 +4,78 @@
 (using datamodel-codegen)
 """
 
 
 from __future__ import annotations
 
 from typing import Any, Dict, List
-from typing_extensions import Literal, TypedDict, NotRequired
+
+from typing_extensions import Literal, NotRequired, TypedDict
 
 
 class ErrorOut(TypedDict):
     type: NotRequired[Literal["api_error", "invalid_request_error"]]
     """
     The type of error returned.
     """
     message: NotRequired[str]
     """
     A message providing more details about the error.
     """
-    request_id: NotRequired[str]
+
+
+class ExperimentalIn(TypedDict):
+    name: NotRequired[str]
+    """
+    Identifier.
+    """
+    args: NotRequired[Dict[str, Any]]
+    """
+    Arguments.
+    """
+    timeout: NotRequired[int]
+    """
+    Timeout in seconds.
+    """
+
+
+class ExperimentalOut(TypedDict):
+    output: NotRequired[Dict[str, Any]]
     """
-    A unique identifier for the request.
+    Response.
     """
 
 
-class RunCodeIn(TypedDict):
+class RunPythonIn(TypedDict):
     code: NotRequired[str]
     """
-    Code to execute.
+    Python code to execute. In your code, access values from the `input` parameter using the `SB_IN` variable. Update the `SB_OUT` variable with results you want returned in `output`.
     """
-    args: NotRequired[List[str]]
+    input: NotRequired[Dict[str, Any]]
     """
-    List of command line arguments.
+    Input to your code, accessible using the preloaded `SB_IN` variable.
     """
-    language: NotRequired[Literal["python", "typescript", "javascript"]]
+    pip_install: NotRequired[List[str]]
     """
-    Interpreter to use.
+    Python packages to install. You must import them in your code.
     """
 
 
-class RunCodeOut(TypedDict):
-    output: NotRequired[str]
+class RunPythonOut(TypedDict):
+    stdout: NotRequired[str]
     """
-    Contents of `stdout` after executing the code.
+    Everything printed to stdout while running your code.
     """
-    json_output: NotRequired[Dict[str, Any]]
+    output: NotRequired[Dict[str, Any]]
     """
-    `output` as parsed JSON. Print serialized json to `stdout` to receive JSON.
+    Contents of the `SB_OUT` variable after running your code.
     """
-    error: NotRequired[str]
+    stderr: NotRequired[str]
     """
-    Contents of `stderr` after executing the code.
+    Contents of stderr if your code did not run successfully.
     """
 
 
 class GenerateTextIn(TypedDict):
     prompt: NotRequired[str]
     """
     Input prompt.
@@ -102,15 +121,15 @@
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     Maximum number of tokens to generate.
     """
-    node: NotRequired[Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"]]
+    node: NotRequired[Literal["Mistral7BInstruct", "Mixtral8x7BInstruct", "Llama3Instruct8B"]]
     """
     Selected node.
     """
 
 
 class GenerateJSONOut(TypedDict):
     json_object: NotRequired[Dict[str, Any]]
@@ -199,28 +218,32 @@
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     Maximum number of tokens to generate.
     """
-    node: NotRequired[Literal["Mistral7BInstruct", "Mixtral8x7BInstruct"]]
+    node: NotRequired[Literal["Mistral7BInstruct", "Mixtral8x7BInstruct", "Llama3Instruct8B"]]
     """
     Selected node.
     """
 
 
 class MultiGenerateJSONOut(TypedDict):
     choices: NotRequired[List[GenerateJSONOut]]
     """
     Response choices.
     """
 
 
 class BatchGenerateJSONIn(TypedDict):
+    node: NotRequired[Literal["Mistral7BInstruct", "Llama3Instruct8B"]]
+    """
+    Selected node.
+    """
     prompts: NotRequired[List[str]]
     """
     Batch input prompts.
     """
     json_schema: NotRequired[Dict[str, Any]]
     """
     JSON schema to guide `json_object` response.
@@ -337,21 +360,29 @@
     """
     Sampling temperature to use. Higher values make the output more random, lower values make the output more deterministic.
     """
     max_tokens: NotRequired[int]
     """
     Maximum number of tokens to generate.
     """
+    json_schema: NotRequired[Dict[str, Any]]
+    """
+    JSON schema to guide response.
+    """
 
 
 class Llama3Instruct8BChoice(TypedDict):
     text: NotRequired[str]
     """
     Text response.
     """
+    json_object: NotRequired[Dict[str, Any]]
+    """
+    JSON response, if `json_schema` was provided.
+    """
 
 
 class Llama3Instruct8BOut(TypedDict):
     choices: NotRequired[List[Llama3Instruct8BChoice]]
     """
     Response choices.
     """
```

### Comparing `substrate-220240509.0.0/PKG-INFO` & `substrate-220240530.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: substrate
-Version: 220240509.0.0
+Version: 220240530.0.0
 Summary: Substrate Python SDK
 Author: vprtwn
 Author-email: ben@substrate.run
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

