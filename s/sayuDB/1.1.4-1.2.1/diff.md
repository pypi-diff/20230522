# Comparing `tmp/sayuDB-1.1.4.tar.gz` & `tmp/sayuDB-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sayuDB-1.1.4.tar", last modified: Thu May 18 13:49:58 2023, max compression
+gzip compressed data, was "sayuDB-1.2.1.tar", last modified: Mon May 22 19:02:33 2023, max compression
```

## Comparing `sayuDB-1.1.4.tar` & `sayuDB-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 13:49:58.520741 sayuDB-1.1.4/
--rw-rw-rw-   0        0        0     1085 2023-04-23 05:32:47.000000 sayuDB-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     9981 2023-05-18 13:49:58.519748 sayuDB-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    10068 2023-05-15 18:43:51.000000 sayuDB-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 13:49:58.498263 sayuDB-1.1.4/sayuDB/
--rw-rw-rw-   0        0        0     2525 2023-05-18 13:08:16.000000 sayuDB-1.1.4/sayuDB/SQLite.py
--rw-rw-rw-   0        0        0     1551 2023-05-18 13:13:51.000000 sayuDB-1.1.4/sayuDB/__init__.py
--rw-rw-rw-   0        0        0     4911 2023-05-18 13:20:28.000000 sayuDB-1.1.4/sayuDB/__main__.py
--rw-rw-rw-   0        0        0    21637 2023-05-18 13:04:44.000000 sayuDB-1.1.4/sayuDB/processor.py
--rw-rw-rw-   0        0        0     2042 2023-04-23 05:32:47.000000 sayuDB-1.1.4/sayuDB/remote.py
--rw-rw-rw-   0        0        0     3252 2023-05-18 13:48:02.000000 sayuDB-1.1.4/sayuDB/server.py
-drwxrwxrwx   0        0        0        0 2023-05-18 13:49:58.518565 sayuDB-1.1.4/sayuDB.egg-info/
--rw-rw-rw-   0        0        0     9981 2023-05-18 13:49:58.000000 sayuDB-1.1.4/sayuDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-05-18 13:49:58.000000 sayuDB-1.1.4/sayuDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 13:49:58.000000 sayuDB-1.1.4/sayuDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       78 2023-05-18 13:49:58.000000 sayuDB-1.1.4/sayuDB.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2023-05-18 13:49:58.000000 sayuDB-1.1.4/sayuDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-18 13:49:58.000000 sayuDB-1.1.4/sayuDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 13:49:58.520741 sayuDB-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0    10344 2023-05-18 13:48:28.000000 sayuDB-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:02:33.581076 sayuDB-1.2.1/
+-rw-rw-rw-   0        0        0     1085 2023-04-23 05:32:47.000000 sayuDB-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     9981 2023-05-22 19:02:33.580082 sayuDB-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10068 2023-05-15 18:43:51.000000 sayuDB-1.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 19:02:33.543880 sayuDB-1.2.1/sayuDB/
+-rw-rw-rw-   0        0        0     2575 2023-05-22 19:01:12.000000 sayuDB-1.2.1/sayuDB/SQLite.py
+-rw-rw-rw-   0        0        0     1551 2023-05-18 13:13:51.000000 sayuDB-1.2.1/sayuDB/__init__.py
+-rw-rw-rw-   0        0        0     4911 2023-05-18 13:20:28.000000 sayuDB-1.2.1/sayuDB/__main__.py
+-rw-rw-rw-   0        0        0    21637 2023-05-18 13:04:44.000000 sayuDB-1.2.1/sayuDB/processor.py
+-rw-rw-rw-   0        0        0     2042 2023-04-23 05:32:47.000000 sayuDB-1.2.1/sayuDB/remote.py
+-rw-rw-rw-   0        0        0     3252 2023-05-18 13:48:02.000000 sayuDB-1.2.1/sayuDB/server.py
+drwxrwxrwx   0        0        0        0 2023-05-22 19:02:33.578088 sayuDB-1.2.1/sayuDB.egg-info/
+-rw-rw-rw-   0        0        0     9981 2023-05-22 19:02:33.000000 sayuDB-1.2.1/sayuDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-05-22 19:02:33.000000 sayuDB-1.2.1/sayuDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 19:02:33.000000 sayuDB-1.2.1/sayuDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       78 2023-05-22 19:02:33.000000 sayuDB-1.2.1/sayuDB.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-05-22 19:02:33.000000 sayuDB-1.2.1/sayuDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-22 19:02:33.000000 sayuDB-1.2.1/sayuDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 19:02:33.581076 sayuDB-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0    10344 2023-05-22 19:01:46.000000 sayuDB-1.2.1/setup.py
```

### Comparing `sayuDB-1.1.4/LICENSE` & `sayuDB-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sayuDB-1.1.4/PKG-INFO` & `sayuDB-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sayuDB
-Version: 1.1.4
+Version: 1.2.1
 Summary: Database management system based on python and JSON.
 Home-page: https://github.com/Arsybai/sayuDB
 Author: Arsybai
 Author-email: me@arsybai.com
 License: MIT
 Keywords: database
 Description-Content-Type: text/markdown
```

### Comparing `sayuDB-1.1.4/README.md` & `sayuDB-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sayuDB-1.1.4/sayuDB/SQLite.py` & `sayuDB-1.2.1/sayuDB/SQLite.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 class sql:
 
     def __init__(self, database:str, as_json:bool=False, auto_commit:bool=True) -> None:
         self.as_json = as_json
         self.auto_commit = auto_commit
         if as_json:
-            self.connection = sqlite3.connect(f'{os.path.dirname(__file__)}/sql/{database}.db')
+            self.connection = sqlite3.connect(f'{os.path.dirname(__file__)}/sql/{database}.db', check_same_thread=False)
             self.connection.row_factory = dict_factory
         else:
-            self.connection = sqlite3.connect(f'{os.path.dirname(__file__)}/sql/{database}.db')
+            self.connection = sqlite3.connect(f'{os.path.dirname(__file__)}/sql/{database}.db', check_same_thread=False)
         pass
 
     def execute(self, query, param=None):
         try:
             if param != None:
                 response = self.connection.execute(query, param)
             else:
```

### Comparing `sayuDB-1.1.4/sayuDB/__init__.py` & `sayuDB-1.2.1/sayuDB/__init__.py`

 * *Files identical despite different names*

### Comparing `sayuDB-1.1.4/sayuDB/__main__.py` & `sayuDB-1.2.1/sayuDB/__main__.py`

 * *Files identical despite different names*

### Comparing `sayuDB-1.1.4/sayuDB/processor.py` & `sayuDB-1.2.1/sayuDB/processor.py`

 * *Files identical despite different names*

### Comparing `sayuDB-1.1.4/sayuDB/remote.py` & `sayuDB-1.2.1/sayuDB/remote.py`

 * *Files identical despite different names*

### Comparing `sayuDB-1.1.4/sayuDB/server.py` & `sayuDB-1.2.1/sayuDB/server.py`

 * *Files identical despite different names*

### Comparing `sayuDB-1.1.4/sayuDB.egg-info/PKG-INFO` & `sayuDB-1.2.1/sayuDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sayuDB
-Version: 1.1.4
+Version: 1.2.1
 Summary: Database management system based on python and JSON.
 Home-page: https://github.com/Arsybai/sayuDB
 Author: Arsybai
 Author-email: me@arsybai.com
 License: MIT
 Keywords: database
 Description-Content-Type: text/markdown
```

### Comparing `sayuDB-1.1.4/setup.py` & `sayuDB-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="sayuDB",
-    version="1.1.4",
+    version="1.2.1",
     author="Arsybai",
     description="Database management system based on python and JSON.",
     packages=["sayuDB"],
     license="MIT",
     author_email="me@arsybai.com",
     url="https://github.com/Arsybai/sayuDB",
     keywords=[
```

