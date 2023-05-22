# Comparing `tmp/hcai-nova-server-0.1.4.tar.gz` & `tmp/hcai-nova-server-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-0.1.4.tar", last modified: Wed May 17 12:18:47 2023, max compression
+gzip compressed data, was "hcai-nova-server-0.1.5.tar", last modified: Mon May 22 14:56:17 2023, max compression
```

## Comparing `hcai-nova-server-0.1.4.tar` & `hcai-nova-server-0.1.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:18:47.443112 hcai-nova-server-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-05-17 12:18:47.443112 hcai-nova-server-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      573 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:18:47.439112 hcai-nova-server-0.1.4/hcai_nova_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-05-17 12:18:47.000000 hcai-nova-server-0.1.4/hcai_nova_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      904 2023-05-17 12:18:47.000000 hcai-nova-server-0.1.4/hcai_nova_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 12:18:47.000000 hcai-nova-server-0.1.4/hcai_nova_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-17 12:18:47.000000 hcai-nova-server-0.1.4/hcai_nova_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-17 12:18:47.000000 hcai-nova-server-0.1.4/hcai_nova_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:18:47.439112 hcai-nova-server-0.1.4/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/nova_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:18:47.439112 hcai-nova-server-0.1.4/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13062 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9891 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7744 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:18:47.443112 hcai-nova-server-0.1.4/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 12:18:47.443112 hcai-nova-server-0.1.4/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12151 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      447 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/utils/img_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 12:18:47.443112 hcai-nova-server-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-05-17 12:18:37.000000 hcai-nova-server-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:17.801628 hcai-nova-server-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-05-22 14:56:17.801628 hcai-nova-server-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      573 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:17.797628 hcai-nova-server-0.1.5/hcai_nova_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1544 2023-05-22 14:56:17.000000 hcai-nova-server-0.1.5/hcai_nova_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      904 2023-05-22 14:56:17.000000 hcai-nova-server-0.1.5/hcai_nova_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 14:56:17.000000 hcai-nova-server-0.1.5/hcai_nova_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-22 14:56:17.000000 hcai-nova-server-0.1.5/hcai_nova_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-22 14:56:17.000000 hcai-nova-server-0.1.5/hcai_nova_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:17.797628 hcai-nova-server-0.1.5/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2568 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/nova_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:17.801628 hcai-nova-server-0.1.5/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13062 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9891 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:17.801628 hcai-nova-server-0.1.5/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:17.801628 hcai-nova-server-0.1.5/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12151 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      447 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/utils/img_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 14:56:17.801628 hcai-nova-server-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2383 2023-05-22 14:56:04.000000 hcai-nova-server-0.1.5/setup.py
```

### Comparing `hcai-nova-server-0.1.4/PKG-INFO` & `hcai-nova-server-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server
-Version: 0.1.4
+Version: 0.1.5
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-0.1.4/README.md` & `hcai-nova-server-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/hcai_nova_server.egg-info/PKG-INFO` & `hcai-nova-server-0.1.5/hcai_nova_server.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server
-Version: 0.1.4
+Version: 0.1.5
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-0.1.4/hcai_nova_server.egg-info/SOURCES.txt` & `hcai-nova-server-0.1.5/hcai_nova_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/nova_server/nova_backend.py` & `hcai-nova-server-0.1.5/nova_server/nova_backend.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/nova_server/route/cancel.py` & `hcai-nova-server-0.1.5/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/nova_server/route/explain.py` & `hcai-nova-server-0.1.5/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/nova_server/route/extract.py` & `hcai-nova-server-0.1.5/nova_server/route/extract.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/nova_server/route/log.py` & `hcai-nova-server-0.1.5/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/nova_server/route/predict.py` & `hcai-nova-server-0.1.5/nova_server/route/predict.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,61 +91,41 @@
     except ValueError as e:
         print(e)
         log_utils.remove_log_from_dict(key)
         logger.error("Not able to load the data from the database!")
         status_utils.update_status(key, status_utils.JobStatus.ERROR)
         return None
 
-
     # Load Trainer
     model_script_path = (trainer_file_path.parent / PureWindowsPath(trainer.model_script_path)).resolve()
     source = SourceFileLoader(
         "ns_tr_" + model_script_path.stem, str(model_script_path)
     ).load_module()
     import_utils.assert_or_install_dependencies(
         source.REQUIREMENTS, Path(model_script_path).stem
     )
     logger.info(f"Trainer module {Path(model_script_path).name} loaded")
     trainer_class = getattr(source, trainer.model_create)
     predictor = trainer_class(logger, log_conform_request)
     logger.info(f"Model {trainer.model_create} created")
-    #model_script = source.TrainerClass(ds_iter, logger, request_form)
-
-    # Set Options
-    logger.info("Setting options...")
-    if not request_form["optStr"] == "":
-        for k, v in dict(
-            option.split("=")
-            for option in request_form["optStr"].split(";")
-        ).items():
-            if v in ("True", "False"):
-                predictor.OPTIONS[k] = True if v == "True" else False
-            elif v == "None":
-                predictor.OPTIONS[k] = True if v == "True" else False
-            else:
-                predictor.OPTIONS[k] = v
-            logger.info(k + "=" + v)
-    logger.info("...done.")
-
+    # model_script = source.TrainerClass(ds_iter, logger, request_form)
 
     # If the module implements the Trainer interface load weights
     if isinstance(predictor, iTrainer):
-
         # Load Model
         model_weight_path = (
                 trainer_file_path.parent / trainer.model_weights_path
         )
         logger.info(f"Loading weights from {model_weight_path}")
         predictor.load(model_weight_path)
         logger.info("Model loaded.")
 
     # Iterate over all sessions
     ds_iter: HcaiNovaDynamicIterable
     for ds_iter in iterators:
-
         # TODO: Remove prior creation of separate iterators to reduce redundancy
         ss_ds_iter = ds_iter.to_single_session_iterator()
 
         logger.info("Predict data...")
         data = predictor.process_data(ss_ds_iter)
         annos = predictor.to_anno(data)
         logger.info("...done")
@@ -158,50 +138,47 @@
         request_form_copy['sessions'] = ss_ds_iter.sessions[0]
         db_utils.write_annotation_to_db(request_form_copy, annos, logger)
         logger.info("...done")
 
     logger.info("Prediction completed!")
     status_utils.update_status(key, status_utils.JobStatus.FINISHED)
 
-        # model_script.ds_iter = ds_iter
-        # model_script.request_form["sessions"] = session
-        # model_script.request_form["roles"] = role
-        #
-        # logger.info("Execute preprocessing.")
-        # model_script.preprocess()
-        # logger.info("Preprocessing done.")
-        #
-        # logger.info("Execute prediction.")
-        # model_script.predict()
-        # logger.info("Prediction done.")
-        #
-        # logger.info("Execute postprocessing.")
-        # results = model_script.postprocess()
-        # logger.info("Postprocessing done.")
-        #
-        # logger.info("Execute saving process.")
-        # db_utils.write_annotation_to_db(request_form, results, logger)
-        # logger.info("Saving process done.")
-
-        # 5. In CML case, delete temporary files..
-        # if request_form["deleteFiles"] == "True":
-        #     trainer_name = request_form["trainerName"]
-        #     logger.info("Deleting temporary CML files...")
-        #     out_dir = Path(cml_dir).joinpath(
-        #         PureWindowsPath(request_form["trainerOutputDirectory"])
-        #     )
-        #     os.remove(out_dir / trainer.model_weights_path)
-        #     os.remove(out_dir / trainer.model_script_path)
-        #     for f in model_script.DEPENDENCIES:
-        #         os.remove(trainer_file_path.parent / f)
-        #     trainer_fullname = trainer_name + ".trainer"
-        #     os.remove(out_dir / trainer_fullname)
-        #     logger.info("...done")
-
-
-
+    # model_script.ds_iter = ds_iter
+    # model_script.request_form["sessions"] = session
+    # model_script.request_form["roles"] = role
+    #
+    # logger.info("Execute preprocessing.")
+    # model_script.preprocess()
+    # logger.info("Preprocessing done.")
+    #
+    # logger.info("Execute prediction.")
+    # model_script.predict()
+    # logger.info("Prediction done.")
+    #
+    # logger.info("Execute postprocessing.")
+    # results = model_script.postprocess()
+    # logger.info("Postprocessing done.")
+    #
+    # logger.info("Execute saving process.")
+    # db_utils.write_annotation_to_db(request_form, results, logger)
+    # logger.info("Saving process done.")
+
+    # 5. In CML case, delete temporary files..
+    # if request_form["deleteFiles"] == "True":
+    #     trainer_name = request_form["trainerName"]
+    #     logger.info("Deleting temporary CML files...")
+    #     out_dir = Path(cml_dir).joinpath(
+    #         PureWindowsPath(request_form["trainerOutputDirectory"])
+    #     )
+    #     os.remove(out_dir / trainer.model_weights_path)
+    #     os.remove(out_dir / trainer.model_script_path)
+    #     for f in model_script.DEPENDENCIES:
+    #         os.remove(trainer_file_path.parent / f)
+    #     trainer_fullname = trainer_name + ".trainer"
+    #     os.remove(out_dir / trainer_fullname)
+    #     logger.info("...done")
 
 # except Exception as e:
 # logger.error('Error:' + str(e))
 #   status_utils.update_status(key, status_utils.JobStatus.ERROR)
 # finally:
 #    del results, ds_iter, ds_iter_pp, model, model_script, model_script_path, model_weight_path, spec
```

### Comparing `hcai-nova-server-0.1.4/nova_server/route/status.py` & `hcai-nova-server-0.1.5/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/nova_server/route/train.py` & `hcai-nova-server-0.1.5/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/nova_server/utils/dataset_utils.py` & `hcai-nova-server-0.1.5/nova_server/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/nova_server/utils/db_utils.py` & `hcai-nova-server-0.1.5/nova_server/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/nova_server/utils/explain_utils.py` & `hcai-nova-server-0.1.5/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/nova_server/utils/import_utils.py` & `hcai-nova-server-0.1.5/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/nova_server/utils/key_utils.py` & `hcai-nova-server-0.1.5/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/nova_server/utils/log_utils.py` & `hcai-nova-server-0.1.5/nova_server/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/nova_server/utils/status_utils.py` & `hcai-nova-server-0.1.5/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/nova_server/utils/thread_utils.py` & `hcai-nova-server-0.1.5/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-0.1.4/setup.py` & `hcai-nova-server-0.1.5/setup.py`

 * *Files identical despite different names*

