# Comparing `tmp/pymachinelearning-0.0.1.tar.gz` & `tmp/pymachinelearning-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymachinelearning-0.0.1.tar", last modified: Thu Apr 18 14:31:28 2024, max compression
+gzip compressed data, was "pymachinelearning-0.0.2.tar", last modified: Fri May 31 19:09:35 2024, max compression
```

## Comparing `pymachinelearning-0.0.1.tar` & `pymachinelearning-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 14:31:28.965992 pymachinelearning-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-12-09 15:06:56.000000 pymachinelearning-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      553 2024-04-18 14:31:28.965992 pymachinelearning-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 14:31:28.800875 pymachinelearning-0.0.1/PyMachineLearning/
--rw-rw-rw-   0        0        0       26 2024-04-18 14:27:41.000000 pymachinelearning-0.0.1/PyMachineLearning/__init__.py
--rw-rw-rw-   0        0        0       39 2024-04-18 14:27:02.000000 pymachinelearning-0.0.1/PyMachineLearning/test.py
-drwxrwxrwx   0        0        0        0 2024-04-18 14:31:28.965263 pymachinelearning-0.0.1/PyMachineLearning.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-18 14:31:28.000000 pymachinelearning-0.0.1/PyMachineLearning.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      286 2024-04-18 14:31:28.000000 pymachinelearning-0.0.1/PyMachineLearning.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 14:31:28.000000 pymachinelearning-0.0.1/PyMachineLearning.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-18 14:31:28.000000 pymachinelearning-0.0.1/PyMachineLearning.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-18 14:31:28.000000 pymachinelearning-0.0.1/PyMachineLearning.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       24 2024-04-18 14:29:21.000000 pymachinelearning-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-18 14:31:28.965992 pymachinelearning-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      798 2024-04-18 14:29:44.000000 pymachinelearning-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:09:35.961695 pymachinelearning-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-12-09 15:06:56.000000 pymachinelearning-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      553 2024-05-31 19:09:35.960693 pymachinelearning-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-31 19:09:35.946449 pymachinelearning-0.0.2/PyMachineLearning/
+-rw-rw-rw-   0        0        0      266 2024-04-11 11:28:18.000000 pymachinelearning-0.0.2/PyMachineLearning/__init__.py
+-rw-rw-rw-   0        0        0    15774 2024-05-10 08:28:24.000000 pymachinelearning-0.0.2/PyMachineLearning/evaluation.py
+-rw-rw-rw-   0        0        0      634 2024-04-12 09:10:16.000000 pymachinelearning-0.0.2/PyMachineLearning/metrics.py
+-rw-rw-rw-   0        0        0     5672 2024-04-20 10:50:01.000000 pymachinelearning-0.0.2/PyMachineLearning/plots.py
+-rw-rw-rw-   0        0        0    12763 2024-04-30 15:34:07.000000 pymachinelearning-0.0.2/PyMachineLearning/preprocessing.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:09:35.959690 pymachinelearning-0.0.2/PyMachineLearning.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-05-31 19:09:35.000000 pymachinelearning-0.0.2/PyMachineLearning.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2024-05-31 19:09:35.000000 pymachinelearning-0.0.2/PyMachineLearning.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 19:09:35.000000 pymachinelearning-0.0.2/PyMachineLearning.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-31 19:09:35.000000 pymachinelearning-0.0.2/PyMachineLearning.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-31 19:09:35.000000 pymachinelearning-0.0.2/PyMachineLearning.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       24 2024-04-18 14:29:21.000000 pymachinelearning-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-31 19:09:35.962693 pymachinelearning-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      798 2024-05-31 19:09:15.000000 pymachinelearning-0.0.2/setup.py
```

### Comparing `pymachinelearning-0.0.1/LICENSE` & `pymachinelearning-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymachinelearning-0.0.1/PKG-INFO` & `pymachinelearning-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMachineLearning
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package with ML utils.
 Home-page: https://github.com/FabioScielzoOrtiz/PyMachineLearning_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pymachinelearning-0.0.1/PyMachineLearning.egg-info/PKG-INFO` & `pymachinelearning-0.0.2/PyMachineLearning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyMachineLearning
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package with ML utils.
 Home-page: https://github.com/FabioScielzoOrtiz/PyMachineLearning_Package
 Author: Fabio Scielzo Ortiz
 Author-email: fabioscielzo98@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pymachinelearning-0.0.1/setup.py` & `pymachinelearning-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PyMachineLearning",
-    version="0.0.1",
+    version="0.0.2",
     author="Fabio Scielzo Ortiz",
     author_email="fabioscielzo98@gmail.com",
     description="A package with ML utils.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FabioScielzoOrtiz/PyMachineLearning_Package",  # add your project URL here
     packages=find_packages(),
```

