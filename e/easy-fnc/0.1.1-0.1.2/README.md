# Comparing `tmp/easy_fnc-0.1.1.tar.gz` & `tmp/easy_fnc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_fnc-0.1.1.tar", last modified: Thu May 30 09:46:03 2024, max compression
+gzip compressed data, was "easy_fnc-0.1.2.tar", last modified: Fri May 31 08:05:36 2024, max compression
```

## Comparing `easy_fnc-0.1.1.tar` & `easy_fnc-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-30 09:46:03.242254 easy_fnc-0.1.1/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     4449 2024-05-30 09:46:03.242030 easy_fnc-0.1.1/PKG-INFO
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     4099 2024-05-30 09:32:04.000000 easy_fnc-0.1.1/README.md
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-30 09:46:03.241735 easy_fnc-0.1.1/easy_fnc.egg-info/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     4449 2024-05-30 09:46:03.000000 easy_fnc-0.1.1/easy_fnc.egg-info/PKG-INFO
--rw-r--r--   0 atakantekparmak   (501) staff       (20)      229 2024-05-30 09:46:03.000000 easy_fnc-0.1.1/easy_fnc.egg-info/SOURCES.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        1 2024-05-30 09:46:03.000000 easy_fnc-0.1.1/easy_fnc.egg-info/dependency_links.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)       15 2024-05-30 09:46:03.000000 easy_fnc-0.1.1/easy_fnc.egg-info/requires.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        7 2024-05-30 09:46:03.000000 easy_fnc-0.1.1/easy_fnc.egg-info/top_level.txt
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-30 09:46:03.241549 easy_fnc-0.1.1/models/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        0 2024-05-02 07:40:29.000000 easy_fnc-0.1.1/models/__init__.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)      972 2024-05-02 07:40:29.000000 easy_fnc-0.1.1/models/model.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     4090 2024-05-10 14:27:19.000000 easy_fnc-0.1.1/models/ollama.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)       38 2024-05-30 09:46:03.242311 easy_fnc-0.1.1/setup.cfg
--rw-r--r--   0 atakantekparmak   (501) staff       (20)      780 2024-05-30 09:45:54.000000 easy_fnc-0.1.1/setup.py
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:05:36.456558 easy_fnc-0.1.2/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     6311 2024-05-31 08:05:36.456349 easy_fnc-0.1.2/PKG-INFO
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     5961 2024-05-31 08:04:19.000000 easy_fnc-0.1.2/README.md
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:05:36.456107 easy_fnc-0.1.2/easy_fnc.egg-info/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     6311 2024-05-31 08:05:36.000000 easy_fnc-0.1.2/easy_fnc.egg-info/PKG-INFO
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)      229 2024-05-31 08:05:36.000000 easy_fnc-0.1.2/easy_fnc.egg-info/SOURCES.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        1 2024-05-31 08:05:36.000000 easy_fnc-0.1.2/easy_fnc.egg-info/dependency_links.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)       15 2024-05-31 08:05:36.000000 easy_fnc-0.1.2/easy_fnc.egg-info/requires.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        7 2024-05-31 08:05:36.000000 easy_fnc-0.1.2/easy_fnc.egg-info/top_level.txt
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:05:36.455912 easy_fnc-0.1.2/models/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        0 2024-05-02 07:40:29.000000 easy_fnc-0.1.2/models/__init__.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     1119 2024-05-30 12:40:49.000000 easy_fnc-0.1.2/models/model.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     4439 2024-05-30 12:39:08.000000 easy_fnc-0.1.2/models/ollama.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)       38 2024-05-31 08:05:36.456642 easy_fnc-0.1.2/setup.cfg
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)      780 2024-05-31 08:04:46.000000 easy_fnc-0.1.2/setup.py
```

### Comparing `easy_fnc-0.1.1/models/model.py` & `easy_fnc-0.1.2/models/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from abc import ABC, abstractmethod
 from json import load as load_json
+from typing import Optional
 
 class EasyFNCModel(ABC):
     """
     Abstract class for EasyFNC models.
     """
     def __init__(self, functions: list[dict[str, str]]) -> None:
         self.functions = functions
@@ -24,15 +25,18 @@
         """
         Get the function calls from the user input.
         """
 
     def load_template(
         self, 
         template_name: str,
-        template_dir: str = "easy_fnc/models/templates/"
-    ) -> dict:
+        template_dir: Optional[str] = None
+        ) -> dict:
         """
-        Load a template from the template directory.
+        Load a template from the specified directory or the default template directory.
         """
+        if template_dir is None:
+            template_dir = "easy_fnc/models/templates/"
+    
         with open(f"{template_dir}{template_name}.json", "r") as file:
             return load_json(file)
```

### Comparing `easy_fnc-0.1.1/models/ollama.py` & `easy_fnc-0.1.2/models/ollama.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,32 @@
 import ollama
+
 import json
+from typing import Union
 
 from easy_fnc.models.model import EasyFNCModel
 
 class OllamaModel(EasyFNCModel):
     """
     A class to generate responses using the Ollama model.
     """
-    def __init__(self, model_name: str, functions: list[dict[str, str]]) -> None:
+    def __init__(
+            self, 
+            model_name: str, 
+            functions: list[dict[str, str]],
+            template: Union[str, dict]
+        ) -> None:
         super().__init__(functions)
         self.model_name = model_name
-        self.template = self.load_template(template_name="hermes2pro-llama3-8b")
+        if isinstance(template, str):
+            self.template = self.load_template(template_name=model_name.split("/")[1])
+        elif isinstance(template, dict):
+            self.template = template
+        else:
+            raise ValueError("Invalid template format. Expected a template name or a dictionary.")
     
     def format_user_input(self, user_input: str) -> str:
         """ Format the user input. """
         # Create the system prompt
         prompt_beginning = self.template["function_call_prompt"]["beginning"]
         system_prompt_end = self.template["function_call_prompt"]["system_prompt_end"]
         system_prompt = prompt_beginning + json.dumps(self.functions, indent=4) + system_prompt_end
```

### Comparing `easy_fnc-0.1.1/setup.py` & `easy_fnc-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Read the README.md file and return its contents."""
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 def main():
     setup(
         name='easy_fnc',
-        version='0.1.1',
+        version='0.1.2',
         description='This package hopes to provide a modular and highly extendable interface to interact with LLMs via (multiple) function calling, easily.',
         long_description=read_readme(),
         long_description_content_type="text/markdown",
         author='Atakan Tekparmak',
         author_email='atakantekerparmak@gmail.com',
         packages=find_packages(),
         install_requires=[
```

