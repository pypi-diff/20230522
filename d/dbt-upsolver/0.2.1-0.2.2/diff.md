# Comparing `tmp/dbt-upsolver-0.2.1.tar.gz` & `tmp/dbt-upsolver-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-upsolver-0.2.1.tar", last modified: Wed May 17 10:47:56 2023, max compression
+gzip compressed data, was "dbt-upsolver-0.2.2.tar", last modified: Mon May 22 18:07:53 2023, max compression
```

## Comparing `dbt-upsolver-0.2.1.tar` & `dbt-upsolver-0.2.2.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.315206 dbt-upsolver-0.2.1/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.315206 dbt-upsolver-0.2.1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.315206 dbt-upsolver-0.2.1/dbt/adapters/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/connection_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/copy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/materialized_view_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/table_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/transformation_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/adapters/upsolver/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.315206 dbt-upsolver-0.2.1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/dbt/include/upsolver/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/connection.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/materializedview.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/utils/ater_job.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/utils/create_table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/utils/render_options.sql
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/dbt/include/upsolver/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/dbt_upsolver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-17 10:47:56.000000 dbt-upsolver-0.2.1/dbt_upsolver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-17 10:47:56.000000 dbt-upsolver-0.2.1/dbt_upsolver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:47:56.000000 dbt-upsolver-0.2.1/dbt_upsolver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 10:47:56.000000 dbt-upsolver-0.2.1/dbt_upsolver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-17 10:47:56.000000 dbt-upsolver-0.2.1/dbt_upsolver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 10:47:56.000000 dbt-upsolver-0.2.1/dbt_upsolver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 10:47:56.319206 dbt-upsolver-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-17 10:47:47.000000 dbt-upsolver-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.687136 dbt-upsolver-0.2.2/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.687136 dbt-upsolver-0.2.2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.687136 dbt-upsolver-0.2.2/dbt/adapters/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.687136 dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/connection_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/copy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/target_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/transformation_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/adapters/upsolver/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.687136 dbt-upsolver-0.2.2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/dbt/include/upsolver/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/connection.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/incremental/create_copy_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/incremental/create_insert_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/materializedview.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/utils/ater_job.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/utils/create_table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/utils/render_options.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/dbt/include/upsolver/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/dbt_upsolver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10508 2023-05-22 18:07:53.000000 dbt-upsolver-0.2.2/dbt_upsolver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-22 18:07:53.000000 dbt-upsolver-0.2.2/dbt_upsolver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:07:53.000000 dbt-upsolver-0.2.2/dbt_upsolver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 18:07:53.000000 dbt-upsolver-0.2.2/dbt_upsolver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-22 18:07:53.000000 dbt-upsolver-0.2.2/dbt_upsolver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-22 18:07:53.000000 dbt-upsolver-0.2.2/dbt_upsolver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 18:07:53.691136 dbt-upsolver-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-22 18:07:39.000000 dbt-upsolver-0.2.2/setup.py
```

### Comparing `dbt-upsolver-0.2.1/LICENSE` & `dbt-upsolver-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.1/PKG-INFO` & `dbt-upsolver-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 0.2.1
+Version: 0.2.2
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dbt-upsolver-0.2.1/README.md` & `dbt-upsolver-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.1/dbt/adapters/upsolver/connections.py` & `dbt-upsolver-0.2.2/dbt/adapters/upsolver/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.1/dbt/adapters/upsolver/impl.py` & `dbt-upsolver-0.2.2/dbt/adapters/upsolver/impl.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 from dbt.events import AdapterLogger
 from dbt.adapters.upsolver.relation import UpsolverRelation
 from typing import List
 from dbt.adapters.base.meta import available
 from dbt.adapters.upsolver.options.copy_options import Copy_options
 from dbt.adapters.upsolver.options.connection_options import Connection_options
 from dbt.adapters.upsolver.options.transformation_options import Transformation_options
-from dbt.adapters.upsolver.options.table_options import Table_options
-from dbt.adapters.upsolver.options.materialized_view_options import Materialized_view_options
+from dbt.adapters.upsolver.options.target_options import Target_options
 import agate
 import datetime
 import re
 import dbt
 
 logger = AdapterLogger("Upsolver")
 LIST_RELATION_MACRO_NAME = "list_relation_without_caching"
@@ -46,15 +45,15 @@
     @available
     def get_connection_from_sql(self, sql):
         try:
             connection_identifier = re.search('"(.*)"', sql).group().split('.')[2] \
                                       .translate(str.maketrans({'\"':'', '\'':''}))
             return connection_identifier
         except Exception:
-            raise dbt.exceptions.ParsingError(f"Error while parsing connection name from sql:\n{sql}")
+            raise dbt.exceptions.ParsingError(f"Error while parsing connection name from sql: {sql}")
 
     @available
     def get_columns_names_with_types(self, list_dict):
         res = []
         for col in list_dict:
             if col.get('type'):
                 res.append(f"{col['field']} {col['type']}")
@@ -69,49 +68,90 @@
 
     @available
     def separate_options(self, config_options, source):
         job_options = self.enrich_options(config_options, source, 'job_options')
         source_options = self.enrich_options(config_options, source, 'source_options')
         return job_options, source_options
 
+    def render_option_from_dict(self, option_value):
+        res = []
+        try:
+            for key, value in option_value.items():
+                item = [f'{key}=']
+                if isinstance(value, list):
+                    item.append('(')
+                    item.append(' ,'.join(value))
+                    item.append(')')
+                else:
+                    item.append(value)
+                res.append(''.join(item))
+            return f"({' ,'.join(res)})"
+        except Exception:
+            raise dbt.exceptions.ParsingError(f"Error while parsing value: {value}")
+
+    def render_option_from_list(self, option_value):
+        try:
+            if not isinstance(option_value, str):
+                return tuple(i for i in option_value)
+            else:
+                return f"('{option_value}')"
+        except Exception:
+            raise dbt.exceptions.ParsingError(f"Error while parsing value: {value}")
+
     @available
     def enrich_options(self, config_options, source, options_type):
         options = self.get_options(source, options_type)
         enriched_options = {}
         for option, value in config_options.items():
             find_value = options.get(option.lower(), None)
             if find_value:
                 if options[option.lower()]['type'] == 'list':
-                    if not isinstance(value, str):
-                        value = tuple(i for i in value)
-                    else:
-                        value = f"('{value}')"
+                    value = self.render_option_from_list(value)
+                elif options[option.lower()]['type'] == 'dict':
+                    value = self.render_option_from_dict(value)
                 enriched_options[option] = find_value
                 enriched_options[option]['value'] = value
             else:
                 logger.warning(f"Options not found: {option}")
         return enriched_options
 
     @available
     def filter_options(self, options, parametr):
         editable = {key:val for key, val in options.items() if val[parametr] == True}
         return editable
 
-    def get_options(self, source, options_type):
-        if options_type == 'connection_options':
-            options = Connection_options[source.lower()]
-        elif options_type == 'transformation_options':
-            options = Transformation_options[source.lower()]
-        elif options_type == 'table_options':
-            options = Table_options
-        elif options_type == 'materialized_view_options':
-            options = Materialized_view_options
+    @available
+    def get(self, config, key, default=None):
+        config = {k.lower(): v for k, v in config.items()}
+        value = config.get(key, default)
+        return value
+
+    @available
+    def require(self, config, key):
+        config = {k.lower(): v for k, v in config.items()}
+        value = config.get(key, None)
+        if value:
+            return value
         else:
-            options = Copy_options[source.lower()][options_type]
-        return options
+            raise dbt.exceptions.ParsingError(f"Required option is missing: {key}")
+
+
+    def get_options(self, source, options_type):
+        try:
+            if options_type == 'connection_options':
+                options = Connection_options[source.lower()]
+            elif options_type == 'transformation_options':
+                options = Transformation_options[source.lower()]
+            elif options_type == 'target_options':
+                options = Target_options[source.lower()]
+            else:
+                options = Copy_options[source.lower()][options_type]
+            return options
+        except Exception:
+            raise dbt.exceptions.ParsingError(f"Undefined option value: {source}")
 
     def list_relations_without_caching(
         self,
         schema_relation: UpsolverRelation,
         ) -> List[UpsolverRelation]:
         materializations = ["table", "job", "connection", "view"]
         results = agate.Table([],[])
```

### Comparing `dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/connection_options.py` & `dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/connection_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/copy_options.py` & `dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/copy_options.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.1/dbt/adapters/upsolver/options/transformation_options.py` & `dbt-upsolver-0.2.2/dbt/adapters/upsolver/options/transformation_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,53 +9,54 @@
         "run_parallelism": {"type": "integer", "editable": True, "optional": True},
         "file_type": {"type": "value", "editable": False, "optional": False},
         "compression": {"type": "value", "editable": False, "optional": True},
         "date_pattern": {"type": "text", "editable": False, "optional": True},
         "output_offset": {"type": "integer", "editable": False, "optional": True},
         "location": {"type": "text", "editable": False, "optional": True}
   },
-  'elasticsearch': {
+  "elasticsearch": {
         "run_interval": {"type": "ineger", "editable": False, "optional": True},
         "start_from": {"type": "value", "editable": False, "optional": True},
         "end_at": {"type": "value", "editable": True, "optional": True},
         "compute_cluster": {"type": "identifier", "editable": True, "optional": True},
         "allow_cartesian_products": {"type": "boolean", "editable": False, "optional": True},
         "aggregation_parallelism": {"type": "integer", "editable": True, "optional": True},
         "run_parallelism": {"type": "integer", "editable": True, "optional": True},
         "bulk_max_size_bytes": {"type": "integer", "editable": True, "optional": True},
         "index_partition_size": {"type": "value", "editable": True, "optional": True},
         "comment": {"type": "text", "editable": True, "optional": True}
   },
-  'snowflake': {
+  "snowflake": {
+        "add_missing_columns": {"type": "boolean", "editable": False, "optional": True},
         "run_interval": {"type": "ineger", "editable": False, "optional": True},
         "start_from": {"type": "value", "editable": False, "optional": True},
         "end_at": {"type": "value", "editable": True, "optional": True},
         "compute_cluster": {"type": "identifier", "editable": True, "optional": True},
         "allow_cartesian_products": {"type": "boolean", "editable": False, "optional": True},
         "aggregation_parallelism": {"type": "integer", "editable": True, "optional": True},
         "run_parallelism": {"type": "integer", "editable": True, "optional": True},
         "comment": {"type": "text", "editable": True, "optional": True}
   },
-    'upsolver_data_lake': {
+    "datalake": {
         "add_missing_columns": {"type": "boolean", "editable": False, "optional": True},
         "run_interval": {"type": "ineger", "editable": False, "optional": True},
         "start_from": {"type": "value", "editable": False, "optional": True},
         "end_at": {"type": "value", "editable": True, "optional": True},
         "compute_cluster": {"type": "identifier", "editable": True, "optional": True},
         "allow_cartesian_products": {"type": "boolean", "editable": False, "optional": True},
         "aggregation_parallelism": {"type": "integer", "editable": True, "optional": True},
         "run_parallelism": {"type": "integer", "editable": True, "optional": True},
         "comment": {"type": "text", "editable": True, "optional": True}
     },
-    'redshift': {
+    "redshift": {
         "run_interval": {"type": "ineger", "editable": False, "optional": True},
         "start_from": {"type": "value", "editable": False, "optional": True},
         "end_at": {"type": "value", "editable": True, "optional": True},
         "compute_cluster": {"type": "identifier", "editable": True, "optional": True},
         "allow_cartesian_products": {"type": "boolean", "editable": False, "optional": True},
         "aggregation_parallelism": {"type": "integer", "editable": True, "optional": True},
         "run_parallelism": {"type": "integer", "editable": True, "optional": True},
-        "skip_faild_files": {"type": "boolean", "editable": False, "optional": True},
+        "skip_failed_files": {"type": "boolean", "editable": False, "optional": True},
         "fail_on_write_error": {"type": "boolean", "editable": False, "optional": True},
         "comment": {"type": "text", "editable": True, "optional": True}
     }
 }
```

### Comparing `dbt-upsolver-0.2.1/dbt/adapters/upsolver/relation.py` & `dbt-upsolver-0.2.2/dbt/adapters/upsolver/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.1/dbt/include/upsolver/macros/adapters.sql` & `dbt-upsolver-0.2.2/dbt/include/upsolver/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/connection.sql` & `dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/connection.sql`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% materialization connection, adapter='upsolver' %}
   {%- set identifier = model['alias'] -%}
-
-  {% set connection_type = config.require('connection_type') %}
-  {% set connection_options = config.require('connection_options') %}
+  {%- set model_config = model['config'] -%}
+  {% set connection_type = adapter.require(model_config, 'connection_type') %}
+  {% set connection_options = adapter.require(model_config, 'connection_options') %}
   {% set enriched_options = adapter.enrich_options(connection_options, connection_type, 'connection_options') %}
   {% set enriched_editable_options = adapter.filter_options(enriched_options, 'editable') %}
 
 
   {%- set old_relation = adapter.get_relation(identifier=identifier,
                                               schema=schema,
                                               database=database) -%}
```

### Comparing `dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql` & `dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/incremental/create_merge_job.sql`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,22 @@
-{% macro get_create_merge_job_sql(job_identifier, table, sync, options, primary_key, delete_condition) -%}
+{% macro get_create_merge_job_sql(job_identifier, into_relation, sync, options, primary_key, delete_condition, target_type) -%}
 
-  {% set enriched_options = adapter.enrich_options(options, 'upsolver_data_lake', 'transformation_options') %}
+  {% set enriched_options = adapter.enrich_options(options, target_type, 'transformation_options') %}
+
+  {%- if target_type == 'datalake' -%}
+    {% set target_type = '' %}
+  {%- endif -%}
 
   CREATE
   {% if sync %}
     SYNC
   {% endif %}
   JOB {{ job_identifier }}
     {{ render_options(enriched_options, 'create') }}
-  AS MERGE INTO {{ table }} AS target
+  AS MERGE INTO {{ target_type }} {{ into_relation }} AS target
   USING (
   {{ sql }}
   )
   {% if primary_key %}
     source ON (
       {% for item in primary_key %}
         target.{{ item['field'] }} = source.{{ item['field'] }}
```

### Comparing `dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/materializedview.sql` & `dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/materializedview.sql`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 {% materialization materializedview, adapter='upsolver' %}
   {%- set identifier = model['alias'] -%}
-  {% set sync = config.get('sync', False) %}
-  {% set options = config.get('options', {}) %}
-  {% set enriched_options = adapter.enrich_options(options, None, 'materialized_view_options') %}
+  {%- set model_config = model['config'] -%}
+  {% set sync = adapter.get(model_config, 'sync', False) %}
+  {% set options = adapter.get(model_config, 'options', {}) %}
+  {% set enriched_options = adapter.enrich_options(options, materialized_view, 'target_options') %}
   {% set enriched_editable_options = adapter.filter_options(enriched_options, 'editable') %}
 
   {%- set old_relation = adapter.get_relation(identifier=identifier,
                                               schema=schema,
                                               database=database) -%}
   {%- set target_relation = api.Relation.create(identifier=identifier,
                                                 schema=schema,
```

### Comparing `dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/utils/ater_job.sql` & `dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/utils/ater_job.sql`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% macro get_alter_job_sql(job_identifier, options, incremental_strategy, source) -%}
 
   {% if incremental_strategy %}
-    {% set enriched_options = adapter.enrich_options(options, 'upsolver_data_lake', 'transformation_options') %}
+    {% set enriched_options = adapter.enrich_options(options, 'datalake', 'transformation_options') %}
   {% else  %}
     {% set enriched_options, _ = adapter.separate_options(options, source) %}
   {% endif %}
   {% set enriched_editable_options = adapter.filter_options(enriched_options, 'editable') %}
 
   ALTER JOB {{job_identifier}}
     {{ render_options(enriched_editable_options, 'alter') }}
```

### Comparing `dbt-upsolver-0.2.1/dbt/include/upsolver/macros/materializations/utils/create_table.sql` & `dbt-upsolver-0.2.2/dbt/include/upsolver/macros/materializations/utils/create_table.sql`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 {%- set old_relation = adapter.get_relation(identifier=target_relation.identifier,
                                             schema=target_relation.schema,
                                             database=target_relation.database) -%}
 
   {%- set columns_with_types = adapter.get_columns_names_with_types(partition_by + primary_key) -%}
   {%- set columns_partitioned_by  = adapter.get_columns_names(partition_by) -%}
   {%- set columns_primary_key  = adapter.get_columns_names(primary_key) -%}
-  {% set enriched_options = adapter.enrich_options(options, None, 'table_options') %}
+  {% set enriched_options = adapter.enrich_options(options, 'datalake', 'target_options') %}
   {% set enriched_editable_options = adapter.filter_options(enriched_options, 'editable') %}
 
   {% if old_relation %}
     ALTER TABLE {{target_relation}}
       {{ render_options(enriched_editable_options, 'alter') }}
   {% else %}
     CREATE TABLE {{ target_relation }}
```

### Comparing `dbt-upsolver-0.2.1/dbt_upsolver.egg-info/PKG-INFO` & `dbt-upsolver-0.2.2/dbt_upsolver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-upsolver
-Version: 0.2.1
+Version: 0.2.2
 Summary: The Upsolver adapter plugin for dbt
 Home-page: https://github.com/tanyshak/dbt-upsolver
 Author: Upsolver Team
 Author-email: info@upsolver.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dbt-upsolver-0.2.1/dbt_upsolver.egg-info/SOURCES.txt` & `dbt-upsolver-0.2.2/dbt_upsolver.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 dbt/adapters/upsolver/__init__.py
 dbt/adapters/upsolver/__version__.py
 dbt/adapters/upsolver/connections.py
 dbt/adapters/upsolver/impl.py
 dbt/adapters/upsolver/relation.py
 dbt/adapters/upsolver/options/connection_options.py
 dbt/adapters/upsolver/options/copy_options.py
-dbt/adapters/upsolver/options/materialized_view_options.py
-dbt/adapters/upsolver/options/table_options.py
+dbt/adapters/upsolver/options/target_options.py
 dbt/adapters/upsolver/options/transformation_options.py
 dbt/include/upsolver/__init__.py
 dbt/include/upsolver/dbt_project.yml
 dbt/include/upsolver/profile_template.yml
 dbt/include/upsolver/macros/adapters.sql
 dbt/include/upsolver/macros/catalog.sql
 dbt/include/upsolver/macros/materializations/connection.sql
```

### Comparing `dbt-upsolver-0.2.1/setup.py` & `dbt-upsolver-0.2.2/setup.py`

 * *Files identical despite different names*

