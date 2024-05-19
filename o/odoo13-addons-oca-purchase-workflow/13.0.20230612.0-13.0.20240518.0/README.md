# Comparing `tmp/odoo13_addons_oca_purchase_workflow-13.0.20230612.0-py3-none-any.whl.zip` & `tmp/odoo13_addons_oca_purchase_workflow-13.0.20240518.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2116 bytes, number of entries: 4
--rw-r--r--  2.0 unx     4727 b- defN 23-Jun-13 05:01 odoo13_addons_oca_purchase_workflow-13.0.20230612.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 05:01 odoo13_addons_oca_purchase_workflow-13.0.20230612.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-13 05:01 odoo13_addons_oca_purchase_workflow-13.0.20230612.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      449 b- defN 23-Jun-13 05:01 odoo13_addons_oca_purchase_workflow-13.0.20230612.0.dist-info/RECORD
-4 files, 5269 bytes uncompressed, 1230 bytes compressed:  76.7%
+Zip file size: 2150 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     4886 b- defN 24-May-19 06:28 odoo13_addons_oca_purchase_workflow-13.0.20240518.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-19 06:28 odoo13_addons_oca_purchase_workflow-13.0.20240518.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-19 06:28 odoo13_addons_oca_purchase_workflow-13.0.20240518.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      449 b- defN 24-May-19 06:28 odoo13_addons_oca_purchase_workflow-13.0.20240518.0.dist-info/RECORD
+4 files, 5428 bytes uncompressed, 1264 bytes compressed:  76.7%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo13_addons_oca_purchase_workflow-13.0.20230612.0.dist-info/METADATA
+Filename: odoo13_addons_oca_purchase_workflow-13.0.20240518.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo13_addons_oca_purchase_workflow-13.0.20230612.0.dist-info/WHEEL
+Filename: odoo13_addons_oca_purchase_workflow-13.0.20240518.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo13_addons_oca_purchase_workflow-13.0.20230612.0.dist-info/top_level.txt
+Filename: odoo13_addons_oca_purchase_workflow-13.0.20240518.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo13_addons_oca_purchase_workflow-13.0.20230612.0.dist-info/RECORD
+Filename: odoo13_addons_oca_purchase_workflow-13.0.20240518.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo13_addons_oca_purchase_workflow-13.0.20230612.0.dist-info/METADATA` & `odoo13_addons_oca_purchase_workflow-13.0.20240518.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: odoo13-addons-oca-purchase-workflow
-Version: 13.0.20230612.0
+Version: 13.0.20240518.0
 Summary: Meta package for oca-purchase-workflow Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 13.0
+Requires-Dist: odoo13-addon-account-fiscal-position-allowed-journal-purchase
+Requires-Dist: odoo13-addon-account-fiscal-position-allowed-journal-sale-purchase
 Requires-Dist: odoo13-addon-procurement-purchase-no-grouping
 Requires-Dist: odoo13-addon-procurement-purchase-sale-no-grouping
 Requires-Dist: odoo13-addon-product-form-purchase-link
 Requires-Dist: odoo13-addon-product-supplierinfo-qty-multiplier
 Requires-Dist: odoo13-addon-purchase-all-shipments
 Requires-Dist: odoo13-addon-purchase-allowed-product
 Requires-Dist: odoo13-addon-purchase-analytic-global
```

