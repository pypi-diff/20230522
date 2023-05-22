# Comparing `tmp/quantbox-0.0.7-py3-none-any.whl.zip` & `tmp/quantbox-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3862 bytes, number of entries: 9
--rw-rw-r--  2.0 unx       65 b- defN 23-May-22 02:43 quantbox/__init__.py
+Zip file size: 3876 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx       84 b- defN 23-May-22 02:45 quantbox/__init__.py
 -rw-rw-r--  2.0 unx     3237 b- defN 23-May-21 12:20 quantbox/quantbox.py
 -rw-rw-r--  2.0 unx     3237 b- defN 23-May-21 12:20 quantbox/witapi.py
 -rw-rw-r--  2.0 unx       66 b- defN 23-May-22 02:39 witapi/__init__.py
 -rw-rw-r--  2.0 unx     3237 b- defN 23-May-21 12:20 witapi/quantbox.py
--rw-rw-r--  2.0 unx      650 b- defN 23-May-22 02:43 quantbox-0.0.7.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-22 02:43 quantbox-0.0.7.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-May-22 02:43 quantbox-0.0.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      675 b- defN 23-May-22 02:43 quantbox-0.0.7.dist-info/RECORD
-9 files, 11268 bytes uncompressed, 2704 bytes compressed:  76.0%
+-rw-rw-r--  2.0 unx      650 b- defN 23-May-22 02:45 quantbox-0.0.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-22 02:45 quantbox-0.0.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-22 02:45 quantbox-0.0.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      675 b- defN 23-May-22 02:45 quantbox-0.0.8.dist-info/RECORD
+9 files, 11287 bytes uncompressed, 2718 bytes compressed:  75.9%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: witapi/__init__.py
 Comment: 
 
 Filename: witapi/quantbox.py
 Comment: 
 
-Filename: quantbox-0.0.7.dist-info/METADATA
+Filename: quantbox-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: quantbox-0.0.7.dist-info/WHEEL
+Filename: quantbox-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: quantbox-0.0.7.dist-info/top_level.txt
+Filename: quantbox-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: quantbox-0.0.7.dist-info/RECORD
+Filename: quantbox-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## quantbox/__init__.py

```diff
@@ -1,2 +1,2 @@
-from .witapi import get_wit, get_shared_wit
+from .witapi import user_id, password, get_wit, get_shared_wit
 __version__ = '0.0.1'
```

## Comparing `quantbox-0.0.7.dist-info/METADATA` & `quantbox-0.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantbox
-Version: 0.0.7
+Version: 0.0.8
 Summary: quantbox wit api
 Home-page: UNKNOWN
 Author: ffolio
 Author-email: service@ffolio.co.kr
 License: UNKNOWN
 Keywords: pypi deploy
 Platform: UNKNOWN
```

## Comparing `quantbox-0.0.7.dist-info/RECORD` & `quantbox-0.0.8.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-quantbox/__init__.py,sha256=_Rlek0ddzkyZW3t4UhGZE5CzSwxFxImPcAOIJtYibtI,65
+quantbox/__init__.py,sha256=7WlGNrcRGJQ5u0beL29LeD7XMGR7um6zOlwbZmdT20M,84
 quantbox/quantbox.py,sha256=ZWQ5p0n9Ph8E5KQxc5bauYZNCMNQAFeoQ3JKzEb2idk,3237
 quantbox/witapi.py,sha256=ZWQ5p0n9Ph8E5KQxc5bauYZNCMNQAFeoQ3JKzEb2idk,3237
 witapi/__init__.py,sha256=WrFKEf-wG4FfrLNsmcGhJzGWQpCAJ6MYBavyBn44fwk,66
 witapi/quantbox.py,sha256=ZWQ5p0n9Ph8E5KQxc5bauYZNCMNQAFeoQ3JKzEb2idk,3237
-quantbox-0.0.7.dist-info/METADATA,sha256=yeKV9ZJqerzah_1nfNtEXo6XwV45e51JNJ9fM0oXCgg,650
-quantbox-0.0.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-quantbox-0.0.7.dist-info/top_level.txt,sha256=SP3T_P5Bvjw4luCDu7_LQwHvrAOTbbEXNdiHQIXuhc4,9
-quantbox-0.0.7.dist-info/RECORD,,
+quantbox-0.0.8.dist-info/METADATA,sha256=StD3F23C1aKyL73QbtNQLgqPHuxK1kcEvBGrBqs1c8E,650
+quantbox-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+quantbox-0.0.8.dist-info/top_level.txt,sha256=SP3T_P5Bvjw4luCDu7_LQwHvrAOTbbEXNdiHQIXuhc4,9
+quantbox-0.0.8.dist-info/RECORD,,
```

