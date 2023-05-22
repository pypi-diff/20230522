# Comparing `tmp/dysweep-0.0.1.tar.gz` & `tmp/dysweep-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dysweep-0.0.1.tar", last modified: Sun May 21 23:36:43 2023, max compression
+gzip compressed data, was "dysweep-0.0.2.tar", last modified: Mon May 22 00:57:00 2023, max compression
```

## Comparing `dysweep-0.0.1.tar` & `dysweep-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:36:43.090593 dysweep-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-21 23:34:26.000000 dysweep-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-21 23:36:43.090593 dysweep-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-21 23:34:26.000000 dysweep-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:36:43.090593 dysweep-0.0.1/dysweep/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-21 23:34:26.000000 dysweep-0.0.1/dysweep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-05-21 23:34:26.000000 dysweep-0.0.1/dysweep/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    20319 2023-05-21 23:34:26.000000 dysweep-0.0.1/dysweep/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-21 23:34:26.000000 dysweep-0.0.1/dysweep/wandbX.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 23:36:43.090593 dysweep-0.0.1/dysweep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-21 23:36:43.000000 dysweep-0.0.1/dysweep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-21 23:36:43.000000 dysweep-0.0.1/dysweep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 23:36:43.000000 dysweep-0.0.1/dysweep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 23:36:43.000000 dysweep-0.0.1/dysweep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 23:36:43.090593 dysweep-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-21 23:34:26.000000 dysweep-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:57:00.325097 dysweep-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-22 00:54:48.000000 dysweep-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-22 00:57:00.325097 dysweep-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-22 00:54:48.000000 dysweep-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:57:00.321097 dysweep-0.0.2/dysweep/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 00:54:48.000000 dysweep-0.0.2/dysweep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-05-22 00:54:48.000000 dysweep-0.0.2/dysweep/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20382 2023-05-22 00:54:48.000000 dysweep-0.0.2/dysweep/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4068 2023-05-22 00:54:48.000000 dysweep-0.0.2/dysweep/wandbX.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 00:57:00.325097 dysweep-0.0.2/dysweep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-22 00:57:00.000000 dysweep-0.0.2/dysweep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-22 00:57:00.000000 dysweep-0.0.2/dysweep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 00:57:00.000000 dysweep-0.0.2/dysweep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-22 00:57:00.000000 dysweep-0.0.2/dysweep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 00:57:00.325097 dysweep-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-22 00:54:48.000000 dysweep-0.0.2/setup.py
```

### Comparing `dysweep-0.0.1/LICENSE` & `dysweep-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.1/PKG-INFO` & `dysweep-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.0.1
+Version: 0.0.2
 Summary: A toolset for dynamic python code manipulations
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: Apache License 2.0
 Description: # DySweep: Use W&B Sweep for Everything!
```

### Comparing `dysweep-0.0.1/dysweep/parallel.py` & `dysweep-0.0.2/dysweep/parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,33 +60,37 @@
                 # they were created.
                 all_subdirs = [
                     d for d in checkpoint_dir.iterdir() if d.is_dir()]
                 all_subdirs = sorted(
                     all_subdirs, key=lambda x: int(x.name.split(SPLIT)[0]))
 
                 # Change the run-name by adding something random to it
+                # if the conf.run_name is None just assign it to None
+                # and wandb will handle the rest.
                 if conf.run_name is not None:
                     r = RandomWords()
                     w = r.get_random_word()
                     run_name = conf.run_name + '-' + w
+                else:
+                    run_name = conf.run_name
 
                 if conf.resume:
                     # Resuming mode
                     if len(all_subdirs) == 0:
                         raise ValueError(
                             f"The checkpoint directory {checkpoint_dir} is empty, so you can't resume from it.")
                     # get the name of the directory that we are trying to resume which
                     # contains the resume_id in its name.
                     dir_name = all_subdirs[0].name
                     resume_id = SPLIT.join(dir_name.split(SPLIT)[1:])
 
                     if conf.use_lightning_logger:
                         # Create a WandbLogger with the resume_id
-                        import lightning.pytorch as pl
-                        logger = pl.WandbLogger(
+                        from lightning.pytorch.loggers import WandbLogger
+                        logger = WandbLogger(
                             project=conf.project,
                             entity=conf.entity,
                             name=run_name,
                             id=resume_id,
                             resume="must",
                         )
                     else:
@@ -114,16 +118,16 @@
 
                     # create a new checkpoint directory for the inner function
                     new_checkpoint_dir = checkpoint_dir / new_dir_name
                 else:
                     # if the run_id doesn't exist, then create a new run
                     # and create the subdirectory
                     if conf.use_lightning_logger:
-                        import lightning.pytorch as pl
-                        logger = pl.WandbLogger(
+                        from lightning.pytorch.loggers import WandbLogger
+                        logger = WandbLogger(
                             project=conf.project,
                             entity=conf.entity,
                             name=run_name,
                         )
                         experiment_id = logger.experiment.id
                         sweep_config = logger.experiment.config
                     else:
@@ -135,14 +139,15 @@
                         )
                         experiment_id = wandb.run.id
                         sweep_config = wandb.config
 
                     new_dir_name = f"{len(all_subdirs)+1}{SPLIT}{experiment_id}"
 
                     os.makedirs(checkpoint_dir / new_dir_name)
+
                     # dump a json in checkpoint_dir/run_id containing the sweep config
                     with open(checkpoint_dir / new_dir_name / "sweep_config.json", "w") as f:
                         json.dump(sweep_config, f)
 
                 new_checkpoint_dir = checkpoint_dir / new_dir_name
             except Exception as e:
                 print(traceback.format_exc())
```

### Comparing `dysweep-0.0.1/dysweep/utils.py` & `dysweep-0.0.2/dysweep/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -403,19 +403,20 @@
         raise e
 
     return args
 
 
 def standardize_sweep_config(sweep_config: dict):
     global remaining_bunch
-    config_copy = {k: v.copy() if isinstance(
-        v, dict) else v for k, v in sweep_config.items()}
+    config_copy = {k: copy.deepcopy(v) if isinstance(
+        v, dict) or isinstance(v, list) else v for k, v in sweep_config.items()}
     flat, remaining_bunch = flatten_sweep_config(config_copy['parameters'])
     config_copy['parameters'] = compress_parameter_config(flat)
     global compression_mapping, value_compression_mapping
+
     return config_copy, {'keys': compression_mapping, 'values': value_compression_mapping, 'remaining_bunch': remaining_bunch}
 
 
 def add_where_needed(
     base: th.Union[th.List, th.Dict],
     to_add: th.Union[th.List, th.Dict]
 ) -> th.Union[th.List, th.Dict]:
@@ -450,13 +451,13 @@
     mapping: th.Optional[dict] = None,
 ) -> dict:
     global compression_mapping, value_compression_mapping, remaining_bunch
     if mapping is not None:
         compression_mapping = mapping['keys']
         value_compression_mapping = mapping['values']
         remaining_bunch = mapping['remaining_bunch']
-    config_copy = {k: v.copy() if isinstance(
-        v, dict) else v for k, v in sweep_config.items()}
+    config_copy = {k: copy.deepcopy(v) if isinstance(
+        v, dict) or isinstance(v, list) else v for k, v in sweep_config.items()}
     config_copy = unflatten_sweep_config(
         decompress_parameter_config(config_copy))
     ret = add_where_needed(config_copy, remaining_bunch)
     return ret
```

### Comparing `dysweep-0.0.1/dysweep/wandbX.py` & `dysweep-0.0.2/dysweep/wandbX.py`

 * *Files identical despite different names*

### Comparing `dysweep-0.0.1/dysweep.egg-info/PKG-INFO` & `dysweep-0.0.2/dysweep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dysweep
-Version: 0.0.1
+Version: 0.0.2
 Summary: A toolset for dynamic python code manipulations
 Home-page: https://github.com/HamidrezaKmK/dysweep
 Author: Hamid Kamkari
 Author-email: hamidrezakamkari@gmail.com
 License: Apache License 2.0
 Description: # DySweep: Use W&B Sweep for Everything!
```

### Comparing `dysweep-0.0.1/setup.py` & `dysweep-0.0.2/setup.py`

 * *Files identical despite different names*

