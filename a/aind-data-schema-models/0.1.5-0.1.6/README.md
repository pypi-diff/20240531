# Comparing `tmp/aind_data_schema_models-0.1.5.tar.gz` & `tmp/aind_data_schema_models-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_data_schema_models-0.1.5.tar", last modified: Sat May 18 16:31:08 2024, max compression
+gzip compressed data, was "aind_data_schema_models-0.1.6.tar", last modified: Thu May 30 22:59:58 2024, max compression
```

## Comparing `aind_data_schema_models-0.1.5.tar` & `aind_data_schema_models-0.1.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:31:08.339160 aind_data_schema_models-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:31:08.327160 aind_data_schema_models-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:31:08.331160 aind_data_schema_models-0.1.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:31:08.331160 aind_data_schema_models-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/.github/workflows/test_and_lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-18 16:31:08.339160 aind_data_schema_models-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:31:08.331160 aind_data_schema_models-0.1.5/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:31:08.331160 aind_data_schema_models-0.1.5/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:31:08.335160 aind_data_schema_models-0.1.5/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 16:31:08.339160 aind_data_schema_models-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:31:08.331160 aind_data_schema_models-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:31:08.335160 aind_data_schema_models-0.1.5/src/aind_data_schema_models/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models/data_name_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models/harp_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models/modalities.py
--rw-r--r--   0 runner    (1001) docker     (127)    28864 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models/pid_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models/platforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models/process_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models/species.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models/specimen_procedure_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:31:08.339160 aind_data_schema_models-0.1.5/src/aind_data_schema_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-18 16:31:08.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-18 16:31:08.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 16:31:08.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-18 16:31:08.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-18 16:31:08.000000 aind_data_schema_models-0.1.5/src/aind_data_schema_models.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:31:08.339160 aind_data_schema_models-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/tests/test_data_name_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/tests/test_modalities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/tests/test_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/tests/test_process_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/tests/test_specimen_procedure_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-18 16:30:58.000000 aind_data_schema_models-0.1.5/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:59:58.581301 aind_data_schema_models-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:59:58.573301 aind_data_schema_models-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:59:58.573301 aind_data_schema_models-0.1.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:59:58.573301 aind_data_schema_models-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/.github/workflows/test_and_lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-30 22:59:58.581301 aind_data_schema_models-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4634 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:59:58.573301 aind_data_schema_models-0.1.6/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:59:58.573301 aind_data_schema_models-0.1.6/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:59:58.577301 aind_data_schema_models-0.1.6/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 22:59:58.581301 aind_data_schema_models-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:59:58.573301 aind_data_schema_models-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:59:58.577301 aind_data_schema_models-0.1.6/src/aind_data_schema_models/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models/data_name_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models/harp_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models/modalities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29679 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models/pid_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models/process_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models/specimen_procedure_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:59:58.581301 aind_data_schema_models-0.1.6/src/aind_data_schema_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-30 22:59:58.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-30 22:59:58.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 22:59:58.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-30 22:59:58.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 22:59:58.000000 aind_data_schema_models-0.1.6/src/aind_data_schema_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:59:58.581301 aind_data_schema_models-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/tests/test_data_name_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/tests/test_modalities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/tests/test_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/tests/test_process_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/tests/test_specimen_procedure_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-30 22:59:48.000000 aind_data_schema_models-0.1.6/tests/test_units.py
```

### Comparing `aind_data_schema_models-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_data_schema_models-0.1.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_data_schema_models-0.1.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/.github/ISSUE_TEMPLATE/user-story.md` & `aind_data_schema_models-0.1.6/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/.github/workflows/tag_and_publish.yml` & `aind_data_schema_models-0.1.6/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/.github/workflows/test_and_lint.yml` & `aind_data_schema_models-0.1.6/.github/workflows/test_and_lint.yml`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/.gitignore` & `aind_data_schema_models-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/LICENSE` & `aind_data_schema_models-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/PKG-INFO` & `aind_data_schema_models-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-data-schema-models
-Version: 0.1.5
+Version: 0.1.6
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_data_schema_models-0.1.5/README.md` & `aind_data_schema_models-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/doc_template/Makefile` & `aind_data_schema_models-0.1.6/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/doc_template/make.bat` & `aind_data_schema_models-0.1.6/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/doc_template/source/_static/dark-logo.svg` & `aind_data_schema_models-0.1.6/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/doc_template/source/_static/favicon.ico` & `aind_data_schema_models-0.1.6/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/doc_template/source/_static/light-logo.svg` & `aind_data_schema_models-0.1.6/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/doc_template/source/conf.py` & `aind_data_schema_models-0.1.6/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/pyproject.toml` & `aind_data_schema_models-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/src/aind_data_schema_models/data_name_patterns.py` & `aind_data_schema_models-0.1.6/src/aind_data_schema_models/data_name_patterns.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/src/aind_data_schema_models/harp_types.py` & `aind_data_schema_models-0.1.6/src/aind_data_schema_models/harp_types.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/src/aind_data_schema_models/modalities.py` & `aind_data_schema_models-0.1.6/src/aind_data_schema_models/modalities.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/src/aind_data_schema_models/organizations.py` & `aind_data_schema_models-0.1.6/src/aind_data_schema_models/organizations.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,23 @@
 
     name: Literal["Abcam"] = "Abcam"
     abbreviation: Literal[None] = Field(None)
     registry: Annotated[Union[ResearchOrganizationRegistry], Field(default=Registry.ROR, discriminator="name")]
     registry_identifier: Literal["02e1wjw63"] = "02e1wjw63"
 
 
+class Addgene(_Organization):
+    """Addgene"""
+
+    name: Literal["Addgene"] = "Addgene"
+    abbreviation: Literal[None] = Field(None)
+    registry: Annotated[Union[ResearchOrganizationRegistry], Field(default=Registry.ROR, discriminator="name")]
+    registry_identifier: Literal["01nn1pw54"] = "01nn1pw54"
+
+
 class AilipuTechnologyCo(_Organization):
     """AilipuTechnologyCo"""
 
     name: Literal["Ailipu Technology Co"] = "Ailipu Technology Co"
     abbreviation: Literal[None] = Field(None)
     registry: Literal[None] = Field(None)
     registry_identifier: Literal[None] = Field(None)
@@ -335,14 +344,23 @@
 
     name: Literal["Jackson Laboratory"] = "Jackson Laboratory"
     abbreviation: Literal["JAX"] = "JAX"
     registry: Annotated[Union[ResearchOrganizationRegistry], Field(default=Registry.ROR, discriminator="name")]
     registry_identifier: Literal["021sy4w91"] = "021sy4w91"
 
 
+class JaneliaResearchCampus(_Organization):
+    """JaneliaResearchCampus"""
+
+    name: Literal["Janelia Research Campus"] = "Janelia Research Campus"
+    abbreviation: Literal["Janelia"] = "Janelia"
+    registry: Annotated[Union[ResearchOrganizationRegistry], Field(default=Registry.ROR, discriminator="name")]
+    registry_identifier: Literal["013sk6x84"] = "013sk6x84"
+
+
 class Julabo(_Organization):
     """Julabo"""
 
     name: Literal["Julabo"] = "Julabo"
     abbreviation: Literal[None] = Field(None)
     registry: Literal[None] = Field(None)
     registry_identifier: Literal[None] = Field(None)
@@ -720,14 +738,15 @@
 
 
 class Organization:
     """Organization definitions"""
 
     AA_OPTO = AAOptoElectronic()
     ABCAM = Abcam()
+    ADDGENE = Addgene()
     AILIPU = AilipuTechnologyCo()
     AI = AllenInstitute()
     AIBS = AllenInstituteForBrainScience()
     AIND = AllenInstituteForNeuralDynamics()
     ALLIED = Allied()
     ASI = AppliedScientificInstrumentation()
     ASUS = Asus()
@@ -753,14 +772,15 @@
     HUST = HuazhongUniversityOfScienceAndTechnology()
     IMAGING_SOURCE = TheImagingSource()
     IMEC = InteruniversityMicroelectronicsCenter()
     INFINITY_PHOTO_OPTICAL = InfinityPhotoOptical()
     INVITROGEN = Invitrogen()
     ISL = ISLProductsInternational()
     JAX = JacksonLaboratory()
+    JANELIA = JaneliaResearchCampus()
     JULABO = Julabo()
     LEE = TheLeeCompany()
     LEICA = Leica()
     LG = Lg()
     LIFECANVAS = LifeCanvas()
     MEADOWLARK = MeadowlarkOptics()
     MIDOPT = MidwestOpticalSystems()
@@ -893,23 +913,25 @@
     ]
     RESEARCH_INSTITUTIONS = Annotated[
         Union[
             AllenInstituteForBrainScience,
             AllenInstituteForNeuralDynamics,
             ColumbiaUniversity,
             HuazhongUniversityOfScienceAndTechnology,
+            JaneliaResearchCampus,
             NewYorkUniversity,
             Other,
         ],
         Field(discriminator="name"),
     ]
     SUBJECT_SOURCES = Annotated[
         Union[
             AllenInstitute,
             ColumbiaUniversity,
             HuazhongUniversityOfScienceAndTechnology,
+            JaneliaResearchCampus,
             JacksonLaboratory,
             NewYorkUniversity,
             Other,
         ],
         Field(discriminator="name"),
     ]
```

### Comparing `aind_data_schema_models-0.1.5/src/aind_data_schema_models/pid_names.py` & `aind_data_schema_models-0.1.6/src/aind_data_schema_models/pid_names.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/src/aind_data_schema_models/platforms.py` & `aind_data_schema_models-0.1.6/src/aind_data_schema_models/platforms.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/src/aind_data_schema_models/process_names.py` & `aind_data_schema_models-0.1.6/src/aind_data_schema_models/process_names.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/src/aind_data_schema_models/registry.py` & `aind_data_schema_models-0.1.6/src/aind_data_schema_models/registry.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/src/aind_data_schema_models/species.py` & `aind_data_schema_models-0.1.6/src/aind_data_schema_models/species.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/src/aind_data_schema_models/specimen_procedure_types.py` & `aind_data_schema_models-0.1.6/src/aind_data_schema_models/specimen_procedure_types.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/src/aind_data_schema_models/units.py` & `aind_data_schema_models-0.1.6/src/aind_data_schema_models/units.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/src/aind_data_schema_models.egg-info/PKG-INFO` & `aind_data_schema_models-0.1.6/src/aind_data_schema_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind-data-schema-models
-Version: 0.1.5
+Version: 0.1.6
 Summary: Generated from aind-library-template
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_data_schema_models-0.1.5/src/aind_data_schema_models.egg-info/SOURCES.txt` & `aind_data_schema_models-0.1.6/src/aind_data_schema_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/tests/test_data_name_patterns.py` & `aind_data_schema_models-0.1.6/tests/test_data_name_patterns.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/tests/test_models.py` & `aind_data_schema_models-0.1.6/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aind_data_schema_models-0.1.5/tests/test_units.py` & `aind_data_schema_models-0.1.6/tests/test_units.py`

 * *Files identical despite different names*

