# Comparing `tmp/rpbp-3.0.1.tar.gz` & `tmp/rpbp-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpbp-3.0.1.tar", last modified: Mon Feb 13 15:18:59 2023, max compression
+gzip compressed data, was "rpbp-3.0.2.tar", last modified: Mon May 22 06:42:49 2023, max compression
```

## Comparing `rpbp-3.0.1.tar` & `rpbp-3.0.2.tar`

### file list

```diff
@@ -1,89 +1,92 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.374886 rpbp-3.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-02-13 15:18:48.000000 rpbp-3.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-13 15:18:48.000000 rpbp-3.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-02-13 15:18:59.374886 rpbp-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-02-13 15:18:48.000000 rpbp-3.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-02-13 15:18:48.000000 rpbp-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 15:18:59.378886 rpbp-3.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.366886 rpbp-3.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.366886 rpbp-3.0.1/src/rpbp/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.370886 rpbp-3.0.1/src/rpbp/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.370886 rpbp-3.0.1/src/rpbp/analysis/profile_construction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/profile_construction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/profile_construction/collect_read_length_orf_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     5406 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/profile_construction/create_read_length_orf_profiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.370886 rpbp-3.0.1/src/rpbp/analysis/profile_construction/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/profile_construction/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/profile_construction/dashboard/controls.py
--rw-r--r--   0 runner    (1001) docker     (123)    51329 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/profile_construction/dashboard/rpbp_profile_construction_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/profile_construction/get_all_read_filtering_counts.py
--rw-r--r--   0 runner    (1001) docker     (123)    16401 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/profile_construction/summarize_rpbp_profile_construction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/profile_construction/visualize_metagene_profile_bayes_factor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.370886 rpbp-3.0.1/src/rpbp/analysis/proteomics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/proteomics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/proteomics/filter_nonunique_peptide_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/proteomics/get_all_orf_peptide_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/proteomics/get_orf_peptide_matches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.370886 rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.370886 rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.370886 rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/dashboard/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   133464 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/dashboard/assets/logo-rpbp.png
--rw-r--r--   0 runner    (1001) docker     (123)    54552 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/dashboard/assets/schematic.png
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/dashboard/assets/style.css
--rw-r--r--   0 runner    (1001) docker     (123)    42504 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/dashboard/rpbp_predictions_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    25985 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/summarize_rpbp_predictions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/visualize_orf_type_metagene_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.370886 rpbp-3.0.1/src/rpbp/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.374886 rpbp-3.0.1/src/rpbp/models/nonperiodic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/models/nonperiodic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/models/nonperiodic/no-periodicity.stan
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/models/nonperiodic/start-high-high-low.stan
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/models/nonperiodic/start-high-low-high.stan
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.374886 rpbp-3.0.1/src/rpbp/models/periodic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/models/periodic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/models/periodic/start-high-low-low.stan
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.374886 rpbp-3.0.1/src/rpbp/models/translated/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/models/translated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/models/translated/periodic-gaussian-mixture.stan
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.374886 rpbp-3.0.1/src/rpbp/models/untranslated/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/models/untranslated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/models/untranslated/gaussian-naive-bayes.stan
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.374886 rpbp-3.0.1/src/rpbp/orf_profile_construction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/orf_profile_construction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/orf_profile_construction/create_base_genome_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/orf_profile_construction/create_orf_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/orf_profile_construction/estimate_metagene_profile_bayes_factors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10131 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/orf_profile_construction/extract_metagene_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/orf_profile_construction/extract_orf_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/orf_profile_construction/select_periodic_offsets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.374886 rpbp-3.0.1/src/rpbp/reference_preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/reference_preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/reference_preprocessing/extract_orf_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    21097 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/reference_preprocessing/label_orfs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/reference_preprocessing/prepare_rpbp_genome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.374886 rpbp-3.0.1/src/rpbp/ribo_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/ribo_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/ribo_utils/compile_rpbp_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/ribo_utils/filenames.py
--rw-r--r--   0 runner    (1001) docker     (123)    25557 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/ribo_utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/run_all_rpbp_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/run_rpbp_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.374886 rpbp-3.0.1/src/rpbp/translation_prediction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/translation_prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/translation_prediction/estimate_orf_bayes_factors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/translation_prediction/merge_replicate_orf_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    14178 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/translation_prediction/predict_translated_orfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-02-13 15:18:48.000000 rpbp-3.0.1/src/rpbp/translation_prediction/select_final_prediction_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 15:18:59.370886 rpbp-3.0.1/src/rpbp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-02-13 15:18:59.000000 rpbp-3.0.1/src/rpbp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-02-13 15:18:59.000000 rpbp-3.0.1/src/rpbp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 15:18:59.000000 rpbp-3.0.1/src/rpbp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-02-13 15:18:59.000000 rpbp-3.0.1/src/rpbp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-02-13 15:18:59.000000 rpbp-3.0.1/src/rpbp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-13 15:18:59.000000 rpbp-3.0.1/src/rpbp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.161435 rpbp-3.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-22 06:42:38.000000 rpbp-3.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-22 06:42:38.000000 rpbp-3.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-22 06:42:49.161435 rpbp-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-05-22 06:42:38.000000 rpbp-3.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-22 06:42:38.000000 rpbp-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:42:49.161435 rpbp-3.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.149435 rpbp-3.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.153435 rpbp-3.0.2/src/rpbp/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.153435 rpbp-3.0.2/src/rpbp/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.153435 rpbp-3.0.2/src/rpbp/analysis/profile_construction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/profile_construction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/profile_construction/collect_read_length_orf_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5405 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/profile_construction/create_read_length_orf_profiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.153435 rpbp-3.0.2/src/rpbp/analysis/profile_construction/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/profile_construction/dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.157435 rpbp-3.0.2/src/rpbp/analysis/profile_construction/dashboard/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   133464 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/profile_construction/dashboard/assets/logo-rpbp.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/profile_construction/dashboard/assets/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/profile_construction/dashboard/controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51525 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/profile_construction/dashboard/rpbp_profile_construction_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4955 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/profile_construction/get_all_read_filtering_counts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/profile_construction/summarize_rpbp_profile_construction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/profile_construction/visualize_metagene_profile_bayes_factor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.157435 rpbp-3.0.2/src/rpbp/analysis/proteomics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/proteomics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/proteomics/filter_nonunique_peptide_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/proteomics/get_all_orf_peptide_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/proteomics/get_orf_peptide_matches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.157435 rpbp-3.0.2/src/rpbp/analysis/rpbp_predictions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/rpbp_predictions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.157435 rpbp-3.0.2/src/rpbp/analysis/rpbp_predictions/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/rpbp_predictions/dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.157435 rpbp-3.0.2/src/rpbp/analysis/rpbp_predictions/dashboard/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   133464 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/rpbp_predictions/dashboard/assets/logo-rpbp.png
+-rw-r--r--   0 runner    (1001) docker     (123)    54552 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/rpbp_predictions/dashboard/assets/schematic.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/rpbp_predictions/dashboard/assets/style.css
+-rw-r--r--   0 runner    (1001) docker     (123)    43445 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/rpbp_predictions/dashboard/rpbp_predictions_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26304 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/rpbp_predictions/summarize_rpbp_predictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8237 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/analysis/rpbp_predictions/visualize_orf_type_metagene_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.157435 rpbp-3.0.2/src/rpbp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.157435 rpbp-3.0.2/src/rpbp/models/nonperiodic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/models/nonperiodic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/models/nonperiodic/no-periodicity.stan
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/models/nonperiodic/start-high-high-low.stan
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/models/nonperiodic/start-high-low-high.stan
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.157435 rpbp-3.0.2/src/rpbp/models/periodic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/models/periodic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/models/periodic/start-high-low-low.stan
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.157435 rpbp-3.0.2/src/rpbp/models/translated/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/models/translated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/models/translated/periodic-gaussian-mixture.stan
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.157435 rpbp-3.0.2/src/rpbp/models/untranslated/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/models/untranslated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/models/untranslated/gaussian-naive-bayes.stan
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.161435 rpbp-3.0.2/src/rpbp/orf_profile_construction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/orf_profile_construction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9334 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/orf_profile_construction/create_base_genome_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12611 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/orf_profile_construction/create_orf_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10005 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/orf_profile_construction/estimate_metagene_profile_bayes_factors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/orf_profile_construction/extract_metagene_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/orf_profile_construction/extract_orf_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/orf_profile_construction/select_periodic_offsets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.161435 rpbp-3.0.2/src/rpbp/reference_preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/reference_preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/reference_preprocessing/extract_orf_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21093 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/reference_preprocessing/label_orfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13938 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/reference_preprocessing/prepare_rpbp_genome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.161435 rpbp-3.0.2/src/rpbp/ribo_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/ribo_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/ribo_utils/compile_rpbp_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13238 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/ribo_utils/filenames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25551 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/ribo_utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7414 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/run_all_rpbp_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/run_rpbp_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.161435 rpbp-3.0.2/src/rpbp/translation_prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/translation_prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/translation_prediction/estimate_orf_bayes_factors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/translation_prediction/merge_replicate_orf_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14176 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/translation_prediction/predict_translated_orfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-05-22 06:42:38.000000 rpbp-3.0.2/src/rpbp/translation_prediction/select_final_prediction_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:42:49.153435 rpbp-3.0.2/src/rpbp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-05-22 06:42:49.000000 rpbp-3.0.2/src/rpbp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-22 06:42:49.000000 rpbp-3.0.2/src/rpbp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:42:49.000000 rpbp-3.0.2/src/rpbp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-22 06:42:49.000000 rpbp-3.0.2/src/rpbp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-22 06:42:49.000000 rpbp-3.0.2/src/rpbp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-22 06:42:49.000000 rpbp-3.0.2/src/rpbp.egg-info/top_level.txt
```

### Comparing `rpbp-3.0.1/LICENSE` & `rpbp-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/PKG-INFO` & `rpbp-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpbp
-Version: 3.0.1
+Version: 3.0.2
 Summary: Rp-Bp: Ribosome Profiling with Bayesian Predictions
 Author: Brandon Malone
 Maintainer-email: Etienne Boileau <boileau@uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/dieterich-lab/rp-bp
 Project-URL: Issues, https://github.com/dieterich-lab/rp-bp/issues
 Keywords: bioinformatics,riboseq,open reading frame discovery,translation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rpbp Version: 3.0.1 Summary: Rp-Bp: Ribosome
+Metadata-Version: 2.1 Name: rpbp Version: 3.0.2 Summary: Rp-Bp: Ribosome
 Profiling with Bayesian Predictions Author: Brandon Malone Maintainer-email:
 Etienne Boileau
 uni-heidelberg.de> License: MIT Project-URL: Github, https://github.com/
 dieterich-lab/rp-bp Project-URL: Issues, https://github.com/dieterich-lab/rp-
 bp/issues Keywords: bioinformatics,riboseq,open reading frame
 discovery,translation Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
```

### Comparing `rpbp-3.0.1/README.md` & `rpbp-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/pyproject.toml` & `rpbp-3.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/analysis/profile_construction/collect_read_length_orf_profiles.py` & `rpbp-3.0.2/src/rpbp/analysis/profile_construction/collect_read_length_orf_profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,14 @@
         riboseq_replicates = ribo_utils.get_riboseq_replicates(config)
         names = [n for n in riboseq_replicates[args.name]]
 
     # keep a map from the lengths to the combined profiles
     length_profile_map = {}
 
     for name in names:
-
         msg = "Processing sample: {}".format(name)
         logger.info(msg)
 
         # get the lengths and offsets which meet the required criteria from the config file
         lengths, offsets = ribo_utils.get_periodic_lengths_and_offsets(
             config, name, is_unique=is_unique, default_params=metagene_options
         )
@@ -100,15 +99,14 @@
                 "min_metagene_profile_count, min_metagene_bf_mean, "
                 "max_metagene_bf_var, and/or min_metagene_bf_likelihood. Qutting."
             )
             logger.critical(msg)
             return
 
         for length, offset in zip(lengths, offsets):
-
             mtx = filenames.get_riboseq_profiles(
                 config["riboseq_data"],
                 name,
                 length=[length],
                 offset=[offset],
                 is_unique=is_unique,
                 note=note,
@@ -121,29 +119,27 @@
             if prior_mtx is None:
                 length_profile_map[length] = mtx
             else:
                 length_profile_map[length] = prior_mtx + mtx
 
     if args.add_ids:
         with gzip.open(args.out, "wb") as target_gz:
-
             for length, mtx in length_profile_map.items():
                 mtx = mtx.tocoo()
 
                 msg = "Writing ORF profiles. length: {}.".format(length)
                 logger.info(msg)
 
                 for row, col, val in zip(mtx.row, mtx.col, mtx.data):
                     # orf_num are both zero-based, since we are now using coo
                     orf_id = orfs.loc[orfs["orf_num"] == row]["id"].values[0]
                     s = "{} {} {} {} {}\n".format(row, orf_id, col, length, val)
                     target_gz.write(s.encode())
     else:
         with gzip.open(args.out, "wb") as target_gz:
-
             for length, mtx in length_profile_map.items():
                 mtx = mtx.tocoo()
 
                 msg = "Writing ORF profiles. length: {}.".format(length)
                 logger.info(msg)
 
                 for row, col, val in zip(mtx.row, mtx.col, mtx.data):
```

### Comparing `rpbp-3.0.1/src/rpbp/analysis/profile_construction/create_read_length_orf_profiles.py` & `rpbp-3.0.2/src/rpbp/analysis/profile_construction/create_read_length_orf_profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,14 @@
     if args.is_condition:
         is_condition_str = "--is-condition"
         riboseq_replicates = ribo_utils.get_riboseq_replicates(config)
         names = [n for n in riboseq_replicates[args.name]]
 
     job_ids = []
     for name in names:
-
         msg = "Processing sample: {}".format(name)
         logger.info(msg)
 
         # now the relevant files
         bam = filenames.get_riboseq_bam(
             config["riboseq_data"], name, is_unique=is_unique, note=note
         )
```

### Comparing `rpbp-3.0.1/src/rpbp/analysis/profile_construction/dashboard/controls.py` & `rpbp-3.0.2/src/rpbp/analysis/profile_construction/dashboard/controls.py`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/analysis/profile_construction/dashboard/rpbp_profile_construction_dashboard.py` & `rpbp-3.0.2/src/rpbp/analysis/profile_construction/dashboard/rpbp_profile_construction_dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,40 +40,48 @@
 sns.set({"ytick.direction": "out"}, style="ticks")
 sns.set(rc={"axes.facecolor": "#F9F9F8", "figure.facecolor": "#F9F9F8"})
 
 
 # ------------------------------------------------------ Functions ------------------------------------------------------
 
 
+def parse_env(key):
+    return (
+        {"default": os.environ.get(key)} if os.environ.get(key) else {"required": True}
+    )
+
+
 def get_parser():
     parser = argparse.ArgumentParser(
         description="Launch a Dash app for quality "
         "control and visualization of ribosome profiling "
         "data processed with Rp-Bp."
     )
 
     parser.add_argument(
-        "config",
+        "--config",
+        "-c",
         type=str,
+        **parse_env("RPBP_CFG"),
         help="A YAML configuration file." "The same used to run the pipeline.",
     )
 
     parser.add_argument("--debug", "-d", action="store_true", help="Enable debug mode.")
 
     parser.add_argument("--host", type=str, default="localhost", help="Host.")
 
     parser.add_argument("--port", type=int, default=8050, help="Port number.")
 
-    args = parser.parse_args()
+    # args = parser.parse_args()
+    args, unkn = parser.parse_known_args()
 
     return args.config, args.debug, args.host, args.port
 
 
 def get_diff_counts(data_np):
-
     # add an extra column so the diff counts will work
     zeros = np.zeros((data_np.shape[0], 1))
     data_np = np.append(zeros, data_np, axis=1)
     # get the diffs so the stacks work correctly
     diff = np.diff(data_np)
 
     return diff
@@ -83,15 +91,14 @@
     metagene_profile,
     offset,
     start_upstream_window,
     start_downstream_window,
     end_upstream_window,
     end_downstream_window,
 ):
-
     # profile around start codon
     start_upstream = start_upstream_window - offset
     start_downstream = start_downstream_window - offset
 
     mask_starts = metagene_profile["type"] == "start"
     m_start_upstream = metagene_profile["position"] >= start_upstream
     m_start_downstream = metagene_profile["position"] <= start_downstream
@@ -116,23 +123,21 @@
 def get_profiles_bars(
     samples,
     start_upstream_window,
     start_downstream_window,
     end_upstream_window,
     end_downstream_window,
 ):
-
     start_window_size = start_downstream_window - start_upstream_window + 1
     end_window_size = end_downstream_window - end_upstream_window + 1
 
     metagene_profile_start = np.zeros(start_window_size)
     metagene_profile_end = np.zeros(end_window_size)
 
     for sample in samples:
-
         sample_name = reverse_sample_name_map[sample]
 
         # TODO: if we have the df with all lengths and offsets ready, we don't need to
         # read them each time, but just subset the pre-loaded dataframe
         lengths, offsets = ribo_utils.get_periodic_lengths_and_offsets(
             config,
             sample_name,
@@ -145,15 +150,14 @@
                 sample_name,
                 is_unique=is_unique,
                 note=config.get("note", None),
             )
         )
 
         for length, offset in zip(lengths, offsets):
-
             m_length = metagene_profiles["length"] == int(length)
             metagene_profile = metagene_profiles[m_length]
 
             start_counts, end_counts = get_window_counts(
                 metagene_profile,
                 int(offset),
                 start_upstream_window,
@@ -170,23 +174,21 @@
 def get_profiles_lines(
     samples,
     start_upstream_window,
     start_downstream_window,
     end_upstream_window,
     end_downstream_window,
 ):
-
     start_window_size = start_downstream_window - start_upstream_window + 1
     end_window_size = end_downstream_window - end_upstream_window + 1
 
     all_ribo_metagene_profile_start_df = pd.DataFrame(columns=range(start_window_size))
     all_ribo_metagene_profile_end_df = pd.DataFrame(columns=range(end_window_size))
 
     for sample in samples:
-
         sample_name = reverse_sample_name_map[sample]
 
         # TODO: if we have the df with all lengths and offsets ready, we don't need to
         # read them each time, but just subset the pre-loaded dataframe
         lengths, offsets = ribo_utils.get_periodic_lengths_and_offsets(
             config,
             sample_name,
@@ -203,15 +205,14 @@
         )
 
         window_count_start, window_count_end = 0, 0
         metagene_profile_start = np.zeros(start_window_size)
         metagene_profile_end = np.zeros(end_window_size)
 
         for length, offset in zip(lengths, offsets):
-
             m_length = metagene_profiles["length"] == int(length)
             metagene_profile = metagene_profiles[m_length]
 
             start_counts, end_counts = get_window_counts(
                 metagene_profile,
                 int(offset),
                 start_upstream_window,
@@ -246,15 +247,14 @@
     end_downstream_window,
     step,
     figsize,
     y_label,
     y_max=None,
     layout=None,
 ):
-
     indices = [(0, 1, 2), (1, 0, 2), (2, 1, 0)]
     start_window_size = start_downstream_window - start_upstream_window + 1
     end_window_size = end_downstream_window - end_upstream_window + 1
 
     if y_max is None:
         ymax = max(max(metagene_profile_start), max(metagene_profile_end))
     else:
@@ -323,15 +323,14 @@
     end_upstream_window,
     end_downstream_window,
     step,
     figsize,
     y_label,
     y_max=None,
 ):
-
     start_window_size = start_downstream_window - start_upstream_window + 1
     end_window_size = end_downstream_window - end_upstream_window + 1
 
     if y_max is None:
         ymax = max(max(metagene_profile_start), max(metagene_profile_end))
     else:
         ymax = y_max
@@ -622,15 +621,15 @@
 
 
 # ------------------------------------------------------ APP ------------------------------------------------------
 
 app = dash.Dash(__name__)
 
 # do we have to expose the flask variable in the file?
-# server = app.server
+server = app.server
 
 app.layout = html.Div(
     [
         html.Div(
             [
                 html.Img(
                     src=app.get_asset_url("logo-rpbp.png"),
@@ -945,15 +944,14 @@
 
 # stacked bars read filtering counts
 @app.callback(
     Output("stacked_reads_fig", "figure"),
     [Input("drop_samples", "value"), Input("radio_stacked_reads", "value")],
 )
 def stacked_reads(selected, zoom):
-
     selected_samples = selected.split(",")
 
     stack_cts_order = STACK_CTS_ORDER
     stack_cts_name = STACK_CTS_NAME
     if zoom == 1:  # exclude ribosomal/poor quality
         stack_cts_order = stack_cts_order[:4]
         stack_cts_name = stack_cts_name[:4]
@@ -988,15 +986,14 @@
     [
         Input("stacked_reads_fig", "hoverData"),
         Input("radio_stacked_reads", "value"),
         Input("drop_samples", "value"),
     ],
 )
 def funnel_reads(hoverData, zoom, selected):
-
     stack_cts_order = STACK_CTS_ORDER
     funnel_cts_name = FUNNEL_CTS_NAME
     if zoom == 1:  # exclude ribosomal/poor quality
         stack_cts_order = stack_cts_order[:4]
         funnel_cts_name = funnel_cts_name[:4]
     pal = pal_set3[: len(stack_cts_order)]
 
@@ -1055,15 +1052,14 @@
         Output("read_length_slider", "min"),
         Output("read_length_slider", "max"),
         Output("read_length_slider", "value"),
     ],
     [Input("dropdown_available_samples", "value"), Input("drop_unique", "value")],
 )
 def read_length_min_max(sample, unique):
-
     unique = ast.literal_eval(unique)
     m_unique = read_length_distributions.is_unique == unique
     m_sample = read_length_distributions.Sample == sample
     df = read_length_distributions[m_sample & m_unique]
     min_length = df.length.min()
     max_length = df.length.max()
 
@@ -1077,15 +1073,14 @@
         Input("dropdown_available_samples", "value"),
         Input("drop_unique", "value"),
         Input("toggle_log", "value"),
         Input("read_length_slider", "value"),
     ],
 )
 def length_bars(sample, unique, log_y, slider):
-
     unique = ast.literal_eval(unique)
     pal = pal_bars[2]
     if unique:
         pal = pal_bars[1]
     color_discrete_map = {"Non-periodic": pal, "Periodic": pal_bars[0]}
 
     m_unique = read_length_distributions.is_unique == unique
@@ -1129,15 +1124,14 @@
     ],
     [
         Input("length_bars_fig", "hoverData"),
         Input("dropdown_available_samples", "value"),
     ],
 )
 def read_length_metagene_bars(hoverData, sample):
-
     # TODO: how to get a default value, i.e. not hoverData['points'][0] is None?
 
     m_sample = lengths_and_offsets.Sample == sample
     sample_lengths_and_offsets = lengths_and_offsets[m_sample]
 
     if hoverData is None:
         length = sample_lengths_and_offsets.length.values.min()
@@ -1267,15 +1261,14 @@
 
     return (out_url, text)
 
 
 # percentage of reads in each frame
 @app.callback(Output("stacked_frames_fig", "figure"), Input("drop_samples", "value"))
 def stacked_frames(selected):
-
     selected_samples = selected.split(",")
     df = frame_counts[frame_counts.Sample.isin(selected_samples)]
 
     fig = (
         px.bar(
             df,
             x="Sample",
@@ -1301,15 +1294,14 @@
         Input("window_downstream", "value"),
         Input("window_step", "value"),
         Input("metagene_type", "value"),
         Input("drop_samples", "value"),
     ],
 )
 def all_metagenes(window_upstream, window_downstream, step, plot, selected):
-
     # instead of defining a default value and override placeholder...
     if window_upstream is None:
         window_upstream = 3
     if window_downstream is None:
         window_downstream = 3
     if step is None:
         step = 1
```

### Comparing `rpbp-3.0.1/src/rpbp/analysis/profile_construction/get_all_read_filtering_counts.py` & `rpbp-3.0.2/src/rpbp/analysis/profile_construction/get_all_read_filtering_counts.py`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/analysis/profile_construction/summarize_rpbp_profile_construction.py` & `rpbp-3.0.2/src/rpbp/analysis/profile_construction/summarize_rpbp_profile_construction.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
 from rpbp.defaults import default_num_cpus, metagene_options
 
 logger = logging.getLogger(__name__)
 
 
 def get_read_filtering_summary(filename, args):
-
     overwrite_str = ""
     if args.overwrite:
         overwrite_str = "--overwrite"
 
     logging_str = logging_utils.get_logging_options_string(args)
 
     cpus_str = "--num-cpus {}".format(args.num_cpus)
@@ -44,15 +43,14 @@
     out_files = [filename]
     shell_utils.call_if_not_exists(
         cmd, out_files, in_files=in_files, overwrite=args.overwrite, call=True
     )
 
 
 def get_read_length_distributions(sample, config, is_unique, note, args):
-
     logging_str = logging_utils.get_logging_options_string(args)
     cpus_str = "--num-cpus {}".format(args.num_cpus)
 
     # distribution for this sample
     read_length_distribution = filenames.get_riboseq_read_length_distribution(
         config["riboseq_data"], sample, note=note
     )
@@ -79,28 +77,26 @@
     out_files = [read_length_distribution]
     shell_utils.call_if_not_exists(
         cmd, out_files, in_files=in_files, overwrite=args.overwrite, call=True
     )
 
 
 def collect_all_read_length_distributions(sample, config, note, args):
-
     # distribution for this sample
     read_length_distribution = filenames.get_riboseq_read_length_distribution(
         config["riboseq_data"], sample, note=note
     )
     read_length_distribution = pd.read_csv(read_length_distribution)
     ret = pd.pivot_table(
         read_length_distribution, values="count", columns="length", index="basename"
     )
     return ret
 
 
 def collect_lengths_and_offsets(sample, config, is_unique, note, args):
-
     # not only the periodic lengths and offsets, but all
     # and add status information based on filters
 
     min_metagene_profile_count = config.get(
         "min_metagene_profile_count", metagene_options["min_metagene_profile_count"]
     )
     min_bf_mean = config.get(
@@ -119,15 +115,14 @@
     offsets_df = pd.read_csv(periodic_offsets)
 
     min_read_length = int(offsets_df["length"].min())
     max_read_length = int(offsets_df["length"].max())
 
     lengths, offsets, statuses = [], [], []
     for length in range(min_read_length, max_read_length + 1):
-
         # check which offset is used
         # select the row for this length
         mask_length = offsets_df["length"] == length
 
         # TODO: this is sometimes length 0. why?
         if sum(mask_length) == 0:
             continue
@@ -190,15 +185,14 @@
         note=note,
     )
 
     return profiles
 
 
 def get_frame_counts(sample, config, is_unique, note):
-
     msg = "{}: extracting frame counts".format(sample)
     logger.info(msg)
 
     mtx = get_profile(sample, config, is_unique, note)
 
     # we don't need to load as sparse matrix, use numpy and
     # mask based on ORF offset (2nd column), taking into account that
@@ -217,15 +211,14 @@
 
     ret = {"sample": sample, "frame": frame1, "frame+1": frame2, "frame+2": frame3}
 
     return pd.Series(ret)
 
 
 def create_fastqc_reports(sample_data, config, note, is_unique, args):
-
     sample, raw_data = sample_data
     msg = "{}: creating fastqc reports".format(sample)
     logger.info(msg)
 
     # first get the filenames
     without_adapters = filenames.get_without_adapters_fastq(
         config["riboseq_data"], sample, note=note
@@ -505,15 +498,14 @@
         sep=",",
         header=True,
         do_not_compress=False,
         quoting=csv.QUOTE_NONE,
     )
 
     if args.create_fastqc_reports:
-
         msg = "Calling FastQC..."
         logger.info(msg)
 
         parallel.apply_parallel_iter(
             config["riboseq_samples"].items(),
             args.num_cpus,
             create_fastqc_reports,
```

### Comparing `rpbp-3.0.1/src/rpbp/analysis/profile_construction/visualize_metagene_profile_bayes_factor.py` & `rpbp-3.0.2/src/rpbp/analysis/profile_construction/visualize_metagene_profile_bayes_factor.py`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/analysis/proteomics/filter_nonunique_peptide_matches.py` & `rpbp-3.0.2/src/rpbp/analysis/proteomics/filter_nonunique_peptide_matches.py`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/analysis/proteomics/get_all_orf_peptide_matches.py` & `rpbp-3.0.2/src/rpbp/analysis/proteomics/get_all_orf_peptide_matches.py`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/analysis/proteomics/get_orf_peptide_matches.py` & `rpbp-3.0.2/src/rpbp/analysis/proteomics/get_orf_peptide_matches.py`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/dashboard/assets/logo-rpbp.png` & `rpbp-3.0.2/src/rpbp/analysis/profile_construction/dashboard/assets/logo-rpbp.png`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/dashboard/assets/schematic.png` & `rpbp-3.0.2/src/rpbp/analysis/rpbp_predictions/dashboard/assets/schematic.png`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/dashboard/assets/style.css` & `rpbp-3.0.2/src/rpbp/analysis/profile_construction/dashboard/assets/style.css`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/dashboard/rpbp_predictions_dashboard.py` & `rpbp-3.0.2/src/rpbp/analysis/rpbp_predictions/dashboard/rpbp_predictions_dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,44 +13,54 @@
 from pathlib import Path
 from dash import Dash, html, dcc, Input, Output, State, dash_table, ctx
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 
+import rpbp.ribo_utils.utils as ribo_utils
+
 from rpbp.defaults import orf_type_colors, orf_type_labels, orf_type_name_map
 
 # ------------------------------------------------------ Functions ------------------------------------------------------
 
 
+def parse_env(key):
+    return (
+        {"default": os.environ.get(key)} if os.environ.get(key) else {"required": True}
+    )
+
+
 def get_parser():
     parser = argparse.ArgumentParser(
         description="Launch a Dash app to visualize "
         "Ribo-seq ORF predicted with Rp-Bp."
     )
 
     parser.add_argument(
-        "config",
+        "--config",
+        "-c",
         type=str,
+        **parse_env("RPBP_CFG"),
         help="A YAML configuration file." "The same used to run the pipeline.",
     )
 
     parser.add_argument("--debug", "-d", action="store_true", help="Enable debug mode.")
 
     parser.add_argument("--host", type=str, default="localhost", help="Host.")
 
     parser.add_argument("--port", type=int, default=8050, help="Port number.")
 
-    args = parser.parse_args()
+    # args = parser.parse_args()
+    args, unkn = parser.parse_known_args()
 
     return args.config, args.debug, args.host, args.port
 
 
 def fmt_tooltip(row):
-
     conditions = row.condition.split("|")
     bayes_factor_mean = row.bayes_factor_mean.split("|")
     bayes_factor_var = row.bayes_factor_var.split("|")
     profile_sum = row.profile_sum.split("|")
     in_frame = row.in_frame.split("|")
 
     it = zip(conditions, bayes_factor_mean, bayes_factor_var, profile_sum, in_frame)
@@ -59,23 +69,21 @@
     fmt.append("| :-------- | :-----: | :----: | :-----: | -------: |")
     for cond, bfm, bfv, ps, inf in it:
         fmt.append(f"| {cond} | {bfm} | {bfv} | {ps} | {inf}% |")
     return "\n".join(fmt)
 
 
 def get_orf_type_counts(condition):
-
     orf_type_counts = condition.groupby(["orf_type", "strand"]).size()
     orf_type_counts = orf_type_counts.reset_index(name="count")
 
     return orf_type_counts
 
 
 def filter_sort_table(filter_query, sort_by):
-
     filtering_expressions = filter_query.split(" && ")
     df = display_table.copy()
 
     # first apply filtering
     for filter_part in filtering_expressions:
         col_name, operator, filter_value = split_filter_part(filter_part)
 
@@ -144,24 +152,35 @@
     **intORF**: Translation event within a CDS (in- or out-of-frame)\n
     **uORF/uoORF**: Translation event in the 5' untranslated region (UTR) of or partially overlapping an annotated protein-coding gene\n
     **dORF/doORF**: Translation event in the 3' untranslated region (UTR) of or partially overlapping an annotated protein-coding gene\n
     **ncORF**: Translation event in an RNA annotated as non-coding (lncRNA, pseudogene, *etc.*)\n
     **Novel**: Translation event inter- or intragenic (only when Rp-Bp is run with a *de novo* assembly)
     """
 
+# ribo_utils._return_key_dict
+sample_name_map = ribo_utils.get_sample_name_map(
+    config
+)  # default to riboseq_samples.keys()
+condition_name_map = ribo_utils.get_condition_name_map(
+    config
+)  # default to riboseq_biological_replicates.keys()
+
 col_rev = {v: k for k, v in orf_type_colors.items()}
 row_col = {}
 for orf_type, labels in orf_type_labels.items():
     types = [orf_type_name_map[label] for label in labels]
     for t in types:
         row_col[t] = col_rev[orf_type]
 
 # *** load/wrangle data
 orfs = pd.read_csv(config["predicted_orfs"], sep="\t", low_memory=False)  # bed_utils
 orfs.columns = orfs.columns.str.replace("#", "")
+orfs["condition"] = orfs["condition"].apply(lambda x: sample_name_map[x])
+# apply condition name map, in case we also have conditions
+orfs["condition"] = orfs["condition"].apply(lambda x: condition_name_map[x])
 orfs["orf_len"] = orfs["orf_len"] / 3
 orfs["profile_sum"] = orfs[["x_1_sum", "x_2_sum", "x_3_sum"]].sum(axis=1)
 orfs["profile_sum"] = orfs["profile_sum"].astype(int)
 orfs["in_frame"] = orfs["x_1_sum"].div(orfs["profile_sum"].values) * 100
 orfs["in_frame"] = orfs["in_frame"].apply(np.round).astype(int)
 orfs["bayes_factor_mean"] = orfs["bayes_factor_mean"].apply(np.round).astype(int)
 orfs["bayes_factor_var"] = orfs["bayes_factor_var"].apply(np.round).astype(int)
@@ -434,18 +453,26 @@
     "outerRadius": circos_outerRadius,
     "color": row_col[orf_type_default],
 }  # "tooltipContent": {"name": "all"}
 
 # ------------------------------------------------------ APP ------------------------------------------------------
 
 app = dash.Dash(__name__)
+server = app.server
+
+# we need this for serving the app
+base_url = (
+    os.environ["DASH_URL_BASE_PATHNAME"]
+    if "DASH_URL_BASE_PATHNAME" in os.environ
+    else ""
+)
 
 
-@app.server.route("/data/<configval>", defaults={"suffix": None})
-@app.server.route("/data/<configval>/<suffix>")
+@app.server.route(f"{base_url}/data/<configval>", defaults={"suffix": None})
+@app.server.route(f"{base_url}/data/<configval>/<suffix>")
 def config_data(configval, suffix):
     """Serve the file specified for the given key in the configuration.
     Potentially apply a suffix for derived files like an index.
     """
 
     # Extract the filename from configuration
     filename = config[configval]
@@ -870,15 +897,14 @@
 
 @app.callback(
     Output("circos_fig", "tracks"),
     Input("drop_orf_types", "value"),
     State("circos_fig", "tracks"),
 )
 def hist_orf_type(value, current):
-
     tracks_config = {
         "innerRadius": circos_innerRadius,
         "outerRadius": circos_outerRadius,
         "color": row_col[value],
     }
     current[0].update(
         data=circos_graph_data[f"histogram_{value}"],
@@ -905,15 +931,14 @@
         Input("main_datatable", "sort_by"),
         Input("main_datatable", "filter_query"),
     ],
     # State("main_datatable", "data"),
     prevent_initial_call=True,
 )
 def func(n_clicks, sort_by, filter_query):  # table_data
-
     # df = pd.DataFrame.from_dict(table_data)
     changed_inputs = [x["prop_id"] for x in ctx.triggered]
     if "btn_csv.n_clicks" in changed_inputs:
         df = filter_sort_table(filter_query, sort_by)
         df.drop(columns="orf_info", inplace=True)
         return dcc.send_data_frame(df.to_csv, "selected-orfs.csv", index=False)
```

### Comparing `rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/summarize_rpbp_predictions.py` & `rpbp-3.0.2/src/rpbp/analysis/rpbp_predictions/summarize_rpbp_predictions.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,14 @@
     fraction,
     reweighting_iterations,
     is_unique,
     is_filtered,
     config,
     ftype="predictions",
 ):
-
     if is_sample:
         try:
             lengths, offsets = ribo_utils.get_periodic_lengths_and_offsets(
                 config, name, is_unique=is_unique, default_params=metagene_options
             )
         except FileNotFoundError:
             msg = (
@@ -165,15 +164,14 @@
     else:
         bins[-2] = size
         bins = np.delete(bins, -1)
     return pd.cut(x["start"].values, bins, right=False)
 
 
 def get_circos_graph(orfs, sub_folder, config, args):
-
     orf_types = orfs.orf_type.unique()
     df = orfs.drop_duplicates(subset=bed_utils.bed12_field_names).copy()
     df.rename(columns={"seqname": "block_id"}, inplace=True)
     df.reset_index(drop=True, inplace=True)
 
     # filter chromosomes to show
     match = r"|".join(args.circos_show_chroms)
@@ -238,15 +236,14 @@
     note,
     fraction,
     reweighting_iterations,
     is_unique,
     is_filtered,
     config,
 ):
-
     orfs_file = get_predictions_file(
         name,
         is_sample,
         note,
         fraction,
         reweighting_iterations,
         is_unique,
@@ -257,15 +254,14 @@
     orfs = orfs[FIELD_NAMES]
     orfs["condition"] = sample_name_map[name]
 
     return orfs
 
 
 def get_bed_blocks(row):
-
     # convert genomic coordinates to bed blocks
     # ad-hoc for standardized ORFs
 
     starts = row.starts.split(";")
     ends = row.ends.split(";")
     # coordinates include stop codon
     # a few ORFs have a stop codon overlapping 2 exons
@@ -294,15 +290,14 @@
     coords["start"] = int(starts[0]) - 1
     coords["end"] = int(ends[-1])
 
     return coords
 
 
 def get_standardized_orfs(filen, sheet):
-
     # ad-hoc for standardized ORFs
 
     colmap = [
         {"chrm": "seqname", "orf_name": "PHASE I ORFs"},
         {"chrm": "seqname", "orf_name": "SS ORFs"},
     ]
     col = colmap[sheet - 2]["orf_name"]
@@ -314,15 +309,14 @@
     standardized_orfs = standardized_orfs.join(blocks)
     standardized_orfs.rename(columns=colmap[sheet - 2], inplace=True)
 
     return col, standardized_orfs[standardized_fields]
 
 
 def _create_figures(name_pretty_name_is_sample, config, args):
-
     name, pretty_name, is_sample = name_pretty_name_is_sample
 
     is_unique = not config.get("keep_riboseq_multimappers", False)
     note = config.get("note", None)
     fraction = config.get("smoothing_fraction", None)
     reweighting_iterations = config.get("smoothing_reweighting_iterations", None)
 
@@ -400,15 +394,14 @@
     out_files = orf_type_profiles_forward + orf_type_profiles_reverse
     shell_utils.call_if_not_exists(
         cmd, out_files, in_files=in_files, overwrite=args.overwrite
     )
 
 
 def create_all_figures(config, sample_name_map, condition_name_map, args):
-
     is_sample = True
     sample_names = sorted(config["riboseq_samples"].keys())
     samples = [(name, sample_name_map[name], is_sample) for name in sample_names]
 
     conditions = []
     if not args.no_replicates:
         is_sample = False
@@ -690,14 +683,18 @@
             is_annotated=False,
             is_de_novo=True,
         )
         cols = ["id", "biotype", "gene_id", "gene_name", "gene_biotype"]
         bed_df_dn = bed_utils.read_bed(transcript_bed_dn, low_memory=False)[cols]
         bed_df_dn.rename(columns={"id": "transcript_id"}, inplace=True)
         bed_df = pd.concat([bed_df, bed_df_dn])
+        # now we have the problem that bed_df may contain duplicate transcript ids
+        # for the purpose of display/annotation, we favour the annotated one
+        # in general the novel transcript will be a variant (matched introns, extension, etc.)
+        bed_df.drop_duplicates(subset=["transcript_id"], inplace=True)
 
     labeled_orfs = filenames.get_labels(
         config["genome_base_path"], config["genome_name"], note=orf_note
     )
     cols = ["id", "orf_type", "transcripts"]
     labels_df = bed_utils.read_bed(labeled_orfs)[cols]
```

### Comparing `rpbp-3.0.1/src/rpbp/analysis/rpbp_predictions/visualize_orf_type_metagene_profiles.py` & `rpbp-3.0.2/src/rpbp/analysis/rpbp_predictions/visualize_orf_type_metagene_profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 default_image_type = "eps"
 default_title = ""
 default_min_profile = 5
 default_max_orfs = 10000
 
 
 def get_windows(profile):
-
     profile = profile / np.max(profile)
 
     orf_len = len(profile)
     if orf_len < 42:
         # we would return first window and exit
         first_window = profile[:21]
         return (first_window, None, None)
@@ -62,15 +61,14 @@
     if sum(profile) < min_profile:
         return None
 
     return profile
 
 
 def plot_windows(windows, title, out):
-
     if len(windows) == 0:
         msg = "Did not find any windows for: {}".format(title)
         logger.warning(msg)
         return
 
     windows_np = np.array(windows)
     first_windows = windows_np[:, 0]
```

### Comparing `rpbp-3.0.1/src/rpbp/defaults.py` & `rpbp-3.0.2/src/rpbp/defaults.py`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/models/nonperiodic/no-periodicity.stan` & `rpbp-3.0.2/src/rpbp/models/nonperiodic/no-periodicity.stan`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/models/nonperiodic/start-high-high-low.stan` & `rpbp-3.0.2/src/rpbp/models/nonperiodic/start-high-high-low.stan`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/models/nonperiodic/start-high-low-high.stan` & `rpbp-3.0.2/src/rpbp/models/nonperiodic/start-high-low-high.stan`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/models/periodic/start-high-low-low.stan` & `rpbp-3.0.2/src/rpbp/models/periodic/start-high-low-low.stan`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/models/translated/periodic-gaussian-mixture.stan` & `rpbp-3.0.2/src/rpbp/models/translated/periodic-gaussian-mixture.stan`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/models/untranslated/gaussian-naive-bayes.stan` & `rpbp-3.0.2/src/rpbp/models/untranslated/gaussian-naive-bayes.stan`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/orf_profile_construction/create_base_genome_profile.py` & `rpbp-3.0.2/src/rpbp/orf_profile_construction/create_base_genome_profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -249,19 +249,34 @@
         call=call,
         keep_delete_files=keep_delete_files,
         to_delete=to_delete,
     )
 
     # rename STAR output to that expected by the pipeline
     genome_star_bam = Path(genome_star_bam)
-    genome_star_bam.replace(genome_sorted_bam)
+    # otherwise check and replace
+    if genome_star_bam.is_file():
+        if not Path(genome_sorted_bam).is_file() or args.overwrite:
+            genome_star_bam.replace(genome_sorted_bam)
+            msg = f"Replacing {genome_star_bam.as_posix()} by {genome_sorted_bam}"
+            logger.info(msg)
+        else:
+            msg = (
+                f"Both files {genome_star_bam.as_posix()} and {genome_sorted_bam} "
+                f"already exist! You should re-run using [--overwrite] to avoid "
+                f"data corruption!"
+            )
+            logger.error(msg)
+    else:
+        # re-run w/o overwrite
+        msg = f"The file {genome_sorted_bam} already exists. Continuing..."
+        logger.warning(msg)
 
     # create the bamtools index
-    cmd = "samtools index -b {}".format(genome_sorted_bam)
-    shell_utils.check_call(cmd, call=call)
+    bam_utils.index_bam_file(genome_sorted_bam, args)
 
     # check if we want to keep multimappers
     if config.get("keep_riboseq_multimappers", False):
         return
 
     # remove multimapping reads from the genome file
     tmp_str = ""
```

### Comparing `rpbp-3.0.1/src/rpbp/orf_profile_construction/create_orf_profiles.py` & `rpbp-3.0.2/src/rpbp/orf_profile_construction/create_orf_profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 
 default_models_base = filenames.get_default_models_base()
 
 logger = logging.getLogger(__name__)
 
 
 def main():
-
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         description="""This script runs all of the processing necessary to
         produce the signals used for ORF translation prediction. In particular, it creates the
         metagene profiles, selected the periodic fragments and generate the ORF profiles.""",
     )
```

### Comparing `rpbp-3.0.1/src/rpbp/orf_profile_construction/estimate_metagene_profile_bayes_factors.py` & `rpbp-3.0.2/src/rpbp/orf_profile_construction/estimate_metagene_profile_bayes_factors.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 default_position_field = "position"
 default_count_field = "count"
 
 
 def estimate_marginal_likelihoods(
     signal, periodic_models, nonperiodic_models, iterations, chains, seed
 ):
-
     # construct the input for the models
     x_1 = signal[0::3]
     x_2 = signal[1::3]
     x_3 = signal[2::3]
     T = len(x_1)
 
     very_high_prior_location = max(signal)
@@ -89,15 +88,14 @@
         for nm in nonperiodic_models
     ]
 
     return (bft_periodic, bft_nonperiodic)
 
 
 def estimate_profile_bayes_factors(profile, args):
-
     # logging
     cmdstanpy_logger.disabled = True
     if args.enable_ext_logging:
         cmdstanpy_logger.disabled = False
 
     length = profile["length"].iloc[0]
```

### Comparing `rpbp-3.0.1/src/rpbp/orf_profile_construction/extract_metagene_profiles.py` & `rpbp-3.0.2/src/rpbp/orf_profile_construction/extract_metagene_profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,28 +30,26 @@
 default_start_upstream = 300
 default_start_downstream = 300
 default_end_upstream = 300
 default_end_downstream = 300
 
 
 def get_interval_df(start, end, seqname, strand):
-
     interval_df = pd.DataFrame()
     interval_df["start"] = start
     interval_df["end"] = end
     interval_df["seqname"] = seqname
     interval_df["strand"] = strand
     interval_df["id"] = "."
     interval_df["score"] = 0
 
     return interval_df
 
 
 def get_length_strand_profiles(matches, profile_length):
-
     init = lambda: np.zeros(profile_length, int)
     length_strand_profiles = collections.defaultdict(init)
 
     for match in matches:
         position_info = match.position_info
 
         relative_offset = int(match.relative_offset)
@@ -64,15 +62,14 @@
 
     return length_strand_profiles
 
 
 def get_metagene_profile_df(
     length, type_label, length_strand_profiles, upstream, downstream
 ):
-
     reverse_metagene_profile = length_strand_profiles[(length, "-")]
     forward_metagene_profile = length_strand_profiles[(length, "+")]
 
     metagene_profile = forward_metagene_profile + reverse_metagene_profile[::-1]
 
     if sum(metagene_profile) == 0:
         return None
@@ -85,15 +82,14 @@
     metagene_profile_df["type"] = type_label
     metagene_profile_df["length"] = length
 
     return metagene_profile_df
 
 
 def main():
-
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         description="""This script extracts the metagene profile
         from reads in a BAM file, possibly filtering by length.""",
     )
 
     parser.add_argument("bam", help="The bam file")
```

### Comparing `rpbp-3.0.1/src/rpbp/orf_profile_construction/extract_orf_profiles.py` & `rpbp-3.0.2/src/rpbp/orf_profile_construction/extract_orf_profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
 # --num-exons is not used in the the Rp-Bp pipeline
 # --seqname-prefix can be overridden via config arguments, but not
 # specified in defaults, as mostly unused
 
 
 def get_p_site_intersections(seqname, strand, p_sites, exons_df):
-
     # only the things in the right direction, etc.
     m_exons_seqname = exons_df["seqname"] == seqname
     m_p_sites_seqname = p_sites["seqname"] == seqname
 
     m_exons_strand = exons_df["strand"] == strand
     m_p_sites_strand = p_sites["strand"] == strand
```

### Comparing `rpbp-3.0.1/src/rpbp/orf_profile_construction/select_periodic_offsets.py` & `rpbp-3.0.2/src/rpbp/orf_profile_construction/select_periodic_offsets.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import pbiotools.misc.logging_utils as logging_utils
 import pbiotools.misc.pandas_utils as pandas_utils
 
 logger = logging.getLogger(__name__)
 
 
 def get_most_periodic_offset(profile_df):
-
     # mask_largest_count = profile_df['profile_sum'] == profile_df['profile_sum'].max()
     # largest_count_row = profile_df[mask_largest_count].iloc[0]
     m_highest_peak = profile_df["profile_peak"] == profile_df["profile_peak"].max()
     highest_peak_row = profile_df[m_highest_peak].iloc[0]
 
     length = highest_peak_row["length"]
```

### Comparing `rpbp-3.0.1/src/rpbp/reference_preprocessing/extract_orf_coordinates.py` & `rpbp-3.0.2/src/rpbp/reference_preprocessing/extract_orf_coordinates.py`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/reference_preprocessing/label_orfs.py` & `rpbp-3.0.2/src/rpbp/reference_preprocessing/label_orfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,29 +327,27 @@
     )
 
     # For standard assembly, we also need to make sure that
     # all extended matches are fully contained within the
     # transcript structure (i.e start upstream but otherwise
     # have the same structure).
     if args.nonoverlapping_label is None:
-
         transcript_matches = bed_utils.get_bed_overlaps(
             annotated_exons, extracted_orf_exons, min_b_overlap=1
         )
         transcript_match_pairs = {(m.a_info, m.b_info) for m in transcript_matches}
 
         extended_match_ids = {
             m.b_info
             for m in extended_matches
             if (m.a_info, m.b_info) in transcript_match_pairs
             and (m.a_info, m.b_info) in canonical_extracted_matching_ends
         }
 
     else:
-
         extended_match_ids = {
             m.b_info
             for m in extended_matches
             if (m.a_info, m.b_info) in canonical_extracted_matching_ends
         }
 
     m_extended_matches = extracted_orf_exons["id"].isin(extended_match_ids)
@@ -410,15 +408,14 @@
     # sense overlapping transcripts, it is assigned by default to the downstream overlap.
     # For de novo, everything is labeled as overlap.
 
     leader_match_pairs = {(m.a_info, m.b_info) for m in leader_matches}
     trailer_match_pairs = {(m.a_info, m.b_info) for m in trailer_matches}
 
     if args.nonoverlapping_label is None:
-
         # For standard assembly, we also need to make sure that
         # all overlap matches are fully contained within the
         # transcript structure.
         transcript_matches = bed_utils.get_bed_overlaps(
             annotated_exons, extracted_orf_exons, min_b_overlap=1
         )
 
@@ -487,15 +484,14 @@
         msg = (
             f"Found {len(trailer_overlap_ids)} three_prime_overlap ORFs "
             f"labeled as {label}"
         )
         logger.info(msg)
 
     else:
-
         overlap_ids = {m.b_info for m in out_of_frame_matches}
         overlap_ids |= {m.b_info for m in leader_matches}
         overlap_ids |= {m.b_info for m in trailer_matches}
 
         m_overlap_matches = extracted_orf_exons["id"].isin(overlap_ids)
         extracted_orf_exons = extracted_orf_exons[~m_overlap_matches]
```

### Comparing `rpbp-3.0.1/src/rpbp/reference_preprocessing/prepare_rpbp_genome.py` & `rpbp-3.0.2/src/rpbp/reference_preprocessing/prepare_rpbp_genome.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 import sys
 import yaml
 import logging
 import argparse
 
 from pathlib import Path
 
+import pandas as pd
+
 import pbiotools.misc.logging_utils as logging_utils
 import pbiotools.misc.shell_utils as shell_utils
 import pbiotools.misc.slurm as slurm
 import pbiotools.misc.utils as utils
 
 import pbiotools.utils.bed_utils as bed_utils
 import pbiotools.utils.pgrm_utils as pgrm_utils
@@ -34,14 +36,19 @@
     default_start_codons,
     default_stop_codons,
 )
 
 logger = logging.getLogger(__name__)
 
 
+class DuplicateIdsError(Exception):
+    def __init__(self, message):
+        self.message = message
+
+
 def get_orfs(gtf, args, config, is_annotated=False, is_de_novo=False):
     """Process a GTF file into its ORFs."""
 
     call = not args.do_not_call
     chr_name_file = os.path.join(config["star_index"], "chrName.txt")
     chr_name_str = "--chr-name-file {}".format(chr_name_file)
 
@@ -329,19 +336,28 @@
         orfs_files_str = " ".join(orfs_files)
         msg = "Concatenating files. Output file: {}; Input files: {}".format(
             orfs_genomic, orfs_files_str
         )
         logger.info(msg)
 
         if call:
-            concatenated_bed = bed_utils.concatenate(orfs_files, sort_bed=True)
-            concatenated_bed["orf_num"] = range(len(concatenated_bed))
+            concatenated_orfs = bed_utils.concatenate(orfs_files, sort_bed=True)
+            # this can happen... and is not currently well handled
+            if not concatenated_orfs.id.is_unique:
+                msg = (
+                    "Duplicate ORF ids were found when merging annotated and de novo ORFs. "
+                    "This is due to matching transcript ids and start/stop boundaries. "
+                    "Check you de novo annotation, and remove (or rename) these transcripts."
+                )
+                logger.error(msg)
+                raise DuplicateIdsError(msg)
+            concatenated_orfs["orf_num"] = range(len(concatenated_orfs))
             additional_columns = ["orf_num", "orf_len"]
             fields = bed_utils.bed12_field_names + additional_columns
-            bed_utils.write_bed(concatenated_bed[fields], orfs_genomic)
+            bed_utils.write_bed(concatenated_orfs[fields], orfs_genomic)
         else:
             msg = "Skipping concatenation due to --call value"
             logger.info(msg)
 
         de_novo_exons_file = filenames.get_exons(
             config["genome_base_path"],
             config["genome_name"],
@@ -355,17 +371,17 @@
         exons_files_str = " ".join(exons_files)
         msg = "Concatenating files. Output file: {}; Input files: {}".format(
             exons_file, exons_files_str
         )
         logger.info(msg)
 
         if call:
-            concatenated_bed = bed_utils.concatenate(exons_files, sort_bed=True)
+            concatenated_exons = bed_utils.concatenate(exons_files, sort_bed=True)
             fields = bed_utils.bed6_field_names + ["exon_index", "transcript_start"]
-            bed_utils.write_bed(concatenated_bed[fields], exons_file)
+            bed_utils.write_bed(concatenated_exons[fields], exons_file)
         else:
             msg = "Skipping concatenation due to --call value"
             logger.info(msg)
 
         de_novo_labeled_orfs = filenames.get_labels(
             config["genome_base_path"],
             config["genome_name"],
@@ -380,16 +396,25 @@
         msg = "Concatenating files. Output file: {}; Input files: {}".format(
             labeled_orfs, label_files_str
         )
         logger.info(msg)
 
         if call:
             # not a BED file
-            concatenated_bed = bed_utils.concatenate(label_files, sort_bed=False)
-            bed_utils.write_bed(concatenated_bed, labeled_orfs)
+            concatenated_labels = bed_utils.concatenate(label_files, sort_bed=False)[
+                ["id", "orf_type", "transcripts"]
+            ]
+            # make sure the orf numbering is the same
+            concatenated_labels = pd.merge(
+                concatenated_labels,
+                concatenated_orfs[["id", "orf_num"]],
+                how="left",
+                on="id",
+            )
+            bed_utils.write_bed(concatenated_labels, labeled_orfs)
         else:
             msg = "Skipping concatenation due to --call value"
             logger.info(msg)
 
         # concat the annotations to inform STAR
         gtf_file = filenames.get_gtf(config)
         star_files_str = " ".join([config["gtf"], config["de_novo_gtf"]])
```

### Comparing `rpbp-3.0.1/src/rpbp/ribo_utils/compile_rpbp_models.py` & `rpbp-3.0.2/src/rpbp/ribo_utils/compile_rpbp_models.py`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/ribo_utils/filenames.py` & `rpbp-3.0.2/src/rpbp/ribo_utils/filenames.py`

 * *Files 8% similar despite different names*

```diff
@@ -102,15 +102,14 @@
     is_unique=False,
     fraction=None,
     reweighting_iterations=None,
     is_chisq=False,
     is_filtered=False,
     note=None,
 ):
-
     unique = get_unique_string(is_unique)
     l = get_length_string(length)
     o = get_offset_string(offset)
     chisq = get_chisq_string(is_chisq)
     n = get_note_string(note)
     f = get_fraction_string(fraction)
     r = get_reweighting_iterations_string(reweighting_iterations)
@@ -118,22 +117,20 @@
 
     fn = "".join([name, n, unique, l, o, f, r, chisq, fi])
 
     return os.path.join(riboseq_base, sub_folder, fn)
 
 
 def get_riboseq_bam_base(riboseq_base, name, **kwargs):
-
     bam_base = get_riboseq_base(riboseq_base, name, "without-rrna-mapping", **kwargs)
 
     return bam_base
 
 
 def get_riboseq_bam(riboseq_base, name, **kwargs):
-
     s = get_riboseq_bam_base(riboseq_base, name, **kwargs)
     s = s + ".bam"
     return s
 
 
 def get_riboseq_bam_fastqc_path(riboseq_data):
     return os.path.join(riboseq_data, "without-rrna-mapping", "fastqc")
@@ -143,15 +140,14 @@
     riboseq_data,
     name,
     length=None,
     is_unique=False,
     note=None,
     is_chisq=False,
 ):
-
     unique = get_unique_string(is_unique)
     l = get_length_string(length)
     n = get_note_string(note)
     c = get_chisq_string(is_chisq)
     name = "{}{}{}{}{}".format(name, n, unique, l, c)
 
     fastqc_folder = "{}_fastqc".format(name)
@@ -162,53 +158,48 @@
 
 def get_bed(
     base_path,
     name,
     is_annotated=False,
     is_de_novo=False,
 ):
-
     c = get_annotated_string(is_annotated)
     d = get_de_novo_string(is_de_novo)
     fn = "{}{}{}.bed.gz".format(name, c, d)
     return os.path.join(base_path, fn)
 
 
 def get_riboseq_bayes_factors(riboseq_base, name, **kwargs):
-
     s = get_riboseq_base(riboseq_base, name, "orf-predictions", **kwargs)
 
     s = s + ".bayes-factors.bed.gz"
     return s
 
 
 # c
 
 
 def get_riboseq_cell_type_protein(riboseq_base, name, **kwargs):
-
     s = get_riboseq_base(riboseq_base, name, "cell-types", **kwargs)
     s = s + ".predicted-orfs.protein.fa"
     return s
 
 
 # e
 
 
 def get_exons(base_path, name, is_annotated=False, is_de_novo=False, note=None):
-
     note_str = get_note_string(note)
     c = get_annotated_string(is_annotated)
     d = get_de_novo_string(is_de_novo)
     fn = "{}.orfs-exons{}{}{}.bed.gz".format(name, c, d, note_str)
     return os.path.join(base_path, "transcript-index", fn)
 
 
 def get_labels(base_path, name, is_annotated=False, is_de_novo=False, note=None):
-
     note_str = get_note_string(note)
     c = get_annotated_string(is_annotated)
     d = get_de_novo_string(is_de_novo)
     fn = "{}.orfs-labels{}{}{}.tab.gz".format(name, c, d, note_str)
     return os.path.join(base_path, "transcript-index", fn)
 
 
@@ -256,43 +247,39 @@
 
 # g
 
 
 def get_gtf(
     config,
 ):
-
     if "de_novo_gtf" in config:
         base_path = config["genome_base_path"]
         name = config["genome_name"]
         fn = f"{name}.gtf"
         return os.path.join(base_path, fn)
     else:
         return config["gtf"]
 
 
 # m
 
 
 def get_metagene_profile_image(base, name, image_type="eps", **kwargs):
-
     s = get_riboseq_base(base, name, "metagene-profiles", **kwargs)
     s = s + "." + image_type
     return s
 
 
 def get_metagene_profiles(riboseq_base, name, **kwargs):
-
     s = get_riboseq_base(riboseq_base, name, "metagene-profiles", **kwargs)
     s = s + ".metagene-profile.csv.gz"
     return s
 
 
 def get_metagene_profiles_bayes_factors(riboseq_base, name, **kwargs):
-
     s = get_riboseq_base(riboseq_base, name, "metagene-profiles", **kwargs)
     s = s + ".metagene-periodicity-bayes-factors.csv.gz"
     return s
 
 
 def get_default_models_base():
     import os
@@ -311,15 +298,14 @@
     models = [shlex.quote(m) for m in models]
     return models
 
 
 def get_metagene_profile_bayes_factor_image(
     riboseq_base, name, image_type="eps", **kwargs
 ):
-
     s = get_riboseq_base(riboseq_base, name, "metagene-profiles", **kwargs)
     s = s + ".bayes-factors." + image_type
     return s
 
 
 # o
 
@@ -340,15 +326,14 @@
     is_unique=False,
     fraction=None,
     reweighting_iterations=None,
     note=None,
     is_chisq=False,
     subfolder="orf-predictions",
 ):
-
     subfolder = os.path.join(subfolder, "plots")
     s = get_riboseq_base(
         riboseq_base,
         name,
         subfolder,
         length=length,
         offset=offset,
@@ -366,23 +351,21 @@
     return base_path + fn
 
 
 # p
 
 
 def get_periodic_offsets(riboseq_base, name, **kwargs):
-
     sub_folder = kwargs.pop("sub_folder", "metagene-profiles")
     s = get_riboseq_base(riboseq_base, name, sub_folder, **kwargs)
     s = s + ".periodic-offsets.csv.gz"
     return s
 
 
 def get_riboseq_peptide_matches(riboseq_base, name, peptide_name, **kwargs):
-
     n = "{}-{}".format(name, peptide_name)
 
     s = get_riboseq_base(riboseq_base, n, "peptide-matches", **kwargs)
     s = s + ".peptide-matches.csv.gz"
     return s
 
 
@@ -390,29 +373,26 @@
     sub_folder = kwargs.pop("sub_folder", "orf-predictions")
     base = get_riboseq_base(riboseq_base, name, sub_folder, **kwargs)
     loc = f"{base}.predicted-orfs.bed.gz"
     return loc
 
 
 def get_riboseq_predicted_orfs_dna(riboseq_base, name, **kwargs):
-
     s = get_riboseq_base(riboseq_base, name, "orf-predictions", **kwargs)
     s = s + ".predicted-orfs.dna.fa"
     return s
 
 
 def get_riboseq_predicted_orfs_protein(riboseq_base, name, **kwargs):
-
     s = get_riboseq_base(riboseq_base, name, "orf-predictions", **kwargs)
     s = s + ".predicted-orfs.protein.fa"
     return s
 
 
 def get_riboseq_profiles(riboseq_base, name, **kwargs):
-
     s = get_riboseq_base(riboseq_base, name, "orf-profiles", **kwargs)
     s = s + ".profiles.mtx.gz"
     return s
 
 
 # r
 
@@ -437,15 +417,14 @@
 
 def get_raw_data_fastqc_path(base_path):
     rdp = get_raw_data_path(base_path)
     return os.path.join(rdp, "fastqc")
 
 
 def get_raw_data_fastqc_data(base_path, filename):
-
     name = get_fastqc_name(filename)
     fastqc_folder = "{}_fastqc".format(name)
     rdp = get_raw_data_fastqc_path(base_path)
 
     p = os.path.join(rdp, fastqc_folder, "fastqc_data.txt")
     return p
 
@@ -463,15 +442,14 @@
 
 def get_transcript_fasta(
     base_path,
     name,
     is_annotated=False,
     is_de_novo=False,
 ):
-
     c = get_annotated_string(is_annotated)
     d = get_de_novo_string(is_de_novo)
     fn = "{}.transcripts{}{}.fa".format(name, c, d)
     return os.path.join(base_path, "transcript-index", fn)
 
 
 # w
```

### Comparing `rpbp-3.0.1/src/rpbp/ribo_utils/utils.py` & `rpbp-3.0.2/src/rpbp/ribo_utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,18 @@
 
 ###
 #   The following functions are helpful for parsing information out of the identifiers.
 ###
 
 
 def get_transcript_id(orf_id, sep="_"):
-
     return orf_id.split(sep)[0]
 
 
 def get_all_transcript_ids(orfs, sep="_", num_cpus=1, progress_bar=False):
-
     import pbiotools.misc.parallel as parallel
 
     transcript_ids = parallel.apply_parallel_iter(
         orfs["id"], num_cpus, get_transcript_id, sep, progress_bar=progress_bar
     )
 
     return transcript_ids
@@ -39,15 +37,14 @@
 
 ###
 #   The following functions are all used for parsing replicates, etc., from the config file.
 ###
 
 
 def get_riboseq_replicates(config):
-
     if "riboseq_biological_replicates" in config:
         if config["riboseq_biological_replicates"] is not None:
             msg = "Found 'riboseq_biological_replicates' key in config file"
             logger.info(msg)
 
             return config["riboseq_biological_replicates"]
 
@@ -127,15 +124,14 @@
 def get_periodic_lengths_and_offsets(
     config,
     name,
     do_not_call=False,
     is_unique=True,
     default_params=None,
 ):
-
     """This function applies a set of filters to metagene profiles to select those
     which are "periodic" based on the read counts and Bayes factor estimates.
 
     First, the function checks if the configuration file sets the
     'use_fixed_lengths' flag is set. If so, then the specified lengths and
     offsets are returned.
 
@@ -465,15 +461,14 @@
 
 
 def smooth_profile(
     profile,
     reweighting_iterations=translation_options["smoothing_reweighting_iterations"],
     fraction=translation_options["smoothing_fraction"],
 ):
-
     """This function smoothes the given ORF profile using the frame-specific
     approach. It assumes the profile is a dense numpy array and that any
     filtering due to differences of counts in reading frames, lengths, etc.,
     has already been performed.
 
     Please see the statsmodels.api.nonparametric.lowess documentation for
     more information about reweighting_iterations and fraction.
@@ -588,15 +583,14 @@
 
 def get_bf_filter(
     bf,
     min_bf_mean=translation_options["min_bf_mean"],
     max_bf_var=translation_options["max_bf_var"],
     min_bf_likelihood=translation_options["min_bf_likelihood"],
 ):
-
     """This function applies filters to the Bayes factor estimates to find all
     ORFs which should be predicted as translated. This does not consider the
     length and profile sums, so this filter would need to be combined with
     the get_base_filter filter to find the true set of predicted ORFs.
 
     Args:
         bf (pd.DataFrame) : a data frame containing the relevant ORF information
```

### Comparing `rpbp-3.0.1/src/rpbp/run_all_rpbp_instances.py` & `rpbp-3.0.2/src/rpbp/run_all_rpbp_instances.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,14 @@
         return
 
     # otherwise, we need to merge the replicates for each condition
     riboseq_replicates = ribo_utils.get_riboseq_replicates(config)
     merge_replicates_str = "--merge-replicates"
 
     for condition_name in sorted(riboseq_replicates.keys()):
-
         # then we predict the ORFs
         cmd = "predict-translated-orfs {} {} --num-cpus {} {} {} {} {} {}".format(
             args.config,
             condition_name,
             args.num_cpus,
             do_not_call_str,
             overwrite_str,
```

### Comparing `rpbp-3.0.1/src/rpbp/run_rpbp_pipeline.py` & `rpbp-3.0.2/src/rpbp/run_rpbp_pipeline.py`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/translation_prediction/estimate_orf_bayes_factors.py` & `rpbp-3.0.2/src/rpbp/translation_prediction/estimate_orf_bayes_factors.py`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,14 @@
     ret["bayes_factor_mean"] = ret["p_translated_mean"] - ret["p_background_mean"]
     ret["bayes_factor_var"] = ret["p_translated_var"] + ret["p_background_var"]
 
     return ret
 
 
 def get_all_bayes_factors(orfs):
-
     """This function calculates the Bayes' factor term for each region in regions. See the
     description of the script for the Bayes' factor calculations.
 
     Args:
         orfs (pd.DataFrame) : a set of orfs. The columns must include:
             orf_num
             exon_lengths
```

### Comparing `rpbp-3.0.1/src/rpbp/translation_prediction/merge_replicate_orf_profiles.py` & `rpbp-3.0.2/src/rpbp/translation_prediction/merge_replicate_orf_profiles.py`

 * *Files identical despite different names*

### Comparing `rpbp-3.0.1/src/rpbp/translation_prediction/predict_translated_orfs.py` & `rpbp-3.0.2/src/rpbp/translation_prediction/predict_translated_orfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
         note=note_str,
     )
 
     return profiles
 
 
 def main():
-
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         description=""""This script runs the second part of the pipeline:
         it estimate ORF Bayes factors using the ORF profiles, then make the final prediction set.""",
     )
 
     parser.add_argument("config", help="The (yaml) config file")
@@ -328,15 +327,14 @@
         call=call,
     )
 
     filters = [True]
     if args.write_unfiltered:
         filters.append(False)
     for is_filtered in filters:
-
         filtered_str = ""
         if is_filtered:
             filtered_str = "--select-longest-by-stop --select-best-overlapping"
 
         # now, select the ORFs (longest for each stop codon) which pass the prediction filters
         predicted_orfs = filenames.get_riboseq_predicted_orfs(
             config["riboseq_data"],
```

### Comparing `rpbp-3.0.1/src/rpbp/translation_prediction/select_final_prediction_set.py` & `rpbp-3.0.2/src/rpbp/translation_prediction/select_final_prediction_set.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 default_bf_var_field = "bayes_factor_var"
 default_profile_sum_field = "profile_sum"
 
 # --filtered-orf-types is not used in the the Rp-Bp pipeline
 
 
 def get_best_overlapping_orf(merged_ids, predicted_orfs):
-
     if len(merged_ids) == 1:
         m_id = predicted_orfs["id"] == merged_ids[0]
         return predicted_orfs[m_id].iloc[0]
 
     m_orfs = predicted_orfs["id"].isin(merged_ids)
 
     sorted_orfs = predicted_orfs[m_orfs].sort_values(
@@ -188,15 +187,14 @@
         use_chi_square=args.chi_square_only,
     )
 
     msg = "Number of selected ORFs: {}".format(len(predicted_orfs))
     logger.info(msg)
 
     if args.select_best_overlapping:
-
         msg = "Finding overlapping ORFs"
         logger.info(msg)
 
         merged_intervals = bed_utils.merge_all_intervals(predicted_orfs)
 
         msg = "Selecting best among overlapping ORFs"
         logger.info(msg)
```

### Comparing `rpbp-3.0.1/src/rpbp.egg-info/PKG-INFO` & `rpbp-3.0.2/src/rpbp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpbp
-Version: 3.0.1
+Version: 3.0.2
 Summary: Rp-Bp: Ribosome Profiling with Bayesian Predictions
 Author: Brandon Malone
 Maintainer-email: Etienne Boileau <boileau@uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/dieterich-lab/rp-bp
 Project-URL: Issues, https://github.com/dieterich-lab/rp-bp/issues
 Keywords: bioinformatics,riboseq,open reading frame discovery,translation
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rpbp Version: 3.0.1 Summary: Rp-Bp: Ribosome
+Metadata-Version: 2.1 Name: rpbp Version: 3.0.2 Summary: Rp-Bp: Ribosome
 Profiling with Bayesian Predictions Author: Brandon Malone Maintainer-email:
 Etienne Boileau
 uni-heidelberg.de> License: MIT Project-URL: Github, https://github.com/
 dieterich-lab/rp-bp Project-URL: Issues, https://github.com/dieterich-lab/rp-
 bp/issues Keywords: bioinformatics,riboseq,open reading frame
 discovery,translation Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Science/Research Classifier: Topic :: Scientific/
```

### Comparing `rpbp-3.0.1/src/rpbp.egg-info/SOURCES.txt` & `rpbp-3.0.2/src/rpbp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 src/rpbp/analysis/profile_construction/create_read_length_orf_profiles.py
 src/rpbp/analysis/profile_construction/get_all_read_filtering_counts.py
 src/rpbp/analysis/profile_construction/summarize_rpbp_profile_construction.py
 src/rpbp/analysis/profile_construction/visualize_metagene_profile_bayes_factor.py
 src/rpbp/analysis/profile_construction/dashboard/__init__.py
 src/rpbp/analysis/profile_construction/dashboard/controls.py
 src/rpbp/analysis/profile_construction/dashboard/rpbp_profile_construction_dashboard.py
+src/rpbp/analysis/profile_construction/dashboard/assets/logo-rpbp.png
+src/rpbp/analysis/profile_construction/dashboard/assets/style.css
 src/rpbp/analysis/proteomics/__init__.py
 src/rpbp/analysis/proteomics/filter_nonunique_peptide_matches.py
 src/rpbp/analysis/proteomics/get_all_orf_peptide_matches.py
 src/rpbp/analysis/proteomics/get_orf_peptide_matches.py
 src/rpbp/analysis/rpbp_predictions/__init__.py
 src/rpbp/analysis/rpbp_predictions/summarize_rpbp_predictions.py
 src/rpbp/analysis/rpbp_predictions/visualize_orf_type_metagene_profiles.py
```

### Comparing `rpbp-3.0.1/src/rpbp.egg-info/entry_points.txt` & `rpbp-3.0.2/src/rpbp.egg-info/entry_points.txt`

 * *Files identical despite different names*

