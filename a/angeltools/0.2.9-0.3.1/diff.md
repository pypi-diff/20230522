# Comparing `tmp/angeltools-0.2.9.tar.gz` & `tmp/angeltools-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angeltools-0.2.9.tar", last modified: Fri May 19 08:24:27 2023, max compression
+gzip compressed data, was "angeltools-0.3.1.tar", last modified: Mon May 22 07:32:11 2023, max compression
```

## Comparing `angeltools-0.2.9.tar` & `angeltools-0.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-19 08:24:27.987460 angeltools-0.2.9/
--rw-rw-r--   0 ga        (1000) ga        (1000)     1073 2019-08-14 09:31:42.000000 angeltools-0.2.9/LICENSE
--rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-19 08:24:27.987460 angeltools-0.2.9/PKG-INFO
--rw-rw-r--   0 ga        (1000) ga        (1000)     7097 2022-04-22 09:10:52.000000 angeltools-0.2.9/README.md
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-19 08:24:27.983460 angeltools-0.2.9/angeltools/
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-19 08:24:27.987460 angeltools-0.2.9/angeltools/Db/
--rw-rw-r--   0 ga        (1000) ga        (1000)     1057 2022-04-20 06:29:56.000000 angeltools-0.2.9/angeltools/Db/__init__.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     3297 2023-05-19 07:03:17.000000 angeltools-0.2.9/angeltools/Db/redis_connector.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     4843 2023-05-15 08:57:48.000000 angeltools-0.2.9/angeltools/ImageTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     2524 2022-04-21 01:32:32.000000 angeltools-0.2.9/angeltools/MathTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     8235 2023-05-15 08:49:17.000000 angeltools-0.2.9/angeltools/Slavers.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    15912 2023-05-19 08:23:24.000000 angeltools-0.2.9/angeltools/StrTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     1409 2023-05-15 08:55:25.000000 angeltools-0.2.9/angeltools/TimeTool.py
--rw-rw-r--   0 ga        (1000) ga        (1000)        0 2022-04-20 03:36:02.000000 angeltools-0.2.9/angeltools/__init__.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     6469 2023-05-15 08:45:59.000000 angeltools-0.2.9/angeltools/commands.py
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-19 08:24:27.987460 angeltools-0.2.9/angeltools/fdfs/
--rw-rw-r--   0 ga        (1000) ga        (1000)      279 2022-04-22 03:00:25.000000 angeltools-0.2.9/angeltools/fdfs/__init__.py
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-19 08:24:27.987460 angeltools-0.2.9/angeltools/fdfs/fdfs_client/
--rw-rw-r--   0 ga        (1000) ga        (1000)       88 2022-03-24 09:03:37.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/__init__.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    25820 2022-04-22 02:43:06.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/client.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     6523 2022-04-22 02:55:22.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/connection.py
--rw-rw-r--   0 ga        (1000) ga        (1000)      328 2022-03-24 09:03:37.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/exceptions.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     8472 2022-04-22 02:55:48.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/fdfs_protol.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    13862 2022-04-22 02:55:48.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/fdfs_test.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    28082 2022-04-22 02:57:59.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/storage_client.py
--rw-rw-r--   0 ga        (1000) ga        (1000)    22129 2022-04-22 02:56:03.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/tracker_client.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     8382 2022-04-22 02:56:37.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_client/utils.py
--rw-rw-r--   0 ga        (1000) ga        (1000)     3683 2022-04-22 09:14:10.000000 angeltools-0.2.9/angeltools/fdfs/fdfs_operator.py
-drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-19 08:24:27.987460 angeltools-0.2.9/angeltools.egg-info/
--rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-19 08:24:27.000000 angeltools-0.2.9/angeltools.egg-info/PKG-INFO
--rw-rw-r--   0 ga        (1000) ga        (1000)      920 2023-05-19 08:24:27.000000 angeltools-0.2.9/angeltools.egg-info/SOURCES.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)        1 2023-05-19 08:24:27.000000 angeltools-0.2.9/angeltools.egg-info/dependency_links.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)      159 2023-05-19 08:24:27.000000 angeltools-0.2.9/angeltools.egg-info/entry_points.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)        1 2019-05-06 02:05:56.000000 angeltools-0.2.9/angeltools.egg-info/not-zip-safe
--rw-rw-r--   0 ga        (1000) ga        (1000)       92 2023-05-19 08:24:27.000000 angeltools-0.2.9/angeltools.egg-info/requires.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)       11 2023-05-19 08:24:27.000000 angeltools-0.2.9/angeltools.egg-info/top_level.txt
--rw-rw-r--   0 ga        (1000) ga        (1000)       38 2023-05-19 08:24:27.987460 angeltools-0.2.9/setup.cfg
--rw-rw-r--   0 ga        (1000) ga        (1000)     1366 2023-05-19 08:24:14.000000 angeltools-0.2.9/setup.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-22 07:32:11.847778 angeltools-0.3.1/
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1073 2019-08-14 09:31:42.000000 angeltools-0.3.1/LICENSE
+-rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-22 07:32:11.847778 angeltools-0.3.1/PKG-INFO
+-rw-rw-r--   0 ga        (1000) ga        (1000)     7097 2022-04-22 09:10:52.000000 angeltools-0.3.1/README.md
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-22 07:32:11.847778 angeltools-0.3.1/angeltools/
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-22 07:32:11.847778 angeltools-0.3.1/angeltools/Db/
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1057 2022-04-20 06:29:56.000000 angeltools-0.3.1/angeltools/Db/__init__.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     3297 2023-05-19 07:03:17.000000 angeltools-0.3.1/angeltools/Db/redis_connector.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     4843 2023-05-15 08:57:48.000000 angeltools-0.3.1/angeltools/ImageTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     2524 2022-04-21 01:32:32.000000 angeltools-0.3.1/angeltools/MathTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     8235 2023-05-15 08:49:17.000000 angeltools-0.3.1/angeltools/Slavers.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    18098 2023-05-22 07:31:05.000000 angeltools-0.3.1/angeltools/StrTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1409 2023-05-15 08:55:25.000000 angeltools-0.3.1/angeltools/TimeTool.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)        0 2022-04-20 03:36:02.000000 angeltools-0.3.1/angeltools/__init__.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     6469 2023-05-15 08:45:59.000000 angeltools-0.3.1/angeltools/commands.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-22 07:32:11.847778 angeltools-0.3.1/angeltools/fdfs/
+-rw-rw-r--   0 ga        (1000) ga        (1000)      279 2022-04-22 03:00:25.000000 angeltools-0.3.1/angeltools/fdfs/__init__.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-22 07:32:11.847778 angeltools-0.3.1/angeltools/fdfs/fdfs_client/
+-rw-rw-r--   0 ga        (1000) ga        (1000)       88 2022-03-24 09:03:37.000000 angeltools-0.3.1/angeltools/fdfs/fdfs_client/__init__.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    25820 2022-04-22 02:43:06.000000 angeltools-0.3.1/angeltools/fdfs/fdfs_client/client.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     6523 2022-04-22 02:55:22.000000 angeltools-0.3.1/angeltools/fdfs/fdfs_client/connection.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)      328 2022-03-24 09:03:37.000000 angeltools-0.3.1/angeltools/fdfs/fdfs_client/exceptions.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     8472 2022-04-22 02:55:48.000000 angeltools-0.3.1/angeltools/fdfs/fdfs_client/fdfs_protol.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    13862 2022-04-22 02:55:48.000000 angeltools-0.3.1/angeltools/fdfs/fdfs_client/fdfs_test.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    28082 2022-04-22 02:57:59.000000 angeltools-0.3.1/angeltools/fdfs/fdfs_client/storage_client.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)    22129 2022-04-22 02:56:03.000000 angeltools-0.3.1/angeltools/fdfs/fdfs_client/tracker_client.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     8382 2022-04-22 02:56:37.000000 angeltools-0.3.1/angeltools/fdfs/fdfs_client/utils.py
+-rw-rw-r--   0 ga        (1000) ga        (1000)     3683 2022-04-22 09:14:10.000000 angeltools-0.3.1/angeltools/fdfs/fdfs_operator.py
+drwxrwxr-x   0 ga        (1000) ga        (1000)        0 2023-05-22 07:32:11.847778 angeltools-0.3.1/angeltools.egg-info/
+-rw-rw-r--   0 ga        (1000) ga        (1000)     7566 2023-05-22 07:32:11.000000 angeltools-0.3.1/angeltools.egg-info/PKG-INFO
+-rw-rw-r--   0 ga        (1000) ga        (1000)      920 2023-05-22 07:32:11.000000 angeltools-0.3.1/angeltools.egg-info/SOURCES.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)        1 2023-05-22 07:32:11.000000 angeltools-0.3.1/angeltools.egg-info/dependency_links.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)      159 2023-05-22 07:32:11.000000 angeltools-0.3.1/angeltools.egg-info/entry_points.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)        1 2019-05-06 02:05:56.000000 angeltools-0.3.1/angeltools.egg-info/not-zip-safe
+-rw-rw-r--   0 ga        (1000) ga        (1000)       92 2023-05-22 07:32:11.000000 angeltools-0.3.1/angeltools.egg-info/requires.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)       11 2023-05-22 07:32:11.000000 angeltools-0.3.1/angeltools.egg-info/top_level.txt
+-rw-rw-r--   0 ga        (1000) ga        (1000)       38 2023-05-22 07:32:11.847778 angeltools-0.3.1/setup.cfg
+-rw-rw-r--   0 ga        (1000) ga        (1000)     1366 2023-05-22 07:32:04.000000 angeltools-0.3.1/setup.py
```

### Comparing `angeltools-0.2.9/LICENSE` & `angeltools-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/PKG-INFO` & `angeltools-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angeltools
-Version: 0.2.9
+Version: 0.3.1
 Summary: personal python small tools collection
 Home-page: https://github.com/ga1008/angeltools
 Author: Guardian
 Author-email: zhling2012@live.com
 Maintainer: Guardian
 Maintainer-email: zhling2012@live.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `angeltools-0.2.9/README.md` & `angeltools-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools/Db/__init__.py` & `angeltools-0.3.1/angeltools/Db/__init__.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools/Db/redis_connector.py` & `angeltools-0.3.1/angeltools/Db/redis_connector.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools/ImageTool.py` & `angeltools-0.3.1/angeltools/ImageTool.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools/MathTool.py` & `angeltools-0.3.1/angeltools/MathTool.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools/Slavers.py` & `angeltools-0.3.1/angeltools/Slavers.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools/StrTool.py` & `angeltools-0.3.1/angeltools/StrTool.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import hashlib
+import json
 import os
 import random
 import re
 import sys
 import time
 import uuid
 from pathlib import Path
@@ -224,14 +225,82 @@
             new_url = sep.join(path_lis)
         return new_url
 
 
 file_lock_prefix = 'file_lock_'
 
 
+class LocalData:
+    def __init__(self, store_path=None):
+        file_dir = self._init_local_path(store_path)
+        file_pre = "core_data_"
+        self.f_pre = f"{file_dir}/{file_pre}"
+        self.expire_time = 3600 * 24 * 365 * 100
+
+    def _init_local_path(self, file_path):
+        import subprocess
+
+        if not file_path:
+            file_path = '/tmp'
+        if not os.path.exists(file_path):
+            params = [
+                f"mkdir -p {file_path}",
+            ]
+            dp = subprocess.run(params, shell=True, capture_output=True)
+            if "无法创建目录" in dp.stderr.decode('utf-8'):
+                file_path = '/tmp'
+        return file_path
+
+    def _file_name(self, fid):
+        return f"{self.f_pre}{fid}.json"
+
+    def get_fid(self, data):
+        if not isinstance(data, str):
+            data = json.dumps(data)
+        return hash_str(data)
+
+    def dump(self, data, fid=None, expire=None):
+        exp = int(expire or self.expire_time) + int(time.time())
+        dm_data = {"data": data, "expire": exp}
+        dm_data = json.dumps(dm_data)
+        if not fid:
+            fid = self.get_fid(data=data)
+        fn = self._file_name(fid)
+        # if os.path.exists(fn):
+        #     return fid
+        with FileLock(lock_id=file_lock_prefix + fid, timeout=10):
+            if os.path.exists(fn):
+                os.remove(fn)
+            with open(fn, 'w') as wf:
+                wf.write(dm_data)
+                wf.flush()
+            wf.close()
+        return fid
+
+    def load(self, fid, default=None):
+        fn = self._file_name(fid)
+        if os.path.exists(fn):
+            try:
+                with open(fn, 'r') as rf:
+                    data = json.loads(rf.read())
+                    data = data.get("data")
+                    expire = data.get("expire")
+                    if expire and expire > int(time.time()):
+                        os.remove(fn)
+                        data = default
+                rf.close()
+            except Exception as E:
+                print(E)
+                os.remove(fn)
+                data = default
+        else:
+            data = default
+        return data
+
+
 class FileLock:
     """
     使用文件操作实现的异步锁
 
     使用方式：
     with FileLock(lock_id='xxxx', timeout=xx.xx):
         do_the_jobs()
```

### Comparing `angeltools-0.2.9/angeltools/TimeTool.py` & `angeltools-0.3.1/angeltools/TimeTool.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools/commands.py` & `angeltools-0.3.1/angeltools/commands.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools/fdfs/fdfs_client/client.py` & `angeltools-0.3.1/angeltools/fdfs/fdfs_client/client.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools/fdfs/fdfs_client/connection.py` & `angeltools-0.3.1/angeltools/fdfs/fdfs_client/connection.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools/fdfs/fdfs_client/fdfs_protol.py` & `angeltools-0.3.1/angeltools/fdfs/fdfs_client/fdfs_protol.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools/fdfs/fdfs_client/fdfs_test.py` & `angeltools-0.3.1/angeltools/fdfs/fdfs_client/fdfs_test.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools/fdfs/fdfs_client/storage_client.py` & `angeltools-0.3.1/angeltools/fdfs/fdfs_client/storage_client.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools/fdfs/fdfs_client/tracker_client.py` & `angeltools-0.3.1/angeltools/fdfs/fdfs_client/tracker_client.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools/fdfs/fdfs_client/utils.py` & `angeltools-0.3.1/angeltools/fdfs/fdfs_client/utils.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools/fdfs/fdfs_operator.py` & `angeltools-0.3.1/angeltools/fdfs/fdfs_operator.py`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/angeltools.egg-info/PKG-INFO` & `angeltools-0.3.1/angeltools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angeltools
-Version: 0.2.9
+Version: 0.3.1
 Summary: personal python small tools collection
 Home-page: https://github.com/ga1008/angeltools
 Author: Guardian
 Author-email: zhling2012@live.com
 Maintainer: Guardian
 Maintainer-email: zhling2012@live.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `angeltools-0.2.9/angeltools.egg-info/SOURCES.txt` & `angeltools-0.3.1/angeltools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `angeltools-0.2.9/setup.py` & `angeltools-0.3.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 using_setuptools = True
 
 setup_args = {
     "name": "angeltools",
-    "version": "0.2.9",
+    "version": "0.3.1",
     "url": "https://github.com/ga1008/angeltools",
     "description": "personal python small tools collection",
     "long_description": long_description,
     "author": "Guardian",
     "author_email": "zhling2012@live.com",
     "maintainer": "Guardian",
     "maintainer_email": "zhling2012@live.com",
```

