# Comparing `tmp/llama_index_llms_deepinfra-0.0.1.tar.gz` & `tmp/llama_index_llms_deepinfra-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_deepinfra-0.0.1.tar", max compression
+gzip compressed data, was "llama_index_llms_deepinfra-0.1.1.tar", max compression
```

## Comparing `llama_index_llms_deepinfra-0.0.1.tar` & `llama_index_llms_deepinfra-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     3430 2024-05-24 05:42:58.705374 llama_index_llms_deepinfra-0.0.1/README.md
--rw-r--r--   0        0        0       85 2024-05-24 05:42:58.705374 llama_index_llms_deepinfra-0.0.1/llama_index/llms/deepinfra/__init__.py
--rw-r--r--   0        0        0    13431 2024-05-24 05:42:58.705374 llama_index_llms_deepinfra-0.0.1/llama_index/llms/deepinfra/base.py
--rw-r--r--   0        0        0     5054 2024-05-24 05:42:58.705374 llama_index_llms_deepinfra-0.0.1/llama_index/llms/deepinfra/client.py
--rw-r--r--   0        0        0      447 2024-05-24 05:42:58.705374 llama_index_llms_deepinfra-0.0.1/llama_index/llms/deepinfra/constants.py
--rw-r--r--   0        0        0     3911 2024-05-24 05:42:58.705374 llama_index_llms_deepinfra-0.0.1/llama_index/llms/deepinfra/utils.py
--rw-r--r--   0        0        0     1487 2024-05-24 05:42:58.705374 llama_index_llms_deepinfra-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 llama_index_llms_deepinfra-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3430 2024-05-31 14:24:30.627321 llama_index_llms_deepinfra-0.1.1/README.md
+-rw-r--r--   0        0        0       85 2024-05-31 14:24:30.627321 llama_index_llms_deepinfra-0.1.1/llama_index/llms/deepinfra/__init__.py
+-rw-r--r--   0        0        0    13431 2024-05-31 14:24:30.627321 llama_index_llms_deepinfra-0.1.1/llama_index/llms/deepinfra/base.py
+-rw-r--r--   0        0        0     5054 2024-05-31 14:24:30.627321 llama_index_llms_deepinfra-0.1.1/llama_index/llms/deepinfra/client.py
+-rw-r--r--   0        0        0      447 2024-05-31 14:24:30.627321 llama_index_llms_deepinfra-0.1.1/llama_index/llms/deepinfra/constants.py
+-rw-r--r--   0        0        0     3911 2024-05-31 14:24:30.627321 llama_index_llms_deepinfra-0.1.1/llama_index/llms/deepinfra/utils.py
+-rw-r--r--   0        0        0     1504 2024-05-31 14:24:30.627321 llama_index_llms_deepinfra-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4095 1970-01-01 00:00:00.000000 llama_index_llms_deepinfra-0.1.1/PKG-INFO
```

### Comparing `llama_index_llms_deepinfra-0.0.1/README.md` & `llama_index_llms_deepinfra-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_llms_deepinfra-0.0.1/llama_index/llms/deepinfra/base.py` & `llama_index_llms_deepinfra-0.1.1/llama_index/llms/deepinfra/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_deepinfra-0.0.1/llama_index/llms/deepinfra/client.py` & `llama_index_llms_deepinfra-0.1.1/llama_index/llms/deepinfra/client.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_deepinfra-0.0.1/llama_index/llms/deepinfra/utils.py` & `llama_index_llms_deepinfra-0.1.1/llama_index/llms/deepinfra/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_deepinfra-0.0.1/pyproject.toml` & `llama_index_llms_deepinfra-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,30 +8,30 @@
 skip = "*.csv,*.html,*.json,*.jsonl,*.pdf,*.txt,*.ipynb"
 
 [tool.llamahub]
 contains_example = false
 import_path = "llama_index.llms.deepinfra"
 
 [tool.llamahub.class_authors]
-DeepInfraLLM = "ovuruska"
+DeepInfraLLM = "deepinfra"
 
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
-authors = ["Your Name <you@example.com>"]
+authors = ["Oguz Vuruskaneer <oguzvuruskaner@gmail.com>"]
 description = "llama-index llms deepinfra integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-deepinfra"
 readme = "README.md"
-version = "0.0.1"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 llama-index-llms-openai = "^0.1.1"
 aiohttp = "^3.8.1"
```

### Comparing `llama_index_llms_deepinfra-0.0.1/PKG-INFO` & `llama_index_llms_deepinfra-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-deepinfra
-Version: 0.0.1
+Version: 0.1.1
 Summary: llama-index llms deepinfra integration
 License: MIT
-Author: Your Name
-Author-email: you@example.com
+Author: Oguz Vuruskaneer
+Author-email: oguzvuruskaner@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
```

