# Comparing `tmp/rick_vfs-0.1.0.tar.gz` & `tmp/rick_vfs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rick_vfs-0.1.0.tar", last modified: Wed Sep 21 10:59:27 2022, max compression
+gzip compressed data, was "rick_vfs-1.0.0.tar", last modified: Mon May 22 08:35:00 2023, max compression
```

## Comparing `rick_vfs-0.1.0.tar` & `rick_vfs-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-09-21 10:59:27.493053 rick_vfs-0.1.0/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2920 2022-09-21 10:59:27.493053 rick_vfs-0.1.0/PKG-INFO
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1649 2022-09-21 10:53:13.000000 rick_vfs-0.1.0/README.md
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-09-21 10:59:27.493053 rick_vfs-0.1.0/rick_vfs/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       99 2022-09-19 14:41:09.000000 rick_vfs-0.1.0/rick_vfs/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-09-21 10:59:27.493053 rick_vfs-0.1.0/rick_vfs/local/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       58 2022-09-19 17:38:19.000000 rick_vfs-0.1.0/rick_vfs/local/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    13500 2022-09-21 07:18:35.000000 rick_vfs-0.1.0/rick_vfs/local/local.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-09-21 10:59:27.493053 rick_vfs-0.1.0/rick_vfs/s3/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       55 2022-09-19 14:41:09.000000 rick_vfs-0.1.0/rick_vfs/s3/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)    23001 2022-09-21 10:46:02.000000 rick_vfs-0.1.0/rick_vfs/s3/s3.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1567 2022-09-19 16:09:33.000000 rick_vfs-0.1.0/rick_vfs/utils.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       94 2022-09-19 17:38:09.000000 rick_vfs-0.1.0/rick_vfs/version.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2554 2022-09-21 07:18:35.000000 rick_vfs-0.1.0/rick_vfs/vfs.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-09-21 10:59:27.493053 rick_vfs-0.1.0/rick_vfs.egg-info/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2920 2022-09-21 10:59:27.000000 rick_vfs-0.1.0/rick_vfs.egg-info/PKG-INFO
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)      535 2022-09-21 10:59:27.000000 rick_vfs-0.1.0/rick_vfs.egg-info/SOURCES.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2022-09-21 10:59:27.000000 rick_vfs-0.1.0/rick_vfs.egg-info/dependency_links.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        1 2022-09-19 15:48:53.000000 rick_vfs-0.1.0/rick_vfs.egg-info/not-zip-safe
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       23 2022-09-21 10:59:27.000000 rick_vfs-0.1.0/rick_vfs.egg-info/requires.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       15 2022-09-21 10:59:27.000000 rick_vfs-0.1.0/rick_vfs.egg-info/top_level.txt
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)       38 2022-09-21 10:59:27.493053 rick_vfs-0.1.0/setup.cfg
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     1517 2022-09-19 14:41:13.000000 rick_vfs-0.1.0/setup.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-09-21 10:59:27.493053 rick_vfs-0.1.0/tests/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-09-19 15:40:16.000000 rick_vfs-0.1.0/tests/__init__.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-09-21 10:59:27.493053 rick_vfs-0.1.0/tests/local/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-09-19 15:40:28.000000 rick_vfs-0.1.0/tests/local/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     9295 2022-09-21 07:19:36.000000 rick_vfs-0.1.0/tests/local/test_vfs.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     2329 2022-09-21 07:20:22.000000 rick_vfs-0.1.0/tests/local/test_volume.py
-drwxrwxr-x   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-09-21 10:59:27.493053 rick_vfs-0.1.0/tests/s3/
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)        0 2022-09-19 15:40:40.000000 rick_vfs-0.1.0/tests/s3/__init__.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     7405 2022-09-21 10:46:34.000000 rick_vfs-0.1.0/tests/s3/test_vfs.py
--rw-rw-r--   0 jpinheiro  (1000) jpinheiro  (1000)     5323 2022-09-21 07:29:08.000000 rick_vfs-0.1.0/tests/s3/test_volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:35:00.986347 rick_vfs-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-22 08:35:00.986347 rick_vfs-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:35:00.986347 rick_vfs-1.0.0/rick_vfs/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/rick_vfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:35:00.986347 rick_vfs-1.0.0/rick_vfs/local/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/rick_vfs/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13500 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/rick_vfs/local/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:35:00.986347 rick_vfs-1.0.0/rick_vfs/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/rick_vfs/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/rick_vfs/s3/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/rick_vfs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/rick_vfs/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/rick_vfs/vfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:35:00.986347 rick_vfs-1.0.0/rick_vfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-05-22 08:35:00.000000 rick_vfs-1.0.0/rick_vfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-22 08:35:00.000000 rick_vfs-1.0.0/rick_vfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:35:00.000000 rick_vfs-1.0.0/rick_vfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:35:00.000000 rick_vfs-1.0.0/rick_vfs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-22 08:35:00.000000 rick_vfs-1.0.0/rick_vfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-22 08:35:00.000000 rick_vfs-1.0.0/rick_vfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 08:35:00.986347 rick_vfs-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:35:00.986347 rick_vfs-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:35:00.986347 rick_vfs-1.0.0/tests/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/tests/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/tests/local/test_vfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/tests/local/test_volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:35:00.986347 rick_vfs-1.0.0/tests/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/tests/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/tests/s3/test_vfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-22 08:34:42.000000 rick_vfs-1.0.0/tests/s3/test_volume.py
```

### Comparing `rick_vfs-0.1.0/PKG-INFO` & `rick_vfs-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 Metadata-Version: 2.1
 Name: rick_vfs
-Version: 0.1.0
+Version: 1.0.0
 Summary: Minio/S3 client VFS abstraction library
-Home-page: https://github.com/oddbit-project/rick_vfs
+Home-page: https://git.oddbit.org/OddBit/rick_vfs
 Author: Joao Pinheiro
 Author-email: 
 License: BSD
-Description: # rick-vfs
-        
-        Minio/S3 client VFS abstraction library
-        
-        [![Tests](https://github.com/oddbit-project/rick_vfs/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/rick_vfs/actions)
-        [![pypi](https://img.shields.io/pypi/v/rick_vfs.svg)](https://pypi.org/project/rick_vfs/)
-        [![license](https://img.shields.io/pypi/l/rick_vfs.svg)](https://github.com/oddbit-project/rick_vfs/blob/master/LICENSE)
-        
-        Rick-vfs is a high-level abstraction library for file operations on local repositories (a locally accessible folder) and 
-        Minio/S3 object storage systems. The main goal is to provide a set of common interface functions with analogous behaviour,
-        to interact with both scenarios.
-        
-        The intention of "analogous behaviour" is to mimick overall intent and response type, when possible. There will always
-        be differences between invoking a given method on two different backends.
-        
-        
-        
-        Example:
-        ```python
-        from io import BytesIO
-        from minio import Minio
-        from rick_vfs.s3 import MinioBucket, MinioVfs
-        
-        client = Minio(
-            "localhost:9010",
-            secure=False,
-            access_key="SomeTestUser",
-            secret_key="SomeTestPassword",
-        )
-        
-        # initialize bucket
-        volume = MinioBucket(client, 'my-bucket')
-        # initialize VFS object
-        vfs = MinioVfs(volume)
-        
-        # create directory
-        vfs.mkdir("contents/files")
-        
-        # create file from buffer
-        buf = BytesIO(b'the quick brown fox jumps over the lazy dog')
-        vfs.write_file(buf, 'contents/files/my_test_file')
-        
-        # read file
-        contents = vfs.read_file('my_test_file')
-        # print contents
-        print(str(contents.getbuffer().tobytes(), 'utf-8'))
-        
-        # list bucket contents
-        print("Bucket contents:")
-        for item in vfs.ls():
-            print(item.object_name)
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: minio
+License-File: LICENSE
+
+# rick-vfs
+
+Minio/S3 client VFS abstraction library
+
+[![Tests](https://github.com/oddbit-project/rick_vfs/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/rick_vfs/actions)
+[![pypi](https://img.shields.io/pypi/v/rick_vfs.svg)](https://pypi.org/project/rick-vfs/)
+[![license](https://img.shields.io/pypi/l/rick_vfs.svg)](https://git.oddbit.org/OddBit/rick_vfs/src/branch/master/LICENSE)
+
+Rick-vfs is a high-level abstraction library for file operations on local repositories (a locally accessible folder) and 
+Minio/S3 object storage systems. The main goal is to provide a set of common interface functions with analogous behaviour,
+to interact with both scenarios.
+
+The intention of "analogous behaviour" is to mimick overall intent and response type, when possible. There will always
+be differences between invoking a given method on two different backends.
+
+
+
+Example:
+```python
+from io import BytesIO
+from minio import Minio
+from rick_vfs.s3 import MinioBucket, MinioVfs
+
+client = Minio(
+    "localhost:9010",
+    secure=False,
+    access_key="SomeTestUser",
+    secret_key="SomeTestPassword",
+)
+
+# initialize bucket
+volume = MinioBucket(client, 'my-bucket')
+# initialize VFS object
+vfs = MinioVfs(volume)
+
+# create directory
+vfs.mkdir("contents/files")
+
+# create file from buffer
+buf = BytesIO(b'the quick brown fox jumps over the lazy dog')
+vfs.write_file(buf, 'contents/files/my_test_file')
+
+# read file
+contents = vfs.read_file('my_test_file')
+# print contents
+print(str(contents.getbuffer().tobytes(), 'utf-8'))
+
+# list bucket contents
+print("Bucket contents:")
+for item in vfs.ls():
+    print(item.object_name)
+```
```

### Comparing `rick_vfs-0.1.0/README.md` & `rick_vfs-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # rick-vfs
 
 Minio/S3 client VFS abstraction library
 
 [![Tests](https://github.com/oddbit-project/rick_vfs/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/rick_vfs/actions)
-[![pypi](https://img.shields.io/pypi/v/rick_vfs.svg)](https://pypi.org/project/rick_vfs/)
-[![license](https://img.shields.io/pypi/l/rick_vfs.svg)](https://github.com/oddbit-project/rick_vfs/blob/master/LICENSE)
+[![pypi](https://img.shields.io/pypi/v/rick_vfs.svg)](https://pypi.org/project/rick-vfs/)
+[![license](https://img.shields.io/pypi/l/rick_vfs.svg)](https://git.oddbit.org/OddBit/rick_vfs/src/branch/master/LICENSE)
 
 Rick-vfs is a high-level abstraction library for file operations on local repositories (a locally accessible folder) and 
 Minio/S3 object storage systems. The main goal is to provide a set of common interface functions with analogous behaviour,
 to interact with both scenarios.
 
 The intention of "analogous behaviour" is to mimick overall intent and response type, when possible. There will always
 be differences between invoking a given method on two different backends.
```

### Comparing `rick_vfs-0.1.0/rick_vfs/local/local.py` & `rick_vfs-1.0.0/rick_vfs/local/local.py`

 * *Files identical despite different names*

### Comparing `rick_vfs-0.1.0/rick_vfs/s3/s3.py` & `rick_vfs-1.0.0/rick_vfs/s3/s3.py`

 * *Files identical despite different names*

### Comparing `rick_vfs-0.1.0/rick_vfs/utils.py` & `rick_vfs-1.0.0/rick_vfs/utils.py`

 * *Files identical despite different names*

### Comparing `rick_vfs-0.1.0/rick_vfs/vfs.py` & `rick_vfs-1.0.0/rick_vfs/vfs.py`

 * *Files identical despite different names*

### Comparing `rick_vfs-0.1.0/rick_vfs.egg-info/PKG-INFO` & `rick_vfs-1.0.0/rick_vfs.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,74 @@
 Metadata-Version: 2.1
 Name: rick-vfs
-Version: 0.1.0
+Version: 1.0.0
 Summary: Minio/S3 client VFS abstraction library
-Home-page: https://github.com/oddbit-project/rick_vfs
+Home-page: https://git.oddbit.org/OddBit/rick_vfs
 Author: Joao Pinheiro
 Author-email: 
 License: BSD
-Description: # rick-vfs
-        
-        Minio/S3 client VFS abstraction library
-        
-        [![Tests](https://github.com/oddbit-project/rick_vfs/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/rick_vfs/actions)
-        [![pypi](https://img.shields.io/pypi/v/rick_vfs.svg)](https://pypi.org/project/rick_vfs/)
-        [![license](https://img.shields.io/pypi/l/rick_vfs.svg)](https://github.com/oddbit-project/rick_vfs/blob/master/LICENSE)
-        
-        Rick-vfs is a high-level abstraction library for file operations on local repositories (a locally accessible folder) and 
-        Minio/S3 object storage systems. The main goal is to provide a set of common interface functions with analogous behaviour,
-        to interact with both scenarios.
-        
-        The intention of "analogous behaviour" is to mimick overall intent and response type, when possible. There will always
-        be differences between invoking a given method on two different backends.
-        
-        
-        
-        Example:
-        ```python
-        from io import BytesIO
-        from minio import Minio
-        from rick_vfs.s3 import MinioBucket, MinioVfs
-        
-        client = Minio(
-            "localhost:9010",
-            secure=False,
-            access_key="SomeTestUser",
-            secret_key="SomeTestPassword",
-        )
-        
-        # initialize bucket
-        volume = MinioBucket(client, 'my-bucket')
-        # initialize VFS object
-        vfs = MinioVfs(volume)
-        
-        # create directory
-        vfs.mkdir("contents/files")
-        
-        # create file from buffer
-        buf = BytesIO(b'the quick brown fox jumps over the lazy dog')
-        vfs.write_file(buf, 'contents/files/my_test_file')
-        
-        # read file
-        contents = vfs.read_file('my_test_file')
-        # print contents
-        print(str(contents.getbuffer().tobytes(), 'utf-8'))
-        
-        # list bucket contents
-        print("Bucket contents:")
-        for item in vfs.ls():
-            print(item.object_name)
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: minio
+License-File: LICENSE
+
+# rick-vfs
+
+Minio/S3 client VFS abstraction library
+
+[![Tests](https://github.com/oddbit-project/rick_vfs/workflows/Tests/badge.svg?branch=master)](https://github.com/oddbit-project/rick_vfs/actions)
+[![pypi](https://img.shields.io/pypi/v/rick_vfs.svg)](https://pypi.org/project/rick-vfs/)
+[![license](https://img.shields.io/pypi/l/rick_vfs.svg)](https://git.oddbit.org/OddBit/rick_vfs/src/branch/master/LICENSE)
+
+Rick-vfs is a high-level abstraction library for file operations on local repositories (a locally accessible folder) and 
+Minio/S3 object storage systems. The main goal is to provide a set of common interface functions with analogous behaviour,
+to interact with both scenarios.
+
+The intention of "analogous behaviour" is to mimick overall intent and response type, when possible. There will always
+be differences between invoking a given method on two different backends.
+
+
+
+Example:
+```python
+from io import BytesIO
+from minio import Minio
+from rick_vfs.s3 import MinioBucket, MinioVfs
+
+client = Minio(
+    "localhost:9010",
+    secure=False,
+    access_key="SomeTestUser",
+    secret_key="SomeTestPassword",
+)
+
+# initialize bucket
+volume = MinioBucket(client, 'my-bucket')
+# initialize VFS object
+vfs = MinioVfs(volume)
+
+# create directory
+vfs.mkdir("contents/files")
+
+# create file from buffer
+buf = BytesIO(b'the quick brown fox jumps over the lazy dog')
+vfs.write_file(buf, 'contents/files/my_test_file')
+
+# read file
+contents = vfs.read_file('my_test_file')
+# print contents
+print(str(contents.getbuffer().tobytes(), 'utf-8'))
+
+# list bucket contents
+print("Bucket contents:")
+for item in vfs.ls():
+    print(item.object_name)
+```
```

### Comparing `rick_vfs-0.1.0/rick_vfs.egg-info/SOURCES.txt` & `rick_vfs-1.0.0/rick_vfs.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 rick_vfs/__init__.py
 rick_vfs/utils.py
 rick_vfs/version.py
 rick_vfs/vfs.py
 rick_vfs.egg-info/PKG-INFO
```

### Comparing `rick_vfs-0.1.0/setup.py` & `rick_vfs-1.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     description = f.read()
 
 setup(
     name='rick_vfs',
     version=version,
     author="Joao Pinheiro",
     author_email="",
-    url="https://github.com/oddbit-project/rick_vfs",
+    url="https://git.oddbit.org/OddBit/rick_vfs",
     description='Minio/S3 client VFS abstraction library',
     license='BSD',
     long_description=description,
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
@@ -36,15 +36,16 @@
         'Topic :: Software Development :: Libraries :: Application Frameworks',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     long_description_content_type='text/markdown',
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.8",
-    extras_require={
-        "minio": ["minio >= 7.1.11"]
-    },
-    install_requires=[],
+    extras_require={},
+    install_requires=[
+        'python-magic==0.4.27',
+        'minio>=7.1.15',
+    ],
     zip_safe=False,
     tests_require=[
     ],
 )
```

### Comparing `rick_vfs-0.1.0/tests/local/test_vfs.py` & `rick_vfs-1.0.0/tests/local/test_vfs.py`

 * *Files identical despite different names*

### Comparing `rick_vfs-0.1.0/tests/local/test_volume.py` & `rick_vfs-1.0.0/tests/local/test_volume.py`

 * *Files identical despite different names*

### Comparing `rick_vfs-0.1.0/tests/s3/test_vfs.py` & `rick_vfs-1.0.0/tests/s3/test_vfs.py`

 * *Files identical despite different names*

### Comparing `rick_vfs-0.1.0/tests/s3/test_volume.py` & `rick_vfs-1.0.0/tests/s3/test_volume.py`

 * *Files identical despite different names*

