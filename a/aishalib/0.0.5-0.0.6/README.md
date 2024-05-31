# Comparing `tmp/aishalib-0.0.5.tar.gz` & `tmp/aishalib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aishalib-0.0.5.tar", last modified: Thu May 30 15:28:13 2024, max compression
+gzip compressed data, was "aishalib-0.0.6.tar", last modified: Fri May 31 09:09:12 2024, max compression
```

## Comparing `aishalib-0.0.5.tar` & `aishalib-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 15:28:13.683395 aishalib-0.0.5/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-29 08:46:39.000000 aishalib-0.0.5/LICENSE
--rw-r--r--   0 man4j     (1000) man4j     (1000)     6728 2024-05-30 15:28:13.683395 aishalib-0.0.5/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)     6130 2024-05-30 15:27:43.000000 aishalib-0.0.5/README.md
--rw-r--r--   0 man4j     (1000) man4j     (1000)      659 2024-05-30 15:28:06.000000 aishalib-0.0.5/pyproject.toml
--rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-05-30 15:28:13.683395 aishalib-0.0.5/setup.cfg
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 15:28:13.683395 aishalib-0.0.5/src/
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 15:28:13.683395 aishalib-0.0.5/src/aishalib/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     3848 2024-05-29 10:48:48.000000 aishalib-0.0.5/src/aishalib/aishalib.py
--rw-r--r--   0 man4j     (1000) man4j     (1000)      922 2024-05-29 09:10:58.000000 aishalib-0.0.5/src/aishalib/llmbackend.py
-drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-30 15:28:13.683395 aishalib-0.0.5/src/aishalib.egg-info/
--rw-r--r--   0 man4j     (1000) man4j     (1000)     6728 2024-05-30 15:28:13.000000 aishalib-0.0.5/src/aishalib.egg-info/PKG-INFO
--rw-r--r--   0 man4j     (1000) man4j     (1000)      263 2024-05-30 15:28:13.000000 aishalib-0.0.5/src/aishalib.egg-info/SOURCES.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-05-30 15:28:13.000000 aishalib-0.0.5/src/aishalib.egg-info/dependency_links.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)       35 2024-05-30 15:28:13.000000 aishalib-0.0.5/src/aishalib.egg-info/requires.txt
--rw-r--r--   0 man4j     (1000) man4j     (1000)        9 2024-05-30 15:28:13.000000 aishalib-0.0.5/src/aishalib.egg-info/top_level.txt
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 09:09:12.663012 aishalib-0.0.6/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     1074 2024-05-29 08:46:39.000000 aishalib-0.0.6/LICENSE
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6728 2024-05-31 09:09:12.663012 aishalib-0.0.6/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6130 2024-05-30 15:27:43.000000 aishalib-0.0.6/README.md
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      659 2024-05-31 09:08:59.000000 aishalib-0.0.6/pyproject.toml
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       38 2024-05-31 09:09:12.663012 aishalib-0.0.6/setup.cfg
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 09:09:12.663012 aishalib-0.0.6/src/
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 09:09:12.663012 aishalib-0.0.6/src/aishalib/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     3775 2024-05-31 09:05:16.000000 aishalib-0.0.6/src/aishalib/aishalib.py
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      922 2024-05-29 09:10:58.000000 aishalib-0.0.6/src/aishalib/llmbackend.py
+drwxr-xr-x   0 man4j     (1000) man4j     (1000)        0 2024-05-31 09:09:12.663012 aishalib-0.0.6/src/aishalib.egg-info/
+-rw-r--r--   0 man4j     (1000) man4j     (1000)     6728 2024-05-31 09:09:12.000000 aishalib-0.0.6/src/aishalib.egg-info/PKG-INFO
+-rw-r--r--   0 man4j     (1000) man4j     (1000)      263 2024-05-31 09:09:12.000000 aishalib-0.0.6/src/aishalib.egg-info/SOURCES.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)        1 2024-05-31 09:09:12.000000 aishalib-0.0.6/src/aishalib.egg-info/dependency_links.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)       35 2024-05-31 09:09:12.000000 aishalib-0.0.6/src/aishalib.egg-info/requires.txt
+-rw-r--r--   0 man4j     (1000) man4j     (1000)        9 2024-05-31 09:09:12.000000 aishalib-0.0.6/src/aishalib.egg-info/top_level.txt
```

### Comparing `aishalib-0.0.5/LICENSE` & `aishalib-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.5/PKG-INFO` & `aishalib-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aishalib
-Version: 0.0.5
+Version: 0.0.6
 Summary: AI Smart Human Assistant Library
 Author-email: Vladimir Petrukhin <man4j@ya.ru>
 Project-URL: Homepage, https://github.com/Equiron-AI/aishalib
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aishalib-0.0.5/README.md` & `aishalib-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.5/pyproject.toml` & `aishalib-0.0.6/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aishalib"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Vladimir Petrukhin", email="man4j@ya.ru" },
 ]
 description = "AI Smart Human Assistant Library"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `aishalib-0.0.5/src/aishalib/aishalib.py` & `aishalib-0.0.6/src/aishalib/aishalib.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,26 +21,25 @@
             self.generation_promp_template = "<|START_OF_TURN_TOKEN|><|CHATBOT_TOKEN|>"
             self.user_req_template = "<|START_OF_TURN_TOKEN|><|USER_TOKEN|>{user_req}<|END_OF_TURN_TOKEN|>"
             self.system_injection_template = "<|START_OF_TURN_TOKEN|><|SYSTEM_TOKEN|>{system_injection}<|END_OF_TURN_TOKEN|>"
             inst = [{"role": "system", "content": prompt}]
             prompt_tokens = self.tokenizer.apply_chat_template(inst)
             stop_token = self.tokenizer.eos_token
         elif config.model_type == "phi3":
-            self.generation_promp_template = "<|assistant|>"
-            self.user_req_template = "<|user|>{user_req}<|end|>"
-            self.system_injection_template = "<|user|>{system_injection}<|end|>"
-            inst = [{"role": "user", "content": prompt}]
-            prompt_tokens = [self.tokenizer.bos_token_id] + self.tokenizer.apply_chat_template(inst)
+            self.generation_promp_template = "<|assistant|>\n"
+            self.user_req_template = "<|user|>\n{user_req}<|end|>\n"
+            self.system_injection_template = "<|system|>\n{system_injection}<|end|>\n"
+            prompt_text = self.tokenizer.bos_token + f"<|system|>\n{prompt}<|end|>\n"
+            prompt_tokens = self.tokenizer(prompt_text)["input_ids"]
             stop_token = "<|end|>"
         else:
             raise RuntimeError("Unknown model: " + config.model_type)
 
         self.llm_backend = LlamaCppBackend(llm_backend_url, stop_token, max_predict)
         self.generation_prompt_tokens = self.tokenizer(self.generation_promp_template)["input_ids"]
-        self.instructions_len = len(inst)
         self.tokens = [prompt_tokens]
 
     def sanitize(self, text):
         return text.replace("#", "").replace("<|", "").replace("|>", "")
 
     def add_user_request(self, user_request, system_injection=""):
         text = self.user_req_template.replace("{user_req}", self.sanitize(user_request.strip()))
@@ -75,9 +74,9 @@
         with open(file_name, "w") as f:
             json.dump(self.tokens, f)
 
     def _cut_context(self):
         busy_tokens = len(sum(self.tokens, []))
         free_tokens = self.max_context - busy_tokens
         while free_tokens < self.max_predict:
-            free_tokens += len(self.tokens[self.instructions_len])
-            del self.tokens[self.instructions_len]
+            free_tokens += len(self.tokens[1])
+            del self.tokens[1]
```

### Comparing `aishalib-0.0.5/src/aishalib/llmbackend.py` & `aishalib-0.0.6/src/aishalib/llmbackend.py`

 * *Files identical despite different names*

### Comparing `aishalib-0.0.5/src/aishalib.egg-info/PKG-INFO` & `aishalib-0.0.6/src/aishalib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aishalib
-Version: 0.0.5
+Version: 0.0.6
 Summary: AI Smart Human Assistant Library
 Author-email: Vladimir Petrukhin <man4j@ya.ru>
 Project-URL: Homepage, https://github.com/Equiron-AI/aishalib
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
```

