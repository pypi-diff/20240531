# Comparing `tmp/lavague_core-0.2.1.tar.gz` & `tmp/lavague_core-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_core-0.2.1.tar", max compression
+gzip compressed data, was "lavague_core-0.2.2.tar", max compression
```

## Comparing `lavague_core-0.2.1.tar` & `lavague_core-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11357 2024-05-28 08:59:04.851483 lavague_core-0.2.1/LICENSE
--rw-r--r--   0        0        0        0 2024-05-28 08:59:04.851521 lavague_core-0.2.1/README.md
--rw-r--r--   0        0        0     1065 2024-05-31 07:36:10.823075 lavague_core-0.2.1/lavague/core/__init__.py
--rw-r--r--   0        0        0     5532 2024-05-31 07:36:10.823398 lavague_core-0.2.1/lavague/core/action_engine.py
--rw-r--r--   0        0        0      374 2024-05-28 08:59:04.852005 lavague_core-0.2.1/lavague/core/action_template.py
--rw-r--r--   0        0        0     2839 2024-05-31 07:36:10.823600 lavague_core-0.2.1/lavague/core/agents.py
--rw-r--r--   0        0        0     3084 2024-05-28 21:01:47.304939 lavague_core-0.2.1/lavague/core/base_driver.py
--rw-r--r--   0        0        0      248 2024-05-31 07:36:10.823728 lavague_core-0.2.1/lavague/core/base_engine.py
--rw-r--r--   0        0        0     1189 2024-05-29 15:40:38.733494 lavague_core-0.2.1/lavague/core/context.py
--rw-r--r--   0        0        0     1296 2024-05-28 08:59:04.852453 lavague_core-0.2.1/lavague/core/extractors.py
--rw-r--r--   0        0        0     1282 2024-05-28 21:01:47.305109 lavague_core-0.2.1/lavague/core/logger.py
--rw-r--r--   0        0        0     1710 2024-05-28 21:01:47.305326 lavague_core-0.2.1/lavague/core/memory.py
--rw-r--r--   0        0        0    12742 2024-05-31 07:36:10.824052 lavague_core-0.2.1/lavague/core/navigation.py
--rw-r--r--   0        0        0     3535 2024-05-31 07:36:10.824535 lavague_core-0.2.1/lavague/core/python_engine.py
--rw-r--r--   0        0        0    12117 2024-05-28 08:59:04.852935 lavague_core-0.2.1/lavague/core/retrievers.py
--rw-r--r--   0        0        0     1795 2024-05-28 08:59:04.853008 lavague_core-0.2.1/lavague/core/rewriter.py
--rw-r--r--   0        0        0     5661 2024-05-30 07:35:09.668782 lavague_core-0.2.1/lavague/core/utilities/format_utils.py
--rw-r--r--   0        0        0     2056 2024-05-30 07:35:09.669367 lavague_core-0.2.1/lavague/core/utilities/telemetry.py
--rw-r--r--   0        0        0     1430 2024-05-28 08:59:53.819092 lavague_core-0.2.1/lavague/core/utilities/version_checker.py
--rw-r--r--   0        0        0     3402 2024-05-28 21:01:47.306593 lavague_core-0.2.1/lavague/core/utilities/web_utils.py
--rw-r--r--   0        0        0    15081 2024-05-28 21:01:47.306918 lavague_core-0.2.1/lavague/core/world_model.py
--rw-r--r--   0        0        0     1128 2024-05-31 07:37:01.231566 lavague_core-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1387 1970-01-01 00:00:00.000000 lavague_core-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 08:59:04.851483 lavague_core-0.2.2/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-28 08:59:04.851521 lavague_core-0.2.2/README.md
+-rw-r--r--   0        0        0     1065 2024-05-31 09:04:25.699400 lavague_core-0.2.2/lavague/core/__init__.py
+-rw-r--r--   0        0        0     5639 2024-05-31 09:22:12.315340 lavague_core-0.2.2/lavague/core/action_engine.py
+-rw-r--r--   0        0        0      374 2024-05-28 08:59:04.852005 lavague_core-0.2.2/lavague/core/action_template.py
+-rw-r--r--   0        0        0     2839 2024-05-31 09:13:21.375968 lavague_core-0.2.2/lavague/core/agents.py
+-rw-r--r--   0        0        0     3084 2024-05-31 09:04:25.700281 lavague_core-0.2.2/lavague/core/base_driver.py
+-rw-r--r--   0        0        0      248 2024-05-31 09:04:25.700517 lavague_core-0.2.2/lavague/core/base_engine.py
+-rw-r--r--   0        0        0     1189 2024-05-29 15:40:38.733494 lavague_core-0.2.2/lavague/core/context.py
+-rw-r--r--   0        0        0     1296 2024-05-28 08:59:04.852453 lavague_core-0.2.2/lavague/core/extractors.py
+-rw-r--r--   0        0        0     1282 2024-05-31 09:04:25.700605 lavague_core-0.2.2/lavague/core/logger.py
+-rw-r--r--   0        0        0     1710 2024-05-31 09:04:25.700831 lavague_core-0.2.2/lavague/core/memory.py
+-rw-r--r--   0        0        0    12884 2024-05-31 09:22:47.918942 lavague_core-0.2.2/lavague/core/navigation.py
+-rw-r--r--   0        0        0     3641 2024-05-31 09:09:03.128947 lavague_core-0.2.2/lavague/core/python_engine.py
+-rw-r--r--   0        0        0    12117 2024-05-28 08:59:04.852935 lavague_core-0.2.2/lavague/core/retrievers.py
+-rw-r--r--   0        0        0     1795 2024-05-28 08:59:04.853008 lavague_core-0.2.2/lavague/core/rewriter.py
+-rw-r--r--   0        0        0     5661 2024-05-31 09:04:25.701914 lavague_core-0.2.2/lavague/core/utilities/format_utils.py
+-rw-r--r--   0        0        0     2056 2024-05-31 09:04:25.702490 lavague_core-0.2.2/lavague/core/utilities/telemetry.py
+-rw-r--r--   0        0        0     1430 2024-05-31 09:04:25.702632 lavague_core-0.2.2/lavague/core/utilities/version_checker.py
+-rw-r--r--   0        0        0     3402 2024-05-31 09:04:25.702910 lavague_core-0.2.2/lavague/core/utilities/web_utils.py
+-rw-r--r--   0        0        0    15134 2024-05-31 09:09:25.856069 lavague_core-0.2.2/lavague/core/world_model.py
+-rw-r--r--   0        0        0     1128 2024-05-31 09:22:54.991300 lavague_core-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1387 1970-01-01 00:00:00.000000 lavague_core-0.2.2/PKG-INFO
```

### Comparing `lavague_core-0.2.1/LICENSE` & `lavague_core-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.1/lavague/core/__init__.py` & `lavague_core-0.2.2/lavague/core/__init__.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.1/lavague/core/action_engine.py` & `lavague_core-0.2.2/lavague/core/action_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,26 +44,32 @@
 
     def __init__(
         self,
         driver: BaseDriver,
         navigation_engine: "BaseEngine" = None,
         python_engine: "BaseEngine" = None,
         navigation_control: "BaseEngine" = None,
-        llm: BaseLLM = get_default_context().llm,
-        embedding: BaseEmbedding = get_default_context().embedding,
+        llm: BaseLLM = None,
+        embedding: BaseEmbedding = None,
         retriever: BaseHtmlRetriever = OpsmSplitRetriever(),
         prompt_template: PromptTemplate = NAVIGATION_ENGINE_PROMPT_TEMPLATE.prompt_template,
         extractor: BaseExtractor = NAVIGATION_ENGINE_PROMPT_TEMPLATE.extractor,
         time_between_actions: float = 1.5,
         n_attempts: int = 5,
         logger: AgentLogger = None,
     ):
         from lavague.core.navigation import NavigationControl, NavigationEngine
         from lavague.core.python_engine import PythonEngine
 
+        if llm is None:
+            llm = get_default_context().llm
+
+        if embedding is None:
+            embedding = get_default_context().embedding
+
         self.driver = driver
         if navigation_engine is None:
             navigation_engine = NavigationEngine(
                 driver,
                 llm,
                 embedding,
                 retriever,
@@ -115,15 +121,15 @@
 
     def set_display(self, display: bool):
         self.navigation_engine.set_display(display)
         self.python_engine.set_display(display)
         self.navigation_control.set_display(display)
 
     def set_logger_all(self, logger: AgentLogger):
-        self.navigation_control.set_logger(logger)
+        self.navigation_engine.set_logger(logger)
         self.python_engine.set_logger(logger)
         self.navigation_control.set_logger(logger)
 
     def dispatch_instruction(self, next_engine_name: str, instruction: str):
         """
         Dispatch the instruction to the appropriate ActionEngine
```

### Comparing `lavague_core-0.2.1/lavague/core/agents.py` & `lavague_core-0.2.2/lavague/core/agents.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.1/lavague/core/base_driver.py` & `lavague_core-0.2.2/lavague/core/base_driver.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.1/lavague/core/context.py` & `lavague_core-0.2.2/lavague/core/context.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.1/lavague/core/extractors.py` & `lavague_core-0.2.2/lavague/core/extractors.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.1/lavague/core/logger.py` & `lavague_core-0.2.2/lavague/core/logger.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.1/lavague/core/memory.py` & `lavague_core-0.2.2/lavague/core/memory.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.1/lavague/core/navigation.py` & `lavague_core-0.2.2/lavague/core/navigation.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,24 +60,28 @@
         logger: (`AgentLogger`)
             Logger to log the actions taken by the agent
     """
 
     def __init__(
         self,
         driver: BaseDriver,
-        llm: BaseLLM = get_default_context().llm,
-        embedding: BaseEmbedding = get_default_context().embedding,
+        llm: BaseLLM = None,
+        embedding: BaseEmbedding = None,
         retriever: BaseHtmlRetriever = OpsmSplitRetriever(),
         prompt_template: PromptTemplate = NAVIGATION_ENGINE_PROMPT_TEMPLATE.prompt_template,
         extractor: BaseExtractor = NAVIGATION_ENGINE_PROMPT_TEMPLATE.extractor,
         time_between_actions: float = 1.5,
         n_attempts: int = 5,
         logger: AgentLogger = None,
         display: bool = False,
     ):
+        if llm is None: 
+            llm: BaseLLM = get_default_context().llm,
+        if embedding is None:
+            embedding: BaseEmbedding = get_default_context().embedding,
         self.driver: BaseDriver = driver
         self.llm: BaseLLM = llm
         self.embedding: BaseEmbedding = embedding
         self.retriever: BaseHtmlRetriever = retriever
         self.prompt_template: PromptTemplate = prompt_template.partial_format(
             driver_capability=driver.get_capability()
         )
@@ -190,26 +194,27 @@
         Return:
             `bool`: True if the code was executed without error
             `Any`: The output of the code
         """
 
         # Navigation has no output
 
+
         output = None
         driver = self.driver.get_driver()
 
         start = time.time()
         source_nodes = self.get_nodes(instruction)
         end = time.time()
         retrieval_time = end - start
 
         llm_context = "\n".join(source_nodes)
         success = False
         logger = self.logger
-
+        
         navigation_log = {
             "navigation_engine_input": instruction,
             "retrieved_html": source_nodes,
             "retrieval_time": retrieval_time,
             "retrieval_name": self.retriever.__class__.__name__,
         }
```

### Comparing `lavague_core-0.2.1/lavague/core/python_engine.py` & `lavague_core-0.2.2/lavague/core/python_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,18 +24,22 @@
     embedding: BaseEmbedding
     # TODO: Design question: should we have a driver available to Python engine?
     driver: BaseDriver
 
     def __init__(
         self,
         driver: BaseDriver,
-        llm: BaseLLM = get_default_context().llm,
-        embedding: BaseEmbedding = get_default_context().embedding,
+        llm: BaseLLM = None,
+        embedding: BaseEmbedding = None,
         logger: AgentLogger = None,
     ):
+        if llm is None:
+            llm = get_default_context().llm
+        if embedding is None:
+            embedding = get_default_context().embedding
         self.llm = llm
         self.embedding = embedding
         self.driver = driver
         self.logger = logger
         self.display = False
 
     @classmethod
```

### Comparing `lavague_core-0.2.1/lavague/core/retrievers.py` & `lavague_core-0.2.2/lavague/core/retrievers.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.1/lavague/core/rewriter.py` & `lavague_core-0.2.2/lavague/core/rewriter.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.1/lavague/core/utilities/format_utils.py` & `lavague_core-0.2.2/lavague/core/utilities/format_utils.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.1/lavague/core/utilities/telemetry.py` & `lavague_core-0.2.2/lavague/core/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.1/lavague/core/utilities/version_checker.py` & `lavague_core-0.2.2/lavague/core/utilities/version_checker.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.1/lavague/core/utilities/web_utils.py` & `lavague_core-0.2.2/lavague/core/utilities/web_utils.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.1/lavague/core/world_model.py` & `lavague_core-0.2.2/lavague/core/world_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,19 +283,21 @@
 
 
 class WorldModel(ABC, Loggable):
     """Abstract class for WorldModel"""
 
     def __init__(
         self,
-        mm_llm: MultiModalLLM = get_default_context().mm_llm,
+        mm_llm: MultiModalLLM = None,
         prompt_template: PromptTemplate = WORLD_MODEL_PROMPT_TEMPLATE,
         examples: str = WORLD_MODEL_GENERAL_EXAMPLES,
         logger: AgentLogger = None,
     ):
+        if mm_llm is None:
+            mm_llm = get_default_context().mm_llm
         self.mm_llm: MultiModalLLM = mm_llm
         self.prompt_template: PromptTemplate = prompt_template.partial_format(
             examples=examples
         )
         self.logger: AgentLogger = logger
 
     @classmethod
```

### Comparing `lavague_core-0.2.1/pyproject.toml` & `lavague_core-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry]
 name = "lavague-core"
-version = "0.2.1"
+version = "0.2.2"
 description = "automation code generation from text instructions"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_core-0.2.1/PKG-INFO` & `lavague_core-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-core
-Version: 0.2.1
+Version: 0.2.2
 Summary: automation code generation from text instructions
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

