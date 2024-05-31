# Comparing `tmp/ragstack_ai_langflow-0.0.5.tar.gz` & `tmp/ragstack_ai_langflow-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai_langflow-0.0.5.tar", max compression
+gzip compressed data, was "ragstack_ai_langflow-0.0.7.tar", max compression
```

## Comparing `ragstack_ai_langflow-0.0.5.tar` & `ragstack_ai_langflow-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3781 2024-05-30 20:48:33.230551 ragstack_ai_langflow-0.0.5/LICENSE.md
--rw-r--r--   0        0        0      286 2024-05-30 20:48:33.230551 ragstack_ai_langflow-0.0.5/README.md
--rw-r--r--   0        0        0     3839 2024-05-30 20:49:01.402521 ragstack_ai_langflow-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       63 2024-05-30 20:48:33.714551 ragstack_ai_langflow-0.0.5/src/backend/langflow/version/__init__.py
--rw-r--r--   0        0        0      339 2024-05-30 20:48:33.714551 ragstack_ai_langflow-0.0.5/src/backend/langflow/version/version.py
--rw-r--r--   0        0        0     3542 1970-01-01 00:00:00.000000 ragstack_ai_langflow-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-31 13:25:59.298499 ragstack_ai_langflow-0.0.7/LICENSE
+-rw-r--r--   0        0        0      285 2024-05-31 13:25:59.298499 ragstack_ai_langflow-0.0.7/README.md
+-rw-r--r--   0        0        0     3979 2024-05-31 13:26:21.126326 ragstack_ai_langflow-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0       63 2024-05-31 13:25:59.986494 ragstack_ai_langflow-0.0.7/src/backend/langflow/version/__init__.py
+-rw-r--r--   0        0        0      339 2024-05-31 13:25:59.986494 ragstack_ai_langflow-0.0.7/src/backend/langflow/version/version.py
+-rw-r--r--   0        0        0     3844 1970-01-01 00:00:00.000000 ragstack_ai_langflow-0.0.7/PKG-INFO
```

### Comparing `ragstack_ai_langflow-0.0.5/pyproject.toml` & `ragstack_ai_langflow-0.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ragstack-ai-langflow"
-version = "0.0.5"
+version = "0.0.7"
 description = "RAGStack Langflow"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 repository = "https://github.com/datastax/ragstack-ai-langflow"
 readme = "README.md"
 keywords = ["nlp", "langchain", "openai", "gpt", "gui"]
 packages = [{ include = "langflow", from = "src/backend" }]
@@ -12,102 +12,105 @@
 documentation = "https://docs.datastax.com/en/ragstack"
 
 [tool.poetry.scripts]
 langflow = "langflow.__main__:main"
 
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
-ragstack-ai-langflow-base = "0.0.5"
+python = ">=3.10,<3.13"
+ragstack-ai-langflow-base = "0.0.7"
 beautifulsoup4 = "^4.12.2"
 google-search-results = "^2.4.1"
-google-api-python-client = "^2.118.0"
+google-api-python-client = "^2.130.0"
 huggingface-hub = { version = "^0.20.0", extras = ["inference"] }
 llama-cpp-python = { version = "~0.2.0", optional = true }
 networkx = "^3.1"
-pysrt = "^1.1.2"
-fake-useragent = "^1.4.0"
+fake-useragent = "^1.5.0"
 psycopg2-binary = "^2.9.6"
 pyarrow = "^14.0.0"
 wikipedia = "^1.4.0"
-qdrant-client = "^1.7.0"
+qdrant-client = "^1.9.0"
 weaviate-client = "*"
 sentence-transformers = { version = "^2.3.1", optional = true }
 ctransformers = { version = "^0.2.10", optional = true }
-cohere = "^5.1.7"
-faiss-cpu = "^1.7.4"
+cohere = "^5.5.3"
+faiss-cpu = "^1.8.0"
 types-cachetools = "^5.3.0.5"
 pinecone-client = "^3.0.3"
 pymongo = "^4.6.0"
 supabase = "^2.3.0"
 certifi = "^2023.11.17"
 psycopg = "^3.1.9"
 psycopg-binary = "^3.1.9"
 fastavro = "^1.8.0"
 celery = { extras = ["redis"], version = "^5.3.6", optional = true }
 redis = { version = "^5.0.1", optional = true }
 flower = { version = "^2.0.0", optional = true }
 metaphor-python = "^0.1.11"
 pywin32 = { version = "^306", markers = "sys_platform == 'win32'" }
-langfuse = "^2.9.0"
+langfuse = "^2.33.0"
 metal-sdk = "^2.5.0"
 markupsafe = "^2.1.3"
-extract-msg = "^0.47.0"
 # jq is not available for windows
 boto3 = "^1.34.0"
 numexpr = "^2.8.6"
 qianfan = "0.3.5"
 pgvector = "^0.2.3"
 pyautogen = "^0.2.0"
+langchain-google-genai = "^0.0.11"
 langchain-cohere = "^0.1.0rc1"
 elasticsearch = "^8.12.0"
 pytube = "^15.0.0"
 dspy-ai = "^2.4.0"
-html2text = "^2024.2.26"
-assemblyai = "^0.23.1"
-litellm = "^1.34.22"
-chromadb = "^0.4.24"
+assemblyai = "^0.26.0"
+litellm = "^1.38.0"
+chromadb = "^0.5.0"
 langchain-anthropic = "^0.1.6"
+langchain-astradb = "^0.3.0"
+langchain-openai = "^0.1.1"
 zep-python = { version = "^2.0.0rc5", allow-prereleases = true }
 langchain-google-vertexai = "^1.0.1"
 langchain-groq = "^0.1.3"
 langchain-pinecone = "^0.1.0"
-langchain-mistralai ="^0.1.6"
-
-
-[tool.poetry.group.test.dependencies]
-ragstack-ai-langflow-base = "^0.0.5"
+langchain-mistralai = "^0.1.6"
+couchbase = "^4.2.1"
+youtube-transcript-api = "^0.6.2"
+markdown = "^3.6"
+langchain-chroma = "^0.1.1"
+upstash-vector = "^0.4.0"
 
 
 [tool.poetry.group.dev.dependencies]
+ragstack-ai-langflow-base = "^0.0.7"
 types-redis = "^4.6.0.5"
 ipykernel = "^6.29.0"
-mypy = "^1.9.0"
-ruff = "^0.3.5"
+mypy = "^1.10.0"
+ruff = "^0.4.5"
 httpx = "*"
-pytest = "^8.1.0"
-types-requests = "^2.31.0"
-requests = "^2.31.0"
-pytest-cov = "^4.1.0"
+pytest = "^8.2.0"
+types-requests = "^2.32.0"
+requests = "^2.32.0"
+pytest-cov = "^5.0.0"
 pandas-stubs = "^2.1.4.231227"
 types-pillow = "^10.2.0.20240213"
 types-pyyaml = "^6.0.12.8"
 types-python-jose = "^3.3.4.8"
 types-passlib = "^1.7.7.13"
 locust = "^2.23.1"
-pytest-mock = "^3.12.0"
-pytest-xdist = "^3.5.0"
+pytest-mock = "^3.14.0"
+pytest-xdist = "^3.6.0"
 types-pywin32 = "^306.0.0.4"
 types-google-cloud-ndb = "^2.2.0.0"
 pytest-sugar = "^1.0.0"
 respx = "^0.21.1"
 pytest-instafail = "^0.5.0"
 pytest-asyncio = "^0.23.0"
 pytest-profiling = "^1.7.0"
 pre-commit = "^3.7.0"
+vulture = "^2.11"
 
 [tool.poetry.extras]
 deploy = ["celery", "redis", "flower"]
 local = ["llama-cpp-python", "sentence-transformers", "ctransformers"]
 
 
 [tool.poetry.group.spelling]
@@ -120,15 +123,15 @@
 skip = '.git,*.pdf,*.svg,*.pdf,*.yaml,*.ipynb,poetry.lock,*.min.js,*.css,package-lock.json,*.trig'
 # Ignore latin etc
 ignore-regex = '.*(Stati Uniti|Tense=Pres).*'
 
 
 [tool.pytest.ini_options]
 minversion = "6.0"
-addopts = "-ra"
+addopts = "-ra -n auto"
 testpaths = ["tests", "integration"]
 console_output_style = "progress"
 filterwarnings = ["ignore::DeprecationWarning"]
 log_cli = true
 markers = ["async_test"]
```

### Comparing `ragstack_ai_langflow-0.0.5/PKG-INFO` & `ragstack_ai_langflow-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,91 @@
 Metadata-Version: 2.1
 Name: ragstack-ai-langflow
-Version: 0.0.5
+Version: 0.0.7
 Summary: RAGStack Langflow
 Home-page: https://github.com/datastax/ragstack-ai-langflow
 License: BUSL-1.1
 Keywords: nlp,langchain,openai,gpt,gui
 Author: DataStax
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: deploy
 Provides-Extra: local
-Requires-Dist: assemblyai (>=0.23.1,<0.24.0)
+Requires-Dist: assemblyai (>=0.26.0,<0.27.0)
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: boto3 (>=1.34.0,<2.0.0)
 Requires-Dist: celery[redis] (>=5.3.6,<6.0.0) ; extra == "deploy"
 Requires-Dist: certifi (>=2023.11.17,<2024.0.0)
-Requires-Dist: chromadb (>=0.4.24,<0.5.0)
-Requires-Dist: cohere (>=5.1.7,<6.0.0)
+Requires-Dist: chromadb (>=0.5.0,<0.6.0)
+Requires-Dist: cohere (>=5.5.3,<6.0.0)
+Requires-Dist: couchbase (>=4.2.1,<5.0.0)
 Requires-Dist: ctransformers (>=0.2.10,<0.3.0) ; extra == "local"
 Requires-Dist: dspy-ai (>=2.4.0,<3.0.0)
 Requires-Dist: elasticsearch (>=8.12.0,<9.0.0)
-Requires-Dist: extract-msg (>=0.47.0,<0.48.0)
-Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
-Requires-Dist: fake-useragent (>=1.4.0,<2.0.0)
+Requires-Dist: faiss-cpu (>=1.8.0,<2.0.0)
+Requires-Dist: fake-useragent (>=1.5.0,<2.0.0)
 Requires-Dist: fastavro (>=1.8.0,<2.0.0)
 Requires-Dist: flower (>=2.0.0,<3.0.0) ; extra == "deploy"
-Requires-Dist: google-api-python-client (>=2.118.0,<3.0.0)
+Requires-Dist: google-api-python-client (>=2.130.0,<3.0.0)
 Requires-Dist: google-search-results (>=2.4.1,<3.0.0)
-Requires-Dist: html2text (>=2024.2.26,<2025.0.0)
 Requires-Dist: huggingface-hub[inference] (>=0.20.0,<0.21.0)
 Requires-Dist: langchain-anthropic (>=0.1.6,<0.2.0)
+Requires-Dist: langchain-astradb (>=0.3.0,<0.4.0)
+Requires-Dist: langchain-chroma (>=0.1.1,<0.2.0)
 Requires-Dist: langchain-cohere (>=0.1.0rc1,<0.2.0)
+Requires-Dist: langchain-google-genai (>=0.0.11,<0.0.12)
 Requires-Dist: langchain-google-vertexai (>=1.0.1,<2.0.0)
 Requires-Dist: langchain-groq (>=0.1.3,<0.2.0)
 Requires-Dist: langchain-mistralai (>=0.1.6,<0.2.0)
+Requires-Dist: langchain-openai (>=0.1.1,<0.2.0)
 Requires-Dist: langchain-pinecone (>=0.1.0,<0.2.0)
-Requires-Dist: langfuse (>=2.9.0,<3.0.0)
-Requires-Dist: litellm (>=1.34.22,<2.0.0)
+Requires-Dist: langfuse (>=2.33.0,<3.0.0)
+Requires-Dist: litellm (>=1.38.0,<2.0.0)
 Requires-Dist: llama-cpp-python (>=0.2.0,<0.3.0) ; extra == "local"
+Requires-Dist: markdown (>=3.6,<4.0)
 Requires-Dist: markupsafe (>=2.1.3,<3.0.0)
 Requires-Dist: metal-sdk (>=2.5.0,<3.0.0)
 Requires-Dist: metaphor-python (>=0.1.11,<0.2.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: numexpr (>=2.8.6,<3.0.0)
 Requires-Dist: pgvector (>=0.2.3,<0.3.0)
 Requires-Dist: pinecone-client (>=3.0.3,<4.0.0)
 Requires-Dist: psycopg (>=3.1.9,<4.0.0)
 Requires-Dist: psycopg-binary (>=3.1.9,<4.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: pyarrow (>=14.0.0,<15.0.0)
 Requires-Dist: pyautogen (>=0.2.0,<0.3.0)
 Requires-Dist: pymongo (>=4.6.0,<5.0.0)
-Requires-Dist: pysrt (>=1.1.2,<2.0.0)
 Requires-Dist: pytube (>=15.0.0,<16.0.0)
 Requires-Dist: pywin32 (>=306,<307) ; sys_platform == "win32"
-Requires-Dist: qdrant-client (>=1.7.0,<2.0.0)
+Requires-Dist: qdrant-client (>=1.9.0,<2.0.0)
 Requires-Dist: qianfan (==0.3.5)
-Requires-Dist: ragstack-ai-langflow-base (==0.0.5)
+Requires-Dist: ragstack-ai-langflow-base (==0.0.7)
 Requires-Dist: redis (>=5.0.1,<6.0.0) ; extra == "deploy"
 Requires-Dist: sentence-transformers (>=2.3.1,<3.0.0) ; extra == "local"
 Requires-Dist: supabase (>=2.3.0,<3.0.0)
 Requires-Dist: types-cachetools (>=5.3.0.5,<6.0.0.0)
+Requires-Dist: upstash-vector (>=0.4.0,<0.5.0)
 Requires-Dist: weaviate-client
 Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
+Requires-Dist: youtube-transcript-api (>=0.6.2,<0.7.0)
 Requires-Dist: zep-python (>=2.0.0rc5,<3.0.0)
 Project-URL: Documentation, https://docs.datastax.com/en/ragstack
 Project-URL: Repository, https://github.com/datastax/ragstack-ai-langflow
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD030 -->
 
 # RAGStack Langflow
 
 ## Documentation
 
-[DataStax RAGStack Documentation](https://docs.datastax.com/en/ragstack/docs/index.html) 
+[DataStax RAGStack Documentation](https://docs.datastax.com/en/ragstack/docs/index.html)
 
 ## 📄 License
 
 RAGStack Langflow is released under the BUSL License. See the [LICENSE](LICENSE.md) file for details.
```

