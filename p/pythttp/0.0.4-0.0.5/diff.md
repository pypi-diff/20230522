# Comparing `tmp/pythttp-0.0.4.tar.gz` & `tmp/pythttp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythttp-0.0.4.tar", last modified: Mon May 22 10:14:26 2023, max compression
+gzip compressed data, was "pythttp-0.0.5.tar", last modified: Mon May 22 10:19:32 2023, max compression
```

## Comparing `pythttp-0.0.4.tar` & `pythttp-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 10:14:26.836784 pythttp-0.0.4/
--rw-rw-rw-   0        0        0     1093 2023-05-22 10:14:26.835685 pythttp-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.0.4/README.md
--rw-rw-rw-   0        0        0      419 2023-05-22 10:14:19.000000 pythttp-0.0.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-22 10:14:26.823973 pythttp-0.0.4/pythttp/
--rw-rw-rw-   0        0        0      726 2023-05-03 09:20:58.000000 pythttp-0.0.4/pythttp/Log_Manager.py
--rw-rw-rw-   0        0        0     6616 2023-05-22 10:13:01.000000 pythttp-0.0.4/pythttp/Protocol.py
--rw-rw-rw-   0        0        0     2732 2023-05-17 09:20:38.000000 pythttp-0.0.4/pythttp/Structure.py
--rw-rw-rw-   0        0        0     2996 2023-05-03 09:21:16.000000 pythttp-0.0.4/pythttp/Thread_Manager.py
--rw-rw-rw-   0        0        0      108 2023-05-22 10:13:49.000000 pythttp-0.0.4/pythttp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 10:14:26.834684 pythttp-0.0.4/pythttp.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-05-22 10:14:26.000000 pythttp-0.0.4/pythttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-22 10:14:26.000000 pythttp-0.0.4/pythttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 10:14:26.000000 pythttp-0.0.4/pythttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 10:14:26.000000 pythttp-0.0.4/pythttp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 10:14:26.836784 pythttp-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-05-22 10:14:23.000000 pythttp-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:19:32.575596 pythttp-0.0.5/
+-rw-rw-rw-   0        0        0     1093 2023-05-22 10:19:32.574597 pythttp-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.0.5/README.md
+-rw-rw-rw-   0        0        0      419 2023-05-22 10:19:19.000000 pythttp-0.0.5/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-22 10:19:32.558035 pythttp-0.0.5/pythttp/
+-rw-rw-rw-   0        0        0      726 2023-05-03 09:20:58.000000 pythttp-0.0.5/pythttp/Log_Manager.py
+-rw-rw-rw-   0        0        0     6666 2023-05-22 10:18:35.000000 pythttp-0.0.5/pythttp/Protocol.py
+-rw-rw-rw-   0        0        0     2732 2023-05-17 09:20:38.000000 pythttp-0.0.5/pythttp/Structure.py
+-rw-rw-rw-   0        0        0     3002 2023-05-22 10:19:02.000000 pythttp-0.0.5/pythttp/Thread_Manager.py
+-rw-rw-rw-   0        0        0      108 2023-05-22 10:13:49.000000 pythttp-0.0.5/pythttp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:19:32.573596 pythttp-0.0.5/pythttp.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-05-22 10:19:32.000000 pythttp-0.0.5/pythttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-22 10:19:32.000000 pythttp-0.0.5/pythttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 10:19:32.000000 pythttp-0.0.5/pythttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 10:19:32.000000 pythttp-0.0.5/pythttp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 10:19:32.575596 pythttp-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-05-22 10:19:26.000000 pythttp-0.0.5/setup.py
```

### Comparing `pythttp-0.0.4/PKG-INFO` & `pythttp-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.0.4/README.md` & `pythttp-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.4/pythttp/Log_Manager.py` & `pythttp-0.0.5/pythttp/Log_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.4/pythttp/Protocol.py` & `pythttp-0.0.5/pythttp/Protocol.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import socket
 from urllib import request
 from urllib import parse
 import Thread_Manager
-from Structure import *
-from Log_Manager import *
+import Structure 
+import Log_Manager 
 
 class HyperTextTransferProtocol:
     def __init__(self):
         self.head = bytes()
         self.recv_datas = bytes()
         self.s = socket.socket()
         self.Thread=Thread_Manager.Thread()
-        self.log=Log().logging
+        self.log=Log_Manager.Log().logging
         self.Content_Length=''
-        self.DB=DBManager()
+        self.DB=Structure.DBManager()
 
     def get(self, url: str, port: int = 80, params: dict = None):
         try:
             self.s.connect((url, port))
-            headers = PrepareHeader()._prepare_request_headers('GET', url, params)
+            headers = Structure.PrepareHeader()._prepare_request_headers('GET', url, params)
             self.s.send(headers.encode())
             return self.receive()
         except ConnectionRefusedError as e:
             print(f'Request to server failed... Reason: {e}')
         finally:
             self.s.close()
 
@@ -112,32 +112,32 @@
             elif '/upload_from' == result:
                 Response= self.HandleTextFileRequest('/upload_from.html')
             return Response
         except FileNotFoundError:
             with open('resource/Hello world.html','r') as arg:
                 print(f'해당 resource{result}파일을 찾을수 없습니다.')
                 Error_Response=arg.read().format(msg=f'해당 resource{result}파일을 찾을수 없습니다.').encode('utf-8')
-                return PrepareHeader()._response_headers('404 Not Found',Error_Response) + Error_Response
+                return Structure.PrepareHeader()._response_headers('404 Not Found',Error_Response) + Error_Response
 
     def ExtractPostBodySize(self, header):
         content_length_header = next((header for header in header if 'Content-Length' in header), None)
         if content_length_header:
             content_length_str = ''.join(filter(str.isdigit, content_length_header))
             return int(content_length_str)
         return 0
         
     def HandleFileRequest(self,img_file='/a.png'):
         with open(f'resource{img_file}', 'rb') as ImgFile:
             Response_file=ImgFile.read()
-            return PrepareHeader()._response_headers('200 OK',Response_file) + Response_file
+            return Structure.PrepareHeader()._response_headers('200 OK',Response_file) + Response_file
         
     def HandleTextFileRequest(self,flie='/Hello world.html', query='아무튼 웹 서버임'):
         with open(f'resource{flie}','r') as TextFile:
             Response_file=TextFile.read().format(msg=query,ImgFiles='<img src="a.png" alt="적당한사진">')
-        return PrepareHeader()._response_headers('200 OK',Response_file) + Response_file.encode('utf-8')
+        return Structure.PrepareHeader()._response_headers('200 OK',Response_file) + Response_file.encode('utf-8')
     
     def ImgFileUpload(self,img_file,file_name):
         #self.DB.loadDB()
         with open(f'resource/ImgFileUpload/{file_name}', 'wb') as ImgFile:
             ImgFile.write(img_file)
             self.DB.ServerDB['Img']={file_name:f'/ImgFileUpload/{file_name}'}
             #self.DB.SaveDB()
```

### Comparing `pythttp-0.0.4/pythttp/Structure.py` & `pythttp-0.0.5/pythttp/Structure.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.4/pythttp/Thread_Manager.py` & `pythttp-0.0.5/pythttp/Thread_Manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import threading
-from Log_Manager import *
+import Log_Manager 
 
 
 class THREAD_PRESET(threading.Thread):
     def __init__(self, target, args=() , daemon=False):
         super(THREAD_PRESET, self).__init__()
         self.target = target
         self.args = args
@@ -26,15 +26,15 @@
         self.USERS=Thread_DataManager().USERS
         self.SESSIONS=Thread_DataManager().SESSIONS
         self.USERS_COUNT=Thread_DataManager().USERS_COUNT
         self.THREADS_COUNT=0
         self.user_socket_dict={}
         self.stopped_threads={}
         self.finished_users=[]
-        self.log=Log().logging
+        self.log=Log_Manager.Log().logging
 
     def display_variables(self):
         LIST_VARIABLES=f'''
                             'SESSIONS':{self.SESSIONS},
                             'USERS':{self.USERS},
                             'USERS_COUNT':{self.USERS_COUNT},
                             'ACTIVATED_THREADS':{self.ACTIVATED_THREADS},
```

### Comparing `pythttp-0.0.4/pythttp.egg-info/PKG-INFO` & `pythttp-0.0.5/pythttp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.0.4/setup.py` & `pythttp-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open(r"README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythttp",
-    version="0.0.4",
+    version="0.0.5",
     author="Example Author",
     author_email="team.longinus.project@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/projectlonginus/httpy",
     install_requires=[],
```

