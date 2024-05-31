# Comparing `tmp/xtbf-0.1.2.tar.gz` & `tmp/xtbf-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtbf-0.1.2.tar", last modified: Thu Feb 15 12:07:52 2024, max compression
+gzip compressed data, was "xtbf-0.1.3.tar", last modified: Fri May 31 07:39:16 2024, max compression
```

## Comparing `xtbf-0.1.2.tar` & `xtbf-0.1.3.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-02-15 12:07:52.192109 xtbf-0.1.2/
--rw-r--r--   0 gnlop      (502) staff       (20)       12 2024-02-15 11:33:34.000000 xtbf-0.1.2/.gitignore
--rw-r--r--   0 gnlop      (502) staff       (20)       10 2024-02-10 14:18:18.000000 xtbf-0.1.2/CODEOWNERS
--rw-r--r--   0 gnlop      (502) staff       (20)     5472 2024-02-10 14:18:18.000000 xtbf-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 gnlop      (502) staff       (20)     1516 2024-02-10 14:18:18.000000 xtbf-0.1.2/LICENSE
--rw-r--r--   0 gnlop      (502) staff       (20)      717 2024-02-15 11:10:25.000000 xtbf-0.1.2/Makefile
--rw-r--r--   0 gnlop      (502) staff       (20)      474 2024-02-15 12:07:52.191916 xtbf-0.1.2/PKG-INFO
--rw-r--r--   0 gnlop      (502) staff       (20)     3544 2024-02-10 14:18:18.000000 xtbf-0.1.2/README.md
--rw-r--r--   0 gnlop      (502) staff       (20)      120 2024-02-10 14:18:18.000000 xtbf-0.1.2/conftest.py
-drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-02-15 12:07:52.179291 xtbf-0.1.2/data/
--rw-r--r--   0 gnlop      (502) staff       (20)       16 2024-02-15 11:31:40.000000 xtbf-0.1.2/data/README.txt
-drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-02-15 12:07:52.183661 xtbf-0.1.2/data/examples/
--rw-r--r--   0 gnlop      (502) staff       (20)  2193844 2024-02-15 11:09:31.000000 xtbf-0.1.2/data/examples/HIV.csv
--rw-r--r--   0 gnlop      (502) staff       (20)   282606 2024-02-15 11:09:31.000000 xtbf-0.1.2/data/examples/Lipophilicity.csv
--rw-r--r--   0 gnlop      (502) staff       (20)    32060 2024-02-15 11:09:31.000000 xtbf-0.1.2/data/examples/SAMPL.csv
--rw-r--r--   0 gnlop      (502) staff       (20)    96699 2024-02-15 11:09:31.000000 xtbf-0.1.2/data/examples/delaney-processed.csv
-drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-02-15 12:07:52.185244 xtbf-0.1.2/doc/
--rw-r--r--   0 gnlop      (502) staff       (20)      135 2024-02-10 14:18:18.000000 xtbf-0.1.2/doc/index.html
--rw-r--r--   0 gnlop      (502) staff       (20)    13759 2024-02-10 14:18:18.000000 xtbf-0.1.2/doc/log_p_parity_plot.png
--rw-r--r--   0 gnlop      (502) staff       (20)    35860 2024-02-10 14:18:18.000000 xtbf-0.1.2/doc/search.js
-drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-02-15 12:07:52.186082 xtbf-0.1.2/doc/xtbf/
--rw-r--r--   0 gnlop      (502) staff       (20)    49452 2024-02-10 14:18:18.000000 xtbf-0.1.2/doc/xtbf/parsers.html
--rw-r--r--   0 gnlop      (502) staff       (20)    52951 2024-02-10 14:18:18.000000 xtbf-0.1.2/doc/xtbf/shortcuts.html
--rw-r--r--   0 gnlop      (502) staff       (20)   154050 2024-02-10 14:18:18.000000 xtbf-0.1.2/doc/xtbf.html
--rw-r--r--   0 gnlop      (502) staff       (20)       75 2024-02-10 14:44:06.000000 xtbf-0.1.2/pytest.ini
--rw-r--r--   0 gnlop      (502) staff       (20)       26 2024-02-10 14:18:18.000000 xtbf-0.1.2/requirements.txt
--rw-r--r--   0 gnlop      (502) staff       (20)       38 2024-02-15 12:07:52.192155 xtbf-0.1.2/setup.cfg
--rw-r--r--   0 gnlop      (502) staff       (20)      697 2024-02-15 12:07:32.000000 xtbf-0.1.2/setup.py
-drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-02-15 12:07:52.189051 xtbf-0.1.2/smal/
--rw-r--r--   0 gnlop      (502) staff       (20)      843 2024-02-15 10:12:57.000000 xtbf-0.1.2/smal/__init__.py
--rw-r--r--   0 gnlop      (502) staff       (20)      752 2024-02-15 10:12:57.000000 xtbf-0.1.2/smal/all.py
--rw-r--r--   0 gnlop      (502) staff       (20)    10155 2024-02-15 10:12:57.000000 xtbf-0.1.2/smal/cluster.py
--rw-r--r--   0 gnlop      (502) staff       (20)      195 2024-02-15 10:12:57.000000 xtbf-0.1.2/smal/config.py
--rw-r--r--   0 gnlop      (502) staff       (20)     1807 2024-02-15 10:12:57.000000 xtbf-0.1.2/smal/example_datasets.py
--rw-r--r--   0 gnlop      (502) staff       (20)     1358 2024-02-15 10:12:57.000000 xtbf-0.1.2/smal/fingerprint.py
--rw-r--r--   0 gnlop      (502) staff       (20)     9809 2024-02-15 11:12:29.000000 xtbf-0.1.2/smal/io.py
--rw-r--r--   0 gnlop      (502) staff       (20)     9066 2024-02-15 11:14:53.000000 xtbf-0.1.2/smal/mol_edit.py
--rw-r--r--   0 gnlop      (502) staff       (20)    10537 2024-02-15 11:29:30.000000 xtbf-0.1.2/smal/mol_standardizer.py
--rw-r--r--   0 gnlop      (502) staff       (20)     4556 2024-02-15 11:15:56.000000 xtbf-0.1.2/smal/viz.py
-drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-02-15 12:07:52.190244 xtbf-0.1.2/xtbf/
--rw-r--r--   0 gnlop      (502) staff       (20)    12166 2024-02-15 11:14:21.000000 xtbf-0.1.2/xtbf/__init__.py
--rw-r--r--   0 gnlop      (502) staff       (20)    13904 2024-02-10 14:18:18.000000 xtbf-0.1.2/xtbf/dc_featurizer.py
--rw-r--r--   0 gnlop      (502) staff       (20)     3748 2024-02-10 14:40:13.000000 xtbf-0.1.2/xtbf/parsers.py
--rw-r--r--   0 gnlop      (502) staff       (20)    10169 2024-02-14 09:12:13.000000 xtbf-0.1.2/xtbf/shortcuts.py
-drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-02-15 12:07:52.191635 xtbf-0.1.2/xtbf.egg-info/
--rw-r--r--   0 gnlop      (502) staff       (20)      474 2024-02-15 12:07:51.000000 xtbf-0.1.2/xtbf.egg-info/PKG-INFO
--rw-r--r--   0 gnlop      (502) staff       (20)      740 2024-02-15 12:07:52.000000 xtbf-0.1.2/xtbf.egg-info/SOURCES.txt
--rw-r--r--   0 gnlop      (502) staff       (20)        1 2024-02-15 12:07:51.000000 xtbf-0.1.2/xtbf.egg-info/dependency_links.txt
--rw-r--r--   0 gnlop      (502) staff       (20)       25 2024-02-15 12:07:51.000000 xtbf-0.1.2/xtbf.egg-info/requires.txt
--rw-r--r--   0 gnlop      (502) staff       (20)       10 2024-02-15 12:07:51.000000 xtbf-0.1.2/xtbf.egg-info/top_level.txt
+drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-05-31 07:39:16.895716 xtbf-0.1.3/
+-rw-r--r--   0 gnlop      (502) staff       (20)       50 2024-02-15 17:44:00.000000 xtbf-0.1.3/.gitignore
+-rw-r--r--   0 gnlop      (502) staff       (20)       10 2024-02-10 14:18:18.000000 xtbf-0.1.3/CODEOWNERS
+-rw-r--r--   0 gnlop      (502) staff       (20)     5472 2024-02-10 14:18:18.000000 xtbf-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0 gnlop      (502) staff       (20)     1516 2024-02-10 14:18:18.000000 xtbf-0.1.3/LICENSE
+-rw-r--r--   0 gnlop      (502) staff       (20)      717 2024-02-15 11:10:25.000000 xtbf-0.1.3/Makefile
+-rw-r--r--   0 gnlop      (502) staff       (20)      531 2024-05-31 07:39:16.895310 xtbf-0.1.3/PKG-INFO
+-rw-r--r--   0 gnlop      (502) staff       (20)     3740 2024-02-15 17:49:31.000000 xtbf-0.1.3/README.md
+-rw-r--r--   0 gnlop      (502) staff       (20)      120 2024-02-10 14:18:18.000000 xtbf-0.1.3/conftest.py
+drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-05-31 07:39:16.879138 xtbf-0.1.3/data/
+-rw-r--r--   0 gnlop      (502) staff       (20)       16 2024-02-15 11:31:40.000000 xtbf-0.1.3/data/README.txt
+drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-05-31 07:39:16.882385 xtbf-0.1.3/data/examples/
+-rw-r--r--   0 gnlop      (502) staff       (20)  2193844 2024-02-15 11:09:31.000000 xtbf-0.1.3/data/examples/HIV.csv
+-rw-r--r--   0 gnlop      (502) staff       (20)   282606 2024-02-15 11:09:31.000000 xtbf-0.1.3/data/examples/Lipophilicity.csv
+-rw-r--r--   0 gnlop      (502) staff       (20)    32060 2024-02-15 11:09:31.000000 xtbf-0.1.3/data/examples/SAMPL.csv
+-rw-r--r--   0 gnlop      (502) staff       (20)    96699 2024-02-15 11:09:31.000000 xtbf-0.1.3/data/examples/delaney-processed.csv
+drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-05-31 07:39:16.884285 xtbf-0.1.3/doc/
+-rw-r--r--   0 gnlop      (502) staff       (20)      135 2024-02-10 14:18:18.000000 xtbf-0.1.3/doc/index.html
+-rw-r--r--   0 gnlop      (502) staff       (20)    13759 2024-02-10 14:18:18.000000 xtbf-0.1.3/doc/log_p_parity_plot.png
+-rw-r--r--   0 gnlop      (502) staff       (20)    35860 2024-02-10 14:18:18.000000 xtbf-0.1.3/doc/search.js
+drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-05-31 07:39:16.885434 xtbf-0.1.3/doc/xtbf/
+-rw-r--r--   0 gnlop      (502) staff       (20)    49452 2024-02-10 14:18:18.000000 xtbf-0.1.3/doc/xtbf/parsers.html
+-rw-r--r--   0 gnlop      (502) staff       (20)    52951 2024-02-10 14:18:18.000000 xtbf-0.1.3/doc/xtbf/shortcuts.html
+-rw-r--r--   0 gnlop      (502) staff       (20)   154050 2024-02-10 14:18:18.000000 xtbf-0.1.3/doc/xtbf.html
+-rw-r--r--   0 gnlop      (502) staff       (20)       75 2024-02-10 14:44:06.000000 xtbf-0.1.3/pytest.ini
+-rw-r--r--   0 gnlop      (502) staff       (20)       26 2024-02-10 14:18:18.000000 xtbf-0.1.3/requirements.txt
+-rw-r--r--   0 gnlop      (502) staff       (20)       38 2024-05-31 07:39:16.895773 xtbf-0.1.3/setup.cfg
+-rw-r--r--   0 gnlop      (502) staff       (20)      698 2024-05-31 07:33:25.000000 xtbf-0.1.3/setup.py
+drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-05-31 07:39:16.890751 xtbf-0.1.3/smal/
+-rw-r--r--   0 gnlop      (502) staff       (20)      843 2024-02-15 10:12:57.000000 xtbf-0.1.3/smal/__init__.py
+-rw-r--r--   0 gnlop      (502) staff       (20)      752 2024-02-15 10:12:57.000000 xtbf-0.1.3/smal/all.py
+-rw-r--r--   0 gnlop      (502) staff       (20)    10155 2024-02-15 10:12:57.000000 xtbf-0.1.3/smal/cluster.py
+-rw-r--r--   0 gnlop      (502) staff       (20)      188 2024-05-27 11:11:10.000000 xtbf-0.1.3/smal/config.py
+-rw-r--r--   0 gnlop      (502) staff       (20)     1296 2024-05-31 07:30:11.000000 xtbf-0.1.3/smal/descriptors.py
+-rw-r--r--   0 gnlop      (502) staff       (20)     1807 2024-02-15 10:12:57.000000 xtbf-0.1.3/smal/example_datasets.py
+-rw-r--r--   0 gnlop      (502) staff       (20)     1359 2024-05-22 07:34:08.000000 xtbf-0.1.3/smal/fingerprint.py
+-rw-r--r--   0 gnlop      (502) staff       (20)     9809 2024-02-15 11:12:29.000000 xtbf-0.1.3/smal/io.py
+-rw-r--r--   0 gnlop      (502) staff       (20)     9250 2024-05-31 07:29:07.000000 xtbf-0.1.3/smal/mol_edit.py
+-rw-r--r--   0 gnlop      (502) staff       (20)    10537 2024-02-15 11:29:30.000000 xtbf-0.1.3/smal/mol_standardizer.py
+-rw-r--r--   0 gnlop      (502) staff       (20)     5915 2024-02-16 08:52:53.000000 xtbf-0.1.3/smal/viz.py
+drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-05-31 07:39:16.892393 xtbf-0.1.3/xtbf/
+-rw-r--r--   0 gnlop      (502) staff       (20)    12749 2024-05-21 07:58:22.000000 xtbf-0.1.3/xtbf/__init__.py
+-rw-r--r--   0 gnlop      (502) staff       (20)    13904 2024-02-10 14:18:18.000000 xtbf-0.1.3/xtbf/dc_featurizer.py
+-rw-r--r--   0 gnlop      (502) staff       (20)     3748 2024-02-10 14:40:13.000000 xtbf-0.1.3/xtbf/parsers.py
+-rw-r--r--   0 gnlop      (502) staff       (20)    10169 2024-02-14 09:12:13.000000 xtbf-0.1.3/xtbf/shortcuts.py
+drwxr-xr-x   0 gnlop      (502) staff       (20)        0 2024-05-31 07:39:16.894796 xtbf-0.1.3/xtbf.egg-info/
+-rw-r--r--   0 gnlop      (502) staff       (20)      531 2024-05-31 07:39:16.000000 xtbf-0.1.3/xtbf.egg-info/PKG-INFO
+-rw-r--r--   0 gnlop      (502) staff       (20)      760 2024-05-31 07:39:16.000000 xtbf-0.1.3/xtbf.egg-info/SOURCES.txt
+-rw-r--r--   0 gnlop      (502) staff       (20)        1 2024-05-31 07:39:16.000000 xtbf-0.1.3/xtbf.egg-info/dependency_links.txt
+-rw-r--r--   0 gnlop      (502) staff       (20)       25 2024-05-31 07:39:16.000000 xtbf-0.1.3/xtbf.egg-info/requires.txt
+-rw-r--r--   0 gnlop      (502) staff       (20)       10 2024-05-31 07:39:16.000000 xtbf-0.1.3/xtbf.egg-info/top_level.txt
```

### Comparing `xtbf-0.1.2/CONTRIBUTING.md` & `xtbf-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/LICENSE` & `xtbf-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/Makefile` & `xtbf-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/README.md` & `xtbf-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -88,14 +88,34 @@
     H <> 0.036
     H <> 0.284
 
 ```
 
 
 # Getting Started
+Installation is possible via pip
+```bash
+pip install xtbf
+```
+
+To run XTB-related functionality, XTB needs to be installed from:
+```
+https://github.com/grimme-lab/xtb/releases
+```
+or alternatively via conda:
+```
+conda install -c conda-forge xtb
+```
+(see here: https://anaconda.org/conda-forge/xtb)
+
+To run the iupac-to-smiles conversion, opsin needs to be installed:
+```bash
+conda install bioconda::opsin
+```
+
 
 ## Dependencies
 You need to have the following minimal dependencies:
 ```
 joblib, tqdm, numpy, pandas
 ```
 aka:
@@ -106,23 +126,14 @@
 	pip install pandas 
 ```
 alternatively, run from make:
 ```
 make install-deps
 ```
 
-Furthermore, XTB needs to be installed from:
-```
-https://github.com/grimme-lab/xtb/releases
-```
-or alternatively via conda:
-```
-conda install -c conda-forge xtb
-```
-(see here: https://anaconda.org/conda-forge/xtb)
 
 For documentation gen, pdoc needs to be installed:
 ```
 pip install pdoc
 ```
 
 # Running Tests
```

### Comparing `xtbf-0.1.2/data/examples/HIV.csv` & `xtbf-0.1.3/data/examples/HIV.csv`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/data/examples/Lipophilicity.csv` & `xtbf-0.1.3/data/examples/Lipophilicity.csv`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/data/examples/SAMPL.csv` & `xtbf-0.1.3/data/examples/SAMPL.csv`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/data/examples/delaney-processed.csv` & `xtbf-0.1.3/data/examples/delaney-processed.csv`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/doc/log_p_parity_plot.png` & `xtbf-0.1.3/doc/log_p_parity_plot.png`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/doc/search.js` & `xtbf-0.1.3/doc/search.js`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/doc/xtbf/parsers.html` & `xtbf-0.1.3/doc/xtbf/parsers.html`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/doc/xtbf/shortcuts.html` & `xtbf-0.1.3/doc/xtbf/shortcuts.html`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/doc/xtbf.html` & `xtbf-0.1.3/doc/xtbf.html`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/setup.py` & `xtbf-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='xtbf',
-    version='0.1.2',    
+    version='0.1.3',    
     description='A minimal, functional interface to the semiempirical extended tight-binding (xtb) program',
     url='https://github.com/Bayer-Group/xtbf',
     author='Jan Wollschläger',
     author_email='janmwoll@gmail.com',
     license='BSD 3-clause',
     packages=find_packages(),
     setup_requires=['setuptools_scm'],
@@ -15,8 +15,8 @@
         'joblib', 'tqdm','numpy', 'pandas',
     ],
     classifiers=[
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',  
         'Programming Language :: Python :: 3',
     ],
-)
+)
```

### Comparing `xtbf-0.1.2/smal/__init__.py` & `xtbf-0.1.3/smal/__init__.py`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/smal/all.py` & `xtbf-0.1.3/smal/all.py`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/smal/cluster.py` & `xtbf-0.1.3/smal/cluster.py`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/smal/example_datasets.py` & `xtbf-0.1.3/smal/example_datasets.py`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/smal/fingerprint.py` & `xtbf-0.1.3/smal/fingerprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,7 +52,8 @@
     return _fingerprint_to_numpy(fp)
 
 
 def ecfp_bin_fingerprint(mol: Chem.Mol) -> np.ndarray:
     """ """
     fpgen = AllChem.GetRDKitFPGenerator()
     return fpgen.GetFingerprintAsNumPy(mol)
+
```

### Comparing `xtbf-0.1.2/smal/io.py` & `xtbf-0.1.3/smal/io.py`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/smal/mol_edit.py` & `xtbf-0.1.3/smal/mol_edit.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,19 @@
     ...     print(to_smi(remove_atom_at_index(m,i)))
     CCCl
     CCl.F
     CF.Cl
     CCF
     """
     mol = copy.deepcopy(mol)
-    mol.GetAtomWithIdx(atm_idx).SetAtomicNum(0)
+    if isinstance(atm_idx,list) or isinstance(atm_idx,tuple):
+        for ai in atm_idx:
+            mol.GetAtomWithIdx(ai).SetAtomicNum(0)
+    else:
+        mol.GetAtomWithIdx(atm_idx).SetAtomicNum(0)
     mol = Chem.DeleteSubstructs(mol, Chem.MolFromSmarts("[#0]"))
     return mol
 
 
 def single_non_ring_bonds(mol: Chem.Mol) -> list:
     """
     >>> m = from_smi('C1CCCCC1CCC=CC')
@@ -85,15 +89,15 @@
     """
     Embeds the given molecule in 3D and returns the
     resulting molecule with 3D coordinates and the
     corresponding xyz string.
 
     >>> mol = from_smi('CCCO')
     >>> mol, xyz = mol_to_xyzstring(mol)
-    >>> print(xyz)
+    >>> print(xyz) #doctest:+SKIP
     12
     <BLANKLINE>
     C     -1.285327   -0.056776    0.434662
     C     -0.175447    0.695786   -0.299881
     C      0.918409   -0.342619   -0.555572
     O      1.309356   -0.801512    0.717050
     H     -1.923389    0.626223    0.994971
@@ -245,16 +249,16 @@
         atm = mol.GetAtomWithIdx(atm_idx)
         symb = atm.GetSymbol()
         if symb.lower() in ["h", "o", "cl", "br", "i"]:
             continue  # can't hydroxylate those elements
         else:
             # This atom could (potentially) by hydroxylated
             for bnd in atm.GetBonds():
-                if round(bnd.GetBondTypeAsDouble()) != 2:
-                    continue  # only break double bonds...
+                if round(bnd.GetBondTypeAsDouble()) not in [2,3]:
+                    continue  # only break double/triple bonds...
 
                 [other_idx] = list(
                     {bnd.GetBeginAtomIdx(), bnd.GetEndAtomIdx()} - {atm_idx}
                 )
                 other_symb = mol.GetAtomWithIdx(other_idx).GetSymbol()
                 if other_symb.lower() in ["c"]:
                     continue  # not valid "leaving groups"
```

### Comparing `xtbf-0.1.2/smal/mol_standardizer.py` & `xtbf-0.1.3/smal/mol_standardizer.py`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/smal/viz.py` & `xtbf-0.1.3/smal/viz.py`

 * *Files 26% similar despite different names*

```diff
@@ -26,14 +26,52 @@
 # from .helper import *
 
 # from .config import ConfigDict, SecretDict
 
 import math
 import random
 from typing import List
+from rdkit import Chem
+from rdkit.Chem.Draw import rdMolDraw2D
+import io
+from PIL import Image
+from collections import defaultdict
+
+def highlight_mol(mol,atom_colors:list=None,atom_radii:list=None,bond_colors:list=None,width=350,height=400) -> str:
+
+    if atom_radii is None:
+        atom_radii = [0.3 for _ in mol.GetAtoms()]
+    if atom_colors is None:
+        atom_colors = [(0.,0.,0.,0.) for _ in mol.GetAtoms()]
+    if bond_colors is None:
+        bond_colors = [(0.,0.,0.,0.) for _ in mol.GetBonds()]
+
+    assert len(atom_colors) == mol.GetNumAtoms()
+    assert len(bond_colors) == mol.GetNumBonds()
+    assert all(len(col) == 4 for col in atom_colors+bond_colors)
+
+    athighlights = defaultdict(list)
+    arads = {}
+    for a in mol.GetAtoms():
+        aid = a.GetIdx()
+        athighlights[aid].append(atom_colors[aid])
+        arads[aid] = atom_radii[aid]
+
+    bndhighlights = defaultdict(list)
+    for bond in mol.GetBonds():
+        aid1 = bond.GetBeginAtomIdx()
+        aid2 = bond.GetEndAtomIdx()
+        bid = mol.GetBondBetweenAtoms(aid1,aid2).GetIdx()
+        bndhighlights[bid].append(bond_colors[bid])
+
+    d2d = rdMolDraw2D.MolDraw2DCairo(width,height)
+    d2d.DrawMoleculeWithHighlights(mol,"",dict(athighlights),dict(bndhighlights),arads,{})
+    d2d.FinishDrawing()
+    bio = io.BytesIO(d2d.GetDrawingText())
+    return Image.open(bio)
 
 
 def mol_to_svg(mol, save_as=None, width=300, height=300) -> Path:
     fle = random_fle("svg")
     fle.touch()
     Draw.MolToFile(
         mol=mol,
```

### Comparing `xtbf-0.1.2/xtbf/__init__.py` & `xtbf-0.1.3/xtbf/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -104,16 +104,15 @@
 if not TMP_ROOT.exists():
     TMP_ROOT = tempfile.gettempdir()
 
 XTB_TMP_DIR = TMP_ROOT / Path("xtbf")
 
 XTB_OUTER_JOBS = min(32,multiprocessing.cpu_count()-1)
 XTB_INNER_JOBS = 1
-XTB_TIMEOUT_SECONDS = 1200 # 20 minutes
-
+XTB_TIMEOUT_SECONDS = int(os.environ.get("XTBF_TIMEOUT",1200)) # 20 minutes
 
 
 def temp_dir():
     """
     Creates a path to a temporary directory
     """
     if Path("/tmp").exists(): # nosec
@@ -210,15 +209,18 @@
     fle = _obj_id_to_fle(obj_id,cache)
     try:
         return joblib.load(fle)
     except:
         return None
 
 def _obj_id_to_fle(obj_id:str, cache:Path,) -> Path:
-    obj_hash = hashlib.sha1(obj_id.encode("utf-8"), usedforsecurity=False,).hexdigest()
+    try:
+        obj_hash = hashlib.sha1(obj_id.encode("utf-8"), usedforsecurity=False,).hexdigest()
+    except:
+        obj_hash = hashlib.sha1(obj_id.encode("utf-8"),).hexdigest()
     sub_dir_0 = obj_hash[0:3]
     sub_dir_1 = obj_hash[3:6]
     obj_fle = cache / sub_dir_0 / sub_dir_1 / obj_hash
     obj_fle = obj_fle.with_suffix(".pkl")
     return obj_fle
 
 def run_parallel(
@@ -282,15 +284,15 @@
             min_conf_id = conf.GetId()
     if min_conf_id is None:
         raise ValueError("no conformer (with energy) found")
 
     return min_conf_id
 
 
-def run_xtb(xtb_command:str, mol:Chem.Mol, multiplicity:int, conf_id:int="lowest", cache=None,):
+def run_xtb(xtb_command:str, mol:Chem.Mol, multiplicity:int, conf_id:int="lowest", cache=None, store_failures=True, charge:int=0,):
     """
 
     >>> mol = Chem.MolFromSmiles("CCCOCCC")
     >>> mol = embed_molecule(mol)
     >>> success,rslt = run_xtb("--opt", mol, 1)
     >>> success
     True
@@ -338,23 +340,32 @@
         mol, xyz_string = mol_to_xyzstring(mol,conf_id=conf_id)
         return run_xtb_xyz(xtb_command=xtb_command,xyz_string=xyz_string, multiplicity=multiplicity, )
     else:
         stored_result = cache_load(obj_id=obj_id,cache=cache)
         if stored_result is not None:
             return stored_result
         else:
+            if str(os.environ.get("XTBF_SKIP_CALCS", None)) in ("1","t","T","True","true"):
+                return None
+            
             if conf_id == "lowest":
                 mol = embed_multi_keep_lowest(mol,100)
                 conf_id = _determine_min_conf_id(mol)
             mol, xyz_string = mol_to_xyzstring(mol,conf_id=conf_id)
-            rslt = run_xtb_xyz(xtb_command=xtb_command,xyz_string=xyz_string, multiplicity=multiplicity, )
+            try:
+                rslt = run_xtb_xyz(xtb_command=xtb_command,xyz_string=xyz_string, multiplicity=multiplicity, charge=charge, )
+            except:
+                if store_failures:
+                    rslt = None
+                else:
+                    raise
             cache_store(rslt,obj_id=obj_id,cache=cache)
             return rslt
 
-def run_xtb_xyz(xtb_command:str, xyz_string:str, multiplicity:int, ):
+def run_xtb_xyz(xtb_command:str, xyz_string:str, multiplicity:int, charge:int=0,):
     """
     Runs the given xtb job as identified by
     the following components:
      - The command <xtb>, 
      - the xyz string of the molecule <xyz_string>
 
     """
@@ -365,23 +376,27 @@
     assert not job_dir.exists(), "internal logic error"
     cwd_before = os.getcwd()
 
     if multiplicity != 1:
         uhf_arg = f"--uhf {multiplicity} "
     else:
         uhf_arg = ""
+    if charge != 0:
+        chrg_arg = f"--chrg {charge} "
+    else:
+        chrg_arg = ""
     try:
         os.mkdir(job_dir)
         os.chdir(job_dir)
         (job_dir / "input.xyz").write_text(xyz_string)
         output_fle = job_dir / "output.out"
         assert not output_fle.exists()
         with Silencer() as s:
             # alpb_str = ""
-            cmd = f"{BIN_XTB} input.xyz --parallel {XTB_INNER_JOBS} {xtb_command} {uhf_arg}> output.out 2> err.out"
+            cmd = f"{BIN_XTB} input.xyz --parallel {XTB_INNER_JOBS} {xtb_command} {uhf_arg} {chrg_arg}> output.out 2> err.out"
 
             # normal approach:
             # subprocess.check_output(cmd,shell=True,timeout=XTB_TIMEOUT_SECONDS)
             # ^
             # \__ sadly, this approach does not work because the timeout isnt applied
             #
             # As suggested in https://stackoverflow.com/questions/48763362/python-subprocess-kill-with-timeout
```

### Comparing `xtbf-0.1.2/xtbf/dc_featurizer.py` & `xtbf-0.1.3/xtbf/dc_featurizer.py`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/xtbf/parsers.py` & `xtbf-0.1.3/xtbf/parsers.py`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/xtbf/shortcuts.py` & `xtbf-0.1.3/xtbf/shortcuts.py`

 * *Files identical despite different names*

### Comparing `xtbf-0.1.2/xtbf.egg-info/SOURCES.txt` & `xtbf-0.1.3/xtbf.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 doc/xtbf.html
 doc/xtbf/parsers.html
 doc/xtbf/shortcuts.html
 smal/__init__.py
 smal/all.py
 smal/cluster.py
 smal/config.py
+smal/descriptors.py
 smal/example_datasets.py
 smal/fingerprint.py
 smal/io.py
 smal/mol_edit.py
 smal/mol_standardizer.py
 smal/viz.py
 xtbf/__init__.py
```

