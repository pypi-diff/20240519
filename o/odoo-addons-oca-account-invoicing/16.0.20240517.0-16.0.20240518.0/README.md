# Comparing `tmp/odoo_addons_oca_account_invoicing-16.0.20240517.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_account_invoicing-16.0.20240518.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
 Zip file size: 1975 bytes, number of entries: 4
--rw-r--r--  2.0 unx     4598 b- defN 24-May-18 02:58 odoo_addons_oca_account_invoicing-16.0.20240517.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-18 02:58 odoo_addons_oca_account_invoicing-16.0.20240517.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-May-18 02:58 odoo_addons_oca_account_invoicing-16.0.20240517.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      441 b- defN 24-May-18 02:58 odoo_addons_oca_account_invoicing-16.0.20240517.0.dist-info/RECORD
-4 files, 5132 bytes uncompressed, 1105 bytes compressed:  78.5%
+-rw-r--r--  2.0 unx     4672 b- defN 24-May-19 03:03 odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-19 03:03 odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-19 03:03 odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      441 b- defN 24-May-19 03:03 odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/RECORD
+4 files, 5206 bytes uncompressed, 1105 bytes compressed:  78.8%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_account_invoicing-16.0.20240517.0.dist-info/METADATA
+Filename: odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20240517.0.dist-info/WHEEL
+Filename: odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20240517.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_account_invoicing-16.0.20240517.0.dist-info/RECORD
+Filename: odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_account_invoicing-16.0.20240517.0.dist-info/METADATA` & `odoo_addons_oca_account_invoicing-16.0.20240518.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-account-invoicing
-Version: 16.0.20240517.0
+Version: 16.0.20240518.0
 Summary: Meta package for oca-account-invoicing Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -47,14 +47,15 @@
 Requires-Dist: odoo-addon-account-move-substate <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-move-tier-validation <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-receipt-journal <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-receipt-send <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-tax-change <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-tax-group-widget-base-amount <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-account-tax-one-vat <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-account-tax-one-vat-purchase <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-invoicing-mode <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-invoicing-mode-at-shipping <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-partner-invoicing-mode-monthly <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-portal-account-personal-data-only <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-product-form-account-move-line-link <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-invoicing-no-zero-line <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-purchase-stock-picking-return-invoicing <16.1dev,>=16.0dev
```

