# Comparing `tmp/easy_fnc-0.1.2.tar.gz` & `tmp/easy_fnc-0.1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_fnc-0.1.2.tar", last modified: Fri May 31 08:05:36 2024, max compression
+gzip compressed data, was "easy_fnc-0.1.2.1.tar", last modified: Fri May 31 08:11:29 2024, max compression
```

## Comparing `easy_fnc-0.1.2.tar` & `easy_fnc-0.1.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:05:36.456558 easy_fnc-0.1.2/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     6311 2024-05-31 08:05:36.456349 easy_fnc-0.1.2/PKG-INFO
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     5961 2024-05-31 08:04:19.000000 easy_fnc-0.1.2/README.md
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:05:36.456107 easy_fnc-0.1.2/easy_fnc.egg-info/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     6311 2024-05-31 08:05:36.000000 easy_fnc-0.1.2/easy_fnc.egg-info/PKG-INFO
--rw-r--r--   0 atakantekparmak   (501) staff       (20)      229 2024-05-31 08:05:36.000000 easy_fnc-0.1.2/easy_fnc.egg-info/SOURCES.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        1 2024-05-31 08:05:36.000000 easy_fnc-0.1.2/easy_fnc.egg-info/dependency_links.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)       15 2024-05-31 08:05:36.000000 easy_fnc-0.1.2/easy_fnc.egg-info/requires.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        7 2024-05-31 08:05:36.000000 easy_fnc-0.1.2/easy_fnc.egg-info/top_level.txt
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:05:36.455912 easy_fnc-0.1.2/models/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        0 2024-05-02 07:40:29.000000 easy_fnc-0.1.2/models/__init__.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     1119 2024-05-30 12:40:49.000000 easy_fnc-0.1.2/models/model.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     4439 2024-05-30 12:39:08.000000 easy_fnc-0.1.2/models/ollama.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)       38 2024-05-31 08:05:36.456642 easy_fnc-0.1.2/setup.cfg
--rw-r--r--   0 atakantekparmak   (501) staff       (20)      780 2024-05-31 08:04:46.000000 easy_fnc-0.1.2/setup.py
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:11:29.095975 easy_fnc-0.1.2.1/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     5747 2024-05-31 08:11:29.095717 easy_fnc-0.1.2.1/PKG-INFO
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     5395 2024-05-31 08:06:39.000000 easy_fnc-0.1.2.1/README.md
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:11:29.095394 easy_fnc-0.1.2.1/easy_fnc.egg-info/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     5747 2024-05-31 08:11:29.000000 easy_fnc-0.1.2.1/easy_fnc.egg-info/PKG-INFO
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)      229 2024-05-31 08:11:29.000000 easy_fnc-0.1.2.1/easy_fnc.egg-info/SOURCES.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        1 2024-05-31 08:11:29.000000 easy_fnc-0.1.2.1/easy_fnc.egg-info/dependency_links.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)       15 2024-05-31 08:11:29.000000 easy_fnc-0.1.2.1/easy_fnc.egg-info/requires.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        7 2024-05-31 08:11:29.000000 easy_fnc-0.1.2.1/easy_fnc.egg-info/top_level.txt
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:11:29.095183 easy_fnc-0.1.2.1/models/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        0 2024-05-02 07:40:29.000000 easy_fnc-0.1.2.1/models/__init__.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     1119 2024-05-30 12:40:49.000000 easy_fnc-0.1.2.1/models/model.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     4439 2024-05-30 12:39:08.000000 easy_fnc-0.1.2.1/models/ollama.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)       38 2024-05-31 08:11:29.096035 easy_fnc-0.1.2.1/setup.cfg
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)      782 2024-05-31 08:11:26.000000 easy_fnc-0.1.2.1/setup.py
```

### Comparing `easy_fnc-0.1.2/PKG-INFO` & `easy_fnc-0.1.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_fnc
-Version: 0.1.2
+Version: 0.1.2.1
 Summary: This package hopes to provide a modular and highly extendable interface to interact with LLMs via (multiple) function calling, easily.
 Author: Atakan Tekparmak
 Author-email: atakantekerparmak@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: ollama
 Requires-Dist: tomllib
 
@@ -99,32 +99,14 @@
 from easy_fnc.models.ollama import OllamaModel
 
 model = OllamaModel(model_name="model_name", functions=[...])
 response = model.generate(user_input="user input")
 function_calls = model.get_function_calls(user_input="user input", verbose=True)
 ```
 
-## Configuration
-
-The package allows users to configure the filename of the functions file using an environment variable `EASY_FNC_FUNCTIONS_FILE`. If the environment variable is not set, it defaults to `easy_fnc/functions.py`.
-
-Example:
-
-```python
-import os
-
-os.environ["EASY_FNC_FUNCTIONS_FILE"] = "path/to/custom_functions.py"
-```
-
-## Templates
-
-Sure! Let's update the README to reflect the changes in the `OllamaModel` class and add a `load_template` method to `utils.py` for loading templates from JSON files.
-
-1. Update the "Templates" section in the README:
-
 ## Templates
 
 The `easy_fnc` package uses JSON templates to format user input and model responses. The `OllamaModel` class accepts both a string and a dictionary as parameters for the template.
 
 To use a custom template, you have two options:
 
 1. Provide the name of a JSON template file located in the `easy_fnc/models/templates/` directory. The `OllamaModel` will automatically load the template using the `load_template` method.
```

### Comparing `easy_fnc-0.1.2/README.md` & `easy_fnc-0.1.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -89,32 +89,14 @@
 from easy_fnc.models.ollama import OllamaModel
 
 model = OllamaModel(model_name="model_name", functions=[...])
 response = model.generate(user_input="user input")
 function_calls = model.get_function_calls(user_input="user input", verbose=True)
 ```
 
-## Configuration
-
-The package allows users to configure the filename of the functions file using an environment variable `EASY_FNC_FUNCTIONS_FILE`. If the environment variable is not set, it defaults to `easy_fnc/functions.py`.
-
-Example:
-
-```python
-import os
-
-os.environ["EASY_FNC_FUNCTIONS_FILE"] = "path/to/custom_functions.py"
-```
-
-## Templates
-
-Sure! Let's update the README to reflect the changes in the `OllamaModel` class and add a `load_template` method to `utils.py` for loading templates from JSON files.
-
-1. Update the "Templates" section in the README:
-
 ## Templates
 
 The `easy_fnc` package uses JSON templates to format user input and model responses. The `OllamaModel` class accepts both a string and a dictionary as parameters for the template.
 
 To use a custom template, you have two options:
 
 1. Provide the name of a JSON template file located in the `easy_fnc/models/templates/` directory. The `OllamaModel` will automatically load the template using the `load_template` method.
```

### Comparing `easy_fnc-0.1.2/easy_fnc.egg-info/PKG-INFO` & `easy_fnc-0.1.2.1/easy_fnc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_fnc
-Version: 0.1.2
+Version: 0.1.2.1
 Summary: This package hopes to provide a modular and highly extendable interface to interact with LLMs via (multiple) function calling, easily.
 Author: Atakan Tekparmak
 Author-email: atakantekerparmak@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: ollama
 Requires-Dist: tomllib
 
@@ -99,32 +99,14 @@
 from easy_fnc.models.ollama import OllamaModel
 
 model = OllamaModel(model_name="model_name", functions=[...])
 response = model.generate(user_input="user input")
 function_calls = model.get_function_calls(user_input="user input", verbose=True)
 ```
 
-## Configuration
-
-The package allows users to configure the filename of the functions file using an environment variable `EASY_FNC_FUNCTIONS_FILE`. If the environment variable is not set, it defaults to `easy_fnc/functions.py`.
-
-Example:
-
-```python
-import os
-
-os.environ["EASY_FNC_FUNCTIONS_FILE"] = "path/to/custom_functions.py"
-```
-
-## Templates
-
-Sure! Let's update the README to reflect the changes in the `OllamaModel` class and add a `load_template` method to `utils.py` for loading templates from JSON files.
-
-1. Update the "Templates" section in the README:
-
 ## Templates
 
 The `easy_fnc` package uses JSON templates to format user input and model responses. The `OllamaModel` class accepts both a string and a dictionary as parameters for the template.
 
 To use a custom template, you have two options:
 
 1. Provide the name of a JSON template file located in the `easy_fnc/models/templates/` directory. The `OllamaModel` will automatically load the template using the `load_template` method.
```

### Comparing `easy_fnc-0.1.2/models/model.py` & `easy_fnc-0.1.2.1/models/model.py`

 * *Files identical despite different names*

### Comparing `easy_fnc-0.1.2/models/ollama.py` & `easy_fnc-0.1.2.1/models/ollama.py`

 * *Files identical despite different names*

### Comparing `easy_fnc-0.1.2/setup.py` & `easy_fnc-0.1.2.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Read the README.md file and return its contents."""
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 def main():
     setup(
         name='easy_fnc',
-        version='0.1.2',
+        version='0.1.2.1',
         description='This package hopes to provide a modular and highly extendable interface to interact with LLMs via (multiple) function calling, easily.',
         long_description=read_readme(),
         long_description_content_type="text/markdown",
         author='Atakan Tekparmak',
         author_email='atakantekerparmak@gmail.com',
         packages=find_packages(),
         install_requires=[
```

