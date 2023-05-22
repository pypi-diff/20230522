# Comparing `tmp/list-cli-0.1.3.tar.gz` & `tmp/list-cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list-cli-0.1.3.tar", last modified: Wed May 17 03:59:02 2023, max compression
+gzip compressed data, was "list-cli-0.1.4.tar", last modified: Mon May 22 17:15:30 2023, max compression
```

## Comparing `list-cli-0.1.3.tar` & `list-cli-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-17 03:59:02.770222 list-cli-0.1.3/
--rw-r--r--   0 jzaleski   (501) staff       (20)     1076 2023-05-15 02:28:40.000000 list-cli-0.1.3/LICENSE
--rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-17 03:59:02.770298 list-cli-0.1.3/PKG-INFO
--rw-r--r--   0 jzaleski   (501) staff       (20)     2569 2023-05-15 02:28:40.000000 list-cli-0.1.3/README.md
-drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-17 03:59:02.769414 list-cli-0.1.3/list_cli/
--rw-r--r--   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:28:18.000000 list-cli-0.1.3/list_cli/__init__.py
--rw-r--r--   0 jzaleski   (501) staff       (20)     1659 2023-05-17 03:52:05.000000 list-cli-0.1.3/list_cli/__main__.py
--rw-r--r--   0 jzaleski   (501) staff       (20)       22 2023-05-17 03:58:31.000000 list-cli-0.1.3/list_cli/__version__.py
--rw-r--r--   0 jzaleski   (501) staff       (20)    12165 2023-05-17 03:54:01.000000 list-cli-0.1.3/list_cli/processors.py
--rw-r--r--   0 jzaleski   (501) staff       (20)      786 2023-05-17 03:52:47.000000 list-cli-0.1.3/list_cli/results.py
-drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-17 03:59:02.770083 list-cli-0.1.3/list_cli.egg-info/
--rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-17 03:59:02.000000 list-cli-0.1.3/list_cli.egg-info/PKG-INFO
--rw-r--r--   0 jzaleski   (501) staff       (20)      308 2023-05-17 03:59:02.000000 list-cli-0.1.3/list_cli.egg-info/SOURCES.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)        1 2023-05-17 03:59:02.000000 list-cli-0.1.3/list_cli.egg-info/dependency_links.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)       52 2023-05-17 03:59:02.000000 list-cli-0.1.3/list_cli.egg-info/entry_points.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)        9 2023-05-17 03:59:02.000000 list-cli-0.1.3/list_cli.egg-info/top_level.txt
--rw-r--r--   0 jzaleski   (501) staff       (20)       79 2023-05-17 03:59:02.770512 list-cli-0.1.3/setup.cfg
--rw-r--r--   0 jzaleski   (501) staff       (20)     1741 2023-05-15 18:28:18.000000 list-cli-0.1.3/setup.py
+drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-22 17:15:30.313138 list-cli-0.1.4/
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1076 2023-05-15 02:28:40.000000 list-cli-0.1.4/LICENSE
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-22 17:15:30.313207 list-cli-0.1.4/PKG-INFO
+-rw-r--r--   0 jzaleski   (501) staff       (20)     2569 2023-05-15 02:28:40.000000 list-cli-0.1.4/README.md
+drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-22 17:15:30.312411 list-cli-0.1.4/list_cli/
+-rw-r--r--   0 jzaleski   (501) staff       (20)        0 2023-05-15 18:28:18.000000 list-cli-0.1.4/list_cli/__init__.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1659 2023-05-17 03:52:05.000000 list-cli-0.1.4/list_cli/__main__.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)       22 2023-05-18 21:29:58.000000 list-cli-0.1.4/list_cli/__version__.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)    12180 2023-05-18 21:27:25.000000 list-cli-0.1.4/list_cli/processors.py
+-rw-r--r--   0 jzaleski   (501) staff       (20)      786 2023-05-17 03:52:47.000000 list-cli-0.1.4/list_cli/results.py
+drwxr-xr-x   0 jzaleski   (501) staff       (20)        0 2023-05-22 17:15:30.313014 list-cli-0.1.4/list_cli.egg-info/
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1142 2023-05-22 17:15:30.000000 list-cli-0.1.4/list_cli.egg-info/PKG-INFO
+-rw-r--r--   0 jzaleski   (501) staff       (20)      308 2023-05-22 17:15:30.000000 list-cli-0.1.4/list_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)        1 2023-05-22 17:15:30.000000 list-cli-0.1.4/list_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)       52 2023-05-22 17:15:30.000000 list-cli-0.1.4/list_cli.egg-info/entry_points.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)        9 2023-05-22 17:15:30.000000 list-cli-0.1.4/list_cli.egg-info/top_level.txt
+-rw-r--r--   0 jzaleski   (501) staff       (20)       79 2023-05-22 17:15:30.313407 list-cli-0.1.4/setup.cfg
+-rw-r--r--   0 jzaleski   (501) staff       (20)     1741 2023-05-15 18:28:18.000000 list-cli-0.1.4/setup.py
```

### Comparing `list-cli-0.1.3/LICENSE` & `list-cli-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.3/PKG-INFO` & `list-cli-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: List Management Application (CLI)
 Home-page: https://github.com/jzaleski/list-cli
 Author: Jonathan W. Zaleski
 Author-email: JonathanZaleski@gmail.com
 License: MIT
 Keywords: list,list-cli,tasktodo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `list-cli-0.1.3/README.md` & `list-cli-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.3/list_cli/__main__.py` & `list-cli-0.1.4/list_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.3/list_cli/processors.py` & `list-cli-0.1.4/list_cli/processors.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,20 +163,20 @@
         database_dirname = dirname(database_file_path)
         if database_dirname and not isdir(database_dirname):
             makedirs(database_dirname)
         if not isfile(database_file_path):
             open(database_file_path, 'w').close()
         return True
 
-    def _get_bucket(self, bucket) -> list:
+    def _get_bucket(self, bucket_id) -> list:
         return sorted(
             (
                 datum
                 for datum in self._database
-                if datum['bucket'] == bucket
+                if datum['bucket'] == bucket_id
             ),
             key=lambda datum: datum['updated_timestamp']
         )
 
     def _get_database(self) -> dict:
         database = []
         with open(self._database_file_path) as database_file:
@@ -263,18 +263,18 @@
                 continue
             datum['updated_by_user'] = self._user
             datum['updated_timestamp'] = self._timestamp
             datum['bucket'] = self.REMOVED_BUCKET
             return SuccessResult() if self._write_database() else ErrorResult()
         return ErrorResult()
 
-    def _render(self, bucket) -> Result:
-        bucket = self._get_bucket(bucket)
+    def _render(self, bucket_id) -> Result:
+        bucket = self._get_bucket(bucket_id)
         if not bucket:
-            return Result(had_error=bucket != self.ADDED_BUCKET, had_output=False)
+            return Result(had_error=bucket_id != self.ADDED_BUCKET, had_output=False)
         if self._output_file_path:
             print(f'{self._database_file_path}:{linesep}')
         for datum_index, datum in enumerate(bucket):
             print('%3d. %s' % (datum_index + 1, datum['message']))
         return SuccessResult(had_output=True)
 
     def _touch(self, index=None) -> Result:
```

### Comparing `list-cli-0.1.3/list_cli/results.py` & `list-cli-0.1.4/list_cli/results.py`

 * *Files identical despite different names*

### Comparing `list-cli-0.1.3/list_cli.egg-info/PKG-INFO` & `list-cli-0.1.4/list_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: List Management Application (CLI)
 Home-page: https://github.com/jzaleski/list-cli
 Author: Jonathan W. Zaleski
 Author-email: JonathanZaleski@gmail.com
 License: MIT
 Keywords: list,list-cli,tasktodo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `list-cli-0.1.3/setup.py` & `list-cli-0.1.4/setup.py`

 * *Files identical despite different names*

