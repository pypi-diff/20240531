# Comparing `tmp/lavague_core-0.2.0.tar.gz` & `tmp/lavague_core-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_core-0.2.0.tar", max compression
+gzip compressed data, was "lavague_core-0.2.1.tar", max compression
```

## Comparing `lavague_core-0.2.0.tar` & `lavague_core-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0    11357 2024-05-28 08:59:04.851483 lavague_core-0.2.0/LICENSE
--rw-r--r--   0        0        0        0 2024-05-28 08:59:04.851521 lavague_core-0.2.0/README.md
--rw-r--r--   0        0        0     1024 2024-05-28 12:06:21.695244 lavague_core-0.2.0/lavague/core/__init__.py
--rw-r--r--   0        0        0    12046 2024-05-28 14:04:20.124802 lavague_core-0.2.0/lavague/core/action_engine.py
--rw-r--r--   0        0        0      374 2024-05-28 08:59:04.852005 lavague_core-0.2.0/lavague/core/action_template.py
--rw-r--r--   0        0        0     2968 2024-05-28 13:56:49.816867 lavague_core-0.2.0/lavague/core/agents.py
--rw-r--r--   0        0        0     3084 2024-05-28 13:56:49.816457 lavague_core-0.2.0/lavague/core/base_driver.py
--rw-r--r--   0        0        0     1189 2024-05-28 08:59:04.852328 lavague_core-0.2.0/lavague/core/context.py
--rw-r--r--   0        0        0     1296 2024-05-28 08:59:04.852453 lavague_core-0.2.0/lavague/core/extractors.py
--rw-r--r--   0        0        0     1282 2024-05-28 09:27:09.045035 lavague_core-0.2.0/lavague/core/logger.py
--rw-r--r--   0        0        0     1710 2024-05-28 12:30:55.080478 lavague_core-0.2.0/lavague/core/memory.py
--rw-r--r--   0        0        0     2978 2024-05-28 13:56:49.816753 lavague_core-0.2.0/lavague/core/navigation.py
--rw-r--r--   0        0        0     3549 2024-05-28 13:56:49.816563 lavague_core-0.2.0/lavague/core/python_engine.py
--rw-r--r--   0        0        0    12117 2024-05-28 08:59:04.852935 lavague_core-0.2.0/lavague/core/retrievers.py
--rw-r--r--   0        0        0     1795 2024-05-28 08:59:04.853008 lavague_core-0.2.0/lavague/core/rewriter.py
--rw-r--r--   0        0        0     5661 2024-05-28 10:20:06.031839 lavague_core-0.2.0/lavague/core/utilities/format_utils.py
--rw-r--r--   0        0        0     2056 2024-05-28 11:59:38.835586 lavague_core-0.2.0/lavague/core/utilities/telemetry.py
--rw-r--r--   0        0        0     1430 2024-05-28 08:59:53.819092 lavague_core-0.2.0/lavague/core/utilities/version_checker.py
--rw-r--r--   0        0        0     3402 2024-05-28 13:56:49.817106 lavague_core-0.2.0/lavague/core/utilities/web_utils.py
--rw-r--r--   0        0        0    15081 2024-05-28 13:56:49.816764 lavague_core-0.2.0/lavague/core/world_model.py
--rw-r--r--   0        0        0     1128 2024-05-28 20:57:30.162718 lavague_core-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1387 1970-01-01 00:00:00.000000 lavague_core-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 08:59:04.851483 lavague_core-0.2.1/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-28 08:59:04.851521 lavague_core-0.2.1/README.md
+-rw-r--r--   0        0        0     1065 2024-05-31 07:36:10.823075 lavague_core-0.2.1/lavague/core/__init__.py
+-rw-r--r--   0        0        0     5532 2024-05-31 07:36:10.823398 lavague_core-0.2.1/lavague/core/action_engine.py
+-rw-r--r--   0        0        0      374 2024-05-28 08:59:04.852005 lavague_core-0.2.1/lavague/core/action_template.py
+-rw-r--r--   0        0        0     2839 2024-05-31 07:36:10.823600 lavague_core-0.2.1/lavague/core/agents.py
+-rw-r--r--   0        0        0     3084 2024-05-28 21:01:47.304939 lavague_core-0.2.1/lavague/core/base_driver.py
+-rw-r--r--   0        0        0      248 2024-05-31 07:36:10.823728 lavague_core-0.2.1/lavague/core/base_engine.py
+-rw-r--r--   0        0        0     1189 2024-05-29 15:40:38.733494 lavague_core-0.2.1/lavague/core/context.py
+-rw-r--r--   0        0        0     1296 2024-05-28 08:59:04.852453 lavague_core-0.2.1/lavague/core/extractors.py
+-rw-r--r--   0        0        0     1282 2024-05-28 21:01:47.305109 lavague_core-0.2.1/lavague/core/logger.py
+-rw-r--r--   0        0        0     1710 2024-05-28 21:01:47.305326 lavague_core-0.2.1/lavague/core/memory.py
+-rw-r--r--   0        0        0    12742 2024-05-31 07:36:10.824052 lavague_core-0.2.1/lavague/core/navigation.py
+-rw-r--r--   0        0        0     3535 2024-05-31 07:36:10.824535 lavague_core-0.2.1/lavague/core/python_engine.py
+-rw-r--r--   0        0        0    12117 2024-05-28 08:59:04.852935 lavague_core-0.2.1/lavague/core/retrievers.py
+-rw-r--r--   0        0        0     1795 2024-05-28 08:59:04.853008 lavague_core-0.2.1/lavague/core/rewriter.py
+-rw-r--r--   0        0        0     5661 2024-05-30 07:35:09.668782 lavague_core-0.2.1/lavague/core/utilities/format_utils.py
+-rw-r--r--   0        0        0     2056 2024-05-30 07:35:09.669367 lavague_core-0.2.1/lavague/core/utilities/telemetry.py
+-rw-r--r--   0        0        0     1430 2024-05-28 08:59:53.819092 lavague_core-0.2.1/lavague/core/utilities/version_checker.py
+-rw-r--r--   0        0        0     3402 2024-05-28 21:01:47.306593 lavague_core-0.2.1/lavague/core/utilities/web_utils.py
+-rw-r--r--   0        0        0    15081 2024-05-28 21:01:47.306918 lavague_core-0.2.1/lavague/core/world_model.py
+-rw-r--r--   0        0        0     1128 2024-05-31 07:37:01.231566 lavague_core-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1387 1970-01-01 00:00:00.000000 lavague_core-0.2.1/PKG-INFO
```

### Comparing `lavague_core-0.2.0/LICENSE` & `lavague_core-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.0/lavague/core/__init__.py` & `lavague_core-0.2.1/lavague/core/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from lavague.core.python_engine import PythonEngine
 from lavague.core.context import Context, get_default_context
 from lavague.core.extractors import PythonFromMarkdownExtractor
 from lavague.core.retrievers import OpsmSplitRetriever
 from lavague.core.world_model import WorldModel
 from lavague.core.utilities.version_checker import check_latest_version
 from lavague.core.action_engine import ActionEngine
+from lavague.core.agents import WebAgent
 
 import os
 import warnings
 
 
 def telemetry_warning():
     telemetry_var = os.getenv("TELEMETRY_VAR")
```

### Comparing `lavague_core-0.2.0/lavague/core/action_engine.py` & `lavague_core-0.2.1/lavague/core/navigation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from __future__ import annotations
-from abc import ABC, abstractmethod
 from io import BytesIO
-from typing import Any, Dict, Optional, Generator, List, Tuple
-from llama_index.core.query_engine import RetrieverQueryEngine
-from llama_index.core import get_response_synthesizer, QueryBundle, PromptTemplate
-from llama_index.core.base.llms.base import BaseLLM
-from llama_index.core.base.embeddings.base import BaseEmbedding
-from lavague.core.extractors import BaseExtractor, PythonFromMarkdownExtractor
-from lavague.core.retrievers import BaseHtmlRetriever, OpsmSplitRetriever
-from lavague.core.base_driver import BaseDriver
+import time
+from typing import Any, List, Optional, Tuple
 from lavague.core.action_template import ActionTemplate
 from lavague.core.context import Context, get_default_context
-import time
-from PIL import Image
-from lavague.core.logger import AgentLogger, Loggable
+from lavague.core.extractors import BaseExtractor, PythonFromMarkdownExtractor
+from lavague.core.retrievers import BaseHtmlRetriever, OpsmSplitRetriever
 from lavague.core.utilities.web_utils import (
     display_screenshot,
     get_highlighted_element,
     sort_files_by_creation,
 )
+from selenium.webdriver.remote.webdriver import WebDriver
+from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.common.by import By
+from lavague.core.logger import AgentLogger
+from llama_index.core.base.embeddings.base import BaseEmbedding
+from lavague.core.base_engine import BaseEngine
+from lavague.core.base_driver import BaseDriver
+from llama_index.core import get_response_synthesizer, QueryBundle, PromptTemplate
+from PIL import Image
+from llama_index.core.base.llms.base import BaseLLM
+from llama_index.core.query_engine import RetrieverQueryEngine
 
-ACTION_ENGINE_PROMPT_TEMPLATE = ActionTemplate(
+NAVIGATION_ENGINE_PROMPT_TEMPLATE = ActionTemplate(
     """
 {driver_capability}
 
 Here is a the next example to answer:
 
 HTML:
 {context_str}
@@ -32,31 +34,21 @@
 Completion:
 
 """,
     PythonFromMarkdownExtractor(),
 )
 
 
-class BaseActionEngine(ABC, Loggable):
-    @abstractmethod
-    def execute_instruction(self, instruction: str) -> Tuple[bool, Any]:
-        pass
-
-
-class ActionEngine(BaseActionEngine):
+class NavigationEngine(BaseEngine):
     """
-    ActionEngine leverages the llm model and the embedding model to output code from the prompt and the html page.
+    NavigationEngine leverages the llm model and the embedding model to output code from the prompt and the html page.
 
     Args:
         driver (`BaseDriver`):
             The Web driver used to interact with the headless browser
-        python_engine (`BaseActionEngine`)
-            Python Engine for generating code that doesn't interact with an html page.
-        navigation_control (`BaseActionEngine`)
-            Navigation Control
         llm (`BaseLLM`)
             llama-index LLM that will generate the action
         embedding (`BaseEmbedding`)
             llama-index Embedding model
         retriever (`BaseHtmlRetriever`)
             Specify which algorithm will be used for RAG
         prompt_template (`PromptTemplate`)
@@ -68,71 +60,51 @@
         logger: (`AgentLogger`)
             Logger to log the actions taken by the agent
     """
 
     def __init__(
         self,
         driver: BaseDriver,
-        python_engine: "BaseActionEngine" = None,
-        navigation_control: "BaseActionEngine" = None,
         llm: BaseLLM = get_default_context().llm,
         embedding: BaseEmbedding = get_default_context().embedding,
         retriever: BaseHtmlRetriever = OpsmSplitRetriever(),
-        prompt_template: PromptTemplate = ACTION_ENGINE_PROMPT_TEMPLATE.prompt_template,
-        extractor: BaseExtractor = ACTION_ENGINE_PROMPT_TEMPLATE.extractor,
+        prompt_template: PromptTemplate = NAVIGATION_ENGINE_PROMPT_TEMPLATE.prompt_template,
+        extractor: BaseExtractor = NAVIGATION_ENGINE_PROMPT_TEMPLATE.extractor,
         time_between_actions: float = 1.5,
         n_attempts: int = 5,
         logger: AgentLogger = None,
         display: bool = False,
     ):
-        from lavague.core.navigation import NavigationControl
-        from lavague.core.python_engine import PythonEngine
-
         self.driver: BaseDriver = driver
         self.llm: BaseLLM = llm
         self.embedding: BaseEmbedding = embedding
         self.retriever: BaseHtmlRetriever = retriever
         self.prompt_template: PromptTemplate = prompt_template.partial_format(
             driver_capability=driver.get_capability()
         )
         self.extractor: BaseExtractor = extractor
         self.time_between_actions = time_between_actions
         self.logger = logger
         self.n_attempts = n_attempts
-        if python_engine is None:
-            python_engine = PythonEngine(self.driver, llm, embedding)
-        if navigation_control is None:
-            navigation_control = NavigationControl(self.driver)
-        self.python_engine = python_engine
-        self.navigation_control = navigation_control
-        self.engines: Dict[str, BaseActionEngine] = {
-            "Navigation Engine": self,
-            "Python Engine": self.python_engine,
-            "Navigation Controls": self.navigation_control,
-        }
         self.display = display
 
     @classmethod
     def from_context(
         cls,
         context: Context,
         driver: BaseDriver,
-        python_engine: BaseActionEngine = None,
-        navigation_control: BaseActionEngine = None,
         retriever: BaseHtmlRetriever = OpsmSplitRetriever(),
-        prompt_template: PromptTemplate = ACTION_ENGINE_PROMPT_TEMPLATE.prompt_template,
-        extractor: BaseExtractor = ACTION_ENGINE_PROMPT_TEMPLATE.extractor,
-    ) -> ActionEngine:
+        prompt_template: PromptTemplate = NAVIGATION_ENGINE_PROMPT_TEMPLATE.prompt_template,
+        extractor: BaseExtractor = NAVIGATION_ENGINE_PROMPT_TEMPLATE.extractor,
+    ) -> "NavigationEngine":
         """
-        Create an ActionEngine from a context
+        Create an NavigationEngine from a context
         """
         return cls(
             driver,
-            python_engine,
-            navigation_control,
             context.llm,
             context.embedding,
             retriever,
             prompt_template,
             extractor,
         )
 
@@ -188,19 +160,14 @@
         response = self.llm.complete(prompt).text
         code = self.extractor.extract(response)
         return code
 
     def set_display(self, display: bool):
         self.display = display
 
-    def set_logger_all(self, logger: AgentLogger):
-        self.set_logger(logger)
-        self.python_engine.set_logger(logger)
-        self.navigation_control.set_logger(logger)
-
     def get_action(self, query: str) -> Optional[str]:
         # TODO: Rename query to instruction to be consistent with other engines
         """
         Generate the code from a query
 
         Args:
             query (`str`): Instructions given at the end of the prompt to tell the model what to do on the html page
@@ -209,30 +176,14 @@
             `str`: The generated code
         """
         query_engine = self._get_query_engine(streaming=False)
         response = query_engine.query(query)
         code = response.response
         return self.extractor.extract(code)
 
-    def dispatch_instruction(self, next_engine_name: str, instruction: str):
-        """
-        Dispatch the instruction to the appropriate ActionEngine
-
-        Args:
-            next_engine_name (`str`): The name of the engine to call
-            instruction (`str`): The instruction to perform
-
-        Return:
-            `bool`: True if the code was executed without error
-            `Any`: The output of the code
-        """
-
-        next_engine = self.engines[next_engine_name]
-        return next_engine.execute_instruction(instruction)
-
     def execute_instruction(self, instruction: str) -> Tuple[bool, Any]:
         """
         Generates code and executes it to answer the instruction
 
         Args:
             instruction (`str`): The instruction to perform
 
@@ -334,14 +285,90 @@
             }
 
             logger.add_log(log)
 
         return success, output
 
 
+class NavigationControl(BaseEngine):
+    driver: BaseDriver
+    time_between_actions: float
+    logger: AgentLogger
+
+    def __init__(
+        self,
+        driver: BaseDriver,
+        time_between_actions: float = 1.5,
+        logger: AgentLogger = None,
+    ) -> None:
+        self.driver: BaseDriver = driver
+        self.time_between_actions = time_between_actions
+        self.logger = logger
+        self.display = False
+
+    def set_display(self, display: bool):
+        self.display = display
+
+    def execute_instruction(self, instruction: str):
+        logger = self.logger
+        # TODO: Not clean the fact that we have driver / meta_driver around. Should settle for better names
+        meta_driver: BaseDriver = self.driver
+        driver: WebDriver = meta_driver.get_driver()
+        display_page = False
+
+        if "SCROLL_DOWN" in instruction:
+            code = (
+                """driver.execute_script("window.scrollBy(0, window.innerHeight);")"""
+            )
+        elif "SCROLL_UP" in instruction:
+            code = (
+                """driver.execute_script("window.scrollBy(0, -window.innerHeight);")"""
+            )
+        elif "WAIT" in instruction:
+            code = f"""
+import time
+time.sleep({self.time_between_actions})"""
+        elif "BACK" in instruction:
+            code = """driver.back()"""
+        elif "SCAN" in instruction:
+            # TODO: Should scan be in the navigation controls or in the driver?
+            code = """meta_driver.get_screenshots_whole_page()"""
+            display_page = True
+        else:
+            raise ValueError(f"Unknown instruction: {instruction}")
+
+        local_scope = {"driver": driver, "meta_driver": meta_driver}
+        exec(code, local_scope, local_scope)
+        if display_page and self.display:
+            try:
+                scr_path = self.driver.get_current_screenshot_folder()
+                lst = sort_files_by_creation(scr_path)
+                for scr in lst:
+                    img = Image.open(scr_path.as_posix() + "/" + scr)
+                    display_screenshot(img)
+                    time.sleep(0.35)
+            except:
+                pass
+        success = True
+        output = None
+
+        if logger:
+            log = {
+                "engine": "Navigation Controls",
+                "instruction": instruction,
+                "engine_log": None,
+                "success": success,
+                "output": output,
+                "code": code,
+            }
+            logger.add_log(log)
+
+        return success, output
+
+
 def get_model_name(llm: BaseLLM) -> str:
     try:
         # Try accessing the 'model' attribute
         return llm.model
     except AttributeError:
         try:
             # Try accessing the 'model_name' attribute
```

### Comparing `lavague_core-0.2.0/lavague/core/agents.py` & `lavague_core-0.2.1/lavague/core/agents.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,16 +44,14 @@
         self.driver.goto(url)
 
     def run(self, objective: str, user_data=None, display: bool = False):
         driver: BaseDriver = self.driver
         logger = self.logger
         n_steps = self.n_steps
         self.action_engine.set_display(display)
-        self.action_engine.navigation_control.set_display(display)
-        self.action_engine.python_engine.set_display(display)
 
         st_memory = self.st_memory
         world_model = self.world_model
 
         try:
             if os.path.isdir("screenshots"):
                 shutil.rmtree("screenshots")
```

### Comparing `lavague_core-0.2.0/lavague/core/base_driver.py` & `lavague_core-0.2.1/lavague/core/base_driver.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.0/lavague/core/context.py` & `lavague_core-0.2.1/lavague/core/context.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.0/lavague/core/extractors.py` & `lavague_core-0.2.1/lavague/core/extractors.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.0/lavague/core/logger.py` & `lavague_core-0.2.1/lavague/core/logger.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.0/lavague/core/memory.py` & `lavague_core-0.2.1/lavague/core/memory.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.0/lavague/core/navigation.py` & `lavague_core-0.2.1/lavague/core/utilities/web_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,111 @@
-import time
-from lavague.core.utilities.web_utils import display_screenshot, sort_files_by_creation
+from IPython.display import display, clear_output
+from PIL.PngImagePlugin import PngImageFile
+from PIL import Image
+import base64
+from lavague.core.utilities.format_utils import (
+    return_assigned_variables,
+    keep_assignments,
+)
+from io import BytesIO
+from selenium.webdriver.remote.webelement import WebElement
 from selenium.webdriver.remote.webdriver import WebDriver
-from selenium.webdriver.common.keys import Keys
+import os
+
+
+def sort_files_by_creation(directory):
+    def get_creation_time(item):
+        item_path = os.path.join(directory, item)
+        return os.path.getctime(item_path)
+
+    items = os.listdir(directory)
+    sorted_items = sorted(items, key=get_creation_time)
+    return sorted_items
+
+
+# Function to encode the image
+def encode_image(image_path):
+    with open(image_path, "rb") as image_file:
+        return base64.b64encode(image_file.read()).decode("utf-8")
+
+
+def display_screenshot(img: PngImageFile):
+    clear_output()
+    if img.mode == "RGBA":
+        img = img.convert("RGB")
+
+    try:
+        __IPYTHON__
+        display(img)
+    except:
+        img.show()
+
+
+def get_highlighted_element(driver: WebDriver, generated_code):
+    # TODO: Make code function with abstract driver
+    # Extract the assignments from the generated code
+    assignment_code = keep_assignments(generated_code)
+
+    # We add imports to the code to be executed
+    code = f"""
 from selenium.webdriver.common.by import By
-from lavague.core.logger import AgentLogger
-from lavague.core.action_engine import BaseActionEngine
-from lavague.core.base_driver import BaseDriver
-from PIL import Image
+from selenium.webdriver.common.keys import Keys
+from selenium.webdriver.common.action_chains import ActionChains
+{assignment_code}""".strip()
 
+    local_scope = {"driver": driver}
 
-class NavigationControl(BaseActionEngine):
-    driver: BaseDriver
-    time_between_actions: float
-    logger: AgentLogger
-
-    def __init__(
-        self,
-        driver: BaseDriver,
-        time_between_actions: float = 1.5,
-        logger: AgentLogger = None,
-    ) -> None:
-        self.driver: BaseDriver = driver
-        self.time_between_actions = time_between_actions
-        self.logger = logger
-        self.display = False
-
-    def set_display(self, display: bool):
-        self.display = display
-
-    def execute_instruction(self, instruction: str):
-        logger = self.logger
-        # TODO: Not clean the fact that we have driver / meta_driver around. Should settle for better names
-        meta_driver: BaseDriver = self.driver
-        driver: WebDriver = meta_driver.get_driver()
-        display_page = False
-
-        if "SCROLL_DOWN" in instruction:
-            code = (
-                """driver.execute_script("window.scrollBy(0, window.innerHeight);")"""
-            )
-        elif "SCROLL_UP" in instruction:
-            code = (
-                """driver.execute_script("window.scrollBy(0, -window.innerHeight);")"""
-            )
-        elif "WAIT" in instruction:
-            code = f"""
-import time
-time.sleep({self.time_between_actions})"""
-        elif "BACK" in instruction:
-            code = """driver.back()"""
-        elif "SCAN" in instruction:
-            # TODO: Should scan be in the navigation controls or in the driver?
-            code = """meta_driver.get_screenshots_whole_page()"""
-            display_page = True
-        else:
-            raise ValueError(f"Unknown instruction: {instruction}")
-
-        local_scope = {"driver": driver, "meta_driver": meta_driver}
-        exec(code, local_scope, local_scope)
-        if display_page and self.display:
-            try:
-                scr_path = self.driver.get_current_screenshot_folder()
-                lst = sort_files_by_creation(scr_path)
-                for scr in lst:
-                    img = Image.open(scr_path.as_posix() + "/" + scr)
-                    display_screenshot(img)
-                    time.sleep(0.35)
-            except:
-                pass
-        success = True
-        output = None
-
-        if logger:
-            log = {
-                "engine": "Navigation Controls",
-                "instruction": instruction,
-                "engine_log": None,
-                "success": success,
-                "output": output,
-                "code": code,
-            }
-            logger.add_log(log)
+    exec(code, local_scope, local_scope)
 
-        return success, output
+    # We extract pairs of variables assigned during execution with their name and pointer
+    variable_names = return_assigned_variables(generated_code)
+
+    elements = {}
+
+    for variable_name in variable_names:
+        var = local_scope[variable_name]
+        if type(var) == WebElement:
+            elements[variable_name] = var
+
+    if len(elements) == 0:
+        raise ValueError(f"No element found.")
+
+    outputs = []
+    for element_name, element in elements.items():
+        local_scope = {"driver": driver, element_name: element}
+
+        code = f"""
+element = {element_name}
+driver.execute_script("arguments[0].setAttribute('style', arguments[1]);", element, "border: 2px solid red;")
+driver.execute_script("arguments[0].scrollIntoView({{block: 'center'}});", element)
+screenshot = driver.get_screenshot_as_png()
+
+x1 = element.location['x']
+y1 = element.location['y']
+
+x2 = x1 + element.size['width']
+y2 = y1 + element.size['height']
+
+viewport_width = driver.execute_script("return window.innerWidth;")
+viewport_height = driver.execute_script("return window.innerHeight;")
+"""
+        exec(code, globals(), local_scope)
+        bounding_box = {
+            "x1": local_scope["x1"],
+            "y1": local_scope["y1"],
+            "x2": local_scope["x2"],
+            "y2": local_scope["y2"],
+        }
+        viewport_size = {
+            "width": local_scope["viewport_width"],
+            "height": local_scope["viewport_height"],
+        }
+        screenshot = local_scope["screenshot"]
+        screenshot = BytesIO(screenshot)
+        screenshot = Image.open(screenshot)
+        output = {
+            "screenshot": screenshot,
+            "bounding_box": bounding_box,
+            "viewport_size": viewport_size,
+        }
+        outputs.append(output)
+    return outputs
```

### Comparing `lavague_core-0.2.0/lavague/core/python_engine.py` & `lavague_core-0.2.1/lavague/core/python_engine.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 from llama_index.core.base.llms.base import BaseLLM
 from llama_index.core.embeddings import BaseEmbedding
 from lavague.core.base_driver import BaseDriver
 
 import trafilatura
 from llama_index.core import Document, VectorStoreIndex
 from lavague.core.logger import AgentLogger
-from lavague.core.action_engine import BaseActionEngine
+from lavague.core.base_engine import BaseEngine
 from PIL import Image
 
 
-class PythonEngine(BaseActionEngine):
+class PythonEngine(BaseEngine):
     llm: BaseLLM
     embedding: BaseEmbedding
     # TODO: Design question: should we have a driver available to Python engine?
     driver: BaseDriver
 
     def __init__(
         self,
```

### Comparing `lavague_core-0.2.0/lavague/core/retrievers.py` & `lavague_core-0.2.1/lavague/core/retrievers.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.0/lavague/core/rewriter.py` & `lavague_core-0.2.1/lavague/core/rewriter.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.0/lavague/core/utilities/format_utils.py` & `lavague_core-0.2.1/lavague/core/utilities/format_utils.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.0/lavague/core/utilities/telemetry.py` & `lavague_core-0.2.1/lavague/core/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.0/lavague/core/utilities/version_checker.py` & `lavague_core-0.2.1/lavague/core/utilities/version_checker.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.0/lavague/core/world_model.py` & `lavague_core-0.2.1/lavague/core/world_model.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.2.0/pyproject.toml` & `lavague_core-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry]
 name = "lavague-core"
-version = "0.2.0"
+version = "0.2.1"
 description = "automation code generation from text instructions"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_core-0.2.0/PKG-INFO` & `lavague_core-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-core
-Version: 0.2.0
+Version: 0.2.1
 Summary: automation code generation from text instructions
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

