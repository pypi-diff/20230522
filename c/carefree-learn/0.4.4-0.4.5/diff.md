# Comparing `tmp/carefree-learn-0.4.4.tar.gz` & `tmp/carefree-learn-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carefree-learn-0.4.4.tar", last modified: Wed May 17 13:23:16 2023, max compression
+gzip compressed data, was "carefree-learn-0.4.5.tar", last modified: Mon May 22 14:46:50 2023, max compression
```

## Comparing `carefree-learn-0.4.4.tar` & `carefree-learn-0.4.5.tar`

### file list

```diff
@@ -1,361 +1,361 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.885306 carefree-learn-0.4.4/
--rw-rw-rw-   0        0        0     1090 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/LICENSE
--rw-rw-rw-   0        0        0       75 2022-11-10 07:33:05.000000 carefree-learn-0.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0     7575 2023-05-17 13:23:16.885306 carefree-learn-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     7038 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.740221 carefree-learn-0.4.4/carefree_learn.egg-info/
--rw-rw-rw-   0        0        0     7575 2023-05-17 13:23:16.000000 carefree-learn-0.4.4/carefree_learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10736 2023-05-17 13:23:16.000000 carefree-learn-0.4.4/carefree_learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 13:23:16.000000 carefree-learn-0.4.4/carefree_learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      635 2023-05-17 13:23:16.000000 carefree-learn-0.4.4/carefree_learn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-17 13:23:16.000000 carefree-learn-0.4.4/carefree_learn.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.744210 carefree-learn-0.4.4/cflearn/
--rw-rw-rw-   0        0        0      658 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.746203 carefree-learn-0.4.4/cflearn/api/
--rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/api/__init__.py
--rw-rw-rw-   0        0        0    24147 2023-03-27 06:18:09.000000 carefree-learn-0.4.4/cflearn/api/api.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.747200 carefree-learn-0.4.4/cflearn/api/cv/
--rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/api/cv/__init__.py
--rw-rw-rw-   0        0        0    63199 2023-05-16 07:51:40.000000 carefree-learn-0.4.4/cflearn/api/cv/diffusion.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.750190 carefree-learn-0.4.4/cflearn/api/cv/third_party/
--rw-rw-rw-   0        0        0      156 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/__init__.py
--rw-rw-rw-   0        0        0     1069 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/blip.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.751187 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/__init__.py
--rw-rw-rw-   0        0        0     1386 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/api.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.753180 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/inference/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/inference/__init__.py
--rw-rw-rw-   0        0        0     1989 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/inference/predictor.py
--rw-rw-rw-   0        0        0     4395 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/inference/transforms.py
--rw-rw-rw-   0        0        0      341 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/inference/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.754177 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/mconfigs/
--rw-rw-rw-   0        0        0      112 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/mconfigs/__init__.py
--rw-rw-rw-   0        0        0     1660 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py
--rw-rw-rw-   0        0        0     1953 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/mconfigs/base.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.756170 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.758164 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/
--rw-rw-rw-   0        0        0       70 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/__init__.py
--rw-rw-rw-   0        0        0     4553 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py
--rw-rw-rw-   0        0        0     6090 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py
--rw-rw-rw-   0        0        0     3629 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.760156 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/
--rw-rw-rw-   0        0        0      130 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/dih_model.py
--rw-rw-rw-   0        0        0     1353 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py
--rw-rw-rw-   0        0        0     3162 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.765140 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/__init__.py
--rw-rw-rw-   0        0        0     8010 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py
--rw-rw-rw-   0        0        0     5571 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py
--rw-rw-rw-   0        0        0     7150 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py
--rw-rw-rw-   0        0        0    19814 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py
--rw-rw-rw-   0        0        0     6392 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py
--rw-rw-rw-   0        0        0     1808 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py
--rw-rw-rw-   0        0        0    13493 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py
--rw-rw-rw-   0        0        0     8229 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/unet.py
--rw-rw-rw-   0        0        0      357 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modifiers.py
--rw-rw-rw-   0        0        0     4927 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/ops.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.766137 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/utils/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/utils/__init__.py
--rw-rw-rw-   0        0        0      445 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/utils/misc.py
--rw-rw-rw-   0        0        0    16017 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/isnet.py
--rw-rw-rw-   0        0        0     9132 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/lama.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.767134 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/__init__.py
--rw-rw-rw-   0        0        0     8006 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/api.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.772117 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/__init__.py
--rw-rw-rw-   0        0        0      383 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/base_model.py
--rw-rw-rw-   0        0        0    10222 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/blocks.py
--rw-rw-rw-   0        0        0     3259 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/dpt_depth.py
--rw-rw-rw-   0        0        0     2803 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/midas_net.py
--rw-rw-rw-   0        0        0     6071 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/midas_net_custom.py
--rw-rw-rw-   0        0        0     8096 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/transforms.py
--rw-rw-rw-   0        0        0    15154 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/vit.py
--rw-rw-rw-   0        0        0     4814 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.773113 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/__init__.py
--rw-rw-rw-   0        0        0     2106 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/api.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.775107 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/models/
--rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/models/__init__.py
--rw-rw-rw-   0        0        0    10142 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py
--rw-rw-rw-   0        0        0     9711 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py
--rw-rw-rw-   0        0        0    26167 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.778097 carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/
--rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/__init__.py
--rw-rw-rw-   0        0        0     2392 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/api.py
--rw-rw-rw-   0        0        0    14093 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/body.py
--rw-rw-rw-   0        0        0     4271 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/hand.py
--rw-rw-rw-   0        0        0     9090 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/model.py
--rw-rw-rw-   0        0        0     8699 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/util.py
--rw-rw-rw-   0        0        0     2053 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/api/cv/third_party/prompt.py
--rw-rw-rw-   0        0        0     2489 2023-03-23 09:35:16.000000 carefree-learn-0.4.4/cflearn/api/cv/translator.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.779094 carefree-learn-0.4.4/cflearn/api/ml/
--rw-rw-rw-   0        0        0       20 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/api/ml/__init__.py
--rw-rw-rw-   0        0        0     8678 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/api/ml/ddr.py
--rw-rw-rw-   0        0        0      524 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/api/schema.py
--rw-rw-rw-   0        0        0     2983 2023-05-17 13:13:35.000000 carefree-learn-0.4.4/cflearn/api/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.780090 carefree-learn-0.4.4/cflearn/api/zoo/
--rw-rw-rw-   0        0        0     6163 2023-03-29 08:24:36.000000 carefree-learn-0.4.4/cflearn/api/zoo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.782084 carefree-learn-0.4.4/cflearn/callbacks/
--rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1118 2023-03-23 09:35:20.000000 carefree-learn-0.4.4/cflearn/callbacks/classification.py
--rw-rw-rw-   0        0        0     9649 2023-03-23 08:40:04.000000 carefree-learn-0.4.4/cflearn/callbacks/general.py
--rw-rw-rw-   0        0        0     4212 2023-03-23 09:35:26.000000 carefree-learn-0.4.4/cflearn/callbacks/generator.py
--rw-rw-rw-   0        0        0      656 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.783080 carefree-learn-0.4.4/cflearn/data/
--rw-rw-rw-   0        0        0      247 2023-03-28 06:24:25.000000 carefree-learn-0.4.4/cflearn/data/__init__.py
--rw-rw-rw-   0        0        0     2798 2023-03-28 02:09:34.000000 carefree-learn-0.4.4/cflearn/data/array.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.784077 carefree-learn-0.4.4/cflearn/data/blocks/
--rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/blocks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.787067 carefree-learn-0.4.4/cflearn/data/blocks/cv/
--rw-rw-rw-   0        0        0      159 2023-03-29 09:56:34.000000 carefree-learn-0.4.4/cflearn/data/blocks/cv/__init__.py
--rw-rw-rw-   0        0        0     1447 2023-03-29 10:00:43.000000 carefree-learn-0.4.4/cflearn/data/blocks/cv/crop.py
--rw-rw-rw-   0        0        0      477 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/blocks/cv/hwc_to_chw.py
--rw-rw-rw-   0        0        0    31082 2023-03-29 07:34:59.000000 carefree-learn-0.4.4/cflearn/data/blocks/cv/image_folder.py
--rw-rw-rw-   0        0        0     2054 2023-03-29 07:34:59.000000 carefree-learn-0.4.4/cflearn/data/blocks/cv/normalize.py
--rw-rw-rw-   0        0        0     1002 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/blocks/cv/to_numpy.py
--rw-rw-rw-   0        0        0      609 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/blocks/cv/tuple_to_batch.py
--rw-rw-rw-   0        0        0      375 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/blocks/flatten.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.791054 carefree-learn-0.4.4/cflearn/data/blocks/ml/
--rw-rw-rw-   0        0        0      176 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/__init__.py
--rw-rw-rw-   0        0        0    19260 2023-03-29 06:28:32.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/file.py
--rw-rw-rw-   0        0        0     1729 2023-03-29 06:29:22.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/gather.py
--rw-rw-rw-   0        0        0     7608 2023-03-29 06:29:31.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/nan_handler.py
--rw-rw-rw-   0        0        0     7327 2023-03-29 06:29:45.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/preprocessor.py
--rw-rw-rw-   0        0        0     6234 2023-03-29 06:30:03.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/recognizer.py
--rw-rw-rw-   0        0        0      416 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/schema.py
--rw-rw-rw-   0        0        0    12175 2023-03-29 06:30:47.000000 carefree-learn-0.4.4/cflearn/data/blocks/ml/splitter.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.792050 carefree-learn-0.4.4/cflearn/data/ml/
--rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/ml/__init__.py
--rw-rw-rw-   0        0        0     7741 2023-03-29 06:34:52.000000 carefree-learn-0.4.4/cflearn/data/ml/api.py
--rw-rw-rw-   0        0        0     1292 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/ml/datasets.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.793047 carefree-learn-0.4.4/cflearn/data/pytorch/
--rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/data/pytorch/__init__.py
--rw-rw-rw-   0        0        0     8349 2023-03-27 12:47:27.000000 carefree-learn-0.4.4/cflearn/data/pytorch/api.py
--rw-rw-rw-   0        0        0     1406 2023-03-29 06:36:58.000000 carefree-learn-0.4.4/cflearn/data/pytorch/datasets.py
--rw-rw-rw-   0        0        0     7842 2023-03-28 02:09:41.000000 carefree-learn-0.4.4/cflearn/data/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.794044 carefree-learn-0.4.4/cflearn/dist/
--rw-rw-rw-   0        0        0       18 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/dist/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.795040 carefree-learn-0.4.4/cflearn/dist/ml/
--rw-rw-rw-   0        0        0      159 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/dist/ml/__init__.py
--rw-rw-rw-   0        0        0     8874 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/dist/ml/experiment.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.797034 carefree-learn-0.4.4/cflearn/dist/ml/runs/
--rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/dist/ml/runs/__init__.py
--rw-rw-rw-   0        0        0     1320 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/dist/ml/runs/_utils.py
--rw-rw-rw-   0        0        0      291 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/dist/ml/runs/basic.py
--rw-rw-rw-   0        0        0     1709 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/dist/ml/task.py
--rw-rw-rw-   0        0        0     8910 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/inference.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.799027 carefree-learn-0.4.4/cflearn/losses/
--rw-rw-rw-   0        0        0       84 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/losses/__init__.py
--rw-rw-rw-   0        0        0     6391 2023-03-29 12:15:03.000000 carefree-learn-0.4.4/cflearn/losses/basic.py
--rw-rw-rw-   0        0        0     2546 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/losses/gan.py
--rw-rw-rw-   0        0        0     2812 2023-03-24 02:18:57.000000 carefree-learn-0.4.4/cflearn/losses/lpips.py
--rw-rw-rw-   0        0        0     3962 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/losses/vae.py
--rw-rw-rw-   0        0        0     5614 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.801020 carefree-learn-0.4.4/cflearn/misc/
--rw-rw-rw-   0        0        0        0 2023-02-14 02:22:11.000000 carefree-learn-0.4.4/cflearn/misc/__init__.py
--rw-rw-rw-   0        0        0    14696 2023-04-20 10:57:14.000000 carefree-learn-0.4.4/cflearn/misc/available.json
--rw-rw-rw-   0        0        0     1375 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/misc/mixins.py
--rw-rw-rw-   0        0        0    44325 2023-05-16 10:13:20.000000 carefree-learn-0.4.4/cflearn/misc/toolkit.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.802017 carefree-learn-0.4.4/cflearn/models/
--rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/__init__.py
--rw-rw-rw-   0        0        0     5563 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/bases.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.803013 carefree-learn-0.4.4/cflearn/models/cv/
--rw-rw-rw-   0        0        0      167 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.805007 carefree-learn-0.4.4/cflearn/models/cv/ae/
--rw-rw-rw-   0        0        0       38 2023-03-22 05:28:24.000000 carefree-learn-0.4.4/cflearn/models/cv/ae/__init__.py
--rw-rw-rw-   0        0        0    12091 2023-03-27 01:50:04.000000 carefree-learn-0.4.4/cflearn/models/cv/ae/common.py
--rw-rw-rw-   0        0        0     8409 2023-03-27 01:52:38.000000 carefree-learn-0.4.4/cflearn/models/cv/ae/kl.py
--rw-rw-rw-   0        0        0     7970 2023-03-27 01:52:49.000000 carefree-learn-0.4.4/cflearn/models/cv/ae/vq.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.806003 carefree-learn-0.4.4/cflearn/models/cv/classifier/
--rw-rw-rw-   0        0        0       24 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/classifier/__init__.py
--rw-rw-rw-   0        0        0     4079 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/classifier/vanilla.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.808993 carefree-learn-0.4.4/cflearn/models/cv/decoder/
--rw-rw-rw-   0        0        0      145 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/decoder/__init__.py
--rw-rw-rw-   0        0        0     3619 2023-02-27 01:58:50.000000 carefree-learn-0.4.4/cflearn/models/cv/decoder/attn.py
--rw-rw-rw-   0        0        0     4162 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/decoder/schema.py
--rw-rw-rw-   0        0        0     8739 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/decoder/style_gan.py
--rw-rw-rw-   0        0        0    14508 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/decoder/style_gan_v2.py
--rw-rw-rw-   0        0        0     9329 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/decoder/vanilla.py
--rw-rw-rw-   0        0        0     3952 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/decoder/vqgan.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.811983 carefree-learn-0.4.4/cflearn/models/cv/diffusion/
--rw-rw-rw-   0        0        0       87 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.813977 carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/
--rw-rw-rw-   0        0        0       69 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/__init__.py
--rw-rw-rw-   0        0        0    10010 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/clip.py
--rw-rw-rw-   0        0        0     1525 2023-03-24 02:19:09.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/rescaler.py
--rw-rw-rw-   0        0        0     1182 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/schema.py
--rw-rw-rw-   0        0        0    28538 2023-05-06 05:26:10.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/ddpm.py
--rw-rw-rw-   0        0        0    10675 2023-05-16 07:51:34.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/ldm.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.818960 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/
--rw-rw-rw-   0        0        0      137 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/__init__.py
--rw-rw-rw-   0        0        0     2258 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/basic.py
--rw-rw-rw-   0        0        0     9817 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/ddim.py
--rw-rw-rw-   0        0        0    13157 2023-04-20 02:12:01.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/k_samplers.py
--rw-rw-rw-   0        0        0     2593 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/plms.py
--rw-rw-rw-   0        0        0     7804 2023-05-04 11:20:31.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/schema.py
--rw-rw-rw-   0        0        0    16613 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/solver.py
--rw-rw-rw-   0        0        0     2561 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/utils.py
--rw-rw-rw-   0        0        0    20269 2023-04-20 03:26:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/unet.py
--rw-rw-rw-   0        0        0      737 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/diffusion/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.823943 carefree-learn-0.4.4/cflearn/models/cv/encoder/
--rw-rw-rw-   0        0        0      240 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/__init__.py
--rw-rw-rw-   0        0        0     3369 2023-02-27 01:58:50.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/attn.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.824941 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/
--rw-rw-rw-   0        0        0       64 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/api.py
--rw-rw-rw-   0        0        0     4242 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/core.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.827930 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/
--rw-rw-rw-   0        0        0       97 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/__init__.py
--rw-rw-rw-   0        0        0      430 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/mobilenet.py
--rw-rw-rw-   0        0        0     1225 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/resnet.py
--rw-rw-rw-   0        0        0     5392 2023-02-10 05:26:29.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/transformer.py
--rw-rw-rw-   0        0        0    13725 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/vgg.py
--rw-rw-rw-   0        0        0      968 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/register.py
--rw-rw-rw-   0        0        0     1133 2023-02-10 03:39:20.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/fnet.py
--rw-rw-rw-   0        0        0     1132 2023-02-10 03:39:20.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/mixer.py
--rw-rw-rw-   0        0        0     2336 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/perceiver.py
--rw-rw-rw-   0        0        0     1149 2023-02-10 03:39:20.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/pool_former.py
--rw-rw-rw-   0        0        0     5124 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/schema.py
--rw-rw-rw-   0        0        0     6125 2023-03-22 07:19:34.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/transformer.py
--rw-rw-rw-   0        0        0     5535 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/vanilla.py
--rw-rw-rw-   0        0        0     5473 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/models/cv/encoder/vqgan.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.830921 carefree-learn-0.4.4/cflearn/models/cv/gan/
--rw-rw-rw-   0        0        0       55 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/gan/__init__.py
--rw-rw-rw-   0        0        0     5920 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/cv/gan/discriminators.py
--rw-rw-rw-   0        0        0     7730 2023-03-29 11:05:45.000000 carefree-learn-0.4.4/cflearn/models/cv/gan/schema.py
--rw-rw-rw-   0        0        0     1913 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/gan/vanilla.py
--rw-rw-rw-   0        0        0     6731 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/general.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.831918 carefree-learn-0.4.4/cflearn/models/cv/translator/
--rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/cv/translator/__init__.py
--rw-rw-rw-   0        0        0     4018 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/cv/translator/rrdb.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.833911 carefree-learn-0.4.4/cflearn/models/implicit/
--rw-rw-rw-   0        0        0       22 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/implicit/__init__.py
--rw-rw-rw-   0        0        0     7927 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/models/implicit/siren.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.839890 carefree-learn-0.4.4/cflearn/models/ml/
--rw-rw-rw-   0        0        0      165 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/__init__.py
--rw-rw-rw-   0        0        0     1857 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/base.py
--rw-rw-rw-   0        0        0    11624 2023-03-29 12:15:02.000000 carefree-learn-0.4.4/cflearn/models/ml/ddr.py
--rw-rw-rw-   0        0        0     8958 2023-03-28 02:09:49.000000 carefree-learn-0.4.4/cflearn/models/ml/encoders.py
--rw-rw-rw-   0        0        0     2392 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/fcnn.py
--rw-rw-rw-   0        0        0     1100 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/linear.py
--rw-rw-rw-   0        0        0     6980 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/mixed_stacked.py
--rw-rw-rw-   0        0        0     7976 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/nbm.py
--rw-rw-rw-   0        0        0     5272 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/ndt.py
--rw-rw-rw-   0        0        0     3068 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/rnn.py
--rw-rw-rw-   0        0        0     2798 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/ml/wnd.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.841884 carefree-learn-0.4.4/cflearn/models/multimodal/
--rw-rw-rw-   0        0        0       21 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/multimodal/__init__.py
--rw-rw-rw-   0        0        0    10260 2023-03-23 08:58:17.000000 carefree-learn-0.4.4/cflearn/models/multimodal/clip.py
--rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/multimodal/constants.py
--rw-rw-rw-   0        0        0     1554 2023-03-29 11:05:45.000000 carefree-learn-0.4.4/cflearn/models/multimodal/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.841884 carefree-learn-0.4.4/cflearn/models/nlp/
--rw-rw-rw-   0        0        0       80 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.843877 carefree-learn-0.4.4/cflearn/models/nlp/encoder/
--rw-rw-rw-   0        0        0       28 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/encoder/__init__.py
--rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/encoder/constants.py
--rw-rw-rw-   0        0        0     3694 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/encoder/transformer.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.846868 carefree-learn-0.4.4/cflearn/models/nlp/tokenizers/
--rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/tokenizers/__init__.py
--rw-rw-rw-   0        0        0     2371 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/nlp/tokenizers/clip.py
--rw-rw-rw-   0        0        0     1226 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/tokenizers/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.849857 carefree-learn-0.4.4/cflearn/models/nlp/transformers/
--rw-rw-rw-   0        0        0       66 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/transformers/__init__.py
--rw-rw-rw-   0        0        0     3547 2023-03-27 13:58:44.000000 carefree-learn-0.4.4/cflearn/models/nlp/transformers/core.py
--rw-rw-rw-   0        0        0     1575 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/transformers/opus.py
--rw-rw-rw-   0        0        0      813 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/models/nlp/transformers/simbert.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.850855 carefree-learn-0.4.4/cflearn/models/schemas/
--rw-rw-rw-   0        0        0       42 2023-03-27 01:49:17.000000 carefree-learn-0.4.4/cflearn/models/schemas/__init__.py
--rw-rw-rw-   0        0        0    12838 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/models/schemas/custom.py
--rw-rw-rw-   0        0        0     4631 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/models/schemas/cv.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.852847 carefree-learn-0.4.4/cflearn/modules/
--rw-rw-rw-   0        0        0       54 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/modules/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.858828 carefree-learn-0.4.4/cflearn/modules/blocks/
--rw-rw-rw-   0        0        0      756 2023-03-24 08:39:05.000000 carefree-learn-0.4.4/cflearn/modules/blocks/__init__.py
--rw-rw-rw-   0        0        0     5165 2023-03-24 02:18:16.000000 carefree-learn-0.4.4/cflearn/modules/blocks/activations.py
--rw-rw-rw-   0        0        0    21356 2023-05-08 11:16:44.000000 carefree-learn-0.4.4/cflearn/modules/blocks/attentions.py
--rw-rw-rw-   0        0        0     6448 2022-11-09 12:05:57.000000 carefree-learn-0.4.4/cflearn/modules/blocks/common.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.860821 carefree-learn-0.4.4/cflearn/modules/blocks/convs/
--rw-rw-rw-   0        0        0       47 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/modules/blocks/convs/__init__.py
--rw-rw-rw-   0        0        0    19321 2023-03-24 02:29:08.000000 carefree-learn-0.4.4/cflearn/modules/blocks/convs/basic.py
--rw-rw-rw-   0        0        0     8836 2023-03-24 02:19:26.000000 carefree-learn-0.4.4/cflearn/modules/blocks/convs/residual.py
--rw-rw-rw-   0        0        0    18802 2023-04-12 11:14:59.000000 carefree-learn-0.4.4/cflearn/modules/blocks/customs.py
--rw-rw-rw-   0        0        0     8503 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/modules/blocks/high_level.py
--rw-rw-rw-   0        0        0    15078 2023-05-16 07:51:00.000000 carefree-learn-0.4.4/cflearn/modules/blocks/hijacks.py
--rw-rw-rw-   0        0        0     1304 2023-04-12 13:32:32.000000 carefree-learn-0.4.4/cflearn/modules/blocks/hooks.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.861817 carefree-learn-0.4.4/cflearn/modules/blocks/implementations/
--rw-rw-rw-   0        0        0       26 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/modules/blocks/implementations/__init__.py
--rw-rw-rw-   0        0        0     4708 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/modules/blocks/implementations/perceiver.py
--rw-rw-rw-   0        0        0     6189 2023-01-29 11:37:21.000000 carefree-learn-0.4.4/cflearn/modules/blocks/mappings.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.865804 carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/
--rw-rw-rw-   0        0        0      127 2023-02-10 03:31:37.000000 carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/__init__.py
--rw-rw-rw-   0        0        0    28432 2023-04-12 08:04:35.000000 carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/api.py
--rw-rw-rw-   0        0        0     3774 2023-03-24 08:39:41.000000 carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/channel_mixers.py
--rw-rw-rw-   0        0        0     1179 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/poolers.py
--rw-rw-rw-   0        0        0     1325 2023-02-10 05:18:20.000000 carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/schema.py
--rw-rw-rw-   0        0        0     6998 2023-02-10 10:31:50.000000 carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/token_mixers.py
--rw-rw-rw-   0        0        0     4682 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/modules/blocks/norms.py
--rw-rw-rw-   0        0        0      863 2023-02-27 01:58:50.000000 carefree-learn-0.4.4/cflearn/modules/blocks/utils.py
--rw-rw-rw-   0        0        0     4751 2022-10-23 14:55:07.000000 carefree-learn-0.4.4/cflearn/modules/optimizers.py
--rw-rw-rw-   0        0        0     9159 2022-11-09 12:09:28.000000 carefree-learn-0.4.4/cflearn/modules/schedulers.py
--rw-rw-rw-   0        0        0     4774 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/monitors.py
--rw-rw-rw-   0        0        0      634 2023-02-16 10:09:59.000000 carefree-learn-0.4.4/cflearn/parameters.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.868794 carefree-learn-0.4.4/cflearn/pipeline/
--rw-rw-rw-   0        0        0       92 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/pipeline/__init__.py
--rw-rw-rw-   0        0        0    23551 2023-03-29 11:32:53.000000 carefree-learn-0.4.4/cflearn/pipeline/api.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.870787 carefree-learn-0.4.4/cflearn/pipeline/blocks/
--rw-rw-rw-   0        0        0       41 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/pipeline/blocks/__init__.py
--rw-rw-rw-   0        0        0    36043 2023-03-27 01:51:03.000000 carefree-learn-0.4.4/cflearn/pipeline/blocks/basic.py
--rw-rw-rw-   0        0        0     2735 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/pipeline/blocks/ml.py
--rw-rw-rw-   0        0        0     1335 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/pipeline/blocks/utils.py
--rw-rw-rw-   0        0        0     3921 2023-03-23 08:46:39.000000 carefree-learn-0.4.4/cflearn/pipeline/core.py
--rw-rw-rw-   0        0        0      310 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/pipeline/schema.py
--rw-rw-rw-   0        0        0     1545 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/pipeline/third_party.py
--rw-rw-rw-   0        0        0      510 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/register.py
--rw-rw-rw-   0        0        0    60784 2023-03-29 15:41:28.000000 carefree-learn-0.4.4/cflearn/schema.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.871784 carefree-learn-0.4.4/cflearn/scripts/
--rw-rw-rw-   0        0        0       18 2023-03-24 10:59:16.000000 carefree-learn-0.4.4/cflearn/scripts/__init__.py
--rw-rw-rw-   0        0        0    12752 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/scripts/sd.py
--rw-rw-rw-   0        0        0    28526 2023-04-04 02:24:07.000000 carefree-learn-0.4.4/cflearn/trainer.py
--rw-rw-rw-   0        0        0     1053 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/types.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.872780 carefree-learn-0.4.4/cflearn/zoo/
--rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.718078 carefree-learn-0.4.4/cflearn/zoo/configs/
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.717081 carefree-learn-0.4.4/cflearn/zoo/configs/ae/
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.873777 carefree-learn-0.4.4/cflearn/zoo/configs/ae/kl/
--rw-rw-rw-   0        0        0      201 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/ae/kl/f16.json
--rw-rw-rw-   0        0        0      868 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/zoo/configs/ae/kl/f4.json
--rw-rw-rw-   0        0        0      160 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/ae/kl/f8.json
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.875331 carefree-learn-0.4.4/cflearn/zoo/configs/ae/vq/
--rw-rw-rw-   0        0        0      205 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/ae/vq/f4.json
--rw-rw-rw-   0        0        0       92 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/ae/vq/f4_no_attn.json
--rw-rw-rw-   0        0        0      295 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/ae/vq/f8.json
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.718078 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.876333 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ddpm/
--rw-rw-rw-   0        0        0     1155 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ddpm/default.json
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.879325 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/
--rw-rw-rw-   0        0        0      513 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/default.json
--rw-rw-rw-   0        0        0      451 2023-05-08 10:29:54.000000 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/sd.json
--rw-rw-rw-   0        0        0      125 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/sd_inpainting.json
--rw-rw-rw-   0        0        0      344 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/sd_v2.json
--rw-rw-rw-   0        0        0      104 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/sd_v2_base.json
--rw-rw-rw-   0        0        0      600 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/vq.json
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.718078 carefree-learn-0.4.4/cflearn/zoo/configs/multimodal/
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.882316 carefree-learn-0.4.4/cflearn/zoo/configs/multimodal/clip/
--rw-rw-rw-   0        0        0      525 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/multimodal/clip/chinese.json
--rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/zoo/configs/multimodal/clip/default.json
--rw-rw-rw-   0        0        0      269 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/multimodal/clip/large.json
--rw-rw-rw-   0        0        0      389 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/multimodal/clip/open_clip_ViT_H_14.json
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.718078 carefree-learn-0.4.4/cflearn/zoo/configs/sr/
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.883312 carefree-learn-0.4.4/cflearn/zoo/configs/sr/esr/
--rw-rw-rw-   0        0        0       81 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/configs/sr/esr/anime.json
--rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/zoo/configs/sr/esr/default.json
--rw-rw-rw-   0        0        0     7814 2023-03-29 11:34:44.000000 carefree-learn-0.4.4/cflearn/zoo/core.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:23:16.884310 carefree-learn-0.4.4/cflearn/zoo/models/
--rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/models/__init__.py
--rw-rw-rw-   0        0        0     1606 2023-03-23 05:48:39.000000 carefree-learn-0.4.4/cflearn/zoo/models/clip.py
--rw-rw-rw-   0        0        0      506 2023-03-22 01:51:15.000000 carefree-learn-0.4.4/cflearn/zoo/models/schema.py
--rw-rw-rw-   0        0        0      383 2023-05-17 13:23:16.888297 carefree-learn-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1727 2023-05-17 13:22:51.000000 carefree-learn-0.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.054180 carefree-learn-0.4.5/
+-rw-rw-rw-   0        0        0     1090 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/LICENSE
+-rw-rw-rw-   0        0        0       75 2022-11-10 07:33:05.000000 carefree-learn-0.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     7575 2023-05-22 14:46:50.054180 carefree-learn-0.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7038 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.918865 carefree-learn-0.4.5/carefree_learn.egg-info/
+-rw-rw-rw-   0        0        0     7575 2023-05-22 14:46:49.000000 carefree-learn-0.4.5/carefree_learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10736 2023-05-22 14:46:49.000000 carefree-learn-0.4.5/carefree_learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 14:46:49.000000 carefree-learn-0.4.5/carefree_learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      644 2023-05-22 14:46:49.000000 carefree-learn-0.4.5/carefree_learn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 14:46:49.000000 carefree-learn-0.4.5/carefree_learn.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.922850 carefree-learn-0.4.5/cflearn/
+-rw-rw-rw-   0        0        0      658 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.924843 carefree-learn-0.4.5/cflearn/api/
+-rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/api/__init__.py
+-rw-rw-rw-   0        0        0    24147 2023-03-27 06:18:09.000000 carefree-learn-0.4.5/cflearn/api/api.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.926836 carefree-learn-0.4.5/cflearn/api/cv/
+-rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/api/cv/__init__.py
+-rw-rw-rw-   0        0        0    74341 2023-05-22 14:45:42.000000 carefree-learn-0.4.5/cflearn/api/cv/diffusion.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.928830 carefree-learn-0.4.5/cflearn/api/cv/third_party/
+-rw-rw-rw-   0        0        0      156 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/__init__.py
+-rw-rw-rw-   0        0        0     1069 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/blip.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.929827 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/__init__.py
+-rw-rw-rw-   0        0        0     1386 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/api.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.931820 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/inference/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/inference/__init__.py
+-rw-rw-rw-   0        0        0     1989 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/inference/predictor.py
+-rw-rw-rw-   0        0        0     4395 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/inference/transforms.py
+-rw-rw-rw-   0        0        0      341 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/inference/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.932816 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/mconfigs/
+-rw-rw-rw-   0        0        0      112 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/mconfigs/__init__.py
+-rw-rw-rw-   0        0        0     1660 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py
+-rw-rw-rw-   0        0        0     1953 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/mconfigs/base.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.934809 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.936803 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/
+-rw-rw-rw-   0        0        0       70 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/__init__.py
+-rw-rw-rw-   0        0        0     4553 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py
+-rw-rw-rw-   0        0        0     6090 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py
+-rw-rw-rw-   0        0        0     3629 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.937801 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/
+-rw-rw-rw-   0        0        0      130 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/dih_model.py
+-rw-rw-rw-   0        0        0     1353 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py
+-rw-rw-rw-   0        0        0     3162 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.942783 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/__init__.py
+-rw-rw-rw-   0        0        0     8010 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py
+-rw-rw-rw-   0        0        0     5571 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py
+-rw-rw-rw-   0        0        0     7150 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py
+-rw-rw-rw-   0        0        0    19814 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py
+-rw-rw-rw-   0        0        0     6392 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py
+-rw-rw-rw-   0        0        0     1808 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py
+-rw-rw-rw-   0        0        0    13493 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py
+-rw-rw-rw-   0        0        0     8229 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/unet.py
+-rw-rw-rw-   0        0        0      357 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modifiers.py
+-rw-rw-rw-   0        0        0     4927 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/ops.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.942783 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/utils/__init__.py
+-rw-rw-rw-   0        0        0      445 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/utils/misc.py
+-rw-rw-rw-   0        0        0    16017 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/isnet.py
+-rw-rw-rw-   0        0        0     9132 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/lama.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.944777 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/__init__.py
+-rw-rw-rw-   0        0        0     8006 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/api.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.947766 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/__init__.py
+-rw-rw-rw-   0        0        0      383 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/base_model.py
+-rw-rw-rw-   0        0        0    10222 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/blocks.py
+-rw-rw-rw-   0        0        0     3259 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/dpt_depth.py
+-rw-rw-rw-   0        0        0     2803 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/midas_net.py
+-rw-rw-rw-   0        0        0     6071 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/midas_net_custom.py
+-rw-rw-rw-   0        0        0     8096 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/transforms.py
+-rw-rw-rw-   0        0        0    15154 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/vit.py
+-rw-rw-rw-   0        0        0     4814 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.948763 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/__init__.py
+-rw-rw-rw-   0        0        0     2106 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/api.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.949759 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/models/
+-rw-rw-rw-   0        0        0        0 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/models/__init__.py
+-rw-rw-rw-   0        0        0    10142 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-rw-   0        0        0     9711 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-rw-   0        0        0    26167 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.951753 carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/
+-rw-rw-rw-   0        0        0       20 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/__init__.py
+-rw-rw-rw-   0        0        0     2392 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/api.py
+-rw-rw-rw-   0        0        0    14093 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/body.py
+-rw-rw-rw-   0        0        0     4271 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/hand.py
+-rw-rw-rw-   0        0        0     9090 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/model.py
+-rw-rw-rw-   0        0        0     8699 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/util.py
+-rw-rw-rw-   0        0        0     2053 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/api/cv/third_party/prompt.py
+-rw-rw-rw-   0        0        0     2489 2023-03-23 09:35:16.000000 carefree-learn-0.4.5/cflearn/api/cv/translator.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.952749 carefree-learn-0.4.5/cflearn/api/ml/
+-rw-rw-rw-   0        0        0       20 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/api/ml/__init__.py
+-rw-rw-rw-   0        0        0     8678 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/api/ml/ddr.py
+-rw-rw-rw-   0        0        0      524 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/api/schema.py
+-rw-rw-rw-   0        0        0     2983 2023-05-17 13:13:35.000000 carefree-learn-0.4.5/cflearn/api/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.952749 carefree-learn-0.4.5/cflearn/api/zoo/
+-rw-rw-rw-   0        0        0     6163 2023-03-29 08:24:36.000000 carefree-learn-0.4.5/cflearn/api/zoo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.954743 carefree-learn-0.4.5/cflearn/callbacks/
+-rw-rw-rw-   0        0        0       81 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1118 2023-03-23 09:35:20.000000 carefree-learn-0.4.5/cflearn/callbacks/classification.py
+-rw-rw-rw-   0        0        0     9649 2023-03-23 08:40:04.000000 carefree-learn-0.4.5/cflearn/callbacks/general.py
+-rw-rw-rw-   0        0        0     4212 2023-03-23 09:35:26.000000 carefree-learn-0.4.5/cflearn/callbacks/generator.py
+-rw-rw-rw-   0        0        0      656 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.955739 carefree-learn-0.4.5/cflearn/data/
+-rw-rw-rw-   0        0        0      247 2023-03-28 06:24:25.000000 carefree-learn-0.4.5/cflearn/data/__init__.py
+-rw-rw-rw-   0        0        0     2798 2023-03-28 02:09:34.000000 carefree-learn-0.4.5/cflearn/data/array.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.955739 carefree-learn-0.4.5/cflearn/data/blocks/
+-rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/blocks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.959727 carefree-learn-0.4.5/cflearn/data/blocks/cv/
+-rw-rw-rw-   0        0        0      159 2023-03-29 09:56:34.000000 carefree-learn-0.4.5/cflearn/data/blocks/cv/__init__.py
+-rw-rw-rw-   0        0        0     1447 2023-03-29 10:00:43.000000 carefree-learn-0.4.5/cflearn/data/blocks/cv/crop.py
+-rw-rw-rw-   0        0        0      477 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/blocks/cv/hwc_to_chw.py
+-rw-rw-rw-   0        0        0    31082 2023-03-29 07:34:59.000000 carefree-learn-0.4.5/cflearn/data/blocks/cv/image_folder.py
+-rw-rw-rw-   0        0        0     2054 2023-03-29 07:34:59.000000 carefree-learn-0.4.5/cflearn/data/blocks/cv/normalize.py
+-rw-rw-rw-   0        0        0     1002 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/blocks/cv/to_numpy.py
+-rw-rw-rw-   0        0        0      609 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/blocks/cv/tuple_to_batch.py
+-rw-rw-rw-   0        0        0      375 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/blocks/flatten.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.963713 carefree-learn-0.4.5/cflearn/data/blocks/ml/
+-rw-rw-rw-   0        0        0      176 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/__init__.py
+-rw-rw-rw-   0        0        0    19260 2023-03-29 06:28:32.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/file.py
+-rw-rw-rw-   0        0        0     1729 2023-03-29 06:29:22.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/gather.py
+-rw-rw-rw-   0        0        0     7608 2023-03-29 06:29:31.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/nan_handler.py
+-rw-rw-rw-   0        0        0     7327 2023-03-29 06:29:45.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/preprocessor.py
+-rw-rw-rw-   0        0        0     6234 2023-03-29 06:30:03.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/recognizer.py
+-rw-rw-rw-   0        0        0      416 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/schema.py
+-rw-rw-rw-   0        0        0    12175 2023-03-29 06:30:47.000000 carefree-learn-0.4.5/cflearn/data/blocks/ml/splitter.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.964710 carefree-learn-0.4.5/cflearn/data/ml/
+-rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/ml/__init__.py
+-rw-rw-rw-   0        0        0     7741 2023-03-29 06:34:52.000000 carefree-learn-0.4.5/cflearn/data/ml/api.py
+-rw-rw-rw-   0        0        0     1292 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/ml/datasets.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.966704 carefree-learn-0.4.5/cflearn/data/pytorch/
+-rw-rw-rw-   0        0        0       45 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/data/pytorch/__init__.py
+-rw-rw-rw-   0        0        0     8349 2023-03-27 12:47:27.000000 carefree-learn-0.4.5/cflearn/data/pytorch/api.py
+-rw-rw-rw-   0        0        0     1406 2023-03-29 06:36:58.000000 carefree-learn-0.4.5/cflearn/data/pytorch/datasets.py
+-rw-rw-rw-   0        0        0     7842 2023-03-28 02:09:41.000000 carefree-learn-0.4.5/cflearn/data/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.967700 carefree-learn-0.4.5/cflearn/dist/
+-rw-rw-rw-   0        0        0       18 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/dist/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.969694 carefree-learn-0.4.5/cflearn/dist/ml/
+-rw-rw-rw-   0        0        0      159 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/dist/ml/__init__.py
+-rw-rw-rw-   0        0        0     8874 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/dist/ml/experiment.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.971687 carefree-learn-0.4.5/cflearn/dist/ml/runs/
+-rw-rw-rw-   0        0        0        0 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/dist/ml/runs/__init__.py
+-rw-rw-rw-   0        0        0     1320 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/dist/ml/runs/_utils.py
+-rw-rw-rw-   0        0        0      291 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/dist/ml/runs/basic.py
+-rw-rw-rw-   0        0        0     1709 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/dist/ml/task.py
+-rw-rw-rw-   0        0        0     8910 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/inference.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.975674 carefree-learn-0.4.5/cflearn/losses/
+-rw-rw-rw-   0        0        0       84 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/losses/__init__.py
+-rw-rw-rw-   0        0        0     6391 2023-03-29 12:15:03.000000 carefree-learn-0.4.5/cflearn/losses/basic.py
+-rw-rw-rw-   0        0        0     2546 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/losses/gan.py
+-rw-rw-rw-   0        0        0     2812 2023-03-24 02:18:57.000000 carefree-learn-0.4.5/cflearn/losses/lpips.py
+-rw-rw-rw-   0        0        0     3962 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/losses/vae.py
+-rw-rw-rw-   0        0        0     5614 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.978666 carefree-learn-0.4.5/cflearn/misc/
+-rw-rw-rw-   0        0        0        0 2023-02-14 02:22:11.000000 carefree-learn-0.4.5/cflearn/misc/__init__.py
+-rw-rw-rw-   0        0        0    14696 2023-04-20 10:57:14.000000 carefree-learn-0.4.5/cflearn/misc/available.json
+-rw-rw-rw-   0        0        0     1375 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/misc/mixins.py
+-rw-rw-rw-   0        0        0    44325 2023-05-19 13:03:56.000000 carefree-learn-0.4.5/cflearn/misc/toolkit.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.979662 carefree-learn-0.4.5/cflearn/models/
+-rw-rw-rw-   0        0        0       62 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/__init__.py
+-rw-rw-rw-   0        0        0     5563 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/bases.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.980659 carefree-learn-0.4.5/cflearn/models/cv/
+-rw-rw-rw-   0        0        0      167 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.982385 carefree-learn-0.4.5/cflearn/models/cv/ae/
+-rw-rw-rw-   0        0        0       38 2023-03-22 05:28:24.000000 carefree-learn-0.4.5/cflearn/models/cv/ae/__init__.py
+-rw-rw-rw-   0        0        0    12091 2023-03-27 01:50:04.000000 carefree-learn-0.4.5/cflearn/models/cv/ae/common.py
+-rw-rw-rw-   0        0        0     8409 2023-03-27 01:52:38.000000 carefree-learn-0.4.5/cflearn/models/cv/ae/kl.py
+-rw-rw-rw-   0        0        0     7970 2023-03-27 01:52:49.000000 carefree-learn-0.4.5/cflearn/models/cv/ae/vq.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.983389 carefree-learn-0.4.5/cflearn/models/cv/classifier/
+-rw-rw-rw-   0        0        0       24 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/classifier/__init__.py
+-rw-rw-rw-   0        0        0     4079 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/classifier/vanilla.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.987376 carefree-learn-0.4.5/cflearn/models/cv/decoder/
+-rw-rw-rw-   0        0        0      145 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/decoder/__init__.py
+-rw-rw-rw-   0        0        0     3619 2023-02-27 01:58:50.000000 carefree-learn-0.4.5/cflearn/models/cv/decoder/attn.py
+-rw-rw-rw-   0        0        0     4162 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/decoder/schema.py
+-rw-rw-rw-   0        0        0     8739 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/decoder/style_gan.py
+-rw-rw-rw-   0        0        0    14508 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/decoder/style_gan_v2.py
+-rw-rw-rw-   0        0        0     9329 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/decoder/vanilla.py
+-rw-rw-rw-   0        0        0     3952 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/decoder/vqgan.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.990365 carefree-learn-0.4.5/cflearn/models/cv/diffusion/
+-rw-rw-rw-   0        0        0       87 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.992358 carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/
+-rw-rw-rw-   0        0        0       69 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/__init__.py
+-rw-rw-rw-   0        0        0    10010 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/clip.py
+-rw-rw-rw-   0        0        0     1525 2023-03-24 02:19:09.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/rescaler.py
+-rw-rw-rw-   0        0        0     1182 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/schema.py
+-rw-rw-rw-   0        0        0    29604 2023-05-19 13:31:09.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/ddpm.py
+-rw-rw-rw-   0        0        0    10675 2023-05-18 07:21:12.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/ldm.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.995377 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/
+-rw-rw-rw-   0        0        0      137 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/__init__.py
+-rw-rw-rw-   0        0        0     2258 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/basic.py
+-rw-rw-rw-   0        0        0     9817 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/ddim.py
+-rw-rw-rw-   0        0        0    13157 2023-05-21 02:40:49.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/k_samplers.py
+-rw-rw-rw-   0        0        0     2593 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/plms.py
+-rw-rw-rw-   0        0        0     7804 2023-05-21 03:23:44.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/schema.py
+-rw-rw-rw-   0        0        0    16613 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/solver.py
+-rw-rw-rw-   0        0        0     2561 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/utils.py
+-rw-rw-rw-   0        0        0    20269 2023-04-20 03:26:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/unet.py
+-rw-rw-rw-   0        0        0      737 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/diffusion/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.999364 carefree-learn-0.4.5/cflearn/models/cv/encoder/
+-rw-rw-rw-   0        0        0      240 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/__init__.py
+-rw-rw-rw-   0        0        0     3369 2023-02-27 01:58:50.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/attn.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.001358 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/
+-rw-rw-rw-   0        0        0       64 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/api.py
+-rw-rw-rw-   0        0        0     4242 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/core.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.003351 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/
+-rw-rw-rw-   0        0        0       97 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/__init__.py
+-rw-rw-rw-   0        0        0      430 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/mobilenet.py
+-rw-rw-rw-   0        0        0     1225 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/resnet.py
+-rw-rw-rw-   0        0        0     5392 2023-02-10 05:26:29.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/transformer.py
+-rw-rw-rw-   0        0        0    13725 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/vgg.py
+-rw-rw-rw-   0        0        0      968 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/register.py
+-rw-rw-rw-   0        0        0     1133 2023-02-10 03:39:20.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/fnet.py
+-rw-rw-rw-   0        0        0     1132 2023-02-10 03:39:20.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/mixer.py
+-rw-rw-rw-   0        0        0     2336 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/perceiver.py
+-rw-rw-rw-   0        0        0     1149 2023-02-10 03:39:20.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/pool_former.py
+-rw-rw-rw-   0        0        0     5124 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/schema.py
+-rw-rw-rw-   0        0        0     6125 2023-03-22 07:19:34.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/transformer.py
+-rw-rw-rw-   0        0        0     5535 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/vanilla.py
+-rw-rw-rw-   0        0        0     5473 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/models/cv/encoder/vqgan.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.004348 carefree-learn-0.4.5/cflearn/models/cv/gan/
+-rw-rw-rw-   0        0        0       55 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/gan/__init__.py
+-rw-rw-rw-   0        0        0     5920 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/cv/gan/discriminators.py
+-rw-rw-rw-   0        0        0     7730 2023-03-29 11:05:45.000000 carefree-learn-0.4.5/cflearn/models/cv/gan/schema.py
+-rw-rw-rw-   0        0        0     1913 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/gan/vanilla.py
+-rw-rw-rw-   0        0        0     6731 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/general.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.005344 carefree-learn-0.4.5/cflearn/models/cv/translator/
+-rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/cv/translator/__init__.py
+-rw-rw-rw-   0        0        0     4018 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/cv/translator/rrdb.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.006342 carefree-learn-0.4.5/cflearn/models/implicit/
+-rw-rw-rw-   0        0        0       22 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/implicit/__init__.py
+-rw-rw-rw-   0        0        0     7927 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/models/implicit/siren.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.011325 carefree-learn-0.4.5/cflearn/models/ml/
+-rw-rw-rw-   0        0        0      165 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/__init__.py
+-rw-rw-rw-   0        0        0     1857 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/base.py
+-rw-rw-rw-   0        0        0    11624 2023-03-29 12:15:02.000000 carefree-learn-0.4.5/cflearn/models/ml/ddr.py
+-rw-rw-rw-   0        0        0     8958 2023-03-28 02:09:49.000000 carefree-learn-0.4.5/cflearn/models/ml/encoders.py
+-rw-rw-rw-   0        0        0     2392 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/fcnn.py
+-rw-rw-rw-   0        0        0     1100 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/linear.py
+-rw-rw-rw-   0        0        0     6980 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/mixed_stacked.py
+-rw-rw-rw-   0        0        0     7976 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/nbm.py
+-rw-rw-rw-   0        0        0     5272 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/ndt.py
+-rw-rw-rw-   0        0        0     3068 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/rnn.py
+-rw-rw-rw-   0        0        0     2798 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/ml/wnd.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.013318 carefree-learn-0.4.5/cflearn/models/multimodal/
+-rw-rw-rw-   0        0        0       21 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/multimodal/__init__.py
+-rw-rw-rw-   0        0        0    10260 2023-03-23 08:58:17.000000 carefree-learn-0.4.5/cflearn/models/multimodal/clip.py
+-rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/multimodal/constants.py
+-rw-rw-rw-   0        0        0     1554 2023-03-29 11:05:45.000000 carefree-learn-0.4.5/cflearn/models/multimodal/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.013318 carefree-learn-0.4.5/cflearn/models/nlp/
+-rw-rw-rw-   0        0        0       80 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.015312 carefree-learn-0.4.5/cflearn/models/nlp/encoder/
+-rw-rw-rw-   0        0        0       28 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/encoder/__init__.py
+-rw-rw-rw-   0        0        0       19 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/encoder/constants.py
+-rw-rw-rw-   0        0        0     3694 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/encoder/transformer.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.016307 carefree-learn-0.4.5/cflearn/models/nlp/tokenizers/
+-rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/tokenizers/__init__.py
+-rw-rw-rw-   0        0        0     2371 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/nlp/tokenizers/clip.py
+-rw-rw-rw-   0        0        0     1226 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/tokenizers/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.018302 carefree-learn-0.4.5/cflearn/models/nlp/transformers/
+-rw-rw-rw-   0        0        0       66 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/transformers/__init__.py
+-rw-rw-rw-   0        0        0     3547 2023-03-27 13:58:44.000000 carefree-learn-0.4.5/cflearn/models/nlp/transformers/core.py
+-rw-rw-rw-   0        0        0     1575 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/transformers/opus.py
+-rw-rw-rw-   0        0        0      813 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/models/nlp/transformers/simbert.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.019298 carefree-learn-0.4.5/cflearn/models/schemas/
+-rw-rw-rw-   0        0        0       42 2023-03-27 01:49:17.000000 carefree-learn-0.4.5/cflearn/models/schemas/__init__.py
+-rw-rw-rw-   0        0        0    12838 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/models/schemas/custom.py
+-rw-rw-rw-   0        0        0     4631 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/models/schemas/cv.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.021292 carefree-learn-0.4.5/cflearn/modules/
+-rw-rw-rw-   0        0        0       54 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/modules/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.030262 carefree-learn-0.4.5/cflearn/modules/blocks/
+-rw-rw-rw-   0        0        0      756 2023-03-24 08:39:05.000000 carefree-learn-0.4.5/cflearn/modules/blocks/__init__.py
+-rw-rw-rw-   0        0        0     5165 2023-03-24 02:18:16.000000 carefree-learn-0.4.5/cflearn/modules/blocks/activations.py
+-rw-rw-rw-   0        0        0    21356 2023-05-08 11:16:44.000000 carefree-learn-0.4.5/cflearn/modules/blocks/attentions.py
+-rw-rw-rw-   0        0        0     6448 2022-11-09 12:05:57.000000 carefree-learn-0.4.5/cflearn/modules/blocks/common.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.031259 carefree-learn-0.4.5/cflearn/modules/blocks/convs/
+-rw-rw-rw-   0        0        0       47 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/modules/blocks/convs/__init__.py
+-rw-rw-rw-   0        0        0    19321 2023-03-24 02:29:08.000000 carefree-learn-0.4.5/cflearn/modules/blocks/convs/basic.py
+-rw-rw-rw-   0        0        0     8836 2023-03-24 02:19:26.000000 carefree-learn-0.4.5/cflearn/modules/blocks/convs/residual.py
+-rw-rw-rw-   0        0        0    18802 2023-04-12 11:14:59.000000 carefree-learn-0.4.5/cflearn/modules/blocks/customs.py
+-rw-rw-rw-   0        0        0     8503 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/modules/blocks/high_level.py
+-rw-rw-rw-   0        0        0    15078 2023-05-16 07:51:00.000000 carefree-learn-0.4.5/cflearn/modules/blocks/hijacks.py
+-rw-rw-rw-   0        0        0     1304 2023-04-12 13:32:32.000000 carefree-learn-0.4.5/cflearn/modules/blocks/hooks.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.032255 carefree-learn-0.4.5/cflearn/modules/blocks/implementations/
+-rw-rw-rw-   0        0        0       26 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/modules/blocks/implementations/__init__.py
+-rw-rw-rw-   0        0        0     4708 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/modules/blocks/implementations/perceiver.py
+-rw-rw-rw-   0        0        0     6189 2023-01-29 11:37:21.000000 carefree-learn-0.4.5/cflearn/modules/blocks/mappings.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.036242 carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/
+-rw-rw-rw-   0        0        0      127 2023-02-10 03:31:37.000000 carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/__init__.py
+-rw-rw-rw-   0        0        0    28432 2023-04-12 08:04:35.000000 carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/api.py
+-rw-rw-rw-   0        0        0     3774 2023-03-24 08:39:41.000000 carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/channel_mixers.py
+-rw-rw-rw-   0        0        0     1179 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/poolers.py
+-rw-rw-rw-   0        0        0     1325 2023-02-10 05:18:20.000000 carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/schema.py
+-rw-rw-rw-   0        0        0     6998 2023-02-10 10:31:50.000000 carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/token_mixers.py
+-rw-rw-rw-   0        0        0     4682 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/modules/blocks/norms.py
+-rw-rw-rw-   0        0        0      863 2023-02-27 01:58:50.000000 carefree-learn-0.4.5/cflearn/modules/blocks/utils.py
+-rw-rw-rw-   0        0        0     4751 2022-10-23 14:55:07.000000 carefree-learn-0.4.5/cflearn/modules/optimizers.py
+-rw-rw-rw-   0        0        0     9159 2022-11-09 12:09:28.000000 carefree-learn-0.4.5/cflearn/modules/schedulers.py
+-rw-rw-rw-   0        0        0     4774 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/monitors.py
+-rw-rw-rw-   0        0        0      744 2023-05-19 03:26:36.000000 carefree-learn-0.4.5/cflearn/parameters.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.039231 carefree-learn-0.4.5/cflearn/pipeline/
+-rw-rw-rw-   0        0        0       92 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/pipeline/__init__.py
+-rw-rw-rw-   0        0        0    23551 2023-03-29 11:32:53.000000 carefree-learn-0.4.5/cflearn/pipeline/api.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.041225 carefree-learn-0.4.5/cflearn/pipeline/blocks/
+-rw-rw-rw-   0        0        0       41 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/pipeline/blocks/__init__.py
+-rw-rw-rw-   0        0        0    36043 2023-03-27 01:51:03.000000 carefree-learn-0.4.5/cflearn/pipeline/blocks/basic.py
+-rw-rw-rw-   0        0        0     2735 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/pipeline/blocks/ml.py
+-rw-rw-rw-   0        0        0     1335 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/pipeline/blocks/utils.py
+-rw-rw-rw-   0        0        0     3921 2023-03-23 08:46:39.000000 carefree-learn-0.4.5/cflearn/pipeline/core.py
+-rw-rw-rw-   0        0        0      310 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/pipeline/schema.py
+-rw-rw-rw-   0        0        0     1545 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/pipeline/third_party.py
+-rw-rw-rw-   0        0        0      510 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/register.py
+-rw-rw-rw-   0        0        0    60784 2023-03-29 15:41:28.000000 carefree-learn-0.4.5/cflearn/schema.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.042221 carefree-learn-0.4.5/cflearn/scripts/
+-rw-rw-rw-   0        0        0       18 2023-03-24 10:59:16.000000 carefree-learn-0.4.5/cflearn/scripts/__init__.py
+-rw-rw-rw-   0        0        0    12752 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/scripts/sd.py
+-rw-rw-rw-   0        0        0    28526 2023-04-04 02:24:07.000000 carefree-learn-0.4.5/cflearn/trainer.py
+-rw-rw-rw-   0        0        0     1053 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/types.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.044216 carefree-learn-0.4.5/cflearn/zoo/
+-rw-rw-rw-   0        0        0       21 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.888455 carefree-learn-0.4.5/cflearn/zoo/configs/
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.886462 carefree-learn-0.4.5/cflearn/zoo/configs/ae/
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.045211 carefree-learn-0.4.5/cflearn/zoo/configs/ae/kl/
+-rw-rw-rw-   0        0        0      201 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/ae/kl/f16.json
+-rw-rw-rw-   0        0        0      868 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/zoo/configs/ae/kl/f4.json
+-rw-rw-rw-   0        0        0      160 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/ae/kl/f8.json
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.047205 carefree-learn-0.4.5/cflearn/zoo/configs/ae/vq/
+-rw-rw-rw-   0        0        0      205 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/ae/vq/f4.json
+-rw-rw-rw-   0        0        0       92 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/ae/vq/f4_no_attn.json
+-rw-rw-rw-   0        0        0      295 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/ae/vq/f8.json
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.887460 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.047205 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ddpm/
+-rw-rw-rw-   0        0        0     1155 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ddpm/default.json
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.050195 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/
+-rw-rw-rw-   0        0        0      513 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/default.json
+-rw-rw-rw-   0        0        0      451 2023-05-08 10:29:54.000000 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/sd.json
+-rw-rw-rw-   0        0        0      125 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/sd_inpainting.json
+-rw-rw-rw-   0        0        0      344 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/sd_v2.json
+-rw-rw-rw-   0        0        0      104 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/sd_v2_base.json
+-rw-rw-rw-   0        0        0      600 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/vq.json
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.887460 carefree-learn-0.4.5/cflearn/zoo/configs/multimodal/
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.052188 carefree-learn-0.4.5/cflearn/zoo/configs/multimodal/clip/
+-rw-rw-rw-   0        0        0      525 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/multimodal/clip/chinese.json
+-rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/zoo/configs/multimodal/clip/default.json
+-rw-rw-rw-   0        0        0      269 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/multimodal/clip/large.json
+-rw-rw-rw-   0        0        0      389 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/multimodal/clip/open_clip_ViT_H_14.json
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:49.888455 carefree-learn-0.4.5/cflearn/zoo/configs/sr/
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.052188 carefree-learn-0.4.5/cflearn/zoo/configs/sr/esr/
+-rw-rw-rw-   0        0        0       81 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/configs/sr/esr/anime.json
+-rw-rw-rw-   0        0        0       79 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/zoo/configs/sr/esr/default.json
+-rw-rw-rw-   0        0        0     7814 2023-03-29 11:34:44.000000 carefree-learn-0.4.5/cflearn/zoo/core.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:46:50.053184 carefree-learn-0.4.5/cflearn/zoo/models/
+-rw-rw-rw-   0        0        0       44 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/models/__init__.py
+-rw-rw-rw-   0        0        0     1606 2023-03-23 05:48:39.000000 carefree-learn-0.4.5/cflearn/zoo/models/clip.py
+-rw-rw-rw-   0        0        0      506 2023-03-22 01:51:15.000000 carefree-learn-0.4.5/cflearn/zoo/models/schema.py
+-rw-rw-rw-   0        0        0      383 2023-05-22 14:46:50.058168 carefree-learn-0.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1748 2023-05-22 14:46:08.000000 carefree-learn-0.4.5/setup.py
```

### Comparing `carefree-learn-0.4.4/LICENSE` & `carefree-learn-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/PKG-INFO` & `carefree-learn-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-learn
-Version: 0.4.4
+Version: 0.4.5
 Summary: Deep Learning with PyTorch made easy
 Home-page: https://github.com/carefree0910/carefree-learn
-Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.4.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.5.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python machine-learning deep-learning solution PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: onnx
 Provides-Extra: cv
 Provides-Extra: cv_full
```

### Comparing `carefree-learn-0.4.4/README.md` & `carefree-learn-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/carefree_learn.egg-info/PKG-INFO` & `carefree-learn-0.4.5/carefree_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: carefree-learn
-Version: 0.4.4
+Version: 0.4.5
 Summary: Deep Learning with PyTorch made easy
 Home-page: https://github.com/carefree0910/carefree-learn
-Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.4.tar.gz
+Download-URL: https://github.com/carefree0910/carefree-learn/archive/v0.4.5.tar.gz
 Author: carefree0910
 Author-email: syameimaru.saki@gmail.com
 Keywords: python machine-learning deep-learning solution PyTorch
 Description-Content-Type: text/markdown
 Provides-Extra: onnx
 Provides-Extra: cv
 Provides-Extra: cv_full
```

### Comparing `carefree-learn-0.4.4/carefree_learn.egg-info/SOURCES.txt` & `carefree-learn-0.4.5/carefree_learn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/carefree_learn.egg-info/requires.txt` & `carefree-learn-0.4.5/carefree_learn.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+filelock
 accelerate
 safetensors
 carefree-toolkit>=0.3.5
 
 [cv]
 ftfy
 lmdb
```

### Comparing `carefree-learn-0.4.4/cflearn/__init__.py` & `carefree-learn-0.4.5/cflearn/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/api.py` & `carefree-learn-0.4.5/cflearn/api/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/diffusion.py` & `carefree-learn-0.4.5/cflearn/api/cv/diffusion.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,25 +20,30 @@
 from typing import Tuple
 from typing import Union
 from typing import TypeVar
 from typing import Callable
 from typing import Optional
 from typing import NamedTuple
 from typing import ContextManager
+from filelock import FileLock
+from dataclasses import dataclass
 from cftool.cv import to_rgb
+from cftool.cv import to_uint8
 from cftool.cv import read_image
 from cftool.cv import save_images
 from cftool.cv import restrict_wh
 from cftool.cv import get_suitable_size
 from cftool.cv import ReadImageResponse
 from cftool.misc import safe_execute
 from cftool.misc import print_warning
 from cftool.misc import shallow_copy_dict
 from cftool.types import arr_type
 from cftool.types import tensor_dict_type
+from safetensors.torch import load_file
+from cflearn.misc.toolkit import _get_file_size
 
 from ..zoo import ldm_sd
 from ..zoo import ldm_sd_v2
 from ..zoo import ldm_sd_v2_base
 from ..zoo import ldm_sd_tag
 from ..zoo import ldm_sd_inpainting
 from ..zoo import ldm_sr
@@ -55,14 +60,15 @@
 from ...schema import DataConfig
 from ...constants import INPUT_KEY
 from ...constants import PREDICTIONS_KEY
 from ...parameters import OPT
 from ...data.utils import predict_array_data
 from ...data.utils import TensorBatcher
 from ...misc.toolkit import slerp
+from ...misc.toolkit import freeze
 from ...misc.toolkit import new_seed
 from ...misc.toolkit import download_model
 from ...misc.toolkit import download_static
 from ...misc.toolkit import seed_everything
 from ...misc.toolkit import eval_context
 from ...modules.blocks import Conv2d
 from ...models.cv.diffusion import LDM
@@ -110,21 +116,26 @@
 
 class SizeInfo(NamedTuple):
     factor: int
     opt_size: int
 
 
 class MaskedCond(NamedTuple):
-    image_res: ReadImageResponse
-    mask_res: ReadImageResponse
+    image: np.ndarray
     mask: np.ndarray
-    remained_image: np.ndarray
-    remained_mask: np.ndarray
     mask_cond: Tensor
     remained_image_cond: Tensor
+    remained_image: np.ndarray
+    remained_mask: np.ndarray
+    image_alpha: Optional[np.ndarray]
+    original_size: Tuple[int, int]
+    original_image: Image.Image
+    original_mask: Image.Image
+    wh_ratio: Tuple[float, float]
+    crop_res: Optional["CropResponse"]
 
 
 T = TypeVar("T", bound="DiffusionAPI")
 TAnnotator = TypeVar("TAnnotator", bound="Annotator")
 
 
 class SDVersions(str, Enum):
@@ -134,15 +145,15 @@
     ANIME_ANYTHING = "anime_anything"
     ANIME_HYBRID = "anime_hybrid"
     ANIME_GUOFENG = "anime_guofeng"
     ANIME_ORANGE = "anime_orange"
     DREAMLIKE = "dreamlike_v1"
 
 
-def get_sd_tag(version: SDVersions) -> str:
+def get_sd_tag(version: str) -> str:
     if version == SDVersions.v1_5_BC:
         return "v1.5"
     if version == SDVersions.ANIME:
         return "anime_nai"
     if version == SDVersions.ANIME_ANYTHING:
         return "anime_anything_v3"
     if version == SDVersions.ANIME_HYBRID:
@@ -178,23 +189,262 @@
     return tuple(map(get_suitable_size, new_size, (anchor, anchor)))  # type: ignore
 
 
 def get_highres_steps(num_steps: int, fidelity: float) -> int:
     return int(num_steps / min(1.0 - fidelity, 0.999))
 
 
+def _convert_external(m: "DiffusionAPI", tag: str, sub_folder: Optional[str]) -> str:
+    external_root = OPT.external_dir
+    if sub_folder is not None:
+        external_root = os.path.join(external_root, sub_folder)
+    lock_path = os.path.join(external_root, "load_external.lock")
+    lock = FileLock(lock_path)
+    with lock:
+        converted_sizes_path = os.path.join(external_root, "sizes.json")
+        sizes: Dict[str, int]
+        if not os.path.isfile(converted_sizes_path):
+            sizes = {}
+        else:
+            with open(converted_sizes_path, "r") as f:
+                sizes = json.load(f)
+        converted_path = os.path.join(external_root, f"{tag}_converted.pt")
+        v_size = sizes.get(tag)
+        f_size = (
+            None
+            if not os.path.isfile(converted_path)
+            else _get_file_size(converted_path)
+        )
+        if f_size is None or v_size != f_size:
+            if f_size is not None:
+                print(f"> '{tag}' has been converted but size mismatch")
+            print(f"> converting external weights '{tag}'")
+            model_path = os.path.join(external_root, f"{tag}.ckpt")
+            if not os.path.isfile(model_path):
+                st_path = os.path.join(external_root, f"{tag}.safetensors")
+                if not os.path.isfile(st_path):
+                    raise FileNotFoundError(f"cannot find '{tag}'")
+                torch.save(load_file(st_path), model_path)
+
+            import cflearn
+
+            d = cflearn.scripts.sd.convert(model_path, m, load=False)
+
+            torch.save(d, converted_path)
+            sizes[tag] = _get_file_size(converted_path)
+        with open(converted_sizes_path, "w") as f:
+            json.dump(sizes, f)
+        return converted_path
+
+
+class InpaintingMode(str, Enum):
+    NORMAL = "normal"
+    MASKED = "masked"
+
+
+TLtRb = Tuple[int, int, int, int]
+
+
+@dataclass
+class InpaintingSettings:
+    mode: InpaintingMode = InpaintingMode.NORMAL
+    mask_blur: Optional[Union[int, Tuple[int, int]]] = None
+    mask_padding: Optional[Union[int, Tuple[int, int]]] = 32
+    mask_binary_threshold: Optional[int] = 32
+
+
+class CropResponse(NamedTuple):
+    lt_rb: TLtRb
+    cropped_mask: np.ndarray
+    resized_image_tensor: np.ndarray
+    resized_mask_tensor: np.ndarray
+
+
+def get_mask_lt_rb(uint8_mask: np.ndarray, threshold: Optional[int]) -> TLtRb:
+    ys, xs = np.where(uint8_mask > (threshold or 0))
+    lt = xs.min().item(), ys.min().item()
+    rb = xs.max().item(), ys.max().item()
+    return *lt, *rb
+
+
+def crop_with(inp: np.ndarray, lt_rb: TLtRb) -> np.ndarray:
+    return inp[lt_rb[1] : lt_rb[3], lt_rb[0] : lt_rb[2]]
+
+
+def crop_tensor_with(inp: Tensor, lt_rb: TLtRb) -> Tensor:
+    return inp[..., lt_rb[1] : lt_rb[3], lt_rb[0] : lt_rb[2]]
+
+
+def resize(
+    inp: np.ndarray,
+    wh: Tuple[int, int],
+    interpolation: int = cv2.INTER_LANCZOS4,
+) -> np.ndarray:
+    return cv2.resize(inp, wh, interpolation=interpolation)
+
+
+def crop_masked_area(
+    image_tensor: np.ndarray,
+    mask_tensor: np.ndarray,
+    settings: InpaintingSettings,
+) -> CropResponse:
+    image = image_tensor[0].transpose(1, 2, 0)
+    mask = mask_tensor[0, 0]
+    h, w = image.shape[:2]
+    l, t, r, b = get_mask_lt_rb(to_uint8(mask), settings.mask_binary_threshold)
+    if settings.mask_padding is not None:
+        padding = settings.mask_padding
+        if isinstance(padding, int):
+            padding = padding, padding
+        l = max(0, l - padding[0])
+        t = max(0, t - padding[1])
+        r = min(w, r + padding[0])
+        b = min(h, b + padding[1])
+    cropped_h, cropped_w = b - t, r - l
+    # adjust lt_rb to make the cropped aspect ratio equals to the original one
+    if cropped_h / cropped_w > h / w:
+        dw = (int(cropped_h * w / h) - cropped_w) // 2
+        dh = 0
+    else:
+        dw = 0
+        dh = (int(cropped_w * h / w) - cropped_h) // 2
+    if dw > 0:
+        if l < dw:
+            l = 0
+            r = min(w, cropped_w + dw * 2)
+        elif r + dw > w:
+            r = w
+            l = max(0, w - cropped_w - dw * 2)
+        else:
+            l -= dw
+            r += dw
+    if dh > 0:
+        if t < dh:
+            t = 0
+            b = min(h, cropped_h + dh * 2)
+        elif b + dh > h:
+            b = h
+            t = max(0, h - cropped_h - dh * 2)
+        else:
+            t -= dh
+            b += dh
+    # finalize
+    lt_rb = l, t, r, b
+    cropped_image = crop_with(image, lt_rb)
+    cropped_mask = crop_with(mask, lt_rb)
+    resized_image = resize(cropped_image, (w, h))
+    resized_mask = resize(cropped_mask, (w, h), cv2.INTER_NEAREST)
+    resized_image = resized_image.transpose(2, 0, 1)[None]
+    resized_mask = resized_mask[None, None]
+    return CropResponse(lt_rb, cropped_mask, resized_image, resized_mask)
+
+
+def normalize_image_to_diffusion(image: Image.Image) -> np.ndarray:
+    return np.array(image).astype(np.float32) / 127.5 - 1.0
+
+
+def recover_with(
+    original: Image.Image,
+    sampled: Tensor,
+    crop: CropResponse,
+    wh_ratio: Tuple[float, float],
+    settings: InpaintingSettings,
+) -> Tensor:
+    l, t, r, b = crop.lt_rb
+    w_ratio, h_ratio = wh_ratio
+    l = round(l * w_ratio)
+    t = round(t * h_ratio)
+    r = round(r * w_ratio)
+    b = round(b * h_ratio)
+    c_mask = crop.cropped_mask
+    if settings.mask_padding is None:
+        c_blurred_mask = c_mask
+    else:
+        blur = settings.mask_padding
+        if isinstance(blur, int):
+            blur = blur, blur
+        c_blurred_mask = cv2.blur(c_mask, blur)
+    sampled_array = sampled.numpy().transpose([0, 2, 3, 1])
+    o_array = normalize_image_to_diffusion(to_rgb(original))
+    c_o_array = crop_with(o_array, (l, t, r, b))
+    ch, cw = c_o_array.shape[:2]
+    if ch != c_blurred_mask.shape[0] or cw != c_blurred_mask.shape[1]:
+        c_blurred_mask = resize(c_blurred_mask, (cw, ch))
+    c_blurred_mask = c_blurred_mask[..., None]
+    mixed: List[np.ndarray] = []
+    for i_sampled in sampled_array:
+        i_sampled = resize(i_sampled, (cw, ch))
+        i_sampled = i_sampled * c_blurred_mask + c_o_array * (1.0 - c_blurred_mask)
+        i_pasted = o_array.copy()
+        i_pasted[t:b, l:r] = i_sampled
+        mixed.append(i_pasted.transpose([2, 0, 1]))
+    return torch.from_numpy(np.stack(mixed, axis=0))
+
+
+def crop_controlnet(kwargs: Dict[str, Any], crop_res: Optional[CropResponse]) -> None:
+    if crop_res is None:
+        return
+    hint: Optional[List[Tuple[str, Tensor]]] = kwargs.get(CONTROL_HINT_KEY, None)
+    if hint is None:
+        return
+    for i, h in enumerate(hint):
+        h_h, h_w = h[1].shape[-2:]
+        h_tensor = crop_tensor_with(h[1], crop_res.lt_rb)
+        h_tensor = F.interpolate(h_tensor, (h_h, h_w), mode="bilinear")
+        hint[i] = h[0], h_tensor
+
+
+class CroppedResponse(NamedTuple):
+    image: np.ndarray
+    mask: np.ndarray
+    wh_ratio: Tuple[float, float]
+    crop_res: Optional[CropResponse]
+
+
+def get_cropped(
+    image_res: ReadImageResponse,
+    mask_res: ReadImageResponse,
+    inpainting_settings: Optional[InpaintingSettings],
+) -> CroppedResponse:
+    ow, oh = image_res.original_size
+    ih, iw = image_res.image.shape[-2:]
+    wh_ratio = ow / iw, oh / ih
+    if inpainting_settings is None or inpainting_settings.mode == InpaintingMode.NORMAL:
+        crop_res = None
+        cropped_image = image_res.image
+        cropped_mask = mask_res.image
+    elif inpainting_settings.mode == InpaintingMode.MASKED:
+        crop_res = crop_masked_area(
+            image_res.image,
+            mask_res.image,
+            inpainting_settings,
+        )
+        cropped_image = crop_res.resized_image_tensor
+        cropped_mask = crop_res.resized_mask_tensor
+    else:
+        raise ValueError(f"Unknown inpainting mode: {inpainting_settings.mode}")
+    if inpainting_settings is not None:
+        if inpainting_settings.mask_blur is not None:
+            cropped_mask = cv2.blur(
+                cropped_mask[0][0],
+                (inpainting_settings.mask_blur, inpainting_settings.mask_blur),
+            )
+            cropped_mask = cropped_mask[None, None]
+    return CroppedResponse(cropped_image, cropped_mask, wh_ratio, crop_res)
+
+
 class DiffusionAPI(APIMixin):
     m: DDPM
     sampler: ISampler
     cond_model: Optional[nn.Module]
     first_stage: Optional[IAutoEncoder]
     latest_seed: int
     latest_variation_seed: Optional[int]
     sd_weights: WeightsPool
-    current_sd_version: Optional[SDVersions]
+    current_sd_version: Optional[str]
 
     def __init__(
         self,
         m: DDPM,
         device: torch.device,
         *,
         use_amp: bool = False,
@@ -265,22 +515,37 @@
         if self.first_stage is not None:
             self.first_stage.to(device)
         if unconditional_cond is not None:
             self.sampler.unconditional_cond = unconditional_cond.to(device)
         for k, v in self._uncond_cache.items():
             self._uncond_cache[k] = v.to(device)
 
-    def prepare_sd(self, versions: List[SDVersions]) -> None:
+    def prepare_sd(
+        self,
+        versions: List[str],
+        *,
+        # inpainting workarounds
+        # should set `force_external` to `True` to prepare inpainting with this method
+        sub_folder: Optional[str] = None,
+        force_external: bool = False,
+    ) -> None:
         root = os.path.join(OPT.cache_dir, DLZoo.model_dir)
         for tag in map(get_sd_tag, versions):
             if tag not in self.sd_weights:
-                model_path = download_model(f"ldm_sd_{tag}", root=root)
+                _load_external = lambda: _convert_external(self, tag, sub_folder)
+                if force_external:
+                    model_path = _load_external()
+                else:
+                    try:
+                        model_path = download_model(f"ldm_sd_{tag}", root=root)
+                    except:
+                        model_path = _load_external()
                 self.sd_weights.register(tag, model_path)
 
-    def switch_sd(self, version: SDVersions) -> None:
+    def switch_sd(self, version: str) -> None:
         tag = get_sd_tag(version)
         if self.current_sd_version is not None:
             if tag == get_sd_tag(self.current_sd_version):
                 return
         d = self.sd_weights.get(tag)
         with self.load_context() as m:
             m.load_state_dict(d)
@@ -622,87 +887,86 @@
         self,
         txt: Union[str, List[str]],
         image: Union[str, Image.Image],
         mask: Union[str, Image.Image],
         export_path: Optional[str] = None,
         *,
         seed: Optional[int] = None,
-        reference: Optional[Union[str, Image.Image]] = None,
-        reference_fidelity: float = 0.2,
         anchor: int = 64,
         max_wh: int = 512,
         num_samples: Optional[int] = None,
         num_steps: Optional[int] = None,
         clip_output: bool = True,
         keep_original: bool = False,
-        ref_mask_smooth: int = 0,
         use_raw_inpainting: bool = False,
-        raw_inpainting_use_ref: bool = False,
-        raw_inpainting_fidelity: float = 0.2,
+        inpainting_settings: Optional[InpaintingSettings] = None,
         callback: Optional[Callable[[Tensor], Tensor]] = None,
-        use_latent_guidance: bool = False,
+        use_background_guidance: bool = False,
+        use_reference: bool = False,
+        reference_fidelity: float = 0.2,
         verbose: bool = True,
         **kwargs: Any,
     ) -> Tensor:
         def get_z_ref_pack(
-            res_: ReadImageResponse,
-            mask_: np.ndarray,
+            normalized_image_: np.ndarray,
+            normalized_mask_: np.ndarray,
         ) -> Tuple[Tensor, Tensor, Tensor]:
-            z_ref = self._get_z(res_.image)
-            if ref_mask_smooth > 0:
-                mask_ = cv2.blur(mask_[0][0], (ref_mask_smooth, ref_mask_smooth))
-                mask_ = mask_[None, None]
+            z_ref = self._get_z(normalized_image_)
             z_ref_mask = 1.0 - F.interpolate(
-                torch.from_numpy(mask_).to(z_ref),
+                torch.from_numpy(normalized_mask_).to(z_ref),
                 z_ref.shape[-2:],
                 mode="bicubic",
             )
             if seed is not None:
                 seed_everything(seed)
             z_ref_noise = torch.randn_like(z_ref)
             return z_ref, z_ref_mask, z_ref_noise
 
         def get_z_info_from(
-            reference_: Optional[Union[str, Image.Image]],
+            z_ref_: Optional[Tensor],
             fidelity_: float,
             shape_: Tuple[int, int],
-        ) -> Tuple[Optional[Tensor], Optional[Tuple[int, int]], Dict[str, Any]]:
-            if reference_ is None:
+        ) -> Tuple[Optional[Tensor], Optional[Tuple[int, int]]]:
+            if z_ref_ is None:
                 z = None
-                new_kw = kwargs
                 size = tuple(map(lambda n: n * self.size_info.factor, shape_))
             else:
                 size = None
-                z = self._get_z(read_image(reference_, max_wh, anchor=anchor).image)
-                if z_ref_mask is not None and z_ref_noise is not None:
-                    z = z * z_ref_mask + z_ref_noise * (1.0 - z_ref_mask)
-                z, _, new_kw = self._q_sample(z, num_steps, fidelity_, seed, **kwargs)
-            return z, size, new_kw  # type: ignore
+                args = z_ref_, num_steps, fidelity_, seed
+                z, _, start_step = self._q_sample(*args, **kwargs)
+                kwargs["start_step"] = start_step
+            return z, size  # type: ignore
 
         def paste_original(
             original_: Image.Image,
             mask_: Image.Image,
             sampled_: Tensor,
         ) -> Tensor:
             rgb = to_rgb(original_)
-            rgb_normalized = np.array(rgb).astype(np.float32) / 127.5 - 1.0
+            rgb_normalized = normalize_image_to_diffusion(rgb)
             rgb_normalized = rgb_normalized.transpose([2, 0, 1])[None]
             mask_res_ = read_image(mask_, None, anchor=None, to_mask=True)
             remained_mask_ = ~(mask_res_.image >= 0.5)
             pasted = np.where(remained_mask_, rgb_normalized, sampled_.numpy())
             return torch.from_numpy(pasted)
 
+        if inpainting_settings is None:
+            inpainting_settings = InpaintingSettings()
         txt_list, num_samples = get_txt_cond(txt, num_samples)
+
+        # raw inpainting
         if use_raw_inpainting:
             image_res = read_image(image, max_wh, anchor=anchor)
             mask_res = read_image(mask, max_wh, anchor=anchor, to_mask=True)
-            z_ref, z_ref_mask, z_ref_noise = get_z_ref_pack(image_res, mask_res.image)
-            z, size, kwargs = get_z_info_from(
-                image_res.image if raw_inpainting_use_ref else None,
-                raw_inpainting_fidelity,
+            cropped_res = get_cropped(image_res, mask_res, inpainting_settings)
+            z_ref_pack = get_z_ref_pack(cropped_res.image, cropped_res.mask)
+            z_ref, z_ref_mask, z_ref_noise = z_ref_pack
+            z, size = get_z_info_from(
+                z_ref if use_reference else None,
+                reference_fidelity,
                 z_ref.shape[-2:][::-1],
             )
             kw = shallow_copy_dict(kwargs)
             kw.update(
                 dict(
                     z=z,
                     size=size,
@@ -714,61 +978,88 @@
                     alpha=None,
                     cond=txt_list,
                     num_steps=num_steps,
                     clip_output=clip_output,
                     verbose=verbose,
                 )
             )
+            crop_controlnet(kw, cropped_res.crop_res)
             sampled = self.sample(num_samples, **kw)
+            crop_res = cropped_res.crop_res
+            if crop_res is not None:
+                sampled = recover_with(
+                    image_res.original,
+                    sampled,
+                    crop_res,
+                    cropped_res.wh_ratio,
+                    inpainting_settings,
+                )
             if keep_original:
                 original = image_res.original
                 sampled = paste_original(original, mask_res.original, sampled)
             return sampled
+
+        # 'real' inpainting
         res = self._get_masked_cond(
             image,
             mask,
             max_wh,
             anchor,
             lambda remained_mask, img: np.where(remained_mask, img, 0.5),
             lambda bool_mask: torch.from_numpy(bool_mask),
+            inpainting_settings,
         )
         # sampling
         with switch_sampler_context(self, kwargs.get("sampler")):
             # calculate `z_ref` stuffs based on `use_image_guidance`
-            if not use_latent_guidance:
+            if not use_background_guidance:
                 z_ref = z_ref_mask = z_ref_noise = None
             else:
-                z_ref, z_ref_mask, z_ref_noise = get_z_ref_pack(res.image_res, res.mask)
-                reference = res.image_res.original
-            # calculate `z` based on `reference`
+                z_ref, z_ref_mask, z_ref_noise = get_z_ref_pack(res.image, res.mask)
+            # calculate `z` based on `z_ref`, if needed
             z_shape = res.remained_image_cond.shape[-2:][::-1]
-            z, size, kwargs = get_z_info_from(reference, reference_fidelity, z_shape)
+            if not use_reference:
+                args = None, reference_fidelity, z_shape
+            elif z_ref is not None:
+                args = z_ref, reference_fidelity, z_shape
+            else:
+                args = self._get_z(res.image), reference_fidelity, z_shape
+            z, size = get_z_info_from(*args)
+            # adjust ControlNet parameters
+            crop_controlnet(kwargs, res.crop_res)
             # core
             sampled = self.sample(
                 num_samples,
                 export_path,
                 seed=seed,
                 z=z,
                 z_ref=z_ref,
                 z_ref_mask=z_ref_mask,
                 z_ref_noise=z_ref_noise,
                 size=size,  # type: ignore
-                original_size=res.image_res.original_size,
+                original_size=res.original_size,
                 alpha=None,
                 cond=txt_list,
                 cond_concat=torch.cat([res.mask_cond, res.remained_image_cond], dim=1),
                 num_steps=num_steps,
                 clip_output=clip_output,
                 callback=callback,
                 verbose=verbose,
                 **kwargs,
             )
+            if res.crop_res is not None:
+                sampled = recover_with(
+                    res.original_image,
+                    sampled,
+                    res.crop_res,
+                    res.wh_ratio,
+                    inpainting_settings,
+                )
         if keep_original:
-            original = res.image_res.original
-            sampled = paste_original(original, res.mask_res.original, sampled)
+            sampled = paste_original(res.original_image, res.original_mask, sampled)
         return sampled
 
     def outpainting(
         self,
         txt: str,
         image: Union[str, Image.Image],
         export_path: Optional[str] = None,
@@ -888,34 +1179,34 @@
             lambda remained_mask, img: np.where(remained_mask, img, 0.0),
             lambda bool_mask: torch.where(torch.from_numpy(bool_mask), 1.0, -1.0),
         )
         cond = torch.cat([res.remained_image_cond, res.mask_cond], dim=1)
         size = self._get_identical_size_with(res.remained_image_cond)
         # refine with img2img
         if refine_fidelity is not None:
-            z = self._get_z(res.image_res.image)
+            z = self._get_z(res.image)
             return self._img2img(
                 z,
                 export_path,
                 fidelity=refine_fidelity,
-                original_size=res.image_res.original_size,
-                alpha=res.image_res.alpha if alpha is None else alpha,
+                original_size=res.original_size,
+                alpha=res.image_alpha if alpha is None else alpha,
                 cond=cond,
                 num_steps=num_steps,
                 clip_output=clip_output,
                 verbose=verbose,
                 **kwargs,
             )
         # sampling
         return self.sample(
             1,
             export_path,
             size=size,  # type: ignore
-            original_size=res.image_res.original_size,
-            alpha=res.image_res.alpha if alpha is None else alpha,
+            original_size=res.original_size,
+            alpha=res.image_alpha if alpha is None else alpha,
             cond=cond,
             num_steps=num_steps,
             clip_output=clip_output,
             callback=callback,
             verbose=verbose,
             **kwargs,
         )
@@ -1079,22 +1370,23 @@
         use_half: bool = False,
     ) -> T:
         return cls.from_pipeline(ldm_sd(), device, use_amp=use_amp, use_half=use_half)
 
     @classmethod
     def from_sd_version(
         cls: Type[T],
-        version: SDVersions,
+        version: str,
         device: Optional[str] = None,
         *,
         use_amp: bool = False,
         use_half: bool = False,
+        **kw: Any,
     ) -> T:
         m = ldm_sd_tag(get_sd_tag(version))
-        return cls.from_pipeline(m, device, use_amp=use_amp, use_half=use_half)
+        return cls.from_pipeline(m, device, use_amp=use_amp, use_half=use_half, **kw)
 
     @classmethod
     def from_sd_anime(
         cls: Type[T],
         device: Optional[str] = None,
         *,
         use_amp: bool = False,
@@ -1106,17 +1398,18 @@
     @classmethod
     def from_sd_inpainting(
         cls: Type[T],
         device: Optional[str] = None,
         *,
         use_amp: bool = False,
         use_half: bool = False,
+        **kw: Any,
     ) -> T:
         m = ldm_sd_inpainting()
-        return cls.from_pipeline(m, device, use_amp=use_amp, use_half=use_half)
+        return cls.from_pipeline(m, device, use_amp=use_amp, use_half=use_half, **kw)
 
     @classmethod
     def from_sd_v2(
         cls: Type[T],
         device: Optional[str] = None,
         *,
         use_amp: bool = False,
@@ -1258,51 +1551,59 @@
         self,
         image: Union[str, Image.Image],
         mask: Union[str, Image.Image],
         max_wh: int,
         anchor: int,
         mask_image_fn: Callable[[np.ndarray, np.ndarray], np.ndarray],
         mask_cond_fn: Callable[[np.ndarray], Tensor],
+        inpainting_settings: Optional[InpaintingSettings] = None,
     ) -> MaskedCond:
         # handle mask stuffs
         image_res = read_image(image, max_wh, anchor=anchor)
         mask_res = read_image(mask, max_wh, anchor=anchor, to_mask=True)
-        mask = mask_res.image
-        bool_mask = np.round(mask) >= 0.5
+        cropped_res = get_cropped(image_res, mask_res, inpainting_settings)
+        c_image = cropped_res.image
+        c_mask = cropped_res.mask
+        bool_mask = np.round(c_mask) >= 0.5
         remained_mask = (~bool_mask).astype(np.float16 if self.use_half else np.float32)
-        remained_image = mask_image_fn(remained_mask, image_res.image)
+        remained_image = mask_image_fn(remained_mask, c_image)
         # construct condition tensor
         remained_cond = self._get_z(remained_image)
         latent_shape = remained_cond.shape[-2:]
         mask_cond = mask_cond_fn(bool_mask).to(torch.float32)
         mask_cond = F.interpolate(mask_cond, size=latent_shape)
         if self.use_half:
             mask_cond = mask_cond.half()
         mask_cond = mask_cond.to(self.device)
         return MaskedCond(
-            image_res,
-            mask_res,
-            mask,
-            remained_image,
-            remained_mask,
+            c_image,
+            c_mask,
             mask_cond,
             remained_cond,
+            remained_image,
+            remained_mask,
+            image_res.alpha,
+            image_res.original_size,
+            image_res.original,
+            mask_res.original,
+            cropped_res.wh_ratio,
+            cropped_res.crop_res,
         )
 
     def _q_sample(
         self,
         z: Tensor,
         num_steps: Optional[int],
         fidelity: float,
         seed: Optional[int],
         variations: Optional[List[Tuple[int, float]]] = None,
         variation_seed: Optional[int] = None,
         variation_strength: Optional[float] = None,
         **kwargs: Any,
-    ) -> Tuple[Tensor, Tensor, Dict[str, Any]]:
+    ) -> Tuple[Tensor, Tensor, int]:
         if num_steps is None:
             num_steps = self.sampler.default_steps
         t = min(num_steps, round((1.0 - fidelity) * (num_steps + 1)))
         ts = get_timesteps(t, 1, z.device)
         if isinstance(self.sampler, (DDIMMixin, KSamplerMixin, DPMSolver)):
             kw = shallow_copy_dict(self.sampler.sample_kwargs)
             kw["total_step"] = num_steps
@@ -1311,16 +1612,16 @@
             seed,
             lambda: torch.randn_like(z),
             lambda noise_: self.sampler.q_sample(z, ts, noise_),
             variations,
             variation_seed,
             variation_strength,
         )
-        kwargs["start_step"] = num_steps - t
-        return z, noise, kwargs
+        start_step = num_steps - t
+        return z, noise, start_step
 
     def _img2img(
         self,
         z: Tensor,
         export_path: Optional[str] = None,
         *,
         z_ref: Optional[Tensor] = None,
@@ -1330,15 +1631,16 @@
         cond: Optional[Any] = None,
         num_steps: Optional[int] = None,
         clip_output: bool = True,
         verbose: bool = True,
         **kwargs: Any,
     ) -> Tensor:
         with switch_sampler_context(self, kwargs.get("sampler")):
-            z, noise, kwargs = self._q_sample(z, num_steps, **kwargs)
+            z, noise, start_step = self._q_sample(z, num_steps, **kwargs)
+            kwargs["start_step"] = start_step
             return self.sample(
                 z.shape[0],
                 export_path,
                 z=z,
                 z_ref=z_ref,
                 z_ref_mask=z_ref_mask,
                 z_ref_noise=None if z_ref is None else noise,
@@ -1387,14 +1689,16 @@
         if mk is None:
             continue
         mv = base_md[mk].to(v)
         # inpainting workaround
         if k == "input_blocks.0.0.weight" and mv.shape[1] == 9:
             mv = mv[:, :4]
         nd[k] = v + mv
+    nd = {k: v.cpu() for k, v in nd.items()}
+    torch.cuda.empty_cache()
     return nd
 
 
 class ControlNetHints(str, Enum):
     DEPTH = "depth"
     CANNY = "canny"
     POSE = "pose"
@@ -1474,15 +1778,15 @@
     ) -> np.ndarray:
         return self.m(uint8_rgb, value_threshold, distance_threshold)
 
 
 class ControlledDiffusionAPI(DiffusionAPI):
     loaded: Dict[ControlNetHints, bool]
     annotators: Dict[ControlNetHints, Annotator]
-    base_sd_versions: Dict[ControlNetHints, SDVersions]
+    base_sd_versions: Dict[ControlNetHints, str]
     controlnet_weights: Dict[ControlNetHints, tensor_dict_type]
 
     control_defaults = {
         ControlNetHints.DEPTH: "ldm.sd_v1.5.control.diff.depth",
         ControlNetHints.CANNY: "ldm.sd_v1.5.control.diff.canny",
         ControlNetHints.POSE: "ldm.sd_v1.5.control.diff.pose",
         ControlNetHints.MLSD: "ldm.sd_v1.5.control.diff.mlsd",
@@ -1500,25 +1804,29 @@
         device: torch.device,
         *,
         use_amp: bool = False,
         use_half: bool = False,
         clip_skip: int = 0,
         hint_channels: int = 3,
         num_pool: int = 4,
+        lazy: bool = False,
     ):
         super().__init__(
             m,
             device,
             use_amp=use_amp,
             use_half=use_half,
             clip_skip=clip_skip,
         )
         pool = sorted(self.control_defaults)
         selected_pool = pool[: min(num_pool, len(pool))]
-        self.m.make_control_net({k: hint_channels for k in selected_pool})
+        self.lazy = lazy
+        self.m.make_control_net({k: hint_channels for k in selected_pool}, lazy)
+        assert self.m.control_model is not None
+        freeze(self.m.control_model)
         self.loaded = {k: False for k in selected_pool}
         self.annotators = {}
         self.num_pool = num_pool
         self.control_model = self.m.control_model
         self.base_sd_versions = {}
         self.controlnet_weights = {}
 
@@ -1527,17 +1835,17 @@
         device: torch.device,
         *,
         use_amp: bool = False,
         use_half: bool = False,
         no_annotator: bool = False,
     ) -> None:
         super().to(device, use_amp=use_amp, use_half=use_half)
-        if not no_annotator:
+        if not no_annotator and not self.lazy:
             for annotator in self.annotators.values():
-                annotator = annotator.to(device, use_half=use_half)
+                self._annotator_to(annotator)
 
     @property
     def available_control_hints(self) -> List[ControlNetHints]:
         return list(self.controlnet_weights)
 
     def set_tome_info(self, tome_info: Optional[Dict[str, Any]]) -> None:
         super().set_tome_info(tome_info)
@@ -1619,16 +1927,19 @@
                     self.base_sd_versions[hint] = self.current_sd_version
 
     def prepare_annotator(self, hint: ControlNetHints) -> None:
         if hint not in self.annotators:
             annotator_class = self.annotator_classes.get(hint)
             if annotator_class is None:
                 raise ValueError(f"annotator for '{hint}' is not implemented")
-            annotator = annotator_class(self.device)
-            annotator = annotator.to(self.device, use_half=self.use_half)
+            if self.lazy:
+                annotator = annotator_class("cpu")
+            else:
+                annotator = annotator_class(self.device)
+                self._annotator_to(annotator)
             self.annotators[hint] = annotator
 
     def prepare_annotators(self) -> None:
         for hint in self.controlnet_weights:
             self.prepare_annotator(hint)
 
     def get_hint_of(
@@ -1641,28 +1952,41 @@
             raise ValueError(f"'{hint}' is not loaded yet, please call `switch` first.")
         annotator = self.annotators.get(hint)
         if annotator is None:
             raise ValueError(
                 f"annotator for '{hint}' is not prepared yet, "
                 "please call `prepare_annotator`/`prepare_annotators` first."
             )
+        if self.lazy:
+            self._annotator_to(annotator)
         kwargs["uint8_rgb"] = uint8_rgb
         out = safe_execute(annotator.annotate, kwargs)
         if len(out.shape) == 2:
             out = out[..., None]
         if out.shape[-1] == 1:
             out = np.repeat(out, 3, axis=2)
+        if self.lazy:
+            self._annotator_to(annotator, "cpu")
         return out
 
     def enable_control(self) -> None:
         self.m.control_model = self.control_model
 
     def disable_control(self) -> None:
         self.m.control_model = None
 
+    # internal
+
+    def _annotator_to(self, annotator: Annotator, device: Optional[str] = None) -> None:
+        if device is None:
+            device = self.device
+        annotator.to(device, use_half=self.use_half)
+
 
 __all__ = [
     "SDVersions",
+    "InpaintingMode",
+    "InpaintingSettings",
     "DiffusionAPI",
     "ControlNetHints",
     "ControlledDiffusionAPI",
 ]
```

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/blip.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/blip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/api.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/inference/predictor.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/inference/predictor.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/inference/transforms.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/inference/transforms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/mconfigs/backboned.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/mconfigs/base.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/mconfigs/base.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/deeplab.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/hrnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/backboned/ih_model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/dih_model.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/dih_model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/iseunet_v1.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/base/ssam_model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/basic_blocks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/conv_autoencoder.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/deeplab_v3.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/hrnet_ocr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/ocr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/resnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/resnetv1b.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/modeling/unet.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/modeling/unet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/iharm/model/ops.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/iharm/model/ops.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/isnet.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/isnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/lama.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/lama.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/api.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/blocks.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/blocks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/dpt_depth.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/midas_net.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/midas_net.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/midas_net_custom.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/transforms.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/transforms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/core/vit.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/core/vit.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/midas/utils.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/midas/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/api.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/mlsd/utils.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/api.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/body.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/body.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/hand.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/hand.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/model.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/model.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/openpose/util.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/openpose/util.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/third_party/prompt.py` & `carefree-learn-0.4.5/cflearn/api/cv/third_party/prompt.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/cv/translator.py` & `carefree-learn-0.4.5/cflearn/api/cv/translator.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/ml/ddr.py` & `carefree-learn-0.4.5/cflearn/api/ml/ddr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/schema.py` & `carefree-learn-0.4.5/cflearn/api/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/utils.py` & `carefree-learn-0.4.5/cflearn/api/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/api/zoo/__init__.py` & `carefree-learn-0.4.5/cflearn/api/zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/callbacks/classification.py` & `carefree-learn-0.4.5/cflearn/callbacks/classification.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/callbacks/general.py` & `carefree-learn-0.4.5/cflearn/callbacks/general.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/callbacks/generator.py` & `carefree-learn-0.4.5/cflearn/callbacks/generator.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/constants.py` & `carefree-learn-0.4.5/cflearn/constants.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/array.py` & `carefree-learn-0.4.5/cflearn/data/array.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/blocks/cv/crop.py` & `carefree-learn-0.4.5/cflearn/data/blocks/cv/crop.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/blocks/cv/image_folder.py` & `carefree-learn-0.4.5/cflearn/data/blocks/cv/image_folder.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/blocks/cv/normalize.py` & `carefree-learn-0.4.5/cflearn/data/blocks/cv/normalize.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/blocks/cv/to_numpy.py` & `carefree-learn-0.4.5/cflearn/data/blocks/cv/to_numpy.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/blocks/cv/tuple_to_batch.py` & `carefree-learn-0.4.5/cflearn/data/blocks/cv/tuple_to_batch.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/blocks/ml/file.py` & `carefree-learn-0.4.5/cflearn/data/blocks/ml/file.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/blocks/ml/gather.py` & `carefree-learn-0.4.5/cflearn/data/blocks/ml/gather.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/blocks/ml/nan_handler.py` & `carefree-learn-0.4.5/cflearn/data/blocks/ml/nan_handler.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/blocks/ml/preprocessor.py` & `carefree-learn-0.4.5/cflearn/data/blocks/ml/preprocessor.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/blocks/ml/recognizer.py` & `carefree-learn-0.4.5/cflearn/data/blocks/ml/recognizer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/blocks/ml/splitter.py` & `carefree-learn-0.4.5/cflearn/data/blocks/ml/splitter.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/ml/api.py` & `carefree-learn-0.4.5/cflearn/data/ml/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/ml/datasets.py` & `carefree-learn-0.4.5/cflearn/data/ml/datasets.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/pytorch/api.py` & `carefree-learn-0.4.5/cflearn/data/pytorch/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/pytorch/datasets.py` & `carefree-learn-0.4.5/cflearn/data/pytorch/datasets.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/data/utils.py` & `carefree-learn-0.4.5/cflearn/data/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/dist/ml/experiment.py` & `carefree-learn-0.4.5/cflearn/dist/ml/experiment.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/dist/ml/runs/_utils.py` & `carefree-learn-0.4.5/cflearn/dist/ml/runs/_utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/dist/ml/task.py` & `carefree-learn-0.4.5/cflearn/dist/ml/task.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/inference.py` & `carefree-learn-0.4.5/cflearn/inference.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/losses/basic.py` & `carefree-learn-0.4.5/cflearn/losses/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/losses/gan.py` & `carefree-learn-0.4.5/cflearn/losses/gan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/losses/lpips.py` & `carefree-learn-0.4.5/cflearn/losses/lpips.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/losses/vae.py` & `carefree-learn-0.4.5/cflearn/losses/vae.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/metrics.py` & `carefree-learn-0.4.5/cflearn/metrics.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/misc/available.json` & `carefree-learn-0.4.5/cflearn/misc/available.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/misc/mixins.py` & `carefree-learn-0.4.5/cflearn/misc/mixins.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/misc/toolkit.py` & `carefree-learn-0.4.5/cflearn/misc/toolkit.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/bases.py` & `carefree-learn-0.4.5/cflearn/models/bases.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/ae/common.py` & `carefree-learn-0.4.5/cflearn/models/cv/ae/common.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/ae/kl.py` & `carefree-learn-0.4.5/cflearn/models/cv/ae/kl.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/ae/vq.py` & `carefree-learn-0.4.5/cflearn/models/cv/ae/vq.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/classifier/vanilla.py` & `carefree-learn-0.4.5/cflearn/models/cv/classifier/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/decoder/attn.py` & `carefree-learn-0.4.5/cflearn/models/cv/decoder/attn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/decoder/schema.py` & `carefree-learn-0.4.5/cflearn/models/cv/decoder/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/decoder/style_gan.py` & `carefree-learn-0.4.5/cflearn/models/cv/decoder/style_gan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/decoder/style_gan_v2.py` & `carefree-learn-0.4.5/cflearn/models/cv/decoder/style_gan_v2.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/decoder/vanilla.py` & `carefree-learn-0.4.5/cflearn/models/cv/decoder/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/decoder/vqgan.py` & `carefree-learn-0.4.5/cflearn/models/cv/decoder/vqgan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/clip.py` & `carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/rescaler.py` & `carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/rescaler.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/diffusion/cond_models/schema.py` & `carefree-learn-0.4.5/cflearn/models/cv/diffusion/cond_models/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/diffusion/ddpm.py` & `carefree-learn-0.4.5/cflearn/models/cv/diffusion/ddpm.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Tuple
 from typing import Union
 from typing import Callable
 from typing import Optional
+from typing import ContextManager
 from cftool.misc import safe_execute
 from cftool.misc import shallow_copy_dict
 from cftool.array import to_torch
 from cftool.types import tensor_dict_type
 
 from .unet import ControlNet
 from .unet import UNetDiffuser
@@ -172,14 +173,15 @@
     cond_key = "cond"
     noise_key = "noise"
     timesteps_key = "timesteps"
     identity_condition_model = "identity"
 
     sampler: ISampler
     control_model: Optional[Union[ControlNet, nn.ModuleDict]]
+    control_model_lazy: bool
     control_scales: Optional[Union[List[float], List[List[float]]]]
 
     def __init__(
         self,
         img_size: int,
         # unet
         in_channels: int,
@@ -260,14 +262,15 @@
             use_checkpoint=use_checkpoint,
             attn_split_chunk=attn_split_chunk,
             tome_info=tome_info,
         )
         self.unet = UNetDiffuser(out_channels=out_channels, **self.unet_kw)  # type: ignore
         # ControlNet
         self.control_model = None
+        self.control_model_lazy = False
         self.only_mid_control = only_mid_control
         self.num_control_scales = len(self.unet.output_blocks) + 1
         self.control_scales = None
         # ema
         if ema_decay is None:
             self.unet_ema = None
         else:
@@ -403,22 +406,23 @@
         *,
         cond: Optional[Any] = None,
         num_steps: Optional[int] = None,
         start_step: Optional[int] = None,
         verbose: bool = True,
         **kwargs: Any,
     ) -> Tensor:
-        return self.sampler.sample(
-            z,
-            cond=cond,
-            num_steps=num_steps,
-            start_step=start_step,
-            verbose=verbose,
-            **kwargs,
-        )
+        with self._control_model_context():
+            return self.sampler.sample(
+                z,
+                cond=cond,
+                num_steps=num_steps,
+                start_step=start_step,
+                verbose=verbose,
+                **kwargs,
+            )
 
     def sample(
         self,
         num_samples: int,
         *,
         cond: Optional[Any] = None,
         num_steps: Optional[int] = None,
@@ -572,33 +576,37 @@
     ) -> Tensor:
         num_dim = image.ndim
         return (
             extract_to(self.sqrt_alphas_cumprod, ts, num_dim) * image
             - extract_to(self.sqrt_one_minus_alphas_cumprod, ts, num_dim) * v
         )
 
-    def make_control_net(self, hint_channels: Union[int, Dict[str, int]]) -> None:
+    def make_control_net(
+        self,
+        hint_channels: Union[int, Dict[str, int]],
+        lazy: bool = False,
+    ) -> None:
         def _make(n: int) -> ControlNet:
             # temporarily make inpainting compatible
             kw = shallow_copy_dict(self.unet_kw)
             kw["in_channels"] = 4
-            dtype = list(self.unet.parameters())[0].dtype
-            control_model = ControlNet(hint_channels=n, **kw)  # type: ignore
-            control_model = control_model.to(get_device(self), dtype=dtype)
-            return control_model
+            return ControlNet(hint_channels=n, **kw)  # type: ignore
 
+        self.control_model_lazy = lazy
         if isinstance(hint_channels, int):
             self.control_model = _make(hint_channels)
         else:
             self.control_model = nn.ModuleDict(
                 {
                     key: _make(key_channels)
                     for key, key_channels in hint_channels.items()
                 }
             )
+        if not lazy:
+            self._control_model_to()
 
     def rename_control_net(self, old: str, new: str) -> None:
         if not isinstance(self.control_model, nn.ModuleDict):
             msg = "`rename_control_net` is only available when multiple `ControlNet` are used"
             raise ValueError(msg)
         if old not in self.control_model:
             raise ValueError(f"cannot find '{old}' in current models")
@@ -617,14 +625,39 @@
         if self.control_model is not None:
             self.control_model.to("cpu")
             del self.control_model
             self.control_model = None
 
     # internal
 
+    def _control_model_to(self, device: Optional[str] = None) -> None:
+        if self.control_model is not None:
+            p = list(self.unet.parameters())[0]
+            if device is None:
+                device = p.device
+            dtype = p.dtype
+            self.control_model.to(device, dtype=dtype)
+
+    def _control_model_context(self) -> ContextManager:
+        class _:
+            def __init__(self, m: DDPM):
+                self.m = m.control_model
+                self.lazy = m.control_model_lazy
+                self.to = m._control_model_to
+
+            def __enter__(self) -> None:
+                if self.m is not None and self.lazy:
+                    self.to()
+
+            def __exit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> None:
+                if self.m is not None and self.lazy:
+                    self.to("cpu")
+
+        return _(self)
+
     def _q_sample(
         self,
         net: Tensor,
         timesteps: Tensor,
         noise: Optional[Tensor] = None,
     ) -> Tensor:
         return self.q_sampler.q_sample(net, timesteps, noise)
```

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/diffusion/ldm.py` & `carefree-learn-0.4.5/cflearn/models/cv/diffusion/ldm.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/basic.py` & `carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/ddim.py` & `carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/ddim.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/k_samplers.py` & `carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/k_samplers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/plms.py` & `carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/plms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/schema.py` & `carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/solver.py` & `carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/solver.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/diffusion/samplers/utils.py` & `carefree-learn-0.4.5/cflearn/models/cv/diffusion/samplers/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/diffusion/unet.py` & `carefree-learn-0.4.5/cflearn/models/cv/diffusion/unet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/diffusion/utils.py` & `carefree-learn-0.4.5/cflearn/models/cv/diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/encoder/attn.py` & `carefree-learn-0.4.5/cflearn/models/cv/encoder/attn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/api.py` & `carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/core.py` & `carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/resnet.py` & `carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/resnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/transformer.py` & `carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/transformer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/models/vgg.py` & `carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/models/vgg.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/encoder/backbone/register.py` & `carefree-learn-0.4.5/cflearn/models/cv/encoder/backbone/register.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/encoder/fnet.py` & `carefree-learn-0.4.5/cflearn/models/cv/encoder/fnet.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/encoder/mixer.py` & `carefree-learn-0.4.5/cflearn/models/cv/encoder/mixer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/encoder/perceiver.py` & `carefree-learn-0.4.5/cflearn/models/cv/encoder/perceiver.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/encoder/pool_former.py` & `carefree-learn-0.4.5/cflearn/models/cv/encoder/pool_former.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/encoder/schema.py` & `carefree-learn-0.4.5/cflearn/models/cv/encoder/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/encoder/transformer.py` & `carefree-learn-0.4.5/cflearn/models/cv/encoder/transformer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/encoder/vanilla.py` & `carefree-learn-0.4.5/cflearn/models/cv/encoder/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/encoder/vqgan.py` & `carefree-learn-0.4.5/cflearn/models/cv/encoder/vqgan.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/gan/discriminators.py` & `carefree-learn-0.4.5/cflearn/models/cv/gan/discriminators.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/gan/schema.py` & `carefree-learn-0.4.5/cflearn/models/cv/gan/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/gan/vanilla.py` & `carefree-learn-0.4.5/cflearn/models/cv/gan/vanilla.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/general.py` & `carefree-learn-0.4.5/cflearn/models/cv/general.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/cv/translator/rrdb.py` & `carefree-learn-0.4.5/cflearn/models/cv/translator/rrdb.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/implicit/siren.py` & `carefree-learn-0.4.5/cflearn/models/implicit/siren.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/ml/base.py` & `carefree-learn-0.4.5/cflearn/models/ml/base.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/ml/ddr.py` & `carefree-learn-0.4.5/cflearn/models/ml/ddr.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/ml/encoders.py` & `carefree-learn-0.4.5/cflearn/models/ml/encoders.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/ml/fcnn.py` & `carefree-learn-0.4.5/cflearn/models/ml/fcnn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/ml/linear.py` & `carefree-learn-0.4.5/cflearn/models/ml/linear.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/ml/mixed_stacked.py` & `carefree-learn-0.4.5/cflearn/models/ml/mixed_stacked.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/ml/nbm.py` & `carefree-learn-0.4.5/cflearn/models/ml/nbm.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/ml/ndt.py` & `carefree-learn-0.4.5/cflearn/models/ml/ndt.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/ml/rnn.py` & `carefree-learn-0.4.5/cflearn/models/ml/rnn.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/ml/wnd.py` & `carefree-learn-0.4.5/cflearn/models/ml/wnd.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/multimodal/clip.py` & `carefree-learn-0.4.5/cflearn/models/multimodal/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/multimodal/schema.py` & `carefree-learn-0.4.5/cflearn/models/multimodal/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/nlp/encoder/transformer.py` & `carefree-learn-0.4.5/cflearn/models/nlp/encoder/transformer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/nlp/tokenizers/clip.py` & `carefree-learn-0.4.5/cflearn/models/nlp/tokenizers/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/nlp/tokenizers/schema.py` & `carefree-learn-0.4.5/cflearn/models/nlp/tokenizers/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/nlp/transformers/core.py` & `carefree-learn-0.4.5/cflearn/models/nlp/transformers/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/nlp/transformers/opus.py` & `carefree-learn-0.4.5/cflearn/models/nlp/transformers/opus.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/nlp/transformers/simbert.py` & `carefree-learn-0.4.5/cflearn/models/nlp/transformers/simbert.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/schemas/custom.py` & `carefree-learn-0.4.5/cflearn/models/schemas/custom.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/models/schemas/cv.py` & `carefree-learn-0.4.5/cflearn/models/schemas/cv.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/__init__.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/activations.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/activations.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/attentions.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/attentions.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/common.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/common.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/convs/basic.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/convs/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/convs/residual.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/convs/residual.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/customs.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/customs.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/high_level.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/high_level.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/hijacks.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/hijacks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/hooks.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/hooks.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/implementations/perceiver.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/implementations/perceiver.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/mappings.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/mappings.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/api.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/channel_mixers.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/channel_mixers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/poolers.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/poolers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/schema.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/mixed_stacks/token_mixers.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/mixed_stacks/token_mixers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/norms.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/norms.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/blocks/utils.py` & `carefree-learn-0.4.5/cflearn/modules/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/optimizers.py` & `carefree-learn-0.4.5/cflearn/modules/optimizers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/modules/schedulers.py` & `carefree-learn-0.4.5/cflearn/modules/schedulers.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/monitors.py` & `carefree-learn-0.4.5/cflearn/monitors.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/parameters.py` & `carefree-learn-0.4.5/cflearn/parameters.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 from typing import Any
 from typing import Dict
 from cftool.misc import OPTBase
 
 
 class OPTClass(OPTBase):
     cache_dir: str
+    external_dir: str
     meta_settings: Dict[str, Any]
 
     @property
     def env_key(self) -> str:
         return "CFLEARN_ENV"
 
     @property
     def defaults(self) -> Dict[str, Any]:
         return dict(
             cache_dir=os.path.join(os.path.expanduser("~"), ".cache", "carefree-learn"),
+            external_dir=os.path.join(os.path.expanduser("~"), ".cache", "external"),
             meta_settings={},
         )
 
     @property
     def data_cache_dir(self) -> str:
         return os.path.join(self.cache_dir, "data")
```

### Comparing `carefree-learn-0.4.4/cflearn/pipeline/api.py` & `carefree-learn-0.4.5/cflearn/pipeline/api.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/pipeline/blocks/basic.py` & `carefree-learn-0.4.5/cflearn/pipeline/blocks/basic.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/pipeline/blocks/ml.py` & `carefree-learn-0.4.5/cflearn/pipeline/blocks/ml.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/pipeline/blocks/utils.py` & `carefree-learn-0.4.5/cflearn/pipeline/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/pipeline/core.py` & `carefree-learn-0.4.5/cflearn/pipeline/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/pipeline/third_party.py` & `carefree-learn-0.4.5/cflearn/pipeline/third_party.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/schema.py` & `carefree-learn-0.4.5/cflearn/schema.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/scripts/sd.py` & `carefree-learn-0.4.5/cflearn/scripts/sd.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/trainer.py` & `carefree-learn-0.4.5/cflearn/trainer.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/types.py` & `carefree-learn-0.4.5/cflearn/types.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/zoo/configs/ae/kl/f4.json` & `carefree-learn-0.4.5/cflearn/zoo/configs/ae/kl/f4.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ddpm/default.json` & `carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ddpm/default.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/default.json` & `carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/default.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/zoo/configs/diffusion/ldm/vq.json` & `carefree-learn-0.4.5/cflearn/zoo/configs/diffusion/ldm/vq.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/zoo/configs/multimodal/clip/chinese.json` & `carefree-learn-0.4.5/cflearn/zoo/configs/multimodal/clip/chinese.json`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/zoo/core.py` & `carefree-learn-0.4.5/cflearn/zoo/core.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/cflearn/zoo/models/clip.py` & `carefree-learn-0.4.5/cflearn/zoo/models/clip.py`

 * *Files identical despite different names*

### Comparing `carefree-learn-0.4.4/setup.py` & `carefree-learn-0.4.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 
 
-VERSION = "0.4.4"
+VERSION = "0.4.5"
 DESCRIPTION = "Deep Learning with PyTorch made easy"
 with open("README.md", encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 cv_requires = [
     "ftfy",
     "lmdb",
@@ -30,14 +30,15 @@
 ]
 
 setup(
     name="carefree-learn",
     version=VERSION,
     packages=find_packages(exclude=("tests",)),
     install_requires=[
+        "filelock",
         "accelerate",
         "safetensors",
         "carefree-toolkit>=0.3.5",
     ],
     extras_require={
         "onnx": onnx_requires,
         "cv": cv_requires,
```

