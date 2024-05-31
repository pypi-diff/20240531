# Comparing `tmp/odoo_addons_oca_stock_logistics_workflow-16.0.20240529.1-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_stock_logistics_workflow-16.0.20240530.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2235 bytes, number of entries: 4
--rw-r--r--  2.0 unx     6061 b- defN 24-May-30 06:32 odoo_addons_oca_stock_logistics_workflow-16.0.20240529.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-30 06:32 odoo_addons_oca_stock_logistics_workflow-16.0.20240529.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-May-30 06:32 odoo_addons_oca_stock_logistics_workflow-16.0.20240529.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      469 b- defN 24-May-30 06:32 odoo_addons_oca_stock_logistics_workflow-16.0.20240529.1.dist-info/RECORD
-4 files, 6623 bytes uncompressed, 1309 bytes compressed:  80.2%
+Zip file size: 2262 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     6215 b- defN 24-May-31 06:52 odoo_addons_oca_stock_logistics_workflow-16.0.20240530.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-31 06:52 odoo_addons_oca_stock_logistics_workflow-16.0.20240530.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-31 06:52 odoo_addons_oca_stock_logistics_workflow-16.0.20240530.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      469 b- defN 24-May-31 06:52 odoo_addons_oca_stock_logistics_workflow-16.0.20240530.0.dist-info/RECORD
+4 files, 6777 bytes uncompressed, 1336 bytes compressed:  80.3%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240529.1.dist-info/METADATA
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240530.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240529.1.dist-info/WHEEL
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240530.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240529.1.dist-info/top_level.txt
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240530.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240529.1.dist-info/RECORD
+Filename: odoo_addons_oca_stock_logistics_workflow-16.0.20240530.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_stock_logistics_workflow-16.0.20240529.1.dist-info/METADATA` & `odoo_addons_oca_stock_logistics_workflow-16.0.20240530.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-stock-logistics-workflow
-Version: 16.0.20240529.1
+Version: 16.0.20240530.0
 Summary: Meta package for oca-stock-logistics-workflow Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-delivery-procurement-group-carrier <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-delivery-total-weight-from-packaging <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-stock-picking-invoice-link <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-line-returned-qty <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-order-global-stock-route <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-stock-restocking-fee-invoicing <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-stock-account-product-run-fifo-hook <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-auto-move <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-customer-deposit <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-customer-deposit-elaboration <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-customer-deposit-sale-margin <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-delivery-note <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-grn <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-landed-costs-currency <16.1dev,>=16.0dev
@@ -81,10 +82,11 @@
 Requires-Dist: odoo-addon-stock-quant-package-dimension <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-quant-package-dimension-total-weight-from-packaging <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-quant-package-product-packaging <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-receipt-lot-info <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-restrict-lot <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-rule-reserve-max-quantity <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-stock-split-picking <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-stock-valuation-layer-usage <16.1dev,>=16.0dev
 
 UNKNOWN
```

