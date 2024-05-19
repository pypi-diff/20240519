# Comparing `tmp/odoo_addons_oca_sale_workflow-16.0.20240213.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_sale_workflow-16.0.20240502.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2223 bytes, number of entries: 4
--rw-r--r--  2.0 unx     6514 b- defN 24-Feb-15 06:38 odoo_addons_oca_sale_workflow-16.0.20240213.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-15 06:38 odoo_addons_oca_sale_workflow-16.0.20240213.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Feb-15 06:38 odoo_addons_oca_sale_workflow-16.0.20240213.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      425 b- defN 24-Feb-15 06:38 odoo_addons_oca_sale_workflow-16.0.20240213.0.dist-info/RECORD
-4 files, 7032 bytes uncompressed, 1385 bytes compressed:  80.3%
+Zip file size: 2239 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     6656 b- defN 24-May-03 05:42 odoo_addons_oca_sale_workflow-16.0.20240502.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-03 05:42 odoo_addons_oca_sale_workflow-16.0.20240502.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-03 05:42 odoo_addons_oca_sale_workflow-16.0.20240502.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      425 b- defN 24-May-03 05:42 odoo_addons_oca_sale_workflow-16.0.20240502.1.dist-info/RECORD
+4 files, 7174 bytes uncompressed, 1401 bytes compressed:  80.5%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_sale_workflow-16.0.20240213.0.dist-info/METADATA
+Filename: odoo_addons_oca_sale_workflow-16.0.20240502.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_sale_workflow-16.0.20240213.0.dist-info/WHEEL
+Filename: odoo_addons_oca_sale_workflow-16.0.20240502.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_sale_workflow-16.0.20240213.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_sale_workflow-16.0.20240502.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_sale_workflow-16.0.20240213.0.dist-info/RECORD
+Filename: odoo_addons_oca_sale_workflow-16.0.20240502.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_sale_workflow-16.0.20240213.0.dist-info/METADATA` & `odoo_addons_oca_sale_workflow-16.0.20240502.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-sale-workflow
-Version: 16.0.20240213.0
+Version: 16.0.20240502.1
 Summary: Meta package for oca-sale-workflow Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
@@ -27,14 +27,15 @@
 Requires-Dist: odoo-addon-sale-discount-display-amount <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-elaboration <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-exception <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-exception-holidays-public <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-fixed-discount <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-force-invoiced <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-invoice-frequency <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-sale-invoice-policy <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-last-price-info <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-loyalty-exclude <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-manual-delivery <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-mrp-bom <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-numeric-step <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-order-amount-to-invoice <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-order-archive <16.1dev,>=16.0dev
@@ -59,14 +60,15 @@
 Requires-Dist: odoo-addon-sale-order-product-availability-inline <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-order-product-picker <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-order-product-recommendation <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-order-product-recommendation-elaboration <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-order-product-recommendation-packaging-default <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-order-product-recommendation-quick-add <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-order-qty-change-no-recompute <16.1dev,>=16.0dev
+Requires-Dist: odoo-addon-sale-order-report-without-price <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-order-revision <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-order-type <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-order-warn-message <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-packaging-default <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-partner-incoterm <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-partner-pricelist <16.1dev,>=16.0dev
 Requires-Dist: odoo-addon-sale-partner-selectable-option <16.1dev,>=16.0dev
```

