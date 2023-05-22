# Comparing `tmp/peewee_migrate-1.7.1.tar.gz` & `tmp/peewee_migrate-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_migrate-1.7.1.tar", max compression
+gzip compressed data, was "peewee_migrate-1.7.2.tar", max compression
```

## Comparing `peewee_migrate-1.7.1.tar` & `peewee_migrate-1.7.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4456 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/README.rst
--rw-r--r--   0        0        0      146 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/__init__.py
--rw-r--r--   0        0        0       78 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/__main__.py
--rw-r--r--   0        0        0    11993 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/auto.py
--rw-r--r--   0        0        0     6597 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/cli.py
--rw-r--r--   0        0        0      146 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/logs.py
--rw-r--r--   0        0        0    15733 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/migrator.py
--rw-r--r--   0        0        0      465 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/models.py
--rw-r--r--   0        0        0        0 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/py.typed
--rw-r--r--   0        0        0    12194 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/router.py
--rw-r--r--   0        0        0     1681 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/template.py
--rw-r--r--   0        0        0      255 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/peewee_migrate/types.py
--rw-r--r--   0        0        0     1600 2023-04-11 12:31:16.306499 peewee_migrate-1.7.1/pyproject.toml
--rw-r--r--   0        0        0     5690 1970-01-01 00:00:00.000000 peewee_migrate-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     4456 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/README.rst
+-rw-r--r--   0        0        0      146 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/__main__.py
+-rw-r--r--   0        0        0    11875 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/auto.py
+-rw-r--r--   0        0        0     6597 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/cli.py
+-rw-r--r--   0        0        0      146 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/logs.py
+-rw-r--r--   0        0        0    15789 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/migrator.py
+-rw-r--r--   0        0        0      465 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/models.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/py.typed
+-rw-r--r--   0        0        0    12235 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/router.py
+-rw-r--r--   0        0        0     1723 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/template.py
+-rw-r--r--   0        0        0      249 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/types.py
+-rw-r--r--   0        0        0     1589 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.7.2/PKG-INFO
```

### Comparing `peewee_migrate-1.7.1/README.rst` & `peewee_migrate-1.7.2/README.rst`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.1/peewee_migrate/auto.py` & `peewee_migrate-1.7.2/peewee_migrate/auto.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Automatically create migrations."""
 from __future__ import annotations
 
-from collections.abc import Hashable
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Dict,
     Final,
     Iterable,
@@ -82,18 +81,18 @@
             find_field_type(field),
             field.field_type,
             field.null,
             primary_key=field.primary_key,
             column_name=field.column_name,
             index=field.index,
             unique=field.unique,
-            extra_parameters=None,
+            **kwargs,
         )
         if field.default is not None and not callable(field.default):
-            self.default = repr(field.default)
+            self.default = repr(field.db_value(field.default))
 
         if self.field_class in FIELD_TO_PARAMS:
             if self.extra_parameters is None:  # type: ignore[has-type]
                 self.extra_parameters = {}
 
             self.extra_parameters.update(FIELD_TO_PARAMS[self.field_class](field))
 
@@ -113,19 +112,24 @@
         field = super(Column, self).get_field()
         module = FIELD_MODULES_MAP.get(self.field_class.__name__, "pw")
         name, _, field = [s and s.strip() for s in field.partition("=")]
         return "{name}{space}={space}{module}.{field}".format(
             name=name, field=field, space=space, module=module
         )
 
-    def get_field_parameters(self) -> TParams:
+    def get_field_parameters(self, *, indexes=False) -> TParams:
         """Generate parameters for self field."""
         params = super(Column, self).get_field_parameters()
         if self.default is not None:
             params["default"] = self.default
+
+        params.pop("backref", None)
+        if indexes:
+            params["unique"] = bool(params.pop("unique", False))
+            params["index"] = bool(params.pop("index", False)) or params["unique"]
         return params
 
 
 def diff_one(model1: TModelType, model2: TModelType, **kwargs) -> List[str]:  # noqa:
     """Find difference between given peewee models."""
     changes = []
 
@@ -149,32 +153,33 @@
     nulls_ = []
     indexes_ = []
     for name in set(field_names1) - names1 - names2:
         field1, field2 = field_names1[name], field_names2[name]
         diff = compare_fields(field1, field2)
         null = diff.pop("null", None)
         index = diff.pop("index", None)
+        unique = diff.pop("unique", None)
 
         if diff:
             fields_.append(field1)
 
         if null is not None:
             nulls_.append((name, null))
 
-        if index is not None:
-            indexes_.append((name, index[0], index[1]))
+        if (index is not None) or (unique is not None):
+            indexes_.append((name, index, unique))
 
     if fields_:
         changes.append(change_fields(model1, *fields_, **kwargs))
 
     for name, null in nulls_:
         changes.append(change_not_null(model1, name, null=null))
 
     for name, index, unique in indexes_:
-        if index is True or unique is True:
+        if (index is True) or (unique is True):
             if field_names2[name].unique or field_names2[name].index:
                 changes.append(drop_index(model1, name))
             changes.append(add_index(model1, name, unique=unique))
         else:
             changes.append(drop_index(model1, name))
 
     # Check additional compound indexes
@@ -292,49 +297,33 @@
         meta.table_name,
         ", ".join(map(repr, fields)),
     )
 
 
 def field_to_code(field: pw.Field, *, space: bool = True, **kwargs) -> str:
     """Generate field description."""
-    col = Column(field, **kwargs)
+    col = Column(field)
     return col.get_field(" " if space else "")
 
 
-def compare_fields(field1: pw.Field, field2: pw.Field, **kwargs) -> Dict:
+def compare_fields(field1: pw.Field, field2: pw.Field) -> Dict:
     """Find diffs between the given fields."""
     ftype1, ftype2 = find_field_type(field1), find_field_type(field2)
     if ftype1 != ftype2:
         return {"cls": True}
 
-    params1 = field_to_params(field1)
-    params1["null"] = field1.null
-    params2 = field_to_params(field2)
-    params2["null"] = field2.null
-
+    col1, col2 = Column(
+        field1, extra_parameters={"index": field1.index, "unique": field1.unique}
+    ), Column(field2, extra_parameters={"index": field2.index, "unique": field2.unique})
+    params1, params2 = col1.get_field_parameters(indexes=True), col2.get_field_parameters(
+        indexes=True
+    )
     return dict(set(params1.items()) - set(params2.items()))
 
 
-def field_to_params(field: pw.Field, **kwargs) -> TParams:
-    """Generate params for the given field."""
-    ftype = find_field_type(field)
-    params = FIELD_TO_PARAMS.get(ftype, lambda f: {})(field)
-    if (
-        field.default is not None
-        and not callable(field.default)
-        and isinstance(field.default, Hashable)
-    ):
-        params["default"] = field.default
-
-    params["index"] = field.index and not field.unique, field.unique
-
-    params.pop("backref", None)  # Ignore backref
-    return params
-
-
 def change_fields(model_cls: TModelType, *fields: pw.Field, **kwargs) -> str:
     """Generate migrations to change fields."""
     meta = model_cls._meta  # type: ignore[]
     return "migrator.change_fields('%s', %s)" % (
         meta.table_name,
         ("," + NEWLINE).join([field_to_code(f, space=False) for f in fields]),
     )
```

### Comparing `peewee_migrate-1.7.1/peewee_migrate/cli.py` & `peewee_migrate-1.7.2/peewee_migrate/cli.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.1/peewee_migrate/migrator.py` & `peewee_migrate-1.7.2/peewee_migrate/migrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
+    Dict,
     List,
     Union,
     cast,
     overload,
 )
 
 import peewee as pw
@@ -132,16 +133,16 @@
         return self._update_column(table, column, fn)  # type: ignore[]
 
 
 class ORM:
     __slots__ = ("__tables__", "__models__")
 
     def __init__(self):
-        self.__tables__ = {}
-        self.__models__ = {}
+        self.__tables__: Dict[str, TModelType] = {}
+        self.__models__: Dict[str, TModelType] = {}
 
     def add(self, model: TModelType):
         self.__models__[model.__name__] = model
         self.__tables__[model._meta.table_name] = model  # type: ignore[]
 
     def remove(self, model: TModelType):
         del self.__models__[model.__name__]
```

### Comparing `peewee_migrate-1.7.1/peewee_migrate/router.py` & `peewee_migrate-1.7.2/peewee_migrate/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 from .migrator import Migrator
 from .models import MIGRATE_TABLE, MigrateHistory
 from .template import TEMPLATE
 
 if TYPE_CHECKING:
     from logging import Logger
 
+    from peewee_migrate.types import TModelType
+
 
 CLEAN_RE: Final = re.compile(r"\s+$", re.M)
 CURDIR: Final = Path.cwd()
 DEFAULT_MIGRATE_DIR: Final = CURDIR / "migrations"
 
 
 def void(m, d, fake=None):
@@ -147,19 +149,15 @@
         return None
 
     def clear(self):
         """Clear migrations."""
         self.model.delete().execute()
 
     def compile(  # noqa:
-        self,
-        name: str,
-        migrate: str = "",
-        rollback: str = "",
-        num: Optional[int] = None,
+        self, name: str, migrate: str = "", rollback: str = "", num: Optional[int] = None
     ) -> str:
         """Create a migration."""
         raise NotImplementedError
 
     def read(self, name: str):
         """Read migration from file."""
         raise NotImplementedError
@@ -359,15 +357,15 @@
 
 
 def _check_model(obj):
     """Check object if it's a peewee model and unique."""
     return isinstance(obj, type) and issubclass(obj, pw.Model) and hasattr(obj, "_meta")
 
 
-def compile_migrations(migrator: Migrator, models, *, reverse=False):
+def compile_migrations(migrator: Migrator, models: List[TModelType], *, reverse=False) -> str:
     """Compile migrations for given models."""
     source = list(migrator.orm)
     if reverse:
         source, models = models, source
 
     migrations = diff_many(models, source, migrator, reverse=reverse)
     if not migrations:
```

### Comparing `peewee_migrate-1.7.1/peewee_migrate/template.py` & `peewee_migrate-1.7.2/peewee_migrate/template.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Basic template for migration file."""
+
 from __future__ import annotations
 
 TEMPLATE = """\
 \"\"\"Peewee migrations -- {name}.
 
 Some examples (model - class or model name)::
```

### Comparing `peewee_migrate-1.7.1/pyproject.toml` & `peewee_migrate-1.7.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "peewee-migrate"
-version = "1.7.1"
+version = "1.7.2"
 homepage = "https://github.com/klen/peewee_migrate"
 repository = "https://github.com/klen/peewee_migrate"
 description = "Support for migrations in Peewee ORM"
 readme = "README.rst"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["peewee", "migrations", "orm"]
 classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-    "Topic :: Utilities",
+  "Development Status :: 5 - Production/Stable",
+  "Intended Audience :: Developers",
+  "License :: OSI Approved :: MIT License",
+  "Programming Language :: Python",
+  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3.8",
+  "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
+  "Topic :: Software Development :: Libraries :: Python Modules",
+  "Topic :: Utilities",
 ]
 
 [tool.poetry.scripts]
 pw_migrate = "peewee_migrate.cli:cli"
 pw-migrate = "peewee_migrate.cli:cli"
 
 [tool.poetry.dependencies]
@@ -39,15 +39,15 @@
 pytest-mypy = "*"
 ruff = "*"
 
 [tool.ruff]
 line-length = 100
 target-version = "py38"
 select = ["ALL"]
-ignore = ["ANN", "ARG", "COM", "D", "N", "UP", "S", "SLF", "INP001"]
+ignore = ["ANN", "ARG", "COM", "D", "N", "UP", "S", "SLF", "INP001", "PLR2004"]
 
 [tool.pytest.ini_options]
 addopts = "-svx --mypy"
 
 [tool.mypy]
 packages = ["peewee_migrate"]
 ignore_missing_imports = true
```

### Comparing `peewee_migrate-1.7.1/PKG-INFO` & `peewee_migrate-1.7.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-migrate
-Version: 1.7.1
+Version: 1.7.2
 Summary: Support for migrations in Peewee ORM
 Home-page: https://github.com/klen/peewee_migrate
 License: MIT
 Keywords: peewee,migrations,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -13,19 +13,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Dist: click
 Requires-Dist: peewee (>=3,<4)
 Project-URL: Repository, https://github.com/klen/peewee_migrate
 Description-Content-Type: text/x-rst
```

