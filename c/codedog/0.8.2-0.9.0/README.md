# Comparing `tmp/codedog-0.8.2.tar.gz` & `tmp/codedog-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedog-0.8.2.tar", max compression
+gzip compressed data, was "codedog-0.9.0.tar", max compression
```

## Comparing `codedog-0.8.2.tar` & `codedog-0.9.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1067 2023-08-22 09:36:57.335069 codedog-0.8.2/LICENSE
--rw-r--r--   0        0        0     3968 2023-08-22 09:36:57.335069 codedog-0.8.2/README.md
--rw-r--r--   0        0        0     3511 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/__init__.py
--rw-r--r--   0        0        0        0 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/actors/__init__.py
--rw-r--r--   0        0        0       22 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/actors/base.py
--rw-r--r--   0        0        0        0 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/actors/reporters/__init__.py
--rw-r--r--   0        0        0      198 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/actors/reporters/base.py
--rw-r--r--   0        0        0     1148 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/actors/reporters/code_review.py
--rw-r--r--   0        0        0     3225 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/actors/reporters/pr_summary.py
--rw-r--r--   0        0        0     2227 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/actors/reporters/pull_request.py
--rw-r--r--   0        0        0      283 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/chains/__init__.py
--rw-r--r--   0        0        0        0 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/chains/code_review/__init__.py
--rw-r--r--   0        0        0     4611 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/chains/code_review/base.py
--rw-r--r--   0        0        0      231 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/chains/code_review/prompts.py
--rw-r--r--   0        0        0     3529 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/chains/code_review/translate_code_review_chain.py
--rw-r--r--   0        0        0        0 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/chains/pr_summary/__init__.py
--rw-r--r--   0        0        0     6809 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/chains/pr_summary/base.py
--rw-r--r--   0        0        0      579 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/chains/pr_summary/prompts.py
--rw-r--r--   0        0        0     5081 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/chains/pr_summary/translate_pr_summary_chain.py
--rw-r--r--   0        0        0      219 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/chains/prompts.py
--rw-r--r--   0        0        0      701 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/localization.py
--rw-r--r--   0        0        0      738 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/models/__init__.py
--rw-r--r--   0        0        0      408 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/models/blob.py
--rw-r--r--   0        0        0     2018 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/models/change_file.py
--rw-r--r--   0        0        0      192 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/models/change_summary.py
--rw-r--r--   0        0        0      150 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/models/code_review.py
--rw-r--r--   0        0        0      818 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/models/commit.py
--rw-r--r--   0        0        0     1148 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/models/diff.py
--rw-r--r--   0        0        0      842 2023-08-22 09:36:57.335069 codedog-0.8.2/codedog/models/issue.py
--rw-r--r--   0        0        0      692 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/models/pr_summary.py
--rw-r--r--   0        0        0     1721 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/models/pull_request.py
--rw-r--r--   0        0        0     1016 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/models/repository.py
--rw-r--r--   0        0        0      111 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/processors/__init__.py
--rw-r--r--   0        0        0     3835 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/processors/pull_request_processor.py
--rw-r--r--   0        0        0      178 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/retrievers/__init__.py
--rw-r--r--   0        0        0     1375 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/retrievers/base.py
--rw-r--r--   0        0        0     8850 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/retrievers/github_retriever.py
--rw-r--r--   0        0        0     9426 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/retrievers/gitlab_retriever.py
--rw-r--r--   0        0        0        0 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/templates/__init__.py
--rw-r--r--   0        0        0        0 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/templates/grimoire_cn.py
--rw-r--r--   0        0        0     4880 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/templates/grimoire_en.py
--rw-r--r--   0        0        0     2596 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/templates/template_cn.py
--rw-r--r--   0        0        0     2519 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/templates/template_en.py
--rw-r--r--   0        0        0        0 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/utils/__init__.py
--rw-r--r--   0        0        0      486 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/utils/diff_utils.py
--rw-r--r--   0        0        0     1563 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/utils/langchain_utils.py
--rw-r--r--   0        0        0      118 2023-08-22 09:36:57.339069 codedog-0.8.2/codedog/version.py
--rw-r--r--   0        0        0     1841 2023-08-22 09:36:57.367070 codedog-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     4875 1970-01-01 00:00:00.000000 codedog-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-11 11:17:10.287728 codedog-0.9.0/LICENSE
+-rw-r--r--   0        0        0     4077 2024-05-31 06:30:36.915000 codedog-0.9.0/README.md
+-rw-r--r--   0        0        0     3511 2023-08-25 09:50:13.784920 codedog-0.9.0/codedog/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-11 11:17:10.288141 codedog-0.9.0/codedog/actors/__init__.py
+-rw-r--r--   0        0        0       22 2023-08-11 11:17:10.288238 codedog-0.9.0/codedog/actors/base.py
+-rw-r--r--   0        0        0        0 2023-08-11 11:17:10.288327 codedog-0.9.0/codedog/actors/reporters/__init__.py
+-rw-r--r--   0        0        0      198 2023-08-11 11:17:10.288421 codedog-0.9.0/codedog/actors/reporters/base.py
+-rw-r--r--   0        0        0     1148 2023-08-12 10:33:58.256966 codedog-0.9.0/codedog/actors/reporters/code_review.py
+-rw-r--r--   0        0        0     3225 2023-08-14 05:45:17.381529 codedog-0.9.0/codedog/actors/reporters/pr_summary.py
+-rw-r--r--   0        0        0     2227 2023-08-12 10:33:58.257212 codedog-0.9.0/codedog/actors/reporters/pull_request.py
+-rw-r--r--   0        0        0      283 2023-08-14 05:45:17.381823 codedog-0.9.0/codedog/chains/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-11 11:17:10.288942 codedog-0.9.0/codedog/chains/code_review/__init__.py
+-rw-r--r--   0        0        0     4611 2023-08-14 05:45:17.382087 codedog-0.9.0/codedog/chains/code_review/base.py
+-rw-r--r--   0        0        0      231 2023-08-11 11:17:10.289177 codedog-0.9.0/codedog/chains/code_review/prompts.py
+-rw-r--r--   0        0        0     3529 2023-08-15 13:47:22.914969 codedog-0.9.0/codedog/chains/code_review/translate_code_review_chain.py
+-rw-r--r--   0        0        0        0 2023-08-11 11:17:10.289260 codedog-0.9.0/codedog/chains/pr_summary/__init__.py
+-rw-r--r--   0        0        0     6809 2023-08-14 05:45:17.382533 codedog-0.9.0/codedog/chains/pr_summary/base.py
+-rw-r--r--   0        0        0      579 2023-08-13 02:49:52.728345 codedog-0.9.0/codedog/chains/pr_summary/prompts.py
+-rw-r--r--   0        0        0     5081 2023-08-15 13:47:22.915179 codedog-0.9.0/codedog/chains/pr_summary/translate_pr_summary_chain.py
+-rw-r--r--   0        0        0      219 2023-08-14 05:45:17.383029 codedog-0.9.0/codedog/chains/prompts.py
+-rw-r--r--   0        0        0      701 2023-08-14 05:45:17.383255 codedog-0.9.0/codedog/localization.py
+-rw-r--r--   0        0        0      738 2023-08-11 11:17:10.289784 codedog-0.9.0/codedog/models/__init__.py
+-rw-r--r--   0        0        0      408 2023-08-11 11:17:10.289867 codedog-0.9.0/codedog/models/blob.py
+-rw-r--r--   0        0        0     2018 2023-08-14 02:40:15.197392 codedog-0.9.0/codedog/models/change_file.py
+-rw-r--r--   0        0        0      192 2023-08-11 11:17:10.290042 codedog-0.9.0/codedog/models/change_summary.py
+-rw-r--r--   0        0        0      150 2023-08-11 11:17:10.290122 codedog-0.9.0/codedog/models/code_review.py
+-rw-r--r--   0        0        0      818 2023-08-25 09:50:13.785186 codedog-0.9.0/codedog/models/commit.py
+-rw-r--r--   0        0        0     1148 2023-08-11 11:17:10.290326 codedog-0.9.0/codedog/models/diff.py
+-rw-r--r--   0        0        0      842 2023-08-25 09:50:13.785400 codedog-0.9.0/codedog/models/issue.py
+-rw-r--r--   0        0        0      692 2023-08-11 11:17:10.290501 codedog-0.9.0/codedog/models/pr_summary.py
+-rw-r--r--   0        0        0     1721 2023-08-25 09:50:13.785638 codedog-0.9.0/codedog/models/pull_request.py
+-rw-r--r--   0        0        0     1016 2023-08-25 09:50:13.785842 codedog-0.9.0/codedog/models/repository.py
+-rw-r--r--   0        0        0      111 2023-08-11 11:17:10.290795 codedog-0.9.0/codedog/processors/__init__.py
+-rw-r--r--   0        0        0     3835 2023-08-11 11:17:10.290940 codedog-0.9.0/codedog/processors/pull_request_processor.py
+-rw-r--r--   0        0        0      178 2023-08-11 11:17:10.291081 codedog-0.9.0/codedog/retrievers/__init__.py
+-rw-r--r--   0        0        0     1375 2023-08-11 11:17:10.291184 codedog-0.9.0/codedog/retrievers/base.py
+-rw-r--r--   0        0        0     8850 2023-08-18 11:50:39.929453 codedog-0.9.0/codedog/retrievers/github_retriever.py
+-rw-r--r--   0        0        0     9426 2023-08-12 10:33:58.257983 codedog-0.9.0/codedog/retrievers/gitlab_retriever.py
+-rw-r--r--   0        0        0        0 2023-08-11 11:17:10.291478 codedog-0.9.0/codedog/templates/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-14 05:45:17.383535 codedog-0.9.0/codedog/templates/grimoire_cn.py
+-rw-r--r--   0        0        0     4880 2023-08-14 05:45:17.383796 codedog-0.9.0/codedog/templates/grimoire_en.py
+-rw-r--r--   0        0        0     2596 2023-08-14 05:45:17.383991 codedog-0.9.0/codedog/templates/template_cn.py
+-rw-r--r--   0        0        0     2519 2023-08-14 05:45:17.384193 codedog-0.9.0/codedog/templates/template_en.py
+-rw-r--r--   0        0        0        0 2023-08-11 11:17:10.291969 codedog-0.9.0/codedog/utils/__init__.py
+-rw-r--r--   0        0        0      486 2023-08-11 11:17:10.292066 codedog-0.9.0/codedog/utils/diff_utils.py
+-rw-r--r--   0        0        0     1579 2024-05-31 07:22:18.652254 codedog-0.9.0/codedog/utils/langchain_utils.py
+-rw-r--r--   0        0        0      118 2024-05-31 06:30:48.052006 codedog-0.9.0/codedog/version.py
+-rw-r--r--   0        0        0     1922 2024-05-31 06:30:48.051824 codedog-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4980 1970-01-01 00:00:00.000000 codedog-0.9.0/PKG-INFO
```

### Comparing `codedog-0.8.2/LICENSE` & `codedog-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/README.md` & `codedog-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # 🐶 Codedog
 
 [![Checkstyle](https://github.com/Arcadia822/codedog/actions/workflows/flake8.yml/badge.svg)](https://github.com/Arcadia822/codedog/actions/workflows/flake8.yml)
 [![Pytest](https://github.com/Arcadia822/codedog/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/Arcadia822/codedog/actions/workflows/test.yml)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Arcadia822/ce38dae58995aeffef42065093fcfe84/raw/codedog_master.json)](https://github.com/Arcadia822/codedog/actions/workflows/test.yml)
+[![](https://dcbadge.vercel.app/api/server/wzfsvaDQ?compact=true&style=flat)](https://discord.gg/6adMQxSpJS)
 
 Review your Github/Gitlab PR with ChatGPT
 
 ## What is codedog?
 
 Codedog is a code review automation tool benefit the power of LLM (Large Language Model) to help developers
 review code faster and more accurately.
```

### Comparing `codedog-0.8.2/codedog/__init__.py` & `codedog-0.9.0/codedog/__init__.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/actors/reporters/code_review.py` & `codedog-0.9.0/codedog/actors/reporters/code_review.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/actors/reporters/pr_summary.py` & `codedog-0.9.0/codedog/actors/reporters/pr_summary.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/actors/reporters/pull_request.py` & `codedog-0.9.0/codedog/actors/reporters/pull_request.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/chains/code_review/base.py` & `codedog-0.9.0/codedog/chains/code_review/base.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/chains/code_review/translate_code_review_chain.py` & `codedog-0.9.0/codedog/chains/code_review/translate_code_review_chain.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/chains/pr_summary/base.py` & `codedog-0.9.0/codedog/chains/pr_summary/base.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/chains/pr_summary/prompts.py` & `codedog-0.9.0/codedog/chains/pr_summary/prompts.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/chains/pr_summary/translate_pr_summary_chain.py` & `codedog-0.9.0/codedog/chains/pr_summary/translate_pr_summary_chain.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/localization.py` & `codedog-0.9.0/codedog/localization.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/models/__init__.py` & `codedog-0.9.0/codedog/models/__init__.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/models/change_file.py` & `codedog-0.9.0/codedog/models/change_file.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/models/commit.py` & `codedog-0.9.0/codedog/models/commit.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/models/diff.py` & `codedog-0.9.0/codedog/models/diff.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/models/issue.py` & `codedog-0.9.0/codedog/models/issue.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/models/pr_summary.py` & `codedog-0.9.0/codedog/models/pr_summary.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/models/pull_request.py` & `codedog-0.9.0/codedog/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/models/repository.py` & `codedog-0.9.0/codedog/models/repository.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/processors/pull_request_processor.py` & `codedog-0.9.0/codedog/processors/pull_request_processor.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/retrievers/base.py` & `codedog-0.9.0/codedog/retrievers/base.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/retrievers/github_retriever.py` & `codedog-0.9.0/codedog/retrievers/github_retriever.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/retrievers/gitlab_retriever.py` & `codedog-0.9.0/codedog/retrievers/gitlab_retriever.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/templates/grimoire_en.py` & `codedog-0.9.0/codedog/templates/grimoire_en.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/templates/template_cn.py` & `codedog-0.9.0/codedog/templates/template_cn.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/templates/template_en.py` & `codedog-0.9.0/codedog/templates/template_en.py`

 * *Files identical despite different names*

### Comparing `codedog-0.8.2/codedog/utils/langchain_utils.py` & `codedog-0.9.0/codedog/utils/langchain_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def load_gpt_llm() -> BaseChatModel:
     """Load GPT 3.5 Model"""
     if env.get("AZURE_OPENAI"):
         llm = AzureChatOpenAI(
             openai_api_type="azure",
             openai_api_key=env.get("AZURE_OPENAI_API_KEY", ""),
             openai_api_base=env.get("AZURE_OPENAI_API_BASE", ""),
-            openai_api_version="2023-05-15",
+            openai_api_version="2024-05-01-preview",
             deployment_name=env.get("AZURE_OPENAI_DEPLOYMENT_ID", "gpt-35-turbo"),
             model="gpt-3.5-turbo",
             temperature=0,
         )
     else:
         llm = ChatOpenAI(
             openai_api_key=env.get("OPENAI_API_KEY"),
@@ -30,15 +30,15 @@
 def load_gpt4_llm():
     """Load GPT 4 Model. Make sure your key have access to GPT 4 API. call this function won't check it."""
     if env.get("AZURE_OPENAI"):
         llm = AzureChatOpenAI(
             openai_api_type="azure",
             openai_api_key=env.get("AZURE_OPENAI_API_KEY", ""),
             openai_api_base=env.get("AZURE_OPENAI_API_BASE", ""),
-            openai_api_version="2023-05-15",
+            openai_api_version="2024-05-01-preview",
             deployment_name=env.get("AZURE_OPENAI_GPT4_DEPLOYMENT_ID", "gpt-4"),
             model="gpt-4",
             temperature=0,
         )
     else:
         llm = ChatOpenAI(
             openai_api_key=env.get("OPENAI_API_KEY"),
```

### Comparing `codedog-0.8.2/pyproject.toml` & `codedog-0.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 [tool.poetry]
 name = "codedog"
-version = "0.8.2"
+version = "0.9.0"
 license = "MIT"
 readme = "README.md"
 authors = ["Arcadia <arcadia822@gmail.com>", "Linpp "]
 description = "Codedog reviews your pull request using llm."
 repository = "https://www.github.com/codedog-ai/codedog"
 homepage = "https://www.codedog.ai"
 keywords = ["code review", "langchain", "llm"]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/codedog-ai/codedog/issues"
 "Discord" = "https://discord.gg/8TfqpFC4"
 
 [tool.poetry.dependencies]
 python = "~3.10"
-langchain = "^0.0.247"
-openai = "^0.27.8"
-pydantic = "^1.10.7"
-python-gitlab = "^3.14.0"
-pygithub = "^1.58.2"
+langchain = ">=0.0.247,<0.0.355"
+openai = ">=0.27.8,<1.31.0"
+pydantic = ">=1.10.7,<3.0.0"
+python-gitlab = ">=3.14,<5.0"
+pygithub = ">=1.58.2,<3.0.0"
 unidiff = "^0.7.5"
 
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-black = "^23.3.0"
-flake8 = "^6.0.0"
+black = ">=23.3,<25.0"
+flake8 = ">=6,<8"
 isort = "^5.12.0"
 python-semantic-release = "^8.0.5"
-langchain-visualizer = "^0.0.28"
+langchain-visualizer = ">=0.0.28,<0.0.31"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest-asyncio = "^0.20.3"
-pytest-cov = "^4.0.0"
+pytest-asyncio = ">=0.20.3,<0.22.0"
+pytest-cov = ">=4,<6"
 
 [tool.poetry.group.http]
 optional = true
 
 [tool.poetry.group.http.dependencies]
-fastapi = "^0.100.1"
-uvicorn = "^0.23.1"
+fastapi = ">=0.100.1,<0.112.0"
+uvicorn = ">=0.23.1,<0.30.0"
 
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
 pdoc = "^14.0.0"
```

### Comparing `codedog-0.8.2/PKG-INFO` & `codedog-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: codedog
-Version: 0.8.2
+Version: 0.9.0
 Summary: Codedog reviews your pull request using llm.
 Home-page: https://www.codedog.ai
 License: MIT
 Keywords: code review,langchain,llm
 Author: Arcadia
 Author-email: arcadia822@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: langchain (>=0.0.247,<0.0.248)
-Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: pygithub (>=1.58.2,<2.0.0)
-Requires-Dist: python-gitlab (>=3.14.0,<4.0.0)
+Requires-Dist: langchain (>=0.0.247,<0.0.355)
+Requires-Dist: openai (>=0.27.8,<1.31.0)
+Requires-Dist: pydantic (>=1.10.7,<3.0.0)
+Requires-Dist: pygithub (>=1.58.2,<3.0.0)
+Requires-Dist: python-gitlab (>=3.14,<5.0)
 Requires-Dist: unidiff (>=0.7.5,<0.8.0)
 Project-URL: Bug Tracker, https://github.com/codedog-ai/codedog/issues
 Project-URL: Discord, https://discord.gg/8TfqpFC4
 Project-URL: Repository, https://www.github.com/codedog-ai/codedog
 Description-Content-Type: text/markdown
 
 # 🐶 Codedog
 
 [![Checkstyle](https://github.com/Arcadia822/codedog/actions/workflows/flake8.yml/badge.svg)](https://github.com/Arcadia822/codedog/actions/workflows/flake8.yml)
 [![Pytest](https://github.com/Arcadia822/codedog/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/Arcadia822/codedog/actions/workflows/test.yml)
 [![Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/Arcadia822/ce38dae58995aeffef42065093fcfe84/raw/codedog_master.json)](https://github.com/Arcadia822/codedog/actions/workflows/test.yml)
+[![](https://dcbadge.vercel.app/api/server/wzfsvaDQ?compact=true&style=flat)](https://discord.gg/6adMQxSpJS)
 
 Review your Github/Gitlab PR with ChatGPT
 
 ## What is codedog?
 
 Codedog is a code review automation tool benefit the power of LLM (Large Language Model) to help developers
 review code faster and more accurately.
```

