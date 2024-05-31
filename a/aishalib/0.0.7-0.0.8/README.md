# Comparing `tmp/aishalib-0.0.7.tar.gz` & `tmp/aishalib-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aishalib-0.0.7.tar", last modified: Fri May 31 13:20:10 2024, max compression
+gzip compressed data, was "aishalib-0.0.8.tar", last modified: Fri May 31 13:21:39 2024, max compression
```

## Comparing `aishalib-0.0.7.tar` & `aishalib-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 13:20:10.976089 aishalib-0.0.7/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-29 08:46:39.000000 aishalib-0.0.7/LICENSE
--rw-r--r--   0 man4j     (1000) man4j     (1000)     6728 2024-05-31 13:20:10.976089 aishalib-0.0.7/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)     6130 2024-05-30 15:27:43.000000 aishalib-0.0.7/README.md
--rw-r--r--   0 man4j     (1000) man4j     (1000)      659 2024-05-31 13:19:49.000000 aishalib-0.0.7/pyproject.toml
--rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-05-31 13:20:10.976089 aishalib-0.0.7/setup.cfg
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 13:20:10.972089 aishalib-0.0.7/src/
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 13:20:10.972089 aishalib-0.0.7/src/aishalib/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     3776 2024-05-31 13:19:25.000000 aishalib-0.0.7/src/aishalib/aishalib.py
--rw-r--r--   0 man4j     (1000) man4j     (1000)      922 2024-05-29 09:10:58.000000 aishalib-0.0.7/src/aishalib/llmbackend.py
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 13:20:10.976089 aishalib-0.0.7/src/aishalib.egg-info/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     6728 2024-05-31 13:20:10.000000 aishalib-0.0.7/src/aishalib.egg-info/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)      263 2024-05-31 13:20:10.000000 aishalib-0.0.7/src/aishalib.egg-info/SOURCES.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-05-31 13:20:10.000000 aishalib-0.0.7/src/aishalib.egg-info/dependency_links.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)       35 2024-05-31 13:20:10.000000 aishalib-0.0.7/src/aishalib.egg-info/requires.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)        9 2024-05-31 13:20:10.000000 aishalib-0.0.7/src/aishalib.egg-info/top_level.txt
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 13:21:39.535357 aishalib-0.0.8/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-29 08:46:39.000000 aishalib-0.0.8/LICENSE
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6728 2024-05-31 13:21:39.535357 aishalib-0.0.8/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6130 2024-05-30 15:27:43.000000 aishalib-0.0.8/README.md
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      659 2024-05-31 13:21:33.000000 aishalib-0.0.8/pyproject.toml
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-05-31 13:21:39.535357 aishalib-0.0.8/setup.cfg
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 13:21:39.535357 aishalib-0.0.8/src/
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 13:21:39.535357 aishalib-0.0.8/src/aishalib/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     3781 2024-05-31 13:21:18.000000 aishalib-0.0.8/src/aishalib/aishalib.py
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      922 2024-05-29 09:10:58.000000 aishalib-0.0.8/src/aishalib/llmbackend.py
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 13:21:39.535357 aishalib-0.0.8/src/aishalib.egg-info/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6728 2024-05-31 13:21:39.000000 aishalib-0.0.8/src/aishalib.egg-info/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      263 2024-05-31 13:21:39.000000 aishalib-0.0.8/src/aishalib.egg-info/SOURCES.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-05-31 13:21:39.000000 aishalib-0.0.8/src/aishalib.egg-info/dependency_links.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       35 2024-05-31 13:21:39.000000 aishalib-0.0.8/src/aishalib.egg-info/requires.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)        9 2024-05-31 13:21:39.000000 aishalib-0.0.8/src/aishalib.egg-info/top_level.txt
```

### Comparing `aishalib-0.0.7/LICENSE` & `aishalib-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.7/PKG-INFO` & `aishalib-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aishalib
-Version: 0.0.7
+Version: 0.0.8
 Summary: AI Smart Human Assistant Library
 Author-email: Vladimir Petrukhin <man4j@ya.ru>
 Project-URL: Homepage, https://github.com/Equiron-AI/aishalib
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aishalib-0.0.7/README.md` & `aishalib-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.7/src/aishalib/aishalib.py` & `aishalib-0.0.8/src/aishalib/aishalib.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             self.system_injection_template = "<|system|>\n{system_injection}<|end|>\n"
             prompt_text = self.tokenizer.bos_token + f"<|system|>\n{prompt}<|end|>\n"
             prompt_tokens = self.tokenizer(prompt_text)["input_ids"]
             self.stop_token = "<|end|>"
         else:
             raise RuntimeError("Unknown model: " + config.model_type)
 
-        self.llm_backend = LlamaCppBackend(llm_backend_url, stop_token, max_predict)
+        self.llm_backend = LlamaCppBackend(llm_backend_url, self.stop_token, max_predict)
         self.generation_prompt_tokens = self.tokenizer(self.generation_promp_template)["input_ids"]
         self.tokens = [prompt_tokens]
 
     def sanitize(self, text):
         return text.replace("#", "").replace("<|", "").replace("|>", "")
 
     def add_user_request(self, user_request, system_injection=""):
```

### Comparing `aishalib-0.0.7/src/aishalib/llmbackend.py` & `aishalib-0.0.8/src/aishalib/llmbackend.py`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.7/src/aishalib.egg-info/PKG-INFO` & `aishalib-0.0.8/src/aishalib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aishalib
-Version: 0.0.7
+Version: 0.0.8
 Summary: AI Smart Human Assistant Library
 Author-email: Vladimir Petrukhin <man4j@ya.ru>
 Project-URL: Homepage, https://github.com/Equiron-AI/aishalib
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

