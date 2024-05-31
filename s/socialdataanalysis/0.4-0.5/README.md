# Comparing `tmp/socialdataanalysis-0.4.tar.gz` & `tmp/socialdataanalysis-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socialdataanalysis-0.4.tar", last modified: Sat May 25 23:59:50 2024, max compression
+gzip compressed data, was "socialdataanalysis-0.5.tar", last modified: Fri May 31 12:33:44 2024, max compression
```

## Comparing `socialdataanalysis-0.4.tar` & `socialdataanalysis-0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:59:50.674422 socialdataanalysis-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-25 23:59:42.000000 socialdataanalysis-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-25 23:59:50.674422 socialdataanalysis-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-25 23:59:42.000000 socialdataanalysis-0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 23:59:50.674422 socialdataanalysis-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-25 23:59:42.000000 socialdataanalysis-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:59:50.670421 socialdataanalysis-0.4/socialdataanalysis/
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-25 23:59:42.000000 socialdataanalysis-0.4/socialdataanalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63872 2024-05-25 23:59:42.000000 socialdataanalysis-0.4/socialdataanalysis/association.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 23:59:50.670421 socialdataanalysis-0.4/socialdataanalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-25 23:59:50.000000 socialdataanalysis-0.4/socialdataanalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-25 23:59:50.000000 socialdataanalysis-0.4/socialdataanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 23:59:50.000000 socialdataanalysis-0.4/socialdataanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-25 23:59:50.000000 socialdataanalysis-0.4/socialdataanalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-25 23:59:50.000000 socialdataanalysis-0.4/socialdataanalysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:33:44.782843 socialdataanalysis-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 12:33:36.000000 socialdataanalysis-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-31 12:33:44.782843 socialdataanalysis-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-31 12:33:36.000000 socialdataanalysis-0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:33:44.782843 socialdataanalysis-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-31 12:33:36.000000 socialdataanalysis-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:33:44.778843 socialdataanalysis-0.5/socialdataanalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-31 12:33:36.000000 socialdataanalysis-0.5/socialdataanalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63870 2024-05-31 12:33:36.000000 socialdataanalysis-0.5/socialdataanalysis/association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-31 12:33:36.000000 socialdataanalysis-0.5/socialdataanalysis/exploratoryfactoranalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:33:44.782843 socialdataanalysis-0.5/socialdataanalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-31 12:33:44.000000 socialdataanalysis-0.5/socialdataanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-31 12:33:44.000000 socialdataanalysis-0.5/socialdataanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:33:44.000000 socialdataanalysis-0.5/socialdataanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 12:33:44.000000 socialdataanalysis-0.5/socialdataanalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 12:33:44.000000 socialdataanalysis-0.5/socialdataanalysis.egg-info/top_level.txt
```

### Comparing `socialdataanalysis-0.4/LICENSE` & `socialdataanalysis-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.4/PKG-INFO` & `socialdataanalysis-0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialdataanalysis
-Version: 0.4
+Version: 0.5
 Summary: Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.
 Home-page: https://github.com/rcmergulhao/socialdataanalysis
 Author: Ricardo Mergulhao
 Author-email: ricardomergulhao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `socialdataanalysis-0.4/README.md` & `socialdataanalysis-0.5/README.md`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.4/setup.py` & `socialdataanalysis-0.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='socialdataanalysis',
-    version='0.4',
+    version='0.5',
     packages=find_packages(),
+    include_package_data=True,
+    package_data={
+        'socialdataanalysis': ['notebooks/*.ipynb'],
+    },
     install_requires=[
         'pandas',
         'numpy',
         'statsmodels',
         'scipy',
         'matplotlib',
         'sympy',
```

### Comparing `socialdataanalysis-0.4/socialdataanalysis/__init__.py` & `socialdataanalysis-0.5/socialdataanalysis/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,8 +21,12 @@
     calcular_e_exibir_odds_ratios_llm,
     criar_tabela_contingencia_expandida_llm,
     plot_stacked_bar_chart,
     realizar_analise_correspondencia,
     detalhar_resultados_analise_correspondencia,
     analise_correspondencia_e_grafico
 )
-
+from .exploratoryfactoranalysis import (
+    inverter_escala,
+    transformar_escala,
+    analisar_consistencia_interna
+)
```

### Comparing `socialdataanalysis-0.4/socialdataanalysis/association.py` & `socialdataanalysis-0.5/socialdataanalysis/association.py`

 * *Files 0% similar despite different names*

```diff
@@ -1244,8 +1244,7 @@
     ).properties(
         width=720,  # Largura desejada do gráfico em pixels
         height=480  # Altura desejada do gráfico em pixels
     )
 
     # Exibe o gráfico com o novo tamanho
     chart.display()
-
```

### Comparing `socialdataanalysis-0.4/socialdataanalysis.egg-info/PKG-INFO` & `socialdataanalysis-0.5/socialdataanalysis.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialdataanalysis
-Version: 0.4
+Version: 0.5
 Summary: Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.
 Home-page: https://github.com/rcmergulhao/socialdataanalysis
 Author: Ricardo Mergulhao
 Author-email: ricardomergulhao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

