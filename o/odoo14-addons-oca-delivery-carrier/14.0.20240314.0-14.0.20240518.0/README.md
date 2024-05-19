# Comparing `tmp/odoo14_addons_oca_delivery_carrier-14.0.20240314.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_delivery_carrier-14.0.20240518.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1828 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2848 b- defN 24-Mar-15 03:49 odoo14_addons_oca_delivery_carrier-14.0.20240314.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-15 03:49 odoo14_addons_oca_delivery_carrier-14.0.20240314.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-15 03:49 odoo14_addons_oca_delivery_carrier-14.0.20240314.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      445 b- defN 24-Mar-15 03:49 odoo14_addons_oca_delivery_carrier-14.0.20240314.0.dist-info/RECORD
-4 files, 3386 bytes uncompressed, 950 bytes compressed:  71.9%
+Zip file size: 1847 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2918 b- defN 24-May-19 03:54 odoo14_addons_oca_delivery_carrier-14.0.20240518.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-19 03:54 odoo14_addons_oca_delivery_carrier-14.0.20240518.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-May-19 03:54 odoo14_addons_oca_delivery_carrier-14.0.20240518.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      445 b- defN 24-May-19 03:54 odoo14_addons_oca_delivery_carrier-14.0.20240518.0.dist-info/RECORD
+4 files, 3456 bytes uncompressed, 969 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_delivery_carrier-14.0.20240314.0.dist-info/METADATA
+Filename: odoo14_addons_oca_delivery_carrier-14.0.20240518.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_delivery_carrier-14.0.20240314.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_delivery_carrier-14.0.20240518.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_delivery_carrier-14.0.20240314.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_delivery_carrier-14.0.20240518.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_delivery_carrier-14.0.20240314.0.dist-info/RECORD
+Filename: odoo14_addons_oca_delivery_carrier-14.0.20240518.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_delivery_carrier-14.0.20240314.0.dist-info/METADATA` & `odoo14_addons_oca_delivery_carrier-14.0.20240518.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-delivery-carrier
-Version: 14.0.20240314.0
+Version: 14.0.20240518.0
 Summary: Meta package for oca-delivery-carrier Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -42,14 +42,15 @@
 Requires-Dist: odoo14-addon-delivery-purchase
 Requires-Dist: odoo14-addon-delivery-roulier
 Requires-Dist: odoo14-addon-delivery-roulier-chronopost-fr
 Requires-Dist: odoo14-addon-delivery-roulier-laposte-fr
 Requires-Dist: odoo14-addon-delivery-roulier-option
 Requires-Dist: odoo14-addon-delivery-schenker
 Requires-Dist: odoo14-addon-delivery-schenker-picking-volume
+Requires-Dist: odoo14-addon-delivery-schenker-quant-package-dimension
 Requires-Dist: odoo14-addon-delivery-send-to-shipper-at-operation
 Requires-Dist: odoo14-addon-delivery-state
 Requires-Dist: odoo14-addon-delivery-tnt-oca
 Requires-Dist: odoo14-addon-partner-default-delivery-carrier
 Requires-Dist: odoo14-addon-partner-delivery-zone
 Requires-Dist: odoo14-addon-server-environment-delivery
 Requires-Dist: odoo14-addon-stock-picking-carrier-from-rule
```

