# Comparing `tmp/datumaro-1.2.1.tar.gz` & `tmp/datumaro-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.2.1.tar", last modified: Thu May  4 07:27:27 2023, max compression
+gzip compressed data, was "datumaro-1.3.0rc1.tar", last modified: Mon May 22 06:25:28 2023, max compression
```

## Comparing `datumaro-1.2.1.tar` & `datumaro-1.3.0rc1.tar`

### file list

```diff
@@ -1,321 +1,330 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.874663 datumaro-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)   373252 2023-05-04 07:27:17.000000 datumaro-1.2.1/3rd-party.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-04 07:27:17.000000 datumaro-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 07:27:17.000000 datumaro-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-04 07:27:17.000000 datumaro-1.2.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-05-04 07:27:27.874663 datumaro-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-05-04 07:27:17.000000 datumaro-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.814663 datumaro-1.2.1/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.814663 datumaro-1.2.1/datumaro/capi/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/capi/pybind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.814663 datumaro-1.2.1/datumaro/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.818663 datumaro-1.2.1/datumaro/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/detect_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.818663 datumaro-1.2.1/datumaro/cli/commands/require_project/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.818663 datumaro-1.2.1/datumaro/cli/commands/require_project/modification/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/modification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/modification/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/modification/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/modification/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/modification/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/modification/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.818663 datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/commands/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.822663 datumaro-1.2.1/datumaro/cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/contexts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.822663 datumaro-1.2.1/datumaro/cli/contexts/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/contexts/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/contexts/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/contexts/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.822663 datumaro-1.2.1/datumaro/cli/util/
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/util/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/cli/util/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.826663 datumaro-1.2.1/datumaro/components/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.826663 datumaro-1.2.1/datumaro/components/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/abstracts/merger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.830663 datumaro-1.2.1/datumaro/components/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.830663 datumaro-1.2.1/datumaro/components/algorithms/noisy_label_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/algorithms/rise.py
--rw-r--r--   0 runner    (1001) docker     (123)    29706 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.830663 datumaro-1.2.1/datumaro/components/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/annotations/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/annotations/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/config_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/crypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    46849 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/dataset_item_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13568 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/extractor_tfds.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19613 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/format_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.830663 datumaro-1.2.1/datumaro/components/hl_ops/
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/hl_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    36004 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/media_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.830663 datumaro-1.2.1/datumaro/components/merge/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/merge/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/merge/exact_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    24147 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/merge/intersect_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/merge/union_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    23487 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/progress_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    89332 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/components/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.834663 datumaro-1.2.1/datumaro/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.834663 datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.834663 datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/details/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/details/representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.842663 datumaro-1.2.1/datumaro/plugins/data_formats/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/ade20k2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/ade20k2020.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.842663 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/arrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.842663 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.846663 datumaro-1.2.1/datumaro/plugins/data_formats/ava/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/ava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/ava/ava.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/brats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/brats_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17438 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/camvid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.846663 datumaro-1.2.1/datumaro/plugins/data_formats/celeba/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/celeba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/celeba/celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20683 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/cityscapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.846663 datumaro-1.2.1/datumaro/plugins/data_formats/coco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19013 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/coco/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28658 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/coco/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/coco/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/coco/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/common_super_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.846663 datumaro-1.2.1/datumaro/plugins/data_formats/cvat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14166 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/cvat/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20627 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/cvat/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/cvat/format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.850663 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11047 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15377 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.850663 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.850663 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.854663 datumaro-1.2.1/datumaro/plugins/data_formats/icdar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/icdar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11780 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/icdar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/icdar/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/icdar/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/image_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/image_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/imagenet_txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.854663 datumaro-1.2.1/datumaro/plugins/data_formats/kitti/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.854663 datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11148 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17831 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    20175 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/labelme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/lfw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.858663 datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12550 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/market1501.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9041 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mnist_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6493 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.858663 datumaro-1.2.1/datumaro/plugins/data_formats/mpii/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mpii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mpii/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.858663 datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38486 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/open_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.858663 datumaro-1.2.1/datumaro/plugins/data_formats/sly_pointcloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16260 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/sly_pointcloud/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/synthia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.862663 datumaro-1.2.1/datumaro/plugins/data_formats/tf_detection_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8812 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/vgg_face2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.862663 datumaro-1.2.1/datumaro/plugins/data_formats/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/voc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    30069 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/voc/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9071 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/voc/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/voc/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/vott_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/vott_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10103 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/widerface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.866663 datumaro-1.2.1/datumaro/plugins/data_formats/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/yolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12397 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/yolo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/yolo/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/yolo/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/data_formats/yolo/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/ndr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.866663 datumaro-1.2.1/datumaro/plugins/openvino_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.866663 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.870663 datumaro-1.2.1/datumaro/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/sampler/relevancy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.870663 datumaro-1.2.1/datumaro/plugins/synthetic_data/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/synthetic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/synthetic_data/background_colors.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/synthetic_data/image_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/synthetic_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.870663 datumaro-1.2.1/datumaro/plugins/tiling/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/tiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/tiling/merge_tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/tiling/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/tiling/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    41240 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    44261 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.874663 datumaro-1.2.1/datumaro/util/
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/annotation_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/attrs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11440 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/mask_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/meta_file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/pickle_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/telemetry_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/telemetry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/util/tf_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 07:27:17.000000 datumaro-1.2.1/datumaro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:27:27.814663 datumaro-1.2.1/datumaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-05-04 07:27:27.000000 datumaro-1.2.1/datumaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-04 07:27:27.000000 datumaro-1.2.1/datumaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:27:27.000000 datumaro-1.2.1/datumaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 07:27:27.000000 datumaro-1.2.1/datumaro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-04 07:27:27.000000 datumaro-1.2.1/datumaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 07:27:27.000000 datumaro-1.2.1/datumaro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-04 07:27:17.000000 datumaro-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-04 07:27:17.000000 datumaro-1.2.1/requirements-core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-04 07:27:17.000000 datumaro-1.2.1/requirements-default.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:27:27.874663 datumaro-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-04 07:27:17.000000 datumaro-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.364167 datumaro-1.3.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)   373252 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/3rd-party.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-05-22 06:25:28.364167 datumaro-1.3.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.324166 datumaro-1.3.0rc1/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.324166 datumaro-1.3.0rc1/datumaro/capi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/capi/pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.324166 datumaro-1.3.0rc1/datumaro/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.328166 datumaro-1.3.0rc1/datumaro/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.328166 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.328166 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.328166 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.328166 datumaro-1.3.0rc1/datumaro/cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/contexts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.328166 datumaro-1.3.0rc1/datumaro/cli/contexts/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/contexts/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/contexts/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/contexts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.332166 datumaro-1.3.0rc1/datumaro/cli/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13328 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/util/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/cli/util/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.332166 datumaro-1.3.0rc1/datumaro/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/components/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/abstracts/merger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/components/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/components/algorithms/noisy_label_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/algorithms/rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29706 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/components/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8965 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/annotations/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/annotations/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/config_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/crypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48204 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10965 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/dataset_item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18012 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13772 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/extractor_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/format_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/components/hl_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/hl_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36004 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/media_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/components/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/merge/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/merge/exact_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24147 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/merge/intersect_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/merge/union_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23487 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/progress_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89679 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9352 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21450 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/components/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.336166 datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.348167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/ade20k2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/ade20k2020.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.348167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/arrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15037 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.348167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.348167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/ava/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/ava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/ava/ava.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/brats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/brats_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/camvid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.348167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/celeba/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12406 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20885 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.352167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20916 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28658 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/common_super_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.352167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/cvat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14327 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/cvat/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20627 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/cvat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.352167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15862 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.352167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11117 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.352167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.352167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/icdar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/icdar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/icdar/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/image_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/image_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7767 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/imagenet_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.356167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.356167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17887 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20296 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/labelme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15144 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/lfw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.356167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7214 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mnist_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.356167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.356167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38719 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/open_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.356167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/segment_anything/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/segment_anything/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/segment_anything/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.356167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16298 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/sly_pointcloud/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.360167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/synthia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/synthia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/synthia/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/synthia/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/synthia/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.360167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/tf_detection_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15649 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/vgg_face2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.360167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31317 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10660 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/vott_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/vott_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/widerface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.360167 datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12632 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5573 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/ndr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.360167 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.360167 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.360167 datumaro-1.3.0rc1/datumaro/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.364167 datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.364167 datumaro-1.3.0rc1/datumaro/plugins/tiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/tiling/merge_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/tiling/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/tiling/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47320 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44207 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.364167 datumaro-1.3.0rc1/datumaro/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/annotation_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/attrs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11657 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/mask_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/meta_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/pickle_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/telemetry_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/util/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/datumaro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 06:25:28.324166 datumaro-1.3.0rc1/datumaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6129 2023-05-22 06:25:28.000000 datumaro-1.3.0rc1/datumaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-05-22 06:25:28.000000 datumaro-1.3.0rc1/datumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 06:25:28.000000 datumaro-1.3.0rc1/datumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-22 06:25:28.000000 datumaro-1.3.0rc1/datumaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-22 06:25:28.000000 datumaro-1.3.0rc1/datumaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-22 06:25:28.000000 datumaro-1.3.0rc1/datumaro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/requirements-default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 06:25:28.364167 datumaro-1.3.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-05-22 06:25:14.000000 datumaro-1.3.0rc1/setup.py
```

### Comparing `datumaro-1.2.1/3rd-party.txt` & `datumaro-1.3.0rc1/3rd-party.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/LICENSE` & `datumaro-1.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/PKG-INFO` & `datumaro-1.3.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.2.1
+Version: 1.3.0rc1
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tf
 Provides-Extra: tfds
-Provides-Extra: tfds-dev
 Provides-Extra: tf-gpu
 Provides-Extra: default
 License-File: LICENSE
 License-File: NOTICE
 
 # Dataset Management Framework (Datumaro)
 
@@ -31,18 +30,19 @@
      +                                     /
 COCO dataset -----> Datumaro ---> dataset ------> Model training
      +                                     \
 CVAT annotations                             ---> Publication, statistics etc.
 ```
 <!--lint enable fenced-code-flag-->
 
-- [Getting started](https://openvinotoolkit.github.io/datumaro/docs/getting_started)
+- [Getting started](https://openvinotoolkit.github.io/datumaro/latest/docs/get-started/quick-start-guide)
+- [Level Up](https://openvinotoolkit.github.io/datumaro/latest/docs/level-up/basic_skills)
 - [Features](#features)
-- [User manual](https://openvinotoolkit.github.io/datumaro/docs/user-manual)
-- [Developer manual](https://openvinotoolkit.github.io/datumaro/api)
+- [User manual](https://openvinotoolkit.github.io/datumaro/latest/docs/user-manual/how_to_use_datumaro)
+- [Developer manual](https://openvinotoolkit.github.io/datumaro/latest/docs/reference/datumaro/datumaro)
 - [Contributing](#contributing)
 
 ## Features
 
 [(Back to top)](#dataset-management-framework-datumaro)
 
 - Dataset reading, writing, conversion in any direction.
@@ -61,15 +61,15 @@
   - [Open Images](https://storage.googleapis.com/openimages/web/download.html)
   - [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/voc2012/htmldoc/index.html)
     (`classification`, `detection`, `segmentation`, `action_classification`, `person_layout`)
   - [TF Detection API](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/using_your_own_dataset.md)
     (`bboxes`, `masks`)
   - [YOLO](https://github.com/AlexeyAB/darknet#how-to-train-pascal-voc-data) (`bboxes`)
 
-  Other formats and documentation for them can be found [here](https://openvinotoolkit.github.io/datumaro/docs/user-manual/supported_formats).
+  Other formats and documentation for them can be found [here](https://openvinotoolkit.github.io/datumaro/latest/docs/data-formats/supported_formats).
 - Dataset building
   - Merging multiple datasets into one
   - Dataset filtering by a custom criteria:
     - remove polygons of a certain class
     - remove images without annotations of a specific class
     - remove `occluded` annotations from images
     - keep only vertically-oriented images
@@ -101,30 +101,30 @@
 - Model integration
   - Inference (OpenVINO, Caffe, PyTorch, TensorFlow, MxNet, etc.)
   - Explainable AI ([RISE algorithm](https://arxiv.org/abs/1806.07421))
     - RISE for classification
     - RISE for object detection
 
 > Check
-  [the design document](https://openvinotoolkit.github.io/datumaro/docs/design)
+  [the design document](https://openvinotoolkit.github.io/datumaro/latest/docs/explanation/architecture)
   for a full list of features.
 > Check
-  [the user manual](https://openvinotoolkit.github.io/datumaro/docs/user-manual)
+  [the user manual](https://openvinotoolkit.github.io/datumaro/latest/docs/user-manual/how_to_use_datumaro)
   for usage instructions.
 
 ## Contributing
 
 [(Back to top)](#dataset-management-framework-datumaro)
 
 Feel free to
 [open an Issue](https://github.com/openvinotoolkit/datumaro/issues/new), if you
 think something needs to be changed. You are welcome to participate in
 development, instructions are available in our
-[contribution guide](https://openvinotoolkit.github.io/datumaro/docs/contributing).
+[contribution guide](https://github.com/openvinotoolkit/datumaro/blob/develop/contributing.md).
 
 ## Telemetry data collection note
 
 The [OpenVINO™ telemetry library](https://github.com/openvinotoolkit/telemetry/)
 is used to collect basic information about Datumaro usage.
 
 To enable/disable telemetry data collection please see the
-[guide](https://openvinotoolkit.github.io/datumaro/docs/user-manual/how_to_control_tm_data_collection/).
+[guide](https://openvinotoolkit.github.io/datumaro/latest/docs/user-manual/how_to_control_tm_data_collection).
```

### Comparing `datumaro-1.2.1/README.md` & `datumaro-1.3.0rc1/datumaro.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: datumaro
+Version: 1.3.0rc1
+Summary: Dataset Management Framework (Datumaro)
+Home-page: https://github.com/openvinotoolkit/datumaro
+Author: Intel
+Author-email: emily.chun@intel.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: tf
+Provides-Extra: tfds
+Provides-Extra: tf-gpu
+Provides-Extra: default
+License-File: LICENSE
+License-File: NOTICE
+
 # Dataset Management Framework (Datumaro)
 
 [![Build status](https://github.com/openvinotoolkit/datumaro/actions/workflows/health_check.yml/badge.svg)](https://github.com/openvinotoolkit/datumaro/actions/workflows/health_check.yml)
 [![codecov](https://codecov.io/gh/openvinotoolkit/datumaro/branch/develop/graph/badge.svg?token=FG25VU096Q)](https://codecov.io/gh/openvinotoolkit/datumaro)
 
 A framework and CLI tool to build, transform, and analyze datasets.
 
@@ -11,18 +30,19 @@
      +                                     /
 COCO dataset -----> Datumaro ---> dataset ------> Model training
      +                                     \
 CVAT annotations                             ---> Publication, statistics etc.
 ```
 <!--lint enable fenced-code-flag-->
 
-- [Getting started](https://openvinotoolkit.github.io/datumaro/docs/getting_started)
+- [Getting started](https://openvinotoolkit.github.io/datumaro/latest/docs/get-started/quick-start-guide)
+- [Level Up](https://openvinotoolkit.github.io/datumaro/latest/docs/level-up/basic_skills)
 - [Features](#features)
-- [User manual](https://openvinotoolkit.github.io/datumaro/docs/user-manual)
-- [Developer manual](https://openvinotoolkit.github.io/datumaro/api)
+- [User manual](https://openvinotoolkit.github.io/datumaro/latest/docs/user-manual/how_to_use_datumaro)
+- [Developer manual](https://openvinotoolkit.github.io/datumaro/latest/docs/reference/datumaro/datumaro)
 - [Contributing](#contributing)
 
 ## Features
 
 [(Back to top)](#dataset-management-framework-datumaro)
 
 - Dataset reading, writing, conversion in any direction.
@@ -41,15 +61,15 @@
   - [Open Images](https://storage.googleapis.com/openimages/web/download.html)
   - [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/voc2012/htmldoc/index.html)
     (`classification`, `detection`, `segmentation`, `action_classification`, `person_layout`)
   - [TF Detection API](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/using_your_own_dataset.md)
     (`bboxes`, `masks`)
   - [YOLO](https://github.com/AlexeyAB/darknet#how-to-train-pascal-voc-data) (`bboxes`)
 
-  Other formats and documentation for them can be found [here](https://openvinotoolkit.github.io/datumaro/docs/user-manual/supported_formats).
+  Other formats and documentation for them can be found [here](https://openvinotoolkit.github.io/datumaro/latest/docs/data-formats/supported_formats).
 - Dataset building
   - Merging multiple datasets into one
   - Dataset filtering by a custom criteria:
     - remove polygons of a certain class
     - remove images without annotations of a specific class
     - remove `occluded` annotations from images
     - keep only vertically-oriented images
@@ -81,30 +101,30 @@
 - Model integration
   - Inference (OpenVINO, Caffe, PyTorch, TensorFlow, MxNet, etc.)
   - Explainable AI ([RISE algorithm](https://arxiv.org/abs/1806.07421))
     - RISE for classification
     - RISE for object detection
 
 > Check
-  [the design document](https://openvinotoolkit.github.io/datumaro/docs/design)
+  [the design document](https://openvinotoolkit.github.io/datumaro/latest/docs/explanation/architecture)
   for a full list of features.
 > Check
-  [the user manual](https://openvinotoolkit.github.io/datumaro/docs/user-manual)
+  [the user manual](https://openvinotoolkit.github.io/datumaro/latest/docs/user-manual/how_to_use_datumaro)
   for usage instructions.
 
 ## Contributing
 
 [(Back to top)](#dataset-management-framework-datumaro)
 
 Feel free to
 [open an Issue](https://github.com/openvinotoolkit/datumaro/issues/new), if you
 think something needs to be changed. You are welcome to participate in
 development, instructions are available in our
-[contribution guide](https://openvinotoolkit.github.io/datumaro/docs/contributing).
+[contribution guide](https://github.com/openvinotoolkit/datumaro/blob/develop/contributing.md).
 
 ## Telemetry data collection note
 
 The [OpenVINO™ telemetry library](https://github.com/openvinotoolkit/telemetry/)
 is used to collect basic information about Datumaro usage.
 
 To enable/disable telemetry data collection please see the
-[guide](https://openvinotoolkit.github.io/datumaro/docs/user-manual/how_to_control_tm_data_collection/).
+[guide](https://openvinotoolkit.github.io/datumaro/latest/docs/user-manual/how_to_control_tm_data_collection).
```

### Comparing `datumaro-1.2.1/datumaro/__init__.py` & `datumaro-1.3.0rc1/datumaro/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/capi/pybind.cpp` & `datumaro-1.3.0rc1/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/__main__.py` & `datumaro-1.3.0rc1/datumaro/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/__init__.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/convert.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/detect_format.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/diff.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/diff.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/download.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/explain.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/explore.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/explore.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
+import os
 import os.path as osp
-
-import numpy as np
+import shutil
 
 from datumaro.components.errors import ProjectNotFoundError
 from datumaro.components.explorer import Explorer
-from datumaro.components.visualizer import Visualizer
-from datumaro.util.image import save_image
+from datumaro.util import str_to_bool
 from datumaro.util.scope import scope_add, scoped
 
 from ..util import MultilineFormatter
 from ..util.project import load_project, parse_full_revpath
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
@@ -38,18 +37,15 @@
         |s|s%(prog)s -q path/to/image1.jpg/ path/to/image2.jpg/ path/to/image3.jpg/ -topk 50|n
         - Explore top50 similar images of text query list in COCO dataset:|n
         |s|s%(prog)s -q motorcycle/ bus/ train/ -topk 50
         """,
         formatter_class=MultilineFormatter,
     )
 
-    parser.add_argument(
-        "_positionals", nargs=argparse.REMAINDER, help=argparse.SUPPRESS
-    )  # workaround for -- eaten by positionals
-    parser.add_argument("target", nargs="+", default="project", help="Target dataset")
+    parser.add_argument("target", nargs="?", help="Target dataset")
     parser.add_argument(
         "-q",
         "--query",
         dest="query",
         required=True,
         help="Image path or id of query to explore similar data",
     )
@@ -57,68 +53,109 @@
     parser.add_argument(
         "-p",
         "--project",
         dest="project_dir",
         help="Directory of the project to operate on (default: current dir)",
     )
     parser.add_argument(
-        "-s", "--save", dest="save", default=True, help="Save explorer result as png"
+        "-s",
+        "--save",
+        action="store_true",
+        default=False,
+        help="Save explorer result files on explore_result folder",
+    )
+    parser.add_argument(
+        "--stage",
+        type=str_to_bool,
+        default=True,
+        help="""
+            Include this action as a project build step.
+            If true, this operation will be saved in the project
+            build tree, allowing to reproduce the resulting dataset later.
+            Applicable only to main project targets (i.e. data sources
+            and the 'project' target, but not intermediate stages)
+            (default: %(default)s)
+            """,
     )
-
     parser.set_defaults(command=explore_command)
 
     return parser
 
 
 def get_sensitive_args():
     return {
         explore_command: [
             "target",
             "query",
             "topk",
-            "save",
+            "project_dir",
         ]
     }
 
 
 @scoped
 def explore_command(args):
     project = None
     try:
         project = scope_add(load_project(args.project_dir))
     except ProjectNotFoundError:
         if args.project_dir:
             raise
 
-    dataset, _ = parse_full_revpath(args.target[0], project)
+    if args.target:
+        targets = [args.target]
+    else:
+        targets = list(project.working_tree.sources)
 
-    explorer = Explorer(dataset)
+    source_datasets = []
+    for target in targets:
+        target_dataset, _ = parse_full_revpath(target, project)
+        source_datasets.append(target_dataset)
+
+    explorer_args = {"save_hashkey": True}
+    build_tree = project.working_tree.clone()
+    for target in targets:
+        build_tree.build_targets.add_explore_stage(target, params=explorer_args)
+
+    explorer = Explorer(*source_datasets)
+    for dataset in source_datasets:
+        dst_dir = dataset.data_path
+        dataset.save(dst_dir, save_media=True)
+
+    if args.stage:
+        project.working_tree.config.update(build_tree.config)
+        project.working_tree.save()
 
     # Get query datasetitem through query path
     if osp.exists(args.query):
-        query_datasetitem = dataset.get_datasetitem_by_path(args.query)
+        query_datasetitem = None
+        for dataset in source_datasets:
+            try:
+                query_datasetitem = dataset.get_datasetitem_by_path(args.query)
+            except Exception:
+                continue
+            if not query_datasetitem:
+                break
     else:
         query_datasetitem = args.query
 
     results = explorer.explore_topk(query_datasetitem, args.topk)
 
-    subset_list = []
-    id_list = []
     result_path_list = []
-    log.info("Most similar {} results of query in dataset".format(args.topk))
+    log.info(f"Most similar {args.topk} results of query in dataset")
     for result in results:
-        subset_list.append(result.subset)
-        id_list.append(result.id)
         path = getattr(result.media, "path", None)
         result_path_list.append(path)
-        log.info("id: {} | subset: {} | path : {}".format(result.id, result.subset, path))
-
-    visualizer = Visualizer(dataset, figsize=(20, 20), alpha=0)
-    fig = visualizer.vis_gallery(id_list, subset_list)
+        log.info(f"id: {result.id} | subset: {result.subset} | path : {path}")
 
     if args.save:
-        fig.canvas.draw()
-        data = np.frombuffer(fig.canvas.tostring_rgb(), dtype=np.uint8)
-        data = data.reshape(fig.canvas.get_width_height()[::-1] + (3,))
-        save_image(osp.join("./explorer.png"), data, create_dir=True)
+        saved_result_path = osp.join(args.project_dir, "explore_result")
+        if osp.exists(saved_result_path):
+            shutil.rmtree(saved_result_path)
+        os.makedirs(saved_result_path)
+        for result in results:
+            saved_subset_path = osp.join(saved_result_path, result.subset)
+            if not osp.exists(saved_subset_path):
+                os.makedirs(saved_subset_path)
+            shutil.copyfile(path, osp.join(saved_subset_path, result.id + ".jpg"))
 
     return 0
```

### Comparing `datumaro-1.2.1/datumaro/cli/commands/filter.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/generate.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/info.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/merge.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/patch.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/patch.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/require_project/__init__.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/add.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/require_project/modification/export.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/export.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/stats.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/stats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/transform.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/transform.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/commands/validate.py` & `datumaro-1.3.0rc1/datumaro/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/contexts/model.py` & `datumaro-1.3.0rc1/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/contexts/project/__init__.py` & `datumaro-1.3.0rc1/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/contexts/source.py` & `datumaro-1.3.0rc1/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/contexts/util.py` & `datumaro-1.3.0rc1/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/util/__init__.py` & `datumaro-1.3.0rc1/datumaro/cli/util/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 def show_video_import_warning():
     log.warning(
         "Using 'video_frames' in a project may lead "
         "to different results across multiple runs, if the "
         "system setup changes (library version, OS, etc.). "
         "If you need stable results, consider splitting the video "
         "manually using instructions at: "
-        "https://openvinotoolkit.github.io/datumaro/docs/media_formats/"
+        "https://openvinotoolkit.github.io/datumaro/latest/docs/data-formats/media_formats"
     )
 
 
 def make_subcommands_help(commands, help_line_start=0):
     desc = ""
     for command_name, command_type, command_help in commands:
         msg = ("  %-" + str(max(0, help_line_start - 2 - 1)) + "s%s\n") % (
```

### Comparing `datumaro-1.2.1/datumaro/cli/util/diff.py` & `datumaro-1.3.0rc1/datumaro/cli/util/diff.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/cli/util/project.py` & `datumaro-1.3.0rc1/datumaro/cli/util/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/abstracts/merger.py` & `datumaro-1.3.0rc1/datumaro/components/abstracts/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-1.3.0rc1/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/algorithms/rise.py` & `datumaro-1.3.0rc1/datumaro/components/algorithms/rise.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/annotation.py` & `datumaro-1.3.0rc1/datumaro/components/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/annotations/matcher.py` & `datumaro-1.3.0rc1/datumaro/components/annotations/matcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/annotations/merger.py` & `datumaro-1.3.0rc1/datumaro/components/annotations/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/cli_plugin.py` & `datumaro-1.3.0rc1/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/config.py` & `datumaro-1.3.0rc1/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/config_model.py` & `datumaro-1.3.0rc1/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/crypter.py` & `datumaro-1.3.0rc1/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/dataset.py` & `datumaro-1.3.0rc1/datumaro/components/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     DatasetItemStorage,
     DatasetItemStorageDatasetView,
 )
 from datumaro.components.environment import DEFAULT_ENVIRONMENT, Environment
 from datumaro.components.errors import (
     CategoriesRedefinedError,
     ConflictingCategoriesError,
+    DatasetImportError,
     DatasetInfosRedefinedError,
     MediaTypeError,
     MultipleFormatsMatchError,
     NoMatchingFormatsError,
     RepeatedItemError,
     UnknownFormatError,
 )
@@ -262,16 +263,21 @@
 
         class _StackedTransform(Transform):
             def __init__(self, source, transforms):
                 super().__init__(source)
 
                 self.is_local = True
                 self.transforms: List[Transform] = []
-                for transform in transforms:
-                    source = transform[0](source, *transform[1], **transform[2])
+                self.malformed_transform_indices: Dict[int, Exception] = {}
+                for idx, transform in enumerate(transforms):
+                    try:
+                        source = transform[0](source, *transform[1], **transform[2])
+                    except Exception as e:
+                        self.malformed_transform_indices[idx] = e
+
                     self.transforms.append(source)
 
                     if self.is_local and not isinstance(source, ItemTransform):
                         self.is_local = False
 
             def transform_item(self, item):
                 for t in self.transforms:
@@ -336,14 +342,16 @@
 
             if not issubclass(transform.media_type(), media_type):
                 # TODO: make it statically available
                 raise MediaTypeError(
                     "Transforms are not allowed to change media " "type of dataset items"
                 )
 
+            self._drop_malformed_transforms(transform.malformed_transform_indices)
+
         i = -1
         for i, item in enumerate(source):
             if item.media and not isinstance(item.media, media_type):
                 raise MediaTypeError(
                     "Unexpected media type of a dataset item '%s'. "
                     "Expected '%s', actual '%s' " % (item.id, media_type, type(item.media))
                 )
@@ -621,14 +629,29 @@
                 source, self.categories().get(AnnotationType.label, LabelCategories())
             ):
                 self.put(item)
         else:
             for item in source:
                 self.put(item)
 
+    def _drop_malformed_transforms(self, malformed_transform_indices: Dict[int, Exception]) -> None:
+        safe_transforms = []
+        for idx, transform in enumerate(self._transforms):
+            if idx in malformed_transform_indices:
+                log.error(
+                    f"Automatically drop {transform} from the transform stack because an error is raised. "
+                    "Therefore, the dataset will not be transformed by this transformation since it is droped.",
+                    exc_info=malformed_transform_indices[idx],
+                )
+                continue
+
+            safe_transforms += [transform]
+
+        self._transforms = safe_transforms
+
 
 class Dataset(IDataset):
     """
     Represents a dataset, contains metainfo about labels and dataset items.
     Provides iteration and access options to dataset elements.
 
     By default, all operations are done lazily, it can be changed by
@@ -1245,15 +1268,19 @@
                         env.make_extractor(src_conf.format, src_conf.url, **extractor_kwargs)
                     )
 
             dataset = cls.from_extractors(*extractors, env=env, merge_policy=merge_policy)
             if eager:
                 dataset.init_cache()
         except _ImportFail as e:
-            raise e.__cause__
+            cause = e.__cause__ if getattr(e, "__cause__", None) is not None else e
+            cause.__traceback__ = e.__traceback__
+            raise DatasetImportError(f"Failed to import dataset '{format}' at '{path}'.") from cause
+        except Exception as e:
+            raise DatasetImportError(f"Failed to import dataset '{format}' at '{path}'.") from e
 
         dataset._source_path = path
         dataset._format = format
 
         return dataset
 
     @staticmethod
```

### Comparing `datumaro-1.2.1/datumaro/components/dataset_base.py` & `datumaro-1.3.0rc1/datumaro/components/dataset_base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/dataset_item_storage.py` & `datumaro-1.3.0rc1/datumaro/components/dataset_item_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/environment.py` & `datumaro-1.3.0rc1/datumaro/components/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,15 +290,17 @@
 
         max_conf = (
             max(all_matched_formats).confidence
             if len(all_matched_formats) > 0
             else FormatDetectionConfidence.NONE
         )
 
-        return [str(format) for format in all_matched_formats if format.confidence == max_conf]
+        return sorted(
+            [str(format) for format in all_matched_formats if format.confidence == max_conf]
+        )
 
     def __reduce__(self):
         return (self.__class__, ())
 
     @classmethod
     def merge(cls, envs: Sequence["Environment"]) -> "Environment":
         if all([env == DEFAULT_ENVIRONMENT for env in envs]):
```

### Comparing `datumaro-1.2.1/datumaro/components/errors.py` & `datumaro-1.3.0rc1/datumaro/components/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,18 +268,20 @@
 class AnnotationImportError(ItemImportError):
     def __str__(self):
         return f"Failed to import item {self.item_id} annotation: {self.__cause__}"
 
 
 @define(auto_exc=False)
 class DatasetNotFoundError(DatasetImportError):
-    path = field()
+    path: str = field()
+    format: str = field()
+    template: str = field(default="Failed to find dataset '{format}' at '{path}'")
 
     def __str__(self):
-        return f"Failed to find dataset at '{self.path}'"
+        return self.template.format(path=self.path, format=self.format)
 
 
 @define(auto_exc=False)
 class MultipleFormatsMatchError(DatasetImportError):
     formats = field()
 
     def __str__(self):
```

### Comparing `datumaro-1.2.1/datumaro/components/explorer.py` & `datumaro-1.3.0rc1/datumaro/components/explorer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,102 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-from typing import List, Optional, Union
+from typing import List, Optional, Sequence, Union
 
 import numpy as np
 
 from datumaro.components.annotation import HashKey
-from datumaro.components.dataset import IDataset
+from datumaro.components.dataset import Dataset
 from datumaro.components.dataset_base import DatasetItem
 from datumaro.components.errors import MediaTypeError
-from datumaro.components.media import Image
+from datumaro.components.media import Image, MediaElement
 from datumaro.plugins.explorer import ExplorerLauncher
 
 
 def calculate_hamming(B1, B2):
     """
     :param B1:  vector [n]
     :param B2:  vector [r*n]
     :return: hamming distance [r]
     """
     q = B2.shape[1]  # max inner product value
     distH = 0.5 * (q - B1 @ B2.transpose())
     return distH
 
 
+def select_uninferenced_dataset(dataset):
+    uninferenced_dataset = Dataset(media_type=MediaElement)
+    for item in dataset:
+        if not any(isinstance(annotation, HashKey) for annotation in item.annotations):
+            uninferenced_dataset.put(item)
+    return uninferenced_dataset
+
+
 class Explorer:
     def __init__(
         self,
-        dataset: IDataset,
+        *datasets: Sequence[Dataset],
         topk: int = 10,
     ) -> None:
         """
         Explorer for Datumaro dataitems
 
         Parameters
         ----------
         dataset:
             Datumaro dataset to explore similar dataitem.
         topk:
             Number of images.
         """
-        self._model = ExplorerLauncher(model_name="clip_visual_ViT-B_32")
-        self._text_model = ExplorerLauncher(model_name="clip_text_ViT-B_32")
-        inference = dataset.run_model(self._model, append_annotation=True)
+        self._model = None
+        self._text_model = None
         self._topk = topk
-
         database_keys = []
         item_list = []
 
-        for item in inference:
-            for annotation in item.annotations:
-                if isinstance(annotation, HashKey):
-                    try:
-                        hash_key = annotation.hash_key[0]
-                        hash_key = np.unpackbits(hash_key, axis=-1)
-                        database_keys.append(hash_key)
-                        item_list.append(item)
-                    except Exception:
-                        hash_key = None
+        datasets_to_infer = [select_uninferenced_dataset(dataset) for dataset in datasets]
+        datasets = self.compute_hash_key(datasets, datasets_to_infer)
+
+        for dataset in datasets:
+            for item in dataset:
+                for annotation in item.annotations:
+                    if isinstance(annotation, HashKey):
+                        try:
+                            hash_key = annotation.hash_key[0]
+                            hash_key = np.unpackbits(hash_key, axis=-1)
+                            database_keys.append(hash_key)
+                            item_list.append(item)
+                        except Exception:
+                            continue
 
         self._database_keys = database_keys
         self._item_list = item_list
 
+    @property
+    def model(self):
+        if self._model is None:
+            self._model = ExplorerLauncher(model_name="clip_visual_ViT-B_32")
+        return self._model
+
+    @property
+    def text_model(self):
+        if self._text_model is None:
+            self._text_model = ExplorerLauncher(model_name="clip_text_ViT-B_32")
+        return self._text_model
+
+    def compute_hash_key(self, datasets, datasets_to_infer):
+        for dataset in datasets_to_infer:
+            if len(dataset) > 0:
+                dataset.run_model(self.model, append_annotation=True)
+        for dataset, dataset_to_infer in zip(datasets, datasets_to_infer):
+            dataset.update(dataset_to_infer)
+        return datasets
+
     def explore_topk(
         self,
         query: Union[DatasetItem, str, List[DatasetItem], List[str]],
         topk: Optional[int] = None,
     ):
         """
         Explore topk similar results based on hamming distance for query DatasetItem
@@ -87,15 +117,15 @@
                     q_hash_key = np.zeros((1, 64))
                     for annotation in q.annotations:
                         if isinstance(annotation, HashKey):
                             q_hash_key = annotation.hash_key
                             break
                     query_hash_key_list.append(q_hash_key)
                 elif isinstance(q, str):
-                    q_hash_key = self._text_model.launch(q)[0][0].hash_key
+                    q_hash_key = self.text_model.launch(q)[0][0].hash_key
                     query_hash_key_list.append(q_hash_key)
 
             sims = np.zeros(shape=database_keys.shape[0] * len(query_hash_key_list))
             for i, query_hash_key in enumerate(query_hash_key_list):
                 query_hash_key = np.unpackbits(query_hash_key[0], axis=-1)
                 sims[i * db_len : (i + 1) * db_len] = calculate_hamming(
                     query_hash_key, database_keys
@@ -127,15 +157,15 @@
                         )
                     query_key = self._model.launch(query.media.data)[0][0].hash_key
                 except Exception:
                     # media.data is None case
                     pass
 
         elif isinstance(query, str):
-            query_key = self._text_model.launch(query)[0][0].hash_key
+            query_key = self.text_model.launch(query)[0][0].hash_key
         else:
             raise MediaTypeError(
                 "Unexpected media type of query '%s'. "
                 "Expected 'DatasetItem' or 'string', actual'%s'" % (query, type(query))
             )
 
         if not query_key.any():
```

### Comparing `datumaro-1.2.1/datumaro/components/exporter.py` & `datumaro-1.3.0rc1/datumaro/components/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     AnnotationExportError,
     DatasetExportError,
     DatumaroError,
     ItemExportError,
 )
 from datumaro.components.media import Image, PointCloud
 from datumaro.components.progress_reporting import NullProgressReporter, ProgressReporter
-from datumaro.util.meta_file_util import save_meta_file
+from datumaro.util.meta_file_util import save_hashkey_file, save_meta_file
 from datumaro.util.os_util import rmtree
 from datumaro.util.scope import on_error_do, scoped
 
 T = TypeVar("T")
 
 
 class _ExportFail(DatumaroError):
@@ -170,14 +170,15 @@
         save_dir: str,
         *,
         save_images=None,  # Deprecated
         save_media: Optional[bool] = None,
         image_ext: Optional[str] = None,
         default_image_ext: Optional[str] = None,
         save_dataset_meta: bool = False,
+        save_hashkey_meta: bool = False,
         ctx: Optional[ExportContext] = None,
     ):
         default_image_ext = default_image_ext or self.DEFAULT_IMAGE_EXT
         assert default_image_ext
         self._default_image_ext = default_image_ext
 
         if save_images is not None and save_media is not None:
@@ -198,14 +199,15 @@
 
         self._image_ext = image_ext
 
         self._extractor = extractor
         self._save_dir = save_dir
 
         self._save_dataset_meta = save_dataset_meta
+        self._save_hashkey_meta = save_hashkey_meta
 
         # TODO: refactor this variable.
         # Can be used by a subclass to store the current patch info
         from datumaro.components.dataset import DatasetPatch
 
         if isinstance(extractor, DatasetPatch.DatasetPatchWrapper):
             self._patch = extractor.patch
@@ -274,17 +276,22 @@
 
         os.makedirs(osp.dirname(path), exist_ok=True)
         item.media.save(path, crypter=NULL_CRYPTER)
 
     def _save_meta_file(self, path):
         save_meta_file(path, self._extractor.categories())
 
+    def _save_hashkey_file(self, path):
+        save_hashkey_file(path, self._extractor)
+
 
 # TODO: Currently, ExportContextComponent is introduced only for Datumaro and DatumaroBinary format
 # for multi-processing. We need to propagate this to everywhere in Datumaro 1.2.0
+
+
 class ExportContextComponent:
     def __init__(
         self,
         save_dir: str,
         save_media: bool,
         images_dir: str,
         pcd_dir: str,
```

### Comparing `datumaro-1.2.1/datumaro/components/extractor_tfds.py` & `datumaro-1.3.0rc1/datumaro/components/extractor_tfds.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/filter.py` & `datumaro-1.3.0rc1/datumaro/components/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/format_detection.py` & `datumaro-1.3.0rc1/datumaro/components/format_detection.py`

 * *Files 1% similar despite different names*

```diff
@@ -261,14 +261,28 @@
         order.
         """
 
         self._start_requirement("require_files")
 
         return sorted(self._require_files_iter(pattern, exclude_fnames=exclude_fnames))
 
+    def require_files_iter(
+        self,
+        pattern: str,
+        *,
+        exclude_fnames: Union[str, Collection[str]] = (),
+    ) -> Iterator[str]:
+        """
+        Same as `require_files`, but returns a generator.
+        """
+
+        self._start_requirement("require_files_iter")
+
+        return self._require_files_iter(pattern, exclude_fnames=exclude_fnames)
+
     def _require_files_iter(
         self,
         pattern: str,
         *,
         exclude_fnames: Union[str, Collection[str]] = (),
     ) -> Iterator[str]:
         if isinstance(exclude_fnames, str):
```

### Comparing `datumaro-1.2.1/datumaro/components/generator.py` & `datumaro-1.3.0rc1/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/hl_ops/__init__.py` & `datumaro-1.3.0rc1/datumaro/components/hl_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/importer.py` & `datumaro-1.3.0rc1/datumaro/components/importer.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,19 +109,19 @@
 
     @classmethod
     def find_sources_with_params(cls, path: str, **extra_params) -> List[Dict]:
         return cls.find_sources(path)
 
     def __call__(self, path, **extra_params):
         if not path or not osp.exists(path):
-            raise DatasetNotFoundError(path)
+            raise DatasetNotFoundError(path, self.NAME)
 
         found_sources = self.find_sources_with_params(osp.normpath(path), **extra_params)
         if not found_sources:
-            raise DatasetNotFoundError(path)
+            raise DatasetNotFoundError(path, self.NAME)
 
         sources = []
         for desc in found_sources:
             params = dict(extra_params)
             params.update(desc.get("options", {}))
             desc["options"] = params
             sources.append(desc)
```

### Comparing `datumaro-1.2.1/datumaro/components/launcher.py` & `datumaro-1.3.0rc1/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/media.py` & `datumaro-1.3.0rc1/datumaro/components/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/media_manager.py` & `datumaro-1.3.0rc1/datumaro/components/media_manager.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/merge/__init__.py` & `datumaro-1.3.0rc1/datumaro/components/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/merge/base.py` & `datumaro-1.3.0rc1/datumaro/components/merge/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/merge/exact_merge.py` & `datumaro-1.3.0rc1/datumaro/components/merge/exact_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/merge/intersect_merge.py` & `datumaro-1.3.0rc1/datumaro/components/merge/intersect_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/merge/union_merge.py` & `datumaro-1.3.0rc1/datumaro/components/merge/union_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/operations.py` & `datumaro-1.3.0rc1/datumaro/components/operations.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/progress_reporting.py` & `datumaro-1.3.0rc1/datumaro/components/progress_reporting.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/project.py` & `datumaro-1.3.0rc1/datumaro/components/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,14 +284,15 @@
 class BuildStageType(Enum):
     source = auto()
     project = auto()
     transform = auto()
     filter = auto()
     convert = auto()
     inference = auto()
+    explore = auto()
 
 
 class Pipeline:
     @staticmethod
     def _create_graph(config: PipelineConfig):
         graph = nx.DiGraph()
         for entry in config:
@@ -911,14 +912,26 @@
                 "type": BuildStageType.convert.name,
                 "kind": format,
                 "params": params or {},
             },
             name=name,
         )
 
+    def add_explore_stage(
+        self, target: str, params: Optional[Dict] = None, name: Optional[str] = None
+    ):
+        return self.add_stage(
+            target,
+            {
+                "type": BuildStageType.explore.name,
+                "params": params or {},
+            },
+            name=name,
+        )
+
     @staticmethod
     def make_target_name(target: str, stage: Optional[str] = None) -> str:
         if stage:
             return "%s.%s" % (target, stage)
         return target
 
     @classmethod
```

### Comparing `datumaro-1.2.1/datumaro/components/shift_analyzer.py` & `datumaro-1.3.0rc1/datumaro/components/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/transformer.py` & `datumaro-1.3.0rc1/datumaro/components/transformer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/components/validator.py` & `datumaro-1.3.0rc1/datumaro/components/validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Dict, List
 
 from datumaro.components.cli_plugin import CliPlugin
 from datumaro.components.dataset import IDataset
 
 
 class Severity(Enum):
+    info = auto()
     warning = auto()
     error = auto()
 
 
 class TaskType(Enum):
     classification = auto()
     detection = auto()
@@ -47,14 +48,15 @@
         # generate validation reports and summary
         reports = self.generate_reports(stats)
         reports = list(map(lambda r: r.to_dict(), reports))
 
         summary = {
             "errors": sum(map(lambda r: r["severity"] == "error", reports)),
             "warnings": sum(map(lambda r: r["severity"] == "warning", reports)),
+            "infos": sum(map(lambda r: r["severity"] == "info", reports)),
         }
 
         validation_results["validation_reports"] = reports
         validation_results["summary"] = summary
 
         return validation_results
```

### Comparing `datumaro-1.2.1/datumaro/components/visualizer.py` & `datumaro-1.3.0rc1/datumaro/components/visualizer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-1.3.0rc1/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-# Copyright (C) 2020-2021 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import glob
 import logging as log
 import os
 import os.path as osp
 import re
+from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, CompiledMask, LabelCategories, Mask
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
+from datumaro.components.errors import InvalidAnnotationError
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.image import IMAGE_EXTENSIONS, find_images, lazy_image, load_image
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 
 class Ade20k2017Path:
     MASK_PATTERN = re.compile(
@@ -25,24 +28,24 @@
         | .+_parts_\d+
     """,
         re.VERBOSE,
     )
 
 
 class Ade20k2017Base(DatasetBase):
-    def __init__(self, path):
+    def __init__(self, path: str, *, ctx: Optional[ImportContext] = None):
         if not osp.isdir(path):
-            raise FileNotFoundError("Can't read dataset directory '%s'" % path)
+            raise NotADirectoryError(errno.ENOTDIR, "Can't find dataset directory", path)
 
         # exclude dataset meta file
         subsets = [subset for subset in os.listdir(path) if osp.splitext(subset)[-1] != ".json"]
         if len(subsets) < 1:
-            raise FileNotFoundError("Can't read subsets in directory '%s'" % path)
+            raise FileNotFoundError(errno.ENOENT, "Can't find subsets in directory", path)
 
-        super().__init__(subsets=sorted(subsets))
+        super().__init__(subsets=sorted(subsets), ctx=ctx)
         self._path = path
 
         self._items = []
         self._categories = {}
 
         if has_meta_file(self._path):
             self._categories = {
@@ -123,24 +126,26 @@
                     annotations=item_annotations,
                 )
             )
 
     def _load_item_info(self, path):
         attr_path = osp.splitext(path)[0] + "_atr.txt"
         if not osp.isfile(attr_path):
-            raise Exception("Can't find annotation file for image %s" % path)
+            raise FileNotFoundError(
+                errno.ENOENT, "Can't find annotation file for image %s" % path, attr_path
+            )
 
         item_info = []
         with open(attr_path, "r", encoding="utf-8") as f:
             for line in f:
                 columns = [s.strip() for s in line.split("#")]
                 if len(columns) != 6:
-                    raise Exception("Invalid line in %s" % attr_path)
+                    raise InvalidAnnotationError("Invalid line in %s" % attr_path)
                 if columns[5][0] != '"' or columns[5][-1] != '"':
-                    raise Exception(
+                    raise InvalidAnnotationError(
                         "Attributes column are expected \
                         in double quotes, file %s"
                         % attr_path
                     )
                 attributes = [s.strip() for s in columns[5][1:-1].split(",") if s]
 
                 item_info.append(
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-# Copyright (C) 2020-2022 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import glob
 import logging as log
 import os
 import os.path as osp
 import re
+from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import (
     AnnotationType,
     CompiledMask,
     LabelCategories,
     Mask,
     Polygon,
 )
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import parse_json
 from datumaro.util.image import IMAGE_EXTENSIONS, find_images, lazy_image, load_image
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 
 class Ade20k2020Path:
@@ -33,24 +35,24 @@
         | instance_.+
     """,
         re.VERBOSE,
     )
 
 
 class Ade20k2020Base(DatasetBase):
-    def __init__(self, path):
+    def __init__(self, path: str, *, ctx: Optional[ImportContext] = None):
         if not osp.isdir(path):
-            raise FileNotFoundError("Can't read dataset directory '%s'" % path)
+            raise NotADirectoryError(errno.ENOTDIR, "Can't find dataset directory", path)
 
         # exclude dataset meta file
         subsets = [subset for subset in os.listdir(path) if osp.splitext(subset)[-1] != ".json"]
         if len(subsets) < 1:
-            raise FileNotFoundError("Can't read subsets in directory '%s'" % path)
+            raise FileNotFoundError(errno.ENOENT, "Can't find subsets in directory", path)
 
-        super().__init__(subsets=sorted(subsets))
+        super().__init__(subsets=sorted(subsets), ctx=ctx)
         self._path = path
 
         self._items = []
         self._categories = {}
 
         if has_meta_file(self._path):
             self._categories = {
@@ -163,18 +165,16 @@
                 )
             )
 
     def _load_item_info(self, path):
         json_path = osp.splitext(path)[0] + ".json"
         item_info = []
         if not osp.isfile(json_path):
-            raise Exception(
-                "Can't find annotation file (*.json) \
-                for image %s"
-                % path
+            raise FileNotFoundError(
+                errno.ENOENT, "Can't find annotation file for image %s" % path, json_path
             )
 
         with open(json_path, "r", encoding="latin-1") as f:
             item_objects = parse_json(f.read())["annotation"]["object"]
             for obj in item_objects:
                 polygon_points = []
                 for x, y in zip(obj["polygon"]["x"], obj["polygon"]["y"]):
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/arrow_dataset.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/arrow_dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 import struct
+from typing import List, Optional
 
 import pyarrow as pa
 
 from datumaro.components.dataset_base import SubsetBase
 from datumaro.components.errors import MediaTypeError
+from datumaro.components.importer import ImportContext
 from datumaro.components.media import MediaType
 from datumaro.components.merge import get_merger
 from datumaro.plugins.data_formats.datumaro.base import DatumaroBase
 from datumaro.plugins.data_formats.datumaro_binary.mapper.common import DictMapper
 
 from .arrow_dataset import ArrowDataset
 from .mapper.dataset_item import DatasetItemMapper
 
 
 class ArrowBase(SubsetBase):
-    def __init__(self, path, ctx, subset, additional_paths=[]):
+    def __init__(
+        self,
+        path: str,
+        additional_paths: Optional[List[str]] = None,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         super().__init__(subset=subset, ctx=ctx)
 
-        self._paths = [path] + additional_paths
+        self._paths = [path]
+        if additional_paths:
+            self._paths += additional_paths
 
         self._load()
 
     def _load(self):
         infos = []
         categories = []
         media_types = set()
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/media.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/arrow/mapper/utils.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/arrow/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/ava/ava.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import csv
+import errno
 import os
 import os.path as osp
+from typing import Optional
 
 import google.protobuf.text_format as text_format
 
 from datumaro.components.annotation import AnnotationType, Bbox, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
-from datumaro.components.errors import DatasetImportError, MediaTypeError
+from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.os_util import find_files
 
 from . import ava_label_pb2
 
 
 class AvaPath:
@@ -28,40 +30,49 @@
     ANNOTATION_PREFIX = "ava_"
     ANNOTATION_VERSION = "_v2.2"
     LABEL_LIST = ANNOTATION_PREFIX + "action_list" + ANNOTATION_VERSION + ".pbtxt"
     PROPOSAL_EXT = ".pkl"
 
 
 class AvaBase(SubsetBase):
-    def __init__(self, path):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isfile(path):
-            raise DatasetImportError(f"Can't find CSV file at '{path}'")
+            raise FileNotFoundError(errno.ENOENT, "Can't find CSV file", path)
         self._path = path
 
-        subset = (
-            osp.splitext(osp.basename(path))[0]
-            .replace(AvaPath.ANNOTATION_PREFIX, "")
-            .replace(AvaPath.ANNOTATION_VERSION, "")
-        )
-        super().__init__(subset=subset)
+        if not subset:
+            subset = (
+                osp.splitext(osp.basename(path))[0]
+                .replace(AvaPath.ANNOTATION_PREFIX, "")
+                .replace(AvaPath.ANNOTATION_VERSION, "")
+            )
+        super().__init__(subset=subset, ctx=ctx)
 
         if path.endswith(osp.join(AvaPath.ANNOTATION_DIR, osp.basename(path))):
             self._rootpath = path.rsplit(AvaPath.ANNOTATION_DIR, maxsplit=1)[0]
         else:
-            raise DatasetImportError(
+            raise FileNotFoundError(
+                errno.ENOENT,
                 f"Annotation path ({path}) should be under the directory which is named {AvaPath.ANNOTATION_DIR}. "
-                "If not, Datumaro fails to find the root path for this dataset."
+                "If not, Datumaro fails to find the root path for this dataset.",
             )
 
         if self._rootpath and osp.isdir(osp.join(self._rootpath, AvaPath.IMAGE_DIR)):
             self._images_dir = osp.join(self._rootpath, AvaPath.IMAGE_DIR)
         else:
-            raise DatasetImportError(
+            raise FileNotFoundError(
+                errno.ENOENT,
                 f"Root path ({self._rootpath}) should contain the directory which is named {AvaPath.IMAGE_DIR}. "
-                "If not, Datumaro fails to find the image directory path."
+                "If not, Datumaro fails to find the image directory path.",
             )
 
         self._infos = self._load_infos(osp.dirname(path))
 
         category_path = osp.join(self._rootpath, AvaPath.ANNOTATION_DIR, AvaPath.LABEL_LIST)
         self._categories = self._load_categories(category_path)
 
@@ -74,17 +85,18 @@
                 name = file.split(".")[0].split("_")[-1]
                 infos[name + "_proposals"] = file
 
         return infos
 
     def _load_categories(self, category_path):
         if not osp.exists(category_path):
-            raise DatasetImportError(
+            raise FileNotFoundError(
+                errno.ENOENT,
                 f"Label lists cannot be found in ({category_path}). "
-                "If not, Datumaro fails to import AVA action dataset."
+                "If not, Datumaro fails to import AVA action dataset.",
             )
 
         with open(category_path, "r") as f:
             pbtxt_data = f.read()
 
         label_list = ava_label_pb2.LabelList()
         text_format.Parse(pbtxt_data, label_list)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/brats.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/brats.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import glob
 import os.path as osp
+from typing import Optional
 
 import nibabel as nib
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, LabelCategories, Mask
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import MultiframeImage
 
 
 class BratsPath:
     IMAGES_DIR = "images"
     LABELS = "labels"
     DATA_EXT = ".nii.gz"
 
 
 class BratsBase(SubsetBase):
-    def __init__(self, path):
+    def __init__(self, path: str, *, ctx: Optional[ImportContext] = None):
         if not osp.isdir(path):
-            raise FileNotFoundError("Can't read dataset directory '%s'" % path)
+            raise NotADirectoryError(errno.ENOTDIR, "Can't find dataset directory", path)
 
         self._subset_suffix = osp.basename(path)[len(BratsPath.IMAGES_DIR) :]
         subset = None
         if self._subset_suffix == "Tr":
             subset = "train"
         elif self._subset_suffix == "Ts":
             subset = "test"
-        super().__init__(subset=subset, media_type=MultiframeImage)
+        super().__init__(subset=subset, media_type=MultiframeImage, ctx=ctx)
 
         self._root_dir = osp.dirname(path)
         self._categories = self._load_categories()
         self._items = list(self._load_items(path).values())
 
     def _load_categories(self):
         label_cat = LabelCategories()
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,45 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import os.path as osp
+from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, Cuboid3d, LabelCategories, Mask
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import MultiframeImage
 from datumaro.util.pickle_util import PickleLoader
 
 
 class BratsNumpyPath:
     IDS_FILE = "val_ids.p"
     BOXES_FILE = "val_brain_bbox.p"
     LABELS_FILE = "labels"
     DATA_SUFFIX = "_data_cropped"
     LABEL_SUFFIX = "_label_cropped"
 
 
 class BratsNumpyBase(SubsetBase):
-    def __init__(self, path):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isfile(path):
-            raise FileNotFoundError("Can't read annotation file '%s'" % path)
+            raise FileNotFoundError(errno.ENOENT, "Can't find annotations file", path)
 
-        super().__init__(media_type=MultiframeImage)
+        super().__init__(subset=subset, media_type=MultiframeImage, ctx=ctx)
 
         self._root_dir = osp.dirname(path)
         self._categories = self._load_categories()
         self._items = list(self._load_items(path).values())
 
     def _load_categories(self):
         label_cat = LabelCategories()
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/camvid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2020-2021 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import glob
 import logging as log
 import os
 import os.path as osp
@@ -17,18 +17,18 @@
     CompiledMask,
     LabelCategories,
     Mask,
     MaskCategories,
 )
 from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
-from datumaro.components.errors import MediaTypeError
+from datumaro.components.errors import AnnotationExportError, InvalidAnnotationError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import find, str_to_bool
 from datumaro.util.annotation_util import make_label_id_mapping
 from datumaro.util.image import save_image
 from datumaro.util.mask_tools import generate_colormap, lazy_mask, paint_mask
 from datumaro.util.meta_file_util import has_meta_file, is_meta_file, parse_meta_file
 
@@ -96,15 +96,15 @@
                 name = label_desc[3]
                 color = tuple([int(c) for c in label_desc[:-1]])
             else:
                 name = label_desc[0]
                 color = None
 
             if name in label_map:
-                raise ValueError("Label '%s' is already defined" % name)
+                raise InvalidAnnotationError("Label '%s' is already defined" % name)
 
             label_map[name] = color
     return label_map
 
 
 def write_label_map(path, label_map):
     with open(path, "w", encoding="utf-8") as f:
@@ -156,33 +156,42 @@
     line = line.strip()
     objects = line.split('"')
     if 1 < len(objects):
         if len(objects) == 5:
             objects[0] = objects[1]
             objects[1] = objects[3]
         else:
-            raise Exception("Line %s: unexpected number " "of quotes in filename" % line)
+            raise InvalidAnnotationError(
+                "Line %s: unexpected number " "of quotes in filename" % line
+            )
     else:
         objects = line.split()
 
     if len(objects) > 1:
         return objects[0], objects[1].lstrip("/")
     else:
         return objects[0], None
 
 
 class CamvidBase(SubsetBase):
-    def __init__(self, path, subset=None):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         assert osp.isfile(path), path
         self._path = path
         self._dataset_dir = osp.dirname(path)
 
         if not subset:
             subset = osp.splitext(osp.basename(path))[0]
-        super().__init__(subset=subset)
+
+        super().__init__(subset=subset, ctx=ctx)
 
         self._categories = self._load_categories(self._dataset_dir)
         self._items = list(self._load_items(path).values())
 
     def _load_categories(self, path):
         label_map = None
         if has_meta_file(path):
@@ -411,15 +420,15 @@
         elif isinstance(label_map_source, str) and osp.isfile(label_map_source):
             if is_meta_file(label_map_source):
                 label_map = parse_meta_file(label_map_source)
             else:
                 label_map = parse_label_map(label_map_source)
 
         else:
-            raise Exception(
+            raise AnnotationExportError(
                 "Wrong labelmap specified, "
                 "expected one of %s or a file path" % ", ".join(t.name for t in LabelmapType)
             )
 
         self._categories = make_camvid_categories(label_map)
         self._label_map = label_map
         self._label_id_mapping = self._make_label_id_map()
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
+import os
 import os.path as osp
+from typing import Optional
 
 from datumaro.components.annotation import (
     AnnotationType,
     Label,
     LabelCategories,
     Points,
     PointsCategories,
 )
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
-from datumaro.components.errors import DatasetImportError
+from datumaro.components.errors import DatasetImportError, InvalidAnnotationError
+from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image
 from datumaro.util.image import find_images
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 from .celeba import CelebaImporter, CelebaPath
 
 
@@ -26,19 +30,25 @@
     LANDMARKS_HEADER = (
         "lefteye_x lefteye_y righteye_x righteye_y "
         "nose_x nose_y leftmouth_x leftmouth_y rightmouth_x rightmouth_y"
     )
 
 
 class AlignCelebaBase(SubsetBase):
-    def __init__(self, path):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isdir(path):
-            raise FileNotFoundError("Can't read dataset directory '%s'" % path)
+            raise NotADirectoryError(errno.ENOTDIR, "Can't find dataset directory", path)
 
-        super().__init__()
+        super().__init__(subset=subset, ctx=ctx)
         self._anno_dir = osp.dirname(path)
 
         self._categories = {AnnotationType.label: LabelCategories()}
         if has_meta_file(path):
             self._categories = {
                 AnnotationType.label: LabelCategories.from_iterable(parse_meta_file(path).keys())
             }
@@ -58,15 +68,15 @@
         else:
             images = {}
 
         label_categories = self._categories[AnnotationType.label]
 
         labels_path = osp.join(root_dir, AlignCelebaPath.LABELS_FILE)
         if not osp.isfile(labels_path):
-            raise DatasetImportError("File '%s': was not found" % labels_path)
+            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), labels_path)
 
         with open(labels_path, encoding="utf-8") as f:
             for line in f:
                 item_id, item_ann = self.split_annotation(line)
                 label_ids = [int(id) for id in item_ann]
                 anno = []
                 for label in label_ids:
@@ -92,32 +102,32 @@
 
                 counter = 0
                 for counter, line in enumerate(f):
                     item_id, item_ann = self.split_annotation(line)
                     landmarks = [float(id) for id in item_ann]
 
                     if len(landmarks) != len(point_cat):
-                        raise DatasetImportError(
+                        raise InvalidAnnotationError(
                             "File '%s', line %s: "
                             "points do not match the header of this file" % (landmark_path, line)
                         )
 
                     if item_id not in items:
-                        raise DatasetImportError(
+                        raise InvalidAnnotationError(
                             "File '%s', line %s: "
                             "for this item are not label in %s "
                             % (landmark_path, line, AlignCelebaPath.LABELS_FILE)
                         )
 
                     anno = items[item_id].annotations
                     label = anno[0].label
                     anno.append(Points(landmarks, label=label))
 
                 if landmarks_number - 1 != counter:
-                    raise DatasetImportError(
+                    raise InvalidAnnotationError(
                         "File '%s': the number of "
                         "landmarks does not match the specified number "
                         "at the beginning of the file " % landmark_path
                     )
 
         attr_path = osp.join(root_dir, AlignCelebaPath.ATTRS_FILE)
         if osp.isfile(attr_path):
@@ -179,15 +189,15 @@
     def split_annotation(self, line):
         item = line.split('"')
         if 1 < len(item):
             if len(item) == 3:
                 item_id = osp.splitext(item[1])[0]
                 item = item[2].split()
             else:
-                raise DatasetImportError(
+                raise InvalidAnnotationError(
                     "Line %s: unexpected number " "of quotes in filename" % line
                 )
         else:
             item = line.split()
             item_id = osp.splitext(item[0])[0]
         return item_id, item[1:]
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
+import os
 import os.path as osp
+from typing import Optional
 
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
     Label,
     LabelCategories,
     Points,
     PointsCategories,
 )
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
-from datumaro.components.errors import DatasetImportError
+from datumaro.components.errors import DatasetImportError, InvalidAnnotationError
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.image import find_images
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 
 class CelebaPath:
     IMAGES_DIR = osp.join("Img", "img_celeba")
@@ -29,19 +32,25 @@
     LANDMARKS_FILE = osp.join("Anno", "list_landmarks_celeba.txt")
     SUBSETS_FILE = osp.join("Eval", "list_eval_partition.txt")
     SUBSETS = {"0": "train", "1": "val", "2": "test"}
     BBOXES_HEADER = "image_id x_1 y_1 width height"
 
 
 class CelebaBase(SubsetBase):
-    def __init__(self, path):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isdir(path):
-            raise FileNotFoundError("Can't read dataset directory '%s'" % path)
+            raise NotADirectoryError(errno.ENOTDIR, "Can't find dataset directory", path)
 
-        super().__init__()
+        super().__init__(subset=subset, ctx=ctx)
 
         self._categories = {AnnotationType.label: LabelCategories()}
         if has_meta_file(path):
             self._categories = {
                 AnnotationType.label: LabelCategories.from_iterable(parse_meta_file(path).keys())
             }
 
@@ -60,15 +69,15 @@
         else:
             images = {}
 
         label_categories = self._categories[AnnotationType.label]
 
         labels_path = osp.join(root_dir, CelebaPath.LABELS_FILE)
         if not osp.isfile(labels_path):
-            raise DatasetImportError("File '%s': was not found" % labels_path)
+            raise FileNotFoundError(errno.ENOENT, os.strerror(errno.ENOENT), labels_path)
 
         with open(labels_path, encoding="utf-8") as f:
             for line in f:
                 item_id, item_ann = self.split_annotation(line)
                 label_ids = [int(id) for id in item_ann]
                 anno = []
                 for label in label_ids:
@@ -94,67 +103,67 @@
 
                 counter = 0
                 for counter, line in enumerate(f):
                     item_id, item_ann = self.split_annotation(line)
                     landmarks = [float(id) for id in item_ann]
 
                     if len(landmarks) != len(point_cat):
-                        raise DatasetImportError(
+                        raise InvalidAnnotationError(
                             "File '%s', line %s: "
                             "points do not match the header of this file" % (landmark_path, line)
                         )
 
                     if item_id not in items:
-                        raise DatasetImportError(
+                        raise InvalidAnnotationError(
                             "File '%s', line %s: "
                             "for this item are not label in %s "
                             % (landmark_path, line, CelebaPath.LABELS_FILE)
                         )
 
                     anno = items[item_id].annotations
                     label = anno[0].label
                     anno.append(Points(landmarks, label=label))
 
                 if landmarks_number - 1 != counter:
-                    raise DatasetImportError(
+                    raise InvalidAnnotationError(
                         "File '%s': the number of "
                         "landmarks does not match the specified number "
                         "at the beginning of the file " % landmark_path
                     )
 
         bbox_path = osp.join(root_dir, CelebaPath.BBOXES_FILE)
         if osp.isfile(bbox_path):
             with open(bbox_path, encoding="utf-8") as f:
                 bboxes_number = int(f.readline().strip())
 
                 if f.readline().strip() != CelebaPath.BBOXES_HEADER:
-                    raise DatasetImportError(
+                    raise InvalidAnnotationError(
                         "File '%s': the header "
                         "does not match the expected format '%s'"
                         % (bbox_path, CelebaPath.BBOXES_HEADER)
                     )
 
                 counter = 0
                 for counter, line in enumerate(f):
                     item_id, item_ann = self.split_annotation(line)
                     bbox = [float(id) for id in item_ann]
 
                     if item_id not in items:
-                        raise DatasetImportError(
+                        raise InvalidAnnotationError(
                             "File '%s', line %s: "
                             "for this item are not label in %s "
                             % (bbox_path, line, CelebaPath.LABELS_FILE)
                         )
 
                     anno = items[item_id].annotations
                     label = anno[0].label
                     anno.append(Bbox(bbox[0], bbox[1], bbox[2], bbox[3], label=label))
 
                 if bboxes_number - 1 != counter:
-                    raise DatasetImportError(
+                    raise InvalidAnnotationError(
                         "File '%s': the number of bounding "
                         "boxes does not match the specified number "
                         "at the beginning of the file " % bbox_path
                     )
 
         attr_path = osp.join(root_dir, CelebaPath.ATTRS_FILE)
         if osp.isfile(attr_path):
@@ -217,15 +226,15 @@
     def split_annotation(self, line):
         item = line.split('"')
         if 1 < len(item):
             if len(item) == 3:
                 item_id = osp.splitext(item[1])[0]
                 item = item[2].split()
             else:
-                raise DatasetImportError(
+                raise InvalidAnnotationError(
                     "Line %s: unexpected number " "of quotes in filename" % line
                 )
         else:
             item = line.split()
             item_id = osp.splitext(item[0])[0]
         return item_id, item[1:]
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/cifar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import os
 import os.path as osp
 import pickle  # nosec import_pickle
 from collections import OrderedDict
 from typing import Any, Dict, List, Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
-from datumaro.components.errors import MediaTypeError
+from datumaro.components.errors import InvalidAnnotationError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import cast
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 from datumaro.util.pickle_util import PickleLoader
 
 
 class CifarPath:
@@ -44,22 +45,28 @@
     "truck",
 ]
 
 # Support for Python version CIFAR-10/100
 
 
 class CifarBase(SubsetBase):
-    def __init__(self, path, subset=None):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isfile(path):
-            raise FileNotFoundError("Can't read annotation file '%s'" % path)
+            raise FileNotFoundError(errno.ENOENT, "Can't find annotations file", path)
 
         if not subset:
             subset = osp.splitext(osp.basename(path))[0]
 
-        super().__init__(subset=subset)
+        super().__init__(subset=subset, ctx=ctx)
 
         self._categories = self._load_categories(osp.dirname(path))
         self._items = list(self._load_items(path).values())
 
     def _load_categories(self, path):
         if has_meta_file(path):
             return {
@@ -117,18 +124,22 @@
         if len(labels) == 0:
             labels = annotation_dict.get("fine_labels", [])
         filenames = annotation_dict.get("filenames", [])
         images_data = annotation_dict.get("data")
         size = annotation_dict.get("image_sizes")
 
         if len(labels) != len(filenames):
-            raise Exception("The sizes of the arrays 'filenames', " "'labels' don't match.")
+            raise InvalidAnnotationError(
+                "The sizes of the arrays 'filenames', " "'labels' don't match."
+            )
 
         if 0 < len(images_data) and len(images_data) != len(filenames):
-            raise Exception("The sizes of the arrays 'data', " "'filenames', 'labels' don't match.")
+            raise InvalidAnnotationError(
+                "The sizes of the arrays 'data', " "'filenames', 'labels' don't match."
+            )
 
         for i, (filename, label) in enumerate(zip(filenames, labels)):
             item_id = osp.splitext(filename)[0]
             annotations = []
             if label is not None:
                 annotations.append(Label(label))
                 if (
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/cityscapes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-# Copyright (C) 2020-2021 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import glob
 import logging as log
 import os
 import os.path as osp
 from collections import OrderedDict
 from enum import Enum, auto
+from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import (
     AnnotationType,
     CompiledMask,
     LabelCategories,
     Mask,
     MaskCategories,
 )
 from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
-from datumaro.components.errors import MediaTypeError
+from datumaro.components.errors import AnnotationExportError, InvalidAnnotationError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import find
 from datumaro.util.annotation_util import make_label_id_mapping
 from datumaro.util.image import find_images, load_image, save_image
 from datumaro.util.mask_tools import generate_colormap, paint_mask
 from datumaro.util.meta_file_util import has_meta_file, is_meta_file, parse_meta_file
 
@@ -161,15 +162,15 @@
                 name = label_desc[3]
                 color = tuple([int(c) for c in label_desc[:-1]])
             else:
                 name = label_desc[0]
                 color = None
 
             if name in label_map:
-                raise ValueError("Label '%s' is already defined" % name)
+                raise InvalidAnnotationError("Label '%s' is already defined" % name)
 
             label_map[name] = color
     return label_map
 
 
 def write_label_map(path, label_map):
     with open(path, "w", encoding="utf-8") as f:
@@ -178,15 +179,21 @@
                 color_rgb = " ".join(str(c) for c in label_desc)
             else:
                 color_rgb = ""
             f.write("%s %s\n" % (color_rgb, label_name))
 
 
 class CityscapesBase(SubsetBase):
-    def __init__(self, path, subset=None):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         assert osp.isdir(path), path
 
         if not subset:
             subset = osp.basename(path)
 
         if osp.basename(osp.dirname(path)) == CityscapesPath.GT_FINE_DIR:
             self._path = osp.dirname(osp.dirname(path))
@@ -195,19 +202,18 @@
                 self._path, CityscapesPath.IMGS_FINE_DIR, CityscapesPath.ORIGINAL_IMAGE_DIR, subset
             )
         else:
             self._path = osp.dirname(osp.dirname(osp.dirname(path)))
             images_dir = path
             annotations_dir = osp.join(self._path, CityscapesPath.GT_FINE_DIR, subset)
 
-        self._subset = subset
         self._images_dir = images_dir
         self._gt_anns_dir = annotations_dir
 
-        super().__init__(subset=subset)
+        super().__init__(subset=subset, ctx=ctx)
 
         self._items = list(self._load_items().values())
 
     def _load_categories(self, path, use_train_label_map=False):
         label_map = None
         if has_meta_file(path):
             label_map = parse_meta_file(path)
@@ -471,15 +477,15 @@
         elif isinstance(label_map_source, str) and osp.isfile(label_map_source):
             if is_meta_file(label_map_source):
                 label_map = parse_meta_file(label_map_source)
             else:
                 label_map = parse_label_map(label_map_source)
 
         else:
-            raise Exception(
+            raise AnnotationExportError(
                 "Wrong labelmap specified, "
                 "expected one of %s or a file path" % ", ".join(t.name for t in LabelmapType)
             )
 
         self._categories = make_cityscapes_categories(label_map)
         self._label_map = label_map
         self._label_id_mapping = self._make_label_id_map()
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (C) 2019-2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
+import logging as log
 import os.path as osp
 from inspect import isclass
-from typing import Any, Dict, Tuple, Type, TypeVar, Union, overload
+from typing import Any, Dict, Optional, Tuple, Type, TypeVar, Union, overload
 
 import pycocotools.mask as mask_utils
 from attrs import define
 
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
@@ -26,52 +28,104 @@
 from datumaro.components.errors import (
     DatasetImportError,
     InvalidAnnotationError,
     InvalidFieldTypeError,
     MissingFieldError,
     UndeclaredLabelError,
 )
+from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image
 from datumaro.util import NOTSET, parse_json_file, take_by
 from datumaro.util.image import lazy_image, load_image
 from datumaro.util.mask_tools import bgr2index
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
-from .format import CocoPath, CocoTask
+from .format import CocoImporterType, CocoPath, CocoTask
 
 T = TypeVar("T")
 
 
+class DirPathExtracter:
+    @staticmethod
+    def find_rootpath(path: str) -> str:
+        """Find root path from annotation json file path."""
+        path = osp.abspath(path)
+        if osp.dirname(path).endswith(CocoPath.ANNOTATIONS_DIR):
+            return path.rsplit(CocoPath.ANNOTATIONS_DIR, maxsplit=1)[0]
+        raise DatasetImportError(
+            f"Annotation path ({path}) should be under the directory which is named {CocoPath.ANNOTATIONS_DIR}. "
+            "If not, Datumaro fails to find the root path for this dataset. "
+            "Please follow this instruction, https://github.com/cocodataset/cocoapi/blob/master/README.txt"
+        )
+
+    @staticmethod
+    def find_images_dir(rootpath: str, subset: str) -> str:
+        """Find images directory from the root path."""
+
+        if rootpath and osp.isdir(osp.join(rootpath, CocoPath.IMAGES_DIR)):
+            images_dir = osp.join(rootpath, CocoPath.IMAGES_DIR)
+            if osp.isdir(osp.join(images_dir, subset or DEFAULT_SUBSET_NAME)):
+                images_dir = osp.join(images_dir, subset or DEFAULT_SUBSET_NAME)
+            return images_dir
+
+        raise DatasetImportError(
+            f"We found the rootpath ({rootpath}) for this dataset. "
+            f"However, there should exist a directory for images as {osp.join(rootpath, CocoPath.IMAGES_DIR)}. "
+            "If not, Datumaro fails to find the image directory path. "
+            "Please follow this instruction, https://github.com/cocodataset/cocoapi/blob/master/README.txt"
+        )
+
+
+class RoboflowDirPathExtracter(DirPathExtracter):
+    @staticmethod
+    def find_rootpath(path: str) -> str:
+        path, _ = osp.split(path)
+        path, _ = osp.split(path)
+        return path
+
+    @staticmethod
+    def find_images_dir(rootpath: str, subset: str) -> str:
+        return osp.join(rootpath, subset)
+
+
 class _CocoBase(SubsetBase):
     """
     Parses COCO annotations written in the following format:
     https://cocodataset.org/#format-data
     """
 
     def __init__(
         self,
         path,
         task,
         *,
-        merge_instance_polygons=False,
-        subset=None,
-        keep_original_category_ids=False,
-        **kwargs,
+        merge_instance_polygons: bool = False,
+        keep_original_category_ids: bool = False,
+        coco_importer_type: CocoImporterType = CocoImporterType.default,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
     ):
         if not osp.isfile(path):
-            raise DatasetImportError(f"Can't find JSON file at '{path}'")
+            raise FileNotFoundError(errno.ENOENT, "Can't find JSON file", path)
         self._path = path
 
         if not subset:
             parts = osp.splitext(osp.basename(path))[0].split(task.name + "_", maxsplit=1)
             subset = parts[1] if len(parts) == 2 else None
-        super().__init__(subset=subset, **kwargs)
+        super().__init__(subset=subset, ctx=ctx)
+
+        if coco_importer_type == CocoImporterType.default:
+            self._rootpath = DirPathExtracter.find_rootpath(path)
+            self._images_dir = DirPathExtracter.find_images_dir(self._rootpath, subset)
+        elif coco_importer_type == CocoImporterType.roboflow:
+            self._rootpath = RoboflowDirPathExtracter.find_rootpath(path)
+            self._images_dir = RoboflowDirPathExtracter.find_images_dir(self._rootpath, subset)
+        else:
+            raise DatasetImportError(f"Not supported type: {coco_importer_type}")
 
-        self._rootpath = self._find_rootpath(path)
-        self._images_dir = self._find_images_dir(subset)
         self._task = task
 
         self._merge_instance_polygons = merge_instance_polygons
 
         json_data = parse_json_file(path)
         self._label_map = {}  # coco_id -> dm_id
         self._load_categories(
@@ -79,69 +133,55 @@
             keep_original_ids=keep_original_category_ids,
         )
 
         if self._task == CocoTask.panoptic:
             self._mask_dir = osp.splitext(path)[0]
         self._items = self._load_items(json_data)
 
-    def _find_rootpath(self, path: str) -> str:
-        """Find root path from annotation json file path."""
-        if path.endswith(osp.join(CocoPath.ANNOTATIONS_DIR, osp.basename(path))):
-            return path.rsplit(CocoPath.ANNOTATIONS_DIR, maxsplit=1)[0]
-        raise DatasetImportError(
-            f"Annotation path ({path}) should be under the directory which is named {CocoPath.ANNOTATIONS_DIR}. "
-            "If not, Datumaro fails to find the root path for this dataset. "
-            "Please follow this instruction, https://github.com/cocodataset/cocoapi/blob/master/README.txt"
-        )
-
-    def _find_images_dir(self, subset: str) -> str:
-        """Find images directory from the root path."""
-
-        rootpath = self._rootpath
-
-        if rootpath and osp.isdir(osp.join(rootpath, CocoPath.IMAGES_DIR)):
-            images_dir = osp.join(rootpath, CocoPath.IMAGES_DIR)
-            if osp.isdir(osp.join(images_dir, subset or DEFAULT_SUBSET_NAME)):
-                images_dir = osp.join(images_dir, subset or DEFAULT_SUBSET_NAME)
-            return images_dir
-
-        raise DatasetImportError(
-            f"We found the rootpath ({rootpath}) for this dataset. "
-            f"However, there should exist a directory for images as {osp.join(rootpath, CocoPath.IMAGES_DIR)}. "
-            "If not, Datumaro fails to find the image directory path. "
-            "Please follow this instruction, https://github.com/cocodataset/cocoapi/blob/master/README.txt"
-        )
-
     def __iter__(self):
         yield from self._items.values()
 
     def _load_categories(self, json_data, *, keep_original_ids):
+        self._categories = {}
+
         if has_meta_file(self._rootpath):
             labels = parse_meta_file(self._rootpath).keys()
             self._categories = {AnnotationType.label: LabelCategories.from_iterable(labels)}
             # 0 is reserved for no class
             self._label_map = {i + 1: i for i in range(len(labels))}
-            return
-
-        self._categories = {}
-
-        if self._task in [
+        elif self._task in [
             CocoTask.instances,
             CocoTask.labels,
             CocoTask.person_keypoints,
             CocoTask.stuff,
             CocoTask.panoptic,
         ]:
             self._load_label_categories(
                 self._parse_field(json_data, "categories", list),
                 keep_original_ids=keep_original_ids,
             )
 
-        if self._task == CocoTask.person_keypoints:
-            self._load_person_kp_categories(self._parse_field(json_data, "categories", list))
+            if self._task == CocoTask.person_keypoints:
+                self._load_person_kp_categories(self._parse_field(json_data, "categories", list))
+
+        # informs users if 0 is found as category id sicne 0 is reserved for no class
+        found = [
+            self._categories[AnnotationType.label][label_id].name
+            for cat_id, label_id in self._label_map.items()
+            if cat_id == 0
+            and self._categories[AnnotationType.label][label_id].name.lower() != "background"
+        ]
+        if found:
+            category_name = found[0]
+            log.warning(
+                "Category id of '0' is reserved for no class (background) but "
+                f"category named '{category_name}' with id of '0' is found in {self._path}. "
+                "Please be warned that annotations with category id of '0' would have `None` as label. "
+                "(https://openvinotoolkit.github.io/datumaro/latest/docs/explanation/formats/coco.html#import-coco-dataset)"
+            )
 
     def _load_label_categories(self, json_cat, *, keep_original_ids):
         categories = LabelCategories()
         label_map = {}
 
         cats = sorted(
             (
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/coco/importer.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,39 +3,41 @@
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import os.path as osp
 from glob import glob
 
 from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME
+from datumaro.components.errors import DatasetNotFoundError
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import Importer
 from datumaro.plugins.data_formats.coco.base import (
     CocoCaptionsBase,
     CocoImageInfoBase,
     CocoInstancesBase,
     CocoLabelsBase,
     CocoPanopticBase,
     CocoPersonKeypointsBase,
     CocoStuffBase,
 )
 
-from .format import CocoTask
+from .format import CocoImporterType, CocoTask
 
 
 class CocoImporter(Importer):
     _TASKS = {
         CocoTask.instances: CocoInstancesBase,
         CocoTask.person_keypoints: CocoPersonKeypointsBase,
         CocoTask.captions: CocoCaptionsBase,
         CocoTask.labels: CocoLabelsBase,
         CocoTask.image_info: CocoImageInfoBase,
         CocoTask.panoptic: CocoPanopticBase,
         CocoTask.stuff: CocoStuffBase,
     }
+    _IMPORTER_TYPE = CocoImporterType.default
 
     @classmethod
     def build_cmdline_parser(cls, **kwargs):
         parser = super().build_cmdline_parser(**kwargs)
         parser.add_argument(
             "--keep-original-category-ids",
             action="store_true",
@@ -62,15 +64,15 @@
                 with context.alternative():
                     context.require_file(f"annotations/{task.name}_*.json")
 
     def __call__(self, path, **extra_params):
         subsets = self.find_sources(path)
 
         if len(subsets) == 0:
-            raise Exception("Failed to find 'coco' dataset at '%s'" % path)
+            raise DatasetNotFoundError(path, self.NAME)
 
         # TODO: should be removed when proper label merging is implemented
         conflicting_types = {
             CocoTask.instances,
             CocoTask.person_keypoints,
             CocoTask.labels,
             CocoTask.panoptic,
@@ -84,29 +86,33 @@
                 "Not implemented: "
                 "Found potentially conflicting source types with labels: %s. "
                 "Only one type will be used: %s"
                 % (", ".join(t.name for t in ann_types), selected_ann_type.name)
             )
 
         sources = []
-        for ann_files in subsets.values():
+        for subset, ann_files in subsets.items():
             for ann_type, ann_file in ann_files.items():
                 if ann_type in conflicting_types:
                     if ann_type is not selected_ann_type:
                         log.warning(
                             "Not implemented: " "conflicting source '%s' is skipped." % ann_file
                         )
                         continue
                 log.info("Found a dataset at '%s'" % ann_file)
 
+                options = dict(extra_params)
+                options["coco_importer_type"] = self._IMPORTER_TYPE
+                options["subset"] = subset
+
                 sources.append(
                     {
                         "url": ann_file,
                         "format": self._TASKS[ann_type].NAME,
-                        "options": dict(extra_params),
+                        "options": options,
                     }
                 )
 
         return sources
 
     @classmethod
     def find_sources(cls, path):
@@ -176,7 +182,33 @@
     _TASK = CocoTask.panoptic
     _TASKS = {_TASK: CocoImporter._TASKS[_TASK]}
 
 
 class CocoStuffImporter(CocoImporter):
     _TASK = CocoTask.stuff
     _TASKS = {_TASK: CocoImporter._TASKS[_TASK]}
+
+
+class CocoRoboflowImporter(CocoImporter):
+    # Currently, All Roboflow exported COCO format can be handled by our Coco instances task implements.
+    _TASK = CocoTask.instances
+    _IMPORTER_TYPE = CocoImporterType.roboflow
+
+    @classmethod
+    def detect(
+        cls,
+        context: FormatDetectionContext,
+    ) -> FormatDetectionConfidence:
+        context.require_file("*/_annotations.coco.json")
+        return FormatDetectionConfidence.MEDIUM
+
+    @classmethod
+    def find_sources(cls, path):
+        subset_paths = glob(osp.join(path, "*", "_annotations.coco.json"), recursive=True)
+
+        subsets = {}
+        for subset_path in subset_paths:
+            subset_name = osp.basename(osp.dirname(subset_path))
+            osp.basename(subset_path)
+            subsets.setdefault(subset_name, {})[cls._TASK] = subset_path
+
+        return subsets
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import glob
 import os.path as osp
+from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, LabelCategories, Mask, MaskCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
-from datumaro.components.errors import DatasetImportError
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
-from datumaro.components.importer import Importer, with_subset_dirs
+from datumaro.components.importer import ImportContext, Importer, with_subset_dirs
 from datumaro.components.media import Image
 from datumaro.util.image import find_images
 from datumaro.util.mask_tools import generate_colormap, lazy_mask
 from datumaro.util.meta_file_util import DATASET_META_FILE, is_meta_file, parse_meta_file
 
 
 class CommonSemanticSegmentationPath:
@@ -44,35 +45,37 @@
     categories[AnnotationType.mask] = mask_categories
     return categories
 
 
 class CommonSemanticSegmentationBase(SubsetBase):
     def __init__(
         self,
-        path,
-        subset=None,
-        image_prefix="",
-        mask_prefix="",
+        path: str,
+        *,
+        image_prefix: str = "",
+        mask_prefix: str = "",
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
     ):
         if not osp.isdir(path):
-            raise FileNotFoundError("Can't read dataset directory '%s'" % path)
+            raise NotADirectoryError(errno.ENOTDIR, "Can't find dataset directory", path)
 
-        super().__init__(subset=subset)
+        super().__init__(subset=subset, ctx=ctx)
 
         self._image_prefix = image_prefix
         self._mask_prefix = mask_prefix
 
         meta_file = glob.glob(osp.join(path, "**", DATASET_META_FILE), recursive=True)
         if is_meta_file(meta_file[0]):
             self._root_dir = osp.dirname(meta_file[0])
 
             label_map = parse_meta_file(meta_file[0])
             self._categories = make_categories(label_map)
         else:
-            raise DatasetImportError("Dataset meta info file was not found in %s" % path)
+            raise FileNotFoundError(errno.ENOENT, "Dataset meta info file was not found", path)
 
         self._items = list(self._load_items().values())
 
     def _load_items(self):
         items = {}
 
         image_dir = osp.join(self._root_dir, CommonSemanticSegmentationPath.IMAGES_DIR)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,41 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import os.path as osp
+from typing import Optional
 
 from datumaro.components.annotation import SuperResolutionAnnotation
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.image import find_images
 
 
 class CommonSuperResolutionPath:
     HR_IMAGES_DIR = "HR"
     LR_IMAGES_DIR = "LR"
     UPSAMPLED_IMAGES_DIR = "upsampled"
 
 
 class CommonSuperResolutionBase(SubsetBase):
-    def __init__(self, path, subset=None):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isdir(path):
-            raise FileNotFoundError("Can't read dataset directory '%s'" % path)
+            raise NotADirectoryError(errno.ENOTDIR, "Can't find dataset directory", path)
 
-        super().__init__(subset=subset)
+        super().__init__(subset=subset, ctx=ctx)
 
         self._items = list(self._load_items(path).values())
 
     def _load_items(self, path):
         items = {}
 
         upsampled_image_dir = osp.join(path, CommonSuperResolutionPath.UPSAMPLED_IMAGES_DIR)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/cvat/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-# Copyright (C) 2019-2021 Intel Corporation
+# Copyright (C) 2019-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 from collections import OrderedDict
 from copy import deepcopy
+from typing import Optional
 
 from defusedxml import ElementTree
 
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
     Label,
@@ -16,15 +17,15 @@
     Points,
     Polygon,
     PolyLine,
 )
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import DatasetImportError
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 
 from .format import CvatPath
 
 
 def _find_meta_root(path: str):
     context = ElementTree.iterparse(path, events=("start", "end"))
@@ -43,26 +44,32 @@
 
     return meta_root, context
 
 
 class CvatBase(SubsetBase):
     _SUPPORTED_SHAPES = ("box", "polygon", "polyline", "points")
 
-    def __init__(self, path, subset=None):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         assert osp.isfile(path), path
         rootpath = osp.dirname(path)
         images_dir = ""
         if osp.isdir(osp.join(rootpath, CvatPath.IMAGES_DIR)):
             images_dir = osp.join(rootpath, CvatPath.IMAGES_DIR)
         self._images_dir = images_dir
         self._path = path
 
         if not subset:
             subset = osp.splitext(osp.basename(path))[0]
-        super().__init__(subset=subset)
+        super().__init__(subset=subset, ctx=ctx)
 
         items, categories = self._parse(path)
         self._items = list(self._load_items(items).values())
         self._categories = categories
 
     def _parse(self, path):
         meta_root, context = _find_meta_root(path)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,74 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
+from typing import Optional
+
+import numpy as np
 
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
     Caption,
     Cuboid3d,
     Ellipse,
+    HashKey,
     Label,
     LabelCategories,
     MaskCategories,
     Points,
     PointsCategories,
     Polygon,
     PolyLine,
     RleMask,
 )
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
-from datumaro.components.errors import DatasetImportError
+from datumaro.components.errors import DatasetImportError, MediaTypeError
+from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image, MediaElement, PointCloud
 from datumaro.util import parse_json_file
+from datumaro.util.meta_file_util import has_hashkey_file, parse_hashkey_file
 from datumaro.version import __version__
 
 from .format import DATUMARO_FORMAT_VERSION, DatumaroPath
 
 
 class DatumaroBase(SubsetBase):
     LEGACY_VERSION = "legacy"
     CURRENT_DATUMARO_FORMAT_VERSION = DATUMARO_FORMAT_VERSION
 
     # If Datumaro format version goes up, it will be
     # ALLOWED_VERSIONS = {LEGACY_VERSION, 1.0, ..., CURRENT_DATUMARO_FORMAT_VERSION}
     ALLOWED_VERSIONS = {LEGACY_VERSION, CURRENT_DATUMARO_FORMAT_VERSION}
 
-    def __init__(self, path):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         assert osp.isfile(path), path
 
         dm_version = self._get_dm_format_version(path)
 
         # when backward compatibility happen, we should implement version specific readers
         if dm_version not in self.ALLOWED_VERSIONS:
             raise DatasetImportError(
                 f"Datumaro format version of the given dataset is {dm_version}, "
                 f"but not supported by this Datumaro version: {__version__}. "
                 f"The allowed datumaro format versions are {self.ALLOWED_VERSIONS}. "
                 "Please install the latest Datumaro."
             )
 
-        self.default_reader(path=path)
+        self.default_reader(path=path, subset=subset, ctx=ctx)
 
-    def default_reader(self, path: str):
+    def default_reader(self, path, subset, ctx):
         """
         Default Datumaro reader for the latest version
         """
         rootpath = ""
         if path.endswith(osp.join(DatumaroPath.ANNOTATIONS_DIR, osp.basename(path))):
             rootpath = path.rsplit(DatumaroPath.ANNOTATIONS_DIR, maxsplit=1)[0]
         self._rootpath = rootpath
@@ -67,15 +79,18 @@
         self._images_dir = images_dir
 
         pcd_dir = ""
         if rootpath and osp.isdir(osp.join(rootpath, DatumaroPath.PCD_DIR)):
             pcd_dir = osp.join(rootpath, DatumaroPath.PCD_DIR)
         self._pcd_dir = pcd_dir
 
-        super().__init__(subset=osp.splitext(osp.basename(path))[0])
+        if not subset:
+            subset = osp.splitext(osp.basename(path))[0]
+
+        super().__init__(subset=subset, ctx=ctx)
         self._load_impl(path)
 
     def _get_dm_format_version(self, path: str):
         """
         Get Datumaro format at exporting the dataset
 
         Note that the regacy Datumaro doesn't store the version into exported dataset.
@@ -84,15 +99,16 @@
         self._parsed_anns = parse_json_file(path)
         return self._parsed_anns.get("dm_format_version", self.LEGACY_VERSION)
 
     def _load_impl(self, path: str) -> None:
         """Actual implementation of loading Datumaro format."""
         self._infos = self._load_infos(self._parsed_anns)
         self._categories = self._load_categories(self._parsed_anns)
-        self._items = self._load_items(self._parsed_anns)
+        items = self._load_items(self._parsed_anns)
+        self._items = self._load_hash_key(items)
 
     @staticmethod
     def _load_infos(parsed):
         return parsed.get("infos", {})
 
     @staticmethod
     def _load_categories(parsed):
@@ -132,14 +148,15 @@
 
             categories[AnnotationType.points] = point_categories
 
         return categories
 
     def _load_items(self, parsed):
         items = []
+
         for item_desc in parsed["items"]:
             item_id = item_desc["id"]
 
             media = None
             image_info = item_desc.get("image")
             if image_info:
                 image_filename = image_info.get("path") or item_id + DatumaroPath.IMAGE_EXT
@@ -151,15 +168,15 @@
                         image_path = old_image_path
 
                 media = Image.from_file(path=image_path, size=image_info.get("size"))
                 self._media_type = Image
 
             pcd_info = item_desc.get("point_cloud")
             if media and pcd_info:
-                raise DatasetImportError("Dataset cannot contain multiple media types")
+                raise MediaTypeError("Dataset cannot contain multiple media types")
             if pcd_info:
                 pcd_path = pcd_info.get("path")
                 point_cloud = osp.join(self._pcd_dir, self._subset, pcd_path)
 
                 related_images = None
                 ri_info = item_desc.get("related_images")
                 if ri_info:
@@ -189,14 +206,24 @@
                 attributes=item_desc.get("attr"),
             )
 
             items.append(item)
 
         return items
 
+    def _load_hash_key(self, items):
+        if not has_hashkey_file(self._rootpath):
+            return items
+
+        hashkey_dict = parse_hashkey_file(self._rootpath)
+        for item in items:
+            hash_key = hashkey_dict[item.subset + "/" + item.id]
+            item.annotations.append(HashKey(hash_key=np.asarray(hash_key, dtype=np.uint8)))
+        return items
+
     @staticmethod
     def _load_annotations(item):
         parsed = item["annotations"]
         loaded = []
 
         for ann in parsed:
             ann_id = ann.get("id")
@@ -302,11 +329,13 @@
                         id=ann_id,
                         attributes=attributes,
                         group=group,
                         z_order=z_order,
                     )
                 )
 
+            elif ann_type == AnnotationType.hash_key:
+                continue
             else:
                 raise NotImplementedError()
 
         return loaded
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from datumaro.components.annotation import (
     Annotation,
     Bbox,
     Caption,
     Cuboid3d,
     Ellipse,
+    HashKey,
     Label,
     LabelCategories,
     Mask,
     MaskCategories,
     Points,
     PointsCategories,
     Polygon,
@@ -170,14 +171,16 @@
                 converted_ann = self._convert_bbox_object(ann)
             elif isinstance(ann, Caption):
                 converted_ann = self._convert_caption_object(ann)
             elif isinstance(ann, Cuboid3d):
                 converted_ann = self._convert_cuboid_3d_object(ann)
             elif isinstance(ann, Ellipse):
                 converted_ann = self._convert_ellipse_object(ann)
+            elif isinstance(ann, HashKey):
+                continue
             else:
                 raise NotImplementedError()
             annotations.append(converted_ann)
 
     def add_infos(self, infos):
         self._data["infos"].update(infos)
 
@@ -415,23 +418,28 @@
             writer.add_infos(self._extractor.infos())
             writer.add_categories(self._extractor.categories())
 
         for item in self._extractor:
             subset = item.subset or DEFAULT_SUBSET_NAME
             writers[subset].add_item(item, pool)
 
+            self._check_hash_key_existence(item)
+
         for subset, writer in writers.items():
             if self._patch and subset in self._patch.updated_subsets and writer.is_empty():
                 if osp.isfile(writer.ann_file):
                     # Remove subsets that became empty
                     os.remove(writer.ann_file)
                 continue
 
             writer.write(pool)
 
+        if self._save_hashkey_meta:
+            self._save_hashkey_file(self._save_dir)
+
     @classmethod
     def patch(cls, dataset, patch, save_dir, **kwargs):
         for subset in patch.updated_subsets:
             conv = cls(dataset.get_subset(subset), save_dir=save_dir, **kwargs)
             conv._patch = patch
             conv.apply()
 
@@ -456,7 +464,15 @@
             )
             if osp.isfile(pcd_path):
                 os.unlink(pcd_path)
 
             related_images_path = osp.join(save_dir, cls.PATH_CLS.IMAGES_DIR, item.subset, item.id)
             if osp.isdir(related_images_path):
                 shutil.rmtree(related_images_path)
+
+    def _check_hash_key_existence(self, item):
+        if self._save_hashkey_meta:
+            return
+        for annotation in item.annotations:
+            if isinstance(annotation, HashKey):
+                self._save_hashkey_meta = True
+                return
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,42 +7,51 @@
 from io import BufferedReader
 from multiprocessing.pool import AsyncResult, Pool
 from typing import Any, Dict, List, Optional
 
 from datumaro.components.crypter import NULL_CRYPTER, Crypter
 from datumaro.components.dataset_base import DatasetItem
 from datumaro.components.errors import DatasetImportError
+from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image, MediaElement, MediaType, PointCloud
 from datumaro.plugins.data_formats.datumaro_binary.format import DatumaroBinaryPath
 from datumaro.plugins.data_formats.datumaro_binary.mapper import DictMapper
 from datumaro.plugins.data_formats.datumaro_binary.mapper.common import IntListMapper
 from datumaro.plugins.data_formats.datumaro_binary.mapper.dataset_item import DatasetItemMapper
 
 from ..datumaro.base import DatumaroBase
 
 
 class DatumaroBinaryBase(DatumaroBase):
     """"""
 
-    def __init__(self, path: str, encryption_key: Optional[bytes] = None, num_workers: int = 0):
+    def __init__(
+        self,
+        path: str,
+        *,
+        encryption_key: Optional[bytes] = None,
+        num_workers: int = 0,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         """
         Parameters
         ----------
         path
             Directory path to import DatumaroBinary format dataset
         encryption_key
             If the dataset is encrypted, it (secret key) is needed to import the dataset.
         num_workers
             The number of multi-processing workers for import. If num_workers = 0, do not use multiprocessing.
         """
         self._fp: Optional[BufferedReader] = None
         self._crypter = Crypter(encryption_key) if encryption_key is not None else NULL_CRYPTER
         self._media_encryption = False
         self._num_workers = num_workers
-        super().__init__(path)
+        super().__init__(path, subset=subset, ctx=ctx)
 
     def _get_dm_format_version(self, path: str) -> str:
         with open(path, "rb") as fp:
             self._fp = fp
             self._check_signature()
             dm_format_version = self._read_version()
         return dm_format_version
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/icdar/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,52 +1,64 @@
-# Copyright (C) 2020-2021 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import csv
+import errno
 import glob
 import logging as log
 import os.path as osp
+from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import Bbox, Caption, Mask, MaskCategories, Polygon
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
+from datumaro.components.errors import InvalidAnnotationError
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.image import IMAGE_EXTENSIONS, find_images
 from datumaro.util.mask_tools import lazy_mask
 
 from .format import IcdarPath, IcdarTask
 
 
 class _IcdarBase(SubsetBase):
-    def __init__(self, path, task, subset=None):
+    def __init__(
+        self,
+        path: str,
+        task: IcdarTask,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         self._path = path
         self._task = task
 
         if task is IcdarTask.word_recognition:
             if not osp.isfile(path):
-                raise FileNotFoundError("Can't read annotation file '%s'" % path)
+                raise FileNotFoundError(errno.ENOENT, "Can't find annotations file", path)
 
             if not subset:
                 subset = osp.basename(osp.dirname(path))
-            super().__init__(subset=subset)
+            super().__init__(subset=subset, ctx=ctx)
 
             self._dataset_dir = osp.dirname(osp.dirname(path))
 
             self._items = list(self._load_recognition_items().values())
         elif task in {IcdarTask.text_localization, IcdarTask.text_segmentation}:
             if not osp.isdir(path):
-                raise NotADirectoryError("Can't open folder with annotation files '%s'" % path)
+                raise NotADirectoryError(
+                    errno.ENOTDIR, "Can't read dataset directory with annotation files", path
+                )
 
             if not subset:
                 subset = osp.basename(path)
-            super().__init__(subset=subset)
+            super().__init__(subset=subset, ctx=ctx)
 
             self._dataset_dir = osp.dirname(path)
 
             if task is IcdarTask.text_localization:
                 self._items = list(self._load_localization_items().values())
             else:
                 self._items = list(self._load_segmentation_items().values())
@@ -114,15 +126,15 @@
                 for line in f:
                     line = line.strip()
                     objects = line.split('"')
                     if 1 < len(objects):
                         if len(objects) == 3:
                             text = objects[1]
                         else:
-                            raise Exception(
+                            raise InvalidAnnotationError(
                                 "Line %s: unexpected number " "of quotes in filename" % line
                             )
                     else:
                         text = ""
                     objects = objects[0].split()
                     if len(objects) == 1:
                         objects = objects[0].split(",")
@@ -200,15 +212,15 @@
 
                     objects = line.split()
                     if objects[0][0] == "#":
                         objects[0] = objects[0][1:]
                         objects[9] = '" "'
                         objects.pop()
                     if len(objects) != 10:
-                        raise Exception(
+                        raise InvalidAnnotationError(
                             "Line %s contains the wrong number "
                             'of arguments, e.g. \'241 73 144 1 4 0 3 1 4 "h"' % line
                         )
 
                     centers.append(objects[3] + " " + objects[4])
                     groups.append(group)
                     colors.append(tuple(int(o) for o in objects[:3]))
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import os.path as osp
 
 from datumaro.components.annotation import AnnotationType, CompiledMask
-from datumaro.components.errors import DatumaroError, MediaTypeError
+from datumaro.components.errors import DatasetExportError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.media import Image
 from datumaro.util.image import save_image
 from datumaro.util.mask_tools import generate_colormap, paint_mask
 
 from .format import IcdarPath
 
@@ -109,15 +109,17 @@
             group = anns[0].group
             for i, ann in enumerate(anns):
                 # Assign new color if it is not defined
                 color = ann.attributes.get("color", "")
                 if color:
                     color = color.split()
                     if len(color) != 3:
-                        raise DatumaroError("Item %s: mask #%s has invalid color" % (item.id, i))
+                        raise DatasetExportError(
+                            "Item %s: mask #%s has invalid color" % (item.id, i)
+                        )
 
                     color = tuple(map(int, color))
                 else:
                     color = next(color_bank)
                     while color in used_colors:
                         color = next(color_bank)
                 colormap.append(color)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/image_dir.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-# Copyright (C) 2019-2021 Intel Corporation
+# Copyright (C) 2019-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import os
 import os.path as osp
+from typing import Optional
 
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionConfidence
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.image import find_images
 
 
 class ImageDirImporter(Importer):
     """
     Reads images from a directory as a dataset.
@@ -34,16 +35,22 @@
     def find_sources(cls, path):
         if not osp.isdir(path):
             return []
         return [{"url": path, "format": ImageDirBase.NAME}]
 
 
 class ImageDirBase(SubsetBase):
-    def __init__(self, url, subset=None):
-        super().__init__(subset=subset)
+    def __init__(
+        self,
+        url: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
+        super().__init__(subset=subset, ctx=ctx)
 
         assert osp.isdir(url), url
 
         for path in find_images(url, recursive=True):
             item_id = osp.relpath(osp.splitext(path)[0], url)
             self._items.append(
                 DatasetItem(id=item_id, subset=self._subset, media=Image.from_file(path=path))
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/image_zip.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# Copyright (C) 2021 Intel Corporation
+# Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import os
 import os.path as osp
 from enum import Enum
+from typing import Optional
 from zipfile import ZIP_BZIP2, ZIP_DEFLATED, ZIP_LZMA, ZIP_STORED, ZipFile
 
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.exporter import Exporter
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import parse_str_enum_value
 from datumaro.util.image import IMAGE_EXTENSIONS, encode_image
 
 
 class Compression(Enum):
     ZIP_STORED = ZIP_STORED
@@ -25,16 +26,22 @@
 
 class ImageZipPath:
     DEFAULT_ARCHIVE_NAME = "default.zip"
     DEFAULT_COMPRESSION = Compression.ZIP_STORED
 
 
 class ImageZipBase(SubsetBase):
-    def __init__(self, url, subset=None):
-        super().__init__(subset=subset, media_type=Image)
+    def __init__(
+        self,
+        url: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
+        super().__init__(subset=subset, media_type=Image, ctx=ctx)
 
         assert url.endswith(".zip"), url
 
         with ZipFile(url, "r") as zf:
             for path in zf.filelist:
                 item_id, extension = osp.splitext(path.filename)
                 if extension.lower() not in IMAGE_EXTENSIONS:
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/imagenet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,54 @@
-# Copyright (C) 2020-2021 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import logging as log
 import os
 import os.path as osp
+from typing import Optional
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
-from datumaro.components.importer import Importer, with_subset_dirs
+from datumaro.components.importer import ImportContext, Importer, with_subset_dirs
 from datumaro.components.media import Image
 from datumaro.util.definitions import SUBSET_NAME_BLACKLIST
 from datumaro.util.image import find_images
 
 
 class ImagenetPath:
     IMAGE_DIR_NO_LABEL = "no_label"
     SEP_TOKEN = ":"
 
 
 class ImagenetBase(SubsetBase):
-    def __init__(self, path, subset=None):
-        assert osp.isdir(path), path
-        super().__init__(subset=subset)
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
+        if not osp.isdir(path):
+            raise NotADirectoryError(errno.ENOTDIR, "Can't find dataset directory", path)
+
+        super().__init__(subset=subset, ctx=ctx)
 
         self._categories = self._load_categories(path)
         self._items = list(self._load_items(path).values())
 
     def _load_categories(self, path):
         label_cat = LabelCategories()
         for dirname in sorted(os.listdir(path)):
+            if not os.path.isdir(os.path.join(path, dirname)):
+                raise NotADirectoryError(errno.ENOTDIR, os.strerror(errno.ENOTDIR), path)
             if dirname != ImagenetPath.IMAGE_DIR_NO_LABEL:
                 label_cat.add(dirname)
         return {AnnotationType.label: label_cat}
 
     def _load_items(self, path):
         items = {}
 
@@ -44,24 +56,32 @@
         # => max_depth=1, min_depth=1
         for image_path in find_images(path, recursive=True, max_depth=1, min_depth=1):
             label = osp.basename(osp.dirname(image_path))
             image_name = osp.splitext(osp.basename(image_path))[0]
 
             item_id = label + ImagenetPath.SEP_TOKEN + image_name
             item = items.get(item_id)
-            if item is None:
-                item = DatasetItem(
-                    id=item_id, subset=self._subset, media=Image.from_file(path=image_path)
-                )
-                items[item_id] = item
+            try:
+                if item is None:
+                    item = DatasetItem(
+                        id=item_id, subset=self._subset, media=Image.from_file(path=image_path)
+                    )
+                    items[item_id] = item
+            except Exception as e:
+                self._ctx.error_policy.report_item_error(e, item_id=(item_id, self._subset))
             annotations = item.annotations
 
             if label != ImagenetPath.IMAGE_DIR_NO_LABEL:
-                label = self._categories[AnnotationType.label].find(label)[0]
-                annotations.append(Label(label=label))
+                try:
+                    label = self._categories[AnnotationType.label].find(label)[0]
+                    annotations.append(Label(label=label))
+                except Exception as e:
+                    self._ctx.error_policy.report_annotation_error(
+                        e, item_id=(item_id, self._subset)
+                    )
 
         return items
 
 
 class ImagenetImporter(Importer):
     """TorchVision's ImageFolder style importer.
     For example, it imports the following directory structure.
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-# Copyright (C) 2020-2021 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import os
 import os.path as osp
 from enum import Enum, auto
 from typing import Iterable, Optional, Sequence, Tuple, Union
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.cli_plugin import CliPlugin
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
-from datumaro.components.errors import DatasetImportError, MediaTypeError
+from datumaro.components.errors import DatasetImportError, InvalidAnnotationError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 
 class ImagenetTxtPath:
     LABELS_FILE = "synsets.txt"
     IMAGE_DIR = "images"
@@ -33,39 +34,43 @@
     if 1 < len(item):
         if len(item) == 3:
             item_id = item[1]
             item = item[2].split()
             image = item_id + item[0]
             label_ids = [int(id) for id in item[1:]]
         else:
-            raise Exception("Line %s: unexpected number " "of quotes in filename" % line)
+            raise InvalidAnnotationError(
+                "Line %s: unexpected number " "of quotes in filename" % line
+            )
     else:
         item = line.split()
         item_id = osp.splitext(item[0])[0]
         image = item[0]
         label_ids = [int(id) for id in item[1:]]
 
     return item_id, image, label_ids
 
 
 class ImagenetTxtBase(SubsetBase):
     def __init__(
         self,
         path: str,
         *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
         labels: Union[Iterable[str], str] = _LabelsSource.file.name,
         labels_file: str = ImagenetTxtPath.LABELS_FILE,
         image_dir: Optional[str] = None,
-        subset: Optional[str] = None,
     ):
-        assert osp.isfile(path), path
+        if not osp.isfile(path):
+            raise FileNotFoundError(errno.ENOENT, "Can't find dataset file", path)
 
         if not subset:
             subset = osp.splitext(osp.basename(path))[0]
-        super().__init__(subset=subset)
+        super().__init__(subset=subset, ctx=ctx)
 
         root_dir = osp.dirname(path)
         if not image_dir:
             image_dir = ImagenetTxtPath.IMAGE_DIR
         self.image_dir = osp.join(root_dir, image_dir)
 
         self._generate_labels = False
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kinetics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import csv
+import errno
 import os
 import os.path as osp
+from typing import Optional
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Video
 from datumaro.plugins.data_formats.video import VIDEO_EXTENSIONS
 from datumaro.util import parse_json, parse_json_file
 from datumaro.util.os_util import find_files
 
 
 class KineticsBase(DatasetBase):
-    def __init__(self, path):
+    def __init__(self, path: str, *, ctx: Optional[ImportContext] = None):
         if not osp.isdir(path):
-            raise FileNotFoundError("Can't read dataset directory '%s'" % path)
+            raise NotADirectoryError(errno.ENOTDIR, "Can't find dataset directory", path)
         self._path = path
 
-        super().__init__(media_type=Video)
+        super().__init__(media_type=Video, ctx=ctx)
 
         self._annotation_files = {}
         for ann_file in find_files(path, ["csv", "json"]):
             filename = osp.splitext(osp.basename(ann_file))[0]
             if (filename not in self._annotation_files) or (
                 self._annotation_files.get(filename, "").endswith("json")
             ):
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,43 @@
-# Copyright (C) 2021 Intel Corporation
+# Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import glob
 import os.path as osp
+from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, Bbox, LabelCategories, Mask
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
+from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image
 from datumaro.util.image import find_images, load_image
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 from .format import KittiLabelMap, KittiPath, KittiTask, make_kitti_categories, parse_label_map
 
 
 class _KittiBase(SubsetBase):
-    def __init__(self, path, task, subset=None):
+    def __init__(
+        self,
+        path: str,
+        task: KittiTask,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         assert osp.isdir(path), path
         self._path = path
         self._task = task
 
         if not subset:
             subset = osp.splitext(osp.basename(path))[0]
-        self._subset = subset
-        super().__init__(subset=subset)
+        super().__init__(subset=subset, ctx=ctx)
 
         self._categories = self._load_categories(osp.dirname(self._path))
         self._items = list(self._load_items().values())
 
     def _load_categories(self, path):
         if self._task == KittiTask.segmentation:
             return self._load_categories_segmentation(path)
@@ -151,14 +159,14 @@
 
     @staticmethod
     def _lazy_extract_mask(mask, c):
         return lambda: mask == c
 
 
 class KittiSegmentationBase(_KittiBase):
-    def __init__(self, path):
-        super().__init__(path, task=KittiTask.segmentation)
+    def __init__(self, path, **kwargs):
+        super().__init__(path, task=KittiTask.segmentation, **kwargs)
 
 
 class KittiDetectionBase(_KittiBase):
-    def __init__(self, path):
-        super().__init__(path, task=KittiTask.detection)
+    def __init__(self, path, **kwargs):
+        super().__init__(path, task=KittiTask.detection, **kwargs)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os.path as osp
 from collections import OrderedDict
 from enum import Enum, auto
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, CompiledMask, LabelCategories
-from datumaro.components.errors import MediaTypeError
+from datumaro.components.errors import InvalidAnnotationError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.media import Image
 from datumaro.util import cast, parse_str_enum_value, str_to_bool
 from datumaro.util.annotation_util import make_label_id_mapping
 from datumaro.util.image import save_image
 from datumaro.util.mask_tools import paint_mask
 from datumaro.util.meta_file_util import is_meta_file, parse_meta_file
@@ -237,15 +237,15 @@
         elif isinstance(label_map_source, str) and osp.isfile(label_map_source):
             if is_meta_file(label_map_source):
                 label_map = parse_meta_file(label_map_source)
             else:
                 label_map = parse_label_map(label_map_source)
 
         else:
-            raise Exception(
+            raise InvalidAnnotationError(
                 "Wrong labelmap specified, "
                 "expected one of %s or a file path" % ", ".join(t.name for t in LabelmapType)
             )
 
         self._categories = make_kitti_categories(label_map)
         self._label_map = label_map
         self._label_id_mapping = self._make_label_id_map()
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import os.path as osp
 from glob import glob
 
+from datumaro.components.errors import DatasetNotFoundError
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import Importer
 
 from .format import KittiPath, KittiTask
 
 
 class KittiImporter(Importer):
@@ -20,15 +21,15 @@
         KittiTask.detection: ("kitti_detection", KittiPath.LABELS_DIR),
     }
 
     def __call__(self, path, **extra_params):
         subsets = self.find_sources(path)
 
         if len(subsets) == 0:
-            raise Exception("Failed to find 'kitti' dataset at '%s'" % path)
+            raise DatasetNotFoundError(path, self.NAME)
 
         # TODO: should be removed when proper label merging is implemented
         conflicting_types = {"kitti_segmentation", "kitti_detection"}
         ann_types = set(t for s in subsets.values() for t in s) & conflicting_types
         if 1 <= len(ann_types):
             selected_ann_type = sorted(ann_types)[0]
         if 1 < len(ann_types):
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,46 @@
-# Copyright (C) 2021 Intel Corporation
+# Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import os.path as osp
+from typing import Optional
 
 from defusedxml import ElementTree as ET
 
 from datumaro.components.annotation import AnnotationType, Cuboid3d, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
+from datumaro.components.errors import InvalidAnnotationError
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image, PointCloud
 from datumaro.util import cast
 from datumaro.util.image import find_images
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 from .format import KittiRawPath, OcclusionStates, TruncationStates
 
 
 class KittiRawBase(SubsetBase):
     # http://www.cvlibs.net/datasets/kitti/raw_data.php
     # https://s3.eu-central-1.amazonaws.com/avg-kitti/devkit_raw_data.zip
     # Check cpp header implementation for field meaning
 
-    def __init__(self, path, subset=None):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         assert osp.isfile(path), path
         self._rootdir = osp.dirname(path)
 
-        super().__init__(subset=subset, media_type=PointCloud)
+        super().__init__(subset=subset, media_type=PointCloud, ctx=ctx)
 
         items, categories = self._parse(path)
         self._items = list(self._load_items(items).values())
         self._categories = categories
 
     @classmethod
     def _parse(cls, path):
@@ -117,27 +125,27 @@
                     shape["occluded_kf"] = elem.text == "1"
                 elif shape and elem.tag == "truncation":
                     shape["truncated"] = TruncationStates(int(elem.text))
 
                 # common tags
                 elif attr is not None and elem.tag == "name":
                     if not elem.text:
-                        raise ValueError("Attribute name can't be empty")
+                        raise InvalidAnnotationError("Attribute name can't be empty")
                     attr["name"] = elem.text
                 elif attr is not None and elem.tag == "value":
                     attr["value"] = elem.text or ""
                 elif attr is not None and elem.tag == "attribute":
                     if shape:
                         shape["attributes"][attr["name"]] = attr["value"]
                     else:
                         track["attributes"][attr["name"]] = attr["value"]
                     attr = None
 
         if track is not None or shape is not None or attr is not None:
-            raise Exception("Failed to parse annotations from '%s'" % path)
+            raise InvalidAnnotationError("Failed to parse annotations from '%s'" % path)
 
         special_attrs = KittiRawPath.SPECIAL_ATTRS
         common_attrs = ["occluded"]
 
         if has_meta_file(path):
             categories = {
                 AnnotationType.label: LabelCategories.from_iterable(parse_meta_file(path).keys())
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Disable B406: import_xml_sax - the library is used for writing
 from xml.sax.saxutils import XMLGenerator  # nosec
 
 from datumaro.components.annotation import AnnotationType, LabelCategories
 from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DatasetItem
-from datumaro.components.errors import MediaTypeError
+from datumaro.components.errors import DatasetExportError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.media import PointCloud
 from datumaro.util import cast
 from datumaro.util.image import find_images
 
 from .format import KittiRawPath, OcclusionStates, PoseStates, TruncationStates
 
@@ -298,15 +298,15 @@
         tracks = {}  # track_id -> track
         name_mapping = {}  # frame_id -> name
 
         for frame_id, item in enumerate(subset):
             frame_id = self._write_item(item, frame_id)
 
             if frame_id in name_mapping:
-                raise Exception(
+                raise DatasetExportError(
                     "Item %s: frame id %s is repeated in the dataset" % (item.id, frame_id)
                 )
             name_mapping[frame_id] = item.id
 
             for ann in item.annotations:
                 if ann.type != AnnotationType.cuboid_3d:
                     continue
@@ -325,15 +325,15 @@
                 track_id = cast(ann.attributes.get("track_id"), int, None)
                 if self._reindex and track_id is None:
                     # In this format, track id is not used for anything except
                     # annotation grouping. So we only need to pick a definitely
                     # unused id. A negative one, for example.
                     track_id = -(len(tracks) + 1)
                 if track_id is None:
-                    raise Exception(
+                    raise DatasetExportError(
                         "Item %s: expected track annotations "
                         "having 'track_id' (integer) attribute. "
                         "Use --reindex to export single shapes." % item.id
                     )
 
                 track = tracks.get(track_id)
                 if not track:
@@ -346,21 +346,21 @@
                         "poses": [],
                         "finished": 1,  # keep last
                     }
                     tracks[track_id] = track
                 else:
                     if [track["w"], track["h"], track["l"]] != ann.scale:
                         # Tracks have fixed scale in the format
-                        raise Exception(
+                        raise DatasetExportError(
                             "Item %s: mismatching track shapes, "
                             "track id %s" % (item.id, track_id)
                         )
 
                     if track["objectType"] != label:
-                        raise Exception(
+                        raise DatasetExportError(
                             "Item %s: mismatching track labels, "
                             "track id %s: %s vs. %s"
                             % (item.id, track_id, track["objectType"], label)
                         )
 
                     # If there is a skip in track frames, add missing as outside
                     if frame_id != track["poses"][-1]["frame_id"] + 1:
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/labelme.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-# Copyright (C) 2020-2022 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import logging as log
 import os
 import os.path as osp
 from collections import defaultdict
 from glob import glob, iglob
+from typing import Optional
 
 import numpy as np
 from defusedxml import ElementTree
 
 from datumaro.components.annotation import AnnotationType, Bbox, LabelCategories, Mask, Polygon
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import cast, escape, unescape
 from datumaro.util.image import save_image
 from datumaro.util.mask_tools import find_mask_bbox, load_mask
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 from datumaro.util.os_util import split_path
 
@@ -40,17 +42,17 @@
         ("=", "\\="),
         ('"', '\\"'),
         (",", "\\,"),
     ]
 
 
 class LabelMeBase(DatasetBase):
-    def __init__(self, path):
+    def __init__(self, path: str, *, ctx: Optional[ImportContext] = None):
         assert osp.isdir(path), path
-        super().__init__()
+        super().__init__(ctx=ctx)
 
         self._items, self._categories, self._subsets = self._parse(path)
         self._length = len(self._items)
 
     def _parse(self, dataset_root):
         items = []
         subsets = set()
@@ -227,15 +229,15 @@
                     user = user_elem.text
                 attributes.append(("username", user))
 
                 mask_path = osp.join(
                     subset_root, LabelMePath.MASKS_DIR, segm_elem.find("mask").text
                 )
                 if not osp.isfile(mask_path):
-                    raise Exception("Can't find mask at '%s'" % mask_path)
+                    raise FileNotFoundError(errno.ENOENT, "Can't find mask", mask_path)
                 mask = load_mask(mask_path)
                 mask = np.any(mask, axis=2)
                 ann_items.append(Mask(image=mask, label=label, id=obj_id, attributes=attributes))
 
             if not deleted:
                 parsed_annotations[obj_id] = ann_items
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/lfw.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# Copyright (C) 2020-2021 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import os
 import os.path as osp
 import re
+from typing import Optional
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories, Points
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.image import find_images
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 
 class LfwPath:
     IMAGES_DIR = "images"
@@ -24,21 +26,28 @@
     PAIRS_FILE = "pairs.txt"
     PEOPLE_FILE = "people.txt"
     IMAGE_EXT = ".jpg"
     PATTERN = re.compile(r"([\w-]+)_([-\d]+)")
 
 
 class LfwBase(SubsetBase):
-    def __init__(self, path, subset=None):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isfile(path):
-            raise FileNotFoundError("Can't read annotation file '%s'" % path)
+            raise FileNotFoundError(errno.ENOENT, "Can't find annotations file", path)
 
         if not subset:
             subset = osp.basename(osp.dirname(osp.dirname(path)))
-        super().__init__(subset=subset)
+
+        super().__init__(subset=subset, ctx=ctx)
 
         self._dataset_dir = osp.dirname(osp.dirname(osp.dirname(path)))
         self._annotations_dir = osp.dirname(path)
         self._images_dir = osp.join(self._dataset_dir, self._subset, LfwPath.IMAGES_DIR)
 
         people_file = osp.join(osp.dirname(path), LfwPath.PEOPLE_FILE)
         self._categories = self._load_categories(people_file)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
-import glob
+
+import errno
 import logging as log
 import os
 import os.path as osp
+from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import (
     AnnotationType,
     CompiledMask,
     LabelCategories,
     Mask,
     MaskCategories,
     Polygon,
 )
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
+from datumaro.components.errors import DatasetImportError
+from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image
 from datumaro.util import parse_json_file
 from datumaro.util.image import find_images, lazy_image, load_image
 from datumaro.util.mask_tools import bgr2index
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 from .format import (
@@ -30,65 +34,82 @@
     make_mapillary_instance_categories,
     parse_config_file,
 )
 
 
 class _MapillaryVistasBase(SubsetBase):
     def __init__(
-        self, path, task, subset=None, use_original_config=False, keep_original_category_ids=False
+        self,
+        path: str,
+        task: MapillaryVistasTask,
+        *,
+        use_original_config: bool = False,
+        keep_original_category_ids: bool = False,
+        format_version: str = "v2.0",
+        parse_polygon: bool = False,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
     ):
+        if format_version == "v1.2" and parse_polygon is True:
+            raise DatasetImportError(
+                f"Format version {format_version} is not available for polygons. "
+                "Please try with v2.0 for parsing polygons."
+            )
+
         assert osp.isdir(path), path
         self._path = path
         if subset is None:
             subset = osp.basename(self._path)
-        super().__init__(subset=subset)
+        super().__init__(subset=subset, ctx=ctx)
 
         annotations_dirs = [d for d in os.listdir(path) if d in MapillaryVistasPath.ANNOTATION_DIRS]
 
         if len(annotations_dirs) == 0:
+            expected_dirs = ",".join(MapillaryVistasPath.ANNOTATION_DIRS[format_version])
             raise NotADirectoryError(
-                "Can't find annotation directory at %s. "
-                "Expected one of these directories: %s"
-                % (path, ",".join(MapillaryVistasPath.ANNOTATIONS_DIR_PATTERNS))
+                errno.ENOTDIR,
+                f"Can't find annotation directory at {path}. "
+                f"Expected one of these directories: {expected_dirs}.",
             )
         elif len(annotations_dirs) > 1:
+            skipped_dirs = ",".join(annotations_dirs[1:])
             log.warning(
-                "Directory(-es): %s will be skipped, dataset should contain "
-                "only one annotation directory" % ",".join(annotations_dirs[1:])
+                f"Directory(-es): {skipped_dirs} will be skipped, dataset should "
+                "contain only one annotation directory"
             )
 
         self._use_original_config = use_original_config
-        self._format_version = annotations_dirs[0]
-        self._annotations_dir = osp.join(path, annotations_dirs[0])
+        self._format_version = format_version
+        self._parse_polygon = parse_polygon
+        self._annotations_dir = osp.join(path, format_version)
         self._images_dir = osp.join(path, MapillaryVistasPath.IMAGES_DIR)
-        self._task = task
 
-        if self._task == MapillaryVistasTask.instances:
+        if task == MapillaryVistasTask.instances:
             if has_meta_file(path):
                 self._categories = make_mapillary_instance_categories(parse_meta_file(path))
             else:
                 self._categories = self._load_instances_categories()
             self._items = self._load_instances_items()
         else:
             panoptic_config = self._load_panoptic_config(self._annotations_dir)
             self._categories = self._load_panoptic_categories(
                 panoptic_config["categories"], keep_original_category_ids
             )
             self._items = self._load_panoptic_items(panoptic_config)
 
-    @staticmethod
-    def _load_panoptic_config(path):
+    def _load_panoptic_config(self, path):
         panoptic_config_path = osp.join(
-            path, MapillaryVistasPath.PANOPTIC_DIR, MapillaryVistasPath.PANOPTIC_CONFIG
+            path,
+            MapillaryVistasPath.PANOPTIC_DIR,
+            MapillaryVistasPath.PANOPTIC_CONFIG[self._format_version],
         )
 
         if not osp.isfile(panoptic_config_path):
             raise FileNotFoundError(
-                "Can't find panoptic config file: '%s' at '%s'"
-                % (MapillaryVistasPath.PANOPTIC_CONFIG, panoptic_config_path)
+                errno.ENOENT, "Can't find panoptic config file", panoptic_config_path
             )
 
         return parse_json_file(panoptic_config_path)
 
     def _load_panoptic_categories(self, categories_info, keep_original_ids):
         label_cat = LabelCategories()
         label_map, color_map = {}, {}
@@ -123,49 +144,64 @@
                 "path": osp.join(self._images_dir, img["file_name"]),
                 "height": img.get("height"),
                 "width": img.get("width"),
             }
             for img in config["images"]
         }
 
+        polygon_dir = osp.join(self._annotations_dir, MapillaryVistasPath.POLYGON_DIR)
+
         for item_ann in config["annotations"]:
             item_id = item_ann["image_id"]
             image = None
             if images_info.get(item_id):
                 image = Image.from_file(
                     path=images_info[item_id]["path"],
                     size=self._get_image_size(images_info[item_id]),
                 )
 
-            annotations = []
             mask_path = osp.join(
                 self._annotations_dir, MapillaryVistasPath.PANOPTIC_DIR, item_ann["file_name"]
             )
             mask = lazy_image(mask_path, loader=self._load_pan_mask)
             mask = CompiledMask(instance_mask=mask)
 
+            annotations = []
             for segment_info in item_ann["segments_info"]:
                 cat_id = self._get_label_id(segment_info)
                 segment_id = segment_info["id"]
                 attributes = {"is_crowd": bool(segment_info["iscrowd"])}
                 annotations.append(
                     Mask(
                         image=mask.lazy_extract(segment_id),
                         label=cat_id,
                         id=segment_id,
                         group=segment_id,
                         attributes=attributes,
                     )
                 )
 
+            if self._parse_polygon:
+                polygon_path = osp.join(polygon_dir, item_id + ".json")
+                item_info = parse_json_file(polygon_path)
+
+                polygons = item_info["objects"]
+                for polygon in polygons:
+                    label = polygon["label"]
+                    label_id = self._categories[AnnotationType.label].find(label)[0]
+                    if label_id is None:
+                        label_id = self._categories[AnnotationType.label].add(label)
+
+                    points = [int(coord) for point in polygon["polygon"] for coord in point]
+                    annotations.append(Polygon(label=label_id, points=points))
+
             items[item_id] = DatasetItem(
                 id=item_id, subset=self._subset, annotations=annotations, media=image
             )
 
-        self._load_polygons(items)
         return items.values()
 
     def _load_instances_categories(self):
         config_file = MapillaryVistasPath.CONFIG_FILES[self._format_version]
         label_map = None
 
         if self._use_original_config:
@@ -176,89 +212,69 @@
             except FileNotFoundError:
                 label_map = parse_config_file(osp.join(osp.dirname(self._path), config_file))
         return make_mapillary_instance_categories(label_map)
 
     def _load_instances_items(self):
         items = {}
 
-        instances_dir = osp.join(self._annotations_dir, MapillaryVistasPath.INSTANCES_DIR)
-        for instance_path in find_images(instances_dir, recursive=True):
-            item_id = osp.splitext(osp.relpath(instance_path, instances_dir))[0]
+        # class_dir = osp.join(self._annotations_dir, MapillaryVistasPath.CLASS_DIR)
+        # for class_path in find_images(class_dir, recursive=True):
+        #     item_id = osp.splitext(osp.relpath(class_path, class_dir))[0]
+        #     if item_id in items:
+        #         continue
+
+        #     from PIL import Image as PILImage
+
+        #     class_mask = np.array(PILImage.open(class_path))
+        #     classes = np.unique(class_mask)
+
+        #     annotations = []
+        #     for label_id in classes:
+        #         annotations.append(
+        #             Mask(label=label_id, image=self._lazy_extract_mask(class_mask, label_id))
+        #         )
+
+        #     items[item_id] = DatasetItem(id=item_id, subset=self._subset, annotations=annotations)
+
+        instance_dir = osp.join(self._annotations_dir, MapillaryVistasPath.INSTANCES_DIR)
+        polygon_dir = osp.join(self._annotations_dir, MapillaryVistasPath.POLYGON_DIR)
+        for image_path in find_images(self._images_dir, recursive=True):
+            item_id = osp.splitext(osp.relpath(image_path, self._images_dir))[0]
+            image = Image.from_file(path=image_path)
 
+            instance_path = osp.join(instance_dir, item_id + MapillaryVistasPath.MASK_EXT)
             mask = load_image(instance_path, dtype=np.uint32)
 
             annotations = []
             for uval in np.unique(mask):
                 label_id, instance_id = uval >> 8, uval & 255
                 annotations.append(
                     Mask(image=self._lazy_extract_mask(mask, uval), label=label_id, id=instance_id)
                 )
 
-            items[item_id] = DatasetItem(id=item_id, subset=self._subset, annotations=annotations)
-
-        class_dir = osp.join(self._annotations_dir, MapillaryVistasPath.CLASS_DIR)
-        for class_path in find_images(class_dir, recursive=True):
-            item_id = osp.splitext(osp.relpath(class_path, class_dir))[0]
-            if item_id in items:
-                continue
-
-            from PIL import Image as PILImage
+            if self._parse_polygon:
+                polygon_path = osp.join(polygon_dir, item_id + ".json")
+                item_info = parse_json_file(polygon_path)
+
+                polygons = item_info["objects"]
+                for polygon in polygons:
+                    label = polygon["label"]
+                    label_id = self._categories[AnnotationType.label].find(label)[0]
+                    if label_id is None:
+                        label_id = self._categories[AnnotationType.label].add(label)
 
-            class_mask = np.array(PILImage.open(class_path))
-            classes = np.unique(class_mask)
+                    points = [int(coord) for point in polygon["polygon"] for coord in point]
+                    annotations.append(Polygon(label=label_id, points=points))
 
-            annotations = []
-            for label_id in classes:
-                annotations.append(
-                    Mask(label=label_id, image=self._lazy_extract_mask(class_mask, label_id))
-                )
-
-            items[item_id] = DatasetItem(id=item_id, subset=self._subset, annotations=annotations)
-
-        for image_path in find_images(self._images_dir, recursive=True):
-            item_id = osp.splitext(osp.relpath(image_path, self._images_dir))[0]
-            image = Image.from_file(path=image_path)
-            if item_id in items:
-                items[item_id].media = image
-            else:
-                items[item_id] = DatasetItem(id=item_id, subset=self._subset, media=image)
+            items[item_id] = DatasetItem(
+                id=item_id, subset=self._subset, media=image, annotations=annotations
+            )
 
-        self._load_polygons(items)
         return items.values()
 
-    def _load_polygons(self, items):
-        polygons_dir = osp.join(self._annotations_dir, MapillaryVistasPath.POLYGON_DIR)
-        for item_path in glob.glob(osp.join(polygons_dir, "**", "*.json"), recursive=True):
-            item_id = osp.splitext(osp.relpath(item_path, polygons_dir))[0]
-            item = items.get(item_id)
-            item_info = {}
-            item_info = parse_json_file(item_path)
-
-            image_size = self._get_image_size(item_info)
-            if image_size and item.has_image:
-                item.media = item.image.from_self(size=image_size)
-
-            polygons = item_info["objects"]
-            annotations = []
-            for polygon in polygons:
-                label = polygon["label"]
-                label_id = self._categories[AnnotationType.label].find(label)[0]
-                if label_id is None:
-                    label_id = self._categories[AnnotationType.label].add(label)
-
-                points = [coord for point in polygon["polygon"] for coord in point]
-                annotations.append(Polygon(label=label_id, points=points))
-
-            if item is None:
-                items[item_id] = DatasetItem(
-                    id=item_id, subset=self._subset, annotations=annotations
-                )
-            else:
-                item.annotations.extend(annotations)
-
     @staticmethod
     def _get_image_size(image_info):
         image_size = image_info.get("height"), image_info.get("width")
         if all(image_size):
             return int(image_size[0]), int(image_size[1])
         return None
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from collections import OrderedDict
 from enum import Enum, auto
 
 from datumaro.components.annotation import AnnotationType, LabelCategories, MaskCategories
@@ -45,20 +45,20 @@
     INSTANCES_DIR = "instances"
     PANOPTIC_DIR = "panoptic"
     POLYGON_DIR = "polygons"
     CLASS_DIR = "labels"
     MASK_EXT = ".png"
 
     ANNOTATION_DIRS = {
-        "v1.2": [CLASS_DIR, INSTANCES_DIR],
+        "v1.2": [CLASS_DIR, INSTANCES_DIR, PANOPTIC_DIR],
         "v2.0": [CLASS_DIR, INSTANCES_DIR, PANOPTIC_DIR, POLYGON_DIR],
     }
 
     CONFIG_FILES = {"v1.2": "config_v1.2.json", "v2.0": "config_v2.0.json"}
-    PANOPTIC_CONFIG = "panoptic_2020.json"
+    PANOPTIC_CONFIG = {"v1.2": "panoptic_2018.json", "v2.0": "panoptic_2020.json"}
 
     CLASS_BY_DIR = {
         INSTANCES_DIR: MapillaryVistasTask.instances,
         CLASS_DIR: MapillaryVistasTask.instances,
         POLYGON_DIR: MapillaryVistasTask.instances,
         PANOPTIC_DIR: MapillaryVistasTask.panoptic,
     }
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
-# Copyright (C) 2021 Intel Corporation
+# Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 import glob
 import logging as log
 import os.path as osp
 
 from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME
+from datumaro.components.errors import DatasetNotFoundError
 from datumaro.components.importer import Importer
+from datumaro.util import str_to_bool
 
 from .base import MapillaryVistasInstancesBase, MapillaryVistasPanopticBase
 from .format import MapillaryVistasPath, MapillaryVistasTask
 
 
 class MapillaryVistasImporter(Importer):
     _TASKS = {
@@ -18,14 +20,26 @@
         MapillaryVistasTask.panoptic: MapillaryVistasPanopticBase,
     }
 
     @classmethod
     def build_cmdline_parser(cls, **kwargs):
         parser = super().build_cmdline_parser(**kwargs)
         parser.add_argument(
+            "--format-version",
+            default="v2.0",
+            type=str,
+            help="Use original config*.json file for your version of dataset",
+        )
+        parser.add_argument(
+            "--parse-polygon",
+            type=str_to_bool,
+            default=False,
+            help="Use original config*.json file for your version of dataset",
+        )
+        parser.add_argument(
             "--use-original-config",
             action="store_true",
             help="Use original config*.json file for your version of dataset",
         )
         parser.add_argument(
             "--keep-original-category-ids",
             action="store_true",
@@ -35,37 +49,39 @@
         )
         return parser
 
     def __call__(self, path, **extra_params):
         subsets = self.find_sources(path)
 
         if len(subsets) == 0:
-            raise Exception("Failed to find Mapillary Vistas dataset at '%s'" % path)
+            raise DatasetNotFoundError(path, self.NAME)
 
         tasks = list(set(task for subset in subsets.values() for task in subset))
         selected_task = tasks[0]
         if 1 < len(tasks):
+            task_types = ",".join(task.name for task in tasks)
             log.warning(
-                "Found potentially conflicting source types: %s"
-                "Only one one type will be used: %s"
-                % (",".join(task.name for task in tasks), selected_task.name)
+                f"Found potentially conflicting source types: {task_types}"
+                f"Only one one type will be used: {selected_task.name}"
             )
 
         if selected_task == MapillaryVistasTask.instances:
             has_config = any(
                 [
                     osp.isfile(osp.join(path, config))
                     for config in MapillaryVistasPath.CONFIG_FILES.values()
                 ]
             )
 
             if not has_config and not extra_params.get("use_original_config"):
-                raise Exception(
-                    "Failed to find config*.json at '%s'. "
-                    "See extra args for using original config" % path
+                raise DatasetNotFoundError(
+                    path,
+                    self.NAME,
+                    "Failed to find config*.json at '{path}'. "
+                    "See extra args for using original configs.",
                 )
 
         sources = [
             {"url": url, "format": self._TASKS[task].NAME, "options": dict(extra_params)}
             for _, subset_info in subsets.items()
             for task, url in subset_info.items()
             if task == selected_task
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/market1501.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-# Copyright (C) 2020-2022 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import os
 import os.path as osp
 import re
+from typing import Optional
 
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionConfidence
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import str_to_bool
 from datumaro.util.image import find_images
 
 
 class Market1501Path:
     QUERY_DIR = "query"
@@ -23,20 +25,20 @@
     PATTERN = re.compile(r"^(-?\d+)_c(\d+)s(\d+)_(\d+)_(\d+)(.*)")
     LIST_PREFIX = "images_"
     UNKNOWN_ID = -1
     ATTRIBUTES = ["person_id", "camera_id", "track_id", "frame_id", "bbox_id"]
 
 
 class Market1501Base(DatasetBase):
-    def __init__(self, path):
+    def __init__(self, path: str, *, ctx: Optional[ImportContext] = None):
         if not osp.isdir(path):
-            raise NotADirectoryError("Can't open folder with annotation files '%s'" % path)
+            raise NotADirectoryError(errno.ENOTDIR, "Can't find dataset directory", path)
 
         self._path = path
-        super().__init__()
+        super().__init__(ctx=ctx)
 
         subsets = {}
         for p in os.listdir(path):
             pf = osp.join(path, p)
 
             if p.startswith(Market1501Path.BBOX_DIR) and osp.isdir(pf):
                 subset = p.replace(Market1501Path.BBOX_DIR, "")
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/mars.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mars.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,37 @@
-# Copyright (C) 2020-2021 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
+
 import fnmatch
 import glob
 import logging as log
 import os
 import os.path as osp
+from typing import Optional
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.dataset import DatasetItem
 from datumaro.components.dataset_base import DatasetBase
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.image import find_images
 
 
 class MarsPath:
     SUBSET_DIR_PATTERN = "bbox_*"
     IMAGE_DIR_PATTERNS = ["[0-9]" * 4, "00-1"]
     IMAGE_NAME_POSTFIX = "C[0-9]" + "T" + "[0-9]" * 4 + "F" + "[0-9]" * 3 + ".*"
 
 
 class MarsBase(DatasetBase):
-    def __init__(self, path):
+    def __init__(self, path: str, *, ctx: Optional[ImportContext] = None):
         assert osp.isdir(path), path
-        super().__init__()
+        super().__init__(ctx=ctx)
 
         self._dataset_dir = path
         self._subsets = {
             subset_dir.split("_", maxsplit=1)[1]: osp.join(path, subset_dir)
             for subset_dir in os.listdir(path)
             if (
                 osp.isdir(osp.join(path, subset_dir))
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mnist.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,59 @@
-# Copyright (C) 2021 Intel Corporation
+# Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import gzip
 import os
 import os.path as osp
+from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 
 class MnistPath:
     TEST_LABELS_FILE = "t10k-labels-idx1-ubyte.gz"
     TEST_IMAGES_FILE = "t10k-images-idx3-ubyte.gz"
     LABELS_FILE = "-labels-idx1-ubyte.gz"
     IMAGES_FILE = "-images-idx3-ubyte.gz"
     IMAGE_SIZE = 28
     NONE_LABEL = 255
 
 
 class MnistBase(SubsetBase):
-    def __init__(self, path, subset=None):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isfile(path):
-            raise FileNotFoundError("Can't read annotation file '%s'" % path)
+            raise FileNotFoundError(errno.ENOENT, "Can't find annotations file", path)
+        self._dataset_dir = osp.dirname(path)
 
         if not subset:
             file_name = osp.splitext(osp.basename(path))[0]
             if file_name.startswith("t10k"):
                 subset = "test"
             else:
                 subset = file_name.split("-", maxsplit=1)[0]
 
-        super().__init__(subset=subset)
-        self._dataset_dir = osp.dirname(path)
+        super().__init__(subset=subset, ctx=ctx)
 
         self._categories = self._load_categories()
-
         self._items = list(self._load_items(path).values())
 
     def _load_categories(self):
         if has_meta_file(self._dataset_dir):
             return {
                 AnnotationType.label: LabelCategories.from_iterable(
                     parse_meta_file(self._dataset_dir).keys()
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,48 @@
-# Copyright (C) 2021 Intel Corporation
+# Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import os
 import os.path as osp
+from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, Label, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 
 class MnistCsvPath:
     IMAGE_SIZE = 28
     NONE_LABEL = -1
 
 
 class MnistCsvBase(SubsetBase):
-    def __init__(self, path, subset=None):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isfile(path):
-            raise FileNotFoundError("Can't read annotation file '%s'" % path)
+            raise FileNotFoundError(errno.ENOENT, "Can't find annotations file", path)
 
         if not subset:
             file_name = osp.splitext(osp.basename(path))[0]
             subset = file_name.rsplit("_", maxsplit=1)[-1]
 
-        super().__init__(subset=subset)
+        super().__init__(subset=subset, ctx=ctx)
         self._dataset_dir = osp.dirname(path)
 
         self._categories = self._load_categories()
 
         self._items = list(self._load_items(path).values())
 
     def _load_categories(self):
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/mot.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-# Copyright (C) 2020-2021 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 # The Multiple Object Tracking Benchmark challenge format support
 # Format description: https://arxiv.org/pdf/1906.04567.pdf
 # Another description: https://motchallenge.net/instructions
 
 import csv
 import logging as log
 import os
 import os.path as osp
 from collections import OrderedDict
 from enum import Enum
+from typing import List, Optional, Union
 
 from datumaro.components.annotation import AnnotationType, Bbox, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import cast
 from datumaro.util.image import find_images
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 MotLabel = Enum(
     "MotLabel",
@@ -62,16 +63,25 @@
         "confidence",  # or 'not ignored' flag for GT anns
         "class_id",
         "visibility",
     ]
 
 
 class MotSeqBase(SubsetBase):
-    def __init__(self, path, labels=None, occlusion_threshold=0, is_gt=None, subset=None):
-        super().__init__(subset=subset)
+    def __init__(
+        self,
+        path: str,
+        *,
+        labels: Optional[Union[str, List[str]]] = None,
+        occlusion_threshold: float = 0.0,
+        is_gt: Optional[bool] = None,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
+        super().__init__(subset=subset, ctx=ctx)
 
         assert osp.isfile(path)
         seq_root = osp.dirname(osp.dirname(path))
         self._image_dir = ""
         if osp.isdir(osp.join(seq_root, MotPath.IMAGE_DIR)):
             self._image_dir = osp.join(seq_root, MotPath.IMAGE_DIR)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/mots.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mots.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# Copyright (C) 2020-2021 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 # Implements MOTS format https://www.vision.rwth-aachen.de/page/mots
 
 import logging as log
 import os
 import os.path as osp
 from enum import Enum
 from glob import iglob
+from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, LabelCategories, Mask
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.image import find_images, load_image, save_image
 from datumaro.util.mask_tools import merge_masks
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 
 class MotsPath:
@@ -41,17 +42,23 @@
 class MotsPngExtractor(SubsetBase):
     @staticmethod
     def detect_dataset(path):
         if osp.isdir(osp.join(path, MotsPath.MASKS_DIR)):
             return [{"url": path, "format": MotsPngExtractor.NAME}]
         return []
 
-    def __init__(self, path, subset=None):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         assert osp.isdir(path), path
-        super().__init__(subset=subset)
+        super().__init__(subset=subset, ctx=ctx)
         self._images_dir = osp.join(path, "images")
         self._anno_dir = osp.join(path, MotsPath.MASKS_DIR)
         if has_meta_file(path):
             self._categories = {
                 AnnotationType.label: LabelCategories.from_iterable(parse_meta_file(path).keys())
             }
         else:
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,44 +1,52 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import os.path as osp
+from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
     LabelCategories,
     Points,
     PointsCategories,
 )
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import parse_json_file
 
 from .format import MPII_POINTS_JOINTS, MPII_POINTS_LABELS
 
 
 class MpiiJsonPath:
     ANNOTATION_FILE = "mpii_annotations.json"
     HEADBOXES_FILE = "mpii_headboxes.npy"
     VISIBILITY_FILE = "jnt_visible.npy"
     POS_GT_FILE = "mpii_pos_gt.npy"
 
 
 class MpiiJsonBase(SubsetBase):
-    def __init__(self, path):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isfile(path):
-            raise FileNotFoundError("Can't read annotation file '%s'" % path)
+            raise FileNotFoundError(errno.ENOENT, "Can't find annotations file", path)
 
-        super().__init__()
+        super().__init__(subset=subset, ctx=ctx)
 
         self._categories = {
             AnnotationType.label: LabelCategories.from_iterable(["human"]),
             AnnotationType.points: PointsCategories.from_iterable(
                 [(0, MPII_POINTS_LABELS, MPII_POINTS_JOINTS)]
             ),
         }
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,44 @@
-# Copyright (C) 2021 Intel Corporation
+# Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import os.path as osp
+from typing import Optional
 
 import scipy.io as spio
 
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
     LabelCategories,
     Points,
     PointsCategories,
 )
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 
 from .format import MPII_POINTS_JOINTS, MPII_POINTS_LABELS
 
 
 class MpiiBase(SubsetBase):
-    def __init__(self, path):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isfile(path):
-            raise FileNotFoundError("Can't read annotation file '%s'" % path)
+            raise FileNotFoundError(errno.ENOENT, "Can't find annotations file", path)
 
-        super().__init__()
+        super().__init__(subset=subset, ctx=ctx)
 
         self._categories = {
             AnnotationType.label: LabelCategories.from_iterable(["human"]),
             AnnotationType.points: PointsCategories.from_iterable(
                 [(0, MPII_POINTS_LABELS, MPII_POINTS_JOINTS)]
             ),
         }
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import os.path as osp
+from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, Bbox, Label, LabelCategories, Mask
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
+from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image
 from datumaro.util.image import find_images, load_image
 
 from .format import MvtecPath, MvtecTask
 
 
 class _MvtecBase(SubsetBase):
-    def __init__(self, path, task, subset=None):
+    def __init__(
+        self,
+        path: str,
+        task: MvtecTask,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         assert osp.isdir(path), path
         self._path = path
         self._task = task
 
         if not subset:
             subset = osp.splitext(osp.basename(path))[0]
-        self._subset = subset
-        super().__init__(subset=subset)
+        super().__init__(subset=subset, ctx=ctx)
 
         self._categories = self._load_categories()
         self._items = list(self._load_items().values())
 
     def _load_categories(self):
         label_path = os.listdir(self._path)
         label_cat = LabelCategories()
@@ -91,18 +99,21 @@
                 else:
                     anns.append(Label(label=label_id))
         return items
 
 
 class MvtecClassificationBase(_MvtecBase):
     def __init__(self, path, **kwargs):
-        super().__init__(path, task=MvtecTask.classification)
+        kwargs.pop("merge_policy")
+        super().__init__(path, task=MvtecTask.classification, **kwargs)
 
 
 class MvtecSegmentationBase(_MvtecBase):
     def __init__(self, path, **kwargs):
-        super().__init__(path, task=MvtecTask.segmentation)
+        kwargs.pop("merge_policy")
+        super().__init__(path, task=MvtecTask.segmentation, **kwargs)
 
 
 class MvtecDetectionBase(_MvtecBase):
     def __init__(self, path, **kwargs):
-        super().__init__(path, task=MvtecTask.detection)
+        kwargs.pop("merge_policy")
+        super().__init__(path, task=MvtecTask.detection, **kwargs)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,38 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import glob
 import os.path as osp
+from typing import Optional
 
 import h5py
 import numpy as np
 
 from datumaro.components.annotation import DepthAnnotation
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 
 
 class NyuDepthV2Base(SubsetBase):
-    def __init__(self, path, subset=None):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isdir(path):
-            raise FileNotFoundError("Can't read dataset directory '%s'" % path)
+            raise NotADirectoryError(errno.ENOTDIR, "Can't find dataset directory", path)
 
-        super().__init__(subset=subset)
+        super().__init__(subset=subset, ctx=ctx)
 
         self._items = list(self._load_items(path).values())
 
     def _load_items(self, path):
         items = {}
 
         anno_files = glob.glob(osp.join(path, "**", "*.h5"), recursive=True)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/open_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-# Copyright (C) 2021 Intel Corporation
+# Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import contextlib
 import csv
+import errno
 import fnmatch
 import functools
 import glob
 import itertools
 import json
 import logging as log
 import os
 import os.path as osp
 import re
 import types
+from typing import Optional, Union
 
 import cv2
 import numpy as np
 from attr import attrs
 
 from datumaro.components.annotation import AnnotationType, Bbox, Label, LabelCategories, Mask
 from datumaro.components.dataset import ItemStatus
@@ -26,15 +28,15 @@
     DatasetError,
     MediaTypeError,
     RepeatedItemError,
     UndefinedLabel,
 )
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.components.validator import Severity
 from datumaro.util import parse_json_file
 from datumaro.util.annotation_util import find_instances
 from datumaro.util.image import (
     DEFAULT_IMAGE_META_FILE_NAME,
     find_images,
@@ -164,19 +166,25 @@
         "BoxYMax",
         "PredictedIoU",
         "Clicks",
     )
 
 
 class OpenImagesBase(DatasetBase):
-    def __init__(self, path, image_meta=None):
+    def __init__(
+        self,
+        path: str,
+        *,
+        image_meta: Optional[Union[dict, str]] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isdir(path):
-            raise FileNotFoundError("Can't read dataset directory '%s'" % path)
+            raise NotADirectoryError(errno.ENOTDIR, "Can't find dataset directory", path)
 
-        super().__init__()
+        super().__init__(ctx=ctx)
 
         self._dataset_dir = path
 
         self._annotation_dir = osp.join(path, OpenImagesPath.ANNOTATIONS_DIR)
         if not osp.exists(self._annotation_dir):
             self._annotation_dir = path
         self._annotation_files = os.listdir(self._annotation_dir)
@@ -234,17 +242,18 @@
 
         class_desc_files = [
             file for pattern in class_desc_patterns for file in self._glob_annotations(pattern)
         ]
 
         if not class_desc_files:
             raise FileNotFoundError(
+                errno.ENOENT,
                 "Can't find class description file, the "
-                "annotations directory does't contain any of these files: %s"
-                % ", ".join(class_desc_patterns)
+                "annotations directory does't contain any of these files",
+                ", ".join(class_desc_patterns),
             )
 
         # In OID v6, the class description file is prefixed with `oidv6-`, whereas
         # in the previous versions, it isn't. We try to find it regardless.
         # We use a wildcard so that if, say, OID v7 is released in the future with
         # a similar layout as v6, it's automatically supported.
         # If the file doesn't exist with either name, we'll fail trying to open
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,45 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import os.path as osp
 from glob import iglob
+from typing import Optional
 
 from datumaro.components.annotation import AnnotationType, Cuboid3d, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
-from datumaro.components.importer import Importer
+from datumaro.components.errors import InvalidFieldError, UndeclaredLabelError
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image, PointCloud
 from datumaro.util import parse_json_file
 from datumaro.util.image import find_images
 
 from .format import PointCloudPath
 
 
 class SuperviselyPointCloudBase(SubsetBase):
     NAME = "sly_pointcloud"
     _SUPPORTED_SHAPES = "cuboid"
 
-    def __init__(self, path, subset=None):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isfile(path):
-            raise FileNotFoundError("Expected a path to 'meta.json', " "got '%s'" % path)
+            raise FileNotFoundError(errno.ENOENT, "Can't find annotations file", path)
 
         rootdir = osp.abspath(osp.dirname(path))
         self._rootdir = rootdir
 
-        super().__init__(subset=subset, media_type=PointCloud)
+        super().__init__(subset=subset, media_type=PointCloud, ctx=ctx)
 
         items, categories = self._parse(rootdir)
         self._items = list(self._load_items(items).values())
         self._categories = categories
 
     @classmethod
     def _parse(cls, rootpath):
@@ -47,24 +56,24 @@
             # https://github.com/supervisely/supervisely/blob/047e52ebe407cfee61464c1bd0beb9c906892253/supervisely_lib/annotation/tag_meta.py#L139
             tags[tag["name"]] = tag
 
             applicable_to = tag.get("applicable_type", "all")
             if applicable_to == "imagesOnly":
                 continue  # an image attribute
             elif applicable_to not in {"all", "objectsOnly"}:
-                raise Exception("Unexpected tag 'applicable_type' value '%s'" % applicable_to)
+                raise InvalidFieldError(applicable_to)
 
             applicable_classes = tag.get("classes", [])
             if not applicable_classes:
                 label_cat.attributes.add(tag["name"])
             else:
                 for label_name in applicable_classes:
                     _, label = label_cat.find(label_name)
                     if label is None:
-                        raise Exception("Unknown class for tag '%s'" % label_name)
+                        raise UndeclaredLabelError(label_name)
 
                     label.attributes.add(tag["name"])
 
         categories = {AnnotationType.label: label_cat}
 
         def _get_label_attrs(label_id):
             attrs = set(label_cat.attributes)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import shutil
 import uuid
 from datetime import datetime
 
 from datumaro.components.annotation import AnnotationType, LabelCategories
 from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DatasetItem, IDataset
-from datumaro.components.errors import MediaTypeError
+from datumaro.components.errors import DatasetExportError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.media import PointCloud
 from datumaro.util import cast, dump_json_file
 
 from .format import PointCloudPath
 
 
@@ -138,15 +138,15 @@
             if tag["applicable_type"] != "imagesOnly":
                 tag["applicable_type"] = "all"
 
             value_type = self._define_attr_type(attr_value)
             if tag["value_type"] is None:
                 tag["value_type"] = value_type
             elif tag["value_type"] != value_type:
-                raise Exception(
+                raise DatasetExportError(
                     "Item %s: mismatching "
                     "value types for tag %s: %s vs %s"
                     % (item.id, attr_name, tag["value_type"], value_type)
                 )
 
             tag_key = str(uuid.uuid4())
             item_ann_data["tags"].append(
@@ -224,15 +224,15 @@
                     elif tag["applicable_type"] == "objectsOnly" and tag["classes"]:
                         tag["classes"].add(object_label)
 
                     value_type = self._define_attr_type(attr_value)
                     if tag["value_type"] is None:
                         tag["value_type"] = value_type
                     elif tag["value_type"] != value_type:
-                        raise Exception(
+                        raise DatasetExportError(
                             "Item %s: mismatching "
                             "value types for tag %s: %s vs %s"
                             % (item.id, attr_name, tag["value_type"], value_type)
                         )
 
                     tag_key = str(uuid.uuid4())
                     obj_ann_data["tags"].append(
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/synthia.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/synthia/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,39 @@
-# Copyright (C) 2021 Intel Corporation
+# Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import os.path as osp
 from collections import OrderedDict
+from glob import glob
+from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, LabelCategories, Mask, MaskCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
-from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.errors import InvalidAnnotationError
+from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image
-from datumaro.util.image import find_images, load_image
-from datumaro.util.mask_tools import generate_colormap, lazy_mask
+from datumaro.util.image import find_images
+from datumaro.util.mask_tools import generate_colormap, load_mask
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
-
-class SynthiaPath:
-    IMAGES_DIR = "RGB"
-    LABELS_SEGM_DIR = "GT/LABELS"
-    SEMANTIC_SEGM_DIR = "GT/COLOR"
-    LABELMAP_FILE = "label_colors.txt"
-
-
-SYNTHIA_LABEL_MAP = OrderedDict(
-    [
-        ("Void", (0, 0, 0)),
-        ("Sky", (128, 128, 128)),
-        ("Building", (128, 0, 0)),
-        ("Road", (128, 64, 128)),
-        ("Sidewalk", (0, 0, 192)),
-        ("Fence", (64, 64, 128)),
-        ("Vegetation", (128, 128, 0)),
-        ("Pole", (192, 192, 128)),
-        ("Car", (64, 0, 128)),
-        ("TrafficSign", (192, 128, 128)),
-        ("Pedestrian", (64, 64, 0)),
-        ("Bicycle", (0, 128, 192)),
-        ("Lanemarking", (0, 172, 0)),
-        ("Reserved_1", (0, 0, 0)),
-        ("Reserved_2", (0, 0, 0)),
-        ("TrafficLight", (0, 128, 128)),
-    ]
+from .format import (
+    SynthiaAlLabelMap,
+    SynthiaAlPath,
+    SynthiaRandLabelMap,
+    SynthiaRandPath,
+    SynthiaSfLabelMap,
+    SynthiaSfPath,
 )
 
 
-def make_categories(label_map=None):
-    if label_map is None:
-        label_map = SYNTHIA_LABEL_MAP
-
+def make_categories(label_map):
     categories = {}
     label_categories = LabelCategories()
     for label in label_map:
         label_categories.add(label)
     categories[AnnotationType.label] = label_categories
 
     has_colors = any(v is not None for v in label_map.values())
@@ -86,91 +66,103 @@
                 name = label_desc[3]
                 color = tuple([int(c) for c in label_desc[:3]])
             else:
                 name = label_desc[0]
                 color = None
 
             if name in label_map:
-                raise ValueError("Label '%s' is already defined" % name)
+                raise InvalidAnnotationError("Label '%s' is already defined" % name)
 
             label_map[name] = color
     return label_map
 
 
-class SynthiaBase(SubsetBase):
-    def __init__(self, path):
+class _SynthiaBase(SubsetBase):
+    def __init__(
+        self,
+        path: str,
+        path_formats,
+        label_map,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isdir(path):
-            raise FileNotFoundError("Can't read dataset directory '%s'" % path)
+            raise NotADirectoryError(errno.ENOTDIR, "Can't find dataset directory", path)
+
+        super().__init__(subset=subset, ctx=ctx)
 
-        super().__init__()
+        self._path_formats = path_formats
+        self._label_map = label_map
+
+        self._img_dir = None
+        self._inst_dir = None
+        self._seg_dir = None
+        for path_format in vars(path_formats).keys():
+            if path_format == "IMAGES_DIR":
+                self._img_dir = osp.join(path, path_formats.IMAGES_DIR)
+            elif path_format == "LABELS_SEGM_DIR":
+                self._inst_dir = osp.join(path, path_formats.LABELS_SEGM_DIR)
+            elif path_format == "SEMANTIC_SEGM_DIR":
+                self._seg_dir = osp.join(path, path_formats.SEMANTIC_SEGM_DIR)
 
         self._categories = self._load_categories(path)
-        self._items = list(self._load_items(path).values())
+        self._items = list(self._load_items().values())
 
     def _load_categories(self, path):
         if has_meta_file(path):
             return make_categories(parse_meta_file(path))
-        label_map_path = osp.join(path, SynthiaPath.LABELMAP_FILE)
+
+        label_map_path = osp.join(path, "label_colors.txt")
         if osp.isfile(label_map_path):
             label_map = parse_label_map(label_map_path)
         else:
-            label_map = SYNTHIA_LABEL_MAP
+            label_map = self._label_map
+
         return make_categories(label_map)
 
-    def _load_items(self, root_dir):
-        image_dir = osp.join(root_dir, SynthiaPath.IMAGES_DIR)
-        if osp.isdir(image_dir):
+    def _load_items(self):
+        if self._img_dir and osp.isdir(self._img_dir):
             images = {
-                osp.splitext(osp.relpath(p, image_dir))[0].replace("\\", "/"): p
-                for p in find_images(image_dir, recursive=True)
+                osp.splitext(osp.relpath(p, self._img_dir))[0].replace("\\", "/"): p
+                for p in find_images(self._img_dir, recursive=True)
             }
         else:
             images = {}
 
         items = {}
-
-        inst_dir = osp.join(root_dir, SynthiaPath.LABELS_SEGM_DIR)
-        if osp.isdir(inst_dir):
-            gt_images = find_images(inst_dir, recursive=True)
-            for gt_img in gt_images:
-                item_id = osp.splitext(osp.relpath(gt_img, inst_dir))[0].replace("\\", "/")
+        if self._inst_dir and osp.isdir(self._inst_dir):
+            gt_labels = glob(self._inst_dir + "/*.txt")
+            for gt_label in gt_labels:
+                item_id = osp.splitext(osp.relpath(gt_label, self._inst_dir))[0].replace("\\", "/")
 
                 anno = []
-                labels_mask = load_image(gt_img, dtype=np.uint16)
-                dynamic_objects = np.unique(labels_mask[:, :, 1])
-                labels_mask = labels_mask[:, :, 2]
-                segm_ids = np.unique(labels_mask)
-                for segm_id in segm_ids:
-                    attr = {"dynamic_object": False}
-                    if segm_id != 0 and segm_id in dynamic_objects:
-                        attr["dynamic_object"] = True
+                labels_mask = np.loadtxt(gt_label)
+                classes = np.unique(labels_mask)
+                for label_id in classes:
                     anno.append(
-                        Mask(
-                            image=self._lazy_extract_mask(labels_mask, segm_id),
-                            label=segm_id,
-                            attributes=attr,
-                        )
+                        Mask(image=self._lazy_extract_mask(labels_mask, label_id), label=label_id)
                     )
 
                 image = images.get(item_id)
                 if image:
                     image = Image.from_file(path=image)
 
                 items[item_id] = DatasetItem(id=item_id, media=image, annotations=anno)
+        elif self._seg_dir and osp.isdir(self._seg_dir):
+            for seg_img_path in find_images(self._seg_dir, recursive=True):
+                item_id = osp.splitext(osp.relpath(seg_img_path, self._seg_dir))[0].replace(
+                    "\\", "/"
+                )
 
-        elif osp.isdir(osp.join(root_dir, SynthiaPath.SEMANTIC_SEGM_DIR)):
-            gt_dir = osp.join(root_dir, SynthiaPath.SEMANTIC_SEGM_DIR)
-            gt_images = find_images(gt_dir, recursive=True)
-            for gt_img in gt_images:
-                item_id = osp.splitext(osp.relpath(gt_img, gt_dir))[0].replace("\\", "/")
+                inverse_cls_colormap = self._categories[AnnotationType.mask].inverse_colormap
+
+                color_mask = load_mask(seg_img_path, inverse_cls_colormap, default_id=0)
 
                 anno = []
-                inverse_cls_colormap = self._categories[AnnotationType.mask].inverse_colormap
-                color_mask = lazy_mask(gt_img, inverse_cls_colormap)
-                color_mask = color_mask()
                 classes = np.unique(color_mask)
                 for label_id in classes:
                     anno.append(
                         Mask(image=self._lazy_extract_mask(color_mask, label_id), label=label_id)
                     )
 
                 image = images.get(item_id)
@@ -182,22 +174,26 @@
         return items
 
     @staticmethod
     def _lazy_extract_mask(mask, c):
         return lambda: mask == c
 
 
-class SynthiaImporter(Importer):
-    @classmethod
-    def detect(cls, context: FormatDetectionContext) -> None:
-        with context.require_any():
-            for prefix in (
-                SynthiaPath.IMAGES_DIR,
-                SynthiaPath.LABELS_SEGM_DIR,
-                SynthiaPath.SEMANTIC_SEGM_DIR,
-            ):
-                with context.alternative():
-                    context.require_file(f"{prefix}/**/*.png")
-
-    @classmethod
-    def find_sources(cls, path):
-        return [{"url": path, "format": "synthia"}]
+class SynthiaRandBase(_SynthiaBase):
+    def __init__(self, path: str, **kwargs):
+        super().__init__(
+            path=path, path_formats=SynthiaRandPath, label_map=SynthiaRandLabelMap, **kwargs
+        )
+
+
+class SynthiaSfBase(_SynthiaBase):
+    def __init__(self, path, **kwargs):
+        super().__init__(
+            path=path, path_formats=SynthiaSfPath, label_map=SynthiaSfLabelMap, **kwargs
+        )
+
+
+class SynthiaAlBase(_SynthiaBase):
+    def __init__(self, path, **kwargs):
+        super().__init__(
+            path=path, path_formats=SynthiaAlPath, label_map=SynthiaAlLabelMap, **kwargs
+        )
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,54 @@
-# Copyright (C) 2019-2020 Intel Corporation
+# Copyright (C) 2019-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 import re
 from collections import OrderedDict
+from typing import Optional
 
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, Bbox, LabelCategories, Mask
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.image import decode_image, lazy_image
 from datumaro.util.tf_util import import_tf as _import_tf
 
 from .format import DetectionApiPath
 
 tf = _import_tf()
 
 
 def clamp(value, _min, _max):
     return max(min(_max, value), _min)
 
 
 class TfDetectionApiBase(SubsetBase):
-    def __init__(self, path, subset=None):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         assert osp.isfile(path), path
         images_dir = ""
         root_dir = osp.dirname(osp.abspath(path))
         if osp.basename(root_dir) == DetectionApiPath.ANNOTATIONS_DIR:
             root_dir = osp.dirname(root_dir)
             images_dir = osp.join(root_dir, DetectionApiPath.IMAGES_DIR)
             if not osp.isdir(images_dir):
                 images_dir = ""
 
         if not subset:
             subset = osp.splitext(osp.basename(path))[0]
-        super().__init__(subset=subset)
+        super().__init__(subset=subset, ctx=ctx)
 
         items, labels = self._parse_tfrecord_file(path, self._subset, images_dir)
         self._items = items
         self._categories = self._load_categories(labels)
 
     @staticmethod
     def _load_categories(labels):
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import logging as log
 import os
 import os.path as osp
 import string
 from collections import OrderedDict
 
 from datumaro.components.annotation import AnnotationType, LabelCategories
+from datumaro.components.errors import DatasetExportError
 from datumaro.components.exporter import Exporter
 from datumaro.components.media import ByteImage, Image, ImageFromBytes
 from datumaro.util.annotation_util import find_group_leader, find_instances, max_bbox
 from datumaro.util.image import encode_image
 from datumaro.util.mask_tools import merge_masks
 from datumaro.util.tf_util import import_tf as _import_tf
 
@@ -164,15 +165,15 @@
             ),
         }
 
         filename = self._make_image_filename(item)
         features["image/filename"] = bytes_feature(filename.encode("utf-8"))
 
         if not isinstance(item.media, Image):
-            raise Exception(
+            raise DatasetExportError(
                 "Failed to export dataset item '%s': " "item has no image info" % item.id
             )
         height, width = item.media.size
 
         features.update(
             {
                 "image/height": int64_feature(height),
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-# Copyright (C) 2020-2021 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import csv
+import errno
 import os
 import os.path as osp
+from typing import Optional
 
 from datumaro.components.annotation import AnnotationType, Bbox, Label, LabelCategories, Points
 from datumaro.components.dataset_base import DatasetBase, DatasetItem
-from datumaro.components.errors import MediaTypeError
+from datumaro.components.errors import (
+    AnnotationExportError,
+    DatasetImportError,
+    InvalidAnnotationError,
+    MediaTypeError,
+)
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.image import find_images
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 
 class VggFace2Path:
     ANNOTATION_DIR = "bb_landmark"
@@ -23,38 +30,38 @@
     BBOXES_FILE = "loose_bb_"
     LANDMARKS_FILE = "loose_landmark_"
     LABELS_FILE = "labels.txt"
     IMAGES_DIR_NO_LABEL = "no_label"
 
 
 class VggFace2Base(DatasetBase):
-    def __init__(self, path):
+    def __init__(self, path: str, *, ctx: Optional[ImportContext] = None):
         subset = None
         if osp.isdir(path):
             self._path = path
         elif osp.isfile(path):
             subset = osp.splitext(osp.basename(path).split("_")[2])[0]
             self._path = osp.dirname(path)
         else:
-            raise Exception("Can't read annotations from '%s'" % path)
+            raise DatasetImportError("Can't read annotations from '%s'" % path)
 
         annotation_files = [
             p
             for p in os.listdir(self._path)
             if (
                 osp.basename(p).startswith(VggFace2Path.BBOXES_FILE)
                 or osp.basename(p).startswith(VggFace2Path.LANDMARKS_FILE)
             )
             and p.endswith(".csv")
         ]
 
         if len(annotation_files) < 1:
-            raise Exception("Can't find annotations in the directory '%s'" % path)
+            raise FileNotFoundError(errno.ENOENT, "Can't find annotations in the directory", path)
 
-        super().__init__()
+        super().__init__(ctx=ctx)
 
         self._dataset_dir = osp.dirname(self._path)
         self._subsets = (
             {subset} if subset else set(osp.splitext(f.split("_")[2])[0] for f in annotation_files)
         )
 
         self._categories = {}
@@ -136,15 +143,15 @@
                     image = images.get(row["NAME_ID"])
                     if image:
                         image = Image.from_file(path=image)
                     items[item_id] = DatasetItem(id=item_id, subset=subset, media=image)
 
                 annotations = items[item_id].annotations
                 if [a for a in annotations if a.type == AnnotationType.points]:
-                    raise Exception(
+                    raise InvalidAnnotationError(
                         "Item %s: an image can have only one " "set of landmarks" % item_id
                     )
 
                 if len([p for p in row if row[p] == ""]) == 0 and len(row) == 11:
                     annotations.append(
                         Points([float(row[p]) for p in row if p != "NAME_ID"], label=label)
                     )
@@ -169,15 +176,17 @@
                     image = images.get(row["NAME_ID"])
                     if image:
                         image = Image.from_file(path=image)
                     items[item_id] = DatasetItem(id=item_id, subset=subset, media=image)
 
                 annotations = items[item_id].annotations
                 if [a for a in annotations if a.type == AnnotationType.bbox]:
-                    raise Exception("Item %s: an image can have only one " "bbox" % item_id)
+                    raise InvalidAnnotationError(
+                        "Item %s: an image can have only one " "bbox" % item_id
+                    )
 
                 if len([p for p in row if row[p] == ""]) == 0 and len(row) == 5:
                     annotations.append(
                         Bbox(
                             float(row["X"]),
                             float(row["Y"]),
                             float(row["W"]),
@@ -271,15 +280,15 @@
                         image_dir = VggFace2Path.IMAGES_DIR_NO_LABEL
                         if 1 < len(item_parts) and image_dir == item_parts[0]:
                             image_dir = ""
                         self._save_image(item, subdir=osp.join(subset_name, image_dir))
 
                 landmarks = [a for a in item.annotations if a.type == AnnotationType.points]
                 if 1 < len(landmarks):
-                    raise Exception(
+                    raise AnnotationExportError(
                         "Item (%s, %s): an image can have only one "
                         "set of landmarks" % (item.id, item.subset)
                     )
                 if landmarks:
                     if landmarks[0].label is not None and label_categories[landmarks[0].label].name:
                         name_id = _get_name_id(
                             item_parts, label_categories[landmarks[0].label].name
@@ -304,15 +313,15 @@
                                 "P5X": points[8],
                                 "P5Y": points[9],
                             }
                         )
 
                 bboxes = [a for a in item.annotations if a.type == AnnotationType.bbox]
                 if 1 < len(bboxes):
-                    raise Exception(
+                    raise AnnotationExportError(
                         "Item (%s, %s): an image can have only one " "bbox" % (item.id, item.subset)
                     )
                 if bboxes:
                     if bboxes[0].label is not None and label_categories[bboxes[0].label].name:
                         name_id = _get_name_id(item_parts, label_categories[bboxes[0].label].name)
                     else:
                         name_id = _get_name_id(item_parts, VggFace2Path.IMAGES_DIR_NO_LABEL)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/video.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/video.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# Copyright (C) 2021 Intel Corporation
+# Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 from typing import Optional, Tuple
 
 import cv2
 import numpy as np
 
 from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME, DatasetBase, DatasetItem
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Video, VideoFrame
 from datumaro.util.os_util import find_files
 
 # Taken from https://en.wikipedia.org/wiki/Comparison_of_video_container_formats
 # An extension does not define file contents, but it can be a good file filter
 VIDEO_EXTENSIONS = [
     "3gp",
@@ -99,22 +99,23 @@
 
 
 class VideoFramesBase(DatasetBase):
     def __init__(
         self,
         url: str,
         *,
-        subset: Optional[str] = None,
         name_pattern: str = "%06d",
         step: int = 1,
         start_frame: int = 0,
         end_frame: Optional[int] = None,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
     ) -> None:
         self._subset = subset or DEFAULT_SUBSET_NAME
-        super().__init__(subsets=[self._subset], media_type=VideoFrame)
+        super().__init__(subsets=[self._subset], media_type=VideoFrame, ctx=ctx)
 
         assert osp.isfile(url), url
 
         self._name_pattern = name_pattern
         self._reader = Video(url, step=step, start_frame=start_frame, end_frame=end_frame)
         self._length = self._reader.length  # NOTE: the value is often incorrect
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (C) 2019-2022 Intel Corporation
+# Copyright (C) 2019-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import os.path as osp
 from typing import List, Optional, Tuple, Type, TypeVar
 
@@ -21,14 +21,15 @@
 from datumaro.components.errors import (
     DatasetImportError,
     InvalidAnnotationError,
     InvalidFieldError,
     MissingFieldError,
     UndeclaredLabelError,
 )
+from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image
 from datumaro.util.image import find_images
 from datumaro.util.mask_tools import invert_colormap, lazy_mask
 from datumaro.util.meta_file_util import has_meta_file
 
 from .format import (
     VocInstColormap,
@@ -40,40 +41,51 @@
 )
 
 _inverse_inst_colormap = invert_colormap(VocInstColormap)
 
 T = TypeVar("T")
 
 
-class _VocBase(SubsetBase):
-    def __init__(self, path, task, **kwargs):
+class VocBase(SubsetBase):
+    def __init__(
+        self,
+        path: str,
+        task: Optional[VocTask] = VocTask.voc,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isfile(path):
             raise DatasetImportError(f"Can't find txt subset list file at '{path}'")
         self._path = path
         self._dataset_dir = osp.dirname(osp.dirname(osp.dirname(path)))
 
         self._task = task
 
-        super().__init__(subset=osp.splitext(osp.basename(path))[0], **kwargs)
+        if not subset:
+            subset = osp.splitext(osp.basename(path))[0]
+
+        super().__init__(subset=subset, ctx=ctx)
 
         self._categories = self._load_categories(self._dataset_dir)
 
-        label_color = lambda label_idx: self._categories[AnnotationType.mask].colormap.get(
-            label_idx, None
-        )
-        log.debug(
-            "Loaded labels: %s",
-            ", ".join(
-                "'%s' %s" % (l.name, ("(%s, %s, %s)" % c) if c else "")
-                for i, l, c in (
-                    (i, l, label_color(i))
-                    for i, l in enumerate(self._categories[AnnotationType.label].items)
-                )
-            ),
-        )
+        if self._task in [VocTask.voc, VocTask.voc_segmentation, VocTask.voc_instance_segmentation]:
+            label_color = lambda label_idx: self._categories[AnnotationType.mask].colormap.get(
+                label_idx, None
+            )
+            log.debug(
+                "Loaded labels: %s",
+                ", ".join(
+                    "'%s' %s" % (l.name, ("(%s, %s, %s)" % c) if c else "")
+                    for i, l, c in (
+                        (i, l, label_color(i))
+                        for i, l in enumerate(self._categories[AnnotationType.label].items)
+                    )
+                ),
+            )
         self._items = {item: None for item in self._load_subset_list(path)}
 
     def _get_label_id(self, label: str) -> int:
         label_id, _ = self._categories[AnnotationType.label].find(label)
         if label_id is None:
             raise UndeclaredLabelError(label)
         return label_id
@@ -83,25 +95,25 @@
         if has_meta_file(dataset_path):
             label_map = parse_meta_file(dataset_path)
         else:
             label_map_path = osp.join(dataset_path, VocPath.LABELMAP_FILE)
             if osp.isfile(label_map_path):
                 label_map = parse_label_map(label_map_path)
 
-        return make_voc_categories(label_map)
+        return make_voc_categories(label_map, self._task)
 
     def _load_subset_list(self, subset_path):
         subset_list = []
         with open(subset_path, encoding="utf-8") as f:
             for i, line in enumerate(f):
                 line = line.strip()
                 if not line or line[0] == "#":
                     continue
 
-                if self._task == VocTask.person_layout:
+                if self._task == VocTask.voc_layout:
                     objects = line.split('"')
                     if 1 < len(objects):
                         if len(objects) == 3:
                             line = objects[1]
                         else:
                             raise InvalidAnnotationError(
                                 f"{osp.basename(subset_path)}:{i+1}: "
@@ -110,116 +122,66 @@
                     else:
                         line = line.split()[0]
                 else:
                     line = line.strip()
                 subset_list.append(line)
             return subset_list
 
-
-class VocClassificationBase(_VocBase):
-    def __init__(self, path, **kwargs):
-        super().__init__(path, VocTask.classification, **kwargs)
-
     def __iter__(self):
-        annotations = self._load_annotations()
-
         image_dir = osp.join(self._dataset_dir, VocPath.IMAGES_DIR)
         if osp.isdir(image_dir):
             images = {
                 osp.splitext(osp.relpath(p, image_dir))[0].replace("\\", "/"): p
                 for p in find_images(image_dir, recursive=True)
             }
         else:
             images = {}
 
-        for item_id in self._ctx.progress_reporter.iter(
-            self._items, desc=f"Parsing labels in '{self._subset}'"
-        ):
-            log.debug("Reading item '%s'", item_id)
-            image = images.get(item_id)
-            if image:
-                image = Image.from_file(path=image)
-            yield DatasetItem(
-                id=item_id, subset=self._subset, media=image, annotations=annotations.get(item_id)
-            )
-
-    def _load_annotations(self):
-        annotations = {}
-        task_dir = osp.dirname(self._path)
-        for label_id, label in enumerate(self._categories[AnnotationType.label]):
-            ann_file = osp.join(task_dir, f"{label.name}_{self._subset}.txt")
-            if not osp.isfile(ann_file):
-                continue
-
-            with open(ann_file, encoding="utf-8") as f:
-                for i, line in enumerate(f):
-                    line = line.strip()
-                    if not line or line[0] == "#":
-                        continue
-
-                    parts = line.rsplit(maxsplit=1)
-                    if len(parts) != 2:
-                        raise InvalidAnnotationError(
-                            f"{osp.basename(ann_file)}:{i+1}: "
-                            "invalid number of fields in line, expected 2"
-                        )
-
-                    item, present = parts
-                    if present not in ["-1", "0", "1"]:
-                        # Both -1 and 0 are used in the original VOC, they mean the same
-                        raise InvalidAnnotationError(
-                            f"{osp.basename(ann_file)}:{i+1}: "
-                            f"unexpected class existence value '{present}', expected -1, 0 or 1"
-                        )
-
-                    if present == "1":
-                        annotations.setdefault(item, []).append(Label(label_id))
-
-        return annotations
-
-
-class _VocXmlBase(_VocBase):
-    def __iter__(self):
-        image_dir = osp.join(self._dataset_dir, VocPath.IMAGES_DIR)
-        if osp.isdir(image_dir):
-            images = {
-                osp.splitext(osp.relpath(p, image_dir))[0].replace("\\", "/"): p
-                for p in find_images(image_dir, recursive=True)
-            }
-        else:
-            images = {}
+        annotations = (
+            self._parse_labels() if self._task in [VocTask.voc, VocTask.voc_classification] else {}
+        )
 
         anno_dir = osp.join(self._dataset_dir, VocPath.ANNOTATIONS_DIR)
 
         for item_id in self._ctx.progress_reporter.iter(
             self._items, desc=f"Parsing boxes in '{self._subset}'"
         ):
             log.debug("Reading item '%s'" % item_id)
             size = None
 
             try:
-                anns = []
+                anns = annotations.get(item_id, [])
                 image = None
 
                 ann_file = osp.join(anno_dir, item_id + ".xml")
-                if osp.isfile(ann_file):
+                if osp.isfile(ann_file) and self._task not in [
+                    VocTask.voc_classification,
+                    VocTask.voc_segmentation,
+                ]:
                     root_elem = ElementTree.parse(ann_file).getroot()
                     if root_elem.tag != "annotation":
                         raise MissingFieldError("annotation")
 
                     height = self._parse_field(root_elem, "size/height", int, required=False)
                     width = self._parse_field(root_elem, "size/width", int, required=False)
                     if height and width:
                         size = (height, width)
 
                     filename_elem = root_elem.find("filename")
                     if filename_elem is not None:
                         image = osp.join(image_dir, filename_elem.text)
 
-                    anns = self._parse_annotations(root_elem, item_id=(item_id, self._subset))
+                    anns += self._parse_annotations(root_elem, item_id=(item_id, self._subset))
+
+                if self._task in [
+                    VocTask.voc,
+                    VocTask.voc_segmentation,
+                    VocTask.voc_instance_segmentation,
+                ]:
+                    anns += self._parse_masks(item_id)
 
                 if image is None:
                     image = images.pop(item_id, None)
 
                 if image or size:
                     image = Image.from_file(path=image, size=size)
 
@@ -256,151 +218,110 @@
         if elem is None:
             return default
 
         if elem.text not in ["0", "1"]:
             raise InvalidFieldError(xpath)
         return elem.text == "1"
 
-    def _parse_annotations(self, root_elem, *, item_id: Tuple[str, str]) -> List[Annotation]:
-        item_annotations = []
+    def _parse_attribute(self, object_elem):
+        attributes = {}
 
-        for obj_id, object_elem in enumerate(root_elem.iterfind("object")):
-            try:
-                obj_id += 1
-                attributes = {}
-                group = obj_id
+        for key in ["difficult", "truncated", "occluded"]:
+            attributes[key] = self._parse_bool_field(object_elem, key, default=False)
 
-                obj_label_id = self._get_label_id(self._parse_field(object_elem, "name"))
-
-                obj_bbox = self._parse_bbox(object_elem)
-
-                for key in ["difficult", "truncated", "occluded"]:
-                    attributes[key] = self._parse_bool_field(object_elem, key, default=False)
-
-                pose_elem = object_elem.find("pose")
-                if pose_elem is not None:
-                    attributes["pose"] = pose_elem.text
-
-                point_elem = object_elem.find("point")
-                if point_elem is not None:
-                    point_x = self._parse_field(point_elem, "x", float)
-                    point_y = self._parse_field(point_elem, "y", float)
-                    attributes["point"] = (point_x, point_y)
-
-                actions_elem = object_elem.find("actions")
-                actions = {
-                    a: False
-                    for a in self._categories[AnnotationType.label].items[obj_label_id].attributes
-                }
-                if actions_elem is not None:
-                    for action_elem in actions_elem:
-                        actions[action_elem.tag] = self._parse_bool_field(
-                            actions_elem, action_elem.tag
-                        )
-                for action, present in actions.items():
-                    attributes[action] = present
-
-                has_parts = False
-                for part_elem in object_elem.findall("part"):
-                    part_label_id = self._get_label_id(self._parse_field(part_elem, "name"))
-                    part_bbox = self._parse_bbox(part_elem)
-
-                    if self._task is not VocTask.person_layout:
-                        break
-                    has_parts = True
-                    item_annotations.append(Bbox(*part_bbox, label=part_label_id, group=group))
-
-                attributes_elem = object_elem.find("attributes")
-                if attributes_elem is not None:
-                    for attr_elem in attributes_elem.iter("attribute"):
-                        attributes[self._parse_field(attr_elem, "name")] = self._parse_field(
-                            attr_elem, "value"
-                        )
-
-                if self._task is VocTask.person_layout and not has_parts:
-                    continue
-                if self._task is VocTask.action_classification and not actions:
-                    continue
-
-                item_annotations.append(
-                    Bbox(
-                        *obj_bbox, label=obj_label_id, attributes=attributes, id=obj_id, group=group
-                    )
+        pose_elem = object_elem.find("pose")
+        if pose_elem is not None:
+            attributes["pose"] = pose_elem.text
+
+        point_elem = object_elem.find("point")
+        if point_elem is not None:
+            point_x = self._parse_field(point_elem, "x", float)
+            point_y = self._parse_field(point_elem, "y", float)
+            attributes["point"] = (point_x, point_y)
+
+        attributes_elem = object_elem.find("attributes")
+        if attributes_elem is not None:
+            for attr_elem in attributes_elem.iter("attribute"):
+                attributes[self._parse_field(attr_elem, "name")] = self._parse_field(
+                    attr_elem, "value"
                 )
-            except Exception as e:
-                self._ctx.error_policy.report_annotation_error(e, item_id=item_id)
 
-        return item_annotations
+        return attributes
 
     @classmethod
     def _parse_bbox(cls, object_elem):
         bbox_elem = object_elem.find("bndbox")
         if not bbox_elem:
             raise MissingFieldError("bndbox")
 
         xmin = cls._parse_field(bbox_elem, "xmin", float)
         xmax = cls._parse_field(bbox_elem, "xmax", float)
         ymin = cls._parse_field(bbox_elem, "ymin", float)
         ymax = cls._parse_field(bbox_elem, "ymax", float)
         return [xmin, ymin, xmax - xmin, ymax - ymin]
 
+    def _parse_annotations(self, root_elem, *, item_id: Tuple[str, str]) -> List[Annotation]:
+        item_annotations = []
 
-class VocDetectionBase(_VocXmlBase):
-    def __init__(self, path, **kwargs):
-        super().__init__(path, task=VocTask.detection, **kwargs)
-
-
-class VocLayoutBase(_VocXmlBase):
-    def __init__(self, path, **kwargs):
-        super().__init__(path, task=VocTask.person_layout, **kwargs)
-
-
-class VocActionBase(_VocXmlBase):
-    def __init__(self, path, **kwargs):
-        super().__init__(path, task=VocTask.action_classification, **kwargs)
-
+        obj_id = 0
+        for object_elem in root_elem.iterfind("object"):
+            try:
+                label_name = self._parse_field(object_elem, "name")
 
-class VocSegmentationBase(_VocBase):
-    def __init__(self, path, **kwargs):
-        super().__init__(path, task=VocTask.segmentation, **kwargs)
+                # person_layout and action_classification are only available for background and person
+                if self._task in [VocTask.voc_layout, VocTask.voc_action] and (
+                    label_name not in ["person", "background"]
+                ):
+                    continue
 
-    def __iter__(self):
-        image_dir = osp.join(self._dataset_dir, VocPath.IMAGES_DIR)
-        if osp.isdir(image_dir):
-            images = {
-                osp.splitext(osp.relpath(p, image_dir))[0].replace("\\", "/"): p
-                for p in find_images(image_dir, recursive=True)
-            }
-        else:
-            images = {}
+                obj_label_id = self._get_label_id(label_name)
+                obj_bbox = self._parse_bbox(object_elem)
+                attributes = self._parse_attribute(object_elem)
 
-        for item_id in self._ctx.progress_reporter.iter(
-            self._items, desc=f"Parsing segmentation in '{self._subset}'"
-        ):
-            log.debug("Reading item '%s'", item_id)
+                group = obj_id
 
-            image = images.get(item_id)
-            if image:
-                image = Image.from_file(path=image)
+                if self._task in [VocTask.voc, VocTask.voc_layout]:
+                    for part_elem in object_elem.findall("part"):
+                        part_label_id = self._get_label_id(self._parse_field(part_elem, "name"))
+                        part_bbox = self._parse_bbox(part_elem)
+
+                        item_annotations.append(Bbox(*part_bbox, label=part_label_id, group=group))
+
+                if self._task in [VocTask.voc, VocTask.voc_action]:
+                    actions_elem = object_elem.find("actions")
+                    actions = {
+                        a: False
+                        for a in self._categories[AnnotationType.label]
+                        .items[obj_label_id]
+                        .attributes
+                    }
+                    if actions_elem is not None:
+                        for action_elem in actions_elem:
+                            actions[action_elem.tag] = self._parse_bool_field(
+                                actions_elem, action_elem.tag
+                            )
+                    for action, present in actions.items():
+                        attributes[action] = present
 
-            try:
-                yield DatasetItem(
-                    id=item_id,
-                    subset=self._subset,
-                    media=image,
-                    annotations=self._load_annotations(item_id),
+                item_annotations.append(
+                    Bbox(
+                        *obj_bbox, label=obj_label_id, attributes=attributes, id=obj_id, group=group
+                    )
                 )
+                obj_id += 1
             except Exception as e:
-                self._ctx.error_policy.report_item_error(e, item_id=(item_id, self._subset))
+                self._ctx.error_policy.report_annotation_error(e, item_id=item_id)
+
+        return item_annotations
 
     @staticmethod
     def _lazy_extract_mask(mask, c):
         return lambda: mask == c
 
-    def _load_annotations(self, item_id):
+    def _parse_masks(self, item_id):
         item_annotations = []
 
         class_mask = None
         segm_path = osp.join(
             self._dataset_dir, VocPath.SEGMENTATION_DIR, item_id + VocPath.SEGM_EXT
         )
         if osp.isfile(segm_path):
@@ -442,7 +363,71 @@
                         UndeclaredLabelError(str(label_id)), item_id=(item_id, self._subset)
                     )
 
                 image = self._lazy_extract_mask(class_mask, label_id)
                 item_annotations.append(Mask(image=image, label=label_id))
 
         return item_annotations
+
+    def _parse_labels(self):
+        annotations = {}
+        task_dir = osp.dirname(self._path)
+        for label_id, label in enumerate(self._categories[AnnotationType.label]):
+            ann_file = osp.join(task_dir, f"{label.name}_{self._subset}.txt")
+            if not osp.isfile(ann_file):
+                continue
+
+            with open(ann_file, encoding="utf-8") as f:
+                for i, line in enumerate(f):
+                    line = line.strip()
+                    if not line or line[0] == "#":
+                        continue
+
+                    parts = line.rsplit(maxsplit=1)
+                    if len(parts) != 2:
+                        raise InvalidAnnotationError(
+                            f"{osp.basename(ann_file)}:{i+1}: "
+                            "invalid number of fields in line, expected 2"
+                        )
+
+                    item, present = parts
+                    if present not in ["-1", "0", "1"]:
+                        # Both -1 and 0 are used in the original VOC, they mean the same
+                        raise InvalidAnnotationError(
+                            f"{osp.basename(ann_file)}:{i+1}: "
+                            f"unexpected class existence value '{present}', expected -1, 0 or 1"
+                        )
+
+                    if present == "1":
+                        annotations.setdefault(item, []).append(Label(label_id))
+
+        return annotations
+
+
+class VocClassificationBase(VocBase):
+    def __init__(self, path, **kwargs):
+        super().__init__(path, task=VocTask.voc_classification, **kwargs)
+
+
+class VocDetectionBase(VocBase):
+    def __init__(self, path, **kwargs):
+        super().__init__(path, task=VocTask.voc_detection, **kwargs)
+
+
+class VocSegmentationBase(VocBase):
+    def __init__(self, path, **kwargs):
+        super().__init__(path, task=VocTask.voc_segmentation, **kwargs)
+
+
+class VocInstanceSegmentationBase(VocBase):
+    def __init__(self, path, **kwargs):
+        super().__init__(path, task=VocTask.voc_instance_segmentation, **kwargs)
+
+
+class VocLayoutBase(VocBase):
+    def __init__(self, path, **kwargs):
+        super().__init__(path, task=VocTask.voc_layout, **kwargs)
+
+
+class VocActionBase(VocBase):
+    def __init__(self, path, **kwargs):
+        super().__init__(path, task=VocTask.voc_action, **kwargs)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     CompiledMask,
     Label,
     LabelCategories,
     Mask,
 )
 from datumaro.components.dataset import ItemStatus
 from datumaro.components.dataset_base import DatasetItem
-from datumaro.components.errors import MediaTypeError
+from datumaro.components.errors import DatasetExportError, InvalidAnnotationError, MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.media import Image
 from datumaro.util import find, str_to_bool
 from datumaro.util.annotation_util import make_label_id_mapping
 from datumaro.util.image import save_image
 from datumaro.util.mask_tools import paint_mask, remap_mask
 from datumaro.util.meta_file_util import has_meta_file
@@ -68,14 +68,20 @@
     ET.SubElement(bbox_elem, "xmax").text = str(x + w)
     ET.SubElement(bbox_elem, "ymax").text = str(y + h)
     return bbox_elem
 
 
 class LabelmapType(Enum):
     voc = auto()
+    voc_classification = auto()
+    voc_detection = auto()
+    voc_segmentation = auto()
+    voc_instance_segmentation = auto()
+    voc_layout = auto()
+    voc_action = auto()
     source = auto()
 
 
 @define
 class _SubsetLists:
     class_lists: Dict[str, Optional[Set[int]]] = field(factory=dict)
     clsdet_list: Dict[str, Optional[bool]] = field(factory=dict)
@@ -85,15 +91,15 @@
 
 
 class VocExporter(Exporter):
     DEFAULT_IMAGE_EXT = VocPath.IMAGE_EXT
     BUILTIN_ATTRS = {"difficult", "pose", "truncated", "occluded"}
 
     @staticmethod
-    def _split_tasks_string(s):
+    def _split_task_string(s):
         return [VocTask[i.strip()] for i in s.split(",")]
 
     @staticmethod
     def _get_labelmap(s):
         if osp.isfile(s):
             return s
         try:
@@ -128,43 +134,43 @@
         parser.add_argument(
             "--keep-empty",
             type=str_to_bool,
             default=False,
             help="Write subset lists even if they are empty " "(default: %(default)s)",
         )
         parser.add_argument(
-            "--tasks",
-            type=cls._split_tasks_string,
-            help="VOC task filter, comma-separated list of {%s} "
-            "(default: all)" % ", ".join(t.name for t in VocTask),
+            "--task",
+            type=cls._split_task_string,
+            default=VocTask.voc,
+            help="VOC task filter, one of list {%s} "
+            "(default: voc)" % ", ".join(t.name for t in VocTask),
         )
 
         return parser
 
     def __init__(
         self,
         extractor,
         save_dir,
-        tasks=None,
+        task=None,
         apply_colormap=True,
         label_map=None,
         allow_attributes=True,
         keep_empty=False,
         **kwargs,
     ):
         super().__init__(extractor, save_dir, **kwargs)
 
-        assert tasks is None or isinstance(tasks, (VocTask, list, set))
-        if tasks is None:
-            tasks = set(VocTask)
-        elif isinstance(tasks, VocTask):
-            tasks = {tasks}
-        else:
-            tasks = set(t if t in VocTask else VocTask[t] for t in tasks)
-        self._tasks = tasks
+        task = VocTask.voc if task is None else task
+        if not isinstance(task, VocTask):
+            raise DatasetExportError(
+                f"The task must be an instance of {VocTask} but {task} is given."
+            )
+
+        self._task = task
 
         self._apply_colormap = apply_colormap
         self._allow_attributes = allow_attributes
         self._keep_empty = keep_empty
 
         if label_map is None:
             label_map = LabelmapType.source.name
@@ -180,18 +186,18 @@
         self.make_dirs()
         self.save_subsets()
         self.save_label_map()
 
     def make_dirs(self):
         save_dir = self._save_dir
         subsets_dir = osp.join(save_dir, VocPath.SUBSETS_DIR)
-        cls_subsets_dir = osp.join(subsets_dir, VocPath.TASK_DIR[VocTask.classification])
-        action_subsets_dir = osp.join(subsets_dir, VocPath.TASK_DIR[VocTask.action_classification])
-        layout_subsets_dir = osp.join(subsets_dir, VocPath.TASK_DIR[VocTask.person_layout])
-        segm_subsets_dir = osp.join(subsets_dir, VocPath.TASK_DIR[VocTask.segmentation])
+        cls_subsets_dir = osp.join(subsets_dir, VocPath.TASK_DIR[VocTask.voc_classification])
+        action_subsets_dir = osp.join(subsets_dir, VocPath.TASK_DIR[VocTask.voc_action])
+        layout_subsets_dir = osp.join(subsets_dir, VocPath.TASK_DIR[VocTask.voc_layout])
+        segm_subsets_dir = osp.join(subsets_dir, VocPath.TASK_DIR[VocTask.voc_segmentation])
         ann_dir = osp.join(save_dir, VocPath.ANNOTATIONS_DIR)
         img_dir = osp.join(save_dir, VocPath.IMAGES_DIR)
         segm_dir = osp.join(save_dir, VocPath.SEGMENTATION_DIR)
         inst_dir = osp.join(save_dir, VocPath.INSTANCES_DIR)
         images_dir = osp.join(save_dir, VocPath.IMAGES_DIR)
 
         os.makedirs(subsets_dir, exist_ok=True)
@@ -232,43 +238,55 @@
                         else:
                             log.debug("Item '%s' has no image", item.id)
 
                     self._export_annotations(item, image_filename=image_filename, lists=lists)
                 except Exception as e:
                     self._ctx.error_policy.report_item_error(e, item_id=(item.id, item.subset))
 
-            if self._tasks & {
-                VocTask.classification,
-                VocTask.detection,
-                VocTask.action_classification,
-                VocTask.person_layout,
-            }:
+            if self._task in [
+                VocTask.voc,
+                VocTask.voc_classification,
+                VocTask.voc_detection,
+                VocTask.voc_action,
+                VocTask.voc_layout,
+                VocTask.voc_instance_segmentation,
+            ]:
                 self.save_clsdet_lists(subset_name, lists.clsdet_list)
-                if self._tasks & {VocTask.classification}:
+                if self._task in [VocTask.voc, VocTask.voc_classification]:
                     self.save_class_lists(subset_name, lists.class_lists)
-            if self._tasks & {VocTask.action_classification}:
+            if self._task in [VocTask.voc, VocTask.voc_action]:
                 self.save_action_lists(subset_name, lists.action_list)
-            if self._tasks & {VocTask.person_layout}:
+            if self._task in [VocTask.voc, VocTask.voc_layout]:
                 self.save_layout_lists(subset_name, lists.layout_list)
-            if self._tasks & {VocTask.segmentation}:
+            if self._task in [
+                VocTask.voc,
+                VocTask.voc_segmentation,
+                VocTask.voc_instance_segmentation,
+            ]:
                 self.save_segm_lists(subset_name, lists.segm_list)
 
     def _export_annotations(self, item: DatasetItem, *, image_filename: str, lists: _SubsetLists):
         labels = []
         bboxes = []
         masks = []
         for a in item.annotations:
             if isinstance(a, Label):
                 labels.append(a)
             elif isinstance(a, Bbox):
                 bboxes.append(a)
             elif isinstance(a, Mask):
                 masks.append(a)
 
-        if self._tasks & {VocTask.detection, VocTask.person_layout, VocTask.action_classification}:
+        if self._task in [
+            VocTask.voc,
+            VocTask.voc_detection,
+            VocTask.voc_instance_segmentation,
+            VocTask.voc_layout,
+            VocTask.voc_action,
+        ]:
             root_elem = ET.Element("annotation")
             if "_" in item.id:
                 folder = item.id[: item.id.find("_")]
             else:
                 folder = ""
             ET.SubElement(root_elem, "folder").text = folder
             ET.SubElement(root_elem, "filename").text = image_filename
@@ -294,18 +312,18 @@
             objects_with_parts = []
             objects_with_actions = defaultdict(dict)
 
             main_bboxes = []
             layout_bboxes = []
             for bbox in bboxes:
                 label = self.get_label(bbox.label)
-                if self._is_part(label):
-                    layout_bboxes.append(bbox)
-                elif self._is_label(label):
+                if self._is_label(label):
                     main_bboxes.append(bbox)
+                elif self._is_part(label):
+                    layout_bboxes.append(bbox)
 
             for new_obj_id, obj in enumerate(main_bboxes):
                 attr = obj.attributes
 
                 obj_elem = ET.SubElement(root_elem, "object")
 
                 obj_label = self.get_label(obj.label)
@@ -324,35 +342,38 @@
                     "difficult", attr, int, 0
                 )
 
                 bbox = obj.get_bbox()
                 if bbox is not None:
                     _write_xml_bbox(bbox, obj_elem)
 
-                for part_bbox in filter(
-                    lambda x: obj.group and obj.group == x.group, layout_bboxes
-                ):
-                    part_elem = ET.SubElement(obj_elem, "part")
-                    ET.SubElement(part_elem, "name").text = self.get_label(part_bbox.label)
-                    _write_xml_bbox(part_bbox.get_bbox(), part_elem)
+                if self._task in [VocTask.voc, VocTask.voc_layout]:
+                    for part_bbox in layout_bboxes:
+                        if part_bbox.group != obj.group:
+                            continue
 
-                    objects_with_parts.append(new_obj_id)
+                        part_elem = ET.SubElement(obj_elem, "part")
+                        ET.SubElement(part_elem, "name").text = self.get_label(part_bbox.label)
+                        _write_xml_bbox(part_bbox.get_bbox(), part_elem)
+
+                        objects_with_parts.append(new_obj_id)
 
                 label_actions = self._get_actions(obj_label)
                 actions_elem = ET.Element("actions")
                 for action in label_actions:
                     present = 0
                     if action in attr:
                         present = _convert_attr(action, attr, lambda v: int(v is True), 0)
                         if action.isdigit():
                             action = "_" + action
                         action = action.replace(" ", "_")
                         ET.SubElement(actions_elem, action).text = "%d" % present
 
                     objects_with_actions[new_obj_id][action] = present
+
                 if len(actions_elem) != 0:
                     obj_elem.append(actions_elem)
 
                 if self._allow_attributes:
                     native_attrs = set(self.BUILTIN_ATTRS)
                     native_attrs.update(label_actions)
 
@@ -362,43 +383,41 @@
                             continue
                         attr_elem = ET.SubElement(attrs_elem, "attribute")
                         ET.SubElement(attr_elem, "name").text = str(k)
                         ET.SubElement(attr_elem, "value").text = str(v)
                     if len(attrs_elem):
                         obj_elem.append(attrs_elem)
 
-            if self._tasks & {
-                VocTask.detection,
-                VocTask.person_layout,
-                VocTask.action_classification,
-            }:
                 ann_path = osp.join(self._ann_dir, item.id + ".xml")
                 os.makedirs(osp.dirname(ann_path), exist_ok=True)
                 with open(ann_path, "w", encoding="utf-8") as f:
                     f.write(ET.tostring(root_elem, encoding="unicode", pretty_print=True))
 
             lists.clsdet_list[item.id] = True
 
-            if objects_with_parts:
+            if self._task in [VocTask.voc, VocTask.voc_layout] and objects_with_parts:
                 lists.layout_list[item.id] = objects_with_parts
 
-            if objects_with_actions:
+            if self._task in [VocTask.voc, VocTask.voc_action] and objects_with_actions:
                 lists.action_list[item.id] = objects_with_actions
 
         for label_ann in labels:
             label = self.get_label(label_ann.label)
             if not self._is_label(label):
                 continue
             class_list = lists.class_lists.get(item.id, set())
             class_list.add(label_ann.label)
             lists.class_lists[item.id] = class_list
 
             lists.clsdet_list[item.id] = True
 
-        if masks and VocTask.segmentation in self._tasks:
+        if (
+            self._task in [VocTask.voc, VocTask.voc_segmentation, VocTask.voc_instance_segmentation]
+            and masks
+        ):
             compiled_mask = CompiledMask.from_instance_masks(
                 masks, instance_labels=[self._label_id_mapping(m.label) for m in masks]
             )
 
             self.save_segm(
                 osp.join(self._segm_dir, item.id + VocPath.SEGM_EXT), compiled_mask.class_mask
             )
@@ -518,14 +537,15 @@
                         print(item, *lines[item], file=f)
 
     def save_clsdet_lists(self, subset_name, clsdet_list):
         os.makedirs(self._cls_subsets_dir, exist_ok=True)
 
         ann_file = osp.join(self._cls_subsets_dir, subset_name + ".txt")
         items = {k: True for k in clsdet_list}
+
         if self._patch and osp.isfile(ann_file):
             self._get_filtered_lines(ann_file, self._patch, subset_name, items)
 
         if items or self._keep_empty:
             with open(ann_file, "w", encoding="utf-8") as f:
                 for item in items:
                     f.write("%s\n" % item)
@@ -588,17 +608,19 @@
         if self._save_dataset_meta:
             write_meta_file(self._save_dir, self._label_map)
         else:
             path = osp.join(self._save_dir, VocPath.LABELMAP_FILE)
             write_label_map(path, self._label_map)
 
     def _load_categories(self, label_map_source):
-        if label_map_source == LabelmapType.voc.name:
-            # use the default VOC colormap
-            label_map = make_voc_label_map()
+        if (
+            label_map_source in [t.name for t in LabelmapType]
+            and label_map_source != LabelmapType.source.name
+        ):
+            label_map = make_voc_label_map(task=self._task)
 
         elif (
             label_map_source == LabelmapType.source.name
             and AnnotationType.mask not in self._extractor.categories()
         ):
             # generate colormap for input labels
             labels = self._extractor.categories().get(AnnotationType.label, LabelCategories())
@@ -623,36 +645,44 @@
         elif isinstance(label_map_source, str) and osp.isfile(label_map_source):
             if has_meta_file(label_map_source):
                 label_map = parse_meta_file(label_map_source)
             else:
                 label_map = parse_label_map(label_map_source)
 
         else:
-            raise Exception(
+            raise InvalidAnnotationError(
                 "Wrong labelmap specified: '%s', "
                 "expected one of %s or a file path"
                 % (label_map_source, ", ".join(t.name for t in LabelmapType))
             )
 
         bg_label = find(label_map.items(), lambda x: x[1][0] == (0, 0, 0))
         if bg_label is None:
             bg_label = "background"
             if bg_label not in label_map:
                 has_colors = any(v[0] is not None for v in label_map.values())
                 color = (0, 0, 0) if has_colors else None
                 label_map[bg_label] = [color, [], []]
             label_map.move_to_end(bg_label, last=False)
 
-        self._categories = make_voc_categories(label_map)
+        self._categories = make_voc_categories(label_map, task=self._task)
 
         # Update colors with assigned values
-        colormap = self._categories[AnnotationType.mask].colormap
-        for label_id, color in colormap.items():
-            label_desc = label_map[self._categories[AnnotationType.label].items[label_id].name]
-            label_desc[0] = color
+        if label_map_source in [
+            LabelmapType.voc.name,
+            LabelmapType.voc_segmentation.name,
+            LabelmapType.voc_instance_segmentation.name,
+        ]:
+            colormap = self._categories[AnnotationType.mask].colormap
+            for label_id, color in colormap.items():
+                if label_id:
+                    label_desc = label_map[
+                        self._categories[AnnotationType.label].items[label_id].name
+                    ]
+                    label_desc[0] = color
 
         self._label_map = label_map
         self._label_id_mapping = self._make_label_id_map()
 
     def _is_label(self, s):
         return self._label_map.get(s) is not None
 
@@ -674,15 +704,15 @@
     def _make_label_id_map(self):
         map_id, id_mapping, src_labels, dst_labels = make_label_id_mapping(
             self._extractor.categories().get(AnnotationType.label),
             self._categories[AnnotationType.label],
         )
 
         void_labels = [
-            src_label for src_id, src_label in src_labels.items() if src_label not in dst_labels
+            src_label for src_label in src_labels.values() if src_label not in dst_labels
         ]
         if void_labels:
             log.warning(
                 "The following labels are remapped to background: %s" % ", ".join(void_labels)
             )
         log.debug(
             "Saving segmentations with the following label mapping: \n%s"
@@ -737,19 +767,21 @@
             else:
                 ids_to_remove.setdefault(item_id, (item, True))
 
         for item, to_remove in ids_to_remove.values():
             if not to_remove:
                 continue
 
-            if conv._tasks & {
-                VocTask.detection,
-                VocTask.action_classification,
-                VocTask.person_layout,
-            }:
+            if conv._task in [
+                VocTask.voc,
+                VocTask.voc_detection,
+                VocTask.voc_instance_segmentation,
+                VocTask.voc_action,
+                VocTask.voc_layout,
+            ]:
                 ann_path = osp.join(conv._ann_dir, item.id + ".xml")
                 if osp.isfile(ann_path):
                     os.remove(ann_path)
 
             image_path = osp.join(conv._images_dir, conv._make_image_filename(item))
             if osp.isfile(image_path):
                 os.unlink(image_path)
@@ -762,33 +794,39 @@
                 path = osp.join(save_dir, VocPath.INSTANCES_DIR, item.id + VocPath.SEGM_EXT)
                 if osp.isfile(path):
                     os.unlink(path)
 
 
 class VocClassificationExporter(VocExporter):
     def __init__(self, *args, **kwargs):
-        kwargs["tasks"] = VocTask.classification
+        kwargs["task"] = VocTask.voc_classification
         super().__init__(*args, **kwargs)
 
 
 class VocDetectionExporter(VocExporter):
     def __init__(self, *args, **kwargs):
-        kwargs["tasks"] = VocTask.detection
+        kwargs["task"] = VocTask.voc_detection
         super().__init__(*args, **kwargs)
 
 
-class VocLayoutExporter(VocExporter):
+class VocSegmentationExporter(VocExporter):
     def __init__(self, *args, **kwargs):
-        kwargs["tasks"] = VocTask.person_layout
+        kwargs["task"] = VocTask.voc_segmentation
         super().__init__(*args, **kwargs)
 
 
-class VocActionExporter(VocExporter):
+class VocInstanceSegmentationExporter(VocExporter):
     def __init__(self, *args, **kwargs):
-        kwargs["tasks"] = VocTask.action_classification
+        kwargs["task"] = VocTask.voc_instance_segmentation
         super().__init__(*args, **kwargs)
 
 
-class VocSegmentationExporter(VocExporter):
+class VocLayoutExporter(VocExporter):
+    def __init__(self, *args, **kwargs):
+        kwargs["task"] = VocTask.voc_layout
+        super().__init__(*args, **kwargs)
+
+
+class VocActionExporter(VocExporter):
     def __init__(self, *args, **kwargs):
-        kwargs["tasks"] = VocTask.segmentation
+        kwargs["task"] = VocTask.voc_action
         super().__init__(*args, **kwargs)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/format.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,19 +20,21 @@
 from datumaro.components.dataset_base import CategoriesInfo
 from datumaro.components.errors import InvalidAnnotationError
 from datumaro.util import dump_json_file, find, parse_json_file
 from datumaro.util.meta_file_util import get_meta_file
 
 
 class VocTask(Enum):
-    classification = auto()
-    detection = auto()
-    segmentation = auto()
-    action_classification = auto()
-    person_layout = auto()
+    voc = auto()
+    voc_classification = auto()
+    voc_detection = auto()
+    voc_segmentation = auto()
+    voc_instance_segmentation = auto()
+    voc_action = auto()
+    voc_layout = auto()
 
 
 class VocLabel(Enum):
     background = 0
     aeroplane = 1
     bicycle = 2
     bird = 3
@@ -112,34 +114,72 @@
     INSTANCES_DIR = "SegmentationObject"
     SUBSETS_DIR = "ImageSets"
     IMAGE_EXT = ".jpg"
     SEGM_EXT = ".png"
     LABELMAP_FILE = "labelmap.txt"
 
     TASK_DIR = {
-        VocTask.classification: "Main",
-        VocTask.detection: "Main",
-        VocTask.segmentation: "Segmentation",
-        VocTask.action_classification: "Action",
-        VocTask.person_layout: "Layout",
+        VocTask.voc: "Main",
+        VocTask.voc_classification: "Main",
+        VocTask.voc_detection: "Main",
+        VocTask.voc_segmentation: "Segmentation",
+        VocTask.voc_instance_segmentation: "Segmentation",
+        VocTask.voc_action: "Action",
+        VocTask.voc_layout: "Layout",
     }
 
 
 LabelMapConfig = Dict[str, Tuple[Optional[RgbColor], List[str], List[str]]]
 """A type representing a label map config"""
 # Not totally type-correct, tuple elements are supposed to support modification.
 # Therefore, the tuple is typically a list
 # TODO: refactor, make type annotations conform with actual usage
 
 
-def make_voc_label_map() -> LabelMapConfig:
-    labels = sorted(VocLabel, key=lambda l: l.value)
-    label_map = OrderedDict((label.name, [VocColormap[label.value], [], []]) for label in labels)
-    label_map[VocLabel.person.name][1] = [p.name for p in VocBodyPart]
-    label_map[VocLabel.person.name][2] = [a.name for a in VocAction]
+def make_voc_label_map(task: VocTask = None) -> LabelMapConfig:
+    if task == VocTask.voc_action:
+        label_map = OrderedDict(
+            {
+                VocLabel.background.name: [VocColormap[VocLabel.background.value], [], []],
+                VocLabel.person.name: [
+                    VocColormap[VocLabel.person.value],
+                    [],
+                    [a.name for a in VocAction],
+                ],
+            }
+        )
+    elif task == VocTask.voc_layout:
+        label_map = OrderedDict(
+            {
+                VocLabel.background.name: [VocColormap[VocLabel.background.value], [], []],
+                VocLabel.person.name: [
+                    VocColormap[VocLabel.person.value],
+                    [p.name for p in VocBodyPart],
+                    [],
+                ],
+            }
+        )
+    elif task in [
+        VocTask.voc_classification,
+        VocTask.voc_detection,
+        VocTask.voc_segmentation,
+        VocTask.voc_instance_segmentation,
+    ]:
+        labels = sorted(VocLabel, key=lambda l: l.value)
+        label_map = OrderedDict(
+            (label.name, [VocColormap[label.value], [], []]) for label in labels
+        )
+    else:
+        labels = sorted(VocLabel, key=lambda l: l.value)
+        label_map = OrderedDict(
+            (label.name, [VocColormap[label.value], [], []]) for label in labels
+        )
+        label_map[VocLabel.person.name][1] = [p.name for p in VocBodyPart]
+        label_map[VocLabel.person.name][2] = [a.name for a in VocAction]
+
     return label_map
 
 
 def parse_label_map(path: str) -> LabelMapConfig:
     """
     Parses a label map file in the format:
     'name : color (r, g, b) : parts (hand, feet, ...) : actions (siting, standing, ...)'
@@ -273,29 +313,39 @@
 
     if any(actions):
         dataset_meta["actions"] = actions
 
     dump_json_file(get_meta_file(path), dataset_meta)
 
 
-def make_voc_categories(label_map: Optional[LabelMapConfig] = None) -> CategoriesInfo:
+def make_voc_categories(
+    label_map: Optional[LabelMapConfig] = None, task: Optional[VocTask] = VocTask.voc
+) -> CategoriesInfo:
     if label_map is None:
-        label_map = make_voc_label_map()
+        label_map = make_voc_label_map(task)
 
     categories = {}
 
     label_categories = LabelCategories()
     label_categories.attributes.update(["difficult", "truncated", "occluded"])
 
     for label, desc in label_map.items():
         label_categories.add(label, attributes=desc[2])
-    for part in OrderedDict((k, None) for k in chain(*(desc[1] for desc in label_map.values()))):
-        label_categories.add(part)
+
+    if task in [VocTask.voc, VocTask.voc_layout]:
+        for part in OrderedDict(
+            (k, None) for k in chain(*(desc[1] for desc in label_map.values()))
+        ):
+            label_categories.add(part)
+
     categories[AnnotationType.label] = label_categories
 
+    if task not in [VocTask.voc, VocTask.voc_segmentation, VocTask.voc_instance_segmentation]:
+        return categories
+
     has_colors = any(v[0] is not None for v in label_map.values())
     if not has_colors:  # generate new colors
         colormap = generate_colormap(len(label_map))
     else:  # only copy defined colors
         label_id = lambda label: label_categories.find(label)[0]
         colormap = {
             label_id(name): desc[0] for name, desc in label_map.items() if desc[0] is not None
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/voc/importer.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import Importer
 
 from .format import VocPath, VocTask
 
 
-class VocImporter(Importer):
+class _VocImporter(Importer):
     _TASKS = {
-        VocTask.classification: ("voc_classification", "Main"),
-        VocTask.detection: ("voc_detection", "Main"),
-        VocTask.segmentation: ("voc_segmentation", "Segmentation"),
-        VocTask.person_layout: ("voc_layout", "Layout"),
-        VocTask.action_classification: ("voc_action", "Action"),
+        VocTask.voc: ("voc", "Main"),
+        VocTask.voc_classification: ("voc_classification", "Main"),
+        VocTask.voc_detection: ("voc_detection", "Main"),
+        VocTask.voc_segmentation: ("voc_segmentation", "Segmentation"),
+        VocTask.voc_instance_segmentation: ("voc_instance_segmentation", "Segmentation"),
+        VocTask.voc_layout: ("voc_layout", "Layout"),
+        VocTask.voc_action: ("voc_action", "Action"),
     }
 
     @classmethod
     def detect(cls, context: FormatDetectionContext) -> None:
         # The `voc` format is inherently ambiguous with `voc_classification`,
         # `voc_detection`, etc. To remove the ambiguity (and thus make it
         # possible to use autodetection with the VOC datasets), disable
         # autodetection for the single-task formats.
-        if len(cls._TASKS) == 1:
-            context.raise_unsupported()
 
         with context.require_any():
             task_dirs = {task_dir for _, task_dir in cls._TASKS.values()}
             for task_dir in sorted(task_dirs):
                 with context.alternative():
                     context.require_file(osp.join(VocPath.SUBSETS_DIR, task_dir, "*.txt"))
 
@@ -60,30 +60,40 @@
 
             if not root_path:
                 root_path = osp.dirname(osp.dirname(osp.dirname(task_subsets[0]["url"])))
 
         return subsets
 
 
-class VocClassificationImporter(VocImporter):
-    _TASK = VocTask.classification
-    _TASKS = {_TASK: VocImporter._TASKS[_TASK]}
+class VocImporter(_VocImporter):
+    _TASK = VocTask.voc
+    _TASKS = {_TASK: _VocImporter._TASKS[_TASK]}
 
 
-class VocDetectionImporter(VocImporter):
-    _TASK = VocTask.detection
-    _TASKS = {_TASK: VocImporter._TASKS[_TASK]}
+class VocClassificationImporter(_VocImporter):
+    _TASK = VocTask.voc_classification
+    _TASKS = {_TASK: _VocImporter._TASKS[_TASK]}
 
 
-class VocSegmentationImporter(VocImporter):
-    _TASK = VocTask.segmentation
-    _TASKS = {_TASK: VocImporter._TASKS[_TASK]}
+class VocDetectionImporter(_VocImporter):
+    _TASK = VocTask.voc_detection
+    _TASKS = {_TASK: _VocImporter._TASKS[_TASK]}
 
 
-class VocLayoutImporter(VocImporter):
-    _TASK = VocTask.person_layout
-    _TASKS = {_TASK: VocImporter._TASKS[_TASK]}
+class VocSegmentationImporter(_VocImporter):
+    _TASK = VocTask.voc_segmentation
+    _TASKS = {_TASK: _VocImporter._TASKS[_TASK]}
 
 
-class VocActionImporter(VocImporter):
-    _TASK = VocTask.action_classification
-    _TASKS = {_TASK: VocImporter._TASKS[_TASK]}
+class VocInstanceSegmentationImporter(_VocImporter):
+    _TASK = VocTask.voc_instance_segmentation
+    _TASKS = {_TASK: _VocImporter._TASKS[_TASK]}
+
+
+class VocLayoutImporter(_VocImporter):
+    _TASK = VocTask.voc_layout
+    _TASKS = {_TASK: _VocImporter._TASKS[_TASK]}
+
+
+class VocActionImporter(_VocImporter):
+    _TASK = VocTask.voc_action
+    _TASKS = {_TASK: _VocImporter._TASKS[_TASK]}
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/vott_csv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,43 @@
-# Copyright (C) 2021 Intel Corporation
+# Copyright (C) 2021-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import csv
+import errno
 import os.path as osp
+from typing import Optional
 
 from datumaro.components.annotation import AnnotationType, Bbox, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 
 class VottCsvPath:
     ANNO_FILE_SUFFIX = "-export.csv"
 
 
 class VottCsvBase(SubsetBase):
-    def __init__(self, path):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isfile(path):
-            raise FileNotFoundError("Can't read annotation file '%s'" % path)
+            raise FileNotFoundError(errno.ENOENT, "Can't find annotations file", path)
 
-        super().__init__(subset=osp.splitext(osp.basename(path))[0].rsplit("-", maxsplit=1)[0])
+        if not subset:
+            subset = osp.splitext(osp.basename(path))[0].rsplit("-", maxsplit=1)[0]
+
+        super().__init__(subset=subset, ctx=ctx)
 
         if has_meta_file(path):
             self._categories = {
                 AnnotationType.label: LabelCategories.from_iterable(parse_meta_file(path).keys())
             }
         else:
             self._categories = {AnnotationType.label: LabelCategories()}
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/vott_json.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,43 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import os.path as osp
+from typing import Optional
 
 from datumaro.components.annotation import AnnotationType, Bbox, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import parse_json_file
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 
 class VottJsonPath:
     ANNO_FILE_SUFFIX = "-export.json"
 
 
 class VottJsonBase(SubsetBase):
-    def __init__(self, path):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isfile(path):
-            raise FileNotFoundError("Can't read annotation file '%s'" % path)
+            raise FileNotFoundError(errno.ENOENT, "Can't find annotations file", path)
 
-        super().__init__(subset=osp.splitext(osp.basename(path))[0].rsplit("-", maxsplit=1)[0])
+        if not subset:
+            subset = osp.splitext(osp.basename(path))[0].rsplit("-", maxsplit=1)[0]
+
+        super().__init__(subset=subset, ctx=ctx)
 
         if has_meta_file(path):
             self._categories = {
                 AnnotationType.label: LabelCategories.from_iterable(parse_meta_file(path).keys())
             }
         else:
             self._categories = {AnnotationType.label: LabelCategories()}
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/widerface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# Copyright (C) 2020-2021 Intel Corporation
+# Copyright (C) 2020-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import errno
 import os
 import os.path as osp
 import re
+from typing import Optional
 
 from datumaro.components.annotation import AnnotationType, Bbox, Label, LabelCategories
 from datumaro.components.dataset_base import DatasetItem, SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.exporter import Exporter
 from datumaro.components.format_detection import FormatDetectionContext
-from datumaro.components.importer import Importer
+from datumaro.components.importer import ImportContext, Importer
 from datumaro.components.media import Image
 from datumaro.util import str_to_bool
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 
 class WiderFacePath:
     IMAGE_EXT = ".jpg"
@@ -25,25 +27,32 @@
     LABELS_FILE = "labels.txt"
     IMAGES_DIR_NO_LABEL = "no_label"
     BBOX_ATTRIBUTES = ["blur", "expression", "illumination", "occluded", "pose", "invalid"]
     DEFAULT_LABEL = "face"
 
 
 class WiderFaceBase(SubsetBase):
-    def __init__(self, path, subset=None):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
         if not osp.isfile(path):
-            raise Exception("Can't read annotation file '%s'" % path)
+            raise FileNotFoundError(errno.ENOENT, "Can't find annotations file", path)
         self._path = path
         self._dataset_dir = osp.dirname(osp.dirname(path))
 
         if not subset:
             subset = osp.splitext(osp.basename(path))[0]
             if re.fullmatch(r"wider_face_\S+((_bbx_gt)|(_filelist))", subset):
                 subset = subset.split("_")[2]
-        super().__init__(subset=subset)
+
+        super().__init__(subset=subset, ctx=ctx)
 
         self._categories = self._load_categories()
         self._items = list(self._load_items(path).values())
 
     def _load_categories(self):
         label_cat = LabelCategories()
         if has_meta_file(self._dataset_dir):
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from datumaro.components.annotation import Annotation, AnnotationType, Bbox, LabelCategories
 from datumaro.components.dataset_base import DatasetBase, DatasetItem, SubsetBase
 from datumaro.components.errors import (
     DatasetImportError,
     InvalidAnnotationError,
     UndeclaredLabelError,
 )
+from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image, ImageFromFile
 from datumaro.util.image import (
     DEFAULT_IMAGE_META_FILE_NAME,
     IMAGE_EXTENSIONS,
     ImageMeta,
     load_image_meta_file,
 )
@@ -53,17 +54,19 @@
         def categories(self):
             return self._parent.categories()
 
     def __init__(
         self,
         config_path: str,
         image_info: Union[None, str, ImageMeta] = None,
-        **kwargs,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
     ) -> None:
-        super().__init__(**kwargs)
+        super().__init__(subset=subset, ctx=ctx)
 
         if not osp.isfile(config_path):
             raise DatasetImportError(f"Can't read dataset descriptor file '{config_path}'")
 
         rootpath = osp.dirname(config_path)
         self._path = rootpath
 
@@ -293,17 +296,19 @@
     META_FILE = YoloLoosePath.NAMES_FILE
 
     def __init__(
         self,
         config_path: str,
         image_info: Union[None, str, ImageMeta] = None,
         urls: Optional[List[str]] = None,
-        **kwargs,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
     ) -> None:
-        super().__init__(**kwargs)
+        super().__init__(subset=subset, ctx=ctx)
 
         if not osp.isdir(config_path):
             raise DatasetImportError(f"{config_path} should be a directory.")
 
         rootpath = config_path
         self._path = rootpath
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,17 @@
 
             f.write("names = %s\n" % osp.join(self._prefix, "obj.names"))
             f.write("backup = backup/\n")
 
     def _export_media(self, item: DatasetItem, subset_img_dir: str) -> str:
         try:
             if not item.media or not (item.media.has_data or item.media.has_size):
-                raise Exception("Failed to export item '%s': " "item has no image info" % item.id)
+                raise DatasetExportError(
+                    "Failed to export item '%s': " "item has no image info" % item.id
+                )
 
             image_name = self._make_image_filename(item)
             image_fpath = osp.join(subset_img_dir, image_name)
 
             if self._save_media:
                 self._save_image(item, image_fpath)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.3.0rc1/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/explorer.py` & `datumaro-1.3.0rc1/datumaro/plugins/explorer.py`

 * *Files 13% similar despite different names*

```diff
@@ -58,24 +58,21 @@
         if isinstance(inputs, str):
             if len(inputs.split()) > 1:
                 prompt_text = inputs
             else:
                 prompt_text = f"a photo of a {inputs}"
             inputs = self._tokenize(prompt_text)
             inputs = {self._input_blob: inputs}
-        else:
-            if not inputs.any():
-                # media.data is None case
-                return None
-
+        elif isinstance(inputs, np.ndarray):
             # when processing a query key, we expand HWC to NHWC
             if len(inputs.shape) == 3:
                 inputs = np.expand_dims(inputs, axis=0)
-
             inputs = self.process_inputs(inputs)
+        else:
+            raise ValueError(f"inputs={inputs} is not allowed type.")
 
         results = self._net.infer(inputs)
         hash_key = self._compute_hash(results[self._output_blobs])
         return hash_key
 
     def launch(self, inputs):
         hash_key = self.infer(inputs)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/ndr.py` & `datumaro-1.3.0rc1/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import os.path as osp
+
 import numpy as np
 
 from datumaro.components.annotation import AnnotationType, HashKey, LabelCategories
+from datumaro.util.samples import get_samples_path
 
 
 def normalize(inputs):
     mean = 255 * np.array([0.485, 0.456, 0.406])
     std = 255 * np.array([0.229, 0.224, 0.225])
 
     normalized_inputs = np.empty_like(inputs, dtype=inputs.dtype)
@@ -22,8 +25,16 @@
 def process_outputs(inputs, outputs):
     results = [[HashKey(outputs)]]
     return results
 
 
 def get_categories():
     label_categories = LabelCategories()
+
+    openvino_plugin_samples_dir = get_samples_path()
+    imagenet_class_path = osp.join(openvino_plugin_samples_dir, "imagenet.class")
+    with open(imagenet_class_path, "r", encoding="utf-8") as file:
+        for line in file.readlines():
+            label = line.strip()
+            label_categories.add(label)
+
     return {AnnotationType.label: label_categories}
```

### Comparing `datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_face_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_mobilenet_coco_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_person_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_person_vehicle_bike_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py` & `datumaro-1.3.0rc1/datumaro/plugins/openvino_plugin/samples/ssd_vehicle_detection_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.3.0rc1/datumaro/plugins/sampler/random_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.3.0rc1/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/shift_analyzer.py` & `datumaro-1.3.0rc1/datumaro/plugins/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/splitter.py` & `datumaro-1.3.0rc1/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/synthetic_data/image_generator.py` & `datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.3.0rc1/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.3.0rc1/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/tiling/tile.py` & `datumaro-1.3.0rc1/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/tiling/util.py` & `datumaro-1.3.0rc1/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/plugins/transforms.py` & `datumaro-1.3.0rc1/datumaro/plugins/transforms.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from __future__ import annotations
 
 import argparse
 import logging as log
 import os.path as osp
 import random
 import re
-from collections import Counter
+from collections import Counter, defaultdict
 from copy import deepcopy
 from enum import Enum, auto
 from itertools import chain
 from typing import Dict, Iterable, List, Optional, Tuple, Union
 
 import cv2
 import numpy as np
@@ -36,15 +36,15 @@
     RleMask,
 )
 from datumaro.components.cli_plugin import CliPlugin
 from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME, DatasetInfo, DatasetItem, IDataset
 from datumaro.components.errors import DatumaroError
 from datumaro.components.media import Image
 from datumaro.components.transformer import ItemTransform, Transform
-from datumaro.util import NOTSET, filter_dict, parse_str_enum_value, take_by
+from datumaro.util import NOTSET, filter_dict, parse_json_file, parse_str_enum_value, take_by
 from datumaro.util.annotation_util import find_group_leader, find_instances
 
 
 class CropCoveredSegments(ItemTransform, CliPlugin):
     """
     Sorts polygons and masks ("segments") according to `z_order`,
     crops covered areas of underlying segments. If a segment is split
@@ -1117,41 +1117,61 @@
 
         |s|s%(prog)s --id 'image1:train' --id 'image2:test'
     """
 
     @staticmethod
     def _parse_id(s):
         full_id = s.split(":")
-        if len(full_id) != 2:
+        if len(full_id) == 3:
+            full_id[-1] = int(full_id[-1])
+        if len(full_id) != 2 or len(full_id) != 3:
             raise argparse.ArgumentTypeError(
-                None, message="Invalid id format of '%s'. " "Expected a 'name:subset' pair." % s
+                None,
+                message="Invalid id format of '%s'. "
+                "Expected 'name:subset:ann_id' or 'name:subset' pair." % s,
             )
         return full_id
 
     @classmethod
     def build_cmdline_parser(cls, **kwargs):
         parser = super().build_cmdline_parser(**kwargs)
         parser.add_argument(
             "--id",
             dest="ids",
             type=cls._parse_id,
             action="append",
             help="Image id to clean from annotations. "
-            "Id is 'name:subset' pair. If not specified, removes "
-            "all annotations (repeatable)",
+            "Id is 'name:subset:(optional)ann_id' pair. If ann_id is not specified, "
+            "removes all annotations (repeatable) in the item 'name:subset'",
         )
         return parser
 
-    def __init__(self, extractor: IDataset, *, ids: Optional[Iterable[Tuple[str, str]]] = None):
+    def __init__(self, extractor: IDataset, *, ids: Iterable[Tuple[str, str, Optional[int]]]):
         super().__init__(extractor)
-        self._ids = set(tuple(v) for v in (ids or []))
+
+        self._ids = defaultdict(list)
+        for v in ids:
+            key = tuple(v[:2])
+            val = v[2] if len(v) == 3 else None
+            if val is not None:
+                self._ids[key].append(val)
+            else:
+                self._ids[key] = []
 
     def transform_item(self, item: DatasetItem):
-        if not self._ids or (item.id, item.subset) in self._ids:
-            return item.wrap(annotations=[])
+        if not self._ids:
+            return item
+
+        for item_id, ann_ids in self._ids.items():
+            if (item.id, item.subset) == item_id:
+                updated_anns = (
+                    [ann for ann in item.annotations if ann.id not in ann_ids] if ann_ids else []
+                )
+                return item.wrap(annotations=updated_anns)
+
         return item
 
 
 class RemoveAttributes(ItemTransform):
     """
     Allows to remove item and annotation attributes in a dataset.|n
     |n
@@ -1225,7 +1245,133 @@
             for ann in item.annotations:
                 filtered_annotations.append(ann.wrap(attributes=self._filter_attrs(ann.attributes)))
 
             return item.wrap(
                 attributes=self._filter_attrs(item.attributes), annotations=filtered_annotations
             )
         return item
+
+
+class Correct(Transform, CliPlugin):
+    """
+    Correct the dataset from a validation report.
+    A user can should feed into validation_reports.json from validator to correct the dataset.
+    This helps to refine the dataset by rejecting undefined labels, missing annotations, and outliers.
+    """
+
+    @classmethod
+    def build_cmdline_parser(cls, **kwargs):
+        parser = super().build_cmdline_parser(**kwargs)
+        parser.add_argument(
+            "-r",
+            "--reports",
+            type=str,
+            default="validation_reports.json",
+            help="A validation report from a 'validate' CLI",
+        )
+        return parser
+
+    def __init__(
+        self,
+        extractor: IDataset,
+        reports: Union[str, Dict],
+    ):
+        super().__init__(extractor)
+
+        if isinstance(reports, str):
+            reports = parse_json_file(reports)
+
+        self._reports = reports["validation_reports"]
+
+        self._categories = self._extractor.categories()
+
+        self._remove_items = set()
+        self._remove_anns = defaultdict(list)
+        self._add_attrs = defaultdict(list)
+
+        self._analyze_reports(report=self._reports)
+
+    def categories(self):
+        return self._categories
+
+    def _parse_ann_ids(self, desc: str):
+        return [int(s) for s in str.split(desc, "'") if s.isdigit()][0]
+
+    def _analyze_reports(self, report):
+        for rep in report:
+            if rep["anomaly_type"] == "MissingLabelCategories":
+                unique_labels = sorted(
+                    list({ann.label for item in self._extractor for ann in item.annotations})
+                )
+                label_categories = LabelCategories().from_iterable(
+                    [str(label) for label in unique_labels]
+                )
+                for item in self._extractor:
+                    for ann in item.annotations:
+                        attrs = {attr for attr in ann.attributes}
+                        label_categories[ann.label].attributes.update(attrs)
+                self._categories[AnnotationType.label] = label_categories
+
+            if rep["anomaly_type"] == "UndefinedLabel":
+                label_categories = self._categories[AnnotationType.label]
+                desc = [s for s in rep["description"].split("'")]
+                add_label_name = desc[1]
+                label_id, _ = label_categories.find(add_label_name)
+                if label_id is None:
+                    label_categories.add(name=add_label_name)
+
+            if rep["anomaly_type"] == "UndefinedAttribute":
+                label_categories = self._categories[AnnotationType.label]
+                desc = [s for s in rep["description"].split("'")]
+                attr_name, label_name = desc[1], desc[3]
+                label_id = label_categories.find(label_name)[0]
+                if label_id is not None:
+                    label_categories[label_id].attributes.add(attr_name)
+
+            # [TODO] Correct LabeleDefinedButNotFound: removing a label, reindexing, remapping others
+            # if rep["anomaly_type"] == "LabelDefinedButNotFound":
+            #     remove_label_name = self._parse_label_cat(rep["description"])
+            #     label_cat = self._extractor.categories()[AnnotationType.label]
+            #     if remove_label_name in [labels.name for labels in label_cat.items]:
+            #         label_cat.remove(remove_label_name)
+
+            if rep["anomaly_type"] in ["MissingAnnotation", "MultiLabelAnnotations"]:
+                self._remove_items.add((rep["item_id"], rep["subset"]))
+
+            if rep["anomaly_type"] in [
+                "NegativeLength",
+                "InvalidValue",
+                "FarFromLabelMean",
+                "FarFromAttrMean",
+            ]:
+                ann_id = None or self._parse_ann_ids(rep["description"])
+                self._remove_anns[(rep["item_id"], rep["subset"])].append(ann_id)
+
+            if rep["anomaly_type"] == "MissingAttribute":
+                desc = [s for s in str.split(rep["description"], "'")]
+                attr_name, label_name = desc[1], desc[3]
+                label_id = self._extractor.categories()[AnnotationType.label].find(label_name)[0]
+                self._add_attrs[(rep["item_id"], rep["subset"])].append((label_id, attr_name))
+
+    def __iter__(self):
+        for item in self._extractor:
+            if (item.id, item.subset) in self._remove_items:
+                continue
+
+            ann_ids = self._remove_anns.get((item.id, item.subset), None)
+            if ann_ids:
+                updated_anns = [ann for ann in item.annotations if ann.id not in ann_ids]
+                yield item.wrap(annotations=updated_anns)
+            else:
+                updated_attrs = defaultdict(list)
+                for label_id, attr_name in self._add_attrs.get((item.id, item.subset), []):
+                    updated_attrs[label_id].append(attr_name)
+
+                updated_anns = []
+                for ann in item.annotations:
+                    new_ann = ann.wrap(attributes=deepcopy(ann.attributes))
+                    if ann.label in updated_attrs:
+                        new_ann.attributes.update(
+                            {attr_name: "" for attr_name in updated_attrs[ann.label]}
+                        )
+                    updated_anns.append(new_ann)
+                yield item.wrap(annotations=updated_anns)
```

### Comparing `datumaro-1.2.1/datumaro/plugins/validators.py` & `datumaro-1.3.0rc1/datumaro/plugins/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -415,27 +415,27 @@
         count_by_defined_labels = stats["label_distribution"]["defined_labels"]
         labels_found = [
             label_name for label_name, count in count_by_defined_labels.items() if count > 0
         ]
 
         if len(labels_found) == 1:
             validation_reports += self._generate_validation_report(
-                OnlyOneLabel, Severity.warning, labels_found[0]
+                OnlyOneLabel, Severity.info, labels_found[0]
             )
 
         return validation_reports
 
     def _check_only_one_attribute(self, label_name, attr_name, attr_dets):
         validation_reports = []
         values = list(attr_dets["distribution"].keys())
 
         if len(values) == 1:
             details = (label_name, attr_name, values[0])
             validation_reports += self._generate_validation_report(
-                OnlyOneAttributeValue, Severity.warning, *details
+                OnlyOneAttributeValue, Severity.info, *details
             )
 
         return validation_reports
 
     def _check_few_samples_in_label(self, stats):
         validation_reports = []
         thr = self.few_samples_thr
@@ -445,15 +445,15 @@
             (label_name, count)
             for label_name, count in defined_label_dist.items()
             if 0 < count <= thr
         ]
 
         for label_name, count in labels_with_few_samples:
             validation_reports += self._generate_validation_report(
-                FewSamplesInLabel, Severity.warning, label_name, count
+                FewSamplesInLabel, Severity.info, label_name, count
             )
 
         return validation_reports
 
     def _check_few_samples_in_attribute(self, label_name, attr_name, attr_dets):
         validation_reports = []
         thr = self.few_samples_thr
@@ -463,15 +463,15 @@
             for attr_value, count in attr_dets["distribution"].items()
             if count <= thr
         ]
 
         for attr_value, count in attr_values_with_few_samples:
             details = (label_name, attr_name, attr_value, count)
             validation_reports += self._generate_validation_report(
-                FewSamplesInAttribute, Severity.warning, *details
+                FewSamplesInAttribute, Severity.info, *details
             )
 
         return validation_reports
 
     def _check_imbalanced_labels(self, stats):
         validation_reports = []
         thr = self.imbalance_ratio_thr
@@ -482,17 +482,15 @@
         if len(count_by_defined_labels) == 0:
             return validation_reports
 
         count_max = np.max(count_by_defined_labels)
         count_min = np.min(count_by_defined_labels)
         balance = count_max / count_min if count_min > 0 else float("inf")
         if balance >= thr:
-            validation_reports += self._generate_validation_report(
-                ImbalancedLabels, Severity.warning
-            )
+            validation_reports += self._generate_validation_report(ImbalancedLabels, Severity.info)
 
         return validation_reports
 
     def _check_imbalanced_attribute(self, label_name, attr_name, attr_dets):
         validation_reports = []
         thr = self.imbalance_ratio_thr
 
@@ -501,15 +499,15 @@
             return validation_reports
 
         count_max = np.max(count_by_defined_attr)
         count_min = np.min(count_by_defined_attr)
         balance = count_max / count_min if count_min > 0 else float("inf")
         if balance >= thr:
             validation_reports += self._generate_validation_report(
-                ImbalancedAttribute, Severity.warning, label_name, attr_name
+                ImbalancedAttribute, Severity.info, label_name, attr_name
             )
 
         return validation_reports
 
 
 class ClassificationValidator(_TaskValidator):
     """
@@ -911,15 +909,15 @@
 
             if topk > 0:
                 topk_values = np.sort(value_counts)[-topk:]
                 ratio = np.sum(topk_values) / np.sum(value_counts)
                 if ratio >= thr:
                     details = (label_name, f"{self.str_ann_type} {prop}")
                     validation_reports += self._generate_validation_report(
-                        ImbalancedDistInLabel, Severity.warning, *details
+                        ImbalancedDistInLabel, Severity.info, *details
                     )
 
         return validation_reports
 
     def _check_imbalanced_dist_in_attr(self, label_name, attr_name, attr_stats):
         validation_reports = []
         thr = self.dominance_thr
@@ -935,15 +933,15 @@
 
                 if topk > 0:
                     topk_values = np.sort(value_counts)[-topk:]
                     ratio = np.sum(topk_values) / np.sum(value_counts)
                     if ratio >= thr:
                         details = (label_name, attr_name, attr_value, f"{self.str_ann_type} {prop}")
                         validation_reports += self._generate_validation_report(
-                            ImbalancedDistInAttribute, Severity.warning, *details
+                            ImbalancedDistInAttribute, Severity.info, *details
                         )
 
         return validation_reports
 
     def _check_far_from_label_mean(self, label_name, label_stats):
         validation_reports = []
```

### Comparing `datumaro-1.2.1/datumaro/util/__init__.py` & `datumaro-1.3.0rc1/datumaro/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/util/annotation_util.py` & `datumaro-1.3.0rc1/datumaro/util/annotation_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,16 @@
 
 
 def _get_bbox(ann: Union[Sequence, SpatialAnnotation]) -> BboxCoords:
     if isinstance(ann, (_Shape, Mask)):
         return ann.get_bbox()
     elif hasattr(ann, "__len__") and len(ann) == 4:
         return ann
+    elif hasattr(ann, "__len__") and len(ann) == 0:
+        return [0, 0, 0, 0]
     else:
         raise ValueError("The value of type '%s' can't be treated as a " "bounding box" % type(ann))
 
 
 def max_bbox(annotations: Iterable[Union[BboxCoords, SpatialAnnotation]]) -> BboxCoords:
     """
     Computes the maximum bbox for the set of spatial annotations and boxes.
```

### Comparing `datumaro-1.2.1/datumaro/util/attrs_util.py` & `datumaro-1.3.0rc1/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/util/file_utils.py` & `datumaro-1.3.0rc1/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/util/image.py` & `datumaro-1.3.0rc1/datumaro/util/image.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/util/image_cache.py` & `datumaro-1.3.0rc1/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/util/log_utils.py` & `datumaro-1.3.0rc1/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/util/mask_tools.py` & `datumaro-1.3.0rc1/datumaro/util/mask_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         assert mask.shape[2] == 1
 
 
 _default_colormap = generate_colormap()
 _default_unpaint_colormap = invert_colormap(_default_colormap)
 
 
-def unpaint_mask(painted_mask, inverse_colormap=None):
+def unpaint_mask(painted_mask, inverse_colormap=None, default_id=None):
     """
     Convert color mask to index mask
 
     mask: HWC BGR [0; 255]
 
     colormap: (R, G, B) -> index
     """
@@ -74,16 +74,18 @@
     painted_mask = (
         painted_mask[:, :, 0] + (painted_mask[:, :, 1] << 8) + (painted_mask[:, :, 2] << 16)
     )
     uvals, unpainted_mask = np.unique(painted_mask, return_inverse=True)
     palette = []
     for v in uvals:
         class_id = map_fn(v)
-        if class_id is None:
+        if class_id is None and default_id is None:
             raise KeyError(f"Undeclared color {((v >> 16) & 255, (v >> 8) & 255, v & 255)}")
+        elif class_id is None and default_id is not None:
+            class_id = default_id
         palette.append(class_id)
     palette = np.array(palette, dtype=np.min_scalar_type(len(uvals)))
     unpainted_mask = palette[unpainted_mask].reshape(painted_mask.shape[:2])
 
     return unpainted_mask
 
 
@@ -137,19 +139,19 @@
     return (img[..., 0] << 16) + (img[..., 1] << 8) + img[..., 2]
 
 
 def index2bgr(id_map):
     return np.dstack((id_map >> 16, id_map >> 8, id_map)).astype(np.uint8)
 
 
-def load_mask(path, inverse_colormap=None):
+def load_mask(path, inverse_colormap=None, default_id=None):
     mask = load_image(path, dtype=np.uint8)
     if inverse_colormap is not None:
         if len(mask.shape) == 3 and mask.shape[2] != 1:
-            mask = unpaint_mask(mask, inverse_colormap)
+            mask = unpaint_mask(mask, inverse_colormap, default_id)
     return mask
 
 
 def lazy_mask(path, inverse_colormap=None):
     return lazy_image(path, partial(load_mask, inverse_colormap=inverse_colormap))
```

### Comparing `datumaro-1.2.1/datumaro/util/meta_file_util.py` & `datumaro-1.3.0rc1/datumaro/util/meta_file_util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,45 @@
-# Copyright (C) 2022 Intel Corporation
+# Copyright (C) 2022-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import os
 import os.path as osp
 from collections import OrderedDict
 
-from datumaro.components.annotation import AnnotationType
+from datumaro.components.annotation import AnnotationType, HashKey
 from datumaro.util import dump_json_file, find, parse_json_file
 
 DATASET_META_FILE = "dataset_meta.json"
+DATASET_HASHKEY_FILE = "hash_keys.json"
 
 
 def is_meta_file(path):
     return osp.splitext(osp.basename(path))[1] == ".json"
 
 
 def has_meta_file(path):
     return osp.isfile(get_meta_file(path))
 
 
+def has_hashkey_file(path):
+    return osp.isfile(get_hashkey_file(path))
+
+
 def get_meta_file(path):
     return osp.join(path, DATASET_META_FILE)
 
 
+def get_hashkey_file(path):
+    hashkey_folder_path = osp.join(path, "hash_key_meta")
+    if not osp.exists(hashkey_folder_path):
+        os.makedirs(hashkey_folder_path)
+    return osp.join(hashkey_folder_path, DATASET_HASHKEY_FILE)
+
+
 def parse_meta_file(path):
     meta_file = path
     if osp.isdir(path):
         meta_file = get_meta_file(path)
 
     dataset_meta = parse_json_file(meta_file)
 
@@ -68,7 +81,48 @@
             dataset_meta["background_label"] = str(bg_label[0])
 
     meta_file = path
     if osp.isdir(path):
         meta_file = get_meta_file(path)
 
     dump_json_file(meta_file, dataset_meta, indent=True)
+
+
+def parse_hashkey_file(path):
+    meta_file = path
+    if osp.isdir(path):
+        meta_file = get_hashkey_file(path)
+
+    if not osp.exists(meta_file):
+        return None
+
+    dataset_meta = parse_json_file(meta_file)
+
+    hashkey_dict = OrderedDict()
+    for id_, hashkey in dataset_meta.get("hashkey", {}).items():
+        hashkey_dict[id_] = hashkey
+
+    return hashkey_dict
+
+
+def save_hashkey_file(path, item_list):
+    dataset_hashkey = {}
+
+    if osp.isdir(path):
+        meta_file = get_hashkey_file(path)
+
+    hashkey_dict = parse_hashkey_file(path)
+    if not hashkey_dict:
+        hashkey_dict = {}
+
+    for item in item_list:
+        item_id = item.id
+        item_subset = item.subset
+        for annotation in item.annotations:
+            if isinstance(annotation, HashKey):
+                hashkey = annotation.hash_key
+                break
+        hashkey_dict.update({item_subset + "/" + item_id: hashkey.tolist()})
+
+    dataset_hashkey["hashkey"] = hashkey_dict
+
+    dump_json_file(meta_file, dataset_hashkey, indent=True)
```

### Comparing `datumaro-1.2.1/datumaro/util/os_util.py` & `datumaro-1.3.0rc1/datumaro/util/os_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/util/pickle_util.py` & `datumaro-1.3.0rc1/datumaro/util/pickle_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/util/scope.py` & `datumaro-1.3.0rc1/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/util/telemetry_stub.py` & `datumaro-1.3.0rc1/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/util/telemetry_utils.py` & `datumaro-1.3.0rc1/datumaro/util/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro/util/tf_util.py` & `datumaro-1.3.0rc1/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/datumaro.egg-info/PKG-INFO` & `datumaro-1.3.0rc1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: datumaro
-Version: 1.2.1
-Summary: Dataset Management Framework (Datumaro)
-Home-page: https://github.com/openvinotoolkit/datumaro
-Author: Intel
-Author-email: emily.chun@intel.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: tf
-Provides-Extra: tfds
-Provides-Extra: tfds-dev
-Provides-Extra: tf-gpu
-Provides-Extra: default
-License-File: LICENSE
-License-File: NOTICE
-
 # Dataset Management Framework (Datumaro)
 
 [![Build status](https://github.com/openvinotoolkit/datumaro/actions/workflows/health_check.yml/badge.svg)](https://github.com/openvinotoolkit/datumaro/actions/workflows/health_check.yml)
 [![codecov](https://codecov.io/gh/openvinotoolkit/datumaro/branch/develop/graph/badge.svg?token=FG25VU096Q)](https://codecov.io/gh/openvinotoolkit/datumaro)
 
 A framework and CLI tool to build, transform, and analyze datasets.
 
@@ -31,18 +11,19 @@
      +                                     /
 COCO dataset -----> Datumaro ---> dataset ------> Model training
      +                                     \
 CVAT annotations                             ---> Publication, statistics etc.
 ```
 <!--lint enable fenced-code-flag-->
 
-- [Getting started](https://openvinotoolkit.github.io/datumaro/docs/getting_started)
+- [Getting started](https://openvinotoolkit.github.io/datumaro/latest/docs/get-started/quick-start-guide)
+- [Level Up](https://openvinotoolkit.github.io/datumaro/latest/docs/level-up/basic_skills)
 - [Features](#features)
-- [User manual](https://openvinotoolkit.github.io/datumaro/docs/user-manual)
-- [Developer manual](https://openvinotoolkit.github.io/datumaro/api)
+- [User manual](https://openvinotoolkit.github.io/datumaro/latest/docs/user-manual/how_to_use_datumaro)
+- [Developer manual](https://openvinotoolkit.github.io/datumaro/latest/docs/reference/datumaro/datumaro)
 - [Contributing](#contributing)
 
 ## Features
 
 [(Back to top)](#dataset-management-framework-datumaro)
 
 - Dataset reading, writing, conversion in any direction.
@@ -61,15 +42,15 @@
   - [Open Images](https://storage.googleapis.com/openimages/web/download.html)
   - [PASCAL VOC](http://host.robots.ox.ac.uk/pascal/VOC/voc2012/htmldoc/index.html)
     (`classification`, `detection`, `segmentation`, `action_classification`, `person_layout`)
   - [TF Detection API](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/using_your_own_dataset.md)
     (`bboxes`, `masks`)
   - [YOLO](https://github.com/AlexeyAB/darknet#how-to-train-pascal-voc-data) (`bboxes`)
 
-  Other formats and documentation for them can be found [here](https://openvinotoolkit.github.io/datumaro/docs/user-manual/supported_formats).
+  Other formats and documentation for them can be found [here](https://openvinotoolkit.github.io/datumaro/latest/docs/data-formats/supported_formats).
 - Dataset building
   - Merging multiple datasets into one
   - Dataset filtering by a custom criteria:
     - remove polygons of a certain class
     - remove images without annotations of a specific class
     - remove `occluded` annotations from images
     - keep only vertically-oriented images
@@ -101,30 +82,30 @@
 - Model integration
   - Inference (OpenVINO, Caffe, PyTorch, TensorFlow, MxNet, etc.)
   - Explainable AI ([RISE algorithm](https://arxiv.org/abs/1806.07421))
     - RISE for classification
     - RISE for object detection
 
 > Check
-  [the design document](https://openvinotoolkit.github.io/datumaro/docs/design)
+  [the design document](https://openvinotoolkit.github.io/datumaro/latest/docs/explanation/architecture)
   for a full list of features.
 > Check
-  [the user manual](https://openvinotoolkit.github.io/datumaro/docs/user-manual)
+  [the user manual](https://openvinotoolkit.github.io/datumaro/latest/docs/user-manual/how_to_use_datumaro)
   for usage instructions.
 
 ## Contributing
 
 [(Back to top)](#dataset-management-framework-datumaro)
 
 Feel free to
 [open an Issue](https://github.com/openvinotoolkit/datumaro/issues/new), if you
 think something needs to be changed. You are welcome to participate in
 development, instructions are available in our
-[contribution guide](https://openvinotoolkit.github.io/datumaro/docs/contributing).
+[contribution guide](https://github.com/openvinotoolkit/datumaro/blob/develop/contributing.md).
 
 ## Telemetry data collection note
 
 The [OpenVINO™ telemetry library](https://github.com/openvinotoolkit/telemetry/)
 is used to collect basic information about Datumaro usage.
 
 To enable/disable telemetry data collection please see the
-[guide](https://openvinotoolkit.github.io/datumaro/docs/user-manual/how_to_control_tm_data_collection/).
+[guide](https://openvinotoolkit.github.io/datumaro/latest/docs/user-manual/how_to_control_tm_data_collection).
```

### Comparing `datumaro-1.2.1/datumaro.egg-info/SOURCES.txt` & `datumaro-1.3.0rc1/datumaro.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,14 @@
 datumaro/plugins/data_formats/mars.py
 datumaro/plugins/data_formats/mnist.py
 datumaro/plugins/data_formats/mnist_csv.py
 datumaro/plugins/data_formats/mot.py
 datumaro/plugins/data_formats/mots.py
 datumaro/plugins/data_formats/nyu_depth_v2.py
 datumaro/plugins/data_formats/open_images.py
-datumaro/plugins/data_formats/synthia.py
 datumaro/plugins/data_formats/vgg_face2.py
 datumaro/plugins/data_formats/video.py
 datumaro/plugins/data_formats/vott_csv.py
 datumaro/plugins/data_formats/vott_json.py
 datumaro/plugins/data_formats/widerface.py
 datumaro/plugins/data_formats/arrow/__init__.py
 datumaro/plugins/data_formats/arrow/arrow_dataset.py
@@ -207,18 +206,26 @@
 datumaro/plugins/data_formats/mpii/mpii_json.py
 datumaro/plugins/data_formats/mpii/mpii_mat.py
 datumaro/plugins/data_formats/mvtec/__init__.py
 datumaro/plugins/data_formats/mvtec/base.py
 datumaro/plugins/data_formats/mvtec/exporter.py
 datumaro/plugins/data_formats/mvtec/format.py
 datumaro/plugins/data_formats/mvtec/importer.py
+datumaro/plugins/data_formats/segment_anything/__init__.py
+datumaro/plugins/data_formats/segment_anything/base.py
+datumaro/plugins/data_formats/segment_anything/exporter.py
+datumaro/plugins/data_formats/segment_anything/importer.py
 datumaro/plugins/data_formats/sly_pointcloud/__init__.py
 datumaro/plugins/data_formats/sly_pointcloud/base.py
 datumaro/plugins/data_formats/sly_pointcloud/exporter.py
 datumaro/plugins/data_formats/sly_pointcloud/format.py
+datumaro/plugins/data_formats/synthia/__init__.py
+datumaro/plugins/data_formats/synthia/base.py
+datumaro/plugins/data_formats/synthia/format.py
+datumaro/plugins/data_formats/synthia/importer.py
 datumaro/plugins/data_formats/tf_detection_api/__init__.py
 datumaro/plugins/data_formats/tf_detection_api/base.py
 datumaro/plugins/data_formats/tf_detection_api/exporter.py
 datumaro/plugins/data_formats/tf_detection_api/format.py
 datumaro/plugins/data_formats/voc/__init__.py
 datumaro/plugins/data_formats/voc/base.py
 datumaro/plugins/data_formats/voc/exporter.py
```

### Comparing `datumaro-1.2.1/datumaro.egg-info/requires.txt` & `datumaro-1.3.0rc1/datumaro.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 requests
 pandas>=1.1.5
 openvino==2022.3.0
 tokenizers
 cryptography>=38.03
 pyemd
 pyarrow
+protobuf
 opencv-python
 
 [:platform_system != "Windows" or python_version >= "3.9"]
 pycocotools>=2.0.4
 
 [:platform_system == "Windows" and python_version < "3.9"]
 pycocotools-windows
@@ -42,10 +43,7 @@
 tensorflow
 
 [tf-gpu]
 tensorflow-gpu
 
 [tfds]
 tensorflow-datasets<4.9.0
-
-[tfds-dev]
-tensorflow-datasets[dev]<4.9.0
```

### Comparing `datumaro-1.2.1/pyproject.toml` & `datumaro-1.3.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datumaro-1.2.1/requirements-core.txt` & `datumaro-1.3.0rc1/requirements-core.txt`

 * *Files 4% similar despite different names*

```diff
@@ -40,7 +40,10 @@
 cryptography>= 38.03
 
 # Shift analyzer
 pyemd
 
 # apache arrow
 pyarrow
+
+# ava data format
+protobuf
```

### Comparing `datumaro-1.2.1/setup.py` & `datumaro-1.3.0rc1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,17 +84,14 @@
     python_requires=">=3.7",
     install_requires=CORE_REQUIREMENTS,
     extras_require={
         "tf": ["tensorflow"],
         "tfds": [
             "tensorflow-datasets<4.9.0"
         ],  # 4.9.0 fails on Windows and MacOS, https://github.com/openvinotoolkit/datumaro/actions/runs/4618774184
-        "tfds-dev": [
-            "tensorflow-datasets[dev]<4.9.0"
-        ],  # 4.9.0 fails on Windows and MacOS, https://github.com/openvinotoolkit/datumaro/actions/runs/4618774184
         "tf-gpu": ["tensorflow-gpu"],
         "default": DEFAULT_REQUIREMENTS,
     },
     ext_modules=ext_modules,
     entry_points={
         "console_scripts": [
             "datum=datumaro.cli.__main__:main",
```

