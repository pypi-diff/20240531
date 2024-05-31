# Comparing `tmp/hnt_sap_service_library-0.0.3.tar.gz` & `tmp/hnt_sap_service_library-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnt_sap_service_library-0.0.3.tar", last modified: Fri May 31 17:36:31 2024, max compression
+gzip compressed data, was "hnt_sap_service_library-0.0.4.tar", last modified: Fri May 31 19:38:06 2024, max compression
```

## Comparing `hnt_sap_service_library-0.0.3.tar` & `hnt_sap_service_library-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 17:36:31.499409 hnt_sap_service_library-0.0.3/
--rw-rw-rw-   0        0        0      288 2024-05-31 17:36:31.499409 hnt_sap_service_library-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2248 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 17:36:31.427006 hnt_sap_service_library-0.0.3/hnt_sap_gui/
--rw-rw-rw-   0        0        0       54 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/RPA_HNT_Constants.py
--rw-rw-rw-   0        0        0       22 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 17:36:31.432862 hnt_sap_service_library-0.0.3/hnt_sap_gui/common/
--rw-rw-rw-   0        0        0      368 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/common/sap_status_bar.py
--rw-rw-rw-   0        0        0     2585 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/common/session.py
--rw-rw-rw-   0        0        0      370 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/common/tx_result.py
--rw-rw-rw-   0        0        0     4268 2024-05-31 17:32:49.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/hnt_sap.py
--rw-rw-rw-   0        0        0      388 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/hnt_sap_exception.py
-drwxrwxrwx   0        0        0        0 2024-05-31 17:36:31.447049 hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/
--rw-rw-rw-   0        0        0     4257 2024-05-31 14:58:51.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/fatura_transaction.py
--rw-rw-rw-   0        0        0     1018 2024-05-31 12:52:15.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/liberacao_transaction.py
--rw-rw-rw-   0        0        0     6291 2024-05-31 12:53:24.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/miro_transaction.py
--rw-rw-rw-   0        0        0     9211 2024-05-31 15:05:23.000000 hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py
-drwxrwxrwx   0        0        0        0 2024-05-31 17:36:31.496988 hnt_sap_service_library-0.0.3/hnt_sap_service_library.egg-info/
--rw-rw-rw-   0        0        0      288 2024-05-31 17:36:31.000000 hnt_sap_service_library-0.0.3/hnt_sap_service_library.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      720 2024-05-31 17:36:31.000000 hnt_sap_service_library-0.0.3/hnt_sap_service_library.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 17:36:31.000000 hnt_sap_service_library-0.0.3/hnt_sap_service_library.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-05-31 17:36:31.000000 hnt_sap_service_library-0.0.3/hnt_sap_service_library.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-31 17:36:31.000000 hnt_sap_service_library-0.0.3/hnt_sap_service_library.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 17:36:31.499409 hnt_sap_service_library-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      472 2024-05-31 17:34:22.000000 hnt_sap_service_library-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 17:36:31.494406 hnt_sap_service_library-0.0.3/tests/
--rw-rw-rw-   0        0        0      413 2024-05-31 14:58:51.000000 hnt_sap_service_library-0.0.3/tests/test_fatura.py
--rw-rw-rw-   0        0        0      378 2024-05-31 12:53:30.000000 hnt_sap_service_library-0.0.3/tests/test_miro.py
--rw-rw-rw-   0        0        0     1144 2024-05-31 15:03:58.000000 hnt_sap_service_library-0.0.3/tests/test_nota_pedido.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:38:06.272155 hnt_sap_service_library-0.0.4/
+-rw-rw-rw-   0        0        0      288 2024-05-31 19:38:06.269155 hnt_sap_service_library-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2248 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 19:38:06.125748 hnt_sap_service_library-0.0.4/hnt_sap_gui/
+-rw-rw-rw-   0        0        0       54 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.4/hnt_sap_gui/RPA_HNT_Constants.py
+-rw-rw-rw-   0        0        0       22 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.4/hnt_sap_gui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:38:06.160992 hnt_sap_service_library-0.0.4/hnt_sap_gui/common/
+-rw-rw-rw-   0        0        0      368 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.4/hnt_sap_gui/common/sap_status_bar.py
+-rw-rw-rw-   0        0        0     2585 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.4/hnt_sap_gui/common/session.py
+-rw-rw-rw-   0        0        0      370 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.4/hnt_sap_gui/common/tx_result.py
+-rw-rw-rw-   0        0        0     4285 2024-05-31 19:03:47.000000 hnt_sap_service_library-0.0.4/hnt_sap_gui/hnt_sap.py
+-rw-rw-rw-   0        0        0      388 2024-05-22 12:00:21.000000 hnt_sap_service_library-0.0.4/hnt_sap_gui/hnt_sap_exception.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:38:06.207150 hnt_sap_service_library-0.0.4/hnt_sap_gui/nota_fiscal/
+-rw-rw-rw-   0        0        0     4260 2024-05-31 19:12:07.000000 hnt_sap_service_library-0.0.4/hnt_sap_gui/nota_fiscal/fatura_transaction.py
+-rw-rw-rw-   0        0        0     1018 2024-05-31 12:52:15.000000 hnt_sap_service_library-0.0.4/hnt_sap_gui/nota_fiscal/liberacao_transaction.py
+-rw-rw-rw-   0        0        0     6291 2024-05-31 12:53:24.000000 hnt_sap_service_library-0.0.4/hnt_sap_gui/nota_fiscal/miro_transaction.py
+-rw-rw-rw-   0        0        0     9211 2024-05-31 15:05:23.000000 hnt_sap_service_library-0.0.4/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:38:06.266156 hnt_sap_service_library-0.0.4/hnt_sap_service_library.egg-info/
+-rw-rw-rw-   0        0        0      288 2024-05-31 19:38:05.000000 hnt_sap_service_library-0.0.4/hnt_sap_service_library.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      720 2024-05-31 19:38:05.000000 hnt_sap_service_library-0.0.4/hnt_sap_service_library.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 19:38:05.000000 hnt_sap_service_library-0.0.4/hnt_sap_service_library.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-05-31 19:38:05.000000 hnt_sap_service_library-0.0.4/hnt_sap_service_library.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-31 19:38:05.000000 hnt_sap_service_library-0.0.4/hnt_sap_service_library.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 19:38:06.273157 hnt_sap_service_library-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      472 2024-05-31 19:38:01.000000 hnt_sap_service_library-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 19:38:06.262156 hnt_sap_service_library-0.0.4/tests/
+-rw-rw-rw-   0        0        0      426 2024-05-31 19:02:06.000000 hnt_sap_service_library-0.0.4/tests/test_fatura.py
+-rw-rw-rw-   0        0        0      378 2024-05-31 12:53:30.000000 hnt_sap_service_library-0.0.4/tests/test_miro.py
+-rw-rw-rw-   0        0        0     1144 2024-05-31 15:03:58.000000 hnt_sap_service_library-0.0.4/tests/test_nota_pedido.py
```

### Comparing `hnt_sap_service_library-0.0.3/README.md` & `hnt_sap_service_library-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.3/hnt_sap_gui/common/session.py` & `hnt_sap_service_library-0.0.4/hnt_sap_gui/common/session.py`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.3/hnt_sap_gui/hnt_sap.py` & `hnt_sap_service_library-0.0.4/hnt_sap_gui/hnt_sap.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     @sessionable
     def hnt_run_transaction_FV60(self, data):
         results = {
             "fatura": None,
             "error": None
         }
         try:
-            results["fatura"] = FaturaTransaction().execute(self, data)
+            results["fatura"] = FaturaTransaction().execute(self, fatura=data["fatura"])
         except Exception as ex:
             logger.error(str(ex))
             results["error"] = str(ex)
         logger.info(f"leave execute run_hnt_transactions result:{', '.join([str(results[obj]) for obj in results])}")
         return results
 
     @sessionable
```

### Comparing `hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/fatura_transaction.py` & `hnt_sap_service_library-0.0.4/hnt_sap_gui/nota_fiscal/fatura_transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,33 +19,33 @@
             sapGuiLib.session.findById("wnd[1]/tbar[0]/btn[0]").press()
 
         # ABA DADOS BÁSICOS
         sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpMAIN/ssubPAGE:SAPLFDCB:0010/ctxtINVFO-ACCNT").Text = fatura['dados_basicos']['cod_fornecedor']
         sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpMAIN/ssubPAGE:SAPLFDCB:0010/ctxtINVFO-BLDAT").Text = fatura['dados_basicos']['data_fatura']
         sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpMAIN/ssubPAGE:SAPLFDCB:0010/txtINVFO-XBLNR").Text = fatura['dados_basicos']['referencia']
         sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpMAIN/ssubPAGE:SAPLFDCB:0010/txtINVFO-WRBTR").Text = sapGuiLib.format_float(fatura['dados_basicos']['montante'])
-        sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpMAIN/ssubPAGE:SAPLFDCB:0010/ctxtINVFO-BUPLA").Text = fatura['dados_basicos']['loc_negocios'] ## 'Loc.negócios Domains.centro.centro_loja
+        sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpMAIN/ssubPAGE:SAPLFDCB:0010/ctxtINVFO-BUPLA").Text = fatura['dados_basicos']['bus_pl_sec_cd'] ## 'Loc.negócios Domains.centro.centro_loja
         sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpMAIN/ssubPAGE:SAPLFDCB:0010/ctxtINVFO-SGTXT").Text = fatura['dados_basicos']['texto']
         sapGuiLib.send_vkey(0)
         status = sapGuiLib.session.findById("wnd[0]/sbar").Text
         if sbar_extracted_text(MSG_SAP_JA_FOI_CRIADO, status) != None:
             raise HntSapException(status)
-        for i, iten in enumerate(fatura['dados_basicos']['itens']):
-            sapGuiLib.session.findById(f"wnd[0]/usr/subITEMS:SAPLFSKB:0100/tblSAPLFSKBTABLE/ctxtACGL_ITEM-HKONT[1,{i}]").Text = iten['cta_razao']
-            sapGuiLib.session.findById(f"wnd[0]/usr/subITEMS:SAPLFSKB:0100/tblSAPLFSKBTABLE/txtACGL_ITEM-WRBTR[4,{i}]").Text = sapGuiLib.format_float(iten['montante'])
-            sapGuiLib.session.findById(f"wnd[0]/usr/subITEMS:SAPLFSKB:0100/tblSAPLFSKBTABLE/ctxtACGL_ITEM-BUPLA[6,{i}]").Text = iten['loc_negocios']
-            sapGuiLib.session.findById(f"wnd[0]/usr/subITEMS:SAPLFSKB:0100/tblSAPLFSKBTABLE/txtACGL_ITEM-ZUONR[10,{i}]").Text = iten['atribuicao']
-            sapGuiLib.session.findById(f"wnd[0]/usr/subITEMS:SAPLFSKB:0100/tblSAPLFSKBTABLE/ctxtACGL_ITEM-SGTXT[12,{i}]").Text = iten['texto']
-            sapGuiLib.session.findById(f"wnd[0]/usr/subITEMS:SAPLFSKB:0100/tblSAPLFSKBTABLE/ctxtACGL_ITEM-KOSTL[18,{i}]").Text = iten['centro_custo']
+        for i, item in enumerate(fatura['dados_basicos']['itens']):
+            sapGuiLib.session.findById(f"wnd[0]/usr/subITEMS:SAPLFSKB:0100/tblSAPLFSKBTABLE/ctxtACGL_ITEM-HKONT[1,{i}]").Text = item['cta_razao']
+            sapGuiLib.session.findById(f"wnd[0]/usr/subITEMS:SAPLFSKB:0100/tblSAPLFSKBTABLE/txtACGL_ITEM-WRBTR[4,{i}]").Text = sapGuiLib.format_float(item['montante'])
+            sapGuiLib.session.findById(f"wnd[0]/usr/subITEMS:SAPLFSKB:0100/tblSAPLFSKBTABLE/ctxtACGL_ITEM-BUPLA[6,{i}]").Text = item['loc_negocios']
+            sapGuiLib.session.findById(f"wnd[0]/usr/subITEMS:SAPLFSKB:0100/tblSAPLFSKBTABLE/txtACGL_ITEM-ZUONR[10,{i}]").Text = item['atribuicao']
+            sapGuiLib.session.findById(f"wnd[0]/usr/subITEMS:SAPLFSKB:0100/tblSAPLFSKBTABLE/ctxtACGL_ITEM-SGTXT[12,{i}]").Text = item['texto']
+            sapGuiLib.session.findById(f"wnd[0]/usr/subITEMS:SAPLFSKB:0100/tblSAPLFSKBTABLE/ctxtACGL_ITEM-KOSTL[18,{i}]").Text = item['centro_custo']
 
         sapGuiLib.send_vkey(0)
         # ABA DADOS PAGAMENTO
         sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpPAYM").Select()
         sapGuiLib.send_vkey(0)
-        sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpPAYM/ssubPAGE:SAPLFDCB:0020/cmbINVFO-ZLSPR").Key = ""
+        # sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpPAYM/ssubPAGE:SAPLFDCB:0020/cmbINVFO-ZLSPR").Key = ""
         sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpPAYM/ssubPAGE:SAPLFDCB:0020/ctxtINVFO-ZFBDT").Text = fatura['pagamento']['data_basica']
         sapGuiLib.session.findById("wnd[0]/usr/tabsTS/tabpPAYM/ssubPAGE:SAPLFDCB:0020/ctxtINVFO-ZTERM").Text = fatura['pagamento']['cond_pgto']
         sapGuiLib.send_vkey(0)
         sapGuiLib.send_vkey(0)
         sbar = sapGuiLib.session.findById("wnd[0]/sbar").Text
         if MSG_SAP_COND_PGTO_MODIFICADAS == sbar:
             sapGuiLib.send_vkey(0)
```

### Comparing `hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/liberacao_transaction.py` & `hnt_sap_service_library-0.0.4/hnt_sap_gui/nota_fiscal/liberacao_transaction.py`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/miro_transaction.py` & `hnt_sap_service_library-0.0.4/hnt_sap_gui/nota_fiscal/miro_transaction.py`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.3/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py` & `hnt_sap_service_library-0.0.4/hnt_sap_gui/nota_fiscal/nota_pedido_transaction.py`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.3/hnt_sap_service_library.egg-info/SOURCES.txt` & `hnt_sap_service_library-0.0.4/hnt_sap_service_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hnt_sap_service_library-0.0.3/tests/test_nota_pedido.py` & `hnt_sap_service_library-0.0.4/tests/test_nota_pedido.py`

 * *Files identical despite different names*

