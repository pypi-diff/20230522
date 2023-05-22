# Comparing `tmp/peewee_migrate-1.7.2.tar.gz` & `tmp/peewee_migrate-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_migrate-1.7.2.tar", max compression
+gzip compressed data, was "peewee_migrate-1.7.3.tar", max compression
```

## Comparing `peewee_migrate-1.7.2.tar` & `peewee_migrate-1.7.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4456 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/README.rst
--rw-r--r--   0        0        0      146 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/__init__.py
--rw-r--r--   0        0        0       78 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/__main__.py
--rw-r--r--   0        0        0    11875 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/auto.py
--rw-r--r--   0        0        0     6597 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/cli.py
--rw-r--r--   0        0        0      146 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/logs.py
--rw-r--r--   0        0        0    15789 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/migrator.py
--rw-r--r--   0        0        0      465 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/models.py
--rw-r--r--   0        0        0        0 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/py.typed
--rw-r--r--   0        0        0    12235 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/router.py
--rw-r--r--   0        0        0     1723 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/template.py
--rw-r--r--   0        0        0      249 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/peewee_migrate/types.py
--rw-r--r--   0        0        0     1589 2023-05-22 16:05:20.522392 peewee_migrate-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0     4456 2023-05-22 16:59:32.423129 peewee_migrate-1.7.3/README.rst
+-rw-r--r--   0        0        0      146 2023-05-22 16:59:32.423129 peewee_migrate-1.7.3/peewee_migrate/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-22 16:59:32.423129 peewee_migrate-1.7.3/peewee_migrate/__main__.py
+-rw-r--r--   0        0        0    12219 2023-05-22 16:59:32.423129 peewee_migrate-1.7.3/peewee_migrate/auto.py
+-rw-r--r--   0        0        0     6597 2023-05-22 16:59:32.423129 peewee_migrate-1.7.3/peewee_migrate/cli.py
+-rw-r--r--   0        0        0      146 2023-05-22 16:59:32.423129 peewee_migrate-1.7.3/peewee_migrate/logs.py
+-rw-r--r--   0        0        0    15789 2023-05-22 16:59:32.423129 peewee_migrate-1.7.3/peewee_migrate/migrator.py
+-rw-r--r--   0        0        0      465 2023-05-22 16:59:32.423129 peewee_migrate-1.7.3/peewee_migrate/models.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:59:32.423129 peewee_migrate-1.7.3/peewee_migrate/py.typed
+-rw-r--r--   0        0        0    12235 2023-05-22 16:59:32.423129 peewee_migrate-1.7.3/peewee_migrate/router.py
+-rw-r--r--   0        0        0     1723 2023-05-22 16:59:32.423129 peewee_migrate-1.7.3/peewee_migrate/template.py
+-rw-r--r--   0        0        0      249 2023-05-22 16:59:32.423129 peewee_migrate-1.7.3/peewee_migrate/types.py
+-rw-r--r--   0        0        0     1589 2023-05-22 16:59:32.423129 peewee_migrate-1.7.3/pyproject.toml
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.7.3/PKG-INFO
```

### Comparing `peewee_migrate-1.7.2/README.rst` & `peewee_migrate-1.7.3/README.rst`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.2/peewee_migrate/auto.py` & `peewee_migrate-1.7.3/peewee_migrate/auto.py`

 * *Files 9% similar despite different names*

```diff
@@ -83,15 +83,20 @@
             field.null,
             primary_key=field.primary_key,
             column_name=field.column_name,
             index=field.index,
             unique=field.unique,
             **kwargs,
         )
-        if field.default is not None and not callable(field.default):
+
+        if (
+            field.default is not None
+            and not callable(field.default)
+            and not isinstance(field.default, pw.Node)
+        ):
             self.default = repr(field.db_value(field.default))
 
         if self.field_class in FIELD_TO_PARAMS:
             if self.extra_parameters is None:  # type: ignore[has-type]
                 self.extra_parameters = {}
 
             self.extra_parameters.update(FIELD_TO_PARAMS[self.field_class](field))
@@ -112,24 +117,28 @@
         field = super(Column, self).get_field()
         module = FIELD_MODULES_MAP.get(self.field_class.__name__, "pw")
         name, _, field = [s and s.strip() for s in field.partition("=")]
         return "{name}{space}={space}{module}.{field}".format(
             name=name, field=field, space=space, module=module
         )
 
-    def get_field_parameters(self, *, indexes=False) -> TParams:
+    def get_field_parameters(self, *, indexes=False, constraints=True) -> TParams:
         """Generate parameters for self field."""
         params = super(Column, self).get_field_parameters()
         if self.default is not None:
             params["default"] = self.default
 
         params.pop("backref", None)
         if indexes:
             params["unique"] = bool(params.pop("unique", False))
             params["index"] = bool(params.pop("index", False)) or params["unique"]
+
+        if not constraints:
+            params.pop("constraints", None)
+
         return params
 
 
 def diff_one(model1: TModelType, model2: TModelType, **kwargs) -> List[str]:  # noqa:
     """Find difference between given peewee models."""
     changes = []
 
@@ -145,40 +154,40 @@
 
     # Drop fields
     names2 = set(field_names2) - set(field_names1)
     if names2:
         changes.append(drop_fields(model1, *names2))
 
     # Change fields
-    fields_ = []
-    nulls_ = []
-    indexes_ = []
+    fields_to_change = []
+    fields_nulls = []
+    fields_indexes = []
     for name in set(field_names1) - names1 - names2:
         field1, field2 = field_names1[name], field_names2[name]
         diff = compare_fields(field1, field2)
         null = diff.pop("null", None)
         index = diff.pop("index", None)
         unique = diff.pop("unique", None)
 
         if diff:
-            fields_.append(field1)
+            fields_to_change.append((field1, diff))
 
         if null is not None:
-            nulls_.append((name, null))
+            fields_nulls.append((name, null))
 
         if (index is not None) or (unique is not None):
-            indexes_.append((name, index, unique))
+            fields_indexes.append((name, index, unique))
 
-    if fields_:
-        changes.append(change_fields(model1, *fields_, **kwargs))
+    if fields_to_change:
+        changes.append(change_fields(model1, *fields_to_change))
 
-    for name, null in nulls_:
+    for name, null in fields_nulls:
         changes.append(change_not_null(model1, name, null=null))
 
-    for name, index, unique in indexes_:
+    for name, index, unique in fields_indexes:
         if (index is True) or (unique is True):
             if field_names2[name].unique or field_names2[name].index:
                 changes.append(drop_index(model1, name))
             changes.append(add_index(model1, name, unique=unique))
         else:
             changes.append(drop_index(model1, name))
 
@@ -233,18 +242,18 @@
     # Remove models
     for name in [m for m in models_map2 if m not in models_map1]:
         changes.append(remove_model(models_map2[name]))
 
     return changes
 
 
-def model_to_code(model_cls: TModelType, **kwargs) -> str:
+def model_to_code(model_type: TModelType, **kwargs) -> str:
     """Generate migrations for the given model."""
     template = "class {classname}(pw.Model):\n{fields}\n\n{meta}"
-    meta = model_cls._meta  # type: ignore[]
+    meta = model_type._meta  # type: ignore[]
     fields = INDENT + NEWLINE.join(
         [
             field_to_code(field, **kwargs)
             for field in meta.sorted_fields
             if not (isinstance(field, pw.PrimaryKeyField) and field.name == "id")
         ]
     )
@@ -261,42 +270,42 @@
                     else ""
                 ),
                 f"{INDENT}indexes = {meta.indexes!r}" if meta.indexes else "",
             ],
         )
     )
 
-    return template.format(classname=model_cls.__name__, fields=fields, meta=meta)
+    return template.format(classname=model_type.__name__, fields=fields, meta=meta)
 
 
-def create_model(model_cls: TModelType, **kwargs) -> str:
+def create_model(model_type: TModelType, **kwargs) -> str:
     """Generate migrations to create model."""
-    return "@migrator.create_model\n" + model_to_code(model_cls, **kwargs)
+    return "@migrator.create_model\n" + model_to_code(model_type, **kwargs)
 
 
-def remove_model(model_cls: TModelType, **kwargs) -> str:
+def remove_model(model_type: TModelType, **kwargs) -> str:
     """Generate migrations to remove model."""
-    meta = model_cls._meta  # type: ignore[]
+    meta = model_type._meta  # type: ignore[]
     return "migrator.remove_model('%s')" % meta.table_name
 
 
-def create_fields(model_cls: TModelType, *fields: pw.Field, **kwargs) -> str:
+def create_fields(model_type: TModelType, *fields: pw.Field, **kwargs) -> str:
     """Generate migrations to add fields."""
-    meta = model_cls._meta  # type: ignore[]
+    meta = model_type._meta  # type: ignore[]
     return "migrator.add_fields(%s'%s', %s)" % (
         NEWLINE,
         meta.table_name,
         NEWLINE
         + ("," + NEWLINE).join([field_to_code(field, space=False, **kwargs) for field in fields]),
     )
 
 
-def drop_fields(model_cls: TModelType, *fields: pw.Field, **kwargs) -> str:
+def drop_fields(model_type: TModelType, *fields: pw.Field, **kwargs) -> str:
     """Generate migrations to remove fields."""
-    meta = model_cls._meta  # type: ignore[]
+    meta = model_type._meta  # type: ignore[]
     return "migrator.remove_fields('%s', %s)" % (
         meta.table_name,
         ", ".join(map(repr, fields)),
     )
 
 
 def field_to_code(field: pw.Field, *, space: bool = True, **kwargs) -> str:
@@ -305,51 +314,53 @@
     return col.get_field(" " if space else "")
 
 
 def compare_fields(field1: pw.Field, field2: pw.Field) -> Dict:
     """Find diffs between the given fields."""
     ftype1, ftype2 = find_field_type(field1), find_field_type(field2)
     if ftype1 != ftype2:
-        return {"cls": True}
+        return {"type": True}
 
-    col1, col2 = Column(
-        field1, extra_parameters={"index": field1.index, "unique": field1.unique}
-    ), Column(field2, extra_parameters={"index": field2.index, "unique": field2.unique})
-    params1, params2 = col1.get_field_parameters(indexes=True), col2.get_field_parameters(
-        indexes=True
+    col1, col2 = (
+        Column(field1, extra_parameters={"index": field1.index, "unique": field1.unique}),
+        Column(field2, extra_parameters={"index": field2.index, "unique": field2.unique}),
+    )
+    params1, params2 = (
+        col1.get_field_parameters(indexes=True, constraints=False),
+        col2.get_field_parameters(indexes=True, constraints=False),
     )
     return dict(set(params1.items()) - set(params2.items()))
 
 
-def change_fields(model_cls: TModelType, *fields: pw.Field, **kwargs) -> str:
+def change_fields(model_cls: TModelType, *fields: pw.Tuple[pw.Field, Dict]) -> str:
     """Generate migrations to change fields."""
     meta = model_cls._meta  # type: ignore[]
     return "migrator.change_fields('%s', %s)" % (
         meta.table_name,
-        ("," + NEWLINE).join([field_to_code(f, space=False) for f in fields]),
+        ("," + NEWLINE).join([field_to_code(f, space=False) for f, diff in fields]),
     )
 
 
-def change_not_null(model_cls: TModelType, name: str, *, null: bool) -> str:
+def change_not_null(model_type: TModelType, name: str, *, null: bool) -> str:
     """Generate migrations."""
-    meta = model_cls._meta  # type: ignore[]
+    meta = model_type._meta  # type: ignore[]
     operation = "drop_not_null" if null else "add_not_null"
     return "migrator.%s('%s', %s)" % (operation, meta.table_name, repr(name))
 
 
-def add_index(model_cls: TModelType, name: Union[str, Iterable[str]], *, unique: bool) -> str:
+def add_index(model_type: TModelType, name: Union[str, Iterable[str]], *, unique: bool) -> str:
     """Generate migrations."""
-    meta = model_cls._meta  # type: ignore[]
+    meta = model_type._meta  # type: ignore[]
     columns = repr(name).strip("()[]")
     return f"migrator.add_index('{meta.table_name}', {columns}, unique={unique})"
 
 
-def drop_index(model_cls: TModelType, name: Union[str, Iterable[str]]) -> str:
+def drop_index(model_type: TModelType, name: Union[str, Iterable[str]]) -> str:
     """Generate migrations."""
-    meta = model_cls._meta  # type: ignore[]
+    meta = model_type._meta  # type: ignore[]
     columns = repr(name).strip("()[]")
     return f"migrator.drop_index('{meta.table_name}', {columns})"
 
 
 def find_field_type(field: pw.Field) -> Type[pw.Field]:
     ftype = type(field)
     if ftype.__module__ not in PW_MODULES:
```

### Comparing `peewee_migrate-1.7.2/peewee_migrate/cli.py` & `peewee_migrate-1.7.3/peewee_migrate/cli.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.2/peewee_migrate/migrator.py` & `peewee_migrate-1.7.3/peewee_migrate/migrator.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.2/peewee_migrate/router.py` & `peewee_migrate-1.7.3/peewee_migrate/router.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.2/peewee_migrate/template.py` & `peewee_migrate-1.7.3/peewee_migrate/template.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.2/pyproject.toml` & `peewee_migrate-1.7.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-migrate"
-version = "1.7.2"
+version = "1.7.3"
 homepage = "https://github.com/klen/peewee_migrate"
 repository = "https://github.com/klen/peewee_migrate"
 description = "Support for migrations in Peewee ORM"
 readme = "README.rst"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["peewee", "migrations", "orm"]
```

### Comparing `peewee_migrate-1.7.2/PKG-INFO` & `peewee_migrate-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-migrate
-Version: 1.7.2
+Version: 1.7.3
 Summary: Support for migrations in Peewee ORM
 Home-page: https://github.com/klen/peewee_migrate
 License: MIT
 Keywords: peewee,migrations,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

