# Comparing `tmp/ragstack_ai_langflow-0.0.4.tar.gz` & `tmp/ragstack_ai_langflow-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai_langflow-0.0.4.tar", max compression
+gzip compressed data, was "ragstack_ai_langflow-0.0.5.tar", max compression
```

## Comparing `ragstack_ai_langflow-0.0.4.tar` & `ragstack_ai_langflow-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3781 2024-05-30 16:46:52.206314 ragstack_ai_langflow-0.0.4/LICENSE.md
--rw-r--r--   0        0        0      286 2024-05-30 16:46:52.206314 ragstack_ai_langflow-0.0.4/README.md
--rw-r--r--   0        0        0     3839 2024-05-30 16:47:21.134339 ragstack_ai_langflow-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       63 2024-05-30 16:46:52.690314 ragstack_ai_langflow-0.0.4/src/backend/langflow/version/__init__.py
--rw-r--r--   0        0        0      339 2024-05-30 16:46:52.690314 ragstack_ai_langflow-0.0.4/src/backend/langflow/version/version.py
--rw-r--r--   0        0        0     3542 1970-01-01 00:00:00.000000 ragstack_ai_langflow-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3781 2024-05-30 20:48:33.230551 ragstack_ai_langflow-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0      286 2024-05-30 20:48:33.230551 ragstack_ai_langflow-0.0.5/README.md
+-rw-r--r--   0        0        0     3839 2024-05-30 20:49:01.402521 ragstack_ai_langflow-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       63 2024-05-30 20:48:33.714551 ragstack_ai_langflow-0.0.5/src/backend/langflow/version/__init__.py
+-rw-r--r--   0        0        0      339 2024-05-30 20:48:33.714551 ragstack_ai_langflow-0.0.5/src/backend/langflow/version/version.py
+-rw-r--r--   0        0        0     3542 1970-01-01 00:00:00.000000 ragstack_ai_langflow-0.0.5/PKG-INFO
```

### Comparing `ragstack_ai_langflow-0.0.4/LICENSE.md` & `ragstack_ai_langflow-0.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ragstack_ai_langflow-0.0.4/pyproject.toml` & `ragstack_ai_langflow-0.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ragstack-ai-langflow"
-version = "0.0.4"
+version = "0.0.5"
 description = "RAGStack Langflow"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 repository = "https://github.com/datastax/ragstack-ai-langflow"
 readme = "README.md"
 keywords = ["nlp", "langchain", "openai", "gpt", "gui"]
 packages = [{ include = "langflow", from = "src/backend" }]
@@ -13,15 +13,15 @@
 
 [tool.poetry.scripts]
 langflow = "langflow.__main__:main"
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
-ragstack-ai-langflow-base = "0.0.3"
+ragstack-ai-langflow-base = "0.0.5"
 beautifulsoup4 = "^4.12.2"
 google-search-results = "^2.4.1"
 google-api-python-client = "^2.118.0"
 huggingface-hub = { version = "^0.20.0", extras = ["inference"] }
 llama-cpp-python = { version = "~0.2.0", optional = true }
 networkx = "^3.1"
 pysrt = "^1.1.2"
@@ -71,15 +71,15 @@
 langchain-google-vertexai = "^1.0.1"
 langchain-groq = "^0.1.3"
 langchain-pinecone = "^0.1.0"
 langchain-mistralai ="^0.1.6"
 
 
 [tool.poetry.group.test.dependencies]
-ragstack-ai-langflow-base = "^0.0.3"
+ragstack-ai-langflow-base = "^0.0.5"
 
 
 [tool.poetry.group.dev.dependencies]
 types-redis = "^4.6.0.5"
 ipykernel = "^6.29.0"
 mypy = "^1.9.0"
 ruff = "^0.3.5"
```

### Comparing `ragstack_ai_langflow-0.0.4/PKG-INFO` & `ragstack_ai_langflow-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragstack-ai-langflow
-Version: 0.0.4
+Version: 0.0.5
 Summary: RAGStack Langflow
 Home-page: https://github.com/datastax/ragstack-ai-langflow
 License: BUSL-1.1
 Keywords: nlp,langchain,openai,gpt,gui
 Author: DataStax
 Requires-Python: >=3.10,<3.12
 Classifier: License :: Other/Proprietary License
@@ -55,15 +55,15 @@
 Requires-Dist: pyautogen (>=0.2.0,<0.3.0)
 Requires-Dist: pymongo (>=4.6.0,<5.0.0)
 Requires-Dist: pysrt (>=1.1.2,<2.0.0)
 Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Requires-Dist: pywin32 (>=306,<307) ; sys_platform == "win32"
 Requires-Dist: qdrant-client (>=1.7.0,<2.0.0)
 Requires-Dist: qianfan (==0.3.5)
-Requires-Dist: ragstack-ai-langflow-base (==0.0.3)
+Requires-Dist: ragstack-ai-langflow-base (==0.0.5)
 Requires-Dist: redis (>=5.0.1,<6.0.0) ; extra == "deploy"
 Requires-Dist: sentence-transformers (>=2.3.1,<3.0.0) ; extra == "local"
 Requires-Dist: supabase (>=2.3.0,<3.0.0)
 Requires-Dist: types-cachetools (>=5.3.0.5,<6.0.0.0)
 Requires-Dist: weaviate-client
 Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
 Requires-Dist: zep-python (>=2.0.0rc5,<3.0.0)
```

