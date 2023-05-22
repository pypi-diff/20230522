# Comparing `tmp/nkululeko-0.45.2.tar.gz` & `tmp/nkululeko-0.45.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.45.2.tar", last modified: Thu May 11 09:24:58 2023, max compression
+gzip compressed data, was "nkululeko-0.45.3.tar", last modified: Thu May 11 14:14:57 2023, max compression
```

## Comparing `nkululeko-0.45.2.tar` & `nkululeko-0.45.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-11 09:24:58.971481 nkululeko-0.45.2/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5810 2023-05-11 09:20:49.000000 nkululeko-0.45.2/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.45.2/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16700 2023-05-11 09:24:58.971481 nkululeko-0.45.2/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10337 2023-05-11 07:49:43.000000 nkululeko-0.45.2/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-11 09:24:58.971481 nkululeko-0.45.2/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-01-20 08:45:34.000000 nkululeko-0.45.2/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.45.2/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.45.2/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.45.2/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.45.2/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       19 2023-05-11 09:19:51.000000 nkululeko-0.45.2/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-05-08 11:23:11.000000 nkululeko-0.45.2/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1908 2023-04-27 08:57:05.000000 nkululeko-0.45.2/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.45.2/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1789 2023-02-15 16:47:19.000000 nkululeko-0.45.2/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.45.2/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20481 2023-05-11 09:16:07.000000 nkululeko-0.45.2/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1934 2023-05-11 09:14:55.000000 nkululeko-0.45.2/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3726 2023-04-18 13:35:09.000000 nkululeko-0.45.2/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.45.2/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.45.2/nkululeko/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.45.2/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.45.2/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.45.2/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.45.2/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.45.2/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1832 2023-05-04 14:30:50.000000 nkululeko-0.45.2/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.45.2/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.45.2/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.45.2/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.45.2/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.45.2/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.45.2/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.45.2/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.45.2/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.45.2/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.45.2/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.45.2/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.45.2/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.45.2/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.45.2/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.45.2/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.45.2/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.45.2/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.45.2/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.45.2/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.45.2/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.45.2/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.45.2/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.45.2/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.45.2/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1514 2023-01-16 11:50:04.000000 nkululeko-0.45.2/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6450 2023-04-20 15:44:41.000000 nkululeko-0.45.2/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10170 2023-03-23 13:43:00.000000 nkululeko-0.45.2/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.45.2/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.45.2/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.45.2/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1340 2023-02-20 12:57:51.000000 nkululeko-0.45.2/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.45.2/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8381 2023-05-11 09:13:01.000000 nkululeko-0.45.2/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-11 09:24:58.971481 nkululeko-0.45.2/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16700 2023-05-11 09:24:58.000000 nkululeko-0.45.2/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1565 2023-05-11 09:24:58.000000 nkululeko-0.45.2/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-05-11 09:24:58.000000 nkululeko-0.45.2/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-05-11 09:24:58.000000 nkululeko-0.45.2/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-05-11 09:24:58.000000 nkululeko-0.45.2/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.45.2/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      938 2023-05-11 09:24:58.971481 nkululeko-0.45.2/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       59 2023-01-20 08:48:57.000000 nkululeko-0.45.2/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-11 14:14:57.449712 nkululeko-0.45.3/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5897 2023-05-11 13:29:31.000000 nkululeko-0.45.3/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.45.3/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16919 2023-05-11 14:14:57.449712 nkululeko-0.45.3/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10469 2023-05-11 10:04:04.000000 nkululeko-0.45.3/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-11 14:14:57.449712 nkululeko-0.45.3/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-01-20 08:45:34.000000 nkululeko-0.45.3/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.45.3/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.45.3/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.45.3/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.45.3/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       19 2023-05-11 13:28:12.000000 nkululeko-0.45.3/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-05-08 11:23:11.000000 nkululeko-0.45.3/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1908 2023-04-27 08:57:05.000000 nkululeko-0.45.3/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.45.3/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1815 2023-05-11 13:37:47.000000 nkululeko-0.45.3/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.45.3/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20481 2023-05-11 13:35:15.000000 nkululeko-0.45.3/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1960 2023-05-11 13:37:32.000000 nkululeko-0.45.3/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3728 2023-05-11 10:12:48.000000 nkululeko-0.45.3/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.45.3/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.45.3/nkululeko/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.45.3/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.45.3/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.45.3/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.45.3/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.45.3/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1832 2023-05-04 14:30:50.000000 nkululeko-0.45.3/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.45.3/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.45.3/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.45.3/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.45.3/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.45.3/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.45.3/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.45.3/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.45.3/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.45.3/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.45.3/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.45.3/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.45.3/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.45.3/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.45.3/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.45.3/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.45.3/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.45.3/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.45.3/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.45.3/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.45.3/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.45.3/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.45.3/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.45.3/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.45.3/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1540 2023-05-11 13:36:48.000000 nkululeko-0.45.3/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6450 2023-04-20 15:44:41.000000 nkululeko-0.45.3/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10170 2023-03-23 13:43:00.000000 nkululeko-0.45.3/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.45.3/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.45.3/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.45.3/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1366 2023-05-11 13:41:29.000000 nkululeko-0.45.3/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.45.3/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8381 2023-05-11 09:13:01.000000 nkululeko-0.45.3/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-11 14:14:57.449712 nkululeko-0.45.3/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16919 2023-05-11 14:14:57.000000 nkululeko-0.45.3/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1565 2023-05-11 14:14:57.000000 nkululeko-0.45.3/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-05-11 14:14:57.000000 nkululeko-0.45.3/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-05-11 14:14:57.000000 nkululeko-0.45.3/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-05-11 14:14:57.000000 nkululeko-0.45.3/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.45.3/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      938 2023-05-11 14:14:57.453712 nkululeko-0.45.3/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       59 2023-01-20 08:48:57.000000 nkululeko-0.45.3/setup.py
```

### Comparing `nkululeko-0.45.2/CHANGELOG.md` & `nkululeko-0.45.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 Version 0.44.1
 --------------
 * bugfixing: feature importance: https://github.com/felixbur/nkululeko/issues/23
 * bugfixing: loading csv database with filewise index https://github.com/felixbur/nkululeko/issues/24 
 
 Version 0.45.2
 --------------
+* bugfix: sample_selection in EXPL was required wrongly
+
+Version 0.45.2
+--------------
 * added sample_selection for sample distribution plots
 
 Version 0.45.1
 --------------
 * fixed dataframe.append bug
 
 Version 0.45.0
```

### Comparing `nkululeko-0.45.2/LICENSE` & `nkululeko-0.45.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/PKG-INFO` & `nkululeko-0.45.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.45.2
+Version: 0.45.3
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -137,14 +137,15 @@
 * [Compare several MLP layer layouts with each other](http://blog.syntheticspeech.de/2022/04/11/how-to-compare-several-mlp-layer-layouts-with-each-other/)
 * [Import features from outside the software](http://blog.syntheticspeech.de/2022/10/18/how-to-import-features-from-outside-the-nkululeko-software/)
 * [Explore feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Plot distributions for feature values](http://blog.syntheticspeech.de/2023/02/16/nkululeko-how-to-plot-distributions-of-feature-values/)
 * [Show feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
  * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
+ * [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
 
 The framework is targeted at the speech domain and supports experiments where different classifiers are combined with different feature extractors.
 
 Here's a rough UML-like sketch of the framework.
 ![sketch](images/class_diagram.png)
 
 Currently, the following linear classifiers are implemented (integrated from sklearn):
@@ -214,14 +215,18 @@
 Version 0.44.1
 --------------
 * bugfixing: feature importance: https://github.com/felixbur/nkululeko/issues/23
 * bugfixing: loading csv database with filewise index https://github.com/felixbur/nkululeko/issues/24 
 
 Version 0.45.2
 --------------
+* bugfix: sample_selection in EXPL was required wrongly
+
+Version 0.45.2
+--------------
 * added sample_selection for sample distribution plots
 
 Version 0.45.1
 --------------
 * fixed dataframe.append bug
 
 Version 0.45.0
```

### Comparing `nkululeko-0.45.2/README.md` & `nkululeko-0.45.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,15 @@
 * [Compare several MLP layer layouts with each other](http://blog.syntheticspeech.de/2022/04/11/how-to-compare-several-mlp-layer-layouts-with-each-other/)
 * [Import features from outside the software](http://blog.syntheticspeech.de/2022/10/18/how-to-import-features-from-outside-the-nkululeko-software/)
 * [Explore feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Plot distributions for feature values](http://blog.syntheticspeech.de/2023/02/16/nkululeko-how-to-plot-distributions-of-feature-values/)
 * [Show feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
  * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
+ * [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
 
 The framework is targeted at the speech domain and supports experiments where different classifiers are combined with different feature extractors.
 
 Here's a rough UML-like sketch of the framework.
 ![sketch](images/class_diagram.png)
 
 Currently, the following linear classifiers are implemented (integrated from sklearn):
```

### Comparing `nkululeko-0.45.2/nkululeko/augment.py` & `nkululeko-0.45.3/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/augmenter.py` & `nkululeko-0.45.3/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/cacheddataset.py` & `nkululeko-0.45.3/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/dataset.py` & `nkululeko-0.45.3/nkululeko/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/dataset_csv.py` & `nkululeko-0.45.3/nkululeko/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/dataset_ravdess.py` & `nkululeko-0.45.3/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/demo.py` & `nkululeko-0.45.3/nkululeko/demo.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
     
     # create a new experiment
     expr = Experiment(config)
     util = Util()
-    util.debug(f'running {expr.name}, nkululeko version {VERSION}')
+    util.debug(f'running {expr.name} from config {config_file}, nkululeko version {VERSION}')
 
     # load the experiment
     expr.load(f'{util.get_save_name()}')
     if args.file is None and args.list is None:
        expr.demo(None, False)
     else:
         if args.list is None:
```

### Comparing `nkululeko-0.45.2/nkululeko/demo_predictor.py` & `nkululeko-0.45.3/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/experiment.py` & `nkululeko-0.45.3/nkululeko/experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,33 +308,34 @@
 
     def analyse_features(self, needs_feats):
         """
         Do a feature exploration
         
         """
 
+        plot_feats = eval(self.util.config_val('EXPL', 'feature_distributions', 'False'))
+        sample_selection = self.util.config_val('EXPL', 'sample_selection', 'all')
+
         if self.util.config_val('EXPL', 'value_counts', False):
             self.plot_distribution()
         if not needs_feats:
             return
-        sample_selection = self.util.config_val('EXPL', 'sample_selection', 'False')
         if sample_selection=='all':
             df_feats = pd.concat([self.feats_train, self.feats_test])
             df_labels = pd.concat([self.df_train, self.df_test])
         elif sample_selection=='train':
             df_feats = self.feats_train
             df_labels = self.df_train
         elif sample_selection=='test':
             df_feats = self.feats_test
             df_labels = self.df_test
-        elif sample_selection=='False':
-            pass
         else:
-            self.util.error(f'unkown sample selection specifier {sample_selection}, should be [all | train | test]')
-        if sample_selection in ('all', 'train', 'test'):
+            self.util.error(f'unknown sample selection specifier {sample_selection}, should be [all | train | test]')
+
+        if plot_feats:
             feat_analyser = FeatureAnalyser(sample_selection, df_labels, df_feats)        
             feat_analyser.analyse()
 
         # check if a scatterplot should be done
         scatter_var = eval(self.util.config_val('EXPL', 'scatter', 'False'))
         if scatter_var:
             scatters = ast.literal_eval(glob_conf.config['EXPL']['scatter'])
```

### Comparing `nkululeko-0.45.2/nkululeko/explore.py` & `nkululeko-0.45.3/nkululeko/explore.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
     # create a new experiment
     expr = Experiment(config)
     util = Util()
-    util.debug(f'running {expr.name}, nkululeko version {VERSION}')
+    util.debug(f'running {expr.name} from config {config_file}, nkululeko version {VERSION}')
 
     # load the data
     expr.load_datasets()
 
     # split into train and test
     expr.fill_train_and_tests()
     util.debug(f'train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}')
```

### Comparing `nkululeko-0.45.2/nkululeko/feats_analyser.py` & `nkululeko-0.45.3/nkululeko/feats_analyser.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
                 model.fit(self.X, self.y)
                 importance = model.coef_
             elif model_s == 'tree':
                 model = DecisionTreeRegressor()
                 model.fit(self.X, self.y)
                 importance = model.feature_importances_
             else:
-                self.util.error(f'invalid analysis method: {model}')
+                self.util.error(f'invalid analysis method: {model_s}')
 
         df_imp = pd.DataFrame({'feats':self.X.columns, 'importance':importance})
         df_imp = df_imp.sort_values(by='importance', ascending=False).iloc[:max_feat_num]
         ax = df_imp.plot(x='feats', y='importance', kind='bar')
         ax.set(title=f'{self.label} samples')
         plt.tight_layout()
         fig_dir = self.util.get_path('fig_dir')+'../' # one up because of the runs
```

### Comparing `nkululeko-0.45.2/nkululeko/feats_audmodel.py` & `nkululeko-0.45.3/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/feats_audmodel_dim.py` & `nkululeko-0.45.3/nkululeko/feats_audmodel_dim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/feats_clap.py` & `nkululeko-0.45.3/nkululeko/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/feats_import.py` & `nkululeko-0.45.3/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/feats_mld.py` & `nkululeko-0.45.3/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/feats_opensmile.py` & `nkululeko-0.45.3/nkululeko/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/feats_oxbow.py` & `nkululeko-0.45.3/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/feats_praat.py` & `nkululeko-0.45.3/nkululeko/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/feats_trill.py` & `nkululeko-0.45.3/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/feats_wav2vec2.py` & `nkululeko-0.45.3/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/feature_extractor.py` & `nkululeko-0.45.3/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/featureset.py` & `nkululeko-0.45.3/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/feinberg_praat.py` & `nkululeko-0.45.3/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/filter_data.py` & `nkululeko-0.45.3/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/loss_ccc.py` & `nkululeko-0.45.3/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/loss_softf1loss.py` & `nkululeko-0.45.3/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/model.py` & `nkululeko-0.45.3/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/model_cnn.py` & `nkululeko-0.45.3/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/model_gmm.py` & `nkululeko-0.45.3/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/model_knn.py` & `nkululeko-0.45.3/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/model_knn_reg.py` & `nkululeko-0.45.3/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/model_mlp.py` & `nkululeko-0.45.3/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/model_mlp_regression.py` & `nkululeko-0.45.3/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/model_svm.py` & `nkululeko-0.45.3/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/modelrunner.py` & `nkululeko-0.45.3/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/nkululeko.py` & `nkululeko-0.45.3/nkululeko/nkululeko.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
     
     # create a new experiment
     expr = exp.Experiment(config)
     util = Util()
-    util.debug(f'running {expr.name}, nkululeko version {VERSION}')
+    util.debug(f'running {expr.name} from config {config_file}, nkululeko version {VERSION}')
 
     # load the data
     expr.load_datasets()
 
     # split into train and test
     expr.fill_train_and_tests()
     util.debug(f'train shape : {expr.df_train.shape}, test shape:{expr.df_test.shape}')
```

### Comparing `nkululeko-0.45.2/nkululeko/plots.py` & `nkululeko-0.45.3/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/reporter.py` & `nkululeko-0.45.3/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/runmanager.py` & `nkululeko-0.45.3/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/scaler.py` & `nkululeko-0.45.3/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/test.py` & `nkululeko-0.45.3/nkululeko/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     # load one configuration per experiment
     config = configparser.ConfigParser()
     config.read(config_file)
     
     # create a new experiment
     expr = Experiment(config)
     util = Util()
-    util.debug(f'running {expr.name}, nkululeko version {VERSION}')
+    util.debug(f'running {expr.name} from config {config_file}, nkululeko version {VERSION}')
 
     # load the experiment
     expr.load(f'{util.get_save_name()}')
     expr.fill_tests()
     expr.extract_test_feats()
     expr.predict_test_and_save(args.outfile)
```

### Comparing `nkululeko-0.45.2/nkululeko/test_predictor.py` & `nkululeko-0.45.3/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko/util.py` & `nkululeko-0.45.3/nkululeko/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.45.3/nkululeko.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.45.2
+Version: 0.45.3
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -137,14 +137,15 @@
 * [Compare several MLP layer layouts with each other](http://blog.syntheticspeech.de/2022/04/11/how-to-compare-several-mlp-layer-layouts-with-each-other/)
 * [Import features from outside the software](http://blog.syntheticspeech.de/2022/10/18/how-to-import-features-from-outside-the-nkululeko-software/)
 * [Explore feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Plot distributions for feature values](http://blog.syntheticspeech.de/2023/02/16/nkululeko-how-to-plot-distributions-of-feature-values/)
 * [Show feature importance](http://blog.syntheticspeech.de/2023/02/20/nkululeko-show-feature-importance/)
 * [Augment the training set](http://blog.syntheticspeech.de/2023/03/13/nkululeko-how-to-augment-the-training-set/)
  * [Visualize clusters of acoustic features](http://blog.syntheticspeech.de/2023/04/20/nkululeko-visualize-clusters-of-your-acoustic-features/)
+ * [Visualize your data distribution](http://blog.syntheticspeech.de/2023/05/11/nkululeko-how-to-visualize-your-data-distribution/)
 
 The framework is targeted at the speech domain and supports experiments where different classifiers are combined with different feature extractors.
 
 Here's a rough UML-like sketch of the framework.
 ![sketch](images/class_diagram.png)
 
 Currently, the following linear classifiers are implemented (integrated from sklearn):
@@ -214,14 +215,18 @@
 Version 0.44.1
 --------------
 * bugfixing: feature importance: https://github.com/felixbur/nkululeko/issues/23
 * bugfixing: loading csv database with filewise index https://github.com/felixbur/nkululeko/issues/24 
 
 Version 0.45.2
 --------------
+* bugfix: sample_selection in EXPL was required wrongly
+
+Version 0.45.2
+--------------
 * added sample_selection for sample distribution plots
 
 Version 0.45.1
 --------------
 * fixed dataframe.append bug
 
 Version 0.45.0
```

### Comparing `nkululeko-0.45.2/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.45.3/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.2/setup.cfg` & `nkululeko-0.45.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nkululeko
-version = 0.45.2
+version = 0.45.3
 author = Felix Burkhardt
 author_email = fxburk@gmail.com
 description = Machine learning audio prediction experiments based on templates
 long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 url = https://github.com/felixbur/nkululeko
 classifiers =
```

