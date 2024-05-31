# Comparing `tmp/easy_fnc-0.1.3.tar.gz` & `tmp/easy_fnc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_fnc-0.1.3.tar", last modified: Fri May 31 08:29:02 2024, max compression
+gzip compressed data, was "easy_fnc-0.1.4.tar", last modified: Fri May 31 08:29:31 2024, max compression
```

## Comparing `easy_fnc-0.1.3.tar` & `easy_fnc-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:29:02.906355 easy_fnc-0.1.3/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     5802 2024-05-31 08:29:02.906138 easy_fnc-0.1.3/PKG-INFO
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     5397 2024-05-31 08:16:58.000000 easy_fnc-0.1.3/README.md
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:29:02.905899 easy_fnc-0.1.3/easy_fnc.egg-info/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     5802 2024-05-31 08:29:02.000000 easy_fnc-0.1.3/easy_fnc.egg-info/PKG-INFO
--rw-r--r--   0 atakantekparmak   (501) staff       (20)      229 2024-05-31 08:29:02.000000 easy_fnc-0.1.3/easy_fnc.egg-info/SOURCES.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        1 2024-05-31 08:29:02.000000 easy_fnc-0.1.3/easy_fnc.egg-info/dependency_links.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)       15 2024-05-31 08:29:02.000000 easy_fnc-0.1.3/easy_fnc.egg-info/requires.txt
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        7 2024-05-31 08:29:02.000000 easy_fnc-0.1.3/easy_fnc.egg-info/top_level.txt
-drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:29:02.905697 easy_fnc-0.1.3/models/
--rw-r--r--   0 atakantekparmak   (501) staff       (20)        0 2024-05-02 07:40:29.000000 easy_fnc-0.1.3/models/__init__.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     1119 2024-05-30 12:40:49.000000 easy_fnc-0.1.3/models/model.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)     4439 2024-05-30 12:39:08.000000 easy_fnc-0.1.3/models/ollama.py
--rw-r--r--   0 atakantekparmak   (501) staff       (20)       38 2024-05-31 08:29:02.906415 easy_fnc-0.1.3/setup.cfg
--rw-r--r--   0 atakantekparmak   (501) staff       (20)      839 2024-05-31 08:28:57.000000 easy_fnc-0.1.3/setup.py
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:29:31.675021 easy_fnc-0.1.4/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     5779 2024-05-31 08:29:31.674725 easy_fnc-0.1.4/PKG-INFO
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     5397 2024-05-31 08:16:58.000000 easy_fnc-0.1.4/README.md
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:29:31.674432 easy_fnc-0.1.4/easy_fnc.egg-info/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     5779 2024-05-31 08:29:31.000000 easy_fnc-0.1.4/easy_fnc.egg-info/PKG-INFO
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)      229 2024-05-31 08:29:31.000000 easy_fnc-0.1.4/easy_fnc.egg-info/SOURCES.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        1 2024-05-31 08:29:31.000000 easy_fnc-0.1.4/easy_fnc.egg-info/dependency_links.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        7 2024-05-31 08:29:31.000000 easy_fnc-0.1.4/easy_fnc.egg-info/requires.txt
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        7 2024-05-31 08:29:31.000000 easy_fnc-0.1.4/easy_fnc.egg-info/top_level.txt
+drwxr-xr-x   0 atakantekparmak   (501) staff       (20)        0 2024-05-31 08:29:31.674113 easy_fnc-0.1.4/models/
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)        0 2024-05-02 07:40:29.000000 easy_fnc-0.1.4/models/__init__.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     1119 2024-05-30 12:40:49.000000 easy_fnc-0.1.4/models/model.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)     4439 2024-05-30 12:39:08.000000 easy_fnc-0.1.4/models/ollama.py
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)       38 2024-05-31 08:29:31.675082 easy_fnc-0.1.4/setup.cfg
+-rw-r--r--   0 atakantekparmak   (501) staff       (20)      816 2024-05-31 08:29:30.000000 easy_fnc-0.1.4/setup.py
```

### Comparing `easy_fnc-0.1.3/PKG-INFO` & `easy_fnc-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: easy_fnc
-Version: 0.1.3
+Version: 0.1.4
 Summary: This package hopes to provide a modular and highly extendable interface to interact with LLMs via (multiple) function calling, easily.
 Home-page: https://github.com/AtakanTekparmak/easy_fnc
 Author: Atakan Tekparmak
 Author-email: atakantekerparmak@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: ollama
-Requires-Dist: tomllib
 
 # Easy FNC (Function Calling) Package
 
 The `easy_fnc` package provides a framework for generating responses using AI models and executing user-defined functions. It allows users to define their own functions and integrate them with AI models to create interactive and customizable applications.
 
 ## Installation
```

### Comparing `easy_fnc-0.1.3/README.md` & `easy_fnc-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `easy_fnc-0.1.3/easy_fnc.egg-info/PKG-INFO` & `easy_fnc-0.1.4/easy_fnc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: easy_fnc
-Version: 0.1.3
+Version: 0.1.4
 Summary: This package hopes to provide a modular and highly extendable interface to interact with LLMs via (multiple) function calling, easily.
 Home-page: https://github.com/AtakanTekparmak/easy_fnc
 Author: Atakan Tekparmak
 Author-email: atakantekerparmak@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: ollama
-Requires-Dist: tomllib
 
 # Easy FNC (Function Calling) Package
 
 The `easy_fnc` package provides a framework for generating responses using AI models and executing user-defined functions. It allows users to define their own functions and integrate them with AI models to create interactive and customizable applications.
 
 ## Installation
```

### Comparing `easy_fnc-0.1.3/models/model.py` & `easy_fnc-0.1.4/models/model.py`

 * *Files identical despite different names*

### Comparing `easy_fnc-0.1.3/models/ollama.py` & `easy_fnc-0.1.4/models/ollama.py`

 * *Files identical despite different names*

### Comparing `easy_fnc-0.1.3/setup.py` & `easy_fnc-0.1.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,22 @@
     """Read the README.md file and return its contents."""
     with open("README.md", "r", encoding="utf-8") as fh:
         return fh.read()
 
 def main():
     setup(
         name='easy_fnc',
-        version='0.1.3',
+        version='0.1.4',
         description='This package hopes to provide a modular and highly extendable interface to interact with LLMs via (multiple) function calling, easily.',
         long_description=read_readme(),
         long_description_content_type="text/markdown",
         author='Atakan Tekparmak',
         author_email='atakantekerparmak@gmail.com',
         url="https://github.com/AtakanTekparmak/easy_fnc",
         packages=find_packages(),
         install_requires=[
             "ollama",
-            "tomllib",
         ],
     )
 
 if __name__ == "__main__":
     main()
```

