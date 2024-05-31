# Comparing `tmp/hashtag_utils-0.5.5.tar.gz` & `tmp/hashtag_utils-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashtag_utils-0.5.5.tar", last modified: Thu May 30 23:09:03 2024, max compression
+gzip compressed data, was "hashtag_utils-0.5.6.tar", last modified: Fri May 31 03:04:59 2024, max compression
```

## Comparing `hashtag_utils-0.5.5.tar` & `hashtag_utils-0.5.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 23:09:03.781400 hashtag_utils-0.5.5/
--rw-r--r--   0 aditya.patange   (502) staff       (20)     1072 2024-05-30 18:56:08.000000 hashtag_utils-0.5.5/LICENSE
--rw-r--r--   0 aditya.patange   (502) staff       (20)     3331 2024-05-30 23:09:03.780989 hashtag_utils-0.5.5/PKG-INFO
--rw-r--r--   0 aditya.patange   (502) staff       (20)     2801 2024-05-30 23:08:09.000000 hashtag_utils-0.5.5/README.md
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 23:09:03.777345 hashtag_utils-0.5.5/hashtag_utils/
--rw-r--r--   0 aditya.patange   (502) staff       (20)      416 2024-05-30 23:08:24.000000 hashtag_utils-0.5.5/hashtag_utils/__init__.py
--rw-r--r--   0 aditya.patange   (502) staff       (20)      283 2024-05-30 22:08:51.000000 hashtag_utils-0.5.5/hashtag_utils/common.py
--rw-r--r--   0 aditya.patange   (502) staff       (20)     7854 2024-05-30 23:05:07.000000 hashtag_utils-0.5.5/hashtag_utils/hashtag_utils.py
-drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-30 23:09:03.780531 hashtag_utils-0.5.5/hashtag_utils.egg-info/
--rw-r--r--   0 aditya.patange   (502) staff       (20)     3331 2024-05-30 23:09:03.000000 hashtag_utils-0.5.5/hashtag_utils.egg-info/PKG-INFO
--rw-r--r--   0 aditya.patange   (502) staff       (20)      291 2024-05-30 23:09:03.000000 hashtag_utils-0.5.5/hashtag_utils.egg-info/SOURCES.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)        1 2024-05-30 23:09:03.000000 hashtag_utils-0.5.5/hashtag_utils.egg-info/dependency_links.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       21 2024-05-30 23:09:03.000000 hashtag_utils-0.5.5/hashtag_utils.egg-info/requires.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       14 2024-05-30 23:09:03.000000 hashtag_utils-0.5.5/hashtag_utils.egg-info/top_level.txt
--rw-r--r--   0 aditya.patange   (502) staff       (20)       38 2024-05-30 23:09:03.781463 hashtag_utils-0.5.5/setup.cfg
--rw-r--r--   0 aditya.patange   (502) staff       (20)      705 2024-05-30 23:08:58.000000 hashtag_utils-0.5.5/setup.py
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-31 03:04:59.735164 hashtag_utils-0.5.6/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     1072 2024-05-30 18:56:08.000000 hashtag_utils-0.5.6/LICENSE
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     3546 2024-05-31 03:04:59.734701 hashtag_utils-0.5.6/PKG-INFO
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     3016 2024-05-31 03:04:11.000000 hashtag_utils-0.5.6/README.md
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-31 03:04:59.729874 hashtag_utils-0.5.6/hashtag_utils/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      416 2024-05-30 23:08:24.000000 hashtag_utils-0.5.6/hashtag_utils/__init__.py
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      283 2024-05-30 22:08:51.000000 hashtag_utils-0.5.6/hashtag_utils/common.py
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     7854 2024-05-30 23:05:07.000000 hashtag_utils-0.5.6/hashtag_utils/hashtag_utils.py
+drwxr-xr-x   0 aditya.patange   (502) staff       (20)        0 2024-05-31 03:04:59.734248 hashtag_utils-0.5.6/hashtag_utils.egg-info/
+-rw-r--r--   0 aditya.patange   (502) staff       (20)     3546 2024-05-31 03:04:59.000000 hashtag_utils-0.5.6/hashtag_utils.egg-info/PKG-INFO
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      291 2024-05-31 03:04:59.000000 hashtag_utils-0.5.6/hashtag_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)        1 2024-05-31 03:04:59.000000 hashtag_utils-0.5.6/hashtag_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       21 2024-05-31 03:04:59.000000 hashtag_utils-0.5.6/hashtag_utils.egg-info/requires.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       14 2024-05-31 03:04:59.000000 hashtag_utils-0.5.6/hashtag_utils.egg-info/top_level.txt
+-rw-r--r--   0 aditya.patange   (502) staff       (20)       38 2024-05-31 03:04:59.735219 hashtag_utils-0.5.6/setup.cfg
+-rw-r--r--   0 aditya.patange   (502) staff       (20)      705 2024-05-31 03:04:57.000000 hashtag_utils-0.5.6/setup.py
```

### Comparing `hashtag_utils-0.5.5/LICENSE` & `hashtag_utils-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hashtag_utils-0.5.5/PKG-INFO` & `hashtag_utils-0.5.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashtag_utils
-Version: 0.5.5
+Version: 0.5.6
 Summary: Simple LLM-powered hashtag utilities.
 Home-page: http://github.com/AdiPat/hashtag_utils
 Author: Aditya Patange
 Author-email: contact.adityapatange@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -33,14 +33,27 @@
 - **Hashtag Definitions**: Get hashtag definitions. 
 
 
 # Usage: HashtagUtils API
 
 Make sure you add your `OPENAI_API_KEY` to a .env file from the location where you're running the script. 
 
+```python
+from hashtag_utils import HashtagUtils
+
+hg = HashtagUtils()
+
+text = "A new study shows that eating chocolate can help you lose weight."
+
+hashtags = hg.get_hashtags(text)
+
+# check other methods below
+
+```
+
 ## Methods
 
 ### `get_hashtags(text: str, temperature: float = 1.0, num_tags: int = 5) -> List[str]`
 
 Generates a list of hashtags based on the given text. 
 
 - `text`: The input text to generate hashtags from.
```

### Comparing `hashtag_utils-0.5.5/README.md` & `hashtag_utils-0.5.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,27 @@
 - **Hashtag Definitions**: Get hashtag definitions. 
 
 
 # Usage: HashtagUtils API
 
 Make sure you add your `OPENAI_API_KEY` to a .env file from the location where you're running the script. 
 
+```python
+from hashtag_utils import HashtagUtils
+
+hg = HashtagUtils()
+
+text = "A new study shows that eating chocolate can help you lose weight."
+
+hashtags = hg.get_hashtags(text)
+
+# check other methods below
+
+```
+
 ## Methods
 
 ### `get_hashtags(text: str, temperature: float = 1.0, num_tags: int = 5) -> List[str]`
 
 Generates a list of hashtags based on the given text. 
 
 - `text`: The input text to generate hashtags from.
```

### Comparing `hashtag_utils-0.5.5/hashtag_utils/hashtag_utils.py` & `hashtag_utils-0.5.6/hashtag_utils/hashtag_utils.py`

 * *Files identical despite different names*

### Comparing `hashtag_utils-0.5.5/hashtag_utils.egg-info/PKG-INFO` & `hashtag_utils-0.5.6/hashtag_utils.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashtag_utils
-Version: 0.5.5
+Version: 0.5.6
 Summary: Simple LLM-powered hashtag utilities.
 Home-page: http://github.com/AdiPat/hashtag_utils
 Author: Aditya Patange
 Author-email: contact.adityapatange@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -33,14 +33,27 @@
 - **Hashtag Definitions**: Get hashtag definitions. 
 
 
 # Usage: HashtagUtils API
 
 Make sure you add your `OPENAI_API_KEY` to a .env file from the location where you're running the script. 
 
+```python
+from hashtag_utils import HashtagUtils
+
+hg = HashtagUtils()
+
+text = "A new study shows that eating chocolate can help you lose weight."
+
+hashtags = hg.get_hashtags(text)
+
+# check other methods below
+
+```
+
 ## Methods
 
 ### `get_hashtags(text: str, temperature: float = 1.0, num_tags: int = 5) -> List[str]`
 
 Generates a list of hashtags based on the given text. 
 
 - `text`: The input text to generate hashtags from.
```

### Comparing `hashtag_utils-0.5.5/setup.py` & `hashtag_utils-0.5.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="hashtag_utils",
-    version="0.5.5",
+    version="0.5.6",
     packages=["hashtag_utils"],
     author="Aditya Patange",
     author_email="contact.adityapatange@gmail.com",
     description="Simple LLM-powered hashtag utilities.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="http://github.com/AdiPat/hashtag_utils",
```

