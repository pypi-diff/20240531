# Comparing `tmp/socialdataanalysis-0.9.6.tar.gz` & `tmp/socialdataanalysis-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socialdataanalysis-0.9.6.tar", last modified: Fri May 31 15:08:00 2024, max compression
+gzip compressed data, was "socialdataanalysis-0.9.7.tar", last modified: Fri May 31 15:18:52 2024, max compression
```

## Comparing `socialdataanalysis-0.9.6.tar` & `socialdataanalysis-0.9.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:08:00.907131 socialdataanalysis-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-31 15:08:00.907131 socialdataanalysis-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:08:00.907131 socialdataanalysis-0.9.6/nb_exercices/
--rw-r--r--   0 runner    (1001) docker     (127)    64456 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex10_Universidades&Tempo_estudo_exame.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    31973 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex11_Medicacao&Sexo Continente.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    36381 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex12_Bronquite&Exposicao Idade.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    44282 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex13_Autonomia&Satisfacao_por_Religiao.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    40329 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex14_Hemisferio&Tumor_por_Sitio.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    50480 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex15_Cinto&Ferimentos_por_Localizacao_e_Sexo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   145918 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex16 SCA_Imagem_Pão Zona.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   175776 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex17 SCA_Prémio_Nobel_Países_Anos.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    57612 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex1_Aborto.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    47432 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex2_Rua&HIV.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    42883 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex3_Bebidas&Feridos.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    29859 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex4_Sexo&Comportamento.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    85397 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex5_Sexo&Compra.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    19798 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex6_Qualidade_de_um_Teste.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex7_Qualidade_entre_dois_Testes.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    21671 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex8_Desempenho_modelo_classificacao_pecas.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    70511 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex9_Votos&Atitudes.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    57016 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/nb_exercices/Cap4_Ex1_Uniformização_de_escalas.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:08:00.907131 socialdataanalysis-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:08:00.907131 socialdataanalysis-0.9.6/socialdataanalysis/
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/socialdataanalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63870 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/socialdataanalysis/association.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-31 15:07:44.000000 socialdataanalysis-0.9.6/socialdataanalysis/exploratoryfactoranalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:08:00.907131 socialdataanalysis-0.9.6/socialdataanalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-31 15:08:00.000000 socialdataanalysis-0.9.6/socialdataanalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-31 15:08:00.000000 socialdataanalysis-0.9.6/socialdataanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:08:00.000000 socialdataanalysis-0.9.6/socialdataanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 15:08:00.000000 socialdataanalysis-0.9.6/socialdataanalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 15:08:00.000000 socialdataanalysis-0.9.6/socialdataanalysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:18:52.630343 socialdataanalysis-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-31 15:18:52.630343 socialdataanalysis-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:18:52.626343 socialdataanalysis-0.9.7/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (127)    64456 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex10_Universidades&Tempo_estudo_exame.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    31973 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex11_Medicacao&Sexo Continente.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    36381 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex12_Bronquite&Exposicao Idade.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    44282 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex13_Autonomia&Satisfacao_por_Religiao.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    40329 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex14_Hemisferio&Tumor_por_Sitio.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    50480 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex15_Cinto&Ferimentos_por_Localizacao_e_Sexo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   145918 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex16 SCA_Imagem_Pão Zona.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   175776 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex17 SCA_Prémio_Nobel_Países_Anos.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    57612 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex1_Aborto.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    47432 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex2_Rua&HIV.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    42883 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex3_Bebidas&Feridos.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    29859 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex4_Sexo&Comportamento.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    85397 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex5_Sexo&Compra.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    19798 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex6_Qualidade_de_um_Teste.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex7_Qualidade_entre_dois_Testes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    21671 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex8_Desempenho_modelo_classificacao_pecas.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    70511 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap2_Ex9_Votos&Atitudes.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    57016 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/notebooks/Cap4_Ex1_Uniformização_de_escalas.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:18:52.630343 socialdataanalysis-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:18:52.626343 socialdataanalysis-0.9.7/socialdataanalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/socialdataanalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63870 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/socialdataanalysis/association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-31 15:18:41.000000 socialdataanalysis-0.9.7/socialdataanalysis/exploratoryfactoranalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:18:52.630343 socialdataanalysis-0.9.7/socialdataanalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-31 15:18:52.000000 socialdataanalysis-0.9.7/socialdataanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-31 15:18:52.000000 socialdataanalysis-0.9.7/socialdataanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:18:52.000000 socialdataanalysis-0.9.7/socialdataanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 15:18:52.000000 socialdataanalysis-0.9.7/socialdataanalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 15:18:52.000000 socialdataanalysis-0.9.7/socialdataanalysis.egg-info/top_level.txt
```

### Comparing `socialdataanalysis-0.9.6/LICENSE` & `socialdataanalysis-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/PKG-INFO` & `socialdataanalysis-0.9.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialdataanalysis
-Version: 0.9.6
+Version: 0.9.7
 Summary: Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.
 Home-page: https://github.com/rcmergulhao/socialdataanalysis
 Author: Ricardo Mergulhao
 Author-email: ricardomergulhao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `socialdataanalysis-0.9.6/README.md` & `socialdataanalysis-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex10_Universidades&Tempo_estudo_exame.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex10_Universidades&Tempo_estudo_exame.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex11_Medicacao&Sexo Continente.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex11_Medicacao&Sexo Continente.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex12_Bronquite&Exposicao Idade.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex12_Bronquite&Exposicao Idade.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex13_Autonomia&Satisfacao_por_Religiao.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex13_Autonomia&Satisfacao_por_Religiao.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex14_Hemisferio&Tumor_por_Sitio.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex14_Hemisferio&Tumor_por_Sitio.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex15_Cinto&Ferimentos_por_Localizacao_e_Sexo.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex15_Cinto&Ferimentos_por_Localizacao_e_Sexo.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex16 SCA_Imagem_Pão Zona.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex16 SCA_Imagem_Pão Zona.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex17 SCA_Prémio_Nobel_Países_Anos.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex17 SCA_Prémio_Nobel_Países_Anos.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex1_Aborto.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex1_Aborto.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex2_Rua&HIV.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex2_Rua&HIV.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex3_Bebidas&Feridos.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex3_Bebidas&Feridos.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex4_Sexo&Comportamento.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex4_Sexo&Comportamento.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex5_Sexo&Compra.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex5_Sexo&Compra.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex6_Qualidade_de_um_Teste.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex6_Qualidade_de_um_Teste.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex7_Qualidade_entre_dois_Testes.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex7_Qualidade_entre_dois_Testes.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex8_Desempenho_modelo_classificacao_pecas.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex8_Desempenho_modelo_classificacao_pecas.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap2_Ex9_Votos&Atitudes.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap2_Ex9_Votos&Atitudes.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/nb_exercices/Cap4_Ex1_Uniformização_de_escalas.ipynb` & `socialdataanalysis-0.9.7/notebooks/Cap4_Ex1_Uniformização_de_escalas.ipynb`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/setup.py` & `socialdataanalysis-0.9.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='socialdataanalysis',
-    version='0.9.6',
+    version='0.9.7',
     packages=find_packages(),
     include_package_data=True,
     package_data={
-        'socialdataanalysis': ['nb_exercices/*.ipynb'],
+        'socialdataanalysis': ['notebooks/*.ipynb'],
     },
+    data_files=[
+        ('notebooks', ['notebooks/Cap2_Ex1_Aborto.ipynb', ]),
+    ],
     install_requires=[
         'pandas',
         'numpy',
         'statsmodels',
         'scipy',
         'matplotlib',
         'sympy',
```

### Comparing `socialdataanalysis-0.9.6/socialdataanalysis/__init__.py` & `socialdataanalysis-0.9.7/socialdataanalysis/__init__.py`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/socialdataanalysis/association.py` & `socialdataanalysis-0.9.7/socialdataanalysis/association.py`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/socialdataanalysis/exploratoryfactoranalysis.py` & `socialdataanalysis-0.9.7/socialdataanalysis/exploratoryfactoranalysis.py`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.9.6/socialdataanalysis.egg-info/PKG-INFO` & `socialdataanalysis-0.9.7/socialdataanalysis.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socialdataanalysis
-Version: 0.9.6
+Version: 0.9.7
 Summary: Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.
 Home-page: https://github.com/rcmergulhao/socialdataanalysis
 Author: Ricardo Mergulhao
 Author-email: ricardomergulhao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```
