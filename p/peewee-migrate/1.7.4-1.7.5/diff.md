# Comparing `tmp/peewee_migrate-1.7.4.tar.gz` & `tmp/peewee_migrate-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_migrate-1.7.4.tar", max compression
+gzip compressed data, was "peewee_migrate-1.7.5.tar", max compression
```

## Comparing `peewee_migrate-1.7.4.tar` & `peewee_migrate-1.7.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4456 2023-05-22 19:59:21.792277 peewee_migrate-1.7.4/README.rst
--rw-r--r--   0        0        0      146 2023-05-22 19:59:21.792277 peewee_migrate-1.7.4/peewee_migrate/__init__.py
--rw-r--r--   0        0        0       78 2023-05-22 19:59:21.792277 peewee_migrate-1.7.4/peewee_migrate/__main__.py
--rw-r--r--   0        0        0    12134 2023-05-22 19:59:21.792277 peewee_migrate-1.7.4/peewee_migrate/auto.py
--rw-r--r--   0        0        0     6597 2023-05-22 19:59:21.792277 peewee_migrate-1.7.4/peewee_migrate/cli.py
--rw-r--r--   0        0        0      146 2023-05-22 19:59:21.792277 peewee_migrate-1.7.4/peewee_migrate/logs.py
--rw-r--r--   0        0        0    16505 2023-05-22 19:59:21.792277 peewee_migrate-1.7.4/peewee_migrate/migrator.py
--rw-r--r--   0        0        0      465 2023-05-22 19:59:21.792277 peewee_migrate-1.7.4/peewee_migrate/models.py
--rw-r--r--   0        0        0        0 2023-05-22 19:59:21.792277 peewee_migrate-1.7.4/peewee_migrate/py.typed
--rw-r--r--   0        0        0    12235 2023-05-22 19:59:21.792277 peewee_migrate-1.7.4/peewee_migrate/router.py
--rw-r--r--   0        0        0     1723 2023-05-22 19:59:21.792277 peewee_migrate-1.7.4/peewee_migrate/template.py
--rw-r--r--   0        0        0      249 2023-05-22 19:59:21.792277 peewee_migrate-1.7.4/peewee_migrate/types.py
--rw-r--r--   0        0        0     1589 2023-05-22 19:59:21.792277 peewee_migrate-1.7.4/pyproject.toml
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.7.4/PKG-INFO
+-rw-r--r--   0        0        0     4456 2023-05-22 20:19:55.220634 peewee_migrate-1.7.5/README.rst
+-rw-r--r--   0        0        0      146 2023-05-22 20:19:55.220634 peewee_migrate-1.7.5/peewee_migrate/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-22 20:19:55.220634 peewee_migrate-1.7.5/peewee_migrate/__main__.py
+-rw-r--r--   0        0        0    12214 2023-05-22 20:19:55.220634 peewee_migrate-1.7.5/peewee_migrate/auto.py
+-rw-r--r--   0        0        0     6597 2023-05-22 20:19:55.220634 peewee_migrate-1.7.5/peewee_migrate/cli.py
+-rw-r--r--   0        0        0      146 2023-05-22 20:19:55.220634 peewee_migrate-1.7.5/peewee_migrate/logs.py
+-rw-r--r--   0        0        0    16505 2023-05-22 20:19:55.220634 peewee_migrate-1.7.5/peewee_migrate/migrator.py
+-rw-r--r--   0        0        0      461 2023-05-22 20:19:55.220634 peewee_migrate-1.7.5/peewee_migrate/models.py
+-rw-r--r--   0        0        0        0 2023-05-22 20:19:55.220634 peewee_migrate-1.7.5/peewee_migrate/py.typed
+-rw-r--r--   0        0        0    12235 2023-05-22 20:19:55.220634 peewee_migrate-1.7.5/peewee_migrate/router.py
+-rw-r--r--   0        0        0     1723 2023-05-22 20:19:55.220634 peewee_migrate-1.7.5/peewee_migrate/template.py
+-rw-r--r--   0        0        0      249 2023-05-22 20:19:55.220634 peewee_migrate-1.7.5/peewee_migrate/types.py
+-rw-r--r--   0        0        0     1589 2023-05-22 20:19:55.220634 peewee_migrate-1.7.5/pyproject.toml
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.7.5/PKG-INFO
```

### Comparing `peewee_migrate-1.7.4/README.rst` & `peewee_migrate-1.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.4/peewee_migrate/auto.py` & `peewee_migrate-1.7.5/peewee_migrate/auto.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,25 +117,27 @@
         field = super(Column, self).get_field()
         module = FIELD_MODULES_MAP.get(self.field_class.__name__, "pw")
         name, _, field = [s and s.strip() for s in field.partition("=")]
         return "{name}{space}={space}{module}.{field}".format(
             name=name, field=field, space=space, module=module
         )
 
-    def get_field_parameters(self, *, indexes=False) -> TParams:
+    def get_field_parameters(self, *, change=False) -> TParams:
         """Generate parameters for self field."""
         params = super(Column, self).get_field_parameters()
         if self.default is not None:
             params["default"] = self.default
             params.pop("constraints", None)
 
         params.pop("backref", None)
-        if indexes:
+        if change:
             params["unique"] = bool(params.pop("unique", False))
             params["index"] = bool(params.pop("index", False)) or params["unique"]
+            params.pop("on_delete", None)
+            params.pop("on_update", None)
 
         return params
 
 
 def diff_one(model1: TModelType, model2: TModelType, **kwargs) -> List[str]:  # noqa:
     """Find difference between given peewee models."""
     changes = []
@@ -319,16 +321,16 @@
         return {"type": True}
 
     col1, col2 = (
         Column(field1, extra_parameters={"index": field1.index, "unique": field1.unique}),
         Column(field2, extra_parameters={"index": field2.index, "unique": field2.unique}),
     )
     params1, params2 = (
-        col1.get_field_parameters(indexes=True),
-        col2.get_field_parameters(indexes=True),
+        col1.get_field_parameters(change=True),
+        col2.get_field_parameters(change=True),
     )
     return dict(set(params1.items()) - set(params2.items()))
 
 
 def change_fields(model_cls: TModelType, *fields: pw.Tuple[pw.Field, Dict]) -> str:
     """Generate migrations to change fields."""
     meta = model_cls._meta  # type: ignore[]
```

### Comparing `peewee_migrate-1.7.4/peewee_migrate/cli.py` & `peewee_migrate-1.7.5/peewee_migrate/cli.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.4/peewee_migrate/migrator.py` & `peewee_migrate-1.7.5/peewee_migrate/migrator.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.4/peewee_migrate/router.py` & `peewee_migrate-1.7.5/peewee_migrate/router.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.4/peewee_migrate/template.py` & `peewee_migrate-1.7.5/peewee_migrate/template.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.4/pyproject.toml` & `peewee_migrate-1.7.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-migrate"
-version = "1.7.4"
+version = "1.7.5"
 homepage = "https://github.com/klen/peewee_migrate"
 repository = "https://github.com/klen/peewee_migrate"
 description = "Support for migrations in Peewee ORM"
 readme = "README.rst"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["peewee", "migrations", "orm"]
```

### Comparing `peewee_migrate-1.7.4/PKG-INFO` & `peewee_migrate-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-migrate
-Version: 1.7.4
+Version: 1.7.5
 Summary: Support for migrations in Peewee ORM
 Home-page: https://github.com/klen/peewee_migrate
 License: MIT
 Keywords: peewee,migrations,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```

