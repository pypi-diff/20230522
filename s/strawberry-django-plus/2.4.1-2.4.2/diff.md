# Comparing `tmp/strawberry_django_plus-2.4.1.tar.gz` & `tmp/strawberry_django_plus-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-2.4.1.tar", max compression
+gzip compressed data, was "strawberry_django_plus-2.4.2.tar", max compression
```

## Comparing `strawberry_django_plus-2.4.1.tar` & `strawberry_django_plus-2.4.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1077 2023-05-19 15:14:15.513954 strawberry_django_plus-2.4.1/LICENSE
--rw-r--r--   0        0        0     3299 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/README.md
--rw-r--r--   0        0        0     4290 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/pyproject.toml
--rw-r--r--   0        0        0     2950 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5562 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5751 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    26052 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3069 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1657 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1389 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1168 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0     6304 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/middlewares/debug_toolbar.py
--rw-r--r--   0        0        0        0 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    25062 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14825 2023-05-19 15:14:15.517954 strawberry_django_plus-2.4.1/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    24443 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1372 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    27526 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0    47560 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1107 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0     1445 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
--rw-r--r--   0        0        0        0 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2337 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    18301 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/type.py
--rw-r--r--   0        0        0    10174 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6916 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    12426 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     5865 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    13142 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0      938 2023-05-19 15:14:15.521954 strawberry_django_plus-2.4.1/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 strawberry_django_plus-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-22 16:44:37.960302 strawberry_django_plus-2.4.2/LICENSE
+-rw-r--r--   0        0        0     3299 2023-05-22 16:44:37.960302 strawberry_django_plus-2.4.2/README.md
+-rw-r--r--   0        0        0     4290 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2950 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5562 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5751 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    26052 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3069 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1657 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1389 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1168 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0     6304 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/middlewares/debug_toolbar.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    25062 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14825 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    24443 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1372 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    27526 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0    47560 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1107 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0     1445 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
+-rw-r--r--   0        0        0        0 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2337 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    18301 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0    10174 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6916 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    13069 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     5865 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    13142 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0      938 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 strawberry_django_plus-2.4.2/PKG-INFO
```

### Comparing `strawberry_django_plus-2.4.1/LICENSE` & `strawberry_django_plus-2.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/README.md` & `strawberry_django_plus-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/pyproject.toml` & `strawberry_django_plus-2.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "2.4.1"
+version = "2.4.2"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
```

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/__init__.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/descriptors.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/directives.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/field.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/field.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/filters.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/filters.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/gql/django.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/gql/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/integrations/guardian.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/management/commands/export_schema.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/middlewares/debug_toolbar.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/middlewares/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/mutations/fields.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/mutations/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/optimizer.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/ordering.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/ordering.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/permissions.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/permissions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/relay.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/settings.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html` & `strawberry_django_plus-2.4.2/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/test/client.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/test/client.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/type.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/type.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/types.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/utils/aio.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/utils/inspect.py`

 * *Files 6% similar despite different names*

```diff
@@ -207,14 +207,35 @@
         All possibilities for the type
 
     """
     # Because of the way graphql spreads fragments,
     # later selections should replace previous ones
     ret: Dict[str, SelectedField] = {}
 
+    def merge_selections(f1: SelectedField, f2: SelectedField) -> SelectedField:
+        if not f1.selections:
+            return f2
+        if not f2.selections:
+            return f1
+
+        f1_selections = {s.name: s for s in cast(List[SelectedField], f1.selections)}
+        f2_selections = {s.name: s for s in cast(List[SelectedField], f2.selections)}
+
+        selections: Dict[str, SelectedField] = {}
+        for f_name in set(f1_selections) - set(f2_selections):
+            selections[f_name] = f1_selections[f_name]
+        for f_name in set(f2_selections) - set(f1_selections):
+            selections[f_name] = f2_selections[f_name]
+        for f_name in set(f2_selections) & set(f1_selections):
+            selections[f_name] = f1_selections[f_name]
+            selections[f_name] = merge_selections(f1_selections[f_name], f2_selections[f_name])
+
+        f1.selections = list(selections.values())
+        return f1
+
     for s in selection.selections:
         if isinstance(s, SelectedField):
             # @include(if: <bool>)
             include = s.directives.get("include")
             if include and not include["if"]:
                 continue
 
@@ -222,36 +243,27 @@
             skip = s.directives.get("skip")
             if skip and skip["if"]:
                 continue
 
             f_name = s.alias or s.name
             existing = ret.get(f_name)
             if existing := ret.get(f_name):
-                s.selections = list(
-                    {
-                        **get_selections(existing),
-                        **get_selections(s),
-                    }.values(),
-                )
+                ret[f_name] = merge_selections(existing, s)
             else:
                 ret[f_name] = s
         elif isinstance(s, (FragmentSpread, InlineFragment)):
             if typename is not None and s.type_condition != typename:
                 continue
 
             for f_name, f in get_selections(s, typename=typename).items():
                 existing = ret.get(f_name)
                 if existing is not None:
-                    f.selections = list(
-                        {
-                            **get_selections(existing),
-                            **get_selections(f),
-                        }.values(),
-                    )
-                ret[f_name] = f
+                    ret[f_name] = merge_selections(existing, f)
+                else:
+                    ret[f_name] = f
         else:  # pragma:nocover
             assert_never(s)
 
     return ret
 
 
 @dataclasses.dataclass(eq=True)
```

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/utils/query.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/utils/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-2.4.2/strawberry_django_plus/utils/typing.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.1/PKG-INFO` & `strawberry_django_plus-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 2.4.1
+Version: 2.4.2
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```

