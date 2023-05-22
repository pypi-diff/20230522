# Comparing `tmp/fluctuate-1.0.0.tar.gz` & `tmp/fluctuate-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluctuate-1.0.0.tar", max compression
+gzip compressed data, was "fluctuate-1.0.1.tar", max compression
```

## Comparing `fluctuate-1.0.0.tar` & `fluctuate-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-05-06 03:47:33.026132 fluctuate-1.0.0/LICENSE
--rw-r--r--   0        0        0     9605 2023-05-06 03:47:33.026132 fluctuate-1.0.0/README.md
--rw-r--r--   0        0        0        0 2023-05-06 03:47:33.026132 fluctuate-1.0.0/fluctuate/__init__.py
--rw-r--r--   0        0        0     4404 2023-05-06 03:47:33.026132 fluctuate-1.0.0/fluctuate/cli.py
--rw-r--r--   0        0        0    25221 2023-05-06 03:47:33.026132 fluctuate-1.0.0/fluctuate/migrations.py
--rw-r--r--   0        0        0     1136 2023-05-06 03:47:33.027132 fluctuate-1.0.0/fluctuate/secrets_manager.py
--rw-r--r--   0        0        0     1385 2023-05-06 03:48:33.024466 fluctuate-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    10540 1970-01-01 00:00:00.000000 fluctuate-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-22 20:29:57.910984 fluctuate-1.0.1/LICENSE
+-rw-r--r--   0        0        0     9458 2023-05-22 20:29:57.911985 fluctuate-1.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-22 20:29:57.911985 fluctuate-1.0.1/fluctuate/__init__.py
+-rw-r--r--   0        0        0     4404 2023-05-22 20:29:57.911985 fluctuate-1.0.1/fluctuate/cli.py
+-rw-r--r--   0        0        0    25195 2023-05-22 20:29:57.911985 fluctuate-1.0.1/fluctuate/migrations.py
+-rw-r--r--   0        0        0     1136 2023-05-22 20:29:57.911985 fluctuate-1.0.1/fluctuate/secrets_manager.py
+-rw-r--r--   0        0        0     1385 2023-05-22 20:30:37.007923 fluctuate-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10393 1970-01-01 00:00:00.000000 fluctuate-1.0.1/PKG-INFO
```

### Comparing `fluctuate-1.0.0/LICENSE` & `fluctuate-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fluctuate-1.0.0/README.md` & `fluctuate-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Fluctuate
 
-[![pipeline status](https://gitlab.com/munipal-oss/fluctuate/badges/master/pipeline.svg)](https://gitlab.com/munipal-oss/fluctuate/-/commits/master)
 [![coverage report](https://gitlab.com/munipal-oss/fluctuate/badges/master/coverage.svg)](https://gitlab.com/munipal-oss/fluctuate/-/commits/master)
 [![Latest Release](https://gitlab.com/munipal-oss/fluctuate/-/badges/release.svg)](https://gitlab.com/munipal-oss/fluctuate/-/releases)
 
 Fluctuate is a simple migration utility for [Fauna DB] written in [Python]. It doesn't
 aim to be as full featured as something like [fauna-schema-migrate], but aims to provide
 a foundation to set up your Fauna dabatases as code.
 
@@ -42,15 +41,15 @@
 
 To define your projects migrations, create a file named `fluctuate_migrations.py` in a
 subfolder of your project along with an `__init__.py` within that subfolder. Within
 `fluctuate_migrations.py` you need to create a tuple or list of `Migration`s named
 "migrations" that defines your migrations. An example from our test suite is below:
 
 ```python
-# faunadb_migrations.py
+# fluctuate_migrations.py
 from faunadb import query
 
 from fluctuate.migrations import Migration
 
 migrations = (
     Migration(
         name="test_migration_1",
```

### Comparing `fluctuate-1.0.0/fluctuate/cli.py` & `fluctuate-1.0.1/fluctuate/cli.py`

 * *Files identical despite different names*

### Comparing `fluctuate-1.0.0/fluctuate/migrations.py` & `fluctuate-1.0.1/fluctuate/migrations.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
     # the child DB.
     if child_db is not None:
         key = _build_scoped_key(key=key, child_db=child_db)
         logger.debug("Creating FaunaDB client for child database %s.", child_db)
     else:
         logger.debug("Creating FaunaDB client for top level database.")
 
-    fauna_client = FaunaClient(secret=key, domain="db.us.fauna.com")
+    fauna_client = FaunaClient(secret=key)
     logger.debug("FaunaDB client initialized.")
 
     return fauna_client
 
 
 # This FQL fragment matches the fluctuate_migrations_unique_name_and_namespace using the variables
 # "migration_name" and "migration_namespace" to retrieve the migration's name and
```

### Comparing `fluctuate-1.0.0/fluctuate/secrets_manager.py` & `fluctuate-1.0.1/fluctuate/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `fluctuate-1.0.0/pyproject.toml` & `fluctuate-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fluctuate"
-version = "1.0.0"
+version = "1.0.1"
 description = "A simple migration utility for Fauna DB."
 authors = ["Ryan Causey <ryan.causey@munipal.io>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://gitlab.com/munipal-oss/fluctuate"
 homepage = "https://gitlab.com/munipal-oss/fluctuate"
```

### Comparing `fluctuate-1.0.0/PKG-INFO` & `fluctuate-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluctuate
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple migration utility for Fauna DB.
 Home-page: https://gitlab.com/munipal-oss/fluctuate
 License: MIT
 Author: Ryan Causey
 Author-email: ryan.causey@munipal.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,14 @@
 Requires-Dist: cloup (>=2.0.0,<3.0.0)
 Requires-Dist: faunadb (>=4.3.1,<5.0.0)
 Project-URL: Repository, https://gitlab.com/munipal-oss/fluctuate
 Description-Content-Type: text/markdown
 
 # Fluctuate
 
-[![pipeline status](https://gitlab.com/munipal-oss/fluctuate/badges/master/pipeline.svg)](https://gitlab.com/munipal-oss/fluctuate/-/commits/master)
 [![coverage report](https://gitlab.com/munipal-oss/fluctuate/badges/master/coverage.svg)](https://gitlab.com/munipal-oss/fluctuate/-/commits/master)
 [![Latest Release](https://gitlab.com/munipal-oss/fluctuate/-/badges/release.svg)](https://gitlab.com/munipal-oss/fluctuate/-/releases)
 
 Fluctuate is a simple migration utility for [Fauna DB] written in [Python]. It doesn't
 aim to be as full featured as something like [fauna-schema-migrate], but aims to provide
 a foundation to set up your Fauna dabatases as code.
 
@@ -66,15 +65,15 @@
 
 To define your projects migrations, create a file named `fluctuate_migrations.py` in a
 subfolder of your project along with an `__init__.py` within that subfolder. Within
 `fluctuate_migrations.py` you need to create a tuple or list of `Migration`s named
 "migrations" that defines your migrations. An example from our test suite is below:
 
 ```python
-# faunadb_migrations.py
+# fluctuate_migrations.py
 from faunadb import query
 
 from fluctuate.migrations import Migration
 
 migrations = (
     Migration(
         name="test_migration_1",
```

