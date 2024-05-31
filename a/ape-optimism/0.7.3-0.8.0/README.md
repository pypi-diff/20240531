# Comparing `tmp/ape-optimism-0.7.3.tar.gz` & `tmp/ape-optimism-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-optimism-0.7.3.tar", last modified: Mon Feb 19 16:25:01 2024, max compression
+gzip compressed data, was "ape-optimism-0.8.0.tar", last modified: Fri May 31 19:01:52 2024, max compression
```

## Comparing `ape-optimism-0.7.3.tar` & `ape-optimism-0.8.0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:25:01.925456 ape-optimism-0.7.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:25:01.925456 ape-optimism-0.7.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:25:01.925456 ape-optimism-0.7.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:25:01.925456 ape-optimism-0.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2336 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-19 16:25:01.925456 ape-optimism-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:25:01.925456 ape-optimism-0.7.3/ape_optimism/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/ape_optimism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/ape_optimism/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/ape_optimism/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-19 16:25:01.000000 ape-optimism-0.7.3/ape_optimism/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:25:01.925456 ape-optimism-0.7.3/ape_optimism.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-02-19 16:25:01.000000 ape-optimism-0.7.3/ape_optimism.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-19 16:25:01.000000 ape-optimism-0.7.3/ape_optimism.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 16:25:01.000000 ape-optimism-0.7.3/ape_optimism.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 16:25:01.000000 ape-optimism-0.7.3/ape_optimism.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-02-19 16:25:01.000000 ape-optimism-0.7.3/ape_optimism.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-19 16:25:01.000000 ape-optimism-0.7.3/ape_optimism.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-19 16:25:01.925456 ape-optimism-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 16:25:01.925456 ape-optimism-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/tests/test_ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-02-19 16:24:03.000000 ape-optimism-0.7.3/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:01:52.627110 ape-optimism-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:01:52.623110 ape-optimism-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:01:52.623110 ape-optimism-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:01:52.627110 ape-optimism-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-31 19:01:52.627110 ape-optimism-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:01:52.627110 ape-optimism-0.8.0/ape_optimism/
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/ape_optimism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/ape_optimism/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/ape_optimism/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 19:01:52.000000 ape-optimism-0.8.0/ape_optimism/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:01:52.627110 ape-optimism-0.8.0/ape_optimism.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-31 19:01:52.000000 ape-optimism-0.8.0/ape_optimism.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-31 19:01:52.000000 ape-optimism-0.8.0/ape_optimism.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:01:52.000000 ape-optimism-0.8.0/ape_optimism.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 19:01:52.000000 ape-optimism-0.8.0/ape_optimism.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-31 19:01:52.000000 ape-optimism-0.8.0/ape_optimism.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 19:01:52.000000 ape-optimism-0.8.0/ape_optimism.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-31 19:01:52.627110 ape-optimism-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 19:01:52.627110 ape-optimism-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/tests/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-31 19:00:58.000000 ape-optimism-0.8.0/tests/test_provider.py
```

### Comparing `ape-optimism-0.7.3/.github/ISSUE_TEMPLATE/bug.md` & `ape-optimism-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.7.3/.github/ISSUE_TEMPLATE/feature.md` & `ape-optimism-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.7.3/.github/ISSUE_TEMPLATE/work-item.md` & `ape-optimism-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.7.3/.github/release-drafter.yml` & `ape-optimism-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.7.3/.github/workflows/commitlint.yaml` & `ape-optimism-0.8.0/.github/workflows/commitlint.yaml`

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

### Comparing `ape-optimism-0.7.3/.github/workflows/prtitle.yaml` & `ape-optimism-0.8.0/.github/workflows/prtitle.yaml`

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

### Comparing `ape-optimism-0.7.3/.github/workflows/publish.yaml` & `ape-optimism-0.8.0/.github/workflows/publish.yaml`

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

### Comparing `ape-optimism-0.7.3/.github/workflows/test.yaml` & `ape-optimism-0.8.0/.github/workflows/test.yaml`

 * *Files 8% similar despite different names*

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
@@ -36,61 +36,63 @@
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
           run: pip install .[lint,test]  # Might need test deps
 
         - name: Run MyPy
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
           run: pip install .[test]
-
-#        - name: Run Tests
-#          run: pytest -m "not fuzzing" -n 0 -s --cov
+        
+        - name: Run Tests
+          run: pytest -m "not fuzzing" -n 0 -s --cov
 
 # NOTE: uncomment this block after you've marked tests with @pytest.mark.fuzzing
 #    fuzzing:
 #        runs-on: ubuntu-latest
 #
 #        strategy:
 #            fail-fast: true
 #
 #        steps:
-#        - uses: actions/checkout@v2
+#        - uses: actions/checkout@v4
 #
 #        - name: Setup Python
-#          uses: actions/setup-python@v2
+#          uses: actions/setup-python@v5
 #          with:
 #              python-version: "3.10"
 #
 #        - name: Install Dependencies
 #          run: pip install .[test]
 #
 #        - name: Run Tests
```

### Comparing `ape-optimism-0.7.3/.gitignore` & `ape-optimism-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.7.3/.pre-commit-config.yaml` & `ape-optimism-0.8.0/.pre-commit-config.yaml`

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
+    rev: v5.13.2
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 24.2.0
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

### Comparing `ape-optimism-0.7.3/CONTRIBUTING.md` & `ape-optimism-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.7.3/LICENSE` & `ape-optimism-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.7.3/PKG-INFO` & `ape-optimism-0.8.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: ape-optimism
-Version: 0.7.3
+Version: 0.8.0
 Summary: ape-optimism: Ape Ecosystem Plugin for Optimism
 Home-page: https://github.com/ApeWorX/ape-optimism
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
 
 Ecosystem Plugin for Optimism support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
 
@@ -71,13 +71,13 @@
 ```
 
 ## Quick Usage
 
 Installing this plugin adds support for the Optimism ecosystem:
 
 ```bash
-ape console --network optimism:goerli
+ape console --network optimism:sepolia
 ```
 
 ## Development
 
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-optimism-0.7.3/ape_optimism/__init__.py` & `ape-optimism-0.8.0/ape_optimism/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ape import plugins
 from ape.api.networks import LOCAL_NETWORK_NAME, ForkedNetworkAPI, NetworkAPI, create_network_type
-from ape_geth import GethProvider
+from ape_node import Node
 from ape_test import LocalProvider
 
 from .ecosystem import NETWORKS, Optimism, OptimismConfig
 
 
 @plugins.register(plugins.Config)
 def config_class():
@@ -25,10 +25,10 @@
     # NOTE: This works for local providers, as they get chain_id from themselves
     yield "optimism", LOCAL_NETWORK_NAME, NetworkAPI
 
 
 @plugins.register(plugins.ProviderPlugin)
 def providers():
     for network_name in NETWORKS:
-        yield "optimism", network_name, GethProvider
+        yield "optimism", network_name, Node
 
     yield "optimism", LOCAL_NETWORK_NAME, LocalProvider
```

### Comparing `ape-optimism-0.7.3/ape_optimism/ecosystem.py` & `ape-optimism-0.8.0/ape_optimism/ecosystem.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,30 +9,28 @@
     create_network_config,
 )
 from eth_pydantic_types import HexBytes
 
 NETWORKS = {
     # chain_id, network_id
     "mainnet": (10, 10),
-    "goerli": (420, 420),
     "sepolia": (11155420, 11155420),
 }
 SYSTEM_TRANSACTION = 126
 
 
 class ApeOptimismError(ApeException):
     """
     Raised in the ape-optimism plugin.
     """
 
 
 # NOTE: Forked networks automatically are included.
 class OptimismConfig(BaseEthereumConfig):
     mainnet: NetworkConfig = create_network_config(block_time=2)
-    goerli: NetworkConfig = create_network_config(block_time=2)
     sepolia: NetworkConfig = create_network_config(block_time=2)
 
 
 class SystemTransaction(TransactionAPI):
     type: int = SYSTEM_TRANSACTION
 
     @property
```

### Comparing `ape-optimism-0.7.3/ape_optimism.egg-info/PKG-INFO` & `ape-optimism-0.8.0/ape_optimism.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: ape-optimism
-Version: 0.7.3
+Version: 0.8.0
 Summary: ape-optimism: Ape Ecosystem Plugin for Optimism
 Home-page: https://github.com/ApeWorX/ape-optimism
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
 
 Ecosystem Plugin for Optimism support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `ape`
 
 You can install this plugin using `ape`:
 
@@ -71,13 +71,13 @@
 ```
 
 ## Quick Usage
 
 Installing this plugin adds support for the Optimism ecosystem:
 
 ```bash
-ape console --network optimism:goerli
+ape console --network optimism:sepolia
 ```
 
 ## Development
 
 Comments, questions, criticisms and pull requests are welcomed.
```

### Comparing `ape-optimism-0.7.3/ape_optimism.egg-info/SOURCES.txt` & `ape-optimism-0.8.0/ape_optimism.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

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
 ape_optimism/__init__.py
 ape_optimism/ecosystem.py
```

### Comparing `ape-optimism-0.7.3/ape_optimism.egg-info/requires.txt` & `ape-optimism-0.8.0/ape_optimism.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-eth-ape<0.8,>=0.7.6
+eth-ape<0.9,>=0.8.1
 ethpm-types
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
-black<25,>=24.2.0
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
-black<25,>=24.2.0
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

### Comparing `ape-optimism-0.7.3/pyproject.toml` & `ape-optimism-0.8.0/pyproject.toml`

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

### Comparing `ape-optimism-0.7.3/setup.py` & `ape-optimism-0.8.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,21 @@
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=24.2.0,<25",  # Auto-formatter and linter
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
     url="https://github.com/ApeWorX/ape-optimism",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.6,<0.8",
+        "eth-ape>=0.8.1,<0.9",
         "ethpm-types",  # Use same version as eth-ape
     ],
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["ape_optimism"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_optimism": ["py.typed"]},
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

### Comparing `ape-optimism-0.7.3/tests/test_ecosystem.py` & `ape-optimism-0.8.0/tests/test_ecosystem.py`

 * *Files identical despite different names*

### Comparing `ape-optimism-0.7.3/tests/test_integration.py` & `ape-optimism-0.8.0/tests/test_integration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import pytest
 from ape._cli import cli as ape_cli
 from click.testing import CliRunner
 
 EXPECTED_OUTPUT = """
 optimism
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
 
@@ -43,13 +41,12 @@
     ]
 
     for expected_line in expected_lines:
         assert expected_line in actual_lines
 
 
 def test_networks(runner, cli, optimism):
-    optimism.mainnet.set_default_provider("geth")
-    optimism.goerli.set_default_provider("geth")
-    optimism.sepolia.set_default_provider("geth")
+    optimism.mainnet.set_default_provider("node")
+    optimism.sepolia.set_default_provider("node")
 
-    result = runner.invoke(cli, ["networks", "list"])
+    result = runner.invoke(cli, ("networks", "list"))
     assert_rich_text(result.output, EXPECTED_OUTPUT)
```

