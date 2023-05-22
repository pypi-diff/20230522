# Comparing `tmp/quantbox-0.0.4-py3-none-any.whl.zip` & `tmp/quantbox-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3032 bytes, number of entries: 8
+Zip file size: 3092 bytes, number of entries: 8
 -rw-rw-r--  2.0 unx       37 b- defN 23-May-22 02:35 quantbox/__init__.py
 -rw-rw-r--  2.0 unx     3237 b- defN 23-May-21 12:20 quantbox/quantbox.py
--rw-rw-r--  2.0 unx       37 b- defN 23-May-22 02:35 witapi/__init__.py
+-rw-rw-r--  2.0 unx       66 b- defN 23-May-22 02:39 witapi/__init__.py
 -rw-rw-r--  2.0 unx     3237 b- defN 23-May-21 12:20 witapi/quantbox.py
--rw-rw-r--  2.0 unx      650 b- defN 23-May-22 02:36 quantbox-0.0.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-22 02:36 quantbox-0.0.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-22 02:36 quantbox-0.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      600 b- defN 23-May-22 02:36 quantbox-0.0.4.dist-info/RECORD
-8 files, 7897 bytes uncompressed, 1986 bytes compressed:  74.9%
+-rw-rw-r--  2.0 unx      650 b- defN 23-May-22 02:39 quantbox-0.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-22 02:39 quantbox-0.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-22 02:39 quantbox-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      600 b- defN 23-May-22 02:39 quantbox-0.0.5.dist-info/RECORD
+8 files, 7926 bytes uncompressed, 2046 bytes compressed:  74.2%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: witapi/__init__.py
 Comment: 
 
 Filename: witapi/quantbox.py
 Comment: 
 
-Filename: quantbox-0.0.4.dist-info/METADATA
+Filename: quantbox-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: quantbox-0.0.4.dist-info/WHEEL
+Filename: quantbox-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: quantbox-0.0.4.dist-info/top_level.txt
+Filename: quantbox-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: quantbox-0.0.4.dist-info/RECORD
+Filename: quantbox-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## witapi/__init__.py

```diff
@@ -1,2 +1,2 @@
-import quantbox
+from quantbox import get_wit, get_shared_wit
 __version__ = '0.0.1'
```

## Comparing `quantbox-0.0.4.dist-info/METADATA` & `quantbox-0.0.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantbox
-Version: 0.0.4
+Version: 0.0.5
 Summary: quantbox wit api
 Home-page: UNKNOWN
 Author: ffolio
 Author-email: service@ffolio.co.kr
 License: UNKNOWN
 Keywords: pypi deploy
 Platform: UNKNOWN
```

