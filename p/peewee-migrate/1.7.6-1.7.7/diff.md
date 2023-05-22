# Comparing `tmp/peewee_migrate-1.7.6.tar.gz` & `tmp/peewee_migrate-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_migrate-1.7.6.tar", max compression
+gzip compressed data, was "peewee_migrate-1.7.7.tar", max compression
```

## Comparing `peewee_migrate-1.7.6.tar` & `peewee_migrate-1.7.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4456 2023-05-22 20:47:41.045604 peewee_migrate-1.7.6/README.rst
--rw-r--r--   0        0        0      146 2023-05-22 20:47:41.045604 peewee_migrate-1.7.6/peewee_migrate/__init__.py
--rw-r--r--   0        0        0       78 2023-05-22 20:47:41.045604 peewee_migrate-1.7.6/peewee_migrate/__main__.py
--rw-r--r--   0        0        0    11979 2023-05-22 20:47:41.045604 peewee_migrate-1.7.6/peewee_migrate/auto.py
--rw-r--r--   0        0        0     6597 2023-05-22 20:47:41.049604 peewee_migrate-1.7.6/peewee_migrate/cli.py
--rw-r--r--   0        0        0      146 2023-05-22 20:47:41.049604 peewee_migrate-1.7.6/peewee_migrate/logs.py
--rw-r--r--   0        0        0    16468 2023-05-22 20:47:41.049604 peewee_migrate-1.7.6/peewee_migrate/migrator.py
--rw-r--r--   0        0        0      461 2023-05-22 20:47:41.049604 peewee_migrate-1.7.6/peewee_migrate/models.py
--rw-r--r--   0        0        0        0 2023-05-22 20:47:41.049604 peewee_migrate-1.7.6/peewee_migrate/py.typed
--rw-r--r--   0        0        0    12235 2023-05-22 20:47:41.049604 peewee_migrate-1.7.6/peewee_migrate/router.py
--rw-r--r--   0        0        0     1723 2023-05-22 20:47:41.049604 peewee_migrate-1.7.6/peewee_migrate/template.py
--rw-r--r--   0        0        0      249 2023-05-22 20:47:41.049604 peewee_migrate-1.7.6/peewee_migrate/types.py
--rw-r--r--   0        0        0     1589 2023-05-22 20:47:41.049604 peewee_migrate-1.7.6/pyproject.toml
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.7.6/PKG-INFO
+-rw-r--r--   0        0        0     4456 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/README.rst
+-rw-r--r--   0        0        0      146 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/__main__.py
+-rw-r--r--   0        0        0    11979 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/auto.py
+-rw-r--r--   0        0        0     6597 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/cli.py
+-rw-r--r--   0        0        0      146 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/logs.py
+-rw-r--r--   0        0        0    16468 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/migrator.py
+-rw-r--r--   0        0        0      461 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/models.py
+-rw-r--r--   0        0        0        0 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/py.typed
+-rw-r--r--   0        0        0    12235 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/router.py
+-rw-r--r--   0        0        0     1709 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/template.py
+-rw-r--r--   0        0        0      249 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/peewee_migrate/types.py
+-rw-r--r--   0        0        0     1589 2023-05-22 21:07:11.068446 peewee_migrate-1.7.7/pyproject.toml
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.7.7/PKG-INFO
```

### Comparing `peewee_migrate-1.7.6/README.rst` & `peewee_migrate-1.7.7/README.rst`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.6/peewee_migrate/auto.py` & `peewee_migrate-1.7.7/peewee_migrate/auto.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.6/peewee_migrate/cli.py` & `peewee_migrate-1.7.7/peewee_migrate/cli.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.6/peewee_migrate/migrator.py` & `peewee_migrate-1.7.7/peewee_migrate/migrator.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.6/peewee_migrate/router.py` & `peewee_migrate-1.7.7/peewee_migrate/router.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.6/peewee_migrate/template.py` & `peewee_migrate-1.7.7/peewee_migrate/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,14 @@
 from decimal import ROUND_HALF_EVEN
 
 try:
     import playhouse.postgres_ext as pw_pext
 except ImportError:
     pass
 
-SQL = pw.SQL
-
 
 def migrate(migrator: Migrator, database: pw.Database, *, fake=False):
     \"\"\"Write your migrations here.\"\"\"
     {migrate}
 
 
 def rollback(migrator: Migrator, database: pw.Database, *, fake=False):
```

### Comparing `peewee_migrate-1.7.6/pyproject.toml` & `peewee_migrate-1.7.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-migrate"
-version = "1.7.6"
+version = "1.7.7"
 homepage = "https://github.com/klen/peewee_migrate"
 repository = "https://github.com/klen/peewee_migrate"
 description = "Support for migrations in Peewee ORM"
 readme = "README.rst"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["peewee", "migrations", "orm"]
```

### Comparing `peewee_migrate-1.7.6/PKG-INFO` & `peewee_migrate-1.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-migrate
-Version: 1.7.6
+Version: 1.7.7
 Summary: Support for migrations in Peewee ORM
 Home-page: https://github.com/klen/peewee_migrate
 License: MIT
 Keywords: peewee,migrations,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

