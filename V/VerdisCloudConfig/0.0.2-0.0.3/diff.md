# Comparing `tmp/VerdisCloudConfig-0.0.2-py3-none-any.whl.zip` & `tmp/VerdisCloudConfig-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2643 bytes, number of entries: 6
--rw-r--r--  2.0 unx      973 b- defN 23-May-22 08:18 CloudConfig/__init__.py
--rw-r--r--  2.0 unx     1050 b- defN 23-May-22 08:19 VerdisCloudConfig-0.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      323 b- defN 23-May-22 08:19 VerdisCloudConfig-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 08:19 VerdisCloudConfig-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-22 08:19 VerdisCloudConfig-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      518 b- defN 23-May-22 08:19 VerdisCloudConfig-0.0.2.dist-info/RECORD
-6 files, 2968 bytes uncompressed, 1693 bytes compressed:  43.0%
+Zip file size: 2659 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     1007 b- defN 23-May-22 09:34 CloudConfig/__init__.py
+-rw-r--r--  2.0 unx     1050 b- defN 23-May-22 09:41 VerdisCloudConfig-0.0.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      323 b- defN 23-May-22 09:41 VerdisCloudConfig-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-22 09:41 VerdisCloudConfig-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-22 09:41 VerdisCloudConfig-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      519 b- defN 23-May-22 09:41 VerdisCloudConfig-0.0.3.dist-info/RECORD
+6 files, 3003 bytes uncompressed, 1709 bytes compressed:  43.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: CloudConfig/__init__.py
 Comment: 
 
-Filename: VerdisCloudConfig-0.0.2.dist-info/LICENSE.txt
+Filename: VerdisCloudConfig-0.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: VerdisCloudConfig-0.0.2.dist-info/METADATA
+Filename: VerdisCloudConfig-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: VerdisCloudConfig-0.0.2.dist-info/WHEEL
+Filename: VerdisCloudConfig-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: VerdisCloudConfig-0.0.2.dist-info/top_level.txt
+Filename: VerdisCloudConfig-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: VerdisCloudConfig-0.0.2.dist-info/RECORD
+Filename: VerdisCloudConfig-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## CloudConfig/__init__.py

```diff
@@ -1,17 +1,17 @@
-# import boto3
+import boto3
 import json
 import os
 def getParameter(name):
-    # session = boto3.Session(
-    # region_name='ap-south-1',
-    # aws_access_key_id=os.environ.get('aws_access_key_id', "ask shivam sir"),
-    # aws_secret_access_key=os.environ.get('aws_secret_access_key', "ask shivam sir"))
-    # ssm = session.client('ssm')
-    # return ssm.get_parameter(Name=name, WithDecryption=True)
+    session = boto3.Session(
+    region_name='ap-south-1',
+    aws_access_key_id=os.environ.get('aws_access_key_id', "ask shivam sir"),
+    aws_secret_access_key=os.environ.get('aws_secret_access_key', "ask shivam sir"))
+    ssm = session.client('ssm')
+    return ssm.get_parameter(Name=name, WithDecryption=True)
 
 
 def recurse(d, keys=()):
     if type(d) == dict:
         for k in d:
             for rv in recurse(d[k], keys + (k,)):
                 yield rv
@@ -26,8 +26,14 @@
         value = out['Parameter']['Value']
         if (-1 < value.find("{")) & (-1 < value.find("}")):
             result = json.loads(value)
         else:
             result = value
         config[compound_key[0]][compound_key[1]] = result
     
-    return config
+    return config
+
+
+def sum(a,b):
+    return a+b
+
+print(sum(3,5))
```

## Comparing `VerdisCloudConfig-0.0.2.dist-info/LICENSE.txt` & `VerdisCloudConfig-0.0.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

