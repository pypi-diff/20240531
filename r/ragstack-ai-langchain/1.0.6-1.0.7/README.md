# Comparing `tmp/ragstack_ai_langchain-1.0.6.tar.gz` & `tmp/ragstack_ai_langchain-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai_langchain-1.0.6.tar", max compression
+gzip compressed data, was "ragstack_ai_langchain-1.0.7.tar", max compression
```

## Comparing `ragstack_ai_langchain-1.0.6.tar` & `ragstack_ai_langchain-1.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      371 2024-05-24 16:21:53.448164 ragstack_ai_langchain-1.0.6/README.md
--rw-r--r--   0        0        0     1243 2024-05-24 16:21:53.448164 ragstack_ai_langchain-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      271 2024-05-24 16:21:53.448164 ragstack_ai_langchain-1.0.6/ragstack_langchain/__init__.py
--rw-r--r--   0        0        0      434 2024-05-24 16:21:53.448164 ragstack_ai_langchain-1.0.6/ragstack_langchain/colbert/__init__.py
--rw-r--r--   0        0        0     2715 2024-05-24 16:21:53.448164 ragstack_ai_langchain-1.0.6/ragstack_langchain/colbert/colbert_retriever.py
--rw-r--r--   0        0        0     9303 2024-05-24 16:21:53.448164 ragstack_ai_langchain-1.0.6/ragstack_langchain/colbert/colbert_vector_store.py
--rw-r--r--   0        0        0     1730 1970-01-01 00:00:00.000000 ragstack_ai_langchain-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      371 2024-05-31 10:57:45.364571 ragstack_ai_langchain-1.0.7/README.md
+-rw-r--r--   0        0        0     1243 2024-05-31 10:57:45.364571 ragstack_ai_langchain-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      271 2024-05-31 10:57:45.364571 ragstack_ai_langchain-1.0.7/ragstack_langchain/__init__.py
+-rw-r--r--   0        0        0      434 2024-05-31 10:57:45.364571 ragstack_ai_langchain-1.0.7/ragstack_langchain/colbert/__init__.py
+-rw-r--r--   0        0        0     2715 2024-05-31 10:57:45.364571 ragstack_ai_langchain-1.0.7/ragstack_langchain/colbert/colbert_retriever.py
+-rw-r--r--   0        0        0     9303 2024-05-31 10:57:45.364571 ragstack_ai_langchain-1.0.7/ragstack_langchain/colbert/colbert_vector_store.py
+-rw-r--r--   0        0        0     1730 1970-01-01 00:00:00.000000 ragstack_ai_langchain-1.0.7/PKG-INFO
```

### Comparing `ragstack_ai_langchain-1.0.6/pyproject.toml` & `ragstack_ai_langchain-1.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ragstack-ai-langchain"
-version = "1.0.6"
+version = "1.0.7"
 description = "DataStax RAGStack Langchain"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack_langchain" }]
@@ -16,15 +16,15 @@
 unstructured = "0.14.2"
 ragstack-ai-colbert = "1.0.5"
 
 # langchain
 langchain = "0.1.19"
 langchain-core = "0.1.52"
 langchain-community = "0.0.38"
-langchain-astradb = "0.3.0"
+langchain-astradb = "0.3.3"
 langchain-openai = "0.1.3"
 langchain-google-genai = { version = "0.0.11", optional = true }
 langchain-google-vertexai = { version = "1.0.1", optional = true }
 langchain-nvidia-ai-endpoints = { version = "0.0.9", optional = true }
 
 [tool.poetry.extras]
 colbert = ["ragstack-ai-colbert"]
```

### Comparing `ragstack_ai_langchain-1.0.6/ragstack_langchain/colbert/colbert_retriever.py` & `ragstack_ai_langchain-1.0.7/ragstack_langchain/colbert/colbert_retriever.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_langchain-1.0.6/ragstack_langchain/colbert/colbert_vector_store.py` & `ragstack_ai_langchain-1.0.7/ragstack_langchain/colbert/colbert_vector_store.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_langchain-1.0.6/PKG-INFO` & `ragstack_ai_langchain-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragstack-ai-langchain
-Version: 1.0.6
+Version: 1.0.7
 Summary: DataStax RAGStack Langchain
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: colbert
 Provides-Extra: google
 Provides-Extra: nvidia
 Requires-Dist: astrapy (>=1,<2)
 Requires-Dist: cassio (>=0.1.4,<0.2.0)
 Requires-Dist: langchain (==0.1.19)
-Requires-Dist: langchain-astradb (==0.3.0)
+Requires-Dist: langchain-astradb (==0.3.3)
 Requires-Dist: langchain-community (==0.0.38)
 Requires-Dist: langchain-core (==0.1.52)
 Requires-Dist: langchain-google-genai (==0.0.11) ; extra == "google"
 Requires-Dist: langchain-google-vertexai (==1.0.1) ; extra == "google"
 Requires-Dist: langchain-nvidia-ai-endpoints (==0.0.9) ; extra == "nvidia"
 Requires-Dist: langchain-openai (==0.1.3)
 Requires-Dist: ragstack-ai-colbert (==1.0.5) ; extra == "colbert"
```

