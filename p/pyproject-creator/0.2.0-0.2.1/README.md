# Comparing `tmp/pyproject_creator-0.2.0.tar.gz` & `tmp/pyproject_creator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_creator-0.2.0.tar", max compression
+gzip compressed data, was "pyproject_creator-0.2.1.tar", max compression
```

## Comparing `pyproject_creator-0.2.0.tar` & `pyproject_creator-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1065 2024-05-29 08:29:46.570895 pyproject_creator-0.2.0/LICENSE
--rw-r--r--   0        0        0     2365 2024-05-29 08:29:46.570895 pyproject_creator-0.2.0/README.md
--rw-r--r--   0        0        0     2691 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/__init__.py
--rw-r--r--   0        0        0     5628 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/cli.py
--rw-r--r--   0        0        0     8420 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/.cz.toml
--rw-r--r--   0        0        0     3077 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/.gitignore
--rw-r--r--   0        0        0     2181 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1127 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/github_action/workflows/test.yml
--rw-r--r--   0        0        0        0 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/logs/__init__.py
--rw-r--r--   0        0        0     3289 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/logs/_default.py
--rw-r--r--   0        0        0     2345 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/pyproject.template
--rw-r--r--   0        0        0        0 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/scripts/__init__.py
--rw-r--r--   0        0        0      339 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/scripts/commit_with_pre_commit.py
--rw-r--r--   0        0        0        0 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/tests/__init__.py
--rw-r--r--   0        0        0       80 2024-05-29 08:29:46.574895 pyproject_creator-0.2.0/pyproject_creator/template/tests/test_sample.py
--rw-r--r--   0        0        0     2890 1970-01-01 00:00:00.000000 pyproject_creator-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2646 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/README.md
+-rw-r--r--   0        0        0     2691 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/pyproject_creator/__init__.py
+-rw-r--r--   0        0        0     5628 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/pyproject_creator/cli.py
+-rw-r--r--   0        0        0     8420 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/pyproject_creator/template/.cz.toml
+-rw-r--r--   0        0        0     3077 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/pyproject_creator/template/.gitignore
+-rw-r--r--   0        0        0     2181 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/pyproject_creator/template/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1127 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/pyproject_creator/template/github_action/workflows/test.yml
+-rw-r--r--   0        0        0        0 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/pyproject_creator/template/logs/__init__.py
+-rw-r--r--   0        0        0     3289 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/pyproject_creator/template/logs/_default.py
+-rw-r--r--   0        0        0     2345 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/pyproject_creator/template/pyproject.template
+-rw-r--r--   0        0        0        0 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/pyproject_creator/template/scripts/__init__.py
+-rw-r--r--   0        0        0      339 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/pyproject_creator/template/scripts/commit_with_pre_commit.py
+-rw-r--r--   0        0        0        0 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/pyproject_creator/template/tests/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-31 16:01:42.176536 pyproject_creator-0.2.1/pyproject_creator/template/tests/test_sample.py
+-rw-r--r--   0        0        0     3171 1970-01-01 00:00:00.000000 pyproject_creator-0.2.1/PKG-INFO
```

### Comparing `pyproject_creator-0.2.0/LICENSE` & `pyproject_creator-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject_creator-0.2.0/README.md` & `pyproject_creator-0.2.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Pyproject Creator
-![test](https://github.com/atiasn/docs/actions/workflows/test.yml/badge.svg?branch=master)
+![test](https://github.com/atiasn/pyproject-creator/actions/workflows/test.yml/badge.svg?branch=master)
+![PyPI - Version](https://img.shields.io/pypi/v/pyproject-creator)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyproject-creator)
+[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
+
 Pyproject Creator 是一个旨在简化创建 Python 项目过程的工具。它可以生成一些基础项目结构组件。
 
 基础组件：
 - Poetry 用于包管理
 - pre-commit 用于代码格式化和 linting
 - Commitizen 用于规范 git commit
```

### Comparing `pyproject_creator-0.2.0/pyproject.toml` & `pyproject_creator-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyproject-creator"
-version = "0.2.0"
+version = "0.2.1"
 description = "A tool to create Python project templates"
 authors = ["NextKele <ritboylei@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `pyproject_creator-0.2.0/pyproject_creator/cli.py` & `pyproject_creator-0.2.1/pyproject_creator/cli.py`

 * *Files identical despite different names*

### Comparing `pyproject_creator-0.2.0/pyproject_creator/template/.cz.toml` & `pyproject_creator-0.2.1/pyproject_creator/template/.cz.toml`

 * *Files identical despite different names*

### Comparing `pyproject_creator-0.2.0/pyproject_creator/template/.gitignore` & `pyproject_creator-0.2.1/pyproject_creator/template/.gitignore`

 * *Files identical despite different names*

### Comparing `pyproject_creator-0.2.0/pyproject_creator/template/.pre-commit-config.yaml` & `pyproject_creator-0.2.1/pyproject_creator/template/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyproject_creator-0.2.0/pyproject_creator/template/github_action/workflows/test.yml` & `pyproject_creator-0.2.1/pyproject_creator/template/github_action/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyproject_creator-0.2.0/pyproject_creator/template/logs/_default.py` & `pyproject_creator-0.2.1/pyproject_creator/template/logs/_default.py`

 * *Files identical despite different names*

### Comparing `pyproject_creator-0.2.0/pyproject_creator/template/pyproject.template` & `pyproject_creator-0.2.1/pyproject_creator/template/pyproject.template`

 * *Files identical despite different names*

