# Comparing `tmp/ape-base-0.7.1.tar.gz` & `tmp/ape-base-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-base-0.7.1.tar", last modified: Tue Jan 23 22:05:57 2024, max compression
+gzip compressed data, was "ape-base-0.8.0.tar", last modified: Fri May 31 20:57:38 2024, max compression
```

## Comparing `ape-base-0.7.1.tar` & `ape-base-0.8.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:05:57.048725 ape-base-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:05:57.044724 ape-base-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:05:57.044724 ape-base-0.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-01-23 22:04:56.000000 ape-base-0.7.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-23 22:04:56.000000 ape-base-0.7.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-01-23 22:04:56.000000 ape-base-0.7.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-23 22:04:56.000000 ape-base-0.7.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-23 22:04:56.000000 ape-base-0.7.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:05:57.048725 ape-base-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-01-23 22:04:56.000000 ape-base-0.7.1/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-01-23 22:04:56.000000 ape-base-0.7.1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-01-23 22:04:56.000000 ape-base-0.7.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-23 22:04:56.000000 ape-base-0.7.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-23 22:04:56.000000 ape-base-0.7.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-01-23 22:04:56.000000 ape-base-0.7.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-01-23 22:04:56.000000 ape-base-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-01-23 22:04:56.000000 ape-base-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-01-23 22:04:56.000000 ape-base-0.7.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-01-23 22:04:56.000000 ape-base-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-01-23 22:05:57.048725 ape-base-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-01-23 22:04:56.000000 ape-base-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:05:57.048725 ape-base-0.7.1/ape_base/
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-01-23 22:04:56.000000 ape-base-0.7.1/ape_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5975 2024-01-23 22:04:56.000000 ape-base-0.7.1/ape_base/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 22:04:56.000000 ape-base-0.7.1/ape_base/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-23 22:05:56.000000 ape-base-0.7.1/ape_base/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:05:57.048725 ape-base-0.7.1/ape_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-01-23 22:05:56.000000 ape-base-0.7.1/ape_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-01-23 22:05:57.000000 ape-base-0.7.1/ape_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 22:05:56.000000 ape-base-0.7.1/ape_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 22:05:56.000000 ape-base-0.7.1/ape_base.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-01-23 22:05:56.000000 ape-base-0.7.1/ape_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-23 22:05:56.000000 ape-base-0.7.1/ape_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-23 22:04:56.000000 ape-base-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-23 22:05:57.048725 ape-base-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3261 2024-01-23 22:04:56.000000 ape-base-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 22:05:57.048725 ape-base-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 22:04:56.000000 ape-base-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-01-23 22:04:56.000000 ape-base-0.7.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-01-23 22:04:56.000000 ape-base-0.7.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-01-23 22:04:56.000000 ape-base-0.7.1/tests/test_ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-01-23 22:04:56.000000 ape-base-0.7.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-01-23 22:04:56.000000 ape-base-0.7.1/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:57:38.795905 ape-base-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:57:38.791905 ape-base-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:57:38.791905 ape-base-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-31 20:56:42.000000 ape-base-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-31 20:56:42.000000 ape-base-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-31 20:56:42.000000 ape-base-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 20:56:42.000000 ape-base-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-31 20:56:42.000000 ape-base-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:57:38.795905 ape-base-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-31 20:56:42.000000 ape-base-0.8.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-31 20:56:42.000000 ape-base-0.8.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 20:56:42.000000 ape-base-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 20:56:42.000000 ape-base-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-31 20:56:42.000000 ape-base-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-31 20:56:42.000000 ape-base-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-31 20:56:42.000000 ape-base-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-31 20:56:42.000000 ape-base-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-31 20:56:42.000000 ape-base-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-31 20:56:42.000000 ape-base-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-31 20:57:38.795905 ape-base-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-31 20:56:42.000000 ape-base-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:57:38.795905 ape-base-0.8.0/ape_base/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-31 20:56:42.000000 ape-base-0.8.0/ape_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-05-31 20:56:42.000000 ape-base-0.8.0/ape_base/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:56:42.000000 ape-base-0.8.0/ape_base/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 20:57:38.000000 ape-base-0.8.0/ape_base/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:57:38.795905 ape-base-0.8.0/ape_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-31 20:57:38.000000 ape-base-0.8.0/ape_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-31 20:57:38.000000 ape-base-0.8.0/ape_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:57:38.000000 ape-base-0.8.0/ape_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:57:38.000000 ape-base-0.8.0/ape_base.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-31 20:57:38.000000 ape-base-0.8.0/ape_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 20:57:38.000000 ape-base-0.8.0/ape_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-31 20:56:42.000000 ape-base-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-31 20:57:38.795905 ape-base-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-05-31 20:56:42.000000 ape-base-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:57:38.795905 ape-base-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:56:42.000000 ape-base-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-31 20:56:42.000000 ape-base-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-31 20:56:42.000000 ape-base-0.8.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-31 20:56:42.000000 ape-base-0.8.0/tests/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-31 20:56:42.000000 ape-base-0.8.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-31 20:56:42.000000 ape-base-0.8.0/tests/test_provider.py
```

### Comparing `ape-base-0.7.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-base-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-base-0.7.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-base-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-base-0.7.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-base-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-base-0.7.1/.github/release-drafter.yml` & `ape-base-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-base-0.7.1/.github/workflows/codeql.yaml` & `ape-base-0.8.0/.github/workflows/codeql.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       security-events: write
 
     strategy:
       fail-fast: false
 
     steps:
     - name: Checkout repository
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
 
     - name: Initialize CodeQL
       uses: github/codeql-action/init@v2
       with:
         languages: python
 
     - name: Autobuild
```

### Comparing `ape-base-0.7.1/.github/workflows/commitlint.yaml` & `ape-base-0.8.0/.github/workflows/commitlint.yaml`

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

### Comparing `ape-base-0.7.1/.github/workflows/prtitle.yaml` & `ape-base-0.8.0/.github/workflows/prtitle.yaml`

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

### Comparing `ape-base-0.7.1/.github/workflows/publish.yaml` & `ape-base-0.8.0/.github/workflows/publish.yaml`

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

### Comparing `ape-base-0.7.1/.github/workflows/test.yaml` & `ape-base-0.8.0/.github/workflows/test.yaml`

 * *Files 10% similar despite different names*

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

### Comparing `ape-base-0.7.1/.gitignore` & `ape-base-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-base-0.7.1/.pre-commit-config.yaml` & `ape-base-0.8.0/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,35 @@
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
     -   id: mdformat
         additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
-
 default_language_version:
     python: python3
```

### Comparing `ape-base-0.7.1/CONTRIBUTING.md` & `ape-base-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-base-0.7.1/LICENSE` & `ape-base-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-base-0.7.1/PKG-INFO` & `ape-base-0.8.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: ape-base
-Version: 0.7.1
+Version: 0.8.0
 Summary: ape-base: Base ecosystem for Ape
 Home-page: https://github.com/ApeWorX/ape-base
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
 
 Ecosystem Plugin for [Base](https://base.org/) support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
 
@@ -55,15 +55,15 @@
 ```
 
 ## Quick Usage
 
 Installing this plugin adds support for the Base ecosystem:
 
 ```
-ape console --network base:goerli 
+ape console --network base:sepolia
 ```
 
 ## Development
 
 This project is in development and should be considered a beta.
 Things might not be in their final state and breaking changes may occur.
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-base-0.7.1/README.md` & `ape-base-0.8.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ecosystem Plugin for [Base](https://base.org/) support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
 
@@ -27,15 +27,15 @@
 ```
 
 ## Quick Usage
 
 Installing this plugin adds support for the Base ecosystem:
 
 ```
-ape console --network base:goerli 
+ape console --network base:sepolia
 ```
 
 ## Development
 
 This project is in development and should be considered a beta.
 Things might not be in their final state and breaking changes may occur.
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-base-0.7.1/ape_base/__init__.py` & `ape-base-0.8.0/ape_base/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ape import plugins
 from ape.api.networks import LOCAL_NETWORK_NAME, ForkedNetworkAPI, NetworkAPI, create_network_type
-from ape_geth import GethProvider
+from ape_node import Node
 from ape_test import LocalProvider
 
 from .ecosystem import NETWORKS, Base, BaseConfig
 
 
 @plugins.register(plugins.Config)
 def config_class():
@@ -25,10 +25,10 @@
     # NOTE: This works for local providers, as they get chain_id from themselves
     yield "base", LOCAL_NETWORK_NAME, NetworkAPI
 
 
 @plugins.register(plugins.ProviderPlugin)
 def providers():
     for network_name in NETWORKS:
-        yield "base", network_name, GethProvider
+        yield "base", network_name, Node
 
     yield "base", LOCAL_NETWORK_NAME, LocalProvider
```

### Comparing `ape-base-0.7.1/ape_base/ecosystem.py` & `ape-base-0.8.0/ape_base/ecosystem.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import ClassVar, Dict, Tuple, Type, cast
+from typing import ClassVar, cast
 
 from ape.api import TransactionAPI
 from ape.types import TransactionSignature
 from ape_ethereum.ecosystem import NetworkConfig, create_network_config
 from ape_ethereum.transactions import (
     AccessListTransaction,
     DynamicFeeTransaction,
@@ -10,28 +10,24 @@
     TransactionType,
 )
 from ape_optimism import Optimism, OptimismConfig
 
 NETWORKS = {
     # chain_id, network_id
     "mainnet": (8453, 8453),
-    "goerli": (84531, 84531),
     "sepolia": (84532, 84532),
 }
 _SECOND_STATIC_TYPE = 126
 
 
 class BaseConfig(OptimismConfig):
     DEFAULT_TRANSACTION_TYPE: ClassVar[int] = TransactionType.STATIC.value
     mainnet: NetworkConfig = create_network_config(
         block_time=2, default_transaction_type=TransactionType.STATIC
     )
-    goerli: NetworkConfig = create_network_config(
-        block_time=2, default_transaction_type=TransactionType.STATIC
-    )
     sepolia: NetworkConfig = create_network_config(
         block_time=2, default_transaction_type=TransactionType.STATIC
     )
 
 
 # NOTE: Since base is built on Optimism, we use Optimism as the base class.
 class Base(Optimism):
@@ -72,15 +68,15 @@
             tx_data["value"] = self.conversion_manager.convert(value, int)
 
         # None is not allowed, the user likely means `b""`.
         if "data" in tx_data and tx_data["data"] is None:
             tx_data["data"] = b""
 
         # Deduce the transaction type.
-        transaction_types: Dict[int, Type[TransactionAPI]] = {
+        transaction_types: dict[int, type[TransactionAPI]] = {
             TransactionType.STATIC.value: StaticFeeTransaction,
             TransactionType.DYNAMIC.value: DynamicFeeTransaction,
             TransactionType.ACCESS_LIST.value: AccessListTransaction,
             _SECOND_STATIC_TYPE: StaticFeeTransaction,
         }
 
         if "type" in tx_data:
@@ -142,15 +138,15 @@
 
         if "gas" not in tx_data:
             tx_data["gas"] = None
 
         return txn_class(**tx_data)
 
 
-def _correct_key(key: str, data: Dict, alt_keys: Tuple[str, ...]) -> Dict:
+def _correct_key(key: str, data: dict, alt_keys: tuple[str, ...]) -> dict:
     if key in data:
         return data
 
     # Check for alternative.
     for possible_key in alt_keys:
         if possible_key not in data:
             continue
```

### Comparing `ape-base-0.7.1/ape_base.egg-info/PKG-INFO` & `ape-base-0.8.0/ape_base.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: ape-base
-Version: 0.7.1
+Version: 0.8.0
 Summary: ape-base: Base ecosystem for Ape
 Home-page: https://github.com/ApeWorX/ape-base
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
 
 Ecosystem Plugin for [Base](https://base.org/) support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
 
@@ -55,15 +55,15 @@
 ```
 
 ## Quick Usage
 
 Installing this plugin adds support for the Base ecosystem:
 
 ```
-ape console --network base:goerli 
+ape console --network base:sepolia
 ```
 
 ## Development
 
 This project is in development and should be considered a beta.
 Things might not be in their final state and breaking changes may occur.
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-base-0.7.1/ape_base.egg-info/SOURCES.txt` & `ape-base-0.8.0/ape_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-base-0.7.1/ape_base.egg-info/requires.txt` & `ape-base-0.8.0/ape_base.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-eth-ape<0.8,>=0.7.6
-ape-optimism<0.8,>=0.7.2
+eth-ape<0.9,>=0.8.1
+ape-optimism
 ethpm-types
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
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

### Comparing `ape-base-0.7.1/pyproject.toml` & `ape-base-0.8.0/pyproject.toml`

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

### Comparing `ape-base-0.7.1/setup.py` & `ape-base-0.8.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # Multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
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
@@ -56,19 +56,19 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-base",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.6,<0.8",
-        "ape-optimism>=0.7.2,<0.8",
+        "eth-ape>=0.8.1,<0.9",
+        "ape-optimism",  # Ape determines the version
         "ethpm-types",  # Use same version as eth-ape
     ],
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["ape_base"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_base": ["py.typed"]},
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

### Comparing `ape-base-0.7.1/tests/test_config.py` & `ape-base-0.8.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ape-base-0.7.1/tests/test_ecosystem.py` & `ape-base-0.8.0/tests/test_ecosystem.py`

 * *Files identical despite different names*

### Comparing `ape-base-0.7.1/tests/test_integration.py` & `ape-base-0.8.0/tests/test_integration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import pytest
 from ape._cli import cli as ape_cli
 from click.testing import CliRunner
 
 EXPECTED_OUTPUT = """
 base
+├── local  (default)
+│   └── test  (default)
 ├── mainnet
-│   └── geth  (default)
-├── goerli
-│   └── geth  (default)
-├── sepolia
-│   └── geth  (default)
-└── local  (default)
-    └── test  (default)
+│   └── node  (default)
+└── sepolia
+    └── node  (default)
 """.strip()
 
 
 @pytest.fixture
 def runner():
     return CliRunner()
 
@@ -44,13 +42,12 @@
 
     for expected_line in expected_lines:
         assert expected_line in actual_lines
 
 
 def test_networks(runner, cli, base):
     # Do this in case local env changed it.
-    base.mainnet.set_default_provider("geth")
-    base.goerli.set_default_provider("geth")
-    base.sepolia.set_default_provider("geth")
+    base.mainnet.set_default_provider("node")
+    base.sepolia.set_default_provider("node")
 
-    result = runner.invoke(cli, ["networks", "list"])
+    result = runner.invoke(cli, ("networks", "list"))
     assert_rich_text(result.output, EXPECTED_OUTPUT)
```

### Comparing `ape-base-0.7.1/tests/test_provider.py` & `ape-base-0.8.0/tests/test_provider.py`

 * *Files identical despite different names*

