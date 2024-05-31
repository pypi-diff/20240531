# Comparing `tmp/ragelo-0.1.1.tar.gz` & `tmp/ragelo-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragelo-0.1.1.tar", last modified: Tue Apr 16 10:38:23 2024, max compression
+gzip compressed data, was "ragelo-0.1.2.tar", last modified: Fri May 31 10:07:17 2024, max compression
```

## Comparing `ragelo-0.1.1.tar` & `ragelo-0.1.2.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.040865 ragelo-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 10:38:14.000000 ragelo-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-16 10:38:23.040865 ragelo-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-04-16 10:38:14.000000 ragelo-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-16 10:38:14.000000 ragelo-0.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.028865 ragelo-0.1.1/ragelo/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.028865 ragelo-0.1.1/ragelo/agent_rankers/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/agent_rankers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/agent_rankers/base_agent_ranker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/agent_rankers/elo_ranker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.032865 ragelo-0.1.1/ragelo/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/cli/agent_rankers_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/cli/answer_evaluators_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/cli/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/cli/retrieval_evaluator_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.032865 ragelo-0.1.1/ragelo/evaluators/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.032865 ragelo-0.1.1/ragelo/evaluators/answer_evaluators/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/answer_evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8734 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/answer_evaluators/base_answer_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/answer_evaluators/custom_prompt_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/answer_evaluators/pairwise_reasoning_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12512 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/base_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.032865 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7901 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/base_retrieval_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/custom_prompt_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7618 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/domain_expert_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/few_shot_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/rdnam_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/reasoner_evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.036865 ragelo-0.1.1/ragelo/llm_providers/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/llm_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/llm_providers/base_llm_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/llm_providers/openai_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.036865 ragelo-0.1.1/ragelo/types/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.036865 ragelo-0.1.1/ragelo/types/configurations/
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/configurations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/configurations/agent_ranker_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/configurations/answer_evaluator_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/configurations/base_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/configurations/llm_provider_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/configurations/retrieval_evaluator_configs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/types/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-04-16 10:38:14.000000 ragelo-0.1.1/ragelo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.036865 ragelo-0.1.1/ragelo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-16 10:38:23.000000 ragelo-0.1.1/ragelo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-16 10:38:23.000000 ragelo-0.1.1/ragelo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 10:38:23.000000 ragelo-0.1.1/ragelo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-16 10:38:23.000000 ragelo-0.1.1/ragelo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-16 10:38:23.000000 ragelo-0.1.1/ragelo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 10:38:23.000000 ragelo-0.1.1/ragelo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 10:38:23.040865 ragelo-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.036865 ragelo-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-16 10:38:14.000000 ragelo-0.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 10:38:23.036865 ragelo-0.1.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-16 10:38:14.000000 ragelo-0.1.1/tests/unit/test_answer_evaluators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-16 10:38:14.000000 ragelo-0.1.1/tests/unit/test_llm_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12893 2024-04-16 10:38:14.000000 ragelo-0.1.1/tests/unit/test_retrieval_evaluators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:07:17.073305 ragelo-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-31 10:07:12.000000 ragelo-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-05-31 10:07:17.073305 ragelo-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-05-31 10:07:12.000000 ragelo-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-05-31 10:07:12.000000 ragelo-0.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:07:17.065305 ragelo-0.1.2/ragelo/
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:07:17.065305 ragelo-0.1.2/ragelo/agent_rankers/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/agent_rankers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4978 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/agent_rankers/base_agent_ranker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/agent_rankers/elo_ranker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:07:17.065305 ragelo-0.1.2/ragelo/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/cli/agent_rankers_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/cli/answer_evaluators_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/cli/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/cli/retrieval_evaluator_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:07:17.065305 ragelo-0.1.2/ragelo/evaluators/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/evaluators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:07:17.069305 ragelo-0.1.2/ragelo/evaluators/answer_evaluators/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/evaluators/answer_evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/evaluators/answer_evaluators/base_answer_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/evaluators/answer_evaluators/custom_prompt_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4329 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/evaluators/answer_evaluators/domain_expert_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/evaluators/answer_evaluators/pairwise_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21974 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/evaluators/base_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:07:17.069305 ragelo-0.1.2/ragelo/evaluators/retrieval_evaluators/
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/evaluators/retrieval_evaluators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11057 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/evaluators/retrieval_evaluators/base_retrieval_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/evaluators/retrieval_evaluators/custom_prompt_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/evaluators/retrieval_evaluators/domain_expert_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/evaluators/retrieval_evaluators/few_shot_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/evaluators/retrieval_evaluators/rdnam_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/evaluators/retrieval_evaluators/reasoner_evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:07:17.069305 ragelo-0.1.2/ragelo/llm_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/llm_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3776 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/llm_providers/base_llm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/llm_providers/openai_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:07:17.069305 ragelo-0.1.2/ragelo/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:07:17.069305 ragelo-0.1.2/ragelo/types/configurations/
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/types/configurations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/types/configurations/agent_ranker_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/types/configurations/answer_evaluator_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/types/configurations/base_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/types/configurations/llm_provider_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/types/configurations/retrieval_evaluator_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/types/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12456 2024-05-31 10:07:12.000000 ragelo-0.1.2/ragelo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:07:17.073305 ragelo-0.1.2/ragelo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10708 2024-05-31 10:07:17.000000 ragelo-0.1.2/ragelo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-05-31 10:07:17.000000 ragelo-0.1.2/ragelo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 10:07:17.000000 ragelo-0.1.2/ragelo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-31 10:07:17.000000 ragelo-0.1.2/ragelo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-31 10:07:17.000000 ragelo-0.1.2/ragelo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-31 10:07:17.000000 ragelo-0.1.2/ragelo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 10:07:17.073305 ragelo-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:07:17.069305 ragelo-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8763 2024-05-31 10:07:12.000000 ragelo-0.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:07:17.073305 ragelo-0.1.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-05-31 10:07:12.000000 ragelo-0.1.2/tests/unit/test_answer_evaluators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-31 10:07:12.000000 ragelo-0.1.2/tests/unit/test_llm_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13102 2024-05-31 10:07:12.000000 ragelo-0.1.2/tests/unit/test_retrieval_evaluators.py
```

### Comparing `ragelo-0.1.1/LICENSE` & `ragelo-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ragelo-0.1.1/PKG-INFO` & `ragelo-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragelo
-Version: 0.1.1
+Version: 0.1.2
 Summary: RAGElo: A Tool for Evaluating Retrieval-Augmented Generation Models
 Author-email: Zeta Alpha <support@zeta-alpha.com>, Arthur Câmara <camara@zeta-alpha.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/zetaalphavector/RAGElo
 Project-URL: Repository, https://github.com/zetaalphavector/RAGElo
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -32,14 +32,15 @@
 Requires-Dist: flake8==6.1.0; extra == "dev"
 Requires-Dist: flake8-black==0.3.6; extra == "dev"
 Requires-Dist: flake8-isort==6.1.0; extra == "dev"
 Requires-Dist: mypy==1.9.0; extra == "dev"
 Requires-Dist: Flake8-pyproject==1.2.3; extra == "dev"
 Requires-Dist: types-tqdm==4.66.0; extra == "dev"
 Requires-Dist: pydantic==2.7.0; extra == "dev"
+Requires-Dist: pytest-asyncio==0.23.6; extra == "dev"
 
 
 <h1 align="center">
 <img style="vertical-align:middle" src="https://raw.githubusercontent.com/zetaalphavector/RAGElo/master/docs/images/RAGElo_logo.png" height="200">
 </h1>
 
 <p  align="center" >
@@ -72,17 +73,17 @@
 
 ```python
 from ragelo import get_retrieval_evaluator
 
 evaluator = get_retrieval_evaluator("RDNAM", llm_provider="openai")
 raw_answer, processed_answer = evaluator.evaluate(query="What is the capital of France?", document='Lyon is the second largest city in France.')
 print(processed_answer)
-# Output: 0
+# Output: 1
 print(raw_answer)
-# Output: '"O": 0\n}'
+# Output: '"O": 1\n}'
 ```
 
 For a more complete example, we can evaluate with a custom prompt, and inject metadata into our evaluation prompt:
 
 ```python
 from ragelo import get_retrieval_evaluator
```

### Comparing `ragelo-0.1.1/README.md` & `ragelo-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -33,17 +33,17 @@
 
 ```python
 from ragelo import get_retrieval_evaluator
 
 evaluator = get_retrieval_evaluator("RDNAM", llm_provider="openai")
 raw_answer, processed_answer = evaluator.evaluate(query="What is the capital of France?", document='Lyon is the second largest city in France.')
 print(processed_answer)
-# Output: 0
+# Output: 1
 print(raw_answer)
-# Output: '"O": 0\n}'
+# Output: '"O": 1\n}'
 ```
 
 For a more complete example, we can evaluate with a custom prompt, and inject metadata into our evaluation prompt:
 
 ```python
 from ragelo import get_retrieval_evaluator
```

### Comparing `ragelo-0.1.1/pyproject.toml` & `ragelo-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     "flake8==6.1.0",
     "flake8-black==0.3.6",
     "flake8-isort==6.1.0",
     "mypy==1.9.0",
     "Flake8-pyproject==1.2.3",
     "types-tqdm==4.66.0",
     "pydantic==2.7.0",
+    "pytest-asyncio==0.23.6",
 ]
 
 [project.scripts]
 ragelo = "ragelo.cli:app"
 
 [project.urls]
 Homepage = "https://github.com/zetaalphavector/RAGElo"
@@ -63,14 +64,14 @@
 warn_redundant_casts = true
 check_untyped_defs = true
 implicit_reexport = true
 exclude = ["build/", "dist/", "venv/"]
 
 
 [tool.flake8]
-ignore = ['E501', "W503"]
+ignore = ['E501', "W503", "E203"]
 per-file-ignores = ['__init__.py:F401,F403']
 exclude = ["build/", "dist/", "venv/"]
 
 
 [tool.setuptools-git-versioning]
 enabled = true
```

### Comparing `ragelo-0.1.1/ragelo/__init__.py` & `ragelo-0.1.2/ragelo/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """CLI for automatically evaluating Retrieval Augmented Generation (RAG) models."""
 
+from ragelo.agent_rankers.base_agent_ranker import get_agent_ranker
 from ragelo.evaluators.answer_evaluators import (
     AnswerEvaluatorFactory,
     get_answer_evaluator,
 )
 from ragelo.evaluators.retrieval_evaluators import (
     RetrievalEvaluatorFactory,
     get_retrieval_evaluator,
```

### Comparing `ragelo-0.1.1/ragelo/agent_rankers/base_agent_ranker.py` & `ragelo-0.1.2/ragelo/agent_rankers/base_agent_ranker.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,64 +1,69 @@
 """Base models for ranking a set of answers generated by LLMs"""
 
 import csv
-from abc import abstractmethod
 from collections import defaultdict
-from typing import Type
+from typing import Optional, Type, get_type_hints
 
+# from ragelo.agent_rankers import *
 from ragelo.logger import logger
 from ragelo.types import AgentRankerConfig
+from ragelo.types.types import Query
+from ragelo.utils import load_answer_evaluations_from_csv
 
 
 class AgentRanker:
     config: AgentRankerConfig
-    evaluations: list[tuple[str, str, str]]
     ranking: defaultdict[str, list[str]]
     output_file: str = "agents_ranking.csv"
     name: str = "Agent Ranker"
 
     def __init__(
         self,
         config: AgentRankerConfig,
-        evaluations: list[tuple[str, str, str]],
     ):
         self.config = config
-        self.evaluations = evaluations
         self.ranking = defaultdict(list)
-        if config.output_file is not None:
-            self.output_file = config.output_file
+        if self.config.output_file:
+            self.output_file = self.config.output_file
 
-    @staticmethod
-    def load_evaluations(answers_file: str) -> list[tuple[str, str, str]]:
-        evaluations = []
-        with open(answers_file, "r") as f:
-            reader = csv.DictReader(f)
-            for row in reader:
-                agent_a = row["agent_a"]
-                agent_b = row["agent_b"]
-                relevant = row["answer"]
-                evaluations.append((agent_a, agent_b, relevant))
-        return evaluations
+    def run(
+        self,
+        queries: Optional[list[Query]] = None,
+        evaluations_file: Optional[str] = None,
+    ) -> list[Query]:
+        """Compute score for each agent"""
+        raise NotImplementedError
+
+    def _prepare_queries(
+        self,
+        queries: Optional[list[Query]] = None,
+        evaluations_file: Optional[str] = None,
+    ) -> list[Query]:
+        if queries is None:
+            if evaluations_file is None:
+                raise ValueError(
+                    "Either queries or evaluations_file should be provided"
+                )
+            queries = load_answer_evaluations_from_csv(evaluations_file)
+        return queries
 
     @classmethod
     def from_config(cls, config: AgentRankerConfig):
-        evaluations = cls.load_evaluations(config.evaluations_file)
-        return cls(config, evaluations)
-
-    @abstractmethod
-    def run(self):
-        """Compute score for each agent"""
-        raise NotImplementedError
+        return cls(config)
+        # evaluations = cls.load_evaluations(config.evaluations_file)
+        # return cls(config, evaluations)
 
-    @abstractmethod
     def get_agents_ratings(self) -> dict[str, float]:
         """Returns the score of all players"""
         raise NotImplementedError
 
     def dump_ranking(self):
+        if not self.config.write_output:
+            return
         with open(self.output_file, "w") as f:
             writer = csv.writer(f)
             writer.writerow(["agent", "score"])
             for agent, rating in sorted(
                 self.get_agents_ratings().items(), key=lambda x: x[1], reverse=True
             ):
                 writer.writerow([agent, rating])
@@ -83,14 +88,31 @@
                 logger.warning("Rich not installed. Using plain print")
                 self.config.rich_print = False
         if not self.config.rich_print:
             print(f"------- Agent Scores by {self.name} -------")
             for agent, rating in scores:
                 print(f"{agent:<15}: {rating:.1f}")
 
+    @classmethod
+    def get_config_class(cls) -> Type[AgentRankerConfig]:
+        return get_type_hints(cls)["config"]
+
+    def _flatten_evaluations(self, queries) -> list[tuple[str, str, str]]:
+        evaluations = []
+        for q in queries:
+            for game in q.pairwise_games:
+                evaluations.append(
+                    (
+                        game.agent_a_answer.agent,
+                        game.agent_b_answer.agent,
+                        game.evaluation.answer,
+                    )
+                )
+        return evaluations
+
 
 class AgentRankerFactory:
     registry: dict[str, Type[AgentRanker]] = {}
 
     @classmethod
     def register(cls, name: str):
         def inner_wrapper(wrapped_class: Type[AgentRanker]):
@@ -98,11 +120,30 @@
                 logger.warning(f"Overwriting {name} in Answer Evaluator registry")
             cls.registry[name.lower()] = wrapped_class
             return wrapped_class
 
         return inner_wrapper
 
     @classmethod
-    def create(cls, ranker_name: str, config: AgentRankerConfig) -> AgentRanker:
+    def create(
+        cls,
+        ranker_name: str,
+        config: Optional[AgentRankerConfig] = None,
+        **kwargs,
+    ) -> AgentRanker:
         if ranker_name.lower() not in cls.registry:
             raise ValueError(f"Unknown Agent Ranker {ranker_name}")
+        if config is None:
+            class_ = cls.registry[ranker_name.lower()]
+            type_config = class_.get_config_class()
+            valid_keys = [field for field in type_config.get_model_fields()]
+            valid_args = {k: v for k, v in kwargs.items() if k in valid_keys}
+            config = type_config(**valid_args)
         return cls.registry[ranker_name.lower()].from_config(config)
+
+
+def get_agent_ranker(
+    ranker_name: str,
+    config: Optional[AgentRankerConfig] = None,
+    **kwargs,
+) -> AgentRanker:
+    return AgentRankerFactory.create(ranker_name, config, **kwargs)
```

### Comparing `ragelo-0.1.1/ragelo/agent_rankers/elo_ranker.py` & `ragelo-0.1.2/ragelo/agent_rankers/elo_ranker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,61 +1,76 @@
 import random
+from typing import Optional
 
 from ragelo.agent_rankers.base_agent_ranker import AgentRanker, AgentRankerFactory
 from ragelo.logger import logger
 from ragelo.types import EloAgentRankerConfig
+from ragelo.types.types import Query
 
 
 @AgentRankerFactory.register("elo")
 class EloRanker(AgentRanker):
     name: str = "Elo Agent Ranker"
     config: EloAgentRankerConfig
 
     def __init__(
         self,
         config: EloAgentRankerConfig,
-        evaluations: list[tuple[str, str, str]],
     ):
-        super().__init__(config, evaluations)
+        super().__init__(config)
         self.score_map = {"A": 1, "B": 0, "C": 0.5}
 
         self.agents: dict[str, int] = {}
         self.games: list[tuple[str, str, float]] = []
         self.computed = False
         self.initial_score = self.config.initial_score
         self.k = self.config.k
 
-    def run(self):
+    def run(
+        self,
+        queries: Optional[list[Query]] = None,
+        evaluations_file: Optional[str] = None,
+    ):
         """Compute score for each agent"""
-        self.games, self.agents = self.__get_elo_scores()
-
-        while self.games:
-            self.__play_one_game()
+        queries = self._prepare_queries(queries, evaluations_file)
+        self.evaluations = self._flatten_evaluations(queries)
+        agent_scores: dict[str, list[int]] = {}
+        for _ in range(self.config.rounds):
+            self.games = self.__get_elo_scores()
+            while self.games:
+                self.__play_one_game()
+            for a in self.agents:
+                if a not in agent_scores:
+                    agent_scores[a] = []
+                agent_scores[a].append(self.agents[a])
+                self.agents[a] = self.initial_score
+        # Average the scores over all rounds
+        for a in agent_scores:
+            self.agents[a] = sum(agent_scores[a]) // len(agent_scores[a])
         self.dump_ranking()
         self.print_ranking()
 
     def get_agents_ratings(self):
         if not self.computed:
             raise ValueError("Ranking not computed yet, Run evaluate() first")
         return self.agents
 
-    def __get_elo_scores(self) -> tuple[list[tuple[str, str, float]], dict[str, int]]:
+    def __get_elo_scores(self) -> list[tuple[str, str, float]]:
         games: list[tuple[str, str, float]] = []
-        agents = {}
         for agent_a, agent_b, score in self.evaluations:
             score_val = self.score_map[score]
             games.append((agent_a, agent_b, score_val))
             logger.info(f"Game: {agent_a} vs {agent_b} -> {score_val}")
-            if agent_a not in agents:
-                agents[agent_a] = self.initial_score
-            if agent_b not in agents:
-                agents[agent_b] = self.initial_score
+            if agent_a not in self.agents:
+                self.agents[agent_a] = self.initial_score
+            if agent_b not in self.agents:
+                self.agents[agent_b] = self.initial_score
         random.shuffle(games)
         self.computed = True
-        return games, agents
+        return games
 
     def __play_one_game(self):
         player1, player2, result = self.games.pop()
         player1_rating = self.agents[player1]
         player2_rating = self.agents[player2]
         expected_score = self.__expected_score(player1_rating, player2_rating)
```

### Comparing `ragelo-0.1.1/ragelo/cli/agent_rankers_cmd.py` & `ragelo-0.1.2/ragelo/cli/agent_rankers_cmd.py`

 * *Files identical despite different names*

### Comparing `ragelo-0.1.1/ragelo/cli/answer_evaluators_cmd.py` & `ragelo-0.1.2/ragelo/cli/answer_evaluators_cmd.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 def pairwise_reasoning(
     config: PairwiseEvaluatorConfig = PairwiseEvaluatorConfig(), **kwargs
 ):
     """A evaluator that evaluates RAG-based answers pairwise, with document reasoning"""
     config = PairwiseEvaluatorConfig(**kwargs)
     config.query_path = get_path(config.data_path, config.query_path)
     config.answers_path = get_path(config.data_path, config.answers_path)
-    config.output_file = get_path(config.data_path, config.output_file)
+    config.answers_evaluations_path = get_path(
+        config.data_path, config.answers_evaluations_path
+    )
     config.documents_path = get_path(config.data_path, config.documents_path)
 
     llm_provider = get_llm_provider(config.llm_provider, **kwargs)
     evaluator = get_answer_evaluator(
-        AnswerEvaluatorTypes.PAIRWISE_REASONING,
+        AnswerEvaluatorTypes.PAIRWISE,
         config=config,
         llm_provider=llm_provider,
     )
     answers = load_answers_from_csv(config.answers_path, queries=config.query_path)
     evaluator.batch_evaluate(answers)
```

### Comparing `ragelo-0.1.1/ragelo/cli/args.py` & `ragelo-0.1.2/ragelo/cli/args.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Parse arguments for the cli app"""
 
+import collections.abc
 import inspect
-from typing import Any, Callable, get_type_hints
+from typing import Any, Callable, get_args, get_origin, get_type_hints
 
 from typer.models import ArgumentInfo, OptionInfo, ParameterInfo, ParamMeta
 
 from ragelo.types import BaseConfig
 from ragelo.types.configurations.base_configs import _PYDANTIC_MAJOR_VERSION
 
 arguments = {
@@ -17,14 +18,18 @@
     "evaluations_file",
     "retrieval_evaluator_name",
     "answer_evaluator_name",
     "output_file",
 }
 
 
+def callable(value: str):
+    return value
+
+
 def get_params_from_function(func: Callable[..., Any]) -> dict[str, ParamMeta]:
     signature = inspect.signature(func)
 
     type_hints = get_type_hints(func)
 
     params = {}
 
@@ -35,29 +40,37 @@
         if param.name in type_hints:
             annotation = type_hints[param.name]
         if inspect.isclass(annotation) and issubclass(annotation, BaseConfig):
             fields = annotation.get_model_fields()
             for k, v in fields.items():
                 if _PYDANTIC_MAJOR_VERSION == 2:
                     description = v.description  # type: ignore
-                    _type = v.annotation
+                    _type = v.annotation  # type: ignore
                 else:
                     description = v.field_info.description  # type: ignore
-                    _type = v.type_
+                    _type = v.type_  # type: ignore
                 if not isinstance(v, ParameterInfo):
                     # get the description from Pydantic model
+                    parser = None
+                    t_args = get_args(_type)
+                    if (
+                        len(t_args) > 0
+                        and get_origin(t_args[0]) == collections.abc.Callable
+                    ):
+                        parser = callable
                     if k in arguments:
                         argument = ArgumentInfo(default=v.default, help=description)
                         params[k] = ParamMeta(
                             name=k, default=argument, annotation=_type
                         )
                     else:
                         option = OptionInfo(
                             default=v.default,
                             help=description,
+                            parser=parser,
                         )
                         params[k] = ParamMeta(name=k, default=option, annotation=_type)
                 else:
                     params[k] = ParamMeta(name=k, default=v, annotation=_type)
 
         else:
             params[param.name] = ParamMeta(
```

### Comparing `ragelo-0.1.1/ragelo/cli/cli.py` & `ragelo-0.1.2/ragelo/cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
 
     answers_evaluator = get_answer_evaluator(
         "pairwise_reasoning",
         llm_provider=llm_provider,
         output_file=config.evaluations_file,
         **args_clean,
     )
-
     answers_evaluator.batch_evaluate(answers)
 
     ranker_config = EloAgentRankerConfig(
         force=config.force,
         rich_print=config.rich_print,
         verbose=config.verbose,
         output_file=config.output_file,
```

### Comparing `ragelo-0.1.1/ragelo/cli/retrieval_evaluator_cmd.py` & `ragelo-0.1.2/ragelo/cli/retrieval_evaluator_cmd.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,61 +31,63 @@
     ragelo retrieval_evaluator domain_expert queries.csv documents.csv "Chemical Engineering" --company "ChemCorp Inc."
 
     """
 
     config = DomainExpertEvaluatorConfig(**kwargs)
     config.query_path = get_path(config.data_path, config.query_path)
     config.documents_path = get_path(config.data_path, config.documents_path)
-    config.output_file = get_path(config.data_path, config.output_file)
+    config.answers_evaluations_path = get_path(
+        config.data_path, config.answers_evaluations_path
+    )
 
     config.verbose = True
 
     llm_provider = get_llm_provider(config.llm_provider, **kwargs)
     evaluator = get_retrieval_evaluator(
         RetrievalEvaluatorTypes.DOMAIN_EXPERT, config=config, llm_provider=llm_provider
     )
     documents = load_retrieved_docs_from_csv(
         config.documents_path, queries=config.query_path
     )
-
     evaluator.batch_evaluate(documents)
 
 
 @app.command()
 def reasoner(config: ReasonerEvaluatorConfig = ReasonerEvaluatorConfig(), **kwargs):
     """
     A document Evaluator that only outputs the reasoning for why a document is relevant.
     """
     config = ReasonerEvaluatorConfig(**kwargs)
     config.query_path = get_path(config.data_path, config.query_path)
     config.documents_path = get_path(config.data_path, config.documents_path)
-    if not config.output_file:
-        config.output_file = get_path(config.data_path, "reasonings.csv")
-    else:
-        config.output_file = get_path(config.data_path, config.output_file)
+    config.answers_evaluations_path = get_path(
+        config.data_path, config.answers_evaluations_path
+    )
 
     config.verbose = True
     llm_provider = get_llm_provider(config.llm_provider, **kwargs)
     evaluator = get_retrieval_evaluator(
         RetrievalEvaluatorTypes.REASONER, config=config, llm_provider=llm_provider
     )
     documents = load_retrieved_docs_from_csv(
         config.documents_path, queries=config.query_path
     )
-
     evaluator.batch_evaluate(documents)
 
 
 @app.command()
 def rdnam(config: RDNAMEvaluatorConfig = RDNAMEvaluatorConfig(), **kwargs):
     """Evaluator based on the paper by Thomas, Spielman, Craswell and Mitra, Large language models can accurately predict searcher preferences."""
     config = RDNAMEvaluatorConfig(**kwargs)
     config.query_path = get_path(config.data_path, config.query_path)
     config.documents_path = get_path(config.data_path, config.documents_path)
-    config.output_file = get_path(config.data_path, config.output_file)
+    config.answers_evaluations_path = get_path(
+        config.data_path, config.answers_evaluations_path
+    )
+
     config.verbose = True
     llm_provider = get_llm_provider(config.llm_provider, **kwargs)
     evaluator = get_retrieval_evaluator(
         RetrievalEvaluatorTypes.RDNAM, config=config, llm_provider=llm_provider
     )
     documents = load_retrieved_docs_from_csv(
         config.documents_path, queries=config.query_path
```

### Comparing `ragelo-0.1.1/ragelo/evaluators/answer_evaluators/base_answer_evaluator.py` & `ragelo-0.1.2/ragelo/evaluators/retrieval_evaluators/base_retrieval_evaluator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,239 +1,291 @@
-"""Base model for dealing with answer evaluators"""
+"""A Retrieval Evaluator is a class that evaluates the results of a retrieval system.
+It receives a set of queries used to retrieve a document and their respective retrieved documents,
+and returns a score or a label for each document."""
 
-from abc import abstractmethod
+import asyncio
+from concurrent.futures import ThreadPoolExecutor
 from typing import Any, Callable, Optional, Type, get_type_hints
 
-from tenacity import RetryError
-from tqdm import tqdm
+from tqdm.auto import tqdm
 
 from ragelo.evaluators.base_evaluator import BaseEvaluator
 from ragelo.llm_providers.base_llm_provider import BaseLLMProvider, get_llm_provider
 from ragelo.logger import logger
 from ragelo.types import (
-    AgentAnswer,
-    AnswerEvaluatorResult,
-    AnswerEvaluatorTypes,
     AnswerFormat,
     Document,
     Query,
+    RetrievalEvaluatorResult,
+    RetrievalEvaluatorTypes,
 )
-from ragelo.types.configurations import BaseAnswerEvaluatorConfig
-from ragelo.utils import load_retrieved_docs_from_csv
+from ragelo.types.configurations import BaseRetrievalEvaluatorConfig
 
 
-class BaseAnswerEvaluator(BaseEvaluator):
-    config: BaseAnswerEvaluatorConfig
-    output_columns = ["qid", "agent", "raw_answer", "answer"]
-    output_file: str = "answers_evaluations.csv"
+class BaseRetrievalEvaluator(BaseEvaluator):
+    config: BaseRetrievalEvaluatorConfig
+    output_columns = ["qid", "did", "raw_answer", "answer"]
 
     def __init__(
         self,
-        config: BaseAnswerEvaluatorConfig,
+        config: BaseRetrievalEvaluatorConfig,
         llm_provider: BaseLLMProvider,
     ):
         self.config = config
         self.llm_provider = llm_provider
-        if config.output_file is not None:
-            self.output_file = config.output_file
+        self.document_evaluations_path = config.document_evaluations_path
+        if config.output_columns:
+            self.output_columns = config.output_columns
         if config.answer_format == AnswerFormat.MULTI_FIELD_JSON:
-            if isinstance(config.scoring_key, str):
-                scoring_keys = [config.scoring_key]
-            else:
-                scoring_keys = config.scoring_key
-            self.output_columns = ["qid", "agent", "raw_answer"] + scoring_keys
-
-    def batch_evaluate(self, queries: list[Query]) -> list[AnswerEvaluatorResult]:
-        use_progress_bar = self.config.verbose
-        failed_evaluations = 0
-        evaluations = [AnswerEvaluatorResult(**x) for x in self._get_existing_output()]
-        skip_tuples = {(x.qid, x.agent) for x in evaluations}
-        tuples_to_eval = []
-        all_tuples = 0
-        queries = self._add_retrieved_documents_to_queries(
-            queries, self.config.documents_path
-        )
-        for query in queries:
-            for agent_answer in query.answers:
-                qid = query.qid
-                agent = agent_answer.agent
-                all_tuples += 1
-                if (qid, agent) in skip_tuples:
-                    logger.debug(f"Skipping {qid} {agent}")
-                    continue
-                tuples_to_eval.append((query, agent_answer))
+            self.config.scoring_keys = config.scoring_keys
+            self.output_columns = [
+                "qid",
+                "did",
+                "raw_answer",
+            ] + self.config.scoring_keys
+
+        if config.scoring_key and config.scoring_key not in self.output_columns:
+            print(f"Adding scoring key {config.scoring_key} to output columns")
+            self.output_columns.append(self.config.scoring_key)
+        if config.scoring_keys:
+            missing_keys = [
+                key for key in config.scoring_keys if key not in self.output_columns
+            ]
+            self.output_columns.extend(missing_keys)
+
+    async def _async_batch_evaluate(self, queries: list[Query]) -> list[Query]:
+        use_progress_bar = self.config.use_progress_bar
+        queries = self.__prepare_queries(queries)
+        tuples_to_eval = self.__get_tuples_to_evaluate(queries)
         if len(tuples_to_eval) == 0:
-            logger.info("All answers have been evaluated")
-            if self.config.verbose:
-                print(
-                    f"All {all_tuples} answers are already evaluated.\n"
-                    "If you want to re-evaluate them, use the force flag"
-                )
-            return evaluations
-
-        for query, agent_answer in tqdm(
-            tuples_to_eval,
-            desc="Annotating Answers",
-            disable=not use_progress_bar,
+            return queries
+        pbar = tqdm(
+            total=len(tuples_to_eval),
             ncols=100,
+            desc="Evaluating answers",
+            disable=not use_progress_bar,
             leave=False,
             position=0,
-        ):
-            qid = query.qid
-            agent = agent_answer.agent
-            try:
-                raw_answer, answer = self.evaluate(query, agent_answer)
-            except (RetryError, ValueError):
-                failed_evaluations += 1
-                continue
-            evaluations.append(
-                AnswerEvaluatorResult(
-                    qid=qid, agent=agent, raw_answer=raw_answer, answer=answer
-                )
+        )
+        awaitables_ended = False
+        pending: set[asyncio.Future] = set()
+        aws = map(self._async_evaluate, tuples_to_eval)
+        aws = iter(aws)
+        evaluations = []
+        failed = 0
+        while pending or not awaitables_ended:
+            while len(pending) < self.config.n_processes and not awaitables_ended:
+                try:
+                    aw = next(aws)
+                except StopIteration:
+                    awaitables_ended = True  # all tasks have been scheduled
+                else:
+                    pending.add(asyncio.ensure_future(aw))
+            if not pending:
+                break
+
+            done, pending = await asyncio.wait(
+                pending, return_when=asyncio.FIRST_COMPLETED
             )
-            self._dump_response(evaluations[-1], self.output_columns, self.output_file)
+            while done:
+                evaluation = await done.pop()
+                pbar.update()
+                if evaluation.exception:
+                    failed += 1
+                    continue
+                evaluations.append(evaluation)
+        pbar.close()
+        self._add_document_evaluations(queries, evaluations)
         if self.config.verbose:
             print("✅ Done!")
-            print(f"Unparsed answers: {failed_evaluations}")
+            print("Failed evaluations:", failed)
             print(f"Total evaluations: {len(evaluations)}")
-        return evaluations
+        return queries
+
+    async def _async_evaluate(
+        self, eval_sample: tuple[Query, Document]
+    ) -> RetrievalEvaluatorResult:
+        query, document = eval_sample
+        exc = None
+        prompt = self._build_message(query, document)
+        try:
+            raw_answer = await self.llm_provider.call_async(prompt)
+        except Exception as e:
+            logger.warning(f"Failed to FETCH answers for qid: {query.qid}")
+            logger.warning(f"document id: {document.did}")
+            exc = str(e)
+            raw_answer = None
+        try:
+            answer = self._process_answer(raw_answer) if raw_answer else None
+        except ValueError as e:
+            logger.warning(
+                f"Failed to PARSE answer for qid: {query.qid} "
+                "document id: {document.did}\n"
+                f"Raw answer: {raw_answer}"
+            )
+            exc = str(e)
+            answer = None
+        ans = RetrievalEvaluatorResult(
+            qid=query.qid,
+            did=document.did,
+            raw_answer=raw_answer,
+            answer=answer,
+            exception=exc,
+        )
+        self._dump_response(ans, self.output_columns, self.document_evaluations_path)
+        return ans
+
+    def __prepare_queries(self, queries: list[Query]) -> list[Query]:
+        queries = self._load_retrieved_documents(queries)
+        queries = self._load_document_evaluations(queries, force=self.config.force)
+        return queries
+
+    def __get_tuples_to_evaluate(
+        self, queries: list[Query]
+    ) -> list[tuple[Query, Document]]:
+        tuples_to_eval = []
+        all_tuples = 0
+        for q in queries:
+            for d in q.retrieved_docs:
+                if d.evaluation is None:
+                    tuples_to_eval.append((q, d))
+                all_tuples += 1
+        if len(tuples_to_eval) == 0:
+            logger.info("All documents have been evaluated")
+            if self.config.verbose:
+                print(
+                    f"All {all_tuples} documents are already evaluated.\n"
+                    "If you want to re-evaluate documents, use the --force flag."
+                )
+        return tuples_to_eval
 
     def evaluate(
         self,
         query: Query | str,
-        answer: AgentAnswer | str,
-        retrieved_documents: Optional[list[str] | list[Document]] = None,
-        document_metadata: Optional[list[dict[str, Any]]] = None,
+        document: Document | str,
         query_metadata: Optional[dict[str, Any]] = None,
-        answer_metadata: Optional[dict[str, Any]] = None,
+        doc_metadata: Optional[dict[str, Any]] = None,
     ) -> tuple[str, Any]:
+        """Evaluates a single query-document pair. Returns the raw answer and the processed answer."""
         query = self._assemble_query(query, query_metadata)
-        answer = self._assemble_answer(answer, answer_metadata)
-        if isinstance(retrieved_documents, str):
-            retrieved_documents = [retrieved_documents]
-        if retrieved_documents:
-            retrieved_and_assembled_docs = self._assemble_documents(
-                retrieved_documents, document_metadata
-            )
-            query.retrieved_docs = retrieved_and_assembled_docs
-
-        message = self._build_message(query, answer)
+        document = self._assemble_document(document, doc_metadata)
         try:
-            raw_answer = self.llm_provider(message)
-        except RetryError as e:
-            logger.warning(
-                f"Failed to fetch answer for qid: {query.qid} agent: {answer.agent}"
+            # Raises RuntimeError if there is no current event loop.
+            asyncio.get_running_loop()
+            # If there is a current event loop, we need to run the async code
+            # in a separate loop, in a separate thread.
+            with ThreadPoolExecutor(max_workers=1) as executor:
+                future = executor.submit(
+                    asyncio.run, self._async_evaluate((query, document))
+                )
+                result = future.result()
+        except RuntimeError:
+            result = asyncio.run(self._async_evaluate((query, document)))
+        if result.exception or result.raw_answer is None or result.answer is None:
+            raise ValueError(
+                f"Failed to evaluate qid: {query.qid} did: {document.did}",
+                f"Exception: {result.exception}",
             )
-            raise e
+        return result.raw_answer, result.answer
+
+    def batch_evaluate(self, queries: list[Query]) -> list[Query]:
         try:
-            processed_answer = self._process_answer(raw_answer)
+            # Raises RuntimeError if there is no current event loop.
+            asyncio.get_running_loop()
+            # If there is a current event loop, we need to run the async code
+            # in a separate loop, in a separate thread.
+            with ThreadPoolExecutor(max_workers=1) as executor:
+                future = executor.submit(
+                    asyncio.run, self._async_batch_evaluate(queries)
+                )
+                result = future.result()
+        except RuntimeError:
+            result = asyncio.run(self._async_batch_evaluate(queries))
 
-        except ValueError as e:
-            logger.warning(
-                f"Failed to parse answer for qid: {query.qid} agent: {answer.agent}"
-                f"Full answer: {raw_answer}"
-            )
-            raise e
-        return raw_answer, processed_answer
+        return result
 
-    @abstractmethod
     def _build_message(
-        self, query: Query, answer: AgentAnswer
+        self,
+        query: Query,
+        document: Document,
     ) -> str | list[dict[str, str]]:
-        """Builds the message to send to the LLM evaluator"""
+        """Builds the prompt to send to the LLM."""
         raise NotImplementedError
 
     @classmethod
     def from_config(
-        cls, config: BaseAnswerEvaluatorConfig, llm_provider: BaseLLMProvider
+        cls, config: BaseRetrievalEvaluatorConfig, llm_provider: BaseLLMProvider
     ):
         return cls(config, llm_provider)
 
     @classmethod
-    def get_config_class(cls) -> Type[BaseAnswerEvaluatorConfig]:
+    def get_config_class(cls) -> Type[BaseRetrievalEvaluatorConfig]:
         return get_type_hints(cls)["config"]
 
     @staticmethod
     def _construct_list_of_answers(
         answers: list[dict[str, str]]
-    ) -> list[AnswerEvaluatorResult]:
-        return [AnswerEvaluatorResult(**x) for x in answers]
-
-    @staticmethod
-    def _prepare_documents(query: Query) -> str:
-        documents = [(d.did, d.text) for d in query.retrieved_docs]
-        if len(documents) == 0:
-            return "NO DOCUMENTS WERE RETRIEVED"
-        return "\n".join([f"[{did}] {doc.strip()}" for did, doc in documents])
-
-    def _add_retrieved_documents_to_queries(
-        self,
-        queries: list[Query],
-        documents_path: Optional[str],
-        text_column: str = "document_text",
-        overwrite: bool = False,
-    ):
-        if all([len(q.retrieved_docs) > 0 for q in queries]) and not overwrite:
-            logger.info("All queries already have retrieved documents")
-            return queries
-        if documents_path is None:
-            logger.warning(
-                "No path with retrieved documents provided."
-                "Evaluator performance may be affected."
-            )
-            return queries
-        queries_with_docs = load_retrieved_docs_from_csv(
-            documents_path, queries, document_text_col=text_column
-        )
-        return queries_with_docs
+    ) -> list[RetrievalEvaluatorResult]:
+        return [RetrievalEvaluatorResult(**x) for x in answers]
 
 
-class AnswerEvaluatorFactory:
-    registry: dict[AnswerEvaluatorTypes | str, Type[BaseAnswerEvaluator]] = {}
+class RetrievalEvaluatorFactory:
+    registry: dict[RetrievalEvaluatorTypes | str, Type[BaseRetrievalEvaluator]] = {}
 
     @classmethod
-    def register(cls, name: AnswerEvaluatorTypes) -> Callable:
-        def inner_wrapper(wrapped_class: Type[BaseAnswerEvaluator]):
-            if name in cls.registry:
-                logger.warning(f"Overwriting {name} in registry")
-            cls.registry[name.lower()] = wrapped_class
+    def register(cls, evaluator_name: RetrievalEvaluatorTypes) -> Callable:
+        def inner_wrapper(
+            wrapped_class: Type[BaseRetrievalEvaluator],
+        ) -> Type[BaseRetrievalEvaluator]:
+            if evaluator_name in cls.registry:
+                logger.debug(f"Overwriting {evaluator_name} in registry")
+            cls.registry[evaluator_name] = wrapped_class
             return wrapped_class
 
         return inner_wrapper
 
     @classmethod
     def create(
         cls,
-        evaluator_name: str,
+        evaluator_name: RetrievalEvaluatorTypes | str,
         llm_provider: BaseLLMProvider | str,
-        config: Optional[BaseAnswerEvaluatorConfig] = None,
+        config: Optional[BaseRetrievalEvaluatorConfig] = None,
         **kwargs,
-    ) -> BaseAnswerEvaluator:
-        if evaluator_name.lower() not in cls.registry:
-            raise ValueError(f"Unknown evaluator {evaluator_name}")
+    ) -> BaseRetrievalEvaluator:
         if isinstance(llm_provider, str):
             llm_provider_instance = get_llm_provider(llm_provider, **kwargs)
         else:
             llm_provider_instance = llm_provider
+        if evaluator_name not in cls.registry:
+            raise ValueError(
+                f"Unknown retrieval evaluator {evaluator_name}\n"
+                f"Valid options are {list(cls.registry.keys())}"
+            )
         if config is None:
             class_ = cls.registry[evaluator_name]
             type_config = class_.get_config_class()
             valid_keys = [field for field in type_config.get_model_fields()]
             valid_args = {k: v for k, v in kwargs.items() if k in valid_keys}
             config = type_config(**valid_args)
-        return cls.registry[evaluator_name.lower()].from_config(
-            config, llm_provider_instance
-        )
+        return cls.registry[evaluator_name].from_config(config, llm_provider_instance)
 
 
-def get_answer_evaluator(
-    evaluator_name: AnswerEvaluatorTypes | str,
-    llm_provider: BaseLLMProvider | str,
-    config: Optional[BaseAnswerEvaluatorConfig] = None,
+def get_retrieval_evaluator(
+    evaluator_name: Optional[RetrievalEvaluatorTypes | str] = None,
+    llm_provider: BaseLLMProvider | str = "openai",
+    config: Optional[BaseRetrievalEvaluatorConfig] = None,
     **kwargs,
-) -> BaseAnswerEvaluator:
-    return AnswerEvaluatorFactory.create(
+) -> BaseRetrievalEvaluator:
+    if evaluator_name is None:
+        # get the name from the config
+        if config is None:
+            raise ValueError(
+                "Either the evaluator_name or a config object must be provided"
+            )
+        evaluator_name = config.evaluator_name
+
+    return RetrievalEvaluatorFactory.create(
         evaluator_name,
         llm_provider=llm_provider,
         config=config,
         **kwargs,
     )
```

### Comparing `ragelo-0.1.1/ragelo/evaluators/answer_evaluators/custom_prompt_evaluator.py` & `ragelo-0.1.2/ragelo/evaluators/answer_evaluators/custom_prompt_evaluator.py`

 * *Files identical despite different names*

### Comparing `ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/custom_prompt_evaluator.py` & `ragelo-0.1.2/ragelo/evaluators/retrieval_evaluators/custom_prompt_evaluator.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from ragelo.types import Document, Query, RetrievalEvaluatorTypes
 from ragelo.types.configurations import CustomPromptEvaluatorConfig
 
 
 @RetrievalEvaluatorFactory.register(RetrievalEvaluatorTypes.CUSTOM_PROMPT)
 class CustomPromptEvaluator(BaseRetrievalEvaluator):
     config: CustomPromptEvaluatorConfig
-    output_file: str = "custom_prompt_evaluations.csv"
 
     def __init__(
         self,
         config: CustomPromptEvaluatorConfig,
         llm_provider: BaseLLMProvider,
     ):
         super().__init__(config, llm_provider)
```

### Comparing `ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/domain_expert_evaluator.py` & `ragelo-0.1.2/ragelo/evaluators/retrieval_evaluators/domain_expert_evaluator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """Evaluator with a domain expert persona"""
 
-import logging
-from typing import Any, Optional
-
-from tenacity import RetryError
-
 from ragelo.evaluators.retrieval_evaluators import (
     BaseRetrievalEvaluator,
     RetrievalEvaluatorFactory,
 )
 from ragelo.llm_providers.base_llm_provider import BaseLLMProvider
-from ragelo.types import Document, Query, RetrievalEvaluatorTypes
+from ragelo.logger import logger
+from ragelo.types import (
+    Document,
+    Query,
+    RetrievalEvaluatorResult,
+    RetrievalEvaluatorTypes,
+)
 from ragelo.types.configurations import DomainExpertEvaluatorConfig
 
 
 @RetrievalEvaluatorFactory.register(RetrievalEvaluatorTypes.DOMAIN_EXPERT)
 class DomainExpertEvaluator(BaseRetrievalEvaluator):
     sys_prompt = """
-You are a domain expert in {domain_long}.{company_prompt_1} You are tasked \
+You are a domain expert in {expert_in}.{company_prompt_1} You are tasked \
 with evaluating the performance of a retrieval system for question \
 answering in this domain. The question answering system will be used \
 by internal users{company_prompt_2}{domain_short}. They are interested \
 in a retrieval system that provides relevant passages based on their questions.
 """.strip()
 
     reason_prompt = """
@@ -88,27 +89,27 @@
 
     def __init__(
         self,
         config: DomainExpertEvaluatorConfig,
         llm_provider: BaseLLMProvider,
     ):
         super().__init__(config, llm_provider)
-        if not self.config.domain_long:
+        if not self.config.expert_in:
             raise ValueError(
-                "You are tying to use the Domain Expert Retrieval Evaluator. "
-                "For this evaluator, you need to provide at least the name of the domain "
-                "in the domain_long field."
+                "You are trying to use the Domain Expert Retrieval Evaluator. "
+                "For this evaluator, you need to provide the domain the evaluator "
+                "is an expert in the expert_in field."
             )
 
-        self.domain_long = self.config.domain_long
+        self.expert_in = self.config.expert_in
         self.domain_short = (
             f" {self.config.domain_short}" if self.config.domain_short else ""
         )
         self.sys_prompt = self.sys_prompt.format(
-            domain_long=self.domain_long,
+            expert_in=self.expert_in,
             company_prompt_1=(
                 self.COMPANY_PROMPT_1.format(company=self.config.company)
                 if self.config.company
                 else ""
             ),
             company_prompt_2=(
                 self.COMPANY_PROMPT_2.format(company=self.config.company)
@@ -120,64 +121,67 @@
                 if self.config.domain_short
                 else ""
             ),
         )
         self.extra_guidelines = (
             self.config.extra_guidelines if self.config.extra_guidelines else []
         )
+        # self.reasoner_eva
 
     def __build_reason_message(self, query: Query, document: Document) -> str:
         guidelines = "\n".join(
             [f"- {guideline}" for guideline in self.extra_guidelines]
         )
         reason_prompt = self.reason_prompt.format(
             query=query.query,
             doc_content=document.text,
             domain_short=self.domain_short if self.domain_short else "",
             extra_guidelines=guidelines,
         )
         return reason_prompt
 
-    def evaluate(
-        self,
-        query: Query | str,
-        document: Document | str,
-        query_metadata: Optional[dict[str, Any]] = None,
-        doc_metadata: Optional[dict[str, Any]] = None,
-    ) -> tuple[str, Any]:
-        """Processes a single pair of qid, did in a two-shot manner"""
-        if isinstance(query, str):
-            query = Query(qid="<no_qid>", query=query)
-        if isinstance(document, str):
-            document = Document(did="<no_did>", text=document)
-        query.add_metadata(query_metadata)
-        document.add_metadata(doc_metadata)
-
-        qid = query.qid
-        did = document.did
+    async def _async_evaluate(
+        self, eval_sample: tuple[Query, Document]
+    ) -> RetrievalEvaluatorResult:
+        query, document = eval_sample
         reason_message = self.__build_reason_message(query, document)
         messages_reasoning = [
             {"role": "system", "content": self.sys_prompt},
             {"role": "user", "content": reason_message},
         ]
+        exc = None
         try:
-            reasoning_answer = self.llm_provider(messages_reasoning)
-
-        except RetryError as e:
-            logging.warning(f"Failed to fetch reasoning for document {qid} {did}")
-            raise e
-        except ValueError as e:
-            logging.warning(f"Failed to parse reasoning for document {qid} {did}")
-            raise e
-
+            reasoning_answer = await self.llm_provider.call_async(messages_reasoning)
+        except Exception as e:
+            logger.warning(f"Failed to FETCH reasonings for qid: {query.qid}")
+            logger.warning(f"document id: {document.did}")
+            exc = str(e)
+            return RetrievalEvaluatorResult(
+                qid=query.qid,
+                did=document.did,
+                raw_answer=None,
+                answer=None,
+                exception=exc,
+            )
         messages_score = messages_reasoning.copy()
         messages_score.append({"role": "assistant", "content": reasoning_answer})
         messages_score.append({"role": "user", "content": self.score_prompt})
         try:
-            score_answer = self._process_answer(self.llm_provider(messages_score))
-        except RetryError as e:
-            logging.warning(f"Failed to fetch evaluation for document {qid} {did}")
-            raise e
+            score_answer = await self.llm_provider.call_async(messages_score)
+            score_answer = self._process_answer(score_answer)
         except ValueError as e:
-            logging.warning(f"Failed to parse evaluation for document {qid} {did}")
-            raise e
-        return reasoning_answer, score_answer
+            logger.warning(f"Failed to parse scores for qid: {query.qid}")
+            logger.warning(f"document id: {document.did}")
+            score_answer = None
+            exc = str(e)
+        except Exception as e:
+            logger.warning(f"Failed to FETCH scores for qid: {query.qid}")
+            logger.warning(f"document id: {document.did}")
+            score_answer = None
+            exc = str(e)
+        return RetrievalEvaluatorResult(
+            qid=query.qid,
+            did=document.did,
+            raw_answer=reasoning_answer,
+            answer=score_answer,
+            exception=exc,
+        )
```

### Comparing `ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/few_shot_evaluator.py` & `ragelo-0.1.2/ragelo/evaluators/retrieval_evaluators/few_shot_evaluator.py`

 * *Files identical despite different names*

### Comparing `ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/rdnam_evaluator.py` & `ragelo-0.1.2/ragelo/evaluators/retrieval_evaluators/rdnam_evaluator.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,17 +57,14 @@
 Measure how trustworthy the web page is (T).""".strip()
     ASPECTS_EXAMPLE = """[{{"M": 2, "T": 1, "O": 1}}, {{"M": 1..."""
     DEFAULT_EXAMPLE = """[{{"O": 1}}, {{"O": 2}}, {{"O": 0..."""
     MULTIPLE_PROMPT = """We asked five search engine raters to evaluate \
 the relevance of the web page for the query.
 Each rater used their own independent judgement."""
     config: RDNAMEvaluatorConfig
-    output_columns = ["qid", "did", "raw_answer", "answer"]
-    scoring_key = "answer"
-    output_file = "rdnam_evaluations.csv"
 
     def __init__(
         self,
         config: RDNAMEvaluatorConfig,
         llm_provider: BaseLLMProvider,
     ):
         """Initializes an evaluator based on RDNAM framework."""
```

### Comparing `ragelo-0.1.1/ragelo/evaluators/retrieval_evaluators/reasoner_evaluator.py` & `ragelo-0.1.2/ragelo/evaluators/retrieval_evaluators/reasoner_evaluator.py`

 * *Files identical despite different names*

### Comparing `ragelo-0.1.1/ragelo/llm_providers/base_llm_provider.py` & `ragelo-0.1.2/ragelo/llm_providers/base_llm_provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,14 +29,22 @@
         self.config = config
 
     @abstractmethod
     def __call__(self, prompt: str | list[dict[str, str]]) -> str:
         """Submits a single query-document pair to the LLM and returns the answer."""
         raise NotImplementedError
 
+    @abstractmethod
+    async def call_async(
+        self,
+        prompt: str | list[dict[str, str]],
+    ) -> str:
+        """Submits a single query-document pair to the LLM and returns the answer."""
+        raise NotImplementedError
+
     @classmethod
     def from_config(
         cls,
         config: LLMProviderConfig,
     ) -> "BaseLLMProvider":
         """Inits the LLM provider from a credentials file."""
         return cls(config)
@@ -73,15 +81,14 @@
         if name not in cls.registry:
             raise ValueError(f"LLM provider {name} not found")
         if credentials_file and os.path.isfile(credentials_file):
             set_credentials_from_file(credentials_file)
         if config is None:
             class_ = cls.registry[name]
             type_config = class_.get_config_class()
-            print(type_config.__fields__)
             valid_keys = [field for field in type_config.get_model_fields()]
             if "api_key" not in kwargs:
                 api_key = os.environ.get(class_.api_key_env_var)
                 if not api_key:
                     raise ValueError(
                         f"API key not found in environment variable {class_.api_key_env_var}"
                     )
```

### Comparing `ragelo-0.1.1/ragelo/llm_providers/openai_client.py` & `ragelo-0.1.2/ragelo/llm_providers/openai_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-from openai import AzureOpenAI, OpenAI
+import asyncio
+
+from openai import AsyncAzureOpenAI, AsyncOpenAI
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 
 from ragelo.llm_providers.base_llm_provider import BaseLLMProvider, LLMProviderFactory
 from ragelo.types import LLMProviderTypes
 from ragelo.types.configurations import OpenAIConfiguration
 
 
-# TODO: Change client to use json_mode
+# TODO: Change client to use tools instead of processing the raw files
 @LLMProviderFactory.register(LLMProviderTypes.OPENAI)
 class OpenAIProvider(BaseLLMProvider):
     """A Wrapper over the OpenAI client."""
 
     config: OpenAIConfiguration
     api_key_env_var: str = "OPENAI_API_KEY"
 
@@ -21,51 +23,78 @@
         super().__init__(config)
         self.__openai_client = self.__get_openai_client(config)
 
     @retry(wait=wait_random_exponential(min=1, max=120), stop=stop_after_attempt(1))
     def __call__(
         self,
         prompt: str | list[dict[str, str]],
-        temperature: float = 0.1,
-        max_tokens: int = 512,
     ) -> str:
         """Calls the OpenAI API.
 
         Args:
             prompt: The prompt to use. Either a list of messages or a string.
             temperature : The temperature to use. Defaults to 0.1.
             max_tokens: The maximum number of tokens to retrieve. Defaults 512.
         """
         if isinstance(prompt, str):
             prompt = [{"role": "system", "content": prompt}]
-        answers = self.__openai_client.chat.completions.create(
+        answers = asyncio.run(
+            self.__openai_client.chat.completions.create(
+                model=self.config.model,
+                messages=prompt,  # type: ignore
+                temperature=self.config.temperature,
+                max_tokens=self.config.max_tokens,
+            )
+        )
+        if (
+            not answers.choices
+            or not answers.choices[0].message
+            or not answers.choices[0].message.content
+        ):
+            raise ValueError("OpenAI did not return any completions.")
+        return answers.choices[0].message.content
+
+    async def call_async(
+        self,
+        prompt: str | list[dict[str, str]],
+    ) -> str:
+        """Calls the OpenAI API asynchronously.
+
+        Args:
+            prompt: The prompt to use. Either a list of messages or a string.
+            temperature : The temperature to use. Defaults to 0.1.
+            max_tokens: The maximum number of tokens to retrieve. Defaults 512.
+        """
+        if isinstance(prompt, str):
+            prompt = [{"role": "system", "content": prompt}]
+        answers = await self.__openai_client.chat.completions.create(
             model=self.config.model,
             messages=prompt,  # type: ignore
-            temperature=temperature,
-            max_tokens=max_tokens,
+            temperature=self.config.temperature,
+            max_tokens=self.config.max_tokens,
         )
         if (
             not answers.choices
             or not answers.choices[0].message
             or not answers.choices[0].message.content
         ):
             raise ValueError("OpenAI did not return any completions.")
         return answers.choices[0].message.content
 
     @staticmethod
-    def __get_openai_client(openai_config: OpenAIConfiguration) -> OpenAI:
+    def __get_openai_client(openai_config: OpenAIConfiguration) -> AsyncOpenAI:
         if openai_config.api_type == "azure":
             if openai_config.api_base is None:
                 raise ValueError("OpenAI base url not found in configuration")
-            return AzureOpenAI(
+            return AsyncAzureOpenAI(
                 azure_endpoint=openai_config.api_base,
                 api_key=openai_config.api_key,
                 api_version=openai_config.api_version,
             )
         elif openai_config.api_type == "open_ai" or openai_config.api_type is None:
-            return OpenAI(
+            return AsyncOpenAI(
                 base_url=openai_config.api_base,
                 api_key=openai_config.api_key,
                 organization=openai_config.org,
             )
         else:
             raise Exception(f"Unknown OpenAI api type: {openai_config.api_type}")
```

### Comparing `ragelo-0.1.1/ragelo/logger.py` & `ragelo-0.1.2/ragelo/logger.py`

 * *Files identical despite different names*

### Comparing `ragelo-0.1.1/ragelo/types/configurations/base_configs.py` & `ragelo-0.1.2/ragelo/types/configurations/base_configs.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,37 +20,48 @@
         default=False,
         description="Whether or not to be verbose and print all intermediate steps",
     )
     credentials_file: Optional[str] = Field(
         default=None,
         description="Path to a txt file with the credentials for the different LLM providers",
     )
-    model: str = Field(
-        default="gpt-4-turbo",
-        description="Name of the model to use for the LLM provider",
-    )
     data_path: str = Field(default="data/", description="Path to the data folder")
 
     llm_provider: str = Field(
         default="openai", description="The name of the LLM provider"
     )
     write_output: bool = Field(
         default=True, description="Whether or not to write the output to a file"
     )
+    use_progress_bar: bool = Field(
+        default=True, description="Whether or not to show a progress bar"
+    )
 
 
 class BaseEvaluatorConfig(BaseConfig):
     query_path: str = Field(
         default="queries.csv", description="Path to the queries file"
     )
     documents_path: str = Field(
         default="documents.csv", description="Path to the documents file"
     )
-    output_file: Optional[str] = Field(
-        default=None, description="Path to the output file"
+    answers_path: str = Field(
+        default="answers.csv", description="Path with agents answers"
+    )
+    document_evaluations_path: str = Field(
+        default="reasonings.csv",
+        description="Path to write (or read) the evaluations of the retrieved documents",
+    )
+    answers_evaluations_path: str = Field(
+        default="answers_evaluations.csv",
+        description="Path to write (or read) the evaluations of each agent's answers",
+    )
+    games_evaluations_path: str = Field(
+        default="pairwise_answer_evaluations.csv",
+        description="Path to write (or read) the evaluations of the pairwise games between agents answers",
     )
     query_placeholder: str = Field(
         default="query",
         description="The placeholder for the query in the prompt",
     )
     scoring_key: str = Field(
         default="relevance",
@@ -60,24 +71,29 @@
         default=["relevance"],
         description="When using answer_format=multi_field_json, the keys to extract from the answer",
     )
     answer_format: str = Field(
         default=AnswerFormat.JSON,
         description="The format of the answer returned by the LLM",
     )
+    n_processes: int = Field(
+        default=1,
+        description="The number of parallel LLM calls to use for the evaluation",
+    )
+    output_columns: Optional[list[str]] = Field(
+        default=["qid", "did", "raw_answer", "answer"],
+        description="The columns to output in the CSV file",
+    )
 
 
 class AllConfig(BaseEvaluatorConfig):
     reasoning_path: str = Field(
         default="reasonings.csv",
         description="CSV file with the reasoning for each retrieved document",
     )
-    answers_path: str = Field(
-        default="answers.csv", description="Path to the answers file"
-    )
     evaluations_file: str = Field(
         default="answers_evaluations.csv",
         description="Path to write the pairwise evaluations of answers",
     )
     output_file: str = Field(
         default="agents_ranking.csv", description="Path to the output file"
     )
```

### Comparing `ragelo-0.1.1/ragelo/types/configurations/retrieval_evaluator_configs.py` & `ragelo-0.1.2/ragelo/types/configurations/answer_evaluator_configs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,129 @@
-from typing import List, Optional
+from typing import Callable, Optional
 
 from pydantic import Field
 
 from ragelo.types.configurations.base_configs import AnswerFormat, BaseEvaluatorConfig
-from ragelo.types.types import FewShotExample
+from ragelo.types.types import AnswerEvaluatorTypes
 
 
-class BaseRetrievalEvaluatorConfig(BaseEvaluatorConfig):
-    document_placeholder: str = Field(
-        default="document",
-        description="The placeholder for the document in the prompt",
+class BaseAnswerEvaluatorConfig(BaseEvaluatorConfig):
+    evaluator_name: str = ""
+    answer_placeholder: str = Field(
+        default="answer", description="The placeholder for the answer in the prompt"
     )
-
-
-class ReasonerEvaluatorConfig(BaseRetrievalEvaluatorConfig):
-    answer_format: str = Field(
-        default=AnswerFormat.TEXT,
-        description="The format of the answer returned by the LLM",
+    documents_placeholder: str = Field(
+        default="documents",
+        description="The placeholder for the documents in the prompt",
     )
-
-
-class DomainExpertEvaluatorConfig(BaseRetrievalEvaluatorConfig):
-    domain_long: str = Field(
-        default="",
-        description="The name of corpus domain. (e.g., Chemical Engineering)",
+    pairwise: bool = Field(
+        default=False, description="Whether or not to the evaluator is pairwise"
     )
-    domain_short: Optional[str] = Field(
-        default=None,
-        description="A short or alternative name of the domain. "
-        "(e.g., Chemistry, CS, etc.)",
+    output_columns: list[str] = Field(
+        default=["qid", "agent", "raw_answer", "answer"],
+        description="The columns to output in the CSV file",
     )
-    company: Optional[str] = Field(
-        default=None,
-        description="Name of the company or organization that the user that "
-        "submitted the query works for. that the domain belongs to. "
-        "(e.g.: ChemCorp, CS Inc.)",
+    document_template: str = Field(
+        default="[{did}] {doc}",
+        description="The template to format each individual document in the prompt",
+    )
+    has_citations: bool = Field(
+        default=True,
+        description=(
+            "Whether or not the answers contain document citations in square brackets. "
+            "If used, the document_ids in the documents and in the answers should match."
+        ),
+    )
+    include_annotations: bool = Field(
+        default=True,
+        description="Whether or not to include the document relevance annotations in the prompt",
+    )
+    include_raw_documents: bool = Field(
+        default=False,
+        description="Whether or not to include the raw documents in the prompt",
+    )
+    document_filter: Optional[Callable[[str], bool]] = Field(
+        default=None, description="A function to filter the documents"
     )
-    extra_guidelines: Optional[List[str]] = Field(
+    document_relevance_threshold: Optional[int] = Field(
         default=None,
-        description="A list of extra guidelines to be used when reasoning about the "
-        "relevancy of the document.",
+        description="The minimum relevance score for a document to be included in the prompt. By default, all documents are included.",
+    )
+
+
+class PairwiseEvaluatorConfig(BaseAnswerEvaluatorConfig):
+    """Configuration for the pairwise evaluator."""
+
+    evaluator_name: str = AnswerEvaluatorTypes.PAIRWISE
+    output_columns: list[str] = Field(
+        default=["qid", "agent_a", "agent_b", "raw_answer", "answer"],
+        description="The columns to output in the CSV file",
+    )
+    bidirectional: bool = Field(
+        default=False, description="Whether or not to run each game in both directions"
     )
-    output_file: str = Field(
-        default="domain_expert_evaluations.csv",
+    n_games_per_query: int = Field(
+        default=100, description="Number of games to generate for each query"
+    )
+    games_evaluations_path: str = Field(
+        default="pairwise_answers_evaluations.csv",
         description="Path to the output file",
     )
-    answer_format: str = Field(
-        default="text",
-        description="The format of the answer returned by the LLM",
+    documents_path: str = Field(
+        default="reasonings.csv",
+        description="Path with the outputs from the reasoner Retrieval Evaluator",
+    )
+    pairwise: bool = Field(
+        default=True, description="Whether or not to the evaluator is pairwise"
+    )
+    document_template: str = Field(
+        default="[{did}] {annotation}",
+        description="The template to format each individual document in the prompt",
     )
-    scoring_key: str = Field(
-        default="score",
-        description="The field to use when parsing the llm answer",
+    prompt: Optional[str] = Field(
+        default=None,
+        description="Prompt to use for the evaluator. If not provided, a default prompt will be used",
+    )
+    factors: str = Field(
+        default=(
+            "the correctness, helpfulness, completeness, accuracy, depth, and "
+            "level of detail of their responses"
+        ),
+        description=(
+            "A string containing the factors to be used when evaluating an answer. "
+            "If not provided, a default string will be used"
+        ),
     )
 
 
-class CustomPromptEvaluatorConfig(BaseRetrievalEvaluatorConfig):
+class CustomPromptAnswerEvaluatorConfig(BaseAnswerEvaluatorConfig):
+    evaluator_name: str = AnswerEvaluatorTypes.CUSTOM_PROMPT
     prompt: str = Field(
-        default="query: {query} document: {document}",
+        default="retrieved documents: {documents} query: {query} answer: {answer}",
         description="The prompt to be used to evaluate the documents. It should contain a {query} and a {document} placeholder",
     )
+    answers_evaluations_path: str = Field(
+        default="custom_prompt_answers_evaluations.csv",
+        description="Path to the output file",
+    )
     scoring_keys: list[str] = Field(
         default=["quality", "trustworthiness", "originality"],
-        description="The fields to use when parsing the llm answer",
+        description="The fields to extract from the answer",
     )
     answer_format: str = Field(
         default=AnswerFormat.MULTI_FIELD_JSON,
         description="The format of the answer returned by the LLM",
     )
 
 
-class FewShotEvaluatorConfig(BaseRetrievalEvaluatorConfig):
-    system_prompt: str = Field(
-        default="You are a helpful assistant.",
-        description="The system prompt to be used to evaluate the documents.",
-    )
-    few_shots: List[FewShotExample] = Field(
-        default=[], description="A list of few-shot examples to be used in the prompt"
-    )
-    few_shot_user_prompt: str = Field(
-        default="Query: {query}\n\nPassage:{passage}",
-        description="The individual prompt to be used to evaluate the documents. It should contain a {query} and a {passage} placeholder",
-    )
-    few_shot_assistant_answer: str = Field(
-        default='{reasoning}\n\n{{"relevance": {relevance}}}',
-        description="The expected answer format from the LLM for each evaluated document "
-        "It should contain a {reasoning} and a {relevance} placeholder",
-    )
-    output_file: str = Field(
-        default="few_shot_evaluations.csv",
-        description="Path to the output file",
-    )
-    reasoning_placeholder: str = Field(
-        default="reasoning",
-        description="The placeholder for the reasoning in the prompt",
-    )
-    relevance_placeholder: str = Field(
-        default="relevance",
-        description="The placeholder for the relevance in the prompt",
+class PairwiseDomainExpertEvaluatorConfig(PairwiseEvaluatorConfig):
+    evaluator_name: str = AnswerEvaluatorTypes.DOMAIN_EXPERT
+    expert_in: str = Field(
+        default="",
+        description="What the LLM should mimic being an expert in.",
     )
-
-
-class RDNAMEvaluatorConfig(BaseRetrievalEvaluatorConfig):
-    annotator_role: Optional[str] = Field(
+    company: Optional[str] = Field(
         default=None,
-        description="A String defining the type of user the LLM should mimic. "
-        "(e.g.: 'You are a search quality rater evaluating the relevance "
-        "of web pages')",
-    )
-    use_aspects: bool = Field(
-        default=False,
-        description="Should the prompt include aspects to get to the final score? "
-        "If true, will prompt the LLM to compute scores for M (intent match) "
-        "and T (trustworthy) for the document before computing the final score.",
-    )
-    use_multiple_annotators: bool = Field(
-        default=False,
-        description="Should the prompt ask the LLM to mimic multiple annotators?",
-    )
-    output_file: str = Field(
-        default="rdnam_evaluations.csv", description="Path to the output file"
+        description="Name of the company or organization that the user that "
+        "submitted the query works for. that the domain belongs to. "
+        "(e.g.: ChemCorp, CS Inc.)",
     )
```

### Comparing `ragelo-0.1.1/ragelo.egg-info/PKG-INFO` & `ragelo-0.1.2/ragelo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragelo
-Version: 0.1.1
+Version: 0.1.2
 Summary: RAGElo: A Tool for Evaluating Retrieval-Augmented Generation Models
 Author-email: Zeta Alpha <support@zeta-alpha.com>, Arthur Câmara <camara@zeta-alpha.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/zetaalphavector/RAGElo
 Project-URL: Repository, https://github.com/zetaalphavector/RAGElo
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -32,14 +32,15 @@
 Requires-Dist: flake8==6.1.0; extra == "dev"
 Requires-Dist: flake8-black==0.3.6; extra == "dev"
 Requires-Dist: flake8-isort==6.1.0; extra == "dev"
 Requires-Dist: mypy==1.9.0; extra == "dev"
 Requires-Dist: Flake8-pyproject==1.2.3; extra == "dev"
 Requires-Dist: types-tqdm==4.66.0; extra == "dev"
 Requires-Dist: pydantic==2.7.0; extra == "dev"
+Requires-Dist: pytest-asyncio==0.23.6; extra == "dev"
 
 
 <h1 align="center">
 <img style="vertical-align:middle" src="https://raw.githubusercontent.com/zetaalphavector/RAGElo/master/docs/images/RAGElo_logo.png" height="200">
 </h1>
 
 <p  align="center" >
@@ -72,17 +73,17 @@
 
 ```python
 from ragelo import get_retrieval_evaluator
 
 evaluator = get_retrieval_evaluator("RDNAM", llm_provider="openai")
 raw_answer, processed_answer = evaluator.evaluate(query="What is the capital of France?", document='Lyon is the second largest city in France.')
 print(processed_answer)
-# Output: 0
+# Output: 1
 print(raw_answer)
-# Output: '"O": 0\n}'
+# Output: '"O": 1\n}'
 ```
 
 For a more complete example, we can evaluate with a custom prompt, and inject metadata into our evaluation prompt:
 
 ```python
 from ragelo import get_retrieval_evaluator
```

### Comparing `ragelo-0.1.1/ragelo.egg-info/SOURCES.txt` & `ragelo-0.1.2/ragelo.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 ragelo/cli/retrieval_evaluator_cmd.py
 ragelo/cli/utils.py
 ragelo/evaluators/__init__.py
 ragelo/evaluators/base_evaluator.py
 ragelo/evaluators/answer_evaluators/__init__.py
 ragelo/evaluators/answer_evaluators/base_answer_evaluator.py
 ragelo/evaluators/answer_evaluators/custom_prompt_evaluator.py
-ragelo/evaluators/answer_evaluators/pairwise_reasoning_evaluator.py
+ragelo/evaluators/answer_evaluators/domain_expert_evaluator.py
+ragelo/evaluators/answer_evaluators/pairwise_evaluator.py
 ragelo/evaluators/retrieval_evaluators/__init__.py
 ragelo/evaluators/retrieval_evaluators/base_retrieval_evaluator.py
 ragelo/evaluators/retrieval_evaluators/custom_prompt_evaluator.py
 ragelo/evaluators/retrieval_evaluators/domain_expert_evaluator.py
 ragelo/evaluators/retrieval_evaluators/few_shot_evaluator.py
 ragelo/evaluators/retrieval_evaluators/rdnam_evaluator.py
 ragelo/evaluators/retrieval_evaluators/reasoner_evaluator.py
```

### Comparing `ragelo-0.1.1/tests/conftest.py` & `ragelo-0.1.2/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
-from unittest.mock import Mock
+from unittest.mock import AsyncMock, Mock
 
 import pytest
-from openai import OpenAI
-from openai.resources.chat import Chat
-from openai.resources.chat.completions import Completions
+from openai import AsyncOpenAI
+from openai.resources.chat import AsyncChat
+from openai.types.chat.chat_completion import ChatCompletion, Choice
+from openai.types.chat.chat_completion_message import ChatCompletionMessage
 
 from ragelo.llm_providers.base_llm_provider import BaseLLMProvider
 from ragelo.llm_providers.openai_client import OpenAIConfiguration
 from ragelo.types.configurations import (
     BaseEvaluatorConfig,
     CustomPromptAnswerEvaluatorConfig,
     CustomPromptEvaluatorConfig,
@@ -26,21 +27,27 @@
 )
 
 
 class MockLLMProvider(BaseLLMProvider):
     def __init__(self, config):
         self.config = config
         self.call_mocker = Mock(
-            side_effect=lambda prompt: f"Received prompt: {prompt}. "
+            side_effect=lambda prompt: f"Received prompt: {prompt}."
+        )
+        self.async_call_mocker = AsyncMock(
+            side_effect=lambda prompt: f"Async prompt: {prompt}."
         )
 
     @classmethod
     def from_configuration(cls, config: LLMProviderConfig):
         return cls(config)
 
+    async def call_async(self, prompt):
+        return await self.async_call_mocker(prompt)
+
     def __call__(self, prompt) -> str:
         return self.call_mocker(prompt)
 
 
 @pytest.fixture
 def queries_test():
     return load_queries_from_csv("tests/data/queries.csv")
@@ -80,47 +87,63 @@
 def llm_provider_config():
     return LLMProviderConfig(
         api_key="fake key",
     )
 
 
 @pytest.fixture
-def chat_completion_mock(mocker):
-    return mocker.Mock(Completions)
+def chat_completion_mock():
+    fake_response = ChatCompletion(
+        id="fake id",
+        choices=[
+            Choice(
+                finish_reason="stop",
+                index=0,
+                logprobs=None,
+                message=ChatCompletionMessage(
+                    content="fake response", role="assistant"
+                ),
+            )
+        ],
+        created=0,
+        model="fake model",
+        object="chat.completion",
+    )
+    async_mock = AsyncMock()
+    async_mock.create.return_value = fake_response
+    return async_mock
 
 
 @pytest.fixture
 def openai_client_mock(mocker, chat_completion_mock):
-    openai_client = mocker.Mock(OpenAI)
-    type(openai_client).chat = mocker.Mock(Chat)
+    openai_client = mocker.AsyncMock(AsyncOpenAI)
+    type(openai_client).chat = mocker.AsyncMock(AsyncChat)
     type(openai_client.chat).completions = mocker.PropertyMock(
         return_value=chat_completion_mock
     )
     return openai_client
 
 
 @pytest.fixture
 def base_eval_config():
     return BaseEvaluatorConfig(
         documents_path="tests/data/documents.csv",
         query_path="tests/data/queries.csv",
-        output_file="tests/data/output.csv",
         force=True,
         verbose=True,
         write_output=False,
     )
 
 
 @pytest.fixture
 def pairwise_answer_eval_config(base_eval_config):
     base_config = base_eval_config.model_dump()
-    del base_config["documents_path"]
+    base_config["document_evaluations_path"] = "tests/data/reasonings.csv"
     config = PairwiseEvaluatorConfig(
-        documents_path="tests/data/reasonings.csv",
-        bidirectional=False,
+        bidirectional=True,
         **base_config,
     )
     return config
 
 
 @pytest.fixture
 def custom_answer_eval_config(base_eval_config):
@@ -133,15 +156,14 @@
 by RAG Agents. Given the following retrieved documents and a user query, evaluate \
 the quality of the answers based on their quality, trustworthiness and originality. \
 The last line of your answer must be a json object with the keys "quality", \
 "trustworthiness" and originality, each of them with a single number between 0 and \
 2, where 2 is the highest score on that aspect.
 DOCUMENTS RETRIEVED:
 {documents}
-
 User Query: {query}
 
 Agent answer: {answer}
 """.strip(),
         **base_config,
     )
     return config
@@ -149,15 +171,15 @@
 
 @pytest.fixture
 def expert_retrieval_eval_config(base_eval_config):
     base_eval_config = base_eval_config.model_dump()
     del base_eval_config["scoring_key"]
     del base_eval_config["answer_format"]
     return DomainExpertEvaluatorConfig(
-        domain_long="Computer Science",
+        expert_in="Computer Science",
         domain_short="computer scientists",
         company="Zeta Alpha",
         extra_guidelines=["Super precise answers only!"],
         **base_eval_config,
     )
 
 
@@ -218,54 +240,58 @@
 
 @pytest.fixture
 def llm_provider_json_mock(llm_provider_config):
     provider = MockLLMProvider(llm_provider_config)
     provider.call_mocker = Mock(
         side_effect=lambda _: 'LLM JSON response\n{"relevance": 0}'
     )
+    provider.async_call_mocker = AsyncMock(
+        side_effect=lambda _: 'Async LLM JSON response\n{"relevance": 1}'
+    )
     return provider
 
 
 @pytest.fixture
 def llm_provider_pairwise_answer_mock(llm_provider_config):
     provider = MockLLMProvider(llm_provider_config)
     provider.call_mocker = Mock(
         side_effect=[
             "Agent [[A]] is better",
             "Agent [[B]] is better",
             "A tie. Therefore, [[C]]",
             "I don't know. [[C]]",
         ]
     )
+    provider.async_call_mocker = AsyncMock(
+        side_effect=[
+            "Async Agent [[A]] is better",
+            "Async Agent [[B]] is better",
+            "Async A tie. Therefore, [[C]]",
+            "Async I don't know. [[C]]",
+        ]
+    )
     return provider
 
 
 @pytest.fixture
 def llm_provider_answer_mock(llm_provider_config):
     provider = MockLLMProvider(llm_provider_config)
     provider.call_mocker = Mock(
         side_effect=lambda prompt: f"Answer for {prompt}\n"
         '{"quality": 2, "trustworthiness": 1, "originality": 1}',
     )
-    return provider
-
-
-@pytest.fixture
-def llm_provider_mock_mock(mocker):
-    return mocker.Mock(MockLLMProvider)
-
-
-@pytest.fixture
-def llm_provider_domain_expert_mock(llm_provider_config):
-    provider = MockLLMProvider(llm_provider_config)
-    provider.call_mocker = Mock(
-        side_effect=["Reasoning answer", "2", "Reasoning_answer 2", "0"]
+    provider.async_call_mocker = AsyncMock(
+        side_effect=lambda prompt: f"Async answer for {prompt}\n"
+        '{"quality": 1, "trustworthiness": 0, "originality": 0}',
     )
     return provider
 
 
 @pytest.fixture
 def llm_provider_mock_rdnam(llm_provider_config):
     mocked_scores = [{"M": 2, "T": 1, "O": 1}, {"M": 1, "T": 1, "O": 2}]
     provider = MockLLMProvider(llm_provider_config)
     provider.call_mocker = Mock(side_effect=lambda _: json.dumps(mocked_scores)[2:])
+    provider.async_call_mocker = AsyncMock(
+        side_effect=lambda _: json.dumps(mocked_scores)[2:]
+    )
     return provider
```

### Comparing `ragelo-0.1.1/tests/unit/test_answer_evaluators.py` & `ragelo-0.1.2/tests/unit/test_answer_evaluators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,44 @@
-from typing import cast
+import pytest
 
 from ragelo import get_answer_evaluator
 from ragelo.evaluators.answer_evaluators import (
     CustomPromptEvaluator,
-    PairwiseWithReasoningEvaluator,
+    PairwiseAnswerEvaluator,
 )
+from ragelo.types.types import AnswerEvaluatorResult
 
 
 class TestPairwiseWithReasoningEvaluator:
-    def test_run(
+    @pytest.mark.asyncio
+    async def test_batch_eval(
         self,
         llm_provider_pairwise_answer_mock,
         pairwise_answer_eval_config,
         answers_test,
     ):
-        evaluator = PairwiseWithReasoningEvaluator.from_config(
+        evaluator = PairwiseAnswerEvaluator.from_config(
             config=pairwise_answer_eval_config,
             llm_provider=llm_provider_pairwise_answer_mock,
         )
-        answers = evaluator.batch_evaluate(answers_test)
-        assert len(answers) == 4
-        assert answers[0].answer == "A" and "[[A]]" in answers[0].raw_answer
-        assert answers[1].answer == "B" and "[[B]]" in answers[1].raw_answer
-        assert answers[2].answer == "C" and "[[C]]" in answers[2].raw_answer
-        assert answers[3].answer == "C" and "[[C]]" in answers[2].raw_answer
+        queries = await evaluator._async_batch_evaluate(answers_test)
+        flat_answers = [(q, a) for q in queries for a in q.pairwise_games]
+        evaluations = [a.evaluation for (_, a) in flat_answers]
+        assert len(evaluations) == 4
+        expected_answers = ["A", "B", "C", "C"]
+        for e, expected_ans in zip(evaluations, expected_answers):
+            assert isinstance(e, AnswerEvaluatorResult)
+            assert isinstance(e.answer, str)
+            assert isinstance(e.raw_answer, str)
+            assert e.answer == expected_ans
+            assert f"[[{expected_ans}]]" in e.raw_answer
 
-        llm_call_args = llm_provider_pairwise_answer_mock.call_mocker.call_args_list
+        llm_call_args = (
+            llm_provider_pairwise_answer_mock.async_call_mocker.call_args_list
+        )
         assert len(llm_call_args) == 4
         assert isinstance(llm_call_args[0][0][0], str)
         assert llm_call_args[0][0][0] != llm_call_args[1][0][0]
         # Make sure that no games with the same agent were called
         for call_arg in llm_call_args:
             agent_a_answer = (
                 call_arg[0][0]
@@ -41,34 +50,42 @@
                 .split("[The Start of Assistant B's Answer]")[1]
                 .split("[The End of Assistant B's Answer]")[0]
             ).strip()
             assert agent_a_answer != agent_b_answer
 
 
 class TestCustomPromptEvaluator:
-    def test_run(
-        self, llm_provider_answer_mock, custom_answer_eval_config, answers_test
+    @pytest.mark.asyncio
+    async def test_batch_eval(
+        self,
+        llm_provider_answer_mock,
+        custom_answer_eval_config,
+        answers_test,
     ):
         evaluator = CustomPromptEvaluator.from_config(
             config=custom_answer_eval_config,
             llm_provider=llm_provider_answer_mock,
         )
-        answers = evaluator.batch_evaluate(answers_test)
-        flat_answers = [(q, a) for q in answers_test for a in q.answers]
-        assert all([isinstance(a.answer, dict) for a in answers])
-        assert len(answers) == 4
-        assert answers[0].agent == answers[2].agent == "agent1"
-        assert answers[1].agent == answers[3].agent == "agent2"
-
-        parsed_answer = cast(dict[str, int], answers[0].answer)
-        assert parsed_answer["quality"] == 2
-        assert parsed_answer["trustworthiness"] == 1
-        assert parsed_answer["originality"] == 1
+        answers = await evaluator._async_batch_evaluate(answers_test)
+        flat_answers = [(q, a) for q in answers for a in q.answers]
+        evaluations = [a.evaluation for (_, a) in flat_answers]
+        assert len(evaluations) == 4
+        for a in evaluations:
+            assert isinstance(a, AnswerEvaluatorResult)
+            assert isinstance(a.answer, dict)
+            assert isinstance(a.raw_answer, str)
+            assert isinstance(a.answer["quality"], int)
+            assert isinstance(a.answer["trustworthiness"], int)
+            assert isinstance(a.answer["originality"], int)
+
+            assert a.answer["quality"] == 1
+            assert a.answer["trustworthiness"] == 0
+            assert a.answer["originality"] == 0
 
-        llm_call_args = llm_provider_answer_mock.call_mocker.call_args_list
+        llm_call_args = llm_provider_answer_mock.async_call_mocker.call_args_list
         assert (
             len(
                 llm_call_args[0][0][0]
                 .split("DOCUMENTS RETRIEVED:")[1]
                 .split("User Query")[0]
                 .strip()
                 .split("\n")
@@ -84,11 +101,11 @@
             expected_answer = a.text
             assert submitted_query == expected_query
             assert submitted_answer == expected_answer
 
 
 def test_get_by_name(llm_provider_pairwise_answer_mock, pairwise_answer_eval_config):
     evaluator = get_answer_evaluator(
-        "pairwise_reasoning",
+        "pairwise",
         llm_provider_pairwise_answer_mock,
     )
-    assert isinstance(evaluator, PairwiseWithReasoningEvaluator)
+    assert isinstance(evaluator, PairwiseAnswerEvaluator)
```

### Comparing `ragelo-0.1.1/tests/unit/test_llm_providers.py` & `ragelo-0.1.2/tests/unit/test_llm_providers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,73 @@
-from openai.types.chat.chat_completion import ChatCompletion, Choice
-from openai.types.chat.chat_completion_message import ChatCompletionMessage
+from unittest.mock import AsyncMock
+
+import pytest
 
 from ragelo import get_llm_provider
 from ragelo.llm_providers.openai_client import OpenAIProvider
 
 
 class TestOpenAIProvider:
     def test_response(
         self,
         chat_completion_mock,
         openai_client_mock,
         openai_client_config,
         monkeypatch,
+        mocker,
     ):
-        chat_completion_mock.create.return_value = ChatCompletion(
-            id="fake id",
-            choices=[
-                Choice(
-                    finish_reason="stop",
-                    index=0,
-                    logprobs=None,
-                    message=ChatCompletionMessage(
-                        content="fake response", role="assistant"
-                    ),
-                )
-            ],
-            created=0,
-            model="fake model",
-            object="chat.completion",
+        mocker.patch("openai.types.chat.chat_completion", new_callable=AsyncMock)
+
+        openai_client = OpenAIProvider(config=openai_client_config)
+        monkeypatch.setattr(
+            openai_client, "_OpenAIProvider__openai_client", openai_client_mock
         )
+
+        prompt = "hello world"
+        prompts = [
+            {"role": "system", "content": "hello world"},
+            {"role": "user", "content": "hello openai"},
+        ]
+        result = openai_client(prompt)
+        assert result == "fake response"
+        result = openai_client(prompts)
+        assert result == "fake response"
+
+        call_args = chat_completion_mock.create.call_args_list
+        assert call_args[0][1]["model"] == "fake model"
+        assert call_args[0][1]["messages"] == [{"role": "system", "content": prompt}]
+        assert call_args[1][1]["messages"] == prompts
+
+    @pytest.mark.asyncio
+    async def test_parallel_call(
+        self,
+        chat_completion_mock,
+        openai_client_mock,
+        openai_client_config,
+        monkeypatch,
+        mocker,
+    ):
+        mocker.patch("openai.types.chat.chat_completion", new_callable=AsyncMock)
+
         openai_client = OpenAIProvider(config=openai_client_config)
         monkeypatch.setattr(
             openai_client, "_OpenAIProvider__openai_client", openai_client_mock
         )
 
         prompt = "hello world"
         prompts = [
             {"role": "system", "content": "hello world"},
             {"role": "user", "content": "hello openai"},
         ]
-        result_1 = openai_client(prompt)
-        openai_client(prompts)
+        result = await openai_client.call_async(prompt)
+        assert result == "fake response"
+        result = await openai_client.call_async(prompts)
+        assert result == "fake response"
+
         call_args = chat_completion_mock.create.call_args_list
         assert call_args[0][1]["model"] == "fake model"
         assert call_args[0][1]["messages"] == [{"role": "system", "content": prompt}]
         assert call_args[1][1]["messages"] == prompts
-        assert result_1 == "fake response"
 
     def test_get_by_name(self, openai_client_config, openai_client_mock):
         provider = get_llm_provider("openai", api_key="fake key")
         assert isinstance(provider, OpenAIProvider)
```

### Comparing `ragelo-0.1.1/tests/unit/test_retrieval_evaluators.py` & `ragelo-0.1.2/tests/unit/test_retrieval_evaluators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import json
-from unittest.mock import Mock
+from unittest.mock import AsyncMock
+
+import pytest
 
 from ragelo import get_retrieval_evaluator
 from ragelo.evaluators.retrieval_evaluators import (
     BaseRetrievalEvaluator,
     CustomPromptEvaluator,
     DomainExpertEvaluator,
     FewShotEvaluator,
     RDNAMEvaluator,
     ReasonerEvaluator,
 )
 from ragelo.types import Document, Query
+from ragelo.types.types import RetrievalEvaluatorResult
 
 
 class RetrievalEvaluator(BaseRetrievalEvaluator):
     def _build_message(self, query: Query, document: Document) -> str:
         return f"Query: {query.query}\nDocument: {document.text}"
 
 
@@ -27,55 +30,53 @@
     ):
         evaluator = RetrievalEvaluator.from_config(
             config=base_eval_config, llm_provider=llm_provider_json_mock
         )
         query = qs_with_docs[0]
         doc = query.retrieved_docs[0]
         raw_answer, answer = evaluator.evaluate(query, doc)
-        assert raw_answer == 'LLM JSON response\n{"relevance": 0}'
-        assert answer == 0
+        assert raw_answer == 'Async LLM JSON response\n{"relevance": 1}'
+        assert answer == 1
 
         expected_prompt = f"Query: {query.query}\nDocument: {doc.text}"
-        call_args = llm_provider_json_mock.call_mocker.call_args_list
+        call_args = llm_provider_json_mock.async_call_mocker.call_args_list
         assert call_args[0][0][0] == expected_prompt
 
-    def test_batch_eval(
+    @pytest.mark.asyncio
+    async def test_batch_eval(
         self,
         llm_provider_json_mock,
         base_eval_config,
         qs_with_docs,
     ):
         base_eval_config.answer_format = "json"
         evaluator = RetrievalEvaluator.from_config(
             config=base_eval_config, llm_provider=llm_provider_json_mock
         )
-        results = evaluator.batch_evaluate(qs_with_docs)
-        assert len(results) == 4
-        assert results[0].qid == results[1].qid == "0"
-        assert results[2].qid == results[3].qid == "1"
-        assert results[0].did == "0"
-        assert results[2].did == "2"
-
-        call_args = llm_provider_json_mock.call_mocker.call_args_list
-        expected_prompts = []
-        for query in qs_with_docs:
-            for doc in query.retrieved_docs:
-                expected_prompts.append(f"Query: {query.query}\nDocument: {doc.text}")
-        for i, call in enumerate(call_args):
-            assert call[0][0] == expected_prompts[i]
+        queries = await evaluator._async_batch_evaluate(qs_with_docs)
+        evaluations = [a.evaluation for q in queries for a in q.retrieved_docs]
+        doc_ids = ["0", "1", "2", "3"]
+        qids = ["0", "0", "1", "1"]
+        for e, did, qid in zip(evaluations, doc_ids, qids):
+            assert isinstance(e, RetrievalEvaluatorResult)
+            assert isinstance(e.raw_answer, str)
+            assert e.raw_answer.startswith("Async")
+            assert isinstance(e.answer, int)
+            assert e.did == did
+            assert e.qid == qid
 
     def test_evaluate_with_text(self, llm_provider_json_mock, base_eval_config):
         evaluator = RetrievalEvaluator.from_config(
             config=base_eval_config, llm_provider=llm_provider_json_mock
         )
         raw_answer, processed_answer = evaluator.evaluate(
             document="This is a query", query="This is a document"
         )
-        assert raw_answer == 'LLM JSON response\n{"relevance": 0}'
-        assert processed_answer == 0
+        assert raw_answer == 'Async LLM JSON response\n{"relevance": 1}'
+        assert processed_answer == 1
 
     def test_rich_printing(
         self,
         llm_provider_json_mock,
         base_eval_config,
         qs_with_docs,
         capsys,
@@ -89,15 +90,15 @@
         captured = capsys.readouterr()
         assert "🔎" in captured.out
 
     def test_get_by_name(self, llm_provider_mock, expert_retrieval_eval_config):
         domain_expert_evaluator = get_retrieval_evaluator(
             "domain_expert",
             llm_provider_mock,
-            domain_long=expert_retrieval_eval_config.domain_long,
+            expert_in=expert_retrieval_eval_config.expert_in,
         )
         assert isinstance(domain_expert_evaluator, DomainExpertEvaluator)
         reasoner_evaluator = get_retrieval_evaluator(
             "reasoner",
             llm_provider_mock,
         )
         assert isinstance(reasoner_evaluator, ReasonerEvaluator)
@@ -120,15 +121,15 @@
         )
         query = rdnam_queries[0]
         doc = query.retrieved_docs[0]
         raw_answer, answer = evaluator.evaluate(query, doc)
         assert raw_answer == '"M": 2, "T": 1, "O": 1}, {"M": 1, "T": 1, "O": 2}]'
         assert answer == 1
 
-        call_args = llm_provider_mock_rdnam.call_mocker.call_args_list
+        call_args = llm_provider_mock_rdnam.async_call_mocker.call_args_list
         assert call_args[0][0][0].startswith(
             "You are a search quality rater evaluating"
         )
 
 
 class TestReasonerEvaluator:
     def test_process_single_answer(
@@ -141,15 +142,15 @@
             config=base_eval_config,
             llm_provider=llm_provider_mock,
         )
         query = qs_with_docs[0]
         doc = query.retrieved_docs[0]
         raw_answer, answer = evaluator.evaluate(query, doc)
         formatted_prompt = evaluator.prompt.format(query=query.query, document=doc.text)
-        call_args = llm_provider_mock.call_mocker.call_args_list
+        call_args = llm_provider_mock.async_call_mocker.call_args_list
 
         assert raw_answer == answer
         assert formatted_prompt in raw_answer
         assert call_args[0][0][0] == formatted_prompt
 
 
 class TestCustomPromptEvaluator:
@@ -171,17 +172,17 @@
             custom_prompt_retrieval_eval_config.document_placeholder: doc.text,
         }
         formatted_prompt = custom_prompt_retrieval_eval_config.prompt.format(
             **formatter
         )
 
         _, answer = evaluator.evaluate(query, doc)
-        call_args = llm_provider_json_mock.call_mocker.call_args_list
+        call_args = llm_provider_json_mock.async_call_mocker.call_args_list
 
-        assert answer == 0
+        assert answer == 1
         assert call_args[0][0][0] == formatted_prompt
 
     def test_process_with_custom_fields(
         self, llm_provider_json_mock, custom_prompt_retrieval_eval_config
     ):
         custom_prompt_retrieval_eval_config.prompt = "query: {query} doc: {document} q_metadata: {q_metadata} d_metadata: {d_metadata}"
         custom_prompt_retrieval_eval_config.query_placeholder = "query"
@@ -194,47 +195,47 @@
         evaluator.evaluate(
             query="this is a query",
             document="this is a document",
             query_metadata={"q_metadata": "q_1"},
             doc_metadata={"d_metadata": "d_1"},
         )
         assert (
-            llm_provider_json_mock.call_mocker.call_args_list[0][0][0]
+            llm_provider_json_mock.async_call_mocker.call_args_list[0][0][0]
             == "query: this is a query doc: this is a document q_metadata: q_1 d_metadata: d_1"
         )
 
 
 class TestDomainExpertEvaluator:
     def test_sys_prompt(self, llm_provider_mock, expert_retrieval_eval_config):
         evaluator = DomainExpertEvaluator.from_config(
             config=expert_retrieval_eval_config, llm_provider=llm_provider_mock
         )
-        assert expert_retrieval_eval_config.domain_long in evaluator.sys_prompt
+        assert expert_retrieval_eval_config.expert_in in evaluator.sys_prompt
         assert expert_retrieval_eval_config.domain_short in evaluator.sys_prompt
         assert (
             f"You work for {expert_retrieval_eval_config.company}"
             in evaluator.sys_prompt
         )
 
     def test_process_single_answer(
         self,
-        llm_provider_mock_mock,
+        llm_provider_mock,
         expert_retrieval_eval_config,
         qs_with_docs,
     ):
         evaluator = DomainExpertEvaluator.from_config(
             config=expert_retrieval_eval_config,
-            llm_provider=llm_provider_mock_mock,
+            llm_provider=llm_provider_mock,
         )
         query = qs_with_docs[0]
         doc = query.retrieved_docs[0]
         _, _ = evaluator.evaluate(query, doc)
 
-        assert llm_provider_mock_mock.call_count == 2
-        call_args = llm_provider_mock_mock.call_args_list
+        assert llm_provider_mock.async_call_mocker.call_count == 2
+        call_args = llm_provider_mock.async_call_mocker.call_args_list
         prompts_reasoning = call_args[0][0][0]
         prompts_score = call_args[1][0][0]
         assert len(prompts_reasoning) == 2
         assert len(prompts_score) == 4
         assert prompts_score[0] == prompts_reasoning[0]
         assert prompts_score[1] == prompts_reasoning[1]
         assert prompts_score[0]["role"] == "system"
@@ -258,34 +259,36 @@
             config=few_shot_retrieval_eval_config,
             llm_provider=llm_provider_json_mock,
         )
         query = qs_with_docs[0]
         doc = query.retrieved_docs[0]
 
         raw_answer, answer = evaluator.evaluate(query, doc)
-        assert raw_answer == 'LLM JSON response\n{"relevance": 0}'
-        assert answer == 0
-        call_args = llm_provider_json_mock.call_mocker.call_args_list
+        assert raw_answer == 'Async LLM JSON response\n{"relevance": 1}'
+        assert answer == 1
+        call_args = llm_provider_json_mock.async_call_mocker.call_args_list
         call_messages = call_args[0][0][0]
         assert len(call_messages) == 6
         assert call_messages[0]["role"] == "system"
         assert (
             call_messages[1]["role"]
             == call_messages[3]["role"]
             == call_messages[5]["role"]
             == "user"
         )
         assert call_messages[2]["role"] == call_messages[4]["role"] == "assistant"
 
 
 class TestReadmeExamples:
     def test_rdnam_example(self, llm_provider_mock_rdnam):
-        llm_provider_mock_rdnam.call_mocker = Mock(side_effect=lambda _: '"O": 0\n}')
+        llm_provider_mock_rdnam.async_call_mocker = AsyncMock(
+            side_effect=lambda _: '"O": 0\n}'
+        )
         evaluator = get_retrieval_evaluator(
-            "RDNAM", llm_provider=llm_provider_mock_rdnam
+            "RDNAM", llm_provider=llm_provider_mock_rdnam, write_output=False
         )
         raw_answer, processed_answer = evaluator.evaluate(
             query="What is the capital of France?",
             document="Lyon is the second largest city in France.",
         )
         assert raw_answer == '"O": 0\n}'
         assert processed_answer == 0
@@ -312,28 +315,31 @@
         answer_dict = {
             "relevance": 0,
             "recency": 0,
             "truthfulness": 0,
             "reasoning": "The document is outdated and incorrect. Rio de Janeiro was the capital of Brazil until 1960 when it was changed to Brasília.",
         }
         mocked_llm_answer = json.dumps(answer_dict)
-        llm_provider_mock.call_mocker = Mock(side_effect=lambda _: mocked_llm_answer)
+        llm_provider_mock.async_call_mocker = AsyncMock(
+            side_effect=lambda _: mocked_llm_answer
+        )
         evaluator = get_retrieval_evaluator(
             "custom_prompt",
             llm_provider=llm_provider_mock,
             prompt=prompt,
             query_placeholder="q",
             document_placeholder="d",
             scoring_keys=["relevance", "recency", "truthfulness", "reasoning"],
             answer_format="multi_field_json",
+            write_output=False,
         )
 
         raw_answer, answer = evaluator.evaluate(
             query="What is the capital of Brazil?",
             document="Rio de Janeiro is the capital of Brazil.",
             query_metadata={"today_date": "08-04-2024"},
             doc_metadata={"document_date": "04-03-1950"},
         )
-        call_args = llm_provider_mock.call_mocker.call_args_list
+        call_args = llm_provider_mock.async_call_mocker.call_args_list
         assert raw_answer == mocked_llm_answer
         assert answer == answer_dict
         assert len(call_args) == 1
```

