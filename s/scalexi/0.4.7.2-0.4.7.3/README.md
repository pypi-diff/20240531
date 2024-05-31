# Comparing `tmp/scalexi-0.4.7.2.tar.gz` & `tmp/scalexi-0.4.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalexi-0.4.7.2.tar", last modified: Fri May 31 14:55:32 2024, max compression
+gzip compressed data, was "scalexi-0.4.7.3.tar", last modified: Fri May 31 21:05:36 2024, max compression
```

## Comparing `scalexi-0.4.7.2.tar` & `scalexi-0.4.7.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.648213 scalexi-0.4.7.2/
--rw-r--r--   0 akoubaa    (501) staff       (20)     2751 2023-11-18 18:27:29.000000 scalexi-0.4.7.2/LICENSE
--rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-31 14:55:32.648096 scalexi-0.4.7.2/PKG-INFO
--rw-r--r--   0 akoubaa    (501) staff       (20)    15922 2023-11-22 16:53:27.000000 scalexi-0.4.7.2/README.md
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.643663 scalexi-0.4.7.2/scalexi/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/__init__.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.644964 scalexi-0.4.7.2/scalexi/data/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/data/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     4882 2024-05-27 15:01:35.000000 scalexi-0.4.7.2/scalexi/data/openai_pricing.json
--rw-r--r--   0 akoubaa    (501) staff       (20)     3723 2024-03-11 15:00:18.000000 scalexi-0.4.7.2/scalexi/data/openai_pricing_v1.json
--rw-r--r--   0 akoubaa    (501) staff       (20)     3517 2024-05-27 15:01:06.000000 scalexi-0.4.7.2/scalexi/data/openai_pricing_v2.json
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.645375 scalexi-0.4.7.2/scalexi/dataset_generation/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/dataset_generation/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    32752 2023-11-20 18:15:53.000000 scalexi-0.4.7.2/scalexi/dataset_generation/prompt_completion.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.645742 scalexi-0.4.7.2/scalexi/document_loaders/
--rw-r--r--   0 akoubaa    (501) staff       (20)        0 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/document_loaders/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     3944 2023-11-20 17:59:39.000000 scalexi-0.4.7.2/scalexi/document_loaders/context_loaders.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     2167 2024-05-23 19:27:41.000000 scalexi-0.4.7.2/scalexi/document_loaders/pdf_loaders.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.646128 scalexi-0.4.7.2/scalexi/llm/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/llm/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     4214 2024-01-29 23:03:40.000000 scalexi-0.4.7.2/scalexi/llm/google_gemini.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     9996 2024-01-29 23:59:01.000000 scalexi-0.4.7.2/scalexi/llm/openai_gpt.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.646425 scalexi-0.4.7.2/scalexi/llm_evaluation/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/llm_evaluation/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    36889 2023-11-22 13:28:34.000000 scalexi-0.4.7.2/scalexi/llm_evaluation/evaluate.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.647114 scalexi-0.4.7.2/scalexi/openai/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/openai/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    29566 2023-11-23 15:04:13.000000 scalexi-0.4.7.2/scalexi/openai/fine_tuning_api.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    34682 2024-05-27 16:10:27.000000 scalexi-0.4.7.2/scalexi/openai/pricing.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    13931 2024-05-30 19:25:30.000000 scalexi-0.4.7.2/scalexi/openai/utilities.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.647893 scalexi-0.4.7.2/scalexi/utilities/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/utilities/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     1040 2024-05-25 09:44:04.000000 scalexi-0.4.7.2/scalexi/utilities/api.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    38655 2024-01-29 19:28:25.000000 scalexi-0.4.7.2/scalexi/utilities/data_formatter.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     2728 2024-01-29 21:41:32.000000 scalexi-0.4.7.2/scalexi/utilities/logger.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    19936 2024-05-29 16:14:23.000000 scalexi-0.4.7.2/scalexi/utilities/text_processing.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.644265 scalexi-0.4.7.2/scalexi.egg-info/
--rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-31 14:55:32.000000 scalexi-0.4.7.2/scalexi.egg-info/PKG-INFO
--rw-r--r--   0 akoubaa    (501) staff       (20)      958 2024-05-31 14:55:32.000000 scalexi-0.4.7.2/scalexi.egg-info/SOURCES.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)        1 2024-05-31 14:55:32.000000 scalexi-0.4.7.2/scalexi.egg-info/dependency_links.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)      130 2024-05-31 14:55:32.000000 scalexi-0.4.7.2/scalexi.egg-info/requires.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)        8 2024-05-31 14:55:32.000000 scalexi-0.4.7.2/scalexi.egg-info/top_level.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)       38 2024-05-31 14:55:32.648265 scalexi-0.4.7.2/setup.cfg
--rw-r--r--   0 akoubaa    (501) staff       (20)     5404 2024-05-31 14:55:24.000000 scalexi-0.4.7.2/setup.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 21:05:36.157422 scalexi-0.4.7.3/
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2751 2023-11-18 18:27:29.000000 scalexi-0.4.7.3/LICENSE
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-31 21:05:36.157300 scalexi-0.4.7.3/PKG-INFO
+-rw-r--r--   0 akoubaa    (501) staff       (20)    15922 2023-11-22 16:53:27.000000 scalexi-0.4.7.3/README.md
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 21:05:36.148222 scalexi-0.4.7.3/scalexi/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.3/scalexi/__init__.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 21:05:36.150318 scalexi-0.4.7.3/scalexi/data/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.3/scalexi/data/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4882 2024-05-27 15:01:35.000000 scalexi-0.4.7.3/scalexi/data/openai_pricing.json
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3723 2024-03-11 15:00:18.000000 scalexi-0.4.7.3/scalexi/data/openai_pricing_v1.json
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3517 2024-05-27 15:01:06.000000 scalexi-0.4.7.3/scalexi/data/openai_pricing_v2.json
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 21:05:36.150769 scalexi-0.4.7.3/scalexi/dataset_generation/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.3/scalexi/dataset_generation/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    32752 2023-11-20 18:15:53.000000 scalexi-0.4.7.3/scalexi/dataset_generation/prompt_completion.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 21:05:36.155170 scalexi-0.4.7.3/scalexi/document_loaders/
+-rw-r--r--   0 akoubaa    (501) staff       (20)        0 2023-11-15 19:31:52.000000 scalexi-0.4.7.3/scalexi/document_loaders/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3944 2023-11-20 17:59:39.000000 scalexi-0.4.7.3/scalexi/document_loaders/context_loaders.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2167 2024-05-23 19:27:41.000000 scalexi-0.4.7.3/scalexi/document_loaders/pdf_loaders.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 21:05:36.155551 scalexi-0.4.7.3/scalexi/llm/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.3/scalexi/llm/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4214 2024-01-29 23:03:40.000000 scalexi-0.4.7.3/scalexi/llm/google_gemini.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     9996 2024-01-29 23:59:01.000000 scalexi-0.4.7.3/scalexi/llm/openai_gpt.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 21:05:36.155800 scalexi-0.4.7.3/scalexi/llm_evaluation/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.3/scalexi/llm_evaluation/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    36889 2023-11-22 13:28:34.000000 scalexi-0.4.7.3/scalexi/llm_evaluation/evaluate.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 21:05:36.156312 scalexi-0.4.7.3/scalexi/openai/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.3/scalexi/openai/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    29566 2023-11-23 15:04:13.000000 scalexi-0.4.7.3/scalexi/openai/fine_tuning_api.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    34682 2024-05-27 16:10:27.000000 scalexi-0.4.7.3/scalexi/openai/pricing.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    14663 2024-05-31 21:04:34.000000 scalexi-0.4.7.3/scalexi/openai/utilities.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 21:05:36.156991 scalexi-0.4.7.3/scalexi/utilities/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.3/scalexi/utilities/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     1040 2024-05-25 09:44:04.000000 scalexi-0.4.7.3/scalexi/utilities/api.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    38655 2024-01-29 19:28:25.000000 scalexi-0.4.7.3/scalexi/utilities/data_formatter.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2728 2024-01-29 21:41:32.000000 scalexi-0.4.7.3/scalexi/utilities/logger.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    19936 2024-05-29 16:14:23.000000 scalexi-0.4.7.3/scalexi/utilities/text_processing.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 21:05:36.148893 scalexi-0.4.7.3/scalexi.egg-info/
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-31 21:05:36.000000 scalexi-0.4.7.3/scalexi.egg-info/PKG-INFO
+-rw-r--r--   0 akoubaa    (501) staff       (20)      958 2024-05-31 21:05:36.000000 scalexi-0.4.7.3/scalexi.egg-info/SOURCES.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)        1 2024-05-31 21:05:36.000000 scalexi-0.4.7.3/scalexi.egg-info/dependency_links.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)      130 2024-05-31 21:05:36.000000 scalexi-0.4.7.3/scalexi.egg-info/requires.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)        8 2024-05-31 21:05:36.000000 scalexi-0.4.7.3/scalexi.egg-info/top_level.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)       38 2024-05-31 21:05:36.157467 scalexi-0.4.7.3/setup.cfg
+-rw-r--r--   0 akoubaa    (501) staff       (20)     5404 2024-05-31 21:05:26.000000 scalexi-0.4.7.3/setup.py
```

### Comparing `scalexi-0.4.7.2/LICENSE` & `scalexi-0.4.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/PKG-INFO` & `scalexi-0.4.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalexi
-Version: 0.4.7.2
+Version: 0.4.7.3
 Summary: The scalexi package is a versatile open-source Python library that focuses on facilitating low-code development and fine-tuning of diverse Large Language Models (LLMs). It extends beyond its initial OpenAI models integration, offering a scalable framework for various LLMs.
 Home-page: https://github.com/scalexi/scalexi
 Author: ScaleX Innovation
 Author-email: akoubaa@scalexi.ai
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `scalexi-0.4.7.2/README.md` & `scalexi-0.4.7.3/README.md`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi/data/openai_pricing.json` & `scalexi-0.4.7.3/scalexi/data/openai_pricing.json`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi/data/openai_pricing_v1.json` & `scalexi-0.4.7.3/scalexi/data/openai_pricing_v1.json`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi/data/openai_pricing_v2.json` & `scalexi-0.4.7.3/scalexi/data/openai_pricing_v2.json`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi/dataset_generation/prompt_completion.py` & `scalexi-0.4.7.3/scalexi/dataset_generation/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi/document_loaders/context_loaders.py` & `scalexi-0.4.7.3/scalexi/document_loaders/context_loaders.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi/document_loaders/pdf_loaders.py` & `scalexi-0.4.7.3/scalexi/document_loaders/pdf_loaders.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi/llm/google_gemini.py` & `scalexi-0.4.7.3/scalexi/llm/google_gemini.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi/llm/openai_gpt.py` & `scalexi-0.4.7.3/scalexi/llm/openai_gpt.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi/llm_evaluation/evaluate.py` & `scalexi-0.4.7.3/scalexi/llm_evaluation/evaluate.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi/openai/fine_tuning_api.py` & `scalexi-0.4.7.3/scalexi/openai/fine_tuning_api.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi/openai/pricing.py` & `scalexi-0.4.7.3/scalexi/openai/pricing.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi/openai/utilities.py` & `scalexi-0.4.7.3/scalexi/openai/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -317,8 +317,26 @@
         }
         #print(token_usage)
         
         # Estimate the cost
         print('estimate_inference_cost  token_usage:', token_usage)
         cost = estimate_inference_cost_by_tokens(token_usage['prompt_tokens'], token_usage['completion_tokens'], model_name)
         
-        return content, token_usage, cost
+        return content, token_usage, cost
+    
+def extract_gpt_token_usage(response):
+        """
+        Extracts the token usage from a ChatCompletion response object and returns it in a dictionary.
+
+        :param response: The ChatCompletion response object.
+        :return: A dictionary containing the number of tokens used for the prompt, completion, and total.
+        """
+        if hasattr(response, 'usage'):
+            token_usage = {
+                "prompt_tokens": response.usage.prompt_tokens,
+                "completion_tokens": response.usage.completion_tokens,
+                "total_tokens": response.usage.total_tokens
+            }
+        else:
+            token_usage = {"error": "No token usage information available"}
+
+        return token_usage
```

### Comparing `scalexi-0.4.7.2/scalexi/utilities/api.py` & `scalexi-0.4.7.3/scalexi/utilities/api.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi/utilities/data_formatter.py` & `scalexi-0.4.7.3/scalexi/utilities/data_formatter.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi/utilities/logger.py` & `scalexi-0.4.7.3/scalexi/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi/utilities/text_processing.py` & `scalexi-0.4.7.3/scalexi/utilities/text_processing.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/scalexi.egg-info/PKG-INFO` & `scalexi-0.4.7.3/scalexi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalexi
-Version: 0.4.7.2
+Version: 0.4.7.3
 Summary: The scalexi package is a versatile open-source Python library that focuses on facilitating low-code development and fine-tuning of diverse Large Language Models (LLMs). It extends beyond its initial OpenAI models integration, offering a scalable framework for various LLMs.
 Home-page: https://github.com/scalexi/scalexi
 Author: ScaleX Innovation
 Author-email: akoubaa@scalexi.ai
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `scalexi-0.4.7.2/scalexi.egg-info/SOURCES.txt` & `scalexi-0.4.7.3/scalexi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.2/setup.py` & `scalexi-0.4.7.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="scalexi",
-    version="0.4.7.2",
+    version="0.4.7.3",
     packages=find_packages(),
     include_package_data=True,
     package_data={'scalexi': ['data/*']},
     install_requires=[
         "pandas",  # Add any package dependencies here
         "openai>=1.10.0", #this package is not compatible with earlier versions of openai
         "sphinx",   # Add any other dependencies as needed
```

