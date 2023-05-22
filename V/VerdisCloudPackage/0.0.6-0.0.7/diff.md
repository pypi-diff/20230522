# Comparing `tmp/VerdisCloudPackage-0.0.6-py3-none-any.whl.zip` & `tmp/VerdisCloudPackage-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2985 bytes, number of entries: 7
+Zip file size: 3007 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      991 b- defN 23-May-22 10:22 VerdisCloudPackage/AWS.py
--rw-rw-rw-  2.0 fat      226 b- defN 23-May-22 10:27 VerdisCloudPackage/__init__.py
--rw-rw-rw-  2.0 fat     1059 b- defN 23-May-22 10:28 VerdisCloudPackage-0.0.6.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      332 b- defN 23-May-22 10:28 VerdisCloudPackage-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-22 10:28 VerdisCloudPackage-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       19 b- defN 23-May-22 10:28 VerdisCloudPackage-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      611 b- defN 23-May-22 10:28 VerdisCloudPackage-0.0.6.dist-info/RECORD
-7 files, 3330 bytes uncompressed, 1885 bytes compressed:  43.4%
+-rw-rw-rw-  2.0 fat      250 b- defN 23-May-22 10:35 VerdisCloudPackage/__init__.py
+-rw-rw-rw-  2.0 fat     1059 b- defN 23-May-22 10:36 VerdisCloudPackage-0.0.7.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      332 b- defN 23-May-22 10:36 VerdisCloudPackage-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-22 10:36 VerdisCloudPackage-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       19 b- defN 23-May-22 10:36 VerdisCloudPackage-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      611 b- defN 23-May-22 10:36 VerdisCloudPackage-0.0.7.dist-info/RECORD
+7 files, 3354 bytes uncompressed, 1907 bytes compressed:  43.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: VerdisCloudPackage/AWS.py
 Comment: 
 
 Filename: VerdisCloudPackage/__init__.py
 Comment: 
 
-Filename: VerdisCloudPackage-0.0.6.dist-info/LICENSE.txt
+Filename: VerdisCloudPackage-0.0.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: VerdisCloudPackage-0.0.6.dist-info/METADATA
+Filename: VerdisCloudPackage-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: VerdisCloudPackage-0.0.6.dist-info/WHEEL
+Filename: VerdisCloudPackage-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: VerdisCloudPackage-0.0.6.dist-info/top_level.txt
+Filename: VerdisCloudPackage-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: VerdisCloudPackage-0.0.6.dist-info/RECORD
+Filename: VerdisCloudPackage-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## VerdisCloudPackage/__init__.py

```diff
@@ -1,9 +1,9 @@
 import os
-import AWS
+from VerdisCloudPackage import AWS
 def cloud_choice(config):
     cloud_ch=os.environ.get('PYTHON_CLOUD', "AWS")
     if cloud_ch=="AWS":
         return AWS.getParams(config)
     else:
         return AWS.getParams(config)
```

## Comparing `VerdisCloudPackage-0.0.6.dist-info/LICENSE.txt` & `VerdisCloudPackage-0.0.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

