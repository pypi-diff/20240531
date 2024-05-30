# Comparing `tmp/hashtag_utils-0.5.3.tar.gz` & `tmp/hashtag_utils-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashtag_utils-0.5.3.tar", last modified: Thu May 30 23:01:13 2024, max compression
+gzip compressed data, was "hashtag_utils-0.5.4.tar", last modified: Thu May 30 23:05:09 2024, max compression
```

## Comparing `hashtag_utils-0.5.3.tar` & `hashtag_utils-0.5.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 23:01:13.794763 hashtag_utils-0.5.3/
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1072 2024-05-30 18:56:08.000000 hashtag_utils-0.5.3/LICENSE
--rw-r--r--   0 aditya.patange   (502) staff       (20)     3125 2024-05-30 23:01:13.794321 hashtag_utils-0.5.3/PKG-INFO
--rw-r--r--   0 aditya.patange   (502) staff       (20)     2595 2024-05-30 22:59:16.000000 hashtag_utils-0.5.3/README.md
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 23:01:13.791064 hashtag_utils-0.5.3/hashtag_utils/
--rw-r--r--   0 aditya.patange   (502) staff       (20)      361 2024-05-30 21:01:49.000000 hashtag_utils-0.5.3/hashtag_utils/__init__.py
--rw-r--r--   0 aditya.patange   (502) staff       (20)      283 2024-05-30 22:08:51.000000 hashtag_utils-0.5.3/hashtag_utils/common.py
--rw-r--r--   0 aditya.patange   (502) staff       (20)     7897 2024-05-30 23:01:04.000000 hashtag_utils-0.5.3/hashtag_utils/hashtag_utils.py
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 23:01:13.793855 hashtag_utils-0.5.3/hashtag_utils.egg-info/
--rw-r--r--   0 aditya.patange   (502) staff       (20)     3125 2024-05-30 23:01:13.000000 hashtag_utils-0.5.3/hashtag_utils.egg-info/PKG-INFO
--rw-r--r--   0 aditya.patange   (502) staff       (20)      291 2024-05-30 23:01:13.000000 hashtag_utils-0.5.3/hashtag_utils.egg-info/SOURCES.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)        1 2024-05-30 23:01:13.000000 hashtag_utils-0.5.3/hashtag_utils.egg-info/dependency_links.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       21 2024-05-30 23:01:13.000000 hashtag_utils-0.5.3/hashtag_utils.egg-info/requires.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       14 2024-05-30 23:01:13.000000 hashtag_utils-0.5.3/hashtag_utils.egg-info/top_level.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       38 2024-05-30 23:01:13.794820 hashtag_utils-0.5.3/setup.cfg
--rw-r--r--   0 aditya.patange   (502) staff       (20)      705 2024-05-30 23:01:08.000000 hashtag_utils-0.5.3/setup.py
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 23:05:09.716472 hashtag_utils-0.5.4/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1072 2024-05-30 18:56:08.000000 hashtag_utils-0.5.4/LICENSE
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     3125 2024-05-30 23:05:09.715973 hashtag_utils-0.5.4/PKG-INFO
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     2595 2024-05-30 22:59:16.000000 hashtag_utils-0.5.4/README.md
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 23:05:09.712712 hashtag_utils-0.5.4/hashtag_utils/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      444 2024-05-30 23:04:46.000000 hashtag_utils-0.5.4/hashtag_utils/__init__.py
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      283 2024-05-30 22:08:51.000000 hashtag_utils-0.5.4/hashtag_utils/common.py
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     7854 2024-05-30 23:05:07.000000 hashtag_utils-0.5.4/hashtag_utils/hashtag_utils.py
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 23:05:09.715444 hashtag_utils-0.5.4/hashtag_utils.egg-info/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     3125 2024-05-30 23:05:09.000000 hashtag_utils-0.5.4/hashtag_utils.egg-info/PKG-INFO
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      291 2024-05-30 23:05:09.000000 hashtag_utils-0.5.4/hashtag_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)        1 2024-05-30 23:05:09.000000 hashtag_utils-0.5.4/hashtag_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       21 2024-05-30 23:05:09.000000 hashtag_utils-0.5.4/hashtag_utils.egg-info/requires.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       14 2024-05-30 23:05:09.000000 hashtag_utils-0.5.4/hashtag_utils.egg-info/top_level.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       38 2024-05-30 23:05:09.716542 hashtag_utils-0.5.4/setup.cfg
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      705 2024-05-30 23:04:58.000000 hashtag_utils-0.5.4/setup.py
```

### Comparing `hashtag_utils-0.5.3/LICENSE` & `hashtag_utils-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hashtag_utils-0.5.3/PKG-INFO` & `hashtag_utils-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashtag_utils
-Version: 0.5.3
+Version: 0.5.4
 Summary: Simple LLM-powered hashtag utilities.
 Home-page: http://github.com/AdiPat/hashtag_utils
 Author: Aditya Patange
 Author-email: contact.adityapatange@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hashtag_utils-0.5.3/README.md` & `hashtag_utils-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `hashtag_utils-0.5.3/hashtag_utils/hashtag_utils.py` & `hashtag_utils-0.5.4/hashtag_utils/hashtag_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import traceback
 from typing import List
 from openai import OpenAI
 import os
 import json
 from .common import is_alphanumeric
-import dotenv
 
 
 
 class HashtagUtils:
     def __init__(self):
-        dotenv.load_dotenv()
         self.client = OpenAI(api_key=os.getenv("OPENAI_API_KEY"))
         
     def get_hashtags(self, content: str, temperature=0.5, num_tags=5) -> List[str]:
         try:
             completion = self.client.chat.completions.create(
                 model="gpt-4o",
                 messages=[
```

### Comparing `hashtag_utils-0.5.3/hashtag_utils.egg-info/PKG-INFO` & `hashtag_utils-0.5.4/hashtag_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashtag_utils
-Version: 0.5.3
+Version: 0.5.4
 Summary: Simple LLM-powered hashtag utilities.
 Home-page: http://github.com/AdiPat/hashtag_utils
 Author: Aditya Patange
 Author-email: contact.adityapatange@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hashtag_utils-0.5.3/setup.py` & `hashtag_utils-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hashtag_utils",
-    version="0.5.3",
+    version="0.5.4",
     packages=["hashtag_utils"],
     author="Aditya Patange",
     author_email="contact.adityapatange@gmail.com",
     description="Simple LLM-powered hashtag utilities.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="http://github.com/AdiPat/hashtag_utils",
```

