# Comparing `tmp/fastapi_easy_cache-0.1.0.tar.gz` & `tmp/fastapi_easy_cache-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_easy_cache-0.1.0.tar", max compression
+gzip compressed data, was "fastapi_easy_cache-0.1.1.tar", max compression
```

## Comparing `fastapi_easy_cache-0.1.0.tar` & `fastapi_easy_cache-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1901 2022-10-13 01:45:08.975849 fastapi_easy_cache-0.1.0/README.md
--rw-r--r--   0        0        0       27 2022-10-13 01:33:34.529473 fastapi_easy_cache-0.1.0/fastapi_easy_cache/__init__.py
--rw-r--r--   0        0        0     3457 2022-10-12 23:42:33.320937 fastapi_easy_cache-0.1.0/fastapi_easy_cache/fastapiCache.py
--rw-r--r--   0        0        0      352 2022-10-13 01:46:51.469386 fastapi_easy_cache-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2511 1970-01-01 00:00:00.000000 fastapi_easy_cache-0.1.0/setup.py
--rw-r--r--   0        0        0     2463 1970-01-01 00:00:00.000000 fastapi_easy_cache-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1786 2023-05-21 23:27:29.535697 fastapi_easy_cache-0.1.1/README.md
+-rw-r--r--   0        0        0       27 2023-05-21 23:06:18.549908 fastapi_easy_cache-0.1.1/fastapi_easy_cache/__init__.py
+-rw-r--r--   0        0        0     3496 2023-05-21 23:14:12.499002 fastapi_easy_cache-0.1.1/fastapi_easy_cache/fastapiCache.py
+-rw-r--r--   0        0        0      342 2023-05-21 23:31:51.966617 fastapi_easy_cache-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2302 1970-01-01 00:00:00.000000 fastapi_easy_cache-0.1.1/PKG-INFO
```

### Comparing `fastapi_easy_cache-0.1.0/README.md` & `fastapi_easy_cache-0.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Fastapi easy cache
 
 <hr>
-An easy to use tool for caching fastapi response
+An easy to use tool for caching fastapi returnings
 
 ### When should I use fastapi-easy-cache?
 1. Returning json serializable data
 2. Using GET method
 3. Returning dynamic but repeated data (like data refresh everyday)
 4. Don't have complicated requirements and too lazy to build a tool yourself
 
@@ -29,20 +29,19 @@
 
 The following code will
 1. create a sqlite database in **dbPath**
 2. using peformance mode when calculating route identifier
 ```python
 import fastapi_easy_cache
 
-fastapi_easy_cache.apiCache(dbPath='cachedb/cache.db',
-                              peformance_or_capacity='peformance')
+fastapi_easy_cache.apiCache(db_path='./temp/cache', in_memory=False)
 ```
 #### args
-    dbPath: path to sqlite database, expected str
-    peformance_or_capacity (optional): more peformance or capacity when calculating route id, epected 'peformance' or 'capacity'
+db_path: path to sqlite database
+in_memory: set up cache in memory, db_path will be database name when set to True
 
 
 ### Using
 You just need to add `@cache(expire=20)` under fastapi route decorator, add flil in expire time and it's all done.
 
 `expire` is counted in second
```

### Comparing `fastapi_easy_cache-0.1.0/fastapi_easy_cache/fastapiCache.py` & `fastapi_easy_cache-0.1.1/fastapi_easy_cache/fastapiCache.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from functools import wraps
-import base64, hashlib
+import hashlib
 import time, sqlite3, json
 
 db = ''
-pOc = ''
 
 # Initializing the module
 class apiCache():
-    def __init__(self, dbPath: str, peformance_or_capacity: str = 'peformance'):
+    def __init__(self, db_path: str, in_memory: bool = False):
         '''This module is for caching fastapi route
 
         This module uses sqlite to cache content, and use md5 as an identifier to each route
         Please note that this module is only for GET request and json serializable data
 
         Args:
-            dbPath: path to sqlite database, expected str
-            peformance_or_capacity: more peformance or capacity when calculating route id, epected 'peformance' or 'capacity'
+            db_path: path to sqlite database, expected str
+            in_memory: set up cache in memory, expected bool
 
         Returns:
             None
         '''
-        global db, pOc
-        db = dbPath
-        pOc = peformance_or_capacity
+        global db
+        if in_memory:
+            db = "file:{dbName}?mode=memory&cache=shared".format(dbName=hashlib.md5(db_path.encode()).hexdigest())
+        else:
+            db = db_path
         conn = sqlite3.connect(db)
 
         initCur = conn.cursor()
         try:
             initCur.execute('''create table fastapicache(identifier varchar, data TEXT, time integer);''')
         except sqlite3.OperationalError:
             initCur.execute('drop table fastapicache')
@@ -77,18 +78,18 @@
     if 'request' in kwargs.keys():
         identifier = str(kwargs['request'].url.path)
         if kwargs['request'].query_params:
             identifier += '?' + str(kwargs['request'].query_params)
     else:
         identifier = func.__name__
 
-    if pOc == 'capacity':
-        identifier = base64.b64encode(hashlib.md5(identifier.encode()).digest())
-    else:
-        identifier = hashlib.md5(identifier.encode()).hexdigest()
+    # identifier took less space
+    # identifier = base64.b64encode(hashlib.md5(identifier.encode()).digest())
+    # identifier took more space
+    identifier = hashlib.md5(identifier.encode()).hexdigest()
 
     return identifier
 
 # Main decorator
 def cache(expire: int):
     def decor(func):
         @wraps(func)
```

### Comparing `fastapi_easy_cache-0.1.0/PKG-INFO` & `fastapi_easy_cache-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: fastapi-easy-cache
-Version: 0.1.0
-Summary: A simple tool for caching fastapi response
-License: MIT
-Author: dregg
+Version: 0.1.1
+Summary: 
+Author: DrEgg
+Author-email: 102451227+SteelDrEgg@users.noreply.github.com
 Requires-Python: >=3.7,<4.0
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Fastapi easy cache
 
 <hr>
-An easy to use tool for caching fastapi response
+An easy to use tool for caching fastapi returnings
 
 ### When should I use fastapi-easy-cache?
 1. Returning json serializable data
 2. Using GET method
 3. Returning dynamic but repeated data (like data refresh everyday)
 4. Don't have complicated requirements and too lazy to build a tool yourself
 
@@ -45,20 +44,19 @@
 
 The following code will
 1. create a sqlite database in **dbPath**
 2. using peformance mode when calculating route identifier
 ```python
 import fastapi_easy_cache
 
-fastapi_easy_cache.apiCache(dbPath='cachedb/cache.db',
-                              peformance_or_capacity='peformance')
+fastapi_easy_cache.apiCache(db_path='./temp/cache', in_memory=False)
 ```
 #### args
-    dbPath: path to sqlite database, expected str
-    peformance_or_capacity (optional): more peformance or capacity when calculating route id, epected 'peformance' or 'capacity'
+db_path: path to sqlite database
+in_memory: set up cache in memory, db_path will be database name when set to True
 
 
 ### Using
 You just need to add `@cache(expire=20)` under fastapi route decorator, add flil in expire time and it's all done.
 
 `expire` is counted in second
```

