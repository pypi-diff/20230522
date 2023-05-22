# Comparing `tmp/controlnet_aux-0.0.3.tar.gz` & `tmp/controlnet_aux-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "controlnet_aux-0.0.3.tar", last modified: Fri Apr 14 17:21:27 2023, max compression
+gzip compressed data, was "controlnet_aux-0.0.4.tar", last modified: Mon May 22 20:32:50 2023, max compression
```

## Comparing `controlnet_aux-0.0.3.tar` & `controlnet_aux-0.0.4.tar`

### file list

```diff
@@ -1,103 +1,180 @@
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2958 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2054 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/README.md
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/setup.cfg
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8636 2023-04-14 17:12:42.000000 controlnet_aux-0.0.3/setup.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      394 2023-04-14 15:41:51.000000 controlnet_aux-0.0.3/src/controlnet_aux/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/canny/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      547 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/canny/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/hed/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7726 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/hed/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/lineart/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5057 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/lineart/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/lineart_anime/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7574 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/lineart_anime/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/midas/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2618 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5276 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/api.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/base_model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9242 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/blocks.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3154 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/dpt_depth.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/midas_net.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/midas_net_custom.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/transforms.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    14625 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/vit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4582 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/midas/utils.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/mlsd/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2170 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/mlsd/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/mlsd/models/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/mlsd/models/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9678 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9180 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    24134 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/mlsd/utils.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2517 2023-04-14 17:15:46.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      597 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/NNET.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:16:17.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2980 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/baseline.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:28.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    10480 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/decoder.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:38.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2428 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5993 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       89 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3000 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/dataset.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3113 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/loader.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     9187 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/tf_preprocessing.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4760 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/transforms.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      206 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4170 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2690 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2294 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4549 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3350 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    12093 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    26514 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    59925 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2833 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    15009 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      707 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       22 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2730 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5821 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2932 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      843 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4905 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1737 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1297 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6632 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     1060 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/encoder.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5703 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/submodules.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/utils/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:16:29.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/utils/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7570 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/utils/losses.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6725 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/normalbae/utils/utils.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/src/controlnet_aux/open_pose/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     5233 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/open_pose/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    10883 2023-04-14 09:59:01.000000 controlnet_aux-0.0.3/src/controlnet_aux/open_pose/body.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    15314 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/open_pose/face.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     6530 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/open_pose/hand.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     8743 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/open_pose/model.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     7934 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/open_pose/util.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/src/controlnet_aux/pidi/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2952 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/pidi/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)    21794 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/pidi/model.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.914428 controlnet_aux-0.0.3/src/controlnet_aux/shuffle/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3468 2023-04-14 15:40:08.000000 controlnet_aux-0.0.3/src/controlnet_aux/shuffle/__init__.py
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     3742 2023-04-11 17:22:02.000000 controlnet_aux-0.0.3/src/controlnet_aux/util.py
-drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:21:27.910428 controlnet_aux-0.0.3/src/controlnet_aux.egg-info/
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     2958 2023-04-14 17:21:27.000000 controlnet_aux-0.0.3/src/controlnet_aux.egg-info/PKG-INFO
--rw-rw-r--   0 patrick   (1000) patrick   (1000)     4410 2023-04-14 17:21:27.000000 controlnet_aux-0.0.3/src/controlnet_aux.egg-info/SOURCES.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-04-14 17:21:27.000000 controlnet_aux-0.0.3/src/controlnet_aux.egg-info/dependency_links.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)      120 2023-04-14 17:21:27.000000 controlnet_aux-0.0.3/src/controlnet_aux.egg-info/requires.txt
--rw-rw-r--   0 patrick   (1000) patrick   (1000)       15 2023-04-14 17:21:27.000000 controlnet_aux-0.0.3/src/controlnet_aux.egg-info/top_level.txt
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    11357 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/LICENSE.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3250 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2320 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/README.md
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       38 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/setup.cfg
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8756 2023-05-22 20:31:03.000000 controlnet_aux-0.0.4/setup.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.557665 controlnet_aux-0.0.4/src/
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      515 2023-05-22 20:31:09.000000 controlnet_aux-0.0.4/src/controlnet_aux/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/canny/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      547 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/canny/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/hed/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7994 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/hed/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/lineart/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5293 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/lineart/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/lineart_anime/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7718 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/lineart_anime/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/mediapipe_face/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      645 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/mediapipe_face/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6870 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/mediapipe_face/mediapipe_face_common.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/midas/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2992 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5276 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/api.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/base_model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9242 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/blocks.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3154 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/dpt_depth.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/midas_net.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/midas_net_custom.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/transforms.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    14625 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/vit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4582 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/midas/utils.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/mlsd/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2314 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/mlsd/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/mlsd/models/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/mlsd/models/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9678 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9180 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    24134 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/mlsd/utils.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2662 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      597 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/NNET.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:16:17.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2980 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/baseline.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:28.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    10480 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/decoder.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:18:38.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2428 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5993 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       89 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3000 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/dataset.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3113 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/loader.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     9187 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/tf_preprocessing.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4760 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/transforms.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      206 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4170 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2690 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2294 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4549 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3350 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12093 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    26514 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    59925 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2833 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    15009 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      707 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       22 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/version.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2730 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5821 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2932 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      843 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4905 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1737 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1297 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6632 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1060 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/encoder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5703 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/submodules.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/utils/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-04-14 17:16:29.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/utils/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7570 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/utils/losses.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6725 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/normalbae/utils/utils.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/open_pose/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5563 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/open_pose/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    10883 2023-04-14 09:59:01.000000 controlnet_aux-0.0.4/src/controlnet_aux/open_pose/body.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    15314 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/open_pose/face.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6530 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/open_pose/hand.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8743 2023-04-11 17:22:02.000000 controlnet_aux-0.0.4/src/controlnet_aux/open_pose/model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7934 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/open_pose/util.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/pidi/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2978 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/pidi/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    21794 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/pidi/model.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2502 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    15148 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/automatic_mask_generator.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2941 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/build_sam.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      385 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1479 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/common.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    14420 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/image_encoder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6615 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/mask_decoder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8594 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/prompt_encoder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7226 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/sam.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8397 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/modeling/transformer.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    11664 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/predictor.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/utils/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      197 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/utils/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12712 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/utils/amg.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5812 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/utils/onnx.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3972 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/segment_anything/utils/transforms.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/shuffle/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3468 2023-04-14 15:40:08.000000 controlnet_aux-0.0.4/src/controlnet_aux/shuffle/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3890 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/util.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2192 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    15248 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    13757 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/hubconf.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        0 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6909 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/beit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3436 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/levit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1045 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/next_vit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      333 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      931 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin2.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1576 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/swin_common.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7284 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/utils.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6899 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/backbones/vit.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      367 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/base_model.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12792 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/blocks.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6099 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/dpt_depth.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2709 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     5207 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/midas_net_custom.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8552 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/model_loader.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7869 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/base_models/midas_repo/midas/transforms.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     2390 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/builder.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     7362 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/depth_model.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1153 2023-05-22 19:47:00.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8693 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/attractor.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4838 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/dist_layers.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     6733 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/localbins_layers.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     4163 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/layers/patch_transformer.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3438 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/model_io.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1270 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1587 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      556 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth/config_zoedepth_kitti.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    12630 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth/zoedepth_v1.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1276 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1968 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/config_zoedepth_nk.json
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    16363 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/models/zoedepth_nk/zoedepth_nk_v1.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     1154 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/__init__.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      624 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/arg_utils.py
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)    16310 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/config.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.565665 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/easydict/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3426 2023-04-20 08:19:12.000000 controlnet_aux-0.0.4/src/controlnet_aux/zoe/zoedepth/utils/easydict/__init__.py
+drwxrwxr-x   0 patrick   (1000) patrick   (1000)        0 2023-05-22 20:32:50.561665 controlnet_aux-0.0.4/src/controlnet_aux.egg-info/
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     3250 2023-05-22 20:32:50.000000 controlnet_aux-0.0.4/src/controlnet_aux.egg-info/PKG-INFO
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)     8351 2023-05-22 20:32:50.000000 controlnet_aux-0.0.4/src/controlnet_aux.egg-info/SOURCES.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)        1 2023-05-22 20:32:50.000000 controlnet_aux-0.0.4/src/controlnet_aux.egg-info/dependency_links.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)      120 2023-05-22 20:32:50.000000 controlnet_aux-0.0.4/src/controlnet_aux.egg-info/requires.txt
+-rw-rw-r--   0 patrick   (1000) patrick   (1000)       15 2023-05-22 20:32:50.000000 controlnet_aux-0.0.4/src/controlnet_aux.egg-info/top_level.txt
```

### Comparing `controlnet_aux-0.0.3/PKG-INFO` & `controlnet_aux-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: controlnet_aux
-Version: 0.0.3
+Version: 0.0.4
 Summary: Human Pose
 Home-page: https://github.com/patrickvonplaten/controlnet_aux
 Author: The HuggingFace team
 Author-email: patrick@huggingface.co
 License: Apache
 Keywords: deep learning
 Platform: UNKNOWN
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 # ControlNet auxiliary models
 
 This is a PyPi installable package of [lllyasviel's ControlNet Annotators](https://github.com/lllyasviel/ControlNet/tree/main/annotator)
 
 The code is copy-pasted from the respective folders in https://github.com/lllyasviel/ControlNet/tree/main/annotator and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
 
@@ -38,15 +39,15 @@
 
 ## Usage
 
 ```python
 from PIL import Image
 import requests
 from io import BytesIO
-from controlnet_aux import HEDdetector, MidasDetector, MLSDdetector, OpenposeDetector, PidiNetDetector, NormalBaeDetector, LineartDetector, LineartAnimeDetector, CannyDetector, ContentShuffleDetector
+from controlnet_aux import HEDdetector, MidasDetector, MLSDdetector, OpenposeDetector, PidiNetDetector, NormalBaeDetector, LineartDetector, LineartAnimeDetector, CannyDetector, ContentShuffleDetector, ZoeDetector, MediapipeFaceDetector, SamDetector
 
 # load image
 url = "https://huggingface.co/lllyasviel/sd-controlnet-openpose/resolve/main/images/pose.png"
 
 response = requests.get(url)
 img = Image.open(BytesIO(response.content)).convert("RGB").resize((512, 512))
 
@@ -55,28 +56,33 @@
 midas = MidasDetector.from_pretrained("lllyasviel/Annotators")
 mlsd = MLSDdetector.from_pretrained("lllyasviel/Annotators")
 open_pose = OpenposeDetector.from_pretrained("lllyasviel/Annotators")
 pidi = PidiNetDetector.from_pretrained("lllyasviel/Annotators")
 normal_bae = NormalBaeDetector.from_pretrained("lllyasviel/Annotators")
 lineart = LineartDetector.from_pretrained("lllyasviel/Annotators")
 lineart_anime = LineartAnimeDetector.from_pretrained("lllyasviel/Annotators")
+zoe = ZoeDetector.from_pretrained("lllyasviel/Annotators")
+sam = SamDetector("./weight_path")
 
 # instantiate
 canny = CannyDetector()
 content = ContentShuffleDetector()
+face_detector = MediapipeFaceDetector()
 
 
 # process
 processed_image_hed = hed(img)
 processed_image_midas = midas(img)
 processed_image_mlsd = mlsd(img)
 processed_image_open_pose = open_pose(img, hand_and_face=True)
 processed_image_pidi = pidi(img, safe=True)
 processed_image_normal_bae = normal_bae(img)
 processed_image_lineart = lineart(img, coarse=True)
 processed_image_lineart_anime = lineart_anime(img)
+processed_image_zoe = zoe(img)
 
 processed_image_canny = canny(img)
 processed_image_content = content(img)
+processed_image_mediapipe_face = face_detector(img)
 ```
```

### Comparing `controlnet_aux-0.0.3/README.md` & `controlnet_aux-0.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 ## Usage
 
 ```python
 from PIL import Image
 import requests
 from io import BytesIO
-from controlnet_aux import HEDdetector, MidasDetector, MLSDdetector, OpenposeDetector, PidiNetDetector, NormalBaeDetector, LineartDetector, LineartAnimeDetector, CannyDetector, ContentShuffleDetector
+from controlnet_aux import HEDdetector, MidasDetector, MLSDdetector, OpenposeDetector, PidiNetDetector, NormalBaeDetector, LineartDetector, LineartAnimeDetector, CannyDetector, ContentShuffleDetector, ZoeDetector, MediapipeFaceDetector, SamDetector
 
 # load image
 url = "https://huggingface.co/lllyasviel/sd-controlnet-openpose/resolve/main/images/pose.png"
 
 response = requests.get(url)
 img = Image.open(BytesIO(response.content)).convert("RGB").resize((512, 512))
 
@@ -31,26 +31,31 @@
 midas = MidasDetector.from_pretrained("lllyasviel/Annotators")
 mlsd = MLSDdetector.from_pretrained("lllyasviel/Annotators")
 open_pose = OpenposeDetector.from_pretrained("lllyasviel/Annotators")
 pidi = PidiNetDetector.from_pretrained("lllyasviel/Annotators")
 normal_bae = NormalBaeDetector.from_pretrained("lllyasviel/Annotators")
 lineart = LineartDetector.from_pretrained("lllyasviel/Annotators")
 lineart_anime = LineartAnimeDetector.from_pretrained("lllyasviel/Annotators")
+zoe = ZoeDetector.from_pretrained("lllyasviel/Annotators")
+sam = SamDetector("./weight_path")
 
 # instantiate
 canny = CannyDetector()
 content = ContentShuffleDetector()
+face_detector = MediapipeFaceDetector()
 
 
 # process
 processed_image_hed = hed(img)
 processed_image_midas = midas(img)
 processed_image_mlsd = mlsd(img)
 processed_image_open_pose = open_pose(img, hand_and_face=True)
 processed_image_pidi = pidi(img, safe=True)
 processed_image_normal_bae = normal_bae(img)
 processed_image_lineart = lineart(img, coarse=True)
 processed_image_lineart_anime = lineart_anime(img)
+processed_image_zoe = zoe(img)
 
 processed_image_canny = canny(img)
 processed_image_content = content(img)
+processed_image_mediapipe_face = face_detector(img)
 ```
```

### Comparing `controlnet_aux-0.0.3/setup.py` & `controlnet_aux-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     deps["torchvision"],
     deps["timm"],
     deps["scikit-image"],
 ]
 
 setup(
     name="controlnet_aux",
-    version="0.0.3",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+    version="0.0.4",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
     description="Human Pose",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="Apache",
     author="The HuggingFace team",
     author_email="patrick@huggingface.co",
@@ -206,14 +206,15 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     cmdclass={"deps_table_update": DepsTableUpdateCommand},
+    package_data={'controlnet_aux' : ['zoe/zoedepth/models/zoedepth/*.json', 'zoe/zoedepth/models/zoedepth_nk/*.json']}
 )
 
 # Release checklist
 # 1. Change the version in __init__.py and setup.py.
 # 2. Commit these changes with the message: "Release: Release"
 # 3. Add a tag in git to mark the release: "git tag RELEASE -m 'Adds tag RELEASE for pypi' "
 #    Push the tag to git: git push --tags origin main
```

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/canny/__init__.py` & `controlnet_aux-0.0.4/src/controlnet_aux/canny/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/hed/__init__.py` & `controlnet_aux-0.0.4/src/controlnet_aux/hed/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import cv2
 import os
 import torch
 from einops import rearrange
 from huggingface_hub import hf_hub_download
 from PIL import Image
 from ..open_pose.util import HWC3, resize_image
+from ..util import safe_step
 
 class Network(torch.nn.Module):
     def __init__(self, model_path):
         super().__init__()
 
         self.netVggOne = torch.nn.Sequential(
             torch.nn.Conv2d(in_channels=3, out_channels=64, kernel_size=3, stride=1, padding=1),
@@ -101,21 +102,24 @@
     @classmethod
     def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
         if pretrained_model_or_path == "lllyasviel/ControlNet":
             filename = filename or "annotator/ckpts/network-bsds500.pth"
         else:
             filename = filename or "network-bsds500.pth"
 
-        model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+        if os.path.isdir(pretrained_model_or_path):
+            model_path = os.path.join(pretrained_model_or_path, filename)
+        else:
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
 
         netNetwork = Network(model_path)
 
         return cls(netNetwork)
 
-    def __call__(self, input_image, detect_resolution=512, image_resolution=512, return_pil=True, scribble=False):
+    def __call__(self, input_image, detect_resolution=512, image_resolution=512, safe=False, return_pil=True, scribble=False):
         device = next(iter(self.netNetwork.parameters())).device
         if not isinstance(input_image, np.ndarray):
             input_image = np.array(input_image, dtype=np.uint8)
 
         input_image = HWC3(input_image)
         input_image = resize_image(input_image, detect_resolution)
 
@@ -123,16 +127,18 @@
         input_image = input_image[:, :, ::-1].copy()
         with torch.no_grad():
             image_hed = torch.from_numpy(input_image).float()
             image_hed = image_hed.to(device)
             image_hed = image_hed / 255.0
             image_hed = rearrange(image_hed, 'h w c -> 1 c h w')
             edge = self.netNetwork(image_hed)[0]
-            edge = (edge.cpu().numpy() * 255.0).clip(0, 255).astype(np.uint8)
-
+            edge = edge.cpu().numpy()
+            if safe:
+                edge = safe_step(edge)
+            edge = (edge * 255.0).clip(0, 255).astype(np.uint8)
 
         detected_map = edge[0]
 
         detected_map = HWC3(detected_map)
 
         img = resize_image(input_image, image_resolution)
         H, W, C = img.shape
```

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/lineart/__init__.py` & `controlnet_aux-0.0.4/src/controlnet_aux/lineart/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,16 +100,20 @@
             self.model_coarse.cuda()
 
     @classmethod
     def from_pretrained(cls, pretrained_model_or_path, filename=None, coarse_filename=None, cache_dir=None):
         filename = filename or "sk_model.pth"
         coarse_filename = coarse_filename or "sk_model2.pth"
 
-        model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
-        coarse_model_path = hf_hub_download(pretrained_model_or_path, coarse_filename, cache_dir=cache_dir)
+        if os.path.isdir(pretrained_model_or_path):
+            model_path = os.path.join(pretrained_model_or_path, filename)
+            coarse_model_path = os.path.join(pretrained_model_or_path, coarse_filename)
+        else:
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+            coarse_model_path = hf_hub_download(pretrained_model_or_path, coarse_filename, cache_dir=cache_dir)
 
         model = Generator(3, 1, 3)
         model.load_state_dict(torch.load(model_path, map_location=torch.device('cpu')))
 
         coarse_model = Generator(3, 1, 3)
         coarse_model.load_state_dict(torch.load(coarse_model_path, map_location=torch.device('cpu')))
```

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/lineart_anime/__init__.py` & `controlnet_aux-0.0.4/src/controlnet_aux/lineart_anime/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,18 @@
         if torch.cuda.is_available():
             self.model.cuda()
 
     @classmethod
     def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
         filename = filename or "netG.pth"
 
-        model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+        if os.path.isdir(pretrained_model_or_path):
+            model_path = os.path.join(pretrained_model_or_path, filename)
+        else:
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
 
         norm_layer = functools.partial(nn.InstanceNorm2d, affine=False, track_running_stats=False)
         net = UnetGenerator(3, 1, 8, 64, norm_layer=norm_layer, use_dropout=False)
         ckpt = torch.load(model_path)
         for key in list(ckpt.keys()):
             if 'module.' in key:
                 ckpt[key.replace('module.', '')] = ckpt[key]
```

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/midas/__init__.py` & `controlnet_aux-0.0.4/src/controlnet_aux/midas/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import cv2
 import numpy as np
 from PIL import Image
 import torch
+import os 
 
 from huggingface_hub import hf_hub_download
 from einops import rearrange
 from .api import MiDaSInference
 from ..util import HWC3
 
 class MidasDetector:
@@ -18,18 +19,22 @@
     @classmethod
     def from_pretrained(cls, pretrained_model_or_path, model_type="dpt_hybrid", filename=None, cache_dir=None):
         if pretrained_model_or_path == "lllyasviel/ControlNet":
             filename = filename or "annotator/ckpts/dpt_hybrid-midas-501f0c75.pt"
         else:
             filename = filename or "dpt_hybrid-midas-501f0c75.pt"
 
-        model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+        if os.path.isdir(pretrained_model_or_path):
+            model_path = os.path.join(pretrained_model_or_path, filename)
+        else:
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+
         return cls(model_type=model_type, model_path=model_path)
         
-    def __call__(self, input_image, a=np.pi * 2.0, bg_th=0.1):
+    def __call__(self, input_image, a=np.pi * 2.0, bg_th=0.1, depth_and_normal=False):
         
         input_type = "np"
         if isinstance(input_image, Image.Image):
             input_image = np.array(input_image)
             input_type = "pil"
             
         input_image = HWC3(input_image)
@@ -45,22 +50,27 @@
             depth_pt = depth.clone()
             depth_pt -= torch.min(depth_pt)
             depth_pt /= torch.max(depth_pt)
             depth_pt = depth_pt.cpu().numpy()
             depth_image = (depth_pt * 255.0).clip(0, 255).astype(np.uint8)
 
             depth_np = depth.cpu().numpy()
-            x = cv2.Sobel(depth_np, cv2.CV_32F, 1, 0, ksize=3)
-            y = cv2.Sobel(depth_np, cv2.CV_32F, 0, 1, ksize=3)
-            z = np.ones_like(x) * a
-            x[depth_pt < bg_th] = 0
-            y[depth_pt < bg_th] = 0
-            normal = np.stack([x, y, z], axis=2)
-            normal /= np.sum(normal ** 2.0, axis=2, keepdims=True) ** 0.5
-            normal_image = (normal * 127.5 + 127.5).clip(0, 255).astype(np.uint8)
+            if depth_and_normal:
+                x = cv2.Sobel(depth_np, cv2.CV_32F, 1, 0, ksize=3)
+                y = cv2.Sobel(depth_np, cv2.CV_32F, 0, 1, ksize=3)
+                z = np.ones_like(x) * a
+                x[depth_pt < bg_th] = 0
+                y[depth_pt < bg_th] = 0
+                normal = np.stack([x, y, z], axis=2)
+                normal /= np.sum(normal ** 2.0, axis=2, keepdims=True) ** 0.5
+                normal_image = (normal * 127.5 + 127.5).clip(0, 255).astype(np.uint8)
         
         if input_type == "pil":
             depth_image = Image.fromarray(depth_image)
             depth_image = depth_image.convert("RGB")
-            normal_image = Image.fromarray(normal_image)
+            if depth_and_normal:
+                normal_image = Image.fromarray(normal_image)
         
-        return depth_image
+        if depth_and_normal:
+            return depth_image, normal_image
+        else:
+            return depth_image
```

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/midas/api.py` & `controlnet_aux-0.0.4/src/controlnet_aux/midas/api.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/blocks.py` & `controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/blocks.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/dpt_depth.py` & `controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/dpt_depth.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/midas_net.py` & `controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/midas_net.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/midas_net_custom.py` & `controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/midas_net_custom.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/transforms.py` & `controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/midas/midas/vit.py` & `controlnet_aux-0.0.4/src/controlnet_aux/midas/midas/vit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/midas/utils.py` & `controlnet_aux-0.0.4/src/controlnet_aux/midas/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/mlsd/__init__.py` & `controlnet_aux-0.0.4/src/controlnet_aux/mlsd/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,18 @@
     @classmethod
     def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
         if pretrained_model_or_path == "lllyasviel/ControlNet":
             filename = filename or "annotator/ckpts/mlsd_large_512_fp32.pth"
         else:
             filename = filename or "mlsd_large_512_fp32.pth"
 
-        model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+        if os.path.isdir(pretrained_model_or_path):
+            model_path = os.path.join(pretrained_model_or_path, filename)
+        else:
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
 
         model = MobileV2_MLSD_Large()
         model.load_state_dict(torch.load(model_path), strict=True)
 
         return cls(model)
 
     def __call__(self, input_image, thr_v=0.1, thr_d=0.1, detect_resolution=512, image_resolution=512, return_pil=True):
```

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py` & `controlnet_aux-0.0.4/src/controlnet_aux/mlsd/models/mbv2_mlsd_large.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py` & `controlnet_aux-0.0.4/src/controlnet_aux/mlsd/models/mbv2_mlsd_tiny.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/mlsd/utils.py` & `controlnet_aux-0.0.4/src/controlnet_aux/mlsd/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/__init__.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,19 @@
             self.model.cuda()
 
         self.norm = transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225])
 
     @classmethod
     def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
         filename = filename or "scannet.pt"
-        model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+
+        if os.path.isdir(pretrained_model_or_path):
+            model_path = os.path.join(pretrained_model_or_path, filename)
+        else:
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
 
         args = types.SimpleNamespace()
         args.mode = 'client'
         args.architecture = 'BN'
         args.pretrained = 'scannet'
         args.sampling_ratio = 0.4
         args.importance_ratio = 0.7
```

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/NNET.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/NNET.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/baseline.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/baseline.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/decoder.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/decoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_benchmark.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/caffe2_validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/dataset.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/dataset.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/loader.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/loader.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/tf_preprocessing.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/tf_preprocessing.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/transforms.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/data/transforms.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_jit.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/activations/activations_me.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/config.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/conv2d_layers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/efficientnet_builder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/gen_efficientnet.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/helpers.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/geffnet/model_factory.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/hubconf.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_export.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_optimize.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_to_caffe.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/onnx_validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/setup.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/efficientnet_repo/validate.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/encoder.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/encoder.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/nets/submodules/submodules.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/nets/submodules/submodules.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/utils/losses.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/utils/losses.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/normalbae/utils/utils.py` & `controlnet_aux-0.0.4/src/controlnet_aux/normalbae/utils/utils.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/open_pose/__init__.py` & `controlnet_aux-0.0.4/src/controlnet_aux/open_pose/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,17 +56,22 @@
         else:
             filename = filename or "body_pose_model.pth"
             hand_filename = hand_filename or "hand_pose_model.pth"
             face_filename = face_filename or "facenet.pth"
 
             face_pretrained_model_or_path = pretrained_model_or_path
 
-        body_model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
-        hand_model_path = hf_hub_download(pretrained_model_or_path, hand_filename, cache_dir=cache_dir)
-        face_model_path = hf_hub_download(face_pretrained_model_or_path, face_filename, cache_dir=cache_dir)
+        if os.path.isdir(pretrained_model_or_path):
+            body_model_path = os.path.join(pretrained_model_or_path, filename)
+            hand_model_path = os.path.join(pretrained_model_or_path, hand_filename)
+            face_model_path = os.path.join(face_pretrained_model_or_path, face_filename)
+        else:
+            body_model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+            hand_model_path = hf_hub_download(pretrained_model_or_path, hand_filename, cache_dir=cache_dir)
+            face_model_path = hf_hub_download(face_pretrained_model_or_path, face_filename, cache_dir=cache_dir)
 
         body_estimation = Body(body_model_path)
         hand_estimation = Hand(hand_model_path)
         face_estimation = Face(face_model_path)
 
         return cls(body_estimation, hand_estimation, face_estimation)
```

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/open_pose/body.py` & `controlnet_aux-0.0.4/src/controlnet_aux/open_pose/body.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/open_pose/face.py` & `controlnet_aux-0.0.4/src/controlnet_aux/open_pose/face.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/open_pose/hand.py` & `controlnet_aux-0.0.4/src/controlnet_aux/open_pose/hand.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/open_pose/model.py` & `controlnet_aux-0.0.4/src/controlnet_aux/open_pose/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/open_pose/util.py` & `controlnet_aux-0.0.4/src/controlnet_aux/open_pose/util.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/pidi/__init__.py` & `controlnet_aux-0.0.4/src/controlnet_aux/pidi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,30 @@
 import torch
 import numpy as np
 from einops import rearrange
 import cv2
 from huggingface_hub import hf_hub_download
 from .model import pidinet
 from ..open_pose.util import HWC3, resize_image
+from ..util import safe_step
 from PIL import Image
 
 
-def safe_step(x, step=2):
-    y = x.astype(np.float32) * float(step + 1)
-    y = y.astype(np.int32).astype(np.float32) / float(step)
-    return y
-
-
 class PidiNetDetector:
     def __init__(self, netNetwork):
         self.netNetwork = netNetwork
 
     @classmethod
     def from_pretrained(cls, pretrained_model_or_path, filename=None, cache_dir=None):
         filename = filename or "table5_pidinet.pth"
-        model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
+
+        if os.path.isdir(pretrained_model_or_path):
+            model_path = os.path.join(pretrained_model_or_path, filename)
+        else:
+            model_path = hf_hub_download(pretrained_model_or_path, filename, cache_dir=cache_dir)
 
         netNetwork = pidinet()
         netNetwork.load_state_dict({k.replace('module.', ''): v for k, v in torch.load(model_path)['state_dict'].items()})
         netNetwork.eval()
 
         return cls(netNetwork)
```

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/pidi/model.py` & `controlnet_aux-0.0.4/src/controlnet_aux/pidi/model.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/shuffle/__init__.py` & `controlnet_aux-0.0.4/src/controlnet_aux/shuffle/__init__.py`

 * *Files identical despite different names*

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux/util.py` & `controlnet_aux-0.0.4/src/controlnet_aux/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,20 @@
     W *= k
     H = int(np.round(H / 64.0)) * 64
     W = int(np.round(W / 64.0)) * 64
     img = cv2.resize(input_image, (W, H), interpolation=cv2.INTER_LANCZOS4 if k > 1 else cv2.INTER_AREA)
     return img
 
 
+def safe_step(x, step=2):
+    y = x.astype(np.float32) * float(step + 1)
+    y = y.astype(np.int32).astype(np.float32) / float(step)
+    return y
+
+
 def ade_palette():
     """ADE20K palette that maps each class to RGB values."""
     return [[120, 120, 120], [180, 120, 120], [6, 230, 230], [80, 50, 50],
             [4, 200, 3], [120, 120, 80], [140, 140, 140], [204, 5, 255],
             [230, 230, 230], [4, 250, 7], [224, 5, 255], [235, 255, 7],
             [150, 5, 61], [120, 120, 70], [8, 255, 51], [255, 6, 82],
             [143, 255, 140], [204, 255, 4], [255, 51, 7], [204, 70, 3],
```

### Comparing `controlnet_aux-0.0.3/src/controlnet_aux.egg-info/PKG-INFO` & `controlnet_aux-0.0.4/src/controlnet_aux.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: controlnet-aux
-Version: 0.0.3
+Version: 0.0.4
 Summary: Human Pose
 Home-page: https://github.com/patrickvonplaten/controlnet_aux
 Author: The HuggingFace team
 Author-email: patrick@huggingface.co
 License: Apache
 Keywords: deep learning
 Platform: UNKNOWN
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
 
 # ControlNet auxiliary models
 
 This is a PyPi installable package of [lllyasviel's ControlNet Annotators](https://github.com/lllyasviel/ControlNet/tree/main/annotator)
 
 The code is copy-pasted from the respective folders in https://github.com/lllyasviel/ControlNet/tree/main/annotator and connected to [the 🤗 Hub](https://huggingface.co/lllyasviel/Annotators).
 
@@ -38,15 +39,15 @@
 
 ## Usage
 
 ```python
 from PIL import Image
 import requests
 from io import BytesIO
-from controlnet_aux import HEDdetector, MidasDetector, MLSDdetector, OpenposeDetector, PidiNetDetector, NormalBaeDetector, LineartDetector, LineartAnimeDetector, CannyDetector, ContentShuffleDetector
+from controlnet_aux import HEDdetector, MidasDetector, MLSDdetector, OpenposeDetector, PidiNetDetector, NormalBaeDetector, LineartDetector, LineartAnimeDetector, CannyDetector, ContentShuffleDetector, ZoeDetector, MediapipeFaceDetector, SamDetector
 
 # load image
 url = "https://huggingface.co/lllyasviel/sd-controlnet-openpose/resolve/main/images/pose.png"
 
 response = requests.get(url)
 img = Image.open(BytesIO(response.content)).convert("RGB").resize((512, 512))
 
@@ -55,28 +56,33 @@
 midas = MidasDetector.from_pretrained("lllyasviel/Annotators")
 mlsd = MLSDdetector.from_pretrained("lllyasviel/Annotators")
 open_pose = OpenposeDetector.from_pretrained("lllyasviel/Annotators")
 pidi = PidiNetDetector.from_pretrained("lllyasviel/Annotators")
 normal_bae = NormalBaeDetector.from_pretrained("lllyasviel/Annotators")
 lineart = LineartDetector.from_pretrained("lllyasviel/Annotators")
 lineart_anime = LineartAnimeDetector.from_pretrained("lllyasviel/Annotators")
+zoe = ZoeDetector.from_pretrained("lllyasviel/Annotators")
+sam = SamDetector("./weight_path")
 
 # instantiate
 canny = CannyDetector()
 content = ContentShuffleDetector()
+face_detector = MediapipeFaceDetector()
 
 
 # process
 processed_image_hed = hed(img)
 processed_image_midas = midas(img)
 processed_image_mlsd = mlsd(img)
 processed_image_open_pose = open_pose(img, hand_and_face=True)
 processed_image_pidi = pidi(img, safe=True)
 processed_image_normal_bae = normal_bae(img)
 processed_image_lineart = lineart(img, coarse=True)
 processed_image_lineart_anime = lineart_anime(img)
+processed_image_zoe = zoe(img)
 
 processed_image_canny = canny(img)
 processed_image_content = content(img)
+processed_image_mediapipe_face = face_detector(img)
 ```
```

