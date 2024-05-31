# Comparing `tmp/scalexi-0.4.7.1.tar.gz` & `tmp/scalexi-0.4.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scalexi-0.4.7.1.tar", last modified: Thu May 30 11:17:22 2024, max compression
+gzip compressed data, was "scalexi-0.4.7.2.tar", last modified: Fri May 31 14:55:32 2024, max compression
```

## Comparing `scalexi-0.4.7.1.tar` & `scalexi-0.4.7.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.902634 scalexi-0.4.7.1/
--rw-r--r--   0 akoubaa    (501) staff       (20)     2751 2023-11-18 18:27:29.000000 scalexi-0.4.7.1/LICENSE
--rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-30 11:17:22.902427 scalexi-0.4.7.1/PKG-INFO
--rw-r--r--   0 akoubaa    (501) staff       (20)    15922 2023-11-22 16:53:27.000000 scalexi-0.4.7.1/README.md
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.888454 scalexi-0.4.7.1/scalexi/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/__init__.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.892992 scalexi-0.4.7.1/scalexi/data/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/data/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     4882 2024-05-27 15:01:35.000000 scalexi-0.4.7.1/scalexi/data/openai_pricing.json
--rw-r--r--   0 akoubaa    (501) staff       (20)     3723 2024-03-11 15:00:18.000000 scalexi-0.4.7.1/scalexi/data/openai_pricing_v1.json
--rw-r--r--   0 akoubaa    (501) staff       (20)     3517 2024-05-27 15:01:06.000000 scalexi-0.4.7.1/scalexi/data/openai_pricing_v2.json
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.894322 scalexi-0.4.7.1/scalexi/dataset_generation/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/dataset_generation/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    32752 2023-11-20 18:15:53.000000 scalexi-0.4.7.1/scalexi/dataset_generation/prompt_completion.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.895465 scalexi-0.4.7.1/scalexi/document_loaders/
--rw-r--r--   0 akoubaa    (501) staff       (20)        0 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/document_loaders/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     3944 2023-11-20 17:59:39.000000 scalexi-0.4.7.1/scalexi/document_loaders/context_loaders.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     2167 2024-05-23 19:27:41.000000 scalexi-0.4.7.1/scalexi/document_loaders/pdf_loaders.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.897065 scalexi-0.4.7.1/scalexi/llm/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/llm/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     4214 2024-01-29 23:03:40.000000 scalexi-0.4.7.1/scalexi/llm/google_gemini.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     9996 2024-01-29 23:59:01.000000 scalexi-0.4.7.1/scalexi/llm/openai_gpt.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.897747 scalexi-0.4.7.1/scalexi/llm_evaluation/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/llm_evaluation/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    36889 2023-11-22 13:28:34.000000 scalexi-0.4.7.1/scalexi/llm_evaluation/evaluate.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.899696 scalexi-0.4.7.1/scalexi/openai/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/openai/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    29566 2023-11-23 15:04:13.000000 scalexi-0.4.7.1/scalexi/openai/fine_tuning_api.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    34682 2024-05-27 16:10:27.000000 scalexi-0.4.7.1/scalexi/openai/pricing.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    12977 2024-05-27 16:28:54.000000 scalexi-0.4.7.1/scalexi/openai/utilities.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.901564 scalexi-0.4.7.1/scalexi/utilities/
--rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.1/scalexi/utilities/__init__.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     1040 2024-05-25 09:44:04.000000 scalexi-0.4.7.1/scalexi/utilities/api.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    38655 2024-01-29 19:28:25.000000 scalexi-0.4.7.1/scalexi/utilities/data_formatter.py
--rw-r--r--   0 akoubaa    (501) staff       (20)     2728 2024-01-29 21:41:32.000000 scalexi-0.4.7.1/scalexi/utilities/logger.py
--rw-r--r--   0 akoubaa    (501) staff       (20)    19936 2024-05-29 16:14:23.000000 scalexi-0.4.7.1/scalexi/utilities/text_processing.py
-drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-30 11:17:22.891130 scalexi-0.4.7.1/scalexi.egg-info/
--rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-30 11:17:22.000000 scalexi-0.4.7.1/scalexi.egg-info/PKG-INFO
--rw-r--r--   0 akoubaa    (501) staff       (20)      958 2024-05-30 11:17:22.000000 scalexi-0.4.7.1/scalexi.egg-info/SOURCES.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)        1 2024-05-30 11:17:22.000000 scalexi-0.4.7.1/scalexi.egg-info/dependency_links.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)      130 2024-05-30 11:17:22.000000 scalexi-0.4.7.1/scalexi.egg-info/requires.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)        8 2024-05-30 11:17:22.000000 scalexi-0.4.7.1/scalexi.egg-info/top_level.txt
--rw-r--r--   0 akoubaa    (501) staff       (20)       38 2024-05-30 11:17:22.902684 scalexi-0.4.7.1/setup.cfg
--rw-r--r--   0 akoubaa    (501) staff       (20)     5404 2024-05-29 10:05:42.000000 scalexi-0.4.7.1/setup.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.648213 scalexi-0.4.7.2/
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2751 2023-11-18 18:27:29.000000 scalexi-0.4.7.2/LICENSE
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-31 14:55:32.648096 scalexi-0.4.7.2/PKG-INFO
+-rw-r--r--   0 akoubaa    (501) staff       (20)    15922 2023-11-22 16:53:27.000000 scalexi-0.4.7.2/README.md
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.643663 scalexi-0.4.7.2/scalexi/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/__init__.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.644964 scalexi-0.4.7.2/scalexi/data/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/data/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4882 2024-05-27 15:01:35.000000 scalexi-0.4.7.2/scalexi/data/openai_pricing.json
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3723 2024-03-11 15:00:18.000000 scalexi-0.4.7.2/scalexi/data/openai_pricing_v1.json
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3517 2024-05-27 15:01:06.000000 scalexi-0.4.7.2/scalexi/data/openai_pricing_v2.json
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.645375 scalexi-0.4.7.2/scalexi/dataset_generation/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/dataset_generation/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    32752 2023-11-20 18:15:53.000000 scalexi-0.4.7.2/scalexi/dataset_generation/prompt_completion.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.645742 scalexi-0.4.7.2/scalexi/document_loaders/
+-rw-r--r--   0 akoubaa    (501) staff       (20)        0 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/document_loaders/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     3944 2023-11-20 17:59:39.000000 scalexi-0.4.7.2/scalexi/document_loaders/context_loaders.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2167 2024-05-23 19:27:41.000000 scalexi-0.4.7.2/scalexi/document_loaders/pdf_loaders.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.646128 scalexi-0.4.7.2/scalexi/llm/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/llm/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4214 2024-01-29 23:03:40.000000 scalexi-0.4.7.2/scalexi/llm/google_gemini.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     9996 2024-01-29 23:59:01.000000 scalexi-0.4.7.2/scalexi/llm/openai_gpt.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.646425 scalexi-0.4.7.2/scalexi/llm_evaluation/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/llm_evaluation/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    36889 2023-11-22 13:28:34.000000 scalexi-0.4.7.2/scalexi/llm_evaluation/evaluate.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.647114 scalexi-0.4.7.2/scalexi/openai/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/openai/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    29566 2023-11-23 15:04:13.000000 scalexi-0.4.7.2/scalexi/openai/fine_tuning_api.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    34682 2024-05-27 16:10:27.000000 scalexi-0.4.7.2/scalexi/openai/pricing.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    13931 2024-05-30 19:25:30.000000 scalexi-0.4.7.2/scalexi/openai/utilities.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.647893 scalexi-0.4.7.2/scalexi/utilities/
+-rw-r--r--   0 akoubaa    (501) staff       (20)       36 2023-11-15 19:31:52.000000 scalexi-0.4.7.2/scalexi/utilities/__init__.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     1040 2024-05-25 09:44:04.000000 scalexi-0.4.7.2/scalexi/utilities/api.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    38655 2024-01-29 19:28:25.000000 scalexi-0.4.7.2/scalexi/utilities/data_formatter.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)     2728 2024-01-29 21:41:32.000000 scalexi-0.4.7.2/scalexi/utilities/logger.py
+-rw-r--r--   0 akoubaa    (501) staff       (20)    19936 2024-05-29 16:14:23.000000 scalexi-0.4.7.2/scalexi/utilities/text_processing.py
+drwxr-xr-x   0 akoubaa    (501) staff       (20)        0 2024-05-31 14:55:32.644265 scalexi-0.4.7.2/scalexi.egg-info/
+-rw-r--r--   0 akoubaa    (501) staff       (20)     4525 2024-05-31 14:55:32.000000 scalexi-0.4.7.2/scalexi.egg-info/PKG-INFO
+-rw-r--r--   0 akoubaa    (501) staff       (20)      958 2024-05-31 14:55:32.000000 scalexi-0.4.7.2/scalexi.egg-info/SOURCES.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)        1 2024-05-31 14:55:32.000000 scalexi-0.4.7.2/scalexi.egg-info/dependency_links.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)      130 2024-05-31 14:55:32.000000 scalexi-0.4.7.2/scalexi.egg-info/requires.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)        8 2024-05-31 14:55:32.000000 scalexi-0.4.7.2/scalexi.egg-info/top_level.txt
+-rw-r--r--   0 akoubaa    (501) staff       (20)       38 2024-05-31 14:55:32.648265 scalexi-0.4.7.2/setup.cfg
+-rw-r--r--   0 akoubaa    (501) staff       (20)     5404 2024-05-31 14:55:24.000000 scalexi-0.4.7.2/setup.py
```

### Comparing `scalexi-0.4.7.1/LICENSE` & `scalexi-0.4.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/PKG-INFO` & `scalexi-0.4.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalexi
-Version: 0.4.7.1
+Version: 0.4.7.2
 Summary: The scalexi package is a versatile open-source Python library that focuses on facilitating low-code development and fine-tuning of diverse Large Language Models (LLMs). It extends beyond its initial OpenAI models integration, offering a scalable framework for various LLMs.
 Home-page: https://github.com/scalexi/scalexi
 Author: ScaleX Innovation
 Author-email: akoubaa@scalexi.ai
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `scalexi-0.4.7.1/README.md` & `scalexi-0.4.7.2/README.md`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi/data/openai_pricing.json` & `scalexi-0.4.7.2/scalexi/data/openai_pricing.json`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi/data/openai_pricing_v1.json` & `scalexi-0.4.7.2/scalexi/data/openai_pricing_v1.json`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi/data/openai_pricing_v2.json` & `scalexi-0.4.7.2/scalexi/data/openai_pricing_v2.json`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi/dataset_generation/prompt_completion.py` & `scalexi-0.4.7.2/scalexi/dataset_generation/prompt_completion.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi/document_loaders/context_loaders.py` & `scalexi-0.4.7.2/scalexi/document_loaders/context_loaders.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi/document_loaders/pdf_loaders.py` & `scalexi-0.4.7.2/scalexi/document_loaders/pdf_loaders.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi/llm/google_gemini.py` & `scalexi-0.4.7.2/scalexi/llm/google_gemini.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi/llm/openai_gpt.py` & `scalexi-0.4.7.2/scalexi/llm/openai_gpt.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi/llm_evaluation/evaluate.py` & `scalexi-0.4.7.2/scalexi/llm_evaluation/evaluate.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi/openai/fine_tuning_api.py` & `scalexi-0.4.7.2/scalexi/openai/fine_tuning_api.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi/openai/pricing.py` & `scalexi-0.4.7.2/scalexi/openai/pricing.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi/openai/utilities.py` & `scalexi-0.4.7.2/scalexi/openai/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,43 @@
 
     :return: A dictionary containing the pricing information for OpenAI models.
     """
     data = pkgutil.get_data('scalexi', 'data/openai_pricing.json')
     pricing_info = json.loads(data)
     return pricing_info
 
+def get_gpt_context_length(model_name):
+    # Dictionary mapping model names to their context lengths
+    gpt_context_lengths = {
+        "gpt-4o": 128000,
+        "gpt-4o-2024-05-13": 128000,
+        "gpt-4-turbo": 128000,
+        "gpt-4-turbo-2024-04-09": 128000,
+        "gpt-4-turbo-preview": 128000,
+        "gpt-4-0125-preview": 128000,
+        "gpt-4-1106-preview": 128000,
+        "gpt-4-vision-preview": 128000,
+        "gpt-4-1106-vision-preview": 128000,
+        "gpt-4": 8192,
+        "gpt-4-0613": 8192,
+        "gpt-4-32k": 32768,
+        "gpt-4-32k-0613": 32768,
+        "gpt-3.5-turbo-0125": 16385,
+        "gpt-3.5-turbo": 16385,
+        "gpt-3.5-turbo-1106": 16385,
+        "gpt-3.5-turbo-instruct": 4096,
+        "gpt-3.5-turbo-16k": 16385,
+        "gpt-3.5-turbo-0613": 4096,
+        "gpt-3.5-turbo-16k-0613": 16385
+    }
+
+    # Return the context length for the specified model
+    return gpt_context_lengths.get(model_name, None)
+
+
 
 def get_context_length(model_name):
     """
     Returns the context length of the specified model using the pricing info from OpenAI.
 
     :param model_name: The name of the model whose context length is needed.
     :return: The context length of the model if found, otherwise returns None.
```

### Comparing `scalexi-0.4.7.1/scalexi/utilities/api.py` & `scalexi-0.4.7.2/scalexi/utilities/api.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi/utilities/data_formatter.py` & `scalexi-0.4.7.2/scalexi/utilities/data_formatter.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi/utilities/logger.py` & `scalexi-0.4.7.2/scalexi/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi/utilities/text_processing.py` & `scalexi-0.4.7.2/scalexi/utilities/text_processing.py`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/scalexi.egg-info/PKG-INFO` & `scalexi-0.4.7.2/scalexi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scalexi
-Version: 0.4.7.1
+Version: 0.4.7.2
 Summary: The scalexi package is a versatile open-source Python library that focuses on facilitating low-code development and fine-tuning of diverse Large Language Models (LLMs). It extends beyond its initial OpenAI models integration, offering a scalable framework for various LLMs.
 Home-page: https://github.com/scalexi/scalexi
 Author: ScaleX Innovation
 Author-email: akoubaa@scalexi.ai
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `scalexi-0.4.7.1/scalexi.egg-info/SOURCES.txt` & `scalexi-0.4.7.2/scalexi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scalexi-0.4.7.1/setup.py` & `scalexi-0.4.7.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="scalexi",
-    version="0.4.7.1",
+    version="0.4.7.2",
     packages=find_packages(),
     include_package_data=True,
     package_data={'scalexi': ['data/*']},
     install_requires=[
         "pandas",  # Add any package dependencies here
         "openai>=1.10.0", #this package is not compatible with earlier versions of openai
         "sphinx",   # Add any other dependencies as needed
```

