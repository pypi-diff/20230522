# Comparing `tmp/query_toolkits-1.2.0-py3-none-any.whl.zip` & `tmp/query_toolkits-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 2514723 bytes, number of entries: 18
--rw-r--r--  2.0 unx      619 b- defN 23-May-16 12:40 query_toolkits/__init__.py
+Zip file size: 2514854 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      845 b- defN 23-May-22 02:33 query_toolkits/__init__.py
 -rw-r--r--  2.0 unx    40836 b- defN 23-Mar-29 03:08 query_toolkits/error_correction.py
--rw-r--r--  2.0 unx    25561 b- defN 23-May-17 07:46 query_toolkits/extractor.py
+-rw-r--r--  2.0 unx    26721 b- defN 23-May-22 02:33 query_toolkits/extractor.py
 -rw-r--r--  2.0 unx      683 b- defN 23-May-16 14:13 query_toolkits/financial_index.txt
 -rw-r--r--  2.0 unx    15889 b- defN 23-May-16 13:44 query_toolkits/financial_index_full.txt
 -rw-r--r--  2.0 unx  1056198 b- defN 23-Feb-27 08:08 query_toolkits/fund_product.txt
 -rw-r--r--  2.0 unx    18015 b- defN 23-May-16 12:35 query_toolkits/index.txt
 -rw-------  2.0 unx 44320114 b- defN 23-Mar-29 02:13 query_toolkits/info.json
 -rw-r--r--  2.0 unx      153 b- defN 22-Oct-10 04:02 query_toolkits/keyword.txt
 -rw-r--r--  2.0 unx   634483 b- defN 22-Oct-12 02:15 query_toolkits/organization.txt
 -rw-r--r--  2.0 unx     9995 b- defN 23-May-16 12:30 query_toolkits/product.txt
 -rw-r--r--  2.0 unx     2237 b- defN 22-Aug-15 03:50 query_toolkits/unit_transform
 -rw-r--r--  2.0 unx     5453 b- defN 23-Mar-29 02:52 query_toolkits/utils.py
 -rw-------  2.0 unx   420676 b- defN 22-Oct-20 07:33 query_toolkits/weapon.txt
--rw-r--r--  2.0 unx      230 b- defN 23-May-17 08:31 query_toolkits-1.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-17 08:31 query_toolkits-1.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-May-17 08:31 query_toolkits-1.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1534 b- defN 23-May-17 08:31 query_toolkits-1.2.0.dist-info/RECORD
-18 files, 46552783 bytes uncompressed, 2512223 bytes compressed:  94.6%
+-rw-r--r--  2.0 unx      230 b- defN 23-May-22 02:34 query_toolkits-1.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-22 02:34 query_toolkits-1.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-May-22 02:34 query_toolkits-1.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1534 b- defN 23-May-22 02:34 query_toolkits-1.2.1.dist-info/RECORD
+18 files, 46554169 bytes uncompressed, 2512354 bytes compressed:  94.6%
```

## zipnote {}

```diff
@@ -36,20 +36,20 @@
 
 Filename: query_toolkits/utils.py
 Comment: 
 
 Filename: query_toolkits/weapon.txt
 Comment: 
 
-Filename: query_toolkits-1.2.0.dist-info/METADATA
+Filename: query_toolkits-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: query_toolkits-1.2.0.dist-info/WHEEL
+Filename: query_toolkits-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: query_toolkits-1.2.0.dist-info/top_level.txt
+Filename: query_toolkits-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: query_toolkits-1.2.0.dist-info/RECORD
+Filename: query_toolkits-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## query_toolkits/__init__.py

```diff
@@ -12,9 +12,17 @@
 extract_financial_index = et.extract_financial_index
 extract_fund_name = et.extract_fund_name
 extract_stock_name = et.extract_stock_name
 extract_product_name = et.extract_product_name
 extract_index_name = et.extract_index_name
 
 
+get_organization = et.get_organization
+get_financial_dict = et.get_financial_dict
+get_fund_name = et.get_fund_name
+get_stock_dict = et.get_stock_dict
+get_product_dict = et.get_product_dict
+get_index_dict = et.get_index_dict
+
+
 c = Corrector()
 correct = c.correct
```

## query_toolkits/extractor.py

```diff
@@ -477,14 +477,51 @@
         di = self.index_dict if word_dict is None else word_dict
         keys = di.keys()
         res = utils.max_backward_match(cut_words, keys, 10)
         res = [(elem[0], di[elem[0]]) for elem in res]
         return res
 
 
+    """
+     self.unit_transform = utils._read_table(_get_module_path("unit_transform"))
+        self.organization = utils._read_list(_get_module_path("organization.txt"))
+        self.keyword = utils._read_list(_get_module_path("keyword.txt"))
+        self.financial_dict = utils.list2dict(utils._read_list(_get_module_path("financial_index.txt")))
+        self.financial_dict_keys = set(self.financial_dict.keys())
+        self.fund_name = utils._read_list(_get_module_path("fund_product.txt"))
+        self.stock_dict = utils._stock_dict(_get_module_path("info.json"))
+        self.product_dict = utils.list2dict(utils._read_list(_get_module_path("product.txt")))
+        self.index_dict = utils.list2dict(utils._read_list(_get_module_path("index.txt")))
+    """
+
+    def get_organization(self):
+        return self.organization
+
+
+    def get_financial_dict(self):
+        return self.financial_dict
+
+
+    def get_fund_name(self):
+        return self.fund_name
+
+
+    def get_stock_dict(self):
+        return self.stock_dict
+
+
+    def get_product_dict(self):
+        return self.product_dict
+
+
+    def get_index_dict(self):
+        return self.index_dict
+
+
+
```

## Comparing `query_toolkits-1.2.0.dist-info/RECORD` & `query_toolkits-1.2.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-query_toolkits/__init__.py,sha256=kQKgjRz0yrN3thfaOX3uJ7JKV1zfunoyHcB7h3tCtsw,619
+query_toolkits/__init__.py,sha256=EveacW4_39hG1bXQXu2-_iach21RtE1NVgSjXgmaDyE,845
 query_toolkits/error_correction.py,sha256=auit3b2ihsuWufmNixOrjC5CEjVrD2IiAzj461YrJUg,40836
-query_toolkits/extractor.py,sha256=mt2_MoyoUBeus3AXepnR896pAfE4L-5ioz_8jSPi3-Y,25561
+query_toolkits/extractor.py,sha256=6QwR2P-SXkf0-HeEtND5n6S-PikZSHQEwUTZSC5JmyM,26721
 query_toolkits/financial_index.txt,sha256=BJDWXmJ0vziCHq6hq8cOEUCdPegzweiugvDObb23lKQ,683
 query_toolkits/financial_index_full.txt,sha256=1ViFxMXJd2BvCxjlOI0vAAKuHFTrx2JAdnjtId9jxqc,15889
 query_toolkits/fund_product.txt,sha256=Fn3FPhk10KjtHkyXD0OHK8OttYjVtN4KRiTQ6X4c0uI,1056198
 query_toolkits/index.txt,sha256=W9_pC0bCTEVykwjwSI1Zi7gFFW94BrsvKdkzRBkhWBw,18015
 query_toolkits/info.json,sha256=BC85jy__r1H89WHSJqkmfKK0arna3MlP0V3cDvARo_w,44320114
 query_toolkits/keyword.txt,sha256=iFtkA8SUDbKViFYSg2YPP9RG_btJ35AlGor06ywy0A4,153
 query_toolkits/organization.txt,sha256=hRLDyvQKxw-_XgM2WEQ9MD3DvmanTluYu2Z6Se5JYro,634483
 query_toolkits/product.txt,sha256=PAWJ7YtTOydgsGcZ470hQ-wgXtYHMEDCFa23lKy1Zns,9995
 query_toolkits/unit_transform,sha256=yHFE7ydHauFdJy13GNCyYmNZy0gQWd0lYlvki_6OUD4,2237
 query_toolkits/utils.py,sha256=zPTVyjmxeioiND7PlUfCkUjMi50wKgcRghyzmo_20ig,5453
 query_toolkits/weapon.txt,sha256=rpGr_JynyYjrvnoM-swGLM1DLdxNKITUNJyfb_juw_E,420676
-query_toolkits-1.2.0.dist-info/METADATA,sha256=rhrq6_s9Ss5rwm_1ZTRc1fVT6hsG6-X0AjRe2VZwrnY,230
-query_toolkits-1.2.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-query_toolkits-1.2.0.dist-info/top_level.txt,sha256=oX-XPh75LlcNrWWX-7EQ7ciThjo7m_iFQkriyWxvwCo,15
-query_toolkits-1.2.0.dist-info/RECORD,,
+query_toolkits-1.2.1.dist-info/METADATA,sha256=suJdXJZE39lMZr_yfg7u78ZQSclXepTJNWjf_vVWfQ0,230
+query_toolkits-1.2.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+query_toolkits-1.2.1.dist-info/top_level.txt,sha256=oX-XPh75LlcNrWWX-7EQ7ciThjo7m_iFQkriyWxvwCo,15
+query_toolkits-1.2.1.dist-info/RECORD,,
```

