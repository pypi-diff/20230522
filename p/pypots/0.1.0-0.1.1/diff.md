# Comparing `tmp/pypots-0.1.0.tar.gz` & `tmp/pypots-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypots-0.1.0.tar", last modified: Wed May 17 02:27:02 2023, max compression
+gzip compressed data, was "pypots-0.1.1.tar", last modified: Mon May 22 10:52:53 2023, max compression
```

## Comparing `pypots-0.1.0.tar` & `pypots-0.1.1.tar`

### file list

```diff
@@ -1,102 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.626746 pypots-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-17 02:24:29.000000 pypots-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 02:24:29.000000 pypots-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19985 2023-05-17 02:27:02.626746 pypots-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-05-17 02:24:29.000000 pypots-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.610746 pypots-0.1.0/pypots/
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.610746 pypots-0.1.0/pypots/classification/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9778 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/classification/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.610746 pypots-0.1.0/pypots/classification/brits/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/classification/brits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/classification/brits/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    14883 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/classification/brits/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/classification/brits/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.614746 pypots-0.1.0/pypots/classification/grud/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/classification/grud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/classification/grud/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/classification/grud/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.614746 pypots-0.1.0/pypots/classification/raindrop/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/classification/raindrop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/classification/raindrop/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    21421 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/classification/raindrop/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/classification/raindrop/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.618746 pypots-0.1.0/pypots/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/cli/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/cli/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/cli/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/cli/pypots_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.618746 pypots-0.1.0/pypots/clustering/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/clustering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/clustering/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.618746 pypots-0.1.0/pypots/clustering/crli/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/clustering/crli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/clustering/crli/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    19565 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/clustering/crli/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/clustering/crli/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.618746 pypots-0.1.0/pypots/clustering/vader/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/clustering/vader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/clustering/vader/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    26039 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/clustering/vader/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/clustering/vader/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.618746 pypots-0.1.0/pypots/data/
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/data/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13628 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/data/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/data/load_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/data/load_specific_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.618746 pypots-0.1.0/pypots/forecasting/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/forecasting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9239 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/forecasting/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.622746 pypots-0.1.0/pypots/forecasting/bttf/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/forecasting/bttf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12613 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/forecasting/bttf/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/forecasting/bttf/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.622746 pypots-0.1.0/pypots/imputation/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/imputation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11766 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/imputation/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.622746 pypots-0.1.0/pypots/imputation/brits/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/imputation/brits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/imputation/brits/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    21684 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/imputation/brits/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/imputation/brits/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.622746 pypots-0.1.0/pypots/imputation/locf/
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/imputation/locf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/imputation/locf/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.622746 pypots-0.1.0/pypots/imputation/saits/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/imputation/saits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/imputation/saits/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    19333 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/imputation/saits/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.622746 pypots-0.1.0/pypots/imputation/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/imputation/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/imputation/transformer/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    16468 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/imputation/transformer/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/imputation/transformer/modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.626746 pypots-0.1.0/pypots/optim/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/optim/adagrad.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/optim/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/optim/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/optim/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/optim/rmsprop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/optim/sgd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.626746 pypots-0.1.0/pypots/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    19264 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-17 02:24:29.000000 pypots-0.1.0/pypots/utils/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:27:02.610746 pypots-0.1.0/pypots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19985 2023-05-17 02:27:02.000000 pypots-0.1.0/pypots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-05-17 02:27:02.000000 pypots-0.1.0/pypots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 02:27:02.000000 pypots-0.1.0/pypots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-17 02:27:02.000000 pypots-0.1.0/pypots.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-17 02:27:02.000000 pypots-0.1.0/pypots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 02:27:02.000000 pypots-0.1.0/pypots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-17 02:27:02.626746 pypots-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-17 02:24:29.000000 pypots-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.737469 pypots-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-22 10:52:08.000000 pypots-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-22 10:52:08.000000 pypots-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20988 2023-05-22 10:52:53.737469 pypots-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-05-22 10:52:08.000000 pypots-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.697469 pypots-0.1.1/pypots/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17760 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.701469 pypots-0.1.1/pypots/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16413 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/classification/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.705469 pypots-0.1.1/pypots/classification/brits/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/classification/brits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/classification/brits/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11556 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/classification/brits/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/classification/brits/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.705469 pypots-0.1.1/pypots/classification/grud/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/classification/grud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/classification/grud/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10733 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/classification/grud/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.709469 pypots-0.1.1/pypots/classification/raindrop/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/classification/raindrop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/classification/raindrop/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18621 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/classification/raindrop/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/classification/raindrop/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.709469 pypots-0.1.1/pypots/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/cli/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/cli/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/cli/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/cli/pypots_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.713469 pypots-0.1.1/pypots/clustering/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/clustering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/clustering/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.713469 pypots-0.1.1/pypots/clustering/crli/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/clustering/crli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/clustering/crli/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17111 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/clustering/crli/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9171 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/clustering/crli/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.717469 pypots-0.1.1/pypots/clustering/vader/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/clustering/vader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/clustering/vader/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23866 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/clustering/vader/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/clustering/vader/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.717469 pypots-0.1.1/pypots/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/data/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12868 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/data/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/data/load_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/data/load_specific_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.721469 pypots-0.1.1/pypots/forecasting/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/forecasting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15277 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/forecasting/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.721469 pypots-0.1.1/pypots/forecasting/bttf/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/forecasting/bttf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/forecasting/bttf/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/forecasting/bttf/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.721469 pypots-0.1.1/pypots/imputation/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16610 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.725469 pypots-0.1.1/pypots/imputation/brits/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/brits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/brits/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17855 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/brits/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/brits/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.725469 pypots-0.1.1/pypots/imputation/locf/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/locf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/locf/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.725469 pypots-0.1.1/pypots/imputation/mrnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/mrnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/mrnn/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/mrnn/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/mrnn/module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.729469 pypots-0.1.1/pypots/imputation/saits/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/saits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/saits/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16214 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/saits/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.729469 pypots-0.1.1/pypots/imputation/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/transformer/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/transformer/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/imputation/transformer/modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.733469 pypots-0.1.1/pypots/optim/
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/optim/adadelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/optim/adagrad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/optim/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/optim/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/optim/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/optim/rmsprop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/optim/sgd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.737469 pypots-0.1.1/pypots/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17891 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-22 10:52:08.000000 pypots-0.1.1/pypots/utils/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 10:52:53.701469 pypots-0.1.1/pypots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20988 2023-05-22 10:52:53.000000 pypots-0.1.1/pypots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-22 10:52:53.000000 pypots-0.1.1/pypots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 10:52:53.000000 pypots-0.1.1/pypots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 10:52:53.000000 pypots-0.1.1/pypots.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-22 10:52:53.000000 pypots-0.1.1/pypots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 10:52:53.000000 pypots-0.1.1/pypots.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-22 10:52:53.737469 pypots-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-22 10:52:08.000000 pypots-0.1.1/setup.py
```

### Comparing `pypots-0.1.0/LICENSE` & `pypots-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pypots-0.1.0/PKG-INFO` & `pypots-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: pypots
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python Toolbox for Data Mining on Partially-Observed Time Series
-Home-page: https://github.com/WenjieDu/PyPOTS
-Download-URL: https://github.com/WenjieDu/PyPOTS/archive/main.zip
+Home-page: https://pypots.com/
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: GPL-3.0
+Project-URL: Documentation, https://docs.pypots.com/
+Project-URL: Source, https://github.com/WenjieDu/PyPOTS/
+Project-URL: Tracker, https://github.com/WenjieDu/PyPOTS/issues/
+Project-URL: Download, https://github.com/WenjieDu/PyPOTS/archive/main.zip
 Keywords: data mining,neural networks,machine learning,deep learning,artificial intelligence,time-series analysis,time series,imputation,classification,clustering,forecasting,partially observed,irregular sampled,partially-observed time series,incomplete time series,missing data,missing values
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -133,16 +136,18 @@
 ## ❖ Usage
 <a href="https://github.com/WenjieDu/BrewPOTS">
     <img src="https://raw.githubusercontent.com/WenjieDu/BrewPOTS/main/figs/BrewPOTS_logo.jpg" align="left" width="160" alt="BrewPOTS logo"/>
 </a>
 
 PyPOTS tutorials have been released. Considering the future workload, I separate the tutorials into a single repo,
 and you can find them in [BrewPOTS](https://github.com/WenjieDu/BrewPOTS).
-Take a look at it now, and brew your POTS dataset into a cup of coffee! 🤓
+Take a look at it now, and learn how to brew your POTS datasets! 🤓
 
+You can also find a simple and quick-start tutorial notebook on Google Colab with
+[this link](https://colab.research.google.com/drive/1HEFjylEy05-r47jRy0H9jiS_WhD0UWmQ?usp=sharing).
 If you have further questions, please refer to PyPOTS documentation 📑[docs.pypots.com](https://docs.pypots.com).
 Besides, you can also [raise an issue](https://github.com/WenjieDu/PyPOTS/issues) or [ask in our community](#-community).
 
 We present you a usage example of imputing missing values in time series with PyPOTS below, you can click it to view.
 
 <details>
 <summary><b>Click here to see an example applying SAITS on PhysioNet2012 for imputation:</b></summary>
@@ -172,33 +177,34 @@
 ```
 </details>
 
 
 ## ❖ Available Algorithms
 PyPOTS supports imputation, classification, clustering, and forecasting tasks on multivariate time series with missing values. The currently available algorithms of four tasks are cataloged in the following table with four partitions. The paper references are all listed at the bottom of this readme file. Please refer to them if you want more details.
 
-|   ***`Imputation`***   |      🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|:----------------------:|:------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------:|
-|        **Type**        |  **Abbr.**   |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|       Neural Net       |    SAITS     |                                                               Self-Attention-based Imputation for Time Series [^1]                                                                |   2023   |
-|       Neural Net       | Transformer  | Attention is All you Need [^2];<br>Self-Attention-based Imputation for Time Series [^1];<br><sub>Note: proposed in [^2], and re-implemented as an imputation model in [^1].</sub> |   2017   |
-|       Neural Net       |    BRITS     |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
-|         Naive          |     LOCF     |                                                                         Last Observation Carried Forward                                                                          |    -     |
-| ***`Classification`*** |      🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**   |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|       Neural Net       |    BRITS     |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
-|       Neural Net       |    GRU-D     |                                                  Recurrent Neural Networks for Multivariate Time Series with Missing Values [^4]                                                  |   2018   |
-|       Neural Net       |   Raindrop   |                                                    Graph-Guided Network for Irregularly Sampled Multivariate Time Series [^5]                                                     |   2022   |
-|   ***`Clustering`***   |      🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**   |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|       Neural Net       |     CRLI     |                                                      Clustering Representation Learning on Incomplete time-series data [^6]                                                       |   2021   |
-|       Neural Net       |    VaDER     |                                                                  Variational Deep Embedding with Recurrence [^7]                                                                  |   2019   |
-|  ***`Forecasting`***   |      🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**   |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|     Probabilistic      |     BTTF     |                                                                    Bayesian Temporal Tensor Factorization [^8]                                                                    |   2021   |
+|   ***`Imputation`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
+|:----------------------:|:-----------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------:|
+|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
+|       Neural Net       |    SAITS    |                                                               Self-Attention-based Imputation for Time Series [^1]                                                                |   2023   |
+|       Neural Net       | Transformer | Attention is All you Need [^2];<br>Self-Attention-based Imputation for Time Series [^1];<br><sub>Note: proposed in [^2], and re-implemented as an imputation model in [^1].</sub> |   2017   |
+|       Neural Net       |    BRITS    |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
+|       Neural Net       |    M-RNN    |                                                                  Multi-directional Recurrent Neural Network [^9]                                                                  |   2019   |
+|         Naive          |    LOCF     |                                                                         Last Observation Carried Forward                                                                          |    -     |
+| ***`Classification`*** |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
+|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
+|       Neural Net       |    BRITS    |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
+|       Neural Net       |    GRU-D    |                                                  Recurrent Neural Networks for Multivariate Time Series with Missing Values [^4]                                                  |   2018   |
+|       Neural Net       |  Raindrop   |                                                    Graph-Guided Network for Irregularly Sampled Multivariate Time Series [^5]                                                     |   2022   |
+|   ***`Clustering`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
+|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
+|       Neural Net       |    CRLI     |                                                      Clustering Representation Learning on Incomplete time-series data [^6]                                                       |   2021   |
+|       Neural Net       |    VaDER    |                                                                  Variational Deep Embedding with Recurrence [^7]                                                                  |   2019   |
+|  ***`Forecasting`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
+|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
+|     Probabilistic      |    BTTF     |                                                                    Bayesian Temporal Tensor Factorization [^8]                                                                    |   2021   |
 
 
 ## ❖ Citing PyPOTS
 We are pursuing to publish a short paper introducing PyPOTS in prestigious academic venues, e.g. JMLR (track for
 [Machine Learning Open Source Software](https://www.jmlr.org/mloss/)). Before that, PyPOTS is using its DOI from Zenodo
 for reference. If you use PyPOTS in your research, please cite it as below and 🌟star this repository to make others
 notice this work. 🤗
@@ -224,15 +230,17 @@
 ## ❖ Contribution
 You're very welcome to contribute to this exciting project!
 
 By committing your code, you'll
 
 1. make your well-established model out-of-the-box for PyPOTS users to run,
    and help your work obtain more exposure and impact.
-   Take a look at our [inclusion criteria](https://docs.pypots.com/en/latest/faq.html#inclusion-criteria);
+   Take a look at our [inclusion criteria](https://docs.pypots.com/en/latest/faq.html#inclusion-criteria).
+   You can utilize the `template` folder in each task package (e.g.
+   [pypots/imputation/template](https://github.com/WenjieDu/PyPOTS/tree/main/pypots/imputation/template)) to quickly start;
 2. be listed as one of [PyPOTS contributors](https://github.com/WenjieDu/PyPOTS/graphs/contributors):
    <img align="center" src="https://contrib.rocks/image?repo=wenjiedu/pypots">;
 3. get mentioned in our [release notes](https://github.com/WenjieDu/PyPOTS/releases);
 
 You can also contribute to PyPOTS by simply staring🌟 this repo to help more people notice it.
 Your star is your recognition to PyPOTS, and it matters!
 
@@ -254,15 +262,15 @@
 
 
 ## ❖ Community
 We care about the feedback from our users, so we're building PyPOTS community on
 
 - [Slack](https://pypots-org.slack.com). General discussion, Q&A, and our development team are here;
 - [LinkedIn](https://www.linkedin.com/company/pypots). Official announcements and news are here;
-- [WeChat (微信公众号)](https://mp.weixin.qq.com/s/m6j83SJNgz-xySSZd-DTBw). We also run a group chat on WeChat,
+- [WeChat (微信公众号)](https://mp.weixin.qq.com/s/sNgZmgAyxDn2sZxXoWJYMA). We also run a group chat on WeChat,
   and you can get the QR code from the official account after following it;
 
 If you have any suggestions or want to contribute ideas or share time-series related papers, join us and tell.
 PyPOTS community is open, transparent, and surely friendly. Let's work together to build and improve PyPOTS 💪!
 
 
 ## ❖ Attention 👀
@@ -278,14 +286,16 @@
 [^2]: Vaswani, A., Shazeer, N.M., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A.N., Kaiser, L., & Polosukhin, I. (2017). [Attention is All you Need](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html). *NeurIPS 2017*.
 [^3]: Cao, W., Wang, D., Li, J., Zhou, H., Li, L., & Li, Y. (2018). [BRITS: Bidirectional Recurrent Imputation for Time Series](https://papers.nips.cc/paper/2018/hash/734e6bfcd358e25ac1db0a4241b95651-Abstract.html). *NeurIPS 2018*.
 [^4]: Che, Z., Purushotham, S., Cho, K., Sontag, D.A., & Liu, Y. (2018). [Recurrent Neural Networks for Multivariate Time Series with Missing Values](https://www.nature.com/articles/s41598-018-24271-9). *Scientific Reports*.
 [^5]: Zhang, X., Zeman, M., Tsiligkaridis, T., & Zitnik, M. (2022). [Graph-Guided Network for Irregularly Sampled Multivariate Time Series](https://arxiv.org/abs/2110.05357). *ICLR 2022*.
 [^6]: Ma, Q., Chen, C., Li, S., & Cottrell, G. W. (2021). [Learning Representations for Incomplete Time Series Clustering](https://ojs.aaai.org/index.php/AAAI/article/view/17070). *AAAI 2021*.
 [^7]: Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P., Ahmad, A., Vrooman, H.A., Hofmann-Apitius, M., & Fröhlich, H. (2019). [Deep learning for clustering of multivariate clinical patient trajectories with missing values](https://academic.oup.com/gigascience/article/8/11/giz134/5626377). *GigaScience*.
 [^8]: Chen, X., & Sun, L. (2021). [Bayesian Temporal Factorization for Multidimensional Time Series Prediction](https://arxiv.org/abs/1910.06366). *IEEE transactions on pattern analysis and machine intelligence*.
+[^9]: Yoon, J., Zame, W. R., & van der Schaar, M. (2019). [Estimating Missing Data in Temporal Data Streams Using Multi-Directional Recurrent Neural Networks](https://ieeexplore.ieee.org/document/8485748). *IEEE Transactions on Biomedical Engineering*.
+
 
 <details>
 <summary>🏠 Visits</summary>
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img alt="PyPOTS visits" align="left" src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Hits&edge_flat=false">
 </a>
 </details>
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 2.1 Name: pypots Version: 0.1.0 Summary: A Python Toolbox for
-Data Mining on Partially-Observed Time Series Home-page: https://github.com/
-WenjieDu/PyPOTS Download-URL: https://github.com/WenjieDu/PyPOTS/archive/
-main.zip Author: Wenjie Du Author-email: wenjay.du@gmail.com License: GPL-3.0
-Keywords: data mining,neural networks,machine learning,deep learning,artificial
-intelligence,time-series analysis,time
+Metadata-Version: 2.1 Name: pypots Version: 0.1.1 Summary: A Python Toolbox for
+Data Mining on Partially-Observed Time Series Home-page: https://pypots.com/
+Author: Wenjie Du Author-email: wenjay.du@gmail.com License: GPL-3.0 Project-
+URL: Documentation, https://docs.pypots.com/ Project-URL: Source, https://
+github.com/WenjieDu/PyPOTS/ Project-URL: Tracker, https://github.com/WenjieDu/
+PyPOTS/issues/ Project-URL: Download, https://github.com/WenjieDu/PyPOTS/
+archive/main.zip Keywords: data mining,neural networks,machine learning,deep
+learning,artificial intelligence,time-series analysis,time
 series,imputation,classification,clustering,forecasting,partially
 observed,irregular sampled,partially-observed time series,incomplete time
 series,missing data,missing values Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: Operating System :: OS Independent Classifier: Programming
@@ -59,55 +61,59 @@
 version # by conda conda install -c conda-forge pypots # the first time
 installation conda update -c conda-forge pypots # update pypots to the latest
 version ```` Alternatively, you can install from the latest source code with
 the latest features but may be not officially released yet: > pip install
 https://github.com/WenjieDu/PyPOTS/archive/main.zip ## â Usage [BrewPOTS
 logo] PyPOTS tutorials have been released. Considering the future workload, I
 separate the tutorials into a single repo, and you can find them in [BrewPOTS]
-(https://github.com/WenjieDu/BrewPOTS). Take a look at it now, and brew your
-POTS dataset into a cup of coffee! ð¤ If you have further questions, please
-refer to PyPOTS documentation ð[docs.pypots.com](https://docs.pypots.com).
-Besides, you can also [raise an issue](https://github.com/WenjieDu/PyPOTS/
-issues) or [ask in our community](#-community). We present you a usage example
-of imputing missing values in time series with PyPOTS below, you can click it
-to view.  Click here to see an example applying SAITS on PhysioNet2012 for
-imputation: ``` python import numpy as np from sklearn.preprocessing import
-StandardScaler from pypots.data import load_specific_dataset, mcar, masked_fill
-from pypots.imputation import SAITS from pypots.utils.metrics import cal_mae #
-Data preprocessing. Tedious, but PyPOTS can help. ð¤ data =
-load_specific_dataset('physionet_2012') # PyPOTS will automatically download
-and extract it. X = data['X'] num_samples = len(X['RecordID'].unique()) X =
-X.drop(['RecordID', 'Time'], axis = 1) X = StandardScaler().fit_transform
-(X.to_numpy()) X = X.reshape(num_samples, 48, -1) X_intact, X, missing_mask,
-indicating_mask = mcar(X, 0.1) # hold out 10% observed values as ground truth X
-= masked_fill(X, 1 - missing_mask, np.nan) dataset = {"X": X} print(dataset
-["X"].shape) # (11988, 48, 37), 11988 samples, 48 time steps, 37 features #
-Model training. This is PyPOTS showtime. ðª saits = SAITS(n_steps=48,
-n_features=37, n_layers=2, d_model=256, d_inner=128, n_head=4, d_k=64, d_v=64,
-dropout=0.1, epochs=10) saits.fit(dataset) # train the model. Here I use the
-whole dataset as the training set, because ground truth is not visible to the
-model. imputation = saits.impute(dataset) # impute the originally-missing
-values and artificially-missing values mae = cal_mae(imputation, X_intact,
-indicating_mask) # calculate mean absolute error on the ground truth
-(artificially-missing values) ```  ## â Available Algorithms PyPOTS supports
-imputation, classification, clustering, and forecasting tasks on multivariate
-time series with missing values. The currently available algorithms of four
-tasks are cataloged in the following table with four partitions. The paper
-references are all listed at the bottom of this readme file. Please refer to
-them if you want more details. | ***`Imputation`*** | ð¥ | ð¥ | ð¥ | |:--
---------------------:|:------------:|:-----------------------------------------
+(https://github.com/WenjieDu/BrewPOTS). Take a look at it now, and learn how to
+brew your POTS datasets! ð¤ You can also find a simple and quick-start
+tutorial notebook on Google Colab with [this link](https://
+colab.research.google.com/drive/1HEFjylEy05-r47jRy0H9jiS_WhD0UWmQ?usp=sharing).
+If you have further questions, please refer to PyPOTS documentation ð
+[docs.pypots.com](https://docs.pypots.com). Besides, you can also [raise an
+issue](https://github.com/WenjieDu/PyPOTS/issues) or [ask in our community](#-
+community). We present you a usage example of imputing missing values in time
+series with PyPOTS below, you can click it to view.  Click here to see an
+example applying SAITS on PhysioNet2012 for imputation: ``` python import numpy
+as np from sklearn.preprocessing import StandardScaler from pypots.data import
+load_specific_dataset, mcar, masked_fill from pypots.imputation import SAITS
+from pypots.utils.metrics import cal_mae # Data preprocessing. Tedious, but
+PyPOTS can help. ð¤ data = load_specific_dataset('physionet_2012') # PyPOTS
+will automatically download and extract it. X = data['X'] num_samples = len(X
+['RecordID'].unique()) X = X.drop(['RecordID', 'Time'], axis = 1) X =
+StandardScaler().fit_transform(X.to_numpy()) X = X.reshape(num_samples, 48, -1)
+X_intact, X, missing_mask, indicating_mask = mcar(X, 0.1) # hold out 10%
+observed values as ground truth X = masked_fill(X, 1 - missing_mask, np.nan)
+dataset = {"X": X} print(dataset["X"].shape) # (11988, 48, 37), 11988 samples,
+48 time steps, 37 features # Model training. This is PyPOTS showtime. ðª
+saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_inner=128,
+n_head=4, d_k=64, d_v=64, dropout=0.1, epochs=10) saits.fit(dataset) # train
+the model. Here I use the whole dataset as the training set, because ground
+truth is not visible to the model. imputation = saits.impute(dataset) # impute
+the originally-missing values and artificially-missing values mae = cal_mae
+(imputation, X_intact, indicating_mask) # calculate mean absolute error on the
+ground truth (artificially-missing values) ```  ## â Available Algorithms
+PyPOTS supports imputation, classification, clustering, and forecasting tasks
+on multivariate time series with missing values. The currently available
+algorithms of four tasks are cataloged in the following table with four
+partitions. The paper references are all listed at the bottom of this readme
+file. Please refer to them if you want more details. | ***`Imputation`*** |
+ð¥ | ð¥ | ð¥ | |:----------------------:|:-----------:|:-----------------
 -------------------------------------------------------------------------------
----------------------------------------------------------:|:--------:| |
-**Type** | **Abbr.** | **Full name of the algorithm/model/paper** | **Year** |
-| Neural Net | SAITS | Self-Attention-based Imputation for Time Series [^1] |
-2023 | | Neural Net | Transformer | Attention is All you Need [^2];
+-------------------------------------------------------------------------------
+--:|:--------:| | **Type** | **Abbr.** | **Full name of the algorithm/model/
+paper** | **Year** | | Neural Net | SAITS | Self-Attention-based Imputation for
+Time Series [^1] | 2023 | | Neural Net | Transformer | Attention is All you
+Need [^2];
 Self-Attention-based Imputation for Time Series [^1];
 Note: proposed in [^2], and re-implemented as an imputation model in [^1]. |
 2017 | | Neural Net | BRITS | Bidirectional Recurrent Imputation for Time
-Series [^3] | 2018 | | Naive | LOCF | Last Observation Carried Forward | - | |
+Series [^3] | 2018 | | Neural Net | M-RNN | Multi-directional Recurrent Neural
+Network [^9] | 2019 | | Naive | LOCF | Last Observation Carried Forward | - | |
 ***`Classification`*** | ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full
 name of the algorithm/model/paper** | **Year** | | Neural Net | BRITS |
 Bidirectional Recurrent Imputation for Time Series [^3] | 2018 | | Neural Net |
 GRU-D | Recurrent Neural Networks for Multivariate Time Series with Missing
 Values [^4] | 2018 | | Neural Net | Raindrop | Graph-Guided Network for
 Irregularly Sampled Multivariate Time Series [^5] | 2022 | | ***`Clustering`***
 | ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
@@ -127,28 +133,31 @@
 WenjieDu/PyPOTS}}, url = {\url{https://github.com/WenjieDu/PyPOTS}}, doi =
 {10.5281/zenodo.6823221}, } ``` or > Wenjie Du. (2022). > PyPOTS: A Python
 Toolbox for Data Mining on Partially-Observed Time Series. > Zenodo. https://
 doi.org/10.5281/zenodo.6823221 ## â Contribution You're very welcome to
 contribute to this exciting project! By committing your code, you'll 1. make
 your well-established model out-of-the-box for PyPOTS users to run, and help
 your work obtain more exposure and impact. Take a look at our [inclusion
-criteria](https://docs.pypots.com/en/latest/faq.html#inclusion-criteria); 2. be
-listed as one of [PyPOTS contributors](https://github.com/WenjieDu/PyPOTS/
-graphs/contributors): [https://contrib.rocks/image?repo=wenjiedu/pypots]; 3.
-get mentioned in our [release notes](https://github.com/WenjieDu/PyPOTS/
-releases); You can also contribute to PyPOTS by simply staringð this repo to
-help more people notice it. Your star is your recognition to PyPOTS, and it
-matters!   ð Click here to view PyPOTS stargazers and forkers.
+criteria](https://docs.pypots.com/en/latest/faq.html#inclusion-criteria). You
+can utilize the `template` folder in each task package (e.g. [pypots/
+imputation/template](https://github.com/WenjieDu/PyPOTS/tree/main/pypots/
+imputation/template)) to quickly start; 2. be listed as one of [PyPOTS
+contributors](https://github.com/WenjieDu/PyPOTS/graphs/contributors): [https:/
+/contrib.rocks/image?repo=wenjiedu/pypots]; 3. get mentioned in our [release
+notes](https://github.com/WenjieDu/PyPOTS/releases); You can also contribute to
+PyPOTS by simply staringð this repo to help more people notice it. Your star
+is your recognition to PyPOTS, and it matters!   ð Click here to view PyPOTS
+stargazers and forkers.
 We're so proud to have more and more awesome users, as well as more bright
 â¨stars:  [PyPOTS_stargazers]
 [PyPOTS_forkers]  ## â Community We care about the feedback from our users,
 so we're building PyPOTS community on - [Slack](https://pypots-org.slack.com).
 General discussion, Q&A, and our development team are here; - [LinkedIn](https:
 //www.linkedin.com/company/pypots). Official announcements and news are here; -
-[WeChat (å¾®ä¿¡å¬ä¼å·)](https://mp.weixin.qq.com/s/m6j83SJNgz-xySSZd-DTBw).
+[WeChat (å¾®ä¿¡å¬ä¼å·)](https://mp.weixin.qq.com/s/sNgZmgAyxDn2sZxXoWJYMA).
 We also run a group chat on WeChat, and you can get the QR code from the
 official account after following it; If you have any suggestions or want to
 contribute ideas or share time-series related papers, join us and tell. PyPOTS
 community is open, transparent, and surely friendly. Let's work together to
 build and improve PyPOTS ðª! ## â Attention ð â¼ï¸ PyPOTS is currently
 under developing. If you like it and look forward to its growth, please give
 PyPOTS a star and watch it to keep you posted on its progress and to let me
@@ -175,8 +184,11 @@
 2021*. [^7]: Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P.,
 Ahmad, A., Vrooman, H.A., Hofmann-Apitius, M., & FrÃ¶hlich, H. (2019). [Deep
 learning for clustering of multivariate clinical patient trajectories with
 missing values](https://academic.oup.com/gigascience/article/8/11/giz134/
 5626377). *GigaScience*. [^8]: Chen, X., & Sun, L. (2021). [Bayesian Temporal
 Factorization for Multidimensional Time Series Prediction](https://arxiv.org/
 abs/1910.06366). *IEEE transactions on pattern analysis and machine
-intelligence*.  ð  Visits [PyPOTS_visits]
+intelligence*. [^9]: Yoon, J., Zame, W. R., & van der Schaar, M. (2019).
+[Estimating Missing Data in Temporal Data Streams Using Multi-Directional
+Recurrent Neural Networks](https://ieeexplore.ieee.org/document/8485748). *IEEE
+Transactions on Biomedical Engineering*.  ð  Visits [PyPOTS_visits]
```

### Comparing `pypots-0.1.0/README.md` & `pypots-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -101,16 +101,18 @@
 ## ❖ Usage
 <a href="https://github.com/WenjieDu/BrewPOTS">
     <img src="https://raw.githubusercontent.com/WenjieDu/BrewPOTS/main/figs/BrewPOTS_logo.jpg" align="left" width="160" alt="BrewPOTS logo"/>
 </a>
 
 PyPOTS tutorials have been released. Considering the future workload, I separate the tutorials into a single repo,
 and you can find them in [BrewPOTS](https://github.com/WenjieDu/BrewPOTS).
-Take a look at it now, and brew your POTS dataset into a cup of coffee! 🤓
+Take a look at it now, and learn how to brew your POTS datasets! 🤓
 
+You can also find a simple and quick-start tutorial notebook on Google Colab with
+[this link](https://colab.research.google.com/drive/1HEFjylEy05-r47jRy0H9jiS_WhD0UWmQ?usp=sharing).
 If you have further questions, please refer to PyPOTS documentation 📑[docs.pypots.com](https://docs.pypots.com).
 Besides, you can also [raise an issue](https://github.com/WenjieDu/PyPOTS/issues) or [ask in our community](#-community).
 
 We present you a usage example of imputing missing values in time series with PyPOTS below, you can click it to view.
 
 <details>
 <summary><b>Click here to see an example applying SAITS on PhysioNet2012 for imputation:</b></summary>
@@ -140,33 +142,34 @@
 ```
 </details>
 
 
 ## ❖ Available Algorithms
 PyPOTS supports imputation, classification, clustering, and forecasting tasks on multivariate time series with missing values. The currently available algorithms of four tasks are cataloged in the following table with four partitions. The paper references are all listed at the bottom of this readme file. Please refer to them if you want more details.
 
-|   ***`Imputation`***   |      🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|:----------------------:|:------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------:|
-|        **Type**        |  **Abbr.**   |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|       Neural Net       |    SAITS     |                                                               Self-Attention-based Imputation for Time Series [^1]                                                                |   2023   |
-|       Neural Net       | Transformer  | Attention is All you Need [^2];<br>Self-Attention-based Imputation for Time Series [^1];<br><sub>Note: proposed in [^2], and re-implemented as an imputation model in [^1].</sub> |   2017   |
-|       Neural Net       |    BRITS     |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
-|         Naive          |     LOCF     |                                                                         Last Observation Carried Forward                                                                          |    -     |
-| ***`Classification`*** |      🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**   |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|       Neural Net       |    BRITS     |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
-|       Neural Net       |    GRU-D     |                                                  Recurrent Neural Networks for Multivariate Time Series with Missing Values [^4]                                                  |   2018   |
-|       Neural Net       |   Raindrop   |                                                    Graph-Guided Network for Irregularly Sampled Multivariate Time Series [^5]                                                     |   2022   |
-|   ***`Clustering`***   |      🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**   |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|       Neural Net       |     CRLI     |                                                      Clustering Representation Learning on Incomplete time-series data [^6]                                                       |   2021   |
-|       Neural Net       |    VaDER     |                                                                  Variational Deep Embedding with Recurrence [^7]                                                                  |   2019   |
-|  ***`Forecasting`***   |      🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**   |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|     Probabilistic      |     BTTF     |                                                                    Bayesian Temporal Tensor Factorization [^8]                                                                    |   2021   |
+|   ***`Imputation`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
+|:----------------------:|:-----------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------:|
+|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
+|       Neural Net       |    SAITS    |                                                               Self-Attention-based Imputation for Time Series [^1]                                                                |   2023   |
+|       Neural Net       | Transformer | Attention is All you Need [^2];<br>Self-Attention-based Imputation for Time Series [^1];<br><sub>Note: proposed in [^2], and re-implemented as an imputation model in [^1].</sub> |   2017   |
+|       Neural Net       |    BRITS    |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
+|       Neural Net       |    M-RNN    |                                                                  Multi-directional Recurrent Neural Network [^9]                                                                  |   2019   |
+|         Naive          |    LOCF     |                                                                         Last Observation Carried Forward                                                                          |    -     |
+| ***`Classification`*** |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
+|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
+|       Neural Net       |    BRITS    |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
+|       Neural Net       |    GRU-D    |                                                  Recurrent Neural Networks for Multivariate Time Series with Missing Values [^4]                                                  |   2018   |
+|       Neural Net       |  Raindrop   |                                                    Graph-Guided Network for Irregularly Sampled Multivariate Time Series [^5]                                                     |   2022   |
+|   ***`Clustering`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
+|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
+|       Neural Net       |    CRLI     |                                                      Clustering Representation Learning on Incomplete time-series data [^6]                                                       |   2021   |
+|       Neural Net       |    VaDER    |                                                                  Variational Deep Embedding with Recurrence [^7]                                                                  |   2019   |
+|  ***`Forecasting`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
+|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
+|     Probabilistic      |    BTTF     |                                                                    Bayesian Temporal Tensor Factorization [^8]                                                                    |   2021   |
 
 
 ## ❖ Citing PyPOTS
 We are pursuing to publish a short paper introducing PyPOTS in prestigious academic venues, e.g. JMLR (track for
 [Machine Learning Open Source Software](https://www.jmlr.org/mloss/)). Before that, PyPOTS is using its DOI from Zenodo
 for reference. If you use PyPOTS in your research, please cite it as below and 🌟star this repository to make others
 notice this work. 🤗
@@ -192,15 +195,17 @@
 ## ❖ Contribution
 You're very welcome to contribute to this exciting project!
 
 By committing your code, you'll
 
 1. make your well-established model out-of-the-box for PyPOTS users to run,
    and help your work obtain more exposure and impact.
-   Take a look at our [inclusion criteria](https://docs.pypots.com/en/latest/faq.html#inclusion-criteria);
+   Take a look at our [inclusion criteria](https://docs.pypots.com/en/latest/faq.html#inclusion-criteria).
+   You can utilize the `template` folder in each task package (e.g.
+   [pypots/imputation/template](https://github.com/WenjieDu/PyPOTS/tree/main/pypots/imputation/template)) to quickly start;
 2. be listed as one of [PyPOTS contributors](https://github.com/WenjieDu/PyPOTS/graphs/contributors):
    <img align="center" src="https://contrib.rocks/image?repo=wenjiedu/pypots">;
 3. get mentioned in our [release notes](https://github.com/WenjieDu/PyPOTS/releases);
 
 You can also contribute to PyPOTS by simply staring🌟 this repo to help more people notice it.
 Your star is your recognition to PyPOTS, and it matters!
 
@@ -222,15 +227,15 @@
 
 
 ## ❖ Community
 We care about the feedback from our users, so we're building PyPOTS community on
 
 - [Slack](https://pypots-org.slack.com). General discussion, Q&A, and our development team are here;
 - [LinkedIn](https://www.linkedin.com/company/pypots). Official announcements and news are here;
-- [WeChat (微信公众号)](https://mp.weixin.qq.com/s/m6j83SJNgz-xySSZd-DTBw). We also run a group chat on WeChat,
+- [WeChat (微信公众号)](https://mp.weixin.qq.com/s/sNgZmgAyxDn2sZxXoWJYMA). We also run a group chat on WeChat,
   and you can get the QR code from the official account after following it;
 
 If you have any suggestions or want to contribute ideas or share time-series related papers, join us and tell.
 PyPOTS community is open, transparent, and surely friendly. Let's work together to build and improve PyPOTS 💪!
 
 
 ## ❖ Attention 👀
@@ -246,14 +251,16 @@
 [^2]: Vaswani, A., Shazeer, N.M., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A.N., Kaiser, L., & Polosukhin, I. (2017). [Attention is All you Need](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html). *NeurIPS 2017*.
 [^3]: Cao, W., Wang, D., Li, J., Zhou, H., Li, L., & Li, Y. (2018). [BRITS: Bidirectional Recurrent Imputation for Time Series](https://papers.nips.cc/paper/2018/hash/734e6bfcd358e25ac1db0a4241b95651-Abstract.html). *NeurIPS 2018*.
 [^4]: Che, Z., Purushotham, S., Cho, K., Sontag, D.A., & Liu, Y. (2018). [Recurrent Neural Networks for Multivariate Time Series with Missing Values](https://www.nature.com/articles/s41598-018-24271-9). *Scientific Reports*.
 [^5]: Zhang, X., Zeman, M., Tsiligkaridis, T., & Zitnik, M. (2022). [Graph-Guided Network for Irregularly Sampled Multivariate Time Series](https://arxiv.org/abs/2110.05357). *ICLR 2022*.
 [^6]: Ma, Q., Chen, C., Li, S., & Cottrell, G. W. (2021). [Learning Representations for Incomplete Time Series Clustering](https://ojs.aaai.org/index.php/AAAI/article/view/17070). *AAAI 2021*.
 [^7]: Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P., Ahmad, A., Vrooman, H.A., Hofmann-Apitius, M., & Fröhlich, H. (2019). [Deep learning for clustering of multivariate clinical patient trajectories with missing values](https://academic.oup.com/gigascience/article/8/11/giz134/5626377). *GigaScience*.
 [^8]: Chen, X., & Sun, L. (2021). [Bayesian Temporal Factorization for Multidimensional Time Series Prediction](https://arxiv.org/abs/1910.06366). *IEEE transactions on pattern analysis and machine intelligence*.
+[^9]: Yoon, J., Zame, W. R., & van der Schaar, M. (2019). [Estimating Missing Data in Temporal Data Streams Using Multi-Directional Recurrent Neural Networks](https://ieeexplore.ieee.org/document/8485748). *IEEE Transactions on Biomedical Engineering*.
+
 
 <details>
 <summary>🏠 Visits</summary>
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img alt="PyPOTS visits" align="left" src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Hits&edge_flat=false">
 </a>
 </details>
```

#### html2text {}

```diff
@@ -39,55 +39,59 @@
 version # by conda conda install -c conda-forge pypots # the first time
 installation conda update -c conda-forge pypots # update pypots to the latest
 version ```` Alternatively, you can install from the latest source code with
 the latest features but may be not officially released yet: > pip install
 https://github.com/WenjieDu/PyPOTS/archive/main.zip ## â Usage [BrewPOTS
 logo] PyPOTS tutorials have been released. Considering the future workload, I
 separate the tutorials into a single repo, and you can find them in [BrewPOTS]
-(https://github.com/WenjieDu/BrewPOTS). Take a look at it now, and brew your
-POTS dataset into a cup of coffee! ð¤ If you have further questions, please
-refer to PyPOTS documentation ð[docs.pypots.com](https://docs.pypots.com).
-Besides, you can also [raise an issue](https://github.com/WenjieDu/PyPOTS/
-issues) or [ask in our community](#-community). We present you a usage example
-of imputing missing values in time series with PyPOTS below, you can click it
-to view.  Click here to see an example applying SAITS on PhysioNet2012 for
-imputation: ``` python import numpy as np from sklearn.preprocessing import
-StandardScaler from pypots.data import load_specific_dataset, mcar, masked_fill
-from pypots.imputation import SAITS from pypots.utils.metrics import cal_mae #
-Data preprocessing. Tedious, but PyPOTS can help. ð¤ data =
-load_specific_dataset('physionet_2012') # PyPOTS will automatically download
-and extract it. X = data['X'] num_samples = len(X['RecordID'].unique()) X =
-X.drop(['RecordID', 'Time'], axis = 1) X = StandardScaler().fit_transform
-(X.to_numpy()) X = X.reshape(num_samples, 48, -1) X_intact, X, missing_mask,
-indicating_mask = mcar(X, 0.1) # hold out 10% observed values as ground truth X
-= masked_fill(X, 1 - missing_mask, np.nan) dataset = {"X": X} print(dataset
-["X"].shape) # (11988, 48, 37), 11988 samples, 48 time steps, 37 features #
-Model training. This is PyPOTS showtime. ðª saits = SAITS(n_steps=48,
-n_features=37, n_layers=2, d_model=256, d_inner=128, n_head=4, d_k=64, d_v=64,
-dropout=0.1, epochs=10) saits.fit(dataset) # train the model. Here I use the
-whole dataset as the training set, because ground truth is not visible to the
-model. imputation = saits.impute(dataset) # impute the originally-missing
-values and artificially-missing values mae = cal_mae(imputation, X_intact,
-indicating_mask) # calculate mean absolute error on the ground truth
-(artificially-missing values) ```  ## â Available Algorithms PyPOTS supports
-imputation, classification, clustering, and forecasting tasks on multivariate
-time series with missing values. The currently available algorithms of four
-tasks are cataloged in the following table with four partitions. The paper
-references are all listed at the bottom of this readme file. Please refer to
-them if you want more details. | ***`Imputation`*** | ð¥ | ð¥ | ð¥ | |:--
---------------------:|:------------:|:-----------------------------------------
+(https://github.com/WenjieDu/BrewPOTS). Take a look at it now, and learn how to
+brew your POTS datasets! ð¤ You can also find a simple and quick-start
+tutorial notebook on Google Colab with [this link](https://
+colab.research.google.com/drive/1HEFjylEy05-r47jRy0H9jiS_WhD0UWmQ?usp=sharing).
+If you have further questions, please refer to PyPOTS documentation ð
+[docs.pypots.com](https://docs.pypots.com). Besides, you can also [raise an
+issue](https://github.com/WenjieDu/PyPOTS/issues) or [ask in our community](#-
+community). We present you a usage example of imputing missing values in time
+series with PyPOTS below, you can click it to view.  Click here to see an
+example applying SAITS on PhysioNet2012 for imputation: ``` python import numpy
+as np from sklearn.preprocessing import StandardScaler from pypots.data import
+load_specific_dataset, mcar, masked_fill from pypots.imputation import SAITS
+from pypots.utils.metrics import cal_mae # Data preprocessing. Tedious, but
+PyPOTS can help. ð¤ data = load_specific_dataset('physionet_2012') # PyPOTS
+will automatically download and extract it. X = data['X'] num_samples = len(X
+['RecordID'].unique()) X = X.drop(['RecordID', 'Time'], axis = 1) X =
+StandardScaler().fit_transform(X.to_numpy()) X = X.reshape(num_samples, 48, -1)
+X_intact, X, missing_mask, indicating_mask = mcar(X, 0.1) # hold out 10%
+observed values as ground truth X = masked_fill(X, 1 - missing_mask, np.nan)
+dataset = {"X": X} print(dataset["X"].shape) # (11988, 48, 37), 11988 samples,
+48 time steps, 37 features # Model training. This is PyPOTS showtime. ðª
+saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_inner=128,
+n_head=4, d_k=64, d_v=64, dropout=0.1, epochs=10) saits.fit(dataset) # train
+the model. Here I use the whole dataset as the training set, because ground
+truth is not visible to the model. imputation = saits.impute(dataset) # impute
+the originally-missing values and artificially-missing values mae = cal_mae
+(imputation, X_intact, indicating_mask) # calculate mean absolute error on the
+ground truth (artificially-missing values) ```  ## â Available Algorithms
+PyPOTS supports imputation, classification, clustering, and forecasting tasks
+on multivariate time series with missing values. The currently available
+algorithms of four tasks are cataloged in the following table with four
+partitions. The paper references are all listed at the bottom of this readme
+file. Please refer to them if you want more details. | ***`Imputation`*** |
+ð¥ | ð¥ | ð¥ | |:----------------------:|:-----------:|:-----------------
 -------------------------------------------------------------------------------
----------------------------------------------------------:|:--------:| |
-**Type** | **Abbr.** | **Full name of the algorithm/model/paper** | **Year** |
-| Neural Net | SAITS | Self-Attention-based Imputation for Time Series [^1] |
-2023 | | Neural Net | Transformer | Attention is All you Need [^2];
+-------------------------------------------------------------------------------
+--:|:--------:| | **Type** | **Abbr.** | **Full name of the algorithm/model/
+paper** | **Year** | | Neural Net | SAITS | Self-Attention-based Imputation for
+Time Series [^1] | 2023 | | Neural Net | Transformer | Attention is All you
+Need [^2];
 Self-Attention-based Imputation for Time Series [^1];
 Note: proposed in [^2], and re-implemented as an imputation model in [^1]. |
 2017 | | Neural Net | BRITS | Bidirectional Recurrent Imputation for Time
-Series [^3] | 2018 | | Naive | LOCF | Last Observation Carried Forward | - | |
+Series [^3] | 2018 | | Neural Net | M-RNN | Multi-directional Recurrent Neural
+Network [^9] | 2019 | | Naive | LOCF | Last Observation Carried Forward | - | |
 ***`Classification`*** | ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full
 name of the algorithm/model/paper** | **Year** | | Neural Net | BRITS |
 Bidirectional Recurrent Imputation for Time Series [^3] | 2018 | | Neural Net |
 GRU-D | Recurrent Neural Networks for Multivariate Time Series with Missing
 Values [^4] | 2018 | | Neural Net | Raindrop | Graph-Guided Network for
 Irregularly Sampled Multivariate Time Series [^5] | 2022 | | ***`Clustering`***
 | ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
@@ -107,28 +111,31 @@
 WenjieDu/PyPOTS}}, url = {\url{https://github.com/WenjieDu/PyPOTS}}, doi =
 {10.5281/zenodo.6823221}, } ``` or > Wenjie Du. (2022). > PyPOTS: A Python
 Toolbox for Data Mining on Partially-Observed Time Series. > Zenodo. https://
 doi.org/10.5281/zenodo.6823221 ## â Contribution You're very welcome to
 contribute to this exciting project! By committing your code, you'll 1. make
 your well-established model out-of-the-box for PyPOTS users to run, and help
 your work obtain more exposure and impact. Take a look at our [inclusion
-criteria](https://docs.pypots.com/en/latest/faq.html#inclusion-criteria); 2. be
-listed as one of [PyPOTS contributors](https://github.com/WenjieDu/PyPOTS/
-graphs/contributors): [https://contrib.rocks/image?repo=wenjiedu/pypots]; 3.
-get mentioned in our [release notes](https://github.com/WenjieDu/PyPOTS/
-releases); You can also contribute to PyPOTS by simply staringð this repo to
-help more people notice it. Your star is your recognition to PyPOTS, and it
-matters!   ð Click here to view PyPOTS stargazers and forkers.
+criteria](https://docs.pypots.com/en/latest/faq.html#inclusion-criteria). You
+can utilize the `template` folder in each task package (e.g. [pypots/
+imputation/template](https://github.com/WenjieDu/PyPOTS/tree/main/pypots/
+imputation/template)) to quickly start; 2. be listed as one of [PyPOTS
+contributors](https://github.com/WenjieDu/PyPOTS/graphs/contributors): [https:/
+/contrib.rocks/image?repo=wenjiedu/pypots]; 3. get mentioned in our [release
+notes](https://github.com/WenjieDu/PyPOTS/releases); You can also contribute to
+PyPOTS by simply staringð this repo to help more people notice it. Your star
+is your recognition to PyPOTS, and it matters!   ð Click here to view PyPOTS
+stargazers and forkers.
 We're so proud to have more and more awesome users, as well as more bright
 â¨stars:  [PyPOTS_stargazers]
 [PyPOTS_forkers]  ## â Community We care about the feedback from our users,
 so we're building PyPOTS community on - [Slack](https://pypots-org.slack.com).
 General discussion, Q&A, and our development team are here; - [LinkedIn](https:
 //www.linkedin.com/company/pypots). Official announcements and news are here; -
-[WeChat (å¾®ä¿¡å¬ä¼å·)](https://mp.weixin.qq.com/s/m6j83SJNgz-xySSZd-DTBw).
+[WeChat (å¾®ä¿¡å¬ä¼å·)](https://mp.weixin.qq.com/s/sNgZmgAyxDn2sZxXoWJYMA).
 We also run a group chat on WeChat, and you can get the QR code from the
 official account after following it; If you have any suggestions or want to
 contribute ideas or share time-series related papers, join us and tell. PyPOTS
 community is open, transparent, and surely friendly. Let's work together to
 build and improve PyPOTS ðª! ## â Attention ð â¼ï¸ PyPOTS is currently
 under developing. If you like it and look forward to its growth, please give
 PyPOTS a star and watch it to keep you posted on its progress and to let me
@@ -155,8 +162,11 @@
 2021*. [^7]: Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P.,
 Ahmad, A., Vrooman, H.A., Hofmann-Apitius, M., & FrÃ¶hlich, H. (2019). [Deep
 learning for clustering of multivariate clinical patient trajectories with
 missing values](https://academic.oup.com/gigascience/article/8/11/giz134/
 5626377). *GigaScience*. [^8]: Chen, X., & Sun, L. (2021). [Bayesian Temporal
 Factorization for Multidimensional Time Series Prediction](https://arxiv.org/
 abs/1910.06366). *IEEE transactions on pattern analysis and machine
-intelligence*.  ð  Visits [PyPOTS_visits]
+intelligence*. [^9]: Yoon, J., Zame, W. R., & van der Schaar, M. (2019).
+[Estimating Missing Data in Temporal Data Streams Using Multi-Directional
+Recurrent Neural Networks](https://ieeexplore.ieee.org/document/8485748). *IEEE
+Transactions on Biomedical Engineering*.  ð  Visits [PyPOTS_visits]
```

### Comparing `pypots-0.1.0/pypots/base.py` & `pypots-0.1.1/pypots/clustering/base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,323 +1,377 @@
 """
-The base (abstract) classes for models in PyPOTS.
+The base classes for PyPOTS clustering models.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
-# License: GLP-v3
+# License: GPL-v3
 
-import os
-from abc import ABC
-from typing import Optional, Union
 
+from abc import abstractmethod
+from typing import Union, Optional
+
+import numpy as np
 import torch
-from torch.utils.tensorboard import SummaryWriter
+from torch.utils.data import DataLoader
 
-from pypots.utils.files import create_dir_if_not_exist
-from pypots.utils.logging import logger
+from ..base import BaseModel, BaseNNModel
+from ..utils.logging import logger
 
 
-class BaseModel(ABC):
-    """The base model class for all model implementations.
+class BaseClusterer(BaseModel):
+    """Abstract class for all clustering models.
 
     Parameters
     ----------
-    device : str or `torch.device`, default = None,
-        The device for the model to run on.
-        If not given, will try to use CUDA devices first (will use the GPU with device number 0 only by default),
+    n_clusters :
+        The number of clusters in the clustering task.
+
+    device :
+        The device for the model to run on. It can be a string, a :class:`torch.device` object, or a list of them.
+        If not given, will try to use CUDA devices first (will use the default CUDA device if there are multiple),
         then CPUs, considering CUDA and CPU are so far the main devices for people to train ML models.
+        If given a list of devices, e.g. ['cuda:0', 'cuda:1'], or [torch.device('cuda:0'), torch.device('cuda:1')] , the
+        model will be parallely trained on the multiple devices (so far only support parallel training on CUDA devices).
         Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
 
-    saving_path : str, default = None,
+    saving_path :
         The path for automatically saving model checkpoints and tensorboard files (i.e. loss values recorded during
         training into a tensorboard file). Will not save if not given.
 
-    model_saving_strategy : str or None, None or "best" or "better" , default = "best",
+    model_saving_strategy :
         The strategy to save model checkpoints. It has to be one of [None, "best", "better"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
 
-    Attributes
-    ----------
-    model : object, default = None,
-        The underlying model or algorithm to finish the task.
-
-    summary_writer : None or torch.utils.tensorboard.SummaryWriter,  default = None,
-        The event writer to save training logs. Default as None. It only works when parameter `tb_file_saving_path` is
-        given, otherwise the training events won't be saved.
-
-        It is designed as being set up while initializing the model because it's created to
-        1). help visualize the model's training procedure (during training not after) and
-        2). assist users to tune the model's hype-parameters.
-        If only setting it up after training with a function like setter(), it cannot achieve the 1st purpose.
-
     """
 
     def __init__(
         self,
-        device: Optional[Union[str, torch.device]] = None,
+        n_clusters: int,
+        device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
         model_saving_strategy: Optional[str] = "best",
     ):
-        saving_strategies = [None, "best", "better"]
-        assert (
-            model_saving_strategy in saving_strategies
-        ), f"saving_strategy must be one of {saving_strategies}, but got f{model_saving_strategy}."
-
-        self.device = None
-        self.saving_path = saving_path
-        self.model_saving_strategy = model_saving_strategy
-
-        self.model = None
-        self.summary_writer = None
-
-        # set up the device for model running below
-        if device is None:
-            # if it is None, then
-            self.device = torch.device(
-                "cuda:0"
-                if torch.cuda.is_available() and torch.cuda.device_count() > 0
-                else "cpu"
-            )
-            logger.info(f"No given device, using default device: {self.device}")
-        else:
-            if isinstance(device, str):
-                self.device = torch.device(device)
-            elif isinstance(device, torch.device):
-                self.device = device
-            else:
-                raise TypeError(
-                    f"device should be str or torch.device, but got {type(device)}"
-                )
-
-        # set up saving_path to save the trained model and training logs
-        if isinstance(saving_path, str):
-            from datetime import datetime
-
-            # get the current time to append to saving_path,
-            # so you can use the same saving_path to run multiple times
-            # and also be aware of when they were run
-            time_now = datetime.now().__format__("%Y%m%d_T%H%M%S")
-            # the actual saving_path for saving both the best model and the tensorboard file
-            self.saving_path = os.path.join(saving_path, time_now)
-
-            # initialize self.summary_writer only if saving_path is given and not None
-            # otherwise self.summary_writer will be None and the training log won't be saved
-            tb_saving_path = os.path.join(self.saving_path, "tensorboard")
-            self.summary_writer = SummaryWriter(
-                tb_saving_path,
-                filename_suffix=".pypots",
-            )
-
-            logger.info(f"the trained model will be saved to {self.saving_path}")
-            logger.info(f"the tensorboard file will be saved to {tb_saving_path}")
-
-    def _save_log_into_tb_file(self, step: int, stage: str, loss_dict: dict) -> None:
-        """Saving training logs into the tensorboard file specified by the given path `tb_file_saving_path`.
-
-        Parameters
-        ----------
-        step : int,
-            The current training step number.
-            One step for one batch processing, so the number of steps means how many batches the model has processed.
-
-        stage : str,
-            The stage of the current operation, e.g. 'pretraining', 'training', 'validating'.
-
-        loss_dict : dict,
-            A dictionary containing items to log, should have at least one item, and only items having its name
-            including "loss" or "error" will be logged, e.g. {'imputation_loss': 0.05, "classification_error": 0.32}.
-
-        """
-        while len(loss_dict) > 0:
-            (item_name, loss) = loss_dict.popitem()
-            # save all items containing "loss" or "error" in the name
-            # WDU: may enable customization keywords in the future
-            if ("loss" in item_name) or ("error" in item_name):
-                self.summary_writer.add_scalar(f"{stage}/{item_name}", loss, step)
+        super().__init__(
+            device,
+            saving_path,
+            model_saving_strategy,
+        )
+        self.n_clusters = n_clusters
 
-    def save_model(
+    @abstractmethod
+    def fit(
         self,
-        saving_dir: str,
-        file_name: str,
-        overwrite: bool = False,
+        train_set: Union[dict, str],
+        file_type: str = "h5py",
     ) -> None:
-        """Save the model with current parameters to a disk file.
-
-        A .pypots extension will be appended to the filename if it does not already have one.
-        Please note that such an extension is not necessary, but to indicate the saved model is from PyPOTS framework
-        so people can distinguish.
+        """Train the cluster.
 
         Parameters
         ----------
-        saving_dir : str,
-            The given directory to save the model.
-
-        file_name : str,
-            The file name of the model to be saved.
-
-        overwrite : bool, default = False,
-            Whether to overwrite the model file if the path already exists.
+        train_set :
+            The dataset for model training, should be a dictionary including the key 'X',
+            or a path string locating a data file.
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            which is time-series data for training, can contain missing values.
+            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
+            key-value pairs like a dict, and it has to include the key 'X'.
 
+        file_type :
+            The type of the given file if train_set is a path string.
         """
-        file_name = (
-            file_name + ".pypots" if file_name.split(".")[-1] != "pypots" else file_name
-        )
-        saving_path = os.path.join(saving_dir, file_name)
+        raise NotImplementedError
 
-        if os.path.exists(saving_path):
-            if overwrite:
-                logger.warning(
-                    f"File {saving_path} exists. Argument `overwrite` is True. Overwriting now..."
-                )
-            else:
-                logger.error(f"File {saving_path} exists. Saving operation aborted.")
-        try:
-            create_dir_if_not_exist(saving_dir)
-            torch.save(self.model, saving_path)
-            logger.info(f"Saved the model to {saving_path}.")
-        except Exception as e:
-            raise RuntimeError(
-                f'Failed to save the model to "{saving_path}" because of the below error! \n{e}'
-            )
-
-    def _auto_save_model_if_necessary(
+    @abstractmethod
+    def cluster(
         self,
-        training_finished: bool = True,
-        saving_name: str = None,
-    ):
-        """Automatically save the current model into a file if in need.
+        X: Union[dict, str],
+        file_type="h5py",
+    ) -> np.ndarray:
+        """Cluster the input with the trained model.
 
         Parameters
         ----------
-        training_finished : bool, default = False,
-            Whether the training is already finished when invoke this function.
-            The saving_strategy "better" only works when training_finished is False.
-            The saving_strategy "best" only works when training_finished is True.
-
-        saving_name : str, default = None,
-            The file name of the saved model.
-
+        X :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+            n_features], or a path string locating a data file, e.g. h5 file.
+
+        file_type :
+            The type of the given file if X is a path string.
+
+        Returns
+        -------
+        array-like,
+            Clustering results.
         """
-        if self.saving_path is not None and self.model_saving_strategy is not None:
-            name = self.__class__.__name__ if saving_name is None else saving_name
-            if not training_finished and self.model_saving_strategy == "better":
-                self.save_model(self.saving_path, name)
-            elif training_finished and self.model_saving_strategy == "best":
-                self.save_model(self.saving_path, name)
-        else:
-            return
-
-    def load_model(self, model_path: str) -> None:
-        """Load the saved model from a disk file.
-
-        Parameters
-        ----------
-        model_path : str,
-            Local path to a disk file saving trained model.
-
-        Notes
-        -----
-        If the training environment and the deploying/test environment use the same type of device (GPU/CPU),
-        you can load the model directly with torch.load(model_path).
-
-        """
-        assert os.path.exists(model_path), f"Model file {model_path} does not exist."
-
-        try:
-            loaded_model = torch.load(model_path, map_location=self.device)
-            if isinstance(loaded_model, torch.nn.Module):
-                self.model.load_state_dict(loaded_model.state_dict())
-            else:
-                self.model = loaded_model.model
-        except Exception as e:
-            raise e
-        logger.info(f"Model loaded successfully from {model_path}.")
+        raise NotImplementedError
 
 
-class BaseNNModel(BaseModel):
-    """The abstract class for all neural-network models.
+class BaseNNClusterer(BaseNNModel):
+    """The abstract class for all neural-network clustering models in PyPOTS.
 
     Parameters
     ----------
-    batch_size : int,
+    n_clusters :
+        The number of clusters in the clustering task.
+
+    batch_size :
         Size of the batch input into the model for one step.
 
-    epochs : int,
+    epochs :
         Training epochs, i.e. the maximum rounds of the model to be trained with.
 
-    patience : int,
+    patience :
         Number of epochs the training procedure will keep if loss doesn't decrease.
         Once exceeding the number, the training will stop.
-        Must be smaller than or equal to the value of `epoches`.
+        Must be smaller than or equal to the value of ``epochs``.
 
-    num_workers : int, default = 0,
+    num_workers :
         The number of subprocesses to use for data loading.
-        `0` means data loading will be in the main process, i.e. there won't be subprocesses.
+        ``0`` means data loading will be in the main process, i.e. there won't be subprocesses.
 
-    device : str or `torch.device`, default = None,
-        The device for the model to run on.
-        If not given, will try to use CUDA devices first, then CPUs. CUDA and CPU are so far the main devices for people
-        to train ML models. Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
+    device :
+        The device for the model to run on. It can be a string, a :class:`torch.device` object, or a list of them.
+        If not given, will try to use CUDA devices first (will use the default CUDA device if there are multiple),
+        then CPUs, considering CUDA and CPU are so far the main devices for people to train ML models.
+        If given a list of devices, e.g. ['cuda:0', 'cuda:1'], or [torch.device('cuda:0'), torch.device('cuda:1')] , the
+        model will be parallely trained on the multiple devices (so far only support parallel training on CUDA devices).
+        Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
 
-    saving_path : str, default = None,
-        The path to save the tensorboard file, which contains the loss values recorded during training.
+    saving_path :
+        The path for automatically saving model checkpoints and tensorboard files (i.e. loss values recorded during
+        training into a tensorboard file). Will not save if not given.
 
-    model_saving_strategy : str or None, None or "best" or "better" , default = "best",
+    model_saving_strategy :
         The strategy to save model checkpoints. It has to be one of [None, "best", "better"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
 
 
-    Attributes
-    ---------
-    best_model_dict : dict, default = None,
-        A dictionary contains the trained model that achieves the best performance according to the loss defined,
-        i.e. the lowest loss.
-
-    best_loss : float, default = inf,
-        The criteria to judge whether the model's performance is the best so far.
-        Usually the lower, the better.
+    Notes
+    -----
+    Optimizers are necessary for training deep-learning neural networks, but we don't put a parameter ``optimizer``
+    here because some models (e.g. GANs) need more than one optimizer (e.g. one for generator, one for discriminator),
+    and ``optimizer`` is ambiguous for them. Therefore, we leave optimizers as parameters for concrete model
+    implementations, and you can pass any number of optimizers to your model when implementing it,
+    :class:`pypots.clustering.crli.CRLI` for example.
+
     """
 
     def __init__(
         self,
+        n_clusters: int,
         batch_size: int,
         epochs: int,
         patience: int,
         num_workers: int = 0,
-        device: Optional[Union[str, torch.device]] = None,
+        device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
         model_saving_strategy: Optional[str] = "best",
     ):
-        super().__init__(device, saving_path, model_saving_strategy)
+        super().__init__(
+            batch_size,
+            epochs,
+            patience,
+            num_workers,
+            device,
+            saving_path,
+            model_saving_strategy,
+        )
+        self.n_clusters = n_clusters
 
-        if patience is None:
-            patience = -1  # early stopping on patience won't work if it is set as < 0
-        else:
-            assert (
-                patience <= epochs
-            ), f"patience must be smaller than epoches which is {epochs}, but got patience={patience}"
-
-        # training hype-parameters
-        self.batch_size = batch_size
-        self.epochs = epochs
-        self.patience = patience
-        self.original_patience = patience
-        self.num_workers = num_workers
+    @abstractmethod
+    def _assemble_input_for_training(self, data: list) -> dict:
+        """Assemble the given data into a dictionary for training input.
 
-        self.model = None
-        self.optimizer = None
-        self.best_model_dict = None
-        # WDU: may enable users to customize the criteria in the future
+        Parameters
+        ----------
+        data :
+            Input data from dataloader, should be list.
+
+        Returns
+        -------
+        dict,
+            A python dictionary contains the input data for model training.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def _assemble_input_for_validating(self, data: list) -> dict:
+        """Assemble the given data into a dictionary for validating input.
+
+        Parameters
+        ----------
+        data :
+            Data output from dataloader, should be list.
+
+        Returns
+        -------
+        dict,
+            A python dictionary contains the input data for model validating.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def _assemble_input_for_testing(self, data: list) -> dict:
+        """Assemble the given data into a dictionary for testing input.
+
+        Notes
+        -----
+        The processing functions of train/val/test stages are separated for the situation that the input of
+        the three stages are different, and this situation usually happens when the Dataset/Dataloader classes
+        used in the train/val/test stages are not the same, e.g. the training data and validating data in a
+        classification task contains labels, but the testing data (from the production environment) generally
+        doesn't have labels.
+
+        Parameters
+        ----------
+        data :
+            Data output from dataloader, should be list.
+
+        Returns
+        -------
+        dict,
+            A python dictionary contains the input data for model testing.
+        """
+        raise NotImplementedError
+
+    def _train_model(
+        self,
+        training_loader: DataLoader,
+        val_loader: DataLoader = None,
+    ) -> None:
+
+        """
+
+        Parameters
+        ----------
+        training_loader
+        val_loader
+
+        Notes
+        -----
+        The training procedures of NN clustering models are very different from each other. For example, VaDER needs
+        pretraining while CRLI doesn't, VaDER only needs one optimizer while CRLI needs two for its generator and
+        discriminator separately. So far, I'd suggest to implement function _train_model() for each model individually.
+
+        """
+        # each training starts from the very beginning, so reset the loss and model dict here
         self.best_loss = float("inf")
+        self.best_model_dict = None
 
-    def _print_model_size(self) -> None:
-        """Print the number of trainable parameters in the initialized NN model."""
-        num_params = sum(p.numel() for p in self.model.parameters() if p.requires_grad)
-        logger.info(
-            f"Model initialized successfully with the number of trainable parameters: {num_params:,}"
-        )
+        try:
+            for epoch in range(self.epochs):
+                self.model.train()
+                epoch_train_loss_collector = []
+                for idx, data in enumerate(training_loader):
+                    inputs = self._assemble_input_for_training(data)
+                    self.optimizer.zero_grad()
+                    results = self.model.forward(inputs)
+                    results["loss"].sum().backward()
+                    self.optimizer.step()
+                    epoch_train_loss_collector.append(results["loss"].sum().item())
+
+                # mean training loss of the current epoch
+                mean_train_loss = np.mean(epoch_train_loss_collector)
+
+                if val_loader is not None:
+                    self.model.eval()
+                    epoch_val_loss_collector = []
+                    with torch.no_grad():
+                        for idx, data in enumerate(val_loader):
+                            inputs = self._assemble_input_for_validating(data)
+                            results = self.model.forward(inputs)
+                            epoch_val_loss_collector.append(
+                                results["loss"].sum().item()
+                            )
+
+                    mean_val_loss = np.mean(epoch_val_loss_collector)
+                    logger.info(
+                        f"epoch {epoch}: "
+                        f"training loss {mean_train_loss:.4f}, "
+                        f"validating loss {mean_val_loss:.4f}"
+                    )
+                    mean_loss = mean_val_loss
+                else:
+                    logger.info(f"epoch {epoch}: training loss {mean_train_loss:.4f}")
+                    mean_loss = mean_train_loss
+
+                if mean_loss < self.best_loss:
+                    self.best_loss = mean_loss
+                    self.best_model_dict = self.model.state_dict()
+                    self.patience = self.original_patience
+                else:
+                    self.patience -= 1
+                    if self.patience == 0:
+                        logger.info(
+                            "Exceeded the training patience. Terminating the training procedure..."
+                        )
+                        break
+        except Exception as e:
+            logger.error(f"Exception: {e}")
+            if self.best_model_dict is None:
+                raise RuntimeError(
+                    "Training got interrupted. Model was not trained. Please investigate the error printed above."
+                )
+            else:
+                RuntimeWarning(
+                    "Training got interrupted. Please investigate the error printed above.\n"
+                    "Model got trained and will load the best checkpoint so far for testing.\n"
+                    "If you don't want it, please try fit() again."
+                )
+
+        if np.equal(self.best_loss, float("inf")):
+            raise ValueError("Something is wrong. best_loss is Nan after training.")
+
+        logger.info("Finished training.")
+
+    @abstractmethod
+    def fit(
+        self,
+        train_set: Union[dict, str],
+        file_type: str = "h5py",
+    ) -> None:
+        """Train the cluster.
+
+        Parameters
+        ----------
+        train_set :
+            The dataset for model training, should be a dictionary including the key 'X',
+            or a path string locating a data file.
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            which is time-series data for training, can contain missing values.
+            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
+            key-value pairs like a dict, and it has to include the key 'X'.
+
+        file_type :
+            The type of the given file if train_set is a path string.
+        """
+        raise NotImplementedError
+
+    @abstractmethod
+    def cluster(
+        self,
+        X: Union[dict, str],
+        file_type="h5py",
+    ) -> np.ndarray:
+        """Cluster the input with the trained model.
+
+        Parameters
+        ----------
+        X :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+            n_features], or a path string locating a data file, e.g. h5 file.
+
+        file_type :
+            The type of the given file if X is a path string.
+
+        Returns
+        -------
+        array-like,
+            Clustering results.
+        """
+        raise NotImplementedError
```

### Comparing `pypots-0.1.0/pypots/classification/base.py` & `pypots-0.1.1/pypots/data/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,271 +1,312 @@
 """
-The base classes for PyPOTS classification models.
+The base class for PyPOTS datasets.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GPL-v3
 
-
 from abc import abstractmethod
-from typing import Optional, Union
+from typing import Union, Optional, Tuple, Iterable
 
+import h5py
 import numpy as np
 import torch
-from torch.utils.data import DataLoader
+from torch.utils.data import Dataset
+
+# Currently we only support h5 files
+SUPPORTED_DATASET_FILE_TYPE = ["h5py"]
 
-from pypots.base import BaseModel, BaseNNModel
-from pypots.utils.logging import logger
 
+class BaseDataset(Dataset):
+    """Base dataset class in PyPOTS.
 
-class BaseClassifier(BaseModel):
-    """The abstract class for all PyPOTS classification models.
     Parameters
-    ---
-    device
-    saving_path
+    ----------
+    data :
+        The dataset for model input, should be a dictionary including keys as 'X' and 'y',
+        or a path string locating a data file.
+        If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+        which is time-series data for input, can contain missing values, and y should be array-like of shape
+        [n_samples], which is classification labels of X.
+        If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
+        key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
+
+    return_labels :
+        Whether to return labels in function __getitem__() if they exist in the given data. If `True`, for example,
+        during training of classification models, the Dataset class will return labels in __getitem__() for model input.
+        Otherwise, labels won't be included in the data returned by __getitem__(). This parameter exists because we
+        need the defined Dataset class for all training/validating/testing stages. For those big datasets stored in h5
+        files, they already have both X and y saved. But we don't read labels from the file for validating and testing
+        with function _fetch_data_from_file(), which works for all three stages. Therefore, we need this parameter for
+        distinction.
+
+    file_type :
+        The type of the given file if train_set and val_set are path strings.
 
     """
 
     def __init__(
         self,
-        device: Optional[Union[str, torch.device]] = None,
-        saving_path: str = None,
-        model_saving_strategy: Optional[str] = "best",
-    ):
-        super().__init__(
-            device,
-            saving_path,
-            model_saving_strategy,
-        )
-
-    @abstractmethod
-    def fit(
-        self,
-        train_set: Union[dict, str],
-        val_set: Optional[Union[dict, str]] = None,
+        data: Union[dict, str],
+        return_labels: bool = True,
         file_type: str = "h5py",
-    ) -> None:
-        """Train the classifier on the given data.
-
-        Parameters
-        ----------
-        train_set : dict or str,
-            The dataset for model training, should be a dictionary including keys as 'X' and 'y',
-            or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-            which is time-series data for training, can contain missing values, and y should be array-like of shape
-            [n_samples], which is classification labels of X.
-            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-            key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
-
-        val_set : dict or str,
-            The dataset for model validating, should be a dictionary including keys as 'X' and 'y',
-            or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-            which is time-series data for validating, can contain missing values, and y should be array-like of shape
-            [n_samples], which is classification labels of X.
-            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-            key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
+    ):
+        super().__init__()
+        # types and shapes had been checked after X and y input into the model
+        # So they are safe to use here. No need to check again.
+
+        self.data = data
+        self.return_labels = return_labels
+        if isinstance(self.data, str):  # data from file
+            # check if the given file type is supported
+            assert (
+                file_type in SUPPORTED_DATASET_FILE_TYPE
+            ), f"file_type should be one of {SUPPORTED_DATASET_FILE_TYPE}, but got {file_type}"
+
+            self.file_type = file_type
+
+            # open the file handle
+            self.file_handle = self._open_file_handle()
+            # check if X exists in the file
+            assert (
+                "X" in self.file_handle.keys()
+            ), "The given dataset file doesn't contains X. Please double check."
+
+        else:  # data from array
+            X = data["X"]
+            y = None if "y" not in data.keys() else data["y"]
+            self.X, self.y = self._check_input(X, y)
+
+        self.sample_num = self._get_sample_num()
+
+        # set up function fetch_data()
+        if isinstance(self.data, str):
+            self.fetch_data = self._fetch_data_from_file
+        else:
+            self.fetch_data = self._fetch_data_from_array
 
-        file_type : str, default = "h5py",
-            The type of the given file if train_set and val_set are path strings.
+    def _get_sample_num(self) -> int:
+        """Determine the number of samples in the dataset and return the number.
 
+        Returns
+        -------
+        sample_num :
+            The number of the samples in the given dataset.
         """
-        pass
-
-    @abstractmethod
-    def classify(
-        self,
-        X: Union[dict, str],
-        file_type: str = "h5py",
-    ) -> np.ndarray:
-        """Classify the input data with the trained model.
+        if isinstance(self.data, str):
+            if self.file_handle is None:
+                self.file_handle = self._open_file_handle()
+            sample_num = len(self.file_handle["X"])
+        else:
+            sample_num = len(self.X)
+
+        return sample_num
+
+    def __len__(self) -> int:
+        return self.sample_num
+
+    @staticmethod
+    def _check_input(
+        X: Union[np.ndarray, torch.Tensor, list],
+        y: Optional[Union[np.ndarray, torch.Tensor, list]] = None,
+        out_dtype: str = "tensor",
+    ) -> Tuple[
+        Union[np.ndarray, torch.Tensor, list],
+        Optional[Union[np.ndarray, torch.Tensor, list]],
+    ]:
+        """Check value type and shape of input X and y
 
         Parameters
         ----------
-        X : array-like or str,
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
-            n_features], or a path string locating a data file, e.g. h5 file.
+        X :
+            Time-series data that must have a shape like [n_samples, expected_n_steps, expected_n_features].
 
-        file_type : str, default = "h5py",
-            The type of the given file if X is a path string.
+        y :
+            Labels of time-series samples (X) that must have a shape like [n_samples] or [n_samples, n_classes].
+
+        out_dtype :
+            Data type of the output, should be np.ndarray or torch.Tensor
 
         Returns
         -------
-        array-like, shape [n_samples],
-            Classification results of the given samples.
-        """
-        pass
+        X :
 
+        y :
 
-class BaseNNClassifier(BaseNNModel, BaseClassifier):
-    def __init__(
-        self,
-        n_classes: int,
-        batch_size: int,
-        epochs: int,
-        patience: int,
-        num_workers: int = 0,
-        device: Optional[Union[str, torch.device]] = None,
-        saving_path: str = None,
-        model_saving_strategy: Optional[str] = "best",
-    ):
-        super().__init__(
-            batch_size,
-            epochs,
-            patience,
-            num_workers,
-            device,
-            saving_path,
-            model_saving_strategy,
+        """
+        assert out_dtype in [
+            "tensor",
+            "ndarray",
+        ], f'out_dtype should be "tensor" or "ndarray", but got {out_dtype}'
+
+        is_list = isinstance(X, list)
+        is_array = isinstance(X, np.ndarray)
+        is_tensor = isinstance(X, torch.Tensor)
+        assert is_tensor or is_array or is_list, TypeError(
+            "X should be an instance of list/np.ndarray/torch.Tensor, "
+            f"but got {type(X)}"
         )
-        self.n_classes = n_classes
+
+        # convert the data type if in need
+        if out_dtype == "tensor":
+            if is_list:
+                X = torch.tensor(X)
+            elif is_array:
+                X = torch.from_numpy(X)
+            else:  # is tensor
+                pass
+        else:  # out_dtype is ndarray
+            # convert to np.ndarray first for shape check
+            if is_list:
+                X = np.asarray(X)
+            elif is_tensor:
+                X = X.numpy()
+            else:  # is ndarray
+                pass
+
+        # check the shape of X here
+        X_shape = X.shape
+        assert len(X_shape) == 3, (
+            f"input should have 3 dimensions [n_samples, seq_len, n_features],"
+            f"but got shape={X_shape}"
+        )
+
+        if y is not None:
+            assert len(X) == len(y), (
+                f"lengths of X and y must match, " f"but got f{len(X)} and {len(y)}"
+            )
+            if isinstance(y, torch.Tensor):
+                y = y if out_dtype == "tensor" else y.numpy()
+            elif isinstance(y, list):
+                y = torch.tensor(y) if out_dtype == "tensor" else np.asarray(y)
+            elif isinstance(y, np.ndarray):
+                y = torch.from_numpy(y) if out_dtype == "tensor" else y
+            else:
+                raise TypeError(
+                    "y should be an instance of list/np.ndarray/torch.Tensor, "
+                    f"but got {type(y)}"
+                )
+
+        return X, y
 
     @abstractmethod
-    def _assemble_input_for_training(self, data) -> dict:
-        """Assemble the given data into a dictionary for training input.
+    def _fetch_data_from_array(self, idx: int) -> Iterable:
+        """Fetch data from self.X if it is given.
 
         Parameters
         ----------
-        data : list,
-            Input data from dataloader, should be list.
+        idx :
+            The index of the sample to be return.
 
         Returns
         -------
-        dict,
-            A python dictionary contains the input data for model training.
+        sample :
+            The collated data sample, a list including all necessary sample info.
         """
-        pass
 
-    @abstractmethod
-    def _assemble_input_for_validating(self, data) -> dict:
-        """Assemble the given data into a dictionary for validating input.
+        X = self.X[idx]
+        missing_mask = ~torch.isnan(X)
+        X = torch.nan_to_num(X)
+        sample = [
+            torch.tensor(idx),
+            X.to(torch.float32),
+            missing_mask.to(torch.float32),
+        ]
 
-        Parameters
-        ----------
-        data : list,
-            Data output from dataloader, should be list.
+        if self.y is not None and self.return_labels:
+            sample.append(self.y[idx].to(torch.long))
+
+        return sample
+
+    def _open_file_handle(self) -> h5py.File:
+        """Open the file handle for reading data from the file.
+
+        Notes
+        -----
+        This function can also help confirm if the given file and file type match.
 
         Returns
         -------
-        dict,
-            A python dictionary contains the input data for model validating.
+        file_handle :
+
         """
-        pass
+        data_file_path = self.data
+        try:
+            file_handler = h5py.File(
+                data_file_path,
+                "r",
+            )  # set swmr=True if the h5 file need to be written into new content during reading
+        except ImportError:
+            raise ImportError(
+                "h5py is missing and cannot be imported. Please install it first."
+            )
+        except OSError as e:
+            raise TypeError(
+                f"{e} This probably is caused by file type error. "
+                f"Please confirm that the given file {data_file_path} is an h5 file."
+            )
+        except Exception as e:
+            raise RuntimeError(e)
+        return file_handler
 
     @abstractmethod
-    def _assemble_input_for_testing(self, data) -> dict:
-        """Assemble the given data into a dictionary for testing input.
+    def _fetch_data_from_file(self, idx: int) -> Iterable:
+        """Fetch data with the lazy-loading strategy, i.e. only loading data from the file while requesting for samples.
+        Here the opened file handle doesn't load the entire dataset into RAM but only load the currently accessed slice.
 
         Notes
         -----
-        The processing functions of train/val/test stages are separated for the situation that the input of
-        the three stages are different, and this situation usually happens when the Dataset/Dataloader classes
-        used in the train/val/test stages are not the same, e.g. the training data and validating data in a
-        classification task contains labels, but the testing data (from the production environment) generally
-        doesn't have labels.
+        Multi workers reading from h5 file is tricky, and I was confronted with a problem similar to
+        https://discuss.pytorch.org/t/dataloader-when-num-worker-0-there-is-bug/25643/7 in 2020, please
+        refer to it for more details about the problem.
+        The implementation here is referred to
+        https://discuss.pytorch.org/t/dataloader-when-num-worker-0-there-is-bug/25643/10
+        And according to https://discuss.pytorch.org/t/dataloader-when-num-worker-0-there-is-bug/25643/37,
+        pytorch v1.7.1 and h5py v3.2.0 work well, so probably updating to the latest version can avoid the
+        issue I met. After all, this implementation may need to be updated in the near future.
 
         Parameters
         ----------
-        data : list,
-            Data output from dataloader, should be list.
+        idx :
+            The index of the sample to be return.
 
         Returns
         -------
-        dict,
-            A python dictionary contains the input data for model testing.
+        sample :
+            The collated data sample, a list including all necessary sample info.
         """
-        pass
 
-    def _train_model(
-        self,
-        training_loader: DataLoader,
-        val_loader: DataLoader = None,
-    ) -> None:
-
-        # each training starts from the very beginning, so reset the loss and model dict here
-        self.best_loss = float("inf")
-        self.best_model_dict = None
+        if self.file_handle is None:
+            self.file_handle = self._open_file_handle()
 
-        try:
-            training_step = 0
-            for epoch in range(self.epochs):
-                self.model.train()
-                epoch_train_loss_collector = []
-                for idx, data in enumerate(training_loader):
-                    training_step += 1
-                    inputs = self._assemble_input_for_training(data)
-                    self.optimizer.zero_grad()
-                    results = self.model.forward(inputs)
-                    results["loss"].backward()
-                    self.optimizer.step()
-                    epoch_train_loss_collector.append(results["loss"].item())
-
-                    # save training loss logs into the tensorboard file for every step if in need
-                    if self.summary_writer is not None:
-                        self._save_log_into_tb_file(training_step, "training", results)
-
-                # mean training loss of the current epoch
-                mean_train_loss = np.mean(epoch_train_loss_collector)
-
-                if val_loader is not None:
-                    self.model.eval()
-                    epoch_val_loss_collector = []
-                    with torch.no_grad():
-                        for idx, data in enumerate(val_loader):
-                            inputs = self._assemble_input_for_validating(data)
-                            results = self.model.forward(inputs)
-                            epoch_val_loss_collector.append(results["loss"].item())
-
-                    mean_val_loss = np.mean(epoch_val_loss_collector)
-
-                    # save validating loss logs into the tensorboard file for every epoch if in need
-                    if self.summary_writer is not None:
-                        val_loss_dict = {
-                            "classification_loss": mean_val_loss,
-                        }
-                        self._save_log_into_tb_file(epoch, "validating", val_loss_dict)
-
-                    logger.info(
-                        f"epoch {epoch}: "
-                        f"training loss {mean_train_loss:.4f}, "
-                        f"validating loss {mean_val_loss:.4f}"
-                    )
-                    mean_loss = mean_val_loss
-                else:
-                    logger.info(f"epoch {epoch}: training loss {mean_train_loss:.4f}")
-                    mean_loss = mean_train_loss
-
-                if mean_loss < self.best_loss:
-                    self.best_loss = mean_loss
-                    self.best_model_dict = self.model.state_dict()
-                    self.patience = self.original_patience
-                    # save the model if necessary
-                    self._auto_save_model_if_necessary(
-                        training_finished=False,
-                        saving_name=f"{self.__class__.__name__}_epoch{epoch}_loss{mean_loss}",
-                    )
-                else:
-                    self.patience -= 1
-                    if self.patience == 0:
-                        logger.info(
-                            "Exceeded the training patience. Terminating the training procedure..."
-                        )
-                        break
-        except Exception as e:
-            logger.info(f"Exception: {e}")
-            if self.best_model_dict is None:
-                raise RuntimeError(
-                    "Training got interrupted. Model was not get trained. Please try fit() again."
-                )
-            else:
-                RuntimeWarning(
-                    "Training got interrupted. "
-                    "Model will load the best parameters so far for testing. "
-                    "If you don't want it, please try fit() again."
-                )
+        X = torch.from_numpy(self.file_handle["X"][idx])
+        missing_mask = ~torch.isnan(X)
+        X = torch.nan_to_num(X)
+        sample = [
+            torch.tensor(idx),
+            X.to(torch.float32),
+            missing_mask.to(torch.float32),
+        ]
+
+        # if the dataset has labels and is for training, then fetch it from the file
+        if "y" in self.file_handle.keys() and self.return_labels:
+            sample.append(self.file_handle["y"][idx].to(torch.long))
+
+        return sample
+
+    def __getitem__(self, idx: int) -> Iterable:
+        """Fetch data according to index.
 
-        if np.equal(self.best_loss, float("inf")):
-            raise ValueError("Something is wrong. best_loss is Nan after training.")
+        Parameters
+        ----------
+        idx :
+            The index to fetch the specified sample.
+
+        Returns
+        -------
+        sample :
+            The collated data sample, a list including all necessary sample info.
+        """
 
-        logger.info("Finished training.")
+        sample = self.fetch_data(idx)
+        return sample
```

### Comparing `pypots-0.1.0/pypots/classification/brits/data.py` & `pypots-0.1.1/pypots/classification/brits/data.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 from typing import Union
 
-from pypots.imputation.brits.data import (
+from ...imputation.brits.data import (
     DatasetForBRITS as DatasetForBRITS_Imputation,
 )
 
 
 class DatasetForBRITS(DatasetForBRITS_Imputation):
     """Dataset class for BRITS.
```

### Comparing `pypots-0.1.0/pypots/classification/brits/model.py` & `pypots-0.1.1/pypots/classification/brits/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 from typing import Optional, Union
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.utils.data import DataLoader
 
-from pypots.classification.base import BaseNNClassifier
-from pypots.classification.brits.data import DatasetForBRITS
-from pypots.classification.brits.modules import RITS
-from pypots.imputation.brits.model import (
+from .data import DatasetForBRITS
+from .modules import RITS
+from ..base import BaseNNClassifier
+from ...imputation.brits.model import (
     _BRITS as imputation_BRITS,
 )
-from pypots.optim.adam import Adam
-from pypots.optim.base import Optimizer
+from ...optim.adam import Adam
+from ...optim.base import Optimizer
 
 
 class _BRITS(imputation_BRITS, nn.Module):
     def __init__(
         self,
         n_steps: int,
         n_features: int,
@@ -53,35 +53,37 @@
         self.rits_b = RITS(n_steps, n_features, rnn_hidden_size, n_classes, device)
         self.classification_weight = classification_weight
         self.reconstruction_weight = reconstruction_weight
 
     def impute(self, inputs: dict) -> torch.Tensor:
         return super().impute(inputs)
 
-    def classify(self, inputs: dict) -> torch.Tensor:
-        ret_f = self.rits_f(inputs, "forward")
-        ret_b = self._reverse(self.rits_b(inputs, "backward"))
-        classification_pred = (ret_f["prediction"] + ret_b["prediction"]) / 2
-        return classification_pred
-
-    def forward(self, inputs: dict) -> dict:
+    def forward(self, inputs: dict, training: bool = True) -> dict:
         """Forward processing of BRITS.
 
         Parameters
         ----------
-        inputs : dict,
+        inputs :
             The input data.
 
+        training :
+            Whether in training mode.
+
         Returns
         -------
         dict, A dictionary includes all results.
         """
         ret_f = self.rits_f(inputs, "forward")
         ret_b = self._reverse(self.rits_b(inputs, "backward"))
 
+        classification_pred = (ret_f["prediction"] + ret_b["prediction"]) / 2
+        if not training:
+            # if not in training mode, return the classification result only
+            return {"classification_pred": classification_pred}
+
         ret_f["classification_loss"] = F.nll_loss(
             torch.log(ret_f["prediction"]), inputs["label"]
         )
         ret_b["classification_loss"] = F.nll_loss(
             torch.log(ret_b["prediction"]), inputs["label"]
         )
         consistency_loss = self._get_consistency_loss(
@@ -97,87 +99,90 @@
         loss = (
             consistency_loss
             + reconstruction_loss * self.reconstruction_weight
             + classification_loss * self.classification_weight
         )
 
         results = {
+            "classification_pred": classification_pred,
             "consistency_loss": consistency_loss,
             "classification_loss": classification_loss,
             "reconstruction_loss": reconstruction_loss,
             "loss": loss,
         }
         return results
 
 
 class BRITS(BaseNNClassifier):
     """The PyTorch implementation of the BRITS model :cite:`cao2018BRITS`.
 
     Parameters
     ----------
-    n_steps : int,
+    n_steps :
         The number of time steps in the time-series data sample.
 
-    n_features : int,
+    n_features :
         The number of features in the time-series data sample.
 
-    n_classes : int,
+    n_classes :
         The number of classes in the classification task.
 
-    rnn_hidden_size : int,
+    rnn_hidden_size :
         The size of the RNN hidden state.
 
-    classification_weight : float, default = 1,
+    classification_weight :
         The loss weight for the classification task.
 
-    reconstruction_weight : float, default = 1,
+    reconstruction_weight :
         The loss weight for the reconstruction task.
 
-    batch_size : int, default = 32,
+    batch_size :
         The batch size for training and evaluating the model.
 
-    epochs : int, default = 100,
+    epochs :
         The number of epochs for training the model.
 
-    patience : int, default = None,
+    patience :
         The patience for the early-stopping mechanism. Given a positive integer, the training process will be
         stopped when the model does not perform better after that number of epochs.
         Leaving it default as None will disable the early-stopping.
 
-    optimizer : ``pypots.optim.base.Optimizer``, default = ``pypots.optim.Adam()``,
+    optimizer :
         The optimizer for model training.
         If not given, will use a default Adam optimizer.
 
-    num_workers : int, default = 0,
+    num_workers :
         The number of subprocesses to use for data loading.
         `0` means data loading will be in the main process, i.e. there won't be subprocesses.
 
-    device : str or `torch.device`, default = None,
-        The device for the model to run on.
-        If not given, will try to use CUDA devices first (will use the GPU with device number 0 only by default),
+    device :
+        The device for the model to run on. It can be a string, a :class:`torch.device` object, or a list of them.
+        If not given, will try to use CUDA devices first (will use the default CUDA device if there are multiple),
         then CPUs, considering CUDA and CPU are so far the main devices for people to train ML models.
+        If given a list of devices, e.g. ['cuda:0', 'cuda:1'], or [torch.device('cuda:0'), torch.device('cuda:1')] , the
+        model will be parallely trained on the multiple devices (so far only support parallel training on CUDA devices).
         Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
 
-    saving_path : str, default = None,
+    saving_path :
         The path for automatically saving model checkpoints and tensorboard files (i.e. loss values recorded during
         training into a tensorboard file). Will not save if not given.
 
-    model_saving_strategy : str, "best" or "better" , default = "best",
+    model_saving_strategy :
         The strategy to save model checkpoints. It has to be one of [None, "best", "better"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
 
     Attributes
     ----------
-    model : object,
+    model : :class:`torch.nn.Module`
         The underlying BRITS model.
 
-    optimizer : object,
+    optimizer : :class:`pypots.optim.Optimizer`
         The optimizer for model training.
 
     """
 
     def __init__(
         self,
         n_steps: int,
@@ -187,15 +192,15 @@
         classification_weight: float = 1,
         reconstruction_weight: float = 1,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
-        device: Optional[Union[str, torch.device]] = None,
+        device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
         model_saving_strategy: Optional[str] = "best",
     ):
         super().__init__(
             n_classes,
             batch_size,
             epochs,
@@ -218,45 +223,33 @@
             self.n_features,
             self.rnn_hidden_size,
             self.n_classes,
             self.classification_weight,
             self.reconstruction_weight,
             self.device,
         )
-        self.model = self.model.to(self.device)
+        self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
 
     def _assemble_input_for_training(self, data: dict) -> dict:
-        """Assemble the input data into a dictionary.
-
-        Parameters
-        ----------
-        data : list
-            A list containing data fetched from Dataset by Dataload.
-
-        Returns
-        -------
-        inputs : dict
-            A dictionary with data assembled.
-        """
         # fetch data
         (
             indices,
             X,
             missing_mask,
             deltas,
             back_X,
             back_missing_mask,
             back_deltas,
             label,
-        ) = map(lambda x: x.to(self.device), data)
+        ) = self._send_data_to_given_device(data)
 
         # assemble input data
         inputs = {
             "indices": indices,
             "label": label,
             "forward": {
                 "X": X,
@@ -268,60 +261,27 @@
                 "missing_mask": back_missing_mask,
                 "deltas": back_deltas,
             },
         }
         return inputs
 
     def _assemble_input_for_validating(self, data: dict) -> dict:
-        """Assemble the given data into a dictionary for validating input.
-
-        Notes
-        -----
-        The validating data assembling processing is the same as training data assembling.
-
-
-        Parameters
-        ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
-
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model validating.
-        """
         return self._assemble_input_for_training(data)
 
     def _assemble_input_for_testing(self, data: dict) -> dict:
-        """Assemble the given data into a dictionary for testing input.
-
-        Notes
-        -----
-        The testing data assembling processing is the same as training data assembling.
-
-        Parameters
-        ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
-
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model testing.
-        """
         # fetch data
         (
             indices,
             X,
             missing_mask,
             deltas,
             back_X,
             back_missing_mask,
             back_deltas,
-        ) = map(lambda x: x.to(self.device), data)
+        ) = self._send_data_to_given_device(data)
 
         # assemble input data
         inputs = {
             "indices": indices,
             "forward": {
                 "X": X,
                 "missing_mask": missing_mask,
@@ -337,44 +297,14 @@
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type: str = "h5py",
     ) -> None:
-        """Train the classifier on the given data.
-
-        Parameters
-        ----------
-        train_set : dict or str,
-            The dataset for model training, should be a dictionary including keys as 'X' and 'y',
-            or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-            which is time-series data for training, can contain missing values, and y should be array-like of shape
-            [n_samples], which is classification labels of X.
-            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-            key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
-
-        val_set : dict or str or None,
-            The dataset for model validating, should be a dictionary including keys as 'X' and 'y',
-            or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-            which is time-series data for validating, can contain missing values, and y should be array-like of shape
-            [n_samples], which is classification labels of X.
-            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-            key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
-
-        file_type : str, default = "h5py"
-            The type of the given file if train_set and val_set are path strings.
-
-        Returns
-        -------
-        self : object,
-            Trained classifier.
-        """
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForBRITS(train_set, file_type=file_type)
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
@@ -394,41 +324,26 @@
         self.model.load_state_dict(self.best_model_dict)
         self.model.eval()  # set the model as eval status to freeze it.
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(training_finished=True)
 
     def classify(self, X: Union[dict, str], file_type: str = "h5py"):
-        """Classify the input data with the trained model.
-
-        Parameters
-        ----------
-        X : array-like or str,
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
-            n_features], or a path string locating a data file, e.g. h5 file.
-
-        file_type : str, default = "h5py",
-            The type of the given file if X is a path string.
-
-        Returns
-        -------
-        array-like, shape [n_samples],
-            Classification results of the given samples.
-        """
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = DatasetForBRITS(X, return_labels=False, file_type=file_type)
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
         prediction_collector = []
 
         with torch.no_grad():
             for idx, data in enumerate(test_loader):
                 inputs = self._assemble_input_for_testing(data)
-                classification_pred = self.model.classify(inputs)
+                results = self.model.forward(inputs, training=False)
+                classification_pred = results["classification_pred"]
                 prediction_collector.append(classification_pred)
 
         predictions = torch.cat(prediction_collector)
         return predictions.cpu().detach().numpy()
```

### Comparing `pypots-0.1.0/pypots/classification/brits/modules.py` & `pypots-0.1.1/pypots/classification/brits/modules.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # License: GPL-v3
 
 from typing import Union
 
 import torch
 import torch.nn as nn
 
-from pypots.imputation.brits.model import (
+from ...imputation.brits.model import (
     RITS as imputation_RITS,
 )
 
 
 class RITS(imputation_RITS):
     def __init__(
         self,
```

### Comparing `pypots-0.1.0/pypots/classification/grud/data.py` & `pypots-0.1.1/pypots/classification/grud/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 # License: GLP-v3
 
 
 from typing import Union, Iterable
 
 import torch
 
-from pypots.data.base import BaseDataset
-from pypots.data.utils import torch_parse_delta
-from pypots.imputation.locf import LOCF
+from ...data.base import BaseDataset
+from ...data.utils import torch_parse_delta
+from ...imputation.locf import LOCF
 
 
 class DatasetForGRUD(BaseDataset):
     """Dataset class for model GRU-D.
 
     Parameters
     ----------
@@ -49,15 +49,15 @@
         file_type: str = "h5py",
     ):
         super().__init__(data, return_labels, file_type)
         self.locf = LOCF()
 
         if not isinstance(self.data, str):  # data from array
             self.missing_mask = (~torch.isnan(self.X)).to(torch.float32)
-            self.X_filledLOCF = self.locf.locf_torch(self.X)
+            self.X_filledLOCF = self.locf._locf_torch(self.X)
             self.X = torch.nan_to_num(self.X)
             self.deltas = torch_parse_delta(self.missing_mask)
             self.empirical_mean = torch.sum(
                 self.missing_mask * self.X, dim=[0, 1]
             ) / torch.sum(self.missing_mask, dim=[0, 1])
 
     def _fetch_data_from_array(self, idx: int) -> Iterable:
@@ -121,15 +121,15 @@
         """
 
         if self.file_handle is None:
             self.file_handle = self._open_file_handle()
 
         X = torch.from_numpy(self.file_handle["X"][idx])
         missing_mask = (~torch.isnan(X)).to(torch.float32)
-        X_filledLOCF = self.locf.locf_torch(X.unsqueeze(dim=0)).squeeze()
+        X_filledLOCF = self.locf._locf_torch(X.unsqueeze(dim=0)).squeeze()
         X = torch.nan_to_num(X)
         deltas = torch_parse_delta(missing_mask)
         empirical_mean = torch.sum(missing_mask * X, dim=[0]) / torch.sum(
             missing_mask, dim=[0]
         )
 
         sample = [
```

### Comparing `pypots-0.1.0/pypots/classification/raindrop/data.py` & `pypots-0.1.1/pypots/imputation/mrnn/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """
-Dataset class for model Raindrop.
+Dataset class for model MRNN.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
-
 from typing import Union
 
-from pypots.classification.grud.data import DatasetForGRUD
+from ..brits.data import DatasetForBRITS
 
 
-class DatasetForRaindrop(DatasetForGRUD):
-    """Dataset class for model GRU-D.
+class DatasetForMRNN(DatasetForBRITS):
+    """Dataset class for BRITS.
 
     Parameters
     ----------
     data : dict or str,
         The dataset for model input, should be a dictionary including keys as 'X' and 'y',
         or a path string locating a data file.
         If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
```

### Comparing `pypots-0.1.0/pypots/classification/raindrop/model.py` & `pypots-0.1.1/pypots/classification/raindrop/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,30 +17,33 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.nn import TransformerEncoderLayer, TransformerEncoder
 from torch.nn.parameter import Parameter
 from torch.utils.data import DataLoader
 
-from pypots.classification.base import BaseNNClassifier
-from pypots.classification.grud.data import DatasetForGRUD
-from pypots.classification.raindrop.modules import (
-    PositionalEncoding,
-    ObservationPropagation,
-)
-from pypots.optim.adam import Adam
-from pypots.optim.base import Optimizer
-from pypots.utils.logging import logger
+from ...classification.base import BaseNNClassifier
+from ...classification.grud.data import DatasetForGRUD
+from ...optim.adam import Adam
+from ...optim.base import Optimizer
+from ...utils.logging import logger
 
 try:
+    from .modules import PositionalEncoding, ObservationPropagation
     from torch_geometric.nn.inits import glorot
 except ImportError as e:
     logger.error(
         f"{e}\n"
-        "torch_geometric is missing, "
+        "Note torch_geometric is missing, "
+        "please install it with 'pip install torch_geometric' or 'conda install -c pyg pyg'"
+    )
+except NameError as e:
+    logger.error(
+        f"{e}\n"
+        "Note torch_geometric is missing, "
         "please install it with 'pip install torch_geometric' or 'conda install -c pyg pyg'"
     )
 
 
 class _Raindrop(nn.Module):
     def __init__(
         self,
@@ -266,111 +269,119 @@
             output = torch.cat([output, emb], dim=1)
 
         logits = self.mlp_static(output)
         prediction = torch.softmax(logits, dim=1)
 
         return prediction
 
-    def forward(self, inputs):
-        prediction = self.classify(inputs)
-        classification_loss = F.nll_loss(torch.log(prediction), inputs["label"])
+    def forward(self, inputs, training=True):
+        classification_pred = self.classify(inputs)
+        if not training:
+            # if not in training mode, return the classification result only
+            return {"classification_pred": classification_pred}
+
+        classification_loss = F.nll_loss(
+            torch.log(classification_pred), inputs["label"]
+        )
 
         results = {
-            "prediction": prediction,
+            "prediction": classification_pred,
             "loss": classification_loss
             # 'distance': distance,
         }
 
         return results
 
 
 class Raindrop(BaseNNClassifier):
     """The PyTorch implementation of the Raindrop model :cite:`zhang2022Raindrop`.
 
     Parameters
     ----------
-    n_steps : int,
+    n_steps :
         The number of time steps in the time-series data sample.
 
-    n_features : int,
+    n_features :
         The number of features in the time-series data samples.
 
-    n_classes : int,
+    n_classes :
         The number of classes in the classification task.
 
-    n_layers : int,
+    n_layers :
         The number of layers in the Transformer encoder in the Raindrop model.
 
-    d_model : int,
+    d_model :
         The dimension of the Transformer encoder backbone.
         It is the input dimension of the multi-head self-attention layers.
 
-    d_inner : int,
+    d_inner :
         The dimension of the layer in the Feed-Forward Networks (FFN).
 
-    n_heads : int,
+    n_heads :
         The number of heads in the multi-head self-attention mechanism.
 
-    dropout : float, 0<= ``dropout`` <1,
+    dropout :
         The dropout rate for all fully-connected layers in the model.
 
-    d_static : int, default = 0,
+    d_static :
         The dimension of the static features.
 
-    aggregation : str, default = "mean",
+    aggregation :
         The aggregation method for the Transformer encoder output.
 
-    sensor_wise_mask : bool, default = False,
+    sensor_wise_mask :
         Whether to apply the sensor-wise masking.
 
-    static : bool, default = False,
+    static :
         Whether to use the static features.
 
-    batch_size : int, default = 32,
+    batch_size :
         The batch size for training and evaluating the model.
 
-    epochs : int, default = 100,
+    epochs :
         The number of epochs for training the model.
 
-    patience : int, default = None,
+    patience :
         The patience for the early-stopping mechanism. Given a positive integer, the training process will be
         stopped when the model does not perform better after that number of epochs.
         Leaving it default as None will disable the early-stopping.
 
-    optimizer : ``pypots.optim.base.Optimizer``, default = ``pypots.optim.Adam()``,
+    optimizer :
         The optimizer for model training.
         If not given, will use a default Adam optimizer.
 
-    num_workers : int, default = 0,
+    num_workers :
         The number of subprocesses to use for data loading.
         `0` means data loading will be in the main process, i.e. there won't be subprocesses.
 
-    device : str or `torch.device`, default = None,
-        The device for the model to run on.
-        If not given, will try to use CUDA devices first (will use the GPU with device number 0 only by default),
+    device :
+        The device for the model to run on. It can be a string, a :class:`torch.device` object, or a list of them.
+        If not given, will try to use CUDA devices first (will use the default CUDA device if there are multiple),
         then CPUs, considering CUDA and CPU are so far the main devices for people to train ML models.
+        If given a list of devices, e.g. ['cuda:0', 'cuda:1'], or [torch.device('cuda:0'), torch.device('cuda:1')] , the
+        model will be parallely trained on the multiple devices (so far only support parallel training on CUDA devices).
         Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
 
-    saving_path : str, default = None,
+    saving_path :
         The path for automatically saving model checkpoints and tensorboard files (i.e. loss values recorded during
         training into a tensorboard file). Will not save if not given.
 
-    model_saving_strategy : str or None, None or "best" or "better" , default = "best",
+    model_saving_strategy :
         The strategy to save model checkpoints. It has to be one of [None, "best", "better"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
 
     Attributes
     ----------
-    model : object,
+    model : :class:`torch.nn.Module`
         The underlying Raindrop model.
 
-    optimizer : object,
+    optimizer : :class:`pypots.optim.Optimizer`
         The optimizer for model training.
 
     """
 
     def __init__(
         self,
         n_steps,
@@ -386,15 +397,15 @@
         sensor_wise_mask=False,
         static=False,
         batch_size=32,
         epochs=100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
-        device: Optional[Union[str, torch.device]] = None,
+        device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
         model_saving_strategy: Optional[str] = "best",
     ):
         super().__init__(
             n_classes,
             batch_size,
             epochs,
@@ -420,38 +431,32 @@
             n_steps,
             d_static,
             aggregation,
             sensor_wise_mask,
             static=static,
             device=self.device,
         )
-        self.model = self.model.to(self.device)
+        self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
 
     def _assemble_input_for_training(self, data: dict) -> dict:
-        """Assemble the input data into a dictionary.
-
-        Parameters
-        ----------
-        data : list
-            A list containing data fetched from Dataset by Dataload.
-
-        Returns
-        -------
-        inputs : dict
-            A dictionary with data assembled.
-        """
         # fetch data
-        indices, X, X_filledLOCF, missing_mask, deltas, empirical_mean, label = map(
-            lambda x: x.to(self.device), data
-        )
+        (
+            indices,
+            X,
+            X_filledLOCF,
+            missing_mask,
+            deltas,
+            empirical_mean,
+            label,
+        ) = self._send_data_to_given_device(data)
 
         bz, n_steps, n_features = X.shape
         lengths = torch.tensor([n_steps] * bz, dtype=torch.float)
         times = torch.tensor(range(n_steps), dtype=torch.float).repeat(bz, 1)
 
         X = X.permute(1, 0, 2)
         missing_mask = missing_mask.permute(1, 0, 2)
@@ -464,49 +469,25 @@
             "lengths": lengths,
             "missing_mask": missing_mask,
             "label": label,
         }
         return inputs
 
     def _assemble_input_for_validating(self, data: dict) -> dict:
-        """Assemble the given data into a dictionary for validating input.
-
-        Notes
-        -----
-        The validating data assembling processing is the same as training data assembling.
-
-
-        Parameters
-        ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
-
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model validating.
-        """
         return self._assemble_input_for_training(data)
 
     def _assemble_input_for_testing(self, data: dict) -> dict:
-        """Assemble the given data into a dictionary for testing input.
-
-        Parameters
-        ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
-
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model testing.
-        """
-        indices, X, X_filledLOCF, missing_mask, deltas, empirical_mean = map(
-            lambda x: x.to(self.device), data
-        )
+        (
+            indices,
+            X,
+            X_filledLOCF,
+            missing_mask,
+            deltas,
+            empirical_mean,
+        ) = self._send_data_to_given_device(data)
         bz, n_steps, n_features = X.shape
         lengths = torch.tensor([n_steps] * bz, dtype=torch.float)
         times = torch.tensor(range(n_steps), dtype=torch.float).repeat(bz, 1)
 
         X = X.permute(1, 0, 2)
         missing_mask = missing_mask.permute(1, 0, 2)
         times = times.permute(1, 0)
@@ -523,44 +504,14 @@
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type="h5py",
     ) -> None:
-        """Fit the model on the given training data.
-
-        Parameters
-        ----------
-        train_set : dict or str,
-            The dataset for model training, should be a dictionary including keys as 'X' and 'y',
-            or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-            which is time-series data for training, can contain missing values, and y should be array-like of shape
-            [n_samples], which is classification labels of X.
-            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-            key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
-
-        val_set : dict or str,
-            The dataset for model validating, should be a dictionary including keys as 'X' and 'y',
-            or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-            which is time-series data for validating, can contain missing values, and y should be array-like of shape
-            [n_samples], which is classification labels of X.
-            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-            key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
-
-        file_type : str, default = "h5py"
-            The type of the given file if train_set and val_set are path strings.
-
-        Returns
-        -------
-        self : object,
-            Trained model.
-        """
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForGRUD(train_set, file_type=file_type)
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
@@ -580,41 +531,26 @@
         self.model.load_state_dict(self.best_model_dict)
         self.model.eval()  # set the model as eval status to freeze it.
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(training_finished=True)
 
     def classify(self, X: Union[dict, str], file_type: str = "h5py") -> np.ndarray:
-        """Classify the input data with the trained model.
-
-        Parameters
-        ----------
-        X : array-like or str,
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
-            n_features], or a path string locating a data file, e.g. h5 file.
-
-        file_type : str, default = "h5py",
-            The type of the given file if X is a path string.
-
-        Returns
-        -------
-        array-like, shape [n_samples],
-            Classification results of the given samples.
-        """
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = DatasetForGRUD(X, return_labels=False, file_type=file_type)
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
 
         prediction_collector = []
         with torch.no_grad():
             for idx, data in enumerate(test_loader):
                 inputs = self._assemble_input_for_testing(data)
-                prediction = self.model.classify(inputs)
+                results = self.model.forward(inputs, training=False)
+                prediction = results["classification_pred"]
                 prediction_collector.append(prediction)
 
         predictions = torch.cat(prediction_collector)
         return predictions.cpu().detach().numpy()
```

### Comparing `pypots-0.1.0/pypots/classification/raindrop/modules.py` & `pypots-0.1.1/pypots/classification/raindrop/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import torch.nn as nn
 import torch.nn.functional as F
 from torch import Tensor
 from torch.nn import Linear
 from torch.nn import init
 from torch.nn.parameter import Parameter
 
-from pypots.utils.logging import logger
+from ...utils.logging import logger
 
 try:
     from torch_geometric.nn.conv import MessagePassing
     from torch_geometric.nn.inits import glorot
     from torch_geometric.typing import PairTensor, Adj, OptTensor
     from torch_geometric.utils import softmax
     from torch_scatter import scatter
```

### Comparing `pypots-0.1.0/pypots/cli/base.py` & `pypots-0.1.1/pypots/cli/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import os
 import subprocess
 import sys
 from abc import ABC, abstractmethod
 from argparse import ArgumentParser
 
-from pypots.utils.logging import logger
+from ..utils.logging import logger
 
 
 class BaseCommand(ABC):
     @staticmethod
     @abstractmethod
     def register_subcommand(parser: ArgumentParser):
         raise NotImplementedError()
```

### Comparing `pypots-0.1.0/pypots/cli/dev.py` & `pypots-0.1.1/pypots/cli/dev.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 import os
 import shutil
 from argparse import Namespace
 
-from pypots.cli.base import BaseCommand
-from pypots.utils.logging import logger
+from .base import BaseCommand
+from ..utils.logging import logger
 
 IMPORT_ERROR_MESSAGE = (
     "`pypots-cli dev` command is for PyPOTS developers to run tests easily. "
     "Therefore, you need a complete PyPOTS development environment. However, you are missing some dependencies. "
     "Please refer to https://github.com/WenjieDu/PyPOTS/blob/main/environment-dev.yml for dependency details. "
 )
```

### Comparing `pypots-0.1.0/pypots/cli/doc.py` & `pypots-0.1.1/pypots/cli/doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 
 import os
 import shutil
 from argparse import Namespace
 
 from tsdb.data_processing import _download_and_extract
 
-from pypots.cli.base import BaseCommand
-from pypots.utils.logging import logger
+from ..cli.base import BaseCommand
+from ..utils.logging import logger
 
 CLONED_LATEST_PYPOTS = "temp_pypots_latest"
 
 # These files need to be updated while generating the new documentation
 DOC_RST_FILES = [
     "pypots.rst",
     "pypots.imputation.rst",
```

### Comparing `pypots-0.1.0/pypots/cli/env.py` & `pypots-0.1.1/pypots/cli/env.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,16 +23,16 @@
         "with at least the scope of `basic` dependencies."
     )
 
 from argparse import ArgumentParser, Namespace
 
 from setuptools.config import read_configuration
 
-from pypots.cli.base import BaseCommand
-from pypots.utils.logging import logger
+from .base import BaseCommand
+from ..utils.logging import logger
 
 
 def env_command_factory(args: Namespace):
     return EnvCommand(
         args.install,
         args.tool,
     )
```

### Comparing `pypots-0.1.0/pypots/clustering/crli/data.py` & `pypots-0.1.1/pypots/clustering/crli/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 
 from typing import Union, Iterable
 
-from pypots.data.base import BaseDataset
+from ...data.base import BaseDataset
 
 
 class DatasetForCRLI(BaseDataset):
     """Dataset class for model CRLI.
 
     Parameters
     ----------
```

### Comparing `pypots-0.1.0/pypots/clustering/crli/model.py` & `pypots-0.1.1/pypots/clustering/crli/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from sklearn.cluster import KMeans
 from torch.utils.data import DataLoader
 
-from pypots.clustering.base import BaseNNClusterer
-from pypots.clustering.crli.data import DatasetForCRLI
-from pypots.clustering.crli.modules import Generator, Decoder, Discriminator
-from pypots.optim.adam import Adam
-from pypots.optim.base import Optimizer
-from pypots.utils.logging import logger
-from pypots.utils.metrics import cal_mse
+from .data import DatasetForCRLI
+from .modules import Generator, Decoder, Discriminator
+from ..base import BaseNNClusterer
+from ...optim.adam import Adam
+from ...optim.base import Optimizer
+from ...utils.logging import logger
+from ...utils.metrics import cal_mse
 
 
 class _CRLI(nn.Module):
     def __init__(
         self,
         n_steps: int,
         n_features: int,
@@ -69,25 +69,34 @@
             return inputs  # if only train discriminator, then no need to run decoder
 
         reconstruction, fcn_latent = self.decoder(inputs)
         inputs["reconstruction"] = reconstruction
         inputs["fcn_latent"] = fcn_latent
         return inputs
 
-    def forward(self, inputs: dict, training_object: str = "generator") -> dict:
+    def forward(
+        self,
+        inputs: dict,
+        training_object: str = "generator",
+        training: bool = True,
+    ) -> dict:
         assert training_object in [
             "generator",
             "discriminator",
         ], 'training_object should be "generator" or "discriminator"'
 
         X = inputs["X"]
         missing_mask = inputs["missing_mask"]
         batch_size, n_steps, n_features = X.shape
         losses = {}
         inputs = self.cluster(inputs, training_object)
+        if not training:
+            # if only run clustering, then no need to calculate loss
+            return inputs
+
         if training_object == "discriminator":
             l_D = F.binary_cross_entropy_with_logits(
                 inputs["discrimination"], missing_mask
             )
             losses["discrimination_loss"] = l_D
         else:
             inputs["discrimination"] = inputs["discrimination"].detach()
@@ -108,91 +117,93 @@
 
 
 class CRLI(BaseNNClusterer):
     """The PyTorch implementation of the CRLI model :cite:`ma2021CRLI`.
 
     Parameters
     ----------
-    n_steps : int,
+    n_steps :
         The number of time steps in the time-series data sample.
 
-    n_features : int,
+    n_features :
         The number of features in the time-series data sample.
 
-    n_clusters : int,
+    n_clusters :
         The number of clusters in the clustering task.
 
-    n_generator_layers : int,
+    n_generator_layers :
         The number of layers in the generator.
 
-    rnn_hidden_size : int,
+    rnn_hidden_size :
         The size of the RNN hidden state, also the number of hidden units in the RNN cell.
 
-    rnn_cell_type : str, default = "GRU"
+    rnn_cell_type :
         The type of RNN cell to use. Can be either "GRU" or "LSTM".
 
-    decoder_fcn_output_dims : list, default = None
+    decoder_fcn_output_dims :
         The output dimensions of each layer in the FCN (fully-connected network) of the decoder.
 
-    lambda_kmeans : float,
+    lambda_kmeans :
         The weight of the k-means loss,
         i.e. the item :math:`\\lambda` ahead of :math:`\\mathcal{L}_{k-means}` in Eq.13 of the original paper.
 
-    G_steps : int, default = 1,
+    G_steps :
         The number of steps to train the generator in each iteration.
 
-    D_steps : int, default = 1,
+    D_steps :
         The number of steps to train the discriminator in each iteration.
 
-    batch_size : int, default = 32,
+    batch_size :
         The batch size for training and evaluating the model.
 
-    epochs : int, default = 100,
+    epochs :
         The number of epochs for training the model.
 
-    patience : int, default = None,
+    patience :
         The patience for the early-stopping mechanism. Given a positive integer, the training process will be
         stopped when the model does not perform better after that number of epochs.
         Leaving it default as None will disable the early-stopping.
 
-    G_optimizer : ``pypots.optim.base.Optimizer``, default = ``pypots.optim.Adam()``,
+    G_optimizer :
         The optimizer for the generator training.
         If not given, will use a default Adam optimizer.
 
-    D_optimizer : ``pypots.optim.base.Optimizer``, default = ``pypots.optim.Adam()``,
+    D_optimizer :
         The optimizer for the discriminator training.
         If not given, will use a default Adam optimizer.
 
-    num_workers : int, default = 0,
+    num_workers :
         The number of subprocesses to use for data loading.
         `0` means data loading will be in the main process, i.e. there won't be subprocesses.
 
-    device : str or `torch.device`, default = None,
-        The device for the model to run on.
-        If not given, will try to use CUDA devices first (will use the GPU with device number 0 only by default),
+    device :
+        The device for the model to run on. It can be a string, a :class:`torch.device` object, or a list of them.
+        If not given, will try to use CUDA devices first (will use the default CUDA device if there are multiple),
         then CPUs, considering CUDA and CPU are so far the main devices for people to train ML models.
+        If given a list of devices, e.g. ['cuda:0', 'cuda:1'], or [torch.device('cuda:0'), torch.device('cuda:1')] , the
+        model will be parallely trained on the multiple devices (so far only support parallel training on CUDA devices).
         Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
 
-    saving_path : str, default = None,
+    saving_path :
         The path for automatically saving model checkpoints and tensorboard files (i.e. loss values recorded during
         training into a tensorboard file). Will not save if not given.
 
-    model_saving_strategy : str or None, None or "best" or "better" , default = "best",
+    model_saving_strategy :
         The strategy to save model checkpoints. It has to be one of [None, "best", "better"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
 
     Attributes
     ----------
-    model : object,
+    model : :class:`torch.nn.Module`
         The underlying CRLI model.
 
-    optimizer : object,
+    optimizer : :class:`pypots.optim.Optimizer`
         The optimizer for model training.
 
     """
 
     def __init__(
         self,
         n_steps: int,
@@ -207,15 +218,15 @@
         D_steps: int = 1,
         batch_size: int = 32,
         epochs: int = 100,
         patience: Optional[int] = None,
         G_optimizer: Optional[Optimizer] = Adam(),
         D_optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
-        device: Optional[Union[str, torch.device]] = None,
+        device: Optional[Union[str, torch.device, list]] = None,
         saving_path: Optional[str] = None,
         model_saving_strategy: Optional[str] = "best",
     ):
 
         super().__init__(
             n_clusters,
             batch_size,
@@ -241,89 +252,43 @@
             n_generator_layers,
             rnn_hidden_size,
             decoder_fcn_output_dims,
             lambda_kmeans,
             rnn_cell_type,
             self.device,
         )
-        self.model = self.model.to(self.device)
+        self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.G_optimizer = G_optimizer
         self.G_optimizer.init_optimizer(
             [
                 {"params": self.model.generator.parameters()},
                 {"params": self.model.decoder.parameters()},
             ]
         )
         self.D_optimizer = D_optimizer
         self.D_optimizer.init_optimizer(self.model.discriminator.parameters())
 
     def _assemble_input_for_training(self, data: list) -> dict:
-        """Assemble the given data into a dictionary for training input.
-
-        Parameters
-        ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
-
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model training.
-        """
-
         # fetch data
-        indices, X, missing_mask = map(lambda x: x.to(self.device), data)
+        indices, X, missing_mask = self._send_data_to_given_device(data)
 
         inputs = {
             "X": X,
             "missing_mask": missing_mask,
         }
 
         return inputs
 
     def _assemble_input_for_validating(self, data: list) -> dict:
-        """Assemble the given data into a dictionary for validating input.
-
-        Notes
-        -----
-        The validating data assembling processing is the same as training data assembling.
-
-
-        Parameters
-        ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
-
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model validating.
-        """
         return self._assemble_input_for_training(data)
 
     def _assemble_input_for_testing(self, data: list) -> dict:
-        """Assemble the given data into a dictionary for testing input.
-
-        Notes
-        -----
-        The testing data assembling processing is the same as training data assembling.
-
-        Parameters
-        ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
-
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model testing.
-        """
         return self._assemble_input_for_validating(data)
 
     def _train_model(
         self,
         training_loader: DataLoader,
         val_loader: DataLoader = None,
     ) -> None:
@@ -404,52 +369,36 @@
                     self.patience -= 1
                     if self.patience == 0:
                         logger.info(
                             "Exceeded the training patience. Terminating the training procedure..."
                         )
                         break
         except Exception as e:
-            logger.info(f"Exception: {e}")
+            logger.error(f"Exception: {e}")
             if self.best_model_dict is None:
                 raise RuntimeError(
-                    "Training got interrupted. Model was not get trained. Please try fit() again."
+                    "Training got interrupted. Model was not trained. Please investigate the error printed above."
                 )
             else:
                 RuntimeWarning(
-                    "Training got interrupted. "
-                    "Model will load the best parameters so far for testing. "
+                    "Training got interrupted. Please investigate the error printed above.\n"
+                    "Model got trained and will load the best checkpoint so far for testing.\n"
                     "If you don't want it, please try fit() again."
                 )
 
         if np.equal(self.best_loss, float("inf")):
             raise ValueError("Something is wrong. best_loss is Nan after training.")
 
         logger.info("Finished training.")
 
     def fit(
         self,
         train_set: Union[dict, str],
         file_type: str = "h5py",
     ) -> None:
-        """Train the cluster.
-
-        Parameters
-        ----------
-        train_set : dict or str,
-            The dataset for model training, should be a dictionary including the key 'X',
-            or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-            which is time-series data for training, can contain missing values.
-            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-            key-value pairs like a dict, and it has to include the key 'X'.
-
-        file_type : str, default = "h5py"
-            The type of the given file if train_set is a path string.
-
-        """
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForCRLI(
             train_set, return_labels=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
@@ -466,43 +415,27 @@
         self._auto_save_model_if_necessary(training_finished=True)
 
     def cluster(
         self,
         X: Union[dict, str],
         file_type: str = "h5py",
     ) -> np.ndarray:
-        """Cluster the input with the trained model.
-
-        Parameters
-        ----------
-        X : array-like or str,
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
-            n_features], or a path string locating a data file, e.g. h5 file.
-
-        file_type : str, default = "h5py"
-            The type of the given file if X is a path string.
-
-        Returns
-        -------
-        array-like, shape [n_samples],
-            Clustering results.
-        """
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = DatasetForCRLI(X, return_labels=False, file_type=file_type)
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
         latent_collector = []
 
         with torch.no_grad():
             for idx, data in enumerate(test_loader):
                 inputs = self._assemble_input_for_testing(data)
-                inputs = self.model.cluster(inputs)
+                inputs = self.model.forward(inputs, training=False)
                 latent_collector.append(inputs["fcn_latent"])
 
         latent_collector = torch.cat(latent_collector).cpu().detach().numpy()
         clustering = self.model.kmeans.fit_predict(latent_collector)
 
         return clustering
```

### Comparing `pypots-0.1.0/pypots/clustering/crli/modules.py` & `pypots-0.1.1/pypots/clustering/crli/modules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.1.0/pypots/clustering/vader/data.py` & `pypots-0.1.1/pypots/clustering/vader/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 
 from typing import Union
 
-from pypots.clustering.crli.data import DatasetForCRLI
+from ..crli.data import DatasetForCRLI
 
 
 class DatasetForVaDER(DatasetForCRLI):
     """Dataset class for model VaDER.
 
     Parameters
     ----------
```

### Comparing `pypots-0.1.0/pypots/clustering/vader/model.py` & `pypots-0.1.1/pypots/clustering/vader/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,39 +16,40 @@
 import numpy as np
 import torch
 import torch.nn as nn
 from scipy.stats import multivariate_normal
 from sklearn.mixture import GaussianMixture
 from torch.utils.data import DataLoader
 
-from pypots.clustering.base import BaseNNClusterer
-from pypots.clustering.vader.data import DatasetForVaDER
-from pypots.clustering.vader.modules import (
+from .data import DatasetForVaDER
+from .modules import (
+    inverse_softplus,
     GMMLayer,
     PeepholeLSTMCell,
     ImplicitImputation,
 )
-from pypots.optim.adam import Adam
-from pypots.optim.base import Optimizer
-from pypots.utils.logging import logger
-from pypots.utils.metrics import cal_mse
+from ..base import BaseNNClusterer
+from ...optim.adam import Adam
+from ...optim.base import Optimizer
+from ...utils.logging import logger
+from ...utils.metrics import cal_mse
 
 
 class _VaDER(nn.Module):
     """
 
     Parameters
     ----------
     n_steps :
     d_input :
     n_clusters :
     d_rnn_hidden :
     d_mu_stddev :
     eps :
-    alpha : float, default=1.0
+    alpha :
         Weight of the latent loss.
         The final loss = `alpha`*latent loss + reconstruction loss
 
 
     Attributes
     ----------
 
@@ -159,61 +160,43 @@
         torch.Tensor,
     ]:
         z, mu_tilde, stddev_tilde = self.encode(X, missing_mask)
         X_reconstructed = self.decode(z)
         mu_c, var_c, phi_c = self.gmm_layer()
         return X_reconstructed, mu_c, var_c, phi_c, z, mu_tilde, stddev_tilde
 
-    def cluster(self, inputs: dict) -> np.ndarray:
+    def forward(
+        self,
+        inputs: dict,
+        pretrain: bool = False,
+        training: bool = True,
+    ) -> dict:
         X, missing_mask = inputs["X"], inputs["missing_mask"]
-        (
-            X_reconstructed,
-            mu_c,
-            var_c,
-            phi_c,
-            z,
-            mu_tilde,
-            stddev_tilde,
-        ) = self.get_results(X, missing_mask)
-
-        def func_to_apply(
-            mu_t_: np.ndarray, mu_: np.ndarray, stddev_: np.ndarray, phi_: np.ndarray
-        ) -> np.ndarray:
-            # the covariance matrix is diagonal, so we can just take the product
-            return np.log(self.eps + phi_) + np.log(
-                self.eps
-                + multivariate_normal.pdf(mu_t_, mean=mu_, cov=np.diag(stddev_))
-            )
-
-        mu_tilde = mu_tilde.detach().cpu().numpy()
-        mu = mu_c.detach().cpu().numpy()
-        var = var_c.detach().cpu().numpy()
-        phi = phi_c.detach().cpu().numpy()
-        p = np.array(
-            [
-                func_to_apply(mu_tilde, mu[i], var[i], phi[i])
-                for i in np.arange(mu.shape[0])
-            ]
-        )
-        clustering_results = np.argmax(p, axis=0)
-        return clustering_results
+        device = X.device
 
-    def forward(self, inputs: dict, pretrain: bool = False) -> dict:
-        X, missing_mask = inputs["X"], inputs["missing_mask"]
         (
             X_reconstructed,
             mu_c,
             var_c,
             phi_c,
             z,
             mu_tilde,
             stddev_tilde,
         ) = self.get_results(X, missing_mask)
 
-        device = X.device
+        if not training and not pretrain:
+
+            results = {
+                "mu_tilde": mu_tilde,
+                "mu": mu_c,
+                "var": var_c,
+                "phi": phi_c,
+            }
+            # if only run clustering, then no need to calculate loss
+            return results
 
         # calculate the reconstruction loss
         unscaled_reconstruction_loss = cal_mse(X_reconstructed, X, missing_mask)
         reconstruction_loss = (
             unscaled_reconstruction_loss
             * self.n_steps
             * self.d_input
@@ -271,89 +254,86 @@
         latent_loss3 = -0.5 * torch.sum(1 + stddev_tilde, dim=1)
 
         latent_loss1 = latent_loss1.mean()
         latent_loss2 = latent_loss2.mean()
         latent_loss3 = latent_loss3.mean()
         latent_loss = latent_loss1 + latent_loss2 + latent_loss3
 
-        results = {"loss": reconstruction_loss + self.alpha * latent_loss, "z": z}
+        results = {
+            "loss": reconstruction_loss + self.alpha * latent_loss,
+            "z": z,
+        }
 
         return results
 
 
-def inverse_softplus(x: np.ndarray) -> np.ndarray:
-    b = x < 1e2
-    x[b] = np.log(np.exp(x[b]) - 1.0 + 1e-9)
-    return x
-
-
 class VaDER(BaseNNClusterer):
     """The PyTorch implementation of the VaDER model :cite:`dejong2019VaDER`.
 
     Parameters
     ----------
-    n_steps : int,
+    n_steps :
         The number of time steps in the time-series data sample.
 
-    n_features : int,
+    n_features :
         The number of features in the time-series data sample.
 
-    n_clusters : int,
+    n_clusters :
         The number of clusters in the clustering task.
 
-    rnn_hidden_size : int,
+    rnn_hidden_size :
         The size of the RNN hidden state, also the number of hidden units in the RNN cell.
 
-    d_mu_stddev : int,
+    d_mu_stddev :
         The dimension of the mean and standard deviation of the Gaussian distribution.
 
-    batch_size : int, default = 32,
+    batch_size :
         The batch size for training and evaluating the model.
 
-    pretrain_epochs : int, default = 10,
+    pretrain_epochs :
         The number of epochs for pretraining the model.
 
-    epochs : int, default = 100,
+    epochs :
         The number of epochs for training the model.
 
-    patience : int, default = None,
+    patience :
         The patience for the early-stopping mechanism. Given a positive integer, the training process will be
         stopped when the model does not perform better after that number of epochs.
         Leaving it default as None will disable the early-stopping.
 
-    optimizer : ``pypots.optim.base.Optimizer``, default = ``pypots.optim.Adam()``,
+    optimizer :
         The optimizer for model training.
         If not given, will use a default Adam optimizer.
-    num_workers : int, default = 0,
+    num_workers :
         The number of subprocesses to use for data loading.
         `0` means data loading will be in the main process, i.e. there won't be subprocesses.
 
-    device : str or `torch.device`, default = None,
+    device :
         The device for the model to run on.
         If not given, will try to use CUDA devices first (will use the GPU with device number 0 only by default),
         then CPUs, considering CUDA and CPU are so far the main devices for people to train ML models.
         Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
 
-    saving_path : str, default = None,
+    saving_path :
         The path for automatically saving model checkpoints and tensorboard files (i.e. loss values recorded during
         training into a tensorboard file). Will not save if not given.
 
-    model_saving_strategy : str or None, None or "best" or "better" , default = "best",
+    model_saving_strategy :
         The strategy to save model checkpoints. It has to be one of [None, "best", "better"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
 
     Attributes
     ----------
-    model : object,
+    model : :class:`torch.nn.Module`
         The underlying VaDER model.
 
-    optimizer : object,
+    optimizer : :class:`pypots.optim.Optimizer`
         The optimizer for model training.
 
     """
 
     def __init__(
         self,
         n_steps: int,
@@ -363,104 +343,63 @@
         d_mu_stddev: int,
         batch_size: int = 32,
         epochs: int = 100,
         pretrain_epochs: int = 10,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
-        device: Optional[Union[str, torch.device]] = None,
+        device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
         model_saving_strategy: Optional[str] = "best",
     ):
         super().__init__(
             n_clusters,
             batch_size,
             epochs,
             patience,
             num_workers,
             device,
             saving_path,
             model_saving_strategy,
         )
+
+        assert (
+            pretrain_epochs > 0
+        ), f"pretrain_epochs must be a positive integer, but got {pretrain_epochs}"
+
         self.n_steps = n_steps
         self.n_features = n_features
         self.pretrain_epochs = pretrain_epochs
 
         # set up the model
         self.model = _VaDER(
             n_steps, n_features, n_clusters, rnn_hidden_size, d_mu_stddev
         )
-        self.model = self.model.to(self.device)
+        self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
 
     def _assemble_input_for_training(self, data: list) -> dict:
-        """Assemble the given data into a dictionary for training input.
-
-        Parameters
-        ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
-
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model training.
-        """
-
         # fetch data
-        indices, X, missing_mask = map(lambda x: x.to(self.device), data)
+        indices, X, missing_mask = self._send_data_to_given_device(data)
 
         inputs = {
             "X": X,
             "missing_mask": missing_mask,
         }
 
         return inputs
 
     def _assemble_input_for_validating(self, data: list) -> dict:
-        """Assemble the given data into a dictionary for validating input.
-
-        Notes
-        -----
-        The validating data assembling processing is the same as training data assembling.
-
-
-        Parameters
-        ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
-
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model validating.
-        """
         return self._assemble_input_for_training(data)
 
     def _assemble_input_for_testing(self, data: list) -> dict:
-        """Assemble the given data into a dictionary for testing input.
-
-        Notes
-        -----
-        The testing data assembling processing is the same as training data assembling.
-
-        Parameters
-        ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
-
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model testing.
-        """
         return self._assemble_input_for_validating(data)
 
     def _train_model(
         self,
         training_loader: DataLoader,
         val_loader: DataLoader = None,
     ) -> None:
@@ -474,15 +413,15 @@
         for epoch in range(self.pretrain_epochs):
             self.model.train()
             for idx, data in enumerate(training_loader):
                 pretraining_step += 1
                 inputs = self._assemble_input_for_training(data)
                 self.optimizer.zero_grad()
                 results = self.model.forward(inputs, pretrain=True)
-                results["loss"].backward()
+                results["loss"].sum().backward()
                 self.optimizer.step()
 
                 # save pre-training loss logs into the tensorboard file for every step if in need
                 if self.summary_writer is not None:
                     self._save_log_into_tb_file(
                         pretraining_step, "pretraining", results
                     )
@@ -528,37 +467,46 @@
                         exit()
                     else:
                         reg_covar *= 2
 
                     continue
 
             # get GMM parameters
-            phi = np.log(gmm.weights_ + 1e-9)  # inverse softmax
             mu = gmm.means_
             var = inverse_softplus(gmm.covariances_)
+            phi = np.log(gmm.weights_ + 1e-9)  # inverse softmax
+            device = results["z"].device
+
             # use trained GMM's parameters to init GMM layer's
-            self.model.gmm_layer.set_values(
-                torch.from_numpy(mu).to(self.device),
-                torch.from_numpy(var).to(self.device),
-                torch.from_numpy(phi).to(self.device),
-            )
+            if isinstance(self.device, list):  # if using multi-GPU
+                self.model.module.gmm_layer.set_values(
+                    torch.from_numpy(mu).to(device),
+                    torch.from_numpy(var).to(device),
+                    torch.from_numpy(phi).to(device),
+                )
+            else:
+                self.model.gmm_layer.set_values(
+                    torch.from_numpy(mu).to(device),
+                    torch.from_numpy(var).to(device),
+                    torch.from_numpy(phi).to(device),
+                )
 
         try:
             training_step = 0
             for epoch in range(self.epochs):
                 self.model.train()
                 epoch_train_loss_collector = []
                 for idx, data in enumerate(training_loader):
                     training_step += 1
                     inputs = self._assemble_input_for_training(data)
                     self.optimizer.zero_grad()
                     results = self.model.forward(inputs)
-                    results["loss"].backward()
+                    results["loss"].sum().backward()
                     self.optimizer.step()
-                    epoch_train_loss_collector.append(results["loss"].item())
+                    epoch_train_loss_collector.append(results["loss"].sum().item())
 
                     # save training loss logs into the tensorboard file for every step if in need
                     if self.summary_writer is not None:
                         self._save_log_into_tb_file(training_step, "training", results)
 
                 # mean training loss of the current epoch
                 mean_train_loss = np.mean(epoch_train_loss_collector)
@@ -566,15 +514,17 @@
                 if val_loader is not None:
                     self.model.eval()
                     epoch_val_loss_collector = []
                     with torch.no_grad():
                         for idx, data in enumerate(val_loader):
                             inputs = self._assemble_input_for_validating(data)
                             results = self.model.forward(inputs)
-                            epoch_val_loss_collector.append(results["loss"].item())
+                            epoch_val_loss_collector.append(
+                                results["loss"].sum().item()
+                            )
 
                     mean_val_loss = np.mean(epoch_val_loss_collector)
 
                     # save validating loss logs into the tensorboard file for every epoch if in need
                     if self.summary_writer is not None:
                         val_loss_dict = {
                             "loss": mean_val_loss,
@@ -604,56 +554,36 @@
                     self.patience -= 1
                     if self.patience == 0:
                         logger.info(
                             "Exceeded the training patience. Terminating the training procedure..."
                         )
                         break
         except Exception as e:
-            logger.info(f"Exception: {e}")
+            logger.error(f"Exception: {e}")
             if self.best_model_dict is None:
                 raise RuntimeError(
-                    "Training got interrupted. Model was not get trained. Please try fit() again."
+                    "Training got interrupted. Model was not trained. Please investigate the error printed above."
                 )
             else:
                 RuntimeWarning(
-                    "Training got interrupted. "
-                    "Model will load the best parameters so far for testing. "
+                    "Training got interrupted. Please investigate the error printed above.\n"
+                    "Model got trained and will load the best checkpoint so far for testing.\n"
                     "If you don't want it, please try fit() again."
                 )
 
         if np.equal(self.best_loss, float("inf")):
             raise ValueError("Something is wrong. best_loss is Nan after training.")
 
         logger.info("Finished training.")
 
     def fit(
         self,
         train_set: Union[dict, str],
         file_type: str = "h5py",
     ) -> None:
-        """Train the cluster.
-
-        Parameters
-        ----------
-        train_set : dict or str,
-            The dataset for model training, should be a dictionary including the key 'X',
-            or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-            which is time-series data for training, can contain missing values.
-            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-            key-value pairs like a dict, and it has to include the key 'X'.
-
-        file_type : str, default = "h5py"
-            The type of the given file if train_set is a path string.
-
-        Returns
-        -------
-        self : object,
-            Trained classifier.
-        """
         # Step 1: wrap the input data with classes Dataset and DataLoader
         training_set = DatasetForVaDER(
             train_set, return_labels=False, file_type=file_type
         )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
@@ -666,41 +596,50 @@
         self.model.load_state_dict(self.best_model_dict)
         self.model.eval()  # set the model as eval status to freeze it.
 
         # Step 3: save the model if necessary
         self._auto_save_model_if_necessary(training_finished=True)
 
     def cluster(self, X: Union[dict, str], file_type: str = "h5py") -> np.ndarray:
-        """Cluster the input with the trained model.
-
-        Parameters
-        ----------
-        X : array-like or str,
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
-            n_features], or a path string locating a data file, e.g. h5 file.
-
-        file_type : str, default = "h5py"
-            The type of the given file if X is a path string.
-
-        Returns
-        -------
-        array-like, shape [n_samples],
-            Clustering results.
-        """
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = DatasetForVaDER(X, return_labels=False, file_type=file_type)
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
         clustering_results_collector = []
 
         with torch.no_grad():
             for idx, data in enumerate(test_loader):
                 inputs = self._assemble_input_for_testing(data)
-                results = self.model.cluster(inputs)
-                clustering_results_collector.append(results)
+                results = self.model.forward(inputs, training=False)
+
+                mu_tilde = results["mu_tilde"].cpu().numpy()
+                mu = results["mu"].cpu().numpy()
+                var = results["var"].cpu().numpy()
+                phi = results["phi"].cpu().numpy()
+
+                def func_to_apply(
+                    mu_t_: np.ndarray,
+                    mu_: np.ndarray,
+                    stddev_: np.ndarray,
+                    phi_: np.ndarray,
+                ) -> np.ndarray:
+                    # the covariance matrix is diagonal, so we can just take the product
+                    return np.log(1e-9 + phi_) + np.log(
+                        1e-9
+                        + multivariate_normal.pdf(mu_t_, mean=mu_, cov=np.diag(stddev_))
+                    )
+
+                p = np.array(
+                    [
+                        func_to_apply(mu_tilde, mu[i], var[i], phi[i])
+                        for i in np.arange(mu.shape[0])
+                    ]
+                )
+                clustering_results = np.argmax(p, axis=0)
+                clustering_results_collector.append(clustering_results)
 
         clustering_results = np.concatenate(clustering_results_collector)
         return clustering_results
```

### Comparing `pypots-0.1.0/pypots/clustering/vader/modules.py` & `pypots-0.1.1/pypots/clustering/vader/modules.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,21 +9,28 @@
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 
 from typing import Tuple, Optional
 
+import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.autograd import Variable
 from torch.nn.parameter import Parameter
 
 
+def inverse_softplus(x: np.ndarray) -> np.ndarray:
+    b = x < 1e2
+    x[b] = np.log(np.exp(x[b]) - 1.0 + 1e-9)
+    return x
+
+
 class ImplicitImputation(nn.Module):
     def __init__(self, d_input: int):
         super().__init__()
         self.projection_layer = nn.Linear(d_input, d_input, bias=False)
 
     def forward(self, X: torch.Tensor, missing_mask: torch.Tensor) -> torch.Tensor:
         imputation = self.projection_layer(X)
@@ -90,27 +97,27 @@
 
 
 class GMMLayer(nn.Module):
     def __init__(self, d_hidden: int, n_clusters: int):
         super().__init__()
         self.mu_c_unscaled = Parameter(torch.Tensor(n_clusters, d_hidden))
         self.var_c_unscaled = Parameter(torch.Tensor(n_clusters, d_hidden))
-        self.phi_c_unscaled = torch.Tensor(n_clusters)
+        self.phi_c_unscaled = Parameter(torch.Tensor(n_clusters))
 
     def set_values(
         self,
         mu: torch.Tensor,
         var: torch.Tensor,
         phi: torch.Tensor,
     ) -> None:
         assert mu.shape == self.mu_c_unscaled.shape
         assert var.shape == self.var_c_unscaled.shape
         assert phi.shape == self.phi_c_unscaled.shape
         self.mu_c_unscaled = torch.nn.Parameter(mu)
         self.var_c_unscaled = torch.nn.Parameter(var)
-        self.phi_c_unscaled = phi
+        self.phi_c_unscaled = torch.nn.Parameter(phi)
 
     def forward(self) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         mu_c = self.mu_c_unscaled
         var_c = F.softplus(self.var_c_unscaled)
         phi_c = torch.softmax(self.phi_c_unscaled, dim=0)
         return mu_c, var_c, phi_c
```

### Comparing `pypots-0.1.0/pypots/data/__init__.py` & `pypots-0.1.1/pypots/data/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """
 Expose all usable data manipulation classes and functions.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GPL-v3
 
-from pypots.data.base import BaseDataset
-from pypots.data.generating import (
+from .base import BaseDataset
+from .generating import (
     gene_complete_random_walk,
     gene_random_walk_for_classification,
     gene_incomplete_random_walk_dataset,
     gene_physionet2012,
 )
-from pypots.data.load_specific_datasets import (
+from .load_specific_datasets import (
     list_supported_datasets,
     load_specific_dataset,
 )
-from pypots.data.utils import (
+from .utils import (
     masked_fill,
     mcar,
     pickle_load,
     pickle_dump,
 )
 
 __all__ = [
```

### Comparing `pypots-0.1.0/pypots/data/base.py` & `pypots-0.1.1/pypots/forecasting/bttf/model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,312 +1,377 @@
 """
-The base class for PyPOTS datasets.
+The implementation of BTTF (Bayesian Temporal Tensor Factorization) for the partially-observed time-series
+forecasting task.
+
+Refer to the paper "Chen, X., & Sun, L. (2021).
+Bayesian Temporal Factorization for Multidimensional Time Series Prediction.
+IEEE transactions on pattern analysis and machine intelligence."
+
+Notes
+-----
+This numpy implementation is the same with the official one from https://github.com/xinychen/transdim.
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
-# License: GPL-v3
+# License: GLP-v3
 
-from abc import abstractmethod
-from typing import Union, Optional, Tuple, Iterable
+import warnings
+from typing import Union, Optional
 
-import h5py
 import numpy as np
 import torch
-from torch.utils.data import Dataset
+from numpy.linalg import inv as inv
+from numpy.linalg import solve as solve
+from scipy.linalg import khatri_rao as kr_prod
+
+from .modules import (
+    mvnrnd_pre,
+    ten2mat,
+    sample_factor_u,
+    sample_factor_v,
+    sample_factor_x,
+    sample_var_coefficient,
+    ar4cast,
+)
+from ..base import BaseForecaster
+
+
+def _BTTF(
+    dense_tensor,
+    sparse_tensor,
+    init,
+    rank,
+    time_lags,
+    burn_iter,
+    gibbs_iter,
+    multi_step=1,
+):
+    """Bayesian Temporal Tensor Factorization, BTTF."""
+
+    dim1, dim2, dim3 = sparse_tensor.shape
+    d = time_lags.shape[0]
+    U = init["U"]
+    V = init["V"]
+    X = init["X"]
+    if not np.isnan(sparse_tensor).any():
+        ind = sparse_tensor != 0
+        pos_test = np.where((dense_tensor != 0) & (sparse_tensor == 0))
+    elif np.isnan(sparse_tensor).any():
+        pos_test = np.where((dense_tensor != 0) & (np.isnan(sparse_tensor)))
+        ind = ~np.isnan(sparse_tensor)
+        # pos_obs = np.where(ind)
+        sparse_tensor[np.isnan(sparse_tensor)] = 0
+    # dense_test = dense_tensor[pos_test]
+    del dense_tensor
+    U_plus = np.zeros((dim1, rank, gibbs_iter))
+    V_plus = np.zeros((dim2, rank, gibbs_iter))
+    X_plus = np.zeros((dim3 + multi_step, rank, gibbs_iter))
+    A_plus = np.zeros((rank * d, rank, gibbs_iter))
+    tau_plus = np.zeros(gibbs_iter)
+    Sigma_plus = np.zeros((rank, rank, gibbs_iter))
+    temp_hat = np.zeros(len(pos_test[0]))
+    show_iter = 500
+    tau = 1
+    tensor_hat_plus = np.zeros(sparse_tensor.shape)
+    tensor_new_plus = np.zeros((dim1, dim2, multi_step))
+    for it in range(burn_iter + gibbs_iter):
+        tau_ind = tau * ind
+        tau_sparse_tensor = tau * sparse_tensor
+        U = sample_factor_u(tau_sparse_tensor, tau_ind, U, V, X)
+        V = sample_factor_v(tau_sparse_tensor, tau_ind, U, V, X)
+        A, Sigma = sample_var_coefficient(X, time_lags)
+        X = sample_factor_x(
+            tau_sparse_tensor, tau_ind, time_lags, U, V, X, A, inv(Sigma)
+        )
+        tensor_hat = np.einsum("is, js, ts -> ijt", U, V, X)
+        tau = np.random.gamma(
+            1e-6 + 0.5 * np.sum(ind),
+            1 / (1e-6 + 0.5 * np.sum(((sparse_tensor - tensor_hat) ** 2) * ind)),
+        )
+        temp_hat += tensor_hat[pos_test]
+        if (it + 1) % show_iter == 0 and it < burn_iter:
+            # temp_hat = temp_hat / show_iter
+            # logger.info('Iter: {}'.format(it + 1))
+            # logger.info('MAPE: {:.6}'.format(compute_mape(dense_test, temp_hat)))
+            # logger.info('RMSE: {:.6}'.format(compute_rmse(dense_test, temp_hat)))
+            temp_hat = np.zeros(len(pos_test[0]))
+        if it + 1 > burn_iter:
+            U_plus[:, :, it - burn_iter] = U
+            V_plus[:, :, it - burn_iter] = V
+            A_plus[:, :, it - burn_iter] = A
+            Sigma_plus[:, :, it - burn_iter] = Sigma
+            tau_plus[it - burn_iter] = tau
+            tensor_hat_plus += tensor_hat
+            X0 = ar4cast(A, X, Sigma, time_lags, multi_step)
+            X_plus[:, :, it - burn_iter] = X0
+            tensor_new_plus += np.einsum("is, js, ts -> ijt", U, V, X0[-multi_step:, :])
+    tensor_hat = tensor_hat_plus / gibbs_iter
+    # logger.info('Imputation MAPE: {:.6}'.format(compute_mape(dense_test, tensor_hat[:, :, : dim3][pos_test])))
+    # logger.info('Imputation RMSE: {:.6}'.format(compute_rmse(dense_test, tensor_hat[:, :, : dim3][pos_test])))
+    tensor_hat = np.append(tensor_hat, tensor_new_plus / gibbs_iter, axis=2)
+    tensor_hat[tensor_hat < 0] = 0
+
+    return tensor_hat, U_plus, V_plus, X_plus, A_plus, Sigma_plus, tau_plus
+
+
+def sample_factor_x_partial(
+    tau_sparse_tensor, tau_ind, time_lags, U, V, X, A, Lambda_x, back_step
+):
+    """Sampling T-by-R factor matrix X."""
+
+    dim3, rank = X.shape
+    tmax = np.max(time_lags)
+    tmin = np.min(time_lags)
+    d = time_lags.shape[0]
+    A0 = np.dstack([A] * d)
+    for k in range(d):
+        A0[k * rank : (k + 1) * rank, :, k] = 0
+    mat0 = Lambda_x @ A.T
+    mat1 = np.einsum("kij, jt -> kit", A.reshape([d, rank, rank]), Lambda_x)
+    mat2 = np.einsum("kit, kjt -> ij", mat1, A.reshape([d, rank, rank]))
+
+    var1 = kr_prod(V, U).T
+    var2 = kr_prod(var1, var1)
+    var3 = (var2 @ ten2mat(tau_ind[:, :, -back_step:], 2).T).reshape(
+        [rank, rank, back_step]
+    ) + Lambda_x[:, :, None]
+    var4 = var1 @ ten2mat(tau_sparse_tensor[:, :, -back_step:], 2).T
+    for t in range(dim3 - back_step, dim3):
+        Mt = np.zeros((rank, rank))
+        Nt = np.zeros(rank)
+        Qt = mat0 @ X[t - time_lags, :].reshape(rank * d)
+        index = list(range(0, d))
+        if dim3 - tmax <= t < dim3 - tmin:
+            index = list(np.where(t + time_lags < dim3))[0]
+        if t < dim3 - tmin:
+            Mt = mat2.copy()
+            temp = np.zeros((rank * d, len(index)))
+            n = 0
+            for k in index:
+                temp[:, n] = X[t + time_lags[k] - time_lags, :].reshape(rank * d)
+                n += 1
+            temp0 = X[t + time_lags[index], :].T - np.einsum(
+                "ijk, ik -> jk", A0[:, :, index], temp
+            )
+            Nt = np.einsum("kij, jk -> i", mat1[index, :, :], temp0)
+        var3[:, :, t + back_step - dim3] = var3[:, :, t + back_step - dim3] + Mt
+        X[t, :] = mvnrnd_pre(
+            solve(
+                var3[:, :, t + back_step - dim3],
+                var4[:, t + back_step - dim3] + Nt + Qt,
+            ),
+            var3[:, :, t + back_step - dim3],
+        )
+    return X
 
-# Currently we only support h5 files
-SUPPORTED_DATASET_FILE_TYPE = ["h5py"]
 
+def _BTTF_partial(
+    sparse_tensor, init, rank, time_lags, gibbs_iter, multi_step=1, gamma=10
+):
+    """Bayesian Temporal Tensor Factorization, BTTF."""
+
+    dim1, dim2, dim3 = sparse_tensor.shape
+    U_plus = init["U_plus"]
+    V_plus = init["V_plus"]
+    X_plus = init["X_plus"]
+    A_plus = init["A_plus"]
+    Sigma_plus = init["Sigma_plus"]
+    tau_plus = init["tau_plus"]
+    if not np.isnan(sparse_tensor).any():
+        ind = sparse_tensor != 0
+    elif np.isnan(sparse_tensor).any():
+        ind = ~np.isnan(sparse_tensor)
+        sparse_tensor[np.isnan(sparse_tensor)] = 0
+    X_new_plus = np.zeros((dim3 + multi_step, rank, gibbs_iter))
+    tensor_new_plus = np.zeros((dim1, dim2, multi_step))
+    back_step = gamma * multi_step
+    for it in range(gibbs_iter):
+        tau_ind = tau_plus[it] * ind
+        tau_sparse_tensor = tau_plus[it] * sparse_tensor
+        X = sample_factor_x_partial(
+            tau_sparse_tensor,
+            tau_ind,
+            time_lags,
+            U_plus[:, :, it],
+            V_plus[:, :, it],
+            X_plus[:, :, it],
+            A_plus[:, :, it],
+            inv(Sigma_plus[:, :, it]),
+            back_step,
+        )
+        X0 = ar4cast(A_plus[:, :, it], X, Sigma_plus[:, :, it], time_lags, multi_step)
+        X_new_plus[:, :, it] = X0
+        tensor_new_plus += np.einsum(
+            "is, js, ts -> ijt", U_plus[:, :, it], V_plus[:, :, it], X0[-multi_step:, :]
+        )
+    tensor_hat = tensor_new_plus / gibbs_iter
+    tensor_hat[tensor_hat < 0] = 0
 
-class BaseDataset(Dataset):
-    """Base dataset class in PyPOTS.
+    return tensor_hat, U_plus, V_plus, X_new_plus, A_plus, Sigma_plus, tau_plus
 
-    Parameters
-    ----------
-    data : dict or str,
-        The dataset for model input, should be a dictionary including keys as 'X' and 'y',
-        or a path string locating a data file.
-        If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-        which is time-series data for input, can contain missing values, and y should be array-like of shape
-        [n_samples], which is classification labels of X.
-        If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-        key-value pairs like a dict, and it has to include keys as 'X' and 'y'.
-
-    return_labels : bool, default = True,
-        Whether to return labels in function __getitem__() if they exist in the given data. If `True`, for example,
-        during training of classification models, the Dataset class will return labels in __getitem__() for model input.
-        Otherwise, labels won't be included in the data returned by __getitem__(). This parameter exists because we
-        need the defined Dataset class for all training/validating/testing stages. For those big datasets stored in h5
-        files, they already have both X and y saved. But we don't read labels from the file for validating and testing
-        with function _fetch_data_from_file(), which works for all three stages. Therefore, we need this parameter for
-        distinction.
 
-    file_type : str, default = "h5py"
-        The type of the given file if train_set and val_set are path strings.
+def BTTF_forecast(
+    dense_tensor,
+    sparse_tensor,
+    pred_step,
+    multi_step,
+    rank,
+    time_lags,
+    burn_iter,
+    gibbs_iter,
+    gamma=10,
+):
+    dim1, dim2, T = dense_tensor.shape
+    start_time = T - pred_step
+    max_count = int(np.ceil(pred_step / multi_step))
+    tensor_hat = np.zeros((dim1, dim2, max_count * multi_step))
+
+    # t==0
+    init = {
+        "U": 0.1 * np.random.randn(dim1, rank),
+        "V": 0.1 * np.random.randn(dim2, rank),
+        "X": 0.1 * np.random.randn(start_time, rank),
+    }
+    tensor, U, V, X_new, A, Sigma, tau = _BTTF(
+        dense_tensor[:, :, :start_time],
+        sparse_tensor[:, :, :start_time],
+        init,
+        rank,
+        time_lags,
+        burn_iter,
+        gibbs_iter,
+        multi_step,
+    )
+    tensor_hat[:, :, 0:multi_step] = tensor[:, :, -multi_step:]
+    # 1<= t <max_count
+    for t in range(1, max_count):
+        init = {
+            "U_plus": U,
+            "V_plus": V,
+            "X_plus": X_new,
+            "A_plus": A,
+            "Sigma_plus": Sigma,
+            "tau_plus": tau,
+        }
+        tensor, U, V, X_new, A, Sigma, tau = _BTTF_partial(
+            sparse_tensor[:, :, : start_time + t * multi_step],
+            init,
+            rank,
+            time_lags,
+            gibbs_iter,
+            multi_step,
+            gamma,
+        )
+        tensor_hat[:, :, t * multi_step : (t + 1) * multi_step] = tensor[
+            :, :, -multi_step:
+        ]
+    return tensor_hat
 
-    """
 
-    def __init__(
-        self,
-        data: Union[dict, str],
-        return_labels: bool = True,
-        file_type: str = "h5py",
-    ):
-        super().__init__()
-        # types and shapes had been checked after X and y input into the model
-        # So they are safe to use here. No need to check again.
-
-        self.data = data
-        self.return_labels = return_labels
-        if isinstance(self.data, str):  # data from file
-            # check if the given file type is supported
-            assert (
-                file_type in SUPPORTED_DATASET_FILE_TYPE
-            ), f"file_type should be one of {SUPPORTED_DATASET_FILE_TYPE}, but got {file_type}"
-
-            self.file_type = file_type
-
-            # open the file handle
-            self.file_handle = self._open_file_handle()
-            # check if X exists in the file
-            assert (
-                "X" in self.file_handle.keys()
-            ), "The given dataset file doesn't contains X. Please double check."
-
-        else:  # data from array
-            X = data["X"]
-            y = None if "y" not in data.keys() else data["y"]
-            self.X, self.y = self._check_input(X, y)
-
-        self.sample_num = self._get_sample_num()
-
-        # set up function fetch_data()
-        if isinstance(self.data, str):
-            self.fetch_data = self._fetch_data_from_file
-        else:
-            self.fetch_data = self._fetch_data_from_array
-
-    def _get_sample_num(self) -> int:
-        """Determine the number of samples in the dataset and return the number.
-
-        Returns
-        -------
-        sample_num : int
-            The number of the samples in the given dataset.
-        """
-        if isinstance(self.data, str):
-            if self.file_handle is None:
-                self.file_handle = self._open_file_handle()
-            sample_num = len(self.file_handle["X"])
-        else:
-            sample_num = len(self.X)
-
-        return sample_num
-
-    def __len__(self) -> int:
-        return self.sample_num
-
-    @staticmethod
-    def _check_input(
-        X: Union[np.ndarray, torch.Tensor, list],
-        y: Optional[Union[np.ndarray, torch.Tensor, list]] = None,
-        out_dtype: str = "tensor",
-    ) -> Tuple[
-        Union[np.ndarray, torch.Tensor, list],
-        Optional[Union[np.ndarray, torch.Tensor, list]],
-    ]:
-        """Check value type and shape of input X and y
-
-        Parameters
-        ----------
-        X : array-like,
-            Time-series data that must have a shape like [n_samples, expected_n_steps, expected_n_features].
-
-        y : array-like, default=None
-            Labels of time-series samples (X) that must have a shape like [n_samples] or [n_samples, n_classes].
-
-        out_dtype : str, in ['tensor', 'ndarray'], default='tensor'
-            Data type of the output, should be np.ndarray or torch.Tensor
-
-        Returns
-        -------
-        X : array-like
+class BTTF(BaseForecaster):
+    """The implementation of the BTTF model :cite:`chen2021BTMF`.
+
+    Parameters
+    ----------
+    n_steps : int,
+        The number of time steps in the time-series data sample.
 
-        y : array-like
+    n_features : int,
+        The number of features in the time-series data sample.
 
-        """
-        assert out_dtype in [
-            "tensor",
-            "ndarray",
-        ], f'out_dtype should be "tensor" or "ndarray", but got {out_dtype}'
-
-        is_list = isinstance(X, list)
-        is_array = isinstance(X, np.ndarray)
-        is_tensor = isinstance(X, torch.Tensor)
-        assert is_tensor or is_array or is_list, TypeError(
-            "X should be an instance of list/np.ndarray/torch.Tensor, "
-            f"but got {type(X)}"
-        )
+    pred_step : int,
+        The number of time steps to forecast.
 
-        # convert the data type if in need
-        if out_dtype == "tensor":
-            if is_list:
-                X = torch.tensor(X)
-            elif is_array:
-                X = torch.from_numpy(X)
-            else:  # is tensor
-                pass
-        else:  # out_dtype is ndarray
-            # convert to np.ndarray first for shape check
-            if is_list:
-                X = np.asarray(X)
-            elif is_tensor:
-                X = X.numpy()
-            else:  # is ndarray
-                pass
-
-        # check the shape of X here
-        X_shape = X.shape
-        assert len(X_shape) == 3, (
-            f"input should have 3 dimensions [n_samples, seq_len, n_features],"
-            f"but got shape={X_shape}"
-        )
+    rank : int,
+        The rank of the low-rank tensor.
 
-        if y is not None:
-            assert len(X) == len(y), (
-                f"lengths of X and y must match, " f"but got f{len(X)} and {len(y)}"
-            )
-            if isinstance(y, torch.Tensor):
-                y = y if out_dtype == "tensor" else y.numpy()
-            elif isinstance(y, list):
-                y = torch.tensor(y) if out_dtype == "tensor" else np.asarray(y)
-            elif isinstance(y, np.ndarray):
-                y = torch.from_numpy(y) if out_dtype == "tensor" else y
-            else:
-                raise TypeError(
-                    "y should be an instance of list/np.ndarray/torch.Tensor, "
-                    f"but got {type(y)}"
-                )
-
-        return X, y
-
-    @abstractmethod
-    def _fetch_data_from_array(self, idx: int) -> Iterable:
-        """Fetch data from self.X if it is given.
-
-        Parameters
-        ----------
-        idx : int,
-            The index of the sample to be return.
-
-        Returns
-        -------
-        sample : list,
-            The collated data sample, a list including all necessary sample info.
-        """
+    time_lags : list,
+        The time lags.
 
-        X = self.X[idx]
-        missing_mask = ~torch.isnan(X)
-        X = torch.nan_to_num(X)
-        sample = [
-            torch.tensor(idx),
-            X.to(torch.float32),
-            missing_mask.to(torch.float32),
-        ]
+    burn_iter : int,
+        The number of burn-in iterations.
 
-        if self.y is not None and self.return_labels:
-            sample.append(self.y[idx].to(torch.long))
+    gibbs_iter : int,
+        The number of Gibbs iterations.
 
-        return sample
+    multi_step : int, default = 1,
+        The number of time steps to forecast at each iteration.
 
-    def _open_file_handle(self) -> h5py.File:
-        """Open the file handle for reading data from the file.
+    device :
+        The device for the model to run on. It can be a string, a :class:`torch.device` object, or a list of them.
+        If not given, will try to use CUDA devices first (will use the default CUDA device if there are multiple),
+        then CPUs, considering CUDA and CPU are so far the main devices for people to train ML models.
+        If given a list of devices, e.g. ['cuda:0', 'cuda:1'], or [torch.device('cuda:0'), torch.device('cuda:1')] , the
+        model will be parallely trained on the multiple devices (so far only support parallel training on CUDA devices).
+        Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
 
-        Notes
-        -----
-        This function can also help confirm if the given file and file type match.
+    Notes
+    -----
+    1). ``n_steps`` must be larger than ``pred_step``;
 
-        Returns
-        -------
-        file_handle : file
+    2). ``n_steps - pred_step`` must be larger than ``max(time_lags)``;
 
-        """
-        data_file_path = self.data
-        try:
-            file_handler = h5py.File(
-                data_file_path,
-                "r",
-            )  # set swmr=True if the h5 file need to be written into new content during reading
-        except ImportError:
-            raise ImportError(
-                "h5py is missing and cannot be imported. Please install it first."
-            )
-        except OSError as e:
-            raise TypeError(
-                f"{e} This probably is caused by file type error. "
-                f"Please confirm that the given file {data_file_path} is an h5 file."
-            )
-        except Exception as e:
-            raise RuntimeError(e)
-        return file_handler
-
-    @abstractmethod
-    def _fetch_data_from_file(self, idx: int) -> Iterable:
-        """Fetch data with the lazy-loading strategy, i.e. only loading data from the file while requesting for samples.
-        Here the opened file handle doesn't load the entire dataset into RAM but only load the currently accessed slice.
-
-        Notes
-        -----
-        Multi workers reading from h5 file is tricky, and I was confronted with a problem similar to
-        https://discuss.pytorch.org/t/dataloader-when-num-worker-0-there-is-bug/25643/7 in 2020, please
-        refer to it for more details about the problem.
-        The implementation here is referred to
-        https://discuss.pytorch.org/t/dataloader-when-num-worker-0-there-is-bug/25643/10
-        And according to https://discuss.pytorch.org/t/dataloader-when-num-worker-0-there-is-bug/25643/37,
-        pytorch v1.7.1 and h5py v3.2.0 work well, so probably updating to the latest version can avoid the
-        issue I met. After all, this implementation may need to be updated in the near future.
-
-        Parameters
-        ----------
-        idx : int,
-            The index of the sample to be return.
-
-        Returns
-        -------
-        sample : list,
-            The collated data sample, a list including all necessary sample info.
-        """
+    """
 
-        if self.file_handle is None:
-            self.file_handle = self._open_file_handle()
+    def __init__(
+        self,
+        n_steps: int,
+        n_features: int,
+        pred_step: int,
+        rank: int,
+        time_lags: list,
+        burn_iter: int,
+        gibbs_iter: int,
+        multi_step: int = 1,
+        device: Optional[Union[str, torch.device, list]] = None,
+    ):
+        super().__init__(device)
+        self.n_steps = n_steps
+        self.n_features = n_features
+        self.pred_step = pred_step
+        self.multi_step = multi_step
+        self.rank = rank
+        self.time_lags = np.asarray(time_lags)
+        self.burn_iter = burn_iter
+        self.gibbs_iter = gibbs_iter
 
-        X = torch.from_numpy(self.file_handle["X"][idx])
-        missing_mask = ~torch.isnan(X)
-        X = torch.nan_to_num(X)
-        sample = [
-            torch.tensor(idx),
-            X.to(torch.float32),
-            missing_mask.to(torch.float32),
-        ]
+    def fit(
+        self,
+        train_set: Union[dict, str],
+        val_set: Optional[Union[dict, str]] = None,
+        file_type="h5py",
+    ) -> None:
+        """Train the forecaster on the given data.
+
+        Warnings
+        --------
+        BTTF does not need to run fit().
+        Please run func ``forecast()`` directly.
 
-        # if the dataset has labels and is for training, then fetch it from the file
-        if "y" in self.file_handle.keys() and self.return_labels:
-            sample.append(self.file_handle["y"][idx].to(torch.long))
-
-        return sample
-
-    def __getitem__(self, idx: int) -> Iterable:
-        """Fetch data according to index.
-
-        Parameters
-        ----------
-        idx : int,
-            The index to fetch the specified sample.
-
-        Returns
-        -------
-        sample : list,
-            The collated data sample, a list including all necessary sample info.
         """
+        warnings.warn("Please run func forecast(X) directly.")
 
-        sample = self.fetch_data(idx)
-        return sample
+    def forecast(
+        self,
+        X: Union[dict, str],
+        file_type: str = "h5py",
+    ) -> np.ndarray:
+        assert not isinstance(
+            X, str
+        ), "BTTF so far does not accept file input. It needs a specified Dataset class."
+
+        X = X["X"]
+        X = X.transpose((0, 2, 1))
+
+        pred = BTTF_forecast(
+            X,
+            X.copy(),
+            self.pred_step,
+            self.multi_step,
+            self.rank,
+            self.time_lags,
+            self.burn_iter,
+            self.gibbs_iter,
+        )
+        pred = pred.transpose((0, 2, 1))
+        return pred
```

### Comparing `pypots-0.1.0/pypots/data/generating.py` & `pypots-0.1.1/pypots/data/generating.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,52 +5,51 @@
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 import math
 from typing import Optional, Tuple
 
 import numpy as np
-from sklearn.utils import check_random_state
-
 import torch
 from sklearn.model_selection import train_test_split
 from sklearn.preprocessing import StandardScaler
+from sklearn.utils import check_random_state
 
-from pypots.data.utils import mcar, masked_fill
-from pypots.data.load_specific_datasets import load_specific_dataset
+from .load_specific_datasets import load_specific_dataset
+from .utils import mcar, masked_fill
 
 
 def gene_complete_random_walk(
     n_samples: int = 1000,
     n_steps: int = 24,
     n_features: int = 10,
     mu: float = 0.0,
     std: float = 1.0,
     random_state: Optional[int] = None,
 ) -> np.ndarray:
     """Generate complete random walk time-series data.
 
     Parameters
     ----------
-    n_samples : int, default=1000
+    n_samples :
         The number of training time-series samples to generate.
 
     n_steps: int, default=24
         The number of time steps (length) of generated time-series samples.
 
-    n_features : int, default=10
+    n_features :
         The number of features (dimensions) of generated time-series samples.
 
-    mu : float, default 0.0,
+    mu :
         Mean of the normal distribution, which random walk steps are sampled from.
 
-    std : float, default 1.,
+    std :
         Standard deviation of the normal distribution, which random walk steps are sampled from.
 
-    random_state : int or numpy.RandomState, default=None,
+    random_state :
         Random seed for data generation.
 
     Returns
     -------
     ts_samples: array, shape of [n_samples, n_steps, n_features]
         Generated random walk time series.
     """
@@ -72,42 +71,42 @@
     shuffle: bool = True,
     random_state: Optional[int] = None,
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Generate complete random walk time-series data for the classification task.
 
     Parameters
     ----------
-    n_classes : int, default=2
+    n_classes :
         Number of classes (types) of the generated data.
 
-    n_samples_each_class : int, default=500
+    n_samples_each_class :
         Number of samples for each class to generate.
 
-    n_steps : int, default=24
+    n_steps :
         Number of time steps in each sample.
 
-    n_features : int, default=10
+    n_features :
         Number of features.
 
-    shuffle : bool, default=True
+    shuffle :
         Whether to shuffle generated samples.
         If not, you can separate samples of each class according to `n_samples_each_class`.
         For example,
         X_class0=X[:n_samples_each_class],
         X_class1=X[n_samples_each_class:n_samples_each_class*2]
 
-    random_state : int or numpy.RandomState, default=None,
+    random_state :
         Random seed for data generation.
 
     Returns
     -------
-    X : array, shape of [n_classes*n_samples_each_class, n_steps, n_features]
+    X :
         Generated time-series data.
 
-    y : array, shape of [n_classes*n_samples_each_class]
+    y :
         Labels indicating classes of time-series samples.
 
     """
     ts_collector = []
     label_collector = []
 
     mu = 0
@@ -146,47 +145,47 @@
     anomaly_scale_factor: float = 2.0,
     random_state: Optional[int] = None,
 ) -> Tuple[np.ndarray, np.ndarray]:
     """Generate random walk time-series data for the anomaly-detection task.
 
     Parameters
     ----------
-    n_samples : int, default=1000
+    n_samples :
         The number of training time-series samples to generate.
 
-    n_features : int, default=10
+    n_features :
         The number of features (dimensions) of generated time-series samples.
 
     n_steps: int, default=24
         The number of time steps (length) of generated time-series samples.
 
-    mu : float, default 0.0,
+    mu :
         Mean of the normal distribution, which random walk steps are sampled from.
 
-    std : float, default 1.,
+    std :
         Standard deviation of the normal distribution, which random walk steps are sampled from.
 
-    anomaly_proportion : float, in (0,1)
+    anomaly_proportion :
         Proportion of anomaly samples in all samples.
 
-    anomaly_fraction : float, in (0,1)
+    anomaly_fraction :
         Fraction of anomaly points in each anomaly sample.
 
-    anomaly_scale_factor : int or float,
+    anomaly_scale_factor :
         Scale factor for value scaling to create anomaly points in time series samples.
 
-    random_state : int or numpy.RandomState, default=None,
+    random_state :
         Random seed for data generation.
 
     Returns
     -------
-    X : array, shape of [n_classes*n_samples_each_class, n_steps, n_features]
+    X :
         Generated time-series data.
 
-    y : array, shape of [n_classes*n_samples_each_class]
+    y :
         Labels indicating if time-series samples are anomalies.
     """
     assert (
         0 < anomaly_proportion < 1
     ), f"anomaly_proportion should be >0 and <1, but got {anomaly_proportion}"
     assert (
         0 < anomaly_fraction < 1
@@ -229,27 +228,27 @@
 def gene_incomplete_random_walk_dataset(
     n_steps=24, n_features=10, n_classes=2, n_samples_each_class=1000, missing_rate=0.1
 ) -> dict:
     """Generate a random-walk data.
 
     Parameters
     ----------
-    n_steps : int, default=24
+    n_steps :
         Number of time steps in each sample.
 
-    n_features : int, default=10
+    n_features :
         Number of features.
 
-    n_classes : int, default=2
+    n_classes :
         Number of classes (types) of the generated data.
 
-    n_samples_each_class : int, default=500
+    n_samples_each_class :
         Number of samples for each class to generate.
 
-    missing_rate : float, default=0.1,
+    missing_rate :
         The rate of randomly missing values to generate.
 
     Returns
     -------
     data: dict,
         A dictionary containing the generated data.
     """
@@ -314,23 +313,24 @@
 
 
 def gene_physionet2012(artificially_missing_rate: float = 0.1):
     """Generate a fully-prepared PhysioNet-2012 dataset for model testing.
 
     Parameters
     ----------
-    artificially_missing_rate : float, default = 0.1
+    artificially_missing_rate :
         The rate of artificially missing values to generate for model evaluation.
         This ratio is calculated based on the number of observed values, i.e. if artificially_missing_rate = 0.1,
         then 10% of the observed values will be randomly masked as missing data and hold out for model evaluation.
 
     Returns
     -------
     data: dict,
         A dictionary containing the generated PhysioNet-2012 dataset.
+
     """
     assert (
         0 <= artificially_missing_rate < 1
     ), "artificially_missing_rate must be in [0,1)"
 
     # generate samples
     dataset = load_specific_dataset("physionet_2012")
```

### Comparing `pypots-0.1.0/pypots/data/load_preprocessing.py` & `pypots-0.1.1/pypots/data/load_preprocessing.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 
 
 def preprocess_physionet2012(data: dict) -> dict:
     """The preprocessing function for dataset PhysioNet-2012.
 
     Parameters
     ----------
-    data : dict,
+    data :
         A data dict from tsdb.load_dataset().
 
     Returns
     -------
-    dataset : dict,
+    dataset :
         A dict containing processed data, including:
             X : pandas.DataFrame,
                 A dataframe contains all time series vectors from 11988 patients, distinguished by column `RecordID`.
             y : pandas.Series
                 The 11988 classification labels of all patients, indicating whether they were deceased.
     """
     # remove the static features, e.g. age, gender
```

### Comparing `pypots-0.1.0/pypots/data/load_specific_datasets.py` & `pypots-0.1.1/pypots/data/load_specific_datasets.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 
 import tsdb
 
-from pypots.data.load_preprocessing import preprocess_physionet2012
-from pypots.utils.logging import logger
+from .load_preprocessing import preprocess_physionet2012
+from ..utils.logging import logger
 
 # currently supported datasets
 SUPPORTED_DATASETS = [
     "physionet_2012",
 ]
 
 # preprocessing functions of the supported datasets
@@ -23,38 +23,38 @@
 
 
 def list_supported_datasets() -> list:
     """Return the datasets natively supported by PyPOTS so far.
 
     Returns
     -------
-    SUPPORTED_DATASETS : list,
+    SUPPORTED_DATASETS :
         A list including all supported datasets.
 
     """
     return SUPPORTED_DATASETS
 
 
 def load_specific_dataset(dataset_name: str, use_cache: bool = True) -> dict:
     """Load specific datasets supported by PyPOTS.
     Different from tsdb.load_dataset(), which only produces merely raw data,
     load_specific_dataset here does some preprocessing operations,
     like truncating time series to generate samples with the same length.
 
     Parameters
     ----------
-    dataset_name : str,
+    dataset_name :
         The name of the dataset to be loaded, which should be supported, i.e. in SUPPORTED_DATASETS.
 
     use_cache :
         Whether to use cache. This is an argument of tsdb.load_dataset().
 
     Returns
     -------
-    data : dict,
+    data :
         A dict contains the preprocessed dataset.
         Users only need to continue the preprocessing steps to generate the data they want,
         e.g. standardizing and splitting.
 
     """
     logger.info(
         f"Loading the dataset {dataset_name} with TSDB (https://github.com/WenjieDu/Time_Series_Database)..."
```

### Comparing `pypots-0.1.0/pypots/data/utils.py` & `pypots-0.1.1/pypots/data/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,20 +21,20 @@
 
 
 def cal_missing_rate(X: Union[np.ndarray, torch.Tensor, list]) -> float:
     """Calculate the missing rate of the given data.
 
     Parameters
     ----------
-    X : np.ndarray, torch.Tensor, list,
+    X :
         The data to calculate missing rate.
 
     Returns
     -------
-    missing_rate : float,
+    missing_rate :
         The missing rate of the given data.
 
     """
     missing_rate = corruptor.cal_missing_rate(X)
     return missing_rate
 
 
@@ -43,26 +43,26 @@
     mask: Union[np.ndarray, torch.Tensor, list],
     value: float,
 ) -> Union[np.ndarray, torch.Tensor]:
     """Fill the masked values in ``X`` according to ``mask`` with the given ``value``.
 
     Parameters
     ----------
-    X : np.ndarray, torch.Tensor, list,
+    X :
         The data to be filled.
 
-    mask : np.ndarray, torch.Tensor, list,
+    mask :
         The mask for filling the given data.
 
-    value : float,
+    value :
         The value to fill the masked values.
 
     Returns
     -------
-    filled_X : np.ndarray, torch.Tensor, list,
+    filled_X :
         The filled data.
 
     """
     filled_X = corruptor.masked_fill(X, mask, value)
     return filled_X
 
 
@@ -71,45 +71,45 @@
     rate: float,
     nan: float = 0,
 ) -> Union[np.ndarray, torch.Tensor]:
     """Generate missing values in the given data with MCAR (Missing Completely At Random) mechanism.
 
     Parameters
     ----------
-    X : np.ndarray, torch.Tensor, list,
+    X :
         The data to add missing values.
 
-    rate : float,
+    rate :
         The missing rate.
 
-    nan : float, default = 0,
+    nan :
         The value to fill the missing values.
 
     Returns
     -------
-    X : np.ndarray, torch.Tensor,
+    X :
         The data with added missing values.
 
     """
     X = corruptor.mcar(X, rate, nan)
     return X
 
 
 def torch_parse_delta(missing_mask: torch.Tensor) -> torch.Tensor:
     """Generate time-gap (delta) matrix from missing masks.
     Please refer to :cite:`che2018GRUD` for its math definition.
 
     Parameters
     ----------
-    missing_mask : torch.tensor, shape of [n_steps, n_features] or [n_samples, n_steps, n_features]
-        Binary masks indicate missing values.
+    missing_mask :
+        Binary masks indicate missing values. Shape of [n_steps, n_features] or [n_samples, n_steps, n_features]
 
     Returns
     -------
-    delta, torch.tensor,
+    delta
         Delta matrix indicates time gaps of missing values.
     """
 
     def cal_delta_for_single_sample(mask: torch.Tensor) -> torch.Tensor:
         """calculate single sample's delta. The sample's shape is [n_steps, n_features]."""
         d = []
         for step in range(n_steps):
@@ -138,20 +138,20 @@
 
 
 def numpy_parse_delta(missing_mask: np.ndarray) -> np.ndarray:
     """Generate time-gap (delta) matrix from missing masks. Please refer to :cite:`che2018GRUD` for its math definition.
 
     Parameters
     ----------
-    missing_mask : np.ndarray, shape of [n_steps, n_features] or [n_samples, n_steps, n_features]
-        Binary masks indicate missing values.
+    missing_mask :
+        Binary masks indicate missing values. Shape of [n_steps, n_features] or [n_samples, n_steps, n_features].
 
     Returns
     -------
-    delta, np.ndarray,
+    delta
         Delta matrix indicates time gaps of missing values.
     """
 
     def cal_delta_for_single_sample(mask: np.ndarray) -> np.ndarray:
         """calculate single sample's delta. The sample's shape is [n_steps, n_features]."""
         d = []
         for step in range(seq_len):
```

### Comparing `pypots-0.1.0/pypots/forecasting/bttf/modules.py` & `pypots-0.1.1/pypots/forecasting/bttf/modules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.1.0/pypots/imputation/base.py` & `pypots-0.1.1/pypots/imputation/mrnn/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,319 +1,312 @@
 """
-The base class for PyPOTS imputation models.
+PyTorch MRNN model for the time-series imputation task.
+Some part of the code is from https://github.com/WenjieDu/SAITS.
+
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
-# License: GPL-v3
+# License: GLP-v3
 
 
-import os
-from abc import abstractmethod
 from typing import Union, Optional
 
+import h5py
 import numpy as np
 import torch
+import torch.nn as nn
 from torch.utils.data import DataLoader
 
-from pypots.base import BaseModel, BaseNNModel
-from pypots.utils.logging import logger
-from pypots.utils.metrics import cal_mae
-
-try:
-    import nni
-except ImportError:
-    pass
+from .data import DatasetForMRNN
+from .module import FCN_Regression
+from ..base import BaseNNImputer
+from ...optim.adam import Adam
+from ...optim.base import Optimizer
+from ...utils.metrics import cal_rmse
+
+
+class _MRNN(nn.Module):
+    def __init__(self, seq_len, feature_num, rnn_hidden_size, device):
+        super().__init__()
+        # data settings
+        self.seq_len = seq_len
+        self.feature_num = feature_num
+        self.rnn_hidden_size = rnn_hidden_size
+        self.device = device
+
+        self.f_rnn = nn.GRUCell(self.feature_num * 3, self.rnn_hidden_size)
+        self.b_rnn = nn.GRUCell(self.feature_num * 3, self.rnn_hidden_size)
+        self.concated_hidden_project = nn.Linear(
+            self.rnn_hidden_size * 2, self.feature_num
+        )
+        self.fcn_regression = FCN_Regression(feature_num, rnn_hidden_size)
+
+    def gene_hidden_states(self, inputs, direction):
+        X = inputs[direction]["X"]
+        masks = inputs[direction]["missing_mask"]
+        deltas = inputs[direction]["deltas"]
+        device = X.device
+
+        hidden_states_collector = []
+        hidden_state = torch.zeros((X.size()[0], self.rnn_hidden_size), device=device)
+
+        for t in range(self.seq_len):
+            x = X[:, t, :]
+            m = masks[:, t, :]
+            d = deltas[:, t, :]
+            inputs = torch.cat([x, m, d], dim=1)
+            if direction == "forward":
+                hidden_state = self.f_rnn(inputs, hidden_state)
+            else:
+                hidden_state = self.b_rnn(inputs, hidden_state)
+            hidden_states_collector.append(hidden_state)
+        return hidden_states_collector
+
+    def forward(self, inputs, training=True):
+        hidden_states_f = self.gene_hidden_states(inputs, "forward")
+        hidden_states_b = self.gene_hidden_states(inputs, "backward")[::-1]
+
+        X = inputs["forward"]["X"]
+        masks = inputs["forward"]["missing_mask"]
+
+        reconstruction_loss = 0
+        estimations = []
+        for i in range(
+            self.seq_len
+        ):  # calculating estimation loss for times can obtain better results than once
+            x = X[:, i, :]
+            m = masks[:, i, :]
+            h_f = hidden_states_f[i]
+            h_b = hidden_states_b[i]
+            h = torch.cat([h_f, h_b], dim=1)
+            RNN_estimation = self.concated_hidden_project(h)  # x̃_t
+            RNN_imputed_data = m * x + (1 - m) * RNN_estimation
+            FCN_estimation = self.fcn_regression(
+                x, m, RNN_imputed_data
+            )  # FCN estimation is output estimation
+            reconstruction_loss += cal_rmse(FCN_estimation, x, m) + cal_rmse(
+                RNN_estimation, x, m
+            )
+            estimations.append(FCN_estimation.unsqueeze(dim=1))
+
+        estimations = torch.cat(estimations, dim=1)
+        imputed_data = masks * X + (1 - masks) * estimations
+
+        if not training:
+            # if not in training mode, return the classification result only
+            return {
+                "imputed_data": imputed_data,
+            }
+
+        reconstruction_loss /= self.seq_len
+
+        ret_dict = {
+            "loss": reconstruction_loss,
+            "imputed_data": imputed_data,
+        }
+        return ret_dict
 
 
-class BaseImputer(BaseModel):
-    """Abstract class for all imputation models.
+class MRNN(BaseNNImputer):
+    """The PyTorch implementation of the MRNN model :cite:`yoon2019MRNN`.
 
     Parameters
     ----------
-    device : str or `torch.device`, default = None,
-        The device for the model to run on.
-        If not given, will try to use CUDA devices first, then CPUs. CUDA and CPU are so far the main devices for people
-        to train ML models. Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
-
-    saving_path : str, default = None,
-        The path to save model checkpoints and tensorboard files,
-        which contains the loss values recorded during training.
-    """
-
-    def __init__(
-        self,
-        device: Optional[Union[str, torch.device]] = None,
-        saving_path: str = None,
-        model_saving_strategy: Optional[str] = "best",
-    ):
-        super().__init__(
-            device,
-            saving_path,
-            model_saving_strategy,
-        )
-
-    @abstractmethod
-    def fit(
-        self,
-        train_set: Union[dict, str],
-        val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
-    ) -> None:
-        """Train the imputer on the given data.
-
-        Parameters
-        ----------
-        train_set : dict or str,
-            The dataset for model training, should be a dictionary including the key 'X',
-            or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-            which is time-series data for training, can contain missing values.
-            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-            key-value pairs like a dict, and it has to include the key 'X'.
-
-        val_set : dict or str,
-            The dataset for model validating, should be a dictionary including the key 'X',
-            or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-            which is time-series data for validating, can contain missing values.
-            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-            key-value pairs like a dict, and it has to include the key 'X'.
-
-        file_type : str, default = "h5py",
-            The type of the given file if train_set and val_set are path strings.
+    rnn_hidden_size :
+        The size of the RNN hidden state, also the number of hidden units in the RNN cell.
 
-        """
-        pass
+    batch_size :
+        The batch size for training and evaluating the model.
 
-    @abstractmethod
-    def impute(
-        self,
-        X: Union[dict, str],
-        file_type: str = "h5py",
-    ) -> np.ndarray:
-        """Impute missing values in the given data with the trained model.
+    epochs :
+        The number of epochs for training the model.
 
-        Parameters
-        ----------
-        X : array-like or str,
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
-            n_features], or a path string locating a data file, e.g. h5 file.
-
-        file_type : str, default = "h5py",
-            The type of the given file if X is a path string.
-
-        Returns
-        -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
-            Imputed data.
-        """
-        pass
+    patience :
+        The patience for the early-stopping mechanism. Given a positive integer, the training process will be
+        stopped when the model does not perform better after that number of epochs.
+        Leaving it default as None will disable the early-stopping.
+
+    optimizer :
+        The optimizer for model training.
+        If not given, will use a default Adam optimizer.
+
+    num_workers :
+        The number of subprocesses to use for data loading.
+        `0` means data loading will be in the main process, i.e. there won't be subprocesses.
+
+    device :
+        The device for the model to run on. It can be a string, a :class:`torch.device` object, or a list of them.
+        If not given, will try to use CUDA devices first (will use the default CUDA device if there are multiple),
+        then CPUs, considering CUDA and CPU are so far the main devices for people to train ML models.
+        If given a list of devices, e.g. ['cuda:0', 'cuda:1'], or [torch.device('cuda:0'), torch.device('cuda:1')] , the
+        model will be parallely trained on the multiple devices (so far only support parallel training on CUDA devices).
+        Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
 
+    saving_path :
+        The path for automatically saving model checkpoints and tensorboard files (i.e. loss values recorded during
+        training into a tensorboard file). Will not save if not given.
 
-class BaseNNImputer(BaseNNModel, BaseImputer):
-    """Abstract class for all neural-network imputation models.
+    model_saving_strategy :
+        The strategy to save model checkpoints. It has to be one of [None, "best", "better"].
+        No model will be saved when it is set as None.
+        The "best" strategy will only automatically save the best model after the training finished.
+        The "better" strategy will automatically save the model during training whenever the model performs
+        better than in previous epochs.
 
-    Parameters
+    Attributes
     ----------
-    batch_size : int,
-        Size of the batch input into the model for one step.
-
-    epochs : int,
-        Training epochs, i.e. the maximum rounds of the model to be trained with.
-
-    patience : int,
-        Number of epochs the training procedure will keep if loss doesn't decrease.
-        Once exceeding the number, the training will stop.
-
-    device : str or `torch.device`, default = None,
-        The device for the model to run on.
-        If not given, will try to use CUDA devices first, then CPUs. CUDA and CPU are so far the main devices for people
-        to train ML models. Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
+    model : :class:`torch.nn.Module`
+        The underlying BRITS model.
 
-    saving_path : str, default = None,
-        The path for automatically saving model checkpoints and tensorboard files (i.e. loss values recorded during
-        training into a tensorboard file). Will not save if not given.
+    optimizer : :class:`pypots.optim.Optimizer`
+        The optimizer for model training.
 
     """
 
     def __init__(
         self,
-        batch_size: int,
-        epochs: int,
-        patience: int,
+        n_steps: int,
+        n_features: int,
+        rnn_hidden_size: int,
+        batch_size: int = 32,
+        epochs: int = 100,
+        patience: int = None,
+        optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
-        device: Optional[Union[str, torch.device]] = None,
+        device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
         model_saving_strategy: Optional[str] = "best",
     ):
         super().__init__(
             batch_size,
             epochs,
             patience,
             num_workers,
             device,
             saving_path,
             model_saving_strategy,
         )
 
-    @abstractmethod
+        self.n_steps = n_steps
+        self.n_features = n_features
+        self.rnn_hidden_size = rnn_hidden_size
+
+        # set up the model
+        self.model = _MRNN(
+            self.n_steps,
+            self.n_features,
+            self.rnn_hidden_size,
+            self.device,
+        )
+        self._send_model_to_given_device()
+        self._print_model_size()
+
+        # set up the optimizer
+        self.optimizer = optimizer
+        self.optimizer.init_optimizer(self.model.parameters())
+
     def _assemble_input_for_training(self, data: list) -> dict:
-        """Assemble the given data into a dictionary for training input.
+        # fetch data
+        (
+            indices,
+            X,
+            missing_mask,
+            deltas,
+            back_X,
+            back_missing_mask,
+            back_deltas,
+        ) = self._send_data_to_given_device(data)
+
+        # assemble input data
+        inputs = {
+            "indices": indices,
+            "forward": {
+                "X": X,
+                "missing_mask": missing_mask,
+                "deltas": deltas,
+            },
+            "backward": {
+                "X": back_X,
+                "missing_mask": back_missing_mask,
+                "deltas": back_deltas,
+            },
+        }
 
-        Parameters
-        ----------
-        data : list,
-            Input data from dataloader, should be list.
-
-        Returns
-        -------
-        dict,
-            A python dictionary contains the input data for model training.
-        """
-        pass
+        return inputs
 
-    @abstractmethod
     def _assemble_input_for_validating(self, data: list) -> dict:
-        """Assemble the given data into a dictionary for validating input.
-
-        Parameters
-        ----------
-        data : list,
-            Data output from dataloader, should be list.
-
-        Returns
-        -------
-        dict,
-            A python dictionary contains the input data for model validating.
-        """
-        pass
+        return self._assemble_input_for_training(data)
 
-    @abstractmethod
     def _assemble_input_for_testing(self, data: list) -> dict:
-        """Assemble the given data into a dictionary for testing input.
-
-        Notes
-        -----
-        The processing functions of train/val/test stages are separated for the situation that the input of
-        the three stages are different, and this situation usually happens when the Dataset/Dataloader classes
-        used in the train/val/test stages are not the same, e.g. the training data and validating data in a
-        classification task contains labels, but the testing data (from the production environment) generally
-        doesn't have labels.
-
-        Parameters
-        ----------
-        data : list,
-            Data output from dataloader, should be list.
-
-        Returns
-        -------
-        dict,
-            A python dictionary contains the input data for model testing.
-        """
-        pass
+        return self._assemble_input_for_validating(data)
 
-    def _train_model(
+    def fit(
         self,
-        training_loader: DataLoader,
-        val_loader: DataLoader = None,
+        train_set: Union[dict, str],
+        val_set: Optional[Union[dict, str]] = None,
+        file_type: str = "h5py",
     ) -> None:
-        # each training starts from the very beginning, so reset the loss and model dict here
-        self.best_loss = float("inf")
-        self.best_model_dict = None
-
-        try:
-            training_step = 0
-            for epoch in range(self.epochs):
-                self.model.train()
-                epoch_train_loss_collector = []
-                for idx, data in enumerate(training_loader):
-                    training_step += 1
-                    inputs = self._assemble_input_for_training(data)
-                    self.optimizer.zero_grad()
-                    results = self.model.forward(inputs)
-                    results["loss"].backward()
-                    self.optimizer.step()
-                    epoch_train_loss_collector.append(results["loss"].item())
-
-                    # save training loss logs into the tensorboard file for every step if in need
-                    if self.summary_writer is not None:
-                        self._save_log_into_tb_file(training_step, "training", results)
-
-                # mean training loss of the current epoch
-                mean_train_loss = np.mean(epoch_train_loss_collector)
-
-                if val_loader is not None:
-                    self.model.eval()
-                    imputation_collector = []
-                    with torch.no_grad():
-                        for idx, data in enumerate(val_loader):
-                            inputs = self._assemble_input_for_validating(data)
-                            imputed_data = self.model.impute(inputs)
-                            imputation_collector.append(imputed_data)
-
-                    imputation_collector = torch.cat(imputation_collector)
-                    imputation_collector = imputation_collector.cpu().detach().numpy()
-
-                    mean_val_loss = cal_mae(
-                        imputation_collector,
-                        val_loader.dataset.data["X_intact"],
-                        val_loader.dataset.data["indicating_mask"],
-                        # the above val_loader.dataset.data is a dict containing the validation dataset
-                    )
-
-                    # save validating loss logs into the tensorboard file for every epoch if in need
-                    if self.summary_writer is not None:
-                        val_loss_dict = {
-                            "imputation_loss": mean_val_loss,
-                        }
-                        self._save_log_into_tb_file(epoch, "validating", val_loss_dict)
-
-                    logger.info(
-                        f"epoch {epoch}: "
-                        f"training loss {mean_train_loss:.4f}, "
-                        f"validating loss {mean_val_loss:.4f}"
-                    )
-                    mean_loss = mean_val_loss
-                else:
-                    logger.info(f"epoch {epoch}: training loss {mean_train_loss:.4f}")
-                    mean_loss = mean_train_loss
-
-                if mean_loss < self.best_loss:
-                    self.best_loss = mean_loss
-                    self.best_model_dict = self.model.state_dict()
-                    self.patience = self.original_patience
-                    # save the model if necessary
-                    self._auto_save_model_if_necessary(
-                        training_finished=False,
-                        saving_name=f"{self.__class__.__name__}_epoch{epoch}_loss{mean_loss}",
-                    )
-                else:
-                    self.patience -= 1
-
-                if os.getenv("enable_nni", False):
-                    nni.report_intermediate_result(mean_loss)
-                    if epoch == self.epochs - 1 or self.patience == 0:
-                        nni.report_final_result(self.best_loss)
-
-                if self.patience == 0:
-                    logger.info(
-                        "Exceeded the training patience. Terminating the training procedure..."
-                    )
-                    break
-
-        except Exception as e:
-            logger.info(f"Exception: {e}")
-            if self.best_model_dict is None:
-                raise RuntimeError(
-                    "Training got interrupted. Model was not get trained. Please try fit() again."
-                )
-            else:
-                RuntimeWarning(
-                    "Training got interrupted. "
-                    "Model will load the best parameters so far for testing. "
-                    "If you don't want it, please try fit() again."
-                )
+        # Step 1: wrap the input data with classes Dataset and DataLoader
+        training_set = DatasetForMRNN(
+            train_set, return_labels=False, file_type=file_type
+        )
+        training_loader = DataLoader(
+            training_set,
+            batch_size=self.batch_size,
+            shuffle=True,
+            num_workers=self.num_workers,
+        )
+        val_loader = None
+        if val_set is not None:
+            if isinstance(val_set, str):
+                with h5py.File(val_set, "r") as hf:
+                    # Here we read the whole validation set from the file to mask a portion for validation.
+                    # In PyPOTS, using a file usually because the data is too big. However, the validation set is
+                    # generally shouldn't be too large. For example, we have 1 billion samples for model training.
+                    # We won't take 20% of them as the validation set because we want as much as possible data for the
+                    # training stage to enhance the model's generalization ability. Therefore, 100,000 representative
+                    # samples will be enough to validate the model.
+                    val_set = {
+                        "X": hf["X"][:],
+                        "X_intact": hf["X_intact"][:],
+                        "indicating_mask": hf["indicating_mask"][:],
+                    }
+            val_set = DatasetForMRNN(val_set, return_labels=False, file_type=file_type)
+            val_loader = DataLoader(
+                val_set,
+                batch_size=self.batch_size,
+                shuffle=False,
+                num_workers=self.num_workers,
+            )
+
+        # Step 2: train the model and freeze it
+        self._train_model(training_loader, val_loader)
+        self.model.load_state_dict(self.best_model_dict)
+        self.model.eval()  # set the model as eval status to freeze it.
+
+        # Step 3: save the model if necessary
+        self._auto_save_model_if_necessary(training_finished=True)
+
+    def impute(
+        self,
+        X: Union[dict, str],
+        file_type="h5py",
+    ) -> np.ndarray:
+        self.model.eval()  # set the model as eval status to freeze it.
+        test_set = DatasetForMRNN(X, return_labels=False, file_type=file_type)
+        test_loader = DataLoader(
+            test_set,
+            batch_size=self.batch_size,
+            shuffle=False,
+            num_workers=self.num_workers,
+        )
+        imputation_collector = []
 
-        if np.equal(self.best_loss.item(), float("inf")):
-            raise ValueError("Something is wrong. best_loss is Nan after training.")
+        with torch.no_grad():
+            for idx, data in enumerate(test_loader):
+                inputs = self._assemble_input_for_testing(data)
+                results = self.model.forward(inputs, training=False)
+                imputed_data = results["imputed_data"]
+                imputation_collector.append(imputed_data)
 
-        logger.info("Finished training.")
+        imputation_collector = torch.cat(imputation_collector)
+        return imputation_collector.cpu().detach().numpy()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pypots-0.1.0/pypots/imputation/brits/data.py` & `pypots-0.1.1/pypots/imputation/brits/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 from typing import Union, Iterable
 
 import torch
 
-from pypots.data.base import BaseDataset
-from pypots.data.utils import torch_parse_delta
+from ...data.base import BaseDataset
+from ...data.utils import torch_parse_delta
 
 
 class DatasetForBRITS(BaseDataset):
     """Dataset class for BRITS.
 
     Parameters
     ----------
```

### Comparing `pypots-0.1.0/pypots/imputation/brits/model.py` & `pypots-0.1.1/pypots/imputation/brits/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,69 +18,69 @@
 
 import h5py
 import numpy as np
 import torch
 import torch.nn as nn
 from torch.utils.data import DataLoader
 
-from pypots.imputation.base import BaseNNImputer
-from pypots.imputation.brits.data import DatasetForBRITS
-from pypots.imputation.brits.modules import TemporalDecay, FeatureRegression
-from pypots.optim.adam import Adam
-from pypots.optim.base import Optimizer
-from pypots.utils.metrics import cal_mae
+from .data import DatasetForBRITS
+from .modules import TemporalDecay, FeatureRegression
+from ..base import BaseNNImputer
+from ...optim.adam import Adam
+from ...optim.base import Optimizer
+from ...utils.metrics import cal_mae
 
 
 class RITS(nn.Module):
     """model RITS: Recurrent Imputation for Time Series
 
     Attributes
     ----------
-    n_steps : int,
+    n_steps :
         sequence length (number of time steps)
 
-    n_features : int,
+    n_features :
         number of features (input dimensions)
 
-    rnn_hidden_size : int,
+    rnn_hidden_size :
         the hidden size of the RNN cell
 
-    device : str, default=None,
+    device :
         specify running the model on which device, CPU/GPU
 
-    rnn_cell : torch.nn.module object
+    rnn_cell :
         the LSTM cell to model temporal data
 
-    temp_decay_h : torch.nn.module object
+    temp_decay_h :
         the temporal decay module to decay RNN hidden state
 
-    temp_decay_x : torch.nn.module object
+    temp_decay_x :
         the temporal decay module to decay data in the raw feature space
 
-    hist_reg : torch.nn.module object
+    hist_reg :
         the temporal-regression module to project RNN hidden state into the raw feature space
 
-    feat_reg : torch.nn.module object
+    feat_reg :
         the feature-regression module
 
-    combining_weight : torch.nn.module object
+    combining_weight :
         the module used to generate the weight to combine history regression and feature regression
 
     Parameters
     ----------
-    n_steps : int,
+    n_steps :
         sequence length (number of time steps)
 
-    n_features : int,
+    n_features :
         number of features (input dimensions)
 
-    rnn_hidden_size : int,
+    rnn_hidden_size :
         the hidden size of the RNN cell
 
-    device : str,
+    device :
         specify running the model on which device, CPU/GPU
 
     """
 
     def __init__(
         self,
         n_steps: int,
@@ -107,46 +107,46 @@
 
     def impute(
         self, inputs: dict, direction: str
     ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
         """The imputation function.
         Parameters
         ----------
-        inputs : dict,
+        inputs :
             Input data, a dictionary includes feature values, missing masks, and time-gap values.
 
-        direction : str, 'forward'/'backward'
+        direction :
             A keyword to extract data from parameter `data`.
 
         Returns
         -------
-        imputed_data : tensor,
+        imputed_data :
             [batch size, sequence length, feature number]
 
         hidden_states: tensor,
             [batch size, RNN hidden size]
 
-        reconstruction_loss : float tensor,
+        reconstruction_loss :
             reconstruction loss
 
         """
         values = inputs[direction]["X"]  # feature values
         masks = inputs[direction]["missing_mask"]  # missing masks
         deltas = inputs[direction]["deltas"]  # time-gap values
 
         # create hidden states and cell states for the lstm cell
         hidden_states = torch.zeros(
-            (values.size()[0], self.rnn_hidden_size), device=self.device
+            (values.size()[0], self.rnn_hidden_size), device=values.device
         )
         cell_states = torch.zeros(
-            (values.size()[0], self.rnn_hidden_size), device=self.device
+            (values.size()[0], self.rnn_hidden_size), device=values.device
         )
 
         estimations = []
-        reconstruction_loss = torch.tensor(0.0).to(self.device)
+        reconstruction_loss = torch.tensor(0.0).to(values.device)
 
         # imputation period
         for t in range(self.n_steps):
             # data shape: [batch, time, features]
             x = values[:, t, :]  # values
             m = masks[:, t, :]  # mask
             d = deltas[:, t, :]  # delta, time gap
@@ -180,54 +180,54 @@
         imputed_data = masks * values + (1 - masks) * estimations
         return imputed_data, hidden_states, reconstruction_loss
 
     def forward(self, inputs: dict, direction: str = "forward") -> dict:
         """Forward processing of the NN module.
         Parameters
         ----------
-        inputs : dict,
+        inputs :
             The input data.
 
-        direction : string, 'forward'/'backward'
+        direction :
             A keyword to extract data from parameter `data`.
 
         Returns
         -------
         dict,
             A dictionary includes all results.
 
         """
         imputed_data, hidden_state, reconstruction_loss = self.impute(inputs, direction)
         # for each iteration, reconstruction_loss increases its value for 3 times
         reconstruction_loss /= self.n_steps * 3
 
         ret_dict = {
             "consistency_loss": torch.tensor(
-                0.0, device=self.device
+                0.0, device=imputed_data.device
             ),  # single direction, has no consistency loss
             "reconstruction_loss": reconstruction_loss,
             "imputed_data": imputed_data,
             "final_hidden_state": hidden_state,
         }
         return ret_dict
 
 
 class _BRITS(nn.Module):
     """model BRITS: Bidirectional RITS
     BRITS consists of two RITS, which take time-series data from two directions (forward/backward) respectively.
 
     Attributes
     ----------
-    n_steps : int,
+    n_steps :
         sequence length (number of time steps)
 
-    n_features : int,
+    n_features :
         number of features (input dimensions)
 
-    rnn_hidden_size : int,
+    rnn_hidden_size :
         the hidden size of the RNN cell
 
     rits_f: RITS object
         the forward RITS model
 
     rits_b: RITS object
         the backward RITS model
@@ -255,18 +255,18 @@
     def _get_consistency_loss(
         pred_f: torch.Tensor, pred_b: torch.Tensor
     ) -> torch.Tensor:
         """Calculate the consistency loss between the imputation from two RITS models.
 
         Parameters
         ----------
-        pred_f : tensor,
+        pred_f :
             The imputation from the forward RITS.
 
-        pred_b : tensor,
+        pred_b :
             The imputation from the backward RITS (already gets reverted).
 
         Returns
         -------
         float tensor,
             The consistency loss.
 
@@ -276,15 +276,15 @@
 
     @staticmethod
     def _reverse(ret: dict) -> dict:
         """Reverse the array values on the time dimension in the given dictionary.
 
         Parameters
         ----------
-        ret : dict
+        ret :
 
         Returns
         -------
         dict,
             A dictionary contains values reversed on the time dimension from the given dict.
 
         """
@@ -299,56 +299,42 @@
             return tensor_.index_select(1, indices)
 
         for key in ret:
             ret[key] = reverse_tensor(ret[key])
 
         return ret
 
-    def impute(self, inputs: dict) -> torch.Tensor:
-        """Impute the missing data. Only impute, this is for test stage.
-
-        Parameters
-        ----------
-        inputs : dict,
-            A dictionary includes all input data.
-
-        Returns
-        -------
-        array-like, the same shape with the input feature vectors.
-            The feature vectors with missing part imputed.
-
-        """
-        imputed_data_f, _, _ = self.rits_f.impute(inputs, "forward")
-        imputed_data_b, _, _ = self.rits_b.impute(inputs, "backward")
-        imputed_data_b = {"imputed_data_b": imputed_data_b}
-        imputed_data_b = self._reverse(imputed_data_b)["imputed_data_b"]
-        imputed_data = (imputed_data_f + imputed_data_b) / 2
-        return imputed_data
-
-    def forward(self, inputs: dict) -> dict:
+    def forward(self, inputs: dict, training: bool = True) -> dict:
         """Forward processing of BRITS.
 
         Parameters
         ----------
-        inputs : dict,
+        inputs :
             The input data.
 
         Returns
         -------
         dict, A dictionary includes all results.
         """
         # Results from the forward RITS.
         ret_f = self.rits_f(inputs, "forward")
         # Results from the backward RITS.
         ret_b = self._reverse(self.rits_b(inputs, "backward"))
 
+        imputed_data = (ret_f["imputed_data"] + ret_b["imputed_data"]) / 2
+
+        if not training:
+            # if not in training mode, return the classification result only
+            return {
+                "imputed_data": imputed_data,
+            }
+
         consistency_loss = self._get_consistency_loss(
             ret_f["imputed_data"], ret_b["imputed_data"]
         )
-        imputed_data = (ret_f["imputed_data"] + ret_b["imputed_data"]) / 2
 
         # `loss` is always the item for backward propagating to update the model
         loss = (
             consistency_loss
             + ret_f["reconstruction_loss"]
             + ret_b["reconstruction_loss"]
         )
@@ -363,74 +349,76 @@
 
 
 class BRITS(BaseNNImputer):
     """The PyTorch implementation of the BRITS model :cite:`cao2018BRITS`.
 
     Parameters
     ----------
-    rnn_hidden_size : int,
+    rnn_hidden_size :
         The size of the RNN hidden state, also the number of hidden units in the RNN cell.
 
-    batch_size : int, default = 32,
+    batch_size :
         The batch size for training and evaluating the model.
 
-    epochs : int, default = 100,
+    epochs :
         The number of epochs for training the model.
 
-    patience : int, default = None,
+    patience :
         The patience for the early-stopping mechanism. Given a positive integer, the training process will be
         stopped when the model does not perform better after that number of epochs.
         Leaving it default as None will disable the early-stopping.
 
-    optimizer : ``pypots.optim.base.Optimizer``, default = ``pypots.optim.Adam()``,
+    optimizer :
         The optimizer for model training.
         If not given, will use a default Adam optimizer.
 
-    num_workers : int, default = 0,
+    num_workers :
         The number of subprocesses to use for data loading.
         `0` means data loading will be in the main process, i.e. there won't be subprocesses.
 
-    device : str or `torch.device`, default = None,
-        The device for the model to run on.
-        If not given, will try to use CUDA devices first (will use the GPU with device number 0 only by default),
+    device :
+        The device for the model to run on. It can be a string, a :class:`torch.device` object, or a list of them.
+        If not given, will try to use CUDA devices first (will use the default CUDA device if there are multiple),
         then CPUs, considering CUDA and CPU are so far the main devices for people to train ML models.
+        If given a list of devices, e.g. ['cuda:0', 'cuda:1'], or [torch.device('cuda:0'), torch.device('cuda:1')] , the
+        model will be parallely trained on the multiple devices (so far only support parallel training on CUDA devices).
         Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
 
-    saving_path : str, default = None,
+    saving_path :
         The path for automatically saving model checkpoints and tensorboard files (i.e. loss values recorded during
         training into a tensorboard file). Will not save if not given.
 
-    model_saving_strategy : str or None, None or "best" or "better" , default = "best",
+    model_saving_strategy :
         The strategy to save model checkpoints. It has to be one of [None, "best", "better"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
 
     Attributes
     ----------
-    model : object,
+    model : :class:`torch.nn.Module`
         The underlying BRITS model.
 
-    optimizer : object,
+    optimizer : :class:`pypots.optim.Optimizer`
         The optimizer for model training.
 
     """
 
     def __init__(
         self,
         n_steps: int,
         n_features: int,
         rnn_hidden_size: int,
         batch_size: int = 32,
         epochs: int = 100,
         patience: int = None,
         optimizer: Optional[Optimizer] = Adam(),
         num_workers: int = 0,
-        device: Optional[Union[str, torch.device]] = None,
+        device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
         model_saving_strategy: Optional[str] = "best",
     ):
         super().__init__(
             batch_size,
             epochs,
             patience,
@@ -442,41 +430,37 @@
 
         self.n_steps = n_steps
         self.n_features = n_features
         self.rnn_hidden_size = rnn_hidden_size
 
         # set up the model
         self.model = _BRITS(
-            self.n_steps, self.n_features, self.rnn_hidden_size, self.device
+            self.n_steps,
+            self.n_features,
+            self.rnn_hidden_size,
+            self.device,
         )
-        self.model = self.model.to(self.device)
+        self._send_model_to_given_device()
         self._print_model_size()
 
         # set up the optimizer
         self.optimizer = optimizer
         self.optimizer.init_optimizer(self.model.parameters())
 
     def _assemble_input_for_training(self, data: list) -> dict:
-        """Assemble the given data into a dictionary for training input.
-
-        Parameters
-        ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
-
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model training.
-        """
-
         # fetch data
-        indices, X, missing_mask, deltas, back_X, back_missing_mask, back_deltas = map(
-            lambda x: x.to(self.device), data
-        )
+        (
+            indices,
+            X,
+            missing_mask,
+            deltas,
+            back_X,
+            back_missing_mask,
+            back_deltas,
+        ) = self._send_data_to_given_device(data)
 
         # assemble input data
         inputs = {
             "indices": indices,
             "forward": {
                 "X": X,
                 "missing_mask": missing_mask,
@@ -488,83 +472,29 @@
                 "deltas": back_deltas,
             },
         }
 
         return inputs
 
     def _assemble_input_for_validating(self, data: list) -> dict:
-        """Assemble the given data into a dictionary for validating input.
-
-        Notes
-        -----
-        The validating data assembling processing is the same as training data assembling.
-
-        Parameters
-        ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
-
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model validating.
-        """
         return self._assemble_input_for_training(data)
 
     def _assemble_input_for_testing(self, data: list) -> dict:
-        """Assemble the given data into a dictionary for testing input.
-
-        Notes
-        -----
-        The testing data assembling processing is the same as training data assembling.
-
-        Parameters
-        ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
-
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model testing.
-        """
         return self._assemble_input_for_validating(data)
 
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type: str = "h5py",
     ) -> None:
-        """Train the imputer on the given data.
-
-        Parameters
-        ----------
-        train_set : dict or str,
-            The dataset for model training, should be a dictionary including the key 'X',
-            or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-            which is time-series data for training, can contain missing values.
-            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-            key-value pairs like a dict, and it has to include the key 'X'.
-
-        val_set : dict or str,
-            The dataset for model validating, should be a dictionary including the key 'X',
-            or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-            which is time-series data for validating, can contain missing values.
-            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-            key-value pairs like a dict, and it has to include the key 'X'.
-
-        file_type : str, default = "h5py",
-            The type of the given file if train_set and val_set are path strings.
-
-        """
         # Step 1: wrap the input data with classes Dataset and DataLoader
-        training_set = DatasetForBRITS(train_set, file_type=file_type)
+        training_set = DatasetForBRITS(
+            train_set, return_labels=False, file_type=file_type
+        )
         training_loader = DataLoader(
             training_set,
             batch_size=self.batch_size,
             shuffle=True,
             num_workers=self.num_workers,
         )
         val_loader = None
@@ -578,15 +508,15 @@
                     # training stage to enhance the model's generalization ability. Therefore, 100,000 representative
                     # samples will be enough to validate the model.
                     val_set = {
                         "X": hf["X"][:],
                         "X_intact": hf["X_intact"][:],
                         "indicating_mask": hf["indicating_mask"][:],
                     }
-            val_set = DatasetForBRITS(val_set, file_type=file_type)
+            val_set = DatasetForBRITS(val_set, return_labels=False, file_type=file_type)
             val_loader = DataLoader(
                 val_set,
                 batch_size=self.batch_size,
                 shuffle=False,
                 num_workers=self.num_workers,
             )
 
@@ -599,41 +529,26 @@
         self._auto_save_model_if_necessary(training_finished=True)
 
     def impute(
         self,
         X: Union[dict, str],
         file_type="h5py",
     ) -> np.ndarray:
-        """Impute missing values in the given data with the trained model.
-
-        Parameters
-        ----------
-        X : array-like or str,
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
-            n_features], or a path string locating a data file, e.g. h5 file.
-
-        file_type : str, default = "h5py",
-            The type of the given file if X is a path string.
-
-        Returns
-        -------
-        array-like, shape [n_samples, sequence length (time steps), n_features],
-            Imputed data.
-        """
         self.model.eval()  # set the model as eval status to freeze it.
         test_set = DatasetForBRITS(X, return_labels=False, file_type=file_type)
         test_loader = DataLoader(
             test_set,
             batch_size=self.batch_size,
             shuffle=False,
             num_workers=self.num_workers,
         )
         imputation_collector = []
 
         with torch.no_grad():
             for idx, data in enumerate(test_loader):
                 inputs = self._assemble_input_for_testing(data)
-                imputed_data = self.model.impute(inputs)
+                results = self.model.forward(inputs, training=False)
+                imputed_data = results["imputed_data"]
                 imputation_collector.append(imputed_data)
 
         imputation_collector = torch.cat(imputation_collector)
         return imputation_collector.cpu().detach().numpy()
```

### Comparing `pypots-0.1.0/pypots/imputation/brits/modules.py` & `pypots-0.1.1/pypots/imputation/brits/modules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.1.0/pypots/imputation/saits/data.py` & `pypots-0.1.1/pypots/imputation/saits/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # License: GLP-v3
 
 from typing import Union, Iterable
 
 import torch
 from pycorruptor import mcar
 
-from pypots.data.base import BaseDataset
+from ...data.base import BaseDataset
 
 
 class DatasetForSAITS(BaseDataset):
     """Dataset for models that need MIT (masked imputation task) in their training, such as SAITS.
 
     For more information about MIT, please refer to :cite:`du2023SAITS`.
```

### Comparing `pypots-0.1.0/pypots/imputation/saits/model.py` & `pypots-0.1.1/pypots/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,530 +1,421 @@
 """
-The implementation of SAITS for the partially-observed time-series imputation task.
-
-Refer to the paper "Du, W., Cote, D., & Liu, Y. (2023). SAITS: Self-Attention-based Imputation for Time Series.
-Expert systems with applications."
-
-Notes
------
-Partial implementation uses code from https://github.com/WenjieDu/SAITS.
-
+The base (abstract) classes for models in PyPOTS.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
-# License: GPL-v3
+# License: GLP-v3
 
-from typing import Tuple, Union, Optional
+import os
+from abc import ABC
+from datetime import datetime
+from typing import Optional, Union
 
-import h5py
-import numpy as np
 import torch
-import torch.nn as nn
-import torch.nn.functional as F
-from torch.utils.data import DataLoader
-
-from pypots.data.base import BaseDataset
-from pypots.imputation.base import BaseNNImputer
-from pypots.imputation.saits.data import DatasetForSAITS
-from pypots.imputation.transformer.modules import EncoderLayer, PositionalEncoding
-from pypots.optim.adam import Adam
-from pypots.optim.base import Optimizer
-from pypots.utils.metrics import cal_mae
-
-
-class _SAITS(nn.Module):
-    def __init__(
-        self,
-        n_layers: int,
-        d_time: int,
-        d_feature: int,
-        d_model: int,
-        d_inner: int,
-        n_heads: int,
-        d_k: int,
-        d_v: int,
-        dropout: float,
-        attn_dropout: float,
-        diagonal_attention_mask: bool = True,
-        ORT_weight: float = 1,
-        MIT_weight: float = 1,
-    ):
-        super().__init__()
-        self.n_layers = n_layers
-        actual_d_feature = d_feature * 2
-        self.ORT_weight = ORT_weight
-        self.MIT_weight = MIT_weight
-
-        self.layer_stack_for_first_block = nn.ModuleList(
-            [
-                EncoderLayer(
-                    d_time,
-                    actual_d_feature,
-                    d_model,
-                    d_inner,
-                    n_heads,
-                    d_k,
-                    d_v,
-                    dropout,
-                    attn_dropout,
-                    diagonal_attention_mask,
-                )
-                for _ in range(n_layers)
-            ]
-        )
-        self.layer_stack_for_second_block = nn.ModuleList(
-            [
-                EncoderLayer(
-                    d_time,
-                    actual_d_feature,
-                    d_model,
-                    d_inner,
-                    n_heads,
-                    d_k,
-                    d_v,
-                    dropout,
-                    attn_dropout,
-                    diagonal_attention_mask,
-                )
-                for _ in range(n_layers)
-            ]
-        )
+from torch.utils.tensorboard import SummaryWriter
 
-        self.dropout = nn.Dropout(p=dropout)
-        self.position_enc = PositionalEncoding(d_model, n_position=d_time)
-        # for operation on time dim
-        self.embedding_1 = nn.Linear(actual_d_feature, d_model)
-        self.reduce_dim_z = nn.Linear(d_model, d_feature)
-        # for operation on measurement dim
-        self.embedding_2 = nn.Linear(actual_d_feature, d_model)
-        self.reduce_dim_beta = nn.Linear(d_model, d_feature)
-        self.reduce_dim_gamma = nn.Linear(d_feature, d_feature)
-        # for delta decay factor
-        self.weight_combine = nn.Linear(d_feature + d_time, d_feature)
-
-    def _process(self, inputs: dict) -> Tuple[torch.Tensor, list]:
-        X, masks = inputs["X"], inputs["missing_mask"]
-        # first DMSA block
-        input_X_for_first = torch.cat([X, masks], dim=2)
-        input_X_for_first = self.embedding_1(input_X_for_first)
-        enc_output = self.dropout(
-            self.position_enc(input_X_for_first)
-        )  # namely, term e in the math equation
-        for encoder_layer in self.layer_stack_for_first_block:
-            enc_output, _ = encoder_layer(enc_output)
-
-        X_tilde_1 = self.reduce_dim_z(enc_output)
-        X_prime = masks * X + (1 - masks) * X_tilde_1
-
-        # second DMSA block
-        input_X_for_second = torch.cat([X_prime, masks], dim=2)
-        input_X_for_second = self.embedding_2(input_X_for_second)
-        enc_output = self.position_enc(
-            input_X_for_second
-        )  # namely term alpha in math algo
-        attn_weights = None
-        for encoder_layer in self.layer_stack_for_second_block:
-            enc_output, attn_weights = encoder_layer(enc_output)
-
-        X_tilde_2 = self.reduce_dim_gamma(F.relu(self.reduce_dim_beta(enc_output)))
-
-        # attention-weighted combine
-        attn_weights = attn_weights.squeeze(dim=1)  # namely term A_hat in Eq.
-        if len(attn_weights.shape) == 4:
-            # if having more than 1 head, then average attention weights from all heads
-            attn_weights = torch.transpose(attn_weights, 1, 3)
-            attn_weights = attn_weights.mean(dim=3)
-            attn_weights = torch.transpose(attn_weights, 1, 2)
-
-        # namely term eta
-        combining_weights = torch.sigmoid(
-            self.weight_combine(torch.cat([masks, attn_weights], dim=2))
-        )
-        # combine X_tilde_1 and X_tilde_2
-        X_tilde_3 = (1 - combining_weights) * X_tilde_2 + combining_weights * X_tilde_1
-        # replace non-missing part with original data
-        X_c = masks * X + (1 - masks) * X_tilde_3
-
-        return X_c, [X_tilde_1, X_tilde_2, X_tilde_3]
-
-    def impute(self, inputs: dict) -> torch.Tensor:
-        imputed_data, _ = self._process(inputs)
-        return imputed_data
-
-    def forward(self, inputs: dict) -> dict:
-        X, masks = inputs["X"], inputs["missing_mask"]
-        ORT_loss = 0
-        imputed_data, [X_tilde_1, X_tilde_2, X_tilde_3] = self._process(inputs)
-
-        ORT_loss += cal_mae(X_tilde_1, X, masks)
-        ORT_loss += cal_mae(X_tilde_2, X, masks)
-        ORT_loss += cal_mae(X_tilde_3, X, masks)
-        ORT_loss /= 3
-
-        MIT_loss = cal_mae(X_tilde_3, inputs["X_intact"], inputs["indicating_mask"])
-
-        # `loss` is always the item for backward propagating to update the model
-        loss = self.ORT_weight * ORT_loss + self.MIT_weight * MIT_loss
-
-        results = {
-            "imputed_data": imputed_data,
-            "ORT_loss": ORT_loss,
-            "MIT_loss": MIT_loss,
-            "loss": loss,  # will be used for backward propagating to update the model
-        }
-        return results
+from .utils.files import create_dir_if_not_exist
+from .utils.logging import logger
 
 
-class SAITS(BaseNNImputer):
-    """The PyTorch implementation of the SAITS model :cite:`du2023SAITS`.
+class BaseModel(ABC):
+    """The base model class for all model implementations.
 
     Parameters
     ----------
-    n_steps : int,
-        The number of time steps in the time-series data sample.
-
-    n_features : int,
-        The number of features in the time-series data sample.
-
-    n_layers : int,
-        The number of layers in the 1st and 2nd DMSA blocks in the SAITS model.
-
-    d_model : int,
-        The dimension of the model's backbone.
-        It is the input dimension of the multi-head DMSA layers.
-
-    d_inner : int,
-        The dimension of the layer in the Feed-Forward Networks (FFN).
-
-    n_heads : int,
-        The number of heads in the multi-head DMSA mechanism.
-        ``d_model`` must be divisible by ``n_heads``, and the result should be equal to ``d_k``.
-
-    d_k : int,
-        The dimension of the `keys` (K) and the `queries` (Q) in the DMSA mechanism.
-        ``d_k`` should be the result of ``d_model`` divided by ``n_heads``. Although ``d_k`` can be directly calculated
-        with given ``d_model`` and ``n_heads``, we want it be explicitly given together with ``d_v`` by users to ensure
-        users be aware of them and to avoid any potential mistakes.
-
-    d_v : int,
-        The dimension of the `values` (V) in the DMSA mechanism.
-
-    dropout : float, 0<= ``dropout`` <1,
-        The dropout rate for all fully-connected layers in the model.
-
-    attn_dropout : float, 0<= ``attn_dropout`` <1,
-        The dropout rate for DMSA.
-
-    diagonal_attention_mask : bool, default = True,
-        Whether to apply a diagonal attention mask to the self-attention mechanism.
-        If so, the attention layers will use DMSA. Otherwise, the attention layers will use the original.
-
-    ORT_weight : float, default = 1.0,
-        The weight for the ORT loss.
-
-    MIT_weight : float, default = 1.0,
-        The weight for the MIT loss.
-
-    batch_size : int, default = 32,
-        The batch size for training and evaluating the model.
-
-    epochs : int, default = 100,
-        The number of epochs for training the model.
-
-    patience : int, default = None,
-        The patience for the early-stopping mechanism. Given a positive integer, the training process will be
-        stopped when the model does not perform better after that number of epochs.
-        Leaving it default as None will disable the early-stopping.
-
-    optimizer : ``pypots.optim.base.Optimizer``, default = ``pypots.optim.Adam()``,
-        The optimizer for model training.
-        If not given, will use a default Adam optimizer.
-
-    num_workers : int, default = 0,
-        The number of subprocesses to use for data loading.
-        `0` means data loading will be in the main process, i.e. there won't be subprocesses.
-
-    device : str or `torch.device`, default = None,
-        The device for the model to run on.
-        If not given, will try to use CUDA devices first (will use the GPU with device number 0 only by default),
+    device :
+        The device for the model to run on. It can be a string, a :class:`torch.device` object, or a list of them.
+        If not given, will try to use CUDA devices first (will use the default CUDA device if there are multiple),
         then CPUs, considering CUDA and CPU are so far the main devices for people to train ML models.
+        If given a list of devices, e.g. ['cuda:0', 'cuda:1'], or [torch.device('cuda:0'), torch.device('cuda:1')] , the
+        model will be parallely trained on the multiple devices (so far only support parallel training on CUDA devices).
         Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
 
-    saving_path : str, default = None,
+    saving_path :
         The path for automatically saving model checkpoints and tensorboard files (i.e. loss values recorded during
         training into a tensorboard file). Will not save if not given.
 
-    model_saving_strategy : str or None, None or "best" or "better" , default = "best",
+    model_saving_strategy :
         The strategy to save model checkpoints. It has to be one of [None, "best", "better"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
 
     Attributes
     ----------
-    model : object,
-        The underlying SAITS model.
+    model : object, default = None
+        The underlying model or algorithm to finish the task.
 
-    optimizer : object,
-        The optimizer for model training.
+    summary_writer : None or torch.utils.tensorboard.SummaryWriter,  default = None,
+        The event writer to save training logs. Default as None. It only works when parameter `tb_file_saving_path` is
+        given, otherwise the training events won't be saved.
+
+        It is designed as being set up while initializing the model because it's created to
+        1). help visualize the model's training procedure (during training not after) and
+        2). assist users to tune the model's hype-parameters.
+        If only setting it up after training with a function like setter(), it cannot achieve the 1st purpose.
 
     """
 
     def __init__(
         self,
-        n_steps: int,
-        n_features: int,
-        n_layers: int,
-        d_model: int,
-        d_inner: int,
-        n_heads: int,
-        d_k: int,
-        d_v: int,
-        dropout: float = 0,
-        attn_dropout: float = 0,
-        diagonal_attention_mask: bool = True,
-        ORT_weight: int = 1,
-        MIT_weight: int = 1,
-        batch_size: int = 32,
-        epochs: int = 100,
-        patience: Optional[int] = None,
-        optimizer: Optional[Optimizer] = Adam(),
-        num_workers: int = 0,
-        device: Optional[Union[str, torch.device]] = None,
-        saving_path: Optional[str] = None,
+        device: Optional[Union[str, torch.device, list]] = None,
+        saving_path: str = None,
         model_saving_strategy: Optional[str] = "best",
     ):
-        super().__init__(
-            batch_size,
-            epochs,
-            patience,
-            num_workers,
-            device,
-            saving_path,
-            model_saving_strategy,
-        )
+        saving_strategies = [None, "best", "better"]
+        assert (
+            model_saving_strategy in saving_strategies
+        ), f"saving_strategy must be one of {saving_strategies}, but got f{model_saving_strategy}."
+
+        self.device = None
+        self.saving_path = saving_path
+        self.model_saving_strategy = model_saving_strategy
+
+        self.model = None
+        self.summary_writer = None
+
+        # set up the device for model running below
+        self._setup_device(device)
+
+        # set up saving_path to save the trained model and training logs
+        self._setup_path(saving_path)
+
+    def _setup_device(self, device):
+        if device is None:
+            # if it is None, then use the first cuda device if cuda is available, otherwise use cpu
+            if torch.cuda.is_available() and torch.cuda.device_count() > 0:
+                self.device = torch.device("cuda")
+            else:
+                self.device = torch.device("cpu")
+            logger.info(f"No given device, using default device: {self.device}")
+        else:
+            if isinstance(device, str):
+                self.device = torch.device(device.lower())
+            elif isinstance(device, torch.device):
+                self.device = device
+            elif isinstance(device, list):
+                # parallely training on multiple CUDA devices
+
+                # ensure the list is not empty
+                assert (
+                    len(device) > 1
+                ), "The list of devices should have at least 1 device, but got 0."
+
+                device_list = []
+                for idx, d in enumerate(device):
+                    if isinstance(d, str):
+                        d = d.lower()
+                        assert (
+                            "cuda" in d
+                        ), "The feature of training on multiple devices currently only support CUDA devices."
+                        device_list.append(torch.device(d))
+                    elif isinstance(d, torch.device):
+                        assert (
+                            "cuda" in d.type
+                        ), "The feature of training on multiple devices currently only support CUDA devices."
+                        device_list.append(d)
+                    else:
+                        raise TypeError(
+                            f"Devices in the list should be str or torch.device, "
+                            f"but the device with index {idx} is {type(d)}."
+                        )
+                if len(device_list) > 1:
+                    self.device = device_list
+                else:
+                    self.device = device_list[0]
+            else:
+                raise TypeError(
+                    f"device should be str/torch.device/a list containing str or torch.device, but got {type(device)}"
+                )
 
-        self.n_steps = n_steps
-        self.n_features = n_features
-        # model hype-parameters
-        self.n_layers = n_layers
-        self.d_model = d_model
-        self.d_inner = d_inner
-        self.n_heads = n_heads
-        self.d_k = d_k
-        self.d_v = d_v
-        self.dropout = dropout
-        self.attn_dropout = attn_dropout
-        self.diagonal_attention_mask = diagonal_attention_mask
-        self.ORT_weight = ORT_weight
-        self.MIT_weight = MIT_weight
-
-        # set up the model
-        self.model = _SAITS(
-            self.n_layers,
-            self.n_steps,
-            self.n_features,
-            self.d_model,
-            self.d_inner,
-            self.n_heads,
-            self.d_k,
-            self.d_v,
-            self.dropout,
-            self.attn_dropout,
-            self.diagonal_attention_mask,
-            self.ORT_weight,
-            self.MIT_weight,
-        )
-        self.model = self.model.to(self.device)
-        self._print_model_size()
+        # check CUDA availability if using CUDA
+        if (isinstance(self.device, list) and "cuda" in self.device[0].type) or (
+            isinstance(self.device, torch.device) and "cuda" in self.device.type
+        ):
+            assert (
+                torch.cuda.is_available() and torch.cuda.device_count() > 0
+            ), "You are trying to use CUDA for model training, but CUDA is not available in your environment."
+
+    def _setup_path(self, saving_path):
+        if isinstance(saving_path, str):
+            # get the current time to append to saving_path,
+            # so you can use the same saving_path to run multiple times
+            # and also be aware of when they were run
+            time_now = datetime.now().__format__("%Y%m%d_T%H%M%S")
+            # the actual saving_path for saving both the best model and the tensorboard file
+            self.saving_path = os.path.join(saving_path, time_now)
+
+            # initialize self.summary_writer only if saving_path is given and not None
+            # otherwise self.summary_writer will be None and the training log won't be saved
+            tb_saving_path = os.path.join(self.saving_path, "tensorboard")
+            self.summary_writer = SummaryWriter(
+                tb_saving_path,
+                filename_suffix=".pypots",
+            )
+            logger.info(f"Model files will be saved to {self.saving_path}")
+            logger.info(f"Tensorboard file will be saved to {tb_saving_path}")
+        else:
+            logger.info(
+                "saving_path not given. Model files and tensorboard file will not be saved."
+            )
 
-        # set up the optimizer
-        self.optimizer = optimizer
-        self.optimizer.init_optimizer(self.model.parameters())
+    def _send_model_to_given_device(self):
+        if isinstance(self.device, list):
+            # parallely training on multiple devices
+            self.model = torch.nn.DataParallel(self.model, device_ids=self.device)
+            self.model = self.model.cuda()
+            logger.info(
+                f"Model has been allocated to the given multiple devices: {self.device}"
+            )
+        else:
+            self.model = self.model.to(self.device)
 
-    def _assemble_input_for_training(self, data: list) -> dict:
-        """Assemble the given data into a dictionary for training input.
+    def _send_data_to_given_device(self, data):
+        if isinstance(self.device, torch.device):  # single device
+            data = map(lambda x: x.to(self.device), data)
+        else:  # parallely training on multiple devices
 
-        Parameters
-        ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
+            # randomly choose one device to balance the workload
+            # device = np.random.choice(self.device)
 
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model training.
-        """
+            data = map(lambda x: x.cuda(), data)
 
-        indices, X_intact, X, missing_mask, indicating_mask = map(
-            lambda x: x.to(self.device), data
-        )
+        return data
 
-        inputs = {
-            "X": X,
-            "X_intact": X_intact,
-            "missing_mask": missing_mask,
-            "indicating_mask": indicating_mask,
-        }
+    def _save_log_into_tb_file(self, step: int, stage: str, loss_dict: dict) -> None:
+        """Saving training logs into the tensorboard file specified by the given path `tb_file_saving_path`.
 
-        return inputs
+        Parameters
+        ----------
+        step :
+            The current training step number.
+            One step for one batch processing, so the number of steps means how many batches the model has processed.
+
+        stage :
+            The stage of the current operation, e.g. 'pretraining', 'training', 'validating'.
+
+        loss_dict :
+            A dictionary containing items to log, should have at least one item, and only items having its name
+            including "loss" or "error" will be logged, e.g. {'imputation_loss': 0.05, "classification_error": 0.32}.
 
-    def _assemble_input_for_validating(self, data) -> dict:
-        """Assemble the given data into a dictionary for validating input.
+        """
+        while len(loss_dict) > 0:
+            (item_name, loss) = loss_dict.popitem()
+            # save all items containing "loss" or "error" in the name
+            # WDU: may enable customization keywords in the future
+            if ("loss" in item_name) or ("error" in item_name):
+                self.summary_writer.add_scalar(f"{stage}/{item_name}", loss.sum(), step)
 
-        Notes
-        -----
-        The validating data assembling processing is the same as training data assembling.
+    def save_model(
+        self,
+        saving_dir: str,
+        file_name: str,
+        overwrite: bool = False,
+    ) -> None:
+        """Save the model with current parameters to a disk file.
 
+        A ``.pypots`` extension will be appended to the filename if it does not already have one.
+        Please note that such an extension is not necessary, but to indicate the saved model is from PyPOTS framework
+        so people can distinguish.
 
         Parameters
         ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
+        saving_dir :
+            The given directory to save the model.
 
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model validating.
-        """
-        indices, X, missing_mask = map(lambda x: x.to(self.device), data)
+        file_name :
+            The file name of the model to be saved.
 
-        inputs = {
-            "X": X,
-            "missing_mask": missing_mask,
-        }
-        return inputs
+        overwrite :
+            Whether to overwrite the model file if the path already exists.
 
-    def _assemble_input_for_testing(self, data) -> dict:
-        """Assemble the given data into a dictionary for testing input.
+        """
+        file_name = (
+            file_name + ".pypots" if file_name.split(".")[-1] != "pypots" else file_name
+        )
+        saving_path = os.path.join(saving_dir, file_name)
 
-        Notes
-        -----
-        The testing data assembling processing is the same as training data assembling.
+        if os.path.exists(saving_path):
+            if overwrite:
+                logger.warning(
+                    f"File {saving_path} exists. Argument `overwrite` is True. Overwriting now..."
+                )
+            else:
+                logger.error(f"File {saving_path} exists. Saving operation aborted.")
+        try:
+            create_dir_if_not_exist(saving_dir)
+            if isinstance(self.device, list):
+                # to save a DataParallel model generically, save the model.module.state_dict()
+                torch.save(self.model.module, saving_path)
+            else:
+                torch.save(self.model, saving_path)
+            logger.info(f"Saved the model to {saving_path}.")
+        except Exception as e:
+            raise RuntimeError(
+                f'Failed to save the model to "{saving_path}" because of the below error! \n{e}'
+            )
+
+    def _auto_save_model_if_necessary(
+        self,
+        training_finished: bool = True,
+        saving_name: str = None,
+    ):
+        """Automatically save the current model into a file if in need.
 
         Parameters
         ----------
-        data : list,
-            A list containing data fetched from Dataset by Dataloader.
+        training_finished :
+            Whether the training is already finished when invoke this function.
+            The saving_strategy "better" only works when training_finished is False.
+            The saving_strategy "best" only works when training_finished is True.
+
+        saving_name :
+            The file name of the saved model.
 
-        Returns
-        -------
-        inputs : dict,
-            A python dictionary contains the input data for model testing.
         """
-        return self._assemble_input_for_validating(data)
+        if self.saving_path is not None and self.model_saving_strategy is not None:
+            name = self.__class__.__name__ if saving_name is None else saving_name
+            if not training_finished and self.model_saving_strategy == "better":
+                self.save_model(self.saving_path, name)
+            elif training_finished and self.model_saving_strategy == "best":
+                self.save_model(self.saving_path, name)
+        else:
+            return
 
-    def fit(
-        self,
-        train_set: Union[dict, str],
-        val_set: Optional[Union[dict, str]] = None,
-        file_type: str = "h5py",
-    ) -> None:
-        """Train the imputer on the given data.
+    def load_model(self, model_path: str) -> None:
+        """Load the saved model from a disk file.
 
         Parameters
         ----------
-        train_set : dict or str,
-            The dataset for model training, should be a dictionary including the key 'X',
-            or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-            which is time-series data for training, can contain missing values.
-            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-            key-value pairs like a dict, and it has to include the key 'X'.
-
-        val_set : dict or str,
-            The dataset for model validating, should be a dictionary including the key 'X',
-            or a path string locating a data file.
-            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
-            which is time-series data for validating, can contain missing values.
-            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
-            key-value pairs like a dict, and it has to include the key 'X'.
+        model_path :
+            Local path to a disk file saving trained model.
 
-        file_type : str, default = "h5py",
-            The type of the given file if train_set and val_set are path strings.
+        Notes
+        -----
+        If the training environment and the deploying/test environment use the same type of device (GPU/CPU),
+        you can load the model directly with torch.load(model_path).
 
         """
-        # Step 1: wrap the input data with classes Dataset and DataLoader
-        training_set = DatasetForSAITS(train_set, file_type=file_type)
-        training_loader = DataLoader(
-            training_set,
-            batch_size=self.batch_size,
-            shuffle=True,
-            num_workers=self.num_workers,
-        )
-        val_loader = None
-        if val_set is not None:
-            if isinstance(val_set, str):
-                with h5py.File(val_set, "r") as hf:
-                    # Here we read the whole validation set from the file to mask a portion for validation.
-                    # In PyPOTS, using a file usually because the data is too big. However, the validation set is
-                    # generally shouldn't be too large. For example, we have 1 billion samples for model training.
-                    # We won't take 20% of them as the validation set because we want as much as possible data for the
-                    # training stage to enhance the model's generalization ability. Therefore, 100,000 representative
-                    # samples will be enough to validate the model.
-                    val_set = {
-                        "X": hf["X"][:],
-                        "X_intact": hf["X_intact"][:],
-                        "indicating_mask": hf["indicating_mask"][:],
-                    }
-
-            val_set = BaseDataset(val_set, file_type=file_type)
-            val_loader = DataLoader(
-                val_set,
-                batch_size=self.batch_size,
-                shuffle=False,
-                num_workers=self.num_workers,
-            )
+        assert os.path.exists(model_path), f"Model file {model_path} does not exist."
 
-        # Step 2: train the model and freeze it
-        self._train_model(training_loader, val_loader)
-        self.model.load_state_dict(self.best_model_dict)
-        self.model.eval()  # set the model as eval status to freeze it.
+        try:
+            if isinstance(self.device, torch.device):
+                loaded_model = torch.load(model_path, map_location=self.device)
+            else:
+                loaded_model = torch.load(model_path)
+            if isinstance(loaded_model, torch.nn.Module):
+                if isinstance(self.device, torch.device):
+                    self.model.load_state_dict(loaded_model.state_dict())
+                else:
+                    self.model.module.load_state_dict(loaded_model.state_dict())
+            else:
+                self.model = loaded_model.model
+        except Exception as e:
+            raise e
+        logger.info(f"Model loaded successfully from {model_path}.")
 
-        # Step 3: save the model if necessary
-        self._auto_save_model_if_necessary(training_finished=True)
 
-    def impute(
-        self,
-        X: Union[dict, str],
-        file_type="h5py",
-    ) -> np.ndarray:
-        """Impute missing values in the given data with the trained model.
+class BaseNNModel(BaseModel):
+    """The abstract class for all neural-network models.
 
-        Parameters
-        ----------
-        X : array-like or str,
-            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
-            n_features], or a path string locating a data file, e.g. h5 file.
-
-        file_type : str, default = "h5py",
-            The type of the given file if X is a path string.
-
-        Returns
-        -------
-        imputed_data : array-like, shape [n_samples, sequence length (time steps), n_features],
-            The imputed data.
+    Parameters
+    ----------
+    batch_size :
+        Size of the batch input into the model for one step.
 
-        """
-        # Step 1: wrap the input data with classes Dataset and DataLoader
-        self.model.eval()  # set the model as eval status to freeze it.
-        test_set = BaseDataset(X, return_labels=False, file_type=file_type)
-        test_loader = DataLoader(
-            test_set,
-            batch_size=self.batch_size,
-            shuffle=False,
-            num_workers=self.num_workers,
+    epochs :
+        Training epochs, i.e. the maximum rounds of the model to be trained with.
+
+    patience :
+        Number of epochs the training procedure will keep if loss doesn't decrease.
+        Once exceeding the number, the training will stop.
+        Must be smaller than or equal to the value of ``epochs``.
+
+    num_workers :
+        The number of subprocesses to use for data loading.
+        `0` means data loading will be in the main process, i.e. there won't be subprocesses.
+
+    device :
+        The device for the model to run on. It can be a string, a :class:`torch.device` object, or a list of them.
+        If not given, will try to use CUDA devices first (will use the default CUDA device if there are multiple),
+        then CPUs, considering CUDA and CPU are so far the main devices for people to train ML models.
+        If given a list of devices, e.g. ['cuda:0', 'cuda:1'], or [torch.device('cuda:0'), torch.device('cuda:1')] , the
+        model will be parallely trained on the multiple devices (so far only support parallel training on CUDA devices).
+        Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
+
+    saving_path :
+        The path for automatically saving model checkpoints and tensorboard files (i.e. loss values recorded during
+        training into a tensorboard file). Will not save if not given.
+
+    model_saving_strategy :
+        The strategy to save model checkpoints. It has to be one of [None, "best", "better"].
+        No model will be saved when it is set as None.
+        The "best" strategy will only automatically save the best model after the training finished.
+        The "better" strategy will automatically save the model during training whenever the model performs
+        better than in previous epochs.
+
+
+    Attributes
+    ---------
+    best_model_dict : dict, default = None,
+        A dictionary contains the trained model that achieves the best performance according to the loss defined,
+        i.e. the lowest loss.
+
+    best_loss : float, default = inf,
+        The criteria to judge whether the model's performance is the best so far.
+        Usually the lower, the better.
+
+
+    Notes
+    -----
+    Optimizers are necessary for training deep-learning neural networks, but we don't put a parameter ``optimizer``
+    here because some models (e.g. GANs) need more than one optimizer (e.g. one for generator, one for discriminator),
+    and ``optimizer`` is ambiguous for them. Therefore, we leave optimizers as parameters for concrete model
+    implementations, and you can pass any number of optimizers to your model when implementing it,
+    :class:`pypots.clustering.crli.CRLI` for example.
+
+    """
+
+    def __init__(
+        self,
+        batch_size: int,
+        epochs: int,
+        patience: int,
+        num_workers: int = 0,
+        device: Optional[Union[str, torch.device, list]] = None,
+        saving_path: str = None,
+        model_saving_strategy: Optional[str] = "best",
+    ):
+        super().__init__(
+            device,
+            saving_path,
+            model_saving_strategy,
         )
-        imputation_collector = []
 
-        # Step 2: process the data with the model
-        with torch.no_grad():
-            for idx, data in enumerate(test_loader):
-                inputs = self._assemble_input_for_testing(data)
-                imputed_data = self.model.impute(inputs)
-                imputation_collector.append(imputed_data)
-
-        # Step 3: output collection and return
-        imputation_collector = torch.cat(imputation_collector)
-        imputed_data = imputation_collector.cpu().detach().numpy()
-        return imputed_data
+        if patience is None:
+            patience = -1  # early stopping on patience won't work if it is set as < 0
+        else:
+            assert (
+                patience <= epochs
+            ), f"patience must be smaller than epoches which is {epochs}, but got patience={patience}"
+
+        # training hype-parameters
+        self.batch_size = batch_size
+        self.epochs = epochs
+        self.patience = patience
+        self.original_patience = patience
+        self.num_workers = num_workers
+
+        self.model = None
+        self.optimizer = None
+        self.best_model_dict = None
+        # WDU: may enable users to customize the criteria in the future
+        self.best_loss = float("inf")
+
+    def _print_model_size(self) -> None:
+        """Print the number of trainable parameters in the initialized NN model."""
+        num_params = sum(p.numel() for p in self.model.parameters() if p.requires_grad)
+        logger.info(
+            f"Model initialized successfully with the number of trainable parameters: {num_params:,}"
+        )
```

### Comparing `pypots-0.1.0/pypots/imputation/transformer/model.py` & `pypots-0.1.1/pypots/imputation/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,458 +1,412 @@
 """
-The implementation of Transformer for the partially-observed time-series imputation task.
-
-Refer to the paper "Du, W., Cote, D., & Liu, Y. (2023). SAITS: Self-Attention-based Imputation for Time Series.
-Expert systems with applications."
-
-Notes
------
-Partial implementation uses code from https://github.com/WenjieDu/SAITS.
-
+The base class for PyPOTS imputation models.
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GPL-v3
 
-from typing import Tuple, Union, Optional
 
-import h5py
+import os
+from abc import abstractmethod
+from typing import Union, Optional
+
 import numpy as np
 import torch
-import torch.nn as nn
 from torch.utils.data import DataLoader
 
-from pypots.data.base import BaseDataset
-from pypots.imputation.base import BaseNNImputer
-from pypots.imputation.transformer.data import DatasetForSAITS
-from pypots.imputation.transformer.modules import EncoderLayer, PositionalEncoding
-from pypots.optim.adam import Adam
-from pypots.optim.base import Optimizer
-from pypots.utils.metrics import cal_mae
+from ..base import BaseModel, BaseNNModel
+from ..utils.logging import logger
+from ..utils.metrics import cal_mae
+
+try:
+    import nni
+except ImportError:
+    pass
 
 
-class _TransformerEncoder(nn.Module):
-    def __init__(
-        self,
-        n_layers: int,
-        d_time: int,
-        d_feature: int,
-        d_model: int,
-        d_inner: int,
-        n_heads: int,
-        d_k: int,
-        d_v: int,
-        dropout: float,
-        attn_dropout: float,
-        ORT_weight: float = 1,
-        MIT_weight: float = 1,
-    ):
-        super().__init__()
-        self.n_layers = n_layers
-        actual_d_feature = d_feature * 2
-        self.ORT_weight = ORT_weight
-        self.MIT_weight = MIT_weight
-
-        self.layer_stack = nn.ModuleList(
-            [
-                EncoderLayer(
-                    d_time,
-                    actual_d_feature,
-                    d_model,
-                    d_inner,
-                    n_heads,
-                    d_k,
-                    d_v,
-                    dropout,
-                    attn_dropout,
-                    False,
-                )
-                for _ in range(n_layers)
-            ]
-        )
-
-        self.embedding = nn.Linear(actual_d_feature, d_model)
-        self.position_enc = PositionalEncoding(d_model, n_position=d_time)
-        self.dropout = nn.Dropout(p=dropout)
-        self.reduce_dim = nn.Linear(d_model, d_feature)
-
-    def _process(self, inputs: dict) -> Tuple[torch.Tensor, torch.Tensor]:
-        X, masks = inputs["X"], inputs["missing_mask"]
-        input_X = torch.cat([X, masks], dim=2)
-        input_X = self.embedding(input_X)
-        enc_output = self.dropout(self.position_enc(input_X))
-
-        for encoder_layer in self.layer_stack:
-            enc_output, _ = encoder_layer(enc_output)
-
-        learned_presentation = self.reduce_dim(enc_output)
-        imputed_data = (
-            masks * X + (1 - masks) * learned_presentation
-        )  # replace non-missing part with original data
-        return imputed_data, learned_presentation
-
-    def impute(self, inputs: dict) -> torch.Tensor:
-        imputed_data, _ = self._process(inputs)
-        return imputed_data
-
-    def forward(self, inputs: dict) -> dict:
-        X, masks = inputs["X"], inputs["missing_mask"]
-        imputed_data, learned_presentation = self._process(inputs)
-        ORT_loss = cal_mae(learned_presentation, X, masks)
+class BaseImputer(BaseModel):
+    """Abstract class for all imputation models.
 
-        MIT_loss = cal_mae(
-            learned_presentation, inputs["X_intact"], inputs["indicating_mask"]
-        )
+    Parameters
+    ----------
+    device :
+        The device for the model to run on. It can be a string, a :class:`torch.device` object, or a list of them.
+        If not given, will try to use CUDA devices first (will use the default CUDA device if there are multiple),
+        then CPUs, considering CUDA and CPU are so far the main devices for people to train ML models.
+        If given a list of devices, e.g. ['cuda:0', 'cuda:1'], or [torch.device('cuda:0'), torch.device('cuda:1')] , the
+        model will be parallely trained on the multiple devices (so far only support parallel training on CUDA devices).
+        Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
 
-        # `loss` is always the item for backward propagating to update the model
-        loss = self.ORT_weight * ORT_loss + self.MIT_weight * MIT_loss
+    saving_path :
+        The path for automatically saving model checkpoints and tensorboard files (i.e. loss values recorded during
+        training into a tensorboard file). Will not save if not given.
 
-        results = {
-            "imputed_data": imputed_data,
-            "ORT_loss": ORT_loss,
-            "MIT_loss": MIT_loss,
-            "loss": loss,
-        }
-        return results
-
-
-class Transformer(BaseNNImputer):
-    """The PyTorch implementation of the Transformer model.
-    Transformer is originally proposed by Vaswani et al. in :cite:`vaswani2017Transformer`,
-    and gets re-implemented as a time-series imputation model by Du et al. in :cite:`du2023SAITS`.
-    Here you should refer to :cite:`du2023SAITS` for details about this Transformer imputation model.
+    model_saving_strategy :
+        The strategy to save model checkpoints. It has to be one of [None, "best", "better"].
+        No model will be saved when it is set as None.
+        The "best" strategy will only automatically save the best model after the training finished.
+        The "better" strategy will automatically save the model during training whenever the model performs
+        better than in previous epochs.
 
-    Parameters
-    ----------
-    n_steps : int,
-        The number of time steps in the time-series data sample.
+    """
 
-    n_features : int,
-        The number of features in the time-series data sample.
+    def __init__(
+        self,
+        device: Optional[Union[str, torch.device, list]] = None,
+        saving_path: str = None,
+        model_saving_strategy: Optional[str] = "best",
+    ):
+        super().__init__(
+            device,
+            saving_path,
+            model_saving_strategy,
+        )
 
-    n_layers : int,
-        The number of layers in the 1st and 2nd DMSA blocks in the SAITS model.
+    @abstractmethod
+    def fit(
+        self,
+        train_set: Union[dict, str],
+        val_set: Optional[Union[dict, str]] = None,
+        file_type: str = "h5py",
+    ) -> None:
+        """Train the imputer on the given data.
 
-    d_model : int,
-        The dimension of the model's backbone.
-        It is the input dimension of the multi-head self-attention layers.
+        Parameters
+        ----------
+        train_set :
+            The dataset for model training, should be a dictionary including the key 'X',
+            or a path string locating a data file.
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            which is time-series data for training, can contain missing values.
+            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
+            key-value pairs like a dict, and it has to include the key 'X'.
 
-    d_inner : int,
-        The dimension of the layer in the Feed-Forward Networks (FFN).
+        val_set :
+            The dataset for model validating, should be a dictionary including the key 'X',
+            or a path string locating a data file.
+            If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
+            which is time-series data for validating, can contain missing values.
+            If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
+            key-value pairs like a dict, and it has to include the key 'X'.
 
-    n_heads : int,
-        The number of heads in the multi-head self-attention mechanism.
-        ``d_model`` must be divisible by ``n_heads``, and the result should be equal to ``d_k``.
+        file_type : str, default = "h5py",
+            The type of the given file if train_set and val_set are path strings.
 
-    d_k : int,
-        The dimension of the `keys` (K) and the `queries` (Q) in the DMSA mechanism.
-        ``d_k`` should be the result of ``d_model`` divided by ``n_heads``. Although ``d_k`` can be directly calculated
-        with given ``d_model`` and ``n_heads``, we want it be explicitly given together with ``d_v`` by users to ensure
-        users be aware of them and to avoid any potential mistakes.
+        """
+        raise NotImplementedError
 
-    d_v : int,
-        The dimension of the `values` (V) in the DMSA mechanism.
+    @abstractmethod
+    def impute(
+        self,
+        X: Union[dict, str],
+        file_type: str = "h5py",
+    ) -> np.ndarray:
+        """Impute missing values in the given data with the trained model.
 
-    dropout : float, 0<= ``dropout`` <1,
-        The dropout rate for all fully-connected layers in the model.
+        Parameters
+        ----------
+        X :
+            The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
+            n_features], or a path string locating a data file, e.g. h5 file.
 
-    attn_dropout : float, 0<= ``attn_dropout`` <1,
-        The dropout rate for DMSA.
+        file_type :
+            The type of the given file if X is a path string.
 
-    ORT_weight : float, default = 1.0,
-        The weight for the ORT loss.
+        Returns
+        -------
+        array-like, shape [n_samples, sequence length (time steps), n_features],
+            Imputed data.
+        """
+        raise NotImplementedError
 
-    MIT_weight : float, default = 1.0,
-        The weight for the MIT loss.
 
-    batch_size : int, default = 32,
-        The batch size for training and evaluating the model.
+class BaseNNImputer(BaseNNModel):
+    """The abstract class for all neural-network imputation models in PyPOTS.
 
-    epochs : int, default = 100,
-        The number of epochs for training the model.
+    Parameters
+    ----------
+    batch_size :
+        Size of the batch input into the model for one step.
 
-    patience : int, default = None,
-        The patience for the early-stopping mechanism. Given a positive integer, the training process will be
-        stopped when the model does not perform better after that number of epochs.
-        Leaving it default as None will disable the early-stopping.
+    epochs :
+        Training epochs, i.e. the maximum rounds of the model to be trained with.
 
-    optimizer : ``pypots.optim.base.Optimizer``, default = ``pypots.optim.Adam()``,
-        The optimizer for model training.
-        If not given, will use a default Adam optimizer.
+    patience :
+        Number of epochs the training procedure will keep if loss doesn't decrease.
+        Once exceeding the number, the training will stop.
+        Must be smaller than or equal to the value of ``epochs``.
 
-    num_workers : int, default = 0,
+    num_workers :
         The number of subprocesses to use for data loading.
         `0` means data loading will be in the main process, i.e. there won't be subprocesses.
 
-    device : str or `torch.device`, default = None,
-        The device for the model to run on.
-        If not given, will try to use CUDA devices first (will use the GPU with device number 0 only by default),
+    device :
+        The device for the model to run on. It can be a string, a :class:`torch.device` object, or a list of them.
+        If not given, will try to use CUDA devices first (will use the default CUDA device if there are multiple),
         then CPUs, considering CUDA and CPU are so far the main devices for people to train ML models.
+        If given a list of devices, e.g. ['cuda:0', 'cuda:1'], or [torch.device('cuda:0'), torch.device('cuda:1')] , the
+        model will be parallely trained on the multiple devices (so far only support parallel training on CUDA devices).
         Other devices like Google TPU and Apple Silicon accelerator MPS may be added in the future.
 
-    saving_path : str, default = None,
+    saving_path :
         The path for automatically saving model checkpoints and tensorboard files (i.e. loss values recorded during
         training into a tensorboard file). Will not save if not given.
 
-    model_saving_strategy : str or None, None or "best" or "better" , default = "best",
+    model_saving_strategy :
         The strategy to save model checkpoints. It has to be one of [None, "best", "better"].
         No model will be saved when it is set as None.
         The "best" strategy will only automatically save the best model after the training finished.
         The "better" strategy will automatically save the model during training whenever the model performs
         better than in previous epochs.
 
-    Attributes
-    ----------
-    model : object,
-        The underlying Transformer model.
-
-    optimizer : object,
-        The optimizer for model training.
+    Notes
+    -----
+    Optimizers are necessary for training deep-learning neural networks, but we don't put  a parameter ``optimizer``
+    here because some models (e.g. GANs) need more than one optimizer (e.g. one for generator, one for discriminator),
+    and ``optimizer`` is ambiguous for them. Therefore, we leave optimizers as parameters for concrete model
+    implementations, and you can pass any number of optimizers to your model when implementing it,
+    :class:`pypots.clustering.crli.CRLI` for example.
 
     """
 
     def __init__(
         self,
-        n_steps: int,
-        n_features: int,
-        n_layers: int,
-        d_model: int,
-        d_inner: int,
-        n_heads: int,
-        d_k: int,
-        d_v: int,
-        dropout: float = 0,
-        attn_dropout: float = 0,
-        ORT_weight: int = 1,
-        MIT_weight: int = 1,
-        batch_size: int = 32,
-        epochs: int = 100,
-        patience: int = None,
-        optimizer: Optional[Optimizer] = Adam(),
+        batch_size: int,
+        epochs: int,
+        patience: int,
         num_workers: int = 0,
-        device: Optional[Union[str, torch.device]] = None,
+        device: Optional[Union[str, torch.device, list]] = None,
         saving_path: str = None,
         model_saving_strategy: Optional[str] = "best",
     ):
         super().__init__(
             batch_size,
             epochs,
             patience,
             num_workers,
             device,
             saving_path,
             model_saving_strategy,
         )
 
-        self.n_steps = n_steps
-        self.n_features = n_features
-        # model hype-parameters
-        self.n_layers = n_layers
-        self.d_model = d_model
-        self.d_inner = d_inner
-        self.n_heads = n_heads
-        self.d_k = d_k
-        self.d_v = d_v
-        self.dropout = dropout
-        self.attn_dropout = attn_dropout
-        self.ORT_weight = ORT_weight
-        self.MIT_weight = MIT_weight
-
-        # set up the model
-        self.model = _TransformerEncoder(
-            self.n_layers,
-            self.n_steps,
-            self.n_features,
-            self.d_model,
-            self.d_inner,
-            self.n_heads,
-            self.d_k,
-            self.d_v,
-            self.dropout,
-            self.ORT_weight,
-            self.MIT_weight,
-        )
-        self.model = self.model.to(self.device)
-        self._print_model_size()
-
-        # set up the optimizer
-        self.optimizer = optimizer
-        self.optimizer.init_optimizer(self.model.parameters())
-
-    def _assemble_input_for_training(self, data: dict) -> dict:
+    @abstractmethod
+    def _assemble_input_for_training(self, data: list) -> dict:
         """Assemble the given data into a dictionary for training input.
 
         Parameters
         ----------
         data : list,
-            A list containing data fetched from Dataset by Dataloader.
+            Input data from dataloader, should be list.
 
         Returns
         -------
-        inputs : dict,
+        dict,
             A python dictionary contains the input data for model training.
         """
+        raise NotImplementedError
 
-        indices, X_intact, X, missing_mask, indicating_mask = map(
-            lambda x: x.to(self.device), data
-        )
-
-        inputs = {
-            "X": X,
-            "X_intact": X_intact,
-            "missing_mask": missing_mask,
-            "indicating_mask": indicating_mask,
-        }
-
-        return inputs
-
+    @abstractmethod
     def _assemble_input_for_validating(self, data: list) -> dict:
         """Assemble the given data into a dictionary for validating input.
 
-        Notes
-        -----
-        The validating data assembling processing is the same as training data assembling.
-
-
         Parameters
         ----------
         data : list,
-            A list containing data fetched from Dataset by Dataloader.
+            Data output from dataloader, should be list.
 
         Returns
         -------
-        inputs : dict,
+        dict,
             A python dictionary contains the input data for model validating.
         """
-        indices, X, missing_mask = map(lambda x: x.to(self.device), data)
-
-        inputs = {
-            "X": X,
-            "missing_mask": missing_mask,
-        }
-
-        return inputs
+        raise NotImplementedError
 
+    @abstractmethod
     def _assemble_input_for_testing(self, data: list) -> dict:
         """Assemble the given data into a dictionary for testing input.
 
         Notes
         -----
-        The testing data assembling processing is the same as training data assembling.
+        The processing functions of train/val/test stages are separated for the situation that the input of
+        the three stages are different, and this situation usually happens when the Dataset/Dataloader classes
+        used in the train/val/test stages are not the same, e.g. the training data and validating data in a
+        classification task contains labels, but the testing data (from the production environment) generally
+        doesn't have labels.
 
         Parameters
         ----------
         data : list,
-            A list containing data fetched from Dataset by Dataloader.
+            Data output from dataloader, should be list.
 
         Returns
         -------
-        inputs : dict,
+        dict,
             A python dictionary contains the input data for model testing.
         """
-        return self._assemble_input_for_validating(data)
+        raise NotImplementedError
+
+    def _train_model(
+        self,
+        training_loader: DataLoader,
+        val_loader: DataLoader = None,
+    ) -> None:
+        # each training starts from the very beginning, so reset the loss and model dict here
+        self.best_loss = float("inf")
+        self.best_model_dict = None
+
+        try:
+            training_step = 0
+            for epoch in range(self.epochs):
+                self.model.train()
+                epoch_train_loss_collector = []
+                for idx, data in enumerate(training_loader):
+                    training_step += 1
+                    inputs = self._assemble_input_for_training(data)
+                    self.optimizer.zero_grad()
+                    results = self.model.forward(inputs)
+                    # use sum() before backward() in case of multi-gpu training
+                    results["loss"].sum().backward()
+                    self.optimizer.step()
+                    epoch_train_loss_collector.append(results["loss"].sum().item())
+
+                    # save training loss logs into the tensorboard file for every step if in need
+                    if self.summary_writer is not None:
+                        self._save_log_into_tb_file(training_step, "training", results)
+
+                # mean training loss of the current epoch
+                mean_train_loss = np.mean(epoch_train_loss_collector)
+
+                if val_loader is not None:
+                    self.model.eval()
+                    imputation_collector = []
+                    with torch.no_grad():
+                        for idx, data in enumerate(val_loader):
+                            inputs = self._assemble_input_for_validating(data)
+                            results = self.model.forward(inputs, training=False)
+                            imputed_data = results["imputed_data"]
+                            imputation_collector.append(imputed_data)
+
+                    imputation_collector = torch.cat(imputation_collector)
+                    imputation_collector = imputation_collector.cpu().detach().numpy()
+
+                    mean_val_loss = cal_mae(
+                        imputation_collector,
+                        val_loader.dataset.data["X_intact"],
+                        val_loader.dataset.data["indicating_mask"],
+                        # the above val_loader.dataset.data is a dict containing the validation dataset
+                    )
+
+                    # save validating loss logs into the tensorboard file for every epoch if in need
+                    if self.summary_writer is not None:
+                        val_loss_dict = {
+                            "imputation_loss": mean_val_loss,
+                        }
+                        self._save_log_into_tb_file(epoch, "validating", val_loss_dict)
+
+                    logger.info(
+                        f"epoch {epoch}: "
+                        f"training loss {mean_train_loss:.4f}, "
+                        f"validating loss {mean_val_loss:.4f}"
+                    )
+                    mean_loss = mean_val_loss
+                else:
+                    logger.info(f"epoch {epoch}: training loss {mean_train_loss:.4f}")
+                    mean_loss = mean_train_loss
+
+                if mean_loss < self.best_loss:
+                    self.best_loss = mean_loss
+                    self.best_model_dict = self.model.state_dict()
+                    self.patience = self.original_patience
+                    # save the model if necessary
+                    self._auto_save_model_if_necessary(
+                        training_finished=False,
+                        saving_name=f"{self.__class__.__name__}_epoch{epoch}_loss{mean_loss}",
+                    )
+                else:
+                    self.patience -= 1
+
+                if os.getenv("enable_nni", False):
+                    nni.report_intermediate_result(mean_loss)
+                    if epoch == self.epochs - 1 or self.patience == 0:
+                        nni.report_final_result(self.best_loss)
+
+                if self.patience == 0:
+                    logger.info(
+                        "Exceeded the training patience. Terminating the training procedure..."
+                    )
+                    break
+
+        except Exception as e:
+            logger.error(f"Exception: {e}")
+            if self.best_model_dict is None:
+                raise RuntimeError(
+                    "Training got interrupted. Model was not trained. Please investigate the error printed above."
+                )
+            else:
+                RuntimeWarning(
+                    "Training got interrupted. Please investigate the error printed above.\n"
+                    "Model got trained and will load the best checkpoint so far for testing.\n"
+                    "If you don't want it, please try fit() again."
+                )
+
+        if np.equal(self.best_loss.item(), float("inf")):
+            raise ValueError("Something is wrong. best_loss is Nan after training.")
 
+        logger.info("Finished training.")
+
+    @abstractmethod
     def fit(
         self,
         train_set: Union[dict, str],
         val_set: Optional[Union[dict, str]] = None,
         file_type: str = "h5py",
     ) -> None:
         """Train the imputer on the given data.
 
         Parameters
         ----------
-        train_set : dict or str,
+        train_set :
             The dataset for model training, should be a dictionary including the key 'X',
             or a path string locating a data file.
             If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
             which is time-series data for training, can contain missing values.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include the key 'X'.
 
-        val_set : dict or str,
+        val_set :
             The dataset for model validating, should be a dictionary including the key 'X',
             or a path string locating a data file.
             If it is a dict, X should be array-like of shape [n_samples, sequence length (time steps), n_features],
             which is time-series data for validating, can contain missing values.
             If it is a path string, the path should point to a data file, e.g. a h5 file, which contains
             key-value pairs like a dict, and it has to include the key 'X'.
 
         file_type : str, default = "h5py",
             The type of the given file if train_set and val_set are path strings.
 
         """
-        # Step 1: wrap the input data with classes Dataset and DataLoader
-        training_set = DatasetForSAITS(train_set, file_type=file_type)
-        training_loader = DataLoader(
-            training_set,
-            batch_size=self.batch_size,
-            shuffle=True,
-            num_workers=self.num_workers,
-        )
-        val_loader = None
-        if val_set is not None:
-            if isinstance(val_set, str):
-                with h5py.File(val_set, "r") as hf:
-                    # Here we read the whole validation set from the file to mask a portion for validation.
-                    # In PyPOTS, using a file usually because the data is too big. However, the validation set is
-                    # generally shouldn't be too large. For example, we have 1 billion samples for model training.
-                    # We won't take 20% of them as the validation set because we want as much as possible data for the
-                    # training stage to enhance the model's generalization ability. Therefore, 100,000 representative
-                    # samples will be enough to validate the model.
-                    val_set = {
-                        "X": hf["X"][:],
-                        "X_intact": hf["X_intact"][:],
-                        "indicating_mask": hf["indicating_mask"][:],
-                    }
-
-            val_set = BaseDataset(val_set, file_type=file_type)
-            val_loader = DataLoader(
-                val_set,
-                batch_size=self.batch_size,
-                shuffle=False,
-                num_workers=self.num_workers,
-            )
-
-        # Step 2: train the model and freeze it
-        self._train_model(training_loader, val_loader)
-        self.model.load_state_dict(self.best_model_dict)
-        self.model.eval()  # set the model as eval status to freeze it.
-
-        # Step 3: save the model if necessary
-        self._auto_save_model_if_necessary(training_finished=True)
+        raise NotImplementedError
 
-    def impute(self, X: Union[dict, str], file_type: str = "h5py") -> np.ndarray:
+    @abstractmethod
+    def impute(
+        self,
+        X: Union[dict, str],
+        file_type: str = "h5py",
+    ) -> np.ndarray:
         """Impute missing values in the given data with the trained model.
 
         Parameters
         ----------
-        X : array-like or str,
+        X :
             The data samples for testing, should be array-like of shape [n_samples, sequence length (time steps),
             n_features], or a path string locating a data file, e.g. h5 file.
 
-        file_type : str, default = "h5py",
+        file_type :
             The type of the given file if X is a path string.
 
         Returns
         -------
         array-like, shape [n_samples, sequence length (time steps), n_features],
             Imputed data.
         """
-        self.model.eval()  # set the model as eval status to freeze it.
-        test_set = BaseDataset(X, return_labels=False, file_type=file_type)
-        test_loader = DataLoader(
-            test_set,
-            batch_size=self.batch_size,
-            shuffle=False,
-            num_workers=self.num_workers,
-        )
-        imputation_collector = []
-
-        with torch.no_grad():
-            for idx, data in enumerate(test_loader):
-                inputs = self._assemble_input_for_testing(data)
-                imputed_data = self.model.impute(inputs)
-                imputation_collector.append(imputed_data)
-
-        imputation_collector = torch.cat(imputation_collector)
-        return imputation_collector.cpu().detach().numpy()
+        raise NotImplementedError
```

### Comparing `pypots-0.1.0/pypots/imputation/transformer/modules.py` & `pypots-0.1.1/pypots/imputation/transformer/modules.py`

 * *Files identical despite different names*

### Comparing `pypots-0.1.0/pypots/optim/adagrad.py` & `pypots-0.1.1/pypots/optim/adagrad.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 from typing import Iterable
 
 from torch.optim import Adagrad as torch_Adagrad
 
-from pypots.optim.base import Optimizer
+from .base import Optimizer
 
 
 class Adagrad(Optimizer):
     """The optimizer wrapper for PyTorch Adagrad.
     https://pytorch.org/docs/stable/generated/torch.optim.Adagrad.html#torch.optim.Adagrad
 
     Parameters
     ----------
-    lr : float, default=0.01
+    lr :
         The learning rate of the optimizer.
 
-    lr_decay : float, default=0
+    lr_decay :
         Learning rate decay.
 
-    weight_decay : float, default=0.01
+    weight_decay :
         Weight decay (L2 penalty).
 
-    eps : float, default=1e-08
+    eps :
         Term added to the denominator to improve numerical stability.
 
-    initial_accumulator_value : float, default=0.01
+    initial_accumulator_value :
         A floating point value. Starting value for the accumulators, must be positive.
 
     """
 
     def __init__(
         self,
         lr: float = 0.01,
@@ -51,16 +51,17 @@
         self.eps = eps
 
     def init_optimizer(self, params: Iterable) -> None:
         """Initialize the torch optimizer wrapped by this class.
 
         Parameters
         ----------
-        params : Iterable,
+        params :
             An iterable of ``torch.Tensor`` or ``dict``. Specifies what Tensors should be optimized.
+
         """
         self.torch_optimizer = torch_Adagrad(
             params=params,
             lr=self.lr,
             lr_decay=self.lr_decay,
             weight_decay=self.weight_decay,
             initial_accumulator_value=self.initial_accumulator_value,
```

### Comparing `pypots-0.1.0/pypots/optim/adam.py` & `pypots-0.1.1/pypots/optim/adam.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 from typing import Iterable, Tuple
 
 from torch.optim import Adam as torch_Adam
 
-from pypots.optim.base import Optimizer
+from .base import Optimizer
 
 
 class Adam(Optimizer):
     """The optimizer wrapper for PyTorch Adam.
     https://pytorch.org/docs/stable/generated/torch.optim.Adam.html#torch.optim.Adam
 
     Parameters
     ----------
-    lr : float, default=0.001,
+    lr :
         The learning rate of the optimizer.
 
-    betas : Tuple[float, float], default=(0.9, 0.999),
+    betas :
         Coefficients used for computing running averages of gradient and its square.
 
-    eps : float, default=1e-08,
+    eps :
         Term added to the denominator to improve numerical stability.
 
-    weight_decay : float, default=0,
+    weight_decay :
         Weight decay (L2 penalty).
 
-    amsgrad : bool, default=False,
+    amsgrad :
         Whether to use the AMSGrad variant of this algorithm from the paper :cite:`reddi2018OnTheConvergence`.
     """
 
     def __init__(
         self,
         lr: float = 0.001,
         betas: Tuple[float, float] = (0.9, 0.999),
@@ -50,16 +50,17 @@
         self.amsgrad = amsgrad
 
     def init_optimizer(self, params: Iterable) -> None:
         """Initialize the torch optimizer wrapped by this class.
 
         Parameters
         ----------
-        params : Iterable,
+        params :
             An iterable of ``torch.Tensor`` or ``dict``. Specifies what Tensors should be optimized.
+
         """
         self.torch_optimizer = torch_Adam(
             params=params,
             lr=self.lr,
             betas=self.betas,
             eps=self.eps,
             weight_decay=self.weight_decay,
```

### Comparing `pypots-0.1.0/pypots/optim/adamw.py` & `pypots-0.1.1/pypots/optim/adamw.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 from typing import Iterable, Tuple
 
 from torch.optim import AdamW as torch_AdamW
 
-from pypots.optim.base import Optimizer
+from .base import Optimizer
 
 
 class AdamW(Optimizer):
     """The optimizer wrapper for PyTorch AdamW.
     https://pytorch.org/docs/stable/generated/torch.optim.AdamW.html#torch.optim.AdamW
 
     Parameters
     ----------
-    lr : float, default=0.001,
+    lr :
         The learning rate of the optimizer.
 
-    betas : Tuple[float, float], default=(0.9, 0.999),
+    betas :
         Coefficients used for computing running averages of gradient and its square.
 
-    eps : float, default=1e-08,
+    eps :
         Term added to the denominator to improve numerical stability.
 
-    weight_decay : float, default=0.01,
+    weight_decay :
         Weight decay (L2 penalty).
 
-    amsgrad : bool, default=False,
+    amsgrad :
         Whether to use the AMSGrad variant of this algorithm from the paper :cite:`reddi2018OnTheConvergence`.
     """
 
     def __init__(
         self,
         lr: float = 0.001,
         betas: Tuple[float, float] = (0.9, 0.999),
@@ -50,16 +50,17 @@
         self.amsgrad = amsgrad
 
     def init_optimizer(self, params: Iterable) -> None:
         """Initialize the torch optimizer wrapped by this class.
 
         Parameters
         ----------
-        params : Iterable,
+        params :
             An iterable of ``torch.Tensor`` or ``dict``. Specifies what Tensors should be optimized.
+
         """
         self.torch_optimizer = torch_AdamW(
             params=params,
             lr=self.lr,
             betas=self.betas,
             eps=self.eps,
             weight_decay=self.weight_decay,
```

### Comparing `pypots-0.1.0/pypots/optim/base.py` & `pypots-0.1.1/pypots/optim/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,90 +21,90 @@
 
 
 class Optimizer(ABC):
     """The base wrapper for PyTorch optimizers, also is the base class for all optimizers in pypots.optim.
 
     Parameters
     ----------
-    lr : float,
+    lr :
         The learning rate of the optimizer.
 
     Attributes
     ----------
-    torch_optimizer : torch.optim.Optimizer,
+    torch_optimizer :
         The torch optimizer wrapped by this class.
 
     """
 
     def __init__(self, lr):
         self.lr = lr
         self.torch_optimizer = None
 
     @abstractmethod
     def init_optimizer(self, params: Iterable) -> None:
         """Initialize the torch optimizer wrapped by this class.
 
         Parameters
         ----------
-        params : Iterable,
+        params :
             An iterable of ``torch.Tensor`` or ``dict``. Specifies what Tensors should be optimized.
         """
         raise NotImplementedError
 
     def add_param_group(self, param_group: dict) -> None:
         """Add a param group to the optimizer param_groups.
 
         Parameters
         ----------
-        param_group : dict,
+        param_group :
             Specifies the parameters to be optimized and group-specific optimization options.
         """
         self.torch_optimizer.add_param_group(param_group)
 
     def load_state_dict(self, state_dict) -> None:
         """Loads the optimizer state.
 
         Parameters
         ----------
-        state_dict : dict,
+        state_dict :
             Optimizer state. It should be an object returned from ``state_dict()``.
         """
 
         self.torch_optimizer.load_state_dict(state_dict)
 
     def state_dict(self) -> dict:
         """Returns the state of the optimizer as a dict.
 
         Returns
         -------
-        state_dict : dict,
+        state_dict :
             The state dict of the optimizer, which contains two entries:
             1). state - a dict holding current optimization state. Its content differs between optimizer classes.
             2). param_groups - a list containing all parameter groups where each parameter group is a dict
 
         """
         state_dict = self.torch_optimizer.state_dict()
         return state_dict
 
     def step(self, closure: Optional[Callable] = None) -> None:
         """Performs a single optimization step (parameter update).
 
         Parameters
         ----------
-        closure : Callable, optional, default=None,
+        closure :
             A closure that reevaluates the model and returns the loss. Optional for most optimizers.
             Refer to the torch.optim.Optimizer.step() docstring for more details.
 
         """
         self.torch_optimizer.step(closure)
 
     def zero_grad(self, set_to_none: bool = True) -> None:
         """Sets the gradients of all optimized ``torch.Tensor`` to zero.
 
         Parameters
         ----------
-        set_to_none : bool,
+        set_to_none :
             Instead of setting to zero, set the grads to None.
             Refer to the torch.optim.Optimizer.zero_grad() docstring for more details.
 
         """
         self.torch_optimizer.zero_grad(set_to_none)
```

### Comparing `pypots-0.1.0/pypots/optim/rmsprop.py` & `pypots-0.1.1/pypots/optim/rmsprop.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,39 +6,39 @@
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 from typing import Iterable
 
 from torch.optim import RMSprop as torch_RMSprop
 
-from pypots.optim.base import Optimizer
+from .base import Optimizer
 
 
 class RMSprop(Optimizer):
     """The optimizer wrapper for PyTorch RMSprop.
     https://pytorch.org/docs/stable/generated/torch.optim.RMSprop.html#torch.optim.RMSprop
 
     Parameters
     ----------
-    lr : float, default=0.001
+    lr :
         The learning rate of the optimizer.
 
-    momentum : float, default=0
+    momentum :
         Momentum factor.
 
-    alpha : float, default=0.99
+    alpha :
         Smoothing constant.
 
-    eps : float, default=1e-08
+    eps :
         Term added to the denominator to improve numerical stability.
 
-    centered : bool, default=False
+    centered :
         If True, compute the centered RMSProp, the gradient is normalized by an estimation of its variance
 
-    weight_decay : float, default=0.01
+    weight_decay :
         Weight decay (L2 penalty).
 
     """
 
     def __init__(
         self,
         lr: float = 0.001,
@@ -56,16 +56,17 @@
         self.weight_decay = weight_decay
 
     def init_optimizer(self, params: Iterable) -> None:
         """Initialize the torch optimizer wrapped by this class.
 
         Parameters
         ----------
-        params : Iterable,
+        params :
             An iterable of ``torch.Tensor`` or ``dict``. Specifies what Tensors should be optimized.
+
         """
         self.torch_optimizer = torch_RMSprop(
             params=params,
             lr=self.lr,
             momentum=self.momentum,
             alpha=self.alpha,
             eps=self.eps,
```

### Comparing `pypots-0.1.0/pypots/optim/sgd.py` & `pypots-0.1.1/pypots/optim/sgd.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,36 +6,36 @@
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 from typing import Iterable
 
 from torch.optim import SGD as torch_SGD
 
-from pypots.optim.base import Optimizer
+from .base import Optimizer
 
 
 class SGD(Optimizer):
     """The optimizer wrapper for PyTorch SGD.
     https://pytorch.org/docs/stable/generated/torch.optim.SGD.html#torch.optim.SGD
 
     Parameters
     ----------
-    lr : float, default=0.001
+    lr :
         The learning rate of the optimizer.
 
-    momentum : float, default=0
+    momentum :
         Momentum factor.
 
-    weight_decay : float, default=0.01
+    weight_decay :
         Weight decay (L2 penalty).
 
-    dampening : float, default = 0
+    dampening :
         Dampening for momentum.
 
-    nesterov : bool, default=False
+    nesterov :
         Whether to enable Nesterov momentum.
 
     """
 
     def __init__(
         self,
         lr: float = 0.001,
@@ -51,16 +51,17 @@
         self.nesterov = nesterov
 
     def init_optimizer(self, params: Iterable) -> None:
         """Initialize the torch optimizer wrapped by this class.
 
         Parameters
         ----------
-        params : Iterable,
+        params :
             An iterable of ``torch.Tensor`` or ``dict``. Specifies what Tensors should be optimized.
+
         """
         self.torch_optimizer = torch_SGD(
             params=params,
             lr=self.lr,
             momentum=self.momentum,
             weight_decay=self.weight_decay,
             dampening=self.dampening,
```

### Comparing `pypots-0.1.0/pypots/utils/files.py` & `pypots-0.1.1/pypots/utils/files.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 import os
 
-from pypots.utils.logging import logger
+from .logging import logger
 
 
 def extract_parent_dir(path: str) -> str:
     """Extract the given path's parent directory.
 
     Parameters
     ----------
-    path : str,
+    path :
         The path for extracting.
 
     Returns
     -------
-    parent_dir : str
+    parent_dir :
         The path to the parent dir of the given path.
 
     """
     parent_dir = os.path.abspath(os.path.join(path, ".."))
     return parent_dir
 
 
 def create_dir_if_not_exist(path: str, is_dir: bool = True) -> None:
     """Create the given directory if it doesn't exist.
 
     Parameters
     ----------
-    path : str,
+    path :
         The path for check.
 
-    is_dir : bool,
+    is_dir :
         Whether the given path is to a directory. If `is_dir` is False, the given path is to a file or an object,
         then this file's parent directory will be checked.
 
     """
     path = extract_parent_dir(path) if not is_dir else path
     if not os.path.exists(path):
         os.makedirs(path, exist_ok=True)
```

### Comparing `pypots-0.1.0/pypots/utils/logging.py` & `pypots-0.1.1/pypots/utils/logging.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,22 +24,23 @@
         name: str = "PyPOTS running log",
         logging_level: str = "debug",
         logging_format: str = "%(asctime)s [%(levelname)s]: %(message)s",
     ):
         """
         Parameters
         ----------
-        name : str,
+        name :
             The name for the logger to be initialized.
 
-        logging_level : str,
+        logging_level :
             The logging level of the logger, should be debug/info/warning/error.
 
-        logging_format : str,
+        logging_format :
             Logging format of the logger.
+
         """
 
         assert (
             logging_level in LEVELS.keys()
         ), f"logging_level should be {list(LEVELS.keys())}, but got {logging_level}"
 
         self.logger = logging.getLogger(name)
@@ -62,21 +63,21 @@
             self.logger.addHandler(self.file_handler)
 
     def set_saving_path(self, saving_dir: str, name: str, mode: str = "a") -> None:
         """Set the logger's saving path. This function will enable saving logs to the specified path.
 
         Parameters
         ----------
-        saving_dir : str,
+        saving_dir :
             The path to the directory for logging file saving.
 
-        name : str,
+        name :
             The name of the logging file to be saved.
 
-        mode : str, default = 'a'
+        mode :
             Logging file writing mode.
 
         """
         if not os.path.exists(saving_dir):
             self.logger.warning(f"{saving_dir} does not exist. Creating it now...")
             os.makedirs(saving_dir)
         path = os.path.join(saving_dir, name)
@@ -87,15 +88,15 @@
         self.logger.info(f"Log will be saved to {path}")
 
     def set_level(self, level: str) -> None:
         """Set the logger's logging level.
 
         Parameters
         ----------
-        level : str,
+        level :
             The logging level of the logger, should be debug/info/warning/error.
 
         """
         self.logging_level = LEVELS[level]
         self.logger.setLevel(self.logging_level)
         if self.stream_handler is not None:
             self.stream_handler.setLevel(self.logging_level)
```

### Comparing `pypots-0.1.0/pypots/utils/metrics.py` & `pypots-0.1.1/pypots/utils/metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,21 +19,21 @@
 ) -> Union[float, torch.Tensor]:
     """Calculate the Mean Absolute Error between ``predictions`` and ``targets``.
     ``masks`` can be used for filtering. For values==0 in ``masks``,
     values at their corresponding positions in ``predictions`` will be ignored.
 
     Parameters
     ----------
-    predictions : Union[np.ndarray, torch.Tensor, list],
+    predictions :
         The prediction data to be evaluated.
 
-    targets : Union[np.ndarray, torch.Tensor, list],
+    targets :
         The target data for helping evaluate the predictions.
 
-    masks : Optional[Union[np.ndarray, torch.Tensor, list]], optional, default = None,
+    masks :
         The masks for filtering the specific values in inputs and target from evaluation.
         When given, only values at corresponding positions where values ==1 in ``masks`` will be used for evaluation.
 
     Examples
     --------
 
     >>> import numpy as np
@@ -74,21 +74,21 @@
 ) -> Union[float, torch.Tensor]:
     """Calculate the Mean Square Error between ``predictions`` and ``targets``.
     ``masks`` can be used for filtering. For values==0 in ``masks``,
     values at their corresponding positions in ``predictions`` will be ignored.
 
     Parameters
     ----------
-    predictions : Union[np.ndarray, torch.Tensor, list],
+    predictions :
         The prediction data to be evaluated.
 
-    targets : Union[np.ndarray, torch.Tensor, list],
+    targets :
         The target data for helping evaluate the predictions.
 
-    masks : Optional[Union[np.ndarray, torch.Tensor, list]], optional, default = None,
+    masks :
         The masks for filtering the specific values in inputs and target from evaluation.
         When given, only values at corresponding positions where values ==1 in ``masks`` will be used for evaluation.
 
     Examples
     --------
 
     >>> import numpy as np
@@ -130,21 +130,21 @@
 ) -> Union[float, torch.Tensor]:
     """Calculate the Root Mean Square Error between ``predictions`` and ``targets``.
     ``masks`` can be used for filtering. For values==0 in ``masks``,
     values at their corresponding positions in ``predictions`` will be ignored.
 
     Parameters
     ----------
-    predictions : Union[np.ndarray, torch.Tensor, list],
+    predictions :
         The prediction data to be evaluated.
 
-    targets : Union[np.ndarray, torch.Tensor, list],
+    targets :
         The target data for helping evaluate the predictions.
 
-    masks : Optional[Union[np.ndarray, torch.Tensor, list]], optional, default = None,
+    masks :
         The masks for filtering the specific values in inputs and target from evaluation.
         When given, only values at corresponding positions where values ==1 in ``masks`` will be used for evaluation.
 
     Examples
     --------
 
     >>> import numpy as np
@@ -181,21 +181,21 @@
 ) -> Union[float, torch.Tensor]:
     """Calculate the Mean Relative Error between ``predictions`` and ``targets``.
     ``masks`` can be used for filtering. For values==0 in ``masks``,
     values at their corresponding positions in ``predictions`` will be ignored.
 
     Parameters
     ----------
-    predictions : Union[np.ndarray, torch.Tensor, list],
+    predictions :
         The prediction data to be evaluated.
 
-    targets : Union[np.ndarray, torch.Tensor, list],
+    targets :
         The target data for helping evaluate the predictions.
 
-    masks : Optional[Union[np.ndarray, torch.Tensor, list]], optional, default = None,
+    masks :
         The masks for filtering the specific values in inputs and target from evaluation.
         When given, only values at corresponding positions where values ==1 in ``masks`` will be used for evaluation.
 
     Examples
     --------
 
     >>> import numpy as np
@@ -239,27 +239,27 @@
 ) -> dict:
     """Calculate the evaluation metrics for the binary classification task,
     including accuracy, precision, recall, f1 score, area under ROC curve, and area under Precision-Recall curve.
     If targets contains multiple categories, please set the positive category as `pos_label`.
 
     Parameters
     ----------
-    prob_predictions : array-like, 1d or 2d, [n_samples] or [n_samples, n_categories]
+    prob_predictions :
         Estimated probability predictions returned by a decision function.
 
-    targets : array-like, 1d or 2d, shape of [n_samples] or [n_samples, 1]
+    targets :
         Ground truth (correct) classification results.
 
-    pos_label : int, default=1
+    pos_label :
         The label of the positive class.
         Note that pos_label is also the index used to extract binary prediction probabilities from `predictions`.
 
     Returns
     -------
-    classification_metrics : dict
+    classification_metrics :
         A dictionary contains classification metrics and useful results:
 
         predictions: binary categories of the prediction results;
 
         accuracy: prediction accuracy;
 
         precision: prediction precision;
@@ -343,32 +343,32 @@
     targets: np.ndarray,
     pos_label: int = 1,
 ) -> Tuple[float, float, float]:
     """Calculate precision, recall, and F1-score of model predictions.
 
     Parameters
     ----------
-    prob_predictions : array-like, 1d or 2d, [n_samples] or [n_samples, n_categories]
+    prob_predictions :
         Estimated probability predictions returned by a decision function.
 
-    targets : array-like, 1d or 2d, shape of [n_samples] or [n_samples, 1]
+    targets :
         Ground truth (correct) classification results.
 
     pos_label: int, default=1
         The label of the positive class.
 
     Returns
     -------
-    precision : float
+    precision :
         The precision value of model predictions.
 
-    recall : float
+    recall :
         The recall value of model predictions.
 
-    f1 : float
+    f1 :
         The F1 score of model predictions.
 
     """
     precision, recall, f1, _ = metrics.precision_recall_fscore_support(
         targets, prob_predictions, pos_label=pos_label
     )
     precision, recall, f1 = precision[pos_label], recall[pos_label], f1[pos_label]
@@ -380,35 +380,35 @@
     targets: np.ndarray,
     pos_label: int = 1,
 ) -> Tuple[float, np.ndarray, np.ndarray, np.ndarray]:
     """Calculate precisions, recalls, and area under PR curve of model predictions.
 
     Parameters
     ----------
-    prob_predictions : array-like, 1d or 2d, [n_samples] or [n_samples, n_categories]
+    prob_predictions :
         Estimated probability predictions returned by a decision function.
 
-    targets : array-like, 1d or 2d, shape of [n_samples] or [n_samples, 1]
+    targets :
         Ground truth (correct) classification results.
 
     pos_label: int, default=1
         The label of the positive class.
 
     Returns
     -------
-    pr_auc : float
+    pr_auc :
         Value of area under Precision-Recall curve.
 
-    precisions : array-like
+    precisions :
         Precision values of Precision-Recall curve.
 
-    recalls : array-like
+    recalls :
         Recall values of Precision-Recall curve.
 
-    thresholds : array-like
+    thresholds :
         Increasing thresholds on the decision function used to compute precision and recall.
 
     """
 
     precisions, recalls, thresholds = metrics.precision_recall_curve(
         targets, prob_predictions, pos_label=pos_label
     )
@@ -421,35 +421,35 @@
     targets: np.ndarray,
     pos_label: int = 1,
 ) -> Tuple[float, np.ndarray, np.ndarray, np.ndarray]:
     """Calculate false positive rates, true positive rates, and area under AUC curve of model predictions.
 
     Parameters
     ----------
-    prob_predictions : array-like, 1d, [n_samples]
+    prob_predictions :
         Estimated probabilities/predictions returned by a decision function.
 
-    targets : array-like, 1d or 2d, shape of [n_samples] or [n_samples, 1]
+    targets :
         Ground truth (correct) classification results.
 
     pos_label: int, default=1
         The label of the positive class.
 
     Returns
     -------
-    roc_auc : float
+    roc_auc :
         The area under ROC curve.
 
-    fprs : array-like
+    fprs :
         False positive rates of ROC curve.
 
-    tprs : array-like
+    tprs :
         True positive rates of ROC curve.
 
-    thresholds : array-like
+    thresholds :
         Increasing thresholds on the decision function used to compute FPR and TPR.
 
     """
     fprs, tprs, thresholds = metrics.roc_curve(
         y_true=targets, y_score=prob_predictions, pos_label=pos_label
     )
     roc_auc = metrics.auc(fprs, tprs)
@@ -457,23 +457,23 @@
 
 
 def cal_acc(class_predictions: np.ndarray, targets: np.ndarray) -> float:
     """Calculate accuracy score of model predictions.
 
     Parameters
     ----------
-    class_predictions : array-like, 1d or 2d, [n_samples] or [n_samples, n_categories]
+    class_predictions :
         Estimated classification predictions returned by a classifier.
 
-    targets : array-like, 1d or 2d, shape of [n_samples] or [n_samples, 1]
+    targets :
         Ground truth (correct) classification results.
 
     Returns
     -------
-    acc_score : float
+    acc_score :
         The accuracy of model predictions.
 
     """
     acc_score = metrics.accuracy_score(targets, class_predictions)
     return acc_score
 
 
@@ -482,23 +482,23 @@
     targets: np.ndarray,
 ) -> float:
     """Calculate Rand Index, a measure of the similarity between two data clusterings.
     Refer to :cite:`rand1971RandIndex`.
 
     Parameters
     ----------
-    class_predictions : array
+    class_predictions :
         Clustering results returned by a clusterer.
 
-    targets : array
+    targets :
         Ground truth (correct) clustering results.
 
     Returns
     -------
-    RI : float
+    RI :
         Rand index.
 
     """
     # # detailed implementation
     # n = len(targets)
     # TP = 0
     # TN = 0
@@ -523,23 +523,23 @@
     class_predictions: np.ndarray,
     targets: np.ndarray,
 ) -> float:
     """Calculate adjusted Rand Index. Refer to :cite:`hubert1985AdjustedRI`.
 
     Parameters
     ----------
-    class_predictions : array
+    class_predictions :
         Clustering results returned by a clusterer.
 
-    targets : array
+    targets :
         Ground truth (correct) clustering results.
 
     Returns
     -------
-    aRI : float
+    aRI :
         Adjusted Rand index.
 
     """
     aRI = metrics.adjusted_rand_score(targets, class_predictions)
     return aRI
 
 
@@ -547,23 +547,23 @@
     class_predictions: np.ndarray,
     targets: np.ndarray,
 ) -> float:
     """Calculate cluster purity.
 
     Parameters
     ----------
-    class_predictions : array
+    class_predictions :
         Clustering results returned by a clusterer.
 
-    targets : array
+    targets :
         Ground truth (correct) clustering results.
 
     Returns
     -------
-    cluster_purity : float
+    cluster_purity :
         cluster purity.
 
     Notes
     -----
     This function is from the answer https://stackoverflow.com/a/51672699 on StackOverflow.
 
     """
```

### Comparing `pypots-0.1.0/pypots/utils/random.py` & `pypots-0.1.1/pypots/utils/random.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 """
 
 # Created by Wenjie Du <wenjay.du@gmail.com>
 # License: GLP-v3
 
 import numpy as np
 import torch
-from pypots.utils.logging import logger
+from .logging import logger
 
 RANDOM_SEED = 2204
 
 
 def set_random_seed(random_seed: int = RANDOM_SEED) -> None:
     """Manually set the random state to make PyPOTS output reproducible results.
 
     Parameters
     ----------
-    random_seed : int, default = RANDOM_SEED,
+    random_seed :
         The seed to be set for generating random numbers in PyPOTS.
 
     """
 
     np.random.seed(RANDOM_SEED)
     torch.manual_seed(random_seed)
     logger.info(
```

### Comparing `pypots-0.1.0/pypots.egg-info/PKG-INFO` & `pypots-0.1.1/pypots.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 Metadata-Version: 2.1
 Name: pypots
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python Toolbox for Data Mining on Partially-Observed Time Series
-Home-page: https://github.com/WenjieDu/PyPOTS
-Download-URL: https://github.com/WenjieDu/PyPOTS/archive/main.zip
+Home-page: https://pypots.com/
 Author: Wenjie Du
 Author-email: wenjay.du@gmail.com
 License: GPL-3.0
+Project-URL: Documentation, https://docs.pypots.com/
+Project-URL: Source, https://github.com/WenjieDu/PyPOTS/
+Project-URL: Tracker, https://github.com/WenjieDu/PyPOTS/issues/
+Project-URL: Download, https://github.com/WenjieDu/PyPOTS/archive/main.zip
 Keywords: data mining,neural networks,machine learning,deep learning,artificial intelligence,time-series analysis,time series,imputation,classification,clustering,forecasting,partially observed,irregular sampled,partially-observed time series,incomplete time series,missing data,missing values
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -133,16 +136,18 @@
 ## ❖ Usage
 <a href="https://github.com/WenjieDu/BrewPOTS">
     <img src="https://raw.githubusercontent.com/WenjieDu/BrewPOTS/main/figs/BrewPOTS_logo.jpg" align="left" width="160" alt="BrewPOTS logo"/>
 </a>
 
 PyPOTS tutorials have been released. Considering the future workload, I separate the tutorials into a single repo,
 and you can find them in [BrewPOTS](https://github.com/WenjieDu/BrewPOTS).
-Take a look at it now, and brew your POTS dataset into a cup of coffee! 🤓
+Take a look at it now, and learn how to brew your POTS datasets! 🤓
 
+You can also find a simple and quick-start tutorial notebook on Google Colab with
+[this link](https://colab.research.google.com/drive/1HEFjylEy05-r47jRy0H9jiS_WhD0UWmQ?usp=sharing).
 If you have further questions, please refer to PyPOTS documentation 📑[docs.pypots.com](https://docs.pypots.com).
 Besides, you can also [raise an issue](https://github.com/WenjieDu/PyPOTS/issues) or [ask in our community](#-community).
 
 We present you a usage example of imputing missing values in time series with PyPOTS below, you can click it to view.
 
 <details>
 <summary><b>Click here to see an example applying SAITS on PhysioNet2012 for imputation:</b></summary>
@@ -172,33 +177,34 @@
 ```
 </details>
 
 
 ## ❖ Available Algorithms
 PyPOTS supports imputation, classification, clustering, and forecasting tasks on multivariate time series with missing values. The currently available algorithms of four tasks are cataloged in the following table with four partitions. The paper references are all listed at the bottom of this readme file. Please refer to them if you want more details.
 
-|   ***`Imputation`***   |      🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|:----------------------:|:------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------:|
-|        **Type**        |  **Abbr.**   |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|       Neural Net       |    SAITS     |                                                               Self-Attention-based Imputation for Time Series [^1]                                                                |   2023   |
-|       Neural Net       | Transformer  | Attention is All you Need [^2];<br>Self-Attention-based Imputation for Time Series [^1];<br><sub>Note: proposed in [^2], and re-implemented as an imputation model in [^1].</sub> |   2017   |
-|       Neural Net       |    BRITS     |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
-|         Naive          |     LOCF     |                                                                         Last Observation Carried Forward                                                                          |    -     |
-| ***`Classification`*** |      🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**   |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|       Neural Net       |    BRITS     |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
-|       Neural Net       |    GRU-D     |                                                  Recurrent Neural Networks for Multivariate Time Series with Missing Values [^4]                                                  |   2018   |
-|       Neural Net       |   Raindrop   |                                                    Graph-Guided Network for Irregularly Sampled Multivariate Time Series [^5]                                                     |   2022   |
-|   ***`Clustering`***   |      🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**   |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|       Neural Net       |     CRLI     |                                                      Clustering Representation Learning on Incomplete time-series data [^6]                                                       |   2021   |
-|       Neural Net       |    VaDER     |                                                                  Variational Deep Embedding with Recurrence [^7]                                                                  |   2019   |
-|  ***`Forecasting`***   |      🚥      |                                                                                        🚥                                                                                         |    🚥    |
-|        **Type**        |  **Abbr.**   |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
-|     Probabilistic      |     BTTF     |                                                                    Bayesian Temporal Tensor Factorization [^8]                                                                    |   2021   |
+|   ***`Imputation`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
+|:----------------------:|:-----------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------:|
+|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
+|       Neural Net       |    SAITS    |                                                               Self-Attention-based Imputation for Time Series [^1]                                                                |   2023   |
+|       Neural Net       | Transformer | Attention is All you Need [^2];<br>Self-Attention-based Imputation for Time Series [^1];<br><sub>Note: proposed in [^2], and re-implemented as an imputation model in [^1].</sub> |   2017   |
+|       Neural Net       |    BRITS    |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
+|       Neural Net       |    M-RNN    |                                                                  Multi-directional Recurrent Neural Network [^9]                                                                  |   2019   |
+|         Naive          |    LOCF     |                                                                         Last Observation Carried Forward                                                                          |    -     |
+| ***`Classification`*** |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
+|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
+|       Neural Net       |    BRITS    |                                                              Bidirectional Recurrent Imputation for Time Series [^3]                                                              |   2018   |
+|       Neural Net       |    GRU-D    |                                                  Recurrent Neural Networks for Multivariate Time Series with Missing Values [^4]                                                  |   2018   |
+|       Neural Net       |  Raindrop   |                                                    Graph-Guided Network for Irregularly Sampled Multivariate Time Series [^5]                                                     |   2022   |
+|   ***`Clustering`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
+|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
+|       Neural Net       |    CRLI     |                                                      Clustering Representation Learning on Incomplete time-series data [^6]                                                       |   2021   |
+|       Neural Net       |    VaDER    |                                                                  Variational Deep Embedding with Recurrence [^7]                                                                  |   2019   |
+|  ***`Forecasting`***   |     🚥      |                                                                                        🚥                                                                                         |    🚥    |
+|        **Type**        |  **Abbr.**  |                                                                    **Full name of the algorithm/model/paper**                                                                     | **Year** |
+|     Probabilistic      |    BTTF     |                                                                    Bayesian Temporal Tensor Factorization [^8]                                                                    |   2021   |
 
 
 ## ❖ Citing PyPOTS
 We are pursuing to publish a short paper introducing PyPOTS in prestigious academic venues, e.g. JMLR (track for
 [Machine Learning Open Source Software](https://www.jmlr.org/mloss/)). Before that, PyPOTS is using its DOI from Zenodo
 for reference. If you use PyPOTS in your research, please cite it as below and 🌟star this repository to make others
 notice this work. 🤗
@@ -224,15 +230,17 @@
 ## ❖ Contribution
 You're very welcome to contribute to this exciting project!
 
 By committing your code, you'll
 
 1. make your well-established model out-of-the-box for PyPOTS users to run,
    and help your work obtain more exposure and impact.
-   Take a look at our [inclusion criteria](https://docs.pypots.com/en/latest/faq.html#inclusion-criteria);
+   Take a look at our [inclusion criteria](https://docs.pypots.com/en/latest/faq.html#inclusion-criteria).
+   You can utilize the `template` folder in each task package (e.g.
+   [pypots/imputation/template](https://github.com/WenjieDu/PyPOTS/tree/main/pypots/imputation/template)) to quickly start;
 2. be listed as one of [PyPOTS contributors](https://github.com/WenjieDu/PyPOTS/graphs/contributors):
    <img align="center" src="https://contrib.rocks/image?repo=wenjiedu/pypots">;
 3. get mentioned in our [release notes](https://github.com/WenjieDu/PyPOTS/releases);
 
 You can also contribute to PyPOTS by simply staring🌟 this repo to help more people notice it.
 Your star is your recognition to PyPOTS, and it matters!
 
@@ -254,15 +262,15 @@
 
 
 ## ❖ Community
 We care about the feedback from our users, so we're building PyPOTS community on
 
 - [Slack](https://pypots-org.slack.com). General discussion, Q&A, and our development team are here;
 - [LinkedIn](https://www.linkedin.com/company/pypots). Official announcements and news are here;
-- [WeChat (微信公众号)](https://mp.weixin.qq.com/s/m6j83SJNgz-xySSZd-DTBw). We also run a group chat on WeChat,
+- [WeChat (微信公众号)](https://mp.weixin.qq.com/s/sNgZmgAyxDn2sZxXoWJYMA). We also run a group chat on WeChat,
   and you can get the QR code from the official account after following it;
 
 If you have any suggestions or want to contribute ideas or share time-series related papers, join us and tell.
 PyPOTS community is open, transparent, and surely friendly. Let's work together to build and improve PyPOTS 💪!
 
 
 ## ❖ Attention 👀
@@ -278,14 +286,16 @@
 [^2]: Vaswani, A., Shazeer, N.M., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A.N., Kaiser, L., & Polosukhin, I. (2017). [Attention is All you Need](https://papers.nips.cc/paper/2017/hash/3f5ee243547dee91fbd053c1c4a845aa-Abstract.html). *NeurIPS 2017*.
 [^3]: Cao, W., Wang, D., Li, J., Zhou, H., Li, L., & Li, Y. (2018). [BRITS: Bidirectional Recurrent Imputation for Time Series](https://papers.nips.cc/paper/2018/hash/734e6bfcd358e25ac1db0a4241b95651-Abstract.html). *NeurIPS 2018*.
 [^4]: Che, Z., Purushotham, S., Cho, K., Sontag, D.A., & Liu, Y. (2018). [Recurrent Neural Networks for Multivariate Time Series with Missing Values](https://www.nature.com/articles/s41598-018-24271-9). *Scientific Reports*.
 [^5]: Zhang, X., Zeman, M., Tsiligkaridis, T., & Zitnik, M. (2022). [Graph-Guided Network for Irregularly Sampled Multivariate Time Series](https://arxiv.org/abs/2110.05357). *ICLR 2022*.
 [^6]: Ma, Q., Chen, C., Li, S., & Cottrell, G. W. (2021). [Learning Representations for Incomplete Time Series Clustering](https://ojs.aaai.org/index.php/AAAI/article/view/17070). *AAAI 2021*.
 [^7]: Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P., Ahmad, A., Vrooman, H.A., Hofmann-Apitius, M., & Fröhlich, H. (2019). [Deep learning for clustering of multivariate clinical patient trajectories with missing values](https://academic.oup.com/gigascience/article/8/11/giz134/5626377). *GigaScience*.
 [^8]: Chen, X., & Sun, L. (2021). [Bayesian Temporal Factorization for Multidimensional Time Series Prediction](https://arxiv.org/abs/1910.06366). *IEEE transactions on pattern analysis and machine intelligence*.
+[^9]: Yoon, J., Zame, W. R., & van der Schaar, M. (2019). [Estimating Missing Data in Temporal Data Streams Using Multi-Directional Recurrent Neural Networks](https://ieeexplore.ieee.org/document/8485748). *IEEE Transactions on Biomedical Engineering*.
+
 
 <details>
 <summary>🏠 Visits</summary>
 <a href="https://github.com/WenjieDu/PyPOTS">
     <img alt="PyPOTS visits" align="left" src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FPyPOTS%2FPyPOTS&count_bg=%23009A0A&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Hits&edge_flat=false">
 </a>
 </details>
```

#### html2text {}

```diff
@@ -1,13 +1,15 @@
-Metadata-Version: 2.1 Name: pypots Version: 0.1.0 Summary: A Python Toolbox for
-Data Mining on Partially-Observed Time Series Home-page: https://github.com/
-WenjieDu/PyPOTS Download-URL: https://github.com/WenjieDu/PyPOTS/archive/
-main.zip Author: Wenjie Du Author-email: wenjay.du@gmail.com License: GPL-3.0
-Keywords: data mining,neural networks,machine learning,deep learning,artificial
-intelligence,time-series analysis,time
+Metadata-Version: 2.1 Name: pypots Version: 0.1.1 Summary: A Python Toolbox for
+Data Mining on Partially-Observed Time Series Home-page: https://pypots.com/
+Author: Wenjie Du Author-email: wenjay.du@gmail.com License: GPL-3.0 Project-
+URL: Documentation, https://docs.pypots.com/ Project-URL: Source, https://
+github.com/WenjieDu/PyPOTS/ Project-URL: Tracker, https://github.com/WenjieDu/
+PyPOTS/issues/ Project-URL: Download, https://github.com/WenjieDu/PyPOTS/
+archive/main.zip Keywords: data mining,neural networks,machine learning,deep
+learning,artificial intelligence,time-series analysis,time
 series,imputation,classification,clustering,forecasting,partially
 observed,irregular sampled,partially-observed time series,incomplete time
 series,missing data,missing values Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Education Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: Operating System :: OS Independent Classifier: Programming
@@ -59,55 +61,59 @@
 version # by conda conda install -c conda-forge pypots # the first time
 installation conda update -c conda-forge pypots # update pypots to the latest
 version ```` Alternatively, you can install from the latest source code with
 the latest features but may be not officially released yet: > pip install
 https://github.com/WenjieDu/PyPOTS/archive/main.zip ## â Usage [BrewPOTS
 logo] PyPOTS tutorials have been released. Considering the future workload, I
 separate the tutorials into a single repo, and you can find them in [BrewPOTS]
-(https://github.com/WenjieDu/BrewPOTS). Take a look at it now, and brew your
-POTS dataset into a cup of coffee! ð¤ If you have further questions, please
-refer to PyPOTS documentation ð[docs.pypots.com](https://docs.pypots.com).
-Besides, you can also [raise an issue](https://github.com/WenjieDu/PyPOTS/
-issues) or [ask in our community](#-community). We present you a usage example
-of imputing missing values in time series with PyPOTS below, you can click it
-to view.  Click here to see an example applying SAITS on PhysioNet2012 for
-imputation: ``` python import numpy as np from sklearn.preprocessing import
-StandardScaler from pypots.data import load_specific_dataset, mcar, masked_fill
-from pypots.imputation import SAITS from pypots.utils.metrics import cal_mae #
-Data preprocessing. Tedious, but PyPOTS can help. ð¤ data =
-load_specific_dataset('physionet_2012') # PyPOTS will automatically download
-and extract it. X = data['X'] num_samples = len(X['RecordID'].unique()) X =
-X.drop(['RecordID', 'Time'], axis = 1) X = StandardScaler().fit_transform
-(X.to_numpy()) X = X.reshape(num_samples, 48, -1) X_intact, X, missing_mask,
-indicating_mask = mcar(X, 0.1) # hold out 10% observed values as ground truth X
-= masked_fill(X, 1 - missing_mask, np.nan) dataset = {"X": X} print(dataset
-["X"].shape) # (11988, 48, 37), 11988 samples, 48 time steps, 37 features #
-Model training. This is PyPOTS showtime. ðª saits = SAITS(n_steps=48,
-n_features=37, n_layers=2, d_model=256, d_inner=128, n_head=4, d_k=64, d_v=64,
-dropout=0.1, epochs=10) saits.fit(dataset) # train the model. Here I use the
-whole dataset as the training set, because ground truth is not visible to the
-model. imputation = saits.impute(dataset) # impute the originally-missing
-values and artificially-missing values mae = cal_mae(imputation, X_intact,
-indicating_mask) # calculate mean absolute error on the ground truth
-(artificially-missing values) ```  ## â Available Algorithms PyPOTS supports
-imputation, classification, clustering, and forecasting tasks on multivariate
-time series with missing values. The currently available algorithms of four
-tasks are cataloged in the following table with four partitions. The paper
-references are all listed at the bottom of this readme file. Please refer to
-them if you want more details. | ***`Imputation`*** | ð¥ | ð¥ | ð¥ | |:--
---------------------:|:------------:|:-----------------------------------------
+(https://github.com/WenjieDu/BrewPOTS). Take a look at it now, and learn how to
+brew your POTS datasets! ð¤ You can also find a simple and quick-start
+tutorial notebook on Google Colab with [this link](https://
+colab.research.google.com/drive/1HEFjylEy05-r47jRy0H9jiS_WhD0UWmQ?usp=sharing).
+If you have further questions, please refer to PyPOTS documentation ð
+[docs.pypots.com](https://docs.pypots.com). Besides, you can also [raise an
+issue](https://github.com/WenjieDu/PyPOTS/issues) or [ask in our community](#-
+community). We present you a usage example of imputing missing values in time
+series with PyPOTS below, you can click it to view.  Click here to see an
+example applying SAITS on PhysioNet2012 for imputation: ``` python import numpy
+as np from sklearn.preprocessing import StandardScaler from pypots.data import
+load_specific_dataset, mcar, masked_fill from pypots.imputation import SAITS
+from pypots.utils.metrics import cal_mae # Data preprocessing. Tedious, but
+PyPOTS can help. ð¤ data = load_specific_dataset('physionet_2012') # PyPOTS
+will automatically download and extract it. X = data['X'] num_samples = len(X
+['RecordID'].unique()) X = X.drop(['RecordID', 'Time'], axis = 1) X =
+StandardScaler().fit_transform(X.to_numpy()) X = X.reshape(num_samples, 48, -1)
+X_intact, X, missing_mask, indicating_mask = mcar(X, 0.1) # hold out 10%
+observed values as ground truth X = masked_fill(X, 1 - missing_mask, np.nan)
+dataset = {"X": X} print(dataset["X"].shape) # (11988, 48, 37), 11988 samples,
+48 time steps, 37 features # Model training. This is PyPOTS showtime. ðª
+saits = SAITS(n_steps=48, n_features=37, n_layers=2, d_model=256, d_inner=128,
+n_head=4, d_k=64, d_v=64, dropout=0.1, epochs=10) saits.fit(dataset) # train
+the model. Here I use the whole dataset as the training set, because ground
+truth is not visible to the model. imputation = saits.impute(dataset) # impute
+the originally-missing values and artificially-missing values mae = cal_mae
+(imputation, X_intact, indicating_mask) # calculate mean absolute error on the
+ground truth (artificially-missing values) ```  ## â Available Algorithms
+PyPOTS supports imputation, classification, clustering, and forecasting tasks
+on multivariate time series with missing values. The currently available
+algorithms of four tasks are cataloged in the following table with four
+partitions. The paper references are all listed at the bottom of this readme
+file. Please refer to them if you want more details. | ***`Imputation`*** |
+ð¥ | ð¥ | ð¥ | |:----------------------:|:-----------:|:-----------------
 -------------------------------------------------------------------------------
----------------------------------------------------------:|:--------:| |
-**Type** | **Abbr.** | **Full name of the algorithm/model/paper** | **Year** |
-| Neural Net | SAITS | Self-Attention-based Imputation for Time Series [^1] |
-2023 | | Neural Net | Transformer | Attention is All you Need [^2];
+-------------------------------------------------------------------------------
+--:|:--------:| | **Type** | **Abbr.** | **Full name of the algorithm/model/
+paper** | **Year** | | Neural Net | SAITS | Self-Attention-based Imputation for
+Time Series [^1] | 2023 | | Neural Net | Transformer | Attention is All you
+Need [^2];
 Self-Attention-based Imputation for Time Series [^1];
 Note: proposed in [^2], and re-implemented as an imputation model in [^1]. |
 2017 | | Neural Net | BRITS | Bidirectional Recurrent Imputation for Time
-Series [^3] | 2018 | | Naive | LOCF | Last Observation Carried Forward | - | |
+Series [^3] | 2018 | | Neural Net | M-RNN | Multi-directional Recurrent Neural
+Network [^9] | 2019 | | Naive | LOCF | Last Observation Carried Forward | - | |
 ***`Classification`*** | ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full
 name of the algorithm/model/paper** | **Year** | | Neural Net | BRITS |
 Bidirectional Recurrent Imputation for Time Series [^3] | 2018 | | Neural Net |
 GRU-D | Recurrent Neural Networks for Multivariate Time Series with Missing
 Values [^4] | 2018 | | Neural Net | Raindrop | Graph-Guided Network for
 Irregularly Sampled Multivariate Time Series [^5] | 2022 | | ***`Clustering`***
 | ð¥ | ð¥ | ð¥ | | **Type** | **Abbr.** | **Full name of the algorithm/
@@ -127,28 +133,31 @@
 WenjieDu/PyPOTS}}, url = {\url{https://github.com/WenjieDu/PyPOTS}}, doi =
 {10.5281/zenodo.6823221}, } ``` or > Wenjie Du. (2022). > PyPOTS: A Python
 Toolbox for Data Mining on Partially-Observed Time Series. > Zenodo. https://
 doi.org/10.5281/zenodo.6823221 ## â Contribution You're very welcome to
 contribute to this exciting project! By committing your code, you'll 1. make
 your well-established model out-of-the-box for PyPOTS users to run, and help
 your work obtain more exposure and impact. Take a look at our [inclusion
-criteria](https://docs.pypots.com/en/latest/faq.html#inclusion-criteria); 2. be
-listed as one of [PyPOTS contributors](https://github.com/WenjieDu/PyPOTS/
-graphs/contributors): [https://contrib.rocks/image?repo=wenjiedu/pypots]; 3.
-get mentioned in our [release notes](https://github.com/WenjieDu/PyPOTS/
-releases); You can also contribute to PyPOTS by simply staringð this repo to
-help more people notice it. Your star is your recognition to PyPOTS, and it
-matters!   ð Click here to view PyPOTS stargazers and forkers.
+criteria](https://docs.pypots.com/en/latest/faq.html#inclusion-criteria). You
+can utilize the `template` folder in each task package (e.g. [pypots/
+imputation/template](https://github.com/WenjieDu/PyPOTS/tree/main/pypots/
+imputation/template)) to quickly start; 2. be listed as one of [PyPOTS
+contributors](https://github.com/WenjieDu/PyPOTS/graphs/contributors): [https:/
+/contrib.rocks/image?repo=wenjiedu/pypots]; 3. get mentioned in our [release
+notes](https://github.com/WenjieDu/PyPOTS/releases); You can also contribute to
+PyPOTS by simply staringð this repo to help more people notice it. Your star
+is your recognition to PyPOTS, and it matters!   ð Click here to view PyPOTS
+stargazers and forkers.
 We're so proud to have more and more awesome users, as well as more bright
 â¨stars:  [PyPOTS_stargazers]
 [PyPOTS_forkers]  ## â Community We care about the feedback from our users,
 so we're building PyPOTS community on - [Slack](https://pypots-org.slack.com).
 General discussion, Q&A, and our development team are here; - [LinkedIn](https:
 //www.linkedin.com/company/pypots). Official announcements and news are here; -
-[WeChat (å¾®ä¿¡å¬ä¼å·)](https://mp.weixin.qq.com/s/m6j83SJNgz-xySSZd-DTBw).
+[WeChat (å¾®ä¿¡å¬ä¼å·)](https://mp.weixin.qq.com/s/sNgZmgAyxDn2sZxXoWJYMA).
 We also run a group chat on WeChat, and you can get the QR code from the
 official account after following it; If you have any suggestions or want to
 contribute ideas or share time-series related papers, join us and tell. PyPOTS
 community is open, transparent, and surely friendly. Let's work together to
 build and improve PyPOTS ðª! ## â Attention ð â¼ï¸ PyPOTS is currently
 under developing. If you like it and look forward to its growth, please give
 PyPOTS a star and watch it to keep you posted on its progress and to let me
@@ -175,8 +184,11 @@
 2021*. [^7]: Jong, J.D., Emon, M.A., Wu, P., Karki, R., Sood, M., Godard, P.,
 Ahmad, A., Vrooman, H.A., Hofmann-Apitius, M., & FrÃ¶hlich, H. (2019). [Deep
 learning for clustering of multivariate clinical patient trajectories with
 missing values](https://academic.oup.com/gigascience/article/8/11/giz134/
 5626377). *GigaScience*. [^8]: Chen, X., & Sun, L. (2021). [Bayesian Temporal
 Factorization for Multidimensional Time Series Prediction](https://arxiv.org/
 abs/1910.06366). *IEEE transactions on pattern analysis and machine
-intelligence*.  ð  Visits [PyPOTS_visits]
+intelligence*. [^9]: Yoon, J., Zame, W. R., & van der Schaar, M. (2019).
+[Estimating Missing Data in Temporal Data Streams Using Multi-Directional
+Recurrent Neural Networks](https://ieeexplore.ieee.org/document/8485748). *IEEE
+Transactions on Biomedical Engineering*.  ð  Visits [PyPOTS_visits]
```

### Comparing `pypots-0.1.0/pypots.egg-info/SOURCES.txt` & `pypots-0.1.1/pypots.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -55,22 +55,27 @@
 pypots/imputation/base.py
 pypots/imputation/brits/__init__.py
 pypots/imputation/brits/data.py
 pypots/imputation/brits/model.py
 pypots/imputation/brits/modules.py
 pypots/imputation/locf/__init__.py
 pypots/imputation/locf/model.py
+pypots/imputation/mrnn/__init__.py
+pypots/imputation/mrnn/data.py
+pypots/imputation/mrnn/model.py
+pypots/imputation/mrnn/module.py
 pypots/imputation/saits/__init__.py
 pypots/imputation/saits/data.py
 pypots/imputation/saits/model.py
 pypots/imputation/transformer/__init__.py
 pypots/imputation/transformer/data.py
 pypots/imputation/transformer/model.py
 pypots/imputation/transformer/modules.py
 pypots/optim/__init__.py
+pypots/optim/adadelta.py
 pypots/optim/adagrad.py
 pypots/optim/adam.py
 pypots/optim/adamw.py
 pypots/optim/base.py
 pypots/optim/rmsprop.py
 pypots/optim/sgd.py
 pypots/utils/__init__.py
```

### Comparing `pypots-0.1.0/setup.py` & `pypots-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,16 +11,21 @@
     version=__version__,
     description="A Python Toolbox for Data Mining on Partially-Observed Time Series",
     long_description=README,
     long_description_content_type="text/markdown",
     license="GPL-3.0",
     author="Wenjie Du",
     author_email="wenjay.du@gmail.com",
-    url="https://github.com/WenjieDu/PyPOTS",
-    download_url="https://github.com/WenjieDu/PyPOTS/archive/main.zip",
+    url="https://pypots.com/",
+    project_urls={
+        "Documentation": "https://docs.pypots.com/",
+        "Source": "https://github.com/WenjieDu/PyPOTS/",
+        "Tracker": "https://github.com/WenjieDu/PyPOTS/issues/",
+        "Download": "https://github.com/WenjieDu/PyPOTS/archive/main.zip",
+    },
     keywords=[
         "data mining",
         "neural networks",
         "machine learning",
         "deep learning",
         "artificial intelligence",
         "time-series analysis",
```

