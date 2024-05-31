# Comparing `tmp/cyclicpeptide-1.0.2.tar.gz` & `tmp/cyclicpeptide-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclicpeptide-1.0.2.tar", last modified: Fri May 31 06:52:50 2024, max compression
+gzip compressed data, was "cyclicpeptide-1.0.3.tar", last modified: Fri May 31 06:58:17 2024, max compression
```

## Comparing `cyclicpeptide-1.0.2.tar` & `cyclicpeptide-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-05-31 06:52:50.223370 cyclicpeptide-1.0.2/
--rw-r--r--   0 willow     (501) staff       (20)     1093 2024-05-31 02:24:37.000000 cyclicpeptide-1.0.2/LICENSE.md
--rw-r--r--   0 willow     (501) staff       (20)     2547 2024-05-31 06:52:50.223304 cyclicpeptide-1.0.2/PKG-INFO
--rw-r--r--   0 willow     (501) staff       (20)     1918 2024-05-31 03:28:51.000000 cyclicpeptide-1.0.2/README.md
-drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-05-31 06:52:50.222036 cyclicpeptide-1.0.2/cyclicpeptide/
--rw-r--r--   0 willow     (501) staff       (20)     1134 2024-03-07 07:35:40.000000 cyclicpeptide-1.0.2/cyclicpeptide/AminoAcids.txt
--rw-r--r--   0 willow     (501) staff       (20)     1662 2024-03-19 07:31:14.000000 cyclicpeptide-1.0.2/cyclicpeptide/Chemical_P.csv
--rwxr-xr-x   0 willow     (501) staff       (20)     5859 2024-05-24 07:25:18.000000 cyclicpeptide-1.0.2/cyclicpeptide/GraphAlignment.py
--rw-r--r--   0 willow     (501) staff       (20)     2476 2024-05-31 06:42:27.000000 cyclicpeptide-1.0.2/cyclicpeptide/IOManager.py
--rw-r--r--   0 willow     (501) staff       (20)     5380 2024-05-31 03:39:15.000000 cyclicpeptide-1.0.2/cyclicpeptide/PropertyAnalysis.py
--rwxr-xr-x   0 willow     (501) staff       (20)     9972 2024-05-31 06:52:09.000000 cyclicpeptide-1.0.2/cyclicpeptide/Sequence2Structure.py
--rw-r--r--   0 willow     (501) staff       (20)    11017 2024-05-13 03:22:59.000000 cyclicpeptide-1.0.2/cyclicpeptide/SequenceTransformer.py
--rwxr-xr-x   0 willow     (501) staff       (20)    39456 2024-05-31 06:52:29.000000 cyclicpeptide-1.0.2/cyclicpeptide/Structure2Sequence.py
--rw-r--r--   0 willow     (501) staff       (20)     2476 2024-04-08 03:27:53.000000 cyclicpeptide-1.0.2/cyclicpeptide/StructureTransformer.py
--rw-r--r--   0 willow     (501) staff       (20)        0 2024-05-31 02:15:42.000000 cyclicpeptide-1.0.2/cyclicpeptide/__init__.py
--rw-r--r--   0 willow     (501) staff       (20)      502 2024-03-08 01:11:36.000000 cyclicpeptide-1.0.2/cyclicpeptide/aa_smiles.txt
--rw-r--r--   0 willow     (501) staff       (20)      116 2024-03-08 01:12:56.000000 cyclicpeptide-1.0.2/cyclicpeptide/aas.txt
-drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-05-31 06:52:50.223029 cyclicpeptide-1.0.2/cyclicpeptide.egg-info/
--rw-r--r--   0 willow     (501) staff       (20)     2547 2024-05-31 06:52:50.000000 cyclicpeptide-1.0.2/cyclicpeptide.egg-info/PKG-INFO
--rw-r--r--   0 willow     (501) staff       (20)      597 2024-05-31 06:52:50.000000 cyclicpeptide-1.0.2/cyclicpeptide.egg-info/SOURCES.txt
--rw-r--r--   0 willow     (501) staff       (20)        1 2024-05-31 06:52:50.000000 cyclicpeptide-1.0.2/cyclicpeptide.egg-info/dependency_links.txt
--rw-r--r--   0 willow     (501) staff       (20)       92 2024-05-31 06:52:50.000000 cyclicpeptide-1.0.2/cyclicpeptide.egg-info/requires.txt
--rw-r--r--   0 willow     (501) staff       (20)       14 2024-05-31 06:52:50.000000 cyclicpeptide-1.0.2/cyclicpeptide.egg-info/top_level.txt
--rw-r--r--   0 willow     (501) staff       (20)       78 2024-05-31 06:52:50.223606 cyclicpeptide-1.0.2/setup.cfg
--rw-r--r--   0 willow     (501) staff       (20)     1099 2024-05-31 06:52:45.000000 cyclicpeptide-1.0.2/setup.py
+drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-05-31 06:58:17.004096 cyclicpeptide-1.0.3/
+-rw-r--r--   0 willow     (501) staff       (20)     1093 2024-05-31 02:24:37.000000 cyclicpeptide-1.0.3/LICENSE.md
+-rw-r--r--   0 willow     (501) staff       (20)     2571 2024-05-31 06:58:17.004024 cyclicpeptide-1.0.3/PKG-INFO
+-rw-r--r--   0 willow     (501) staff       (20)     1918 2024-05-31 03:28:51.000000 cyclicpeptide-1.0.3/README.md
+drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-05-31 06:58:17.002242 cyclicpeptide-1.0.3/cyclicpeptide/
+-rw-r--r--   0 willow     (501) staff       (20)     1134 2024-03-07 07:35:40.000000 cyclicpeptide-1.0.3/cyclicpeptide/AminoAcids.txt
+-rw-r--r--   0 willow     (501) staff       (20)     1662 2024-03-19 07:31:14.000000 cyclicpeptide-1.0.3/cyclicpeptide/Chemical_P.csv
+-rwxr-xr-x   0 willow     (501) staff       (20)     5859 2024-05-24 07:25:18.000000 cyclicpeptide-1.0.3/cyclicpeptide/GraphAlignment.py
+-rw-r--r--   0 willow     (501) staff       (20)     2476 2024-05-31 06:42:27.000000 cyclicpeptide-1.0.3/cyclicpeptide/IOManager.py
+-rw-r--r--   0 willow     (501) staff       (20)     5380 2024-05-31 03:39:15.000000 cyclicpeptide-1.0.3/cyclicpeptide/PropertyAnalysis.py
+-rwxr-xr-x   0 willow     (501) staff       (20)     9972 2024-05-31 06:52:09.000000 cyclicpeptide-1.0.3/cyclicpeptide/Sequence2Structure.py
+-rw-r--r--   0 willow     (501) staff       (20)    11017 2024-05-13 03:22:59.000000 cyclicpeptide-1.0.3/cyclicpeptide/SequenceTransformer.py
+-rwxr-xr-x   0 willow     (501) staff       (20)    39456 2024-05-31 06:52:29.000000 cyclicpeptide-1.0.3/cyclicpeptide/Structure2Sequence.py
+-rw-r--r--   0 willow     (501) staff       (20)     2476 2024-04-08 03:27:53.000000 cyclicpeptide-1.0.3/cyclicpeptide/StructureTransformer.py
+-rw-r--r--   0 willow     (501) staff       (20)        0 2024-05-31 02:15:42.000000 cyclicpeptide-1.0.3/cyclicpeptide/__init__.py
+-rw-r--r--   0 willow     (501) staff       (20)      502 2024-03-08 01:11:36.000000 cyclicpeptide-1.0.3/cyclicpeptide/aa_smiles.txt
+-rw-r--r--   0 willow     (501) staff       (20)      116 2024-03-08 01:12:56.000000 cyclicpeptide-1.0.3/cyclicpeptide/aas.txt
+-rw-r--r--   0 willow     (501) staff       (20)    79050 2024-05-28 02:09:41.000000 cyclicpeptide-1.0.3/cyclicpeptide/monomer.tsv
+drwxr-xr-x   0 willow     (501) staff       (20)        0 2024-05-31 06:58:17.003740 cyclicpeptide-1.0.3/cyclicpeptide.egg-info/
+-rw-r--r--   0 willow     (501) staff       (20)     2571 2024-05-31 06:58:16.000000 cyclicpeptide-1.0.3/cyclicpeptide.egg-info/PKG-INFO
+-rw-r--r--   0 willow     (501) staff       (20)      623 2024-05-31 06:58:16.000000 cyclicpeptide-1.0.3/cyclicpeptide.egg-info/SOURCES.txt
+-rw-r--r--   0 willow     (501) staff       (20)        1 2024-05-31 06:58:16.000000 cyclicpeptide-1.0.3/cyclicpeptide.egg-info/dependency_links.txt
+-rw-r--r--   0 willow     (501) staff       (20)       92 2024-05-31 06:58:16.000000 cyclicpeptide-1.0.3/cyclicpeptide.egg-info/requires.txt
+-rw-r--r--   0 willow     (501) staff       (20)       14 2024-05-31 06:58:16.000000 cyclicpeptide-1.0.3/cyclicpeptide.egg-info/top_level.txt
+-rw-r--r--   0 willow     (501) staff       (20)       78 2024-05-31 06:58:17.004350 cyclicpeptide-1.0.3/setup.cfg
+-rw-r--r--   0 willow     (501) staff       (20)     1124 2024-05-31 06:57:47.000000 cyclicpeptide-1.0.3/setup.py
```

### Comparing `cyclicpeptide-1.0.2/LICENSE.md` & `cyclicpeptide-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.2/PKG-INFO` & `cyclicpeptide-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cyclicpeptide
-Version: 1.0.2
-Summary: A simple example package
+Version: 1.0.3
+Summary: A python package for cyclic peptides drug design
 Home-page: https://github.com/Willow0316/cyclicpeptide/tree/master
 Author: Willow
 Author-email: willow.yang.b@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cyclicpeptide-1.0.2/README.md` & `cyclicpeptide-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.2/cyclicpeptide/AminoAcids.txt` & `cyclicpeptide-1.0.3/cyclicpeptide/AminoAcids.txt`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.2/cyclicpeptide/Chemical_P.csv` & `cyclicpeptide-1.0.3/cyclicpeptide/Chemical_P.csv`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.2/cyclicpeptide/GraphAlignment.py` & `cyclicpeptide-1.0.3/cyclicpeptide/GraphAlignment.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.2/cyclicpeptide/IOManager.py` & `cyclicpeptide-1.0.3/cyclicpeptide/IOManager.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.2/cyclicpeptide/PropertyAnalysis.py` & `cyclicpeptide-1.0.3/cyclicpeptide/PropertyAnalysis.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.2/cyclicpeptide/Sequence2Structure.py` & `cyclicpeptide-1.0.3/cyclicpeptide/Sequence2Structure.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.2/cyclicpeptide/SequenceTransformer.py` & `cyclicpeptide-1.0.3/cyclicpeptide/SequenceTransformer.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.2/cyclicpeptide/Structure2Sequence.py` & `cyclicpeptide-1.0.3/cyclicpeptide/Structure2Sequence.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.2/cyclicpeptide/StructureTransformer.py` & `cyclicpeptide-1.0.3/cyclicpeptide/StructureTransformer.py`

 * *Files identical despite different names*

### Comparing `cyclicpeptide-1.0.2/cyclicpeptide.egg-info/PKG-INFO` & `cyclicpeptide-1.0.3/cyclicpeptide.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cyclicpeptide
-Version: 1.0.2
-Summary: A simple example package
+Version: 1.0.3
+Summary: A python package for cyclic peptides drug design
 Home-page: https://github.com/Willow0316/cyclicpeptide/tree/master
 Author: Willow
 Author-email: willow.yang.b@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cyclicpeptide-1.0.2/cyclicpeptide.egg-info/SOURCES.txt` & `cyclicpeptide-1.0.3/cyclicpeptide.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -10,12 +10,13 @@
 cyclicpeptide/Sequence2Structure.py
 cyclicpeptide/SequenceTransformer.py
 cyclicpeptide/Structure2Sequence.py
 cyclicpeptide/StructureTransformer.py
 cyclicpeptide/__init__.py
 cyclicpeptide/aa_smiles.txt
 cyclicpeptide/aas.txt
+cyclicpeptide/monomer.tsv
 cyclicpeptide.egg-info/PKG-INFO
 cyclicpeptide.egg-info/SOURCES.txt
 cyclicpeptide.egg-info/dependency_links.txt
 cyclicpeptide.egg-info/requires.txt
 cyclicpeptide.egg-info/top_level.txt
```

### Comparing `cyclicpeptide-1.0.2/setup.py` & `cyclicpeptide-1.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setup(
     name='cyclicpeptide',
-    version='1.0.2',
+    version='1.0.3',
     packages=find_packages(),
-    description='A simple example package',
+    description='A python package for cyclic peptides drug design',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Willow0316/cyclicpeptide/tree/master',
     author='Willow',
     author_email='willow.yang.b@gmail.com',
     python_requires='>=3.8',  # Python 版本要求
     license='MIT',
@@ -24,10 +24,10 @@
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.8',
     ],
-    package_data={'': ['*.csv', '*.txt','.tsv']}, #这个很重要
+    package_data={'': ['*.csv', '*.txt','*.tsv']}, #这个很重要
     include_package_data=True #也选上
 )
```

