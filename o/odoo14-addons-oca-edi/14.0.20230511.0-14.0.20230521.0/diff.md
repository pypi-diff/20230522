# Comparing `tmp/odoo14_addons_oca_edi-14.0.20230511.0-py3-none-any.whl.zip` & `tmp/odoo14_addons_oca_edi-14.0.20230521.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1664 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2954 b- defN 23-May-12 04:19 odoo14_addons_oca_edi-14.0.20230511.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-12 04:19 odoo14_addons_oca_edi-14.0.20230511.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-12 04:19 odoo14_addons_oca_edi-14.0.20230511.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      393 b- defN 23-May-12 04:19 odoo14_addons_oca_edi-14.0.20230511.0.dist-info/RECORD
-4 files, 3440 bytes uncompressed, 890 bytes compressed:  74.1%
+Zip file size: 1669 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2999 b- defN 23-May-22 05:08 odoo14_addons_oca_edi-14.0.20230521.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-22 05:08 odoo14_addons_oca_edi-14.0.20230521.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-22 05:08 odoo14_addons_oca_edi-14.0.20230521.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      393 b- defN 23-May-22 05:08 odoo14_addons_oca_edi-14.0.20230521.0.dist-info/RECORD
+4 files, 3485 bytes uncompressed, 895 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_oca_edi-14.0.20230511.0.dist-info/METADATA
+Filename: odoo14_addons_oca_edi-14.0.20230521.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_oca_edi-14.0.20230511.0.dist-info/WHEEL
+Filename: odoo14_addons_oca_edi-14.0.20230521.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_oca_edi-14.0.20230511.0.dist-info/top_level.txt
+Filename: odoo14_addons_oca_edi-14.0.20230521.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_oca_edi-14.0.20230511.0.dist-info/RECORD
+Filename: odoo14_addons_oca_edi-14.0.20230521.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_oca_edi-14.0.20230511.0.dist-info/METADATA` & `odoo14_addons_oca_edi-14.0.20230521.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-oca-edi
-Version: 14.0.20230511.0
+Version: 14.0.20230521.0
 Summary: Meta package for oca-edi Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -33,14 +33,15 @@
 Requires-Dist: odoo14-addon-edi-account-oca
 Requires-Dist: odoo14-addon-edi-backend-partner-oca
 Requires-Dist: odoo14-addon-edi-endpoint-oca
 Requires-Dist: odoo14-addon-edi-exchange-template-oca
 Requires-Dist: odoo14-addon-edi-exchange-template-party-data
 Requires-Dist: odoo14-addon-edi-oca
 Requires-Dist: odoo14-addon-edi-party-data-oca
+Requires-Dist: odoo14-addon-edi-pdf2data-oca
 Requires-Dist: odoo14-addon-edi-purchase-oca
 Requires-Dist: odoo14-addon-edi-sale-order-import
 Requires-Dist: odoo14-addon-edi-sale-order-import-ubl
 Requires-Dist: odoo14-addon-edi-sale-order-import-ubl-endpoint
 Requires-Dist: odoo14-addon-edi-stock-oca
 Requires-Dist: odoo14-addon-edi-storage-oca
 Requires-Dist: odoo14-addon-edi-ubl-oca
```

