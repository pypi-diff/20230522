# Comparing `tmp/dysweep-0.0.4.tar.gz` & `tmp/dysweep-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dysweep-0.0.4.tar", last modified: Mon May 22 03:53:51 2023, max compression
+gzip compressed data, was "dysweep-0.0.5.tar", last modified: Mon May 22 17:04:15 2023, max compression
```

## Comparing `dysweep-0.0.4.tar` & `dysweep-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:53:51.913491 dysweep-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 03:51:35.000000 dysweep-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-22 03:53:51.913491 dysweep-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 03:51:35.000000 dysweep-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:53:51.913491 dysweep-0.0.4/dysweep/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 03:51:35.000000 dysweep-0.0.4/dysweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-22 03:51:35.000000 dysweep-0.0.4/dysweep/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    20767 2023-05-22 03:51:35.000000 dysweep-0.0.4/dysweep/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-05-22 03:51:35.000000 dysweep-0.0.4/dysweep/wandbX.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 03:53:51.913491 dysweep-0.0.4/dysweep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-22 03:53:51.000000 dysweep-0.0.4/dysweep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-22 03:53:51.000000 dysweep-0.0.4/dysweep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 03:53:51.000000 dysweep-0.0.4/dysweep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 03:53:51.000000 dysweep-0.0.4/dysweep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 03:53:51.913491 dysweep-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-22 03:51:35.000000 dysweep-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:15.000854 dysweep-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 17:01:33.000000 dysweep-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-22 17:04:15.000854 dysweep-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 17:01:33.000000 dysweep-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:15.000854 dysweep-0.0.5/dysweep/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 17:01:33.000000 dysweep-0.0.5/dysweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-22 17:01:33.000000 dysweep-0.0.5/dysweep/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20432 2023-05-22 17:01:33.000000 dysweep-0.0.5/dysweep/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-05-22 17:01:33.000000 dysweep-0.0.5/dysweep/wandbX.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:04:15.000854 dysweep-0.0.5/dysweep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-22 17:04:14.000000 dysweep-0.0.5/dysweep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-22 17:04:14.000000 dysweep-0.0.5/dysweep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:04:14.000000 dysweep-0.0.5/dysweep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 17:04:14.000000 dysweep-0.0.5/dysweep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 17:04:15.000854 dysweep-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-22 17:01:33.000000 dysweep-0.0.5/setup.py
```

### Comparing `dysweep-0.0.4/LICENSE` & `dysweep-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.4/PKG-INFO` & `dysweep-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.0.4
+Version: 0.0.5
 Summary: A toolset for dynamic python code manipulations
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: Apache License 2.0
 Description: # DySweep: Use W&B Sweep for Everything!
```

### Comparing `dysweep-0.0.4/dysweep/parallel.py` & `dysweep-0.0.5/dysweep/parallel.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.4/dysweep/utils.py` & `dysweep-0.0.5/dysweep/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,38 +6,39 @@
 import json
 import copy
 
 SEPARATOR = "__CUSTOM_SEPERATOR__"
 IDX_INDICATOR = "__IDX__"
 
 SWEEP_INDICATION = "sweep"
-UNIQUE_NAME_IDENT = "sweep_identifier"
-VALUES_DISPLAY_NAME = "sweep_alias"
+SWEEP_IDENT = "sweep_identifier"
+SWEEP_ALIAS = "sweep_alias"
 SWEEP_GROUP = "sweep_group"
-UPSERT_GROUP_IDENTIFIER = "upsert"
-SWEEP_LIST_OPERATIONS = "sweep_list_operations"
-SWEEP_LIST_INSERT = "sweep_insert"
-SWEEP_LIST_REMOVE = "sweep_remove"
-SWEEP_LIST_OVERWRITE = "sweep_overwrite"
-SWEEP_OPERATION_VAL = "dy_eval"
+
+DY_UPSERT = "dy__upsert"
+DY_LIST_OPERATIONS = "dy__list__operations"
+DY_LIST_INSERT = "dy__insert"
+DY_LIST_REMOVE = "dy__remove"
+DY_LIST_OVERWRITE = "dy__overwrite"
+DY_EVAL = "dy__eval"
 
 SPLIT = "-"
 EXCEPTION_OCCURED = False
 
 SPECIAL_KEYS = [
     SWEEP_INDICATION,
-    UNIQUE_NAME_IDENT,
-    VALUES_DISPLAY_NAME,
+    SWEEP_IDENT,
+    SWEEP_ALIAS,
     SWEEP_GROUP,
-    SWEEP_LIST_OPERATIONS,
-    UPSERT_GROUP_IDENTIFIER,
-    SWEEP_OPERATION_VAL,
-    SWEEP_LIST_INSERT,
-    SWEEP_LIST_REMOVE,
-    SWEEP_LIST_OVERWRITE,
+    DY_LIST_OPERATIONS,
+    DY_UPSERT,
+    DY_EVAL,
+    DY_LIST_INSERT,
+    DY_LIST_REMOVE,
+    DY_LIST_OVERWRITE,
 ]
 
 compression_mapping = {}
 value_compression_mapping = {}
 remaining_bunch = {}
 
 
@@ -47,28 +48,28 @@
     global compression_mapping
     global value_compression_mapping
 
     # if unique identifiers are provided in the sweep config, use them
     for key, val in parameter_config.items():
         if isinstance(val, dict):
             inner_dict = val.copy()
-            if UNIQUE_NAME_IDENT in inner_dict:
-                compression_mapping[key] = inner_dict[UNIQUE_NAME_IDENT]
-                inner_dict.pop(UNIQUE_NAME_IDENT)
-            if VALUES_DISPLAY_NAME in inner_dict and "values" in inner_dict:
+            if SWEEP_IDENT in inner_dict:
+                compression_mapping[key] = inner_dict[SWEEP_IDENT]
+                inner_dict.pop(SWEEP_IDENT)
+            if SWEEP_ALIAS in inner_dict and "values" in inner_dict:
                 new_values = []
                 for idx, value in enumerate(inner_dict["values"]):
-                    if inner_dict[VALUES_DISPLAY_NAME][idx] in value_compression_mapping:
+                    if inner_dict[SWEEP_ALIAS][idx] in value_compression_mapping:
                         raise Exception(
-                            f"Value {inner_dict[VALUES_DISPLAY_NAME][idx]} is already used in the sweep config"
+                            f"Value {inner_dict[SWEEP_ALIAS][idx]} is already used in the sweep config"
                         )
-                    value_compression_mapping[inner_dict[VALUES_DISPLAY_NAME][idx]] = value
-                    new_values.append(inner_dict[VALUES_DISPLAY_NAME][idx])
+                    value_compression_mapping[inner_dict[SWEEP_ALIAS][idx]] = value
+                    new_values.append(inner_dict[SWEEP_ALIAS][idx])
                 inner_dict["values"] = new_values
-                inner_dict.pop(VALUES_DISPLAY_NAME)
+                inner_dict.pop(SWEEP_ALIAS)
             parameter_config[key] = inner_dict
 
     all_keys = list(parameter_config.keys())
     for key in all_keys:
         to_path = key.split(SEPARATOR)
         # reverse to_path
         from_path = to_path[::-1]
@@ -203,126 +204,132 @@
                   sweep_config: th.Union[th.Dict, th.List, int, float, str],
                   current_path: th.Optional[th.List[str]] = None,
                   root_args: th.Optional[th.Union[th.Dict, th.List]] = None):
     # try and catch an exception and add "line" to the exception and then re-raise it
     if current_path is None:
         current_path = []
     if root_args is None:
-        root_args = [x for x in args] if isinstance(
-            args, list) else {k: v for k, v in args.items()}
-
+        root_args = args
+        
     try:
         if isinstance(args, list):
             if isinstance(sweep_config, dict):
-                if SWEEP_LIST_OPERATIONS in sweep_config:
-                    ops = sweep_config.pop(SWEEP_LIST_OPERATIONS)
+                if DY_LIST_OPERATIONS in sweep_config:
+                    ops = sweep_config.pop(DY_LIST_OPERATIONS)
+                    
+                    # Convert operations from dictionary to a list
                     if not isinstance(ops, list):
-                        raise Exception(
-                            f"Expected a list for {SWEEP_LIST_OPERATIONS} but got: {type(ops)}")
+                        real_ops = [None for _ in range(len(ops.keys()))]
+                        for key, val in ops.items():
+                            real_ops[int(key[len(IDX_INDICATOR):])] = val
+                        ops = real_ops
+                    
+                    
                     for op in ops:
                         if len(op.keys()) != 1:
                             raise Exception(
                                 "Any sweep list operation should be a dictionary with a single key")
-                        if SWEEP_LIST_INSERT in op:
+                        if DY_LIST_INSERT in op:
                             val = None
-                            idx = op[SWEEP_LIST_INSERT]
+                            idx = op[DY_LIST_INSERT]
                             if not isinstance(idx, int):
                                 if isinstance(idx, list):
                                     if len(idx) != 2:
                                         raise Exception(
-                                            f"Expected a list of length 2 for {SWEEP_LIST_INSERT} but got: {idx}")
+                                            f"Expected a list of length 2 for {DY_LIST_INSERT} but got: {idx}")
                                     val = idx[1]
                                     idx = idx[0]
                                 else:
                                     raise Exception(
-                                        f"Expected an integer for {SWEEP_LIST_INSERT} but got: {idx}")
+                                        f"Expected an integer for {DY_LIST_INSERT} but got: {idx}")
                             if idx == -1:
                                 args.append(
                                     sweep_config if val is None else val)
                             else:
                                 args.insert(
                                     idx, sweep_config if val is None else val)
-                        elif SWEEP_LIST_OVERWRITE in op:
+                        elif DY_LIST_OVERWRITE in op:
                             val = None
-                            idx = op[SWEEP_LIST_OVERWRITE]
+                            idx = op[DY_LIST_OVERWRITE]
                             if not isinstance(idx, int):
                                 if isinstance(idx, list):
                                     if len(idx) != 2:
                                         raise Exception(
-                                            f"Expected a list of length 2 for {SWEEP_LIST_OVERWRITE} but got: {idx}")
+                                            f"Expected a list of length 2 for {DY_LIST_OVERWRITE} but got: {idx}")
 
                                     val = idx[1]
                                     idx = idx[0]
                                 else:
                                     raise Exception(
-                                        f"Expected an integer for {SWEEP_LIST_OVERWRITE} but got: {idx}")
+                                        f"Expected an integer for {DY_LIST_OVERWRITE} but got: {idx}")
                             if val is None:
                                 new_arg = upsert_config(
                                     args[idx], sweep_config, current_path + [str(idx)], root_args)
                                 args[idx] = new_arg
                             else:
                                 args[idx] = val
-                        elif SWEEP_LIST_REMOVE in op:
-                            idx = op[SWEEP_LIST_REMOVE]
+                        elif DY_LIST_REMOVE in op:
+                            idx = op[DY_LIST_REMOVE]
                             if not isinstance(idx, int):
                                 raise Exception(
-                                    f"Expected an integer for {SWEEP_LIST_REMOVE} but got: {idx}")
+                                    f"Expected an integer for {DY_LIST_REMOVE} but got: {idx}")
                             args.pop(idx)
                         else:
                             raise Exception(
                                 f"Unknown sweep list operation: {op}")
-                    sweep_config[SWEEP_LIST_OPERATIONS] = ops
+                
+                    sweep_config[DY_LIST_OPERATIONS] = ops
                 else:
                     for key, val in sweep_config.items():
                         args_key = int(key[len(IDX_INDICATOR):])
                         if isinstance(val, dict) or isinstance(val, list):
 
-                            if isinstance(val, dict) and SWEEP_OPERATION_VAL in val:
-                                if isinstance(val[SWEEP_OPERATION_VAL], str):
+                            if isinstance(val, dict) and DY_EVAL in val:
+                                if isinstance(val[DY_EVAL], str):
                                     args[key] = dy.eval(
-                                        val[SWEEP_OPERATION_VAL])(root_args)
+                                        val[DY_EVAL])(root_args)
                                 else:
                                     args[key] = dy.eval(
-                                        **val[SWEEP_OPERATION_VAL])(root_args)
+                                        **val[DY_EVAL])(root_args)
                                 continue
 
                             new_args = upsert_config(
                                 args[args_key], val, current_path + [str(args_key)], root_args)
                             args[args_key] = new_args
 
-                        elif not isinstance(val, str) or val.find(SWEEP_OPERATION_VAL) == -1:
+                        elif not isinstance(val, str) or val.find(DY_EVAL) == -1:
                             args[args_key] = val
                         else:
-                            pat = f"{SWEEP_OPERATION_VAL}\((.*)\)"
+                            pat = f"{DY_EVAL}\((.*)\)"
                             func_to_eval = re.search(pat, val).group(1)
                             args[args_key] = dy.eval(
                                 func_to_eval)(args[args_key])
             elif isinstance(sweep_config, list):
                 if len(sweep_config) != len(args):
                     raise Exception(
                         f"Expected a list of length {len(args)} but got a list of length {len(sweep_config)}")
                 for idx, val in enumerate(sweep_config):
                     if isinstance(val, dict) or isinstance(val, list):
 
-                        if isinstance(val, dict) and SWEEP_OPERATION_VAL in val:
-                            if isinstance(val[SWEEP_OPERATION_VAL], str):
+                        if isinstance(val, dict) and DY_EVAL in val:
+                            if isinstance(val[DY_EVAL], str):
                                 args[key] = dy.eval(
-                                    val[SWEEP_OPERATION_VAL])(root_args)
+                                    val[DY_EVAL])(root_args)
                             else:
                                 args[key] = dy.eval(
-                                    **val[SWEEP_OPERATION_VAL])(root_args)
+                                    **val[DY_EVAL])(root_args)
                             continue
 
                         new_args = upsert_config(
                             args[idx], val, current_path + [str(idx)], root_args)
                         args[idx] = new_args
-                    elif not isinstance(val, str) or val.find(SWEEP_OPERATION_VAL) == -1:
+                    elif not isinstance(val, str) or val.find(DY_EVAL) == -1:
                         args[idx] = val
                     else:
-                        pat = f"{SWEEP_OPERATION_VAL}\((.*)\)"
+                        pat = f"{DY_EVAL}\((.*)\)"
                         func_to_eval = re.search(pat, val).group(1)
                         args[idx] = dy.eval(func_to_eval)(args[idx])
 
         else:
             all_sweep_group_keys = []
             if isinstance(args, dict):
                 is_list_pretender = True
@@ -332,64 +339,64 @@
                 if is_list_pretender:
                     true_args = [None for _ in range(len(args.keys()))]
                     for key in args.keys():
                         true_args[int(key[len(IDX_INDICATOR):])] = args[key]
                     return upsert_config(true_args, sweep_config, current_path, root_args)
                 else:
                     all_upsert = []
-                    if UPSERT_GROUP_IDENTIFIER in sweep_config:
-                        all_upsert = sweep_config.pop(UPSERT_GROUP_IDENTIFIER)
+                    if DY_UPSERT in sweep_config:
+                        all_upsert = sweep_config.pop(DY_UPSERT)
                     for key, val in sweep_config.items():
                         if key.startswith(SWEEP_GROUP):
                             all_sweep_group_keys.append(key)
                             continue
                         if key not in args:
                             args[key] = None
                         if isinstance(val, dict) or isinstance(val, list):
 
-                            if isinstance(val, dict) and SWEEP_OPERATION_VAL in val:
-                                if isinstance(val[SWEEP_OPERATION_VAL], str):
+                            if isinstance(val, dict) and DY_EVAL in val:
+                                if isinstance(val[DY_EVAL], str):
                                     args[key] = dy.eval(
-                                        val[SWEEP_OPERATION_VAL])(root_args)
+                                        val[DY_EVAL])(root_args)
                                 else:
                                     args[key] = dy.eval(
-                                        **val[SWEEP_OPERATION_VAL])(root_args)
+                                        **val[DY_EVAL])(root_args)
                                 continue
 
                             new_args = upsert_config(
                                 args[key] if key in args else None, val, current_path + [str(key)], root_args)
                             args[key] = new_args
-                        elif not isinstance(val, str) or val.find(SWEEP_OPERATION_VAL) == -1:
+                        elif not isinstance(val, str) or val.find(DY_EVAL) == -1:
                             args[key] = val
                         else:
-                            pat = f"{SWEEP_OPERATION_VAL}\((.*)\)"
+                            pat = f"{DY_EVAL}\((.*)\)"
                             func_to_eval = re.search(pat, val).group(1)
                             args[key] = dy.eval(func_to_eval)(args[key])
-            elif isinstance(sweep_config, str) and sweep_config.find(SWEEP_OPERATION_VAL) != -1:
-                pat = f"{SWEEP_OPERATION_VAL}\((.*)\)"
+            elif isinstance(sweep_config, str) and sweep_config.find(DY_EVAL) != -1:
+                pat = f"{DY_EVAL}\((.*)\)"
                 func_to_eval = re.search(pat, sweep_config).group(1)
                 return dy.eval(func_to_eval)(args)
             else:
                 return sweep_config
             # sort all_sweep_group_keys
             all_sweep_group_keys.sort()
             for key in all_sweep_group_keys:
                 val = sweep_config[key]
                 new_args = upsert_config(
                     args, val, current_path + [f"{key}"], root_args)
                 args = new_args
             if isinstance(all_upsert, list):
                 for i, val in enumerate(all_upsert):
                     new_args = upsert_config(
-                        args, val, current_path + [f"{UPSERT_GROUP_IDENTIFIER}-{i}"], root_args)
+                        args, val, current_path + [f"{DY_UPSERT}-{i}"], root_args)
                     args = new_args
             elif isinstance(all_upsert, dict):
                 for key, val in all_upsert.items():
                     new_args = upsert_config(
-                        args, val, current_path + [f"{UPSERT_GROUP_IDENTIFIER}-{key}"], root_args)
+                        args, val, current_path + [f"{DY_UPSERT}-{key}"], root_args)
                     args = new_args
         if len(current_path) == 0:
             # Sanity check if any of the nested dicts contain special keys
             # If they do, then we need to throw an error
             # This is because we don't want to allow the user to specify
             # a sweep config that has a special key in it
             sanity_check_special_keys(args, current_path=current_path)
@@ -461,9 +468,11 @@
         compression_mapping = mapping['keys']
         value_compression_mapping = mapping['values']
         remaining_bunch = mapping['remaining_bunch']
     config_copy = {k: copy.deepcopy(v) if isinstance(
         v, dict) or isinstance(v, list) else v for k, v in sweep_config.items()}
     config_copy = unflatten_sweep_config(
         decompress_parameter_config(config_copy))
+    
     ret = add_where_needed(config_copy, remaining_bunch)
+
     return ret
```

### Comparing `dysweep-0.0.4/dysweep/wandbX.py` & `dysweep-0.0.5/dysweep/wandbX.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import wandb
 from pprint import pprint
 import os
 from .utils import standardize_sweep_config, destandardize_sweep_config, upsert_config
 from wandb.sdk.wandb_run import Run, _run_decorator
 from wandb.sdk import wandb_config
 import warnings
+import copy
 
 METADATA_RUN_NAME_PREFIX = "HIERARCHICAL_SWEEP_"
-ARTIFACT_NAME = "hierarchical_sweep"
 
 base_config: th.Optional[dict] = None
 compression: th.Optional[dict] = None
 
 
 def hierarchical_config(conf):
     if base_config is None or compression is None:
         return conf
-    return upsert_config(base_config, destandardize_sweep_config(conf, compression))
+    # make a deep copy of the base config
+    return upsert_config(copy.deepcopy(base_config), destandardize_sweep_config(conf, compression))
 
 
 def sweep(
     base_config: dict,
     sweep_config: dict,
     entity: th.Optional[str] = None,
     project: th.Optional[str] = None,
```

### Comparing `dysweep-0.0.4/dysweep.egg-info/PKG-INFO` & `dysweep-0.0.5/dysweep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.0.4
+Version: 0.0.5
 Summary: A toolset for dynamic python code manipulations
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: Apache License 2.0
 Description: # DySweep: Use W&B Sweep for Everything!
```

### Comparing `dysweep-0.0.4/setup.py` & `dysweep-0.0.5/setup.py`

 * *Files identical despite different names*

