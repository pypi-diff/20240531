# Comparing `tmp/hnt_sap_service_library-0.0.1.tar.gz` & `tmp/hnt_sap_service_library-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_sap_service_library-0.0.1.tar", last modified: Fri May 31 12:10:04 2024, max compression
+gzip compressed data, was "hnt_sap_service_library-0.0.2.tar", last modified: Fri May 31 13:30:22 2024, max compression
```

## Comparing `hnt_sap_service_library-0.0.1.tar` & `hnt_sap_service_library-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 12:10:04.421482 hnt_sap_service_library-0.0.1/
--rw-rw-rw-   0        0        0      279 2024-05-31 12:10:04.412768 hnt_sap_service_library-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2248 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 12:10:04.312832 hnt_sap_service_library-0.0.1/hnt_sap_gui/
--rw-rw-rw-   0        0        0       54 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.1/hnt_sap_gui/RPA_HNT_Constants.py
--rw-rw-rw-   0        0        0       22 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.1/hnt_sap_gui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:10:04.329782 hnt_sap_service_library-0.0.1/hnt_sap_gui/common/
--rw-rw-rw-   0        0        0      368 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.1/hnt_sap_gui/common/sap_status_bar.py
--rw-rw-rw-   0        0        0     2585 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.1/hnt_sap_gui/common/session.py
--rw-rw-rw-   0        0        0      370 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.1/hnt_sap_gui/common/tx_result.py
--rw-rw-rw-   0        0        0     4081 2024-05-31 12:07:06.000000 hnt_sap_service_library-0.0.1/hnt_sap_gui/hnt_sap.py
--rw-rw-rw-   0        0        0      388 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.1/hnt_sap_gui/hnt_sap_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:10:04.346502 hnt_sap_service_library-0.0.1/hnt_sap_gui/nota_fiscal/
--rw-rw-rw-   0        0        0     4217 2024-05-31 12:07:06.000000 hnt_sap_service_library-0.0.1/hnt_sap_gui/nota_fiscal/fatura_transaction.py
--rw-rw-rw-   0        0        0     1018 2024-05-31 12:07:06.000000 hnt_sap_service_library-0.0.1/hnt_sap_gui/nota_fiscal/liberacao_transaction.py
--rw-rw-rw-   0        0        0     7410 2024-05-31 12:07:06.000000 hnt_sap_service_library-0.0.1/hnt_sap_gui/nota_fiscal/miro_transaction.py
--rw-rw-rw-   0        0        0     8680 2024-05-31 12:07:06.000000 hnt_sap_service_library-0.0.1/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:10:04.412768 hnt_sap_service_library-0.0.1/hnt_sap_service_library.egg-info/
--rw-rw-rw-   0        0        0      279 2024-05-31 12:10:03.000000 hnt_sap_service_library-0.0.1/hnt_sap_service_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      744 2024-05-31 12:10:04.000000 hnt_sap_service_library-0.0.1/hnt_sap_service_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 12:10:03.000000 hnt_sap_service_library-0.0.1/hnt_sap_service_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-31 12:10:03.000000 hnt_sap_service_library-0.0.1/hnt_sap_service_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-31 12:10:03.000000 hnt_sap_service_library-0.0.1/hnt_sap_service_library.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 12:10:04.421985 hnt_sap_service_library-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      463 2024-05-31 12:09:04.000000 hnt_sap_service_library-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 12:10:04.406017 hnt_sap_service_library-0.0.1/tests/
--rw-rw-rw-   0        0        0      284 2024-05-31 12:07:06.000000 hnt_sap_service_library-0.0.1/tests/test_fatura.py
--rw-rw-rw-   0        0        0      287 2024-05-31 12:07:06.000000 hnt_sap_service_library-0.0.1/tests/test_liberacao.py
--rw-rw-rw-   0        0        0      331 2024-05-31 12:07:06.000000 hnt_sap_service_library-0.0.1/tests/test_miro.py
--rw-rw-rw-   0        0        0      605 2024-05-31 12:07:06.000000 hnt_sap_service_library-0.0.1/tests/test_nota_pedido.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:30:22.654539 hnt_sap_service_library-0.0.2/
+-rw-rw-rw-   0        0        0      288 2024-05-31 13:30:22.649540 hnt_sap_service_library-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2248 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 13:30:22.556519 hnt_sap_service_library-0.0.2/hnt_sap_gui/
+-rw-rw-rw-   0        0        0       54 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/RPA_HNT_Constants.py
+-rw-rw-rw-   0        0        0       22 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:30:22.567520 hnt_sap_service_library-0.0.2/hnt_sap_gui/common/
+-rw-rw-rw-   0        0        0      368 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/common/sap_status_bar.py
+-rw-rw-rw-   0        0        0     2585 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/common/session.py
+-rw-rw-rw-   0        0        0      370 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/common/tx_result.py
+-rw-rw-rw-   0        0        0     4271 2024-05-31 12:53:02.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/hnt_sap.py
+-rw-rw-rw-   0        0        0      388 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/hnt_sap_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:30:22.584520 hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/
+-rw-rw-rw-   0        0        0     4257 2024-05-31 12:52:05.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/fatura_transaction.py
+-rw-rw-rw-   0        0        0     1018 2024-05-31 12:52:15.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/liberacao_transaction.py
+-rw-rw-rw-   0        0        0     6291 2024-05-31 12:53:24.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/miro_transaction.py
+-rw-rw-rw-   0        0        0     9211 2024-05-31 12:51:50.000000 hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:30:22.646543 hnt_sap_service_library-0.0.2/hnt_sap_service_library.egg-info/
+-rw-rw-rw-   0        0        0      288 2024-05-31 13:30:22.000000 hnt_sap_service_library-0.0.2/hnt_sap_service_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      720 2024-05-31 13:30:22.000000 hnt_sap_service_library-0.0.2/hnt_sap_service_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 13:30:22.000000 hnt_sap_service_library-0.0.2/hnt_sap_service_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-31 13:30:22.000000 hnt_sap_service_library-0.0.2/hnt_sap_service_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-31 13:30:22.000000 hnt_sap_service_library-0.0.2/hnt_sap_service_library.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 13:30:22.655538 hnt_sap_service_library-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      472 2024-05-31 13:30:15.000000 hnt_sap_service_library-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 13:30:22.642539 hnt_sap_service_library-0.0.2/tests/
+-rw-rw-rw-   0        0        0      413 2024-05-31 12:52:05.000000 hnt_sap_service_library-0.0.2/tests/test_fatura.py
+-rw-rw-rw-   0        0        0      378 2024-05-31 12:53:30.000000 hnt_sap_service_library-0.0.2/tests/test_miro.py
+-rw-rw-rw-   0        0        0     1133 2024-05-31 12:53:37.000000 hnt_sap_service_library-0.0.2/tests/test_nota_pedido.py
```

### Comparing `hnt_sap_service_library-0.0.1/README.md` & `hnt_sap_service_library-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.1/hnt_sap_gui/common/session.py` & `hnt_sap_service_library-0.0.2/hnt_sap_gui/common/session.py`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.1/hnt_sap_gui/hnt_sap.py` & `hnt_sap_service_library-0.0.2/hnt_sap_gui/hnt_sap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import logging
 import locale
 from SapGuiLibrary import SapGuiLibrary
 from dotenv import load_dotenv
 
 from hnt_sap_gui.RPA_HNT_Constants import COD_LIBERACAO_BLOQUADO
-from hnt_sap_gui.nota_fiscal.fatura_transaction import FaturaTransaction
-from hnt_sap_gui.nota_fiscal.miro_transaction import MiroTransaction
 
 from .common.session import sessionable
 from .nota_fiscal.nota_pedido_transaction import NotaPedidoTransaction
+from .nota_fiscal.fatura_transaction import FaturaTransaction
+from .nota_fiscal.miro_transaction import MiroTransaction
 from .nota_fiscal.liberacao_transaction import LiberacaoTransaction
 
 logger = logging.getLogger(__name__)
 
 class SapGui(SapGuiLibrary):
     def __init__(self) -> None:
         locale.setlocale(locale.LC_ALL, ('pt_BR.UTF-8'))
@@ -22,76 +22,84 @@
         return locale.format_string("%.2f", value)
 
     @sessionable
     def hnt_run_transaction(self, data):
         logger.info(f"enter execute run_hnt_transactions data:{data}")
         results = {
             "nota_pedido": None,
-            "liberacao": None,
-            "miro": None,
             "error": None
         }
         try:
-            tx_result_nota_pedido = NotaPedidoTransaction().execute(self, nota_pedido=data['nota_pedido'])
-            results['nota_pedido'] = tx_result_nota_pedido
-            tx_result_liberacao = LiberacaoTransaction().execute(self, tx_result_nota_pedido.codigo)
-            results['liberacao'] = tx_result_liberacao
-            if COD_LIBERACAO_BLOQUADO == tx_result_liberacao.codigo:
-                logger.info(f"leave execute run_hnt_transactions result:{', '.join([str(results[obj]) for obj in results])}")
-                return results
+            if 'nota_pedido' in data:
+                tx_result_nota_pedido = NotaPedidoTransaction().execute(self, nota_pedido=data['nota_pedido'])
+                results['nota_pedido'] = tx_result_nota_pedido
+
+                tx_result_liberacao = LiberacaoTransaction().execute(self, results['nota_pedido']['codigo'])
+                results["liberacao"] = tx_result_liberacao
+            
+                if COD_LIBERACAO_BLOQUADO == tx_result_liberacao.codigo:
+                    logger.info(f"leave execute hnt_run_transaction_miro result:{', '.join([str(results[obj]) for  obj in results])}")
+                    return results
             
-            results['miro'] = MiroTransaction().execute(self, data=data["miro"], numero_pedido=tx_result_nota_pedido.codigo)
+                results["miro"] = MiroTransaction().execute(self, data, results['nota_pedido']['codigo'])
         except Exception as ex:
             logger.error(str(ex))
             results["error"] = str(ex)
         logger.info(f"leave execute run_hnt_transactions result:{', '.join([str(results[obj]) for obj in results])}")
         return results
-
+    
     @sessionable
-    def hnt_run_transaction_miro(self, numero_pedido, data):
-        logger.info(f"enter execute hnt_run_transaction_miro data:{data}")
+    def hnt_run_transaction_FV60(self, data):
         results = {
-            "liberacao": None,
-            "miro": None,
+            "fatura": None,
             "error": None
         }
         try:
-            tx_result_liberacao = LiberacaoTransaction().execute(self, numero_pedido)
-            results["liberacao"] = tx_result_liberacao
-            if COD_LIBERACAO_BLOQUADO == tx_result_liberacao.codigo:
-                logger.info(f"leave execute hnt_run_transaction_miro result:{', '.join([str(results[obj]) for obj in results])}")
-                return results
-            
-            results['miro'] = MiroTransaction().execute(self, data, numero_pedido)
+            results["fatura"] = FaturaTransaction().execute(self, data)
         except Exception as ex:
             logger.error(str(ex))
             results["error"] = str(ex)
-        logger.info(f"leave execute hnt_run_transaction_miro result:{', '.join([str(results[obj]) for obj in results])}")
+        logger.info(f"leave execute run_hnt_transactions result:{', '.join([str(results[obj]) for obj in results])}")
         return results
 
     @sessionable
-    def hnt_run_transaction_FV60(self, data):
+    def hnt_run_transaction_ME21N(self, data):
+        logger.info(f"enter execute run_hnt_transactions data:{data}")
         results = {
-            "fatura": None,
+            "nota_pedido": None,
             "error": None
         }
         try:
-            results["fatura"] = FaturaTransaction().execute(self, data)
+            if 'nota_pedido' in data:
+                tx_result_nota_pedido = NotaPedidoTransaction().execute(self, nota_pedido=data['nota_pedido'])
+                results['nota_pedido'] = tx_result_nota_pedido
         except Exception as ex:
             logger.error(str(ex))
             results["error"] = str(ex)
-        logger.info(f"leave execute hnt_run_transaction_FV60 result:{', '.join([str(results[obj]) for obj in results])}")
+        logger.info(f"leave execute run_hnt_transactions result:{', '.join([str(results[obj]) for obj in results])}")
         return results
-
+    
     @sessionable
-    def hnt_run_transaction_liberacao(self, cod_nota_pedido):
+    def hnt_run_transaction_miro(self, numero_pedido, data):
+        logger.info(f"enter execute run_hnt_transactions data:{data}")
         results = {
+            "miro": None,
             "liberacao": None,
             "error": None
         }
+
         try:
-            results["liberacao"] = LiberacaoTransaction().execute(self, cod_nota_pedido)
-        except Exception as ex:
-            logger.error(str(ex))
-            results["error"] = str(ex)
-        logger.info(f"leave execute hnt_run_transaction_FV60 result:{', '.join([str(results[obj]) for obj in results])}")
+            tx_result_liberacao = LiberacaoTransaction().execute(self, numero_pedido)
+            results["liberacao"] = tx_result_liberacao
+            
+            if COD_LIBERACAO_BLOQUADO == tx_result_liberacao.codigo:
+                logger.info(f"leave execute hnt_run_transaction_miro result:{', '.join([str(results[obj]) for  obj in results])}")
+                return results
+            
+            results["miro"] = MiroTransaction().execute(self, data, numero_pedido)
+
+        except Exception as e:
+            logger.error(str(e))
+            results["error"] = str(e)
+
+        logger.info(f"leave execute hnt_run_transaction_miro result:{', '.join([str(results[obj]) for obj in results])}")
         return results
```

### Comparing `hnt_sap_service_library-0.0.1/hnt_sap_gui/nota_fiscal/fatura_transaction.py` & `hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/fatura_transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             sapGuiLib.session.findById("wnd[1]/tbar[0]/btn[0]").press()
 
         # ABA DADOS BÁSICOS
         sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpMAIN/ssubPAGE:SAPLFDCB:0010/ctxtINVFO-ACCNT").Text = fatura['dados_basicos']['cod_fornecedor']
         sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpMAIN/ssubPAGE:SAPLFDCB:0010/ctxtINVFO-BLDAT").Text = fatura['dados_basicos']['data_fatura']
         sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpMAIN/ssubPAGE:SAPLFDCB:0010/txtINVFO-XBLNR").Text = fatura['dados_basicos']['referencia']
         sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpMAIN/ssubPAGE:SAPLFDCB:0010/txtINVFO-WRBTR").Text = sapGuiLib.format_float(fatura['dados_basicos']['montante'])
-        sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpMAIN/ssubPAGE:SAPLFDCB:0010/ctxtINVFO-BUPLA").Text = fatura['dados_basicos']['bus_pl_sec_cd']
+        sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpMAIN/ssubPAGE:SAPLFDCB:0010/ctxtINVFO-BUPLA").Text = fatura['dados_basicos']['loc_negocios'] ## 'Loc.negócios Domains.centro.centro_loja
         sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpMAIN/ssubPAGE:SAPLFDCB:0010/ctxtINVFO-SGTXT").Text = fatura['dados_basicos']['texto']
         sapGuiLib.send_vkey(0)
         status = sapGuiLib.session.findById("wnd[0]/sbar").Text
         if sbar_extracted_text(MSG_SAP_JA_FOI_CRIADO, status) != None:
             raise HntSapException(status)
         for i, iten in enumerate(fatura['dados_basicos']['itens']):
             sapGuiLib.session.findById(f"wnd[0]/usr/subITEMS:SAPLFSKB:0100/tblSAPLFSKBTABLE/ctxtACGL_ITEM-HKONT[1,{i}]").Text = iten['cta_razao']
@@ -51,9 +51,8 @@
             sapGuiLib.send_vkey(0)
 
         sapGuiLib.session.findById("wnd[0]/tbar[1]/btn[42]").press()
         sbar = sapGuiLib.session.findById("wnd[0]/sbar").Text
         documento = sbar_extracted_text(MSG_SAP_CODIGO_DOCUMENTO, sbar)
         if documento == None:
             raise HntSapException(sbar)
-        return TxResult(documento, sbar)
-
+        return TxResult(documento, sbar)
```

### Comparing `hnt_sap_service_library-0.0.1/hnt_sap_gui/nota_fiscal/liberacao_transaction.py` & `hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/liberacao_transaction.py`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.1/hnt_sap_gui/nota_fiscal/miro_transaction.py` & `hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/miro_transaction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,95 @@
 import logging
 from hnt_sap_gui.common.sap_status_bar import sbar_extracted_text
 from hnt_sap_gui.common.tx_result import TxResult
 from hnt_sap_gui.hnt_sap_exception import HntSapException
 
 logger = logging.getLogger(__name__)
-
 MSG_SAP_EXIST_DOC = '^Verificar se fatura já foi registrada sob documento contábil ([0-9]{10,15}) ([0-9]+)$'
 MSG_SAP_CODIGO_DOCUMENTO = '^O documento do faturamento ([0-9]{10,15}) foi registrado  \( Doc.contábil ([0-9]{10,15}) \)$'
 MSG_MIRO_SEM_ESTRAGIA_DE_APROVACAO = "^Doc.faturamento ([0-9]+) lançado; bloqueado para pagamento  \( Doc.contábil ([0-9]+) \)$"
 MSG_MIRO_VALID_PERIOD = "Períodos contábeis permitidos:"
-# Ex status bar msgs:
-# Verificar se fatura já foi registrada sob documento contábil 5100918001 2024
-# O documento de compra 4505629945 ainda não está liberado
-# Doc.faturamento 5109872720 lançado; bloqueado para pagamento  ( Doc.contábil 5100526500 )
-# Ped.C.Custo/Ordem criado sob o nº 4505629947
-
 class MiroTransaction:
     def __init__(self) -> None:
         pass
 
-    def execute(self, sapGuiLib, data, numero_pedido):
-        sapGuiLib.run_transaction("/nMIRO")
-        sapGuiLib.send_vkey(0)
+    def execute(self, sapGuiLib, miro, numero_pedido):
+        logger.info(f"enter execute miro:{miro}")
+        #ABRE TRANSAÇÃO
+        sapGuiLib.session.findById("wnd[0]/tbar[0]/okcd").Text = "/nMIRO"
+        sapGuiLib.session.findById("wnd[0]").sendVKey(0)
         if sapGuiLib.session.findById("wnd[1]/usr/ctxtBKPF-BUKRS", False) != None:
             sapGuiLib.session.findById("wnd[1]/usr/ctxtBKPF-BUKRS").Text = "HFNT"
             sapGuiLib.session.findById("wnd[1]/tbar[0]/btn[0]").press()
-            
-        sapGuiLib.session.findById("wnd[0]/usr/cmbRM08M-VORGANG").Key = "1"
-        sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/tabsHEADER/tabpHEADER_TOTAL/ssubHEADER_SCREEN:SAPLFDCB:0010/ctxtINVFO-BLDAT").Text = data['dados_basicos']['data_da_fatura'] #Data da fatura
-        sapGuiLib.send_vkey(0)
-        sapGuiLib.send_vkey(0)
+        
+        sapGuiLib.session.findById("wnd[0]/usr/cmbRM08M-VORGANG").Key = "1"  #Operação: "Fatura"
+
+
+    #====================================
+    #         Aba | DdsBásicos
+    #====================================
+
+        sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/tabsHEADER/tabpHEADER_TOTAL/ssubHEADER_SCREEN:SAPLFDCB:0010/ctxtINVFO-BLDAT").Text = miro["dados_basicos"]["data_da_fatura"] #Data da fatura Form.Data Emissão
+        sapGuiLib.session.findById("wnd[0]").sendVKey(0)
+        sapGuiLib.session.findById("wnd[0]").sendVKey(0)
+
         if sapGuiLib.session.findById("wnd[1]/usr/txtMESSTXT1", False) != None:
             msg1 = sapGuiLib.session.findById("wnd[1]/usr/txtMESSTXT1").Text
             msg2 = sapGuiLib.session.findById("wnd[1]/usr/txtMESSTXT2").Text
             sapGuiLib.send_vkey(0)
             if MSG_MIRO_VALID_PERIOD == msg1:
                 raise HntSapException(f"{msg1} : {msg2}")
-
-        sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/tabsHEADER/tabpHEADER_TOTAL/ssubHEADER_SCREEN:SAPLFDCB:0010/txtINVFO-XBLNR").Text = data['dados_basicos']['referencia'] #Referência (Nº NF | Formato: 9 dígitos + "-" + série com 3 dígitos)
-        sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/tabsHEADER/tabpHEADER_TOTAL/ssubHEADER_SCREEN:SAPLFDCB:0010/txtINVFO-WRBTR").Text = sapGuiLib.format_float(data['dados_basicos']['montante'])  #Montante
-        sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/tabsHEADER/tabpHEADER_TOTAL/ssubHEADER_SCREEN:SAPLFDCB:0010/ctxtINVFO-SGTXT").Text = data['dados_basicos']['texto']  #Texto (Mês de referência + Dt leitura anterior + Dt leitura atual)
-        sapGuiLib.send_vkey(0)
+            
+        sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/tabsHEADER/tabpHEADER_TOTAL/ssubHEADER_SCREEN:SAPLFDCB:0010/txtINVFO-XBLNR").Text = miro["dados_basicos"]["referencia"]  #Referência (Nº NF | Formato: 9 dígitos + "-" + série com 3 dígitos) Form.Nº Nota Fiscal (Ver regra em consumo)
+        sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/tabsHEADER/tabpHEADER_TOTAL/ssubHEADER_SCREEN:SAPLFDCB:0010/txtINVFO-WRBTR").Text = miro["dados_basicos"]["montante"]  #Montante Form.Valor Nota
+        sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/tabsHEADER/tabpHEADER_TOTAL/ssubHEADER_SCREEN:SAPLFDCB:0010/ctxtINVFO-SGTXT").Text = miro["dados_basicos"]["texto"]  #Texto (Mês de referência + Dt leitura anterior + Dt leitura atual) TODO
+        sapGuiLib.session.findById("wnd[0]").sendVKey(0)
 
 
+    #====================================
+    #    ABA | REFERÊNCIA AO PEDIDO
+    #====================================
+    
         sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/subITEMS:SAPLMR1M:6010/tabsITEMTAB/tabpITEMS_PO/ssubTABS:SAPLMR1M:6020/subREFERENZBELEG:SAPLMR1M:6211/ctxtRM08M-EBELN").Text = numero_pedido  #Nº Pedido
-        sapGuiLib.send_vkey(0)
+        sapGuiLib.session.findById("wnd[0]").sendVKey(0)
+        sapGuiLib.session.findById("wnd[0]").sendVKey(0)
+    
+    #Caso haja pendência de liberação, o SAP exibirá a seguinte mensagem na barra de status:
+    #O documento de compra 4505629357 ainda não está liberado
+
+    #Caso o SAP identifique fatura registrada com os mesmos dados, será exibida a seguinte mensagem impeditiva na barra de status:
+    #Verificar se fatura já foi registrada sob documento contábil 5100528501 2024  (O nº de doc exibido na msg refere a MIRO criada anteriormente com os mesmos dados)
+
+
+    #====================================
+    #           Aba | Detalhe
+    #====================================
 
-        sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/tabsHEADER/tabpHEADER_PAY").Select()  #Exibe Pagamento
-        sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/tabsHEADER/tabpHEADER_PAY/ssubHEADER_SCREEN:SAPLFDCB:0020/ctxtINVFO-ZFBDT").Text = data['pagamento']['data_basica'] #Data de vencimento
-        sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/tabsHEADER/tabpHEADER_PAY/ssubHEADER_SCREEN:SAPLFDCB:0020/ctxtINVFO-ZTERM").Text = data['pagamento']['cond_pgto']
-        sapGuiLib.send_vkey(0)
-        
         sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/tabsHEADER/tabpHEADER_FI").Select()  #Exibe cabeçalho
         if sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/tabsHEADER/tabpHEADER_FI/ssubHEADER_SCREEN:SAPLFDCB:0150/ctxtINVFO-J_1BNFTYPE", False) == None:
             msg = sapGuiLib.session.findById("wnd[0]/sbar").Text
             if sbar_extracted_text(MSG_SAP_EXIST_DOC, msg) != None:
                 raise HntSapException(msg)
 
-        sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/tabsHEADER/tabpHEADER_FI/ssubHEADER_SCREEN:SAPLFDCB:0150/ctxtINVFO-J_1BNFTYPE").Text = data['detalhe']['ctg_nf']  #Ctg.NF
-        sapGuiLib.send_vkey(0)
-        sapGuiLib.session.findById("wnd[0]/tbar[1]/btn[21]").press()
-        sapGuiLib.session.findById("wnd[0]/usr/tabsTABSTRIP1/tabpTAB1/ssubHEADER_TAB:SAPLJ1BB2:2100/tblSAPLJ1BB2ITEM_CONTROL/ctxtJ_1BDYLIN-CFOP[9,0]").Text = data['sintese']['CFOP']  #CFOP
-        
-        if data['dados_nfe']['chave_acesso_sefaz']['tp_emissao'] != None and data['dados_nfe']['nfe_sefaz']['numero_log'] != None:
-            sapGuiLib.session.findById("wnd[0]/usr/tabsTABSTRIP1/tabpTAB8").Select()
-            sapGuiLib.session.findById("wnd[0]/usr/tabsTABSTRIP1/tabpTAB8/ssubHEADER_TAB:SAPLJ1BB2:2800/subRANDOM_NUMBER:SAPLJ1BB2:2801/ctxtJ_1BNFE_DOCNUM9_DIVIDED-TPEMIS").Text = data['dados_nfe']['chave_acesso_sefaz']['tp_emissao']  #Tipo emissão (1 dígitos da Chave de Acesso, contando a partir do dígito 35)
-            sapGuiLib.session.findById("wnd[0]/usr/tabsTABSTRIP1/tabpTAB8/ssubHEADER_TAB:SAPLJ1BB2:2800/subRANDOM_NUMBER:SAPLJ1BB2:2801/txtJ_1BNFE_DOCNUM9_DIVIDED-DOCNUM8").Text = data['dados_nfe']['chave_acesso_sefaz']['numero_aleatorio']  #Nº aleatório (8 dígitos da Chave de Acesso, contando a partir do dígito 36)
-            sapGuiLib.session.findById("wnd[0]/usr/tabsTABSTRIP1/tabpTAB8/ssubHEADER_TAB:SAPLJ1BB2:2800/subRANDOM_NUMBER:SAPLJ1BB2:2801/txtJ_1BNFE_ACTIVE-CDV").Text = data['dados_nfe']['chave_acesso_sefaz']['dig_verif']  #Díg.verif.
-            sapGuiLib.session.findById("wnd[0]/usr/tabsTABSTRIP1/tabpTAB8/ssubHEADER_TAB:SAPLJ1BB2:2800/subTIMESTAMP:SAPLJ1BB2:2803/txtJ_1BDYDOC-AUTHCOD").Text = data['dados_nfe']['nfe_sefaz']['numero_log']  #Nº do log (Protocolo de autorização - 15 primeiros dígitos)
-            sapGuiLib.session.findById("wnd[0]/usr/tabsTABSTRIP1/tabpTAB8/ssubHEADER_TAB:SAPLJ1BB2:2800/subTIMESTAMP:SAPLJ1BB2:2803/ctxtJ_1BDYDOC-AUTHDATE").Text = data['dados_nfe']['nfe_sefaz']['data_procmto']  #Data procmto.
-            sapGuiLib.session.findById("wnd[0]/usr/tabsTABSTRIP1/tabpTAB8/ssubHEADER_TAB:SAPLJ1BB2:2800/subTIMESTAMP:SAPLJ1BB2:2803/ctxtJ_1BDYDOC-AUTHTIME").Text = data['dados_nfe']['nfe_sefaz']['hora_procmto']  #Hora procmto.
-            sapGuiLib.send_vkey(0)
+        sapGuiLib.session.findById("wnd[0]/usr/subHEADER_AND_ITEMS:SAPLMR1M:6005/tabsHEADER/tabpHEADER_FI/ssubHEADER_SCREEN:SAPLFDCB:0150/ctxtINVFO-J_1BNFTYPE").Text = miro["detalhe"]["ctg_nf"]   #Ctg.NF Form.Forncedor categoria NF
+        sapGuiLib.session.findById("wnd[0]").sendVKey(0)
+
+
+    #====================================
+    #        Botão | Nota Fiscal
+    #====================================
+
+        sapGuiLib.session.findById("wnd[0]/tbar[1]/btn[21]").press()  #Botão [Nota Fiscal] \ Menu superior SAP
+    
+    #Aba | Síntese
+    #====================================
+    
+        sapGuiLib.session.findById("wnd[0]/usr/tabsTABSTRIP1/tabpTAB1/ssubHEADER_TAB:SAPLJ1BB2:2100/tblSAPLJ1BB2ITEM_CONTROL/ctxtJ_1BDYLIN-CFOP[9,0]").Text = miro["sintese"]["CFOP"]  #CFOP  TODO (Definimos no Form mais um input do fornecedor?)
+
+        sapGuiLib.session.findById("wnd[0]").sendVKey(0)
 
         sapGuiLib.session.findById("wnd[0]/tbar[0]/btn[3]").press()  #Voltar
         sapGuiLib.session.findById("wnd[0]/tbar[0]/btn[11]").press()  #Gravar
         sbar = sapGuiLib.session.findById("wnd[0]/sbar").Text
         documento = None
         for patter in [MSG_SAP_CODIGO_DOCUMENTO, MSG_MIRO_SEM_ESTRAGIA_DE_APROVACAO]: 
             documento = sbar_extracted_text(patter, sbar)
```

### Comparing `hnt_sap_service_library-0.0.1/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py` & `hnt_sap_service_library-0.0.2/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,91 +6,101 @@
 MSG_SAP_CODIGO_NOTA_PEDIDO = "^Ped.C.Custo\\/Ordem criado sob o nº ([0-9]{10,11})$"
 class NotaPedidoTransaction:
     def __init__(self) -> None:
         pass
 
     def execute(self, sapGuiLib, nota_pedido):
         logger.info(f"enter execute nota_pedido:{nota_pedido}")
+        # ABRE TRANSAÇÃO
         sapGuiLib.run_transaction('/nme21n')
-
         sapGuiLib.send_vkey(0)
 
         # REORGANIZA ELEMENTOS PARA GARANTIR QUE CABEÇALHO ESTEJA ABERTO
         sapGuiLib.send_vkey(29) # Fechar Cabeçalho
         sapGuiLib.send_vkey(30) # Fechar Síntese de itens
         sapGuiLib.send_vkey(31) # Fechar Detahe de item
         sapGuiLib.send_vkey(26) # Abrir Cabeçalho
 
         # PREENCHE DADOS INICIAIS (Antes do cabeçalho)
         sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB0:SAPLMEGUI:0030/subSUB1:SAPLMEGUI:1105/cmbMEPO_TOPLINE-BSART").Key = nota_pedido['tipo'] # Define o tipo de pedido como Ped.C.Custo/Ordem
-        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB0:SAPLMEGUI:0030/subSUB1:SAPLMEGUI:1105/ctxtMEPO_TOPLINE-SUPERFIELD").Text = nota_pedido['cod_fornecedor'] # Fornecedor
+        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB0:SAPLMEGUI:0030/subSUB1:SAPLMEGUI:1105/ctxtMEPO_TOPLINE-SUPERFIELD").Text = nota_pedido['cod_fornecedor']
 
         # CABEÇALHO | Aba Dados Organizacionais
         sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB1:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1102/tabsHEADER_DETAIL/tabpTABHDT9").Select() #Seleciona a aba Dados organizacionais
-        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB1:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1102/tabsHEADER_DETAIL/tabpTABHDT9/ssubTABSTRIPCONTROL2SUB:SAPLMEGUI:1221/ctxtMEPO1222-EKORG").Text = nota_pedido['org_compras'] #orgCompras
-        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB1:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1102/tabsHEADER_DETAIL/tabpTABHDT9/ssubTABSTRIPCONTROL2SUB:SAPLMEGUI:1221/ctxtMEPO1222-EKGRP").Text = nota_pedido['grp_compradores'] #grpCompradores '(Constante: S01)
-        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB1:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1102/tabsHEADER_DETAIL/tabpTABHDT9/ssubTABSTRIPCONTROL2SUB:SAPLMEGUI:1221/ctxtMEPO1222-BUKRS").Text = nota_pedido['empresa'] #empresa '(Constante: HFNT)
-        # Application.Wait Now + #12:00:02 AM# '(Avaliar a necessidade de inserir espera)
+        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB1:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1102/tabsHEADER_DETAIL/tabpTABHDT9/ssubTABSTRIPCONTROL2SUB:SAPLMEGUI:1221/ctxtMEPO1222-EKORG").Text = nota_pedido['org_compras']  # (orgCompras)
+        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB1:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1102/tabsHEADER_DETAIL/tabpTABHDT9/ssubTABSTRIPCONTROL2SUB:SAPLMEGUI:1221/ctxtMEPO1222-EKGRP").Text = nota_pedido['grp_compradores'] # grpCompradores)
+        sapGuiLib.session.findById("wnd[0]/usr/subSUB0:SAPLMEGUI:0013/subSUB1:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1102/tabsHEADER_DETAIL/tabpTABHDT9/ssubTABSTRIPCONTROL2SUB:SAPLMEGUI:1221/ctxtMEPO1222-BUKRS").Text = nota_pedido['empresa']  # (Empresa)
 
         # REORGANIZA ELEMENTOS PARA GARANTIR QUE SÍNTESE DE ITENS ESTEJA ABERTO
         sapGuiLib.send_vkey(29) #Fechar cabeçalho
         sapGuiLib.send_vkey(27) #Abrir Síntese de itens
         sapGuiLib.send_vkey(31) #Fechar Detahe de item
         sapGuiLib.send_vkey(26) #Abrir Cabeçalho
         sapGuiLib.send_vkey(29) #Fechar cabeçalho
 
 
         # SÍNTESE DE ITENS
-        for i, sintese_de_iten in enumerate(nota_pedido['sintese_itens']):
-            id_0015 = "wnd[0]/usr/subSUB0:SAPLMEGUI:0015"
-            id_0016 = "wnd[0]/usr/subSUB0:SAPLMEGUI:0016"
-            id_0019 = "wnd[0]/usr/subSUB0:SAPLMEGUI:0019"
-            id_gui = id_0016 if sapGuiLib.session.findById(id_0016, False) != None else id_0019
-            
-            sapGuiLib.session.findById(f"{id_gui}/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/ctxtMEPO1211-KNTTP[2,{i}]").Text = sintese_de_iten['categoria_cc'] #categoriaCC '(Constante: K)
-            sapGuiLib.session.findById(f"{id_gui}/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/ctxtMEPO1211-EMATN[4,{i}]").Text = sintese_de_iten['cod_material']  # material
-            sapGuiLib.session.findById(f"{id_gui}/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/txtMEPO1211-MENGE[6,{i}]").Text = sintese_de_iten['quantidade'] #quantidade
-            sapGuiLib.session.findById(f"{id_gui}/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/ctxtMEPO1211-NAME1[10,{i}]").Text = sintese_de_iten['item']['centro'] #centro 'Local de negócio
-            sapGuiLib.send_vkey(0)
+        for index, sintese_item in enumerate(nota_pedido['sintese_itens']):
 
-            # DETALHES DE ITEM | Aba Fatura
-            id_gui_detalhes_item = id_0015 if sapGuiLib.session.findById(id_0015, False) != None else id_0019
-            if sapGuiLib.session.findById(f"{id_gui_detalhes_item}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT7", False) != None:
-                sapGuiLib.session.findById(f"{id_gui_detalhes_item}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT7").Select() #Seleciona a aba fatura
-            
-            id_gui_detalhes_item = id_0015 if sapGuiLib.session.findById(id_0015, False) != None else id_0019
-            sapGuiLib.session.findById(f"{id_gui_detalhes_item}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT7/ssubTABSTRIPCONTROL1SUB:SAPLMEGUI:1317/ctxtMEPO1317-MWSKZ").Text = sintese_de_iten['item']['cod_imposto'] #codigoImposto #Inclui o código do imposto
-            sapGuiLib.send_vkey(0)
+            item = sintese_item['item']
+            fatura = sintese_item['fatura']
 
-            # DETALHES DE ITEM | Aba C|C
-            id_gui_detalhes_item = id_0015 if sapGuiLib.session.findById(id_0015, False) != None else id_0019
-            if sapGuiLib.session.findById(f"{id_gui_detalhes_item}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT13", False) != None:
-                sapGuiLib.session.findById(f"{id_gui_detalhes_item}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT13").Select() #Seleciona a aba C|C
+            id_0015  = "wnd[0]/usr/subSUB0:SAPLMEGUI:0015"
+            id_0016  = "wnd[0]/usr/subSUB0:SAPLMEGUI:0016"
+            id_0019  = "wnd[0]/usr/subSUB0:SAPLMEGUI:0019"
 
-            id_gui_detalhes_item = id_0015 if sapGuiLib.session.findById(id_0015, False) != None else id_0019
-            sapGuiLib.session.findById(f"{id_gui_detalhes_item}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT13/ssubTABSTRIPCONTROL1SUB:SAPLMEVIEWS:1101/subSUB2:SAPLMEACCTVI:0100/subSUB1:SAPLMEACCTVI:1100/subKONTBLOCK:SAPLKACB:1101/ctxtCOBL-KOSTL").Text = sintese_de_iten['item']['centro_custo'] #centroCusto
-            sapGuiLib.send_vkey(0)
+            check_id_sintese  = sapGuiLib.session.findById(id_0016, False) != None
+            id_gui_sintese    = id_0016 if check_id_sintese else id_0019
+
+            check_id_detalhes = sapGuiLib.session.findById(id_0015, False) != None
+            id_gui_detalhes   = id_0015 if check_id_detalhes else id_0019
+
+            sapGuiLib.session.findById(f"{id_gui_sintese}/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/ctxtMEPO1211-KNTTP[2,{index}]").Text = sintese_item['categoria_cc']  # (Categoria C|C)
+            sapGuiLib.session.findById(f"{id_gui_sintese}/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/ctxtMEPO1211-EPSTP[3,{index}]").Text = sintese_item['categoria_item']  # (Categoria do item)
+            sapGuiLib.session.findById(f"{id_gui_sintese}/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/txtMEPO1211-TXZ01[5,{index}]").Text = sintese_item['texto_breve']  # (Texto breve)
+            sapGuiLib.session.findById(f"{id_gui_sintese}/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/txtMEPO1211-MENGE[6,{index}]").Text = sintese_item['quantidade']  # (Qtd.do pedido)
+            sapGuiLib.session.findById(f"{id_gui_sintese}/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/ctxtMEPO1211-NAME1[10,{index}]").Text = sintese_item['centro']  # (Centro)
+            sapGuiLib.session.findById(f"{id_gui_sintese}/subSUB2:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1211/tblSAPLMEGUITC_1211/ctxtMEPO1211-WGBEZ[19,{index}]").Text = sintese_item['grp_mercadorias']  # (Grupo de mercadorias)
             sapGuiLib.send_vkey(0)
+
+            # DETALHES DE ITEM | Aba Serviços
+            check_id_detalhes = sapGuiLib.session.findById(id_0015, False) != None
+            id_gui_detalhes   = id_0015 if check_id_detalhes else id_0019
+            # id_gui_detalhes   = id_0015
+
+            if sapGuiLib.session.findById(f"{id_gui_detalhes}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT1", False) != None:  
+                # Seleciona aba "Serviços"
+                sapGuiLib.session.findById(f"{id_gui_detalhes}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT1").select()
+
+            sapGuiLib.session.findById(f"{id_gui_detalhes}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT1/ssubTABSTRIPCONTROL1SUB:SAPLMEGUI:1328/subSUB0:SAPLMLSP:0400/tblSAPLMLSPTC_VIEW/ctxtESLL-SRVPOS[2,{index}]").Text = item['nro_servico'] # (Nº serviço)
+            sapGuiLib.session.findById(f"{id_gui_detalhes}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT1/ssubTABSTRIPCONTROL1SUB:SAPLMEGUI:1328/subSUB0:SAPLMLSP:0400/tblSAPLMLSPTC_VIEW/ctxtRM11P-KOSTL[3,{index}]").Text = item['centro_custo']  # (Centro custo)
+            sapGuiLib.session.findById(f"{id_gui_detalhes}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT1/ssubTABSTRIPCONTROL1SUB:SAPLMEGUI:1328/subSUB0:SAPLMLSP:0400/tblSAPLMLSPTC_VIEW/txtESLL-MENGE[4,{index}]").Text = item['quantidade']  # (Quantidade)
+            sapGuiLib.session.findById(f"{id_gui_detalhes}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT1/ssubTABSTRIPCONTROL1SUB:SAPLMEGUI:1328/subSUB0:SAPLMLSP:0400/tblSAPLMLSPTC_VIEW/txtESLL-TBTWR[5,{index}]").Text = item['valor_bruto'] # (Preço bruto)
             sapGuiLib.send_vkey(0)
-            id_gui_detalhes_item = id_0015 if sapGuiLib.session.findById(id_0015, False) != None else id_0019
-            # DETALHES DE ITEM | Aba Condições
-            if sapGuiLib.session.findById(f"{id_gui_detalhes_item}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT8", False) != None:
-                sapGuiLib.session.findById(f"{id_gui_detalhes_item}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT8").Select() #Seleciona a aba Condições
-            sapGuiLib.session.findById(f"{id_gui_detalhes_item}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT8/ssubTABSTRIPCONTROL1SUB:SAPLMEGUI:1333/ssubSUB0:SAPLV69A:6201/tblSAPLV69ATCTRL_KONDITIONEN/txtKOMV-KBETR[3,1]").Text = sapGuiLib.format_float(sintese_de_iten['item']['montante']) #valorItem 'Valor bruto
+
+            check_id_detalhes = sapGuiLib.session.findById(id_0015, False) != None
+            id_gui_detalhes   = id_0015 if check_id_detalhes else id_0019
+
+            # DETALHES DE ITEM | Aba Fatura
+            if sapGuiLib.session.findById(f"{id_gui_detalhes}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT7", False) != None:
+                sapGuiLib.session.findById(f"{id_gui_detalhes}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT7").Select() #Seleciona a aba "Fatura"
+
+            sapGuiLib.session.findById(f"{id_gui_detalhes}/subSUB3:SAPLMEVIEWS:1100/subSUB2:SAPLMEVIEWS:1200/subSUB1:SAPLMEGUI:1301/subSUB2:SAPLMEGUI:1303/tabsITEM_DETAIL/tabpTABIDT7/ssubTABSTRIPCONTROL1SUB:SAPLMEGUI:1317/ctxtMEPO1317-MWSKZ").Text = fatura['cod_imposto']  # (Cód.imposto)
             sapGuiLib.send_vkey(0)
 
+
         # PROCESSO PARA ANEXAR O DOCUMENTO NO PEDIDO
         for anexo in nota_pedido['anexo']:
             sapGuiLib.session.findById("wnd[0]/titl/shellcont/shell").pressButton("%GOS_TOOLBOX")
             sapGuiLib.session.findById("wnd[0]/shellcont[1]/shell").pressContextButton("CREATE_ATTA")
             sapGuiLib.session.findById("wnd[0]/shellcont[1]/shell").selectContextMenuItem("PCATTA_CREA")
             sapGuiLib.session.findById("wnd[1]/usr/ctxtDY_PATH").Text = anexo['path'] #Diretório de NFs
             sapGuiLib.session.findById("wnd[1]/usr/ctxtDY_FILENAME").Text = anexo['filename'] #PDF da DANFE
             sapGuiLib.session.findById("wnd[1]/tbar[0]/btn[0]").press()
 
-        sapGuiLib.session.findById("wnd[0]/tbar[0]/btn[11]").press() #'Grava o lançamento
-        sbar = sapGuiLib.session.findById("wnd[0]/sbar").Text
+        sapGuiLib.session.findById("wnd[0]/tbar[0]/btn[11]").press() # Grava o lançamento
+        sbar = sapGuiLib.session.findById("wnd[0]/sbar").Text # Captura do nº do documento exibido na barra de status do SAP (últimos 10 caracteres da mensagem)
         cod_nota_pedido = sbar_extracted_text(MSG_SAP_CODIGO_NOTA_PEDIDO, sbar)
         tx_result = TxResult(cod_nota_pedido, sbar)
-        logger.info(f"Leave execute código da nota_pedido:{str(tx_result)}")
+        logger.info(f"Leave execute code service_note:{str(tx_result)}")
 
-        return tx_result
+        return tx_result
```

### Comparing `hnt_sap_service_library-0.0.1/hnt_sap_service_library.egg-info/SOURCES.txt` & `hnt_sap_service_library-0.0.2/hnt_sap_service_library.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,10 +13,9 @@
 hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py
 hnt_sap_service_library.egg-info/PKG-INFO
 hnt_sap_service_library.egg-info/SOURCES.txt
 hnt_sap_service_library.egg-info/dependency_links.txt
 hnt_sap_service_library.egg-info/requires.txt
 hnt_sap_service_library.egg-info/top_level.txt
 tests/test_fatura.py
-tests/test_liberacao.py
 tests/test_miro.py
 tests/test_nota_pedido.py
```

