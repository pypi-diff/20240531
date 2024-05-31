# Comparing `tmp/llama_index_graph_stores_nebula-0.1.3.tar.gz` & `tmp/llama_index_graph_stores_nebula-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_graph_stores_nebula-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_graph_stores_nebula-0.2.0.tar", max compression
```

## Comparing `llama_index_graph_stores_nebula-0.1.3.tar` & `llama_index_graph_stores_nebula-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0       46 2024-05-22 04:36:10.141452 llama_index_graph_stores_nebula-0.1.3/README.md
--rw-r--r--   0        0        0       98 2024-05-22 04:36:10.141452 llama_index_graph_stores_nebula-0.1.3/llama_index/graph_stores/nebula/__init__.py
--rw-r--r--   0        0        0    25688 2024-05-22 04:36:10.141452 llama_index_graph_stores_nebula-0.1.3/llama_index/graph_stores/nebula/base.py
--rw-r--r--   0        0        0     1481 2024-05-22 04:36:10.141452 llama_index_graph_stores_nebula-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 llama_index_graph_stores_nebula-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-05-31 17:47:32.534486 llama_index_graph_stores_nebula-0.2.0/README.md
+-rw-r--r--   0        0        0      240 2024-05-31 17:47:32.534486 llama_index_graph_stores_nebula-0.2.0/llama_index/graph_stores/nebula/__init__.py
+-rw-r--r--   0        0        0    25688 2024-05-31 17:47:32.534486 llama_index_graph_stores_nebula-0.2.0/llama_index/graph_stores/nebula/nebula_graph_store.py
+-rw-r--r--   0        0        0    30276 2024-05-31 17:47:32.534486 llama_index_graph_stores_nebula-0.2.0/llama_index/graph_stores/nebula/nebula_property_graph.py
+-rw-r--r--   0        0        0    10859 2024-05-31 17:47:32.534486 llama_index_graph_stores_nebula-0.2.0/llama_index/graph_stores/nebula/utils.py
+-rw-r--r--   0        0        0     1489 2024-05-31 17:47:32.534486 llama_index_graph_stores_nebula-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 llama_index_graph_stores_nebula-0.2.0/PKG-INFO
```

### Comparing `llama_index_graph_stores_nebula-0.1.3/llama_index/graph_stores/nebula/base.py` & `llama_index_graph_stores_nebula-0.2.0/llama_index/graph_stores/nebula/nebula_graph_store.py`

 * *Files identical despite different names*

### Comparing `llama_index_graph_stores_nebula-0.1.3/pyproject.toml` & `llama_index_graph_stores_nebula-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -20,23 +20,23 @@
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index graph stores nebula integration"
 exclude = ["**/BUILD"]
-license = "MIT"
+license = "Apache-2.0"
 name = "llama-index-graph-stores-nebula"
 readme = "README.md"
-version = "0.1.3"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.1"
-nebula3-python = "^3.4.0"
+llama-index-core = "^0.10.40"
+nebula3-python = "^3.8.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_graph_stores_nebula-0.1.3/PKG-INFO` & `llama_index_graph_stores_nebula-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-graph-stores-nebula
-Version: 0.1.3
+Version: 0.2.0
 Summary: llama-index graph stores nebula integration
-License: MIT
+License: Apache-2.0
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
-Requires-Dist: nebula3-python (>=3.4.0,<4.0.0)
+Requires-Dist: llama-index-core (>=0.10.40,<0.11.0)
+Requires-Dist: nebula3-python (>=3.8.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Graph Stores Integration: Nebula
```

