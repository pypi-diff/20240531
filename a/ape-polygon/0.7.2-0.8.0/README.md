# Comparing `tmp/ape-polygon-0.7.2.tar.gz` & `tmp/ape-polygon-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-polygon-0.7.2.tar", last modified: Thu Mar 28 17:49:46 2024, max compression
+gzip compressed data, was "ape-polygon-0.8.0.tar", last modified: Fri May 31 19:30:07 2024, max compression
```

## Comparing `ape-polygon-0.7.2.tar` & `ape-polygon-0.8.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:49:46.935617 ape-polygon-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:49:46.931617 ape-polygon-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:49:46.931617 ape-polygon-0.7.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:49:46.931617 ape-polygon-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-28 17:49:46.935617 ape-polygon-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:49:46.931617 ape-polygon-0.7.2/ape_polygon/
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/ape_polygon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/ape_polygon/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/ape_polygon/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-28 17:49:46.000000 ape-polygon-0.7.2/ape_polygon/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:49:46.931617 ape-polygon-0.7.2/ape_polygon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-28 17:49:46.000000 ape-polygon-0.7.2/ape_polygon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-28 17:49:46.000000 ape-polygon-0.7.2/ape_polygon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:49:46.000000 ape-polygon-0.7.2/ape_polygon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:49:46.000000 ape-polygon-0.7.2/ape_polygon.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-28 17:49:46.000000 ape-polygon-0.7.2/ape_polygon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-28 17:49:46.000000 ape-polygon-0.7.2/ape_polygon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-28 17:49:46.935617 ape-polygon-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:49:46.935617 ape-polygon-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/tests/test_ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-28 17:48:15.000000 ape-polygon-0.7.2/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:30:07.233206 ape-polygon-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:30:07.229206 ape-polygon-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:30:07.229206 ape-polygon-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:30:07.233206 ape-polygon-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-31 19:30:07.233206 ape-polygon-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:30:07.233206 ape-polygon-0.8.0/ape_polygon/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/ape_polygon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/ape_polygon/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/ape_polygon/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 19:30:06.000000 ape-polygon-0.8.0/ape_polygon/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:30:07.233206 ape-polygon-0.8.0/ape_polygon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-31 19:30:07.000000 ape-polygon-0.8.0/ape_polygon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-31 19:30:07.000000 ape-polygon-0.8.0/ape_polygon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:30:07.000000 ape-polygon-0.8.0/ape_polygon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:30:07.000000 ape-polygon-0.8.0/ape_polygon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-31 19:30:07.000000 ape-polygon-0.8.0/ape_polygon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 19:30:07.000000 ape-polygon-0.8.0/ape_polygon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-31 19:30:07.233206 ape-polygon-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:30:07.233206 ape-polygon-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/tests/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-31 19:29:15.000000 ape-polygon-0.8.0/tests/test_provider.py
```

### Comparing `ape-polygon-0.7.2/.github/ISSUE_TEMPLATE/bug.md` & `ape-polygon-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.7.2/.github/ISSUE_TEMPLATE/feature.md` & `ape-polygon-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.7.2/.github/ISSUE_TEMPLATE/work-item.md` & `ape-polygon-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.7.2/.github/release-drafter.yml` & `ape-polygon-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.7.2/.github/workflows/commitlint.yaml` & `ape-polygon-0.8.0/.github/workflows/commitlint.yaml`

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

### Comparing `ape-polygon-0.7.2/.github/workflows/prtitle.yaml` & `ape-polygon-0.8.0/.github/workflows/prtitle.yaml`

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

### Comparing `ape-polygon-0.7.2/.github/workflows/publish.yaml` & `ape-polygon-0.8.0/.github/workflows/publish.yaml`

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

### Comparing `ape-polygon-0.7.2/.github/workflows/test.yaml` & `ape-polygon-0.8.0/.github/workflows/test.yaml`

 * *Files 5% similar despite different names*

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
           run: pip install .[lint]
 
         - name: Run Black
@@ -54,22 +54,24 @@
           run: mypy .
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
-                os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, '3.10', '3.11']
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
           run: pip install .[test]
 
         - name: Run Tests
@@ -79,18 +81,18 @@
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

### Comparing `ape-polygon-0.7.2/.gitignore` & `ape-polygon-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.7.2/.pre-commit-config.yaml` & `ape-polygon-0.8.0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,31 @@
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
-    rev: 23.12.1
+    rev: 24.4.2
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
     rev: 7.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.10.0
     hooks:
     -   id: mypy
         additional_dependencies: [types-setuptools, pydantic]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
```

### Comparing `ape-polygon-0.7.2/CONTRIBUTING.md` & `ape-polygon-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.7.2/LICENSE` & `ape-polygon-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.7.2/PKG-INFO` & `ape-polygon-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: ape-polygon
-Version: 0.7.2
+Version: 0.8.0
 Summary: ape-polygon: Ape Ecosystem Plugin for Polygon
 Home-page: https://github.com/ApeWorX/ape-polygon
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
 
 Ecosystem Plugin for Polygon support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
```

### Comparing `ape-polygon-0.7.2/README.md` & `ape-polygon-0.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ecosystem Plugin for Polygon support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
```

### Comparing `ape-polygon-0.7.2/ape_polygon/__init__.py` & `ape-polygon-0.8.0/ape_polygon/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ape import plugins
 from ape.api.networks import LOCAL_NETWORK_NAME, ForkedNetworkAPI, NetworkAPI, create_network_type
-from ape_geth import GethProvider
+from ape_node import Node
 from ape_test import LocalProvider
 
 from .ecosystem import NETWORKS, Polygon, PolygonConfig
 
 
 @plugins.register(plugins.Config)
 def config_class():
@@ -25,10 +25,10 @@
     # NOTE: This works for development providers, as they get chain_id from themselves
     yield "polygon", LOCAL_NETWORK_NAME, NetworkAPI
 
 
 @plugins.register(plugins.ProviderPlugin)
 def providers():
     for network_name in NETWORKS:
-        yield "polygon", network_name, GethProvider
+        yield "polygon", network_name, Node
 
     yield "polygon", LOCAL_NETWORK_NAME, LocalProvider
```

### Comparing `ape-polygon-0.7.2/ape_polygon/ecosystem.py` & `ape-polygon-0.8.0/ape_polygon/ecosystem.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.7.2/ape_polygon.egg-info/PKG-INFO` & `ape-polygon-0.8.0/ape_polygon.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: ape-polygon
-Version: 0.7.2
+Version: 0.8.0
 Summary: ape-polygon: Ape Ecosystem Plugin for Polygon
 Home-page: https://github.com/ApeWorX/ape-polygon
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
 
 Ecosystem Plugin for Polygon support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
```

### Comparing `ape-polygon-0.7.2/ape_polygon.egg-info/SOURCES.txt` & `ape-polygon-0.8.0/ape_polygon.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.cfg
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
 .github/release-drafter.yml
 .github/ISSUE_TEMPLATE/bug.md
 .github/ISSUE_TEMPLATE/feature.md
 .github/ISSUE_TEMPLATE/work-item.md
+.github/workflows/codeql.yml
 .github/workflows/commitlint.yaml
 .github/workflows/draft.yaml
 .github/workflows/prtitle.yaml
 .github/workflows/publish.yaml
 .github/workflows/test.yaml
 ape_polygon/__init__.py
 ape_polygon/ecosystem.py
```

### Comparing `ape-polygon-0.7.2/ape_polygon.egg-info/requires.txt` & `ape-polygon-0.8.0/ape_polygon.egg-info/requires.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-eth-ape<0.8,>=0.7.6
+eth-ape<0.9,>=0.8.1
 ethpm-types
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7,>=6.2.0
-black<24,>=23.12.1
-mypy<2,>=1.8.0
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
 flake8<8,>=7.0.0
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
-black<24,>=23.12.1
-mypy<2,>=1.8.0
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
 flake8<8,>=7.0.0
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

### Comparing `ape-polygon-0.7.2/pyproject.toml` & `ape-polygon-0.8.0/pyproject.toml`

 * *Files 11% similar despite different names*

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

### Comparing `ape-polygon-0.7.2/setup.py` & `ape-polygon-0.8.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # Multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=23.12.1,<24",  # Auto-formatter and linter
-        "mypy>=1.8.0,<2",  # Static type analyzer
+        "black>=24.4.2,<25",  # Auto-formatter and linter
+        "mypy>=1.10.0,<2",  # Static type analyzer
         "types-setuptools",  # Needed for mypy type shed
         "flake8>=7.0.0,<8",  # Style linter
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
@@ -56,18 +56,18 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-polygon",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.6,<0.8",
+        "eth-ape>=0.8.1,<0.9",
         "ethpm-types",  # Use same version as eth-ape
     ],
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["ape_polygon"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_polygon": ["py.typed"]},
@@ -75,13 +75,13 @@
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

### Comparing `ape-polygon-0.7.2/tests/test_config.py` & `ape-polygon-0.8.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.7.2/tests/test_ecosystem.py` & `ape-polygon-0.8.0/tests/test_ecosystem.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-0.7.2/tests/test_integration.py` & `ape-polygon-0.8.0/tests/test_integration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import pytest
 from ape._cli import cli as ape_cli
 from click.testing import CliRunner
 
 EXPECTED_OUTPUT = """
 polygon
 ├── amoy
-│   └── geth  (default)
+│   └── node  (default)
 ├── local  (default)
 │   └── test  (default)
 ├── mainnet
-│   └── geth  (default)
+│   └── node  (default)
 └── mumbai
-    └── geth  (default)
+    └── node  (default)
 """.strip()
 
 
 @pytest.fixture
 def runner():
     return CliRunner()
 
@@ -44,13 +44,13 @@
 
     for expected_line in expected_lines:
         assert expected_line in actual_lines
 
 
 def test_networks(runner, cli, polygon):
     # Do this in case local env changed it.
-    polygon.mainnet.set_default_provider("geth")
-    polygon.mumbai.set_default_provider("geth")
-    polygon.amoy.set_default_provider("geth")
+    polygon.mainnet.set_default_provider("node")
+    polygon.mumbai.set_default_provider("node")
+    polygon.amoy.set_default_provider("node")
 
-    result = runner.invoke(cli, ["networks", "list"])
+    result = runner.invoke(cli, ("networks", "list"))
     assert_rich_text(result.output, EXPECTED_OUTPUT)
```

