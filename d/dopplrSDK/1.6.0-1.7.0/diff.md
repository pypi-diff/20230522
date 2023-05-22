# Comparing `tmp/dopplrSDK-1.6.0-py3-none-any.whl.zip` & `tmp/dopplrSDK-1.7.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3779 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     4865 b- defN 23-May-17 17:34 dopplrSDK/__init__.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-May-19 10:15 dopplrSDK-1.6.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      457 b- defN 23-May-19 10:15 dopplrSDK-1.6.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-19 10:15 dopplrSDK-1.6.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-May-19 10:15 dopplrSDK-1.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      477 b- defN 23-May-19 10:15 dopplrSDK-1.6.0.dist-info/RECORD
-6 files, 6978 bytes uncompressed, 2913 bytes compressed:  58.3%
+Zip file size: 3788 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     4924 b- defN 23-May-22 10:25 dopplrSDK/__init__.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-May-22 10:26 dopplrSDK-1.7.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      457 b- defN 23-May-22 10:26 dopplrSDK-1.7.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-22 10:26 dopplrSDK-1.7.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-22 10:26 dopplrSDK-1.7.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      477 b- defN 23-May-22 10:26 dopplrSDK-1.7.0.dist-info/RECORD
+6 files, 7037 bytes uncompressed, 2922 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: dopplrSDK/__init__.py
 Comment: 
 
-Filename: dopplrSDK-1.6.0.dist-info/LICENSE.txt
+Filename: dopplrSDK-1.7.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dopplrSDK-1.6.0.dist-info/METADATA
+Filename: dopplrSDK-1.7.0.dist-info/METADATA
 Comment: 
 
-Filename: dopplrSDK-1.6.0.dist-info/WHEEL
+Filename: dopplrSDK-1.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: dopplrSDK-1.6.0.dist-info/top_level.txt
+Filename: dopplrSDK-1.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dopplrSDK-1.6.0.dist-info/RECORD
+Filename: dopplrSDK-1.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dopplrSDK/__init__.py

```diff
@@ -55,15 +55,16 @@
         s3.upload_file(filePath, ContainerName, ConnectionString)
 
          # Generate a pre-signed URL
         
         s3.put_object_acl(ACL='public-read',
                           Bucket=ContainerName,
                           Key=ConnectionString)
-        url = f"https://{ContainerName}.s3.ap-south-1.amazonaws.com/{ConnectionString}"
+        #url = f"https://{ContainerName}.s3.ap-south-1.amazonaws.com/{ConnectionString}"
+        url = f"s3://{ContainerName}/{ConnectionString}"
         print("url : ",url)
         cnxn.close()
         #print("done")
     except Exception as error:
         if 'NoneType' in str(error):
             dopplrsource= 'File does not exists'
             print("Error : ", dopplrsource)
```

## Comparing `dopplrSDK-1.6.0.dist-info/LICENSE.txt` & `dopplrSDK-1.7.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

