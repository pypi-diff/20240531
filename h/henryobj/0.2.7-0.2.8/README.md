# Comparing `tmp/henryobj-0.2.7.tar.gz` & `tmp/henryobj-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henryobj-0.2.7.tar", last modified: Thu Apr 18 07:34:23 2024, max compression
+gzip compressed data, was "henryobj-0.2.8.tar", last modified: Fri May 31 14:09:10 2024, max compression
```

## Comparing `henryobj-0.2.7.tar` & `henryobj-0.2.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-18 07:34:23.893001 henryobj-0.2.7/
--rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-18 07:34:23.892851 henryobj-0.2.7/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)     2976 2024-01-24 08:03:39.000000 henryobj-0.2.7/README.md
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-18 07:34:23.891800 henryobj-0.2.7/henryobj/
--rw-r--r--   0 henry      (501) staff       (20)      224 2024-04-09 07:08:41.000000 henryobj-0.2.7/henryobj/__init__.py
--rw-r--r--   0 henry      (501) staff       (20)    22625 2024-04-11 08:30:24.000000 henryobj-0.2.7/henryobj/base.py
--rw-r--r--   0 henry      (501) staff       (20)     1563 2024-04-18 07:33:26.000000 henryobj-0.2.7/henryobj/config.py
--rw-r--r--   0 henry      (501) staff       (20)    13971 2024-04-11 08:30:55.000000 henryobj-0.2.7/henryobj/gpt.py
--rw-r--r--   0 henry      (501) staff       (20)    30005 2024-04-18 07:33:58.000000 henryobj-0.2.7/henryobj/oai.py
--rw-r--r--   0 henry      (501) staff       (20)    14269 2024-04-15 10:23:49.000000 henryobj-0.2.7/henryobj/web.py
-drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-04-18 07:34:23.892660 henryobj-0.2.7/henryobj.egg-info/
--rw-r--r--   0 henry      (501) staff       (20)     3115 2024-04-18 07:34:23.000000 henryobj-0.2.7/henryobj.egg-info/PKG-INFO
--rw-r--r--   0 henry      (501) staff       (20)      282 2024-04-18 07:34:23.000000 henryobj-0.2.7/henryobj.egg-info/SOURCES.txt
--rw-r--r--   0 henry      (501) staff       (20)        1 2024-04-18 07:34:23.000000 henryobj-0.2.7/henryobj.egg-info/dependency_links.txt
--rw-r--r--   0 henry      (501) staff       (20)       60 2024-04-18 07:34:23.000000 henryobj-0.2.7/henryobj.egg-info/requires.txt
--rw-r--r--   0 henry      (501) staff       (20)        9 2024-04-18 07:34:23.000000 henryobj-0.2.7/henryobj.egg-info/top_level.txt
--rw-r--r--   0 henry      (501) staff       (20)       38 2024-04-18 07:34:23.893063 henryobj-0.2.7/setup.cfg
--rw-r--r--   0 henry      (501) staff       (20)      574 2024-04-18 07:34:20.000000 henryobj-0.2.7/setup.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-31 14:09:10.647433 henryobj-0.2.8/
+-rw-r--r--   0 henry      (501) staff       (20)     3115 2024-05-31 14:09:10.647274 henryobj-0.2.8/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)     2976 2024-01-24 08:03:39.000000 henryobj-0.2.8/README.md
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-31 14:09:10.646330 henryobj-0.2.8/henryobj/
+-rw-r--r--   0 henry      (501) staff       (20)      224 2024-04-09 07:08:41.000000 henryobj-0.2.8/henryobj/__init__.py
+-rw-r--r--   0 henry      (501) staff       (20)    22672 2024-05-31 14:08:15.000000 henryobj-0.2.8/henryobj/base.py
+-rw-r--r--   0 henry      (501) staff       (20)     1586 2024-05-31 14:06:51.000000 henryobj-0.2.8/henryobj/config.py
+-rw-r--r--   0 henry      (501) staff       (20)    13971 2024-04-11 08:30:55.000000 henryobj-0.2.8/henryobj/gpt.py
+-rw-r--r--   0 henry      (501) staff       (20)    30590 2024-05-31 14:06:34.000000 henryobj-0.2.8/henryobj/oai.py
+-rw-r--r--   0 henry      (501) staff       (20)    14269 2024-04-15 10:23:49.000000 henryobj-0.2.8/henryobj/web.py
+drwxr-xr-x   0 henry      (501) staff       (20)        0 2024-05-31 14:09:10.647057 henryobj-0.2.8/henryobj.egg-info/
+-rw-r--r--   0 henry      (501) staff       (20)     3115 2024-05-31 14:09:10.000000 henryobj-0.2.8/henryobj.egg-info/PKG-INFO
+-rw-r--r--   0 henry      (501) staff       (20)      282 2024-05-31 14:09:10.000000 henryobj-0.2.8/henryobj.egg-info/SOURCES.txt
+-rw-r--r--   0 henry      (501) staff       (20)        1 2024-05-31 14:09:10.000000 henryobj-0.2.8/henryobj.egg-info/dependency_links.txt
+-rw-r--r--   0 henry      (501) staff       (20)       60 2024-05-31 14:09:10.000000 henryobj-0.2.8/henryobj.egg-info/requires.txt
+-rw-r--r--   0 henry      (501) staff       (20)        9 2024-05-31 14:09:10.000000 henryobj-0.2.8/henryobj.egg-info/top_level.txt
+-rw-r--r--   0 henry      (501) staff       (20)       38 2024-05-31 14:09:10.647495 henryobj-0.2.8/setup.cfg
+-rw-r--r--   0 henry      (501) staff       (20)      574 2024-05-31 14:08:53.000000 henryobj-0.2.8/setup.py
```

### Comparing `henryobj-0.2.7/PKG-INFO` & `henryobj-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henryobj
-Version: 0.2.7
+Version: 0.2.8
 Home-page: https://github.com/HenryObj/mypip
 Description-Content-Type: text/markdown
 
 # PIP Package henryobj Overview - 24th of January
 
 This codebase is a Python package designed to facilitate web scraping, interactions with OpenAI's API, and provide a suite of utility functions. It is structured to be modular, allowing each component to function independently or in conjunction with others, promoting maintainability and scalability.
```

### Comparing `henryobj-0.2.7/README.md` & `henryobj-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.7/henryobj/base.py` & `henryobj-0.2.8/henryobj/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,19 +332,19 @@
     module_name = get_module_name(func)
     print(f"** LOG ** {line_number} of {module_name} ** INFO: {additional_info}")
     
 def perf(function: Callable[..., Any]):
     """
     To be used as a decorator to a function to display the time to run the said function.
     """
-    start = time.perf_counter()
     def wrapper(*args, **kwargs):
-        res = function(*args,**kwargs)
-        end = time.perf_counter()
-        duration = round((end-start), 2)
+        start = time.perf_counter()  # Start timing here
+        res = function(*args, **kwargs)
+        end = time.perf_counter()  # End timing here
+        duration = round((end - start), 2)
         print(f"{function.__name__} done in {duration} seconds")
         return res
     return wrapper
 
 def print_dir_structure(startpath: str, include_dot_contents: bool = False, use_pipes: bool = True, save_to_file: bool = False, output_file: str = 'dir_structure.txt'):
     """
     Prints or saves the directory and its content, excluding files and directories specified in .gitignore and __pycache__.
```

### Comparing `henryobj-0.2.7/henryobj/config.py` & `henryobj-0.2.8/henryobj/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # PIP Package of utlity functions used in various projects
 
 # Made by Henry Obegi - hobegi@gmail.com
 # First version: September 2023
-# Last update: 30th of March 2024
+# Last update: 31st of May 2024
 
 
 
 # ****** TEXT
 OPEN_AI_ISSUE = r"%$144$%" # When OpenAI is down
 ERROR_MESSAGE = "An error occurred and was logged"
 WARNING_UNKNOWN = "\033[31mUNKNOWN\033[0m"
@@ -25,17 +25,19 @@
 MAX_TOKEN_OUTPUT_DEFAULT = 300
 MAX_TOKEN_OUTPUT_DEFAULT_HUGE = 3000
 
 MAX_TOKEN_WINDOW_OLD = 4096 
 MAX_TOKEN_WINDOW_GPT4_TURBO = 128000
 MAX_TOKEN_WINDOW_GPT35_TURBO = 16385
 MAX_TOKEN_WINDOW_GPT4 = 8192
-WINDOW_BUFFER = 100
+WINDOW_BUFFER = 150
 
 # ****** MODELS
+MODEL_GPT4O = r"gpt-4o"
+
 MODEL_GPT4_TURBO = r"gpt-4-1106-preview" #Max 128,000 token context window total with 4,096 output
 MODEL_GPT4_STABLE = r"gpt-4" # 8K context window and 4,096 output
 
 MODEL_CHAT_BACKUP = r"gpt-3.5-turbo-1106" # Context 16,385 tokens - Reply 4,096
 MODEL_CHAT = r"gpt-3.5-turbo-0125"
 MODEL_CHAT_STABLE = r"gpt-3.5-turbo"
```

### Comparing `henryobj-0.2.7/henryobj/gpt.py` & `henryobj-0.2.8/henryobj/gpt.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.7/henryobj/oai.py` & `henryobj-0.2.8/henryobj/oai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # All that is related ot Open AI
 
 from .config import (
     ERROR_MESSAGE, OPEN_AI_ISSUE, MAX_TOKEN_OUTPUT_DEFAULT, MAX_TOKEN_OUTPUT_DEFAULT_HUGE, MAX_TOKEN_WINDOW_GPT4, 
-    MAX_TOKEN_WINDOW_GPT4_TURBO, MAX_TOKEN_WINDOW_OLD, MAX_TOKEN_WINDOW_GPT35_TURBO, MODEL_GPT4_TURBO,
+    MAX_TOKEN_WINDOW_GPT4_TURBO, MAX_TOKEN_WINDOW_OLD, MAX_TOKEN_WINDOW_GPT35_TURBO, MODEL_GPT4_TURBO, MODEL_GPT4O,
     MODEL_GPT4_STABLE, MODEL_CHAT, MODEL_EMB_LARGE, MODEL_CHAT_STABLE, MODEL_CHAT_BACKUP, WINDOW_BUFFER
 )
 from .base import log_warning, log_issue, split_into_sentences, custom_round, check_co
 
 
 from typing import Optional
 
@@ -488,29 +488,30 @@
 
 # *************************************************************************************************
 # ****************************************** REGULAR API CALLS ************************************
 # *************************************************************************************************
 
 def ask_question_gpt(question:str, role:str = "", model:str = MODEL_CHAT, max_tokens:int = MAX_TOKEN_OUTPUT_DEFAULT, verbose:bool = True, temperature=0, top_p=1, json_on: bool = False) -> str:
     """
-    Queries an OpenAI GPT model (GPT-3.5 Turbo or GPT-4) with a specific question.
+    Queries an OpenAI GPT model (GPT-3.5 Turbo / GPT-4 / GPT-4O) with a specific question.
 
     Args:
         question (str): The question to ask the model.
         role (str, optional): System prompt to be initialized in the chat table, defining ChatGPT's behavior.
-        model (str, optional): The model to use. Defaults to GPT-3.5 Turbo. To choose GPT 4, use 'MODEL_GPT4_TURBO'
+        model (str, optional): The model to use. Defaults to GPT-3.5 Turbo. To choose GPT-4O, use 'MODEL_GPT4O' or call 'ask_question_gpto'.
         max_tokens (int, optional): Maximum number of tokens for the answer.
         verbose (bool, optional): Will print information in the console.
         json_on (bool, optional): Whether to force the output in JSON format // UNUSED FOR NOW
 
     Returns:
         str: The model's reply to the question.
     """
     max_token_window = {
         MODEL_GPT4_TURBO: MAX_TOKEN_WINDOW_GPT4_TURBO - WINDOW_BUFFER,
+        MODEL_GPT4O: MAX_TOKEN_WINDOW_GPT4_TURBO - WINDOW_BUFFER,
         MODEL_GPT4_STABLE: MAX_TOKEN_WINDOW_GPT4 - WINDOW_BUFFER,
         MODEL_CHAT: MAX_TOKEN_WINDOW_GPT35_TURBO - WINDOW_BUFFER,
         MODEL_CHAT_STABLE: MAX_TOKEN_WINDOW_GPT35_TURBO - WINDOW_BUFFER,
     }.get(model, MAX_TOKEN_WINDOW_OLD - WINDOW_BUFFER)
     initial_token_usage = calculate_token(role) + calculate_token(question)
     if initial_token_usage > max_token_window:
         print("Your input is too large for the query regardless of the max_tokens for the reply.")
@@ -527,14 +528,20 @@
 
 def ask_question_gpt4(question: str, role: str, model=MODEL_GPT4_TURBO, max_tokens=MAX_TOKEN_OUTPUT_DEFAULT_HUGE, verbose = False, temperature=0, top_p=1, json_on=False) -> str:
     """
     Queries Chat GPT 4 with a specific question if too lazy to change the param in ask_question_gpt)
     """
     return ask_question_gpt(question = question, role = role, model = model, max_tokens= max_tokens, verbose=verbose, temperature=temperature, top_p=top_p, json_on=json_on)
 
+def ask_question_gpto(question: str, role: str, model=MODEL_GPT4_TURBO, max_tokens=MAX_TOKEN_OUTPUT_DEFAULT_HUGE, verbose = False, temperature=0, top_p=1, json_on=False) -> str:
+    """
+    Queries Chat GPT 4 with a specific question if too lazy to change the param in ask_question_gpt)
+    """
+    return ask_question_gpt(question = question, role = role, model = model, max_tokens= max_tokens, verbose=verbose, temperature=temperature, top_p=top_p, json_on=json_on)
+
 def embed_text(text:str, max_attempts:int=3, model=MODEL_EMB_LARGE) -> Optional[list[float]]:
     """
     Micro function which returns the embedding of one chunk of text or 0 if issue.
     Used for the multi-threading.
 
     Model is the new large new embedding one. Use Small if speed is a concern.
     Returns None if issue.
@@ -568,15 +575,15 @@
     Calls the ChatGPT OpenAI completion endpoint with specified parameters.
 
     Args:
         current_chat (list): The prompt used for the request.
         max_tokens (int, optional): Maximum number of tokens for the answer.
         stop_list (bool, optional): Whether to use specific stop tokens. Defaults to False.
         max_attempts (int, optional): Maximum number of retries. Defaults to 3.
-        model (str, optional): ChatGPT OpenAI model used for the request. Defaults to 'MODEL_CHAT'.
+        model (str, optional): ChatGPT OpenAI model used for the request. Defaults to the GPT-3.5 Turbo
         temperature (float, optional): Sampling temperature for the response. A value of 0 means deterministic output. Defaults to 0.
         top_p (float, optional): Nucleus sampling parameter, with 1 being 'take the best'. Defaults to 1.
         json (bool, optional): Whether we want to force the output in JSON or not.
 
     Returns:
         str: The response text or 'OPEN_AI_ISSUE' if an error occurs (e.g., if OpenAI service is down).
     """
```

### Comparing `henryobj-0.2.7/henryobj/web.py` & `henryobj-0.2.8/henryobj/web.py`

 * *Files identical despite different names*

### Comparing `henryobj-0.2.7/henryobj.egg-info/PKG-INFO` & `henryobj-0.2.8/henryobj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: henryobj
-Version: 0.2.7
+Version: 0.2.8
 Home-page: https://github.com/HenryObj/mypip
 Description-Content-Type: text/markdown
 
 # PIP Package henryobj Overview - 24th of January
 
 This codebase is a Python package designed to facilitate web scraping, interactions with OpenAI's API, and provide a suite of utility functions. It is structured to be modular, allowing each component to function independently or in conjunction with others, promoting maintainability and scalability.
```

### Comparing `henryobj-0.2.7/setup.py` & `henryobj-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="henryobj",
-    version="0.2.7", # need to increment this everytime otherwise Pypi will not accept the new version
+    version="0.2.8", # need to increment this everytime otherwise Pypi will not accept the new version
      url='https://github.com/HenryObj/mypip',
     packages=find_packages(),
     install_requires=[
         "openai>=1.9.0",
         "tiktoken>=0.5.2",
         "requests>=2.31.0",
         "bs4",
```

