# Comparing `tmp/indic_num2words-1.2.1.tar.gz` & `tmp/indic_num2words-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indic_num2words-1.2.1.tar", last modified: Tue Apr 16 02:07:12 2024, max compression
+gzip compressed data, was "indic_num2words-1.2.2.tar", last modified: Thu May 30 22:01:25 2024, max compression
```

## Comparing `indic_num2words-1.2.1.tar` & `indic_num2words-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:07:12.772409 indic_num2words-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 02:07:08.000000 indic_num2words-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-16 02:07:12.772409 indic_num2words-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-16 02:07:08.000000 indic_num2words-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:07:12.772409 indic_num2words-1.2.1/indic_num2words.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-16 02:07:12.000000 indic_num2words-1.2.1/indic_num2words.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-16 02:07:12.000000 indic_num2words-1.2.1/indic_num2words.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 02:07:12.000000 indic_num2words-1.2.1/indic_num2words.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 02:07:12.000000 indic_num2words-1.2.1/indic_num2words.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 02:07:12.000000 indic_num2words-1.2.1/indic_num2words.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:07:12.772409 indic_num2words-1.2.1/num_to_words/
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-16 02:07:08.000000 indic_num2words-1.2.1/num_to_words/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-16 02:07:08.000000 indic_num2words-1.2.1/num_to_words/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 02:07:12.772409 indic_num2words-1.2.1/num_to_words/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 02:07:08.000000 indic_num2words-1.2.1/num_to_words/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37477 2024-04-16 02:07:08.000000 indic_num2words-1.2.1/num_to_words/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 02:07:08.000000 indic_num2words-1.2.1/num_to_words/version.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-16 02:07:12.772409 indic_num2words-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-16 02:07:08.000000 indic_num2words-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:01:25.554345 indic_num2words-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 22:01:21.000000 indic_num2words-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-30 22:01:25.554345 indic_num2words-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-30 22:01:21.000000 indic_num2words-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:01:25.554345 indic_num2words-1.2.2/indic_num2words.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-30 22:01:25.000000 indic_num2words-1.2.2/indic_num2words.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-30 22:01:25.000000 indic_num2words-1.2.2/indic_num2words.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 22:01:25.000000 indic_num2words-1.2.2/indic_num2words.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 22:01:25.000000 indic_num2words-1.2.2/indic_num2words.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-30 22:01:25.000000 indic_num2words-1.2.2/indic_num2words.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:01:25.554345 indic_num2words-1.2.2/num_to_words/
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-30 22:01:21.000000 indic_num2words-1.2.2/num_to_words/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-05-30 22:01:21.000000 indic_num2words-1.2.2/num_to_words/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:01:25.554345 indic_num2words-1.2.2/num_to_words/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-30 22:01:21.000000 indic_num2words-1.2.2/num_to_words/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37477 2024-05-30 22:01:21.000000 indic_num2words-1.2.2/num_to_words/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-30 22:01:21.000000 indic_num2words-1.2.2/num_to_words/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-30 22:01:25.554345 indic_num2words-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-05-30 22:01:21.000000 indic_num2words-1.2.2/setup.py
```

### Comparing `indic_num2words-1.2.1/LICENSE` & `indic_num2words-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `indic_num2words-1.2.1/num_to_words/__init__.py` & `indic_num2words-1.2.2/num_to_words/__init__.py`

 * *Files identical despite different names*

### Comparing `indic_num2words-1.2.1/num_to_words/exception.py` & `indic_num2words-1.2.2/num_to_words/exception.py`

 * *Files identical despite different names*

### Comparing `indic_num2words-1.2.1/num_to_words/utils/constants.py` & `indic_num2words-1.2.2/num_to_words/utils/constants.py`

 * *Files identical despite different names*

### Comparing `indic_num2words-1.2.1/setup.py` & `indic_num2words-1.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     name="indic-num2words",
     version=version,
     license="Apache License",
     author="Indic-Num2Words Contributors",
     author_email="sutariyaraj77725@gmail.com",
     description="Package to convert numbers to words with support of multiple indian languages.",
     long_description=long_description,
-    long_description_content_type="text/x-rst",
+    long_description_content_type="text/markdown",
     url="https://github.com/sutariyaraj/indic-num2words/",
     packages=find_packages(),
     zip_safe=False,
     install_requires=[],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

