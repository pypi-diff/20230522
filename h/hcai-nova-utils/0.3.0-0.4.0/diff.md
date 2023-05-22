# Comparing `tmp/hcai-nova-utils-0.3.0.tar.gz` & `tmp/hcai-nova-utils-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-utils-0.3.0.tar", last modified: Wed May 17 07:37:47 2023, max compression
+gzip compressed data, was "hcai-nova-utils-0.4.0.tar", last modified: Mon May 22 14:54:42 2023, max compression
```

## Comparing `hcai-nova-utils-0.3.0.tar` & `hcai-nova-utils-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:47.086952 hcai-nova-utils-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-05-17 07:37:47.086952 hcai-nova-utils-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:47.082952 hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-05-17 07:37:46.000000 hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      664 2023-05-17 07:37:47.000000 hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 07:37:46.000000 hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-17 07:37:46.000000 hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-17 07:37:46.000000 hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:47.082952 hcai-nova-utils-0.3.0/nova_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:47.082952 hcai-nova-utils-0.3.0/nova_utils/db_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/db_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/db_utils/nova_types.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:47.082952 hcai-nova-utils-0.3.0/nova_utils/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      616 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/interfaces/dataset_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)     6821 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/interfaces/server_module.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:47.082952 hcai-nova-utils-0.3.0/nova_utils/ssi_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/ssi_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6664 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_data_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_sample_list_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     4545 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_stream_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8508 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_xml_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 07:37:47.086952 hcai-nova-utils-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-05-17 07:37:28.000000 hcai-nova-utils-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:42.896829 hcai-nova-utils-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-05-22 14:54:42.896829 hcai-nova-utils-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:42.892828 hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-05-22 14:54:42.000000 hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      664 2023-05-22 14:54:42.000000 hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 14:54:42.000000 hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 14:54:42.000000 hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-22 14:54:42.000000 hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:42.892828 hcai-nova-utils-0.4.0/nova_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:42.892828 hcai-nova-utils-0.4.0/nova_utils/db_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/db_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/db_utils/nova_types.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:42.892828 hcai-nova-utils-0.4.0/nova_utils/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      616 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/interfaces/dataset_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7501 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/interfaces/server_module.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:42.896829 hcai-nova-utils-0.4.0/nova_utils/ssi_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/ssi_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6664 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3783 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_sample_list_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4545 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_stream_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8551 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_xml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-22 14:54:42.896829 hcai-nova-utils-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2046 2023-05-22 14:54:26.000000 hcai-nova-utils-0.4.0/setup.py
```

### Comparing `hcai-nova-utils-0.3.0/PKG-INFO` & `hcai-nova-utils-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-utils
-Version: 0.3.0
+Version: 0.4.0
 Summary: This repository contains utility functions and interfaces that can be used to interact with the NOVA annotation tool.
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/PKG-INFO` & `hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-utils
-Version: 0.3.0
+Version: 0.4.0
 Summary: This repository contains utility functions and interfaces that can be used to interact with the NOVA annotation tool.
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hcai-nova-utils-0.3.0/hcai_nova_utils.egg-info/SOURCES.txt` & `hcai-nova-utils-0.4.0/hcai_nova_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.3.0/nova_utils/db_utils/nova_types.py` & `hcai-nova-utils-0.4.0/nova_utils/db_utils/nova_types.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.3.0/nova_utils/interfaces/dataset_iterable.py` & `hcai-nova-utils-0.4.0/nova_utils/interfaces/dataset_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.3.0/nova_utils/interfaces/server_module.py` & `hcai-nova-utils-0.4.0/nova_utils/interfaces/server_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,23 +29,39 @@
     Base class of a data processor. This interface builds the foundation for all data processing classes.
     """
 
     # List of dependencies that need to be installed when the script is loaded
     DEPENDENCIES = []
 
     # Flag to indicate whether the processed input belongs to one role or to multiple roles
-    # SINGLE_ROLE_INPUT = True
+    SINGLE_ROLE_INPUT = True
 
     def __init__(self, logger, request_form=None):
         self.logger = logger
         self.request_form = request_form
-        self.options = {"input_1": None}
         self.model = None
         self.data = None
         self.output = None
+        self.options = {}
+
+        if self.request_form is not None:
+            # Set Options
+            logger.info("Setting options...")
+            if not request_form["optStr"] == "":
+                for k, v in dict(
+                        option.split("=") for option in request_form["optStr"].split(";")
+                ).items():
+                    if v in ("True", "False"):
+                        self.options[k] = True if v == "True" else False
+                    elif v == "None":
+                        self.options[k] = True if v == "True" else False
+                    else:
+                        self.options[k] = v
+                    logger.info(k + "=" + v)
+            logger.info("...done.")
 
     @abstractmethod
     def preprocess_sample(self, sample: dict ):
         """Preprocess data to convert between nova-server dataset iterator item to the raw model input as required in process_sample.
 
         Args:
             sample (dict):
```

### Comparing `hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_anno_utils.py` & `hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_anno_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_data_types.py` & `hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_data_types.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_sample_list_utils.py` & `hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_sample_list_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_stream_utils.py` & `hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_stream_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-utils-0.3.0/nova_utils/ssi_utils/ssi_xml_utils.py` & `hcai-nova-utils-0.4.0/nova_utils/ssi_utils/ssi_xml_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
             meta_left_ctx: int = 0,
             meta_balance: str = "none",
             meta_backend: str = "nova-server",
             ssi_v="5",
             xml_version="1.0",
     ):
 
+        self.model_multi_role_input = None
         self.model_script_path = model_script_path
         self.model_option_path = model_option_path
         self.model_optstr = model_option_string
         self.model_weights_path = model_weights_path
         self.model_stream = model_stream
         self.model_create = model_create
         self.users = users if users is not None else []
```

### Comparing `hcai-nova-utils-0.3.0/setup.py` & `hcai-nova-utils-0.4.0/setup.py`

 * *Files identical despite different names*

