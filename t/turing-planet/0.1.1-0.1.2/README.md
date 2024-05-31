# Comparing `tmp/turing-planet-0.1.1.tar.gz` & `tmp/turing-planet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turing-planet-0.1.1.tar", last modified: Thu Apr 25 12:14:26 2024, max compression
+gzip compressed data, was "turing-planet-0.1.2.tar", last modified: Fri May 31 06:03:39 2024, max compression
```

## Comparing `turing-planet-0.1.1.tar` & `turing-planet-0.1.2.tar`

### file list

```diff
@@ -1,127 +1,137 @@
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.885544 turing-planet-0.1.1/
--rw-rw-rw-   0        0        0     2579 2024-04-25 12:14:26.883535 turing-planet-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-25 12:14:26.885544 turing-planet-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      891 2024-04-25 12:14:25.000000 turing-planet-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.643176 turing-planet-0.1.1/test/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.649160 turing-planet-0.1.1/test/api/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/api/__init__.py
--rw-rw-rw-   0        0        0     2914 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/api/sample_spark_chat_client.py
--rw-rw-rw-   0        0        0     6166 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/api/sample_spark_embedding.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.668110 turing-planet-0.1.1/test/langchain/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/langchain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.690051 turing-planet-0.1.1/test/langchain/agents/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/langchain/agents/__init__.py
--rw-rw-rw-   0        0        0     1722 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/langchain/agents/agent_qa.py
--rw-rw-rw-   0        0        0     1842 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/langchain/agents/ask.py
--rw-rw-rw-   0        0        0     2006 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/langchain/agents/ask2.py
--rw-rw-rw-   0        0        0     3471 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/langchain/agents/plan.py
--rw-rw-rw-   0        0        0     1178 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/langchain/agents/quick_start.py
--rw-rw-rw-   0        0        0     4196 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/langchain/agents/react.py
--rw-rw-rw-   0        0        0     2021 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/langchain/agents/slot.py
--rw-rw-rw-   0        0        0     2335 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/langchain/agents/slot2.py
--rw-rw-rw-   0        0        0     8842 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/langchain/agents/sparkai_agent.py
--rw-rw-rw-   0        0        0     2223 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/langchain/agents/tools.py
--rw-rw-rw-   0        0        0     2822 2024-04-18 03:49:36.000000 turing-planet-0.1.1/test/langchain/agents.py
--rw-rw-rw-   0        0        0     3405 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/langchain/chat_model.py
--rw-rw-rw-   0        0        0     2987 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/langchain/embed.py
--rw-rw-rw-   0        0        0     4898 2024-04-18 03:49:37.000000 turing-planet-0.1.1/test/langchain/function_call.py
--rw-rw-rw-   0        0        0     2554 2024-04-18 03:49:37.000000 turing-planet-0.1.1/test/langchain/function_call_aiui.py
--rw-rw-rw-   0        0        0     2332 2024-04-18 03:49:37.000000 turing-planet-0.1.1/test/langchain/llm.py
--rw-rw-rw-   0        0        0     3279 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/langchain/memory.py
--rw-rw-rw-   0        0        0     4790 2024-04-18 03:49:37.000000 turing-planet-0.1.1/test/langchain/retrieval.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.704013 turing-planet-0.1.1/test/llama_index/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/test/llama_index/__init__.py
--rw-rw-rw-   0        0        0      148 2024-04-18 03:49:37.000000 turing-planet-0.1.1/test/llama_index/base.py
--rw-rw-rw-   0        0        0     4960 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/indexing.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.740914 turing-planet-0.1.1/test/llama_index/introduce/
--rw-rw-rw-   0        0        0     1282 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/introduce/01_start.py
--rw-rw-rw-   0        0        0     1154 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/introduce/02_reader.py
--rw-rw-rw-   0        0        0     1064 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/introduce/03_custom_file_reader.py
--rw-rw-rw-   0        0        0      920 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/introduce/04_doc_metadata.py
--rw-rw-rw-   0        0        0     1716 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/introduce/05_splitter.py
--rw-rw-rw-   0        0        0     3275 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/introduce/06_node_metadata.py
--rw-rw-rw-   0        0        0     1296 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/introduce/07_retriever.py
--rw-rw-rw-   0        0        0     4030 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/introduce/07_retriever_custom.py
--rw-rw-rw-   0        0        0     1891 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/introduce/08_postprocessor.py
--rw-rw-rw-   0        0        0      791 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/introduce/09_prompt.py
--rw-rw-rw-   0        0        0     1441 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/introduce/10_multistep_query_engine.py
--rw-rw-rw-   0        0        0     3375 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/introduce/11_route_query_engine.py
--rw-rw-rw-   0        0        0      716 2024-04-18 03:49:37.000000 turing-planet-0.1.1/test/llama_index/introduce/12_llamahub.py
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/test/llama_index/introduce/__init__.py
--rw-rw-rw-   0        0        0     2423 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/introduce/introduce_base.py
--rw-rw-rw-   0        0        0      497 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/introduce/nltk_demo.py
--rw-rw-rw-   0        0        0     5622 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/metadata.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.768840 turing-planet-0.1.1/test/llama_index/optimizing/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/test/llama_index/optimizing/__init__.py
--rw-rw-rw-   0        0        0     8086 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/optimizing/base.py
--rw-rw-rw-   0        0        0     3311 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/optimizing/custom_keyword_extractor.py
--rw-rw-rw-   0        0        0     4533 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/optimizing/docx_keyword_vector.py
--rw-rw-rw-   0        0        0       27 2024-04-18 03:49:37.000000 turing-planet-0.1.1/test/llama_index/optimizing/kg_index.py
--rw-rw-rw-   0        0        0     7180 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/optimizing/qa_metadata.py
--rw-rw-rw-   0        0        0     4294 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/optimizing/summary_index.py
--rw-rw-rw-   0        0        0      301 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/optimizing/summary_metadata.py
--rw-rw-rw-   0        0        0     4301 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/optimizing/turing_knowledge.py
--rw-rw-rw-   0        0        0    12176 2024-04-18 03:49:37.000000 turing-planet-0.1.1/test/llama_index/optimizing/vector_index.py
--rw-rw-rw-   0        0        0     8677 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/optimizing/vector_index_cq.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.795769 turing-planet-0.1.1/test/llama_index/pk/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/test/llama_index/pk/__init__.py
--rw-rw-rw-   0        0        0     1615 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/pk/base.py
--rw-rw-rw-   0        0        0     3819 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/pk/llama_index_spark-0131.py
--rw-rw-rw-   0        0        0     5240 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/pk/pk.py
--rw-rw-rw-   0        0        0     5585 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/pk/pk_excel_chunsize.py
--rw-rw-rw-   0        0        0     5904 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/pk/pk_excel_chunsize_rerank.py
--rw-rw-rw-   0        0        0     5320 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/pk/pk_excel_embedding.py
--rw-rw-rw-   0        0        0     6263 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/pk/pk_word_0201.py
--rw-rw-rw-   0        0        0     8691 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/pk/pk_word_es_0201.py
--rw-rw-rw-   0        0        0     3881 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/pk/sample_excel.py
--rw-rw-rw-   0        0        0     3730 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/skydoc-embedding.py
--rw-rw-rw-   0        0        0     5113 2024-04-25 12:11:33.000000 turing-planet-0.1.1/test/llama_index/start.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.798761 turing-planet-0.1.1/turing_planet/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.818707 turing-planet-0.1.1/turing_planet/api/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/api/__init__.py
--rw-rw-rw-   0        0        0     2478 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/api/planet_embedding_client.py
--rw-rw-rw-   0        0        0     4873 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/api/planet_vector_client.py
--rw-rw-rw-   0        0        0     8107 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/api/spark_chat_client.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.821699 turing-planet-0.1.1/turing_planet/deprecated/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/deprecated/__init__.py
--rw-rw-rw-   0        0        0     6952 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/deprecated/spark_embedding_client.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.824692 turing-planet-0.1.1/turing_planet/langchain/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/langchain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.827684 turing-planet-0.1.1/turing_planet/langchain/chat_models/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/langchain/chat_models/__init__.py
--rw-rw-rw-   0        0        0     8131 2024-04-25 12:11:33.000000 turing-planet-0.1.1/turing_planet/langchain/chat_models/sparkai.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.831673 turing-planet-0.1.1/turing_planet/langchain/embeddings/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/langchain/embeddings/__init__.py
--rw-rw-rw-   0        0        0      765 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/langchain/embeddings/sparkai.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.835662 turing-planet-0.1.1/turing_planet/langchain/llm/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/langchain/llm/__init__.py
--rw-rw-rw-   0        0        0     5350 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/langchain/llm/sparkai.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.838655 turing-planet-0.1.1/turing_planet/llama_index/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/llama_index/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.843642 turing-planet-0.1.1/turing_planet/llama_index/embeddings/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/llama_index/embeddings/__init__.py
--rw-rw-rw-   0        0        0     1592 2024-04-25 12:11:33.000000 turing-planet-0.1.1/turing_planet/llama_index/embeddings/sparkai.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.850623 turing-planet-0.1.1/turing_planet/llama_index/llms/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/llama_index/llms/__init__.py
--rw-rw-rw-   0        0        0     3143 2024-04-25 12:11:33.000000 turing-planet-0.1.1/turing_planet/llama_index/llms/sparkai.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.855609 turing-planet-0.1.1/turing_planet/llama_index/readers/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/llama_index/readers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.864588 turing-planet-0.1.1/turing_planet/llama_index/readers/file/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/llama_index/readers/file/__init__.py
--rw-rw-rw-   0        0        0     1705 2024-04-25 12:11:33.000000 turing-planet-0.1.1/turing_planet/llama_index/readers/file/excel.py
--rw-rw-rw-   0        0        0     1190 2024-04-25 12:11:33.000000 turing-planet-0.1.1/turing_planet/llama_index/readers/file/turing_markdown_reader.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.869572 turing-planet-0.1.1/turing_planet/llama_index/vector_stores/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/llama_index/vector_stores/__init__.py
--rw-rw-rw-   0        0        0     3320 2024-04-25 12:11:33.000000 turing-planet-0.1.1/turing_planet/llama_index/vector_stores/planet.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.877550 turing-planet-0.1.1/turing_planet/utils/
--rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/utils/__init__.py
--rw-rw-rw-   0        0        0     2102 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/utils/auth_util.py
--rw-rw-rw-   0        0        0     1009 2024-04-18 03:49:37.000000 turing-planet-0.1.1/turing_planet/utils/env.py
-drwxrwxrwx   0        0        0        0 2024-04-25 12:14:26.880543 turing-planet-0.1.1/turing_planet.egg-info/
--rw-rw-rw-   0        0        0     2579 2024-04-25 12:14:26.000000 turing-planet-0.1.1/turing_planet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3871 2024-04-25 12:14:26.000000 turing-planet-0.1.1/turing_planet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-25 12:14:26.000000 turing-planet-0.1.1/turing_planet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-04-25 12:14:26.000000 turing-planet-0.1.1/turing_planet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-25 12:14:26.000000 turing-planet-0.1.1/turing_planet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.746788 turing-planet-0.1.2/
+-rw-rw-rw-   0        0        0     2579 2024-05-31 06:03:39.743797 turing-planet-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-31 06:03:39.746788 turing-planet-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      891 2024-05-31 06:03:14.000000 turing-planet-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.229174 turing-planet-0.1.2/test/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.242142 turing-planet-0.1.2/test/api/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/api/__init__.py
+-rw-rw-rw-   0        0        0     2914 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/api/sample_spark_chat_client.py
+-rw-rw-rw-   0        0        0     6166 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/api/sample_spark_embedding.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.282030 turing-planet-0.1.2/test/langchain/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/langchain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.343865 turing-planet-0.1.2/test/langchain/agents/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/langchain/agents/__init__.py
+-rw-rw-rw-   0        0        0     1722 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/langchain/agents/agent_qa.py
+-rw-rw-rw-   0        0        0     1842 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/langchain/agents/ask.py
+-rw-rw-rw-   0        0        0     2006 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/langchain/agents/ask2.py
+-rw-rw-rw-   0        0        0     3471 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/langchain/agents/plan.py
+-rw-rw-rw-   0        0        0     1178 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/langchain/agents/quick_start.py
+-rw-rw-rw-   0        0        0     4196 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/langchain/agents/react.py
+-rw-rw-rw-   0        0        0     2021 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/langchain/agents/slot.py
+-rw-rw-rw-   0        0        0     2335 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/langchain/agents/slot2.py
+-rw-rw-rw-   0        0        0     8842 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/langchain/agents/sparkai_agent.py
+-rw-rw-rw-   0        0        0     2223 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/langchain/agents/tools.py
+-rw-rw-rw-   0        0        0     2822 2024-04-18 03:49:36.000000 turing-planet-0.1.2/test/langchain/agents.py
+-rw-rw-rw-   0        0        0     3405 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/langchain/chat_model.py
+-rw-rw-rw-   0        0        0     2987 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/langchain/embed.py
+-rw-rw-rw-   0        0        0     4898 2024-04-18 03:49:37.000000 turing-planet-0.1.2/test/langchain/function_call.py
+-rw-rw-rw-   0        0        0     2554 2024-04-18 03:49:37.000000 turing-planet-0.1.2/test/langchain/function_call_aiui.py
+-rw-rw-rw-   0        0        0     2332 2024-04-18 03:49:37.000000 turing-planet-0.1.2/test/langchain/llm.py
+-rw-rw-rw-   0        0        0     3279 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/langchain/memory.py
+-rw-rw-rw-   0        0        0     4790 2024-04-18 03:49:37.000000 turing-planet-0.1.2/test/langchain/retrieval.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.371791 turing-planet-0.1.2/test/llama_index/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/test/llama_index/__init__.py
+-rw-rw-rw-   0        0        0      148 2024-04-18 03:49:37.000000 turing-planet-0.1.2/test/llama_index/base.py
+-rw-rw-rw-   0        0        0     4960 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/indexing.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.459557 turing-planet-0.1.2/test/llama_index/introduce/
+-rw-rw-rw-   0        0        0     1282 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/01_start.py
+-rw-rw-rw-   0        0        0     1154 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/02_reader.py
+-rw-rw-rw-   0        0        0     1064 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/03_custom_file_reader.py
+-rw-rw-rw-   0        0        0      920 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/04_doc_metadata.py
+-rw-rw-rw-   0        0        0     1716 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/05_splitter.py
+-rw-rw-rw-   0        0        0     3275 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/06_node_metadata.py
+-rw-rw-rw-   0        0        0     1296 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/07_retriever.py
+-rw-rw-rw-   0        0        0     4030 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/07_retriever_custom.py
+-rw-rw-rw-   0        0        0     1891 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/08_postprocessor.py
+-rw-rw-rw-   0        0        0      791 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/09_prompt.py
+-rw-rw-rw-   0        0        0     1441 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/10_multistep_query_engine.py
+-rw-rw-rw-   0        0        0     3375 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/11_route_query_engine.py
+-rw-rw-rw-   0        0        0      716 2024-04-18 03:49:37.000000 turing-planet-0.1.2/test/llama_index/introduce/12_llamahub.py
+-rw-rw-rw-   0        0        0      685 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/13_docqa_split.py
+-rw-rw-rw-   0        0        0      277 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/14_docqa_index.py
+-rw-rw-rw-   0        0        0     1199 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/15_docqa_retriever.py
+-rw-rw-rw-   0        0        0     1075 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/16_docstore.py
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/test/llama_index/introduce/__init__.py
+-rw-rw-rw-   0        0        0     2445 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/introduce_base.py
+-rw-rw-rw-   0        0        0      497 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/introduce/nltk_demo.py
+-rw-rw-rw-   0        0        0     5622 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/metadata.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.520394 turing-planet-0.1.2/test/llama_index/optimizing/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/test/llama_index/optimizing/__init__.py
+-rw-rw-rw-   0        0        0     8086 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/optimizing/base.py
+-rw-rw-rw-   0        0        0     3311 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/optimizing/custom_keyword_extractor.py
+-rw-rw-rw-   0        0        0     4533 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/optimizing/docx_keyword_vector.py
+-rw-rw-rw-   0        0        0       27 2024-04-18 03:49:37.000000 turing-planet-0.1.2/test/llama_index/optimizing/kg_index.py
+-rw-rw-rw-   0        0        0     7180 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/optimizing/qa_metadata.py
+-rw-rw-rw-   0        0        0     4294 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/optimizing/summary_index.py
+-rw-rw-rw-   0        0        0      301 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/optimizing/summary_metadata.py
+-rw-rw-rw-   0        0        0     4301 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/optimizing/turing_knowledge.py
+-rw-rw-rw-   0        0        0    12176 2024-04-18 03:49:37.000000 turing-planet-0.1.2/test/llama_index/optimizing/vector_index.py
+-rw-rw-rw-   0        0        0     8677 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/optimizing/vector_index_cq.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.564278 turing-planet-0.1.2/test/llama_index/pk/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/test/llama_index/pk/__init__.py
+-rw-rw-rw-   0        0        0     1615 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/pk/base.py
+-rw-rw-rw-   0        0        0     3819 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/pk/llama_index_spark-0131.py
+-rw-rw-rw-   0        0        0     5240 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/pk/pk.py
+-rw-rw-rw-   0        0        0     5585 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/pk/pk_excel_chunsize.py
+-rw-rw-rw-   0        0        0     5904 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/pk/pk_excel_chunsize_rerank.py
+-rw-rw-rw-   0        0        0     5320 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/pk/pk_excel_embedding.py
+-rw-rw-rw-   0        0        0     6263 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/pk/pk_word_0201.py
+-rw-rw-rw-   0        0        0     8691 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/pk/pk_word_es_0201.py
+-rw-rw-rw-   0        0        0     3881 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/pk/sample_excel.py
+-rw-rw-rw-   0        0        0     3730 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/skydoc-embedding.py
+-rw-rw-rw-   0        0        0     5724 2024-05-31 06:03:14.000000 turing-planet-0.1.2/test/llama_index/start.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.568266 turing-planet-0.1.2/turing_planet/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.609156 turing-planet-0.1.2/turing_planet/api/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/api/__init__.py
+-rw-rw-rw-   0        0        0     2478 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/api/planet_embedding_client.py
+-rw-rw-rw-   0        0        0     4873 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/api/planet_vector_client.py
+-rw-rw-rw-   0        0        0     8107 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/api/spark_chat_client.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.618133 turing-planet-0.1.2/turing_planet/deprecated/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/deprecated/__init__.py
+-rw-rw-rw-   0        0        0     6952 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/deprecated/spark_embedding_client.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.623120 turing-planet-0.1.2/turing_planet/langchain/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/langchain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.629103 turing-planet-0.1.2/turing_planet/langchain/chat_models/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/langchain/chat_models/__init__.py
+-rw-rw-rw-   0        0        0     8131 2024-05-31 06:03:14.000000 turing-planet-0.1.2/turing_planet/langchain/chat_models/sparkai.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.640074 turing-planet-0.1.2/turing_planet/langchain/embeddings/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/langchain/embeddings/__init__.py
+-rw-rw-rw-   0        0        0      765 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/langchain/embeddings/sparkai.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.650046 turing-planet-0.1.2/turing_planet/langchain/llm/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/langchain/llm/__init__.py
+-rw-rw-rw-   0        0        0     5350 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/langchain/llm/sparkai.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.654038 turing-planet-0.1.2/turing_planet/llama_index/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/llama_index/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.675979 turing-planet-0.1.2/turing_planet/llama_index/docqa/
+-rw-rw-rw-   0        0        0        0 2024-05-31 06:03:14.000000 turing-planet-0.1.2/turing_planet/llama_index/docqa/__init__.py
+-rw-rw-rw-   0        0        0     9736 2024-05-31 06:03:14.000000 turing-planet-0.1.2/turing_planet/llama_index/docqa/docqa_client.py
+-rw-rw-rw-   0        0        0     3111 2024-05-31 06:03:14.000000 turing-planet-0.1.2/turing_planet/llama_index/docqa/docqa_index.py
+-rw-rw-rw-   0        0        0     2608 2024-05-31 06:03:14.000000 turing-planet-0.1.2/turing_planet/llama_index/docqa/docqa_node_parser.py
+-rw-rw-rw-   0        0        0     1857 2024-05-31 06:03:14.000000 turing-planet-0.1.2/turing_planet/llama_index/docqa/docqa_retriever.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.684956 turing-planet-0.1.2/turing_planet/llama_index/embeddings/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/llama_index/embeddings/__init__.py
+-rw-rw-rw-   0        0        0     1592 2024-05-31 06:03:14.000000 turing-planet-0.1.2/turing_planet/llama_index/embeddings/sparkai.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.692933 turing-planet-0.1.2/turing_planet/llama_index/llms/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/llama_index/llms/__init__.py
+-rw-rw-rw-   0        0        0     4707 2024-05-31 06:03:14.000000 turing-planet-0.1.2/turing_planet/llama_index/llms/sparkai.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.697920 turing-planet-0.1.2/turing_planet/llama_index/readers/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/llama_index/readers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.710884 turing-planet-0.1.2/turing_planet/llama_index/readers/file/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/llama_index/readers/file/__init__.py
+-rw-rw-rw-   0        0        0     1705 2024-05-31 06:03:14.000000 turing-planet-0.1.2/turing_planet/llama_index/readers/file/excel.py
+-rw-rw-rw-   0        0        0     1190 2024-05-31 06:03:14.000000 turing-planet-0.1.2/turing_planet/llama_index/readers/file/turing_markdown_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.718863 turing-planet-0.1.2/turing_planet/llama_index/vector_stores/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/llama_index/vector_stores/__init__.py
+-rw-rw-rw-   0        0        0     3320 2024-05-31 06:03:14.000000 turing-planet-0.1.2/turing_planet/llama_index/vector_stores/planet.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.734821 turing-planet-0.1.2/turing_planet/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/utils/__init__.py
+-rw-rw-rw-   0        0        0     2102 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/utils/auth_util.py
+-rw-rw-rw-   0        0        0     1009 2024-04-18 03:49:37.000000 turing-planet-0.1.2/turing_planet/utils/env.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:03:39.740806 turing-planet-0.1.2/turing_planet.egg-info/
+-rw-rw-rw-   0        0        0     2579 2024-05-31 06:03:38.000000 turing-planet-0.1.2/turing_planet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4295 2024-05-31 06:03:38.000000 turing-planet-0.1.2/turing_planet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 06:03:38.000000 turing-planet-0.1.2/turing_planet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-31 06:03:38.000000 turing-planet-0.1.2/turing_planet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-31 06:03:38.000000 turing-planet-0.1.2/turing_planet.egg-info/top_level.txt
```

### Comparing `turing-planet-0.1.1/PKG-INFO` & `turing-planet-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turing-planet
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Extension Framework For Turing Planet
 Home-page: https://code.iflytek.com/osc/_source/Y_RDG-TURING/gpt/turing-planet/-/tree/heads%2Fdevelop
 Author: jianwu6
 Author-email: jianwu6@iflytek.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `turing-planet-0.1.1/setup.py` & `turing-planet-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('readme.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="turing-planet",
-    version="0.1.1",
+    version="0.1.2",
     author="jianwu6",
     author_email="jianwu6@iflytek.com",
     description="Python Extension Framework For Turing Planet",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://code.iflytek.com/osc/_source/Y_RDG-TURING/gpt/turing-planet/-/tree/heads%2Fdevelop",
     python_requires=">=3.9.0, <3.10.0",
```

### Comparing `turing-planet-0.1.1/test/api/sample_spark_chat_client.py` & `turing-planet-0.1.2/test/api/sample_spark_chat_client.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/api/sample_spark_embedding.py` & `turing-planet-0.1.2/test/api/sample_spark_embedding.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/agents/agent_qa.py` & `turing-planet-0.1.2/test/langchain/agents/agent_qa.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/agents/ask.py` & `turing-planet-0.1.2/test/langchain/agents/ask.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/agents/ask2.py` & `turing-planet-0.1.2/test/langchain/agents/ask2.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/agents/plan.py` & `turing-planet-0.1.2/test/langchain/agents/plan.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/agents/quick_start.py` & `turing-planet-0.1.2/test/langchain/agents/quick_start.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/agents/react.py` & `turing-planet-0.1.2/test/langchain/agents/react.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/agents/slot.py` & `turing-planet-0.1.2/test/langchain/agents/slot.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/agents/slot2.py` & `turing-planet-0.1.2/test/langchain/agents/slot2.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/agents/sparkai_agent.py` & `turing-planet-0.1.2/test/langchain/agents/sparkai_agent.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/agents/tools.py` & `turing-planet-0.1.2/test/langchain/agents/tools.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/agents.py` & `turing-planet-0.1.2/test/langchain/agents.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/chat_model.py` & `turing-planet-0.1.2/test/langchain/chat_model.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/embed.py` & `turing-planet-0.1.2/test/langchain/embed.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/function_call.py` & `turing-planet-0.1.2/test/langchain/function_call.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/function_call_aiui.py` & `turing-planet-0.1.2/test/langchain/function_call_aiui.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/llm.py` & `turing-planet-0.1.2/test/langchain/llm.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/memory.py` & `turing-planet-0.1.2/test/langchain/memory.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/langchain/retrieval.py` & `turing-planet-0.1.2/test/langchain/retrieval.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/indexing.py` & `turing-planet-0.1.2/test/llama_index/indexing.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/introduce/01_start.py` & `turing-planet-0.1.2/test/llama_index/introduce/01_start.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/introduce/02_reader.py` & `turing-planet-0.1.2/test/llama_index/introduce/02_reader.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/introduce/03_custom_file_reader.py` & `turing-planet-0.1.2/test/llama_index/introduce/03_custom_file_reader.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/introduce/04_doc_metadata.py` & `turing-planet-0.1.2/test/llama_index/introduce/04_doc_metadata.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/introduce/05_splitter.py` & `turing-planet-0.1.2/test/llama_index/introduce/05_splitter.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/introduce/06_node_metadata.py` & `turing-planet-0.1.2/test/llama_index/introduce/06_node_metadata.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/introduce/07_retriever.py` & `turing-planet-0.1.2/test/llama_index/introduce/07_retriever.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/introduce/07_retriever_custom.py` & `turing-planet-0.1.2/test/llama_index/introduce/07_retriever_custom.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/introduce/08_postprocessor.py` & `turing-planet-0.1.2/test/llama_index/introduce/08_postprocessor.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/introduce/09_prompt.py` & `turing-planet-0.1.2/test/llama_index/introduce/09_prompt.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/introduce/10_multistep_query_engine.py` & `turing-planet-0.1.2/test/llama_index/introduce/10_multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/introduce/11_route_query_engine.py` & `turing-planet-0.1.2/test/llama_index/introduce/11_route_query_engine.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/introduce/12_llamahub.py` & `turing-planet-0.1.2/test/llama_index/introduce/12_llamahub.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/introduce/introduce_base.py` & `turing-planet-0.1.2/test/llama_index/introduce/introduce_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 logging.basicConfig(
     level=logging.DEBUG,  # 设置日志级别为DEBUG，可以根据需要修改
     format="%(asctime)s - %(levelname)s - %(message)s",
 )
 # 向量特征维度
 dims = 2560
 endpoint = "172.31.164.103:9980"
-Settings.llm = SparkAI(endpoint=endpoint)
+Settings.llm = SparkAI(endpoint=endpoint, domain="generalv3.5")
 Settings.embed_model = SparkAIEmbedding(endpoint=endpoint, domain="emb_xfyun")
 Settings.chunk_size = 1024
 
 # TODO 额外参数
 vector_filter_key = "location"
 
 redis_index_schema = IndexSchema.from_dict(
```

### Comparing `turing-planet-0.1.1/test/llama_index/metadata.py` & `turing-planet-0.1.2/test/llama_index/metadata.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/optimizing/base.py` & `turing-planet-0.1.2/test/llama_index/optimizing/base.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/optimizing/custom_keyword_extractor.py` & `turing-planet-0.1.2/test/llama_index/optimizing/custom_keyword_extractor.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/optimizing/docx_keyword_vector.py` & `turing-planet-0.1.2/test/llama_index/optimizing/docx_keyword_vector.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/optimizing/qa_metadata.py` & `turing-planet-0.1.2/test/llama_index/optimizing/qa_metadata.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/optimizing/summary_index.py` & `turing-planet-0.1.2/test/llama_index/optimizing/summary_index.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/optimizing/turing_knowledge.py` & `turing-planet-0.1.2/test/llama_index/optimizing/turing_knowledge.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/optimizing/vector_index.py` & `turing-planet-0.1.2/test/llama_index/optimizing/vector_index.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/optimizing/vector_index_cq.py` & `turing-planet-0.1.2/test/llama_index/optimizing/vector_index_cq.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/pk/base.py` & `turing-planet-0.1.2/test/llama_index/pk/base.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/pk/llama_index_spark-0131.py` & `turing-planet-0.1.2/test/llama_index/pk/llama_index_spark-0131.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/pk/pk.py` & `turing-planet-0.1.2/test/llama_index/pk/pk.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/pk/pk_excel_chunsize.py` & `turing-planet-0.1.2/test/llama_index/pk/pk_excel_chunsize.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/pk/pk_excel_chunsize_rerank.py` & `turing-planet-0.1.2/test/llama_index/pk/pk_excel_chunsize_rerank.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/pk/pk_excel_embedding.py` & `turing-planet-0.1.2/test/llama_index/pk/pk_excel_embedding.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/pk/pk_word_0201.py` & `turing-planet-0.1.2/test/llama_index/pk/pk_word_0201.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/pk/pk_word_es_0201.py` & `turing-planet-0.1.2/test/llama_index/pk/pk_word_es_0201.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/pk/sample_excel.py` & `turing-planet-0.1.2/test/llama_index/pk/sample_excel.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/skydoc-embedding.py` & `turing-planet-0.1.2/test/llama_index/skydoc-embedding.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/test/llama_index/start.py` & `turing-planet-0.1.2/test/llama_index/start.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 
 from llama_index.core import ServiceContext, SimpleDirectoryReader, VectorStoreIndex, StorageContext, KnowledgeGraphIndex, \
     TreeIndex, PromptTemplate
+from llama_index.core.base.llms.types import ChatMessage, MessageRole
 from llama_index.core.graph_stores import SimpleGraphStore
 from llama_index.core.postprocessor import KeywordNodePostprocessor
 from llama_index.core.vector_stores import MetadataFilters, MetadataFilter, FilterOperator
 
 from turing_planet.llama_index.embeddings.sparkai import SparkAIEmbedding
 from turing_planet.llama_index.llms.sparkai import SparkAI
 
@@ -22,15 +23,15 @@
 # embed_model = SparkAIEmbedding(endpoint="172.31.164.103:9980")
 # embed_model = SparkAIEmbedding(endpoint="172.31.164.103:9980", domain="emb_v1")
 # 私有化2560维
 # embed_model = SparkAIEmbedding(endpoint="172.31.164.103:9980", domain="emb_v2")
 # 公有云2560维
 embed_model = SparkAIEmbedding(endpoint="172.31.164.103:9980", domain="emb_xfyun")
 
-llm = SparkAI(endpoint="172.31.164.103:9980", domain="xfyun-generalv3.5")
+llm = SparkAI(endpoint="172.31.164.103:9980")
 service_context = ServiceContext.from_defaults(embed_model=embed_model, llm=llm)
 
 # set_global_service_context(service_context)
 
 # load data
 documents = SimpleDirectoryReader("./data").load_data(show_progress=True)
 
@@ -133,11 +134,17 @@
     # query
     query_engine = index.as_query_engine()
     response = query_engine.query("半小时时长的语音会比2分钟时长的语音，提取的声纹效果好吗？")
     print(response)
 
 
 if __name__ == '__main__':
-    simple()
+    # simple()
     # graph()
     # tree()
     # post_processor()
+    # print(llm.chat(messages=[ChatMessage.from_str(content='明天天气怎么样？', role=MessageRole.USER)]))
+    chat = llm.stream_chat(messages=[ChatMessage.from_str(content='我的名字叫姚明，但是我不会打篮球', role=MessageRole.USER),
+                                     ChatMessage.from_str(content='你好姚明！我能帮你做些什么', role=MessageRole.ASSISTANT),
+                                     ChatMessage.from_str(content='你知道我的名字吗？', role=MessageRole.USER), ])
+    for item in chat:
+        print(item)
```

### Comparing `turing-planet-0.1.1/turing_planet/api/planet_embedding_client.py` & `turing-planet-0.1.2/turing_planet/api/planet_embedding_client.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/turing_planet/api/planet_vector_client.py` & `turing-planet-0.1.2/turing_planet/api/planet_vector_client.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/turing_planet/api/spark_chat_client.py` & `turing-planet-0.1.2/turing_planet/api/spark_chat_client.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/turing_planet/deprecated/spark_embedding_client.py` & `turing-planet-0.1.2/turing_planet/deprecated/spark_embedding_client.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/turing_planet/langchain/chat_models/sparkai.py` & `turing-planet-0.1.2/turing_planet/langchain/chat_models/sparkai.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/turing_planet/langchain/embeddings/sparkai.py` & `turing-planet-0.1.2/turing_planet/langchain/embeddings/sparkai.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/turing_planet/langchain/llm/sparkai.py` & `turing-planet-0.1.2/turing_planet/langchain/llm/sparkai.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/turing_planet/llama_index/embeddings/sparkai.py` & `turing-planet-0.1.2/turing_planet/llama_index/embeddings/sparkai.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/turing_planet/llama_index/readers/file/excel.py` & `turing-planet-0.1.2/turing_planet/llama_index/readers/file/excel.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/turing_planet/llama_index/readers/file/turing_markdown_reader.py` & `turing-planet-0.1.2/turing_planet/llama_index/readers/file/turing_markdown_reader.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/turing_planet/llama_index/vector_stores/planet.py` & `turing-planet-0.1.2/turing_planet/llama_index/vector_stores/planet.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/turing_planet/utils/auth_util.py` & `turing-planet-0.1.2/turing_planet/utils/auth_util.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/turing_planet/utils/env.py` & `turing-planet-0.1.2/turing_planet/utils/env.py`

 * *Files identical despite different names*

### Comparing `turing-planet-0.1.1/turing_planet.egg-info/PKG-INFO` & `turing-planet-0.1.2/turing_planet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turing-planet
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python Extension Framework For Turing Planet
 Home-page: https://code.iflytek.com/osc/_source/Y_RDG-TURING/gpt/turing-planet/-/tree/heads%2Fdevelop
 Author: jianwu6
 Author-email: jianwu6@iflytek.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `turing-planet-0.1.1/turing_planet.egg-info/SOURCES.txt` & `turing-planet-0.1.2/turing_planet.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,18 @@
 test/llama_index/introduce/07_retriever.py
 test/llama_index/introduce/07_retriever_custom.py
 test/llama_index/introduce/08_postprocessor.py
 test/llama_index/introduce/09_prompt.py
 test/llama_index/introduce/10_multistep_query_engine.py
 test/llama_index/introduce/11_route_query_engine.py
 test/llama_index/introduce/12_llamahub.py
+test/llama_index/introduce/13_docqa_split.py
+test/llama_index/introduce/14_docqa_index.py
+test/llama_index/introduce/15_docqa_retriever.py
+test/llama_index/introduce/16_docstore.py
 test/llama_index/introduce/__init__.py
 test/llama_index/introduce/introduce_base.py
 test/llama_index/introduce/nltk_demo.py
 test/llama_index/optimizing/__init__.py
 test/llama_index/optimizing/base.py
 test/llama_index/optimizing/custom_keyword_extractor.py
 test/llama_index/optimizing/docx_keyword_vector.py
@@ -82,14 +86,19 @@
 turing_planet/langchain/chat_models/__init__.py
 turing_planet/langchain/chat_models/sparkai.py
 turing_planet/langchain/embeddings/__init__.py
 turing_planet/langchain/embeddings/sparkai.py
 turing_planet/langchain/llm/__init__.py
 turing_planet/langchain/llm/sparkai.py
 turing_planet/llama_index/__init__.py
+turing_planet/llama_index/docqa/__init__.py
+turing_planet/llama_index/docqa/docqa_client.py
+turing_planet/llama_index/docqa/docqa_index.py
+turing_planet/llama_index/docqa/docqa_node_parser.py
+turing_planet/llama_index/docqa/docqa_retriever.py
 turing_planet/llama_index/embeddings/__init__.py
 turing_planet/llama_index/embeddings/sparkai.py
 turing_planet/llama_index/llms/__init__.py
 turing_planet/llama_index/llms/sparkai.py
 turing_planet/llama_index/readers/__init__.py
 turing_planet/llama_index/readers/file/__init__.py
 turing_planet/llama_index/readers/file/excel.py
```

