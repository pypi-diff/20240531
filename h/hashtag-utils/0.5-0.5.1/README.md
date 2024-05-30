# Comparing `tmp/hashtag_utils-0.5.tar.gz` & `tmp/hashtag_utils-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashtag_utils-0.5.tar", last modified: Thu May 30 20:56:03 2024, max compression
+gzip compressed data, was "hashtag_utils-0.5.1.tar", last modified: Thu May 30 22:37:36 2024, max compression
```

## Comparing `hashtag_utils-0.5.tar` & `hashtag_utils-0.5.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:56:03.887614 hashtag_utils-0.5/
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1072 2024-05-30 18:56:08.000000 hashtag_utils-0.5/LICENSE
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1543 2024-05-30 20:56:03.887151 hashtag_utils-0.5/PKG-INFO
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1066 2024-05-30 20:53:45.000000 hashtag_utils-0.5/README.md
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:56:03.884093 hashtag_utils-0.5/hashtag_utils/
--rw-r--r--   0 aditya.patange   (502) staff       (20)      365 2024-05-30 20:55:08.000000 hashtag_utils-0.5/hashtag_utils/__init__.py
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1138 2024-05-30 20:55:03.000000 hashtag_utils-0.5/hashtag_utils/hashtag_utils.py
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:56:03.886584 hashtag_utils-0.5/hashtag_utils.egg-info/
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1543 2024-05-30 20:56:03.000000 hashtag_utils-0.5/hashtag_utils.egg-info/PKG-INFO
--rw-r--r--   0 aditya.patange   (502) staff       (20)      231 2024-05-30 20:56:03.000000 hashtag_utils-0.5/hashtag_utils.egg-info/SOURCES.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)        1 2024-05-30 20:56:03.000000 hashtag_utils-0.5/hashtag_utils.egg-info/dependency_links.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       14 2024-05-30 20:56:03.000000 hashtag_utils-0.5/hashtag_utils.egg-info/top_level.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       38 2024-05-30 20:56:03.887683 hashtag_utils-0.5/setup.cfg
--rw-r--r--   0 aditya.patange   (502) staff       (20)      628 2024-05-30 20:55:58.000000 hashtag_utils-0.5/setup.py
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 22:37:36.982932 hashtag_utils-0.5.1/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1072 2024-05-30 18:56:08.000000 hashtag_utils-0.5.1/LICENSE
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1598 2024-05-30 22:37:36.982483 hashtag_utils-0.5.1/PKG-INFO
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1119 2024-05-30 22:05:42.000000 hashtag_utils-0.5.1/README.md
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 22:37:36.978850 hashtag_utils-0.5.1/hashtag_utils/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      361 2024-05-30 21:01:49.000000 hashtag_utils-0.5.1/hashtag_utils/__init__.py
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      283 2024-05-30 22:08:51.000000 hashtag_utils-0.5.1/hashtag_utils/common.py
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     7846 2024-05-30 22:33:30.000000 hashtag_utils-0.5.1/hashtag_utils/hashtag_utils.py
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 22:37:36.981920 hashtag_utils-0.5.1/hashtag_utils.egg-info/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1598 2024-05-30 22:37:36.000000 hashtag_utils-0.5.1/hashtag_utils.egg-info/PKG-INFO
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      255 2024-05-30 22:37:36.000000 hashtag_utils-0.5.1/hashtag_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)        1 2024-05-30 22:37:36.000000 hashtag_utils-0.5.1/hashtag_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       14 2024-05-30 22:37:36.000000 hashtag_utils-0.5.1/hashtag_utils.egg-info/top_level.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       38 2024-05-30 22:37:36.982997 hashtag_utils-0.5.1/setup.cfg
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      630 2024-05-30 22:37:27.000000 hashtag_utils-0.5.1/setup.py
```

### Comparing `hashtag_utils-0.5/LICENSE` & `hashtag_utils-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hashtag_utils-0.5/PKG-INFO` & `hashtag_utils-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashtag_utils
-Version: 0.5
+Version: 0.5.1
 Summary: Simple LLM-powered hashtag utilities.
 Home-page: http://github.com/AdiPat/hashtag_utils
 Author: Aditya Patange
 Author-email: contact.adityapatange@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -24,10 +24,11 @@
 **Feel free to suggest features, ideas and improvements! If you want to contribute, feel free to fork and send a Pull Request. I'm actively working on this project.**
 
 ## Features 
 - **Hashtag Generator:** Generates hashtags for a content piece.
 - **Hashtag Relevance:** Returns the percentage relevance of a hashtag with respect to a content piece.
 - **Similar Hashtags:** Generates hash tages similar to the provided ones.
 - **Hashtag Distance:** Computes how close two hashtags are.
+- **Hashtag Definitions**: Get hashtag definitions. 
 
 # Contributors 
 - [Aditya Patange (AdiPat)](https://wwww.github.com/AdiPat)
```

### Comparing `hashtag_utils-0.5/README.md` & `hashtag_utils-0.5.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,10 +10,11 @@
 **Feel free to suggest features, ideas and improvements! If you want to contribute, feel free to fork and send a Pull Request. I'm actively working on this project.**
 
 ## Features 
 - **Hashtag Generator:** Generates hashtags for a content piece.
 - **Hashtag Relevance:** Returns the percentage relevance of a hashtag with respect to a content piece.
 - **Similar Hashtags:** Generates hash tages similar to the provided ones.
 - **Hashtag Distance:** Computes how close two hashtags are.
+- **Hashtag Definitions**: Get hashtag definitions. 
 
 # Contributors 
 - [Aditya Patange (AdiPat)](https://wwww.github.com/AdiPat)
```

### Comparing `hashtag_utils-0.5/hashtag_utils.egg-info/PKG-INFO` & `hashtag_utils-0.5.1/hashtag_utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashtag_utils
-Version: 0.5
+Version: 0.5.1
 Summary: Simple LLM-powered hashtag utilities.
 Home-page: http://github.com/AdiPat/hashtag_utils
 Author: Aditya Patange
 Author-email: contact.adityapatange@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -24,10 +24,11 @@
 **Feel free to suggest features, ideas and improvements! If you want to contribute, feel free to fork and send a Pull Request. I'm actively working on this project.**
 
 ## Features 
 - **Hashtag Generator:** Generates hashtags for a content piece.
 - **Hashtag Relevance:** Returns the percentage relevance of a hashtag with respect to a content piece.
 - **Similar Hashtags:** Generates hash tages similar to the provided ones.
 - **Hashtag Distance:** Computes how close two hashtags are.
+- **Hashtag Definitions**: Get hashtag definitions. 
 
 # Contributors 
 - [Aditya Patange (AdiPat)](https://wwww.github.com/AdiPat)
```

### Comparing `hashtag_utils-0.5/setup.py` & `hashtag_utils-0.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hashtag_utils",
-    version="0.5",
+    version="0.5.1",
     packages=find_packages(),
     author="Aditya Patange",
     author_email="contact.adityapatange@gmail.com",
     description="Simple LLM-powered hashtag utilities.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="http://github.com/AdiPat/hashtag_utils",
```

