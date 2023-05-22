# Comparing `tmp/pythttp-0.0.6.tar.gz` & `tmp/pythttp-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythttp-0.0.6.tar", last modified: Mon May 22 10:25:54 2023, max compression
+gzip compressed data, was "pythttp-0.0.7.tar", last modified: Mon May 22 10:28:32 2023, max compression
```

## Comparing `pythttp-0.0.6.tar` & `pythttp-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 10:25:54.518541 pythttp-0.0.6/
--rw-rw-rw-   0        0        0     1093 2023-05-22 10:25:54.518541 pythttp-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.0.6/README.md
--rw-rw-rw-   0        0        0      419 2023-05-22 10:25:21.000000 pythttp-0.0.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-22 10:25:54.507594 pythttp-0.0.6/pythttp/
--rw-rw-rw-   0        0        0      726 2023-05-03 09:20:58.000000 pythttp-0.0.6/pythttp/Log_Manager.py
--rw-rw-rw-   0        0        0     6611 2023-05-22 10:25:00.000000 pythttp-0.0.6/pythttp/Protocol.py
--rw-rw-rw-   0        0        0     2732 2023-05-17 09:20:38.000000 pythttp-0.0.6/pythttp/Structure.py
--rw-rw-rw-   0        0        0     3009 2023-05-22 10:24:50.000000 pythttp-0.0.6/pythttp/Thread_Manager.py
--rw-rw-rw-   0        0        0      108 2023-05-22 10:13:49.000000 pythttp-0.0.6/pythttp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-22 10:25:54.516359 pythttp-0.0.6/pythttp.egg-info/
--rw-rw-rw-   0        0        0     1093 2023-05-22 10:25:54.000000 pythttp-0.0.6/pythttp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-05-22 10:25:54.000000 pythttp-0.0.6/pythttp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 10:25:54.000000 pythttp-0.0.6/pythttp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 10:25:54.000000 pythttp-0.0.6/pythttp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 10:25:54.518541 pythttp-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      603 2023-05-22 10:25:12.000000 pythttp-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:28:32.386756 pythttp-0.0.7/
+-rw-rw-rw-   0        0        0     1093 2023-05-22 10:28:32.385753 pythttp-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-05-03 09:40:52.000000 pythttp-0.0.7/README.md
+-rw-rw-rw-   0        0        0      419 2023-05-22 10:28:29.000000 pythttp-0.0.7/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-22 10:28:32.374119 pythttp-0.0.7/pythttp/
+-rw-rw-rw-   0        0        0      726 2023-05-03 09:20:58.000000 pythttp-0.0.7/pythttp/Log_Manager.py
+-rw-rw-rw-   0        0        0     6611 2023-05-22 10:25:00.000000 pythttp-0.0.7/pythttp/Protocol.py
+-rw-rw-rw-   0        0        0     2732 2023-05-17 09:20:38.000000 pythttp-0.0.7/pythttp/Structure.py
+-rw-rw-rw-   0        0        0     2997 2023-05-22 10:27:50.000000 pythttp-0.0.7/pythttp/Thread_Manager.py
+-rw-rw-rw-   0        0        0      108 2023-05-22 10:13:49.000000 pythttp-0.0.7/pythttp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:28:32.385753 pythttp-0.0.7/pythttp.egg-info/
+-rw-rw-rw-   0        0        0     1093 2023-05-22 10:28:32.000000 pythttp-0.0.7/pythttp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-05-22 10:28:32.000000 pythttp-0.0.7/pythttp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 10:28:32.000000 pythttp-0.0.7/pythttp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 10:28:32.000000 pythttp-0.0.7/pythttp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 10:28:32.386756 pythttp-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      603 2023-05-22 10:28:19.000000 pythttp-0.0.7/setup.py
```

### Comparing `pythttp-0.0.6/PKG-INFO` & `pythttp-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.0.6/README.md` & `pythttp-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.6/pythttp/Log_Manager.py` & `pythttp-0.0.7/pythttp/Log_Manager.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.6/pythttp/Protocol.py` & `pythttp-0.0.7/pythttp/Protocol.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.6/pythttp/Structure.py` & `pythttp-0.0.7/pythttp/Structure.py`

 * *Files identical despite different names*

### Comparing `pythttp-0.0.6/pythttp/Thread_Manager.py` & `pythttp-0.0.7/pythttp/Thread_Manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.USERS=Thread_DataManager().USERS
         self.SESSIONS=Thread_DataManager().SESSIONS
         self.USERS_COUNT=Thread_DataManager().USERS_COUNT
         self.THREADS_COUNT=0
         self.user_socket_dict={}
         self.stopped_threads={}
         self.finished_users=[]
-        self.log=Log_Manager.Log().logging
+        self.log=Log().logging
 
     def display_variables(self):
         LIST_VARIABLES=f'''
                             'SESSIONS':{self.SESSIONS},
                             'USERS':{self.USERS},
                             'USERS_COUNT':{self.USERS_COUNT},
                             'ACTIVATED_THREADS':{self.ACTIVATED_THREADS},
```

### Comparing `pythttp-0.0.6/pythttp.egg-info/PKG-INFO` & `pythttp-0.0.7/pythttp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pythttp
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/httpy
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/httpy
 Project-URL: Bug Tracker, https://github.com/projectlonginus/httpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pythttp-0.0.6/setup.py` & `pythttp-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open(r"README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pythttp",
-    version="0.0.6",
+    version="0.0.7",
     author="Example Author",
     author_email="team.longinus.project@gmail.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/projectlonginus/httpy",
     install_requires=[],
```

