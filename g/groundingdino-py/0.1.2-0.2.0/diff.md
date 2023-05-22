# Comparing `tmp/groundingdino-py-0.1.2.tar.gz` & `tmp/groundingdino-py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groundingdino-py-0.1.2.tar", last modified: Mon May 22 17:23:23 2023, max compression
+gzip compressed data, was "groundingdino-py-0.2.0.tar", last modified: Mon May 22 17:31:32 2023, max compression
```

## Comparing `groundingdino-py-0.1.2.tar` & `groundingdino-py-0.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.419133 groundingdino-py-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    28221 2023-05-22 17:23:23.419133 groundingdino-py-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.399133 groundingdino-py-0.1.2/groundingdino/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.399133 groundingdino-py-0.1.2/groundingdino/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/config/GroundingDINO_SwinB_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/config/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.399133 groundingdino-py-0.1.2/groundingdino/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/datasets/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.403133 groundingdino-py-0.1.2/groundingdino/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.407133 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.411133 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/backbone.py
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/bertwarper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/fuse_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    16691 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/groundingdino.py
--rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/ms_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)    36805 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/transformer_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.415133 groundingdino-py-0.1.2/groundingdino/util/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/get_tokenlizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/slconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/slio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/vl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 17:23:23.000000 groundingdino-py-0.1.2/groundingdino/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.419133 groundingdino-py-0.1.2/groundingdino_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28221 2023-05-22 17:23:23.000000 groundingdino-py-0.1.2/groundingdino_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-22 17:23:23.000000 groundingdino-py-0.1.2/groundingdino_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:23:23.000000 groundingdino-py-0.1.2/groundingdino_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 17:23:23.000000 groundingdino-py-0.1.2/groundingdino_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 17:23:23.000000 groundingdino-py-0.1.2/groundingdino_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-22 17:23:23.419133 groundingdino-py-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:31:32.141072 groundingdino-py-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-05-22 17:31:32.141072 groundingdino-py-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:31:32.129072 groundingdino-py-0.2.0/groundingdino/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:31:32.133072 groundingdino-py-0.2.0/groundingdino/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/config/GroundingDINO_SwinB_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/config/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:31:32.133072 groundingdino-py-0.2.0/groundingdino/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/datasets/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:31:32.133072 groundingdino-py-0.2.0/groundingdino/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:31:32.137072 groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:31:32.137072 groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/backbone/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/bertwarper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/fuse_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16691 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/groundingdino.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/ms_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36805 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/transformer_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:31:32.141072 groundingdino-py-0.2.0/groundingdino/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/util/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/util/get_tokenlizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/util/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/util/slconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/util/slio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/util/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/util/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/groundingdino/util/vl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 17:31:32.000000 groundingdino-py-0.2.0/groundingdino/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:31:32.141072 groundingdino-py-0.2.0/groundingdino_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28214 2023-05-22 17:31:32.000000 groundingdino-py-0.2.0/groundingdino_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-22 17:31:32.000000 groundingdino-py-0.2.0/groundingdino_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:31:32.000000 groundingdino-py-0.2.0/groundingdino_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 17:31:32.000000 groundingdino-py-0.2.0/groundingdino_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 17:31:32.000000 groundingdino-py-0.2.0/groundingdino_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-22 17:31:32.141072 groundingdino-py-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7334 2023-05-22 17:28:53.000000 groundingdino-py-0.2.0/setup.py
```

### Comparing `groundingdino-py-0.1.2/LICENSE` & `groundingdino-py-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/PKG-INFO` & `groundingdino-py-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: groundingdino-py
-Version: 0.1.2
+Version: 0.2.0
 Summary: open-set object detector
-Home-page: https://github.com/IDEA-Research/GroundingDINO
+Home-page: https://github.com/giswqs/GroundingDINO
 Author: International Digital Economy Academy, Shilong Liu
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `groundingdino-py-0.1.2/README.md` & `groundingdino-py-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/config/GroundingDINO_SwinB_cfg.py` & `groundingdino-py-0.2.0/groundingdino/config/GroundingDINO_SwinB_cfg.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/config/GroundingDINO_SwinT_OGC.py` & `groundingdino-py-0.2.0/groundingdino/config/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/datasets/transforms.py` & `groundingdino-py-0.2.0/groundingdino/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/__init__.py` & `groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/__init__.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/backbone.py` & `groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/position_encoding.py` & `groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/backbone/position_encoding.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/swin_transformer.py` & `groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/backbone/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/bertwarper.py` & `groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/bertwarper.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/fuse_modules.py` & `groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/fuse_modules.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/groundingdino.py` & `groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/groundingdino.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/ms_deform_attn.py` & `groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/transformer.py` & `groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/transformer.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/transformer_vanilla.py` & `groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/transformer_vanilla.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/utils.py` & `groundingdino-py-0.2.0/groundingdino/models/GroundingDINO/utils.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/models/__init__.py` & `groundingdino-py-0.2.0/groundingdino/models/__init__.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/models/registry.py` & `groundingdino-py-0.2.0/groundingdino/models/registry.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/util/box_ops.py` & `groundingdino-py-0.2.0/groundingdino/util/box_ops.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/util/get_tokenlizer.py` & `groundingdino-py-0.2.0/groundingdino/util/get_tokenlizer.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/util/inference.py` & `groundingdino-py-0.2.0/groundingdino/util/inference.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/util/logger.py` & `groundingdino-py-0.2.0/groundingdino/util/logger.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/util/misc.py` & `groundingdino-py-0.2.0/groundingdino/util/misc.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/util/slconfig.py` & `groundingdino-py-0.2.0/groundingdino/util/slconfig.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/util/slio.py` & `groundingdino-py-0.2.0/groundingdino/util/slio.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/util/time_counter.py` & `groundingdino-py-0.2.0/groundingdino/util/time_counter.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/util/utils.py` & `groundingdino-py-0.2.0/groundingdino/util/utils.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/util/visualizer.py` & `groundingdino-py-0.2.0/groundingdino/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino/util/vl_utils.py` & `groundingdino-py-0.2.0/groundingdino/util/vl_utils.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/groundingdino_py.egg-info/PKG-INFO` & `groundingdino-py-0.2.0/groundingdino_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: groundingdino-py
-Version: 0.1.2
+Version: 0.2.0
 Summary: open-set object detector
-Home-page: https://github.com/IDEA-Research/GroundingDINO
+Home-page: https://github.com/giswqs/GroundingDINO
 Author: International Digital Economy Academy, Shilong Liu
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `groundingdino-py-0.1.2/groundingdino_py.egg-info/SOURCES.txt` & `groundingdino-py-0.2.0/groundingdino_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.2/setup.py` & `groundingdino-py-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,17 +189,17 @@
     with open("LICENSE", "r", encoding="utf-8") as f:
         license = f.read()
 
     write_version_file()
 
     setup(
         name="groundingdino-py",
-        version='0.1.2',
+        version='0.2.0',
         author="International Digital Economy Academy, Shilong Liu",
-        url="https://github.com/IDEA-Research/GroundingDINO",
+        url="https://github.com/giswqs/GroundingDINO",
         description="open-set object detector",
         license=license,
         install_requires=parse_requirements("requirements.txt"),
         packages=find_packages(
             exclude=(
                 "configs",
                 "tests",
```

