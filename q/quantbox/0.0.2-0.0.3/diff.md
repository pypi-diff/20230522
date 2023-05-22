# Comparing `tmp/quantbox-0.0.2-py3-none-any.whl.zip` & `tmp/quantbox-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2117 bytes, number of entries: 6
--rw-rw-r--  2.0 unx       21 b- defN 23-May-20 23:51 quantbox/__init__.py
+Zip file size: 2128 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx       37 b- defN 23-May-22 02:35 quantbox/__init__.py
 -rw-rw-r--  2.0 unx     3237 b- defN 23-May-21 12:20 quantbox/quantbox.py
--rw-rw-r--  2.0 unx      650 b- defN 23-May-22 01:50 quantbox-0.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-22 01:50 quantbox-0.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-May-22 01:50 quantbox-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      452 b- defN 23-May-22 01:50 quantbox-0.0.2.dist-info/RECORD
-6 files, 4461 bytes uncompressed, 1295 bytes compressed:  71.0%
+-rw-rw-r--  2.0 unx      650 b- defN 23-May-22 02:35 quantbox-0.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-22 02:35 quantbox-0.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-22 02:35 quantbox-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      452 b- defN 23-May-22 02:35 quantbox-0.0.3.dist-info/RECORD
+6 files, 4477 bytes uncompressed, 1306 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: quantbox/__init__.py
 Comment: 
 
 Filename: quantbox/quantbox.py
 Comment: 
 
-Filename: quantbox-0.0.2.dist-info/METADATA
+Filename: quantbox-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: quantbox-0.0.2.dist-info/WHEEL
+Filename: quantbox-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: quantbox-0.0.2.dist-info/top_level.txt
+Filename: quantbox-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: quantbox-0.0.2.dist-info/RECORD
+Filename: quantbox-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quantbox/__init__.py

```diff
@@ -1 +1,2 @@
+import quantbox
 __version__ = '0.0.1'
```

## Comparing `quantbox-0.0.2.dist-info/METADATA` & `quantbox-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantbox
-Version: 0.0.2
+Version: 0.0.3
 Summary: quantbox wit api
 Home-page: UNKNOWN
 Author: ffolio
 Author-email: service@ffolio.co.kr
 License: UNKNOWN
 Keywords: pypi deploy
 Platform: UNKNOWN
```

