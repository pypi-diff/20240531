# Comparing `tmp/odoo_addons_oca_partner_contact-16.0.20240313.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_partner_contact-16.0.20240506.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1989 bytes, number of entries: 4
--rw-r--r--  2.0 unx     5017 b- defN 24-Mar-14 05:35 odoo_addons_oca_partner_contact-16.0.20240313.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-14 05:35 odoo_addons_oca_partner_contact-16.0.20240313.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-14 05:35 odoo_addons_oca_partner_contact-16.0.20240313.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      433 b- defN 24-Mar-14 05:35 odoo_addons_oca_partner_contact-16.0.20240313.0.dist-info/RECORD
-4 files, 5543 bytes uncompressed, 1135 bytes compressed:  79.5%
+Zip file size: 1992 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     5023 b- defN 24-May-07 05:46 odoo_addons_oca_partner_contact-16.0.20240506.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-07 05:46 odoo_addons_oca_partner_contact-16.0.20240506.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-07 05:46 odoo_addons_oca_partner_contact-16.0.20240506.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      433 b- defN 24-May-07 05:46 odoo_addons_oca_partner_contact-16.0.20240506.0.dist-info/RECORD
+4 files, 5549 bytes uncompressed, 1138 bytes compressed:  79.5%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_partner_contact-16.0.20240313.0.dist-info/METADATA
+Filename: odoo_addons_oca_partner_contact-16.0.20240506.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_partner_contact-16.0.20240313.0.dist-info/WHEEL
+Filename: odoo_addons_oca_partner_contact-16.0.20240506.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_partner_contact-16.0.20240313.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_partner_contact-16.0.20240506.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_partner_contact-16.0.20240313.0.dist-info/RECORD
+Filename: odoo_addons_oca_partner_contact-16.0.20240506.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_partner_contact-16.0.20240313.0.dist-info/METADATA` & `odoo_addons_oca_partner_contact-16.0.20240506.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-partner-contact
-Version: 16.0.20240313.0
+Version: 16.0.20240506.0
 Summary: Meta package for oca-partner-contact Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -14,15 +14,14 @@
 Requires-Dist: odoo-addon-base-location-geonames-import <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-partner-company-group <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-base-partner-sequence <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-crm-partner-company-group <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-accreditation <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-address-split <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-address-street3 <16.1dev,>=16.0dev
-Requires-Dist: odoo-addon-partner-address-two-lines <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-affiliate <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-auto-archive <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-bank-acc-type-constraint <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-bank-code <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-capital <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-category-security <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-category-security-crm <16.1dev,>=16.0dev
@@ -42,14 +41,15 @@
 Requires-Dist: odoo-addon-partner-contact-personal-information-page <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-contact-type-end-user <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-country-state-required <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-deduplicate-acl <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-deduplicate-by-ref <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-deduplicate-filter <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-disable-gravatar <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-partner-display-name-line-break <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-email-check <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-email-duplicate-warn <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-employee-quantity <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-external-map <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-fax <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-firstname <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-identification <16.1dev,>=16.0dev
```

