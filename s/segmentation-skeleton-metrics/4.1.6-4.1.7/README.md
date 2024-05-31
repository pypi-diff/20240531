# Comparing `tmp/segmentation_skeleton_metrics-4.1.6.tar.gz` & `tmp/segmentation_skeleton_metrics-4.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmentation_skeleton_metrics-4.1.6.tar", last modified: Sat May  4 00:04:45 2024, max compression
+gzip compressed data, was "segmentation_skeleton_metrics-4.1.7.tar", last modified: Fri May 31 18:44:26 2024, max compression
```

## Comparing `segmentation_skeleton_metrics-4.1.6.tar` & `segmentation_skeleton_metrics-4.1.7.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:04:45.733333 segmentation_skeleton_metrics-4.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:04:45.701332 segmentation_skeleton_metrics-4.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:04:45.701332 segmentation_skeleton_metrics-4.1.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:04:45.701332 segmentation_skeleton_metrics-4.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-04 00:04:45.733333 segmentation_skeleton_metrics-4.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:04:45.705332 segmentation_skeleton_metrics-4.1.6/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:04:45.705332 segmentation_skeleton_metrics-4.1.6/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:04:45.705332 segmentation_skeleton_metrics-4.1.6/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:04:45.717332 segmentation_skeleton_metrics-4.1.6/resources/
--rw-r--r--   0 runner    (1001) docker     (127)  9596734 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/resources/pred_labels.tif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:04:45.729333 segmentation_skeleton_metrics-4.1.6/resources/target_graphs/
--rw-r--r--   0 runner    (1001) docker     (127)    72420 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/resources/target_graphs/0.swc
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/resources/target_graphs/1.swc
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/resources/target_graphs/2.swc
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/resources/target_graphs/3.swc
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/resources/target_graphs/4.swc
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/resources/target_graphs/5.swc
--rw-r--r--   0 runner    (1001) docker     (127)  9602600 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/resources/target_labels.tif
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 00:04:45.733333 segmentation_skeleton_metrics-4.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:04:45.701332 segmentation_skeleton_metrics-4.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:04:45.729333 segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-04 00:04:31.000000 segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics/merge_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    28825 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics/skeleton_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics/split_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics/swc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:04:45.733333 segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-04 00:04:45.000000 segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-04 00:04:45.000000 segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:04:45.000000 segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-04 00:04:45.000000 segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-04 00:04:45.000000 segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:04:45.733333 segmentation_skeleton_metrics-4.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-04 00:04:30.000000 segmentation_skeleton_metrics-4.1.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.749428 segmentation_skeleton_metrics-4.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.713427 segmentation_skeleton_metrics-4.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.717427 segmentation_skeleton_metrics-4.1.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.717427 segmentation_skeleton_metrics-4.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-31 18:44:26.749428 segmentation_skeleton_metrics-4.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.717427 segmentation_skeleton_metrics-4.1.7/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.717427 segmentation_skeleton_metrics-4.1.7/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.717427 segmentation_skeleton_metrics-4.1.7/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.729427 segmentation_skeleton_metrics-4.1.7/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)  9596734 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/pred_labels.tif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.741428 segmentation_skeleton_metrics-4.1.7/resources/target_graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)    72420 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/target_graphs/0.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/target_graphs/1.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/target_graphs/2.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/target_graphs/3.swc
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/target_graphs/4.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/target_graphs/5.swc
+-rw-r--r--   0 runner    (1001) docker     (127)  9602600 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/target_labels.tif
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:44:26.749428 segmentation_skeleton_metrics-4.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.713427 segmentation_skeleton_metrics-4.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.745427 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-31 18:44:16.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/merge_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29165 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/skeleton_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/split_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/swc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.745427 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-31 18:44:26.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-31 18:44:26.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:44:26.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-31 18:44:26.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-31 18:44:26.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.745427 segmentation_skeleton_metrics-4.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/tests/__init__.py
```

### Comparing `segmentation_skeleton_metrics-4.1.6/.github/ISSUE_TEMPLATE/bug_report.md` & `segmentation_skeleton_metrics-4.1.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/.github/ISSUE_TEMPLATE/feature_request.md` & `segmentation_skeleton_metrics-4.1.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/.github/ISSUE_TEMPLATE/user-story.md` & `segmentation_skeleton_metrics-4.1.7/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/.github/workflows/lint_and_test.yml` & `segmentation_skeleton_metrics-4.1.7/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/.github/workflows/tag_and_publish.yml` & `segmentation_skeleton_metrics-4.1.7/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/.gitignore` & `segmentation_skeleton_metrics-4.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/LICENSE` & `segmentation_skeleton_metrics-4.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/PKG-INFO` & `segmentation_skeleton_metrics-4.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation_skeleton_metrics
-Version: 4.1.6
+Version: 4.1.7
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `segmentation_skeleton_metrics-4.1.6/README.md` & `segmentation_skeleton_metrics-4.1.7/README.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/doc_template/Makefile` & `segmentation_skeleton_metrics-4.1.7/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/doc_template/make.bat` & `segmentation_skeleton_metrics-4.1.7/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/doc_template/source/_static/dark-logo.svg` & `segmentation_skeleton_metrics-4.1.7/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/doc_template/source/_static/favicon.ico` & `segmentation_skeleton_metrics-4.1.7/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/doc_template/source/_static/light-logo.svg` & `segmentation_skeleton_metrics-4.1.7/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/doc_template/source/conf.py` & `segmentation_skeleton_metrics-4.1.7/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/pyproject.toml` & `segmentation_skeleton_metrics-4.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/resources/pred_labels.tif` & `segmentation_skeleton_metrics-4.1.7/resources/pred_labels.tif`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/resources/target_graphs/0.swc` & `segmentation_skeleton_metrics-4.1.7/resources/target_graphs/0.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/resources/target_graphs/1.swc` & `segmentation_skeleton_metrics-4.1.7/resources/target_graphs/1.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/resources/target_graphs/2.swc` & `segmentation_skeleton_metrics-4.1.7/resources/target_graphs/2.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/resources/target_graphs/3.swc` & `segmentation_skeleton_metrics-4.1.7/resources/target_graphs/3.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/resources/target_graphs/4.swc` & `segmentation_skeleton_metrics-4.1.7/resources/target_graphs/4.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/resources/target_graphs/5.swc` & `segmentation_skeleton_metrics-4.1.7/resources/target_graphs/5.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/resources/target_labels.tif` & `segmentation_skeleton_metrics-4.1.7/resources/target_labels.tif`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics/graph_utils.py` & `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/graph_utils.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics/merge_detection.py` & `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/merge_detection.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics/skeleton_metric.py` & `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/skeleton_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,18 +113,17 @@
         self.save = save_swc
 
         self.init_black_holes(black_holes_xyz_id)
         self.black_hole_radius = black_hole_radius
 
         # Labels
         self.label_mask = pred_labels
-        self.valid_labels = None
-        # swc_utils.parse(
-        #      pred_swc_paths, valid_size_threshold, anisotropy
-        # )
+        self.valid_labels = swc_utils.parse(
+            pred_swc_paths, valid_size_threshold, anisotropy
+        )
         self.init_equiv_labels(connections_path)
 
         # Build Graphs
         self.graphs = self.init_graphs(target_swc_paths, anisotropy)
         self.init_labeled_graphs()
 
         # Build kdtree
@@ -210,15 +209,15 @@
         Parameters
         ----------
         graph : networkx.Graph
             Graph that represents a neuron from the ground truth.
 
         Returns
         -------
-        graph : networkx.Graph
+        networkx.Graph
             Updated graph with node-level attributes called "label".
 
         """
         labeled_graph = nx.Graph(graph)
         id_to_label_nodes = dict()
         with ThreadPoolExecutor() as executor:
             # Assign threads
@@ -318,15 +317,15 @@
         Parameters
         ----------
         label : int
             Label to be validated.
 
         Returns
         -------
-        label : int
+        int
             There are two possibilities: (1) original label if either "label"
             is contained in "self.valid_labels" or "self.valid_labels" is
             None, or (2) 0 if "label" is not contained in self.valid_labels.
 
         """
         if self.valid_labels:
             return 0 if label not in self.valid_labels.keys() else label
@@ -379,15 +378,15 @@
         xyz : tuple
             xyz coordinate to be queried.
 
         Returns
         -------
         tuple
             xyz coordinate of the nearest neighbor of "xyz".
-        d : float
+        float
             Projection distance.
 
         """
         d, idx = self.graphs_kdtree.query(xyz, k=1)
         return tuple(self.graphs_kdtree.data[idx]), d
 
     def init_black_holes(self, black_holes):
@@ -455,29 +454,47 @@
         self.quantify_merges()
 
         # Compute metrics
         full_results, avg_results = self.compile_results()
         return full_results, avg_results
 
     def get_all_labels(self):
+        """
+        Gets the set of all labels belonging to nodes across all graphs in
+        "self.graphs", except the label 0 is discarded.
+
+        Parameters
+        ----------
+        None
+
+        Returns
+        -------
+        set
+            Labels belonging to nodes across all graphs in "self.graphs"
+        
+        """
         labels = set()
         for id in self.graphs.keys():
             labels = labels.union(self.get_labels(id))
         labels.discard(0)
         return labels
 
     def get_labels(self, id):
         """
-        Gets the predicted label ids that intersect with the target graph
+        Gets the predicted labels that intersect with the target graph
         corresponding to "id".
 
         Parameters
         ----------
         id : str
 
+        Returns
+        -------
+        set
+            Labels that intersect with the target graph corresponding to "id".
         """
         return set(self.id_to_label_nodes[id].keys())
 
     def zero_nodes(self, id, label):
         """
         Zeros out nodes in "self.labeled_graph[id]" in the sense that
         nodes with "label" are updated to zero.
@@ -649,15 +666,15 @@
         Parameters
         ----------
         xyz : numpy.ndarray
             xyz coordinate to be checked
 
         Returns
         -------
-        near_bdd_bool : bool
+        bool
             Indication of whether "xyz" is near the boundary of the image.
 
         """
         near_bdd_bool = False
         if self.ignore_boundary_mistakes:
             mask_shape = self.label_mask.shape
             above = [xyz[i] >= mask_shape[i] - 32 for i in range(3)]
@@ -695,17 +712,17 @@
         """
         Once a merge has been detected that corresponds to "id", every
         node in "self.labeled_graph[id]" with that "label" is
         deleted.
 
         Parameters
         ----------
-        id : str
+        str
             Key associated with the labeled_graph to be searched.
-        label : int
+        int
             Label in prediction that is assocatied with a merge.
 
         Returns
         -------
         None
 
         """
@@ -740,18 +757,18 @@
 
         Parameters
         ----------
         None
 
         Returns
         -------
-        full_results : dict
+        dict
             Dictionary where the keys are ids and the values are the
             result of computing each metric for the corresponding graphs.
-        avg_result : dict
+        dict
             Dictionary where the keys are names of metrics computed by this
             module and values are the averaged result over all ids.
 
         """
         # Compute remaining metrics
         self.compute_edge_accuracy()
         self.compute_erl()
@@ -777,17 +794,17 @@
 
         Parameters
         ----------
         None
 
         Results
         -------
-        grids : list[str]
+        list[str]
             Specifies the ordering of results for each value in "stats".
-        stats : dict
+        dict
             Dictionary where the keys are metrics and values are the result of
             computing that metric for each graph in labeled_graphs.
 
         """
         ids = list(self.labeled_graphs.keys())
         ids.sort()
         stats = {
@@ -879,16 +896,16 @@
 
         Parameters
         ----------
         None
 
         Returns
         -------
-        metrics : list[str]
-            List of metrics computed by this module.
+        list[str]
+            Metrics computed by this module.
 
         """
         metrics = [
             "# splits",
             "# merges",
             "% omit",
             "% merged",
```

### Comparing `segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics/split_detection.py` & `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/split_detection.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics/swc_utils.py` & `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/swc_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,14 @@
     print("Downloading predicted swc files from cloud...")
     print("# zip files:", len(zip_paths))
     for i, path in enumerate(zip_paths):
         valid_labels.update(download(bucket, path, min_size, anisotropy))
         if i > cnt * chunk_size:
             utils.progress_bar(i + 1, len(zip_paths))
             cnt += 1
-        break
 
     # Report Results
     print("\n#Valid Labels:", len(valid_labels))
     print("")
     return valid_labels
```

### Comparing `segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics/utils.py` & `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics.egg-info/PKG-INFO` & `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segmentation_skeleton_metrics
-Version: 4.1.6
+Version: 4.1.7
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `segmentation_skeleton_metrics-4.1.6/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt` & `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

