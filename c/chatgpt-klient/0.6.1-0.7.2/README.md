# Comparing `tmp/chatgpt_klient-0.6.1.tar.gz` & `tmp/chatgpt_klient-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt_klient-0.6.1.tar", last modified: Tue May 28 08:25:19 2024, max compression
+gzip compressed data, was "chatgpt_klient-0.7.2.tar", last modified: Fri May 31 09:15:58 2024, max compression
```

## Comparing `chatgpt_klient-0.6.1.tar` & `chatgpt_klient-0.7.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-05-28 08:25:19.573268 chatgpt_klient-0.6.1/
--rw-r--r--   0 serpucga  (1000) serpucga  (1000)      219 2024-05-28 08:25:19.573268 chatgpt_klient-0.6.1/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      508 2023-11-07 16:15:45.000000 chatgpt_klient-0.6.1/README.md
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      274 2024-05-28 08:24:20.000000 chatgpt_klient-0.6.1/pyproject.toml
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2024-05-28 08:25:19.573268 chatgpt_klient-0.6.1/setup.cfg
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-05-28 08:25:19.561268 chatgpt_klient-0.6.1/src/
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-05-28 08:25:19.569268 chatgpt_klient-0.6.1/src/chatgpt_klient/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       71 2024-05-28 08:24:26.000000 chatgpt_klient-0.6.1/src/chatgpt_klient/__init__.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)    17830 2024-05-28 07:45:57.000000 chatgpt_klient-0.6.1/src/chatgpt_klient/client.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     2306 2024-05-28 07:45:31.000000 chatgpt_klient-0.6.1/src/chatgpt_klient/consts.py
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      140 2023-07-14 07:46:22.000000 chatgpt_klient-0.6.1/src/chatgpt_klient/exceptions.py
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-05-28 08:25:19.573268 chatgpt_klient-0.6.1/src/chatgpt_klient.egg-info/
--rw-r--r--   0 serpucga  (1000) serpucga  (1000)      219 2024-05-28 08:25:19.000000 chatgpt_klient-0.6.1/src/chatgpt_klient.egg-info/PKG-INFO
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      376 2024-05-28 08:25:19.000000 chatgpt_klient-0.6.1/src/chatgpt_klient.egg-info/SOURCES.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2024-05-28 08:25:19.000000 chatgpt_klient-0.6.1/src/chatgpt_klient.egg-info/dependency_links.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       86 2024-05-28 08:25:19.000000 chatgpt_klient-0.6.1/src/chatgpt_klient.egg-info/requires.txt
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2024-05-28 08:25:19.000000 chatgpt_klient-0.6.1/src/chatgpt_klient.egg-info/top_level.txt
-drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-05-28 08:25:19.569268 chatgpt_klient-0.6.1/tests/
--rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     2015 2024-05-28 08:10:24.000000 chatgpt_klient-0.6.1/tests/test_client.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-05-31 09:15:58.340453 chatgpt_klient-0.7.2/
+-rw-r--r--   0 serpucga  (1000) serpucga  (1000)      219 2024-05-31 09:15:58.340453 chatgpt_klient-0.7.2/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      508 2023-11-07 16:15:45.000000 chatgpt_klient-0.7.2/README.md
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      274 2024-05-31 09:14:44.000000 chatgpt_klient-0.7.2/pyproject.toml
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       38 2024-05-31 09:15:58.340453 chatgpt_klient-0.7.2/setup.cfg
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-05-31 09:15:58.332453 chatgpt_klient-0.7.2/src/
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-05-31 09:15:58.336453 chatgpt_klient-0.7.2/src/chatgpt_klient/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       67 2024-05-31 09:14:54.000000 chatgpt_klient-0.7.2/src/chatgpt_klient/__init__.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)    17199 2024-05-31 09:13:21.000000 chatgpt_klient-0.7.2/src/chatgpt_klient/client.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     2377 2024-05-31 08:41:30.000000 chatgpt_klient-0.7.2/src/chatgpt_klient/consts.py
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      140 2023-07-14 07:46:22.000000 chatgpt_klient-0.7.2/src/chatgpt_klient/exceptions.py
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-05-31 09:15:58.340453 chatgpt_klient-0.7.2/src/chatgpt_klient.egg-info/
+-rw-r--r--   0 serpucga  (1000) serpucga  (1000)      219 2024-05-31 09:15:58.000000 chatgpt_klient-0.7.2/src/chatgpt_klient.egg-info/PKG-INFO
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)      376 2024-05-31 09:15:58.000000 chatgpt_klient-0.7.2/src/chatgpt_klient.egg-info/SOURCES.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)        1 2024-05-31 09:15:58.000000 chatgpt_klient-0.7.2/src/chatgpt_klient.egg-info/dependency_links.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       86 2024-05-31 09:15:58.000000 chatgpt_klient-0.7.2/src/chatgpt_klient.egg-info/requires.txt
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)       15 2024-05-31 09:15:58.000000 chatgpt_klient-0.7.2/src/chatgpt_klient.egg-info/top_level.txt
+drwxrwxr-x   0 serpucga  (1000) serpucga  (1000)        0 2024-05-31 09:15:58.340453 chatgpt_klient-0.7.2/tests/
+-rw-rw-r--   0 serpucga  (1000) serpucga  (1000)     1927 2024-05-31 08:51:15.000000 chatgpt_klient-0.7.2/tests/test_client.py
```

### Comparing `chatgpt_klient-0.6.1/src/chatgpt_klient/client.py` & `chatgpt_klient-0.7.2/src/chatgpt_klient/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,148 +1,159 @@
 import copy
 from openai import OpenAI, AzureOpenAI
 from openai import RateLimitError, APITimeoutError, BadRequestError
 import math
 import time
 import tiktoken
-import time
-from typing import Generator, Union, Literal
+from typing import Generator, Union, Literal, Dict
 from logutils import get_logger
 from chatgpt_klient.consts import (
     MAX_DELAY,
     ENGINES,
     DEFAULT_ENGINES,
     CLIENT_TIMEOUT,
     DEFAULT_AZURE_API_VERSION,
     DEFAULT_AZURE_ENDPOINT,
 )
 from chatgpt_klient.exceptions import (
-    InvalidAPIKeyError,
     InvalidModelError,
     InvalidResponseError,
 )
 from rich.console import Console
 
 logger = get_logger("chatgpt_client")
 console = Console()
 
 
-class ChatGPTPrompt:
+class LLMClient:
     def __init__(
         self,
         api_key,
-        engine="gpt3.5-default",
+        model: str | Dict = "gpt3.5-default",
         cap_tokens=math.inf,
         service: Literal["openai", "azure", "openai-compatible"] = "openai",
         azure_api_version: str = DEFAULT_AZURE_API_VERSION,
         azure_endpoint: str = DEFAULT_AZURE_ENDPOINT,
         azure_instance: str | None = None,
         openai_endpoint: str | None = None,
+        insecure_mode: bool = False,
     ):
+        # Initialize some attributes
         self.api_key = api_key
         self.service = service
+        self.msg_history = {"messages": [], "tokens": []}
+        self.last_prompt_tokens = 0
+        self.cap_tokens = cap_tokens
+        self.insecure_mode = insecure_mode
+        if isinstance(model, Dict):
+            self.model_name = model["name"]
+            model_definition = model
+        else:
+            self.model_name = model
+            if self.model_name in DEFAULT_ENGINES.keys():
+                self.model_name = DEFAULT_ENGINES[self.model_name]
+            for k, v in ENGINES.items():
+                if k == self.model_name:
+                    model_definition = v
+                    break
+            else:
+                if not self.insecure_mode:
+                    raise Exception(f"Model {self.model_name} not found")
+
+        if self.insecure_mode:
+            self.type = None
+            self.model_max_output_tokens = None
+            self.model_max_tokens = None
+        else:
+            self.type = model_definition["type"]
+            self.model_max_tokens = model_definition["max_tokens"]
+            if "max_output_tokens" in model_definition:
+                self.model_max_output_tokens = model_definition["max_output_tokens"]
+                self.max_tokens = self.model_max_tokens - self.model_max_output_tokens
+            else:
+                self.model_max_output_tokens = self.model_max_tokens
+                self.max_tokens = int(self.model_max_tokens / 2)
+
+            if service in ("openai", "azure"):
+                self.tokenizer = tiktoken.encoding_for_model(self.model_name)
+                self.encode = self.tokenizer.encode
+            else:
+                from transformers import AutoTokenizer
+                from huggingface_hub import login
+
+                try:
+                    login(model_definition["hf_token"])
+                    self.tokenizer = AutoTokenizer.from_pretrained(
+                        model_definition["base_model"]
+                    )
+                    self.encode = self.tokenizer.tokenize
+                except Exception:
+                    self.tokenizer = tiktoken.get_encoding(model_definition["encoding"])
+
+        self.azure_instance = None
+        if self.service == "azure":
+            if azure_instance is None:
+                raise NoAzureInstanceError("Azure API requires passing an instance")
+            self.model_name = azure_instance
+            self.azure_instance = azure_instance
+
+        # Initialize the OpenAI/Azure/OpenAI-compatible engine
         if self.service == "openai":
-            logger.info(f"Initializing an OpenAI {engine} engine")
+            logger.info(f"Initializing an OpenAI {self.model_name} engine")
             self.openai = OpenAI(api_key=self.api_key, timeout=CLIENT_TIMEOUT)
-        elif self.service == "openai-compatible":
-            logger.info(
-                f"Initializing an OpenAI-compatible {engine} engine with endpoint {openai_endpoint}"
-            )
-            self.openai = OpenAI(
-                api_key=self.api_key,
-                base_url=openai_endpoint,
-                timeout=CLIENT_TIMEOUT,
-            )
         elif self.service == "azure":
             if azure_instance is None:
                 raise NoAzureInstanceError
             logger.info(
-                f"Initializing an Azure connection to the {azure_instance} instance (model {engine})"
+                f"Initializing an Azure connection to the {azure_instance} instance (model {self.model_name})"
             )
             self.openai = AzureOpenAI(
-                api_key=api_key,
+                api_key=self.api_key,
                 api_version=azure_api_version,
                 azure_endpoint=azure_endpoint,
             )
-
-        self.msg_history = {"messages": [], "tokens": []}
-        self.last_prompt_tokens = 0
-        self.cap_tokens = cap_tokens
-        self.set_engine(engine, azure_instance)
-        self.check_api_key_validity()
-
-    def list_models(self):
-        return list(ENGINES.keys()) + list(DEFAULT_ENGINES.keys())
-
-    def check_api_key_validity(self):
-        try:
-            if self.service == "openai":
-                r = self.openai.completions.create(
-                    model="davinci-002",
-                    prompt="Hi",
-                    max_tokens=5,
-                ).model_dump()
-            elif self.service == "azure":
-                r = self.openai.chat.completions.create(
-                    model=self.engine,
-                    messages=[{"role": "user", "content": "Hola!"}],
-                    max_tokens=5,
-                    stream=False,
-                ).model_dump()
-            elif self.service == "openai-compatible":
-                r = self.openai.chat.completions.create(
-                    model="poligpt-light",
-                    messages=[{"role": "user", "content": "Hola!"}],
-                    max_tokens=5,
-                    stream=False,
-                ).model_dump()
-            r = self.check_response_validity(r)
-        except Exception:
-            logger.exception("Invalid API key.")
-            raise InvalidAPIKeyError(
-                "Your API key does not seem to be valid. Please check it."
+        elif self.service == "openai-compatible":
+            logger.info(
+                f"Initializing an OpenAI-compatible {self.model_name} engine with endpoint {openai_endpoint}"
             )
-        else:
-            logger.info("API key seems valid and working.")
+            self.openai = OpenAI(
+                api_key=self.api_key,
+                base_url=openai_endpoint,
+                timeout=CLIENT_TIMEOUT,
+            )
+
+        if not self.insecure_mode:
+            self.check_model_validity()
 
     def check_model_validity(self):
-        if self.real_engine not in self.list_models():
-            logger.error(f"Engine {self.real_engine} is not supported")
-            raise InvalidModelError(f"Engine {self.real_engine} not supported")
-        elif self.engine is None:
-            raise InvalidModelError("No engine instance")
         try:
-            if self.real_engine in [
-                k for k, v in ENGINES.items() if v["type"] == "legacy"
-            ]:
+            if self.type == "legacy":
                 r = self.openai.completions.create(
-                    model=self.engine,
+                    model=self.model_name,
                     prompt="Hi",
                     max_tokens=5,
                 ).model_dump()
                 r = self.check_response_validity(r)
-            elif self.real_engine in [
-                k for k, v in ENGINES.items() if v["type"] == "chat"
-            ]:
+            elif self.type == "chat":
                 r = self.openai.chat.completions.create(
-                    model=self.engine,
+                    model=self.model_name,
                     messages=[{"role": "user", "content": "Hi"}],
                     max_tokens=5,
                 ).model_dump()
                 r = self.check_response_validity(r)
                 logger.debug(
                     f'Model validity test: {r["choices"][0]["message"]["content"]}'
                 )
             else:
-                raise InvalidModelError(f"Engine {self.real_engine} not supported")
+                raise InvalidModelError(f"Engine {self.model_name} not supported")
         except Exception:
-            logger.exception(f"Invalid model ({self.engine}) for your API key")
-            raise InvalidModelError(f"Engine {self.engine} not supported")
+            logger.exception(f"Invalid model ({self.model_name}) for your API key")
+            raise InvalidModelError(f"Engine {self.model_name} not supported")
         else:
-            logger.info(f"Model ({self.engine}) seems to be valid.")
+            logger.info(f"Model ({self.model_name}) and API key seem to be valid.")
 
     def check_response_validity(self, r) -> dict:
         try:
             match r:
                 case {"choices": [{"text": str()}]}:
                     pass
                 case {"choices": [{"message": {"content": str()}}]}:
@@ -151,47 +162,23 @@
                     raise InvalidModelError
         except Exception:
             raise InvalidResponseError(f"Response is not well formed: {r}")
         else:
             logger.debug("Response seems to be well formed")
             return r
 
-    def set_engine(self, engine: str, azure_instance: str | None = None):
-        if engine in DEFAULT_ENGINES.keys():
-            self.real_engine = DEFAULT_ENGINES[engine]
-        else:
-            self.real_engine = engine
-        if self.service in ("openai", "openai-compatible"):
-            self.engine = self.real_engine
-            self.azure_instance = None
-        elif self.service == "azure":
-            if azure_instance is None:
-                raise NoAzureInstanceError("Azure API requires passing an instance")
-            self.engine = azure_instance
-            self.azure_instance = azure_instance
-        self.check_model_validity()
-        if self.service in ("openai", "azure"):
-            self.encoding = tiktoken.encoding_for_model(self.real_engine)
-        else:
-            self.encoding = tiktoken.get_encoding(ENGINES[self.real_engine]["encoding"])
-        eng_attrs = ENGINES[self.real_engine]
-        if "max_output_tokens" in eng_attrs:
-            self.max_tokens = eng_attrs["max_tokens"] - eng_attrs["max_output_tokens"]
-        else:
-            self.max_tokens = int(eng_attrs["max_tokens"] / 2)
-
     def set_system_directive(self, directive: str):
         self.clean_history(keep_sysdir=False)
         self.msg_history["messages"].append(
             {
                 "role": "system",
                 "content": directive,
             }
         )
-        self.msg_history["tokens"].append(len(self.encoding.encode(directive)))
+        self.msg_history["tokens"].append(len(self.tokenizer.encode(directive)))
 
     def clean_history(self, keep_sysdir=True):
         new_history = {"messages": [], "tokens": []}
         if keep_sysdir:
             for i, m in enumerate(self.msg_history["messages"]):
                 if m["role"] == "system":
                     new_history["messages"].append(
@@ -202,39 +189,33 @@
         self.last_prompt_tokens = 0
 
     def get_max_tokens_allowed(self):
         return (
             min(
                 [
                     self.max_tokens,
-                    ENGINES[self.real_engine]["max_tokens"],
+                    self.model_max_tokens or math.inf,
                     self.cap_tokens,
                 ]
             )
             - 10
         )
 
-    def get_max_output_tokens_allowed(self):
-        aux = math.inf
-        if "max_output_tokens" in ENGINES[self.real_engine]:
-            aux = ENGINES[self.real_engine]["max_output_tokens"]
-        return min(self.get_max_tokens_allowed(), aux)
-
     def calculate_prompt_tokens(self, text, no_history=True, keep_sysdir=False):
         aux_history = copy.deepcopy(self.msg_history)
         aux_last_prompt = self.last_prompt_tokens
         if no_history:
             self.clean_history(keep_sysdir=keep_sysdir)
         self.msg_history["messages"].append(
             {
                 "role": "user",
                 "content": text,
             }
         )
-        self.msg_history["tokens"].append(len(self.encoding.encode(text)))
+        self.msg_history["tokens"].append(len(self.tokenizer.encode(text)))
         potential_tokens = self.msg_history["tokens"][-1] + self.last_prompt_tokens
         self.msg_history = aux_history
         self.last_prompt_tokens = aux_last_prompt
         return potential_tokens
 
     def send_prompt(
         self, text: str, no_history: bool = False, stream: bool = False
@@ -250,49 +231,50 @@
         :param stream: set to True to return the generated tokens synchronously, one
           by one as we receive them from ChatGPT. Otherwise, the text will be returned
           as a whole once it is ready.
         :returns: either a string with the whole text, or a generator of the tokens
           composing the text
         """
         response = "No response"
-        if self.real_engine in [k for k, v in ENGINES.items() if v["type"] == "legacy"]:
+        if self.type == "legacy":
             r = self.openai.completions.create(
-                model=self.engine,
+                model=self.model_name,
                 prompt=text,
-                max_tokens=self.get_max_output_tokens_allowed(),
+                max_tokens=self.model_max_output_tokens,
             ).model_dump()
             r = self.check_response_validity(r)
             response = r["choices"][0]["text"]
-        elif self.real_engine in [k for k, v in ENGINES.items() if v["type"] == "chat"]:
+        elif self.type == "chat" or (self.type is None and self.insecure_mode):
             if no_history:
                 self.clean_history()
             self.msg_history["messages"].append(
                 {
                     "role": "user",
                     "content": text,
                 }
             )
-            self.msg_history["tokens"].append(len(self.encoding.encode(text)))
-            self.reduce_msg_history(text)
+            if not self.insecure_mode:
+                self.msg_history["tokens"].append(len(self.tokenizer.encode(text)))
+                self.reduce_msg_history(text)
             if stream:
                 return self.chat_completion_stream(text)
             else:
                 return self.chat_completion_no_stream(text)
         else:
-            logger.warning(f"Engine {self.engine} not supported")
+            logger.warning(f"Engine {self.model_name} not supported")
         return response
 
     def interactive_prompt(self, system_directive: str | None = None):
         if system_directive:
             self.set_system_directive(system_directive)
         console.print("###########", style="bold")
         console.print("# ChatGPT #", style="bold")
         console.print("###########", style="bold")
         console.print(
-            f"[bold yellow]Engine:[/bold yellow] {self.engine}", highlight=False
+            f"[bold yellow]Engine:[/bold yellow] {self.model_name}", highlight=False
         )
         console.print("[bold cyan]Enter 'q'/'quit' to exit the chat[/]")
         console.print("[bold cyan]Enter anything to start chatting.[/]")
         console.print()
         while True:
             input_text = input("$ ")
             if input_text in ("q", "quit"):
@@ -333,31 +315,34 @@
             raise TooManyTokensError(
                 f"The maximum accepted tokens ({self.get_max_tokens_allowed()}) is not big enough to process your prompt"
             )
 
     def chat_completion_no_stream(self, text: str, delay: int = 5) -> str:
         try:
             r = self.openai.chat.completions.create(
-                model=self.engine,
+                model=self.model_name,
                 messages=self.msg_history["messages"],
-                max_tokens=self.get_max_output_tokens_allowed(),
+                max_tokens=self.model_max_output_tokens,
                 stream=False,
             ).model_dump()
             logger.debug(r)
             r = self.check_response_validity(r)
             self.last_prompt_tokens = r["usage"]["total_tokens"]
             response = r["choices"][0]["message"]["content"]
             if response:
                 self.msg_history["messages"].append(
                     {
                         "role": "assistant",
                         "content": response,
                     }
                 )
-                self.msg_history["tokens"].append(len(self.encoding.encode(response)))
+                if not self.insecure_mode:
+                    self.msg_history["tokens"].append(
+                        len(self.tokenizer.encode(response))
+                    )
         except RateLimitError:
             logger.warning(f"Rate limit reached, delaying request {delay} seconds")
             if delay > MAX_DELAY:
                 raise Exception(
                     "Recurring RateLimitError and delaying requests not working"
                 )
             time.sleep(delay)
@@ -379,17 +364,17 @@
             return response
 
     def chat_completion_stream(
         self, text: str, delay: int = 5
     ) -> Generator[str, None, None]:
         try:
             stream = self.openai.chat.completions.create(
-                model=self.engine,
+                model=self.model_name,
                 messages=self.msg_history["messages"],
-                max_tokens=self.get_max_output_tokens_allowed(),
+                max_tokens=self.model_max_output_tokens,
                 stream=True,
             )
             aux_num_tokens = 0
             aux_text = ""
             for r in stream:
                 match chunk := r.choices[0].model_dump():
                     case {"finish_reason": "stop"}:
@@ -404,15 +389,16 @@
             self.last_prompt_tokens = aux_num_tokens
             self.msg_history["messages"].append(
                 {
                     "role": "assistant",
                     "content": aux_text,
                 }
             )
-            self.msg_history["tokens"].append(len(self.encoding.encode(aux_text)))
+            if not self.insecure_mode:
+                self.msg_history["tokens"].append(len(self.tokenizer.encode(aux_text)))
         except RateLimitError:
             logger.warning(f"Rate limit reached, delaying request {delay} seconds")
             if delay > MAX_DELAY:
                 raise Exception(
                     "Recurring RateLimitError and delaying requests not working"
                 )
             time.sleep(delay)
```

### Comparing `chatgpt_klient-0.6.1/src/chatgpt_klient/consts.py` & `chatgpt_klient-0.7.2/src/chatgpt_klient/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,7 +84,11 @@
 }
 
 MAX_DELAY = 500
 CLIENT_TIMEOUT = 300
 DEFAULT_AZURE_API_VERSION = "2023-05-15"
 DEFAULT_AZURE_ENDPOINT = "https://azureaistudio-swedencentral.openai.azure.com/"
 DEFAULT_AZURE_ENGINE = DEFAULT_ENGINES["gpt3.5-default"]
+
+OPENAI_LIGHT_MODEL = "gpt-3.5-turbo-0125"
+
+DEFAULT_MAX_TOKENS = 65535
```

