# Comparing `tmp/llama_index_postprocessor_cohere_rerank-0.1.6.tar.gz` & `tmp/llama_index_postprocessor_cohere_rerank-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_postprocessor_cohere_rerank-0.1.6.tar", max compression
+gzip compressed data, was "llama_index_postprocessor_cohere_rerank-0.1.7.tar", max compression
```

## Comparing `llama_index_postprocessor_cohere_rerank-0.1.6.tar` & `llama_index_postprocessor_cohere_rerank-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       54 2024-05-13 21:57:40.363680 llama_index_postprocessor_cohere_rerank-0.1.6/README.md
--rw-r--r--   0        0        0       98 2024-05-13 21:57:40.363680 llama_index_postprocessor_cohere_rerank-0.1.6/llama_index/postprocessor/cohere_rerank/__init__.py
--rw-r--r--   0        0        0     3168 2024-05-13 21:57:40.363680 llama_index_postprocessor_cohere_rerank-0.1.6/llama_index/postprocessor/cohere_rerank/base.py
--rw-r--r--   0        0        0     1494 2024-05-13 21:57:40.363680 llama_index_postprocessor_cohere_rerank-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 llama_index_postprocessor_cohere_rerank-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       54 2024-05-31 04:53:38.131158 llama_index_postprocessor_cohere_rerank-0.1.7/README.md
+-rw-r--r--   0        0        0       98 2024-05-31 04:53:38.131158 llama_index_postprocessor_cohere_rerank-0.1.7/llama_index/postprocessor/cohere_rerank/__init__.py
+-rw-r--r--   0        0        0     3115 2024-05-31 04:53:38.131158 llama_index_postprocessor_cohere_rerank-0.1.7/llama_index/postprocessor/cohere_rerank/base.py
+-rw-r--r--   0        0        0     1494 2024-05-31 04:53:38.131158 llama_index_postprocessor_cohere_rerank-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 llama_index_postprocessor_cohere_rerank-0.1.7/PKG-INFO
```

### Comparing `llama_index_postprocessor_cohere_rerank-0.1.6/llama_index/postprocessor/cohere_rerank/base.py` & `llama_index_postprocessor_cohere_rerank-0.1.7/llama_index/postprocessor/cohere_rerank/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,16 +48,15 @@
         return "CohereRerank"
 
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
@@ -88,9 +87,9 @@
             for result in results.results:
                 new_node_with_score = NodeWithScore(
                     node=nodes[result.index].node, score=result.relevance_score
                 )
                 new_nodes.append(new_node_with_score)
             event.on_end(payload={EventPayload.NODES: new_nodes})
 
-        dispatch_event(ReRankEndEvent(nodes=new_nodes))
+        dispatcher.event(ReRankEndEvent(nodes=new_nodes))
         return new_nodes
```

### Comparing `llama_index_postprocessor_cohere_rerank-0.1.6/pyproject.toml` & `llama_index_postprocessor_cohere_rerank-0.1.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index postprocessor cohere rerank integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-postprocessor-cohere-rerank"
 readme = "README.md"
-version = "0.1.6"
+version = "0.1.7"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.35"
+llama-index-core = "^0.10.41"
 cohere = "^5.1.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
```

### Comparing `llama_index_postprocessor_cohere_rerank-0.1.6/PKG-INFO` & `llama_index_postprocessor_cohere_rerank-0.1.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-postprocessor-cohere-rerank
-Version: 0.1.6
+Version: 0.1.7
 Summary: llama-index postprocessor cohere rerank integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cohere (>=5.1.1,<6.0.0)
-Requires-Dist: llama-index-core (>=0.10.35,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.41,<0.11.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Postprocessor Integration: Cohere Rerank
```

