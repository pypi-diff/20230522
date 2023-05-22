# Comparing `tmp/newtools-2.2.471.tar.gz` & `tmp/newtools-2.2.475.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/newtools-2.2.471.tar", last modified: Tue May 16 16:12:50 2023, max compression
+gzip compressed data, was "dist/newtools-2.2.475.tar", last modified: Mon May 22 09:59:48 2023, max compression
```

## Comparing `newtools-2.2.471.tar` & `newtools-2.2.475.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-16 16:10:45.000000 newtools-2.2.471/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-05-16 16:12:50.000000 newtools-2.2.471/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-16 16:10:45.000000 newtools-2.2.471/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools/aws/
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/aws/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9641 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/aws/load_partitions.py
--rw-rw-rw-   0 root         (0) root         (0)     6435 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/aws/s3_location.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools/db/
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6912 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/db/athena.py
--rw-rw-rw-   0 root         (0) root         (0)    40091 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/db/cached_query.py
--rw-rw-rw-   0 root         (0) root         (0)    12954 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/db/sql_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools/doggo/
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/doggo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5576 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/doggo/csv.py
--rw-rw-rw-   0 root         (0) root         (0)    13397 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/doggo/doggo.py
--rw-rw-rw-   0 root         (0) root         (0)    19227 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/doggo/fs.py
--rw-rw-rw-   0 root         (0) root         (0)     9277 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/doggo/lock.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools/log/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/log/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9531 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/log/json_persistent_field_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3858 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/log/log.py
--rw-rw-rw-   0 root         (0) root         (0)     2931 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/log/persistent_field_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3452 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/optional_imports.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools/queue/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/queue/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5151 2023-05-16 16:10:45.000000 newtools-2.2.471/newtools/queue/task_queue.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-16 16:12:50.000000 newtools-2.2.471/newtools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-16 16:10:45.000000 newtools-2.2.471/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-16 16:12:50.000000 newtools-2.2.471/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2296 2023-05-16 16:10:45.000000 newtools-2.2.471/setup.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-16 16:12:47.000000 newtools-2.2.471/version.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-05-22 09:57:42.000000 newtools-2.2.475/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-05-22 09:59:48.000000 newtools-2.2.475/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-22 09:57:42.000000 newtools-2.2.475/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools/aws/
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/aws/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9641 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/aws/load_partitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6435 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/aws/s3_location.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools/db/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6912 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/db/athena.py
+-rw-rw-rw-   0 root         (0) root         (0)    40091 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/db/cached_query.py
+-rw-rw-rw-   0 root         (0) root         (0)    12954 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/db/sql_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools/doggo/
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/doggo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5576 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/doggo/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    13423 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/doggo/doggo.py
+-rw-rw-rw-   0 root         (0) root         (0)    19227 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/doggo/fs.py
+-rw-rw-rw-   0 root         (0) root         (0)     9277 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/doggo/lock.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools/log/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/log/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9531 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/log/json_persistent_field_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/log/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/log/persistent_field_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3452 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/optional_imports.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools/queue/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/queue/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5151 2023-05-22 09:57:42.000000 newtools-2.2.475/newtools/queue/task_queue.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-05-22 09:59:48.000000 newtools-2.2.475/newtools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-22 09:57:42.000000 newtools-2.2.475/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-05-22 09:59:48.000000 newtools-2.2.475/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2296 2023-05-22 09:57:42.000000 newtools-2.2.475/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-05-22 09:59:44.000000 newtools-2.2.475/version.txt
```

### Comparing `newtools-2.2.471/PKG-INFO` & `newtools-2.2.475/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newtools
-Version: 2.2.471
+Version: 2.2.475
 Summary: Provides useful libraries for processing large data sets.
 Home-page: https://bitbucket.org/deductive/newtools/
 Author: Deductive
 Author-email: hello@deductive.com
 License: MIT
 Project-URL: Documentation, https://newtools.readthedocs.io/en/latest/
 Project-URL: Source, https://bitbucket.org/deductive/newtools/
```

### Comparing `newtools-2.2.471/README.md` & `newtools-2.2.475/README.md`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/newtools/__init__.py` & `newtools-2.2.475/newtools/__init__.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/newtools/aws/load_partitions.py` & `newtools-2.2.475/newtools/aws/load_partitions.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/newtools/aws/s3_location.py` & `newtools-2.2.475/newtools/aws/s3_location.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/newtools/db/athena.py` & `newtools-2.2.475/newtools/db/athena.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/newtools/db/cached_query.py` & `newtools-2.2.475/newtools/db/cached_query.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/newtools/db/sql_client.py` & `newtools-2.2.475/newtools/db/sql_client.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/newtools/doggo/csv.py` & `newtools-2.2.475/newtools/doggo/csv.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/newtools/doggo/doggo.py` & `newtools-2.2.475/newtools/doggo/doggo.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         """
 
         if boto_session:
             self.s3_client = boto_session.client('s3')
         else:
             self.s3_client = None
 
-        self.dfs = DoggoFileSystem()
+        self.dfs = DoggoFileSystem(boto3_session=boto_session)
         self._logger = logger
 
     @staticmethod
     def _extract_file_format(path):
 
         for part in reversed(path.split(".")[-2:]):
             if part in ('csv', 'parquet', 'pq'):
```

### Comparing `newtools-2.2.471/newtools/doggo/fs.py` & `newtools-2.2.475/newtools/doggo/fs.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/newtools/doggo/lock.py` & `newtools-2.2.475/newtools/doggo/lock.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/newtools/log/json_persistent_field_logger.py` & `newtools-2.2.475/newtools/log/json_persistent_field_logger.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/newtools/log/log.py` & `newtools-2.2.475/newtools/log/log.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/newtools/log/persistent_field_logger.py` & `newtools-2.2.475/newtools/log/persistent_field_logger.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/newtools/optional_imports.py` & `newtools-2.2.475/newtools/optional_imports.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/newtools/queue/task_queue.py` & `newtools-2.2.475/newtools/queue/task_queue.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/newtools.egg-info/PKG-INFO` & `newtools-2.2.475/newtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newtools
-Version: 2.2.471
+Version: 2.2.475
 Summary: Provides useful libraries for processing large data sets.
 Home-page: https://bitbucket.org/deductive/newtools/
 Author: Deductive
 Author-email: hello@deductive.com
 License: MIT
 Project-URL: Documentation, https://newtools.readthedocs.io/en/latest/
 Project-URL: Source, https://bitbucket.org/deductive/newtools/
```

### Comparing `newtools-2.2.471/newtools.egg-info/SOURCES.txt` & `newtools-2.2.475/newtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `newtools-2.2.471/setup.py` & `newtools-2.2.475/setup.py`

 * *Files identical despite different names*

