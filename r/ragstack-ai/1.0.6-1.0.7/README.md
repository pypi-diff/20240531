# Comparing `tmp/ragstack_ai-1.0.6.tar.gz` & `tmp/ragstack_ai-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai-1.0.6.tar", max compression
+gzip compressed data, was "ragstack_ai-1.0.7.tar", max compression
```

## Comparing `ragstack_ai-1.0.6.tar` & `ragstack_ai-1.0.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3781 2024-05-24 16:54:11.689631 ragstack_ai-1.0.6/LICENSE.md
--rw-r--r--   0        0        0     2395 2024-05-24 16:54:11.689631 ragstack_ai-1.0.6/PACKAGE_README.md
--rw-r--r--   0        0        0     1812 2024-05-24 16:54:11.733631 ragstack_ai-1.0.6/pyproject.toml
--rw-r--r--   0        0        0      271 2024-05-24 16:54:11.733631 ragstack_ai-1.0.6/ragstack/__init__.py
--rw-r--r--   0        0        0     3258 1970-01-01 00:00:00.000000 ragstack_ai-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     3781 2024-05-31 11:48:13.425773 ragstack_ai-1.0.7/LICENSE.md
+-rw-r--r--   0        0        0     2395 2024-05-31 11:48:13.425773 ragstack_ai-1.0.7/PACKAGE_README.md
+-rw-r--r--   0        0        0     1812 2024-05-31 11:48:13.477774 ragstack_ai-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0      271 2024-05-31 11:48:13.477774 ragstack_ai-1.0.7/ragstack/__init__.py
+-rw-r--r--   0        0        0     3258 1970-01-01 00:00:00.000000 ragstack_ai-1.0.7/PKG-INFO
```

### Comparing `ragstack_ai-1.0.6/LICENSE.md` & `ragstack_ai-1.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ragstack_ai-1.0.6/PACKAGE_README.md` & `ragstack_ai-1.0.7/PACKAGE_README.md`

 * *Files identical despite different names*

### Comparing `ragstack_ai-1.0.6/pyproject.toml` & `ragstack_ai-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "ragstack-ai"
-version = "1.0.6"
+version = "1.0.7"
 description = "DataStax RAGStack"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "PACKAGE_README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
-ragstack-ai-langchain = { version = "1.0.6", extras = ["colbert", "google", "nvidia"] }
+ragstack-ai-langchain = { version = "1.0.7", extras = ["colbert", "google", "nvidia"] }
 ragstack-ai-llamaindex = { version = "1.0.5", extras = ["colbert", "google", "azure", "bedrock"] }
 ragstack-ai-colbert = "1.0.5"
 
 [tool.poetry.group.test.dependencies]
 ragstack-ai-langchain = { path = "libs/langchain", develop = true, extras = ["colbert", "google", "nvidia"] }
 ragstack-ai-llamaindex = { path = "libs/llamaindex", develop = true, extras = ["colbert", "google", "azure", "bedrock"] }
 ragstack-ai-colbert = { path = "libs/colbert", develop = true }
```

### Comparing `ragstack_ai-1.0.6/PKG-INFO` & `ragstack_ai-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ragstack-ai
-Version: 1.0.6
+Version: 1.0.7
 Summary: DataStax RAGStack
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ragstack-ai-colbert (==1.0.5)
-Requires-Dist: ragstack-ai-langchain[colbert,google,nvidia] (==1.0.6)
+Requires-Dist: ragstack-ai-langchain[colbert,google,nvidia] (==1.0.7)
 Requires-Dist: ragstack-ai-llamaindex[azure,bedrock,colbert,google] (==1.0.5)
 Project-URL: Documentation, https://docs.datastax.com/en/ragstack
 Project-URL: Repository, https://github.com/datastax/ragstack-ai
 Description-Content-Type: text/markdown
 
 # RAGStack
 [![Release Notes](https://img.shields.io/github/v/release/datastax/ragstack-ai.svg)](https://github.com/datastax/ragstack-ai/releases)
```

