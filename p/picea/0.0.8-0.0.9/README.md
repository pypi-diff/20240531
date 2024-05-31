# Comparing `tmp/picea-0.0.8.tar.gz` & `tmp/picea-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/picea-0.0.8.tar", last modified: Tue Jun 30 13:22:35 2020, max compression
+gzip compressed data, was "dist/picea-0.0.9.tar", last modified: Thu Jul  2 06:26:37 2020, max compression
```

## Comparing `picea-0.0.8.tar` & `picea-0.0.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-06-30 13:22:35.000000 picea-0.0.8/
--rw-r--r--   0 rensholmer   (501) staff       (20)       74 2019-06-07 12:54:58.000000 picea-0.0.8/.coveragerc
-drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-06-30 13:22:35.000000 picea-0.0.8/.github/
-drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-06-30 13:22:35.000000 picea-0.0.8/.github/workflows/
--rw-r--r--   0 rensholmer   (501) staff       (20)      378 2020-06-30 11:55:00.000000 picea-0.0.8/.github/workflows/docs.yml
--rw-r--r--   0 rensholmer   (501) staff       (20)     1303 2020-06-30 11:48:58.000000 picea-0.0.8/.github/workflows/tests.yml
--rw-r--r--   0 rensholmer   (501) staff       (20)     1221 2020-06-12 07:53:26.000000 picea-0.0.8/.gitignore
--rw-r--r--   0 rensholmer   (501) staff       (20)        1 2020-06-30 11:48:16.000000 picea-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 rensholmer   (501) staff       (20)    35149 2019-06-07 12:46:29.000000 picea-0.0.8/LICENSE
--rw-r--r--   0 rensholmer   (501) staff       (20)      303 2020-06-30 13:22:35.000000 picea-0.0.8/PKG-INFO
--rw-r--r--   0 rensholmer   (501) staff       (20)     1476 2020-06-29 11:19:34.000000 picea-0.0.8/README.md
-drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-06-30 13:22:35.000000 picea-0.0.8/docs/
-drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-06-30 13:22:35.000000 picea-0.0.8/docs/API/
--rw-r--r--   0 rensholmer   (501) staff       (20)      182 2020-06-29 10:28:22.000000 picea-0.0.8/docs/API/sequence.md
--rw-r--r--   0 rensholmer   (501) staff       (20)       39 2020-06-29 10:28:16.000000 picea-0.0.8/docs/API/tree.md
--rw-r--r--   0 rensholmer   (501) staff       (20)      638 2019-07-01 12:26:26.000000 picea-0.0.8/docs/Makefile
--rw-r--r--   0 rensholmer   (501) staff       (20)      189 2020-06-30 11:46:44.000000 picea-0.0.8/docs/README.md
--rw-r--r--   0 rensholmer   (501) staff       (20)    19613 2019-07-03 08:40:44.000000 picea-0.0.8/docs/example1.png
--rw-r--r--   0 rensholmer   (501) staff       (20)     1476 2020-06-29 11:19:34.000000 picea-0.0.8/docs/index.md
--rw-r--r--   0 rensholmer   (501) staff       (20)      799 2019-07-01 12:26:26.000000 picea-0.0.8/docs/make.bat
--rw-r--r--   0 rensholmer   (501) staff       (20)       12 2020-06-30 11:46:44.000000 picea-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-06-30 13:22:35.000000 picea-0.0.8/docs/source/
--rw-r--r--   0 rensholmer   (501) staff       (20)      242 2019-07-01 14:07:29.000000 picea-0.0.8/docs/source/api-documentation.rst
--rw-r--r--   0 rensholmer   (501) staff       (20)     1991 2019-07-01 14:11:35.000000 picea-0.0.8/docs/source/conf.py
--rw-r--r--   0 rensholmer   (501) staff       (20)      428 2019-07-01 13:32:42.000000 picea-0.0.8/docs/source/index.rst
--rw-r--r--   0 rensholmer   (501) staff       (20)      255 2019-07-01 13:17:19.000000 picea-0.0.8/docs/source/installation.rst
-drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-06-30 13:22:35.000000 picea-0.0.8/examples/
-drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-06-30 13:22:35.000000 picea-0.0.8/examples/data/
--rw-r--r--   0 rensholmer   (501) staff       (20)    18905 2020-06-25 06:07:02.000000 picea-0.0.8/examples/data/HCT.fasta
--rw-r--r--   0 rensholmer   (501) staff       (20)     3145 2020-06-25 13:54:21.000000 picea-0.0.8/examples/data/genemodel.gff3
--rw-r--r--   0 rensholmer   (501) staff       (20)    10579 2020-06-25 10:41:42.000000 picea-0.0.8/examples/data/genemodel.json
--rw-r--r--   0 rensholmer   (501) staff       (20)    24723 2020-06-25 14:36:25.000000 picea-0.0.8/examples/data/multiple_sequence_alignment.fasta
--rw-r--r--   0 rensholmer   (501) staff       (20)    26489 2020-06-25 14:21:49.000000 picea-0.0.8/examples/data/multiple_sequence_alignment.json
--rw-r--r--   0 rensholmer   (501) staff       (20)    22566 2020-06-26 06:52:56.000000 picea-0.0.8/examples/data/tree.json
--rw-r--r--   0 rensholmer   (501) staff       (20)     2181 2020-06-26 06:47:31.000000 picea-0.0.8/examples/data/tree.newick
--rw-r--r--   0 rensholmer   (501) staff       (20)    32018 2020-06-26 05:40:06.000000 picea-0.0.8/examples/sequence annotation.ipynb
--rw-r--r--   0 rensholmer   (501) staff       (20)   281877 2020-06-25 14:48:50.000000 picea-0.0.8/examples/sequence collection.ipynb
--rw-r--r--   0 rensholmer   (501) staff       (20)    68146 2020-06-26 06:49:54.000000 picea-0.0.8/examples/tree.ipynb
--rw-r--r--   0 rensholmer   (501) staff       (20)      281 2020-06-29 10:30:38.000000 picea-0.0.8/mkdocs.yml
-drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-06-30 13:22:35.000000 picea-0.0.8/picea/
--rw-r--r--   0 rensholmer   (501) staff       (20)      248 2020-06-30 11:58:15.000000 picea-0.0.8/picea/__init__.py
--rw-r--r--   0 rensholmer   (501) staff       (20)    29336 2020-06-28 05:21:48.000000 picea-0.0.8/picea/sequence.py
--rw-r--r--   0 rensholmer   (501) staff       (20)    11743 2020-06-26 14:35:00.000000 picea-0.0.8/picea/tree.py
-drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-06-30 13:22:35.000000 picea-0.0.8/picea.egg-info/
--rw-r--r--   0 rensholmer   (501) staff       (20)      303 2020-06-30 13:22:34.000000 picea-0.0.8/picea.egg-info/PKG-INFO
--rw-r--r--   0 rensholmer   (501) staff       (20)      979 2020-06-30 13:22:34.000000 picea-0.0.8/picea.egg-info/SOURCES.txt
--rw-r--r--   0 rensholmer   (501) staff       (20)        1 2020-06-30 13:22:34.000000 picea-0.0.8/picea.egg-info/dependency_links.txt
--rw-r--r--   0 rensholmer   (501) staff       (20)       24 2020-06-30 13:22:34.000000 picea-0.0.8/picea.egg-info/requires.txt
--rw-r--r--   0 rensholmer   (501) staff       (20)        6 2020-06-30 13:22:34.000000 picea-0.0.8/picea.egg-info/top_level.txt
--rw-r--r--   0 rensholmer   (501) staff       (20)       22 2020-06-30 11:55:06.000000 picea-0.0.8/requirements.txt
--rw-r--r--   0 rensholmer   (501) staff       (20)      230 2020-06-30 13:22:35.000000 picea-0.0.8/setup.cfg
--rw-r--r--   0 rensholmer   (501) staff       (20)      986 2020-06-30 11:58:58.000000 picea-0.0.8/setup.py
-drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-06-30 13:22:35.000000 picea-0.0.8/tests/
--rw-r--r--   0 rensholmer   (501) staff       (20)      173 2019-09-05 09:41:52.000000 picea-0.0.8/tests/annotation_tests.py
--rw-r--r--   0 rensholmer   (501) staff       (20)     1860 2020-06-26 06:15:26.000000 picea-0.0.8/tests/sequence_tests.py
--rw-r--r--   0 rensholmer   (501) staff       (20)      299 2019-07-03 08:56:32.000000 picea-0.0.8/tests/tree_tests.py
+drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-07-02 06:26:37.000000 picea-0.0.9/
+-rw-r--r--   0 rensholmer   (501) staff       (20)       74 2019-06-07 12:54:58.000000 picea-0.0.9/.coveragerc
+drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-07-02 06:26:37.000000 picea-0.0.9/.github/
+drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-07-02 06:26:37.000000 picea-0.0.9/.github/workflows/
+-rw-r--r--   0 rensholmer   (501) staff       (20)      378 2020-06-30 11:55:00.000000 picea-0.0.9/.github/workflows/docs.yml
+-rw-r--r--   0 rensholmer   (501) staff       (20)     1303 2020-06-30 11:48:58.000000 picea-0.0.9/.github/workflows/tests.yml
+-rw-r--r--   0 rensholmer   (501) staff       (20)     1221 2020-06-12 07:53:26.000000 picea-0.0.9/.gitignore
+-rw-r--r--   0 rensholmer   (501) staff       (20)        1 2020-06-30 11:48:16.000000 picea-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 rensholmer   (501) staff       (20)    35149 2019-06-07 12:46:29.000000 picea-0.0.9/LICENSE
+-rw-r--r--   0 rensholmer   (501) staff       (20)      303 2020-07-02 06:26:37.000000 picea-0.0.9/PKG-INFO
+-rw-r--r--   0 rensholmer   (501) staff       (20)     1475 2020-06-30 15:08:16.000000 picea-0.0.9/README.md
+drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-07-02 06:26:37.000000 picea-0.0.9/docs/
+drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-07-02 06:26:37.000000 picea-0.0.9/docs/API/
+-rw-r--r--   0 rensholmer   (501) staff       (20)      166 2020-06-30 15:11:06.000000 picea-0.0.9/docs/API/sequence.md
+-rw-r--r--   0 rensholmer   (501) staff       (20)       39 2020-06-29 10:28:16.000000 picea-0.0.9/docs/API/tree.md
+-rw-r--r--   0 rensholmer   (501) staff       (20)      638 2019-07-01 12:26:26.000000 picea-0.0.9/docs/Makefile
+-rw-r--r--   0 rensholmer   (501) staff       (20)      189 2020-06-30 11:46:44.000000 picea-0.0.9/docs/README.md
+-rw-r--r--   0 rensholmer   (501) staff       (20)    19613 2019-07-03 08:40:44.000000 picea-0.0.9/docs/example1.png
+-rw-r--r--   0 rensholmer   (501) staff       (20)     1475 2020-06-30 15:08:16.000000 picea-0.0.9/docs/index.md
+-rw-r--r--   0 rensholmer   (501) staff       (20)      799 2019-07-01 12:26:26.000000 picea-0.0.9/docs/make.bat
+-rw-r--r--   0 rensholmer   (501) staff       (20)       12 2020-06-30 11:46:44.000000 picea-0.0.9/docs/requirements.txt
+drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-07-02 06:26:37.000000 picea-0.0.9/docs/source/
+-rw-r--r--   0 rensholmer   (501) staff       (20)      242 2019-07-01 14:07:29.000000 picea-0.0.9/docs/source/api-documentation.rst
+-rw-r--r--   0 rensholmer   (501) staff       (20)     1991 2019-07-01 14:11:35.000000 picea-0.0.9/docs/source/conf.py
+-rw-r--r--   0 rensholmer   (501) staff       (20)      428 2019-07-01 13:32:42.000000 picea-0.0.9/docs/source/index.rst
+-rw-r--r--   0 rensholmer   (501) staff       (20)      255 2019-07-01 13:17:19.000000 picea-0.0.9/docs/source/installation.rst
+drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-07-02 06:26:37.000000 picea-0.0.9/examples/
+drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-07-02 06:26:37.000000 picea-0.0.9/examples/data/
+-rw-r--r--   0 rensholmer   (501) staff       (20)    18905 2020-06-25 06:07:02.000000 picea-0.0.9/examples/data/HCT.fasta
+-rw-r--r--   0 rensholmer   (501) staff       (20)     3145 2020-06-25 13:54:21.000000 picea-0.0.9/examples/data/genemodel.gff3
+-rw-r--r--   0 rensholmer   (501) staff       (20)    10579 2020-06-25 10:41:42.000000 picea-0.0.9/examples/data/genemodel.json
+-rw-r--r--   0 rensholmer   (501) staff       (20)    24723 2020-06-25 14:36:25.000000 picea-0.0.9/examples/data/multiple_sequence_alignment.fasta
+-rw-r--r--   0 rensholmer   (501) staff       (20)    26489 2020-06-25 14:21:49.000000 picea-0.0.9/examples/data/multiple_sequence_alignment.json
+-rw-r--r--   0 rensholmer   (501) staff       (20)    22566 2020-06-26 06:52:56.000000 picea-0.0.9/examples/data/tree.json
+-rw-r--r--   0 rensholmer   (501) staff       (20)     2181 2020-06-26 06:47:31.000000 picea-0.0.9/examples/data/tree.newick
+-rw-r--r--   0 rensholmer   (501) staff       (20)    32018 2020-06-26 05:40:06.000000 picea-0.0.9/examples/sequence annotation.ipynb
+-rw-r--r--   0 rensholmer   (501) staff       (20)   281877 2020-06-25 14:48:50.000000 picea-0.0.9/examples/sequence collection.ipynb
+-rw-r--r--   0 rensholmer   (501) staff       (20)    68146 2020-06-26 06:49:54.000000 picea-0.0.9/examples/tree.ipynb
+-rw-r--r--   0 rensholmer   (501) staff       (20)      281 2020-06-29 10:30:38.000000 picea-0.0.9/mkdocs.yml
+drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-07-02 06:26:37.000000 picea-0.0.9/picea/
+-rw-r--r--   0 rensholmer   (501) staff       (20)      248 2020-07-02 06:26:05.000000 picea-0.0.9/picea/__init__.py
+-rw-r--r--   0 rensholmer   (501) staff       (20)    29336 2020-06-28 05:21:48.000000 picea-0.0.9/picea/sequence.py
+-rw-r--r--   0 rensholmer   (501) staff       (20)    12174 2020-07-02 06:25:22.000000 picea-0.0.9/picea/tree.py
+drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-07-02 06:26:37.000000 picea-0.0.9/picea.egg-info/
+-rw-r--r--   0 rensholmer   (501) staff       (20)      303 2020-07-02 06:26:37.000000 picea-0.0.9/picea.egg-info/PKG-INFO
+-rw-r--r--   0 rensholmer   (501) staff       (20)      979 2020-07-02 06:26:37.000000 picea-0.0.9/picea.egg-info/SOURCES.txt
+-rw-r--r--   0 rensholmer   (501) staff       (20)        1 2020-07-02 06:26:37.000000 picea-0.0.9/picea.egg-info/dependency_links.txt
+-rw-r--r--   0 rensholmer   (501) staff       (20)       24 2020-07-02 06:26:37.000000 picea-0.0.9/picea.egg-info/requires.txt
+-rw-r--r--   0 rensholmer   (501) staff       (20)        6 2020-07-02 06:26:37.000000 picea-0.0.9/picea.egg-info/top_level.txt
+-rw-r--r--   0 rensholmer   (501) staff       (20)       22 2020-06-30 11:55:06.000000 picea-0.0.9/requirements.txt
+-rw-r--r--   0 rensholmer   (501) staff       (20)      230 2020-07-02 06:26:37.000000 picea-0.0.9/setup.cfg
+-rw-r--r--   0 rensholmer   (501) staff       (20)      986 2020-06-30 11:58:58.000000 picea-0.0.9/setup.py
+drwxr-xr-x   0 rensholmer   (501) staff       (20)        0 2020-07-02 06:26:37.000000 picea-0.0.9/tests/
+-rw-r--r--   0 rensholmer   (501) staff       (20)      173 2019-09-05 09:41:52.000000 picea-0.0.9/tests/annotation_tests.py
+-rw-r--r--   0 rensholmer   (501) staff       (20)     1860 2020-06-26 06:15:26.000000 picea-0.0.9/tests/sequence_tests.py
+-rw-r--r--   0 rensholmer   (501) staff       (20)      299 2019-07-03 08:56:32.000000 picea-0.0.9/tests/tree_tests.py
```

### Comparing `picea-0.0.8/.github/workflows/tests.yml` & `picea-0.0.9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/.gitignore` & `picea-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/LICENSE` & `picea-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/README.md` & `picea-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![Coverage Status](https://coveralls.io/repos/github/holmrenser/picea/badge.svg?branch=master)](https://coveralls.io/github/holmrenser/picea?branch=master)
 [![PyPI version](https://badge.fury.io/py/picea.svg)](https://badge.fury.io/py/picea)
 
 ```
 pip install picea
 ```
 
-![example figure](https://github.com/holmrenser/picea/blob/master/docs/example1.png)
+![example figure](https://github.com/holmrenser/picea/raw/master/docs/example1.png)
 
 The above figure can be generated with the following code
 
 ```python
 from picea import Tree
 import matplotlib.pyplot as plt
```

### Comparing `picea-0.0.8/docs/Makefile` & `picea-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/docs/example1.png` & `picea-0.0.9/docs/example1.png`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/docs/index.md` & `picea-0.0.9/docs/index.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![Coverage Status](https://coveralls.io/repos/github/holmrenser/picea/badge.svg?branch=master)](https://coveralls.io/github/holmrenser/picea?branch=master)
 [![PyPI version](https://badge.fury.io/py/picea.svg)](https://badge.fury.io/py/picea)
 
 ```
 pip install picea
 ```
 
-![example figure](https://github.com/holmrenser/picea/blob/master/docs/example1.png)
+![example figure](https://github.com/holmrenser/picea/raw/master/docs/example1.png)
 
 The above figure can be generated with the following code
 
 ```python
 from picea import Tree
 import matplotlib.pyplot as plt
```

### Comparing `picea-0.0.8/docs/make.bat` & `picea-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/docs/source/conf.py` & `picea-0.0.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/examples/data/HCT.fasta` & `picea-0.0.9/examples/data/HCT.fasta`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/examples/data/genemodel.gff3` & `picea-0.0.9/examples/data/genemodel.gff3`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/examples/data/genemodel.json` & `picea-0.0.9/examples/data/genemodel.json`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/examples/data/multiple_sequence_alignment.fasta` & `picea-0.0.9/examples/data/multiple_sequence_alignment.fasta`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/examples/data/multiple_sequence_alignment.json` & `picea-0.0.9/examples/data/multiple_sequence_alignment.json`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/examples/data/tree.json` & `picea-0.0.9/examples/data/tree.json`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/examples/data/tree.newick` & `picea-0.0.9/examples/data/tree.newick`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/examples/sequence annotation.ipynb` & `picea-0.0.9/examples/sequence annotation.ipynb`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/examples/sequence collection.ipynb` & `picea-0.0.9/examples/sequence collection.ipynb`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/examples/tree.ipynb` & `picea-0.0.9/examples/tree.ipynb`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/picea/sequence.py` & `picea-0.0.9/picea/sequence.py`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/picea/tree.py` & `picea-0.0.9/picea/tree.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import re
-from typing import Iterable, Callable, List, Optional
+from typing import \
+    Iterable, Callable, List, Optional, Generator, Dict, Union, Tuple
 import json
 
+TreeDict = Dict[str, Union[str, int, float, List[Optional['TreeDict']]]]
+
 
 def unequal_separation(
     node_a: 'Tree',
     node_b: 'Tree',
     sep_1: float = 1.0,
     sep_2: float = 2.0
 ) -> float:
@@ -74,22 +77,22 @@
     """
     return node.name == name
 
 
 class Tree:
     def __init__(
         self,
-        ID: int = None,
-        children: List['Tree'] = None,
+        ID: Optional[int] = None,
+        children: Optional[List['Tree']] = None,
         # x: float = 0.0,
         # y: float = 0.0,
         name: str = '',
         length: float = 0.0,
-        depth: float = None,
-        parent: 'Tree' = None,
+        depth: Optional[int] = None,
+        parent: Optional['Tree'] = None,
         cumulative_length: float = 0.0
     ):
         """Recursive datastructure holding tree objects
 
         Args:
             ID (int, optional): [description]. Defaults to None.
             children (list, optional): [description]. Defaults to None.
@@ -116,15 +119,15 @@
     def __repr__(self):
         return (
             f'<TreeNode ID={self.ID} depth={self.depth}'
             f' length={self.length} name={str(self.name)}>'
         )
 
     @property
-    def loc(self):
+    def loc(self) -> 'Tree':
         """Name based index
 
         Example:
             >>> from picea import Tree
             >>> newick = '(((a,b),(c,d)),e);'
             >>> tree = Tree.from_newick(newick)
             >>> tree.loc['a']
@@ -135,15 +138,15 @@
 
         Raises:
             IndexError
         """
         return TreeIndex(iterator=self.depth_first, eq_func=name_equals)
 
     @property
-    def iloc(self):
+    def iloc(self) -> 'Tree':
         """Index based index
 
         Example:
             >>> from picea import Tree
             >>> newick = '(((a,b),(c,d)),e);'
             >>> tree = Tree.from_newick(newick)
             >>> tree.iloc[1]
@@ -151,33 +154,33 @@
 
         Returns:
             Tree: tree node matching index
         """
         return TreeIndex(iterator=self.depth_first, eq_func=index_equals)
 
     @property
-    def nodes(self):
+    def nodes(self) -> List['Tree']:
         """A list of all tree nodes in breadth-first order
 
         Returns:
             list: A list of all tree nodes
         """
         return list(self.breadth_first())
 
     @property
-    def leaves(self):
+    def leaves(self) -> List['Tree']:
         """A list of leaf nodes only
 
         Returns:
             list: A list of leaf nodes only
         """
         return [n for n in self.nodes if not n.children]
 
     @property
-    def links(self):
+    def links(self) -> List[Tuple['Tree', 'Tree']]:
         """A list of all (parent, child) combinations
 
         Returns:
             list: All (parent,child) combinations
         """
         _links = []
         for node in self.nodes:
@@ -187,15 +190,15 @@
         return _links
 
     @classmethod
     def from_newick(
         cls,
         string: Optional[str] = None,
         filename: Optional[str] = None
-    ):
+    ) -> 'Tree':
         """Parse a newick formatted string into a Tree object
 
         Arguments:
             newick_string (string): Newick formatted tree string
 
         Returns:
             Tree: Tree object
@@ -241,15 +244,15 @@
             queue += node.children
 
         return tree
 
     def to_newick(
         self,
         branch_lengths: bool = True
-    ):
+    ) -> str:
         """Make a Newick formatted string
 
         Args:
             branch_lengths (bool, optional): Whether to include branch lengths\
              in the Newick string. Defaults to True.
 
         Returns:
@@ -275,15 +278,15 @@
 
         return newick
 
     @classmethod
     def from_sklearn(
         cls,
         clustering
-    ):
+    ) -> 'Tree':
         """Read a tree from sklearn agglomerative clustering
 
         Args:
             clustering (sklearn object): sklearn agglomerative clustering\
                  object.
 
         Returns:
@@ -312,41 +315,46 @@
         raise NotImplementedError()
 
     @classmethod
     def from_json(cls):
         # TODO
         raise NotImplementedError()
 
-    def to_json(self, indent: Optional[int] = None):
+    def to_json(self, indent: Optional[int] = None) -> str:
         return json.dumps(self.to_dict(), indent=indent)
 
     @classmethod
     def from_dict(cls):
         # TODO
         raise NotImplementedError()
 
-    def to_dict(self):
+    def to_dict(self) -> TreeDict:
+        """[summary]
+
+        Returns:
+            TreeDict: [description]
+        """
         return dict(
             ID=self.ID, name=self.name, length=self.length,
             children=[child.to_dict() for child in self.children]
         )
 
-    def breadth_first(self):
+    def breadth_first(self) -> Generator['Tree', None, None]:
         """Generator implementing breadth first search starting at root node
         """
         queue = [self]
         while queue:
             node = queue.pop(0)
             queue += node.children
             yield node
 
     def depth_first(
         self,
         post_order: bool = True
-    ):
+    ) -> Generator['Tree', None, None]:
         """Generator implementing depth first search in either post- or
         pre-order traversel
 
         Keyword Arguments:
             post_order (bool, optional): Depth first search in post-order
             traversal or not. Defaults to True
         """
```

### Comparing `picea-0.0.8/picea.egg-info/SOURCES.txt` & `picea-0.0.9/picea.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/setup.py` & `picea-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `picea-0.0.8/tests/sequence_tests.py` & `picea-0.0.9/tests/sequence_tests.py`

 * *Files identical despite different names*

