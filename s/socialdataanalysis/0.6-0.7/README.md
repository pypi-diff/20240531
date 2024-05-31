# Comparing `tmp/socialdataanalysis-0.6.tar.gz` & `tmp/socialdataanalysis-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socialdataanalysis-0.6.tar", last modified: Fri May 31 13:19:23 2024, max compression
+gzip compressed data, was "socialdataanalysis-0.7.tar", last modified: Fri May 31 13:34:55 2024, max compression
```

## Comparing `socialdataanalysis-0.6.tar` & `socialdataanalysis-0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:19:23.869259 socialdataanalysis-0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 13:19:13.000000 socialdataanalysis-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-31 13:19:23.869259 socialdataanalysis-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-31 13:19:13.000000 socialdataanalysis-0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:19:23.869259 socialdataanalysis-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-31 13:19:13.000000 socialdataanalysis-0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:19:23.869259 socialdataanalysis-0.6/socialdataanalysis/
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-31 13:19:13.000000 socialdataanalysis-0.6/socialdataanalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63870 2024-05-31 13:19:13.000000 socialdataanalysis-0.6/socialdataanalysis/association.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-31 13:19:13.000000 socialdataanalysis-0.6/socialdataanalysis/exploratoryfactoranalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:19:23.869259 socialdataanalysis-0.6/socialdataanalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-31 13:19:23.000000 socialdataanalysis-0.6/socialdataanalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-31 13:19:23.000000 socialdataanalysis-0.6/socialdataanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:19:23.000000 socialdataanalysis-0.6/socialdataanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 13:19:23.000000 socialdataanalysis-0.6/socialdataanalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 13:19:23.000000 socialdataanalysis-0.6/socialdataanalysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:34:55.125286 socialdataanalysis-0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 13:34:47.000000 socialdataanalysis-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-31 13:34:55.125286 socialdataanalysis-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-31 13:34:47.000000 socialdataanalysis-0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:34:55.125286 socialdataanalysis-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-31 13:34:47.000000 socialdataanalysis-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:34:55.125286 socialdataanalysis-0.7/socialdataanalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-31 13:34:47.000000 socialdataanalysis-0.7/socialdataanalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63870 2024-05-31 13:34:47.000000 socialdataanalysis-0.7/socialdataanalysis/association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-31 13:34:47.000000 socialdataanalysis-0.7/socialdataanalysis/exploratoryfactoranalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:34:55.125286 socialdataanalysis-0.7/socialdataanalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-31 13:34:55.000000 socialdataanalysis-0.7/socialdataanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-31 13:34:55.000000 socialdataanalysis-0.7/socialdataanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:34:55.000000 socialdataanalysis-0.7/socialdataanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 13:34:55.000000 socialdataanalysis-0.7/socialdataanalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 13:34:55.000000 socialdataanalysis-0.7/socialdataanalysis.egg-info/top_level.txt
```

### Comparing `socialdataanalysis-0.6/LICENSE` & `socialdataanalysis-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.6/PKG-INFO` & `socialdataanalysis-0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialdataanalysis
-Version: 0.6
+Version: 0.7
 Summary: Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.
 Home-page: https://github.com/rcmergulhao/socialdataanalysis
 Author: Ricardo Mergulhao
 Author-email: ricardomergulhao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `socialdataanalysis-0.6/README.md` & `socialdataanalysis-0.7/README.md`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.6/setup.py` & `socialdataanalysis-0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='socialdataanalysis',
-    version='0.6',
+    version='0.7',
     packages=find_packages(),
     include_package_data=True,
     package_data={
         'socialdataanalysis': ['notebooks/*.ipynb'],
     },
     install_requires=[
         'pandas',
```

### Comparing `socialdataanalysis-0.6/socialdataanalysis/__init__.py` & `socialdataanalysis-0.7/socialdataanalysis/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-'''
 from .association import (
     criar_mapeamento_categorias,
     analisar_independencia_variaveis_tabela_contingencia,
     calcular_odds_ratio_razao_risco_discrepancia,
     calcular_distribuicao_probabilidades_e_decisao_hipotese,
     complementar_tabela_contingencia_com_analise_estatistica,
     resolver_sistema_equacoes_dada_variavel_tabela_contingencia,
@@ -21,13 +20,8 @@
     detalhar_resultados_analise_correspondencia,
     analise_correspondencia_e_grafico,
 )
 from .exploratoryfactoranalysis import (
     inverter_escala,
     transformar_escala,
     analisar_consistencia_interna,
-)
-'''
-from .association import Association
-from .exploratoryfactoranalysis import ExploratoryFactorAnalysis
-
-__all__ = ['Association', 'ExploratoryFactorAnalysis']
+)
```

### Comparing `socialdataanalysis-0.6/socialdataanalysis/association.py` & `socialdataanalysis-0.7/socialdataanalysis/association.py`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.6/socialdataanalysis/exploratoryfactoranalysis.py` & `socialdataanalysis-0.7/socialdataanalysis/exploratoryfactoranalysis.py`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.6/socialdataanalysis.egg-info/PKG-INFO` & `socialdataanalysis-0.7/socialdataanalysis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialdataanalysis
-Version: 0.6
+Version: 0.7
 Summary: Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.
 Home-page: https://github.com/rcmergulhao/socialdataanalysis
 Author: Ricardo Mergulhao
 Author-email: ricardomergulhao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

