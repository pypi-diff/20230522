# Comparing `tmp/dbml-to-fides-1.0.0a2.tar.gz` & `tmp/dbml-to-fides-1.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbml-to-fides-1.0.0a2.tar", last modified: Mon May 22 16:01:44 2023, max compression
+gzip compressed data, was "dbml-to-fides-1.0.0a3.tar", last modified: Mon May 22 19:36:12 2023, max compression
```

## Comparing `dbml-to-fides-1.0.0a2.tar` & `dbml-to-fides-1.0.0a3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:01:44.526357 dbml-to-fides-1.0.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-22 16:01:35.000000 dbml-to-fides-1.0.0a2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-05-22 16:01:44.526357 dbml-to-fides-1.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-05-22 16:01:35.000000 dbml-to-fides-1.0.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:01:44.526357 dbml-to-fides-1.0.0a2/dbml_to_fides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:01:35.000000 dbml-to-fides-1.0.0a2/dbml_to_fides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-22 16:01:35.000000 dbml-to-fides-1.0.0a2/dbml_to_fides/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-05-22 16:01:35.000000 dbml-to-fides-1.0.0a2/dbml_to_fides/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:01:44.526357 dbml-to-fides-1.0.0a2/dbml_to_fides.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-05-22 16:01:44.000000 dbml-to-fides-1.0.0a2/dbml_to_fides.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-22 16:01:44.000000 dbml-to-fides-1.0.0a2/dbml_to_fides.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:01:44.000000 dbml-to-fides-1.0.0a2/dbml_to_fides.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 16:01:44.000000 dbml-to-fides-1.0.0a2/dbml_to_fides.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 16:01:44.000000 dbml-to-fides-1.0.0a2/dbml_to_fides.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 16:01:44.000000 dbml-to-fides-1.0.0a2/dbml_to_fides.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-22 16:01:35.000000 dbml-to-fides-1.0.0a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:01:44.526357 dbml-to-fides-1.0.0a2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:36:12.519281 dbml-to-fides-1.0.0a3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-22 19:36:03.000000 dbml-to-fides-1.0.0a3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-05-22 19:36:12.519281 dbml-to-fides-1.0.0a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-05-22 19:36:03.000000 dbml-to-fides-1.0.0a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:36:12.519281 dbml-to-fides-1.0.0a3/dbml_to_fides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:36:03.000000 dbml-to-fides-1.0.0a3/dbml_to_fides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-22 19:36:03.000000 dbml-to-fides-1.0.0a3/dbml_to_fides/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-22 19:36:03.000000 dbml-to-fides-1.0.0a3/dbml_to_fides/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:36:12.519281 dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-05-22 19:36:12.000000 dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-22 19:36:12.000000 dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:36:12.000000 dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 19:36:12.000000 dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 19:36:12.000000 dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 19:36:12.000000 dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-22 19:36:03.000000 dbml-to-fides-1.0.0a3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 19:36:12.519281 dbml-to-fides-1.0.0a3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:36:12.519281 dbml-to-fides-1.0.0a3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-22 19:36:03.000000 dbml-to-fides-1.0.0a3/tests/test_transforms.py
```

### Comparing `dbml-to-fides-1.0.0a2/LICENSE.txt` & `dbml-to-fides-1.0.0a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbml-to-fides-1.0.0a2/PKG-INFO` & `dbml-to-fides-1.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbml-to-fides
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Interoperatbility for DBML and Fides dataset manifests
 Author-email: Ee Durbin <ee.opensource@pyfound.org>
 License: Copyright 2023 Ee Durbin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `dbml-to-fides-1.0.0a2/README.md` & `dbml-to-fides-1.0.0a3/README.md`

 * *Files identical despite different names*

### Comparing `dbml-to-fides-1.0.0a2/dbml_to_fides/cli.py` & `dbml-to-fides-1.0.0a3/dbml_to_fides/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import tempfile
 
 import click
+import yaml
 
 from pydbml import PyDBML
 from fideslang.manifests import ingest_manifests, write_manifest
 
 from dbml_to_fides.transform import (
     dbml_to_fides_dataset_dict,
     merge_fides_dataset_dicts,
@@ -23,15 +24,16 @@
         _base_dataset_dict = ingest_manifests(base_dataset)
         _fides_dataset_dict = merge_fides_dataset_dicts(
             _base_dataset_dict, _fides_dataset_dict
         )
 
     if output_file is None:
         with tempfile.NamedTemporaryFile() as f:
-            write_manifest(f.name, _fides_dataset_dict, "dataset")
+            yaml.dump(_fides_dataset_dict, f, sort_keys=False, indent=2)
             click.echo(f.read())
     else:
-        write_manifest(output_file, _fides_dataset_dict, "dataset")
+        with open(output_file, "w") as f:
+            yaml.dump(_fides_dataset_dict, f, sort_keys=False, indent=2)
 
 
 if __name__ == "__main__":
     transform_and_merge()
```

### Comparing `dbml-to-fides-1.0.0a2/dbml_to_fides/transform.py` & `dbml-to-fides-1.0.0a3/dbml_to_fides/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                     field.get("fides_meta", {}).get("references", {}).values()
                 )
                 if references:
                     field["fides_meta"]["references"] = references
             collections.append(collection)
         dataset["collections"] = collections
         relistified.append(dataset)
-    return relistified
+    return {"dataset": relistified}
 
 
 def merge_fides_dataset_dicts(existing, new):
     _existing = unlistify(existing)
     _new = unlistify(new)
 
     updated = always_merger.merge(_existing, _new)
```

### Comparing `dbml-to-fides-1.0.0a2/dbml_to_fides.egg-info/PKG-INFO` & `dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbml-to-fides
-Version: 1.0.0a2
+Version: 1.0.0a3
 Summary: Interoperatbility for DBML and Fides dataset manifests
 Author-email: Ee Durbin <ee.opensource@pyfound.org>
 License: Copyright 2023 Ee Durbin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `dbml-to-fides-1.0.0a2/pyproject.toml` & `dbml-to-fides-1.0.0a3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbml-to-fides"
-version = "1.0.0a2"
+version = "1.0.0a3"
 description = "Interoperatbility for DBML and Fides dataset manifests"
 
 readme = "README.md"
 requires-python = ">=3.8, <4"
 license = {file = "LICENSE.txt"}
 
 keywords = ["fides", "dbml"]
@@ -29,14 +29,15 @@
 ]
 
 dependencies = [ # Optional
   "click",
   "deepmerge",
   "fideslang",
   "pydbml",
+  "pyaml",
 ]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/ewdurbin/dbml-to-fides"
 "Source" = "https://github.com/ewdurbin/dbml-to-fides"
 
 [project.scripts]  # Optional
```

