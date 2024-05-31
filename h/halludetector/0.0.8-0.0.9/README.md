# Comparing `tmp/halludetector-0.0.8.tar.gz` & `tmp/halludetector-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "halludetector-0.0.8.tar", last modified: Mon Apr  8 15:44:05 2024, max compression
+gzip compressed data, was "halludetector-0.0.9.tar", last modified: Fri May 31 07:08:55 2024, max compression
```

## Comparing `halludetector-0.0.8.tar` & `halludetector-0.0.9.tar`

### file list

```diff
@@ -1,57 +1,54 @@
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:44:05.877883 halludetector-0.0.8/
--rw-r--r--   0 onofreimihai   (502) staff       (20)     3303 2024-04-08 15:44:05.876623 halludetector-0.0.8/PKG-INFO
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2068 2024-03-18 17:05:40.000000 halludetector-0.0.8/README.md
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2240 2024-04-08 14:32:22.000000 halludetector-0.0.8/README.rst
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:44:05.839458 halludetector-0.0.8/halludetector/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      610 2024-03-16 16:01:59.000000 halludetector-0.0.8/halludetector/__init__.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:44:05.846969 halludetector-0.0.8/halludetector/checker/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      231 2024-02-29 16:02:48.000000 halludetector-0.0.8/halludetector/checker/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      277 2024-03-16 09:24:35.000000 halludetector-0.0.8/halludetector/checker/checker.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2764 2024-03-16 09:24:35.000000 halludetector-0.0.8/halludetector/checker/checker_base.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     3773 2024-03-16 09:24:35.000000 halludetector-0.0.8/halludetector/checker/gpt4_checker.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1801 2024-04-08 15:23:11.000000 halludetector-0.0.8/halludetector/config.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:44:05.851519 halludetector-0.0.8/halludetector/datasets/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      454 2024-03-23 07:46:24.000000 halludetector-0.0.8/halludetector/datasets/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      845 2024-03-23 07:52:44.000000 halludetector-0.0.8/halludetector/datasets/covid_qa.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      794 2024-03-23 07:52:44.000000 halludetector-0.0.8/halludetector/datasets/databricks_dolly.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1697 2024-03-23 07:52:44.000000 halludetector-0.0.8/halludetector/datasets/drop.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      300 2024-03-23 07:39:58.000000 halludetector-0.0.8/halludetector/datasets/parser.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:44:05.858119 halludetector-0.0.8/halludetector/detectors/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      235 2024-04-03 17:45:46.000000 halludetector-0.0.8/halludetector/detectors/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2148 2024-03-26 10:45:06.000000 halludetector-0.0.8/halludetector/detectors/base.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1188 2024-04-08 15:39:22.000000 halludetector-0.0.8/halludetector/detectors/chainpoll.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      282 2024-04-03 15:22:49.000000 halludetector-0.0.8/halludetector/detectors/custom.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2254 2024-04-08 15:39:22.000000 halludetector-0.0.8/halludetector/detectors/geval.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1389 2024-03-17 10:29:34.000000 halludetector-0.0.8/halludetector/detectors/refchecker.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     5253 2024-04-03 14:38:13.000000 halludetector-0.0.8/halludetector/detectors/selfcheckgpt.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:44:05.864690 halludetector-0.0.8/halludetector/extractor/
--rw-r--r--   0 onofreimihai   (502) staff       (20)      192 2024-02-29 16:01:22.000000 halludetector-0.0.8/halludetector/extractor/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     4495 2024-02-29 15:45:58.000000 halludetector-0.0.8/halludetector/extractor/claude2_extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      528 2024-03-26 11:22:28.000000 halludetector-0.0.8/halludetector/extractor/extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     2094 2024-02-29 15:45:58.000000 halludetector-0.0.8/halludetector/extractor/extractor_base.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     4423 2024-03-16 10:06:20.000000 halludetector-0.0.8/halludetector/extractor/gpt4_extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     4833 2024-02-29 15:45:58.000000 halludetector-0.0.8/halludetector/extractor/mistral_extractor.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     9086 2024-02-29 15:45:58.000000 halludetector-0.0.8/halludetector/extractor/mixtral_extractor.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:44:05.866498 halludetector-0.0.8/halludetector/generators/
--rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:56:29.000000 halludetector-0.0.8/halludetector/generators/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      919 2024-03-26 11:32:51.000000 halludetector-0.0.8/halludetector/generators/question.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:44:05.869867 halludetector-0.0.8/halludetector/llm/
--rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:35:21.000000 halludetector-0.0.8/halludetector/llm/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      800 2024-04-03 13:24:02.000000 halludetector-0.0.8/halludetector/llm/mistral.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      698 2024-04-08 15:30:03.000000 halludetector-0.0.8/halludetector/llm/openai.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:44:05.871727 halludetector-0.0.8/halludetector/prompts/
--rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:43:40.000000 halludetector-0.0.8/halludetector/prompts/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     4549 2024-04-08 15:37:10.000000 halludetector-0.0.8/halludetector/prompts/default.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:44:05.874746 halludetector-0.0.8/halludetector/retrievers/
--rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 09:05:44.000000 halludetector-0.0.8/halludetector/retrievers/__init__.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)     9189 2024-03-17 09:49:36.000000 halludetector-0.0.8/halludetector/retrievers/google_retriever.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      275 2024-03-16 09:12:53.000000 halludetector-0.0.8/halludetector/retrievers/retriever.py
--rw-r--r--   0 onofreimihai   (502) staff       (20)      736 2024-04-03 17:45:46.000000 halludetector-0.0.8/halludetector/scorer.py
-drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:44:05.843744 halludetector-0.0.8/halludetector.egg-info/
--rw-r--r--   0 onofreimihai   (502) staff       (20)     3303 2024-04-08 15:44:05.000000 halludetector-0.0.8/halludetector.egg-info/PKG-INFO
--rw-r--r--   0 onofreimihai   (502) staff       (20)     1497 2024-04-08 15:44:05.000000 halludetector-0.0.8/halludetector.egg-info/SOURCES.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)        1 2024-04-08 15:44:05.000000 halludetector-0.0.8/halludetector.egg-info/dependency_links.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)      439 2024-04-08 15:44:05.000000 halludetector-0.0.8/halludetector.egg-info/requires.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)       14 2024-04-08 15:44:05.000000 halludetector-0.0.8/halludetector.egg-info/top_level.txt
--rw-r--r--   0 onofreimihai   (502) staff       (20)       38 2024-04-08 15:44:05.878142 halludetector-0.0.8/setup.cfg
--rw-r--r--   0 onofreimihai   (502) staff       (20)      901 2024-04-08 15:43:54.000000 halludetector-0.0.8/setup.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-05-31 07:08:55.322243 halludetector-0.0.9/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     9997 2024-05-31 07:08:55.321723 halludetector-0.0.9/PKG-INFO
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     8934 2024-05-31 07:08:13.000000 halludetector-0.0.9/README.rst
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-05-31 07:08:55.308935 halludetector-0.0.9/halludetector/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      610 2024-03-16 16:01:59.000000 halludetector-0.0.9/halludetector/__init__.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-05-31 07:08:55.311479 halludetector-0.0.9/halludetector/checker/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      231 2024-02-29 16:02:48.000000 halludetector-0.0.9/halludetector/checker/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      277 2024-03-16 09:24:35.000000 halludetector-0.0.9/halludetector/checker/checker.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2764 2024-03-16 09:24:35.000000 halludetector-0.0.9/halludetector/checker/checker_base.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     3773 2024-03-16 09:24:35.000000 halludetector-0.0.9/halludetector/checker/gpt4_checker.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1801 2024-04-13 09:34:01.000000 halludetector-0.0.9/halludetector/config.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-05-31 07:08:55.314154 halludetector-0.0.9/halludetector/datasets/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      499 2024-04-13 08:17:23.000000 halludetector-0.0.9/halludetector/datasets/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      845 2024-03-23 07:52:44.000000 halludetector-0.0.9/halludetector/datasets/covid_qa.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      794 2024-03-23 07:52:44.000000 halludetector-0.0.9/halludetector/datasets/databricks_dolly.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1697 2024-03-23 07:52:44.000000 halludetector-0.0.9/halludetector/datasets/drop.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      432 2024-04-13 07:39:18.000000 halludetector-0.0.9/halludetector/datasets/parser.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      678 2024-04-13 08:44:11.000000 halludetector-0.0.9/halludetector/datasets/summeval.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-05-31 07:08:55.316208 halludetector-0.0.9/halludetector/detectors/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      200 2024-04-13 08:07:09.000000 halludetector-0.0.9/halludetector/detectors/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2162 2024-04-13 08:15:02.000000 halludetector-0.0.9/halludetector/detectors/base.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1202 2024-04-13 08:15:02.000000 halludetector-0.0.9/halludetector/detectors/chainpoll.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2868 2024-04-21 08:50:08.000000 halludetector-0.0.9/halludetector/detectors/geval.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1403 2024-04-29 14:58:50.000000 halludetector-0.0.9/halludetector/detectors/refchecker.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     5286 2024-04-13 08:15:02.000000 halludetector-0.0.9/halludetector/detectors/selfcheckgpt.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-05-31 07:08:55.317640 halludetector-0.0.9/halludetector/extractor/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      192 2024-02-29 16:01:22.000000 halludetector-0.0.9/halludetector/extractor/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      528 2024-03-26 11:22:28.000000 halludetector-0.0.9/halludetector/extractor/extractor.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     2097 2024-04-13 07:48:40.000000 halludetector-0.0.9/halludetector/extractor/extractor_base.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     4423 2024-03-16 10:06:20.000000 halludetector-0.0.9/halludetector/extractor/gpt4_extractor.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-05-31 07:08:55.318312 halludetector-0.0.9/halludetector/generators/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:56:29.000000 halludetector-0.0.9/halludetector/generators/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      919 2024-03-26 11:32:51.000000 halludetector-0.0.9/halludetector/generators/question.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-05-31 07:08:55.319560 halludetector-0.0.9/halludetector/llm/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 08:35:21.000000 halludetector-0.0.9/halludetector/llm/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1483 2024-04-21 08:49:33.000000 halludetector-0.0.9/halludetector/llm/cohere.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      800 2024-04-03 13:24:02.000000 halludetector-0.0.9/halludetector/llm/mistral.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      702 2024-04-13 09:03:25.000000 halludetector-0.0.9/halludetector/llm/openai.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-05-31 07:08:55.320088 halludetector-0.0.9/halludetector/prompts/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-04-08 15:43:40.000000 halludetector-0.0.9/halludetector/prompts/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     4723 2024-04-13 07:48:40.000000 halludetector-0.0.9/halludetector/prompts/default.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-05-31 07:08:55.320973 halludetector-0.0.9/halludetector/retrievers/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        0 2024-03-16 09:05:44.000000 halludetector-0.0.9/halludetector/retrievers/__init__.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     9189 2024-03-17 09:49:36.000000 halludetector-0.0.9/halludetector/retrievers/google_retriever.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      275 2024-03-16 09:12:53.000000 halludetector-0.0.9/halludetector/retrievers/retriever.py
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      714 2024-04-13 08:40:34.000000 halludetector-0.0.9/halludetector/scorer.py
+drwxr-xr-x   0 onofreimihai   (502) staff       (20)        0 2024-05-31 07:08:55.310346 halludetector-0.0.9/halludetector.egg-info/
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     9997 2024-05-31 07:08:55.000000 halludetector-0.0.9/halludetector.egg-info/PKG-INFO
+-rw-r--r--   0 onofreimihai   (502) staff       (20)     1381 2024-05-31 07:08:55.000000 halludetector-0.0.9/halludetector.egg-info/SOURCES.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)        1 2024-05-31 07:08:55.000000 halludetector-0.0.9/halludetector.egg-info/dependency_links.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      439 2024-05-31 07:08:55.000000 halludetector-0.0.9/halludetector.egg-info/requires.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)       14 2024-05-31 07:08:55.000000 halludetector-0.0.9/halludetector.egg-info/top_level.txt
+-rw-r--r--   0 onofreimihai   (502) staff       (20)       38 2024-05-31 07:08:55.322326 halludetector-0.0.9/setup.cfg
+-rw-r--r--   0 onofreimihai   (502) staff       (20)      901 2024-05-31 07:08:48.000000 halludetector-0.0.9/setup.py
```

### Comparing `halludetector-0.0.8/halludetector/__init__.py` & `halludetector-0.0.9/halludetector/__init__.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.8/halludetector/checker/checker_base.py` & `halludetector-0.0.9/halludetector/checker/checker_base.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.8/halludetector/checker/gpt4_checker.py` & `halludetector-0.0.9/halludetector/checker/gpt4_checker.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.8/halludetector/config.py` & `halludetector-0.0.9/halludetector/config.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.8/halludetector/datasets/covid_qa.py` & `halludetector-0.0.9/halludetector/datasets/covid_qa.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.8/halludetector/datasets/databricks_dolly.py` & `halludetector-0.0.9/halludetector/datasets/databricks_dolly.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.8/halludetector/datasets/drop.py` & `halludetector-0.0.9/halludetector/datasets/drop.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.8/halludetector/detectors/base.py` & `halludetector-0.0.9/halludetector/detectors/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,9 +52,9 @@
     def similarity_ngram(self, sentences, passage, sampled_passages):
         return self.ngramscorer.predict(
             passage=passage,
             sentences=sentences,  # list of sentences
             sampled_passages=sampled_passages,  # list of sampled passages
         )
 
-    def score(self, question, answer=None, samples=None):
+    def score(self, question, answer=None, samples=None, summary=None):
         raise NotImplementedError
```

### Comparing `halludetector-0.0.8/halludetector/detectors/chainpoll.py` & `halludetector-0.0.9/halludetector/detectors/chainpoll.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 
     def check_hallucinations(self, completion, question):
         text = self.prompt.format(completion=completion, question=question)
         responses = self.ask_llm(text, n=int(os.getenv("CHAINPOLL_SAMPLING_NUMBER")), temperature=0.2)
         logger.info(f'Hallucination check response: {responses}')
         return [response.lower().startswith("yes") for response in responses], responses
 
-    def score(self, question, answer=None, samples=None):
+    def score(self, question, answer=None, samples=None, summary=None):
         if not answer:
             answer = self.ask_llm(question.strip())[0]
         hallucinations, responses = self.check_hallucinations(answer.strip(), question.strip())
 
         score = hallucinations.count(True) / len(hallucinations)
         return score, answer, responses
```

### Comparing `halludetector-0.0.8/halludetector/detectors/geval.py` & `halludetector-0.0.9/halludetector/detectors/geval.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,22 +10,33 @@
 logger = logging.getLogger(__name__)
 
 
 class GEval(Detector):
     metrics = ['coherence', 'consistency', 'fluency', 'relevance']
     @staticmethod
     def parse_output(output):
+        if ':' in output:
+            output = output.rsplit(':', 1)[-1]
         matched = re.search("^ ?([\d\.]+)", output)
         if matched:
             try:
                 score = float(matched.group(1))
             except:
                 score = 0
         else:
-            score = 0
+            if ':' in output:
+                output = output.rsplit(':', 1)[-1]
+                matched = re.search("^ ?([\d\.]+)", output)
+                if matched:
+                    try:
+                        score = float(matched.group(1))
+                    except:
+                        score = 0
+            else:
+                score = 0
         return score
 
     @staticmethod
     def normalize_score(score):
         max_score = 5  # Maximum possible score
         normalized_score = score / max_score
         return normalized_score
@@ -42,23 +53,25 @@
                 prompt = readfile.read()
         except:
             prompt = mapping[metric][1]
 
         cur_prompt = prompt.replace('{{Document}}', answer).replace('{{Summary}}', summary)
         return cur_prompt
 
-    def score(self, question, answer=None, samples=None):
+    def score(self, question, answer=None, samples=None, summary=None):
         scores = {}
+        samples = []
         if not answer:
             answer = self.ask_llm(question)[0]
         answer = answer.strip()
-        summary_prompt = f"Create a summary with 20 maximum words from {answer}"
-        summary = self.ask_llm(summary_prompt)[0].strip()
-
+        if not summary:
+            summary_prompt = f"Create a summary with 20 maximum words from {answer}"
+            summary = self.ask_llm(summary_prompt)[0].strip()
         for metric in self.metrics:
             prompt = self.create_prompt(answer, summary, metric)
-            answers = self.ask_llm(prompt, n=int(os.getenv("GEVAL_SAMPLING_NUMBER", 5)))
-
+            answers = self.ask_llm(prompt, n=int(os.getenv("GEVAL_SAMPLING_NUMBER", 20)))
+            samples.append(answers)
             all_scores = [self.parse_output(x.strip()) for x in answers]
             score = sum(all_scores) / len(all_scores)
             scores[metric.title()] = float("{:.2f}".format(self.normalize_score(score)))
-        return scores, answer, []
+        scores['Overall'] = float("{:.2f}".format(sum([v for k, v in scores.items()])/len(scores)))
+        return scores, answer, samples
```

### Comparing `halludetector-0.0.8/halludetector/detectors/refchecker.py` & `halludetector-0.0.9/halludetector/detectors/refchecker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .base import Detector
 
 
 class RefChecker(Detector):
     def __init__(self):
         super().__init__()
 
-    def score(self, question=None, answer=None, samples=None):
+    def score(self, question=None, answer=None, samples=None, summary=None):
         if not question:
             question = self.generate_question(answer)
 
         if not answer:
             answer = self.ask_llm(question.strip())[0]
 
         triplets = self.extract_triplets(answer, question, max_new_tokens=200)
```

### Comparing `halludetector-0.0.8/halludetector/detectors/selfcheckgpt.py` & `halludetector-0.0.9/halludetector/detectors/selfcheckgpt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import logging
 import os
 import spacy
 import numpy as np
 from selfcheckgpt.modeling_selfcheck import SelfCheckMQAG
 
 from .base import Detector
-
+from ..prompts.default import DEFAULT_SELFCHECK_WITH_PROMPT_PROMPT
 
 logger = logging.getLogger(__name__)
 
 
 class SelfCheckGPTBertScore(Detector):
 
     def __init__(self):
         super().__init__()
         self.sample_number = int(os.getenv("BERT_SCORE_SAMPLING_NUMBER", 3))
 
-    def score(self, question, answer=None, samples=None):
+    def score(self, question, answer=None, samples=None, summary=None):
         if not answer:
             answer = self.ask_llm(question)[0]
 
         sentences = self.extract_sentences(answer)
         sentences = [s.text for s in sentences]
         if not samples:
             samples = self.ask_llm(question, n=self.sample_number, temperature=0.4)
@@ -38,15 +38,15 @@
 
 class SelfCheckGPTNGram(Detector):
 
     def __init__(self):
         super().__init__()
         self.sample_number = int(os.getenv("NGRAM_SAMPLING_NUMBER", 3))
 
-    def score(self, question, answer=None, samples=None):
+    def score(self, question, answer=None, samples=None, summary=None):
         if not answer:
             answer = self.ask_llm(question)[0]
 
         sentences = self.extract_sentences(answer)
         sentences = [s.text for s in sentences]
         if not samples:
             samples = self.ask_llm(question, n=self.sample_number, temperature=0.4)
@@ -62,18 +62,18 @@
 
 
 class SelfCheckGPTPrompt(Detector):
 
     def __init__(self):
         super().__init__()
         self.sample_number = int(os.getenv("PROMPT_SAMPLING_NUMBER", 3))
-        self.prompt_template = "Context: {context}\n\nSentence: {sentence}\n\nIs the sentence supported by the context above? Answer Yes or No.\n\nAnswer: "
+        self.prompt_template = DEFAULT_SELFCHECK_WITH_PROMPT_PROMPT
         self.text_mapping = {'yes': 0.0, 'no': 1.0, 'n/a': 0.5}
 
-    def score(self, question, answer=None, samples=None):
+    def score(self, question, answer=None, samples=None, summary=None):
 
         if not answer:
             answer = self.ask_llm(question)[0]
 
         if not samples:
             samples = self.ask_llm(question, n=self.sample_number, temperature=0.4)
 
@@ -124,15 +124,15 @@
 
     def __init__(self):
         import torch
         device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
         self.scorer = SelfCheckMQAG(device=device)
         self.sample_number = 3
 
-    def score(self, question, answer=None, samples=None):
+    def score(self, question, answer=None, samples=None, summary=None):
         samples = []
         if not answer:
             answer = self.ask_llm(question)[0]
 
         nlp = spacy.load("en_core_web_sm")
         sentences = [sent.text.strip() for sent in nlp(answer).sents]
```

### Comparing `halludetector-0.0.8/halludetector/extractor/claude2_extractor.py` & `halludetector-0.0.9/halludetector/extractor/gpt4_extractor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from .extractor_base import ExtractorBase
-from ..utils import get_claude2_response
 
 
-CLAUDE2_TRIPLET_EXTRACTION_PROMPT_Q = \
-"""Given a question and a candidate answer to the question, please extract a KG from the candidate answer condition on the question and represent the KG with triples formatted with ("subject", "predicate", "object"), each triplet in a line.
+GPT4_TRIPLET_EXTRACTION_PROMPT_Q = \
+"""Given a question and a candidate answer to the question, please extract a KG from the candidate answer condition on the question and represent the KG with triples formatted with ("subject", "predicate", "object").
 Please note that this is an EXTRACTION task, so DO NOT care about whether the content of the candidate answer is factual or not, just extract the triplets from it.
 
 Here are some in-context examples:
 
 ### Question:
 Given these paragraphs about the Tesla bot, what is its alias?
 
@@ -40,15 +39,15 @@
 
 ### Candidate Answer:
 {a}
 
 ### KG:
 """
 
-CLAUDE2_TRIPLET_EXTRACTION_PROMPT = \
+GPT4_TRIPLET_EXTRACTION_PROMPT = \
 """Given an input text, please extract a KG from the text and represent the KG with triples formatted with ("subject", "predicate", "object"), each triplet in a line. Please note that this is an EXTRACTION task, so DO NOT care about whether the content of the candidate answer is factual or not, just extract the triplets from it.
 
 Here are some in-context examples:
 
 ### Input:
 Optimus (or Tesla Bot) is a robotic humanoid under development by Tesla, Inc. It was announced at the company's Artificial Intelligence (AI) Day event on August 19, 2021.
 
@@ -77,44 +76,42 @@
 ### Input:
 {input_text}
 
 ### KG:
 """
 
 
-class Claude2Extractor(ExtractorBase):
+class GPT4Extractor(ExtractorBase):
     def __init__(
         self,
-        claim_format:str='triplet'
+        llm_handler,
+        claim_format: str = 'triplet'
     ) -> None:
         super().__init__(claim_format=claim_format)
-        
         if self.claim_format == 'triplet':
-            self.prompt_temp_wq = CLAUDE2_TRIPLET_EXTRACTION_PROMPT_Q
-            self.prompt_temp = CLAUDE2_TRIPLET_EXTRACTION_PROMPT
-
+            self.prompt_temp_wq = GPT4_TRIPLET_EXTRACTION_PROMPT_Q
+            self.prompt_temp = GPT4_TRIPLET_EXTRACTION_PROMPT
+        self.llm_handler = llm_handler
+    
     def extract_claim_triplets(self, response, question=None, max_new_tokens=500):
         if question is None:
             prompt = self.prompt_temp.format(
                 input_text=response
             )
         else:
             prompt = self.prompt_temp_wq.format(
                 q=question,
                 a=response
             )
-
-        claude2_response = get_claude2_response(
-            prompt=prompt,
-            temperature=0,
+        gpt4_response = self.llm_handler.ask_llm(
+            prompt,
             max_new_tokens=max_new_tokens
-        )
-
-        if claude2_response and len(claude2_response):
+        )[0]
+        if gpt4_response and len(gpt4_response):
             kg_str = None
-            if '###' in claude2_response:
-                kg_str = claude2_response[:claude2_response.index('###')]
+            if '###' in gpt4_response:
+                kg_str = gpt4_response[:gpt4_response.index('###')]
             else:
-                kg_str = claude2_response
+                kg_str = gpt4_response
             triplets = self._parse_claim_triplets(kg_str)
             return triplets
         return []
```

### Comparing `halludetector-0.0.8/halludetector/extractor/extractor.py` & `halludetector-0.0.9/halludetector/extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.8/halludetector/extractor/extractor_base.py` & `halludetector-0.0.9/halludetector/extractor/extractor_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 
 
 class ExtractorBase:
     def __init__(
         self,
-        claim_format:str='triplet'
+        claim_format: str = 'triplet'
     ) -> None:
         self.claim_format = claim_format
 
     def extract(self, response, question=None, max_new_tokens=500):
         claims = None
         if self.claim_format == 'triplet':
             claims = self.extract_claim_triplets(
```

### Comparing `halludetector-0.0.8/halludetector/generators/question.py` & `halludetector-0.0.9/halludetector/generators/question.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.8/halludetector/llm/mistral.py` & `halludetector-0.0.9/halludetector/llm/mistral.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.8/halludetector/llm/openai.py` & `halludetector-0.0.9/halludetector/llm/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 logger = logging.getLogger(__name__)
 
 
 class OpenAIHandler:
     def __init__(self):
         self.client = OpenAI(api_key=os.getenv('OPENAI_API_KEY'))
 
-    def ask_llm(self, prompt, n=1, temperature=0, max_new_tokens=int(os.getenv("OPENAI_MAX_TOKENS", 400))):
+    def ask_llm(self, prompt, n=1, temperature=0.5, max_new_tokens=int(os.getenv("OPENAI_MAX_TOKENS", 400))):
         response = self.client.completions.create(
             model=os.getenv("OPENAI_MODEL", "gpt-3.5-turbo-instruct"),
             prompt=prompt,
             max_tokens=max_new_tokens,
             n=n,
-            temperature=temperature
+            temperature=temperature,
+
         )
         results = [r.text.strip() for r in response.choices]
         logger.info(f'Prompt responses: {results}')
         return results
```

### Comparing `halludetector-0.0.8/halludetector/prompts/default.py` & `halludetector-0.0.9/halludetector/prompts/default.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,8 +139,12 @@
 Completion: {completion}
 It was based on this question:
 Question: {question}
 Use chain of thought to explain the completion. Rebuild the completion using your answer and check again if the completion is right.
 It is mandatory that your first word in your response is yes or no as the response of the following question.
 It is mandatory to explain yourself after.
 Does this completion contain hallucinations?
+'''
+
+DEFAULT_SELFCHECK_WITH_PROMPT_PROMPT = '''
+"Context: {context}\n\nSentence: {sentence}\n\nIs the sentence supported by the context above? Answer Yes or No.\n\nAnswer: "
 '''
```

### Comparing `halludetector-0.0.8/halludetector/retrievers/google_retriever.py` & `halludetector-0.0.9/halludetector/retrievers/google_retriever.py`

 * *Files identical despite different names*

### Comparing `halludetector-0.0.8/halludetector/scorer.py` & `halludetector-0.0.9/halludetector/scorer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import logging
 
 from halludetector.detectors import (
     ChainPoll, SelfCheckGPTBertScore,
     SelfCheckGPTNGram, SelfCheckGPTMQAG,
-    RefChecker, GEval, CustomDetector,
+    RefChecker, GEval,
     SelfCheckGPTPrompt
 )
 
 scorer_mapping = {
     'Self-Check GPT Bert Score': SelfCheckGPTBertScore,
     'Self-Check GPT NGram': SelfCheckGPTNGram,
     'Self-Check GPT Prompt': SelfCheckGPTPrompt,
     'RefChecker': RefChecker,
     'G-Eval': GEval,
     'Chain Poll': ChainPoll,
-    'Custom': CustomDetector
 }
 
 logger = logging.getLogger(__name__)
 
 
-def calculate_score(method, question, answer=None, samples=None):
+def calculate_score(method, question, answer=None, samples=None, summary=None):
     scorer_class = scorer_mapping.get(method)
     if scorer_class:
         scorer = scorer_class()
-    return scorer.score(question, answer, samples)
+    return scorer.score(question, answer, samples, summary)
```

### Comparing `halludetector-0.0.8/halludetector.egg-info/SOURCES.txt` & `halludetector-0.0.9/halludetector.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-README.md
 README.rst
 setup.py
 halludetector/__init__.py
 halludetector/config.py
 halludetector/scorer.py
 halludetector.egg-info/PKG-INFO
 halludetector.egg-info/SOURCES.txt
@@ -14,31 +13,29 @@
 halludetector/checker/checker_base.py
 halludetector/checker/gpt4_checker.py
 halludetector/datasets/__init__.py
 halludetector/datasets/covid_qa.py
 halludetector/datasets/databricks_dolly.py
 halludetector/datasets/drop.py
 halludetector/datasets/parser.py
+halludetector/datasets/summeval.py
 halludetector/detectors/__init__.py
 halludetector/detectors/base.py
 halludetector/detectors/chainpoll.py
-halludetector/detectors/custom.py
 halludetector/detectors/geval.py
 halludetector/detectors/refchecker.py
 halludetector/detectors/selfcheckgpt.py
 halludetector/extractor/__init__.py
-halludetector/extractor/claude2_extractor.py
 halludetector/extractor/extractor.py
 halludetector/extractor/extractor_base.py
 halludetector/extractor/gpt4_extractor.py
-halludetector/extractor/mistral_extractor.py
-halludetector/extractor/mixtral_extractor.py
 halludetector/generators/__init__.py
 halludetector/generators/question.py
 halludetector/llm/__init__.py
+halludetector/llm/cohere.py
 halludetector/llm/mistral.py
 halludetector/llm/openai.py
 halludetector/prompts/__init__.py
 halludetector/prompts/default.py
 halludetector/retrievers/__init__.py
 halludetector/retrievers/google_retriever.py
 halludetector/retrievers/retriever.py
```

### Comparing `halludetector-0.0.8/setup.py` & `halludetector-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 requirements = parse_requirements('requirements.txt')
 
 
 setup(
     name='halludetector',
-    version='0.0.8',
+    version='0.0.9',
     author='Mihai Onofrei',
     author_email='monofrei@cisco.com',
     url='https://github.com/Mihai-Onofrei/Hallucination-detector',  # Replace with your project's URL
     license='MIT',  # Choose an appropriate license
     description="Hallucination detection package",
     long_description=open('README.rst').read(),
     include_package_data=True,
```

