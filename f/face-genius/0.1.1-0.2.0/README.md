# Comparing `tmp/face_genius-0.1.1.tar.gz` & `tmp/face_genius-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "face_genius-0.1.1.tar", last modified: Fri May 17 15:39:04 2024, max compression
+gzip compressed data, was "face_genius-0.2.0.tar", last modified: Fri May 31 14:32:28 2024, max compression
```

## Comparing `face_genius-0.1.1.tar` & `face_genius-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 15:39:04.168555 face_genius-0.1.1/
--rw-rw-rw-   0        0        0      482 2024-05-17 15:39:04.166557 face_genius-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       24 2024-05-17 15:34:54.000000 face_genius-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 15:39:04.128555 face_genius-0.1.1/face_genius/
--rw-rw-rw-   0        0        0       83 2024-05-17 14:37:03.000000 face_genius-0.1.1/face_genius/__init__.py
--rw-rw-rw-   0        0        0      385 2024-05-17 14:38:04.000000 face_genius-0.1.1/face_genius/face_recognizer_module.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:39:04.161559 face_genius-0.1.1/face_genius.egg-info/
--rw-rw-rw-   0        0        0      482 2024-05-17 15:39:03.000000 face_genius-0.1.1/face_genius.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-05-17 15:39:04.000000 face_genius-0.1.1/face_genius.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 15:39:03.000000 face_genius-0.1.1/face_genius.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-17 15:39:03.000000 face_genius-0.1.1/face_genius.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-17 15:39:03.000000 face_genius-0.1.1/face_genius.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-17 15:39:04.169556 face_genius-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      675 2024-05-17 15:37:23.000000 face_genius-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 15:39:04.164558 face_genius-0.1.1/tests/
--rw-rw-rw-   0        0        0      464 2024-05-17 15:17:28.000000 face_genius-0.1.1/tests/test_face_genius.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:32:28.316600 face_genius-0.2.0/
+-rw-rw-rw-   0        0        0     1188 2024-05-31 14:32:28.314599 face_genius-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      716 2024-05-31 13:44:44.000000 face_genius-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 14:32:28.298599 face_genius-0.2.0/face_genius/
+-rw-rw-rw-   0        0        0      125 2024-05-31 13:46:20.000000 face_genius-0.2.0/face_genius/__init__.py
+-rw-rw-rw-   0        0        0      702 2024-05-31 12:09:16.000000 face_genius-0.2.0/face_genius/face_genius.py
+-rw-rw-rw-   0        0        0      235 2024-05-31 12:09:51.000000 face_genius-0.2.0/face_genius/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:32:28.312600 face_genius-0.2.0/face_genius.egg-info/
+-rw-rw-rw-   0        0        0     1188 2024-05-31 14:32:28.000000 face_genius-0.2.0/face_genius.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2024-05-31 14:32:28.000000 face_genius-0.2.0/face_genius.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 14:32:28.000000 face_genius-0.2.0/face_genius.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-31 14:32:28.000000 face_genius-0.2.0/face_genius.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-31 14:32:28.000000 face_genius-0.2.0/face_genius.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 14:32:28.316600 face_genius-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      698 2024-05-31 14:32:04.000000 face_genius-0.2.0/setup.py
```

### Comparing `face_genius-0.1.1/setup.py` & `face_genius-0.2.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 
 from setuptools import setup, find_packages
 
+
 setup(
     name="face_genius",
-    version="0.1.1",
-    author="VT",
+    version="0.2.0",
+    packages=find_packages(),
+    install_requires=[
+        "face_recognition",
+        "numpy"
+    ],
+    author="Victor Tkachev",
     author_email="vic.tkachev@gmail.com",
     description="A simple face recognition example package",
-    long_description=open("README.md").read(),
+    long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
-    url="https://github.com/victk/face_genius",
-    packages=find_packages(),
+    url="https://github.com/NeuronsUII/LizaAlert_n",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.11',
-    install_requires=[
-        "face_recognition",
-    ],
 )
```

