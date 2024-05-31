# Comparing `tmp/ares_ai-0.5.9.tar.gz` & `tmp/ares_ai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ares_ai-0.5.9.tar", last modified: Thu May 30 03:20:40 2024, max compression
+gzip compressed data, was "ares_ai-0.6.0.tar", last modified: Fri May 31 19:02:48 2024, max compression
```

## Comparing `ares_ai-0.5.9.tar` & `ares_ai-0.6.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.367965 ares_ai-0.5.9/
--rw-rw-rw-   0 manihani (23549) future   (20099)     5118 2024-05-21 10:25:44.000000 ares_ai-0.5.9/.gitignore
--rw-rw-rw-   0 manihani (23549) future   (20099)      268 2024-04-22 03:39:34.000000 ares_ai-0.5.9/CHANGELOG.md
--rw-rw-rw-   0 manihani (23549) future   (20099)    11357 2024-01-08 23:19:52.000000 ares_ai-0.5.9/LICENSE
--rw-rw-rw-   0 manihani (23549) future   (20099)       51 2024-04-25 23:18:28.000000 ares_ai-0.5.9/MANIFEST.in
--rw-r--r--   0 manihani (23549) future   (20099)    28521 2024-05-30 03:20:40.366965 ares_ai-0.5.9/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)    12913 2024-05-30 02:01:56.000000 ares_ai-0.5.9/README.md
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.234971 ares_ai-0.5.9/ares/
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.245971 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/
--rw-rw-rw-   0 manihani (23549) future   (20099)    10726 2024-05-15 09:28:04.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    39458 2024-05-20 03:54:50.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    26352 2024-05-16 09:44:16.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    27757 2024-05-15 04:45:07.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__init__.py
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.265970 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)     7375 2024-05-15 22:43:28.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9231 2024-05-07 02:24:59.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    27821 2024-05-20 22:16:50.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    37386 2024-05-07 02:24:59.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    19424 2024-05-16 10:41:36.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    21777 2024-05-07 02:24:37.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    18303 2024-05-15 07:02:35.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    17731 2024-05-07 02:24:59.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      159 2024-04-24 01:00:10.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      175 2024-05-07 02:24:37.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2243 2024-04-24 05:41:16.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     2109 2024-04-22 03:39:34.000000 ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.278969 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/
--rw-rw-rw-   0 manihani (23549) future   (20099)    55776 2024-05-15 03:08:44.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    65867 2024-05-30 03:04:39.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py
--rw-rw-rw-   0 manihani (23549) future   (20099)       36 2024-05-18 12:00:35.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/Prepare_FinanceBench.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    18046 2024-04-22 03:39:34.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     7091 2024-04-30 23:25:14.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__init__.py
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.306968 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)    31119 2024-05-15 03:09:09.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    32115 2024-05-07 02:30:43.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    39869 2024-05-30 03:04:51.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    49640 2024-05-07 02:25:02.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     7856 2024-04-24 01:01:09.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    19694 2024-05-07 02:25:08.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     4250 2024-04-30 23:25:39.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9532 2024-05-07 02:25:08.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      158 2024-04-24 01:01:00.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      174 2024-05-07 02:25:02.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     5437 2024-01-20 22:01:06.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      172 2024-05-07 22:44:26.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/counter.cpython-310.pyc
--rw-r--r--   0 manihani (23549) future   (20099)    17791 2024-05-21 10:44:15.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    19175 2024-05-07 02:25:02.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      494 2024-01-20 21:58:30.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/test.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    21593 2024-05-21 10:43:03.000000 ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/ppi.py
--rw-rw-rw-   0 manihani (23549) future   (20099)       22 2024-04-22 03:39:34.000000 ares_ai-0.5.9/ares/__init__.py
--rw-r--r--   0 manihani (23549) future   (20099)      152 2024-03-25 00:40:39.000000 ares_ai-0.5.9/ares/__init__.pyc
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.335966 ares_ai-0.5.9/ares/__pycache__/
--rw-rw-rw-   0 manihani (23549) future   (20099)      166 2024-04-24 01:00:10.000000 ares_ai-0.5.9/ares/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      196 2024-05-07 02:24:37.000000 ares_ai-0.5.9/ares/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 manihani (23549) future   (20099)     8166 2024-05-21 06:03:02.000000 ares_ai-0.5.9/ares/__pycache__/ares.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    10977 2024-05-07 02:55:57.000000 ares_ai-0.5.9/ares/__pycache__/ares.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     5615 2024-05-15 22:43:28.000000 ares_ai-0.5.9/ares/__pycache__/binary_classifier.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     7124 2024-05-07 02:24:59.000000 ares_ai-0.5.9/ares/__pycache__/binary_classifier.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      371 2024-04-24 01:01:09.000000 ares_ai-0.5.9/ares/__pycache__/kilt_filter.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      469 2024-05-07 02:25:08.000000 ares_ai-0.5.9/ares/__pycache__/kilt_filter.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     1908 2024-05-13 22:37:10.000000 ares_ai-0.5.9/ares/__pycache__/prompts.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     4836 2024-05-30 02:34:05.000000 ares_ai-0.5.9/ares/__pycache__/rag_scoring.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     3941 2024-05-07 02:25:02.000000 ares_ai-0.5.9/ares/__pycache__/rag_scoring.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      356 2024-04-24 01:01:09.000000 ares_ai-0.5.9/ares/__pycache__/superglue_filter.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)      442 2024-05-07 02:25:08.000000 ares_ai-0.5.9/ares/__pycache__/superglue_filter.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     4330 2024-05-16 10:41:36.000000 ares_ai-0.5.9/ares/__pycache__/synthetic_generator.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     3518 2024-05-07 02:24:37.000000 ares_ai-0.5.9/ares/__pycache__/synthetic_generator.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)     9413 2024-05-15 09:11:08.000000 ares_ai-0.5.9/ares/__pycache__/ues_idp.cpython-310.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    10990 2024-05-07 03:18:13.000000 ares_ai-0.5.9/ares/__pycache__/ues_idp.cpython-311.pyc
--rw-rw-rw-   0 manihani (23549) future   (20099)    11647 2024-05-21 06:01:01.000000 ares_ai-0.5.9/ares/ares.py
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.345966 ares_ai-0.5.9/ares/ares_ai.egg-info/
--rw-r--r--   0 manihani (23549) future   (20099)    26304 2024-04-05 05:20:31.000000 ares_ai-0.5.9/ares/ares_ai.egg-info/PKG-INFO
--rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-05 05:20:31.000000 ares_ai-0.5.9/ares/ares_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-05 05:20:31.000000 ares_ai-0.5.9/ares/ares_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-05 05:20:31.000000 ares_ai-0.5.9/ares/ares_ai.egg-info/entry_points.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)      627 2024-04-05 05:20:31.000000 ares_ai-0.5.9/ares/ares_ai.egg-info/requires.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-05 05:20:31.000000 ares_ai-0.5.9/ares/ares_ai.egg-info/top_level.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)     8374 2024-05-15 22:27:43.000000 ares_ai-0.5.9/ares/binary_classifier.py
--rw-rw-rw-   0 manihani (23549) future   (20099)      154 2024-04-22 03:39:34.000000 ares_ai-0.5.9/ares/kilt_filter.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     1862 2024-05-13 05:25:48.000000 ares_ai-0.5.9/ares/prompts.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     8523 2024-05-30 02:06:37.000000 ares_ai-0.5.9/ares/rag_scoring.py
--rw-rw-rw-   0 manihani (23549) future   (20099)      134 2024-04-22 03:39:34.000000 ares_ai-0.5.9/ares/superglue_filter.py
--rw-rw-rw-   0 manihani (23549) future   (20099)     5844 2024-05-16 09:46:01.000000 ares_ai-0.5.9/ares/synthetic_generator.py
--rw-rw-rw-   0 manihani (23549) future   (20099)    15573 2024-05-15 09:10:54.000000 ares_ai-0.5.9/ares/ues_idp.py
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.362965 ares_ai-0.5.9/ares_ai.egg-info/
--rw-r--r--   0 manihani (23549) future   (20099)    28521 2024-05-30 03:20:31.000000 ares_ai-0.5.9/ares_ai.egg-info/PKG-INFO
--rw-r--r--   0 manihani (23549) future   (20099)     4238 2024-05-30 03:20:40.000000 ares_ai-0.5.9/ares_ai.egg-info/SOURCES.txt
--rw-r--r--   0 manihani (23549) future   (20099)        1 2024-05-30 03:20:31.000000 ares_ai-0.5.9/ares_ai.egg-info/dependency_links.txt
--rw-r--r--   0 manihani (23549) future   (20099)       43 2024-05-30 03:20:31.000000 ares_ai-0.5.9/ares_ai.egg-info/entry_points.txt
--rw-r--r--   0 manihani (23549) future   (20099)      706 2024-05-30 03:20:31.000000 ares_ai-0.5.9/ares_ai.egg-info/requires.txt
--rw-r--r--   0 manihani (23549) future   (20099)        5 2024-05-30 03:20:31.000000 ares_ai-0.5.9/ares_ai.egg-info/top_level.txt
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.358965 ares_ai-0.5.9/checkpoints/
--rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:34.000000 ares_ai-0.5.9/checkpoints/.gitignore
--rw-rw-rw-   0 manihani (23549) future   (20099)     2966 2024-05-30 01:53:53.000000 ares_ai-0.5.9/pyproject.toml
--rw-rw-rw-   0 manihani (23549) future   (20099)     5082 2024-05-30 02:07:52.000000 ares_ai-0.5.9/requirements.txt
--rw-rw-rw-   0 manihani (23549) future   (20099)       93 2024-05-30 03:20:40.370965 ares_ai-0.5.9/setup.cfg
-drwxr-sr-x   0 manihani (23549) future   (20099)        0 2024-05-30 03:20:40.360965 ares_ai-0.5.9/tests/
--rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:53.000000 ares_ai-0.5.9/tests/.gitignore
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-31 19:02:48.753399 ares_ai-0.6.0/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5118 2024-05-21 10:25:44.000000 ares_ai-0.6.0/.gitignore
+-rw-rw-rw-   0 manihani (23549) future   (20099)      268 2024-04-22 03:39:34.000000 ares_ai-0.6.0/CHANGELOG.md
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11357 2024-01-08 23:19:52.000000 ares_ai-0.6.0/LICENSE
+-rw-rw-rw-   0 manihani (23549) future   (20099)       51 2024-04-25 23:18:28.000000 ares_ai-0.6.0/MANIFEST.in
+-rw-r--r--   0 manihani (23549) future   (20099)    28521 2024-05-31 19:02:48.752399 ares_ai-0.6.0/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)    12913 2024-05-30 02:01:56.000000 ares_ai-0.6.0/README.md
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-31 19:02:48.538408 ares_ai-0.6.0/ares/
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-31 19:02:48.553408 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/
+-rw-rw-rw-   0 manihani (23549) future   (20099)    10726 2024-05-15 09:28:04.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    39458 2024-05-20 03:54:50.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    26352 2024-05-16 09:44:16.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    27757 2024-05-15 04:45:07.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__init__.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-31 19:02:48.582406 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7375 2024-05-15 22:43:28.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9231 2024-05-07 02:24:59.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    27821 2024-05-20 22:16:50.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    37386 2024-05-07 02:24:59.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    19424 2024-05-16 10:41:36.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    21777 2024-05-07 02:24:37.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    18303 2024-05-15 07:02:35.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    17731 2024-05-07 02:24:59.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      159 2024-04-24 01:00:10.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      175 2024-05-07 02:24:37.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2243 2024-04-24 05:41:16.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2109 2024-04-22 03:39:34.000000 ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-31 19:02:48.603405 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/
+-rw-rw-rw-   0 manihani (23549) future   (20099)    57034 2024-05-31 19:01:47.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    65867 2024-05-30 03:04:39.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)       36 2024-05-18 12:00:35.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/Prepare_FinanceBench.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    18046 2024-04-22 03:39:34.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7091 2024-04-30 23:25:14.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-22 03:39:34.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__init__.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-31 19:02:48.664403 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)    31119 2024-05-15 03:09:09.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    32115 2024-05-07 02:30:43.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    39869 2024-05-30 03:04:51.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    49640 2024-05-07 02:25:02.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7856 2024-04-24 01:01:09.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    19694 2024-05-07 02:25:08.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     4250 2024-04-30 23:25:39.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9532 2024-05-07 02:25:08.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      158 2024-04-24 01:01:00.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      174 2024-05-07 02:25:02.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5437 2024-01-20 22:01:06.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      172 2024-05-07 22:44:26.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/counter.cpython-310.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)    17791 2024-05-21 10:44:15.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    19175 2024-05-07 02:25:02.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      494 2024-01-20 21:58:30.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/test.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    21593 2024-05-21 10:43:03.000000 ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/ppi.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)       22 2024-04-22 03:39:34.000000 ares_ai-0.6.0/ares/__init__.py
+-rw-r--r--   0 manihani (23549) future   (20099)      152 2024-03-25 00:40:39.000000 ares_ai-0.6.0/ares/__init__.pyc
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-31 19:02:48.705401 ares_ai-0.6.0/ares/__pycache__/
+-rw-rw-rw-   0 manihani (23549) future   (20099)      166 2024-04-24 01:00:10.000000 ares_ai-0.6.0/ares/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      196 2024-05-07 02:24:37.000000 ares_ai-0.6.0/ares/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 manihani (23549) future   (20099)     8166 2024-05-21 06:03:02.000000 ares_ai-0.6.0/ares/__pycache__/ares.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    10977 2024-05-07 02:55:57.000000 ares_ai-0.6.0/ares/__pycache__/ares.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5615 2024-05-15 22:43:28.000000 ares_ai-0.6.0/ares/__pycache__/binary_classifier.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     7124 2024-05-07 02:24:59.000000 ares_ai-0.6.0/ares/__pycache__/binary_classifier.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      371 2024-04-24 01:01:09.000000 ares_ai-0.6.0/ares/__pycache__/kilt_filter.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      469 2024-05-07 02:25:08.000000 ares_ai-0.6.0/ares/__pycache__/kilt_filter.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     1908 2024-05-13 22:37:10.000000 ares_ai-0.6.0/ares/__pycache__/prompts.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4836 2024-05-30 02:34:05.000000 ares_ai-0.6.0/ares/__pycache__/rag_scoring.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     3941 2024-05-07 02:25:02.000000 ares_ai-0.6.0/ares/__pycache__/rag_scoring.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      356 2024-04-24 01:01:09.000000 ares_ai-0.6.0/ares/__pycache__/superglue_filter.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)      442 2024-05-07 02:25:08.000000 ares_ai-0.6.0/ares/__pycache__/superglue_filter.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     4330 2024-05-16 10:41:36.000000 ares_ai-0.6.0/ares/__pycache__/synthetic_generator.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     3518 2024-05-07 02:24:37.000000 ares_ai-0.6.0/ares/__pycache__/synthetic_generator.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)     9413 2024-05-15 09:11:08.000000 ares_ai-0.6.0/ares/__pycache__/ues_idp.cpython-310.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    10990 2024-05-07 03:18:13.000000 ares_ai-0.6.0/ares/__pycache__/ues_idp.cpython-311.pyc
+-rw-rw-rw-   0 manihani (23549) future   (20099)    11647 2024-05-21 06:01:01.000000 ares_ai-0.6.0/ares/ares.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-31 19:02:48.721400 ares_ai-0.6.0/ares/ares_ai.egg-info/
+-rw-r--r--   0 manihani (23549) future   (20099)    26304 2024-04-05 05:20:31.000000 ares_ai-0.6.0/ares/ares_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0 manihani (23549) future   (20099)        0 2024-04-05 05:20:31.000000 ares_ai-0.6.0/ares/ares_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        1 2024-04-05 05:20:31.000000 ares_ai-0.6.0/ares/ares_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       43 2024-04-05 05:20:31.000000 ares_ai-0.6.0/ares/ares_ai.egg-info/entry_points.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)      627 2024-04-05 05:20:31.000000 ares_ai-0.6.0/ares/ares_ai.egg-info/requires.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)        5 2024-04-05 05:20:31.000000 ares_ai-0.6.0/ares/ares_ai.egg-info/top_level.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)     8374 2024-05-15 22:27:43.000000 ares_ai-0.6.0/ares/binary_classifier.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)      154 2024-04-22 03:39:34.000000 ares_ai-0.6.0/ares/kilt_filter.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     1862 2024-05-13 05:25:48.000000 ares_ai-0.6.0/ares/prompts.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     8523 2024-05-30 02:06:37.000000 ares_ai-0.6.0/ares/rag_scoring.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)      134 2024-04-22 03:39:34.000000 ares_ai-0.6.0/ares/superglue_filter.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5844 2024-05-16 09:46:01.000000 ares_ai-0.6.0/ares/synthetic_generator.py
+-rw-rw-rw-   0 manihani (23549) future   (20099)    15573 2024-05-15 09:10:54.000000 ares_ai-0.6.0/ares/ues_idp.py
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-31 19:02:48.748399 ares_ai-0.6.0/ares_ai.egg-info/
+-rw-r--r--   0 manihani (23549) future   (20099)    28521 2024-05-31 19:02:42.000000 ares_ai-0.6.0/ares_ai.egg-info/PKG-INFO
+-rw-r--r--   0 manihani (23549) future   (20099)     4238 2024-05-31 19:02:48.000000 ares_ai-0.6.0/ares_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 manihani (23549) future   (20099)        1 2024-05-31 19:02:42.000000 ares_ai-0.6.0/ares_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 manihani (23549) future   (20099)       43 2024-05-31 19:02:42.000000 ares_ai-0.6.0/ares_ai.egg-info/entry_points.txt
+-rw-r--r--   0 manihani (23549) future   (20099)      706 2024-05-31 19:02:42.000000 ares_ai-0.6.0/ares_ai.egg-info/requires.txt
+-rw-r--r--   0 manihani (23549) future   (20099)        5 2024-05-31 19:02:42.000000 ares_ai-0.6.0/ares_ai.egg-info/top_level.txt
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-31 19:02:48.743399 ares_ai-0.6.0/checkpoints/
+-rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:34.000000 ares_ai-0.6.0/checkpoints/.gitignore
+-rw-rw-rw-   0 manihani (23549) future   (20099)     2966 2024-05-31 19:02:30.000000 ares_ai-0.6.0/pyproject.toml
+-rw-rw-rw-   0 manihani (23549) future   (20099)     5082 2024-05-30 02:07:52.000000 ares_ai-0.6.0/requirements.txt
+-rw-rw-rw-   0 manihani (23549) future   (20099)       93 2024-05-31 19:02:48.756399 ares_ai-0.6.0/setup.cfg
+drwxrwsrwx   0 manihani (23549) future   (20099)        0 2024-05-31 19:02:48.745399 ares_ai-0.6.0/tests/
+-rw-rw-rw-   0 manihani (23549) future   (20099)       71 2024-04-22 03:39:53.000000 ares_ai-0.6.0/tests/.gitignore
```

### Comparing `ares_ai-0.5.9/.gitignore` & `ares_ai-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/LICENSE` & `ares_ai-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/PKG-INFO` & `ares_ai-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ares-ai
-Version: 0.5.9
+Version: 0.6.0
 Summary: ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 Author-email: Jon Saad-Falcon <jonsaadfalcon@stanford.edu>, Robby Manihani <manihani@stanford.edu>, Omar Khattab <okhattab@stanford.edu>, Christopher Potts <cgpotts@stanford.edu>, Matei Zaharia <matei@berkeley.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ares_ai-0.5.9/README.md` & `ares_ai-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py` & `ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/Filter_Synthetic_Queries.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py` & `ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/General_Binary_Classifier.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py` & `ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/Generate_Synthetic_Queries_and_Answers.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py` & `ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/LLM_Generation_Functions.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc` & `ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc` & `ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/Filter_Synthetic_Queries.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc` & `ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc` & `ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/General_Binary_Classifier.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc` & `ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc` & `ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/Generate_Synthetic_Queries_and_Answers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc` & `ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc` & `ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/LLM_Generation_Functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc` & `ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/__pycache__/pytorchtools.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py` & `ares_ai-0.6.0/ares/LLM_as_a_Judge_Adaptation/pytorchtools.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/Evaluation_Functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,21 @@
 import openai
 from together import Together
 from datasets import Dataset
 from openai import OpenAI
 from sklearn.model_selection import train_test_split
 from tqdm import tqdm
 from transformers import AutoTokenizer, AutoModelForSeq2SeqLM, AutoConfig, AutoModelForCausalLM
-from vllm import LLM
+
+try:
+    from vllm import LLM
+    VLLM_AVAILABLE = True
+except ImportError:
+    VLLM_AVAILABLE = False
+    print("vLLM not imported.")
 
 def calculate_accuracy(predictions, ground_truth) -> float:
     """
     Calculate the accuracy percentage between predictions and ground truths.
 
     Args:
     predictions (list): A list of predicted values.
@@ -941,314 +947,315 @@
             if attempt < 4:  # Only print the error message if not on the last attempt
                 print(f"Attempt {attempt + 1} failed with error: {e}")
                 time.sleep(60)  # Sleep for 60 seconds before retrying
             else:
                 print("All attempts failed. Last error was:", e)
                 return 0
 
-def few_shot_context_relevance_scoring_vllm(
-    system_prompt: str, query: str, document: str, model_choice: str, 
-    query_id: str, debug_mode: bool, host_url: str, request_delay: int, 
-    failed_extraction_count: Dict[str,int] = {'failed': 0}, 
-    few_shot_examples=None
-) -> int:
-    """
-    Evaluates the relevance of a query given a document using few-shot examples.
-    This function constructs a user prompt with few-shot examples (if provided) and the current query,
-    document, and answer. It then queries a local vLLM model to determine if the query is context relevant to the
-    document.
-
-    Args:
-    system_prompt (str): The prompt for the system role in the conversation.
-    query (str): The query to be evaluated.
-    document (str): The document to be evaluated.
-    model_choice (str): The model identifier for vLLM's model.
-    query_id (str): The identifier for the query column in few_shot_examples.
-    debug_mode (bool): Flag to turn on debug mode for additional output.
-    host_url (str): The URL is used to send requests to the locally running model.
-    request_delay (int): Time in seconds to delay the request (simulating network latency).
-    failed_extraction_count (Dict[str, int]): A dictionary to count the number of failed extractions.
-    few_shot_examples (DataFrame, optional): A DataFrame containing few-shot examples.
-
-    Returns:
-    int: The label indicating context relevance (1 for relevant, 0 for not relevant).
-
-    Raises:
-    Warning: If incorrect labels are detected in the few-shot examples.
-    """
-    for attempt in range(5):
-        try:
-            user_prompt = ""
-            if few_shot_examples is not None:
-                for row in range(len(few_shot_examples)):
-                    user_prompt += f"Question: {few_shot_examples.iloc[row][query_id]}\n"
-                    user_prompt += f"Document: {few_shot_examples.iloc[row]['Document']}\n"
-                    current_label = few_shot_examples.iloc[row]['Context_Relevance_Label']
-                    if current_label in {1, 1.0}:
-                        warnings.warn("Incorrect label '1' detected. Please use '[[Yes]]' instead.")
-                        current_label = "[[Yes]]"
-                    elif current_label in {0, 0.0}:
-                        warnings.warn("Incorrect label '0' detected. Please use '[[No]]' instead.")
-                        current_label = "[[No]]"
-                    user_prompt += "Label: " + str(current_label) + "\n\n"
-            
-            user_prompt += f"Question: {query}\nDocument: {document}\nLabel: "
-
-            time.sleep(request_delay)
-
-            if debug_mode: 
-                print("------------------------------------------")
-                print("Context Relevance Evaluation:")
-                print(user_prompt)
-            
-            openai_api_key = "EMPTY"
-            client = OpenAI(
-            api_key=openai_api_key,
-            base_url=host_url
-            )
-
-            chat_completion = client.chat.completions.create(
-            messages=[
-                {
-                "role": "system",
-                "content": system_prompt,
-                },
-                {
-                "role": "user",
-                "content": user_prompt,
-                }
-            ],
-            model=model_choice
-            )
-            final_response = chat_completion.choices[0].message.content
-
-            if debug_mode: 
-                print(final_response)
-
-            yes = r"\[\s*\[?\s*Yes\s*\]?\s*\]"
-            no = r"\[\s*\[?\s*No\s*\]?\s*\]"
-
-            if re.search(yes, final_response): 
-                if debug_mode:
-                    print("Returned label 1")
-                return 1
-            elif re.search(no, final_response):
-                if debug_mode:
-                    print("Returned label 0")
-                return 0
-            else:
-                print("Didn't extract Yes or No!")
-                failed_extraction_count['failed'] += 1
-                return 0
-        except Exception as e:
-            if attempt < 4:  # Only print the error message if not on the last attempt
-                print(f"Attempt {attempt + 1} failed with error: {e}")
-                time.sleep(60)  # Sleep for 60 seconds before retrying
-            else:
-                print("All attempts failed. Last error was:", e)
-                return 0
-    
-def few_shot_answer_faithfulness_scoring_vllm(
-    system_prompt: str, query: str, document: str, answer: str, model_choice: str, 
-    query_id: str, debug_mode: bool, host_url: str, request_delay: int, 
-    failed_extraction_count: Dict[str,int] = {'failed': 0}, 
-    few_shot_examples=None
-) -> int:
-    """
-    Evaluates the faithfulness of an answer given a document and a query using few-shot examples.
-    This function constructs a user prompt with few-shot examples (if provided) and the current query,
-    document, and answer. It then queries a local vLLM model to determine if the answer is faithful.
-
-    Args:
-    system_prompt (str): The prompt for the system role in the conversation.
-    query (str): The query related to the document.
-    document (str): The document to be evaluated.
-    answer (str): The answer to be evaluated for faithfulness.
-    model_choice (str): The model identifier for vLLM's model.
-    query_id (str): The identifier for the query column in few_shot_examples.
-    debug_mode (bool): Flag to turn on debug mode for additional output.
-    host_url (str): The URL is used to send requests to the locally running model.
-    request_delay (int): Time in seconds to delay the request (simulating network latency).
-    failed_extraction_count (Dict[str, int]): A dictionary to count the number of failed extractions.
-    few_shot_examples (DataFrame, optional): A DataFrame containing few-shot examples.
-
-    Returns:
-    int: The label indicating answer faithfulness 1 if the answer is faithful, 0 otherwise.
-
-    Raises:
-    Warning: If incorrect labels are detected in the few-shot examples.
-    """
-    for attempt in range(5):
-        try:
-            user_prompt = ""
-            if few_shot_examples is not None:
-                for row in range(len(few_shot_examples)):
-                    user_prompt += f"Question: {few_shot_examples.iloc[row][query_id]}\n"
-                    user_prompt += f"Document: {few_shot_examples.iloc[row]['Document']}\n"
-                    user_prompt += f"Answer: {few_shot_examples.iloc[row]['Answer']}\n"
-                    current_label = few_shot_examples.iloc[row]['Answer_Faithfulness_Label']
-                    if current_label in {1, 1.0}:
-                        warnings.warn("Incorrect label '1' detected. Please use '[[Yes]]' instead.")
-                        current_label = "[[Yes]]"
-                    elif current_label in {0, 0.0}:
-                        warnings.warn("Incorrect label '0' detected. Please use '[[No]]' instead.")
-                        current_label = "[[No]]"
-                    user_prompt += "Label: " + str(current_label) + "\n\n"
-
-            user_prompt += f"Question: {query}\nDocument: {document}\nAnswer: {answer}\nLabel: "
+if VLLM_AVAILABLE:
+    def few_shot_context_relevance_scoring_vllm(
+        system_prompt: str, query: str, document: str, model_choice: str, 
+        query_id: str, debug_mode: bool, host_url: str, request_delay: int, 
+        failed_extraction_count: Dict[str,int] = {'failed': 0}, 
+        few_shot_examples=None
+    ) -> int:
+        """
+        Evaluates the relevance of a query given a document using few-shot examples.
+        This function constructs a user prompt with few-shot examples (if provided) and the current query,
+        document, and answer. It then queries a local vLLM model to determine if the query is context relevant to the
+        document.
+
+        Args:
+        system_prompt (str): The prompt for the system role in the conversation.
+        query (str): The query to be evaluated.
+        document (str): The document to be evaluated.
+        model_choice (str): The model identifier for vLLM's model.
+        query_id (str): The identifier for the query column in few_shot_examples.
+        debug_mode (bool): Flag to turn on debug mode for additional output.
+        host_url (str): The URL is used to send requests to the locally running model.
+        request_delay (int): Time in seconds to delay the request (simulating network latency).
+        failed_extraction_count (Dict[str, int]): A dictionary to count the number of failed extractions.
+        few_shot_examples (DataFrame, optional): A DataFrame containing few-shot examples.
+
+        Returns:
+        int: The label indicating context relevance (1 for relevant, 0 for not relevant).
+
+        Raises:
+        Warning: If incorrect labels are detected in the few-shot examples.
+        """
+        for attempt in range(5):
+            try:
+                user_prompt = ""
+                if few_shot_examples is not None:
+                    for row in range(len(few_shot_examples)):
+                        user_prompt += f"Question: {few_shot_examples.iloc[row][query_id]}\n"
+                        user_prompt += f"Document: {few_shot_examples.iloc[row]['Document']}\n"
+                        current_label = few_shot_examples.iloc[row]['Context_Relevance_Label']
+                        if current_label in {1, 1.0}:
+                            warnings.warn("Incorrect label '1' detected. Please use '[[Yes]]' instead.")
+                            current_label = "[[Yes]]"
+                        elif current_label in {0, 0.0}:
+                            warnings.warn("Incorrect label '0' detected. Please use '[[No]]' instead.")
+                            current_label = "[[No]]"
+                        user_prompt += "Label: " + str(current_label) + "\n\n"
+                
+                user_prompt += f"Question: {query}\nDocument: {document}\nLabel: "
+
+                time.sleep(request_delay)
+
+                if debug_mode: 
+                    print("------------------------------------------")
+                    print("Context Relevance Evaluation:")
+                    print(user_prompt)
+                
+                openai_api_key = "EMPTY"
+                client = OpenAI(
+                api_key=openai_api_key,
+                base_url=host_url
+                )
 
-            time.sleep(request_delay) # Model query delay chosen by user
+                chat_completion = client.chat.completions.create(
+                messages=[
+                    {
+                    "role": "system",
+                    "content": system_prompt,
+                    },
+                    {
+                    "role": "user",
+                    "content": user_prompt,
+                    }
+                ],
+                model=model_choice
+                )
+                final_response = chat_completion.choices[0].message.content
 
-            if debug_mode: 
-                print("------------------------------------------")
-                print("Answer Faithfulness Evaluation")
-                print(user_prompt)
+                if debug_mode: 
+                    print(final_response)
 
-            openai_api_key = "EMPTY"
-            client = OpenAI(
-            api_key=openai_api_key,
-            base_url=host_url
-            )
+                yes = r"\[\s*\[?\s*Yes\s*\]?\s*\]"
+                no = r"\[\s*\[?\s*No\s*\]?\s*\]"
 
-            chat_completion = client.chat.completions.create(
-            messages=[
-                {
-                "role": "system",
-                "content": system_prompt,
-                },
-                {
-                "role": "user",
-                "content": user_prompt,
-                }
-            ],
-            model=model_choice
-            )
-            final_response = chat_completion.choices[0].message.content
-            
-            if debug_mode: 
-                print(final_response)
-
-            yes = r"\[\s*\[?\s*Yes\s*\]?\s*\]"
-            no = r"\[\s*\[?\s*No\s*\]?\s*\]"
-            
-            if re.search(yes, final_response): 
-                if debug_mode:
-                    print("Returned label 1")
-                return 1
-            elif re.search(no, final_response):
-                if debug_mode:
-                    print("Returned label 0")
-                return 0
-            else:
-                print("Didn't extract Yes or No!")
-                failed_extraction_count['failed'] += 1
-                return 0
-        except Exception as e:
-            if attempt < 4:  # Only print the error message if not on the last attempt
-                print(f"Attempt {attempt + 1} failed with error: {e}")
-                time.sleep(60)  # Sleep for 60 seconds before retrying
-            else:
-                print("All attempts failed. Last error was:", e)
-                return 0
+                if re.search(yes, final_response): 
+                    if debug_mode:
+                        print("Returned label 1")
+                    return 1
+                elif re.search(no, final_response):
+                    if debug_mode:
+                        print("Returned label 0")
+                    return 0
+                else:
+                    print("Didn't extract Yes or No!")
+                    failed_extraction_count['failed'] += 1
+                    return 0
+            except Exception as e:
+                if attempt < 4:  # Only print the error message if not on the last attempt
+                    print(f"Attempt {attempt + 1} failed with error: {e}")
+                    time.sleep(60)  # Sleep for 60 seconds before retrying
+                else:
+                    print("All attempts failed. Last error was:", e)
+                    return 0
         
-def few_shot_answer_relevance_scoring_vllm(
-    system_prompt: str, query: str, document: str, answer: str, model_choice: str, 
-    query_id: str, debug_mode: bool, host_url: str, request_delay: int, 
-    failed_extraction_count: Dict[str,int] = {'failed': 0}, 
-    few_shot_examples=None
-) -> int:
-    """
-    Evaluates the relevance of an answer given a document and a query using few-shot examples.
-    This function constructs a user prompt with few-shot examples (if provided) and the current query,
-    document, and answer. It then queries a local vLLM model to determine if the answer is relevant.
+    def few_shot_answer_faithfulness_scoring_vllm(
+        system_prompt: str, query: str, document: str, answer: str, model_choice: str, 
+        query_id: str, debug_mode: bool, host_url: str, request_delay: int, 
+        failed_extraction_count: Dict[str,int] = {'failed': 0}, 
+        few_shot_examples=None
+    ) -> int:
+        """
+        Evaluates the faithfulness of an answer given a document and a query using few-shot examples.
+        This function constructs a user prompt with few-shot examples (if provided) and the current query,
+        document, and answer. It then queries a local vLLM model to determine if the answer is faithful.
+
+        Args:
+        system_prompt (str): The prompt for the system role in the conversation.
+        query (str): The query related to the document.
+        document (str): The document to be evaluated.
+        answer (str): The answer to be evaluated for faithfulness.
+        model_choice (str): The model identifier for vLLM's model.
+        query_id (str): The identifier for the query column in few_shot_examples.
+        debug_mode (bool): Flag to turn on debug mode for additional output.
+        host_url (str): The URL is used to send requests to the locally running model.
+        request_delay (int): Time in seconds to delay the request (simulating network latency).
+        failed_extraction_count (Dict[str, int]): A dictionary to count the number of failed extractions.
+        few_shot_examples (DataFrame, optional): A DataFrame containing few-shot examples.
+
+        Returns:
+        int: The label indicating answer faithfulness 1 if the answer is faithful, 0 otherwise.
+
+        Raises:
+        Warning: If incorrect labels are detected in the few-shot examples.
+        """
+        for attempt in range(5):
+            try:
+                user_prompt = ""
+                if few_shot_examples is not None:
+                    for row in range(len(few_shot_examples)):
+                        user_prompt += f"Question: {few_shot_examples.iloc[row][query_id]}\n"
+                        user_prompt += f"Document: {few_shot_examples.iloc[row]['Document']}\n"
+                        user_prompt += f"Answer: {few_shot_examples.iloc[row]['Answer']}\n"
+                        current_label = few_shot_examples.iloc[row]['Answer_Faithfulness_Label']
+                        if current_label in {1, 1.0}:
+                            warnings.warn("Incorrect label '1' detected. Please use '[[Yes]]' instead.")
+                            current_label = "[[Yes]]"
+                        elif current_label in {0, 0.0}:
+                            warnings.warn("Incorrect label '0' detected. Please use '[[No]]' instead.")
+                            current_label = "[[No]]"
+                        user_prompt += "Label: " + str(current_label) + "\n\n"
+
+                user_prompt += f"Question: {query}\nDocument: {document}\nAnswer: {answer}\nLabel: "
+
+                time.sleep(request_delay) # Model query delay chosen by user
+
+                if debug_mode: 
+                    print("------------------------------------------")
+                    print("Answer Faithfulness Evaluation")
+                    print(user_prompt)
+
+                openai_api_key = "EMPTY"
+                client = OpenAI(
+                api_key=openai_api_key,
+                base_url=host_url
+                )
 
-    Args:
-    system_prompt (str): The prompt for the system role in the conversation.
-    query (str): The query related to the document.
-    document (str): The document to be evaluated.
-    answer (str): The answer to be evaluated for relevance.
-    model_choice (str): The model identifier for vLLM's model.
-    query_id (str): The identifier for the query column in few_shot_examples.
-    debug_mode (bool): Flag to turn on debug mode for additional output.
-    host_url (str): The URL is used to send requests to the locally running model.
-    request_delay (int): Time in seconds to delay the request (simulating network latency).
-    failed_extraction_count (Dict[str, int]): A dictionary to count the number of failed extractions.
-    few_shot_examples (DataFrame, optional): A DataFrame containing few-shot examples.
-
-    Returns:
-    int: The label indicating answer relevance 1 if the answer is relevant, 0 otherwise.
-
-    Raises:
-    Warning: If incorrect labels are detected in the few-shot examples.
-    """
-    for attempt in range(5):
-        try:
-            user_prompt = ""
-            if few_shot_examples is not None:
-                for row in range(len(few_shot_examples)):
-                    user_prompt += f"Question: {few_shot_examples.iloc[row][query_id]}\n"
-                    user_prompt += f"Document: {few_shot_examples.iloc[row]['Document']}\n"
-                    user_prompt += f"Answer: {few_shot_examples.iloc[row]['Answer']}\n"
-                    current_label = few_shot_examples.iloc[row]['Answer_Relevance_Label']
-                    if current_label in {1, 1.0}:
-                        warnings.warn("Incorrect label '1' detected. Please use '[[Yes]]' instead.")
-                        current_label = "[[Yes]]"
-                    elif current_label in {0, 0.0}:
-                        warnings.warn("Incorrect label '0' detected. Please use '[[No]]' instead.")
-                        current_label = "[[No]]"
-                    user_prompt += "Label: " + str(current_label) + "\n\n"
-            
-            user_prompt += f"Question: {query}\nDocument: {document}\nAnswer: {answer}\nLabel: "
-
-            time.sleep(request_delay) # Model query delay chosen by user
-
-            if debug_mode: 
-                print("------------------------------------------")
-                print("Answer Relevance Evaluation")
-                print(user_prompt)
-
-            openai_api_key = "EMPTY"
-            client = OpenAI(
-            api_key=openai_api_key,
-            base_url=host_url
-            )
-
-            chat_completion = client.chat.completions.create(
-            messages=[
-                {
-                "role": "system",
-                "content": system_prompt,
-                },
-                {
-                "role": "user",
-                "content": user_prompt,
-                }
-            ],
-            model=model_choice
-            )
-            final_response = chat_completion.choices[0].message.content
-            
-            if debug_mode is True: 
-                print(final_response)
+                chat_completion = client.chat.completions.create(
+                messages=[
+                    {
+                    "role": "system",
+                    "content": system_prompt,
+                    },
+                    {
+                    "role": "user",
+                    "content": user_prompt,
+                    }
+                ],
+                model=model_choice
+                )
+                final_response = chat_completion.choices[0].message.content
+                
+                if debug_mode: 
+                    print(final_response)
+
+                yes = r"\[\s*\[?\s*Yes\s*\]?\s*\]"
+                no = r"\[\s*\[?\s*No\s*\]?\s*\]"
+                
+                if re.search(yes, final_response): 
+                    if debug_mode:
+                        print("Returned label 1")
+                    return 1
+                elif re.search(no, final_response):
+                    if debug_mode:
+                        print("Returned label 0")
+                    return 0
+                else:
+                    print("Didn't extract Yes or No!")
+                    failed_extraction_count['failed'] += 1
+                    return 0
+            except Exception as e:
+                if attempt < 4:  # Only print the error message if not on the last attempt
+                    print(f"Attempt {attempt + 1} failed with error: {e}")
+                    time.sleep(60)  # Sleep for 60 seconds before retrying
+                else:
+                    print("All attempts failed. Last error was:", e)
+                    return 0
+            
+    def few_shot_answer_relevance_scoring_vllm(
+        system_prompt: str, query: str, document: str, answer: str, model_choice: str, 
+        query_id: str, debug_mode: bool, host_url: str, request_delay: int, 
+        failed_extraction_count: Dict[str,int] = {'failed': 0}, 
+        few_shot_examples=None
+    ) -> int:
+        """
+        Evaluates the relevance of an answer given a document and a query using few-shot examples.
+        This function constructs a user prompt with few-shot examples (if provided) and the current query,
+        document, and answer. It then queries a local vLLM model to determine if the answer is relevant.
+
+        Args:
+        system_prompt (str): The prompt for the system role in the conversation.
+        query (str): The query related to the document.
+        document (str): The document to be evaluated.
+        answer (str): The answer to be evaluated for relevance.
+        model_choice (str): The model identifier for vLLM's model.
+        query_id (str): The identifier for the query column in few_shot_examples.
+        debug_mode (bool): Flag to turn on debug mode for additional output.
+        host_url (str): The URL is used to send requests to the locally running model.
+        request_delay (int): Time in seconds to delay the request (simulating network latency).
+        failed_extraction_count (Dict[str, int]): A dictionary to count the number of failed extractions.
+        few_shot_examples (DataFrame, optional): A DataFrame containing few-shot examples.
+
+        Returns:
+        int: The label indicating answer relevance 1 if the answer is relevant, 0 otherwise.
+
+        Raises:
+        Warning: If incorrect labels are detected in the few-shot examples.
+        """
+        for attempt in range(5):
+            try:
+                user_prompt = ""
+                if few_shot_examples is not None:
+                    for row in range(len(few_shot_examples)):
+                        user_prompt += f"Question: {few_shot_examples.iloc[row][query_id]}\n"
+                        user_prompt += f"Document: {few_shot_examples.iloc[row]['Document']}\n"
+                        user_prompt += f"Answer: {few_shot_examples.iloc[row]['Answer']}\n"
+                        current_label = few_shot_examples.iloc[row]['Answer_Relevance_Label']
+                        if current_label in {1, 1.0}:
+                            warnings.warn("Incorrect label '1' detected. Please use '[[Yes]]' instead.")
+                            current_label = "[[Yes]]"
+                        elif current_label in {0, 0.0}:
+                            warnings.warn("Incorrect label '0' detected. Please use '[[No]]' instead.")
+                            current_label = "[[No]]"
+                        user_prompt += "Label: " + str(current_label) + "\n\n"
+                
+                user_prompt += f"Question: {query}\nDocument: {document}\nAnswer: {answer}\nLabel: "
+
+                time.sleep(request_delay) # Model query delay chosen by user
+
+                if debug_mode: 
+                    print("------------------------------------------")
+                    print("Answer Relevance Evaluation")
+                    print(user_prompt)
+
+                openai_api_key = "EMPTY"
+                client = OpenAI(
+                api_key=openai_api_key,
+                base_url=host_url
+                )
 
-            yes = r"\[\s*\[?\s*Yes\s*\]?\s*\]"
-            no = r"\[\s*\[?\s*No\s*\]?\s*\]"
-            
-            if re.search(yes, final_response): 
-                if debug_mode is True:
-                    print("Returned label 1")
-                return 1
-            elif re.search(no, final_response):
-                if debug_mode is True:
-                    print("Returned label 0")
-                return 0
-            else:
-                print("Didn't extract Yes or No!")
-                failed_extraction_count['failed'] += 1
-                return 0
-        except Exception as e:
-            if attempt < 4:  # Only print the error message if not on the last attempt
-                print(f"Attempt {attempt + 1} failed with error: {e}")
-                time.sleep(60)  # Sleep for 60 seconds before retrying
-            else:
-                print("All attempts failed. Last error was:", e)
-                return 0
+                chat_completion = client.chat.completions.create(
+                messages=[
+                    {
+                    "role": "system",
+                    "content": system_prompt,
+                    },
+                    {
+                    "role": "user",
+                    "content": user_prompt,
+                    }
+                ],
+                model=model_choice
+                )
+                final_response = chat_completion.choices[0].message.content
+                
+                if debug_mode is True: 
+                    print(final_response)
+
+                yes = r"\[\s*\[?\s*Yes\s*\]?\s*\]"
+                no = r"\[\s*\[?\s*No\s*\]?\s*\]"
+                
+                if re.search(yes, final_response): 
+                    if debug_mode is True:
+                        print("Returned label 1")
+                    return 1
+                elif re.search(no, final_response):
+                    if debug_mode is True:
+                        print("Returned label 0")
+                    return 0
+                else:
+                    print("Didn't extract Yes or No!")
+                    failed_extraction_count['failed'] += 1
+                    return 0
+            except Exception as e:
+                if attempt < 4:  # Only print the error message if not on the last attempt
+                    print(f"Attempt {attempt + 1} failed with error: {e}")
+                    time.sleep(60)  # Sleep for 60 seconds before retrying
+                else:
+                    print("All attempts failed. Last error was:", e)
+                    return 0
```

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/LLMJudge_RAG_Compared_Scoring.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/Prepare_KILT_Dataset.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/Prepare_SuperGLUE_Datasets.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/Evaluation_Functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/LLMJudge_RAG_Compared_Scoring.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_KILT_Dataset.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/Prepare_SuperGLUE_Datasets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/ares.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/__pycache__/ppi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/RAG_Automatic_Evaluation/ppi.py` & `ares_ai-0.6.0/ares/RAG_Automatic_Evaluation/ppi.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/__pycache__/ares.cpython-310.pyc` & `ares_ai-0.6.0/ares/__pycache__/ares.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/__pycache__/ares.cpython-311.pyc` & `ares_ai-0.6.0/ares/__pycache__/ares.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/__pycache__/binary_classifier.cpython-310.pyc` & `ares_ai-0.6.0/ares/__pycache__/binary_classifier.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/__pycache__/binary_classifier.cpython-311.pyc` & `ares_ai-0.6.0/ares/__pycache__/binary_classifier.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/__pycache__/prompts.cpython-310.pyc` & `ares_ai-0.6.0/ares/__pycache__/prompts.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/__pycache__/rag_scoring.cpython-310.pyc` & `ares_ai-0.6.0/ares/__pycache__/rag_scoring.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/__pycache__/rag_scoring.cpython-311.pyc` & `ares_ai-0.6.0/ares/__pycache__/rag_scoring.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/__pycache__/synthetic_generator.cpython-310.pyc` & `ares_ai-0.6.0/ares/__pycache__/synthetic_generator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/__pycache__/synthetic_generator.cpython-311.pyc` & `ares_ai-0.6.0/ares/__pycache__/synthetic_generator.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/__pycache__/ues_idp.cpython-310.pyc` & `ares_ai-0.6.0/ares/__pycache__/ues_idp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/__pycache__/ues_idp.cpython-311.pyc` & `ares_ai-0.6.0/ares/__pycache__/ues_idp.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/ares.py` & `ares_ai-0.6.0/ares/ares.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/ares_ai.egg-info/PKG-INFO` & `ares_ai-0.6.0/ares/ares_ai.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/ares_ai.egg-info/requires.txt` & `ares_ai-0.6.0/ares/ares_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/binary_classifier.py` & `ares_ai-0.6.0/ares/binary_classifier.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/prompts.py` & `ares_ai-0.6.0/ares/prompts.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/rag_scoring.py` & `ares_ai-0.6.0/ares/rag_scoring.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/synthetic_generator.py` & `ares_ai-0.6.0/ares/synthetic_generator.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares/ues_idp.py` & `ares_ai-0.6.0/ares/ues_idp.py`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares_ai.egg-info/PKG-INFO` & `ares_ai-0.6.0/ares_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ares-ai
-Version: 0.5.9
+Version: 0.6.0
 Summary: ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 Author-email: Jon Saad-Falcon <jonsaadfalcon@stanford.edu>, Robby Manihani <manihani@stanford.edu>, Omar Khattab <okhattab@stanford.edu>, Christopher Potts <cgpotts@stanford.edu>, Matei Zaharia <matei@berkeley.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `ares_ai-0.5.9/ares_ai.egg-info/SOURCES.txt` & `ares_ai-0.6.0/ares_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/ares_ai.egg-info/requires.txt` & `ares_ai-0.6.0/ares_ai.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `ares_ai-0.5.9/pyproject.toml` & `ares_ai-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ares-ai"
-version = "0.5.9"
+version = "0.6.0"
 description = """ 
 ARES is an advanced evaluation framework for Retrieval-Augmented Generation (RAG) systems, 
 utilizing fine-tuned classifiers and synthetic data to assess performance efficiently. It streamlines 
 the evaluation of context relevance, answer faithfulness, and answer relevance with minimal human annotations.
 """
 readme = "README.md"
 authors = [
```

### Comparing `ares_ai-0.5.9/requirements.txt` & `ares_ai-0.6.0/requirements.txt`

 * *Files identical despite different names*

