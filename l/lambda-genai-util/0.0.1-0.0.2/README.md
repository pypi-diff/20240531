# Comparing `tmp/lambda_genai_util-0.0.1.tar.gz` & `tmp/lambda_genai_util-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lambda_genai_util-0.0.1.tar", last modified: Fri May 31 11:31:03 2024, max compression
+gzip compressed data, was "lambda_genai_util-0.0.2.tar", last modified: Fri May 31 11:53:08 2024, max compression
```

## Comparing `lambda_genai_util-0.0.1.tar` & `lambda_genai_util-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 11:31:03.195114 lambda_genai_util-0.0.1/
--rw-rw-rw-   0        0        0     1089 2024-05-30 13:47:39.000000 lambda_genai_util-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1712 2024-05-31 11:31:03.194079 lambda_genai_util-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      611 2024-05-31 11:30:34.000000 lambda_genai_util-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-31 11:31:03.195114 lambda_genai_util-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-31 11:31:03.164627 lambda_genai_util-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-31 11:31:03.178769 lambda_genai_util-0.0.1/src/lambda_genai_util/
--rw-rw-rw-   0        0        0     1453 2024-05-31 10:56:27.000000 lambda_genai_util-0.0.1/src/lambda_genai_util/AnthropicBedrockUtil.py
--rw-rw-rw-   0        0        0     1660 2024-05-31 10:56:38.000000 lambda_genai_util-0.0.1/src/lambda_genai_util/AwsTitanBedrockUtil.py
--rw-rw-rw-   0        0        0      182 2024-05-31 05:52:08.000000 lambda_genai_util-0.0.1/src/lambda_genai_util/BedrockUtil.py
--rw-rw-rw-   0        0        0     1390 2024-05-31 10:56:44.000000 lambda_genai_util-0.0.1/src/lambda_genai_util/CohereBedrockUtil.py
--rw-rw-rw-   0        0        0     1233 2024-05-31 10:56:49.000000 lambda_genai_util-0.0.1/src/lambda_genai_util/MetaBedrockUtil.py
--rw-rw-rw-   0        0        0     1175 2024-05-31 10:56:54.000000 lambda_genai_util-0.0.1/src/lambda_genai_util/MistralBedrockUtil.py
--rw-rw-rw-   0        0        0     1328 2024-05-31 10:57:53.000000 lambda_genai_util-0.0.1/src/lambda_genai_util/TextCompletionUtil.py
--rw-rw-rw-   0        0        0        0 2024-05-31 10:47:21.000000 lambda_genai_util-0.0.1/src/lambda_genai_util/__init__.py
--rw-rw-rw-   0        0        0     1039 2024-05-31 05:52:08.000000 lambda_genai_util-0.0.1/src/lambda_genai_util/model_map.py
--rw-rw-rw-   0        0        0     2024 2024-05-31 11:08:54.000000 lambda_genai_util-0.0.1/src/lambda_genai_util/prompt_service.py
-drwxrwxrwx   0        0        0        0 2024-05-31 11:31:03.192079 lambda_genai_util-0.0.1/src/lambda_genai_util.egg-info/
--rw-rw-rw-   0        0        0     1712 2024-05-31 11:31:03.000000 lambda_genai_util-0.0.1/src/lambda_genai_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      659 2024-05-31 11:31:03.000000 lambda_genai_util-0.0.1/src/lambda_genai_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 11:31:03.000000 lambda_genai_util-0.0.1/src/lambda_genai_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-31 11:31:03.000000 lambda_genai_util-0.0.1/src/lambda_genai_util.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-31 11:31:03.000000 lambda_genai_util-0.0.1/src/lambda_genai_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 11:53:08.467369 lambda_genai_util-0.0.2/
+-rw-rw-rw-   0        0        0     1089 2024-05-30 13:47:39.000000 lambda_genai_util-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1712 2024-05-31 11:53:08.466369 lambda_genai_util-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2024-05-31 11:52:01.000000 lambda_genai_util-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 11:53:08.467369 lambda_genai_util-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 11:53:08.442517 lambda_genai_util-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-31 11:53:08.456631 lambda_genai_util-0.0.2/src/lambda_genai_util/
+-rw-rw-rw-   0        0        0     1453 2024-05-31 10:56:27.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/AnthropicBedrockUtil.py
+-rw-rw-rw-   0        0        0     1660 2024-05-31 10:56:38.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/AwsTitanBedrockUtil.py
+-rw-rw-rw-   0        0        0      182 2024-05-31 05:52:08.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/BedrockUtil.py
+-rw-rw-rw-   0        0        0     1390 2024-05-31 10:56:44.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/CohereBedrockUtil.py
+-rw-rw-rw-   0        0        0     1233 2024-05-31 10:56:49.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/MetaBedrockUtil.py
+-rw-rw-rw-   0        0        0     1175 2024-05-31 10:56:54.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/MistralBedrockUtil.py
+-rw-rw-rw-   0        0        0     1345 2024-05-31 11:52:25.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/TextCompletionUtil.py
+-rw-rw-rw-   0        0        0        0 2024-05-31 10:47:21.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/__init__.py
+-rw-rw-rw-   0        0        0     1039 2024-05-31 05:52:08.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/model_map.py
+-rw-rw-rw-   0        0        0     2026 2024-05-31 11:52:42.000000 lambda_genai_util-0.0.2/src/lambda_genai_util/prompt_service.py
+drwxrwxrwx   0        0        0        0 2024-05-31 11:53:08.465369 lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/
+-rw-rw-rw-   0        0        0     1712 2024-05-31 11:53:08.000000 lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      659 2024-05-31 11:53:08.000000 lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 11:53:08.000000 lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-31 11:53:08.000000 lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-31 11:53:08.000000 lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/top_level.txt
```

### Comparing `lambda_genai_util-0.0.1/LICENSE.txt` & `lambda_genai_util-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lambda_genai_util-0.0.1/PKG-INFO` & `lambda_genai_util-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda_genai_util
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for GenAI Utility for AWS Based development
 Author-email: Biprajeet Kar <biprokvs@gmail.com>
 Maintainer-email: Biprajeet Kar <biprokvs@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Biprajeet Kar
```

### Comparing `lambda_genai_util-0.0.1/pyproject.toml` & `lambda_genai_util-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lambda_genai_util"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Biprajeet Kar", email="biprokvs@gmail.com" },
 ]
 maintainers = [
   {name="Biprajeet Kar", email="biprokvs@gmail.com"}
 ]
 description = "Library for GenAI Utility for AWS Based development"
```

### Comparing `lambda_genai_util-0.0.1/src/lambda_genai_util/AnthropicBedrockUtil.py` & `lambda_genai_util-0.0.2/src/lambda_genai_util/AnthropicBedrockUtil.py`

 * *Files identical despite different names*

### Comparing `lambda_genai_util-0.0.1/src/lambda_genai_util/AwsTitanBedrockUtil.py` & `lambda_genai_util-0.0.2/src/lambda_genai_util/AwsTitanBedrockUtil.py`

 * *Files identical despite different names*

### Comparing `lambda_genai_util-0.0.1/src/lambda_genai_util/CohereBedrockUtil.py` & `lambda_genai_util-0.0.2/src/lambda_genai_util/CohereBedrockUtil.py`

 * *Files identical despite different names*

### Comparing `lambda_genai_util-0.0.1/src/lambda_genai_util/MetaBedrockUtil.py` & `lambda_genai_util-0.0.2/src/lambda_genai_util/MetaBedrockUtil.py`

 * *Files identical despite different names*

### Comparing `lambda_genai_util-0.0.1/src/lambda_genai_util/MistralBedrockUtil.py` & `lambda_genai_util-0.0.2/src/lambda_genai_util/MistralBedrockUtil.py`

 * *Files identical despite different names*

### Comparing `lambda_genai_util-0.0.1/src/lambda_genai_util/TextCompletionUtil.py` & `lambda_genai_util-0.0.2/src/lambda_genai_util/TextCompletionUtil.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-import boto3
+from lambda_util import boto3
 from MetaBedrockUtil import MetaBedrockUtil
 from MistralBedrockUtil import MistralBedrockUtil
 from AwsTitanBedrockUtil import AwsTitanBedrockUtil
 from AnthropicBedrockUtil import AnthropicBedrockUtil
 from CohereBedrockUtil import CohereBedrockUtil
 from model_map import model_map
```

### Comparing `lambda_genai_util-0.0.1/src/lambda_genai_util/model_map.py` & `lambda_genai_util-0.0.2/src/lambda_genai_util/model_map.py`

 * *Files identical despite different names*

### Comparing `lambda_genai_util-0.0.1/src/lambda_genai_util/prompt_service.py` & `lambda_genai_util-0.0.2/src/lambda_genai_util/prompt_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from genai_lib import yaml
+from lambda_util import yaml
 from TextCompletionUtil import generate_text_completion
 from model_map import model_map
 
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
```

### Comparing `lambda_genai_util-0.0.1/src/lambda_genai_util.egg-info/PKG-INFO` & `lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lambda_genai_util
-Version: 0.0.1
+Version: 0.0.2
 Summary: Library for GenAI Utility for AWS Based development
 Author-email: Biprajeet Kar <biprokvs@gmail.com>
 Maintainer-email: Biprajeet Kar <biprokvs@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Biprajeet Kar
```

### Comparing `lambda_genai_util-0.0.1/src/lambda_genai_util.egg-info/SOURCES.txt` & `lambda_genai_util-0.0.2/src/lambda_genai_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

