# Comparing `tmp/syngen-0.1.4.tar.gz` & `tmp/syngen-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.1.4.tar", last modified: Fri May 19 12:52:04 2023, max compression
+gzip compressed data, was "syngen-0.1.5.tar", last modified: Mon May 22 08:44:40 2023, max compression
```

## Comparing `syngen-0.1.4.tar` & `syngen-0.1.5.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.415522 syngen-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-19 12:50:37.000000 syngen-0.1.4/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-19 12:50:37.000000 syngen-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-19 12:50:37.000000 syngen-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-19 12:52:04.415522 syngen-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14309 2023-05-19 12:50:37.000000 syngen-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-19 12:50:37.000000 syngen-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-19 12:52:04.415522 syngen-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.403522 syngen-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.407522 syngen-0.1.4/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.407522 syngen-0.1.4/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.407522 syngen-0.1.4/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.407522 syngen-0.1.4/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.407522 syngen-0.1.4/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7879 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.411522 syngen-0.1.4/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.411522 syngen-0.1.4/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.403522 syngen-0.1.4/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.411522 syngen-0.1.4/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.411522 syngen-0.1.4/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.411522 syngen-0.1.4/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.411522 syngen-0.1.4/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.411522 syngen-0.1.4/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6972 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.415522 syngen-0.1.4/src/syngen/ml/train_chain/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/train_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15251 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/train_chain/train_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.415522 syngen-0.1.4/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      373 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6064 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.415522 syngen-0.1.4/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.415522 syngen-0.1.4/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    33024 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10467 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.415522 syngen-0.1.4/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.415522 syngen-0.1.4/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.415522 syngen-0.1.4/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-05-19 12:50:37.000000 syngen-0.1.4/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-19 12:52:04.407522 syngen-0.1.4/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15048 2023-05-19 12:52:04.000000 syngen-0.1.4/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-19 12:52:04.000000 syngen-0.1.4/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-19 12:52:04.000000 syngen-0.1.4/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-19 12:52:04.000000 syngen-0.1.4/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-19 12:52:04.000000 syngen-0.1.4/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-19 12:52:04.000000 syngen-0.1.4/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.261839 syngen-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-22 08:43:19.000000 syngen-0.1.5/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-22 08:43:19.000000 syngen-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-22 08:43:19.000000 syngen-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    16393 2023-05-22 08:44:40.261839 syngen-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    15654 2023-05-22 08:43:19.000000 syngen-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-22 08:43:19.000000 syngen-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-22 08:44:40.261839 syngen-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.245839 syngen-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.253839 syngen-0.1.5/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.253839 syngen-0.1.5/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.253839 syngen-0.1.5/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10086 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.253839 syngen-0.1.5/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3475 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.253839 syngen-0.1.5/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7887 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.253839 syngen-0.1.5/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5294 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.249839 syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6972 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/train_chain/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/train_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15251 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/train_chain/train_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      373 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6064 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.257839 syngen-0.1.5/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.261839 syngen-0.1.5/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33024 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10467 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.261839 syngen-0.1.5/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11347 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.261839 syngen-0.1.5/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2115 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.261839 syngen-0.1.5/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13244 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/ml/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-05-22 08:43:19.000000 syngen-0.1.5/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-22 08:44:40.253839 syngen-0.1.5/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    16393 2023-05-22 08:44:40.000000 syngen-0.1.5/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-22 08:44:40.000000 syngen-0.1.5/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-22 08:44:40.000000 syngen-0.1.5/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-22 08:44:40.000000 syngen-0.1.5/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-22 08:44:40.000000 syngen-0.1.5/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-22 08:44:40.000000 syngen-0.1.5/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.1.4/LICENSE` & `syngen-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/PKG-INFO` & `syngen-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.1.4
+Version: 0.1.5
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -73,30 +73,30 @@
     --epochs INT \
     --row_limit INT \
     --drop_null BOOL \
     --print_report BOOL \
     --batch_size INT
 ```
 
-For training of the multiple linked tables call:
+To train one or more tables using a metadata file, you can use the following command:
 
 ```bash
 train --metadata_path PATH_TO_METADATA_YAML
 ```
 
 The parameters which you can set up for training process:
 
 - <i>source</i> – required parameter for training of single table, a path to the file that you want to use as a reference
 - <i>table_name</i> – required parameter for training of single table, an arbitrary string to name the directories 
 - <i>epochs</i> – a number of training epochs. Since the early stopping mechanism is implemented the bigger value of epochs is the better
 - <i>row_limit</i> – a number of rows to train over. A number less than the original table length will randomly subset the specified number of rows
 - <i>drop_null</i> – whether to drop rows with at least one missing value
 - <i>batch_size</i> – if specified, the training is split into batches. This can save the RAM
 - <i>print_report</i> - whether to generate accuracy and sampling reports. Please note that the sampling report is generated only if the `row_limit` parameter is set.
-- <i>metadata_path</i> – a path to the metadata file containing the metadata for linked tables
+- <i>metadata_path</i> – a path to the metadata file containing the metadata
 - <i>column_types</i> - might include the section <i>categorical</i> which contains the listed columns defined as categorical by a user
 
 Requirements for parameters of training process:
 * <i>source</i> - data type - string
 * <i>table_name</i> - data type - string
 * <i>epochs</i> - data type - integer, must be equal to or more than 1, default value is 10
 * <i>row_limit</i> - data type - integer
@@ -116,29 +116,29 @@
     --table_name STR \
     --run_parallel BOOL \
     --batch_size INT \
     --random_seed INT \
     --print_report BOOL
 ```
  
-For linked tables you can simply call:
+To generate one or more tables using a metadata file, you can use the following command:
 
 ```bash
 infer --metadata_path PATH_TO_METADATA
 ```
 
 The parameters which you can set up for generation process:
 
 - <i>size</i> - the desired number of rows to generate
 - <i>table_name</i> – required parameter for inference of single table, the name of the table, same as in training
 - <i>run_parallel</i> – whether to use multiprocessing (feasible for tables > 5000 rows)
 - <i>batch_size</i> – if specified, the generation is split into batches. This can save the RAM
 - <i>random_seed</i> – if specified, generates a reproducible result
 - <i>print_report</i> – whether to generate accuracy and sampling reports. Please note that the sampling report is generated only if the row_limit parameter is set.
-- <i>metadata_path</i> – a path to metadata file to generate linked tables
+- <i>metadata_path</i> – a path to metadata file
 
 Requirements for parameters of generation process:
 * <i>size</i> - data type - integer, must be equal to or more than 1, default value is 100
 * <i>table_name</i> - data type - string
 * <i>run_parallel</i> - data type - boolean, default value is False
 * <i>batch_size</i> - data type - integer, must be equal to or more than 1
 * <i>random_seed</i> - data type - integer, must be equal to or more than 0
@@ -147,41 +147,45 @@
 
 The metadata can contain any of the arguments above for each table. If so, the duplicated arguments from the CLI 
 will be ignored.
 
 
 ### Linked tables generation
 
-To generate linked tables, you should provide metadata in yaml format. It is used to handle complex 
-relations for any number of tables. You can also specify additional parameters needed for training and inference in the metadata file 
-and in this case, they will be ignored in the CLI call.
+To generate one or more tables, you might provide metadata in yaml format. By providing information about the relationships 
+between tables via metadata, it becomes possible to manage complex relationships across any number of tables. 
+You can also specify additional parameters needed for training and inference in the metadata file and in this case, 
+they will be ignored in the CLI call.
+
+<i>Note:</i> By using metadata file, you can also generate tables with absent relationships. 
+In this case, the tables will be generated independently.
 
 The yaml metadata file should match the following template:
 
-    CUSTOMER:                                       # Table name
-        source: "./files/customer.csv"              # Supported formats include local files in CSV, Avro formats
+    CUSTOMER:                                       # Table name. Required parameter
+        source: "./files/customer.csv"              # Supported formats include local files in CSV, Avro formats. Required parameter
                  
-        train_settings:                             # Settings for training process
-            epochs: 10                              # Number of epochs if different from the default in the command line options
-            drop_null: False                        # Drop rows with NULL values
-            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number
-            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM
-            print_report: False                     # Turn on or turn off generation of the report
+        train_settings:                             # Settings for training process. Optional parameter
+            epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
+            drop_null: False                        # Drop rows with NULL values. Optional parameter
+            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
+            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
+            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
             column_types:
-                categorical:                        # Force listed columns to have categorical type (use dictionary of values)
+                categorical:                        # Force listed columns to have categorical type (use dictionary of values). Optional parameter
                     - gender
                     - marital_status
                  
-        infer_settings:                             # Settings for infer process
-            size: 100                               # Size for generated data
-            run_parallel: False                     # Turn on or turn off parallel training process
-            print_report: False                     # Turn on or turn off generation of the report
-            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM
-            random_seed: None                       # If specified, generates a reproducible result
-        keys:
+        infer_settings:                             # Settings for infer process. Optional parameter
+            size: 100                               # Size for generated data. Optional parameter
+            run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
+            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
+            random_seed: None                       # If specified, generates a reproducible result. Optional parameter
+        keys:                                       # Keys of the table. Optional parameter
             PK_CUSTOMER_ID:                         # Name of a key. Only one PK per table.
                 type: "PK"                          # The key type. Supported: PK - primary key, FK - foreign key, TKN - token key
                 columns:                            # Array of column names
                     - customer_id
      
             UQ1:                                    # Name of a key
                 type: "UQ"                          # One or many unique keys
@@ -205,35 +209,35 @@
                     - address_id
                 references:
                     table: "ADDRESS"
                     columns:
                         - address_id
 
      
-    ORDER:
-        source: "./files/order.csv"
+    ORDER:                                          # Table name. Required parameter
+        source: "./files/order.csv"                 # Supported formats include local files in CSV, Avro formats. Required parameter
      
-        train_settings:
-            epochs: 10                              # Number of epochs if different from the default in the command line options
-            drop_null: False                        # Drop rows with NULL values
-            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number
-            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM
-            print_report: False                     # Turn on or turn off generation of the report
+        train_settings:                             # Settings for training process. Optional parameter
+            epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
+            drop_null: False                        # Drop rows with NULL values. Optional parameter
+            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
+            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
+            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
             column_types:
-                categorical:                        # Force listed columns to have categorical type (use dictionary of values)
+                categorical:                        # Force listed columns to have categorical type (use dictionary of values). Optional parameter
                     - gender
                     - marital_status
      
-        infer_settings:                             # Settings for infer process
-            size: 100                               # Size for generated data
-            run_parallel: False                     # Turn on or turn off parallel training process
-            print_report: False                     # Turn on or turn off generation of the report
-            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM
-            random_seed: None                       # If specified, generates a reproducible result
-        keys:
+        infer_settings:                             # Settings for infer process. Optional parameter
+            size: 100                               # Size for generated data. Optional parameter
+            run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
+            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
+            random_seed: None                       # If specified, generates a reproducible result. Optional parameter
+        keys:                                       # Keys of the table. Optional parameter
             pk_order_id:
                 type: "PK"
                 columns:
                     - order_id
      
             FK1:
                 type: "FK"
@@ -242,15 +246,15 @@
                 references:
                     table: "CUSTOMER"
                     columns:
                         - customer_id
 
 <i>You can find the example of metadata file in [example-metadata/housing_metadata.yaml](example-metadata/housing_metadata.yaml)</i><br>
 
-For related tables training you can use the commands:
+By providing the necessary information through a metadata file, you can initiate training and inference processes using the following commands:
 
 ```bash
 train --metadata_path=PATH_TO_YAML_METADATA_FILE
 infer --metadata_path=PATH_TO_YAML_METADATA_FILE
 ```
 Here is a quick example:
 
@@ -284,15 +288,15 @@
   --table_name=TABLE_NAME
 ```
 
 PATH_TO_LOCAL_FOLDER is an absolute path to the folder where your original csv is stored.
 
 You can add any arguments listed in the corresponding sections for infer and training processes in the CLI call.
 
-To run dockerized code for linked tables simply call:
+To run dockerized code by providing the metadata file simply call:
 
 ```bash
 docker pull tdspora/syngen-train:latest
 docker run --rm \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-train \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.1.4 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.1.5 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
@@ -31,104 +31,120 @@
 data/housing.csv â-table_name Housing infer --table_name Housing ``` As the
 example you can use the dataset "Housing" in [example-data/housing.csv]
 (example-data/housing.csv). In this example, our real-world data is "Housing"
 from Kaggle. ## Features ### Training You can add flexibility to the training
 and inference processes using additional hyperparameters.
 For training of single table call: ```bash train --source PATH_TO_ORIGINAL_CSV
 \ --table_name TABLE_NAME \ --epochs INT \ --row_limit INT \ --drop_null BOOL \
---print_report BOOL \ --batch_size INT ``` For training of the multiple linked
-tables call: ```bash train --metadata_path PATH_TO_METADATA_YAML ``` The
-parameters which you can set up for training process: - source â required
-parameter for training of single table, a path to the file that you want to use
-as a reference - table_name â required parameter for training of single
-table, an arbitrary string to name the directories - epochs â a number of
-training epochs. Since the early stopping mechanism is implemented the bigger
-value of epochs is the better - row_limit â a number of rows to train over. A
-number less than the original table length will randomly subset the specified
-number of rows - drop_null â whether to drop rows with at least one missing
-value - batch_size â if specified, the training is split into batches. This
-can save the RAM - print_report - whether to generate accuracy and sampling
-reports. Please note that the sampling report is generated only if the
-`row_limit` parameter is set. - metadata_path â a path to the metadata file
-containing the metadata for linked tables - column_types - might include the
-section categorical which contains the listed columns defined as categorical by
-a user Requirements for parameters of training process: * source - data type -
-string * table_name - data type - string * epochs - data type - integer, must
-be equal to or more than 1, default value is 10 * row_limit - data type -
-integer * drop_null - data type - boolean, default value - False * batch_size -
-data type - integer, must be equal to or more than 1, default value - 32 *
-print_report - data type - boolean, default value is False * metadata_path -
-data type - string * column_types - data type - dictionary with the key
-categorical - the list of columns (data type - string) ### Inference
-(generation) You can customize the inference processes by calling for one
-table: ```bash infer --size INT \ --table_name STR \ --run_parallel BOOL \ --
-batch_size INT \ --random_seed INT \ --print_report BOOL ``` For linked tables
-you can simply call: ```bash infer --metadata_path PATH_TO_METADATA ``` The
-parameters which you can set up for generation process: - size - the desired
-number of rows to generate - table_name â required parameter for inference of
-single table, the name of the table, same as in training - run_parallel â
-whether to use multiprocessing (feasible for tables > 5000 rows) - batch_size
-â if specified, the generation is split into batches. This can save the RAM -
-random_seed â if specified, generates a reproducible result - print_report
-â whether to generate accuracy and sampling reports. Please note that the
-sampling report is generated only if the row_limit parameter is set. -
-metadata_path â a path to metadata file to generate linked tables
+--print_report BOOL \ --batch_size INT ``` To train one or more tables using a
+metadata file, you can use the following command: ```bash train --metadata_path
+PATH_TO_METADATA_YAML ``` The parameters which you can set up for training
+process: - source â required parameter for training of single table, a path
+to the file that you want to use as a reference - table_name â required
+parameter for training of single table, an arbitrary string to name the
+directories - epochs â a number of training epochs. Since the early stopping
+mechanism is implemented the bigger value of epochs is the better - row_limit
+â a number of rows to train over. A number less than the original table
+length will randomly subset the specified number of rows - drop_null â
+whether to drop rows with at least one missing value - batch_size â if
+specified, the training is split into batches. This can save the RAM -
+print_report - whether to generate accuracy and sampling reports. Please note
+that the sampling report is generated only if the `row_limit` parameter is set.
+- metadata_path â a path to the metadata file containing the metadata -
+column_types - might include the section categorical which contains the listed
+columns defined as categorical by a user Requirements for parameters of
+training process: * source - data type - string * table_name - data type -
+string * epochs - data type - integer, must be equal to or more than 1, default
+value is 10 * row_limit - data type - integer * drop_null - data type -
+boolean, default value - False * batch_size - data type - integer, must be
+equal to or more than 1, default value - 32 * print_report - data type -
+boolean, default value is False * metadata_path - data type - string *
+column_types - data type - dictionary with the key categorical - the list of
+columns (data type - string) ### Inference (generation) You can customize the
+inference processes by calling for one table: ```bash infer --size INT \ --
+table_name STR \ --run_parallel BOOL \ --batch_size INT \ --random_seed INT \ -
+-print_report BOOL ``` To generate one or more tables using a metadata file,
+you can use the following command: ```bash infer --metadata_path
+PATH_TO_METADATA ``` The parameters which you can set up for generation
+process: - size - the desired number of rows to generate - table_name â
+required parameter for inference of single table, the name of the table, same
+as in training - run_parallel â whether to use multiprocessing (feasible for
+tables > 5000 rows) - batch_size â if specified, the generation is split into
+batches. This can save the RAM - random_seed â if specified, generates a
+reproducible result - print_report â whether to generate accuracy and
+sampling reports. Please note that the sampling report is generated only if the
+row_limit parameter is set. - metadata_path â a path to metadata file
 Requirements for parameters of generation process: * size - data type -
 integer, must be equal to or more than 1, default value is 100 * table_name -
 data type - string * run_parallel - data type - boolean, default value is False
 * batch_size - data type - integer, must be equal to or more than 1 *
 random_seed - data type - integer, must be equal to or more than 0 *
 print_report - data type - boolean, default value is False * metadata_path -
 data type - string The metadata can contain any of the arguments above for each
 table. If so, the duplicated arguments from the CLI will be ignored. ### Linked
-tables generation To generate linked tables, you should provide metadata in
-yaml format. It is used to handle complex relations for any number of tables.
-You can also specify additional parameters needed for training and inference in
-the metadata file and in this case, they will be ignored in the CLI call. The
-yaml metadata file should match the following template: CUSTOMER: # Table name
-source: "./files/customer.csv" # Supported formats include local files in CSV,
-Avro formats train_settings: # Settings for training process epochs: 10 #
-Number of epochs if different from the default in the command line options
-drop_null: False # Drop rows with NULL values row_limit: None # Number of rows
-to train over. A number less than the original table length will randomly
-subset the specified rows number batch_size: 32 # If specified, the training is
-split into batches. This can save the RAM print_report: False # Turn on or turn
-off generation of the report column_types: categorical: # Force listed columns
-to have categorical type (use dictionary of values) - gender - marital_status
-infer_settings: # Settings for infer process size: 100 # Size for generated
-data run_parallel: False # Turn on or turn off parallel training process
-print_report: False # Turn on or turn off generation of the report batch_size:
+tables generation To generate one or more tables, you might provide metadata in
+yaml format. By providing information about the relationships between tables
+via metadata, it becomes possible to manage complex relationships across any
+number of tables. You can also specify additional parameters needed for
+training and inference in the metadata file and in this case, they will be
+ignored in the CLI call. Note: By using metadata file, you can also generate
+tables with absent relationships. In this case, the tables will be generated
+independently. The yaml metadata file should match the following template:
+CUSTOMER: # Table name. Required parameter source: "./files/customer.csv" #
+Supported formats include local files in CSV, Avro formats. Required parameter
+train_settings: # Settings for training process. Optional parameter epochs: 10
+# Number of epochs if different from the default in the command line options.
+Optional parameter drop_null: False # Drop rows with NULL values. Optional
+parameter row_limit: None # Number of rows to train over. A number less than
+the original table length will randomly subset the specified rows number.
+Optional parameter batch_size: 32 # If specified, the training is split into
+batches. This can save the RAM. Optional parameter print_report: False # Turn
+on or turn off generation of the report. Optional parameter column_types:
+categorical: # Force listed columns to have categorical type (use dictionary of
+values). Optional parameter - gender - marital_status infer_settings: #
+Settings for infer process. Optional parameter size: 100 # Size for generated
+data. Optional parameter run_parallel: False # Turn on or turn off parallel
+training process. Optional parameter print_report: False # Turn on or turn off
+generation of the report. Optional parameter batch_size: None # If specified,
+the generation is split into batches. This can save the RAM. Optional parameter
+random_seed: None # If specified, generates a reproducible result. Optional
+parameter keys: # Keys of the table. Optional parameter PK_CUSTOMER_ID: # Name
+of a key. Only one PK per table. type: "PK" # The key type. Supported: PK -
+primary key, FK - foreign key, TKN - token key columns: # Array of column names
+- customer_id UQ1: # Name of a key type: "UQ" # One or many unique keys
+columns: - e_mail FK1: # One or many foreign keys type: "FK" columns: # Array
+of columns in the current table - e_mail - alias references: table: "PROFILE" #
+Name of the parent table columns: # Array of columns in the parent table -
+e_mail - alias FK2: type: "FK" columns: - address_id references: table:
+"ADDRESS" columns: - address_id ORDER: # Table name. Required parameter source:
+"./files/order.csv" # Supported formats include local files in CSV, Avro
+formats. Required parameter train_settings: # Settings for training process.
+Optional parameter epochs: 10 # Number of epochs if different from the default
+in the command line options. Optional parameter drop_null: False # Drop rows
+with NULL values. Optional parameter row_limit: None # Number of rows to train
+over. A number less than the original table length will randomly subset the
+specified rows number. Optional parameter batch_size: 32 # If specified, the
+training is split into batches. This can save the RAM. Optional parameter
+print_report: False # Turn on or turn off generation of the report. Optional
+parameter column_types: categorical: # Force listed columns to have categorical
+type (use dictionary of values). Optional parameter - gender - marital_status
+infer_settings: # Settings for infer process. Optional parameter size: 100 #
+Size for generated data. Optional parameter run_parallel: False # Turn on or
+turn off parallel training process. Optional parameter print_report: False #
+Turn on or turn off generation of the report. Optional parameter batch_size:
 None # If specified, the generation is split into batches. This can save the
-RAM random_seed: None # If specified, generates a reproducible result keys:
-PK_CUSTOMER_ID: # Name of a key. Only one PK per table. type: "PK" # The key
-type. Supported: PK - primary key, FK - foreign key, TKN - token key columns: #
-Array of column names - customer_id UQ1: # Name of a key type: "UQ" # One or
-many unique keys columns: - e_mail FK1: # One or many foreign keys type: "FK"
-columns: # Array of columns in the current table - e_mail - alias references:
-table: "PROFILE" # Name of the parent table columns: # Array of columns in the
-parent table - e_mail - alias FK2: type: "FK" columns: - address_id references:
-table: "ADDRESS" columns: - address_id ORDER: source: "./files/order.csv"
-train_settings: epochs: 10 # Number of epochs if different from the default in
-the command line options drop_null: False # Drop rows with NULL values
-row_limit: None # Number of rows to train over. A number less than the original
-table length will randomly subset the specified rows number batch_size: 32 # If
-specified, the training is split into batches. This can save the RAM
-print_report: False # Turn on or turn off generation of the report
-column_types: categorical: # Force listed columns to have categorical type (use
-dictionary of values) - gender - marital_status infer_settings: # Settings for
-infer process size: 100 # Size for generated data run_parallel: False # Turn on
-or turn off parallel training process print_report: False # Turn on or turn off
-generation of the report batch_size: None # If specified, the generation is
-split into batches. This can save the RAM random_seed: None # If specified,
-generates a reproducible result keys: pk_order_id: type: "PK" columns: -
-order_id FK1: type: "FK" columns: - customer_id references: table: "CUSTOMER"
-columns: - customer_id You can find the example of metadata file in [example-
-metadata/housing_metadata.yaml](example-metadata/housing_metadata.yaml)
-For related tables training you can use the commands: ```bash train --
-metadata_path=PATH_TO_YAML_METADATA_FILE infer --
+RAM. Optional parameter random_seed: None # If specified, generates a
+reproducible result. Optional parameter keys: # Keys of the table. Optional
+parameter pk_order_id: type: "PK" columns: - order_id FK1: type: "FK" columns:
+- customer_id references: table: "CUSTOMER" columns: - customer_id You can find
+the example of metadata file in [example-metadata/housing_metadata.yaml]
+(example-metadata/housing_metadata.yaml)
+By providing the necessary information through a metadata file, you can
+initiate training and inference processes using the following commands: ```bash
+train --metadata_path=PATH_TO_YAML_METADATA_FILE infer --
 metadata_path=PATH_TO_YAML_METADATA_FILE ``` Here is a quick example: ```bash
 train --metadata_path="./example-metadata/housing_metadata.yaml" infer --
 metadata_path="./example-metadata/housing_metadata.yaml" ``` If `--
 metadata_path` is present and the metadata contains the necessary parameters,
 other CLI parameters will be ignored.
 ### Docker images The train and inference components of syngen is available as
 public docker images:
@@ -138,30 +154,30 @@
 docker pull tdspora/syngen-train:latest docker run --rm \ -
 v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-train \ --
 table_name=TABLE_NAME \ --source=./model_artifacts/YOUR_CSV_FILE.csv docker
 pull tdspora/syngen-infer:latest docker run --rm \ -v PATH_TO_LOCAL_FOLDER:/
 src/model_artifacts tdspora/syngen-infer \ --table_name=TABLE_NAME ```
 PATH_TO_LOCAL_FOLDER is an absolute path to the folder where your original csv
 is stored. You can add any arguments listed in the corresponding sections for
-infer and training processes in the CLI call. To run dockerized code for linked
-tables simply call: ```bash docker pull tdspora/syngen-train:latest docker run
---rm \ -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-train \ --
-metadata_path=./model_artifacts/PATH_TO_METADATA_YAML docker pull tdspora/
-syngen-infer:latest docker run --rm \ -v PATH_TO_LOCAL_FOLDER:/src/
-model_artifacts tdspora/syngen-infer \ --metadata_path=./model_artifacts/
-PATH_TO_METADATA_YAML ``` You can add any arguments listed in the corresponding
-sections for infer and training processes in the CLI call, however, they will
-be overwritten by corresponding arguments in the metadata file. ## Contribution
-We welcome contributions from the community to help us improve and maintain our
-public GitHub repository. We appreciate any feedback, bug reports, or feature
-requests, and we encourage developers to submit fixes or new features using
-issues. If you have found a bug or have a feature request, please submit an
-issue to our GitHub repository. Please provide as much detail as possible,
-including steps to reproduce the issue or a clear description of the feature
-request. Our team will review the issue and work with you to address any
-problems or discuss any potential new features. If you would like to contribute
-a fix or a new feature, please submit a pull request to our GitHub repository.
-Please make sure your code follows our coding standards and best practices. Our
-team will review your pull request and work with you to ensure that it meets
-our standards and is ready for inclusion in our codebase. We appreciate your
-contributions and thank you for your interest in helping us maintain and
-improve our public GitHub repository.
+infer and training processes in the CLI call. To run dockerized code by
+providing the metadata file simply call: ```bash docker pull tdspora/syngen-
+train:latest docker run --rm \ -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts
+tdspora/syngen-train \ --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
+docker pull tdspora/syngen-infer:latest docker run --rm \ -
+v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-infer \ --
+metadata_path=./model_artifacts/PATH_TO_METADATA_YAML ``` You can add any
+arguments listed in the corresponding sections for infer and training processes
+in the CLI call, however, they will be overwritten by corresponding arguments
+in the metadata file. ## Contribution We welcome contributions from the
+community to help us improve and maintain our public GitHub repository. We
+appreciate any feedback, bug reports, or feature requests, and we encourage
+developers to submit fixes or new features using issues. If you have found a
+bug or have a feature request, please submit an issue to our GitHub repository.
+Please provide as much detail as possible, including steps to reproduce the
+issue or a clear description of the feature request. Our team will review the
+issue and work with you to address any problems or discuss any potential new
+features. If you would like to contribute a fix or a new feature, please submit
+a pull request to our GitHub repository. Please make sure your code follows our
+coding standards and best practices. Our team will review your pull request and
+work with you to ensure that it meets our standards and is ready for inclusion
+in our codebase. We appreciate your contributions and thank you for your
+interest in helping us maintain and improve our public GitHub repository.
```

### Comparing `syngen-0.1.4/README.md` & `syngen-0.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -54,30 +54,30 @@
     --epochs INT \
     --row_limit INT \
     --drop_null BOOL \
     --print_report BOOL \
     --batch_size INT
 ```
 
-For training of the multiple linked tables call:
+To train one or more tables using a metadata file, you can use the following command:
 
 ```bash
 train --metadata_path PATH_TO_METADATA_YAML
 ```
 
 The parameters which you can set up for training process:
 
 - <i>source</i> – required parameter for training of single table, a path to the file that you want to use as a reference
 - <i>table_name</i> – required parameter for training of single table, an arbitrary string to name the directories 
 - <i>epochs</i> – a number of training epochs. Since the early stopping mechanism is implemented the bigger value of epochs is the better
 - <i>row_limit</i> – a number of rows to train over. A number less than the original table length will randomly subset the specified number of rows
 - <i>drop_null</i> – whether to drop rows with at least one missing value
 - <i>batch_size</i> – if specified, the training is split into batches. This can save the RAM
 - <i>print_report</i> - whether to generate accuracy and sampling reports. Please note that the sampling report is generated only if the `row_limit` parameter is set.
-- <i>metadata_path</i> – a path to the metadata file containing the metadata for linked tables
+- <i>metadata_path</i> – a path to the metadata file containing the metadata
 - <i>column_types</i> - might include the section <i>categorical</i> which contains the listed columns defined as categorical by a user
 
 Requirements for parameters of training process:
 * <i>source</i> - data type - string
 * <i>table_name</i> - data type - string
 * <i>epochs</i> - data type - integer, must be equal to or more than 1, default value is 10
 * <i>row_limit</i> - data type - integer
@@ -97,29 +97,29 @@
     --table_name STR \
     --run_parallel BOOL \
     --batch_size INT \
     --random_seed INT \
     --print_report BOOL
 ```
  
-For linked tables you can simply call:
+To generate one or more tables using a metadata file, you can use the following command:
 
 ```bash
 infer --metadata_path PATH_TO_METADATA
 ```
 
 The parameters which you can set up for generation process:
 
 - <i>size</i> - the desired number of rows to generate
 - <i>table_name</i> – required parameter for inference of single table, the name of the table, same as in training
 - <i>run_parallel</i> – whether to use multiprocessing (feasible for tables > 5000 rows)
 - <i>batch_size</i> – if specified, the generation is split into batches. This can save the RAM
 - <i>random_seed</i> – if specified, generates a reproducible result
 - <i>print_report</i> – whether to generate accuracy and sampling reports. Please note that the sampling report is generated only if the row_limit parameter is set.
-- <i>metadata_path</i> – a path to metadata file to generate linked tables
+- <i>metadata_path</i> – a path to metadata file
 
 Requirements for parameters of generation process:
 * <i>size</i> - data type - integer, must be equal to or more than 1, default value is 100
 * <i>table_name</i> - data type - string
 * <i>run_parallel</i> - data type - boolean, default value is False
 * <i>batch_size</i> - data type - integer, must be equal to or more than 1
 * <i>random_seed</i> - data type - integer, must be equal to or more than 0
@@ -128,41 +128,45 @@
 
 The metadata can contain any of the arguments above for each table. If so, the duplicated arguments from the CLI 
 will be ignored.
 
 
 ### Linked tables generation
 
-To generate linked tables, you should provide metadata in yaml format. It is used to handle complex 
-relations for any number of tables. You can also specify additional parameters needed for training and inference in the metadata file 
-and in this case, they will be ignored in the CLI call.
+To generate one or more tables, you might provide metadata in yaml format. By providing information about the relationships 
+between tables via metadata, it becomes possible to manage complex relationships across any number of tables. 
+You can also specify additional parameters needed for training and inference in the metadata file and in this case, 
+they will be ignored in the CLI call.
+
+<i>Note:</i> By using metadata file, you can also generate tables with absent relationships. 
+In this case, the tables will be generated independently.
 
 The yaml metadata file should match the following template:
 
-    CUSTOMER:                                       # Table name
-        source: "./files/customer.csv"              # Supported formats include local files in CSV, Avro formats
+    CUSTOMER:                                       # Table name. Required parameter
+        source: "./files/customer.csv"              # Supported formats include local files in CSV, Avro formats. Required parameter
                  
-        train_settings:                             # Settings for training process
-            epochs: 10                              # Number of epochs if different from the default in the command line options
-            drop_null: False                        # Drop rows with NULL values
-            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number
-            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM
-            print_report: False                     # Turn on or turn off generation of the report
+        train_settings:                             # Settings for training process. Optional parameter
+            epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
+            drop_null: False                        # Drop rows with NULL values. Optional parameter
+            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
+            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
+            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
             column_types:
-                categorical:                        # Force listed columns to have categorical type (use dictionary of values)
+                categorical:                        # Force listed columns to have categorical type (use dictionary of values). Optional parameter
                     - gender
                     - marital_status
                  
-        infer_settings:                             # Settings for infer process
-            size: 100                               # Size for generated data
-            run_parallel: False                     # Turn on or turn off parallel training process
-            print_report: False                     # Turn on or turn off generation of the report
-            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM
-            random_seed: None                       # If specified, generates a reproducible result
-        keys:
+        infer_settings:                             # Settings for infer process. Optional parameter
+            size: 100                               # Size for generated data. Optional parameter
+            run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
+            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
+            random_seed: None                       # If specified, generates a reproducible result. Optional parameter
+        keys:                                       # Keys of the table. Optional parameter
             PK_CUSTOMER_ID:                         # Name of a key. Only one PK per table.
                 type: "PK"                          # The key type. Supported: PK - primary key, FK - foreign key, TKN - token key
                 columns:                            # Array of column names
                     - customer_id
      
             UQ1:                                    # Name of a key
                 type: "UQ"                          # One or many unique keys
@@ -186,35 +190,35 @@
                     - address_id
                 references:
                     table: "ADDRESS"
                     columns:
                         - address_id
 
      
-    ORDER:
-        source: "./files/order.csv"
+    ORDER:                                          # Table name. Required parameter
+        source: "./files/order.csv"                 # Supported formats include local files in CSV, Avro formats. Required parameter
      
-        train_settings:
-            epochs: 10                              # Number of epochs if different from the default in the command line options
-            drop_null: False                        # Drop rows with NULL values
-            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number
-            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM
-            print_report: False                     # Turn on or turn off generation of the report
+        train_settings:                             # Settings for training process. Optional parameter
+            epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
+            drop_null: False                        # Drop rows with NULL values. Optional parameter
+            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
+            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
+            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
             column_types:
-                categorical:                        # Force listed columns to have categorical type (use dictionary of values)
+                categorical:                        # Force listed columns to have categorical type (use dictionary of values). Optional parameter
                     - gender
                     - marital_status
      
-        infer_settings:                             # Settings for infer process
-            size: 100                               # Size for generated data
-            run_parallel: False                     # Turn on or turn off parallel training process
-            print_report: False                     # Turn on or turn off generation of the report
-            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM
-            random_seed: None                       # If specified, generates a reproducible result
-        keys:
+        infer_settings:                             # Settings for infer process. Optional parameter
+            size: 100                               # Size for generated data. Optional parameter
+            run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
+            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
+            random_seed: None                       # If specified, generates a reproducible result. Optional parameter
+        keys:                                       # Keys of the table. Optional parameter
             pk_order_id:
                 type: "PK"
                 columns:
                     - order_id
      
             FK1:
                 type: "FK"
@@ -223,15 +227,15 @@
                 references:
                     table: "CUSTOMER"
                     columns:
                         - customer_id
 
 <i>You can find the example of metadata file in [example-metadata/housing_metadata.yaml](example-metadata/housing_metadata.yaml)</i><br>
 
-For related tables training you can use the commands:
+By providing the necessary information through a metadata file, you can initiate training and inference processes using the following commands:
 
 ```bash
 train --metadata_path=PATH_TO_YAML_METADATA_FILE
 infer --metadata_path=PATH_TO_YAML_METADATA_FILE
 ```
 Here is a quick example:
 
@@ -265,15 +269,15 @@
   --table_name=TABLE_NAME
 ```
 
 PATH_TO_LOCAL_FOLDER is an absolute path to the folder where your original csv is stored.
 
 You can add any arguments listed in the corresponding sections for infer and training processes in the CLI call.
 
-To run dockerized code for linked tables simply call:
+To run dockerized code by providing the metadata file simply call:
 
 ```bash
 docker pull tdspora/syngen-train:latest
 docker run --rm \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-train \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
```

#### html2text {}

```diff
@@ -21,104 +21,120 @@
 data/housing.csv â-table_name Housing infer --table_name Housing ``` As the
 example you can use the dataset "Housing" in [example-data/housing.csv]
 (example-data/housing.csv). In this example, our real-world data is "Housing"
 from Kaggle. ## Features ### Training You can add flexibility to the training
 and inference processes using additional hyperparameters.
 For training of single table call: ```bash train --source PATH_TO_ORIGINAL_CSV
 \ --table_name TABLE_NAME \ --epochs INT \ --row_limit INT \ --drop_null BOOL \
---print_report BOOL \ --batch_size INT ``` For training of the multiple linked
-tables call: ```bash train --metadata_path PATH_TO_METADATA_YAML ``` The
-parameters which you can set up for training process: - source â required
-parameter for training of single table, a path to the file that you want to use
-as a reference - table_name â required parameter for training of single
-table, an arbitrary string to name the directories - epochs â a number of
-training epochs. Since the early stopping mechanism is implemented the bigger
-value of epochs is the better - row_limit â a number of rows to train over. A
-number less than the original table length will randomly subset the specified
-number of rows - drop_null â whether to drop rows with at least one missing
-value - batch_size â if specified, the training is split into batches. This
-can save the RAM - print_report - whether to generate accuracy and sampling
-reports. Please note that the sampling report is generated only if the
-`row_limit` parameter is set. - metadata_path â a path to the metadata file
-containing the metadata for linked tables - column_types - might include the
-section categorical which contains the listed columns defined as categorical by
-a user Requirements for parameters of training process: * source - data type -
-string * table_name - data type - string * epochs - data type - integer, must
-be equal to or more than 1, default value is 10 * row_limit - data type -
-integer * drop_null - data type - boolean, default value - False * batch_size -
-data type - integer, must be equal to or more than 1, default value - 32 *
-print_report - data type - boolean, default value is False * metadata_path -
-data type - string * column_types - data type - dictionary with the key
-categorical - the list of columns (data type - string) ### Inference
-(generation) You can customize the inference processes by calling for one
-table: ```bash infer --size INT \ --table_name STR \ --run_parallel BOOL \ --
-batch_size INT \ --random_seed INT \ --print_report BOOL ``` For linked tables
-you can simply call: ```bash infer --metadata_path PATH_TO_METADATA ``` The
-parameters which you can set up for generation process: - size - the desired
-number of rows to generate - table_name â required parameter for inference of
-single table, the name of the table, same as in training - run_parallel â
-whether to use multiprocessing (feasible for tables > 5000 rows) - batch_size
-â if specified, the generation is split into batches. This can save the RAM -
-random_seed â if specified, generates a reproducible result - print_report
-â whether to generate accuracy and sampling reports. Please note that the
-sampling report is generated only if the row_limit parameter is set. -
-metadata_path â a path to metadata file to generate linked tables
+--print_report BOOL \ --batch_size INT ``` To train one or more tables using a
+metadata file, you can use the following command: ```bash train --metadata_path
+PATH_TO_METADATA_YAML ``` The parameters which you can set up for training
+process: - source â required parameter for training of single table, a path
+to the file that you want to use as a reference - table_name â required
+parameter for training of single table, an arbitrary string to name the
+directories - epochs â a number of training epochs. Since the early stopping
+mechanism is implemented the bigger value of epochs is the better - row_limit
+â a number of rows to train over. A number less than the original table
+length will randomly subset the specified number of rows - drop_null â
+whether to drop rows with at least one missing value - batch_size â if
+specified, the training is split into batches. This can save the RAM -
+print_report - whether to generate accuracy and sampling reports. Please note
+that the sampling report is generated only if the `row_limit` parameter is set.
+- metadata_path â a path to the metadata file containing the metadata -
+column_types - might include the section categorical which contains the listed
+columns defined as categorical by a user Requirements for parameters of
+training process: * source - data type - string * table_name - data type -
+string * epochs - data type - integer, must be equal to or more than 1, default
+value is 10 * row_limit - data type - integer * drop_null - data type -
+boolean, default value - False * batch_size - data type - integer, must be
+equal to or more than 1, default value - 32 * print_report - data type -
+boolean, default value is False * metadata_path - data type - string *
+column_types - data type - dictionary with the key categorical - the list of
+columns (data type - string) ### Inference (generation) You can customize the
+inference processes by calling for one table: ```bash infer --size INT \ --
+table_name STR \ --run_parallel BOOL \ --batch_size INT \ --random_seed INT \ -
+-print_report BOOL ``` To generate one or more tables using a metadata file,
+you can use the following command: ```bash infer --metadata_path
+PATH_TO_METADATA ``` The parameters which you can set up for generation
+process: - size - the desired number of rows to generate - table_name â
+required parameter for inference of single table, the name of the table, same
+as in training - run_parallel â whether to use multiprocessing (feasible for
+tables > 5000 rows) - batch_size â if specified, the generation is split into
+batches. This can save the RAM - random_seed â if specified, generates a
+reproducible result - print_report â whether to generate accuracy and
+sampling reports. Please note that the sampling report is generated only if the
+row_limit parameter is set. - metadata_path â a path to metadata file
 Requirements for parameters of generation process: * size - data type -
 integer, must be equal to or more than 1, default value is 100 * table_name -
 data type - string * run_parallel - data type - boolean, default value is False
 * batch_size - data type - integer, must be equal to or more than 1 *
 random_seed - data type - integer, must be equal to or more than 0 *
 print_report - data type - boolean, default value is False * metadata_path -
 data type - string The metadata can contain any of the arguments above for each
 table. If so, the duplicated arguments from the CLI will be ignored. ### Linked
-tables generation To generate linked tables, you should provide metadata in
-yaml format. It is used to handle complex relations for any number of tables.
-You can also specify additional parameters needed for training and inference in
-the metadata file and in this case, they will be ignored in the CLI call. The
-yaml metadata file should match the following template: CUSTOMER: # Table name
-source: "./files/customer.csv" # Supported formats include local files in CSV,
-Avro formats train_settings: # Settings for training process epochs: 10 #
-Number of epochs if different from the default in the command line options
-drop_null: False # Drop rows with NULL values row_limit: None # Number of rows
-to train over. A number less than the original table length will randomly
-subset the specified rows number batch_size: 32 # If specified, the training is
-split into batches. This can save the RAM print_report: False # Turn on or turn
-off generation of the report column_types: categorical: # Force listed columns
-to have categorical type (use dictionary of values) - gender - marital_status
-infer_settings: # Settings for infer process size: 100 # Size for generated
-data run_parallel: False # Turn on or turn off parallel training process
-print_report: False # Turn on or turn off generation of the report batch_size:
+tables generation To generate one or more tables, you might provide metadata in
+yaml format. By providing information about the relationships between tables
+via metadata, it becomes possible to manage complex relationships across any
+number of tables. You can also specify additional parameters needed for
+training and inference in the metadata file and in this case, they will be
+ignored in the CLI call. Note: By using metadata file, you can also generate
+tables with absent relationships. In this case, the tables will be generated
+independently. The yaml metadata file should match the following template:
+CUSTOMER: # Table name. Required parameter source: "./files/customer.csv" #
+Supported formats include local files in CSV, Avro formats. Required parameter
+train_settings: # Settings for training process. Optional parameter epochs: 10
+# Number of epochs if different from the default in the command line options.
+Optional parameter drop_null: False # Drop rows with NULL values. Optional
+parameter row_limit: None # Number of rows to train over. A number less than
+the original table length will randomly subset the specified rows number.
+Optional parameter batch_size: 32 # If specified, the training is split into
+batches. This can save the RAM. Optional parameter print_report: False # Turn
+on or turn off generation of the report. Optional parameter column_types:
+categorical: # Force listed columns to have categorical type (use dictionary of
+values). Optional parameter - gender - marital_status infer_settings: #
+Settings for infer process. Optional parameter size: 100 # Size for generated
+data. Optional parameter run_parallel: False # Turn on or turn off parallel
+training process. Optional parameter print_report: False # Turn on or turn off
+generation of the report. Optional parameter batch_size: None # If specified,
+the generation is split into batches. This can save the RAM. Optional parameter
+random_seed: None # If specified, generates a reproducible result. Optional
+parameter keys: # Keys of the table. Optional parameter PK_CUSTOMER_ID: # Name
+of a key. Only one PK per table. type: "PK" # The key type. Supported: PK -
+primary key, FK - foreign key, TKN - token key columns: # Array of column names
+- customer_id UQ1: # Name of a key type: "UQ" # One or many unique keys
+columns: - e_mail FK1: # One or many foreign keys type: "FK" columns: # Array
+of columns in the current table - e_mail - alias references: table: "PROFILE" #
+Name of the parent table columns: # Array of columns in the parent table -
+e_mail - alias FK2: type: "FK" columns: - address_id references: table:
+"ADDRESS" columns: - address_id ORDER: # Table name. Required parameter source:
+"./files/order.csv" # Supported formats include local files in CSV, Avro
+formats. Required parameter train_settings: # Settings for training process.
+Optional parameter epochs: 10 # Number of epochs if different from the default
+in the command line options. Optional parameter drop_null: False # Drop rows
+with NULL values. Optional parameter row_limit: None # Number of rows to train
+over. A number less than the original table length will randomly subset the
+specified rows number. Optional parameter batch_size: 32 # If specified, the
+training is split into batches. This can save the RAM. Optional parameter
+print_report: False # Turn on or turn off generation of the report. Optional
+parameter column_types: categorical: # Force listed columns to have categorical
+type (use dictionary of values). Optional parameter - gender - marital_status
+infer_settings: # Settings for infer process. Optional parameter size: 100 #
+Size for generated data. Optional parameter run_parallel: False # Turn on or
+turn off parallel training process. Optional parameter print_report: False #
+Turn on or turn off generation of the report. Optional parameter batch_size:
 None # If specified, the generation is split into batches. This can save the
-RAM random_seed: None # If specified, generates a reproducible result keys:
-PK_CUSTOMER_ID: # Name of a key. Only one PK per table. type: "PK" # The key
-type. Supported: PK - primary key, FK - foreign key, TKN - token key columns: #
-Array of column names - customer_id UQ1: # Name of a key type: "UQ" # One or
-many unique keys columns: - e_mail FK1: # One or many foreign keys type: "FK"
-columns: # Array of columns in the current table - e_mail - alias references:
-table: "PROFILE" # Name of the parent table columns: # Array of columns in the
-parent table - e_mail - alias FK2: type: "FK" columns: - address_id references:
-table: "ADDRESS" columns: - address_id ORDER: source: "./files/order.csv"
-train_settings: epochs: 10 # Number of epochs if different from the default in
-the command line options drop_null: False # Drop rows with NULL values
-row_limit: None # Number of rows to train over. A number less than the original
-table length will randomly subset the specified rows number batch_size: 32 # If
-specified, the training is split into batches. This can save the RAM
-print_report: False # Turn on or turn off generation of the report
-column_types: categorical: # Force listed columns to have categorical type (use
-dictionary of values) - gender - marital_status infer_settings: # Settings for
-infer process size: 100 # Size for generated data run_parallel: False # Turn on
-or turn off parallel training process print_report: False # Turn on or turn off
-generation of the report batch_size: None # If specified, the generation is
-split into batches. This can save the RAM random_seed: None # If specified,
-generates a reproducible result keys: pk_order_id: type: "PK" columns: -
-order_id FK1: type: "FK" columns: - customer_id references: table: "CUSTOMER"
-columns: - customer_id You can find the example of metadata file in [example-
-metadata/housing_metadata.yaml](example-metadata/housing_metadata.yaml)
-For related tables training you can use the commands: ```bash train --
-metadata_path=PATH_TO_YAML_METADATA_FILE infer --
+RAM. Optional parameter random_seed: None # If specified, generates a
+reproducible result. Optional parameter keys: # Keys of the table. Optional
+parameter pk_order_id: type: "PK" columns: - order_id FK1: type: "FK" columns:
+- customer_id references: table: "CUSTOMER" columns: - customer_id You can find
+the example of metadata file in [example-metadata/housing_metadata.yaml]
+(example-metadata/housing_metadata.yaml)
+By providing the necessary information through a metadata file, you can
+initiate training and inference processes using the following commands: ```bash
+train --metadata_path=PATH_TO_YAML_METADATA_FILE infer --
 metadata_path=PATH_TO_YAML_METADATA_FILE ``` Here is a quick example: ```bash
 train --metadata_path="./example-metadata/housing_metadata.yaml" infer --
 metadata_path="./example-metadata/housing_metadata.yaml" ``` If `--
 metadata_path` is present and the metadata contains the necessary parameters,
 other CLI parameters will be ignored.
 ### Docker images The train and inference components of syngen is available as
 public docker images:
@@ -128,30 +144,30 @@
 docker pull tdspora/syngen-train:latest docker run --rm \ -
 v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-train \ --
 table_name=TABLE_NAME \ --source=./model_artifacts/YOUR_CSV_FILE.csv docker
 pull tdspora/syngen-infer:latest docker run --rm \ -v PATH_TO_LOCAL_FOLDER:/
 src/model_artifacts tdspora/syngen-infer \ --table_name=TABLE_NAME ```
 PATH_TO_LOCAL_FOLDER is an absolute path to the folder where your original csv
 is stored. You can add any arguments listed in the corresponding sections for
-infer and training processes in the CLI call. To run dockerized code for linked
-tables simply call: ```bash docker pull tdspora/syngen-train:latest docker run
---rm \ -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-train \ --
-metadata_path=./model_artifacts/PATH_TO_METADATA_YAML docker pull tdspora/
-syngen-infer:latest docker run --rm \ -v PATH_TO_LOCAL_FOLDER:/src/
-model_artifacts tdspora/syngen-infer \ --metadata_path=./model_artifacts/
-PATH_TO_METADATA_YAML ``` You can add any arguments listed in the corresponding
-sections for infer and training processes in the CLI call, however, they will
-be overwritten by corresponding arguments in the metadata file. ## Contribution
-We welcome contributions from the community to help us improve and maintain our
-public GitHub repository. We appreciate any feedback, bug reports, or feature
-requests, and we encourage developers to submit fixes or new features using
-issues. If you have found a bug or have a feature request, please submit an
-issue to our GitHub repository. Please provide as much detail as possible,
-including steps to reproduce the issue or a clear description of the feature
-request. Our team will review the issue and work with you to address any
-problems or discuss any potential new features. If you would like to contribute
-a fix or a new feature, please submit a pull request to our GitHub repository.
-Please make sure your code follows our coding standards and best practices. Our
-team will review your pull request and work with you to ensure that it meets
-our standards and is ready for inclusion in our codebase. We appreciate your
-contributions and thank you for your interest in helping us maintain and
-improve our public GitHub repository.
+infer and training processes in the CLI call. To run dockerized code by
+providing the metadata file simply call: ```bash docker pull tdspora/syngen-
+train:latest docker run --rm \ -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts
+tdspora/syngen-train \ --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
+docker pull tdspora/syngen-infer:latest docker run --rm \ -
+v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-infer \ --
+metadata_path=./model_artifacts/PATH_TO_METADATA_YAML ``` You can add any
+arguments listed in the corresponding sections for infer and training processes
+in the CLI call, however, they will be overwritten by corresponding arguments
+in the metadata file. ## Contribution We welcome contributions from the
+community to help us improve and maintain our public GitHub repository. We
+appreciate any feedback, bug reports, or feature requests, and we encourage
+developers to submit fixes or new features using issues. If you have found a
+bug or have a feature request, please submit an issue to our GitHub repository.
+Please provide as much detail as possible, including steps to reproduce the
+issue or a clear description of the feature request. Our team will review the
+issue and work with you to address any problems or discuss any potential new
+features. If you would like to contribute a fix or a new feature, please submit
+a pull request to our GitHub repository. Please make sure your code follows our
+coding standards and best practices. Our team will review your pull request and
+work with you to ensure that it meets our standards and is ready for inclusion
+in our codebase. We appreciate your contributions and thank you for your
+interest in helping us maintain and improve our public GitHub repository.
```

### Comparing `syngen-0.1.4/setup.cfg` & `syngen-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/infer.py` & `syngen-0.1.5/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/config/configurations.py` & `syngen-0.1.5/src/syngen/ml/config/configurations.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/convertor/convertor.py` & `syngen-0.1.5/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.1.5/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     """
     Class for loading and saving data in YAML format
     """
     def load_data(self, metadata_path: str) -> dict:
         with open(metadata_path, "r", encoding="utf-8") as metadata_file:
             metadata = yaml.load(metadata_file, Loader=Loader)
             validate_schema(configuration_schema, metadata)
-            parameters = ["train_settings", "infer_settings"]
+            parameters = ["train_settings", "infer_settings", "keys"]
             metadata = self.replace_none_values_of_metadata_settings(parameters, metadata)
         return metadata
 
     @staticmethod
     def replace_none_values_of_metadata_settings(parameters, metadata: dict):
         """
         Replace None values for parameters
```

### Comparing `syngen-0.1.4/src/syngen/ml/metrics/__init__.py` & `syngen-0.1.5/src/syngen/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.1.5/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.1.5/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.1.5/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.1.5/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/metrics/utils.py` & `syngen-0.1.5/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/reporters/reporters.py` & `syngen-0.1.5/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/strategies/strategies.py` & `syngen-0.1.5/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/train_chain/train_chain.py` & `syngen-0.1.5/src/syngen/ml/train_chain/train_chain.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/utils/utils.py` & `syngen-0.1.5/src/syngen/ml/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.1.5/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/vae/models/dataset.py` & `syngen-0.1.5/src/syngen/ml/vae/models/dataset.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/vae/models/features.py` & `syngen-0.1.5/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/vae/models/model.py` & `syngen-0.1.5/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.1.5/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.1.5/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,27 @@
-from typing import Dict
+from typing import Dict, List
 
 from schema import Schema, Optional, And, Or, SchemaError
 from loguru import logger
 
 
+def keys_schema(types_of_keys: List[str]):
+    schema = {
+        str: {
+            "type": Or(*types_of_keys),
+            "columns": [str],
+            Optional("joined_sample"): bool
+        }
+    }
+    if schema[str]["type"] == "FK":
+        schema[str]["references"] = {"table": str, "columns": [str]}
+    else:
+        schema[str][Optional("references")] = {"table": str, "columns": [str]}
+    return schema
+
 configuration_schema = Schema({
     str: {
         Optional("train_settings"): Or(
             {
                 Optional("epochs"): And(int, lambda n: n >= 1),
                 Optional("drop_null"): bool,
                 Optional("row_limit"): And(int, lambda n: n >= 1),
@@ -26,28 +40,17 @@
                 Optional("batch_size"): And(int, lambda n: n >= 1),
                 Optional("random_seed"): And(int, lambda n: n >= 0),
                 Optional("print_report"): bool
             },
             None
         ),
         "source": str,
-        Optional("keys"): {
-            str: {
-                "type": Or("FK", "PK", "UQ"),
-                "columns": [str],
-                Optional("references"): {
-                    "table": str,
-                    "columns": [str]
-                },
-                Optional("joined_sample"): bool
-            }
-        }
+        Optional("keys"): Or(keys_schema(types_of_keys=["FK", "PK", "UQ"]), None)
     }
-}
-)
+})
 
 
 def validate_schema(configuration_schema: Schema, metadata: Dict):
     """
     Validate the metadata file regarding the configuration_schema
     :param configuration_schema: Schema
     :param metadata: Dict
```

### Comparing `syngen-0.1.4/src/syngen/ml/worker/worker.py` & `syngen-0.1.5/src/syngen/ml/worker/worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,28 @@
             "run_parallel": run_parallel,
             "random_seed": random_seed,
             "batch_size": batch_size,
             "print_report": print_report
         }
 
     @staticmethod
+    def _get_tables_without_keys(config_of_tables: Dict) -> List[str]:
+        """
+        Return the list of tables without the information about keys
+        """
+        tables_without_keys = []
+        for table in config_of_tables.keys():
+            if not config_of_tables[table].get("keys"):
+                tables_without_keys.append(table)
+        return tables_without_keys
+
+    @staticmethod
     def _get_tables(config: Dict, key_type: str):
         """
-        Return the list of related tables regarding to the type of key - 'primary key', 'foreign key'
+        Return the list of related tables regarding the type of key - 'primary key', 'foreign key'
         :param config: configuration of related tables declared in metadata.yaml file
         :param key_type: type of key either 'primary key' ('PK') or 'foreign key' ('FK')
         """
         try:
             tables = [table_name for table_name, config in config.items()
                       for key in config["keys"]
                       if config["keys"][key]["type"] == key_type]
@@ -98,25 +109,21 @@
         """
         Return the list of related tables for training or infer process,
         configuration of related tables
 
         type_of_process can be "train", "infer" or "all" for the Enterprise version
         """
         config_of_tables = deepcopy(self.metadata)
-        table_names = list(config_of_tables.keys())
-        if len(table_names) == 1 and "keys" not in config_of_tables[table_names[0]]:
-            # case with one table without any keys
-            chain_of_tables = table_names
-        else:
-            if kwargs.get("type_of_process") in ("infer", "all"):
-                config_of_tables = self._split_pk_fk_metadata(config_of_tables, list(config_of_tables.keys()))
-            pk_tables = self._get_tables(config_of_tables, "PK")
-            uq_tables = self._get_tables(config_of_tables, "UQ")
-            fk_tables = self._get_tables(config_of_tables, "FK")
-            chain_of_tables = list(dict.fromkeys([*pk_tables, *uq_tables, *fk_tables]))
+        tables_without_keys = self._get_tables_without_keys(config_of_tables)
+        if kwargs.get("type_of_process") in ("infer", "all"):
+            config_of_tables = self._split_pk_fk_metadata(config_of_tables, list(config_of_tables.keys()))
+        pk_tables = self._get_tables(config_of_tables, "PK")
+        uq_tables = self._get_tables(config_of_tables, "UQ")
+        fk_tables = self._get_tables(config_of_tables, "FK")
+        chain_of_tables = list(dict.fromkeys([*tables_without_keys, *pk_tables, *uq_tables, *fk_tables]))
 
         return chain_of_tables, config_of_tables
 
     def _split_pk_fk_metadata(self, config, tables):
         for table in tables:
             types_of_keys = [value["type"] for key, value in config[table]["keys"].items()]
             if "PK" in types_of_keys and "FK" in types_of_keys:
```

### Comparing `syngen-0.1.4/src/syngen/train.py` & `syngen-0.1.5/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.1.4/src/syngen.egg-info/PKG-INFO` & `syngen-0.1.5/src/syngen.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.1.4
+Version: 0.1.5
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -73,30 +73,30 @@
     --epochs INT \
     --row_limit INT \
     --drop_null BOOL \
     --print_report BOOL \
     --batch_size INT
 ```
 
-For training of the multiple linked tables call:
+To train one or more tables using a metadata file, you can use the following command:
 
 ```bash
 train --metadata_path PATH_TO_METADATA_YAML
 ```
 
 The parameters which you can set up for training process:
 
 - <i>source</i> – required parameter for training of single table, a path to the file that you want to use as a reference
 - <i>table_name</i> – required parameter for training of single table, an arbitrary string to name the directories 
 - <i>epochs</i> – a number of training epochs. Since the early stopping mechanism is implemented the bigger value of epochs is the better
 - <i>row_limit</i> – a number of rows to train over. A number less than the original table length will randomly subset the specified number of rows
 - <i>drop_null</i> – whether to drop rows with at least one missing value
 - <i>batch_size</i> – if specified, the training is split into batches. This can save the RAM
 - <i>print_report</i> - whether to generate accuracy and sampling reports. Please note that the sampling report is generated only if the `row_limit` parameter is set.
-- <i>metadata_path</i> – a path to the metadata file containing the metadata for linked tables
+- <i>metadata_path</i> – a path to the metadata file containing the metadata
 - <i>column_types</i> - might include the section <i>categorical</i> which contains the listed columns defined as categorical by a user
 
 Requirements for parameters of training process:
 * <i>source</i> - data type - string
 * <i>table_name</i> - data type - string
 * <i>epochs</i> - data type - integer, must be equal to or more than 1, default value is 10
 * <i>row_limit</i> - data type - integer
@@ -116,29 +116,29 @@
     --table_name STR \
     --run_parallel BOOL \
     --batch_size INT \
     --random_seed INT \
     --print_report BOOL
 ```
  
-For linked tables you can simply call:
+To generate one or more tables using a metadata file, you can use the following command:
 
 ```bash
 infer --metadata_path PATH_TO_METADATA
 ```
 
 The parameters which you can set up for generation process:
 
 - <i>size</i> - the desired number of rows to generate
 - <i>table_name</i> – required parameter for inference of single table, the name of the table, same as in training
 - <i>run_parallel</i> – whether to use multiprocessing (feasible for tables > 5000 rows)
 - <i>batch_size</i> – if specified, the generation is split into batches. This can save the RAM
 - <i>random_seed</i> – if specified, generates a reproducible result
 - <i>print_report</i> – whether to generate accuracy and sampling reports. Please note that the sampling report is generated only if the row_limit parameter is set.
-- <i>metadata_path</i> – a path to metadata file to generate linked tables
+- <i>metadata_path</i> – a path to metadata file
 
 Requirements for parameters of generation process:
 * <i>size</i> - data type - integer, must be equal to or more than 1, default value is 100
 * <i>table_name</i> - data type - string
 * <i>run_parallel</i> - data type - boolean, default value is False
 * <i>batch_size</i> - data type - integer, must be equal to or more than 1
 * <i>random_seed</i> - data type - integer, must be equal to or more than 0
@@ -147,41 +147,45 @@
 
 The metadata can contain any of the arguments above for each table. If so, the duplicated arguments from the CLI 
 will be ignored.
 
 
 ### Linked tables generation
 
-To generate linked tables, you should provide metadata in yaml format. It is used to handle complex 
-relations for any number of tables. You can also specify additional parameters needed for training and inference in the metadata file 
-and in this case, they will be ignored in the CLI call.
+To generate one or more tables, you might provide metadata in yaml format. By providing information about the relationships 
+between tables via metadata, it becomes possible to manage complex relationships across any number of tables. 
+You can also specify additional parameters needed for training and inference in the metadata file and in this case, 
+they will be ignored in the CLI call.
+
+<i>Note:</i> By using metadata file, you can also generate tables with absent relationships. 
+In this case, the tables will be generated independently.
 
 The yaml metadata file should match the following template:
 
-    CUSTOMER:                                       # Table name
-        source: "./files/customer.csv"              # Supported formats include local files in CSV, Avro formats
+    CUSTOMER:                                       # Table name. Required parameter
+        source: "./files/customer.csv"              # Supported formats include local files in CSV, Avro formats. Required parameter
                  
-        train_settings:                             # Settings for training process
-            epochs: 10                              # Number of epochs if different from the default in the command line options
-            drop_null: False                        # Drop rows with NULL values
-            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number
-            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM
-            print_report: False                     # Turn on or turn off generation of the report
+        train_settings:                             # Settings for training process. Optional parameter
+            epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
+            drop_null: False                        # Drop rows with NULL values. Optional parameter
+            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
+            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
+            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
             column_types:
-                categorical:                        # Force listed columns to have categorical type (use dictionary of values)
+                categorical:                        # Force listed columns to have categorical type (use dictionary of values). Optional parameter
                     - gender
                     - marital_status
                  
-        infer_settings:                             # Settings for infer process
-            size: 100                               # Size for generated data
-            run_parallel: False                     # Turn on or turn off parallel training process
-            print_report: False                     # Turn on or turn off generation of the report
-            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM
-            random_seed: None                       # If specified, generates a reproducible result
-        keys:
+        infer_settings:                             # Settings for infer process. Optional parameter
+            size: 100                               # Size for generated data. Optional parameter
+            run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
+            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
+            random_seed: None                       # If specified, generates a reproducible result. Optional parameter
+        keys:                                       # Keys of the table. Optional parameter
             PK_CUSTOMER_ID:                         # Name of a key. Only one PK per table.
                 type: "PK"                          # The key type. Supported: PK - primary key, FK - foreign key, TKN - token key
                 columns:                            # Array of column names
                     - customer_id
      
             UQ1:                                    # Name of a key
                 type: "UQ"                          # One or many unique keys
@@ -205,35 +209,35 @@
                     - address_id
                 references:
                     table: "ADDRESS"
                     columns:
                         - address_id
 
      
-    ORDER:
-        source: "./files/order.csv"
+    ORDER:                                          # Table name. Required parameter
+        source: "./files/order.csv"                 # Supported formats include local files in CSV, Avro formats. Required parameter
      
-        train_settings:
-            epochs: 10                              # Number of epochs if different from the default in the command line options
-            drop_null: False                        # Drop rows with NULL values
-            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number
-            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM
-            print_report: False                     # Turn on or turn off generation of the report
+        train_settings:                             # Settings for training process. Optional parameter
+            epochs: 10                              # Number of epochs if different from the default in the command line options. Optional parameter
+            drop_null: False                        # Drop rows with NULL values. Optional parameter
+            row_limit: None                         # Number of rows to train over. A number less than the original table length will randomly subset the specified rows number. Optional parameter
+            batch_size: 32                          # If specified, the training is split into batches. This can save the RAM. Optional parameter
+            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
             column_types:
-                categorical:                        # Force listed columns to have categorical type (use dictionary of values)
+                categorical:                        # Force listed columns to have categorical type (use dictionary of values). Optional parameter
                     - gender
                     - marital_status
      
-        infer_settings:                             # Settings for infer process
-            size: 100                               # Size for generated data
-            run_parallel: False                     # Turn on or turn off parallel training process
-            print_report: False                     # Turn on or turn off generation of the report
-            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM
-            random_seed: None                       # If specified, generates a reproducible result
-        keys:
+        infer_settings:                             # Settings for infer process. Optional parameter
+            size: 100                               # Size for generated data. Optional parameter
+            run_parallel: False                     # Turn on or turn off parallel training process. Optional parameter
+            print_report: False                     # Turn on or turn off generation of the report. Optional parameter
+            batch_size: None                        # If specified, the generation is split into batches. This can save the RAM. Optional parameter
+            random_seed: None                       # If specified, generates a reproducible result. Optional parameter
+        keys:                                       # Keys of the table. Optional parameter
             pk_order_id:
                 type: "PK"
                 columns:
                     - order_id
      
             FK1:
                 type: "FK"
@@ -242,15 +246,15 @@
                 references:
                     table: "CUSTOMER"
                     columns:
                         - customer_id
 
 <i>You can find the example of metadata file in [example-metadata/housing_metadata.yaml](example-metadata/housing_metadata.yaml)</i><br>
 
-For related tables training you can use the commands:
+By providing the necessary information through a metadata file, you can initiate training and inference processes using the following commands:
 
 ```bash
 train --metadata_path=PATH_TO_YAML_METADATA_FILE
 infer --metadata_path=PATH_TO_YAML_METADATA_FILE
 ```
 Here is a quick example:
 
@@ -284,15 +288,15 @@
   --table_name=TABLE_NAME
 ```
 
 PATH_TO_LOCAL_FOLDER is an absolute path to the folder where your original csv is stored.
 
 You can add any arguments listed in the corresponding sections for infer and training processes in the CLI call.
 
-To run dockerized code for linked tables simply call:
+To run dockerized code by providing the metadata file simply call:
 
 ```bash
 docker pull tdspora/syngen-train:latest
 docker run --rm \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-train \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.1.4 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.1.5 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
@@ -31,104 +31,120 @@
 data/housing.csv â-table_name Housing infer --table_name Housing ``` As the
 example you can use the dataset "Housing" in [example-data/housing.csv]
 (example-data/housing.csv). In this example, our real-world data is "Housing"
 from Kaggle. ## Features ### Training You can add flexibility to the training
 and inference processes using additional hyperparameters.
 For training of single table call: ```bash train --source PATH_TO_ORIGINAL_CSV
 \ --table_name TABLE_NAME \ --epochs INT \ --row_limit INT \ --drop_null BOOL \
---print_report BOOL \ --batch_size INT ``` For training of the multiple linked
-tables call: ```bash train --metadata_path PATH_TO_METADATA_YAML ``` The
-parameters which you can set up for training process: - source â required
-parameter for training of single table, a path to the file that you want to use
-as a reference - table_name â required parameter for training of single
-table, an arbitrary string to name the directories - epochs â a number of
-training epochs. Since the early stopping mechanism is implemented the bigger
-value of epochs is the better - row_limit â a number of rows to train over. A
-number less than the original table length will randomly subset the specified
-number of rows - drop_null â whether to drop rows with at least one missing
-value - batch_size â if specified, the training is split into batches. This
-can save the RAM - print_report - whether to generate accuracy and sampling
-reports. Please note that the sampling report is generated only if the
-`row_limit` parameter is set. - metadata_path â a path to the metadata file
-containing the metadata for linked tables - column_types - might include the
-section categorical which contains the listed columns defined as categorical by
-a user Requirements for parameters of training process: * source - data type -
-string * table_name - data type - string * epochs - data type - integer, must
-be equal to or more than 1, default value is 10 * row_limit - data type -
-integer * drop_null - data type - boolean, default value - False * batch_size -
-data type - integer, must be equal to or more than 1, default value - 32 *
-print_report - data type - boolean, default value is False * metadata_path -
-data type - string * column_types - data type - dictionary with the key
-categorical - the list of columns (data type - string) ### Inference
-(generation) You can customize the inference processes by calling for one
-table: ```bash infer --size INT \ --table_name STR \ --run_parallel BOOL \ --
-batch_size INT \ --random_seed INT \ --print_report BOOL ``` For linked tables
-you can simply call: ```bash infer --metadata_path PATH_TO_METADATA ``` The
-parameters which you can set up for generation process: - size - the desired
-number of rows to generate - table_name â required parameter for inference of
-single table, the name of the table, same as in training - run_parallel â
-whether to use multiprocessing (feasible for tables > 5000 rows) - batch_size
-â if specified, the generation is split into batches. This can save the RAM -
-random_seed â if specified, generates a reproducible result - print_report
-â whether to generate accuracy and sampling reports. Please note that the
-sampling report is generated only if the row_limit parameter is set. -
-metadata_path â a path to metadata file to generate linked tables
+--print_report BOOL \ --batch_size INT ``` To train one or more tables using a
+metadata file, you can use the following command: ```bash train --metadata_path
+PATH_TO_METADATA_YAML ``` The parameters which you can set up for training
+process: - source â required parameter for training of single table, a path
+to the file that you want to use as a reference - table_name â required
+parameter for training of single table, an arbitrary string to name the
+directories - epochs â a number of training epochs. Since the early stopping
+mechanism is implemented the bigger value of epochs is the better - row_limit
+â a number of rows to train over. A number less than the original table
+length will randomly subset the specified number of rows - drop_null â
+whether to drop rows with at least one missing value - batch_size â if
+specified, the training is split into batches. This can save the RAM -
+print_report - whether to generate accuracy and sampling reports. Please note
+that the sampling report is generated only if the `row_limit` parameter is set.
+- metadata_path â a path to the metadata file containing the metadata -
+column_types - might include the section categorical which contains the listed
+columns defined as categorical by a user Requirements for parameters of
+training process: * source - data type - string * table_name - data type -
+string * epochs - data type - integer, must be equal to or more than 1, default
+value is 10 * row_limit - data type - integer * drop_null - data type -
+boolean, default value - False * batch_size - data type - integer, must be
+equal to or more than 1, default value - 32 * print_report - data type -
+boolean, default value is False * metadata_path - data type - string *
+column_types - data type - dictionary with the key categorical - the list of
+columns (data type - string) ### Inference (generation) You can customize the
+inference processes by calling for one table: ```bash infer --size INT \ --
+table_name STR \ --run_parallel BOOL \ --batch_size INT \ --random_seed INT \ -
+-print_report BOOL ``` To generate one or more tables using a metadata file,
+you can use the following command: ```bash infer --metadata_path
+PATH_TO_METADATA ``` The parameters which you can set up for generation
+process: - size - the desired number of rows to generate - table_name â
+required parameter for inference of single table, the name of the table, same
+as in training - run_parallel â whether to use multiprocessing (feasible for
+tables > 5000 rows) - batch_size â if specified, the generation is split into
+batches. This can save the RAM - random_seed â if specified, generates a
+reproducible result - print_report â whether to generate accuracy and
+sampling reports. Please note that the sampling report is generated only if the
+row_limit parameter is set. - metadata_path â a path to metadata file
 Requirements for parameters of generation process: * size - data type -
 integer, must be equal to or more than 1, default value is 100 * table_name -
 data type - string * run_parallel - data type - boolean, default value is False
 * batch_size - data type - integer, must be equal to or more than 1 *
 random_seed - data type - integer, must be equal to or more than 0 *
 print_report - data type - boolean, default value is False * metadata_path -
 data type - string The metadata can contain any of the arguments above for each
 table. If so, the duplicated arguments from the CLI will be ignored. ### Linked
-tables generation To generate linked tables, you should provide metadata in
-yaml format. It is used to handle complex relations for any number of tables.
-You can also specify additional parameters needed for training and inference in
-the metadata file and in this case, they will be ignored in the CLI call. The
-yaml metadata file should match the following template: CUSTOMER: # Table name
-source: "./files/customer.csv" # Supported formats include local files in CSV,
-Avro formats train_settings: # Settings for training process epochs: 10 #
-Number of epochs if different from the default in the command line options
-drop_null: False # Drop rows with NULL values row_limit: None # Number of rows
-to train over. A number less than the original table length will randomly
-subset the specified rows number batch_size: 32 # If specified, the training is
-split into batches. This can save the RAM print_report: False # Turn on or turn
-off generation of the report column_types: categorical: # Force listed columns
-to have categorical type (use dictionary of values) - gender - marital_status
-infer_settings: # Settings for infer process size: 100 # Size for generated
-data run_parallel: False # Turn on or turn off parallel training process
-print_report: False # Turn on or turn off generation of the report batch_size:
+tables generation To generate one or more tables, you might provide metadata in
+yaml format. By providing information about the relationships between tables
+via metadata, it becomes possible to manage complex relationships across any
+number of tables. You can also specify additional parameters needed for
+training and inference in the metadata file and in this case, they will be
+ignored in the CLI call. Note: By using metadata file, you can also generate
+tables with absent relationships. In this case, the tables will be generated
+independently. The yaml metadata file should match the following template:
+CUSTOMER: # Table name. Required parameter source: "./files/customer.csv" #
+Supported formats include local files in CSV, Avro formats. Required parameter
+train_settings: # Settings for training process. Optional parameter epochs: 10
+# Number of epochs if different from the default in the command line options.
+Optional parameter drop_null: False # Drop rows with NULL values. Optional
+parameter row_limit: None # Number of rows to train over. A number less than
+the original table length will randomly subset the specified rows number.
+Optional parameter batch_size: 32 # If specified, the training is split into
+batches. This can save the RAM. Optional parameter print_report: False # Turn
+on or turn off generation of the report. Optional parameter column_types:
+categorical: # Force listed columns to have categorical type (use dictionary of
+values). Optional parameter - gender - marital_status infer_settings: #
+Settings for infer process. Optional parameter size: 100 # Size for generated
+data. Optional parameter run_parallel: False # Turn on or turn off parallel
+training process. Optional parameter print_report: False # Turn on or turn off
+generation of the report. Optional parameter batch_size: None # If specified,
+the generation is split into batches. This can save the RAM. Optional parameter
+random_seed: None # If specified, generates a reproducible result. Optional
+parameter keys: # Keys of the table. Optional parameter PK_CUSTOMER_ID: # Name
+of a key. Only one PK per table. type: "PK" # The key type. Supported: PK -
+primary key, FK - foreign key, TKN - token key columns: # Array of column names
+- customer_id UQ1: # Name of a key type: "UQ" # One or many unique keys
+columns: - e_mail FK1: # One or many foreign keys type: "FK" columns: # Array
+of columns in the current table - e_mail - alias references: table: "PROFILE" #
+Name of the parent table columns: # Array of columns in the parent table -
+e_mail - alias FK2: type: "FK" columns: - address_id references: table:
+"ADDRESS" columns: - address_id ORDER: # Table name. Required parameter source:
+"./files/order.csv" # Supported formats include local files in CSV, Avro
+formats. Required parameter train_settings: # Settings for training process.
+Optional parameter epochs: 10 # Number of epochs if different from the default
+in the command line options. Optional parameter drop_null: False # Drop rows
+with NULL values. Optional parameter row_limit: None # Number of rows to train
+over. A number less than the original table length will randomly subset the
+specified rows number. Optional parameter batch_size: 32 # If specified, the
+training is split into batches. This can save the RAM. Optional parameter
+print_report: False # Turn on or turn off generation of the report. Optional
+parameter column_types: categorical: # Force listed columns to have categorical
+type (use dictionary of values). Optional parameter - gender - marital_status
+infer_settings: # Settings for infer process. Optional parameter size: 100 #
+Size for generated data. Optional parameter run_parallel: False # Turn on or
+turn off parallel training process. Optional parameter print_report: False #
+Turn on or turn off generation of the report. Optional parameter batch_size:
 None # If specified, the generation is split into batches. This can save the
-RAM random_seed: None # If specified, generates a reproducible result keys:
-PK_CUSTOMER_ID: # Name of a key. Only one PK per table. type: "PK" # The key
-type. Supported: PK - primary key, FK - foreign key, TKN - token key columns: #
-Array of column names - customer_id UQ1: # Name of a key type: "UQ" # One or
-many unique keys columns: - e_mail FK1: # One or many foreign keys type: "FK"
-columns: # Array of columns in the current table - e_mail - alias references:
-table: "PROFILE" # Name of the parent table columns: # Array of columns in the
-parent table - e_mail - alias FK2: type: "FK" columns: - address_id references:
-table: "ADDRESS" columns: - address_id ORDER: source: "./files/order.csv"
-train_settings: epochs: 10 # Number of epochs if different from the default in
-the command line options drop_null: False # Drop rows with NULL values
-row_limit: None # Number of rows to train over. A number less than the original
-table length will randomly subset the specified rows number batch_size: 32 # If
-specified, the training is split into batches. This can save the RAM
-print_report: False # Turn on or turn off generation of the report
-column_types: categorical: # Force listed columns to have categorical type (use
-dictionary of values) - gender - marital_status infer_settings: # Settings for
-infer process size: 100 # Size for generated data run_parallel: False # Turn on
-or turn off parallel training process print_report: False # Turn on or turn off
-generation of the report batch_size: None # If specified, the generation is
-split into batches. This can save the RAM random_seed: None # If specified,
-generates a reproducible result keys: pk_order_id: type: "PK" columns: -
-order_id FK1: type: "FK" columns: - customer_id references: table: "CUSTOMER"
-columns: - customer_id You can find the example of metadata file in [example-
-metadata/housing_metadata.yaml](example-metadata/housing_metadata.yaml)
-For related tables training you can use the commands: ```bash train --
-metadata_path=PATH_TO_YAML_METADATA_FILE infer --
+RAM. Optional parameter random_seed: None # If specified, generates a
+reproducible result. Optional parameter keys: # Keys of the table. Optional
+parameter pk_order_id: type: "PK" columns: - order_id FK1: type: "FK" columns:
+- customer_id references: table: "CUSTOMER" columns: - customer_id You can find
+the example of metadata file in [example-metadata/housing_metadata.yaml]
+(example-metadata/housing_metadata.yaml)
+By providing the necessary information through a metadata file, you can
+initiate training and inference processes using the following commands: ```bash
+train --metadata_path=PATH_TO_YAML_METADATA_FILE infer --
 metadata_path=PATH_TO_YAML_METADATA_FILE ``` Here is a quick example: ```bash
 train --metadata_path="./example-metadata/housing_metadata.yaml" infer --
 metadata_path="./example-metadata/housing_metadata.yaml" ``` If `--
 metadata_path` is present and the metadata contains the necessary parameters,
 other CLI parameters will be ignored.
 ### Docker images The train and inference components of syngen is available as
 public docker images:
@@ -138,30 +154,30 @@
 docker pull tdspora/syngen-train:latest docker run --rm \ -
 v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-train \ --
 table_name=TABLE_NAME \ --source=./model_artifacts/YOUR_CSV_FILE.csv docker
 pull tdspora/syngen-infer:latest docker run --rm \ -v PATH_TO_LOCAL_FOLDER:/
 src/model_artifacts tdspora/syngen-infer \ --table_name=TABLE_NAME ```
 PATH_TO_LOCAL_FOLDER is an absolute path to the folder where your original csv
 is stored. You can add any arguments listed in the corresponding sections for
-infer and training processes in the CLI call. To run dockerized code for linked
-tables simply call: ```bash docker pull tdspora/syngen-train:latest docker run
---rm \ -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-train \ --
-metadata_path=./model_artifacts/PATH_TO_METADATA_YAML docker pull tdspora/
-syngen-infer:latest docker run --rm \ -v PATH_TO_LOCAL_FOLDER:/src/
-model_artifacts tdspora/syngen-infer \ --metadata_path=./model_artifacts/
-PATH_TO_METADATA_YAML ``` You can add any arguments listed in the corresponding
-sections for infer and training processes in the CLI call, however, they will
-be overwritten by corresponding arguments in the metadata file. ## Contribution
-We welcome contributions from the community to help us improve and maintain our
-public GitHub repository. We appreciate any feedback, bug reports, or feature
-requests, and we encourage developers to submit fixes or new features using
-issues. If you have found a bug or have a feature request, please submit an
-issue to our GitHub repository. Please provide as much detail as possible,
-including steps to reproduce the issue or a clear description of the feature
-request. Our team will review the issue and work with you to address any
-problems or discuss any potential new features. If you would like to contribute
-a fix or a new feature, please submit a pull request to our GitHub repository.
-Please make sure your code follows our coding standards and best practices. Our
-team will review your pull request and work with you to ensure that it meets
-our standards and is ready for inclusion in our codebase. We appreciate your
-contributions and thank you for your interest in helping us maintain and
-improve our public GitHub repository.
+infer and training processes in the CLI call. To run dockerized code by
+providing the metadata file simply call: ```bash docker pull tdspora/syngen-
+train:latest docker run --rm \ -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts
+tdspora/syngen-train \ --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
+docker pull tdspora/syngen-infer:latest docker run --rm \ -
+v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen-infer \ --
+metadata_path=./model_artifacts/PATH_TO_METADATA_YAML ``` You can add any
+arguments listed in the corresponding sections for infer and training processes
+in the CLI call, however, they will be overwritten by corresponding arguments
+in the metadata file. ## Contribution We welcome contributions from the
+community to help us improve and maintain our public GitHub repository. We
+appreciate any feedback, bug reports, or feature requests, and we encourage
+developers to submit fixes or new features using issues. If you have found a
+bug or have a feature request, please submit an issue to our GitHub repository.
+Please provide as much detail as possible, including steps to reproduce the
+issue or a clear description of the feature request. Our team will review the
+issue and work with you to address any problems or discuss any potential new
+features. If you would like to contribute a fix or a new feature, please submit
+a pull request to our GitHub repository. Please make sure your code follows our
+coding standards and best practices. Our team will review your pull request and
+work with you to ensure that it meets our standards and is ready for inclusion
+in our codebase. We appreciate your contributions and thank you for your
+interest in helping us maintain and improve our public GitHub repository.
```

### Comparing `syngen-0.1.4/src/syngen.egg-info/SOURCES.txt` & `syngen-0.1.5/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

