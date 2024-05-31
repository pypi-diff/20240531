# Comparing `tmp/llama_index_embeddings_deepinfra-0.1.0.tar.gz` & `tmp/llama_index_embeddings_deepinfra-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_deepinfra-0.1.0.tar", max compression
+gzip compressed data, was "llama_index_embeddings_deepinfra-0.1.1.tar", max compression
```

## Comparing `llama_index_embeddings_deepinfra-0.1.0.tar` & `llama_index_embeddings_deepinfra-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1506 2024-05-13 15:28:11.038066 llama_index_embeddings_deepinfra-0.1.0/README.md
--rw-r--r--   0        0        0       17 2024-05-13 15:28:11.038066 llama_index_embeddings_deepinfra-0.1.0/llama_index/embeddings/deepinfra/BUILD
--rw-r--r--   0        0        0      129 2024-05-13 15:28:11.038066 llama_index_embeddings_deepinfra-0.1.0/llama_index/embeddings/deepinfra/__init__.py
--rw-r--r--   0        0        0     7468 2024-05-13 15:28:11.038066 llama_index_embeddings_deepinfra-0.1.0/llama_index/embeddings/deepinfra/base.py
--rw-r--r--   0        0        0     1222 2024-05-13 15:28:11.038066 llama_index_embeddings_deepinfra-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2111 1970-01-01 00:00:00.000000 llama_index_embeddings_deepinfra-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1506 2024-05-31 14:24:30.591321 llama_index_embeddings_deepinfra-0.1.1/README.md
+-rw-r--r--   0        0        0       17 2024-05-31 14:24:30.591321 llama_index_embeddings_deepinfra-0.1.1/llama_index/embeddings/deepinfra/BUILD
+-rw-r--r--   0        0        0      129 2024-05-31 14:24:30.591321 llama_index_embeddings_deepinfra-0.1.1/llama_index/embeddings/deepinfra/__init__.py
+-rw-r--r--   0        0        0     7468 2024-05-31 14:24:30.591321 llama_index_embeddings_deepinfra-0.1.1/llama_index/embeddings/deepinfra/base.py
+-rw-r--r--   0        0        0     1397 2024-05-31 14:24:30.591321 llama_index_embeddings_deepinfra-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2126 1970-01-01 00:00:00.000000 llama_index_embeddings_deepinfra-0.1.1/PKG-INFO
```

### Comparing `llama_index_embeddings_deepinfra-0.1.0/README.md` & `llama_index_embeddings_deepinfra-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `llama_index_embeddings_deepinfra-0.1.0/llama_index/embeddings/deepinfra/base.py` & `llama_index_embeddings_deepinfra-0.1.1/llama_index/embeddings/deepinfra/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_embeddings_deepinfra-0.1.0/pyproject.toml` & `llama_index_embeddings_deepinfra-0.1.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -3,28 +3,35 @@
 requires = ["poetry-core"]
 
 [tool.codespell]
 check-filenames = true
 check-hidden = true
 skip = "*.csv,*.html,*.json,*.jsonl,*.pdf,*.txt,*.ipynb"
 
+[tool.llamahub]
+contains_example = false
+import_path = "llama_index.embeddings.deepinfra"
+
+[tool.llamahub.class_authors]
+DeepInfraEmbeddingModel = "deepinfra"
+
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
-authors = ["Your Name <you@example.com>"]
+authors = ["Oguz Vuruskaner <oguzvuruskaner@gmail.com>"]
 description = "llama-index embeddings deepinfra integration"
 license = "MIT"
 name = "llama-index-embeddings-deepinfra"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.0"
 aiohttp = "^3.8.1"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_embeddings_deepinfra-0.1.0/PKG-INFO` & `llama_index_embeddings_deepinfra-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-deepinfra
-Version: 0.1.0
+Version: 0.1.1
 Summary: llama-index embeddings deepinfra integration
 License: MIT
-Author: Your Name
-Author-email: you@example.com
+Author: Oguz Vuruskaner
+Author-email: oguzvuruskaner@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
```

