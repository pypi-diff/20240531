# Comparing `tmp/hnt_sap_service_library-0.0.2.tar.gz` & `tmp/hnt_sap_service_library-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_sap_service_library-0.0.2.tar", last modified: Fri May 31 13:30:22 2024, max compression
+gzip compressed data, was "hnt_sap_service_library-0.0.3.tar", last modified: Fri May 31 17:36:31 2024, max compression
```

## Comparing `hnt_sap_service_library-0.0.2.tar` & `hnt_sap_service_library-0.0.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 13:30:22.654539 hnt_sap_service_library-0.0.2/
--rw-rw-rw-   0        0        0      288 2024-05-31 13:30:22.649540 hnt_sap_service_library-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2248 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 13:30:22.556519 hnt_sap_service_library-0.0.2/hnt_sap_gui/
--rw-rw-rw-   0        0        0       54 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/RPA_HNT_Constants.py
--rw-rw-rw-   0        0        0       22 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:30:22.567520 hnt_sap_service_library-0.0.2/hnt_sap_gui/common/
--rw-rw-rw-   0        0        0      368 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/common/sap_status_bar.py
--rw-rw-rw-   0        0        0     2585 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/common/session.py
--rw-rw-rw-   0        0        0      370 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/common/tx_result.py
--rw-rw-rw-   0        0        0     4271 2024-05-31 12:53:02.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/hnt_sap.py
--rw-rw-rw-   0        0        0      388 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/hnt_sap_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:30:22.584520 hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/
--rw-rw-rw-   0        0        0     4257 2024-05-31 12:52:05.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/fatura_transaction.py
--rw-rw-rw-   0        0        0     1018 2024-05-31 12:52:15.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/liberacao_transaction.py
--rw-rw-rw-   0        0        0     6291 2024-05-31 12:53:24.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/miro_transaction.py
--rw-rw-rw-   0        0        0     9211 2024-05-31 12:51:50.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:30:22.646543 hnt_sap_service_library-0.0.2/hnt_sap_service_library.egg-info/
--rw-rw-rw-   0        0        0      288 2024-05-31 13:30:22.000000 hnt_sap_service_library-0.0.2/hnt_sap_service_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      720 2024-05-31 13:30:22.000000 hnt_sap_service_library-0.0.2/hnt_sap_service_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 13:30:22.000000 hnt_sap_service_library-0.0.2/hnt_sap_service_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-31 13:30:22.000000 hnt_sap_service_library-0.0.2/hnt_sap_service_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-31 13:30:22.000000 hnt_sap_service_library-0.0.2/hnt_sap_service_library.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 13:30:22.655538 hnt_sap_service_library-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      472 2024-05-31 13:30:15.000000 hnt_sap_service_library-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:30:22.642539 hnt_sap_service_library-0.0.2/tests/
--rw-rw-rw-   0        0        0      413 2024-05-31 12:52:05.000000 hnt_sap_service_library-0.0.2/tests/test_fatura.py
--rw-rw-rw-   0        0        0      378 2024-05-31 12:53:30.000000 hnt_sap_service_library-0.0.2/tests/test_miro.py
--rw-rw-rw-   0        0        0     1133 2024-05-31 12:53:37.000000 hnt_sap_service_library-0.0.2/tests/test_nota_pedido.py
+drwxrwxrwx   0        0        0        0 2024-05-31 17:36:31.499409 hnt_sap_service_library-0.0.3/
+-rw-rw-rw-   0        0        0      288 2024-05-31 17:36:31.499409 hnt_sap_service_library-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2248 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 17:36:31.427006 hnt_sap_service_library-0.0.3/hnt_sap_gui/
+-rw-rw-rw-   0        0        0       54 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/RPA_HNT_Constants.py
+-rw-rw-rw-   0        0        0       22 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 17:36:31.432862 hnt_sap_service_library-0.0.3/hnt_sap_gui/common/
+-rw-rw-rw-   0        0        0      368 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/common/sap_status_bar.py
+-rw-rw-rw-   0        0        0     2585 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/common/session.py
+-rw-rw-rw-   0        0        0      370 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/common/tx_result.py
+-rw-rw-rw-   0        0        0     4268 2024-05-31 17:32:49.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/hnt_sap.py
+-rw-rw-rw-   0        0        0      388 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/hnt_sap_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-31 17:36:31.447049 hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/
+-rw-rw-rw-   0        0        0     4257 2024-05-31 14:58:51.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/fatura_transaction.py
+-rw-rw-rw-   0        0        0     1018 2024-05-31 12:52:15.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/liberacao_transaction.py
+-rw-rw-rw-   0        0        0     6291 2024-05-31 12:53:24.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/miro_transaction.py
+-rw-rw-rw-   0        0        0     9211 2024-05-31 15:05:23.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py
+drwxrwxrwx   0        0        0        0 2024-05-31 17:36:31.496988 hnt_sap_service_library-0.0.3/hnt_sap_service_library.egg-info/
+-rw-rw-rw-   0        0        0      288 2024-05-31 17:36:31.000000 hnt_sap_service_library-0.0.3/hnt_sap_service_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      720 2024-05-31 17:36:31.000000 hnt_sap_service_library-0.0.3/hnt_sap_service_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 17:36:31.000000 hnt_sap_service_library-0.0.3/hnt_sap_service_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-31 17:36:31.000000 hnt_sap_service_library-0.0.3/hnt_sap_service_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-31 17:36:31.000000 hnt_sap_service_library-0.0.3/hnt_sap_service_library.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 17:36:31.499409 hnt_sap_service_library-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      472 2024-05-31 17:34:22.000000 hnt_sap_service_library-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 17:36:31.494406 hnt_sap_service_library-0.0.3/tests/
+-rw-rw-rw-   0        0        0      413 2024-05-31 14:58:51.000000 hnt_sap_service_library-0.0.3/tests/test_fatura.py
+-rw-rw-rw-   0        0        0      378 2024-05-31 12:53:30.000000 hnt_sap_service_library-0.0.3/tests/test_miro.py
+-rw-rw-rw-   0        0        0     1144 2024-05-31 15:03:58.000000 hnt_sap_service_library-0.0.3/tests/test_nota_pedido.py
```

### Comparing `hnt_sap_service_library-0.0.2/README.md` & `hnt_sap_service_library-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.2/hnt_sap_gui/common/session.py` & `hnt_sap_service_library-0.0.3/hnt_sap_gui/common/session.py`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.2/hnt_sap_gui/hnt_sap.py` & `hnt_sap_service_library-0.0.3/hnt_sap_gui/hnt_sap.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             "error": None
         }
         try:
             if 'nota_pedido' in data:
                 tx_result_nota_pedido = NotaPedidoTransaction().execute(self, nota_pedido=data['nota_pedido'])
                 results['nota_pedido'] = tx_result_nota_pedido
 
-                tx_result_liberacao = LiberacaoTransaction().execute(self, results['nota_pedido']['codigo'])
+                tx_result_liberacao = LiberacaoTransaction().execute(self, results['nota_pedido'].codigo)
                 results["liberacao"] = tx_result_liberacao
             
                 if COD_LIBERACAO_BLOQUADO == tx_result_liberacao.codigo:
                     logger.info(f"leave execute hnt_run_transaction_miro result:{', '.join([str(results[obj]) for  obj in results])}")
                     return results
             
                 results["miro"] = MiroTransaction().execute(self, data, results['nota_pedido']['codigo'])
```

### Comparing `hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/fatura_transaction.py` & `hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/fatura_transaction.py`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/liberacao_transaction.py` & `hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/liberacao_transaction.py`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/miro_transaction.py` & `hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/miro_transaction.py`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py` & `hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.2/hnt_sap_service_library.egg-info/SOURCES.txt` & `hnt_sap_service_library-0.0.3/hnt_sap_service_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.2/tests/test_nota_pedido.py` & `hnt_sap_service_library-0.0.3/tests/test_nota_pedido.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import json
 from os import getcwd, makedirs, path
 from hnt_sap_gui import SapGui
 
 def test_create():
-    with open("./expected_nota_servico.json", "r", encoding="utf-8") as nota_pedido_arquivo_json: nota_pedido = json.load(nota_pedido_arquivo_json)
-
+    with open("./devdata/json/expected_nota_servico.json", "r", encoding="utf-8") as nota_pedido_arquivo_json: nota_pedido = json.load(nota_pedido_arquivo_json)
     data = {
         "nota_pedido": nota_pedido,
     }
     result = SapGui().hnt_run_transaction(data)
     assert result is not None
 
 def test_get_many_codes():
```

