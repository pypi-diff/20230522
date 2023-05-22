# Comparing `tmp/evidently-0.3.2.tar.gz` & `tmp/evidently-0.3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evidently-0.3.2.tar", last modified: Fri May 19 15:30:22 2023, max compression
+gzip compressed data, was "evidently-0.3.2.1.tar", last modified: Mon May 22 10:49:13 2023, max compression
```

## Comparing `evidently-0.3.2.tar` & `evidently-0.3.2.1.tar`

### file list

```diff
@@ -1,209 +1,209 @@
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:22.012442 evidently-0.3.2/
--rw-r--r--   0 emelidral   (501) staff       (20)      373 2023-05-19 15:30:22.012584 evidently-0.3.2/PKG-INFO
--rw-r--r--   0 emelidral   (501) staff       (20)     1447 2023-04-11 11:50:44.033151 evidently-0.3.2/setup.cfg
--rw-r--r--   0 emelidral   (501) staff       (20)     2103 2023-05-19 15:16:08.556083 evidently-0.3.2/setup.py
--rw-r--r--   0 emelidral   (501) staff       (20)    22071 2023-04-11 11:50:44.033364 evidently-0.3.2/setupbase.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:21.972941 evidently-0.3.2/src/
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:21.976785 evidently-0.3.2/src/evidently/
--rw-r--r--   0 emelidral   (501) staff       (20)      256 2023-04-11 11:50:44.033482 evidently-0.3.2/src/evidently/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1892 2023-04-27 10:27:02.402053 evidently-0.3.2/src/evidently/__main__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      162 2023-04-11 11:50:44.033618 evidently-0.3.2/src/evidently/_config.py
--rw-r--r--   0 emelidral   (501) staff       (20)      111 2023-05-19 15:29:00.246632 evidently-0.3.2/src/evidently/_version.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7505 2023-04-27 10:27:02.402425 evidently-0.3.2/src/evidently/base_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:21.978301 evidently-0.3.2/src/evidently/calculations/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.034605 evidently-0.3.2/src/evidently/calculations/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)    14543 2023-04-11 11:50:44.034697 evidently-0.3.2/src/evidently/calculations/classification_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)    16746 2023-05-19 15:16:08.556277 evidently-0.3.2/src/evidently/calculations/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2662 2023-04-11 11:50:44.034844 evidently-0.3.2/src/evidently/calculations/data_integration.py
--rw-r--r--   0 emelidral   (501) staff       (20)    32977 2023-05-19 15:16:08.556544 evidently-0.3.2/src/evidently/calculations/data_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8286 2023-04-11 11:50:44.035061 evidently-0.3.2/src/evidently/calculations/regression_performance.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:21.983571 evidently-0.3.2/src/evidently/calculations/stattests/
--rw-r--r--   0 emelidral   (501) staff       (20)     1258 2023-04-27 10:27:02.403157 evidently-0.3.2/src/evidently/calculations/stattests/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1337 2023-04-11 11:50:44.035216 evidently-0.3.2/src/evidently/calculations/stattests/anderson_darling_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1741 2023-04-11 11:50:44.035280 evidently-0.3.2/src/evidently/calculations/stattests/chisquare_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7331 2023-04-27 10:27:02.403563 evidently-0.3.2/src/evidently/calculations/stattests/cramer_von_mises_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1533 2023-04-11 11:50:44.035446 evidently-0.3.2/src/evidently/calculations/stattests/energy_distance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2108 2023-04-11 11:50:44.035531 evidently-0.3.2/src/evidently/calculations/stattests/epps_singleton_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2592 2023-04-11 11:50:44.035581 evidently-0.3.2/src/evidently/calculations/stattests/fisher_exact_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2025 2023-04-11 11:50:44.035635 evidently-0.3.2/src/evidently/calculations/stattests/g_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2983 2023-04-11 11:50:44.035704 evidently-0.3.2/src/evidently/calculations/stattests/hellinger_distance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2152 2023-04-11 11:50:44.035768 evidently-0.3.2/src/evidently/calculations/stattests/jensenshannon.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1899 2023-04-11 11:50:44.035819 evidently-0.3.2/src/evidently/calculations/stattests/kl_div.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1545 2023-04-11 11:50:44.035878 evidently-0.3.2/src/evidently/calculations/stattests/ks_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1752 2023-05-19 15:16:08.556697 evidently-0.3.2/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4683 2023-04-11 11:50:44.036014 evidently-0.3.2/src/evidently/calculations/stattests/mmd_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1812 2023-04-11 11:50:44.036061 evidently-0.3.2/src/evidently/calculations/stattests/psi.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4696 2023-04-27 10:27:02.403868 evidently-0.3.2/src/evidently/calculations/stattests/registry.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1490 2023-04-11 11:50:44.036213 evidently-0.3.2/src/evidently/calculations/stattests/t_test.py
--rw-r--r--   0 emelidral   (501) staff       (20)      799 2023-04-27 10:27:02.404121 evidently-0.3.2/src/evidently/calculations/stattests/text_content_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)      791 2023-04-27 10:27:02.404318 evidently-0.3.2/src/evidently/calculations/stattests/text_content_drift_abs.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2746 2023-04-11 11:50:44.036327 evidently-0.3.2/src/evidently/calculations/stattests/tvd_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4825 2023-04-11 11:50:44.036404 evidently-0.3.2/src/evidently/calculations/stattests/utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1832 2023-04-11 11:50:44.036454 evidently-0.3.2/src/evidently/calculations/stattests/wasserstein_distance_norm.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2878 2023-04-11 11:50:44.036512 evidently-0.3.2/src/evidently/calculations/stattests/z_stattest.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-04-11 11:50:44.036630 evidently-0.3.2/src/evidently/calculations/utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7042 2023-04-24 17:06:50.387018 evidently-0.3.2/src/evidently/core.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:21.984707 evidently-0.3.2/src/evidently/descriptors/
--rw-r--r--   0 emelidral   (501) staff       (20)      249 2023-04-11 11:50:44.040731 evidently-0.3.2/src/evidently/descriptors/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      578 2023-04-11 11:50:44.040789 evidently-0.3.2/src/evidently/descriptors/non_letter_character_percentage_descriptor.py
--rw-r--r--   0 emelidral   (501) staff       (20)      582 2023-04-11 11:50:44.040840 evidently-0.3.2/src/evidently/descriptors/oov_words_percentage_descriptor.py
--rw-r--r--   0 emelidral   (501) staff       (20)      464 2023-04-11 11:50:44.040888 evidently-0.3.2/src/evidently/descriptors/text_length_descriptor.py
--rw-r--r--   0 emelidral   (501) staff       (20)      776 2023-04-11 11:50:44.040933 evidently-0.3.2/src/evidently/descriptors/trigger_words_presence_descriptor.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:21.985906 evidently-0.3.2/src/evidently/features/
--rw-r--r--   0 emelidral   (501) staff       (20)     1682 2023-04-11 11:50:44.041013 evidently-0.3.2/src/evidently/features/OOV_words_percentage_feature.py
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.041037 evidently-0.3.2/src/evidently/features/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1894 2023-04-11 11:50:44.041102 evidently-0.3.2/src/evidently/features/generated_features.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1095 2023-04-11 11:50:44.041157 evidently-0.3.2/src/evidently/features/non_letter_character_percentage_feature.py
--rw-r--r--   0 emelidral   (501) staff       (20)      966 2023-04-11 11:50:44.041206 evidently-0.3.2/src/evidently/features/text_length_feature.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2121 2023-04-11 11:50:44.041271 evidently-0.3.2/src/evidently/features/trigger_words_presence_feature.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:21.987489 evidently-0.3.2/src/evidently/metric_preset/
--rw-r--r--   0 emelidral   (501) staff       (20)      496 2023-04-11 11:50:44.041350 evidently-0.3.2/src/evidently/metric_preset/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2526 2023-04-11 11:50:44.041407 evidently-0.3.2/src/evidently/metric_preset/classification_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4787 2023-04-27 10:27:02.404624 evidently-0.3.2/src/evidently/metric_preset/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1325 2023-04-11 11:50:44.041535 evidently-0.3.2/src/evidently/metric_preset/data_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)      343 2023-04-11 11:50:44.041591 evidently-0.3.2/src/evidently/metric_preset/metric_preset.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1817 2023-04-11 11:50:44.041650 evidently-0.3.2/src/evidently/metric_preset/regression_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7282 2023-04-11 11:50:44.041719 evidently-0.3.2/src/evidently/metric_preset/target_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1811 2023-04-11 11:50:44.041776 evidently-0.3.2/src/evidently/metric_preset/text_overview.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8904 2023-05-19 15:16:08.556895 evidently-0.3.2/src/evidently/metric_results.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:21.988087 evidently-0.3.2/src/evidently/metrics/
--rw-r--r--   0 emelidral   (501) staff       (20)     3737 2023-04-11 11:50:44.041950 evidently-0.3.2/src/evidently/metrics/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      691 2023-04-11 11:50:44.042032 evidently-0.3.2/src/evidently/metrics/base_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:21.991014 evidently-0.3.2/src/evidently/metrics/classification_performance/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.042092 evidently-0.3.2/src/evidently/metrics/classification_performance/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3021 2023-05-19 15:16:08.557044 evidently-0.3.2/src/evidently/metrics/classification_performance/base_classification_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3132 2023-04-27 10:27:02.405129 evidently-0.3.2/src/evidently/metrics/classification_performance/class_balance_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6441 2023-05-19 15:16:08.557179 evidently-0.3.2/src/evidently/metrics/classification_performance/class_separation_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12015 2023-04-27 10:27:02.405315 evidently-0.3.2/src/evidently/metrics/classification_performance/classification_dummy_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5193 2023-04-11 11:50:44.042500 evidently-0.3.2/src/evidently/metrics/classification_performance/classification_quality_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3569 2023-04-27 10:27:02.405480 evidently-0.3.2/src/evidently/metrics/classification_performance/confusion_matrix_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1534 2023-04-11 11:50:44.042621 evidently-0.3.2/src/evidently/metrics/classification_performance/objects.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4483 2023-04-11 11:50:44.042685 evidently-0.3.2/src/evidently/metrics/classification_performance/pr_curve_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6020 2023-04-11 11:50:44.042749 evidently-0.3.2/src/evidently/metrics/classification_performance/pr_table_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5959 2023-04-11 11:50:44.042828 evidently-0.3.2/src/evidently/metrics/classification_performance/probability_distribution_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7318 2023-04-11 11:50:44.042904 evidently-0.3.2/src/evidently/metrics/classification_performance/quality_by_class_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    17138 2023-05-19 15:16:08.557405 evidently-0.3.2/src/evidently/metrics/classification_performance/quality_by_feature_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4425 2023-04-11 11:50:44.043054 evidently-0.3.2/src/evidently/metrics/classification_performance/roc_curve_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:21.993035 evidently-0.3.2/src/evidently/metrics/data_drift/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.043120 evidently-0.3.2/src/evidently/metrics/data_drift/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)    18520 2023-05-19 15:16:08.557594 evidently-0.3.2/src/evidently/metrics/data_drift/column_drift_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     9686 2023-05-19 15:16:08.557756 evidently-0.3.2/src/evidently/metrics/data_drift/column_value_plot.py
--rw-r--r--   0 emelidral   (501) staff       (20)    13396 2023-05-19 15:16:08.557920 evidently-0.3.2/src/evidently/metrics/data_drift/data_drift_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4733 2023-05-19 15:16:08.558070 evidently-0.3.2/src/evidently/metrics/data_drift/dataset_drift_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    10729 2023-04-27 10:27:02.406479 evidently-0.3.2/src/evidently/metrics/data_drift/embedding_drift_methods.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4538 2023-05-19 15:16:08.558192 evidently-0.3.2/src/evidently/metrics/data_drift/embeddings_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)    13793 2023-05-19 15:16:08.558333 evidently-0.3.2/src/evidently/metrics/data_drift/target_by_features_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)    11082 2023-05-19 15:16:08.558473 evidently-0.3.2/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    11173 2023-04-11 11:50:44.043845 evidently-0.3.2/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:21.994225 evidently-0.3.2/src/evidently/metrics/data_integrity/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.043904 evidently-0.3.2/src/evidently/metrics/data_integrity/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8345 2023-04-11 11:50:44.043991 evidently-0.3.2/src/evidently/metrics/data_integrity/column_missing_values_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7142 2023-04-11 11:50:44.044068 evidently-0.3.2/src/evidently/metrics/data_integrity/column_regexp_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    28022 2023-05-19 15:16:08.558666 evidently-0.3.2/src/evidently/metrics/data_integrity/column_summary_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12456 2023-04-11 11:50:44.044306 evidently-0.3.2/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8789 2023-04-11 11:50:44.044393 evidently-0.3.2/src/evidently/metrics/data_integrity/dataset_summary_metric.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:21.996914 evidently-0.3.2/src/evidently/metrics/data_quality/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.044472 evidently-0.3.2/src/evidently/metrics/data_quality/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5821 2023-04-11 11:50:44.044563 evidently-0.3.2/src/evidently/metrics/data_quality/column_correlations_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3054 2023-04-11 11:50:44.044629 evidently-0.3.2/src/evidently/metrics/data_quality/column_distribution_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5896 2023-04-27 10:27:02.407846 evidently-0.3.2/src/evidently/metrics/data_quality/column_quantile_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6872 2023-04-11 11:50:44.044766 evidently-0.3.2/src/evidently/metrics/data_quality/column_value_list_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8991 2023-04-11 11:50:44.044848 evidently-0.3.2/src/evidently/metrics/data_quality/column_value_range_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4336 2023-04-11 11:50:44.044913 evidently-0.3.2/src/evidently/metrics/data_quality/conflict_prediction_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3927 2023-04-11 11:50:44.044975 evidently-0.3.2/src/evidently/metrics/data_quality/conflict_target_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    13927 2023-04-11 11:50:44.045061 evidently-0.3.2/src/evidently/metrics/data_quality/dataset_correlations_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2657 2023-04-11 11:50:44.045118 evidently-0.3.2/src/evidently/metrics/data_quality/stability_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7248 2023-04-11 11:50:44.045194 evidently-0.3.2/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5215 2023-04-11 11:50:44.045257 evidently-0.3.2/src/evidently/metrics/data_quality/text_descriptors_distribution.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:21.999998 evidently-0.3.2/src/evidently/metrics/regression_performance/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.045310 evidently-0.3.2/src/evidently/metrics/regression_performance/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6449 2023-05-19 15:16:08.558812 evidently-0.3.2/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py
--rw-r--r--   0 emelidral   (501) staff       (20)    28994 2023-05-19 15:16:08.558914 evidently-0.3.2/src/evidently/metrics/regression_performance/error_bias_table.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3936 2023-04-11 11:50:44.045565 evidently-0.3.2/src/evidently/metrics/regression_performance/error_distribution.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6093 2023-05-19 15:16:08.559044 evidently-0.3.2/src/evidently/metrics/regression_performance/error_in_time.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7598 2023-05-19 15:16:08.559168 evidently-0.3.2/src/evidently/metrics/regression_performance/error_normality.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1675 2023-04-11 11:50:44.045735 evidently-0.3.2/src/evidently/metrics/regression_performance/objects.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7833 2023-05-19 15:16:08.559285 evidently-0.3.2/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6610 2023-05-19 15:16:08.559434 evidently-0.3.2/src/evidently/metrics/regression_performance/predicted_vs_actual.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8427 2023-04-11 11:50:44.045914 evidently-0.3.2/src/evidently/metrics/regression_performance/regression_dummy_metric.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12823 2023-04-11 11:50:44.045990 evidently-0.3.2/src/evidently/metrics/regression_performance/regression_performance_metrics.py
--rw-r--r--   0 emelidral   (501) staff       (20)    12845 2023-04-11 11:50:44.046056 evidently-0.3.2/src/evidently/metrics/regression_performance/regression_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)    13755 2023-05-19 15:16:08.559658 evidently-0.3.2/src/evidently/metrics/regression_performance/top_error.py
--rw-r--r--   0 emelidral   (501) staff       (20)      628 2023-04-11 11:50:44.046174 evidently-0.3.2/src/evidently/metrics/regression_performance/utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4630 2023-04-11 11:50:44.046235 evidently-0.3.2/src/evidently/metrics/regression_performance/visualization.py
--rw-r--r--   0 emelidral   (501) staff       (20)      847 2023-04-11 11:50:44.046284 evidently-0.3.2/src/evidently/metrics/utils.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:22.000578 evidently-0.3.2/src/evidently/model/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.046336 evidently-0.3.2/src/evidently/model/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      230 2023-04-11 11:50:44.046390 evidently-0.3.2/src/evidently/model/dashboard.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2262 2023-04-11 11:50:44.046446 evidently-0.3.2/src/evidently/model/widget.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:22.000776 evidently-0.3.2/src/evidently/nbextension/
--rw-r--r--   0 emelidral   (501) staff       (20)      195 2023-04-11 11:50:44.047775 evidently-0.3.2/src/evidently/nbextension/__init__.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:22.001580 evidently-0.3.2/src/evidently/nbextension/static/
--rw-r--r--   0 emelidral   (501) staff       (20)      409 2023-04-11 11:50:44.047847 evidently-0.3.2/src/evidently/nbextension/static/extension.js
--rw-r--r--   0 emelidral   (501) staff       (20)  2586352 2023-04-11 11:50:44.055472 evidently-0.3.2/src/evidently/nbextension/static/index.js
--rw-r--r--   0 emelidral   (501) staff       (20)     2238 2023-04-11 11:50:44.055652 evidently-0.3.2/src/evidently/nbextension/static/index.js.LICENSE.txt
--rw-r--r--   0 emelidral   (501) staff       (20)    94648 2023-04-11 11:50:44.056026 evidently-0.3.2/src/evidently/nbextension/static/material-ui-icons.woff2
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:22.002992 evidently-0.3.2/src/evidently/options/
--rw-r--r--   0 emelidral   (501) staff       (20)      471 2023-04-27 10:27:02.408578 evidently-0.3.2/src/evidently/options/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)      102 2023-05-19 15:16:08.559716 evidently-0.3.2/src/evidently/options/agg_data.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2770 2023-05-19 15:16:08.559823 evidently-0.3.2/src/evidently/options/base.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3357 2023-05-19 15:16:08.559935 evidently-0.3.2/src/evidently/options/color_scheme.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8204 2023-04-11 11:50:44.056254 evidently-0.3.2/src/evidently/options/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)       67 2023-04-27 10:27:02.409017 evidently-0.3.2/src/evidently/options/option.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1209 2023-04-11 11:50:44.056307 evidently-0.3.2/src/evidently/options/quality_metrics.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:22.003404 evidently-0.3.2/src/evidently/pipeline/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.056358 evidently-0.3.2/src/evidently/pipeline/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1162 2023-04-27 10:27:02.409249 evidently-0.3.2/src/evidently/pipeline/column_mapping.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:22.004502 evidently-0.3.2/src/evidently/renderers/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.056636 evidently-0.3.2/src/evidently/renderers/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     3114 2023-04-11 11:50:44.056702 evidently-0.3.2/src/evidently/renderers/base_renderer.py
--rw-r--r--   0 emelidral   (501) staff       (20)    29101 2023-05-19 15:16:08.560226 evidently-0.3.2/src/evidently/renderers/html_widgets.py
--rw-r--r--   0 emelidral   (501) staff       (20)      733 2023-04-11 11:50:44.056873 evidently-0.3.2/src/evidently/renderers/notebook_utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1781 2023-04-11 11:50:44.056927 evidently-0.3.2/src/evidently/renderers/render_utils.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:22.005006 evidently-0.3.2/src/evidently/report/
--rw-r--r--   0 emelidral   (501) staff       (20)       27 2023-04-11 11:50:44.057001 evidently-0.3.2/src/evidently/report/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7413 2023-05-19 15:16:08.560356 evidently-0.3.2/src/evidently/report/report.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:22.005624 evidently-0.3.2/src/evidently/runner/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.057130 evidently-0.3.2/src/evidently/runner/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2842 2023-04-11 11:50:44.057260 evidently-0.3.2/src/evidently/runner/loader.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2134 2023-04-11 11:50:44.057381 evidently-0.3.2/src/evidently/runner/runner.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:22.006258 evidently-0.3.2/src/evidently/suite/
--rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.057438 evidently-0.3.2/src/evidently/suite/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)    14249 2023-05-19 15:16:08.560498 evidently-0.3.2/src/evidently/suite/base_suite.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1991 2023-04-11 11:50:44.057593 evidently-0.3.2/src/evidently/suite/execution_graph.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:22.006660 evidently-0.3.2/src/evidently/telemetry/
--rw-r--r--   0 emelidral   (501) staff       (20)       36 2023-04-11 11:50:44.057752 evidently-0.3.2/src/evidently/telemetry/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1007 2023-04-11 11:50:44.057808 evidently-0.3.2/src/evidently/telemetry/sender.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:22.008636 evidently-0.3.2/src/evidently/test_preset/
--rw-r--r--   0 emelidral   (501) staff       (20)      859 2023-04-11 11:50:44.057891 evidently-0.3.2/src/evidently/test_preset/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2707 2023-04-11 11:50:44.058127 evidently-0.3.2/src/evidently/test_preset/classification_binary.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1948 2023-04-11 11:50:44.058178 evidently-0.3.2/src/evidently/test_preset/classification_binary_topk.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2507 2023-04-11 11:50:44.058248 evidently-0.3.2/src/evidently/test_preset/classification_multiclass.py
--rw-r--r--   0 emelidral   (501) staff       (20)     7352 2023-04-27 10:27:02.410133 evidently-0.3.2/src/evidently/test_preset/data_drift.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-04-11 11:50:44.058356 evidently-0.3.2/src/evidently/test_preset/data_quality.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1559 2023-04-11 11:50:44.058402 evidently-0.3.2/src/evidently/test_preset/data_stability.py
--rw-r--r--   0 emelidral   (501) staff       (20)     6811 2023-04-27 10:27:02.410385 evidently-0.3.2/src/evidently/test_preset/no_target_performance.py
--rw-r--r--   0 emelidral   (501) staff       (20)      750 2023-04-11 11:50:44.058506 evidently-0.3.2/src/evidently/test_preset/regression.py
--rw-r--r--   0 emelidral   (501) staff       (20)      298 2023-04-11 11:50:44.058559 evidently-0.3.2/src/evidently/test_preset/test_preset.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:22.009020 evidently-0.3.2/src/evidently/test_suite/
--rw-r--r--   0 emelidral   (501) staff       (20)       34 2023-04-11 11:50:44.058625 evidently-0.3.2/src/evidently/test_suite/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8647 2023-05-19 15:16:08.560630 evidently-0.3.2/src/evidently/test_suite/test_suite.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:22.010552 evidently-0.3.2/src/evidently/tests/
--rw-r--r--   0 emelidral   (501) staff       (20)     4460 2023-04-27 10:27:02.410897 evidently-0.3.2/src/evidently/tests/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)    11758 2023-04-11 11:50:44.058862 evidently-0.3.2/src/evidently/tests/base_test.py
--rw-r--r--   0 emelidral   (501) staff       (20)    22752 2023-04-11 11:50:44.059177 evidently-0.3.2/src/evidently/tests/classification_performance_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    21931 2023-05-19 15:16:08.560789 evidently-0.3.2/src/evidently/tests/data_drift_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    42332 2023-04-27 10:27:02.411682 evidently-0.3.2/src/evidently/tests/data_integrity_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    53681 2023-04-27 10:27:02.412175 evidently-0.3.2/src/evidently/tests/data_quality_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    10930 2023-04-11 11:50:44.059579 evidently-0.3.2/src/evidently/tests/regression_performance_tests.py
--rw-r--r--   0 emelidral   (501) staff       (20)    16360 2023-04-11 11:50:44.059661 evidently-0.3.2/src/evidently/tests/utils.py
-drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-19 15:30:22.012402 evidently-0.3.2/src/evidently/utils/
--rw-r--r--   0 emelidral   (501) staff       (20)       40 2023-04-11 11:50:44.059731 evidently-0.3.2/src/evidently/utils/__init__.py
--rw-r--r--   0 emelidral   (501) staff       (20)     5800 2023-04-11 11:50:44.059794 evidently-0.3.2/src/evidently/utils/dashboard.py
--rw-r--r--   0 emelidral   (501) staff       (20)     9086 2023-04-27 10:27:02.412473 evidently-0.3.2/src/evidently/utils/data_drift_utils.py
--rw-r--r--   0 emelidral   (501) staff       (20)     8133 2023-04-11 11:50:44.059931 evidently-0.3.2/src/evidently/utils/data_operations.py
--rw-r--r--   0 emelidral   (501) staff       (20)    20996 2023-04-11 11:50:44.060030 evidently-0.3.2/src/evidently/utils/data_preprocessing.py
--rw-r--r--   0 emelidral   (501) staff       (20)     4375 2023-04-11 11:50:44.060100 evidently-0.3.2/src/evidently/utils/generators.py
--rw-r--r--   0 emelidral   (501) staff       (20)     1392 2023-04-24 17:06:50.391821 evidently-0.3.2/src/evidently/utils/numpy_encoder.py
--rw-r--r--   0 emelidral   (501) staff       (20)     2262 2023-04-11 11:50:44.060206 evidently-0.3.2/src/evidently/utils/types.py
--rw-r--r--   0 emelidral   (501) staff       (20)    35867 2023-05-19 15:16:08.561016 evidently-0.3.2/src/evidently/utils/visualizations.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.036625 evidently-0.3.2.1/
+-rw-r--r--   0 emelidral   (501) staff       (20)      375 2023-05-22 10:49:13.036769 evidently-0.3.2.1/PKG-INFO
+-rw-r--r--   0 emelidral   (501) staff       (20)     1447 2023-04-11 11:50:44.033151 evidently-0.3.2.1/setup.cfg
+-rw-r--r--   0 emelidral   (501) staff       (20)     2103 2023-05-19 15:16:08.556083 evidently-0.3.2.1/setup.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    22071 2023-04-11 11:50:44.033364 evidently-0.3.2.1/setupbase.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:12.997738 evidently-0.3.2.1/src/
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.001421 evidently-0.3.2.1/src/evidently/
+-rw-r--r--   0 emelidral   (501) staff       (20)      256 2023-04-11 11:50:44.033482 evidently-0.3.2.1/src/evidently/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1892 2023-04-27 10:27:02.402053 evidently-0.3.2.1/src/evidently/__main__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      162 2023-04-11 11:50:44.033618 evidently-0.3.2.1/src/evidently/_config.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      114 2023-05-22 10:49:07.844116 evidently-0.3.2.1/src/evidently/_version.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7505 2023-04-27 10:27:02.402425 evidently-0.3.2.1/src/evidently/base_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.002922 evidently-0.3.2.1/src/evidently/calculations/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.034605 evidently-0.3.2.1/src/evidently/calculations/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    14543 2023-04-11 11:50:44.034697 evidently-0.3.2.1/src/evidently/calculations/classification_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    16746 2023-05-19 15:16:08.556277 evidently-0.3.2.1/src/evidently/calculations/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2662 2023-04-11 11:50:44.034844 evidently-0.3.2.1/src/evidently/calculations/data_integration.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    32977 2023-05-19 15:16:08.556544 evidently-0.3.2.1/src/evidently/calculations/data_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8286 2023-04-11 11:50:44.035061 evidently-0.3.2.1/src/evidently/calculations/regression_performance.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.007816 evidently-0.3.2.1/src/evidently/calculations/stattests/
+-rw-r--r--   0 emelidral   (501) staff       (20)     1258 2023-04-27 10:27:02.403157 evidently-0.3.2.1/src/evidently/calculations/stattests/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1337 2023-04-11 11:50:44.035216 evidently-0.3.2.1/src/evidently/calculations/stattests/anderson_darling_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1741 2023-04-11 11:50:44.035280 evidently-0.3.2.1/src/evidently/calculations/stattests/chisquare_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7331 2023-04-27 10:27:02.403563 evidently-0.3.2.1/src/evidently/calculations/stattests/cramer_von_mises_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1533 2023-04-11 11:50:44.035446 evidently-0.3.2.1/src/evidently/calculations/stattests/energy_distance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2108 2023-04-11 11:50:44.035531 evidently-0.3.2.1/src/evidently/calculations/stattests/epps_singleton_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2592 2023-04-11 11:50:44.035581 evidently-0.3.2.1/src/evidently/calculations/stattests/fisher_exact_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2025 2023-04-11 11:50:44.035635 evidently-0.3.2.1/src/evidently/calculations/stattests/g_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2983 2023-04-11 11:50:44.035704 evidently-0.3.2.1/src/evidently/calculations/stattests/hellinger_distance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2152 2023-04-11 11:50:44.035768 evidently-0.3.2.1/src/evidently/calculations/stattests/jensenshannon.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1899 2023-04-11 11:50:44.035819 evidently-0.3.2.1/src/evidently/calculations/stattests/kl_div.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1545 2023-04-11 11:50:44.035878 evidently-0.3.2.1/src/evidently/calculations/stattests/ks_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1752 2023-05-19 15:16:08.556697 evidently-0.3.2.1/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4683 2023-04-11 11:50:44.036014 evidently-0.3.2.1/src/evidently/calculations/stattests/mmd_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1812 2023-04-11 11:50:44.036061 evidently-0.3.2.1/src/evidently/calculations/stattests/psi.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4696 2023-04-27 10:27:02.403868 evidently-0.3.2.1/src/evidently/calculations/stattests/registry.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1490 2023-04-11 11:50:44.036213 evidently-0.3.2.1/src/evidently/calculations/stattests/t_test.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      799 2023-04-27 10:27:02.404121 evidently-0.3.2.1/src/evidently/calculations/stattests/text_content_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      791 2023-04-27 10:27:02.404318 evidently-0.3.2.1/src/evidently/calculations/stattests/text_content_drift_abs.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2746 2023-04-11 11:50:44.036327 evidently-0.3.2.1/src/evidently/calculations/stattests/tvd_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4825 2023-04-11 11:50:44.036404 evidently-0.3.2.1/src/evidently/calculations/stattests/utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1832 2023-04-11 11:50:44.036454 evidently-0.3.2.1/src/evidently/calculations/stattests/wasserstein_distance_norm.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2878 2023-04-11 11:50:44.036512 evidently-0.3.2.1/src/evidently/calculations/stattests/z_stattest.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-04-11 11:50:44.036630 evidently-0.3.2.1/src/evidently/calculations/utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7042 2023-04-24 17:06:50.387018 evidently-0.3.2.1/src/evidently/core.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.008892 evidently-0.3.2.1/src/evidently/descriptors/
+-rw-r--r--   0 emelidral   (501) staff       (20)      249 2023-04-11 11:50:44.040731 evidently-0.3.2.1/src/evidently/descriptors/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      578 2023-04-11 11:50:44.040789 evidently-0.3.2.1/src/evidently/descriptors/non_letter_character_percentage_descriptor.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      582 2023-04-11 11:50:44.040840 evidently-0.3.2.1/src/evidently/descriptors/oov_words_percentage_descriptor.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      464 2023-04-11 11:50:44.040888 evidently-0.3.2.1/src/evidently/descriptors/text_length_descriptor.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      776 2023-04-11 11:50:44.040933 evidently-0.3.2.1/src/evidently/descriptors/trigger_words_presence_descriptor.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.010153 evidently-0.3.2.1/src/evidently/features/
+-rw-r--r--   0 emelidral   (501) staff       (20)     1682 2023-04-11 11:50:44.041013 evidently-0.3.2.1/src/evidently/features/OOV_words_percentage_feature.py
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.041037 evidently-0.3.2.1/src/evidently/features/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1894 2023-04-11 11:50:44.041102 evidently-0.3.2.1/src/evidently/features/generated_features.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1095 2023-04-11 11:50:44.041157 evidently-0.3.2.1/src/evidently/features/non_letter_character_percentage_feature.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      966 2023-04-11 11:50:44.041206 evidently-0.3.2.1/src/evidently/features/text_length_feature.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2121 2023-04-11 11:50:44.041271 evidently-0.3.2.1/src/evidently/features/trigger_words_presence_feature.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.011770 evidently-0.3.2.1/src/evidently/metric_preset/
+-rw-r--r--   0 emelidral   (501) staff       (20)      496 2023-04-11 11:50:44.041350 evidently-0.3.2.1/src/evidently/metric_preset/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2526 2023-04-11 11:50:44.041407 evidently-0.3.2.1/src/evidently/metric_preset/classification_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4787 2023-04-27 10:27:02.404624 evidently-0.3.2.1/src/evidently/metric_preset/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1325 2023-04-11 11:50:44.041535 evidently-0.3.2.1/src/evidently/metric_preset/data_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      343 2023-04-11 11:50:44.041591 evidently-0.3.2.1/src/evidently/metric_preset/metric_preset.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1817 2023-04-11 11:50:44.041650 evidently-0.3.2.1/src/evidently/metric_preset/regression_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7282 2023-04-11 11:50:44.041719 evidently-0.3.2.1/src/evidently/metric_preset/target_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1811 2023-04-11 11:50:44.041776 evidently-0.3.2.1/src/evidently/metric_preset/text_overview.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8904 2023-05-19 15:16:08.556895 evidently-0.3.2.1/src/evidently/metric_results.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.012364 evidently-0.3.2.1/src/evidently/metrics/
+-rw-r--r--   0 emelidral   (501) staff       (20)     3737 2023-04-11 11:50:44.041950 evidently-0.3.2.1/src/evidently/metrics/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      691 2023-04-11 11:50:44.042032 evidently-0.3.2.1/src/evidently/metrics/base_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.015254 evidently-0.3.2.1/src/evidently/metrics/classification_performance/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.042092 evidently-0.3.2.1/src/evidently/metrics/classification_performance/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3021 2023-05-19 15:16:08.557044 evidently-0.3.2.1/src/evidently/metrics/classification_performance/base_classification_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3132 2023-04-27 10:27:02.405129 evidently-0.3.2.1/src/evidently/metrics/classification_performance/class_balance_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6441 2023-05-19 15:16:08.557179 evidently-0.3.2.1/src/evidently/metrics/classification_performance/class_separation_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12015 2023-04-27 10:27:02.405315 evidently-0.3.2.1/src/evidently/metrics/classification_performance/classification_dummy_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5193 2023-04-11 11:50:44.042500 evidently-0.3.2.1/src/evidently/metrics/classification_performance/classification_quality_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3569 2023-04-27 10:27:02.405480 evidently-0.3.2.1/src/evidently/metrics/classification_performance/confusion_matrix_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1534 2023-04-11 11:50:44.042621 evidently-0.3.2.1/src/evidently/metrics/classification_performance/objects.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4483 2023-04-11 11:50:44.042685 evidently-0.3.2.1/src/evidently/metrics/classification_performance/pr_curve_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6020 2023-04-11 11:50:44.042749 evidently-0.3.2.1/src/evidently/metrics/classification_performance/pr_table_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5959 2023-04-11 11:50:44.042828 evidently-0.3.2.1/src/evidently/metrics/classification_performance/probability_distribution_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7318 2023-04-11 11:50:44.042904 evidently-0.3.2.1/src/evidently/metrics/classification_performance/quality_by_class_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    17138 2023-05-19 15:16:08.557405 evidently-0.3.2.1/src/evidently/metrics/classification_performance/quality_by_feature_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4425 2023-04-11 11:50:44.043054 evidently-0.3.2.1/src/evidently/metrics/classification_performance/roc_curve_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.017255 evidently-0.3.2.1/src/evidently/metrics/data_drift/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.043120 evidently-0.3.2.1/src/evidently/metrics/data_drift/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    18498 2023-05-22 10:48:01.966184 evidently-0.3.2.1/src/evidently/metrics/data_drift/column_drift_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     9686 2023-05-19 15:16:08.557756 evidently-0.3.2.1/src/evidently/metrics/data_drift/column_value_plot.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    13396 2023-05-19 15:16:08.557920 evidently-0.3.2.1/src/evidently/metrics/data_drift/data_drift_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4733 2023-05-19 15:16:08.558070 evidently-0.3.2.1/src/evidently/metrics/data_drift/dataset_drift_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    10729 2023-04-27 10:27:02.406479 evidently-0.3.2.1/src/evidently/metrics/data_drift/embedding_drift_methods.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4538 2023-05-19 15:16:08.558192 evidently-0.3.2.1/src/evidently/metrics/data_drift/embeddings_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    13793 2023-05-19 15:16:08.558333 evidently-0.3.2.1/src/evidently/metrics/data_drift/target_by_features_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    11082 2023-05-19 15:16:08.558473 evidently-0.3.2.1/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    11173 2023-04-11 11:50:44.043845 evidently-0.3.2.1/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.018445 evidently-0.3.2.1/src/evidently/metrics/data_integrity/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.043904 evidently-0.3.2.1/src/evidently/metrics/data_integrity/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8345 2023-04-11 11:50:44.043991 evidently-0.3.2.1/src/evidently/metrics/data_integrity/column_missing_values_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7142 2023-04-11 11:50:44.044068 evidently-0.3.2.1/src/evidently/metrics/data_integrity/column_regexp_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    28022 2023-05-19 15:16:08.558666 evidently-0.3.2.1/src/evidently/metrics/data_integrity/column_summary_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12456 2023-04-11 11:50:44.044306 evidently-0.3.2.1/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8789 2023-04-11 11:50:44.044393 evidently-0.3.2.1/src/evidently/metrics/data_integrity/dataset_summary_metric.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.020816 evidently-0.3.2.1/src/evidently/metrics/data_quality/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.044472 evidently-0.3.2.1/src/evidently/metrics/data_quality/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5821 2023-04-11 11:50:44.044563 evidently-0.3.2.1/src/evidently/metrics/data_quality/column_correlations_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3054 2023-04-11 11:50:44.044629 evidently-0.3.2.1/src/evidently/metrics/data_quality/column_distribution_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5896 2023-04-27 10:27:02.407846 evidently-0.3.2.1/src/evidently/metrics/data_quality/column_quantile_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6872 2023-04-11 11:50:44.044766 evidently-0.3.2.1/src/evidently/metrics/data_quality/column_value_list_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8991 2023-04-11 11:50:44.044848 evidently-0.3.2.1/src/evidently/metrics/data_quality/column_value_range_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4336 2023-04-11 11:50:44.044913 evidently-0.3.2.1/src/evidently/metrics/data_quality/conflict_prediction_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3927 2023-04-11 11:50:44.044975 evidently-0.3.2.1/src/evidently/metrics/data_quality/conflict_target_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    13927 2023-04-11 11:50:44.045061 evidently-0.3.2.1/src/evidently/metrics/data_quality/dataset_correlations_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2657 2023-04-11 11:50:44.045118 evidently-0.3.2.1/src/evidently/metrics/data_quality/stability_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7248 2023-04-11 11:50:44.045194 evidently-0.3.2.1/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5215 2023-04-11 11:50:44.045257 evidently-0.3.2.1/src/evidently/metrics/data_quality/text_descriptors_distribution.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.023777 evidently-0.3.2.1/src/evidently/metrics/regression_performance/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.045310 evidently-0.3.2.1/src/evidently/metrics/regression_performance/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6449 2023-05-19 15:16:08.558812 evidently-0.3.2.1/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    28994 2023-05-19 15:16:08.558914 evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_bias_table.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3936 2023-04-11 11:50:44.045565 evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_distribution.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6093 2023-05-19 15:16:08.559044 evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_in_time.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7598 2023-05-19 15:16:08.559168 evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_normality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1675 2023-04-11 11:50:44.045735 evidently-0.3.2.1/src/evidently/metrics/regression_performance/objects.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7833 2023-05-19 15:16:08.559285 evidently-0.3.2.1/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6610 2023-05-19 15:16:08.559434 evidently-0.3.2.1/src/evidently/metrics/regression_performance/predicted_vs_actual.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8427 2023-04-11 11:50:44.045914 evidently-0.3.2.1/src/evidently/metrics/regression_performance/regression_dummy_metric.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12823 2023-04-11 11:50:44.045990 evidently-0.3.2.1/src/evidently/metrics/regression_performance/regression_performance_metrics.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    12845 2023-04-11 11:50:44.046056 evidently-0.3.2.1/src/evidently/metrics/regression_performance/regression_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    13755 2023-05-19 15:16:08.559658 evidently-0.3.2.1/src/evidently/metrics/regression_performance/top_error.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      628 2023-04-11 11:50:44.046174 evidently-0.3.2.1/src/evidently/metrics/regression_performance/utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4630 2023-04-11 11:50:44.046235 evidently-0.3.2.1/src/evidently/metrics/regression_performance/visualization.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      847 2023-04-11 11:50:44.046284 evidently-0.3.2.1/src/evidently/metrics/utils.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.024350 evidently-0.3.2.1/src/evidently/model/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.046336 evidently-0.3.2.1/src/evidently/model/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      230 2023-04-11 11:50:44.046390 evidently-0.3.2.1/src/evidently/model/dashboard.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2262 2023-04-11 11:50:44.046446 evidently-0.3.2.1/src/evidently/model/widget.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.024544 evidently-0.3.2.1/src/evidently/nbextension/
+-rw-r--r--   0 emelidral   (501) staff       (20)      195 2023-04-11 11:50:44.047775 evidently-0.3.2.1/src/evidently/nbextension/__init__.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.025353 evidently-0.3.2.1/src/evidently/nbextension/static/
+-rw-r--r--   0 emelidral   (501) staff       (20)      409 2023-04-11 11:50:44.047847 evidently-0.3.2.1/src/evidently/nbextension/static/extension.js
+-rw-r--r--   0 emelidral   (501) staff       (20)  2586352 2023-04-11 11:50:44.055472 evidently-0.3.2.1/src/evidently/nbextension/static/index.js
+-rw-r--r--   0 emelidral   (501) staff       (20)     2238 2023-04-11 11:50:44.055652 evidently-0.3.2.1/src/evidently/nbextension/static/index.js.LICENSE.txt
+-rw-r--r--   0 emelidral   (501) staff       (20)    94648 2023-04-11 11:50:44.056026 evidently-0.3.2.1/src/evidently/nbextension/static/material-ui-icons.woff2
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.026717 evidently-0.3.2.1/src/evidently/options/
+-rw-r--r--   0 emelidral   (501) staff       (20)      471 2023-04-27 10:27:02.408578 evidently-0.3.2.1/src/evidently/options/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      102 2023-05-19 15:16:08.559716 evidently-0.3.2.1/src/evidently/options/agg_data.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2770 2023-05-19 15:16:08.559823 evidently-0.3.2.1/src/evidently/options/base.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3357 2023-05-19 15:16:08.559935 evidently-0.3.2.1/src/evidently/options/color_scheme.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8204 2023-04-11 11:50:44.056254 evidently-0.3.2.1/src/evidently/options/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)       67 2023-04-27 10:27:02.409017 evidently-0.3.2.1/src/evidently/options/option.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1209 2023-04-11 11:50:44.056307 evidently-0.3.2.1/src/evidently/options/quality_metrics.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.027105 evidently-0.3.2.1/src/evidently/pipeline/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.056358 evidently-0.3.2.1/src/evidently/pipeline/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1162 2023-04-27 10:27:02.409249 evidently-0.3.2.1/src/evidently/pipeline/column_mapping.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.028131 evidently-0.3.2.1/src/evidently/renderers/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.056636 evidently-0.3.2.1/src/evidently/renderers/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     3114 2023-04-11 11:50:44.056702 evidently-0.3.2.1/src/evidently/renderers/base_renderer.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    29101 2023-05-19 15:16:08.560226 evidently-0.3.2.1/src/evidently/renderers/html_widgets.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      733 2023-04-11 11:50:44.056873 evidently-0.3.2.1/src/evidently/renderers/notebook_utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1781 2023-04-11 11:50:44.056927 evidently-0.3.2.1/src/evidently/renderers/render_utils.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.028569 evidently-0.3.2.1/src/evidently/report/
+-rw-r--r--   0 emelidral   (501) staff       (20)       27 2023-04-11 11:50:44.057001 evidently-0.3.2.1/src/evidently/report/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7413 2023-05-19 15:16:08.560356 evidently-0.3.2.1/src/evidently/report/report.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.029264 evidently-0.3.2.1/src/evidently/runner/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.057130 evidently-0.3.2.1/src/evidently/runner/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2842 2023-04-11 11:50:44.057260 evidently-0.3.2.1/src/evidently/runner/loader.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2134 2023-04-11 11:50:44.057381 evidently-0.3.2.1/src/evidently/runner/runner.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.030003 evidently-0.3.2.1/src/evidently/suite/
+-rw-r--r--   0 emelidral   (501) staff       (20)        0 2023-04-11 11:50:44.057438 evidently-0.3.2.1/src/evidently/suite/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    14249 2023-05-19 15:16:08.560498 evidently-0.3.2.1/src/evidently/suite/base_suite.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1991 2023-04-11 11:50:44.057593 evidently-0.3.2.1/src/evidently/suite/execution_graph.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.030420 evidently-0.3.2.1/src/evidently/telemetry/
+-rw-r--r--   0 emelidral   (501) staff       (20)       36 2023-04-11 11:50:44.057752 evidently-0.3.2.1/src/evidently/telemetry/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1007 2023-04-11 11:50:44.057808 evidently-0.3.2.1/src/evidently/telemetry/sender.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.032523 evidently-0.3.2.1/src/evidently/test_preset/
+-rw-r--r--   0 emelidral   (501) staff       (20)      859 2023-04-11 11:50:44.057891 evidently-0.3.2.1/src/evidently/test_preset/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2707 2023-04-11 11:50:44.058127 evidently-0.3.2.1/src/evidently/test_preset/classification_binary.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1948 2023-04-11 11:50:44.058178 evidently-0.3.2.1/src/evidently/test_preset/classification_binary_topk.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2507 2023-04-11 11:50:44.058248 evidently-0.3.2.1/src/evidently/test_preset/classification_multiclass.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     7352 2023-04-27 10:27:02.410133 evidently-0.3.2.1/src/evidently/test_preset/data_drift.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1482 2023-04-11 11:50:44.058356 evidently-0.3.2.1/src/evidently/test_preset/data_quality.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1559 2023-04-11 11:50:44.058402 evidently-0.3.2.1/src/evidently/test_preset/data_stability.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     6811 2023-04-27 10:27:02.410385 evidently-0.3.2.1/src/evidently/test_preset/no_target_performance.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      750 2023-04-11 11:50:44.058506 evidently-0.3.2.1/src/evidently/test_preset/regression.py
+-rw-r--r--   0 emelidral   (501) staff       (20)      298 2023-04-11 11:50:44.058559 evidently-0.3.2.1/src/evidently/test_preset/test_preset.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.032945 evidently-0.3.2.1/src/evidently/test_suite/
+-rw-r--r--   0 emelidral   (501) staff       (20)       34 2023-04-11 11:50:44.058625 evidently-0.3.2.1/src/evidently/test_suite/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8647 2023-05-19 15:16:08.560630 evidently-0.3.2.1/src/evidently/test_suite/test_suite.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.034615 evidently-0.3.2.1/src/evidently/tests/
+-rw-r--r--   0 emelidral   (501) staff       (20)     4460 2023-04-27 10:27:02.410897 evidently-0.3.2.1/src/evidently/tests/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    11758 2023-04-11 11:50:44.058862 evidently-0.3.2.1/src/evidently/tests/base_test.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    22752 2023-04-11 11:50:44.059177 evidently-0.3.2.1/src/evidently/tests/classification_performance_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    21931 2023-05-19 15:16:08.560789 evidently-0.3.2.1/src/evidently/tests/data_drift_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    42332 2023-04-27 10:27:02.411682 evidently-0.3.2.1/src/evidently/tests/data_integrity_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    53681 2023-04-27 10:27:02.412175 evidently-0.3.2.1/src/evidently/tests/data_quality_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    10930 2023-04-11 11:50:44.059579 evidently-0.3.2.1/src/evidently/tests/regression_performance_tests.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    16360 2023-04-11 11:50:44.059661 evidently-0.3.2.1/src/evidently/tests/utils.py
+drwxr-xr-x   0 emelidral   (501) staff       (20)        0 2023-05-22 10:49:13.036582 evidently-0.3.2.1/src/evidently/utils/
+-rw-r--r--   0 emelidral   (501) staff       (20)       40 2023-04-11 11:50:44.059731 evidently-0.3.2.1/src/evidently/utils/__init__.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     5800 2023-04-11 11:50:44.059794 evidently-0.3.2.1/src/evidently/utils/dashboard.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     9086 2023-04-27 10:27:02.412473 evidently-0.3.2.1/src/evidently/utils/data_drift_utils.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     8133 2023-04-11 11:50:44.059931 evidently-0.3.2.1/src/evidently/utils/data_operations.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    20996 2023-04-11 11:50:44.060030 evidently-0.3.2.1/src/evidently/utils/data_preprocessing.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     4375 2023-04-11 11:50:44.060100 evidently-0.3.2.1/src/evidently/utils/generators.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     1392 2023-04-24 17:06:50.391821 evidently-0.3.2.1/src/evidently/utils/numpy_encoder.py
+-rw-r--r--   0 emelidral   (501) staff       (20)     2262 2023-04-11 11:50:44.060206 evidently-0.3.2.1/src/evidently/utils/types.py
+-rw-r--r--   0 emelidral   (501) staff       (20)    35867 2023-05-19 15:16:08.561016 evidently-0.3.2.1/src/evidently/utils/visualizations.py
```

### Comparing `evidently-0.3.2/setup.cfg` & `evidently-0.3.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/setup.py` & `evidently-0.3.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/setupbase.py` & `evidently-0.3.2.1/setupbase.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/__main__.py` & `evidently-0.3.2.1/src/evidently/__main__.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/base_metric.py` & `evidently-0.3.2.1/src/evidently/base_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/classification_performance.py` & `evidently-0.3.2.1/src/evidently/calculations/classification_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/data_drift.py` & `evidently-0.3.2.1/src/evidently/calculations/data_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/data_integration.py` & `evidently-0.3.2.1/src/evidently/calculations/data_integration.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/data_quality.py` & `evidently-0.3.2.1/src/evidently/calculations/data_quality.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/regression_performance.py` & `evidently-0.3.2.1/src/evidently/calculations/regression_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/__init__.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/__init__.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/anderson_darling_stattest.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/anderson_darling_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/chisquare_stattest.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/chisquare_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/cramer_von_mises_stattest.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/cramer_von_mises_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/energy_distance.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/energy_distance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/epps_singleton_stattest.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/epps_singleton_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/fisher_exact_stattest.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/fisher_exact_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/g_stattest.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/g_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/hellinger_distance.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/hellinger_distance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/jensenshannon.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/jensenshannon.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/kl_div.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/kl_div.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/ks_stattest.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/ks_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/mann_whitney_urank_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/mmd_stattest.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/mmd_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/psi.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/psi.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/registry.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/registry.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/t_test.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/t_test.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/text_content_drift.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/text_content_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/text_content_drift_abs.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/text_content_drift_abs.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/tvd_stattest.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/tvd_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/utils.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/wasserstein_distance_norm.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/wasserstein_distance_norm.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/stattests/z_stattest.py` & `evidently-0.3.2.1/src/evidently/calculations/stattests/z_stattest.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/calculations/utils.py` & `evidently-0.3.2.1/src/evidently/calculations/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/core.py` & `evidently-0.3.2.1/src/evidently/core.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/descriptors/non_letter_character_percentage_descriptor.py` & `evidently-0.3.2.1/src/evidently/descriptors/non_letter_character_percentage_descriptor.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/descriptors/oov_words_percentage_descriptor.py` & `evidently-0.3.2.1/src/evidently/descriptors/oov_words_percentage_descriptor.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/descriptors/trigger_words_presence_descriptor.py` & `evidently-0.3.2.1/src/evidently/descriptors/trigger_words_presence_descriptor.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/features/OOV_words_percentage_feature.py` & `evidently-0.3.2.1/src/evidently/features/OOV_words_percentage_feature.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/features/generated_features.py` & `evidently-0.3.2.1/src/evidently/features/generated_features.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/features/non_letter_character_percentage_feature.py` & `evidently-0.3.2.1/src/evidently/features/non_letter_character_percentage_feature.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/features/text_length_feature.py` & `evidently-0.3.2.1/src/evidently/features/text_length_feature.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/features/trigger_words_presence_feature.py` & `evidently-0.3.2.1/src/evidently/features/trigger_words_presence_feature.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metric_preset/classification_performance.py` & `evidently-0.3.2.1/src/evidently/metric_preset/classification_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metric_preset/data_drift.py` & `evidently-0.3.2.1/src/evidently/metric_preset/data_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metric_preset/data_quality.py` & `evidently-0.3.2.1/src/evidently/metric_preset/data_quality.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metric_preset/regression_performance.py` & `evidently-0.3.2.1/src/evidently/metric_preset/regression_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metric_preset/target_drift.py` & `evidently-0.3.2.1/src/evidently/metric_preset/target_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metric_preset/text_overview.py` & `evidently-0.3.2.1/src/evidently/metric_preset/text_overview.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metric_results.py` & `evidently-0.3.2.1/src/evidently/metric_results.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/__init__.py` & `evidently-0.3.2.1/src/evidently/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/base_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/base_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/classification_performance/base_classification_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/classification_performance/base_classification_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/classification_performance/class_balance_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/classification_performance/class_balance_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/classification_performance/class_separation_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/classification_performance/class_separation_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/classification_performance/classification_dummy_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/classification_performance/classification_dummy_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/classification_performance/classification_quality_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/classification_performance/classification_quality_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/classification_performance/confusion_matrix_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/classification_performance/confusion_matrix_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/classification_performance/objects.py` & `evidently-0.3.2.1/src/evidently/metrics/classification_performance/objects.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/classification_performance/pr_curve_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/classification_performance/pr_curve_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/classification_performance/pr_table_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/classification_performance/pr_table_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/classification_performance/probability_distribution_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/classification_performance/probability_distribution_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/classification_performance/quality_by_class_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/classification_performance/quality_by_class_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/classification_performance/quality_by_feature_table.py` & `evidently-0.3.2.1/src/evidently/metrics/classification_performance/quality_by_feature_table.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/classification_performance/roc_curve_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/classification_performance/roc_curve_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_drift/column_drift_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_drift/column_drift_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from tkinter import N
 from typing import List
 from typing import Optional
 from typing import Union
 
 import numpy as np
 import pandas as pd
```

### Comparing `evidently-0.3.2/src/evidently/metrics/data_drift/column_value_plot.py` & `evidently-0.3.2.1/src/evidently/metrics/data_drift/column_value_plot.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_drift/data_drift_table.py` & `evidently-0.3.2.1/src/evidently/metrics/data_drift/data_drift_table.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_drift/dataset_drift_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_drift/dataset_drift_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_drift/embedding_drift_methods.py` & `evidently-0.3.2.1/src/evidently/metrics/data_drift/embedding_drift_methods.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_drift/embeddings_drift.py` & `evidently-0.3.2.1/src/evidently/metrics/data_drift/embeddings_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_drift/target_by_features_table.py` & `evidently-0.3.2.1/src/evidently/metrics/data_drift/target_by_features_table.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_drift/text_descriptors_drift_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_drift/text_domain_classifier_drift_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_integrity/column_missing_values_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_integrity/column_missing_values_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_integrity/column_regexp_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_integrity/column_regexp_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_integrity/column_summary_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_integrity/column_summary_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_integrity/dataset_missing_values_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_integrity/dataset_summary_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_integrity/dataset_summary_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_quality/column_correlations_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_quality/column_correlations_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_quality/column_distribution_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_quality/column_distribution_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_quality/column_quantile_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_quality/column_quantile_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_quality/column_value_list_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_quality/column_value_list_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_quality/column_value_range_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_quality/column_value_range_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_quality/conflict_prediction_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_quality/conflict_prediction_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_quality/conflict_target_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_quality/conflict_target_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_quality/dataset_correlations_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_quality/dataset_correlations_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_quality/stability_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_quality/stability_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/data_quality/text_descriptors_correlation_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/data_quality/text_descriptors_distribution.py` & `evidently-0.3.2.1/src/evidently/metrics/data_quality/text_descriptors_distribution.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py` & `evidently-0.3.2.1/src/evidently/metrics/regression_performance/abs_perc_error_in_time.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/regression_performance/error_bias_table.py` & `evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_bias_table.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/regression_performance/error_distribution.py` & `evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_distribution.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/regression_performance/error_in_time.py` & `evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_in_time.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/regression_performance/error_normality.py` & `evidently-0.3.2.1/src/evidently/metrics/regression_performance/error_normality.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/regression_performance/objects.py` & `evidently-0.3.2.1/src/evidently/metrics/regression_performance/objects.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py` & `evidently-0.3.2.1/src/evidently/metrics/regression_performance/predicted_and_actual_in_time.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/regression_performance/predicted_vs_actual.py` & `evidently-0.3.2.1/src/evidently/metrics/regression_performance/predicted_vs_actual.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/regression_performance/regression_dummy_metric.py` & `evidently-0.3.2.1/src/evidently/metrics/regression_performance/regression_dummy_metric.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/regression_performance/regression_performance_metrics.py` & `evidently-0.3.2.1/src/evidently/metrics/regression_performance/regression_performance_metrics.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/regression_performance/regression_quality.py` & `evidently-0.3.2.1/src/evidently/metrics/regression_performance/regression_quality.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/regression_performance/top_error.py` & `evidently-0.3.2.1/src/evidently/metrics/regression_performance/top_error.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/regression_performance/utils.py` & `evidently-0.3.2.1/src/evidently/metrics/regression_performance/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/regression_performance/visualization.py` & `evidently-0.3.2.1/src/evidently/metrics/regression_performance/visualization.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/metrics/utils.py` & `evidently-0.3.2.1/src/evidently/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/model/widget.py` & `evidently-0.3.2.1/src/evidently/model/widget.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/nbextension/static/index.js` & `evidently-0.3.2.1/src/evidently/nbextension/static/index.js`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/nbextension/static/index.js.LICENSE.txt` & `evidently-0.3.2.1/src/evidently/nbextension/static/index.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/nbextension/static/material-ui-icons.woff2` & `evidently-0.3.2.1/src/evidently/nbextension/static/material-ui-icons.woff2`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/options/base.py` & `evidently-0.3.2.1/src/evidently/options/base.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/options/color_scheme.py` & `evidently-0.3.2.1/src/evidently/options/color_scheme.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/options/data_drift.py` & `evidently-0.3.2.1/src/evidently/options/data_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/options/quality_metrics.py` & `evidently-0.3.2.1/src/evidently/options/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/pipeline/column_mapping.py` & `evidently-0.3.2.1/src/evidently/pipeline/column_mapping.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/renderers/base_renderer.py` & `evidently-0.3.2.1/src/evidently/renderers/base_renderer.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/renderers/html_widgets.py` & `evidently-0.3.2.1/src/evidently/renderers/html_widgets.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/renderers/notebook_utils.py` & `evidently-0.3.2.1/src/evidently/renderers/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/renderers/render_utils.py` & `evidently-0.3.2.1/src/evidently/renderers/render_utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/report/report.py` & `evidently-0.3.2.1/src/evidently/report/report.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/runner/loader.py` & `evidently-0.3.2.1/src/evidently/runner/loader.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/runner/runner.py` & `evidently-0.3.2.1/src/evidently/runner/runner.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/suite/base_suite.py` & `evidently-0.3.2.1/src/evidently/suite/base_suite.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/suite/execution_graph.py` & `evidently-0.3.2.1/src/evidently/suite/execution_graph.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/telemetry/sender.py` & `evidently-0.3.2.1/src/evidently/telemetry/sender.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/test_preset/__init__.py` & `evidently-0.3.2.1/src/evidently/test_preset/__init__.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/test_preset/classification_binary.py` & `evidently-0.3.2.1/src/evidently/test_preset/classification_binary.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/test_preset/classification_binary_topk.py` & `evidently-0.3.2.1/src/evidently/test_preset/classification_binary_topk.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/test_preset/classification_multiclass.py` & `evidently-0.3.2.1/src/evidently/test_preset/classification_multiclass.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/test_preset/data_drift.py` & `evidently-0.3.2.1/src/evidently/test_preset/data_drift.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/test_preset/data_quality.py` & `evidently-0.3.2.1/src/evidently/test_preset/data_quality.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/test_preset/data_stability.py` & `evidently-0.3.2.1/src/evidently/test_preset/data_stability.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/test_preset/no_target_performance.py` & `evidently-0.3.2.1/src/evidently/test_preset/no_target_performance.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/test_preset/regression.py` & `evidently-0.3.2.1/src/evidently/test_preset/regression.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/test_suite/test_suite.py` & `evidently-0.3.2.1/src/evidently/test_suite/test_suite.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/tests/__init__.py` & `evidently-0.3.2.1/src/evidently/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/tests/base_test.py` & `evidently-0.3.2.1/src/evidently/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/tests/classification_performance_tests.py` & `evidently-0.3.2.1/src/evidently/tests/classification_performance_tests.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/tests/data_drift_tests.py` & `evidently-0.3.2.1/src/evidently/tests/data_drift_tests.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/tests/data_integrity_tests.py` & `evidently-0.3.2.1/src/evidently/tests/data_integrity_tests.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/tests/data_quality_tests.py` & `evidently-0.3.2.1/src/evidently/tests/data_quality_tests.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/tests/regression_performance_tests.py` & `evidently-0.3.2.1/src/evidently/tests/regression_performance_tests.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/tests/utils.py` & `evidently-0.3.2.1/src/evidently/tests/utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/utils/dashboard.py` & `evidently-0.3.2.1/src/evidently/utils/dashboard.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/utils/data_drift_utils.py` & `evidently-0.3.2.1/src/evidently/utils/data_drift_utils.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/utils/data_operations.py` & `evidently-0.3.2.1/src/evidently/utils/data_operations.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/utils/data_preprocessing.py` & `evidently-0.3.2.1/src/evidently/utils/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/utils/generators.py` & `evidently-0.3.2.1/src/evidently/utils/generators.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/utils/numpy_encoder.py` & `evidently-0.3.2.1/src/evidently/utils/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/utils/types.py` & `evidently-0.3.2.1/src/evidently/utils/types.py`

 * *Files identical despite different names*

### Comparing `evidently-0.3.2/src/evidently/utils/visualizations.py` & `evidently-0.3.2.1/src/evidently/utils/visualizations.py`

 * *Files identical despite different names*

