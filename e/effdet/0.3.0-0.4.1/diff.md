# Comparing `tmp/effdet-0.3.0.tar.gz` & `tmp/effdet-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "effdet-0.3.0.tar", last modified: Thu Jan  6 21:01:33 2022, max compression
+gzip compressed data, was "effdet-0.4.1.tar", last modified: Sun May 21 22:16:45 2023, max compression
```

## Comparing `effdet-0.3.0.tar` & `effdet-0.4.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2022-01-06 21:01:33.872753 effdet-0.3.0/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11343 2020-11-10 01:29:39.000000 effdet-0.3.0/LICENSE
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    32752 2022-01-06 21:01:33.872753 effdet-0.3.0/PKG-INFO
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    31665 2022-01-06 20:57:53.000000 effdet-0.3.0/README.md
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2022-01-06 21:01:33.868753 effdet-0.3.0/effdet/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      479 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17212 2022-01-06 20:22:46.000000 effdet-0.3.0/effdet/anchors.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7373 2022-01-06 20:22:46.000000 effdet-0.3.0/effdet/bench.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2022-01-06 21:01:33.868753 effdet-0.3.0/effdet/config/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      247 2022-01-06 20:22:46.000000 effdet-0.3.0/effdet/config/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      178 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/config/config_utils.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6758 2022-01-06 20:22:46.000000 effdet-0.3.0/effdet/config/fpn_config.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    26363 2022-01-06 20:47:33.000000 effdet-0.3.0/effdet/config/model_config.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      798 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/config/train_config.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2022-01-06 21:01:33.872753 effdet-0.3.0/effdet/data/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      235 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/data/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2624 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/data/dataset.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6378 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/data/dataset_config.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4170 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/data/dataset_factory.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2808 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/data/input_config.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9187 2022-01-06 20:22:46.000000 effdet-0.3.0/effdet/data/loader.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2022-01-06 21:01:33.872753 effdet-0.3.0/effdet/data/parsers/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      118 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/data/parsers/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3481 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/data/parsers/parser.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3321 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/data/parsers/parser_coco.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1182 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/data/parsers/parser_config.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      491 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/data/parsers/parser_factory.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9161 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/data/parsers/parser_open_images.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5140 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/data/parsers/parser_voc.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4422 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/data/random_erasing.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9504 2022-01-06 20:22:46.000000 effdet-0.3.0/effdet/data/transforms.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9700 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/distributed.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    26746 2022-01-06 20:22:46.000000 effdet-0.3.0/effdet/efficientdet.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2022-01-06 21:01:33.872753 effdet-0.3.0/effdet/evaluation/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)        0 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/evaluation/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    29907 2022-01-06 20:22:46.000000 effdet-0.3.0/effdet/evaluation/detection_evaluator.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4327 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/evaluation/fields.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6591 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/evaluation/metrics.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    27721 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/evaluation/np_box_list.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    19429 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/evaluation/np_mask_list.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    14552 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/evaluation/object_detection_evaluation.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    31672 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/evaluation/per_image_evaluation.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7828 2022-01-06 20:22:46.000000 effdet-0.3.0/effdet/evaluator.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2186 2022-01-06 20:22:46.000000 effdet-0.3.0/effdet/factory.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      737 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/helpers.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    10711 2022-01-06 20:22:46.000000 effdet-0.3.0/effdet/loss.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2022-01-06 21:01:33.872753 effdet-0.3.0/effdet/object_detection/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1074 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/object_detection/__init__.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8550 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/object_detection/argmax_matcher.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6391 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/object_detection/box_coder.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7034 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/object_detection/box_list.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7492 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/object_detection/matcher.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3610 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/object_detection/region_similarity_calculator.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    12981 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/object_detection/target_assigner.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6229 2020-11-10 01:29:39.000000 effdet-0.3.0/effdet/soft_nms.py
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       22 2022-01-06 20:24:25.000000 effdet-0.3.0/effdet/version.py
-drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2022-01-06 21:01:33.868753 effdet-0.3.0/effdet.egg-info/
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    32752 2022-01-06 21:01:33.000000 effdet-0.3.0/effdet.egg-info/PKG-INFO
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1558 2022-01-06 21:01:33.000000 effdet-0.3.0/effdet.egg-info/SOURCES.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)        1 2022-01-06 21:01:33.000000 effdet-0.3.0/effdet.egg-info/dependency_links.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       70 2022-01-06 21:01:33.000000 effdet-0.3.0/effdet.egg-info/requires.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)        7 2022-01-06 21:01:33.000000 effdet-0.3.0/effdet.egg-info/top_level.txt
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       38 2022-01-06 21:01:33.872753 effdet-0.3.0/setup.cfg
--rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1829 2022-01-06 20:22:46.000000 effdet-0.3.0/setup.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-21 22:16:45.988235 effdet-0.4.1/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    11343 2020-11-10 01:29:39.000000 effdet-0.4.1/LICENSE
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    33145 2023-05-21 22:16:45.988235 effdet-0.4.1/PKG-INFO
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    32094 2023-05-21 22:03:32.000000 effdet-0.4.1/README.md
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-21 22:16:45.980234 effdet-0.4.1/effdet/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      479 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/__init__.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    17224 2023-05-21 22:16:25.000000 effdet-0.4.1/effdet/anchors.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7962 2023-02-09 23:37:17.000000 effdet-0.4.1/effdet/bench.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-21 22:16:45.980234 effdet-0.4.1/effdet/config/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      247 2022-01-06 20:22:46.000000 effdet-0.4.1/effdet/config/__init__.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      178 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/config/config_utils.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6758 2022-01-06 20:22:46.000000 effdet-0.4.1/effdet/config/fpn_config.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    26363 2022-01-06 20:47:33.000000 effdet-0.4.1/effdet/config/model_config.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      798 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/config/train_config.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-21 22:16:45.984234 effdet-0.4.1/effdet/data/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      235 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/data/__init__.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2624 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/data/dataset.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6378 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/data/dataset_config.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4170 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/data/dataset_factory.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2808 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/data/input_config.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9187 2022-01-06 20:22:46.000000 effdet-0.4.1/effdet/data/loader.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-21 22:16:45.984234 effdet-0.4.1/effdet/data/parsers/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      118 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/data/parsers/__init__.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3481 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/data/parsers/parser.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3321 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/data/parsers/parser_coco.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1182 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/data/parsers/parser_config.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      491 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/data/parsers/parser_factory.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9161 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/data/parsers/parser_open_images.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     5140 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/data/parsers/parser_voc.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4422 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/data/random_erasing.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9504 2022-01-06 20:22:46.000000 effdet-0.4.1/effdet/data/transforms.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     9700 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/distributed.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    28412 2023-02-10 01:38:34.000000 effdet-0.4.1/effdet/efficientdet.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-21 22:16:45.984234 effdet-0.4.1/effdet/evaluation/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)        0 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/evaluation/__init__.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    29907 2022-01-06 20:22:46.000000 effdet-0.4.1/effdet/evaluation/detection_evaluator.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     4327 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/evaluation/fields.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6595 2023-05-21 20:42:36.000000 effdet-0.4.1/effdet/evaluation/metrics.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    27721 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/evaluation/np_box_list.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    19429 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/evaluation/np_mask_list.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    14552 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/evaluation/object_detection_evaluation.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    31672 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/evaluation/per_image_evaluation.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7828 2022-01-06 20:22:46.000000 effdet-0.4.1/effdet/evaluator.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     2186 2022-01-06 20:22:46.000000 effdet-0.4.1/effdet/factory.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)      737 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/helpers.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    10720 2023-05-21 21:45:54.000000 effdet-0.4.1/effdet/loss.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-21 22:16:45.988235 effdet-0.4.1/effdet/object_detection/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1074 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/object_detection/__init__.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     8550 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/object_detection/argmax_matcher.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6391 2023-05-21 20:42:36.000000 effdet-0.4.1/effdet/object_detection/box_coder.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7034 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/object_detection/box_list.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     7492 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/object_detection/matcher.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     3610 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/object_detection/region_similarity_calculator.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    12981 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/object_detection/target_assigner.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     6229 2020-11-10 01:29:39.000000 effdet-0.4.1/effdet/soft_nms.py
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       22 2023-05-21 22:03:32.000000 effdet-0.4.1/effdet/version.py
+drwxrwxr-x   0 wiggs     (1000) wiggs     (1000)        0 2023-05-21 22:16:45.980234 effdet-0.4.1/effdet.egg-info/
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)    33145 2023-05-21 22:16:45.000000 effdet-0.4.1/effdet.egg-info/PKG-INFO
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1558 2023-05-21 22:16:45.000000 effdet-0.4.1/effdet.egg-info/SOURCES.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)        1 2023-05-21 22:16:45.000000 effdet-0.4.1/effdet.egg-info/dependency_links.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       72 2023-05-21 22:16:45.000000 effdet-0.4.1/effdet.egg-info/requires.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)        7 2023-05-21 22:16:45.000000 effdet-0.4.1/effdet.egg-info/top_level.txt
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)       38 2023-05-21 22:16:45.988235 effdet-0.4.1/setup.cfg
+-rw-rw-r--   0 wiggs     (1000) wiggs     (1000)     1832 2023-05-21 22:01:25.000000 effdet-0.4.1/setup.py
```

### Comparing `effdet-0.3.0/LICENSE` & `effdet-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/PKG-INFO` & `effdet-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: effdet
-Version: 0.3.0
+Version: 0.4.1
 Summary: EfficientDet for PyTorch
 Home-page: https://github.com/rwightman/efficientdet-pytorch
 Author: Ross Wightman
 Author-email: hello@rwightman.com
-License: UNKNOWN
 Keywords: pytorch pretrained efficientdet efficientnet bifpn object detection
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EfficientDet (PyTorch)
 
 A PyTorch implementation of EfficientDet.
 
@@ -39,16 +37,26 @@
 * BiFPN connections and combination mode are fully configurable and not baked into the model code
 * BiFPN and head modules can be switched between depthwise separable or standard convolutions
 * Activations, batch norm layers are switchable via arguments (soon config)
 * Any backbone in my `timm` model collection that supports feature extraction (`features_only` arg) can be used as a bacbkone.
 
 ## Updates
 
+### 2023-05-21
+* Depend on `timm` 0.9
+* Minor bug fixes
+* Version 0.4.1 release
+
+### 2023-02-09
+* Testing with PyTorch 2.0 (nightlies), add --torchcompile support to train and validate scripts
+* A small code cleanup pass, support bwd/fwd compat across timm 0.8.x and previous releases
+* Use `timm` convert_sync_batchnorm function as it handles updated models w/ BatchNormAct2d layers
+
 ### 2022-01-06
-* New `efficientnetv2_ds` weights 50.1 mAP @ 1024x0124, using AGC clipping. Memory use comparable to D3, speed faster than D4. Smaller than optimal training batch size so can probably do better... 
+* New `efficientnetv2_ds` weights 50.1 mAP @ 1024x0124, using AGC clipping and `timm`'s `efficientnetv2_rw_s` backbone. Memory use comparable to D3, speed faster than D4. Smaller than optimal training batch size so can probably do better... 
 
 ### 2021-11-30
 * Update `efficientnetv2_dt` weights to a new set, 46.1 mAP @ 768x768, 47.0 mAP @ 896x896 using AGC clipping.
 * Add AGC (Adaptive Gradient Clipping support via `timm`). Idea from (`High-Performance Large-Scale Image Recognition Without Normalization` - https://arxiv.org/abs/2102.06171)
 * `timm` minimum version bumped up to 0.4.12
 
 ### 2021-11-16
@@ -514,9 +522,7 @@
 - [ ] Training (semantic segmentation) experiments
 - [ ] Integration with Detectron2 / MMDetection codebases
 - [ ] Addition and cleanup of EfficientNet based U-Net and DeepLab segmentation models that I've used in past projects
 - [x] Addition and cleanup of OpenImages dataset/training support from a past project
 - [ ] Exploration of instance segmentation possibilities...
 
 If you are an organization is interested in sponsoring and any of this work, or prioritization of the possible future directions interests you, feel free to contact me (issue, LinkedIn, Twitter, hello at rwightman dot com). I will setup a github sponser if there is any interest.
-
-
```

### Comparing `effdet-0.3.0/README.md` & `effdet-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,26 @@
 * BiFPN connections and combination mode are fully configurable and not baked into the model code
 * BiFPN and head modules can be switched between depthwise separable or standard convolutions
 * Activations, batch norm layers are switchable via arguments (soon config)
 * Any backbone in my `timm` model collection that supports feature extraction (`features_only` arg) can be used as a bacbkone.
 
 ## Updates
 
+### 2023-05-21
+* Depend on `timm` 0.9
+* Minor bug fixes
+* Version 0.4.1 release
+
+### 2023-02-09
+* Testing with PyTorch 2.0 (nightlies), add --torchcompile support to train and validate scripts
+* A small code cleanup pass, support bwd/fwd compat across timm 0.8.x and previous releases
+* Use `timm` convert_sync_batchnorm function as it handles updated models w/ BatchNormAct2d layers
+
 ### 2022-01-06
-* New `efficientnetv2_ds` weights 50.1 mAP @ 1024x0124, using AGC clipping. Memory use comparable to D3, speed faster than D4. Smaller than optimal training batch size so can probably do better... 
+* New `efficientnetv2_ds` weights 50.1 mAP @ 1024x0124, using AGC clipping and `timm`'s `efficientnetv2_rw_s` backbone. Memory use comparable to D3, speed faster than D4. Smaller than optimal training batch size so can probably do better... 
 
 ### 2021-11-30
 * Update `efficientnetv2_dt` weights to a new set, 46.1 mAP @ 768x768, 47.0 mAP @ 896x896 using AGC clipping.
 * Add AGC (Adaptive Gradient Clipping support via `timm`). Idea from (`High-Performance Large-Scale Image Recognition Without Normalization` - https://arxiv.org/abs/2102.06171)
 * `timm` minimum version bumped up to 0.4.12
 
 ### 2021-11-16
```

### Comparing `effdet-0.3.0/effdet/anchors.py` & `effdet-0.4.1/effdet/anchors.py`

 * *Files 2% similar despite different names*

```diff
@@ -349,16 +349,16 @@
 
         # Unpack labels.
         """Unpacks an array of cls/box into multiple scales."""
         count = 0
         for level in range(self.anchors.min_level, self.anchors.max_level + 1):
             feat_size = self.anchors.feat_sizes[level]
             steps = feat_size[0] * feat_size[1] * self.anchors.get_anchors_per_location()
-            cls_targets_out.append(cls_targets[count:count + steps].view([feat_size[0], feat_size[1], -1]))
-            box_targets_out.append(box_targets[count:count + steps].view([feat_size[0], feat_size[1], -1]))
+            cls_targets_out.append(cls_targets[count:count + steps].reshape([feat_size[0], feat_size[1], -1]))
+            box_targets_out.append(box_targets[count:count + steps].reshape([feat_size[0], feat_size[1], -1]))
             count += steps
 
         num_positives = (matches.match_results > -1).float().sum()
 
         return cls_targets_out, box_targets_out, num_positives
 
     def batch_label_anchors(self, gt_boxes, gt_classes, filter_valid=True):
@@ -389,17 +389,17 @@
             """Unpacks an array of cls/box into multiple scales."""
             count = 0
             for level in range(self.anchors.min_level, self.anchors.max_level + 1):
                 level_idx = level - self.anchors.min_level
                 feat_size = self.anchors.feat_sizes[level]
                 steps = feat_size[0] * feat_size[1] * self.anchors.get_anchors_per_location()
                 cls_targets_out[level_idx].append(
-                    cls_targets[count:count + steps].view([feat_size[0], feat_size[1], -1]))
+                    cls_targets[count:count + steps].reshape([feat_size[0], feat_size[1], -1]))
                 box_targets_out[level_idx].append(
-                    box_targets[count:count + steps].view([feat_size[0], feat_size[1], -1]))
+                    box_targets[count:count + steps].reshape([feat_size[0], feat_size[1], -1]))
                 count += steps
                 if last_sample:
                     cls_targets_out[level_idx] = torch.stack(cls_targets_out[level_idx])
                     box_targets_out[level_idx] = torch.stack(box_targets_out[level_idx])
 
             num_positives_out.append((matches.match_results > -1).float().sum())
             if last_sample:
```

### Comparing `effdet-0.3.0/effdet/bench.py` & `effdet-0.4.1/effdet/bench.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,16 +76,24 @@
 ):
     batch_detections = []
     # FIXME we may be able to do this as a batch with some tensor reshaping/indexing, PR welcome
     for i in range(batch_size):
         img_scale_i = None if img_scale is None else img_scale[i]
         img_size_i = None if img_size is None else img_size[i]
         detections = generate_detections(
-            class_out[i], box_out[i], anchor_boxes, indices[i], classes[i],
-            img_scale_i, img_size_i, max_det_per_image=max_det_per_image, soft_nms=soft_nms)
+            class_out[i],
+            box_out[i],
+            anchor_boxes,
+            indices[i],
+            classes[i],
+            img_scale_i,
+            img_size_i,
+            max_det_per_image=max_det_per_image,
+            soft_nms=soft_nms,
+        )
         batch_detections.append(detections)
     return torch.stack(batch_detections, dim=0)
 
 
 class DetBenchPredict(nn.Module):
     def __init__(self, model):
         super(DetBenchPredict, self).__init__()
@@ -97,23 +105,35 @@
         self.max_detection_points = model.config.max_detection_points
         self.max_det_per_image = model.config.max_det_per_image
         self.soft_nms = model.config.soft_nms
 
     def forward(self, x, img_info: Optional[Dict[str, torch.Tensor]] = None):
         class_out, box_out = self.model(x)
         class_out, box_out, indices, classes = _post_process(
-            class_out, box_out, num_levels=self.num_levels, num_classes=self.num_classes,
-            max_detection_points=self.max_detection_points)
+            class_out,
+            box_out,
+            num_levels=self.num_levels,
+            num_classes=self.num_classes,
+            max_detection_points=self.max_detection_points,
+        )
         if img_info is None:
             img_scale, img_size = None, None
         else:
             img_scale, img_size = img_info['img_scale'], img_info['img_size']
         return _batch_detection(
-            x.shape[0], class_out, box_out, self.anchors.boxes, indices, classes,
-            img_scale, img_size, max_det_per_image=self.max_det_per_image, soft_nms=self.soft_nms
+            x.shape[0],
+            class_out,
+            box_out,
+            self.anchors.boxes,
+            indices,
+            classes,
+            img_scale,
+            img_size,
+            max_det_per_image=self.max_det_per_image,
+            soft_nms=self.soft_nms,
         )
 
 
 class DetBenchTrain(nn.Module):
     def __init__(self, model, create_labeler=True):
         super(DetBenchTrain, self).__init__()
         self.model = model
@@ -122,40 +142,64 @@
         self.num_classes = model.config.num_classes
         self.anchors = Anchors.from_config(model.config)
         self.max_detection_points = model.config.max_detection_points
         self.max_det_per_image = model.config.max_det_per_image
         self.soft_nms = model.config.soft_nms
         self.anchor_labeler = None
         if create_labeler:
-            self.anchor_labeler = AnchorLabeler(self.anchors, self.num_classes, match_threshold=0.5)
+            self.anchor_labeler = AnchorLabeler(
+                self.anchors,
+                self.num_classes,
+                match_threshold=0.5,
+            )
         self.loss_fn = DetectionLoss(model.config)
 
     def forward(self, x, target: Dict[str, torch.Tensor]):
         class_out, box_out = self.model(x)
         if self.anchor_labeler is None:
             # target should contain pre-computed anchor labels if labeler not present in bench
             assert 'label_num_positives' in target
             cls_targets = [target[f'label_cls_{l}'] for l in range(self.num_levels)]
             box_targets = [target[f'label_bbox_{l}'] for l in range(self.num_levels)]
             num_positives = target['label_num_positives']
         else:
             cls_targets, box_targets, num_positives = self.anchor_labeler.batch_label_anchors(
-                target['bbox'], target['cls'])
-
-        loss, class_loss, box_loss = self.loss_fn(class_out, box_out, cls_targets, box_targets, num_positives)
+                target['bbox'],
+                target['cls'],
+            )
+
+        loss, class_loss, box_loss = self.loss_fn(
+            class_out,
+            box_out,
+            cls_targets,
+            box_targets,
+            num_positives,
+        )
         output = {'loss': loss, 'class_loss': class_loss, 'box_loss': box_loss}
         if not self.training:
             # if eval mode, output detections for evaluation
             class_out_pp, box_out_pp, indices, classes = _post_process(
-                class_out, box_out, num_levels=self.num_levels, num_classes=self.num_classes,
-                max_detection_points=self.max_detection_points)
+                class_out,
+                box_out,
+                num_levels=self.num_levels,
+                num_classes=self.num_classes,
+                max_detection_points=self.max_detection_points,
+            )
             output['detections'] = _batch_detection(
-                x.shape[0], class_out_pp, box_out_pp, self.anchors.boxes, indices, classes,
-                target['img_scale'], target['img_size'],
-                max_det_per_image=self.max_det_per_image, soft_nms=self.soft_nms)
+                x.shape[0],
+                class_out_pp,
+                box_out_pp,
+                self.anchors.boxes,
+                indices,
+                classes,
+                target['img_scale'],
+                target['img_size'],
+                max_det_per_image=self.max_det_per_image,
+                soft_nms=self.soft_nms,
+            )
         return output
 
 
 def unwrap_bench(model):
     # Unwrap a model in support bench so that various other fns can access the weights and attribs of the
     # underlying model directly
     if hasattr(model, 'module'):  # unwrap DDP or EMA
```

### Comparing `effdet-0.3.0/effdet/config/fpn_config.py` & `effdet-0.4.1/effdet/config/fpn_config.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/config/model_config.py` & `effdet-0.4.1/effdet/config/model_config.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/config/train_config.py` & `effdet-0.4.1/effdet/config/train_config.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/data/dataset.py` & `effdet-0.4.1/effdet/data/dataset.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/data/dataset_config.py` & `effdet-0.4.1/effdet/data/dataset_config.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/data/dataset_factory.py` & `effdet-0.4.1/effdet/data/dataset_factory.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/data/input_config.py` & `effdet-0.4.1/effdet/data/input_config.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/data/loader.py` & `effdet-0.4.1/effdet/data/loader.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/data/parsers/parser.py` & `effdet-0.4.1/effdet/data/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/data/parsers/parser_coco.py` & `effdet-0.4.1/effdet/data/parsers/parser_coco.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/data/parsers/parser_config.py` & `effdet-0.4.1/effdet/data/parsers/parser_config.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/data/parsers/parser_open_images.py` & `effdet-0.4.1/effdet/data/parsers/parser_open_images.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/data/parsers/parser_voc.py` & `effdet-0.4.1/effdet/data/parsers/parser_voc.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/data/random_erasing.py` & `effdet-0.4.1/effdet/data/random_erasing.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/data/transforms.py` & `effdet-0.4.1/effdet/data/transforms.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/distributed.py` & `effdet-0.4.1/effdet/distributed.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/efficientdet.py` & `effdet-0.4.1/effdet/efficientdet.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,16 +12,18 @@
 from typing import List, Callable, Optional, Union, Tuple
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from timm import create_model
-from timm.models.layers import create_conv2d, create_pool2d, get_act_layer
-
+try:
+    from timm.layers import create_conv2d, create_pool2d, get_act_layer
+except ImportError:
+    from timm.models.layers import create_conv2d, create_pool2d, get_act_layer
 from .anchors import get_feat_sizes
 from .config import get_fpn_config, set_config_writeable, set_config_readonly
 
 _DEBUG = False
 _USE_SCALE = False
 _ACT_LAYER = get_act_layer('silu')
 
@@ -34,19 +36,36 @@
     def forward(self, x: List[torch.Tensor]) -> List[torch.Tensor]:
         for module in self:
             x = module(x)
         return x
 
 
 class ConvBnAct2d(nn.Module):
-    def __init__(self, in_channels, out_channels, kernel_size, stride=1, dilation=1, padding='', bias=False,
-                 norm_layer=nn.BatchNorm2d, act_layer=_ACT_LAYER):
+    def __init__(
+            self,
+            in_channels,
+            out_channels,
+            kernel_size,
+            stride=1,
+            dilation=1,
+            padding='',
+            bias=False,
+            norm_layer=nn.BatchNorm2d,
+            act_layer=_ACT_LAYER,
+    ):
         super(ConvBnAct2d, self).__init__()
         self.conv = create_conv2d(
-            in_channels, out_channels, kernel_size, stride=stride, dilation=dilation, padding=padding, bias=bias)
+            in_channels,
+            out_channels,
+            kernel_size,
+            stride=stride,
+            dilation=dilation,
+            padding=padding,
+            bias=bias,
+        )
         self.bn = None if norm_layer is None else norm_layer(out_channels)
         self.act = None if act_layer is None else act_layer(inplace=True)
 
     def forward(self, x):
         x = self.conv(x)
         if self.bn is not None:
             x = self.bn(x)
@@ -54,24 +73,45 @@
             x = self.act(x)
         return x
 
 
 class SeparableConv2d(nn.Module):
     """ Separable Conv
     """
-    def __init__(self, in_channels, out_channels, kernel_size=3, stride=1, dilation=1, padding='', bias=False,
-                 channel_multiplier=1.0, pw_kernel_size=1, norm_layer=nn.BatchNorm2d, act_layer=_ACT_LAYER):
+    def __init__(
+            self,
+            in_channels,
+            out_channels,
+            kernel_size=3,
+            stride=1,
+            dilation=1,
+            padding='',
+            bias=False,
+            channel_multiplier=1.0,
+            pw_kernel_size=1,
+            norm_layer=nn.BatchNorm2d,
+            act_layer=_ACT_LAYER,
+    ):
         super(SeparableConv2d, self).__init__()
         self.conv_dw = create_conv2d(
-            in_channels, int(in_channels * channel_multiplier), kernel_size,
-            stride=stride, dilation=dilation, padding=padding, depthwise=True)
-
+            in_channels,
+            int(in_channels * channel_multiplier),
+            kernel_size,
+            stride=stride,
+            dilation=dilation,
+            padding=padding,
+            depthwise=True,
+        )
         self.conv_pw = create_conv2d(
-            int(in_channels * channel_multiplier), out_channels, pw_kernel_size, padding=padding, bias=bias)
-
+            int(in_channels * channel_multiplier),
+            out_channels,
+            pw_kernel_size,
+            padding=padding,
+            bias=bias,
+        )
         self.bn = None if norm_layer is None else norm_layer(out_channels)
         self.act = None if act_layer is None else act_layer(inplace=True)
 
     def forward(self, x):
         x = self.conv_dw(x)
         x = self.conv_pw(x)
         if self.bn is not None:
@@ -111,52 +151,78 @@
     __constants__ = ['size', 'scale_factor', 'mode', 'align_corners', 'name']
     name: str
     size: Optional[Union[int, Tuple[int, int]]]
     scale_factor: Optional[Union[float, Tuple[float, float]]]
     mode: str
     align_corners: Optional[bool]
 
-    def __init__(self,
-                 size: Optional[Union[int, Tuple[int, int]]] = None,
-                 scale_factor: Optional[Union[float, Tuple[float, float]]] = None,
-                 mode: str = 'nearest',
-                 align_corners: bool = False) -> None:
+    def __init__(
+            self,
+            size: Optional[Union[int, Tuple[int, int]]] = None,
+            scale_factor: Optional[Union[float, Tuple[float, float]]] = None,
+            mode: str = 'nearest',
+            align_corners: bool = False,
+    ) -> None:
         super(Interpolate2d, self).__init__()
         self.name = type(self).__name__
         self.size = size
         if isinstance(scale_factor, tuple):
             self.scale_factor = tuple(float(factor) for factor in scale_factor)
         else:
             self.scale_factor = float(scale_factor) if scale_factor else None
         self.mode = mode
         self.align_corners = None if mode == 'nearest' else align_corners
 
     def forward(self, input: torch.Tensor) -> torch.Tensor:
         return F.interpolate(
-            input, self.size, self.scale_factor, self.mode, self.align_corners, recompute_scale_factor=False)
+            input,
+            self.size,
+            self.scale_factor,
+            self.mode,
+            self.align_corners,
+            recompute_scale_factor=False,
+        )
 
 
 class ResampleFeatureMap(nn.Sequential):
 
     def __init__(
-            self, in_channels, out_channels, input_size, output_size, pad_type='',
-            downsample=None, upsample=None, norm_layer=nn.BatchNorm2d, apply_bn=False, redundant_bias=False):
+            self,
+            in_channels,
+            out_channels,
+            input_size,
+            output_size,
+            pad_type='',
+            downsample=None,
+            upsample=None,
+            norm_layer=nn.BatchNorm2d,
+            apply_bn=False,
+            redundant_bias=False,
+    ):
         super(ResampleFeatureMap, self).__init__()
         downsample = downsample or 'max'
         upsample = upsample or 'nearest'
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.input_size = input_size
         self.output_size = output_size
 
         if in_channels != out_channels:
-            self.add_module('conv', ConvBnAct2d(
-                in_channels, out_channels, kernel_size=1, padding=pad_type,
-                norm_layer=norm_layer if apply_bn else None,
-                bias=not apply_bn or redundant_bias, act_layer=None))
+            self.add_module(
+                'conv',
+                ConvBnAct2d(
+                    in_channels,
+                    out_channels,
+                    kernel_size=1,
+                    padding=pad_type,
+                    norm_layer=norm_layer if apply_bn else None,
+                    bias=not apply_bn or redundant_bias,
+                    act_layer=None,
+                )
+            )
 
         if input_size[0] > output_size[0] and input_size[1] > output_size[1]:
             if downsample in ('max', 'avg'):
                 stride_size_h = int((input_size[0] - 1) // output_size[0] + 1)
                 stride_size_w = int((input_size[1] - 1) // output_size[1] + 1)
                 if stride_size_h == stride_size_w:
                     kernel_size = stride_size_h + 1
@@ -179,28 +245,46 @@
                     scale = (output_size[0] / input_size[0], output_size[1] / input_size[1])
                     self.add_module('upsample', Interpolate2d(scale_factor=scale, mode=upsample))
                 else:
                     self.add_module('upsample', Interpolate2d(size=output_size, mode=upsample))
 
 
 class FpnCombine(nn.Module):
-    def __init__(self, feature_info, fpn_channels, inputs_offsets, output_size, pad_type='',
-                 downsample=None, upsample=None, norm_layer=nn.BatchNorm2d, apply_resample_bn=False,
-                 redundant_bias=False, weight_method='attn'):
+    def __init__(
+            self,
+            feature_info,
+            fpn_channels,
+            inputs_offsets,
+            output_size,
+            pad_type='',
+            downsample=None,
+            upsample=None,
+            norm_layer=nn.BatchNorm2d,
+            apply_resample_bn=False,
+            redundant_bias=False,
+            weight_method='attn',
+    ):
         super(FpnCombine, self).__init__()
         self.inputs_offsets = inputs_offsets
         self.weight_method = weight_method
 
         self.resample = nn.ModuleDict()
         for idx, offset in enumerate(inputs_offsets):
             self.resample[str(offset)] = ResampleFeatureMap(
-                feature_info[offset]['num_chs'], fpn_channels,
-                input_size=feature_info[offset]['size'], output_size=output_size, pad_type=pad_type,
-                downsample=downsample, upsample=upsample, norm_layer=norm_layer, apply_bn=apply_resample_bn,
-                redundant_bias=redundant_bias)
+                feature_info[offset]['num_chs'],
+                fpn_channels,
+                input_size=feature_info[offset]['size'],
+                output_size=output_size,
+                pad_type=pad_type,
+                downsample=downsample,
+                upsample=upsample,
+                norm_layer=norm_layer,
+                apply_bn=apply_resample_bn,
+                redundant_bias=redundant_bias,
+            )
 
         if weight_method == 'attn' or weight_method == 'fastattn':
             self.edge_weights = nn.Parameter(torch.ones(len(inputs_offsets)), requires_grad=True)  # WSM
         else:
             self.edge_weights = None
 
     def forward(self, x: List[torch.Tensor]):
@@ -237,36 +321,64 @@
         self.after_combine = after_combine
 
     def forward(self, x: List[torch.Tensor]) -> torch.Tensor:
         return self.after_combine(self.combine(x))
 
 
 class BiFpnLayer(nn.Module):
-    def __init__(self, feature_info, feat_sizes, fpn_config, fpn_channels, num_levels=5, pad_type='',
-                 downsample=None, upsample=None, norm_layer=nn.BatchNorm2d, act_layer=_ACT_LAYER,
-                 apply_resample_bn=False, pre_act=True, separable_conv=True, redundant_bias=False):
+    def __init__(
+            self,
+            feature_info,
+            feat_sizes,
+            fpn_config,
+            fpn_channels,
+            num_levels=5,
+            pad_type='',
+            downsample=None,
+            upsample=None,
+            norm_layer=nn.BatchNorm2d,
+            act_layer=_ACT_LAYER,
+            apply_resample_bn=False,
+            pre_act=True,
+            separable_conv=True,
+            redundant_bias=False,
+    ):
         super(BiFpnLayer, self).__init__()
         self.num_levels = num_levels
         # fill feature info for all FPN nodes (chs and feat size) before creating FPN nodes
         fpn_feature_info = feature_info + [
             dict(num_chs=fpn_channels, size=feat_sizes[fc['feat_level']]) for fc in fpn_config.nodes]
 
         self.fnode = nn.ModuleList()
         for i, fnode_cfg in enumerate(fpn_config.nodes):
             logging.debug('fnode {} : {}'.format(i, fnode_cfg))
             combine = FpnCombine(
-                fpn_feature_info, fpn_channels, tuple(fnode_cfg['inputs_offsets']),
-                output_size=feat_sizes[fnode_cfg['feat_level']], pad_type=pad_type,
-                downsample=downsample, upsample=upsample, norm_layer=norm_layer, apply_resample_bn=apply_resample_bn,
-                redundant_bias=redundant_bias, weight_method=fnode_cfg['weight_method'])
+                fpn_feature_info,
+                fpn_channels,
+                tuple(fnode_cfg['inputs_offsets']),
+                output_size=feat_sizes[fnode_cfg['feat_level']],
+                pad_type=pad_type,
+                downsample=downsample,
+                upsample=upsample,
+                norm_layer=norm_layer,
+                apply_resample_bn=apply_resample_bn,
+                redundant_bias=redundant_bias,
+                weight_method=fnode_cfg['weight_method'],
+            )
 
             after_combine = nn.Sequential()
             conv_kwargs = dict(
-                in_channels=fpn_channels, out_channels=fpn_channels, kernel_size=3, padding=pad_type,
-                bias=False, norm_layer=norm_layer, act_layer=act_layer)
+                in_channels=fpn_channels,
+                out_channels=fpn_channels,
+                kernel_size=3,
+                padding=pad_type,
+                bias=False,
+                norm_layer=norm_layer,
+                act_layer=act_layer,
+            )
             if pre_act:
                 conv_kwargs['bias'] = redundant_bias
                 conv_kwargs['act_layer'] = None
                 after_combine.add_module('act', act_layer(inplace=True))
             after_combine.add_module(
                 'conv', SeparableConv2d(**conv_kwargs) if separable_conv else ConvBnAct2d(**conv_kwargs))
 
@@ -358,16 +470,22 @@
             norm_layer = partial(norm_layer, **config.norm_kwargs)
         act_type = config.head_act_type if getattr(config, 'head_act_type', None) else config.act_type
         act_layer = get_act_layer(act_type) or _ACT_LAYER
 
         # Build convolution repeats
         conv_fn = SeparableConv2d if config.separable_conv else ConvBnAct2d
         conv_kwargs = dict(
-            in_channels=config.fpn_channels, out_channels=config.fpn_channels, kernel_size=3,
-            padding=config.pad_type, bias=config.redundant_bias, act_layer=None, norm_layer=None)
+            in_channels=config.fpn_channels,
+            out_channels=config.fpn_channels,
+            kernel_size=3,
+            padding=config.pad_type,
+            bias=config.redundant_bias,
+            act_layer=None,
+            norm_layer=None,
+        )
         self.conv_rep = nn.ModuleList([conv_fn(**conv_kwargs) for _ in range(config.box_class_repeats)])
 
         # Build batchnorm repeats. There is a unique batchnorm per feature level for each repeat.
         # This can be organized with repeats first or feature levels first in module lists, the original models
         # and weights were setup with repeats first, levels first is required for efficient torchscript usage.
         self.bn_rep = nn.ModuleList()
         if self.bn_level_first:
@@ -381,16 +499,22 @@
                     for _ in range(self.num_levels)]))
 
         self.act = act_layer(inplace=True)
 
         # Prediction (output) layer. Has bias with special init reqs, see init fn.
         num_anchors = len(config.aspect_ratios) * config.num_scales
         predict_kwargs = dict(
-            in_channels=config.fpn_channels, out_channels=num_outputs * num_anchors, kernel_size=3,
-            padding=config.pad_type, bias=True, norm_layer=None, act_layer=None)
+            in_channels=config.fpn_channels,
+            out_channels=num_outputs * num_anchors,
+            kernel_size=3,
+            padding=config.pad_type,
+            bias=True,
+            norm_layer=None,
+            act_layer=None,
+        )
         self.predict = conv_fn(**predict_kwargs)
 
     @torch.jit.ignore()
     def toggle_bn_level_first(self):
         """ Toggle the batchnorm layers between feature level first vs repeat first access pattern
         Limitations in torchscript require feature levels to be iterated over first.
 
@@ -525,32 +649,36 @@
         m.weight.data.fill_(1.0)
         m.bias.data.zero_()
 
 
 def get_feature_info(backbone):
     if isinstance(backbone.feature_info, Callable):
         # old accessor for timm versions <= 0.1.30, efficientnet and mobilenetv3 and related nets only
-        feature_info = [dict(num_chs=f['num_chs'], reduction=f['reduction'])
-                        for i, f in enumerate(backbone.feature_info())]
+        feature_info = [
+            dict(num_chs=f['num_chs'], reduction=f['reduction'])
+            for i, f in enumerate(backbone.feature_info())]
     else:
         # new feature info accessor, timm >= 0.2, all models supported
         feature_info = backbone.feature_info.get_dicts(keys=['num_chs', 'reduction'])
     return feature_info
 
 
 class EfficientDet(nn.Module):
 
     def __init__(self, config, pretrained_backbone=True, alternate_init=False):
         super(EfficientDet, self).__init__()
         self.config = config
         set_config_readonly(self.config)
         self.backbone = create_model(
-            config.backbone_name, features_only=True,
+            config.backbone_name,
+            features_only=True,
             out_indices=self.config.backbone_indices or (2, 3, 4),
-            pretrained=pretrained_backbone, **config.backbone_args)
+            pretrained=pretrained_backbone,
+            **config.backbone_args,
+        )
         feature_info = get_feature_info(self.backbone)
         self.fpn = BiFpn(self.config, feature_info)
         self.class_net = HeadNet(self.config, num_outputs=self.config.num_classes)
         self.box_net = HeadNet(self.config, num_outputs=4)
 
         for n, m in self.named_modules():
             if 'backbone' not in n:
```

### Comparing `effdet-0.3.0/effdet/evaluation/detection_evaluator.py` & `effdet-0.4.1/effdet/evaluation/detection_evaluator.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/evaluation/fields.py` & `effdet-0.4.1/effdet/evaluation/fields.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/evaluation/metrics.py` & `effdet-0.4.1/effdet/evaluation/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
             None if no ground truth labels are present.
         recall: Fraction of detected positive instance over all positive instances.
             This value is None if no ground truth labels are present.
     """
     if not isinstance(labels, np.ndarray) or len(labels.shape) != 1:
         raise ValueError("labels must be single dimension numpy array")
 
-    if labels.dtype != np.float and labels.dtype != np.bool:
+    if labels.dtype != np.float_ and labels.dtype != np.bool_:
         raise ValueError("labels type must be either bool or float")
 
     if not isinstance(scores, np.ndarray) or len(scores.shape) != 1:
         raise ValueError("scores must be single dimension numpy array")
 
     if num_gt < np.sum(labels):
         raise ValueError("Number of true positives must be smaller than num_gt.")
@@ -60,15 +60,15 @@
     if precision is None:
         if recall is not None:
             raise ValueError("If precision is None, recall must also be None")
         return np.NAN
 
     if not isinstance(precision, np.ndarray) or not isinstance(recall, np.ndarray):
         raise ValueError("precision and recall must be numpy array")
-    if precision.dtype != np.float or recall.dtype != np.float:
+    if precision.dtype != np.float_ or recall.dtype != np.float_:
         raise ValueError("input must be float numpy array.")
     if len(precision) != len(recall):
         raise ValueError("precision and recall must be of the same size.")
     if not precision.size:
         return 0.0
     if np.amin(precision) < 0 or np.amax(precision) > 1:
         raise ValueError("Precision must be in the range of [0, 1].")
```

### Comparing `effdet-0.3.0/effdet/evaluation/np_box_list.py` & `effdet-0.4.1/effdet/evaluation/np_box_list.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/evaluation/np_mask_list.py` & `effdet-0.4.1/effdet/evaluation/np_mask_list.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/evaluation/object_detection_evaluation.py` & `effdet-0.4.1/effdet/evaluation/object_detection_evaluation.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/evaluation/per_image_evaluation.py` & `effdet-0.4.1/effdet/evaluation/per_image_evaluation.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/evaluator.py` & `effdet-0.4.1/effdet/evaluator.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/factory.py` & `effdet-0.4.1/effdet/factory.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/helpers.py` & `effdet-0.4.1/effdet/helpers.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/loss.py` & `effdet-0.4.1/effdet/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     """
     err = input - target
     abs_err = err.abs()
     quadratic = torch.clamp(abs_err, max=delta)
     linear = abs_err - quadratic
     loss = 0.5 * quadratic.pow(2) + delta * linear
     if weights is not None:
-        loss *= weights
+        loss = loss.mul(weights)
     if size_average:
         return loss.mean()
     else:
         return loss.sum()
 
 
 def smooth_l1_loss(
```

### Comparing `effdet-0.3.0/effdet/object_detection/__init__.py` & `effdet-0.4.1/effdet/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/object_detection/argmax_matcher.py` & `effdet-0.4.1/effdet/object_detection/argmax_matcher.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/object_detection/box_coder.py` & `effdet-0.4.1/effdet/object_detection/box_coder.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
   coordinates, width and height. tx, ty, tw and th denote the anchor-encoded
   center, width and height respectively.
 
   See http://arxiv.org/abs/1506.01497 for details.
 """
 
 
-EPS = 1e-8
+EPS = 1e-7
 
 
 #@torch.jit.script
 class FasterRcnnBoxCoder(object):
     """Faster RCNN box coder."""
 
     def __init__(self, scale_factors: Optional[List[float]] = None, eps: float = EPS):
```

### Comparing `effdet-0.3.0/effdet/object_detection/box_list.py` & `effdet-0.4.1/effdet/object_detection/box_list.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/object_detection/matcher.py` & `effdet-0.4.1/effdet/object_detection/matcher.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/object_detection/region_similarity_calculator.py` & `effdet-0.4.1/effdet/object_detection/region_similarity_calculator.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/object_detection/target_assigner.py` & `effdet-0.4.1/effdet/object_detection/target_assigner.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet/soft_nms.py` & `effdet-0.4.1/effdet/soft_nms.py`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/effdet.egg-info/PKG-INFO` & `effdet-0.4.1/effdet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: effdet
-Version: 0.3.0
+Version: 0.4.1
 Summary: EfficientDet for PyTorch
 Home-page: https://github.com/rwightman/efficientdet-pytorch
 Author: Ross Wightman
 Author-email: hello@rwightman.com
-License: UNKNOWN
 Keywords: pytorch pretrained efficientdet efficientnet bifpn object detection
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EfficientDet (PyTorch)
 
 A PyTorch implementation of EfficientDet.
 
@@ -39,16 +37,26 @@
 * BiFPN connections and combination mode are fully configurable and not baked into the model code
 * BiFPN and head modules can be switched between depthwise separable or standard convolutions
 * Activations, batch norm layers are switchable via arguments (soon config)
 * Any backbone in my `timm` model collection that supports feature extraction (`features_only` arg) can be used as a bacbkone.
 
 ## Updates
 
+### 2023-05-21
+* Depend on `timm` 0.9
+* Minor bug fixes
+* Version 0.4.1 release
+
+### 2023-02-09
+* Testing with PyTorch 2.0 (nightlies), add --torchcompile support to train and validate scripts
+* A small code cleanup pass, support bwd/fwd compat across timm 0.8.x and previous releases
+* Use `timm` convert_sync_batchnorm function as it handles updated models w/ BatchNormAct2d layers
+
 ### 2022-01-06
-* New `efficientnetv2_ds` weights 50.1 mAP @ 1024x0124, using AGC clipping. Memory use comparable to D3, speed faster than D4. Smaller than optimal training batch size so can probably do better... 
+* New `efficientnetv2_ds` weights 50.1 mAP @ 1024x0124, using AGC clipping and `timm`'s `efficientnetv2_rw_s` backbone. Memory use comparable to D3, speed faster than D4. Smaller than optimal training batch size so can probably do better... 
 
 ### 2021-11-30
 * Update `efficientnetv2_dt` weights to a new set, 46.1 mAP @ 768x768, 47.0 mAP @ 896x896 using AGC clipping.
 * Add AGC (Adaptive Gradient Clipping support via `timm`). Idea from (`High-Performance Large-Scale Image Recognition Without Normalization` - https://arxiv.org/abs/2102.06171)
 * `timm` minimum version bumped up to 0.4.12
 
 ### 2021-11-16
@@ -514,9 +522,7 @@
 - [ ] Training (semantic segmentation) experiments
 - [ ] Integration with Detectron2 / MMDetection codebases
 - [ ] Addition and cleanup of EfficientNet based U-Net and DeepLab segmentation models that I've used in past projects
 - [x] Addition and cleanup of OpenImages dataset/training support from a past project
 - [ ] Exploration of instance segmentation possibilities...
 
 If you are an organization is interested in sponsoring and any of this work, or prioritization of the possible future directions interests you, feel free to contact me (issue, LinkedIn, Twitter, hello at rwightman dot com). I will setup a github sponser if there is any interest.
-
-
```

### Comparing `effdet-0.3.0/effdet.egg-info/SOURCES.txt` & `effdet-0.4.1/effdet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `effdet-0.3.0/setup.py` & `effdet-0.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,24 +25,24 @@
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
 
     # Note that this is a string of words separated by whitespace, not a list.
     keywords='pytorch pretrained efficientdet efficientnet bifpn object detection',
     packages=find_packages(exclude=['data']),
-    install_requires=['torch >= 1.4', 'torchvision', 'timm >= 0.4.12', 'pycocotools>=2.0.2', 'omegaconf>=2.0'],
-    python_requires='>=3.6',
+    install_requires=['torch >= 1.12.1', 'torchvision', 'timm >= 0.9.2', 'pycocotools>=2.0.2', 'omegaconf>=2.0'],
+    python_requires='>=3.7',
 )
```

