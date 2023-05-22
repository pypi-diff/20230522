# Comparing `tmp/carefree-creator-0.2.5.tar.gz` & `tmp/carefree-creator-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-creator-0.2.5.tar", last modified: Wed May 17 13:25:15 2023, max compression
+gzip compressed data, was "carefree-creator-0.2.6.tar", last modified: Mon May 22 14:47:54 2023, max compression
```

## Comparing `carefree-creator-0.2.5.tar` & `carefree-creator-0.2.6.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 13:25:15.245986 carefree-creator-0.2.5/
--rw-rw-rw-   0        0        0     1090 2022-10-31 07:20:41.000000 carefree-creator-0.2.5/LICENSE
--rw-rw-rw-   0        0        0      195 2023-04-13 07:31:10.000000 carefree-creator-0.2.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4419 2023-05-17 13:25:15.245986 carefree-creator-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     4117 2023-05-06 03:00:57.000000 carefree-creator-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 13:25:15.234023 carefree-creator-0.2.5/carefree_creator.egg-info/
--rw-rw-rw-   0        0        0     4419 2023-05-17 13:25:15.000000 carefree-creator-0.2.5/carefree_creator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      962 2023-05-17 13:25:15.000000 carefree-creator-0.2.5/carefree_creator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 13:25:15.000000 carefree-creator-0.2.5/carefree_creator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-17 13:25:15.000000 carefree-creator-0.2.5/carefree_creator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      139 2023-05-17 13:25:15.000000 carefree-creator-0.2.5/carefree_creator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-17 13:25:15.000000 carefree-creator-0.2.5/carefree_creator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 13:25:15.240006 carefree-creator-0.2.5/cfcreator/
--rw-rw-rw-   0        0        0       96 2023-04-18 08:30:52.000000 carefree-creator-0.2.5/cfcreator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:25:15.241003 carefree-creator-0.2.5/cfcreator/apis/
--rw-rw-rw-   0        0        0      821 2023-04-13 07:31:10.000000 carefree-creator-0.2.5/cfcreator/apis/config.yml
--rw-rw-rw-   0        0        0     9028 2023-05-17 13:02:59.000000 carefree-creator-0.2.5/cfcreator/apis/interface.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:25:15.241999 carefree-creator-0.2.5/cfcreator/apis/kafka/
--rw-rw-rw-   0        0        0      821 2023-04-18 08:30:52.000000 carefree-creator-0.2.5/cfcreator/apis/kafka/config.yml
--rw-rw-rw-   0        0        0    13714 2023-05-17 13:00:21.000000 carefree-creator-0.2.5/cfcreator/apis/kafka/consumer.py
--rw-rw-rw-   0        0        0    12102 2023-05-17 13:02:27.000000 carefree-creator-0.2.5/cfcreator/apis/kafka/producer.py
--rw-rw-rw-   0        0        0     2984 2023-04-23 02:27:17.000000 carefree-creator-0.2.5/cfcreator/cli.py
--rw-rw-rw-   0        0        0    23231 2023-05-17 10:12:51.000000 carefree-creator-0.2.5/cfcreator/common.py
--rw-rw-rw-   0        0        0    16085 2023-05-17 09:12:37.000000 carefree-creator-0.2.5/cfcreator/control.py
--rw-rw-rw-   0        0        0     2226 2023-05-09 07:17:42.000000 carefree-creator-0.2.5/cfcreator/control_multi.py
--rw-rw-rw-   0        0        0     8444 2023-05-17 10:12:51.000000 carefree-creator-0.2.5/cfcreator/cos.py
--rw-rw-rw-   0        0        0     4566 2023-04-18 08:30:52.000000 carefree-creator-0.2.5/cfcreator/cv.py
--rw-rw-rw-   0        0        0     2458 2023-05-17 10:12:51.000000 carefree-creator-0.2.5/cfcreator/endpoints.py
--rw-rw-rw-   0        0        0    20523 2023-05-17 09:12:37.000000 carefree-creator-0.2.5/cfcreator/img2img.py
--rw-rw-rw-   0        0        0     1657 2023-05-17 09:12:37.000000 carefree-creator-0.2.5/cfcreator/img2txt.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:25:15.243993 carefree-creator-0.2.5/cfcreator/legacy/
--rw-rw-rw-   0        0        0        0 2023-05-06 03:00:57.000000 carefree-creator-0.2.5/cfcreator/legacy/__init__.py
--rw-rw-rw-   0        0        0     2102 2023-05-17 10:12:51.000000 carefree-creator-0.2.5/cfcreator/legacy/common.py
--rw-rw-rw-   0        0        0    13724 2023-05-17 10:12:51.000000 carefree-creator-0.2.5/cfcreator/legacy/control.py
--rw-rw-rw-   0        0        0     3216 2023-05-06 03:00:57.000000 carefree-creator-0.2.5/cfcreator/legacy/control_multi.py
--rw-rw-rw-   0        0        0     3298 2023-05-17 10:12:51.000000 carefree-creator-0.2.5/cfcreator/parameters.py
--rw-rw-rw-   0        0        0     3431 2023-05-17 10:12:51.000000 carefree-creator-0.2.5/cfcreator/pipeline.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:25:15.244989 carefree-creator-0.2.5/cfcreator/sdks/
--rw-rw-rw-   0        0        0       45 2023-04-18 08:30:52.000000 carefree-creator-0.2.5/cfcreator/sdks/__init__.py
--rw-rw-rw-   0        0        0      659 2023-04-23 02:27:17.000000 carefree-creator-0.2.5/cfcreator/sdks/direct.py
--rw-rw-rw-   0        0        0     2130 2023-04-23 02:27:17.000000 carefree-creator-0.2.5/cfcreator/sdks/kafka.py
--rw-rw-rw-   0        0        0     1103 2023-04-23 02:27:17.000000 carefree-creator-0.2.5/cfcreator/sdks/utils.py
--rw-rw-rw-   0        0        0     7087 2023-05-17 09:12:37.000000 carefree-creator-0.2.5/cfcreator/txt2img.py
--rw-rw-rw-   0        0        0     2371 2023-04-23 02:27:17.000000 carefree-creator-0.2.5/cfcreator/txt2txt.py
--rw-rw-rw-   0        0        0     5451 2023-05-17 09:12:37.000000 carefree-creator-0.2.5/cfcreator/utils.py
--rw-rw-rw-   0        0        0       42 2023-05-17 13:25:15.245986 carefree-creator-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1015 2023-05-17 13:23:54.000000 carefree-creator-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:47:54.250428 carefree-creator-0.2.6/
+-rw-rw-rw-   0        0        0     1090 2022-10-31 07:20:41.000000 carefree-creator-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0      195 2023-04-13 07:31:10.000000 carefree-creator-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4419 2023-05-22 14:47:54.250428 carefree-creator-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4117 2023-05-22 08:04:35.000000 carefree-creator-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 14:47:54.237466 carefree-creator-0.2.6/carefree_creator.egg-info/
+-rw-rw-rw-   0        0        0     4419 2023-05-22 14:47:54.000000 carefree-creator-0.2.6/carefree_creator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      962 2023-05-22 14:47:54.000000 carefree-creator-0.2.6/carefree_creator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 14:47:54.000000 carefree-creator-0.2.6/carefree_creator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-22 14:47:54.000000 carefree-creator-0.2.6/carefree_creator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      139 2023-05-22 14:47:54.000000 carefree-creator-0.2.6/carefree_creator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-22 14:47:54.000000 carefree-creator-0.2.6/carefree_creator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 14:47:54.244447 carefree-creator-0.2.6/cfcreator/
+-rw-rw-rw-   0        0        0       96 2023-04-18 08:30:52.000000 carefree-creator-0.2.6/cfcreator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:47:54.245444 carefree-creator-0.2.6/cfcreator/apis/
+-rw-rw-rw-   0        0        0      821 2023-04-13 07:31:10.000000 carefree-creator-0.2.6/cfcreator/apis/config.yml
+-rw-rw-rw-   0        0        0     9028 2023-05-22 08:04:35.000000 carefree-creator-0.2.6/cfcreator/apis/interface.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:47:54.247437 carefree-creator-0.2.6/cfcreator/apis/kafka/
+-rw-rw-rw-   0        0        0      821 2023-04-18 08:30:52.000000 carefree-creator-0.2.6/cfcreator/apis/kafka/config.yml
+-rw-rw-rw-   0        0        0    13714 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/apis/kafka/consumer.py
+-rw-rw-rw-   0        0        0    12102 2023-05-22 08:53:07.000000 carefree-creator-0.2.6/cfcreator/apis/kafka/producer.py
+-rw-rw-rw-   0        0        0     2984 2023-04-23 02:27:17.000000 carefree-creator-0.2.6/cfcreator/cli.py
+-rw-rw-rw-   0        0        0    20510 2023-05-22 08:04:35.000000 carefree-creator-0.2.6/cfcreator/common.py
+-rw-rw-rw-   0        0        0    16286 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/control.py
+-rw-rw-rw-   0        0        0     2270 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/control_multi.py
+-rw-rw-rw-   0        0        0     8444 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/cos.py
+-rw-rw-rw-   0        0        0     4566 2023-04-18 08:30:52.000000 carefree-creator-0.2.6/cfcreator/cv.py
+-rw-rw-rw-   0        0        0     2408 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/endpoints.py
+-rw-rw-rw-   0        0        0    20532 2023-05-22 14:06:32.000000 carefree-creator-0.2.6/cfcreator/img2img.py
+-rw-rw-rw-   0        0        0     1657 2023-05-22 08:04:35.000000 carefree-creator-0.2.6/cfcreator/img2txt.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:47:54.248434 carefree-creator-0.2.6/cfcreator/legacy/
+-rw-rw-rw-   0        0        0        0 2023-05-22 08:04:35.000000 carefree-creator-0.2.6/cfcreator/legacy/__init__.py
+-rw-rw-rw-   0        0        0     2169 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/legacy/common.py
+-rw-rw-rw-   0        0        0    13783 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/legacy/control.py
+-rw-rw-rw-   0        0        0     3216 2023-05-22 08:04:35.000000 carefree-creator-0.2.6/cfcreator/legacy/control_multi.py
+-rw-rw-rw-   0        0        0     3271 2023-05-22 08:53:07.000000 carefree-creator-0.2.6/cfcreator/parameters.py
+-rw-rw-rw-   0        0        0     3431 2023-05-22 14:06:42.000000 carefree-creator-0.2.6/cfcreator/pipeline.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:47:54.250428 carefree-creator-0.2.6/cfcreator/sdks/
+-rw-rw-rw-   0        0        0       45 2023-04-18 08:30:52.000000 carefree-creator-0.2.6/cfcreator/sdks/__init__.py
+-rw-rw-rw-   0        0        0      659 2023-04-23 02:27:17.000000 carefree-creator-0.2.6/cfcreator/sdks/direct.py
+-rw-rw-rw-   0        0        0     2130 2023-04-23 02:27:17.000000 carefree-creator-0.2.6/cfcreator/sdks/kafka.py
+-rw-rw-rw-   0        0        0     1103 2023-04-23 02:27:17.000000 carefree-creator-0.2.6/cfcreator/sdks/utils.py
+-rw-rw-rw-   0        0        0     7034 2023-05-22 08:04:35.000000 carefree-creator-0.2.6/cfcreator/txt2img.py
+-rw-rw-rw-   0        0        0     2371 2023-04-23 02:27:17.000000 carefree-creator-0.2.6/cfcreator/txt2txt.py
+-rw-rw-rw-   0        0        0     5715 2023-05-22 11:54:08.000000 carefree-creator-0.2.6/cfcreator/utils.py
+-rw-rw-rw-   0        0        0       42 2023-05-22 14:47:54.251424 carefree-creator-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2023-05-22 14:47:31.000000 carefree-creator-0.2.6/setup.py
```

### Comparing `carefree-creator-0.2.5/LICENSE` & `carefree-creator-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/PKG-INFO` & `carefree-creator-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-creator
-Version: 0.2.5
+Version: 0.2.6
 Summary: An AI-powered creator for everyone.
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: kafka
 License-File: LICENSE
```

### Comparing `carefree-creator-0.2.5/README.md` & `carefree-creator-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/carefree_creator.egg-info/PKG-INFO` & `carefree-creator-0.2.6/carefree_creator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carefree-creator
-Version: 0.2.5
+Version: 0.2.6
 Summary: An AI-powered creator for everyone.
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python carefree-learn PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: kafka
 License-File: LICENSE
```

### Comparing `carefree-creator-0.2.5/carefree_creator.egg-info/SOURCES.txt` & `carefree-creator-0.2.6/carefree_creator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/apis/config.yml` & `carefree-creator-0.2.6/cfcreator/apis/config.yml`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/apis/interface.py` & `carefree-creator-0.2.6/cfcreator/apis/interface.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/apis/kafka/config.yml` & `carefree-creator-0.2.6/cfcreator/apis/kafka/config.yml`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/apis/kafka/consumer.py` & `carefree-creator-0.2.6/cfcreator/apis/kafka/consumer.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/apis/kafka/producer.py` & `carefree-creator-0.2.6/cfcreator/apis/kafka/producer.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/cli.py` & `carefree-creator-0.2.6/cfcreator/cli.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/common.py` & `carefree-creator-0.2.6/cfcreator/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 import os
-import json
-import torch
-import cflearn
 
 import numpy as np
 
 from abc import ABCMeta
 from PIL import Image
 from enum import Enum
 from typing import Any
@@ -20,21 +17,21 @@
 from functools import partial
 from cftool.cv import np_to_bytes
 from cflearn.zoo import DLZoo
 from cflearn.parameters import OPT
 from cfclient.models import TextModel
 from cfclient.models import ImageModel
 from cfclient.models import AlgorithmBase
-from safetensors.torch import load_file
 from cflearn.api.cv import SDVersions
 from cflearn.api.cv import DiffusionAPI
 from cflearn.api.cv import TranslatorAPI
 from cflearn.api.cv import ImageHarmonizationAPI
 from cflearn.api.cv import ControlledDiffusionAPI
-from cflearn.misc.toolkit import _get_file_size
+from cflearn.api.cv.diffusion import InpaintingMode
+from cflearn.api.cv.diffusion import InpaintingSettings
 from cflearn.misc.toolkit import download_model
 from cflearn.models.cv.diffusion import StableDiffusion
 from cflearn.api.cv.third_party.blip import BLIPAPI
 from cflearn.api.cv.third_party.lama import LaMa
 from cflearn.api.cv.third_party.isnet import ISNetAPI
 from cflearn.api.cv.third_party.prompt import PromptEnhanceAPI
 
@@ -44,113 +41,32 @@
 from .utils import APIs
 from .parameters import verbose
 from .parameters import get_focus
 from .parameters import pool_limit
 from .parameters import Focus
 
 
-class ExternalVersions(str, Enum):
-    """
-    Specify external SD weights that need to be loaded.
-    * these weights should be placed under ~/.cache/external/ folder.
-    * file name should be {version}.ckpt
-
-    Example
-    -------
-    class ExternalVersions(str, Enum):
-        MY_FANCY_MODEL = "my_fancy_model"
-
-    then you can place your model at ~/.cache/external/my_fancy_model.ckpt,
-    after which you can specify `my_fancy_model` as the `version` parameter!
-    """
-
-
 class SDInpaintingVersions(str, Enum):
     v1_5 = "v1.5"
 
 
-class ExternalInpaintingVersions(str, Enum):
-    """
-    Specify external SD-inpainting weights that need to be loaded.
-    * these weights should be placed under ~/.cache/external/inpainting/ folder.
-    * file name should be {version}.ckpt
-
-    Example
-    -------
-    class ExternalVersions(str, Enum):
-        MY_FANCY_MODEL = "my_fancy_model"
-
-    then you can place your model at ~/.cache/external/inpainting/my_fancy_model.ckpt,
-    after which you can specify `my_fancy_model` as the `version` parameter!
-    """
-
-
-def merge_enums(*enums: Enum) -> Enum:
-    members: Dict[str, str] = {}
-    for e in enums:
-        for name, member in e.__members__.items():
-            members[name] = member.value
-    return Enum("MergedVersions", members, type=str)
-
-
-MergedVersions = merge_enums(SDVersions, ExternalVersions)
-MergedInpaintingVersions = merge_enums(SDInpaintingVersions, ExternalInpaintingVersions)
 BaseSDTag = "_base_sd"
 
 
 def _base_sd_path() -> str:
     root = os.path.join(OPT.cache_dir, DLZoo.model_dir)
     return download_model("ldm_sd_v1.5", root=root)
 
 
 def _get(init_fn: Callable, init_to_cpu: bool) -> Any:
     if init_to_cpu:
         return init_fn()
     return init_fn("cuda:0", use_half=True)
 
 
-def _load_external(
-    m: ControlledDiffusionAPI,
-    external_enum: Enum,
-    external_folder: str,
-) -> None:
-    print(f"> handling external weights under '{external_folder}'")
-    os.makedirs(external_folder, exist_ok=True)
-    converted_sizes_path = os.path.join(external_folder, "sizes.json")
-    sizes: Dict[str, int]
-    if not os.path.isfile(converted_sizes_path):
-        sizes = {}
-    else:
-        with open(converted_sizes_path, "r") as f:
-            sizes = json.load(f)
-    for version in external_enum:
-        print(f">> handling {version}")
-        converted_path = os.path.join(external_folder, f"{version}_converted.pt")
-        v_size = sizes.get(version)
-        f_size = (
-            None
-            if not os.path.isfile(converted_path)
-            else _get_file_size(converted_path)
-        )
-        if f_size is None or v_size != f_size:
-            if f_size is not None:
-                print(f">> {version} has been converted but size mismatch")
-            print(f">> converting {version}")
-            model_path = os.path.join(external_folder, f"{version}.ckpt")
-            if not os.path.isfile(model_path):
-                st_path = os.path.join(external_folder, f"{version}.safetensors")
-                torch.save(load_file(st_path), model_path)
-            d = cflearn.scripts.sd.convert(model_path, m, load=False)
-            torch.save(d, converted_path)
-            sizes[version] = _get_file_size(converted_path)
-        m.sd_weights.register(version, converted_path)
-    with open(converted_sizes_path, "w") as f:
-        json.dump(sizes, f)
-
-
 def _load_lora(m: ControlledDiffusionAPI, external_folder: str) -> None:
     print("> loading lora")
     num_lora = 0
     lora_folder = os.path.join(external_folder, "lora")
     os.makedirs(lora_folder, exist_ok=True)
     for lora_file in os.listdir(lora_folder):
         try:
@@ -162,78 +78,64 @@
         except:
             print(f">>>> Failed to load!")
             continue
     print(f"> {num_lora} lora loaded")
 
 
 def init_sd(init_to_cpu: bool) -> ControlledDiffusionAPI:
-    version = MergedVersions.v1_5
-    init_fn = partial(ControlledDiffusionAPI.from_sd_version, version)
+    version = SDVersions.v1_5
+    init_fn = partial(ControlledDiffusionAPI.from_sd_version, version, lazy=True)
     m: ControlledDiffusionAPI = _get(init_fn, init_to_cpu)
     focus = get_focus()
     m.sd_weights.limit = pool_limit()
     m.current_sd_version = version
-    targets = []
-    common = Focus.ALL, Focus.SD, Focus.CONTROL, Focus.PIPELINE
-    if focus in common + (Focus.SD_BASE,):
-        targets.append(MergedVersions.v1_5)
-    if focus in common + (Focus.SD_ANIME,):
-        targets.append(MergedVersions.ANIME)
-        targets.append(MergedVersions.DREAMLIKE)
-        targets.append(MergedVersions.ANIME_ANYTHING)
-        targets.append(MergedVersions.ANIME_HYBRID)
-        targets.append(MergedVersions.ANIME_GUOFENG)
-        targets.append(MergedVersions.ANIME_ORANGE)
-    print(f"> preparing sd weights ({', '.join(targets)}) (focus={focus})")
-    m.prepare_sd(targets)
+    print("> registering base sd")
+    m.prepare_sd([version])
     m.sd_weights.register(BaseSDTag, _base_sd_path())
     # when focus is SYNC, `init_sd` is called because we need to expose `control_hint`
     # endpoints. However, `sd` itself will never be used, so we can skip some stuffs
     user_folder = os.path.expanduser("~")
     external_folder = os.path.join(user_folder, ".cache", "external")
     if focus == Focus.SYNC:
         print("> prepare ControlNet Annotators")
         for hint in m.control_defaults:
             m.prepare_annotator(hint)
     else:
-        _load_external(m, ExternalVersions, external_folder)
         print("> prepare ControlNet weights")
         m.prepare_control_defaults()
         print("> prepare ControlNet Annotators")
         m.prepare_annotators()
         print("> warmup ControlNet")
         m.switch_control(*m.available_control_hints)
     # lora stuffs
     _load_lora(m, external_folder)
     # return
     return m
 
 
 def init_sd_inpainting(init_to_cpu: bool) -> ControlledDiffusionAPI:
-    register_sd()
-    sd: ControlledDiffusionAPI = api_pool.get(APIs.SD, no_change=True)
-    init_fn = ControlledDiffusionAPI.from_sd_inpainting
+    init_fn = partial(ControlledDiffusionAPI.from_sd_inpainting, lazy=True)
     api: ControlledDiffusionAPI = _get(init_fn, init_to_cpu)
     # manually maintain sd_weights
     ## original weights
     api.sd_weights.register(BaseSDTag, _base_sd_path())
     ## inpainting weights
     root = os.path.join(OPT.cache_dir, DLZoo.model_dir)
     inpainting_path = download_model("ldm.sd_inpainting", root=root)
-    api.sd_weights.register(MergedInpaintingVersions.v1_5, inpainting_path)
+    api.sd_weights.register(SDInpaintingVersions.v1_5, inpainting_path)
+    api.current_sd_version = SDInpaintingVersions.v1_5
+    # lora stuffs
     user_folder = os.path.expanduser("~")
     external_folder = os.path.join(user_folder, ".cache", "external")
-    external_inpainting_folder = os.path.join(external_folder, "inpainting")
-    _load_external(api, ExternalInpaintingVersions, external_inpainting_folder)
-    # lora stuffs
     _load_lora(api, external_folder)
     # inject properties from sd
+    register_sd()
+    sd: ControlledDiffusionAPI = api_pool.get(APIs.SD, no_change=True)
     api.annotators = sd.annotators
     api.controlnet_weights = sd.controlnet_weights
-    api.current_sd_version = MergedInpaintingVersions.v1_5
     api.switch_control(*api.available_control_hints)
     return api
 
 
 def register_sd() -> None:
     api_pool.register(APIs.SD, init_sd)
 
@@ -419,16 +321,16 @@
         "",
         description="Negative prompt for classifier-free guidance.",
     )
     is_anime: bool = Field(
         False,
         description="Whether should we generate anime images or not.",
     )
-    version: MergedVersions = Field(
-        MergedVersions.v1_5,
+    version: str = Field(
+        SDVersions.v1_5,
         description="Version of the diffusion model",
     )
     sampler: SDSamplers = Field(
         SDSamplers.K_EULER,
         description="Sampler of the diffusion model",
     )
     clip_skip: int = Field(
@@ -463,41 +365,52 @@
 
 
 class CommonSDInpaintingModel(ReturnArraysModel):
     keep_original: bool = Field(
         False,
         description="Whether strictly keep the original image identical in the output image.",
     )
-    ref_mask_smooth: int = Field(
-        3,
-        description="The smoothness of the reference's mask, `0` means no smooth.",
-    )
     use_raw_inpainting: bool = Field(
         False,
         description="""
 Whether use the raw inpainting method.
 > This is useful when you want to apply inpainting with custom SD models.
 """,
     )
-    raw_inpainting_use_ref: bool = Field(
+    use_background_guidance: bool = Field(
         False,
-        description="Whether use input image as reference.",
-    )
-    raw_inpainting_fidelity: float = Field(
-        0.2,
-        ge=0.0,
-        le=1.0,
-        description="The fidelity of the input image when it is used as reference in raw inpainting.",
+        description="""
+Whether inject the latent of the background during the generation.
+> If `use_raw_inpainting`, this will always be `True` because in this case
+the latent of the background is the only information for us to inpaint.
+""",
     )
-    use_latent_guidance: bool = Field(
+    use_reference: bool = Field(
         False,
-        description="Whether use the latent of the givent image to guide the generation.",
+        description="Whether use the original image as reference.",
     )
     reference_fidelity: float = Field(
-        0.0, description="Fidelity of the reference image."
+        0.0,
+        description="Fidelity of the reference image, only take effects when `use_reference` is `True`.",
+    )
+    inpainting_mode: InpaintingMode = Field(
+        InpaintingMode.NORMAL,
+        description="Inpainting mode. MASKED is preferred when the masked area is small.",
+    )
+    inpainting_mask_blur: Optional[int] = Field(
+        None,
+        description="The smoothness of the inpainting's mask, `None` means no smooth.",
+    )
+    inpainting_mask_padding: Optional[int] = Field(
+        32,
+        description="Padding of the inpainting mask under MASKED mode. If `None`, then no padding.",
+    )
+    inpainting_mask_binary_threshold: Optional[int] = Field(
+        32,
+        description="Binary threshold of the inpainting mask under MASKED mode. If `None`, then no thresholding.",
     )
 
 
 class HighresModel(BaseModel):
     fidelity: float = Field(0.3, description="Fidelity of the original latent.")
     upscale_factor: float = Field(2.0, description="Upscale factor.")
     max_wh: int = Field(1024, description="Max width or height of the output image.")
@@ -535,25 +448,30 @@
         0.05,
         ge=0.0,
         le=1.0,
         description="The fidelity of the input image, only take effects when `url` is not `None`.",
     )
     num_samples: int = Field(1, ge=1, le=4, description="Number of samples.")
     bypass_annotator: bool = Field(False, description="Bypass the annotator.")
-    base_model: MergedVersions = Field(
-        MergedVersions.v1_5,
+    base_model: str = Field(
+        SDVersions.v1_5,
         description="The base model.",
     )
     guess_mode: bool = Field(False, description="Guess mode.")
     use_audit: bool = Field(False, description="Whether audit the outputs.")
     no_switch: bool = Field(
         False,
         description="Whether not to switch the ControlNet weights even when the base model has switched.",
     )
     mask_url: Optional[str] = Field(None, description="specify this to do inpainting")
+    use_inpainting: bool = Field(False, description="Whether use inpainting model.")
+
+    @property
+    def version(self) -> str:
+        return self.base_model
 
 
 class ControlNetModel(
     CommonSDInpaintingModel,
     DiffusionModel,
     MaxWHModel,
     _ControlNetModel,
@@ -614,18 +532,24 @@
         clip_skip=clip_skip,
         custom_embeddings=data.custom_embeddings or None,
     )
 
 
 def handle_diffusion_inpainting_model(data: CommonSDInpaintingModel) -> Dict[str, Any]:
     return dict(
-        ref_mask_smooth=data.ref_mask_smooth,
         use_raw_inpainting=data.use_raw_inpainting,
-        raw_inpainting_use_ref=data.raw_inpainting_use_ref,
-        raw_inpainting_fidelity=data.raw_inpainting_fidelity,
+        use_background_guidance=data.use_background_guidance,
+        use_reference=data.use_reference,
+        reference_fidelity=data.reference_fidelity,
+        inpainting_settings=InpaintingSettings(
+            data.inpainting_mode,
+            data.inpainting_mask_blur,
+            data.inpainting_mask_padding,
+            data.inpainting_mask_binary_threshold,
+        ),
     )
 
 
 class GetPromptModel(BaseModel):
     text: str
     need_translate: bool = Field(
         True,
@@ -679,33 +603,38 @@
 
 
 # shortcuts
 
 
 class SDParameters(BaseModel):
     is_anime: bool
-    version: MergedVersions
+    version: str
     lora_paths: Optional[List[str]]
 
 
-def get_sd_from(data: SDParameters) -> ControlledDiffusionAPI:
+def load_sd_lora_with(sd: ControlledDiffusionAPI, data: SDParameters) -> None:
+    if data.lora_paths is not None:
+        for lora_path in data.lora_paths:
+            key = Path(lora_path).stem
+            sd.load_sd_lora(key, path=lora_path)
+
+
+def get_sd_from(api_key: APIs, data: SDParameters, **kw: Any) -> ControlledDiffusionAPI:
     if not data.is_anime:
         version = data.version
     else:
         version = data.version if data.version.startswith("anime") else "anime"
-    sd: ControlledDiffusionAPI = api_pool.get(APIs.SD)
+    sd: ControlledDiffusionAPI = api_pool.get(api_key, **kw)
+    if api_key != APIs.SD_INPAINTING:
+        sd.prepare_sd([version])
+    elif version != SDInpaintingVersions.v1_5:
+        sd.prepare_sd([version], sub_folder="inpainting", force_external=True)
     sd.switch_sd(version)
     sd.disable_control()
-    if data.lora_paths is not None:
-        sd_m = sd.m
-        if not isinstance(sd_m, StableDiffusion):
-            raise ValueError("sd lora only works for StableDiffusion")
-        for lora_path in data.lora_paths:
-            key = Path(lora_path).stem
-            sd.load_sd_lora(key, path=lora_path)
+    load_sd_lora_with(sd, data)
     return sd
 
 
 __all__ = [
     "endpoint2algorithm",
     "DiffusionModel",
     "HighresModel",
```

### Comparing `carefree-creator-0.2.5/cfcreator/control.py` & `carefree-creator-0.2.6/cfcreator/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,23 +19,26 @@
 from cftool.cv import to_rgb
 from cftool.cv import to_uint8
 from cftool.cv import np_to_bytes
 from cftool.cv import restrict_wh
 from cftool.cv import get_suitable_size
 from cfclient.models.core import ImageModel
 from cflearn.api.cv.diffusion import ControlNetHints
-from cflearn.api.cv.diffusion import ControlledDiffusionAPI
+from cflearn.models.cv.diffusion.utils import CONTROL_HINT_KEY
+from cflearn.models.cv.diffusion.utils import CONTROL_HINT_START_KEY
 
 from .utils import api_pool
 from .utils import to_canvas
 from .utils import resize_image
 from .utils import to_contrast_rgb
 from .utils import APIs
 from .common import BaseSDTag
+from .common import get_sd_from
 from .common import register_sd
+from .common import register_sd_inpainting
 from .common import handle_diffusion_model
 from .common import handle_diffusion_inpainting_model
 from .common import IAlgorithm
 from .common import ControlNetModel
 from .common import ReturnArraysModel
 from .common import ControlStrengthModel
 
@@ -73,20 +76,20 @@
 
 def get_hint_url_key(url: str) -> str:
     return f"{url}-hint"
 
 
 async def apply_control(
     self: IAlgorithm,
-    api_key: APIs,
     common: ControlNetModel,
     controls: List[ControlNetBundle],
     normalized_inpainting_mask: Optional[np.ndarray] = None,
 ) -> apply_response:
-    api: ControlledDiffusionAPI = api_pool.get(api_key, no_change=True)
+    api_key = APIs.SD_INPAINTING if common.use_inpainting else APIs.SD
+    api = get_sd_from(api_key, common, no_change=True)
     need_change_device = api_pool.need_change_device(api_key)
     api.enable_control()
     # download images
     urls = set()
     is_hint = {}
     is_global = {}
     if common.url is not None:
@@ -134,15 +137,14 @@
     h = get_suitable_size(h, 64)
     # activate corresponding ControlNet
     t0 = time.time()
     hint_types = sorted(set(bundle.type for bundle in controls))
     if len(hint_types) > api.num_pool:
         msg = f"maximum number of control is {api.num_pool}, but got {len(hint_types)}"
         raise ValueError(msg)
-    api.switch_sd(common.base_model)
     base_md = api.sd_weights.get(BaseSDTag) if common.no_switch else None
     api.switch_control(*hint_types, base_md=base_md)
     t1 = time.time()
     # gather hints
     all_keys: List[TKey] = []
     ## Tensor for input, ndarray for results
     all_key_values: Dict[TKey, Tuple[torch.Tensor, np.ndarray]] = {}
@@ -199,24 +201,25 @@
             else ([i_data.control_strength] * num_scales)
         )
     api.m.control_scales = all_scales
     if not common.prompt:
         raise ValueError("prompt should be provided in `common`")
     cond = [common.prompt] * common.num_samples
     kw = handle_diffusion_model(api, common)
-    kw["hint"] = [(b.type, all_key_values[k][0]) for b, k in zip(controls, all_keys)]
-    kw["hint_start"] = [b.data.hint_start for b in controls]
+    hint = [(b.type, all_key_values[k][0]) for b, k in zip(controls, all_keys)]
+    kw[CONTROL_HINT_KEY] = hint
+    kw[CONTROL_HINT_START_KEY] = [b.data.hint_start for b in controls]
     kw["max_wh"] = common.max_wh
     dt = time.time()
     if need_change_device:
         api.to("cuda:0", use_half=True, no_annotator=True)
     change_diffusion_device_time = time.time() - dt
     # inpainting workaround
     common = common.copy()
-    is_sd_inpainting = api.m.unet_kw["in_channels"] == 9
+    is_sd_inpainting = common.use_inpainting
     common.use_raw_inpainting = not is_sd_inpainting
     if common.mask_url is not None or is_sd_inpainting:
         if common.url is None:
             raise ValueError("`url` should be provided to inpainting")
         if normalized_inpainting_mask is not None:
             inpainting_mask = Image.fromarray(to_uint8(normalized_inpainting_mask))
         else:
@@ -272,29 +275,30 @@
 async def run_single_control(
     self: IAlgorithm,
     data: ControlNetModel,
     hint_type: ControlNetHints,
 ) -> Tuple[List[np.ndarray], Dict[str, float]]:
     self.log_endpoint(data)
     bundle = ControlNetBundle(type=hint_type, data=data)
-    return await apply_control(self, APIs.SD, data, [bundle])
+    return await apply_control(self, data, [bundle])
 
 
 def register_control(
     algorithm_model_class: Type[ControlNetModel],
     algorithm_endpoint: str,
     hint_type: ControlNetHints,
 ) -> None:
     class _(IAlgorithm):
         model_class = algorithm_model_class
 
         endpoint = algorithm_endpoint
 
         def initialize(self) -> None:
             register_sd()
+            register_sd_inpainting()
 
         async def run(self, data: algorithm_model_class, *args: Any) -> Response:
             results, latencies = await run_single_control(self, data, hint_type)
             t0 = time.time()
             content = None if data.return_arrays else np_to_bytes(to_canvas(results))
             t1 = time.time()
             latencies["to_canvas"] = t1 - t0
```

### Comparing `carefree-creator-0.2.5/cfcreator/control_multi.py` & `carefree-creator-0.2.6/cfcreator/control_multi.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from typing import Union
 from fastapi import Response
 from pydantic import Field
 from pydantic import BaseModel
 from cftool.cv import np_to_bytes
 
 from .utils import to_canvas
-from .utils import APIs
 from .common import register_sd
+from .common import register_sd_inpainting
 from .common import IAlgorithm
 from .common import ControlNetModel
 from .control import apply_control
 from .control import ControlNetHints
 from .control import ControlMLSDModel
 from .control import ControlPoseModel
 from .control import ControlCannyModel
@@ -55,18 +55,19 @@
 class ControlMulti(IAlgorithm):
     model_class = ControlMultiModel
 
     endpoint = new_control_multi_endpoint
 
     def initialize(self) -> None:
         register_sd()
+        register_sd_inpainting()
 
     async def run(self, data: ControlMultiModel, *args: Any) -> Response:
         self.log_endpoint(data)
-        results, latencies = await apply_control(self, APIs.SD, data, data.controls)
+        results, latencies = await apply_control(self, data, data.controls)
         t0 = time.time()
         content = None if data.return_arrays else np_to_bytes(to_canvas(results))
         t1 = time.time()
         latencies["to_canvas"] = t1 - t0
         self.log_times(latencies)
         if data.return_arrays:
             return results
```

### Comparing `carefree-creator-0.2.5/cfcreator/cos.py` & `carefree-creator-0.2.6/cfcreator/cos.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/cv.py` & `carefree-creator-0.2.6/cfcreator/cv.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/endpoints.py` & `carefree-creator-0.2.6/cfcreator/endpoints.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,27 +15,25 @@
 
 endpoint_to_focuses = {
     # txt2img
     txt2img_sd_endpoint: [
         Focus.ALL,
         Focus.SD,
         Focus.SD_BASE,
-        Focus.SD_ANIME,
         Focus.CONTROL,
     ],
     txt2img_sd_inpainting_endpoint: [Focus.ALL, Focus.SD],
     txt2img_sd_outpainting_endpoint: [Focus.ALL, Focus.SD],
     # txt2txt
     txt2txt_prompt_enhance_endpoint: [Focus.ALL, Focus.SYNC],
     # img2img
     img2img_sd_endpoint: [
         Focus.ALL,
         Focus.SD,
         Focus.SD_BASE,
-        Focus.SD_ANIME,
         Focus.CONTROL,
     ],
     img2img_semantic2img_endpoint: [Focus.ALL],
     img2img_sr_endpoint: [Focus.ALL, Focus.SYNC],
     img2img_inpainting_endpoint: [Focus.ALL, Focus.SYNC],
     img2img_harmonization_endpoint: [Focus.ALL, Focus.SYNC],
     img2img_sod_endpoint: [Focus.ALL, Focus.SYNC],
```

### Comparing `carefree-creator-0.2.5/cfcreator/img2img.py` & `carefree-creator-0.2.6/cfcreator/img2img.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         t1 = time.time()
         if not data.keep_alpha:
             image = to_rgb(image)
         w, h = data.wh
         if w > 0 and h > 0:
             image = image.resize((w, h), Image.LANCZOS)
         t2 = time.time()
-        m = get_sd_from(data)
+        m = get_sd_from(APIs.SD, data)
         t3 = time.time()
         kwargs.update(handle_diffusion_model(m, data))
         if data.highres_info is not None:
             kwargs["highres_info"] = data.highres_info.dict()
         img_arr = m.img2img(
             image,
             cond=[data.text],
```

### Comparing `carefree-creator-0.2.5/cfcreator/img2txt.py` & `carefree-creator-0.2.6/cfcreator/img2txt.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/legacy/common.py` & `carefree-creator-0.2.6/cfcreator/legacy/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict
 from pydantic import Field
 from pydantic import BaseModel
 from cfclient.models import ImageModel
+from cflearn.api.cv import SDVersions
 
-from ..common import MergedVersions
 from ..common import MaxWHModel
 from ..common import DiffusionModel
 from ..common import ReturnArraysModel
 
 
 class _ControlNetModel(BaseModel):
     hint_url: str = Field(
@@ -28,25 +28,29 @@
         ge=0.0,
         le=1.0,
         description="The fidelity of the input image, only take effects when `use_img2img` is True.",
     )
     use_img2img: bool = Field(True, description="Whether use img2img method.")
     num_samples: int = Field(1, ge=1, le=4, description="Number of samples.")
     bypass_annotator: bool = Field(False, description="Bypass the annotator.")
-    base_model: MergedVersions = Field(
-        MergedVersions.v1_5,
+    base_model: str = Field(
+        SDVersions.v1_5,
         description="The base model.",
     )
     guess_mode: bool = Field(False, description="Guess mode.")
     use_audit: bool = Field(False, description="Whether audit the outputs.")
     no_switch: bool = Field(
         False,
         description="Whether not to switch the ControlNet weights even when the base model has switched.",
     )
 
+    @property
+    def version(self) -> str:
+        return self.base_model
+
 
 # only useful when inpainting model is used
 class _InpaintingMixin(BaseModel):
     use_latent_guidance: bool = Field(
         False,
         description="Whether use the latent of the givent image to guide the generation.",
     )
```

### Comparing `carefree-creator-0.2.5/cfcreator/legacy/control.py` & `carefree-creator-0.2.6/cfcreator/legacy/control.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,24 +19,27 @@
 from cftool.cv import to_rgb
 from cftool.cv import to_uint8
 from cftool.cv import np_to_bytes
 from cftool.cv import restrict_wh
 from cftool.cv import get_suitable_size
 from cfclient.models.core import ImageModel
 from cflearn.api.cv.diffusion import ControlNetHints
-from cflearn.api.cv.diffusion import ControlledDiffusionAPI
+from cflearn.models.cv.diffusion.utils import CONTROL_HINT_KEY
+from cflearn.models.cv.diffusion.utils import CONTROL_HINT_START_KEY
 
 from .common import ControlNetModel
 from ..utils import api_pool
 from ..utils import to_canvas
 from ..utils import resize_image
 from ..utils import APIs
 from ..common import BaseSDTag
+from ..common import get_sd_from
 from ..common import register_sd
 from ..common import handle_diffusion_model
+from ..common import handle_diffusion_inpainting_model
 from ..common import IAlgorithm
 from ..common import ReturnArraysModel
 from ..common import ControlStrengthModel
 
 
 root = os.path.dirname(__file__)
 control_depth_endpoint = "/control/depth"
@@ -65,25 +68,25 @@
     data: Union[ControlNetModelPlaceholder, Dict[str, ControlNetModelPlaceholder]],
     api_key: APIs,
     input_image: np.ndarray,
     hint_image: np.ndarray,
     hint_types: Union[ControlNetHints, List[ControlNetHints]],
     normalized_inpainting_mask: Optional[np.ndarray] = None,
 ) -> apply_response:
-    api: ControlledDiffusionAPI = api_pool.get(api_key, no_change=True)
-    need_change_device = api_pool.need_change_device(api_key)
-    api.enable_control()
     if not isinstance(data, dict):
         common_data = data
         detect_resolution = getattr(data, "detect_resolution", None)
     else:
         common_data = list(data.values())[0]
         detect_resolution = {}
         for hint_type, h_data in data.items():
             detect_resolution[hint_type] = getattr(h_data, "detect_resolution", None)
+    api = get_sd_from(api_key, common_data, no_change=True)
+    need_change_device = api_pool.need_change_device(api_key)
+    api.enable_control()
     original_h, original_w = input_image.shape[:2]
     resize_to_original = lambda array: cv2.resize(
         array,
         (original_w, original_h),
         interpolation=cv2.INTER_CUBIC,
     )
     w, h = restrict_wh(original_w, original_h, common_data.max_wh)
@@ -91,15 +94,14 @@
     h = get_suitable_size(h, 64)
     t0 = time.time()
     if not isinstance(hint_types, list):
         hint_types = [hint_types]
     if len(hint_types) > api.num_pool:
         msg = f"maximum number of control is {api.num_pool}, but got {len(hint_types)}"
         raise ValueError(msg)
-    api.switch_sd(common_data.base_model)
     base_md = api.sd_weights.get(BaseSDTag) if common_data.no_switch else None
     api.switch_control(*hint_types, base_md=base_md)
     t1 = time.time()
     all_hint = {}
     all_o_hint_arrays = []
     all_annotator_change_device_times = []
     for hint_type in sorted(hint_types):
@@ -153,30 +155,29 @@
             ]
             if h_data.guess_mode
             else ([h_data.control_strength] * num_scales)
         )
     cond = [common_data.prompt] * common_data.num_samples
     kw = handle_diffusion_model(api, common_data)
     keys = sorted([k.value if isinstance(k, ControlNetHints) else k for k in all_hint])
-    kw["hint"] = [(k, all_hint[k]) for k in keys]
-    kw["hint_start"] = [common_data.hint_starts.get(k) for k in keys]
+    kw[CONTROL_HINT_KEY] = [(k, all_hint[k]) for k in keys]
+    kw[CONTROL_HINT_START_KEY] = [common_data.hint_starts.get(k) for k in keys]
     kw["max_wh"] = common_data.max_wh
     api.m.control_scales = [all_scales[k] for k in keys]
     dt = time.time()
     if need_change_device:
         api.to("cuda:0", use_half=True, no_annotator=True)
     change_diffusion_device_time = time.time() - dt
     # inpainting workaround
     if api.m.unet_kw["in_channels"] == 9:
         if normalized_inpainting_mask is None:
             raise ValueError("`normalized_input_mask` should be provided to inpainting")
         image = Image.fromarray(input_image)
         inpainting_mask = Image.fromarray(to_uint8(normalized_inpainting_mask))
-        kw["use_latent_guidance"] = common_data.use_latent_guidance
-        kw["reference_fidelity"] = common_data.reference_fidelity
+        kw.update(handle_diffusion_inpainting_model(common_data))
         outs = api.txt2img_inpainting(cond, image, inpainting_mask, **kw)
     elif not common_data.use_img2img:
         kw["size"] = w, h
         outs = api.txt2img(cond, **kw)
     else:
         init_image = cv2.resize(
             input_image,
```

### Comparing `carefree-creator-0.2.5/cfcreator/legacy/control_multi.py` & `carefree-creator-0.2.6/cfcreator/legacy/control_multi.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/parameters.py` & `carefree-creator-0.2.6/cfcreator/parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,14 @@
             os.environ[OPT_ENV_KEY] = self._backup
 
 
 class Focus(str, Enum):
     ALL = "all"
     SD = "sd"
     SD_BASE = "sd.base"
-    SD_ANIME = "sd.anime"
     SD_INPAINTING = "sd.inpainting"
     SYNC = "sync"
     CONTROL = "control"
     PIPELINE = "pipeline"
 
 
 def verbose() -> bool:
```

### Comparing `carefree-creator-0.2.5/cfcreator/pipeline.py` & `carefree-creator-0.2.6/cfcreator/pipeline.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/sdks/direct.py` & `carefree-creator-0.2.6/cfcreator/sdks/direct.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/sdks/kafka.py` & `carefree-creator-0.2.6/cfcreator/sdks/kafka.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/sdks/utils.py` & `carefree-creator-0.2.6/cfcreator/sdks/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/txt2img.py` & `carefree-creator-0.2.6/cfcreator/txt2img.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def initialize(self) -> None:
         register_sd()
 
     async def run(self, data: Txt2ImgSDModel, *args: Any, **kwargs: Any) -> Response:
         self.log_endpoint(data)
         t0 = time.time()
-        m = get_sd_from(data)
+        m = get_sd_from(APIs.SD, data)
         t1 = time.time()
         size = data.w, data.h
         kwargs.update(handle_diffusion_model(m, data))
         if data.highres_info is not None:
             kwargs["highres_info"] = data.highres_info.dict()
         img_arr = m.txt2img(
             data.text,
@@ -124,19 +124,17 @@
         self.log_endpoint(data)
         t0 = time.time()
         image = await self.download_image_with_retry(data.url)
         mask = await self.download_image_with_retry(data.mask_url)
         t1 = time.time()
         if data.use_raw_inpainting:
             api_key = APIs.SD
-            m = get_sd_from(data)
         else:
             api_key = APIs.SD_INPAINTING
-            m = api_pool.get(api_key)
-            m.disable_control()
+        m = get_sd_from(api_key, data)
         t2 = time.time()
         kwargs.update(handle_diffusion_model(m, data))
         kwargs.update(handle_diffusion_inpainting_model(data))
         mask_arr = np.array(mask)
         mask_arr[..., -1] = np.where(mask_arr[..., -1] > 0, 255, 0)
         mask = Image.fromarray(mask_arr)
         img_arr = m.txt2img_inpainting(
@@ -182,15 +180,15 @@
         *args: Any,
         **kwargs: Any,
     ) -> Response:
         self.log_endpoint(data)
         t0 = time.time()
         image = await self.download_image_with_retry(data.url)
         t1 = time.time()
-        m = api_pool.get(APIs.SD_INPAINTING)
+        m = get_sd_from(APIs.SD_INPAINTING, data)
         m.disable_control()
         t2 = time.time()
         kwargs.update(handle_diffusion_model(m, data))
         kwargs.update(handle_diffusion_inpainting_model(data))
         img_arr = m.outpainting(
             data.text,
             image,
```

### Comparing `carefree-creator-0.2.5/cfcreator/txt2txt.py` & `carefree-creator-0.2.6/cfcreator/txt2txt.py`

 * *Files identical despite different names*

### Comparing `carefree-creator-0.2.5/cfcreator/utils.py` & `carefree-creator-0.2.6/cfcreator/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -113,58 +113,63 @@
 
 class LoadableAPI(ILoadableItem[IAPI]):
     def __init__(
         self,
         init_fn: APIInit,
         *,
         init: bool = False,
-        is_sd: bool = False,
+        force_not_lazy: bool = False,
+        has_annotator: bool = False,
     ):
         super().__init__(lambda: init_fn(self.init_to_cpu), init=init)
-        self.is_sd = is_sd
+        self.force_not_lazy = force_not_lazy
+        self.has_annotator = has_annotator
 
     @property
     def lazy(self) -> bool:
-        return lazy_load() and not self.is_sd
+        return lazy_load() and not self.force_not_lazy
 
     @property
     def init_to_cpu(self) -> bool:
         return self.lazy or OPT["cpu"]
 
     @property
     def need_change_device(self) -> bool:
         return self.lazy and not OPT["cpu"]
 
     @property
-    def sd_kwargs(self) -> Dict[str, Any]:
-        return {"no_annotator": True} if self.is_sd else {}
+    def annotator_kwargs(self) -> Dict[str, Any]:
+        return {"no_annotator": True} if self.has_annotator else {}
 
     def load(self, *, no_change: bool = False, **kwargs: Any) -> IAPI:
         super().load()
         if not no_change and self.need_change_device:
-            self._item.to("cuda:0", use_half=True, **self.sd_kwargs)
+            self._item.to("cuda:0", use_half=True, **self.annotator_kwargs)
         return self._item
 
     def cleanup(self) -> None:
         if self.need_change_device:
-            self._item.to("cpu", use_half=False, **self.sd_kwargs)
+            self._item.to("cpu", use_half=False, **self.annotator_kwargs)
             torch.cuda.empty_cache()
 
     def unload(self) -> None:
         self.cleanup()
         return super().unload()
 
 
 class APIPool(ILoadablePool[IAPI]):
     def register(self, key: str, init_fn: APIInit) -> None:
         def _init(init: bool) -> LoadableAPI:
-            is_sd = key in (APIs.SD, APIs.SD_INPAINTING)
-            api = LoadableAPI(init_fn, init=False, is_sd=is_sd)
-            print("> init", key, "(lazy)" if api.lazy else "")
+            kw = dict(
+                force_not_lazy=key in (APIs.SD, APIs.SD_INPAINTING),
+                has_annotator=key in (APIs.SD, APIs.SD_INPAINTING),
+            )
+            api = LoadableAPI(init_fn, init=False, **kw)
             if init:
+                print("> init", key, "(lazy)" if api.lazy else "")
                 api.load(no_change=api.lazy)
             return api
 
         if key in self:
             return
         return super().register(key, _init)
```

### Comparing `carefree-creator-0.2.5/setup.py` & `carefree-creator-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.2.5"
+VERSION = "0.2.6"
 PACKAGE_NAME = "carefree-creator"
 
 DESCRIPTION = "An AI-powered creator for everyone."
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
@@ -13,15 +13,15 @@
     packages=find_packages(exclude=("tests",)),
     include_package_data=True,
     entry_points={"console_scripts": ["cfcreator = cfcreator.cli:main"]},
     install_requires=[
         "click>=8.1.3",
         "fastapi>=0.95.1",
         "carefree-client>=0.1.10",
-        "carefree-learn[cv_full]>=0.4.4",
+        "carefree-learn[cv_full]>=0.4.5",
     ],
     extras_require={
         "kafka": [
             "kafka-python",
             "redis[hiredis]",
             "cos-python-sdk-v5",
         ]
```

