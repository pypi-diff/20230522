# Comparing `tmp/dysweep-0.0.3.tar.gz` & `tmp/dysweep-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dysweep-0.0.3.tar", last modified: Mon May 22 03:44:12 2023, max compression
+gzip compressed data, was "dysweep-0.0.4.tar", last modified: Mon May 22 03:53:51 2023, max compression
```

## Comparing `dysweep-0.0.3.tar` & `dysweep-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:44:12.157792 dysweep-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 03:41:25.000000 dysweep-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-22 03:44:12.157792 dysweep-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 03:41:25.000000 dysweep-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:44:12.157792 dysweep-0.0.3/dysweep/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 03:41:25.000000 dysweep-0.0.3/dysweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-22 03:41:25.000000 dysweep-0.0.3/dysweep/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    20382 2023-05-22 03:41:25.000000 dysweep-0.0.3/dysweep/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-22 03:41:25.000000 dysweep-0.0.3/dysweep/wandbX.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:44:12.157792 dysweep-0.0.3/dysweep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-22 03:44:12.000000 dysweep-0.0.3/dysweep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-22 03:44:12.000000 dysweep-0.0.3/dysweep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 03:44:12.000000 dysweep-0.0.3/dysweep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 03:44:12.000000 dysweep-0.0.3/dysweep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 03:44:12.157792 dysweep-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-22 03:41:25.000000 dysweep-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:53:51.913491 dysweep-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 03:51:35.000000 dysweep-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-22 03:53:51.913491 dysweep-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 03:51:35.000000 dysweep-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:53:51.913491 dysweep-0.0.4/dysweep/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 03:51:35.000000 dysweep-0.0.4/dysweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-22 03:51:35.000000 dysweep-0.0.4/dysweep/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20767 2023-05-22 03:51:35.000000 dysweep-0.0.4/dysweep/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-22 03:51:35.000000 dysweep-0.0.4/dysweep/wandbX.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:53:51.913491 dysweep-0.0.4/dysweep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-22 03:53:51.000000 dysweep-0.0.4/dysweep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-22 03:53:51.000000 dysweep-0.0.4/dysweep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 03:53:51.000000 dysweep-0.0.4/dysweep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 03:53:51.000000 dysweep-0.0.4/dysweep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 03:53:51.913491 dysweep-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-22 03:51:35.000000 dysweep-0.0.4/setup.py
```

### Comparing `dysweep-0.0.3/LICENSE` & `dysweep-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.3/PKG-INFO` & `dysweep-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.0.3
+Version: 0.0.4
 Summary: A toolset for dynamic python code manipulations
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: Apache License 2.0
 Description: # DySweep: Use W&B Sweep for Everything!
```

### Comparing `dysweep-0.0.3/dysweep/parallel.py` & `dysweep-0.0.4/dysweep/parallel.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.3/dysweep/utils.py` & `dysweep-0.0.4/dysweep/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,32 +128,32 @@
     # Define a flattening method for the tree
     def flatten_tree(
         tree_dict: th.Union[dict, th.List]
     ) -> dict:
         ret = {}
         has_something_to_iterate_over = False
         if isinstance(tree_dict, list):
-            rem = []
+            rem = {}
             for idx, val in enumerate(tree_dict):
                 if isinstance(val, dict) or isinstance(val, list):
                     if isinstance(val, dict) and SWEEP_INDICATION in val:
                         # pass a version of val without the sweep indication
                         ret[IDX_INDICATOR +
                             str(idx)] = postprocess_inner_sweep(val)
                         has_something_to_iterate_over = True
                     else:
                         flattened, has_something, subrem = flatten_tree(val)
                         if has_something:
                             has_something_to_iterate_over = True
                             for subkey, subval in flattened.items():
                                 ret[SEPARATOR.join(
                                     [IDX_INDICATOR + str(idx), subkey])] = subval
-                        rem.append(subrem)
+                        rem[IDX_INDICATOR + str(idx)] = subrem
                 else:
-                    rem.append(val)
+                    rem[IDX_INDICATOR + str(idx)] = val
         elif isinstance(tree_dict, dict):
             rem = {}
             if SWEEP_INDICATION in tree_dict:
                 for key, val in tree_dict.items():
                     if key != SWEEP_INDICATION:
                         ret[key] = val
             else:
@@ -373,18 +373,24 @@
             # sort all_sweep_group_keys
             all_sweep_group_keys.sort()
             for key in all_sweep_group_keys:
                 val = sweep_config[key]
                 new_args = upsert_config(
                     args, val, current_path + [f"{key}"], root_args)
                 args = new_args
-            for i, val in enumerate(all_upsert):
-                new_args = upsert_config(
-                    args, val, current_path + [f"{UPSERT_GROUP_IDENTIFIER}-{i}"], root_args)
-                args = new_args
+            if isinstance(all_upsert, list):
+                for i, val in enumerate(all_upsert):
+                    new_args = upsert_config(
+                        args, val, current_path + [f"{UPSERT_GROUP_IDENTIFIER}-{i}"], root_args)
+                    args = new_args
+            elif isinstance(all_upsert, dict):
+                for key, val in all_upsert.items():
+                    new_args = upsert_config(
+                        args, val, current_path + [f"{UPSERT_GROUP_IDENTIFIER}-{key}"], root_args)
+                    args = new_args
         if len(current_path) == 0:
             # Sanity check if any of the nested dicts contain special keys
             # If they do, then we need to throw an error
             # This is because we don't want to allow the user to specify
             # a sweep config that has a special key in it
             sanity_check_special_keys(args, current_path=current_path)
 
@@ -408,15 +414,15 @@
 def standardize_sweep_config(sweep_config: dict):
     global remaining_bunch
     config_copy = {k: copy.deepcopy(v) if isinstance(
         v, dict) or isinstance(v, list) else v for k, v in sweep_config.items()}
     flat, remaining_bunch = flatten_sweep_config(config_copy['parameters'])
     config_copy['parameters'] = compress_parameter_config(flat)
     global compression_mapping, value_compression_mapping
-
+    
     return config_copy, {'keys': compression_mapping, 'values': value_compression_mapping, 'remaining_bunch': remaining_bunch}
 
 
 def add_where_needed(
     base: th.Union[th.List, th.Dict],
     to_add: th.Union[th.List, th.Dict]
 ) -> th.Union[th.List, th.Dict]:
```

### Comparing `dysweep-0.0.3/dysweep/wandbX.py` & `dysweep-0.0.4/dysweep/wandbX.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.3/dysweep.egg-info/PKG-INFO` & `dysweep-0.0.4/dysweep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.0.3
+Version: 0.0.4
 Summary: A toolset for dynamic python code manipulations
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: Apache License 2.0
 Description: # DySweep: Use W&B Sweep for Everything!
```

### Comparing `dysweep-0.0.3/setup.py` & `dysweep-0.0.4/setup.py`

 * *Files identical despite different names*

