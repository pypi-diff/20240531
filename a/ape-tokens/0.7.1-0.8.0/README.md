# Comparing `tmp/ape-tokens-0.7.1.tar.gz` & `tmp/ape-tokens-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-tokens-0.7.1.tar", last modified: Fri Feb  2 22:50:00 2024, max compression
+gzip compressed data, was "ape-tokens-0.8.0.tar", last modified: Fri May 31 21:53:20 2024, max compression
```

## Comparing `ape-tokens-0.7.1.tar` & `ape-tokens-0.8.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:50:00.906854 ape-tokens-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:50:00.902854 ape-tokens-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:50:00.902854 ape-tokens-0.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:50:00.902854 ape-tokens-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-02-02 22:50:00.906854 ape-tokens-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:50:00.902854 ape-tokens-0.7.1/ape_tokens/
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/ape_tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/ape_tokens/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/ape_tokens/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/ape_tokens/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/ape_tokens/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-02 22:50:00.000000 ape-tokens-0.7.1/ape_tokens/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:50:00.902854 ape-tokens-0.7.1/ape_tokens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-02-02 22:50:00.000000 ape-tokens-0.7.1/ape_tokens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-02 22:50:00.000000 ape-tokens-0.7.1/ape_tokens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 22:50:00.000000 ape-tokens-0.7.1/ape_tokens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-02 22:50:00.000000 ape-tokens-0.7.1/ape_tokens.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-02 22:50:00.000000 ape-tokens-0.7.1/ape_tokens.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-02 22:50:00.000000 ape-tokens-0.7.1/ape_tokens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-02 22:50:00.000000 ape-tokens-0.7.1/ape_tokens.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-02 22:50:00.906854 ape-tokens-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-02 22:50:00.902854 ape-tokens-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-02 22:49:06.000000 ape-tokens-0.7.1/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:53:20.155982 ape-tokens-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:53:20.155982 ape-tokens-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:53:20.155982 ape-tokens-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:53:20.155982 ape-tokens-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-31 21:53:20.155982 ape-tokens-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:53:20.155982 ape-tokens-0.8.0/ape_tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/ape_tokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/ape_tokens/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/ape_tokens/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/ape_tokens/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/ape_tokens/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 21:53:19.000000 ape-tokens-0.8.0/ape_tokens/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:53:20.155982 ape-tokens-0.8.0/ape_tokens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-31 21:53:20.000000 ape-tokens-0.8.0/ape_tokens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-31 21:53:20.000000 ape-tokens-0.8.0/ape_tokens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 21:53:20.000000 ape-tokens-0.8.0/ape_tokens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-31 21:53:20.000000 ape-tokens-0.8.0/ape_tokens.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 21:53:20.000000 ape-tokens-0.8.0/ape_tokens.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-31 21:53:20.000000 ape-tokens-0.8.0/ape_tokens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 21:53:20.000000 ape-tokens-0.8.0/ape_tokens.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-31 21:53:20.155982 ape-tokens-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3377 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:53:20.155982 ape-tokens-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-31 21:52:29.000000 ape-tokens-0.8.0/tests/test_integration.py
```

### Comparing `ape-tokens-0.7.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-tokens-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.7.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-tokens-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.7.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-tokens-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.7.1/.github/release-drafter.yml` & `ape-tokens-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.7.1/.github/workflows/commit.yaml` & `ape-tokens-0.8.0/.github/workflows/commit.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # NOTE: Skip check on PR so as not to confuse contributors
 # NOTE: Also install a PR title checker so we don't mess up merges
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
           with:
               fetch-depth: 0
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check commit history
```

### Comparing `ape-tokens-0.7.1/.github/workflows/prtitle.yaml` & `ape-tokens-0.8.0/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
       - synchronize
 
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
```

### Comparing `ape-tokens-0.7.1/.github/workflows/publish.yaml` & `ape-tokens-0.8.0/.github/workflows/publish.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
```

### Comparing `ape-tokens-0.7.1/.github/workflows/test.yaml` & `ape-tokens-0.8.0/.github/workflows/test.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -10,18 +10,18 @@
   cancel-in-progress: true
 
 jobs:
     linting:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
@@ -38,18 +38,18 @@
         - name: Run mdformat
           run: mdformat . --check
 
     type-check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
@@ -58,22 +58,24 @@
           run: mypy .
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
-                os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10", "3.11"]
+                # TODO: Replace with macos-latest when works again.
+                #   https://github.com/actions/setup-python/issues/808
+                os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
+                python-version: [3.9, "3.10", "3.11", "3.12"]
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: ${{ matrix.python-version }}
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[test]
@@ -85,18 +87,18 @@
 #    fuzzing:
 #        runs-on: ubuntu-latest
 #
 #        strategy:
 #            fail-fast: true
 #
 #        steps:
-#        - uses: actions/checkout@v3
+#        - uses: actions/checkout@v4
 #
 #        - name: Setup Python
-#          uses: actions/setup-python@v4
+#          uses: actions/setup-python@v5
 #          with:
 #              python-version: "3.10"
 #
 #        - name: Install Dependencies
 #          run: pip install .[test]
 #
 #        - name: Run Tests
```

### Comparing `ape-tokens-0.7.1/.gitignore` & `ape-tokens-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.7.1/.pre-commit-config.yaml` & `ape-tokens-0.8.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: check-yaml
 
--   repo: https://github.com/pre-commit/mirrors-isort
-    rev: v5.10.1
+-   repo: https://github.com/PyCQA/isort
+    rev: 5.13.2
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 23.12.0
+    rev: 24.4.2
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.7.1
+    rev: v1.10.0
     hooks:
     -   id: mypy
         additional_dependencies: [types-setuptools, pydantic]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
     -   id: mdformat
-        additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
+        additional_dependencies: [mdformat-gfm, mdformat-frontmatter, mdformat-pyproject]
 
 default_language_version:
     python: python3
```

### Comparing `ape-tokens-0.7.1/LICENSE` & `ape-tokens-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.7.1/PKG-INFO` & `ape-tokens-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: ape-tokens
-Version: 0.7.1
+Version: 0.8.0
 Summary: ape-tokens: tokenlists plugin for Ape
 Home-page: https://github.com/ApeWorX/ape-tokens
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 A series of utilities for working with tokens, based on the [`py-tokenlists`](https://github.com/ApeWorX/py-tokenlists).
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-tokens-0.7.1/README.md` & `ape-tokens-0.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 A series of utilities for working with tokens, based on the [`py-tokenlists`](https://github.com/ApeWorX/py-tokenlists).
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-tokens-0.7.1/ape_tokens/converters.py` & `ape-tokens-0.8.0/ape_tokens/converters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from collections.abc import Iterator
 from decimal import Decimal
-from typing import Any, Iterator
+from typing import Any
 
 from ape.api import ConverterAPI
 from ape.exceptions import ConversionError, ProviderNotConnectedError
 from ape.logging import logger
 from ape.types import AddressType
 from ape.utils import cached_property
 from tokenlists import TokenInfo, TokenListManager
```

### Comparing `ape-tokens-0.7.1/ape_tokens/managers.py` & `ape-tokens-0.8.0/ape_tokens/managers.py`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.7.1/ape_tokens.egg-info/PKG-INFO` & `ape-tokens-0.8.0/ape_tokens.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: ape-tokens
-Version: 0.7.1
+Version: 0.8.0
 Summary: ape-tokens: tokenlists plugin for Ape
 Home-page: https://github.com/ApeWorX/ape-tokens
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 A series of utilities for working with tokens, based on the [`py-tokenlists`](https://github.com/ApeWorX/py-tokenlists).
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-tokens-0.7.1/ape_tokens.egg-info/SOURCES.txt` & `ape-tokens-0.8.0/ape_tokens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-tokens-0.7.1/ape_tokens.egg-info/requires.txt` & `ape-tokens-0.8.0/ape_tokens.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-eth-ape<0.8,>=0.7.0
+eth-ape<0.9,>=0.8.1
 tokenlists>=0.1.7
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
-flake8<7,>=6.1.0
-isort<6,>=5.10.1
+flake8<8,>=7.0.0
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
@@ -30,19 +30,19 @@
 
 [doc]
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
 
 [lint]
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
-flake8<7,>=6.1.0
-isort<6,>=5.10.1
+flake8<8,>=7.0.0
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 
 [release]
 setuptools
```

### Comparing `ape-tokens-0.7.1/pyproject.toml` & `ape-tokens-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311']
+target-version = ['py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ape-tokens-0.7.1/setup.py` & `ape-tokens-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 from setuptools import find_packages, setup
 
 extras_require = {
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # Multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=23.12.0,<24",  # Auto-formatter and linter
-        "mypy>=1.7.1,<2",  # Static type analyzer
+        "black>=24.4.2,<25",  # Auto-formatter and linter
+        "mypy>=1.10.0,<2",  # Static type analyzer
         "types-setuptools",  # Needed for mypy type shed
-        "flake8>=6.1.0,<7",  # Style linter
-        "isort>=5.10.1,<6",  # Import sorting linter
+        "flake8>=7.0.0,<8",  # Style linter
+        "isort>=5.13.2,<6",  # Import sorting linter
         "mdformat>=0.7.17",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
         "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
     ],
     "doc": [
         "Sphinx>=6.1.3,<7",  # Documentation generator
@@ -59,17 +58,17 @@
     description="ape-tokens: tokenlists plugin for Ape",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-tokens",
     include_package_data=True,
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     install_requires=[
-        "eth-ape>=0.7.0,<0.8",
+        "eth-ape>=0.8.1,<0.9",
         "tokenlists>=0.1.7",
     ],
     entry_points={
         "ape_cli_subcommands": [
             "ape_tokens=ape_tokens._cli:cli",
         ],
     },
@@ -84,13 +83,13 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

