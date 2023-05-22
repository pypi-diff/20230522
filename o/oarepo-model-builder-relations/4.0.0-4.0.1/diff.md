# Comparing `tmp/oarepo-model-builder-relations-4.0.0.tar.gz` & `tmp/oarepo-model-builder-relations-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-relations-4.0.0.tar", last modified: Mon May 22 10:09:41 2023, max compression
+gzip compressed data, was "oarepo-model-builder-relations-4.0.1.tar", last modified: Mon May 22 13:15:16 2023, max compression
```

## Comparing `oarepo-model-builder-relations-4.0.0.tar` & `oarepo-model-builder-relations-4.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:09:41.235659 oarepo-model-builder-relations-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-22 10:09:41.235659 oarepo-model-builder-relations-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:09:41.235659 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:09:41.235659 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/templates/record.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:09:41.235659 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-22 10:09:41.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-22 10:09:41.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:09:41.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-22 10:09:41.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:06:04.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-22 10:09:41.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 10:09:41.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-22 10:09:41.239659 oarepo-model-builder-relations-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:15:16.484234 oarepo-model-builder-relations-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 13:11:19.000000 oarepo-model-builder-relations-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-22 13:15:16.484234 oarepo-model-builder-relations-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-22 13:11:19.000000 oarepo-model-builder-relations-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:15:16.480234 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-22 13:11:19.000000 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-22 13:11:19.000000 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10662 2023-05-22 13:11:19.000000 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-22 13:11:19.000000 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:15:16.484234 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:11:19.000000 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-22 13:11:19.000000 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations/templates/record.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:15:16.484234 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-22 13:15:16.000000 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-22 13:15:16.000000 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:15:16.000000 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-22 13:15:16.000000 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:12:11.000000 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-22 13:15:16.000000 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 13:15:16.000000 oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 13:11:19.000000 oarepo-model-builder-relations-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-22 13:15:16.484234 oarepo-model-builder-relations-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-22 13:11:19.000000 oarepo-model-builder-relations-4.0.1/setup.py
```

### Comparing `oarepo-model-builder-relations-4.0.0/PKG-INFO` & `oarepo-model-builder-relations-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-relations
-Version: 4.0.0
+Version: 4.0.1
 Summary: "A model builder plugin to reference relations"
 Home-page: https://github.com/oarepo/oarepo-model-builder-relations
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio relations model builder
 Platform: any
```

### Comparing `oarepo-model-builder-relations-4.0.0/README.md` & `oarepo-model-builder-relations-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/builders.py` & `oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations/builders.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/components.py` & `oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     eligible_datatypes = [RelationDataType]
 
     def resolve_relation(self, datatype: RelationDataType, *, context, **kwargs):
         if datatype.internal_link:
             root_datatype = datatype.stack[0]
             dt_id = datatype.model_name[1:]
         else:
-            loaded_schema = datatype.schema._load("referred")
+            loaded_schema = datatype.schema._load(datatype.model_name)
             root_datatype = datatypes.get_datatype(
                 datatype, loaded_schema["model"], None, datatype.model, datatype.schema
             )
             root_datatype.prepare(
                 {
                     "profile": context["profile"],
                     "profile_module": context["profile_module"],
```

### Comparing `oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/datatypes.py` & `oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations/datatypes.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/PKG-INFO` & `oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-relations
-Version: 4.0.0
+Version: 4.0.1
 Summary: "A model builder plugin to reference relations"
 Home-page: https://github.com/oarepo/oarepo-model-builder-relations
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio relations model builder
 Platform: any
```

### Comparing `oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/SOURCES.txt` & `oarepo-model-builder-relations-4.0.1/oarepo_model_builder_relations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-relations-4.0.0/setup.cfg` & `oarepo-model-builder-relations-4.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-relations
-version = 4.0.0
+version = 4.0.1
 description = "A model builder plugin to reference relations"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio relations model builder
 license = MIT
 author = Miroslav Simek
 author_email = simek.miroslav@techlib.cz
```

