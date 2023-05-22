# Comparing `tmp/oarepo-model-builder-relations-1.0.4.tar.gz` & `tmp/oarepo-model-builder-relations-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-relations-1.0.4.tar", last modified: Fri Mar 10 08:39:01 2023, max compression
+gzip compressed data, was "oarepo-model-builder-relations-4.0.0.tar", last modified: Mon May 22 10:09:41 2023, max compression
```

## Comparing `oarepo-model-builder-relations-1.0.4.tar` & `oarepo-model-builder-relations-4.0.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:39:01.866644 oarepo-model-builder-relations-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-10 08:36:25.000000 oarepo-model-builder-relations-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-10 08:39:01.866644 oarepo-model-builder-relations-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-03-10 08:36:25.000000 oarepo-model-builder-relations-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:39:01.866644 oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-10 08:36:25.000000 oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-10 08:36:25.000000 oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations/builders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-03-10 08:36:25.000000 oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:39:01.866644 oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations/templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-10 08:36:25.000000 oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-10 08:36:25.000000 oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations/templates/record.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 08:39:01.866644 oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-10 08:39:01.000000 oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-10 08:39:01.000000 oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 08:39:01.000000 oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-10 08:39:01.000000 oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 08:37:20.000000 oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-10 08:39:01.000000 oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-10 08:39:01.000000 oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-10 08:36:25.000000 oarepo-model-builder-relations-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-10 08:39:01.866644 oarepo-model-builder-relations-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-10 08:36:25.000000 oarepo-model-builder-relations-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:09:41.235659 oarepo-model-builder-relations-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-22 10:09:41.235659 oarepo-model-builder-relations-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:09:41.235659 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10653 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:09:41.235659 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations/templates/record.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:09:41.235659 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-22 10:09:41.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-22 10:09:41.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:09:41.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-22 10:09:41.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:06:04.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-22 10:09:41.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 10:09:41.000000 oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-22 10:09:41.239659 oarepo-model-builder-relations-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-22 10:05:14.000000 oarepo-model-builder-relations-4.0.0/setup.py
```

### Comparing `oarepo-model-builder-relations-1.0.4/PKG-INFO` & `oarepo-model-builder-relations-4.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-relations
-Version: 1.0.4
+Version: 4.0.0
 Summary: "A model builder plugin to reference relations"
 Home-page: https://github.com/oarepo/oarepo-model-builder-relations
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio relations model builder
 Platform: any
```

### Comparing `oarepo-model-builder-relations-1.0.4/README.md` & `oarepo-model-builder-relations-4.0.0/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations.egg-info/PKG-INFO` & `oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-relations
-Version: 1.0.4
+Version: 4.0.0
 Summary: "A model builder plugin to reference relations"
 Home-page: https://github.com/oarepo/oarepo-model-builder-relations
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio relations model builder
 Platform: any
```

### Comparing `oarepo-model-builder-relations-1.0.4/oarepo_model_builder_relations.egg-info/SOURCES.txt` & `oarepo-model-builder-relations-4.0.0/oarepo_model_builder_relations.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 oarepo_model_builder_relations/__init__.py
 oarepo_model_builder_relations/builders.py
+oarepo_model_builder_relations/components.py
 oarepo_model_builder_relations/datatypes.py
 oarepo_model_builder_relations.egg-info/PKG-INFO
 oarepo_model_builder_relations.egg-info/SOURCES.txt
 oarepo_model_builder_relations.egg-info/dependency_links.txt
 oarepo_model_builder_relations.egg-info/entry_points.txt
 oarepo_model_builder_relations.egg-info/not-zip-safe
 oarepo_model_builder_relations.egg-info/requires.txt
```

### Comparing `oarepo-model-builder-relations-1.0.4/setup.cfg` & `oarepo-model-builder-relations-4.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-relations
-version = 1.0.4
+version = 4.0.0
 description = "A model builder plugin to reference relations"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio relations model builder
 license = MIT
 author = Miroslav Simek
 author_email = simek.miroslav@techlib.cz
@@ -14,35 +14,36 @@
 	Development Status :: 3 - Alpha
 
 [options]
 packages = find:
 python_requires = >=3.9
 zip_safe = False
 install_requires = 
-	oarepo-model-builder>=3.2.16
+	oarepo-model-builder>=4.0.0
+	oarepo-model-builder-cf>=4.0.0
 
 [options.package_data]
 * = *.yaml, *.json, *.json5, *.jinja2
 
 [options.extras_require]
 tests = 
 	pytest
 	black
 	autoflake
 	isort
 
 [options.entry_points]
 oarepo_model_builder.datatypes = 
 	relations = oarepo_model_builder_relations.datatypes:DATATYPES
+oarepo_model_builder.datatypes.components = 
+	relations = oarepo_model_builder_relations.components:COMPONENTS
 oarepo_model_builder.templates = 
 	99-relations-templates  = oarepo_model_builder_relations
-oarepo_model_builder.builders.model = 
+oarepo_model_builder.builders.record = 
 	1000-relation-field = oarepo_model_builder_relations.builders:InvenioRecordRelationsBuilder
-oarepo_model_builder.validation = 
-	relations = oarepo_model_builder_relations.datatypes:VALIDATORS
 
 [build_sphinx]
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
 
 [bdist_wheel]
```

