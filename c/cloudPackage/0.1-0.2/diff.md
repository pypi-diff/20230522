# Comparing `tmp/cloudPackage-0.1-py3-none-any.whl.zip` & `tmp/cloudPackage-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2631 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat      936 b- defN 23-May-17 10:15 cloudPackage/__init__.py
--rw-rw-rw-  2.0 fat     1069 b- defN 23-May-17 10:47 cloudPackage-0.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      337 b- defN 23-May-17 10:47 cloudPackage-0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-17 10:47 cloudPackage-0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-May-17 10:47 cloudPackage-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      484 b- defN 23-May-17 10:47 cloudPackage-0.1.dist-info/RECORD
-6 files, 2931 bytes uncompressed, 1749 bytes compressed:  40.3%
+Zip file size: 2653 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     1023 b- defN 23-May-22 06:36 cloudPackage/__init__.py
+-rw-rw-rw-  2.0 fat     1069 b- defN 23-May-22 06:37 cloudPackage-0.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      337 b- defN 23-May-22 06:37 cloudPackage-0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-22 06:37 cloudPackage-0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-May-22 06:37 cloudPackage-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      485 b- defN 23-May-22 06:37 cloudPackage-0.2.dist-info/RECORD
+6 files, 3019 bytes uncompressed, 1771 bytes compressed:  41.3%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: cloudPackage/__init__.py
 Comment: 
 
-Filename: cloudPackage-0.1.dist-info/LICENSE.txt
+Filename: cloudPackage-0.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cloudPackage-0.1.dist-info/METADATA
+Filename: cloudPackage-0.2.dist-info/METADATA
 Comment: 
 
-Filename: cloudPackage-0.1.dist-info/WHEEL
+Filename: cloudPackage-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: cloudPackage-0.1.dist-info/top_level.txt
+Filename: cloudPackage-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: cloudPackage-0.1.dist-info/RECORD
+Filename: cloudPackage-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloudPackage/__init__.py

```diff
@@ -1,15 +1,15 @@
 import boto3
 import json
-
+import os
 def getParameter(name):
     session = boto3.Session(
     region_name='ap-south-1',
-    aws_access_key_id='AKIAYRRINRHOI2WGJOUL',
-    aws_secret_access_key='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')
+    aws_access_key_id=os.environ.get('aws_access_key_id', "AKIAYRRINRHOI2WGJOUL"),
+    aws_secret_access_key=os.environ.get('aws_secret_access_key', "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"))
     ssm = session.client('ssm')
     return ssm.get_parameter(Name=name, WithDecryption=True)
 
 
 def recurse(d, keys=()):
     if type(d) == dict:
         for k in d:
```

## Comparing `cloudPackage-0.1.dist-info/LICENSE.txt` & `cloudPackage-0.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

