# Comparing `tmp/deepparse-0.9.6.tar.gz` & `tmp/deepparse-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepparse-0.9.6.tar", last modified: Fri Mar 31 10:50:16 2023, max compression
+gzip compressed data, was "deepparse-0.9.7.tar", last modified: Mon May 22 13:13:16 2023, max compression
```

## Comparing `deepparse-0.9.6.tar` & `deepparse-0.9.7.tar`

### file list

```diff
@@ -1,212 +1,214 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.059616 deepparse-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-03-31 10:50:06.000000 deepparse-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-03-31 10:50:16.059616 deepparse-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-03-31 10:50:06.000000 deepparse-0.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.043616 deepparse-0.9.6/deepparse/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.043616 deepparse-0.9.6/deepparse/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/cli/download_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/cli/download_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/cli/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/cli/parser_arguments_adder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/cli/retrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/cli/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/cli/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.043616 deepparse-0.9.6/deepparse/comparer/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/comparer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/comparer/addresses_comparer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/comparer/formatted_compared_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/comparer/formatted_compared_addresses_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/comparer/formatted_compared_addresses_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.047617 deepparse-0.9.6/deepparse/converter/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/converter/data_padder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/converter/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/converter/data_processor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/converter/target_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.047617 deepparse-0.9.6/deepparse/data_validation/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/data_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/data_validation/data_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.047617 deepparse-0.9.6/deepparse/dataset_container/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/dataset_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/dataset_container/dataset_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/dataset_container/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.047617 deepparse-0.9.6/deepparse/embeddings_models/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/embeddings_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/embeddings_models/bpemb_embeddings_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/embeddings_models/embeddings_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/embeddings_models/embeddings_model_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/embeddings_models/fasttext_embeddings_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/embeddings_models/magnitude_embeddings_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.047617 deepparse-0.9.6/deepparse/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/errors/data_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/errors/model_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/errors/server_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/fasttext_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.047617 deepparse-0.9.6/deepparse/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/metrics/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/metrics/nll_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.047617 deepparse-0.9.6/deepparse/network/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/network/bpemb_seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/network/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/network/embedding_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/network/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/network/fasttext_seq2seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/network/model_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/network/seq2seq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.047617 deepparse-0.9.6/deepparse/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61170 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/parser/address_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/parser/capturing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/parser/formatted_parsed_address.py
--rw-r--r--   0 runner    (1001) docker     (123)     5544 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/parser/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.047617 deepparse-0.9.6/deepparse/pre_processing/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/pre_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/pre_processing/pre_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.047617 deepparse-0.9.6/deepparse/vectorizer/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/vectorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/vectorizer/bpemb_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/vectorizer/fasttext_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/vectorizer/magnitude_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/vectorizer/vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/vectorizer/vectorizer_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-31 10:50:15.000000 deepparse-0.9.6/deepparse/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-31 10:50:06.000000 deepparse-0.9.6/deepparse/weights_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.043616 deepparse-0.9.6/deepparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-03-31 10:50:15.000000 deepparse-0.9.6/deepparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-03-31 10:50:16.000000 deepparse-0.9.6/deepparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 10:50:15.000000 deepparse-0.9.6/deepparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-31 10:50:15.000000 deepparse-0.9.6/deepparse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-31 10:50:15.000000 deepparse-0.9.6/deepparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-31 10:50:15.000000 deepparse-0.9.6/deepparse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.051617 deepparse-0.9.6/models_evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/models_evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-31 10:50:06.000000 deepparse-0.9.6/models_evaluation/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-03-31 10:50:06.000000 deepparse-0.9.6/models_evaluation/evaluate_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-31 10:50:06.000000 deepparse-0.9.6/models_evaluation/generate_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-03-31 10:50:06.000000 deepparse-0.9.6/models_evaluation/speed_test_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.051617 deepparse-0.9.6/models_evaluation/timer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/models_evaluation/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-03-31 10:50:06.000000 deepparse-0.9.6/models_evaluation/timer/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-03-31 10:50:06.000000 deepparse-0.9.6/models_evaluation/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-31 10:50:06.000000 deepparse-0.9.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.051617 deepparse-0.9.6/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-31 10:50:06.000000 deepparse-0.9.6/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-31 10:50:16.059616 deepparse-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-03-31 10:50:06.000000 deepparse-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.051617 deepparse-0.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/base_capture_output.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/base_file_exist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.051617 deepparse-0.9.6/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/cli/test_download_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/cli/test_download_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/cli/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/cli/test_retrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/cli/test_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/cli/test_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.051617 deepparse-0.9.6/tests/comparer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/comparer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/comparer/test_addresses_comparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/comparer/test_formatted_compared_addresses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/comparer/test_formatted_compared_addresses_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/comparer/test_formatted_compared_addresses_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.051617 deepparse-0.9.6/tests/converter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/converter/test_data_padder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/converter/test_data_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/converter/test_data_processor_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/converter/test_target_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.051617 deepparse-0.9.6/tests/data_validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/data_validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/data_validation/test_data_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.051617 deepparse-0.9.6/tests/dataset_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/dataset_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23762 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/dataset_container/test_dataset_container.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/dataset_container/test_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.051617 deepparse-0.9.6/tests/embeddings_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/embeddings_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/embeddings_models/test_bpemb_embeddings_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/embeddings_models/test_embeddings_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/embeddings_models/test_embeddings_model_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/embeddings_models/test_fasttext_embeddings_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/embeddings_models/test_magnitude_embeddings_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.055616 deepparse-0.9.6/tests/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/metrics/test_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/metrics/test_nll_loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.055616 deepparse-0.9.6/tests/models_evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/models_evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/models_evaluation/test_tools_models_evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.055616 deepparse-0.9.6/tests/network/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.055616 deepparse-0.9.6/tests/network/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/integration/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/integration/test_integration_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/integration/test_integration_embedding_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/integration/test_integration_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/integration/test_integration_seq2seq_bpemb_model_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/integration/test_integration_seq2seq_bpemb_model_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/integration/test_integration_seq2seq_fasttext_model_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/integration/test_integration_seq2seq_fasttext_model_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/integration/test_integration_seq2seq_model_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/integration/test_integration_seq2seq_model_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    18257 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/test_bpemb_seq2seq_model_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    17978 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/test_bpemb_seq2seq_model_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/test_embedding_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14689 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/test_fasttext_seq2seq_model_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    14903 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/test_fasttext_seq2seq_model_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/test_model_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17747 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/network/test_seq2seq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.055616 deepparse-0.9.6/tests/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.059616 deepparse-0.9.6/tests/parser/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/base_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/base_retrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/test_integration_address_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6861 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_new_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_new_params_new_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_retrain_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_retrain_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_retrain_freeze_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_retrain_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    21743 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_retrain_new_address_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_test_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/test_integration_reload_retrain_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/integration/test_integration_retrain_test_api_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    74223 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/test_address_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    70964 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/test_address_parser_retrain_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/test_address_parser_test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/test_formatted_parsed_address.py
--rw-r--r--   0 runner    (1001) docker     (123)    19555 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/parser/test_user_fromatted_parsed_address.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.059616 deepparse-0.9.6/tests/pre_processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/pre_processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/pre_processing/test_address_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/test_fasttext_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/test_integration_fasttext_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:16.059616 deepparse-0.9.6/tests/vectorizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/vectorizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/vectorizer/test_bpemb_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/vectorizer/test_fasttext_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/vectorizer/test_magnitude_vectorizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-03-31 10:50:06.000000 deepparse-0.9.6/tests/vectorizer/test_vectorizer_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.332264 deepparse-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-22 13:13:05.000000 deepparse-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-05-22 13:13:16.332264 deepparse-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19777 2023-05-22 13:13:05.000000 deepparse-0.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.316264 deepparse-0.9.7/deepparse/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/download_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/download_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/parser_arguments_adder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/retrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/cli/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/comparer/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/comparer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/comparer/addresses_comparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/comparer/formatted_compared_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/comparer/formatted_compared_addresses_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/comparer/formatted_compared_addresses_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/converter/data_padder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/converter/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/converter/data_processor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/converter/target_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/data_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/data_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/data_validation/data_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/dataset_container/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/dataset_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/dataset_container/dataset_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/dataset_container/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/embeddings_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/embeddings_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/embeddings_models/bpemb_embeddings_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/embeddings_models/embeddings_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/embeddings_models/embeddings_model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/embeddings_models/fasttext_embeddings_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/embeddings_models/magnitude_embeddings_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/errors/data_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/errors/model_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/errors/server_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/fasttext_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/metrics/accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/metrics/nll_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/bpemb_seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/embedding_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/fasttext_seq2seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/network/seq2seq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/deepparse/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65091 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/parser/address_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/parser/capturing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12628 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/parser/formatted_parsed_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/parser/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/deepparse/pre_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/pre_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/pre_processing/pre_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/deepparse/vectorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/vectorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/vectorizer/bpemb_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/vectorizer/fasttext_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/vectorizer/magnitude_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/vectorizer/vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/vectorizer/vectorizer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-22 13:13:16.000000 deepparse-0.9.7/deepparse/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-22 13:13:05.000000 deepparse-0.9.7/deepparse/weights_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.320264 deepparse-0.9.7/deepparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-05-22 13:13:16.000000 deepparse-0.9.7/deepparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-05-22 13:13:16.000000 deepparse-0.9.7/deepparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:13:16.000000 deepparse-0.9.7/deepparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-22 13:13:16.000000 deepparse-0.9.7/deepparse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 13:13:16.000000 deepparse-0.9.7/deepparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-22 13:13:16.000000 deepparse-0.9.7/deepparse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/models_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/evaluate_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/generate_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/speed_test_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/models_evaluation/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/timer/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-05-22 13:13:05.000000 deepparse-0.9.7/models_evaluation/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 13:13:05.000000 deepparse-0.9.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-22 13:13:05.000000 deepparse-0.9.7/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-22 13:13:16.332264 deepparse-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-22 13:13:05.000000 deepparse-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/base_capture_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/base_file_exist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/cli/test_download_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/cli/test_download_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12091 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/cli/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11827 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/cli/test_retrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/cli/test_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15172 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/cli/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.324264 deepparse-0.9.7/tests/comparer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/comparer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/comparer/test_addresses_comparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/comparer/test_formatted_compared_addresses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/comparer/test_formatted_compared_addresses_raw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/comparer/test_formatted_compared_addresses_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/converter/test_data_padder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/converter/test_data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/converter/test_data_processor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/converter/test_target_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/data_validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/data_validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/data_validation/test_data_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/dataset_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/dataset_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23762 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/dataset_container/test_dataset_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/dataset_container/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/embeddings_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/embeddings_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/embeddings_models/test_bpemb_embeddings_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/embeddings_models/test_embeddings_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/embeddings_models/test_embeddings_model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/embeddings_models/test_fasttext_embeddings_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/embeddings_models/test_magnitude_embeddings_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/metrics/test_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/metrics/test_nll_loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/models_evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/models_evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/models_evaluation/test_tools_models_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/network/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.328264 deepparse-0.9.7/tests/network/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_embedding_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_bpemb_model_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_bpemb_model_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_fasttext_model_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_fasttext_model_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_model_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_model_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18841 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_bpemb_seq2seq_model_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18562 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_bpemb_seq2seq_model_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_embedding_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_fasttext_seq2seq_model_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15426 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_fasttext_seq2seq_model_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_model_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17727 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/network/test_seq2seq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.332264 deepparse-0.9.7/tests/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.332264 deepparse-0.9.7/tests/parser/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/base_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/base_retrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9558 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6891 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_new_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_new_params_new_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_freeze_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21743 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_new_address_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_test_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_reload_retrain_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_retrain_test_api_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/integration/test_integration_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74223 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/test_address_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70964 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/test_address_parser_retrain_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15345 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/test_address_parser_test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/test_formatted_parsed_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19555 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/parser/test_user_fromatted_parsed_address.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.332264 deepparse-0.9.7/tests/pre_processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/pre_processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/pre_processing/test_address_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/test_fasttext_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/test_integration_fasttext_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14735 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/test_weights_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:16.332264 deepparse-0.9.7/tests/vectorizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/vectorizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/vectorizer/test_bpemb_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/vectorizer/test_fasttext_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/vectorizer/test_magnitude_vectorizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-22 13:13:05.000000 deepparse-0.9.7/tests/vectorizer/test_vectorizer_factory.py
```

### Comparing `deepparse-0.9.6/LICENSE` & `deepparse-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/PKG-INFO` & `deepparse-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: deepparse
-Version: 0.9.6
+Version: 0.9.7
 Summary: A library for parsing multinational street addresses using deep learning.
 Home-page: https://deepparse.org/
-Download-URL: https://github.com/GRAAL-Research/deepparse/archive/v0.9.6.zip
+Download-URL: https://github.com/GRAAL-Research/deepparse/archive/v0.9.7.zip
 Author: Marouane Yassine, David Beauchemin
 Author-email: marouane.yassine.1@ulaval.ca, david.beauchemin.5@ulaval.ca
 License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: deepparse Version: 0.9.6 Summary: A library for
+Metadata-Version: 2.1 Name: deepparse Version: 0.9.7 Summary: A library for
 parsing multinational street addresses using deep learning. Home-page: https://
 deepparse.org/ Download-URL: https://github.com/GRAAL-Research/deepparse/
-archive/v0.9.6.zip Author: Marouane Yassine, David Beauchemin Author-email:
+archive/v0.9.7.zip Author: Marouane Yassine, David Beauchemin Author-email:
 marouane.yassine.1@ulaval.ca, david.beauchemin.5@ulaval.ca License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 GNU Lesser General Public License v3 (LGPLv3) Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `deepparse-0.9.6/README.md` & `deepparse-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/cli/download_model.py` & `deepparse-0.9.7/deepparse/cli/download_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/cli/download_models.py` & `deepparse-0.9.7/deepparse/cli/download_models.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/cli/parse.py` & `deepparse-0.9.7/deepparse/cli/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
         parse fasttext ./dataset_path.csv parsed_address.p --device 0
 
     Using a CSV dataset
 
     .. code-block:: sh
 
-        parse fasttext ./dataset.csv parsed_address.pckl --path_to_retrained_model ./path
+        parse fasttext ./dataset.csv parsed_address.pckl --path_to_model_weights ./path
 
     """
     if args is None:  # pragma: no cover
         args = sys.argv[1:]
 
     parsed_args = get_args(args)
```

### Comparing `deepparse-0.9.6/deepparse/cli/parser_arguments_adder.py` & `deepparse-0.9.7/deepparse/cli/parser_arguments_adder.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         default=32,
     )
 
 
 def add_path_to_retrained_model_arg(parser: ArgumentParser) -> None:
     parser.add_argument(
         "--path_to_retrained_model",
-        help=wrap("A path to a retrained model to use for testing."),
+        help=wrap("A path to a retrained model to use. It can be an S3-URI."),
         type=str,
         default=None,
     )
 
 
 def add_num_workers_arg(parser: ArgumentParser) -> None:
     parser.add_argument(
```

### Comparing `deepparse-0.9.6/deepparse/cli/retrain.py` & `deepparse-0.9.7/deepparse/cli/retrain.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/cli/test.py` & `deepparse-0.9.7/deepparse/cli/test.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/cli/tools.py` & `deepparse-0.9.7/deepparse/cli/tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/comparer/addresses_comparer.py` & `deepparse-0.9.7/deepparse/comparer/addresses_comparer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/comparer/formatted_compared_addresses.py` & `deepparse-0.9.7/deepparse/comparer/formatted_compared_addresses.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/comparer/formatted_compared_addresses_raw.py` & `deepparse-0.9.7/deepparse/comparer/formatted_compared_addresses_raw.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/comparer/formatted_compared_addresses_tags.py` & `deepparse-0.9.7/deepparse/comparer/formatted_compared_addresses_tags.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/converter/data_padder.py` & `deepparse-0.9.7/deepparse/converter/data_padder.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/converter/data_processor.py` & `deepparse-0.9.7/deepparse/converter/data_processor.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/converter/data_processor_factory.py` & `deepparse-0.9.7/deepparse/converter/data_processor_factory.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/converter/target_converter.py` & `deepparse-0.9.7/deepparse/converter/target_converter.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/data_validation/data_validation.py` & `deepparse-0.9.7/deepparse/data_validation/data_validation.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/dataset_container/dataset_container.py` & `deepparse-0.9.7/deepparse/dataset_container/dataset_container.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/dataset_container/tools.py` & `deepparse-0.9.7/deepparse/dataset_container/tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/embeddings_models/bpemb_embeddings_model.py` & `deepparse-0.9.7/deepparse/embeddings_models/bpemb_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/embeddings_models/embeddings_model_factory.py` & `deepparse-0.9.7/deepparse/embeddings_models/embeddings_model_factory.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/embeddings_models/fasttext_embeddings_model.py` & `deepparse-0.9.7/deepparse/embeddings_models/fasttext_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/embeddings_models/magnitude_embeddings_model.py` & `deepparse-0.9.7/deepparse/embeddings_models/magnitude_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/fasttext_tools.py` & `deepparse-0.9.7/deepparse/fasttext_tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/network/bpemb_seq2seq.py` & `deepparse-0.9.7/deepparse/network/bpemb_seq2seq.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/network/decoder.py` & `deepparse-0.9.7/deepparse/network/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # pylint: disable=W0223, too-many-arguments, too-many-instance-attributes
 
 from typing import Tuple, List
 
 import torch
 from torch import nn
 
-from ..weights_init import weights_init
+from .. import weights_init
 
 
 class Decoder(nn.Module):
     """
     Decoder module that use a LSTM to decode a previously encoded sequence and a linear layer to map
     the decoded sequence tags.
```

### Comparing `deepparse-0.9.6/deepparse/network/embedding_network.py` & `deepparse-0.9.7/deepparse/network/embedding_network.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/network/encoder.py` & `deepparse-0.9.7/deepparse/network/encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from typing import Tuple, List
 
 import torch
 from torch import nn
 from torch.nn.utils.rnn import pack_padded_sequence, pad_packed_sequence
 
-from ..weights_init import weights_init
+from .. import weights_init
 
 
 class Encoder(nn.Module):
     """
     Encoder module that use a LSTM to encode a sequence.
 
     Args:
```

### Comparing `deepparse-0.9.6/deepparse/network/fasttext_seq2seq.py` & `deepparse-0.9.7/deepparse/network/fasttext_seq2seq.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/network/model_factory.py` & `deepparse-0.9.7/deepparse/network/model_factory.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/network/seq2seq.py` & `deepparse-0.9.7/deepparse/network/seq2seq.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # pylint: disable=too-many-arguments
 
 import os
 import random
 import warnings
 from abc import ABC
-from collections import OrderedDict
 from typing import Tuple, Union, List
 
 import torch
 from torch import nn
 
 from .decoder import Decoder
 from .encoder import Encoder
+from .. import handle_weights_upload
 from ..tools import download_weights, latest_version
 
 
 class Seq2SeqModel(ABC, nn.Module):
     """
     Abstract class for Seq2Seq networks.
 
@@ -109,28 +109,29 @@
                 if self.verbose:
                     warnings.warn(
                         "A new version of the pretrained model is available. The newest model will be downloaded.",
                         category=UserWarning,
                     )
                 download_weights(model_type, cache_dir, verbose=self.verbose)
 
-        all_layers_params = torch.load(model_path, map_location=self.device)
-        self.load_state_dict(all_layers_params)
+        self._load_weights(path_to_model_torch_archive=model_path)
 
-    def _load_weights(self, path_to_retrained_model: str) -> None:
+    def _load_weights(self, path_to_model_torch_archive: str) -> None:
         """
         Method to load (into the network) the weights.
 
         Args:
-            path_to_retrained_model (str): The path to the fine-tuned model.
+            path_to_model_torch_archive (str): The path to the fine-tuned model Torch archive.
         """
-        all_layers_params = torch.load(path_to_retrained_model, map_location=self.device)
-        if isinstance(all_layers_params, dict) and not isinstance(all_layers_params, OrderedDict):
-            # Case where we have a retrained model with a different tagging space
-            all_layers_params = all_layers_params.get("address_tagger_model")
+        all_layers_params = handle_weights_upload(
+            path_to_model_to_upload=path_to_model_torch_archive, device=self.device
+        )
+
+        # All the time, our torch archive include meta-data along with the model weights
+        all_layers_params = all_layers_params.get("address_tagger_model")
         self.load_state_dict(all_layers_params)
 
     def _encoder_step(self, to_predict: torch.Tensor, lengths: List, batch_size: int) -> Tuple:
         """
         Step of the encoder.
 
         Args:
```

### Comparing `deepparse-0.9.6/deepparse/parser/address_parser.py` & `deepparse-0.9.7/deepparse/parser/address_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import warnings
 from functools import partial
 from pathlib import Path
 from platform import system
 from typing import Dict, List, Tuple, Union, Callable
 
 import torch
+from cloudpathlib import CloudPath, S3Path
 from poutyne.framework import Experiment
 from torch.optim import SGD
 from torch.utils.data import DataLoader, Subset
 
 from . import formatted_parsed_address
 from .capturing import Capturing
 from .formatted_parsed_address import FormattedParsedAddress
@@ -39,14 +40,15 @@
 from ..errors import FastTextModelError
 from ..metrics import nll_loss, accuracy
 from ..network import ModelFactory
 from ..pre_processing import coma_cleaning, lower_cleaning, hyphen_cleaning
 from ..pre_processing import trailing_whitespace_cleaning, double_whitespaces_cleaning
 from ..tools import CACHE_PATH, valid_poutyne_version
 from ..vectorizer import VectorizerFactory
+from ..weights_tools import handle_weights_upload
 
 _pre_trained_tags_to_idx = {
     "StreetNumber": 0,
     "StreetName": 1,
     "Unit": 2,
     "Municipality": 3,
     "Province": 4,
@@ -82,15 +84,15 @@
             - ``"fasttext"`` (need ~9 GO of RAM to be used),
             - ``"fasttext-light"`` (need ~2 GO of RAM to be used, but slower than fasttext version),
             - ``"bpemb"`` (need ~2 GO of RAM to be used),
             - ``"fastest"`` (quicker to process one address) (equivalent to ``"fasttext"``),
             - ``"lightest"`` (the one using the less RAM and GPU usage) (equivalent to ``"fasttext-light"``),
             - ``"best"`` (the best accuracy performance) (equivalent to ``"bpemb"``).
 
-            The default value is ``"best"`` for the most accurate model. Ignored if ``path_to_retrained_model`` is not
+            The default value is ``"best"`` for the most accurate model. Ignored if ``path_to_model_weights`` is not
             ``None``. To further improve performance, consider using the models (fasttext or BPEmb) with their
             counterparts using an attention mechanism with the ``attention_mechanism`` flag.
         attention_mechanism (bool): Whether to use the model with an attention mechanism. The model will use an
             attention mechanism that takes an extra 100 MB on GPU usage (see the doc for more statistics).
             The default value is False.
         device (Union[int, str, torch.torch.device]): The device to use can be either:
 
@@ -98,30 +100,33 @@
             - a complete device name in a string format (e.g. ``"cuda:0"``),
             - a :class:`~torch.torch.device` object,
             - ``"cpu"`` for a  ``CPU`` use.
 
             The default value is GPU with the index ``0`` if it exists. Otherwise, the value is ``CPU``.
         rounding (int): The rounding to use when asking the probability of the tags. The default value is four digits.
         verbose (bool): Turn on/off the verbosity of the model weights download and loading. The default value is True.
-        path_to_retrained_model (Union[str, None]): The path to the retrained model to use for prediction. We will
-            infer the ``model_type`` of the retrained model. The default value is ``None``, meaning we use our
+        path_to_retrained_model (Union[S3Path, str, None]): The path to the retrained model to use for prediction.
+            We will infer the ``model_type`` of the retrained model. The default value is ``None``, meaning we use our
             pretrained model. If the retrained model uses an attention mechanism, ``attention_mechanism`` needs to
-            be set to True.
+            be set to True. The path_to_retrain_model can also be a S3-like (Azure, AWS, Google) bucket URI string path
+            (e.g. ``"s3://path/to/aws/s3/bucket.ckpt"``). Or it can be a ``S3Path`` S3-like URI using `cloudpathlib`
+            to handle S3-like bucket. See `cloudpathlib <https://cloudpathlib.drivendata.org/stable/>`
+            for detail on supported S3 buckets provider and URI condition. The default value is None.
         cache_dir (Union[str, None]): The path to the cached directory to use for downloading (and loading) the
             embeddings model and the model pretrained weights.
         offline (bool): Whether or not the model is an offline one, meaning you have already downloaded the pre-trained
             weights and embeddings weights in either the default Deepparse cache directory (``"~./cache/deepparse"``) or
             the ``cache_dir`` directory. When offline, we will not verify if the model is the latest. You can use our
             ``download_models`` CLI function to download all the requirements for a model. The default value is False
             (not an offline parsing model).
 
     Note:
         For both networks, we will download the pretrained weights and embeddings in the ``.cache`` directory
         for the root user. The pretrained weights take at most 44 MB. The fastText embeddings take 6.8 GO,
-        the fastText-light embeddings take 3.3 GO and bpemb take 116 MB (in .cache/bpemb).
+        the fastText-light embeddings take 3.3 GO and bpemb take 116 MB (in ``".cache/bpemb"``).
 
         Also, one can download all the dependencies of our pretrained model using our CLI
         (e.g. download_model fasttext) before sending it to a node without access to Internet.
 
         Here are the URLs to download our pretrained models directly
 
             - `FastText <https://graal.ift.ulaval.ca/public/deepparse/fasttext.ckpt>`_,
@@ -160,53 +165,68 @@
             parse_address = address_parser("350 rue des Lilas Ouest Quebec city Quebec G1L 1B6")
 
         Using a retrained model
 
         .. code-block:: python
 
             address_parser = AddressParser(model_type="fasttext",
-                                           path_to_retrained_model="/path_to_a_retrain_fasttext_model")
+                                           path_to_model_weights="/path_to_a_retrain_fasttext_model.ckpt")
             parse_address = address_parser("350 rue des Lilas Ouest Quebec city Quebec G1L 1B6")
 
         Using a retrained model trained on different tags
 
         .. code-block:: python
 
-            # We don't give the model_type since it's ignored when using path_to_retrained_model
-            address_parser = AddressParser(path_to_retrained_model="/path_to_a_retrain_fasttext_model")
+            # We don't give the model_type since it's ignored when using path_to_model_weights
+            address_parser = AddressParser(path_to_model_weights="/path_to_a_retrain_fasttext_model.ckpt")
             parse_address = address_parser("350 rue des Lilas Ouest Quebec city Quebec G1L 1B6")
 
         Using a retrained model with attention
 
         .. code-block:: python
 
             address_parser = AddressParser(model_type="fasttext",
-                                           path_to_retrained_model="/path_to_a_retrain_fasttext_attention_model",
+                                           path_to_model_weights="/path_to_a_retrain_fasttext_attention_model.ckpt",
                                            attention_mechanism=True)
             parse_address = address_parser("350 rue des Lilas Ouest Quebec city Quebec G1L 1B6")
 
         Using Deepparse as an offline service (assuming all dependencies have been downloaded in the default cache
         dir or a specified dir using the cache_dir parameter).
 
         .. code-block:: python
 
             address_parser = AddressParser(model_type="fasttext",
                                            offline=True)
             parse_address = address_parser("350 rue des Lilas Ouest Quebec city Quebec G1L 1B6")
 
+         Using a retrained model in an S3-like bucket.
+
+        .. code-block:: python
+
+            address_parser = AddressParser(model_type="fasttext",
+                                           path_to_model_weights="s3://path/to/bucket.ckpt")
+            parse_address = address_parser("350 rue des Lilas Ouest Quebec city Quebec G1L 1B6")
+
+         Using a retrained model in an S3-like bucket using CloudPathLib.
+
+        .. code-block:: python
+
+            address_parser = AddressParser(model_type="fasttext",
+                                           path_to_model_weights=CloudPath("s3://path/to/bucket.ckpt"))
+            parse_address = address_parser("350 rue des Lilas Ouest Quebec city Quebec G1L 1B6")
     """
 
     def __init__(
         self,
         model_type: str = "best",
         attention_mechanism: bool = False,
         device: Union[int, str, torch.device] = 0,
         rounding: int = 4,
         verbose: bool = True,
-        path_to_retrained_model: Union[str, None] = None,
+        path_to_retrained_model: Union[S3Path, str, None] = None,
         cache_dir: Union[str, None] = None,
         offline: bool = False,
     ) -> None:
         # pylint: disable=too-many-arguments
         self._process_device(device)
 
         self.rounding = rounding
@@ -218,25 +238,29 @@
         tags_to_idx = _pre_trained_tags_to_idx
         # Default FIELDS of the formatted address
         fields = list(tags_to_idx)
         # Default new config seq2seq model params
         seq2seq_kwargs = {}  # Empty for default settings
 
         if path_to_retrained_model is not None:
-            checkpoint_weights = torch.load(path_to_retrained_model, map_location="cpu")
+            checkpoint_weights = handle_weights_upload(path_to_model_to_upload=path_to_retrained_model)
             if checkpoint_weights.get("model_type") is None:
                 # Validate if we have the proper metadata, it has at least the parser model type
                 # if no other thing have been modified.
-                raise RuntimeError(
-                    "You are not using the proper retrained checkpoint. "
+                error_text = (
+                    "You are not using the proper retrained checkpoint for Deepparse, since we also export other"
+                    "informations along with the model weights. "
                     "When we retrain an AddressParser, by default, we create a "
-                    "checkpoint name 'retrained_modeltype_address_parser.ckpt'. Be sure to use that"
-                    "checkpoint since it includes some metadata for the reloading."
+                    "checkpoint name 'retrained_modeltype_address_parser.ckpt'. "
+                    "Where 'modeltype' is the AddressParser model type (e.g. 'fasttext', 'bpemb'). "
+                    "The checkpoint name can also change if you give the retrained model a name. "
+                    "Be sure to use that checkpoint since it includes some metadata for the reloading. "
                     "See AddressParser.retrain for more details."
                 )
+                raise RuntimeError(error_text)
             if validate_if_new_seq2seq_params(checkpoint_weights):
                 seq2seq_kwargs = checkpoint_weights.get("seq2seq_params")
             if validate_if_new_prediction_tags(checkpoint_weights):
                 # We load the new tags_to_idx
                 tags_to_idx = checkpoint_weights.get("prediction_tags")
                 # We change the FIELDS for the FormattedParsedAddress
                 fields = list(tags_to_idx)
@@ -449,14 +473,15 @@
         seed: int = 42,
         logging_path: str = "./checkpoints",
         disable_tensorboard: bool = True,
         prediction_tags: Union[Dict, None] = None,
         seq2seq_params: Union[Dict, None] = None,
         layers_to_freeze: Union[str, None] = None,
         name_of_the_retrain_parser: Union[None, str] = None,
+        verbose: Union[None, bool] = None,
     ) -> List[Dict]:
         # pylint: disable=too-many-arguments, too-many-locals, too-many-branches, too-many-statements
 
         """
         Method to retrain the address parser model using a dataset with the same tags. We train using
         `experiment <https://poutyne.org/experiment.html>`_ from `poutyne <https://poutyne.org/index.html>`_
         framework. The experiment module allows us to save checkpoints (``ckpt``, in a pickle format) and a log.tsv
@@ -493,14 +518,20 @@
             callbacks (Union[list, None]): List of callbacks to use during training.
                 See Poutyne `callback <https://poutyne.org/callbacks.html#callback-class>`_ for more information. By
                 default, we set no callback.
             seed (int): The seed to use (default 42).
             logging_path (str): The logging path for the checkpoints. Poutyne will use the best one and reload the
                 state if any checkpoints are there. Thus, an error will be raised if you change the model type.
                 For example,  you retrain a FastText model and then retrain a BPEmb in the same logging path directory.
+                The logging_path can also be a S3-like (Azure, AWS, Google) bucket URI string path
+                (e.g. ``"s3://path/to/aws/s3/bucket.ckpt"``). Or it can be a ``S3Path`` S3-like URI using `cloudpathlib`
+                to handle S3-like bucket. See `cloudpathlib <https://cloudpathlib.drivendata.org/stable/>`
+                for detail on supported S3 buckets provider and URI condition.
+                If the logging_path is a S3 bucket, we will only save the best checkpoint to the S3 Bucket at the end
+                of training.
                 By default, the path is ``./checkpoints``.
             disable_tensorboard (bool): To disable Poutyne automatic Tensorboard monitoring. By default, we disable them
                 (true).
             prediction_tags (Union[dict, None]): A dictionary where the keys are the address components
                 (e.g. street name) and the values are the components indices (from 0 to N + 1) to use during retraining
                 of a model. The ``+ 1`` corresponds to the End Of Sequence (EOS) token that needs to be included in the
                 dictionary. We will use this dictionary's length for the prediction layer's output size.
@@ -538,14 +569,17 @@
                 Default settings for the parser name will use the training settings for the name using the
                 following pattern:
 
                     - the pretrained architecture (``'fasttext'`` or ``'bpemb'`` and if an attention mechanism is use),
                     - if prediction_tags is not ``None``, the following tag: ``ModifiedPredictionTags``,
                     - if seq2seq_params is not ``None``, the following tag: ``ModifiedSeq2SeqConfiguration``, and
                     - if layers_to_freeze is not ``None``, the following tag: ``FreezedLayer{portion}``.
+            verbose (Union[None, bool]): To override the AddressParser verbosity for the test. When set to True or
+                False, it will override (but it does not change the AddressParser verbosity) the test verbosity.
+                If set to the default value None, the AddressParser verbosity is used as the test verbosity.
 
 
         Return:
             A list of dictionaries with the best epoch stats (see `Experiment class
             <https://poutyne.org/experiment.html#poutyne.Experiment.train>`_ for details). The pretrained is
             saved using a default file name of using the name_of_the_retrain_parser. See the last note for
             more details.
@@ -738,14 +772,18 @@
             self.model,
             device=self.device,
             optimizer=optimizer,
             loss_function=nll_loss,
             batch_metrics=[accuracy],
         )
 
+        # Handle the verbose overriding param
+        if verbose is None:
+            verbose = self.verbose
+
         try:
             with_capturing_context = False
             if not valid_poutyne_version(min_major=1, min_minor=8):
                 print(
                     "You are using a older version of Poutyne that does not support properly error management."
                     " Due to that, we cannot show retrain progress. To fix that, update Poutyne to "
                     "the newest version."
@@ -756,14 +794,15 @@
                 train_generator=train_generator,
                 valid_generator=valid_generator,
                 epochs=epochs,
                 seed=seed,
                 callbacks=callbacks,
                 disable_tensorboard=disable_tensorboard,
                 capturing_context=with_capturing_context,
+                verbose=verbose,
             )
         except RuntimeError as error:
             list_of_file_path = os.listdir(path=".")
             if list_of_file_path:
                 if pretrained_parser_in_directory(logging_path):
                     # Mean we might already have checkpoint in the training directory
                     files_in_directory = get_files_in_directory(logging_path)
@@ -793,14 +832,15 @@
         else:
             file_name = (
                 name_of_the_retrain_parser + ".ckpt"
                 if name_of_the_retrain_parser is not None
                 else f"retrained_{self.model_type}_address_parser.ckpt"
             )
             file_path = os.path.join(logging_path, file_name)
+
             torch_save = {
                 "address_tagger_model": exp.model.network.state_dict(),
                 "model_type": self.model_type,
             }
 
             if seq2seq_params is not None:
                 # Means we have changed the seq2seq params
@@ -813,15 +853,37 @@
                 {
                     "named_parser": name_of_the_retrain_parser
                     if name_of_the_retrain_parser is not None
                     else self._formatted_named_parser_name(prediction_tags, seq2seq_params, layers_to_freeze)
                 }
             )
 
-            torch.save(torch_save, file_path)
+            if isinstance(file_path, S3Path):
+                # To handle CloudPath path_to_model_weights
+                try:
+                    with file_path.open("wb") as file:
+                        torch.save(torch_save, file)
+                except FileNotFoundError as error:
+                    raise FileNotFoundError("The file in the S3 bucket was not found.") from error
+
+            elif "s3://" in file_path:
+                file_path = CloudPath(file_path)
+                try:
+                    with file_path.open("wb") as file:
+                        torch.save(torch_save, file)
+                except FileNotFoundError as error:
+                    raise FileNotFoundError("The file in the S3 bucket was not found.") from error
+            else:
+                try:
+                    torch.save(torch_save, file_path)
+                except FileNotFoundError as error:
+                    if "s3" in file_path or "//" in file_path or ":" in file_path:
+                        raise FileNotFoundError(
+                            "Are You trying to use a AWS S3 URI? If so path need to start with s3://."
+                        ) from error
             return train_res
 
     def test(
         self,
         test_dataset_container: DatasetContainer,
         batch_size: int = 32,
         num_workers: int = 1,
@@ -1110,36 +1172,38 @@
 
     def _predict_pipeline(self, data: List) -> Tuple:
         """
         Pipeline to process data in a data loader for prediction.
         """
         return self.processor.process_for_inference(data)
 
-    @staticmethod
     def _retrain(
+        self,
         experiment: Experiment,
         train_generator: DatasetContainer,
         valid_generator: DatasetContainer,
         epochs: int,
         seed: int,
         callbacks: List,
         disable_tensorboard: bool,
         capturing_context: bool,
+        verbose: Union[None, bool],
     ) -> List[Dict]:
         # pylint: disable=too-many-arguments
         # If Poutyne 1.7 and before, we capture poutyne print since it print some exception.
         # Otherwise, we use a null context manager.
         with Capturing() if capturing_context else contextlib.nullcontext():
             train_res = experiment.train(
                 train_generator,
                 valid_generator=valid_generator,
                 epochs=epochs,
                 seed=seed,
                 callbacks=callbacks,
                 disable_tensorboard=disable_tensorboard,
+                verbose=verbose,
             )
         return train_res
 
     def _freeze_model_params(self, layers_to_freeze: Union[str]) -> None:
         layers_to_freeze = layers_to_freeze.lower()
         if layers_to_freeze not in ("encoder", "decoder", "prediction_layer", "seq2seq"):
             raise ValueError(
@@ -1246,14 +1310,17 @@
                 category=UserWarning,
             )
 
     def _apply_pre_processors(self, addresses: List[str]) -> List[str]:
         res = []
 
         for address in addresses:
+            processed_address = address
+
             for pre_processor in self.pre_processors:
                 processed_address = pre_processor(address)
-                res.append(" ".join(processed_address.split()))
+
+            res.append(" ".join(processed_address.split()))
         return res
 
     def is_same_model_type(self, other) -> bool:
         return self.model_type == other.model_type
```

### Comparing `deepparse-0.9.6/deepparse/parser/formatted_parsed_address.py` & `deepparse-0.9.7/deepparse/parser/formatted_parsed_address.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/parser/tools.py` & `deepparse-0.9.7/deepparse/parser/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import math
 import os
 from typing import List, OrderedDict, Tuple
 
+import math
 import numpy as np
 import torch
 
 
 def validate_if_new_prediction_tags(checkpoint_weights: dict) -> bool:
     return checkpoint_weights.get("prediction_tags") is not None
 
@@ -130,11 +130,14 @@
         model_type = inferred_model_type
     else:
         if "embedding_network.model.weight_ih_l0" in checkpoint_weights.keys():
             model_type = "bpemb"
         else:
             model_type = "fasttext"
 
-    if "decoder.linear_attention_mechanism_encoder_outputs.weight" in checkpoint_weights.keys():
+    if (
+        "decoder.linear_attention_mechanism_encoder_outputs.weight"
+        in checkpoint_weights.get("address_tagger_model").keys()
+    ):
         attention_mechanism = True
 
     return model_type, attention_mechanism
```

### Comparing `deepparse-0.9.6/deepparse/pre_processing/pre_processor.py` & `deepparse-0.9.7/deepparse/pre_processing/pre_processor.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/tools.py` & `deepparse-0.9.7/deepparse/tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/vectorizer/bpemb_vectorizer.py` & `deepparse-0.9.7/deepparse/vectorizer/bpemb_vectorizer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/vectorizer/fasttext_vectorizer.py` & `deepparse-0.9.7/deepparse/vectorizer/fasttext_vectorizer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/vectorizer/magnitude_vectorizer.py` & `deepparse-0.9.7/deepparse/vectorizer/magnitude_vectorizer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/vectorizer/vectorizer.py` & `deepparse-0.9.7/deepparse/vectorizer/vectorizer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse/vectorizer/vectorizer_factory.py` & `deepparse-0.9.7/deepparse/vectorizer/vectorizer_factory.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/deepparse.egg-info/PKG-INFO` & `deepparse-0.9.7/deepparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: deepparse
-Version: 0.9.6
+Version: 0.9.7
 Summary: A library for parsing multinational street addresses using deep learning.
 Home-page: https://deepparse.org/
-Download-URL: https://github.com/GRAAL-Research/deepparse/archive/v0.9.6.zip
+Download-URL: https://github.com/GRAAL-Research/deepparse/archive/v0.9.7.zip
 Author: Marouane Yassine, David Beauchemin
 Author-email: marouane.yassine.1@ulaval.ca, david.beauchemin.5@ulaval.ca
 License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
-Metadata-Version: 2.1 Name: deepparse Version: 0.9.6 Summary: A library for
+Metadata-Version: 2.1 Name: deepparse Version: 0.9.7 Summary: A library for
 parsing multinational street addresses using deep learning. Home-page: https://
 deepparse.org/ Download-URL: https://github.com/GRAAL-Research/deepparse/
-archive/v0.9.6.zip Author: Marouane Yassine, David Beauchemin Author-email:
+archive/v0.9.7.zip Author: Marouane Yassine, David Beauchemin Author-email:
 marouane.yassine.1@ulaval.ca, david.beauchemin.5@ulaval.ca License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Education Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 GNU Lesser General Public License v3 (LGPLv3) Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
```

### Comparing `deepparse-0.9.6/deepparse.egg-info/SOURCES.txt` & `deepparse-0.9.7/deepparse.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 deepparse/__init__.py
 deepparse/fasttext_tools.py
 deepparse/tools.py
 deepparse/version.py
-deepparse/weights_init.py
+deepparse/weights_tools.py
 deepparse.egg-info/PKG-INFO
 deepparse.egg-info/SOURCES.txt
 deepparse.egg-info/dependency_links.txt
 deepparse.egg-info/entry_points.txt
 deepparse.egg-info/requires.txt
 deepparse.egg-info/top_level.txt
 deepparse/cli/__init__.py
@@ -83,14 +83,15 @@
 settings/settings.py
 tests/__init__.py
 tests/base_capture_output.py
 tests/base_file_exist.py
 tests/test_fasttext_tools.py
 tests/test_integration_fasttext_tools.py
 tests/test_tools.py
+tests/test_weights_tools.py
 tests/tools.py
 tests/cli/__init__.py
 tests/cli/test_download_model.py
 tests/cli/test_download_models.py
 tests/cli/test_parse.py
 tests/cli/test_retrain.py
 tests/cli/test_testing.py
@@ -165,14 +166,15 @@
 tests/parser/integration/test_integration_address_parser_retrain_gpu.py
 tests/parser/integration/test_integration_address_parser_retrain_new_address_components.py
 tests/parser/integration/test_integration_address_parser_test_api.py
 tests/parser/integration/test_integration_address_parser_test_cpu.py
 tests/parser/integration/test_integration_address_parser_test_gpu.py
 tests/parser/integration/test_integration_reload_retrain_parser.py
 tests/parser/integration/test_integration_retrain_test_api_integration.py
+tests/parser/integration/test_integration_uri.py
 tests/pre_processing/__init__.py
 tests/pre_processing/test_address_cleaner.py
 tests/vectorizer/__init__.py
 tests/vectorizer/test_bpemb_vectorizer.py
 tests/vectorizer/test_fasttext_vectorizer.py
 tests/vectorizer/test_magnitude_vectorizer.py
 tests/vectorizer/test_vectorizer_factory.py
```

### Comparing `deepparse-0.9.6/models_evaluation/evaluate_model.py` & `deepparse-0.9.7/models_evaluation/evaluate_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/models_evaluation/generate_tables.py` & `deepparse-0.9.7/models_evaluation/generate_tables.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/models_evaluation/speed_test_evaluation.py` & `deepparse-0.9.7/models_evaluation/speed_test_evaluation.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/models_evaluation/timer/timer.py` & `deepparse-0.9.7/models_evaluation/timer/timer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/models_evaluation/tools.py` & `deepparse-0.9.7/models_evaluation/tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/setup.py` & `deepparse-0.9.7/setup.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/cli/test_download_model.py` & `deepparse-0.9.7/tests/cli/test_download_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/cli/test_download_models.py` & `deepparse-0.9.7/tests/cli/test_download_models.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/cli/test_parse.py` & `deepparse-0.9.7/tests/cli/test_parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,15 +260,15 @@
                     self.cpu_device,
                     "--path_to_retrained_model",
                     self.path_to_retrain_fasttext,
                 ]
             )
 
         expected_first_message = (
-            f"Parsing dataset file {self.fake_data_path_pickle} using the parser " f"PreTrainedFastTextAddressParser"
+            f"Parsing dataset file {self.fake_data_path_pickle} using the parser PreTrainedFastTextAddressParser"
         )
         actual_first_message = self._caplog.records[0].message
         self.assertEqual(expected_first_message, actual_first_message)
 
     def test_ifPathToFastTextRetrainModel_thenUseFastTextRetrainModel(self):
         with self._caplog.at_level(logging.INFO):
             path_to_retrained_model = self.path_to_retrain_fasttext
```

### Comparing `deepparse-0.9.6/tests/cli/test_retrain.py` & `deepparse-0.9.7/tests/cli/test_retrain.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/cli/test_testing.py` & `deepparse-0.9.7/tests/cli/test_testing.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/cli/test_tools.py` & `deepparse-0.9.7/tests/cli/test_tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/comparer/test_addresses_comparer.py` & `deepparse-0.9.7/tests/comparer/test_addresses_comparer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/comparer/test_formatted_compared_addresses.py` & `deepparse-0.9.7/tests/comparer/test_formatted_compared_addresses.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/comparer/test_formatted_compared_addresses_raw.py` & `deepparse-0.9.7/tests/comparer/test_formatted_compared_addresses_raw.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/comparer/test_formatted_compared_addresses_tags.py` & `deepparse-0.9.7/tests/comparer/test_formatted_compared_addresses_tags.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/converter/test_data_padder.py` & `deepparse-0.9.7/tests/converter/test_data_padder.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/converter/test_data_processor.py` & `deepparse-0.9.7/tests/converter/test_data_processor.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/converter/test_data_processor_factory.py` & `deepparse-0.9.7/tests/converter/test_data_processor_factory.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/converter/test_target_converter.py` & `deepparse-0.9.7/tests/converter/test_target_converter.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/data_validation/test_data_validation.py` & `deepparse-0.9.7/tests/data_validation/test_data_validation.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/dataset_container/test_dataset_container.py` & `deepparse-0.9.7/tests/dataset_container/test_dataset_container.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/dataset_container/test_tools.py` & `deepparse-0.9.7/tests/dataset_container/test_tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/embeddings_models/test_bpemb_embeddings_model.py` & `deepparse-0.9.7/tests/embeddings_models/test_bpemb_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/embeddings_models/test_embeddings_model.py` & `deepparse-0.9.7/tests/embeddings_models/test_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/embeddings_models/test_embeddings_model_factory.py` & `deepparse-0.9.7/tests/embeddings_models/test_embeddings_model_factory.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/embeddings_models/test_fasttext_embeddings_model.py` & `deepparse-0.9.7/tests/embeddings_models/test_fasttext_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/embeddings_models/test_magnitude_embeddings_model.py` & `deepparse-0.9.7/tests/embeddings_models/test_magnitude_embeddings_model.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/metrics/test_accuracy.py` & `deepparse-0.9.7/tests/metrics/test_accuracy.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/metrics/test_nll_loss.py` & `deepparse-0.9.7/tests/metrics/test_nll_loss.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/models_evaluation/test_tools_models_evaluation.py` & `deepparse-0.9.7/tests/models_evaluation/test_tools_models_evaluation.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/base.py` & `deepparse-0.9.7/tests/network/base.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/integration/base.py` & `deepparse-0.9.7/tests/network/integration/base.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/integration/test_integration_decoder.py` & `deepparse-0.9.7/tests/network/integration/test_integration_decoder.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/integration/test_integration_embedding_network.py` & `deepparse-0.9.7/tests/network/integration/test_integration_embedding_network.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/integration/test_integration_encoder.py` & `deepparse-0.9.7/tests/network/integration/test_integration_encoder.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/integration/test_integration_seq2seq_bpemb_model_cpu.py` & `deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_bpemb_model_cpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/integration/test_integration_seq2seq_bpemb_model_gpu.py` & `deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_bpemb_model_gpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/integration/test_integration_seq2seq_fasttext_model_cpu.py` & `deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_fasttext_model_cpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/integration/test_integration_seq2seq_fasttext_model_gpu.py` & `deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_fasttext_model_gpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/integration/test_integration_seq2seq_model_cpu.py` & `deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_model_cpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/integration/test_integration_seq2seq_model_gpu.py` & `deepparse-0.9.7/tests/network/integration/test_integration_seq2seq_model_gpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/test_bpemb_seq2seq_model_cpu.py` & `deepparse-0.9.7/tests/network/test_bpemb_seq2seq_model_cpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,52 +36,55 @@
         self.assertEqual(self.input_size, seq2seq_model.embedding_network.model.input_size)
         self.assertEqual(self.hidden_size, seq2seq_model.embedding_network.model.hidden_size)
         self.assertEqual(
             self.projection_size,
             seq2seq_model.embedding_network.projection_layer.out_features,
         )
 
+    @patch("deepparse.weights_tools.torch")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_givenNotLocalWeights_whenInstantiatingABPEmbSeq2SeqModel_thenShouldDownloadWeights(
-        self, load_state_dict_mock, torch_mock, isfile_mock
+        self, load_state_dict_mock, torch_mock, isfile_mock, torch_load_mock
     ):
         isfile_mock.return_value = False
         with patch("deepparse.network.seq2seq.download_weights") as download_weights_mock:
             BPEmbSeq2SeqModel(self.cache_dir, self.a_cpu_device, output_size=self.output_size, verbose=self.verbose)
             download_weights_mock.assert_called_with(self.model_type, self.a_root_path, verbose=self.verbose)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_givenLocalWeightsNotLastVersion_whenInstantiatingABPEmbSeq2SeqModel_thenShouldDownloadWeights(
-        self, load_state_dict_mock, torch_mock, isfile_mock, last_version_mock
+        self, load_state_dict_mock, torch_mock, isfile_mock, last_version_mock, torch_load_mock
     ):
         isfile_mock.return_value = True
         last_version_mock.return_value = False
         with patch("deepparse.network.seq2seq.download_weights") as download_weights_mock:
             BPEmbSeq2SeqModel(self.cache_dir, self.a_cpu_device, output_size=self.output_size, verbose=self.verbose)
             download_weights_mock.assert_called_with(self.model_type, self.a_root_path, verbose=self.verbose)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_givenLocalWeights_whenInstantiatingABPEmbSeq2SeqModel_thenShouldntDownloadWeights(
-        self, load_state_dict_mock, torch_mock, isfile_mock, last_version_mock
+        self, load_state_dict_mock, torch_mock, isfile_mock, last_version_mock, torch_load_mock
     ):
         isfile_mock.return_value = True
         last_version_mock.return_value = True
         with patch("deepparse.network.seq2seq.download_weights") as download_weights_mock:
             BPEmbSeq2SeqModel(self.cache_dir, self.a_cpu_device, output_size=self.output_size, verbose=self.verbose)
             download_weights_mock.assert_not_called()
 
-    @patch("deepparse.network.seq2seq.torch")
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_givenRetrainedWeights_whenInstantiatingAFastTextSeq2SeqModel_thenShouldUseRetrainedWeights(
         self, load_state_dict_mock, torch_mock
     ):
         all_layers_params = MagicMock()
         torch_mock.load.return_value = all_layers_params
         BPEmbSeq2SeqModel(
@@ -91,56 +94,59 @@
             verbose=self.verbose,
             path_to_retrained_model=self.a_path_to_retrained_model,
         )
 
         torch_load_call = [call.load(self.a_path_to_retrained_model, map_location=self.a_cpu_device)]
         torch_mock.assert_has_calls(torch_load_call)
 
-        load_state_dict_call = [call(all_layers_params)]
-        load_state_dict_mock.assert_has_calls(load_state_dict_call)
+        load_state_dict_mock.assert_called()
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_whenInstantiateASeq2SeqModel_thenEncoderIsCalledOnce(
         self,
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         encoder_mock,
+        torch_load_mock,
     ):
         seq2seq_model = BPEmbSeq2SeqModel(self.cache_dir, self.a_cpu_device, self.output_size, self.verbose)
 
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
         encoder_mock.__call__().return_value = (MagicMock(), MagicMock())
         seq2seq_model._encoder_step(to_predict_mock, lengths_list, self.a_batch_size)
 
         encoder_call = [call()(to_predict_mock, lengths_list)]
 
         encoder_mock.assert_has_calls(encoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_whenInstantiateASeq2SeqModelNoTarget_thenDecoderIsCalled(
         self,
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
+        torch_load_mock,
     ):
         seq2seq_model = BPEmbSeq2SeqModel(
             self.cache_dir, self.a_cpu_device, output_size=self.output_size, verbose=self.verbose
         )
 
         decoder_input_mock, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=False)
 
@@ -159,28 +165,30 @@
 
         decoder_call = [
             call()(view_mock, decoder_hidden_mock, encoder_outputs, self.a_lengths_list)
         ] * self.a_longest_sequence_length
 
         decoder_mock.assert_has_calls(decoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_whenInstantiateASeq2SeqAttModelNoTarget_thenDecoderIsCalled(
         self,
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
+        torch_load_mock,
     ):
         seq2seq_model = BPEmbSeq2SeqModel(
             self.cache_dir,
             self.a_cpu_device,
             output_size=self.output_size,
             verbose=self.verbose,
             attention_mechanism=True,
@@ -203,14 +211,15 @@
 
         decoder_call = [
             call()(view_mock, decoder_hidden_mock, encoder_outputs, self.a_lengths_list)
         ] * self.a_longest_sequence_length
 
         decoder_mock.assert_has_calls(decoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.random.random")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
@@ -219,14 +228,15 @@
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         random_mock,
+        torch_load_mock,
     ):
         random_mock.return_value = self.a_value_lower_than_threshold
 
         seq2seq_model = BPEmbSeq2SeqModel(
             self.cache_dir, self.a_cpu_device, output_size=self.output_size, verbose=self.verbose
         )
 
@@ -250,14 +260,15 @@
                     self.a_transpose_target_vector[idx].view(1, self.a_batch_size, 1),
                     decoder_hidden_mock,
                 )
             )
 
         self.assert_has_calls_tensor_equals(decoder_mock, decoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
@@ -266,14 +277,15 @@
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         encoder_mock,
+        torch_load_mock,
     ):
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
 
         _, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=False)
         decomposition_lengths_mock = MagicMock()
 
         # we don't use the one of the setUp_decoder_mocks since we do the full loop
@@ -312,14 +324,15 @@
                                     decoder_hidden_mock,
                                     decoder_input_mock,
                                     lengths_list,
                                 )
                             ]
                         )
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.random.random")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
@@ -330,14 +343,15 @@
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         encoder_mock,
         random_mock,
+        torch_load_mock,
     ):
         random_mock.return_value = self.a_value_lower_than_threshold
 
         target_mock = MagicMock()
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
 
         # 1) We reset it later
@@ -376,14 +390,15 @@
                         decoder_input_mock,
                         lengths_list,
                     )
                 ]
             )
             target_mock.assert_has_calls([call.transpose(0, 1)])
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.random.random")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
@@ -394,14 +409,15 @@
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         encoder_mock,
         random_mock,
+        torch_load_mock,
     ):
         random_mock.return_value = self.a_value_lower_than_threshold
 
         target_mock = MagicMock()
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
 
         _, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=True)
```

### Comparing `deepparse-0.9.6/tests/network/test_bpemb_seq2seq_model_gpu.py` & `deepparse-0.9.7/tests/network/test_bpemb_seq2seq_model_gpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,52 +37,55 @@
         self.assertEqual(self.input_size, seq2seq_model.embedding_network.model.input_size)
         self.assertEqual(self.hidden_size, seq2seq_model.embedding_network.model.hidden_size)
         self.assertEqual(
             self.projection_size,
             seq2seq_model.embedding_network.projection_layer.out_features,
         )
 
+    @patch("deepparse.weights_tools.torch")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_givenNotLocalWeights_whenInstantiatingABPEmbSeq2SeqModel_thenShouldDownloadWeights(
-        self, load_state_dict_mock, torch_mock, isfile_mock
+        self, load_state_dict_mock, torch_mock, isfile_mock, torch_load_mock
     ):
         isfile_mock.return_value = False
         with patch("deepparse.network.seq2seq.download_weights") as download_weights_mock:
             BPEmbSeq2SeqModel(self.cache_dir, self.a_torch_device, output_size=self.output_size, verbose=self.verbose)
             download_weights_mock.assert_called_with(self.model_type, self.a_root_path, verbose=self.verbose)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_givenLocalWeightsNotLastVersion_whenInstantiatingABPEmbSeq2SeqModel_thenShouldDownloadWeights(
-        self, load_state_dict_mock, torch_mock, isfile_mock, last_version_mock
+        self, load_state_dict_mock, torch_mock, isfile_mock, last_version_mock, torch_load_mock
     ):
         isfile_mock.return_value = True
         last_version_mock.return_value = False
         with patch("deepparse.network.seq2seq.download_weights") as download_weights_mock:
             BPEmbSeq2SeqModel(self.cache_dir, self.a_torch_device, output_size=self.output_size, verbose=self.verbose)
             download_weights_mock.assert_called_with(self.model_type, self.a_root_path, verbose=self.verbose)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_givenLocalWeights_whenInstantiatingABPEmbSeq2SeqModel_thenShouldntDownloadWeights(
-        self, load_state_dict_mock, torch_mock, isfile_mock, last_version_mock
+        self, load_state_dict_mock, torch_mock, isfile_mock, last_version_mock, torch_load_mock
     ):
         isfile_mock.return_value = True
         last_version_mock.return_value = True
         with patch("deepparse.network.seq2seq.download_weights") as download_weights_mock:
             BPEmbSeq2SeqModel(self.cache_dir, self.a_torch_device, output_size=self.output_size, verbose=self.verbose)
             download_weights_mock.assert_not_called()
 
-    @patch("deepparse.network.seq2seq.torch")
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_givenRetrainedWeights_whenInstantiatingAFastTextSeq2SeqModel_thenShouldUseRetrainedWeights(
         self, load_state_dict_mock, torch_mock
     ):
         all_layers_params = MagicMock()
         torch_mock.load.return_value = all_layers_params
         BPEmbSeq2SeqModel(
@@ -92,56 +95,59 @@
             verbose=self.verbose,
             path_to_retrained_model=self.a_path_to_retrained_model,
         )
 
         torch_load_call = [call.load(self.a_path_to_retrained_model, map_location=self.a_torch_device)]
         torch_mock.assert_has_calls(torch_load_call)
 
-        load_state_dict_call = [call(all_layers_params)]
-        load_state_dict_mock.assert_has_calls(load_state_dict_call)
+        load_state_dict_mock.assert_called()
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_whenInstantiateASeq2SeqModel_thenEncoderIsCalledOnce(
         self,
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         encoder_mock,
+        torch_load_mock,
     ):
         seq2seq_model = BPEmbSeq2SeqModel(self.cache_dir, self.a_torch_device, self.output_size, self.verbose)
 
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
         encoder_mock.__call__().return_value = (MagicMock(), MagicMock())
         seq2seq_model._encoder_step(to_predict_mock, lengths_list, self.a_batch_size)
 
         encoder_call = [call()(to_predict_mock, lengths_list)]
 
         encoder_mock.assert_has_calls(encoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_whenInstantiateASeq2SeqModelNoTarget_thenDecoderIsCalled(
         self,
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
+        torch_load_mock,
     ):
         seq2seq_model = BPEmbSeq2SeqModel(
             self.cache_dir, self.a_torch_device, output_size=self.output_size, verbose=self.verbose
         )
 
         decoder_input_mock, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=False)
 
@@ -160,28 +166,30 @@
 
         decoder_call = [
             call()(view_mock, decoder_hidden_mock, encoder_outputs, self.a_lengths_list)
         ] * self.a_longest_sequence_length
 
         decoder_mock.assert_has_calls(decoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_whenInstantiateASeq2SeqAttModelNoTarget_thenDecoderIsCalled(
         self,
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
+        torch_load_mock,
     ):
         seq2seq_model = BPEmbSeq2SeqModel(
             self.cache_dir,
             self.a_torch_device,
             output_size=self.output_size,
             verbose=self.verbose,
             attention_mechanism=True,
@@ -204,14 +212,15 @@
 
         decoder_call = [
             call()(view_mock, decoder_hidden_mock, encoder_outputs, self.a_lengths_list)
         ] * self.a_longest_sequence_length
 
         decoder_mock.assert_has_calls(decoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.random.random")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
@@ -220,14 +229,15 @@
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         random_mock,
+        torch_load_mock,
     ):
         random_mock.return_value = self.a_value_lower_than_threshold
 
         seq2seq_model = BPEmbSeq2SeqModel(
             self.cache_dir, self.a_torch_device, output_size=self.output_size, verbose=self.verbose
         )
 
@@ -251,14 +261,15 @@
                     self.a_transpose_target_vector[idx].view(1, self.a_batch_size, 1),
                     decoder_hidden_mock,
                 )
             )
 
         self.assert_has_calls_tensor_equals(decoder_mock, decoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
@@ -267,14 +278,15 @@
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         encoder_mock,
+        torch_load_mock,
     ):
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
 
         _, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=False)
         decomposition_lengths_mock = MagicMock()
 
         # we don't use the one of the setUp_decoder_mocks since we do the full loop
@@ -308,14 +320,15 @@
                         decoder_hidden_mock,
                         decoder_input_mock,
                         lengths_list,
                     )
                 ]
             )
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.random.random")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
@@ -326,14 +339,15 @@
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         encoder_mock,
         random_mock,
+        torch_load_mock,
     ):
         random_mock.return_value = self.a_value_lower_than_threshold
 
         target_mock = MagicMock()
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
 
         # 1) We reset it later
@@ -372,14 +386,15 @@
                         decoder_input_mock,
                         lengths_list,
                     )
                 ]
             )
             target_mock.assert_has_calls([call.transpose(0, 1)])
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.random.random")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
@@ -390,14 +405,15 @@
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         encoder_mock,
         random_mock,
+        torch_load_mock,
     ):
         random_mock.return_value = self.a_value_lower_than_threshold
 
         target_mock = MagicMock()
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
 
         _, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=True)
```

### Comparing `deepparse-0.9.6/tests/network/test_decoder.py` & `deepparse-0.9.7/tests/network/test_decoder.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/test_embedding_network.py` & `deepparse-0.9.7/tests/network/test_embedding_network.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/test_encoder.py` & `deepparse-0.9.7/tests/network/test_encoder.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/test_fasttext_seq2seq_model_cpu.py` & `deepparse-0.9.7/tests/network/test_fasttext_seq2seq_model_gpu.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,123 +1,133 @@
 # Since we use patch we skip the unused argument error
 # We also skip protected-access since we test the encoder and decoder step
-# pylint: disable=W0613, protected-access, too-many-arguments, too-many-locals
 # Bug with PyTorch source code makes torch.tensor as not callable for pylint.
-# pylint: disable=not-callable
+# pylint: disable=unused-argument, protected-access, too-many-arguments, not-callable, too-many-locals
 
 # Pylint raise error for the call method mocking
 # pylint: disable=unnecessary-dunder-call
 
 import unittest
+from unittest import skipIf
 from unittest.mock import patch, call, MagicMock
 
 import torch
 
 from deepparse.network import FastTextSeq2SeqModel
 from tests.network.base import Seq2SeqTestCase
 
 
-class FasttextSeq2SeqCPUTest(Seq2SeqTestCase):
+@skipIf(not torch.cuda.is_available(), "no gpu available")
+class FasttextSeq2SeqGPUTest(Seq2SeqTestCase):
     @classmethod
     def setUpClass(cls):
-        super(FasttextSeq2SeqCPUTest, cls).setUpClass()
+        super(FasttextSeq2SeqGPUTest, cls).setUpClass()
         cls.model_type = "fasttext"
 
-        cls.a_target_vector = torch.tensor([[0, 1, 1, 4, 5, 8], [1, 0, 3, 8, 0, 0]], device=cls.a_cpu_device)
+        cls.a_target_vector = torch.tensor([[0, 1, 1, 4, 5, 8], [1, 0, 3, 8, 0, 0]], device=cls.a_torch_device)
         cls.a_transpose_target_vector = cls.a_target_vector.transpose(0, 1)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_givenNotLocalWeights_whenInstantiatingAFastTextSeq2SeqModel_thenShouldDownloadWeights(
-        self, load_state_dict_mock, torch_mock, isfile_mock
+        self, load_state_dict_mock, torch_mock, isfile_mock, torch_load_mock
     ):
         isfile_mock.return_value = False
         with patch("deepparse.network.seq2seq.download_weights") as download_weights_mock:
-            FastTextSeq2SeqModel(self.cache_dir, self.a_cpu_device, output_size=self.output_size, verbose=self.verbose)
+            FastTextSeq2SeqModel(
+                self.cache_dir, self.a_torch_device, output_size=self.output_size, verbose=self.verbose
+            )
             download_weights_mock.assert_called_with(self.model_type, self.a_root_path, verbose=self.verbose)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_givenLocalWeightsNotLastVersion_whenInstantiatingAFastTextSeq2SeqModel_thenShouldDownloadWeights(
-        self, load_state_dict_mock, torch_mock, isfile_mock, last_version_mock
+        self, load_state_dict_mock, torch_mock, isfile_mock, last_version_mock, torch_load_mock
     ):
         isfile_mock.return_value = True
         last_version_mock.return_value = False
         with patch("deepparse.network.seq2seq.download_weights") as download_weights_mock:
-            FastTextSeq2SeqModel(self.cache_dir, self.a_cpu_device, output_size=self.output_size, verbose=self.verbose)
+            FastTextSeq2SeqModel(
+                self.cache_dir, self.a_torch_device, output_size=self.output_size, verbose=self.verbose
+            )
             download_weights_mock.assert_called_with(self.model_type, self.a_root_path, verbose=self.verbose)
 
-    @patch("deepparse.network.seq2seq.torch")
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_givenRetrainedWeights_whenInstantiatingAFastTextSeq2SeqModel_thenShouldUseRetrainedWeights(
         self, load_state_dict_mock, torch_mock
     ):
         all_layers_params = MagicMock()
         torch_mock.load.return_value = all_layers_params
         FastTextSeq2SeqModel(
             self.cache_dir,
-            self.a_cpu_device,
+            self.a_torch_device,
             output_size=self.output_size,
             verbose=self.verbose,
             path_to_retrained_model=self.a_path_to_retrained_model,
         )
 
-        torch_load_call = [call.load(self.a_path_to_retrained_model, map_location=self.a_cpu_device)]
+        torch_load_call = [call.load(self.a_path_to_retrained_model, map_location=self.a_torch_device)]
         torch_mock.assert_has_calls(torch_load_call)
 
-        load_state_dict_call = [call(all_layers_params)]
-        load_state_dict_mock.assert_has_calls(load_state_dict_call)
+        load_state_dict_mock.assert_called()
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_whenInstantiateASeq2SeqModel_thenEncodeIsCalledOnce(
         self,
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         encoder_mock,
+        torch_load_mock,
     ):
-        seq2seq_model = FastTextSeq2SeqModel(self.cache_dir, self.a_cpu_device, self.output_size, self.verbose)
+        seq2seq_model = FastTextSeq2SeqModel(self.cache_dir, self.a_torch_device, self.output_size, self.verbose)
 
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
         encoder_mock.__call__().return_value = (MagicMock(), MagicMock())
 
         seq2seq_model._encoder_step(to_predict_mock, lengths_list, self.a_batch_size)
 
         encoder_call = [call()(to_predict_mock, lengths_list)]
 
         encoder_mock.assert_has_calls(encoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_whenInstantiateASeq2SeqModelNoTarget_thenDecoderIsCalled(
         self,
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
+        torch_load_mock,
     ):
         seq2seq_model = FastTextSeq2SeqModel(
             self.cache_dir,
-            self.a_cpu_device,
+            self.a_torch_device,
             output_size=self.output_size,
             verbose=self.verbose,
             attention_mechanism=False,
         )
 
         decoder_input_mock, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=True)
 
@@ -136,32 +146,34 @@
 
         decoder_call = [
             call()(view_mock, decoder_hidden_mock, encoder_outputs, self.a_lengths_list)
         ] * self.a_longest_sequence_length
 
         decoder_mock.assert_has_calls(decoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_whenInstantiateASeq2SeqAttModelNoTarget_thenDecoderIsCalled(
         self,
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
+        torch_load_mock,
     ):
         seq2seq_model = FastTextSeq2SeqModel(
             self.cache_dir,
-            self.a_cpu_device,
+            self.a_torch_device,
             output_size=self.output_size,
             verbose=self.verbose,
             attention_mechanism=True,
         )
 
         decoder_input_mock, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=True)
 
@@ -180,14 +192,15 @@
 
         decoder_call = [
             call()(view_mock, decoder_hidden_mock, encoder_outputs, self.a_lengths_list)
         ] * self.a_longest_sequence_length
 
         decoder_mock.assert_has_calls(decoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.random.random")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
@@ -196,19 +209,20 @@
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         random_mock,
+        torch_load_mock,
     ):
         random_mock.return_value = self.a_value_lower_than_threshold
 
         seq2seq_model = FastTextSeq2SeqModel(
-            self.cache_dir, self.a_cpu_device, output_size=self.output_size, verbose=self.verbose
+            self.cache_dir, self.a_torch_device, output_size=self.output_size, verbose=self.verbose
         )
 
         decoder_input_mock, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=False)
 
         encoder_outputs = MagicMock()
         seq2seq_model._decoder_step(
             decoder_input_mock,
@@ -227,14 +241,15 @@
                     self.a_transpose_target_vector[idx].view(1, self.a_batch_size, 1),
                     decoder_hidden_mock,
                 )
             )
 
         self.assert_has_calls_tensor_equals(decoder_mock, decoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
@@ -243,28 +258,29 @@
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         encoder_mock,
+        torch_load_mock,
     ):
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
 
         _, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=False)
 
         # we don't use the one of the setUp_decoder_mocks since we do the full loop
         decoder_input_mock = MagicMock()
         to_mock = MagicMock()
         torch_mock.zeros().new_full.return_value = to_mock
 
         # We mock the return of the decoder output
         encoder_mock.__call__().return_value = (decoder_input_mock, decoder_hidden_mock)
 
-        seq2seq_model = FastTextSeq2SeqModel(self.cache_dir, self.a_cpu_device, self.output_size, self.verbose)
+        seq2seq_model = FastTextSeq2SeqModel(self.cache_dir, self.a_torch_device, self.output_size, self.verbose)
 
         seq2seq_model.forward(to_predict=to_predict_mock, lengths=lengths_list, target=None)
 
         encoder_mock.assert_has_calls([call()(to_predict_mock, lengths_list)])
 
         decoder_mock.assert_has_calls(
             [
@@ -273,14 +289,15 @@
                     decoder_hidden_mock,
                     decoder_input_mock,
                     lengths_list,
                 )
             ]
         )
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.random.random")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
@@ -291,14 +308,15 @@
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         encoder_mock,
         random_mock,
+        torch_load_mock,
     ):
         random_mock.return_value = self.a_value_lower_than_threshold
 
         target_mock = MagicMock()
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
 
         _, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=False)
@@ -307,15 +325,15 @@
         decoder_input_mock = MagicMock()
         to_mock = MagicMock()
         torch_mock.zeros().new_full.return_value = to_mock
 
         # We mock the return of the decoder output
         encoder_mock.__call__().return_value = (decoder_input_mock, decoder_hidden_mock)
 
-        seq2seq_model = FastTextSeq2SeqModel(self.cache_dir, self.a_cpu_device, self.output_size, self.verbose)
+        seq2seq_model = FastTextSeq2SeqModel(self.cache_dir, self.a_torch_device, self.output_size, self.verbose)
 
         seq2seq_model.forward(
             to_predict=to_predict_mock,
             lengths=lengths_list,
             target=target_mock,
         )
 
@@ -329,14 +347,15 @@
                     decoder_input_mock,
                     lengths_list,
                 )
             ]
         )
         target_mock.assert_has_calls([call.transpose(0, 1)])
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.random.random")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
@@ -347,14 +366,15 @@
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         encoder_mock,
         random_mock,
+        torch_load_mock,
     ):
         random_mock.return_value = self.a_value_lower_than_threshold
 
         target_mock = MagicMock()
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
 
         _, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=True)
@@ -362,16 +382,21 @@
         # we don't use the one of the setUp_decoder_mocks since we do the full loop
         decoder_input_mock = MagicMock()
         to_mock = MagicMock()
         torch_mock.zeros().new_full.return_value = to_mock
 
         # We mock the return of the decoder output
         encoder_mock.__call__().return_value = (decoder_input_mock, decoder_hidden_mock)
+
         seq2seq_model = FastTextSeq2SeqModel(
-            self.cache_dir, self.a_cpu_device, self.output_size, self.verbose, attention_mechanism=True
+            self.cache_dir,
+            self.a_torch_device,
+            self.output_size,
+            self.verbose,
+            attention_mechanism=True,
         )
 
         seq2seq_model.forward(
             to_predict=to_predict_mock,
             lengths=lengths_list,
             target=target_mock,
         )
```

### Comparing `deepparse-0.9.6/tests/network/test_fasttext_seq2seq_model_gpu.py` & `deepparse-0.9.7/tests/network/test_fasttext_seq2seq_model_cpu.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,128 +1,128 @@
 # Since we use patch we skip the unused argument error
 # We also skip protected-access since we test the encoder and decoder step
+# pylint: disable=W0613, protected-access, too-many-arguments, too-many-locals
 # Bug with PyTorch source code makes torch.tensor as not callable for pylint.
-# pylint: disable=unused-argument, protected-access, too-many-arguments, not-callable, too-many-locals
+# pylint: disable=not-callable
 
 # Pylint raise error for the call method mocking
 # pylint: disable=unnecessary-dunder-call
 
 import unittest
-from unittest import skipIf
 from unittest.mock import patch, call, MagicMock
 
 import torch
 
 from deepparse.network import FastTextSeq2SeqModel
 from tests.network.base import Seq2SeqTestCase
 
 
-@skipIf(not torch.cuda.is_available(), "no gpu available")
-class FasttextSeq2SeqGPUTest(Seq2SeqTestCase):
+class FasttextSeq2SeqCPUTest(Seq2SeqTestCase):
     @classmethod
     def setUpClass(cls):
-        super(FasttextSeq2SeqGPUTest, cls).setUpClass()
+        super(FasttextSeq2SeqCPUTest, cls).setUpClass()
         cls.model_type = "fasttext"
 
-        cls.a_target_vector = torch.tensor([[0, 1, 1, 4, 5, 8], [1, 0, 3, 8, 0, 0]], device=cls.a_torch_device)
+        cls.a_target_vector = torch.tensor([[0, 1, 1, 4, 5, 8], [1, 0, 3, 8, 0, 0]], device=cls.a_cpu_device)
         cls.a_transpose_target_vector = cls.a_target_vector.transpose(0, 1)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_givenNotLocalWeights_whenInstantiatingAFastTextSeq2SeqModel_thenShouldDownloadWeights(
-        self, load_state_dict_mock, torch_mock, isfile_mock
+        self, load_state_dict_mock, torch_mock, isfile_mock, torch_load_mock
     ):
         isfile_mock.return_value = False
         with patch("deepparse.network.seq2seq.download_weights") as download_weights_mock:
-            FastTextSeq2SeqModel(
-                self.cache_dir, self.a_torch_device, output_size=self.output_size, verbose=self.verbose
-            )
+            FastTextSeq2SeqModel(self.cache_dir, self.a_cpu_device, output_size=self.output_size, verbose=self.verbose)
             download_weights_mock.assert_called_with(self.model_type, self.a_root_path, verbose=self.verbose)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_givenLocalWeightsNotLastVersion_whenInstantiatingAFastTextSeq2SeqModel_thenShouldDownloadWeights(
-        self, load_state_dict_mock, torch_mock, isfile_mock, last_version_mock
+        self, load_state_dict_mock, torch_mock, isfile_mock, last_version_mock, torch_load_mock
     ):
         isfile_mock.return_value = True
         last_version_mock.return_value = False
         with patch("deepparse.network.seq2seq.download_weights") as download_weights_mock:
-            FastTextSeq2SeqModel(
-                self.cache_dir, self.a_torch_device, output_size=self.output_size, verbose=self.verbose
-            )
+            FastTextSeq2SeqModel(self.cache_dir, self.a_cpu_device, output_size=self.output_size, verbose=self.verbose)
             download_weights_mock.assert_called_with(self.model_type, self.a_root_path, verbose=self.verbose)
 
-    @patch("deepparse.network.seq2seq.torch")
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_givenRetrainedWeights_whenInstantiatingAFastTextSeq2SeqModel_thenShouldUseRetrainedWeights(
         self, load_state_dict_mock, torch_mock
     ):
         all_layers_params = MagicMock()
         torch_mock.load.return_value = all_layers_params
         FastTextSeq2SeqModel(
             self.cache_dir,
-            self.a_torch_device,
+            self.a_cpu_device,
             output_size=self.output_size,
             verbose=self.verbose,
             path_to_retrained_model=self.a_path_to_retrained_model,
         )
 
-        torch_load_call = [call.load(self.a_path_to_retrained_model, map_location=self.a_torch_device)]
+        torch_load_call = [call.load(self.a_path_to_retrained_model, map_location=self.a_cpu_device)]
         torch_mock.assert_has_calls(torch_load_call)
 
-        load_state_dict_call = [call(all_layers_params)]
-        load_state_dict_mock.assert_has_calls(load_state_dict_call)
+        load_state_dict_mock.assert_called()
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_whenInstantiateASeq2SeqModel_thenEncodeIsCalledOnce(
         self,
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         encoder_mock,
+        torch_load_mock,
     ):
-        seq2seq_model = FastTextSeq2SeqModel(self.cache_dir, self.a_torch_device, self.output_size, self.verbose)
+        seq2seq_model = FastTextSeq2SeqModel(self.cache_dir, self.a_cpu_device, self.output_size, self.verbose)
 
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
         encoder_mock.__call__().return_value = (MagicMock(), MagicMock())
 
         seq2seq_model._encoder_step(to_predict_mock, lengths_list, self.a_batch_size)
 
         encoder_call = [call()(to_predict_mock, lengths_list)]
 
         encoder_mock.assert_has_calls(encoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_whenInstantiateASeq2SeqModelNoTarget_thenDecoderIsCalled(
         self,
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
+        torch_load_mock,
     ):
         seq2seq_model = FastTextSeq2SeqModel(
             self.cache_dir,
-            self.a_torch_device,
+            self.a_cpu_device,
             output_size=self.output_size,
             verbose=self.verbose,
             attention_mechanism=False,
         )
 
         decoder_input_mock, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=True)
 
@@ -141,32 +141,34 @@
 
         decoder_call = [
             call()(view_mock, decoder_hidden_mock, encoder_outputs, self.a_lengths_list)
         ] * self.a_longest_sequence_length
 
         decoder_mock.assert_has_calls(decoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
     def test_whenInstantiateASeq2SeqAttModelNoTarget_thenDecoderIsCalled(
         self,
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
+        torch_load_mock,
     ):
         seq2seq_model = FastTextSeq2SeqModel(
             self.cache_dir,
-            self.a_torch_device,
+            self.a_cpu_device,
             output_size=self.output_size,
             verbose=self.verbose,
             attention_mechanism=True,
         )
 
         decoder_input_mock, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=True)
 
@@ -185,14 +187,15 @@
 
         decoder_call = [
             call()(view_mock, decoder_hidden_mock, encoder_outputs, self.a_lengths_list)
         ] * self.a_longest_sequence_length
 
         decoder_mock.assert_has_calls(decoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.random.random")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
@@ -201,19 +204,20 @@
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         random_mock,
+        torch_load_mock,
     ):
         random_mock.return_value = self.a_value_lower_than_threshold
 
         seq2seq_model = FastTextSeq2SeqModel(
-            self.cache_dir, self.a_torch_device, output_size=self.output_size, verbose=self.verbose
+            self.cache_dir, self.a_cpu_device, output_size=self.output_size, verbose=self.verbose
         )
 
         decoder_input_mock, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=False)
 
         encoder_outputs = MagicMock()
         seq2seq_model._decoder_step(
             decoder_input_mock,
@@ -232,14 +236,15 @@
                     self.a_transpose_target_vector[idx].view(1, self.a_batch_size, 1),
                     decoder_hidden_mock,
                 )
             )
 
         self.assert_has_calls_tensor_equals(decoder_mock, decoder_call)
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
     @patch("deepparse.network.seq2seq.Seq2SeqModel.load_state_dict")
@@ -248,28 +253,29 @@
         load_state_dict_mock,
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         encoder_mock,
+        torch_load_mock,
     ):
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
 
         _, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=False)
 
         # we don't use the one of the setUp_decoder_mocks since we do the full loop
         decoder_input_mock = MagicMock()
         to_mock = MagicMock()
         torch_mock.zeros().new_full.return_value = to_mock
 
         # We mock the return of the decoder output
         encoder_mock.__call__().return_value = (decoder_input_mock, decoder_hidden_mock)
 
-        seq2seq_model = FastTextSeq2SeqModel(self.cache_dir, self.a_torch_device, self.output_size, self.verbose)
+        seq2seq_model = FastTextSeq2SeqModel(self.cache_dir, self.a_cpu_device, self.output_size, self.verbose)
 
         seq2seq_model.forward(to_predict=to_predict_mock, lengths=lengths_list, target=None)
 
         encoder_mock.assert_has_calls([call()(to_predict_mock, lengths_list)])
 
         decoder_mock.assert_has_calls(
             [
@@ -278,14 +284,15 @@
                     decoder_hidden_mock,
                     decoder_input_mock,
                     lengths_list,
                 )
             ]
         )
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.random.random")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
@@ -296,14 +303,15 @@
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         encoder_mock,
         random_mock,
+        torch_load_mock,
     ):
         random_mock.return_value = self.a_value_lower_than_threshold
 
         target_mock = MagicMock()
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
 
         _, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=False)
@@ -312,15 +320,15 @@
         decoder_input_mock = MagicMock()
         to_mock = MagicMock()
         torch_mock.zeros().new_full.return_value = to_mock
 
         # We mock the return of the decoder output
         encoder_mock.__call__().return_value = (decoder_input_mock, decoder_hidden_mock)
 
-        seq2seq_model = FastTextSeq2SeqModel(self.cache_dir, self.a_torch_device, self.output_size, self.verbose)
+        seq2seq_model = FastTextSeq2SeqModel(self.cache_dir, self.a_cpu_device, self.output_size, self.verbose)
 
         seq2seq_model.forward(
             to_predict=to_predict_mock,
             lengths=lengths_list,
             target=target_mock,
         )
 
@@ -334,14 +342,15 @@
                     decoder_input_mock,
                     lengths_list,
                 )
             ]
         )
         target_mock.assert_has_calls([call.transpose(0, 1)])
 
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.random.random")
     @patch("deepparse.network.seq2seq.Encoder")
     @patch("deepparse.network.seq2seq.Decoder")
     @patch("deepparse.network.seq2seq.download_weights")
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
     @patch("deepparse.network.seq2seq.torch")
@@ -352,14 +361,15 @@
         torch_mock,
         isfile_mock,
         last_version_mock,
         download_weights_mock,
         decoder_mock,
         encoder_mock,
         random_mock,
+        torch_load_mock,
     ):
         random_mock.return_value = self.a_value_lower_than_threshold
 
         target_mock = MagicMock()
         to_predict_mock, lengths_list = self.setup_encoder_mocks()
 
         _, decoder_hidden_mock = self.setUp_decoder_mocks(decoder_mock, attention_mechanism=True)
@@ -367,21 +377,16 @@
         # we don't use the one of the setUp_decoder_mocks since we do the full loop
         decoder_input_mock = MagicMock()
         to_mock = MagicMock()
         torch_mock.zeros().new_full.return_value = to_mock
 
         # We mock the return of the decoder output
         encoder_mock.__call__().return_value = (decoder_input_mock, decoder_hidden_mock)
-
         seq2seq_model = FastTextSeq2SeqModel(
-            self.cache_dir,
-            self.a_torch_device,
-            self.output_size,
-            self.verbose,
-            attention_mechanism=True,
+            self.cache_dir, self.a_cpu_device, self.output_size, self.verbose, attention_mechanism=True
         )
 
         seq2seq_model.forward(
             to_predict=to_predict_mock,
             lengths=lengths_list,
             target=target_mock,
         )
```

### Comparing `deepparse-0.9.6/tests/network/test_model_factory.py` & `deepparse-0.9.7/tests/network/test_model_factory.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/network/test_seq2seq.py` & `deepparse-0.9.7/tests/network/test_seq2seq.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,15 +126,15 @@
         actual = seq2seq_model.output_size
         self.assertEqual(expected, actual)
 
         actual = seq2seq_model.decoder.linear.out_features
         self.assertEqual(expected, actual)
 
     @patch("os.path.isfile")
-    @patch("deepparse.network.seq2seq.torch")
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.torch.nn.Module.load_state_dict")
     def test_givenSeq2seqModel_whenNoPretrainedWeights_thenDownloadIt(
         self,
         torch_nn_mock,
         torch_mock,
         isfile_mock,
     ):
@@ -152,15 +152,15 @@
         with patch("deepparse.network.seq2seq.download_weights") as download_weights_mock:
             seq2seq_model._load_pre_trained_weights(self.a_model_type, cache_dir=self.cache_dir, offline=False)
 
             download_weights_mock.assert_called()
             download_weights_mock.assert_called_with(self.a_model_type, self.cache_dir, verbose=False)
 
     @patch("os.path.isfile")
-    @patch("deepparse.network.seq2seq.torch")
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.torch.nn.Module.load_state_dict")
     def test_givenSeq2seqModelVerbose_whenNoPretrainedWeights_thenWarns(
         self,
         torch_nn_mock,
         torch_mock,
         isfile_mock,
     ):
@@ -177,15 +177,15 @@
         isfile_mock.return_value = False
         with patch("deepparse.network.seq2seq.download_weights"):
             with self.assertWarns(UserWarning):
                 seq2seq_model._load_pre_trained_weights(self.a_model_type, cache_dir=self.cache_dir, offline=False)
 
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
-    @patch("deepparse.network.seq2seq.torch")
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.torch.nn.Module.load_state_dict")
     @skipIf(not torch.cuda.is_available(), "no gpu available")
     def test_givenSeq2seqModel_whenLoadPreTrainedWeightsNotRecentVersion_thenDownloadIt(
         self, torch_nn_mock, torch_mock, isfile_mock, last_version_mock
     ):
         seq2seq_model = Seq2SeqModel(
             self.a_torch_device,
@@ -202,15 +202,15 @@
         with patch("deepparse.network.seq2seq.download_weights") as download_weights_mock:
             seq2seq_model._load_pre_trained_weights(self.a_model_type, cache_dir=self.cache_dir, offline=False)
             download_weights_mock.assert_called()
             download_weights_mock.assert_called_with(self.a_model_type, self.cache_dir, verbose=True)
 
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
-    @patch("deepparse.network.seq2seq.torch")
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.torch.nn.Module.load_state_dict")
     @skipIf(not torch.cuda.is_available(), "no gpu available")
     def test_givenSeq2seqModel_whenLoadPreTrainedWeightsVerboseGPU_thenWarningsRaised(
         self, torch_nn_mock, torch_mock, isfile_mock, last_version_mock
     ):
         seq2seq_model = Seq2SeqModel(
             self.a_torch_device,
@@ -226,15 +226,15 @@
         last_version_mock.return_value = False
         with patch("deepparse.network.seq2seq.download_weights"):
             with self.assertWarns(UserWarning):
                 seq2seq_model._load_pre_trained_weights(self.a_model_type, cache_dir=self.cache_dir, offline=False)
 
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
-    @patch("deepparse.network.seq2seq.torch")
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.torch.nn.Module.load_state_dict")
     def test_givenSeq2seqModel_whenLoadPreTrainedWeightsNotVerboseGPU_thenWarningsNotRaised(
         self, torch_nn_mock, torch_mock, isfile_mock, last_version_mock
     ):
         seq2seq_model = Seq2SeqModel(
             self.a_cpu_device,
             input_size=self.encoder_input_size_dim,
@@ -250,15 +250,15 @@
         with patch("deepparse.network.seq2seq.download_weights"):
             with pytest.warns(None) as record:
                 seq2seq_model._load_pre_trained_weights(self.a_model_type, cache_dir=self.cache_dir, offline=False)
             self.assertEqual(0, len(record))
 
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
-    @patch("deepparse.network.seq2seq.torch")
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.torch.nn.Module.load_state_dict")
     def test_givenSeq2seqModel_whenLoadPreTrainedWeightsVerboseCPU_thenWarningsRaised(
         self, torch_nn_mock, torch_mock, isfile_mock, last_version_mock
     ):
         seq2seq_model = Seq2SeqModel(
             self.a_cpu_device,
             input_size=self.encoder_input_size_dim,
@@ -273,15 +273,15 @@
         last_version_mock.return_value = False
         with patch("deepparse.network.seq2seq.download_weights"):
             with self.assertWarns(UserWarning):
                 seq2seq_model._load_pre_trained_weights(self.a_model_type, cache_dir=self.cache_dir, offline=False)
 
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
-    @patch("deepparse.network.seq2seq.torch")
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.torch.nn.Module.load_state_dict")
     def test_givenSeq2seqModel_whenLoadPreTrainedWeightsNotVerboseCPU_thenWarningsNotRaised(
         self, torch_nn_mock, torch_mock, isfile_mock, last_version_mock
     ):
         seq2seq_model = Seq2SeqModel(
             self.a_cpu_device,
             input_size=self.encoder_input_size_dim,
@@ -295,15 +295,15 @@
         isfile_mock.return_value = True
         last_version_mock.return_value = False
         with patch("deepparse.network.seq2seq.download_weights"):
             with pytest.warns(None) as record:
                 seq2seq_model._load_pre_trained_weights(self.a_model_type, cache_dir=self.cache_dir, offline=False)
             self.assertEqual(0, len(record))
 
-    @patch("deepparse.network.seq2seq.torch")
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.torch.nn.Module.load_state_dict")
     def test_givenSeq2SeqModelRetrained_whenLoadRetrainedWeights_thenLoadProperly(self, torch_nn_mock, torch_mock):
         # pylint: disable=unnecessary-dunder-call
         all_layers_params_mock = MagicMock()
         all_layers_params_mock.__getitem__().__len__.return_value = self.decoder_output_size
         torch_mock.load.return_value = all_layers_params_mock
 
@@ -320,15 +320,15 @@
         seq2seq_model._load_weights(self.a_fake_retrain_path)
 
         torch_mock.assert_has_calls([call.load(self.a_fake_retrain_path, map_location=self.a_cpu_device)])
 
         torch_nn_mock.assert_called()
         torch_nn_mock.asser_has_calls([call(all_layers_params_mock)])
 
-    @patch("deepparse.network.seq2seq.torch")
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.torch.nn.Module.load_state_dict")
     def test_givenSeq2SeqModelRetrained_whenLoadRetrainedWeightsNewTagModel_thenLoadProperDict(
         self, torch_nn_mock, torch_mock
     ):
         # pylint: disable=unnecessary-dunder-call
 
         all_layers_params_mock = MagicMock(spec=dict)
@@ -347,15 +347,15 @@
         )
         seq2seq_model._load_weights(self.a_fake_retrain_path)
 
         all_layers_params_mock.get.assert_called()
 
     @patch("deepparse.network.seq2seq.latest_version")
     @patch("os.path.isfile")
-    @patch("deepparse.network.seq2seq.torch")
+    @patch("deepparse.weights_tools.torch")
     @patch("deepparse.network.seq2seq.torch.nn.Module.load_state_dict")
     def test_givenAnOfflineSeq2SeqModel_whenInit_thenDontCallOnlineFunctions(
         self, torch_nn_mock, torch_mock, isfile_mock, last_version_mock
     ):
         # Test if functions latest_version and download_weights
         seq2seq_model = Seq2SeqModel(
             self.a_cpu_device,
```

### Comparing `deepparse-0.9.6/tests/parser/base.py` & `deepparse-0.9.7/tests/parser/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,29 +26,29 @@
     @classmethod
     def prepare_pre_trained_weights(cls):
         cls.fake_cache_path = os.path.join(cls.model_weights_temp_dir.name, "fake_cache")
 
         path_to_default_model = os.path.join(os.path.expanduser("~"), ".cache", "deepparse", "fasttext.ckpt")
         default_checkpoint_weights = torch.load(path_to_default_model, map_location="cpu")
         checkpoint_weights = {
-            "address_tagger_model": default_checkpoint_weights,
+            "address_tagger_model": default_checkpoint_weights.get("address_tagger_model"),
             "model_type": "fasttext",
             "named_parser": "PreTrainedFastTextAddressParser",
         }
 
         cls.path_to_retrain_fasttext = os.path.join(
             cls.model_weights_temp_dir.name, "retrained_fasttext_address_parser.ckpt"
         )
         with open(cls.path_to_retrain_fasttext, "wb") as file:
             torch.save(checkpoint_weights, file)
 
         path_to_default_model = os.path.join(os.path.expanduser("~"), ".cache", "deepparse", "bpemb.ckpt")
         default_checkpoint_weights = torch.load(path_to_default_model, map_location="cpu")
         checkpoint_weights = {
-            "address_tagger_model": default_checkpoint_weights,
+            "address_tagger_model": default_checkpoint_weights.get("address_tagger_model"),
             "model_type": "bpemb",
             "named_parser": "PreTrainedBPEmbAddressParser",
         }
 
         cls.path_to_retrain_bpemb = os.path.join(cls.model_weights_temp_dir.name, "retrained_bpemb_address_parser.ckpt")
         with open(cls.path_to_retrain_bpemb, "wb") as file:
             torch.save(checkpoint_weights, file)
```

### Comparing `deepparse-0.9.6/tests/parser/integration/base_predict.py` & `deepparse-0.9.7/tests/parser/integration/base_predict.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,23 +16,25 @@
 from deepparse.parser import AddressParser, FormattedParsedAddress
 
 
 class AddressParserBase(TestCase):
     @classmethod
     def setUpClass(cls):
         cls.an_address_to_parse = "350 rue des lilas o"
+        cls.another_address_to_parse = "425 rue des lilas o"
 
     def setup_model_with_config(self, config):
         self.a_model = AddressParser(**config)
 
 
 class AddressParserPredictBase(AddressParserBase):
     def assert_properly_parse(self, parsed_address, multiple_address=False):
         if multiple_address:
             self.assertIsInstance(parsed_address, List)
+            self.assertNotEqual(parsed_address[0], parsed_address[1])
             parsed_address = parsed_address[0]
         self.assertIsInstance(parsed_address, FormattedParsedAddress)
 
     def tearDown(self) -> None:
         del self.a_model
```

### Comparing `deepparse-0.9.6/tests/parser/integration/base_retrain.py` & `deepparse-0.9.7/tests/parser/integration/base_retrain.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/integration/test_integration_address_parser.py` & `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_cpu.py` & `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_cpu.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,23 +100,23 @@
         parse_address = self.a_model(self.an_address_to_parse)
         self.assert_properly_parse(parse_address)
 
     def test_givenAListOfAddress_whenParseFastText_thenParseAllAddress(self):
         config = {"model_type": "fasttext", "device": self.device, "verbose": False}
         self.setup_model_with_config(config)
 
-        parse_address = self.a_model([self.an_address_to_parse, self.an_address_to_parse])
+        parse_address = self.a_model([self.an_address_to_parse, self.another_address_to_parse])
         self.assert_properly_parse(parse_address, multiple_address=True)
 
     def test_givenAListOfAddress_whenParseBPEmb_thenParseAllAddress(self):
         config = {"model_type": "bpemb", "device": self.device, "verbose": False}
         self.setup_model_with_config(config)
 
-        parse_address = self.a_model([self.an_address_to_parse, self.an_address_to_parse])
-        self.assert_properly_parse(parse_address, multiple_address=True)
+        parse_addresses = self.a_model([self.an_address_to_parse, self.another_address_to_parse])
+        self.assert_properly_parse(parse_addresses, multiple_address=True)
 
 
 # test if num_workers > 0 is correct for the data loader
 @skipIf(
     not os.path.exists(os.path.join(os.path.expanduser("~"), ".cache", "deepparse", "cc.fr.300.bin")),
     "download of model too long for test in runner",
 )
@@ -140,22 +140,22 @@
         parse_address = self.a_model(self.an_address_to_parse, num_workers=1)
         self.assert_properly_parse(parse_address)
 
     def test_givenAListOfAddress_whenParseFastTextNumWorkers1_thenParseAllAddress(self):
         config = {"model_type": "fasttext", "device": self.device, "verbose": False}
         self.setup_model_with_config(config)
 
-        parse_address = self.a_model([self.an_address_to_parse, self.an_address_to_parse], num_workers=1)
+        parse_address = self.a_model([self.an_address_to_parse, self.another_address_to_parse], num_workers=1)
         self.assert_properly_parse(parse_address, multiple_address=True)
 
     def test_givenAListOfAddress_whenParseBPEmbNumWorkers1_thenParseAllAddress(self):
         config = {"model_type": "bpemb", "device": self.device, "verbose": False}
         self.setup_model_with_config(config)
 
-        parse_address = self.a_model([self.an_address_to_parse, self.an_address_to_parse], num_workers=1)
+        parse_address = self.a_model([self.an_address_to_parse, self.another_address_to_parse], num_workers=1)
         self.assert_properly_parse(parse_address, multiple_address=True)
 
     def test_givenAAddress_whenParseFastTextNumWorkers2_thenParseAddress(self):
         config = {"model_type": "fasttext", "device": self.device, "verbose": False}
         self.setup_model_with_config(config)
 
         parse_address = self.a_model(self.an_address_to_parse, num_workers=2)
@@ -168,22 +168,22 @@
         parse_address = self.a_model(self.an_address_to_parse, num_workers=2)
         self.assert_properly_parse(parse_address)
 
     def test_givenAListOfAddress_whenParseFastTextNumWorkers2_thenParseAllAddress(self):
         config = {"model_type": "fasttext", "device": self.device, "verbose": False}
         self.setup_model_with_config(config)
 
-        parse_address = self.a_model([self.an_address_to_parse, self.an_address_to_parse], num_workers=2)
+        parse_address = self.a_model([self.an_address_to_parse, self.another_address_to_parse], num_workers=2)
         self.assert_properly_parse(parse_address, multiple_address=True)
 
     def test_givenAListOfAddress_whenParseBPEmbNumWorkers2_thenParseAllAddress(self):
         config = {"model_type": "bpemb", "device": self.device, "verbose": False}
         self.setup_model_with_config(config)
 
-        parse_address = self.a_model([self.an_address_to_parse, self.an_address_to_parse], num_workers=2)
+        parse_address = self.a_model([self.an_address_to_parse, self.another_address_to_parse], num_workers=2)
         self.assert_properly_parse(parse_address, multiple_address=True)
 
     def test_givenAAttentionModel_whenParseFastTextNumWorkers2_thenProperlyParseAddress(
         self,
     ):
         config = {
             "model_type": "fasttext",
```

### Comparing `deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_gpu.py` & `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_gpu.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,22 +53,22 @@
         parse_address = self.a_model(self.an_address_to_parse)
         self.assert_properly_parse(parse_address)
 
     def test_givenAListOfAddress_whenParseFastText_thenParseAllAddress(self):
         config = {"model_type": "fasttext", "device": self.device, "verbose": False}
         self.setup_model_with_config(config)
 
-        parse_address = self.a_model([self.an_address_to_parse, self.an_address_to_parse])
+        parse_address = self.a_model([self.an_address_to_parse, self.another_address_to_parse])
         self.assert_properly_parse(parse_address, multiple_address=True)
 
     def test_givenAListOfAddress_whenParseBPEmb_thenParseAllAddress(self):
         config = {"model_type": "bpemb", "device": self.device, "verbose": False}
         self.setup_model_with_config(config)
 
-        parse_address = self.a_model([self.an_address_to_parse, self.an_address_to_parse])
+        parse_address = self.a_model([self.an_address_to_parse, self.another_address_to_parse])
         self.assert_properly_parse(parse_address, multiple_address=True)
 
 
 # test if num_workers > 0 is correct for the data loader
 @skipIf(not torch.cuda.is_available(), "no gpu available")
 class AddressParserPredictGPUMultiProcessTest(AddressParserPredictBase):
     @classmethod
@@ -90,22 +90,22 @@
         parse_address = self.a_model(self.an_address_to_parse, num_workers=1)
         self.assert_properly_parse(parse_address)
 
     def test_givenAListOfAddress_whenParseFastTextNumWorkers1_thenParseAllAddress(self):
         config = {"model_type": "fasttext", "device": self.device, "verbose": False}
         self.setup_model_with_config(config)
 
-        parse_address = self.a_model([self.an_address_to_parse, self.an_address_to_parse], num_workers=1)
+        parse_address = self.a_model([self.an_address_to_parse, self.another_address_to_parse], num_workers=1)
         self.assert_properly_parse(parse_address, multiple_address=True)
 
     def test_givenAListOfAddress_whenParseBPEmbNumWorkers1_thenParseAllAddress(self):
         config = {"model_type": "bpemb", "device": self.device, "verbose": False}
         self.setup_model_with_config(config)
 
-        parse_address = self.a_model([self.an_address_to_parse, self.an_address_to_parse], num_workers=1)
+        parse_address = self.a_model([self.an_address_to_parse, self.another_address_to_parse], num_workers=1)
         self.assert_properly_parse(parse_address, multiple_address=True)
 
     def test_givenAAddress_whenParseFastTextNumWorkers2_thenParseAddress(self):
         config = {"model_type": "fasttext", "device": self.device, "verbose": False}
         self.setup_model_with_config(config)
 
         parse_address = self.a_model(self.an_address_to_parse, num_workers=2)
@@ -118,22 +118,22 @@
         parse_address = self.a_model(self.an_address_to_parse, num_workers=2)
         self.assert_properly_parse(parse_address)
 
     def test_givenAListOfAddress_whenParseFastTextNumWorkers2_thenParseAllAddress(self):
         config = {"model_type": "fasttext", "device": self.device, "verbose": False}
         self.setup_model_with_config(config)
 
-        parse_address = self.a_model([self.an_address_to_parse, self.an_address_to_parse], num_workers=2)
+        parse_address = self.a_model([self.an_address_to_parse, self.another_address_to_parse], num_workers=2)
         self.assert_properly_parse(parse_address, multiple_address=True)
 
     def test_givenAListOfAddress_whenParseBPEmbNumWorkers2_thenParseAllAddress(self):
         config = {"model_type": "bpemb", "device": self.device, "verbose": False}
         self.setup_model_with_config(config)
 
-        parse_address = self.a_model([self.an_address_to_parse, self.an_address_to_parse], num_workers=2)
+        parse_address = self.a_model([self.an_address_to_parse, self.another_address_to_parse], num_workers=2)
         self.assert_properly_parse(parse_address, multiple_address=True)
 
     def test_givenAAttentionModel_whenParseFastTextNumWorkers2_thenProperlyParseAddress(
         self,
     ):
         config = {
             "model_type": "fasttext",
```

### Comparing `deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_new_params.py` & `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_new_params.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_new_params_new_tags.py` & `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_new_params_new_tags.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_retrain_api.py` & `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_api.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_retrain_cpu.py` & `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_cpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_retrain_freeze_layers.py` & `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_freeze_layers.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_retrain_gpu.py` & `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_gpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_retrain_new_address_components.py` & `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_retrain_new_address_components.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_test_api.py` & `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_test_api.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_test_cpu.py` & `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_test_cpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/integration/test_integration_address_parser_test_gpu.py` & `deepparse-0.9.7/tests/parser/integration/test_integration_address_parser_test_gpu.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/integration/test_integration_reload_retrain_parser.py` & `deepparse-0.9.7/tests/parser/integration/test_integration_reload_retrain_parser.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/integration/test_integration_retrain_test_api_integration.py` & `deepparse-0.9.7/tests/parser/integration/test_integration_retrain_test_api_integration.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/test_address_parser.py` & `deepparse-0.9.7/tests/parser/test_address_parser.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/test_address_parser_retrain_api.py` & `deepparse-0.9.7/tests/parser/test_address_parser_retrain_api.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/test_address_parser_test_api.py` & `deepparse-0.9.7/tests/parser/test_address_parser_test_api.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/test_formatted_parsed_address.py` & `deepparse-0.9.7/tests/parser/test_formatted_parsed_address.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/test_tools.py` & `deepparse-0.9.7/tests/parser/test_tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/parser/test_user_fromatted_parsed_address.py` & `deepparse-0.9.7/tests/parser/test_user_fromatted_parsed_address.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/pre_processing/test_address_cleaner.py` & `deepparse-0.9.7/tests/pre_processing/test_address_cleaner.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/test_fasttext_tools.py` & `deepparse-0.9.7/tests/test_fasttext_tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/test_integration_fasttext_tools.py` & `deepparse-0.9.7/tests/test_integration_fasttext_tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/test_tools.py` & `deepparse-0.9.7/tests/test_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
 
 class ToolsTests(CaptureOutputTestCase, FileCreationTestCase):
     def setUp(self) -> None:
         self.temp_dir_obj = TemporaryDirectory()
         self.fake_cache_path = self.temp_dir_obj.name
         self.a_file_extension = "version"
-        self.latest_fasttext_version = "b4f098bb8909b1c8a8d24eea07df3435"
-        self.latest_bpemb_version = "ac0dc019748b6853dca412add7234203"
+        self.latest_fasttext_version = "f67a0517c70a314bdde0b8440f21139d"
+        self.latest_bpemb_version = "aa32fa918494b461202157c57734c374"
         self.a_seed = 42
         self.verbose = False
 
         self.a_model_type_checkpoint = "a_fake_model_type"
         self.a_fasttext_model_type_checkpoint = "fasttext"
         self.a_bpemb_model_type_checkpoint = "bpemb"
```

### Comparing `deepparse-0.9.6/tests/tools.py` & `deepparse-0.9.7/tests/tools.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/vectorizer/test_bpemb_vectorizer.py` & `deepparse-0.9.7/tests/vectorizer/test_bpemb_vectorizer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/vectorizer/test_fasttext_vectorizer.py` & `deepparse-0.9.7/tests/vectorizer/test_fasttext_vectorizer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/vectorizer/test_magnitude_vectorizer.py` & `deepparse-0.9.7/tests/vectorizer/test_magnitude_vectorizer.py`

 * *Files identical despite different names*

### Comparing `deepparse-0.9.6/tests/vectorizer/test_vectorizer_factory.py` & `deepparse-0.9.7/tests/vectorizer/test_vectorizer_factory.py`

 * *Files identical despite different names*

