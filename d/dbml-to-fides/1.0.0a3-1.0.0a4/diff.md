# Comparing `tmp/dbml-to-fides-1.0.0a3.tar.gz` & `tmp/dbml-to-fides-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbml-to-fides-1.0.0a3.tar", last modified: Mon May 22 19:36:12 2023, max compression
+gzip compressed data, was "dbml-to-fides-1.0.0a4.tar", last modified: Mon May 22 19:44:28 2023, max compression
```

## Comparing `dbml-to-fides-1.0.0a3.tar` & `dbml-to-fides-1.0.0a4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:36:12.519281 dbml-to-fides-1.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-22 19:36:03.000000 dbml-to-fides-1.0.0a3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-05-22 19:36:12.519281 dbml-to-fides-1.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-05-22 19:36:03.000000 dbml-to-fides-1.0.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:36:12.519281 dbml-to-fides-1.0.0a3/dbml_to_fides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:36:03.000000 dbml-to-fides-1.0.0a3/dbml_to_fides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-22 19:36:03.000000 dbml-to-fides-1.0.0a3/dbml_to_fides/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-22 19:36:03.000000 dbml-to-fides-1.0.0a3/dbml_to_fides/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:36:12.519281 dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-05-22 19:36:12.000000 dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-22 19:36:12.000000 dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:36:12.000000 dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 19:36:12.000000 dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 19:36:12.000000 dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 19:36:12.000000 dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-22 19:36:03.000000 dbml-to-fides-1.0.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 19:36:12.519281 dbml-to-fides-1.0.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:36:12.519281 dbml-to-fides-1.0.0a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-22 19:36:03.000000 dbml-to-fides-1.0.0a3/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:28.368521 dbml-to-fides-1.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-22 19:44:19.000000 dbml-to-fides-1.0.0a4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-05-22 19:44:28.364520 dbml-to-fides-1.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-22 19:44:19.000000 dbml-to-fides-1.0.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:28.364520 dbml-to-fides-1.0.0a4/dbml_to_fides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:19.000000 dbml-to-fides-1.0.0a4/dbml_to_fides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-22 19:44:19.000000 dbml-to-fides-1.0.0a4/dbml_to_fides/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-22 19:44:19.000000 dbml-to-fides-1.0.0a4/dbml_to_fides/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:28.364520 dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-05-22 19:44:28.000000 dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-22 19:44:28.000000 dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 19:44:28.000000 dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 19:44:28.000000 dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 19:44:28.000000 dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 19:44:28.000000 dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-22 19:44:19.000000 dbml-to-fides-1.0.0a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 19:44:28.368521 dbml-to-fides-1.0.0a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 19:44:28.364520 dbml-to-fides-1.0.0a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-22 19:44:19.000000 dbml-to-fides-1.0.0a4/tests/test_transforms.py
```

### Comparing `dbml-to-fides-1.0.0a3/LICENSE.txt` & `dbml-to-fides-1.0.0a4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbml-to-fides-1.0.0a3/PKG-INFO` & `dbml-to-fides-1.0.0a4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbml-to-fides
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Interoperatbility for DBML and Fides dataset manifests
 Author-email: Ee Durbin <ee.opensource@pyfound.org>
 License: Copyright 2023 Ee Durbin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -71,40 +71,39 @@
 
 `dbml-to-fides` will output what it can infer from the DBML file as a Fides
 dataset:
 
 ```sh
 $ dbml-to-fides sample.dbml
 dataset:
-- dataset:
-  - name: public
-    collections:
-    - name: users
-      fields:
-      - name: id
-        fides_meta:
-          primary_key: true
-      - name: username
-      - name: role
-      - name: created_at
-    - name: posts
-      fields:
-      - name: id
-        fides_meta:
-          primary_key: true
-      - name: title
-      - name: body
-      - name: user_id
-        fides_meta:
-          references:
-          - dataset: public
-            field: users.id
-            direction: to
-      - name: status
-      - name: created_at
+- name: public
+  collections:
+  - name: users
+    fields:
+    - name: id
+      fides_meta:
+        primary_key: true
+    - name: username
+    - name: role
+    - name: created_at
+  - name: posts
+    fields:
+    - name: id
+      fides_meta:
+        primary_key: true
+    - name: title
+    - name: body
+    - name: user_id
+      fides_meta:
+        references:
+        - dataset: public
+          field: users.id
+          direction: to
+    - name: status
+    - name: created_at
 
 ```
 
 If you have an existing Fides dataset in `.fides/sample_dataset.yml`:
 
 ```yaml
 dataset:
@@ -208,25 +207,38 @@
  Table posts {
 ```
 
 Then running our diff again will add the field to our Fides dataset:
 
 ```shell
 $ diff -u .fides/sample_dataset.yml <(dbml-to-fides sample.dbml --base-dataset .fides/sample_dataset.yml)
---- .fides/sample_dataset.yml	2023-05-22 11:30:41
-+++ /dev/fd/63	2023-05-22 11:35:13
+--- .fides/sample_dataset.yml	2023-05-22 15:39:24
++++ /dev/fd/63	2023-05-22 15:40:07
 @@ -34,6 +34,7 @@
        data_categories:
        - system.operations
        data_qualifier: aggregated.anonymized.unlinked_pseudonymized.pseudonymized.identified
 +    - name: social_security_number
    - name: posts
      description: Post information
      fields:
 ```
 
 If we wanted to write the output to a file,
 we would add the `--output-file` flag:
 
 ```shell
-$ dbml-to-fides sample.dbml --base-dataset .fides/sample_dataset.yml
+$ dbml-to-fides sample.dbml --base-dataset .fides/sample_dataset.yml --output-file .fides/sample_dataset.yml
+$ git diff
+diff --git a/.fides/sample_dataset.yml b/.fides/sample_dataset.yml
+index 594cee4..edc3141 100644
+--- a/.fides/sample_dataset.yml
++++ b/.fides/sample_dataset.yml
+@@ -34,6 +34,7 @@ dataset:
+       data_categories:
+       - system.operations
+       data_qualifier: aggregated.anonymized.unlinked_pseudonymized.pseudonymized.identified
++    - name: social_security_number
+   - name: posts
+     description: Post information
+     fields:
 ```
```

### Comparing `dbml-to-fides-1.0.0a3/README.md` & `dbml-to-fides-1.0.0a4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -41,40 +41,39 @@
 
 `dbml-to-fides` will output what it can infer from the DBML file as a Fides
 dataset:
 
 ```sh
 $ dbml-to-fides sample.dbml
 dataset:
-- dataset:
-  - name: public
-    collections:
-    - name: users
-      fields:
-      - name: id
-        fides_meta:
-          primary_key: true
-      - name: username
-      - name: role
-      - name: created_at
-    - name: posts
-      fields:
-      - name: id
-        fides_meta:
-          primary_key: true
-      - name: title
-      - name: body
-      - name: user_id
-        fides_meta:
-          references:
-          - dataset: public
-            field: users.id
-            direction: to
-      - name: status
-      - name: created_at
+- name: public
+  collections:
+  - name: users
+    fields:
+    - name: id
+      fides_meta:
+        primary_key: true
+    - name: username
+    - name: role
+    - name: created_at
+  - name: posts
+    fields:
+    - name: id
+      fides_meta:
+        primary_key: true
+    - name: title
+    - name: body
+    - name: user_id
+      fides_meta:
+        references:
+        - dataset: public
+          field: users.id
+          direction: to
+    - name: status
+    - name: created_at
 
 ```
 
 If you have an existing Fides dataset in `.fides/sample_dataset.yml`:
 
 ```yaml
 dataset:
@@ -178,25 +177,38 @@
  Table posts {
 ```
 
 Then running our diff again will add the field to our Fides dataset:
 
 ```shell
 $ diff -u .fides/sample_dataset.yml <(dbml-to-fides sample.dbml --base-dataset .fides/sample_dataset.yml)
---- .fides/sample_dataset.yml	2023-05-22 11:30:41
-+++ /dev/fd/63	2023-05-22 11:35:13
+--- .fides/sample_dataset.yml	2023-05-22 15:39:24
++++ /dev/fd/63	2023-05-22 15:40:07
 @@ -34,6 +34,7 @@
        data_categories:
        - system.operations
        data_qualifier: aggregated.anonymized.unlinked_pseudonymized.pseudonymized.identified
 +    - name: social_security_number
    - name: posts
      description: Post information
      fields:
 ```
 
 If we wanted to write the output to a file,
 we would add the `--output-file` flag:
 
 ```shell
-$ dbml-to-fides sample.dbml --base-dataset .fides/sample_dataset.yml
+$ dbml-to-fides sample.dbml --base-dataset .fides/sample_dataset.yml --output-file .fides/sample_dataset.yml
+$ git diff
+diff --git a/.fides/sample_dataset.yml b/.fides/sample_dataset.yml
+index 594cee4..edc3141 100644
+--- a/.fides/sample_dataset.yml
++++ b/.fides/sample_dataset.yml
+@@ -34,6 +34,7 @@ dataset:
+       data_categories:
+       - system.operations
+       data_qualifier: aggregated.anonymized.unlinked_pseudonymized.pseudonymized.identified
++    - name: social_security_number
+   - name: posts
+     description: Post information
+     fields:
 ```
```

### Comparing `dbml-to-fides-1.0.0a3/dbml_to_fides/cli.py` & `dbml-to-fides-1.0.0a4/dbml_to_fides/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,17 +23,15 @@
     if base_dataset is not None:
         _base_dataset_dict = ingest_manifests(base_dataset)
         _fides_dataset_dict = merge_fides_dataset_dicts(
             _base_dataset_dict, _fides_dataset_dict
         )
 
     if output_file is None:
-        with tempfile.NamedTemporaryFile() as f:
-            yaml.dump(_fides_dataset_dict, f, sort_keys=False, indent=2)
-            click.echo(f.read())
+        click.echo(yaml.dump(_fides_dataset_dict,sort_keys=False, indent=2), nl=False)
     else:
         with open(output_file, "w") as f:
             yaml.dump(_fides_dataset_dict, f, sort_keys=False, indent=2)
 
 
 if __name__ == "__main__":
     transform_and_merge()
```

### Comparing `dbml-to-fides-1.0.0a3/dbml_to_fides/transform.py` & `dbml-to-fides-1.0.0a4/dbml_to_fides/transform.py`

 * *Files identical despite different names*

### Comparing `dbml-to-fides-1.0.0a3/dbml_to_fides.egg-info/PKG-INFO` & `dbml-to-fides-1.0.0a4/dbml_to_fides.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbml-to-fides
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Interoperatbility for DBML and Fides dataset manifests
 Author-email: Ee Durbin <ee.opensource@pyfound.org>
 License: Copyright 2023 Ee Durbin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -71,40 +71,39 @@
 
 `dbml-to-fides` will output what it can infer from the DBML file as a Fides
 dataset:
 
 ```sh
 $ dbml-to-fides sample.dbml
 dataset:
-- dataset:
-  - name: public
-    collections:
-    - name: users
-      fields:
-      - name: id
-        fides_meta:
-          primary_key: true
-      - name: username
-      - name: role
-      - name: created_at
-    - name: posts
-      fields:
-      - name: id
-        fides_meta:
-          primary_key: true
-      - name: title
-      - name: body
-      - name: user_id
-        fides_meta:
-          references:
-          - dataset: public
-            field: users.id
-            direction: to
-      - name: status
-      - name: created_at
+- name: public
+  collections:
+  - name: users
+    fields:
+    - name: id
+      fides_meta:
+        primary_key: true
+    - name: username
+    - name: role
+    - name: created_at
+  - name: posts
+    fields:
+    - name: id
+      fides_meta:
+        primary_key: true
+    - name: title
+    - name: body
+    - name: user_id
+      fides_meta:
+        references:
+        - dataset: public
+          field: users.id
+          direction: to
+    - name: status
+    - name: created_at
 
 ```
 
 If you have an existing Fides dataset in `.fides/sample_dataset.yml`:
 
 ```yaml
 dataset:
@@ -208,25 +207,38 @@
  Table posts {
 ```
 
 Then running our diff again will add the field to our Fides dataset:
 
 ```shell
 $ diff -u .fides/sample_dataset.yml <(dbml-to-fides sample.dbml --base-dataset .fides/sample_dataset.yml)
---- .fides/sample_dataset.yml	2023-05-22 11:30:41
-+++ /dev/fd/63	2023-05-22 11:35:13
+--- .fides/sample_dataset.yml	2023-05-22 15:39:24
++++ /dev/fd/63	2023-05-22 15:40:07
 @@ -34,6 +34,7 @@
        data_categories:
        - system.operations
        data_qualifier: aggregated.anonymized.unlinked_pseudonymized.pseudonymized.identified
 +    - name: social_security_number
    - name: posts
      description: Post information
      fields:
 ```
 
 If we wanted to write the output to a file,
 we would add the `--output-file` flag:
 
 ```shell
-$ dbml-to-fides sample.dbml --base-dataset .fides/sample_dataset.yml
+$ dbml-to-fides sample.dbml --base-dataset .fides/sample_dataset.yml --output-file .fides/sample_dataset.yml
+$ git diff
+diff --git a/.fides/sample_dataset.yml b/.fides/sample_dataset.yml
+index 594cee4..edc3141 100644
+--- a/.fides/sample_dataset.yml
++++ b/.fides/sample_dataset.yml
+@@ -34,6 +34,7 @@ dataset:
+       data_categories:
+       - system.operations
+       data_qualifier: aggregated.anonymized.unlinked_pseudonymized.pseudonymized.identified
++    - name: social_security_number
+   - name: posts
+     description: Post information
+     fields:
 ```
```

### Comparing `dbml-to-fides-1.0.0a3/pyproject.toml` & `dbml-to-fides-1.0.0a4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbml-to-fides"
-version = "1.0.0a3"
+version = "1.0.0a4"
 description = "Interoperatbility for DBML and Fides dataset manifests"
 
 readme = "README.md"
 requires-python = ">=3.8, <4"
 license = {file = "LICENSE.txt"}
 
 keywords = ["fides", "dbml"]
```

### Comparing `dbml-to-fides-1.0.0a3/tests/test_transforms.py` & `dbml-to-fides-1.0.0a4/tests/test_transforms.py`

 * *Files identical despite different names*

