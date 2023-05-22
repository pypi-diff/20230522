# Comparing `tmp/transphone-1.5.0.tar.gz` & `tmp/transphone-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transphone-1.5.0.tar", last modified: Fri May 19 07:10:16 2023, max compression
+gzip compressed data, was "dist/transphone-1.5.1.tar", last modified: Mon May 22 17:14:33 2023, max compression
```

## Comparing `transphone-1.5.0.tar` & `transphone-1.5.1.tar`

### file list

```diff
@@ -1,66 +1,68 @@
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1072 2022-10-27 20:49:08.000000 transphone-1.5.0/LICENSE
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-19 07:10:15.000000 transphone-1.5.0/PKG-INFO
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8168 2023-05-15 07:50:03.000000 transphone-1.5.0/README.md
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       38 2023-05-19 07:10:15.000000 transphone-1.5.0/setup.cfg
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      387 2023-05-19 07:10:11.000000 transphone-1.5.0/setup.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/test/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2730 2023-05-08 16:31:27.000000 transphone-1.5.0/test/test_tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       47 2022-11-23 17:53:06.000000 transphone-1.5.0/transphone/__init__.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/bin/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:22.000000 transphone-1.5.0/transphone/bin/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1545 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/download_model.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3451 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/eval_epitran.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3551 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/eval_g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3634 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/eval_zsl_g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2844 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2679 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/tokenize.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3816 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/train_g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1618 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/bin/update_model.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      325 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/config.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/data/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:30.000000 transphone-1.5.0/transphone/data/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9371 2023-05-19 07:10:11.000000 transphone-1.5.0/transphone/g2p.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/lang/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.0/transphone/lang/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2128 2023-05-19 07:10:11.000000 transphone-1.5.0/transphone/lang/base_tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/lang/cmn/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.0/transphone/lang/cmn/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    55821 2022-11-24 02:03:19.000000 transphone-1.5.0/transphone/lang/cmn/normalizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1750 2023-05-15 07:50:03.000000 transphone-1.5.0/transphone/lang/cmn/tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/lang/eng/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.0/transphone/lang/eng/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3341 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/lang/eng/normalizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2284 2023-05-19 07:10:11.000000 transphone-1.5.0/transphone/lang/eng/tokenizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9371 2023-05-15 13:58:49.000000 transphone-1.5.0/transphone/lang/epitran_tokenizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1826 2023-05-19 07:10:11.000000 transphone-1.5.0/transphone/lang/g2p_tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/lang/jpn/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.0/transphone/lang/jpn/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9740 2022-11-25 20:08:08.000000 transphone-1.5.0/transphone/lang/jpn/conv_table.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    15327 2022-11-25 20:04:35.000000 transphone-1.5.0/transphone/lang/jpn/jaconv.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9520 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/lang/jpn/kana2phoneme.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5192 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/lang/jpn/normalizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2775 2023-05-15 07:50:03.000000 transphone-1.5.0/transphone/lang/jpn/tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/model/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:35.000000 transphone-1.5.0/transphone/model/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    13693 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/checkpoint_utils.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6628 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/dataset.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5388 2022-03-13 19:18:49.000000 transphone-1.5.0/transphone/model/ensemble.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1782 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/grapheme.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      409 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/loader.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8331 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/lstm.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7420 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/transformer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1722 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/utils.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1046 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/model/vocab.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone/pretrained/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 18:28:14.000000 transphone-1.5.0/transphone/pretrained/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2536 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/run.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1350 2023-05-15 07:50:03.000000 transphone-1.5.0/transphone/tokenizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      491 2023-05-08 16:31:27.000000 transphone-1.5.0/transphone/utils.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone.egg-info/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone.egg-info/PKG-INFO
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1478 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone.egg-info/SOURCES.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        1 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone.egg-info/dependency_links.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      111 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone.egg-info/requires.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       11 2023-05-19 07:10:15.000000 transphone-1.5.0/transphone.egg-info/top_level.txt
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1072 2022-10-27 20:49:08.000000 transphone-1.5.1/LICENSE
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-22 17:14:33.000000 transphone-1.5.1/PKG-INFO
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8168 2023-05-15 07:50:03.000000 transphone-1.5.1/README.md
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       38 2023-05-22 17:14:33.000000 transphone-1.5.1/setup.cfg
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      387 2023-05-22 17:14:30.000000 transphone-1.5.1/setup.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/test/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2730 2023-05-08 16:31:27.000000 transphone-1.5.1/test/test_tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       47 2022-11-23 17:53:06.000000 transphone-1.5.1/transphone/__init__.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/bin/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:22.000000 transphone-1.5.1/transphone/bin/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1545 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/download_model.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3451 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/eval_epitran.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3551 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/eval_g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3634 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/eval_zsl_g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2844 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2679 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/tokenize.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3816 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/train_g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1618 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/update_model.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      325 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/config.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/data/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:30.000000 transphone-1.5.1/transphone/data/__init__.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/data/exp/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       86 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/data/exp/042801_base.yml
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9371 2023-05-19 07:10:11.000000 transphone-1.5.1/transphone/g2p.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/lang/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.1/transphone/lang/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2128 2023-05-19 07:10:11.000000 transphone-1.5.1/transphone/lang/base_tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/lang/cmn/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.1/transphone/lang/cmn/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    55821 2022-11-24 02:03:19.000000 transphone-1.5.1/transphone/lang/cmn/normalizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1750 2023-05-15 07:50:03.000000 transphone-1.5.1/transphone/lang/cmn/tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/lang/eng/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.1/transphone/lang/eng/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3341 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/lang/eng/normalizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2284 2023-05-19 07:10:11.000000 transphone-1.5.1/transphone/lang/eng/tokenizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9371 2023-05-15 13:58:49.000000 transphone-1.5.1/transphone/lang/epitran_tokenizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1826 2023-05-19 07:10:11.000000 transphone-1.5.1/transphone/lang/g2p_tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/lang/jpn/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.1/transphone/lang/jpn/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9740 2022-11-25 20:08:08.000000 transphone-1.5.1/transphone/lang/jpn/conv_table.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    15327 2022-11-25 20:04:35.000000 transphone-1.5.1/transphone/lang/jpn/jaconv.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9520 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/lang/jpn/kana2phoneme.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5192 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/lang/jpn/normalizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2775 2023-05-15 07:50:03.000000 transphone-1.5.1/transphone/lang/jpn/tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/model/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:35.000000 transphone-1.5.1/transphone/model/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    13693 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/checkpoint_utils.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6628 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/dataset.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5388 2022-03-13 19:18:49.000000 transphone-1.5.1/transphone/model/ensemble.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1782 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/grapheme.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      409 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/loader.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8331 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/lstm.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7420 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/transformer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1722 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/utils.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1046 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/vocab.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/pretrained/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 18:28:14.000000 transphone-1.5.1/transphone/pretrained/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2536 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/run.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1350 2023-05-15 07:50:03.000000 transphone-1.5.1/transphone/tokenizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      491 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/utils.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone.egg-info/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone.egg-info/PKG-INFO
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1514 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone.egg-info/SOURCES.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        1 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone.egg-info/dependency_links.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      111 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone.egg-info/requires.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       11 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone.egg-info/top_level.txt
```

### Comparing `transphone-1.5.0/LICENSE` & `transphone-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/README.md` & `transphone-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/test/test_tokenizer.py` & `transphone-1.5.1/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/bin/download_model.py` & `transphone-1.5.1/transphone/bin/download_model.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/bin/eval_epitran.py` & `transphone-1.5.1/transphone/bin/eval_epitran.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/bin/eval_g2p.py` & `transphone-1.5.1/transphone/bin/eval_g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/bin/eval_zsl_g2p.py` & `transphone-1.5.1/transphone/bin/eval_zsl_g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/bin/g2p.py` & `transphone-1.5.1/transphone/bin/g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/bin/tokenize.py` & `transphone-1.5.1/transphone/bin/tokenize.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/bin/train_g2p.py` & `transphone-1.5.1/transphone/bin/train_g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/bin/update_model.py` & `transphone-1.5.1/transphone/bin/update_model.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/g2p.py` & `transphone-1.5.1/transphone/g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/lang/base_tokenizer.py` & `transphone-1.5.1/transphone/lang/base_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/lang/cmn/normalizer.py` & `transphone-1.5.1/transphone/lang/cmn/normalizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/lang/cmn/tokenizer.py` & `transphone-1.5.1/transphone/lang/cmn/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/lang/eng/normalizer.py` & `transphone-1.5.1/transphone/lang/eng/normalizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/lang/eng/tokenizer.py` & `transphone-1.5.1/transphone/lang/eng/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/lang/epitran_tokenizer.py` & `transphone-1.5.1/transphone/lang/epitran_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/lang/g2p_tokenizer.py` & `transphone-1.5.1/transphone/lang/g2p_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/lang/jpn/conv_table.py` & `transphone-1.5.1/transphone/lang/jpn/conv_table.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/lang/jpn/jaconv.py` & `transphone-1.5.1/transphone/lang/jpn/jaconv.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/lang/jpn/kana2phoneme.py` & `transphone-1.5.1/transphone/lang/jpn/kana2phoneme.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/lang/jpn/normalizer.py` & `transphone-1.5.1/transphone/lang/jpn/normalizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/lang/jpn/tokenizer.py` & `transphone-1.5.1/transphone/lang/jpn/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/model/checkpoint_utils.py` & `transphone-1.5.1/transphone/model/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/model/dataset.py` & `transphone-1.5.1/transphone/model/dataset.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/model/ensemble.py` & `transphone-1.5.1/transphone/model/ensemble.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/model/grapheme.py` & `transphone-1.5.1/transphone/model/grapheme.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/model/lstm.py` & `transphone-1.5.1/transphone/model/lstm.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/model/transformer.py` & `transphone-1.5.1/transphone/model/transformer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/model/utils.py` & `transphone-1.5.1/transphone/model/utils.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/model/vocab.py` & `transphone-1.5.1/transphone/model/vocab.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/run.py` & `transphone-1.5.1/transphone/run.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone/tokenizer.py` & `transphone-1.5.1/transphone/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.0/transphone.egg-info/SOURCES.txt` & `transphone-1.5.1/transphone.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 transphone/bin/eval_g2p.py
 transphone/bin/eval_zsl_g2p.py
 transphone/bin/g2p.py
 transphone/bin/tokenize.py
 transphone/bin/train_g2p.py
 transphone/bin/update_model.py
 transphone/data/__init__.py
+transphone/data/exp/042801_base.yml
 transphone/lang/__init__.py
 transphone/lang/base_tokenizer.py
 transphone/lang/epitran_tokenizer.py
 transphone/lang/g2p_tokenizer.py
 transphone/lang/cmn/__init__.py
 transphone/lang/cmn/normalizer.py
 transphone/lang/cmn/tokenizer.py
```

