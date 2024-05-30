# Comparing `tmp/llmint-0.0.2.tar.gz` & `tmp/llmint-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/llmint-0.0.2.tar", last modified: Thu Oct 12 20:14:34 2023, max compression
+gzip compressed data, was "llmint-0.0.3.tar", last modified: Thu May 30 22:45:55 2024, max compression
```

## Comparing `llmint-0.0.2.tar` & `llmint-0.0.3.tar`

### file list

```diff
@@ -1,48 +1,58 @@
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-10-12 20:14:34.218961 llmint-0.0.2/
--rw-r--r--   0 silv       (501) staff       (20)      253 2023-10-12 20:14:34.218829 llmint-0.0.2/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)     6583 2023-10-12 04:09:16.000000 llmint-0.0.2/README.md
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-10-12 20:14:34.212509 llmint-0.0.2/benchmark/
--rw-r--r--   0 silv       (501) staff       (20)       37 2023-10-09 07:41:13.000000 llmint-0.0.2/benchmark/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     4777 2023-10-12 17:18:06.000000 llmint-0.0.2/benchmark/benchmark_record_mapper.py
--rw-r--r--   0 silv       (501) staff       (20)     4908 2023-10-12 17:08:25.000000 llmint-0.0.2/benchmark/benchmark_record_match.py
--rw-r--r--   0 silv       (501) staff       (20)     2775 2023-10-11 19:34:08.000000 llmint-0.0.2/benchmark/log.py
--rw-r--r--   0 silv       (501) staff       (20)     1068 2023-10-11 16:25:49.000000 llmint-0.0.2/benchmark/util.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-10-12 20:14:34.213142 llmint-0.0.2/llmint/
--rw-r--r--   0 silv       (501) staff       (20)      344 2023-10-12 02:37:56.000000 llmint-0.0.2/llmint/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-10-12 20:14:34.214107 llmint-0.0.2/llmint/assembly/
--rw-r--r--   0 silv       (501) staff       (20)        0 2023-10-10 06:13:00.000000 llmint-0.0.2/llmint/assembly/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-10-12 20:14:34.214208 llmint-0.0.2/llmint/discover/
--rw-r--r--   0 silv       (501) staff       (20)        0 2023-10-05 00:04:30.000000 llmint-0.0.2/llmint/discover/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-10-12 20:14:34.214896 llmint-0.0.2/llmint/extract/
--rw-r--r--   0 silv       (501) staff       (20)       53 2023-10-09 05:34:02.000000 llmint-0.0.2/llmint/extract/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     1582 2023-10-11 00:31:32.000000 llmint-0.0.2/llmint/extract/from_json.py
--rw-r--r--   0 silv       (501) staff       (20)     1305 2023-10-11 15:48:19.000000 llmint-0.0.2/llmint/extract/from_mint_sample.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-10-12 20:14:34.215163 llmint-0.0.2/llmint/identify/
--rw-r--r--   0 silv       (501) staff       (20)        0 2023-10-05 17:00:10.000000 llmint-0.0.2/llmint/identify/__init__.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-10-12 20:14:34.216343 llmint-0.0.2/llmint/mapper/
--rw-r--r--   0 silv       (501) staff       (20)     1383 2023-10-12 03:21:16.000000 llmint-0.0.2/llmint/mapper/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     2286 2023-10-12 03:37:52.000000 llmint-0.0.2/llmint/mapper/output.py
--rw-r--r--   0 silv       (501) staff       (20)     2048 2023-10-12 02:41:56.000000 llmint-0.0.2/llmint/mapper/record.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2023-10-12 02:11:10.000000 llmint-0.0.2/llmint/mapper/schema.py
--rw-r--r--   0 silv       (501) staff       (20)      705 2023-10-11 16:01:28.000000 llmint-0.0.2/llmint/mapper/stored_mapping.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-10-12 20:14:34.217289 llmint-0.0.2/llmint/match/
--rw-r--r--   0 silv       (501) staff       (20)     1421 2023-10-12 02:42:38.000000 llmint-0.0.2/llmint/match/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)     3255 2023-10-12 01:51:04.000000 llmint-0.0.2/llmint/match/record.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2023-10-12 02:10:58.000000 llmint-0.0.2/llmint/match/schema.py
--rw-r--r--   0 silv       (501) staff       (20)     1012 2023-10-11 16:58:02.000000 llmint-0.0.2/llmint/match/util.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-10-12 20:14:34.218287 llmint-0.0.2/llmint/mint/
--rw-r--r--   0 silv       (501) staff       (20)       30 2023-10-12 02:00:19.000000 llmint-0.0.2/llmint/mint/__init__.py
--rw-r--r--   0 silv       (501) staff       (20)       14 2023-10-09 08:39:31.000000 llmint-0.0.2/llmint/mint/core.py
--rw-r--r--   0 silv       (501) staff       (20)        0 2023-10-10 06:13:22.000000 llmint-0.0.2/llmint/mint/retrospect.py
--rw-r--r--   0 silv       (501) staff       (20)     2713 2023-10-12 02:32:06.000000 llmint-0.0.2/llmint/mint/telemetry.py
--rw-r--r--   0 silv       (501) staff       (20)      882 2023-10-12 01:51:27.000000 llmint-0.0.2/llmint/util.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-10-12 20:14:34.213987 llmint-0.0.2/llmint.egg-info/
--rw-r--r--   0 silv       (501) staff       (20)      253 2023-10-12 20:14:33.000000 llmint-0.0.2/llmint.egg-info/PKG-INFO
--rw-r--r--   0 silv       (501) staff       (20)      839 2023-10-12 20:14:33.000000 llmint-0.0.2/llmint.egg-info/SOURCES.txt
--rw-r--r--   0 silv       (501) staff       (20)        1 2023-10-12 20:14:33.000000 llmint-0.0.2/llmint.egg-info/dependency_links.txt
--rw-r--r--   0 silv       (501) staff       (20)       13 2023-10-12 20:14:33.000000 llmint-0.0.2/llmint.egg-info/requires.txt
--rw-r--r--   0 silv       (501) staff       (20)       22 2023-10-12 20:14:33.000000 llmint-0.0.2/llmint.egg-info/top_level.txt
--rw-r--r--   0 silv       (501) staff       (20)       38 2023-10-12 20:14:34.218999 llmint-0.0.2/setup.cfg
--rw-r--r--   0 silv       (501) staff       (20)      413 2023-10-12 20:14:29.000000 llmint-0.0.2/setup.py
-drwxr-xr-x   0 silv       (501) staff       (20)        0 2023-10-12 20:14:34.218687 llmint-0.0.2/test/
--rw-r--r--   0 silv       (501) staff       (20)        0 2023-10-09 05:41:30.000000 llmint-0.0.2/test/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-30 22:45:55.257378 llmint-0.0.3/
+-rw-r--r--   0 silv       (501) staff       (20)    11357 2024-03-14 22:39:17.000000 llmint-0.0.3/LICENSE
+-rw-r--r--   0 silv       (501) staff       (20)      265 2024-05-30 22:45:55.257241 llmint-0.0.3/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)     3451 2024-04-11 15:49:34.000000 llmint-0.0.3/README.md
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-30 22:45:55.250030 llmint-0.0.3/benchmark/
+-rw-r--r--   0 silv       (501) staff       (20)       37 2024-03-14 22:39:17.000000 llmint-0.0.3/benchmark/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     4693 2024-03-14 22:39:17.000000 llmint-0.0.3/benchmark/benchmark_record_mapper.py
+-rw-r--r--   0 silv       (501) staff       (20)     5757 2024-03-14 22:39:43.000000 llmint-0.0.3/benchmark/benchmark_record_match.py
+-rw-r--r--   0 silv       (501) staff       (20)     7404 2024-05-30 22:44:17.000000 llmint-0.0.3/benchmark/benchmark_schema_mapper.py
+-rw-r--r--   0 silv       (501) staff       (20)     2775 2024-03-14 22:39:17.000000 llmint-0.0.3/benchmark/log.py
+-rw-r--r--   0 silv       (501) staff       (20)     1068 2024-03-14 22:39:17.000000 llmint-0.0.3/benchmark/util.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-30 22:45:55.250669 llmint-0.0.3/llmint/
+-rw-r--r--   0 silv       (501) staff       (20)      267 2024-04-18 23:48:06.000000 llmint-0.0.3/llmint/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-30 22:45:55.251475 llmint-0.0.3/llmint/assembly/
+-rw-r--r--   0 silv       (501) staff       (20)      101 2024-04-11 17:25:42.000000 llmint-0.0.3/llmint/assembly/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-30 22:45:55.251688 llmint-0.0.3/llmint/assembly/zed/
+-rw-r--r--   0 silv       (501) staff       (20)       24 2024-04-11 17:25:42.000000 llmint-0.0.3/llmint/assembly/zed/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-30 22:45:55.252375 llmint-0.0.3/llmint/extract/
+-rw-r--r--   0 silv       (501) staff       (20)       53 2024-03-14 22:39:17.000000 llmint-0.0.3/llmint/extract/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       64 2024-03-14 22:39:17.000000 llmint-0.0.3/llmint/extract/from_json.py
+-rw-r--r--   0 silv       (501) staff       (20)     1660 2024-03-14 22:39:43.000000 llmint-0.0.3/llmint/extract/from_mint_sample.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-30 22:45:55.252606 llmint-0.0.3/llmint/mapper/
+-rw-r--r--   0 silv       (501) staff       (20)       64 2024-04-18 23:48:06.000000 llmint-0.0.3/llmint/mapper/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-30 22:45:55.254494 llmint-0.0.3/llmint/mapper/command/
+-rw-r--r--   0 silv       (501) staff       (20)       41 2024-04-18 23:48:06.000000 llmint-0.0.3/llmint/mapper/command/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)     1735 2024-05-30 22:44:17.000000 llmint-0.0.3/llmint/mapper/command/api.py
+-rw-r--r--   0 silv       (501) staff       (20)    26831 2024-05-30 22:44:17.000000 llmint-0.0.3/llmint/mapper/command/model.py
+-rw-r--r--   0 silv       (501) staff       (20)     5293 2024-05-30 22:44:17.000000 llmint-0.0.3/llmint/mapper/command/util.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-30 22:45:55.254743 llmint-0.0.3/llmint/mapper/functions/
+-rw-r--r--   0 silv       (501) staff       (20)      705 2024-03-14 22:39:17.000000 llmint-0.0.3/llmint/mapper/functions/retrieve.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-30 22:45:55.255120 llmint-0.0.3/llmint/mint/
+-rw-r--r--   0 silv       (501) staff       (20)       53 2024-03-14 22:39:17.000000 llmint-0.0.3/llmint/mint/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-30 22:45:55.255910 llmint-0.0.3/llmint/mint/core/
+-rw-r--r--   0 silv       (501) staff       (20)       64 2024-03-14 22:39:17.000000 llmint-0.0.3/llmint/mint/core/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)      637 2024-03-14 22:39:17.000000 llmint-0.0.3/llmint/mint/core/correspondence.py
+-rw-r--r--   0 silv       (501) staff       (20)      814 2024-03-14 22:39:17.000000 llmint-0.0.3/llmint/mint/core/mapping.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-30 22:45:55.256551 llmint-0.0.3/llmint/mint/core/prompts/
+-rw-r--r--   0 silv       (501) staff       (20)       85 2024-03-14 22:39:17.000000 llmint-0.0.3/llmint/mint/core/prompts/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)       35 2024-03-14 22:39:17.000000 llmint-0.0.3/llmint/mint/core/prompts/prompt_correspondence.py
+-rw-r--r--   0 silv       (501) staff       (20)     1496 2024-03-14 22:39:43.000000 llmint-0.0.3/llmint/mint/core/prompts/prompt_mapping.py
+-rw-r--r--   0 silv       (501) staff       (20)       25 2024-03-14 22:39:17.000000 llmint-0.0.3/llmint/mint/core/prompts/prompt_schema.py
+-rw-r--r--   0 silv       (501) staff       (20)     8711 2024-03-14 22:39:17.000000 llmint-0.0.3/llmint/mint/core/schema.py
+-rw-r--r--   0 silv       (501) staff       (20)     1511 2024-03-14 22:39:17.000000 llmint-0.0.3/llmint/mint/llm.py
+-rw-r--r--   0 silv       (501) staff       (20)     2762 2024-03-14 22:39:17.000000 llmint-0.0.3/llmint/mint/telemetry.py
+-rw-r--r--   0 silv       (501) staff       (20)      851 2024-03-14 22:39:17.000000 llmint-0.0.3/llmint/util.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-30 22:45:55.251381 llmint-0.0.3/llmint.egg-info/
+-rw-r--r--   0 silv       (501) staff       (20)      265 2024-05-30 22:45:55.000000 llmint-0.0.3/llmint.egg-info/PKG-INFO
+-rw-r--r--   0 silv       (501) staff       (20)     1159 2024-05-30 22:45:55.000000 llmint-0.0.3/llmint.egg-info/SOURCES.txt
+-rw-r--r--   0 silv       (501) staff       (20)        1 2024-05-30 22:45:55.000000 llmint-0.0.3/llmint.egg-info/dependency_links.txt
+-rw-r--r--   0 silv       (501) staff       (20)       52 2024-05-30 22:45:55.000000 llmint-0.0.3/llmint.egg-info/requires.txt
+-rw-r--r--   0 silv       (501) staff       (20)       22 2024-05-30 22:45:55.000000 llmint-0.0.3/llmint.egg-info/top_level.txt
+-rw-r--r--   0 silv       (501) staff       (20)       38 2024-05-30 22:45:55.257410 llmint-0.0.3/setup.cfg
+-rw-r--r--   0 silv       (501) staff       (20)      414 2024-05-30 22:44:41.000000 llmint-0.0.3/setup.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-30 22:45:55.256803 llmint-0.0.3/test/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-03-14 22:39:17.000000 llmint-0.0.3/test/__init__.py
+drwxr-xr-x   0 silv       (501) staff       (20)        0 2024-05-30 22:45:55.257100 llmint-0.0.3/test/test_extract/
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-03-14 22:39:17.000000 llmint-0.0.3/test/test_extract/__init__.py
+-rw-r--r--   0 silv       (501) staff       (20)        0 2024-03-14 22:39:17.000000 llmint-0.0.3/test/test_extract/test_schema_extract.py
```

### Comparing `llmint-0.0.2/benchmark/benchmark_record_mapper.py` & `llmint-0.0.3/benchmark/benchmark_record_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import llmint.mapper.output as output_util
 
 __dir__ = os.path.dirname(__file__)
 __log_dir__ = os.path.join(__dir__, "logs")
 default_dataset = os.path.join(
     __dir__, "..", "..",
     "mint-sample-data",
-    "device", "flat_light_varied_value.yaml"
+    "record", "flat_light.yaml"
 )
 
 
 def run(mapper, test_set):
     map_correct = []
 
     log("Examples:")
@@ -27,18 +27,15 @@
         log(header(f"Test {i + 1}"))
         log(header("Input"))
 
         source, target = sample["source"], sample["target"]
         true_mapping = sample["mapping"]
         log(mapper.format_input(source, target))
 
-        pred_mapping = mapper.invoke(
-            source_schema=source,
-            target_schema=target,
-        )["text"]
+        pred_mapping = mapper.invoke(source, target)
 
         # validate the prediction
         try:
             pred_mapping = output_util.format_output(pred_mapping)
         except:
             pass
         is_correct = pred_mapping == true_mapping
@@ -78,16 +75,16 @@
         filepath=default_dataset,
         test_size=0.75,
         # match params
         model="gpt-3.5-turbo",
         temperature=0.0,
         match_method=RecordChatMapper,
         # benchmark params
-        min_num_shot=0,
-        max_num_shot=2,
+        min_num_shot=1,
+        max_num_shot=1,
         num_test=5,
         verbose=True,
         seed=42,
 ):
     """
     Run a benchmark test on a device dataset with varying shots.
```

### Comparing `llmint-0.0.2/benchmark/benchmark_record_match.py` & `llmint-0.0.3/benchmark/benchmark_record_match.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,97 +2,106 @@
 from benchmark import util
 from benchmark.log import (
     init_logger, log_name, log, header
 )
 import numpy as np
 
 from llmint.extract import from_mint_sample
-from llmint.match.record import RecordChatMatch
+from llmint.match.record import RecordChatMatch, RecordPromptMatch
 import llmint.match.util as match_util
 
 __dir__ = os.path.dirname(__file__)
 __log_dir__ = os.path.join(__dir__, "logs")
 default_dataset = os.path.join(
     __dir__, "..", "..",
     "mint-sample-data",
-    "device", "flat.yaml"
+    "record", "flat_light.yaml" # CHANGE HERE
 )
+matchClass = RecordChatMatch # CHANGE HERE
 
+"""
+Benchmark script for testing accuracy, latency, and token count of RecordPromptMatch and RecordChatMatch.
+
+Modify matchClass on line 19 to change which match class you want to test. 
+Modify the yaml file name on line 17 to change which test/training example file you want to use.
+
+The only yaml file for RecordPromptMatch is currently the record_match_prompt.yaml file. RecordChatMatch
+can use any other yaml file for benchmarking.
+"""
 
-# TBD: refactor this to use the Match base class
 def run(match, test_set):
     match_correct = []
 
     log("Examples:")
     log(match.examples)
 
     for i, sample in enumerate(test_set):
         log(header(f"Test {i + 1}"))
         log(header("Input"))
 
         source, target = sample["source"], sample["target"]
-        true_corresp = sample["correspondence"]
+        true_corresp = sample["correspondence"] if matchClass == RecordChatMatch \
+                                                else match_util.pt_format_input(sample["correspondence"])
         log(match.format_input(source, target))
 
         pred_corresp = match.invoke(
             source_schema=source,
             target_schema=target,
         )["text"]
-
+        
         # validate the prediction
         try:
-            pred_corresp = match_util.format_output(pred_corresp)
+            pred_corresp = match_util.format_output(pred_corresp) if matchClass == RecordChatMatch \
+                                                                  else match_util.pt_format_output(pred_corresp)
         except:
             pass
         is_correct = pred_corresp == true_corresp
         match_correct.append(is_correct)
 
         log(header("Prediction"))
         log(f"True: {true_corresp}")
         log(f"Pred: {pred_corresp}")
 
         log(header("Stats"))
         log(f"{'Correct' if is_correct else 'Incorrect'}")
         if not is_correct:
             log(header("Diff"))
             log(match_util.diff_corresp(true_corresp, pred_corresp))
-        log(f"Latency: {match.latencies[-1]}")
-        log(f"Token_count: {match.token_counts[-1]}")
+        log(f"Latency: {match.telemetry.latencies[-1]}")
+        log(f"Token_count: {match.telemetry.total_tokens[-1]}")
 
-    summary = {
+    stats = {
         "match_correct": match_correct,
-        "token_counts": match.token_counts,
-        "latencies": match.latencies,
+        **match.telemetry.stats(),
     }
-    stats = {
+    summary = {
         "total": len(match_correct),
         "accuracy": sum(match_correct) / len(match_correct),
-        "avg_token_count": np.mean(match.token_counts),
-        "avg_latency": np.mean(match.latencies),
+        **match.telemetry.summary(),
     }
 
     log(header("Summary"))
-    log(summary, pretty=True)
     log(stats, pretty=True)
+    log(summary, pretty=True)
 
     return stats, summary
 
 
 def benchmark_vary_shot(
         # dataset params
         filepath=default_dataset,
-        test_size=0.75,
+        test_size=0.25,
         # match params
         model="gpt-3.5-turbo", # "gpt-4"
         temperature=0.0,
-        match_method=RecordChatMatch,
+        match_method=matchClass,
         # benchmark params
         min_num_shot=0,
         max_num_shot=2,
-        num_test=10,
+        num_test=1,
         verbose=True,
         seed=42,
 ):
     """
     Run a benchmark test on a device dataset with varying shots.
 
     Args:
@@ -114,48 +123,51 @@
         add_timestamp=True
     )
     log(f"Setup: {locals()}")
 
     # Prepare dataset
     data = util.from_yaml(filepath)
     # XXX detect sample type
-    samples = list(from_mint_sample.read_match(data))
+    if (match_method == RecordChatMatch):
+        samples = list(from_mint_sample.read_match(data))
+    elif (match_method == RecordPromptMatch):
+        samples = list(from_mint_sample.read_pt_match(data))
     train_set, test_set = util.train_test_split(samples, test_size=test_size, seed=seed)
 
     assert len(test_set) >= num_test, "Number of test samples is greater than the actual test set size."
     log(f"train size {len(train_set)}, test size {len(test_set)}")
 
     # Initialize benchmark results containers
-    all_stats = {}
+    all_summaries = {}
     token_count = 0
 
     # Run the benchmark
     for num_shot in range(min_num_shot, max_num_shot + 1):
         log(header(f"Running for {num_shot} shots", char="="))
 
         # Initialize matching method with current shot
         match = match_method(
-            examples=train_set[:num_shot],
-            model=model,
+            examples = train_set[:num_shot],
+            model=model, 
             temperature=temperature,
             verbose=verbose,
         )
 
         # Evaluate the current shot
         stats, summary = run(match, test_set[:num_test])
 
-        all_stats[num_shot] = stats
-        token_count += sum(summary["token_counts"])
+        all_summaries[num_shot] = summary
+        token_count += summary["total_tokens"]
 
     # Print summary of benchmarks
     log(header("Benchmark summary", char="="))
     log({
-        "Accuracy": {num_shot: stats["accuracy"] for num_shot, stats in all_stats.items()},
-        "Avg token count": {num_shot: stats["avg_token_count"] for num_shot, stats in all_stats.items()},
-        "Avg latency": {num_shot: stats["avg_latency"] for num_shot, stats in all_stats.items()},
+        "Accuracy": {num_shot: summary["accuracy"] for num_shot, summary in all_summaries.items()},
+        "Avg token count": {num_shot: summary["avg_tokens"] for num_shot, summary in all_summaries.items()},
+        "Avg latency": {num_shot: summary["avg_latency"] for num_shot, summary in all_summaries.items()},
         "Total tokens used": token_count
     }, pretty=True)
 
 
 def main():
     benchmark_vary_shot()
```

### Comparing `llmint-0.0.2/benchmark/log.py` & `llmint-0.0.3/benchmark/log.py`

 * *Files identical despite different names*

### Comparing `llmint-0.0.2/benchmark/util.py` & `llmint-0.0.3/benchmark/util.py`

 * *Files identical despite different names*

### Comparing `llmint-0.0.2/llmint/extract/from_mint_sample.py` & `llmint-0.0.3/llmint/extract/from_mint_sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,7 +35,17 @@
                 "target": row["target"],
                 "correspondence": [
                     {"from": mapping["from"],
                      "to": mapping["to"]}
                     for mapping in row["mapping"]
                 ],
             }
+
+def read_pt_match(input_data: Dict[str, List[Dict]]) -> Generator:
+    for kind, rows in input_data.items():
+        for row in rows:
+            yield {
+                "kind": kind,
+                "source": row["source"],
+                "target": row["target"],
+                "correspondence": [mapping for mapping in row["mapping"]]
+            }
```

### Comparing `llmint-0.0.2/llmint/mapper/stored_mapping.py` & `llmint-0.0.3/llmint/mapper/functions/retrieve.py`

 * *Files identical despite different names*

### Comparing `llmint-0.0.2/llmint/mint/telemetry.py` & `llmint-0.0.3/llmint/mint/telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 import numpy as np
 from langchain.callbacks import manager as cb_manager
 from langchain.callbacks import get_openai_callback
 
-
+# TBD make Telemetry mergeable (.add method).
 class Telemetry:
     def __init__(self):
         self.total_tokens = []
         self.prompt_tokens = []
         self.completion_tokens = []
         self.latencies = []
         self.total_costs = []
@@ -70,15 +70,15 @@
 
 
 def test():
     from langchain.llms import OpenAI
     from llmint import util
     import pprint as pp
 
-    llm = OpenAI(openai_api_key=util.get_openai_key())
+    llm = OpenAI(openai_api_key=util.get_openai_api_key())
 
     telemetry = Telemetry()
     with get_openai_callback() as cb:
         with telemetry.report(cb):
             print(llm("Hello!", temperature=0.1))
 
     pp.pprint(telemetry.summary())
```

### Comparing `llmint-0.0.2/llmint/util.py` & `llmint-0.0.3/llmint/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import yaml
 
 from langchain.schema import BaseOutputParser
 
 
 # Read OpenAI key from ~/.llmint/config.yaml
-# XXX rename to get_openai_api_key
-def get_openai_key():
+def get_openai_api_key():
     with open(os.path.expanduser("~/.llmint/config.yaml"), "r") as f:
         config = yaml.load(f, Loader=yaml.SafeLoader)
         if "openai_api_key" not in config:
             raise Exception("OpenAI API key not found in ~/.llmint/config.yaml,"
                             " please add 'openai_api_key: YOUR_KEY' in the file.")
         openai_api_key = config["openai_api_key"]
         return openai_api_key
```

### Comparing `llmint-0.0.2/llmint.egg-info/SOURCES.txt` & `llmint-0.0.3/llmint.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,41 @@
+LICENSE
 README.md
 setup.py
 benchmark/__init__.py
 benchmark/benchmark_record_mapper.py
 benchmark/benchmark_record_match.py
+benchmark/benchmark_schema_mapper.py
 benchmark/log.py
 benchmark/util.py
 llmint/__init__.py
 llmint/util.py
 llmint.egg-info/PKG-INFO
 llmint.egg-info/SOURCES.txt
 llmint.egg-info/dependency_links.txt
 llmint.egg-info/requires.txt
 llmint.egg-info/top_level.txt
 llmint/assembly/__init__.py
-llmint/discover/__init__.py
+llmint/assembly/zed/__init__.py
 llmint/extract/__init__.py
 llmint/extract/from_json.py
 llmint/extract/from_mint_sample.py
-llmint/identify/__init__.py
 llmint/mapper/__init__.py
-llmint/mapper/output.py
-llmint/mapper/record.py
-llmint/mapper/schema.py
-llmint/mapper/stored_mapping.py
-llmint/match/__init__.py
-llmint/match/record.py
-llmint/match/schema.py
-llmint/match/util.py
+llmint/mapper/command/__init__.py
+llmint/mapper/command/api.py
+llmint/mapper/command/model.py
+llmint/mapper/command/util.py
+llmint/mapper/functions/retrieve.py
 llmint/mint/__init__.py
-llmint/mint/core.py
-llmint/mint/retrospect.py
+llmint/mint/llm.py
 llmint/mint/telemetry.py
-test/__init__.py
+llmint/mint/core/__init__.py
+llmint/mint/core/correspondence.py
+llmint/mint/core/mapping.py
+llmint/mint/core/schema.py
+llmint/mint/core/prompts/__init__.py
+llmint/mint/core/prompts/prompt_correspondence.py
+llmint/mint/core/prompts/prompt_mapping.py
+llmint/mint/core/prompts/prompt_schema.py
+test/__init__.py
+test/test_extract/__init__.py
+test/test_extract/test_schema_extract.py
```

