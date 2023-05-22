# Comparing `tmp/FyersTestSDK-0.0.1-py3-none-any.whl.zip` & `tmp/FyersTestSDK-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,11 @@
-Zip file size: 2263 bytes, number of entries: 5
--rwxrwxr-x  2.0 unx     1063 b- defN 23-May-22 11:35 FyersTestSDK-0.0.1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      887 b- defN 23-May-22 11:35 FyersTestSDK-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-22 11:35 FyersTestSDK-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 23-May-22 11:35 FyersTestSDK-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      413 b- defN 23-May-22 11:35 FyersTestSDK-0.0.1.dist-info/RECORD
-5 files, 2456 bytes uncompressed, 1485 bytes compressed:  39.5%
+Zip file size: 12258 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx        0 b- defN 23-May-22 11:49 fyerstest/__init__.py
+-rw-rw-r--  2.0 unx    16452 b- defN 23-May-22 11:30 fyerstest/fyersApi.py
+-rw-rw-r--  2.0 unx    15732 b- defN 23-May-22 11:31 fyerstest/hsmFyers.py
+-rw-rw-r--  2.0 unx     7894 b- defN 23-May-22 11:30 fyerstest/ws.py
+-rwxrwxr-x  2.0 unx     1063 b- defN 23-May-22 11:49 FyersTestSDK-0.0.2.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      887 b- defN 23-May-22 11:49 FyersTestSDK-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-22 11:49 FyersTestSDK-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-22 11:49 FyersTestSDK-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      719 b- defN 23-May-22 11:49 FyersTestSDK-0.0.2.dist-info/RECORD
+9 files, 42849 bytes uncompressed, 11020 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -1,16 +1,28 @@
-Filename: FyersTestSDK-0.0.1.dist-info/LICENSE.txt
+Filename: fyerstest/__init__.py
 Comment: 
 
-Filename: FyersTestSDK-0.0.1.dist-info/METADATA
+Filename: fyerstest/fyersApi.py
 Comment: 
 
-Filename: FyersTestSDK-0.0.1.dist-info/WHEEL
+Filename: fyerstest/hsmFyers.py
 Comment: 
 
-Filename: FyersTestSDK-0.0.1.dist-info/top_level.txt
+Filename: fyerstest/ws.py
 Comment: 
 
-Filename: FyersTestSDK-0.0.1.dist-info/RECORD
+Filename: FyersTestSDK-0.0.2.dist-info/LICENSE.txt
+Comment: 
+
+Filename: FyersTestSDK-0.0.2.dist-info/METADATA
+Comment: 
+
+Filename: FyersTestSDK-0.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: FyersTestSDK-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: FyersTestSDK-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `FyersTestSDK-0.0.1.dist-info/LICENSE.txt` & `FyersTestSDK-0.0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `FyersTestSDK-0.0.1.dist-info/METADATA` & `FyersTestSDK-0.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FyersTestSDK
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fyers trading APIs.
 Home-page: https://github.com/
 Author: Fyers-Tech
 Author-email: support@fyers.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

