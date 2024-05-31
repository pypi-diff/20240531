# Comparing `tmp/lambda_genai_util-0.0.2.tar.gz` & `tmp/lambda_genai_util-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambda_genai_util-0.0.2.tar", last modified: Fri May 31 11:53:08 2024, max compression
+gzip compressed data, was "lambda_genai_util-0.0.3.tar", last modified: Fri May 31 12:16:54 2024, max compression
```

## Comparing `lambda_genai_util-0.0.2.tar` & `lambda_genai_util-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 11:53:08.467369 lambda_genai_util-0.0.2/
--rw-rw-rw-   0        0        0     1089 2024-05-30 13:47:39.000000 lambda_genai_util-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1712 2024-05-31 11:53:08.466369 lambda_genai_util-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      611 2024-05-31 11:52:01.000000 lambda_genai_util-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-31 11:53:08.467369 lambda_genai_util-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-31 11:53:08.442517 lambda_genai_util-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-31 11:53:08.456631 lambda_genai_util-0.0.2/src/lambda_genai_util/
--rw-rw-rw-   0        0        0     1453 2024-05-31 10:56:27.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/AnthropicBedrockUtil.py
--rw-rw-rw-   0        0        0     1660 2024-05-31 10:56:38.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/AwsTitanBedrockUtil.py
--rw-rw-rw-   0        0        0      182 2024-05-31 05:52:08.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/BedrockUtil.py
--rw-rw-rw-   0        0        0     1390 2024-05-31 10:56:44.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/CohereBedrockUtil.py
--rw-rw-rw-   0        0        0     1233 2024-05-31 10:56:49.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/MetaBedrockUtil.py
--rw-rw-rw-   0        0        0     1175 2024-05-31 10:56:54.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/MistralBedrockUtil.py
--rw-rw-rw-   0        0        0     1345 2024-05-31 11:52:25.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/TextCompletionUtil.py
--rw-rw-rw-   0        0        0        0 2024-05-31 10:47:21.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/__init__.py
--rw-rw-rw-   0        0        0     1039 2024-05-31 05:52:08.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/model_map.py
--rw-rw-rw-   0        0        0     2026 2024-05-31 11:52:42.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/prompt_service.py
-drwxrwxrwx   0        0        0        0 2024-05-31 11:53:08.465369 lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/
--rw-rw-rw-   0        0        0     1712 2024-05-31 11:53:08.000000 lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      659 2024-05-31 11:53:08.000000 lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 11:53:08.000000 lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-31 11:53:08.000000 lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-31 11:53:08.000000 lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 12:16:54.106489 lambda_genai_util-0.0.3/
+-rw-rw-rw-   0        0        0     1089 2024-05-30 13:47:39.000000 lambda_genai_util-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1712 2024-05-31 12:16:54.106489 lambda_genai_util-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2024-05-31 12:15:34.000000 lambda_genai_util-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 12:16:54.107508 lambda_genai_util-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 12:16:54.080325 lambda_genai_util-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-31 12:16:54.091330 lambda_genai_util-0.0.3/src/lambda_genai_util/
+-rw-rw-rw-   0        0        0     1471 2024-05-31 12:16:33.000000 lambda_genai_util-0.0.3/src/lambda_genai_util/AnthropicBedrockUtil.py
+-rw-rw-rw-   0        0        0     1678 2024-05-31 12:16:29.000000 lambda_genai_util-0.0.3/src/lambda_genai_util/AwsTitanBedrockUtil.py
+-rw-rw-rw-   0        0        0      182 2024-05-31 05:52:08.000000 lambda_genai_util-0.0.3/src/lambda_genai_util/BedrockUtil.py
+-rw-rw-rw-   0        0        0     1408 2024-05-31 12:16:24.000000 lambda_genai_util-0.0.3/src/lambda_genai_util/CohereBedrockUtil.py
+-rw-rw-rw-   0        0        0     1251 2024-05-31 12:16:19.000000 lambda_genai_util-0.0.3/src/lambda_genai_util/MetaBedrockUtil.py
+-rw-rw-rw-   0        0        0     1193 2024-05-31 12:16:16.000000 lambda_genai_util-0.0.3/src/lambda_genai_util/MistralBedrockUtil.py
+-rw-rw-rw-   0        0        0     1453 2024-05-31 12:15:59.000000 lambda_genai_util-0.0.3/src/lambda_genai_util/TextCompletionUtil.py
+-rw-rw-rw-   0        0        0        0 2024-05-31 10:47:21.000000 lambda_genai_util-0.0.3/src/lambda_genai_util/__init__.py
+-rw-rw-rw-   0        0        0     1039 2024-05-31 05:52:08.000000 lambda_genai_util-0.0.3/src/lambda_genai_util/model_map.py
+-rw-rw-rw-   0        0        0     2062 2024-05-31 12:16:09.000000 lambda_genai_util-0.0.3/src/lambda_genai_util/prompt_service.py
+drwxrwxrwx   0        0        0        0 2024-05-31 12:16:54.104489 lambda_genai_util-0.0.3/src/lambda_genai_util.egg-info/
+-rw-rw-rw-   0        0        0     1712 2024-05-31 12:16:54.000000 lambda_genai_util-0.0.3/src/lambda_genai_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      659 2024-05-31 12:16:54.000000 lambda_genai_util-0.0.3/src/lambda_genai_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 12:16:54.000000 lambda_genai_util-0.0.3/src/lambda_genai_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-31 12:16:54.000000 lambda_genai_util-0.0.3/src/lambda_genai_util.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-31 12:16:54.000000 lambda_genai_util-0.0.3/src/lambda_genai_util.egg-info/top_level.txt
```

### Comparing `lambda_genai_util-0.0.2/LICENSE.txt` & `lambda_genai_util-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lambda_genai_util-0.0.2/PKG-INFO` & `lambda_genai_util-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda_genai_util
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for GenAI Utility for AWS Based development
 Author-email: Biprajeet Kar <biprokvs@gmail.com>
 Maintainer-email: Biprajeet Kar <biprokvs@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Biprajeet Kar
```

### Comparing `lambda_genai_util-0.0.2/pyproject.toml` & `lambda_genai_util-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lambda_genai_util"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Biprajeet Kar", email="biprokvs@gmail.com" },
 ]
 maintainers = [
   {name="Biprajeet Kar", email="biprokvs@gmail.com"}
 ]
 description = "Library for GenAI Utility for AWS Based development"
```

### Comparing `lambda_genai_util-0.0.2/src/lambda_genai_util/AnthropicBedrockUtil.py` & `lambda_genai_util-0.0.3/src/lambda_genai_util/AnthropicBedrockUtil.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import logging
-from BedrockUtil import BedrockUtil
+from lambda_genai_util.BedrockUtil import BedrockUtil
 
 logger = logging.getLogger(__name__)
 
 class AnthropicBedrockUtil(BedrockUtil):
 
     def text_completion(self, bedrock_client, model, prompt, **model_kwargs):
         prompt_request = {}
```

### Comparing `lambda_genai_util-0.0.2/src/lambda_genai_util/AwsTitanBedrockUtil.py` & `lambda_genai_util-0.0.3/src/lambda_genai_util/AwsTitanBedrockUtil.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import logging
 
-from BedrockUtil import BedrockUtil
+from lambda_genai_util.BedrockUtil import BedrockUtil
 
 logger = logging.getLogger(__name__)
 
 class AwsTitanBedrockUtil(BedrockUtil):
 
     def text_completion(self, bedrock_client, model, prompt, **model_kwargs):
         prompt_request = {}
```

### Comparing `lambda_genai_util-0.0.2/src/lambda_genai_util/CohereBedrockUtil.py` & `lambda_genai_util-0.0.3/src/lambda_genai_util/CohereBedrockUtil.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import logging
-from BedrockUtil import BedrockUtil
+from lambda_genai_util.BedrockUtil import BedrockUtil
 
 logger = logging.getLogger(__name__)
 
 class CohereBedrockUtil(BedrockUtil):
 
     def text_completion(self, bedrock_client, model, prompt, **model_kwargs):
         prompt_request = {}
```

### Comparing `lambda_genai_util-0.0.2/src/lambda_genai_util/MetaBedrockUtil.py` & `lambda_genai_util-0.0.3/src/lambda_genai_util/MetaBedrockUtil.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import logging
 
-from BedrockUtil import BedrockUtil
+from lambda_genai_util.BedrockUtil import BedrockUtil
 
 logger = logging.getLogger(__name__)
 
 class MetaBedrockUtil(BedrockUtil):
 
     def text_completion(self, bedrock_client, model, prompt, **model_kwargs):
         prompt_request = {}
```

### Comparing `lambda_genai_util-0.0.2/src/lambda_genai_util/MistralBedrockUtil.py` & `lambda_genai_util-0.0.3/src/lambda_genai_util/MistralBedrockUtil.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import logging
 
-from BedrockUtil import BedrockUtil
+from lambda_genai_util.BedrockUtil import BedrockUtil
 
 logger = logging.getLogger(__name__)
 
 class MistralBedrockUtil(BedrockUtil):
 
     def text_completion(self, bedrock_client, model, prompt, **model_kwargs):
         prompt_request = {}
```

### Comparing `lambda_genai_util-0.0.2/src/lambda_genai_util/model_map.py` & `lambda_genai_util-0.0.3/src/lambda_genai_util/model_map.py`

 * *Files identical despite different names*

### Comparing `lambda_genai_util-0.0.2/src/lambda_genai_util/prompt_service.py` & `lambda_genai_util-0.0.3/src/lambda_genai_util/prompt_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from lambda_util import yaml
-from TextCompletionUtil import generate_text_completion
-from model_map import model_map
+from lambda_genai_util.TextCompletionUtil import generate_text_completion
+from lambda_genai_util.model_map import model_map
 
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 def read_prompt_config(file_path):
     try:
```

### Comparing `lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/PKG-INFO` & `lambda_genai_util-0.0.3/src/lambda_genai_util.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda_genai_util
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for GenAI Utility for AWS Based development
 Author-email: Biprajeet Kar <biprokvs@gmail.com>
 Maintainer-email: Biprajeet Kar <biprokvs@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Biprajeet Kar
```

### Comparing `lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/SOURCES.txt` & `lambda_genai_util-0.0.3/src/lambda_genai_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

