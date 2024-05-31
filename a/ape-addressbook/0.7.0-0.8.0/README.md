# Comparing `tmp/ape-addressbook-0.7.0.tar.gz` & `tmp/ape-addressbook-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-addressbook-0.7.0.tar", last modified: Tue Dec 19 05:09:36 2023, max compression
+gzip compressed data, was "ape-addressbook-0.8.0.tar", last modified: Fri May 31 21:23:29 2024, max compression
```

## Comparing `ape-addressbook-0.7.0.tar` & `ape-addressbook-0.8.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 05:09:36.656490 ape-addressbook-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 05:09:36.656490 ape-addressbook-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 05:09:36.656490 ape-addressbook-0.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 05:09:36.656490 ape-addressbook-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-12-19 05:09:36.656490 ape-addressbook-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      997 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 05:09:36.656490 ape-addressbook-0.7.0/ape_addressbook/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/ape_addressbook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/ape_addressbook/addressbook.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/ape_addressbook/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/ape_addressbook/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-19 05:09:36.000000 ape-addressbook-0.7.0/ape_addressbook/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 05:09:36.656490 ape-addressbook-0.7.0/ape_addressbook.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-12-19 05:09:36.000000 ape-addressbook-0.7.0/ape_addressbook.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-19 05:09:36.000000 ape-addressbook-0.7.0/ape_addressbook.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 05:09:36.000000 ape-addressbook-0.7.0/ape_addressbook.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 05:09:36.000000 ape-addressbook-0.7.0/ape_addressbook.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-12-19 05:09:36.000000 ape-addressbook-0.7.0/ape_addressbook.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-19 05:09:36.000000 ape-addressbook-0.7.0/ape_addressbook.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-19 05:09:36.656490 ape-addressbook-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 05:09:36.656490 ape-addressbook-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-12-19 05:08:44.000000 ape-addressbook-0.7.0/tests/test_addressbook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:23:29.320218 ape-addressbook-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:23:29.316218 ape-addressbook-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:23:29.316218 ape-addressbook-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:23:29.316218 ape-addressbook-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-31 21:23:29.320218 ape-addressbook-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:23:29.320218 ape-addressbook-0.8.0/ape_addressbook/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/ape_addressbook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/ape_addressbook/addressbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/ape_addressbook/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/ape_addressbook/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 21:23:29.000000 ape-addressbook-0.8.0/ape_addressbook/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:23:29.320218 ape-addressbook-0.8.0/ape_addressbook.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-31 21:23:29.000000 ape-addressbook-0.8.0/ape_addressbook.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-31 21:23:29.000000 ape-addressbook-0.8.0/ape_addressbook.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 21:23:29.000000 ape-addressbook-0.8.0/ape_addressbook.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 21:23:29.000000 ape-addressbook-0.8.0/ape_addressbook.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-31 21:23:29.000000 ape-addressbook-0.8.0/ape_addressbook.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 21:23:29.000000 ape-addressbook-0.8.0/ape_addressbook.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-31 21:23:29.320218 ape-addressbook-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 21:23:29.320218 ape-addressbook-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-31 21:22:30.000000 ape-addressbook-0.8.0/tests/test_addressbook.py
```

### Comparing `ape-addressbook-0.7.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-addressbook-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.7.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-addressbook-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.7.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-addressbook-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.7.0/.github/release-drafter.yml` & `ape-addressbook-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.7.0/.github/workflows/commitlint.yaml` & `ape-addressbook-0.8.0/.github/workflows/commitlint.yaml`

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

### Comparing `ape-addressbook-0.7.0/.github/workflows/prtitle.yaml` & `ape-addressbook-0.8.0/.github/workflows/prtitle.yaml`

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

### Comparing `ape-addressbook-0.7.0/.github/workflows/publish.yaml` & `ape-addressbook-0.8.0/.github/workflows/publish.yaml`

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

### Comparing `ape-addressbook-0.7.0/.github/workflows/test.yaml` & `ape-addressbook-0.8.0/.github/workflows/test.yaml`

 * *Files 18% similar despite different names*

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
@@ -55,22 +55,24 @@
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
@@ -82,18 +84,18 @@
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

### Comparing `ape-addressbook-0.7.0/.gitignore` & `ape-addressbook-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.7.0/.pre-commit-config.yaml` & `ape-addressbook-0.8.0/.pre-commit-config.yaml`

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

### Comparing `ape-addressbook-0.7.0/CONTRIBUTING.md` & `ape-addressbook-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.7.0/LICENSE` & `ape-addressbook-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.7.0/PKG-INFO` & `ape-addressbook-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: ape-addressbook
-Version: 0.7.0
+Version: 0.8.0
 Summary: ape-addressbook: Ape plugin that allows tracking addresses and contracts
 Home-page: https://github.com/ApeWorX/ape-addressbook
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
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 Ape plugin that allows tracking addresses and contracts in projects and globally.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-addressbook-0.7.0/README.md` & `ape-addressbook-0.8.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ape plugin that allows tracking addresses and contracts in projects and globally.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-addressbook-0.7.0/ape_addressbook/addressbook.py` & `ape-addressbook-0.8.0/ape_addressbook/addressbook.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from typing import Dict, Iterator, cast
+from collections.abc import Iterator
+from typing import cast
 
 from ape.api import PluginConfig
 from ape.logging import logger
 from ape.types import AddressType
 from ape.utils import ManagerAccessMixin
 from eth_utils import is_checksum_address, to_checksum_address
 from pydantic import model_validator
 from pydantic_settings import SettingsConfigDict
 
 
-def _validate_entries(entries: Dict) -> Dict:
-    validated: Dict[str, AddressType] = {}
+def _validate_entries(entries: dict) -> dict:
+    validated: dict[str, AddressType] = {}
     for k, v in entries.items():
         # Attempt to handle EVM-like addresses but if it fails,
         # let it be in case it is for a more unique ecosystem.
         try:
             if not is_checksum_address(v):
                 v = to_checksum_address(v)
 
@@ -62,15 +63,15 @@
         may contain more addressbook entries.
         """
 
         config_obj = self.config_manager.get_config("addressbook")
         return cast(AddressBookConfig, config_obj)
 
     @property
-    def registry(self) -> Dict[str, AddressType]:
+    def registry(self) -> dict[str, AddressType]:
         """
         The complete registry of addresses, including both global
         and project addresses.
         """
 
         data = self.config.model_dump()
```

### Comparing `ape-addressbook-0.7.0/ape_addressbook.egg-info/PKG-INFO` & `ape-addressbook-0.8.0/ape_addressbook.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: ape-addressbook
-Version: 0.7.0
+Version: 0.8.0
 Summary: ape-addressbook: Ape plugin that allows tracking addresses and contracts
 Home-page: https://github.com/ApeWorX/ape-addressbook
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
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 Ape plugin that allows tracking addresses and contracts in projects and globally.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-addressbook-0.7.0/ape_addressbook.egg-info/SOURCES.txt` & `ape-addressbook-0.8.0/ape_addressbook.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-addressbook-0.7.0/ape_addressbook.egg-info/requires.txt` & `ape-addressbook-0.8.0/ape_addressbook.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-eth-ape<0.8,>=0.7.0
+eth-ape<0.9,>=0.8.1
 pydantic
 pydantic-settings
 
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
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 setuptools
 wheel
 twine
 commitizen
 pre-commit
 pytest-watch
 IPython
 ipdb
 
 [lint]
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 
 [release]
 setuptools
```

### Comparing `ape-addressbook-0.7.0/pyproject.toml` & `ape-addressbook-0.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
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

### Comparing `ape-addressbook-0.7.0/setup.py` & `ape-addressbook-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
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
+        "flake8>=7.0.0,<8",  # Style linter
         "flake8-breakpoint>=1.1.0,<2",  # Detect breakpoints left in code
         "flake8-print>=5.0.0,<6",  # Detect print statements left in code
-        "isort>=5.10.1,<6",  # Import sorting linter
+        "isort>=5.13.2,<6",  # Import sorting linter
         "mdformat>=0.7.17",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
         "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
     ],
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
@@ -56,19 +56,19 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-addressbook",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.0,<0.8",
+        "eth-ape>=0.8.1,<0.9",
         "pydantic",  # Use same version as eth-ape.
         "pydantic-settings",  # Use same version as eth-ape.
     ],
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["ape_addressbook"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_addressbook": ["py.typed"]},
@@ -76,13 +76,13 @@
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

### Comparing `ape-addressbook-0.7.0/tests/test_addressbook.py` & `ape-addressbook-0.8.0/tests/test_addressbook.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,40 @@
 from ape_addressbook import addressbook
 
 
-def test_config(project_alias_unchecksummed, project_alias_no_quotes, project_address):
+def test_config(project_alias_unchecksummed, project_alias_int, project_address):
     """
     This test shows that we are able to read values from a
     project's config as well as handle checksumming them if needbe.
     """
 
     actual = addressbook.config
     assert len(actual) == 2
     assert actual[project_alias_unchecksummed] == project_address
-    assert actual[project_alias_no_quotes] == project_address
+    assert actual[project_alias_int] == project_address
 
 
-def test_registry(
-    project_alias_unchecksummed,
-    project_alias_no_quotes,
-    project_address,
-):
+def test_registry(project_alias_unchecksummed, project_alias_int, project_address):
     actual = addressbook.registry
     assert len(actual) == 2
     assert actual[project_alias_unchecksummed] == project_address
-    assert actual[project_alias_no_quotes] == project_address
+    assert actual[project_alias_int] == project_address
 
 
-def test_aliases(project_alias_unchecksummed, project_alias_no_quotes):
+def test_aliases(project_alias_unchecksummed, project_alias_int):
     """
     The aliases includes both project and global addresses.
     """
 
     actual = list(addressbook.aliases)
-    expected = [project_alias_no_quotes, project_alias_unchecksummed]
+    expected = [project_alias_int, project_alias_unchecksummed]
     assert actual == expected
 
 
-def test_contains(
-    project_alias_unchecksummed,
-    project_alias_no_quotes,
-):
+def test_contains(project_alias_unchecksummed, project_alias_int):
     assert project_alias_unchecksummed in addressbook
-    assert project_alias_no_quotes in addressbook
+    assert project_alias_int in addressbook
 
 
-def test_get_item(
-    project_alias_unchecksummed,
-    project_address,
-    project_alias_no_quotes,
-):
+def test_get_item(project_alias_unchecksummed, project_address, project_alias_int):
     assert addressbook[project_alias_unchecksummed] == project_address
-    assert addressbook[project_alias_no_quotes] == project_address
+    assert addressbook[project_alias_int] == project_address
```

