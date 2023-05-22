# Comparing `tmp/nexus-utilities-0.4.1.tar.gz` & `tmp/nexus-utilities-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexus-utilities-0.4.1.tar", last modified: Thu May 18 17:23:41 2023, max compression
+gzip compressed data, was "nexus-utilities-0.5.0.tar", last modified: Mon May 22 14:43:42 2023, max compression
```

## Comparing `nexus-utilities-0.4.1.tar` & `nexus-utilities-0.5.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:41.006468 nexus-utilities-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-18 17:23:41.006468 nexus-utilities-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:41.002468 nexus-utilities-0.4.1/nexus_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-18 17:23:40.000000 nexus-utilities-0.4.1/nexus_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-18 17:23:40.000000 nexus-utilities-0.4.1/nexus_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:23:40.000000 nexus-utilities-0.4.1/nexus_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-18 17:23:40.000000 nexus-utilities-0.4.1/nexus_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-18 17:23:40.000000 nexus-utilities-0.4.1/nexus_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:23:41.006468 nexus-utilities-0.4.1/nexus_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/database_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/datetime_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/flatfile_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/package_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/password_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/nexus_utils/string_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 17:23:41.006468 nexus-utilities-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-18 17:23:30.000000 nexus-utilities-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:43:42.113603 nexus-utilities-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-22 14:43:42.113603 nexus-utilities-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13576 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:43:42.113603 nexus-utilities-0.5.0/nexus_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-22 14:43:41.000000 nexus-utilities-0.5.0/nexus_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-22 14:43:42.000000 nexus-utilities-0.5.0/nexus_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 14:43:41.000000 nexus-utilities-0.5.0/nexus_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 14:43:41.000000 nexus-utilities-0.5.0/nexus_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 14:43:41.000000 nexus-utilities-0.5.0/nexus_utilities.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 14:43:42.113603 nexus-utilities-0.5.0/nexus_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11114 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/database_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/datetime_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/flatfile_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/package_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/password_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/nexus_utils/string_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 14:43:42.113603 nexus-utilities-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-22 14:43:31.000000 nexus-utilities-0.5.0/setup.py
```

### Comparing `nexus-utilities-0.4.1/LICENSE.txt` & `nexus-utilities-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.4.1/PKG-INFO` & `nexus-utilities-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.4.1
+Version: 0.5.0
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.4.1/README.md` & `nexus-utilities-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.4.1/nexus_utilities.egg-info/PKG-INFO` & `nexus-utilities-0.5.0/nexus_utilities.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexus-utilities
-Version: 0.4.1
+Version: 0.5.0
 Summary: Common python utilities
 Home-page: https://github.com/james-larsen/nexus-utilities
 Author: James Larsen
 Author-email: james.larsen42@gmail.com
 License: UNKNOWN
 Description: This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.
 Platform: UNKNOWN
```

### Comparing `nexus-utilities-0.4.1/nexus_utils/config_utils.py` & `nexus-utilities-0.5.0/nexus_utils/config_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.4.1/nexus_utils/database_utils.py` & `nexus-utilities-0.5.0/nexus_utils/database_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,16 +64,19 @@
 
     sql_statement = re.sub('^\n', '', sql_statement, flags = re.DOTALL)
     sql_statement = re.sub('\n$', '', sql_statement, flags = re.DOTALL)
     #print(sql_statement)
 
     sql_statements = sql_statement.split(';')
 
+    sql_statements = [statement.strip() for statement in sql_statements]
+
     # Remove blank statements
-    sql_statements.remove("")
+    if "" in sql_statements:
+        sql_statements.remove("")
     #print(len(sql_statements))
 
     # Add ';' to the end of each statement
     sql_statements_output = []
     for statement in sql_statements:
         statement_output = re.sub('^\n', '', statement)
         statement_output = re.sub('\n^', '', statement_output)
```

### Comparing `nexus-utilities-0.4.1/nexus_utils/datetime_utils.py` & `nexus-utilities-0.5.0/nexus_utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.4.1/nexus_utils/package_utils.py` & `nexus-utilities-0.5.0/nexus_utils/package_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.4.1/nexus_utils/password_utils.py` & `nexus-utilities-0.5.0/nexus_utils/password_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.4.1/nexus_utils/string_utils.py` & `nexus-utilities-0.5.0/nexus_utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `nexus-utilities-0.4.1/setup.py` & `nexus-utilities-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='nexus-utilities',
-    version='0.4.1',
+    version='0.5.0',
     author='James Larsen',
     author_email='james.larsen42@gmail.com',
     description='Common python utilities',
     long_description='This package is meant to hold various useful utilities for functionality I find myself using across multiple projects.  I will try to keep this documentation updated as I expand the toolkit.',
     long_description_content_type='text/markdown',
     url='https://github.com/james-larsen/nexus-utilities',
     packages=['nexus_utils'],
```

