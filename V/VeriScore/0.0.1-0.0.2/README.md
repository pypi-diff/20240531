# Comparing `tmp/veriscore-0.0.1.tar.gz` & `tmp/veriscore-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veriscore-0.0.1.tar", last modified: Fri May 31 18:03:25 2024, max compression
+gzip compressed data, was "veriscore-0.0.2.tar", last modified: Fri May 31 18:43:36 2024, max compression
```

## Comparing `veriscore-0.0.1.tar` & `veriscore-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,20 @@
-drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-31 18:03:25.505184 veriscore-0.0.1/
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     1068 2024-05-21 17:48:27.000000 veriscore-0.0.1/LICENSE
--rw-r--r--   0 yekyungkim (32790) yekyungkim (32790)      522 2024-05-31 18:03:25.505184 veriscore-0.0.1/PKG-INFO
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       11 2024-05-21 17:48:27.000000 veriscore-0.0.1/README.md
-drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-31 18:03:25.505184 veriscore-0.0.1/VeriScore.egg-info/
--rw-r--r--   0 yekyungkim (32790) yekyungkim (32790)      522 2024-05-31 18:03:25.000000 veriscore-0.0.1/VeriScore.egg-info/PKG-INFO
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      190 2024-05-31 18:03:25.000000 veriscore-0.0.1/VeriScore.egg-info/SOURCES.txt
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)        1 2024-05-31 18:03:25.000000 veriscore-0.0.1/VeriScore.egg-info/dependency_links.txt
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       31 2024-05-31 18:03:25.000000 veriscore-0.0.1/VeriScore.egg-info/requires.txt
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)        1 2024-05-31 18:03:25.000000 veriscore-0.0.1/VeriScore.egg-info/top_level.txt
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       38 2024-05-31 18:03:25.505184 veriscore-0.0.1/setup.cfg
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      685 2024-05-31 17:15:51.000000 veriscore-0.0.1/setup.py
+drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-31 18:43:36.448060 veriscore-0.0.2/
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     1068 2024-05-21 17:48:27.000000 veriscore-0.0.2/LICENSE
+-rw-r--r--   0 yekyungkim (32790) yekyungkim (32790)      522 2024-05-31 18:43:36.448060 veriscore-0.0.2/PKG-INFO
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       11 2024-05-21 17:48:27.000000 veriscore-0.0.2/README.md
+drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-31 18:43:36.448060 veriscore-0.0.2/VeriScore.egg-info/
+-rw-r--r--   0 yekyungkim (32790) yekyungkim (32790)      522 2024-05-31 18:43:36.000000 veriscore-0.0.2/VeriScore.egg-info/PKG-INFO
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      391 2024-05-31 18:43:36.000000 veriscore-0.0.2/VeriScore.egg-info/SOURCES.txt
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)        1 2024-05-31 18:43:36.000000 veriscore-0.0.2/VeriScore.egg-info/dependency_links.txt
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       31 2024-05-31 18:43:36.000000 veriscore-0.0.2/VeriScore.egg-info/requires.txt
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       10 2024-05-31 18:43:36.000000 veriscore-0.0.2/VeriScore.egg-info/top_level.txt
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       38 2024-05-31 18:43:36.448060 veriscore-0.0.2/setup.cfg
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      685 2024-05-31 18:42:29.000000 veriscore-0.0.2/setup.py
+drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-31 18:43:36.448060 veriscore-0.0.2/veriscore/
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     6857 2024-05-22 19:10:56.000000 veriscore-0.0.2/veriscore/ClaimExtractor.py
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     4003 2024-05-22 19:10:56.000000 veriscore-0.0.2/veriscore/GetResponse.py
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     3315 2024-05-22 19:10:56.000000 veriscore-0.0.2/veriscore/SearchAPI.py
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       22 2024-05-31 18:42:25.000000 veriscore-0.0.2/veriscore/__init__.py
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)    26609 2024-05-22 19:10:56.000000 veriscore-0.0.2/veriscore/claim_extraction_prompt_utils.py
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     2006 2024-05-22 19:10:56.000000 veriscore-0.0.2/veriscore/evidence_retrieval.py
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     7023 2024-05-22 19:10:56.000000 veriscore-0.0.2/veriscore/extract_claims.py
```

### Comparing `veriscore-0.0.1/LICENSE` & `veriscore-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `veriscore-0.0.1/PKG-INFO` & `veriscore-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VeriScore
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pip package for Verifact
 Home-page: https://github.com/mungg/VeriScore
 Author: Yixio Song
 Author-email: yixiaosong@umass.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `veriscore-0.0.1/VeriScore.egg-info/PKG-INFO` & `veriscore-0.0.2/VeriScore.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VeriScore
-Version: 0.0.1
+Version: 0.0.2
 Summary: Pip package for Verifact
 Home-page: https://github.com/mungg/VeriScore
 Author: Yixio Song
 Author-email: yixiaosong@umass.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `veriscore-0.0.1/setup.py` & `veriscore-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
    name="VeriScore",
-   version="0.0.1",
+   version="0.0.2",
    packages=find_packages(),
    install_requires=[
        #'requests', 'numpy'
       'openai',
       'anthropic',
       'tiktoken',
       'tqdm'
```

