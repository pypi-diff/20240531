# Comparing `tmp/hnt_nf_jira_servicos_library-0.0.2.tar.gz` & `tmp/hnt_nf_jira_servicos_library-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_servicos_library-0.0.2.tar", last modified: Fri May 31 14:54:35 2024, max compression
+gzip compressed data, was "hnt_nf_jira_servicos_library-0.0.3.tar", last modified: Fri May 31 14:55:07 2024, max compression
```

## Comparing `hnt_nf_jira_servicos_library-0.0.2.tar` & `hnt_nf_jira_servicos_library-0.0.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 14:54:35.600521 hnt_nf_jira_servicos_library-0.0.2/
--rw-rw-rw-   0        0        0      267 2024-05-31 14:54:35.600521 hnt_nf_jira_servicos_library-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      713 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 14:54:35.592519 hnt_nf_jira_servicos_library-0.0.2/hnt_nf_jira_servicos_library.egg-info/
--rw-rw-rw-   0        0        0      267 2024-05-31 14:54:35.000000 hnt_nf_jira_servicos_library-0.0.2/hnt_nf_jira_servicos_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-05-31 14:54:35.000000 hnt_nf_jira_servicos_library-0.0.2/hnt_nf_jira_servicos_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 14:54:35.000000 hnt_nf_jira_servicos_library-0.0.2/hnt_nf_jira_servicos_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-31 14:54:35.000000 hnt_nf_jira_servicos_library-0.0.2/hnt_nf_jira_servicos_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-31 14:54:35.000000 hnt_nf_jira_servicos_library-0.0.2/hnt_nf_jira_servicos_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 14:54:35.436823 hnt_nf_jira_servicos_library-0.0.2/nf_jira/
--rw-rw-rw-   0        0        0       41 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 14:54:35.554158 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      211 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/chave_acesso.py
-drwxrwxrwx   0        0        0        0 2024-05-31 14:54:35.584519 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/classes/
--rw-rw-rw-   0        0        0     4245 2024-05-31 13:26:08.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/classes/factories.py
--rw-rw-rw-   0        0        0     4997 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/classes/form_jira.py
--rw-rw-rw-   0        0        0    13316 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/classes/helper.py
--rw-rw-rw-   0        0        0     1947 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/classes/issue_fields.py
--rw-rw-rw-   0        0        0     8146 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/classes/issue_jira.py
--rw-rw-rw-   0        0        0     1505 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/classes/n8n_domain.py
--rw-rw-rw-   0        0        0     4729 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      527 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/dados_basicos_fatura.py
--rw-rw-rw-   0        0        0      526 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/dados_basicos_miro.py
--rw-rw-rw-   0        0        0       76 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      246 2024-05-29 18:45:22.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/fatura.py
--rw-rw-rw-   0        0        0       88 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/fatura_servico.py
--rw-rw-rw-   0        0        0      456 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0      410 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/item_servico.py
--rw-rw-rw-   0        0        0      485 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/itens_fatura.py
--rw-rw-rw-   0        0        0       97 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      398 2024-05-29 18:42:32.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      207 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0     1593 2024-05-29 15:16:24.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0     1154 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/nota_servico.py
--rw-rw-rw-   0        0        0      103 2024-05-29 18:44:59.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/pagamento.py
--rw-rw-rw-   0        0        0       92 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0      406 2024-05-31 13:24:32.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/sintese_servico.py
--rw-rw-rw-   0        0        0     6010 2024-05-31 14:49:06.000000 hnt_nf_jira_servicos_library-0.0.2/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-05-31 14:54:35.608523 hnt_nf_jira_servicos_library-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      501 2024-05-31 14:53:30.000000 hnt_nf_jira_servicos_library-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:55:07.085201 hnt_nf_jira_servicos_library-0.0.3/
+-rw-rw-rw-   0        0        0      267 2024-05-31 14:55:07.077112 hnt_nf_jira_servicos_library-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 14:55:07.075573 hnt_nf_jira_servicos_library-0.0.3/hnt_nf_jira_servicos_library.egg-info/
+-rw-rw-rw-   0        0        0      267 2024-05-31 14:55:06.000000 hnt_nf_jira_servicos_library-0.0.3/hnt_nf_jira_servicos_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-05-31 14:55:06.000000 hnt_nf_jira_servicos_library-0.0.3/hnt_nf_jira_servicos_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 14:55:06.000000 hnt_nf_jira_servicos_library-0.0.3/hnt_nf_jira_servicos_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-31 14:55:06.000000 hnt_nf_jira_servicos_library-0.0.3/hnt_nf_jira_servicos_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-31 14:55:06.000000 hnt_nf_jira_servicos_library-0.0.3/hnt_nf_jira_servicos_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 14:55:06.945744 hnt_nf_jira_servicos_library-0.0.3/nf_jira/
+-rw-rw-rw-   0        0        0       41 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:55:07.042152 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      211 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/chave_acesso.py
+drwxrwxrwx   0        0        0        0 2024-05-31 14:55:07.062155 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/
+-rw-rw-rw-   0        0        0     4245 2024-05-31 13:26:08.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/factories.py
+-rw-rw-rw-   0        0        0     4997 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/form_jira.py
+-rw-rw-rw-   0        0        0    13316 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/helper.py
+-rw-rw-rw-   0        0        0     1947 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/issue_fields.py
+-rw-rw-rw-   0        0        0     8146 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/issue_jira.py
+-rw-rw-rw-   0        0        0     1505 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/n8n_domain.py
+-rw-rw-rw-   0        0        0     4729 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      527 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/dados_basicos_fatura.py
+-rw-rw-rw-   0        0        0      526 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/dados_basicos_miro.py
+-rw-rw-rw-   0        0        0       76 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      246 2024-05-29 18:45:22.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/fatura.py
+-rw-rw-rw-   0        0        0       88 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/fatura_servico.py
+-rw-rw-rw-   0        0        0      456 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0      410 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/item_servico.py
+-rw-rw-rw-   0        0        0      485 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/itens_fatura.py
+-rw-rw-rw-   0        0        0       97 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      398 2024-05-29 18:42:32.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      207 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0     1593 2024-05-29 15:16:24.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0     1154 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/nota_servico.py
+-rw-rw-rw-   0        0        0      103 2024-05-29 18:44:59.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/pagamento.py
+-rw-rw-rw-   0        0        0       92 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0      406 2024-05-31 13:24:32.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/sintese_servico.py
+-rw-rw-rw-   0        0        0     6010 2024-05-31 14:49:06.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-05-31 14:55:07.086542 hnt_nf_jira_servicos_library-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      501 2024-05-31 14:55:01.000000 hnt_nf_jira_servicos_library-0.0.3/setup.py
```

### Comparing `hnt_nf_jira_servicos_library-0.0.2/README.md` & `hnt_nf_jira_servicos_library-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.2/hnt_nf_jira_servicos_library.egg-info/SOURCES.txt` & `hnt_nf_jira_servicos_library-0.0.3/hnt_nf_jira_servicos_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/classes/factories.py` & `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/factories.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/classes/form_jira.py` & `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/form_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/classes/helper.py` & `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/helper.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/classes/issue_fields.py` & `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/issue_fields.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/classes/issue_jira.py` & `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/issue_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/classes/n8n_domain.py` & `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/n8n_domain.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/constants.py` & `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/constants.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/dados_basicos_fatura.py` & `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/dados_basicos_fatura.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/dados_basicos_miro.py` & `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/dados_basicos_miro.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/nota_pedido.py` & `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/nota_pedido.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.2/nf_jira/entities/nota_servico.py` & `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/nota_servico.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.2/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_servicos_library-0.0.3/nf_jira/wrapper_nf_jira.py`

 * *Files identical despite different names*

