# Comparing `tmp/rich_structlog-0.1.0.tar.gz` & `tmp/rich_structlog-0.1.1.tar.gz`

## Comparing `rich_structlog-0.1.0.tar` & `rich_structlog-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 rich_structlog-0.1.0/README.md
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 rich_structlog-0.1.0/requirements.dev.txt
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 rich_structlog-0.1.0/requirements.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 rich_structlog-0.1.0/rich_structlog/__init__.py
--rw-r--r--   0        0        0     9575 2020-02-02 00:00:00.000000 rich_structlog-0.1.0/rich_structlog/log.py
--rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 rich_structlog-0.1.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 rich_structlog-0.1.0/LICENSE
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 rich_structlog-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 rich_structlog-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 rich_structlog-0.1.1/requirements.dev.txt
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 rich_structlog-0.1.1/requirements.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 rich_structlog-0.1.1/rich_structlog/__init__.py
+-rw-r--r--   0        0        0     9575 2020-02-02 00:00:00.000000 rich_structlog-0.1.1/rich_structlog/log.py
+-rw-r--r--   0        0        0     3139 2020-02-02 00:00:00.000000 rich_structlog-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 rich_structlog-0.1.1/LICENSE
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 rich_structlog-0.1.1/README.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 rich_structlog-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 rich_structlog-0.1.1/PKG-INFO
```

### Comparing `rich_structlog-0.1.0/rich_structlog/log.py` & `rich_structlog-0.1.1/rich_structlog/log.py`

 * *Files identical despite different names*

### Comparing `rich_structlog-0.1.0/.gitignore` & `rich_structlog-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rich_structlog-0.1.0/LICENSE` & `rich_structlog-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rich_structlog-0.1.0/pyproject.toml` & `rich_structlog-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 [project]
 name = "rich-structlog"
 dynamic = ["version", "dependencies", "optional-dependencies"]
 authors = [{ name = "Khaled Sakallah", email = "ks.dev@posteo.de" }]
 requires-python = ">=3.10"
 license = { text = "MIT" }
+readme = "README.md"
 
 [tool.hatch.version]
 source = "vcs"
 
 [tool.hatch.metadata]
 allow-direct-references = true
```

