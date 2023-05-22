# Comparing `tmp/FyersTestSDK-0.0.2-py3-none-any.whl.zip` & `tmp/FyersTestSDK-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12258 bytes, number of entries: 9
--rw-rw-r--  2.0 unx        0 b- defN 23-May-22 11:49 fyerstest/__init__.py
+Zip file size: 12276 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       18 b- defN 23-May-22 11:53 fyerstest/__init__.py
 -rw-rw-r--  2.0 unx    16452 b- defN 23-May-22 11:30 fyerstest/fyersApi.py
 -rw-rw-r--  2.0 unx    15732 b- defN 23-May-22 11:31 fyerstest/hsmFyers.py
 -rw-rw-r--  2.0 unx     7894 b- defN 23-May-22 11:30 fyerstest/ws.py
--rwxrwxr-x  2.0 unx     1063 b- defN 23-May-22 11:49 FyersTestSDK-0.0.2.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      887 b- defN 23-May-22 11:49 FyersTestSDK-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-22 11:49 FyersTestSDK-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-May-22 11:49 FyersTestSDK-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      719 b- defN 23-May-22 11:49 FyersTestSDK-0.0.2.dist-info/RECORD
-9 files, 42849 bytes uncompressed, 11020 bytes compressed:  74.3%
+-rwxrwxr-x  2.0 unx     1063 b- defN 23-May-22 11:53 FyersTestSDK-0.0.3.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      887 b- defN 23-May-22 11:53 FyersTestSDK-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-22 11:53 FyersTestSDK-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-22 11:53 FyersTestSDK-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      720 b- defN 23-May-22 11:53 FyersTestSDK-0.0.3.dist-info/RECORD
+9 files, 42868 bytes uncompressed, 11038 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: fyerstest/hsmFyers.py
 Comment: 
 
 Filename: fyerstest/ws.py
 Comment: 
 
-Filename: FyersTestSDK-0.0.2.dist-info/LICENSE.txt
+Filename: FyersTestSDK-0.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: FyersTestSDK-0.0.2.dist-info/METADATA
+Filename: FyersTestSDK-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: FyersTestSDK-0.0.2.dist-info/WHEEL
+Filename: FyersTestSDK-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: FyersTestSDK-0.0.2.dist-info/top_level.txt
+Filename: FyersTestSDK-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: FyersTestSDK-0.0.2.dist-info/RECORD
+Filename: FyersTestSDK-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fyerstest/__init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 6e61 6d65 203d 2022 6679 6572 7374 6573  name = "fyerstes
+00000010: 7422                                     t"
```

## Comparing `FyersTestSDK-0.0.2.dist-info/LICENSE.txt` & `FyersTestSDK-0.0.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `FyersTestSDK-0.0.2.dist-info/METADATA` & `FyersTestSDK-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FyersTestSDK
-Version: 0.0.2
+Version: 0.0.3
 Summary: Fyers trading APIs.
 Home-page: https://github.com/
 Author: Fyers-Tech
 Author-email: support@fyers.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `FyersTestSDK-0.0.2.dist-info/RECORD` & `FyersTestSDK-0.0.3.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-fyerstest/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+fyerstest/__init__.py,sha256=1WtJ-kBOz0GPiSSxR-0td92oauv9r-T1OZzwbWY7wSw,18
 fyerstest/fyersApi.py,sha256=b3sBmhimC8QRfTUFGvuxJdQOENPKJuZfaLzcPP-xqQs,16452
 fyerstest/hsmFyers.py,sha256=reTSHoHsTTc8fwWEsVOicnSFUcOVbJdE1E0idHLKkmM,15732
 fyerstest/ws.py,sha256=9oGuGvjxVi7KnbnuPnF_nRyufydQS5Nh-ao_7b-ea8Y,7894
-FyersTestSDK-0.0.2.dist-info/LICENSE.txt,sha256=_a5I4lWvSmoZQxwGSPGVVvUbuYby780N9YevsBqNY3k,1063
-FyersTestSDK-0.0.2.dist-info/METADATA,sha256=jiP2LCpriCeaJtFN0Zch8Cyniarfnp2rBwoCVpTZJRA,887
-FyersTestSDK-0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-FyersTestSDK-0.0.2.dist-info/top_level.txt,sha256=Eyvif7X2Qc19PxARHGE_TXQWTytbm9zBR8d1dFWJogI,10
-FyersTestSDK-0.0.2.dist-info/RECORD,,
+FyersTestSDK-0.0.3.dist-info/LICENSE.txt,sha256=_a5I4lWvSmoZQxwGSPGVVvUbuYby780N9YevsBqNY3k,1063
+FyersTestSDK-0.0.3.dist-info/METADATA,sha256=koWjbifmoSaDnj7aGbIPUsqHrdEiMTz-oTb2VdTHBys,887
+FyersTestSDK-0.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+FyersTestSDK-0.0.3.dist-info/top_level.txt,sha256=Eyvif7X2Qc19PxARHGE_TXQWTytbm9zBR8d1dFWJogI,10
+FyersTestSDK-0.0.3.dist-info/RECORD,,
```

