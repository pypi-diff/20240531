# Comparing `tmp/llama_index_postprocessor_colbert_rerank-0.1.2.tar.gz` & `tmp/llama_index_postprocessor_colbert_rerank-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_postprocessor_colbert_rerank-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_postprocessor_colbert_rerank-0.1.3.tar", max compression
```

## Comparing `llama_index_postprocessor_colbert_rerank-0.1.2.tar` & `llama_index_postprocessor_colbert_rerank-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      350 2024-05-13 21:57:40.363680 llama_index_postprocessor_colbert_rerank-0.1.2/README.md
--rw-r--r--   0        0        0      101 2024-05-13 21:57:40.363680 llama_index_postprocessor_colbert_rerank-0.1.2/llama_index/postprocessor/colbert_rerank/__init__.py
--rw-r--r--   0        0        0     4882 2024-05-13 21:57:40.363680 llama_index_postprocessor_colbert_rerank-0.1.2/llama_index/postprocessor/colbert_rerank/base.py
--rw-r--r--   0        0        0     1672 2024-05-13 21:57:40.363680 llama_index_postprocessor_colbert_rerank-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 llama_index_postprocessor_colbert_rerank-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      350 2024-05-31 04:53:38.131158 llama_index_postprocessor_colbert_rerank-0.1.3/README.md
+-rw-r--r--   0        0        0      101 2024-05-31 04:53:38.131158 llama_index_postprocessor_colbert_rerank-0.1.3/llama_index/postprocessor/colbert_rerank/__init__.py
+-rw-r--r--   0        0        0     4829 2024-05-31 04:53:38.131158 llama_index_postprocessor_colbert_rerank-0.1.3/llama_index/postprocessor/colbert_rerank/base.py
+-rw-r--r--   0        0        0     1672 2024-05-31 04:53:38.131158 llama_index_postprocessor_colbert_rerank-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1016 1970-01-01 00:00:00.000000 llama_index_postprocessor_colbert_rerank-0.1.3/PKG-INFO
```

### Comparing `llama_index_postprocessor_colbert_rerank-0.1.2/llama_index/postprocessor/colbert_rerank/base.py` & `llama_index_postprocessor_colbert_rerank-0.1.3/llama_index/postprocessor/colbert_rerank/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,16 +81,15 @@
         return rerank_score_list
 
     def _postprocess_nodes(
         self,
         nodes: List[NodeWithScore],
         query_bundle: Optional[QueryBundle] = None,
     ) -> List[NodeWithScore]:
-        dispatch_event = dispatcher.get_dispatch_event()
-        dispatch_event(
+        dispatcher.event(
             ReRankStartEvent(
                 query=query_bundle, nodes=nodes, top_n=self.top_n, model_name=self.model
             )
         )
 
         if query_bundle is None:
             raise ValueError("Missing query bundle in extra info.")
@@ -122,9 +121,9 @@
                 node.score = float(score)
 
             reranked_nodes = sorted(nodes, key=lambda x: -x.score if x.score else 0)[
                 : self.top_n
             ]
             event.on_end(payload={EventPayload.NODES: reranked_nodes})
 
-        dispatch_event(ReRankEndEvent(nodes=reranked_nodes))
+        dispatcher.event(ReRankEndEvent(nodes=reranked_nodes))
         return reranked_nodes
```

### Comparing `llama_index_postprocessor_colbert_rerank-0.1.2/pyproject.toml` & `llama_index_postprocessor_colbert_rerank-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index postprocessor colbert-rerank integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-postprocessor-colbert-rerank"
 packages = [{include = "llama_index/"}]
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.35"
+llama-index-core = "^0.10.41"
 torch = "^2.2.0"
 transformers = "^4.37.2"
 
 [tool.poetry.group.dev.dependencies]
 black = {extras = ["jupyter"], version = "<=23.9.1,>=23.7.0"}
 codespell = {extras = ["toml"], version = ">=v2.2.6"}
 ipython = "8.10.0"
```

### Comparing `llama_index_postprocessor_colbert_rerank-0.1.2/PKG-INFO` & `llama_index_postprocessor_colbert_rerank-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: llama-index-postprocessor-colbert-rerank
-Version: 0.1.2
+Version: 0.1.3
 Summary: llama-index postprocessor colbert-rerank integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: llama-index-core (>=0.10.35,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.41,<0.11.0)
 Requires-Dist: torch (>=2.2.0,<3.0.0)
 Requires-Dist: transformers (>=4.37.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Postprocessor Integration: Colbert Rerank
 
 [Colbert](https://github.com/stanford-futuredata/ColBERT): ColBERT is a fast and accurate retrieval model, enabling scalable BERT-based search over large text collections in tens of milliseconds.
```

