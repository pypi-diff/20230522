# Comparing `tmp/nkululeko-0.45.3.tar.gz` & `tmp/nkululeko-0.45.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nkululeko-0.45.3.tar", last modified: Thu May 11 14:14:57 2023, max compression
+gzip compressed data, was "nkululeko-0.45.5.tar", last modified: Mon May 22 09:13:44 2023, max compression
```

## Comparing `nkululeko-0.45.3.tar` & `nkululeko-0.45.5.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-11 14:14:57.449712 nkululeko-0.45.3/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5897 2023-05-11 13:29:31.000000 nkululeko-0.45.3/CHANGELOG.md
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.45.3/LICENSE
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16919 2023-05-11 14:14:57.449712 nkululeko-0.45.3/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10469 2023-05-11 10:04:04.000000 nkululeko-0.45.3/README.md
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-11 14:14:57.449712 nkululeko-0.45.3/nkululeko/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        0 2023-01-20 08:45:34.000000 nkululeko-0.45.3/nkululeko/__init__.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.45.3/nkululeko/augment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.45.3/nkululeko/augmenter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.45.3/nkululeko/balancer.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.45.3/nkululeko/cacheddataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       19 2023-05-11 13:28:12.000000 nkululeko-0.45.3/nkululeko/constants.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-05-08 11:23:11.000000 nkululeko-0.45.3/nkululeko/dataset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1908 2023-04-27 08:57:05.000000 nkululeko-0.45.3/nkululeko/dataset_csv.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.45.3/nkululeko/dataset_ravdess.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1815 2023-05-11 13:37:47.000000 nkululeko-0.45.3/nkululeko/demo.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.45.3/nkululeko/demo_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20481 2023-05-11 13:35:15.000000 nkululeko-0.45.3/nkululeko/experiment.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1960 2023-05-11 13:37:32.000000 nkululeko-0.45.3/nkululeko/explore.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3728 2023-05-11 10:12:48.000000 nkululeko-0.45.3/nkululeko/feats_analyser.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.45.3/nkululeko/feats_audmodel.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.45.3/nkululeko/feats_audmodel_dim.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.45.3/nkululeko/feats_clap.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.45.3/nkululeko/feats_import.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.45.3/nkululeko/feats_mld.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.45.3/nkululeko/feats_opensmile.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.45.3/nkululeko/feats_oxbow.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1832 2023-05-04 14:30:50.000000 nkululeko-0.45.3/nkululeko/feats_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.45.3/nkululeko/feats_trill.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.45.3/nkululeko/feats_wav2vec2.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.45.3/nkululeko/feature_extractor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.45.3/nkululeko/featureset.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.45.3/nkululeko/feinberg_praat.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.45.3/nkululeko/filter_data.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.45.3/nkululeko/glob_conf.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.45.3/nkululeko/loss_ccc.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.45.3/nkululeko/loss_softf1loss.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.45.3/nkululeko/model.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.45.3/nkululeko/model_bayes.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.45.3/nkululeko/model_cnn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.45.3/nkululeko/model_gmm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.45.3/nkululeko/model_knn.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.45.3/nkululeko/model_knn_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.45.3/nkululeko/model_mlp.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.45.3/nkululeko/model_mlp_regression.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.45.3/nkululeko/model_svm.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.45.3/nkululeko/model_svr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.45.3/nkululeko/model_tree.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.45.3/nkululeko/model_tree_reg.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.45.3/nkululeko/model_xgb.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.45.3/nkululeko/model_xgr.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.45.3/nkululeko/modelrunner.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1540 2023-05-11 13:36:48.000000 nkululeko-0.45.3/nkululeko/nkululeko.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6450 2023-04-20 15:44:41.000000 nkululeko-0.45.3/nkululeko/plots.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10170 2023-03-23 13:43:00.000000 nkululeko-0.45.3/nkululeko/reporter.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.45.3/nkululeko/result.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.45.3/nkululeko/runmanager.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.45.3/nkululeko/scaler.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1366 2023-05-11 13:41:29.000000 nkululeko-0.45.3/nkululeko/test.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.45.3/nkululeko/test_predictor.py
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8381 2023-05-11 09:13:01.000000 nkululeko-0.45.3/nkululeko/util.py
-drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-11 14:14:57.449712 nkululeko-0.45.3/nkululeko.egg-info/
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    16919 2023-05-11 14:14:57.000000 nkululeko-0.45.3/nkululeko.egg-info/PKG-INFO
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1565 2023-05-11 14:14:57.000000 nkululeko-0.45.3/nkululeko.egg-info/SOURCES.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-05-11 14:14:57.000000 nkululeko-0.45.3/nkululeko.egg-info/dependency_links.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-05-11 14:14:57.000000 nkululeko-0.45.3/nkululeko.egg-info/requires.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-05-11 14:14:57.000000 nkululeko-0.45.3/nkululeko.egg-info/top_level.txt
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.45.3/pyproject.toml
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      938 2023-05-11 14:14:57.453712 nkululeko-0.45.3/setup.cfg
--rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       59 2023-01-20 08:48:57.000000 nkululeko-0.45.3/setup.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-22 09:13:44.156439 nkululeko-0.45.5/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6029 2023-05-22 09:13:10.000000 nkululeko-0.45.5/CHANGELOG.md
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1076 2021-10-28 13:49:53.000000 nkululeko-0.45.5/LICENSE
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17051 2023-05-22 09:13:44.156439 nkululeko-0.45.5/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10469 2023-05-11 10:04:04.000000 nkululeko-0.45.5/README.md
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-22 09:13:44.156439 nkululeko-0.45.5/nkululeko/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       63 2023-05-22 09:01:23.000000 nkululeko-0.45.5/nkululeko/__init__.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1385 2023-03-07 15:26:22.000000 nkululeko-0.45.5/nkululeko/augment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2399 2023-03-23 15:05:56.000000 nkululeko-0.45.5/nkululeko/augmenter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       12 2023-01-14 20:36:15.000000 nkululeko-0.45.5/nkululeko/balancer.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      955 2023-01-16 11:55:06.000000 nkululeko-0.45.5/nkululeko/cacheddataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       19 2023-05-22 09:12:46.000000 nkululeko-0.45.5/nkululeko/constants.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    21627 2023-05-08 11:23:11.000000 nkululeko-0.45.5/nkululeko/dataset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1908 2023-04-27 08:57:05.000000 nkululeko-0.45.5/nkululeko/dataset_csv.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      537 2023-01-16 11:56:12.000000 nkululeko-0.45.5/nkululeko/dataset_ravdess.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1815 2023-05-11 13:37:47.000000 nkululeko-0.45.5/nkululeko/demo.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2286 2023-02-15 16:29:45.000000 nkululeko-0.45.5/nkululeko/demo_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    20481 2023-05-11 13:35:15.000000 nkululeko-0.45.5/nkululeko/experiment.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1960 2023-05-11 13:37:32.000000 nkululeko-0.45.5/nkululeko/explore.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3728 2023-05-11 10:12:48.000000 nkululeko-0.45.5/nkululeko/feats_analyser.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2748 2023-05-04 14:30:28.000000 nkululeko-0.45.5/nkululeko/feats_audmodel.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2739 2023-05-04 14:30:21.000000 nkululeko-0.45.5/nkululeko/feats_audmodel_dim.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3250 2023-05-04 14:30:36.000000 nkululeko-0.45.5/nkululeko/feats_clap.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2045 2023-05-04 14:08:00.000000 nkululeko-0.45.5/nkululeko/feats_import.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1949 2023-02-09 11:57:32.000000 nkululeko-0.45.5/nkululeko/feats_mld.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2772 2023-02-09 11:59:54.000000 nkululeko-0.45.5/nkululeko/feats_opensmile.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4425 2023-02-09 12:00:41.000000 nkululeko-0.45.5/nkululeko/feats_oxbow.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1832 2023-05-04 14:30:50.000000 nkululeko-0.45.5/nkululeko/feats_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2975 2023-04-19 20:26:13.000000 nkululeko-0.45.5/nkululeko/feats_trill.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     4005 2023-02-09 12:01:59.000000 nkululeko-0.45.5/nkululeko/feats_wav2vec2.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3456 2023-05-04 13:43:15.000000 nkululeko-0.45.5/nkululeko/feature_extractor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1319 2023-02-28 14:54:13.000000 nkululeko-0.45.5/nkululeko/featureset.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    13546 2023-01-16 10:52:58.000000 nkululeko-0.45.5/nkululeko/feinberg_praat.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1821 2023-01-16 12:04:04.000000 nkululeko-0.45.5/nkululeko/filter_data.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      237 2023-01-16 11:49:55.000000 nkululeko-0.45.5/nkululeko/glob_conf.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      939 2023-01-14 20:36:15.000000 nkululeko-0.45.5/nkululeko/loss_ccc.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1329 2023-01-14 20:36:15.000000 nkululeko-0.45.5/nkululeko/loss_softf1loss.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    12074 2023-02-20 12:50:06.000000 nkululeko-0.45.5/nkululeko/model.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      432 2023-03-24 08:08:57.000000 nkululeko-0.45.5/nkululeko/model_bayes.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5029 2023-03-24 08:09:03.000000 nkululeko-0.45.5/nkululeko/model_cnn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      603 2023-03-24 08:09:21.000000 nkululeko-0.45.5/nkululeko/model_gmm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      544 2023-03-24 08:10:02.000000 nkululeko-0.45.5/nkululeko/model_knn.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      551 2023-03-24 08:09:46.000000 nkululeko-0.45.5/nkululeko/model_knn_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8007 2023-03-24 08:10:19.000000 nkululeko-0.45.5/nkululeko/model_mlp.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8781 2023-03-24 08:10:12.000000 nkululeko-0.45.5/nkululeko/model_mlp_regression.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      522 2023-03-24 08:10:26.000000 nkululeko-0.45.5/nkululeko/model_svm.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      505 2023-03-24 08:10:49.000000 nkululeko-0.45.5/nkululeko/model_svr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      382 2023-03-24 08:11:15.000000 nkululeko-0.45.5/nkululeko/model_tree.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      389 2023-03-24 08:10:58.000000 nkululeko-0.45.5/nkululeko/model_tree_reg.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      236 2023-03-24 08:11:22.000000 nkululeko-0.45.5/nkululeko/model_xgb.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      242 2023-03-24 08:11:33.000000 nkululeko-0.45.5/nkululeko/model_xgr.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     5367 2023-03-24 08:13:41.000000 nkululeko-0.45.5/nkululeko/modelrunner.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1540 2023-05-11 13:36:48.000000 nkululeko-0.45.5/nkululeko/nkululeko.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6450 2023-04-20 15:44:41.000000 nkululeko-0.45.5/nkululeko/plots.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    10170 2023-03-23 13:43:00.000000 nkululeko-0.45.5/nkululeko/reporter.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      406 2023-01-16 11:15:47.000000 nkululeko-0.45.5/nkululeko/result.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     6753 2023-02-20 11:58:56.000000 nkululeko-0.45.5/nkululeko/runmanager.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     3013 2023-01-16 11:17:07.000000 nkululeko-0.45.5/nkululeko/scaler.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1366 2023-05-11 13:41:29.000000 nkululeko-0.45.5/nkululeko/test.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     2315 2023-01-16 12:10:32.000000 nkululeko-0.45.5/nkululeko/test_predictor.py
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     8381 2023-05-11 09:13:01.000000 nkululeko-0.45.5/nkululeko/util.py
+drwxr-xr-x   0 fburkhardt (767601207) domain users (767600513)        0 2023-05-22 09:13:44.156439 nkululeko-0.45.5/nkululeko.egg-info/
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)    17051 2023-05-22 09:13:44.000000 nkululeko-0.45.5/nkululeko.egg-info/PKG-INFO
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)     1565 2023-05-22 09:13:44.000000 nkululeko-0.45.5/nkululeko.egg-info/SOURCES.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)        1 2023-05-22 09:13:44.000000 nkululeko-0.45.5/nkululeko.egg-info/dependency_links.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      259 2023-05-22 09:13:44.000000 nkululeko-0.45.5/nkululeko.egg-info/requires.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       10 2023-05-22 09:13:44.000000 nkululeko-0.45.5/nkululeko.egg-info/top_level.txt
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      100 2023-01-16 10:13:10.000000 nkululeko-0.45.5/pyproject.toml
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)      959 2023-05-22 09:13:44.156439 nkululeko-0.45.5/setup.cfg
+-rw-r--r--   0 fburkhardt (767601207) domain users (767600513)       57 2023-05-22 09:01:18.000000 nkululeko-0.45.5/setup.py
```

### Comparing `nkululeko-0.45.3/CHANGELOG.md` & `nkululeko-0.45.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+Version 0.45.4
+--------------
+* added version attribute to setup.cfg
+
+Version 0.45.4
+--------------
+* added __version__ attribute
+
+
 Version 0.44.1
 --------------
 * bugfixing: feature importance: https://github.com/felixbur/nkululeko/issues/23
 * bugfixing: loading csv database with filewise index https://github.com/felixbur/nkululeko/issues/24 
 
 Version 0.45.2
 --------------
```

### Comparing `nkululeko-0.45.3/LICENSE` & `nkululeko-0.45.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/PKG-INFO` & `nkululeko-0.45.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.45.3
+Version: 0.45.5
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -208,14 +208,23 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.45.4
+--------------
+* added version attribute to setup.cfg
+
+Version 0.45.4
+--------------
+* added __version__ attribute
+
+
 Version 0.44.1
 --------------
 * bugfixing: feature importance: https://github.com/felixbur/nkululeko/issues/23
 * bugfixing: loading csv database with filewise index https://github.com/felixbur/nkululeko/issues/24 
 
 Version 0.45.2
 --------------
```

### Comparing `nkululeko-0.45.3/README.md` & `nkululeko-0.45.5/README.md`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/augment.py` & `nkululeko-0.45.5/nkululeko/augment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/augmenter.py` & `nkululeko-0.45.5/nkululeko/augmenter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/cacheddataset.py` & `nkululeko-0.45.5/nkululeko/cacheddataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/dataset.py` & `nkululeko-0.45.5/nkululeko/dataset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/dataset_csv.py` & `nkululeko-0.45.5/nkululeko/dataset_csv.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/dataset_ravdess.py` & `nkululeko-0.45.5/nkululeko/dataset_ravdess.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/demo.py` & `nkululeko-0.45.5/nkululeko/demo.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/demo_predictor.py` & `nkululeko-0.45.5/nkululeko/demo_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/experiment.py` & `nkululeko-0.45.5/nkululeko/experiment.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/explore.py` & `nkululeko-0.45.5/nkululeko/explore.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/feats_analyser.py` & `nkululeko-0.45.5/nkululeko/feats_analyser.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/feats_audmodel.py` & `nkululeko-0.45.5/nkululeko/feats_audmodel.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/feats_audmodel_dim.py` & `nkululeko-0.45.5/nkululeko/feats_audmodel_dim.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/feats_clap.py` & `nkululeko-0.45.5/nkululeko/feats_clap.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/feats_import.py` & `nkululeko-0.45.5/nkululeko/feats_import.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/feats_mld.py` & `nkululeko-0.45.5/nkululeko/feats_mld.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/feats_opensmile.py` & `nkululeko-0.45.5/nkululeko/feats_opensmile.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/feats_oxbow.py` & `nkululeko-0.45.5/nkululeko/feats_oxbow.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/feats_praat.py` & `nkululeko-0.45.5/nkululeko/feats_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/feats_trill.py` & `nkululeko-0.45.5/nkululeko/feats_trill.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/feats_wav2vec2.py` & `nkululeko-0.45.5/nkululeko/feats_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/feature_extractor.py` & `nkululeko-0.45.5/nkululeko/feature_extractor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/featureset.py` & `nkululeko-0.45.5/nkululeko/featureset.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/feinberg_praat.py` & `nkululeko-0.45.5/nkululeko/feinberg_praat.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/filter_data.py` & `nkululeko-0.45.5/nkululeko/filter_data.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/loss_ccc.py` & `nkululeko-0.45.5/nkululeko/loss_ccc.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/loss_softf1loss.py` & `nkululeko-0.45.5/nkululeko/loss_softf1loss.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/model.py` & `nkululeko-0.45.5/nkululeko/model.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/model_cnn.py` & `nkululeko-0.45.5/nkululeko/model_cnn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/model_gmm.py` & `nkululeko-0.45.5/nkululeko/model_gmm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/model_knn.py` & `nkululeko-0.45.5/nkululeko/model_knn.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/model_knn_reg.py` & `nkululeko-0.45.5/nkululeko/model_knn_reg.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/model_mlp.py` & `nkululeko-0.45.5/nkululeko/model_mlp.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/model_mlp_regression.py` & `nkululeko-0.45.5/nkululeko/model_mlp_regression.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/model_svm.py` & `nkululeko-0.45.5/nkululeko/model_svm.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/modelrunner.py` & `nkululeko-0.45.5/nkululeko/modelrunner.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/nkululeko.py` & `nkululeko-0.45.5/nkululeko/nkululeko.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/plots.py` & `nkululeko-0.45.5/nkululeko/plots.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/reporter.py` & `nkululeko-0.45.5/nkululeko/reporter.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/runmanager.py` & `nkululeko-0.45.5/nkululeko/runmanager.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/scaler.py` & `nkululeko-0.45.5/nkululeko/scaler.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/test.py` & `nkululeko-0.45.5/nkululeko/test.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/test_predictor.py` & `nkululeko-0.45.5/nkululeko/test_predictor.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko/util.py` & `nkululeko-0.45.5/nkululeko/util.py`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/nkululeko.egg-info/PKG-INFO` & `nkululeko-0.45.5/nkululeko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nkululeko
-Version: 0.45.3
+Version: 0.45.5
 Summary: Machine learning audio prediction experiments based on templates
 Home-page: https://github.com/felixbur/nkululeko
 Author: Felix Burkhardt
 Author-email: fxburk@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -208,14 +208,23 @@
 
 ## License
 Nkululeko can be used under the [MIT license](https://choosealicense.com/licenses/mit/)
 
 Changelog
 =========
 
+Version 0.45.4
+--------------
+* added version attribute to setup.cfg
+
+Version 0.45.4
+--------------
+* added __version__ attribute
+
+
 Version 0.44.1
 --------------
 * bugfixing: feature importance: https://github.com/felixbur/nkululeko/issues/23
 * bugfixing: loading csv database with filewise index https://github.com/felixbur/nkululeko/issues/24 
 
 Version 0.45.2
 --------------
```

### Comparing `nkululeko-0.45.3/nkululeko.egg-info/SOURCES.txt` & `nkululeko-0.45.5/nkululeko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nkululeko-0.45.3/setup.cfg` & `nkululeko-0.45.5/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = nkululeko
-version = 0.45.3
 author = Felix Burkhardt
 author_email = fxburk@gmail.com
 description = Machine learning audio prediction experiments based on templates
+version = attr: nkululeko.__version__
 long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 url = https://github.com/felixbur/nkululeko
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
```

