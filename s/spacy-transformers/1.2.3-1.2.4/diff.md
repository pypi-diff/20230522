# Comparing `tmp/spacy-transformers-1.2.3.tar.gz` & `tmp/spacy-transformers-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacy-transformers-1.2.3.tar", last modified: Mon Apr 17 12:38:13 2023, max compression
+gzip compressed data, was "spacy-transformers-1.2.4.tar", last modified: Mon May 22 15:30:04 2023, max compression
```

## Comparing `spacy-transformers-1.2.3.tar` & `spacy-transformers-1.2.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 12:38:13.278227 spacy-transformers-1.2.3/
--rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     5491 2023-04-17 12:38:13.278227 spacy-transformers-1.2.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     4073 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      129 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     3067 2023-04-17 12:38:13.278227 spacy-transformers-1.2.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     2214 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 12:38:13.270227 spacy-transformers-1.2.3/spacy_transformers/
--rw-r--r--   0 vsts      (1001) docker     (122)      499 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      692 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/align.pyi
--rw-r--r--   0 vsts      (1001) docker     (122)     9887 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/align.pyx
--rw-r--r--   0 vsts      (1001) docker     (122)      597 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/annotation_setters.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11525 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/architectures.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14828 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/data_classes.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 12:38:13.274227 spacy-transformers-1.2.3/spacy_transformers/layers/
--rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      663 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/_util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4871 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/hf_shim.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2563 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/hf_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2999 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/listener.py
--rw-r--r--   0 vsts      (1001) docker     (122)      427 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/split_trf.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11549 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/transformer_model.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6448 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/layers/trfs2arrays.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17118 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/pipeline_component.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/py.typed
--rw-r--r--   0 vsts      (1001) docker     (122)     2449 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/span_getters.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 12:38:13.278227 spacy-transformers-1.2.3/spacy_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 12:38:13.278227 spacy-transformers-1.2.3/spacy_transformers/tests/regression/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/regression/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2017 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/regression/test_spacy_issue6401.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1830 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/regression/test_spacy_issue7029.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3175 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_alignment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2057 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_configs.py
--rw-r--r--   0 vsts      (1001) docker     (122)      834 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_data_classes.py
--rw-r--r--   0 vsts      (1001) docker     (122)      440 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_deprecations.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5442 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_model_sequence_classification.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3359 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_model_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16846 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_pipeline_component.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9837 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_serialize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2288 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_spanners.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1588 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_textcatcnn.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3132 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_tok2vectransformer.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4054 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/test_truncation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/tests/util.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4636 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/truncate.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5440 2023-04-17 12:35:54.000000 spacy-transformers-1.2.3/spacy_transformers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-17 12:38:13.270227 spacy-transformers-1.2.3/spacy_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     5491 2023-04-17 12:38:13.000000 spacy-transformers-1.2.3/spacy_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1876 2023-04-17 12:38:13.000000 spacy-transformers-1.2.3/spacy_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-17 12:38:13.000000 spacy-transformers-1.2.3/spacy_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      819 2023-04-17 12:38:13.000000 spacy-transformers-1.2.3/spacy_transformers.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-17 12:38:13.000000 spacy-transformers-1.2.3/spacy_transformers.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      519 2023-04-17 12:38:13.000000 spacy-transformers-1.2.3/spacy_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-04-17 12:38:13.000000 spacy-transformers-1.2.3/spacy_transformers.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 15:30:04.553306 spacy-transformers-1.2.4/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1073 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      191 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     6089 2023-05-22 15:30:04.553306 spacy-transformers-1.2.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     4671 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      129 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     3067 2023-05-22 15:30:04.557306 spacy-transformers-1.2.4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     2214 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 15:30:04.549306 spacy-transformers-1.2.4/spacy_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      499 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      692 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/align.pyi
+-rw-r--r--   0 vsts      (1001) docker     (122)     9887 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/align.pyx
+-rw-r--r--   0 vsts      (1001) docker     (122)      597 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/annotation_setters.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11525 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/architectures.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14828 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/data_classes.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 15:30:04.549306 spacy-transformers-1.2.4/spacy_transformers/layers/
+-rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      663 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/_util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4871 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/hf_shim.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2563 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/hf_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2999 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/listener.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      427 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/split_trf.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11549 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/transformer_model.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6448 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/layers/trfs2arrays.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17118 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/pipeline_component.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/py.typed
+-rw-r--r--   0 vsts      (1001) docker     (122)     2449 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/span_getters.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 15:30:04.553306 spacy-transformers-1.2.4/spacy_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       45 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 15:30:04.553306 spacy-transformers-1.2.4/spacy_transformers/tests/regression/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/regression/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2017 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/regression/test_spacy_issue6401.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1830 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/regression/test_spacy_issue7029.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3175 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_alignment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2057 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_configs.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      834 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_data_classes.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      440 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_deprecations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5442 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_model_sequence_classification.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3359 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_model_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16846 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_pipeline_component.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9837 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_serialize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2288 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_spanners.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1588 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_textcatcnn.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3132 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_tok2vectransformer.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4054 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/test_truncation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5727 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/tests/util.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4636 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/truncate.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5440 2023-05-22 15:29:48.000000 spacy-transformers-1.2.4/spacy_transformers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-22 15:30:04.549306 spacy-transformers-1.2.4/spacy_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6089 2023-05-22 15:30:04.000000 spacy-transformers-1.2.4/spacy_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1876 2023-05-22 15:30:04.000000 spacy-transformers-1.2.4/spacy_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 15:30:04.000000 spacy-transformers-1.2.4/spacy_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      819 2023-05-22 15:30:04.000000 spacy-transformers-1.2.4/spacy_transformers.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-22 15:30:04.000000 spacy-transformers-1.2.4/spacy_transformers.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      519 2023-05-22 15:30:04.000000 spacy-transformers-1.2.4/spacy_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       19 2023-05-22 15:30:04.000000 spacy-transformers-1.2.4/spacy_transformers.egg-info/top_level.txt
```

### Comparing `spacy-transformers-1.2.3/LICENSE` & `spacy-transformers-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/PKG-INFO` & `spacy-transformers-1.2.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-transformers
-Version: 1.2.3
+Version: 1.2.4
 Summary: spaCy pipelines for pre-trained BERT and other transformers
 Home-page: https://spacy.io
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -44,19 +44,19 @@
 
 This package provides [spaCy](https://github.com/explosion/spaCy) components and
 architectures to use transformer models via
 [Hugging Face's `transformers`](https://github.com/huggingface/transformers) in
 spaCy. The result is convenient access to state-of-the-art transformer
 architectures, such as BERT, GPT-2, XLNet, etc.
 
-> **This release requires [spaCy v3](https://spacy.io/usage/v3).** For
-> the previous version of this library, see the
+> **This release requires [spaCy v3](https://spacy.io/usage/v3).** For the
+> previous version of this library, see the
 > [`v0.6.x` branch](https://github.com/explosion/spacy-transformers/tree/v0.6.x).
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/18/master.svg?logo=azure-pipelines&style=flat-square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=18)
+[![tests](https://github.com/explosion/spacy-transformers/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/spacy-transformers/actions/workflows/tests.yml)
 [![PyPi](https://img.shields.io/pypi/v/spacy-transformers.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/spacy-transformers)
 [![GitHub](https://img.shields.io/github/release/explosion/spacy-transformers/all.svg?style=flat-square&logo=github)](https://github.com/explosion/spacy-transformers/releases)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 ## Features
 
 - Use pretrained transformer models like **BERT**, **RoBERTa** and **XLNet** to
@@ -83,40 +83,50 @@
 For GPU installation, find your CUDA version using `nvcc --version` and add the
 [version in brackets](https://spacy.io/usage/#gpu), e.g.
 `spacy[transformers,cuda92]` for CUDA9.2 or `spacy[transformers,cuda100]` for
 CUDA10.0.
 
 If you are having trouble installing PyTorch, follow the
 [instructions](https://pytorch.org/get-started/locally/) on the official website
-for your specific operating system and requirements, or try the following:
-
-```bash
-pip install spacy-transformers -f https://download.pytorch.org/whl/torch_stable.html
-```
+for your specific operating system and requirements.
 
 ## 📖 Documentation
 
 > ⚠️ **Important note:** This package has been extensively refactored to take
-> advantage of [spaCy v3.0](https://spacy.io). Previous versions that
-> were built for [spaCy v2.x](https://v2.spacy.io) worked considerably
-> differently. Please see previous tagged versions of this README for
-> documentation on prior versions.
+> advantage of [spaCy v3.0](https://spacy.io). Previous versions that were built
+> for [spaCy v2.x](https://v2.spacy.io) worked considerably differently. Please
+> see previous tagged versions of this README for documentation on prior
+> versions.
 
 - 📘
   [Embeddings, Transformers and Transfer Learning](https://spacy.io/usage/embeddings-transformers):
   How to use transformers in spaCy
-- 📘 [Training Pipelines and Models](https://spacy.io/usage/training):
-  Train and update components on your own data and integrate custom models
+- 📘 [Training Pipelines and Models](https://spacy.io/usage/training): Train and
+  update components on your own data and integrate custom models
 - 📘
   [Layers and Model Architectures](https://spacy.io/usage/layers-architectures):
   Power spaCy components with custom neural networks
-- 📗 [`Transformer`](https://spacy.io/api/transformer): Pipeline
-  component API reference
+- 📗 [`Transformer`](https://spacy.io/api/transformer): Pipeline component API
+  reference
 - 📗
   [Transformer architectures](https://spacy.io/api/architectures#transformers):
   Architectures and registered functions
 
+## Applying pretrained text and token classification models
+
+Note that the `transformer` component from `spacy-transformers` does not support
+task-specific heads like token or text classification. A task-specific
+transformer model can be used as a source of features to train spaCy components
+like `ner` or `textcat`, but the `transformer` component does not provide access
+to task-specific heads for training or inference.
+
+Alternatively, if you only want use to the **predictions** from an existing
+Hugging Face text or token classification model, you can use the wrappers from
+[`spacy-huggingface-pipelines`](https://github.com/explosion/spacy-huggingface-pipelines)
+to incorporate task-specific transformer models into your spaCy pipelines.
+
 ## Bug reports and other issues
 
-Please use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues) to report a bug, or open a new thread on the
-[discussion board](https://github.com/explosion/spaCy/discussions)
-for any other issue.
+Please use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues) to
+report a bug, or open a new thread on the
+[discussion board](https://github.com/explosion/spaCy/discussions) for any other
+issue.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-transformers Version: 1.2.3 Summary: spaCy
+Metadata-Version: 2.1 Name: spacy-transformers Version: 1.2.4 Summary: spaCy
 pipelines for pre-trained BERT and other transformers Home-page: https://
 spacy.io Author: Explosion Author-email: contact@explosion.ai License: MIT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
@@ -19,53 +19,61 @@
 Provides-Extra: cuda112 License-File: LICENSE [https://explosion.ai/assets/img/
 logo.svg] # spacy-transformers: Use pretrained transformers like BERT, XLNet
 and GPT-2 in spaCy This package provides [spaCy](https://github.com/explosion/
 spaCy) components and architectures to use transformer models via [Hugging
 Face's `transformers`](https://github.com/huggingface/transformers) in spaCy.
 The result is convenient access to state-of-the-art transformer architectures,
 such as BERT, GPT-2, XLNet, etc. > **This release requires [spaCy v3](https://
-spacy.io/usage/v3).** For > the previous version of this library, see the >
+spacy.io/usage/v3).** For the > previous version of this library, see the >
 [`v0.6.x` branch](https://github.com/explosion/spacy-transformers/tree/v0.6.x).
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/
-public/18/master.svg?logo=azure-pipelines&style=flat-square)](https://
-dev.azure.com/explosion-ai/public/_build?definitionId=18) [![PyPi](https://
-img.shields.io/pypi/v/spacy-transformers.svg?style=flat-
-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/spacy-
-transformers) [![GitHub](https://img.shields.io/github/release/explosion/spacy-
-transformers/all.svg?style=flat-square&logo=github)](https://github.com/
-explosion/spacy-transformers/releases) [![Code style: black](https://
-img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://
-github.com/ambv/black) ## Features - Use pretrained transformer models like
-**BERT**, **RoBERTa** and **XLNet** to power your spaCy pipeline. - Easy
-**multi-task learning**: backprop to one transformer model from several
-pipeline components. - Train using spaCy v3's powerful and extensible config
-system. - Automatic alignment of transformer output to spaCy's tokenization. -
-Easily customize what transformer data is saved in the `Doc` object. - Easily
-customize how long documents are processed. - Out-of-the-box serialization and
-model packaging. ## ð Installation Installing the package from pip will
-automatically install all dependencies, including PyTorch and spaCy. Make sure
-you install this package **before** you install the models. Also note that this
-package requires **Python 3.6+**, **PyTorch v1.5+** and **spaCy v3.0+**.
-```bash pip install 'spacy[transformers]' ``` For GPU installation, find your
-CUDA version using `nvcc --version` and add the [version in brackets](https://
-spacy.io/usage/#gpu), e.g. `spacy[transformers,cuda92]` for CUDA9.2 or `spacy
-[transformers,cuda100]` for CUDA10.0. If you are having trouble installing
-PyTorch, follow the [instructions](https://pytorch.org/get-started/locally/) on
-the official website for your specific operating system and requirements, or
-try the following: ```bash pip install spacy-transformers -f https://
-download.pytorch.org/whl/torch_stable.html ``` ## ð Documentation > â ï¸
-**Important note:** This package has been extensively refactored to take >
-advantage of [spaCy v3.0](https://spacy.io). Previous versions that > were
-built for [spaCy v2.x](https://v2.spacy.io) worked considerably > differently.
-Please see previous tagged versions of this README for > documentation on prior
-versions. - ð [Embeddings, Transformers and Transfer Learning](https://
-spacy.io/usage/embeddings-transformers): How to use transformers in spaCy -
-ð [Training Pipelines and Models](https://spacy.io/usage/training): Train
-and update components on your own data and integrate custom models - ð
-[Layers and Model Architectures](https://spacy.io/usage/layers-architectures):
-Power spaCy components with custom neural networks - ð [`Transformer`]
-(https://spacy.io/api/transformer): Pipeline component API reference - ð
-[Transformer architectures](https://spacy.io/api/architectures#transformers):
-Architectures and registered functions ## Bug reports and other issues Please
-use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues) to
-report a bug, or open a new thread on the [discussion board](https://
+[![tests](https://github.com/explosion/spacy-transformers/actions/workflows/
+tests.yml/badge.svg)](https://github.com/explosion/spacy-transformers/actions/
+workflows/tests.yml) [![PyPi](https://img.shields.io/pypi/v/spacy-
+transformers.svg?style=flat-square&logo=pypi&logoColor=white)](https://
+pypi.python.org/pypi/spacy-transformers) [![GitHub](https://img.shields.io/
+github/release/explosion/spacy-transformers/all.svg?style=flat-
+square&logo=github)](https://github.com/explosion/spacy-transformers/releases)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg?style=flat-square)](https://github.com/ambv/black) ## Features - Use
+pretrained transformer models like **BERT**, **RoBERTa** and **XLNet** to power
+your spaCy pipeline. - Easy **multi-task learning**: backprop to one
+transformer model from several pipeline components. - Train using spaCy v3's
+powerful and extensible config system. - Automatic alignment of transformer
+output to spaCy's tokenization. - Easily customize what transformer data is
+saved in the `Doc` object. - Easily customize how long documents are processed.
+- Out-of-the-box serialization and model packaging. ## ð Installation
+Installing the package from pip will automatically install all dependencies,
+including PyTorch and spaCy. Make sure you install this package **before** you
+install the models. Also note that this package requires **Python 3.6+**,
+**PyTorch v1.5+** and **spaCy v3.0+**. ```bash pip install 'spacy
+[transformers]' ``` For GPU installation, find your CUDA version using `nvcc --
+version` and add the [version in brackets](https://spacy.io/usage/#gpu), e.g.
+`spacy[transformers,cuda92]` for CUDA9.2 or `spacy[transformers,cuda100]` for
+CUDA10.0. If you are having trouble installing PyTorch, follow the
+[instructions](https://pytorch.org/get-started/locally/) on the official
+website for your specific operating system and requirements. ## ð
+Documentation > â ï¸ **Important note:** This package has been extensively
+refactored to take > advantage of [spaCy v3.0](https://spacy.io). Previous
+versions that were built > for [spaCy v2.x](https://v2.spacy.io) worked
+considerably differently. Please > see previous tagged versions of this README
+for documentation on prior > versions. - ð [Embeddings, Transformers and
+Transfer Learning](https://spacy.io/usage/embeddings-transformers): How to use
+transformers in spaCy - ð [Training Pipelines and Models](https://spacy.io/
+usage/training): Train and update components on your own data and integrate
+custom models - ð [Layers and Model Architectures](https://spacy.io/usage/
+layers-architectures): Power spaCy components with custom neural networks -
+ð [`Transformer`](https://spacy.io/api/transformer): Pipeline component API
+reference - ð [Transformer architectures](https://spacy.io/api/
+architectures#transformers): Architectures and registered functions ## Applying
+pretrained text and token classification models Note that the `transformer`
+component from `spacy-transformers` does not support task-specific heads like
+token or text classification. A task-specific transformer model can be used as
+a source of features to train spaCy components like `ner` or `textcat`, but the
+`transformer` component does not provide access to task-specific heads for
+training or inference. Alternatively, if you only want use to the
+**predictions** from an existing Hugging Face text or token classification
+model, you can use the wrappers from [`spacy-huggingface-pipelines`](https://
+github.com/explosion/spacy-huggingface-pipelines) to incorporate task-specific
+transformer models into your spaCy pipelines. ## Bug reports and other issues
+Please use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues)
+to report a bug, or open a new thread on the [discussion board](https://
 github.com/explosion/spaCy/discussions) for any other issue.
```

### Comparing `spacy-transformers-1.2.3/README.md` & `spacy-transformers-1.2.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 This package provides [spaCy](https://github.com/explosion/spaCy) components and
 architectures to use transformer models via
 [Hugging Face's `transformers`](https://github.com/huggingface/transformers) in
 spaCy. The result is convenient access to state-of-the-art transformer
 architectures, such as BERT, GPT-2, XLNet, etc.
 
-> **This release requires [spaCy v3](https://spacy.io/usage/v3).** For
-> the previous version of this library, see the
+> **This release requires [spaCy v3](https://spacy.io/usage/v3).** For the
+> previous version of this library, see the
 > [`v0.6.x` branch](https://github.com/explosion/spacy-transformers/tree/v0.6.x).
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/18/master.svg?logo=azure-pipelines&style=flat-square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=18)
+[![tests](https://github.com/explosion/spacy-transformers/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/spacy-transformers/actions/workflows/tests.yml)
 [![PyPi](https://img.shields.io/pypi/v/spacy-transformers.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/spacy-transformers)
 [![GitHub](https://img.shields.io/github/release/explosion/spacy-transformers/all.svg?style=flat-square&logo=github)](https://github.com/explosion/spacy-transformers/releases)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 ## Features
 
 - Use pretrained transformer models like **BERT**, **RoBERTa** and **XLNet** to
@@ -43,40 +43,50 @@
 For GPU installation, find your CUDA version using `nvcc --version` and add the
 [version in brackets](https://spacy.io/usage/#gpu), e.g.
 `spacy[transformers,cuda92]` for CUDA9.2 or `spacy[transformers,cuda100]` for
 CUDA10.0.
 
 If you are having trouble installing PyTorch, follow the
 [instructions](https://pytorch.org/get-started/locally/) on the official website
-for your specific operating system and requirements, or try the following:
-
-```bash
-pip install spacy-transformers -f https://download.pytorch.org/whl/torch_stable.html
-```
+for your specific operating system and requirements.
 
 ## 📖 Documentation
 
 > ⚠️ **Important note:** This package has been extensively refactored to take
-> advantage of [spaCy v3.0](https://spacy.io). Previous versions that
-> were built for [spaCy v2.x](https://v2.spacy.io) worked considerably
-> differently. Please see previous tagged versions of this README for
-> documentation on prior versions.
+> advantage of [spaCy v3.0](https://spacy.io). Previous versions that were built
+> for [spaCy v2.x](https://v2.spacy.io) worked considerably differently. Please
+> see previous tagged versions of this README for documentation on prior
+> versions.
 
 - 📘
   [Embeddings, Transformers and Transfer Learning](https://spacy.io/usage/embeddings-transformers):
   How to use transformers in spaCy
-- 📘 [Training Pipelines and Models](https://spacy.io/usage/training):
-  Train and update components on your own data and integrate custom models
+- 📘 [Training Pipelines and Models](https://spacy.io/usage/training): Train and
+  update components on your own data and integrate custom models
 - 📘
   [Layers and Model Architectures](https://spacy.io/usage/layers-architectures):
   Power spaCy components with custom neural networks
-- 📗 [`Transformer`](https://spacy.io/api/transformer): Pipeline
-  component API reference
+- 📗 [`Transformer`](https://spacy.io/api/transformer): Pipeline component API
+  reference
 - 📗
   [Transformer architectures](https://spacy.io/api/architectures#transformers):
   Architectures and registered functions
 
+## Applying pretrained text and token classification models
+
+Note that the `transformer` component from `spacy-transformers` does not support
+task-specific heads like token or text classification. A task-specific
+transformer model can be used as a source of features to train spaCy components
+like `ner` or `textcat`, but the `transformer` component does not provide access
+to task-specific heads for training or inference.
+
+Alternatively, if you only want use to the **predictions** from an existing
+Hugging Face text or token classification model, you can use the wrappers from
+[`spacy-huggingface-pipelines`](https://github.com/explosion/spacy-huggingface-pipelines)
+to incorporate task-specific transformer models into your spaCy pipelines.
+
 ## Bug reports and other issues
 
-Please use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues) to report a bug, or open a new thread on the
-[discussion board](https://github.com/explosion/spaCy/discussions)
-for any other issue.
+Please use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues) to
+report a bug, or open a new thread on the
+[discussion board](https://github.com/explosion/spaCy/discussions) for any other
+issue.
```

#### html2text {}

```diff
@@ -1,53 +1,61 @@
 [https://explosion.ai/assets/img/logo.svg] # spacy-transformers: Use pretrained
 transformers like BERT, XLNet and GPT-2 in spaCy This package provides [spaCy]
 (https://github.com/explosion/spaCy) components and architectures to use
 transformer models via [Hugging Face's `transformers`](https://github.com/
 huggingface/transformers) in spaCy. The result is convenient access to state-
 of-the-art transformer architectures, such as BERT, GPT-2, XLNet, etc. > **This
-release requires [spaCy v3](https://spacy.io/usage/v3).** For > the previous
+release requires [spaCy v3](https://spacy.io/usage/v3).** For the > previous
 version of this library, see the > [`v0.6.x` branch](https://github.com/
-explosion/spacy-transformers/tree/v0.6.x). [![Azure Pipelines](https://
-img.shields.io/azure-devops/build/explosion-ai/public/18/master.svg?logo=azure-
-pipelines&style=flat-square)](https://dev.azure.com/explosion-ai/public/
-_build?definitionId=18) [![PyPi](https://img.shields.io/pypi/v/spacy-
-transformers.svg?style=flat-square&logo=pypi&logoColor=white)](https://
-pypi.python.org/pypi/spacy-transformers) [![GitHub](https://img.shields.io/
-github/release/explosion/spacy-transformers/all.svg?style=flat-
-square&logo=github)](https://github.com/explosion/spacy-transformers/releases)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-
-000000.svg?style=flat-square)](https://github.com/ambv/black) ## Features - Use
-pretrained transformer models like **BERT**, **RoBERTa** and **XLNet** to power
-your spaCy pipeline. - Easy **multi-task learning**: backprop to one
-transformer model from several pipeline components. - Train using spaCy v3's
-powerful and extensible config system. - Automatic alignment of transformer
-output to spaCy's tokenization. - Easily customize what transformer data is
-saved in the `Doc` object. - Easily customize how long documents are processed.
-- Out-of-the-box serialization and model packaging. ## ð Installation
-Installing the package from pip will automatically install all dependencies,
-including PyTorch and spaCy. Make sure you install this package **before** you
-install the models. Also note that this package requires **Python 3.6+**,
-**PyTorch v1.5+** and **spaCy v3.0+**. ```bash pip install 'spacy
-[transformers]' ``` For GPU installation, find your CUDA version using `nvcc --
-version` and add the [version in brackets](https://spacy.io/usage/#gpu), e.g.
-`spacy[transformers,cuda92]` for CUDA9.2 or `spacy[transformers,cuda100]` for
-CUDA10.0. If you are having trouble installing PyTorch, follow the
-[instructions](https://pytorch.org/get-started/locally/) on the official
-website for your specific operating system and requirements, or try the
-following: ```bash pip install spacy-transformers -f https://
-download.pytorch.org/whl/torch_stable.html ``` ## ð Documentation > â ï¸
-**Important note:** This package has been extensively refactored to take >
-advantage of [spaCy v3.0](https://spacy.io). Previous versions that > were
-built for [spaCy v2.x](https://v2.spacy.io) worked considerably > differently.
-Please see previous tagged versions of this README for > documentation on prior
-versions. - ð [Embeddings, Transformers and Transfer Learning](https://
-spacy.io/usage/embeddings-transformers): How to use transformers in spaCy -
-ð [Training Pipelines and Models](https://spacy.io/usage/training): Train
-and update components on your own data and integrate custom models - ð
-[Layers and Model Architectures](https://spacy.io/usage/layers-architectures):
-Power spaCy components with custom neural networks - ð [`Transformer`]
-(https://spacy.io/api/transformer): Pipeline component API reference - ð
-[Transformer architectures](https://spacy.io/api/architectures#transformers):
-Architectures and registered functions ## Bug reports and other issues Please
-use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues) to
-report a bug, or open a new thread on the [discussion board](https://
-github.com/explosion/spaCy/discussions) for any other issue.
+explosion/spacy-transformers/tree/v0.6.x). [![tests](https://github.com/
+explosion/spacy-transformers/actions/workflows/tests.yml/badge.svg)](https://
+github.com/explosion/spacy-transformers/actions/workflows/tests.yml) [![PyPi]
+(https://img.shields.io/pypi/v/spacy-transformers.svg?style=flat-
+square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/spacy-
+transformers) [![GitHub](https://img.shields.io/github/release/explosion/spacy-
+transformers/all.svg?style=flat-square&logo=github)](https://github.com/
+explosion/spacy-transformers/releases) [![Code style: black](https://
+img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://
+github.com/ambv/black) ## Features - Use pretrained transformer models like
+**BERT**, **RoBERTa** and **XLNet** to power your spaCy pipeline. - Easy
+**multi-task learning**: backprop to one transformer model from several
+pipeline components. - Train using spaCy v3's powerful and extensible config
+system. - Automatic alignment of transformer output to spaCy's tokenization. -
+Easily customize what transformer data is saved in the `Doc` object. - Easily
+customize how long documents are processed. - Out-of-the-box serialization and
+model packaging. ## ð Installation Installing the package from pip will
+automatically install all dependencies, including PyTorch and spaCy. Make sure
+you install this package **before** you install the models. Also note that this
+package requires **Python 3.6+**, **PyTorch v1.5+** and **spaCy v3.0+**.
+```bash pip install 'spacy[transformers]' ``` For GPU installation, find your
+CUDA version using `nvcc --version` and add the [version in brackets](https://
+spacy.io/usage/#gpu), e.g. `spacy[transformers,cuda92]` for CUDA9.2 or `spacy
+[transformers,cuda100]` for CUDA10.0. If you are having trouble installing
+PyTorch, follow the [instructions](https://pytorch.org/get-started/locally/) on
+the official website for your specific operating system and requirements. ##
+ð Documentation > â ï¸ **Important note:** This package has been
+extensively refactored to take > advantage of [spaCy v3.0](https://spacy.io).
+Previous versions that were built > for [spaCy v2.x](https://v2.spacy.io)
+worked considerably differently. Please > see previous tagged versions of this
+README for documentation on prior > versions. - ð [Embeddings, Transformers
+and Transfer Learning](https://spacy.io/usage/embeddings-transformers): How to
+use transformers in spaCy - ð [Training Pipelines and Models](https://
+spacy.io/usage/training): Train and update components on your own data and
+integrate custom models - ð [Layers and Model Architectures](https://
+spacy.io/usage/layers-architectures): Power spaCy components with custom neural
+networks - ð [`Transformer`](https://spacy.io/api/transformer): Pipeline
+component API reference - ð [Transformer architectures](https://spacy.io/
+api/architectures#transformers): Architectures and registered functions ##
+Applying pretrained text and token classification models Note that the
+`transformer` component from `spacy-transformers` does not support task-
+specific heads like token or text classification. A task-specific transformer
+model can be used as a source of features to train spaCy components like `ner`
+or `textcat`, but the `transformer` component does not provide access to task-
+specific heads for training or inference. Alternatively, if you only want use
+to the **predictions** from an existing Hugging Face text or token
+classification model, you can use the wrappers from [`spacy-huggingface-
+pipelines`](https://github.com/explosion/spacy-huggingface-pipelines) to
+incorporate task-specific transformer models into your spaCy pipelines. ## Bug
+reports and other issues Please use [spaCy's issue tracker](https://github.com/
+explosion/spaCy/issues) to report a bug, or open a new thread on the
+[discussion board](https://github.com/explosion/spaCy/discussions) for any
+other issue.
```

### Comparing `spacy-transformers-1.2.3/setup.cfg` & `spacy-transformers-1.2.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.2.3
+version = 1.2.4
 description = spaCy pipelines for pre-trained BERT and other transformers
 url = https://spacy.io
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -29,15 +29,15 @@
 [options]
 zip_safe = false
 include_package_data = true
 python_requires = >=3.6
 install_requires = 
 	spacy>=3.5.0,<4.0.0
 	numpy>=1.15.0
-	transformers>=3.4.0,<4.29.0
+	transformers>=3.4.0,<4.30.0
 	torch>=1.8.0
 	srsly>=2.4.0,<3.0.0
 	dataclasses>=0.6,<1.0; python_version < "3.7"
 	spacy-alignments>=0.7.2,<1.0.0
 
 [options.extras_require]
 cuda =
```

### Comparing `spacy-transformers-1.2.3/setup.py` & `spacy-transformers-1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/align.pyi` & `spacy-transformers-1.2.4/spacy_transformers/align.pyi`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/align.pyx` & `spacy-transformers-1.2.4/spacy_transformers/align.pyx`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/annotation_setters.py` & `spacy-transformers-1.2.4/spacy_transformers/annotation_setters.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/architectures.py` & `spacy-transformers-1.2.4/spacy_transformers/architectures.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/data_classes.py` & `spacy-transformers-1.2.4/spacy_transformers/data_classes.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/layers/_util.py` & `spacy-transformers-1.2.4/spacy_transformers/layers/_util.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/layers/hf_shim.py` & `spacy-transformers-1.2.4/spacy_transformers/layers/hf_shim.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/layers/hf_wrapper.py` & `spacy-transformers-1.2.4/spacy_transformers/layers/hf_wrapper.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/layers/listener.py` & `spacy-transformers-1.2.4/spacy_transformers/layers/listener.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/layers/transformer_model.py` & `spacy-transformers-1.2.4/spacy_transformers/layers/transformer_model.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/layers/trfs2arrays.py` & `spacy-transformers-1.2.4/spacy_transformers/layers/trfs2arrays.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/pipeline_component.py` & `spacy-transformers-1.2.4/spacy_transformers/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/span_getters.py` & `spacy-transformers-1.2.4/spacy_transformers/span_getters.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/tests/regression/test_spacy_issue6401.py` & `spacy-transformers-1.2.4/spacy_transformers/tests/regression/test_spacy_issue6401.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/tests/regression/test_spacy_issue7029.py` & `spacy-transformers-1.2.4/spacy_transformers/tests/regression/test_spacy_issue7029.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/tests/test_alignment.py` & `spacy-transformers-1.2.4/spacy_transformers/tests/test_alignment.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/tests/test_configs.py` & `spacy-transformers-1.2.4/spacy_transformers/tests/test_configs.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/tests/test_data_classes.py` & `spacy-transformers-1.2.4/spacy_transformers/tests/test_data_classes.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/tests/test_model_sequence_classification.py` & `spacy-transformers-1.2.4/spacy_transformers/tests/test_model_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/tests/test_model_wrapper.py` & `spacy-transformers-1.2.4/spacy_transformers/tests/test_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/tests/test_pipeline_component.py` & `spacy-transformers-1.2.4/spacy_transformers/tests/test_pipeline_component.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/tests/test_serialize.py` & `spacy-transformers-1.2.4/spacy_transformers/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/tests/test_spanners.py` & `spacy-transformers-1.2.4/spacy_transformers/tests/test_spanners.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/tests/test_textcatcnn.py` & `spacy-transformers-1.2.4/spacy_transformers/tests/test_textcatcnn.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/tests/test_tok2vectransformer.py` & `spacy-transformers-1.2.4/spacy_transformers/tests/test_tok2vectransformer.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/tests/test_truncation.py` & `spacy-transformers-1.2.4/spacy_transformers/tests/test_truncation.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/tests/util.py` & `spacy-transformers-1.2.4/spacy_transformers/tests/util.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/truncate.py` & `spacy-transformers-1.2.4/spacy_transformers/truncate.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers/util.py` & `spacy-transformers-1.2.4/spacy_transformers/util.py`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers.egg-info/PKG-INFO` & `spacy-transformers-1.2.4/spacy_transformers.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacy-transformers
-Version: 1.2.3
+Version: 1.2.4
 Summary: spaCy pipelines for pre-trained BERT and other transformers
 Home-page: https://spacy.io
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -44,19 +44,19 @@
 
 This package provides [spaCy](https://github.com/explosion/spaCy) components and
 architectures to use transformer models via
 [Hugging Face's `transformers`](https://github.com/huggingface/transformers) in
 spaCy. The result is convenient access to state-of-the-art transformer
 architectures, such as BERT, GPT-2, XLNet, etc.
 
-> **This release requires [spaCy v3](https://spacy.io/usage/v3).** For
-> the previous version of this library, see the
+> **This release requires [spaCy v3](https://spacy.io/usage/v3).** For the
+> previous version of this library, see the
 > [`v0.6.x` branch](https://github.com/explosion/spacy-transformers/tree/v0.6.x).
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/18/master.svg?logo=azure-pipelines&style=flat-square)](https://dev.azure.com/explosion-ai/public/_build?definitionId=18)
+[![tests](https://github.com/explosion/spacy-transformers/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/spacy-transformers/actions/workflows/tests.yml)
 [![PyPi](https://img.shields.io/pypi/v/spacy-transformers.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/spacy-transformers)
 [![GitHub](https://img.shields.io/github/release/explosion/spacy-transformers/all.svg?style=flat-square&logo=github)](https://github.com/explosion/spacy-transformers/releases)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://github.com/ambv/black)
 
 ## Features
 
 - Use pretrained transformer models like **BERT**, **RoBERTa** and **XLNet** to
@@ -83,40 +83,50 @@
 For GPU installation, find your CUDA version using `nvcc --version` and add the
 [version in brackets](https://spacy.io/usage/#gpu), e.g.
 `spacy[transformers,cuda92]` for CUDA9.2 or `spacy[transformers,cuda100]` for
 CUDA10.0.
 
 If you are having trouble installing PyTorch, follow the
 [instructions](https://pytorch.org/get-started/locally/) on the official website
-for your specific operating system and requirements, or try the following:
-
-```bash
-pip install spacy-transformers -f https://download.pytorch.org/whl/torch_stable.html
-```
+for your specific operating system and requirements.
 
 ## 📖 Documentation
 
 > ⚠️ **Important note:** This package has been extensively refactored to take
-> advantage of [spaCy v3.0](https://spacy.io). Previous versions that
-> were built for [spaCy v2.x](https://v2.spacy.io) worked considerably
-> differently. Please see previous tagged versions of this README for
-> documentation on prior versions.
+> advantage of [spaCy v3.0](https://spacy.io). Previous versions that were built
+> for [spaCy v2.x](https://v2.spacy.io) worked considerably differently. Please
+> see previous tagged versions of this README for documentation on prior
+> versions.
 
 - 📘
   [Embeddings, Transformers and Transfer Learning](https://spacy.io/usage/embeddings-transformers):
   How to use transformers in spaCy
-- 📘 [Training Pipelines and Models](https://spacy.io/usage/training):
-  Train and update components on your own data and integrate custom models
+- 📘 [Training Pipelines and Models](https://spacy.io/usage/training): Train and
+  update components on your own data and integrate custom models
 - 📘
   [Layers and Model Architectures](https://spacy.io/usage/layers-architectures):
   Power spaCy components with custom neural networks
-- 📗 [`Transformer`](https://spacy.io/api/transformer): Pipeline
-  component API reference
+- 📗 [`Transformer`](https://spacy.io/api/transformer): Pipeline component API
+  reference
 - 📗
   [Transformer architectures](https://spacy.io/api/architectures#transformers):
   Architectures and registered functions
 
+## Applying pretrained text and token classification models
+
+Note that the `transformer` component from `spacy-transformers` does not support
+task-specific heads like token or text classification. A task-specific
+transformer model can be used as a source of features to train spaCy components
+like `ner` or `textcat`, but the `transformer` component does not provide access
+to task-specific heads for training or inference.
+
+Alternatively, if you only want use to the **predictions** from an existing
+Hugging Face text or token classification model, you can use the wrappers from
+[`spacy-huggingface-pipelines`](https://github.com/explosion/spacy-huggingface-pipelines)
+to incorporate task-specific transformer models into your spaCy pipelines.
+
 ## Bug reports and other issues
 
-Please use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues) to report a bug, or open a new thread on the
-[discussion board](https://github.com/explosion/spaCy/discussions)
-for any other issue.
+Please use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues) to
+report a bug, or open a new thread on the
+[discussion board](https://github.com/explosion/spaCy/discussions) for any other
+issue.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spacy-transformers Version: 1.2.3 Summary: spaCy
+Metadata-Version: 2.1 Name: spacy-transformers Version: 1.2.4 Summary: spaCy
 pipelines for pre-trained BERT and other transformers Home-page: https://
 spacy.io Author: Explosion Author-email: contact@explosion.ai License: MIT
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
 :: Console Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
@@ -19,53 +19,61 @@
 Provides-Extra: cuda112 License-File: LICENSE [https://explosion.ai/assets/img/
 logo.svg] # spacy-transformers: Use pretrained transformers like BERT, XLNet
 and GPT-2 in spaCy This package provides [spaCy](https://github.com/explosion/
 spaCy) components and architectures to use transformer models via [Hugging
 Face's `transformers`](https://github.com/huggingface/transformers) in spaCy.
 The result is convenient access to state-of-the-art transformer architectures,
 such as BERT, GPT-2, XLNet, etc. > **This release requires [spaCy v3](https://
-spacy.io/usage/v3).** For > the previous version of this library, see the >
+spacy.io/usage/v3).** For the > previous version of this library, see the >
 [`v0.6.x` branch](https://github.com/explosion/spacy-transformers/tree/v0.6.x).
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/
-public/18/master.svg?logo=azure-pipelines&style=flat-square)](https://
-dev.azure.com/explosion-ai/public/_build?definitionId=18) [![PyPi](https://
-img.shields.io/pypi/v/spacy-transformers.svg?style=flat-
-square&logo=pypi&logoColor=white)](https://pypi.python.org/pypi/spacy-
-transformers) [![GitHub](https://img.shields.io/github/release/explosion/spacy-
-transformers/all.svg?style=flat-square&logo=github)](https://github.com/
-explosion/spacy-transformers/releases) [![Code style: black](https://
-img.shields.io/badge/code%20style-black-000000.svg?style=flat-square)](https://
-github.com/ambv/black) ## Features - Use pretrained transformer models like
-**BERT**, **RoBERTa** and **XLNet** to power your spaCy pipeline. - Easy
-**multi-task learning**: backprop to one transformer model from several
-pipeline components. - Train using spaCy v3's powerful and extensible config
-system. - Automatic alignment of transformer output to spaCy's tokenization. -
-Easily customize what transformer data is saved in the `Doc` object. - Easily
-customize how long documents are processed. - Out-of-the-box serialization and
-model packaging. ## ð Installation Installing the package from pip will
-automatically install all dependencies, including PyTorch and spaCy. Make sure
-you install this package **before** you install the models. Also note that this
-package requires **Python 3.6+**, **PyTorch v1.5+** and **spaCy v3.0+**.
-```bash pip install 'spacy[transformers]' ``` For GPU installation, find your
-CUDA version using `nvcc --version` and add the [version in brackets](https://
-spacy.io/usage/#gpu), e.g. `spacy[transformers,cuda92]` for CUDA9.2 or `spacy
-[transformers,cuda100]` for CUDA10.0. If you are having trouble installing
-PyTorch, follow the [instructions](https://pytorch.org/get-started/locally/) on
-the official website for your specific operating system and requirements, or
-try the following: ```bash pip install spacy-transformers -f https://
-download.pytorch.org/whl/torch_stable.html ``` ## ð Documentation > â ï¸
-**Important note:** This package has been extensively refactored to take >
-advantage of [spaCy v3.0](https://spacy.io). Previous versions that > were
-built for [spaCy v2.x](https://v2.spacy.io) worked considerably > differently.
-Please see previous tagged versions of this README for > documentation on prior
-versions. - ð [Embeddings, Transformers and Transfer Learning](https://
-spacy.io/usage/embeddings-transformers): How to use transformers in spaCy -
-ð [Training Pipelines and Models](https://spacy.io/usage/training): Train
-and update components on your own data and integrate custom models - ð
-[Layers and Model Architectures](https://spacy.io/usage/layers-architectures):
-Power spaCy components with custom neural networks - ð [`Transformer`]
-(https://spacy.io/api/transformer): Pipeline component API reference - ð
-[Transformer architectures](https://spacy.io/api/architectures#transformers):
-Architectures and registered functions ## Bug reports and other issues Please
-use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues) to
-report a bug, or open a new thread on the [discussion board](https://
+[![tests](https://github.com/explosion/spacy-transformers/actions/workflows/
+tests.yml/badge.svg)](https://github.com/explosion/spacy-transformers/actions/
+workflows/tests.yml) [![PyPi](https://img.shields.io/pypi/v/spacy-
+transformers.svg?style=flat-square&logo=pypi&logoColor=white)](https://
+pypi.python.org/pypi/spacy-transformers) [![GitHub](https://img.shields.io/
+github/release/explosion/spacy-transformers/all.svg?style=flat-
+square&logo=github)](https://github.com/explosion/spacy-transformers/releases)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-
+000000.svg?style=flat-square)](https://github.com/ambv/black) ## Features - Use
+pretrained transformer models like **BERT**, **RoBERTa** and **XLNet** to power
+your spaCy pipeline. - Easy **multi-task learning**: backprop to one
+transformer model from several pipeline components. - Train using spaCy v3's
+powerful and extensible config system. - Automatic alignment of transformer
+output to spaCy's tokenization. - Easily customize what transformer data is
+saved in the `Doc` object. - Easily customize how long documents are processed.
+- Out-of-the-box serialization and model packaging. ## ð Installation
+Installing the package from pip will automatically install all dependencies,
+including PyTorch and spaCy. Make sure you install this package **before** you
+install the models. Also note that this package requires **Python 3.6+**,
+**PyTorch v1.5+** and **spaCy v3.0+**. ```bash pip install 'spacy
+[transformers]' ``` For GPU installation, find your CUDA version using `nvcc --
+version` and add the [version in brackets](https://spacy.io/usage/#gpu), e.g.
+`spacy[transformers,cuda92]` for CUDA9.2 or `spacy[transformers,cuda100]` for
+CUDA10.0. If you are having trouble installing PyTorch, follow the
+[instructions](https://pytorch.org/get-started/locally/) on the official
+website for your specific operating system and requirements. ## ð
+Documentation > â ï¸ **Important note:** This package has been extensively
+refactored to take > advantage of [spaCy v3.0](https://spacy.io). Previous
+versions that were built > for [spaCy v2.x](https://v2.spacy.io) worked
+considerably differently. Please > see previous tagged versions of this README
+for documentation on prior > versions. - ð [Embeddings, Transformers and
+Transfer Learning](https://spacy.io/usage/embeddings-transformers): How to use
+transformers in spaCy - ð [Training Pipelines and Models](https://spacy.io/
+usage/training): Train and update components on your own data and integrate
+custom models - ð [Layers and Model Architectures](https://spacy.io/usage/
+layers-architectures): Power spaCy components with custom neural networks -
+ð [`Transformer`](https://spacy.io/api/transformer): Pipeline component API
+reference - ð [Transformer architectures](https://spacy.io/api/
+architectures#transformers): Architectures and registered functions ## Applying
+pretrained text and token classification models Note that the `transformer`
+component from `spacy-transformers` does not support task-specific heads like
+token or text classification. A task-specific transformer model can be used as
+a source of features to train spaCy components like `ner` or `textcat`, but the
+`transformer` component does not provide access to task-specific heads for
+training or inference. Alternatively, if you only want use to the
+**predictions** from an existing Hugging Face text or token classification
+model, you can use the wrappers from [`spacy-huggingface-pipelines`](https://
+github.com/explosion/spacy-huggingface-pipelines) to incorporate task-specific
+transformer models into your spaCy pipelines. ## Bug reports and other issues
+Please use [spaCy's issue tracker](https://github.com/explosion/spaCy/issues)
+to report a bug, or open a new thread on the [discussion board](https://
 github.com/explosion/spaCy/discussions) for any other issue.
```

### Comparing `spacy-transformers-1.2.3/spacy_transformers.egg-info/SOURCES.txt` & `spacy-transformers-1.2.4/spacy_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers.egg-info/entry_points.txt` & `spacy-transformers-1.2.4/spacy_transformers.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `spacy-transformers-1.2.3/spacy_transformers.egg-info/requires.txt` & `spacy-transformers-1.2.4/spacy_transformers.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 spacy<4.0.0,>=3.5.0
 numpy>=1.15.0
-transformers<4.29.0,>=3.4.0
+transformers<4.30.0,>=3.4.0
 torch>=1.8.0
 srsly<3.0.0,>=2.4.0
 spacy-alignments<1.0.0,>=0.7.2
 
 [:python_version < "3.7"]
 dataclasses<1.0,>=0.6
```

