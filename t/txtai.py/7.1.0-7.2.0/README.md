# Comparing `tmp/txtai.py-7.1.0.tar.gz` & `tmp/txtai.py-7.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "txtai.py-7.1.0.tar", last modified: Fri Apr 19 15:05:33 2024, max compression
+gzip compressed data, was "txtai.py-7.2.0.tar", last modified: Fri May 31 15:17:40 2024, max compression
```

## Comparing `txtai.py-7.1.0.tar` & `txtai.py-7.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 15:05:33.736921 txtai.py-7.1.0/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    10754 2023-12-17 14:57:29.000000 txtai.py-7.1.0/LICENSE
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3438 2024-04-19 15:05:33.735921 txtai.py-7.1.0/PKG-INFO
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2524 2023-12-22 16:12:16.000000 txtai.py-7.1.0/README.md
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       31 2023-12-17 14:57:37.000000 txtai.py-7.1.0/pyproject.toml
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       38 2024-04-19 15:05:33.736921 txtai.py-7.1.0/setup.cfg
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1352 2024-04-19 15:02:19.000000 txtai.py-7.1.0/setup.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 15:05:33.734921 txtai.py-7.1.0/src/
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 15:05:33.734921 txtai.py-7.1.0/src/python/
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 15:05:33.735921 txtai.py-7.1.0/src/python/txtai/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        0 2023-12-17 14:57:01.000000 txtai.py-7.1.0/src/python/txtai/__init__.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 15:05:33.735921 txtai.py-7.1.0/src/python/txtai/client/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      388 2023-12-22 15:42:41.000000 txtai.py-7.1.0/src/python/txtai/client/__init__.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3063 2023-12-26 16:31:53.000000 txtai.py-7.1.0/src/python/txtai/client/api.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4875 2023-12-17 17:20:58.000000 txtai.py-7.1.0/src/python/txtai/client/embeddings.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      516 2023-12-22 16:20:42.000000 txtai.py-7.1.0/src/python/txtai/client/extractor.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1112 2023-12-22 16:26:04.000000 txtai.py-7.1.0/src/python/txtai/client/labels.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      655 2023-12-22 16:25:50.000000 txtai.py-7.1.0/src/python/txtai/client/segmentation.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1108 2023-12-22 16:25:45.000000 txtai.py-7.1.0/src/python/txtai/client/similarity.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1259 2023-12-22 16:26:49.000000 txtai.py-7.1.0/src/python/txtai/client/summary.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      657 2023-12-22 16:32:38.000000 txtai.py-7.1.0/src/python/txtai/client/textractor.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      670 2023-12-22 16:28:54.000000 txtai.py-7.1.0/src/python/txtai/client/transcription.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1316 2023-12-22 16:29:56.000000 txtai.py-7.1.0/src/python/txtai/client/translation.py
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      486 2023-12-22 16:30:43.000000 txtai.py-7.1.0/src/python/txtai/client/workflow.py
-drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-04-19 15:05:33.735921 txtai.py-7.1.0/src/python/txtai.py.egg-info/
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3438 2024-04-19 15:05:33.000000 txtai.py-7.1.0/src/python/txtai.py.egg-info/PKG-INFO
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      727 2024-04-19 15:05:33.000000 txtai.py-7.1.0/src/python/txtai.py.egg-info/SOURCES.txt
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        1 2024-04-19 15:05:33.000000 txtai.py-7.1.0/src/python/txtai.py.egg-info/dependency_links.txt
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       15 2024-04-19 15:05:33.000000 txtai.py-7.1.0/src/python/txtai.py.egg-info/requires.txt
--rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        6 2024-04-19 15:05:33.000000 txtai.py-7.1.0/src/python/txtai.py.egg-info/top_level.txt
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 15:17:40.863525 txtai.py-7.2.0/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)    10754 2023-12-17 14:57:29.000000 txtai.py-7.2.0/LICENSE
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3438 2024-05-31 15:17:40.862526 txtai.py-7.2.0/PKG-INFO
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     2524 2023-12-22 16:12:16.000000 txtai.py-7.2.0/README.md
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       31 2023-12-17 14:57:37.000000 txtai.py-7.2.0/pyproject.toml
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       38 2024-05-31 15:17:40.863525 txtai.py-7.2.0/setup.cfg
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1352 2024-05-31 15:13:26.000000 txtai.py-7.2.0/setup.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 15:17:40.861526 txtai.py-7.2.0/src/
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 15:17:40.861526 txtai.py-7.2.0/src/python/
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 15:17:40.862526 txtai.py-7.2.0/src/python/txtai/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        0 2023-12-17 14:57:01.000000 txtai.py-7.2.0/src/python/txtai/__init__.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 15:17:40.862526 txtai.py-7.2.0/src/python/txtai/client/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      388 2023-12-22 15:42:41.000000 txtai.py-7.2.0/src/python/txtai/client/__init__.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3063 2023-12-26 16:31:53.000000 txtai.py-7.2.0/src/python/txtai/client/api.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     4875 2023-12-17 17:20:58.000000 txtai.py-7.2.0/src/python/txtai/client/embeddings.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      516 2023-12-22 16:20:42.000000 txtai.py-7.2.0/src/python/txtai/client/extractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1112 2023-12-22 16:26:04.000000 txtai.py-7.2.0/src/python/txtai/client/labels.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      655 2023-12-22 16:25:50.000000 txtai.py-7.2.0/src/python/txtai/client/segmentation.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1108 2023-12-22 16:25:45.000000 txtai.py-7.2.0/src/python/txtai/client/similarity.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1259 2023-12-22 16:26:49.000000 txtai.py-7.2.0/src/python/txtai/client/summary.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      657 2023-12-22 16:32:38.000000 txtai.py-7.2.0/src/python/txtai/client/textractor.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      670 2023-12-22 16:28:54.000000 txtai.py-7.2.0/src/python/txtai/client/transcription.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     1316 2023-12-22 16:29:56.000000 txtai.py-7.2.0/src/python/txtai/client/translation.py
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      486 2023-12-22 16:30:43.000000 txtai.py-7.2.0/src/python/txtai/client/workflow.py
+drwxr-xr-x   0 dmezzett  (1000) dmezzett  (1000)        0 2024-05-31 15:17:40.862526 txtai.py-7.2.0/src/python/txtai.py.egg-info/
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)     3438 2024-05-31 15:17:40.000000 txtai.py-7.2.0/src/python/txtai.py.egg-info/PKG-INFO
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)      727 2024-05-31 15:17:40.000000 txtai.py-7.2.0/src/python/txtai.py.egg-info/SOURCES.txt
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        1 2024-05-31 15:17:40.000000 txtai.py-7.2.0/src/python/txtai.py.egg-info/dependency_links.txt
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)       15 2024-05-31 15:17:40.000000 txtai.py-7.2.0/src/python/txtai.py.egg-info/requires.txt
+-rw-r--r--   0 dmezzett  (1000) dmezzett  (1000)        6 2024-05-31 15:17:40.000000 txtai.py-7.2.0/src/python/txtai.py.egg-info/top_level.txt
```

### Comparing `txtai.py-7.1.0/LICENSE` & `txtai.py-7.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `txtai.py-7.1.0/PKG-INFO` & `txtai.py-7.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txtai.py
-Version: 7.1.0
+Version: 7.2.0
 Summary: Python client for txtai
 Home-page: https://github.com/neuml/txtai.py
 Author: NeuML
 License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/neuml/txtai.py
 Project-URL: Issue Tracker, https://github.com/neuml/txtai.py/issues
 Project-URL: Source Code, https://github.com/neuml/txtai.py
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: txtai.py Version: 7.1.0 Summary: Python client for
+Metadata-Version: 2.1 Name: txtai.py Version: 7.2.0 Summary: Python client for
 txtai Home-page: https://github.com/neuml/txtai.py Author: NeuML License:
 Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0 Project-URL:
 Documentation, https://github.com/neuml/txtai.py Project-URL: Issue Tracker,
 https://github.com/neuml/txtai.py/issues Project-URL: Source Code, https://
 github.com/neuml/txtai.py Keywords: search embedding machine-learning nlp
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

### Comparing `txtai.py-7.1.0/README.md` & `txtai.py-7.2.0/README.md`

 * *Files identical despite different names*

### Comparing `txtai.py-7.1.0/setup.py` & `txtai.py-7.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r", encoding="utf-8") as f:
     # Remove GitHub dark mode images
     DESCRIPTION = "".join([line for line in f if "gh-dark-mode-only" not in line])
 
 setup(
     name="txtai.py",
-    version="7.1.0",
+    version="7.2.0",
     author="NeuML",
     description="Python client for txtai",
     long_description=DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/neuml/txtai.py",
     project_urls={
         "Documentation": "https://github.com/neuml/txtai.py",
```

### Comparing `txtai.py-7.1.0/src/python/txtai/client/api.py` & `txtai.py-7.2.0/src/python/txtai/client/api.py`

 * *Files identical despite different names*

### Comparing `txtai.py-7.1.0/src/python/txtai/client/embeddings.py` & `txtai.py-7.2.0/src/python/txtai/client/embeddings.py`

 * *Files identical despite different names*

### Comparing `txtai.py-7.1.0/src/python/txtai/client/extractor.py` & `txtai.py-7.2.0/src/python/txtai/client/extractor.py`

 * *Files identical despite different names*

### Comparing `txtai.py-7.1.0/src/python/txtai/client/labels.py` & `txtai.py-7.2.0/src/python/txtai/client/labels.py`

 * *Files identical despite different names*

### Comparing `txtai.py-7.1.0/src/python/txtai/client/segmentation.py` & `txtai.py-7.2.0/src/python/txtai/client/segmentation.py`

 * *Files identical despite different names*

### Comparing `txtai.py-7.1.0/src/python/txtai/client/similarity.py` & `txtai.py-7.2.0/src/python/txtai/client/similarity.py`

 * *Files identical despite different names*

### Comparing `txtai.py-7.1.0/src/python/txtai/client/summary.py` & `txtai.py-7.2.0/src/python/txtai/client/summary.py`

 * *Files identical despite different names*

### Comparing `txtai.py-7.1.0/src/python/txtai/client/textractor.py` & `txtai.py-7.2.0/src/python/txtai/client/textractor.py`

 * *Files identical despite different names*

### Comparing `txtai.py-7.1.0/src/python/txtai/client/transcription.py` & `txtai.py-7.2.0/src/python/txtai/client/transcription.py`

 * *Files identical despite different names*

### Comparing `txtai.py-7.1.0/src/python/txtai/client/translation.py` & `txtai.py-7.2.0/src/python/txtai/client/translation.py`

 * *Files identical despite different names*

### Comparing `txtai.py-7.1.0/src/python/txtai.py.egg-info/PKG-INFO` & `txtai.py-7.2.0/src/python/txtai.py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: txtai.py
-Version: 7.1.0
+Version: 7.2.0
 Summary: Python client for txtai
 Home-page: https://github.com/neuml/txtai.py
 Author: NeuML
 License: Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0
 Project-URL: Documentation, https://github.com/neuml/txtai.py
 Project-URL: Issue Tracker, https://github.com/neuml/txtai.py/issues
 Project-URL: Source Code, https://github.com/neuml/txtai.py
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: txtai.py Version: 7.1.0 Summary: Python client for
+Metadata-Version: 2.1 Name: txtai.py Version: 7.2.0 Summary: Python client for
 txtai Home-page: https://github.com/neuml/txtai.py Author: NeuML License:
 Apache 2.0: http://www.apache.org/licenses/LICENSE-2.0 Project-URL:
 Documentation, https://github.com/neuml/txtai.py Project-URL: Issue Tracker,
 https://github.com/neuml/txtai.py/issues Project-URL: Source Code, https://
 github.com/neuml/txtai.py Keywords: search embedding machine-learning nlp
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

### Comparing `txtai.py-7.1.0/src/python/txtai.py.egg-info/SOURCES.txt` & `txtai.py-7.2.0/src/python/txtai.py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

