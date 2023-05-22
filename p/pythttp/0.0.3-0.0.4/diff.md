# Comparing `tmp/pythttp-0.0.3.tar.gz` & `tmp/pythttp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythttp-0.0.3.tar", last modified: Mon May 22 10:06:55 2023, max compression
+gzip compressed data, was "pythttp-0.0.4.tar", last modified: Mon May 22 10:14:26 2023, max compression
```

## Comparing `pythttp-0.0.3.tar` & `pythttp-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 10:06:55.114865 pythttp-0.0.3/
--rw-rw-rw-   0        0        0     1093 2023-05-22 10:06:55.113865 pythttp-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.0.3/README.md
--rw-rw-rw-   0        0        0      419 2023-05-22 10:06:41.000000 pythttp-0.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-22 10:06:55.096681 pythttp-0.0.3/pythttp/
--rw-rw-rw-   0        0        0      726 2023-05-03 09:20:58.000000 pythttp-0.0.3/pythttp/Log_Manager.py
--rw-rw-rw-   0        0        0     6610 2023-05-22 09:54:38.000000 pythttp-0.0.3/pythttp/Protocol.py
--rw-rw-rw-   0        0        0     2732 2023-05-17 09:20:38.000000 pythttp-0.0.3/pythttp/Structure.py
--rw-rw-rw-   0        0        0     2996 2023-05-03 09:21:16.000000 pythttp-0.0.3/pythttp/Thread_Manager.py
--rw-rw-rw-   0        0        0      156 2023-05-03 09:21:32.000000 pythttp-0.0.3/pythttp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 10:06:55.112864 pythttp-0.0.3/pythttp.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-05-22 10:06:55.000000 pythttp-0.0.3/pythttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-22 10:06:55.000000 pythttp-0.0.3/pythttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 10:06:55.000000 pythttp-0.0.3/pythttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 10:06:55.000000 pythttp-0.0.3/pythttp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 10:06:55.114865 pythttp-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-05-22 10:06:47.000000 pythttp-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:14:26.836784 pythttp-0.0.4/
+-rw-rw-rw-   0        0        0     1093 2023-05-22 10:14:26.835685 pythttp-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.0.4/README.md
+-rw-rw-rw-   0        0        0      419 2023-05-22 10:14:19.000000 pythttp-0.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-22 10:14:26.823973 pythttp-0.0.4/pythttp/
+-rw-rw-rw-   0        0        0      726 2023-05-03 09:20:58.000000 pythttp-0.0.4/pythttp/Log_Manager.py
+-rw-rw-rw-   0        0        0     6616 2023-05-22 10:13:01.000000 pythttp-0.0.4/pythttp/Protocol.py
+-rw-rw-rw-   0        0        0     2732 2023-05-17 09:20:38.000000 pythttp-0.0.4/pythttp/Structure.py
+-rw-rw-rw-   0        0        0     2996 2023-05-03 09:21:16.000000 pythttp-0.0.4/pythttp/Thread_Manager.py
+-rw-rw-rw-   0        0        0      108 2023-05-22 10:13:49.000000 pythttp-0.0.4/pythttp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:14:26.834684 pythttp-0.0.4/pythttp.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-05-22 10:14:26.000000 pythttp-0.0.4/pythttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-22 10:14:26.000000 pythttp-0.0.4/pythttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 10:14:26.000000 pythttp-0.0.4/pythttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 10:14:26.000000 pythttp-0.0.4/pythttp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 10:14:26.836784 pythttp-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-05-22 10:14:23.000000 pythttp-0.0.4/setup.py
```

### Comparing `pythttp-0.0.3/PKG-INFO` & `pythttp-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.0.3/README.md` & `pythttp-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.3/pythttp/Log_Manager.py` & `pythttp-0.0.4/pythttp/Log_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.3/pythttp/Protocol.py` & `pythttp-0.0.4/pythttp/Protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import socket
 from urllib import request
 from urllib import parse
-from Thread_Manager import *
+import Thread_Manager
 from Structure import *
 from Log_Manager import *
 
 class HyperTextTransferProtocol:
     def __init__(self):
         self.head = bytes()
         self.recv_datas = bytes()
         self.s = socket.socket()
-        self.Thread=Thread()
+        self.Thread=Thread_Manager.Thread()
         self.log=Log().logging
         self.Content_Length=''
         self.DB=DBManager()
 
     def get(self, url: str, port: int = 80, params: dict = None):
         try:
             self.s.connect((url, port))
@@ -138,8 +138,8 @@
     def ImgFileUpload(self,img_file,file_name):
         #self.DB.loadDB()
         with open(f'resource/ImgFileUpload/{file_name}', 'wb') as ImgFile:
             ImgFile.write(img_file)
             self.DB.ServerDB['Img']={file_name:f'/ImgFileUpload/{file_name}'}
             #self.DB.SaveDB()
             return file_name
-        
+
```

### Comparing `pythttp-0.0.3/pythttp/Structure.py` & `pythttp-0.0.4/pythttp/Structure.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.3/pythttp/Thread_Manager.py` & `pythttp-0.0.4/pythttp/Thread_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.3/pythttp.egg-info/PKG-INFO` & `pythttp-0.0.4/pythttp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.0.3
+Version: 0.0.4
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.0.3/setup.py` & `pythttp-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open(r"README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythttp",
-    version="0.0.3",
+    version="0.0.4",
     author="Example Author",
     author_email="team.longinus.project@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/projectlonginus/httpy",
     install_requires=[],
```

