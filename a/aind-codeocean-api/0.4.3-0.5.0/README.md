# Comparing `tmp/aind_codeocean_api-0.4.3.tar.gz` & `tmp/aind_codeocean_api-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_codeocean_api-0.4.3.tar", last modified: Wed May 22 22:19:55 2024, max compression
+gzip compressed data, was "aind_codeocean_api-0.5.0.tar", last modified: Fri May 31 01:22:48 2024, max compression
```

## Comparing `aind_codeocean_api-0.4.3.tar` & `aind_codeocean_api-0.5.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.793037 aind_codeocean_api-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.785036 aind_codeocean_api-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.785036 aind_codeocean_api-0.4.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.785036 aind_codeocean_api-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-22 22:19:55.793037 aind_codeocean_api-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.789037 aind_codeocean_api-0.4.3/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.789037 aind_codeocean_api-0.4.3/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.789037 aind_codeocean_api-0.4.3/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/source/aind_codeocean_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/doc_template/source/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.789037 aind_codeocean_api-0.4.3/integration/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/integration/.env.template
--rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/integration/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:19:55.793037 aind_codeocean_api-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.785036 aind_codeocean_api-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.789037 aind_codeocean_api-0.4.3/src/aind_codeocean_api/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/codeocean.py
--rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.793037 aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/basic_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/computations_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/data_assets_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.793037 aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-22 22:19:55.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-22 22:19:55.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:19:55.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-22 22:19:55.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 22:19:55.000000 aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.793037 aind_codeocean_api-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:19:55.793037 aind_codeocean_api-0.4.3/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/tests/resources/fake_credentials.json
--rw-r--r--   0 runner    (1001) docker     (127)    36949 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/tests/test_codeocean_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-05-22 22:19:46.000000 aind_codeocean_api-0.4.3/tests/test_credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:22:48.614507 aind_codeocean_api-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:22:48.606507 aind_codeocean_api-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:22:48.610507 aind_codeocean_api-0.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:22:48.610507 aind_codeocean_api-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-31 01:22:48.614507 aind_codeocean_api-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:22:48.610507 aind_codeocean_api-0.5.0/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:22:48.610507 aind_codeocean_api-0.5.0/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:22:48.610507 aind_codeocean_api-0.5.0/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/doc_template/source/aind_codeocean_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/doc_template/source/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:22:48.610507 aind_codeocean_api-0.5.0/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/integration/.env.template
+-rw-r--r--   0 runner    (1001) docker     (127)     7006 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/integration/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 01:22:48.614507 aind_codeocean_api-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:22:48.606507 aind_codeocean_api-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:22:48.610507 aind_codeocean_api-0.5.0/src/aind_codeocean_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/src/aind_codeocean_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20628 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/src/aind_codeocean_api/codeocean.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/src/aind_codeocean_api/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:22:48.614507 aind_codeocean_api-0.5.0/src/aind_codeocean_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/src/aind_codeocean_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/src/aind_codeocean_api/models/basic_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/src/aind_codeocean_api/models/computations_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/src/aind_codeocean_api/models/data_assets_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/src/aind_codeocean_api/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:22:48.614507 aind_codeocean_api-0.5.0/src/aind_codeocean_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2024-05-31 01:22:48.000000 aind_codeocean_api-0.5.0/src/aind_codeocean_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-31 01:22:48.000000 aind_codeocean_api-0.5.0/src/aind_codeocean_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 01:22:48.000000 aind_codeocean_api-0.5.0/src/aind_codeocean_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-31 01:22:48.000000 aind_codeocean_api-0.5.0/src/aind_codeocean_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 01:22:48.000000 aind_codeocean_api-0.5.0/src/aind_codeocean_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:22:48.614507 aind_codeocean_api-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:22:48.614507 aind_codeocean_api-0.5.0/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/tests/resources/fake_credentials.json
+-rw-r--r--   0 runner    (1001) docker     (127)    39651 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/tests/test_codeocean_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11255 2024-05-31 01:22:35.000000 aind_codeocean_api-0.5.0/tests/test_credentials.py
```

### Comparing `aind_codeocean_api-0.4.3/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_codeocean_api-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_codeocean_api-0.5.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/.github/ISSUE_TEMPLATE/user-story.md` & `aind_codeocean_api-0.5.0/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/.github/workflows/lint_and_test.yml` & `aind_codeocean_api-0.5.0/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/.github/workflows/tag_and_publish.yml` & `aind_codeocean_api-0.5.0/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/.gitignore` & `aind_codeocean_api-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/LICENSE` & `aind_codeocean_api-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/PKG-INFO` & `aind_codeocean_api-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_codeocean_api
-Version: 0.4.3
+Version: 0.5.0
 Summary: CodeOcean API manager in Python
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_codeocean_api-0.4.3/README.md` & `aind_codeocean_api-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/doc_template/Makefile` & `aind_codeocean_api-0.5.0/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/doc_template/make.bat` & `aind_codeocean_api-0.5.0/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/doc_template/source/_static/dark-logo.svg` & `aind_codeocean_api-0.5.0/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/doc_template/source/_static/favicon.ico` & `aind_codeocean_api-0.5.0/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/doc_template/source/_static/light-logo.svg` & `aind_codeocean_api-0.5.0/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/doc_template/source/aind_codeocean_api.rst` & `aind_codeocean_api-0.5.0/doc_template/source/aind_codeocean_api.rst`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/doc_template/source/conf.py` & `aind_codeocean_api-0.5.0/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/integration/run_tests.py` & `aind_codeocean_api-0.5.0/integration/run_tests.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/pyproject.toml` & `aind_codeocean_api-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/src/aind_codeocean_api/codeocean.py` & `aind_codeocean_api-0.5.0/src/aind_codeocean_api/codeocean.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module to interface with Code Ocean's backend.
 """
 
 import json
 import logging
 from enum import Enum
 from inspect import signature
+from time import sleep
 from typing import Dict, List, Optional, Union
 
 import requests
 
 from aind_codeocean_api.credentials import CodeOceanCredentials
 from aind_codeocean_api.models.computations_requests import RunCapsuleRequest
 from aind_codeocean_api.models.data_assets_requests import (
@@ -196,26 +197,26 @@
             self.asset_url, params=query_params, auth=(self.token, "")
         )
 
         self.logger.info(response.url)
 
         return response
 
-    def search_all_data_assets(
+    def _paginate_data_assets(
         self,
         sort_order: Optional[str] = None,
         sort_field: Optional[str] = None,
         type: Optional[str] = None,
         ownership: Optional[str] = None,
         favorite: Optional[bool] = None,
         archived: Optional[bool] = None,
         query: Optional[str] = None,
-    ) -> requests.models.Response:
+    ):
         """
-        Utility method to return all the search results that match a query
+        Utility method to paginate through search results returned by search
         Parameters
         ----------
         sort_order : Optional[str]
             Determines the result sort order.
         sort_field : Optional[str]
             Determines the field to sort by.
         type : Optional[str]
@@ -228,58 +229,139 @@
         archived : Optional[bool]
             Search only archived data assets.
         query : Optional[str]
             Determines the search query.
 
         Returns
         -------
-        requests.models.Response
+        Iterator[List[dict]]
         """
 
-        # TODO: it'd be nice to re-use the search_data_assets function, but
-        #  it'll require passing in a requests.Session object into that method.
         frame_locals = locals()
         query_params = dict(
             [
                 (k, frame_locals[k])
                 for k, v in signature(
                     self.search_all_data_assets
                 ).parameters.items()
                 if frame_locals[k] is not None
             ]
         )
 
-        requests_session = requests.Session()
-        all_results = []
+        def get_page(
+            r: requests.Session,
+            qp: dict,
+            max_retries: int = 3,
+        ) -> dict:
+            """
+            Get a single list of results back from Code Ocean. It will retry
+            a request up to the max amount of retries. It will wait
+            min(retry_count**2, 15) seconds.
+            Parameters
+            ----------
+            r : requests.Session
+            qp : dict
+              query parameters
+            max_retries : int
+              Max number of retries before raising an error
+
+            Returns
+            -------
+            dict
+              Response from Code Ocean
+            """
+            rsp = r.get(self.asset_url, params=qp, auth=(self.token, ""))
+            if rsp.status_code == 200:
+                return rsp.json()
+            else:
+                retry = 1
+                while retry <= max_retries and rsp.status_code != 200:
+                    logging.debug(
+                        f"Backing off and retrying: {retry}. "
+                        f"Reason: {rsp.status_code}"
+                    )
+                    sleep(min(retry**2, 15))
+                    retry += 1
+                    rsp = r.get(
+                        self.asset_url, params=qp, auth=(self.token, "")
+                    )
+                if rsp.status_code == 200:
+                    return rsp.json()
+                else:
+                    raise ConnectionError(
+                        f"There was an error getting data from Code Ocean: "
+                        f"{rsp.status_code}"
+                    )
+
         with requests.Session() as requests_session:
             has_more = True
             status_code = 200
             start_index = 0
             limit = self._MAX_SEARCH_BATCH_REQUEST
-            while has_more and status_code == 200:
+            while has_more:
                 query_params[self._Fields.START.value] = start_index
                 query_params[self._Fields.LIMIT.value] = limit
-                response = requests_session.get(
-                    self.asset_url, params=query_params, auth=(self.token, "")
-                )
-
-                self.logger.info(response.url)
-
-                status_code = response.status_code
-                if status_code == 200:
-                    has_more = response.json()[self._Fields.HAS_MORE.value]
-                    response_results = response.json()[
-                        self._Fields.RESULTS.value
-                    ]
-                    num_of_results = len(response_results)
-                    all_results.extend(response_results)
-                    has_more = has_more if num_of_results > 0 else False
-                    start_index += num_of_results
-                else:
-                    return response
+                page = get_page(requests_session, query_params)
+                has_more = page.get(self._Fields.HAS_MORE.value)
+                results = page.get("results", [])
+                num_of_results = len(results)
+                has_more = has_more if num_of_results > 0 else False
+                start_index += num_of_results
+                yield results
+
+    def search_all_data_assets(
+        self,
+        sort_order: Optional[str] = None,
+        sort_field: Optional[str] = None,
+        type: Optional[str] = None,
+        ownership: Optional[str] = None,
+        favorite: Optional[bool] = None,
+        archived: Optional[bool] = None,
+        query: Optional[str] = None,
+    ) -> requests.models.Response:
+        """
+        Utility method to return all the search results that match a query
+        Parameters
+        ----------
+        sort_order : Optional[str]
+            Determines the result sort order.
+        sort_field : Optional[str]
+            Determines the field to sort by.
+        type : Optional[str]
+            Type of data asset: dataset or result.
+            Returns both if omitted.
+        ownership : Optional[str]
+            Search data asset by ownership: owner or shared.
+        favorite : Optional[bool]
+            Search only favorite data assets.
+        archived : Optional[bool]
+            Search only archived data assets.
+        query : Optional[str]
+            Determines the search query.
+
+        Returns
+        -------
+        requests.models.Response
+        """
+
+        # TODO: it'd be nice to re-use the search_data_assets function, but
+        #  it'll require passing in a requests.Session object into that method.
+
+        all_results = []
+
+        for page in self._paginate_data_assets(
+            sort_order=sort_order,
+            sort_field=sort_field,
+            type=type,
+            ownership=ownership,
+            favorite=favorite,
+            archived=archived,
+            query=query,
+        ):
+            all_results.extend(list(page))
 
         all_response = requests.Response()
         all_response.status_code = 200
         all_response._content = json.dumps({"results": all_results}).encode(
             "utf-8"
         )
         return all_response
```

### Comparing `aind_codeocean_api-0.4.3/src/aind_codeocean_api/credentials.py` & `aind_codeocean_api-0.5.0/src/aind_codeocean_api/credentials.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/basic_request.py` & `aind_codeocean_api-0.5.0/src/aind_codeocean_api/models/basic_request.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/computations_requests.py` & `aind_codeocean_api-0.5.0/src/aind_codeocean_api/models/computations_requests.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/src/aind_codeocean_api/models/data_assets_requests.py` & `aind_codeocean_api-0.5.0/src/aind_codeocean_api/models/data_assets_requests.py`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/PKG-INFO` & `aind_codeocean_api-0.5.0/src/aind_codeocean_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_codeocean_api
-Version: 0.4.3
+Version: 0.5.0
 Summary: CodeOcean API manager in Python
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_codeocean_api-0.4.3/src/aind_codeocean_api.egg-info/SOURCES.txt` & `aind_codeocean_api-0.5.0/src/aind_codeocean_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_codeocean_api-0.4.3/tests/test_codeocean_requests.py` & `aind_codeocean_api-0.5.0/tests/test_codeocean_requests.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,15 @@
                 status_code=200, content=success_message, url=url
             )
 
         def request_patch_response(url: str) -> MockResponse:
             """Mock a patch response"""
             success_message = map_input_to_success_message(url)
             return MockResponse(
-                status_code=202, content=success_message, url=url
+                status_code=204, content=success_message, url=url
             )
 
         def request_delete_response(url: str) -> MockResponse:
             """Mock a delete response"""
             success_message = map_input_to_success_message(url)
             return MockResponse(
                 status_code=204, content=success_message, url=url
@@ -503,47 +503,131 @@
                 {"id": "ghi789", "type": "result"},
                 {"id": "jkl101", "type": "result"},
             ]
         }
 
         actual_response = response.json()
 
-        bad_response = requests.Response()
-        bad_response.status_code = 500
-        bad_response._content = json.dumps(
-            {"message": "Internal Server Error"}
-        ).encode("utf-8")
-        mock_api_get.side_effect = [bad_response]
-        expected_bad_response = {"message": "Internal Server Error"}
-        response_bad = self.co_client.search_all_data_assets(archived=False)
-        actual_bad_response = response_bad.json()
-
         mock_api_get.assert_has_calls(
             [
                 call(
                     "https://acmecorp.codeocean.com/api/v1/data_assets",
                     params={"start": 2, "limit": 1000},
                     auth=("CODEOCEAN_API_TOKEN", ""),
                 ),
                 call(
                     "https://acmecorp.codeocean.com/api/v1/data_assets",
                     params={"start": 2, "limit": 1000},
                     auth=("CODEOCEAN_API_TOKEN", ""),
                 ),
-                call(
-                    "https://acmecorp.codeocean.com/api/v1/data_assets",
-                    params={"archived": False, "start": 0, "limit": 1000},
-                    auth=("CODEOCEAN_API_TOKEN", ""),
-                ),
             ]
         )
         self.assertEqual(200, response.status_code)
         self.assertEqual(expected_response, actual_response)
-        self.assertEqual(500, response_bad.status_code)
-        self.assertEqual(expected_bad_response, actual_bad_response)
+
+    @mock.patch("requests.Session.get")
+    @mock.patch("aind_codeocean_api.codeocean.sleep", return_value=None)
+    def test_search_all_data_assets_bad_response_max_retry_once(
+        self,
+        mock_sleep: unittest.mock.MagicMock,
+        mock_api_get: unittest.mock.MagicMock,
+    ) -> None:
+        """Tests search_all_data_assets method when a bad response is
+        returned once and then a good response is returned."""
+
+        mocked_response1 = requests.Response()
+        mocked_response1.status_code = 200
+        mocked_response1._content = json.dumps(
+            {
+                "has_more": True,
+                "results": [
+                    {"id": "abc123", "type": "dataset"},
+                    {"id": "def456", "type": "result"},
+                ],
+            }
+        ).encode("utf-8")
+
+        mocked_response2 = requests.Response()
+        mocked_response2.status_code = 200
+        mocked_response2._content = json.dumps(
+            {
+                "has_more": False,
+                "results": [
+                    {"id": "ghi789", "type": "result"},
+                    {"id": "jkl101", "type": "result"},
+                ],
+            }
+        ).encode("utf-8")
+
+        bad_response = requests.Response()
+        bad_response.status_code = 500
+        bad_response._content = json.dumps(
+            {"message": "Internal Server Error"}
+        ).encode("utf-8")
+
+        mock_api_get.side_effect = [
+            mocked_response1,
+            bad_response,
+            mocked_response2,
+        ]
+        expected_response = {
+            "results": [
+                {"id": "abc123", "type": "dataset"},
+                {"id": "def456", "type": "result"},
+                {"id": "ghi789", "type": "result"},
+                {"id": "jkl101", "type": "result"},
+            ]
+        }
+        response = self.co_client.search_all_data_assets()
+        actual_response = response.json()
+        self.assertEqual(expected_response, actual_response)
+        mock_sleep.assert_has_calls([call(1)])
+
+    @mock.patch("requests.Session.get")
+    @mock.patch("aind_codeocean_api.codeocean.sleep", return_value=None)
+    def test_search_all_data_assets_bad_response_max_retries(
+        self,
+        mock_sleep: unittest.mock.MagicMock,
+        mock_api_get: unittest.mock.MagicMock,
+    ) -> None:
+        """Tests search_all_data_assets method when a bad response is
+        returned."""
+
+        mocked_response1 = requests.Response()
+        mocked_response1.status_code = 200
+        mocked_response1._content = json.dumps(
+            {
+                "has_more": True,
+                "results": [
+                    {"id": "abc123", "type": "dataset"},
+                    {"id": "def456", "type": "result"},
+                ],
+            }
+        ).encode("utf-8")
+
+        bad_response = requests.Response()
+        bad_response.status_code = 500
+        bad_response._content = json.dumps(
+            {"message": "Internal Server Error"}
+        ).encode("utf-8")
+
+        mock_api_get.side_effect = [
+            mocked_response1,
+            bad_response,
+            bad_response,
+            bad_response,
+            bad_response,
+        ]
+        with self.assertRaises(ConnectionError) as e:
+            self.co_client.search_all_data_assets()
+        self.assertEqual(
+            "There was an error getting data from Code Ocean: 500",
+            e.exception.args[0],
+        )
+        mock_sleep.assert_has_calls([call(1), call(4), call(9)])
 
     @mock.patch("requests.put")
     def test_update_data_asset(
         self, mock_api_put: unittest.mock.MagicMock
     ) -> None:
         """Tests update_data_asset_method"""
 
@@ -945,20 +1029,20 @@
         """Tests the response of updating permissions"""
 
         def mock_success_response() -> Callable[..., MockResponse]:
             """Mock a successful response"""
 
             def request_post_response(json: dict) -> MockResponse:
                 """Mock a post response"""
-                return MockResponse(status_code=204, content=None, url="")
+                return MockResponse(status_code=204, content={}, url="")
 
             return request_post_response
 
-        users = ([{"email": "user2@email.com", "role": "viewer"}],)
-        groups = ([{"group": "group4", "role": "viewer"}],)
+        users = [{"email": "user2@email.com", "role": "viewer"}]
+        groups = [{"group": "group4", "role": "viewer"}]
         everyone = "viewer"
 
         example_data_asset_id = "648473aa-791e-4372-bd25-205cc587ec56"
         input_json_data = {
             "data_asset_id": example_data_asset_id,
             "users": users,
             "groups": groups,
@@ -983,20 +1067,20 @@
         """Tests the response of updating permissions"""
 
         def mock_success_response() -> Callable[..., MockResponse]:
             """Mock a success response"""
 
             def request_post_response(json: dict) -> MockResponse:
                 """Mock a post response"""
-                return MockResponse(status_code=204, content=None, url="")
+                return MockResponse(status_code=204, content={}, url="")
 
             return request_post_response
 
-        users = ([{"email": "user2@email.com", "role": "viewer"}],)
-        groups = ([{"group": "group4", "role": "viewer"}],)
+        users: List[dict] = [{"email": "user2@email.com", "role": "viewer"}]
+        groups: List[dict] = [{"group": "group4", "role": "viewer"}]
 
         example_data_asset_id = "648473aa-791e-4372-bd25-205cc587ec56"
         input_json_data = {
             "data_asset_id": example_data_asset_id,
             "users": users,
             "groups": groups,
         }
@@ -1013,15 +1097,15 @@
     def test_archive_data_asset(
         self, mock_api_patch: unittest.mock.MagicMock
     ) -> None:
         """Tests the response of archiving a data asset"""
 
         def map_to_success_message(_) -> dict:
             """Map to a success message"""
-            return ""
+            return {}
 
         mocked_success_patch = self.mock_success_response(
             map_to_success_message, req_type="patch"
         )
 
         example_data_asset_id = "da8dd108-2a10-471d-82b9-1e671b107bf8"
         expected_url = (
@@ -1032,25 +1116,25 @@
         mock_api_patch.return_value = mocked_success_patch(url=expected_url)
 
         response = self.co_client.archive_data_asset(
             data_asset_id=example_data_asset_id, archive=True
         )
 
         self.assertEqual(response.url, expected_url)
-        self.assertEqual(response.status_code, 202)
+        self.assertEqual(response.status_code, 204)
 
     @mock.patch("requests.delete")
     def test_delete_data_asset(
         self, mock_api_delete: unittest.mock.MagicMock
     ) -> None:
         """Tests the response of deleting a data asset"""
 
         def map_to_success_message(_) -> dict:
             """Map to a success message"""
-            return ""
+            return {}
 
         mocked_success_delete = self.mock_success_response(
             map_to_success_message, req_type="delete"
         )
 
         example_data_asset_id = "da8dd108-2a10-471d-82b9-1e671b107bf8"
         expected_url = f"{self.co_client.asset_url}/{example_data_asset_id}"
```

### Comparing `aind_codeocean_api-0.4.3/tests/test_credentials.py` & `aind_codeocean_api-0.5.0/tests/test_credentials.py`

 * *Files identical despite different names*

