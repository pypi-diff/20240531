# Comparing `tmp/prompt_learner-0.3.1.tar.gz` & `tmp/prompt_learner-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_learner-0.3.1.tar", max compression
+gzip compressed data, was "prompt_learner-0.3.2.tar", max compression
```

## Comparing `prompt_learner-0.3.1.tar` & `prompt_learner-0.3.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2288 2024-05-28 21:05:53.126497 prompt_learner-0.3.1/README.md
--rw-r--r--   0        0        0     6148 2024-05-24 20:42:17.913011 prompt_learner-0.3.1/prompt_learner/.DS_Store
--rw-r--r--   0        0        0       28 2024-05-24 20:42:17.913126 prompt_learner-0.3.1/prompt_learner/adapters/__init__.py
--rw-r--r--   0        0        0     1145 2024-05-30 22:27:02.624759 prompt_learner-0.3.1/prompt_learner/adapters/adapter.py
--rw-r--r--   0        0        0      817 2024-05-28 21:04:11.862612 prompt_learner-0.3.1/prompt_learner/adapters/anthropic.py
--rw-r--r--   0        0        0      757 2024-05-28 19:57:13.623830 prompt_learner-0.3.1/prompt_learner/adapters/llama.py
--rw-r--r--   0        0        0     1076 2024-05-30 21:49:22.419061 prompt_learner-0.3.1/prompt_learner/adapters/ollama_local.py
--rw-r--r--   0        0        0      757 2024-05-28 19:57:09.541479 prompt_learner-0.3.1/prompt_learner/adapters/openai.py
--rw-r--r--   0        0        0     1278 2024-05-24 20:42:17.913806 prompt_learner-0.3.1/prompt_learner/evals/metrics/accuracy.py
--rw-r--r--   0        0        0       29 2024-05-24 20:42:17.913956 prompt_learner-0.3.1/prompt_learner/examples/__init__.py
--rw-r--r--   0        0        0      316 2024-05-24 20:42:17.914044 prompt_learner-0.3.1/prompt_learner/examples/example.py
--rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914130 prompt_learner-0.3.1/prompt_learner/examples/manipulation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914236 prompt_learner-0.3.1/prompt_learner/inference/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914292 prompt_learner-0.3.1/prompt_learner/inference/predict.py
--rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914393 prompt_learner-0.3.1/prompt_learner/optimizers/__init__.py
--rw-r--r--   0        0        0     2999 2024-05-29 00:12:25.436308 prompt_learner-0.3.1/prompt_learner/optimizers/grid_search.py
--rw-r--r--   0        0        0      539 2024-05-28 21:03:53.376070 prompt_learner-0.3.1/prompt_learner/optimizers/optimizer.py
--rw-r--r--   0        0        0       26 2024-05-24 20:42:17.914611 prompt_learner-0.3.1/prompt_learner/prompts/__init__.py
--rw-r--r--   0        0        0      597 2024-05-24 20:42:17.914685 prompt_learner-0.3.1/prompt_learner/prompts/cot.py
--rw-r--r--   0        0        0     1114 2024-05-24 20:42:17.914765 prompt_learner-0.3.1/prompt_learner/prompts/prompt.py
--rw-r--r--   0        0        0       30 2024-05-24 20:42:17.914890 prompt_learner-0.3.1/prompt_learner/selectors/__init__.py
--rw-r--r--   0        0        0     1635 2024-05-25 21:40:52.339141 prompt_learner-0.3.1/prompt_learner/selectors/diverse_sampler.py
--rw-r--r--   0        0        0      599 2024-05-25 21:40:21.427745 prompt_learner-0.3.1/prompt_learner/selectors/random_sampler.py
--rw-r--r--   0        0        0      880 2024-05-26 04:26:50.424797 prompt_learner-0.3.1/prompt_learner/selectors/selector.py
--rw-r--r--   0        0        0      888 2024-05-24 20:42:17.915207 prompt_learner-0.3.1/prompt_learner/selectors/stratified_sampler.py
--rw-r--r--   0        0        0       22 2024-05-24 20:42:17.915348 prompt_learner-0.3.1/prompt_learner/tasks/__init__.py
--rw-r--r--   0        0        0      625 2024-05-24 20:42:17.915451 prompt_learner-0.3.1/prompt_learner/tasks/classification.py
--rw-r--r--   0        0        0      400 2024-05-24 20:42:17.915556 prompt_learner-0.3.1/prompt_learner/tasks/sql_generation.py
--rw-r--r--   0        0        0      529 2024-05-24 20:42:17.915946 prompt_learner-0.3.1/prompt_learner/tasks/tagging.py
--rw-r--r--   0        0        0     1589 2024-05-24 20:42:17.916465 prompt_learner-0.3.1/prompt_learner/tasks/task.py
--rw-r--r--   0        0        0       30 2024-05-24 20:42:17.916660 prompt_learner-0.3.1/prompt_learner/templates/__init__.py
--rw-r--r--   0        0        0     2805 2024-05-28 21:04:48.274343 prompt_learner-0.3.1/prompt_learner/templates/markdown.py
--rw-r--r--   0        0        0     1638 2024-05-26 04:26:03.988721 prompt_learner-0.3.1/prompt_learner/templates/template.py
--rw-r--r--   0        0        0     2906 2024-05-28 20:19:06.403920 prompt_learner-0.3.1/prompt_learner/templates/xml.py
--rw-r--r--   0        0        0     3373 2024-05-24 20:42:17.917199 prompt_learner-0.3.1/prompt_learner/translator/translate.py
--rw-r--r--   0        0        0      485 2024-05-30 22:27:59.034869 prompt_learner-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 prompt_learner-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2288 2024-05-28 21:05:53.126497 prompt_learner-0.3.2/README.md
+-rw-r--r--   0        0        0     6148 2024-05-24 20:42:17.913011 prompt_learner-0.3.2/prompt_learner/.DS_Store
+-rw-r--r--   0        0        0       28 2024-05-24 20:42:17.913126 prompt_learner-0.3.2/prompt_learner/adapters/__init__.py
+-rw-r--r--   0        0        0     1179 2024-05-30 22:59:33.687050 prompt_learner-0.3.2/prompt_learner/adapters/adapter.py
+-rw-r--r--   0        0        0      817 2024-05-28 21:04:11.862612 prompt_learner-0.3.2/prompt_learner/adapters/anthropic.py
+-rw-r--r--   0        0        0      757 2024-05-28 19:57:13.623830 prompt_learner-0.3.2/prompt_learner/adapters/llama.py
+-rw-r--r--   0        0        0     1076 2024-05-30 21:49:22.419061 prompt_learner-0.3.2/prompt_learner/adapters/ollama_local.py
+-rw-r--r--   0        0        0      757 2024-05-28 19:57:09.541479 prompt_learner-0.3.2/prompt_learner/adapters/openai.py
+-rw-r--r--   0        0        0     1278 2024-05-24 20:42:17.913806 prompt_learner-0.3.2/prompt_learner/evals/metrics/accuracy.py
+-rw-r--r--   0        0        0       29 2024-05-24 20:42:17.913956 prompt_learner-0.3.2/prompt_learner/examples/__init__.py
+-rw-r--r--   0        0        0      316 2024-05-24 20:42:17.914044 prompt_learner-0.3.2/prompt_learner/examples/example.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914130 prompt_learner-0.3.2/prompt_learner/examples/manipulation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914236 prompt_learner-0.3.2/prompt_learner/inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914292 prompt_learner-0.3.2/prompt_learner/inference/predict.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914393 prompt_learner-0.3.2/prompt_learner/optimizers/__init__.py
+-rw-r--r--   0        0        0     2999 2024-05-29 00:12:25.436308 prompt_learner-0.3.2/prompt_learner/optimizers/grid_search.py
+-rw-r--r--   0        0        0      539 2024-05-28 21:03:53.376070 prompt_learner-0.3.2/prompt_learner/optimizers/optimizer.py
+-rw-r--r--   0        0        0       26 2024-05-24 20:42:17.914611 prompt_learner-0.3.2/prompt_learner/prompts/__init__.py
+-rw-r--r--   0        0        0      597 2024-05-24 20:42:17.914685 prompt_learner-0.3.2/prompt_learner/prompts/cot.py
+-rw-r--r--   0        0        0     1114 2024-05-24 20:42:17.914765 prompt_learner-0.3.2/prompt_learner/prompts/prompt.py
+-rw-r--r--   0        0        0       30 2024-05-24 20:42:17.914890 prompt_learner-0.3.2/prompt_learner/selectors/__init__.py
+-rw-r--r--   0        0        0     1635 2024-05-25 21:40:52.339141 prompt_learner-0.3.2/prompt_learner/selectors/diverse_sampler.py
+-rw-r--r--   0        0        0      599 2024-05-25 21:40:21.427745 prompt_learner-0.3.2/prompt_learner/selectors/random_sampler.py
+-rw-r--r--   0        0        0      880 2024-05-26 04:26:50.424797 prompt_learner-0.3.2/prompt_learner/selectors/selector.py
+-rw-r--r--   0        0        0      888 2024-05-24 20:42:17.915207 prompt_learner-0.3.2/prompt_learner/selectors/stratified_sampler.py
+-rw-r--r--   0        0        0       22 2024-05-24 20:42:17.915348 prompt_learner-0.3.2/prompt_learner/tasks/__init__.py
+-rw-r--r--   0        0        0      625 2024-05-24 20:42:17.915451 prompt_learner-0.3.2/prompt_learner/tasks/classification.py
+-rw-r--r--   0        0        0      400 2024-05-24 20:42:17.915556 prompt_learner-0.3.2/prompt_learner/tasks/sql_generation.py
+-rw-r--r--   0        0        0      529 2024-05-24 20:42:17.915946 prompt_learner-0.3.2/prompt_learner/tasks/tagging.py
+-rw-r--r--   0        0        0     1589 2024-05-24 20:42:17.916465 prompt_learner-0.3.2/prompt_learner/tasks/task.py
+-rw-r--r--   0        0        0       30 2024-05-24 20:42:17.916660 prompt_learner-0.3.2/prompt_learner/templates/__init__.py
+-rw-r--r--   0        0        0     2805 2024-05-28 21:04:48.274343 prompt_learner-0.3.2/prompt_learner/templates/markdown.py
+-rw-r--r--   0        0        0     1638 2024-05-26 04:26:03.988721 prompt_learner-0.3.2/prompt_learner/templates/template.py
+-rw-r--r--   0        0        0     2906 2024-05-28 20:19:06.403920 prompt_learner-0.3.2/prompt_learner/templates/xml.py
+-rw-r--r--   0        0        0     3373 2024-05-24 20:42:17.917199 prompt_learner-0.3.2/prompt_learner/translator/translate.py
+-rw-r--r--   0        0        0      485 2024-05-30 23:00:07.919274 prompt_learner-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 prompt_learner-0.3.2/PKG-INFO
```

### Comparing `prompt_learner-0.3.1/README.md` & `prompt_learner-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/.DS_Store` & `prompt_learner-0.3.2/prompt_learner/.DS_Store`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/adapters/adapter.py` & `prompt_learner-0.3.2/prompt_learner/adapters/adapter.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,17 +16,18 @@
         content = content.replace("'", "")
         #if xml tag is not present, it will return the content as it is
         content = self.extract_xml_tag(content, "label")
         return content
 
     def extract_xml_tag(self, data: str, tag: str) -> str:
         """Extracts the data between the XML tags."""
+        open_tag = "<" + tag + ">"
         close_tag = "</" + tag + ">"
-        try:#since we prefill response with opening tag, only closing tag is checked
-            data = data.split(close_tag)[0].strip()
-        except IndexError:
-            pass
+        #replace open tag and close tag with empty string
+        data = re.sub(open_tag, "", data)
+        data = re.sub(close_tag, "", data)
+        #replace new line characters
         data = re.sub(r"^\\n|\\n$", "", data)
         return data
 
     def __repr__(self):
         return "Generic Adapter"
```

### Comparing `prompt_learner-0.3.1/prompt_learner/adapters/anthropic.py` & `prompt_learner-0.3.2/prompt_learner/adapters/anthropic.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/adapters/llama.py` & `prompt_learner-0.3.2/prompt_learner/adapters/llama.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/adapters/ollama_local.py` & `prompt_learner-0.3.2/prompt_learner/adapters/ollama_local.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/adapters/openai.py` & `prompt_learner-0.3.2/prompt_learner/adapters/openai.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/evals/metrics/accuracy.py` & `prompt_learner-0.3.2/prompt_learner/evals/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/optimizers/grid_search.py` & `prompt_learner-0.3.2/prompt_learner/optimizers/grid_search.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/optimizers/optimizer.py` & `prompt_learner-0.3.2/prompt_learner/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/prompts/cot.py` & `prompt_learner-0.3.2/prompt_learner/prompts/cot.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/prompts/prompt.py` & `prompt_learner-0.3.2/prompt_learner/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/selectors/diverse_sampler.py` & `prompt_learner-0.3.2/prompt_learner/selectors/diverse_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/selectors/random_sampler.py` & `prompt_learner-0.3.2/prompt_learner/selectors/random_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/selectors/selector.py` & `prompt_learner-0.3.2/prompt_learner/selectors/selector.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/selectors/stratified_sampler.py` & `prompt_learner-0.3.2/prompt_learner/selectors/stratified_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/tasks/classification.py` & `prompt_learner-0.3.2/prompt_learner/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/tasks/tagging.py` & `prompt_learner-0.3.2/prompt_learner/tasks/tagging.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/tasks/task.py` & `prompt_learner-0.3.2/prompt_learner/tasks/task.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/templates/markdown.py` & `prompt_learner-0.3.2/prompt_learner/templates/markdown.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/templates/template.py` & `prompt_learner-0.3.2/prompt_learner/templates/template.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/templates/xml.py` & `prompt_learner-0.3.2/prompt_learner/templates/xml.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/prompt_learner/translator/translate.py` & `prompt_learner-0.3.2/prompt_learner/translator/translate.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.3.1/PKG-INFO` & `prompt_learner-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-learner
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 Author: Aditya Lahiri
 Author-email: adityalahiri13@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

