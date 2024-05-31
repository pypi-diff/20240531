# Comparing `tmp/ape-arbitrum-0.7.2.tar.gz` & `tmp/ape-arbitrum-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-arbitrum-0.7.2.tar", last modified: Tue Jan 23 19:19:20 2024, max compression
+gzip compressed data, was "ape-arbitrum-0.8.0.tar", last modified: Fri May 31 20:44:51 2024, max compression
```

## Comparing `ape-arbitrum-0.7.2.tar` & `ape-arbitrum-0.8.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 19:19:20.436377 ape-arbitrum-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 19:19:20.432377 ape-arbitrum-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 19:19:20.432377 ape-arbitrum-0.7.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 19:19:20.432377 ape-arbitrum-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/.github/workflows/title.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-23 19:19:20.436377 ape-arbitrum-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 19:19:20.436377 ape-arbitrum-0.7.2/ape_arbitrum/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/ape_arbitrum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10375 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/ape_arbitrum/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/ape_arbitrum/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-23 19:19:20.000000 ape-arbitrum-0.7.2/ape_arbitrum/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 19:19:20.436377 ape-arbitrum-0.7.2/ape_arbitrum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-23 19:19:20.000000 ape-arbitrum-0.7.2/ape_arbitrum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-01-23 19:19:20.000000 ape-arbitrum-0.7.2/ape_arbitrum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 19:19:20.000000 ape-arbitrum-0.7.2/ape_arbitrum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 19:19:20.000000 ape-arbitrum-0.7.2/ape_arbitrum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-01-23 19:19:20.000000 ape-arbitrum-0.7.2/ape_arbitrum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-23 19:19:20.000000 ape-arbitrum-0.7.2/ape_arbitrum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-23 19:19:20.436377 ape-arbitrum-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3822 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 19:19:20.436377 ape-arbitrum-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/tests/test_ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-01-23 19:18:10.000000 ape-arbitrum-0.7.2/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:44:51.502602 ape-arbitrum-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:44:51.502602 ape-arbitrum-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:44:51.502602 ape-arbitrum-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:44:51.502602 ape-arbitrum-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/.github/workflows/title.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-31 20:44:51.502602 ape-arbitrum-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:44:51.502602 ape-arbitrum-0.8.0/ape_arbitrum/
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/ape_arbitrum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/ape_arbitrum/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/ape_arbitrum/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 20:44:51.000000 ape-arbitrum-0.8.0/ape_arbitrum/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:44:51.502602 ape-arbitrum-0.8.0/ape_arbitrum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-31 20:44:51.000000 ape-arbitrum-0.8.0/ape_arbitrum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-31 20:44:51.000000 ape-arbitrum-0.8.0/ape_arbitrum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:44:51.000000 ape-arbitrum-0.8.0/ape_arbitrum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:44:51.000000 ape-arbitrum-0.8.0/ape_arbitrum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-31 20:44:51.000000 ape-arbitrum-0.8.0/ape_arbitrum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 20:44:51.000000 ape-arbitrum-0.8.0/ape_arbitrum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-31 20:44:51.506602 ape-arbitrum-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:44:51.502602 ape-arbitrum-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/tests/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-31 20:44:02.000000 ape-arbitrum-0.8.0/tests/test_provider.py
```

### Comparing `ape-arbitrum-0.7.2/.github/ISSUE_TEMPLATE/bug.md` & `ape-arbitrum-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.7.2/.github/ISSUE_TEMPLATE/feature.md` & `ape-arbitrum-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.7.2/.github/ISSUE_TEMPLATE/work-item.md` & `ape-arbitrum-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.7.2/.github/release-drafter.yml` & `ape-arbitrum-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.7.2/.github/workflows/commitlint.yaml` & `ape-arbitrum-0.8.0/.github/workflows/commitlint.yaml`

 * *Files 3% similar despite different names*

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
           run: pip install .[dev]
 
         - name: Check commit history
```

### Comparing `ape-arbitrum-0.7.2/.github/workflows/publish.yaml` & `ape-arbitrum-0.8.0/.github/workflows/publish.yaml`

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

### Comparing `ape-arbitrum-0.7.2/.github/workflows/test.yaml` & `ape-arbitrum-0.8.0/.github/workflows/test.yaml`

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

### Comparing `ape-arbitrum-0.7.2/.github/workflows/title.yaml` & `ape-arbitrum-0.8.0/.github/workflows/title.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
       - synchronize
 
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v2
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v2
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
```

### Comparing `ape-arbitrum-0.7.2/.gitignore` & `ape-arbitrum-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.7.2/.pre-commit-config.yaml` & `ape-arbitrum-0.8.0/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

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

### Comparing `ape-arbitrum-0.7.2/CONTRIBUTING.md` & `ape-arbitrum-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.7.2/LICENSE` & `ape-arbitrum-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.7.2/PKG-INFO` & `ape-arbitrum-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: ape-arbitrum
-Version: 0.7.2
+Version: 0.8.0
 Summary: ape-arbitrum: Ape Ecosystem Plugin for Arbitrum
 Home-page: https://github.com/ApeWorX/ape-arbitrum
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
 
 Ecosystem Plugin for Arbitrum support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
```

### Comparing `ape-arbitrum-0.7.2/README.md` & `ape-arbitrum-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ecosystem Plugin for Arbitrum support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
```

### Comparing `ape-arbitrum-0.7.2/ape_arbitrum/__init__.py` & `ape-arbitrum-0.8.0/ape_arbitrum/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ape import plugins
 from ape.api.networks import LOCAL_NETWORK_NAME, ForkedNetworkAPI, NetworkAPI, create_network_type
-from ape_geth import GethProvider
+from ape_node import Node
 from ape_test import LocalProvider
 
 from .ecosystem import NETWORKS, Arbitrum, ArbitrumConfig
 
 
 @plugins.register(plugins.Config)
 def config_class():
@@ -25,10 +25,10 @@
     # NOTE: This works for development providers, as they get chain_id from themselves
     yield "arbitrum", LOCAL_NETWORK_NAME, NetworkAPI
 
 
 @plugins.register(plugins.ProviderPlugin)
 def providers():
     for network_name in NETWORKS:
-        yield "arbitrum", network_name, GethProvider
+        yield "arbitrum", network_name, Node
 
     yield "arbitrum", LOCAL_NETWORK_NAME, LocalProvider
```

### Comparing `ape-arbitrum-0.7.2/ape_arbitrum/ecosystem.py` & `ape-arbitrum-0.8.0/ape_arbitrum/ecosystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-from typing import ClassVar, Dict, Tuple, Type, cast
+from typing import ClassVar, cast
 
 from ape.api.transactions import ConfirmationsProgressBar, ReceiptAPI, TransactionAPI
 from ape.exceptions import ApeException, TransactionError
 from ape.logging import logger
 from ape.types import GasLimit, TransactionSignature
 from ape_ethereum.ecosystem import BaseEthereumConfig, Ethereum, NetworkConfig
 from ape_ethereum.transactions import (
@@ -16,15 +16,14 @@
 from ape_ethereum.transactions import TransactionType as EthTransactionType
 from eth_pydantic_types import HexBytes
 from pydantic.fields import Field
 
 NETWORKS = {
     # chain_id, network_id
     "mainnet": (42161, 42161),
-    "goerli": (421613, 421613),
     "sepolia": (421614, 421614),
 }
 INTERNAL_TRANSACTION_TYPE = 106
 
 # NOTE: Use a hard-coded gas limit for testing
 #   because the block gasLimit is extremely high in Arbitrum networks.
 LOCAL_GAS_LIMIT = 30_000_000
@@ -89,30 +88,29 @@
 
         return self
 
 
 def _create_config(
     required_confirmations: int = 1,
     block_time: int = 1,
-    cls: Type = NetworkConfig,
+    cls: type = NetworkConfig,
     **kwargs,
 ) -> NetworkConfig:
     return cls(
         required_confirmations=required_confirmations,
         block_time=block_time,
         default_transaction_type=EthTransactionType.STATIC,
         **kwargs,
     )
 
 
 class ArbitrumConfig(BaseEthereumConfig):
     DEFAULT_TRANSACTION_TYPE: ClassVar[int] = EthTransactionType.STATIC.value
     DEFAULT_LOCAL_GAS_LIMIT: ClassVar[GasLimit] = LOCAL_GAS_LIMIT
     mainnet: NetworkConfig = _create_config()
-    goerli: NetworkConfig = _create_config()
     sepolia: NetworkConfig = _create_config()
 
 
 class Arbitrum(Ethereum):
     @property
     def config(self) -> ArbitrumConfig:  # type: ignore[override]
         return cast(ArbitrumConfig, self.config_manager.get_config("arbitrum"))
@@ -150,15 +148,15 @@
             tx_data["value"] = self.conversion_manager.convert(value, int)
 
         # None is not allowed, the user likely means `b""`.
         if "data" in tx_data and tx_data["data"] is None:
             tx_data["data"] = b""
 
         # Deduce the transaction type.
-        transaction_types: Dict[int, Type[TransactionAPI]] = {
+        transaction_types: dict[int, type[TransactionAPI]] = {
             EthTransactionType.STATIC.value: StaticFeeTransaction,
             EthTransactionType.DYNAMIC.value: DynamicFeeTransaction,
             EthTransactionType.ACCESS_LIST.value: AccessListTransaction,
             INTERNAL_TRANSACTION_TYPE: InternalTransaction,
         }
 
         if "type" in tx_data:
@@ -262,15 +260,15 @@
             logs=data.get("logs", []),
             status=status,
             txn_hash=txn_hash,
             transaction=self.create_transaction(**data),
         )
 
 
-def _correct_key(key: str, data: Dict, alt_keys: Tuple[str, ...]) -> Dict:
+def _correct_key(key: str, data: dict, alt_keys: tuple[str, ...]) -> dict:
     if key in data:
         return data
 
     # Check for alternative.
     for possible_key in alt_keys:
         if possible_key not in data:
             continue
```

### Comparing `ape-arbitrum-0.7.2/ape_arbitrum.egg-info/PKG-INFO` & `ape-arbitrum-0.8.0/ape_arbitrum.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: ape-arbitrum
-Version: 0.7.2
+Version: 0.8.0
 Summary: ape-arbitrum: Ape Ecosystem Plugin for Arbitrum
 Home-page: https://github.com/ApeWorX/ape-arbitrum
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
 
 Ecosystem Plugin for Arbitrum support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
```

### Comparing `ape-arbitrum-0.7.2/ape_arbitrum.egg-info/SOURCES.txt` & `ape-arbitrum-0.8.0/ape_arbitrum.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 setup.cfg
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
 .github/release-drafter.yml
 .github/ISSUE_TEMPLATE/bug.md
 .github/ISSUE_TEMPLATE/feature.md
 .github/ISSUE_TEMPLATE/work-item.md
+.github/workflows/codeql.yaml
 .github/workflows/commitlint.yaml
 .github/workflows/draft.yaml
 .github/workflows/publish.yaml
 .github/workflows/test.yaml
 .github/workflows/title.yaml
 ape_arbitrum/__init__.py
 ape_arbitrum/ecosystem.py
```

### Comparing `ape-arbitrum-0.7.2/ape_arbitrum.egg-info/requires.txt` & `ape-arbitrum-0.8.0/ape_arbitrum.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-eth-ape<0.8,>=0.7.6
+eth-ape<0.9,>=0.8.1
 eth-pydantic-types
 ethpm-types
 
 [dev]
 pytest>=6.0
 pytest-mock
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
 myst-parser<2,>=1.0.0
 sphinx-click<5,>=4.4.0
 Sphinx<7,>=6.1.3
@@ -39,21 +39,21 @@
 sphinx-click<5,>=4.4.0
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 sphinxcontrib-napoleon>=0.7
 sphinx-plausible<0.2,>=0.1.2
 
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

### Comparing `ape-arbitrum-0.7.2/pyproject.toml` & `ape-arbitrum-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

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

### Comparing `ape-arbitrum-0.7.2/setup.py` & `ape-arbitrum-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,21 +7,21 @@
         "pytest>=6.0",  # Core testing package
         "pytest-mock",  # For patching and mocking
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
     "doc": [
         "myst-parser>=1.0.0,<2",  # Parse markdown docs
@@ -67,19 +67,19 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-arbitrum",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.6,<0.8",
+        "eth-ape>=0.8.1,<0.9",
         "eth-pydantic-types",  # Use same version as eth-ape
         "ethpm-types",  # Use same version as eth-ape
     ],
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["ape_arbitrum"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_arbitrum": ["py.typed"]},
@@ -87,13 +87,13 @@
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

### Comparing `ape-arbitrum-0.7.2/tests/conftest.py` & `ape-arbitrum-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.7.2/tests/test_config.py` & `ape-arbitrum-0.8.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.7.2/tests/test_ecosystem.py` & `ape-arbitrum-0.8.0/tests/test_ecosystem.py`

 * *Files identical despite different names*

### Comparing `ape-arbitrum-0.7.2/tests/test_integration.py` & `ape-arbitrum-0.8.0/tests/test_integration.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import pytest
 from ape._cli import cli as ape_cli
 from click.testing import CliRunner
 
 EXPECTED_OUTPUT = """
 arbitrum
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
 
 
 def test_networks(runner, cli, arbitrum):
     # Do this in case local env changed it.
-    arbitrum.mainnet.set_default_provider("geth")
-    arbitrum.goerli.set_default_provider("geth")
-    arbitrum.sepolia.set_default_provider("geth")
+    arbitrum.mainnet.set_default_provider("node")
+    arbitrum.sepolia.set_default_provider("node")
 
-    result = runner.invoke(cli, ["networks", "list"])
+    result = runner.invoke(cli, ("networks", "list"))
     assert_rich_text(result.output, EXPECTED_OUTPUT)
```

