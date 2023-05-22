# Comparing `tmp/ibis_singlestoredb-0.2.0.tar.gz` & `tmp/ibis_singlestoredb-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibis_singlestoredb-0.2.0.tar", last modified: Fri Dec  9 21:27:12 2022, max compression
+gzip compressed data, was "ibis_singlestoredb-0.3.0.tar", last modified: Mon May 22 16:07:24 2023, max compression
```

## Comparing `ibis_singlestoredb-0.2.0.tar` & `ibis_singlestoredb-0.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:27:12.183771 ibis_singlestoredb-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2022-12-09 21:27:12.183771 ibis_singlestoredb-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:27:12.179771 ibis_singlestoredb-0.2.0/ibis_singlestoredb/
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    12003 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23670 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:27:12.183771 ibis_singlestoredb-0.2.0/ibis_singlestoredb/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9538 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb/tests/datatypes.csv
--rw-r--r--   0 runner    (1001) docker     (123)      971 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb/tests/test_op_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    18868 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb/tests/test_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-09 21:27:12.183771 ibis_singlestoredb-0.2.0/ibis_singlestoredb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2022-12-09 21:27:12.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      772 2022-12-09 21:27:12.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-09 21:27:12.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2022-12-09 21:27:12.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-09 21:27:12.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-09 21:27:12.000000 ibis_singlestoredb-0.2.0/ibis_singlestoredb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2022-12-09 21:27:12.183771 ibis_singlestoredb-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      136 2022-12-09 21:26:35.000000 ibis_singlestoredb-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:07:24.901703 ibis_singlestoredb-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-22 16:07:24.901703 ibis_singlestoredb-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:07:24.897704 ibis_singlestoredb-0.3.0/ibis_singlestoredb/
+-rw-r--r--   0 runner    (1001) docker     (123)    14372 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8349 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24436 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:07:24.901703 ibis_singlestoredb-0.3.0/ibis_singlestoredb/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9538 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb/tests/datatypes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb/tests/test_op_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19181 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb/tests/test_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:07:24.897704 ibis_singlestoredb-0.3.0/ibis_singlestoredb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-22 16:07:24.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-22 16:07:24.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:07:24.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-22 16:07:24.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-22 16:07:24.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-22 16:07:24.000000 ibis_singlestoredb-0.3.0/ibis_singlestoredb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-22 16:07:24.901703 ibis_singlestoredb-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-22 16:06:49.000000 ibis_singlestoredb-0.3.0/setup.py
```

### Comparing `ibis_singlestoredb-0.2.0/LICENSE` & `ibis_singlestoredb-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibis_singlestoredb-0.2.0/PKG-INFO` & `ibis_singlestoredb-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibis_singlestoredb
-Version: 0.2.0
+Version: 0.3.0
 Summary: Ibis backend for the SingleStore database
 Home-page: https://github.com/singlestore-labs/ibis-singlestoredb
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ibis_singlestoredb-0.2.0/README.md` & `ibis_singlestoredb-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ibis_singlestoredb-0.2.0/ibis_singlestoredb/__init__.py` & `ibis_singlestoredb-0.3.0/ibis_singlestoredb/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,49 @@
 """The SingleStoreDB backend."""
 from __future__ import annotations
 
-import atexit
-import contextlib
+import re
 import warnings
 from typing import Any
 from typing import Dict
-from typing import Generator
+from typing import Iterable
 from typing import Optional
+from typing import Union
 
-import ibis.common.exceptions as com
 import ibis.expr.datatypes as dt
 import ibis.expr.schema as sch
 import ibis.expr.types as ir
 import ibis.util
 import pandas as pd
 import sqlalchemy as sa
-import sqlalchemy.dialects.mysql as singlestoredb
+import sqlalchemy_singlestoredb as singlestoredb
 from ibis.backends.base.sql.alchemy import BaseAlchemyBackend
-from ibis.backends.base.sql.registry.helpers import quote_identifier
-from ibis.expr.types import AnyColumn
-from pandas.io.json import build_table_schema
 from singlestoredb.connection import build_params
-from sqlalchemy_singlestoredb.base import SingleStoreDBDialect
 
 from . import functions as fn
 from .compiler import SingleStoreDBCompiler
 from .database import SingleStoreDBDatabase
 from .database import SingleStoreDBDatabaseTable
 from .datatypes import _type_from_cursor_info
+from .datatypes import SingleStoreDBDateTime
 from .expr import SingleStoreDBTable
+# from . import functions as fn
 
 
-__version__ = '0.2.0'
+__version__ = '0.3.0'
 
 
 class Backend(BaseAlchemyBackend):
     name = 'singlestoredb'
-    compiler = SingleStoreDBCompiler
 
+    compiler = SingleStoreDBCompiler
     database_class = SingleStoreDBDatabase
     table_class = SingleStoreDBDatabaseTable
     table_expr_class = SingleStoreDBTable
+    supports_create_or_replace = False
 
     _database_name: Optional[str] = None
 
     @property
     def database_name(self) -> Optional[str]:
         """Get the currently selected database."""
         return self._database_name
@@ -140,57 +138,59 @@
             driver=driver,
         )
 
         alchemy_url.set(query={k: str(v) for k, v in params.items()})
 
         self.database_name = alchemy_url.database
 
-        super().do_connect(
-            sa.create_engine(
-                alchemy_url,
-                echo=kwargs.get('echo', False), future=kwargs.get('future', False),
-            ),
-        )
+        engine = sa.create_engine(alchemy_url, poolclass=sa.pool.StaticPool)
 
-        self.sync_functions()
+        @sa.event.listens_for(engine, 'connect')
+        def connect(
+            dbapi_connection: singlestoredb.Connection,
+            connection_record: Any,
+        ) -> None:
+            with dbapi_connection.cursor() as cur:
+                try:
+                    cur.execute("SET @@session.time_zone = 'UTC'")
+                except sa.exc.OperationalError:
+                    warnings.warn('Unable to set session timezone to UTC.')
 
-#   @contextlib.contextmanager
-#   def begin(self) -> Generator[Any, Any, Any]:
-#       with super().begin() as bind:
-#           previous_timezone = bind.execute(
-#               'SELECT @@session.time_zone',
-#           ).scalar()
-#           unset_timezone = False
-#           try:
-#               bind.execute("SET @@session.time_zone = 'UTC'")
-#               unset_timezone = True
-#           except Exception as e:
-#               warnings.warn(f"Couldn't set singlestore timezone: {str(e)}")
-
-#           try:
-#               yield bind
-#           finally:
-#               if unset_timezone:
-#                   query = "SET @@session.time_zone = '{}'"
-#                   bind.execute(query.format(previous_timezone))
+        super().do_connect(engine)
+
+        self.sync_functions()
 
     def _table_from_schema(
-        self, name: str, schema: sch.Schema, database: str | None = None,
-        storage_type: Optional[str] = None,
+        self,
+        name: str,
+        schema: sch.Schema,
+        temp: bool = False,
+        database: Optional[str] = None,
+        **kwargs: Any,
     ) -> sa.Table:
         columns = self._columns_from_schema(name, schema)
-        kw = {}
+        prefixes = []
+        if temp:
+            prefixes.append(self._temporary_prefix)
+        storage_type = kwargs.pop('storage_type', None)
         if storage_type:
-            kw['prefixes'] = [storage_type.upper()]
-        return sa.Table(name, self.meta, *columns, **kw)
+            prefixes.append(storage_type.upper())
+        return sa.Table(
+            name,
+            sa.MetaData(),
+            *columns,
+            prefixes=prefixes,
+            quote=self.compiler.translator_class._quote_table_names,
+            **kwargs,
+        )
 
     def _merge_schema_overrides(
         self,
         schema: sch.Schema,
-        overrides: Dict[str, str] | sch.Schema,
+        overrides: Union[Dict[str, str], sch.Schema],
     ) -> sch.Schema:
         """
         Merge type overrides into a schema.
 
         Parameters
         ----------
         schema : Schema
@@ -200,32 +200,32 @@
 
         Returns
         -------
         Schema
 
         """
         if not isinstance(overrides, sch.Schema):
-            overrides = sch.Schema.from_dict(overrides)
+            overrides = sch.Schema.from_tuples(list(overrides.items()))
 
         items = list(schema.items())
         for i, item in enumerate(items):
             if item[0] in overrides:
                 items[i] = (item[0], overrides[item[0]])
 
         return ibis.Schema.from_tuples(items)
 
     def create_table(
         self,
         name: str,
-        expr: Optional[pd.DataFrame | ir.TableExpr] = None,
+        expr: Optional[Union[pd.DataFrame, ir.TableExpr]] = None,
         schema: Optional[sch.Schema] = None,
         database: Optional[str] = None,
         force: bool = False,
         storage_type: Optional[str] = None,
-        schema_overrides: Optional[Dict[str, str] | sch.Schema] = None,
+        schema_overrides: Optional[Union[Dict[str, str], sch.Schema]] = None,
     ) -> ir.Table:
         """
         Create a new table.
 
         Parameters
         ----------
         name : str
@@ -372,103 +372,54 @@
                 '`expr` and/or `schema` are not an expected type: {} / {}'.format(
                     type(expr).__name__, type(schema).__name__,
                 ),
             )
 
         return self.table(name)
 
+    @staticmethod
+    def _new_sa_metadata() -> sa.MetaData:
+        meta = sa.MetaData()
+
+        @sa.event.listens_for(meta, 'column_reflect')
+        def column_reflect(
+            inspector: Any,
+            table: Any,
+            column_info: Dict[str, Any],
+        ) -> None:
+            if isinstance(column_info['type'], singlestoredb.DATETIME):
+                column_info['type'] = SingleStoreDBDateTime()
+
+        return meta
+
+    def _metadata(self, query: str) -> Iterable[tuple[str, dt.DataType]]:
+        if (
+            re.search(r'^\s*SELECT\s', query, flags=re.MULTILINE | re.IGNORECASE)
+            is not None
+        ):
+            query = f'({query})'
+
+        with self.begin() as con:
+            result = con.exec_driver_sql(f'SELECT * FROM {query} _ LIMIT 0')
+            cursor = result.cursor
+            yield from (
+                (field.name, _type_from_cursor_info(descr, field))
+                for descr, field in zip(cursor.description, cursor._result.fields)
+            )
+
     def _get_schema_using_query(self, query: str) -> sch.Schema:
         """Infer the schema of `query`."""
-        result = self.con.execute(f'SELECT * FROM ({query}) _ LIMIT 0')
-        cursor = result.cursor
-        fields = [
-            (field.name, _type_from_cursor_info(descr, field))
-            for descr, field in zip(cursor.description, cursor._result.fields)
-        ]
-        return sch.Schema.from_tuples(fields)
+        with self.begin() as con:
+            result = con.exec_driver_sql(f'SELECT * FROM ({query}) _ LIMIT 0')
+            cursor = result.cursor
+            fields = [
+                (field.name, _type_from_cursor_info(descr, field))
+                for descr, field in zip(cursor.description, cursor._result.fields)
+            ]
+            return sch.Schema.from_tuples(fields)
 
     def _get_temp_view_definition(
         self,
         name: str,
         definition: sa.sql.compiler.Compiled,
     ) -> str:
         return f'CREATE VIEW {name} AS {definition}'
-
-    def _register_temp_view_cleanup(self, name: str, raw_name: str) -> None:
-        query = f'DROP VIEW IF EXISTS {name}'
-
-        def drop(self: Backend, raw_name: str, query: str) -> None:
-            self.con.execute(query)
-            self._temp_views.discard(raw_name)
-
-        atexit.register(drop, self, raw_name, query)
-
-
-# TODO(kszucs): unsigned integers
-
-
-@dt.dtype.register((singlestoredb.DOUBLE, singlestoredb.REAL))
-def singlestoredb_double(satype: Any, nullable: bool = True) -> dt.Float64:
-    return dt.Float64(nullable=nullable)
-
-
-@dt.dtype.register(singlestoredb.FLOAT)
-def singlestoredb_float(satype: Any, nullable: bool = True) -> dt.Float32:
-    return dt.Float32(nullable=nullable)
-
-
-@dt.dtype.register(singlestoredb.TINYINT)
-def singlestoredb_tinyint(satype: Any, nullable: bool = True) -> dt.Int8:
-    return dt.Int8(nullable=nullable)
-
-
-@dt.dtype.register(SingleStoreDBDialect, singlestoredb.YEAR)
-def singlestoredb_year(dialect: Any, satype: Any, nullable: bool = True) -> dt.Int16:
-    return dt.Int16(nullable=nullable)
-
-
-@dt.dtype.register(singlestoredb.BLOB)
-def singlestoredb_blob(satype: Any, nullable: bool = True) -> dt.Binary:
-    return dt.Binary(nullable=nullable)
-
-
-@dt.dtype.register(SingleStoreDBDialect, singlestoredb.BIT)
-def singlestoredb_bit(dialect: Any, satype: Any, nullable: bool = True) -> dt.Binary:
-    return dt.Binary(nullable=nullable)
-
-
-@dt.dtype.register(SingleStoreDBDialect, singlestoredb.BINARY)
-def singlestoredb_binary(dialect: Any, satype: Any, nullable: bool = True) -> dt.Binary:
-    return dt.Binary(nullable=nullable)
-
-
-@dt.dtype.register(SingleStoreDBDialect, singlestoredb.VARBINARY)
-def singlestoredb_varbinary(
-    dialect: Any,
-    satype: Any,
-    nullable: bool = True,
-) -> dt.Binary:
-    return dt.Binary(nullable=nullable)
-
-
-@dt.dtype.register(SingleStoreDBDialect, singlestoredb.LONGBLOB)
-def singlestoredb_longblob(dialect: Any, satype: Any, nullable: bool = True) -> dt.Binary:
-    return dt.Binary(nullable=nullable)
-
-
-@dt.dtype.register(SingleStoreDBDialect, singlestoredb.MEDIUMBLOB)
-def singlestoredb_mediumblob(
-    dialect: Any,
-    satype: Any,
-    nullable: bool = True,
-) -> dt.Binary:
-    return dt.Binary(nullable=nullable)
-
-
-@dt.dtype.register(SingleStoreDBDialect, singlestoredb.TINYBLOB)
-def singlestoredb_tinyblob(dialect: Any, satype: Any, nullable: bool = True) -> dt.Binary:
-    return dt.Binary(nullable=nullable)
-
-
-@dt.dtype.register(SingleStoreDBDialect, singlestoredb.JSON)
-def singlestoredb_json(dialect: Any, satype: Any, nullable: bool = True) -> dt.JSON:
-    return dt.JSON(nullable=nullable)
```

### Comparing `ibis_singlestoredb-0.2.0/ibis_singlestoredb/functions.py` & `ibis_singlestoredb-0.3.0/ibis_singlestoredb/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,11 +385,11 @@
             setattr(types.StringValue, name, eval_func)
         elif isinstance(inputs[0][1], dt.Integer):
             setattr(types.IntegerValue, name, eval_func)
         elif isinstance(inputs[0][1], dt.Floating):
             setattr(types.FloatingValue, name, eval_func)
 
     @ibis.singlestoredb.add_operation(func_type)
-    def _eval_func(t: tr.ExprTranslator, expr: types.Expr) -> types.Expr:
-        return getattr(sa.func, name)(*[t.translate(x) for x in expr.op().args])
+    def _eval_func(t: tr.ExprTranslator, op: ops.ValueOp) -> types.Expr:
+        return getattr(sa.func, name)(*[t.translate(x) for x in op.args])
 
     return eval_func
```

### Comparing `ibis_singlestoredb-0.2.0/ibis_singlestoredb/registry.py` & `ibis_singlestoredb-0.3.0/ibis_singlestoredb/registry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,346 +1,358 @@
-#!/usr/bin/env python
-"""SingleStoreDB function registry."""
 from __future__ import annotations
 
+import contextlib
+import functools
 import operator
+import string
 from typing import Any
-from typing import Callable
+from typing import Dict
 from typing import Optional
 from typing import Sequence
 from typing import Set
+from typing import Union
 
 import ibis
-import ibis.backends.base.sql.compiler.translator as tr
 import ibis.common.exceptions as com
 import ibis.expr.datatypes as dt
 import ibis.expr.operations as ops
 import ibis.expr.types as ir
-import ibis.expr.types.groupby as ig
+import ibis.expr.types.groupby as gby
 import numpy as np
 import pandas as pd
 import sqlalchemy as sa
+from ibis.backends.base.sql.alchemy import AlchemyExprTranslator as ExprTranslator
 from ibis.backends.base.sql.alchemy import fixed_arity
 from ibis.backends.base.sql.alchemy import sqlalchemy_operation_registry
 from ibis.backends.base.sql.alchemy import sqlalchemy_window_functions_registry
 from ibis.backends.base.sql.alchemy import unary
+from ibis.backends.base.sql.alchemy.geospatial import geospatial_supported
+from ibis.backends.base.sql.alchemy.registry import geospatial_functions
+from sqlalchemy.ext.compiler import compiles
+from sqlalchemy.sql.functions import GenericFunction
+
 
 operation_registry = sqlalchemy_operation_registry.copy()
+
+# NOTE: window functions are available from MySQL 8 and MariaDB 10.2
 operation_registry.update(sqlalchemy_window_functions_registry)
 
+if geospatial_supported:
+    operation_registry.update(geospatial_functions)
 
-def _substr(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    f = sa.func.substr
 
-    arg, start, length = expr.op().args
+def _substr(t: ExprTranslator, op: ops.Substring) -> ir.Expr:
+    f = sa.func.substr
 
-    sa_arg = t.translate(arg)
-    sa_start = t.translate(start)
+    sa_arg = t.translate(op.arg)
+    sa_start = t.translate(op.start)
 
-    if length is None:
+    if op.length is None:
         return f(sa_arg, sa_start + 1)
-    else:
-        sa_length = t.translate(length)
-        return f(sa_arg, sa_start + 1, sa_length)
 
+    sa_length = t.translate(op.length)
+    return f(sa_arg, sa_start + 1, sa_length)
 
-def _capitalize(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    (arg,) = expr.op().args
-    sa_arg = t.translate(arg)
+
+def _capitalize(t: ExprTranslator, op: ops.Capitalize) -> ir.Expr:
+    sa_arg = t.translate(op.arg)
     return sa.func.concat(
         sa.func.ucase(sa.func.left(sa_arg, 1)), sa.func.substring(sa_arg, 2),
     )
 
 
-def _extract(fmt: str) -> Callable[[tr.ExprTranslator, ir.Expr], ir.Expr]:
-    def translator(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-        (arg,) = expr.op().args
-        sa_arg = t.translate(arg)
-        if fmt == 'millisecond':
-            return sa.extract('microsecond', sa_arg) % 1000
-        return sa.extract(fmt, sa_arg)
-
-    return translator
-
-
 _truncate_formats = {
     's': '%Y-%m-%d %H:%i:%s',
     'm': '%Y-%m-%d %H:%i:00',
     'h': '%Y-%m-%d %H:00:00',
     'D': '%Y-%m-%d',
     # 'W': 'week',
     'M': '%Y-%m-01',
     'Y': '%Y-01-01',
 }
 
 
-def _truncate(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    arg, unit = expr.op().args
-    sa_arg = t.translate(arg)
+def _truncate(
+    t: ExprTranslator,
+    op: Union[ops.TimestampTruncate, ops.DateTruncate, ops.TimeTruncate],
+) -> ir.Expr:
+    sa_arg = t.translate(op.arg)
     try:
-        fmt = _truncate_formats[unit]
+        fmt = _truncate_formats[op.unit.short]
     except KeyError:
-        raise com.UnsupportedOperationError(
-            f'Unsupported truncate unit {unit}',
-        )
+        raise com.UnsupportedOperationError(f'Unsupported truncate unit {op.unit}')
     return sa.func.date_format(sa_arg, fmt)
 
 
-def _cast(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    arg, typ = expr.op().args
-
+def _cast(t: ExprTranslator, op: ops.Cast) -> ir.Expr:
+    arg = op.arg
+    to = op.to
     sa_arg = t.translate(arg)
-    sa_type = t.get_sqla_type(typ)
+    sa_type = t.get_sqla_type(op.to)
 
     # specialize going from an integer type to a timestamp
-    if isinstance(arg.type(), dt.Integer) and isinstance(sa_type, sa.DateTime):
+    if isinstance(arg.output_dtype, dt.Integer) and isinstance(sa_type, sa.DateTime):
         return sa.func.convert_tz(sa.func.from_unixtime(sa_arg), 'SYSTEM', 'UTC')
 
-    if arg.type().equals(dt.binary) and typ.equals(dt.string):
+    if arg.output_dtype.equals(dt.binary) and to.equals(dt.string):
         return sa.func.hex(sa_arg)
 
-    if typ.equals(dt.binary):
+    if to.equals(dt.binary):
         #  decode yields a column of memoryview which is annoying to deal with
         # in pandas. CAST(expr AS BYTEA) is correct and returns byte strings.
         return sa.cast(sa_arg, sa.LargeBinary())
 
     return sa.cast(sa_arg, sa_type)
 
 
-def _log(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    arg, base = expr.op().args
-    sa_arg = t.translate(arg)
-    sa_base = t.translate(base)
-    return sa.func.log(sa_base, sa_arg)
-
-
-def _identical_to(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    left, right = args = expr.op().args
-    if left.equals(right):
-        return True
-    else:
-        left, right = map(t.translate, args)
-        return left.op('<=>')(right)
-
-
-def _round(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    arg, digits = expr.op().args
-    sa_arg = t.translate(arg)
-
-    if digits is None:
+def _round(t: ExprTranslator, op: ops.Round) -> ir.Expr:
+    sa_arg = t.translate(op.arg)
+    if op.digits is None:
         sa_digits = 0
     else:
-        sa_digits = t.translate(digits)
-
+        sa_digits = t.translate(op.digits)
     return sa.func.round(sa_arg, sa_digits)
 
 
-def _quantile(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    arg, quantile, interpolation = expr.op().args
-    sa_arg = t.translate(arg)
-    sa_quantile = t.translate(quantile)
+def _quantile(t: ExprTranslator, op: ops.Quantile) -> ir.Expr:
+    sa_arg = t.translate(op.arg)
+    sa_quantile = t.translate(op.quantile)
     return sa.func.approx_percentile(sa_arg, sa_quantile)
 
 
-def _floor_divide(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    left, right = map(t.translate, expr.op().args)
-    return sa.func.floor(left / right)
-
-
-def _string_join(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    sep, elements = expr.op().args
-    return sa.func.concat_ws(t.translate(sep), *map(t.translate, elements))
-
-
-def _interval_from_integer(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    arg, unit = expr.op().args
-    if unit in {'ms', 'ns'}:
+def _interval_from_integer(t: ExprTranslator, op: ops.IntervalFromInteger) -> ir.Expr:
+    if op.unit.short in {'ms', 'ns'}:
         raise com.UnsupportedOperationError(
-            'SingleStoreDB does not allow operation '
-            'with INTERVAL offset {}'.format(unit),
+            f'SingloStoreDB does not allow operation with INTERVAL offset {op.unit}',
         )
 
-    sa_arg = t.translate(arg)
-    text_unit = expr.type().resolution.upper()
+    sa_arg = t.translate(op.arg)
+    text_unit = op.output_dtype.resolution.upper()
 
     # XXX: Is there a better way to handle this? I.e. can we somehow use
     # the existing bind parameter produced by translate and reuse its name in
     # the string passed to sa.text?
     if isinstance(sa_arg, sa.sql.elements.BindParameter):
-        return sa.text(f'INTERVAL :arg {text_unit}').bindparams(
-            arg=sa_arg.value,
-        )
+        return sa.text(f'INTERVAL :arg {text_unit}').bindparams(arg=sa_arg.value)
     return sa.text(f'INTERVAL {sa_arg} {text_unit}')
 
 
-def _timestamp_diff(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    left, right = expr.op().args
-    sa_left = t.translate(left)
-    sa_right = t.translate(right)
-    return sa.func.timestampdiff(sa.text('SECOND'), sa_right, sa_left)
-
-
-def _literal(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    if isinstance(expr, ir.IntervalScalar):
-        if expr.type().unit in {'ms', 'ns'}:
+def _literal(t: ExprTranslator, op: ops.Literal) -> ir.Expr:
+    if op.output_dtype.is_interval():
+        if op.output_dtype.unit.short in {'ms', 'ns'}:
             raise com.UnsupportedOperationError(
-                'SingleStoreDB does not allow operation '
-                'with INTERVAL offset {}'.format(expr.type().unit),
+                'SingloStoreDB does not allow operation '
+                f'with INTERVAL offset {op.output_dtype.unit}',
             )
-        text_unit = expr.type().resolution.upper()
-        value = expr.op().value
-        return sa.text(f'INTERVAL :value {text_unit}').bindparams(value=value)
-    elif isinstance(expr, ir.SetScalar):
-        return list(map(sa.literal, expr.op().value))
+        text_unit = op.output_dtype.resolution.upper()
+        sa_text = sa.text(f'INTERVAL :value {text_unit}')
+        return sa_text.bindparams(value=op.value)
+
+    elif op.output_dtype.is_binary():
+        # the cast to BINARY is necessary here, otherwise the data come back as
+        # Python strings
+        #
+        # This lets the database handle encoding rather than ibis
+        return sa.cast(sa.literal(op.value), type_=sa.BINARY())
+
+    value = op.value
+    with contextlib.suppress(AttributeError):
+        value = value.to_pydatetime()
+
+    return sa.literal(value)
+
+
+def _group_concat(t: ExprTranslator, op: ops.GroupConcat) -> ir.Expr:
+    if op.where is not None:
+        arg = t.translate(ops.Where(op.where, op.arg, ibis.NA))
     else:
-        value = expr.op().value
-        if isinstance(value, pd.Timestamp):
-            value = value.to_pydatetime()
-        return sa.literal(value)
-
-
-def _random(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    return sa.func.random()
-
-
-def _group_concat(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    op = expr.op()
-    arg, sep, where = op.args
-    if where is not None:
-        case = where.ifelse(arg, ibis.NA)
-        arg = t.translate(case)
-    else:
-        arg = t.translate(arg)
-    return sa.func.group_concat(arg.op('SEPARATOR')(t.translate(sep)))
+        arg = t.translate(op.arg)
+    sep = t.translate(op.sep)
+    return sa.func.group_concat(arg.op('SEPARATOR')(sep))
 
 
-def _day_of_week_index(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    (arg,) = expr.op().args
-    left = sa.func.dayofweek(t.translate(arg)) - 2
-    right = 7
-    return ((left % right) + right) % right
+def _json_get_item(t: ExprTranslator, op: ops.JSONGetItem) -> ir.Expr:
+    arg = t.translate(op.arg)
+    index = t.translate(op.index)
+    if op.index.output_dtype.is_integer():
+        path = '$[' + sa.cast(index, sa.TEXT) + ']'
+    else:
+        path = '$.' + index
+    return sa.func.json_extract(arg, path)
 
 
-def _day_of_week_name(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    (arg,) = expr.op().args
-    return sa.func.dayname(t.translate(arg))
+class _singlestoredb_trim(GenericFunction):
+    inherit_cache = True
 
+    def __init__(self, input: ir.Expr, side: str) -> None:
+        super().__init__(input)
+        self.type = sa.VARCHAR()
+        self.side = side
+
+
+@compiles(_singlestoredb_trim, 'singlestoredb')
+def compiles_singlestoredb_trim(
+    element: ir.Expr,
+    compiler: Any,
+    **kw: Dict[str, Any],
+) -> ir.Expr:
+    arg = compiler.function_argspec(element, **kw)
+    side = element.side.upper()
+    # has to be called once for every whitespace character because singlestoredb
+    # interprets `char` literally, not as a set of characters like Python
+    return functools.reduce(
+        lambda arg, char: f"TRIM({side} '{char}' FROM {arg})", string.whitespace, arg,
+    )
 
-def _string_find(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    op = expr.op()
 
+def _string_find(t: ExprTranslator, op: ops.StringFind) -> ir.Expr:
     if op.end is not None:
         raise NotImplementedError('`end` not yet implemented')
 
     if op.start is not None:
         return sa.func.locate(
             t.translate(op.substr),
             t.translate(op.arg),
             t.translate(op.start),
         ) - 1
 
     return sa.func.locate(t.translate(op.substr), t.translate(op.arg)) - 1
 
 
-def _string_contains(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    return _string_find(t, expr) >= 0
+def _string_contains(t: ExprTranslator, op: ops.StringContains) -> ir.Expr:
+    return (sa.func.locate(t.translate(op.needle), t.translate(op.haystack)) - 1) >= 0
 
 
-def _approx_median(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    args = expr.op().args
-    return sa.func.median(t.translate(args[0]))
+def _approx_median(t: ExprTranslator, op: ops.ApproxMedian) -> ir.Expr:
+    return sa.func.median(t.translate(op.arg))
 
 
-def _regex_search(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    args = expr.op().args
-    return sa.func.regexp_instr(*[t.translate(x) for x in args], sa.literal('g')) > 0
+def _regex_search(t: ExprTranslator, op: ops.RegexSearch) -> ir.Expr:
+    args = (op.arg, op.pattern)
+    return sa.type_coerce(
+        sa.func.regexp_instr(*[t.translate(x) for x in args], sa.literal('g')) > 0,
+        sa.BOOLEAN,
+    )
 
 
-def _regex_replace(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
+def _regex_replace(t: ExprTranslator, op: ops.RegexReplace) -> ir.Expr:
     # TODO: Requires regexp_format='advanced'
-    args = expr.op().args
+    args = (op.arg, op.pattern, op.replacement)
     return sa.func.regexp_replace(*[t.translate(x) for x in args], sa.literal('g'))
 
 
-def _regex_extract(t: tr.ExprTranslator, expr: ir.Expr) -> ir.Expr:
-    args = expr.op().args
+def _regex_extract(t: ExprTranslator, op: ops.RegexExtract) -> ir.Expr:
+    args = (op.arg, op.pattern, op.index)
     return sa.func.regexp_extract(*[t.translate(x) for x in args], sa.literal('g'))
 
 
 operation_registry.update(
     {
         ops.Literal: _literal,
+        ops.Cast: _cast,
         ops.IfNull: fixed_arity(sa.func.ifnull, 2),
+        # static checks are not happy with using "if" as a property
+        ops.Where: fixed_arity(getattr(sa.func, 'if'), 3),
         # strings
         ops.Substring: _substr,
         ops.StringFind: _string_find,
         ops.StringContains: _string_contains,
         ops.Capitalize: _capitalize,
+        ops.FindInSet: (
+            lambda t, op: (
+                sa.func.find_in_set(
+                    t.translate(op.needle),
+                    sa.func.concat_ws(',', *map(t.translate, op.values)),
+                )
+                - 1
+            )
+        ),
+        # LIKE in singlestoredb is case insensitive
+        ops.StartsWith: fixed_arity(
+            lambda arg, start: sa.type_coerce(
+                arg.op('LIKE BINARY')(sa.func.concat(start, '%')), sa.BOOLEAN(),
+            ),
+            2,
+        ),
+        ops.EndsWith: fixed_arity(
+            lambda arg, end: sa.type_coerce(
+                arg.op('LIKE BINARY')(sa.func.concat('%', end)), sa.BOOLEAN(),
+            ),
+            2,
+        ),
         ops.RegexSearch: _regex_search,
         ops.RegexReplace: _regex_replace,
         ops.RegexExtract: _regex_extract,
-        ops.Cast: _cast,
         # math
-        ops.Log: _log,
+        ops.Log: fixed_arity(lambda arg, base: sa.func.log(base, arg), 2),
         ops.Log2: unary(sa.func.log2),
         ops.Log10: unary(sa.func.log10),
         ops.Round: _round,
-        ops.RandomScalar: _random,
         ops.Quantile: _quantile,
         # dates and times
-        ops.Date: unary(sa.func.date),
         ops.DateAdd: fixed_arity(operator.add, 2),
         ops.DateSub: fixed_arity(operator.sub, 2),
         ops.DateDiff: fixed_arity(sa.func.datediff, 2),
         ops.TimestampAdd: fixed_arity(operator.add, 2),
         ops.TimestampSub: fixed_arity(operator.sub, 2),
-        ops.TimestampDiff: _timestamp_diff,
+        ops.TimestampDiff: fixed_arity(
+            lambda left, right: sa.func.timestampdiff(sa.text('SECOND'), right, left), 2,
+        ),
+        ops.StringToTimestamp: fixed_arity(
+            lambda arg, format_str: sa.func.str_to_date(arg, format_str), 2,
+        ),
         ops.DateTruncate: _truncate,
         ops.TimestampTruncate: _truncate,
         ops.IntervalFromInteger: _interval_from_integer,
         ops.Strftime: fixed_arity(sa.func.date_format, 2),
-        ops.ExtractYear: _extract('year'),
-        ops.ExtractMonth: _extract('month'),
-        ops.ExtractDay: _extract('day'),
-        ops.ExtractDayOfYear: unary('dayofyear'),
-        ops.ExtractQuarter: _extract('quarter'),
-        ops.ExtractEpochSeconds: unary('UNIX_TIMESTAMP'),
-        ops.ExtractWeekOfYear: fixed_arity('weekofyear', 1),
-        ops.ExtractHour: _extract('hour'),
-        ops.ExtractMinute: _extract('minute'),
-        ops.ExtractSecond: _extract('second'),
-        ops.ExtractMillisecond: _extract('millisecond'),
+        ops.ExtractDayOfYear: unary(sa.func.dayofyear),
+        ops.ExtractEpochSeconds: unary(sa.func.UNIX_TIMESTAMP),
+        ops.ExtractWeekOfYear: unary(sa.func.weekofyear),
+        ops.ExtractMillisecond: fixed_arity(
+            lambda arg: sa.func.floor(sa.extract('microsecond', arg) / 1000), 1,
+        ),
+        ops.TimestampNow: fixed_arity(sa.func.now, 0),
         # reductions
         ops.ApproxMedian: _approx_median,
-        #       ops.BitAnd: reduction(sa.func.bit_and),
-        #       ops.BitOr: reduction(sa.func.bit_or),
-        #       ops.BitXor: reduction(sa.func.bit_xor),
-        #       ops.Variance: variance_reduction('var'),
-        #       ops.StandardDev: variance_reduction('stddev'),
-        #       ops.IdenticalTo: _identical_to,
-        #       ops.TimestampNow: fixed_arity(sa.func.now, 0),
         # others
         ops.GroupConcat: _group_concat,
-        ops.DayOfWeekIndex: _day_of_week_index,
-        ops.DayOfWeekName: _day_of_week_name,
-        #       ops.HLLCardinality: reduction(
-        #           lambda arg: sa.func.count(arg.distinct()),
-        #       ),
+        ops.DayOfWeekIndex: fixed_arity(
+            lambda arg: (sa.func.dayofweek(arg) + 5) % 7, 1,
+        ),
+        ops.DayOfWeekName: fixed_arity(lambda arg: sa.func.dayname(arg), 1),
+        ops.JSONGetItem: _json_get_item,
+        ops.Strip: unary(lambda arg: _singlestoredb_trim(arg, 'both')),
+        ops.LStrip: unary(lambda arg: _singlestoredb_trim(arg, 'leading')),
+        ops.RStrip: unary(lambda arg: _singlestoredb_trim(arg, 'trailing')),
     },
 )
 
+_invalid_operations = {
+    ops.CumulativeAll,
+    ops.CumulativeAny,
+    ops.CumulativeMax,
+    ops.CumulativeMean,
+    ops.CumulativeMin,
+    ops.CumulativeSum,
+    ops.NTile,
+}
+
+operation_registry = {
+    k: v for k, v in operation_registry.items() if k not in _invalid_operations
+}
+
 
 def _describe_table(
     self: Any,
     percentiles: Sequence[float] = [0.25, 0.5, 0.75],
     include: Optional[Sequence[Any]] = None,
     exclude: Optional[Sequence[Any]] = None,
     datetime_is_numeric: bool = False,
     stats: Optional[Sequence[str]] = None,
-    by: Optional[Sequence[str | ir.Expr]] = None,
+    by: Optional[Sequence[Union[str, ir.Expr]]] = None,
     having: Optional[Sequence[ir.Expr]] = None,
 ) -> ir.TableExpr:
     """
     Compute descriptive statistics.
 
     Note that since all statistics are stored in columns, there can
     be mixed data types represented in some columns such as ``min``,
@@ -405,15 +417,15 @@
 
     if exclude is None:
         exclude = []
     elif not isinstance(exclude, Sequence) or isinstance(exclude, str):
         exclude = [exclude]
 
     include_map = {
-        np.object: 'object', np.datetime64: 'datetime',
+        np.datetime64: 'datetime',
         'datetime64': 'datetime', np.timedelta64: 'timedelta',
         'timedelta64': 'timedelta', 'category': 'object',
         'datetimetz': 'datetime', 'datetime64[ns, tz]': 'datetime',
         int: 'int', 'i': 'int', float: 'float', 'f': 'float',
         str: 'string', 'str': 'string', bytes: 'binary',
         'bytes': 'binary', 'O': 'object',
     }
@@ -461,15 +473,15 @@
         )
 
     # Compute stats list
     type_stats: Set[str] = set()
     for name, dtype in include_vars:
         if isinstance(dtype, (dt.Timestamp, dt.Date, dt.Time, dt.Interval)):
             type_stats = type_stats.union(dt_stats)
-        elif isinstance(dtype, (dt.String, dt.Binary, dt.Set, dt.Enum)):
+        elif isinstance(dtype, (dt.String, dt.Binary, dt.Array, dt.Enum)):
             type_stats = type_stats.union(str_stats)
         else:
             type_stats = type_stats.union(num_stats)
 
     stats = [
         x for x in [
             'count', 'unique', 'mean', 'median', 'std', 'var',
@@ -565,15 +577,15 @@
     TableExpr
 
     """
     return self.table.describe(*args, by=self.by, having=self._having, **kwargs)\
                      .select(lambda x: x).sort_by([x.get_name() for x in self.by])
 
 
-ig.GroupedTable.describe = _grouped_describe
+gby.GroupedTable.describe = _grouped_describe
 
 
 def _describe_column(
     self: Any,
     percentiles: Sequence[float] = [0.25, 0.5, 0.75],
     datetime_is_numeric: bool = False,
     stats: Optional[Sequence[str]] = None,
@@ -618,17 +630,17 @@
 
 
 ir.AnyColumn.head = _head_column
 
 
 def _drop_duplicates(
     self: Any,
-    subset: Optional[str | Sequence[str]] = None,
+    subset: Optional[Union[str, Sequence[str]]] = None,
     keep: str = 'first',
-    order_by: Optional[str | Sequence[str] | ir.Expr] = None,
+    order_by: Optional[Union[str, Sequence[str], ir.Expr]] = None,
 ) -> ir.Table:
     """
     Drop rows with duplicate values.
 
     Parameters
     ----------
     subset : str or list-of-strs, optional
```

### Comparing `ibis_singlestoredb-0.2.0/ibis_singlestoredb/tests/conftest.py` & `ibis_singlestoredb-0.3.0/ibis_singlestoredb/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ibis_singlestoredb-0.2.0/ibis_singlestoredb/tests/datatypes.csv` & `ibis_singlestoredb-0.3.0/ibis_singlestoredb/tests/datatypes.csv`

 * *Files identical despite different names*

### Comparing `ibis_singlestoredb-0.2.0/ibis_singlestoredb/tests/test.sql` & `ibis_singlestoredb-0.3.0/ibis_singlestoredb/tests/test.sql`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     varchar42_c varchar(42),
     longtext_c longtext,
     mediumtext_c mediumtext,
     tinytext_c tinytext,
     text_c text,
     text4_c text(4),
     blob_c blob,
-    enum_sml_c enum('s', 'm', 'l'),
+    enum_sml_c enum('small', 'medium', 'large'),
     set_abcd_c set('a', 'b', 'c', 'd'),
     negative_int_c int,
     negative_float_c float,
     bool_c bool
 );
 
 load data local infile '{{TEST_PATH}}/datatypes.csv' into table datatypes
```

### Comparing `ibis_singlestoredb-0.2.0/ibis_singlestoredb/tests/test_client.py` & `ibis_singlestoredb-0.3.0/ibis_singlestoredb/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `ibis_singlestoredb-0.2.0/ibis_singlestoredb/tests/test_op_matrix.py` & `ibis_singlestoredb-0.3.0/ibis_singlestoredb/tests/test_op_matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     # Min
     ('min()', lambda x: x.min()),
     # Modulus
     ('mod()', lambda x: x.mod(8)),
     # Multiply
     ('mul()', lambda x: x.mul(3)),
     # NTile
-    ('ntile()', lambda x: x.ntile(2)),
+    # ('ntile()', lambda x: x.ntile(2)),
     # Negate
     ('negate()', lambda x: x.negate()),
     # NotAll
     # NotAny
     # NotContains
     # NotEquals
     # NotNull
@@ -275,8 +275,9 @@
 def test_operations(con, operation, column, ibis_operation):
     datatypes = con.table('datatypes')
 
     try:
         ibis_operation(getattr(datatypes, column)).name('_').execute()
     except AttributeError:
         return
+
     print(operation, 'is supported for', column)
```

### Comparing `ibis_singlestoredb-0.2.0/ibis_singlestoredb/tests/test_ops.py` & `ibis_singlestoredb-0.3.0/ibis_singlestoredb/tests/test_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,16 +460,22 @@
         ibis_result = result[i]
         expected_result = expected_operation(value)
 
         if test_name == 'abs()' and type(ibis_result) == float:
             ibis_result = truncate(ibis_result, 2)
             expected_result = truncate(expected_result, 2)
 
-        if test_name == 'add()' and type(ibis_result) == float:
+        elif test_name == 'add()' and type(ibis_result) == float:
             if column == 'decimal5_c':
                 ibis_result = round(ibis_result, 3)
                 expected_result = round(expected_result, 3)
             else:
                 ibis_result = truncate(ibis_result, 3)
                 expected_result = truncate(expected_result, 3)
 
+        elif test_name == 'cast()' and type(ibis_result) == str \
+                and ('float_c' in column or 'timestamp_c' in column):
+            max_len = min(len(ibis_result), len(expected_result))
+            ibis_result = ibis_result[:max_len-1]
+            expected_result = expected_result[:max_len-1]
+
         assert ibis_result == expected_result
```

### Comparing `ibis_singlestoredb-0.2.0/ibis_singlestoredb.egg-info/PKG-INFO` & `ibis_singlestoredb-0.3.0/ibis_singlestoredb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibis-singlestoredb
-Version: 0.2.0
+Version: 0.3.0
 Summary: Ibis backend for the SingleStore database
 Home-page: https://github.com/singlestore-labs/ibis-singlestoredb
 Author: SingleStore
 Author-email: support@singlestore.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ibis_singlestoredb-0.2.0/ibis_singlestoredb.egg-info/SOURCES.txt` & `ibis_singlestoredb-0.3.0/ibis_singlestoredb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibis_singlestoredb-0.2.0/setup.cfg` & `ibis_singlestoredb-0.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ibis_singlestoredb
-version = 0.2.0
+version = 0.3.0
 description = Ibis backend for the SingleStore database
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/singlestore-labs/ibis-singlestoredb
 author = SingleStore
 author_email = support@singlestore.com
 license = Apache-2.0
@@ -18,15 +18,15 @@
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Database
 
 [options]
 packages = find:
 install_requires = 
-	ibis-framework>=3.0.0,<4.0.0dev
+	ibis-framework>=5.1.0,<6.0.0dev
 	singlestoredb>=0.5.1
 	sqlalchemy-singlestoredb>=0.2.0
 python_requires = >=3.8
 tests_require = 
 	pytest
 	coverage
 	nose2
```

