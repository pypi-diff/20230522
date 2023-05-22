# Comparing `tmp/groundingdino-py-0.1.0.tar.gz` & `tmp/groundingdino-py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groundingdino-py-0.1.0.tar", last modified: Mon May 22 16:59:22 2023, max compression
+gzip compressed data, was "groundingdino-py-0.1.2.tar", last modified: Mon May 22 17:23:23 2023, max compression
```

## Comparing `groundingdino-py-0.1.0.tar` & `groundingdino-py-0.1.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1000)        0 2023-05-22 16:59:22.913868 groundingdino-py-0.1.0/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)    11354 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/LICENSE
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)      122 2023-05-22 16:26:18.000000 groundingdino-py-0.1.0/MANIFEST.in
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)    13205 2023-05-22 16:59:22.913868 groundingdino-py-0.1.0/PKG-INFO
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)    14882 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/README.md
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1000)        0 2023-05-22 16:59:22.910535 groundingdino-py-0.1.0/groundingdino/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)       21 2023-05-22 16:30:11.000000 groundingdino-py-0.1.0/groundingdino/__init__.py
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1000)        0 2023-05-22 16:59:22.910535 groundingdino-py-0.1.0/groundingdino/config/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     1007 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/config/GroundingDINO_SwinB_cfg.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     1006 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/config/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)        0 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/config/__init__.py
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1000)        0 2023-05-22 16:59:22.910535 groundingdino-py-0.1.0/groundingdino/datasets/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)        0 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/datasets/__init__.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     9711 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/datasets/transforms.py
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1000)        0 2023-05-22 16:59:22.910535 groundingdino-py-0.1.0/groundingdino/models/
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1000)        0 2023-05-22 16:59:22.913868 groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)      823 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1000)        0 2023-05-22 16:59:22.913868 groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/backbone/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)       37 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/backbone/__init__.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     7972 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/backbone/backbone.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     6866 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/backbone/position_encoding.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)    29339 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)    12242 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/bertwarper.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)    11825 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/fuse_modules.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)    16691 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/groundingdino.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)    15482 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/ms_deform_attn.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)    36805 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/transformer.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     4020 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/transformer_vanilla.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)    10087 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/utils.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)      754 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/models/__init__.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     2143 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/models/registry.py
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1000)        0 2023-05-22 16:59:22.913868 groundingdino-py-0.1.0/groundingdino/util/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)       71 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/util/__init__.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     3905 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/util/box_ops.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     1345 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/util/get_tokenlizer.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     8062 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/util/inference.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     3303 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/util/logger.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)    23348 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/util/misc.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)    14380 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/util/slconfig.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     5377 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/util/slio.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     1567 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/util/time_counter.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)    17712 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/util/utils.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)    12047 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/util/visualizer.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     3489 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/groundingdino/util/vl_utils.py
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)       22 2023-05-22 16:59:22.000000 groundingdino-py-0.1.0/groundingdino/version.py
-drwxr-xr-x   0 qiusheng  (1000) qiusheng  (1000)        0 2023-05-22 16:59:22.913868 groundingdino-py-0.1.0/groundingdino_py.egg-info/
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)    13205 2023-05-22 16:59:22.000000 groundingdino-py-0.1.0/groundingdino_py.egg-info/PKG-INFO
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     2041 2023-05-22 16:59:22.000000 groundingdino-py-0.1.0/groundingdino_py.egg-info/SOURCES.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)        1 2023-05-22 16:59:22.000000 groundingdino-py-0.1.0/groundingdino_py.egg-info/dependency_links.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)       99 2023-05-22 16:59:22.000000 groundingdino-py-0.1.0/groundingdino_py.egg-info/requires.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)       14 2023-05-22 16:59:22.000000 groundingdino-py-0.1.0/groundingdino_py.egg-info/top_level.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)       99 2023-05-22 16:22:30.000000 groundingdino-py-0.1.0/requirements.txt
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)      396 2023-05-22 16:59:22.913868 groundingdino-py-0.1.0/setup.cfg
--rw-r--r--   0 qiusheng  (1000) qiusheng  (1000)     7182 2023-05-22 16:59:13.000000 groundingdino-py-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.419133 groundingdino-py-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    28221 2023-05-22 17:23:23.419133 groundingdino-py-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14975 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.399133 groundingdino-py-0.1.2/groundingdino/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.399133 groundingdino-py-0.1.2/groundingdino/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/config/GroundingDINO_SwinB_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/config/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.399133 groundingdino-py-0.1.2/groundingdino/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/datasets/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.403133 groundingdino-py-0.1.2/groundingdino/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.407133 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.411133 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29339 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12242 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/bertwarper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11825 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/fuse_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16691 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/groundingdino.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15482 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/ms_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36805 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/transformer_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.415133 groundingdino-py-0.1.2/groundingdino/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/get_tokenlizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23348 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/slconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/slio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/groundingdino/util/vl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 17:23:23.000000 groundingdino-py-0.1.2/groundingdino/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 17:23:23.419133 groundingdino-py-0.1.2/groundingdino_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28221 2023-05-22 17:23:23.000000 groundingdino-py-0.1.2/groundingdino_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-22 17:23:23.000000 groundingdino-py-0.1.2/groundingdino_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 17:23:23.000000 groundingdino-py-0.1.2/groundingdino_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 17:23:23.000000 groundingdino-py-0.1.2/groundingdino_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 17:23:23.000000 groundingdino-py-0.1.2/groundingdino_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-22 17:23:23.419133 groundingdino-py-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-05-22 17:20:58.000000 groundingdino-py-0.1.2/setup.py
```

### Comparing `groundingdino-py-0.1.0/LICENSE` & `groundingdino-py-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/README.md` & `groundingdino-py-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-# :sauropod: Grounding DINO 
+# :sauropod: Grounding DINO
 
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/zero-shot-object-detection-on-mscoco)](https://paperswithcode.com/sota/zero-shot-object-detection-on-mscoco?p=grounding-dino-marrying-dino-with-grounded) [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/zero-shot-object-detection-on-odinw)](https://paperswithcode.com/sota/zero-shot-object-detection-on-odinw?p=grounding-dino-marrying-dino-with-grounded) \
 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/object-detection-on-coco-minival)](https://paperswithcode.com/sota/object-detection-on-coco-minival?p=grounding-dino-marrying-dino-with-grounded) [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/grounding-dino-marrying-dino-with-grounded/object-detection-on-coco)](https://paperswithcode.com/sota/object-detection-on-coco?p=grounding-dino-marrying-dino-with-grounded)
-
+[![image](https://img.shields.io/pypi/v/groundingdino-py.svg)](https://pypi.python.org/pypi/groundingdino-py)
 
 Official PyTorch implementation of ["Grounding DINO: Marrying DINO with Grounded Pre-Training for Open-Set Object Detection"](https://arxiv.org/abs/2303.05499): the SoTA open-set object detector.
 
 ## :sun_with_face: Helpful Tutorial
 
 - :grapes: [[Read our arXiv Paper](https://arxiv.org/abs/2303.05499)]
-- :apple:  [[Watch our simple introduction video on YouTube](https://youtu.be/wxWDt5UiwY8)]
-- :rose:   &nbsp;[[Try the Colab Demo](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb)]
+- :apple: [[Watch our simple introduction video on YouTube](https://youtu.be/wxWDt5UiwY8)]
+- :rose: &nbsp;[[Try the Colab Demo](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb)]
 - :sunflower: [[Try our Official Huggingface Demo](https://huggingface.co/spaces/ShilongLiu/Grounding_DINO_demo)]
 - :maple_leaf: [[Watch the Step by Step Tutorial about GroundingDINO by Robotflow AI](https://youtu.be/cMa77r3YrDk)]
 - :mushroom: [[GroundingDINO: Automated Dataset Annotation and Evaluation by Robotflow AI](https://youtu.be/C4NqaRBz_Kw)]
 - :hibiscus: [[Accelerate Image Annotation with SAM and GroundingDINO by Robotflow AI](https://youtu.be/oEQYStnF2l8)]
 
-<!-- Grounding DINO Methods | 
-[![arXiv](https://img.shields.io/badge/arXiv-2303.05499-b31b1b.svg)](https://arxiv.org/abs/2303.05499) 
+<!-- Grounding DINO Methods |
+[![arXiv](https://img.shields.io/badge/arXiv-2303.05499-b31b1b.svg)](https://arxiv.org/abs/2303.05499)
 [![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/wxWDt5UiwY8) -->
 
 <!-- Grounding DINO Demos |
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb) -->
 <!-- [![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/cMa77r3YrDk)
 [![HuggingFace space](https://img.shields.io/badge/🤗-HuggingFace%20Space-cyan.svg)](https://huggingface.co/spaces/ShilongLiu/Grounding_DINO_demo)
 [![YouTube](https://badges.aleen42.com/src/youtube.svg)](https://youtu.be/oEQYStnF2l8)
@@ -37,31 +37,26 @@
 - [SEEM: Segment Everything Everywhere All at Once](https://github.com/UX-Decoder/Segment-Everything-Everywhere-All-At-Once)
 - [X-GPT: Conversational Visual Agent supported by X-Decoder](https://github.com/microsoft/X-Decoder/tree/xgpt)
 - [GLIGEN: Open-Set Grounded Text-to-Image Generation](https://github.com/gligen/GLIGEN)
 - [LLaVA: Large Language and Vision Assistant](https://github.com/haotian-liu/LLaVA)
 
 <!-- Extensions | [Grounding DINO with Segment Anything](https://github.com/IDEA-Research/Grounded-Segment-Anything); [Grounding DINO with Stable Diffusion](demo/image_editing_with_groundingdino_stablediffusion.ipynb); [Grounding DINO with GLIGEN](demo/image_editing_with_groundingdino_gligen.ipynb)  -->
 
-
-
 <!-- Official PyTorch implementation of [Grounding DINO](https://arxiv.org/abs/2303.05499), a stronger open-set object detector. Code is available now! -->
 
-
 ## :bulb: Highlight
 
 - **Open-Set Detection.** Detect **everything** with language!
 - **High Performancce.** COCO zero-shot **52.5 AP** (training without COCO data!). COCO fine-tune **63.0 AP**.
 - **Flexible.** Collaboration with Stable Diffusion for Image Editting.
 
-
-
-
 ## :fire: News
+
 - **`2023/04/15`**: Refer to [CV in the Wild Readings](https://github.com/Computer-Vision-in-the-Wild/CVinW_Readings) for those who are interested in open-set recognition!
-- **`2023/04/08`**: We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN)  for more controllable image editings.
+- **`2023/04/08`**: We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN) for more controllable image editings.
 - **`2023/04/08`**: We release [demos](demo/image_editing_with_groundingdino_stablediffusion.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [Stable Diffusion](https://github.com/Stability-AI/StableDiffusion) for image editings.
 - **`2023/04/06`**: We build a new demo by marrying GroundingDINO with [Segment-Anything](https://github.com/facebookresearch/segment-anything) named **[Grounded-Segment-Anything](https://github.com/IDEA-Research/Grounded-Segment-Anything)** aims to support segmentation in GroundingDINO.
 - **`2023/03/28`**: A YouTube [video](https://youtu.be/cMa77r3YrDk) about Grounding DINO and basic object detection prompt engineering. [[SkalskiP](https://github.com/SkalskiP)]
 - **`2023/03/28`**: Add a [demo](https://huggingface.co/spaces/ShilongLiu/Grounding_DINO_demo) on Hugging Face Space!
 - **`2023/03/27`**: Support CPU-only mode. Now the model can run on machines without GPUs.
 - **`2023/03/25`**: A [demo](https://colab.research.google.com/github/roboflow-ai/notebooks/blob/main/notebooks/zero-shot-object-detection-with-grounding-dino.ipynb) for Grounding DINO is available at Colab. [[SkalskiP](https://github.com/SkalskiP)]
 - **`2023/03/22`**: Code is available Now!
@@ -73,32 +68,33 @@
  <a href="https://arxiv.org/abs/2303.05499">Paper</a> introduction.
 <img src=".asset/hero_figure.png" alt="ODinW" width="100%">
 Marrying <a href="https://github.com/IDEA-Research/GroundingDINO">Grounding DINO</a> and <a href="https://github.com/gligen/GLIGEN">GLIGEN</a>
 <img src="https://huggingface.co/ShilongLiu/GroundingDINO/resolve/main/GD_GLIGEN.png" alt="gd_gligen" width="100%">
 </details>
 
 ## :star: Explanations/Tips for Grounding DINO Inputs and Outputs
+
 - Grounding DINO accepts an `(image, text)` pair as inputs.
 - It outputs `900` (by default) object boxes. Each box has similarity scores across all input words. (as shown in Figures below.)
 - We defaultly choose the boxes whose highest similarities are higher than a `box_threshold`.
 - We extract the words whose similarities are higher than the `text_threshold` as predicted labels.
-- If you want to obtain objects of specific phrases, like the `dogs` in the sentence `two dogs with a stick.`, you can select the boxes with highest text similarities with `dogs` as final outputs. 
+- If you want to obtain objects of specific phrases, like the `dogs` in the sentence `two dogs with a stick.`, you can select the boxes with highest text similarities with `dogs` as final outputs.
 - Note that each word can be split to **more than one** tokens with different tokenlizers. The number of words in a sentence may not equal to the number of text tokens.
 - We suggest separating different category names with `.` for Grounding DINO.
-![model_explain1](.asset/model_explan1.PNG)
-![model_explain2](.asset/model_explan2.PNG)
+  ![model_explain1](.asset/model_explan1.PNG)
+  ![model_explain2](.asset/model_explan2.PNG)
 
-## :label: TODO 
+## :label: TODO
 
 - [x] Release inference code and demo.
 - [x] Release checkpoints.
 - [x] Grounding DINO with Stable Diffusion and GLIGEN demos.
 - [ ] Release training codes.
 
-## :hammer_and_wrench: Install 
+## :hammer_and_wrench: Install
 
 **Note:**
 
 If you have a CUDA environment, please make sure the environment variable `CUDA_HOME` is set. It will be compiled under CPU-only mode if no CUDA available.
 
 **Installation:**
 
@@ -115,14 +111,15 @@
 ```
 
 Install the required dependencies in the current directory.
 
 ```bash
 pip3 install -q -e .
 ```
+
 Create a new directory called "weights" to store the model weights.
 
 ```bash
 mkdir weights
 ```
 
 Change the current directory to the "weights" folder.
@@ -134,29 +131,33 @@
 Download the model weights file.
 
 ```bash
 wget -q https://github.com/IDEA-Research/GroundingDINO/releases/download/v0.1.0-alpha/groundingdino_swint_ogc.pth
 ```
 
 ## :arrow_forward: Demo
+
 Check your GPU ID (only if you're using a GPU)
 
 ```bash
 nvidia-smi
 ```
+
 Replace `{GPU ID}`, `image_you_want_to_detect.jpg`, and `"dir you want to save the output"` with appropriate values in the following command
+
 ```bash
 CUDA_VISIBLE_DEVICES={GPU ID} python demo/inference_on_a_image.py \
 -c /GroundingDINO/groundingdino/config/GroundingDINO_SwinT_OGC.py \
 -p /GroundingDINO/weights/groundingdino_swint_ogc.pth \
 -i image_you_want_to_detect.jpg \
 -o "dir you want to save the output" \
 -t "chair"
  [--cpu-only] # open it for cpu mode
 ```
+
 See the `demo/inference_on_a_image.py` for more details.
 
 **Running with Python:**
 
 ```python
 from groundingdino.util.inference import load_model, load_image, predict, annotate
 import cv2
@@ -176,24 +177,24 @@
     box_threshold=BOX_TRESHOLD,
     text_threshold=TEXT_TRESHOLD
 )
 
 annotated_frame = annotate(image_source=image_source, boxes=boxes, logits=logits, phrases=phrases)
 cv2.imwrite("annotated_image.jpg", annotated_frame)
 ```
+
 **Web UI**
 
 We also provide a demo code to integrate Grounding DINO with Gradio Web UI. See the file `demo/gradio_app.py` for more details.
 
 **Notebooks**
 
-- We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN)  for more controllable image editings.
+- We release [demos](demo/image_editing_with_groundingdino_gligen.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [GLIGEN](https://github.com/gligen/GLIGEN) for more controllable image editings.
 - We release [demos](demo/image_editing_with_groundingdino_stablediffusion.ipynb) to combine [Grounding DINO](https://arxiv.org/abs/2303.05499) with [Stable Diffusion](https://github.com/Stability-AI/StableDiffusion) for image editings.
 
-
 ## :luggage: Checkpoints
 
 <!-- insert a table -->
 <table>
   <thead>
     <tr style="text-align: right;">
       <th></th>
@@ -247,48 +248,41 @@
 <summary><font size="4">
 Marrying Grounding DINO with <a href="https://github.com/Stability-AI/StableDiffusion">Stable Diffusion</a> for Image Editing
 </font></summary>
 See our example <a href="https://github.com/IDEA-Research/GroundingDINO/blob/main/demo/image_editing_with_groundingdino_stablediffusion.ipynb">notebook</a> for more details.
 <img src=".asset/GD_SD.png" alt="GD_SD" width="100%">
 </details>
 
-
 <details open>
 <summary><font size="4">
 Marrying Grounding DINO with <a href="https://github.com/gligen/GLIGEN">GLIGEN</a> for more Detailed Image Editing.
 </font></summary>
 See our example <a href="https://github.com/IDEA-Research/GroundingDINO/blob/main/demo/image_editing_with_groundingdino_gligen.ipynb">notebook</a> for more details.
 <img src=".asset/GD_GLIGEN.png" alt="GD_GLIGEN" width="100%">
 </details>
 
 ## :sauropod: Model: Grounding DINO
 
 Includes: a text backbone, an image backbone, a feature enhancer, a language-guided query selection, and a cross-modality decoder.
 
 ![arch](.asset/arch.png)
 
-
 ## :hearts: Acknowledgement
 
 Our model is related to [DINO](https://github.com/IDEA-Research/DINO) and [GLIP](https://github.com/microsoft/GLIP). Thanks for their great work!
 
 We also thank great previous work including DETR, Deformable DETR, SMCA, Conditional DETR, Anchor DETR, Dynamic DETR, DAB-DETR, DN-DETR, etc. More related work are available at [Awesome Detection Transformer](https://github.com/IDEACVR/awesome-detection-transformer). A new toolbox [detrex](https://github.com/IDEA-Research/detrex) is available as well.
 
 Thanks [Stable Diffusion](https://github.com/Stability-AI/StableDiffusion) and [GLIGEN](https://github.com/gligen/GLIGEN) for their awesome models.
 
-
 ## :black_nib: Citation
 
-If you find our work helpful for your research, please consider citing the following BibTeX entry.   
+If you find our work helpful for your research, please consider citing the following BibTeX entry.
 
 ```bibtex
 @article{liu2023grounding,
   title={Grounding dino: Marrying dino with grounded pre-training for open-set object detection},
   author={Liu, Shilong and Zeng, Zhaoyang and Ren, Tianhe and Li, Feng and Zhang, Hao and Yang, Jie and Li, Chunyuan and Yang, Jianwei and Su, Hang and Zhu, Jun and others},
   journal={arXiv preprint arXiv:2303.05499},
   year={2023}
 }
 ```
-
-
-
-
```

### Comparing `groundingdino-py-0.1.0/groundingdino/config/GroundingDINO_SwinB_cfg.py` & `groundingdino-py-0.1.2/groundingdino/config/GroundingDINO_SwinB_cfg.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/config/GroundingDINO_SwinT_OGC.py` & `groundingdino-py-0.1.2/groundingdino/config/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/datasets/transforms.py` & `groundingdino-py-0.1.2/groundingdino/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/__init__.py` & `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/__init__.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/backbone/backbone.py` & `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/backbone/position_encoding.py` & `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/position_encoding.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/backbone/swin_transformer.py` & `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/backbone/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/bertwarper.py` & `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/bertwarper.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/fuse_modules.py` & `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/fuse_modules.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/groundingdino.py` & `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/groundingdino.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/ms_deform_attn.py` & `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/ms_deform_attn.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/transformer.py` & `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/transformer.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/transformer_vanilla.py` & `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/transformer_vanilla.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/models/GroundingDINO/utils.py` & `groundingdino-py-0.1.2/groundingdino/models/GroundingDINO/utils.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/models/__init__.py` & `groundingdino-py-0.1.2/groundingdino/models/__init__.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/models/registry.py` & `groundingdino-py-0.1.2/groundingdino/models/registry.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/util/box_ops.py` & `groundingdino-py-0.1.2/groundingdino/util/box_ops.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/util/get_tokenlizer.py` & `groundingdino-py-0.1.2/groundingdino/util/get_tokenlizer.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/util/inference.py` & `groundingdino-py-0.1.2/groundingdino/util/inference.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/util/logger.py` & `groundingdino-py-0.1.2/groundingdino/util/logger.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/util/misc.py` & `groundingdino-py-0.1.2/groundingdino/util/misc.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/util/slconfig.py` & `groundingdino-py-0.1.2/groundingdino/util/slconfig.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/util/slio.py` & `groundingdino-py-0.1.2/groundingdino/util/slio.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/util/time_counter.py` & `groundingdino-py-0.1.2/groundingdino/util/time_counter.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/util/utils.py` & `groundingdino-py-0.1.2/groundingdino/util/utils.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/util/visualizer.py` & `groundingdino-py-0.1.2/groundingdino/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino/util/vl_utils.py` & `groundingdino-py-0.1.2/groundingdino/util/vl_utils.py`

 * *Files identical despite different names*

### Comparing `groundingdino-py-0.1.0/groundingdino_py.egg-info/SOURCES.txt` & `groundingdino-py-0.1.2/groundingdino_py.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
-/home/qiusheng/Documents/GitHub/GroundingDINO/groundingdino/models/GroundingDINO/csrc/cuda_version.cu
-/home/qiusheng/Documents/GitHub/GroundingDINO/groundingdino/models/GroundingDINO/csrc/vision.cpp
-/home/qiusheng/Documents/GitHub/GroundingDINO/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cpu.cpp
-/home/qiusheng/Documents/GitHub/GroundingDINO/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cuda.cu
 groundingdino/__init__.py
 groundingdino/version.py
 groundingdino/config/GroundingDINO_SwinB_cfg.py
 groundingdino/config/GroundingDINO_SwinT_OGC.py
 groundingdino/config/__init__.py
 groundingdino/datasets/__init__.py
 groundingdino/datasets/transforms.py
```

### Comparing `groundingdino-py-0.1.0/setup.py` & `groundingdino-py-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 from torch.utils.cpp_extension import CUDA_HOME, CppExtension, CUDAExtension
 
 # groundingdino version info
 version = "0.1.0"
 package_name = "groundingdino"
 cwd = os.path.dirname(os.path.abspath(__file__))
 
+with open('README.md') as readme_file:
+    readme = readme_file.read()
 
 sha = "Unknown"
 try:
     sha = subprocess.check_output(["git", "rev-parse", "HEAD"], cwd=cwd).decode("ascii").strip()
 except Exception:
     pass
 
@@ -187,22 +189,24 @@
     with open("LICENSE", "r", encoding="utf-8") as f:
         license = f.read()
 
     write_version_file()
 
     setup(
         name="groundingdino-py",
-        version="0.1.0",
+        version='0.1.2',
         author="International Digital Economy Academy, Shilong Liu",
         url="https://github.com/IDEA-Research/GroundingDINO",
         description="open-set object detector",
         license=license,
         install_requires=parse_requirements("requirements.txt"),
         packages=find_packages(
             exclude=(
                 "configs",
                 "tests",
             )
         ),
         ext_modules=get_extensions(),
         cmdclass={"build_ext": torch.utils.cpp_extension.BuildExtension},
+        long_description=readme,
+        long_description_content_type='text/markdown',
     )
```

