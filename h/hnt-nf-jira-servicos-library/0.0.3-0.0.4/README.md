# Comparing `tmp/hnt_nf_jira_servicos_library-0.0.3.tar.gz` & `tmp/hnt_nf_jira_servicos_library-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_nf_jira_servicos_library-0.0.3.tar", last modified: Fri May 31 14:55:07 2024, max compression
+gzip compressed data, was "hnt_nf_jira_servicos_library-0.0.4.tar", last modified: Fri May 31 17:36:57 2024, max compression
```

## Comparing `hnt_nf_jira_servicos_library-0.0.3.tar` & `hnt_nf_jira_servicos_library-0.0.4.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 14:55:07.085201 hnt_nf_jira_servicos_library-0.0.3/
--rw-rw-rw-   0        0        0      267 2024-05-31 14:55:07.077112 hnt_nf_jira_servicos_library-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      713 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 14:55:07.075573 hnt_nf_jira_servicos_library-0.0.3/hnt_nf_jira_servicos_library.egg-info/
--rw-rw-rw-   0        0        0      267 2024-05-31 14:55:06.000000 hnt_nf_jira_servicos_library-0.0.3/hnt_nf_jira_servicos_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-05-31 14:55:06.000000 hnt_nf_jira_servicos_library-0.0.3/hnt_nf_jira_servicos_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 14:55:06.000000 hnt_nf_jira_servicos_library-0.0.3/hnt_nf_jira_servicos_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-31 14:55:06.000000 hnt_nf_jira_servicos_library-0.0.3/hnt_nf_jira_servicos_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-31 14:55:06.000000 hnt_nf_jira_servicos_library-0.0.3/hnt_nf_jira_servicos_library.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 14:55:06.945744 hnt_nf_jira_servicos_library-0.0.3/nf_jira/
--rw-rw-rw-   0        0        0       41 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 14:55:07.042152 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/
--rw-rw-rw-   0        0        0       92 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/anexo.py
--rw-rw-rw-   0        0        0      211 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/chave_acesso.py
-drwxrwxrwx   0        0        0        0 2024-05-31 14:55:07.062155 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/
--rw-rw-rw-   0        0        0     4245 2024-05-31 13:26:08.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/factories.py
--rw-rw-rw-   0        0        0     4997 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/form_jira.py
--rw-rw-rw-   0        0        0    13316 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/helper.py
--rw-rw-rw-   0        0        0     1947 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/issue_fields.py
--rw-rw-rw-   0        0        0     8146 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/issue_jira.py
--rw-rw-rw-   0        0        0     1505 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/n8n_domain.py
--rw-rw-rw-   0        0        0     4729 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/constants.py
--rw-rw-rw-   0        0        0      527 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/dados_basicos_fatura.py
--rw-rw-rw-   0        0        0      526 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/dados_basicos_miro.py
--rw-rw-rw-   0        0        0       76 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/detalhe.py
--rw-rw-rw-   0        0        0      246 2024-05-29 18:45:22.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/fatura.py
--rw-rw-rw-   0        0        0       88 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/fatura_servico.py
--rw-rw-rw-   0        0        0      456 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/item.py
--rw-rw-rw-   0        0        0      410 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/item_servico.py
--rw-rw-rw-   0        0        0      485 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/itens_fatura.py
--rw-rw-rw-   0        0        0       97 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/jira_info.py
--rw-rw-rw-   0        0        0      398 2024-05-29 18:42:32.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/miro.py
--rw-rw-rw-   0        0        0      207 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/nfe_sefaz.py
--rw-rw-rw-   0        0        0     1593 2024-05-29 15:16:24.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/nota_pedido.py
--rw-rw-rw-   0        0        0     1154 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/nota_servico.py
--rw-rw-rw-   0        0        0      103 2024-05-29 18:44:59.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/pagamento.py
--rw-rw-rw-   0        0        0       92 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/referencia_pedido.py
--rw-rw-rw-   0        0        0      173 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/sintese_itens.py
--rw-rw-rw-   0        0        0       78 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/sintese_miro.py
--rw-rw-rw-   0        0        0      406 2024-05-31 13:24:32.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/sintese_servico.py
--rw-rw-rw-   0        0        0     6010 2024-05-31 14:49:06.000000 hnt_nf_jira_servicos_library-0.0.3/nf_jira/wrapper_nf_jira.py
--rw-rw-rw-   0        0        0       42 2024-05-31 14:55:07.086542 hnt_nf_jira_servicos_library-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      501 2024-05-31 14:55:01.000000 hnt_nf_jira_servicos_library-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 17:36:57.297449 hnt_nf_jira_servicos_library-0.0.4/
+-rw-rw-rw-   0        0        0      267 2024-05-31 17:36:57.295360 hnt_nf_jira_servicos_library-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 17:36:57.293356 hnt_nf_jira_servicos_library-0.0.4/hnt_nf_jira_servicos_library.egg-info/
+-rw-rw-rw-   0        0        0      267 2024-05-31 17:36:57.000000 hnt_nf_jira_servicos_library-0.0.4/hnt_nf_jira_servicos_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-05-31 17:36:57.000000 hnt_nf_jira_servicos_library-0.0.4/hnt_nf_jira_servicos_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 17:36:57.000000 hnt_nf_jira_servicos_library-0.0.4/hnt_nf_jira_servicos_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-31 17:36:57.000000 hnt_nf_jira_servicos_library-0.0.4/hnt_nf_jira_servicos_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-31 17:36:57.000000 hnt_nf_jira_servicos_library-0.0.4/hnt_nf_jira_servicos_library.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 17:36:57.223010 hnt_nf_jira_servicos_library-0.0.4/nf_jira/
+-rw-rw-rw-   0        0        0       41 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 17:36:57.276393 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/
+-rw-rw-rw-   0        0        0       92 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/anexo.py
+-rw-rw-rw-   0        0        0      211 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/chave_acesso.py
+drwxrwxrwx   0        0        0        0 2024-05-31 17:36:57.289378 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/classes/
+-rw-rw-rw-   0        0        0     4242 2024-05-31 17:29:10.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/classes/factories.py
+-rw-rw-rw-   0        0        0     5206 2024-05-31 17:24:07.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/classes/form_jira.py
+-rw-rw-rw-   0        0        0    13316 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/classes/helper.py
+-rw-rw-rw-   0        0        0     1947 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/classes/issue_fields.py
+-rw-rw-rw-   0        0        0     8146 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/classes/issue_jira.py
+-rw-rw-rw-   0        0        0     1505 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/classes/n8n_domain.py
+-rw-rw-rw-   0        0        0     4729 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/constants.py
+-rw-rw-rw-   0        0        0      527 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/dados_basicos_fatura.py
+-rw-rw-rw-   0        0        0      526 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/dados_basicos_miro.py
+-rw-rw-rw-   0        0        0       76 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/detalhe.py
+-rw-rw-rw-   0        0        0      246 2024-05-29 18:45:22.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/fatura.py
+-rw-rw-rw-   0        0        0       88 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/fatura_servico.py
+-rw-rw-rw-   0        0        0      456 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/item.py
+-rw-rw-rw-   0        0        0      410 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/item_servico.py
+-rw-rw-rw-   0        0        0      485 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/itens_fatura.py
+-rw-rw-rw-   0        0        0       97 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/jira_info.py
+-rw-rw-rw-   0        0        0      398 2024-05-29 18:42:32.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/miro.py
+-rw-rw-rw-   0        0        0      207 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/nfe_sefaz.py
+-rw-rw-rw-   0        0        0     1593 2024-05-29 15:16:24.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/nota_pedido.py
+-rw-rw-rw-   0        0        0     1154 2024-05-29 18:39:30.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/nota_servico.py
+-rw-rw-rw-   0        0        0      103 2024-05-29 18:44:59.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/pagamento.py
+-rw-rw-rw-   0        0        0       92 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/referencia_pedido.py
+-rw-rw-rw-   0        0        0      173 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/sintese_itens.py
+-rw-rw-rw-   0        0        0       78 2024-05-28 12:01:11.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/sintese_miro.py
+-rw-rw-rw-   0        0        0      406 2024-05-31 13:24:32.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/sintese_servico.py
+-rw-rw-rw-   0        0        0     6010 2024-05-31 14:49:06.000000 hnt_nf_jira_servicos_library-0.0.4/nf_jira/wrapper_nf_jira.py
+-rw-rw-rw-   0        0        0       42 2024-05-31 17:36:57.297449 hnt_nf_jira_servicos_library-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      501 2024-05-31 17:36:53.000000 hnt_nf_jira_servicos_library-0.0.4/setup.py
```

### Comparing `hnt_nf_jira_servicos_library-0.0.3/README.md` & `hnt_nf_jira_servicos_library-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.3/hnt_nf_jira_servicos_library.egg-info/SOURCES.txt` & `hnt_nf_jira_servicos_library-0.0.4/hnt_nf_jira_servicos_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/factories.py` & `hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/classes/factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
             "nro_servico": issue["json_data"][CODIGO_SAP_SERVICO][0],
             "centro_custo": f"{issue['json_data'][CENTRO_DE_CUSTO][0]}" if CENTRO_DE_CUSTO in issue["json_data"] and issue["json_data"][CENTRO_DE_CUSTO] != None else None,
             "ord_interna": f"{issue['json_data'][ORDEM_INTERNA][0]}" if ORDEM_INTERNA in issue["json_data"] and issue["json_data"][ORDEM_INTERNA] != None else None,
             "valor_bruto": float(issue["json_data"][VALOR_TOTAL_DA_FATURA].replace(",","."))
         }
 
         fatura = {
-            "cod_imposto": issue['json_data'][CODIGO_IMPOSTO][0]
+            "cod_imposto": issue['json_data'][CODIGO_IMPOSTO]
         }
 
         sintese_item = {
             "categoria_cc": "K" if item['centro_custo'] is not None else "F",
             "centro": issue['domain_data']['centro']['centro'],
             "texto_breve": issue['json_data']["texto_breve"],
             "fatura": fatura,
```

### Comparing `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/form_jira.py` & `hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/classes/form_jira.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,17 +85,21 @@
         fields_values = data.get('state')['answers']
         fields_root = data.get('design')['questions']
         
         for root in fields_root:
 
             field_name = fields_root[root].get('questionKey')
             if fields_values.get(root) is not None:
-                # field_index = list(fields_values.get(root).keys())[0]
                 if "choices" in list(fields_values.get(root).keys()):
-                    field_value = fields_values.get(root)['choices']
+                    if field_name == 'codigo_imposto':
+                        field_index = fields_values.get(root)['choices'][0]
+                        field_value = fields_root[root]['choices'][int(field_index) - 1]['label'].split(' ', 1)[0]
+                    else:
+                        field_value = fields_values.get(root)['choices']
+
                 else:
                     field_index = list(fields_values.get(root).keys())[0]
                     field_value = fields_values.get(root)[field_index]
             else: 
                 field_value = None
 
             fields_json[field_name] = field_value
```

### Comparing `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/helper.py` & `hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/classes/helper.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/issue_fields.py` & `hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/classes/issue_fields.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/issue_jira.py` & `hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/classes/issue_jira.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/classes/n8n_domain.py` & `hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/classes/n8n_domain.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/constants.py` & `hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/constants.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/dados_basicos_fatura.py` & `hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/dados_basicos_fatura.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/dados_basicos_miro.py` & `hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/dados_basicos_miro.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/nota_pedido.py` & `hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/nota_pedido.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.3/nf_jira/entities/nota_servico.py` & `hnt_nf_jira_servicos_library-0.0.4/nf_jira/entities/nota_servico.py`

 * *Files identical despite different names*

### Comparing `hnt_nf_jira_servicos_library-0.0.3/nf_jira/wrapper_nf_jira.py` & `hnt_nf_jira_servicos_library-0.0.4/nf_jira/wrapper_nf_jira.py`

 * *Files identical despite different names*

