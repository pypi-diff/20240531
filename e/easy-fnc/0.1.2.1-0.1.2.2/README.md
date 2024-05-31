# Comparing `tmp/easy_fnc-0.1.2.1.tar.gz` & `tmp/easy_fnc-0.1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_fnc-0.1.2.1.tar", last modified: Fri May 31 08:11:29 2024, max compression
+gzip compressed data, was "easy_fnc-0.1.2.2.tar", last modified: Fri May 31 08:17:41 2024, max compression
```

## Comparing `easy_fnc-0.1.2.1.tar` & `easy_fnc-0.1.2.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:11:29.095975 easy_fnc-0.1.2.1/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     5747 2024-05-31 08:11:29.095717 easy_fnc-0.1.2.1/PKG-INFO
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     5395 2024-05-31 08:06:39.000000 easy_fnc-0.1.2.1/README.md
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:11:29.095394 easy_fnc-0.1.2.1/easy_fnc.egg-info/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     5747 2024-05-31 08:11:29.000000 easy_fnc-0.1.2.1/easy_fnc.egg-info/PKG-INFO
--rw-r--r--   0 atakantekparmak   (501) staff       (20)      229 2024-05-31 08:11:29.000000 easy_fnc-0.1.2.1/easy_fnc.egg-info/SOURCES.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        1 2024-05-31 08:11:29.000000 easy_fnc-0.1.2.1/easy_fnc.egg-info/dependency_links.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)       15 2024-05-31 08:11:29.000000 easy_fnc-0.1.2.1/easy_fnc.egg-info/requires.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        7 2024-05-31 08:11:29.000000 easy_fnc-0.1.2.1/easy_fnc.egg-info/top_level.txt
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:11:29.095183 easy_fnc-0.1.2.1/models/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        0 2024-05-02 07:40:29.000000 easy_fnc-0.1.2.1/models/__init__.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     1119 2024-05-30 12:40:49.000000 easy_fnc-0.1.2.1/models/model.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     4439 2024-05-30 12:39:08.000000 easy_fnc-0.1.2.1/models/ollama.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)       38 2024-05-31 08:11:29.096035 easy_fnc-0.1.2.1/setup.cfg
--rw-r--r--   0 atakantekparmak   (501) staff       (20)      782 2024-05-31 08:11:26.000000 easy_fnc-0.1.2.1/setup.py
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:17:41.644762 easy_fnc-0.1.2.2/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     5749 2024-05-31 08:17:41.644487 easy_fnc-0.1.2.2/PKG-INFO
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     5397 2024-05-31 08:16:58.000000 easy_fnc-0.1.2.2/README.md
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:17:41.644205 easy_fnc-0.1.2.2/easy_fnc.egg-info/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     5749 2024-05-31 08:17:41.000000 easy_fnc-0.1.2.2/easy_fnc.egg-info/PKG-INFO
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)      229 2024-05-31 08:17:41.000000 easy_fnc-0.1.2.2/easy_fnc.egg-info/SOURCES.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        1 2024-05-31 08:17:41.000000 easy_fnc-0.1.2.2/easy_fnc.egg-info/dependency_links.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)       15 2024-05-31 08:17:41.000000 easy_fnc-0.1.2.2/easy_fnc.egg-info/requires.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        7 2024-05-31 08:17:41.000000 easy_fnc-0.1.2.2/easy_fnc.egg-info/top_level.txt
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:17:41.643982 easy_fnc-0.1.2.2/models/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        0 2024-05-02 07:40:29.000000 easy_fnc-0.1.2.2/models/__init__.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     1119 2024-05-30 12:40:49.000000 easy_fnc-0.1.2.2/models/model.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     4439 2024-05-30 12:39:08.000000 easy_fnc-0.1.2.2/models/ollama.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)       38 2024-05-31 08:17:41.644817 easy_fnc-0.1.2.2/setup.cfg
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)      782 2024-05-31 08:17:39.000000 easy_fnc-0.1.2.2/setup.py
```

### Comparing `easy_fnc-0.1.2.1/PKG-INFO` & `easy_fnc-0.1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_fnc
-Version: 0.1.2.1
+Version: 0.1.2.2
 Summary: This package hopes to provide a modular and highly extendable interface to interact with LLMs via (multiple) function calling, easily.
 Author: Atakan Tekparmak
 Author-email: atakantekerparmak@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: ollama
 Requires-Dist: tomllib
 
@@ -63,15 +63,15 @@
 ### Models
 
 The package provides an abstract base class `EasyFNCModel` in the `model.py` file. This class defines the interface for implementing AI models that can generate responses based on user input and execute function calls.
 
 To create a custom model, subclass `EasyFNCModel` and implement the required methods:
 
 - `generate(self, user_input: str) -> dict`: Generate a response based on the user input.
-- `get_function_calls(self, user_input: str, verbose: bool = False) -> list[dict]`: Extract function calls from the user input.
+- `get_function_calls(self, user_input: str, verbose: bool = False) -> list[dict]`: Extract function calls from the model output.
 
 Example:
 
 ```python
 from easy_fnc.models.model import EasyFNCModel
 
 class CustomModel(EasyFNCModel):
```

### Comparing `easy_fnc-0.1.2.1/README.md` & `easy_fnc-0.1.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 ### Models
 
 The package provides an abstract base class `EasyFNCModel` in the `model.py` file. This class defines the interface for implementing AI models that can generate responses based on user input and execute function calls.
 
 To create a custom model, subclass `EasyFNCModel` and implement the required methods:
 
 - `generate(self, user_input: str) -> dict`: Generate a response based on the user input.
-- `get_function_calls(self, user_input: str, verbose: bool = False) -> list[dict]`: Extract function calls from the user input.
+- `get_function_calls(self, user_input: str, verbose: bool = False) -> list[dict]`: Extract function calls from the model output.
 
 Example:
 
 ```python
 from easy_fnc.models.model import EasyFNCModel
 
 class CustomModel(EasyFNCModel):
```

### Comparing `easy_fnc-0.1.2.1/easy_fnc.egg-info/PKG-INFO` & `easy_fnc-0.1.2.2/easy_fnc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy_fnc
-Version: 0.1.2.1
+Version: 0.1.2.2
 Summary: This package hopes to provide a modular and highly extendable interface to interact with LLMs via (multiple) function calling, easily.
 Author: Atakan Tekparmak
 Author-email: atakantekerparmak@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: ollama
 Requires-Dist: tomllib
 
@@ -63,15 +63,15 @@
 ### Models
 
 The package provides an abstract base class `EasyFNCModel` in the `model.py` file. This class defines the interface for implementing AI models that can generate responses based on user input and execute function calls.
 
 To create a custom model, subclass `EasyFNCModel` and implement the required methods:
 
 - `generate(self, user_input: str) -> dict`: Generate a response based on the user input.
-- `get_function_calls(self, user_input: str, verbose: bool = False) -> list[dict]`: Extract function calls from the user input.
+- `get_function_calls(self, user_input: str, verbose: bool = False) -> list[dict]`: Extract function calls from the model output.
 
 Example:
 
 ```python
 from easy_fnc.models.model import EasyFNCModel
 
 class CustomModel(EasyFNCModel):
```

### Comparing `easy_fnc-0.1.2.1/models/model.py` & `easy_fnc-0.1.2.2/models/model.py`

 * *Files identical despite different names*

### Comparing `easy_fnc-0.1.2.1/models/ollama.py` & `easy_fnc-0.1.2.2/models/ollama.py`

 * *Files identical despite different names*

### Comparing `easy_fnc-0.1.2.1/setup.py` & `easy_fnc-0.1.2.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Read the README.md file and return its contents."""
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 def main():
     setup(
         name='easy_fnc',
-        version='0.1.2.1',
+        version='0.1.2.2',
         description='This package hopes to provide a modular and highly extendable interface to interact with LLMs via (multiple) function calling, easily.',
         long_description=read_readme(),
         long_description_content_type="text/markdown",
         author='Atakan Tekparmak',
         author_email='atakantekerparmak@gmail.com',
         packages=find_packages(),
         install_requires=[
```

