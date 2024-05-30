# Comparing `tmp/hashtag_utils-0.4.tar.gz` & `tmp/hashtag_utils-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashtag_utils-0.4.tar", last modified: Thu May 30 20:53:55 2024, max compression
+gzip compressed data, was "hashtag_utils-0.5.tar", last modified: Thu May 30 20:56:03 2024, max compression
```

## Comparing `hashtag_utils-0.4.tar` & `hashtag_utils-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:53:55.946855 hashtag_utils-0.4/
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1072 2024-05-30 18:56:08.000000 hashtag_utils-0.4/LICENSE
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1543 2024-05-30 20:53:55.946445 hashtag_utils-0.4/PKG-INFO
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1066 2024-05-30 20:53:45.000000 hashtag_utils-0.4/README.md
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:53:55.943853 hashtag_utils-0.4/hashtag_utils/
--rw-r--r--   0 aditya.patange   (502) staff       (20)      369 2024-05-30 20:06:44.000000 hashtag_utils-0.4/hashtag_utils/__init__.py
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1142 2024-05-30 20:32:27.000000 hashtag_utils-0.4/hashtag_utils/hashtag_generator.py
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:53:55.946013 hashtag_utils-0.4/hashtag_utils.egg-info/
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1543 2024-05-30 20:53:55.000000 hashtag_utils-0.4/hashtag_utils.egg-info/PKG-INFO
--rw-r--r--   0 aditya.patange   (502) staff       (20)      235 2024-05-30 20:53:55.000000 hashtag_utils-0.4/hashtag_utils.egg-info/SOURCES.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)        1 2024-05-30 20:53:55.000000 hashtag_utils-0.4/hashtag_utils.egg-info/dependency_links.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       14 2024-05-30 20:53:55.000000 hashtag_utils-0.4/hashtag_utils.egg-info/top_level.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       38 2024-05-30 20:53:55.946918 hashtag_utils-0.4/setup.cfg
--rw-r--r--   0 aditya.patange   (502) staff       (20)      628 2024-05-30 20:53:52.000000 hashtag_utils-0.4/setup.py
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:56:03.887614 hashtag_utils-0.5/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1072 2024-05-30 18:56:08.000000 hashtag_utils-0.5/LICENSE
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1543 2024-05-30 20:56:03.887151 hashtag_utils-0.5/PKG-INFO
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1066 2024-05-30 20:53:45.000000 hashtag_utils-0.5/README.md
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:56:03.884093 hashtag_utils-0.5/hashtag_utils/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      365 2024-05-30 20:55:08.000000 hashtag_utils-0.5/hashtag_utils/__init__.py
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1138 2024-05-30 20:55:03.000000 hashtag_utils-0.5/hashtag_utils/hashtag_utils.py
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 20:56:03.886584 hashtag_utils-0.5/hashtag_utils.egg-info/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1543 2024-05-30 20:56:03.000000 hashtag_utils-0.5/hashtag_utils.egg-info/PKG-INFO
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      231 2024-05-30 20:56:03.000000 hashtag_utils-0.5/hashtag_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)        1 2024-05-30 20:56:03.000000 hashtag_utils-0.5/hashtag_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       14 2024-05-30 20:56:03.000000 hashtag_utils-0.5/hashtag_utils.egg-info/top_level.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       38 2024-05-30 20:56:03.887683 hashtag_utils-0.5/setup.cfg
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      628 2024-05-30 20:55:58.000000 hashtag_utils-0.5/setup.py
```

### Comparing `hashtag_utils-0.4/LICENSE` & `hashtag_utils-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hashtag_utils-0.4/PKG-INFO` & `hashtag_utils-0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashtag_utils
-Version: 0.4
+Version: 0.5
 Summary: Simple LLM-powered hashtag utilities.
 Home-page: http://github.com/AdiPat/hashtag_utils
 Author: Aditya Patange
 Author-email: contact.adityapatange@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hashtag_utils-0.4/README.md` & `hashtag_utils-0.5/README.md`

 * *Files identical despite different names*

### Comparing `hashtag_utils-0.4/hashtag_utils/hashtag_generator.py` & `hashtag_utils-0.5/hashtag_utils/hashtag_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from openai import OpenAI
 import os
 import json
 
 
-class HashtagGenerator:
+class HashtagUtils:
     def __init__(self):
         self.client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
 
     def get_hashtags(self, content, temperature=0.5, num_tags=5):
         completion = self.client.chat.completions.create(
             model="gpt-4o",
             messages=[
```

### Comparing `hashtag_utils-0.4/hashtag_utils.egg-info/PKG-INFO` & `hashtag_utils-0.5/hashtag_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashtag_utils
-Version: 0.4
+Version: 0.5
 Summary: Simple LLM-powered hashtag utilities.
 Home-page: http://github.com/AdiPat/hashtag_utils
 Author: Aditya Patange
 Author-email: contact.adityapatange@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hashtag_utils-0.4/setup.py` & `hashtag_utils-0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hashtag_utils",
-    version="0.4",
+    version="0.5",
     packages=find_packages(),
     author="Aditya Patange",
     author_email="contact.adityapatange@gmail.com",
     description="Simple LLM-powered hashtag utilities.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="http://github.com/AdiPat/hashtag_utils",
```

