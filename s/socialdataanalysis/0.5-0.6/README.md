# Comparing `tmp/socialdataanalysis-0.5.tar.gz` & `tmp/socialdataanalysis-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socialdataanalysis-0.5.tar", last modified: Fri May 31 12:33:44 2024, max compression
+gzip compressed data, was "socialdataanalysis-0.6.tar", last modified: Fri May 31 13:19:23 2024, max compression
```

## Comparing `socialdataanalysis-0.5.tar` & `socialdataanalysis-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:33:44.782843 socialdataanalysis-0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 12:33:36.000000 socialdataanalysis-0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-31 12:33:44.782843 socialdataanalysis-0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-31 12:33:36.000000 socialdataanalysis-0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 12:33:44.782843 socialdataanalysis-0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-31 12:33:36.000000 socialdataanalysis-0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:33:44.778843 socialdataanalysis-0.5/socialdataanalysis/
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-31 12:33:36.000000 socialdataanalysis-0.5/socialdataanalysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    63870 2024-05-31 12:33:36.000000 socialdataanalysis-0.5/socialdataanalysis/association.py
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-31 12:33:36.000000 socialdataanalysis-0.5/socialdataanalysis/exploratoryfactoranalysis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 12:33:44.782843 socialdataanalysis-0.5/socialdataanalysis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-31 12:33:44.000000 socialdataanalysis-0.5/socialdataanalysis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-31 12:33:44.000000 socialdataanalysis-0.5/socialdataanalysis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 12:33:44.000000 socialdataanalysis-0.5/socialdataanalysis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 12:33:44.000000 socialdataanalysis-0.5/socialdataanalysis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 12:33:44.000000 socialdataanalysis-0.5/socialdataanalysis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:19:23.869259 socialdataanalysis-0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 13:19:13.000000 socialdataanalysis-0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-31 13:19:23.869259 socialdataanalysis-0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-31 13:19:13.000000 socialdataanalysis-0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 13:19:23.869259 socialdataanalysis-0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-31 13:19:13.000000 socialdataanalysis-0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:19:23.869259 socialdataanalysis-0.6/socialdataanalysis/
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-31 13:19:13.000000 socialdataanalysis-0.6/socialdataanalysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63870 2024-05-31 13:19:13.000000 socialdataanalysis-0.6/socialdataanalysis/association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-05-31 13:19:13.000000 socialdataanalysis-0.6/socialdataanalysis/exploratoryfactoranalysis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 13:19:23.869259 socialdataanalysis-0.6/socialdataanalysis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-31 13:19:23.000000 socialdataanalysis-0.6/socialdataanalysis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-31 13:19:23.000000 socialdataanalysis-0.6/socialdataanalysis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 13:19:23.000000 socialdataanalysis-0.6/socialdataanalysis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 13:19:23.000000 socialdataanalysis-0.6/socialdataanalysis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 13:19:23.000000 socialdataanalysis-0.6/socialdataanalysis.egg-info/top_level.txt
```

### Comparing `socialdataanalysis-0.5/LICENSE` & `socialdataanalysis-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.5/README.md` & `socialdataanalysis-0.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 # socialdataanalysis
 
 **Funções personalizadas para análise de dados nas ciências sociais, complementando o uso do SPSS.**
 
 Este pacote oferece uma coleção de funções úteis para análise de dados, especialmente projetadas para complementar as capacidades do SPSS em pesquisas nas ciências sociais. As funções incluídas cobrem diversos aspectos da análise de associação, conforme descrito no livro [Análise de Dados Para Ciências Sociais: A Complementaridade do SPSS](https://silabo.pt/catalogo/informatica/aplicativos-estatisticos/livro/analise-de-dados-para-ciencias-sociais/).
 
-## Instalação
+## Features
+
+- Association Analysis
+- Exploratory Factor Analysis
+
+## Installation
 
 Você pode instalar o pacote diretamente do PyPI usando pip:
 
 ```bash
 pip install socialdataanalysis
```

### Comparing `socialdataanalysis-0.5/socialdataanalysis/__init__.py` & `socialdataanalysis-0.6/socialdataanalysis/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,33 @@
+'''
 from .association import (
     criar_mapeamento_categorias,
     analisar_independencia_variaveis_tabela_contingencia,
     calcular_odds_ratio_razao_risco_discrepancia,
     calcular_distribuicao_probabilidades_e_decisao_hipotese,
     complementar_tabela_contingencia_com_analise_estatistica,
     resolver_sistema_equacoes_dada_variavel_tabela_contingencia,
     decompor_tabela_contingencia,
-    encontrar_maiores_valores,
-    criar_subtabela,
     gerar_tabela_contingencia,
     complementar_e_filtrar_tabelas_contingencia,
     avaliar_homogeneidade_odds_ratio,
     avaliar_independencia_condicional,
     avaliar_associacao_condicional,
     analisar_frequencias_esperadas,
-    gerar_interacoes,
-    eliminacao_reversa,
-    gerar_todas_as_interacoes_possiveis,
     eliminacao_reversa_com_comparacao_llm,
     calcular_e_exibir_odds_ratios_llm,
     criar_tabela_contingencia_expandida_llm,
     plot_stacked_bar_chart,
     realizar_analise_correspondencia,
     detalhar_resultados_analise_correspondencia,
-    analise_correspondencia_e_grafico
+    analise_correspondencia_e_grafico,
 )
 from .exploratoryfactoranalysis import (
     inverter_escala,
     transformar_escala,
-    analisar_consistencia_interna
-)
+    analisar_consistencia_interna,
+)
+'''
+from .association import Association
+from .exploratoryfactoranalysis import ExploratoryFactorAnalysis
+
+__all__ = ['Association', 'ExploratoryFactorAnalysis']
```

### Comparing `socialdataanalysis-0.5/socialdataanalysis/association.py` & `socialdataanalysis-0.6/socialdataanalysis/association.py`

 * *Files identical despite different names*

### Comparing `socialdataanalysis-0.5/socialdataanalysis/exploratoryfactoranalysis.py` & `socialdataanalysis-0.6/socialdataanalysis/exploratoryfactoranalysis.py`

 * *Files identical despite different names*

