# Comparing `tmp/aishalib-0.0.8.tar.gz` & `tmp/aishalib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aishalib-0.0.8.tar", last modified: Fri May 31 13:21:39 2024, max compression
+gzip compressed data, was "aishalib-0.0.9.tar", last modified: Fri May 31 16:39:08 2024, max compression
```

## Comparing `aishalib-0.0.8.tar` & `aishalib-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 13:21:39.535357 aishalib-0.0.8/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-29 08:46:39.000000 aishalib-0.0.8/LICENSE
--rw-r--r--   0 man4j     (1000) man4j     (1000)     6728 2024-05-31 13:21:39.535357 aishalib-0.0.8/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)     6130 2024-05-30 15:27:43.000000 aishalib-0.0.8/README.md
--rw-r--r--   0 man4j     (1000) man4j     (1000)      659 2024-05-31 13:21:33.000000 aishalib-0.0.8/pyproject.toml
--rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-05-31 13:21:39.535357 aishalib-0.0.8/setup.cfg
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 13:21:39.535357 aishalib-0.0.8/src/
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 13:21:39.535357 aishalib-0.0.8/src/aishalib/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     3781 2024-05-31 13:21:18.000000 aishalib-0.0.8/src/aishalib/aishalib.py
--rw-r--r--   0 man4j     (1000) man4j     (1000)      922 2024-05-29 09:10:58.000000 aishalib-0.0.8/src/aishalib/llmbackend.py
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 13:21:39.535357 aishalib-0.0.8/src/aishalib.egg-info/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     6728 2024-05-31 13:21:39.000000 aishalib-0.0.8/src/aishalib.egg-info/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)      263 2024-05-31 13:21:39.000000 aishalib-0.0.8/src/aishalib.egg-info/SOURCES.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-05-31 13:21:39.000000 aishalib-0.0.8/src/aishalib.egg-info/dependency_links.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)       35 2024-05-31 13:21:39.000000 aishalib-0.0.8/src/aishalib.egg-info/requires.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)        9 2024-05-31 13:21:39.000000 aishalib-0.0.8/src/aishalib.egg-info/top_level.txt
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 16:39:08.719200 aishalib-0.0.9/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-29 08:46:39.000000 aishalib-0.0.9/LICENSE
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6728 2024-05-31 16:39:08.719200 aishalib-0.0.9/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6130 2024-05-30 15:27:43.000000 aishalib-0.0.9/README.md
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      659 2024-05-31 16:38:59.000000 aishalib-0.0.9/pyproject.toml
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-05-31 16:39:08.719200 aishalib-0.0.9/setup.cfg
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 16:39:08.715200 aishalib-0.0.9/src/
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 16:39:08.715200 aishalib-0.0.9/src/aishalib/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     3906 2024-05-31 16:38:06.000000 aishalib-0.0.9/src/aishalib/aishalib.py
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      922 2024-05-29 09:10:58.000000 aishalib-0.0.9/src/aishalib/llmbackend.py
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 16:39:08.719200 aishalib-0.0.9/src/aishalib.egg-info/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6728 2024-05-31 16:39:08.000000 aishalib-0.0.9/src/aishalib.egg-info/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      263 2024-05-31 16:39:08.000000 aishalib-0.0.9/src/aishalib.egg-info/SOURCES.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-05-31 16:39:08.000000 aishalib-0.0.9/src/aishalib.egg-info/dependency_links.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       35 2024-05-31 16:39:08.000000 aishalib-0.0.9/src/aishalib.egg-info/requires.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)        9 2024-05-31 16:39:08.000000 aishalib-0.0.9/src/aishalib.egg-info/top_level.txt
```

### Comparing `aishalib-0.0.8/LICENSE` & `aishalib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.8/PKG-INFO` & `aishalib-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aishalib
-Version: 0.0.8
+Version: 0.0.9
 Summary: AI Smart Human Assistant Library
 Author-email: Vladimir Petrukhin <man4j@ya.ru>
 Project-URL: Homepage, https://github.com/Equiron-AI/aishalib
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aishalib-0.0.8/README.md` & `aishalib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.8/pyproject.toml` & `aishalib-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aishalib"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Vladimir Petrukhin", email="man4j@ya.ru" },
 ]
 description = "AI Smart Human Assistant Library"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `aishalib-0.0.8/src/aishalib/aishalib.py` & `aishalib-0.0.9/src/aishalib/aishalib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import os
 import json
+import logging
 from transformers import AutoTokenizer, AutoConfig
 from aishalib.llmbackend import LlamaCppBackend
 
 
+logger = logging.getLogger(__name__)
+
+
 class Aisha:
     def __init__(self, llm_backend_url, base_model, max_context=4096, max_predict=256, prompt="", prompt_file=""):
         self.llm_backend_url = llm_backend_url
         self.tokenizer = AutoTokenizer.from_pretrained(base_model, add_bos_token=False)
         self.max_context = max_context
         self.max_predict = max_predict
 
@@ -33,14 +37,15 @@
             self.stop_token = "<|end|>"
         else:
             raise RuntimeError("Unknown model: " + config.model_type)
 
         self.llm_backend = LlamaCppBackend(llm_backend_url, self.stop_token, max_predict)
         self.generation_prompt_tokens = self.tokenizer(self.generation_promp_template)["input_ids"]
         self.tokens = [prompt_tokens]
+        logger.info(f"System prompt size: " + str(len(prompt_tokens)))
 
     def sanitize(self, text):
         return text.replace("#", "").replace("<|", "").replace("|>", "")
 
     def add_user_request(self, user_request, system_injection=""):
         text = self.user_req_template.replace("{user_req}", self.sanitize(user_request.strip()))
         if system_injection:
```

### Comparing `aishalib-0.0.8/src/aishalib/llmbackend.py` & `aishalib-0.0.9/src/aishalib/llmbackend.py`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.8/src/aishalib.egg-info/PKG-INFO` & `aishalib-0.0.9/src/aishalib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aishalib
-Version: 0.0.8
+Version: 0.0.9
 Summary: AI Smart Human Assistant Library
 Author-email: Vladimir Petrukhin <man4j@ya.ru>
 Project-URL: Homepage, https://github.com/Equiron-AI/aishalib
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

