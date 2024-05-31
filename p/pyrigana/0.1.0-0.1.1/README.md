# Comparing `tmp/pyrigana-0.1.0.tar.gz` & `tmp/pyrigana-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrigana-0.1.0.tar", last modified: Thu May 30 16:37:16 2024, max compression
+gzip compressed data, was "pyrigana-0.1.1.tar", last modified: Fri May 31 16:31:00 2024, max compression
```

## Comparing `pyrigana-0.1.0.tar` & `pyrigana-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 aknay     (1000) aknay     (1000)        0 2024-05-30 16:37:16.422690 pyrigana-0.1.0/
--rw-rw-r--   0 aknay     (1000) aknay     (1000)       33 2024-05-30 15:39:26.000000 pyrigana-0.1.0/MANIFEST.in
--rw-r--r--   0 aknay     (1000) aknay     (1000)      567 2024-05-30 16:37:16.422690 pyrigana-0.1.0/PKG-INFO
--rw-rw-r--   0 aknay     (1000) aknay     (1000)       10 2024-05-30 16:29:08.000000 pyrigana-0.1.0/README.md
-drwxrwxr-x   0 aknay     (1000) aknay     (1000)        0 2024-05-30 16:37:16.422690 pyrigana-0.1.0/examples/
--rw-rw-r--   0 aknay     (1000) aknay     (1000)        0 2024-05-30 16:08:19.000000 pyrigana-0.1.0/examples/__init__.py
--rw-rw-r--   0 aknay     (1000) aknay     (1000)      533 2024-05-30 16:33:54.000000 pyrigana-0.1.0/examples/get_furigana_html_example.py
-drwxrwxr-x   0 aknay     (1000) aknay     (1000)        0 2024-05-30 16:37:16.422690 pyrigana-0.1.0/pyrigana/
--rw-rw-r--   0 aknay     (1000) aknay     (1000)       39 2024-05-30 16:10:59.000000 pyrigana-0.1.0/pyrigana/__init__.py
-drwxrwxr-x   0 aknay     (1000) aknay     (1000)        0 2024-05-30 16:37:16.422690 pyrigana-0.1.0/pyrigana/_internal/
--rw-rw-r--   0 aknay     (1000) aknay     (1000)        0 2024-05-30 15:29:34.000000 pyrigana-0.1.0/pyrigana/_internal/__init__.py
--rw-rw-r--   0 aknay     (1000) aknay     (1000)     2227 2024-05-30 16:22:53.000000 pyrigana-0.1.0/pyrigana/_internal/utils.py
--rw-rw-r--   0 aknay     (1000) aknay     (1000)      176 2024-05-30 16:04:46.000000 pyrigana-0.1.0/pyrigana/pyrigana.py
-drwxrwxr-x   0 aknay     (1000) aknay     (1000)        0 2024-05-30 16:37:16.422690 pyrigana-0.1.0/pyrigana/tests/
--rw-rw-r--   0 aknay     (1000) aknay     (1000)        0 2024-05-30 15:40:43.000000 pyrigana-0.1.0/pyrigana/tests/__init__.py
--rw-rw-r--   0 aknay     (1000) aknay     (1000)     1054 2024-05-30 16:24:44.000000 pyrigana-0.1.0/pyrigana/tests/test_compare_list.py
--rw-rw-r--   0 aknay     (1000) aknay     (1000)      976 2024-05-30 16:24:19.000000 pyrigana-0.1.0/pyrigana/tests/test_furigana_html.py
--rw-rw-r--   0 aknay     (1000) aknay     (1000)      458 2024-05-30 16:00:51.000000 pyrigana-0.1.0/pyrigana/tests/test_pair_list.py
-drwxrwxr-x   0 aknay     (1000) aknay     (1000)        0 2024-05-30 16:37:16.422690 pyrigana-0.1.0/pyrigana.egg-info/
--rw-r--r--   0 aknay     (1000) aknay     (1000)      567 2024-05-30 16:37:16.000000 pyrigana-0.1.0/pyrigana.egg-info/PKG-INFO
--rw-rw-r--   0 aknay     (1000) aknay     (1000)      492 2024-05-30 16:37:16.000000 pyrigana-0.1.0/pyrigana.egg-info/SOURCES.txt
--rw-rw-r--   0 aknay     (1000) aknay     (1000)        1 2024-05-30 16:37:16.000000 pyrigana-0.1.0/pyrigana.egg-info/dependency_links.txt
--rw-rw-r--   0 aknay     (1000) aknay     (1000)       50 2024-05-30 16:37:16.000000 pyrigana-0.1.0/pyrigana.egg-info/requires.txt
--rw-rw-r--   0 aknay     (1000) aknay     (1000)       18 2024-05-30 16:37:16.000000 pyrigana-0.1.0/pyrigana.egg-info/top_level.txt
--rw-rw-r--   0 aknay     (1000) aknay     (1000)       79 2024-05-30 16:37:16.422690 pyrigana-0.1.0/setup.cfg
--rw-rw-r--   0 aknay     (1000) aknay     (1000)      848 2024-05-30 15:51:58.000000 pyrigana-0.1.0/setup.py
+drwxrwxr-x   0 aknay     (1000) aknay     (1000)        0 2024-05-31 16:31:00.954510 pyrigana-0.1.1/
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)       33 2024-05-30 15:39:26.000000 pyrigana-0.1.1/MANIFEST.in
+-rw-r--r--   0 aknay     (1000) aknay     (1000)      567 2024-05-31 16:31:00.954510 pyrigana-0.1.1/PKG-INFO
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)       10 2024-05-30 16:29:08.000000 pyrigana-0.1.1/README.md
+drwxrwxr-x   0 aknay     (1000) aknay     (1000)        0 2024-05-31 16:31:00.950510 pyrigana-0.1.1/examples/
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)        0 2024-05-30 16:08:19.000000 pyrigana-0.1.1/examples/__init__.py
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)      533 2024-05-30 16:33:54.000000 pyrigana-0.1.1/examples/get_furigana_html_example.py
+drwxrwxr-x   0 aknay     (1000) aknay     (1000)        0 2024-05-31 16:31:00.950510 pyrigana-0.1.1/pyrigana/
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)       39 2024-05-30 16:10:59.000000 pyrigana-0.1.1/pyrigana/__init__.py
+drwxrwxr-x   0 aknay     (1000) aknay     (1000)        0 2024-05-31 16:31:00.954510 pyrigana-0.1.1/pyrigana/_internal/
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)        0 2024-05-30 15:29:34.000000 pyrigana-0.1.1/pyrigana/_internal/__init__.py
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)     3239 2024-05-31 16:18:07.000000 pyrigana-0.1.1/pyrigana/_internal/utils.py
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)      176 2024-05-30 16:04:46.000000 pyrigana-0.1.1/pyrigana/pyrigana.py
+drwxrwxr-x   0 aknay     (1000) aknay     (1000)        0 2024-05-31 16:31:00.954510 pyrigana-0.1.1/pyrigana/tests/
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)        0 2024-05-30 15:40:43.000000 pyrigana-0.1.1/pyrigana/tests/__init__.py
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)     2340 2024-05-31 16:18:07.000000 pyrigana-0.1.1/pyrigana/tests/test_compare_list.py
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)      976 2024-05-30 16:24:19.000000 pyrigana-0.1.1/pyrigana/tests/test_furigana_html.py
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)      458 2024-05-30 16:00:51.000000 pyrigana-0.1.1/pyrigana/tests/test_pair_list.py
+drwxrwxr-x   0 aknay     (1000) aknay     (1000)        0 2024-05-31 16:31:00.954510 pyrigana-0.1.1/pyrigana.egg-info/
+-rw-r--r--   0 aknay     (1000) aknay     (1000)      567 2024-05-31 16:31:00.000000 pyrigana-0.1.1/pyrigana.egg-info/PKG-INFO
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)      492 2024-05-31 16:31:00.000000 pyrigana-0.1.1/pyrigana.egg-info/SOURCES.txt
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)        1 2024-05-31 16:31:00.000000 pyrigana-0.1.1/pyrigana.egg-info/dependency_links.txt
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)       50 2024-05-31 16:31:00.000000 pyrigana-0.1.1/pyrigana.egg-info/requires.txt
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)       18 2024-05-31 16:31:00.000000 pyrigana-0.1.1/pyrigana.egg-info/top_level.txt
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)       79 2024-05-31 16:31:00.954510 pyrigana-0.1.1/setup.cfg
+-rw-rw-r--   0 aknay     (1000) aknay     (1000)      848 2024-05-31 16:19:13.000000 pyrigana-0.1.1/setup.py
```

### Comparing `pyrigana-0.1.0/PKG-INFO` & `pyrigana-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrigana
-Version: 0.1.0
+Version: 0.1.1
 Summary: A brief description of my package
 Home-page: https://github.com/aknay/pyrigana
 Author: Nay Aung Kyaw
 Author-email: aknay@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrigana-0.1.0/examples/get_furigana_html_example.py` & `pyrigana-0.1.1/examples/get_furigana_html_example.py`

 * *Files identical despite different names*

### Comparing `pyrigana-0.1.0/pyrigana/tests/test_furigana_html.py` & `pyrigana-0.1.1/pyrigana/tests/test_furigana_html.py`

 * *Files identical despite different names*

### Comparing `pyrigana-0.1.0/pyrigana.egg-info/PKG-INFO` & `pyrigana-0.1.1/pyrigana.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrigana
-Version: 0.1.0
+Version: 0.1.1
 Summary: A brief description of my package
 Home-page: https://github.com/aknay/pyrigana
 Author: Nay Aung Kyaw
 Author-email: aknay@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyrigana-0.1.0/setup.py` & `pyrigana-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pyrigana',
-    version='0.1.0',
+    version='0.1.1',
     description='A brief description of my package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/aknay/pyrigana',
     author='Nay Aung Kyaw',
     author_email='aknay@outlook.com',
     license='MIT',
```

