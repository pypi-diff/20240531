# Comparing `tmp/socialdataanalysis-0.9.1.tar.gz` & `tmp/socialdataanalysis-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socialdataanalysis-0.9.1.tar", last modified: Fri May 31 14:09:26 2024, max compression
+gzip compressed data, was "socialdataanalysis-0.9.2.tar", last modified: Fri May 31 14:27:09 2024, max compression
```

## Comparing `socialdataanalysis-0.9.1.tar` & `socialdataanalysis-0.9.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:09:26.994492 socialdataanalysis-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 14:09:18.000000 socialdataanalysis-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-31 14:09:26.994492 socialdataanalysis-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-31 14:09:18.000000 socialdataanalysis-0.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:09:26.994492 socialdataanalysis-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-31 14:09:18.000000 socialdataanalysis-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:09:26.994492 socialdataanalysis-0.9.1/socialdataanalysis/
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-31 14:09:18.000000 socialdataanalysis-0.9.1/socialdataanalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63870 2024-05-31 14:09:18.000000 socialdataanalysis-0.9.1/socialdataanalysis/association.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-31 14:09:18.000000 socialdataanalysis-0.9.1/socialdataanalysis/exploratoryfactoranalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:09:26.994492 socialdataanalysis-0.9.1/socialdataanalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-31 14:09:26.000000 socialdataanalysis-0.9.1/socialdataanalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-31 14:09:26.000000 socialdataanalysis-0.9.1/socialdataanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:09:26.000000 socialdataanalysis-0.9.1/socialdataanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 14:09:26.000000 socialdataanalysis-0.9.1/socialdataanalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 14:09:26.000000 socialdataanalysis-0.9.1/socialdataanalysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:27:09.529188 socialdataanalysis-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 14:27:00.000000 socialdataanalysis-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-31 14:27:00.000000 socialdataanalysis-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-31 14:27:09.529188 socialdataanalysis-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-31 14:27:00.000000 socialdataanalysis-0.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:27:09.529188 socialdataanalysis-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-31 14:27:00.000000 socialdataanalysis-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:27:09.529188 socialdataanalysis-0.9.2/socialdataanalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-31 14:27:00.000000 socialdataanalysis-0.9.2/socialdataanalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63870 2024-05-31 14:27:00.000000 socialdataanalysis-0.9.2/socialdataanalysis/association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-31 14:27:00.000000 socialdataanalysis-0.9.2/socialdataanalysis/exploratoryfactoranalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:27:09.529188 socialdataanalysis-0.9.2/socialdataanalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-31 14:27:09.000000 socialdataanalysis-0.9.2/socialdataanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-31 14:27:09.000000 socialdataanalysis-0.9.2/socialdataanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:27:09.000000 socialdataanalysis-0.9.2/socialdataanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 14:27:09.000000 socialdataanalysis-0.9.2/socialdataanalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 14:27:09.000000 socialdataanalysis-0.9.2/socialdataanalysis.egg-info/top_level.txt
```

### Comparing `socialdataanalysis-0.9.1/LICENSE` & `socialdataanalysis-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.1/PKG-INFO` & `socialdataanalysis-0.9.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialdataanalysis
-Version: 0.9.1
+Version: 0.9.2
 Summary: Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.
 Home-page: https://github.com/rcmergulhao/socialdataanalysis
 Author: Ricardo Mergulhao
 Author-email: ricardomergulhao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,15 @@
 Requires-Dist: numpy
 Requires-Dist: statsmodels
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: sympy
 Requires-Dist: prince
 Requires-Dist: altair
+Requires-Dist: pyreadstat
 
 # socialdataanalysis
 
 **Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.**
 
 Este pacote oferece uma coleção de funções úteis para análise de dados, especialmente projetadas para complementar as capacidades do SPSS em pesquisas nas ciências sociais. As funções incluídas cobrem diversos aspectos da análise de associação, conforme descrito no livro [Análise de Dados Para Ciências Sociais: A Complementaridade do SPSS](https://silabo.pt/catalogo/informatica/aplicativos-estatisticos/livro/analise-de-dados-para-ciencias-sociais/).
```

### Comparing `socialdataanalysis-0.9.1/README.md` & `socialdataanalysis-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.1/setup.py` & `socialdataanalysis-0.9.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from setuptools import setup, find_packages
 
 setup(
     name='socialdataanalysis',
-    version='0.9.1',
+    version='0.9.2',
     packages=find_packages(),
     include_package_data=True,
     package_data={
         'socialdataanalysis': ['notebooks/*.ipynb'],
     },
     install_requires=[
         'pandas',
         'numpy',
         'statsmodels',
         'scipy',
         'matplotlib',
         'sympy',
         'prince',
-        'altair'
+        'altair',
+        'pyreadstat'
     ],
     author='Ricardo Mergulhao',
     author_email='ricardomergulhao@gmail.com',
     description='Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/rcmergulhao/socialdataanalysis',
```

### Comparing `socialdataanalysis-0.9.1/socialdataanalysis/__init__.py` & `socialdataanalysis-0.9.2/socialdataanalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.1/socialdataanalysis/association.py` & `socialdataanalysis-0.9.2/socialdataanalysis/association.py`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.1/socialdataanalysis/exploratoryfactoranalysis.py` & `socialdataanalysis-0.9.2/socialdataanalysis/exploratoryfactoranalysis.py`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.1/socialdataanalysis.egg-info/PKG-INFO` & `socialdataanalysis-0.9.2/socialdataanalysis.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialdataanalysis
-Version: 0.9.1
+Version: 0.9.2
 Summary: Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.
 Home-page: https://github.com/rcmergulhao/socialdataanalysis
 Author: Ricardo Mergulhao
 Author-email: ricardomergulhao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -15,14 +15,15 @@
 Requires-Dist: numpy
 Requires-Dist: statsmodels
 Requires-Dist: scipy
 Requires-Dist: matplotlib
 Requires-Dist: sympy
 Requires-Dist: prince
 Requires-Dist: altair
+Requires-Dist: pyreadstat
 
 # socialdataanalysis
 
 **Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.**
 
 Este pacote oferece uma coleção de funções úteis para análise de dados, especialmente projetadas para complementar as capacidades do SPSS em pesquisas nas ciências sociais. As funções incluídas cobrem diversos aspectos da análise de associação, conforme descrito no livro [Análise de Dados Para Ciências Sociais: A Complementaridade do SPSS](https://silabo.pt/catalogo/informatica/aplicativos-estatisticos/livro/analise-de-dados-para-ciencias-sociais/).
```

